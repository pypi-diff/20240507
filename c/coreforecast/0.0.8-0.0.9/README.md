# Comparing `tmp/coreforecast-0.0.8.tar.gz` & `tmp/coreforecast-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "coreforecast-0.0.8.tar", last modified: Wed Nov  9 12:37:21 2022, max compression
+gzip compressed data, was "coreforecast-0.0.9.tar", last modified: Wed Nov  9 12:37:21 2022, max compression
```

## Comparing `coreforecast-0.0.8.tar` & `coreforecast-0.0.9.tar`

### file list

```diff
@@ -1,46 +1,45 @@
--rw-r--r--   0        0        0     1189 2022-11-09 12:37:21.000000 coreforecast-0.0.8/.github/workflows/build-docs.yaml
--rw-r--r--   0        0        0     2624 2022-11-09 12:37:21.000000 coreforecast-0.0.8/.github/workflows/ci.yaml
--rw-r--r--   0        0        0     1641 2022-11-09 12:37:21.000000 coreforecast-0.0.8/.github/workflows/release.yaml
--rw-r--r--   0        0        0      313 2022-11-09 12:37:21.000000 coreforecast-0.0.8/.gitignore
--rw-r--r--   0        0        0      255 2022-11-09 12:37:21.000000 coreforecast-0.0.8/.vscode/c_cpp_properties.json
--rw-r--r--   0        0        0      208 2022-11-09 12:37:21.000000 coreforecast-0.0.8/.vscode/settings.json
--rw-r--r--   0        0        0     2265 2022-11-09 12:37:21.000000 coreforecast-0.0.8/CMakeLists.txt
--rw-r--r--   0        0        0    11357 2022-11-09 12:37:21.000000 coreforecast-0.0.8/LICENSE
--rw-r--r--   0        0        0     2390 2022-11-09 12:37:21.000000 coreforecast-0.0.8/README.md
--rw-r--r--   0        0        0       22 2022-11-09 12:37:21.000000 coreforecast-0.0.8/coreforecast/__init__.py
--rw-r--r--   0        0        0      486 2022-11-09 12:37:21.000000 coreforecast-0.0.8/coreforecast/_lib.py
--rw-r--r--   0        0        0     2029 2022-11-09 12:37:21.000000 coreforecast-0.0.8/coreforecast/differences.py
--rw-r--r--   0        0        0    15261 2022-11-09 12:37:21.000000 coreforecast-0.0.8/coreforecast/grouped_array.py
--rw-r--r--   0        0        0    12313 2022-11-09 12:37:21.000000 coreforecast-0.0.8/coreforecast/lag_transforms.py
--rw-r--r--   0        0        0    23057 2022-11-09 12:37:21.000000 coreforecast-0.0.8/coreforecast/scalers.py
--rw-r--r--   0        0        0      800 2022-11-09 12:37:21.000000 coreforecast-0.0.8/coreforecast/seasonal.py
--rw-r--r--   0        0        0      885 2022-11-09 12:37:21.000000 coreforecast-0.0.8/coreforecast/utils.py
--rw-r--r--   0        0        0     2883 2022-11-09 12:37:21.000000 coreforecast-0.0.8/docs/mintlify/dark.png
--rw-r--r--   0        0        0     1633 2022-11-09 12:37:21.000000 coreforecast-0.0.8/docs/mintlify/favicon.svg
--rw-r--r--   0        0        0     2851 2022-11-09 12:37:21.000000 coreforecast-0.0.8/docs/mintlify/light.png
--rw-r--r--   0        0        0      694 2022-11-09 12:37:21.000000 coreforecast-0.0.8/docs/mintlify/mint.json
--rw-r--r--   0        0        0      711 2022-11-09 12:37:21.000000 coreforecast-0.0.8/docs/to_mdx.py
--rw-r--r--   0        0        0     2033 2022-11-09 12:37:21.000000 coreforecast-0.0.8/include/brent.h
--rw-r--r--   0        0        0     3545 2022-11-09 12:37:21.000000 coreforecast-0.0.8/include/diff.h
--rw-r--r--   0        0        0     1984 2022-11-09 12:37:21.000000 coreforecast-0.0.8/include/expanding.h
--rw-r--r--   0        0        0      353 2022-11-09 12:37:21.000000 coreforecast-0.0.8/include/exponentially_weighted.h
--rw-r--r--   0        0        0      103 2022-11-09 12:37:21.000000 coreforecast-0.0.8/include/export.h
--rw-r--r--   0        0        0     5456 2022-11-09 12:37:21.000000 coreforecast-0.0.8/include/grouped_array.h
--rw-r--r--   0        0        0     2529 2022-11-09 12:37:21.000000 coreforecast-0.0.8/include/grouped_array_functions.h
--rw-r--r--   0        0        0      794 2022-11-09 12:37:21.000000 coreforecast-0.0.8/include/kpss.h
--rw-r--r--   0        0        0      368 2022-11-09 12:37:21.000000 coreforecast-0.0.8/include/lag.h
--rw-r--r--   0        0        0    12968 2022-11-09 12:37:21.000000 coreforecast-0.0.8/include/rolling.h
--rw-r--r--   0        0        0     4467 2022-11-09 12:37:21.000000 coreforecast-0.0.8/include/scalers.h
--rw-r--r--   0        0        0     1701 2022-11-09 12:37:21.000000 coreforecast-0.0.8/include/seasonal.h
--rw-r--r--   0        0        0     1416 2022-11-09 12:37:21.000000 coreforecast-0.0.8/include/stats.h
--rw-r--r--   0        0        0     1501 2022-11-09 12:37:21.000000 coreforecast-0.0.8/pyproject.toml
--rw-r--r--   0        0        0      121 2022-11-09 12:37:21.000000 coreforecast-0.0.8/requirements-test.txt
--rwxr-xr-x   0        0        0      199 2022-11-09 12:37:21.000000 coreforecast-0.0.8/scripts/switch_xcode
--rw-r--r--   0        0        0     8132 2022-11-09 12:37:21.000000 coreforecast-0.0.8/src/diff.cpp
--rw-r--r--   0        0        0     5055 2022-11-09 12:37:21.000000 coreforecast-0.0.8/src/expanding.cpp
--rw-r--r--   0        0        0      872 2022-11-09 12:37:21.000000 coreforecast-0.0.8/src/exponentially_weighted.cpp
--rw-r--r--   0        0        0     4287 2022-11-09 12:37:21.000000 coreforecast-0.0.8/src/grouped_array_functions.cpp
--rw-r--r--   0        0        0      631 2022-11-09 12:37:21.000000 coreforecast-0.0.8/src/lag.cpp
--rw-r--r--   0        0        0    26212 2022-11-09 12:37:21.000000 coreforecast-0.0.8/src/rolling.cpp
--rw-r--r--   0        0        0    13389 2022-11-09 12:37:21.000000 coreforecast-0.0.8/src/scalers.cpp
--rw-r--r--   0        0        0     3403 2022-11-09 12:37:21.000000 coreforecast-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0     1189 2022-11-09 12:37:21.000000 coreforecast-0.0.9/.github/workflows/build-docs.yaml
+-rw-r--r--   0        0        0     2856 2022-11-09 12:37:21.000000 coreforecast-0.0.9/.github/workflows/ci.yaml
+-rw-r--r--   0        0        0     1641 2022-11-09 12:37:21.000000 coreforecast-0.0.9/.github/workflows/release.yaml
+-rw-r--r--   0        0        0      313 2022-11-09 12:37:21.000000 coreforecast-0.0.9/.gitignore
+-rw-r--r--   0        0        0      313 2022-11-09 12:37:21.000000 coreforecast-0.0.9/.vscode/c_cpp_properties.json
+-rw-r--r--   0        0        0      208 2022-11-09 12:37:21.000000 coreforecast-0.0.9/.vscode/settings.json
+-rw-r--r--   0        0        0     2808 2022-11-09 12:37:21.000000 coreforecast-0.0.9/CMakeLists.txt
+-rw-r--r--   0        0        0     5215 2022-11-09 12:37:21.000000 coreforecast-0.0.9/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0    11357 2022-11-09 12:37:21.000000 coreforecast-0.0.9/LICENSE
+-rw-r--r--   0        0        0     2390 2022-11-09 12:37:21.000000 coreforecast-0.0.9/README.md
+-rw-r--r--   0        0        0     2883 2022-11-09 12:37:21.000000 coreforecast-0.0.9/docs/mintlify/dark.png
+-rw-r--r--   0        0        0     1633 2022-11-09 12:37:21.000000 coreforecast-0.0.9/docs/mintlify/favicon.svg
+-rw-r--r--   0        0        0     2851 2022-11-09 12:37:21.000000 coreforecast-0.0.9/docs/mintlify/light.png
+-rw-r--r--   0        0        0      694 2022-11-09 12:37:21.000000 coreforecast-0.0.9/docs/mintlify/mint.json
+-rw-r--r--   0        0        0      711 2022-11-09 12:37:21.000000 coreforecast-0.0.9/docs/to_mdx.py
+-rw-r--r--   0        0        0     2033 2022-11-09 12:37:21.000000 coreforecast-0.0.9/include/brent.h
+-rw-r--r--   0        0        0    29219 2022-11-09 12:37:21.000000 coreforecast-0.0.9/include/c_api.h
+-rw-r--r--   0        0        0     2981 2022-11-09 12:37:21.000000 coreforecast-0.0.9/include/diff.h
+-rw-r--r--   0        0        0     1173 2022-11-09 12:37:21.000000 coreforecast-0.0.9/include/expanding.h
+-rw-r--r--   0        0        0      286 2022-11-09 12:37:21.000000 coreforecast-0.0.9/include/exponentially_weighted.h
+-rw-r--r--   0        0        0     5435 2022-11-09 12:37:21.000000 coreforecast-0.0.9/include/grouped_array.h
+-rw-r--r--   0        0        0      875 2022-11-09 12:37:21.000000 coreforecast-0.0.9/include/grouped_array_functions.h
+-rw-r--r--   0        0        0      774 2022-11-09 12:37:21.000000 coreforecast-0.0.9/include/kpss.h
+-rw-r--r--   0        0        0      129 2022-11-09 12:37:21.000000 coreforecast-0.0.9/include/lag.h
+-rw-r--r--   0        0        0    12213 2022-11-09 12:37:21.000000 coreforecast-0.0.9/include/rolling.h
+-rw-r--r--   0        0        0     5690 2022-11-09 12:37:21.000000 coreforecast-0.0.9/include/scalers.h
+-rw-r--r--   0        0        0     1947 2022-11-09 12:37:21.000000 coreforecast-0.0.9/include/seasonal.h
+-rw-r--r--   0        0        0     1501 2022-11-09 12:37:21.000000 coreforecast-0.0.9/include/stats.h
+-rw-r--r--   0        0        0     1452 2022-11-09 12:37:21.000000 coreforecast-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0       22 2022-11-09 12:37:21.000000 coreforecast-0.0.9/python/coreforecast/__init__.py
+-rw-r--r--   0        0        0      486 2022-11-09 12:37:21.000000 coreforecast-0.0.9/python/coreforecast/_lib.py
+-rw-r--r--   0        0        0     2029 2022-11-09 12:37:21.000000 coreforecast-0.0.9/python/coreforecast/differences.py
+-rw-r--r--   0        0        0     2086 2022-11-09 12:37:21.000000 coreforecast-0.0.9/python/coreforecast/expanding.py
+-rw-r--r--   0        0        0      836 2022-11-09 12:37:21.000000 coreforecast-0.0.9/python/coreforecast/exponentially_weighted.py
+-rw-r--r--   0        0        0    15261 2022-11-09 12:37:21.000000 coreforecast-0.0.9/python/coreforecast/grouped_array.py
+-rw-r--r--   0        0        0    12313 2022-11-09 12:37:21.000000 coreforecast-0.0.9/python/coreforecast/lag_transforms.py
+-rw-r--r--   0        0        0     6838 2022-11-09 12:37:21.000000 coreforecast-0.0.9/python/coreforecast/rolling.py
+-rw-r--r--   0        0        0    23057 2022-11-09 12:37:21.000000 coreforecast-0.0.9/python/coreforecast/scalers.py
+-rw-r--r--   0        0        0      800 2022-11-09 12:37:21.000000 coreforecast-0.0.9/python/coreforecast/seasonal.py
+-rw-r--r--   0        0        0      885 2022-11-09 12:37:21.000000 coreforecast-0.0.9/python/coreforecast/utils.py
+-rw-r--r--   0        0        0      121 2022-11-09 12:37:21.000000 coreforecast-0.0.9/requirements-test.txt
+-rw-r--r--   0        0        0      808 2022-11-09 12:37:21.000000 coreforecast-0.0.9/scripts/float64_methods.py
+-rwxr-xr-x   0        0        0      199 2022-11-09 12:37:21.000000 coreforecast-0.0.9/scripts/switch_xcode
+-rw-r--r--   0        0        0    48128 2022-11-09 12:37:21.000000 coreforecast-0.0.9/src/c_api.cpp
+-rw-r--r--   0        0        0     3419 2022-11-09 12:37:21.000000 coreforecast-0.0.9/PKG-INFO
```

### Comparing `coreforecast-0.0.8/.github/workflows/build-docs.yaml` & `coreforecast-0.0.9/.github/workflows/build-docs.yaml`

 * *Files identical despite different names*

### Comparing `coreforecast-0.0.8/.github/workflows/ci.yaml` & `coreforecast-0.0.9/.github/workflows/ci.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -21,24 +21,32 @@
     runs-on: ${{ matrix.os }}
     strategy:
       fail-fast: false
       matrix:
         include:
           - os: ubuntu-20.04
             platform-id: manylinux_x86_64
