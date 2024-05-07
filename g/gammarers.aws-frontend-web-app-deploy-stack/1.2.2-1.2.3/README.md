# Comparing `tmp/gammarers.aws-frontend-web-app-deploy-stack-1.2.2.tar.gz` & `tmp/gammarers.aws-frontend-web-app-deploy-stack-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gammarers.aws-frontend-web-app-deploy-stack-1.2.2.tar", last modified: Tue Apr 30 19:13:37 2024, max compression
+gzip compressed data, was "gammarers.aws-frontend-web-app-deploy-stack-1.2.3.tar", last modified: Tue May  7 19:14:20 2024, max compression
```

## Comparing `gammarers.aws-frontend-web-app-deploy-stack-1.2.2.tar` & `gammarers.aws-frontend-web-app-deploy-stack-1.2.3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 19:13:37.468958 gammarers.aws-frontend-web-app-deploy-stack-1.2.2/
--rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-04-30 19:13:26.000000 gammarers.aws-frontend-web-app-deploy-stack-1.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-30 19:13:26.000000 gammarers.aws-frontend-web-app-deploy-stack-1.2.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3547 2024-04-30 19:13:37.468958 gammarers.aws-frontend-web-app-deploy-stack-1.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2515 2024-04-30 19:13:26.000000 gammarers.aws-frontend-web-app-deploy-stack-1.2.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-30 19:13:26.000000 gammarers.aws-frontend-web-app-deploy-stack-1.2.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 19:13:37.468958 gammarers.aws-frontend-web-app-deploy-stack-1.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2225 2024-04-30 19:13:26.000000 gammarers.aws-frontend-web-app-deploy-stack-1.2.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 19:13:37.464958 gammarers.aws-frontend-web-app-deploy-stack-1.2.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 19:13:37.464958 gammarers.aws-frontend-web-app-deploy-stack-1.2.2/src/gammarers/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 19:13:37.468958 gammarers.aws-frontend-web-app-deploy-stack-1.2.2/src/gammarers/aws_frontend_web_app_deploy_stack/
--rw-r--r--   0 runner    (1001) docker     (127)    27776 2024-04-30 19:13:26.000000 gammarers.aws-frontend-web-app-deploy-stack-1.2.2/src/gammarers/aws_frontend_web_app_deploy_stack/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 19:13:37.468958 gammarers.aws-frontend-web-app-deploy-stack-1.2.2/src/gammarers/aws_frontend_web_app_deploy_stack/_jsii/
--rw-r--r--   0 runner    (1001) docker     (127)      708 2024-04-30 19:13:26.000000 gammarers.aws-frontend-web-app-deploy-stack-1.2.2/src/gammarers/aws_frontend_web_app_deploy_stack/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    36124 2024-04-30 19:13:26.000000 gammarers.aws-frontend-web-app-deploy-stack-1.2.2/src/gammarers/aws_frontend_web_app_deploy_stack/_jsii/aws-frontend-web-app-deploy-stack@1.2.2.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 19:13:26.000000 gammarers.aws-frontend-web-app-deploy-stack-1.2.2/src/gammarers/aws_frontend_web_app_deploy_stack/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 19:13:37.468958 gammarers.aws-frontend-web-app-deploy-stack-1.2.2/src/gammarers.aws_frontend_web_app_deploy_stack.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3547 2024-04-30 19:13:37.000000 gammarers.aws-frontend-web-app-deploy-stack-1.2.2/src/gammarers.aws_frontend_web_app_deploy_stack.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      693 2024-04-30 19:13:37.000000 gammarers.aws-frontend-web-app-deploy-stack-1.2.2/src/gammarers.aws_frontend_web_app_deploy_stack.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 19:13:37.000000 gammarers.aws-frontend-web-app-deploy-stack-1.2.2/src/gammarers.aws_frontend_web_app_deploy_stack.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      289 2024-04-30 19:13:37.000000 gammarers.aws-frontend-web-app-deploy-stack-1.2.2/src/gammarers.aws_frontend_web_app_deploy_stack.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-30 19:13:37.000000 gammarers.aws-frontend-web-app-deploy-stack-1.2.2/src/gammarers.aws_frontend_web_app_deploy_stack.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 19:14:20.479334 gammarers.aws-frontend-web-app-deploy-stack-1.2.3/
+-rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-05-07 19:14:05.000000 gammarers.aws-frontend-web-app-deploy-stack-1.2.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-07 19:14:05.000000 gammarers.aws-frontend-web-app-deploy-stack-1.2.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3547 2024-05-07 19:14:20.479334 gammarers.aws-frontend-web-app-deploy-stack-1.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2515 2024-05-07 19:14:05.000000 gammarers.aws-frontend-web-app-deploy-stack-1.2.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-07 19:14:05.000000 gammarers.aws-frontend-web-app-deploy-stack-1.2.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 19:14:20.479334 gammarers.aws-frontend-web-app-deploy-stack-1.2.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2225 2024-05-07 19:14:05.000000 gammarers.aws-frontend-web-app-deploy-stack-1.2.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 19:14:20.475334 gammarers.aws-frontend-web-app-deploy-stack-1.2.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 19:14:20.475334 gammarers.aws-frontend-web-app-deploy-stack-1.2.3/src/gammarers/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 19:14:20.479334 gammarers.aws-frontend-web-app-deploy-stack-1.2.3/src/gammarers/aws_frontend_web_app_deploy_stack/
+-rw-r--r--   0 runner    (1001) docker     (127)    27776 2024-05-07 19:14:05.000000 gammarers.aws-frontend-web-app-deploy-stack-1.2.3/src/gammarers/aws_frontend_web_app_deploy_stack/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 19:14:20.479334 gammarers.aws-frontend-web-app-deploy-stack-1.2.3/src/gammarers/aws_frontend_web_app_deploy_stack/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (127)      708 2024-05-07 19:14:05.000000 gammarers.aws-frontend-web-app-deploy-stack-1.2.3/src/gammarers/aws_frontend_web_app_deploy_stack/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36129 2024-05-07 19:14:05.000000 gammarers.aws-frontend-web-app-deploy-stack-1.2.3/src/gammarers/aws_frontend_web_app_deploy_stack/_jsii/aws-frontend-web-app-deploy-stack@1.2.3.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 19:14:05.000000 gammarers.aws-frontend-web-app-deploy-stack-1.2.3/src/gammarers/aws_frontend_web_app_deploy_stack/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 19:14:20.479334 gammarers.aws-frontend-web-app-deploy-stack-1.2.3/src/gammarers.aws_frontend_web_app_deploy_stack.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3547 2024-05-07 19:14:20.000000 gammarers.aws-frontend-web-app-deploy-stack-1.2.3/src/gammarers.aws_frontend_web_app_deploy_stack.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      693 2024-05-07 19:14:20.000000 gammarers.aws-frontend-web-app-deploy-stack-1.2.3/src/gammarers.aws_frontend_web_app_deploy_stack.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 19:14:20.000000 gammarers.aws-frontend-web-app-deploy-stack-1.2.3/src/gammarers.aws_frontend_web_app_deploy_stack.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      289 2024-05-07 19:14:20.000000 gammarers.aws-frontend-web-app-deploy-stack-1.2.3/src/gammarers.aws_frontend_web_app_deploy_stack.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-07 19:14:20.000000 gammarers.aws-frontend-web-app-deploy-stack-1.2.3/src/gammarers.aws_frontend_web_app_deploy_stack.egg-info/top_level.txt
```

### Comparing `gammarers.aws-frontend-web-app-deploy-stack-1.2.2/LICENSE` & `gammarers.aws-frontend-web-app-deploy-stack-1.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `gammarers.aws-frontend-web-app-deploy-stack-1.2.2/PKG-INFO` & `gammarers.aws-frontend-web-app-deploy-stack-1.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gammarers.aws-frontend-web-app-deploy-stack
-Version: 1.2.2
+Version: 1.2.3
 Summary: This is an AWS CDK Construct to make deploying a Frontend Web App (SPA) deploy to S3 behind CloudFront.
 Home-page: https://github.com/gammarers/aws-frontend-web-app-deploy-stack.git
 Author: yicr<yicr@users.noreply.github.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/gammarers/aws-frontend-web-app-deploy-stack.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `gammarers.aws-frontend-web-app-deploy-stack-1.2.2/README.md` & `gammarers.aws-frontend-web-app-deploy-stack-1.2.3/README.md`

 * *Files identical despite different names*

### Comparing `gammarers.aws-frontend-web-app-deploy-stack-1.2.2/setup.py` & `gammarers.aws-frontend-web-app-deploy-stack-1.2.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "gammarers.aws-frontend-web-app-deploy-stack",
-    "version": "1.2.2",
+    "version": "1.2.3",
     "description": "This is an AWS CDK Construct to make deploying a Frontend Web App (SPA) deploy to S3 behind CloudFront.",
     "license": "Apache-2.0",
     "url": "https://github.com/gammarers/aws-frontend-web-app-deploy-stack.git",
     "long_description_content_type": "text/markdown",
     "author": "yicr<yicr@users.noreply.github.com>",
     "bdist_wheel": {
         "universal": true
@@ -22,28 +22,28 @@
     },
     "packages": [
         "gammarers.aws_frontend_web_app_deploy_stack",
         "gammarers.aws_frontend_web_app_deploy_stack._jsii"
     ],
     "package_data": {
         "gammarers.aws_frontend_web_app_deploy_stack._jsii": [
-            "aws-frontend-web-app-deploy-stack@1.2.2.jsii.tgz"
+            "aws-frontend-web-app-deploy-stack@1.2.3.jsii.tgz"
         ],
         "gammarers.aws_frontend_web_app_deploy_stack": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.8",
     "install_requires": [
         "aws-cdk-lib>=2.80.0, <3.0.0",
         "constructs>=10.0.5, <11.0.0",
         "gammarers.aws-secure-bucket>=1.3.1, <1.4.0",
         "gammarers.aws-secure-cloudfront-origin-bucket>=1.5.0, <1.6.0",
         "gammarers.aws-secure-frontend-web-app-cloudfront-distribution>=1.3.0, <1.4.0",
-        "jsii>=1.97.0, <2.0.0",
+        "jsii>=1.98.0, <2.0.0",
         "publication>=0.0.3",
         "typeguard~=2.13.3"
     ],
     "classifiers": [
         "Intended Audience :: Developers",
         "Operating System :: OS Independent",
         "Programming Language :: JavaScript",
```

### Comparing `gammarers.aws-frontend-web-app-deploy-stack-1.2.2/src/gammarers/aws_frontend_web_app_deploy_stack/__init__.py` & `gammarers.aws-frontend-web-app-deploy-stack-1.2.3/src/gammarers/aws_frontend_web_app_deploy_stack/__init__.py`

 * *Files identical despite different names*

### Comparing `gammarers.aws-frontend-web-app-deploy-stack-1.2.2/src/gammarers/aws_frontend_web_app_deploy_stack/_jsii/__init__.py` & `gammarers.aws-frontend-web-app-deploy-stack-1.2.3/src/gammarers/aws_frontend_web_app_deploy_stack/_jsii/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,17 +17,17 @@
 import constructs._jsii
 import gammarers.aws_secure_bucket._jsii
 import gammarers.aws_secure_cloudfront_origin_bucket._jsii
 import gammarers.aws_secure_frontend_web_app_cloudfront_distribution._jsii
 
 __jsii_assembly__ = jsii.JSIIAssembly.load(
     "@gammarers/aws-frontend-web-app-deploy-stack",
-    "1.2.2",
+    "1.2.3",
     __name__[0:-6],
-    "aws-frontend-web-app-deploy-stack@1.2.2.jsii.tgz",
+    "aws-frontend-web-app-deploy-stack@1.2.3.jsii.tgz",
 )
 
 __all__ = [
     "__jsii_assembly__",
 ]
 
 publication.publish()
```

### Comparing `gammarers.aws-frontend-web-app-deploy-stack-1.2.2/src/gammarers/aws_frontend_web_app_deploy_stack/_jsii/aws-frontend-web-app-deploy-stack@1.2.2.jsii.tgz` & `gammarers.aws-frontend-web-app-deploy-stack-1.2.3/src/gammarers/aws_frontend_web_app_deploy_stack/_jsii/aws-frontend-web-app-deploy-stack@1.2.3.jsii.tgz`

 * *Files 24% similar despite different names*

#### Comparing `aws-frontend-web-app-deploy-stack@1.2.2.jsii.tgz-content` & `aws-frontend-web-app-deploy-stack@1.2.3.jsii.tgz-content`

##### package/.jsii

###### Pretty-printed

 * *Similarity: 0.9444444444444444%*

 * *Differences: {"'fingerprint'": "'RMUTTB5JMn3L3ehwzCacBQ4VGnGHYYS8LIV0N4SJMgU='", "'version'": "'1.2.3'"}*

```diff
@@ -3496,15 +3496,15 @@
             }
         }
     },
     "description": "This is an AWS CDK Construct to make deploying a Frontend Web App (SPA) deploy to S3 behind CloudFront.",
     "docs": {
         "stability": "stable"
     },
