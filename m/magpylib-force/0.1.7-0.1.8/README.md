# Comparing `tmp/magpylib_force-0.1.7.tar.gz` & `tmp/magpylib_force-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "magpylib_force-0.1.7.tar", last modified: Sun May  5 05:57:04 2024, max compression
+gzip compressed data, was "magpylib_force-0.1.8.tar", last modified: Tue May  7 09:25:54 2024, max compression
```

## Comparing `magpylib_force-0.1.7.tar` & `magpylib_force-0.1.8.tar`

### file list

```diff
@@ -1,24 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 05:57:04.515523 magpylib_force-0.1.7/
--rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-05-05 05:56:58.000000 magpylib_force-0.1.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1119 2024-05-05 05:57:04.515523 magpylib_force-0.1.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      555 2024-05-05 05:56:58.000000 magpylib_force-0.1.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 05:57:04.515523 magpylib_force-0.1.7/magpylib_force/
--rw-r--r--   0 runner    (1001) docker     (127)      213 2024-05-05 05:56:58.000000 magpylib_force-0.1.7/magpylib_force/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7923 2024-05-05 05:56:58.000000 magpylib_force-0.1.7/magpylib_force/force.py
--rw-r--r--   0 runner    (1001) docker     (127)     4887 2024-05-05 05:56:58.000000 magpylib_force-0.1.7/magpylib_force/meshing.py
--rw-r--r--   0 runner    (1001) docker     (127)     1769 2024-05-05 05:56:58.000000 magpylib_force-0.1.7/magpylib_force/utility.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 05:57:04.515523 magpylib_force-0.1.7/magpylib_force.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1119 2024-05-05 05:57:04.000000 magpylib_force-0.1.7/magpylib_force.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      453 2024-05-05 05:57:04.000000 magpylib_force-0.1.7/magpylib_force.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-05 05:57:04.000000 magpylib_force-0.1.7/magpylib_force.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-05 05:57:04.000000 magpylib_force-0.1.7/magpylib_force.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-05 05:57:04.000000 magpylib_force-0.1.7/magpylib_force.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-05 05:57:04.515523 magpylib_force-0.1.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1217 2024-05-05 05:56:58.000000 magpylib_force-0.1.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 05:57:04.515523 magpylib_force-0.1.7/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 05:56:58.000000 magpylib_force-0.1.7/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13390 2024-05-05 05:56:58.000000 magpylib_force-0.1.7/tests/test_FEM.py
--rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-05-05 05:56:58.000000 magpylib_force-0.1.7/tests/test_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)      597 2024-05-05 05:56:58.000000 magpylib_force-0.1.7/tests/test_meshing.py
--rw-r--r--   0 runner    (1001) docker     (127)     6355 2024-05-05 05:56:58.000000 magpylib_force-0.1.7/tests/test_physics.py
--rw-r--r--   0 runner    (1001) docker     (127)     5520 2024-05-05 05:56:58.000000 magpylib_force-0.1.7/tests/test_self_consistency.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 09:25:54.537328 magpylib_force-0.1.8/
+-rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-05-07 09:25:47.000000 magpylib_force-0.1.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2140 2024-05-07 09:25:54.537328 magpylib_force-0.1.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1576 2024-05-07 09:25:47.000000 magpylib_force-0.1.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 09:25:54.537328 magpylib_force-0.1.8/magpylib_force/
+-rw-r--r--   0 runner    (1001) docker     (127)      213 2024-05-07 09:25:47.000000 magpylib_force-0.1.8/magpylib_force/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12050 2024-05-07 09:25:47.000000 magpylib_force-0.1.8/magpylib_force/force.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5622 2024-05-07 09:25:47.000000 magpylib_force-0.1.8/magpylib_force/meshing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1842 2024-05-07 09:25:47.000000 magpylib_force-0.1.8/magpylib_force/utility.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 09:25:54.537328 magpylib_force-0.1.8/magpylib_force.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2140 2024-05-07 09:25:54.000000 magpylib_force-0.1.8/magpylib_force.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      474 2024-05-07 09:25:54.000000 magpylib_force-0.1.8/magpylib_force.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 09:25:54.000000 magpylib_force-0.1.8/magpylib_force.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-07 09:25:54.000000 magpylib_force-0.1.8/magpylib_force.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-07 09:25:54.000000 magpylib_force-0.1.8/magpylib_force.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 09:25:54.537328 magpylib_force-0.1.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1217 2024-05-07 09:25:47.000000 magpylib_force-0.1.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 09:25:54.537328 magpylib_force-0.1.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 09:25:47.000000 magpylib_force-0.1.8/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13382 2024-05-07 09:25:47.000000 magpylib_force-0.1.8/tests/test_FEM.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1349 2024-05-07 09:25:47.000000 magpylib_force-0.1.8/tests/test_basics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1014 2024-05-07 09:25:47.000000 magpylib_force-0.1.8/tests/test_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)      597 2024-05-07 09:25:47.000000 magpylib_force-0.1.8/tests/test_meshing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7126 2024-05-07 09:25:47.000000 magpylib_force-0.1.8/tests/test_physics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5520 2024-05-07 09:25:47.000000 magpylib_force-0.1.8/tests/test_self_consistency.py
```

### Comparing `magpylib_force-0.1.7/LICENSE` & `magpylib_force-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `magpylib_force-0.1.7/magpylib_force/force.py` & `magpylib_force-0.1.8/magpylib_force/force.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 import numpy as np
 import magpylib as magpy
+from magpylib_force.meshing import mesh_target
 from magpylib_force.meshing import mesh_cuboid
 from magpylib_force.utility import check_input_anchor
 from magpylib_force.utility import check_input_targets
 from magpylib._src.obj_classes.class_current_Polyline import Polyline
 from magpylib._src.obj_classes.class_magnet_Cuboid import Cuboid
+from magpylib._src.obj_classes.class_magnet_Sphere import Sphere
 
 
 def getFT(sources, targets, anchor=None, eps=1e-5, squeeze=True):
     """
     Compute force and torque between sources and targets.
     SI units are assumed for all inputs and outputs.
 
@@ -17,123 +19,156 @@
     sources: source and collection objects or 1D list thereof
         Sources that generate the magnetic field. Can be a single source (or collection)
         or a 1D list of l sources and/or collection objects.
 
     targets: single object or 1D list of t objects that are in [Cuboid, Polyline]
         Force and Torque acting on targets in the magnetic field generated by the sources
         will be computed. A target must have a valid `meshing` parameter.
-    
-    eps: float, default=1e-5
-        For magnet-targets the magnetic field gradient is computed using finite
-        differences (FD). `eps` is the FD step size. A good value
-        is 1e-5 * characteristic system size (magnet size, distance between sources
-        and targets, ...).
 
     anchor: array_like, default=None
         The Force adds to the Torque via the anchor point. For a freely floating magnet
         this would be the barycenter. If `anchor=None`, this part of the Torque computation
         is ommitted.
 
+    eps: float, default=1e-5
+        This is only used for magnet targets for computing the magnetic field gradient
+        using finite differences (FD). `eps` is the FD step size. A good value
+        is 1e-5 * characteristic_system_size (magnet size, distance between sources
+        and targets, ...).
+
     squeeze: bool, default=True
         The output of the computation has the shape (n,3) where n corresponds to the number
         of targets. By default this is reduced to (3,) when there is only one target.
 
     Returns
     -------
-    Force-Torque as ndarray of shape (2,3), of (t,2,3) when t targets are given
+    Force-Torque as ndarray of shape (2,3), or (t,2,3) when t targets are given
     """
     anchor = check_input_anchor(anchor)
     targets = check_input_targets(targets)
-    # MISSING: allow Collections
+    # MISSING: allow Collections as targets
 
     n = len(targets)
 
-    cuboids, order_cub = [], []
-    polylines, order_poly = [], []
-    for i,t in enumerate(targets):
-        if isinstance(t, Cuboid):
-            cuboids.append(t)
-            order_cub.append(i)
-        elif isinstance(t, Polyline):
-            polylines.append(t)
-            order_poly.append(i)
+    # split targets into lists of similar types
+    TARGET_TYPES = [Cuboid, Polyline, Sphere]
+    getFT_FUNCS = [getFTmagnet, getFTcurrent, getFTmagnet]
+    objects = [[] for _ in TARGET_TYPES]
+    orders  = [[] for _ in TARGET_TYPES]
+
+    for i,tgt in enumerate(targets):
+        for j,ttyp in enumerate(TARGET_TYPES):
+            if isinstance(tgt, ttyp):
+                objects[j].append(tgt)
+                orders[j].append(i)
 
+    # allocate FT
     FT = np.zeros((n, 2, 3))
-    if cuboids:
-        FT_cube = getFTcube(sources, cuboids, eps=eps, anchor=anchor, squeeze=False)
-        FT_cube = np.swapaxes(FT_cube, 0, 1)
-        for ft,o in zip(FT_cube, order_cub):
-            FT[o] = ft
-    if polylines:
-        FT_poly = getFTwire(sources, polylines, anchor=anchor, squeeze=False)
-        FT_poly = np.swapaxes(FT_poly, 0, 1)
-        for ft,o in zip(FT_poly, order_poly):
-            FT[o] = ft
-    #FT = np.swapaxes(FT, 0, 1)
+
+    # FT-computation and broadcasting
+    for i in range(len(TARGET_TYPES)):
+        if objects[i]:
+            ft_part = getFT_FUNCS[i](sources, objects[i], eps=eps, anchor=anchor)
+            ft_part = np.swapaxes(ft_part, 0, 1)
+            for ft,j in zip(ft_part, orders[i]):
+                FT[j] = ft
+
     if squeeze:
         return np.squeeze(FT)
     return FT
 
 
-def getFTcube(sources, targets, eps=1e-5, anchor=None, squeeze=True):
+def mesh_instances(targets):
+    """
+    utility for getFTmagnet: compute number of mesh instances for each target magnet
+    targets: list of target magnet objects
+    returns: int
+    """
+    if isinstance(targets[0], Cuboid):
+        return np.array([np.prod(tgt.meshing) for tgt in targets])
+    elif isinstance(targets[0], Sphere):
+        SPH_MESH = (0,1,8,19,32,81,136,179,280,389,552,739,912,1189,1472,1791,2176,2553,3112,3695,4224)
+        return np.array([SPH_MESH[tgt.meshing] for tgt in targets])
+    raise RuntimeError("fktn `mesh_instances` - I shouldt be here.")
+
+
+def volume(target):
     """
-    Compute force and torque acting on a Cuboid magnet.
+    utility for getFTmagnet: compute physical volume of target magnets
+    target: target magnet object
+    return: volume, float
+    """
+    if isinstance(target, Cuboid):
+        return np.prod(target.dimension)
+    elif isinstance(target, Sphere):
+        return target.diameter**3 * np.pi / 6
+    raise RuntimeError("fktn `volume` - I shouldt be here.")
+
+
+def getFTmagnet(sources, targets, eps=1e-5, anchor=None):
+    """
+    Compute force and torque acting on magnets of same type
 
     Parameters
     ----------
     sources: source and collection objects or 1D list thereof
         Sources that generate the magnetic field. Can be a single source (or collection)
         or a 1D list of l sources and/or collection objects.
 
     targets: Cuboid object or 1D list of Cuboid objects
         Force and Torque acting on targets in the magnetic field generated by the sources
         will be computed. A target must have a valid `meshing` parameter.
-    
+
     eps: float, default=1e-5
         The magnetic field gradient is computed using finite differences (FD). eps is
         the FD step size. A good value is 1e-5 * characteristic system size (magnet size,
         distance between sources and targets, ...).
-    
+
     anchor: array_like, default=None
         The Force adds to the Torque via the anchor point. For a freely floating magnet
         this would be the barycenter. If `anchor=None`, this part of the Torque computation
         is ommitted.
-
-    squeeze: bool, default=True
-        The output of the computation has the shape (n,3) where n corresponds to the number
-        of targets. By default this is reduced to (3,) when there is only one target.
     """
-
-    # number of Cuboids
+    # number of magnets
     tgt_number = len(targets)
 
-    # number of instances of each Cuboid
-    inst_numbers = np.array([np.prod(tgt.meshing) for tgt in targets])
+    # number of instances of each magnet
+    inst_numbers = mesh_instances(targets)
 
     # total number of instances
     no_inst = np.sum(inst_numbers)
 
     # cumsum of number of instances (used for indexing)
     insti = np.r_[0, np.cumsum(inst_numbers)]
 
     # field computation positions (1xfor B, 6x for gradB)
     POSS = np.zeros((no_inst,7,3))
 
     # moment of each instance
     MOM = np.zeros((no_inst,3))
 
-    # MISSING: eps should be defined relative to the sizes of the system
+    # MISSING: eps should be defined relative to the sizes of the objects
     eps_vec = np.array([(0,0,0), (eps,0,0), (-eps,0,0), (0,eps,0), (0,-eps,0), (0,0,eps), (0,0,-eps)])
 
     for i,tgt in enumerate(targets):
-        tgt_vol = np.prod(tgt.dimension)
-        inst_mom = tgt.magnetization * tgt_vol / inst_numbers[i]
+        tgt_vol = volume(tgt)
+        inst_mom = tgt.orientation.apply(tgt.magnetization) * tgt_vol / inst_numbers[i]
         MOM[insti[i]:insti[i+1]] = inst_mom
 
-        mesh = mesh_cuboid(tgt)
+        mesh = mesh_target(tgt)
+        #import matplotlib.pyplot as plt
+        #ax = plt.figure().add_subplot(projection='3d')
+        #ax.plot(mesh[:,0], mesh[:,1], mesh[:,2], ls='', marker='.')
+
+        mesh = tgt.orientation.apply(mesh)
+        #ax.plot(mesh[:,0], mesh[:,1], mesh[:,2], ls='', marker='.', color='r')
+        #plt.show()
+        #import sys
+        #sys.exit()
+
         for j,ev in enumerate(eps_vec):
             POSS[insti[i]:insti[i+1],j] = mesh + ev + tgt.position
 
     BB = magpy.getB(sources, POSS, sumup=True)
     gradB = (BB[:,1::2]-BB[:,2::2]) / (2*eps)
     gradB = np.swapaxes(gradB,0,1)
 
@@ -142,25 +177,102 @@
     Ts = np.cross(BB[:,0], MOM)
     if anchor is not None:
         Ts -= np.cross(POSS[:,0]-anchor, Fs)
 
     T = np.array([np.sum(Ts[insti[i]:insti[i+1]],axis=0) for i in range(tgt_number)])
     F = np.array([np.sum(Fs[insti[i]:insti[i+1]],axis=0) for i in range(tgt_number)])
 
-    if squeeze:
-        F = np.squeeze(F)
-        T = np.squeeze(T)
-
     return np.array((F, T))
 
 
 
-def getFTwire(sources, targets, anchor=None, squeeze=True):
+# def getFTcube(sources, targets, eps=1e-5, anchor=None, squeeze=True):
+#     """
+#     Compute force and torque acting on a Cuboid magnet.
+
+#     Parameters
+#     ----------
+#     sources: source and collection objects or 1D list thereof
+#         Sources that generate the magnetic field. Can be a single source (or collection)
+#         or a 1D list of l sources and/or collection objects.
+
+#     targets: Cuboid object or 1D list of Cuboid objects
+#         Force and Torque acting on targets in the magnetic field generated by the sources
+#         will be computed. A target must have a valid `meshing` parameter.
+
+#     eps: float, default=1e-5
+#         The magnetic field gradient is computed using finite differences (FD). eps is
+#         the FD step size. A good value is 1e-5 * characteristic system size (magnet size,
+#         distance between sources and targets, ...).
+
+#     anchor: array_like, default=None
+#         The Force adds to the Torque via the anchor point. For a freely floating magnet
+#         this would be the barycenter. If `anchor=None`, this part of the Torque computation
+#         is ommitted.
+
+#     squeeze: bool, default=True
+#         The output of the computation has the shape (n,3) where n corresponds to the number
+#         of targets. By default this is reduced to (3,) when there is only one target.
+#     """
+
+#     # number of Cuboids
+#     tgt_number = len(targets)
+
+#     # number of instances of each Cuboid
+#     inst_numbers = np.array([np.prod(tgt.meshing) for tgt in targets])
+
+#     # total number of instances
+#     no_inst = np.sum(inst_numbers)
+
+#     # cumsum of number of instances (used for indexing)
+#     insti = np.r_[0, np.cumsum(inst_numbers)]
+
+#     # field computation positions (1xfor B, 6x for gradB)
+#     POSS = np.zeros((no_inst,7,3))
+
+#     # moment of each instance
+#     MOM = np.zeros((no_inst,3))
+
+#     # MISSING: eps should be defined relative to the sizes of the system
+#     eps_vec = np.array([(0,0,0), (eps,0,0), (-eps,0,0), (0,eps,0), (0,-eps,0), (0,0,eps), (0,0,-eps)])
+
+#     for i,tgt in enumerate(targets):
+#         tgt_vol = np.prod(tgt.dimension)
+#         inst_mom = tgt.magnetization * tgt_vol / inst_numbers[i]
+#         MOM[insti[i]:insti[i+1]] = inst_mom
+
+#         mesh = mesh_cuboid(tgt)
+#         for j,ev in enumerate(eps_vec):
+#             POSS[insti[i]:insti[i+1],j] = mesh + ev + tgt.position
+
+#     BB = magpy.getB(sources, POSS, sumup=True)
+#     gradB = (BB[:,1::2]-BB[:,2::2]) / (2*eps)
+#     gradB = np.swapaxes(gradB,0,1)
+
+#     Fs = np.sum((gradB*MOM),axis=2).T
+#     #Ts = np.zeros((no_inst,3))
+#     Ts = np.cross(BB[:,0], MOM)
+#     if anchor is not None:
+#         Ts -= np.cross(POSS[:,0]-anchor, Fs)
+
+#     T = np.array([np.sum(Ts[insti[i]:insti[i+1]],axis=0) for i in range(tgt_number)])
+#     F = np.array([np.sum(Fs[insti[i]:insti[i+1]],axis=0) for i in range(tgt_number)])
+
+#     if squeeze:
+#         F = np.squeeze(F)
+#         T = np.squeeze(T)
+
+#     return np.array((F, T))
+
+
+
+def getFTcurrent(sources, targets, anchor=None, eps=None):
     """
     compute force acting on tgt Polyline
+    eps is a dummy variable that is not used
 
     info:
     targets = Polyline objects
     segements = linear segments within Polyline objects
     instances = computation instances, each segment is split into `meshing` points
     """
 
@@ -186,22 +298,22 @@
     LVEC = np.zeros((no_inst,3))
     # central location of each instance
     POSS = np.zeros((no_inst,3))
     # current of each instance
     CURR = np.zeros((no_inst,))
 
     for i,tgt in enumerate(targets):
-        verts = tgt.vertices
+        verts = tgt.orientation.apply(tgt.vertices)
         mesh = mesh_numbers[i]
 
         lvec = np.repeat(verts[1:] - verts[:-1], mesh, axis=0)/mesh
         LVEC[insti[i]:insti[i+1]] = lvec
 
         CURR[insti[i]:insti[i+1]] = [tgt.current]*mesh*seg_numbers[i]
-        
+
         for j in range(seg_numbers[i]):
             poss = np.linspace(verts[j]+lvec[j*mesh]/2, verts[j+1]-lvec[j*mesh]/2, mesh) + tgt.position
             POSS[insti[i]+mesh*j:insti[i]+mesh*(j+1)] = poss
 
     # field of every instance
     B = magpy.getB(sources, POSS, sumup=True)
 
@@ -214,13 +326,8 @@
         T = np.array([np.sum(T[insti[i]:insti[i+1]],axis=0) for i in range(tgt_number)])
     else:
         T = np.zeros((tgt_number,3))
 
     # sumup force for every target
     F = np.array([np.sum(F[insti[i]:insti[i+1]],axis=0) for i in range(tgt_number)])
 
-    # squeeze output
-    if squeeze:
-        F = np.squeeze(F)
-        T = np.squeeze(T)
-
     return np.array((F, T))
```

