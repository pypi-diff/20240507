# Comparing `tmp/upc_pymotion-0.1.5.tar.gz` & `tmp/upc_pymotion-0.1.7.tar.gz`

## Comparing `upc_pymotion-0.1.5.tar` & `upc_pymotion-0.1.7.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 upc_pymotion-0.1.5/pymotion/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 upc_pymotion-0.1.5/pymotion/io/__init__.py
--rw-r--r--   0        0        0    16615 2020-02-02 00:00:00.000000 upc_pymotion-0.1.5/pymotion/io/bvh.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 upc_pymotion-0.1.5/pymotion/ops/__init__.py
--rw-r--r--   0        0        0     2296 2020-02-02 00:00:00.000000 upc_pymotion-0.1.5/pymotion/ops/center_of_mass.py
--rw-r--r--   0        0        0     2402 2020-02-02 00:00:00.000000 upc_pymotion-0.1.5/pymotion/ops/center_of_mass_torch.py
--rw-r--r--   0        0        0     1826 2020-02-02 00:00:00.000000 upc_pymotion-0.1.5/pymotion/ops/forward_kinematics.py
--rw-r--r--   0        0        0     1766 2020-02-02 00:00:00.000000 upc_pymotion-0.1.5/pymotion/ops/forward_kinematics_torch.py
--rw-r--r--   0        0        0     3273 2020-02-02 00:00:00.000000 upc_pymotion-0.1.5/pymotion/ops/skeleton.py
--rw-r--r--   0        0        0     3382 2020-02-02 00:00:00.000000 upc_pymotion-0.1.5/pymotion/ops/skeleton_torch.py
--rw-r--r--   0        0        0     2289 2020-02-02 00:00:00.000000 upc_pymotion-0.1.5/pymotion/ops/time.py
--rw-r--r--   0        0        0     2516 2020-02-02 00:00:00.000000 upc_pymotion-0.1.5/pymotion/ops/time_torch.py
--rw-r--r--   0        0        0      727 2020-02-02 00:00:00.000000 upc_pymotion-0.1.5/pymotion/render/__init__.py
--rw-r--r--   0        0        0     2537 2020-02-02 00:00:00.000000 upc_pymotion-0.1.5/pymotion/render/blender.py
--rw-r--r--   0        0        0    19647 2020-02-02 00:00:00.000000 upc_pymotion-0.1.5/pymotion/render/viewer.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 upc_pymotion-0.1.5/pymotion/rotations/__init__.py
--rw-r--r--   0        0        0     5346 2020-02-02 00:00:00.000000 upc_pymotion-0.1.5/pymotion/rotations/dual_quat.py
--rw-r--r--   0        0        0     5759 2020-02-02 00:00:00.000000 upc_pymotion-0.1.5/pymotion/rotations/dual_quat_torch.py
--rw-r--r--   0        0        0     3006 2020-02-02 00:00:00.000000 upc_pymotion-0.1.5/pymotion/rotations/ortho6d.py
--rw-r--r--   0        0        0     3095 2020-02-02 00:00:00.000000 upc_pymotion-0.1.5/pymotion/rotations/ortho6d_torch.py
--rw-r--r--   0        0        0    14671 2020-02-02 00:00:00.000000 upc_pymotion-0.1.5/pymotion/rotations/quat.py
--rw-r--r--   0        0        0    15451 2020-02-02 00:00:00.000000 upc_pymotion-0.1.5/pymotion/rotations/quat_torch.py
--rw-r--r--   0        0        0     3787 2020-02-02 00:00:00.000000 upc_pymotion-0.1.5/.gitignore
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 upc_pymotion-0.1.5/LICENSE
--rw-r--r--   0        0        0     8986 2020-02-02 00:00:00.000000 upc_pymotion-0.1.5/README.md
--rw-r--r--   0        0        0      950 2020-02-02 00:00:00.000000 upc_pymotion-0.1.5/pyproject.toml
--rw-r--r--   0        0        0    11177 2020-02-02 00:00:00.000000 upc_pymotion-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 upc_pymotion-0.1.7/pymotion/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 upc_pymotion-0.1.7/pymotion/io/__init__.py
+-rw-r--r--   0        0        0    16697 2020-02-02 00:00:00.000000 upc_pymotion-0.1.7/pymotion/io/bvh.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 upc_pymotion-0.1.7/pymotion/ops/__init__.py
+-rw-r--r--   0        0        0     2296 2020-02-02 00:00:00.000000 upc_pymotion-0.1.7/pymotion/ops/center_of_mass.py
+-rw-r--r--   0        0        0     2402 2020-02-02 00:00:00.000000 upc_pymotion-0.1.7/pymotion/ops/center_of_mass_torch.py
+-rw-r--r--   0        0        0     1826 2020-02-02 00:00:00.000000 upc_pymotion-0.1.7/pymotion/ops/forward_kinematics.py
+-rw-r--r--   0        0        0     1766 2020-02-02 00:00:00.000000 upc_pymotion-0.1.7/pymotion/ops/forward_kinematics_torch.py
+-rw-r--r--   0        0        0     3273 2020-02-02 00:00:00.000000 upc_pymotion-0.1.7/pymotion/ops/skeleton.py
+-rw-r--r--   0        0        0     3382 2020-02-02 00:00:00.000000 upc_pymotion-0.1.7/pymotion/ops/skeleton_torch.py
+-rw-r--r--   0        0        0     2289 2020-02-02 00:00:00.000000 upc_pymotion-0.1.7/pymotion/ops/time.py
+-rw-r--r--   0        0        0     2516 2020-02-02 00:00:00.000000 upc_pymotion-0.1.7/pymotion/ops/time_torch.py
+-rw-r--r--   0        0        0      727 2020-02-02 00:00:00.000000 upc_pymotion-0.1.7/pymotion/render/__init__.py
+-rw-r--r--   0        0        0     2537 2020-02-02 00:00:00.000000 upc_pymotion-0.1.7/pymotion/render/blender.py
+-rw-r--r--   0        0        0    19647 2020-02-02 00:00:00.000000 upc_pymotion-0.1.7/pymotion/render/viewer.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 upc_pymotion-0.1.7/pymotion/rotations/__init__.py
+-rw-r--r--   0        0        0     5346 2020-02-02 00:00:00.000000 upc_pymotion-0.1.7/pymotion/rotations/dual_quat.py
+-rw-r--r--   0        0        0     5759 2020-02-02 00:00:00.000000 upc_pymotion-0.1.7/pymotion/rotations/dual_quat_torch.py
+-rw-r--r--   0        0        0     3006 2020-02-02 00:00:00.000000 upc_pymotion-0.1.7/pymotion/rotations/ortho6d.py
+-rw-r--r--   0        0        0     3095 2020-02-02 00:00:00.000000 upc_pymotion-0.1.7/pymotion/rotations/ortho6d_torch.py
+-rw-r--r--   0        0        0    14671 2020-02-02 00:00:00.000000 upc_pymotion-0.1.7/pymotion/rotations/quat.py
+-rw-r--r--   0        0        0    15451 2020-02-02 00:00:00.000000 upc_pymotion-0.1.7/pymotion/rotations/quat_torch.py
+-rw-r--r--   0        0        0     3787 2020-02-02 00:00:00.000000 upc_pymotion-0.1.7/.gitignore
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 upc_pymotion-0.1.7/LICENSE
+-rw-r--r--   0        0        0     8986 2020-02-02 00:00:00.000000 upc_pymotion-0.1.7/README.md
+-rw-r--r--   0        0        0      950 2020-02-02 00:00:00.000000 upc_pymotion-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0    11177 2020-02-02 00:00:00.000000 upc_pymotion-0.1.7/PKG-INFO
```

### Comparing `upc_pymotion-0.1.5/pymotion/io/bvh.py` & `upc_pymotion-0.1.7/pymotion/io/bvh.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,24 +30,24 @@
         filename : str
             path to the file.
 
         Results
         ------
         self.data : dict
             dictionary with the data.
