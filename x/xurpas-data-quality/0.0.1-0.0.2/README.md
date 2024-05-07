# Comparing `tmp/xurpas_data_quality-0.0.1-py3-none-any.whl.zip` & `tmp/xurpas_data_quality-0.0.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,24 @@
-Zip file size: 5077 bytes, number of entries: 10
--rw-rw-rw-  2.0 fat       35 b- defN 24-May-02 06:14 xurpas_data_quality/__init__.py
--rw-rw-rw-  2.0 fat     1361 b- defN 24-May-02 06:14 xurpas_data_quality/data_report.py
--rw-rw-rw-  2.0 fat       30 b- defN 24-May-02 06:14 xurpas_data_quality/report/__init__.py
--rw-rw-rw-  2.0 fat     5254 b- defN 24-May-02 06:14 xurpas_data_quality/report/report.py
--rw-rw-rw-  2.0 fat      152 b- defN 24-May-02 06:14 xurpas_data_quality/visuals/__init__.py
--rw-rw-rw-  2.0 fat     1939 b- defN 24-May-02 06:14 xurpas_data_quality/visuals/plots.py
--rw-rw-rw-  2.0 fat      496 b- defN 24-May-02 06:48 xurpas_data_quality-0.0.1.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-May-02 06:48 xurpas_data_quality-0.0.1.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       20 b- defN 24-May-02 06:48 xurpas_data_quality-0.0.1.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      896 b- defN 24-May-02 06:48 xurpas_data_quality-0.0.1.dist-info/RECORD
-10 files, 10275 bytes uncompressed, 3515 bytes compressed:  65.8%
+Zip file size: 12370 bytes, number of entries: 22
+-rw-rw-rw-  2.0 fat       35 b- defN 24-Apr-30 01:38 xurpas_data_quality/__init__.py
+-rw-rw-rw-  2.0 fat     1011 b- defN 24-May-03 02:20 xurpas_data_quality/data_report.py
+-rw-rw-rw-  2.0 fat        0 b- defN 24-May-07 05:20 xurpas_data_quality/data/__init__.py
+-rw-rw-rw-  2.0 fat      286 b- defN 24-Apr-30 02:18 xurpas_data_quality/data/dataframe.py
+-rw-rw-rw-  2.0 fat     6613 b- defN 24-May-06 01:25 xurpas_data_quality/data/describe.py
+-rw-rw-rw-  2.0 fat      224 b- defN 24-May-06 01:15 xurpas_data_quality/data/descriptions.py
+-rw-rw-rw-  2.0 fat      350 b- defN 24-Apr-26 07:12 xurpas_data_quality/data/pandas_dataframe.py
+-rw-rw-rw-  2.0 fat        0 b- defN 24-May-03 07:10 xurpas_data_quality/data/alerts/__init__.py
+-rw-rw-rw-  2.0 fat      953 b- defN 24-May-06 00:02 xurpas_data_quality/data/alerts/alerts.py
+-rw-rw-rw-  2.0 fat       54 b- defN 24-May-03 03:30 xurpas_data_quality/data/algorithms/__init__.py
+-rw-rw-rw-  2.0 fat      495 b- defN 24-May-03 03:47 xurpas_data_quality/data/algorithms/algorithms.py
+-rw-rw-rw-  2.0 fat        0 b- defN 24-May-07 05:20 xurpas_data_quality/render/__init__.py
+-rw-rw-rw-  2.0 fat     4411 b- defN 24-May-06 05:05 xurpas_data_quality/render/renderer.py
+-rw-rw-rw-  2.0 fat      569 b- defN 24-Apr-30 07:06 xurpas_data_quality/render/templates.py
+-rw-rw-rw-  2.0 fat       30 b- defN 24-Apr-30 02:52 xurpas_data_quality/report/__init__.py
+-rw-rw-rw-  2.0 fat     7914 b- defN 24-May-06 05:08 xurpas_data_quality/report/report.py
+-rw-rw-rw-  2.0 fat      141 b- defN 24-May-06 02:32 xurpas_data_quality/visuals/__init__.py
+-rw-rw-rw-  2.0 fat     2257 b- defN 24-May-06 02:30 xurpas_data_quality/visuals/plots.py
+-rw-rw-rw-  2.0 fat      535 b- defN 24-May-07 05:22 xurpas_data_quality-0.0.2.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-May-07 05:22 xurpas_data_quality-0.0.2.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       20 b- defN 24-May-07 05:22 xurpas_data_quality-0.0.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     2051 b- defN 24-May-07 05:22 xurpas_data_quality-0.0.2.dist-info/RECORD
+22 files, 28041 bytes uncompressed, 8920 bytes compressed:  68.2%
```

## zipnote {}

```diff
@@ -1,31 +1,67 @@
 Filename: xurpas_data_quality/__init__.py
 Comment: 
 
 Filename: xurpas_data_quality/data_report.py
 Comment: 
 