### Comparing `magpylib_force-0.1.7/magpylib_force/meshing.py` & `magpylib_force-0.1.8/magpylib_force/meshing.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,37 @@
 import numpy as np
 import itertools
 import math as m
 import pint
+from magpylib._src.obj_classes.class_magnet_Cuboid import Cuboid
+from magpylib._src.obj_classes.class_magnet_Sphere import Sphere
+
+def mesh_target(object):
+    """
+    create mesh for target objects
+    """
+    if isinstance(object, Cuboid):
+        return mesh_cuboid(object)
+    elif isinstance(object, Sphere):
+        return mesh_sphere(object)
+    raise RuntimeError("fktn `mesh_target`: should not be here!")
+
+
+def mesh_sphere(object):
+    """
+    create sphere mesh from object meshing parameter
+    """
+    n = object.meshing
+    dia = object.diameter
+    a = -dia/2+dia/(2*n)
+    b =  dia/2-dia/(2*n)
+    c = n*1j
+    mesh = np.mgrid[a:b:c, a:b:c, a:b:c].T.reshape(n**3,3)
+    return mesh[np.linalg.norm(mesh, axis=1)<dia/2]
+
 
 def mesh_cuboid(object):
     """
     splits cuboid into given mesh
     returns grid positions relative to cuboid position
     """
     a,b,c = object.dimension
