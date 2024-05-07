# Comparing `tmp/nbappinator-0.0.6.tar.gz` & `tmp/nbappinator-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nbappinator-0.0.6.tar", last modified: Tue Apr 30 23:08:06 2024, max compression
+gzip compressed data, was "nbappinator-0.1.0.tar", last modified: Tue May  7 01:11:48 2024, max compression
```

## Comparing `nbappinator-0.0.6.tar` & `nbappinator-0.1.0.tar`

### file list

```diff
@@ -1,19 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 23:08:06.073922 nbappinator-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (127)     1479 2024-04-30 23:07:15.000000 nbappinator-0.0.6/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)      390 2024-04-30 23:08:06.073922 nbappinator-0.0.6/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 23:08:06.069922 nbappinator-0.0.6/nbappinator/
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-30 23:07:15.000000 nbappinator-0.0.6/nbappinator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      972 2024-04-30 23:07:15.000000 nbappinator-0.0.6/nbappinator/aggridhelper.py
--rw-r--r--   0 runner    (1001) docker     (127)    22472 2024-04-30 23:07:15.000000 nbappinator-0.0.6/nbappinator/appinator.py
--rw-r--r--   0 runner    (1001) docker     (127)    15397 2024-04-30 23:07:15.000000 nbappinator-0.0.6/nbappinator/datagrid.py
--rw-r--r--   0 runner    (1001) docker     (127)     1602 2024-04-30 23:07:15.000000 nbappinator-0.0.6/nbappinator/plotly_charts.py
--rw-r--r--   0 runner    (1001) docker     (127)     2339 2024-04-30 23:07:15.000000 nbappinator-0.0.6/nbappinator/treew.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 23:08:06.069922 nbappinator-0.0.6/nbappinator.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      390 2024-04-30 23:08:06.000000 nbappinator-0.0.6/nbappinator.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      370 2024-04-30 23:08:06.000000 nbappinator-0.0.6/nbappinator.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 23:08:06.000000 nbappinator-0.0.6/nbappinator.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-30 23:08:06.000000 nbappinator-0.0.6/nbappinator.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-30 23:08:06.000000 nbappinator-0.0.6/nbappinator.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      544 2024-04-30 23:07:15.000000 nbappinator-0.0.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     3048 2024-04-30 23:07:15.000000 nbappinator-0.0.6/readme.md
--rw-r--r--   0 runner    (1001) docker     (127)      333 2024-04-30 23:08:06.073922 nbappinator-0.0.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:11:48.553390 nbappinator-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1479 2024-05-07 01:10:49.000000 nbappinator-0.1.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)      390 2024-05-07 01:11:48.553390 nbappinator-0.1.0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:11:48.553390 nbappinator-0.1.0/nbappinator/
+-rw-r--r--   0 runner    (1001) docker     (127)      237 2024-05-07 01:10:49.000000 nbappinator-0.1.0/nbappinator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-05-07 01:10:49.000000 nbappinator-0.1.0/nbappinator/aggridhelper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21269 2024-05-07 01:10:49.000000 nbappinator-0.1.0/nbappinator/appinator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      746 2024-05-07 01:10:49.000000 nbappinator-0.1.0/nbappinator/browser_title.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15322 2024-05-07 01:10:49.000000 nbappinator-0.1.0/nbappinator/datagrid.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 01:10:49.000000 nbappinator-0.1.0/nbappinator/jinjamagic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1839 2024-05-07 01:10:49.000000 nbappinator-0.1.0/nbappinator/plotly_charts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1579 2024-05-07 01:10:49.000000 nbappinator-0.1.0/nbappinator/treew.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:11:48.553390 nbappinator-0.1.0/nbappinator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      390 2024-05-07 01:11:48.000000 nbappinator-0.1.0/nbappinator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-07 01:11:48.000000 nbappinator-0.1.0/nbappinator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 01:11:48.000000 nbappinator-0.1.0/nbappinator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-07 01:11:48.000000 nbappinator-0.1.0/nbappinator.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-07 01:11:48.000000 nbappinator-0.1.0/nbappinator.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      544 2024-05-07 01:10:49.000000 nbappinator-0.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     4564 2024-05-07 01:10:49.000000 nbappinator-0.1.0/readme.md
+-rw-r--r--   0 runner    (1001) docker     (127)      333 2024-05-07 01:11:48.553390 nbappinator-0.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:11:48.553390 nbappinator-0.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 01:10:49.000000 nbappinator-0.1.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      523 2024-05-07 01:10:49.000000 nbappinator-0.1.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      636 2024-05-07 01:10:49.000000 nbappinator-0.1.0/tests/env_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5963 2024-05-07 01:10:49.000000 nbappinator-0.1.0/tests/snapshot_mgr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1265 2024-05-07 01:10:49.000000 nbappinator-0.1.0/tests/test_fails.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2683 2024-05-07 01:10:49.000000 nbappinator-0.1.0/tests/test_nb.py
```

### Comparing `nbappinator-0.0.6/LICENSE.md` & `nbappinator-0.1.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `nbappinator-0.0.6/nbappinator/aggridhelper.py` & `nbappinator-0.1.0/nbappinator/aggridhelper.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,38 +1,40 @@
 import ipyaggrid as ag
 import pandas as pd
 from .datagrid import ColMd, DataGrid
-from typing import Optional, Callable
+from typing import Optional, Callable, Literal
 
 
 def display_ag(
     input_df: pd.DataFrame,
     is_tree: bool,
     pathcol: Optional[str] = "path",
     pathdelim="/",
     col_md: list[ColMd] = [],  # noqa: F821
     showindex: bool = False,
     action: Optional[Callable] = None,
     num_toppinned_rows: int = 0,
     grid_options: dict = {},
     flatten_columns: bool = True,
     default_precision: int = 2,
+    select_mode: Optional[Literal["single", "multiple"]] = None,
 ) -> ag.Grid:
 
     grid = DataGrid(
         grid_data=input_df,
         is_tree=is_tree,
         pathcol=pathcol,
         pathdelim=pathdelim,
         col_md=col_md,
         showindex=showindex,
         num_toppinned_rows=num_toppinned_rows,
         grid_options=grid_options,
         default_precision=default_precision,
         flatten_columns=flatten_columns,
+        select_mode=select_mode,
     )
 
     if action is not None:
         grid.on("cellClicked", action)
 
     grid.df = input_df  # type: ignore
     return grid
```