-            ["names"] : list[str]
+            ["names"] : np.array[str]
                 ith-element contain the name of ith-joint.
             ["offsets"] : np.array[n_joints, 3]
                 ith-element contain the offset of ith-joint wrt. its parent joint.
             ["end_sites"] : np.array[n_end_sites, 3]
                 ith-element contain the offset of ith-end-site wrt. its parent joint.
-            ["end_sites_parents"] : list[int]
+            ["end_sites_parents"] : np.array[int]
                 ith-element contain the joint parent of the ith end-site.
-            ["parents"] : list[int]
-                ith-element contain the parent of the ith joint.
+            ["parents"] : np.array[int]
+                ith-element contain the parent of the ith joint. The root joint has parent 0 (itself).
             ["rot_order"] : np.array[n_joints, 3]
                 order per channel of the rotations. The order is 'x', 'y' or 'z'.
             ["positions"] : np.array[n_frames, n_joints, 3]
                 local positions.
             ["rotations"] : np.array[n_frames, n_joints, 3]
                 local rotations in euler angles with the order specified in rot_order.
             ["frame_time"] : float
@@ -114,17 +114,21 @@
                     elif number_channels == 3:
                         rot_order[current] = [self.bvh_rot_map[x] for x in words[2 : 2 + 3]]
                     else:
                         raise Exception("Unknown number of channels")
                     continue
 
                 if "Frames" in line:
+                    names = np.array(names)
                     number_frames = int(line.split()[1])
                     offsets = np.array(offsets)
+                    parents[0] = 0
+                    parents = np.array(parents)
                     end_sites = np.array(end_sites)
+                    end_sites_parents = np.array(end_sites_parents)
                     rot_order = np.array(rot_order)
                     positions = np.tile(offsets, (number_frames, 1)).reshape(number_frames, len(offsets), 3)
                     rotations = np.zeros((number_frames, len(names), 3))
                     continue
 
                 if "Frame Time" in line:
                     frame_time = float(line.split()[2])
@@ -165,15 +169,14 @@
         filename : str
             path to the file.
         data : dict
             dictionary with the data following the
             returned dict structure from load(...).
             positions in data["positions"] are assumed to be X,Y,Z order.
             rotations in data["rotations"] are assumed to be in the specified order in data["rot_order"].
-            if data == None, then self.data is used.
         """
 
         with open(filename, "w") as f:
             tab = ""
             f.write("%sHIERARCHY\n" % tab)
             f.write("%sROOT %s\n" % (tab, self.data["names"][0]))
             f.write("%s{\n" % tab)
@@ -197,15 +200,15 @@
                     self.inv_bvh_rot_map[self.data["rot_order"][0, 2]],
                 )
             )
 
             joint_order = [0]
 
             for i in range(len(self.data["parents"])):
-                if self.data["parents"][i] == 0:
+                if self.data["parents"][i] == 0 and i != 0:
                     tab = self._save_joint(f, self.data, tab, i, joint_order)
 
             tab = tab[:-1]
             f.write("%s}\n" % tab)
 
             f.write("%sMOTION\n" % tab)
             f.write("%sFrames: %d\n" % (tab, self.data["positions"].shape[0]))
@@ -253,20 +256,20 @@
         assert order[0] == 0, "root joint should not change"
         assert len(order) == len(
             self.data["names"]
         ), "order should have the same number of joints as the original bvh file"
 
         reverse_order = [order.index(i) for i in range(len(order))]
 
-        self.data["names"] = [self.data["names"][reverse_order[i]] for i in range(len(order))]
+        self.data["names"] = np.array([self.data["names"][reverse_order[i]] for i in range(len(order))])
         self.data["offsets"] = self.data["offsets"][reverse_order]
-        self.data["end_sites_parents"] = [order[j] for j in self.data["end_sites_parents"]]
-        self.data["parents"][0] = 0
-        self.data["parents"] = [order[self.data["parents"][reverse_order[i]]] for i in range(len(order))]
-        self.data["parents"][0] = None
+        self.data["end_sites_parents"] = np.array([order[j] for j in self.data["end_sites_parents"]])
+        self.data["parents"] = np.array(
+            [order[self.data["parents"][reverse_order[i]]] for i in range(len(order))]
+        )
         self.data["rot_order"] = self.data["rot_order"][reverse_order]
         self.data["positions"] = self.data["positions"][:, reverse_order]
         self.data["rotations"] = self.data["rotations"][:, reverse_order]
 
     def remove_joints(self, delete_joints: list[int]):
         """
         Removes joints from the .bvh file.
@@ -300,85 +303,83 @@
                 parents[j] = parents[p]
 
         # Update parent indices for remaining joints
         new_parents = [0] * len(keep_joints)
         for i, p in enumerate(parents):
             if i in keep_joints:
                 new_parents[old_to_new[i]] = old_to_new[p]
-        new_parents[0] = None
 
         # Update end_sites_parents to reflect the removal of joints
         updated_end_sites_parents = [
             old_to_new[es_parent] for es_parent in end_sites_parents if es_parent in old_to_new
         ]
         # Remove end sites associated with deleted joints, if necessary
         valid_end_sites_indices = [
             i for i, es_parent in enumerate(end_sites_parents) if es_parent not in delete_joints
         ]
 
         # Update data
-        self.data["names"] = [self.data["names"][i] for i in keep_joints]
+        self.data["names"] = np.array([self.data["names"][i] for i in keep_joints])
         self.data["rot_order"] = self.data["rot_order"][..., keep_joints, :]
         self.data["positions"] = new_pos
         self.data["rotations"] = np.degrees(
             quat.to_euler(new_rots, order=np.tile(self.data["rot_order"], (rots.shape[0], 1, 1)))
         )
