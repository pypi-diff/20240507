# Comparing `tmp/pytorch_volumetric-0.5.0.tar.gz` & `tmp/pytorch_volumetric-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytorch_volumetric-0.5.0.tar", last modified: Thu Jan 25 21:48:59 2024, max compression
+gzip compressed data, was "pytorch_volumetric-0.5.2.tar", last modified: Mon May  6 22:49:46 2024, max compression
```

## Comparing `pytorch_volumetric-0.5.0.tar` & `pytorch_volumetric-0.5.2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxr-x   0 zhsh      (1001) zhsh      (1001)        0 2024-01-25 21:48:59.154377 pytorch_volumetric-0.5.0/
--rw-rw-r--   0 zhsh      (1001) zhsh      (1001)     1075 2023-02-10 04:07:46.000000 pytorch_volumetric-0.5.0/LICENSE.txt
--rw-r--r--   0 zhsh      (1001) zhsh      (1001)     8609 2024-01-25 21:48:59.154377 pytorch_volumetric-0.5.0/PKG-INFO
--rw-rw-r--   0 zhsh      (1001) zhsh      (1001)     6258 2024-01-25 21:47:26.000000 pytorch_volumetric-0.5.0/README.md
--rw-rw-r--   0 zhsh      (1001) zhsh      (1001)     4238 2024-01-25 21:48:19.000000 pytorch_volumetric-0.5.0/pyproject.toml
--rw-rw-r--   0 zhsh      (1001) zhsh      (1001)       38 2024-01-25 21:48:59.154377 pytorch_volumetric-0.5.0/setup.cfg
-drwxrwxr-x   0 zhsh      (1001) zhsh      (1001)        0 2024-01-25 21:48:59.150376 pytorch_volumetric-0.5.0/src/
-drwxrwxr-x   0 zhsh      (1001) zhsh      (1001)        0 2024-01-25 21:48:59.154377 pytorch_volumetric-0.5.0/src/pytorch_volumetric/
--rw-rw-r--   0 zhsh      (1001) zhsh      (1001)      670 2024-01-25 21:07:30.000000 pytorch_volumetric-0.5.0/src/pytorch_volumetric/__init__.py
--rw-rw-r--   0 zhsh      (1001) zhsh      (1001)     7183 2023-08-14 19:52:35.000000 pytorch_volumetric-0.5.0/src/pytorch_volumetric/chamfer.py
--rw-rw-r--   0 zhsh      (1001) zhsh      (1001)     8121 2024-01-25 02:03:45.000000 pytorch_volumetric-0.5.0/src/pytorch_volumetric/model_to_sdf.py
--rw-rw-r--   0 zhsh      (1001) zhsh      (1001)    30065 2024-01-25 21:36:00.000000 pytorch_volumetric-0.5.0/src/pytorch_volumetric/sdf.py
--rw-rw-r--   0 zhsh      (1001) zhsh      (1001)     3755 2023-08-31 19:01:35.000000 pytorch_volumetric-0.5.0/src/pytorch_volumetric/visualization.py
--rw-rw-r--   0 zhsh      (1001) zhsh      (1001)      428 2024-01-17 23:13:19.000000 pytorch_volumetric-0.5.0/src/pytorch_volumetric/volume.py
--rw-rw-r--   0 zhsh      (1001) zhsh      (1001)     5796 2024-01-25 00:32:52.000000 pytorch_volumetric-0.5.0/src/pytorch_volumetric/voxel.py
-drwxrwxr-x   0 zhsh      (1001) zhsh      (1001)        0 2024-01-25 21:48:59.154377 pytorch_volumetric-0.5.0/src/pytorch_volumetric.egg-info/
--rw-r--r--   0 zhsh      (1001) zhsh      (1001)     8609 2024-01-25 21:48:59.000000 pytorch_volumetric-0.5.0/src/pytorch_volumetric.egg-info/PKG-INFO
--rw-rw-r--   0 zhsh      (1001) zhsh      (1001)      599 2024-01-25 21:48:59.000000 pytorch_volumetric-0.5.0/src/pytorch_volumetric.egg-info/SOURCES.txt
--rw-rw-r--   0 zhsh      (1001) zhsh      (1001)        1 2024-01-25 21:48:59.000000 pytorch_volumetric-0.5.0/src/pytorch_volumetric.egg-info/dependency_links.txt
--rw-rw-r--   0 zhsh      (1001) zhsh      (1001)      114 2024-01-25 21:48:59.000000 pytorch_volumetric-0.5.0/src/pytorch_volumetric.egg-info/requires.txt
--rw-rw-r--   0 zhsh      (1001) zhsh      (1001)       19 2024-01-25 21:48:59.000000 pytorch_volumetric-0.5.0/src/pytorch_volumetric.egg-info/top_level.txt
-drwxrwxr-x   0 zhsh      (1001) zhsh      (1001)        0 2024-01-25 21:48:59.154377 pytorch_volumetric-0.5.0/tests/
--rw-rw-r--   0 zhsh      (1001) zhsh      (1001)     5993 2023-11-21 20:38:03.000000 pytorch_volumetric-0.5.0/tests/test_chamfer.py
--rw-rw-r--   0 zhsh      (1001) zhsh      (1001)     9777 2023-11-02 20:34:23.000000 pytorch_volumetric-0.5.0/tests/test_model_to_sdf.py
--rw-rw-r--   0 zhsh      (1001) zhsh      (1001)     4064 2023-12-15 19:28:01.000000 pytorch_volumetric-0.5.0/tests/test_sdf.py
--rw-rw-r--   0 zhsh      (1001) zhsh      (1001)     1300 2023-09-28 22:41:17.000000 pytorch_volumetric-0.5.0/tests/test_voxel_sdf.py
+drwxrwxr-x   0 zhsh      (1002) zhsh      (1002)        0 2024-05-06 22:49:46.597101 pytorch_volumetric-0.5.2/
+-rw-rw-r--   0 zhsh      (1002) zhsh      (1002)     1075 2024-05-01 19:56:53.000000 pytorch_volumetric-0.5.2/LICENSE.txt
+-rw-r--r--   0 zhsh      (1002) zhsh      (1002)     8755 2024-05-06 22:49:46.593101 pytorch_volumetric-0.5.2/PKG-INFO
+-rw-rw-r--   0 zhsh      (1002) zhsh      (1002)     6404 2024-05-06 18:17:15.000000 pytorch_volumetric-0.5.2/README.md
+-rw-rw-r--   0 zhsh      (1002) zhsh      (1002)     4238 2024-05-06 22:46:23.000000 pytorch_volumetric-0.5.2/pyproject.toml
+-rw-rw-r--   0 zhsh      (1002) zhsh      (1002)       38 2024-05-06 22:49:46.597101 pytorch_volumetric-0.5.2/setup.cfg
+drwxrwxr-x   0 zhsh      (1002) zhsh      (1002)        0 2024-05-06 22:49:46.593101 pytorch_volumetric-0.5.2/src/
+drwxrwxr-x   0 zhsh      (1002) zhsh      (1002)        0 2024-05-06 22:49:46.593101 pytorch_volumetric-0.5.2/src/pytorch_volumetric/
+-rw-rw-r--   0 zhsh      (1002) zhsh      (1002)      670 2024-05-01 19:56:53.000000 pytorch_volumetric-0.5.2/src/pytorch_volumetric/__init__.py
+-rw-rw-r--   0 zhsh      (1002) zhsh      (1002)     7183 2024-05-01 19:56:53.000000 pytorch_volumetric-0.5.2/src/pytorch_volumetric/chamfer.py
+-rw-rw-r--   0 zhsh      (1002) zhsh      (1002)     8121 2024-05-01 19:56:53.000000 pytorch_volumetric-0.5.2/src/pytorch_volumetric/model_to_sdf.py
+-rw-rw-r--   0 zhsh      (1002) zhsh      (1002)    30680 2024-05-06 18:15:50.000000 pytorch_volumetric-0.5.2/src/pytorch_volumetric/sdf.py
+-rw-rw-r--   0 zhsh      (1002) zhsh      (1002)     3779 2024-05-01 19:56:53.000000 pytorch_volumetric-0.5.2/src/pytorch_volumetric/visualization.py
+-rw-rw-r--   0 zhsh      (1002) zhsh      (1002)      428 2024-05-01 19:56:53.000000 pytorch_volumetric-0.5.2/src/pytorch_volumetric/volume.py
+-rw-rw-r--   0 zhsh      (1002) zhsh      (1002)     6245 2024-05-06 22:44:34.000000 pytorch_volumetric-0.5.2/src/pytorch_volumetric/voxel.py
+drwxrwxr-x   0 zhsh      (1002) zhsh      (1002)        0 2024-05-06 22:49:46.593101 pytorch_volumetric-0.5.2/src/pytorch_volumetric.egg-info/
+-rw-r--r--   0 zhsh      (1002) zhsh      (1002)     8755 2024-05-06 22:49:46.000000 pytorch_volumetric-0.5.2/src/pytorch_volumetric.egg-info/PKG-INFO
+-rw-rw-r--   0 zhsh      (1002) zhsh      (1002)      599 2024-05-06 22:49:46.000000 pytorch_volumetric-0.5.2/src/pytorch_volumetric.egg-info/SOURCES.txt
+-rw-rw-r--   0 zhsh      (1002) zhsh      (1002)        1 2024-05-06 22:49:46.000000 pytorch_volumetric-0.5.2/src/pytorch_volumetric.egg-info/dependency_links.txt
+-rw-rw-r--   0 zhsh      (1002) zhsh      (1002)      114 2024-05-06 22:49:46.000000 pytorch_volumetric-0.5.2/src/pytorch_volumetric.egg-info/requires.txt
+-rw-rw-r--   0 zhsh      (1002) zhsh      (1002)       19 2024-05-06 22:49:46.000000 pytorch_volumetric-0.5.2/src/pytorch_volumetric.egg-info/top_level.txt
+drwxrwxr-x   0 zhsh      (1002) zhsh      (1002)        0 2024-05-06 22:49:46.593101 pytorch_volumetric-0.5.2/tests/
+-rw-rw-r--   0 zhsh      (1002) zhsh      (1002)     5993 2024-05-01 19:56:53.000000 pytorch_volumetric-0.5.2/tests/test_chamfer.py
+-rw-rw-r--   0 zhsh      (1002) zhsh      (1002)     9777 2024-05-01 19:56:53.000000 pytorch_volumetric-0.5.2/tests/test_model_to_sdf.py
+-rw-rw-r--   0 zhsh      (1002) zhsh      (1002)     4064 2024-05-01 19:56:53.000000 pytorch_volumetric-0.5.2/tests/test_sdf.py
+-rw-rw-r--   0 zhsh      (1002) zhsh      (1002)     1300 2024-05-01 19:56:53.000000 pytorch_volumetric-0.5.2/tests/test_voxel_sdf.py
```

### Comparing `pytorch_volumetric-0.5.0/LICENSE.txt` & `pytorch_volumetric-0.5.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pytorch_volumetric-0.5.0/PKG-INFO` & `pytorch_volumetric-0.5.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytorch_volumetric
-Version: 0.5.0
+Version: 0.5.2
 Summary: Volumetric structures such as voxels and SDFs implemented in pytorch
 Author-email: Sheng Zhong <zhsh@umich.edu>
 Maintainer-email: Sheng Zhong <zhsh@umich.edu>
 License: Copyright (c) 2023 University of Michigan ARM Lab
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of
         this software and associated documentation files (the "Software"), to deal in