### Comparing `nbappinator-0.0.6/nbappinator/appinator.py` & `nbappinator-0.1.0/nbappinator/appinator.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,216 +1,244 @@
 import enum
 import logging
+import io
+
 from functools import partial
 from dataclasses import dataclass, field
 from typing import Callable, Dict, List, Optional, Union, Annotated, ContextManager
 
 import ipytree
 import ipyvuetify as v
 import ipywidgets
 from ipyvuetify import Tab, TabItem
-from ipywidgets import HBox, Widget
+from ipywidgets import Widget
 from IPython.display import display
 import traitlets
 
-
+from . import BrowserTitle
 from . import aggridhelper as g
 from . import treew
 from . import datagrid
 from . import plotly_charts as pcharts
 
 logger = logging.getLogger(__name__)
 
 PATHDELIM = "~"
 
 
 @dataclass
 class UiWidget:
     w: Widget
-    name: str
-    replaceable: bool = False
+    name: Optional[str]
 
 
 class SelectTypes(enum.Enum):
     dropdown = 1
     combobox = 2
     slider = 3
     radio = 4
 
 
 @dataclass
 class UiPage:
     app: "UiModel"
     name: str
+
     widget: ipywidgets.Widget
 
-    def clear_page(self):
-        self.app.clear_page(self.name)
+    def clear(self):
+        p = self.widget
+        if p is not None:
+            # TODO: Remove from self.widgets. Not critical, since widgets are overwritten by key value
+            p.children = []  # type: ignore
 
-    def add_box(
-        self, name: str, horiz: bool = False, override_page: Optional[str] = None
-    ):
-        """Adds either a horizontal or vertical box to contain the element. It can be given a container name (to_container) so the container can be cleared and repopulated.
+    def add(self, elements: Union[UiWidget, List[UiWidget]]):
+        self.app._add(target=self.name, elements=elements)
+
+    def add_box(self, name: str, horiz: bool = False) -> "UiPage":
+        """Adds either a horizontal or vertical box to contain the element.
 
 
         Args:
             page (str): App page to add this box to
             name (str): A globally unique name for the box widget, so it can be later modified
             horiz (bool, optional): Horizontal or Vertical. Defaults to False (Vertical).