+Filename: xurpas_data_quality/data/__init__.py
+Comment: 
+
+Filename: xurpas_data_quality/data/dataframe.py
+Comment: 
+
+Filename: xurpas_data_quality/data/describe.py
+Comment: 
+
+Filename: xurpas_data_quality/data/descriptions.py
+Comment: 
+
+Filename: xurpas_data_quality/data/pandas_dataframe.py
+Comment: 
+
+Filename: xurpas_data_quality/data/alerts/__init__.py
+Comment: 
+
+Filename: xurpas_data_quality/data/alerts/alerts.py
+Comment: 
+
+Filename: xurpas_data_quality/data/algorithms/__init__.py
+Comment: 
+
+Filename: xurpas_data_quality/data/algorithms/algorithms.py
+Comment: 
+
+Filename: xurpas_data_quality/render/__init__.py
+Comment: 
+
+Filename: xurpas_data_quality/render/renderer.py
+Comment: 
+
+Filename: xurpas_data_quality/render/templates.py
+Comment: 
+
 Filename: xurpas_data_quality/report/__init__.py
 Comment: 
 
 Filename: xurpas_data_quality/report/report.py
 Comment: 
 
 Filename: xurpas_data_quality/visuals/__init__.py
 Comment: 
 
 Filename: xurpas_data_quality/visuals/plots.py
 Comment: 
 
-Filename: xurpas_data_quality-0.0.1.dist-info/METADATA
+Filename: xurpas_data_quality-0.0.2.dist-info/METADATA
 Comment: 
 
-Filename: xurpas_data_quality-0.0.1.dist-info/WHEEL
+Filename: xurpas_data_quality-0.0.2.dist-info/WHEEL
 Comment: 
 
-Filename: xurpas_data_quality-0.0.1.dist-info/top_level.txt
+Filename: xurpas_data_quality-0.0.2.dist-info/top_level.txt
 Comment: 
 
-Filename: xurpas_data_quality-0.0.1.dist-info/RECORD
+Filename: xurpas_data_quality-0.0.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## xurpas_data_quality/data_report.py

```diff
@@ -3,23 +3,14 @@
 from pathlib import Path
 
 from xurpas_data_quality.render.renderer import HTMLBase
 from xurpas_data_quality.data.dataframe import load_dataframe, validate_dataframe
 from xurpas_data_quality.data.describe import describe
 from xurpas_data_quality.report import get_report
 
-"""def get_data_quality_report():
-    return HTMLBase(body=None, name='Manhour Utilization Summary').render()
-
-def to_file(file_path:str, file_name:str="report.html"):
-    output = Path(file_path+ "/" + file_name)
-    print(f"saving to {file_path}")
-    output.write_text(get_data_quality_report(), encoding='utf-8')
-    print(f"saved!")"""
-
 
 class DataReport:
     def __init__(self, df:str):
         if df is None:
             raise ValueError("there must be an input!")
         self.df = load_dataframe(df)
         
@@ -27,12 +18,12 @@
         self.description = describe(self.df)
 
     def get_data_quality_report(self, name=None):
         self.describe_dataframe()
         report = get_report(self.description, name=name)
         return report.render()
     
-    def to_file(self, file_path:str, file_name:str="report.html"):
-        output = Path(file_path+ "/" + file_name)
-        print(f"saving to {file_path}")
-        output.write_text(self.get_data_quality_report(), encoding='utf-8')
+    def to_file(self, report_name:str=None, file_name:str="report.html"):
+        output = Path(file_name)
+        print(f"saving as {file_name}")
+        output.write_text(self.get_data_quality_report(report_name), encoding='utf-8')
         print(f"saved!")
```

## xurpas_data_quality/report/report.py