+          - os: ubuntu-20.04
+            platform-id: manylinux_aarch64
           - os: windows-2019
             platform-id: win_amd64
           - os: macos-11
             platform-id: macosx_x86_64
           - os: macos-14
             platform-id: macosx_arm64
 
     steps:
       - uses: actions/checkout@v4
 
+      - name: Set up QEMU
+        if: matrix.platform-id == 'manylinux_aarch64'
+        uses: docker/setup-qemu-action@v3
+        with:
+          platforms: arm64
+
       - name: Build wheels
         uses: pypa/cibuildwheel@v2.16.5
         env:
           CIBW_BUILD: cp310-${{ matrix.platform-id }}
 
       - uses: actions/upload-artifact@v3
         with:
@@ -47,15 +55,15 @@
 
   run_tests:
     needs: [build_wheels]
     runs-on: ${{ matrix.os }}
     strategy:
       fail-fast: false
       matrix:
-        os: [macos-latest, ubuntu-latest, windows-latest]
+        os: [macos-13, ubuntu-latest, windows-latest]
         python-version: ['3.8', '3.9', '3.10', '3.11']
     steps:
       - name: Clone repo
         uses: actions/checkout@v3
 
       - uses: actions/setup-python@v4
         with:
```

### Comparing `coreforecast-0.0.8/.github/workflows/release.yaml` & `coreforecast-0.0.9/.github/workflows/release.yaml`

 * *Files identical despite different names*

### Comparing `coreforecast-0.0.8/CMakeLists.txt` & `coreforecast-0.0.9/CMakeLists.txt`

 * *Files 10% similar despite different names*

```diff
@@ -5,61 +5,84 @@
 option(USE_OPENMP "Enable OpenMP" ON)
 
 if(NOT CMAKE_BUILD_TYPE)
     set(CMAKE_BUILD_TYPE Release)
 endif()
 
 set(CMAKE_CXX_STANDARD 17)