-        self.data["parents"] = new_parents
+        self.data["parents"] = np.array(new_parents)
         self.data["offsets"] = new_offsets
         self.data["end_sites"] = end_sites[valid_end_sites_indices]
-        self.data["end_sites_parents"] = updated_end_sites_parents
+        self.data["end_sites_parents"] = np.array(updated_end_sites_parents)
 
     def get_data(self):
         """
         Returns unrolled rotations (transformed to quaternions),
         positions, parents and offsets.
 
         Returns
         -------
         rots : np.array[n_frames, n_joints, 4]
             unrolled local rotations (transformed to quaternions).
         pos : np.array[n_frames, n_joints, 3]
             local positions.
-        parents : list[int]
+        parents : np.array[int]
             ith-element contain the parent of the ith joint.
         offsets : np.array[n_joints, 3]
             ith-element contain the offset of ith-joint wrt. its parent joint.
         end_sites : np.array[n_joints, 3]
             ith-element contain the offset of ith-end-site wrt. its parent joint.
-        end_sites_parents : list[int]
+        end_sites_parents : np.array[int]
             ith-element contain the joint parent of the ith end-site.
         """
         rots = quat.unroll(
             quat.from_euler(
                 np.radians(self.data["rotations"]),
                 order=np.tile(self.data["rot_order"], (self.data["rotations"].shape[0], 1, 1)),
             ),
             axis=0,
         )
         rots = quat.normalize(rots)  # make sure all quaternions are unit quaternions
         pos = self.data["positions"]
         parents = self.data["parents"]
-        parents[0] = 0  # BVH sets root as None
         offsets = self.data["offsets"]
         end_sites = self.data["end_sites"]
         end_sites_parents = self.data["end_sites_parents"]
-        return rots, pos, np.array(parents), offsets, end_sites, end_sites_parents
+        return rots, pos, parents, offsets, end_sites, end_sites_parents
 
     def set_data(self, rots, pos):
         """
         Sets the data of the BVH from rotations represented as quaternions,
         positions, parents and offsets.
 
         Parameters
         ----------
         rots : np.array[n_frames, n_joints, 4]
             local rotations (quaternions).
         pos : np.array[n_frames, n_joints, 3]
             local positions.
-        parents : list[int]
+        parents : np.array[int]
             ith-element contain the parent of the ith joint.
         offsets : np.array[n_joints, 3]
             ith-element contain the offset of ith-joint wrt. its parent joint.
         """
         assert (
             self.data is not None
         ), "load a BVH file first or create a self.data dict with the same structure as the one returned by load(...)"
@@ -386,15 +387,14 @@
             self.data["rot_order"] is not None
         ), "load a BVH file first or create a self.data dict with the same structure as the one returned by load(...)"
 
         self.data["rotations"] = np.degrees(
             quat.to_euler(rots, order=np.tile(self.data["rot_order"], (rots.shape[0], 1, 1)))
         )
         self.data["positions"] = pos
-        self.data["parents"][0] = None  # BVH sets root as None
 
     def _save_joint(self, f, data, tab, i, joint_order):
         joint_order.append(i)
 
         f.write("%sJOINT %s\n" % (tab, data["names"][i]))
         f.write("%s{\n" % tab)
         tab += "\t"
@@ -426,15 +426,15 @@
                 is_end_site = False
 
         if is_end_site:
             f.write("%sEnd Site\n" % tab)
             f.write("%s{\n" % tab)
             tab += "\t"
             try:
-                end_site_data = data["end_sites"][data["end_sites_parents"].index(i)]
+                end_site_data = data["end_sites"][np.where(data["end_sites_parents"] == i)[0][0]]
             except ValueError:
                 end_site_data = np.zeros(3)
             f.write("%sOFFSET %f %f %f\n" % (tab, end_site_data[0], end_site_data[1], end_site_data[2]))
             tab = tab[:-1]
             f.write("%s}\n" % tab)
 
         tab = tab[:-1]