-            to_container (Optional[str], optional): Creates a container, so the widgets can later be added using a container parameter. Defaults to None.
 
         Returns:
             _type_: _description_
         """
         if horiz:
             h = v.Html(tag="div", class_="d-flex flex-row", children=[])
         else:
             h = v.Html(tag="div", class_="d-flex flex-column", children=[])
 
         self.app.containers[name] = h
 
-        return self.app.add(
-            page=self.name,
-            override_page=override_page,
+        self.add(
             elements=UiWidget(w=h, name=name),
         )
 
-    def add_separator(self, name: str, color: str = "gray"):
+        return UiPage(self.app, name, h)  # type: ignore
+
+    def add_separator(self, color: str = "gray", name: Optional[str] = None):
         w = v.Html(tag="hr", style_=f"border: none; border-top: 5px solid {color};")
 
-        return self.app.add(page=self.name, elements=UiWidget(w=w, name=name))
+        return self.add(
+            elements=UiWidget(w=w, name=name),
+        )
 
-    def add_container(self, name: str):
+    def add_container(self, name: str) -> "UiPage":
+        """Use add_box instead"""
         w = v.Container()
         self.app.containers[name] = w
-        return self.app.add(page=self.name, elements=UiWidget(w=w, name=name))
+        w = self.add(
+            elements=UiWidget(w=w, name=name),
+        )
 
-    def add_tree(self, name: str, paths: list[str], delim: str = PATHDELIM):
+        return UiPage(self.app, name, w)  # type: ignore
+
+    def add_tree(
+        self,
+        paths: list[str],
+        delim: str = PATHDELIM,
+        name: Optional[str] = None,
+    ):
         w = treew.w_tree_paths(
             paths=paths, pathdelim=delim if delim is not None else PATHDELIM
         )
-        return self.app.add(page=self.name, elements=UiWidget(w=w, name=name))
+        self.add(
+            elements=UiWidget(w=w, name=name),
+        )
 
     def add_textarea(
-        self, name: str, label: str, disabled: bool = False, value: str = ""
+        self,
+        label: str,
+        name: Optional[str] = None,
+        disabled: bool = False,
+        value: str = "",
     ):
         w = v.Textarea(label=label, v_model=value, disabled=disabled)
-        return self.app.add(page=self.name, elements=UiWidget(w=w, name=name))
+        self.add(
+            elements=UiWidget(w=w, name=name),
+        )
 
     def add_textfield(
         self,
-        name: str,
         label: Optional[str] = None,
         class_: Optional[str] = None,
         disabled: bool = False,
         value: str = "",
         solo=False,
         flat=False,
-        override_page: Optional[str] = None,
+        name: Optional[str] = None,
     ):
         w = v.TextField(
             class_=class_,
             label=label,
             v_model=value,
             disabled=disabled,
             solo=solo,
             flat=flat,
         )
-        return self.app.add(
-            page=self.name,
-            override_page=override_page,
+        return self.add(
             elements=UiWidget(w=w, name=name),
         )
 
-    def add_progress(self, name: str, override_page: Optional[str] = None):
+    def add_progress(
+        self,
+        name: Optional[str] = None,
+    ):
         w = v.ProgressLinear(
             class_="progress-bar", width=0, color="blue", indeterminate=True
         )
         w.hide()
-        self.app.add(
-            page=self.name,
-            override_page=override_page,
+        self.add(
             elements=UiWidget(w=w, name=name),
         )
 
-    def add_textstatic(self, value: str = "", name: str = "anonymous"):
+    def add_textstatic(
+        self,
+        value: str = "",
+        name: Optional[str] = None,
+    ):
         w = v.CardText(children=value)
-        return self.app.add(page=self.name, elements=UiWidget(w=w, name=name))
+        return self.add(
+            elements=UiWidget(w=w, name=name),
+        )
 
-    def add_textpre(self, name: str, value: str = ""):
+    def add_textpre(
+        self,
+        value: str = "",
+        name: Optional[str] = None,
+    ):
         w = v.Html(tag="pre", children=[value], style_="max-height:80vh")
-        return self.app.add(page=self.name, elements=UiWidget(w=w, name=name))
+        return self.add(
+            elements=UiWidget(w=w, name=name),
+        )
 
-    def add_output(self, name: str, max_outputs: Optional[int] = None):
+    def add_output(
+        self,
+        max_outputs: Optional[int] = None,
+        name: Optional[str] = None,
+    ):
         w = ipywidgets.Output()
         if max_outputs is not None:
             w.max_outputs = max_outputs  # type: ignore
 
-        return self.app.add(page=self.name, elements=UiWidget(w=w, name=name))
+        return self.add(
+            elements=UiWidget(w=w, name=name),
+        )
 
     def add_plt(
         self,
-        name: str,
         plt,
         width=1024,
         height=1024,
-        override_page: Optional[str] = None,
+        name: Optional[str] = None,
     ):
-        import io
 
         buf = io.BytesIO()
         plt.fig.savefig(buf, format="png")
         image_widget = ipywidgets.widgets.Image(
             value=buf.getvalue(), format="png", width=width, height=height
         )
 
-        return self.app.add(
-            page=self.name,
-            override_page=override_page,
+        return self.add(
             elements=UiWidget(w=image_widget, name=name),
         )
 
     def add_plotly_fig(
         self,
-        name: str,
         fig,
         height=None,
         width=None,
         png=False,
         setcolors=True,
-        override_page: Optional[str] = None,
+        name: Optional[str] = None,
     ):
         w = pcharts.create_widget(
             fig=fig, setcolors=setcolors, height=height, width=width, png=png
         )
 
-        return self.app.add(
-            page=self.name,
-            override_page=override_page,
+        return self.add(
             elements=UiWidget(w=w, name=name),
         )
 
     def add_select(
         self,
-        name: str,
         label: str,
         disabled: bool = False,
         options: List = [],
         value=None,
         type: SelectTypes = SelectTypes.dropdown,
         multiple: bool = False,
         action: Optional[Callable] = None,
         horiz: bool = False,
-        override_page: Optional[str] = None,
+        name: Optional[str] = None,
     ):
-        if not isinstance(options, list):
-            options = list(options)
-
-        if value is True:
-            value = options[0]
 
         if type == SelectTypes.dropdown:
             w = v.Select(
                 label=label,
                 disabled=disabled,
                 items=options,
                 multiple=multiple,
@@ -240,28 +268,25 @@
         else:
             raise ValueError(f"Unexpected type: {type}")
 
         if action is not None:
             # Use partial to pass the app & the caller name
             action = partial(action, app=self.app, caller=name)
             w.on_event("change", action)
-        return self.app.add(
-            page=self.name,
-            override_page=override_page,
+        return self.add(
             elements=UiWidget(w=w, name=name),
         )
 
     def add_button(
         self,
-        name: str,
+        label: str,
         action: Callable[..., None],
         disabled: bool = False,
         status: bool = False,
-        label: Optional[str] = None,
-        override_page: Optional[str] = None,
+        name: Optional[str] = None,
     ):
         """
 
         Args:
             page (str): The tab (page) or the container to add the button to.
             name (str): Internal name used to reference the button widget
             action (Callable): Callable that is executed when button is clicked. Must take four parameters: component, action, args, app, and caller.
