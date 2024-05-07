# Comparing `tmp/scenebuilder-0.1.4.tar.gz` & `tmp/scenebuilder-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scenebuilder-0.1.4.tar", max compression
+gzip compressed data, was "scenebuilder-0.1.5.tar", max compression
```

## Comparing `scenebuilder-0.1.4.tar` & `scenebuilder-0.1.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0    11357 2023-10-19 10:53:34.751175 scenebuilder-0.1.4/LICENSE
--rw-r--r--   0        0        0     3665 2024-05-06 09:27:57.007567 scenebuilder-0.1.4/README.md
--rw-r--r--   0        0        0      486 2024-05-06 09:29:22.928854 scenebuilder-0.1.4/pyproject.toml
--rw-r--r--   0        0        0       39 2024-05-06 09:11:58.678352 scenebuilder-0.1.4/scenebuilder/__init__.py
--rw-r--r--   0        0        0      851 2024-05-06 09:09:11.273082 scenebuilder-0.1.4/scenebuilder/actions_stack.py
--rw-r--r--   0        0        0     4206 2024-05-06 09:09:05.634947 scenebuilder-0.1.4/scenebuilder/construction.py
--rw-r--r--   0        0        0     4909 2024-05-05 23:20:22.042742 scenebuilder-0.1.4/scenebuilder/entities.py
--rw-r--r--   0        0        0      601 2024-05-06 09:05:40.973167 scenebuilder-0.1.4/scenebuilder/main.py
--rw-r--r--   0        0        0      454 2024-05-05 23:20:17.691922 scenebuilder-0.1.4/scenebuilder/mixins.py
--rw-r--r--   0        0        0     2194 2024-05-06 09:08:29.586634 scenebuilder-0.1.4/scenebuilder/observer_utils.py
--rw-r--r--   0        0        0     4329 2024-05-06 09:08:22.356210 scenebuilder-0.1.4/scenebuilder/patches.py
--rw-r--r--   0        0        0    20347 2024-05-06 09:08:16.420109 scenebuilder-0.1.4/scenebuilder/scenebuilder.py
--rw-r--r--   0        0        0     1698 2024-05-06 09:11:58.711638 scenebuilder-0.1.4/scenebuilder/ui_components.py
--rw-r--r--   0        0        0     3763 2024-05-06 09:11:58.729421 scenebuilder-0.1.4/scenebuilder/utils.py
--rw-r--r--   0        0        0     4194 1970-01-01 00:00:00.000000 scenebuilder-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-10-19 10:53:34.751175 scenebuilder-0.1.5/LICENSE
+-rw-r--r--   0        0        0     3771 2024-05-07 15:17:47.657485 scenebuilder-0.1.5/README.md
+-rw-r--r--   0        0        0      486 2024-05-07 15:18:28.059816 scenebuilder-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0       39 2024-05-06 09:11:58.678352 scenebuilder-0.1.5/scenebuilder/__init__.py
+-rw-r--r--   0        0        0     1020 2024-05-07 09:01:36.601969 scenebuilder-0.1.5/scenebuilder/actions_stack.py
+-rw-r--r--   0        0        0     4951 2024-05-07 08:15:28.842583 scenebuilder-0.1.5/scenebuilder/entities.py
+-rw-r--r--   0        0        0      604 2024-05-07 05:46:06.554704 scenebuilder-0.1.5/scenebuilder/main.py
+-rw-r--r--   0        0        0      454 2024-05-05 23:20:17.691922 scenebuilder-0.1.5/scenebuilder/mixins.py
+-rw-r--r--   0        0        0     2196 2024-05-07 10:52:47.060418 scenebuilder-0.1.5/scenebuilder/observer_utils.py
+-rw-r--r--   0        0        0     4211 2024-05-07 06:08:47.691838 scenebuilder-0.1.5/scenebuilder/patch_manager.py
+-rw-r--r--   0        0        0     4334 2024-05-07 05:25:24.471252 scenebuilder-0.1.5/scenebuilder/patches.py
+-rw-r--r--   0        0        0    23610 2024-05-07 13:49:30.666638 scenebuilder-0.1.5/scenebuilder/scenebuilder.py
+-rw-r--r--   0        0        0     4060 2024-05-07 14:23:30.282485 scenebuilder-0.1.5/scenebuilder/ui_components.py
+-rw-r--r--   0        0        0     4254 2024-05-07 08:21:02.590859 scenebuilder-0.1.5/scenebuilder/utils.py
+-rw-r--r--   0        0        0     4300 1970-01-01 00:00:00.000000 scenebuilder-0.1.5/PKG-INFO
```

### Comparing `scenebuilder-0.1.4/LICENSE` & `scenebuilder-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `scenebuilder-0.1.4/README.md` & `scenebuilder-0.1.5/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -18,23 +18,36 @@
 pip install scenebuilder
 ```
 
 This command installs SceneBuilder along with numpy and matplotlib, ensuring that everything needed to run the GUI is properly set up.
 
 
 
-## Getting Started
 
-### Prerequisites
+## Prerequisites
 
 SceneBuilder's prerequisites are defined in the pyproject.toml file and include Matplotlib and numpy.
 
-### Quick Start Guide
+## Quick Start Guide
 
