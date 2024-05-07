# Comparing `tmp/trc_data_reader-0.3.3-py3-none-any.whl.zip` & `tmp/trc_data_reader-0.3.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 10372 bytes, number of entries: 6
--rw-r--r--  2.0 unx    15713 b- defN 24-Apr-18 03:32 trc.py
--rw-r--r--  2.0 unx    11357 b- defN 24-Apr-18 03:32 trc_data_reader-0.3.3.dist-info/LICENSE
--rw-r--r--  2.0 unx     1453 b- defN 24-Apr-18 03:32 trc_data_reader-0.3.3.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Apr-18 03:32 trc_data_reader-0.3.3.dist-info/WHEEL
--rw-r--r--  2.0 unx        4 b- defN 24-Apr-18 03:32 trc_data_reader-0.3.3.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      490 b- defN 24-Apr-18 03:32 trc_data_reader-0.3.3.dist-info/RECORD
-6 files, 29109 bytes uncompressed, 9484 bytes compressed:  67.4%
+Zip file size: 10962 bytes, number of entries: 6
+-rw-r--r--  2.0 unx    17855 b- defN 24-May-07 06:46 trc.py
+-rw-r--r--  2.0 unx    11357 b- defN 24-May-07 06:46 trc_data_reader-0.3.4.dist-info/LICENSE
+-rw-r--r--  2.0 unx     1453 b- defN 24-May-07 06:46 trc_data_reader-0.3.4.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-07 06:46 trc_data_reader-0.3.4.dist-info/WHEEL
+-rw-r--r--  2.0 unx        4 b- defN 24-May-07 06:46 trc_data_reader-0.3.4.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      490 b- defN 24-May-07 06:46 trc_data_reader-0.3.4.dist-info/RECORD
+6 files, 31251 bytes uncompressed, 10074 bytes compressed:  67.8%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: trc.py
 Comment: 
 
-Filename: trc_data_reader-0.3.3.dist-info/LICENSE
+Filename: trc_data_reader-0.3.4.dist-info/LICENSE
 Comment: 
 
-Filename: trc_data_reader-0.3.3.dist-info/METADATA
+Filename: trc_data_reader-0.3.4.dist-info/METADATA
 Comment: 
 
-Filename: trc_data_reader-0.3.3.dist-info/WHEEL
+Filename: trc_data_reader-0.3.4.dist-info/WHEEL
 Comment: 
 
-Filename: trc_data_reader-0.3.3.dist-info/top_level.txt
+Filename: trc_data_reader-0.3.4.dist-info/top_level.txt
 Comment: 
 
-Filename: trc_data_reader-0.3.3.dist-info/RECORD
+Filename: trc_data_reader-0.3.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## trc.py

