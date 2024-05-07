# Comparing `tmp/nada_dsl-0.1.1-py3-none-any.whl.zip` & `tmp/nada_dsl-0.2.1-py3-none-any.whl.zip`

## zipinfo -v {}

 * *Differences in extra fields detected; using output from zipinfo -v*

```diff
@@ -1,41 +1,41 @@
 There is no zipfile comment.
 
 End-of-central-directory record:
 -------------------------------
 
-  Zip archive file size:                     27463 (0000000000006B47h)
-  Actual end-cent-dir record offset:         27441 (0000000000006B31h)
-  Expected end-cent-dir record offset:       27441 (0000000000006B31h)
+  Zip archive file size:                     45565 (000000000000B1FDh)
+  Actual end-cent-dir record offset:         45543 (000000000000B1E7h)
+  Expected end-cent-dir record offset:       45543 (000000000000B1E7h)
   (based on the length of the central directory and its expected offset)
 
   This zipfile constitutes the sole disk of a single-part archive; its
-  central directory contains 25 entries.
-  The central directory is 2405 (0000000000000965h) bytes long,
+  central directory contains 33 entries.
+  The central directory is 3159 (0000000000000C57h) bytes long,
   and its (expected) offset in bytes from the beginning of the zipfile
-  is 25036 (00000000000061CCh).
+  is 42384 (000000000000A590h).
 
 
 Central directory entry #1:
 ---------------------------
 
-  nada_dsl-0.1.1.dist-info/
+  nada_dsl-0.2.1.dist-info/
 
   offset of local header from start of archive:   0
                                                   (0000000000000000h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   1.0
   compression method:                             none (stored)
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Apr 3 09:47:58
-  file last modified on (UT extra field modtime): 2024 Apr 3 09:47:58 local
-  file last modified on (UT extra field modtime): 2024 Apr 3 09:47:58 UTC
+  file last modified on (DOS date/time):          2024 May 7 14:44:56
+  file last modified on (UT extra field modtime): 2024 May 7 14:44:55 local
+  file last modified on (UT extra field modtime): 2024 May 7 14:44:55 UTC
   32-bit CRC value (hex):                         00000000
   compressed size:                                0 bytes
   uncompressed size:                              0 bytes
   length of filename:                             25 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
@@ -50,28 +50,28 @@
     01 04 e9 03 00 00 04 e9 03 00 00.
 
   There is no file comment.
 
 Central directory entry #2:
 ---------------------------
 
-  nada_dsl-0.1.1.dist-info/top_level.txt
+  nada_dsl-0.2.1.dist-info/top_level.txt
 
   offset of local header from start of archive:   83
                                                   (0000000000000053h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   1.0
   compression method:                             none (stored)
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Apr 3 08:32:02
-  file last modified on (UT extra field modtime): 2024 Apr 3 08:32:02 local
-  file last modified on (UT extra field modtime): 2024 Apr 3 08:32:02 UTC
+  file last modified on (DOS date/time):          2024 May 3 11:44:24
+  file last modified on (UT extra field modtime): 2024 May 3 11:44:24 local
+  file last modified on (UT extra field modtime): 2024 May 3 11:44:24 UTC
   32-bit CRC value (hex):                         a3957946
   compressed size:                                9 bytes
   uncompressed size:                              9 bytes
   length of filename:                             38 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
@@ -86,32 +86,32 @@
     01 04 e9 03 00 00 04 e9 03 00 00.
 
   There is no file comment.
 
 Central directory entry #3:
 ---------------------------
 
-  nada_dsl-0.1.1.dist-info/RECORD
+  nada_dsl-0.2.1.dist-info/RECORD
 
   offset of local header from start of archive:   188
                                                   (00000000000000BCh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Apr 3 09:47:58
-  file last modified on (UT extra field modtime): 2024 Apr 3 09:47:58 local
-  file last modified on (UT extra field modtime): 2024 Apr 3 09:47:58 UTC
-  32-bit CRC value (hex):                         1a7a04c2
-  compressed size:                                981 bytes
-  uncompressed size:                              1719 bytes
+  file last modified on (DOS date/time):          2024 May 7 14:44:56
+  file last modified on (UT extra field modtime): 2024 May 7 14:44:55 local
+  file last modified on (UT extra field modtime): 2024 May 7 14:44:55 UTC
+  32-bit CRC value (hex):                         93d54a06
+  compressed size:                                1298 bytes
+  uncompressed size:                              2297 bytes
   length of filename:                             31 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
   Unix file attributes (100664 octal):            -rw-rw-r--
   MS-DOS file attributes (00 hex):                none
@@ -123,28 +123,28 @@
     01 04 e9 03 00 00 04 e9 03 00 00.
 
   There is no file comment.
 
 Central directory entry #4:
 ---------------------------
 
-  nada_dsl-0.1.1.dist-info/WHEEL
+  nada_dsl-0.2.1.dist-info/WHEEL
 
-  offset of local header from start of archive:   1258
-                                                  (00000000000004EAh) bytes
+  offset of local header from start of archive:   1575
+                                                  (0000000000000627h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   1.0
   compression method:                             none (stored)
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Apr 3 08:32:02
-  file last modified on (UT extra field modtime): 2024 Apr 3 08:32:02 local
-  file last modified on (UT extra field modtime): 2024 Apr 3 08:32:02 UTC
+  file last modified on (DOS date/time):          2024 May 3 11:44:24
+  file last modified on (UT extra field modtime): 2024 May 3 11:44:24 local
+  file last modified on (UT extra field modtime): 2024 May 3 11:44:24 UTC
   32-bit CRC value (hex):                         e0b8491e
   compressed size:                                92 bytes
   uncompressed size:                              92 bytes
   length of filename:                             30 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
@@ -159,29 +159,29 @@
     01 04 e9 03 00 00 04 e9 03 00 00.
 
   There is no file comment.
 
 Central directory entry #5:
 ---------------------------
 
-  nada_dsl-0.1.1.dist-info/LICENSE
+  nada_dsl-0.2.1.dist-info/LICENSE
 
-  offset of local header from start of archive:   1438
-                                                  (000000000000059Eh) bytes
+  offset of local header from start of archive:   1755
+                                                  (00000000000006DBh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Apr 3 08:32:02
-  file last modified on (UT extra field modtime): 2024 Apr 3 08:32:02 local
-  file last modified on (UT extra field modtime): 2024 Apr 3 08:32:02 UTC
+  file last modified on (DOS date/time):          2024 May 3 11:44:24
+  file last modified on (UT extra field modtime): 2024 May 3 11:44:24 local
+  file last modified on (UT extra field modtime): 2024 May 3 11:44:24 UTC
   32-bit CRC value (hex):                         6f45abe4
   compressed size:                                3944 bytes
   uncompressed size:                              11337 bytes
   length of filename:                             32 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
@@ -196,32 +196,32 @@
     01 04 e9 03 00 00 04 e9 03 00 00.
 
   There is no file comment.
 
 Central directory entry #6:
 ---------------------------
 
-  nada_dsl-0.1.1.dist-info/METADATA
+  nada_dsl-0.2.1.dist-info/METADATA
 
-  offset of local header from start of archive:   5472
-                                                  (0000000000001560h) bytes
+  offset of local header from start of archive:   5789
+                                                  (000000000000169Dh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Apr 3 09:47:58
-  file last modified on (UT extra field modtime): 2024 Apr 3 09:47:58 local
-  file last modified on (UT extra field modtime): 2024 Apr 3 09:47:58 UTC
-  32-bit CRC value (hex):                         16752d2f
-  compressed size:                                4620 bytes
-  uncompressed size:                              14148 bytes
+  file last modified on (DOS date/time):          2024 May 7 14:44:56
+  file last modified on (UT extra field modtime): 2024 May 7 14:44:55 local
+  file last modified on (UT extra field modtime): 2024 May 7 14:44:55 UTC
+  32-bit CRC value (hex):                         99938da8
+  compressed size:                                4509 bytes
+  uncompressed size:                              14009 bytes
   length of filename:                             33 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
   Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
@@ -235,26 +235,26 @@
   There is no file comment.
 
 Central directory entry #7:
 ---------------------------
 
   nada_dsl/
 
-  offset of local header from start of archive:   10183
-                                                  (00000000000027C7h) bytes
+  offset of local header from start of archive:   10389
+                                                  (0000000000002895h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   1.0
   compression method:                             none (stored)
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Apr 3 09:47:58
-  file last modified on (UT extra field modtime): 2024 Apr 3 09:47:58 local
-  file last modified on (UT extra field modtime): 2024 Apr 3 09:47:58 UTC
+  file last modified on (DOS date/time):          2024 May 7 14:44:56
+  file last modified on (UT extra field modtime): 2024 May 7 14:44:55 local
+  file last modified on (UT extra field modtime): 2024 May 7 14:44:55 UTC
   32-bit CRC value (hex):                         00000000
   compressed size:                                0 bytes
   uncompressed size:                              0 bytes
   length of filename:                             9 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
@@ -271,30 +271,30 @@
   There is no file comment.
 
 Central directory entry #8:
 ---------------------------
 
   nada_dsl/compile.py
 
-  offset of local header from start of archive:   10250
-                                                  (000000000000280Ah) bytes
+  offset of local header from start of archive:   10456
+                                                  (00000000000028D8h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Apr 3 08:29:10
-  file last modified on (UT extra field modtime): 2024 Apr 3 08:29:10 local
-  file last modified on (UT extra field modtime): 2024 Apr 3 08:29:10 UTC
-  32-bit CRC value (hex):                         a1ca370f
-  compressed size:                                888 bytes
-  uncompressed size:                              2615 bytes
+  file last modified on (DOS date/time):          2024 May 3 11:41:36
+  file last modified on (UT extra field modtime): 2024 May 3 11:41:36 local
+  file last modified on (UT extra field modtime): 2024 May 3 11:41:36 UTC
+  32-bit CRC value (hex):                         0ef1c3c7
+  compressed size:                                863 bytes
+  uncompressed size:                              2559 bytes
   length of filename:                             19 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
   Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
@@ -306,29 +306,66 @@
     01 04 e9 03 00 00 04 e9 03 00 00.
 
   There is no file comment.
 
 Central directory entry #9:
 ---------------------------
 
+  nada_dsl/audit_strict_test.py
+
+  offset of local header from start of archive:   11396
+                                                  (0000000000002C84h) bytes
+  file system or operating system of origin:      Unix
+  version of encoding software:                   3.0
+  minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
+  minimum software version required to extract:   2.0
+  compression method:                             deflated
+  compression sub-type (deflation):               normal
+  file security status:                           not encrypted
+  extended local header:                          no
+  file last modified on (DOS date/time):          2024 May 3 11:41:36
+  file last modified on (UT extra field modtime): 2024 May 3 11:41:36 local
+  file last modified on (UT extra field modtime): 2024 May 3 11:41:36 UTC
+  32-bit CRC value (hex):                         2ada852f
+  compressed size:                                904 bytes
+  uncompressed size:                              3040 bytes
+  length of filename:                             29 characters
+  length of extra field:                          24 bytes
+  length of file comment:                         0 characters
+  disk number on which file begins:               disk 1
+  apparent file type:                             text
+  Unix file attributes (100644 octal):            -rw-r--r--
+  MS-DOS file attributes (00 hex):                none
+
+  The central-directory extra field contains:
+  - A subfield with ID 0x5455 (universal time) and 5 data bytes.
+    The local extra field has UTC/GMT modification/access times.
+  - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
+    01 04 e9 03 00 00 04 e9 03 00 00.
+
+  There is no file comment.
+
+Central directory entry #10:
+---------------------------
+
   nada_dsl/source_ref.py
 
-  offset of local header from start of archive:   11215
-                                                  (0000000000002BCFh) bytes
+  offset of local header from start of archive:   12387
+                                                  (0000000000003063h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Apr 3 08:29:10
-  file last modified on (UT extra field modtime): 2024 Apr 3 08:29:10 local
-  file last modified on (UT extra field modtime): 2024 Apr 3 08:29:10 UTC
+  file last modified on (DOS date/time):          2024 May 3 11:41:36
+  file last modified on (UT extra field modtime): 2024 May 3 11:41:36 local
+  file last modified on (UT extra field modtime): 2024 May 3 11:41:36 UTC
   32-bit CRC value (hex):                         148987cb
   compressed size:                                726 bytes
   uncompressed size:                              2046 bytes
   length of filename:                             22 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
@@ -340,32 +377,32 @@
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e9 03 00 00 04 e9 03 00 00.
 
   There is no file comment.
 
-Central directory entry #10:
+Central directory entry #11:
 ---------------------------
 
   nada_dsl/errors.py
 
-  offset of local header from start of archive:   12021
-                                                  (0000000000002EF5h) bytes
+  offset of local header from start of archive:   13193
+                                                  (0000000000003389h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Apr 3 08:29:10
-  file last modified on (UT extra field modtime): 2024 Apr 3 08:29:10 local
-  file last modified on (UT extra field modtime): 2024 Apr 3 08:29:10 UTC
+  file last modified on (DOS date/time):          2024 May 3 11:41:36
+  file last modified on (UT extra field modtime): 2024 May 3 11:41:36 local
+  file last modified on (UT extra field modtime): 2024 May 3 11:41:36 UTC
   32-bit CRC value (hex):                         ce6214a4
   compressed size:                                84 bytes
   uncompressed size:                              99 bytes
   length of filename:                             18 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
@@ -377,35 +414,35 @@
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e9 03 00 00 04 e9 03 00 00.
 
   There is no file comment.
 
-Central directory entry #11:
+Central directory entry #12:
 ---------------------------
 
   nada_dsl/compile_test.py
 
-  offset of local header from start of archive:   12181
-                                                  (0000000000002F95h) bytes
+  offset of local header from start of archive:   13353
+                                                  (0000000000003429h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Apr 3 08:29:10
-  file last modified on (UT extra field modtime): 2024 Apr 3 08:29:10 local
-  file last modified on (UT extra field modtime): 2024 Apr 3 08:29:10 UTC
-  32-bit CRC value (hex):                         bbe641df
-  compressed size:                                266 bytes
-  uncompressed size:                              529 bytes
+  file last modified on (DOS date/time):          2024 May 3 11:41:36
+  file last modified on (UT extra field modtime): 2024 May 3 11:41:36 local
+  file last modified on (UT extra field modtime): 2024 May 3 11:41:36 UTC
+  32-bit CRC value (hex):                         f570d64e
+  compressed size:                                260 bytes
+  uncompressed size:                              512 bytes
   length of filename:                             24 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
   Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
@@ -414,32 +451,32 @@
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e9 03 00 00 04 e9 03 00 00.
 
   There is no file comment.
 
-Central directory entry #12:
+Central directory entry #13:
 ---------------------------
 
   nada_dsl/circuit_io.py
 
-  offset of local header from start of archive:   12529
-                                                  (00000000000030F1h) bytes
+  offset of local header from start of archive:   13695
+                                                  (000000000000357Fh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Apr 3 08:29:10
-  file last modified on (UT extra field modtime): 2024 Apr 3 08:29:10 local
-  file last modified on (UT extra field modtime): 2024 Apr 3 08:29:10 UTC
+  file last modified on (DOS date/time):          2024 May 3 11:41:36
+  file last modified on (UT extra field modtime): 2024 May 3 11:41:36 local
+  file last modified on (UT extra field modtime): 2024 May 3 11:41:36 UTC
   32-bit CRC value (hex):                         e4e155ab
   compressed size:                                575 bytes
   uncompressed size:                              1975 bytes
   length of filename:                             22 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
@@ -451,31 +488,31 @@
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e9 03 00 00 04 e9 03 00 00.
 
   There is no file comment.
 
-Central directory entry #13:
+Central directory entry #14:
 ---------------------------
 
   nada_dsl/future/
 
-  offset of local header from start of archive:   13184
-                                                  (0000000000003380h) bytes
+  offset of local header from start of archive:   14350
+                                                  (000000000000380Eh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   1.0
   compression method:                             none (stored)
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Apr 3 09:47:58
-  file last modified on (UT extra field modtime): 2024 Apr 3 09:47:58 local
-  file last modified on (UT extra field modtime): 2024 Apr 3 09:47:58 UTC
+  file last modified on (DOS date/time):          2024 May 7 14:44:56
+  file last modified on (UT extra field modtime): 2024 May 7 14:44:55 local
+  file last modified on (UT extra field modtime): 2024 May 7 14:44:55 UTC
   32-bit CRC value (hex):                         00000000
   compressed size:                                0 bytes
   uncompressed size:                              0 bytes
   length of filename:                             16 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
@@ -487,108 +524,108 @@
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e9 03 00 00 04 e9 03 00 00.
 
   There is no file comment.
 
-Central directory entry #14:
+Central directory entry #15:
 ---------------------------
 
   nada_dsl/future/__init__.py
 
-  offset of local header from start of archive:   13258
-                                                  (00000000000033CAh) bytes
+  offset of local header from start of archive:   14424
+                                                  (0000000000003858h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   1.0
   compression method:                             none (stored)
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Apr 3 08:29:10
-  file last modified on (UT extra field modtime): 2024 Apr 3 08:29:10 local
-  file last modified on (UT extra field modtime): 2024 Apr 3 08:29:10 UTC
+  file last modified on (DOS date/time):          2024 May 3 11:41:36
+  file last modified on (UT extra field modtime): 2024 May 3 11:41:36 local
+  file last modified on (UT extra field modtime): 2024 May 3 11:41:36 UTC
   32-bit CRC value (hex):                         00000000
   compressed size:                                0 bytes
   uncompressed size:                              0 bytes
   length of filename:                             27 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             binary
-  Unix file attributes (100664 octal):            -rw-rw-r--
+  Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
   The central-directory extra field contains:
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e9 03 00 00 04 e9 03 00 00.
 
   There is no file comment.
 
-Central directory entry #15:
+Central directory entry #16:
 ---------------------------
 
   nada_dsl/future/operations.py
 
-  offset of local header from start of archive:   13343
-                                                  (000000000000341Fh) bytes
+  offset of local header from start of archive:   14509
+                                                  (00000000000038ADh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Apr 3 08:29:10
-  file last modified on (UT extra field modtime): 2024 Apr 3 08:29:10 local
-  file last modified on (UT extra field modtime): 2024 Apr 3 08:29:10 UTC
+  file last modified on (DOS date/time):          2024 May 3 11:41:36
+  file last modified on (UT extra field modtime): 2024 May 3 11:41:36 local
+  file last modified on (UT extra field modtime): 2024 May 3 11:41:36 UTC
   32-bit CRC value (hex):                         ccdc42b1
   compressed size:                                115 bytes
   uncompressed size:                              214 bytes
   length of filename:                             29 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
-  Unix file attributes (100664 octal):            -rw-rw-r--
+  Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
   The central-directory extra field contains:
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e9 03 00 00 04 e9 03 00 00.
 
   There is no file comment.
 
-Central directory entry #16:
+Central directory entry #17:
 ---------------------------
 
   nada_dsl/__init__.py
 
-  offset of local header from start of archive:   13545
-                                                  (00000000000034E9h) bytes
+  offset of local header from start of archive:   14711
+                                                  (0000000000003977h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Apr 3 08:29:10
-  file last modified on (UT extra field modtime): 2024 Apr 3 08:29:10 local
-  file last modified on (UT extra field modtime): 2024 Apr 3 08:29:10 UTC
-  32-bit CRC value (hex):                         ac6a7a48
-  compressed size:                                133 bytes
-  uncompressed size:                              355 bytes
+  file last modified on (DOS date/time):          2024 May 3 11:41:36
+  file last modified on (UT extra field modtime): 2024 May 3 11:41:36 local
+  file last modified on (UT extra field modtime): 2024 May 3 11:41:36 UTC
+  32-bit CRC value (hex):                         0f5f6aa3
+  compressed size:                                137 bytes
+  uncompressed size:                              384 bytes
   length of filename:                             20 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
   Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
@@ -597,35 +634,35 @@
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e9 03 00 00 04 e9 03 00 00.
 
   There is no file comment.
 
-Central directory entry #17:
+Central directory entry #18:
 ---------------------------
 
   nada_dsl/compiler_frontend.py
 
-  offset of local header from start of archive:   13756
-                                                  (00000000000035BCh) bytes
+  offset of local header from start of archive:   14926
+                                                  (0000000000003A4Eh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Apr 3 08:29:10
-  file last modified on (UT extra field modtime): 2024 Apr 3 08:29:10 local
-  file last modified on (UT extra field modtime): 2024 Apr 3 08:29:10 UTC
-  32-bit CRC value (hex):                         9fe7cf94
-  compressed size:                                2649 bytes
-  uncompressed size:                              12074 bytes
+  file last modified on (DOS date/time):          2024 May 3 11:41:36
+  file last modified on (UT extra field modtime): 2024 May 3 11:41:36 local
+  file last modified on (UT extra field modtime): 2024 May 3 11:41:36 UTC
+  32-bit CRC value (hex):                         ee74141f
+  compressed size:                                2782 bytes
+  uncompressed size:                              15060 bytes
   length of filename:                             29 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
   Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
@@ -634,31 +671,289 @@
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e9 03 00 00 04 e9 03 00 00.
 
   There is no file comment.
 
-Central directory entry #18:
+Central directory entry #19:
+---------------------------
+
+  nada_dsl/audit/
+
+  offset of local header from start of archive:   17795
+                                                  (0000000000004583h) bytes
+  file system or operating system of origin:      Unix
+  version of encoding software:                   3.0
+  minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
+  minimum software version required to extract:   1.0
+  compression method:                             none (stored)
+  file security status:                           not encrypted
+  extended local header:                          no
+  file last modified on (DOS date/time):          2024 May 7 14:44:56
+  file last modified on (UT extra field modtime): 2024 May 7 14:44:55 local
+  file last modified on (UT extra field modtime): 2024 May 7 14:44:55 UTC
+  32-bit CRC value (hex):                         00000000
+  compressed size:                                0 bytes
+  uncompressed size:                              0 bytes
+  length of filename:                             15 characters
+  length of extra field:                          24 bytes
+  length of file comment:                         0 characters
+  disk number on which file begins:               disk 1
+  apparent file type:                             binary
+  Unix file attributes (040755 octal):            drwxr-xr-x
+  MS-DOS file attributes (10 hex):                dir 
+
+  The central-directory extra field contains:
+  - A subfield with ID 0x5455 (universal time) and 5 data bytes.
+    The local extra field has UTC/GMT modification/access times.
+  - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
+    01 04 e9 03 00 00 04 e9 03 00 00.
+
+  There is no file comment.
+
+Central directory entry #20:
+---------------------------
+
+  nada_dsl/audit/__main__.py
+
+  offset of local header from start of archive:   17868
+                                                  (00000000000045CCh) bytes
+  file system or operating system of origin:      Unix
+  version of encoding software:                   3.0
+  minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
+  minimum software version required to extract:   2.0
+  compression method:                             deflated
+  compression sub-type (deflation):               normal
+  file security status:                           not encrypted
+  extended local header:                          no
+  file last modified on (DOS date/time):          2024 May 3 11:41:36
+  file last modified on (UT extra field modtime): 2024 May 3 11:41:36 local
+  file last modified on (UT extra field modtime): 2024 May 3 11:41:36 UTC
+  32-bit CRC value (hex):                         906cb172
+  compressed size:                                84 bytes
+  uncompressed size:                              95 bytes
+  length of filename:                             26 characters
+  length of extra field:                          24 bytes
+  length of file comment:                         0 characters
+  disk number on which file begins:               disk 1
+  apparent file type:                             text
+  Unix file attributes (100644 octal):            -rw-r--r--
+  MS-DOS file attributes (00 hex):                none
+
+  The central-directory extra field contains:
+  - A subfield with ID 0x5455 (universal time) and 5 data bytes.
+    The local extra field has UTC/GMT modification/access times.
+  - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
+    01 04 e9 03 00 00 04 e9 03 00 00.
+
+  There is no file comment.
+
+Central directory entry #21:
+---------------------------
+
+  nada_dsl/audit/strict.py
+
+  offset of local header from start of archive:   18036
+                                                  (0000000000004674h) bytes
+  file system or operating system of origin:      Unix
+  version of encoding software:                   3.0
+  minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
+  minimum software version required to extract:   2.0
+  compression method:                             deflated
+  compression sub-type (deflation):               normal
+  file security status:                           not encrypted
+  extended local header:                          no
+  file last modified on (DOS date/time):          2024 May 3 11:41:36
+  file last modified on (UT extra field modtime): 2024 May 3 11:41:36 local
+  file last modified on (UT extra field modtime): 2024 May 3 11:41:36 UTC
+  32-bit CRC value (hex):                         d54bb426
+  compressed size:                                5276 bytes
+  uncompressed size:                              32922 bytes
+  length of filename:                             24 characters
+  length of extra field:                          24 bytes
+  length of file comment:                         0 characters
+  disk number on which file begins:               disk 1
+  apparent file type:                             text
+  Unix file attributes (100644 octal):            -rw-r--r--
+  MS-DOS file attributes (00 hex):                none
+
+  The central-directory extra field contains:
+  - A subfield with ID 0x5455 (universal time) and 5 data bytes.
+    The local extra field has UTC/GMT modification/access times.
+  - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
+    01 04 e9 03 00 00 04 e9 03 00 00.
+
+  There is no file comment.
+
+Central directory entry #22:
+---------------------------
+
+  nada_dsl/audit/abstract.py
+
+  offset of local header from start of archive:   23394
+                                                  (0000000000005B62h) bytes
+  file system or operating system of origin:      Unix
+  version of encoding software:                   3.0
+  minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
+  minimum software version required to extract:   2.0
+  compression method:                             deflated
+  compression sub-type (deflation):               normal
+  file security status:                           not encrypted
+  extended local header:                          no
+  file last modified on (DOS date/time):          2024 May 3 11:41:36
+  file last modified on (UT extra field modtime): 2024 May 3 11:41:36 local
+  file last modified on (UT extra field modtime): 2024 May 3 11:41:36 UTC
+  32-bit CRC value (hex):                         f0d0d195
+  compressed size:                                4914 bytes
+  uncompressed size:                              37770 bytes
+  length of filename:                             26 characters
+  length of extra field:                          24 bytes
+  length of file comment:                         0 characters
+  disk number on which file begins:               disk 1
+  apparent file type:                             text
+  Unix file attributes (100644 octal):            -rw-r--r--
+  MS-DOS file attributes (00 hex):                none
+
+  The central-directory extra field contains:
+  - A subfield with ID 0x5455 (universal time) and 5 data bytes.
+    The local extra field has UTC/GMT modification/access times.
+  - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
+    01 04 e9 03 00 00 04 e9 03 00 00.
+
+  There is no file comment.
+
+Central directory entry #23:
+---------------------------
+
+  nada_dsl/audit/__init__.py
+
+  offset of local header from start of archive:   28392
+                                                  (0000000000006EE8h) bytes
+  file system or operating system of origin:      Unix
+  version of encoding software:                   3.0
+  minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
+  minimum software version required to extract:   2.0
+  compression method:                             deflated
+  compression sub-type (deflation):               normal
+  file security status:                           not encrypted
+  extended local header:                          no
+  file last modified on (DOS date/time):          2024 May 3 11:41:36
+  file last modified on (UT extra field modtime): 2024 May 3 11:41:36 local
+  file last modified on (UT extra field modtime): 2024 May 3 11:41:36 UTC
+  32-bit CRC value (hex):                         2e13c551
+  compressed size:                                334 bytes
+  uncompressed size:                              672 bytes
+  length of filename:                             26 characters
+  length of extra field:                          24 bytes
+  length of file comment:                         0 characters
+  disk number on which file begins:               disk 1
+  apparent file type:                             text
+  Unix file attributes (100644 octal):            -rw-r--r--
+  MS-DOS file attributes (00 hex):                none
+
+  The central-directory extra field contains:
+  - A subfield with ID 0x5455 (universal time) and 5 data bytes.
+    The local extra field has UTC/GMT modification/access times.
+  - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
+    01 04 e9 03 00 00 04 e9 03 00 00.
+
+  There is no file comment.
+
+Central directory entry #24:
+---------------------------
+
+  nada_dsl/audit/common.py
+
+  offset of local header from start of archive:   28810
+                                                  (000000000000708Ah) bytes
+  file system or operating system of origin:      Unix
+  version of encoding software:                   3.0
+  minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
+  minimum software version required to extract:   2.0
+  compression method:                             deflated
+  compression sub-type (deflation):               normal
+  file security status:                           not encrypted
+  extended local header:                          no
+  file last modified on (DOS date/time):          2024 May 3 11:41:36
+  file last modified on (UT extra field modtime): 2024 May 3 11:41:36 local
+  file last modified on (UT extra field modtime): 2024 May 3 11:41:36 UTC
+  32-bit CRC value (hex):                         518a2e70
+  compressed size:                                1035 bytes
+  uncompressed size:                              2851 bytes
+  length of filename:                             24 characters
+  length of extra field:                          24 bytes
+  length of file comment:                         0 characters
+  disk number on which file begins:               disk 1
+  apparent file type:                             text
+  Unix file attributes (100644 octal):            -rw-r--r--
+  MS-DOS file attributes (00 hex):                none
+
+  The central-directory extra field contains:
+  - A subfield with ID 0x5455 (universal time) and 5 data bytes.
+    The local extra field has UTC/GMT modification/access times.
+  - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
+    01 04 e9 03 00 00 04 e9 03 00 00.
+
+  There is no file comment.
+
+Central directory entry #25:
+---------------------------
+
+  nada_dsl/audit/report.py
+
+  offset of local header from start of archive:   29927
+                                                  (00000000000074E7h) bytes
+  file system or operating system of origin:      Unix
+  version of encoding software:                   3.0
+  minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
+  minimum software version required to extract:   2.0
+  compression method:                             deflated
+  compression sub-type (deflation):               normal
+  file security status:                           not encrypted
+  extended local header:                          no
+  file last modified on (DOS date/time):          2024 May 3 11:41:36
+  file last modified on (UT extra field modtime): 2024 May 3 11:41:36 local
+  file last modified on (UT extra field modtime): 2024 May 3 11:41:36 UTC
+  32-bit CRC value (hex):                         2b1c81dc
+  compressed size:                                3022 bytes
+  uncompressed size:                              14124 bytes
+  length of filename:                             24 characters
+  length of extra field:                          24 bytes
+  length of file comment:                         0 characters
+  disk number on which file begins:               disk 1
+  apparent file type:                             text
+  Unix file attributes (100644 octal):            -rw-r--r--
+  MS-DOS file attributes (00 hex):                none
+
+  The central-directory extra field contains:
+  - A subfield with ID 0x5455 (universal time) and 5 data bytes.
+    The local extra field has UTC/GMT modification/access times.
+  - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
+    01 04 e9 03 00 00 04 e9 03 00 00.
+
+  There is no file comment.
+
+Central directory entry #26:
 ---------------------------
 
   nada_dsl/nada_types/
 
-  offset of local header from start of archive:   16492
-                                                  (000000000000406Ch) bytes
+  offset of local header from start of archive:   33031
+                                                  (0000000000008107h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   1.0
   compression method:                             none (stored)
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Apr 3 09:47:58
-  file last modified on (UT extra field modtime): 2024 Apr 3 09:47:58 local
-  file last modified on (UT extra field modtime): 2024 Apr 3 09:47:58 UTC
+  file last modified on (DOS date/time):          2024 May 7 14:44:56
+  file last modified on (UT extra field modtime): 2024 May 7 14:44:55 local
+  file last modified on (UT extra field modtime): 2024 May 7 14:44:55 UTC
   32-bit CRC value (hex):                         00000000
   compressed size:                                0 bytes
   uncompressed size:                              0 bytes
   length of filename:                             20 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
@@ -670,220 +965,220 @@
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e9 03 00 00 04 e9 03 00 00.
 
   There is no file comment.
 
-Central directory entry #19:
+Central directory entry #27:
 ---------------------------
 
   nada_dsl/nada_types/function.py
 
-  offset of local header from start of archive:   16570
-                                                  (00000000000040BAh) bytes
+  offset of local header from start of archive:   33109
+                                                  (0000000000008155h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Apr 3 08:29:10
-  file last modified on (UT extra field modtime): 2024 Apr 3 08:29:10 local
-  file last modified on (UT extra field modtime): 2024 Apr 3 08:29:10 UTC
+  file last modified on (DOS date/time):          2024 May 3 11:41:36
+  file last modified on (UT extra field modtime): 2024 May 3 11:41:36 local
+  file last modified on (UT extra field modtime): 2024 May 3 11:41:36 UTC
   32-bit CRC value (hex):                         b27912cc
   compressed size:                                884 bytes
   uncompressed size:                              2593 bytes
   length of filename:                             31 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
-  Unix file attributes (100664 octal):            -rw-rw-r--
+  Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
   The central-directory extra field contains:
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e9 03 00 00 04 e9 03 00 00.
 
   There is no file comment.
 
-Central directory entry #20:
+Central directory entry #28:
 ---------------------------
 
   nada_dsl/nada_types/types.py
 
-  offset of local header from start of archive:   17543
-                                                  (0000000000004487h) bytes
+  offset of local header from start of archive:   34082
+                                                  (0000000000008522h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Apr 3 08:29:10
-  file last modified on (UT extra field modtime): 2024 Apr 3 08:29:10 local
-  file last modified on (UT extra field modtime): 2024 Apr 3 08:29:10 UTC
-  32-bit CRC value (hex):                         f301962a
-  compressed size:                                2264 bytes
-  uncompressed size:                              59216 bytes
+  file last modified on (DOS date/time):          2024 May 3 11:41:36
+  file last modified on (UT extra field modtime): 2024 May 3 11:41:36 local
+  file last modified on (UT extra field modtime): 2024 May 3 11:41:36 UTC
+  32-bit CRC value (hex):                         70585cc0
+  compressed size:                                2817 bytes
+  uncompressed size:                              75321 bytes
   length of filename:                             28 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
-  Unix file attributes (100664 octal):            -rw-rw-r--
+  Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
   The central-directory extra field contains:
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e9 03 00 00 04 e9 03 00 00.
 
   There is no file comment.
 
-Central directory entry #21:
+Central directory entry #29:
 ---------------------------
 
   nada_dsl/nada_types/collections.py
 
-  offset of local header from start of archive:   19893
-                                                  (0000000000004DB5h) bytes
+  offset of local header from start of archive:   36985
+                                                  (0000000000009079h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Apr 3 08:29:10
-  file last modified on (UT extra field modtime): 2024 Apr 3 08:29:10 local
-  file last modified on (UT extra field modtime): 2024 Apr 3 08:29:10 UTC
+  file last modified on (DOS date/time):          2024 May 3 11:41:36
+  file last modified on (UT extra field modtime): 2024 May 3 11:41:36 local
+  file last modified on (UT extra field modtime): 2024 May 3 11:41:36 UTC
   32-bit CRC value (hex):                         506e4919
   compressed size:                                1275 bytes
   uncompressed size:                              6273 bytes
   length of filename:                             34 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
-  Unix file attributes (100664 octal):            -rw-rw-r--
+  Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
   The central-directory extra field contains:
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e9 03 00 00 04 e9 03 00 00.
 
   There is no file comment.
 
-Central directory entry #22:
+Central directory entry #30:
 ---------------------------
 
   nada_dsl/nada_types/generics.py
 
-  offset of local header from start of archive:   21260
-                                                  (000000000000530Ch) bytes
+  offset of local header from start of archive:   38352
+                                                  (00000000000095D0h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Apr 3 08:29:10
-  file last modified on (UT extra field modtime): 2024 Apr 3 08:29:10 local
-  file last modified on (UT extra field modtime): 2024 Apr 3 08:29:10 UTC
+  file last modified on (DOS date/time):          2024 May 3 11:41:36
+  file last modified on (UT extra field modtime): 2024 May 3 11:41:36 local
+  file last modified on (UT extra field modtime): 2024 May 3 11:41:36 UTC
   32-bit CRC value (hex):                         49e9623b
   compressed size:                                77 bytes
   uncompressed size:                              151 bytes
   length of filename:                             31 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
-  Unix file attributes (100664 octal):            -rw-rw-r--
+  Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
   The central-directory extra field contains:
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e9 03 00 00 04 e9 03 00 00.
 
   There is no file comment.
 
-Central directory entry #23:
+Central directory entry #31:
 ---------------------------
 
   nada_dsl/nada_types/__init__.py
 
-  offset of local header from start of archive:   21426
-                                                  (00000000000053B2h) bytes
+  offset of local header from start of archive:   38518
+                                                  (0000000000009676h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Apr 3 08:29:10
-  file last modified on (UT extra field modtime): 2024 Apr 3 08:29:10 local
-  file last modified on (UT extra field modtime): 2024 Apr 3 08:29:10 UTC
+  file last modified on (DOS date/time):          2024 May 3 11:41:36
+  file last modified on (UT extra field modtime): 2024 May 3 11:41:36 local
+  file last modified on (UT extra field modtime): 2024 May 3 11:41:36 UTC
   32-bit CRC value (hex):                         0df05c41
   compressed size:                                355 bytes
   uncompressed size:                              1103 bytes
   length of filename:                             31 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
-  Unix file attributes (100664 octal):            -rw-rw-r--
+  Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
   The central-directory extra field contains:
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e9 03 00 00 04 e9 03 00 00.
 
   There is no file comment.
 
-Central directory entry #24:
+Central directory entry #32:
 ---------------------------
 
   nada_dsl/compiler_frontend_test.py
 
-  offset of local header from start of archive:   21870
-                                                  (000000000000556Eh) bytes
+  offset of local header from start of archive:   38962
+                                                  (0000000000009832h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Apr 3 08:29:10
-  file last modified on (UT extra field modtime): 2024 Apr 3 08:29:10 local
-  file last modified on (UT extra field modtime): 2024 Apr 3 08:29:10 UTC
-  32-bit CRC value (hex):                         7dd33e4b
-  compressed size:                                2434 bytes
-  uncompressed size:                              13738 bytes
+  file last modified on (DOS date/time):          2024 May 3 11:41:36
+  file last modified on (UT extra field modtime): 2024 May 3 11:41:36 local
+  file last modified on (UT extra field modtime): 2024 May 3 11:41:36 UTC
+  32-bit CRC value (hex):                         5e8093c5
+  compressed size:                                2645 bytes
+  uncompressed size:                              15381 bytes
   length of filename:                             34 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
   Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
@@ -892,35 +1187,35 @@
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e9 03 00 00 04 e9 03 00 00.
 
   There is no file comment.
 
-Central directory entry #25:
+Central directory entry #33:
 ---------------------------
 
   nada_dsl/operations.py
 
-  offset of local header from start of archive:   24396
-                                                  (0000000000005F4Ch) bytes
+  offset of local header from start of archive:   41699
+                                                  (000000000000A2E3h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Apr 3 08:29:10
-  file last modified on (UT extra field modtime): 2024 Apr 3 08:29:10 local
-  file last modified on (UT extra field modtime): 2024 Apr 3 08:29:10 UTC
-  32-bit CRC value (hex):                         08c50a10
-  compressed size:                                560 bytes
-  uncompressed size:                              2549 bytes
+  file last modified on (DOS date/time):          2024 May 3 11:41:36
+  file last modified on (UT extra field modtime): 2024 May 3 11:41:36 local
+  file last modified on (UT extra field modtime): 2024 May 3 11:41:36 UTC
+  32-bit CRC value (hex):                         75908fbc
+  compressed size:                                605 bytes
+  uncompressed size:                              2732 bytes
   length of filename:                             22 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
   Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
```