-To start using SceneBuilder, you need to create an instance of the `SceneBuilder` class and invoke the `draw_scene()` method. Below is a simple example to get you started:
+### Using Command-Line Options
+
+You can use SceneBuilder directly from the command line with the following options:
+
+- `-o`, `--output`: Specify the path where the scene should be saved as a JSON file.
+- `-l`, `--load`: Specify a JSON file path to load an existing scene.
+
+Example usage:
+
+```bash
+scenebuilder --load path/to/scene.json --output path/to/output.json
+```
+
+### In Code
+To use SceneBuilder in code, you need to create an instance of the `SceneBuilder` class and invoke the `draw_scene()` method. Below is a simple example to get you started:
 
 ```python
 from scenebuilder import SceneBuilder
 
 # Create an instance of the SceneBuilder
 scene = SceneBuilder()
 
@@ -52,34 +65,24 @@
 Specify the path to save your output json to:
 
 ```python
 scene.set_output_path("path/to/output.json")
 scene.draw_scene()
 ```
 
-### Using Command-Line Options
-
-You can also use SceneBuilder directly from the command line with the following options:
-
-- `-o`, `--output`: Specify the path where the scene should be saved as a JSON file.
-- `-l`, `--load`: Specify a JSON file path to load an existing scene.
 
-Example usage:
-
-```bash
-scenebuilder --load path/to/scene.json --output path/to/output.json
-```
 
 ## Features
 
 - **Draw Obstacles**: Click within the GUI to place vertices of polygons that represent obstacles. Press Tab to complete an obstacle.
 - **Add new obstacle vertices**: To add new vertices, click somewhere on the polygon's perimeter and drag to move the vertex to its desired location.
 - **Set Drone Paths**: Click once to place the starting point, and again to place the goal of an agent/drone. An arrow will automatically be drawn from start to goal.
 - **Move or adjust existing obstacles/drones**: Obstacles and drones can be moved by clicking and dragging. Drone start and goal points, as well as existing obstacle vertices can be moved in the same way.
 - **Switch between Obstacle and Drone Modes**: Press b to switch to building/obstacle mode. Press d to switch to drone/agent mode. Alternatively click the Switch button on the bottom left of the gui.
+- **Delete obstacles**: Select the obstacle and press delete or backspace. NOTE this is not yet available for drones.
 - **Remove unwanted points**: To remove unwanted points (either obstacle vertices or a drone start point), press escape.
 - **Undo drone/obstacle placement**: To remove the last obstacle or drone, press ctrl+z.
 - **Reset Scene**: To reset the scene to a blank canvas, click the Reset button in the gui.
 
 ## Saving Scenes
 
 Once you have created a scene, you can save it to a JSON file by clicking the 'Create JSON' button in the GUI. This file can then be used as input for path planning algorithms that require predefined scenes with obstacles and paths.
```

### Comparing `scenebuilder-0.1.4/scenebuilder/construction.py` & `scenebuilder-0.1.5/scenebuilder/patch_manager.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 
 from matplotlib.lines import Line2D
 from typing import List
 import numpy as np
 from .entities import Obstacle, Drone
 from .patches import ObstaclePatch, DronePatch, Marker
 
-
 class PatchManager:
     def __init__(self, ax: plt.Axes):
         self.ax = ax
         self.building_patches: dict[Obstacle, ObstaclePatch] = {}
         self.drone_patches: dict[Drone, DronePatch] = {}
         # self.temp_drone_starts:list[Line2D] = []
         self.current_building_vertices: list[Line2D] = []
@@ -29,15 +28,15 @@
         self.building_patches[building] = patch
 
     def add_building_vertex(self, vertex: tuple) -> None:
         point = Marker(vertex, "go").create_marker()
         self.current_building_vertices.append(point)
 
     def get_building_patch(self, building: Obstacle) -> ObstaclePatch:
-        """Obtains the patch for the building passed as argument
+        """Obtains the paftch for the building passed as argument
         and returns it. If the patch doesn't exist, returns KeyError.
         """
         return self.building_patches[building]
 
     def get_building_from_patch(self, patch: ObstaclePatch) -> Obstacle:
         """Obtains the building from the patch passed as argument"""
         for building, building_patch in self.building_patches.items():
@@ -105,7 +104,9 @@
         for patch in self.building_patches.values():
             patch.remove()
         for patch in self.drone_patches.values():
             patch.remove()
         self.remove_temp_drone_start()
         self.building_patches.clear()
         self.drone_patches.clear()
+
+
```

### Comparing `scenebuilder-0.1.4/scenebuilder/entities.py` & `scenebuilder-0.1.5/scenebuilder/entities.py`

 * *Files 1% similar despite different names*

```diff
@@ -69,15 +69,16 @@
 
 
 class Obstacle(Entity):
     """Class containing all necessary information about a Building Entity, not including its graphics"""
 
     def __init__(self, vertices: ArrayLike):
         super().__init__(ID="building", position=None)
-        self.vertices = self.sort_vertices(vertices[:, :2])
+        # self.vertices = self.sort_vertices(vertices[:, :2])
+        self.vertices = vertices[:, :2]
 
     def sort_vertices(self, vertices):
         """Sorts the vertices by angle around the centre of mass of the polygon"""
         Xavg = np.mean(vertices[:, 0:1])
         Yavg = np.mean(vertices[:, 1:2])
         angles = np.arctan2(
             (Yavg * np.ones(len(vertices[:, 1])) - vertices[:, 1]),
```

### Comparing `scenebuilder-0.1.4/scenebuilder/main.py` & `scenebuilder-0.1.5/scenebuilder/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,12 +11,12 @@
     app = SceneBuilder()
 
     if args.load:
         app.load_scene(args.load)
 
     if args.output:
         app.set_output_path(args.output)
- 
+    
     app.draw_scene()
 
 if __name__ == "__main__":
     main()
```

### Comparing `scenebuilder-0.1.4/scenebuilder/observer_utils.py` & `scenebuilder-0.1.5/scenebuilder/observer_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     The `abstractmethod` decorator is used to declare methods that have to be
     overridden by concrete subclasses. This enforces the implementation of
     these methods in each subclass, ensuring that they adhere to the defined
     interface.
     """
 
     @abstractmethod
