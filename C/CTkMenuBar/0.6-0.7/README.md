# Comparing `tmp/ctkmenubar-0.6.tar.gz` & `tmp/ctkmenubar-0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ctkmenubar-0.6.tar", last modified: Thu Apr 25 11:29:00 2024, max compression
+gzip compressed data, was "ctkmenubar-0.7.tar", last modified: Tue May  7 08:07:06 2024, max compression
```

## Comparing `ctkmenubar-0.6.tar` & `ctkmenubar-0.7.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-04-25 11:29:00.837409 ctkmenubar-0.6/
-drwxrwxrwx   0        0        0        0 2024-04-25 11:29:00.814413 ctkmenubar-0.6/CTkMenuBar/
--rw-rw-rw-   0        0        0      269 2024-04-25 11:27:10.000000 ctkmenubar-0.6/CTkMenuBar/__init__.py
--rw-rw-rw-   0        0        0    14537 2024-04-25 11:25:38.000000 ctkmenubar-0.6/CTkMenuBar/dropdown_menu.py
--rw-rw-rw-   0        0        0     2184 2024-03-25 11:25:04.000000 ctkmenubar-0.6/CTkMenuBar/menu_bar.py
--rw-rw-rw-   0        0        0     4474 2024-03-25 11:33:03.000000 ctkmenubar-0.6/CTkMenuBar/title_menu_win.py
-drwxrwxrwx   0        0        0        0 2024-04-25 11:29:00.835413 ctkmenubar-0.6/CTkMenuBar.egg-info/
--rw-rw-rw-   0        0        0     4491 2024-04-25 11:29:00.000000 ctkmenubar-0.6/CTkMenuBar.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      308 2024-04-25 11:29:00.000000 ctkmenubar-0.6/CTkMenuBar.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0       40 2024-04-25 11:29:00.000000 ctkmenubar-0.6/CTkMenuBar.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2024-04-25 11:29:00.000000 ctkmenubar-0.6/CTkMenuBar.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-04-25 11:29:00.000000 ctkmenubar-0.6/CTkMenuBar.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     7048 2022-11-20 16:16:56.000000 ctkmenubar-0.6/LICENSE
--rw-rw-rw-   0        0        0     4491 2024-04-25 11:29:00.836411 ctkmenubar-0.6/PKG-INFO
--rw-rw-rw-   0        0        0     3769 2024-03-25 11:15:27.000000 ctkmenubar-0.6/README.md
--rw-rw-rw-   0        0        0      582 2024-04-25 11:29:00.840412 ctkmenubar-0.6/setup.cfg
--rw-rw-rw-   0        0        0     1129 2024-04-25 11:28:38.000000 ctkmenubar-0.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-07 08:07:05.996886 ctkmenubar-0.7/
+drwxrwxrwx   0        0        0        0 2024-05-07 08:07:05.960703 ctkmenubar-0.7/CTkMenuBar/
+-rw-rw-rw-   0        0        0      269 2024-05-07 08:00:37.000000 ctkmenubar-0.7/CTkMenuBar/__init__.py
+-rw-rw-rw-   0        0        0    14973 2024-05-07 08:02:44.000000 ctkmenubar-0.7/CTkMenuBar/dropdown_menu.py
+-rw-rw-rw-   0        0        0     2328 2024-05-07 07:47:33.000000 ctkmenubar-0.7/CTkMenuBar/menu_bar.py
+-rw-rw-rw-   0        0        0     4942 2024-05-07 07:48:19.000000 ctkmenubar-0.7/CTkMenuBar/title_menu_win.py
+drwxrwxrwx   0        0        0        0 2024-05-07 08:07:05.993354 ctkmenubar-0.7/CTkMenuBar.egg-info/
+-rw-rw-rw-   0        0        0     4669 2024-05-07 08:07:05.000000 ctkmenubar-0.7/CTkMenuBar.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      308 2024-05-07 08:07:05.000000 ctkmenubar-0.7/CTkMenuBar.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0       40 2024-05-07 08:07:05.000000 ctkmenubar-0.7/CTkMenuBar.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2024-05-07 08:07:05.000000 ctkmenubar-0.7/CTkMenuBar.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-05-07 08:07:05.000000 ctkmenubar-0.7/CTkMenuBar.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     7048 2022-11-20 16:16:56.000000 ctkmenubar-0.7/LICENSE
+-rw-rw-rw-   0        0        0     4669 2024-05-07 08:07:05.995875 ctkmenubar-0.7/PKG-INFO
+-rw-rw-rw-   0        0        0     3944 2024-05-07 08:06:18.000000 ctkmenubar-0.7/README.md
+-rw-rw-rw-   0        0        0      582 2024-05-07 08:07:06.005395 ctkmenubar-0.7/setup.cfg
+-rw-rw-rw-   0        0        0     1129 2024-05-07 08:01:32.000000 ctkmenubar-0.7/setup.py
```

### Comparing `ctkmenubar-0.6/CTkMenuBar/dropdown_menu.py` & `ctkmenubar-0.7/CTkMenuBar/dropdown_menu.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,18 +10,38 @@
 import tkinter as tk
 from typing import Callable
 
 class _CDMOptionButton(customtkinter.CTkButton):
     def setParentMenu(self, menu: "CustomDropdownMenu"):
         self.parent_menu = menu
 
