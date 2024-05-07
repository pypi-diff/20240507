# Comparing `tmp/covplan-0.1.0.tar.gz` & `tmp/covplan-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "covplan-0.1.0.tar", last modified: Thu Mar 21 15:50:22 2024, max compression
+gzip compressed data, was "covplan-0.2.0.tar", last modified: Tue May  7 14:20:48 2024, max compression
```

## Comparing `covplan-0.1.0.tar` & `covplan-0.2.0.tar`

### file list

```diff
@@ -1,23 +1,25 @@
-drwxrwxrwx   0        0        0        0 2024-03-21 15:50:22.752719 covplan-0.1.0/
--rw-rw-rw-   0        0        0     1091 2023-09-05 15:09:52.000000 covplan-0.1.0/LICENSE
--rw-rw-rw-   0        0        0     3342 2024-03-21 15:50:22.751720 covplan-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     2520 2024-03-21 15:19:32.000000 covplan-0.1.0/README.md
--rw-rw-rw-   0        0        0      869 2024-03-21 15:48:44.000000 covplan-0.1.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-03-21 15:50:22.753719 covplan-0.1.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-03-21 15:50:22.709414 covplan-0.1.0/src/
-drwxrwxrwx   0        0        0        0 2024-03-21 15:50:22.732720 covplan-0.1.0/src/covplan/
--rw-rw-rw-   0        0        0     1796 2024-03-18 20:06:00.000000 covplan-0.1.0/src/covplan/angles.py
--rw-rw-rw-   0        0        0     8617 2023-04-27 12:59:51.000000 covplan-0.1.0/src/covplan/convert_coordinates.py
--rw-rw-rw-   0        0        0     1103 2024-03-21 14:52:59.000000 covplan-0.1.0/src/covplan/coverage_path_planner.py
--rw-rw-rw-   0        0        0    10552 2024-03-21 13:48:42.000000 covplan-0.1.0/src/covplan/dubins_path_planner.py
--rw-rw-rw-   0        0        0    12732 2024-03-21 13:49:09.000000 covplan-0.1.0/src/covplan/field.py
--rw-rw-rw-   0        0        0     9110 2024-03-20 16:00:47.000000 covplan-0.1.0/src/covplan/lines.py
--rw-rw-rw-   0        0        0      719 2023-09-20 16:23:41.000000 covplan-0.1.0/src/covplan/main.py
-drwxrwxrwx   0        0        0        0 2024-03-21 15:50:22.749719 covplan-0.1.0/src/covplan.egg-info/
--rw-rw-rw-   0        0        0     3342 2024-03-21 15:50:22.000000 covplan-0.1.0/src/covplan.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      416 2024-03-21 15:50:22.000000 covplan-0.1.0/src/covplan.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-21 15:50:22.000000 covplan-0.1.0/src/covplan.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       81 2024-03-21 15:50:22.000000 covplan-0.1.0/src/covplan.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-03-21 15:50:22.000000 covplan-0.1.0/src/covplan.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-03-21 15:50:22.746719 covplan-0.1.0/tests/
--rw-rw-rw-   0        0        0      971 2024-03-21 15:17:24.000000 covplan-0.1.0/tests/test_main.py
+drwxrwxrwx   0        0        0        0 2024-05-07 14:20:48.764154 covplan-0.2.0/
+-rw-rw-rw-   0        0        0     1091 2023-09-05 15:09:52.000000 covplan-0.2.0/LICENSE
+-rw-rw-rw-   0        0        0     3753 2024-05-07 14:20:48.763154 covplan-0.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2929 2024-05-07 14:20:32.000000 covplan-0.2.0/README.md
+-rw-rw-rw-   0        0        0      869 2024-05-07 14:20:11.000000 covplan-0.2.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-07 14:20:48.764154 covplan-0.2.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-07 14:20:48.732998 covplan-0.2.0/src/
+drwxrwxrwx   0        0        0        0 2024-05-07 14:20:48.749153 covplan-0.2.0/src/covplan/
+-rw-rw-rw-   0        0        0       75 2024-05-07 10:58:53.000000 covplan-0.2.0/src/covplan/__init__.py
+-rw-rw-rw-   0        0        0     8617 2023-04-27 12:59:51.000000 covplan-0.2.0/src/covplan/convert_coordinates.py
+-rw-rw-rw-   0        0        0     2237 2024-05-07 10:58:44.000000 covplan-0.2.0/src/covplan/coverage_path_planner.py
+-rw-rw-rw-   0        0        0    12336 2024-05-07 13:38:24.000000 covplan-0.2.0/src/covplan/dubins_path_planner.py
+-rw-rw-rw-   0        0        0    14038 2024-05-06 15:41:09.000000 covplan-0.2.0/src/covplan/field.py
+-rw-rw-rw-   0        0        0     8492 2024-05-07 12:55:51.000000 covplan-0.2.0/src/covplan/lines.py
+drwxrwxrwx   0        0        0        0 2024-05-07 14:20:48.762154 covplan-0.2.0/src/covplan.egg-info/
+-rw-rw-rw-   0        0        0     3753 2024-05-07 14:20:48.000000 covplan-0.2.0/src/covplan.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      456 2024-05-07 14:20:48.000000 covplan-0.2.0/src/covplan.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-07 14:20:48.000000 covplan-0.2.0/src/covplan.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       81 2024-05-07 14:20:48.000000 covplan-0.2.0/src/covplan.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-05-07 14:20:48.000000 covplan-0.2.0/src/covplan.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-07 14:20:48.761154 covplan-0.2.0/tests/
+-rw-rw-rw-   0        0        0      971 2024-05-06 15:42:16.000000 covplan-0.2.0/tests/test_field.py
+-rw-rw-rw-   0        0        0      699 2024-05-06 15:34:03.000000 covplan-0.2.0/tests/test_line.py
+-rw-rw-rw-   0        0        0      925 2024-05-07 13:15:18.000000 covplan-0.2.0/tests/test_main.py
+-rw-rw-rw-   0        0        0      492 2024-05-07 11:00:20.000000 covplan-0.2.0/tests/test_plan.py
```

### Comparing `covplan-0.1.0/LICENSE` & `covplan-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `covplan-0.1.0/PKG-INFO` & `covplan-0.2.0/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: covplan
-Version: 0.1.0
+Version: 0.2.0
 Summary: A package to generate a guidance trajectory for complete 2D coverage of a region of interest
 Author-email: "Sanjeev Kumar R. S." <sanjeev.k.r.sudha@ntnu.no>, "Ibrahim A. Hameed" <ibib@ntnu.no>
 Project-URL: Homepage, https://github.com/sanjeevrs2000/cpp
 Project-URL: Bug Tracker, https://github.com/sanjeevrs2000/cpp/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -15,52 +15,71 @@
 Requires-Dist: scipy>=1.10
 Requires-Dist: scikit-learn>=1.2.0
 Requires-Dist: wheel
 Requires-Dist: utm
 Requires-Dist: folium
 Requires-Dist: python-tsp>=0.3
 
-# Complete coverage Path Planning (CCPP)
+# CovPlan
 
-[![PyPI](https://img.shields.io/pypi/v/cc_pathplanner?color=blue&label=pypi)](https://pypi.org/project/cc-pathplanner/0.1.0/)
-[![PyPi license](https://img.shields.io/pypi/l/ansicolortags.svg)](https://pypi.org/project/cc-pathplanner/0.1.0/)
+A Python package for coverage path planning
 
+[![PyPI](https://img.shields.io/pypi/v/covplan?color=blue&label=pypi)](https://pypi.org/project/covplan/0.2.0/)
+[![PyPi license](https://img.shields.io/pypi/l/ansicolortags.svg)](https://pypi.org/project/covplan/0.2.0/)
 
-## Getting started
-This repository contains a program which generates a guidance trajectory for complete 2D coverage. It can be used for operations where complete coverage of an Area of Interest (AoI) is required for various applications.
-The package can be installed from PyPi by running 'pip install covplan'
+This repository can be used for generating guidance trajectories for complete field coverage. It can be used for operations where complete coverage of an Area of Interest (AoI) is required for various applications. It is an updated Python implementation of the method that was presented in [this paper](https://journals.sagepub.com/doi/full/10.5772/56248).
+> Hameed IA, Bochtis D, Sørensen CA. An Optimized Field Coverage Planning Approach for Navigation of Agricultural Robots in Fields Involving Obstacle Areas. International Journal of Advanced Robotic Systems. 2013;10(5). doi:10.5772/56248
+
+
+## Installation
+
+The package can be installed using pip 
 
+```shell
+pip install covplan
+```
+
+## Getting started
 
-## How to use the program
-To use the program, run `coverage_path_planner.covplan(input_file, params)`. It returns a list of coordinates that compose a path for complete coverage.
+To generate a guidance trajectory for full coverage, use the API `covplan.pathplan(input_file, params)`. It returns a list of coordinates that compose a path for complete coverage.
 In the input file, describe the boundaries of the AoI using its lat-lon coordinates in the following format:  
 ```
   lat1  lon1
   lat2  lon2
   ...
   lat1  lon1
   NaN  NaN
 ```
 Ensure that the AoI is a closed polygon, by keeping the first coordinate the same as the last coordinate. Separate different polygons by including a `NaN NaN` at the end. Also ensure that the coordinates of the polygon are described clockwise, and counter-clockwise for any obstacles and forbidden regions.
-`coverage_path_planner.find_min(input_file, params)` runs a single objective optimizer to find the driving angle that minimizes the trajectory length for a given AoI and the specified parameters.
+`covplan.find_min(input_file, params)` runs a single objective optimizer to find the driving angle that minimizes the trajectory length for a given AoI and the specified parameters.
 
-## Example usage
+### Example usage
 ```python