## zipnote {}

```diff
@@ -1,31 +1,34 @@
-Filename: nada_dsl-0.1.1.dist-info/
+Filename: nada_dsl-0.2.1.dist-info/
 Comment: 
 
-Filename: nada_dsl-0.1.1.dist-info/top_level.txt
+Filename: nada_dsl-0.2.1.dist-info/top_level.txt
 Comment: 
 
-Filename: nada_dsl-0.1.1.dist-info/RECORD
+Filename: nada_dsl-0.2.1.dist-info/RECORD
 Comment: 
 
-Filename: nada_dsl-0.1.1.dist-info/WHEEL
+Filename: nada_dsl-0.2.1.dist-info/WHEEL
 Comment: 
 
-Filename: nada_dsl-0.1.1.dist-info/LICENSE
+Filename: nada_dsl-0.2.1.dist-info/LICENSE
 Comment: 
 
-Filename: nada_dsl-0.1.1.dist-info/METADATA
+Filename: nada_dsl-0.2.1.dist-info/METADATA
 Comment: 
 
 Filename: nada_dsl/
 Comment: 
 
 Filename: nada_dsl/compile.py
 Comment: 
 
+Filename: nada_dsl/audit_strict_test.py
+Comment: 
+
 Filename: nada_dsl/source_ref.py
 Comment: 
 
 Filename: nada_dsl/errors.py
 Comment: 
 
 Filename: nada_dsl/compile_test.py
@@ -45,14 +48,35 @@
 
 Filename: nada_dsl/__init__.py
 Comment: 
 
 Filename: nada_dsl/compiler_frontend.py
 Comment: 
 
+Filename: nada_dsl/audit/
+Comment: 
+
+Filename: nada_dsl/audit/__main__.py
+Comment: 
+
+Filename: nada_dsl/audit/strict.py
+Comment: 
+
+Filename: nada_dsl/audit/abstract.py
+Comment: 
+
+Filename: nada_dsl/audit/__init__.py
+Comment: 
+
+Filename: nada_dsl/audit/common.py
+Comment: 
+
+Filename: nada_dsl/audit/report.py
+Comment: 
+
 Filename: nada_dsl/nada_types/
 Comment: 
 
 Filename: nada_dsl/nada_types/function.py
 Comment: 
 
 Filename: nada_dsl/nada_types/types.py
```

