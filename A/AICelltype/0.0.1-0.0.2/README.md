# Comparing `tmp/aicelltype-0.0.1.tar.gz` & `tmp/aicelltype-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aicelltype-0.0.1.tar", last modified: Sun May  5 16:41:25 2024, max compression
+gzip compressed data, was "aicelltype-0.0.2.tar", last modified: Mon May  6 09:31:10 2024, max compression
```

## Comparing `aicelltype-0.0.1.tar` & `aicelltype-0.0.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-05-05 16:41:25.697567 aicelltype-0.0.1/
--rw-rw-rw-   0        0        0        0 2024-02-03 13:10:46.000000 aicelltype-0.0.1/LICENSE
--rw-rw-rw-   0        0        0        0 2024-02-03 13:12:25.000000 aicelltype-0.0.1/MANIFEST.in
--rw-rw-rw-   0        0        0      727 2024-05-05 16:41:25.697567 aicelltype-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      120 2024-05-05 16:01:16.000000 aicelltype-0.0.1/README.md
--rw-rw-rw-   0        0        0      684 2024-05-05 14:34:53.000000 aicelltype-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-05 16:41:25.697567 aicelltype-0.0.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-05-05 16:41:25.675433 aicelltype-0.0.1/src/
-drwxrwxrwx   0        0        0        0 2024-05-05 16:41:25.675433 aicelltype-0.0.1/src/AICelltype/
--rw-rw-rw-   0        0        0     5009 2024-05-05 16:41:08.000000 aicelltype-0.0.1/src/AICelltype/__init__.py
--rw-rw-rw-   0        0        0       21 2024-05-05 04:52:48.000000 aicelltype-0.0.1/src/AICelltype/aicelltype.py
-drwxrwxrwx   0        0        0        0 2024-05-05 16:41:25.697567 aicelltype-0.0.1/src/AICelltype.egg-info/
--rw-rw-rw-   0        0        0      727 2024-05-05 16:41:25.000000 aicelltype-0.0.1/src/AICelltype.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      305 2024-05-05 16:41:25.000000 aicelltype-0.0.1/src/AICelltype.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-05 16:41:25.000000 aicelltype-0.0.1/src/AICelltype.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       35 2024-05-05 16:41:25.000000 aicelltype-0.0.1/src/AICelltype.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2024-05-05 16:41:25.000000 aicelltype-0.0.1/src/AICelltype.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      490 2024-02-03 13:12:00.000000 aicelltype-0.0.1/src/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-06 09:31:10.047422 aicelltype-0.0.2/
+-rw-rw-rw-   0        0        0        0 2024-02-03 13:10:46.000000 aicelltype-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0        0 2024-02-03 13:12:25.000000 aicelltype-0.0.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     3600 2024-05-06 09:31:10.045400 aicelltype-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     3120 2024-05-06 09:21:04.000000 aicelltype-0.0.2/README.md
+-rw-rw-rw-   0        0        0      575 2024-05-06 09:31:03.000000 aicelltype-0.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-06 09:31:10.047422 aicelltype-0.0.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-06 09:31:10.015419 aicelltype-0.0.2/src/
+drwxrwxrwx   0        0        0        0 2024-05-06 09:31:10.021402 aicelltype-0.0.2/src/AICelltype/
+-rw-rw-rw-   0        0        0     6502 2024-05-06 08:50:43.000000 aicelltype-0.0.2/src/AICelltype/__init__.py
+-rw-rw-rw-   0        0        0       21 2024-05-05 04:52:48.000000 aicelltype-0.0.2/src/AICelltype/aicelltype.py
+drwxrwxrwx   0        0        0        0 2024-05-06 09:31:10.044400 aicelltype-0.0.2/src/AICelltype.egg-info/
+-rw-rw-rw-   0        0        0     3600 2024-05-06 09:31:09.000000 aicelltype-0.0.2/src/AICelltype.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      305 2024-05-06 09:31:09.000000 aicelltype-0.0.2/src/AICelltype.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-06 09:31:09.000000 aicelltype-0.0.2/src/AICelltype.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       35 2024-05-06 09:31:09.000000 aicelltype-0.0.2/src/AICelltype.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2024-05-06 09:31:09.000000 aicelltype-0.0.2/src/AICelltype.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      490 2024-02-03 13:12:00.000000 aicelltype-0.0.2/src/__init__.py
```

### Comparing `aicelltype-0.0.1/pyproject.toml` & `aicelltype-0.0.2/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 [project]
 name = "AICelltype"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name = "renzhg", email = "rzgedu@163.com" },
 ]
 dependencies = ['dashscope==1.17.1', 'requests==2.31.0']