-from covplan import coverage_path_planner
+from covplan import pathplan
 
 def main():
 	n_clusters=4	#number of sections
 	r=2	#radius for Dubins curves
 	input_file='sample_area.txt' #location of the input file containing coordinates of the field
 	width = 10	#distance between tracks
 	driving_angle=90	#angle wrt X-axis in degrees
 	no_hd=0	#number of margins around boundary (each with distance=0.5*width) if needed, otherwise 0
 	
-	op=coverage_path_planner.covplan(input_file,num_hd=no_hd,width=width,theta=driving_angle,num_clusters=n_clusters,radius=r,visualize=False) # returns list of waypoint coordinates composing full trajectory for coverage
+	op=pathplan(input_file,num_hd=no_hd,width=width,theta=driving_angle,num_clusters=n_clusters,radius=r,visualize=False) # returns list of waypoint coordinates composing full trajectory for coverage
 	print('The trajectory for full coverage consists of the following waypoints:',op)
 	
-	min=coverage_path_planner.find_min(input_file,width=width,num_hd=no_hd,num_clusters=n_clusters,radius=r,verbose=True)  # runs optimizer and returns angle corresponding to minimum path length
-	# print('Angle for trajectory with minimum length:', min)
 
 if __name__ == '__main__':
 	main()
 ```
+
+## Documentation
+
+The full documentation can be found [here](https://covplan.readthedocs.io/).
+
+## Contributing
+
+Contributions are always welcome!
+
+See [contributing.md](/contributing.md) for ways to get started.
+
+Please adhere to this project's [code of conduct](/contributing.md#code-of-conduct)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `covplan-0.1.0/pyproject.toml` & `covplan-0.2.0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=0.61"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "covplan"
-version = "0.1.0"
+version = "0.2.0"
 authors = [
   { name="Sanjeev Kumar R. S.", email="sanjeev.k.r.sudha@ntnu.no" },
   { name="Ibrahim A. Hameed", email="ibib@ntnu.no" }
 ]
 description = "A package to generate a guidance trajectory for complete 2D coverage of a region of interest"
 readme = "README.md"
 requires-python = ">=3.7"