-    "fingerprint": "JpIrJMYFfaPQCR3XiXOE4aoBvQmn5/GRM2sRHEur3QE=",
+    "fingerprint": "RMUTTB5JMn3L3ehwzCacBQ4VGnGHYYS8LIV0N4SJMgU=",
     "homepage": "https://github.com/gammarers/aws-frontend-web-app-deploy-stack.git",
     "jsiiVersion": "5.2.44 (build ff4e411)",
     "keywords": [
         "aws",
         "cdk",
         "cdn",
         "cloudfront",
@@ -3680,9 +3680,9 @@
                         "primitive": "string"
                     }
                 }
             ],
             "symbolId": "src/index:FrontendWebAppDeployStackProps"
         }
     },
-    "version": "1.2.2"
+    "version": "1.2.3"
 }
```

##### package/lib/index.js

###### js-beautify {}

```diff
@@ -62,10 +62,10 @@
         });
     }
 }
 exports.FrontendWebAppDeployStack = FrontendWebAppDeployStack;
 _a = JSII_RTTI_SYMBOL_1;
 FrontendWebAppDeployStack[_a] = {
     fqn: "@gammarers/aws-frontend-web-app-deploy-stack.FrontendWebAppDeployStack",
-    version: "1.2.2"
+    version: "1.2.3"
 };
 //# sourceMappingURL=data:application/json;base64,eyJ2ZXJzaW9uIjozLCJmaWxlIjoiaW5kZXguanMiLCJzb3VyY2VSb290IjoiIiwic291cmNlcyI6WyIuLi9zcmMvaW5kZXgudHMiXSwibmFtZXMiOltdLCJtYXBwaW5ncyI6Ijs7Ozs7QUFBQSx3R0FBMEg7QUFDMUgsd0lBQWdKO0FBQ2hKLG1DQUFtQztBQUNuQywwREFBMEQ7QUFDMUQseURBQXlEO0FBQ3pELG1EQUFtRDtBQUNuRCx5REFBeUQ7QUFDekQseUNBQXlDO0FBQ3pDLDBEQUEwRDtBQVcxRCxNQUFhLHlCQUEwQixTQUFRLEdBQUcsQ0FBQyxLQUFLO0lBQ3RELFlBQVksS0FBZ0IsRUFBRSxFQUFVLEVBQUUsS0FBcUM7UUFDN0UsS0FBSyxDQUFDLEtBQUssRUFBRSxFQUFFLEVBQUUsS0FBSyxDQUFDLENBQUM7UUFFeEIsOENBQThDO1FBQzlDLE1BQU0sR0FBRyxHQUFHLElBQUksVUFBVSxDQUFDLG9CQUFvQixDQUFDLElBQUksRUFBRSxzQkFBc0IsQ0FBQyxDQUFDO1FBRTlFLDRDQUE0QztRQUM1QyxNQUFNLFlBQVksR0FBRyxJQUFJLGtFQUE0QixDQUFDLElBQUksRUFBRSw4QkFBOEIsRUFBRTtZQUMxRixVQUFVLEVBQUUsS0FBSyxDQUFDLGdCQUFnQjtZQUNsQyxvQkFBb0IsRUFBRSxnRUFBMEIsQ0FBQyxzQkFBc0I7WUFDdkUsK0NBQStDLEVBQUUsR0FBRyxDQUFDLCtDQUErQztTQUNyRyxDQUFDLENBQUM7UUFFSCxxQkFBcUI7UUFDckIsTUFBTSxVQUFVLEdBQUcsT0FBTyxDQUFDLFVBQVUsQ0FBQyx3QkFBd0IsQ0FBQyxJQUFJLEVBQUUsWUFBWSxFQUFFO1lBQ2pGLFlBQVksRUFBRSxLQUFLLENBQUMsWUFBWTtZQUNoQyxRQUFRLEVBQUUsS0FBSyxDQUFDLFVBQVU7U0FDM0IsQ0FBQyxDQUFDO1FBRUgsMENBQTBDO1FBQzFDLE1BQU0sV0FBVyxHQUFHLElBQUksR0FBRyxDQUFDLFdBQVcsQ0FBQyxJQUFJLEVBQUUsYUFBYSxFQUFFO1lBQzNELFVBQVUsRUFBRSxLQUFLLENBQUMsVUFBVTtZQUM1QixVQUFVLEVBQUUsR0FBRyxDQUFDLHFCQUFxQixDQUFDLE9BQU8sQ0FBQyxVQUFVLENBQUM7U0FDMUQsQ0FBQyxDQUFDO1FBRUgscURBQXFEO1FBQ3JELE1BQU0sWUFBWSxHQUFHLElBQUksZ0dBQTBDLENBQUMsSUFBSSxFQUFFLDRDQUE0QyxFQUFFO1lBQ3RILE9BQU8sRUFBRSxnQ0FBZ0M7WUFDekMsZUFBZSxFQUFFLEVBQUUsQ0FBQyxNQUFNLENBQUMsYUFBYSxDQUFDLElBQUksRUFBRSxXQUFXLEVBQUUsS0FBSyxDQUFDLFlBQVksQ0FBQztZQUMvRSxXQUFXLEVBQUUsV0FBVztZQUN4QixVQUFVLEVBQUUsS0FBSyxDQUFDLFVBQVU7WUFDNUIsa0JBQWtCLEVBQUUsd0VBQWtCLENBQUMsc0JBQXNCO1lBQzdELG9CQUFvQixFQUFFLEdBQUc7WUFDekIsWUFBWSxFQUFFLFlBQVk7U0FDM0IsQ0FBQyxDQUFDO1FBRUgseUJBQXlCO1FBQ3pCLElBQUksT0FBTyxDQUFDLE9BQU8sQ0FBQyxJQUFJLEVBQUUsWUFBWSxFQUFFO1lBQ3RDLElBQUksRUFBRSxVQUFVO1lBQ2hCLFVBQVUsRUFBRSxLQUFLLENBQUMsVUFBVTtZQUM1QixNQUFNLEVBQUUsT0FBTyxDQUFDLFlBQVksQ0FBQyxTQUFTLENBQUMsSUFBSSxLQUFLLENBQUMsZ0JBQWdCLENBQUMsWUFBWSxDQUFDLENBQUM7WUFDaEYsR0FBRyxFQUFFLEdBQUcsQ0FBQyxRQUFRLENBQUMsT0FBTyxDQUFDLEdBQUcsQ0FBQztTQUMvQixDQUFDLENBQUM7UUFFSCxzREFBc0Q7UUFDdEQsSUFBSSxRQUFRLENBQUMsZ0JBQWdCLENBQUMsSUFBSSxFQUFFLHdCQUF3QixFQUFFO1lBQzVELE9BQU8sRUFBRSxDQUFDLFFBQVEsQ0FBQyxNQUFNLENBQUMsS0FBSyxDQUFDLEtBQUssQ0FBQyxxQkFBcUIsQ0FBQyxDQUFDO1lBQzdELGlCQUFpQixFQUFFLFlBQVk7WUFDL0IsS0FBSyxFQUFFLElBQUk7WUFDWCxZQUFZO1lBQ1osaUJBQWlCLEVBQUUsQ0FBQyxJQUFJLENBQUM7U0FDMUIsQ0FBQyxDQUFDO0lBQ0wsQ0FBQzs7QUFyREgsOERBc0RDIiwic291cmNlc0NvbnRlbnQiOlsiaW1wb3J0IHsgU2VjdXJlQ2xvdWRGcm9udE9yaWdpbkJ1Y2tldCwgU2VjdXJlQ2xvdWRGcm9udE9yaWdpblR5cGUgfSBmcm9tICdAZ2FtbWFyZXJzL2F3cy1zZWN1cmUtY2xvdWRmcm9udC1vcmlnaW4tYnVja2V0JztcbmltcG9ydCB7IFNlY3VyZUZyb250ZW5kV2ViQXBwQ2xvdWRGcm9udERpc3RyaWJ1dGlvbiwgUzNPcmlnaW5BY2Nlc3NUeXBlIH0gZnJvbSAnQGdhbW1hcmVycy9hd3Mtc2VjdXJlLWZyb250ZW5kLXdlYi1hcHAtY2xvdWRmcm9udC1kaXN0cmlidXRpb24nO1xuaW1wb3J0ICogYXMgY2RrIGZyb20gJ2F3cy1jZGstbGliJztcbmltcG9ydCAqIGFzIGFjbSBmcm9tICdhd3MtY2RrLWxpYi9hd3MtY2VydGlmaWNhdGVtYW5hZ2VyJztcbmltcG9ydCAqIGFzIGNsb3VkZnJvbnQgZnJvbSAnYXdzLWNkay1saWIvYXdzLWNsb3VkZnJvbnQnO1xuaW1wb3J0ICogYXMgcm91dGU1MyBmcm9tICdhd3MtY2RrLWxpYi9hd3Mtcm91dGU1Myc7XG5pbXBvcnQgKiBhcyBhbGlhcyBmcm9tICdhd3MtY2RrLWxpYi9hd3Mtcm91dGU1My10YXJnZXRzJztcbmltcG9ydCAqIGFzIHMzIGZyb20gJ2F3cy1jZGstbGliL2F3cy1zMyc7XG5pbXBvcnQgKiBhcyBzM2RlcGxveSBmcm9tICdhd3MtY2RrLWxpYi9hd3MtczMtZGVwbG95bWVudCc7XG5pbXBvcnQgeyBDb25zdHJ1Y3QgfSBmcm9tICdjb25zdHJ1Y3RzJztcblxuZXhwb3J0IGludGVyZmFjZSBGcm9udGVuZFdlYkFwcERlcGxveVN0YWNrUHJvcHMgZXh0ZW5kcyBjZGsuU3RhY2tQcm9wcyB7XG4gIHJlYWRvbmx5IGRvbWFpbk5hbWU6IHN0cmluZztcbiAgcmVhZG9ubHkgaG9zdGVkWm9uZUlkOiBzdHJpbmc7XG4gIHJlYWRvbmx5IG9yaWdpbkJ1Y2tldE5hbWU6IHN0cmluZztcbiAgcmVhZG9ubHkgbG9nQnVja2V0QXJuOiBzdHJpbmc7XG4gIHJlYWRvbmx5IGRlcGxveVNvdXJjZUFzc2V0UGF0aDogc3RyaW5nO1xufVxuXG5leHBvcnQgY2xhc3MgRnJvbnRlbmRXZWJBcHBEZXBsb3lTdGFjayBleHRlbmRzIGNkay5TdGFjayB7XG4gIGNvbnN0cnVjdG9yKHNjb3BlOiBDb25zdHJ1Y3QsIGlkOiBzdHJpbmcsIHByb3BzOiBGcm9udGVuZFdlYkFwcERlcGxveVN0YWNrUHJvcHMpIHtcbiAgICBzdXBlcihzY29wZSwgaWQsIHByb3BzKTtcblxuICAgIC8vIPCfkYdDcmVhdGUgQ2xvdWRGcm9udCBPcmlnaW4gQWNjZXNzIElkZW50aXR5LlxuICAgIGNvbnN0IG9haSA9IG5ldyBjbG91ZGZyb250Lk9yaWdpbkFjY2Vzc0lkZW50aXR5KHRoaXMsICdPcmlnaW5BY2Nlc3NJZGVudGl0eScpO1xuXG4gICAgLy8g8J+Rh0NyZWF0ZSBTZWN1cmUgQ2xvdWQgRnJvbnQgT3JpZ2luIEJ1Y2tldFxuICAgIGNvbnN0IG9yaWdpbkJ1Y2tldCA9IG5ldyBTZWN1cmVDbG91ZEZyb250T3JpZ2luQnVja2V0KHRoaXMsICdTZWN1cmVDbG91ZEZyb250T3JpZ2luQnVja2V0Jywge1xuICAgICAgYnVja2V0TmFtZTogcHJvcHMub3JpZ2luQnVja2V0TmFtZSxcbiAgICAgIGNsb3VkRnJvbnRPcmlnaW5UeXBlOiBTZWN1cmVDbG91ZEZyb250T3JpZ2luVHlwZS5PUklHSU5fQUNDRVNTX0lERU5USVRZLFxuICAgICAgY2xvdWRGcm9udE9yaWdpbkFjY2Vzc0lkZW50aXR5UzNDYW5vbmljYWxVc2VySWQ6IG9haS5jbG91ZEZyb250T3JpZ2luQWNjZXNzSWRlbnRpdHlTM0Nhbm9uaWNhbFVzZXJJZCxcbiAgICB9KTtcblxuICAgIC8vIPCfkYdHZXQgSG9zdGVkIFpvbmUuXG4gICAgY29uc3QgaG9zdGVkWm9uZSA9IHJvdXRlNTMuSG9zdGVkWm9uZS5mcm9tSG9zdGVkWm9uZUF0dHJpYnV0ZXModGhpcywgJ0hvc3RlZFpvbmUnLCB7XG4gICAgICBob3N0ZWRab25lSWQ6IHByb3BzLmhvc3RlZFpvbmVJZCxcbiAgICAgIHpvbmVOYW1lOiBwcm9wcy5kb21haW5OYW1lLFxuICAgIH0pO1xuXG4gICAgLy8g8J+Rh0NyZWF0ZSBDZXJ0aWZpY2F0ZSB3aXRoIEROUyB2YWxpZGF0ZS5cbiAgICBjb25zdCBjZXJ0aWZpY2F0ZSA9IG5ldyBhY20uQ2VydGlmaWNhdGUodGhpcywgJ0NlcnRpZmljYXRlJywge1xuICAgICAgZG9tYWluTmFtZTogcHJvcHMuZG9tYWluTmFtZSxcbiAgICAgIHZhbGlkYXRpb246IGFjbS5DZXJ0aWZpY2F0ZVZhbGlkYXRpb24uZnJvbURucyhob3N0ZWRab25lKSxcbiAgICB9KTtcblxuICAgIC8vIPCfkYdTZWN1cmUgRnJvbnRlbmQgV2ViIEFwcCBDbG91ZEZyb250IERpc3RyaWJ1dGlvbi5cbiAgICBjb25zdCBkaXN0cmlidXRpb24gPSBuZXcgU2VjdXJlRnJvbnRlbmRXZWJBcHBDbG91ZEZyb250RGlzdHJpYnV0aW9uKHRoaXMsICdTZWN1cmVGcm9udGVuZFdlYkFwcENsb3VkRnJvbnREaXN0cmlidXRpb24nLCB7XG4gICAgICBjb21tZW50OiAnZnJvbnRlbmQgd2ViIGFwcCBkaXN0cmlidXRpb24uJyxcbiAgICAgIGFjY2Vzc0xvZ0J1Y2tldDogczMuQnVja2V0LmZyb21CdWNrZXRBcm4odGhpcywgJ0xvZ0J1Y2tldCcsIHByb3BzLmxvZ0J1Y2tldEFybiksXG4gICAgICBjZXJ0aWZpY2F0ZTogY2VydGlmaWNhdGUsXG4gICAgICBkb21haW5OYW1lOiBwcm9wcy5kb21haW5OYW1lLFxuICAgICAgczNPcmlnaW5BY2Nlc3NUeXBlOiBTM09yaWdpbkFjY2Vzc1R5cGUuT1JJR0lOX0FDQ0VTU19JREVOVElUWSxcbiAgICAgIG9yaWdpbkFjY2Vzc0lkZW50aXR5OiBvYWksXG4gICAgICBvcmlnaW5CdWNrZXQ6IG9yaWdpbkJ1Y2tldCxcbiAgICB9KTtcblxuICAgIC8vIPCfkYdSb3V0ZSA1MyBETlMgKEFsaWFzKVxuICAgIG5ldyByb3V0ZTUzLkFSZWNvcmQodGhpcywgJ0ROU0FSZWNvcmQnLCB7XG4gICAgICB6b25lOiBob3N0ZWRab25lLFxuICAgICAgcmVjb3JkTmFtZTogcHJvcHMuZG9tYWluTmFtZSxcbiAgICAgIHRhcmdldDogcm91dGU1My5SZWNvcmRUYXJnZXQuZnJvbUFsaWFzKG5ldyBhbGlhcy5DbG91ZEZyb250VGFyZ2V0KGRpc3RyaWJ1dGlvbikpLFxuICAgICAgdHRsOiBjZGsuRHVyYXRpb24uc2Vjb25kcygzMDApLFxuICAgIH0pO1xuXG4gICAgLy8g8J+Rh0RlcGxveSB0byBCdWNrZXQgd2l0aCBDbG91ZEZyb250IENhY2hlIGludmFsaWRhdGVcbiAgICBuZXcgczNkZXBsb3kuQnVja2V0RGVwbG95bWVudCh0aGlzLCAnRGVwbG95V2l0aEludmFsaWRhdGlvbicsIHtcbiAgICAgIHNvdXJjZXM6IFtzM2RlcGxveS5Tb3VyY2UuYXNzZXQocHJvcHMuZGVwbG95U291cmNlQXNzZXRQYXRoKV0sXG4gICAgICBkZXN0aW5hdGlvbkJ1Y2tldDogb3JpZ2luQnVja2V0LFxuICAgICAgcHJ1bmU6IHRydWUsXG4gICAgICBkaXN0cmlidXRpb24sXG4gICAgICBkaXN0cmlidXRpb25QYXRoczogWycvKiddLFxuICAgIH0pO1xuICB9XG59XG4iXX0=