@@ -269,110 +294,123 @@
             status (bool, optional): Adds a status field to the right of the button. Useful for showing feedback to user of application process. Defaults to False.
             label (Optional[str], optional): Label to show to side of button. Defaults to None.
 
         Returns:
             _type_: _description_
         """
 
-        if label is None:  # label must be set, but default to the name
-            label = name
+        if name is None:  # label must be set, but default to the name
+            name = label
 
         if status:
             status_container = name + ".box"
-            self.add_box(
-                name=status_container, horiz=False, override_page=override_page
-            )
-            target = status_container
+            status_box = self.add_box(name=status_container, horiz=False)
         else:
-            target = self.name
+            status_box = None
 
         b = v.Btn(children=[label], disabled=disabled, outlined=True)
 
         if action is not None:
             # Use partial to pass the app & the caller name
             action = partial(action, app=self.app, caller=name)
             b.on_event("click", action)
 
-        o = self.app.add(
-            page=self.name, override_page=target, elements=UiWidget(w=b, name=name)
-        )
+        if status_box:
+            o = status_box.add(elements=UiWidget(w=b, name=name))
+        else:
+            o = self.add(elements=UiWidget(w=b, name=name))
 
         if status:
             self.add_textfield(
-                override_page=target,
                 name=name + ".status",
                 label=None,
                 disabled=True,
                 value="Not Run",
                 solo=True,
                 flat=True,
                 class_="for-progress",
             )
 
             progress_container = name + ".box.progress"
-            self.add_box(name=progress_container, override_page=target, horiz=False)
+            box = self.add_box(name=progress_container, horiz=False)
 
-            self.add_progress(
-                override_page=progress_container, name=name + ".status_bar"
-            )
+            box.add_progress(name=name + ".status_bar")
         return o
 
     def add_df(
         self,
-        name,
         df,
         tree: bool = False,
         pathcol: Optional[str] = None,
-        perccols=[],  # deprecated
-        coltypes={},  # deprecated use col_md
         col_md: List[g.ColMd] = [],
         showindex: bool = False,
         action: Optional[Callable] = None,
         num_toppinned_rows: int = 0,
-        is_table_viewer_df: bool = False,
+        table_viewer: bool = False,
         flatten_columns: bool = True,
         pathdelim: str = PATHDELIM,
         precision: int = 2,
+        grid_options: dict = {},
+        multiselect: bool = False,
+        name: Optional[str] = None,
     ):
-        if perccols or coltypes:
-            raise ValueError("Deprecated, use col_md")
-
-        grid_options = {}
-
-        if is_table_viewer_df is True:
+        if table_viewer is True:
             grid_options["autoGroupColumnDef"] = {
                 "cellRendererParams": {
                     "suppressCount": True,
                     "suppressGroupCheckbox": """function(params) {
                         return params.node.allLeafChildren.length === 1;
                     }""",
                 },
             }
 
             grid_options["groupDefaultExpanded"] = -1
 
+        if multiselect:
+            select_mode = "multiple"
+        else:
+            select_mode = None
+
+        if tree and pathcol not in df.columns:
+            raise ValueError("If tree, then pathcol must be in df.columns")
+
         w = g.display_ag(
             df,
             tree,
             pathcol=pathcol,
             pathdelim=pathdelim,
             showindex=showindex,
             col_md=col_md,
             action=action,
             num_toppinned_rows=num_toppinned_rows,
             grid_options=grid_options,
             flatten_columns=flatten_columns,
             default_precision=precision,
+            select_mode=select_mode,
         )
 
-        return self.app.add(page=self.name, elements=UiWidget(w=w, name=name))
+        return self.add(
+            elements=UiWidget(w=w, name=name),
+        )
+
+    def add_html(
+        self,
+        html: str,
+        name: Optional[str],
+    ):
+
+        ho = HTMLOutput()
+        ho.html = html
+        w = UiWidget(name=name, w=ho)
+        self.add(w)
 
 
 @dataclass
 class UiModel:
+
     pages: List[str]
 
     log_page: Optional[str] = None
 
     _page_widgets: Dict[str, UiPage] = field(default_factory=dict)
 
     messages: Annotated[ContextManager[str], field(init=False)] = field(init=False)
@@ -380,109 +418,82 @@
     # Containers are used for replacing existing elements and are optional
     containers: Dict[str, ipywidgets.Widget] = field(default_factory=dict)
 
     # Every UI widget is stored by name (globally in the app). This is used
     # to retrieve the current value of individual widgets.
     widgets: Dict[str, UiWidget] = field(default_factory=dict)
 
-    def __post_init__(self):
-        for p in self.pages:
-            self._add_page(title=p)
-
-        if self.log_page is not None:
-            self.get_page(self.log_page).add_output(name="m.ta")
-            self.messages = self.widgets["m.ta"].w  # type: ignore
+    title: Optional[str] = None
 
     def get_valuestr(self, name):
         return str(self.get_values(name))  # type: ignore
 
     def get_values(self, name):
         w = self.widgets[name].w
 
         if isinstance(w, datagrid.DataGrid):
             return w.current_selection
         if isinstance(w, ipytree.tree.Tree):
             return w.value()  # type: ignore
         else:
             return self.widgets[name].w.v_model  # type: ignore
 
-    def _add_page(self, title: str, children: List = []):
-        self._page_widgets[title] = UiPage(
-            app=self, name=title, widget=ipywidgets.VBox(children)
-        )
-
-    def add(
-        self,
-        page: str,
-        elements: Union[UiWidget, List[UiWidget]],
-        override_page: Optional[str] = None,
-    ):
-        page = page if override_page is None else override_page
-        if page is None:
-            raise ValueError(
-                "Page must be set to either a page name or a container name"
-            )
+    def _add(self, target: str, elements: Union[UiWidget, List[UiWidget]]):
+        """Target can be either a Page name or a Container name"""
+        if isinstance(elements, UiWidget):
+            elements = [elements]
 
-        if not isinstance(elements, list):
-            elements_list = [elements]
-        else:
-            elements_list = elements
-
-        if page in self.containers:
+        if target in self.containers:
             logger.debug("Adding to container")
-            widgets = [e.w for e in elements_list]
-            self.containers[page].children = (  # type: ignore
-                *self.containers[page].children,  # type: ignore
+            widgets = [e.w for e in elements]
+            self.containers[target].children = (  # type: ignore
+                *self.containers[target].children,  # type: ignore
                 *widgets,
             )
-            for e in elements_list:
-                self.widgets[e.name] = e
+            for e in elements:
+                if e.name is not None:
+                    self.widgets[e.name] = e
         else:
             logger.debug("Adding to page")
 
-            page = self._page_widgets[page].widget  # type: ignore
+            page = self._page_widgets[target].widget  # type: ignore
 
             children = page.children  # type: ignore
             newchildren = []
-            for e in elements_list:
-                self.widgets[e.name] = e
+            for e in elements:
+                if e.name is not None:
+                    self.widgets[e.name] = e
 
-                if e.replaceable:
-                    new_container = HBox([e.w])
-                    self.containers[e.name] = new_container
-                    newchildren.append(new_container)
-                else:
-                    newchildren.append(e.w)
+                newchildren.append(e.w)
 
             page.children = (*children, *newchildren)  # type: ignore
 
-        return elements
+    def get_page(self, title: Union[str, int]):
+        """
 