@@ -73,14 +73,17 @@
 import pytorch_volumetric as pv
 
 # supposing we have an object mesh (most formats supported) - from https://github.com/eleramp/pybullet-object-models
 obj = pv.MeshObjectFactory("YcbPowerDrill/textured_simple_reoriented.obj")
 sdf = pv.MeshSDF(obj)
 ```
 
+An `open3d` mesh can be provided via the `mesh=` argument to `MeshObjectFactory`. When doing so, transform parameters
+such as scale are ignored.
+
 ### Cached SDF
 
 ```python
 import pytorch_volumetric as pv
 
 obj = pv.MeshObjectFactory("YcbPowerDrill/textured_simple_reoriented.obj")
 sdf = pv.MeshSDF(obj)
```

### Comparing `pytorch_volumetric-0.5.0/README.md` & `pytorch_volumetric-0.5.2/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -24,14 +24,17 @@
 import pytorch_volumetric as pv
 
 # supposing we have an object mesh (most formats supported) - from https://github.com/eleramp/pybullet-object-models
 obj = pv.MeshObjectFactory("YcbPowerDrill/textured_simple_reoriented.obj")
 sdf = pv.MeshSDF(obj)
 ```
 
+An `open3d` mesh can be provided via the `mesh=` argument to `MeshObjectFactory`. When doing so, transform parameters
+such as scale are ignored.
+
 ### Cached SDF
 
 ```python
 import pytorch_volumetric as pv
 
 obj = pv.MeshObjectFactory("YcbPowerDrill/textured_simple_reoriented.obj")
 sdf = pv.MeshSDF(obj)