## nada_dsl/compile.py

```diff
@@ -9,86 +9,89 @@
 import traceback
 import importlib.util
 import nada_dsl
 from nada_dsl.compiler_frontend import nada_compile
 
 
 @dataclass
-class CompileOutput:
+class CompilerOutput:
     """ Compiler Output
     """
     mir: str
-    nada_dsl_path: str
 
+def compile(script_path: str) -> CompilerOutput:
+    """Compiles a NADA program
 
-def transform_program(script_path: str) -> CompileOutput:
+    Args:
+        script_path (str): The nada program path
+
+    Returns:
+        CompilerOutput: The Compiler Output
+    """
     script_dir = os.path.dirname(script_path)
     sys.path.insert(0, script_dir)
     script_name = os.path.basename(script_path)
     if script_name.endswith(".py"):
         script_name = script_name[:-3]
 
     script = __import__(script_name)
 
     try:
         main = getattr(script, "nada_main")
     except:
         raise Exception("'nada_dsl' entrypoint function is missing in program " + script_name)
     outputs = main()
     compile_output = nada_compile(outputs)
-    nada_dsl_path = nada_dsl.__path__[0]
-    return CompileOutput(compile_output, nada_dsl_path)
+    return CompilerOutput(compile_output)
 
 
-def compile_string(script: str) -> CompileOutput:
-    """Compiles a NADA program as string
+def compile_string(script: str) -> CompilerOutput:
+    """Compiles a NADA program from a string
 
     Args:
         script (str): The nada program as a base64 encoded string (UTF-8)
 
     Returns:
-        CompileOutput: The Compiler Output
+        CompilerOutput: The Compiler Output
     """
     decoded_program = base64.b64decode(script).decode('utf-8')
     temp_name = 'temp_program'
     spec = importlib.util.spec_from_loader(temp_name, loader=None)
     module = importlib.util.module_from_spec(spec)
     exec(decoded_program, module.__dict__)
     sys.modules[temp_name] = module
     globals()[temp_name] = module
 
-    
     outputs = module.nada_main()
     compile_output = nada_compile(outputs)
-    nada_dsl_path = nada_dsl.__path__[0]
-    return CompileOutput(compile_output, nada_dsl_path)
+    return CompilerOutput(compile_output)
 
 
-def print_output(output: CompileOutput): 
+def print_output(output: CompilerOutput):
     """Prints compiler output
 
     Args:
-        output (CompileOutput): Output of the compiler
+        output (CompilerOutput): Output of the compiler
     """
     output_json = {
-            "result": "Success",
-            "mir": output.mir,
-            "nada_dsl_path": output.nada_dsl_path,
-        }
+        "result": "Success",
+        "mir": output.mir,
+    }
     print(json.dumps(output_json))
 
+
 if __name__ == "__main__":
     try:
         args_length = len(sys.argv)
         if args_length < 2:
             raise Exception("expected program as argument")
         if args_length == 2:
-            output = transform_program(sys.argv[1])
+            output = compile(sys.argv[1])
             print_output(output)
         if args_length == 3 and sys.argv[1] == '-s':
-            output = compile_string(sys.argv[2]) 
+            output = compile_string(sys.argv[2])
             print_output(output)
 
     except Exception as ex:
         tb = traceback.format_exc()
         output = {"result": "Failure", "reason": str(ex), "traceback": str(tb)}
         print(json.dumps(output))
```

