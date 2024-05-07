# Comparing `tmp/dynamic_graphs_with_pygame-1.0.9.tar.gz` & `tmp/dynamic_graphs_with_pygame-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dynamic_graphs_with_pygame-1.0.9.tar", last modified: Mon Apr  1 11:41:59 2024, max compression
+gzip compressed data, was "dynamic_graphs_with_pygame-1.1.0.tar", last modified: Tue May  7 05:02:40 2024, max compression
```

## Comparing `dynamic_graphs_with_pygame-1.0.9.tar` & `dynamic_graphs_with_pygame-1.1.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0 linuxchrisbotos  (1000) linuxchrisbotos  (1000)        0 2024-04-01 11:41:59.647888 dynamic_graphs_with_pygame-1.0.9/
--rwxrwxrwx   0 linuxchrisbotos  (1000) linuxchrisbotos  (1000)     1092 2024-03-27 15:32:27.000000 dynamic_graphs_with_pygame-1.0.9/LICENSE
--rwxrwxrwx   0 linuxchrisbotos  (1000) linuxchrisbotos  (1000)     4092 2024-04-01 11:41:59.646890 dynamic_graphs_with_pygame-1.0.9/PKG-INFO
--rwxrwxrwx   0 linuxchrisbotos  (1000) linuxchrisbotos  (1000)     3545 2024-03-28 10:16:11.000000 dynamic_graphs_with_pygame-1.0.9/README.md
-drwxrwxrwx   0 linuxchrisbotos  (1000) linuxchrisbotos  (1000)        0 2024-04-01 11:41:59.587889 dynamic_graphs_with_pygame-1.0.9/dynamic_graphs_with_pygame/
--rwxrwxrwx   0 linuxchrisbotos  (1000) linuxchrisbotos  (1000)       81 2024-03-29 14:04:41.000000 dynamic_graphs_with_pygame-1.0.9/dynamic_graphs_with_pygame/__init__.py
--rwxrwxrwx   0 linuxchrisbotos  (1000) linuxchrisbotos  (1000)    27822 2024-04-01 11:40:25.000000 dynamic_graphs_with_pygame-1.0.9/dynamic_graphs_with_pygame/dyn_graphs.py
-drwxrwxrwx   0 linuxchrisbotos  (1000) linuxchrisbotos  (1000)        0 2024-04-01 11:41:59.635889 dynamic_graphs_with_pygame-1.0.9/dynamic_graphs_with_pygame.egg-info/
--rwxrwxrwx   0 linuxchrisbotos  (1000) linuxchrisbotos  (1000)     4092 2024-04-01 11:41:59.000000 dynamic_graphs_with_pygame-1.0.9/dynamic_graphs_with_pygame.egg-info/PKG-INFO
--rwxrwxrwx   0 linuxchrisbotos  (1000) linuxchrisbotos  (1000)      355 2024-04-01 11:41:59.000000 dynamic_graphs_with_pygame-1.0.9/dynamic_graphs_with_pygame.egg-info/SOURCES.txt
--rwxrwxrwx   0 linuxchrisbotos  (1000) linuxchrisbotos  (1000)        1 2024-04-01 11:41:59.000000 dynamic_graphs_with_pygame-1.0.9/dynamic_graphs_with_pygame.egg-info/dependency_links.txt
--rwxrwxrwx   0 linuxchrisbotos  (1000) linuxchrisbotos  (1000)       13 2024-04-01 11:41:59.000000 dynamic_graphs_with_pygame-1.0.9/dynamic_graphs_with_pygame.egg-info/requires.txt
--rwxrwxrwx   0 linuxchrisbotos  (1000) linuxchrisbotos  (1000)       27 2024-04-01 11:41:59.000000 dynamic_graphs_with_pygame-1.0.9/dynamic_graphs_with_pygame.egg-info/top_level.txt
--rwxrwxrwx   0 linuxchrisbotos  (1000) linuxchrisbotos  (1000)       38 2024-04-01 11:41:59.648889 dynamic_graphs_with_pygame-1.0.9/setup.cfg
--rwxrwxrwx   0 linuxchrisbotos  (1000) linuxchrisbotos  (1000)      992 2024-04-01 11:41:19.000000 dynamic_graphs_with_pygame-1.0.9/setup.py
+drwxrwxrwx   0 linuxchrisbotos  (1000) linuxchrisbotos  (1000)        0 2024-05-07 05:02:40.818873 dynamic_graphs_with_pygame-1.1.0/
+-rwxrwxrwx   0 linuxchrisbotos  (1000) linuxchrisbotos  (1000)     1092 2024-03-27 15:32:27.000000 dynamic_graphs_with_pygame-1.1.0/LICENSE
+-rwxrwxrwx   0 linuxchrisbotos  (1000) linuxchrisbotos  (1000)     4092 2024-05-07 05:02:40.816242 dynamic_graphs_with_pygame-1.1.0/PKG-INFO
+-rwxrwxrwx   0 linuxchrisbotos  (1000) linuxchrisbotos  (1000)     3545 2024-03-28 10:16:11.000000 dynamic_graphs_with_pygame-1.1.0/README.md
+drwxrwxrwx   0 linuxchrisbotos  (1000) linuxchrisbotos  (1000)        0 2024-05-07 05:02:40.723943 dynamic_graphs_with_pygame-1.1.0/dynamic_graphs_with_pygame/
+-rwxrwxrwx   0 linuxchrisbotos  (1000) linuxchrisbotos  (1000)       81 2024-03-29 14:04:41.000000 dynamic_graphs_with_pygame-1.1.0/dynamic_graphs_with_pygame/__init__.py
+-rwxrwxrwx   0 linuxchrisbotos  (1000) linuxchrisbotos  (1000)    28176 2024-05-07 04:58:39.000000 dynamic_graphs_with_pygame-1.1.0/dynamic_graphs_with_pygame/dyn_graphs.py
+drwxrwxrwx   0 linuxchrisbotos  (1000) linuxchrisbotos  (1000)        0 2024-05-07 05:02:40.798886 dynamic_graphs_with_pygame-1.1.0/dynamic_graphs_with_pygame.egg-info/
+-rwxrwxrwx   0 linuxchrisbotos  (1000) linuxchrisbotos  (1000)     4092 2024-05-07 05:02:40.000000 dynamic_graphs_with_pygame-1.1.0/dynamic_graphs_with_pygame.egg-info/PKG-INFO
+-rwxrwxrwx   0 linuxchrisbotos  (1000) linuxchrisbotos  (1000)      355 2024-05-07 05:02:40.000000 dynamic_graphs_with_pygame-1.1.0/dynamic_graphs_with_pygame.egg-info/SOURCES.txt
+-rwxrwxrwx   0 linuxchrisbotos  (1000) linuxchrisbotos  (1000)        1 2024-05-07 05:02:40.000000 dynamic_graphs_with_pygame-1.1.0/dynamic_graphs_with_pygame.egg-info/dependency_links.txt
+-rwxrwxrwx   0 linuxchrisbotos  (1000) linuxchrisbotos  (1000)       13 2024-05-07 05:02:40.000000 dynamic_graphs_with_pygame-1.1.0/dynamic_graphs_with_pygame.egg-info/requires.txt
+-rwxrwxrwx   0 linuxchrisbotos  (1000) linuxchrisbotos  (1000)       27 2024-05-07 05:02:40.000000 dynamic_graphs_with_pygame-1.1.0/dynamic_graphs_with_pygame.egg-info/top_level.txt
+-rwxrwxrwx   0 linuxchrisbotos  (1000) linuxchrisbotos  (1000)       38 2024-05-07 05:02:40.818873 dynamic_graphs_with_pygame-1.1.0/setup.cfg
+-rwxrwxrwx   0 linuxchrisbotos  (1000) linuxchrisbotos  (1000)      992 2024-05-07 04:58:39.000000 dynamic_graphs_with_pygame-1.1.0/setup.py
```

### Comparing `dynamic_graphs_with_pygame-1.0.9/LICENSE` & `dynamic_graphs_with_pygame-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dynamic_graphs_with_pygame-1.0.9/PKG-INFO` & `dynamic_graphs_with_pygame-1.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dynamic_graphs_with_pygame
-Version: 1.0.9
+Version: 1.1.0
 Summary: A class for drawing dynamic graphs using Pygame.
 Home-page: https://github.com/ChrisBotos/Dynamic_Graphs_with_Pygame
 Author: Christos Botos
 Author-email: hcty02@gmail.com
 License: UNKNOWN
 Project-URL: LinkedIn, https://www.linkedin.com/in/your_username/
 Keywords: pygame graphs dynamic visualization