```

##### package/package.json

###### Pretty-printed

 * *Similarity: 0.9712918660287081%*

 * *Differences: {"'devDependencies'": "{'jsii-diff': '^1.98.0', 'jsii-docgen': '^10.4.6', 'jsii-pacmak': "*

 * *                      "'^1.98.0', 'projen': '^0.81.7'}",*

 * * "'version'": "'1.2.3'"}*

```diff
@@ -21,19 +21,19 @@
         "constructs": "10.0.5",
         "eslint": "^8",
         "eslint-import-resolver-typescript": "^3.6.1",
         "eslint-plugin-import": "^2.29.1",
         "jest": "^29.7.0",
         "jest-junit": "^15",
         "jsii": "5.2.x",
-        "jsii-diff": "^1.97.0",
-        "jsii-docgen": "^10.4.3",
-        "jsii-pacmak": "^1.97.0",
+        "jsii-diff": "^1.98.0",
+        "jsii-docgen": "^10.4.6",
+        "jsii-pacmak": "^1.98.0",
         "jsii-rosetta": "5.2.x",
-        "projen": "^0.81.5",
+        "projen": "^0.81.7",
         "standard-version": "^9",
         "ts-jest": "^29.1.2",
         "ts-node": "^10.9.2",
         "typescript": "5.2.x"
     },
     "engines": {
         "node": ">= 16.0.0"
@@ -150,9 +150,9 @@
         "test:watch": "npx projen test:watch",
         "unbump": "npx projen unbump",
         "upgrade": "npx projen upgrade",
         "watch": "npx projen watch"
     },
     "stability": "stable",
     "types": "lib/index.d.ts",