## nada_dsl/compile_test.py

```diff
@@ -1,19 +1,20 @@
 """
 Compilation tests.
 """
 import os
 import json
-from nada_dsl.compile import transform_program
+from nada_dsl.compile import compile
+
 
 def get_test_programs_folder():
     file_path = os.path.realpath(__file__)
     this_directory = os.path.dirname(file_path)
-    return this_directory+'/../../test-programs/programs'
+    return this_directory + '/../../test-programs/programs'
 
 
 def test_compile_nada_fn_simple():
-    mir_str = transform_program(f'{get_test_programs_folder()}/nada_fn_simple.py').mir
+    mir_str = compile(f'{get_test_programs_folder()}/nada_fn_simple.py').mir
     assert mir_str != ""
     mir = json.loads(mir_str)
     mir_functions = mir['functions']
     assert len(mir_functions) == 1
```

## nada_dsl/__init__.py

```diff
@@ -1,10 +1,11 @@
 """
 Package exports.
 """
+from nada_dsl.audit import *
 from nada_dsl.source_ref import *
 from nada_dsl.nada_types.types import *
 from nada_dsl.nada_types.generics import *
 from nada_dsl.nada_types.function import *
 from nada_dsl.nada_types.collections import *
 from nada_dsl.operations import unzip
 from nada_dsl.circuit_io import *
```

## nada_dsl/compiler_frontend.py

```diff
@@ -33,20 +33,21 @@
     Power,
     RightShift,
     LeftShift,
     LessThan,
     GreaterThan,
     LessOrEqualThan,
     GreaterOrEqualThan,
-    Equals,
     PublicOutputEquality,
+    Equals,
     Unzip,
     Random,
     IfElse,
-    Reveal
+    Reveal,
+    TruncPr
 )
 
 from nada_dsl.nada_types.collections import (
     Map,
     Reduce,
     Zip,
 )
@@ -90,34 +91,36 @@
 
 def nada_dsl_to_nada_mir(outputs: List[Output]) -> Dict[str, Any]:
     """Convert Nada DSL to Nada MIR."""
     new_outputs = []
     PARTIES.clear()
     INPUTS.clear()
     LITERALS.clear()
+    instructions = {}
     for output in outputs:
-        new_out = process_operation(output.inner)
+        out_instruction_id = process_operation(output.inner, instructions)
         party = output.party
         PARTIES[party.name] = party
         new_outputs.append(
             {
-                "inner": new_out,
+                "instruction_id": out_instruction_id,
                 "name": output.name,
                 "party": party.name,
                 "type": to_type_dict(output.inner),
                 "source_ref": output.source_ref.to_dict(),
             }
         )
 
     return {
         "functions": to_function_list(FUNCTIONS),
         "parties": to_party_list(PARTIES),
         "inputs": to_input_list(INPUTS),
         "literals": to_literal_list(LITERALS),
         "outputs": new_outputs,
+        "instructions": instructions,
         "source_files": SourceRef.get_sources(),
     }
 
 
 def to_party_list(parties):
     """Convert parties to a list."""
     return [
@@ -199,203 +202,277 @@
         return to_type(op_wrapper.__class__.__name__)
 
 
 def to_type(name: str):
     """Convert a type name."""
     # Rename public variables so they are considered as the same as literals.
     if name.startswith("Public"):
-        name = name[len("Public") :].lstrip()
+        name = name[len("Public"):].lstrip()
         return name
     else:
         return name
 
 
 def to_fn_dict(fn: NadaFunction):
     """Convert a function to a dictionary."""
+
+    instructions = {}
+    op_id = process_operation(fn.inner, instructions)
     return {
         "id": fn.id,
         "args": [
             {
                 "name": arg.name,
                 "type": to_type_dict(arg.type),
                 "source_ref": arg.source_ref.to_dict(),
             }
             for arg in fn.args
         ],
         "function": fn.function.__name__,
-        "body": process_operation(fn.inner),
+        "return_instruction_id": op_id,
+        "instructions": instructions,
         "return_type": to_type_dict(fn.return_type),
         "source_ref": fn.source_ref.to_dict(),
     }
 
 
-def process_operation(operation_wrapper):
+def process_operation(operation_wrapper, instructions):
     """Process an operation."""
     from nada_dsl.nada_types.function import NadaFunctionArg
 
     ty = to_type_dict(operation_wrapper)
     operation = operation_wrapper.inner
 
     if isinstance(
-        operation,
-        (
-            Addition,
-            Subtraction,
-            Multiplication,
-            Division,
-            Modulo,
-            Power,
-            RightShift,
-            LeftShift,
-            LessThan,
-            GreaterThan,
-            GreaterOrEqualThan,
-            LessOrEqualThan,
-            Equals,
-            PublicOutputEquality,
-            Zip,
-        ),
+            operation,
+            (
+                    Addition,
+                    Subtraction,
+                    Multiplication,
+                    Division,
+                    Modulo,
+                    Power,
+                    RightShift,
+                    LeftShift,
+                    LessThan,
+                    GreaterThan,
+                    GreaterOrEqualThan,
+                    LessOrEqualThan,
+                    Equals,
+                    PublicOutputEquality,
+                    Zip,
+            ),
     ):
-        return {
+        op_id = id(operation)
+        op_instruction = {
             type(operation).__name__: {
-                "left": process_operation(operation.left),
-                "right": process_operation(operation.right),
+                "id": op_id,
+                "left": process_operation(operation.left, instructions),
+                "right": process_operation(operation.right, instructions),
                 "type": ty,
                 "source_ref": operation.source_ref.to_dict(),
             }
         }
+        instructions[op_id] = op_instruction
+        return op_id
 
     elif isinstance(operation, Cast):
-        return {
+        op_id = id(operation)
+        op_instruction = {
             "Cast": {
-                "target": process_operation(operation.target),
+                "id": op_id,
+                "target": process_operation(operation.target, instructions),
                 "to": operation.to.__name__,
                 "type": ty,
                 "source_ref": operation.source_ref.to_dict(),
             }
         }
+        instructions[op_id] = op_instruction
+        return op_id
     elif isinstance(operation, Input):
         party_name = operation.party.name
         PARTIES[party_name] = operation.party
         if party_name not in INPUTS:
             INPUTS[party_name] = {}
         if operation.name in INPUTS[party_name] and id(
-            INPUTS[party_name][operation.name][0]
+                INPUTS[party_name][operation.name][0]
         ) != id(operation):
             raise Exception(f"Input is duplicated: {operation.name}")
         else:
             INPUTS[party_name][operation.name] = (operation, ty)
-        return {
+        op_id = id(operation)
+        op_instruction = {
             "InputReference": {
+                "id": op_id,
                 "refers_to": operation.name,
                 "type": ty,
                 "source_ref": operation.source_ref.to_dict(),
             }
         }
+        instructions[op_id] = op_instruction
+        return op_id
     elif isinstance(operation, Literal):
         # Generate a unique name depending on the value and type to prevent duplicating literals in the bytecode.
         literal_name = hashlib.md5(
             (str(operation.value) + str(ty)).encode("UTF-8")
         ).hexdigest()
         LITERALS[literal_name] = (str(operation.value), ty)
-        return {
+        op_id = id(operation)
+        op_instruction = {
             "LiteralReference": {
+                "id": op_id,
                 "refers_to": literal_name,
                 "type": ty,
                 "source_ref": operation.source_ref.to_dict(),
             }
         }
+        instructions[op_id] = op_instruction
+        return op_id
     elif isinstance(operation, Map):
         if operation.fn.id not in FUNCTIONS:
             FUNCTIONS[operation.fn.id] = operation.fn
-        return {
+        op_id = id(operation)
+        op_instruction = {
             "Map": {
+                "id": op_id,
                 "fn": operation.fn.id,
-                "inner": process_operation(operation.inner),
+                "inner": process_operation(operation.inner, instructions),
                 "type": ty,
                 "source_ref": operation.source_ref.to_dict(),
             }
         }
+        instructions[op_id] = op_instruction
+        return op_id
     elif isinstance(operation, Reduce):
         if operation.fn.id not in FUNCTIONS:
             FUNCTIONS[operation.fn.id] = operation.fn
-        return {
+        op_id = id(operation)
+        op_instruction = {
             "Reduce": {
+                "id": op_id,
                 "fn": operation.fn.id,
-                "inner": process_operation(operation.inner),
-                "initial": process_operation(operation.initial),
+                "inner": process_operation(operation.inner, instructions),
+                "initial": process_operation(operation.initial, instructions),
                 "type": ty,
                 "source_ref": operation.source_ref.to_dict(),
             }
         }
+        instructions[op_id] = op_instruction
+        return op_id
     elif isinstance(operation, Unzip):
-        return {
+        op_id = id(operation)
+        op_instruction = {
             "Unzip": {
-                "inner": process_operation(operation.inner),
+                "id": op_id,
+                "inner": process_operation(operation.inner, instructions),
                 "type": ty,
                 "source_ref": operation.source_ref.to_dict(),
             }
         }
+        instructions[op_id] = op_instruction
+        return op_id
     elif isinstance(operation, NadaFunctionArg):
-        return {
+        op_id = id(operation)
+        op_instruction = {
             "NadaFunctionArgRef": {
+                "id": op_id,
                 "function_id": operation.function_id,
                 "refers_to": operation.name,
                 "type": to_type_dict(operation.type),
                 "source_ref": operation.source_ref.to_dict(),
             }
         }
+        instructions[op_id] = op_instruction
+        return op_id
     elif isinstance(operation, NadaFunctionCall):
         if operation.fn.id not in FUNCTIONS:
             FUNCTIONS[operation.fn.id] = operation.fn
-        return {
+        op_id = id(operation)
+        op_instruction = {
             "NadaFunctionCall": {
+                "id": op_id,
                 "function_id": operation.fn.id,
-                "args": [process_operation(arg) for arg in operation.args],
+                "args": [process_operation(arg, instructions) for arg in operation.args],
                 "type": ty,
                 "source_ref": operation.source_ref.to_dict(),
                 "return_type": to_type_dict(operation.fn.return_type),
             }
         }
+        instructions[op_id] = op_instruction
+        return op_id
     elif isinstance(operation, Random):
-        return {
+        op_id = id(operation)
+        op_instruction = {
             "Random": {
+                "id": op_id,
                 "type": ty,
                 "source_ref": operation.source_ref.to_dict(),
             }
         }
+        instructions[op_id] = op_instruction
+        return op_id
     elif isinstance(operation, IfElse):
-        return {
+        op_id = id(operation)
+        op_instruction = {
             "IfElse": {
-                "this": process_operation(operation.this),
-                "arg_0": process_operation(operation.arg_0),
-                "arg_1": process_operation(operation.arg_1),
+                "id": op_id,
+                "this": process_operation(operation.this, instructions),
+                "arg_0": process_operation(operation.arg_0, instructions),
+                "arg_1": process_operation(operation.arg_1, instructions),
                 "type": ty,
                 "source_ref": operation.source_ref.to_dict(),
             }
         }
+        instructions[op_id] = op_instruction
+        return op_id
     elif isinstance(operation, Reveal):
-        return {
+        op_id = id(operation)
+        op_instruction = {
             "Reveal": {
-                "this": process_operation(operation.this),
+                "id": op_id,
+                "this": process_operation(operation.this, instructions),
+                "type": ty,
+                "source_ref": operation.source_ref.to_dict(),
+            }
+        }
+        instructions[op_id] = op_instruction
+        return op_id
+    elif isinstance(operation, TruncPr):
+        op_id = id(operation)
+        op_instruction = {
+            "TruncPr": {
+                "id": op_id,
+                "left": process_operation(operation.left, instructions),
+                "right": process_operation(operation.right, instructions),
                 "type": ty,
                 "source_ref": operation.source_ref.to_dict(),
             }
         }
+        instructions[op_id] = op_instruction
+        return op_id
     elif isinstance(operation, ArrayNew):
-        return {
+        op_id = id(operation)
+        op_instruction = {
             "New": {
-                "elements": [process_operation(arg) for arg in operation.inner],
+                "id": op_id,
+                "elements": [process_operation(arg, instructions) for arg in operation.inner],
                 "type": to_type_dict(operation.inner_type),
                 "source_ref": operation.source_ref.to_dict(),
             }
         }
+        instructions[op_id] = op_instruction
+        return op_id
     elif isinstance(operation, TupleNew):
-        return {
+        op_id = id(operation)
+        op_instruction = {
             "New": {
-                "elements": [process_operation(operation.inner[0]), process_operation(operation.inner[1])],
+                "id": op_id,
+                "elements": [process_operation(operation.inner[0], instructions),
+                             process_operation(operation.inner[1], instructions)],
                 "type": to_type_dict(operation.inner_type),
                 "source_ref": operation.source_ref.to_dict(),
             }
         }
+        instructions[op_id] = op_instruction
+        return op_id
     else:
         raise Exception(f"Compilation of Operation {operation} is not supported")
```