```

### Comparing `pytorch_volumetric-0.5.0/pyproject.toml` & `pytorch_volumetric-0.5.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "pytorch_volumetric"
-version = "0.5.0"
+version = "0.5.2"
 description = "Volumetric structures such as voxels and SDFs implemented in pytorch"
 readme = "README.md" # Optional
 
 # Specify which Python versions you support. In contrast to the
 # 'Programming Language' classifiers above, 'pip install' will check this
 # and refuse to install the project if the version does not match. See
 # https://packaging.python.org/guides/distributing-packages-using-setuptools/#python-requires
```

### Comparing `pytorch_volumetric-0.5.0/src/pytorch_volumetric/__init__.py` & `pytorch_volumetric-0.5.2/src/pytorch_volumetric/__init__.py`

 * *Files identical despite different names*

### Comparing `pytorch_volumetric-0.5.0/src/pytorch_volumetric/chamfer.py` & `pytorch_volumetric-0.5.2/src/pytorch_volumetric/chamfer.py`

 * *Files identical despite different names*

### Comparing `pytorch_volumetric-0.5.0/src/pytorch_volumetric/model_to_sdf.py` & `pytorch_volumetric-0.5.2/src/pytorch_volumetric/model_to_sdf.py`

 * *Files identical despite different names*

### Comparing `pytorch_volumetric-0.5.0/src/pytorch_volumetric/sdf.py` & `pytorch_volumetric-0.5.2/src/pytorch_volumetric/sdf.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,29 +24,39 @@
     closest: torch.Tensor
     distance: torch.Tensor
     gradient: torch.Tensor
     normal: Union[torch.Tensor, None]
 
 
 class ObjectFactory(abc.ABC):
