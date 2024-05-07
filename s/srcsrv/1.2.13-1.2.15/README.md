# Comparing `tmp/srcsrv-1.2.13.tar.gz` & `tmp/srcsrv-1.2.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "srcsrv-1.2.13.tar", last modified: Sun Apr 28 00:43:33 2024, max compression
+gzip compressed data, was "srcsrv-1.2.15.tar", last modified: Tue May  7 05:43:54 2024, max compression
```

## Comparing `srcsrv-1.2.13.tar` & `srcsrv-1.2.15.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxrwx   0        0        0        0 2024-04-28 00:43:33.835469 srcsrv-1.2.13/
--rw-rw-rw-   0        0        0     1069 2022-08-20 22:38:23.000000 srcsrv-1.2.13/LICENSE
--rw-rw-rw-   0        0        0    14500 2024-04-28 00:43:33.831522 srcsrv-1.2.13/PKG-INFO
--rw-rw-rw-   0        0        0    13978 2024-04-26 16:19:46.000000 srcsrv-1.2.13/README.md
--rw-rw-rw-   0        0        0       42 2024-04-28 00:43:33.838240 srcsrv-1.2.13/setup.cfg
--rw-rw-rw-   0        0        0     2582 2024-04-28 00:38:01.000000 srcsrv-1.2.13/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-28 00:43:33.742861 srcsrv-1.2.13/srcsrv/
--rw-rw-rw-   0        0        0     1275 2023-09-14 12:28:57.000000 srcsrv-1.2.13/srcsrv/__init__.py
--rw-rw-rw-   0        0        0    14634 2024-03-01 07:11:59.000000 srcsrv-1.2.13/srcsrv/__main__.py
--rw-rw-rw-   0        0        0     6391 2024-03-01 07:11:59.000000 srcsrv-1.2.13/srcsrv/indexer.py
--rw-rw-rw-   0        0        0     7683 2024-04-28 00:38:01.000000 srcsrv-1.2.13/srcsrv/pdb.py
-drwxrwxrwx   0        0        0        0 2024-04-28 00:43:33.775724 srcsrv-1.2.13/srcsrv/plugins/
--rw-rw-rw-   0        0        0     1349 2023-09-14 12:28:57.000000 srcsrv-1.2.13/srcsrv/plugins/__init__.py
--rw-rw-rw-   0        0        0    10631 2024-03-01 07:11:59.000000 srcsrv-1.2.13/srcsrv/plugins/bitbucket.py
--rw-rw-rw-   0        0        0     8788 2024-03-01 07:11:59.000000 srcsrv-1.2.13/srcsrv/plugins/codebase.py
--rw-rw-rw-   0        0        0     8250 2024-03-01 07:11:59.000000 srcsrv-1.2.13/srcsrv/plugins/github.py
--rw-rw-rw-   0        0        0    10106 2024-03-01 07:11:59.000000 srcsrv-1.2.13/srcsrv/plugins/gitlab.py
--rw-rw-rw-   0        0        0     6801 2023-09-14 12:28:57.000000 srcsrv-1.2.13/srcsrv/plugins/plugin.py
-drwxrwxrwx   0        0        0        0 2024-04-28 00:43:33.783131 srcsrv-1.2.13/srcsrv/tools/
--rw-rw-rw-   0        0        0     1156 2023-09-14 12:28:57.000000 srcsrv-1.2.13/srcsrv/tools/__init__.py
--rw-rw-rw-   0        0        0     3681 2023-09-14 12:28:57.000000 srcsrv-1.2.13/srcsrv/tools/api.py
-drwxrwxrwx   0        0        0        0 2024-04-28 00:43:33.790975 srcsrv-1.2.13/srcsrv/utils/
--rw-rw-rw-   0        0        0     4484 2024-03-01 07:11:59.000000 srcsrv-1.2.13/srcsrv/utils/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-28 00:43:33.817676 srcsrv-1.2.13/srcsrv.egg-info/
--rw-rw-rw-   0        0        0    14500 2024-04-28 00:43:33.000000 srcsrv-1.2.13/srcsrv.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      498 2024-04-28 00:43:33.000000 srcsrv-1.2.13/srcsrv.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-28 00:43:33.000000 srcsrv-1.2.13/srcsrv.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       25 2024-04-28 00:43:33.000000 srcsrv-1.2.13/srcsrv.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-04-28 00:43:33.000000 srcsrv-1.2.13/srcsrv.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-07 05:43:54.728567 srcsrv-1.2.15/
+-rw-rw-rw-   0        0        0     1069 2022-08-20 22:38:23.000000 srcsrv-1.2.15/LICENSE
+-rw-rw-rw-   0        0        0    14742 2024-05-07 05:43:54.721205 srcsrv-1.2.15/PKG-INFO
+-rw-rw-rw-   0        0        0    14243 2024-05-07 05:33:22.000000 srcsrv-1.2.15/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-07 05:43:54.729600 srcsrv-1.2.15/setup.cfg
+-rw-rw-rw-   0        0        0     2582 2024-05-07 05:33:22.000000 srcsrv-1.2.15/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-07 05:43:54.601426 srcsrv-1.2.15/srcsrv/
+-rw-rw-rw-   0        0        0     1275 2023-09-14 12:28:57.000000 srcsrv-1.2.15/srcsrv/__init__.py
+-rw-rw-rw-   0        0        0    14634 2024-03-01 07:11:59.000000 srcsrv-1.2.15/srcsrv/__main__.py
+-rw-rw-rw-   0        0        0     6391 2024-03-01 07:11:59.000000 srcsrv-1.2.15/srcsrv/indexer.py
+-rw-rw-rw-   0        0        0     7683 2024-04-28 00:38:01.000000 srcsrv-1.2.15/srcsrv/pdb.py
+drwxrwxrwx   0        0        0        0 2024-05-07 05:43:54.640175 srcsrv-1.2.15/srcsrv/plugins/
+-rw-rw-rw-   0        0        0     1349 2023-09-14 12:28:57.000000 srcsrv-1.2.15/srcsrv/plugins/__init__.py
+-rw-rw-rw-   0        0        0    10631 2024-03-01 07:11:59.000000 srcsrv-1.2.15/srcsrv/plugins/bitbucket.py
+-rw-rw-rw-   0        0        0     8802 2024-05-07 05:33:22.000000 srcsrv-1.2.15/srcsrv/plugins/codebase.py
+-rw-rw-rw-   0        0        0     8269 2024-05-07 05:33:22.000000 srcsrv-1.2.15/srcsrv/plugins/github.py
+-rw-rw-rw-   0        0        0    10130 2024-05-07 05:33:22.000000 srcsrv-1.2.15/srcsrv/plugins/gitlab.py
+-rw-rw-rw-   0        0        0     6801 2023-09-14 12:28:57.000000 srcsrv-1.2.15/srcsrv/plugins/plugin.py
+drwxrwxrwx   0        0        0        0 2024-05-07 05:43:54.646702 srcsrv-1.2.15/srcsrv/tools/
+-rw-rw-rw-   0        0        0     1156 2023-09-14 12:28:57.000000 srcsrv-1.2.15/srcsrv/tools/__init__.py
+-rw-rw-rw-   0        0        0     3681 2023-09-14 12:28:57.000000 srcsrv-1.2.15/srcsrv/tools/api.py
+drwxrwxrwx   0        0        0        0 2024-05-07 05:43:54.646702 srcsrv-1.2.15/srcsrv/utils/
+-rw-rw-rw-   0        0        0     4484 2024-03-01 07:11:59.000000 srcsrv-1.2.15/srcsrv/utils/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-07 05:43:54.709018 srcsrv-1.2.15/srcsrv.egg-info/
+-rw-rw-rw-   0        0        0    14742 2024-05-07 05:43:54.000000 srcsrv-1.2.15/srcsrv.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      498 2024-05-07 05:43:54.000000 srcsrv-1.2.15/srcsrv.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-07 05:43:54.000000 srcsrv-1.2.15/srcsrv.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       25 2024-05-07 05:43:54.000000 srcsrv-1.2.15/srcsrv.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-05-07 05:43:54.000000 srcsrv-1.2.15/srcsrv.egg-info/top_level.txt
```

### Comparing `srcsrv-1.2.13/LICENSE` & `srcsrv-1.2.15/LICENSE`

 * *Files identical despite different names*

### Comparing `srcsrv-1.2.13/PKG-INFO` & `srcsrv-1.2.15/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: srcsrv
-Version: 1.2.13
+Version: 1.2.15
 Summary: Source indexing package
 Home-page: https://github.com/urielmann/srcsrv-public
 Author: Uri Mann
 Author-email: abba.mann@gmail.com
 License: MIT
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Development Status :: 4 - Beta
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -126,28 +125,28 @@
 
 # Plugins
 Each plugin has unique name of an environment variable containing the authentication used to connect to the remote repository. The value stored in the environment variable will be evaluated as python language expression. It is expected to be in one of three types. See more information in the plugins section.  
 >1. Dictionary (*dict*) entry which is interpreted as HTTPS Authorization header (e.g., *{'Authorization':'Bearer &lt;token&gt;'}*).  
 >2. Tuple (*tuple*) value which in interpreted as HTTPS basic authentication (e.g., *('&lt;account&gt;','&lt;password&gt;')*).  
 >3. The value is missing or *None* to indicate no authentication is required by the remote repository.  
 ## Github options
