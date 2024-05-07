# Comparing `tmp/biaplotter-0.0.1.tar.gz` & `tmp/biaplotter-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "biaplotter-0.0.1.tar", last modified: Mon May  6 09:48:32 2024, max compression
+gzip compressed data, was "biaplotter-0.0.2.tar", last modified: Tue May  7 13:47:55 2024, max compression
```

## Comparing `biaplotter-0.0.1.tar` & `biaplotter-0.0.2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0        0        0        0 2024-05-06 09:48:32.847975 biaplotter-0.0.1/
--rw-rw-rw-   0        0        0     1582 2024-03-27 10:29:48.000000 biaplotter-0.0.1/LICENSE
--rw-rw-rw-   0        0        0      101 2024-03-27 10:02:04.000000 biaplotter-0.0.1/MANIFEST.in
--rw-rw-rw-   0        0        0     5033 2024-05-06 09:48:32.846987 biaplotter-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     3426 2024-05-03 12:30:29.000000 biaplotter-0.0.1/README.md
--rw-rw-rw-   0        0        0     1243 2024-05-03 12:30:29.000000 biaplotter-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0     1732 2024-05-06 09:48:32.851971 biaplotter-0.0.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-05-06 09:48:32.772489 biaplotter-0.0.1/src/
-drwxrwxrwx   0        0        0        0 2024-05-06 09:48:32.810316 biaplotter-0.0.1/src/biaplotter/
--rw-rw-rw-   0        0        0      362 2024-05-03 12:30:29.000000 biaplotter-0.0.1/src/biaplotter/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-06 09:48:32.841956 biaplotter-0.0.1/src/biaplotter/_tests/
--rw-rw-rw-   0        0        0        0 2024-03-27 10:02:04.000000 biaplotter-0.0.1/src/biaplotter/_tests/__init__.py
--rw-rw-rw-   0        0        0     3870 2024-05-03 15:07:26.000000 biaplotter-0.0.1/src/biaplotter/_tests/test_artists.py
--rw-rw-rw-   0        0        0     4318 2024-04-11 09:35:42.000000 biaplotter-0.0.1/src/biaplotter/_tests/test_selectors.py
--rw-rw-rw-   0        0        0      413 2024-04-10 08:33:29.000000 biaplotter-0.0.1/src/biaplotter/_tests/test_widget.py
--rw-rw-rw-   0        0        0    17797 2024-05-03 15:07:26.000000 biaplotter-0.0.1/src/biaplotter/artists.py
--rw-rw-rw-   0        0        0      519 2024-05-03 12:30:29.000000 biaplotter-0.0.1/src/biaplotter/napari.yaml
--rw-rw-rw-   0        0        0    10886 2024-05-03 12:30:29.000000 biaplotter-0.0.1/src/biaplotter/plotter.py
--rw-rw-rw-   0        0        0    18794 2024-05-06 09:46:37.000000 biaplotter-0.0.1/src/biaplotter/selectors.py
-drwxrwxrwx   0        0        0        0 2024-05-06 09:48:32.844989 biaplotter-0.0.1/src/biaplotter.egg-info/
--rw-rw-rw-   0        0        0     5033 2024-05-06 09:48:32.000000 biaplotter-0.0.1/src/biaplotter.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      567 2024-05-06 09:48:32.000000 biaplotter-0.0.1/src/biaplotter.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-06 09:48:32.000000 biaplotter-0.0.1/src/biaplotter.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       54 2024-05-06 09:48:32.000000 biaplotter-0.0.1/src/biaplotter.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      116 2024-05-06 09:48:32.000000 biaplotter-0.0.1/src/biaplotter.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-05-06 09:48:32.000000 biaplotter-0.0.1/src/biaplotter.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 13:47:55.919432 biaplotter-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1554 2024-05-07 13:47:45.000000 biaplotter-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-07 13:47:45.000000 biaplotter-0.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4899 2024-05-07 13:47:55.919432 biaplotter-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3331 2024-05-07 13:47:45.000000 biaplotter-0.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1187 2024-05-07 13:47:45.000000 biaplotter-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1667 2024-05-07 13:47:55.919432 biaplotter-0.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 13:47:55.915432 biaplotter-0.0.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 13:47:55.915432 biaplotter-0.0.2/src/biaplotter/
+-rw-r--r--   0 runner    (1001) docker     (127)      354 2024-05-07 13:47:45.000000 biaplotter-0.0.2/src/biaplotter/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 13:47:55.919432 biaplotter-0.0.2/src/biaplotter/_tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 13:47:45.000000 biaplotter-0.0.2/src/biaplotter/_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3767 2024-05-07 13:47:45.000000 biaplotter-0.0.2/src/biaplotter/_tests/test_artists.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4212 2024-05-07 13:47:45.000000 biaplotter-0.0.2/src/biaplotter/_tests/test_selectors.py
+-rw-r--r--   0 runner    (1001) docker     (127)      395 2024-05-07 13:47:45.000000 biaplotter-0.0.2/src/biaplotter/_tests/test_widget.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17302 2024-05-07 13:47:45.000000 biaplotter-0.0.2/src/biaplotter/artists.py
+-rw-r--r--   0 runner    (1001) docker     (127)      505 2024-05-07 13:47:45.000000 biaplotter-0.0.2/src/biaplotter/napari.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    10621 2024-05-07 13:47:45.000000 biaplotter-0.0.2/src/biaplotter/plotter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18420 2024-05-07 13:47:45.000000 biaplotter-0.0.2/src/biaplotter/selectors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 13:47:55.919432 biaplotter-0.0.2/src/biaplotter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4899 2024-05-07 13:47:55.000000 biaplotter-0.0.2/src/biaplotter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      567 2024-05-07 13:47:55.000000 biaplotter-0.0.2/src/biaplotter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 13:47:55.000000 biaplotter-0.0.2/src/biaplotter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-07 13:47:55.000000 biaplotter-0.0.2/src/biaplotter.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-05-07 13:47:55.000000 biaplotter-0.0.2/src/biaplotter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-07 13:47:55.000000 biaplotter-0.0.2/src/biaplotter.egg-info/top_level.txt
```

### Comparing `biaplotter-0.0.1/LICENSE` & `biaplotter-0.0.2/LICENSE`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,28 +1,28 @@
-
-Copyright (c) 2024, DFG Cluster of Excellence "Physics of Life" TU Dresden: Marcelo Leomil Zoccoler
-All rights reserved.
-
-Redistribution and use in source and binary forms, with or without
-modification, are permitted provided that the following conditions are met:
-
-* Redistributions of source code must retain the above copyright notice, this
-  list of conditions and the following disclaimer.
-
-* Redistributions in binary form must reproduce the above copyright notice,
-  this list of conditions and the following disclaimer in the documentation
-  and/or other materials provided with the distribution.
-
-* Neither the name of copyright holder nor the names of its
-  contributors may be used to endorse or promote products derived from
-  this software without specific prior written permission.
-
-THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
-AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
-IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
-DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
-FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
-DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
-SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
-CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
-OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
-OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+
+Copyright (c) 2024, DFG Cluster of Excellence "Physics of Life" TU Dresden: Marcelo Leomil Zoccoler
+All rights reserved.
+
+Redistribution and use in source and binary forms, with or without
+modification, are permitted provided that the following conditions are met:
+
+* Redistributions of source code must retain the above copyright notice, this
+  list of conditions and the following disclaimer.
+
+* Redistributions in binary form must reproduce the above copyright notice,
+  this list of conditions and the following disclaimer in the documentation
+  and/or other materials provided with the distribution.
+
+* Neither the name of copyright holder nor the names of its
+  contributors may be used to endorse or promote products derived from
+  this software without specific prior written permission.
+
+THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
+AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
+IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
+DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
+FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
+DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
+SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
+CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
+OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
+OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
```