-    def call(self, event: str, *args, **kwargs):
+    def _call(self, event: str, *args, **kwargs):
         """
         Abstract method that must be implemented by concrete subclasses.
 
         This method is called when the subject (Observable) to which the
         observer is attached, triggers an event. The subclass should implement
         the logic for handling these events here.
 
@@ -52,8 +52,8 @@
         self._observers.append(observer)
 
     def remove_observer(self, observer: Observer):
         self._observers.remove(observer)
 
     def notify_observers(self, event: str, *args, **kwargs):
         for observer in self._observers:
-            observer.call(event, *args, **kwargs)
+            observer._call(event, *args, **kwargs)
```

### Comparing `scenebuilder-0.1.4/scenebuilder/patches.py` & `scenebuilder-0.1.5/scenebuilder/patches.py`

 * *Files 1% similar despite different names*

```diff
@@ -103,15 +103,15 @@
         self.marker_end.update_position(self.drone.goal[:2])
         self.arrow.update_arrow_position(self.drone.position[:2], self.drone.goal[:2])
 
 
 class ObstaclePatch(Polygon):
     """
     Example usage:
-    patch = BuildingPatch(building_instance, facecolor='blue', edgecolor='red', linewidth=2.0)
+    patch = BuildingPatch(ax, building_instance, facecolor='blue', edgecolor='red', linewidth=2.0)
     """
 
     def __init__(self, building: Obstacle, **kwargs) -> None:
         super().__init__(building.vertices, **kwargs)
         self.vertices = self.get_xy()
         # Storing original colors
         self.original_facecolor = self.get_facecolor()
@@ -128,7 +128,8 @@
         """Revert appearance to the original state."""
         self.set_facecolor(self.original_facecolor)
         self.set_edgecolor(self.original_edgecolor)
 
     def update_visual(self):
         """Update the visual representation based on the building state."""
         self.set_xy(self.building.vertices)
+
```

### Comparing `scenebuilder-0.1.4/scenebuilder/scenebuilder.py` & `scenebuilder-0.1.5/scenebuilder/scenebuilder.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,98 +1,154 @@
 from __future__ import annotations
 
 import matplotlib.pyplot as plt
-import matplotlib.patches as mpatches
 
 import numpy as np
 
 from .entities import Drone, Obstacle
 from .utils import distance_between_points, create_json, get_from_json
 from .utils import load_from_json, validate_json_path
-from .construction import PatchManager
+from .patch_manager import PatchManager
 from .actions_stack import ActionsStack
 from .ui_components import UIComponents
 from .observer_utils import Observer, Observable
 from threading import Timer
-
+from pathlib import Path
+import traceback
+import os
 
 class SceneBuilder(Observer, Observable):
 
     CLICK_THRESHOLD = 0.14
-    FIG_SIZE = (8, 8)
+    FIG_SIZE = (8, 8.5)
     AXIS_LIMITS = (-5, 5)
 
     def __init__(self):
         # initialise Observable (Observer has no init)
         super().__init__()
         self._selected_building: Obstacle = None
         self.original_colors: dict = {}
         # Setup the default plot
-        self.plot_setup()
+        self._plot_setup()
         # Define variables
-        self.setup_data()
+        self._setup_data()
+        
         # Connect event handlers
-        self.connect_event_handlers()
+        self._connect_event_handlers()
+
+    def set_output_path(self, path: str, exit = False, skip_check = False) -> None:
+        '''Set output path to validated path. call sys.exit() if exit is True and path is invalid'''
+        try:
+            if not skip_check:
+                # Validate the path if not skipping
+                response = validate_json_path(path, exit)
+                result = response['result']
+                #if path invalid, don't set
+                if result == 0:
+                    return
+        finally:
+            # This block runs whether validation was skipped, passed, or failed.
+            self.output_path = path
+            self.ui_components.modify_current_file_text(self.output_path)
+            self._show_warning(f'Set new output path\n{path}', 3, color='g')
+
+    def load_scene(self, path: str) -> None:
+        """Populates the scene with the obstacles and drones in the specified json
+        path: path to compatible json file"""
+        self._reset()
+        case_info = load_from_json(path)
+        drones, buildings = get_from_json(case_info)
+        self.drones = drones
+        self.buildings = buildings
+        for building in self.buildings:
+            self.patch_manager.add_building_patch(building)
+        for drone in self.drones:
+            self.patch_manager.add_drone_patch(drone)
+        self._update()
+
+    def draw_scene(self):
+        """Draw the scene."""
+        plt.show()
+
+    def _plot_setup(self):
+        fig = plt.figure(figsize=self.FIG_SIZE)
+        ax = fig.add_subplot(111)
+
+        fig.subplots_adjust(bottom=0.05, top=0.9)
+
+        ax.set_xlim(self.AXIS_LIMITS)
+        ax.set_ylim(self.AXIS_LIMITS)
+        ax.set_box_aspect(1)
+        ax.grid(color="k", linestyle="-", linewidth=0.5, which="major")
+        ax.grid(color="k", linestyle=":", linewidth=0.5, which="minor")
+        # ax.grid(True)
+        ax.minorticks_on()
+
+        # Add instructions
+        instructions = (
+            "Instructions:\n"
+            "'b': switch to building mode, click to place vertices of building\n"
+            "Tab: complete a building, \n"
+            "'d': switch to drone mode. "
+            "'esc': clear unwanted points."
+        )
+
+        fig.text(
+            0.2,
+            0.91,
+            instructions,
+            fontsize=10,
+            bbox=dict(boxstyle="round", facecolor="wheat", alpha=0.5),
+        )
+        #modifiable/interactive ui elements are in ui_components.py
 
-    def setup_data(self) -> None:
-        # self.ui_components:UIComponents = UIComponents(self.ax)
+        
+        
+        self.fig, self.ax = fig, ax
+
+        return None
+    
+    def _setup_data(self) -> None:
+        '''define additional attributes'''
         self.ui_components = UIComponents(self.ax)
         self.ui_components.add_observer(self)
+
         # this line makes sure the current axes are the main ones
         plt.sca(self.ax)
 
         self.patch_manager = PatchManager(self.ax)
         self.output_path = "scenebuilder.json"
+        
+        self.timer:Timer|None = None
 
         self.drones: list[Drone] = []
         self.buildings: list[Obstacle] = []
         self.current_drone = None
         self.mode = "building"  # 'building', 'drone', or None
         self.actions_stack = ActionsStack()  # New line to track the actions
 
-        self.selected_drone: Drone = None
+        self.selected_drone: Drone|None = None
         self.initial_click_position = None
         self.selected_vertex = None
         self.warning = self.ax.annotate(
             "WARNING, No Drones!",
             xy=(0.5, 0.5),
             xycoords="axes fraction",
             fontsize=12,
             fontweight="bold",
             color="red",
             ha="center",
+            bbox=dict(boxstyle="round", fc="w", ec="0.5", alpha=1),
+            wrap=True
         )
 
         self.warning.set_visible(False)  # Start with warning hidden
 
         return None
 
-    def set_output_path(self, path: str) -> None:
-        try:
-            validate_json_path(path)
-            self.output_path = path
-        except Exception as e:
-            print(f"Error: {e}")
-
-    def load_scene(self, path: str) -> None:
-        """Populates the scene with the obstacles and drones in the specified json
-        path: path to compatible json file"""
-        case_info = load_from_json(path)
-        drones, buildings = get_from_json(case_info)
-        self.drones = drones
-        self.buildings = buildings
-        for building in self.buildings:
-            self.patch_manager.add_building_patch(building)
-        for drone in self.drones:
-            self.patch_manager.add_drone_patch(drone)
-
-    def draw_scene(self):
-        """Draw the scene."""
-        plt.show()
-
     @property
     def selected_building(self):
         return self._selected_building
 
     @selected_building.setter
     def selected_building(self, new_building: Obstacle):
         """Highlight selected building in pink or deselect it if it is already selected.
