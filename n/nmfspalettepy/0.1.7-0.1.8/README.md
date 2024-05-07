# Comparing `tmp/nmfspalettepy-0.1.7.tar.gz` & `tmp/nmfspalettepy-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nmfspalettepy-0.1.7.tar", last modified: Sat May  4 00:08:33 2024, max compression
+gzip compressed data, was "nmfspalettepy-0.1.8.tar", last modified: Sat May  4 00:10:23 2024, max compression
```

## Comparing `nmfspalettepy-0.1.7.tar` & `nmfspalettepy-0.1.8.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-05-04 00:08:33.646851 nmfspalettepy-0.1.7/
--rw-rw-rw-   0        0        0      523 2023-12-06 21:45:16.000000 nmfspalettepy-0.1.7/LICENSE.md
--rw-rw-rw-   0        0        0     6423 2024-05-04 00:08:33.646851 nmfspalettepy-0.1.7/PKG-INFO
--rw-rw-rw-   0        0        0     6173 2024-05-04 00:06:31.000000 nmfspalettepy-0.1.7/README.md
-drwxrwxrwx   0        0        0        0 2024-05-04 00:08:33.631226 nmfspalettepy-0.1.7/nmfspalettepy/
--rw-rw-rw-   0        0        0      141 2024-05-01 19:42:52.000000 nmfspalettepy-0.1.7/nmfspalettepy/__init__.py
--rw-rw-rw-   0        0        0     1924 2024-05-01 19:34:30.000000 nmfspalettepy-0.1.7/nmfspalettepy/palettes.py
-drwxrwxrwx   0        0        0        0 2024-05-04 00:08:33.646851 nmfspalettepy-0.1.7/nmfspalettepy.egg-info/
--rw-rw-rw-   0        0        0     6423 2024-05-04 00:08:33.000000 nmfspalettepy-0.1.7/nmfspalettepy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      265 2024-05-04 00:08:33.000000 nmfspalettepy-0.1.7/nmfspalettepy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-04 00:08:33.000000 nmfspalettepy-0.1.7/nmfspalettepy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2024-05-04 00:08:33.000000 nmfspalettepy-0.1.7/nmfspalettepy.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-05-04 00:08:33.000000 nmfspalettepy-0.1.7/nmfspalettepy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-04 00:08:33.646851 nmfspalettepy-0.1.7/setup.cfg
--rw-rw-rw-   0        0        0      538 2024-05-04 00:06:50.000000 nmfspalettepy-0.1.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-04 00:10:23.454048 nmfspalettepy-0.1.8/
+-rw-rw-rw-   0        0        0      523 2023-12-06 21:45:16.000000 nmfspalettepy-0.1.8/LICENSE.md
+-rw-rw-rw-   0        0        0     5691 2024-05-04 00:10:23.454048 nmfspalettepy-0.1.8/PKG-INFO
+-rw-rw-rw-   0        0        0     5441 2024-05-04 00:10:16.000000 nmfspalettepy-0.1.8/README.md
+drwxrwxrwx   0        0        0        0 2024-05-04 00:10:23.438412 nmfspalettepy-0.1.8/nmfspalettepy/
+-rw-rw-rw-   0        0        0      141 2024-05-01 19:42:52.000000 nmfspalettepy-0.1.8/nmfspalettepy/__init__.py
+-rw-rw-rw-   0        0        0     1924 2024-05-01 19:34:30.000000 nmfspalettepy-0.1.8/nmfspalettepy/palettes.py
+drwxrwxrwx   0        0        0        0 2024-05-04 00:10:23.454048 nmfspalettepy-0.1.8/nmfspalettepy.egg-info/
+-rw-rw-rw-   0        0        0     5691 2024-05-04 00:10:23.000000 nmfspalettepy-0.1.8/nmfspalettepy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      265 2024-05-04 00:10:23.000000 nmfspalettepy-0.1.8/nmfspalettepy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-04 00:10:23.000000 nmfspalettepy-0.1.8/nmfspalettepy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2024-05-04 00:10:23.000000 nmfspalettepy-0.1.8/nmfspalettepy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-05-04 00:10:23.000000 nmfspalettepy-0.1.8/nmfspalettepy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-04 00:10:23.454048 nmfspalettepy-0.1.8/setup.cfg
+-rw-rw-rw-   0        0        0      538 2024-05-04 00:09:30.000000 nmfspalettepy-0.1.8/setup.py
```

### Comparing `nmfspalettepy-0.1.7/LICENSE.md` & `nmfspalettepy-0.1.8/LICENSE.md`

 * *Files identical despite different names*

### Comparing `nmfspalettepy-0.1.7/PKG-INFO` & `nmfspalettepy-0.1.8/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nmfspalettepy
-Version: 0.1.7
+Version: 0.1.8
 Summary: NMFS color palettes handling library
 Author: Michael Akridge
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 Requires-Dist: numpy
 Requires-Dist: matplotlib
 