## nada_dsl/nada_types/types.py

```diff
@@ -1,13 +1,13 @@
 # This file is automatically generated. Do not edit!
 
 from . import NadaType
 from dataclasses import dataclass
 from nada_dsl.circuit_io import Literal
-from nada_dsl.operations import Addition, Division, GreaterOrEqualThan, GreaterThan, IfElse, LessOrEqualThan, LessThan, Modulo, Multiplication, Power, PublicOutputEquality, Random, Reveal, Subtraction
+from nada_dsl.operations import Addition, Division, Equals, GreaterOrEqualThan, GreaterThan, IfElse, LeftShift, LessOrEqualThan, LessThan, Modulo, Multiplication, Power, PublicOutputEquality, Random, Reveal, RightShift, Subtraction, TruncPr
 from nada_dsl.source_ref import SourceRef
 from typing import Union
 
 @dataclass
 class Integer(NadaType):
     value: int
 
@@ -84,14 +84,36 @@
             return PublicInteger(inner=operation)
         elif isinstance(other, SecretInteger):
             operation = Modulo(left=self, right=other, source_ref=SourceRef.back_frame())
             return SecretInteger(inner=operation)
         else:
             raise TypeError(f"Invalid operation: {self} % {other}")
 
+    def __lshift__(
+        self, other: Union["PublicUnsignedInteger", "UnsignedInteger"]
+    ) -> Union["Integer", "PublicUnsignedInteger"]:
+        if isinstance(other, UnsignedInteger):
+            return Integer(value=int(self.value << other.value))
+        elif isinstance(other, PublicUnsignedInteger):
+            operation = LeftShift(left=self, right=other, source_ref=SourceRef.back_frame())
+            return PublicUnsignedInteger(inner=operation)
+        else:
+            raise TypeError(f"Invalid operation: {self} << {other}")
+
+    def __rshift__(
+        self, other: Union["PublicUnsignedInteger", "UnsignedInteger"]
+    ) -> Union["Integer", "PublicUnsignedInteger"]:
+        if isinstance(other, UnsignedInteger):
+            return Integer(value=int(self.value >> other.value))
+        elif isinstance(other, PublicUnsignedInteger):
+            operation = RightShift(left=self, right=other, source_ref=SourceRef.back_frame())
+            return PublicUnsignedInteger(inner=operation)
+        else:
+            raise TypeError(f"Invalid operation: {self} >> {other}")
+
     def __lt__(
         self, other: Union["Integer", "PublicInteger", "SecretInteger"]
     ) -> Union["Boolean", "PublicBoolean", "SecretBoolean"]:
         if isinstance(other, Integer):
             return Boolean(value=bool(self.value < other.value))
         elif isinstance(other, PublicInteger):
             operation = LessThan(left=self, right=other, source_ref=SourceRef.back_frame())
@@ -140,14 +162,28 @@
             return PublicBoolean(inner=operation)
         elif isinstance(other, SecretInteger):
             operation = GreaterOrEqualThan(left=self, right=other, source_ref=SourceRef.back_frame())
             return SecretBoolean(inner=operation)
         else:
             raise TypeError(f"Invalid operation: {self} >= {other}")
 
+    def __eq__(
+        self, other: Union["Integer", "PublicInteger", "SecretInteger"]
+    ) -> Union["Boolean", "PublicBoolean", "SecretBoolean"]:
+        if isinstance(other, Integer):
+            return Boolean(value=bool(self.value == other.value))
+        elif isinstance(other, PublicInteger):
+            operation = Equals(left=self, right=other, source_ref=SourceRef.back_frame())
+            return PublicBoolean(inner=operation)
+        elif isinstance(other, SecretInteger):
+            operation = Equals(left=self, right=other, source_ref=SourceRef.back_frame())
+            return SecretBoolean(inner=operation)
+        else:
+            raise TypeError(f"Invalid operation: {self} == {other}")
+
 @dataclass
 class UnsignedInteger(NadaType):
     value: int
 
     def __init__(self, value: int):
         super().__init__(inner=Literal(value=value, source_ref=SourceRef.back_frame()))
         if isinstance(value, int):
@@ -232,14 +268,36 @@
             return UnsignedInteger(value=int(self.value ** other.value))
         elif isinstance(other, PublicUnsignedInteger):
             operation = Power(left=self, right=other, source_ref=SourceRef.back_frame())
             return PublicUnsignedInteger(inner=operation)
         else:
             raise TypeError(f"Invalid operation: {self} ** {other}")
 
+    def __lshift__(
+        self, other: Union["PublicUnsignedInteger", "UnsignedInteger"]
+    ) -> Union["PublicUnsignedInteger", "UnsignedInteger"]:
+        if isinstance(other, UnsignedInteger):
+            return UnsignedInteger(value=int(self.value << other.value))
+        elif isinstance(other, PublicUnsignedInteger):
+            operation = LeftShift(left=self, right=other, source_ref=SourceRef.back_frame())
+            return PublicUnsignedInteger(inner=operation)
+        else:
+            raise TypeError(f"Invalid operation: {self} << {other}")
+
+    def __rshift__(
+        self, other: Union["PublicUnsignedInteger", "UnsignedInteger"]
+    ) -> Union["PublicUnsignedInteger", "UnsignedInteger"]:
+        if isinstance(other, UnsignedInteger):
+            return UnsignedInteger(value=int(self.value >> other.value))
+        elif isinstance(other, PublicUnsignedInteger):
+            operation = RightShift(left=self, right=other, source_ref=SourceRef.back_frame())
+            return PublicUnsignedInteger(inner=operation)
+        else:
+            raise TypeError(f"Invalid operation: {self} >> {other}")
+
     def __lt__(
         self, other: Union["PublicUnsignedInteger", "SecretUnsignedInteger", "UnsignedInteger"]
     ) -> Union["Boolean", "PublicBoolean", "SecretBoolean"]:
         if isinstance(other, UnsignedInteger):
             return Boolean(value=bool(self.value < other.value))
         elif isinstance(other, PublicUnsignedInteger):
             operation = LessThan(left=self, right=other, source_ref=SourceRef.back_frame())
@@ -288,26 +346,53 @@
             return PublicBoolean(inner=operation)
         elif isinstance(other, SecretUnsignedInteger):
             operation = GreaterOrEqualThan(left=self, right=other, source_ref=SourceRef.back_frame())
             return SecretBoolean(inner=operation)
         else:
             raise TypeError(f"Invalid operation: {self} >= {other}")
 
+    def __eq__(
+        self, other: Union["PublicUnsignedInteger", "SecretUnsignedInteger", "UnsignedInteger"]
+    ) -> Union["Boolean", "PublicBoolean", "SecretBoolean"]:
+        if isinstance(other, UnsignedInteger):
+            return Boolean(value=bool(self.value == other.value))
+        elif isinstance(other, PublicUnsignedInteger):
+            operation = Equals(left=self, right=other, source_ref=SourceRef.back_frame())
+            return PublicBoolean(inner=operation)
+        elif isinstance(other, SecretUnsignedInteger):
+            operation = Equals(left=self, right=other, source_ref=SourceRef.back_frame())
+            return SecretBoolean(inner=operation)
+        else:
+            raise TypeError(f"Invalid operation: {self} == {other}")
+
 @dataclass
 class Boolean(NadaType):
     value: bool
 
     def __init__(self, value: bool):
         super().__init__(inner=Literal(value=value, source_ref=SourceRef.back_frame()))
         if isinstance(value, bool):
             self.value = value
         else:
             raise ValueError(f"Expected bool, got {type(value).__name__}")
 
-    pass
+    def __eq__(
+        self, other: Union["Boolean", "PublicBoolean", "SecretBoolean"]
+    ) -> Union["Boolean", "PublicBoolean", "SecretBoolean"]:
+        if isinstance(other, Boolean):
+            return Boolean(value=bool(self.value == other.value))
+        elif isinstance(other, PublicBoolean):
+            operation = Equals(left=self, right=other, source_ref=SourceRef.back_frame())
+            return PublicBoolean(inner=operation)
+        elif isinstance(other, SecretBoolean):
+            operation = Equals(left=self, right=other, source_ref=SourceRef.back_frame())
+            return SecretBoolean(inner=operation)
+        else:
+            raise TypeError(f"Invalid operation: {self} == {other}")
+
 @dataclass
 class PublicInteger(NadaType):
     def __add__(
         self, other: Union["Integer", "PublicInteger", "SecretInteger"]
     ) -> Union["PublicInteger", "SecretInteger"]:
         if isinstance(other, Integer):
             operation = Addition(left=self, right=other, source_ref=SourceRef.back_frame())
@@ -377,14 +462,38 @@
             return PublicInteger(inner=operation)
         elif isinstance(other, SecretInteger):
             operation = Modulo(left=self, right=other, source_ref=SourceRef.back_frame())
             return SecretInteger(inner=operation)
         else:
             raise TypeError(f"Invalid operation: {self} % {other}")
 
+    def __lshift__(
+        self, other: Union["PublicUnsignedInteger", "UnsignedInteger"]
+    ) -> "PublicInteger":
+        if isinstance(other, UnsignedInteger):
+            operation = LeftShift(left=self, right=other, source_ref=SourceRef.back_frame())
+            return PublicInteger(inner=operation)
+        elif isinstance(other, PublicUnsignedInteger):
+            operation = LeftShift(left=self, right=other, source_ref=SourceRef.back_frame())
+            return PublicInteger(inner=operation)
+        else:
+            raise TypeError(f"Invalid operation: {self} << {other}")
+
+    def __rshift__(
+        self, other: Union["PublicUnsignedInteger", "UnsignedInteger"]
+    ) -> "PublicInteger":
+        if isinstance(other, UnsignedInteger):
+            operation = RightShift(left=self, right=other, source_ref=SourceRef.back_frame())
+            return PublicInteger(inner=operation)
+        elif isinstance(other, PublicUnsignedInteger):
+            operation = RightShift(left=self, right=other, source_ref=SourceRef.back_frame())
+            return PublicInteger(inner=operation)
+        else:
+            raise TypeError(f"Invalid operation: {self} >> {other}")
+
     def __lt__(
         self, other: Union["Integer", "PublicInteger", "SecretInteger"]
     ) -> Union["PublicBoolean", "SecretBoolean"]:
         if isinstance(other, Integer):
             operation = LessThan(left=self, right=other, source_ref=SourceRef.back_frame())
             return PublicBoolean(inner=operation)
         elif isinstance(other, PublicInteger):
@@ -437,14 +546,29 @@
             return PublicBoolean(inner=operation)
         elif isinstance(other, SecretInteger):
             operation = GreaterOrEqualThan(left=self, right=other, source_ref=SourceRef.back_frame())
             return SecretBoolean(inner=operation)
         else:
             raise TypeError(f"Invalid operation: {self} >= {other}")
 
+    def __eq__(
+        self, other: Union["Integer", "PublicInteger", "SecretInteger"]
+    ) -> Union["PublicBoolean", "SecretBoolean"]:
+        if isinstance(other, Integer):
+            operation = Equals(left=self, right=other, source_ref=SourceRef.back_frame())
+            return PublicBoolean(inner=operation)
+        elif isinstance(other, PublicInteger):
+            operation = Equals(left=self, right=other, source_ref=SourceRef.back_frame())
+            return PublicBoolean(inner=operation)
+        elif isinstance(other, SecretInteger):
+            operation = Equals(left=self, right=other, source_ref=SourceRef.back_frame())
+            return SecretBoolean(inner=operation)
+        else:
+            raise TypeError(f"Invalid operation: {self} == {other}")
+
     def public_equals(
         self, other: Union["PublicInteger", "SecretInteger"]
     ) -> "PublicBoolean":
         if isinstance(other, PublicInteger):
             operation = PublicOutputEquality(left=self, right=other, source_ref=SourceRef.back_frame())
             return PublicBoolean(inner=operation)
         elif isinstance(other, SecretInteger):
@@ -538,14 +662,38 @@
             return PublicUnsignedInteger(inner=operation)
         elif isinstance(other, PublicUnsignedInteger):
             operation = Power(left=self, right=other, source_ref=SourceRef.back_frame())
             return PublicUnsignedInteger(inner=operation)
         else:
             raise TypeError(f"Invalid operation: {self} ** {other}")
 
+    def __lshift__(
+        self, other: Union["PublicUnsignedInteger", "UnsignedInteger"]
+    ) -> "PublicUnsignedInteger":
+        if isinstance(other, UnsignedInteger):
+            operation = LeftShift(left=self, right=other, source_ref=SourceRef.back_frame())
+            return PublicUnsignedInteger(inner=operation)
+        elif isinstance(other, PublicUnsignedInteger):
+            operation = LeftShift(left=self, right=other, source_ref=SourceRef.back_frame())
+            return PublicUnsignedInteger(inner=operation)
+        else:
+            raise TypeError(f"Invalid operation: {self} << {other}")
+
+    def __rshift__(
+        self, other: Union["PublicUnsignedInteger", "UnsignedInteger"]
+    ) -> "PublicUnsignedInteger":
+        if isinstance(other, UnsignedInteger):
+            operation = RightShift(left=self, right=other, source_ref=SourceRef.back_frame())
+            return PublicUnsignedInteger(inner=operation)
+        elif isinstance(other, PublicUnsignedInteger):
+            operation = RightShift(left=self, right=other, source_ref=SourceRef.back_frame())
+            return PublicUnsignedInteger(inner=operation)
+        else:
+            raise TypeError(f"Invalid operation: {self} >> {other}")
+
     def __lt__(
         self, other: Union["PublicUnsignedInteger", "SecretUnsignedInteger", "UnsignedInteger"]
     ) -> Union["PublicBoolean", "SecretBoolean"]:
         if isinstance(other, UnsignedInteger):
             operation = LessThan(left=self, right=other, source_ref=SourceRef.back_frame())
             return PublicBoolean(inner=operation)
         elif isinstance(other, PublicUnsignedInteger):
@@ -598,28 +746,58 @@
             return PublicBoolean(inner=operation)
         elif isinstance(other, SecretUnsignedInteger):
             operation = GreaterOrEqualThan(left=self, right=other, source_ref=SourceRef.back_frame())
             return SecretBoolean(inner=operation)
         else:
             raise TypeError(f"Invalid operation: {self} >= {other}")
 
+    def __eq__(
+        self, other: Union["PublicUnsignedInteger", "SecretUnsignedInteger", "UnsignedInteger"]
+    ) -> Union["PublicBoolean", "SecretBoolean"]:
+        if isinstance(other, UnsignedInteger):
+            operation = Equals(left=self, right=other, source_ref=SourceRef.back_frame())
+            return PublicBoolean(inner=operation)
+        elif isinstance(other, PublicUnsignedInteger):
+            operation = Equals(left=self, right=other, source_ref=SourceRef.back_frame())
+            return PublicBoolean(inner=operation)
+        elif isinstance(other, SecretUnsignedInteger):
+            operation = Equals(left=self, right=other, source_ref=SourceRef.back_frame())
+            return SecretBoolean(inner=operation)
+        else:
+            raise TypeError(f"Invalid operation: {self} == {other}")
+
     def public_equals(
         self, other: Union["PublicUnsignedInteger", "SecretUnsignedInteger"]
     ) -> "PublicBoolean":
         if isinstance(other, PublicUnsignedInteger):
             operation = PublicOutputEquality(left=self, right=other, source_ref=SourceRef.back_frame())
             return PublicBoolean(inner=operation)
         elif isinstance(other, SecretUnsignedInteger):
             operation = PublicOutputEquality(left=self, right=other, source_ref=SourceRef.back_frame())
             return PublicBoolean(inner=operation)
         else:
             raise TypeError(f"Invalid operation: {self}.public_equals({other})")
 
 @dataclass
 class PublicBoolean(NadaType):
+    def __eq__(
+        self, other: Union["Boolean", "PublicBoolean", "SecretBoolean"]
+    ) -> Union["PublicBoolean", "SecretBoolean"]:
+        if isinstance(other, Boolean):
+            operation = Equals(left=self, right=other, source_ref=SourceRef.back_frame())
+            return PublicBoolean(inner=operation)
+        elif isinstance(other, PublicBoolean):
+            operation = Equals(left=self, right=other, source_ref=SourceRef.back_frame())
+            return PublicBoolean(inner=operation)
+        elif isinstance(other, SecretBoolean):
+            operation = Equals(left=self, right=other, source_ref=SourceRef.back_frame())
+            return SecretBoolean(inner=operation)
+        else:
+            raise TypeError(f"Invalid operation: {self} == {other}")
+
     def if_else(
         self: "PublicBoolean",
         arg_0, arg_1: Union["Integer", "PublicInteger", "PublicUnsignedInteger", "SecretInteger", "SecretUnsignedInteger", "UnsignedInteger"]
     ) -> Union["PublicInteger", "PublicUnsignedInteger", "SecretInteger", "SecretUnsignedInteger"]:
         if isinstance(arg_0, SecretInteger) and isinstance(arg_1, SecretInteger):
             operation = IfElse(this=self, arg_0=arg_0, arg_1=arg_1, source_ref=SourceRef.back_frame())
             return SecretInteger(inner=operation)
@@ -673,15 +851,14 @@
             return PublicUnsignedInteger(inner=operation)
         elif isinstance(arg_0, UnsignedInteger) and isinstance(arg_1, PublicUnsignedInteger):
             operation = IfElse(this=self, arg_0=arg_0, arg_1=arg_1, source_ref=SourceRef.back_frame())
             return PublicUnsignedInteger(inner=operation)
         else:
             raise TypeError(f"Invalid operation: {self}.IfElse({arg_0}, {arg_1})")
     
-    pass
 @dataclass
 class SecretInteger(NadaType):
     def __add__(
         self, other: Union["Integer", "PublicInteger", "SecretInteger"]
     ) -> "SecretInteger":
         if isinstance(other, Integer):
             operation = Addition(left=self, right=other, source_ref=SourceRef.back_frame())
@@ -751,14 +928,38 @@
             return SecretInteger(inner=operation)
         elif isinstance(other, SecretInteger):
             operation = Modulo(left=self, right=other, source_ref=SourceRef.back_frame())
             return SecretInteger(inner=operation)
         else:
             raise TypeError(f"Invalid operation: {self} % {other}")
 
+    def __lshift__(
+        self, other: Union["PublicUnsignedInteger", "UnsignedInteger"]
+    ) -> "SecretInteger":
+        if isinstance(other, UnsignedInteger):
+            operation = LeftShift(left=self, right=other, source_ref=SourceRef.back_frame())
+            return SecretInteger(inner=operation)
+        elif isinstance(other, PublicUnsignedInteger):
+            operation = LeftShift(left=self, right=other, source_ref=SourceRef.back_frame())
+            return SecretInteger(inner=operation)
+        else:
+            raise TypeError(f"Invalid operation: {self} << {other}")
+
+    def __rshift__(
+        self, other: Union["PublicUnsignedInteger", "UnsignedInteger"]
+    ) -> "SecretInteger":
+        if isinstance(other, UnsignedInteger):
+            operation = RightShift(left=self, right=other, source_ref=SourceRef.back_frame())
+            return SecretInteger(inner=operation)
+        elif isinstance(other, PublicUnsignedInteger):
+            operation = RightShift(left=self, right=other, source_ref=SourceRef.back_frame())
+            return SecretInteger(inner=operation)
+        else:
+            raise TypeError(f"Invalid operation: {self} >> {other}")
+
     def __lt__(
         self, other: Union["Integer", "PublicInteger", "SecretInteger"]
     ) -> "SecretBoolean":
         if isinstance(other, Integer):
             operation = LessThan(left=self, right=other, source_ref=SourceRef.back_frame())
             return SecretBoolean(inner=operation)
         elif isinstance(other, PublicInteger):
@@ -811,14 +1012,29 @@
             return SecretBoolean(inner=operation)
         elif isinstance(other, SecretInteger):
             operation = GreaterOrEqualThan(left=self, right=other, source_ref=SourceRef.back_frame())
             return SecretBoolean(inner=operation)
         else:
             raise TypeError(f"Invalid operation: {self} >= {other}")
 
+    def __eq__(
+        self, other: Union["Integer", "PublicInteger", "SecretInteger"]
+    ) -> "SecretBoolean":
+        if isinstance(other, Integer):
+            operation = Equals(left=self, right=other, source_ref=SourceRef.back_frame())
+            return SecretBoolean(inner=operation)
+        elif isinstance(other, PublicInteger):
+            operation = Equals(left=self, right=other, source_ref=SourceRef.back_frame())
+            return SecretBoolean(inner=operation)
+        elif isinstance(other, SecretInteger):
+            operation = Equals(left=self, right=other, source_ref=SourceRef.back_frame())
+            return SecretBoolean(inner=operation)
+        else:
+            raise TypeError(f"Invalid operation: {self} == {other}")
+
     def public_equals(
         self, other: Union["PublicInteger", "SecretInteger"]
     ) -> "PublicBoolean":
         if isinstance(other, PublicInteger):
             operation = PublicOutputEquality(left=self, right=other, source_ref=SourceRef.back_frame())
             return PublicBoolean(inner=operation)
         elif isinstance(other, SecretInteger):
@@ -833,14 +1049,33 @@
     
     def reveal(
         self: "SecretInteger",
     ) -> "PublicInteger":
         operation = Reveal(this=self, source_ref=SourceRef.back_frame())
         return PublicInteger(inner=operation)
     
+    def trunc_pr(
+        self: "SecretInteger",
+        arg_0: Union["Integer", "PublicInteger", "PublicUnsignedInteger", "UnsignedInteger"]
+    ) -> "SecretInteger":
+        if isinstance(arg_0, PublicInteger):
+            operation = TruncPr(left=self, right=arg_0, source_ref=SourceRef.back_frame())
+            return SecretInteger(inner=operation)
+        elif isinstance(arg_0, Integer):
+            operation = TruncPr(left=self, right=arg_0, source_ref=SourceRef.back_frame())
+            return SecretInteger(inner=operation)
+        elif isinstance(arg_0, PublicUnsignedInteger):
+            operation = TruncPr(left=self, right=arg_0, source_ref=SourceRef.back_frame())
+            return SecretInteger(inner=operation)
+        elif isinstance(arg_0, UnsignedInteger):
+            operation = TruncPr(left=self, right=arg_0, source_ref=SourceRef.back_frame())
+            return SecretInteger(inner=operation)
+        else:
+            raise TypeError(f"Invalid operation: {self}.TruncPr({arg_0})")
+    
 @dataclass
 class SecretUnsignedInteger(NadaType):
     def __add__(
         self, other: Union["PublicUnsignedInteger", "SecretUnsignedInteger", "UnsignedInteger"]
     ) -> "SecretUnsignedInteger":
         if isinstance(other, UnsignedInteger):
             operation = Addition(left=self, right=other, source_ref=SourceRef.back_frame())
@@ -910,14 +1145,38 @@
             return SecretUnsignedInteger(inner=operation)
         elif isinstance(other, SecretUnsignedInteger):
             operation = Modulo(left=self, right=other, source_ref=SourceRef.back_frame())
             return SecretUnsignedInteger(inner=operation)
         else:
             raise TypeError(f"Invalid operation: {self} % {other}")
 
+    def __lshift__(
+        self, other: Union["PublicUnsignedInteger", "UnsignedInteger"]
+    ) -> "SecretUnsignedInteger":
+        if isinstance(other, UnsignedInteger):
+            operation = LeftShift(left=self, right=other, source_ref=SourceRef.back_frame())
+            return SecretUnsignedInteger(inner=operation)
+        elif isinstance(other, PublicUnsignedInteger):
+            operation = LeftShift(left=self, right=other, source_ref=SourceRef.back_frame())
+            return SecretUnsignedInteger(inner=operation)
+        else:
+            raise TypeError(f"Invalid operation: {self} << {other}")
+
+    def __rshift__(
+        self, other: Union["PublicUnsignedInteger", "UnsignedInteger"]
+    ) -> "SecretUnsignedInteger":
+        if isinstance(other, UnsignedInteger):
+            operation = RightShift(left=self, right=other, source_ref=SourceRef.back_frame())
+            return SecretUnsignedInteger(inner=operation)
+        elif isinstance(other, PublicUnsignedInteger):
+            operation = RightShift(left=self, right=other, source_ref=SourceRef.back_frame())
+            return SecretUnsignedInteger(inner=operation)
+        else:
+            raise TypeError(f"Invalid operation: {self} >> {other}")
+
     def __lt__(
         self, other: Union["PublicUnsignedInteger", "SecretUnsignedInteger", "UnsignedInteger"]
     ) -> "SecretBoolean":
         if isinstance(other, UnsignedInteger):
             operation = LessThan(left=self, right=other, source_ref=SourceRef.back_frame())
             return SecretBoolean(inner=operation)
         elif isinstance(other, PublicUnsignedInteger):
@@ -970,14 +1229,29 @@
             return SecretBoolean(inner=operation)
         elif isinstance(other, SecretUnsignedInteger):
             operation = GreaterOrEqualThan(left=self, right=other, source_ref=SourceRef.back_frame())
             return SecretBoolean(inner=operation)
         else:
             raise TypeError(f"Invalid operation: {self} >= {other}")
 
+    def __eq__(
+        self, other: Union["PublicUnsignedInteger", "SecretUnsignedInteger", "UnsignedInteger"]
+    ) -> "SecretBoolean":
+        if isinstance(other, UnsignedInteger):
+            operation = Equals(left=self, right=other, source_ref=SourceRef.back_frame())
+            return SecretBoolean(inner=operation)
+        elif isinstance(other, PublicUnsignedInteger):
+            operation = Equals(left=self, right=other, source_ref=SourceRef.back_frame())
+            return SecretBoolean(inner=operation)
+        elif isinstance(other, SecretUnsignedInteger):
+            operation = Equals(left=self, right=other, source_ref=SourceRef.back_frame())
+            return SecretBoolean(inner=operation)
+        else:
+            raise TypeError(f"Invalid operation: {self} == {other}")
+
     def public_equals(
         self, other: Union["PublicUnsignedInteger", "SecretUnsignedInteger"]
     ) -> "PublicBoolean":
         if isinstance(other, PublicUnsignedInteger):
             operation = PublicOutputEquality(left=self, right=other, source_ref=SourceRef.back_frame())
             return PublicBoolean(inner=operation)
         elif isinstance(other, SecretUnsignedInteger):
@@ -992,16 +1266,56 @@
     
     def reveal(
         self: "SecretUnsignedInteger",
     ) -> "PublicUnsignedInteger":
         operation = Reveal(this=self, source_ref=SourceRef.back_frame())
         return PublicUnsignedInteger(inner=operation)
     
+    def trunc_pr(
+        self: "SecretUnsignedInteger",
+        arg_0: Union["Integer", "PublicInteger", "PublicUnsignedInteger", "UnsignedInteger"]
+    ) -> "SecretUnsignedInteger":
+        if isinstance(arg_0, PublicInteger):
+            operation = TruncPr(left=self, right=arg_0, source_ref=SourceRef.back_frame())
+            return SecretUnsignedInteger(inner=operation)
+        elif isinstance(arg_0, Integer):
+            operation = TruncPr(left=self, right=arg_0, source_ref=SourceRef.back_frame())
+            return SecretUnsignedInteger(inner=operation)
+        elif isinstance(arg_0, PublicUnsignedInteger):
+            operation = TruncPr(left=self, right=arg_0, source_ref=SourceRef.back_frame())
+            return SecretUnsignedInteger(inner=operation)
+        elif isinstance(arg_0, UnsignedInteger):
+            operation = TruncPr(left=self, right=arg_0, source_ref=SourceRef.back_frame())
+            return SecretUnsignedInteger(inner=operation)
+        else:
+            raise TypeError(f"Invalid operation: {self}.TruncPr({arg_0})")
+    
+@dataclass
+class SecretNonZeroInteger(NadaType):
+    pass
+@dataclass
+class SecretNonZeroUnsignedInteger(NadaType):
+    pass
 @dataclass
 class SecretBoolean(NadaType):
+    def __eq__(
+        self, other: Union["Boolean", "PublicBoolean", "SecretBoolean"]
+    ) -> "SecretBoolean":
+        if isinstance(other, Boolean):
+            operation = Equals(left=self, right=other, source_ref=SourceRef.back_frame())
+            return SecretBoolean(inner=operation)
+        elif isinstance(other, PublicBoolean):
+            operation = Equals(left=self, right=other, source_ref=SourceRef.back_frame())
+            return SecretBoolean(inner=operation)
+        elif isinstance(other, SecretBoolean):
+            operation = Equals(left=self, right=other, source_ref=SourceRef.back_frame())
+            return SecretBoolean(inner=operation)
+        else:
+            raise TypeError(f"Invalid operation: {self} == {other}")
+
     def reveal(
         self: "SecretBoolean",
     ) -> "PublicBoolean":
         operation = Reveal(this=self, source_ref=SourceRef.back_frame())
         return PublicBoolean(inner=operation)
     
     def if_else(
@@ -1061,15 +1375,14 @@
             return SecretUnsignedInteger(inner=operation)
         elif isinstance(arg_0, UnsignedInteger) and isinstance(arg_1, PublicUnsignedInteger):
             operation = IfElse(this=self, arg_0=arg_0, arg_1=arg_1, source_ref=SourceRef.back_frame())
             return SecretUnsignedInteger(inner=operation)
         else:
             raise TypeError(f"Invalid operation: {self}.IfElse({arg_0}, {arg_1})")
     
-    pass
 @dataclass
 class SecretBlob(NadaType):
     pass
 @dataclass
 class ShamirShareInteger(NadaType):
     pass
 @dataclass
```