+    def cget(self, param):
+        if param=="option":
+            return self.cget("text")
+        return super().cget(param)
+    
+    def configure(self, **kwargs):
+        if "option" in kwargs:
+            super().configure(text=kwargs.pop("option"))
+        super().configure(**kwargs)
+        
 class _CDMSubmenuButton(_CDMOptionButton):
     def setSubmenu(self, submenu: "CustomDropdownMenu"):
         self.submenu = submenu
-
+        
+    def cget(self, param):
+        if param=="submenu_name":
+            return self.cget("text")
+        return super().cget(param)
+    
+    def configure(self, **kwargs):
+        if "submenu_name" in kwargs:
+            super().configure(text=kwargs.pop("submenu_name"))
+        super().configure(**kwargs)
+        
 class CustomDropdownMenu(customtkinter.CTkFrame):
     
     def __init__(self, 
                  widget: customtkinter.CTkBaseClass | _CDMSubmenuButton,
                  master: any = None,
                  border_width: int = 1,
                  width: int = 150,
@@ -109,15 +129,15 @@
 
         optionButton.pack(
             side="top",
             fill="both", 
             expand=True,
             padx=3+(self.corner_radius/5),
             pady=3+(self.corner_radius/5))
-        
+        return optionButton
     
     def add_submenu(self, submenu_name: str, **kwargs) -> "CustomDropdownMenu":
         submenuButtonSeed = _CDMSubmenuButton(self, text=submenu_name, anchor="w",
                                               text_color=self.text_color,
                                               width=self.width, height=self.height, **kwargs)
         submenuButtonSeed.setParentMenu(self)
         self._options_list.append(submenuButtonSeed)
@@ -137,35 +157,27 @@
             separator_color=self.separator_color,
             text_color=self.text_color,
             font=self.font)
         
         submenuButtonSeed.setSubmenu(submenu=submenu)
         submenuButtonSeed.configure(command=submenu.toggleShow)
         submenu.bind("<Enter>", lambda e: submenu._show_submenu(self, hovered=True))
-        
-        self.after(300, self.update)
-            
-        submenuButtonSeed.bind("<Enter>", lambda e: self.after(500, lambda: submenu._show_submenu(self)))
+  
+        submenu.bind("<Enter>", lambda e, submenu=submenu: submenu._show_submenu(self, hovered=True), add="+")
+        submenuButtonSeed.bind("<Enter>", lambda e: self.after(500, lambda: submenu._show_submenu(self)), add="+")
         submenuButtonSeed.bind("<Leave>", lambda e: self.after(500, lambda: submenu._left(self)), add="+")
         submenuButtonSeed.configure(cursor=self.cursor)
         
         submenuButtonSeed.pack(
             side="top",
             fill="both", 
             expand=True,
             padx=3+(self.corner_radius/5),
             pady=3+(self.corner_radius/5))
         return submenu
-    
-    def update(self):
-        subMenus = self._getSubMenus()
-        for submenu in subMenus:
-            for widget in submenu.winfo_children():
-                widget.bind("<Enter>", lambda e, submenu=submenu: submenu._show_submenu(self, hovered=True))
-        super().update()
         
     def _left(self, parent):
         if parent.hovered:
             return
         
         subMenus = parent._getSubMenus()
