# Comparing `tmp/odk_tools-0.1.8.tar.gz` & `tmp/odk_tools-0.1.9.tar.gz`

## Comparing `odk_tools-0.1.8.tar` & `odk_tools-0.1.9.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 odk_tools-0.1.8/src/odk_tools/__init__.py
--rw-r--r--   0        0        0    20111 2020-02-02 00:00:00.000000 odk_tools-0.1.8/src/odk_tools/classes.py
--rw-r--r--   0        0        0     3012 2020-02-02 00:00:00.000000 odk_tools-0.1.8/src/odk_tools/functions.py
--rw-r--r--   0        0        0    21128 2020-02-02 00:00:00.000000 odk_tools-0.1.8/src/odk_tools/odk.py
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 odk_tools-0.1.8/.gitignore
--rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 odk_tools-0.1.8/LICENSE
--rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 odk_tools-0.1.8/README.md
--rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 odk_tools-0.1.8/pyproject.toml
--rw-r--r--   0        0        0      704 2020-02-02 00:00:00.000000 odk_tools-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 odk_tools-0.1.9/src/odk_tools/__init__.py
+-rw-r--r--   0        0        0    15381 2020-02-02 00:00:00.000000 odk_tools-0.1.9/src/odk_tools/classes.py
+-rw-r--r--   0        0        0     3074 2020-02-02 00:00:00.000000 odk_tools-0.1.9/src/odk_tools/functions.py
+-rw-r--r--   0        0        0    21128 2020-02-02 00:00:00.000000 odk_tools-0.1.9/src/odk_tools/odk.py
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 odk_tools-0.1.9/.gitignore
+-rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 odk_tools-0.1.9/LICENSE
+-rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 odk_tools-0.1.9/README.md
+-rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 odk_tools-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0      704 2020-02-02 00:00:00.000000 odk_tools-0.1.9/PKG-INFO
```

### Comparing `odk_tools-0.1.8/src/odk_tools/classes.py` & `odk_tools-0.1.9/src/odk_tools/odk.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,472 +1,552 @@
+#%% #@ Libraries imports
+
 import pandas as pd
-import copy
-import matplotlib.gridspec as gridspec
-from fpdf import FPDF
-import matplotlib.pyplot as plt
-from io import BytesIO
 import numpy as np
+import requests
+import json
+from io import BytesIO
+import copy
+import zipfile as zip
+import xlsxwriter
+import xml.etree.ElementTree as ET
+import uuid
+from types import FunctionType
+from .classes import Form
+
+#%% #@ Functions
+
+def save_to_excel(data, filename="output.xlsx", column_width=25, include_index=False, row_colours={0: "#D8E4BC", 1: "#C5D9F1"}, row_bold=[0], row_wrap=[1], autofilter=True, freeze_panes=True):
+
+    workbook = xlsxwriter.Workbook(filename)
+    worksheet = workbook.add_worksheet()
+
+    for i in range(len(data.columns)):
+        worksheet.write(0, i, data.columns[i])
+
+    for i in range(len(data)):
+        for j in range(len(data.columns)):
+            if pd.isna(data.iloc[i, j]):
+                pass
+            else:
+                worksheet.write(i+1, j, data.iloc[i, j])
+
+    worksheet.set_column(0, len(data.columns), width=column_width)
+
+    for i in range(len(data)):
+        a = {}
+        if i in list(row_colours.keys()):
+            a["bg_color"] = row_colours[i]
+        if i in row_bold:
+            a["bold"] = True
+        if i in row_wrap:
+            a["text_wrap"] = True
+        if len(a) != 0:
+            worksheet.set_row(i, cell_format=workbook.add_format(a))
 
+    if autofilter:
+        worksheet.autofilter(1, 0, len(data), len(data.columns)-1)
 