## nada_dsl/compiler_frontend_test.py

```diff
@@ -44,40 +44,44 @@
 def create_collection(cls, inner_input, size, **kwargs):
     return cls(inner_input, size, **kwargs)
 
 
 def create_output(root: AllTypes, name: str, party: str) -> Output:
     return Output(root, name, Party(party))
 
+
 def to_type(name: str):
     # Rename public variables so they are considered as the same as literals.
     if name.startswith("Public"):
-        name = name[len("Public") :].lstrip()
+        name = name[len("Public"):].lstrip()
         return name
     else:
         return name
 
+
 # Generated tests are added below this line. Please leave it as it is.
 
 
 def test_root_conversion():
     input = create_input(SecretInteger, "input", "input_party")
     output = create_output(input, "output", "output_party")
     mir = nada_dsl_to_nada_mir([output])
     assert len(mir["parties"]) == 2
     assert len(mir["inputs"]) == 1
     assert len(mir["literals"]) == 0
     assert len(mir["outputs"]) == 1
     assert "source_files" in mir
 
+    instructions = mir["instructions"]
     mir_output = mir["outputs"][0]
     assert mir_output["name"] == "output"
     assert mir_output["type"] == "SecretInteger"
     assert mir_output["party"] == "output_party"
-    assert list(mir_output["inner"].keys()) == ["InputReference"]
+
+    assert list(instructions[mir_output["instruction_id"]].keys()) == ["InputReference"]
 
 
 def test_input_conversion():
     input = Input(name="input", party=Party("party"))
     inputs = {"party": {"input": (input, "SecretInteger")}}
     converted_inputs = to_input_list(inputs)
     assert len(converted_inputs) == 1
@@ -115,21 +119,25 @@
 )
 def test_zip(input_type, input_name):
     inner_input = create_input(SecretInteger, "left", "party", **{})
     left = create_collection(input_type, inner_input, 10, **{})
     inner_input = create_input(SecretInteger, "right", "party", **{})
     right = create_collection(input_type, inner_input, 10, **{})
     zipped = left.zip(right)
-    op = process_operation(zipped)
+    instructions = {}
+    op_id = process_operation(zipped, instructions)
+    op = instructions[op_id]
     assert list(op.keys()) == ["Zip"]
 
     inner = op["Zip"]
 
-    assert input_reference(inner["left"]) == "left"
-    assert input_reference(inner["right"]) == "right"
+    left = instructions[inner["left"]]
+    right = instructions[inner["right"]]
+    assert input_reference(left) == "left"
+    assert input_reference(right) == "right"
     assert inner["type"][input_name]["inner_type"] == {
         "Tuple": {
             "left_type": "SecretInteger",
             "right_type": "SecretInteger",
         }
     }
 
@@ -140,21 +148,23 @@
 )
 def test_unzip(input_type, input_name):
     inner_input = create_input(SecretInteger, "left", "party", **{})
     left = create_collection(input_type, inner_input, 10, **{})
     inner_input = create_input(SecretInteger, "right", "party", **{})
     right = create_collection(input_type, inner_input, 10, **{})
     unzipped = unzip(left.zip(right))
-    op = process_operation(unzipped)
+    instructions = {}
+    op_id = process_operation(unzipped, instructions)
+    op = instructions[op_id]
 
     assert list(op.keys()) == ["Unzip"]
 
     inner = op["Unzip"]
-
-    assert list(inner["inner"].keys()) == [
+    inner_inner = instructions[inner["inner"]]
+    assert list(inner_inner.keys()) == [
         "Zip"
     ]  # We don't check Zip operation because it has its test
     assert inner["type"] == {
         "Tuple": {
             "left_type": {
                 "Array": {"inner_type": "SecretInteger", "size": 10}
             },
@@ -173,20 +183,24 @@
     @nada_fn
     def nada_function(a: SecretInteger) -> SecretInteger:
         return a + a
 
     inner_input = create_input(SecretInteger, "inner", "party", **{})
     left = create_collection(input_type, inner_input, 10, **{})
     map_operation = left.map(nada_function)
-    op = process_operation(map_operation)
+    instructions = {}
+    op_id = process_operation(map_operation, instructions)
+    op = instructions[op_id]
+
     assert list(op.keys()) == ["Map"]
     inner = op["Map"]
     assert inner["fn"] in FUNCTIONS
     assert list(inner["type"].keys()) == [input_name]
-    assert input_reference(inner["inner"]) == "inner"
+    inner_inner = instructions[inner["inner"]]
+    assert input_reference(inner_inner) == "inner"
     assert inner["type"][input_name]["inner_type"] == "SecretInteger"
 
 
 @pytest.mark.parametrize(
     ("input_type", "input_name"),
     [(Array, "Array"), (Vector, "Vector")],
 )
@@ -196,20 +210,24 @@
     @nada_fn
     def nada_function(a: SecretInteger, b: SecretInteger) -> SecretInteger:
         return a + b
 
     inner_input = create_input(SecretInteger, "inner", "party", **{})
     left = create_collection(input_type, inner_input, 10, **{})
     reduce_operation = left.reduce(nada_function, c)
-    op = process_operation(reduce_operation)
+    instructions = {}
+    op_id = process_operation(reduce_operation, instructions)
+    op = instructions[op_id]
+
     assert list(op.keys()) == ["Reduce"]
     inner = op["Reduce"]
     assert inner["fn"] in FUNCTIONS
     assert inner["type"] == "SecretInteger"
-    assert input_reference(inner["inner"]) == "inner"
+    inner_inner = instructions[inner["inner"]]
+    assert input_reference(inner_inner) == "inner"
 
 
 def check_arg(arg: NadaFunctionArg, arg_name, arg_type):
     assert arg["name"] == arg_name
     assert arg["type"] == arg_type
 
 
@@ -228,21 +246,25 @@
     nada_function = to_fn_dict(nada_function)
     assert nada_function["function"] == "nada_function"
     args = nada_function["args"]
     assert len(args) == 2
     check_arg(args[0], "a", "SecretInteger")
     check_arg(args[1], "b", "SecretInteger")
     assert nada_function["return_type"] == "SecretInteger"
-    assert list(nada_function["body"].keys()) == ["Addition"]
-    addition = nada_function["body"]["Addition"]
+
+    instruction = nada_function["instructions"]
+    return_op = instruction[nada_function['return_instruction_id']]
+    assert list(return_op.keys()) == ["Addition"]
+    addition = return_op["Addition"]
+
     check_nada_function_arg_ref(
-        addition["left"], nada_function["id"], "a", "SecretInteger"
+        instruction[addition["left"]], nada_function["id"], "a", "SecretInteger"
     )
     check_nada_function_arg_ref(
-        addition["right"], nada_function["id"], "b", "SecretInteger"
+        instruction[addition["right"]], nada_function["id"], "b", "SecretInteger"
     )
 
 
 def test_nada_function_using_inputs():
     c = create_input(SecretInteger, "c", "party", **{})
 
     @nada_fn
@@ -252,24 +274,32 @@
     nada_function = to_fn_dict(nada_function)
     assert nada_function["function"] == "nada_function"
     args = nada_function["args"]
     assert len(args) == 2
     check_arg(args[0], "a", "SecretInteger")
     check_arg(args[1], "b", "SecretInteger")
     assert nada_function["return_type"] == "SecretInteger"
-    assert list(nada_function["body"].keys()) == ["Addition"]
-    addition = nada_function["body"]["Addition"]
-    assert input_reference(addition["right"]) == "c"
-    assert list(addition["left"].keys()) == ["Addition"]
-    addition = addition["left"]["Addition"]
+
+    instruction = nada_function["instructions"]
+    return_op = instruction[nada_function['return_instruction_id']]
+
+    assert list(return_op.keys()) == ["Addition"]
+    addition = return_op["Addition"]
+    addition_right = instruction[addition["right"]]
+    assert input_reference(addition_right) == "c"
+    addition_left = instruction[addition["left"]]
+    assert list(addition_left.keys()) == ["Addition"]
+
+    addition = addition_left["Addition"]
+
     check_nada_function_arg_ref(
-        addition["left"], nada_function["id"], "a", "SecretInteger"
+        instruction[addition["left"]], nada_function["id"], "a", "SecretInteger"
     )
     check_nada_function_arg_ref(
-        addition["right"], nada_function["id"], "b", "SecretInteger"
+        instruction[addition["right"]], nada_function["id"], "b", "SecretInteger"
     )
 
 
 def test_nada_function_call():
     c = create_input(SecretInteger, "c", "party", **{})
     d = create_input(SecretInteger, "c", "party", **{})
 
@@ -296,27 +326,36 @@
     nada_function = to_fn_dict(nada_function)
     assert nada_function["function"] == "nada_function"
     args = nada_function["args"]
     assert len(args) == 2
     check_arg(args[0], "a", "SecretInteger")
     check_arg(args[1], "b", "SecretInteger")
     assert nada_function["return_type"] == "SecretInteger"
-    assert list(nada_function["body"].keys()) == ["Addition"]
-    addition = nada_function["body"]["Addition"]
-    assert input_reference(addition["right"]) == "d"
-    assert list(addition["left"].keys()) == ["Addition"]
-    addition = addition["left"]["Addition"]
-    assert input_reference(addition["right"]) == "c"
-    assert list(addition["left"].keys()) == ["Addition"]
-    addition = addition["left"]["Addition"]
+
+    instruction = nada_function["instructions"]
+    return_op = instruction[nada_function['return_instruction_id']]
+
+    assert list(return_op.keys()) == ["Addition"]
+    addition = return_op["Addition"]
+
+    assert input_reference(instruction[addition["right"]]) == "d"
+    addition_left = instruction[addition["left"]]
+    assert list(addition_left.keys()) == ["Addition"]
+    addition = addition_left["Addition"]
+    assert input_reference(instruction[addition["right"]]) == "c"
+
+    addition_left = instruction[addition["left"]]
+    assert list(addition_left.keys()) == ["Addition"]
+    addition = addition_left["Addition"]
+
     check_nada_function_arg_ref(
-        addition["left"], nada_function["id"], "a", "SecretInteger"
+        instruction[addition["left"]], nada_function["id"], "a", "SecretInteger"
     )
     check_nada_function_arg_ref(
-        addition["right"], nada_function["id"], "b", "SecretInteger"
+        instruction[addition["right"]], nada_function["id"], "b", "SecretInteger"
     )
 
 
 @pytest.mark.parametrize(
     ("input_type", "input_name"),
     [(Array, "Array"), (Vector, "Vector")],
 )
@@ -338,49 +377,60 @@
     assert len(args) == 2
     a_arg_type = {input_name: {"inner_type": "SecretInteger"}}
     check_arg(args[0], "a", a_arg_type)
     b_arg_type = {input_name: {"inner_type": "T"}}
     check_arg(args[1], "b", b_arg_type)
     assert matrix_addition_fn["return_type"] == "SecretInteger"
 
-    assert list(matrix_addition_fn["body"].keys()) == ["Reduce"]
-    reduce_op = matrix_addition_fn["body"]["Reduce"]
+    instructions = matrix_addition_fn["instructions"]
+    return_op = instructions[matrix_addition_fn["return_instruction_id"]]
+    assert list(return_op.keys()) == ["Reduce"]
+    reduce_op = return_op["Reduce"]
     reduce_op["function_id"] = add_fn["id"]
     reduce_op["type"] = "SecretInteger"
 
-    assert list(reduce_op["inner"].keys()) == ["Map"]
-    map_op = reduce_op["inner"]["Map"]
+    reduce_op_inner = instructions[reduce_op["inner"]]
+    assert list(reduce_op_inner.keys()) == ["Map"]
+    map_op = reduce_op_inner["Map"]
     map_op["function_id"] = add_fn["id"]
     map_op["type"] = {
         input_name: {"inner_type": "SecretInteger", "size": None}
     }
 
-    assert list(map_op["inner"].keys()) == ["Zip"]
-    zip_op = map_op["inner"]["Zip"]
+    map_op_inner = instructions[map_op["inner"]]
+    assert list(map_op_inner.keys()) == ["Zip"]
+    zip_op = map_op_inner["Zip"]
 
+    zip_op_left = instructions[zip_op["left"]]
+    zip_op_right = instructions[zip_op["right"]]
     check_nada_function_arg_ref(
-        zip_op["left"], matrix_addition_fn["id"], "a", a_arg_type
+        zip_op_left, matrix_addition_fn["id"], "a", a_arg_type
     )
     check_nada_function_arg_ref(
-        zip_op["right"], matrix_addition_fn["id"], "b", b_arg_type
+        zip_op_right, matrix_addition_fn["id"], "b", b_arg_type
     )
 
 
 def test_array_new():
     first_input = create_input(SecretInteger, "first", "party", **{})
     second_input = create_input(SecretInteger, "second", "party", **{})
     array = Array.new(first_input, second_input)
-    op = process_operation(array)
+    instructions = {}
+    op_id = process_operation(array, instructions)
+    op = instructions[op_id]
 
     assert list(op.keys()) == ["New"]
 
     inner = op["New"]
 
-    assert input_reference(inner["elements"][0]) == "first"
-    assert input_reference(inner["elements"][1]) == "second"
+    first = instructions[inner["elements"][0]]
+    second = instructions[inner["elements"][1]]
+
+    assert input_reference(first) == "first"
+    assert input_reference(second) == "second"
     assert inner["type"]["Array"] == {
         "inner_type": "SecretInteger",
         "size": 2,
     }
 
 
 def test_array_new_empty():
@@ -398,22 +448,25 @@
     assert str(e.value) == "All arguments must be of the same type"
 
 
 def test_tuple_new():
     first_input = create_input(SecretInteger, "first", "party", **{})
     second_input = create_input(PublicInteger, "second", "party", **{})
     array = Tuple.new(first_input, second_input)
-    op = process_operation(array)
+    instructions = {}
+    op_id = process_operation(array, instructions)
+    op = instructions[op_id]
 
     assert list(op.keys()) == ["New"]
 
     inner = op["New"]
-
-    assert input_reference(inner["elements"][0]) == "first"
-    assert input_reference(inner["elements"][1]) == "second"
+    left = instructions[inner["elements"][0]]
+    right = instructions[inner["elements"][1]]
+    assert input_reference(left) == "first"
+    assert input_reference(right) == "second"
     assert inner["type"]["Tuple"] == {
         "left_type": "SecretInteger",
         "right_type": "Integer",
     }
 
 
 def test_tuple_new_empty():
```