-    def replace(self, container: str, element: UiWidget):
-        if element is None:
-            self.containers[container].children = []  # type: ignore
-        else:
-            self.containers[container].children = [element.w]  # type: ignore
-            self.widgets[element.name] = element
+        Args:
+            title (Union[str, int]): If int, returns the page at the offset given from self.pages. If str, returns the page by name
+
+        Raises:
+            ValueError: An error if the input is not a Page
+
+        """
+        if isinstance(title, int):
+            title = self.pages[title]
 
-    def get_page(self, title: str):
         if title in self._page_widgets:
             return self._page_widgets[title]
         else:
             raise ValueError(f"{title} is not a page")
 
     def set_value(self, name, value):
         self.widgets[name].w.v_model = value  # type: ignore
 
-    def clear_page(self, title: str):
-        p = self.get_page(title=title).widget
-
-        if p is not None:
-            # TODO: Remove from self.widgets. Not critical, since widgets are overwritten by key value
-            p.children = []  # type: ignore
+    def clear_messages(self):
+        self.messages.clear_output()  # type: ignore
 
     def clear_container(self, id: str):
         w = self.widgets[id].w
         w.children = []  # type: ignore
 
     def update_status(self, name: str, message: str, running: bool = True):
         self.set_value(f"{name}.status", message)
@@ -558,33 +569,37 @@
                 ]
             )
         if log_page_name is not None:
             self.get_page(log_page_name).add_output(name="m.ta", max_outputs=100)
             self._tabWidget = v.Tabs(v_model=[0], children=children)
             self.messages = self.widgets["m.ta"].w  # type: ignore
 
+        if self.title is not None:
+            BrowserTitle(self.title)
+
     def add_page(
         self, title: str, children: List = [], selected_tab=True
     ) -> ipywidgets.Widget:
         self.pages.append(title)
 
         tab_children = [*self._tabWidget.children]
 
         t = Tab(children=[title])
         ti = TabItem(
             children=children, style_="padding-left: 20px; padding-right: 20px;"
         )
         tab_children.append(t)
         tab_children.append(ti)
-        self._page_widgets[title] = ti  # type: ignore
+        self._page_widgets[title] = UiPage(app=self, name=title, widget=ti)
+
         self._tabWidget.children = tab_children
         if selected_tab:
             self._tabWidget.v_model = len(tab_children) / 2 - 1
 
-        return ti  # type: ignore
+        return self._page_widgets[title]  # type: ignore
 
     def remove_page(self, title: str):
         if title in self.pages:
             index = list(self.pages).index(title)
             self.pages.remove(title)
 
             tab_children = [*self._tabWidget.children]
@@ -596,25 +611,22 @@
             if self._tabWidget.v_model == index:
                 self._tabWidget.v_model = index - 1
 
     def open_tab(self, name: str):
         if name in self.pages:
             self._tabWidget.v_model = list(self.pages).index(name)
 
-        # display(f"Toggling {index} {name} {self.tabWidget.children[index]}")
-
     def toggle_tab(self, name: str, disabled: bool):
         if name in self.pages:
             index = list(self.pages).index(name)
             index *= 2
             self._tabWidget.children[index].disabled = disabled
         if self.headers is not None and name in self.headers:
             index = list(self.headers).index(name)
             self._headerWidget.children[index].disabled = disabled  # type: ignore
-        # display(f"Toggling {index} {name} {self.tabWidget.children[index]}")
 
     def get_children(self):
         children = []
         if self._headerWidget is not None:
             children.append(self._headerWidget)
         if self._tabWidget is not None:
             children.append(self._tabWidget)
@@ -675,15 +687,14 @@
     html = traitlets.Unicode(default_value=None, allow_none=True).tag(sync=True)
 
     @traitlets.default("template")
     def _template(self):
         return """
             <template>
                 <div v-html="html">