```diff
@@ -1,8 +1,10 @@
 import os
+import math
+
 import c3d
 
 
 _REQUIRED_HEADER_KEYS = ['DataRate', 'CameraRate', 'NumFrames', 'NumMarkers', 'Units', 'OrigDataRate']
 _HEADER_KEYS = ['DataRate', 'CameraRate', 'NumFrames', 'NumMarkers', 'Units', 'OrigDataRate', 'OrigDataStartFrame', 'OrigNumFrames']
 _HEADER_TYPES = [float, float, int, int, str, float, int, int]
 _COORDINATE_LABELS = ['X', 'Y', 'Z']
@@ -158,14 +160,17 @@
         """
         Parse trc formatted motion capture data into a dictionary like object.
 
         :param data: The multi-line string of the data to parse.
         :param line_sep: The line separator to split lines with.
         """
         contents = data.split(line_sep)
+        if len(contents) == 1:
+            data.replace('\r\n', '\n')
+            contents = data.split('\n')
         self._process_contents(contents)
 
     def load(self, filename, encoding="utf-8", errors="strict"):
         """
         Load a trc motion capture data file into a dictionary like object.
 
         :param filename: The name of the file to load.
@@ -174,57 +179,90 @@
         """
         with open(filename, 'rb') as f:
             contents = f.read().decode(encoding=encoding, errors=errors)
 
         contents = contents.split(os.linesep)
         self._process_contents(contents)
 
-    def _import_from_c3d(self, filename):
+    def _import_from_c3d(self, filename, filter_output=None, label_params=None):
         """
         Extracts TRC data from a C3D file.
 
         :param filename: The C3D file to be parsed.
+        :param filter_output: Optional; A list of model-output parameters to be filtered out from
+            the list of marker labels (e.g., ANGLES, FORCES, MOMENTS, POWERS, SCALARS).
+        :param label_params: Optional; A list of label parameters to be checked for marker labels.
         """
         with open(filename, 'rb') as handle:
             reader = c3d.Reader(handle)
 
             # Set file metadata.
             self['PathFileType'] = 3
             self['DataFormat'] = "(X/Y/Z)"
             self['FileName'] = os.path.basename(filename)
 
             # Set file header values.
             self['DataRate'] = reader.header.frame_rate
             self['CameraRate'] = reader.header.frame_rate
-            self['NumFrames'] = reader.header.last_frame
-            self['NumMarkers'] = reader.get('POINT').get('USED').int16_value
+            self['NumFrames'] = reader.header.last_frame - reader.header.first_frame + 1
             self['Units'] = reader.get('POINT').get('UNITS').string_value
             self['OrigDataRate'] = reader.header.frame_rate
             self['OrigDataStartFrame'] = reader.header.first_frame
             self['OrigNumFrames'] = reader.header.last_frame - reader.header.first_frame + 1
 
-            # Set data column labels.
-            self['Markers'] = [label.strip() for label in reader.point_labels]
-
             # Set frame numbers.
             self['Frame#'] = [i for i in range(reader.header.first_frame, reader.header.last_frame + 1)]
 
+            if filter_output is None:
+                filter_output = ['ANGLES', 'FORCES', 'MOMENTS', 'POWERS', 'SCALARS']
+            if label_params is None:
+                label_params = ['LABELS', 'LABELS2']
+
+            # Filter out model outputs (Angles, Forces, Moments, Powers, Scalars) from point labels.
+            point_group = reader.get('POINT')
+            model_outputs = set()
+            for param in filter_output:
+                if param in point_group.param_keys():
+                    model_outputs.update(point_group.get(param).string_array)
+            point_labels = []
+            for param in label_params:
+                if param in point_group.param_keys():
+                    filtered_labels = [None if label in model_outputs else label.strip() for label in point_group.get(param).string_array]
+                    point_labels.extend(filtered_labels)
+
+            # Set marker labels.
+            self['Markers'] = [label for label in point_labels if label]
+            self['NumMarkers'] = len(self['Markers'])
+
             # Set marker data.
             for i, points, analog in reader.read_frames():
                 time = (i - 1) * (1 / reader.point_rate)
-                self[i] = time, [point[:3].tolist() for point in points]
+                point_data = []
+                for j in range(len(points)):
+                    if point_labels[j]:
+                        coordinates = points[j][:3].tolist()
+                        errors = points[j][3:]
+                        for error in errors:
+                            if error == -1:
+                                coordinates = _convert_coordinates(['', '', ''])
+                                break
+                        point_data.append(coordinates)
+                self[i] = time, point_data
 
-    def import_from(self, filename):
+    def import_from(self, filename, *args, **kwargs):
         """
         Import data from a non-TRC file source.
-        Currently, the only alternative supported format is c3d.
+        Currently, the only alternative supported format is c3d. The C3D import method also
+        accepts: `filter_output`, an optional argument allowing the user to specify C3D model-
+        output groups that should be filtered out from the list of marker labels; and
+        `label_params`, an optional list of the C3D parameters containing the marker labels.
 
         :param filename: The source file of the data to be imported.
         """
-        self._import_from_c3d(filename)
+        self._import_from_c3d(filename, *args, **kwargs)
 
     def save(self, filename):
         if 'PathFileType' in self:
             header_line_1 = f"PathFileType\t{self['PathFileType']}\t{self['DataFormat']}\t{self['FileName']}{os.linesep}"
         else:
             raise NotImplementedError('Do not know this file type.')
 
@@ -237,15 +275,15 @@
 
         header_line_2 = '\t'.join(_HEADER_KEYS) + os.linesep
         header_line_3 = '\t'.join([str(_convert_header_key_value_to_type(key, self[key])) for key in _HEADER_KEYS]) + os.linesep
 
         coordinate_labels = _COORDINATE_LABELS[:data_format_count]
         markers_header = [entry for marker in self['Markers'] for entry in [marker, '', '']]
         marker_sub_heading = [f'{coordinate}{i + 1}' for i in range(len(self['Markers'])) for coordinate in coordinate_labels]
-        data_header_line_1 = 'Frame#\tTime\t' + '\t'.join(markers_header).strip() + os.linesep
+        data_header_line_1 = 'Frame#\tTime\t' + '\t'.join(markers_header) + os.linesep
         data_header_line_2 = '\t\t' + '\t'.join(marker_sub_heading) + os.linesep
 
         blank_line = os.linesep
 
         with open(filename, 'w', newline='') as f:
 
             f.write(header_line_1)
@@ -255,15 +293,15 @@
             f.write(data_header_line_1)
             f.write(data_header_line_2)
 
             f.write(blank_line)
 
             for frame in self['Frame#']:
                 time, line_data = self[frame]
-                values = [f'{v:.5f}' for values in line_data for v in values]
+                values = ['' if math.isnan(v) else f'{v:.5f}' for values in line_data for v in values]
                 numeric_values = '\t'.join(values)
                 f.write(f'{frame}\t{time:.3f}\t{numeric_values}{os.linesep}')
 
 
 # #!/usr/bin/env python
 # '''This creates an app to launch a python script. The app is
 # created in the directory where python is called. A version of Python
```

## Comparing `trc_data_reader-0.3.3.dist-info/LICENSE` & `trc_data_reader-0.3.4.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `trc_data_reader-0.3.3.dist-info/METADATA` & `trc_data_reader-0.3.4.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trc-data-reader
-Version: 0.3.3
+Version: 0.3.4
 Summary: A package for reading track row column (trc) motion capture data.
 Home-page: https://github.com/hsorby/trc-data-reader
 Author: Hugh Sorby
 Author-email: h.sorby@auckland.ac.nz
 License: Apache 2.0
 Description-Content-Type: text/x-rst
 License-File: LICENSE
```