### Comparing `biaplotter-0.0.1/PKG-INFO` & `biaplotter-0.0.2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,134 +1,134 @@
-Metadata-Version: 2.1
-Name: biaplotter
-Version: 0.0.1
-Summary: A base napari plotter widget for interactive plotting
-Home-page: https://github.com/BiAPoL/biaplotter
-Author: Marcelo Leomil Zoccoler
-Author-email: marzoccoler@gmail.com
-License: BSD-3-Clause
-Project-URL: Bug Tracker, https://github.com/BiAPoL/biaplotter/issues
-Project-URL: Documentation, https://github.com/BiAPoL/biaplotter#README.md
-Project-URL: Source Code, https://github.com/BiAPoL/biaplotter
-Project-URL: User Support, https://github.com/BiAPoL/biaplotter/issues
-Classifier: Development Status :: 2 - Pre-Alpha
-Classifier: Framework :: napari
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: BSD License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Topic :: Scientific/Engineering :: Image Processing
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: numpy
-Requires-Dist: magicgui
-Requires-Dist: qtpy
-Requires-Dist: napari-matplotlib
-Requires-Dist: nap-plot-tools>=0.1.0
-Provides-Extra: testing
-Requires-Dist: tox; extra == "testing"
-Requires-Dist: pytest; extra == "testing"
-Requires-Dist: pytest-cov; extra == "testing"
-Requires-Dist: pytest-qt; extra == "testing"
-Requires-Dist: napari; extra == "testing"
-Requires-Dist: pyqt5; extra == "testing"
-
-# biaplotter
-
-[![License BSD-3](https://img.shields.io/pypi/l/biaplotter.svg?color=green)](https://github.com/BiAPoL/biaplotter/raw/main/LICENSE)
-[![PyPI](https://img.shields.io/pypi/v/biaplotter.svg?color=green)](https://pypi.org/project/biaplotter)
-[![Python Version](https://img.shields.io/pypi/pyversions/biaplotter.svg?color=green)](https://python.org)
-[![tests](https://github.com/BiAPoL/biaplotter/workflows/tests/badge.svg)](https://github.com/BiAPoL/biaplotter/actions)
-[![codecov](https://codecov.io/gh/BiAPoL/biaplotter/branch/main/graph/badge.svg)](https://codecov.io/gh/BiAPoL/biaplotter)
-[![napari hub](https://img.shields.io/endpoint?url=https://api.napari-hub.org/shields/biaplotter)](https://napari-hub.org/plugins/biaplotter)
-
-A base napari plotter widget for interactive plotting
-
-----------------------------------
-
-This [napari] plugin was generated with [Cookiecutter] using [@napari]'s [cookiecutter-napari-plugin] template.
-
-<!--
-Don't miss the full getting started guide to set up your new package:
-https://github.com/napari/cookiecutter-napari-plugin#getting-started
-
-and review the napari docs for plugin developers:
-https://napari.org/stable/plugins/index.html
--->
-
-## Documentation
-
-The full documentation with API and examples can be found [here](https://biapol.github.io/biaplotter/).
-
-## Installation
-
-* Make sure you have Python in your computer, e.g. download [miniforge](https://github.com/conda-forge/miniforge?tab=readme-ov-file#download).
-
-* Create a new environment, for example, like this:
-
-```
-mamba create --name biaplotter-env python=3.9
-```
-
-If you never used mamba/conda environments before, take a look at [this blog post](https://biapol.github.io/blog/mara_lampert/getting_started_with_mambaforge_and_python/readme.html).
-
-* **Activate** the new environment with `mamba`:
-
-```
-mamba activate biaplotter-env
-```
-
-* Install [napari](https://napari.org/stable/), e.g. via `mamba`:
-
-```
-mamba install -c conda-forge napari pyqt
-```
-
-Afterwards, install `biaplotter` via `pip`:
-
-```
-pip install biaplotter
-```
-
-To install latest development version :
-
-```
-pip install git+https://github.com/BiAPoL/biaplotter.git
-```
-
-
-## Contributing
-
-Contributions are very welcome. Tests can be run with [tox], please ensure
-the coverage at least stays the same before you submit a pull request.
-
-## License
-
-Distributed under the terms of the [BSD-3] license,
-"biaplotter" is free and open source software
-
-## Issues
-
-If you encounter any problems, please [file an issue] along with a detailed description.
-
-[napari]: https://github.com/napari/napari
-[Cookiecutter]: https://github.com/audreyr/cookiecutter
-[@napari]: https://github.com/napari
-[MIT]: http://opensource.org/licenses/MIT
-[BSD-3]: http://opensource.org/licenses/BSD-3-Clause
-[GNU GPL v3.0]: http://www.gnu.org/licenses/gpl-3.0.txt
-[GNU LGPL v3.0]: http://www.gnu.org/licenses/lgpl-3.0.txt
-[Apache Software License 2.0]: http://www.apache.org/licenses/LICENSE-2.0
-[Mozilla Public License 2.0]: https://www.mozilla.org/media/MPL/2.0/index.txt
-[cookiecutter-napari-plugin]: https://github.com/napari/cookiecutter-napari-plugin
-
-[file an issue]: https://github.com/BiAPoL/biaplotter/issues
-
-[napari]: https://github.com/napari/napari
-[tox]: https://tox.readthedocs.io/en/latest/
-[pip]: https://pypi.org/project/pip/
-[PyPI]: https://pypi.org/
+Metadata-Version: 2.1
+Name: biaplotter
+Version: 0.0.2
+Summary: A base napari plotter widget for interactive plotting
+Home-page: https://github.com/BiAPoL/biaplotter
+Author: Marcelo Leomil Zoccoler
+Author-email: marzoccoler@gmail.com
+License: BSD-3-Clause
+Project-URL: Bug Tracker, https://github.com/BiAPoL/biaplotter/issues
+Project-URL: Documentation, https://github.com/BiAPoL/biaplotter#README.md
+Project-URL: Source Code, https://github.com/BiAPoL/biaplotter
+Project-URL: User Support, https://github.com/BiAPoL/biaplotter/issues
+Classifier: Development Status :: 2 - Pre-Alpha
+Classifier: Framework :: napari
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: BSD License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Topic :: Scientific/Engineering :: Image Processing
+Requires-Python: >=3.9
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: numpy
+Requires-Dist: magicgui
+Requires-Dist: qtpy
+Requires-Dist: napari-matplotlib
+Requires-Dist: nap-plot-tools>=0.1.0
+Provides-Extra: testing
+Requires-Dist: tox; extra == "testing"
+Requires-Dist: pytest; extra == "testing"
+Requires-Dist: pytest-cov; extra == "testing"
+Requires-Dist: pytest-qt; extra == "testing"
+Requires-Dist: napari; extra == "testing"
+Requires-Dist: pyqt5; extra == "testing"
+
+# biaplotter
+
+[![License BSD-3](https://img.shields.io/pypi/l/biaplotter.svg?color=green)](https://github.com/BiAPoL/biaplotter/raw/main/LICENSE)
+[![PyPI](https://img.shields.io/pypi/v/biaplotter.svg?color=green)](https://pypi.org/project/biaplotter)
+[![Python Version](https://img.shields.io/pypi/pyversions/biaplotter.svg?color=green)](https://python.org)
+[![tests](https://github.com/BiAPoL/biaplotter/workflows/tests/badge.svg)](https://github.com/BiAPoL/biaplotter/actions)
+[![codecov](https://codecov.io/gh/BiAPoL/biaplotter/branch/main/graph/badge.svg)](https://codecov.io/gh/BiAPoL/biaplotter)
+[![napari hub](https://img.shields.io/endpoint?url=https://api.napari-hub.org/shields/biaplotter)](https://napari-hub.org/plugins/biaplotter)
+
+A base napari plotter widget for interactive plotting
+
+----------------------------------
+
+This [napari] plugin was generated with [Cookiecutter] using [@napari]'s [cookiecutter-napari-plugin] template.
+
+<!--
+Don't miss the full getting started guide to set up your new package:
+https://github.com/napari/cookiecutter-napari-plugin#getting-started
+
+and review the napari docs for plugin developers:
+https://napari.org/stable/plugins/index.html
+-->
+
+## Documentation
+
+The full documentation with API and examples can be found [here](https://biapol.github.io/biaplotter/).
+
+## Installation
+
+* Make sure you have Python in your computer, e.g. download [miniforge](https://github.com/conda-forge/miniforge?tab=readme-ov-file#download).
+
+* Create a new environment, for example, like this:
+
+```
+mamba create --name biaplotter-env python=3.9
+```
+
+If you never used mamba/conda environments before, take a look at [this blog post](https://biapol.github.io/blog/mara_lampert/getting_started_with_mambaforge_and_python/readme.html).
+
+* **Activate** the new environment with `mamba`:
+
+```
+mamba activate biaplotter-env
+```
+
+* Install [napari](https://napari.org/stable/), e.g. via `mamba`:
+
+```
+mamba install -c conda-forge napari pyqt
+```
+
+Afterwards, install `biaplotter` via `pip`:
+
+```
+pip install biaplotter
+```
+
+To install latest development version :
+
+```
+pip install git+https://github.com/BiAPoL/biaplotter.git
+```
+
+
+## Contributing
+
+Contributions are very welcome. Tests can be run with [tox], please ensure
+the coverage at least stays the same before you submit a pull request.
+
+## License
+
+Distributed under the terms of the [BSD-3] license,
+"biaplotter" is free and open source software
+
+## Issues
+
+If you encounter any problems, please [file an issue] along with a detailed description.
+
+[napari]: https://github.com/napari/napari
+[Cookiecutter]: https://github.com/audreyr/cookiecutter
+[@napari]: https://github.com/napari
+[MIT]: http://opensource.org/licenses/MIT
+[BSD-3]: http://opensource.org/licenses/BSD-3-Clause
+[GNU GPL v3.0]: http://www.gnu.org/licenses/gpl-3.0.txt
+[GNU LGPL v3.0]: http://www.gnu.org/licenses/lgpl-3.0.txt
+[Apache Software License 2.0]: http://www.apache.org/licenses/LICENSE-2.0
+[Mozilla Public License 2.0]: https://www.mozilla.org/media/MPL/2.0/index.txt
+[cookiecutter-napari-plugin]: https://github.com/napari/cookiecutter-napari-plugin
+
+[file an issue]: https://github.com/BiAPoL/biaplotter/issues
+
+[napari]: https://github.com/napari/napari
+[tox]: https://tox.readthedocs.io/en/latest/
+[pip]: https://pypi.org/project/pip/
+[PyPI]: https://pypi.org/
```

### Comparing `biaplotter-0.0.1/README.md` & `biaplotter-0.0.2/README.md`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,95 +1,95 @@
-# biaplotter
-
-[![License BSD-3](https://img.shields.io/pypi/l/biaplotter.svg?color=green)](https://github.com/BiAPoL/biaplotter/raw/main/LICENSE)
-[![PyPI](https://img.shields.io/pypi/v/biaplotter.svg?color=green)](https://pypi.org/project/biaplotter)
-[![Python Version](https://img.shields.io/pypi/pyversions/biaplotter.svg?color=green)](https://python.org)
-[![tests](https://github.com/BiAPoL/biaplotter/workflows/tests/badge.svg)](https://github.com/BiAPoL/biaplotter/actions)
-[![codecov](https://codecov.io/gh/BiAPoL/biaplotter/branch/main/graph/badge.svg)](https://codecov.io/gh/BiAPoL/biaplotter)
-[![napari hub](https://img.shields.io/endpoint?url=https://api.napari-hub.org/shields/biaplotter)](https://napari-hub.org/plugins/biaplotter)
-
-A base napari plotter widget for interactive plotting
-
-----------------------------------
-
-This [napari] plugin was generated with [Cookiecutter] using [@napari]'s [cookiecutter-napari-plugin] template.
-
-<!--
-Don't miss the full getting started guide to set up your new package:
-https://github.com/napari/cookiecutter-napari-plugin#getting-started
-
-and review the napari docs for plugin developers:
-https://napari.org/stable/plugins/index.html
--->
-
-## Documentation
-
-The full documentation with API and examples can be found [here](https://biapol.github.io/biaplotter/).
-
-## Installation
-
-* Make sure you have Python in your computer, e.g. download [miniforge](https://github.com/conda-forge/miniforge?tab=readme-ov-file#download).
-
-* Create a new environment, for example, like this:
-
-```
-mamba create --name biaplotter-env python=3.9
-```
-
-If you never used mamba/conda environments before, take a look at [this blog post](https://biapol.github.io/blog/mara_lampert/getting_started_with_mambaforge_and_python/readme.html).
-
-* **Activate** the new environment with `mamba`:
-
-```
-mamba activate biaplotter-env
-```
-
-* Install [napari](https://napari.org/stable/), e.g. via `mamba`:
-
-```
-mamba install -c conda-forge napari pyqt
-```
-
-Afterwards, install `biaplotter` via `pip`:
-
-```
-pip install biaplotter
-```
-
-To install latest development version :
-
-```
-pip install git+https://github.com/BiAPoL/biaplotter.git
-```
-
-
-## Contributing
-
-Contributions are very welcome. Tests can be run with [tox], please ensure
-the coverage at least stays the same before you submit a pull request.
-
-## License
-
-Distributed under the terms of the [BSD-3] license,
-"biaplotter" is free and open source software
-
-## Issues
-
-If you encounter any problems, please [file an issue] along with a detailed description.
-
-[napari]: https://github.com/napari/napari
-[Cookiecutter]: https://github.com/audreyr/cookiecutter
-[@napari]: https://github.com/napari
-[MIT]: http://opensource.org/licenses/MIT
-[BSD-3]: http://opensource.org/licenses/BSD-3-Clause
-[GNU GPL v3.0]: http://www.gnu.org/licenses/gpl-3.0.txt
-[GNU LGPL v3.0]: http://www.gnu.org/licenses/lgpl-3.0.txt
-[Apache Software License 2.0]: http://www.apache.org/licenses/LICENSE-2.0
-[Mozilla Public License 2.0]: https://www.mozilla.org/media/MPL/2.0/index.txt
-[cookiecutter-napari-plugin]: https://github.com/napari/cookiecutter-napari-plugin
-
-[file an issue]: https://github.com/BiAPoL/biaplotter/issues
-
-[napari]: https://github.com/napari/napari
-[tox]: https://tox.readthedocs.io/en/latest/
-[pip]: https://pypi.org/project/pip/
-[PyPI]: https://pypi.org/
+# biaplotter
+
+[![License BSD-3](https://img.shields.io/pypi/l/biaplotter.svg?color=green)](https://github.com/BiAPoL/biaplotter/raw/main/LICENSE)
+[![PyPI](https://img.shields.io/pypi/v/biaplotter.svg?color=green)](https://pypi.org/project/biaplotter)
+[![Python Version](https://img.shields.io/pypi/pyversions/biaplotter.svg?color=green)](https://python.org)
+[![tests](https://github.com/BiAPoL/biaplotter/workflows/tests/badge.svg)](https://github.com/BiAPoL/biaplotter/actions)
+[![codecov](https://codecov.io/gh/BiAPoL/biaplotter/branch/main/graph/badge.svg)](https://codecov.io/gh/BiAPoL/biaplotter)
+[![napari hub](https://img.shields.io/endpoint?url=https://api.napari-hub.org/shields/biaplotter)](https://napari-hub.org/plugins/biaplotter)
+
+A base napari plotter widget for interactive plotting
+
+----------------------------------
+
+This [napari] plugin was generated with [Cookiecutter] using [@napari]'s [cookiecutter-napari-plugin] template.
+
+<!--
+Don't miss the full getting started guide to set up your new package:
+https://github.com/napari/cookiecutter-napari-plugin#getting-started
+
+and review the napari docs for plugin developers:
+https://napari.org/stable/plugins/index.html
+-->
+
+## Documentation
+
+The full documentation with API and examples can be found [here](https://biapol.github.io/biaplotter/).
+
+## Installation
+
+* Make sure you have Python in your computer, e.g. download [miniforge](https://github.com/conda-forge/miniforge?tab=readme-ov-file#download).
+
+* Create a new environment, for example, like this:
+
+```
+mamba create --name biaplotter-env python=3.9
+```
+
+If you never used mamba/conda environments before, take a look at [this blog post](https://biapol.github.io/blog/mara_lampert/getting_started_with_mambaforge_and_python/readme.html).
+
+* **Activate** the new environment with `mamba`:
+
+```
+mamba activate biaplotter-env
+```
+
+* Install [napari](https://napari.org/stable/), e.g. via `mamba`:
+
+```
+mamba install -c conda-forge napari pyqt
+```
+
+Afterwards, install `biaplotter` via `pip`:
+
+```
+pip install biaplotter
+```
+
+To install latest development version :
+
+```
+pip install git+https://github.com/BiAPoL/biaplotter.git
+```
+
+
+## Contributing
+
+Contributions are very welcome. Tests can be run with [tox], please ensure
+the coverage at least stays the same before you submit a pull request.
+
+## License
+
+Distributed under the terms of the [BSD-3] license,
+"biaplotter" is free and open source software
+
+## Issues
+
+If you encounter any problems, please [file an issue] along with a detailed description.
+
+[napari]: https://github.com/napari/napari
+[Cookiecutter]: https://github.com/audreyr/cookiecutter
+[@napari]: https://github.com/napari
+[MIT]: http://opensource.org/licenses/MIT
+[BSD-3]: http://opensource.org/licenses/BSD-3-Clause
+[GNU GPL v3.0]: http://www.gnu.org/licenses/gpl-3.0.txt
+[GNU LGPL v3.0]: http://www.gnu.org/licenses/lgpl-3.0.txt
+[Apache Software License 2.0]: http://www.apache.org/licenses/LICENSE-2.0
+[Mozilla Public License 2.0]: https://www.mozilla.org/media/MPL/2.0/index.txt
+[cookiecutter-napari-plugin]: https://github.com/napari/cookiecutter-napari-plugin
+
+[file an issue]: https://github.com/BiAPoL/biaplotter/issues
+
+[napari]: https://github.com/napari/napari
+[tox]: https://tox.readthedocs.io/en/latest/
+[pip]: https://pypi.org/project/pip/
+[PyPI]: https://pypi.org/
```

### Comparing `biaplotter-0.0.1/pyproject.toml` & `biaplotter-0.0.2/pyproject.toml`

 * *Ordering differences only*

 * *Files 27% similar despite different names*

```diff
@@ -1,56 +1,56 @@
-[build-system]
-requires = ["setuptools>=42.0.0", "wheel"]
-build-backend = "setuptools.build_meta"
-
-
-
-[tool.black]
-line-length = 79
-target-version = ['py38', 'py39', 'py310']
-
-
-[tool.ruff]
-line-length = 79
-lint.select = [
-    "E", "F", "W", #flake8
-    "UP", # pyupgrade
-    "I", # isort
-    "BLE", # flake8-blind-exception
-    "B", # flake8-bugbear
-    "A", # flake8-builtins
-    "C4", # flake8-comprehensions
-    "ISC", # flake8-implicit-str-concat
-    "G", # flake8-logging-format
-    "PIE", # flake8-pie
-    "SIM", # flake8-simplify
-]
-lint.ignore = [
-    "E501", # line too long. let black handle this
-    "UP006", "UP007", # type annotation. As using magicgui require runtime type annotation then we disable this.
-    "SIM117", # flake8-simplify - some of merged with statements are not looking great with black, reanble after drop python 3.9
-]
-
-exclude = [
-    ".bzr",
-    ".direnv",
-    ".eggs",
-    ".git",
-    ".mypy_cache",
-    ".pants.d",
-    ".ruff_cache",
-    ".svn",
-    ".tox",
-    ".venv",
-    "__pypackages__",
-    "_build",
-    "buck-out",
-    "build",
-    "dist",
-    "node_modules",
-    "venv",
-    "*vendored*",
-    "*_vendor*",
-]
-
-target-version = "py39"
-fix = true
+[build-system]
+requires = ["setuptools>=42.0.0", "wheel"]
+build-backend = "setuptools.build_meta"
+
+
+
+[tool.black]
+line-length = 79
+target-version = ['py38', 'py39', 'py310']
+
+
+[tool.ruff]
+line-length = 79
+lint.select = [
+    "E", "F", "W", #flake8
+    "UP", # pyupgrade
+    "I", # isort
+    "BLE", # flake8-blind-exception
+    "B", # flake8-bugbear
+    "A", # flake8-builtins
+    "C4", # flake8-comprehensions
+    "ISC", # flake8-implicit-str-concat
+    "G", # flake8-logging-format
+    "PIE", # flake8-pie
+    "SIM", # flake8-simplify
+]
+lint.ignore = [
+    "E501", # line too long. let black handle this
+    "UP006", "UP007", # type annotation. As using magicgui require runtime type annotation then we disable this.
+    "SIM117", # flake8-simplify - some of merged with statements are not looking great with black, reanble after drop python 3.9
+]
+
+exclude = [
+    ".bzr",
+    ".direnv",
+    ".eggs",
+    ".git",
+    ".mypy_cache",
+    ".pants.d",
+    ".ruff_cache",
+    ".svn",
+    ".tox",
+    ".venv",
+    "__pypackages__",
+    "_build",
+    "buck-out",
+    "build",
+    "dist",
+    "node_modules",
+    "venv",
+    "*vendored*",
+    "*_vendor*",
+]
+
+target-version = "py39"
+fix = true
```

### Comparing `biaplotter-0.0.1/setup.cfg` & `biaplotter-0.0.2/setup.cfg`

 * *Files 14% similar despite different names*

```diff
@@ -1,109 +1,105 @@
-00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
-00000010: 203d 2062 6961 706c 6f74 7465 720d 0a76   = biaplotter..v
-00000020: 6572 7369 6f6e 203d 2061 7474 723a 2062  ersion = attr: b
-00000030: 6961 706c 6f74 7465 722e 5f5f 7665 7273  iaplotter.__vers
-00000040: 696f 6e5f 5f0d 0a64 6573 6372 6970 7469  ion__..descripti
-00000050: 6f6e 203d 2041 2062 6173 6520 6e61 7061  on = A base napa
-00000060: 7269 2070 6c6f 7474 6572 2077 6964 6765  ri plotter widge
-00000070: 7420 666f 7220 696e 7465 7261 6374 6976  t for interactiv
-00000080: 6520 706c 6f74 7469 6e67 0d0a 6c6f 6e67  e plotting..long
-00000090: 5f64 6573 6372 6970 7469 6f6e 203d 2066  _description = f
-000000a0: 696c 653a 2052 4541 444d 452e 6d64 0d0a  ile: README.md..
-000000b0: 6c6f 6e67 5f64 6573 6372 6970 7469 6f6e  long_description
-000000c0: 5f63 6f6e 7465 6e74 5f74 7970 6520 3d20  _content_type = 
-000000d0: 7465 7874 2f6d 6172 6b64 6f77 6e0d 0a75  text/markdown..u
-000000e0: 726c 203d 2068 7474 7073 3a2f 2f67 6974  rl = https://git
-000000f0: 6875 622e 636f 6d2f 4269 4150 6f4c 2f62  hub.com/BiAPoL/b
-00000100: 6961 706c 6f74 7465 720d 0a61 7574 686f  iaplotter..autho
-00000110: 7220 3d20 4d61 7263 656c 6f20 4c65 6f6d  r = Marcelo Leom
-00000120: 696c 205a 6f63 636f 6c65 720d 0a61 7574  il Zoccoler..aut
-00000130: 686f 725f 656d 6169 6c20 3d20 6d61 727a  hor_email = marz
-00000140: 6f63 636f 6c65 7240 676d 6169 6c2e 636f  occoler@gmail.co
-00000150: 6d0d 0a6c 6963 656e 7365 203d 2042 5344  m..license = BSD
-00000160: 2d33 2d43 6c61 7573 650d 0a6c 6963 656e  -3-Clause..licen
-00000170: 7365 5f66 696c 6573 203d 204c 4943 454e  se_files = LICEN
-00000180: 5345 0d0a 636c 6173 7369 6669 6572 7320  SE..classifiers 
-00000190: 3d20 0d0a 0944 6576 656c 6f70 6d65 6e74  = ...Development
-000001a0: 2053 7461 7475 7320 3a3a 2032 202d 2050   Status :: 2 - P
-000001b0: 7265 2d41 6c70 6861 0d0a 0946 7261 6d65  re-Alpha...Frame
-000001c0: 776f 726b 203a 3a20 6e61 7061 7269 0d0a  work :: napari..
-000001d0: 0949 6e74 656e 6465 6420 4175 6469 656e  .Intended Audien
-000001e0: 6365 203a 3a20 4465 7665 6c6f 7065 7273  ce :: Developers
-000001f0: 0d0a 094c 6963 656e 7365 203a 3a20 4f53  ...License :: OS
-00000200: 4920 4170 7072 6f76 6564 203a 3a20 4253  I Approved :: BS
-00000210: 4420 4c69 6365 6e73 650d 0a09 4f70 6572  D License...Oper
-00000220: 6174 696e 6720 5379 7374 656d 203a 3a20  ating System :: 
-00000230: 4f53 2049 6e64 6570 656e 6465 6e74 0d0a  OS Independent..
-00000240: 0950 726f 6772 616d 6d69 6e67 204c 616e  .Programming Lan
-00000250: 6775 6167 6520 3a3a 2050 7974 686f 6e0d  guage :: Python.
-00000260: 0a09 5072 6f67 7261 6d6d 696e 6720 4c61  ..Programming La
-00000270: 6e67 7561 6765 203a 3a20 5079 7468 6f6e  nguage :: Python
-00000280: 203a 3a20 330d 0a09 5072 6f67 7261 6d6d   :: 3...Programm
-00000290: 696e 6720 4c61 6e67 7561 6765 203a 3a20  ing Language :: 
-000002a0: 5079 7468 6f6e 203a 3a20 3320 3a3a 204f  Python :: 3 :: O
-000002b0: 6e6c 790d 0a09 5072 6f67 7261 6d6d 696e  nly...Programmin
-000002c0: 6720 4c61 6e67 7561 6765 203a 3a20 5079  g Language :: Py
-000002d0: 7468 6f6e 203a 3a20 332e 390d 0a09 5072  thon :: 3.9...Pr
-000002e0: 6f67 7261 6d6d 696e 6720 4c61 6e67 7561  ogramming Langua
-000002f0: 6765 203a 3a20 5079 7468 6f6e 203a 3a20  ge :: Python :: 
-00000300: 332e 3130 0d0a 0954 6f70 6963 203a 3a20  3.10...Topic :: 
-00000310: 5363 6965 6e74 6966 6963 2f45 6e67 696e  Scientific/Engin
-00000320: 6565 7269 6e67 203a 3a20 496d 6167 6520  eering :: Image 
-00000330: 5072 6f63 6573 7369 6e67 0d0a 7072 6f6a  Processing..proj
-00000340: 6563 745f 7572 6c73 203d 200d 0a09 4275  ect_urls = ...Bu
-00000350: 6720 5472 6163 6b65 7220 3d20 6874 7470  g Tracker = http
-00000360: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f42  s://github.com/B
-00000370: 6941 506f 4c2f 6269 6170 6c6f 7474 6572  iAPoL/biaplotter
-00000380: 2f69 7373 7565 730d 0a09 446f 6375 6d65  /issues...Docume
-00000390: 6e74 6174 696f 6e20 3d20 6874 7470 733a  ntation = https:
-000003a0: 2f2f 6769 7468 7562 2e63 6f6d 2f42 6941  //github.com/BiA
-000003b0: 506f 4c2f 6269 6170 6c6f 7474 6572 2352  PoL/biaplotter#R
-000003c0: 4541 444d 452e 6d64 0d0a 0953 6f75 7263  EADME.md...Sourc
-000003d0: 6520 436f 6465 203d 2068 7474 7073 3a2f  e Code = https:/
-000003e0: 2f67 6974 6875 622e 636f 6d2f 4269 4150  /github.com/BiAP
-000003f0: 6f4c 2f62 6961 706c 6f74 7465 720d 0a09  oL/biaplotter...
-00000400: 5573 6572 2053 7570 706f 7274 203d 2068  User Support = h
-00000410: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-00000420: 6d2f 4269 4150 6f4c 2f62 6961 706c 6f74  m/BiAPoL/biaplot
-00000430: 7465 722f 6973 7375 6573 0d0a 0d0a 5b6f  ter/issues....[o
-00000440: 7074 696f 6e73 5d0d 0a70 6163 6b61 6765  ptions]..package
-00000450: 7320 3d20 6669 6e64 3a0d 0a69 6e73 7461  s = find:..insta
-00000460: 6c6c 5f72 6571 7569 7265 7320 3d20 0d0a  ll_requires = ..
-00000470: 096e 756d 7079 0d0a 096d 6167 6963 6775  .numpy...magicgu
-00000480: 690d 0a09 7174 7079 0d0a 096e 6170 6172  i...qtpy...napar
-00000490: 692d 6d61 7470 6c6f 746c 6962 0d0a 096e  i-matplotlib...n
-000004a0: 6170 2d70 6c6f 742d 746f 6f6c 733e 3d30  ap-plot-tools>=0
-000004b0: 2e31 2e30 0d0a 7079 7468 6f6e 5f72 6571  .1.0..python_req
-000004c0: 7569 7265 7320 3d20 3e3d 332e 390d 0a69  uires = >=3.9..i
-000004d0: 6e63 6c75 6465 5f70 6163 6b61 6765 5f64  nclude_package_d
-000004e0: 6174 6120 3d20 5472 7565 0d0a 7061 636b  ata = True..pack
-000004f0: 6167 655f 6469 7220 3d20 0d0a 093d 7372  age_dir = ...=sr
-00000500: 630d 0a0d 0a5b 6f70 7469 6f6e 732e 7061  c....[options.pa
-00000510: 636b 6167 6573 2e66 696e 645d 0d0a 7768  ckages.find]..wh
-00000520: 6572 6520 3d20 7372 630d 0a0d 0a5b 6f70  ere = src....[op
-00000530: 7469 6f6e 732e 656e 7472 795f 706f 696e  tions.entry_poin
-00000540: 7473 5d0d 0a6e 6170 6172 692e 6d61 6e69  ts]..napari.mani
-00000550: 6665 7374 203d 200d 0a09 6269 6170 6c6f  fest = ...biaplo
-00000560: 7474 6572 203d 2062 6961 706c 6f74 7465  tter = biaplotte
-00000570: 723a 6e61 7061 7269 2e79 616d 6c0d 0a0d  r:napari.yaml...
-00000580: 0a5b 6f70 7469 6f6e 732e 6578 7472 6173  .[options.extras
-00000590: 5f72 6571 7569 7265 5d0d 0a74 6573 7469  _require]..testi
-000005a0: 6e67 203d 200d 0a09 746f 780d 0a09 7079  ng = ...tox...py
-000005b0: 7465 7374 2020 2320 6874 7470 733a 2f2f  test  # https://
-000005c0: 646f 6373 2e70 7974 6573 742e 6f72 672f  docs.pytest.org/
-000005d0: 656e 2f6c 6174 6573 742f 636f 6e74 656e  en/latest/conten
-000005e0: 7473 2e68 746d 6c0d 0a09 7079 7465 7374  ts.html...pytest
-000005f0: 2d63 6f76 2020 2320 6874 7470 733a 2f2f  -cov  # https://
-00000600: 7079 7465 7374 2d63 6f76 2e72 6561 6474  pytest-cov.readt
-00000610: 6865 646f 6373 2e69 6f2f 656e 2f6c 6174  hedocs.io/en/lat
-00000620: 6573 742f 0d0a 0970 7974 6573 742d 7174  est/...pytest-qt
-00000630: 2020 2320 6874 7470 733a 2f2f 7079 7465    # https://pyte
-00000640: 7374 2d71 742e 7265 6164 7468 6564 6f63  st-qt.readthedoc
-00000650: 732e 696f 2f65 6e2f 6c61 7465 7374 2f0d  s.io/en/latest/.
-00000660: 0a09 6e61 7061 7269 0d0a 0970 7971 7435  ..napari...pyqt5
-00000670: 0d0a 0d0a 5b6f 7074 696f 6e73 2e70 6163  ....[options.pac
-00000680: 6b61 6765 5f64 6174 615d 0d0a 2a20 3d20  kage_data]..* = 
-00000690: 2a2e 7961 6d6c 0d0a 0d0a 5b65 6767 5f69  *.yaml....[egg_i
-000006a0: 6e66 6f5d 0d0a 7461 675f 6275 696c 6420  nfo]..tag_build 
-000006b0: 3d20 0d0a 7461 675f 6461 7465 203d 2030  = ..tag_date = 0
-000006c0: 0d0a 0d0a                                ....
+00000000: 5b6d 6574 6164 6174 615d 0a6e 616d 6520  [metadata].name 
+00000010: 3d20 6269 6170 6c6f 7474 6572 0a76 6572  = biaplotter.ver
+00000020: 7369 6f6e 203d 2061 7474 723a 2062 6961  sion = attr: bia
+00000030: 706c 6f74 7465 722e 5f5f 7665 7273 696f  plotter.__versio
+00000040: 6e5f 5f0a 6465 7363 7269 7074 696f 6e20  n__.description 
+00000050: 3d20 4120 6261 7365 206e 6170 6172 6920  = A base napari 
+00000060: 706c 6f74 7465 7220 7769 6467 6574 2066  plotter widget f
+00000070: 6f72 2069 6e74 6572 6163 7469 7665 2070  or interactive p
+00000080: 6c6f 7474 696e 670a 6c6f 6e67 5f64 6573  lotting.long_des
+00000090: 6372 6970 7469 6f6e 203d 2066 696c 653a  cription = file:
+000000a0: 2052 4541 444d 452e 6d64 0a6c 6f6e 675f   README.md.long_
+000000b0: 6465 7363 7269 7074 696f 6e5f 636f 6e74  description_cont
+000000c0: 656e 745f 7479 7065 203d 2074 6578 742f  ent_type = text/
+000000d0: 6d61 726b 646f 776e 0a75 726c 203d 2068  markdown.url = h
+000000e0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+000000f0: 6d2f 4269 4150 6f4c 2f62 6961 706c 6f74  m/BiAPoL/biaplot
+00000100: 7465 720a 6175 7468 6f72 203d 204d 6172  ter.author = Mar
+00000110: 6365 6c6f 204c 656f 6d69 6c20 5a6f 6363  celo Leomil Zocc
+00000120: 6f6c 6572 0a61 7574 686f 725f 656d 6169  oler.author_emai
+00000130: 6c20 3d20 6d61 727a 6f63 636f 6c65 7240  l = marzoccoler@
+00000140: 676d 6169 6c2e 636f 6d0a 6c69 6365 6e73  gmail.com.licens
+00000150: 6520 3d20 4253 442d 332d 436c 6175 7365  e = BSD-3-Clause
+00000160: 0a6c 6963 656e 7365 5f66 696c 6573 203d  .license_files =
+00000170: 204c 4943 454e 5345 0a63 6c61 7373 6966   LICENSE.classif
+00000180: 6965 7273 203d 200a 0944 6576 656c 6f70  iers = ..Develop
+00000190: 6d65 6e74 2053 7461 7475 7320 3a3a 2032  ment Status :: 2
+000001a0: 202d 2050 7265 2d41 6c70 6861 0a09 4672   - Pre-Alpha..Fr
+000001b0: 616d 6577 6f72 6b20 3a3a 206e 6170 6172  amework :: napar
+000001c0: 690a 0949 6e74 656e 6465 6420 4175 6469  i..Intended Audi
+000001d0: 656e 6365 203a 3a20 4465 7665 6c6f 7065  ence :: Develope
+000001e0: 7273 0a09 4c69 6365 6e73 6520 3a3a 204f  rs..License :: O
+000001f0: 5349 2041 7070 726f 7665 6420 3a3a 2042  SI Approved :: B
+00000200: 5344 204c 6963 656e 7365 0a09 4f70 6572  SD License..Oper
+00000210: 6174 696e 6720 5379 7374 656d 203a 3a20  ating System :: 
+00000220: 4f53 2049 6e64 6570 656e 6465 6e74 0a09  OS Independent..
+00000230: 5072 6f67 7261 6d6d 696e 6720 4c61 6e67  Programming Lang
+00000240: 7561 6765 203a 3a20 5079 7468 6f6e 0a09  uage :: Python..
+00000250: 5072 6f67 7261 6d6d 696e 6720 4c61 6e67  Programming Lang
+00000260: 7561 6765 203a 3a20 5079 7468 6f6e 203a  uage :: Python :
+00000270: 3a20 330a 0950 726f 6772 616d 6d69 6e67  : 3..Programming
+00000280: 204c 616e 6775 6167 6520 3a3a 2050 7974   Language :: Pyt
+00000290: 686f 6e20 3a3a 2033 203a 3a20 4f6e 6c79  hon :: 3 :: Only
+000002a0: 0a09 5072 6f67 7261 6d6d 696e 6720 4c61  ..Programming La
+000002b0: 6e67 7561 6765 203a 3a20 5079 7468 6f6e  nguage :: Python
+000002c0: 203a 3a20 332e 390a 0950 726f 6772 616d   :: 3.9..Program
+000002d0: 6d69 6e67 204c 616e 6775 6167 6520 3a3a  ming Language ::
+000002e0: 2050 7974 686f 6e20 3a3a 2033 2e31 300a   Python :: 3.10.
+000002f0: 0954 6f70 6963 203a 3a20 5363 6965 6e74  .Topic :: Scient
+00000300: 6966 6963 2f45 6e67 696e 6565 7269 6e67  ific/Engineering
+00000310: 203a 3a20 496d 6167 6520 5072 6f63 6573   :: Image Proces
+00000320: 7369 6e67 0a70 726f 6a65 6374 5f75 726c  sing.project_url
+00000330: 7320 3d20 0a09 4275 6720 5472 6163 6b65  s = ..Bug Tracke
+00000340: 7220 3d20 6874 7470 733a 2f2f 6769 7468  r = https://gith
+00000350: 7562 2e63 6f6d 2f42 6941 506f 4c2f 6269  ub.com/BiAPoL/bi
+00000360: 6170 6c6f 7474 6572 2f69 7373 7565 730a  aplotter/issues.
+00000370: 0944 6f63 756d 656e 7461 7469 6f6e 203d  .Documentation =
+00000380: 2068 7474 7073 3a2f 2f67 6974 6875 622e   https://github.
+00000390: 636f 6d2f 4269 4150 6f4c 2f62 6961 706c  com/BiAPoL/biapl
+000003a0: 6f74 7465 7223 5245 4144 4d45 2e6d 640a  otter#README.md.
+000003b0: 0953 6f75 7263 6520 436f 6465 203d 2068  .Source Code = h
+000003c0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+000003d0: 6d2f 4269 4150 6f4c 2f62 6961 706c 6f74  m/BiAPoL/biaplot
+000003e0: 7465 720a 0955 7365 7220 5375 7070 6f72  ter..User Suppor
+000003f0: 7420 3d20 6874 7470 733a 2f2f 6769 7468  t = https://gith
+00000400: 7562 2e63 6f6d 2f42 6941 506f 4c2f 6269  ub.com/BiAPoL/bi
+00000410: 6170 6c6f 7474 6572 2f69 7373 7565 730a  aplotter/issues.
+00000420: 0a5b 6f70 7469 6f6e 735d 0a70 6163 6b61  .[options].packa
+00000430: 6765 7320 3d20 6669 6e64 3a0a 696e 7374  ges = find:.inst
+00000440: 616c 6c5f 7265 7175 6972 6573 203d 200a  all_requires = .
+00000450: 096e 756d 7079 0a09 6d61 6769 6367 7569  .numpy..magicgui
+00000460: 0a09 7174 7079 0a09 6e61 7061 7269 2d6d  ..qtpy..napari-m
+00000470: 6174 706c 6f74 6c69 620a 096e 6170 2d70  atplotlib..nap-p
+00000480: 6c6f 742d 746f 6f6c 733e 3d30 2e31 2e30  lot-tools>=0.1.0
+00000490: 0a70 7974 686f 6e5f 7265 7175 6972 6573  .python_requires
+000004a0: 203d 203e 3d33 2e39 0a69 6e63 6c75 6465   = >=3.9.include
+000004b0: 5f70 6163 6b61 6765 5f64 6174 6120 3d20  _package_data = 
+000004c0: 5472 7565 0a70 6163 6b61 6765 5f64 6972  True.package_dir
+000004d0: 203d 200a 093d 7372 630a 0a5b 6f70 7469   = ..=src..[opti
+000004e0: 6f6e 732e 7061 636b 6167 6573 2e66 696e  ons.packages.fin
+000004f0: 645d 0a77 6865 7265 203d 2073 7263 0a0a  d].where = src..
+00000500: 5b6f 7074 696f 6e73 2e65 6e74 7279 5f70  [options.entry_p
+00000510: 6f69 6e74 735d 0a6e 6170 6172 692e 6d61  oints].napari.ma
+00000520: 6e69 6665 7374 203d 200a 0962 6961 706c  nifest = ..biapl
+00000530: 6f74 7465 7220 3d20 6269 6170 6c6f 7474  otter = biaplott
+00000540: 6572 3a6e 6170 6172 692e 7961 6d6c 0a0a  er:napari.yaml..
+00000550: 5b6f 7074 696f 6e73 2e65 7874 7261 735f  [options.extras_
+00000560: 7265 7175 6972 655d 0a74 6573 7469 6e67  require].testing
+00000570: 203d 200a 0974 6f78 0a09 7079 7465 7374   = ..tox..pytest
+00000580: 2020 2320 6874 7470 733a 2f2f 646f 6373    # https://docs
+00000590: 2e70 7974 6573 742e 6f72 672f 656e 2f6c  .pytest.org/en/l
+000005a0: 6174 6573 742f 636f 6e74 656e 7473 2e68  atest/contents.h
+000005b0: 746d 6c0a 0970 7974 6573 742d 636f 7620  tml..pytest-cov 
+000005c0: 2023 2068 7474 7073 3a2f 2f70 7974 6573   # https://pytes
+000005d0: 742d 636f 762e 7265 6164 7468 6564 6f63  t-cov.readthedoc
+000005e0: 732e 696f 2f65 6e2f 6c61 7465 7374 2f0a  s.io/en/latest/.
+000005f0: 0970 7974 6573 742d 7174 2020 2320 6874  .pytest-qt  # ht
+00000600: 7470 733a 2f2f 7079 7465 7374 2d71 742e  tps://pytest-qt.
+00000610: 7265 6164 7468 6564 6f63 732e 696f 2f65  readthedocs.io/e
+00000620: 6e2f 6c61 7465 7374 2f0a 096e 6170 6172  n/latest/..napar
+00000630: 690a 0970 7971 7435 0a0a 5b6f 7074 696f  i..pyqt5..[optio
+00000640: 6e73 2e70 6163 6b61 6765 5f64 6174 615d  ns.package_data]
+00000650: 0a2a 203d 202a 2e79 616d 6c0a 0a5b 6567  .* = *.yaml..[eg
+00000660: 675f 696e 666f 5d0a 7461 675f 6275 696c  g_info].tag_buil
+00000670: 6420 3d20 0a74 6167 5f64 6174 6520 3d20  d = .tag_date = 
+00000680: 300a 0a                                  0..
```

### Comparing `biaplotter-0.0.1/src/biaplotter/_tests/test_artists.py` & `biaplotter-0.0.2/src/biaplotter/_tests/test_artists.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,103 +1,103 @@
-import numpy as np
-import matplotlib.pyplot as plt
-
-from biaplotter.artists import (
-    Scatter, Histogram2D
-)
-
-
-def test_scatter():
-    size = 100
-    data = np.random.rand(size, 2)
-    fig, ax = plt.subplots()
-    scatter = Scatter(ax)
-    # Test Scatter signals
-    collected_data_signals = []
-    def on_data_changed(data):
-        collected_data_signals.append(data)
-    scatter.data_changed_signal.connect(on_data_changed)
-    assert len(collected_data_signals) == 0
-    # Set data
-    scatter.data = data
-    assert len(collected_data_signals) == 1
-    assert np.all(collected_data_signals[0] == data)
-    collected_color_indices_signals = []
-    def on_color_indices_changed(color_indices):
-        collected_color_indices_signals.append(color_indices)
-    scatter.color_indices_changed_signal.connect(on_color_indices_changed)
-    assert len(collected_color_indices_signals) == 0
-    # Set color_indices with an array of increasing repeating integers from 0 to 5
-    scatter.color_indices = np.linspace(
-        start=0, stop=5, num=size, endpoint=False, dtype=int)
-    assert len(collected_color_indices_signals) == 1
-    assert np.all(collected_color_indices_signals[0] == scatter.color_indices)
-    scatter.visible = True
-
-    # Test Scatter properties
-    assert scatter.data.shape == (size, 2)
-    assert scatter.visible == True
-    assert scatter.color_indices.shape == (size,)
-    assert scatter.color_indices.dtype == int
-
-    # Test scatter colors
-    colors = scatter._scatter.get_facecolors()
-    assert np.all(colors[0] == scatter.categorical_colormap(0))
-    assert np.all(colors[50] == scatter.categorical_colormap(2))
-
-
-def test_histogram2d():
-    # Inputs
-    threshold = 20
-    size = 1000
-    bins = 20
-
-    # Expected output
-    indices_non_zero_overlay = (
-        np.array([8, 9, 10], dtype=int), np.array([8, 9, 7], dtype=int))
-
-    np.random.seed(42)
-
-    # Generate gaussian distribution 2d data
-    x = np.random.normal(loc=0, scale=1, size=size)
-    y = np.random.normal(loc=0, scale=1, size=size)
-    data = np.column_stack([x, y])
-    fig, ax = plt.subplots()
-    histogram = Histogram2D(ax)
-    # Test Histogram2D signals
-    collected_data_signals = []
-    def on_data_changed(data):
-        collected_data_signals.append(data)
-    histogram.data_changed_signal.connect(on_data_changed)
-    assert len(collected_data_signals) == 0
-    histogram.data = data
-    assert len(collected_data_signals) == 1
-    assert np.all(collected_data_signals[0] == data)
-    collected_color_indices_signals = []
-    def on_color_indices_changed(color_indices):
-        collected_color_indices_signals.append(color_indices)
-    histogram.color_indices_changed_signal.connect(on_color_indices_changed)
-    assert len(collected_color_indices_signals) == 0
-    # Set color indices of data in patches exceeding threshold to 1 (orange color)
-    indices = histogram.indices_in_above_threshold_patches(threshold=threshold)
-    color_indices = np.zeros(size)
-    color_indices[indices] = 1
-    histogram.color_indices = color_indices
-    assert len(collected_color_indices_signals) == 1
-    assert np.all(collected_color_indices_signals[0] == color_indices)
-
-    histogram.visible = True
-    histogram.bins = bins
-
-    # Test Histogram2D properties
-    assert histogram.data.shape == (size, 2)
-    assert histogram.visible == True
-    assert histogram.color_indices.shape == (size,)
-    assert histogram.color_indices.dtype == int
-    assert histogram.bins == bins
-
-    # Test overlay colors
-    overlay_array = histogram._overlay.get_array()
-    assert overlay_array.shape == (bins, bins, 4)
-    # indices where overlay_array is not zero
-    indices = np.where(overlay_array[..., -1] != 0)
-    assert np.all(indices[0] == indices_non_zero_overlay[0])
+import numpy as np
+import matplotlib.pyplot as plt
+
+from biaplotter.artists import (
+    Scatter, Histogram2D
+)
+
+
+def test_scatter():
+    size = 100
+    data = np.random.rand(size, 2)
+    fig, ax = plt.subplots()
+    scatter = Scatter(ax)
+    # Test Scatter signals
+    collected_data_signals = []
+    def on_data_changed(data):
+        collected_data_signals.append(data)
+    scatter.data_changed_signal.connect(on_data_changed)
+    assert len(collected_data_signals) == 0
+    # Set data
+    scatter.data = data
+    assert len(collected_data_signals) == 1
+    assert np.all(collected_data_signals[0] == data)
+    collected_color_indices_signals = []
+    def on_color_indices_changed(color_indices):
+        collected_color_indices_signals.append(color_indices)
+    scatter.color_indices_changed_signal.connect(on_color_indices_changed)
+    assert len(collected_color_indices_signals) == 0
+    # Set color_indices with an array of increasing repeating integers from 0 to 5
+    scatter.color_indices = np.linspace(
+        start=0, stop=5, num=size, endpoint=False, dtype=int)
+    assert len(collected_color_indices_signals) == 1
+    assert np.all(collected_color_indices_signals[0] == scatter.color_indices)
+    scatter.visible = True
+
+    # Test Scatter properties
+    assert scatter.data.shape == (size, 2)
+    assert scatter.visible == True
+    assert scatter.color_indices.shape == (size,)
+    assert scatter.color_indices.dtype == int
+
+    # Test scatter colors
+    colors = scatter._scatter.get_facecolors()
+    assert np.all(colors[0] == scatter.categorical_colormap(0))
+    assert np.all(colors[50] == scatter.categorical_colormap(2))
+
+
+def test_histogram2d():
+    # Inputs
+    threshold = 20
+    size = 1000
+    bins = 20
+
+    # Expected output
+    indices_non_zero_overlay = (
+        np.array([8, 9, 10], dtype=int), np.array([8, 9, 7], dtype=int))
+
+    np.random.seed(42)
+
+    # Generate gaussian distribution 2d data
+    x = np.random.normal(loc=0, scale=1, size=size)
+    y = np.random.normal(loc=0, scale=1, size=size)
+    data = np.column_stack([x, y])
+    fig, ax = plt.subplots()
+    histogram = Histogram2D(ax)
+    # Test Histogram2D signals
+    collected_data_signals = []
+    def on_data_changed(data):
+        collected_data_signals.append(data)
+    histogram.data_changed_signal.connect(on_data_changed)
+    assert len(collected_data_signals) == 0
+    histogram.data = data
+    assert len(collected_data_signals) == 1
+    assert np.all(collected_data_signals[0] == data)
+    collected_color_indices_signals = []
+    def on_color_indices_changed(color_indices):
+        collected_color_indices_signals.append(color_indices)
+    histogram.color_indices_changed_signal.connect(on_color_indices_changed)
+    assert len(collected_color_indices_signals) == 0
+    # Set color indices of data in patches exceeding threshold to 1 (orange color)
+    indices = histogram.indices_in_above_threshold_patches(threshold=threshold)
+    color_indices = np.zeros(size)
+    color_indices[indices] = 1
+    histogram.color_indices = color_indices
+    assert len(collected_color_indices_signals) == 1
+    assert np.all(collected_color_indices_signals[0] == color_indices)
+
+    histogram.visible = True
+    histogram.bins = bins
+
+    # Test Histogram2D properties
+    assert histogram.data.shape == (size, 2)
+    assert histogram.visible == True
+    assert histogram.color_indices.shape == (size,)
+    assert histogram.color_indices.dtype == int
+    assert histogram.bins == bins
+
+    # Test overlay colors
+    overlay_array = histogram._overlay.get_array()
+    assert overlay_array.shape == (bins, bins, 4)
+    # indices where overlay_array is not zero
+    indices = np.where(overlay_array[..., -1] != 0)
+    assert np.all(indices[0] == indices_non_zero_overlay[0])
```

### Comparing `biaplotter-0.0.1/src/biaplotter/_tests/test_selectors.py` & `biaplotter-0.0.2/src/biaplotter/_tests/test_selectors.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,106 +1,106 @@
-import pytest
-import numpy as np
-import matplotlib.pyplot as plt
-
-from biaplotter.selectors import (
-    BaseEllipseSelector, BaseRectangleSelector, BaseLassoSelector,
-    InteractiveRectangleSelector, InteractiveEllipseSelector, InteractiveLassoSelector
-)
-from biaplotter.plotter import CanvasWidget
-from biaplotter.artists import Scatter
-
-
-class MockMouseEvent:
-    """A mock event class to simulate MouseEvent with necessary attributes."""
-
-    def __init__(self, xdata, ydata):
-        self.xdata = xdata
-        self.ydata = ydata
-
-
-@pytest.fixture
-def setup_selector(request):
-    """Setup for base selector tests."""
-    fig, ax = plt.subplots()
-    data = np.array([[0, 0], [1, 1], [2, 2], [3, 3], [4, 4], [5, 5]])
-    selector_class = request.param
-    selector = selector_class(ax)
-    selector.data = data
-    selector.create_selector()
-    return selector
-
-
-@pytest.mark.parametrize("setup_selector, eclick_coords, erelease_coords, expected_indices", [
-    # Test case for BaseEllipseSelector
-    (BaseEllipseSelector, (1, 1), (5, 5), [2, 3, 4]),
-    # Empty region test case for BaseEllipseSelector
-    (BaseEllipseSelector, (0, 3), (1, 4), []),
-    # Test case for BaseRectangleSelector
-    (BaseRectangleSelector, (1.5, 1), (4.5, 5), [2, 3, 4]),
-    # Empty region test case for BaseRectangleSelector
-    (BaseRectangleSelector, (0, 3), (1, 4), [])
-], indirect=["setup_selector"])
-def test_base_ellipse_and_rectangle_selectors(setup_selector, eclick_coords, erelease_coords, expected_indices):
-    """Test BaseEllipseSelector and BaseRectangleSelector."""
-    selector = setup_selector
-    eclick = MockMouseEvent(*eclick_coords)
-    erelease = MockMouseEvent(*erelease_coords)
-    actual_indices = selector.on_select(eclick, erelease)
-    actual_indices.sort()
-
-    assert np.array_equal(actual_indices, expected_indices), "Indices of selected points {} do not match expected values {}.".format(
-        actual_indices, expected_indices)
-
-
-@pytest.mark.parametrize("setup_selector, vertices, expected_indices", [
-    (BaseLassoSelector, [(1.5, 1), (1.5, 5), (4.5, 5), (4.5, 1)], [
-     2, 3, 4]),  # Test case for BaseLassoSelector
-    # Empty region test case for BaseLassoSelector
-    (BaseLassoSelector, [(0, 3), (0, 4), (1, 4)], []),
-], indirect=["setup_selector"])
-def test_base_lasso_selector(setup_selector, vertices, expected_indices):
-    """Test BaseLassoSelector."""
-    selector = setup_selector
-    actual_indices = selector.on_select(vertices)
-    actual_indices.sort()
-
-    assert np.array_equal(actual_indices, expected_indices), "Indices of selected points {} do not match expected values {}.".format(
-        actual_indices, expected_indices)
-
-
-@pytest.fixture
-def selector_class(request):
-    """Fixture to dynamically handle the selector class type."""
-    return request.param
-
-
-@pytest.mark.parametrize("selector_class, expected_color_indices", [
-    # Test case for InteractiveRectangleSelector
-    (InteractiveRectangleSelector, [0, 0, 1, 1, 1, 0]),
-    # Test case for InteractiveEllipseSelector
-    (InteractiveEllipseSelector, [0, 0, 1, 1, 1, 0]),
-    # Test case for InteractiveLassoSelector
-    (InteractiveLassoSelector, [0, 0, 1, 1, 1, 0])
-], indirect=["selector_class"])
-def test_interactive_selectors(make_napari_viewer, selector_class, expected_color_indices):
-    """Test InteractiveRectangleSelector, InteractiveEllipseSelector, and InteractiveLassoSelector."""
-    viewer = make_napari_viewer()
-    widget = CanvasWidget(viewer)
-    selector = selector_class(widget.axes, widget)
-    assert selector is not None
-
-    data = np.array([[0, 0], [1, 1], [2, 2], [3, 3], [4, 4], [5, 5]])
-    # Set artist data to initialize color indices
-    artist = widget.active_artist
-    artist.data = data
-    selector.data = data
-    selector.create_selector()
-    assert selector._selector is not None
-
-    selector.class_value = 1
-    selector.selected_indices = [2, 3, 4]
-    # artist color indices are updated based on selected indices
-    selector.apply_selection()
-    assert np.array_equal(artist.color_indices, expected_color_indices), \
-        "Color indices {} do not match expected values {}.".format(
-            selector.color_indices, expected_color_indices)
+import pytest
+import numpy as np
+import matplotlib.pyplot as plt
+
+from biaplotter.selectors import (
+    BaseEllipseSelector, BaseRectangleSelector, BaseLassoSelector,
+    InteractiveRectangleSelector, InteractiveEllipseSelector, InteractiveLassoSelector
+)
+from biaplotter.plotter import CanvasWidget
+from biaplotter.artists import Scatter
+
+
+class MockMouseEvent:
+    """A mock event class to simulate MouseEvent with necessary attributes."""
+
+    def __init__(self, xdata, ydata):
+        self.xdata = xdata
+        self.ydata = ydata
+
+
+@pytest.fixture
+def setup_selector(request):
+    """Setup for base selector tests."""
+    fig, ax = plt.subplots()
+    data = np.array([[0, 0], [1, 1], [2, 2], [3, 3], [4, 4], [5, 5]])
+    selector_class = request.param
+    selector = selector_class(ax)
+    selector.data = data
+    selector.create_selector()
+    return selector
+
+
+@pytest.mark.parametrize("setup_selector, eclick_coords, erelease_coords, expected_indices", [
+    # Test case for BaseEllipseSelector
+    (BaseEllipseSelector, (1, 1), (5, 5), [2, 3, 4]),
+    # Empty region test case for BaseEllipseSelector
+    (BaseEllipseSelector, (0, 3), (1, 4), []),
+    # Test case for BaseRectangleSelector
+    (BaseRectangleSelector, (1.5, 1), (4.5, 5), [2, 3, 4]),
+    # Empty region test case for BaseRectangleSelector
+    (BaseRectangleSelector, (0, 3), (1, 4), [])
+], indirect=["setup_selector"])
+def test_base_ellipse_and_rectangle_selectors(setup_selector, eclick_coords, erelease_coords, expected_indices):
+    """Test BaseEllipseSelector and BaseRectangleSelector."""
+    selector = setup_selector
+    eclick = MockMouseEvent(*eclick_coords)
+    erelease = MockMouseEvent(*erelease_coords)
+    actual_indices = selector.on_select(eclick, erelease)
+    actual_indices.sort()
+
+    assert np.array_equal(actual_indices, expected_indices), "Indices of selected points {} do not match expected values {}.".format(
+        actual_indices, expected_indices)
+
+
+@pytest.mark.parametrize("setup_selector, vertices, expected_indices", [
+    (BaseLassoSelector, [(1.5, 1), (1.5, 5), (4.5, 5), (4.5, 1)], [
+     2, 3, 4]),  # Test case for BaseLassoSelector
+    # Empty region test case for BaseLassoSelector
+    (BaseLassoSelector, [(0, 3), (0, 4), (1, 4)], []),
+], indirect=["setup_selector"])
+def test_base_lasso_selector(setup_selector, vertices, expected_indices):
+    """Test BaseLassoSelector."""
+    selector = setup_selector
+    actual_indices = selector.on_select(vertices)
+    actual_indices.sort()
+
+    assert np.array_equal(actual_indices, expected_indices), "Indices of selected points {} do not match expected values {}.".format(
+        actual_indices, expected_indices)
+
+
+@pytest.fixture
+def selector_class(request):
+    """Fixture to dynamically handle the selector class type."""
+    return request.param
+
+
+@pytest.mark.parametrize("selector_class, expected_color_indices", [
+    # Test case for InteractiveRectangleSelector
+    (InteractiveRectangleSelector, [0, 0, 1, 1, 1, 0]),
+    # Test case for InteractiveEllipseSelector
+    (InteractiveEllipseSelector, [0, 0, 1, 1, 1, 0]),
+    # Test case for InteractiveLassoSelector
+    (InteractiveLassoSelector, [0, 0, 1, 1, 1, 0])
+], indirect=["selector_class"])
+def test_interactive_selectors(make_napari_viewer, selector_class, expected_color_indices):
+    """Test InteractiveRectangleSelector, InteractiveEllipseSelector, and InteractiveLassoSelector."""
+    viewer = make_napari_viewer()
+    widget = CanvasWidget(viewer)
+    selector = selector_class(widget.axes, widget)
+    assert selector is not None
+
+    data = np.array([[0, 0], [1, 1], [2, 2], [3, 3], [4, 4], [5, 5]])
+    # Set artist data to initialize color indices
+    artist = widget.active_artist
+    artist.data = data
+    selector.data = data
+    selector.create_selector()
+    assert selector._selector is not None
+
+    selector.class_value = 1
+    selector.selected_indices = [2, 3, 4]
+    # artist color indices are updated based on selected indices
+    selector.apply_selection()
+    assert np.array_equal(artist.color_indices, expected_color_indices), \
+        "Color indices {} do not match expected values {}.".format(
+            selector.color_indices, expected_color_indices)
```

### Comparing `biaplotter-0.0.1/src/biaplotter/artists.py` & `biaplotter-0.0.2/src/biaplotter/artists.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,495 +1,495 @@
-import numpy as np
-import matplotlib.pyplot as plt
-
-from matplotlib.colors import Colormap
-from matplotlib.collections import QuadMesh
-from abc import ABC, abstractmethod
-from nap_plot_tools.cmap import cat10_mod_cmap, cat10_mod_cmap_first_transparent
-from psygnal import Signal
-from typing import Tuple, List
-
-
-class Artist(ABC):
-    """Abstract base class for artists in the BiAPlotter.
-
-    Parameters
-    ----------
-    ax : plt.Axes, optional
-        axes to plot on, by default None
-    data : (N, 2) np.ndarray
-        data to be plotted
-    categorical_colormap : Colormap, optional
-        a colormap to use for the artist, by default cat10_mod_cmap from nap-plot-tools
-    color_indices : (N,) np.ndarray, optional
-        array of indices to map to the colormap, by default None
-    """
-
-    def __init__(self, ax: plt.Axes = None, data: np.ndarray = None, categorical_colormap: Colormap = cat10_mod_cmap, color_indices: np.ndarray = None):
-        """Initializes the abstract artist.
-        """
-        #: Stores data to be plotted
-        self._data: np.ndarray = data
-        #: Stores axes to plot on
-        self.ax: plt.Axes = ax if ax is not None else plt.gca()
-        #: Stores visibility of the artist
-        self._visible: bool = True
-        #: Stores the colormap to use for the artist
-        self.categorical_colormap: Colormap = categorical_colormap
-        #: Stores the array of indices to map to the colormap
-        self._color_indices: np.array = color_indices
-
-    @property
-    @abstractmethod
-    def data(self) -> np.ndarray:
-        """Abstract property for the artist's data."""
-        pass
-
-    @data.setter
-    @abstractmethod
-    def data(self, value: np.ndarray):
-        """Abstract setter for the artist's data."""
-        pass
-
-    @property
-    @abstractmethod
-    def visible(self) -> bool:
-        """Abstract property for the artist's visibility."""
-        pass
-
-    @visible.setter
-    @abstractmethod
-    def visible(self, value: bool):
-        """Abstract setter for the artist's visibility."""
-        pass
-
-    @property
-    @abstractmethod
-    def color_indices(self) -> np.ndarray:
-        """Abstract property for the indices into the colormap."""
-        pass
-
-    @color_indices.setter
-    @abstractmethod
-    def color_indices(self, indices: np.ndarray):
-        """Abstract setter for the indices into the colormap."""
-        pass
-
-    @abstractmethod
-    def draw(self):
-        """Abstract method to draw or redraw the artist."""
-        pass
-
-
-class Scatter(Artist):
-    """Scatter plot artist for the BiAPlotter.
-
-    Inherits all parameters and attributes from abstract Artist.
-    For parameter and attribute details, see the abstract Artist class documentation.
-
-    Parameters
-    ----------
-    ax : plt.Axes, optional
-        axes to plot on, by default None
-    data : (N, 2) np.ndarray
-        data to be plotted
-    categorical_colormap : Colormap, optional
-        a colormap to use for the artist, by default cat10_mod_cmap from nap-plot-tools
-    color_indices : (N,) np.ndarray[int] or int, optional
-        array of indices to map to the colormap, by default None
-
-    Notes
-    -----
-    **Signals:**
-
-        * **data_changed_signal** emitted when the data is changed.
-        * **color_indices_changed_signal** emitted when the color indices are changed.
-
-    Examples
-    --------
-    >>> import numpy as np
-    >>> import matplotlib.pyplot as plt
-    >>> from biaplotter.artists import Scatter
-    >>> data = np.random.rand(100, 2)
-    >>> fig, ax = plt.subplots()
-    >>> scatter = Scatter(ax)
-    >>> scatter.data = data
-    >>> scatter.visible = True
-    >>> scatter.color_indices = np.linspace(start=0, stop=5, num=100, endpoint=False, dtype=int)
-    >>> plt.show()
-    """
-    #: Signal emitted when the `data` is changed.
-    data_changed_signal: Signal = Signal(np.ndarray)
-    #: Signal emitted when the `color_indices` are changed.
-    color_indices_changed_signal: Signal = Signal(np.ndarray)
-
-    def __init__(self, ax: plt.Axes = None, data: np.ndarray = None, categorical_colormap: Colormap = cat10_mod_cmap, color_indices: np.ndarray = None):
-        """Initializes the scatter plot artist.
-        """
-        super().__init__(ax, data, categorical_colormap, color_indices)
-        #: Stores the scatter plot matplotlib object
-        self._scatter = None
-        self.data = data
-        self.draw()  # Initial draw of the scatter plot
-
-    @property
-    def data(self) -> np.ndarray:
-        """Gets or sets the data associated with the scatter plot.
-
-        Updates colors if color_indices are set. Triggers a draw idle command.
-
-        Returns
-        -------
-        data : (N, 2) np.ndarray
-           data for the artist. Does not respond if set to None or empty array.
-
-        Notes
-        -----
-        data_changed_signal : Signal
-            Signal emitted when the data is changed.
-        """
-        return self._data
-
-    @data.setter
-    def data(self, value: np.ndarray):
-        """Sets the data for the scatter plot, updating the display as needed."""
-        if value is None:
-            return
-        if len(value) == 0:
-            return
-        self._data = value
-        # emit signal
-        self.data_changed_signal.emit(self._data)
-        if self._scatter is None:
-            self._scatter = self.ax.scatter(value[:, 0], value[:, 1])
-            self.color_indices = 0  # Set default color index
-        else:
-            # If the scatter plot already exists, just update its data
-            self._scatter.set_offsets(value)
-        
-        if self._color_indices is None:
-            self.color_indices = 0  # Set default color index
-        else:
-            # Update colors if color indices are set, resize if data shape has changed
-            color_indices_size = len(self._color_indices)
-            color_indices = np.resize(self._color_indices, self._data.shape[0])
-            if len(color_indices) > color_indices_size:
-                # fill with zeros where new data is larger
-                color_indices[color_indices_size:] = 0
-            self.color_indices = color_indices
-        self.draw()
-
-    @property
-    def visible(self) -> bool:
-        """Gets or sets the visibility of the scatter plot.
-
-        Triggers a draw idle command.
-
-        Returns
-        -------
-        visible : bool
-            visibility of the scatter plot.
-        """
-        return self._visible
-
-    @visible.setter
-    def visible(self, value: bool):
-        """Sets the visibility of the scatter plot."""
-        self._visible = value
-        if self._scatter is not None:
-            self._scatter.set_visible(value)
-        self.draw()
-
-    @property
-    def color_indices(self) -> np.ndarray:
-        """Gets or sets the current color indices used for the scatter plot.
-
-        Triggers a draw idle command.
-
-        Returns
-        -------
-        color_indices : (N,) np.ndarray[int] or int
-            indices to map to the categorical_colormap. Accepts a scalar or an array of integers.
-        
-        Notes
-        -----
-        color_indices_changed_signal : Signal
-            Signal emitted when the color indices are changed.
-
-        """
-        return self._color_indices
-
-    @color_indices.setter
-    def color_indices(self, indices: np.ndarray):
-        """Sets color indices for the scatter plot and updates colors accordingly."""
-        # Check if indices are a scalar
-        if np.isscalar(indices):
-            indices = np.full(len(self._data), indices)
-        # Check if indices data type is float
-        if indices.dtype == float:
-            indices = indices.astype(int)
-        self._color_indices = indices
-        if indices is not None and self._scatter is not None:
-            new_colors = self.categorical_colormap(indices)
-            self._scatter.set_facecolor(new_colors)
-            self._scatter.set_edgecolor(None)
-        # emit signal
-        self.color_indices_changed_signal.emit(self._color_indices)
-        self.draw()
-
-    def draw(self):
-        """Draws or redraws the scatter plot."""
-        self.ax.figure.canvas.draw_idle()
-
-
-class Histogram2D(Artist):
-    """2D histogram artist for the BiAPlotter.
-
-    Inherits all parameters and attributes from abstract Artist.
-    For parameter and attribute details, see the abstract Artist class documentation.
-
-    Parameters
-    ----------
-    ax : plt.Axes, optional
-        axes to plot on, by default None
-    data : (N, 2) np.ndarray
-        data to be plotted
-    categorical_colormap : Colormap, optional
-        a colormap to use for the artist overlay, by default cat10_mod_cmap_first_transparent from nap-plot-tools (first color is transparent)
-    color_indices : (N,) np.ndarray[int] or int, optional
-        array of indices to map to the categorical_colormap, by default None
-    bins : int, optional
-        number of bins for the histogram, by default 20
-    histogram_colormap : Colormap, optional
-        colormap for the histogram, by default plt.cm.magma
-
-    Notes
-    -----
-    **Signals:**
-
-        * **data_changed_signal** emitted when the data is changed.
-        * **color_indices_changed_signal** emitted when the color indices are changed.
-
-    """
-    #: Signal emitted when the `data` is changed.
-    data_changed_signal: Signal = Signal(np.ndarray)
-    #: Signal emitted when the `color_indices` are changed.
-    color_indices_changed_signal: Signal = Signal(np.ndarray)
-
-    def __init__(self, ax: plt.Axes = None, data: np.ndarray = None, categorical_colormap: Colormap = cat10_mod_cmap_first_transparent, color_indices: np.ndarray = None, bins=20, histogram_colormap: Colormap = plt.cm.magma):
-        super().__init__(ax, data, categorical_colormap, color_indices)
-        """Initializes the 2D histogram artist.
-        """
-        #: Stores the matplotlib histogram2D object
-        self._histogram = None
-        self._bins = bins
-        self._histogram_colormap = histogram_colormap
-        self._overlay = None
-        self.data = data
-        self.draw()  # Initial draw of the histogram
-
-    @property
-    def data(self) -> np.ndarray:
-        """Gets or sets the data associated with the 2D histogram.
-
-        Updates colors if color_indices are set. Triggers a draw idle command.
-
-        Returns
-        -------
-        data : (N, 2) np.ndarray
-            data for the artist. Does not respond if set to None or empty array.
-
-        Notes
-        -----
-        data_changed_signal : Signal
-            Signal emitted when the data is changed.
-        """
-        return self._data
-
-    @data.setter
-    def data(self, value: np.ndarray):
-        """Sets the data for the 2D histogram, updating the display as needed."""
-        if value is None:
-            return
-        if len(value) == 0:
-            return
-        self._data = value
-        # emit signal
-        self.data_changed_signal.emit(self._data)
-        # Remove the existing histogram to redraw
-        if self._histogram is not None:
-            self._histogram[-1].remove()
-        # Draw the new histogram
-        self._histogram = self.ax.hist2d(
-            value[:, 0], value[:, 1], bins=self._bins, cmap=self._histogram_colormap, zorder=1)
-        if self._color_indices is None:
-            self.color_indices = 0  # Set default color index
-        else:
-            # Update colors if color indices are set, resize if data shape has changed
-            color_indices_size = len(self._color_indices)
-            color_indices = np.resize(self._color_indices, self._data.shape[0])
-            if len(color_indices) > color_indices_size:
-                # fill with zeros where new data is larger
-                color_indices[color_indices_size:] = 0
-            self.color_indices = color_indices
-        self.draw()
-
-    @property
-    def visible(self) -> bool:
-        """Gets or sets the visibility of the 2D histogram.
-
-        Triggers a draw idle command.
-
-        Returns
-        -------
-        visible : bool
-            visibility of the 2D histogram.
-        """
-        return self._visible
-
-    @visible.setter
-    def visible(self, value: bool):
-        """Sets the visibility of the 2D histogram."""
-        self._visible = value
-        if self._histogram is not None:
-            artist = self._histogram[-1]
-            artist.set_visible(value)
-            if self._overlay is not None:
-                self._overlay.set_visible(value)
-        self.draw()
-
-    @property
-    def color_indices(self) -> np.ndarray:
-        """Gets or sets the current color indices used for the 2D histogram underlying data.
-
-        Triggers a draw idle command.
-
-        Returns
-        -------
-        color_indices : (N,) np.ndarray[int] or int
-            indices to map to the overlay colormap. Accepts a scalar or an array.
-        
-        Notes
-        -----
-        color_indices_changed_signal : Signal
-            Signal emitted when the color indices are changed.
-
-        """
-        return self._color_indices
-
-    @color_indices.setter
-    def color_indices(self, indices: np.ndarray):
-        """Sets color indices for the 2D histogram underlying data and updates colors accordingly."""
-        # Check if indices are a scalar
-        if np.isscalar(indices):
-            indices = np.full(len(self._data), indices)
-        # Check if indices data type is float
-        if indices.dtype == float:
-            indices = indices.astype(int)
-        self._color_indices = indices
-        h, xedges, yedges, _ = self._histogram
-        # Create empty overlay
-        overlay_rgba = np.zeros((*h.shape, 4), dtype=float)
-        output_max = np.zeros(h.shape, dtype=float)
-        for i in np.unique(self._color_indices):
-            # Filter data by class
-            data_filtered_by_class = self._data[self._color_indices == i]
-            # Calculate histogram of filtered data while fixing the bins
-            histogram_filtered_by_class, _, _ = np.histogram2d(
-                data_filtered_by_class[:, 0], data_filtered_by_class[:, 1], bins=[xedges, yedges])
-            class_mask = histogram_filtered_by_class > output_max
-            output_max = np.maximum(histogram_filtered_by_class, output_max)
-            overlay_rgba[class_mask] = self.categorical_colormap(i)
-        # Remove the existing overlay to redraw
-        if self._overlay is not None:
-            self._overlay.remove()
-        # Draw the overlay
-        self._overlay = self.ax.imshow(overlay_rgba.swapaxes(0, 1), origin='lower', extent=[
-            xedges[0], xedges[-1], yedges[0], yedges[-1]], aspect='auto', alpha=1, zorder=2)
-        # emit signal
-        self.color_indices_changed_signal.emit(self._color_indices)
-        self.draw()
-
-    @property
-    def bins(self) -> int:
-        """Gets or sets the number of bins for the histogram.
-
-        Returns
-        -------
-        bins : int
-            number of bins for the histogram.
-        """
-        return self._bins
-
-    @bins.setter
-    def bins(self, value: int):
-        """Sets the number of bins for the histogram."""
-        self._bins = value
-        self.data = self._data
-
-    @property
-    def histogram_colormap(self) -> Colormap:
-        """Gets or sets the colormap for the histogram.
-
-        Returns
-        -------
-        histogram_colormap : Colormap
-            colormap for the histogram.
-        """
-        return self._histogram_colormap
-
-    @histogram_colormap.setter
-    def histogram_colormap(self, value: Colormap):
-        """Sets the colormap for the histogram."""
-        self._histogram_colormap = value
-        self.data = self._data
-
-    @property
-    def histogram(self) -> Tuple[np.ndarray, np.ndarray, np.ndarray, QuadMesh]:
-        """Returns the 2D histogram matplotlib object.
-
-        Returns
-        -------
-        histogram : Tuple[np.ndarray, np.ndarray, np.ndarray, QuadMesh]
-            2D histogram matplotlib object.
-        """
-        return self._histogram
-
-    def indices_in_above_threshold_patches(self, threshold: int) -> List[int]:
-        """
-        Returns the indices of the points in that fall into the bins
-        of the 2D histogram exceeding a specified threshold.
-
-        Parameters
-        ----------
-        threshold : int
-            The count threshold to exceed.
-
-        Returns
-        -------
-        indices : List[int]
-            list of indices of points falling into the exceeding bins.
-        """
-        counts, xedges, yedges, _ = self._histogram
-
-        # Identify bins that exceed the threshold
-        exceeding_bins = np.argwhere(counts > threshold)
-
-        # Prepare to collect indices
-        indices = []
-
-        # For each bin exceeding the threshold...
-        for bin_x, bin_y in exceeding_bins:
-            # Identify the edges of the current bin
-            x_min, x_max = xedges[bin_x], xedges[bin_x + 1]
-            y_min, y_max = yedges[bin_y], yedges[bin_y + 1]
-
-            # Find indices of points within these edges
-            bin_indices = np.where((self._data[:, 0] >= x_min) & (self._data[:, 0] < x_max) & (
-                self._data[:, 1] >= y_min) & (self._data[:, 1] < y_max))[0]
-            indices.extend(bin_indices)
-
-        return indices
-
-    def draw(self):
-        """Draws or redraws the 2D histogram."""
-        self.ax.figure.canvas.draw_idle()
+import numpy as np
+import matplotlib.pyplot as plt
+
+from matplotlib.colors import Colormap
+from matplotlib.collections import QuadMesh
+from abc import ABC, abstractmethod
+from nap_plot_tools.cmap import cat10_mod_cmap, cat10_mod_cmap_first_transparent
+from psygnal import Signal
+from typing import Tuple, List
+
+
+class Artist(ABC):
+    """Abstract base class for artists in the BiAPlotter.
+
+    Parameters
+    ----------
+    ax : plt.Axes, optional
+        axes to plot on, by default None
+    data : (N, 2) np.ndarray
+        data to be plotted
+    categorical_colormap : Colormap, optional
+        a colormap to use for the artist, by default cat10_mod_cmap from nap-plot-tools
+    color_indices : (N,) np.ndarray, optional
+        array of indices to map to the colormap, by default None
+    """
+
+    def __init__(self, ax: plt.Axes = None, data: np.ndarray = None, categorical_colormap: Colormap = cat10_mod_cmap, color_indices: np.ndarray = None):
+        """Initializes the abstract artist.
+        """
+        #: Stores data to be plotted
+        self._data: np.ndarray = data
+        #: Stores axes to plot on
+        self.ax: plt.Axes = ax if ax is not None else plt.gca()
+        #: Stores visibility of the artist
+        self._visible: bool = True
+        #: Stores the colormap to use for the artist
+        self.categorical_colormap: Colormap = categorical_colormap
+        #: Stores the array of indices to map to the colormap
+        self._color_indices: np.array = color_indices
+
+    @property
+    @abstractmethod
+    def data(self) -> np.ndarray:
+        """Abstract property for the artist's data."""
+        pass
+
+    @data.setter
+    @abstractmethod
+    def data(self, value: np.ndarray):
+        """Abstract setter for the artist's data."""
+        pass
+
+    @property
+    @abstractmethod
+    def visible(self) -> bool:
+        """Abstract property for the artist's visibility."""
+        pass
+
+    @visible.setter
+    @abstractmethod
+    def visible(self, value: bool):
+        """Abstract setter for the artist's visibility."""
+        pass
+
+    @property
+    @abstractmethod
+    def color_indices(self) -> np.ndarray:
+        """Abstract property for the indices into the colormap."""
+        pass
+
+    @color_indices.setter
+    @abstractmethod
+    def color_indices(self, indices: np.ndarray):
+        """Abstract setter for the indices into the colormap."""
+        pass
+
+    @abstractmethod
+    def draw(self):
+        """Abstract method to draw or redraw the artist."""
+        pass
+
+
+class Scatter(Artist):
+    """Scatter plot artist for the BiAPlotter.
+
+    Inherits all parameters and attributes from abstract Artist.
+    For parameter and attribute details, see the abstract Artist class documentation.
+
+    Parameters
+    ----------
+    ax : plt.Axes, optional
+        axes to plot on, by default None
+    data : (N, 2) np.ndarray
+        data to be plotted
+    categorical_colormap : Colormap, optional
+        a colormap to use for the artist, by default cat10_mod_cmap from nap-plot-tools
+    color_indices : (N,) np.ndarray[int] or int, optional
+        array of indices to map to the colormap, by default None
+
+    Notes
+    -----
+    **Signals:**
+
+        * **data_changed_signal** emitted when the data is changed.
+        * **color_indices_changed_signal** emitted when the color indices are changed.
+
+    Examples
+    --------
+    >>> import numpy as np
+    >>> import matplotlib.pyplot as plt
+    >>> from biaplotter.artists import Scatter
+    >>> data = np.random.rand(100, 2)
+    >>> fig, ax = plt.subplots()
+    >>> scatter = Scatter(ax)
+    >>> scatter.data = data
+    >>> scatter.visible = True
+    >>> scatter.color_indices = np.linspace(start=0, stop=5, num=100, endpoint=False, dtype=int)
+    >>> plt.show()
+    """
+    #: Signal emitted when the `data` is changed.
+    data_changed_signal: Signal = Signal(np.ndarray)
+    #: Signal emitted when the `color_indices` are changed.
+    color_indices_changed_signal: Signal = Signal(np.ndarray)
+
+    def __init__(self, ax: plt.Axes = None, data: np.ndarray = None, categorical_colormap: Colormap = cat10_mod_cmap, color_indices: np.ndarray = None):
+        """Initializes the scatter plot artist.
+        """
+        super().__init__(ax, data, categorical_colormap, color_indices)
+        #: Stores the scatter plot matplotlib object
+        self._scatter = None
+        self.data = data
+        self.draw()  # Initial draw of the scatter plot
+
+    @property
+    def data(self) -> np.ndarray:
+        """Gets or sets the data associated with the scatter plot.
+
+        Updates colors if color_indices are set. Triggers a draw idle command.
+
+        Returns
+        -------
+        data : (N, 2) np.ndarray
+           data for the artist. Does not respond if set to None or empty array.
+
+        Notes
+        -----
+        data_changed_signal : Signal
+            Signal emitted when the data is changed.
+        """
+        return self._data
+
+    @data.setter
+    def data(self, value: np.ndarray):
+        """Sets the data for the scatter plot, updating the display as needed."""
+        if value is None:
+            return
+        if len(value) == 0:
+            return
+        self._data = value
+        # emit signal
+        self.data_changed_signal.emit(self._data)
+        if self._scatter is None:
+            self._scatter = self.ax.scatter(value[:, 0], value[:, 1])
+            self.color_indices = 0  # Set default color index
+        else:
+            # If the scatter plot already exists, just update its data
+            self._scatter.set_offsets(value)
+        
+        if self._color_indices is None:
+            self.color_indices = 0  # Set default color index
+        else:
+            # Update colors if color indices are set, resize if data shape has changed
+            color_indices_size = len(self._color_indices)
+            color_indices = np.resize(self._color_indices, self._data.shape[0])
+            if len(color_indices) > color_indices_size:
+                # fill with zeros where new data is larger
+                color_indices[color_indices_size:] = 0
+            self.color_indices = color_indices
+        self.draw()
+
+    @property
+    def visible(self) -> bool:
+        """Gets or sets the visibility of the scatter plot.
+
+        Triggers a draw idle command.
+
+        Returns
+        -------
+        visible : bool
+            visibility of the scatter plot.
+        """
+        return self._visible
+
+    @visible.setter
+    def visible(self, value: bool):
+        """Sets the visibility of the scatter plot."""
+        self._visible = value
+        if self._scatter is not None:
+            self._scatter.set_visible(value)
+        self.draw()
+
+    @property
+    def color_indices(self) -> np.ndarray:
+        """Gets or sets the current color indices used for the scatter plot.
+
+        Triggers a draw idle command.
+
+        Returns
+        -------
+        color_indices : (N,) np.ndarray[int] or int
+            indices to map to the categorical_colormap. Accepts a scalar or an array of integers.
+        
+        Notes
+        -----
+        color_indices_changed_signal : Signal
+            Signal emitted when the color indices are changed.
+
+        """
+        return self._color_indices
+
+    @color_indices.setter
+    def color_indices(self, indices: np.ndarray):
+        """Sets color indices for the scatter plot and updates colors accordingly."""
+        # Check if indices are a scalar
+        if np.isscalar(indices):
+            indices = np.full(len(self._data), indices)
+        # Check if indices data type is float
+        if indices.dtype == float:
+            indices = indices.astype(int)
+        self._color_indices = indices
+        if indices is not None and self._scatter is not None:
+            new_colors = self.categorical_colormap(indices)
+            self._scatter.set_facecolor(new_colors)
+            self._scatter.set_edgecolor(None)
+        # emit signal
+        self.color_indices_changed_signal.emit(self._color_indices)
+        self.draw()
+
+    def draw(self):
+        """Draws or redraws the scatter plot."""
+        self.ax.figure.canvas.draw_idle()
+
+
+class Histogram2D(Artist):
+    """2D histogram artist for the BiAPlotter.
+
+    Inherits all parameters and attributes from abstract Artist.
+    For parameter and attribute details, see the abstract Artist class documentation.
+
+    Parameters
+    ----------
+    ax : plt.Axes, optional
+        axes to plot on, by default None
+    data : (N, 2) np.ndarray
+        data to be plotted
+    categorical_colormap : Colormap, optional
+        a colormap to use for the artist overlay, by default cat10_mod_cmap_first_transparent from nap-plot-tools (first color is transparent)
+    color_indices : (N,) np.ndarray[int] or int, optional
+        array of indices to map to the categorical_colormap, by default None
+    bins : int, optional
+        number of bins for the histogram, by default 20
+    histogram_colormap : Colormap, optional
+        colormap for the histogram, by default plt.cm.magma
+
+    Notes
+    -----
+    **Signals:**
+
+        * **data_changed_signal** emitted when the data is changed.
+        * **color_indices_changed_signal** emitted when the color indices are changed.
+
+    """
+    #: Signal emitted when the `data` is changed.
+    data_changed_signal: Signal = Signal(np.ndarray)
+    #: Signal emitted when the `color_indices` are changed.
+    color_indices_changed_signal: Signal = Signal(np.ndarray)
+
+    def __init__(self, ax: plt.Axes = None, data: np.ndarray = None, categorical_colormap: Colormap = cat10_mod_cmap_first_transparent, color_indices: np.ndarray = None, bins=20, histogram_colormap: Colormap = plt.cm.magma):
+        super().__init__(ax, data, categorical_colormap, color_indices)
+        """Initializes the 2D histogram artist.
+        """
+        #: Stores the matplotlib histogram2D object
+        self._histogram = None
+        self._bins = bins
+        self._histogram_colormap = histogram_colormap
+        self._overlay = None
+        self.data = data
+        self.draw()  # Initial draw of the histogram
+
+    @property
+    def data(self) -> np.ndarray:
+        """Gets or sets the data associated with the 2D histogram.
+
+        Updates colors if color_indices are set. Triggers a draw idle command.
+
+        Returns
+        -------
+        data : (N, 2) np.ndarray
+            data for the artist. Does not respond if set to None or empty array.
+
+        Notes
+        -----
+        data_changed_signal : Signal
+            Signal emitted when the data is changed.
+        """
+        return self._data
+
+    @data.setter
+    def data(self, value: np.ndarray):
+        """Sets the data for the 2D histogram, updating the display as needed."""
+        if value is None:
+            return
+        if len(value) == 0:
+            return
+        self._data = value
+        # emit signal
+        self.data_changed_signal.emit(self._data)
+        # Remove the existing histogram to redraw
+        if self._histogram is not None:
+            self._histogram[-1].remove()
+        # Draw the new histogram
+        self._histogram = self.ax.hist2d(
+            value[:, 0], value[:, 1], bins=self._bins, cmap=self._histogram_colormap, zorder=1)
+        if self._color_indices is None:
+            self.color_indices = 0  # Set default color index
+        else:
+            # Update colors if color indices are set, resize if data shape has changed
+            color_indices_size = len(self._color_indices)
+            color_indices = np.resize(self._color_indices, self._data.shape[0])
+            if len(color_indices) > color_indices_size:
+                # fill with zeros where new data is larger
+                color_indices[color_indices_size:] = 0
+            self.color_indices = color_indices
+        self.draw()
+
+    @property
+    def visible(self) -> bool:
+        """Gets or sets the visibility of the 2D histogram.
+
+        Triggers a draw idle command.
+
+        Returns
+        -------
+        visible : bool
+            visibility of the 2D histogram.
+        """
+        return self._visible
+
+    @visible.setter
+    def visible(self, value: bool):
+        """Sets the visibility of the 2D histogram."""
+        self._visible = value
+        if self._histogram is not None:
+            artist = self._histogram[-1]
+            artist.set_visible(value)
+            if self._overlay is not None:
+                self._overlay.set_visible(value)
+        self.draw()
+
+    @property
+    def color_indices(self) -> np.ndarray:
+        """Gets or sets the current color indices used for the 2D histogram underlying data.
+
+        Triggers a draw idle command.
+
+        Returns
+        -------
+        color_indices : (N,) np.ndarray[int] or int
+            indices to map to the overlay colormap. Accepts a scalar or an array.
+        
+        Notes
+        -----
+        color_indices_changed_signal : Signal
+            Signal emitted when the color indices are changed.
+
+        """
+        return self._color_indices
+
+    @color_indices.setter
+    def color_indices(self, indices: np.ndarray):
+        """Sets color indices for the 2D histogram underlying data and updates colors accordingly."""
+        # Check if indices are a scalar
+        if np.isscalar(indices):
+            indices = np.full(len(self._data), indices)
+        # Check if indices data type is float
+        if indices.dtype == float:
+            indices = indices.astype(int)
+        self._color_indices = indices
+        h, xedges, yedges, _ = self._histogram
+        # Create empty overlay
+        overlay_rgba = np.zeros((*h.shape, 4), dtype=float)
+        output_max = np.zeros(h.shape, dtype=float)
+        for i in np.unique(self._color_indices):
+            # Filter data by class
+            data_filtered_by_class = self._data[self._color_indices == i]
+            # Calculate histogram of filtered data while fixing the bins
+            histogram_filtered_by_class, _, _ = np.histogram2d(
+                data_filtered_by_class[:, 0], data_filtered_by_class[:, 1], bins=[xedges, yedges])
+            class_mask = histogram_filtered_by_class > output_max
+            output_max = np.maximum(histogram_filtered_by_class, output_max)
+            overlay_rgba[class_mask] = self.categorical_colormap(i)
+        # Remove the existing overlay to redraw
+        if self._overlay is not None:
+            self._overlay.remove()
+        # Draw the overlay
+        self._overlay = self.ax.imshow(overlay_rgba.swapaxes(0, 1), origin='lower', extent=[
+            xedges[0], xedges[-1], yedges[0], yedges[-1]], aspect='auto', alpha=1, zorder=2)
+        # emit signal
+        self.color_indices_changed_signal.emit(self._color_indices)
+        self.draw()
+
+    @property
+    def bins(self) -> int:
+        """Gets or sets the number of bins for the histogram.
+
+        Returns
+        -------
+        bins : int
+            number of bins for the histogram.
+        """
+        return self._bins
+
+    @bins.setter
+    def bins(self, value: int):
+        """Sets the number of bins for the histogram."""
+        self._bins = value
+        self.data = self._data
+
+    @property
+    def histogram_colormap(self) -> Colormap:
+        """Gets or sets the colormap for the histogram.
+
+        Returns
+        -------
+        histogram_colormap : Colormap
+            colormap for the histogram.
+        """
+        return self._histogram_colormap
+
+    @histogram_colormap.setter
+    def histogram_colormap(self, value: Colormap):
+        """Sets the colormap for the histogram."""
+        self._histogram_colormap = value
+        self.data = self._data
+
+    @property
+    def histogram(self) -> Tuple[np.ndarray, np.ndarray, np.ndarray, QuadMesh]:
+        """Returns the 2D histogram matplotlib object.
+
+        Returns
+        -------
+        histogram : Tuple[np.ndarray, np.ndarray, np.ndarray, QuadMesh]
+            2D histogram matplotlib object.
+        """
+        return self._histogram
+
+    def indices_in_above_threshold_patches(self, threshold: int) -> List[int]:
+        """
+        Returns the indices of the points in that fall into the bins
+        of the 2D histogram exceeding a specified threshold.
+
+        Parameters
+        ----------
+        threshold : int
+            The count threshold to exceed.
+
+        Returns
+        -------
+        indices : List[int]
+            list of indices of points falling into the exceeding bins.
+        """
+        counts, xedges, yedges, _ = self._histogram
+
+        # Identify bins that exceed the threshold
+        exceeding_bins = np.argwhere(counts > threshold)
+
+        # Prepare to collect indices
+        indices = []
+
+        # For each bin exceeding the threshold...
+        for bin_x, bin_y in exceeding_bins:
+            # Identify the edges of the current bin
+            x_min, x_max = xedges[bin_x], xedges[bin_x + 1]
+            y_min, y_max = yedges[bin_y], yedges[bin_y + 1]
+
+            # Find indices of points within these edges
+            bin_indices = np.where((self._data[:, 0] >= x_min) & (self._data[:, 0] < x_max) & (
+                self._data[:, 1] >= y_min) & (self._data[:, 1] < y_max))[0]
+            indices.extend(bin_indices)
+
+        return indices
+
+    def draw(self):
+        """Draws or redraws the 2D histogram."""
+        self.ax.figure.canvas.draw_idle()
```

### Comparing `biaplotter-0.0.1/src/biaplotter/plotter.py` & `biaplotter-0.0.2/src/biaplotter/plotter.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,265 +1,265 @@
-from __future__ import annotations
-
-from pathlib import Path
-from enum import Enum, auto
-from nap_plot_tools import CustomToolbarWidget, QtColorSpinBox
-from napari.layers import Labels, Points, Tracks
-from napari_matplotlib.base import BaseNapariMPLWidget
-from napari_matplotlib.util import Interval
-from qtpy.QtWidgets import QHBoxLayout, QLabel, QWidget
-from psygnal import Signal
-from typing import Union, TYPE_CHECKING, Optional
-
-from biaplotter.artists import Scatter, Histogram2D
-from biaplotter.selectors import InteractiveRectangleSelector, InteractiveEllipseSelector, InteractiveLassoSelector
-
-if TYPE_CHECKING:
-    import napari
-
-icon_folder_path = (
-    Path(__file__).parent / "icons"
-)
-
-
-class ArtistType(Enum):
-    HISTOGRAM2D = auto()
-    SCATTER = auto()
-
-
-class SelectorType(Enum):
-    LASSO = auto()
-    ELLIPSE = auto()
-    RECTANGLE = auto()
-
-
-class CanvasWidget(BaseNapariMPLWidget):
-    """A widget that contains a canvas with matplotlib axes and a selection toolbar.
-
-    The widget includes a selection toolbar with buttons to enable/disable selection tools.
-    The selection toolbar includes a color class spinbox to select the class to assign to selections.
-    The widget includes artists and selectors to plot data and select points.
-
-    Parameters
-    ----------
-    napari_viewer : napari.viewer.Viewer
-        The napari viewer.
-    parent : QWidget, optional
-        The parent widget, by default None.
-    label_text : str, optional
-        The text to display next to the class spinbox, by default "Class:".
-
-    Notes
-    -----
-
-    Signals:
-
-        * **artist_changed_signal** emitted when the current artist changes.
-
-    Signals and Slots:
-
-        This class automatically connects the following signals to slots:
-
-        * **data_changed_signal** from each artist to the **update_data** slot in each selector. This allows artists to notify selectors when the data changes. Selectors can then synchronize their data with the artist's data.  
-    """
-
-    #: Signal emitted when the current `active_artist` changes
-    artist_changed_signal: Signal = Signal(ArtistType)
-
-    def __init__(self, napari_viewer: "napari.viewer.Viewer", parent: Optional[QWidget] = None, label_text: str = "Class:"):
-        super().__init__(napari_viewer, parent=parent)
-        self.add_single_axes()
-        # Add selection tools layout below canvas
-        selection_tools_layout, selection_toolbar, class_spinbox = self._build_selection_toolbar_layout(
-            label_text=label_text)
-        #: The selection tools layout.
-        self.selection_tools_layout: QHBoxLayout = selection_tools_layout
-        #: The selection toolbar.
-        self.selection_toolbar: CustomToolbarWidget = selection_toolbar
-        #: The color class spinbox.
-        self.class_spinbox: QtColorSpinBox = class_spinbox
-        # Add button to selection_toolbar
-        self.selection_toolbar.add_custom_button(
-            name=SelectorType.LASSO.name,
-            tooltip="Click to enable/disable Lasso selection",
-            default_icon_path=icon_folder_path / "lasso.png",
-            checkable=True,
-            checked_icon_path=icon_folder_path / "lasso_checked.png",
-            callback=self.on_enable_selector,
-        )
-        # Add button to selection_toolbar
-        self.selection_toolbar.add_custom_button(
-            name=SelectorType.ELLIPSE.name,
-            tooltip="Click to enable/disable Ellipse selection",
-            default_icon_path=icon_folder_path / "ellipse.png",
-            checkable=True,
-            checked_icon_path=icon_folder_path / "ellipse_checked.png",
-            callback=self.on_enable_selector,
-        )
-        # Add button to selection_toolbar
-        self.selection_toolbar.add_custom_button(
-            name=SelectorType.RECTANGLE.name,
-            tooltip="Click to enable/disable Rectangle selection",
-            default_icon_path=icon_folder_path / "rectangle.png",
-            checkable=True,
-            checked_icon_path=icon_folder_path / "rectangle_checked.png",
-            callback=self.on_enable_selector,
-        )
-
-        # Add selection tools layout to main layout below matplotlib toolbar and above canvas
-        self.layout().insertLayout(1, self.selection_tools_layout)
-
-        # Create artists
-        #: Stores the active artist.
-        self._active_artist: Scatter | Histogram2D = None
-        #: Dictionary of artists.
-        self.artists: dict = {}
-        self.add_artist(ArtistType.SCATTER, Scatter(ax=self.axes))
-        self.add_artist(ArtistType.HISTOGRAM2D, Histogram2D(ax=self.axes))
-        # Set histogram2d as the default artist
-        self.active_artist = self.artists[ArtistType.HISTOGRAM2D]
-
-        # Create selectors
-        #: Dictionary of selectors.
-        self.selectors: dict = {}
-        self.add_selector(SelectorType.LASSO, InteractiveLassoSelector(
-            ax=self.axes, canvas_widget=self))
-        self.add_selector(SelectorType.ELLIPSE, InteractiveEllipseSelector(
-            ax=self.axes, canvas_widget=self))
-        self.add_selector(SelectorType.RECTANGLE,
-                          InteractiveRectangleSelector(self.axes, self))
-        # Connect data_changed signals from each artist to set data in each selector
-        for artist in self.artists.values():
-            for selector in self.selectors.values():
-                artist.data_changed_signal.connect(selector.update_data)
-
-    def _build_selection_toolbar_layout(self, label_text: str = "Class:"):
-        """Builds the selection toolbar layout.
-
-        The toolbar starts without any buttons. Add buttons using the add_custom_button method.
-        The toolbar includes a color class spinbox to select the class to assign to selections.
-
-        Parameters
-        ----------
-        label_text : str, optional
-            The text to display next to the class spinbox, by default "Class:"
-
-        Returns
-        -------
-        selection_tools_layout : QHBoxLayout
-            The selection tools layout.
-        selection_toolbar : CustomToolbarWidget
-            The toolbar widget
-        class_spinbox : QtColorSpinBox
-            The color class spinbox.
-        """
-        # Add selection tools layout below canvas
-        selection_tools_layout = QHBoxLayout()
-        # Add selection toolbar
-        selection_toolbar = CustomToolbarWidget(self)
-        selection_tools_layout.addWidget(selection_toolbar)
-        # Add class spinbox
-        selection_tools_layout.addWidget(QLabel(label_text))
-        # Add color class spinbox
-        class_spinbox = QtColorSpinBox(first_color_transparent=False)
-        selection_tools_layout.addWidget(class_spinbox)
-        # Add stretch to the right to push buttons to the left
-        selection_tools_layout.addStretch(1)
-        return selection_tools_layout, selection_toolbar, class_spinbox
-
-    def on_enable_selector(self, checked: bool):
-        """Enables or disables the selected selector.
-
-        Enabling a selector disables all other selectors.
-
-        Parameters
-        ----------
-        checked : bool
-            Whether the button is checked or not.
-        """
-        sender_name = self.sender().text()
-        if checked:
-            # If the button is checked, disable all other buttons
-            for button_name, button in self.selection_toolbar.buttons.items():
-                if button.isChecked() and button_name != sender_name:
-                    button.setChecked(False)
-            # Remove all selectors
-            for selector in self.selectors.values():
-                selector.selected_indices = None
-                selector.remove()
-            # Create the chosen selector
-            for selector_type, selector in self.selectors.items():
-                if selector_type.name == sender_name:
-                    selector.create_selector()
-        else:
-            # If the button is unchecked, remove the selector
-            for selector_type, selector in self.selectors.items():
-                if selector_type.name == sender_name:
-                    selector.selected_indices = None
-                    selector.remove()
-
-    @property
-    def active_artist(self):
-        """Sets or returns the active artist.
-
-        If set, makes the selected artist visible and all other artists invisible.
-
-        Returns
-        -------
-        Scatter or Histogram2D
-            The active artist.
-
-        Notes
-        -----
-        artist_changed_signal : Signal
-            Signal emitted when the current artist changes.
-        """
-        return self._active_artist
-
-    @active_artist.setter
-    def active_artist(self, value: Scatter | Histogram2D):
-        """Sets the active artist.
-        """
-        self._active_artist = value
-        for artist in self.artists.values():
-            if artist == self._active_artist:
-                artist.visible = True
-            else:
-                artist.visible = False
-        # Gets artist type
-        for artist_type, artist in self.artists.items():
-            if artist == value:
-                active_artist_type = artist_type
-        # Emit signal to notify that the current artist has changed
-        self.artist_changed_signal.emit(active_artist_type)
-
-    def add_artist(self, artist_type: ArtistType, artist_instance: Scatter | Histogram2D, visible: bool = False):
-        """
-        Adds a new artist instance to the artists dictionary.
-
-        Parameters
-        ----------
-        artist_type : ArtistType
-            The type of the artist, defined by the ArtistType enum.
-        artist_instance : Scatter or Histogram2D
-            An instance of the artist class.
-        """
-        if artist_type in self.artists:
-            raise ValueError(f"Artist '{artist_type.name}' already exists.")
-        self.artists[artist_type] = artist_instance
-        artist_instance.visible = visible
-
-    def add_selector(self, selector_type: SelectorType, selector_instance: InteractiveRectangleSelector | InteractiveEllipseSelector | InteractiveLassoSelector):
-        """
-        Adds a new selector instance to the selectors dictionary.
-
-        Parameters
-        ----------
-        selector_type : SelectorType
-            The type of the selector, defined by the SelectorType enum.
-        selector_instance : InteractiveRectangleSelector or InteractiveEllipseSelector or InteractiveLassoSelector
-            An instance of the selector class.
-        """
-        if selector_type in self.selectors:
-            raise ValueError(
-                f"Selector '{selector_type.name}' already exists.")
-        self.selectors[selector_type] = selector_instance
+from __future__ import annotations
+
+from pathlib import Path
+from enum import Enum, auto
+from nap_plot_tools import CustomToolbarWidget, QtColorSpinBox
+from napari.layers import Labels, Points, Tracks
+from napari_matplotlib.base import BaseNapariMPLWidget
+from napari_matplotlib.util import Interval
+from qtpy.QtWidgets import QHBoxLayout, QLabel, QWidget
+from psygnal import Signal
+from typing import Union, TYPE_CHECKING, Optional
+
+from biaplotter.artists import Scatter, Histogram2D
+from biaplotter.selectors import InteractiveRectangleSelector, InteractiveEllipseSelector, InteractiveLassoSelector
+
+if TYPE_CHECKING:
+    import napari
+
+icon_folder_path = (
+    Path(__file__).parent / "icons"
+)
+
+
+class ArtistType(Enum):
+    HISTOGRAM2D = auto()
+    SCATTER = auto()
+
+
+class SelectorType(Enum):
+    LASSO = auto()
+    ELLIPSE = auto()
+    RECTANGLE = auto()
+
+
+class CanvasWidget(BaseNapariMPLWidget):
+    """A widget that contains a canvas with matplotlib axes and a selection toolbar.
+
+    The widget includes a selection toolbar with buttons to enable/disable selection tools.
+    The selection toolbar includes a color class spinbox to select the class to assign to selections.
+    The widget includes artists and selectors to plot data and select points.
+
+    Parameters
+    ----------
+    napari_viewer : napari.viewer.Viewer
+        The napari viewer.
+    parent : QWidget, optional
+        The parent widget, by default None.
+    label_text : str, optional
+        The text to display next to the class spinbox, by default "Class:".
+
+    Notes
+    -----
+
+    Signals:
+
+        * **artist_changed_signal** emitted when the current artist changes.
+
+    Signals and Slots:
+
+        This class automatically connects the following signals to slots:
+
+        * **data_changed_signal** from each artist to the **update_data** slot in each selector. This allows artists to notify selectors when the data changes. Selectors can then synchronize their data with the artist's data.  
+    """
+
+    #: Signal emitted when the current `active_artist` changes
+    artist_changed_signal: Signal = Signal(ArtistType)
+
+    def __init__(self, napari_viewer: "napari.viewer.Viewer", parent: Optional[QWidget] = None, label_text: str = "Class:"):
+        super().__init__(napari_viewer, parent=parent)
+        self.add_single_axes()
+        # Add selection tools layout below canvas
+        selection_tools_layout, selection_toolbar, class_spinbox = self._build_selection_toolbar_layout(
+            label_text=label_text)
+        #: The selection tools layout.
+        self.selection_tools_layout: QHBoxLayout = selection_tools_layout
+        #: The selection toolbar.
+        self.selection_toolbar: CustomToolbarWidget = selection_toolbar
+        #: The color class spinbox.
+        self.class_spinbox: QtColorSpinBox = class_spinbox
+        # Add button to selection_toolbar
+        self.selection_toolbar.add_custom_button(
+            name=SelectorType.LASSO.name,
+            tooltip="Click to enable/disable Lasso selection",
+            default_icon_path=icon_folder_path / "lasso.png",
+            checkable=True,
+            checked_icon_path=icon_folder_path / "lasso_checked.png",
+            callback=self.on_enable_selector,
+        )
+        # Add button to selection_toolbar
+        self.selection_toolbar.add_custom_button(
+            name=SelectorType.ELLIPSE.name,
+            tooltip="Click to enable/disable Ellipse selection",
+            default_icon_path=icon_folder_path / "ellipse.png",
+            checkable=True,
+            checked_icon_path=icon_folder_path / "ellipse_checked.png",
+            callback=self.on_enable_selector,
+        )
+        # Add button to selection_toolbar
+        self.selection_toolbar.add_custom_button(
+            name=SelectorType.RECTANGLE.name,
+            tooltip="Click to enable/disable Rectangle selection",
+            default_icon_path=icon_folder_path / "rectangle.png",
+            checkable=True,
+            checked_icon_path=icon_folder_path / "rectangle_checked.png",
+            callback=self.on_enable_selector,
+        )
+
+        # Add selection tools layout to main layout below matplotlib toolbar and above canvas
+        self.layout().insertLayout(1, self.selection_tools_layout)
+
+        # Create artists
+        #: Stores the active artist.
+        self._active_artist: Scatter | Histogram2D = None
+        #: Dictionary of artists.
+        self.artists: dict = {}
+        self.add_artist(ArtistType.SCATTER, Scatter(ax=self.axes))
+        self.add_artist(ArtistType.HISTOGRAM2D, Histogram2D(ax=self.axes))
+        # Set histogram2d as the default artist
+        self.active_artist = self.artists[ArtistType.HISTOGRAM2D]
+
+        # Create selectors
+        #: Dictionary of selectors.
+        self.selectors: dict = {}
+        self.add_selector(SelectorType.LASSO, InteractiveLassoSelector(
+            ax=self.axes, canvas_widget=self))
+        self.add_selector(SelectorType.ELLIPSE, InteractiveEllipseSelector(
+            ax=self.axes, canvas_widget=self))
+        self.add_selector(SelectorType.RECTANGLE,
+                          InteractiveRectangleSelector(self.axes, self))
+        # Connect data_changed signals from each artist to set data in each selector
+        for artist in self.artists.values():
+            for selector in self.selectors.values():
+                artist.data_changed_signal.connect(selector.update_data)
+
+    def _build_selection_toolbar_layout(self, label_text: str = "Class:"):
+        """Builds the selection toolbar layout.
+
+        The toolbar starts without any buttons. Add buttons using the add_custom_button method.
+        The toolbar includes a color class spinbox to select the class to assign to selections.
+
+        Parameters
+        ----------
+        label_text : str, optional
+            The text to display next to the class spinbox, by default "Class:"
+
+        Returns
+        -------
+        selection_tools_layout : QHBoxLayout
+            The selection tools layout.
+        selection_toolbar : CustomToolbarWidget
+            The toolbar widget
+        class_spinbox : QtColorSpinBox
+            The color class spinbox.
+        """
+        # Add selection tools layout below canvas
+        selection_tools_layout = QHBoxLayout()
+        # Add selection toolbar
+        selection_toolbar = CustomToolbarWidget(self)
+        selection_tools_layout.addWidget(selection_toolbar)
+        # Add class spinbox
+        selection_tools_layout.addWidget(QLabel(label_text))
+        # Add color class spinbox
+        class_spinbox = QtColorSpinBox(first_color_transparent=False)
+        selection_tools_layout.addWidget(class_spinbox)
+        # Add stretch to the right to push buttons to the left
+        selection_tools_layout.addStretch(1)
+        return selection_tools_layout, selection_toolbar, class_spinbox
+
+    def on_enable_selector(self, checked: bool):
+        """Enables or disables the selected selector.
+
+        Enabling a selector disables all other selectors.
+
+        Parameters
+        ----------
+        checked : bool
+            Whether the button is checked or not.
+        """
+        sender_name = self.sender().text()
+        if checked:
+            # If the button is checked, disable all other buttons
+            for button_name, button in self.selection_toolbar.buttons.items():
+                if button.isChecked() and button_name != sender_name:
+                    button.setChecked(False)
+            # Remove all selectors
+            for selector in self.selectors.values():
+                selector.selected_indices = None
+                selector.remove()
+            # Create the chosen selector
+            for selector_type, selector in self.selectors.items():
+                if selector_type.name == sender_name:
+                    selector.create_selector()
+        else:
+            # If the button is unchecked, remove the selector
+            for selector_type, selector in self.selectors.items():
+                if selector_type.name == sender_name:
+                    selector.selected_indices = None
+                    selector.remove()
+
+    @property
+    def active_artist(self):
+        """Sets or returns the active artist.
+
+        If set, makes the selected artist visible and all other artists invisible.
+
+        Returns
+        -------
+        Scatter or Histogram2D
+            The active artist.
+
+        Notes
+        -----
+        artist_changed_signal : Signal
+            Signal emitted when the current artist changes.
+        """
+        return self._active_artist
+
+    @active_artist.setter
+    def active_artist(self, value: Scatter | Histogram2D):
+        """Sets the active artist.
+        """
+        self._active_artist = value
+        for artist in self.artists.values():
+            if artist == self._active_artist:
+                artist.visible = True
+            else:
+                artist.visible = False
+        # Gets artist type
+        for artist_type, artist in self.artists.items():
+            if artist == value:
+                active_artist_type = artist_type
+        # Emit signal to notify that the current artist has changed
+        self.artist_changed_signal.emit(active_artist_type)
+
+    def add_artist(self, artist_type: ArtistType, artist_instance: Scatter | Histogram2D, visible: bool = False):
+        """
+        Adds a new artist instance to the artists dictionary.
+
+        Parameters
+        ----------
+        artist_type : ArtistType
+            The type of the artist, defined by the ArtistType enum.
+        artist_instance : Scatter or Histogram2D
+            An instance of the artist class.
+        """
+        if artist_type in self.artists:
+            raise ValueError(f"Artist '{artist_type.name}' already exists.")
+        self.artists[artist_type] = artist_instance
+        artist_instance.visible = visible
+
+    def add_selector(self, selector_type: SelectorType, selector_instance: InteractiveRectangleSelector | InteractiveEllipseSelector | InteractiveLassoSelector):
+        """
+        Adds a new selector instance to the selectors dictionary.
+
+        Parameters
+        ----------
+        selector_type : SelectorType
+            The type of the selector, defined by the SelectorType enum.
+        selector_instance : InteractiveRectangleSelector or InteractiveEllipseSelector or InteractiveLassoSelector
+            An instance of the selector class.
+        """
+        if selector_type in self.selectors:
+            raise ValueError(
+                f"Selector '{selector_type.name}' already exists.")
+        self.selectors[selector_type] = selector_instance
```

### Comparing `biaplotter-0.0.1/src/biaplotter/selectors.py` & `biaplotter-0.0.2/src/biaplotter/selectors.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,532 +1,535 @@
-from __future__ import annotations  # Only necessary for Python 3.7 to 3.9
-
-import numpy as np
-import matplotlib.pyplot as plt
-
-from typing import TYPE_CHECKING
-from abc import ABC, abstractmethod
-from matplotlib.path import Path as mplPath
-from matplotlib.widgets import LassoSelector, RectangleSelector, EllipseSelector
-
-
-if TYPE_CHECKING:
-    from biaplotter.plotter import CanvasWidget
-
-
-class Selector(ABC):
-    """Abstract class for creating a selector.
-
-    Parameters
-    ----------
-    ax : plt.Axes, optional
-        axes to which the selector will be applied.
-    data : np.ndarray
-        data to be selected.
-    """
-
-    def __init__(self, ax: plt.Axes = None, data: np.ndarray = None):
-        """Initializes the selector.
-        """
-        #: Stores the axes to which the selector will be applied.
-        self.ax: plt.Axes = ax
-        #: Stores the data to be selected
-        self._data = data
-        #: Stores the selector
-        self._selector = None
-
-    @property
-    @abstractmethod
-    def data(self) -> np.ndarray:
-        """Abstract property for the selector's data."""
-        pass
-
-    @data.setter
-    @abstractmethod
-    def data(self, value: np.ndarray):
-        """Abstract setter for the selector's data."""
-        pass
-
-    @abstractmethod
-    def create_selector(self):
-        """Abstract method to create a selector."""
-        pass
-
-    @abstractmethod
-    def on_select(self, vertices: np.ndarray):
-        """Abstract method to select points based on the selector's shape."""
-        pass
-
-    def remove(self):
-        """Removes the selector from the canvas."""
-        if self._selector:
-            self._selector.clear()
-            self._selector.disconnect_events()
-            self._selector = None
-
-
-class BaseRectangleSelector(Selector):
-    """Base class for creating a rectangle selector.	
-
-    Inherits all parameters and attributes from Selector.
-    For parameter and attribute details, see the Selector class documentation.
-
-    Parameters
-    ----------
-    ax : plt.Axes
-        axes to which the selector will be applied.
-    data : (N, 2) np.ndarray
-        data to be selected.
-  
-    """
-
-    def __init__(self, ax: plt.Axes, data: np.ndarray = None):
-        """Initializes the rectangle selector.
-        """
-        super().__init__(ax, data)
-        #: The name of the selector, set to 'Rectangle Selector' by default.
-        self.name: str = 'Rectangle Selector'
-        self.data = data
-
-    def on_select(self, eclick, erelease) -> np.ndarray:
-        """Selects points within the rectangle and returns their indices.
-        
-        Parameters
-        ----------
-        eclick : MouseEvent
-            The press event.
-        erelease : MouseEvent
-            The release event.
-
-        Returns
-        -------
-        np.ndarray
-            The indices of the selected points.
-        """
-        if self._data is None or len(self._data) == 0:
-            return
-        x1, y1 = eclick.xdata, eclick.ydata
-        x2, y2 = erelease.xdata, erelease.ydata
-        mask = (self._data[:, 0] >= min(x1, x2)) & (self._data[:, 0] <= max(x1, x2)) & (
-            self._data[:, 1] >= min(y1, y2)) & (self._data[:, 1] <= max(y1, y2))
-        indices = np.where(mask)[0]
-        return indices
-
-    @property
-    def data(self) -> np.ndarray:
-        """Gets or sets the data from which points will be selected."""
-        return self._data
-
-    @data.setter
-    def data(self, value: np.ndarray):
-        """Sets the data from which points will be selected."""
-        self._data = value
-
-    def create_selector(self):
-        """Creates a rectangle selector.
-
-        Useblit is set to True to improve performance.
-        Left mouse button is used to draw the rectangle.
-        Minimum span in x and y is set to 5 pixels.
-        Span coordinates are set to pixels.
-        Interactive is set to True to allow for interaction.
-        Drag from anywhere is set to True to allow for drawing from any point.
-        """
-        self._selector = RectangleSelector(self.ax, self.on_select, useblit=True, button=[
-                                           1], minspanx=5, minspany=5, spancoords='pixels', interactive=True, drag_from_anywhere=True)
-
-
-class BaseEllipseSelector(Selector):
-    """Base class for creating an ellipse selector.
-
-    Inherits all parameters and attributes from Selector.
-    For parameter and attribute details, see the Selector class documentation.
-
-    Parameters
-    ----------
-    ax : plt.Axes
-        axes to which the selector will be applied.
-    data : np.ndarray
-        data to be selected.
-
-    """
-
-    def __init__(self, ax: plt.Axes, data: np.ndarray = None):
-        """Initializes the ellipse selector.
-        """
-        super().__init__(ax, data)
-        #: The name of the selector, set to 'Ellipse Selector' by default.
-        self.name: str = 'Ellipse Selector'
-        self.data = data
-
-    def on_select(self, eclick, erelease):
-        """Selects points within the ellipse and returns their indices.
-        
-        Parameters
-        ----------
-        eclick : MouseEvent
-            The press event.
-        erelease : MouseEvent
-            The release event.
-            
-        Returns
-        -------
-        np.ndarray
-            The indices of the selected points."""
-        if self._data is None or len(self._data) == 0:
-            return
-        center = np.array([(eclick.xdata + erelease.xdata) / 2,
-                          (eclick.ydata + erelease.ydata) / 2])
-        width = abs(eclick.xdata - erelease.xdata)
-        height = abs(eclick.ydata - erelease.ydata)
-        mask = (((self._data[:, 0] - center[0]) / (width / 2))**2 +
-                ((self._data[:, 1] - center[1]) / (height / 2))**2) <= 1
-        indices = np.where(mask)[0]
-        return indices
-
-    @property
-    def data(self) -> np.ndarray:
-        """Gets or sets the data from which points will be selected."""
-        return self._data
-
-    @data.setter
-    def data(self, value: np.ndarray):
-        """Sets the data from which points will be selected."""
-        self._data = value
-
-    def create_selector(self):
-        """Creates an ellipse selector.
-
-        Useblit is set to True to improve performance.
-        Left mouse button is used to draw the ellipse.
-        Minimum span in x and y is set to 5 pixels.
-        Span coordinates are set to pixels.
-        Interactive is set to True to allow for interaction.
-        Drag from anywhere is set to True to allow for drawing from any point.
-        """
-        self._selector = EllipseSelector(self.ax, self.on_select, useblit=True, button=[
-            1], minspanx=5, minspany=5, spancoords='pixels', interactive=True, drag_from_anywhere=True)
-
-
-class BaseLassoSelector(Selector):
-    """Base class for creating a lasso selector.
-
-    Inherits all parameters and attributes from Selector.
-    For parameter and attribute details, see the Selector class documentation.
-
-    Parameters
-    ----------
-    ax : plt.Axes
-        axes to which the selector will be applied.
-    data : np.ndarray
-        data to be selected.
-
-    """
-    def __init__(self, ax: plt.Axes, data: np.ndarray = None):
-        super().__init__(ax, data)
-        #: The name of the selector, set to 'Lasso Selector' by default.
-        self.name: str = 'Lasso Selector'
-        self.data = data
-
-    def on_select(self, vertices):
-        """Selects points within the lasso and returns their indices.	
-
-        Parameters
-        ----------
-        vertices : np.ndarray
-            The vertices of the lasso.
-
-        Returns
-        -------
-        np.ndarray
-            The indices of the selected points.
-        """
-        if self._data is None or len(self._data) == 0:
-            return
-        path = mplPath(vertices)
-        mask = path.contains_points(self._data)
-        indices = np.where(mask)[0]
-        return indices
-
-    @property
-    def data(self) -> np.ndarray:
-        """Gets or sets the data from which points will be selected."""
-        return self._data
-
-    @data.setter
-    def data(self, value: np.ndarray):
-        """Sets the data from which points will be selected."""
-        self._data = value
-
-    def create_selector(self):
-        """Creates a lasso selector.
-
-        Useblit is set to True to improve performance.
-        Left mouse button is used to draw the lasso.
-        """
-        self._selector = LassoSelector(self.ax, self.on_select, useblit=True, button=[
-            1], props={'color': 'r', 'linestyle': '--'})
-
-
-class Interactive(Selector):
-    """Interactive selector class.
-
-    Inherits all parameters and attributes from Selector.
-    To be used as a base class together with a selector to turn selectors interactive.
-
-    Parameters
-    ----------
-    ax : plt.Axes
-        axes to which the selector will be applied.
-    canvas_widget : CanvasWidget
-        canvas widget to which the selector will be applied.
-    data : (N, 2) np.ndarray, optional
-        data to be selected.
-
-    Notes
-    -----
-    **Slots:**
-
-        * **update_class_value** method intended to be connected by the **color_spinbox_value_changed_signal** emitted by the canvas_widget to have class_value synchronized.
-        * **update_data** method intended to be connected by the **data_changed_signal** emitted by the active_artist to have the selector data synchronized.
-        * **update_active_artist** method intended to be connected by the **artist_changed_signal** emitted by the canvas_widget to have the active_artist synchronized.
-
-    **Signals and Slots:**
-
-        This class automatically connects the following signals to slots:
-
-        * **color_spinbox_value_changed_signal** emitted by the canvas_widget to **update_class_value** slot.
-        * **data_changed_signal** emitted by the active_artist to **update_data** slot.
-
-    """
-
-    def __init__(self, ax: plt.Axes, canvas_widget: "CanvasWidget", data: np.ndarray = None):
-        """Initializes the interactive rectangle selector.
-        """
-        super().__init__(ax, data)
-        #: The canvas widget to which the selector will be applied.
-        self.canvas_widget: "CanvasWidget" = canvas_widget
-
-        self._selected_indices = None  # To store indices of selected points
-        # Get initial class value
-        self._class_value = self.canvas_widget.class_spinbox.value
-        # Get initial active artist
-        self._active_artist = self.canvas_widget.active_artist
-
-        # Connect external signals to internal slots
-        # Connect class_spinbox_value_changed signal (emitted by colorspinbox when its value changes) to update current_class_value
-        self.canvas_widget.class_spinbox.color_spinbox_value_changed_signal.connect(
-            self.update_class_value)
-        # Connect artist_changed_signal (emitted by canvas widget when the current artist changes) to update active_artist
-        self.canvas_widget.artist_changed_signal.connect(
-            self.update_active_artist)
-
-    @property
-    def class_value(self):
-        """Gets or sets the current class value."""
-        return self._class_value
-
-    @class_value.setter
-    def class_value(self, value: int):
-        """Sets the current class value."""
-        self._class_value = value
-
-    @property
-    def active_artist(self):
-        """Gets or sets the active artist."""
-        return self._active_artist
-    
-    @active_artist.setter
-    def active_artist(self, value):
-        """Sets the active artist."""
-        self._active_artist = value
-
-    @property
-    def selected_indices(self):
-        """Gets or sets the indices of the selected points."""
-        return self._selected_indices
-
-    @selected_indices.setter
-    def selected_indices(self, value: np.ndarray):
-        """Sets the indices of the selected points."""
-        self._selected_indices = value
-
-    def create_selector(self):
-        """Creates the selector and connects the button press event."""
-        super().create_selector()
-        self.canvas_widget.canvas.mpl_connect(
-            'button_press_event', self.on_button_press)
-
-    def remove(self):
-        """Removes the selector from the canvas and disconnects the button press event."""
-        super().remove()
-        self.canvas_widget.canvas.mpl_disconnect(self.canvas_widget.canvas.mpl_connect(
-            'button_press_event', self.on_button_press))
-        
-    def apply_selection(self):
-        """Applies the selection to the data, updating the colors."""
-        if self._selected_indices is not None:
-            if len(self._selected_indices) > 0:
-                color_indices = self._active_artist.color_indices
-                color_indices[self._selected_indices] = self._class_value
-                self._active_artist.color_indices = color_indices
-            self._selected_indices = None
-        # Remove selector and create a new one
-        self.remove()
-        self.create_selector()
-        
-    def on_button_press(self, event):
-        """Handles the button press event. Right-click applies the selection.
-        
-        Parameters
-        ----------
-        event : MouseEvent
-            The button press event."""
-        if event.button == 3:
-            self.apply_selection()
-
-    def update_class_value(self, value: int):
-        """Update the class value.
-        
-        Notes
-        -----
-        This slot is connected to the **color_spinbox_value_changed_signal** emitted by the canvas widget."""
-        self.class_value = value
-
-    def update_data(self, value: np.ndarray):
-        """Update the selector data.
-        
-        Notes
-        -----
-        This slot is connected to the **data_changed_signal** emitted by the active artist."""
-        self.data = value
-
-    def update_active_artist(self):
-        """Update the active artist.
-        
-        Notes
-        -----
-        This slot is connected to the **artist_changed_signal** emitted by the canvas widget."""
-        self.active_artist = self.canvas_widget.active_artist
-
-
-class InteractiveRectangleSelector(Interactive, BaseRectangleSelector):
-    """Interactive rectangle selector class.
-
-    Inherits all parameters and attributes from Interactive and BaseRectangleSelector.
-    To be used as an interactive rectangle selector.
-
-    Parameters
-    ----------
-    ax : plt.Axes
-        The axes to which the selector will be applied.
-    canvas_widget : biaplotter.plotter.CanvasWidget
-        The canvas widget to which the selector will be applied.
-    data : (N, 2) np.ndarray, optional
-        The data to be selected.
-
-    """
-
-    def __init__(self, ax: plt.Axes, canvas_widget: "CanvasWidget", data: np.ndarray = None):
-        """Initializes the interactive rectangle selector."""
-        super().__init__(ax, canvas_widget, data)
-        #: The name of the selector, set to 'Interactive Rectangle Selector' by default.
-        self.name: str = 'Interactive Rectangle Selector'
-
-    def on_select(self, eclick, erelease):
-        """Selects points within the rectangle and assigns them to selected indices.
-        
-        Parameters
-        ----------
-        eclick : MouseEvent
-            The press event.
-        erelease : MouseEvent
-            The release event.
-            
-        Returns
-        -------
-        np.ndarray
-            The indices of the selected points."""
-        self.selected_indices = super().on_select(eclick, erelease)
-
-
-class InteractiveEllipseSelector(Interactive, BaseEllipseSelector):
-    """Interactive ellipse selector class.
-
-    Inherits all parameters and attributes from Interactive and BaseEllipseSelector.
-    To be used as an interactive ellipse selector.
-
-    Parameters
-    ----------
-    ax : plt.Axes
-        The axes to which the selector will be applied.
-    canvas_widget : biaplotter.plotter.CanvasWidget
-        The canvas widget to which the selector will be applied.
-    data : (N, 2) np.ndarray, optional
-        The data to be selected.
-
-    """
-
-    def __init__(self, ax: plt.Axes, canvas_widget: "CanvasWidget", data: np.ndarray = None):
-        """Initializes the interactive ellipse selector."""
-        super().__init__(ax, canvas_widget, data)
-        #: The name of the selector, set to 'Interactive Ellipse Selector' by default.
-        self.name: str = 'Interactive Ellipse Selector'
-
-    def on_select(self, eclick, erelease):
-        """Selects points within the ellipse and assigns them to selected indices.
-        
-        Parameters
-        ----------
-        eclick : MouseEvent
-            The press event.
-        erelease : MouseEvent
-            The release event.
-            
-        Returns
-        -------
-        np.ndarray
-            The indices of the selected points."""
-        self.selected_indices = super().on_select(eclick, erelease)
-
-
-class InteractiveLassoSelector(Interactive, BaseLassoSelector):
-    """Interactive lasso selector class.
-
-    Inherits all parameters and attributes from Interactive and BaseLassoSelector.
-    To be used as an interactive lasso selector.
-
-    Parameters
-    ----------
-    ax : plt.Axes
-        The axes to which the selector will be applied.
-    canvas_widget : biaplotter.plotter.CanvasWidget
-        The canvas widget to which the selector will be applied.
-    data : (N, 2) np.ndarray, optional
-        The data to be selected.
-
-    Other Parameters
-    ----------------
-    name : str
-        The name of the selector, set to 'Interactive Lasso Selector' by default.
-    """
-
-    def __init__(self, ax: plt.Axes, canvas_widget: "CanvasWidget", data: np.ndarray = None):
-        """Initializes the interactive lasso selector."""
-        super().__init__(ax, canvas_widget, data)
-        #: The name of the selector, set to 'Interactive Lasso Selector' by default.
-        self.name: str = 'Interactive Lasso Selector'
-
-    def on_select(self, vertices: np.ndarray):
-        """Selects points within the lasso and assigns them the current class value, updating colors.
-        
-        Parameters
-        ----------
-        vertices : np.ndarray
-            The vertices of the lasso.
-            
-        Returns
-        -------
-        np.ndarray
-            The indices of the selected points."""
-        self.selected_indices = super().on_select(vertices)
-        self.apply_selection()
+from __future__ import annotations  # Only necessary for Python 3.7 to 3.9
+
+import numpy as np
+import matplotlib.pyplot as plt
+
+from typing import TYPE_CHECKING
+from abc import ABC, abstractmethod
+from matplotlib.path import Path as mplPath
+from matplotlib.widgets import LassoSelector, RectangleSelector, EllipseSelector
+
+
+if TYPE_CHECKING:
+    from biaplotter.plotter import CanvasWidget
+
+
+class Selector(ABC):
+    """Abstract class for creating a selector.
+
+    Parameters
+    ----------
+    ax : plt.Axes, optional
+        axes to which the selector will be applied.
+    data : np.ndarray
+        data to be selected.
+    """
+
+    def __init__(self, ax: plt.Axes = None, data: np.ndarray = None):
+        """Initializes the selector.
+        """
+        #: Stores the axes to which the selector will be applied.
+        self.ax: plt.Axes = ax
+        #: Stores the data to be selected
+        self._data = data
+        #: Stores the selector
+        self._selector = None
+
+    @property
+    @abstractmethod
+    def data(self) -> np.ndarray:
+        """Abstract property for the selector's data."""
+        pass
+
+    @data.setter
+    @abstractmethod
+    def data(self, value: np.ndarray):
+        """Abstract setter for the selector's data."""
+        pass
+
+    @abstractmethod
+    def create_selector(self):
+        """Abstract method to create a selector."""
+        pass
+
+    @abstractmethod
+    def on_select(self, vertices: np.ndarray):
+        """Abstract method to select points based on the selector's shape."""
+        pass
+
+    def remove(self):
+        """Removes the selector from the canvas."""
+        if self._selector:
+            self._selector.clear()
+            self._selector.disconnect_events()
+            self._selector = None
+
+
+class BaseRectangleSelector(Selector):
+    """Base class for creating a rectangle selector.	
+
+    Inherits all parameters and attributes from Selector.
+    For parameter and attribute details, see the Selector class documentation.
+
+    Parameters
+    ----------
+    ax : plt.Axes
+        axes to which the selector will be applied.
+    data : (N, 2) np.ndarray
+        data to be selected.
+
+    """
+
+    def __init__(self, ax: plt.Axes, data: np.ndarray = None):
+        """Initializes the rectangle selector.
+        """
+        super().__init__(ax, data)
+        #: The name of the selector, set to 'Rectangle Selector' by default.
+        self.name: str = 'Rectangle Selector'
+        self.data = data
+
+    def on_select(self, eclick, erelease) -> np.ndarray:
+        """Selects points within the rectangle and returns their indices.
+
+        Parameters
+        ----------
+        eclick : MouseEvent
+            The press event.
+        erelease : MouseEvent
+            The release event.
+
+        Returns
+        -------
+        np.ndarray
+            The indices of the selected points.
+        """
+        if self._data is None or len(self._data) == 0:
+            return
+        x1, y1 = eclick.xdata, eclick.ydata
+        x2, y2 = erelease.xdata, erelease.ydata
+        mask = (self._data[:, 0] >= min(x1, x2)) & (self._data[:, 0] <= max(x1, x2)) & (
+            self._data[:, 1] >= min(y1, y2)) & (self._data[:, 1] <= max(y1, y2))
+        indices = np.where(mask)[0]
+        return indices
+
+    @property
+    def data(self) -> np.ndarray:
+        """Gets or sets the data from which points will be selected."""
+        return self._data
+
+    @data.setter
+    def data(self, value: np.ndarray):
+        """Sets the data from which points will be selected."""
+        self._data = value
+
+    def create_selector(self):
+        """Creates a rectangle selector.
+
+        Useblit is set to True to improve performance.
+        Left mouse button is used to draw the rectangle.
+        Minimum span in x and y is set to 5 pixels.
+        Span coordinates are set to pixels.
+        Interactive is set to True to allow for interaction.
+        Drag from anywhere is set to True to allow for drawing from any point.
+        """
+        self._selector = RectangleSelector(self.ax, self.on_select, useblit=True, button=[
+                                           1], minspanx=5, minspany=5, spancoords='pixels', interactive=True, drag_from_anywhere=True,
+                                           props=dict(facecolor='#00c18c', edgecolor='#00c18c', alpha=0.3, fill=True, linewidth=2.5, linestyle='--'))
+
+
+class BaseEllipseSelector(Selector):
+    """Base class for creating an ellipse selector.
+
+    Inherits all parameters and attributes from Selector.
+    For parameter and attribute details, see the Selector class documentation.
+
+    Parameters
+    ----------
+    ax : plt.Axes
+        axes to which the selector will be applied.
+    data : np.ndarray
+        data to be selected.
+
+    """
+
+    def __init__(self, ax: plt.Axes, data: np.ndarray = None):
+        """Initializes the ellipse selector.
+        """
+        super().__init__(ax, data)
+        #: The name of the selector, set to 'Ellipse Selector' by default.
+        self.name: str = 'Ellipse Selector'
+        self.data = data
+
+    def on_select(self, eclick, erelease):
+        """Selects points within the ellipse and returns their indices.
+
+        Parameters
+        ----------
+        eclick : MouseEvent
+            The press event.
+        erelease : MouseEvent
+            The release event.
+
+        Returns
+        -------
+        np.ndarray
+            The indices of the selected points."""
+        if self._data is None or len(self._data) == 0:
+            return
+        center = np.array([(eclick.xdata + erelease.xdata) / 2,
+                          (eclick.ydata + erelease.ydata) / 2])
+        width = abs(eclick.xdata - erelease.xdata)
+        height = abs(eclick.ydata - erelease.ydata)
+        mask = (((self._data[:, 0] - center[0]) / (width / 2))**2 +
+                ((self._data[:, 1] - center[1]) / (height / 2))**2) <= 1
+        indices = np.where(mask)[0]
+        return indices
+
+    @property
+    def data(self) -> np.ndarray:
+        """Gets or sets the data from which points will be selected."""
+        return self._data
+
+    @data.setter
+    def data(self, value: np.ndarray):
+        """Sets the data from which points will be selected."""
+        self._data = value
+
+    def create_selector(self):
+        """Creates an ellipse selector.
+
+        Useblit is set to True to improve performance.
+        Left mouse button is used to draw the ellipse.
+        Minimum span in x and y is set to 5 pixels.
+        Span coordinates are set to pixels.
+        Interactive is set to True to allow for interaction.
+        Drag from anywhere is set to True to allow for drawing from any point.
+        """
+        self._selector = EllipseSelector(self.ax, self.on_select, useblit=True, button=[
+            1], minspanx=5, minspany=5, spancoords='pixels', interactive=True, drag_from_anywhere=True,
+            props=dict(facecolor='#00c18c', edgecolor='#00c18c', alpha=0.3, fill=True, linewidth=2.5, linestyle='--'))
+
+
+class BaseLassoSelector(Selector):
+    """Base class for creating a lasso selector.
+
+    Inherits all parameters and attributes from Selector.
+    For parameter and attribute details, see the Selector class documentation.
+
+    Parameters
+    ----------
+    ax : plt.Axes
+        axes to which the selector will be applied.
+    data : np.ndarray
+        data to be selected.
+
+    """
+
+    def __init__(self, ax: plt.Axes, data: np.ndarray = None):
+        super().__init__(ax, data)
+        #: The name of the selector, set to 'Lasso Selector' by default.
+        self.name: str = 'Lasso Selector'
+        self.data = data
+
+    def on_select(self, vertices):
+        """Selects points within the lasso and returns their indices.	
+
+        Parameters
+        ----------
+        vertices : np.ndarray
+            The vertices of the lasso.
+
+        Returns
+        -------
+        np.ndarray
+            The indices of the selected points.
+        """
+        if self._data is None or len(self._data) == 0:
+            return
+        path = mplPath(vertices)
+        mask = path.contains_points(self._data)
+        indices = np.where(mask)[0]
+        return indices
+
+    @property
+    def data(self) -> np.ndarray:
+        """Gets or sets the data from which points will be selected."""
+        return self._data
+
+    @data.setter
+    def data(self, value: np.ndarray):
+        """Sets the data from which points will be selected."""
+        self._data = value
+
+    def create_selector(self):
+        """Creates a lasso selector.
+
+        Useblit is set to True to improve performance.
+        Left mouse button is used to draw the lasso.
+        """
+        self._selector = LassoSelector(self.ax, self.on_select, useblit=True, button=[
+            1], props=dict(color='#05ffe2', linestyle='--', linewidth=2.5, alpha=0.6))
+
+
+class Interactive(Selector):
+    """Interactive selector class.
+
+    Inherits all parameters and attributes from Selector.
+    To be used as a base class together with a selector to turn selectors interactive.
+
+    Parameters
+    ----------
+    ax : plt.Axes
+        axes to which the selector will be applied.
+    canvas_widget : CanvasWidget
+        canvas widget to which the selector will be applied.
+    data : (N, 2) np.ndarray, optional
+        data to be selected.
+
+    Notes
+    -----
+    **Slots:**
+
+        * **update_class_value** method intended to be connected by the **color_spinbox_value_changed_signal** emitted by the canvas_widget to have class_value synchronized.
+        * **update_data** method intended to be connected by the **data_changed_signal** emitted by the active_artist to have the selector data synchronized.
+        * **update_active_artist** method intended to be connected by the **artist_changed_signal** emitted by the canvas_widget to have the active_artist synchronized.
+
+    **Signals and Slots:**
+
+        This class automatically connects the following signals to slots:
+
+        * **color_spinbox_value_changed_signal** emitted by the canvas_widget to **update_class_value** slot.
+        * **data_changed_signal** emitted by the active_artist to **update_data** slot.
+
+    """
+
+    def __init__(self, ax: plt.Axes, canvas_widget: "CanvasWidget", data: np.ndarray = None):
+        """Initializes the interactive rectangle selector.
+        """
+        super().__init__(ax, data)
+        #: The canvas widget to which the selector will be applied.
+        self.canvas_widget: "CanvasWidget" = canvas_widget
+
+        self._selected_indices = None  # To store indices of selected points
+        # Get initial class value
+        self._class_value = self.canvas_widget.class_spinbox.value
+        # Get initial active artist
+        self._active_artist = self.canvas_widget.active_artist
+
+        # Connect external signals to internal slots
+        # Connect class_spinbox_value_changed signal (emitted by colorspinbox when its value changes) to update current_class_value
+        self.canvas_widget.class_spinbox.color_spinbox_value_changed_signal.connect(
+            self.update_class_value)
+        # Connect artist_changed_signal (emitted by canvas widget when the current artist changes) to update active_artist
+        self.canvas_widget.artist_changed_signal.connect(
+            self.update_active_artist)
+
+    @property
+    def class_value(self):
+        """Gets or sets the current class value."""
+        return self._class_value
+
+    @class_value.setter
+    def class_value(self, value: int):
+        """Sets the current class value."""
+        self._class_value = value
+
+    @property
+    def active_artist(self):
+        """Gets or sets the active artist."""
+        return self._active_artist
+
+    @active_artist.setter
+    def active_artist(self, value):
+        """Sets the active artist."""
+        self._active_artist = value
+
+    @property
+    def selected_indices(self):
+        """Gets or sets the indices of the selected points."""
+        return self._selected_indices
+
+    @selected_indices.setter
+    def selected_indices(self, value: np.ndarray):
+        """Sets the indices of the selected points."""
+        self._selected_indices = value
+
+    def create_selector(self):
+        """Creates the selector and connects the button press event."""
+        super().create_selector()
+        self.canvas_widget.canvas.mpl_connect(
+            'button_press_event', self.on_button_press)
+
+    def remove(self):
+        """Removes the selector from the canvas and disconnects the button press event."""
+        super().remove()
+        self.canvas_widget.canvas.mpl_disconnect(self.canvas_widget.canvas.mpl_connect(
+            'button_press_event', self.on_button_press))
+
+    def apply_selection(self):
+        """Applies the selection to the data, updating the colors."""
+        if self._selected_indices is not None:
+            if len(self._selected_indices) > 0:
+                color_indices = self._active_artist.color_indices
+                color_indices[self._selected_indices] = self._class_value
+                self._active_artist.color_indices = color_indices
+            self._selected_indices = None
+        # Remove selector and create a new one
+        self.remove()
+        self.create_selector()
+
+    def on_button_press(self, event):
+        """Handles the button press event. Right-click applies the selection.
+
+        Parameters
+        ----------
+        event : MouseEvent
+            The button press event."""
+        if event.button == 3:
+            self.apply_selection()
+
+    def update_class_value(self, value: int):
+        """Update the class value.
+
+        Notes
+        -----
+        This slot is connected to the **color_spinbox_value_changed_signal** emitted by the canvas widget."""
+        self.class_value = value
+
+    def update_data(self, value: np.ndarray):
+        """Update the selector data.
+
+        Notes
+        -----
+        This slot is connected to the **data_changed_signal** emitted by the active artist."""
+        self.data = value
+
+    def update_active_artist(self):
+        """Update the active artist.
+
+        Notes
+        -----
+        This slot is connected to the **artist_changed_signal** emitted by the canvas widget."""
+        self.active_artist = self.canvas_widget.active_artist
+
+
+class InteractiveRectangleSelector(Interactive, BaseRectangleSelector):
+    """Interactive rectangle selector class.
+
+    Inherits all parameters and attributes from Interactive and BaseRectangleSelector.
+    To be used as an interactive rectangle selector.
+
+    Parameters
+    ----------
+    ax : plt.Axes
+        The axes to which the selector will be applied.
+    canvas_widget : biaplotter.plotter.CanvasWidget
+        The canvas widget to which the selector will be applied.
+    data : (N, 2) np.ndarray, optional
+        The data to be selected.
+
+    """
+
+    def __init__(self, ax: plt.Axes, canvas_widget: "CanvasWidget", data: np.ndarray = None):
+        """Initializes the interactive rectangle selector."""
+        super().__init__(ax, canvas_widget, data)
+        #: The name of the selector, set to 'Interactive Rectangle Selector' by default.
+        self.name: str = 'Interactive Rectangle Selector'
+
+    def on_select(self, eclick, erelease):
+        """Selects points within the rectangle and assigns them to selected indices.
+
+        Parameters
+        ----------
+        eclick : MouseEvent
+            The press event.
+        erelease : MouseEvent
+            The release event.
+
+        Returns
+        -------
+        np.ndarray
+            The indices of the selected points."""
+        self.selected_indices = super().on_select(eclick, erelease)
+
+
+class InteractiveEllipseSelector(Interactive, BaseEllipseSelector):
+    """Interactive ellipse selector class.
+
+    Inherits all parameters and attributes from Interactive and BaseEllipseSelector.
+    To be used as an interactive ellipse selector.
+
+    Parameters
+    ----------
+    ax : plt.Axes
+        The axes to which the selector will be applied.
+    canvas_widget : biaplotter.plotter.CanvasWidget
+        The canvas widget to which the selector will be applied.
+    data : (N, 2) np.ndarray, optional
+        The data to be selected.
+
+    """
+
+    def __init__(self, ax: plt.Axes, canvas_widget: "CanvasWidget", data: np.ndarray = None):
+        """Initializes the interactive ellipse selector."""
+        super().__init__(ax, canvas_widget, data)
+        #: The name of the selector, set to 'Interactive Ellipse Selector' by default.
+        self.name: str = 'Interactive Ellipse Selector'
+
+    def on_select(self, eclick, erelease):
+        """Selects points within the ellipse and assigns them to selected indices.
+
+        Parameters
+        ----------
+        eclick : MouseEvent
+            The press event.
+        erelease : MouseEvent
+            The release event.
+
+        Returns
+        -------
+        np.ndarray
+            The indices of the selected points."""
+        self.selected_indices = super().on_select(eclick, erelease)
+
+
+class InteractiveLassoSelector(Interactive, BaseLassoSelector):
+    """Interactive lasso selector class.
+
+    Inherits all parameters and attributes from Interactive and BaseLassoSelector.
+    To be used as an interactive lasso selector.
+
+    Parameters
+    ----------
+    ax : plt.Axes
+        The axes to which the selector will be applied.
+    canvas_widget : biaplotter.plotter.CanvasWidget
+        The canvas widget to which the selector will be applied.
+    data : (N, 2) np.ndarray, optional
+        The data to be selected.
+
+    Other Parameters
+    ----------------
+    name : str
+        The name of the selector, set to 'Interactive Lasso Selector' by default.
+    """
+
+    def __init__(self, ax: plt.Axes, canvas_widget: "CanvasWidget", data: np.ndarray = None):
+        """Initializes the interactive lasso selector."""
+        super().__init__(ax, canvas_widget, data)
+        #: The name of the selector, set to 'Interactive Lasso Selector' by default.
+        self.name: str = 'Interactive Lasso Selector'
+
+    def on_select(self, vertices: np.ndarray):
+        """Selects points within the lasso and assigns them the current class value, updating colors.
+
+        Parameters
+        ----------
+        vertices : np.ndarray
+            The vertices of the lasso.
+
+        Returns
+        -------
+        np.ndarray
+            The indices of the selected points."""
+        self.selected_indices = super().on_select(vertices)
+        self.apply_selection()
```

### Comparing `biaplotter-0.0.1/src/biaplotter.egg-info/PKG-INFO` & `biaplotter-0.0.2/src/biaplotter.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,134 +1,134 @@
-Metadata-Version: 2.1
-Name: biaplotter
-Version: 0.0.1
-Summary: A base napari plotter widget for interactive plotting
-Home-page: https://github.com/BiAPoL/biaplotter
-Author: Marcelo Leomil Zoccoler
-Author-email: marzoccoler@gmail.com
-License: BSD-3-Clause
-Project-URL: Bug Tracker, https://github.com/BiAPoL/biaplotter/issues
-Project-URL: Documentation, https://github.com/BiAPoL/biaplotter#README.md
-Project-URL: Source Code, https://github.com/BiAPoL/biaplotter
-Project-URL: User Support, https://github.com/BiAPoL/biaplotter/issues
-Classifier: Development Status :: 2 - Pre-Alpha
-Classifier: Framework :: napari
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: BSD License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Topic :: Scientific/Engineering :: Image Processing
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: numpy
-Requires-Dist: magicgui
-Requires-Dist: qtpy
-Requires-Dist: napari-matplotlib
-Requires-Dist: nap-plot-tools>=0.1.0
-Provides-Extra: testing
-Requires-Dist: tox; extra == "testing"
-Requires-Dist: pytest; extra == "testing"
-Requires-Dist: pytest-cov; extra == "testing"
-Requires-Dist: pytest-qt; extra == "testing"
-Requires-Dist: napari; extra == "testing"
-Requires-Dist: pyqt5; extra == "testing"
-
-# biaplotter
-
-[![License BSD-3](https://img.shields.io/pypi/l/biaplotter.svg?color=green)](https://github.com/BiAPoL/biaplotter/raw/main/LICENSE)
-[![PyPI](https://img.shields.io/pypi/v/biaplotter.svg?color=green)](https://pypi.org/project/biaplotter)
-[![Python Version](https://img.shields.io/pypi/pyversions/biaplotter.svg?color=green)](https://python.org)
-[![tests](https://github.com/BiAPoL/biaplotter/workflows/tests/badge.svg)](https://github.com/BiAPoL/biaplotter/actions)
-[![codecov](https://codecov.io/gh/BiAPoL/biaplotter/branch/main/graph/badge.svg)](https://codecov.io/gh/BiAPoL/biaplotter)
-[![napari hub](https://img.shields.io/endpoint?url=https://api.napari-hub.org/shields/biaplotter)](https://napari-hub.org/plugins/biaplotter)
-
-A base napari plotter widget for interactive plotting
-
-----------------------------------
-
-This [napari] plugin was generated with [Cookiecutter] using [@napari]'s [cookiecutter-napari-plugin] template.
-
-<!--
-Don't miss the full getting started guide to set up your new package:
-https://github.com/napari/cookiecutter-napari-plugin#getting-started
-
-and review the napari docs for plugin developers:
-https://napari.org/stable/plugins/index.html
--->
-
-## Documentation
-
-The full documentation with API and examples can be found [here](https://biapol.github.io/biaplotter/).
-
-## Installation
-
-* Make sure you have Python in your computer, e.g. download [miniforge](https://github.com/conda-forge/miniforge?tab=readme-ov-file#download).
-
-* Create a new environment, for example, like this:
-
-```
-mamba create --name biaplotter-env python=3.9
-```
-
-If you never used mamba/conda environments before, take a look at [this blog post](https://biapol.github.io/blog/mara_lampert/getting_started_with_mambaforge_and_python/readme.html).
-
-* **Activate** the new environment with `mamba`:
-
-```
-mamba activate biaplotter-env
-```
-
-* Install [napari](https://napari.org/stable/), e.g. via `mamba`:
-
-```
-mamba install -c conda-forge napari pyqt
-```
-
-Afterwards, install `biaplotter` via `pip`:
-
-```
-pip install biaplotter
-```
-
-To install latest development version :
-
-```
-pip install git+https://github.com/BiAPoL/biaplotter.git
-```
-
-
-## Contributing
-
-Contributions are very welcome. Tests can be run with [tox], please ensure
-the coverage at least stays the same before you submit a pull request.
-
-## License
-
-Distributed under the terms of the [BSD-3] license,
-"biaplotter" is free and open source software
-
-## Issues
-
-If you encounter any problems, please [file an issue] along with a detailed description.
-
-[napari]: https://github.com/napari/napari
-[Cookiecutter]: https://github.com/audreyr/cookiecutter
-[@napari]: https://github.com/napari
-[MIT]: http://opensource.org/licenses/MIT
-[BSD-3]: http://opensource.org/licenses/BSD-3-Clause
-[GNU GPL v3.0]: http://www.gnu.org/licenses/gpl-3.0.txt
-[GNU LGPL v3.0]: http://www.gnu.org/licenses/lgpl-3.0.txt
-[Apache Software License 2.0]: http://www.apache.org/licenses/LICENSE-2.0
-[Mozilla Public License 2.0]: https://www.mozilla.org/media/MPL/2.0/index.txt
-[cookiecutter-napari-plugin]: https://github.com/napari/cookiecutter-napari-plugin
-
-[file an issue]: https://github.com/BiAPoL/biaplotter/issues
-
-[napari]: https://github.com/napari/napari
-[tox]: https://tox.readthedocs.io/en/latest/
-[pip]: https://pypi.org/project/pip/
-[PyPI]: https://pypi.org/
+Metadata-Version: 2.1
+Name: biaplotter
+Version: 0.0.2
+Summary: A base napari plotter widget for interactive plotting
+Home-page: https://github.com/BiAPoL/biaplotter
+Author: Marcelo Leomil Zoccoler
+Author-email: marzoccoler@gmail.com
+License: BSD-3-Clause
+Project-URL: Bug Tracker, https://github.com/BiAPoL/biaplotter/issues
+Project-URL: Documentation, https://github.com/BiAPoL/biaplotter#README.md
+Project-URL: Source Code, https://github.com/BiAPoL/biaplotter
+Project-URL: User Support, https://github.com/BiAPoL/biaplotter/issues
+Classifier: Development Status :: 2 - Pre-Alpha
+Classifier: Framework :: napari
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: BSD License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Topic :: Scientific/Engineering :: Image Processing
+Requires-Python: >=3.9
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: numpy
+Requires-Dist: magicgui
+Requires-Dist: qtpy
+Requires-Dist: napari-matplotlib
+Requires-Dist: nap-plot-tools>=0.1.0
+Provides-Extra: testing
+Requires-Dist: tox; extra == "testing"
+Requires-Dist: pytest; extra == "testing"
+Requires-Dist: pytest-cov; extra == "testing"
+Requires-Dist: pytest-qt; extra == "testing"
+Requires-Dist: napari; extra == "testing"
+Requires-Dist: pyqt5; extra == "testing"
+
+# biaplotter
+
+[![License BSD-3](https://img.shields.io/pypi/l/biaplotter.svg?color=green)](https://github.com/BiAPoL/biaplotter/raw/main/LICENSE)
+[![PyPI](https://img.shields.io/pypi/v/biaplotter.svg?color=green)](https://pypi.org/project/biaplotter)
+[![Python Version](https://img.shields.io/pypi/pyversions/biaplotter.svg?color=green)](https://python.org)
+[![tests](https://github.com/BiAPoL/biaplotter/workflows/tests/badge.svg)](https://github.com/BiAPoL/biaplotter/actions)
+[![codecov](https://codecov.io/gh/BiAPoL/biaplotter/branch/main/graph/badge.svg)](https://codecov.io/gh/BiAPoL/biaplotter)
+[![napari hub](https://img.shields.io/endpoint?url=https://api.napari-hub.org/shields/biaplotter)](https://napari-hub.org/plugins/biaplotter)
+
+A base napari plotter widget for interactive plotting
+
+----------------------------------
+
+This [napari] plugin was generated with [Cookiecutter] using [@napari]'s [cookiecutter-napari-plugin] template.
+
+<!--
+Don't miss the full getting started guide to set up your new package:
+https://github.com/napari/cookiecutter-napari-plugin#getting-started
+
+and review the napari docs for plugin developers:
+https://napari.org/stable/plugins/index.html
+-->
+
+## Documentation
+
+The full documentation with API and examples can be found [here](https://biapol.github.io/biaplotter/).
+
+## Installation
+
+* Make sure you have Python in your computer, e.g. download [miniforge](https://github.com/conda-forge/miniforge?tab=readme-ov-file#download).
+
+* Create a new environment, for example, like this:
+
+```
+mamba create --name biaplotter-env python=3.9
+```
+
+If you never used mamba/conda environments before, take a look at [this blog post](https://biapol.github.io/blog/mara_lampert/getting_started_with_mambaforge_and_python/readme.html).
+
+* **Activate** the new environment with `mamba`:
+
+```
+mamba activate biaplotter-env
+```
+
+* Install [napari](https://napari.org/stable/), e.g. via `mamba`:
+
+```
+mamba install -c conda-forge napari pyqt
+```
+
+Afterwards, install `biaplotter` via `pip`:
+
+```
+pip install biaplotter
+```
+
+To install latest development version :
+
+```
+pip install git+https://github.com/BiAPoL/biaplotter.git
+```
+
+
+## Contributing
+
+Contributions are very welcome. Tests can be run with [tox], please ensure
+the coverage at least stays the same before you submit a pull request.
+
+## License
+
+Distributed under the terms of the [BSD-3] license,
+"biaplotter" is free and open source software
+
+## Issues
+
+If you encounter any problems, please [file an issue] along with a detailed description.
+
+[napari]: https://github.com/napari/napari
+[Cookiecutter]: https://github.com/audreyr/cookiecutter
+[@napari]: https://github.com/napari
+[MIT]: http://opensource.org/licenses/MIT
+[BSD-3]: http://opensource.org/licenses/BSD-3-Clause
+[GNU GPL v3.0]: http://www.gnu.org/licenses/gpl-3.0.txt
+[GNU LGPL v3.0]: http://www.gnu.org/licenses/lgpl-3.0.txt
+[Apache Software License 2.0]: http://www.apache.org/licenses/LICENSE-2.0
+[Mozilla Public License 2.0]: https://www.mozilla.org/media/MPL/2.0/index.txt
+[cookiecutter-napari-plugin]: https://github.com/napari/cookiecutter-napari-plugin
+
+[file an issue]: https://github.com/BiAPoL/biaplotter/issues
+
+[napari]: https://github.com/napari/napari
+[tox]: https://tox.readthedocs.io/en/latest/
+[pip]: https://pypi.org/project/pip/
+[PyPI]: https://pypi.org/
```

### Comparing `biaplotter-0.0.1/src/biaplotter.egg-info/SOURCES.txt` & `biaplotter-0.0.2/src/biaplotter.egg-info/SOURCES.txt`

 * *Files identical despite different names*