-    def __init__(self, name, scale=1.0, vis_frame_pos=(0, 0, 0), vis_frame_rot=(0, 0, 0, 1),
-                 plausible_suboptimality=0.001, **kwargs):
+    def __init__(self, name='', scale=1.0, vis_frame_pos=(0, 0, 0), vis_frame_rot=(0, 0, 0, 1),
+                 plausible_suboptimality=0.001, mesh=None, **kwargs):
+        """
+        :param name: path to the mesh obj if loading from file
+        :param scale: scaling factor for the mesh
+        :param vis_frame_pos: position of the mesh in the object frame
+        :param vis_frame_rot: quaternion rotation of the mesh in the object frame
+        :param plausible_suboptimality: how much error to tolerate in the SDF
+        :param mesh: open3d mesh object; can be provided instead of the path to the mesh; however,
+        giving this directly means scale, vis_frame_pos, and vis_frame_rot are ignored
+        """
         self.name = name
         self.scale = scale if scale is not None else 1.0
         # frame from model's base frame to the simulation's use of the model
         self.vis_frame_pos = vis_frame_pos
         self.vis_frame_rot = vis_frame_rot
         self.other_load_kwargs = kwargs
         self.plausible_suboptimality = plausible_suboptimality
 
         # use external mesh library to compute closest point for non-convex meshes