```

### Comparing `covplan-0.1.0/src/covplan/convert_coordinates.py` & `covplan-0.2.0/src/covplan/convert_coordinates.py`

 * *Files identical despite different names*

### Comparing `covplan-0.1.0/src/covplan/dubins_path_planner.py` & `covplan-0.2.0/src/covplan/dubins_path_planner.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 """
 Dubins path planner
 Courtesy to Atsushi Sakai(@Atsushi_twi)
+PythonRobotics https://github.com/AtsushiSakai/PythonRobotics
 """
 
 import sys
 import pathlib
 sys.path.append(str(pathlib.Path(__file__).parent.parent.parent))
-
 from math import sin, cos, atan2, sqrt, acos, pi, hypot
+from scipy.spatial.transform import Rotation as Rot
 import numpy as np
-from cc_pathplanner.angles import angle_mod, rot_mat_2d
 
 show_animation = True
 
 
 def plan_dubins_path(s_x, s_y, s_yaw, g_x, g_y, g_yaw, curvature,
                      step_size=0.1, selected_types=None):
     """
@@ -273,14 +273,82 @@
             current_length += step_size
 
         p_x, p_y, p_yaw = _interpolate(length, mode, max_curvature, origin_x,
                                        origin_y, origin_yaw, p_x, p_y, p_yaw)
 
     return p_x, p_y, p_yaw
 
+def rot_mat_2d(angle):
+    """
+    Create 2D rotation matrix from an angle
+    Parameters
+    ----------
+    angle :
+    Returns
+    -------
+    A 2D rotation matrix
+    Examples
+    --------
+    >>> angle_mod(-4.0)
+    """
+    return Rot.from_euler('z', angle).as_matrix()[0:2, 0:2]
+
+
+def angle_mod(x, zero_2_2pi=False, degree=False):
+    """
+    Angle modulo operation
+    Default angle modulo range is [-pi, pi)
+    Parameters
+    ----------
+    x : float or array_like
+        A angle or an array of angles. This array is flattened for
+        the calculation. When an angle is provided, a float angle is returned.
+    zero_2_2pi : bool, optional
+        Change angle modulo range to [0, 2pi)
+        Default is False.
+    degree : bool, optional
+        If True, then the given angles are assumed to be in degrees.
+        Default is False.
+    Returns
+    -------
+    ret : float or ndarray
+        an angle or an array of modulated angle.
+    Examples
+    --------
+    >>> angle_mod(-4.0)
+    2.28318531
+    >>> angle_mod([-4.0])
+    np.array(2.28318531)
+    >>> angle_mod([-150.0, 190.0, 350], degree=True)
+    array([-150., -170.,  -10.])
+    >>> angle_mod(-60.0, zero_2_2pi=True, degree=True)
+    array([300.])
+    """
+    if isinstance(x, float):
+        is_float = True
+    else:
+        is_float = False
+
+    x = np.asarray(x).flatten()
+    if degree:
+        x = np.deg2rad(x)
+
+    if zero_2_2pi:
+        mod_angle = x % (2 * np.pi)
+    else:
+        mod_angle = (x + np.pi) % (2 * np.pi) - np.pi
+
+    if degree:
+        mod_angle = np.rad2deg(mod_angle)
+
+    if is_float:
+        return mod_angle.item()
+    else:
+        return mod_angle
+
 
 def main():
     print("Dubins path planner sample start!!")
     import matplotlib.pyplot as plt
     # from utils.plot import plot_arrow
 
     start_x = 1.0  # [m]
@@ -308,8 +376,9 @@
     #     plt.legend()
     #     plt.grid(True)
     #     plt.axis("equal")
     #     plt.show()
 
 
 # if __name__ == '__main__':
-#     main()
+#     main()
+
```

### Comparing `covplan-0.1.0/src/covplan/field.py` & `covplan-0.2.0/src/covplan/field.py`

 * *Files 18% similar despite different names*

```diff
@@ -10,15 +10,29 @@
 from covplan.lines import computeAngle, pointOnLine, intersectLines, intersectPointOnLine
 from covplan.lines import getPoly, numPoly
 # from LLcoordinates import LLtoUTM, UTMtoLL
 import folium
 import utm
 
 class Field:
+
+	"""
+	Creates an object of the Area of interest(AoI); does the required preprocessing and further operations for generating a trajectory for coverage
+	"""
+
 	def __init__(self, filename, opw, nhp, theta):
+		
+		"""
+		args:
+		filename - location of the input textfile that describes the region of interest
+		opw - the distance between the parallel tracks, otherwise known as the operating width
+		nhp - number of headlands of boundary margins to be created within the AoI
+		theta - the angle that the parallel tracks make with the longitudinal axis
+
+		"""
 		self.opw = opw
 		self.nhp = nhp
 		self.theta = math.fmod( theta * pi/180+ 2 * pi, 2 * pi)
 		self.data = []  # data file containing field polygons
 		self.tracks = [] # field tracks
 		self.hd = []     #headland paths
 		self.labels = [] # labels of track clusters of Kmeans
@@ -42,14 +56,15 @@
 			ux,uy,z,l=utm.from_latlon(self.data[i][0],self.data[i][1])
 			self.utmzone=z
 			self.utm_l=l
 			self.data[i]=[ux,uy]
 
 
 	def showField(self):
+		"""Visualizes the desired path on a map"""
 
 		tracks_lower,tracks_upper = [], []
 		for i in range(0, len(self.tracks)):
 			tracks_lower.append((self.tracks[i][0,0] , self.tracks[i][0,1]))
 			tracks_upper.append((self.tracks[i][1,0] , self.tracks[i][1,1]))
 		tracks_lower = np.asarray(tracks_lower)
 		tracks_upper = np.asarray(tracks_upper)
@@ -99,14 +114,18 @@
 			
 			folium.PolyLine(self.hd_ll,color='red').add_to(map)
 
 		folium.Polygon(self.latlon,color='blue').add_to(map)
 		map.show_in_browser()
 
 	def trackGen(self):
+		"""
+		Generates parallel tracks for the AoI with the given theta and width, that together compose the overall tracjectory
+		"""
+
 		poly = getPoly(self.data, 1) 
 	
 		# find minimum bounding box (MBB)
 		xmin = np.min(poly[:,0])
 		xmax = np.max(poly[:,0])
 		ymin = np.min(poly[:,1])
 		ymax = np.max(poly[:,1])
@@ -164,14 +183,18 @@
 		self.track_len=0
 		for tr in self.tracks:
 			self.track_len+=np.sqrt((tr[0,0]-tr[1,0])**2 + (tr[0,1]-tr[1,1])**2)
 
 
 
 	def headlandGen(self):
+		"""
+		Generates boundary margins, otherwise known as headlands
+		each headland has a distance of width/2 in between them
+		"""
 
 		for i in  range(1, int(numPoly(self.data))+1):
 			poly = getPoly(self.data, i)
 			# check order: if ord < 0 it is anti-clockwise
 			ord = 0
 			for j in range(0, len(poly)-1):
 				ord += (poly[j+1,0]-poly[j,0])*(poly[j+1,1]+poly[j,1])
@@ -204,15 +227,20 @@
 				Y = np.hstack((Y,Y[0]))
 				#combine
 				tmp = np.vstack((X,Y)).T		
 				self.hd.append(tmp)
 				
 
 	def cluster(self,num_clusters=4):
-
+		"""
+		Divides the region of interest into sections/clusters by using K-means clustering
+		
+		args:
+		num_clusters - Number of sections into which the region is divided into
+		"""
 		self.num_clusters=num_clusters
 		np.random.seed(0)
 		data = []
 		for i in range(0, len(self.tracks)):
 			data.append((self.tracks[i][0,0] , self.tracks[i][0,1]))
 		data = np.asarray(data)
 
@@ -269,15 +297,18 @@
 	# 			happy = pl.waitforbuttonpress()
 
 
 	# 	self.robotinitpos = pts
 	# 	plt.close(1)
 
 	def tsp_opt(self):
-
+		"""
+		Finds optimal order of visits to the clusters/sections using a TSP solver
+		
+		"""
 		# self.getRobotIntialPoition()
 		self.robotinitpos=self.data[0]
 		#nodes locations using cluster centers and robot position at nodes number (n_cluster+1)
 		nodes = np.vstack((self.robotinitpos,self.cluster_centers))
 
 		
 		n_nodes = len(nodes)
@@ -297,15 +328,22 @@
 		path,_=solve_tsp_dynamic_programming(dist)
 		# path = solve_tsp( dist )
 		self.path=path
 		self.nodes=nodes				
 
 
 	def trajGen(self, turning_radius=1.5):
-		
+		"""
+		Generates complete trajectory for coverage
+		Uses Dubins curves to connect waypoints for generating a smooth trajectory
+
+		arg:
+		turning_radius - radius of the Dubins curves
+		"""
+
 		step_size = 1
 
 		self.turn_dist=0
 		tracks_lower,tracks_upper = [], []
 		for i in range(0, len(self.tracks)):
 			tracks_lower.append((self.tracks[i][0,0] , self.tracks[i][0,1]))
 			tracks_upper.append((self.tracks[i][1,0] , self.tracks[i][1,1]))
```

### Comparing `covplan-0.1.0/src/covplan/lines.py` & `covplan-0.2.0/src/covplan/lines.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,110 +1,94 @@
 from numpy import *
 from math import *
 import numpy as np
 import math, numpy.linalg
 import matplotlib.pyplot as plt
 
 def createLine(p1, p2):
-	'''
-	CREATELINE create a line from two points (p1 and p2) and return it as p1 (a point belonging to the line), 
+	"""
+	CREATELINE creates a line from two points (p1 and p2) and returns it as p1 (a point belonging to the line), 
 	and dx, dy (direction vector of the line) where dx=p1(:,1)-p2(:,1) and dy=p1(:,2)-p2(:,2).
 
 	Line is represented in a parametric form : [x0 y0 dx dy]
 	  x = x0 + t*dx
 	  y = y0 + t*dy;
 