-    "version": "1.2.2"
+    "version": "1.2.3"
 }
```

### Comparing `gammarers.aws-frontend-web-app-deploy-stack-1.2.2/src/gammarers.aws_frontend_web_app_deploy_stack.egg-info/PKG-INFO` & `gammarers.aws-frontend-web-app-deploy-stack-1.2.3/src/gammarers.aws_frontend_web_app_deploy_stack.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gammarers.aws-frontend-web-app-deploy-stack
-Version: 1.2.2
+Version: 1.2.3
 Summary: This is an AWS CDK Construct to make deploying a Frontend Web App (SPA) deploy to S3 behind CloudFront.
 Home-page: https://github.com/gammarers/aws-frontend-web-app-deploy-stack.git
 Author: yicr<yicr@users.noreply.github.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/gammarers/aws-frontend-web-app-deploy-stack.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `gammarers.aws-frontend-web-app-deploy-stack-1.2.2/src/gammarers.aws_frontend_web_app_deploy_stack.egg-info/SOURCES.txt` & `gammarers.aws-frontend-web-app-deploy-stack-1.2.3/src/gammarers.aws_frontend_web_app_deploy_stack.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -7,8 +7,8 @@
 src/gammarers.aws_frontend_web_app_deploy_stack.egg-info/SOURCES.txt
 src/gammarers.aws_frontend_web_app_deploy_stack.egg-info/dependency_links.txt
 src/gammarers.aws_frontend_web_app_deploy_stack.egg-info/requires.txt
 src/gammarers.aws_frontend_web_app_deploy_stack.egg-info/top_level.txt
 src/gammarers/aws_frontend_web_app_deploy_stack/__init__.py
 src/gammarers/aws_frontend_web_app_deploy_stack/py.typed
 src/gammarers/aws_frontend_web_app_deploy_stack/_jsii/__init__.py
-src/gammarers/aws_frontend_web_app_deploy_stack/_jsii/aws-frontend-web-app-deploy-stack@1.2.2.jsii.tgz
+src/gammarers/aws_frontend_web_app_deploy_stack/_jsii/aws-frontend-web-app-deploy-stack@1.2.3.jsii.tgz
```