-        self._mesh = None
+        self._mesh = mesh
         self._mesht = None
         self._raycasting_scene = None
         self._face_normals = None
+        self.precompute_sdf()
 
     def __reduce__(self):
         return partial(self.__class__, scale=self.scale, vis_frame_pos=self.vis_frame_pos,
                        vis_frame_rot=self.vis_frame_rot,
                        plausible_suboptimality=self.plausible_suboptimality, **self.other_load_kwargs), \
             (self.name,)
 
@@ -63,18 +73,15 @@
         return self.get_mesh_resource_filename()
 
     def draw_mesh(self, dd, name, pose, rgba, object_id=None):
         frame_pos = np.array(self.vis_frame_pos) * self.scale
         return dd.draw_mesh(name, self.get_mesh_resource_filename(), pose, scale=self.scale, rgba=rgba,
                             object_id=object_id, vis_frame_pos=frame_pos, vis_frame_rot=self.vis_frame_rot)
 
-    def bounding_box(self, padding=0., padding_ratio=0.):
-        if self._mesh is None:
-            self.precompute_sdf()
-
+    def bounding_box(self, padding=0., padding_ratio=0):
         aabb = self._mesh.get_axis_aligned_bounding_box()
         world_min = aabb.get_min_bound()
         world_max = aabb.get_max_bound()
         # already scaled, but we add a little padding
         ranges = np.array(list(zip(world_min, world_max)))
         extents = ranges[:, 1] - ranges[:, 0]
         ranges[:, 0] -= padding + padding_ratio * extents
@@ -84,40 +91,40 @@
     def center(self):
         """Get center of mass assuming uniform density. Return is in object frame"""
         if self._mesh is None:
             self.precompute_sdf()
         return self._mesh.get_center()
 
     def precompute_sdf(self):
-        # scale mesh the approrpiate amount
-        full_path = self.get_mesh_high_poly_resource_filename()
-        full_path = os.path.expanduser(full_path)
-        if not os.path.exists(full_path):
-            raise RuntimeError(f"Expected mesh file does not exist: {full_path}")
-        self._mesh = o3d.io.read_triangle_mesh(full_path)
-        # scale mesh
-        scale_transform = np.eye(4)
-        np.fill_diagonal(scale_transform[:3, :3], self.scale)
-        self._mesh.transform(scale_transform)
-        # convert from mesh object frame to simulator object frame
-        x, y, z, w = self.vis_frame_rot
-        self._mesh = self._mesh.rotate(o3d.geometry.get_rotation_matrix_from_quaternion((w, x, y, z)),
-                                       center=[0, 0, 0])
-        self._mesh = self._mesh.translate(np.array(self.vis_frame_pos) * self.scale)
-
-        self._mesht = o3d.t.geometry.TriangleMesh.from_legacy(self._mesh)
-        self._raycasting_scene = o3d.t.geometry.RaycastingScene()
-        _ = self._raycasting_scene.add_triangles(self._mesht)
-        self._mesh.compute_triangle_normals()
-        self._face_normals = np.asarray(self._mesh.triangle_normals)
+        if self._mesh is None:
+            full_path = self.get_mesh_high_poly_resource_filename()
+            full_path = os.path.expanduser(full_path)
+            if not os.path.exists(full_path):
+                raise RuntimeError(f"Expected mesh file does not exist: {full_path}")
+            self._mesh = o3d.io.read_triangle_mesh(full_path)
+            # scale mesh
+            scale_transform = np.eye(4)
+            np.fill_diagonal(scale_transform[:3, :3], self.scale)
+            self._mesh.transform(scale_transform)
+            
+            # convert from mesh object frame to simulator object frame
+            x, y, z, w = self.vis_frame_rot
+            self._mesh = self._mesh.rotate(o3d.geometry.get_rotation_matrix_from_quaternion((w, x, y, z)),
+                                           center=[0, 0, 0])
+            self._mesh = self._mesh.translate(np.array(self.vis_frame_pos) * self.scale)
+
+        if self._mesht is None:
+            self._mesht = o3d.t.geometry.TriangleMesh.from_legacy(self._mesh)
+            self._raycasting_scene = o3d.t.geometry.RaycastingScene()
+            _ = self._raycasting_scene.add_triangles(self._mesht)
+            self._mesh.compute_triangle_normals()
+            self._face_normals = np.asarray(self._mesh.triangle_normals)
 
     @tensor_utils.handle_batch_input(n=2)
     def _do_object_frame_closest_point(self, points_in_object_frame, compute_normal=False):