-description = "AICelltype: Annotate cell type through AI/LLM/GPT"
+description = "AICelltype: Annotate cell type through gpt-4 without openai_key."
 readme = "README.md"
 requires-python = ">=3.10.0"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project.urls]
-"Homepage" = "https://github.com/renzhonggan/AICelltype"
-"Bug Tracker" = "https://github.com/renzhonggan/AICelltype/issues"
+
```

### Comparing `aicelltype-0.0.1/src/AICelltype/__init__.py` & `aicelltype-0.0.2/src/AICelltype/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -10,40 +10,67 @@
 import dashscope
 
 dashscope.api_key = os.environ.get('QWEN_KEY', '')
 API_KEY = os.environ.get('API_KEY', '')
 SECRET_KEY = os.environ.get('SECRET_KEY', '')
 
 
-def aicelltype(issue_name, gene_list, model='gpt4'):
+def aicelltype(tissue_name, gene_list, model='gpt4'):
+    """
+    Parameters
+    ----------
+    tissue_name
+        In theory, issue_name can be any type of biological tissue.
+    gene_list
+        Identify one cell type for each row in gene_lt.
+    model
+        model should be chosen from ['gpt4', 'qwen-max', 'ERNIE-4.0'].
+        gpt4: annotate cell type through gpt4 (default);
+        qwen-max: annotate cell type through ali qwen model, QWEN_KEY needed, refer to https://help.aliyun.com/zh/dashscope/developer-reference/activate-dashscope-and-create-an-api-key for a key;
+        ERNIE-4.0: annotate cell type through  baidu qianfan model, API_KEY and SECRET_KEY, refer to https://console.bce.baidu.com/qianfan/ais/console/applicationConsole/application for them.
+
+    usage:
+        issue_name = 'human prostate'
+        gene_lt = [
+            ['KLK3', 'KRT8', 'KLK2', 'MSMB', 'ACPP', 'KLK1', 'KLK4'],
+            ['MMRN1', 'FLT4', 'RELN', 'CCL21', 'PROX1', 'LYVE1'],
+            ['CD69', 'IL7R', 'CD3D', 'CD3E', 'CD3G', 'ACTA2', 'MYO1B', 'ACTA2', 'ANPEP', 'PDGFRB', 'CSPG4'],
+            ['DDX49', 'LOC105371196', 'MTND1P30', 'LOC105373682', 'TAGLN2', 'ZNF836', 'ZNF677', 'COILP1']
+        ]
+
+        from AICelltype import aicelltype
+        cell_lt = aicelltype(issue_name, gene_lt, model='gpt4')
+        print(cell_lt)
+    output:
+        ['Prostate Epithelial Cells', 'Lymphatic Endothelial Cells', 'T Cell and Myofibroblast', 'Unknown Cell Type']
+        In result, you can get a list with four cell types which have the same order with parameter gene_list.
+    """
     if model == 'gpt4':
-        cell_lt = gpt4(issue_name, gene_list)
+        cell_lt = gpt4(tissue_name, gene_list)
     elif model == 'qwen-max':