-	 the line is represented by first one is a point belonging to the linethey are x0, y0 (point belongng to line) and 
+	 the line is represented by x0, y0 (point belongng to line) and 
 	 dx, dy (direction vector of the line).
 
-	l = CREATELINE(p1, p2) return the line going through the two given points.
-	'''
+	l = CREATELINE(p1, p2) returns the line going through the two given points.
+	"""
 	#line = np.array( [p1[0,0], p1[0,1], p2[0,0]-p1[0,0], p2[0,1]-p1[0,1] ])
 	#p1 = np.array(p1)
 	#p2 = np.array(p2)
 	line = []	#np.zeros([p1.shape[0],4])
 	if p1.size == 2:
 		line = [p1[0], p1[1], p2[0]-p1[0], p2[1]-p1[1]]
 	else:
 		for i in range(p1.size/2):
 			line.append([p1[i,0], p1[i,1], p2[i,0]-p1[i,0], p2[i,1]-p1[i,1]])
 	#line = np.array([p1,np.subtract(p2,p1)])
 	return line
 
 def pointOnLine(line, d):
-	'''
-	POINTONLINE create a point on a line at a given distance from line origin
+	"""
+	POINTONLINE creates a point on a line at a given distance from line origin
 	
-	P = POINTONLINE(LINE, D) create the point located on the line LINE, and
+	P = POINTONLINE(LINE, D) creates the point located on the line LINE, and
 	located at the distance D from origin of line.
 	LINE has the form [x0 y0 dx dy].
 	LINE and D should have the same number N of rows. The result will have
 	N rows ans 2 column (x and y positions).
-	'''
-
-	angle = lineAngle(line)
-	#point = np.zeros([len(d), 2])
-	point = []
-	for i in range(len(d)):
-		#point[i,:] = [line[0]+d[i]*math.cos(angle), line[1]+d[i]*math.sin(angle)];
-		point.append([line[0]+d[i]*math.cos(angle), line[1]+d[i]*math.sin(angle)])
-	return point
-
-def pointOnLine(line, d):
-	'''
-	POINTONLINE create a point on a line at a given distance from line origin
-	
-	P = POINTONLINE(LINE, D) create the point located on the line LINE, and
-	located at the distance D from origin of line.
-	LINE has the form [x0 y0 dx dy].
-	LINE and D should have the same number N of rows. The result will have
-	N rows ans 2 column (x and y positions).
-	'''
+	"""
 
 	angle = lineAngle(line)
 	#point = np.zeros([len(d), 2])
 	point = []
 	for i in range(len(d)):
 		#point[i,:] = [line[0]+d[i]*math.cos(angle), line[1]+d[i]*math.sin(angle)];
 		point.append([line[0]+d[i]*math.cos(angle), line[1]+d[i]*math.sin(angle)])
 	return np.array(point, dtype=np.double)
 
 def lineAngle(line):