@@ -105,31 +161,31 @@
                 self._selected_building
             )
             current_patch.deselect()
         if new_building:
             new_building_patch = self.patch_manager.get_building_patch(new_building)
             new_building_patch.select()
         self._selected_building = new_building
-        self.update()
+        self._update()
 
-    def hide_warning(self):
+    def _hide_warning(self):
         self.warning.set_visible(False)
-        self.update()
+        self._update()
 
-    def connect_event_handlers(self) -> None:
+    def _connect_event_handlers(self) -> None:
 
-        self.fig.canvas.mpl_connect("pick_event", self.on_pick)
-        self.fig.canvas.mpl_connect("button_press_event", self.on_click)
-        self.fig.canvas.mpl_connect("key_press_event", self.on_key_press)
-        self.fig.canvas.mpl_connect("button_release_event", self.on_button_release)
-        self.fig.canvas.mpl_connect("motion_notify_event", self.on_mouse_move)
+        self.fig.canvas.mpl_connect("pick_event", self._on_pick)
+        self.fig.canvas.mpl_connect("button_press_event", self._on_click)
+        self.fig.canvas.mpl_connect("key_press_event", self._on_key_press)
+        self.fig.canvas.mpl_connect("button_release_event", self._on_button_release)
+        self.fig.canvas.mpl_connect("motion_notify_event", self._on_mouse_move)
 
         return None
 
-    def handle_vertex_movement(self, event):
+    def _handle_vertex_movement(self, event):
         """Returns True if a click is near a vertex of an obstacle"""
         if not self.buildings:
             return False
 
         # Find the closest vertex
         closest_building, closest_vertex_index = self._get_closest_vertex(
             [event.xdata, event.ydata]
@@ -157,15 +213,15 @@
         )
 
         return min(
             all_vertices,
             key=lambda x: distance_between_points(x[0].vertices[x[1]][:2], point),
         )
 