-# class SurveyPlus(pd.DataFrame):
-#     """
-#     attribute = surveys \n
-#     methods = surveyfilter, surveysubset, get_survey, merge_horizontal, merge_vertical
-#     """
-
-#     def __init__(self, *args, **kwargs):
-#         pd.DataFrame.__init__(self, *args, **kwargs)
-
-#     @property
-#     def _constructor(self):
-#         return SurveyPlus
-
-#     _metadata = ["surveys"]
-
-#     surveys = {'baseline': ['_B'],
-#                'recruitment': ['_R'],
-#                'diary': ['_D'],
-#                'weekly': ['_W'],
-#                'pay': ['_P'],
-#                'end': ['_E']}
-
-#     def check_surveys(x):
-#         tocheck = x.surveys
-#         suffix = list(set(pd.Series(x.columns).apply(
-#             lambda a: "_"+a.split("_")[-1])))
-#         for j in tocheck.keys():
-#             for k in tocheck[j]:
-#                 if k not in suffix:
-#                     tocheck[j].remove(k)
-#         new = {}
-#         for j in tocheck.keys():
-#             if len(tocheck[j]) != 0:
-#                 new[j] = tocheck[j]
-#         x.surveys = new
-
-#     def survey_filter(self, survey_in=None, x=surveys):
-#         """
-#         Input list of surveys.
-#         """
-#         if survey_in == None:
-#             return self
-#         else:
-#             get_extension = []
-#             for j in survey_in:
-#                 for k in x[j]:
-#                     get_extension.append(k)
-#             get_columns = []
-#             for k in self.columns:
-#                 if "_"+k.split("_")[-1] in get_extension:
-#                     get_columns.append(k)
-#             self = self.drop_duplicates(subset=get_columns).dropna(
-#                 how="all", subset=get_columns)
-#             self.surveys = {key: value for key,
-#                             value in x.items() if key in survey_in}
-#             return self
-
-#     def survey_subset(self, survey_in=None, x=surveys, id_column=None):
-#         if survey_in == None:
-#             return self
-#         else:
-#             try:
-#                 get_extension = []
-#                 for j in survey_in:
-#                     for k in x[j]:
-#                         get_extension.append(k)
-#                 get_columns = []
-#                 for k in self.columns:
-#                     if "_"+k.split("_")[-1] in get_extension:
-#                         get_columns.append(k)
-#                 if id_column == None:
-#                     return self[get_columns]
-#                 else:
-#                     return self[[id_column]+get_columns]
-#             except:
-#                 print("error")
-
-#     def get_survey(self, survey=None):
-#         if survey == None:
-#             return self
-#         else:
-#             self = self.survey_filter(survey_in=[survey])
-#             self = self.survey_subset(survey_in=[survey])
-#             self.surveys = {key: value for key,
-#                             value in self.surveys.items() if key in [survey]}
-#             return self
-
-#     def merge_horizontal(self, other, set_index=None):
-#         surveys = {key: [] for key in list(
-#             set(self.surveys.keys()).union(set(other.surveys.keys())))}
-#         for j in surveys.keys():
-#             for k in (self.surveys, other.surveys):
-#                 if j in k.keys():
-#                     surveys[j] = surveys[j] + k[j]
-#             surveys[j] = list(set(surveys[j]))
-#         if set_index == None:
-#             output = self.join(other, how="outer")
-#         else:
-#             output = self.set_index(set_index).join(
-#                 other.set_index(set_index), how="other")
-#         output.surveys = surveys
-#         return output
-
-#     def merge_vertical(self, other, set_index=None):
-#         shared = list(set(self.columns).intersection(set(other.columns)))
-#         surveys = {key: [] for key in list(
-#             set(self.surveys.keys()).union(set(other.surveys.keys())))}
-#         for j in surveys.keys():
-#             for k in (self.surveys, other.surveys):
-#                 if j in k.keys():
-#                     surveys[j] = surveys[j] + k[j]
-#             surveys[j] = list(set(surveys[j]))
-#         if set_index == None:
-#             output = pd.concat(
-#                 [self[[i for i in self.columns if i in shared]], other[[i for i in other.columns if i in shared]]])
-#         else:
-#             output = pd.concat([self.set_index(set_index)[[i for i in self.columns if i in shared]], other.set_index(
-#                 set_index)[[i for i in other.columns if i in shared]]])
-#         output.surveys = surveys
-#         SurveyPlus.check_surveys(output)
-#         return output
+    if freeze_panes:
+        worksheet.freeze_panes(2, 0)
 
-class Form():
+    workbook.close()
+
+#%% #@ ODK Class
+
+class ODK():
 
     """
-    submissions
-    repeats
-    variable
-    time_variable
-    survey_name
-    choices
-    survey
+    The class is used to access the ODK server and download or upload data to projects.
+    class parameters:
+    url
+
+    class functions:\n
+    connect: connects to the webserver by providing username and password\n
+    set_target: defines the project and form to connect to\n
+    list_projects:\n
+    get_project:\n
+    list_forms:\n
+    get_form:\n
+    save_form:\n
+    save_data:\n
+    get_submissions:\n
+    survey:\n
+    choices:\n
+    get_repeats:\n
+    get_attachments:\n
+    processing_submission:\n
+    processing_repeats:\n
+    process_all:\n
+    save_main:\n
+    save_repeat:\n
+    listing_submissions:\n
+    get_submission_metadata:\n
+    get_submission_xml:\n
+    put_submission:\n
+    return_element:\n
+    modify_xml:\n
+    update_xml:\n
+    change_submission:\n
     """
 