## nada_dsl/operations.py

```diff
@@ -131,14 +131,22 @@
 class Reveal:
     '''
     secret.reveal()
     '''
     this: AllTypes  # secret to reveal
     source_ref: SourceRef
 
+@dataclass
+class TruncPr:
+    '''
+    left.trunc_pr(right)
+    '''
+    left: AllTypes  # number to truncate
+    right: AllTypes # number of bits to truncate
+    source_ref: SourceRef
 
 def unzip(array: Array[Tuple[T, R]]) -> Tuple[Array[T], Array[R]]:
     right_type = Array.generic_type(array.inner_type.right_type, size=array.size)
     left_type = Array.generic_type(array.inner_type.left_type, size=array.size)
 
     return Tuple(
         right_type=right_type,
```

## Comparing `nada_dsl-0.1.1.dist-info/RECORD` & `nada_dsl-0.2.1.dist-info/RECORD`

 * *Files 26% similar despite different names*

```diff
@@ -1,21 +1,28 @@
-nada_dsl/__init__.py,sha256=DV4DEF5K__SvdoJnVaqmY092SUCz5U_OWH10t3etprA,355
+nada_dsl/__init__.py,sha256=-lYSknGDUXyYKviT79CAWykIEcl6UGXZRWQQVVzwZUE,384
+nada_dsl/audit_strict_test.py,sha256=QEsu6mxi-h4TcKVOFQ2iT9GJY6QKfgyAP3xCkN7Xra8,3040
 nada_dsl/circuit_io.py,sha256=jNynCibfVkwwB2TMRFLmHqWFP5k5EBqVeRvJTUwaLUA,1975
-nada_dsl/compile.py,sha256=9ZAWZxkiyzNTBnZYTVAayHLPamhuARkUIGm_aRmYK0E,2615
-nada_dsl/compile_test.py,sha256=nmgQxlGeK6LfEbIokQ3wUouQUxi88deyv9xYVNIGEjY,529
-nada_dsl/compiler_frontend.py,sha256=U3d8apbRcTagCXuhyI5geYkxOysTm_gDm6x33faxGuQ,12074
-nada_dsl/compiler_frontend_test.py,sha256=RK8Lt27Z7T8-faCWVfyTO0z8lrktYpQl_EXo-ImEFGs,13738
+nada_dsl/compile.py,sha256=o-dyVfUrV1WwHQChWhcjRQvwr5-IJ6qFGvcrVZS67JM,2559
+nada_dsl/compile_test.py,sha256=tneeSwXRUYmL2Td0tbZEqdLrpE-H0rUVBdk4E_H2FMU,512
+nada_dsl/compiler_frontend.py,sha256=1ZCU9i_S5niCtq2pJTMCCccfQ4mI8Mj45r0in87O3KM,15060
+nada_dsl/compiler_frontend_test.py,sha256=vbw6BlgMEapm3CEtu2Rs2KvhTEHdbnq4W9_50Vj_RCQ,15381
 nada_dsl/errors.py,sha256=cDLmAIo3HsdwVzDiKumRJQRNfrhodrB90uaEHetZUAU,99
-nada_dsl/operations.py,sha256=stwkyxmVwPnQTr4XYladuc5xHE1v7ydJAXpixEKc_3I,2549
+nada_dsl/operations.py,sha256=M-8syzZFsE_ZPR1Dfc_ek-mh0OClmrZyJSUXtE58TOU,2732
 nada_dsl/source_ref.py,sha256=P4hRKB9FPrNkxiYw5jtzKvT12X-FxUjIo7PYlZzANPY,2046
+nada_dsl/audit/__init__.py,sha256=6kNPqYFTFgyCEuGBsifi8N34KJlzrnXycheLp9TUvf0,672
+nada_dsl/audit/__main__.py,sha256=2slmlztLqr745Gup92ROfYdTTCQIhovaDvVph0ca0no,95
+nada_dsl/audit/abstract.py,sha256=YES_clrZh-bg1WJplWz8teXtg-On7UKN9hILsClrUpo,37770
+nada_dsl/audit/common.py,sha256=UXdJPcQmsjkod0bqCgvTnBfOonHshe419viW2uk-QjQ,2851
+nada_dsl/audit/report.py,sha256=iPMoBw6TkACKLIE4Shb_xi61Zt796xPQytcQf9xr5rU,14124
+nada_dsl/audit/strict.py,sha256=BaV0X-boNyI6Iva-hUscBRnqCAS2bab97Z1c3bU5T4U,32922
 nada_dsl/future/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 nada_dsl/future/operations.py,sha256=yBStRga6IYbkut6gCdEiD-5hLq9GMo50KZGR0ETz7FA,214
 nada_dsl/nada_types/__init__.py,sha256=PcScrr5zzHsMQtY0W1vvFn_0SaVdgdb3H_eVyaiSdb8,1103
 nada_dsl/nada_types/collections.py,sha256=NtLsxJEaBlAc-MS0Lzq36aqGGH662B6bXNpWnHJBEnU,6273
 nada_dsl/nada_types/function.py,sha256=-SMDBnWlgvFWRvydhIb-Q2oHE5Bzh3rZP6Yzj_bqgPY,2593
 nada_dsl/nada_types/generics.py,sha256=i1bRfs87TRwxkojBce_Jr3TlkTfsR64HT-g9Ym-lmJs,151
-nada_dsl/nada_types/types.py,sha256=pZrHnhJg_bG-8cPHpQf7SzrfswUsi9pdnaKa8jX2h5A,59216
-nada_dsl-0.1.1.dist-info/LICENSE,sha256=sBBGrKOWYbPzZAdvbkzxcmqBg7rSLFeODtZgqMYL5cY,11337
-nada_dsl-0.1.1.dist-info/METADATA,sha256=evFoARbrMZJE-ERuM1zdVDrVMPi-_sFtj7OiCEIsqJo,14148
-nada_dsl-0.1.1.dist-info/WHEEL,sha256=yQN5g4mg4AybRjkgi-9yy4iQEFibGQmlz78Pik5Or-A,92
-nada_dsl-0.1.1.dist-info/top_level.txt,sha256=GOx1gwiez4xwNtM9pHe78Sa5owsJvnUJOgfM1GtZGuM,9
-nada_dsl-0.1.1.dist-info/RECORD,,
+nada_dsl/nada_types/types.py,sha256=d-J1g667Jeq0CcoH4tvvDk_t8gy9aHsCwR3QsV1c6p0,75321
+nada_dsl-0.2.1.dist-info/LICENSE,sha256=sBBGrKOWYbPzZAdvbkzxcmqBg7rSLFeODtZgqMYL5cY,11337
+nada_dsl-0.2.1.dist-info/METADATA,sha256=18OY338uX-KfZPsK0lFbKoaBtVYRkrehAp7lSeCz1PY,14009
+nada_dsl-0.2.1.dist-info/WHEEL,sha256=yQN5g4mg4AybRjkgi-9yy4iQEFibGQmlz78Pik5Or-A,92
+nada_dsl-0.2.1.dist-info/top_level.txt,sha256=GOx1gwiez4xwNtM9pHe78Sa5owsJvnUJOgfM1GtZGuM,9
+nada_dsl-0.2.1.dist-info/RECORD,,
```