```

### Comparing `ctkmenubar-0.6/CTkMenuBar/menu_bar.py` & `ctkmenubar-0.7/CTkMenuBar/menu_bar.py`

 * *Files 4% similar despite different names*

```diff
@@ -31,15 +31,15 @@
         self.num = 0
         self.menu = []
         self.padx = padx
         self.pady = pady
 
         super().pack(anchor="n", fill="x")
 
-    def add_cascade(self, text=None, **kwargs):
+    def add_cascade(self, text=None, postcommand=None, **kwargs):
     
         if not "fg_color" in kwargs:
             fg_color = "transparent"
         else:
             fg_color = kwargs.pop("fg_color")
         if not "text_color" in kwargs:
             text_color = customtkinter.ThemeManager.theme["CTkLabel"]["text_color"]
@@ -55,14 +55,17 @@
             text = f"Menu {self.num+1}"
             
         self.menu_button = customtkinter.CTkButton(self, text=text, fg_color=fg_color,
                                                    text_color=text_color, width=self.width,
                                                    height=self.height, anchor=anchor, **kwargs)
         self.menu_button.grid(row=0, column=self.num, padx=(self.padx,0), pady=self.pady)
         
+        if postcommand:
+            self.menu_button.bind("<Button-1>", lambda event: postcommand(), add="+")
+            
         self.num += 1
 
         return self.menu_button
     
     def configure(self, **kwargs):
         if "bg_color" in kwargs:
            super().configure(fg_color=kwargs.pop("bg_color"))
```

### Comparing `ctkmenubar-0.6/CTkMenuBar/title_menu_win.py` & `ctkmenubar-0.7/CTkMenuBar/title_menu_win.py`

 * *Files 5% similar despite different names*

```diff
@@ -68,16 +68,24 @@
         self.padding = padx
   
         self.master.bind("<Configure>", lambda _: self.change_dimension())
         self.master.bind("<Destroy>", lambda _: super().destroy() if not self.master.winfo_viewable() else None)
         self.num = 0
         
         self.master.bind("<Map>", lambda e: self.withdraw)
+
+    def _set_appearance_mode(self, mode_string):
+        if customtkinter.get_appearance_mode()=="Light":
+            self.caption_color = 0xFFFFFF # RGB order: 0xrrggbb             
+        else:
+            self.caption_color = 0x303030 # RGB order: 0xrrggbb
+
+        self.change_header_color(self.caption_color)
         
-    def add_cascade(self, text=None, **kwargs):
+    def add_cascade(self, text=None, postcommand=None, **kwargs):
     
         if not "fg_color" in kwargs:
             fg_color = customtkinter.ThemeManager.theme["CTkFrame"]["fg_color"]
         else:
             fg_color = kwargs.pop("fg_color")
         if not "text_color" in kwargs:
             text_color = customtkinter.ThemeManager.theme["CTkLabel"]["text_color"]
@@ -88,14 +96,17 @@
             text = f"Tab {self.num+1}"
     
         self.menu_button = customtkinter.CTkButton(self, text=text, fg_color=fg_color,
                                                    text_color=text_color, width=self.width, height=10, **kwargs)
         self.menu_button.grid(row=0, column=self.num, padx=(0, self.padding))
         self.num += 1
 
+        if postcommand:
+            self.menu_button.bind("<Button-1>", lambda event: postcommand(), add="+")
+            
         return self.menu_button
     
     def change_dimension(self):
         width = self.master.winfo_width()-130-self.x_offset
         if width<0:
             self.withdraw()
             return
```

### Comparing `ctkmenubar-0.6/CTkMenuBar.egg-info/PKG-INFO` & `ctkmenubar-0.7/CTkMenuBar.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CTkMenuBar
-Version: 0.6
+Version: 0.7
 Summary: Customtkinter Menu Widget
 Home-page: https://github.com/Akascape/CTkMenuBar
 Author: Akash Bora
 License: Creative Commons Zero v1.0 Universal
 Keywords: customtkinter,customtkinter-menu,ctkmenubar,titlemenu,menubar,tkinter,menu-widget,tkinter-gui
 Classifier: License :: CC0 1.0 Universal (CC0 1.0) Public Domain Dedication
 Classifier: Programming Language :: Python :: 3