-    def __init__(self, submissions, survey, choices, repeats, survey_name, variable, time_variable) -> None:
-        self.submissions =submissions
-        self.repeats = repeats
-        self.variable = variable
-        self.time_variable = time_variable
-        self.survey_name = survey_name
-        self.survey = survey
-        self.choices = choices
-
-    @property
-    def _constructor(self):
-        return Form
-
-    def filter_variable(self, x):
-        submissions = copy.copy(
-            self.submissions.loc[self.submissions[self.variable] == x])
-        set_not_rejected = list(submissions["KEY"])
-        reps =copy.copy(self.repeats)
-        for j in reps.keys():
-            reps[j] = reps[j].loc[[True if reps[j]["PARENT_KEY"].iloc[i].split("/")[0] in set_not_rejected else False for i in range(len(reps[j]))]]
-        return Form(submissions, repeats=reps, survey_name=self.survey_name, variable=self.variable, time_variable=self.time_variable, survey=self.survey, choices=self.choices)
-
-    def date_time_filter(
-            self,
-            time_start=None,
-            time_end=None,
-            date_start=None,
-            date_end=None,
-            day=None):
-        if date_start is not None:
-            submissions = copy.copy(self.submissions.loc[self.submissions[self.time_variable] >= date_start])
-        if date_end is not None:
-            submissions = copy.copy(self.submissions.loc[self.submissions[self.time_variable] <= date_end])
-        if (time_start is not None) & (time_end is not None):
-            if time_start > time_end:
-                submissions = copy.copy(self.submissions.loc[(self.submissions[self.time_variable].time >= time_start)
-                                | (self.submissions[self.time_variable].time < time_end)])
-            else:
-                submissions = copy.copy(self.submissions.loc[(self.submissions[self.time_variable].time >= time_start)
-                                & (self.submissions[self.time_variable].time < time_end)])
-        if (time_start is not None) & (time_end is None):
-            submissions = copy.copy(self.submissions.loc[self.submissions[self.time_variable].time >= time_start])
-        if (time_start is None) & (time_end is not None):
-            submissions = copy.copy(self.submissions.loc[self.submissions[self.time_variable].time <= time_end])
-
-        if day is not None:
-            submissions = copy.copy(self.submissions.loc[[a in day for a in [self.submissions[self.time_variable][i].date().isoweekday()
-                                                for i in range(len(self.submissions[self.time_variable]))]]])
-        set_not_rejected = list(submissions["KEY"])
-        reps = copy.copy(self.repeats)
-        for j in reps.keys():
-            reps[j] = reps[j].loc[[True if reps[j]["PARENT_KEY"].iloc[i].split(
-                "/")[0] in set_not_rejected else False for i in range(len(reps[j]))]]
-        return Form(submissions, repeats=reps, survey_name=self.survey_name, variable=self.variable, time_variable=self.time_variable, survey=self.survey, choices=self.choices)
-
-    def pdf_summary(self, directory=''):
-
-        def filter_text(s, filter=["""<span style="color:red">""", "</span>", "**"]):
-            for j in filter:
-                s = s.replace(j, "")
-            return s
-
-        def insert_newline(s):
-            if len(s) < 2:
-                return s[0]
-            else:
-                b = range(1, len(s))
-                for i in range(len(b)):
-                    s.insert(b[i]+i, "\n")
-                z = "".join(s)
-                return z
-
-        def group_text(s, no):
-            a = filter_text(s).split()
-            if len(a) < no:
-                return s
-            else:
-                b = [" ".join(a[x:x+no]) for x in range(0, len(a), no)]
-                return insert_newline(b)
+    def __init__(self, url):
+        self.url=url
 
-        def question_type(var, survey=self.survey):
-            return survey["type"].loc[survey["name"] == var].iloc[0].split()
+    def connect(self, email, password):
 