```diff
@@ -1,17 +1,18 @@
 from xurpas_data_quality.data.descriptions import TableDescription
-from xurpas_data_quality.render.renderer import HTMLBase, HTMLContainer, HTMLTable, HTMLVariable, HTMLPlot, HTMLToggle, HTMLCollapse
-from xurpas_data_quality.visuals import plot_to_base64, create_tiny_histogram, create_histogram, create_distribution_plot, create_heatmap, create_distribution_from_dataframe
+from xurpas_data_quality.render.renderer import HTMLBase, HTMLContainer, HTMLTable, HTMLVariable, HTMLPlot, HTMLToggle, HTMLCollapse, HTMLDropdown
+from xurpas_data_quality.visuals import plot_to_base64, create_tiny_histogram, create_histogram, create_distribution_plot, create_heatmap, create_interaction_plot
 
 from dataclasses import fields
 
-def get_detailed_variable_info(df, key, details:list):
+def get_detailed_variable_info(df, key:str, variables:dict):
+    details = variables['details']
     bottom = [            
         HTMLContainer(
-            type="box",
+            type="default",
             name="Statistics",
             id= "stats",
             container_items= [
                 HTMLContainer(
                     type="column",
                     container_items=
                         HTMLTable(
@@ -32,14 +33,34 @@
             ]
         ),
         HTMLPlot(
             name="Histogram",
             type="large",
             id="histo",
             plot=plot_to_base64(create_histogram(df[key]))
+        ),
+        HTMLTable(
+            id = f"{key}-common_values",
+            name = "Common Values",
+            data= variables["common"].to_html(classes="table table-sm", border=0)),
+        HTMLContainer(
+            type="tabs",
+            name="Extreme Values",
+            container_items=[
+                HTMLTable(
+                    id = f"{key}-min-values",
+                    name="Minimum 10 Values",
+                    data=variables["min"].to_html(classes="table table-sm", border=0)
+                ),
+                HTMLTable(
+                    id = f"{key}-max-values",
+                    name="Maximum 10 Values",
+                    data=variables["max"].to_html(classes="table table-sm", border=0)
+                )
+            ]
         )
     ]
     if df[key].dtype != 'object':
         bottom.append(            
             HTMLPlot(
                 name="Distribution",
                 id="distribution",
@@ -48,15 +69,15 @@
             ))
     return HTMLContainer(
         type="tabs",
         col=key,
         container_items=bottom
     )
 
-def get_variable_data(data: TableDescription):
+def get_variable_data(data: TableDescription) -> list:
     variables = []
 
     for key, value in data.variables.items():
         split_dict = lambda d: (dict(list(d.items())[:len(d)//2]), dict(list(d.items())[len(d)//2:]))
         table_1, table_2 = split_dict(value['overview'])
 
         variable_body = {
@@ -65,22 +86,54 @@
             'plot': HTMLPlot(plot=plot_to_base64(create_tiny_histogram(data.df[key])))
         }
         btn = HTMLToggle("More details", key)
         variables.append(
                     HTMLVariable(
                         name=key,
                         body = variable_body,
-                        bottom = HTMLCollapse(btn, get_detailed_variable_info(data.df,key,data.variables[key]['details']))
-                    ))
+                        bottom = HTMLCollapse(btn, 
+                                              get_detailed_variable_info(data.df,
+                                                                         key,
+                                                                         data.variables[key]))
+                    )
+                )
     
     return variables
 
+def get_interactions(data:TableDescription):
+    df = data.df.select_dtypes(exclude=['object'])
+    outer_tabs = []
+    for column in df.columns:
+        inner_tabs = []
+        for inner_col in df.columns:
+            inner_tabs.append(
+                HTMLContainer(
+                    type="default",
+                    name= inner_col,
+                    id = f"{column}-{inner_col}-interaction-inner",
+                    container_items = [HTMLPlot(
+                        plot= plot_to_base64(create_interaction_plot(df[inner_col],df[column])),
+                        type = "large",
+                        name = f"{column}-{inner_col} Interaction Plot",
+                        id = f"{column}-{inner_col}_interaction_plot"
+                    )]
+                )
+            )
+        outer_tabs.append(
+            HTMLContainer(
+                type="tabs",
+                name = column,
+                id = f"{column}-interaction-outer",
+                container_items = inner_tabs
+            )
+        )
+    return outer_tabs
+
 def get_report(data: TableDescription, name:str=None)-> HTMLBase:
     content = []
-
     overview_section = HTMLContainer(
         type="box",
         name="Overview",
         container_items = [
             HTMLContainer(
                 type="column",
                 container_items = HTMLTable(
@@ -92,19 +145,25 @@
                 container_items =  HTMLTable(
                     data=data.var_types,
                     name="Variable Types"
                 )
             )
         ]
     )
-
+    dropdown = [HTMLDropdown(
+        dropdown_items= list(data.df),
+        dropdown_content= HTMLContainer(
+            type="default",
+            container_items=get_variable_data(data)),
+        id="variables-dropdown"
+    )]
     variables_section = HTMLContainer(
         type="box",
         name="Variables",
-        container_items = get_variable_data(data)
+        container_items = dropdown
     )
 
     corr_df = data.df.corr(numeric_only=True).round(3)
     correlation = HTMLContainer(
         type="box",
         name="Correlation",
         container_items=[
@@ -131,38 +190,49 @@
             HTMLTable(
                 id = "sample",
                 data=data.df.head(10).to_html(classes="table table-sm", border=0)
             )
         ]
     )
 
-    distribution = HTMLContainer(
+    interactions = HTMLContainer(
         type="box",
-        name="Distribution",
+        name="Interactions",
         container_items=[
-            HTMLPlot(
-                plot= plot_to_base64(create_distribution_from_dataframe(data.df)),
-                type="large"
+            HTMLContainer(
+                type="tabs",
+                container_items= get_interactions(data)
             )
         ]
     )
+
+    """    distribution = HTMLContainer(
+            type="box",
+            name="Distribution",
+            container_items=[
+                HTMLPlot(
+                    plot= plot_to_base64(create_distribution_from_dataframe(data.df)),
+                    type="large"
+                )
+            ]
+        )"""
     
     content.extend([
         overview_section,
         variables_section,
         correlation,
-        samples,
-        distribution
+        interactions,
+        samples
     ])
 
     body = HTMLContainer(
         type="sections",
         container_items = content,
     )
-
+    
     if name is not None:
         return HTMLBase(
             body=body,
             name=name
         )
     
     else:
```