@@ -53,14 +53,15 @@
 |-----------| ------------|
 | **master** | define the master widget, can be root or frame |
 | bg_color | set the bg color of the menu bar |
 | height | set height of the menu bar |
 | width | set width of the menu bar buttons |
 | padx | set internal padding between menu bar buttons |
 | pady | set internal padding in top and bottom of menu bar |
+| postcommand | add a command before spawing the dropdown |
 | _*other frame parameters_ | other ctk frame parameters can also be passed |
 
 - ## CTkTitleMenu
 
 _This title menu is only supported in windows OS!_
 
 ![titlebar](https://github.com/Akascape/CTkMenuBar/assets/89206401/da6cd858-f700-476c-a2f0-93a1c6335a4d)
@@ -83,14 +84,15 @@
 | **master** | define the master window, can be **root or toplevel** only |
 | bg_color | set the bg color of the menu bar |
 | title_bar_color | set color to the header (**only works with windows 11**), `RGB order: 0x00rrggbb` |
 | width | set width of the menu bar buttons |
 | padx | set internal padding between menu bar buttons |
 | x_offset | set the x distance from the header |
 | y_offset | set the y distance from the header |
+| postcommand | add a command before spawing the dropdown |
 | _*other frame parameters_ | other ctk frame parameters can also be passed |
 
 ## CustomDropdownMenu
 
 This is the common dropdown menu class which is used by both ctkmenubar and ctktitlemenu. 
 
 ### Usage
@@ -105,15 +107,16 @@
 ...
 ```
 
 ### Methods
 - **.add_option(option, command)**: add option to the dropdown and attach the command
 - **.add_separator()**: add a separator line between the options
 - **.add_submenu(submenu_name)**: add a submenu as option
-
+- **.configure(**args): change dropdown menu options
+  
 ### Arguments
 | Parameter | Description |
 |-----------| ------------|
 | **widget** | attach the dropdown to the cascade widget |
 | master | *optional*, change the spawn window if required |
 | bg_color | set the bg color of the dropdown |
 | fg_color | set the option button fg color |
```

### Comparing `ctkmenubar-0.6/LICENSE` & `ctkmenubar-0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `ctkmenubar-0.6/PKG-INFO` & `ctkmenubar-0.7/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CTkMenuBar
-Version: 0.6
+Version: 0.7
 Summary: Customtkinter Menu Widget
 Home-page: https://github.com/Akascape/CTkMenuBar
 Author: Akash Bora
 License: Creative Commons Zero v1.0 Universal
 Keywords: customtkinter,customtkinter-menu,ctkmenubar,titlemenu,menubar,tkinter,menu-widget,tkinter-gui
 Classifier: License :: CC0 1.0 Universal (CC0 1.0) Public Domain Dedication
 Classifier: Programming Language :: Python :: 3
@@ -53,14 +53,15 @@
 |-----------| ------------|
 | **master** | define the master widget, can be root or frame |
 | bg_color | set the bg color of the menu bar |
 | height | set height of the menu bar |
 | width | set width of the menu bar buttons |
 | padx | set internal padding between menu bar buttons |
 | pady | set internal padding in top and bottom of menu bar |
+| postcommand | add a command before spawing the dropdown |
 | _*other frame parameters_ | other ctk frame parameters can also be passed |
 
 - ## CTkTitleMenu
 
 _This title menu is only supported in windows OS!_
 
 ![titlebar](https://github.com/Akascape/CTkMenuBar/assets/89206401/da6cd858-f700-476c-a2f0-93a1c6335a4d)
@@ -83,14 +84,15 @@
 | **master** | define the master window, can be **root or toplevel** only |
 | bg_color | set the bg color of the menu bar |
 | title_bar_color | set color to the header (**only works with windows 11**), `RGB order: 0x00rrggbb` |
 | width | set width of the menu bar buttons |
 | padx | set internal padding between menu bar buttons |
 | x_offset | set the x distance from the header |
 | y_offset | set the y distance from the header |
+| postcommand | add a command before spawing the dropdown |
 | _*other frame parameters_ | other ctk frame parameters can also be passed |
 
 ## CustomDropdownMenu
 
 This is the common dropdown menu class which is used by both ctkmenubar and ctktitlemenu. 
 
 ### Usage
@@ -105,15 +107,16 @@
 ...
 ```
 
 ### Methods
 - **.add_option(option, command)**: add option to the dropdown and attach the command
 - **.add_separator()**: add a separator line between the options
 - **.add_submenu(submenu_name)**: add a submenu as option
-
+- **.configure(**args): change dropdown menu options
+  
 ### Arguments
 | Parameter | Description |
 |-----------| ------------|
 | **widget** | attach the dropdown to the cascade widget |
 | master | *optional*, change the spawn window if required |
 | bg_color | set the bg color of the dropdown |
 | fg_color | set the option button fg color |
```

### Comparing `ctkmenubar-0.6/README.md` & `ctkmenubar-0.7/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -37,14 +37,15 @@
 |-----------| ------------|
 | **master** | define the master widget, can be root or frame |
 | bg_color | set the bg color of the menu bar |
 | height | set height of the menu bar |
 | width | set width of the menu bar buttons |
 | padx | set internal padding between menu bar buttons |
 | pady | set internal padding in top and bottom of menu bar |
+| postcommand | add a command before spawing the dropdown |
 | _*other frame parameters_ | other ctk frame parameters can also be passed |
 
 - ## CTkTitleMenu
 
 _This title menu is only supported in windows OS!_
 
 ![titlebar](https://github.com/Akascape/CTkMenuBar/assets/89206401/da6cd858-f700-476c-a2f0-93a1c6335a4d)
@@ -67,14 +68,15 @@
 | **master** | define the master window, can be **root or toplevel** only |
 | bg_color | set the bg color of the menu bar |
 | title_bar_color | set color to the header (**only works with windows 11**), `RGB order: 0x00rrggbb` |
 | width | set width of the menu bar buttons |
 | padx | set internal padding between menu bar buttons |
 | x_offset | set the x distance from the header |
 | y_offset | set the y distance from the header |
+| postcommand | add a command before spawing the dropdown |
 | _*other frame parameters_ | other ctk frame parameters can also be passed |
 
 ## CustomDropdownMenu
 
 This is the common dropdown menu class which is used by both ctkmenubar and ctktitlemenu. 
 
 ### Usage
@@ -89,15 +91,16 @@
 ...
 ```
 
 ### Methods
 - **.add_option(option, command)**: add option to the dropdown and attach the command
 - **.add_separator()**: add a separator line between the options
 - **.add_submenu(submenu_name)**: add a submenu as option
-
+- **.configure(**args): change dropdown menu options
+  
 ### Arguments
 | Parameter | Description |
 |-----------| ------------|
 | **widget** | attach the dropdown to the cascade widget |
 | master | *optional*, change the spawn window if required |
 | bg_color | set the bg color of the dropdown |
 | fg_color | set the option button fg color |
```

### Comparing `ctkmenubar-0.6/setup.cfg` & `ctkmenubar-0.7/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2043 546b 4d65 6e75 4261 720d 0a76   = CTkMenuBar..v
-00000020: 6572 7369 6f6e 203d 2030 2e36 0d0a 6465  ersion = 0.6..de
+00000020: 6572 7369 6f6e 203d 2030 2e37 0d0a 6465  ersion = 0.7..de
 00000030: 7363 7269 7074 696f 6e20 3d20 4375 7374  scription = Cust
 00000040: 6f6d 746b 696e 7465 7220 4d65 6e75 2057  omtkinter Menu W
 00000050: 6964 6765 740d 0a6c 6f6e 675f 6465 7363  idget..long_desc
 00000060: 7269 7074 696f 6e20 3d20 6669 6c65 3a20  ription = file: 
 00000070: 5245 4144 4d45 2e6d 640d 0a6c 6f6e 675f  README.md..long_
 00000080: 6465 7363 7269 7074 696f 6e5f 636f 6e74  description_cont
 00000090: 656e 745f 7479 7065 203d 2074 6578 742f  ent_type = text/
```

### Comparing `ctkmenubar-0.6/setup.py` & `ctkmenubar-0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     """Opens and fetches text of long descrition file."""
     with open(path, 'r') as f:
         text = f.read()
     return text
 
 setup(
     name = 'CTkMenuBar',
-    version = '0.6',
+    version = '0.7',
     description = "Customtkinter Menu Widget",
     license = "Creative Commons Zero v1.0 Universal",
     readme = "README.md",
     long_description = get_long_description('README.md'),
     long_description_content_type = "text/markdown",
     author = 'Akash Bora',
     url = "https://github.com/Akascape/CTkMenuBar",
```

