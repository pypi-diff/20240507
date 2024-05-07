# Comparing `tmp/slpkg-5.0.6.tar.gz` & `tmp/slpkg-5.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "slpkg-5.0.6.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "slpkg-5.0.7.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `slpkg-5.0.6.tar` & `slpkg-5.0.7.tar`

### file list

```diff
@@ -1,47 +1,48 @@
--rw-r--r--   0        0        0     1945 2024-04-19 17:35:54.000000 slpkg-5.0.6/README.md
--rw-r--r--   0        0        0     1694 2024-04-19 17:35:54.000000 slpkg-5.0.6/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-19 17:35:54.000000 slpkg-5.0.6/slpkg/__init__.py
--rw-r--r--   0        0        0        0 2024-04-19 17:35:54.000000 slpkg-5.0.6/slpkg/binaries/__init__.py
--rw-r--r--   0        0        0     9302 2024-04-19 17:35:54.000000 slpkg-5.0.6/slpkg/binaries/install.py
--rw-r--r--   0        0        0     2084 2024-04-19 17:35:54.000000 slpkg-5.0.6/slpkg/binaries/required.py
--rw-r--r--   0        0        0     1074 2024-04-19 17:35:54.000000 slpkg-5.0.6/slpkg/blacklist.py
--rw-r--r--   0        0        0     6492 2024-04-19 17:35:54.000000 slpkg-5.0.6/slpkg/check_updates.py
--rw-r--r--   0        0        0     1273 2024-04-19 17:35:54.000000 slpkg-5.0.6/slpkg/checks.py
--rw-r--r--   0        0        0     1404 2024-04-19 17:35:54.000000 slpkg-5.0.6/slpkg/checksum.py
--rw-r--r--   0        0        0     4184 2024-04-19 17:35:54.000000 slpkg-5.0.6/slpkg/choose_packages.py
--rw-r--r--   0        0        0      845 2024-04-19 17:35:54.000000 slpkg-5.0.6/slpkg/cleanings.py
--rw-r--r--   0        0        0     5679 2024-04-19 17:35:54.000000 slpkg-5.0.6/slpkg/configs.py
--rw-r--r--   0        0        0     3725 2024-04-19 17:35:54.000000 slpkg-5.0.6/slpkg/dependees.py
--rw-r--r--   0        0        0     1944 2024-04-19 17:35:54.000000 slpkg-5.0.6/slpkg/dialog_box.py
--rw-r--r--   0        0        0     5138 2024-04-19 17:35:54.000000 slpkg-5.0.6/slpkg/dialog_configs.py
--rw-r--r--   0        0        0     4144 2024-04-19 17:35:54.000000 slpkg-5.0.6/slpkg/download_only.py
--rw-r--r--   0        0        0     3992 2024-04-19 17:35:54.000000 slpkg-5.0.6/slpkg/downloader.py
--rw-r--r--   0        0        0      430 2024-04-19 17:35:54.000000 slpkg-5.0.6/slpkg/error_messages.py
--rw-r--r--   0        0        0     1738 2024-04-19 17:35:54.000000 slpkg-5.0.6/slpkg/find_installed.py
--rw-r--r--   0        0        0     1328 2024-04-19 17:35:54.000000 slpkg-5.0.6/slpkg/gpg_verify.py
--rw-r--r--   0        0        0    10735 2024-04-19 17:35:54.000000 slpkg-5.0.6/slpkg/install_data.py
--rw-r--r--   0        0        0     4723 2024-04-19 17:35:54.000000 slpkg-5.0.6/slpkg/load_data.py
--rw-r--r--   0        0        0    27957 2024-04-19 17:35:54.000000 slpkg-5.0.6/slpkg/main.py
--rw-r--r--   0        0        0     6253 2024-04-19 17:35:54.000000 slpkg-5.0.6/slpkg/multi_process.py
--rw-r--r--   0        0        0    11270 2024-04-19 17:35:54.000000 slpkg-5.0.6/slpkg/new_configs.py
--rw-r--r--   0        0        0     2661 2024-04-19 17:35:54.000000 slpkg-5.0.6/slpkg/progress_bar.py
--rw-r--r--   0        0        0     5685 2024-04-19 17:35:54.000000 slpkg-5.0.6/slpkg/remove_packages.py
--rw-r--r--   0        0        0     4816 2024-04-19 17:35:54.000000 slpkg-5.0.6/slpkg/repo_info.py
--rw-r--r--   0        0        0    17927 2024-04-19 17:35:54.000000 slpkg-5.0.6/slpkg/repositories.py
--rw-r--r--   0        0        0        0 2024-04-19 17:35:54.000000 slpkg-5.0.6/slpkg/sbos/__init__.py
--rw-r--r--   0        0        0     1075 2024-04-19 17:35:54.000000 slpkg-5.0.6/slpkg/sbos/dependencies.py
--rw-r--r--   0        0        0     4561 2024-04-19 17:35:54.000000 slpkg-5.0.6/slpkg/sbos/sbo_generate.py
--rw-r--r--   0        0        0    12368 2024-04-19 17:35:54.000000 slpkg-5.0.6/slpkg/sbos/slackbuild.py
--rw-r--r--   0        0        0     3119 2024-04-19 17:35:54.000000 slpkg-5.0.6/slpkg/search.py
--rw-r--r--   0        0        0      587 2024-04-19 17:35:54.000000 slpkg-5.0.6/slpkg/toml_errors.py
--rw-r--r--   0        0        0     4391 2024-04-19 17:35:54.000000 slpkg-5.0.6/slpkg/tracking.py
--rw-r--r--   0        0        0     4557 2024-04-19 17:35:54.000000 slpkg-5.0.6/slpkg/update_repositories.py
--rw-r--r--   0        0        0    10748 2024-04-19 17:35:54.000000 slpkg-5.0.6/slpkg/upgrade.py
--rw-r--r--   0        0        0     8049 2024-04-19 17:35:54.000000 slpkg-5.0.6/slpkg/utilities.py
--rw-r--r--   0        0        0        0 2024-04-19 17:35:54.000000 slpkg-5.0.6/slpkg/views/__init__.py
--rw-r--r--   0        0        0     5768 2024-04-19 17:35:54.000000 slpkg-5.0.6/slpkg/views/asciibox.py
--rw-r--r--   0        0        0     6265 2024-04-19 17:35:54.000000 slpkg-5.0.6/slpkg/views/cli_menu.py
--rw-r--r--   0        0        0      740 2024-04-19 17:35:54.000000 slpkg-5.0.6/slpkg/views/version.py
--rw-r--r--   0        0        0     6932 2024-04-19 17:35:54.000000 slpkg-5.0.6/slpkg/views/view_package.py
--rw-r--r--   0        0        0     9950 2024-04-19 17:35:54.000000 slpkg-5.0.6/slpkg/views/views.py
--rw-r--r--   0        0        0     3424 1970-01-01 00:00:00.000000 slpkg-5.0.6/PKG-INFO
+-rw-r--r--   0        0        0     1945 2024-05-07 07:23:19.000000 slpkg-5.0.7/README.md
+-rw-r--r--   0        0        0     1693 2024-05-07 07:23:19.000000 slpkg-5.0.7/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-07 07:23:19.000000 slpkg-5.0.7/slpkg/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-07 07:23:19.000000 slpkg-5.0.7/slpkg/binaries/__init__.py
+-rw-r--r--   0        0        0     9687 2024-05-07 07:23:19.000000 slpkg-5.0.7/slpkg/binaries/install.py
+-rw-r--r--   0        0        0     2284 2024-05-07 07:23:19.000000 slpkg-5.0.7/slpkg/binaries/required.py
+-rw-r--r--   0        0        0     1117 2024-05-07 07:23:19.000000 slpkg-5.0.7/slpkg/blacklist.py
+-rw-r--r--   0        0        0     7545 2024-05-07 07:23:19.000000 slpkg-5.0.7/slpkg/check_updates.py
+-rw-r--r--   0        0        0     1558 2024-05-07 07:23:19.000000 slpkg-5.0.7/slpkg/checks.py
+-rw-r--r--   0        0        0     1856 2024-05-07 07:23:19.000000 slpkg-5.0.7/slpkg/checksum.py
+-rw-r--r--   0        0        0     4548 2024-05-07 07:23:19.000000 slpkg-5.0.7/slpkg/choose_packages.py
+-rw-r--r--   0        0        0      948 2024-05-07 07:23:19.000000 slpkg-5.0.7/slpkg/cleanings.py
+-rw-r--r--   0        0        0     5722 2024-05-07 07:23:19.000000 slpkg-5.0.7/slpkg/configs.py
+-rw-r--r--   0        0        0     4783 2024-05-07 07:23:19.000000 slpkg-5.0.7/slpkg/dependees.py
+-rw-r--r--   0        0        0     2080 2024-05-07 07:23:19.000000 slpkg-5.0.7/slpkg/dialog_box.py
+-rw-r--r--   0        0        0     5293 2024-05-07 07:23:19.000000 slpkg-5.0.7/slpkg/dialog_configs.py
+-rw-r--r--   0        0        0     4699 2024-05-07 07:23:19.000000 slpkg-5.0.7/slpkg/download_only.py
+-rw-r--r--   0        0        0     4283 2024-05-07 07:23:19.000000 slpkg-5.0.7/slpkg/downloader.py
+-rw-r--r--   0        0        0      667 2024-05-07 07:23:19.000000 slpkg-5.0.7/slpkg/error_messages.py
+-rw-r--r--   0        0        0     2284 2024-05-07 07:23:19.000000 slpkg-5.0.7/slpkg/find_installed.py
+-rw-r--r--   0        0        0     1558 2024-05-07 07:23:19.000000 slpkg-5.0.7/slpkg/gpg_verify.py
+-rw-r--r--   0        0        0    10625 2024-05-07 07:23:19.000000 slpkg-5.0.7/slpkg/install_data.py
+-rw-r--r--   0        0        0     4211 2024-05-07 07:23:19.000000 slpkg-5.0.7/slpkg/load_data.py
+-rw-r--r--   0        0        0    29927 2024-05-07 07:23:19.000000 slpkg-5.0.7/slpkg/main.py
+-rw-r--r--   0        0        0     6630 2024-05-07 07:23:19.000000 slpkg-5.0.7/slpkg/multi_process.py
+-rw-r--r--   0        0        0    12003 2024-05-07 07:23:19.000000 slpkg-5.0.7/slpkg/new_configs.py
+-rw-r--r--   0        0        0     3207 2024-05-07 07:23:19.000000 slpkg-5.0.7/slpkg/progress_bar.py
+-rw-r--r--   0        0        0     6881 2024-05-07 07:23:19.000000 slpkg-5.0.7/slpkg/remove_packages.py
+-rw-r--r--   0        0        0     5389 2024-05-07 07:23:19.000000 slpkg-5.0.7/slpkg/repo_info.py
+-rw-r--r--   0        0        0    18095 2024-05-07 07:23:19.000000 slpkg-5.0.7/slpkg/repositories.py
+-rw-r--r--   0        0        0        0 2024-05-07 07:23:19.000000 slpkg-5.0.7/slpkg/sbos/__init__.py
+-rw-r--r--   0        0        0      858 2024-05-07 07:23:19.000000 slpkg-5.0.7/slpkg/sbos/dependencies.py
+-rw-r--r--   0        0        0     5192 2024-05-07 07:23:19.000000 slpkg-5.0.7/slpkg/sbos/sbo_generate.py
+-rw-r--r--   0        0        0    13290 2024-05-07 07:23:19.000000 slpkg-5.0.7/slpkg/sbos/slackbuild.py
+-rw-r--r--   0        0        0     3684 2024-05-07 07:23:19.000000 slpkg-5.0.7/slpkg/search.py
+-rw-r--r--   0        0        0      712 2024-05-07 07:23:19.000000 slpkg-5.0.7/slpkg/toml_errors.py
+-rw-r--r--   0        0        0     5185 2024-05-07 07:23:19.000000 slpkg-5.0.7/slpkg/tracking.py
+-rw-r--r--   0        0        0     6878 2024-05-07 07:23:19.000000 slpkg-5.0.7/slpkg/update_repositories.py
+-rw-r--r--   0        0        0    11475 2024-05-07 07:23:19.000000 slpkg-5.0.7/slpkg/upgrade.py
+-rw-r--r--   0        0        0     9832 2024-05-07 07:23:19.000000 slpkg-5.0.7/slpkg/utilities.py
+-rw-r--r--   0        0        0        0 2024-05-07 07:23:19.000000 slpkg-5.0.7/slpkg/views/__init__.py
+-rw-r--r--   0        0        0     6757 2024-05-07 07:23:19.000000 slpkg-5.0.7/slpkg/views/asciibox.py
+-rw-r--r--   0        0        0     6696 2024-05-07 07:23:19.000000 slpkg-5.0.7/slpkg/views/cli_menu.py
+-rw-r--r--   0        0        0      690 2024-05-07 07:23:19.000000 slpkg-5.0.7/slpkg/views/version.py
+-rw-r--r--   0        0        0     8072 2024-05-07 07:23:19.000000 slpkg-5.0.7/slpkg/views/view_package.py
+-rw-r--r--   0        0        0     1942 2024-05-07 07:23:19.000000 slpkg-5.0.7/slpkg/views/view_process.py
+-rw-r--r--   0        0        0    12662 2024-05-07 07:23:19.000000 slpkg-5.0.7/slpkg/views/views.py
+-rw-r--r--   0        0        0     3424 1970-01-01 00:00:00.000000 slpkg-5.0.7/PKG-INFO
```

### Comparing `slpkg-5.0.6/README.md` & `slpkg-5.0.7/README.md`

 * *Files identical despite different names*

### Comparing `slpkg-5.0.6/pyproject.toml` & `slpkg-5.0.7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["flit_core>=3.2.0,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "slpkg"
-version = "5.0.6"
+version = "5.0.7"
 authors = [
     {name = "Dimitris Zlatanidis", email = "dslackw@gmail.com"},
 ]
 maintainers = [
     {name = "Dimitris Zlatanidis", email = "dslackw@gmail.com"},
 ]
 description = "Package manager utility for Slackware Linux"
@@ -21,16 +21,15 @@
 	"Natural Language :: English",
     "Environment :: Console",
 	"Operating System :: POSIX",
 	"Operating System :: POSIX :: Linux",
 	"Programming Language :: Python",
 	"Programming Language :: Python :: 3",
 	"Programming Language :: Unix Shell",
-    "Topic :: Utilities",
-    "Topic :: Software Development :: Build Tools",
+    "Topic :: Utilities",    "Topic :: Software Development :: Build Tools",
     "Topic :: System :: Archiving :: Packaging",
     "Topic :: System :: Software Distribution",
     "Topic :: System :: Installation/Setup",
     "Topic :: System :: Systems Administration",
     "Topic :: System :: Software Distribution",
     "Development Status :: 5 - Production/Stable"
 ]
```

### Comparing `slpkg-5.0.6/slpkg/binaries/install.py` & `slpkg-5.0.7/slpkg/binaries/install.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,50 +1,56 @@
 #!/usr/bin/python3
 # -*- coding: utf-8 -*-
 
+
 import os
 import time
 import json
 from pathlib import Path
 from collections import OrderedDict
-from multiprocessing import Process
 
 from slpkg.upgrade import Upgrade
 from slpkg.configs import Configs
 from slpkg.checksum import Md5sum
 from slpkg.views.views import View
 from slpkg.utilities import Utilities
 from slpkg.dialog_box import DialogBox
 from slpkg.gpg_verify import GPGVerify
 from slpkg.downloader import Downloader
 from slpkg.views.asciibox import AsciiBox
 from slpkg.progress_bar import ProgressBar
 from slpkg.multi_process import MultiProcess
 from slpkg.binaries.required import Required
+from slpkg.views.view_process import ViewProcess
+
 
+class Packages(Configs):  # pylint: disable=[R0902]
 
-class Packages(Configs):
+    """
+    Download and install packages with dependencies.
+    """
 
-    def __init__(self, repository: str, data: dict, packages: list, flags: list, mode: str):
+    def __init__(self, repository: str, data: dict, packages: list, flags: list, mode: str):  # pylint: disable=[R0913]
         super(Configs, self).__init__()
         self.repository = repository
         self.data: dict = data
         self.packages: list = packages
         self.flags: list = flags
         self.mode: str = mode
 
         self.utils = Utilities()
         self.dialogbox = DialogBox()
         self.multi_proc = MultiProcess(flags)
         self.view = View(flags, repository, data)
+        self.view_process = ViewProcess(flags)
         self.check_md5 = Md5sum(flags)
         self.download = Downloader(flags)
         self.upgrade = Upgrade(repository, data)
         self.ascii = AsciiBox()
-        self.gpg = GPGVerify()
+        self.gpg = GPGVerify(flags)
         self.progress = ProgressBar()
 
         self.dependencies: list = []
         self.install_order: list = []
         self.binary_packages: list = []
         self.skipped_packages: list = []
         self.progress_message: str = f'{self.cyan}Installing{self.endc}'
@@ -52,21 +58,20 @@
 
         self.option_for_reinstall: bool = self.utils.is_option(
             ('-r', '--reinstall'), flags)
 
         self.option_for_skip_installed: bool = self.utils.is_option(
             ('-k', '--skip-installed'), flags)
 
-        self.option_for_progress_bar: bool = self.utils.is_option(
-            ('-B', '--progress-bar'), flags)
-
         self.packages: list = self.utils.apply_package_pattern(data, packages)
 
     def execute(self) -> None:
-        self.bar_progress()
+        """ Calls methods in order.
+        """
+        self.view_process.message('Resolving dependencies')
         self.creating_dependencies_list()
         self.choose_package_dependencies()
         self.add_dependencies_to_install_order()
         self.clean_the_main_slackbuilds()
         self.add_main_packages_to_install_order()
         self.check_for_skipped()
 
@@ -80,48 +85,60 @@
         self.set_progress_message()
         self.install_packages()
         elapsed_time: float = time.time() - start
 
         self.utils.finished_time(elapsed_time)
 
     def creating_dependencies_list(self) -> None:
+        """ Creating the full list o f dependencies.
+        """
         for package in self.packages:
             dependencies: tuple = Required(self.data, package, self.flags).resolve()
 
             for dependency in dependencies:
                 self.dependencies.append(dependency)
 
         self.dependencies: list = list(OrderedDict.fromkeys(self.dependencies))
 
     def add_dependencies_to_install_order(self) -> None:
+        """ Adds dependencies in order to install.
+        """
         self.install_order.extend(self.dependencies)
 
     def clean_the_main_slackbuilds(self) -> None:
+        """ Removes packages that already listed in dependencies.
+        """
         for dependency in self.dependencies:
             if dependency in self.packages:
                 self.packages.remove(dependency)
 
     def add_main_packages_to_install_order(self) -> None:
+        """ Adds main packages in order to install.
+        """
         self.install_order.extend(self.packages)
 
-    def check_for_skipped(self):
+    def check_for_skipped(self) -> None:
+        """ Skip packages by user.
+        """
         if self.option_for_skip_installed:
             for name in self.install_order:
                 installed: str = self.utils.is_package_installed(name)
                 if installed:
                     self.skipped_packages.append(name)
 
         # Remove packages from skipped packages.
         self.install_order: list = [pkg for pkg in self.install_order if pkg not in self.skipped_packages]
 
     def crating_the_package_urls_list(self) -> None:
+        """ Prepare package urls for downloading.
+        """
         packages: dict = {}
         asc_files: list = []
         if self.install_order:
-            print(f'\rPrepare sources for downloading... ', end='')
+            self.view_process.message('Prepare sources for downloading')
             for pkg in self.install_order:
                 package: str = self.data[pkg]['package']
                 mirror: str = self.data[pkg]['mirror']
                 location: str = self.data[pkg]['location']
                 url: list = [f'{mirror}{location}/{package}']
                 asc_url: list = [f'{mirror}{location}/{package}.asc']
                 asc_file: Path = Path(self.tmp_slpkg, f'{package}.asc')
@@ -130,32 +147,41 @@
                 if self.gpg_verification:
                     packages[f'{pkg}.asc'] = (asc_url, self.tmp_slpkg)
                     asc_files.append(asc_file)
 
                 self.binary_packages.append(package)
                 self.utils.remove_file_if_exists(self.tmp_slpkg, package)
 
-            print(f'{self.bgreen}{self.ascii.done}{self.endc}')
+            self.view_process.done()
             self.download_the_binary_packages(packages)
             if self.gpg_verification:
                 self.gpg.verify(asc_files)
 
     def download_the_binary_packages(self, packages: dict) -> None:
+        """ Download the packages.
+
+        Args:
+            packages (dict): Packages for downloading.
+        """
         if packages:
             print(f'Started to download total ({self.cyan}{len(packages)}{self.endc}) packages:\n')
             self.download.download(packages)
             print()
 
     def checksum_binary_packages(self) -> None:
+        """ Checksum packages.
+        """
         for package in self.binary_packages:
             name: str = self.utils.split_package(Path(package).stem)['name']
             pkg_checksum: str = self.data[name]['checksum']
             self.check_md5.md5sum(self.tmp_slpkg, package, pkg_checksum)
 
     def install_packages(self) -> None:
+        """ Install the packages.
+        """
         # Remove old slpkg.log file.
         if self.slpkg_log_file.is_file():
             self.slpkg_log_file.unlink()
 
         if self.binary_packages:
             print(f'Started the processing of ({self.cyan}{len(self.binary_packages)}{self.endc}) packages:\n')
 
@@ -165,34 +191,43 @@
                     command: str = f'{self.reinstall} {self.tmp_slpkg}/{package}'
 
                 self.multi_proc.process_and_log(command, package, self.progress_message)
                 name: str = self.utils.split_package(package)['name']
                 self.write_deps_log(name)
 
     def write_deps_log(self, name: str) -> None:
+        """ Create log file with installed packages with dependencies.
+
+        Args:
+            name (str): Package name.
+        """
         deps: dict = {}
         deps_logs: dict = {}
         installed_requires: list = []
         requires: tuple = Required(self.data, name, self.flags).resolve()
         # Verify for installation.
         for req in requires:
             if self.utils.is_package_installed(req):
                 installed_requires.append(req)
 
         deps[name] = installed_requires
         if self.deps_log_file.is_file():
             deps_logs: dict = self.utils.read_json_file(self.deps_log_file)
             deps_logs.update(deps)
-        self.deps_log_file.write_text(json.dumps(deps_logs, indent=4))
+        self.deps_log_file.write_text(json.dumps(deps_logs, indent=4), encoding='utf-8')
 
     def set_progress_message(self) -> None:
+        """ Set message for upgrade method.
+        """
         if self.mode == 'upgrade' or self.option_for_reinstall:
             self.progress_message: str = f'{self.violet}Upgrading{self.endc}'
 
     def choose_package_dependencies(self) -> None:
+        """ Choose dependencies for install with dialog tool.
+        """
         if self.dependencies and self.dialog:
             height: int = 10
             width: int = 70
             list_height: int = 0
             choices: list = []
             title: str = ' Choose dependencies you want to install '
 
@@ -210,32 +245,15 @@
                     status: bool = True
 
                 if self.option_for_reinstall:
                     status: bool = True
 
                 choices.extend([(package, repo_ver, status, help_text)])
 
-            self.done_process()
+            self.view_process.done()
 
             text: str = f'There are {len(choices)} dependencies:'
-            code, self.dependencies = self.dialogbox.checklist(text, title, height, width, list_height, choices)
+            code, self.dependencies = self.dialogbox.checklist(text, title, height, width, list_height, choices)  # pylint: disable=[W0612]
 
             os.system('clear')
         else:
-            self.done_process()
-
-    def bar_progress(self) -> None:
-        if self.progress_bar or self.option_for_progress_bar:
-            message: str = 'Resolving dependencies'
-            self.bar_process = Process(target=self.progress.progress_bar, args=(message,))
-            self.bar_process.start()
-        else:
-            print('\rResolving dependencies... ', end='')
-
-    def done_process(self) -> None:
-        if self.progress_bar or self.option_for_progress_bar:
-            time.sleep(0.1)
-            self.bar_process.terminate()
-            self.bar_process.join()
-            print('\x1b[?25h')
-        else:
-            print(f'{self.bgreen}{self.ascii.done}{self.endc}')
+            self.view_process.done()
```

### Comparing `slpkg-5.0.6/slpkg/binaries/required.py` & `slpkg-5.0.7/slpkg/binaries/required.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,22 @@
 #!/usr/bin/python3
 # -*- coding: utf-8 -*-
 
+
 from slpkg.utilities import Utilities
 from slpkg.repositories import Repositories
 
 
 class Required:
-    """ Creates a tuple of dependencies with
-    the right order to install. """
+
+    """
+    Creates a tuple of dependencies with
+    the right order to install.
+    """
+
     __slots__ = ('data', 'name', 'flags', 'repos', 'utils',
                  'full_requires', 'repository_packages',
                  'option_for_resolve_off')
 
     def __init__(self, data: dict, name: str, flags: list):
         self.data: dict = data
         self.name: str = name
@@ -29,27 +34,37 @@
 
         self.repository_packages: tuple = tuple(self.data.keys())
 
         self.option_for_resolve_off: bool = self.utils.is_option(
             ('-O', '--resolve-off'), flags)
 
     def resolve(self) -> tuple:
-        """ Resolve the dependencies. """
+        """ Resolve the dependencies.
+        """
         dependencies: tuple = ()
         if not self.option_for_resolve_off:
             requires: list[str] = self.remove_deps(self.data[self.name]['requires'])
 
             # Resolve dependencies for some special repos.
             if not self.full_requires:
                 for require in requires:
+
                     sub_requires: list[str] = self.remove_deps(self.data[require]['requires'])
                     for sub in sub_requires:
-                        requires.append(sub)
+                        if sub not in requires:
+                            requires.append(sub)
 
             requires.reverse()
             dependencies: tuple = tuple(dict.fromkeys(requires))
 
         return dependencies
 
     def remove_deps(self, requires: list) -> list:
-        """ Remove requirements that not in the repository. """
+        """Remove requirements that not in the repository.
+
+        Args:
+            requires (list): List of requires.
+
+        Returns:
+            list: List of packages name.
+        """
         return [req for req in requires if req in self.repository_packages]
```

### Comparing `slpkg-5.0.6/slpkg/blacklist.py` & `slpkg-5.0.7/slpkg/blacklist.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,29 +1,33 @@
 #!/usr/bin/python3
 # -*- coding: utf-8 -*-
 
+
 try:
     import tomli
 except ModuleNotFoundError:
     import tomllib as tomli
 
 from pathlib import Path
 
 from slpkg.configs import Configs
 from slpkg.toml_errors import TomlErrors
 
 
-class Blacklist(Configs):
-    """ Reads and returns the blacklist. """
+class Blacklist(Configs):  # pylint: disable=[R0903]
+
+    """
+    Reads and returns the blacklist.
+    """
 
     def __init__(self):
         super(Configs, self).__init__()
 
         self.toml_errors = TomlErrors()
-        self.blacklist_file_toml = Path(self.etc_path, 'blacklist.toml')
+        self.blacklist_file_toml: Path = Path(self.etc_path, 'blacklist.toml')
 
     def packages(self) -> tuple:
         """ Reads the blacklist file. """
         packages: tuple = tuple()
         if self.blacklist_file_toml.is_file():
             try:
                 with open(self.blacklist_file_toml, 'rb') as black_file:
```

### Comparing `slpkg-5.0.6/slpkg/check_updates.py` & `slpkg-5.0.7/slpkg/check_updates.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,25 +1,29 @@
 #!/usr/bin/python3
 # -*- coding: utf-8 -*-
 
+
 import os
 from pathlib import Path
 from multiprocessing import Process, Queue
 from urllib3.exceptions import HTTPError, NewConnectionError
 from urllib3 import PoolManager, ProxyManager, make_headers
 
 from slpkg.configs import Configs
 from slpkg.repo_info import RepoInfo
 from slpkg.utilities import Utilities
 from slpkg.progress_bar import ProgressBar
 from slpkg.repositories import Repositories
 
 
-class CheckUpdates(Configs):
-    """ Check for changes in the ChangeLog file. """
+class CheckUpdates(Configs):  # pylint: disable=[R0902]
+
+    """
+    Checks for changes in the ChangeLog files.
+    """
 
     def __init__(self, flags: list, repository: str):
         super(Configs, self).__init__()
         self.flags: list = flags
         self.repository: str = repository
 
         self.utils = Utilities()
@@ -39,40 +43,68 @@
 
         self.option_for_check: bool = self.utils.is_option(
             ('-c', '--check'), flags)
 
         self.option_for_progress_bar: bool = self.utils.is_option(
             ('-B', '--progress-bar'), flags)
 
-    def check_the_repositories(self, queue=None) -> None:
+    def check_the_repositories(self, queue: str = None) -> None:
+        """ Saves checks to a dictionary.
+
+        Args:
+            queue (str, optional): Puts attributes to the queue.
+        """
         if self.option_for_repository:
             self.save_the_compares(self.repository)
         else:
             for repo, enable in self.repos.repositories.items():
                 if enable['enable']:
                     self.save_the_compares(repo)
 
         if queue is not None:
             queue.put(self.compare)
             queue.put(self.error_connected)
 
     def save_the_compares(self, repo: str) -> None:
-        local_chg_txt: Path = Path(self.repos.repositories[repo]['path'],
-                                   self.repos.repositories[repo]['changelog_txt'])
-        repo_chg_txt: str = (f"{self.repos.repositories[repo]['mirror_changelog']}"
-                             f"{self.repos.repositories[repo]['changelog_txt']}")
+        """ Saves compares to a dictionary.
+
+        Args:
+            repo (str): Repository name.
+        """
+        local_chg_txt: Path = Path(
+            self.repos.repositories[repo]['path'],
+            self.repos.repositories[repo]['changelog_txt']
+        )
+
+        repo_chg_txt: str = (
+            f"{self.repos.repositories[repo]['mirror_changelog']}"
+            f"{self.repos.repositories[repo]['changelog_txt']}"
+        )
         repo_data_file: Path = Path(self.repos.repositories[repo]['path'],
                                     self.repos.data_json)
 
         if not repo_data_file.is_file():
             self.compare[repo] = True
         else:
-            self.compare[repo] = self.compare_the_changelogs(local_chg_txt, repo_chg_txt)
+            self.compare[repo] = self.compare_the_changelogs(
+                local_chg_txt, repo_chg_txt)
 
     def compare_the_changelogs(self, local_chg_txt: Path, repo_chg_txt: str) -> bool:
+        """ Compares the two ChangeLog files for changes.
+
+        Args:
+            local_chg_txt (Path): Path to local ChangeLog file.
+            repo_chg_txt (str): Mirror or remote ChangeLog file.
+
+        Returns:
+            bool: True of False.
+
+        Raises:
+            SystemExit: For keyboard interrupt.
+        """
         local_size: int = 0
         repo_size: int = 0
 
         if self.proxy_address.startswith('http'):
             self.set_http_proxy_server()
 
         if self.proxy_address.startswith('socks'):
@@ -84,42 +116,50 @@
 
         try:  # Get repository changelog file size.
             repo = self.http.request(
                 'GET', repo_chg_txt,
                 retries=self.urllib_retries,
                 redirect=self.urllib_redirect)
             repo_size: int = int(repo.headers.get('content-length', 0))
-        except KeyboardInterrupt:
-            raise SystemExit(1)
+        except KeyboardInterrupt as e:
+            raise SystemExit(1) from e
         except (HTTPError, NewConnectionError):
             self.error_connected.append(repo_chg_txt)
 
         if repo_size == 0:
             return False
 
         return local_size != repo_size
 
     def check_for_error_connected(self) -> None:
+        """ Checks for error connected and prints a message.
+        """
         if self.error_connected:
             print(f'\n{self.endc}Failed connected to the mirrors:\n')
             for repo in self.error_connected:
                 print(f'{self.red}>{self.endc} {repo}')
 
     def set_http_proxy_server(self) -> None:
+        """ Sets for HTTP proxy server.
+        """
         self.http = ProxyManager(f'{self.proxy_address}', headers=self.proxy_default_headers)
 
     def set_socks_proxy_server(self) -> None:
+        """ Sets for proxy server.
+        """
         try:  # Try to import PySocks if it's installed.
-            from urllib3.contrib.socks import SOCKSProxyManager
+            from urllib3.contrib.socks import SOCKSProxyManager  # pylint: disable=[W0621,C0415]
         except (ModuleNotFoundError, ImportError) as error:
             print(error)
         # https://urllib3.readthedocs.io/en/stable/advanced-usage.html#socks-proxies
         self.http = SOCKSProxyManager(f'{self.proxy_address}', headers=self.proxy_default_headers)
 
     def view_messages(self) -> None:
+        """ Prints for update messages.
+        """
         repo_for_update: list = []
         for repo, comp in self.compare.items():
             if comp:
                 repo_for_update.append(repo)
 
         if repo_for_update:
             last_updates: dict = self.repo_info.repo_information()
@@ -140,17 +180,22 @@
         else:
             print(f'\n{self.endc}{self.yellow}No updated packages since the last check.{self.endc}')
 
         if self.option_for_check:
             print()
 
     def updates(self) -> dict:
+        """ Calls methods in parallel with progress tool or single.
+
+        Returns:
+            dict: Description
+        """
         message: str = 'Checking for news, please wait'
-        if self.progress_bar or self.option_for_progress_bar:
-            queue = Queue()
+        if self.progress_bar_conf or self.option_for_progress_bar:
+            queue: Queue = Queue()
 
             # Starting multiprocessing
             process_1 = Process(target=self.check_the_repositories, args=(queue,))
             process_2 = Process(target=self.progress.progress_bar, args=(message,))
 
             process_1.start()
             process_2.start()
```

### Comparing `slpkg-5.0.6/slpkg/checks.py` & `slpkg-5.0.7/slpkg/checks.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,38 +1,52 @@
 #!/usr/bin/python3
 # -*- coding: utf-8 -*-
 
+
 from slpkg.configs import Configs
 from slpkg.utilities import Utilities
 from slpkg.error_messages import Errors
 
 
 class Check(Configs):
-    """ Some checks before proceed. """
+
+    """
+    Some checks before proceed.
+    """
 
     def __init__(self, repository: str):
         super(Configs, self).__init__()
         self.repository = repository
 
         self.errors = Errors()
         self.utils = Utilities()
 
     def package_exists_in_the_database(self, packages: list, data: dict) -> None:
+        """ Check if the package exist if not prints a message.
+
+        Args:
+            packages (list): List of packages.
+            data (dict): Repository data.
+        """
         not_packages: list = []
 
         for pkg in packages:
             if not data.get(pkg) and pkg != '*':
                 not_packages.append(pkg)
 
         if not_packages:
             self.errors.raise_error_message(f"Packages '{', '.join(not_packages)}' does not exists",
                                             exit_status=1)
 
     def is_package_installed(self, packages: list) -> None:
-        """ Checking for installed packages. """
+        """Checking for installed packages and prints message if not.
+
+        Args:
+            packages (list): List of packages.
+        """
         not_found: list = []
 
         for pkg in packages:
             if not self.utils.is_package_installed(pkg):
                 not_found.append(pkg)
 
         if not_found:
```

### Comparing `slpkg-5.0.6/slpkg/choose_packages.py` & `slpkg-5.0.7/slpkg/choose_packages.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,33 +1,50 @@
 #!/usr/bin/python3
 # -*- coding: utf-8 -*-
 
+
 import os
 
 from slpkg.configs import Configs
 from slpkg.utilities import Utilities
 from slpkg.dialog_box import DialogBox
 
 
 class Choose(Configs):
-    """ Choose packages with dialog utility and -S, --search flag. """
+
+    """
+    Choose packages with dialog utility and -S, --search flag.
+    """
 
     def __init__(self, repository: str):
         super(Configs, self).__init__()
         self.repository: str = repository
 
         self.utils = Utilities()
         self.dialogbox = DialogBox()
 
         self.choices: list = []
         self.height: int = 10
         self.width: int = 70
         self.list_height: int = 0
 
     def packages(self, data: dict, packages: list, method: str) -> list:
+        """ Calls methods to choosing packages via dialog tool.
+
+        Args:
+            data (dict): Repository data.
+            packages (list): List of packages.
+            method (str): Type of method.
+
+        Returns:
+            list: Name of packages.
+
+        Raises:
+            SystemExit: Exit code 0.
+        """
         if self.dialog:
             title: str = f' Choose packages you want to {method} '
 
             if method in ('remove', 'find'):
                 self.choose_from_installed(packages)
             elif method == 'upgrade':
                 title: str = f' Choose packages you want to {method} or add '
@@ -46,24 +63,26 @@
                 raise SystemExit(0)
 
             os.system('clear')
 
         return packages
 
     def choose_from_installed(self, packages: list) -> None:
-        """ Choose installed packages for remove or find. """
+        """ Choose installed packages for remove or find.
+        """
         for name, package in self.utils.all_installed().items():
             version: str = self.utils.split_package(package)['version']
 
             for pkg in sorted(packages):
                 if pkg in name or pkg == '*':
                     self.choices.extend([(name, version, False, f'Package: {package}')])
 
     def choose_for_upgraded(self, data: dict, packages: list) -> None:
-        """ Choose packages that they will going to upgrade. """
+        """ Choose packages that they will going to upgrade.
+        """
         for package in sorted(packages):
 
             inst_package: str = self.utils.is_package_installed(package)
             inst_package_version: str = self.utils.split_package(inst_package)['version']
             inst_package_build: str = self.utils.split_package(inst_package)['build']
 
             repo_ver: str = data[package]['version']
@@ -76,15 +95,16 @@
             else:
                 self.choices.extend(
                     [(package, f'{inst_package_version} -> {repo_ver}', True,
                         f'Installed: {package}-{inst_package_version} Build: {inst_package_build} -> '
                         f'Available: {repo_ver} Build: {repo_build_tag}')])
 
     def choose_for_others(self, data: dict, packages: list) -> None:
-        """ Choose packages for others methods like install, tracking etc. """
+        """ Choose packages for others methods like install, tracking etc.
+        """
         if self.repository == '*':
             for pkg in sorted(packages):
                 for repo_name, repo_data in data.items():
                     for package in repo_data.keys():
                         if pkg in package or pkg == '*':
                             version: str = repo_data[package]['version']
                             self.choices.extend([(package, version, False, f'Package: {package}-{version} '
```

### Comparing `slpkg-5.0.6/slpkg/cleanings.py` & `slpkg-5.0.7/slpkg/cleanings.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,31 +1,35 @@
 #!/usr/bin/python3
 # -*- coding: utf-8 -*-
 
+
 from slpkg.configs import Configs
 from slpkg.utilities import Utilities
 from slpkg.views.views import View
 
 
-class Cleanings(Configs):
-    """ Cleans the logs from packages. """
+class Cleanings(Configs):  # pylint: disable=[R0903]
+    """ Cleans the logs from packages.
+    """
 
     def __init__(self):
         super(Configs, self).__init__()
 
         self.view = View()
         self.utils = Utilities()
 
     def tmp(self) -> None:
+        """ Delete files and folders in /tmp/slpkg/ folder.
+        """
         print('Deleting of local data:\n')
 
         for file in self.tmp_slpkg.rglob('*'):
             print(f"  {self.bred}>{self.endc} {file}")
 
         print(f"\n{self.prog_name}: {self.bold}{self.bred}WARNING{self.endc}: All the files and "
               f"folders will delete!")
 
         self.view.question()
 
         self.utils.remove_folder_if_exists(self.tmp_slpkg)
         self.utils.create_directory(self.build_path)
-        print(f'Successfully cleared!\n')
+        print('Successfully cleared!\n')
```

### Comparing `slpkg-5.0.6/slpkg/configs.py` & `slpkg-5.0.7/slpkg/configs.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 #!/usr/bin/python3
 # -*- coding: utf-8 -*-
 
+
 try:
     import tomli
 except ModuleNotFoundError:
     import tomllib as tomli
 
 import platform
 from typing import Any
 from pathlib import Path
 from dataclasses import dataclass
 
 from slpkg.toml_errors import TomlErrors
 
 
 @dataclass
-class Configs:
+class Configs:  # pylint: disable=[R0902]
     """ Default configurations. """
     toml_errors = TomlErrors()
 
     prog_name: str = 'slpkg'
     os_arch: str = platform.machine()
     tmp_path: Path = Path('/tmp')
     tmp_slpkg: Path = Path(tmp_path, prog_name)
@@ -50,15 +51,15 @@
     curl_options: str = ''
     lftp_get_options: str = '-c get -e'
     lftp_mirror_options: str = '-c mirror --parallel=100 --only-newer --delete'
     ascii_characters: bool = True
     ask_question: bool = True
     parallel_downloads: bool = False
     maximum_parallel: int = 5
-    progress_bar: bool = False
+    progress_bar_conf: bool = False
     progress_spinner: str = 'pixel'
     spinner_color: str = 'green'
     border_color: str = 'bold_green'
     process_log: bool = True
 
     urllib_retries: Any = False
     urllib_redirect: Any = False
@@ -97,30 +98,30 @@
             curl_options: str = config['curl_options']
             lftp_get_options: str = config['lftp_get_options']
             lftp_mirror_options: str = config['lftp_mirror_options']
             ascii_characters: bool = config['ascii_characters']
             file_list_suffix: str = config['file_list_suffix']
             parallel_downloads: bool = config['parallel_downloads']
             maximum_parallel: int = config['maximum_parallel']
-            progress_bar: bool = config['progress_bar']
+            progress_bar_conf: bool = config['progress_bar']
             progress_spinner: str = config['progress_spinner']
             spinner_color: str = config['spinner_color']
             border_color: str = config['border_color']
             process_log: bool = config['process_log']
 
             urllib_retries: Any = config['urllib_retries']
             urllib_redirect: Any = config['urllib_redirect']
             urllib_timeout: float = config['urllib_timeout']
 
             proxy_address: str = config['proxy_address']
             proxy_username: str = config['proxy_username']
             proxy_password: str = config['proxy_password']
 
     except (KeyError, tomli.TOMLDecodeError) as error:
-        toml_errors.raise_toml_error_message(error, toml_file='/etc/slpkg/slpkg.toml')
+        toml_errors.raise_toml_error_message(error, toml_file=Path('/etc/slpkg/slpkg.toml'))
 
     blink: str = ''
     bold: str = ''
     red: str = ''
     bred: str = ''
     green: str = ''
     bgreen: str = ''
@@ -141,15 +142,15 @@
         bred: str = f'{bold}{red}'
         green: str = '\x1b[32m'
         bgreen: str = f'{bold}{green}'
         yellow: str = '\x1b[93m'
         byellow: str = f'{bold}{yellow}'
         cyan: str = '\x1b[96m'
         bcyan: str = f'{bold}{cyan}'
-        blue: str = f'\x1b[94m'
+        blue: str = '\x1b[94m'
         bblue: str = f'{bold}{blue}'
         grey: str = '\x1b[38;5;247m'
         violet: str = '\x1b[35m'
         endc: str = '\x1b[0m'
 
     # Creating the paths if not exists
     paths = [
```

### Comparing `slpkg-5.0.6/slpkg/dependees.py` & `slpkg-5.0.7/slpkg/dependees.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,18 +1,22 @@
 #!/usr/bin/python3
 # -*- coding: utf-8 -*-
 
+
 from typing import Generator
 from slpkg.configs import Configs
 from slpkg.utilities import Utilities
 from slpkg.views.asciibox import AsciiBox
 
 
-class Dependees(Configs):
-    """ Prints the packages that depend on. """
+class Dependees(Configs):  # pylint: disable=[R0902]
+
+    """
+    Prints the packages that depend on.
+    """
 
     def __init__(self, data: dict, packages: list, flags: list):
         super(Configs, self).__init__()
         self.data: dict = data
         self.packages: list = packages
         self.flags: list = flags
 
@@ -27,52 +31,84 @@
         self.option_for_full_reverse: bool = self.utils.is_option(
             ('-E', '--full-reverse'), flags)
 
         self.option_for_pkg_version: bool = self.utils.is_option(
             ('-p', '--pkg-version'), flags)
 
     def find(self) -> None:
-        self.view_the_title()
+        """ Calls the methods.
+        """
+        print('The list below shows the packages that dependees on:\n')
+        self.packages: list = self.utils.apply_package_pattern(self.data, self.packages)
 
         for package in self.packages:
             dependees: dict = dict(self.find_requires(package))
             self.view_the_main_package(package)
             self.view_no_dependees(dependees)
             self.view_dependees(dependees)
             self.view_summary_of_dependees(dependees, package)
 
     def set_the_package_version(self, package: str) -> None:
+        """ Set the version of the package.
+
+        Args:
+            package (str): Package name.
+        """
         self.package_version: str = self.data[package]['version']
 
     def find_requires(self, package: str) -> Generator:
-        """ Find requires that package dependees. """
+        """Find requires that package dependees.
+
+        Args:
+            package (str): Package name.
+
+        Yields:
+            Generator: List of names with requires.
+        """
         for name, data in self.data.items():
             if package in data['requires']:
                 yield name, data['requires']
 
-    def view_the_title(self) -> None:
-        print(f"The list below shows the packages that dependees on:\n")
-        self.packages: tuple = tuple(self.utils.apply_package_pattern(self.data, self.packages))
-
     def view_no_dependees(self, dependees: dict) -> None:
+        """ Prints for no dependees.
+
+        Args:
+            dependees (dict): Packages data.
+        """
         if not dependees:
             print(f"{'':>1}{self.cyan}No dependees{self.endc}")
 
     def view_the_main_package(self, package: str) -> None:
+        """ Prints the main package.
+
+        Args:
+            package (str): Package name.
+        """
         print(f'{self.byellow}{package}{self.endc}')
         print(f"{'':>1}{self.llc}{self.hl}", end='')
 
     @staticmethod
     def view_dependency_line(n: int, dependency: str) -> None:
+        """ Prints the dependency line.
+
+        Args:
+            n (int): Line number.
+            dependency (str): Name of dependency.
+        """
         str_dependency: str = f"{'':>4}{dependency}"
         if n == 1:
             str_dependency: str = f"{'':>1}{dependency}"
         print(str_dependency)
 
     def view_dependees(self, dependees: dict) -> None:
+        """ View packages that depend on.
+
+        Args:
+            dependees (dict): Packages data.
+        """
         name_length: int = 0
         if dependees:
             name_length: int = max(len(name) for name in dependees.keys())
         for n, (name, requires) in enumerate(dependees.items(), start=1):
             dependency: str = f'{self.cyan}{name}{self.endc}'
             if self.option_for_pkg_version:
                 self.set_the_package_version(name)
@@ -81,14 +117,27 @@
 
             self.view_dependency_line(n, dependency)
 
             if self.option_for_full_reverse:
                 self.view_full_reverse(n, dependees, requires)
 
     def view_full_reverse(self, n: int, dependees: dict, requires: str) -> None:
+        """ Prints all packages.
+
+        Args:
+            n (int): Number of line.
+            dependees (dict): Packages data.
+            requires (str): Package requires.
+        """
         line_requires: str = f"{'':>5}{self.var}{self.hl} {self.violet}{','.join(requires)}{self.endc}"
         if n == len(dependees):
             line_requires: str = f"{'':>5}{self.llc}{self.hl} {self.violet}{','.join(requires)}{self.endc}"
         print(line_requires)
 
     def view_summary_of_dependees(self, dependees: dict, package: str) -> None:
+        """ Prints the summary.
+
+        Args:
+            dependees (dict): Packages data.
+            package (str): Package name.
+        """
         print(f'\n{self.grey}{len(dependees)} dependees for {package}{self.endc}\n')
```

### Comparing `slpkg-5.0.6/slpkg/dialog_box.py` & `slpkg-5.0.7/slpkg/dialog_box.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 #!/usr/bin/python3
 # -*- coding: utf-8 -*-
 
+
 import locale
-from dialog import Dialog
 from pathlib import Path
 from typing import Union, Tuple
+from dialog import Dialog
 
 from slpkg.configs import Configs
 from slpkg.views.version import Version
 
 locale.setlocale(locale.LC_ALL, '')
 
 
@@ -18,38 +19,43 @@
     def __init__(self):
         super(Configs).__init__()
         self.more_kwargs: dict = {}
 
         self.d = Dialog(dialog="dialog")
         self.d.set_background_title(f'{self.prog_name} {Version().version} - Software Package Manager')
 
-    def checklist(self, text: str, title: str, height: int, width: int,
+    def checklist(self, text: str, title: str, height: int, width: int,  # pylint: disable=[R0913]
                   list_height: int, choices: list) -> Tuple[bool, list]:
-        """ Display a checklist box. """
+        """ Display a checklist box.
+        """
         self.more_kwargs.update(
             {"item_help": True}
         )
 
-        code, tags = self.d.checklist(text=text, choices=choices, title=title, height=height,  width=width,
+        code, tags = self.d.checklist(text=text, choices=choices, title=title, height=height, width=width,  # pylint: disable=[R0913]
                                       list_height=list_height, help_status=True, **self.more_kwargs)
 
         return code, tags
 
-    def mixedform(self, text: str, title: str, elements: list, height: int, width: int, form_height) -> Tuple[bool, list]:
-        """ Display a mixedform box. """
+    def mixedform(self, text: str, title: str, elements: list, height: int, width: int,  # pylint: disable=[R0913]
+                  form_height: int) -> Tuple[bool, list]:
+        """ Display a mixedform box.
+        """
         self.more_kwargs.update(
             {"item_help": True,
              "help_tags": True}
         )
         code, tags = self.d.mixedform(text=text, title=title, elements=elements,  # type: ignore
                                       height=height, width=width, form_height=form_height, help_button=True,
                                       help_status=True, **self.more_kwargs)
 
         return code, tags
 
     def msgbox(self, text: str, height: int, width: int) -> None:
-        """ Display a message box. """
+        """ Display a message box.
+        """
         self.d.msgbox(text, height, width)
 
     def textbox(self, text: Union[str, Path], height: int, width: int) -> None:
-        """ Display a text box. """
+        """ Display a text box.
+        """
         self.d.textbox(text, height, width)
```

### Comparing `slpkg-5.0.6/slpkg/dialog_configs.py` & `slpkg-5.0.7/slpkg/dialog_configs.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,38 +1,45 @@
 #!/usr/bin/python3
 # -*- coding: utf-8 -*-
 
+
 import os
 from pathlib import Path
 
 from slpkg.configs import Configs
 from slpkg.utilities import Utilities
 from slpkg.dialog_box import DialogBox
 from slpkg.error_messages import Errors
 
 
 class FormConfigs(Configs):
 
+    """
+    Edit slpkg.toml config file with dialog utility.
+    """
+
     def __init__(self):
         super(Configs).__init__()
         self.dialogbox = DialogBox()
         self.errors = Errors()
         self.utils = Utilities()
 
         self.orig_configs: list = []
         self.config_file: Path = Path(self.etc_path, f'{self.prog_name}.toml')
 
     def is_dialog_enabled(self) -> None:
-        """ Checking if the dialog box is enabled by the user. """
+        """ Checking if the dialog box is enabled by the user.
+        """
         if not self.dialog:
             self.errors.raise_error_message(f"You should enable the dialog in the "
                                             f"'{self.etc_path}/{self.prog_name}.toml' file", exit_status=1)
 
     def edit(self) -> None:
-        """ Read and write the configuration file. """
+        """ Read and write the configuration file.
+        """
         self.is_dialog_enabled()
         elements: list = []
         height: int = 9
         width: int = 0
         form_height: int = 0
         text: str = f'Edit the configuration file: {self.config_file}'
         title: str = ' Configuration File '
@@ -60,20 +67,22 @@
         if code == 'ok' and check:
             self.write_file(tags)
 
         elif not check:
             self.edit()
 
     def help(self) -> None:
-        """ Load the configuration file on a text box. """
+        """ Load the configuration file on a text box.
+        """
         self.dialogbox.textbox(str(self.config_file), 40, 60)
         self.edit()
 
     def check_configs(self, tags: list) -> bool:
-        """ Check for true of false values. """
+        """ Check for true of false values.
+        """
         keys: list = [
             'COLORS',
             'DIALOG',
             'SILENT_MODE',
             'ASCII_CHARACTERS',
             'ASK_QUESTION',
             'KERNEL_VERSION',
@@ -102,23 +111,25 @@
                 self.dialogbox.msgbox(f"\nError: Value for '{key}' not supported.\n",
                                       height=7, width=60)
                 return False
 
         return True
 
     def read_configs(self) -> None:
-        """ Read the original config file. """
-        with open(self.config_file, 'r') as toml_file:
+        """ Read the original config file.
+        """
+        with open(self.config_file, 'r', encoding='utf-8') as toml_file:
             self.orig_configs: list = toml_file.readlines()
 
     def write_file(self, tags: list) -> None:
-        """ Write the new values to the config file. """
+        """ Write the new values to the config file.
+        """
         self.read_configs()
 
-        with open(self.config_file, 'w') as patch_toml:
+        with open(self.config_file, 'w', encoding='utf-8') as patch_toml:
             for line in self.orig_configs:
                 for key, value in zip(self.configs['configs'].keys(), tags):
 
                     if line.lstrip().startswith(f'{key} ='):
                         line = f'  {key} = "{value}"\n'
 
                     if line.lstrip().startswith(
```

### Comparing `slpkg-5.0.6/slpkg/download_only.py` & `slpkg-5.0.7/slpkg/download_only.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,27 +1,30 @@
 #!/usr/bin/python3
 # -*- coding: utf-8 -*-
 
+
 import time
 import shutil
 from pathlib import Path
 
 from slpkg.configs import Configs
 from slpkg.views.views import View
 from slpkg.utilities import Utilities
 from slpkg.gpg_verify import GPGVerify
 from slpkg.downloader import Downloader
 from slpkg.error_messages import Errors
 from slpkg.views.asciibox import AsciiBox
 from slpkg.repositories import Repositories
 
 
-class DownloadOnly(Configs):
-    """ Download only the sources and the slackbuilds or the packages
-        for binary repositories.
+class DownloadOnly(Configs):  # pylint: disable=[R0902]
+
+    """
+    Download only the sources and the slackbuilds or the packages
+    for binary repositories.
     """
 
     def __init__(self, directory: str, flags: list, data: dict, repository: str):
         super(Configs, self).__init__()
         self.directory: Path = Path(directory)
         self.flags: list = flags
         self.data: dict = data
@@ -29,79 +32,101 @@
 
         self.view = View(flags, repository, data)
         self.download = Downloader(flags)
         self.repos = Repositories()
         self.utils = Utilities()
         self.ascii = AsciiBox()
         self.errors = Errors()
-        self.gpg = GPGVerify()
+        self.gpg = GPGVerify(flags)
 
         self.urls: dict = {}
         self.asc_files: list = []
 
         self.option_for_directory: bool = self.utils.is_option(
             ('-z', '--directory'), flags)
 
-    def packages(self, packages: list) -> None: # type: ignore
+    def packages(self, packages: list) -> None:
+        """ Download the packages.
 
+        Args:
+            packages (list): List of packages.
+        """
         if not self.directory.is_dir():
-            print(self.errors.raise_error_message(f"Path '{self.directory}' does not exist", 1))
+            self.errors.raise_error_message(f"Path '{self.directory}' does not exist", 1)
 
         packages: list = self.utils.apply_package_pattern(self.data, packages)
 
         self.view.download_packages(packages, self.directory)
         self.view.question()
         start: float = time.time()
 
-        print(f'\rPrepare sources for downloading... ', end='')
+        print('\rPrepare sources for downloading... ', end='')
         for pkg in packages:
             if self.repository in [self.repos.sbo_repo_name, self.repos.ponce_repo_name]:
                 self.save_slackbuild_sources(pkg)
                 self.copy_slackbuild_scripts(pkg)
             else:
                 self.save_binary_sources(pkg)
 
         print(f'{self.bgreen}{self.ascii.done}{self.endc}')
         self.download_the_sources()
 
         elapsed_time: float = time.time() - start
         self.utils.finished_time(elapsed_time)
 
     def save_binary_sources(self, name: str) -> None:
+        """ Assign for binary repositories.
+
+        Args:
+            name (str): Package name.
+        """
         package: str = self.data[name]['package']
         mirror: str = self.data[name]['mirror']
         location: str = self.data[name]['location']
         url: str = f'{mirror}{location}/{package}'
         self.urls[name] = ((url,), self.directory)
         asc_url: list = [f'{mirror}{location}/{package}.asc']
         asc_file: Path = Path(self.directory, f'{package}.asc')
 
         if self.gpg_verification:
             self.urls[f'{name}.asc'] = (asc_url, self.directory)
             self.asc_files.append(asc_file)
 
     def save_slackbuild_sources(self, name: str) -> None:
+        """ Assign for sbo repositories.
+
+        Args:
+            name (str): SBo name.
+        """
         if self.os_arch == 'x86_64' and self.data[name]['download64']:
             sources: tuple = self.data[name]['download64']
         else:
             sources: tuple = self.data[name]['download']
         self.urls[name] = (sources, Path(self.directory, name))
 
         if self.gpg_verification and self.repository == self.repos.sbo_repo_name:
             location: str = self.data[name]['location']
             asc_file: Path = Path(self.repos.repositories_path, self.repos.sbo_repo_name,
                                   location, f'{name}{self.repos.sbo_repo_tar_suffix}.asc')
             self.asc_files.append(asc_file)
 
     def copy_slackbuild_scripts(self, name: str) -> None:
-        repo_path_package: Path = Path(self.repos.repositories[self.repository]['path'], self.data[name]['location'], name)
+        """ Copy slackbuilds from local repository to download path.
+
+        Args:
+            name (str): SBo name.
+        """
+        repo_path_package: Path = Path(self.repos.repositories[self.repository]['path'],
+                                       self.data[name]['location'], name)
         if not Path(self.directory, name).is_dir():
             shutil.copytree(repo_path_package, Path(self.directory, name))
 
     def download_the_sources(self) -> None:
+        """ Starts to download the sources.
+        """
         if self.urls:
             print(f'\nStarted to download total ({self.cyan}{len(self.urls)}{self.endc}) sources:\n')
             self.download.download(self.urls)
             print()
 
         if self.gpg_verification and self.repository != self.repos.ponce_repo_name:
             self.gpg.verify(self.asc_files)
```

### Comparing `slpkg-5.0.6/slpkg/downloader.py` & `slpkg-5.0.7/slpkg/downloader.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,24 +1,28 @@
 #!/usr/bin/python3
 # -*- coding: utf-8 -*-
 
+
 import os
-import shutil
 from pathlib import Path
 from multiprocessing import Process, Semaphore
 from urllib.parse import unquote, urlparse
 
 from slpkg.configs import Configs
 from slpkg.utilities import Utilities
 from slpkg.error_messages import Errors
 from slpkg.multi_process import MultiProcess
 from slpkg.views.views import View
 
 
-class Downloader(Configs):
+class Downloader(Configs):  # pylint: disable=[R0902]
+
+    """
+    Downloads the sources using external tools.
+    """
 
     def __init__(self, flags: list):
         super(Configs, self).__init__()
         self.flags: list = flags
 
         self.errors = Errors()
         self.utils = Utilities()
@@ -61,47 +65,67 @@
     def normal_download(self, sources: dict) -> None:
         """ Download sources with normal mode. """
         for urls, path in sources.values():
             for url in urls:
                 self.tools(url, path)
 
     def tools(self, url: str, path: Path) -> None:
+        """ Run the tool to downloading.
+
+        Args:
+            url (str): The URL link.
+            path (Path): Path to save.
+        """
         self.semaphore.acquire()
         url_parse: str = urlparse(url).path
         self.filename: str = unquote(Path(url_parse).name)
 
-        if url.startswith('file'):
-            self.copy_local_binary_file(url)
-        else:
-            try:
-                self.downloader_tools[self.downloader](url, path)
-            except KeyError:
-                self.errors.raise_error_message(f"Downloader '{self.downloader}' not supported", exit_status=1)
+        try:
+            self.downloader_tools[self.downloader](url, path)
+        except KeyError:
+            self.errors.raise_error_message(f"Downloader '{self.downloader}' not supported", exit_status=1)
 
-            self.multi_process.process(self.downloader_command)
-            self.check_if_downloaded(url, path)
+        self.multi_process.process(self.downloader_command)
+        self.check_if_downloaded(url, path)
         self.semaphore.release()
 
-    def copy_local_binary_file(self, url: str) -> None:
-        try:
-            shutil.copy2(Path(url.replace('file:', '')), self.tmp_slpkg)
-            print(f"{self.byellow}Copying{self.endc}: {Path(url.replace('file:', ''))} -> {self.tmp_slpkg}")
-        except FileNotFoundError as error:
-            self.errors.raise_error_message(f'{error}', 1)
-
     def set_wget_downloader(self, url: str, path: Path) -> None:
+        """ Set for wget tool.
+
+        Args:
+            url (str): URL link.
+            path (Path): Path to save.
+        """
         self.downloader_command: str = f'{self.downloader} {self.wget_options} --directory-prefix={path} "{url}"'
 
     def set_curl_downloader(self, url: str, path: Path) -> None:
+        """ Set for curl tool.
+
+        Args:
+            url (str): URL link.
+            path (Path): Path to save.
+        """
         self.downloader_command: str = (f'{self.downloader} {self.curl_options} "{url}" '
                                         f'--output {path}/{self.filename}')
 
     def set_lftp_downloader(self, url: str, path: Path) -> None:
+        """ Set for lftp tool.
+
+        Args:
+            url (str): URL link.
+            path (Path): Path to save.
+        """
         self.downloader_command: str = f'{self.downloader} {self.lftp_get_options} {url} -o {path}'
 
     def check_if_downloaded(self, url: str, path: Path) -> None:
+        """ Checking if file downloaded.
+
+        Args:
+            url (str): URL link.
+            path (Path): Path to check the file.
+        """
         path_file: Path = Path(path, self.filename)
         if not path_file.exists():
             parsed_url = urlparse(url)
             filename: str = os.path.basename(parsed_url.path)
             print(f"{self.red}>{self.endc} Failed to download the file: '{filename}'")
             self.views.question()
```

### Comparing `slpkg-5.0.6/slpkg/find_installed.py` & `slpkg-5.0.7/slpkg/find_installed.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,53 +1,75 @@
 #!/usr/bin/python3
 # -*- coding: utf-8 -*-
 
+
 from slpkg.configs import Configs
 from slpkg.utilities import Utilities
 
 
 class FindInstalled(Configs):
-    """ Find installed packages. """
+
+    """
+    Find installed packages.
+    """
 
     def __init__(self, flags: list, packages: list):
         super(Configs, self).__init__()
         self.packages: list = packages
 
         self.utils = Utilities()
         self.matching: list = []
+        self.total_size: int = 0
 
         self.option_for_no_case: bool = self.utils.is_option(
             ('-m', '--no-case'), flags)
 
     def find(self) -> None:
+        """ Find packages installed packages.
+        """
         self.view_title()
         for package in self.packages:
             for name in self.utils.all_installed().values():
 
                 if package in name or package == '*' or self.is_not_case_sensitive(package, name):
                     self.matching.append(name)
-        self.matched()
+        self.view_matched_packages()
 
     @staticmethod
     def view_title() -> None:
-        print(f'The list below shows the installed packages:\n')
+        """ Prints the title.
+        """
+        print('The list below shows the installed packages:\n')
 
-    def matched(self) -> None:
+    def view_matched_packages(self) -> None:
+        """ Prints the matching packages.
+        """
         if self.matching:
-            self.view_matched_packages()
+            for package in self.matching:
+                name: str = self.utils.split_package(package)['name']
+                pkg_size: int = self.utils.count_file_size(name)
+                size: str = self.utils.convert_file_sizes(pkg_size)
+                self.total_size += pkg_size
+                print(f'{self.cyan}{package}{self.endc} ({size})')
+            self.view_summary()
         else:
             print('\nDoes not match any package.\n')
 
-    def view_matched_packages(self) -> None:
-        for package in self.matching:
-            name: str = self.utils.split_package(package)['name']
-            pkg_size: int = self.utils.count_file_size(name)
-            size: str = self.utils.convert_file_sizes(pkg_size)
-            print(f'{self.cyan}{package}{self.endc} ({size})')
-        self.view_summary()
-
     def view_summary(self) -> None:
-        print(f'\n{self.grey}Total found {len(self.matching)} packages.{self.endc}')
+        """ Prints the summary.
+        """
+        print(f'\n{self.grey}Total found {len(self.matching)} packages with '
+              f'{self.utils.convert_file_sizes(self.total_size)} size.{self.endc}')
 
     def is_not_case_sensitive(self, package: str, name: str) -> bool:
+        """ Checks for case sensitive.
+
+        Args:
+            package (str): Package file.
+            name (str): Name of package.
+
+        Returns:
+            bool: True or False.
+        """
         if self.option_for_no_case:
             return package.lower() in name.lower()
+        return False
```

### Comparing `slpkg-5.0.6/slpkg/gpg_verify.py` & `slpkg-5.0.7/slpkg/gpg_verify.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,40 +1,52 @@
 #!/usr/bin/python3
 # -*- coding: utf-8 -*-
 
+
 import subprocess
 
 from slpkg.configs import Configs
 from slpkg.views.asciibox import AsciiBox
 from slpkg.views.views import View
+from slpkg.views.view_process import ViewProcess
+
 
+class GPGVerify(Configs):  # pylint: disable=[R0903]
 
-class GPGVerify(Configs):
+    """ GPG verify files.
+    """
 
-    def __init__(self):
+    def __init__(self, flags: list):
         super(Configs, self).__init__()
         self.ascii = AsciiBox()
         self.view = View()
+        self.view_process = ViewProcess(flags)
 
     def verify(self, asc_files: list) -> None:
+        """ Verify files with gpg tool.
+
+        Args:
+            asc_files (list): List of files.
+        """
         if self.gpg_verification:
-            verify_message: str = '\rVerify files with GPG... '
+            output: dict = {}
             gpg_command: str = 'gpg --verify'
-            print(verify_message, end='')
+            self.view_process.message('Verify files with GPG')
+
+            for file in asc_files:
+
+                with subprocess.Popen(f'{gpg_command} {file}', shell=True, stdout=subprocess.PIPE,
+                                      stderr=subprocess.STDOUT, text=True) as process:
+
+                    process.wait()
 
-            exit_code: int = 0
-            for i, file in enumerate(asc_files):
-                process = subprocess.Popen(f'{gpg_command} {file}', shell=True, stdout=subprocess.PIPE,
-                                           stderr=subprocess.STDOUT, text=True)
-
-                process.wait()
-
-                if process.returncode != 0:
-                    exit_code: int = process.returncode
-                    if i == 0:
-                        print(f'{self.bred}{self.ascii.failed}{self.endc}')
-                    print(f"{'':>2}Error {process.returncode}: {file.name}")
-
-            if exit_code == 0:
-                print(f'{self.bgreen}{self.ascii.done}{self.endc}')
-            elif exit_code != 0 and self.dialog:
-                self.view.question()
+                    output[file.name] = process.returncode
+
+            all_zero = all(value == 0 for value in output.values())
+            if all_zero:
+                self.view_process.done()
+            else:
+                self.view_process.failed()
+                for file, code in output.items():
+                    if code != 0:
+                        print(f"{'':>2}{self.red}Error{self.endc} {code}: {file}")
+                        self.view.question()
```

### Comparing `slpkg-5.0.6/slpkg/install_data.py` & `slpkg-5.0.7/slpkg/install_data.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 #!/usr/bin/python3
 # -*- coding: utf-8 -*-
 
+
 import re
 import json
 from pathlib import Path
 
 from slpkg.configs import Configs
 from slpkg.utilities import Utilities
 from slpkg.views.asciibox import AsciiBox
 from slpkg.repositories import Repositories
 from slpkg.multi_process import MultiProcess
+from slpkg.views.view_process import ViewProcess
 
 
 class InstallData(Configs):
 
-    def __init__(self):
+    """ Installs data to the repositories path.
+    """
+
+    def __init__(self, flags: list):
         super(Configs, self).__init__()
         self.utils = Utilities()
         self.repos = Repositories()
         self.ascii = AsciiBox()
         self.multi_process = MultiProcess()
-
-    def _import_GPG_KEY(self, mirror: str, gpg_key='GPG-KEY') -> None:
-        if self.gpg_verification:
-            gpg_command: str = 'gpg --quiet --fetch-key'
-            GPG_KEY: str = f'{mirror}{gpg_key}'
-            self.multi_process.process(f'{gpg_command} {GPG_KEY}')
+        self.view_process = ViewProcess(flags)
 
     def write_repo_info(self, changelog_file: Path, info: dict) -> None:
         """ Reads the first date of the changelog file."""
         repo_name: str = info['repo_name']
         full_requires: bool = info['full_requires']
         last_date: str = ''
         repo_info: dict = {}
@@ -44,29 +44,27 @@
             repo_info: dict = self.utils.read_json_file(self.repos.repos_information)
 
         repo_info[repo_name] = {
             'last_updated': last_date,
             'full_requires': full_requires
         }
 
-        self.repos.repos_information.write_text(json.dumps(repo_info, indent=4))
+        self.repos.repos_information.write_text(json.dumps(repo_info, indent=4), encoding='utf-8')
 
-    def view_done_message(self) -> None:
-        print(f'{self.bgreen}{self.ascii.done}{self.endc}\n')
+    def install_sbo_data(self, repo: str) -> None:  # pylint: disable=[R0914]
+        """ Reads the SLACKBUILDS.TXT FILE and creates a json data file.
 
-    def install_sbo_data(self, repo: str) -> None:
-        """
-        Reads the SLACKBUILDS.TXT FILE and creates a json data file.
-        Returns:
+        Args:
+            repo (str): repository name.
+
+        No Longer Returned:
             None.
         """
-        print(f"Updating the database for '{self.cyan}{repo}{self.endc}'... ",
-              end='', flush=True)
-
-        self._import_GPG_KEY(mirror='https://www.slackbuilds.org/')
+        print()
+        self.view_process.message(f'Updating the database for {repo}')
 
         data: dict = {}
         cache: list = []
         names: list = []
         sbo_tags: list = [
             'SLACKBUILD NAME:',
             'SLACKBUILD LOCATION:',
@@ -101,15 +99,15 @@
                 location: str = cache[1].split('/')[1]
                 requires: list = [item for item in cache[8].split() if item in names]
 
                 data[name] = {
                     'location': location,
                     'files': cache[2].split(),
                     'version': version,
-                    'download':  cache[4].split(),
+                    'download': cache[4].split(),
                     'download64': cache[5].split(),
                     'md5sum': cache[6].split(),
                     'md5sum64': cache[7].split(),
                     'requires': requires,
                     'description': cache[9]
                 }
 
@@ -136,31 +134,33 @@
         }
 
         path_changelog: Path = Path(self.repos.repositories[repo]['path'],
                                     self.repos.repositories[repo]['changelog_txt'])
         self.write_repo_info(path_changelog, repo_info)
 
         data_file: Path = Path(self.repos.repositories[repo]['path'], self.repos.data_json)
-        data_file.write_text(json.dumps(data, indent=4))
+        data_file.write_text(json.dumps(data, indent=4), encoding='utf-8')
 
-        self.view_done_message()
+        self.view_process.done()
+        print()
 
-    def install_binary_data(self, repo: str) -> None:
-        """ Install the data for alien repository. """
-        print(f"\nUpdating the database for '{self.cyan}{repo}{self.endc}'... ",
-              end='', flush=True)
+    def install_binary_data(self, repo: str) -> None:  # pylint: disable=[R0912,R0914,R0915]
+        """ Installs the data for binary repositories.
+        Args:
+            repo (str): Description
+        """
+        print()
+        self.view_process.message(f'Updating the database for {repo}')
 
         slack_repos: list = [self.repos.slack_patches_repo_name, self.repos.slack_extra_repo_name]
 
         mirror: str = self.repos.repositories[repo]['mirror_packages']
         if repo in slack_repos:
             mirror: str = self.repos.repositories[repo]['mirror_changelog']
 
-        self._import_GPG_KEY(mirror=mirror)
-
         checksums_dict: dict = {}
         data: dict = {}
         build: str = ''
         arch: str = ''
         requires: list = []
         names: list = []
         full_requires: bool = False
@@ -267,10 +267,11 @@
         }
 
         path_changelog: Path = Path(self.repos.repositories[repo]['path'],
                                     self.repos.repositories[repo]['changelog_txt'])
         self.write_repo_info(path_changelog, repo_info)
 
         data_file: Path = Path(self.repos.repositories[repo]['path'], self.repos.data_json)
-        data_file.write_text(json.dumps(data, indent=4))
+        data_file.write_text(json.dumps(data, indent=4), encoding='utf-8')
 
-        self.view_done_message()
+        self.view_process.done()
+        print()
```

### Comparing `slpkg-5.0.6/slpkg/load_data.py` & `slpkg-5.0.7/slpkg/load_data.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,84 +1,92 @@
 #!/usr/bin/python3
 # -*- coding: utf-8 -*-
 
+
 import json
-import time
 from pathlib import Path
-from multiprocessing import Process
 
 from slpkg.configs import Configs
 from slpkg.utilities import Utilities
 from slpkg.blacklist import Blacklist
 from slpkg.views.asciibox import AsciiBox
-from slpkg.progress_bar import ProgressBar
 from slpkg.repositories import Repositories
+from slpkg.views.view_process import ViewProcess
 
 
 class LoadData(Configs):
 
-    def __init__(self, flags=None):
+    """ Reads data form json file and load to dictionary.
+    """
+
+    def __init__(self, flags: list = None):
+        super(Configs, self).__init__()
+
+        if flags is None:
+            flags = []
+
         self.repos = Repositories()
         self.utils = Utilities()
         self.black = Blacklist()
         self.ascii = AsciiBox()
-        self.progress = ProgressBar()
-
-        if flags is None:
-            flags = []
+        self.view_process = ViewProcess(flags)
 
-        self.bar_process = None
+    def load(self, repository: str, message: bool = True) -> dict:
+        """ Load data to the dictionary.
 
-        self.option_for_progress_bar: bool = self.utils.is_option(
-            ('-B', '--progress-bar'), flags)
+        Args:
+            repository (str): Repository name.
+            message (bool, optional): Prints or not progress message.
 
-    def load(self, repository: str, message=True) -> dict:
+        Returns:
+            dict: Dictionary data.
+        """
         if message:
-            self.bar_progress()
+            self.view_process.message('Database loading')
 
         data: dict = {}
         if repository == '*':
-            for repo, item in self.repos.repositories.items():
-                if item['enable']:  # Check if the repository is enabled
-                    json_data_file: Path = Path(self.repos.repositories[repo]['path'], self.repos.data_json)
+            for repo, value in self.repos.repositories.items():
+                if value['enable']:  # Check if the repository is enabled
+                    json_data_file: Path = Path(value['path'], self.repos.data_json)
                     data[repo] = self.read_data_file(json_data_file)
         else:
             json_data_file: Path = Path(self.repos.repositories[repository]['path'], self.repos.data_json)
 
             data: dict = self.read_data_file(json_data_file)
 
         blacklist: tuple = self.black.packages()
         if blacklist:
             if repository == '*':
                 self._remove_blacklist_from_all_repos(data)
             else:
                 self._remove_blacklist_from_a_repo(data)
 
         if message:
-            self.done_process()
-            # print(f'{self.bgreen}{self.ascii.done}{self.endc}')
+            self.view_process.done()
+
         return data
 
     def read_data_file(self, file: Path) -> dict:
         """
         Read JSON data from the file.
         Args:
             file: Path file for reading.
         Returns:
             Dictionary with data.
         """
         json_data: dict = {}
         try:
             json_data: dict = json.loads(file.read_text(encoding='utf-8'))
-        except FileNotFoundError:
+        except FileNotFoundError as e:
             print(f'{self.bred}{self.ascii.failed}{self.endc}')
             print(f'\nFile {file} not found!')
             print('\nNeed to update the database first, please run:\n')
             print(f"{'':>2} $ {self.green}slpkg update{self.endc}\n")
-            raise SystemExit(1)
+            raise SystemExit(1) from e
         except json.decoder.JSONDecodeError:
             pass
         return json_data
 
     def _remove_blacklist_from_all_repos(self, data: dict) -> dict:
         # Remove blacklist packages from keys.
         for name, repo in data.items():
@@ -109,24 +117,7 @@
         for pkg, dep in data.items():
             deps: list = dep['requires']
             for blk in blacklist_packages:
                 if blk in deps:
                     deps.remove(blk)
                     data[pkg]['requires'] = deps
         return data
-
-    def bar_progress(self) -> None:
-        if self.progress_bar or self.option_for_progress_bar:
-            message: str = 'Database loading'
-            self.bar_process = Process(target=self.progress.progress_bar, args=(message,))
-            self.bar_process.start()
-        else:
-            print('\rDatabase loading... ', end='')
-
-    def done_process(self) -> None:
-        if self.progress_bar or self.option_for_progress_bar:
-            time.sleep(0.1)
-            self.bar_process.terminate()
-            self.bar_process.join()
-            print('\x1b[?25h')
-        else:
-            print(f'{self.bgreen}{self.ascii.done}{self.endc}')
```

### Comparing `slpkg-5.0.6/slpkg/main.py` & `slpkg-5.0.7/slpkg/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 #!/usr/bin/python3
 # -*- coding: utf-8 -*-
 
+
 import sys
 from pathlib import Path
+from signal import signal, SIGPIPE, SIG_DFL
 
 from slpkg.checks import Check
 from slpkg.upgrade import Upgrade
 from slpkg.configs import Configs
 from slpkg.tracking import Tracking
 from slpkg.load_data import LoadData
 from slpkg.repo_info import RepoInfo
@@ -24,22 +26,26 @@
 from slpkg.download_only import DownloadOnly
 from slpkg.sbos.slackbuild import Slackbuilds
 from slpkg.find_installed import FindInstalled
 from slpkg.views.view_package import ViewPackage
 from slpkg.remove_packages import RemovePackages
 from slpkg.update_repositories import UpdateRepositories
 
-from signal import signal, SIGPIPE, SIG_DFL
 signal(SIGPIPE, SIG_DFL)
 
 
-class Menu(Configs):
+class Menu(Configs):  # pylint: disable=[R0902]
+
+    """
+    Control cli options
+    """
+
+    def __init__(self, args: list):  # pylint: disable=[R0915]
+        super(Configs, self).__init__()
 
-    def __init__(self, args: list):
-        super(Configs).__init__()
         self.args: list = args
         self.flags: list = []
         self.directory: str = str(self.tmp_slpkg)
 
         self.utils = Utilities()
         self.usage = Usage()
         self.repos = Repositories()
@@ -294,35 +300,37 @@
         self.check_for_repositories()
         self.load_data = LoadData(self.flags)
 
         self.check = Check(self.repository)
         self.choose = Choose(self.repository)
 
     def check_for_repositories(self) -> None:
-        """ Checks a combination for binaries use repositories only and if repository exists. """
+        """ Checks a combination for binaries use repositories only and if repository exists.
+        """
         except_options: tuple = (
             '-s', 'search',
             '-U', 'upgrade'
         )
         if self.repository == '*' and not self.utils.is_option(except_options, self.args):
             self.usage.help_minimal(f"{self.prog_name}: invalid repository '{self.repository}'")
 
-        elif self.repository not in list(self.repos.repositories.keys()) and self.repository != '*':
+        elif self.repository not in self.repos.repositories and self.repository != '*':
             self.usage.help_minimal(f"{self.prog_name}: invalid repository '{self.repository}'")
 
         if self.repository != '*':
             if not self.repos.repositories[self.repository]['enable']:
                 self.usage.help_minimal(f"{self.prog_name}: repository '{self.repository}' is disabled")
 
     def invalid_options(self) -> None:
-        """ Checks for invalid options. """
+        """ Checks for invalid options.
+        """
         invalid, commands, repeat = [], [], []
 
         for arg in self.args:
-            if arg[0] == '-' and arg in self.commands.keys():
+            if arg[0] == '-' and arg in self.commands:
                 commands.append(arg)
             elif arg[0] == '-' and arg not in self.options:
                 invalid.append(arg)
 
         # Counts the recurring options.
         for opt in self.flags:
             if self.flags.count(opt) > 1:
@@ -357,16 +365,16 @@
             Put the command first and options after.
             Result: ['-i', '-y', '-j', '-R']
         """
         for args in self.args:
             if args[0] == '-' and args[:2] != '--' and len(args) >= 3 and '=' not in args:
                 self.args.remove(args)
 
-                for opt in list(map(lambda x: f'-{x}', [arg for arg in list(args[1:])])):
-                    if opt in self.commands.keys():
+                for opt in map(lambda x: f'-{x}', list(args[1:])):
+                    if opt in self.commands:
                         self.args.insert(0, opt)
                         continue
 
                     self.args.append(opt)
 
     def split_options_from_args(self) -> None:
         """ Split options from arguments.
@@ -394,60 +402,72 @@
 
             try:
                 if arg == self.flag_short_directory:
                     self.directory: str = self.args[self.args.index(arg) + 1]
                     remove_args.append(self.directory)
             except IndexError:
                 self.directory: str = ''
-            
+
             try:
                 if arg == self.flag_short_repository:
                     self.repository: str = self.args[self.args.index(arg) + 1]
                     remove_args.append(self.repository)
             except IndexError:
                 self.repository: str = ''
 
         for arg in remove_args:
             if arg in self.args:
                 self.args.remove(arg)
 
     def move_options(self) -> None:
-        """ Move options to the flags and removes from the arguments. """
+        """ Move options to the flags and removes from the arguments.
+        """
         new_args: list = []
 
         for arg in self.args:
             if arg in self.options:
                 self.flags.append(arg)
             else:
                 new_args.append(arg)
 
         self.args: list = new_args
 
     def is_file_list_packages(self) -> list:
-        """ Checks if the arg is filelist.pkgs. """
+        """ Checks if the arg is filelist.pkgs.
+        """
         if self.args[1].endswith(self.file_list_suffix):
             file = Path(self.args[1])
             packages: list = list(self.utils.read_packages_from_file(file))
         else:
             packages: list = list(set(self.args[1:]))
 
         return packages
 
     def update(self) -> None:
+        """ Update the local repositories.
+
+        Raises:
+            SystemExit: Exit code 0.
+        """
         if len(self.args) == 1:
             if self.utils.is_option((self.flag_check, self.flag_short_check), self.flags):
                 check = CheckUpdates(self.flags, self.repository)
                 check.updates()
             else:
                 update = UpdateRepositories(self.flags, self.repository)
                 update.repositories()
             raise SystemExit(0)
         self.usage.help_short(1)
 
     def upgrade(self) -> None:
+        """ Upgrade the installed packages.
+
+        Raises:
+            SystemExit: Exit code 0.
+        """
         command: str = Menu.upgrade.__name__
         removed: list = []
 
         if len(self.args) == 1:
 
             if self.utils.is_option((self.flag_check, self.flag_short_check), self.flags):
                 self.data: dict = self.load_data.load(self.repository)
@@ -471,81 +491,101 @@
                 packages: list = self.choose.packages(self.data, packages, command)
 
                 if not packages:
                     print('\nEverything is up-to-date!\n')
                     raise SystemExit(0)
 
                 if self.repository not in [self.repos.sbo_repo_name, self.repos.ponce_repo_name]:
-                    install = Packages(
+                    install_bin = Packages(
                         self.repository, self.data, packages, self.flags, mode=command)
-                    install.execute()
+                    install_bin.execute()
                 else:
-                    install = Slackbuilds(
+                    install_sbo = Slackbuilds(
                         self.repository, self.data, packages, self.flags, mode=command)
-                    install.execute()
+                    install_sbo.execute()
             else:
                 self.usage.help_minimal(f"{self.prog_name}: invalid repository '{self.repository}'")
 
             raise SystemExit(0)
         self.usage.help_short(1)
 
     def repo_info(self) -> None:
+        """ Prints repositories information.
+
+        Raises:
+            SystemExit: Exit code 0.
+        """
         if len(self.args) == 1:
             repo = RepoInfo(self.flags, self.repository)
             repo.info()
             raise SystemExit(0)
         self.usage.help_short(1)
 
     def build(self) -> None:
+        """ Builds slackbuilds with dependencies without install.
+
+        Raises:
+            SystemExit: Exit code 0.
+        """
         command: str = Menu.build.__name__
 
         if len(self.args) >= 2:
             self.data: dict = self.load_data.load(self.repository)
             packages: list = self.is_file_list_packages()
             packages: list = self.utils.case_insensitive_pattern_matching(packages, self.data, self.flags)
 
             if self.utils.is_option(self.flag_searches, self.flags):
                 packages: list = self.choose.packages(self.data, packages, command)
 
             self.check.package_exists_in_the_database(packages, self.data)
 
-            if self.repository in list(self.repos.repositories.keys())[:2]:
+            if self.repository in list(self.repos.repositories)[:2]:
                 build = Slackbuilds(
                     self.repository, self.data, packages, self.flags, mode=command
                 )
                 build.execute()
             else:
                 self.usage.help_minimal(f"{self.prog_name}: invalid repository '{self.repository}'")
 
             raise SystemExit(0)
         self.usage.help_short(1)
 
     def install(self) -> None:
+        """ Builds and install packages with dependencies.
+
+        Raises:
+            SystemExit: Exit code 0.
+        """
         command: str = Menu.install.__name__
 
         if len(self.args) >= 2:
             self.data: dict = self.load_data.load(self.repository)
             packages: list = self.is_file_list_packages()
             packages: list = self.utils.case_insensitive_pattern_matching(packages, self.data, self.flags)
 
             if self.utils.is_option(self.flag_searches, self.flags):
                 packages: list = self.choose.packages(self.data, packages, command)
 
             self.check.package_exists_in_the_database(packages, self.data)
 
             if self.repository not in [self.repos.sbo_repo_name, self.repos.ponce_repo_name]:
-                install = Packages(self.repository, self.data, packages, self.flags, mode=command)
-                install.execute()
+                install_bin = Packages(self.repository, self.data, packages, self.flags, mode=command)
+                install_bin.execute()
             else:
-                install = Slackbuilds(self.repository, self.data, packages, self.flags, mode=command)
-                install.execute()
+                install_sbo = Slackbuilds(self.repository, self.data, packages, self.flags, mode=command)
+                install_sbo.execute()
             raise SystemExit(0)
         self.usage.help_short(1)
 
     def download(self) -> None:
+        """ Download only packages.
+
+        Raises:
+            SystemExit: Exit code 0.
+        """
         command: str = Menu.download.__name__
 
         if len(self.args) >= 2:
             self.data: dict = self.load_data.load(self.repository)
             packages: list = self.is_file_list_packages()
             packages: list = self.utils.case_insensitive_pattern_matching(packages, self.data, self.flags)
 
@@ -555,14 +595,19 @@
             self.check.package_exists_in_the_database(packages, self.data)
             down_only = DownloadOnly(self.directory, self.flags, self.data, self.repository)
             down_only.packages(packages)
             raise SystemExit(0)
         self.usage.help_short(1)
 
     def remove(self) -> None:
+        """ Remove packages with dependencies.
+
+        Raises:
+            SystemExit: Exit code 0.
+        """
         command: str = Menu.remove.__name__
 
         if len(self.args) >= 2:
             packages: list = self.is_file_list_packages()
 
             if self.utils.is_option(self.flag_searches, self.flags):
                 packages: list = self.choose.packages(self.data, packages, command)
@@ -571,14 +616,19 @@
 
             remove = RemovePackages(packages, self.flags)
             remove.remove()
             raise SystemExit(0)
         self.usage.help_short(1)
 
     def find(self) -> None:
+        """ Find installed packages.
+
+        Raises:
+            SystemExit: Exit code 0.
+        """
         command: str = Menu.find.__name__
 
         if len(self.args) >= 2:
             packages: list = self.is_file_list_packages()
             self.data: dict = self.load_data.load(self.repository)
             packages: list = self.utils.case_insensitive_pattern_matching(packages, self.data, self.flags)
 
@@ -587,14 +637,19 @@
 
             find = FindInstalled(self.flags, packages)
             find.find()
             raise SystemExit(0)
         self.usage.help_short(1)
 
     def view(self) -> None:
+        """ View package information.
+
+        Raises:
+            SystemExit: Exit code 0.
+        """
         command: str = Menu.view.__name__
 
         if len(self.args) >= 2:
             self.data: dict = self.load_data.load(self.repository)
             packages: list = self.is_file_list_packages()
             packages: list = self.utils.case_insensitive_pattern_matching(packages, self.data, self.flags)
 
@@ -609,14 +664,19 @@
                 view.package(self.data, packages)
             else:
                 view.slackbuild(self.data, packages)
             raise SystemExit(0)
         self.usage.help_short(1)
 
     def search(self) -> None:
+        """ Searching packages to the repositories.
+
+        Raises:
+            SystemExit: Exit code 0.
+        """
         command: str = Menu.search.__name__
         self.data: dict = self.load_data.load(self.repository)
 
         if len(self.args) >= 2:
             packages: list = self.is_file_list_packages()
 
             if self.utils.is_option(self.flag_searches, self.flags):
@@ -624,14 +684,19 @@
 
             pkgs = SearchPackage(self.flags, packages, self.data, self.repository)
             pkgs.search()
             raise SystemExit(0)
         self.usage.help_short(1)
 
     def dependees(self) -> None:
+        """ View packages that depend on other packages.
+
+        Raises:
+            SystemExit: Exit code 0.
+        """
         command: str = Menu.dependees.__name__
 
         if len(self.args) >= 2:
             self.data: dict = self.load_data.load(self.repository)
             packages: list = self.is_file_list_packages()
             packages: list = self.utils.case_insensitive_pattern_matching(packages, self.data, self.flags)
 
@@ -642,14 +707,19 @@
 
             dependees = Dependees(self.data, packages, self.flags)
             dependees.find()
             raise SystemExit(0)
         self.usage.help_short(1)
 
     def tracking(self) -> None:
+        """ Tracking package dependencies.
+
+        Raises:
+            SystemExit: Exit code 0.
+        """
         command: str = Menu.tracking.__name__
 
         if len(self.args) >= 2:
             self.data: dict = self.load_data.load(self.repository)
             packages: list = self.is_file_list_packages()
             packages: list = self.utils.case_insensitive_pattern_matching(packages, self.data, self.flags)
 
@@ -662,48 +732,71 @@
             tracking.package()
             raise SystemExit(0)
         self.usage.help_short(1)
 
 
 class SubMenu:
     """ Submenu that separate from the main menu because of
-    have no options to manage here. """
+    have no options to manage here.
+    """
 
     def __init__(self, args: list):
         self.args: list = args
         self.usage = Usage()
         self.form_configs = FormConfigs()
         self.clean = Cleanings()
 
     def help(self) -> None:
+        """ Prints help menu and exit.
+        """
         if len(self.args) == 1:
             self.usage.help(0)
         self.usage.help_short(1)
 
     def version(self) -> None:
+        """ Print program version and exit.
+
+        Raises:
+            SystemExit: Exit code 0.
+        """
         if len(self.args) == 1:
             version = Version()
             version.view()
             raise SystemExit(0)
         self.usage.help_short(1)
 
     def edit_configs(self) -> None:
+        """ Edit configurations via dialog box.
+
+        Raises:
+            SystemExit: Exit code 0.
+        """
         if len(self.args) == 1:
             self.form_configs.edit()
             raise SystemExit(0)
         self.usage.help_short(1)
 
     def clean_tmp(self) -> None:
+        """ Remove all files and directories from tmp.
+
+        Raises:
+            SystemExit: Exit code 0.
+        """
         if len(self.args) == 1:
             self.clean.tmp()
             raise SystemExit(0)
         self.usage.help_short(1)
 
 
 def main() -> None:
+    """ Call options and commands.
+
+    Raises:
+        SystemExit: Exit code 0.
+    """
     args: list = sys.argv
     args.pop(0)
     usage = Usage()
 
     if len(args) == 0 or '' in args:
         usage.help_short(1)
 
@@ -719,16 +812,16 @@
         '-T': sub_menu.clean_tmp
     }
 
     try:
         arguments_no_options[args[0]]()
     except (KeyError, IndexError):
         pass
-    except KeyboardInterrupt:
-        raise SystemExit(1)
+    except KeyboardInterrupt as e:
+        raise SystemExit(1) from e
 
     menu = Menu(args)
     arguments: dict = {
         'update': menu.update,
         '-u': menu.update,
         'upgrade': menu.upgrade,
         '-U': menu.upgrade,
@@ -754,13 +847,13 @@
         '-t': menu.tracking
     }
 
     try:
         arguments[args[0]]()
     except (KeyError, IndexError):
         usage.help_short(1)
-    except KeyboardInterrupt:
-        raise SystemExit(1)
+    except KeyboardInterrupt as e:
+        raise SystemExit(1) from e
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `slpkg-5.0.6/slpkg/multi_process.py` & `slpkg-5.0.7/slpkg/multi_process.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,30 @@
 #!/usr/bin/python3
 # -*- coding: utf-8 -*-
 
+
 import shutil
 import subprocess
 from datetime import datetime
 from multiprocessing import Process
 
 from slpkg.configs import Configs
 from slpkg.utilities import Utilities
 from slpkg.error_messages import Errors
 from slpkg.views.asciibox import AsciiBox
 from slpkg.progress_bar import ProgressBar
 
 
-class MultiProcess(Configs):
+class MultiProcess(Configs):  # pylint: disable=[R0902]
+
+    """
+    Creates parallel process between progress bar and process.
+    """
 
-    def __init__(self, flags=None):
+    def __init__(self, flags: list = None):
         super(Configs, self).__init__()
 
         self.utils = Utilities()
         self.progress = ProgressBar()
         self.ascii = AsciiBox()
         self.errors = Errors()
 
@@ -40,15 +45,15 @@
         Args:
             command: The command of process
             filename: The filename of process.
             progress_message: The message of progress.
         Returns:
             None.
         """
-        if self.progress_bar or self.option_for_progress_bar:
+        if self.progress_bar_conf or self.option_for_progress_bar:
             skip: str = f'{self.bred}{self.ascii.skipped}{self.endc}'
             done: str = f'{self.bgreen}{self.ascii.done}{self.endc}'
             failed: str = f'{self.bred}{self.ascii.failed}{self.endc}'
             installed: str = ''
 
             if filename.endswith(('.tgz', 'txz')) and not self.option_for_reinstall:
                 installed_package = self.log_packages.glob(filename[:-4])
@@ -78,84 +83,87 @@
                     print(f"\r{'':>2}{self.bgreen}{self.ascii.bullet}{self.endc} {filename} {done}", end='')
 
             # Restore the terminal cursor
             print('\x1b[?25h', self.endc)
         else:
             self._run(command)
 
-    def _run(self, command: str, stdout=subprocess.PIPE, stderr=subprocess.STDOUT) -> None:
+    def _run(self, command: str, stdout: subprocess = subprocess.PIPE, stderr: subprocess = subprocess.STDOUT) -> None:
         """
         Build the package and write a log file.
         Args:
             command: The command of process
             stdout: Captured stdout from the child process.
             stderr: Captured stderr from the child process.
         Returns:
             None.
         """
-        process = subprocess.Popen(command, shell=True, stdout=stdout, stderr=stderr, text=True)
+        with subprocess.Popen(command, shell=True, stdout=stdout, stderr=stderr, text=True) as process:
+
+            self._write_log_head()
 
-        self._write_log_head()
+            # Write the process to the log file and to the terminal.
+            with process.stdout as output:  # type: ignore[union-attr]
+                for line in output:
+                    if not self.progress_bar_conf and not self.option_for_progress_bar:
+                        print(line.strip())  # Print to console
+                    if self.process_log:
+                        with open(self.slpkg_log_file, 'a', encoding='utf-8') as log:
+                            log.write(line)  # Write to log file
+
+            self._write_log_eof()
+
+            process.wait()  # Wait for the process to finish
+
+            # If the process failed, return exit code.
+            if process.returncode != 0:
+                self._error_process()
+                raise SystemExit(process.returncode)
 
-        # Write the process to the log file and to the terminal.
-        with process.stdout as output:
-            for i, line in enumerate(output):
-                if not self.progress_bar and not self.option_for_progress_bar:
-                    print(line.strip())  # Print to console
-                if self.process_log:
-                    with open(self.slpkg_log_file, 'a') as log:
-                        log.write(line)  # Write to log file
-
-        self._write_log_eof()
-
-        process.wait()  # Wait for the process to finish
-
-        # If the process failed, return exit code.
-        if process.returncode != 0:
-            self._error_process()
-            raise SystemExit(process.returncode)
-
-    def _error_process(self):
-        """ Prints error message for a process. """
-        if not self.progress_bar and not self.option_for_progress_bar:
-            message: str = f'Error occurred with process. Please check the log file.'
+    def _error_process(self) -> None:
+        """ Prints error message for a process.
+        """
+        if not self.progress_bar_conf and not self.option_for_progress_bar:
+            message: str = 'Error occurred with process. Please check the log file.'
             print()
             print(len(message) * '=')
             print(f'{self.bred}{message}{self.endc}')
             print(len(message) * '=')
             print()
 
     def _write_log_head(self) -> None:
-        """ Write the timestamp at the head of the log file. """
+        """ Write the timestamp at the head of the log file.
+        """
         if self.process_log:
-            with open(self.slpkg_log_file, 'a') as log:
+            with open(self.slpkg_log_file, 'a', encoding='utf-8') as log:
                 log.write(f"{len(self.head_message) * '='}\n")
                 log.write(f'{self.head_message}\n')
                 log.write(f"{len(self.head_message) * '='}\n")
 
     def _write_log_eof(self) -> None:
-        """ Write the bottom of the log file. """
+        """ Write the bottom of the log file.
+        """
         if self.process_log:
-            with open(self.slpkg_log_file, 'a') as log:
+            with open(self.slpkg_log_file, 'a', encoding='utf-8') as log:
                 log.write(f"\n{len(self.bottom_message) * '='}\n")
                 log.write(f'{self.bottom_message}\n')
                 log.write(f"{len(self.bottom_message) * '='}\n\n")
 
     @staticmethod
-    def process(command: str, stderr=None, stdout=None) -> None:
+    def process(command: str, stderr: subprocess = None, stdout: subprocess = None) -> None:
         """
         Build the package and write a log file.
         Args:
             command: The command of process
             stdout: Captured stdout from the child process.
             stderr: Captured stderr from the child process.
         Returns:
             None.
         """
         try:
-            output = subprocess.run(f'{command}', shell=True, stderr=stderr, stdout=stdout)
-        except KeyboardInterrupt:
-            raise SystemExit(1)
+            output = subprocess.run(f'{command}', shell=True, stderr=stderr, stdout=stdout, check=True)
+        except KeyboardInterrupt as e:
+            raise SystemExit(1) from e
 
         if output.returncode != 0:
             if not command.startswith(('wget', 'wget2', 'curl', 'lftp')):
                 raise SystemExit(output.returncode)
```

### Comparing `slpkg-5.0.6/slpkg/new_configs.py` & `slpkg-5.0.7/slpkg/new_configs.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,19 +1,23 @@
 #!/usr/bin/python3
 # -*- coding: utf-8 -*-
 
+
 import sys
 import shutil
 import difflib
 import subprocess
-from typing import Any
 from pathlib import Path
 
 
-class NewConfigs:
+class NewConfigs:  # pylint: disable=[R0902]
+
+    """
+    Tool that manage the config files.
+    """
 
     def __init__(self, options: list):
         self.options: list = options
         self.etc_path: Path = Path('/etc/slpkg')
         self.slpkg_config: Path = Path(self.etc_path, 'slpkg.toml')
         self.repositories_config: Path = Path(self.etc_path, 'repositories.toml')
         self.blacklist_config: Path = Path(self.etc_path, 'blacklist.toml')
@@ -30,25 +34,28 @@
         self.endc: str = '\x1b[0m'
 
         self.set_no_colors()
 
         self.choice = None
 
     def set_no_colors(self) -> None:
+        """ Switch off colors.
+        """
         if '--no-colors' in self.options:
             self.bold: str = ''
             self.red: str = ''
             self.green: str = ''
             self.bgreen: str = ''
             self.yellow: str = ''
             self.byellow: str = ''
             self.endc: str = ''
 
     def check(self) -> None:
-        """ Checks for .new files. """
+        """ Checks for .new files.
+        """
         print('Checking for NEW configuration files...\n')
         if (self.slpkg_config_new.is_file() or self.blacklist_config_new.is_file()
                 or self.repositories_config_new.is_file()):
             print('There are NEW files:\n')
 
             if self.slpkg_config_new.is_file():
                 print(f"{self.bgreen:>12}{self.slpkg_config_new}{self.endc}")
@@ -70,15 +77,16 @@
 
             self.menu()
 
         else:
             print(f"\n{'No .new files found.':>23}\n")
 
     def menu(self) -> None:
-        """ Menu of choices. """
+        """ Menu of choices.
+        """
         choice: str = input('Choice: ')
 
         choice: str = choice.lower()
 
         arguments: dict = {
             'k': self.keep,
             'o': self.overwrite,
@@ -89,98 +97,111 @@
         try:
             arguments[choice]()
         except KeyError:
             self.keep()
 
     @staticmethod
     def keep() -> None:
+        """ Prints a message.
+        """
         print("\nNo changes were made.\n")
 
     def overwrite(self) -> None:
-        """ Copy tne .new files and rename the olds to .orig.  """
+        """ Copy tne .new files and rename the olds to .orig.
+        """
         if self.slpkg_config_new.is_file():
             self.overwrite_config_file()
 
         if self.repositories_config_new.is_file():
             self.overwrite_repositories_file()
 
         if self.blacklist_config_new.is_file():
             self.overwrite_blacklist_file()
 
         print()  # new line
 
     def overwrite_config_file(self) -> None:
-        """ Copy tne slpkg.toml.new file and rename the old to .orig. """
+        """ Copy the slpkg.toml.new file and rename the old to .orig.
+        """
         if self.slpkg_config.is_file():
             shutil.copy(self.slpkg_config, f"{self.slpkg_config}.orig")
             print(f"\ncp {self.green}{self.slpkg_config}{self.endc} -> {self.slpkg_config}.orig")
 
         shutil.move(self.slpkg_config_new, self.slpkg_config)
         print(f"mv {self.slpkg_config_new} -> {self.green}{self.slpkg_config}{self.endc}")
 
     def overwrite_repositories_file(self) -> None:
-        """ Copy tne repositories.toml.new file and rename the old to .orig. """
+        """ Copy the repositories.toml.new file and rename the old to .orig.
+        """
         if self.slpkg_config.is_file():
             shutil.copy(self.repositories_config, f"{self.repositories_config}.orig")
             print(f"\ncp {self.green}{self.repositories_config}{self.endc} -> {self.repositories_config}.orig")
 
         shutil.move(self.repositories_config_new, self.repositories_config)
         print(f"mv {self.repositories_config_new} -> {self.green}{self.repositories_config}{self.endc}")
 
     def overwrite_blacklist_file(self) -> None:
-        """ Copy tne blacklist.toml.new file and rename the old to .orig. """
+        """ Copy the blacklist.toml.new file and rename the old to .orig.
+        """
         if self.blacklist_config.is_file():
             shutil.copy(self.blacklist_config, f"{self.blacklist_config}.orig")
             print(f"\ncp {self.green}{self.blacklist_config}{self.endc} -> {self.blacklist_config}.orig")
 
         shutil.move(self.blacklist_config_new, self.blacklist_config)
         print(f"mv {self.blacklist_config_new} -> {self.green}{self.blacklist_config}{self.endc}")
 
     def remove(self) -> None:
-        """ Removes the .new files. """
+        """ Removes the .new files.
+        """
         print()  # new line
         self.remove_config_new_file()
         self.remove_repositories_new_file()
         self.remove_blacklist_new_file()
         print()  # new line
 
     def remove_config_new_file(self) -> None:
-        """ Remove slpkg.toml.new file. """
+        """ Remove slpkg.toml.new file.
+        """
         if self.slpkg_config_new.is_file():
             self.slpkg_config_new.unlink()
             print(f"rm {self.red}{self.slpkg_config_new}{self.endc}")
 
     def remove_repositories_new_file(self) -> None:
-        """ Remove repositories.toml.new file. """
+        """ Remove repositories.toml.new file.
+        """
         if self.repositories_config_new.is_file():
             self.repositories_config_new.unlink()
             print(f"rm {self.red}{self.repositories_config_new}{self.endc}")
 
     def remove_blacklist_new_file(self) -> None:
-        """ Remove blacklist.toml.new file. """
+        """ Remove blacklist.toml.new file.
+        """
         if self.blacklist_config_new.is_file():
             self.blacklist_config_new.unlink()
             print(f"rm {self.red}{self.blacklist_config_new}{self.endc}")
 
     def prompt(self) -> None:
-        """ Prompt K, O, R selection for every single file. """
+        """ Prompt K, O, R selection for every single file.
+        """
         print(f"\n{'':>2}({self.byellow}K{self.endc})eep, ({self.byellow}O{self.endc})verwrite, "
               f"({self.byellow}R{self.endc})emove, ({self.byellow}D{self.endc})iff, "
               f"({self.byellow}V{self.endc})imdiff\n")
 
         if self.slpkg_config_new.is_file():
             self.prompt_slpkg_config()
 
         if self.repositories_config_new.is_file():
             self.prompt_repositories_config()
 
         if self.blacklist_config_new.is_file():
             self.prompt_blacklist_config()
 
     def prompt_slpkg_config(self) -> None:
+        """ Prompt for slpkg.toml file.
+        """
         make: str = input(f'{self.bgreen}{self.slpkg_config_new}{self.endc} - '
                           f'({self.byellow}K{self.endc}/{self.byellow}O{self.endc}/'
                           f'{self.byellow}R{self.endc}/{self.byellow}D{self.endc}/'
                           f'{self.byellow}V{self.endc}): ')
 
         if make.lower() == 'k':
             pass
@@ -194,14 +215,16 @@
         if make.lower() == 'd':
             self.diff_files(self.slpkg_config_new, self.slpkg_config)
             self.prompt_slpkg_config()
         if make.lower() == 'v':
             self.vimdiff(self.slpkg_config_new, self.slpkg_config)
 
     def prompt_repositories_config(self) -> None:
+        """ Prompt for repositories.toml file.
+        """
         make: str = input(f'{self.bgreen}{self.repositories_config_new}{self.endc} - '
                           f'({self.byellow}K{self.endc}/{self.byellow}O{self.endc}/'
                           f'{self.byellow}R{self.endc}/{self.byellow}D{self.endc}/'
                           f'{self.byellow}V{self.endc}): ')
 
         if make.lower() == 'k':
             pass
@@ -215,14 +238,16 @@
         if make.lower() == 'd':
             self.diff_files(self.repositories_config_new, self.repositories_config)
             self.prompt_repositories_config()
         if make.lower() == 'v':
             self.vimdiff(self.repositories_config_new, self.repositories_config)
 
     def prompt_blacklist_config(self) -> None:
+        """ Prompt for blacklist.toml file.
+        """
         make: str = input(f'{self.bgreen}{self.blacklist_config_new}{self.endc} - '
                           f'({self.byellow}K{self.endc}/{self.byellow}O{self.endc}/'
                           f'{self.byellow}R{self.endc}/{self.byellow}D{self.endc}/'
                           f'{self.byellow}V{self.endc}): ')
 
         if make.lower() == 'k':
             pass
@@ -236,35 +261,50 @@
         if make.lower() == 'd':
             self.diff_files(self.blacklist_config_new, self.blacklist_config)
             self.prompt_blacklist_config()
         if make.lower() == 'v':
             self.vimdiff(self.blacklist_config_new, self.blacklist_config)
 
     @staticmethod
-    def diff_files(file2: Any, file1: Any) -> None:
-        """ Diff the .new and the current file. """
-        with open(file1, 'r') as f1:
-            with open(file2, 'r') as f2:
+    def diff_files(file2: Path, file1: Path) -> None:
+        """ Diff the .new and the current file.
+        """
+        with open(file1, 'r', encoding='utf-8') as f1:
+            with open(file2, 'r', encoding='utf-8') as f2:
                 diff = difflib.context_diff(
                     f1.readlines(),
                     f2.readlines(),
                     fromfile=str(file1),
                     tofile=str(file2)
                 )
                 for line in diff:
                     print(line, end='')
 
     @staticmethod
-    def vimdiff(file1: Any, file2: Any) -> None:
+    def vimdiff(file1: Path, file2: Path) -> None:
+        """ Show vimdiff command.
+
+        Args:
+            file1 (Any): First file.
+            file2 (Any): Second file.
+
+        Raises:
+            SystemExit: Raise exit code.
+        """
         output = subprocess.call(f'vimdiff {file1} {file2}', shell=True)
         if output != 0:
             raise SystemExit(output)
 
 
 def main() -> None:
+    """ Manage arguments.
+
+    Raises:
+        SystemExit: Description
+    """
     args: list = sys.argv
     args.pop(0)
 
     options: list = [
         '--no-colors',
         '-h',
         '--help'
@@ -284,9 +324,9 @@
     elif len(args) > 1:
         print('\ntry: slpkg_new-configs --help\n')
         sys.exit(1)
 
     try:
         config = NewConfigs(args)
         config.check()
-    except KeyboardInterrupt:
-        raise SystemExit(1)
+    except KeyboardInterrupt as e:
+        raise SystemExit(1) from e
```

### Comparing `slpkg-5.0.6/slpkg/progress_bar.py` & `slpkg-5.0.7/slpkg/progress_bar.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,77 +1,100 @@
 #!/usr/bin/python3
 # -*- coding: utf-8 -*-
 
+
 import time
 
 from slpkg.configs import Configs
 from slpkg.views.asciibox import AsciiBox
 
 
 class ProgressBar(Configs):
 
+    """
+    Progress bar that show spinner instead of the
+    of the file progress.
+    """
+
     def __init__(self):
         super(Configs, self).__init__()
         self.ascii = AsciiBox()
 
         self.color: str = self.endc
         self.spinners: dict = {}
         self.spinners_color: dict = {}
         self.spinner: str = ''
         self.bar_message: str = ''
 
-    def progress_bar(self, message: str, filename=None) -> None:
+    def progress_bar(self, message: str, filename: str = None) -> None:
         """ Creating progress bar. """
+        self.assign_spinner_chars()
         self.set_spinner()
         self.assign_spinner_colors()
         self.set_color()
         self.set_the_spinner_message(filename, message)
         print('\x1b[?25l', end='')  # Hide cursor before starting
 
         current_state = 0  # Index of the current state
         try:
             while True:
                 print(f"\r{self.bar_message}{self.color}{self.spinner[current_state]}{self.endc}", end="")
                 time.sleep(0.1)
                 current_state = (current_state + 1) % len(self.spinner)
-        except KeyboardInterrupt:
+        except KeyboardInterrupt as e:
             print('\x1b[?25h', end='')
-            raise SystemExit(1)
+            raise SystemExit(1) from e
 
     def assign_spinner_colors(self) -> None:
+        """ Assign spinner colors.
+        """
         self.spinners_color: dict = {
             'green': self.green,
             'violet': self.violet,
             'yellow': self.yellow,
             'blue': self.blue,
             'cyan': self.cyan,
             'grey': self.grey,
             'red': self.red,
             'white': self.endc
         }
 
-    def set_the_spinner_message(self, filename: str, message: str) -> None:
-        self.bar_message: str = f'{message}... '
-        if filename:
-            self.bar_message: str = (f"{'':>2}{self.yellow}{self.ascii.bullet}{self.endc} {filename}: "
-                                     f"{message}... ")
-
-    def set_spinner(self) -> None:
+    def assign_spinner_chars(self) -> None:
+        """ Assign for characters.
+        """
         self.spinners: dict = {
             'spinner': ('-', '\\', '|', '/'),
             'pie': ('◷', '◶', '◵', '◴'),
             'moon': ('◑', '◒', '◐', '◓'),
             'line': ('⎺', '⎻', '⎼', '⎽', '⎼', '⎻'),
             'pixel': ('⣾', '⣷', '⣯', '⣟', '⡿', '⢿', '⣻', '⣽'),
             'ball': ('_', '.', '|', 'o'),
             'clock': ('🕛', '🕑', '🕒', '🕔', '🕧', '🕗', '🕘', '🕚')
         }
+
+    def set_the_spinner_message(self, filename: str, message: str) -> None:
+        """ Set message to the spinner.
+
+        Args:
+            filename (str): Name of file.
+            message (str): The progress bar message.
+        """
+        self.bar_message: str = f'{message}... '
+        if filename:
+            self.bar_message: str = (f"{'':>2}{self.yellow}{self.ascii.bullet}{self.endc} {filename}: "
+                                     f"{message}... ")
+
+    def set_spinner(self) -> None:
+        """ Spinners characters.
+        """
         try:
             self.spinner: tuple = self.spinners[self.progress_spinner]
         except KeyError:
             self.spinner: tuple = self.spinners['spinner']
 
     def set_color(self) -> None:
+        """ Setting the spinner color.
+        """
         try:
             self.color: str = self.spinners_color[self.spinner_color]
         except KeyError:
             self.color: str = self.endc
```

### Comparing `slpkg-5.0.6/slpkg/remove_packages.py` & `slpkg-5.0.7/slpkg/remove_packages.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,24 +1,29 @@
 #!/usr/bin/python3
 # -*- coding: utf-8 -*-
 
+
+from __future__ import annotations
+
 import os
 import time
 import json
 
 from slpkg.configs import Configs
+from slpkg.views.views import View
 from slpkg.utilities import Utilities
 from slpkg.dialog_box import DialogBox
-from slpkg.views.views import View
 from slpkg.multi_process import MultiProcess
 
 
-class RemovePackages(Configs):
-    """ Removes installed packages with dependencies if they installed with
-        slpkg install command.
+class RemovePackages(Configs):  # pylint: disable=[R0902]
+
+    """
+    Removes installed packages with dependencies if they installed with
+    slpkg install command.
     """
 
     def __init__(self, packages: list, flags: list):
         super(Configs, self).__init__()
         self.packages: list = packages
 
         self.dialogbox = DialogBox()
@@ -30,94 +35,125 @@
         self.packages_for_remove: list = []
         self.dependencies: list = []
         self.found_dependent_packages: dict = {}
 
         self.option_for_yes: bool = self.utils.is_option(
             ('-y', '--yes'), flags)
 
-    def remove(self, upgrade=False) -> None:
-        self.deps_log: dict = self.utils.read_json_file(self.deps_log_file)
+        self.option_for_resolve_off: bool = self.utils.is_option(
+            ('-O', '--resolve-off'), flags)
+
+    def remove(self, upgrade: bool = False) -> None:
+        """ Remove packages
+
+        Args:
+            upgrade (bool, optional): Is packages comes from upgrade method.
+        """
+        if not self.option_for_resolve_off:
+            self.deps_log: dict = self.utils.read_json_file(self.deps_log_file)
 
         if upgrade:
             self.packages: list = self.choose_packages_for_remove(self.packages, upgrade)
 
         if self.packages:
             self.add_packages_for_remove()
             self.remove_doubles_dependencies()
             self.dependencies: list = self.choose_packages_for_remove(self.dependencies)
             self.add_installed_dependencies_to_remove()
 
             self.view.remove_packages(self.packages, self.dependencies)
-            self.found_dependent()
+            self.find_dependent()
 
             answer: str = 'y'
             if upgrade:
                 answer: str = self.remove_question()
             else:
                 self.view.question()
 
             if answer in ['y', 'Y']:
                 start: float = time.time()
                 self.remove_packages()
                 elapsed_time: float = time.time() - start
                 self.utils.finished_time(elapsed_time)
 
     def add_packages_for_remove(self) -> None:
+        """ Add packages for remove.
+        """
         for package in self.packages:
             installed: str = self.utils.is_package_installed(package)
             if installed:
                 self.packages_for_remove.append(installed)
 
             if self.deps_log.get(package):
                 dependencies: list = self.deps_log[package]
                 for dep in dependencies:
                     if self.utils.is_package_installed(dep) and dep not in self.packages:
                         self.dependencies.append(dep)
 
-    def found_dependent(self) -> None:
+    def find_dependent(self) -> None:
+        """ Find packages that depend on other packages.
+        """
         for package in self.packages_for_remove:
             name: str = self.utils.split_package(package)['name']
-            version: str = self.utils.split_package(package)['version']
             for pkg, deps in self.deps_log.items():
                 if name in deps and pkg not in self.packages + self.dependencies:
+                    version: str = ''
+                    installed: str = self.utils.is_package_installed(pkg)
+                    if installed:
+                        version: str = self.utils.split_package(installed)['version']
                     self.found_dependent_packages[pkg] = version
 
         if self.found_dependent_packages:
             dependent_packages: list = list(set(self.found_dependent_packages))
             print(f'\n{self.bred}Warning: {self.endc}found extra ({len(dependent_packages)}) dependent packages:')
             for pkg, ver in self.found_dependent_packages.items():
                 print(f"{'':>2}{pkg} {self.grey}{ver}{self.endc}")
 
     def remove_doubles_dependencies(self) -> None:
+        """ Removes doubles packages.
+        """
         self.dependencies: list = list(set(self.dependencies))
 
     def add_installed_dependencies_to_remove(self) -> None:
+        """ Adds dependencies for remove.
+        """
         for dep in self.dependencies:
             installed: str = self.utils.is_package_installed(dep)
             if installed:
                 self.packages_for_remove.append(installed)
 
     def remove_packages(self) -> None:
+        """ Remove packages.
+        """
         # Remove old slpkg.log file.
         if self.slpkg_log_file.is_file():
             self.slpkg_log_file.unlink()
 
         print(f'Started of removing total ({self.cyan}{len(self.packages_for_remove)}{self.endc}) packages:\n')
         for package in self.packages_for_remove:
             command: str = f'{self.removepkg} {package}'
             progress_message: str = f'{self.bold}{self.red}Removing{self.endc}'
 
             self.multi_proc.process_and_log(command, package, progress_message)
             name: str = self.utils.split_package(package)['name']
             if name in self.deps_log.keys():
                 self.deps_log.pop(name)
 
-        self.deps_log_file.write_text(json.dumps(self.deps_log, indent=4))
+        self.deps_log_file.write_text(json.dumps(self.deps_log, indent=4), encoding='utf-8')
 
-    def choose_packages_for_remove(self, packages: list, upgrade=False) -> list:
+    def choose_packages_for_remove(self, packages: list, upgrade: bool = False) -> list:
+        """ Choose packages via dialog utility.
+
+        Args:
+            packages (list): Description
+            upgrade (bool, optional): Description
+
+        Returns:
+            list: List of package names.
+        """
         if packages and self.dialog:
             height: int = 10
             width: int = 70
             list_height: int = 0
             choices: list = []
             title: str = " Choose dependencies you want to remove "
             if upgrade:
@@ -127,16 +163,22 @@
                 installed_package: str = self.utils.is_package_installed(package)
                 installed_version: str = self.utils.split_package(installed_package)['version']
                 choices.extend([(package, installed_version, True, f'Package: {installed_package}')])
 
             text: str = f'There are {len(choices)} dependencies:'
             if upgrade:
                 text: str = f'There are {len(choices)} packages:'
-            code, packages = self.dialogbox.checklist(text, title, height, width, list_height, choices)
+            code, packages = self.dialogbox.checklist(text, title, height, width, list_height, choices)  # pylint: disable=[W0612]
             os.system('clear')
             return packages
         return packages
 
-    def remove_question(self) -> str:
+    def remove_question(self) -> str | None:
+        """ Question about remove packages.
+
+        Returns:
+            str | None: Answer.
+        """
         if not self.option_for_yes and self.ask_question:
             answer: str = input('\nDo you want to remove these packages? [y/N] ')
             return answer
+        return None
```

### Comparing `slpkg-5.0.6/slpkg/repo_info.py` & `slpkg-5.0.7/slpkg/repo_info.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,125 +1,159 @@
 #!/usr/bin/python3
 # -*- coding: utf-8 -*-
 
+
 import shutil
 from pathlib import Path
 
 from slpkg.configs import Configs
 from slpkg.load_data import LoadData
 from slpkg.utilities import Utilities
 from slpkg.repositories import Repositories
 
 
-class RepoInfo(Configs):
+class RepoInfo(Configs):  # pylint: disable=[R0902]
+
+    """
+    View information about repositories.
+    """
 
     def __init__(self, flags: list, repository: str):
         super(Configs, self).__init__()
         self.flags: list = flags
         self.repository: str = repository
 
         self.load_data = LoadData(flags)
         self.utils = Utilities()
         self.repos = Repositories()
         self.columns, self.rows = shutil.get_terminal_size()
         self.name_alignment: int = self.columns - 61
 
-        if self.name_alignment < 1:
-            self.name_alignment: int = 1
+        self.name_alignment = max(self.name_alignment, 1)
 
         self.enabled: int = 0
         self.total_packages: int = 0
         self.repo_data: dict = {}
         self.dates: dict = {}
 
         self.option_for_repository: bool = self.utils.is_option(
             ('-o', '--repository'), flags)
 
-    def repo_information(self) -> dict:
-        repo_info_json: Path = Path(f'{self.repos.repositories_path}', self.repos.repos_information)
-        if repo_info_json.is_file():
-            repo_info_json: Path = Path(f'{self.repos.repositories_path}', self.repos.repos_information)
-            return self.utils.read_json_file(repo_info_json)
-        return {}
-
     def info(self) -> None:
-        """ Prints information about repositories. """
-        self.dates: dict = self.repo_information()
-        if self.option_for_repository:
-            self.repo_data: dict = self.load_data.load(self.repository)
-        else:
-            self.repo_data: dict = self.load_data.load('*')
+        """ Prints information about repositories.
+        """
+        self.load_repo_data()
+
         self.view_the_title()
 
         if self.option_for_repository:
             self.view_the_repository_information()
         else:
             self.view_the_repositories_information()
 
-    def count_the_packages(self, repository: str) -> int:
+    def load_repo_data(self) -> None:
+        """ Loads repository data.
+        """
+        self.dates: dict = self.repo_information()
         if self.option_for_repository:
-            count: int = len(self.repo_data.keys())
+            self.repo_data: dict = self.load_data.load(self.repository)
         else:
-            count: int = len(self.repo_data[repository].keys())
-        self.total_packages += count
-        return count
+            self.repo_data: dict = self.load_data.load('*')
+
+    def repo_information(self) -> dict:
+        """ Loads repository information.
+
+        Returns:
+            dict: Description
+        """
+        repo_info_json: Path = Path(f'{self.repos.repositories_path}', self.repos.repos_information)
+        if repo_info_json.is_file():
+            repo_info_json: Path = Path(f'{self.repos.repositories_path}', self.repos.repos_information)
+            return self.utils.read_json_file(repo_info_json)
+        return {}
 
     def view_the_title(self) -> None:
-        title: str = f'repositories information:'.title()
+        """ Prints the title.
+        """
+        title: str = 'repositories information:'.title()
         if self.option_for_repository:
-            title: str = f'repository information:'.title()
+            title: str = 'repository information:'.title()
         print(f'\n{title}')
         print('=' * (self.columns - 1))
         print(f"{'Name:':<{self.name_alignment}}{'Status:':<14}{'Last Updated:':<34}{'Packages:':>12}")
         print('=' * (self.columns - 1))
 
     def view_the_repository_information(self) -> None:
-        date: str = 'None'
-        count: int = 0
-        color: str = self.red
-        status: str = 'Disabled'
+        """ Prints the repository information.
+        # """
+        args: dict = {
+            'repo': self.repository,
+            'date': 'None',
+            'count': 0,
+            'color': self.red,
+            'status': 'Disable'
+        }
+
         if self.dates.get(self.repository):
-            date: str = self.dates[self.repository].get('last_updated', 'None')
+            args['date']: str = self.dates[self.repository].get('last_updated', 'None')
 
         if self.repos.repositories[self.repository]['enable']:
-            status: str = 'Enabled'
-            color: str = self.green
-            count: int = self.count_the_packages(self.repository)
+            self.enabled += 1
+            args['status'] = 'Enabled'
+            args['color'] = self.green
+            args['count'] = len(self.repo_data)
 
-        self.view_the_line_information(self.repository, status, date, count, color)
-        self.view_summary_of_repository()
+        self.view_the_line_information(args)
+        self.view_summary_of_all_repositories()
 
     def view_the_repositories_information(self) -> None:
-        for repo, item in self.repos.repositories.items():
-            date: str = 'None'
-            count: int = 0
-            color: str = self.red
-            status: str = 'Disabled'
+        """ Prints the repositories information.
+        """
+        args: dict = {}
+        for repo, conf in self.repos.repositories.items():
+            args: dict = {
+                'repo': repo,
+                'date': 'None',
+                'count': 0,
+                'color': self.red,
+                'status': 'Disable'
+            }
+
             if self.dates.get(repo):
-                date: str = self.dates[repo].get('last_updated', 'None')
-    
-            if item['enable']:
+                args['date']: str = self.dates[repo].get('last_updated', 'None')
+
+            if conf['enable']:
                 self.enabled += 1
-                status: str = 'Enabled'
-                color: str = self.green
-                count: int = self.count_the_packages(repo)
+                args['status'] = 'Enabled'
+                args['color'] = self.green
+                args['count'] = len(self.repo_data[repo])
 
-            self.view_the_line_information(repo, status, date, count, color)
+            self.view_the_line_information(args)
         self.view_summary_of_all_repositories()
 
-    def view_the_line_information(self, repository: str, status: str, date: str, count: int, color: str) -> None:
+    def view_the_line_information(self, args: dict) -> None:
+        """Prints the row of information.
+
+        Args:
+            args (dict): Arguments for print.
+        """
+        repository: str = args['repo']
         repo_color: str = self.cyan
-        if repository == self.repos.default_repository:
+        if args['repo'] == self.repos.default_repository:
             repo_color: str = self.byellow
-            repository: str = f'{repository} (default)'
+            repository: str = f"{args['repo']} (default)"
 
-        print(f"{repo_color}{repository:<{self.name_alignment}}{self.endc}{color}{status:<14}{self.endc}{date:<34}"
-              f"{self.yellow}{count:>12}{self.endc}")
+        print(f"{repo_color}{repository:<{self.name_alignment}}{self.endc}{args['color']}{args['status']:<14}"
+              f"{self.endc}{args['date']:<34}{self.yellow}{args['count']:>12}{self.endc}")
 
     def view_summary_of_repository(self) -> None:
+        """ Prints the repository summary.
+        """
         print('=' * (self.columns - 1))
         print(f"{self.grey}Total {self.total_packages} packages available from the '{self.repository}' repository.\n")
 
     def view_summary_of_all_repositories(self) -> None:
+        """ Prints the total summary of repositories.
+        """
         print('=' * (self.columns - 1))
         print(f"{self.grey}Total of {self.enabled}/{len(self.repos.repositories)} "
               f"repositories are enabled with {self.total_packages} packages available.\n")
```

### Comparing `slpkg-5.0.6/slpkg/repositories.py` & `slpkg-5.0.7/slpkg/repositories.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,32 +4,38 @@
 
 try:
     import tomli
 except ModuleNotFoundError:
     import tomllib as tomli
 
 from pathlib import Path
+from typing import ClassVar
 from dataclasses import dataclass
 
 from slpkg.configs import Configs
 from slpkg.utilities import Utilities
 from slpkg.toml_errors import TomlErrors
 
 
 @dataclass
-class Repositories:
+class Repositories:  # pylint: disable=[R0902]
+
+    """
+    Repositories configurations.
+    """
+
     toml_errors = TomlErrors()
     utils = Utilities()
 
     repositories_toml_file: Path = Path(Configs.etc_path, 'repositories.toml')
     repositories_path: Path = Path(Configs.lib_path, 'repos')
 
     repos_config = {}
     repositories = {}
-    repos_toml = {}
+    repos_toml = {}  # type: ignore[var-annotated]
 
     data_json: str = 'data.json'
     repos_information: Path = Path(repositories_path, 'repos_information.json')
     default_repository: str = 'sbo'
 
     slackbuilds_txt: str = 'SLACKBUILDS.TXT'
     packages_txt: str = 'PACKAGES.TXT'
@@ -235,15 +241,15 @@
 
             pprkut_repo: bool = repos_config['pprkut']['enable']
             pprkut_repo_mirror: str = repos_config['pprkut']['mirror']
     except (tomli.TOMLDecodeError, KeyError) as error:
         toml_errors.raise_toml_error_message(error, repositories_toml_file)
 
     # Dictionary configurations of repositories.
-    repositories = {
+    repositories: ClassVar[list[str]] = {
         sbo_repo_name: {
             'enable': sbo_repo,
             'path': sbo_repo_path,
             'mirror_packages': sbo_repo_mirror,
             'mirror_changelog': sbo_repo_mirror,
             'slackbuilds_txt': slackbuilds_txt,
             'changelog_txt': changelog_txt,
@@ -444,16 +450,16 @@
                 mirror_packages: str = data.get('mirror', '')
                 mirror_changelog: str = mirror_packages
                 if data.get('changelog'):
                     mirror_changelog: str = data.get('changelog', '')
 
                 values = {
                     'enable': data.get('enable', False),
-                    'path': Path(repositories_path, repo),
+                    'path': Path(repositories_path, str(repo)),
                     'mirror_packages': mirror_packages,
                     'mirror_changelog': mirror_changelog,
                     'packages_txt': packages_txt,
                     'checksums_md5': checksums_md5,
                     'changelog_txt': changelog_txt,
                     'repo_tag': data.get('tag', '')
                 }
-                repositories[repo] = values
+                repositories[str(repo)] = values
```

### Comparing `slpkg-5.0.6/slpkg/sbos/sbo_generate.py` & `slpkg-5.0.7/slpkg/sbos/sbo_generate.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,23 +1,33 @@
 #!/usr/bin/python3
 # -*- coding: utf-8 -*-
 
+
 from pathlib import Path
 from slpkg.configs import Configs
 from slpkg.views.asciibox import AsciiBox
 
 
 class SBoGenerate(Configs):
-    """ Generating the SLACKBUILDS.TXT file. """
+
+    """
+    Generating the SLACKBUILDS.TXT file.
+    """
 
     def __init__(self):
         super(Configs, self).__init__()
         self.ascii = AsciiBox()
 
-    def slackbuild_file(self, repo_path: Path, repo_slackbuild_txt: str) -> None:
+    def slackbuild_file(self, repo_path: Path, repo_slackbuild_txt: str) -> None:  # pylint: disable=[R0914]
+        """ Creates a SLACKBUILDS.TXT file.
+
+        Args:
+            repo_path (Path): Path to file.
+            repo_slackbuild_txt (str): Name of file to create.
+        """
         print(f'Generating the {repo_slackbuild_txt} file... ', end='', flush=True)
 
         # slackbuild.info variables
         info_var: dict = {
             1: 'PRGNAM=',
             2: 'VERSION=',
             3: 'HOMEPAGE=',
@@ -26,15 +36,15 @@
             6: 'DOWNLOAD_x86_64=',
             7: 'MD5SUM_x86_64=',
             8: 'REQUIRES=',
             9: 'MAINTAINER=',
             10: 'EMAIL='
         }
 
-        with open(Path(repo_path, repo_slackbuild_txt), 'w') as sbo:
+        with open(Path(repo_path, repo_slackbuild_txt), 'w', encoding='utf-8') as sbo:
             for path in repo_path.glob('**/*'):
                 if path.name.endswith('.info'):
                     sbo_path = Path('/'.join(str(path).split('/')[:-1]))
 
                     name: str = str(path).split('/')[-2]
                     location: str = str(Path('/'.join(str(path).split('/')[-3:-1])))
                     files: str = ' '.join([file.name for file in list(sbo_path.iterdir())])
@@ -55,16 +65,16 @@
                         ' '.join([var.replace('\\', '').strip() for var in self.read_info_file(
                             path, info_var[5], info_var[6])])[len(info_var[5]):].replace('"', ''))
 
                     md5sum_x86_64: str = (
                         ' '.join([var.replace('\\', '').strip() for var in self.read_info_file(
                             path, info_var[7], info_var[8])])[len(info_var[7]):].replace('"', ''))
 
-                    requires: str = (' '.join([var for var in self.read_info_file(
-                        path, info_var[8], info_var[9])])[len(info_var[8]):].replace('"', ''))
+                    requires: str = (' '.join(list(self.read_info_file(
+                        path, info_var[8], info_var[9])))[len(info_var[8]):].replace('"', ''))
 
                     short_description: str = self.read_short_description(sbo_path, name)
 
                     sbo.write(f'SLACKBUILD NAME: {name}\n')
                     sbo.write(f'SLACKBUILD LOCATION: ./{location}\n')
                     sbo.write(f'SLACKBUILD FILES: {files}\n')
                     sbo.write(f'SLACKBUILD VERSION: {version}\n')
@@ -76,31 +86,48 @@
                     sbo.write(f'SLACKBUILD SHORT DESCRIPTION: {short_description}\n')
                     sbo.write('\n')
 
         print(f'{self.bgreen}{self.ascii.done}{self.endc}\n')
 
     @staticmethod
     def read_short_description(path: Path, name: str) -> str:
-        """ Returns the short description. """
+        """ Returns the short description.
+
+        Args:
+            path (Path): Path to file.
+            name (str): Slackbuild name.
+
+        Returns:
+            str: Description
+        """
         slack_desc: Path = Path(path, 'slack-desc')
         if slack_desc.is_file():
-            with open(slack_desc, 'r') as f:
+            with open(slack_desc, 'r', encoding='utf-8') as f:
                 slack = f.readlines()
 
             for line in slack:
                 pattern: str = f'{name}: {name}'
                 if line.startswith(pattern):
                     return line[len(name) + 1:].strip()
         return ''
 
     @staticmethod
     def read_info_file(info_file: Path, start: str, stop: str) -> list:
-        """ Reads the .info file and return the line between to variables. """
+        """Reads the .info file and return the line between to variables.
+
+        Args:
+            info_file (Path): Slackbuild file name.
+            start (str): Variable name to start.
+            stop (str): Variable name to stop.
+
+        Returns:
+            list: Results in list.
+        """
         begin = end = 0
-        with open(info_file, 'r') as f:
+        with open(info_file, 'r', encoding='utf-8') as f:
             info = f.read().splitlines()
 
         for index, line in enumerate(info):
             if line.startswith(start):
                 begin = index
             if line.startswith(stop):
                 end = index
```

### Comparing `slpkg-5.0.6/slpkg/search.py` & `slpkg-5.0.7/slpkg/search.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,17 +1,21 @@
 #!/usr/bin/python3
 # -*- coding: utf-8 -*-
 
+
 from slpkg.configs import Configs
 from slpkg.utilities import Utilities
 from slpkg.repositories import Repositories
 
 
-class SearchPackage(Configs):
-    """ Search packages from the repositories. """
+class SearchPackage(Configs):  # pylint: disable=[R0902]
+
+    """
+    Search packages from the repositories.
+    """
 
     def __init__(self, flags: list, packages: list, data: dict, repository: str):
         super(Configs, self).__init__()
         self.packages: list = packages
         self.data: dict = data
         self.repository: str = repository
 
@@ -25,43 +29,54 @@
         self.option_for_no_case: bool = self.utils.is_option(
             ('-m', '--no-case'), flags)
 
         self.option_for_pkg_version: bool = self.utils.is_option(
             ('-p', '--pkg-version'), flags)
 
     def search(self) -> None:
+        """ Choose between all and one repository.
+        """
         if self.repository == '*':
             self.search_to_all_repositories()
         else:
             self.repo_data: dict = self.data
             self.search_for_the_packages(self.repository)
 
-        print(f'The list below shows the repository packages:\n')
+        print('The list below shows the repository packages:\n')
         self.summary_of_searching()
 
     def search_to_all_repositories(self) -> None:
+        """ Search package name to all enabled repositories.
+        """
         all_data: dict = self.data
         for name, repo in all_data.items():
             self.repo_data: dict = repo
             self.search_for_the_packages(name)
 
     def search_for_the_packages(self, repo: str) -> None:
+        """ Search for packages and save in a dictionary.
+
+        Args:
+            repo (str): repository name.
+        """
         for package in self.packages:
-            for name, data_pkg in self.repo_data.items():
+            for name, data_pkg in sorted(self.repo_data.items()):
 
                 if package in name or package == '*' or self.is_not_case_sensitive(package, name):
                     self.matching += 1
 
                     self.data_dict[self.matching] = {
                         'repository': repo,
                         'name': name,
                         'version': data_pkg['version']
                     }
 
     def summary_of_searching(self) -> None:
+        """ Prints the result.
+        """
         try:
             repo_length: int = max(len(repo['repository']) for repo in self.data_dict.values())
         except ValueError:
             repo_length: int = 1
 
         try:
             name_length: int = max(len(name['name']) for name in self.data_dict.values())
@@ -81,9 +96,19 @@
                       f"{self.yellow}{version}{self.endc}")
 
             print(f'\n{self.grey}Total found {self.matching} packages.{self.endc}')
         else:
             print('\nDoes not match any package.\n')
 
     def is_not_case_sensitive(self, package: str, name: str) -> bool:
+        """ Check for case sensitive.
+
+        Args:
+            package (str): Package file.
+            name (str): Package name.
+
+        Returns:
+            bool: True or False.
+        """
         if self.option_for_no_case:
             return package.lower() in name.lower()
+        return False
```

### Comparing `slpkg-5.0.6/slpkg/tracking.py` & `slpkg-5.0.7/slpkg/tracking.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,20 +1,24 @@
 #!/usr/bin/python3
 # -*- coding: utf-8 -*-
 
+
 from slpkg.configs import Configs
 from slpkg.utilities import Utilities
 from slpkg.views.asciibox import AsciiBox
-from slpkg.sbos.dependencies import Requires
-from slpkg.binaries.required import Required
 from slpkg.repositories import Repositories
+from slpkg.sbos.dependencies import resolve_requires
+from slpkg.binaries.required import Required
 
 
-class Tracking(Configs):
-    """ Tracking of the package dependencies. """
+class Tracking(Configs):  # pylint: disable=[R0902]
+
+    """
+    Tracking of the package dependencies.
+    """
 
     def __init__(self, data: dict, packages: list, flags: list, repository: str):
         super(Configs, self).__init__()
         self.data: dict = data
         self.packages: list = packages
         self.flags: list = flags
         self.repository: str = repository
@@ -33,14 +37,16 @@
         self.count_requires: int = 0
         self.require_length: int = 0
 
         self.option_for_pkg_version: bool = self.utils.is_option(
             ('-p', '--pkg-version'), flags)
 
     def package(self) -> None:
+        """ Call methods and prints the results.
+        """
         self.view_the_title()
 
         for package in self.packages:
             self.count_requires: int = 0
 
             self.set_the_package_line(package)
             self.set_package_requires(package)
@@ -52,58 +58,95 @@
 
                 self.set_the_package_require_line(require)
                 self.view_requires()
 
             self.view_summary_of_tracking(package)
 
     def view_the_title(self) -> None:
-        print(f"The list below shows the packages with dependencies:\n")
-        self.packages: tuple = tuple(self.utils.apply_package_pattern(self.data, self.packages))
+        """ Prints the title.
+        """
+        print("The list below shows the packages with dependencies:\n")
+        self.packages: list = self.utils.apply_package_pattern(self.data, self.packages)
 
     def view_the_main_package(self) -> None:
+        """ Prints the main package.
+        """
         print(self.package_line)
         print(f"{'':>1}{self.llc}{self.hl}", end='')
 
     def view_requires(self) -> None:
+        """ Prints the requires.
+        """
         if self.count_requires == 1:
             print(f"{'':>1}{self.require_line}")
         else:
             print(f"{'':>4}{self.require_line}")
 
     def view_no_dependencies(self) -> None:
+        """ Prints the message 'No dependencies'.
+        """
         if not self.package_requires:
             print(f"{'':>1}{self.cyan}No dependencies{self.endc}")
 
     def set_the_package_line(self, package: str) -> None:
+        """ Sets for package line.
+
+        Args:
+            package (str): Package name.
+        """
         self.package_line: str = f'{self.yellow}{package}{self.endc}'
         if self.option_for_pkg_version:
             self.set_package_version(package)
             self.package_line: str = f'{self.yellow}{package} {self.package_version}{self.endc}'
 
     def set_the_package_require_line(self, require: str) -> None:
+        """ Sets the requires.
+
+        Args:
+            require (str): Require name.
+        """
         self.require_line: str = f'{self.cyan}{require}{self.endc}'
         if self.option_for_pkg_version:
             self.set_package_dependency_version(require)
             self.require_line: str = (f'{self.cyan}{require:<{self.require_length}}{self.endc}'
                                       f'{self.package_dependency_version}')
 
     def set_package_dependency_version(self, require: str) -> None:
-        try:
-            self.package_dependency_version: str = f"{'':>1}(not included)"
-            if self.data.get(require):
-                self.package_dependency_version: str = f"{'':>1}{self.yellow}{self.data[require]['version']}{self.endc}"
-        except KeyError:  # KeyError here because of the '%README%' as dependency
-            self.package_dependency_version: str = ''
+        """ Sets the dependency version.
+
+        Args:
+            require (str): Description
+        """
+        self.package_dependency_version: str = f"{'':>1}(not included)"
+        if self.data.get(require):
+            self.package_dependency_version: str = (
+                f"{'':>1}{self.yellow}{self.data[require]['version']}{self.endc}"
+            )
 
     def set_package_version(self, package: str) -> None:
+        """ Sets the main package version.
+
+        Args:
+            package (str): Package name.
+        """
         self.package_version: str = self.data[package]['version']
 
     def set_package_requires(self, package: str) -> None:
+        """ Sets for the package require.
+
+        Args:
+            package (str): Package name.
+        """
         if self.repository not in [self.repos.sbo_repo_name, self.repos.ponce_repo_name]:
             self.package_requires: tuple = Required(self.data, package, self.flags).resolve()
         else:
-            self.package_requires: tuple = Requires(self.data, package, self.flags).resolve()
+            self.package_requires: tuple = resolve_requires(self.data, package, self.flags)
         if self.package_requires:
             self.require_length: int = max(len(name) for name in self.package_requires)
 
     def view_summary_of_tracking(self, package: str) -> None:
+        """ Prints the summary.
+
+        Args:
+            package (str): Package name.
+        """
         print(f'\n{self.grey}{self.count_requires} dependencies for {package}{self.endc}\n')
```

### Comparing `slpkg-5.0.6/slpkg/upgrade.py` & `slpkg-5.0.7/slpkg/upgrade.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,28 @@
 #!/usr/bin/python3
 # -*- coding: utf-8 -*-
 
+
 import shutil
 import platform
 from pathlib import Path
 from typing import Generator
 from packaging.version import parse, InvalidVersion
 
 from slpkg.configs import Configs
 from slpkg.utilities import Utilities
 from slpkg.repositories import Repositories
 from slpkg.load_data import LoadData
 
 
-class Upgrade(Configs):
-    """ Upgrade the installed packages. """
+class Upgrade(Configs):  # pylint: disable=[R0902]
+
+    """
+    Upgrade the installed packages.
+    """
 
     def __init__(self, repository: str, data: dict):
         super(Configs, self).__init__()
         self.repository: str = repository
         self.data: dict = data
 
         self.utils = Utilities()
@@ -32,42 +36,48 @@
         self.installed_names: list = []
         self.installed_packages: list = []
 
         self.kernel_ver: str = platform.uname()[2]
         self.columns, self.rows = shutil.get_terminal_size()
 
     def load_installed_packages(self, repository: str) -> None:
+        """Summary
+
+        Args:
+            repository (str): Repository name.
+        """
         if repository == self.repos.slack_repo_name:
             extra_repo: dict = {}
 
             extra_data_file: Path = Path(self.repos.repositories[self.repos.slack_extra_repo_name]['path'],
                                          self.repos.data_json)
 
             if self.repos.repositories[self.repos.slack_extra_repo_name]['enable'] and extra_data_file.is_file():
                 extra_repo: dict = self.load_data.load(self.repos.slack_extra_repo_name, message=False)
 
             installed: dict = self.utils.all_installed()
 
             for name, package in installed.items():
                 tag: str = self.utils.split_package(package)['tag']
-                if not tag:  # Add only slackware original packages that have not package tag.
+                if not tag:  # Add only Slackware original packages that have not package tag.
                     if extra_repo.get(name):  # Avoid installed packages from extra repository.
                         extra_package: str = extra_repo[name]['package']
                         if extra_package[:-4] != package:
                             self.installed_packages.append(Path(package))
                             self.installed_names.append(name)
                     else:
                         self.installed_packages.append(Path(package))
                         self.installed_names.append(name)
         else:
             repo_tag: str = self.repos.repositories[repository]['repo_tag']
             self.installed_packages: list = list(self.log_packages.glob(f'*{repo_tag}'))
 
     def packages(self) -> Generator:
-        """ Returns the upgradable packages. """
+        """ Returns the upgradeable packages.
+        """
         # Delete log file before starts.
         if self.upgrade_log_file.is_file():
             self.upgrade_log_file.unlink()
 
         self.load_installed_packages(self.repository)
 
         for inst in self.installed_packages:
@@ -81,57 +91,73 @@
 
         if self.repository == self.repos.slack_repo_name and self.new_packages:
             for name in self.data.keys():
                 # if not self.utils.is_package_installed(name):
                 if name not in self.installed_names:
                     yield name
 
-    def is_package_upgradeable(self, installed: str) -> bool:
-        """ Returns True for upgradeable packages. """
+    def is_package_upgradeable(self, installed: str) -> bool:  # pylint: disable=[R0911]
+        """Returns True for upgradeable packages.
+
+        Args:
+            installed (str): Installed package.
+
+        Returns:
+            bool: True if the package is upgradeable.
+        """
         inst_name: str = self.utils.split_package(installed)['name']
+
         if self.data.get(inst_name):
             repo_version: str = self.data[inst_name]['version']
             repo_build: str = self.data[inst_name]['build']
 
             inst_version: str = self.utils.split_package(installed)['version']
-            if (self.kernel_version and self.repository in [self.repos.sbo_repo_name, self.repos.ponce_repo_name]
-                    and inst_version.endswith(f'_{self.kernel_ver}')):
+            if (self.kernel_version and inst_version.endswith(f'_{self.kernel_ver}')):
                 inst_version: str = inst_version.replace(f'_{self.kernel_ver}', '')
 
             inst_build: str = self.utils.split_package(installed)['build']
+
             try:
                 if parse(repo_version) > parse(inst_version):
                     return True
 
                 if parse(repo_version) == parse(inst_version) and int(repo_build) > int(inst_build):
                     return True
             except InvalidVersion as err:
                 # Different options to compare packages.
                 repo_package: str = self.data[inst_name]['package']
                 if repo_version > inst_version:  # Try to compare the strings.
                     return True
-                elif repo_version == inst_version and int(repo_build) > int(inst_build):
+                if repo_version == inst_version and int(repo_build) > int(inst_build):
                     return True
-                elif installed != repo_package[:-4]:  # Add the package if a new one on the repository.
+                if installed != repo_package[:-4]:  # Add the package if a new one on the repository.
                     return True
-                elif installed == repo_package[:-4]:  # Not new packages in the repository.
+                if installed == repo_package[:-4]:  # Not new packages in the repository.
                     return False
                 self._write_log_file(installed, inst_name, err)
 
         return False
 
     def _write_log_file(self, installed: str, name: str, err: InvalidVersion) -> None:
-        """ Writes a log file for invalid versions. """
+        """Writes a log file for invalid versions.
+
+        Args:
+            installed (str): Installed package.
+            name (str): Package name.
+            err (InvalidVersion): InvalidVersion error.
+        """
         if self.log_path.is_dir():
-            with self.upgrade_log_file.open('a') as log:
+            with self.upgrade_log_file.open('a', encoding='utf-8') as log:
                 log.write(f"Installed: {installed}, "
                           f"Repository: {self.data[name]['package']}, "
                           f"Error: {err}\n")
 
     def check_packages(self) -> None:
+        """ Checks only which packages are upgradeable.
+        """
         repo_data: dict = {}
         found_packages: dict = {}
 
         if self.repository == '*':
             repo_data: dict = self.data
         else:
             repo_data[self.repository] = self.data
@@ -144,14 +170,15 @@
 
                 if data.get(name):
                     self.data: dict = data
 
                     if self.is_package_upgradeable(installed.name):
                         self.id += 1
                         self.sum_upgrade += 1
+
                         inst_version: str = self.utils.split_package(installed.name)['version']
                         inst_build: str = self.utils.split_package(installed.name)['build']
                         repo_version: str = data[name]['version']
                         repo_build: str = data[name]['build']
 
                         found_packages[self.id] = {
                             'name': name,
@@ -195,15 +222,25 @@
                             'inst_version': '',
                             'inst_build': '',
                             'repo_version': repo_version,
                             'repo_build': repo_build,
                             'repo': self.repos.slack_repo_name,
                             'type': 'add'
                         }
+        self._results(found_packages)
+
+    def _results(self, found_packages: dict) -> None:
+        """ Prints the results of checking.
+
+        Args:
+            found_packages (dict): Data of packages.
 
+        Raises:
+            SystemExit: Exit code 0.
+        """
         if found_packages:
             print()
 
             name_alignment: int = 18
             if self.columns > 80:
                 name_alignment: int = (self.columns - 80) + 18
```

### Comparing `slpkg-5.0.6/slpkg/utilities.py` & `slpkg-5.0.7/slpkg/utilities.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 #!/usr/bin/python3
 # -*- coding: utf-8 -*-
+
+
 from __future__ import annotations
 
 import os
 import re
 import time
 import json
 import shutil
@@ -13,31 +15,47 @@
 from slpkg.configs import Configs
 from slpkg.blacklist import Blacklist
 from slpkg.error_messages import Errors
 
 
 class Utilities(Configs):
 
+    """
+    List of utilities.
+    """
+
     def __init__(self):
         super(Configs, self).__init__()
+
         self.black = Blacklist()
         self.errors = Errors()
 
     def is_package_installed(self, name: str) -> str:
-        """ Returns the installed package binary. """
+        """Returns the installed package binary.
+
+        Args:
+            name (str): Package name.
+
+        Returns:
+            str: Full package name.
+        """
         installed_package: Generator = self.log_packages.glob(f'{name}*')
 
         for installed in installed_package:
             inst_name: str = self.split_package(installed.name)['name']
             if inst_name == name and inst_name not in self.ignore_packages([inst_name]):
                 return installed.name
         return ''
 
     def all_installed(self) -> dict:
-        """ Return all installed packages from /val/log/packages folder. """
+        """Return all installed packages from /val/log/packages folder.
+
+        Returns:
+            dict: All installed packages and names.
+        """
         installed_packages: dict = {}
 
         for file in self.log_packages.glob('*'):
             name: str = self.split_package(file.name)['name']
 
             if not name.startswith('.'):
                 installed_packages[name] = file.name
@@ -47,34 +65,54 @@
             for black in blacklist_packages:
                 del installed_packages[black]
 
         return installed_packages
 
     @staticmethod
     def remove_file_if_exists(path: Path, file: str) -> None:
-        """ Remove the old files. """
+        """Remove the old files.
+
+        Args:
+            path (Path): Path to the file.
+            file (str): File name.
+        """
         archive: Path = Path(path, file)
         if archive.is_file():
             archive.unlink()
 
     @staticmethod
     def remove_folder_if_exists(folder: Path) -> None:
-        """ Remove the old folders. """
+        """Removes the folder if exist.
+
+        Args:
+            folder (Path): Path to the folder.
+        """
         if folder.exists():
             shutil.rmtree(folder)
 
     @staticmethod
     def create_directory(directory: Path) -> None:
-        """ Creates folder like mkdir -p. """
+        """Creates folder like mkdir -p.
+
+        Args:
+            directory (Path): Path to folder.
+        """
         if not directory.is_dir():
             directory.mkdir(parents=True, exist_ok=True)
 
     @staticmethod
     def split_package(package: str) -> dict:
-        """ Splits the binary package name in name, version, arch, build and tag. """
+        """Splits the binary package name in name, version, arch, build and tag.
+
+        Args:
+            package (str): Full package name for spliting.
+
+        Returns:
+            dict: Splitted package by name, version, arch, build and package tag.
+        """
         name: str = '-'.join(package.split('-')[:-3])
         version: str = ''.join(package[len(name):].split('-')[:-2])
         arch: str = ''.join(package[len(name + version) + 2:].split('-')[:-1])
         build_tag: str = package.split('-')[-1]
         build: str = ''.join(re.findall(r'\d+', build_tag[:2]))
         pkg_tag: str = build_tag[len(build):]
 
@@ -84,60 +122,88 @@
             'arch': arch,
             'build': build,
             'tag': pkg_tag
         }
 
     @staticmethod
     def finished_time(elapsed_time: float) -> None:
-        """ Printing the elapsed time. """
-        print(f'\nFinished:', time.strftime(f'%H:%M:%S', time.gmtime(elapsed_time)))
+        """Printing the elapsed time.
+
+        Args:
+            elapsed_time (float): Unformatted time.
+        """
+        print('\nFinished:', time.strftime('%H:%M:%S', time.gmtime(elapsed_time)))
 
     @staticmethod
     def is_option(options: tuple, flags: list) -> bool:
-        """ Returns True if option applied. """
+        """Returns True if option applied.
+
+        Args:
+            options (tuple): Options for checking.
+            flags (list): The flags applied by the user.
+
+        Returns:
+            bool: True if match or False, if not matched.
+        """
         for option in options:
             if option in flags:
                 return True
+        return False
 
     def read_packages_from_file(self, file: Path) -> Generator:
-        """ Reads name packages from file and split these to list. """
+        """Reads name packages from file.
+
+        Args:
+            file (Path): Path to the file.
+
+        Yields:
+            Generator: Package names.
+        """
         try:
             with open(file, 'r', encoding='utf-8') as pkgs:
                 packages: list = pkgs.read().splitlines()
 
             for package in packages:
                 if package and not package.startswith('#'):
                     if '#' in package:
                         package: str = package.split('#')[0].strip()
                     yield package
         except FileNotFoundError:
             self.errors.raise_error_message(f"No such file or directory: '{file}'", exit_status=20)
 
     def read_text_file(self, file: Path) -> list:
-        """ Reads the text file and returns it into a list. """
+        """Reads a text file.
+
+        Args:
+            file (Path): Path to the file.
+
+        Returns:
+            list: The lines in the list.
+        """
         try:
             with open(file, 'r', encoding='utf-8', errors='replace') as text_file:
                 return text_file.readlines()
         except FileNotFoundError:
             self.errors.raise_error_message(f"No such file or directory: '{file}'", exit_status=20)
+        return []
 
     def count_file_size(self, name: str) -> int:
         """
         Read the contents files from the package file list and count
         the total installation file size in bytes.
         Args:
             name: The name of the package.
 
         Returns:
             The total package installation file size.
         """
         count_files: int = 0
         installed: Path = Path(self.log_packages, self.is_package_installed(name))
         if installed:
-            file_installed: list = installed.read_text().splitlines()
+            file_installed: list = installed.read_text(encoding="utf-8").splitlines()
             for line in file_installed:
                 file: Path = Path('/', line)
                 if file.is_file():
                     count_files += file.stat().st_size
         return count_files
 
     @staticmethod
@@ -151,39 +217,60 @@
         """
         kb_size: float = byte_size / 1024
         mb_size: float = kb_size / 1024
         gb_size: float = mb_size / 1024
 
         if gb_size >= 1:
             return f"{gb_size:.0f} GB"
-        elif mb_size >= 1:
+        if mb_size >= 1:
             return f"{mb_size:.0f} MB"
-        elif kb_size >= 1:
+        if kb_size >= 1:
             return f"{kb_size:.0f} KB"
-        else:
-            return f"{byte_size} B"
+
+        return f"{byte_size} B"
 
     @staticmethod
     def apply_package_pattern(data: dict, packages: list) -> list:
-        """ If the '*' applied returns all the package names. """
+        """If the '*' applied returns all the package names.
+
+        Args:
+            data (dict): The repository data.
+            packages (list): The packages that applied.
+
+        Returns:
+            list: Package names.
+        """
         for pkg in packages:
             if pkg == '*':
                 packages.remove('*')
                 packages.extend(list(data.keys()))
         return packages
 
     @staticmethod
     def change_owner_privileges(folder: Path) -> None:
-        """ Changes the owner privileges. """
+        """Changes the owner privileges.
+
+        Args:
+            folder (Path): Path to the folder.
+        """
         os.chown(folder, 0, 0)
         for file in os.listdir(folder):
             os.chown(Path(folder, file), 0, 0)
 
     def case_insensitive_pattern_matching(self, packages: list, data: dict, flags: list) -> list:
-        """ Case-insensitive pattern matching packages. """
+        """Case-insensitive pattern matching packages.
+
+        Args:
+            packages (list): List of packages.
+            data (dict): Repository data.
+            flags (list): User options.
+
+        Returns:
+            list: Matched packages.
+        """
         if self.is_option(('-m', '--no-case'), flags):
             repo_packages: tuple = tuple(data.keys())
             for package in packages:
                 for pkg in repo_packages:
                     if package.lower() == pkg.lower():
                         packages.append(pkg)
                         packages.remove(package)
@@ -207,26 +294,33 @@
             pass
         return json_data
 
     def ignore_packages(self, packages: list) -> list:
         """
         Matching packages using regular expression.
         Args:
-            packages: Tha packages to apply the pattern.
+            packages: The packages to apply the pattern.
         Returns:
             The matching packages.
         """
         matching_packages: list = []
         blacklist: tuple = self.black.packages()
         if blacklist:
             pattern: str = '|'.join(blacklist)
             matching_packages: list = [pkg for pkg in packages if re.search(pattern, pkg)]
         return matching_packages
 
     def convert_dict_keys_to_lower(self, d: dict) -> dict:
+        """ Converts dictionary keys to lower.
+
+        Args:
+            d (dict): Dictionary data.
+
+        Returns:
+            dict: Dictionary in lower case.
+        """
         new_dict = {}
         for key, value in d.items():
             if isinstance(value, dict):
                 value = self.convert_dict_keys_to_lower(value)
             new_dict[key.lower()] = value
         return new_dict
-
```

### Comparing `slpkg-5.0.6/slpkg/views/asciibox.py` & `slpkg-5.0.7/slpkg/views/asciibox.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,27 +1,34 @@
 #!/usr/bin/python3
 # -*- coding: utf-8 -*-
 
+
 import shutil
 
 from slpkg.configs import Configs
 
 
-class AsciiBox(Configs):
+class AsciiBox(Configs):  # pylint: disable=[R0902]
+
+    """
+    Managing the ASCII characters.
+    """
 
     def __init__(self):
         super(Configs, self).__init__()
         self.columns, self.rows = shutil.get_terminal_size()
         self.package_alignment: int = self.columns - 56
         self.version_alignment: int = 29
         self.size_alignment: int = 9
         self.repo_alignment: int = 14
 
-        if self.package_alignment < 1:
-            self.package_alignment = 1
+        # if self.package_alignment < 1:
+        #     self.package_alignment = 1
+
+        self.package_alignment = max(self.package_alignment, 1)
 
         self.bd_color: str = self.endc
         self.border_colors: dict = {}
         self.assign_border_color()
 
         self.bullet: str = '-'
         self.done: str = 'Done'
@@ -53,15 +60,17 @@
             self.lower_right_corner: str = '┘'
             self.upper_left_corner: str = '┌'
             self.horizontal_and_up: str = '┴'
             self.horizontal_and_down: str = '┬'
             self.vertical_and_right: str = '├'
             self.vertical_and_left: str = '┤'
 
-    def assign_border_color(self):
+    def assign_border_color(self) -> None:
+        """ Assign the colors.
+        """
         self.border_colors: dict = {
             'red': self.red,
             'blue': self.blue,
             'cyan': self.cyan,
             'white': self.endc,
             'green': self.green,
             'yellow': self.yellow,
@@ -73,49 +82,77 @@
         }
         try:
             self.bd_color: str = self.border_colors[self.border_color]
         except KeyError:
             self.bd_color: str = self.endc
 
     def draw_package_title(self, message: str, title: str) -> None:
+        """ Draw the package title.
+
+        Args:
+            message (str): Message about the action.
+            title (str): Slpkg title.
+        """
         title = title.title()
         print(f"{self.bd_color}{self.upper_left_corner}{self.horizontal_line * (self.columns - 2)}"
               f"{self.upper_right_corner}")
         print(f"{self.vertical_line}{title.center(self.columns - 2, ' ')}{self.vertical_line}")
         self.draw_middle_line()
         print(f"{self.vertical_line} {self.endc}{message.ljust(self.columns - 3, ' ')}"
               f"{self.bd_color}{self.vertical_line}")
         self.draw_middle_line()
         print(f"{self.bd_color}{self.vertical_line}{self.endc} {'Package:':<{self.package_alignment}}"
               f"{'Version:':<{self.version_alignment}}{'Size:':<{self.size_alignment}}{'Repo:':>{self.repo_alignment}} "
               f"{self.bd_color}{self.vertical_line}{self.endc}")
 
-    def draw_package_line(self, package: str, version: str, size: str, color: str, repo: str) -> None:
+    def draw_package_line(self, package: str, version: str, size: str, color: str, repo: str) -> None:  # pylint: disable=[R0913]
+        """ Draw the package line.
+
+        Args:
+            package (str): Package name.
+            version (str): Package version.
+            size (str): Package size.
+            color (str): Package highlight.
+            repo (str): Repository name.
+        """
         if len(version) >= (self.version_alignment - 5):
             version: str = f'{version[:self.version_alignment - 5]}...'
         if len(package) >= (self.package_alignment - 4):
             package: str = f'{package[:self.package_alignment - 4]}...'
 
         print(f"{self.bd_color}{self.vertical_line} {self.bold}{color}{package:<{self.package_alignment}}{self.endc}"
               f"{self.bd_color}{version:<{self.version_alignment}}{self.endc}{size:<{self.size_alignment}}{self.blue}"
               f"{repo:>{self.repo_alignment}}{self.bd_color} {self.vertical_line}{self.endc}")
 
     def draw_middle_line(self) -> None:
+        """ Draw the middle line
+        """
         print(f"{self.bd_color}{self.vertical_and_right}{self.horizontal_line * (self.columns - 2)}"
               f"{self.vertical_and_left}")
 
     def draw_dependency_line(self) -> None:
+        """ Draw the dependency line.
+        """
         print(f"{self.bd_color}{self.vertical_line}{self.endc} Dependencies:{' ' * (self.columns - 16)}"
               f"{self.bd_color}{self.vertical_line}{self.endc}")
 
     def draw_bottom_line(self) -> None:
+        """ Draw the bottom line.
+        """
         print(f"{self.bd_color}{self.lower_left_corner}{self.horizontal_line * (self.columns - 2)}"
               f"{self.lower_right_corner}{self.endc}")
 
     def draw_checksum_error_box(self, name: str, checksum: str, file_check: str) -> None:
+        """ Draw a checksum error box.
+
+        Args:
+            name (str): Package name.
+            checksum (str): Expected checksum.
+            file_check (str): Found checksum.
+        """
         print(f"{self.bred}{self.upper_left_corner}{self.horizontal_line * (self.columns - 2)}"
               f"{self.upper_right_corner}")
         print(f"{self.bred}{self.vertical_line}{self.bred} FAILED:{self.endc} MD5SUM check for "
               f"'{self.cyan}{name}'{' ' * (self.columns - len(name) - 30)}{self.red}{self.vertical_line}")
         print(f"{self.bred}{self.vertical_and_right}{self.horizontal_line * (self.columns - 2)}"
               f"{self.vertical_and_left}")
         print(f"{self.bred}{self.vertical_line}{self.yellow} Expected:{self.endc} {checksum}{self.bred}"
```

### Comparing `slpkg-5.0.6/slpkg/views/cli_menu.py` & `slpkg-5.0.7/slpkg/views/cli_menu.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,33 +1,52 @@
 #!/usr/bin/python3
 # -*- coding: utf-8 -*-
 
+
 from typing import NoReturn
 from slpkg.configs import Configs
 from slpkg.views.version import Version
 
 
 class Usage(Configs):
 
+    """
+    CLI Usage menu.
+    """
+
     def __init__(self):
         super(Configs, self).__init__()
 
     def help_minimal(self, message: str) -> NoReturn:
-        """ Prints the minimal help menu. """
+        """ Prints the minimal help menu.
+
+        Args:
+            message (str): Message of error.
+
+        Raises:
+            SystemExit: Raises an exit code 1.
+        """
         print(message)
         args: str = (
             f'Usage: {self.prog_name} [{self.cyan}COMMAND{self.endc}] [{self.yellow}OPTIONS{self.endc}] '
             f'<packages>\n'
             f"\nTry '{self.prog_name} --help' for more options.")
 
         print(args)
         raise SystemExit(1)
 
     def help_short(self, status: int) -> NoReturn:
-        """ Prints the short menu. """
+        """Prints the short menu.
+
+        Args:
+            status (int): Status exit code.
+
+        Raises:
+            SystemExit: Raises the status code.
+        """
         args: str = (
             f'USAGE: {self.prog_name} [{self.cyan}COMMAND{self.endc}] [{self.yellow}OPTIONS{self.endc}] '
             f'<packages>\n'
             f'\n  slpkg [{self.cyan}COMMAND{self.endc}] [-u, update, -U, upgrade]\n'
             f'  slpkg [{self.cyan}COMMAND{self.endc}] [-I, repo-info, -g, configs, -T, clean-tmp]\n'
             f'  slpkg [{self.cyan}COMMAND{self.endc}] [-b, build, -i, install, -R, remove <packages>]\n'
             f'  slpkg [{self.cyan}COMMAND{self.endc}] [-d, download, -f, find, -w, view <packages>]\n'
@@ -39,15 +58,22 @@
             f'  slpkg [{self.yellow}OPTIONS{self.endc}] [-o, --repository=NAME, -z, --directory=PATH]\n'
             "  \nIf you need more information please try 'slpkg --help'.")
 
         print(args)
         raise SystemExit(status)
 
     def help(self, status: int) -> NoReturn:
-        """ Prints the main menu. """
+        """Prints the main menu.
+
+        Args:
+            status (int): Status exit code
+
+        Raises:
+            SystemExit: Raises the status code.
+        """
         args: str = (
             f'{self.prog_name} - version {Version().version}\n\n'
             f'{self.bold}USAGE:{self.endc}\n  {self.prog_name} [{self.cyan}COMMAND{self.endc}] '
             f'[{self.yellow}OPTIONS{self.endc}] <packages>\n'
             f'\n{self.bold}DESCRIPTION:{self.endc}\n  Package manager utility for Slackware.\n'
             f'\n{self.bold}COMMANDS:{self.endc}\n'
             f'  {self.red}-u, update{self.endc}                Synchronizes the repositories database\n'
```

### Comparing `slpkg-5.0.6/slpkg/views/version.py` & `slpkg-5.0.7/slpkg/views/version.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 #!/usr/bin/python3
 # -*- coding: utf-8 -*-
 
-class Version:
+
+class Version:  # pylint: disable=[R0903]
     """ Print the version. """
 
     def __init__(self):
-        self.version_info: tuple = (5, 0, 6)
-        self.version: str = '{0}.{1}.{2}'.format(*self.version_info)
+        self.version: str = "5.0.7"
         self.license: str = 'GNU General Public License v3 (GPLv3)'
         self.author: str = 'Dimitris Zlatanidis (dslackw)'
         self.homepage: str = 'https://dslackw.gitlab.io/slpkg'
         self.email: str = 'dslackw@gmail.com'
 
     def view(self) -> None:
         """ Prints the version. """
```

### Comparing `slpkg-5.0.6/slpkg/views/view_package.py` & `slpkg-5.0.7/slpkg/views/view_package.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,22 +1,27 @@
 #!/usr/bin/python3
 # -*- coding: utf-8 -*-
 
+
 from pathlib import Path
 
 from slpkg.configs import Configs
 from slpkg.utilities import Utilities
 from slpkg.repositories import Repositories
 
 
-class ViewPackage(Configs):
-    """ View the repository packages. """
+class ViewPackage(Configs):  # pylint: disable=[R0902]
+
+    """
+    View the packages information.
+    """
 
     def __init__(self, flags: list, repository: str):
         super(Configs, self).__init__()
+
         self.flags: list = flags
         self.repository: str = repository
 
         self.utils = Utilities()
         self.repos = Repositories()
 
         self.repository_packages: tuple = ()
@@ -30,27 +35,32 @@
         self.dependencies: str = ''
         self.repo_tar_suffix: str = ''
 
         self.option_for_pkg_version: bool = self.utils.is_option(
             ('-p', '--pkg-version'), flags)
 
     def slackbuild(self, data: dict, slackbuilds: list) -> None:
-        """ View slackbuild packages information. """
+        """View slackbuilds information.
+
+        Args:
+            data (dict): Repository data.
+            slackbuilds (list): List of slackbuilds.
+        """
         print()
         repo: dict = {
             self.repos.sbo_repo_name: self.repos.sbo_repo_tar_suffix,
             self.repos.ponce_repo_name: ''
         }
         self.repo_tar_suffix: str = repo[self.repository]
         self.repository_packages: tuple = tuple(data.keys())
 
         for sbo in slackbuilds:
             for name, item in data.items():
 
-                if sbo == name or sbo == '*':
+                if sbo in [name, '*']:
                     path_file: Path = Path(self.repos.repositories[self.repository]['path'],
                                            item['location'], name, 'README')
                     path_info: Path = Path(self.repos.repositories[self.repository]['path'],
                                            item['location'], name, f'{name}.info')
 
                     self.read_the_readme_file(path_file)
                     self.read_the_info_file(path_info)
@@ -58,42 +68,73 @@
                     self.assign_the_sbo_mirror()
                     self.assign_the_info_file_variables()
                     self.assign_dependencies(item)
                     self.assign_dependencies_with_version(item, data)
                     self.view_slackbuild_package(name, item)
 
     def read_the_readme_file(self, path_file: Path) -> None:
+        """ Reads the README file.
+
+        Args:
+            path_file (Path): Path to the file.
+        """
         self.readme: list = self.utils.read_text_file(path_file)
 
     def read_the_info_file(self, path_info: Path) -> None:
+        """ reads the .info file.
+
+        Args:
+            path_info (Path): Path to the file.
+        """
         self.info_file: list = self.utils.read_text_file(path_info)
 
     def assign_the_sbo_mirror(self) -> None:
+        """ Assign the url for the PACKAGES.TXT file.
+        """
         self.mirror: str = self.repos.repositories[self.repository]['mirror_packages']
 
     def assign_the_info_file_variables(self) -> None:
+        """ Assign data from the .info file.
+        """
         for line in self.info_file:
             if line.startswith('HOMEPAGE'):
                 self.homepage: str = line[10:-2].strip()
             if line.startswith('MAINTAINER'):
                 self.maintainer: str = line[12:-2].strip()
             if line.startswith('EMAIL'):
                 self.email: str = line[7:-2].strip()
 
     def assign_dependencies(self, item: dict) -> None:
-        self.dependencies: str = (', '.join([f'{self.cyan}{pkg}' for pkg in item['requires']]))
+        """Assign the package dependencies.
+
+        Args:
+            item (dict): Data value.
+        """
+        self.dependencies: str = ', '.join([f'{self.cyan}{pkg}' for pkg in item['requires']])
 
     def assign_dependencies_with_version(self, item: dict, data: dict) -> None:
+        """ Assign dependencies with version.
+
+        Args:
+            item (dict): Data value.
+            data (dict): Repository data.
+        """
         if self.option_for_pkg_version:
             self.dependencies: str = (', '.join(
                 [f"{self.cyan}{pkg}{self.endc}-{self.yellow}{data[pkg]['version']}"
                  f"{self.green}" for pkg in item['requires']
                  if pkg in self.repository_packages]))
 
     def view_slackbuild_package(self, name: str, item: dict) -> None:
+        """ Prints slackbuild information.
+
+        Args:
+            name (str): Slackbuild name.
+            item (dict): Data value.
+        """
         space_align: str = ''
         print(f"{'Repository':<15}: {self.green}{self.repository}{self.endc}\n"
               f"{'Name':<15}: {self.green}{name}{self.endc}\n"
               f"{'Version':<15}: {self.green}{item['version']}{self.endc}\n"
               f"{'Build':<15}: {self.green}{self.repo_build_tag}{self.endc}\n"
               f"{'Homepage':<15}: {self.blue}{self.homepage}{self.endc}\n"
               f"{'Download SBo':<15}: {self.blue}{self.mirror}"
@@ -108,26 +149,37 @@
               f"{'Maintainer':<15}: {self.yellow}{self.maintainer}{self.endc}\n"
               f"{'Email':<15}: {self.yellow}{self.email}{self.endc}\n"
               f"{'Requires':<15}: {self.green}{self.dependencies}{self.endc}\n"
               f"{'Description':<15}: {self.green}{item['description']}{self.endc}\n"
               f"{'README':<15}: {self.cyan}{f'{space_align:>17}'.join(self.readme)}{self.endc}")
 
     def package(self, data: dict, packages: list) -> None:
-        """ View binary packages information. """
+        """ View binary packages information.
+
+        Args:
+            data (dict): Repository data.
+            packages (list): List of packages.
+        """
         print()
         self.repository_packages: tuple = tuple(data.keys())
         for package in packages:
             for name, item in data.items():
-                if package == name or package == '*':
+                if package in [name, '*']:
 
                     self.assign_dependencies(item)
                     self.assign_dependencies_with_version(item, data)
                     self.view_binary_package(name, item)
 
     def view_binary_package(self, name: str, item: dict) -> None:
+        """ Print binary packages information.
+
+        Args:
+            name (str): Package name.
+            item (dict): Data values.
+        """
         print(f"{'Repository':<15}: {self.green}{self.repository}{self.endc}\n"
               f"{'Name':<15}: {self.green}{name}{self.endc}\n"
               f"{'Version':<15}: {self.green}{item['version']}{self.endc}\n"
               f"{'Build':<15}: {self.green}{item['build']}{self.endc}\n"
               f"{'Package':<15}: {self.cyan}{item['package']}{self.endc}\n"
               f"{'Download':<15}: {self.blue}{item['mirror']}{item['location']}/{item['package']}{self.endc}\n"
               f"{'Md5sum':<15}: {item['checksum']}\n"
```

### Comparing `slpkg-5.0.6/slpkg/views/views.py` & `slpkg-5.0.7/slpkg/views/views.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,27 +1,32 @@
 #!/usr/bin/python3
 # -*- coding: utf-8 -*-
 
+
 import shutil
-from typing import Any
 from pathlib import Path
 
 from slpkg.configs import Configs
 from slpkg.upgrade import Upgrade
 from slpkg.utilities import Utilities
 from slpkg.views.asciibox import AsciiBox
 from slpkg.repositories import Repositories
 
 
-class View(Configs):
+class View(Configs):  # pylint: disable=[R0902]
+
+    """ Views packages for build, install, remove or download.
+    """
 
-    def __init__(self, flags=None, repository=None, data=None):
+    def __init__(self, flags: list = None, repository: str = None, data: dict = None):
         super(Configs, self).__init__()
+
         if flags is None:
             flags: list = []
+
         self.flags: list = flags
         self.repository: str = repository
         self.data: dict = data
 
         self.repos = Repositories()
         self.utils = Utilities()
         self.ascii = AsciiBox()
@@ -41,99 +46,134 @@
         self.option_for_reinstall: bool = self.utils.is_option(
             ('-r', '--reinstall'), flags)
 
         self.option_for_yes: bool = self.utils.is_option(
             ('-y', '--yes'), flags)
 
     def build_packages(self, slackbuilds: list, dependencies: list) -> None:
+        """ View packages for build method.
+
+        Args:
+            slackbuilds (list): Slackbuilds for build.
+            dependencies (list): Dependencies for build.
+        """
         mode: str = 'build'
         self.ascii.draw_package_title('The following packages will be build:',
                                       'slpkg build packages')
 
         for slackbuild in slackbuilds:
-            self.build_package(slackbuild)
+            self.draw_build_package(slackbuild)
             self.summary(slackbuild, mode)
 
         if dependencies:
             self.ascii.draw_middle_line()
             self.ascii.draw_dependency_line()
 
             for dependency in dependencies:
-                self.build_package(dependency)
+                self.draw_build_package(dependency)
                 self.summary(dependency, mode)
 
         self.ascii.draw_bottom_line()
         self.set_summary_for_build(slackbuilds + dependencies)
         print(self.summary_message)
 
     def install_upgrade_packages(self, packages: list, dependencies: list, mode: str) -> None:
+        """ View packages for install or upgrade.
+
+        Args:
+            packages (list): Packages for install.
+            dependencies (list): Dependencies for install.
+            mode (str): Type of mode.
+        """
         title: str = 'slpkg install packages'
         if mode == 'upgrade':
             title: str = 'slpkg upgrade packages'
         self.ascii.draw_package_title('The following packages will be installed or upgraded:', title)
 
         for package in packages:
-            self.install_upgrade_package(package)
+            self.draw_install_upgrade_package(package)
             self.summary(package, mode)
 
         if dependencies:
             self.ascii.draw_middle_line()
             self.ascii.draw_dependency_line()
 
             for dependency in dependencies:
-                self.install_upgrade_package(dependency)
+                self.draw_install_upgrade_package(dependency)
                 self.summary(dependency, mode)
 
         self.ascii.draw_bottom_line()
         self.set_summary_for_install_and_upgrade(self.sum_install, self.sum_upgrade,
                                                  self.sum_size_comp, self.sum_size_uncomp)
         print(self.summary_message)
 
     def download_packages(self, packages: list, directory: Path) -> None:
+        """ View packages for download method.
+
+        Args:
+            packages (list): Packages name for download.
+            directory (Path): Path to download.
+        """
         mode: str = 'download'
         self.download_only: Path = directory
         self.ascii.draw_package_title('The following packages will be downloaded:',
                                       'slpkg download packages')
 
         for package in packages:
-            self.download_package(package)
+            self.draw_download_package(package)
             self.summary(package, mode)
 
         self.ascii.draw_bottom_line()
         self.set_summary_for_download(packages, self.sum_size_comp)
         print(self.summary_message)
 
-    def remove_packages(self, packages: list, dependencies: list) -> Any:
+    def remove_packages(self, packages: list, dependencies: list) -> None:
+        """ View packages for remove.
+
+        Args:
+            packages (list): List of packages.
+            dependencies (list): List of dependencies.
+        """
         mode: str = 'remove'
         self.ascii.draw_package_title('The following packages will be removed:',
                                       'slpkg remove packages')
         for package in packages:
-            self.remove_package(package)
+            self.draw_remove_package(package)
             self.summary(package, mode)
 
         if dependencies:
             self.ascii.draw_middle_line()
             self.ascii.draw_dependency_line()
 
             for dependency in dependencies:
-                self.remove_package(dependency)
+                self.draw_remove_package(dependency)
                 self.summary(dependency, mode)
 
         self.ascii.draw_bottom_line()
         self.set_summary_for_remove(self.sum_remove, self.sum_size_remove)
         print(self.summary_message)
 
-    def build_package(self, package: str) -> None:
+    def draw_build_package(self, package: str) -> None:
+        """ Draw line for build package method.
+
+        Args:
+            package (str): Package name.
+        """
         size: str = ''
         color: str = self.yellow
         version: str = self.data[package]['version']
 
         self.ascii.draw_package_line(package, version, size, color, self.repository)
 
-    def install_upgrade_package(self, package: str) -> None:
+    def draw_install_upgrade_package(self, package: str) -> None:
+        """ Draw line for install or upgrade package method.
+
+        Args:
+            package (str): Package name.
+        """
         size: str = ''
         color: str = self.cyan
         version: str = self.data[package]['version']
         installed: str = self.utils.is_package_installed(package)
         upgradable: bool = self.upgrade.is_package_upgradeable(installed)
 
         if self.repository not in [self.repos.sbo_repo_name, self.repos.ponce_repo_name]:
@@ -149,97 +189,159 @@
 
         if installed and self.option_for_reinstall and not upgradable:
             color: str = self.violet
             package: str = self.build_package_and_version(package)
 
         self.ascii.draw_package_line(package, version, size, color, self.repository)
 
-    def download_package(self, package: str) -> None:
+    def draw_download_package(self, package: str) -> None:
+        """ Draw package for download method.
+
+        Args:
+            package (str): Package name.
+        """
         size: str = ''
         color: str = self.cyan
         version: str = self.data[package]['version']
 
         if self.repository not in [self.repos.sbo_repo_name, self.repos.ponce_repo_name]:
             size_comp: float = float(self.data[package]['size_comp']) * 1024
             size: str = self.utils.convert_file_sizes(size_comp)
 
         self.ascii.draw_package_line(package, version, size, color, self.repository)
 
-    def remove_package(self, package: str) -> None:
+    def draw_remove_package(self, package: str) -> None:
+        """ Draw package for remove method.
+
+        Args:
+            package (str): Package name.
+        """
         count_size: int = self.utils.count_file_size(package)
         installed: str = self.utils.is_package_installed(package)
         version: str = self.utils.split_package(installed)['version']
         repo_tag: str = self.utils.split_package(installed)['tag']
         size: str = self.utils.convert_file_sizes(count_size)
         repository: str = repo_tag.lower().replace('_', '')
 
         self.ascii.draw_package_line(package, version, size, self.red, repository)
 
-    def summary(self, package: str, option: str) -> None:
+    def summary(self, package: str, method: str) -> None:
+        """ Counts packages per method.
+
+        Args:
+            package (str): Package name.
+            method (str): Type of method.
+        """
         installed: str = self.utils.is_package_installed(package)
 
-        if self.repository not in list(self.repos.repositories.keys())[:2] and self.repository is not None:
+        if self.repository not in list(self.repos.repositories)[:2] and self.repository is not None:
             self.sum_size_comp += float(self.data[package]['size_comp']) * 1024
             self.sum_size_uncomp += float(self.data[package]['size_uncomp']) * 1024
 
-        if installed and option == 'remove':
+        if installed and method == 'remove':
             self.sum_size_remove += self.utils.count_file_size(package)
 
         upgradeable: bool = False
-        if option != 'remove':
+        if method != 'remove':
             upgradeable: bool = self.upgrade.is_package_upgradeable(installed)
 
         if not installed:
             self.sum_install += 1
         elif installed and self.option_for_reinstall:
             self.sum_upgrade += 1
         elif upgradeable:
             self.sum_upgrade += 1
-        elif installed and option == 'remove':
+        elif installed and method == 'remove':
             self.sum_remove += 1
 
     def set_summary_for_build(self, packages: list) -> None:
+        """ Sets summary message for build.
+
+        Args:
+            packages (list): List of packages.
+        """
         self.summary_message: str = (
             f'{self.grey}Total {len(packages)} packages '
             f'will be build in {self.tmp_path} folder.{self.endc}')
 
     def set_summary_for_install_and_upgrade(self, install: int, upgrade: int, size_comp: int, size_uncomp: int) -> None:
+        """ Sets summary for install or upgrade.
+
+        Args:
+            install (int): Counts for installs.
+            upgrade (int): Counts for upgrades.
+            size_comp (int): Counts of compressed sizes.
+            size_uncomp (int): Counts of uncompressed sizes.
+        """
         split_message: str = '\n'
         if self.columns > 80:
             split_message: str = ''
         total_packages: str = (f'{self.grey}Total {install} packages will be installed and {upgrade} '
                                f'will be upgraded, while a total ')
         total_sizes: str = (f'{self.utils.convert_file_sizes(size_comp)} will be downloaded and '
                             f'{self.utils.convert_file_sizes(size_uncomp)} will be installed.{self.endc}')
         self.summary_message: str = f'{total_packages}{split_message}{total_sizes}'
 
     def set_summary_for_remove(self, remove: int, size_rmv: int) -> None:
+        """ Sets summary for removes.
+
+        Args:
+            remove (int): Counts of removes.
+            size_rmv (int): Size of removes.
+        """
         self.summary_message: str = (
             f'{self.grey}Total {remove} packages '
             f'will be removed and {self.utils.convert_file_sizes(size_rmv)} '
             f'of space will be freed up.{self.endc}')
 
     def set_summary_for_download(self, packages: list, size_comp: int) -> None:
+        """ Sets summary for downloads.
+
+        Args:
+            packages (list): List of packages.
+            size_comp (int): Size of downloads.
+        """
         self.summary_message: str = (
             f'{self.grey}Total {len(packages)} packages and {self.utils.convert_file_sizes(size_comp)} '
             f'will be downloaded in {self.download_only} folder.{self.endc}')
 
     def build_package_and_version(self, package: str) -> str:
+        """ Builds package and version.
+
+        Args:
+            package (str): Package name.
+
+        Returns:
+            str: Package with the version.
+        """
         installed_package: str = self.utils.is_package_installed(package)
         version: str = self.utils.split_package(installed_package)['version']
         return f'{package}-{version}'
 
     def skipping_packages(self, packages: list) -> None:
+        """ View skipped packages.
+
+        Args:
+            packages (list): List of packages.
+        """
         if packages:
             print('Packages skipped by the user:\n')
             for name in packages:
                 failed: str = f'{self.red}{self.ascii.skipped}{self.endc}'
                 print(f"\r{'':>2}{self.bred}{self.ascii.bullet}{self.endc} "
                       f"{self.data[name]['package']} {failed}{' ' * 17}")
             print()
 
-    def question(self, message='Do you want to continue?') -> None:
+    def question(self, message: str = 'Do you want to continue?') -> None:
+        """ View a question.
+
+        Args:
+            message (str, optional): Message of question.
+
+        Raises:
+            SystemExit: Raise a exit code 0.
+        """
         if not self.option_for_yes and self.ask_question:
             answer: str = input(f'\n{message} [y/N] ')
             if answer not in ['Y', 'y']:
                 raise SystemExit(0)
         print()
```

### Comparing `slpkg-5.0.6/PKG-INFO` & `slpkg-5.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slpkg
-Version: 5.0.6
+Version: 5.0.7
 Summary: Package manager utility for Slackware Linux
 Keywords: slackware,linux,package,manager,tool
 Author-email: Dimitris Zlatanidis <dslackw@gmail.com>
 Maintainer-email: Dimitris Zlatanidis <dslackw@gmail.com>
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: slpkg Version: 5.0.6 Summary: Package manager
+Metadata-Version: 2.1 Name: slpkg Version: 5.0.7 Summary: Package manager
 utility for Slackware Linux Keywords: slackware,linux,package,manager,tool
 Author-email: Dimitris Zlatanidis
 gmail.com> Maintainer-email: Dimitris Zlatanidis
 gmail.com> Requires-Python: >=3.9 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Natural Language :: English Classifier: Environment :: Console
 Classifier: Operating System :: POSIX Classifier: Operating System :: POSIX ::
```