-    def handle_drone_movement(self, event) -> bool:
+    def _handle_drone_movement(self, event) -> bool:
         # Check if a drone starting or ending point was clicked
         point = [event.xdata, event.ydata]
         for drone in self.drones:
             start_dist = distance_between_points(drone.position[:2], point)
             end_dist = distance_between_points(drone.goal[:2], point)
             if (
                 start_dist < self.CLICK_THRESHOLD
@@ -190,127 +246,126 @@
                 self.initial_click_position = point
                 return True
 
         self.selected_drone = None
         self.dragging_drone_point = None
         return False
 
-    def handle_building_placement(self, event) -> None:
+    def _handle_building_placement(self, event) -> None:
         self.selected_building = None
         if self.current_drone:
             self.patch_manager.remove_temp_drone_start()
             self.current_drone = None
         # Add a corner to the current building at the click location
         # plot the point in the patch manager
         self.patch_manager.add_building_vertex((event.xdata, event.ydata))
-        self.update()
+        self._update()
         return None
 
-    def handle_drone_placement(self, event) -> None:
+    def _handle_drone_placement(self, event) -> None:
         # clear any buildings before starting drones
         # Add a drone at the click location
         self.selected_building = None
         if self.current_drone is None:
             # initialise the drone
             # what to do when we draw the initial position of the drone
             # This is the initial position of the drone
             # clear all other temporary elements
             self.patch_manager.clear_building_vertices()
             self.current_drone = Drone(
                 ID=f"V{len(self.drones)}", position=None, goal=None
             )
             self.current_drone.position = np.array([event.xdata, event.ydata, 0.5])
             self.patch_manager.add_temp_drone_start(self.current_drone.position[:2])
-            self.update()
+            self._update()
         else:
             # drone initial position is already defined, now add the destination (goal)
             # This is the goal position of the drone
             self.current_drone.goal = np.array([event.xdata, event.ydata, 0.5])
 
             self.drones.append(self.current_drone)
             self.actions_stack.add_action("drone", self.current_drone)
             self.patch_manager.remove_temp_drone_start()
 
             # add drone patch to patch_manager
             self.patch_manager.add_drone_patch(self.current_drone)
             self.current_drone = None
-            self.update()
+            self._update()
         return None
 
-    def add_new_vertex(self, event) -> bool:
+    def _add_new_vertex(self, event) -> bool:
         for building in self.buildings:
             if building.insert_vertex((event.xdata, event.ydata)):
                 # Redraw the building if a vertex was added
                 self.patch_manager.redraw_building(building)
-                self.update()
+                self._update()
                 return True
         return False
 
-    def handle_deselect(self, event):
+    def _handle_deselect(self, event):
         if self.selected_building:
             if not self.selected_building.contains_point([event.xdata, event.ydata]):
                 self.selected_building = None
             return True
 
-    def on_click(self, event):
+    def _on_click(self, event):
         """
         This method is called when a click is detected on the plot.
         The event object contains information about the click, such as its position.
         You can use this information to add new elements to the plot, such as a new building or a new drone.
-        #TODO ORDER MATTERS, events will be handled in the order they are listed in this method"""
-
+        #NOTE ORDER MATTERS, events will be handled in the order they are listed in this method"""
         # If clicked outside of the plot, do nothing
         # if not event.xdata or not event.ydata:
         #     return
         if event.inaxes != self.ax:
             return
 
         # handle moving building vertices
-        if self.handle_vertex_movement(event):
+        if self._handle_vertex_movement(event):
             return
 
         # add a new vertex if near a building edge and allow moving it around with the mouse...
         # by calling the vertex movement handler again
-        if self.add_new_vertex(event):
-            self.handle_vertex_movement(event)
+        if self._add_new_vertex(event):
+            self._handle_vertex_movement(event)
             return
 
         # if a building is selected and we click outside of it, it is deselected (but nothing else happens)
-        if self.handle_deselect(event):
+        if self._handle_deselect(event):
             return
 
         # Check if a drone was clicked and handle its movement if necessary
-        if self.handle_drone_movement(event):
+        if self._handle_drone_movement(event):
             return
         # Check if a building was clicked and handle its movement if necessary
 
         # Proceed with building placement
         if self.mode == "building":
-            self.handle_building_placement(event)
+            self._handle_building_placement(event)
             return
 
         # Proceed with drone placement
         elif self.mode == "drone":
-            self.handle_drone_placement(event)
+            self._handle_drone_placement(event)
             return
 
         # Update the plot
-        self.update()
+        self._update()
 
-    def on_pick(self, event):
+    def _on_pick(self, event):
         # Check if the picked artist is a Polygon (optional but can be useful)
         if not isinstance(event.artist, plt.Polygon):
             return
         # polygon = event.artist
         building = self.patch_manager.get_building_from_patch(event.artist)
         self.selected_building = building
 
         self.initial_click_position = [event.mouseevent.xdata, event.mouseevent.ydata]
 
-    def on_mouse_move(self, event):
+    def _on_mouse_move(self, event):
 
         # check to make sure the mouse is still in the main axes
         # and not over a button or other axes object
         # or outside the axes altogether
         if event.inaxes != self.ax:
             return
 
@@ -319,30 +374,16 @@
         ##########################################################################################
         # move the vertex if one is selected
         if self.selected_building is not None and self.selected_vertex is not None:
             # # move the relevent vertex
             self.selected_building.move_vertex(self.selected_vertex, point)
             self.patch_manager.redraw_building(self.selected_building)
 
-            self.update()  # Redraw to show the moved vertex
-
-        ###########################################################################################
-        # move the whole building patch
-        elif self.selected_building and self.initial_click_position:
-            ds = np.array(point) - np.array(self.initial_click_position)
-            # Move the building
-            # set the vertices of the src.Building object, then copy them into the building patch
-            self.selected_building.move_building(ds)
-            self.patch_manager.redraw_building(self.selected_building)
-            # self.building_patches[self.selected_building].update_visual()
-            # Update the initial click position for next movement calculation
-            self.initial_click_position = point
+            self._update()  # Redraw to show the moved vertex
 
-            # Redraw to show the moved building
-            self.update()
         ###########################################################################################
         # Move the drone
         elif self.selected_drone:
             if self.dragging_drone_point == "start":
                 self.selected_drone.position = np.array([*point, 0.5])
 
             elif self.dragging_drone_point == "end":
@@ -353,76 +394,89 @@
 
                 self.selected_drone.move_whole_drone(ds)
 
             self.initial_click_position = point
             # This will redraw the drone starting or ending point in its new position
             self.patch_manager.redraw_drone(self.selected_drone)
 
-            self.update()
+            self._update()
+        ###########################################################################################
+        # move the whole building patch
+        elif self.selected_building and self.initial_click_position:
+            ds = np.array(point) - np.array(self.initial_click_position)
+            # Move the building
+            # set the vertices of the src.Building object, then copy them into the building patch
+            self.selected_building.move_building(ds)
+            self.patch_manager.redraw_building(self.selected_building)
+            # Update the initial click position for next movement calculation
+            self.initial_click_position = point
+
+            # Redraw to show the moved building
+            self._update()
 
-    def on_button_release(self, event):
+    def _on_button_release(self, event):
         self.initial_click_position = None
         self.selected_drone = None
         self.dragging_drone_point = None
         self.selected_vertex = None
 
-    def delete_selected_building(self):
+    def _delete_selected_building(self):
         if self.selected_building:
             self.actions_stack.remove_action("building", self.selected_building)
             building = self.selected_building
             self.selected_building = None
             self.patch_manager.remove_building_patch(building)
             self.buildings.remove(building)
-            self.update()
+            self._update()
 
-    def on_key_press(self, event):
+    def _on_key_press(self, event):
         # switch between building and drone placement modes
-        self.switch_mode(event)
+        self._switch_mode(event)
 
         if event.key == "tab" and self.mode == "building":
             # plot the building
-            self.finalize_building()
-
-        if event.key == "cmd+z":
-            self.undo_last_action()
+            self._finalize_building()
 
-        elif event.key == "backspace":
-            self.delete_selected_building()
+        if event.key in ["cmd+z", "ctrl+z"]:
+            self._undo_last_action()
 
-        elif event.key == "escape":
-            self.clear_temp_elements()
-
-    def set_path(self, path: str) -> None:
-        self.output_path = path
+        if event.key in ["cmd+s", "ctrl+s"]:
+            self._create_json(self.output_path)
 
-    def create_json(self):
-        if not self.drones:
-            # print("Make sure to have at least one drone")
-            self.warning.set_visible(True)  # Start with warning hidden
-            # Set a timer to hide the warning after 2 seconds
-            t = Timer(2, self.hide_warning)
-            t.start()
+        elif event.key in ["backspace", "delete"]:
+            self._delete_selected_building()
 
-            self.update()
-        else:
-            create_json(self.output_path, self.buildings, self.drones)
+        elif event.key == "escape":
+            self._clear_temp_elements()
 
-    def update(self):
+    def _show_warning(self, text:str, duration:float = 3, **kwargs)->None:
+        '''Display the central warning temporarily, set kwargs as per ax.annotate'''
+        self.warning.set_text(text)
+        self.warning.set(**kwargs)
+        self.warning.set_visible(True)  # Start with warning hidden
+        self._update()
+        # Set a timer to hide the warning after {duration} seconds
+        if self.timer and self.timer.is_alive():
+            self.timer.cancel()
+        self.timer = Timer(duration, self._hide_warning)
+        self.timer.start()
+        
+    def _update(self):
         # draw the canvas again
         self.fig.canvas.draw()
 
-    def clear_temp_elements(self):
+    def _clear_temp_elements(self):
 
         self.patch_manager.remove_temp_drone_start()
         self.patch_manager.clear_building_vertices()
 
         self.current_drone = None
-        self.update()
+        self._update()
 
-    def undo_last_action(self):
+    def _undo_last_action(self):
         if not self.actions_stack.actions:
             return
 
         action, obj = self.actions_stack.retrieve_last_action()
         if action == "building":
             self.selected_building = None
             self.patch_manager.remove_building_patch(obj)
@@ -430,17 +484,17 @@
             self.buildings.remove(obj)
 
         elif action == "drone":
             if obj in self.drones:
                 self.drones.remove(obj)
                 self.patch_manager.remove_drone_patch(obj)
 
-        self.update()
+        self._update()
 
-    def switch_mode(self, event=None):
+    def _switch_mode(self, event=None):
         """
         Switch between building and drone placement modes.
         If an event is provided and the key is 'd' or 'b', switch to the respective mode.
         If no event is provided, toggle between modes.
         """
         # If an event is provided, check the key and switch mode accordingly
         if event:
@@ -459,103 +513,120 @@
         self.mode = new_mode
         switch_label = (
             "Switch to Buildings" if self.mode == "drone" else "Switch to Drones"
         )
         self.ui_components.rename_button(button_key="switch", new_label=switch_label)
 
         # Call the update method
-        self.update()
+        self._update()
 
-    def finalize_building(self):
+    def _finalize_building(self):
         building = self.patch_manager.make_building()
         if building:
             # this if statement checks to see if a building was created
             # ie if the vertex number was >=3
             self.buildings.append(building)
             self.actions_stack.add_action("building", building)
-            self.update()
-
-    def plot_setup(self):
-        fig = plt.figure(figsize=self.FIG_SIZE)
-        ax = fig.add_subplot(111)
-
-        fig.subplots_adjust(bottom=0.1, top=0.9)
+            self._update()
 
-        ax.set_xlim(self.AXIS_LIMITS)
-        ax.set_ylim(self.AXIS_LIMITS)
-        ax.set_box_aspect(1)
-        # ax.set_xlabel("East --> (m)")
-        # ax.set_ylabel("North --> (m)")
-        ax.grid(color="k", linestyle="-", linewidth=0.5, which="major")
-        ax.grid(color="k", linestyle=":", linewidth=0.5, which="minor")
-        # ax.grid(True)
-        ax.minorticks_on()
-
-        # Add instructions
-        instructions = (
-            "Instructions:\n"
-            "'b': switch to building mode, click to place vertices of building\n"
-            "Tab: complete a building, \n"
-            "'d': switch to drone mode. "
-            "'esc': clear unwanted points."
-        )
-
-        fig.text(
-            0.2,
-            0.91,
-            instructions,
-            fontsize=10,
-            bbox=dict(boxstyle="round", facecolor="wheat", alpha=0.5),
-        )
-
-        self.fig, self.ax = fig, ax
+    def _verify_path(self, path:str)->bool:
+        '''Verify if path is a json file (existing or not) in a valid directory
+        and show relevant warnings'''
+        response = validate_json_path(path)
+        result, info = response['result'], response['info']
+        if result!=0:
+            self._show_warning(info, 3, color='g')
+            return True
+        else:
+            self._show_warning(info,duration=3,color='r')
+            return False        
 
-        return None
+    def _text_box_submit(self, path:str):
+        if self._verify_path(path):
+            #set the new path and overwrite any previous warnings
+            self.set_output_path(path, skip_check=True)
+
+    def _load_json(self, path:str):
+        '''Checks validity of input json, shows relevant warnings and calls load_scene'''
+        #first save the existing plot to temporary file
+        create_json('TEMP.json', self.buildings, self.drones)
+        if not self._verify_path(path):
+            return
+        try:
+            self.load_scene(path)
+            self._show_warning(f'Loaded {Path(path).resolve().name}', duration=3, color='g')
+        except FileNotFoundError as e:
+            self._show_warning(f'Error: {path} does not exist.', 3, color='r')
+            #TODO print full exception
+            traceback.print_exc()
+            #load back the temporary file
+            self.load_scene('TEMP.json')
+        except Exception as e:
+            #not ideal but catch and json formatting errors for now
+            self._show_warning(f'JSON Decode Error: {Path(path).resolve().name} format incompatible', 3, color='r')
+            #TODO print full exception
+            traceback.print_exc()
+            #load back the temporary file
+            self.load_scene('TEMP.json')
+        
+        os.remove('TEMP.json')
+        
+    def _create_json(self, path:str):
+        if not self.drones:
+            #amber warning for no drones
+            self._show_warning(f"Saving scene to file: {path}\nWARNING, No Drones!", duration=3, color = (1,0.75,0,1))
+        else:
+            #green warning if at least one drone
+            self._show_warning(f'Saving to file: \n{path}', duration=3, color = 'g')
+        create_json(path, self.buildings, self.drones)
 
-    def call(self, event: str, *args, **kwargs):
+    def _call(self, event: str, *args, **kwargs):
+        '''class called by observers triggered by button or text_box, see ui_components.py and observer_utils.py'''
         if event == "switch_mode":
-            self.switch_mode()
+            self._switch_mode()
         elif event == "reset":
-            self.reset()
-        # elif event == "run":
-        #     self.run()
+            self._reset()
         elif event == "create_json":
-            self.create_json()
-        # elif event == "generate_case":
-        #     case = generate_case(name="my_case", buildings=self.buildings, drones = self.drones)
-        #     #return the case to whichever application might be interested
-        #     # the event is generate_case
-        #     # plt.close()
-        #     self.notify_observers(event, case)
+            self._create_json(path=self.output_path)
+        elif event == "load_json":
+            path = kwargs["input"]
+            self._load_json(path)
+        elif event=="text_box_submit":
+            path = kwargs["input"]
+            self._text_box_submit(path)
 
-    def reset(self):
+
+    def _reset(self):
         self.selected_building = None
-        self.clear_temp_elements()
+        self._clear_temp_elements()
         # Remove all building and drone patches
         self.patch_manager.clear_all()
 
         # Empty the buildings and drones lists
         self.buildings.clear()
         self.drones.clear()
 
         # Empty the actions stack
         self.actions_stack.clear()
 
         # Redraw the plot
         self.ax.figure.canvas.draw()
 
 
-if __name__ == "__main__":
-    # Example usage:
-
-    plot = SceneBuilder()
-    plot.draw_scene("scenebuilder.json")
-    # plot.draw_scene()
+# if __name__ == "__main__":
+#     # Example usage:
+#     import runpy
+
+#     # Replace 'module_name' with the name of your module
+#     runpy.run_module('module_name', run_name='__main__')
+#     plot = SceneBuilder()
+#     plot.draw_scene()
+#     # plot.draw_scene()
 
-    print("done")
+#     print("done")
 
 
 # Suggestions:
 # Save arena, just buildings, just drones etc
 # better instructions
 # vectors showing output of panel flow for each drone
 # dragging buildings
```

### Comparing `scenebuilder-0.1.4/scenebuilder/utils.py` & `scenebuilder-0.1.5/scenebuilder/utils.py`

 * *Files 24% similar despite different names*

```diff
@@ -88,31 +88,42 @@
     def default(self, obj):
         if isinstance(obj, np.ndarray):
             return obj.tolist()  # Convert numpy arrays to lists
         # Let the base class default method raise the TypeError
         return json.JSONEncoder.default(self, obj)
 
 
-def validate_json_path(path):
+def validate_json_path(path:str, exit = False)->dict:
+    '''Check if json input path is valid
+    return True if valid, otherwise return False and quit if exit=True'''
     # Create a Path object
     p = Path(path)
     # Convert path to absolute path for checking existence and permissions
     abs_path = p.resolve()
-
+    pathOK = True
+    info = f'Path {abs_path} is valid'
     # Check if the path ends with .json
-    if not path.endswith(".json"):
-        print(f"The file name '{abs_path.name}' must end with '.json'.")
-        sys.exit(1)
+    if abs_path.is_dir():
+        info = f"{abs_path} is a directory.\nPlease enter path ending with a .json file"
+        pathOK = False
+    elif not path.endswith(".json"):
+        info = f"The file name '{abs_path.name}' must end with '.json'."
+        pathOK=False
+    # print(f"2:{abs_path.parent=}, {abs_path.parent.is_dir()}")
 
     # Check if the directory exists and is writable
-    if not abs_path.parent.exists() or not abs_path.parent.is_dir():
-        print(
-            f"The directory '{abs_path.parent}' does not exist or is not a directory."
-        )
+    elif not abs_path.parent.exists() or not abs_path.parent.is_dir():
+        info=f"The directory '{abs_path.parent}' does not exist or is not a directory."
+        pathOK=False
+
+    elif not os.access(abs_path.parent, os.W_OK):
+        info = f"The directory '{abs_path.parent}' is not writable."
+        pathOK=False
+
+    if not exit:
+        return {'result': pathOK, 'info': info}
+    elif not pathOK:
         sys.exit(1)
 
-    if not os.access(abs_path.parent, os.W_OK):
-        print(f"The directory '{abs_path.parent}' is not writable.")
-        sys.exit(1)
 
     # If all checks are passed, confirm the path is valid
     # print(f"The path: {path} is valid.")
```

### Comparing `scenebuilder-0.1.4/PKG-INFO` & `scenebuilder-0.1.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scenebuilder
-Version: 0.1.4
+Version: 0.1.5
 Summary: A simple GUI to create 2D scenes with obstacles and drone paths for multi-agent path planning algorithms
 Author: Adrian del Ser
 Author-email: adrian.delser@gmail.com
 Requires-Python: >=3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
@@ -32,23 +32,36 @@
 pip install scenebuilder
 ```
 
 This command installs SceneBuilder along with numpy and matplotlib, ensuring that everything needed to run the GUI is properly set up.
 
 
 
-## Getting Started
 
-### Prerequisites
+## Prerequisites
 
 SceneBuilder's prerequisites are defined in the pyproject.toml file and include Matplotlib and numpy.
 
-### Quick Start Guide
+## Quick Start Guide
 
-To start using SceneBuilder, you need to create an instance of the `SceneBuilder` class and invoke the `draw_scene()` method. Below is a simple example to get you started:
+### Using Command-Line Options
+
+You can use SceneBuilder directly from the command line with the following options:
+
+- `-o`, `--output`: Specify the path where the scene should be saved as a JSON file.
+- `-l`, `--load`: Specify a JSON file path to load an existing scene.
+
+Example usage:
+
+```bash
+scenebuilder --load path/to/scene.json --output path/to/output.json
+```
+
+### In Code
+To use SceneBuilder in code, you need to create an instance of the `SceneBuilder` class and invoke the `draw_scene()` method. Below is a simple example to get you started:
 
 ```python
 from scenebuilder import SceneBuilder
 
 # Create an instance of the SceneBuilder
 scene = SceneBuilder()
 
@@ -66,34 +79,24 @@
 Specify the path to save your output json to:
 
 ```python
 scene.set_output_path("path/to/output.json")
 scene.draw_scene()
 ```
 
-### Using Command-Line Options
-
-You can also use SceneBuilder directly from the command line with the following options:
-
-- `-o`, `--output`: Specify the path where the scene should be saved as a JSON file.
-- `-l`, `--load`: Specify a JSON file path to load an existing scene.
 
-Example usage:
-
-```bash
-scenebuilder --load path/to/scene.json --output path/to/output.json
-```
 
 ## Features
 
 - **Draw Obstacles**: Click within the GUI to place vertices of polygons that represent obstacles. Press Tab to complete an obstacle.
 - **Add new obstacle vertices**: To add new vertices, click somewhere on the polygon's perimeter and drag to move the vertex to its desired location.
 - **Set Drone Paths**: Click once to place the starting point, and again to place the goal of an agent/drone. An arrow will automatically be drawn from start to goal.
 - **Move or adjust existing obstacles/drones**: Obstacles and drones can be moved by clicking and dragging. Drone start and goal points, as well as existing obstacle vertices can be moved in the same way.
 - **Switch between Obstacle and Drone Modes**: Press b to switch to building/obstacle mode. Press d to switch to drone/agent mode. Alternatively click the Switch button on the bottom left of the gui.
+- **Delete obstacles**: Select the obstacle and press delete or backspace. NOTE this is not yet available for drones.
 - **Remove unwanted points**: To remove unwanted points (either obstacle vertices or a drone start point), press escape.
 - **Undo drone/obstacle placement**: To remove the last obstacle or drone, press ctrl+z.
 - **Reset Scene**: To reset the scene to a blank canvas, click the Reset button in the gui.
 
 ## Saving Scenes
 
 Once you have created a scene, you can save it to a JSON file by clicking the 'Create JSON' button in the GUI. This file can then be used as input for path planning algorithms that require predefined scenes with obstacles and paths.
```