## Comparing `nada_dsl-0.1.1.dist-info/LICENSE` & `nada_dsl-0.2.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `nada_dsl-0.1.1.dist-info/METADATA` & `nada_dsl-0.2.1.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nada-dsl
-Version: 0.1.1
+Version: 0.2.1
 Summary: Nillion Nada DSL to create Nillion MPC programs.
 License: Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
         
@@ -204,35 +204,29 @@
            See the License for the specific language governing permissions and
            limitations under the License.
         
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: asttokens ~=2.4
+Requires-Dist: richreports ~=0.2
+Requires-Dist: parsial ~=0.1
 Provides-Extra: docs
 Requires-Dist: toml ~=0.10.2 ; extra == 'docs'
-Requires-Dist: sphinx ~=5.0 ; extra == 'docs'
-Requires-Dist: sphinx-rtd-theme ~=1.0.0 ; extra == 'docs'
+Requires-Dist: sphinx <8,>=5 ; extra == 'docs'
+Requires-Dist: sphinx-rtd-theme <2.1,>=1.0 ; extra == 'docs'
 Provides-Extra: lint
-Requires-Dist: pylint ~=2.17.0 ; extra == 'lint'
+Requires-Dist: pylint <3.2,>=2.17 ; extra == 'lint'
+Provides-Extra: test
+Requires-Dist: pytest <9.0,>=7.4 ; extra == 'test'
+Requires-Dist: pytest-cov <6,>=4 ; extra == 'test'
 
 # nada-dsl
 
 nada-dsl is a Python DSL for building MPC programs on the Nillion Network.
 
-See the official Nillion documentation site for more about the [Nada-Lang
-Framework][framework] and [Nada Program Examples][examples].
+See the official Nillion documentation site for more about the [Nada Language][nada-language] and
+[Nada Program Examples][examples].
 
 [examples]: https://github.com/NillionNetwork/nillion-python-starter/tree/main/programs
-[framework]: https://docs.nillion.com/nada-lang-framework
-
-## Auto-Generated Documentation
-
-Documentation for this package can be generated automatically via the commands below (using a variant of `python` appropriate for the environment):
-
-```console
-python -m pip install '.[docs]'
-cd docs
-sphinx-build . _build
-```
-
-Alternatively, you can use the `just` target (from the root of nillion): `just nada-dsl-doc`
+[nada-language]: https://docs.nillion.com/nada-lang
```