@@ -20,43 +20,22 @@
   - https://github.com/MichaelAkridge-NOAA/NOAA-NMFS-Brand-Resources/tree/nmfspalettepy
 
 ### Features
 
 - Provides a set of predefined color palettes using the NMFS color palettes.
 - Functions to display and utilize these palettes in visualizations.
 - Easy integration with matplotlib for creating custom color maps.
-# Table of Contents
 
-- [Installation](#installation)
-  - [To Install via pip](#installation)
-  - [To Install From Source](#to-install-from-source)
-- [Usage](#usage)
-  - [Listing Available Color Palettes](#listing-available-color-palettes)
-  - [Display a Color Gradient](#display-a-color-gradient)
-  - [Creating a Custom Color Map](#creating-a-custom-color-map)
-  - [Getting Hex Codes for a Palette](#getting-hex-codes-for-a-palette)
-- [Examples](#examples)
-  - [Plot](#plot)
-  - [Boxplot](#boxplot)
-  - [LinePlot](#lineplot)
 ## Installation
 #### To Install via pip
 To install `nmfspalettepy`, you can use pip. Simply run the following command:
 
 ```
 pip install nmfspalettepy
 ```
-
-#### To Install From Source
-```
-git clone -b nmfspalettepy https://github.com/MichaelAkridge-NOAA/NOAA-NMFS-Brand-Resources.git
-cd NOAA-NMFS-Brand-Resources
-python setup.py install
-```
-
 ## Usage
 
 ## Listing Available Color Palettes
 
 To see a list of all available color palettes you can use with `nmfspalettepy`, simply call the `list_nmfs_palettes` function:
 
 ```
```

#### html2text {}

```diff
@@ -1,42 +1,33 @@
-Metadata-Version: 2.1 Name: nmfspalettepy Version: 0.1.7 Summary: NMFS color
+Metadata-Version: 2.1 Name: nmfspalettepy Version: 0.1.8 Summary: NMFS color
 palettes handling library Author: Michael Akridge Description-Content-Type:
 text/markdown License-File: LICENSE.md Requires-Dist: numpy Requires-Dist:
 matplotlib # nmfspalettepy _[_l_o_g_o_]`nmfspalettepy` is a Python library designed
 to facilitate the use of National Marine Fisheries Service (NMFS) color
 palettes for data visualization. It provides easy access to a series of NMFS
 color schemes. ## Source Code: - view on Github - https://github.com/
 MichaelAkridge-NOAA/NOAA-NMFS-Brand-Resources/tree/nmfspalettepy ### Features -
 Provides a set of predefined color palettes using the NMFS color palettes. -
 Functions to display and utilize these palettes in visualizations. - Easy
-integration with matplotlib for creating custom color maps. # Table of Contents
-- [Installation](#installation) - [To Install via pip](#installation) - [To
-Install From Source](#to-install-from-source) - [Usage](#usage) - [Listing
-Available Color Palettes](#listing-available-color-palettes) - [Display a Color
-Gradient](#display-a-color-gradient) - [Creating a Custom Color Map](#creating-
-a-custom-color-map) - [Getting Hex Codes for a Palette](#getting-hex-codes-for-
-a-palette) - [Examples](#examples) - [Plot](#plot) - [Boxplot](#boxplot) -
-[LinePlot](#lineplot) ## Installation #### To Install via pip To install
-`nmfspalettepy`, you can use pip. Simply run the following command: ``` pip
-install nmfspalettepy ``` #### To Install From Source ``` git clone -
-b nmfspalettepy https://github.com/MichaelAkridge-NOAA/NOAA-NMFS-Brand-
-Resources.git cd NOAA-NMFS-Brand-Resources python setup.py install ``` ## Usage
-## Listing Available Color Palettes To see a list of all available color
-palettes you can use with `nmfspalettepy`, simply call the `list_nmfs_palettes`
-function: ``` import nmfspalettepy print(nmfspalettepy.list_nmfs_palettes())
-``` ### output ``` ['oceans', 'waves', 'seagrass', 'urchin', 'crustacean',
-'coral'] ``` ### Display a Color Gradient To display a color gradient using one
-of the available NMFS color palettes, you can use the `display_color_gradient`
-function. Here's an example using the "oceans" palette: ``` from nmfspalettepy
-import display_color_gradient, get_palette_colors # Display the 'oceans'
-palette gradient display_color_gradient(get_palette_colors("oceans")) ``` ![]
-(https://github.com/MichaelAkridge-NOAA/NOAA-NMFS-Brand-Resources/raw/
-nmfspalettepy/docs/waves_palette.png) ### Creating a Custom Color Map ```
-import matplotlib.pyplot as plt from nmfspalettepy import create_nmfs_colormap
-# Create a custom colormap cmap = create_nmfs_colormap("coral") # Use the
+integration with matplotlib for creating custom color maps. ## Installation
+#### To Install via pip To install `nmfspalettepy`, you can use pip. Simply run
+the following command: ``` pip install nmfspalettepy ``` ## Usage ## Listing
+Available Color Palettes To see a list of all available color palettes you can
+use with `nmfspalettepy`, simply call the `list_nmfs_palettes` function: ```
+import nmfspalettepy print(nmfspalettepy.list_nmfs_palettes()) ``` ### output
+``` ['oceans', 'waves', 'seagrass', 'urchin', 'crustacean', 'coral'] ``` ###
+Display a Color Gradient To display a color gradient using one of the available
+NMFS color palettes, you can use the `display_color_gradient` function. Here's
+an example using the "oceans" palette: ``` from nmfspalettepy import
+display_color_gradient, get_palette_colors # Display the 'oceans' palette
+gradient display_color_gradient(get_palette_colors("oceans")) ``` ![](https://
+github.com/MichaelAkridge-NOAA/NOAA-NMFS-Brand-Resources/raw/nmfspalettepy/
+docs/waves_palette.png) ### Creating a Custom Color Map ``` import
+matplotlib.pyplot as plt from nmfspalettepy import create_nmfs_colormap #
+Create a custom colormap cmap = create_nmfs_colormap("coral") # Use the
 colormap in a plot plt.imshow([[1,2],[2,3]], cmap=cmap) plt.colorbar() plt.show
 () ``` ![](https://github.com/MichaelAkridge-NOAA/NOAA-NMFS-Brand-Resources/
 raw/nmfspalettepy/docs/waves_plot_square.png) ### Getting Hex Codes for a
 Palette ``` from nmfspalettepy import get_palette_colors # Get hex codes for
 the 'waves' palette colors_hex = get_palette_colors("waves") print("Hex codes
 for 'waves':", colors_hex) ``` ### output ``` Hex codes for 'waves':
 ['#005E5E', '#00797F', '#1EBEC7', '#90DFE3'] ``` ## Examples ### Plot ![]
```

### Comparing `nmfspalettepy-0.1.7/README.md` & `nmfspalettepy-0.1.8/nmfspalettepy.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,17 @@
+Metadata-Version: 2.1
+Name: nmfspalettepy
+Version: 0.1.8
+Summary: NMFS color palettes handling library
+Author: Michael Akridge
+Description-Content-Type: text/markdown
+License-File: LICENSE.md
+Requires-Dist: numpy
+Requires-Dist: matplotlib
+
 # nmfspalettepy
 <a href="https://github.com/MichaelAkridge-NOAA/NOAA-NMFS-Brand-Resources/tree/nmfspalettepy">
     <img src="https://github.com/MichaelAkridge-NOAA/NOAA-NMFS-Brand-Resources/raw/main/logos/nmfspalettepy_250.png" align="right" alt="logo"/>
 </a>
 
 `nmfspalettepy` is a Python library designed to facilitate the use of National Marine Fisheries Service (NMFS) color palettes for data visualization. It provides easy access to a series of NMFS color schemes.
 
@@ -10,43 +20,22 @@
   - https://github.com/MichaelAkridge-NOAA/NOAA-NMFS-Brand-Resources/tree/nmfspalettepy
 
 ### Features
 
 - Provides a set of predefined color palettes using the NMFS color palettes.
 - Functions to display and utilize these palettes in visualizations.
 - Easy integration with matplotlib for creating custom color maps.
-# Table of Contents
 
-- [Installation](#installation)
-  - [To Install via pip](#installation)
-  - [To Install From Source](#to-install-from-source)
-- [Usage](#usage)
-  - [Listing Available Color Palettes](#listing-available-color-palettes)
-  - [Display a Color Gradient](#display-a-color-gradient)
-  - [Creating a Custom Color Map](#creating-a-custom-color-map)
-  - [Getting Hex Codes for a Palette](#getting-hex-codes-for-a-palette)
-- [Examples](#examples)
-  - [Plot](#plot)
-  - [Boxplot](#boxplot)
-  - [LinePlot](#lineplot)
 ## Installation
 #### To Install via pip
 To install `nmfspalettepy`, you can use pip. Simply run the following command:
 
 ```
 pip install nmfspalettepy
 ```
-
-#### To Install From Source
-```
-git clone -b nmfspalettepy https://github.com/MichaelAkridge-NOAA/NOAA-NMFS-Brand-Resources.git
-cd NOAA-NMFS-Brand-Resources
-python setup.py install
-```
-
 ## Usage
 
 ## Listing Available Color Palettes
 
 To see a list of all available color palettes you can use with `nmfspalettepy`, simply call the `list_nmfs_palettes` function:
 
 ```
```

#### html2text {}

```diff
@@ -1,39 +1,33 @@
-# nmfspalettepy _[_l_o_g_o_]`nmfspalettepy` is a Python library designed to
-facilitate the use of National Marine Fisheries Service (NMFS) color palettes
-for data visualization. It provides easy access to a series of NMFS color
-schemes. ## Source Code: - view on Github - https://github.com/MichaelAkridge-
-NOAA/NOAA-NMFS-Brand-Resources/tree/nmfspalettepy ### Features - Provides a set
-of predefined color palettes using the NMFS color palettes. - Functions to
-display and utilize these palettes in visualizations. - Easy integration with
-matplotlib for creating custom color maps. # Table of Contents - [Installation]
-(#installation) - [To Install via pip](#installation) - [To Install From
-Source](#to-install-from-source) - [Usage](#usage) - [Listing Available Color
-Palettes](#listing-available-color-palettes) - [Display a Color Gradient]
-(#display-a-color-gradient) - [Creating a Custom Color Map](#creating-a-custom-
-color-map) - [Getting Hex Codes for a Palette](#getting-hex-codes-for-a-
-palette) - [Examples](#examples) - [Plot](#plot) - [Boxplot](#boxplot) -
-[LinePlot](#lineplot) ## Installation #### To Install via pip To install
-`nmfspalettepy`, you can use pip. Simply run the following command: ``` pip
-install nmfspalettepy ``` #### To Install From Source ``` git clone -
-b nmfspalettepy https://github.com/MichaelAkridge-NOAA/NOAA-NMFS-Brand-
-Resources.git cd NOAA-NMFS-Brand-Resources python setup.py install ``` ## Usage
-## Listing Available Color Palettes To see a list of all available color
-palettes you can use with `nmfspalettepy`, simply call the `list_nmfs_palettes`
-function: ``` import nmfspalettepy print(nmfspalettepy.list_nmfs_palettes())
-``` ### output ``` ['oceans', 'waves', 'seagrass', 'urchin', 'crustacean',
-'coral'] ``` ### Display a Color Gradient To display a color gradient using one
-of the available NMFS color palettes, you can use the `display_color_gradient`
-function. Here's an example using the "oceans" palette: ``` from nmfspalettepy
-import display_color_gradient, get_palette_colors # Display the 'oceans'
-palette gradient display_color_gradient(get_palette_colors("oceans")) ``` ![]
-(https://github.com/MichaelAkridge-NOAA/NOAA-NMFS-Brand-Resources/raw/
-nmfspalettepy/docs/waves_palette.png) ### Creating a Custom Color Map ```
-import matplotlib.pyplot as plt from nmfspalettepy import create_nmfs_colormap
-# Create a custom colormap cmap = create_nmfs_colormap("coral") # Use the
+Metadata-Version: 2.1 Name: nmfspalettepy Version: 0.1.8 Summary: NMFS color
+palettes handling library Author: Michael Akridge Description-Content-Type:
+text/markdown License-File: LICENSE.md Requires-Dist: numpy Requires-Dist:
+matplotlib # nmfspalettepy _[_l_o_g_o_]`nmfspalettepy` is a Python library designed
+to facilitate the use of National Marine Fisheries Service (NMFS) color
+palettes for data visualization. It provides easy access to a series of NMFS
+color schemes. ## Source Code: - view on Github - https://github.com/
+MichaelAkridge-NOAA/NOAA-NMFS-Brand-Resources/tree/nmfspalettepy ### Features -
+Provides a set of predefined color palettes using the NMFS color palettes. -
+Functions to display and utilize these palettes in visualizations. - Easy
+integration with matplotlib for creating custom color maps. ## Installation
+#### To Install via pip To install `nmfspalettepy`, you can use pip. Simply run
+the following command: ``` pip install nmfspalettepy ``` ## Usage ## Listing
+Available Color Palettes To see a list of all available color palettes you can
+use with `nmfspalettepy`, simply call the `list_nmfs_palettes` function: ```
+import nmfspalettepy print(nmfspalettepy.list_nmfs_palettes()) ``` ### output
+``` ['oceans', 'waves', 'seagrass', 'urchin', 'crustacean', 'coral'] ``` ###
+Display a Color Gradient To display a color gradient using one of the available
+NMFS color palettes, you can use the `display_color_gradient` function. Here's
+an example using the "oceans" palette: ``` from nmfspalettepy import
+display_color_gradient, get_palette_colors # Display the 'oceans' palette
+gradient display_color_gradient(get_palette_colors("oceans")) ``` ![](https://
+github.com/MichaelAkridge-NOAA/NOAA-NMFS-Brand-Resources/raw/nmfspalettepy/
+docs/waves_palette.png) ### Creating a Custom Color Map ``` import
+matplotlib.pyplot as plt from nmfspalettepy import create_nmfs_colormap #
+Create a custom colormap cmap = create_nmfs_colormap("coral") # Use the
 colormap in a plot plt.imshow([[1,2],[2,3]], cmap=cmap) plt.colorbar() plt.show
 () ``` ![](https://github.com/MichaelAkridge-NOAA/NOAA-NMFS-Brand-Resources/
 raw/nmfspalettepy/docs/waves_plot_square.png) ### Getting Hex Codes for a
 Palette ``` from nmfspalettepy import get_palette_colors # Get hex codes for
 the 'waves' palette colors_hex = get_palette_colors("waves") print("Hex codes
 for 'waves':", colors_hex) ``` ### output ``` Hex codes for 'waves':
 ['#005E5E', '#00797F', '#1EBEC7', '#90DFE3'] ``` ## Examples ### Plot ![]
```

### Comparing `nmfspalettepy-0.1.7/nmfspalettepy/palettes.py` & `nmfspalettepy-0.1.8/nmfspalettepy/palettes.py`

 * *Files identical despite different names*

### Comparing `nmfspalettepy-0.1.7/nmfspalettepy.egg-info/PKG-INFO` & `nmfspalettepy-0.1.8/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,17 +1,7 @@
-Metadata-Version: 2.1
-Name: nmfspalettepy
-Version: 0.1.7
-Summary: NMFS color palettes handling library
-Author: Michael Akridge
-Description-Content-Type: text/markdown
-License-File: LICENSE.md
-Requires-Dist: numpy
-Requires-Dist: matplotlib
-
 # nmfspalettepy
 <a href="https://github.com/MichaelAkridge-NOAA/NOAA-NMFS-Brand-Resources/tree/nmfspalettepy">
     <img src="https://github.com/MichaelAkridge-NOAA/NOAA-NMFS-Brand-Resources/raw/main/logos/nmfspalettepy_250.png" align="right" alt="logo"/>
 </a>
 
 `nmfspalettepy` is a Python library designed to facilitate the use of National Marine Fisheries Service (NMFS) color palettes for data visualization. It provides easy access to a series of NMFS color schemes.
 
@@ -20,43 +10,22 @@
   - https://github.com/MichaelAkridge-NOAA/NOAA-NMFS-Brand-Resources/tree/nmfspalettepy
 
 ### Features
 
 - Provides a set of predefined color palettes using the NMFS color palettes.
 - Functions to display and utilize these palettes in visualizations.
 - Easy integration with matplotlib for creating custom color maps.
-# Table of Contents
 
-- [Installation](#installation)
-  - [To Install via pip](#installation)
-  - [To Install From Source](#to-install-from-source)
-- [Usage](#usage)
-  - [Listing Available Color Palettes](#listing-available-color-palettes)
-  - [Display a Color Gradient](#display-a-color-gradient)
-  - [Creating a Custom Color Map](#creating-a-custom-color-map)
-  - [Getting Hex Codes for a Palette](#getting-hex-codes-for-a-palette)
-- [Examples](#examples)
-  - [Plot](#plot)
-  - [Boxplot](#boxplot)
-  - [LinePlot](#lineplot)
 ## Installation
 #### To Install via pip
 To install `nmfspalettepy`, you can use pip. Simply run the following command:
 
 ```
 pip install nmfspalettepy
 ```
-
-#### To Install From Source
-```
-git clone -b nmfspalettepy https://github.com/MichaelAkridge-NOAA/NOAA-NMFS-Brand-Resources.git
-cd NOAA-NMFS-Brand-Resources
-python setup.py install
-```
-
 ## Usage
 
 ## Listing Available Color Palettes
 
 To see a list of all available color palettes you can use with `nmfspalettepy`, simply call the `list_nmfs_palettes` function:
 
 ```
```

#### html2text {}

```diff
@@ -1,42 +1,30 @@
-Metadata-Version: 2.1 Name: nmfspalettepy Version: 0.1.7 Summary: NMFS color
-palettes handling library Author: Michael Akridge Description-Content-Type:
-text/markdown License-File: LICENSE.md Requires-Dist: numpy Requires-Dist:
-matplotlib # nmfspalettepy _[_l_o_g_o_]`nmfspalettepy` is a Python library designed
-to facilitate the use of National Marine Fisheries Service (NMFS) color
-palettes for data visualization. It provides easy access to a series of NMFS
-color schemes. ## Source Code: - view on Github - https://github.com/
-MichaelAkridge-NOAA/NOAA-NMFS-Brand-Resources/tree/nmfspalettepy ### Features -
-Provides a set of predefined color palettes using the NMFS color palettes. -
-Functions to display and utilize these palettes in visualizations. - Easy
-integration with matplotlib for creating custom color maps. # Table of Contents
-- [Installation](#installation) - [To Install via pip](#installation) - [To
-Install From Source](#to-install-from-source) - [Usage](#usage) - [Listing
-Available Color Palettes](#listing-available-color-palettes) - [Display a Color
-Gradient](#display-a-color-gradient) - [Creating a Custom Color Map](#creating-
-a-custom-color-map) - [Getting Hex Codes for a Palette](#getting-hex-codes-for-
-a-palette) - [Examples](#examples) - [Plot](#plot) - [Boxplot](#boxplot) -
-[LinePlot](#lineplot) ## Installation #### To Install via pip To install
-`nmfspalettepy`, you can use pip. Simply run the following command: ``` pip
-install nmfspalettepy ``` #### To Install From Source ``` git clone -
-b nmfspalettepy https://github.com/MichaelAkridge-NOAA/NOAA-NMFS-Brand-
-Resources.git cd NOAA-NMFS-Brand-Resources python setup.py install ``` ## Usage
-## Listing Available Color Palettes To see a list of all available color
-palettes you can use with `nmfspalettepy`, simply call the `list_nmfs_palettes`
-function: ``` import nmfspalettepy print(nmfspalettepy.list_nmfs_palettes())
-``` ### output ``` ['oceans', 'waves', 'seagrass', 'urchin', 'crustacean',
-'coral'] ``` ### Display a Color Gradient To display a color gradient using one
-of the available NMFS color palettes, you can use the `display_color_gradient`
-function. Here's an example using the "oceans" palette: ``` from nmfspalettepy
-import display_color_gradient, get_palette_colors # Display the 'oceans'
-palette gradient display_color_gradient(get_palette_colors("oceans")) ``` ![]
-(https://github.com/MichaelAkridge-NOAA/NOAA-NMFS-Brand-Resources/raw/
-nmfspalettepy/docs/waves_palette.png) ### Creating a Custom Color Map ```
-import matplotlib.pyplot as plt from nmfspalettepy import create_nmfs_colormap
-# Create a custom colormap cmap = create_nmfs_colormap("coral") # Use the
+# nmfspalettepy _[_l_o_g_o_]`nmfspalettepy` is a Python library designed to
+facilitate the use of National Marine Fisheries Service (NMFS) color palettes
+for data visualization. It provides easy access to a series of NMFS color
+schemes. ## Source Code: - view on Github - https://github.com/MichaelAkridge-
+NOAA/NOAA-NMFS-Brand-Resources/tree/nmfspalettepy ### Features - Provides a set
+of predefined color palettes using the NMFS color palettes. - Functions to
+display and utilize these palettes in visualizations. - Easy integration with
+matplotlib for creating custom color maps. ## Installation #### To Install via
+pip To install `nmfspalettepy`, you can use pip. Simply run the following
+command: ``` pip install nmfspalettepy ``` ## Usage ## Listing Available Color
+Palettes To see a list of all available color palettes you can use with
+`nmfspalettepy`, simply call the `list_nmfs_palettes` function: ``` import
+nmfspalettepy print(nmfspalettepy.list_nmfs_palettes()) ``` ### output ```
+['oceans', 'waves', 'seagrass', 'urchin', 'crustacean', 'coral'] ``` ###
+Display a Color Gradient To display a color gradient using one of the available
+NMFS color palettes, you can use the `display_color_gradient` function. Here's
+an example using the "oceans" palette: ``` from nmfspalettepy import
+display_color_gradient, get_palette_colors # Display the 'oceans' palette
+gradient display_color_gradient(get_palette_colors("oceans")) ``` ![](https://
+github.com/MichaelAkridge-NOAA/NOAA-NMFS-Brand-Resources/raw/nmfspalettepy/
+docs/waves_palette.png) ### Creating a Custom Color Map ``` import
+matplotlib.pyplot as plt from nmfspalettepy import create_nmfs_colormap #
+Create a custom colormap cmap = create_nmfs_colormap("coral") # Use the
 colormap in a plot plt.imshow([[1,2],[2,3]], cmap=cmap) plt.colorbar() plt.show
 () ``` ![](https://github.com/MichaelAkridge-NOAA/NOAA-NMFS-Brand-Resources/
 raw/nmfspalettepy/docs/waves_plot_square.png) ### Getting Hex Codes for a
 Palette ``` from nmfspalettepy import get_palette_colors # Get hex codes for
 the 'waves' palette colors_hex = get_palette_colors("waves") print("Hex codes
 for 'waves':", colors_hex) ``` ### output ``` Hex codes for 'waves':
 ['#005E5E', '#00797F', '#1EBEC7', '#90DFE3'] ``` ## Examples ### Plot ![]
```