```

### Comparing `magpylib_force-0.1.7/magpylib_force/utility.py` & `magpylib_force-0.1.8/magpylib_force/utility.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import numpy as np
 from magpylib._src.obj_classes.class_magnet_Cuboid import Cuboid
 from magpylib._src.obj_classes.class_current_Polyline import Polyline
-
+from magpylib._src.obj_classes.class_magnet_Sphere import Sphere
 
 def check_input_anchor(anchor):
     """
     check and format anchor input
     """
     if anchor is None:
         return None
@@ -19,15 +19,15 @@
 
 
 def check_input_targets(targets):
     """ check and format targets input """
     if not isinstance(targets, list):
         targets = [targets]
     for t in targets:
-        if not isinstance(t, (Cuboid, Polyline)):
+        if not isinstance(t, (Cuboid, Polyline, Sphere)):
             raise ValueError(
                 "Bad `targets` input for getFT."
                 " `targets` can only be Cuboids and Polylines."
                 f" Instead receivd type {type(t)} target."
             )
         if not hasattr(t, "meshing"):
             raise ValueError(
@@ -47,8 +47,8 @@
 
 # def check_input_targets_Polyline(targets):
 #     """ check and format targets input """
 #     if isinstance(targets, Polyline):
 #         targets = [targets]
 #     if not isinstance(targets, list):
 #         raise ValueError("Bad targets input.")
-#     return targets
+#     return targets
```

### Comparing `magpylib_force-0.1.7/setup.py` & `magpylib_force-0.1.8/setup.py`

 * *Files identical despite different names*

### Comparing `magpylib_force-0.1.7/tests/test_FEM.py` & `magpylib_force-0.1.8/tests/test_FEM.py`

 * *Files 0% similar despite different names*

```diff
@@ -218,15 +218,15 @@
         i0 = d[0]*1e-3 #ampere
         pos = np.array((d[3]*1e-3, d[1], d[2]))*1e-3
         f2 = np.array((d[4], d[5], d[6]))*1e-6
         f1 = np.array((d[7], d[8], d[9]))*1e-6
 
         t1 = np.array((t[4], t[5], t[6]))*1e-9
         t2 = np.array((t[7], t[8], t[9]))*1e-9
-        
+
         for wire in wires:
             wire.current = i0
         magnet.position = pos + np.array((0,0,.15))*1e-3
 
         F1,_ = getFT(wires, magnet, anchor=(0,0,0))
         F2,T2 = np.sum(getFT(magnet, wires, anchor=(0,0,0)), axis=0)
```

### Comparing `magpylib_force-0.1.7/tests/test_interface.py` & `magpylib_force-0.1.8/tests/test_interface.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,18 +18,18 @@
     wire1.meshing=20
     wire2.meshing=20
     wire3.meshing=20
 
     FT1 = getFT(src1, wire1, anchor=(0,0,0))
     FT2 = getFT(src1, [wire1], anchor=(0,0,0))
     FT3 = getFT(src1, [wire1,wire2,wire3], anchor=(0,0,0))
-    
+
     np.testing.assert_allclose(FT1,FT2)
     np.testing.assert_allclose(FT1,FT3[0])
     np.testing.assert_allclose(FT1,FT3[1])
     np.testing.assert_allclose(FT1,FT3[2])
 
     FT4 = getFT(src1, wire1, anchor=(0,0,0))
     FT5 = getFT([src1, src2], wire1, anchor=(0,0,0))
-    
+
+    np.testing.assert_allclose(FT4*2,FT5)
     np.testing.assert_allclose(FT4*2,FT5)
-    np.testing.assert_allclose(FT4*2,FT5)
```

### Comparing `magpylib_force-0.1.7/tests/test_meshing.py` & `magpylib_force-0.1.8/tests/test_meshing.py`

 * *Files identical despite different names*

### Comparing `magpylib_force-0.1.7/tests/test_physics.py` & `magpylib_force-0.1.8/tests/test_physics.py`

 * *Files 7% similar despite different names*

```diff
@@ -225,7 +225,40 @@
         currs.append(loop)
 
     F1,T1 = getFT(gen, cube, anchor=np.array((0,0,0)))
     F2,T2 = np.sum(getFT(gen, currs, anchor=np.array((0,0,0))), axis=0)
 
     assert np.amax(abs((F1-F2)/(F1+F2)*2))<1e-2
     assert np.amax(abs((T1-T2)/(T1+T2)*2))<1e-2
+
+
+def test_sphere_cube_at_distance():
+    """
+    A sphere and a cuboid with similar volume should see a similar torque and force
+    at a distance
+    """
+    source = magpy.magnet.Sphere(diameter=1, polarization=(1,2,3))
+
+    J = (3,2,1)
+    pos = (5,-7,11)
+
+    cube = magpy.magnet.Cuboid(
+        dimension=(1,1,1),
+        polarization=J,
+        position=pos
+    )
+    cube.meshing = (2,2,2)
+
+    sphere = magpy.magnet.Sphere(
+        diameter=(6/np.pi)**(1/3),
+        polarization=J,
+        position=pos,
+    )
+    sphere.meshing=2
+
+    FT = getFT(source, [cube, sphere], anchor=(0,0,0))
+
+    errF = (FT[0,0]-FT[1,0])/np.linalg.norm(FT[0,0])
+    errT = (FT[0,1]-FT[1,1])/np.linalg.norm(FT[0,1])
+
+    assert max(abs(errF)) < 1e-5
+    assert max(abs(errT)) < 1e-5
```

### Comparing `magpylib_force-0.1.7/tests/test_self_consistency.py` & `magpylib_force-0.1.8/tests/test_self_consistency.py`

 * *Files identical despite different names*