-        # print(dashscope.api_key)
-        cell_lt = qwen(issue_name, gene_list)
+        cell_lt = qwen(tissue_name, gene_list)
     elif model == 'ERNIE-4.0':
-        # print(API_KEY, SECRET_KEY)
-        cell_lt = ernie(issue_name, gene_list)
+        cell_lt = ernie(tissue_name, gene_list)
     else:
         print(f'error:model {model} no found, choose one from ["gpt4", "qwen-max", "ERNIE-4.0"]')
         return
     return cell_lt
 
 
-def gpt4(issue_name, gene_list):
+def gpt4(tissue_name, gene_list):
     token_js = get_token()
     gene_str = '\n'.join([','.join(i) for i in gene_list])
     url = 'https://gq86p6-3000.csb.app/api/sydney'
     data = {
         "conversationId": token_js['conversationId'],
         "encryptedconversationsignature": token_js['encryptedconversationsignature'],
         "clientId": token_js['clientId'],
         "invocationId": 0,
         "conversationStyle": "Precise",
-        "prompt": f"Identify cell types of {issue_name} cells using the following markers. Identify one cell type for each row. Only print the cell type name without any markdown code. Some could be a mixture of multiple cell types. Some could be unknown cell types.\n{gene_str}",
+        "prompt": f"Identify cell types of {tissue_name} cells using the following markers. Identify one cell type for each row. Only print the cell type name without any markdown code. Some could be a mixture of multiple cell types. Some could be unknown cell types.\n{gene_str}",
         "allowSearch": "false",
         "context": ""
     }
     response = requests.post(url, json=data)
     if response.status_code == 200:
         result = response.text
         print("success:", response.status_code)
@@ -57,17 +84,17 @@
 
 def get_token():
     url = 'https://gq86p6-3000.csb.app/api/create'
     response = requests.post(url, data={})
     return response.json()
 
 
-def qwen(issue_name, gene_list):
+def qwen(tissue_name, gene_list):
     gene_str = '\n'.join([','.join(i) for i in gene_list])
-    input_msg = f'Identify cell types of {issue_name} cells using the following markers. Identify one cell type for each row. Only provide the cell type name and nothing else. Some could be a mixture of multiple cell types. Some could be unknown cell types.\n{gene_str}'
+    input_msg = f'Identify cell types of {tissue_name} cells using the following markers. Identify one cell type for each row. Only provide the cell type name and nothing else. Some could be a mixture of multiple cell types. Some could be unknown cell types.\n{gene_str}'
     # print(input_msg)
     messages = [{'role': 'user', 'content': input_msg}]
     response = Generation.call("qwen-max",
                                messages=messages,
                                result_format='message',
                               )
     if response.status_code == HTTPStatus.OK:
@@ -79,17 +106,17 @@
         print('Request id: %s, Status code: %s, error code: %s, error message: %s' % (
             response.request_id, response.status_code,
             response.code, response.message
         ))
         return [''] * len(gene_list)
 
 
-def ernie(issue_name, gene_list):
+def ernie(tissue_name, gene_list):
     gene_str = '\n'.join([','.join(i) for i in gene_list])
-    input_msg = f'Identify cell types of {issue_name} cells using the following markers. Identify one cell type for each row. Only provide the cell type name and nothing else. Some could be a mixture of multiple cell types. Some could be unknown cell types.\n{gene_str}'
+    input_msg = f'Identify cell types of {tissue_name} cells using the following markers. Identify one cell type for each row. Only provide the cell type name and nothing else. Some could be a mixture of multiple cell types. Some could be unknown cell types.\n{gene_str}'
     # print(input_msg)
     # print('token', get_access_token())
     url = "https://aip.baidubce.com/rpc/2.0/ai_custom/v1/wenxinworkshop/chat/ernie-4.0-8k-preview?access_token=" + get_access_token()
     payload = json.dumps({
         "messages": [
             {
                 "role": "user",
```