-        def reindex(input, var, choices=self.choices):
-            if question_type(var)[0] == "select_one":
-                selects = choices["label::English (en)"].loc[choices["list_name"]
-                                                            == question_type(var)[1]]
-                input = input.reindex(selects)
-            if question_type(var)[0] == "integer":
-                input = input.sort_index()
-            if question_type(var)[0] == "decimal":
-                input = input.sort_index()
-            if question_type(var)[0] == "select_multiple":
-                selects = choices["label::English (en)"].loc[choices["list_name"]
-                                                            == question_type(var)[1]]
-                input = input.reindex(selects)
-            return input
-
-        def multiprocess(series):
-            out = []
-            for j in series.index:
-                if not pd.isna(series[j]):
-                    step = series[j].split(" \n")
-                    for i in step:
-                        out.append(i)
-            out = pd.Series(out)
-            return (out)
-
-        def getIndexLength(var, data):
-            if question_type(var)[0] != "select_multiple":
-                a = data[var].loc[~data[var].isna()].value_counts()
-                a = reindex(a, var).fillna(0)
-            else:
-                a = multiprocess(data[var].loc[~data[var].isna()]).value_counts()
-                a = reindex(a, var).fillna(0)
-            return len(a.index)
-
-        def pie(ax, var, data, survey=self.survey, title_group=4, label_group=3):
-            if question_type(var)[0] != "select_multiple":
-                a = data[var].loc[~data[var].isna()].value_counts()
-                a = reindex(a, var).fillna(0)
-            else:
-                a = multiprocess(data[var].loc[~data[var].isna()]).value_counts()
-                a = reindex(a, var).fillna(0)
-            title = group_text(
-                survey["label::English (en)"].loc[survey["name"] == var].iloc[0], title_group)
-            labels = [group_text(str(i), label_group) for i in a.index]
-            if max(a, default=0) == 0:
-                ax.set_title(title)
-                ax.set_xlabel("(total="+str(a.sum())+")", labelpad=1)
-            else:
-                ax.pie(x=a.values, labels=labels,
-                    autopct=lambda x: '{:.0f}'.format(x*a.values.sum()/100))
-                ax.set_title(title)
-                ax.set_xlabel("(total="+str(a.sum())+")", labelpad=1)
-
-        def bar(ax, var, data, survey=self.survey, title_group=4, label_group=3):
-            if question_type(var)[0] != "select_multiple":
-                a = data[var].loc[~data[var].isna()].value_counts()
-                a = reindex(a, var).fillna(0)
-            else:
-                a = multiprocess(data[var].loc[~data[var].isna()]).value_counts()
-                a = reindex(a, var).fillna(0)
-            title = group_text(
-                survey["label::English (en)"].loc[survey["name"] == var].iloc[0], title_group)
-            label = [group_text(str(i), label_group) for i in a.index]
-            y = range(len(a))
-            width = a.values
-            if max(a, default=0) == 0:
-                ax.set_title(title)
-                ax.set_xlabel("Count (total="+str(a.sum())+")", labelpad=1)
-            else:
-                bars = ax.barh(y=y, width=width, tick_label=label)
-                ax.bar_label(bars)
-                ax.set_title(title)
-                ax.set_xlabel("Count (total="+str(a.sum())+")", labelpad=1)
-
-        def hist(ax, var, data, survey=self.survey, title_group=4, label_group=3):
-            a = data[var].loc[~data[var].isna()]
-            title = group_text(
-                survey["label::English (en)"].loc[survey["name"] == var].iloc[0], title_group)
-            if len(a) == 0:
-                ax.set_title(title)
-                ax.set_ylabel("Count", labelpad=1)
-                ax.set_xlabel("Participant's reply", labelpad=1)
-            else:
-                align = "mid"
-                ax.hist(x=a, align=align, bins=int(max(a)-min(a)+1),
-                        range=(min(a)-0.5, max(a)+0.5))
-                ax.set_title(title)
-                ax.set_ylabel("Count (total="+str(len(a))+")", labelpad=1)
-                ax.set_xlabel("Participant's reply", labelpad=1)
-
-        def inches(cm):
-            return cm/2.54
-
-        def fig_wrap(var, data, typ="bar", title_group=4, label_group=3, width=20, height=12):
-
-            indexLength = getIndexLength(var, data=data)
-            if indexLength > 7:
-                height = min(height + (height/7)*(indexLength-7), 27)
-
-            gs = gridspec.GridSpec(nrows=1, ncols=1)
-            fig = plt.figure(figsize=(inches(width)*gs.nrows,
-                                    inches(height)*gs.ncols))
-
-            for i in range(0, gs.nrows*gs.ncols):
-                ax = plt.subplot(gs[i//gs.ncols, i % gs.ncols])
-                if typ == "bar":
-                    bar(ax, var, data=data, title_group=title_group,
-                        label_group=label_group)
-                elif typ == "pie":
-                    pie(ax, var, data=data, title_group=title_group,
-                        label_group=label_group)
-                elif typ == "hist":
-                    hist(ax, var, data=data, title_group=title_group,
-                        label_group=label_group)
-            gs.tight_layout(fig)
-            b = BytesIO()
-            plt.savefig(b, format="png")
-            plt.close()
-            return b, height
-
-        pdf = FPDF()
-
-        pdf.add_page()
-        pdf.set_font('Arial', 'B', 20)
-        pdf.cell(w=210, txt=self.survey_name, align="C")
-        pdf.ln(h=20)
-        pdf.set_font('Arial', 'B', 12)
-        pdf.cell(w=210, txt='Total number of submissions = ' +
-                 str(len(self.submissions)), align="L")
-
-        pdf.add_page()
-        pdf.set_font('Arial', 'B', 16)
-
-        ty = ['select_one', 'select_multiple', 'integer']
-
-        print_dic = {self.survey['name'].iloc[j]: 'bar' for j in range(
-            len(self.survey)) if question_type(self.survey['name'].iloc[j])[0] in ty}
-
-        for i in print_dic.keys():
-            figu, figuHeight = fig_wrap(
-                i, data=self.submissions, typ=print_dic[i])
-
-            pdf.set_x(105-100)
-            pdf.image(figu, w=200, h=figuHeight*10)
-            pdf.ln(10)
-
-        pdf.output(directory+self.survey_name+'.pdf', 'F')
-
-    def add_headers(self, questions=True, variable=None):
-        df = self.submissions
-        repeats = self.repeats
-        survey = self.survey
+        self.email = email
+        self.password = password
 
-        if questions == True:
+        req = requests.post(self.url+'/v1/sessions', data=json.dumps(
+            {"email": self.email, "password": self.password}), headers={'Content-Type': 'application/json'})
+    
+        self.token = req.json()["token"]
+        self.headers = {'Authorization': 'Bearer '+self.token}
+
+    def set_target(self, project_name, form_name):
+        self.project_name = project_name
+        self.form_name = form_name
+
+    def list_projects(self):
+        req = requests.get(self.url+'/v1/projects', headers=self.headers)
+        projects = [req.json()[i]["name"] for i in range(len(req.json()))]
+        return projects
+
+    def get_project(self):
+        req = requests.get(self.url+'/v1/projects', headers=self.headers)
+        project = [req.json()[i]["id"] for i in range(len(req.json()))
+                if req.json()[i]["name"] == self.project_name][0]
+    
+        return project
+
+    def list_forms(self,project=None):
+        req = requests.get(self.url+'/v1/projects', headers=self.headers)
+        if project!=None:
+            project = [req.json()[i]["id"] for i in range(len(req.json())) if req.json()[i]["name"] == project][0]
+        else:
+            project = [req.json()[i]["id"] for i in range(
+                len(req.json())) if req.json()[i]["name"] == self.project_name][0]
+        req = requests.get(self.url+'/v1/projects/' +
+                           str(project)+"/forms", headers=self.headers)
+        forms = [req.json()[i]["name"] for i in range(len(req.json()))]
+        return forms
+
+    def get_form(self):
+
+        req = requests.get(self.url+'/v1/projects/' +
+                           str(self.get_project())+"/forms", headers=self.headers)
+        form = [req.json()[i]["xmlFormId"] for i in range(len(req.json())) if req.json()[i]["name"] == self.form_name][0]
+
+        return form
+
+    def save_form(self, xlsx="form",path=""):
+        
+        req = requests.get(self.url+'/v1/projects/'+str(self.get_project())+"/forms/"+self.get_form()+".xlsx", headers=self.headers).content
+        
+        version = str(pd.read_excel(BytesIO(req),
+                    sheet_name="settings")["version"].iloc[0])
+
+        file = open(path+xlsx+"_v"+version+".xlsx", "wb")
+        file.write(req)
+        file.close()
+
+    def save_data(self, path=""):
+        req = requests.get(self.url+'/v1/projects/'+str(self.get_project()) +
+                           "/forms/"+self.get_form()+".xlsx", headers=self.headers).content
+
+        version = str(pd.read_excel(BytesIO(req),
+                                    sheet_name="settings")["version"].iloc[0])
+        req = (requests.post(self.url+'/v1/projects/' +
+                         str(self.get_project())+"/forms/"+self.get_form()+"/submissions.csv.zip?",
+                         headers=self.headers))
+
+        file = open(path+self.form_name+"_v"+version+".zip", "wb")
+        file.write(req.content)
+        file.close()
+
+    def get_submissions(self):
+
+        req = (requests.get(self.url+'/v1/projects/' +
+                            str(self.get_project())+"/forms/"+self.get_form()+"/submissions.csv?",
+                            headers=self.headers))
+        df = pd.read_csv(BytesIO(req.content))
+        return df
+
+    def survey(self):
+        req = requests.get(self.url+'/v1/projects/'+str(self.get_project())+"/forms/"+self.get_form()+".xlsx", headers=self.headers)
+        survey = pd.read_excel(BytesIO(req.content))
+        return survey
+
+    def choices(self):
+        req = requests.get(self.url+'/v1/projects/'+str(self.get_project())+"/forms/"+self.get_form()+".xlsx", headers=self.headers)
+        choices = pd.read_excel(BytesIO(req.content), sheet_name="choices")
+        return choices
+    
+    def get_repeats(self):
+
+        survey = self.survey()
+        req = (requests.get(self.url+'/v1/projects/' +
+                            str(self.get_project())+"/forms/"+self.get_form()+"/submissions.csv.zip?attachments=false",
+                            headers=self.headers))
+        zipfile = zip.ZipFile(BytesIO(req.content))
+
+        repeats = {}
+
+        form_id = str(pd.read_excel(BytesIO(requests.get(self.url+'/v1/projects/'+str(self.get_project())+"/forms/"+self.get_form()+".xlsx", headers=self.headers).content),
+                    sheet_name="settings")["form_id"].iloc[0])
+        
+        for j in survey["name"].loc[survey["type"] == "begin_repeat"]:
+            repeats[form_id+"-" +j] = pd.read_csv(zipfile.open(form_id+"-" +j+".csv"))
+
+        return repeats
+
+    def get_attachments(self):
+
+        survey = self.survey()
+        req = (requests.get(self.url+'/v1/projects/' +
+                            str(self.get_project())+"/forms/"+self.get_form()+"/attachments",
+                            headers=self.headers))
+        
+        attachments = {}
+
+        for j in req.json():
+            attachments[j["name"]] = pd.read_csv(BytesIO((requests.get(self.url+'/v1/projects/' +str(self.get_project())+"/forms/"+self.get_form()+"/attachments/"+j["name"], headers=self.headers)).content))
+        return attachments
+
+    def processing_submission(self,process_datetimes=False):
+        survey = self.survey()
+        choices = self.choices()
+        df = self.get_submissions()
+
+        def remove_tail(list_in):
             a = []
-            for j in df.columns:
-                if j in list(survey["name"]):
-                    x = survey["label::English (en)"].loc[survey["name"]
-                                                          == j].iloc[0]
-                    a.append(x)
+            for j in list_in:
+                if j[-2:] == ".0":
+                    a.append(j[:-2])
                 else:
-                    a.append(np.nan)
-            df_out = copy.deepcopy(df)
-            df_out.loc[-1] = a
-            df_out.sort_index(inplace=True)
-
-            reps = copy.copy(repeats)
-            for k in reps.keys():
-                a = []
-                for j in reps[k].columns:
-                    if j in list(survey["name"]):
-                        x = survey["label::English (en)"].loc[survey["name"]
-                                                              == j].iloc[0]
-                        a.append(x)
-                    else:
-                        a.append(np.nan)
-                rep_out = copy.deepcopy(repeats[k])
-                rep_out.loc[-1] = a
-                rep_out.sort_index(inplace=True)
-                reps[k] = rep_out
+                    a.append(j)
+            return a
+
+
+        def select_one(select, value):
+            x = survey["type"].loc[survey["name"] == select].iloc[0].split(" ")[1]
+            y = choices["label::English (en)"].loc[choices["list_name"]
+                                                   == x].loc[choices["name"] == value].iloc[0]
+            return y
+
+
+        def select_multiple(select, value):
+            x = survey["type"].loc[survey["name"] == select].iloc[0].split(" ")[1]
+            y = choices.loc[choices["list_name"] == x]
+            z = []
+            for i in range(len(y)):
+                if str(y["name"].iloc[i]) in remove_tail(list(str(value).split(" "))):
+                    z.append(y["label::English (en)"].iloc[i])
+            return " \n".join(z)
+
+
+        def select_one_from_file(select, value):
+            x = survey["type"].loc[survey["name"] == select].iloc[0].split(" ")[1]
+            y = pd.read_csv(x)
+            z = y["label"].loc[y["name"] == value].iloc[0]
+            return z
 
-        if variable != None:
+
+        func = {"select_one_from_file": select_one_from_file,
+                "select_one": select_one, "select_multiple": select_multiple}
+
+        group_names = list(survey["name"].loc[survey["type"] == "begin_group"])
+        group_names = sorted(group_names, key=len, reverse=True)
+
+        column_names = sorted(list(set(survey["name"].loc[((survey["type"] != "begin_group") & (survey["type"] != "end_group") & (
+            survey["type"] != "begin_repeat") & (survey["type"] != "end_repeat"))]).difference(set([np.nan]))), key=len, reverse=True)
+
+
+        df_columns = sorted(list(df.columns), key=len, reverse=True)
+
+        for i in df_columns:
+            for j in column_names:
+                if i.endswith(j):
+                    df = df.rename(columns={i: j})
+
+        for i in df_columns:
+            for j in group_names:
+                if i.startswith(j):
+                    df = df.rename(columns={i: i[len(j):]})
+
+        for i in df.columns:
+            # try:
+            a = i
+            b = survey["type"].loc[survey["name"] == a]
+            if len(b) == 0:
+                pass
+            else:
+                b = b.iloc[0].split(" ")[0]
+                if b in list(func.keys()):
+                    for j in range(len(df)):
+                        if pd.isna(df[i].iloc[j]):
+                            pass
+                        else:
+                            try:
+                                df[i].iat[j] = func[b](a, df[i].iat[j])
+                            except:
+                                pass
+
+        df = df.loc[df["ReviewState"] != "rejected"]
+
+        if process_datetimes:
+            df["SubmissionDate"] = pd.to_datetime(
+                df["SubmissionDate"], format="%Y-%m-%dT%H:%M:%S.%fZ")
+            df["start"] = pd.to_datetime(df["start"], format="%Y-%m-%dT%H:%M:%S.%f%z")
+
+            for j in survey["name"].loc[survey["type"] == "datetime"]:
+                try:
+                    df[j] = pd.to_datetime(df[j], format="%Y-%m-%dT%H:%M:%S.%f%z")
+                except:
+                    df[j] = pd.to_datetime(df[j], format="mixed")
+
+            for j in survey["name"].loc[survey["type"] == "date"]:
+                df[j] = pd.to_datetime(df[j], format="%Y-%m-%d").dt.date
+
+            for j in survey["name"].loc[survey["type"] == "time"]:
+                df[j] = pd.to_datetime(df[j], format="%H:%M:%S.%f%z").dt.time
+        
+        
+        return df
+
+    def processing_repeats(self, data=None, process_datetimes=False):
+        survey = self.survey()
+        choices = self.choices()
+        repeats = self.get_repeats()
+        df = self.processing_submission() if type(data) == type(None) else data
+        set_not_rejected = list(df["KEY"])
+        def remove_tail(list_in):
             a = []
-            for j in df.columns:
+            for j in list_in:
+                if j[-2:] == ".0":
+                    a.append(j[:-2])
+                else:
+                    a.append(j)
+            return a
+
+        def select_one(select, value):
+            x = survey["type"].loc[survey["name"] == select].iloc[0].split(" ")[
+                1]
+            y = choices["label::English (en)"].loc[choices["list_name"]
+                                                   == x].loc[choices["name"] == value].iloc[0]
+            return y
+
+        def select_multiple(select, value):
+            x = survey["type"].loc[survey["name"] == select].iloc[0].split(" ")[
+                1]
+            y = choices.loc[choices["list_name"] == x]
+            z = []
+            for i in range(len(y)):
+                if str(y["name"].iloc[i]) in remove_tail(list(str(value).split(" "))):
+                    z.append(y["label::English (en)"].iloc[i])
+            return " \n".join(z)
+
+        def select_one_from_file(select, value):
+            x = survey["type"].loc[survey["name"] == select].iloc[0].split(" ")[
+                1]
+            y = pd.read_csv(x)
+            z = y["label"].loc[y["name"] == value].iloc[0]
+            return z
+
+        func = {"select_one_from_file": select_one_from_file,
+                "select_one": select_one, "select_multiple": select_multiple}
+
+        group_names = list(survey["name"].loc[survey["type"] == "begin_group"])
+        group_names = sorted(group_names, key=len, reverse=True)
+
+        column_names = sorted(list(set(survey["name"].loc[((survey["type"] != "begin_group") & (survey["type"] != "end_group") & (
+            survey["type"] != "begin_repeat") & (survey["type"] != "end_repeat"))]).difference(set([np.nan]))), key=len, reverse=True)
+
+
+        for k in repeats.keys():
+            for i in repeats[k].columns:
+                # try:
+                a = i
+                b = survey["type"].loc[survey["name"] == a]
+                if len(b) == 0:
+                    pass
+                else:
+                    b = b.iloc[0].split(" ")[0]
+                    if b in list(func.keys()):
+                        for j in range(len(repeats[k])):
+                            if pd.isna(repeats[k][i].iloc[j]):
+                                pass
+                            else:
+                                try:
+                                    repeats[k][i].iat[j] = func[b](
+                                        a, repeats[k][i].iat[j])
+                                except:
+                                    pass
+
+        for j in repeats.keys():
+
+            repeats[j] = repeats[j].loc[[True if repeats[j]["PARENT_KEY"].iloc[i].split(
+                "/")[0] in set_not_rejected else False for i in range(len(repeats[j]))]]
+            
+            if process_datetimes:
+
+                for i in survey["name"].loc[survey["type"] == "datetime"]:
+                    if i in repeats[j].columns:
+                        try:
+                            repeats[j][i] = pd.to_datetime(
+                                repeats[j][i], format="%Y-%m-%dT%H:%M:%S.%f%z")
+                        except:
+                            repeats[j][i] = pd.to_datetime(
+                                repeats[j][i], format="mixed")
+
+                for i in survey["name"].loc[survey["type"] == "date"]:
+                    if i in repeats[j].columns:
+                        repeats[j][i] = pd.to_datetime(
+                            repeats[j][i], format="%Y-%m-%d").dt.date
+
+                for i in survey["name"].loc[survey["type"] == "time"]:
+                    if i in repeats[j].columns:
+                        repeats[j][i] = pd.to_datetime(
+                            repeats[j][i], format="%H:%M:%S.%f%z").dt.time
+
+        return repeats
+
+    def process_all(self,variable='',time_variable='starttime'):
+
+        submissions = self.processing_submission()
+        survey = self.survey().dropna(how='all')
+        choices = self.choices()
+        repeats = self.processing_repeats()
+        survey_name = self.form_name
+        variable = variable
+        time_variable = time_variable
+
+        return Form(submissions,survey,choices,repeats,survey_name,variable,time_variable)
+
+    def save_main(self,data=None,path=""):
+
+        df = self.processing_submission() if type(data) == type(None) else data
+        survey = self.survey()
+        a = []
+        for j in df.columns:
+            if j in list(survey["name"]):
+                x = survey["label::English (en)"].loc[survey["name"] == j].iloc[0]
+                a.append(x)
+            else:
+                a.append(np.nan)
+
+        df_out = copy.deepcopy(df)
+
+        df_out.loc[-1] = a
+
+        df_out.sort_index(inplace=True)
+
+        save_to_excel(df_out, path+self.form_name+"_submissions.xlsx")
+
+    def save_repeat(self,data=None, path=""):
+        repeats = self.processing_repeats() if type(data) == type(None) else data
+        survey = self.survey()
+
+        for k in repeats.keys():
+            a = []
+            for j in repeats[k].columns:
                 if j in list(survey["name"]):
-                    x = survey[variable].loc[survey["name"]
-                                                          == j].iloc[0]
+                    x = survey["label::English (en)"].loc[survey["name"] == j].iloc[0]
                     a.append(x)
                 else:
                     a.append(np.nan)
-            if not questions:
-                df_out = copy.deepcopy(df)
-                df_out.loc[-1] = a
-                df_out.sort_index(inplace=True)
+
+            rep_out = copy.deepcopy(repeats[k])
+
+            rep_out.loc[-1] = a
+
+            rep_out.sort_index(inplace=True)
+
+            save_to_excel(rep_out, path+k+".xlsx")
+
+    def listing_submissions(self):
+        req = (requests.get(self.url+'/v1/projects/' +
+                            str(self.get_project())+"/forms/"+self.get_form()+"/submissions",
+                            headers=self.headers))
+        return req.json()
+
+    def get_submission_metadata(self,instance):
+        req = (requests.get(self.url+'/v1/projects/' +
+                            str(self.get_project())+"/forms/" +
+                            self.get_form()+"/submissions/"+instance,
+                            headers=self.headers))
+        return req.json()
+    
+    def get_submission_xml(self,instance):
+        req = (requests.get(self.url+'/v1/projects/' +
+                            str(self.get_project())+"/forms/" +
+                            self.get_form()+"/submissions/"+instance+".xml",
+                            headers=self.headers))
+        return req.content
+
+    def put_submission(self, instance, data):
+        req = (requests.put(url=self.url+'/v1/projects/' +
+                            str(self.get_project())+"/forms/" +
+                            self.get_form()+"/submissions/"+instance,data=data,
+                            headers=self.headers))
+        return req
+
+    def return_element(self,tree, data: str):
+        for elem in tree.iter():
+            if elem.tag == data:
+                return elem
             else:
-                df_out.loc[-2] = a
-                df_out.sort_index(inplace=True)
+                pass
+        return None
 
-            if not questions:
-                reps = copy.copy(repeats)
-            for k in reps.keys():
-                a = []
-                for j in reps[k].columns:
-                    if j in list(survey["name"]):
-                        x = survey[variable].loc[survey["name"]
-                                                              == j].iloc[0]
-                        a.append(x)
-                    else:
-                        a.append(np.nan)
-                if not questions:
-                    rep_out = copy.deepcopy(reps[k])
-                    rep_out.loc[-1] = a
-                    rep_out.sort_index(inplace=True)
-                else:
-                    rep_out.loc[-2] = a
-                    rep_out.sort_index(inplace=True)
-                reps[k] = rep_out
-
-
-        if variable == None:
-            new_labels = pd.MultiIndex.from_arrays(
-                [df_out.columns, df_out.iloc[0]], names=['code', 'question'])
-            df_out = df_out.set_axis(new_labels, axis=1).iloc[1:]
-            for k in reps.keys():
-                new_labels = pd.MultiIndex.from_arrays(
-                    [reps[k].columns, reps[k].iloc[0]], names=['code', 'question'])
-                reps[k] = reps[k].set_axis(new_labels, axis=1).iloc[1:]
-        elif not questions:
-            new_labels = pd.MultiIndex.from_arrays(
-                [df_out.columns, df_out.iloc[0]], names=['code', 'variable'])
-            df_out = df_out.set_axis(new_labels, axis=1).iloc[1:]
-            for k in reps.keys():
-                new_labels = pd.MultiIndex.from_arrays(
-                    [reps[k].columns, reps[k].iloc[0]], names=['code', 'variable'])
-                reps[k] = reps[k].set_axis(new_labels, axis=1).iloc[1:]
+    def modify_xml(self, xml, variable: str, function):
+            
+        tree = ET.parse(BytesIO(xml))
+        d = self.return_element(tree,variable)
+        if d == None:
+            return xml
         else:
-            new_labels = pd.MultiIndex.from_arrays(
-                [df_out.columns, df_out.iloc[0], df_out.iloc[1]], names=['code', 'variable','question'])
-            df_out = df_out.set_axis(new_labels, axis=1).iloc[2:]
-            for k in reps.keys():
-                new_labels = pd.MultiIndex.from_arrays(
-                    [reps[k].columns, reps[k].iloc[0],reps[k].iloc[1]], names=['code', 'variable','question'])
-                reps[k] = reps[k].set_axis(new_labels, axis=1).iloc[2:]
+            try:
+                k = d.text
+                d.text = function(k)
+                xml_out = BytesIO()
+                tree.write(xml_out, encoding='utf-8')
+                return xml_out.getvalue()
+            except:
+                print('an error occurred while processing for variable ', variable)
+                return xml
+
+    def update_xml(self, xml):
+
+        tree = ET.parse(BytesIO(xml))
+        root = tree.getroot()
+      
+        if tree.find('meta').find('deprecatedID') == None:
+            old = tree.find('meta').find('instanceID').text
+            tree.find('meta').find(
+                'instanceID').text = 'uuid:'+str(uuid.uuid4())
+            deprecated = ET.Element("deprecatedID")
+            deprecated.text = old
+            root.find('meta').append(deprecated)
 
-
-        return Form(submissions=df_out, repeats=reps, survey=survey, survey_name=self.survey_name, variable=self.variable, time_variable=self.time_variable,  choices=self.choices)
+        else:
+            if len(tree.find('meta').find('deprecatedID').text)>0:
+                old = tree.find('meta').find('instanceID').text
+                tree.find('meta').find('instanceID').text = 'uuid:'+str(uuid.uuid4())
+                root.find('meta').find('deprecatedID').text = old
+        xml_out = BytesIO()
+        tree.write(xml_out, encoding='utf-8')
+        return xml_out.getvalue()
+
+    def change_submission(self, variable: str | list[str], id, project=None, form=None, func: FunctionType = lambda x: x | list[FunctionType]):
+        if (project != None) | (form != None):
+            self.set_target(project, form)
+        if type(variable) == str:
+            c = self.get_submission_xml(id)
+            ff = self.modify_xml(c, variable, func)
+            self.put_submission(id, self.update_xml(ff))
+        else:
+            c = self.get_submission_xml(id)
+            for i in range(len(variable)):
+                c = self.modify_xml(c, variable[i], func[i])
+            self.put_submission(id, self.update_xml(c))
```

### Comparing `odk_tools-0.1.8/src/odk_tools/functions.py` & `odk_tools-0.1.9/src/odk_tools/functions.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     if type(subs.columns) == pd.core.indexes.base.Index:
         if len(reps) == 0:
             subs = subs.set_index('KEY', drop=False)
             return subs
         else:
             subs = subs.set_index('KEY', drop=False)
             out = subs.join(other=[value.set_index('PARENT_KEY').rename(columns={
-                            'KEY': 'KEY'+key.split('-')[-1]}) for key, value in reps.items()], how='outer', validate='one_to_many')
+                            'KEY': 'KEY'+key.split('-')[-1]}) for key, value in reps.items() if len(value)>0], how='outer', validate='one_to_many')
             drops = []
             for j in range(len(out.columns)):
                 a = out.columns[j]
                 for i in range(len(out.columns)):
                     b = out.columns[i]
                     if (a[:-2] == b[:-2]) & (a[-2:] == '_x') & (b[-2:] == '_y'):
                         out[a] = out[b]