```

### Comparing `upc_pymotion-0.1.5/pymotion/ops/center_of_mass.py` & `upc_pymotion-0.1.7/pymotion/ops/center_of_mass.py`

 * *Files identical despite different names*

### Comparing `upc_pymotion-0.1.5/pymotion/ops/center_of_mass_torch.py` & `upc_pymotion-0.1.7/pymotion/ops/center_of_mass_torch.py`

 * *Files identical despite different names*

### Comparing `upc_pymotion-0.1.5/pymotion/ops/forward_kinematics.py` & `upc_pymotion-0.1.7/pymotion/ops/forward_kinematics.py`

 * *Files identical despite different names*

### Comparing `upc_pymotion-0.1.5/pymotion/ops/forward_kinematics_torch.py` & `upc_pymotion-0.1.7/pymotion/ops/forward_kinematics_torch.py`

 * *Files identical despite different names*

### Comparing `upc_pymotion-0.1.5/pymotion/ops/skeleton.py` & `upc_pymotion-0.1.7/pymotion/ops/skeleton.py`

 * *Files identical despite different names*

### Comparing `upc_pymotion-0.1.5/pymotion/ops/skeleton_torch.py` & `upc_pymotion-0.1.7/pymotion/ops/skeleton_torch.py`

 * *Files identical despite different names*

### Comparing `upc_pymotion-0.1.5/pymotion/ops/time.py` & `upc_pymotion-0.1.7/pymotion/ops/time.py`

 * *Files identical despite different names*

### Comparing `upc_pymotion-0.1.5/pymotion/ops/time_torch.py` & `upc_pymotion-0.1.7/pymotion/ops/time_torch.py`

 * *Files identical despite different names*

### Comparing `upc_pymotion-0.1.5/pymotion/render/__init__.py` & `upc_pymotion-0.1.7/pymotion/render/__init__.py`

 * *Files identical despite different names*

### Comparing `upc_pymotion-0.1.5/pymotion/render/blender.py` & `upc_pymotion-0.1.7/pymotion/render/blender.py`

 * *Files identical despite different names*

### Comparing `upc_pymotion-0.1.5/pymotion/render/viewer.py` & `upc_pymotion-0.1.7/pymotion/render/viewer.py`

 * *Files identical despite different names*

### Comparing `upc_pymotion-0.1.5/pymotion/rotations/dual_quat.py` & `upc_pymotion-0.1.7/pymotion/rotations/dual_quat.py`

 * *Files identical despite different names*

### Comparing `upc_pymotion-0.1.5/pymotion/rotations/dual_quat_torch.py` & `upc_pymotion-0.1.7/pymotion/rotations/dual_quat_torch.py`

 * *Files identical despite different names*

### Comparing `upc_pymotion-0.1.5/pymotion/rotations/ortho6d.py` & `upc_pymotion-0.1.7/pymotion/rotations/ortho6d.py`

 * *Files identical despite different names*

### Comparing `upc_pymotion-0.1.5/pymotion/rotations/ortho6d_torch.py` & `upc_pymotion-0.1.7/pymotion/rotations/ortho6d_torch.py`

 * *Files identical despite different names*

### Comparing `upc_pymotion-0.1.5/pymotion/rotations/quat.py` & `upc_pymotion-0.1.7/pymotion/rotations/quat.py`

 * *Files identical despite different names*

### Comparing `upc_pymotion-0.1.5/pymotion/rotations/quat_torch.py` & `upc_pymotion-0.1.7/pymotion/rotations/quat_torch.py`

 * *Files identical despite different names*

### Comparing `upc_pymotion-0.1.5/.gitignore` & `upc_pymotion-0.1.7/.gitignore`

 * *Files identical despite different names*

### Comparing `upc_pymotion-0.1.5/LICENSE` & `upc_pymotion-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `upc_pymotion-0.1.5/README.md` & `upc_pymotion-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `upc_pymotion-0.1.5/pyproject.toml` & `upc_pymotion-0.1.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 [tool.hatch.build]
 include = ["pymotion/*"]
 exclude = ["*test*"]
 
 [project]
 name = "upc-pymotion"
-version = "0.1.5"
+version = "0.1.7"
 description = "A Python library for working with motion data in NumPy or PyTorch."
 readme = "README.md"
 authors = [{ name = "Jose Luis Ponton", email = "jose.luis.ponton@upc.edu" }]
 license = { file = "LICENSE" }
 classifiers = [
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
```

### Comparing `upc_pymotion-0.1.5/PKG-INFO` & `upc_pymotion-0.1.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: upc-pymotion
-Version: 0.1.5
+Version: 0.1.7
 Summary: A Python library for working with motion data in NumPy or PyTorch.
 Project-URL: Homepage, https://github.com/UPC-ViRVIG/pymotion
 Author-email: Jose Luis Ponton <jose.luis.ponton@upc.edu>
 License: MIT License
         
         Copyright (c) 2024 Jose Luis Ponton
```