+
 if(USE_OPENMP)
     if(APPLE)
         find_package(OpenMP)
+
         if(NOT OpenMP_FOUND)
             # libomp 15.0+ from brew is keg-only, so have to search in other locations.
             # See https://github.com/Homebrew/homebrew-core/issues/112107#issuecomment-1278042927.
             execute_process(COMMAND brew --prefix libomp
-                            OUTPUT_VARIABLE HOMEBREW_LIBOMP_PREFIX
-                            OUTPUT_STRIP_TRAILING_WHITESPACE)
+                OUTPUT_VARIABLE HOMEBREW_LIBOMP_PREFIX
+                OUTPUT_STRIP_TRAILING_WHITESPACE)
             set(OpenMP_C_FLAGS "-Xpreprocessor -fopenmp -I${HOMEBREW_LIBOMP_PREFIX}/include")
             set(OpenMP_CXX_FLAGS "-Xpreprocessor -fopenmp -I${HOMEBREW_LIBOMP_PREFIX}/include")
             set(OpenMP_C_LIB_NAMES omp)
             set(OpenMP_CXX_LIB_NAMES omp)
             set(OpenMP_omp_LIBRARY ${HOMEBREW_LIBOMP_PREFIX}/lib/libomp.dylib)
         endif()
     endif()