-        if self._mesh is None:
-            self.precompute_sdf()
 
         if torch.is_tensor(points_in_object_frame):
             dtype = points_in_object_frame.dtype
             device = points_in_object_frame.device
             points_in_object_frame = points_in_object_frame.detach().cpu().numpy()
         else:
             dtype = torch.float
@@ -179,15 +186,15 @@
         (points from the query point to the closest point), and the surface normal at the closest point
         """
 
         return SDFQuery(*self._do_object_frame_closest_point(points_in_object_frame, compute_normal=compute_normal))
 
 
 class MeshObjectFactory(ObjectFactory):
-    def __init__(self, mesh_name, path_prefix='', **kwargs):
+    def __init__(self, mesh_name='', path_prefix='', **kwargs):
         self.path_prefix = path_prefix
         # whether to strip the package:// prefix from the mesh name, for example if we are loading a mesh manually
         # with a path prefix
         self.strip_package_prefix = path_prefix != ''
         # specify ranges=None to infer the range from the object's bounding box
         super(MeshObjectFactory, self).__init__(mesh_name, **kwargs)
 
@@ -609,14 +616,15 @@
     if obj_factory._mesh is None:
         obj_factory.precompute_sdf()
 
     mesh = obj_factory._mesh
 
     with rand.SavedRNG():
         rand.seed(seed)
+        o3d.utility.random.seed(seed)
 
         # because the point sampling is not dispersed, we do the dispersion ourselves
         # we accomplish this by sampling more points than we need then randomly selecting a subset
         sample_num_points = max(min_init_sample_points, 2 * num_points)
 
         # assume mesh is in object frame
         # pcd = mesh.sample_points_poisson_disk(number_of_points=num_points, init_factor=init_factor, seed=seed)
```

### Comparing `pytorch_volumetric-0.5.0/src/pytorch_volumetric/visualization.py` & `pytorch_volumetric-0.5.2/src/pytorch_volumetric/visualization.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,14 +64,15 @@
         # subsample arrows
         subsample_n = 5
         ax.quiver(x[::subsample_n],
                   z[::subsample_n],
                sdf_grad_uv[::subsample_n, ::subsample_n, shown_dims[0]],
                sdf_grad_uv[::subsample_n, ::subsample_n, shown_dims[1]], color='g')
     ax.clabel(cset2, cset2.levels, inline=True, fontsize=13, fmt=fmt)
+    plt.colorbar(cset1)
     # fig = plt.gcf()
     # fig.canvas.draw()
     plt.draw()
     plt.pause(0.005)
     return sdf_val, sdf_grad, pts, ax, cset1, cset2, v
```

### Comparing `pytorch_volumetric-0.5.0/src/pytorch_volumetric/voxel.py` & `pytorch_volumetric-0.5.2/src/pytorch_volumetric/voxel.py`

 * *Files 7% similar despite different names*

```diff
@@ -113,28 +113,36 @@
         self.positions = torch.cat((self.positions, pts.view(-1, self.positions.shape[-1])), dim=0)
         self.values = torch.cat((self.values, value))
 
     def get_known_pos_and_values(self):
         return self.positions, self.values
 
 
+def bounds_contain_another_bounds(outer_bounds: np.array, inner_bounds: np.array):
+    """Return whether outer_bounds contains inner_bounds"""
+    return np.all(outer_bounds[:, 0] <= inner_bounds[:, 0]) and np.all(outer_bounds[:, 1] >= inner_bounds[:, 1])
+
+
 def voxel_down_sample(points, resolution, range_per_dim=None, ignore_flat_dim=False):
     """
     Down sample point clouds to the center of a voxel grid with a given resolution.
     Much faster than open3d's voxel_down_sample but at the cost of more memory usage since they
     loop over points while we process all points in parallel.
     :param points: N x D point cloud
     :param resolution: Voxel size
     :param range_per_dim: Range of the voxel grid, if None, will be determined by the points (you may want to specify
     smaller range than the range the points to ignore outliers)
     :return:
     """
-    if range_per_dim is None:
-        range_per_dim = np.stack(
-            (points.min(dim=0)[0].cpu().numpy(), points.max(dim=0)[0].cpu().numpy())).T
+    if points.shape[0] == 0:
+        return points
+    data_bounds = np.stack((points.min(dim=0)[0].cpu().numpy() - resolution * 2,
+                            points.max(dim=0)[0].cpu().numpy() + resolution * 2)).T
+    if range_per_dim is None or bounds_contain_another_bounds(range_per_dim, data_bounds):
+        range_per_dim = data_bounds
 
     # special case for flat dimensions; assumes only last dimension can be flat
     flat_z = ignore_flat_dim and range_per_dim[-1][0] == range_per_dim[-1][1]
     flat_z_val = range_per_dim[-1][0]
     if flat_z:
         range_per_dim = range_per_dim[:-1]
         points = points[..., :-1]
```

### Comparing `pytorch_volumetric-0.5.0/src/pytorch_volumetric.egg-info/PKG-INFO` & `pytorch_volumetric-0.5.2/src/pytorch_volumetric.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytorch_volumetric
-Version: 0.5.0
+Version: 0.5.2
 Summary: Volumetric structures such as voxels and SDFs implemented in pytorch
 Author-email: Sheng Zhong <zhsh@umich.edu>
 Maintainer-email: Sheng Zhong <zhsh@umich.edu>
 License: Copyright (c) 2023 University of Michigan ARM Lab
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of
         this software and associated documentation files (the "Software"), to deal in
@@ -73,14 +73,17 @@
 import pytorch_volumetric as pv
 
 # supposing we have an object mesh (most formats supported) - from https://github.com/eleramp/pybullet-object-models
 obj = pv.MeshObjectFactory("YcbPowerDrill/textured_simple_reoriented.obj")
 sdf = pv.MeshSDF(obj)
 ```
 
+An `open3d` mesh can be provided via the `mesh=` argument to `MeshObjectFactory`. When doing so, transform parameters
+such as scale are ignored.
+
 ### Cached SDF
 
 ```python
 import pytorch_volumetric as pv
 
 obj = pv.MeshObjectFactory("YcbPowerDrill/textured_simple_reoriented.obj")
 sdf = pv.MeshSDF(obj)
```

### Comparing `pytorch_volumetric-0.5.0/src/pytorch_volumetric.egg-info/SOURCES.txt` & `pytorch_volumetric-0.5.2/src/pytorch_volumetric.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pytorch_volumetric-0.5.0/tests/test_chamfer.py` & `pytorch_volumetric-0.5.2/tests/test_chamfer.py`

 * *Files identical despite different names*

### Comparing `pytorch_volumetric-0.5.0/tests/test_model_to_sdf.py` & `pytorch_volumetric-0.5.2/tests/test_model_to_sdf.py`

 * *Files identical despite different names*

### Comparing `pytorch_volumetric-0.5.0/tests/test_sdf.py` & `pytorch_volumetric-0.5.2/tests/test_sdf.py`

 * *Files identical despite different names*

### Comparing `pytorch_volumetric-0.5.0/tests/test_voxel_sdf.py` & `pytorch_volumetric-0.5.2/tests/test_voxel_sdf.py`

 * *Files identical despite different names*

