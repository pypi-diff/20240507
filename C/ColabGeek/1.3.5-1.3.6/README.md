# Comparing `tmp/colabgeek-1.3.5.tar.gz` & `tmp/colabgeek-1.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "colabgeek-1.3.5.tar", last modified: Sat Apr 20 08:11:11 2024, max compression
+gzip compressed data, was "colabgeek-1.3.6.tar", last modified: Tue May  7 05:10:07 2024, max compression
```

## Comparing `colabgeek-1.3.5.tar` & `colabgeek-1.3.6.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxr-x   0 sunym     (1000) sunym     (1000)        0 2024-04-20 08:11:11.810792 colabgeek-1.3.5/
--rw-rw-r--   0 sunym     (1000) sunym     (1000)     1067 2024-04-20 06:51:09.000000 colabgeek-1.3.5/LICENSE
--rw-r--r--   0 sunym     (1000) sunym     (1000)     9955 2024-04-20 08:11:11.809792 colabgeek-1.3.5/PKG-INFO
--rw-rw-r--   0 sunym     (1000) sunym     (1000)     9151 2024-04-20 07:59:49.000000 colabgeek-1.3.5/README.md
--rw-rw-r--   0 sunym     (1000) sunym     (1000)      999 2024-04-20 07:59:49.000000 colabgeek-1.3.5/pyproject.toml
--rw-rw-r--   0 sunym     (1000) sunym     (1000)       38 2024-04-20 08:11:11.810792 colabgeek-1.3.5/setup.cfg
-drwxrwxr-x   0 sunym     (1000) sunym     (1000)        0 2024-04-20 08:11:11.806792 colabgeek-1.3.5/src/
-drwxrwxr-x   0 sunym     (1000) sunym     (1000)        0 2024-04-20 08:11:11.807792 colabgeek-1.3.5/src/ColabGeek/
--rw-rw-r--   0 sunym     (1000) sunym     (1000)    34654 2024-04-20 07:59:49.000000 colabgeek-1.3.5/src/ColabGeek/ColabGeek.py
--rw-rw-r--   0 sunym     (1000) sunym     (1000)       25 2024-04-20 06:51:09.000000 colabgeek-1.3.5/src/ColabGeek/__init__.py
-drwxrwxr-x   0 sunym     (1000) sunym     (1000)        0 2024-04-20 08:11:11.809792 colabgeek-1.3.5/src/ColabGeek/shell_scripts/
--rw-rw-r--   0 sunym     (1000) sunym     (1000)      817 2024-04-20 06:51:09.000000 colabgeek-1.3.5/src/ColabGeek/shell_scripts/Install_Homebrew.exp
--rw-rw-r--   0 sunym     (1000) sunym     (1000)      325 2024-04-20 06:51:09.000000 colabgeek-1.3.5/src/ColabGeek/shell_scripts/Install_Jekyll.exp
--rw-rw-r--   0 sunym     (1000) sunym     (1000)      621 2024-04-20 06:51:09.000000 colabgeek-1.3.5/src/ColabGeek/shell_scripts/Install_Miniconda.sh
--rw-rw-r--   0 sunym     (1000) sunym     (1000)      486 2024-04-20 06:51:09.000000 colabgeek-1.3.5/src/ColabGeek/shell_scripts/Install_Ruby.exp
--rw-rw-r--   0 sunym     (1000) sunym     (1000)      443 2024-04-20 06:51:09.000000 colabgeek-1.3.5/src/ColabGeek/shell_scripts/Install_rbenv.exp
--rw-rw-r--   0 sunym     (1000) sunym     (1000)      382 2024-04-20 06:51:09.000000 colabgeek-1.3.5/src/ColabGeek/shell_scripts/Run_Rstudio_server.sh
--rw-rw-r--   0 sunym     (1000) sunym     (1000)     1193 2024-04-20 06:51:09.000000 colabgeek-1.3.5/src/ColabGeek/shell_scripts/Run_code_server.exp
-drwxrwxr-x   0 sunym     (1000) sunym     (1000)        0 2024-04-20 08:11:11.809792 colabgeek-1.3.5/src/ColabGeek.egg-info/
--rw-r--r--   0 sunym     (1000) sunym     (1000)     9955 2024-04-20 08:11:11.000000 colabgeek-1.3.5/src/ColabGeek.egg-info/PKG-INFO
--rw-rw-r--   0 sunym     (1000) sunym     (1000)      603 2024-04-20 08:11:11.000000 colabgeek-1.3.5/src/ColabGeek.egg-info/SOURCES.txt
--rw-rw-r--   0 sunym     (1000) sunym     (1000)        1 2024-04-20 08:11:11.000000 colabgeek-1.3.5/src/ColabGeek.egg-info/dependency_links.txt
--rw-rw-r--   0 sunym     (1000) sunym     (1000)       23 2024-04-20 08:11:11.000000 colabgeek-1.3.5/src/ColabGeek.egg-info/requires.txt
--rw-rw-r--   0 sunym     (1000) sunym     (1000)       10 2024-04-20 08:11:11.000000 colabgeek-1.3.5/src/ColabGeek.egg-info/top_level.txt
+drwxrwxr-x   0 sunym     (1000) sunym     (1000)        0 2024-05-07 05:10:07.598215 colabgeek-1.3.6/
+-rw-rw-r--   0 sunym     (1000) sunym     (1000)     1067 2024-05-07 03:05:41.000000 colabgeek-1.3.6/LICENSE
+-rw-r--r--   0 sunym     (1000) sunym     (1000)    10032 2024-05-07 05:10:07.598215 colabgeek-1.3.6/PKG-INFO
+-rw-rw-r--   0 sunym     (1000) sunym     (1000)     9228 2024-05-07 04:55:36.000000 colabgeek-1.3.6/README.md
+-rw-rw-r--   0 sunym     (1000) sunym     (1000)      999 2024-05-07 04:55:36.000000 colabgeek-1.3.6/pyproject.toml
+-rw-rw-r--   0 sunym     (1000) sunym     (1000)       38 2024-05-07 05:10:07.598215 colabgeek-1.3.6/setup.cfg
+drwxrwxr-x   0 sunym     (1000) sunym     (1000)        0 2024-05-07 05:10:07.593216 colabgeek-1.3.6/src/
+drwxrwxr-x   0 sunym     (1000) sunym     (1000)        0 2024-05-07 05:10:07.595216 colabgeek-1.3.6/src/ColabGeek/
+-rw-rw-r--   0 sunym     (1000) sunym     (1000)    34654 2024-05-07 03:05:41.000000 colabgeek-1.3.6/src/ColabGeek/ColabGeek.py
+-rw-rw-r--   0 sunym     (1000) sunym     (1000)       25 2024-05-07 03:05:41.000000 colabgeek-1.3.6/src/ColabGeek/__init__.py
+drwxrwxr-x   0 sunym     (1000) sunym     (1000)        0 2024-05-07 05:10:07.597216 colabgeek-1.3.6/src/ColabGeek/shell_scripts/
+-rw-rw-r--   0 sunym     (1000) sunym     (1000)      817 2024-05-07 03:05:41.000000 colabgeek-1.3.6/src/ColabGeek/shell_scripts/Install_Homebrew.exp
+-rw-rw-r--   0 sunym     (1000) sunym     (1000)      325 2024-05-07 03:05:41.000000 colabgeek-1.3.6/src/ColabGeek/shell_scripts/Install_Jekyll.exp
+-rw-rw-r--   0 sunym     (1000) sunym     (1000)      621 2024-05-07 03:05:41.000000 colabgeek-1.3.6/src/ColabGeek/shell_scripts/Install_Miniconda.sh
+-rw-rw-r--   0 sunym     (1000) sunym     (1000)      486 2024-05-07 03:05:41.000000 colabgeek-1.3.6/src/ColabGeek/shell_scripts/Install_Ruby.exp
+-rw-rw-r--   0 sunym     (1000) sunym     (1000)      443 2024-05-07 03:05:41.000000 colabgeek-1.3.6/src/ColabGeek/shell_scripts/Install_rbenv.exp
+-rw-rw-r--   0 sunym     (1000) sunym     (1000)      382 2024-05-07 04:55:36.000000 colabgeek-1.3.6/src/ColabGeek/shell_scripts/Run_Rstudio_server.sh
+-rw-rw-r--   0 sunym     (1000) sunym     (1000)     1193 2024-05-07 03:05:41.000000 colabgeek-1.3.6/src/ColabGeek/shell_scripts/Run_code_server.exp
+drwxrwxr-x   0 sunym     (1000) sunym     (1000)        0 2024-05-07 05:10:07.597216 colabgeek-1.3.6/src/ColabGeek.egg-info/
+-rw-r--r--   0 sunym     (1000) sunym     (1000)    10032 2024-05-07 05:10:07.000000 colabgeek-1.3.6/src/ColabGeek.egg-info/PKG-INFO
+-rw-rw-r--   0 sunym     (1000) sunym     (1000)      603 2024-05-07 05:10:07.000000 colabgeek-1.3.6/src/ColabGeek.egg-info/SOURCES.txt
+-rw-rw-r--   0 sunym     (1000) sunym     (1000)        1 2024-05-07 05:10:07.000000 colabgeek-1.3.6/src/ColabGeek.egg-info/dependency_links.txt
+-rw-rw-r--   0 sunym     (1000) sunym     (1000)       23 2024-05-07 05:10:07.000000 colabgeek-1.3.6/src/ColabGeek.egg-info/requires.txt
+-rw-rw-r--   0 sunym     (1000) sunym     (1000)       10 2024-05-07 05:10:07.000000 colabgeek-1.3.6/src/ColabGeek.egg-info/top_level.txt
```

### Comparing `colabgeek-1.3.5/LICENSE` & `colabgeek-1.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `colabgeek-1.3.5/PKG-INFO` & `colabgeek-1.3.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ColabGeek
-Version: 1.3.5
+Version: 1.3.6
 Summary: ColabGeek is designed to help run useful tools on Google Colab, including port forwarding, web IDE and so on. It is worth noting that this package is also compatible with other Ubuntu operating system servers, so try on other platforms as well.
 Author-email: Yiming Sun <yiming.sun12138@gmail.com>
 Project-URL: Homepage, https://github.com/yimingsun12138/ColabGeek
 Project-URL: Bug Tracker, https://github.com/yimingsun12138/ColabGeek/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
@@ -33,21 +33,23 @@
 
 ```python
 import ColabGeek
 
 ColabGeek.update_environment()
 ```
 
-Initiate the Colab session by add linux users and mount Google Drive.
+Initiate the Colab session by adding linux users and mounting Google Drive.
 
 ```python
 main = ColabGeek.ColabSession(user='Knight',password='midnight',mount_GD=True)
 ```
 
-As a cloud computing platform based on Jupyter notebooks, Google Colab does not provide a top-notch comfortable environment for R language data analysis and other non-Python programming. Therefore, this project provides a method for quickly installing other web IDE on Google Colab, enabling it to expand its range of capabilities.
+## Web IDE methods
+
+As a cloud computing platform based on Jupyter notebooks, Google Colab does not provide a top-notch comfortable environment for R language data analysis and other non-Python programming. Therefore, this project provides methods for quickly installing other web IDEs on Google Colab, enabling it to expand its range of capabilities.
 
 ### Run code server
 
 [code server](https://github.com/coder/code-server) is a web IDE provided by Coder that enables developers to write, run and debug code from a web browser. It is built on the open-source Visual Studio Code editor and offers many of the same features, such as code highlighting, auto completion, and debugging.
 
 ```python
 # ColabGeek.Run_code_server has the following parameters:
@@ -83,15 +85,15 @@
 
 ### Run Rstudio server
 
 [Rstudio server](https://posit.co/products/open-source/rstudio-server/) is a web IDE for R programming. With Rstudio server, users can run R scripts, create and manage R projects, develop and test code, and share their work with others. Rstudio server also offers powerful features such as syntax highlighting, code completion, debugging and data visualization.
 
 ```python
 # ColabGeek.Run_Rstudio_server has the following parameters:
-# - port The port you want to run Rstudio on, set to None to use the default port.
+# - port The port you want to run Rstudio server on, set to None to use the default port.
 # - verbose Show the running logs.
 
 main.Run_Rstudio_server()
 ```
 
 ### Run JupyterLab
 [JupyterLab](https://jupyterlab.readthedocs.io/en/stable/index.html) is an interactive web IDE for working with Jupyter notebooks, code, and data. It is a flexible and extensible platform designed to support the entire workflow in data science, scientific computing, and machine learning projects. ColabGeek pulls the [mrdoge/jupyterlab docker image](https://hub.docker.com/r/mrdoge/jupyterlab) from Docker Hub and execute the docker container using [udocker](https://github.com/indigo-dc/udocker). Notice that it is not recommended to run udocker and JupyterLab under user root.
@@ -102,14 +104,16 @@
 # - password The JupyterLab login password, set to None and use the linux user password by default.
 # - mount_Colab Whether map the Colab /content directory to the JupyterLab container /content directory.
 # - verbose Show the running logs.
 
 main.Run_JupyterLab()
 ```
 
+## Port forwarding methods
+
 Google Colab does not allow any internet connections to their servers except the official web interface. So, port forwarding methods are required to proxy the web IDE installed.
 
 ### localtunnel
 
 ```python
 # ColabGeek.Run_localtunnel has the following parameters:
 # - port The port you want to expose to localtunnel, set to None and you will use the default port.
@@ -135,17 +139,19 @@
 ### Cloudflare Tunnel
 
 ```python
 # ColabGeek.Run_Cloudflare_Tunnel has the following parameters:
 # - token The token of your tunnels created on Cloudflare.
 # - verbose Show the running logs.
 
-main.Run_Cloudflare_Tunnel(token = 'replace with your own tunnel token!')
+main.Run_Cloudflare_Tunnel(token='replace with your own tunnel token!')
 ```
 
+## Other methods
+
 ### shadowsocks
 
 Although not allowed by Google and not recommended by myself, building a proxy server using Colab sounds pretty 'Geek'. However, this function only helps to install and run shadowsocks on Colab, and I have no clue how to connect to the shadowsocks server. Just use this method on your own Ubuntu servers, that should work. If you have any good ideas, leave an issue please!
 
 ```python
 # ColabGeek.Run_shadowsocks has the following parameters:
 # - port The server port of shadowsocks, set to None and you will use the default port.
```

### Comparing `colabgeek-1.3.5/README.md` & `colabgeek-1.3.6/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -17,21 +17,23 @@
 
 ```python
 import ColabGeek
 
 ColabGeek.update_environment()
 ```
 
-Initiate the Colab session by add linux users and mount Google Drive.
+Initiate the Colab session by adding linux users and mounting Google Drive.
 
 ```python
 main = ColabGeek.ColabSession(user='Knight',password='midnight',mount_GD=True)
 ```
 
-As a cloud computing platform based on Jupyter notebooks, Google Colab does not provide a top-notch comfortable environment for R language data analysis and other non-Python programming. Therefore, this project provides a method for quickly installing other web IDE on Google Colab, enabling it to expand its range of capabilities.
+## Web IDE methods
+
+As a cloud computing platform based on Jupyter notebooks, Google Colab does not provide a top-notch comfortable environment for R language data analysis and other non-Python programming. Therefore, this project provides methods for quickly installing other web IDEs on Google Colab, enabling it to expand its range of capabilities.
 
 ### Run code server
 
 [code server](https://github.com/coder/code-server) is a web IDE provided by Coder that enables developers to write, run and debug code from a web browser. It is built on the open-source Visual Studio Code editor and offers many of the same features, such as code highlighting, auto completion, and debugging.
 
 ```python
 # ColabGeek.Run_code_server has the following parameters:
@@ -67,15 +69,15 @@
 
 ### Run Rstudio server
 
 [Rstudio server](https://posit.co/products/open-source/rstudio-server/) is a web IDE for R programming. With Rstudio server, users can run R scripts, create and manage R projects, develop and test code, and share their work with others. Rstudio server also offers powerful features such as syntax highlighting, code completion, debugging and data visualization.
 
 ```python
 # ColabGeek.Run_Rstudio_server has the following parameters:
-# - port The port you want to run Rstudio on, set to None to use the default port.
+# - port The port you want to run Rstudio server on, set to None to use the default port.
 # - verbose Show the running logs.
 
 main.Run_Rstudio_server()
 ```
 
 ### Run JupyterLab
 [JupyterLab](https://jupyterlab.readthedocs.io/en/stable/index.html) is an interactive web IDE for working with Jupyter notebooks, code, and data. It is a flexible and extensible platform designed to support the entire workflow in data science, scientific computing, and machine learning projects. ColabGeek pulls the [mrdoge/jupyterlab docker image](https://hub.docker.com/r/mrdoge/jupyterlab) from Docker Hub and execute the docker container using [udocker](https://github.com/indigo-dc/udocker). Notice that it is not recommended to run udocker and JupyterLab under user root.
@@ -86,14 +88,16 @@
 # - password The JupyterLab login password, set to None and use the linux user password by default.
 # - mount_Colab Whether map the Colab /content directory to the JupyterLab container /content directory.
 # - verbose Show the running logs.
 
 main.Run_JupyterLab()
 ```
 
+## Port forwarding methods
+
 Google Colab does not allow any internet connections to their servers except the official web interface. So, port forwarding methods are required to proxy the web IDE installed.
 
 ### localtunnel
 
 ```python
 # ColabGeek.Run_localtunnel has the following parameters:
 # - port The port you want to expose to localtunnel, set to None and you will use the default port.
@@ -119,17 +123,19 @@
 ### Cloudflare Tunnel
 
 ```python
 # ColabGeek.Run_Cloudflare_Tunnel has the following parameters:
 # - token The token of your tunnels created on Cloudflare.
 # - verbose Show the running logs.
 
-main.Run_Cloudflare_Tunnel(token = 'replace with your own tunnel token!')
+main.Run_Cloudflare_Tunnel(token='replace with your own tunnel token!')
 ```
 
+## Other methods
+
 ### shadowsocks
 
 Although not allowed by Google and not recommended by myself, building a proxy server using Colab sounds pretty 'Geek'. However, this function only helps to install and run shadowsocks on Colab, and I have no clue how to connect to the shadowsocks server. Just use this method on your own Ubuntu servers, that should work. If you have any good ideas, leave an issue please!
 
 ```python
 # ColabGeek.Run_shadowsocks has the following parameters:
 # - port The server port of shadowsocks, set to None and you will use the default port.
```

### Comparing `colabgeek-1.3.5/pyproject.toml` & `colabgeek-1.3.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 where = ["src"]
 
 [tool.setuptools.package-data]
 "ColabGeek.shell_scripts" = ["*"]
 
 [project]
 name = "ColabGeek"
-version = "1.3.5"
+version = "1.3.6"
 authors = [
     {name = "Yiming Sun",email = "yiming.sun12138@gmail.com"},
 ]
 description = "ColabGeek is designed to help run useful tools on Google Colab, including port forwarding, web IDE and so on. It is worth noting that this package is also compatible with other Ubuntu operating system servers, so try on other platforms as well."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `colabgeek-1.3.5/src/ColabGeek/ColabGeek.py` & `colabgeek-1.3.6/src/ColabGeek/ColabGeek.py`

 * *Files identical despite different names*

### Comparing `colabgeek-1.3.5/src/ColabGeek/shell_scripts/Install_Homebrew.exp` & `colabgeek-1.3.6/src/ColabGeek/shell_scripts/Install_Homebrew.exp`

 * *Files identical despite different names*

### Comparing `colabgeek-1.3.5/src/ColabGeek/shell_scripts/Install_Miniconda.sh` & `colabgeek-1.3.6/src/ColabGeek/shell_scripts/Install_Miniconda.sh`

 * *Files identical despite different names*

### Comparing `colabgeek-1.3.5/src/ColabGeek/shell_scripts/Run_code_server.exp` & `colabgeek-1.3.6/src/ColabGeek/shell_scripts/Run_code_server.exp`

 * *Files identical despite different names*

### Comparing `colabgeek-1.3.5/src/ColabGeek.egg-info/PKG-INFO` & `colabgeek-1.3.6/src/ColabGeek.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ColabGeek
-Version: 1.3.5
+Version: 1.3.6
 Summary: ColabGeek is designed to help run useful tools on Google Colab, including port forwarding, web IDE and so on. It is worth noting that this package is also compatible with other Ubuntu operating system servers, so try on other platforms as well.
 Author-email: Yiming Sun <yiming.sun12138@gmail.com>
 Project-URL: Homepage, https://github.com/yimingsun12138/ColabGeek
 Project-URL: Bug Tracker, https://github.com/yimingsun12138/ColabGeek/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
@@ -33,21 +33,23 @@
 
 ```python
 import ColabGeek
 
 ColabGeek.update_environment()
 ```
 
-Initiate the Colab session by add linux users and mount Google Drive.
+Initiate the Colab session by adding linux users and mounting Google Drive.
 
 ```python
 main = ColabGeek.ColabSession(user='Knight',password='midnight',mount_GD=True)
 ```
 
-As a cloud computing platform based on Jupyter notebooks, Google Colab does not provide a top-notch comfortable environment for R language data analysis and other non-Python programming. Therefore, this project provides a method for quickly installing other web IDE on Google Colab, enabling it to expand its range of capabilities.
+## Web IDE methods
+
+As a cloud computing platform based on Jupyter notebooks, Google Colab does not provide a top-notch comfortable environment for R language data analysis and other non-Python programming. Therefore, this project provides methods for quickly installing other web IDEs on Google Colab, enabling it to expand its range of capabilities.
 
 ### Run code server
 
 [code server](https://github.com/coder/code-server) is a web IDE provided by Coder that enables developers to write, run and debug code from a web browser. It is built on the open-source Visual Studio Code editor and offers many of the same features, such as code highlighting, auto completion, and debugging.
 
 ```python
 # ColabGeek.Run_code_server has the following parameters:
@@ -83,15 +85,15 @@
 
 ### Run Rstudio server
 
 [Rstudio server](https://posit.co/products/open-source/rstudio-server/) is a web IDE for R programming. With Rstudio server, users can run R scripts, create and manage R projects, develop and test code, and share their work with others. Rstudio server also offers powerful features such as syntax highlighting, code completion, debugging and data visualization.
 
 ```python
 # ColabGeek.Run_Rstudio_server has the following parameters:
-# - port The port you want to run Rstudio on, set to None to use the default port.
+# - port The port you want to run Rstudio server on, set to None to use the default port.
 # - verbose Show the running logs.
 
 main.Run_Rstudio_server()
 ```
 
 ### Run JupyterLab
 [JupyterLab](https://jupyterlab.readthedocs.io/en/stable/index.html) is an interactive web IDE for working with Jupyter notebooks, code, and data. It is a flexible and extensible platform designed to support the entire workflow in data science, scientific computing, and machine learning projects. ColabGeek pulls the [mrdoge/jupyterlab docker image](https://hub.docker.com/r/mrdoge/jupyterlab) from Docker Hub and execute the docker container using [udocker](https://github.com/indigo-dc/udocker). Notice that it is not recommended to run udocker and JupyterLab under user root.
@@ -102,14 +104,16 @@
 # - password The JupyterLab login password, set to None and use the linux user password by default.
 # - mount_Colab Whether map the Colab /content directory to the JupyterLab container /content directory.
 # - verbose Show the running logs.
 
 main.Run_JupyterLab()
 ```
 
+## Port forwarding methods
+
 Google Colab does not allow any internet connections to their servers except the official web interface. So, port forwarding methods are required to proxy the web IDE installed.
 
 ### localtunnel
 
 ```python
 # ColabGeek.Run_localtunnel has the following parameters:
 # - port The port you want to expose to localtunnel, set to None and you will use the default port.
@@ -135,17 +139,19 @@
 ### Cloudflare Tunnel
 
 ```python
 # ColabGeek.Run_Cloudflare_Tunnel has the following parameters:
 # - token The token of your tunnels created on Cloudflare.
 # - verbose Show the running logs.
 
-main.Run_Cloudflare_Tunnel(token = 'replace with your own tunnel token!')
+main.Run_Cloudflare_Tunnel(token='replace with your own tunnel token!')
 ```
 
+## Other methods
+
 ### shadowsocks
 
 Although not allowed by Google and not recommended by myself, building a proxy server using Colab sounds pretty 'Geek'. However, this function only helps to install and run shadowsocks on Colab, and I have no clue how to connect to the shadowsocks server. Just use this method on your own Ubuntu servers, that should work. If you have any good ideas, leave an issue please!
 
 ```python
 # ColabGeek.Run_shadowsocks has the following parameters:
 # - port The server port of shadowsocks, set to None and you will use the default port.
```

### Comparing `colabgeek-1.3.5/src/ColabGeek.egg-info/SOURCES.txt` & `colabgeek-1.3.6/src/ColabGeek.egg-info/SOURCES.txt`

 * *Files identical despite different names*

