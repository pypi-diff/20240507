# Comparing `tmp/zelas-1.3.240505.tar.gz` & `tmp/zelas-1.3.240507.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zelas-1.3.240505.tar", last modified: Sun May  5 11:15:09 2024, max compression
+gzip compressed data, was "zelas-1.3.240507.tar", last modified: Tue May  7 10:03:57 2024, max compression
```

## Comparing `zelas-1.3.240505.tar` & `zelas-1.3.240507.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxrwxrwx   0        0        0        0 2024-05-05 11:15:09.413273 zelas-1.3.240505/
--rw-rw-rw-   0        0        0      644 2024-05-05 11:15:09.412291 zelas-1.3.240505/PKG-INFO
--rw-rw-rw-   0        0        0       42 2024-05-05 11:15:09.413690 zelas-1.3.240505/setup.cfg
--rw-rw-rw-   0        0        0     1141 2024-05-05 10:30:49.000000 zelas-1.3.240505/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-05 11:15:09.407189 zelas-1.3.240505/zelas/
--rw-rw-rw-   0        0        0    18970 2024-05-04 23:23:16.000000 zelas-1.3.240505/zelas/Ellipse.py
--rw-rw-rw-   0        0        0    17674 2024-05-04 12:33:33.000000 zelas-1.3.240505/zelas/Multispectral.py
--rw-rw-rw-   0        0        0    40295 2024-05-04 23:59:49.000000 zelas-1.3.240505/zelas/RedundancyElimination.py
--rw-rw-rw-   0        0        0     7796 2024-05-04 12:33:33.000000 zelas-1.3.240505/zelas/TheHeartOfTheMilitaryGod.py
--rw-rw-rw-   0        0        0      189 2024-05-05 10:27:30.000000 zelas-1.3.240505/zelas/__init__.py
--rw-rw-rw-   0        0        0     9366 2024-05-04 12:41:19.000000 zelas-1.3.240505/zelas/ransac.py
--rw-rw-rw-   0        0        0    90380 2024-05-04 23:23:31.000000 zelas-1.3.240505/zelas/shield.py
--rw-rw-rw-   0        0        0    77960 2024-05-05 09:18:08.000000 zelas-1.3.240505/zelas/voxel.py
-drwxrwxrwx   0        0        0        0 2024-05-05 11:15:09.411732 zelas-1.3.240505/zelas.egg-info/
--rw-rw-rw-   0        0        0      644 2024-05-05 11:15:09.000000 zelas-1.3.240505/zelas.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      294 2024-05-05 11:15:09.000000 zelas-1.3.240505/zelas.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-05 11:15:09.000000 zelas-1.3.240505/zelas.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2024-05-05 11:15:09.000000 zelas-1.3.240505/zelas.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-07 10:03:57.570114 zelas-1.3.240507/
+-rw-rw-rw-   0        0        0      646 2024-05-07 10:03:57.570114 zelas-1.3.240507/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2024-05-07 10:03:57.570114 zelas-1.3.240507/setup.cfg
+-rw-rw-rw-   0        0        0     1143 2024-05-07 10:02:32.000000 zelas-1.3.240507/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-07 10:03:57.557118 zelas-1.3.240507/zelas/
+-r--r--r--   0        0        0    18970 2024-05-04 23:23:16.000000 zelas-1.3.240507/zelas/Ellipse.py
+-r--r--r--   0        0        0    17674 2024-05-04 12:33:33.000000 zelas-1.3.240507/zelas/Multispectral.py
+-r--r--r--   0        0        0    40295 2024-05-04 23:59:49.000000 zelas-1.3.240507/zelas/RedundancyElimination.py
+-rw-rw-rw-   0        0        0     8775 2024-05-07 07:19:56.000000 zelas-1.3.240507/zelas/TheHeartOfTheMilitaryGod.py
+-rw-rw-rw-   0        0        0      189 2024-05-05 10:27:30.000000 zelas-1.3.240507/zelas/__init__.py
+-r--r--r--   0        0        0     9366 2024-05-04 12:41:19.000000 zelas-1.3.240507/zelas/ransac.py
+-rw-rw-rw-   0        0        0     1141 2024-05-05 10:16:09.000000 zelas-1.3.240507/zelas/setup.py
+-rw-rw-rw-   0        0        0    90398 2024-05-07 06:47:15.000000 zelas-1.3.240507/zelas/shield.py
+-rw-rw-rw-   0        0        0    82564 2024-05-07 07:41:56.000000 zelas-1.3.240507/zelas/voxel.py
+drwxrwxrwx   0        0        0        0 2024-05-07 10:03:57.569080 zelas-1.3.240507/zelas.egg-info/
+-rw-rw-rw-   0        0        0      646 2024-05-07 10:03:57.000000 zelas-1.3.240507/zelas.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      309 2024-05-07 10:03:57.000000 zelas-1.3.240507/zelas.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-07 10:03:57.000000 zelas-1.3.240507/zelas.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2024-05-07 10:03:57.000000 zelas-1.3.240507/zelas.egg-info/top_level.txt
```

### Comparing `zelas-1.3.240505/PKG-INFO` & `zelas-1.3.240507/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: zelas
-Version: 1.3.240505
+Version: 1.3.240507
 Summary: Professor Liying Wang official point clouds database 
 Home-page: UNKNOWN
 Author: Zelas You
 Author-email: youze1997@163.com
 License: UNKNOWN
 Description: Produced by CCG.Lidar Point Cloud Research Institute
 Keywords: python,las
 Platform: UNKNOWN
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
-Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
```

### Comparing `zelas-1.3.240505/setup.py` & `zelas-1.3.240507/zelas/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 setup(
     name="zelas",
     version=VERSION,
     author="Zelas You",
     author_email="youze1997@163.com",
     description=DESCRIPTION,
     long_description_content_type="text/markdown",
-    long_description=LONG_DESCRIPTION,
+    long_description=long_description,
     packages=find_packages(),
     install_requires=[],
     keywords=['python', 'las'],
     classifiers=[
         "Development Status :: 1 - Planning",
         "Intended Audience :: Developers",
         "Programming Language :: Python :: 3",
```

### Comparing `zelas-1.3.240505/zelas/Ellipse.py` & `zelas-1.3.240507/zelas/Ellipse.py`

 * *Files identical despite different names*

### Comparing `zelas-1.3.240505/zelas/Multispectral.py` & `zelas-1.3.240507/zelas/Multispectral.py`

 * *Files identical despite different names*

### Comparing `zelas-1.3.240505/zelas/RedundancyElimination.py` & `zelas-1.3.240507/zelas/RedundancyElimination.py`

 * *Files identical despite different names*

### Comparing `zelas-1.3.240505/zelas/TheHeartOfTheMilitaryGod.py` & `zelas-1.3.240507/zelas/TheHeartOfTheMilitaryGod.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,53 +1,68 @@
 from __future__ import division
 # 这是一个关于私人用途的代码原文件库
 import numpy as np
 from numpy import *
 import sys  # maxint
+import matplotlib.pyplot as plt
+import pyvista as pv
+import matplotlib.cm as cm
+
 
 # C-均值聚类
-def FCM_train(X,n_centers,m,max_iter = 100,theta=1e-5,seed=0):
+def FCM_train(X, n_centers, m, max_iter=100, theta=1e-5, seed=0):
     rng = np.random.RandomState(seed)
-    N,D = np.shape(X)
+    N, D = np.shape(X)
     # 随机初始化关系矩阵
     U = rng.uniform(size=(N, n_centers))
     # 保证每行和为1
-    U = U/np.sum(U,axis=1,keepdims=True)
+    U = U / np.sum(U, axis=1, keepdims=True)
     # 开始迭代
     for i in range(max_iter):
         print(i)
         U_old = U.copy()
-        centers = FCM_getCenters(U,X,m)
-        U=FCM_getU(X,centers,m)
+        centers = FCM_getCenters(U, X, m)
+        U = FCM_getU(X, centers, m)
         # 两次关系的距离矩阵过小，结束训练
-        if np.linalg.norm(U-U_old) < theta:
+        if np.linalg.norm(U - U_old) < theta:
             break
-    return centers,U
+    return centers, U
+
 
-def FCM_getCenters(U,X,m):
-    N,D = np.shape(X)
-    N,C = np.shape(U)
-    um = U** m
-    tile_X = np.tile(np.expand_dims(X,1),[1,C,1])
-    tile_um = np.tile(np.expand_dims(um,1),[1,1,D])
-    temp = tile_X*tile_um
-    new_C = np.sum(temp,axis=0)/np.expand_dims(np.sum(um,axis=0),axis=-1)
+def FCM_getCenters(U, X, m):
+    N, D = np.shape(X)
+    N, C = np.shape(U)
+    um = U ** m
+    tile_X = np.tile(np.expand_dims(X, 1), [1, C, 1])
+    tile_um = np.tile(np.expand_dims(um, 1), [1, 1, D])
+    temp = tile_X * tile_um
+    new_C = np.sum(temp, axis=0) / np.expand_dims(np.sum(um, axis=0), axis=-1)
     return new_C
 
-def FCM_getU(X,Centers,m):
-    N,D =np.shape(X)
-    C,D = np.shape(Centers)
-    temp = FCM_dist(X,Centers)**float(2/(m-1))
-    tile_temp = np.tile(np.expand_dims(temp,1),[1,C,1])
-    denominator_ = np.expand_dims(temp,-1)/tile_temp
-    return 1/np.sum(denominator_,axis=-1)
+
+def FCM_getU(X, Centers, m):
+    N, D = np.shape(X)
+    C, D = np.shape(Centers)
+    temp = FCM_dist(X, Centers) ** float(2 / (m - 1))
+    tile_temp = np.tile(np.expand_dims(temp, 1), [1, C, 1])
+    denominator_ = np.expand_dims(temp, -1) / tile_temp
+    return 1 / np.sum(denominator_, axis=-1)
+
+def FCM_dist(X, Centers):
+    N, D = np.shape(X)
+    C, D = np.shape(Centers)
+    tile_x = np.tile(np.expand_dims(X, 1), [1, C, 1])
+    tile_centers = np.tile(np.expand_dims(Centers, axis=0), [N, 1, 1])
+    dist = np.sum((tile_x - tile_centers) ** 2, axis=-1)
+    return np.sqrt(dist)
 
 def qhull2D(sample):
     link = lambda a, b: concatenate((a, b[1:]))
     edge = lambda a, b: concatenate(([a], [b]))
+
     def dome(sample, base):
         h, t = base
         dists = dot(sample - h, dot(((0, -1), (1, 0)), (t - h)))
         outer = repeat(sample, dists > 0, 0)
         if len(outer):
             pivot = sample[argmax(dists)]
             return link(dome(outer, edge(h, pivot)),
@@ -58,125 +73,146 @@
     if len(sample) > 2:
         axis = sample[:, 0]
         base = take(sample, [argmin(axis), argmax(axis)], 0)
         return link(dome(sample, base), dome(sample, base[::-1]))
     else:
         return sample
 
+
 def minBoundingRect(hull_points_2d):
-    #print "Input convex hull points: "
-    #print hull_points_2d
+    # print "Input convex hull points: "
+    # print hull_points_2d
 
     # Compute edges (x2-x1,y2-y1)
-    edges = zeros( (len(hull_points_2d)-1,2) ) # empty 2 column array
-    for i in range( len(edges) ):
-        edge_x = hull_points_2d[i+1,0] - hull_points_2d[i,0]
-        edge_y = hull_points_2d[i+1,1] - hull_points_2d[i,1]
-        edges[i] = [edge_x,edge_y]
-    #print "Edges: \n", edges
+    edges = zeros((len(hull_points_2d) - 1, 2))  # empty 2 column array
+    for i in range(len(edges)):
+        edge_x = hull_points_2d[i + 1, 0] - hull_points_2d[i, 0]
+        edge_y = hull_points_2d[i + 1, 1] - hull_points_2d[i, 1]
+        edges[i] = [edge_x, edge_y]
+    # print "Edges: \n", edges
 
     # Calculate edge angles   atan2(y/x)
-    edge_angles = zeros( (len(edges)) ) # empty 1 column array
-    for i in range( len(edge_angles) ):
-        edge_angles[i] = math.atan2( edges[i,1], edges[i,0] )
-    #print "Edge angles: \n", edge_angles
+    edge_angles = zeros((len(edges)))  # empty 1 column array
+    for i in range(len(edge_angles)):
+        edge_angles[i] = math.atan2(edges[i, 1], edges[i, 0])
+    # print "Edge angles: \n", edge_angles
 
     # Check for angles in 1st quadrant
-    for i in range( len(edge_angles) ):
-        edge_angles[i] = abs( edge_angles[i] % (math.pi/2) ) # want strictly positive answers
-    #print "Edge angles in 1st Quadrant: \n", edge_angles
+    for i in range(len(edge_angles)):
+        edge_angles[i] = abs(edge_angles[i] % (math.pi / 2))  # want strictly positive answers
+    # print "Edge angles in 1st Quadrant: \n", edge_angles
 
     # Remove duplicate angles
     edge_angles = unique(edge_angles)
-    #print "Unique edge angles: \n", edge_angles
+    # print "Unique edge angles: \n", edge_angles
 
     # Test each angle to find bounding box with smallest area
-    min_bbox = (0, sys.maxsize, 0, 0, 0, 0, 0, 0) # rot_angle, area, width, height, min_x, max_x, min_y, max_y  sys.maxint
-    print ("Testing", len(edge_angles), "possible rotations for bounding box... \n")
-    for i in range( len(edge_angles) ):
+    min_bbox = (0, sys.maxsize, 0, 0, 0, 0, 0, 0)  # rot_angle, area, width, height, min_x, max_x, min_y, max_y  sys.maxint
+    print("Testing", len(edge_angles), "possible rotations for bounding box... \n")
+    for i in range(len(edge_angles)):
 
         # Create rotation matrix to shift points to baseline
         # R = [ cos(theta)      , cos(theta-PI/2)
         #       cos(theta+PI/2) , cos(theta)     ]
-        R = array([ [ math.cos(edge_angles[i]), math.cos(edge_angles[i]-(math.pi/2)) ], [ math.cos(edge_angles[i]+(math.pi/2)), math.cos(edge_angles[i]) ] ])
-        #print "Rotation matrix for ", edge_angles[i], " is \n", R
+        R = array([[math.cos(edge_angles[i]), math.cos(edge_angles[i] - (math.pi / 2))], [math.cos(edge_angles[i] + (math.pi / 2)), math.cos(edge_angles[i])]])
+        # print "Rotation matrix for ", edge_angles[i], " is \n", R
 
         # Apply this rotation to convex hull points
-        rot_points = dot(R, transpose(hull_points_2d) ) # 2x2 * 2xn
-        #print "Rotated hull points are \n", rot_points
+        rot_points = dot(R, transpose(hull_points_2d))  # 2x2 * 2xn
+        # print "Rotated hull points are \n", rot_points
 
         # Find min/max x,y points
         min_x = nanmin(rot_points[0], axis=0)
         max_x = nanmax(rot_points[0], axis=0)
         min_y = nanmin(rot_points[1], axis=0)
         max_y = nanmax(rot_points[1], axis=0)
-        #print "Min x:", min_x, " Max x: ", max_x, "   Min y:", min_y, " Max y: ", max_y
+        # print "Min x:", min_x, " Max x: ", max_x, "   Min y:", min_y, " Max y: ", max_y
 
         # Calculate height/width/area of this bounding rectangle
         width = max_x - min_x
         height = max_y - min_y
-        area = width*height
-        #print "Potential bounding box ", i, ":  width: ", width, " height: ", height, "  area: ", area
+        area = width * height
+        # print "Potential bounding box ", i, ":  width: ", width, " height: ", height, "  area: ", area
 
         # Store the smallest rect found first (a simple convex hull might have 2 answers with same area)
         if (area < min_bbox[1]):
-            min_bbox = ( edge_angles[i], area, width, height, min_x, max_x, min_y, max_y )
+            min_bbox = (edge_angles[i], area, width, height, min_x, max_x, min_y, max_y)
         # Bypass, return the last found rect
-        #min_bbox = ( edge_angles[i], area, width, height, min_x, max_x, min_y, max_y )
+        # min_bbox = ( edge_angles[i], area, width, height, min_x, max_x, min_y, max_y )
 
     # Re-create rotation matrix for smallest rect
     angle = min_bbox[0]
-    R = array([ [ math.cos(angle), math.cos(angle-(math.pi/2)) ], [ math.cos(angle+(math.pi/2)), math.cos(angle) ] ])
-    #print "Projection matrix: \n", R
+    R = array([[math.cos(angle), math.cos(angle - (math.pi / 2))], [math.cos(angle + (math.pi / 2)), math.cos(angle)]])
+    # print "Projection matrix: \n", R
 
     # Project convex hull points onto rotated frame
-    proj_points = dot(R, transpose(hull_points_2d) ) # 2x2 * 2xn
-    #print "Project hull points are \n", proj_points
+    proj_points = dot(R, transpose(hull_points_2d))  # 2x2 * 2xn
+    # print "Project hull points are \n", proj_points
 
     # min/max x,y points are against baseline
     min_x = min_bbox[4]
     max_x = min_bbox[5]
     min_y = min_bbox[6]
     max_y = min_bbox[7]
-    #print "Min x:", min_x, " Max x: ", max_x, "   Min y:", min_y, " Max y: ", max_y
+    # print "Min x:", min_x, " Max x: ", max_x, "   Min y:", min_y, " Max y: ", max_y
 
     # Calculate center point and project onto rotated frame
-    center_x = (min_x + max_x)/2
-    center_y = (min_y + max_y)/2
-    center_point = dot( [ center_x, center_y ], R )
-    #print "Bounding box center point: \n", center_point
+    center_x = (min_x + max_x) / 2
+    center_y = (min_y + max_y) / 2
+    center_point = dot([center_x, center_y], R)
+    # print "Bounding box center point: \n", center_point
 
     # Calculate corner points and project onto rotated frame
-    corner_points = zeros( (4,2) ) # empty 2 column array
-    corner_points[0] = dot( [ max_x, min_y ], R )
-    corner_points[1] = dot( [ min_x, min_y ], R )
-    corner_points[2] = dot( [ min_x, max_y ], R )
-    corner_points[3] = dot( [ max_x, max_y ], R )
-    #print "Bounding box corner points: \n", corner_points
+    corner_points = zeros((4, 2))  # empty 2 column array
+    corner_points[0] = dot([max_x, min_y], R)
+    corner_points[1] = dot([min_x, min_y], R)
+    corner_points[2] = dot([min_x, max_y], R)
+    corner_points[3] = dot([max_x, max_y], R)
+    # print "Bounding box corner points: \n", corner_points
 
-    #print "Angle of rotation: ", angle, "rad  ", angle * (180/math.pi), "deg"
+    # print "Angle of rotation: ", angle, "rad  ", angle * (180/math.pi), "deg"
+
+    return (angle, min_bbox[1], min_bbox[2], min_bbox[3], center_point, corner_points)  # rot_angle, area, width, height, center_point, corner_points
 
-    return (angle, min_bbox[1], min_bbox[2], min_bbox[3], center_point, corner_points) # rot_angle, area, width, height, center_point, corner_points
 
 def Get_MBR(points):
     '求平面包围盒'
     hull_points = qhull2D(points)  # Find convex hull 查找凸包
     hull_points = hull_points[::-1]  # Reverse order of points, to match output from other qhull implementations 颠倒点的顺序，以匹配其他qhull实现的输出
     print('凸包点: \n', hull_points, "\n")
     (rot_angle, area, width, height, center_point, corner_points) = minBoundingRect(hull_points)  # Find minimum area bounding rectangle 查找最小面积边界矩形
-    print ("Minimum area bounding box 最小面积边界框:")
-    print ("Rotation angle 旋转角:", rot_angle, "rad  (", rot_angle*(180/math.pi), "deg )")
-    print ("Width 宽度:", width, " Height 长度:", height, "  Area 面积:", area)
-    print ("Center point 中心点: \n", center_point) # numpy array
-    print ("Corner points 转角点: \n", corner_points, "\n")  # numpy array
-    RectangleProperties = np.array([width,height,area])  # 合并矩形属性
-    return corner_points,RectangleProperties
+    print("Minimum area bounding box 最小面积边界框:")
+    print("Rotation angle 旋转角:", rot_angle, "rad  (", rot_angle * (180 / math.pi), "deg )")
+    print("Width 宽度:", width, " Height 长度:", height, "  Area 面积:", area)
+    print("Center point 中心点: \n", center_point)  # numpy array
+    print("Corner points 转角点: \n", corner_points, "\n")  # numpy array
+    RectangleProperties = np.array([width, height, area])  # 合并矩形属性
+    return corner_points, RectangleProperties
+
 
 def Get_KB(x1, y1, x2, y2):
     '通过两点式求二维直线的截距和斜率'
     # 计算斜率
     slope = (y2 - y1) / (x2 - x1)
     # 计算截距
     intercept = y1 - slope * x1
     print(f"斜率：{slope}")
     print(f"截距：{intercept}")
-    return slope, intercept
+    return slope, intercept
+
+
+def get_cm_all():
+    '获得plt和pv支持的colormap列表'
+    colormaps = plt.colormaps()  # 列出所有colormap的名字
+    j = 0
+    for i in colormaps:
+        print('colormap', j, ':', i)
+        j += 1
+    return colormaps
+
+
+def view_pointclouds(xyz,i,i_name='intensity',colormap='gray'):
+    '基于pyvista显示点云'
+    points = pv.PolyData(xyz)  # 建立pv类
+    points[i_name] = i  # 将特征填入类
+    # 显示点云
+    points.plot(eye_dome_lighting=True,cmap=colormap)
```

### Comparing `zelas-1.3.240505/zelas/ransac.py` & `zelas-1.3.240507/zelas/ransac.py`

 * *Files identical despite different names*

### Comparing `zelas-1.3.240505/zelas/shield.py` & `zelas-1.3.240507/zelas/shield.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,17 +4,17 @@
 from matplotlib import pyplot as plt
 from matplotlib.patches import Circle
 import math
 import multiprocessing as mp  # 添加多进程（并行计算）库
 import pyransac3d as pyrsc
 import zelas.Multispectral as p1  # 添加自己的库
 import plotly.graph_objects as go  # 添加其他显示库
-import voxel as vl  # 添加体素类
-import ransac as rs
-import Ellipse as ep
+import zelas.voxel as vl  # 添加体素类
+import zelas.ransac as rs
+import zelas.Ellipse as ep
 
 
 def random_partition(n, n_data):
     """return n random rows of data and the other len(data) - n rows"""
     all_idxs = np.arange(n_data)  # 获取n_data下标索引
     np.random.shuffle(all_idxs)  # 打乱下标索引
     idxs1 = all_idxs[:n]
```

### Comparing `zelas-1.3.240505/zelas/voxel.py` & `zelas-1.3.240507/zelas/voxel.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,15 +45,14 @@
         self.VoxelLength = (voxel_end - self.voxel_start + 1).astype(int)  # 刷新体元数量
         self.VoxelLengthDigit = [len(str(self.VoxelLength[0])), len(str(self.VoxelLength[1])), len(str(self.VoxelLength[2]))]  # 刷新体元长宽高的位数
         print('体素的长宽高为', self.VoxelLength)
         # self.voxel_values = np.zeros(self.VoxelLength, dtype=np.float16)  # 设置三维体素(类型设置为16位浮点型)
         self.voxel_values = np.zeros(self.VoxelLength, dtype=np.float32)  # 设置三维体素(类型设置为16位浮点型)
         print('体素已建立')
 
-
     def P2V(self, values):
         '''
         点云连接体素（默认使用并行计算），并返回下标
         :param values: 点云特征值数组
         :return: 每个体素的周围26邻域中的有值体素位置
                  其他返回在类的属性中
         '''
@@ -90,15 +89,14 @@
             for j in range(self.VoxelLength[1]):
                 self.pixel_min_un[k,0] = i
                 self.pixel_min_un[k,1] = j
                 self.pixel_min_un[k,2] = pixel_values_min[i,j]
                 k += 1
         return self.pixel_min_un
 
-
     def P2Vm(self, values):
         '点云体素化赋值（平均值版）'
         self.voxel_values = np.zeros([int(self.VoxelLength[0]), int(self.VoxelLength[1]), int(self.VoxelLength[2])],dtype=np.float32)  # 存储总值的容器
         voxel_num = np.zeros([int(self.VoxelLength[0]), int(self.VoxelLength[1]), int(self.VoxelLength[2])],dtype=np.float32)  # 存储体素数量的容器
         for i in tqdm(range(self.num)):
             self.points_local[i, :] = np.floor(self.xyz[i, :] / self.pixel) - self.voxel_start  # 遍历点属于哪个体素
             self.voxel_values[int(self.points_local[i, 0]), int(self.points_local[i, 1]), int(self.points_local[i, 2])] += values[i]  # 体素赋值
@@ -153,15 +151,15 @@
         '''
         查询某一批点云的所在体素的位置
         :param xyz_: 某一批点云的三维坐标
         :return: 这批点云所在的体素位置
         '''
         points_local_new = np.empty([len(xyz_), 3])  # 存储当前点云所在体素的位置
         for i in range(len(xyz_)):
-            points_local_new[i, :] = np.round(xyz_[i, :3] / self.pixel) - self.voxel_start  # 遍历点属于哪个体素
+            points_local_new[i, :] = np.floor(xyz_[i, :3] / self.pixel) - self.voxel_start  # 遍历点属于哪个体素
         return points_local_new
 
     def V2P(self, v_local_un):
         '体素转点云'
         lwd_321 = v_local_un[:, 0] * (10 ** self.VoxelLengthDigit[-2]) + v_local_un[:, 1] + v_local_un[:, 2] * (10 ** (self.VoxelLengthDigit[-1] * (-1)))
         p_lwd_321 = self.points_local[:, 0] * (10 ** self.VoxelLengthDigit[-2]) + self.points_local[:, 1] + self.points_local[:, 2] * (10 ** (self.VoxelLengthDigit[-1] * (-1)))
         points_index = np.isin(p_lwd_321, lwd_321)  # 提取点云的下标 by:Zelas
@@ -569,14 +567,86 @@
     # 单个点在un上的位置，然后将标签赋值
     p_lwd_321 = points_local[:, 0] * (10 ** VoxelLengthDigit[-2]) + points_local[:, 1] + points_local[:, 2] * (10 ** (VoxelLengthDigit[-1] * (-1)))  # 点在体素坐标的匹配标签
     labels_points = np.empty(len(p_lwd_321))  # 每个点云的标签容器
     for i in range(len(p_lwd_321)):  # 遍历点云
         labels_points[i] = labels[np.where(un_321 == p_lwd_321[i])]  # 对每个点云赋值标签
     return labels, labels_points  # 返回每个体素的标签和每个点云的标签
 
+def FindConnectedSeed(seed_voxel_local,points_local_un,binary,VoxelLengthDigit,points_local,num_Nei=26):
+    '''
+    基于种子体素连通区域增长
+    :param seed_voxel_local: 种子体素位置
+    :param points_local_un:所有有值体素的位置
+    :param binary: 三维体素
+    :param VoxelLengthDigit: 体素长宽高位数
+    :param points_local: 体素中每个点云在体素上的位置
+    :param num_Nei: 搜索的邻域数量，默认为26，实际上可以挑选6/18/26/128邻域等
+    :return: 每个体素的标签和每个点云的标签，其中0为无用位置
+    '''
+    '1.寻找每个体素的有效邻域体素'
+    # 先找points_local_un的6/18/26/56/80/128邻域
+    limit_box = np.array(binary.shape)  # 给出默认体素尺寸限制
+    FunName_FindNei = 'Nei_'+str(num_Nei)  # 函数名
+    FindNei = globals()[FunName_FindNei]  # 使用 globals() 函数获取函数引用
+    num_un = len(points_local_un)  # 有值体素数量
+    a = []  # 有值体素的邻域嵌套数组
+    for i in range(num_un):
+        print('当前体素',i)
+        x = points_local_un[i, 0]
+        y = points_local_un[i, 1]
+        z = points_local_un[i, 2]  # 遍历到当前体素位置
+        neighbour = FindNei(x,y,z)  # 函数引用-求邻域
+        # 找到“正常”的邻域
+        neighbour = neighbour[neighbour[:, 0] < limit_box[0]]
+        neighbour = neighbour[neighbour[:, 0] >= 0]
+        neighbour = neighbour[neighbour[:, 1] < limit_box[1]]
+        neighbour = neighbour[neighbour[:, 1] >= 0]
+        neighbour = neighbour[neighbour[:, 2] < limit_box[2]]
+        neighbour = neighbour[neighbour[:, 2] >= 0]
+        # 清除无值邻域
+        for j in range(len(neighbour)):  # binary(neighbour(1,r),neighbour(2,r),neighbour(3,r))~=0
+            print('当前邻域', j)
+            b_x = int(neighbour[j, 0])
+            b_y = int(neighbour[j, 1])
+            b_z = int(neighbour[j, 2])
+            if binary[b_x, b_y, b_z] == 0:
+                neighbour[j, :] = [-1, -1, -1]
+        neighbour = neighbour[neighbour[:, 2] >= 0]
+        a.append(neighbour)
+    '2:种子体素区域增长并划分标签'
+    labels = np.zeros(num_un)  # 建立空标签数组  默认为0
+    arange_ = np.arange(num_un)  # 自增标签
+    label_ = 1  # 标签自增工具
+    num_seed = len(seed_voxel_local)  # 种子体素数量
+    seed_321 = seed_voxel_local[:, 0] * (10 ** VoxelLengthDigit[-2]) + seed_voxel_local[:, 1] + seed_voxel_local[:, 2] * (10 ** (VoxelLengthDigit[-1] * (-1)))  # 种子体素标签
+    un_321 = points_local_un[:, 0] * (10 ** VoxelLengthDigit[-2]) + points_local_un[:, 1] + points_local_un[:, 2] * (10 ** (VoxelLengthDigit[-1] * (-1)))  # 有值体素标签
+    for i in range(num_seed):  # 对种子点进行循环
+        seed_321_ = seed_321[i]  # 当前种子体素下标
+        # ind = np.isin(un_321,seed_321)  # 当前种子体素下标
+        ind = np.where(np.isin(un_321, seed_321_))[0]  # 当前种子体素下标
+        if labels[ind] == 0:  # 如果还没有给标签
+            labels[ind] = label_  # 给一个起始便签
+            vessel = a[ind[0]]  # 新便签起始邻域
+            while len(vessel) > 0:  # 种子体素还有邻域时
+                v_321_0_ = vessel[0, 0] * (10 ** VoxelLengthDigit[-2]) + vessel[0, 1] + vessel[0, 2] * (10 ** (VoxelLengthDigit[-1] * (-1)))  # 容器开始的标签
+                index_ = np.isin(un_321, v_321_0_)  # 所在的un下标
+                if labels[index_] == 0:  # 如果是没分类的体素
+                    index_ = int(arange_[index_])  # 当前邻域容器的下标
+                    vessel = np.vstack([vessel, a[index_]])  # 增加容器
+                    labels[index_] = label_  # 赋予便签
+                vessel = np.delete(vessel, 0, axis=0)  # 删除已用的邻域
+                print('总进度', np.round(i / num_seed, 2), '标签', label_, '剩余待处理体素', len(vessel))
+            label_ += 1  # 标签增加
+    '3：体素标签转所有点云标签'
+    p_lwd_321 = points_local[:, 0] * (10 ** VoxelLengthDigit[-2]) + points_local[:, 1] + points_local[:, 2] * (10 ** (VoxelLengthDigit[-1] * (-1)))  # 点在体素坐标的匹配标签
+    labels_points = np.empty(len(p_lwd_321))  # 每个点云的标签容器
+    for i in range(len(p_lwd_321)):  # 遍历点云
+        labels_points[i] = labels[np.where(un_321 == p_lwd_321[i])]  # 对每个点云赋值标签
+    return labels, labels_points  # 返回每个体素的标签和每个点云的标签
+
 def FindNeiSameLabel(points_local_un, binary, VoxelLengthDigit, binary_limit, points_local, limit_box=None):
     '''区域增长划定相同的体素标签
     :param points_local: 体素中每个点云在体素上的位置
     :param binary_limit: 每个类别的特征值限制数组 [特征均值_i,特征方差_i]*n ,i=1:n
     :param points_local_un: 所有有值体素的位置
     :param binary: 三维体素
     :param VoxelLengthDigit：体素长宽高位数
@@ -1174,15 +1244,15 @@
             # labels_points[i] = labels[np.int16(np.array(np.where(un_321 == p_lwd_321[i])))]
             labels_points[i] = labels[np.where(un_321 == p_lwd_321[i])]
         return labels, labels_points  # labels:每个像素的标签,labels_points：每个点云的标签
 
 class voxel3:
     '建立体素类（笛卡尔坐标系但体素长宽高尺寸不一致）'
     # 输入点云位置，体元边长，找最邻近的邻域数量
-    def __init__(self, xyz, rr_x=0,rr_y=0,rr_z=0):  # 每个点云所在体素的位置，总共的体素。体素所在的位置
+    def __init__(self, xyz, rr_x=1,rr_y=1,rr_z=1):  # 每个点云所在体素的位置，总共的体素。体素所在的位置
         self.xyz = xyz  # 存储点云位置
         self.num = len(self.xyz)  # 存储点云数量
         self.rr = [rr_x,rr_y,rr_z]  # 体素的点云分辨率
         print('体素三轴分辨率为',self.rr)
         self.SpaceBoundary = np.array([self.xyz.max(axis=0), self.xyz.min(axis=0)])  # 点云的边界
         self.find_VoxelLength()  # 求长宽高 的数量
         self.points_local = np.empty([self.num, 3])  # 每个点云所在的体素位置
```

### Comparing `zelas-1.3.240505/zelas.egg-info/PKG-INFO` & `zelas-1.3.240507/zelas.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: zelas
-Version: 1.3.240505
+Version: 1.3.240507
 Summary: Professor Liying Wang official point clouds database 
 Home-page: UNKNOWN
 Author: Zelas You
 Author-email: youze1997@163.com
 License: UNKNOWN
 Description: Produced by CCG.Lidar Point Cloud Research Institute
 Keywords: python,las
 Platform: UNKNOWN
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
-Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
```