## xurpas_data_quality/visuals/__init__.py

```diff
@@ -1 +1 @@
-from .plots import create_tiny_histogram, plot_to_base64, create_histogram, create_heatmap, create_distribution_plot, create_distribution_from_dataframe
+from .plots import create_tiny_histogram, plot_to_base64, create_histogram, create_heatmap, create_distribution_plot, create_interaction_plot
```

## xurpas_data_quality/visuals/plots.py

```diff
@@ -2,29 +2,31 @@
 import base64
 
 import pandas as pd
 import numpy as np
 import matplotlib as mpl
 import matplotlib.pyplot as plt
 
-def create_tiny_histogram(df):
+from xurpas_data_quality.data.algorithms import sturges, rice,freedman_diaconis
+
+def create_tiny_histogram(data: pd.Series):
     fig= plt.figure()
-    plt.hist(df, edgecolor="white")
+    plt.hist(data, edgecolor="white")
     plt.box(False)
 
     return fig
 
-def create_histogram(df):
+def create_histogram(data: pd.Series):
     fig= plt.figure(figsize=(8,4))
-    plt.hist(df, edgecolor="white")
+    plt.hist(data, edgecolor="white", bins=freedman_diaconis(data))
     plt.box(False)
 
     return fig
 
-def create_heatmap(df):
+def create_heatmap(df: pd.DataFrame):
     # Create a figure and a set of subplots
     fig, ax = plt.subplots()
     plt.box(False)
     # Create the heatmap
     heatmap = ax.imshow(df, cmap='RdYlBu', interpolation='nearest', vmin=-1.0, vmax=1.0)
 
     # Set the column names as x-axis labels
@@ -51,14 +53,21 @@
 
     axs[1].violinplot(column)
 
     fig.suptitle(f'{column.name} distribution')
 
     return fig
 
+def create_interaction_plot(x: pd.Series, y: pd.Series):
+    fig = plt.figure(figsize=(8,4))
+    plt.scatter(x,y,edgecolor="white")
+
+    return fig
+    
+
 def create_distribution_from_dataframe(df: pd.DataFrame):
     if 'employee_code' in df.columns:
         df = df.drop('employee_code', axis=1)
 
     fig = plt.figure()
     boxplot = df.boxplot(figsize=(15,3))
     return fig
```