+
     find_package(OpenMP REQUIRED)
     set(CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS} ${OpenMP_CXX_FLAGS}")
 endif()
 
 if(APPLE)
     set(CMAKE_SHARED_LIBRARY_SUFFIX ".so")
 endif()
 
 if(UNIX)
     set(CMAKE_CXX_FLAGS_DEBUG "${CMAKE_CXX_FLAGS_DEBUG} -fPIC -O0 -g -Wall -Wextra -Wpedantic")
     set(CMAKE_CXX_FLAGS_RELEASE "${CMAKE_CXX_FLAGS_RELEASE} -fPIC -O3 -Wall -Wextra -Wpedantic")
+    set(CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS} -Wno-unknown-pragmas")
 else()
     set(CMAKE_CXX_FLAGS_RELEASE "${CMAKE_CXX_FLAGS_RELEASE} /O2 /Ob2 /Ot /Oy /W4")
+    set(CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS} /wd4068")
 endif()
 
 if(SKBUILD)
     set(LIBRARY_OUTPUT_PATH ${SKBUILD_PLATLIB_DIR}/coreforecast/lib)
 else()
-    set(LIBRARY_OUTPUT_PATH ${PROJECT_SOURCE_DIR}/coreforecast/lib)
+    set(LIBRARY_OUTPUT_PATH ${PROJECT_SOURCE_DIR}/python/coreforecast/lib)
 endif()
 
 include_directories(include)
 FetchContent_Declare(
     stl-cpp
     GIT_REPOSITORY https://github.com/jmoralez/stl-cpp.git
     GIT_TAG 13d26c0d0653ddcdbf853de3f92f56faa831a330
 )