@@ -33,17 +33,18 @@
         if len(reps) == 0:
             subs = subs.set_index('KEY', drop=False)
             return subs
         else:
             subs = subs.set_index('KEY', drop=False)
             out = subs
             for key,value in reps.items():
-                middle = out.join(value.set_index('PARENT_KEY').rename(columns={
-                    'KEY': 'KEY'+key.split('-')[-1]}, level='code'), how='outer', lsuffix='_x', rsuffix='_y')
-                out = middle
+                if len(value)>0:
+                    middle = out.join(value.set_index('PARENT_KEY').rename(columns={
+                        'KEY': 'KEY'+key.split('-')[-1]}, level='code'), how='outer', lsuffix='_x', rsuffix='_y')
+                    out = middle
             drops = []
             for j in range(len(out.columns.get_level_values('code'))):
                 a = out.columns.get_level_values('code')[j]
                 for i in range(len(out.columns.get_level_values('code'))):
                     b = out.columns.get_level_values('code')[i]
                     if (a[:-2] == b[:-2]) & (a[-2:] == '_x') & (b[-2:] == '_y'):
                         out[a] = out[b]
```

### Comparing `odk_tools-0.1.8/LICENSE` & `odk_tools-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `odk_tools-0.1.8/pyproject.toml` & `odk_tools-0.1.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "odk_tools"
-version = "0.1.8"
+version = "0.1.9"
 authors = [
   { name="Federico Lorenzetti", email="lorenzetti.federico@gmail.com" },
 ]
 description = "A collection of tools for interacting with an ODK server and uploading/downloading submissions"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `odk_tools-0.1.8/PKG-INFO` & `odk_tools-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: odk_tools
-Version: 0.1.8
+Version: 0.1.9
 Summary: A collection of tools for interacting with an ODK server and uploading/downloading submissions
 Project-URL: Homepage, https://github.com/federlorenz/odk_tools
 Author-email: Federico Lorenzetti <lorenzetti.federico@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