->**-u**, **--account** - User's account.  
+>**-u**, **--account** - User's account (default: *%SRCSRV_USERNAME%*).  
 >**-r**, **--repo** - Github repository name.  
 ## Github environment
 >**SRCSRV_GITHUB_AUTH** - User [token](https://help.github.com/en/github/authenticating-to-github/creating-a-personal-access-token-for-the-command-line) This is expected to be the string in the format of *{'Authorization':'Token &lt;token&gt;'}*. The value is evaluated as a python language expression.  
 
 ## Bitbucket options
 >**-i**, **--api** - Version of [Bitbucket REST API](https://docs.atlassian.com/bitbucket-server/rest/latest/bitbucket-rest.html) used. The default is *2.0*.  
 >**-t**, **--project-key** - Project key name.  
 >**-r**, **--repo-slug** - Repository slug name.  
 ## Bitbucket environment
 >**SRCSRV_BITBUCKET_AUTH** - User [token](https://developer.atlassian.com/cloud/bitbucket/rest/intro/#authentication_old). This is expected to be the string in the format of *{'Authorization':'Bearer &lt;token&gt;'}*. The value is evaluated as a python language expression.  
 
 ## Gitlab options
->**-u**, **--account** - User's account.  
+>**-u**, **--account** - User's account (default: *%SRCSRV_USERNAME%*).  
 >**-t**, **--project-id** - Project id value.  
 <!--
 @TODO:
 >**-S**, **--sudo** - Gitlab repository sudo account name.  
 -->
 >**-i**, **--api** - Version of [Gitlab REST API](https://docs.gitlab.com/ee/api/rest/) used. The default is *v4*.
 ## Gitlab environment
@@ -155,15 +154,15 @@
 . It may be one of three token types.  
 >1. [Personal access tokens](https://docs.gitlab.com/ee/user/profile/personal_access_tokens.html).  
 >2. [Project access tokens](https://docs.gitlab.com/ee/user/project/settings/project_access_tokens.html)
 >3. [Group access tokens](https://docs.gitlab.com/ee/user/group/settings/group_access_tokens.html)
   
 
 ## Codebase options
->**-u**, **--account** - User's account.  
+>**-u**, **--account** - User's account (default: *%SRCSRV_USERNAME%*).  
 >**-i**, **--domain** - Codebase repository domain.  
 >**-t**, **--proj-permalink** - Project perma link.  
 >**-r**, **--repo-permalink** - Repository perma link.  
 >**-j**, **--api** - REST API version (default is *api3*).  
 ## Codebase environment
 >**SRCSRV_CODEBASE_AUTH** - [Basic authentication used for authorization](https://support.codebasehq.com/kb). This is expected to be the string in the format of *('&lt;domain&gt;/&lt;account&gt;':'&lt;token&gt;')*. The value is evaluated as a python language expression.  
 
@@ -179,17 +178,16 @@
 --project-key myproj
 --repo-slug testing
 --commit release-1.0.0
 --log ..\srcsrv.log
 --plugin srcsrv.plugins.Bitbucket
 ```
 Similar to the command line the option and argument may be separated by space, new line, or equal sign.  
-# External Links
 
+# External Links
+Note that these links may not work properly in the package site (https://pypi.org/project/srcsrv/). Go to https://github.com/urielmann/srcsrv-public for better results.  
 [Srcsrv.doc](https://www.google.com/url?sa=t&rct=j&q=&esrc=s&source=web&cd=3&ved=2ahUKEwjO_sL72NHlAhVYnp4KHcdmCdgQFjACegQIAxAC&url=https%3A%2F%2Fcrashopensource.files.wordpress.com%2F2007%2F10%2Fsrcsrv.doc&usg=AOvVaw0ONZV3AtYTB1S8sgPqhTsU)  
 [The SrcTool Utility](https://learn.microsoft.com/en-us/windows-hardware/drivers/debugger/the-srctool-utility)  
 [Source Indexing is Underused Awesomeness](https://randomascii.wordpress.com/2011/11/11/source-indexing-is-underused-awesomeness/)  
 [Debugging with source indexed **.PDB**](docs/SETUP.md)  
 [Advance topics **.PDB**](docs/ADVANCE.md)  
 [Introduction to SRCSRV Package](https://drive.google.com/drive/folders/1j785kRtb1VvbeqtbieNoWMpL2L2obcpn?usp=drive_link)
-
-
```

### Comparing `srcsrv-1.2.13/README.md` & `srcsrv-1.2.15/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -109,28 +109,28 @@
 
 # Plugins
 Each plugin has unique name of an environment variable containing the authentication used to connect to the remote repository. The value stored in the environment variable will be evaluated as python language expression. It is expected to be in one of three types. See more information in the plugins section.  
 >1. Dictionary (*dict*) entry which is interpreted as HTTPS Authorization header (e.g., *{'Authorization':'Bearer &lt;token&gt;'}*).  
 >2. Tuple (*tuple*) value which in interpreted as HTTPS basic authentication (e.g., *('&lt;account&gt;','&lt;password&gt;')*).  
 >3. The value is missing or *None* to indicate no authentication is required by the remote repository.  
 ## Github options
->**-u**, **--account** - User's account.  
+>**-u**, **--account** - User's account (default: *%SRCSRV_USERNAME%*).  
 >**-r**, **--repo** - Github repository name.  
 ## Github environment
 >**SRCSRV_GITHUB_AUTH** - User [token](https://help.github.com/en/github/authenticating-to-github/creating-a-personal-access-token-for-the-command-line) This is expected to be the string in the format of *{'Authorization':'Token &lt;token&gt;'}*. The value is evaluated as a python language expression.  
 
 ## Bitbucket options
 >**-i**, **--api** - Version of [Bitbucket REST API](https://docs.atlassian.com/bitbucket-server/rest/latest/bitbucket-rest.html) used. The default is *2.0*.  
 >**-t**, **--project-key** - Project key name.  
 >**-r**, **--repo-slug** - Repository slug name.  
 ## Bitbucket environment
 >**SRCSRV_BITBUCKET_AUTH** - User [token](https://developer.atlassian.com/cloud/bitbucket/rest/intro/#authentication_old). This is expected to be the string in the format of *{'Authorization':'Bearer &lt;token&gt;'}*. The value is evaluated as a python language expression.  
 
 ## Gitlab options
->**-u**, **--account** - User's account.  
+>**-u**, **--account** - User's account (default: *%SRCSRV_USERNAME%*).  
 >**-t**, **--project-id** - Project id value.  
 <!--
 @TODO:
 >**-S**, **--sudo** - Gitlab repository sudo account name.  
 -->
 >**-i**, **--api** - Version of [Gitlab REST API](https://docs.gitlab.com/ee/api/rest/) used. The default is *v4*.
 ## Gitlab environment
@@ -138,15 +138,15 @@
 . It may be one of three token types.  
 >1. [Personal access tokens](https://docs.gitlab.com/ee/user/profile/personal_access_tokens.html).  
 >2. [Project access tokens](https://docs.gitlab.com/ee/user/project/settings/project_access_tokens.html)
 >3. [Group access tokens](https://docs.gitlab.com/ee/user/group/settings/group_access_tokens.html)
   
 
 ## Codebase options
->**-u**, **--account** - User's account.  
+>**-u**, **--account** - User's account (default: *%SRCSRV_USERNAME%*).  
 >**-i**, **--domain** - Codebase repository domain.  
 >**-t**, **--proj-permalink** - Project perma link.  
 >**-r**, **--repo-permalink** - Repository perma link.  
 >**-j**, **--api** - REST API version (default is *api3*).  
 ## Codebase environment
 >**SRCSRV_CODEBASE_AUTH** - [Basic authentication used for authorization](https://support.codebasehq.com/kb). This is expected to be the string in the format of *('&lt;domain&gt;/&lt;account&gt;':'&lt;token&gt;')*. The value is evaluated as a python language expression.  
 
@@ -162,15 +162,16 @@
 --project-key myproj
 --repo-slug testing
 --commit release-1.0.0
 --log ..\srcsrv.log
 --plugin srcsrv.plugins.Bitbucket
 ```
 Similar to the command line the option and argument may be separated by space, new line, or equal sign.  
-# External Links
 
+# External Links
+Note that these links may not work properly in the package site (https://pypi.org/project/srcsrv/). Go to https://github.com/urielmann/srcsrv-public for better results.  
 [Srcsrv.doc](https://www.google.com/url?sa=t&rct=j&q=&esrc=s&source=web&cd=3&ved=2ahUKEwjO_sL72NHlAhVYnp4KHcdmCdgQFjACegQIAxAC&url=https%3A%2F%2Fcrashopensource.files.wordpress.com%2F2007%2F10%2Fsrcsrv.doc&usg=AOvVaw0ONZV3AtYTB1S8sgPqhTsU)  
 [The SrcTool Utility](https://learn.microsoft.com/en-us/windows-hardware/drivers/debugger/the-srctool-utility)  
 [Source Indexing is Underused Awesomeness](https://randomascii.wordpress.com/2011/11/11/source-indexing-is-underused-awesomeness/)  
 [Debugging with source indexed **.PDB**](docs/SETUP.md)  
 [Advance topics **.PDB**](docs/ADVANCE.md)  
 [Introduction to SRCSRV Package](https://drive.google.com/drive/folders/1j785kRtb1VvbeqtbieNoWMpL2L2obcpn?usp=drive_link)
```

### Comparing `srcsrv-1.2.13/setup.py` & `srcsrv-1.2.15/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 import setuptools
 
 with open('README.md', 'r') as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='srcsrv',
-    version='1.2.13',
+    version='1.2.15',
     author='Uri Mann',
     author_email='abba.mann@gmail.com',
     description='Source indexing package',
     long_description=long_description,
     long_description_content_type='text/markdown',
     # Additional assets for README.md
     package_data={'': [
```

### Comparing `srcsrv-1.2.13/srcsrv/__init__.py` & `srcsrv-1.2.15/srcsrv/__init__.py`

 * *Files identical despite different names*

### Comparing `srcsrv-1.2.13/srcsrv/__main__.py` & `srcsrv-1.2.15/srcsrv/__main__.py`

 * *Files identical despite different names*

### Comparing `srcsrv-1.2.13/srcsrv/indexer.py` & `srcsrv-1.2.15/srcsrv/indexer.py`

 * *Files identical despite different names*

### Comparing `srcsrv-1.2.13/srcsrv/pdb.py` & `srcsrv-1.2.15/srcsrv/pdb.py`

 * *Files identical despite different names*

### Comparing `srcsrv-1.2.13/srcsrv/plugins/__init__.py` & `srcsrv-1.2.15/srcsrv/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `srcsrv-1.2.13/srcsrv/plugins/bitbucket.py` & `srcsrv-1.2.15/srcsrv/plugins/bitbucket.py`

 * *Files identical despite different names*

### Comparing `srcsrv-1.2.13/srcsrv/plugins/codebase.py` & `srcsrv-1.2.15/srcsrv/plugins/codebase.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,15 +51,15 @@
         unparsed_args - Remaining arguments to parse
         '''
 
         # Add plugin specific arguments
         parser = argparse.ArgumentParser(allow_abbrev=False)
 
         parser.add_argument('-i', '--domain',         help='Repository domain',     required=True)
-        parser.add_argument('-u', '--account',        help='Repository account',    required=True)
+        parser.add_argument('-u', '--account',        help='Repository account',    default='%SRCSRV_USERNAME%')
         parser.add_argument('-t', '--proj-permalink', help='Project permalink',     required=True)
         parser.add_argument('-r', '--repo-permalink', help='Repository  permalink', required=True)
         parser.add_argument('-j', '--api',            help='REST API version',
                                                       default='api3')
 
         super().__init__(parser=parser, args=args, unparsed_args=unparsed_args)
```

### Comparing `srcsrv-1.2.13/srcsrv/plugins/github.py` & `srcsrv-1.2.15/srcsrv/plugins/github.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,16 +50,16 @@
         args - All currently parsed arguments
         unparsed_args - Remaining arguments to parse
         '''
 
         # Add plugin specific arguments
         parser = argparse.ArgumentParser(allow_abbrev=False)
 
-        parser.add_argument('-u', '--account', help='Repository owner', required=True)
-        parser.add_argument('-r', '--repo',    help='Repository name', required=True)
+        parser.add_argument('-u', '--account', help='Repository account', default='%SRCSRV_USERNAME%')
+        parser.add_argument('-r', '--repo',    help='Repository name',    required=True)
 
         super().__init__(parser=parser, args=args, unparsed_args=unparsed_args)
 
     @staticmethod
     def route(account, repo, file_path, file_name):
         '''
         Routing for mocking github REST API
```

### Comparing `srcsrv-1.2.13/srcsrv/plugins/gitlab.py` & `srcsrv-1.2.15/srcsrv/plugins/gitlab.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,17 +51,17 @@
         args - All currently parsed arguments
         unparsed_args - Remaining arguments to parse
         '''
 
         # Add plugin specific arguments
         parser = argparse.ArgumentParser(allow_abbrev=False)
 
-        parser.add_argument('-u', '--account',    help='Repository owner', required=True)
+        parser.add_argument('-u', '--account',    help='Repository account',    default='%SRCSRV_USERNAME%')
         parser.add_argument('-t', '--project-id', help='Repository project ID', required=True)
-        parser.add_argument('-i', '--api',        help='REST API version', default='v4')
+        parser.add_argument('-i', '--api',        help='REST API version',      default='v4')
         parser.add_argument('-j', '--sudo',       help='REST API sudo user')
 
         super().__init__(parser=parser, args=args, unparsed_args=unparsed_args)
 
     @staticmethod
     def json(api_ver, project_id, encoded_file_path):
         '''
```

### Comparing `srcsrv-1.2.13/srcsrv/plugins/plugin.py` & `srcsrv-1.2.15/srcsrv/plugins/plugin.py`

 * *Files identical despite different names*

### Comparing `srcsrv-1.2.13/srcsrv/tools/__init__.py` & `srcsrv-1.2.15/srcsrv/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `srcsrv-1.2.13/srcsrv/tools/api.py` & `srcsrv-1.2.15/srcsrv/tools/api.py`

 * *Files identical despite different names*

### Comparing `srcsrv-1.2.13/srcsrv/utils/__init__.py` & `srcsrv-1.2.15/srcsrv/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `srcsrv-1.2.13/srcsrv.egg-info/PKG-INFO` & `srcsrv-1.2.15/srcsrv.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: srcsrv
-Version: 1.2.13
+Version: 1.2.15
 Summary: Source indexing package
 Home-page: https://github.com/urielmann/srcsrv-public
 Author: Uri Mann
 Author-email: abba.mann@gmail.com
 License: MIT
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Development Status :: 4 - Beta
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -126,28 +125,28 @@
 
 # Plugins
 Each plugin has unique name of an environment variable containing the authentication used to connect to the remote repository. The value stored in the environment variable will be evaluated as python language expression. It is expected to be in one of three types. See more information in the plugins section.  
 >1. Dictionary (*dict*) entry which is interpreted as HTTPS Authorization header (e.g., *{'Authorization':'Bearer &lt;token&gt;'}*).  
 >2. Tuple (*tuple*) value which in interpreted as HTTPS basic authentication (e.g., *('&lt;account&gt;','&lt;password&gt;')*).  
 >3. The value is missing or *None* to indicate no authentication is required by the remote repository.  
 ## Github options
->**-u**, **--account** - User's account.  
+>**-u**, **--account** - User's account (default: *%SRCSRV_USERNAME%*).  
 >**-r**, **--repo** - Github repository name.  
 ## Github environment
 >**SRCSRV_GITHUB_AUTH** - User [token](https://help.github.com/en/github/authenticating-to-github/creating-a-personal-access-token-for-the-command-line) This is expected to be the string in the format of *{'Authorization':'Token &lt;token&gt;'}*. The value is evaluated as a python language expression.  
 
 ## Bitbucket options
 >**-i**, **--api** - Version of [Bitbucket REST API](https://docs.atlassian.com/bitbucket-server/rest/latest/bitbucket-rest.html) used. The default is *2.0*.  
 >**-t**, **--project-key** - Project key name.  
 >**-r**, **--repo-slug** - Repository slug name.  
 ## Bitbucket environment
 >**SRCSRV_BITBUCKET_AUTH** - User [token](https://developer.atlassian.com/cloud/bitbucket/rest/intro/#authentication_old). This is expected to be the string in the format of *{'Authorization':'Bearer &lt;token&gt;'}*. The value is evaluated as a python language expression.  
 
 ## Gitlab options
->**-u**, **--account** - User's account.  
+>**-u**, **--account** - User's account (default: *%SRCSRV_USERNAME%*).  
 >**-t**, **--project-id** - Project id value.  
 <!--
 @TODO:
 >**-S**, **--sudo** - Gitlab repository sudo account name.  
 -->
 >**-i**, **--api** - Version of [Gitlab REST API](https://docs.gitlab.com/ee/api/rest/) used. The default is *v4*.
 ## Gitlab environment
@@ -155,15 +154,15 @@
 . It may be one of three token types.  
 >1. [Personal access tokens](https://docs.gitlab.com/ee/user/profile/personal_access_tokens.html).  
 >2. [Project access tokens](https://docs.gitlab.com/ee/user/project/settings/project_access_tokens.html)
 >3. [Group access tokens](https://docs.gitlab.com/ee/user/group/settings/group_access_tokens.html)
   
 
 ## Codebase options
->**-u**, **--account** - User's account.  
+>**-u**, **--account** - User's account (default: *%SRCSRV_USERNAME%*).  
 >**-i**, **--domain** - Codebase repository domain.  
 >**-t**, **--proj-permalink** - Project perma link.  
 >**-r**, **--repo-permalink** - Repository perma link.  
 >**-j**, **--api** - REST API version (default is *api3*).  
 ## Codebase environment
 >**SRCSRV_CODEBASE_AUTH** - [Basic authentication used for authorization](https://support.codebasehq.com/kb). This is expected to be the string in the format of *('&lt;domain&gt;/&lt;account&gt;':'&lt;token&gt;')*. The value is evaluated as a python language expression.  
 
@@ -179,17 +178,16 @@
 --project-key myproj
 --repo-slug testing
 --commit release-1.0.0
 --log ..\srcsrv.log
 --plugin srcsrv.plugins.Bitbucket
 ```
 Similar to the command line the option and argument may be separated by space, new line, or equal sign.  
-# External Links
 
+# External Links
+Note that these links may not work properly in the package site (https://pypi.org/project/srcsrv/). Go to https://github.com/urielmann/srcsrv-public for better results.  
 [Srcsrv.doc](https://www.google.com/url?sa=t&rct=j&q=&esrc=s&source=web&cd=3&ved=2ahUKEwjO_sL72NHlAhVYnp4KHcdmCdgQFjACegQIAxAC&url=https%3A%2F%2Fcrashopensource.files.wordpress.com%2F2007%2F10%2Fsrcsrv.doc&usg=AOvVaw0ONZV3AtYTB1S8sgPqhTsU)  
 [The SrcTool Utility](https://learn.microsoft.com/en-us/windows-hardware/drivers/debugger/the-srctool-utility)  
 [Source Indexing is Underused Awesomeness](https://randomascii.wordpress.com/2011/11/11/source-indexing-is-underused-awesomeness/)  
 [Debugging with source indexed **.PDB**](docs/SETUP.md)  
 [Advance topics **.PDB**](docs/ADVANCE.md)  
 [Introduction to SRCSRV Package](https://drive.google.com/drive/folders/1j785kRtb1VvbeqtbieNoWMpL2L2obcpn?usp=drive_link)
-
-
```