-FetchContent_MakeAvailable(stl-cpp)
-include_directories(${stl-cpp_SOURCE_DIR}/include)
-file(GLOB SOURCES src/*.cpp)
+FetchContent_GetProperties(stl-cpp)
+
+if(NOT stl-cpp_POPULATED)
+    FetchContent_Populate(stl-cpp)
+    include_directories(${stl-cpp_SOURCE_DIR}/include)
+endif()
+
+FetchContent_Declare(
+    skiplist
+    GIT_REPOSITORY https://github.com/paulross/skiplist.git
+    GIT_TAG aace571a8564067820ff7a5e34ba68d0a9782153
+)
+FetchContent_GetProperties(skiplist)
+
+if(NOT skiplist_POPULATED)
+    FetchContent_Populate(skiplist)
+    include_directories(${skiplist_SOURCE_DIR}/src/cpp)
+endif()
+
+file(GLOB SOURCES src/*.cpp ${skiplist_SOURCE_DIR}/src/cpp/SkipList.cpp)
 add_library(coreforecast SHARED ${SOURCES})
+
 if(MSVC)
     set_target_properties(coreforecast PROPERTIES OUTPUT_NAME "libcoreforecast")
 endif()
 
 if(USE_OPENMP AND CMAKE_CXX_COMPILER_ID STREQUAL "AppleClang")
     target_link_libraries(coreforecast PUBLIC OpenMP::OpenMP_CXX)
 endif()
```

### Comparing `coreforecast-0.0.8/LICENSE` & `coreforecast-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `coreforecast-0.0.8/README.md` & `coreforecast-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `coreforecast-0.0.8/coreforecast/differences.py` & `coreforecast-0.0.9/python/coreforecast/differences.py`

 * *Files identical despite different names*

### Comparing `coreforecast-0.0.8/coreforecast/grouped_array.py` & `coreforecast-0.0.9/python/coreforecast/grouped_array.py`

 * *Files identical despite different names*

### Comparing `coreforecast-0.0.8/coreforecast/lag_transforms.py` & `coreforecast-0.0.9/python/coreforecast/lag_transforms.py`

 * *Files identical despite different names*

### Comparing `coreforecast-0.0.8/coreforecast/scalers.py` & `coreforecast-0.0.9/python/coreforecast/scalers.py`

 * *Files identical despite different names*

### Comparing `coreforecast-0.0.8/coreforecast/seasonal.py` & `coreforecast-0.0.9/python/coreforecast/seasonal.py`

 * *Files identical despite different names*

### Comparing `coreforecast-0.0.8/coreforecast/utils.py` & `coreforecast-0.0.9/python/coreforecast/utils.py`

 * *Files identical despite different names*

### Comparing `coreforecast-0.0.8/docs/mintlify/dark.png` & `coreforecast-0.0.9/docs/mintlify/dark.png`

 * *Files identical despite different names*

### Comparing `coreforecast-0.0.8/docs/mintlify/favicon.svg` & `coreforecast-0.0.9/docs/mintlify/favicon.svg`

 * *Files identical despite different names*

### Comparing `coreforecast-0.0.8/docs/mintlify/light.png` & `coreforecast-0.0.9/docs/mintlify/light.png`

 * *Files identical despite different names*

### Comparing `coreforecast-0.0.8/docs/mintlify/mint.json` & `coreforecast-0.0.9/docs/mintlify/mint.json`

 * *Files identical despite different names*

### Comparing `coreforecast-0.0.8/docs/to_mdx.py` & `coreforecast-0.0.9/docs/to_mdx.py`

 * *Files identical despite different names*

### Comparing `coreforecast-0.0.8/include/brent.h` & `coreforecast-0.0.9/include/brent.h`

 * *Files identical despite different names*

### Comparing `coreforecast-0.0.8/include/grouped_array.h` & `coreforecast-0.0.9/include/grouped_array.h`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 #pragma once
 
 #include <algorithm>
 #include <cmath>
 #include <cstdint>
 
-#include "export.h"
-
 using GroupedArrayHandle = void *;
 using indptr_t = int32_t;
 
 template <typename T> inline indptr_t FirstNotNaN(const T *data, indptr_t n) {
   indptr_t i = 0;
   while (std::isnan(data[i]) && i < n) {
     ++i;
```

### Comparing `coreforecast-0.0.8/include/kpss.h` & `coreforecast-0.0.9/include/kpss.h`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 #pragma once
 
-#include "export.h"
 #include "stats.h"
 
 #include <cmath>
 #include <numeric>
 #include <vector>
 
 template <typename T> T KPSS(const T *x, size_t n, size_t lags) {
```

### Comparing `coreforecast-0.0.8/include/seasonal.h` & `coreforecast-0.0.9/include/seasonal.h`

 * *Files 11% similar despite different names*

```diff
@@ -1,16 +1,25 @@
 #pragma once
 
-#include "diff.h"
-#include "export.h"
 #include "stats.h"
 #include "stl.hpp"
 
 #include <cmath>
 
+template <typename T> void Difference(const T *data, int n, T *out, int d) {
+  if (d == 0) {
+    std::copy(data, data + n, out);
+    return;
+  }
+  std::fill(out, out + d, std::numeric_limits<T>::quiet_NaN());
+  for (int i = d; i < n; ++i) {
+    out[i] = data[i] - data[i - d];
+  }
+}
+
 template <typename T> T SeasHeuristic(const T *x, size_t n, size_t period) {
   constexpr size_t seasonal = 11;
   size_t trend_length =
       static_cast<size_t>(std::ceil(1.5 * period / (1.0 - 1.5 / seasonal)));
   trend_length += trend_length % 2 == 0;
   size_t low_pass = period + (period % 2 == 0);
   stl::StlResult stl_fit = stl::params<T>()
```

### Comparing `coreforecast-0.0.8/include/stats.h` & `coreforecast-0.0.9/include/stats.h`

 * *Files 13% similar despite different names*

```diff
@@ -1,32 +1,36 @@
 #pragma once
 
+#include "SkipList.h"
+
 #include <algorithm>
 #include <numeric>
 
 template <typename T> inline T Quantile(T *data, T p, int n) {
   T i_plus_g = p * (n - 1);
   int i = static_cast<int>(i_plus_g);
   T g = i_plus_g - i;
   std::nth_element(data, data + i, data + n);
   T out = data[i];
   if (g > 0.0) {
-    std::nth_element(data, data + i + 1, data + n);
-    out += g * (data[i + 1] - out);
+    auto it = std::min_element(data + i + 1, data + n);
+    out += g * (*it - out);
   }
   return out;
 }
 
-template <typename T> inline T SortedQuantile(T *data, T p, int n) {
+template <typename T>
+inline T SortedQuantile(OrderedStructs::SkipList::HeadNode<T> &data, T p,
+                        int n) {
   T i_plus_g = p * (n - 1);
   int i = static_cast<int>(i_plus_g);
   T g = i_plus_g - i;
-  T out = data[i];
+  T out = data.at(i);
   if (g > 0.0) {
-    out += g * (data[i + 1] - out);
+    out += g * (data.at(i + 1) - out);
   }
   return out;
 }
 
 template <typename T> double Mean(const T *data, int n) {
   double sum = std::accumulate(data, data + n, 0.0);
   return sum / n;
```

### Comparing `coreforecast-0.0.8/pyproject.toml` & `coreforecast-0.0.9/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "coreforecast"
-version = "0.0.8"
+version = "0.0.9"
 requires-python = ">=3.8"
 dependencies = [
     "importlib_resources ; python_version < '3.10'",
     "numpy>=1.20.0",
 ]
 license = { text = "Apache-2.0" }
 classifiers = [
@@ -14,17 +14,15 @@
     "Natural Language :: English",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
 ]
 description = "Fast implementations of common forecasting routines"
-authors = [
-    {name = "José Morales", email = "jmoralz92@gmail.com"},
-]
+authors = [{ name = "José Morales", email = "jmoralz92@gmail.com" }]
 readme = "README.md"
 keywords = ["forecasting", "time-series"]
 
 [project.urls]
 homepage = "https://nixtla.github.io/coreforecast"
 documentation = "https://nixtla.github.io/coreforecast"
 repository = "https://github.com/Nixtla/coreforecast"
@@ -35,19 +33,15 @@
 
 [tool.scikit-build]
 cmake.verbose = true
 logging.level = "INFO"
 sdist.exclude = ["tests", "*.yml"]
 sdist.reproducible = true
 wheel.install-dir = "coreforecast"
-wheel.packages = ["coreforecast"]
+wheel.packages = ["python/coreforecast"]
 wheel.py-api = "py3"
 
 [tool.cibuildwheel]
 archs = "all"
 build-verbosity = 3
-macos.before-build = [
-    "brew install libomp",
-    "./scripts/switch_xcode",
-]
-test-requires = "pandas pytest window-ops"
-test-command = "pytest {project}/tests -k correct"
+macos.before-build = ["brew install libomp", "./scripts/switch_xcode"]
+test-command = 'python -c "import coreforecast._lib"'
```

### Comparing `coreforecast-0.0.8/PKG-INFO` & `coreforecast-0.0.9/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: coreforecast
-Version: 0.0.8
+Version: 0.0.9
 Summary: Fast implementations of common forecasting routines
-Keywords: forecasting time-series
+Keywords: forecasting,time-series
 Home-page: https://nixtla.github.io/coreforecast
-Author-Email: José Morales <jmoralz92@gmail.com>
+Author-Email: =?utf-8?q?Jos=C3=A9_Morales?= <jmoralz92@gmail.com>
 License: Apache-2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