-                    
                 </div>
             </template>
         """
 
 
 class ThemeFixer:
     def _repr_html_(self) -> str:
```

### Comparing `nbappinator-0.0.6/nbappinator/datagrid.py` & `nbappinator-0.1.0/nbappinator/datagrid.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,26 +13,22 @@
 @dataclass
 class ColMd:
     name: str
     label: Optional[str] = None
     format: str = "default"  # percent, decimal, mag_si (convert to K/M/G suffixes)
     pinned: bool = False
     hidden: bool = False
-    display_props = None
     precision: Optional[int] = None
 
     def __post_init__(self):
         if not isinstance(self.name, str):
             self.name = str(self.name)
         if self.label is None:
             self.label = self.name.title().replace("_", " ")
 
-        if self.display_props is not None and self.display_props.pinned:
-            self.pinned = True
-
 
 def _addcol(
     md: ColMd,
     allcols: Dict[str, Dict[str, object]],
     autodetect: bool = True,
     precision: int = 2,
 ):
@@ -189,33 +185,36 @@
         showindex: bool = False,
         js_post_grid: List = [],
         js_pre_grid: List = [],
         grid_options: Dict = {},
         num_toppinned_rows=0,
         flatten_columns=True,
         default_precision=2,
-        license="community",
+        license="e",
         *argv,
         **kargv,
     ):
         # if pathcol is not None:
         #    pathcol = pathcol.title()
         sortcols = False
         if isinstance(grid_data, pd.DataFrame) and flatten_columns:
             input_df = grid_data.copy()
             input_df.columns = [str(col) for col in input_df.columns]
-
         else:
             input_df = pd.DataFrame(grid_data)
+
         if showindex:
             input_df = input_df.reset_index()
 
         allcols = {}
 
-        self._select_mode = select_mode
+        if select_mode is not None:
+            self._select_mode = select_mode
+        else:
+            self._select_mode = "single"
 
         # Handle MD's first
         for md in col_md:
             _addcol(md, allcols, precision=default_precision)
 
             if md.format == "perc_div":
                 input_df[md.name] = input_df[md.name] / 100
@@ -379,47 +378,47 @@
             **kargv,
         }
 
         super().__init__(*argv, **args)
 
         self.message_handlers = []
 
-        def msg_rx(_, msg, buffers):
+        def msg_rx(
+            _, msg, buffers
+        ):  # pragma: no cover  # bypassing because only reached from js
             try:
                 self.process_message(msg)
             except Exception as e:
                 logger.info("Unable to send msg")
                 logger.exception(e)
 
         self.on_msg(msg_rx)
 
     def process_message(self, msg: Any):
-        logger.debug("Widget got message", msg)
+        logger.debug("Widget got message: %s", msg)
         pMsg = msg
 
         # make sure its one of our events
         if "type" not in pMsg or pMsg["type"] != "gridEvent" and "event_type" in pMsg:
             return
+
         if self._select_mode is not None:
             if pMsg["event_type"] == "cellClicked" and "currentSelection" in pMsg:
                 self.current_selection = pMsg["currentSelection"]
 
         logger.debug("Checking message handler for %s", len(self.message_handlers))
         for handler, handle_msg_type in self.message_handlers:
             logger.debug(
                 "Checking message handler for %s and message type %s",
                 handle_msg_type,
                 pMsg["type"],
             )
             if handle_msg_type is None or pMsg["event_type"] == handle_msg_type:
                 logger.debug("Calling handler")
-                try:
-                    handler(pMsg)
-                except Exception:
-                    logger.exception("Error running handler")
+                handler(pMsg)
 
     def on(
         self,
         msg_type: str,
         handler: Callable[[Dict], None],
     ):
         self.message_handlers.append((handler, msg_type))
```

### Comparing `nbappinator-0.0.6/nbappinator/plotly_charts.py` & `nbappinator-0.1.0/nbappinator/plotly_charts.py`

 * *Files 8% similar despite different names*

```diff
@@ -25,30 +25,37 @@
 ) -> w.Widget:
     if setcolors:
         default_color_scale = pc.DEFAULT_PLOTLY_COLORS
         numcolors = len(default_color_scale)
 
         line_dash_sequence = ["solid", "dot", "dash"]
         for i, trace in enumerate(fig.data):
-            try:
+            if hasattr(trace, "line"):
                 line_dash_index = (i // numcolors) % len(line_dash_sequence)
                 trace.line.dash = line_dash_sequence[line_dash_index]  # type: ignore
-            except Exception:
-                logger.exception("Error setting colors")
 
     if height is not None:
         fig.layout.height = height
     if width is not None:
         fig.layout.width = width
 
     if png:
+        raise ValueError(
+            "Not supported at this time due to kaleido hanging on some environments."
+        )
+        import kaleido  # type: ignore  # noqa
+
+        # Kaleido is only required if png generation is needed. This ensures it is installed.
+        # App may hang otherwise
+
+        # if width is None:
+        #    fig.layout.width = 900
         image_bytes = pio.to_image(fig, format="png")
         encoded_image = base64.b64encode(image_bytes).decode("utf-8")
-        if width is None:
-            fig.layout.width = 900
+
         w = v.Html(
             tag="img",
             children=[],
             attributes={"src": "data:image/png;base64," + encoded_image},
         )
 
     else:
```

### Comparing `nbappinator-0.0.6/nbappinator/treew.py` & `nbappinator-0.1.0/nbappinator/treew.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,19 +1,17 @@
 import logging
-import ipywidgets
-import ipyvuetify as v
 from ipytree import Node, Tree
 
 logger = logging.getLogger(__name__)
 
 
-def w_tree(root: str):
-    rootText = f'<span style="color: green;font-weight: italic;">{root}</span>'
-    tree = Tree(nodes=[Node(rootText)])
-    return tree
+# def w_tree(root: str):
+#    rootText = f'<span style="color: green;font-weight: italic;">{root}</span>'
+#    tree = Tree(nodes=[Node(rootText)])
+#    return tree
 
 
 def w_tree_paths(paths: list[str], pathdelim):
     nodes = {}  # defaultdict(default_factor=list)
     rootnodes = []
 
     paths = sorted(paths)
@@ -56,37 +54,7 @@
     Tree.value = tree_value  # type: ignore
 
     tree = Tree()
     for n in rootnodes:
         tree.add_node(n)
 
     return tree
-
-
-def w_output():
-    out = ipywidgets.Output()
-    with out:
-        print("Hi!")
-    return out
-
-
-def w_tabs(tabs: dict[str, list[ipywidgets.Widget]]):
-    # Create three Tab components
-
-    children = []
-
-    for k, w in tabs.items():
-        tab = v.Tab(children=[k])
-        if isinstance(v, list):
-            content = v.TabItem(
-                children=w, style_="padding-left: 40%; padding-right: 10%;"
-            )
-        else:
-            content = v.TabItem(
-                children=[w], style_="padding-left: 40%; padding-right: 10%;"
-            )
-        children.append(tab)
-        children.append(content)
-
-    tabWidget = v.Tabs(v_model=0, children=children)  # select first tab
-
-    return tabWidget
```

### Comparing `nbappinator-0.0.6/pyproject.toml` & `nbappinator-0.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "nbappinator"
-version = "0.0.6"
+version = "0.1.0"
 description = "Jupyter Notebook Application Builder"
 authors = [{ name = "Paul Timmins", email = "paul@iqmo.com" }]
 dependencies = ["ipywidgets~=7.8.0", "plotly", "ipyvuetify>=1.9", "ipyaggrid", "ipytree", "pandas>=1.5.3"]
 readme = "README.md"
 
 
 [build-system]
```