```

### Comparing `dynamic_graphs_with_pygame-1.0.9/README.md` & `dynamic_graphs_with_pygame-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `dynamic_graphs_with_pygame-1.0.9/dynamic_graphs_with_pygame/dyn_graphs.py` & `dynamic_graphs_with_pygame-1.1.0/dynamic_graphs_with_pygame/dyn_graphs.py`

 * *Files 1% similar despite different names*

```diff
@@ -170,18 +170,26 @@
 
 
         """Draw the rects for the bins"""
         counter = 0
         for bin_value in bin_array:
 
             if bin_value != 0:
-                bar_coordinates = (self.x + counter * graph_bin_size,
-                                   self.y + graph_y - bin_value * y_amplifier,
-                                   graph_bin_size,
-                                   bin_value * abs(y_amplifier))
+                bar_height = int(bin_value * y_amplifier)
+
+                if bar_height > 0:
+                    bar_coordinates = (self.x + counter * graph_bin_size,
+                                       self.y + graph_y - bar_height,
+                                       graph_bin_size,
+                                       bar_height)
+                else:
+                    bar_coordinates = (self.x + counter * graph_bin_size,
+                                       self.y + graph_y,
+                                       graph_bin_size,
+                                       np.abs(bar_height))
 
                 # I use semi_transparency in case we want to show one graph behind the other.
                 # This function draws objects in pygame that can also be transparent.
                 draw_rect_alpha(self.screen,
                                 bar_color,
                                 bar_coordinates)
```

### Comparing `dynamic_graphs_with_pygame-1.0.9/dynamic_graphs_with_pygame.egg-info/PKG-INFO` & `dynamic_graphs_with_pygame-1.1.0/dynamic_graphs_with_pygame.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dynamic-graphs-with-pygame
-Version: 1.0.9
+Version: 1.1.0
 Summary: A class for drawing dynamic graphs using Pygame.
 Home-page: https://github.com/ChrisBotos/Dynamic_Graphs_with_Pygame
 Author: Christos Botos
 Author-email: hcty02@gmail.com
 License: UNKNOWN
 Project-URL: LinkedIn, https://www.linkedin.com/in/your_username/
 Keywords: pygame graphs dynamic visualization
```

### Comparing `dynamic_graphs_with_pygame-1.0.9/setup.py` & `dynamic_graphs_with_pygame-1.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="dynamic_graphs_with_pygame",
-    version="1.0.9",
+    version="1.1.0",
     description="A class for drawing dynamic graphs using Pygame.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Christos Botos",
     author_email="hcty02@gmail.com",
     url="https://github.com/ChrisBotos/Dynamic_Graphs_with_Pygame",
     packages=find_packages(),  # Use find_packages to automatically discover packages
```