-	'''
-	LINEANGLE return angle between lines
+	"""
+	LINEANGLE returns slope of the line
 	a = LINEANGLE(line) return the angle between horizontal, right-axis
 	and the given line. Angle is given in radians, between 0 and 2*pi,
 	in counter-clockwise direction.
 	see createLine for more details on line representation.
-	'''
+	"""
 	# one line
 	#theta = math.fmod(math.atan2(line[3], line[2]) + 2*pi, 2*pi);
 	#print line
 	theta = math.fmod( math.atan2(line[3],line[2]) + 2 * math.pi, 2 * math.pi)
 	return theta
 
 def numPoly(data):
+	"""returns number of polygons in data"""
 	index = np.nonzero(np.isnan(data)) #find(np.isnan(data)==True)
 	n = len(index[0])/2
 	return n 
 
 def getPoly(data, n):
+	"""extracts nth polygon boundaries from data"""
 	# this function returns polygon n stored in data
 	index = np.nonzero(np.isnan(data)) #find(np.isnan(data)==True)
 	nop = len(index[0])/2
 
 	if n == 1:
 		poly = data[0:index[0][0],:]
 	elif n <= nop and n > 0:
 		poly = data[index[0][2*n-3]+1:index[0][2*n-2],:]
 	else:
 		print("Oops!  the data file has only %d polygons and there is no polygon with number %d!" %(nop,n))
 		poly = []
 
 	return poly
+
 def intersectLines(line1, line2):
 	#INTERSECTLINES return all intersection points of N lines in 2D
 	x1 =  line1[0]
 	y1 =  line1[1]
 	dx1 = line1[2]
 	dy1 = line1[3]
 
@@ -221,15 +205,15 @@
 				cross = not cross
 		i += 1
 
 	if sum(poly[-1, :] == poly[0,:]) != 2:
 		poly = np.vstack((poly, poly[0,:]))
 	return poly
 
-def rmGabs(poly, width, N):
+def rmGaps(poly, width, N):
 	#remove any crossovers up to N=5
 	# generate xPolygon
 	if sum(poly[-1, :] == poly[0,:]) != 2:
 		xpoly = np.vstack((poly, poly[0:,:]))
 	else:
 		xpoly = np.vstack((poly, poly[1:,:]))
 
@@ -253,15 +237,15 @@
 				if (intersectPointOnLine(p, p1, p2) and gab1 > width) | \
 				   (intersectPointOnLine(p, p3, p4) and gab2 > width):
 					#print "a gab is discovered: ", gab1, gab2
 					#if there is a gab
 					poly_new = np.delete(poly, list(range(i+1,i+N)), axis = 0)  #range(i+1,i+N-1)
 					poly = poly_new
 					poly = np.vstack((poly[0:i,:], p, poly[i+N:,:]))
-					poly = rmGabs(poly, width, N)
+					poly = rmGaps(poly, width, N)
 					cross = not cross
 		i += 1
 	if sum(poly[-1, :] == poly[0,:]) != 2:
 		poly = np.vstack((poly, poly[0,:]))
 	return poly
 
 def intersectPointOnLine(p, p1, p2):
```

### Comparing `covplan-0.1.0/src/covplan.egg-info/PKG-INFO` & `covplan-0.2.0/src/covplan.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: covplan
-Version: 0.1.0
+Version: 0.2.0
 Summary: A package to generate a guidance trajectory for complete 2D coverage of a region of interest
 Author-email: "Sanjeev Kumar R. S." <sanjeev.k.r.sudha@ntnu.no>, "Ibrahim A. Hameed" <ibib@ntnu.no>
 Project-URL: Homepage, https://github.com/sanjeevrs2000/cpp
 Project-URL: Bug Tracker, https://github.com/sanjeevrs2000/cpp/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -15,52 +15,71 @@
 Requires-Dist: scipy>=1.10
 Requires-Dist: scikit-learn>=1.2.0
 Requires-Dist: wheel
 Requires-Dist: utm
 Requires-Dist: folium
 Requires-Dist: python-tsp>=0.3
 
-# Complete coverage Path Planning (CCPP)
+# CovPlan
 
-[![PyPI](https://img.shields.io/pypi/v/cc_pathplanner?color=blue&label=pypi)](https://pypi.org/project/cc-pathplanner/0.1.0/)
-[![PyPi license](https://img.shields.io/pypi/l/ansicolortags.svg)](https://pypi.org/project/cc-pathplanner/0.1.0/)
+A Python package for coverage path planning
 
+[![PyPI](https://img.shields.io/pypi/v/covplan?color=blue&label=pypi)](https://pypi.org/project/covplan/0.2.0/)
+[![PyPi license](https://img.shields.io/pypi/l/ansicolortags.svg)](https://pypi.org/project/covplan/0.2.0/)
 
-## Getting started
-This repository contains a program which generates a guidance trajectory for complete 2D coverage. It can be used for operations where complete coverage of an Area of Interest (AoI) is required for various applications.
-The package can be installed from PyPi by running 'pip install covplan'
+This repository can be used for generating guidance trajectories for complete field coverage. It can be used for operations where complete coverage of an Area of Interest (AoI) is required for various applications. It is an updated Python implementation of the method that was presented in [this paper](https://journals.sagepub.com/doi/full/10.5772/56248).
+> Hameed IA, Bochtis D, Sørensen CA. An Optimized Field Coverage Planning Approach for Navigation of Agricultural Robots in Fields Involving Obstacle Areas. International Journal of Advanced Robotic Systems. 2013;10(5). doi:10.5772/56248
+
+
+## Installation
+
+The package can be installed using pip 
 
+```shell
+pip install covplan
+```
+
+## Getting started
 
-## How to use the program
-To use the program, run `coverage_path_planner.covplan(input_file, params)`. It returns a list of coordinates that compose a path for complete coverage.
+To generate a guidance trajectory for full coverage, use the API `covplan.pathplan(input_file, params)`. It returns a list of coordinates that compose a path for complete coverage.
 In the input file, describe the boundaries of the AoI using its lat-lon coordinates in the following format:  
 ```
   lat1  lon1
   lat2  lon2
   ...
   lat1  lon1
   NaN  NaN
 ```
 Ensure that the AoI is a closed polygon, by keeping the first coordinate the same as the last coordinate. Separate different polygons by including a `NaN NaN` at the end. Also ensure that the coordinates of the polygon are described clockwise, and counter-clockwise for any obstacles and forbidden regions.
-`coverage_path_planner.find_min(input_file, params)` runs a single objective optimizer to find the driving angle that minimizes the trajectory length for a given AoI and the specified parameters.
+`covplan.find_min(input_file, params)` runs a single objective optimizer to find the driving angle that minimizes the trajectory length for a given AoI and the specified parameters.
 
-## Example usage
+### Example usage
 ```python
-from covplan import coverage_path_planner
+from covplan import pathplan
 
 def main():
 	n_clusters=4	#number of sections
 	r=2	#radius for Dubins curves
 	input_file='sample_area.txt' #location of the input file containing coordinates of the field
 	width = 10	#distance between tracks
 	driving_angle=90	#angle wrt X-axis in degrees
 	no_hd=0	#number of margins around boundary (each with distance=0.5*width) if needed, otherwise 0
 	
-	op=coverage_path_planner.covplan(input_file,num_hd=no_hd,width=width,theta=driving_angle,num_clusters=n_clusters,radius=r,visualize=False) # returns list of waypoint coordinates composing full trajectory for coverage
+	op=pathplan(input_file,num_hd=no_hd,width=width,theta=driving_angle,num_clusters=n_clusters,radius=r,visualize=False) # returns list of waypoint coordinates composing full trajectory for coverage
 	print('The trajectory for full coverage consists of the following waypoints:',op)
 	
-	min=coverage_path_planner.find_min(input_file,width=width,num_hd=no_hd,num_clusters=n_clusters,radius=r,verbose=True)  # runs optimizer and returns angle corresponding to minimum path length
-	# print('Angle for trajectory with minimum length:', min)
 
 if __name__ == '__main__':
 	main()
 ```
+
+## Documentation
+
+The full documentation can be found [here](https://covplan.readthedocs.io/).
+
+## Contributing
+
+Contributions are always welcome!
+
+See [contributing.md](/contributing.md) for ways to get started.
+
+Please adhere to this project's [code of conduct](/contributing.md#code-of-conduct)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `covplan-0.1.0/tests/test_main.py` & `covplan-0.2.0/tests/test_main.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-from covplan import coverage_path_planner
+from covplan import pathplan, find_min
 
 def main():
 	n_clusters=4	#number of sections
 	r=2	#radius for Dubins curves
 	input_file='sample_area.txt' #location of the input file containing coordinates of the field
 	width = 10	#distance between tracks
 	driving_angle=90	#angle wrt X-axis in degrees
 	no_hd=0	#number of margins around boundary (each with distance=0.5*width) if needed, otherwise 0
 	
-	op=coverage_path_planner.covplan(input_file,num_hd=no_hd,width=width,theta=driving_angle,num_clusters=n_clusters,radius=r,visualize=False) # returns list of waypoint coordinates composing trajectory
+	op=pathplan(input_file,num_hd=no_hd,width=width,theta=driving_angle,num_clusters=n_clusters,radius=r,visualize=False) # returns list of waypoint coordinates composing trajectory
 	print('The trajectory for full coverage consists of the following waypoints:',op)
 	
-	min=coverage_path_planner.find_min(input_file,width=width,num_hd=no_hd,num_clusters=n_clusters,radius=r)  # runs optimizer and returns angle corresponding to minimum path length
+	min=find_min(input_file,width=width,num_hd=no_hd,num_clusters=n_clusters,radius=r)  # runs optimizer and returns angle corresponding to minimum path length
 	print('Angle for trajectory with minimum length:', min)
 
 if __name__ == '__main__':
 	main()
```

