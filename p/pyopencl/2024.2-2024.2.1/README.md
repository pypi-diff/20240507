# Comparing `tmp/pyopencl-2024.2.tar.gz` & `tmp/pyopencl-2024.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyopencl-2024.2.tar", last modified: Sun May  5 15:53:41 2024, max compression
+gzip compressed data, was "pyopencl-2024.2.1.tar", last modified: Tue May  7 14:22:45 2024, max compression
```

## Comparing `pyopencl-2024.2.tar` & `pyopencl-2024.2.1.tar`

### file list

```diff
@@ -1,141 +1,142 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 15:53:41.178653 pyopencl-2024.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1910 2024-05-05 15:53:24.000000 pyopencl-2024.2/CITATION.cff
--rw-r--r--   0 runner    (1001) docker     (127)     3844 2024-05-05 15:53:24.000000 pyopencl-2024.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      570 2024-05-05 15:53:24.000000 pyopencl-2024.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      323 2024-05-05 15:53:24.000000 pyopencl-2024.2/Makefile.in
--rw-r--r--   0 runner    (1001) docker     (127)     4536 2024-05-05 15:53:41.178653 pyopencl-2024.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3233 2024-05-05 15:53:24.000000 pyopencl-2024.2/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1090 2024-05-05 15:53:24.000000 pyopencl-2024.2/README_SETUP.txt
--rw-r--r--   0 runner    (1001) docker     (127)    32285 2024-05-05 15:53:24.000000 pyopencl-2024.2/aksetup_helper.py
--rwxr-xr-x   0 runner    (1001) docker     (127)       94 2024-05-05 15:53:24.000000 pyopencl-2024.2/configure.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 15:53:41.162653 pyopencl-2024.2/contrib/
--rw-r--r--   0 runner    (1001) docker     (127)     3638 2024-05-05 15:53:24.000000 pyopencl-2024.2/contrib/cldis.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 15:53:41.162653 pyopencl-2024.2/contrib/fortran-to-opencl/
--rw-r--r--   0 runner    (1001) docker     (127)      889 2024-05-05 15:53:24.000000 pyopencl-2024.2/contrib/fortran-to-opencl/README
--rw-r--r--   0 runner    (1001) docker     (127)    43618 2024-05-05 15:53:24.000000 pyopencl-2024.2/contrib/fortran-to-opencl/translate.py
--rw-r--r--   0 runner    (1001) docker     (127)     2379 2024-05-05 15:53:24.000000 pyopencl-2024.2/contrib/pyopencl.vim
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 15:53:41.162653 pyopencl-2024.2/doc/
--rw-r--r--   0 runner    (1001) docker     (127)      726 2024-05-05 15:53:24.000000 pyopencl-2024.2/doc/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     6878 2024-05-05 15:53:24.000000 pyopencl-2024.2/doc/algorithm.rst
--rw-r--r--   0 runner    (1001) docker     (127)     8473 2024-05-05 15:53:24.000000 pyopencl-2024.2/doc/array.rst
--rw-r--r--   0 runner    (1001) docker     (127)      861 2024-05-05 15:53:24.000000 pyopencl-2024.2/doc/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     3432 2024-05-05 15:53:24.000000 pyopencl-2024.2/doc/howto.rst
--rw-r--r--   0 runner    (1001) docker     (127)     5465 2024-05-05 15:53:24.000000 pyopencl-2024.2/doc/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)    17804 2024-05-05 15:53:24.000000 pyopencl-2024.2/doc/make_constants.py
--rw-r--r--   0 runner    (1001) docker     (127)    29441 2024-05-05 15:53:24.000000 pyopencl-2024.2/doc/misc.rst
--rw-r--r--   0 runner    (1001) docker     (127)      968 2024-05-05 15:53:24.000000 pyopencl-2024.2/doc/runtime.rst
--rw-r--r--   0 runner    (1001) docker     (127)      572 2024-05-05 15:53:24.000000 pyopencl-2024.2/doc/runtime_const.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2206 2024-05-05 15:53:24.000000 pyopencl-2024.2/doc/runtime_gl.rst
--rw-r--r--   0 runner    (1001) docker     (127)    17090 2024-05-05 15:53:24.000000 pyopencl-2024.2/doc/runtime_memory.rst
--rw-r--r--   0 runner    (1001) docker     (127)     5634 2024-05-05 15:53:24.000000 pyopencl-2024.2/doc/runtime_platform.rst
--rw-r--r--   0 runner    (1001) docker     (127)    12672 2024-05-05 15:53:24.000000 pyopencl-2024.2/doc/runtime_program.rst
--rw-r--r--   0 runner    (1001) docker     (127)     5231 2024-05-05 15:53:24.000000 pyopencl-2024.2/doc/runtime_queue.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2244 2024-05-05 15:53:24.000000 pyopencl-2024.2/doc/subst.rst
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-05 15:53:24.000000 pyopencl-2024.2/doc/tools.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1246 2024-05-05 15:53:24.000000 pyopencl-2024.2/doc/types.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 15:53:41.166653 pyopencl-2024.2/examples/
--rw-r--r--   0 runner    (1001) docker     (127)    54750 2024-05-05 15:53:24.000000 pyopencl-2024.2/examples/black-hole-accretion.py
--rw-r--r--   0 runner    (1001) docker     (127)     1824 2024-05-05 15:53:24.000000 pyopencl-2024.2/examples/demo-struct-reduce.py
--rw-r--r--   0 runner    (1001) docker     (127)     1013 2024-05-05 15:53:24.000000 pyopencl-2024.2/examples/demo.py
--rw-r--r--   0 runner    (1001) docker     (127)      838 2024-05-05 15:53:24.000000 pyopencl-2024.2/examples/demo_array.py
--rw-r--r--   0 runner    (1001) docker     (127)      938 2024-05-05 15:53:24.000000 pyopencl-2024.2/examples/demo_array_svm.py
--rw-r--r--   0 runner    (1001) docker     (127)      817 2024-05-05 15:53:24.000000 pyopencl-2024.2/examples/demo_elementwise.py
--rw-r--r--   0 runner    (1001) docker     (127)     1525 2024-05-05 15:53:24.000000 pyopencl-2024.2/examples/demo_elementwise_complex.py
--rw-r--r--   0 runner    (1001) docker     (127)     5051 2024-05-05 15:53:24.000000 pyopencl-2024.2/examples/demo_mandelbrot.py
--rw-r--r--   0 runner    (1001) docker     (127)     1707 2024-05-05 15:53:24.000000 pyopencl-2024.2/examples/demo_meta_codepy.py
--rw-r--r--   0 runner    (1001) docker     (127)     1475 2024-05-05 15:53:24.000000 pyopencl-2024.2/examples/demo_meta_template.py
--rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-05-05 15:53:24.000000 pyopencl-2024.2/examples/dump-performance.py
--rw-r--r--   0 runner    (1001) docker     (127)     3284 2024-05-05 15:53:24.000000 pyopencl-2024.2/examples/dump-properties.py
--rw-r--r--   0 runner    (1001) docker     (127)     2435 2024-05-05 15:53:24.000000 pyopencl-2024.2/examples/gl_interop_demo.py
--rw-r--r--   0 runner    (1001) docker     (127)     6534 2024-05-05 15:53:24.000000 pyopencl-2024.2/examples/gl_particle_animation.py
--rw-r--r--   0 runner    (1001) docker     (127)     3985 2024-05-05 15:53:24.000000 pyopencl-2024.2/examples/ipython-demo.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     2648 2024-05-05 15:53:24.000000 pyopencl-2024.2/examples/median-filter.py
--rw-r--r--   0 runner    (1001) docker     (127)    32124 2024-05-05 15:53:24.000000 pyopencl-2024.2/examples/n-body.py
--rw-r--r--   0 runner    (1001) docker     (127)      707 2024-05-05 15:53:24.000000 pyopencl-2024.2/examples/narray.py
--rw-r--r--   0 runner    (1001) docker     (127)    66806 2024-05-05 15:53:24.000000 pyopencl-2024.2/examples/noisyImage.jpg
--rw-r--r--   0 runner    (1001) docker     (127)    35442 2024-05-05 15:53:24.000000 pyopencl-2024.2/examples/pi-monte-carlo.py
--rw-r--r--   0 runner    (1001) docker     (127)     1981 2024-05-05 15:53:24.000000 pyopencl-2024.2/examples/svm.py
--rw-r--r--   0 runner    (1001) docker     (127)     6484 2024-05-05 15:53:24.000000 pyopencl-2024.2/examples/transpose.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 15:53:41.170653 pyopencl-2024.2/pyopencl/
--rw-r--r--   0 runner    (1001) docker     (127)    80676 2024-05-05 15:53:24.000000 pyopencl-2024.2/pyopencl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2074 2024-05-05 15:53:24.000000 pyopencl-2024.2/pyopencl/_cluda.py
--rw-r--r--   0 runner    (1001) docker     (127)      610 2024-05-05 15:53:24.000000 pyopencl-2024.2/pyopencl/_mymako.py
--rw-r--r--   0 runner    (1001) docker     (127)    51196 2024-05-05 15:53:24.000000 pyopencl-2024.2/pyopencl/algorithm.py
--rw-r--r--   0 runner    (1001) docker     (127)   111717 2024-05-05 15:53:24.000000 pyopencl-2024.2/pyopencl/array.py
--rw-r--r--   0 runner    (1001) docker     (127)     7876 2024-05-05 15:53:24.000000 pyopencl-2024.2/pyopencl/bitonic_sort.py
--rw-r--r--   0 runner    (1001) docker     (127)    16172 2024-05-05 15:53:24.000000 pyopencl-2024.2/pyopencl/bitonic_sort_templates.py
--rw-r--r--   0 runner    (1001) docker     (127)    15959 2024-05-05 15:53:24.000000 pyopencl-2024.2/pyopencl/cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     5661 2024-05-05 15:53:24.000000 pyopencl-2024.2/pyopencl/capture_call.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 15:53:41.170653 pyopencl-2024.2/pyopencl/characterize/
--rw-r--r--   0 runner    (1001) docker     (127)    13829 2024-05-05 15:53:24.000000 pyopencl-2024.2/pyopencl/characterize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6866 2024-05-05 15:53:24.000000 pyopencl-2024.2/pyopencl/characterize/performance.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 15:53:41.174653 pyopencl-2024.2/pyopencl/cl/
--rw-r--r--   0 runner    (1001) docker     (127)     8122 2024-05-05 15:53:24.000000 pyopencl-2024.2/pyopencl/cl/pyopencl-airy.cl
--rw-r--r--   0 runner    (1001) docker     (127)     6026 2024-05-05 15:53:24.000000 pyopencl-2024.2/pyopencl/cl/pyopencl-bessel-j-complex.cl
--rw-r--r--   0 runner    (1001) docker     (127)    23274 2024-05-05 15:53:24.000000 pyopencl-2024.2/pyopencl/cl/pyopencl-bessel-j.cl
--rw-r--r--   0 runner    (1001) docker     (127)    12297 2024-05-05 15:53:24.000000 pyopencl-2024.2/pyopencl/cl/pyopencl-bessel-y.cl
--rw-r--r--   0 runner    (1001) docker     (127)     8544 2024-05-05 15:53:24.000000 pyopencl-2024.2/pyopencl/cl/pyopencl-complex.h
--rw-r--r--   0 runner    (1001) docker     (127)     2616 2024-05-05 15:53:24.000000 pyopencl-2024.2/pyopencl/cl/pyopencl-eval-tbl.cl
--rw-r--r--   0 runner    (1001) docker     (127)    31561 2024-05-05 15:53:24.000000 pyopencl-2024.2/pyopencl/cl/pyopencl-hankel-complex.cl
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 15:53:41.174653 pyopencl-2024.2/pyopencl/cl/pyopencl-random123/
--rw-r--r--   0 runner    (1001) docker     (127)    17088 2024-05-05 15:53:24.000000 pyopencl-2024.2/pyopencl/cl/pyopencl-random123/array.h
--rw-r--r--   0 runner    (1001) docker     (127)     2881 2024-05-05 15:53:24.000000 pyopencl-2024.2/pyopencl/cl/pyopencl-random123/openclfeatures.h
--rw-r--r--   0 runner    (1001) docker     (127)    21740 2024-05-05 15:53:24.000000 pyopencl-2024.2/pyopencl/cl/pyopencl-random123/philox.cl
--rw-r--r--   0 runner    (1001) docker     (127)    54699 2024-05-05 15:53:24.000000 pyopencl-2024.2/pyopencl/cl/pyopencl-random123/threefry.cl
--rw-r--r--   0 runner    (1001) docker     (127)     8222 2024-05-05 15:53:24.000000 pyopencl-2024.2/pyopencl/clmath.py
--rw-r--r--   0 runner    (1001) docker     (127)    13043 2024-05-05 15:53:24.000000 pyopencl-2024.2/pyopencl/clrandom.py
--rw-r--r--   0 runner    (1001) docker     (127)     4818 2024-05-05 15:53:24.000000 pyopencl-2024.2/pyopencl/cltypes.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 15:53:41.174653 pyopencl-2024.2/pyopencl/compyte/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 15:53:40.000000 pyopencl-2024.2/pyopencl/compyte/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7422 2024-05-05 15:53:40.000000 pyopencl-2024.2/pyopencl/compyte/array.py
--rw-r--r--   0 runner    (1001) docker     (127)     9809 2024-05-05 15:53:40.000000 pyopencl-2024.2/pyopencl/compyte/dtypes.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 15:53:41.174653 pyopencl-2024.2/pyopencl/compyte/ndarray/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 15:53:40.000000 pyopencl-2024.2/pyopencl/compyte/ndarray/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    76820 2024-05-05 15:53:40.000000 pyopencl-2024.2/pyopencl/compyte/ndarray/gen_elemwise.py
--rw-r--r--   0 runner    (1001) docker     (127)    56315 2024-05-05 15:53:40.000000 pyopencl-2024.2/pyopencl/compyte/ndarray/gen_reduction.py
--rw-r--r--   0 runner    (1001) docker     (127)     3809 2024-05-05 15:53:40.000000 pyopencl-2024.2/pyopencl/compyte/ndarray/setup_opencl.py
--rw-r--r--   0 runner    (1001) docker     (127)    18438 2024-05-05 15:53:40.000000 pyopencl-2024.2/pyopencl/compyte/ndarray/test_gpu_elemwise.py
--rw-r--r--   0 runner    (1001) docker     (127)    17781 2024-05-05 15:53:40.000000 pyopencl-2024.2/pyopencl/compyte/ndarray/test_gpu_ndarray.py
--rw-r--r--   0 runner    (1001) docker     (127)    38602 2024-05-05 15:53:24.000000 pyopencl-2024.2/pyopencl/elementwise.py
--rw-r--r--   0 runner    (1001) docker     (127)    13994 2024-05-05 15:53:24.000000 pyopencl-2024.2/pyopencl/invoker.py
--rw-r--r--   0 runner    (1001) docker     (127)     1914 2024-05-05 15:53:24.000000 pyopencl-2024.2/pyopencl/ipython_ext.py
--rw-r--r--   0 runner    (1001) docker     (127)    25524 2024-05-05 15:53:24.000000 pyopencl-2024.2/pyopencl/reduction.py
--rw-r--r--   0 runner    (1001) docker     (127)    65500 2024-05-05 15:53:24.000000 pyopencl-2024.2/pyopencl/scan.py
--rw-r--r--   0 runner    (1001) docker     (127)    45510 2024-05-05 15:53:24.000000 pyopencl-2024.2/pyopencl/tools.py
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-05 15:53:24.000000 pyopencl-2024.2/pyopencl/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 15:53:41.178653 pyopencl-2024.2/pyopencl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4536 2024-05-05 15:53:41.000000 pyopencl-2024.2/pyopencl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3038 2024-05-05 15:53:41.000000 pyopencl-2024.2/pyopencl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-05 15:53:41.000000 pyopencl-2024.2/pyopencl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-05 15:53:40.000000 pyopencl-2024.2/pyopencl.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      204 2024-05-05 15:53:41.000000 pyopencl-2024.2/pyopencl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-05 15:53:41.000000 pyopencl-2024.2/pyopencl.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1939 2024-05-05 15:53:24.000000 pyopencl-2024.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-05 15:53:24.000000 pyopencl-2024.2/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-05-05 15:53:41.178653 pyopencl-2024.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     8648 2024-05-05 15:53:24.000000 pyopencl-2024.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 15:53:41.178653 pyopencl-2024.2/src/
--rw-r--r--   0 runner    (1001) docker     (127)     2083 2024-05-05 15:53:24.000000 pyopencl-2024.2/src/bitlog.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2170 2024-05-05 15:53:24.000000 pyopencl-2024.2/src/bitlog.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     4542 2024-05-05 15:53:24.000000 pyopencl-2024.2/src/clinfo_ext.h
--rw-r--r--   0 runner    (1001) docker     (127)    11806 2024-05-05 15:53:24.000000 pyopencl-2024.2/src/mempool.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     2109 2024-05-05 15:53:24.000000 pyopencl-2024.2/src/pyopencl_ext.h
--rw-r--r--   0 runner    (1001) docker     (127)     2348 2024-05-05 15:53:24.000000 pyopencl-2024.2/src/tools.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1805 2024-05-05 15:53:24.000000 pyopencl-2024.2/src/wrap_cl.cpp
--rw-r--r--   0 runner    (1001) docker     (127)   165179 2024-05-05 15:53:24.000000 pyopencl-2024.2/src/wrap_cl.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    10872 2024-05-05 15:53:24.000000 pyopencl-2024.2/src/wrap_cl_part_1.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    19945 2024-05-05 15:53:24.000000 pyopencl-2024.2/src/wrap_cl_part_2.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    38496 2024-05-05 15:53:24.000000 pyopencl-2024.2/src/wrap_constants.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     6579 2024-05-05 15:53:24.000000 pyopencl-2024.2/src/wrap_helpers.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    18776 2024-05-05 15:53:24.000000 pyopencl-2024.2/src/wrap_mempool.cpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 15:53:41.178653 pyopencl-2024.2/test/
--rw-r--r--   0 runner    (1001) docker     (127)      792 2024-05-05 15:53:24.000000 pyopencl-2024.2/test/add-vectors-32.spv
--rw-r--r--   0 runner    (1001) docker     (127)      952 2024-05-05 15:53:24.000000 pyopencl-2024.2/test/add-vectors-64.spv
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-05 15:53:24.000000 pyopencl-2024.2/test/empty-header.h
--rw-r--r--   0 runner    (1001) docker     (127)    35331 2024-05-05 15:53:24.000000 pyopencl-2024.2/test/test_algorithm.py
--rw-r--r--   0 runner    (1001) docker     (127)    63792 2024-05-05 15:53:24.000000 pyopencl-2024.2/test/test_array.py
--rw-r--r--   0 runner    (1001) docker     (127)     3515 2024-05-05 15:53:24.000000 pyopencl-2024.2/test/test_arrays_in_structs.py
--rw-r--r--   0 runner    (1001) docker     (127)    16184 2024-05-05 15:53:24.000000 pyopencl-2024.2/test/test_clmath.py
--rw-r--r--   0 runner    (1001) docker     (127)     2460 2024-05-05 15:53:24.000000 pyopencl-2024.2/test/test_clrandom.py
--rw-r--r--   0 runner    (1001) docker     (127)     9776 2024-05-05 15:53:24.000000 pyopencl-2024.2/test/test_enqueue_copy.py
--rw-r--r--   0 runner    (1001) docker     (127)    44638 2024-05-05 15:53:24.000000 pyopencl-2024.2/test/test_wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:22:45.268943 pyopencl-2024.2.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1910 2024-05-07 14:22:29.000000 pyopencl-2024.2.1/CITATION.cff
+-rw-r--r--   0 runner    (1001) docker     (127)     2209 2024-05-07 14:22:29.000000 pyopencl-2024.2.1/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3844 2024-05-07 14:22:29.000000 pyopencl-2024.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      594 2024-05-07 14:22:29.000000 pyopencl-2024.2.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      323 2024-05-07 14:22:29.000000 pyopencl-2024.2.1/Makefile.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4538 2024-05-07 14:22:45.268943 pyopencl-2024.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3233 2024-05-07 14:22:29.000000 pyopencl-2024.2.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1090 2024-05-07 14:22:29.000000 pyopencl-2024.2.1/README_SETUP.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    32285 2024-05-07 14:22:29.000000 pyopencl-2024.2.1/aksetup_helper.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)       94 2024-05-07 14:22:29.000000 pyopencl-2024.2.1/configure.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:22:45.248943 pyopencl-2024.2.1/contrib/
+-rw-r--r--   0 runner    (1001) docker     (127)     3638 2024-05-07 14:22:29.000000 pyopencl-2024.2.1/contrib/cldis.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:22:45.248943 pyopencl-2024.2.1/contrib/fortran-to-opencl/
+-rw-r--r--   0 runner    (1001) docker     (127)      889 2024-05-07 14:22:29.000000 pyopencl-2024.2.1/contrib/fortran-to-opencl/README
+-rw-r--r--   0 runner    (1001) docker     (127)    43618 2024-05-07 14:22:29.000000 pyopencl-2024.2.1/contrib/fortran-to-opencl/translate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2379 2024-05-07 14:22:29.000000 pyopencl-2024.2.1/contrib/pyopencl.vim
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:22:45.252943 pyopencl-2024.2.1/doc/
+-rw-r--r--   0 runner    (1001) docker     (127)      726 2024-05-07 14:22:29.000000 pyopencl-2024.2.1/doc/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     6878 2024-05-07 14:22:29.000000 pyopencl-2024.2.1/doc/algorithm.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     8473 2024-05-07 14:22:29.000000 pyopencl-2024.2.1/doc/array.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      861 2024-05-07 14:22:29.000000 pyopencl-2024.2.1/doc/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3432 2024-05-07 14:22:29.000000 pyopencl-2024.2.1/doc/howto.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     5465 2024-05-07 14:22:29.000000 pyopencl-2024.2.1/doc/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    17804 2024-05-07 14:22:29.000000 pyopencl-2024.2.1/doc/make_constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29441 2024-05-07 14:22:29.000000 pyopencl-2024.2.1/doc/misc.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      968 2024-05-07 14:22:29.000000 pyopencl-2024.2.1/doc/runtime.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      572 2024-05-07 14:22:29.000000 pyopencl-2024.2.1/doc/runtime_const.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2206 2024-05-07 14:22:29.000000 pyopencl-2024.2.1/doc/runtime_gl.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    17090 2024-05-07 14:22:29.000000 pyopencl-2024.2.1/doc/runtime_memory.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     5634 2024-05-07 14:22:29.000000 pyopencl-2024.2.1/doc/runtime_platform.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    12672 2024-05-07 14:22:29.000000 pyopencl-2024.2.1/doc/runtime_program.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     5231 2024-05-07 14:22:29.000000 pyopencl-2024.2.1/doc/runtime_queue.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2244 2024-05-07 14:22:29.000000 pyopencl-2024.2.1/doc/subst.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-07 14:22:29.000000 pyopencl-2024.2.1/doc/tools.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1246 2024-05-07 14:22:29.000000 pyopencl-2024.2.1/doc/types.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:22:45.256943 pyopencl-2024.2.1/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)    54750 2024-05-07 14:22:29.000000 pyopencl-2024.2.1/examples/black-hole-accretion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1824 2024-05-07 14:22:29.000000 pyopencl-2024.2.1/examples/demo-struct-reduce.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1013 2024-05-07 14:22:29.000000 pyopencl-2024.2.1/examples/demo.py
+-rw-r--r--   0 runner    (1001) docker     (127)      838 2024-05-07 14:22:29.000000 pyopencl-2024.2.1/examples/demo_array.py
+-rw-r--r--   0 runner    (1001) docker     (127)      938 2024-05-07 14:22:29.000000 pyopencl-2024.2.1/examples/demo_array_svm.py
+-rw-r--r--   0 runner    (1001) docker     (127)      817 2024-05-07 14:22:29.000000 pyopencl-2024.2.1/examples/demo_elementwise.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1525 2024-05-07 14:22:29.000000 pyopencl-2024.2.1/examples/demo_elementwise_complex.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5051 2024-05-07 14:22:29.000000 pyopencl-2024.2.1/examples/demo_mandelbrot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1707 2024-05-07 14:22:29.000000 pyopencl-2024.2.1/examples/demo_meta_codepy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1475 2024-05-07 14:22:29.000000 pyopencl-2024.2.1/examples/demo_meta_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-05-07 14:22:29.000000 pyopencl-2024.2.1/examples/dump-performance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3284 2024-05-07 14:22:29.000000 pyopencl-2024.2.1/examples/dump-properties.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2435 2024-05-07 14:22:29.000000 pyopencl-2024.2.1/examples/gl_interop_demo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6534 2024-05-07 14:22:29.000000 pyopencl-2024.2.1/examples/gl_particle_animation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3985 2024-05-07 14:22:29.000000 pyopencl-2024.2.1/examples/ipython-demo.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     2648 2024-05-07 14:22:29.000000 pyopencl-2024.2.1/examples/median-filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32124 2024-05-07 14:22:29.000000 pyopencl-2024.2.1/examples/n-body.py
+-rw-r--r--   0 runner    (1001) docker     (127)      707 2024-05-07 14:22:29.000000 pyopencl-2024.2.1/examples/narray.py
+-rw-r--r--   0 runner    (1001) docker     (127)    66806 2024-05-07 14:22:29.000000 pyopencl-2024.2.1/examples/noisyImage.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)    35442 2024-05-07 14:22:29.000000 pyopencl-2024.2.1/examples/pi-monte-carlo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1981 2024-05-07 14:22:29.000000 pyopencl-2024.2.1/examples/svm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6484 2024-05-07 14:22:29.000000 pyopencl-2024.2.1/examples/transpose.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:22:45.260943 pyopencl-2024.2.1/pyopencl/
+-rw-r--r--   0 runner    (1001) docker     (127)    80676 2024-05-07 14:22:29.000000 pyopencl-2024.2.1/pyopencl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2074 2024-05-07 14:22:29.000000 pyopencl-2024.2.1/pyopencl/_cluda.py
+-rw-r--r--   0 runner    (1001) docker     (127)      610 2024-05-07 14:22:29.000000 pyopencl-2024.2.1/pyopencl/_mymako.py
+-rw-r--r--   0 runner    (1001) docker     (127)    51196 2024-05-07 14:22:29.000000 pyopencl-2024.2.1/pyopencl/algorithm.py
+-rw-r--r--   0 runner    (1001) docker     (127)   111717 2024-05-07 14:22:29.000000 pyopencl-2024.2.1/pyopencl/array.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7876 2024-05-07 14:22:29.000000 pyopencl-2024.2.1/pyopencl/bitonic_sort.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16172 2024-05-07 14:22:29.000000 pyopencl-2024.2.1/pyopencl/bitonic_sort_templates.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15959 2024-05-07 14:22:29.000000 pyopencl-2024.2.1/pyopencl/cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5661 2024-05-07 14:22:29.000000 pyopencl-2024.2.1/pyopencl/capture_call.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:22:45.260943 pyopencl-2024.2.1/pyopencl/characterize/
+-rw-r--r--   0 runner    (1001) docker     (127)    13829 2024-05-07 14:22:29.000000 pyopencl-2024.2.1/pyopencl/characterize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6866 2024-05-07 14:22:29.000000 pyopencl-2024.2.1/pyopencl/characterize/performance.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:22:45.260943 pyopencl-2024.2.1/pyopencl/cl/
+-rw-r--r--   0 runner    (1001) docker     (127)     8122 2024-05-07 14:22:29.000000 pyopencl-2024.2.1/pyopencl/cl/pyopencl-airy.cl
+-rw-r--r--   0 runner    (1001) docker     (127)     6026 2024-05-07 14:22:29.000000 pyopencl-2024.2.1/pyopencl/cl/pyopencl-bessel-j-complex.cl
+-rw-r--r--   0 runner    (1001) docker     (127)    23274 2024-05-07 14:22:29.000000 pyopencl-2024.2.1/pyopencl/cl/pyopencl-bessel-j.cl
+-rw-r--r--   0 runner    (1001) docker     (127)    12297 2024-05-07 14:22:29.000000 pyopencl-2024.2.1/pyopencl/cl/pyopencl-bessel-y.cl
+-rw-r--r--   0 runner    (1001) docker     (127)     8544 2024-05-07 14:22:29.000000 pyopencl-2024.2.1/pyopencl/cl/pyopencl-complex.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2616 2024-05-07 14:22:29.000000 pyopencl-2024.2.1/pyopencl/cl/pyopencl-eval-tbl.cl
+-rw-r--r--   0 runner    (1001) docker     (127)    31561 2024-05-07 14:22:29.000000 pyopencl-2024.2.1/pyopencl/cl/pyopencl-hankel-complex.cl
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:22:45.260943 pyopencl-2024.2.1/pyopencl/cl/pyopencl-random123/
+-rw-r--r--   0 runner    (1001) docker     (127)    17088 2024-05-07 14:22:29.000000 pyopencl-2024.2.1/pyopencl/cl/pyopencl-random123/array.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2881 2024-05-07 14:22:29.000000 pyopencl-2024.2.1/pyopencl/cl/pyopencl-random123/openclfeatures.h
+-rw-r--r--   0 runner    (1001) docker     (127)    21740 2024-05-07 14:22:29.000000 pyopencl-2024.2.1/pyopencl/cl/pyopencl-random123/philox.cl
+-rw-r--r--   0 runner    (1001) docker     (127)    54699 2024-05-07 14:22:29.000000 pyopencl-2024.2.1/pyopencl/cl/pyopencl-random123/threefry.cl
+-rw-r--r--   0 runner    (1001) docker     (127)     8222 2024-05-07 14:22:29.000000 pyopencl-2024.2.1/pyopencl/clmath.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13043 2024-05-07 14:22:29.000000 pyopencl-2024.2.1/pyopencl/clrandom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4818 2024-05-07 14:22:29.000000 pyopencl-2024.2.1/pyopencl/cltypes.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:22:45.264943 pyopencl-2024.2.1/pyopencl/compyte/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 14:22:44.000000 pyopencl-2024.2.1/pyopencl/compyte/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7422 2024-05-07 14:22:44.000000 pyopencl-2024.2.1/pyopencl/compyte/array.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9809 2024-05-07 14:22:44.000000 pyopencl-2024.2.1/pyopencl/compyte/dtypes.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:22:45.264943 pyopencl-2024.2.1/pyopencl/compyte/ndarray/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 14:22:44.000000 pyopencl-2024.2.1/pyopencl/compyte/ndarray/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    76820 2024-05-07 14:22:44.000000 pyopencl-2024.2.1/pyopencl/compyte/ndarray/gen_elemwise.py
+-rw-r--r--   0 runner    (1001) docker     (127)    56315 2024-05-07 14:22:44.000000 pyopencl-2024.2.1/pyopencl/compyte/ndarray/gen_reduction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3809 2024-05-07 14:22:44.000000 pyopencl-2024.2.1/pyopencl/compyte/ndarray/setup_opencl.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18438 2024-05-07 14:22:44.000000 pyopencl-2024.2.1/pyopencl/compyte/ndarray/test_gpu_elemwise.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17781 2024-05-07 14:22:44.000000 pyopencl-2024.2.1/pyopencl/compyte/ndarray/test_gpu_ndarray.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38602 2024-05-07 14:22:29.000000 pyopencl-2024.2.1/pyopencl/elementwise.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13994 2024-05-07 14:22:29.000000 pyopencl-2024.2.1/pyopencl/invoker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1914 2024-05-07 14:22:29.000000 pyopencl-2024.2.1/pyopencl/ipython_ext.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25524 2024-05-07 14:22:29.000000 pyopencl-2024.2.1/pyopencl/reduction.py
+-rw-r--r--   0 runner    (1001) docker     (127)    65500 2024-05-07 14:22:29.000000 pyopencl-2024.2.1/pyopencl/scan.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45510 2024-05-07 14:22:29.000000 pyopencl-2024.2.1/pyopencl/tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-05-07 14:22:29.000000 pyopencl-2024.2.1/pyopencl/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:22:45.268943 pyopencl-2024.2.1/pyopencl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4538 2024-05-07 14:22:45.000000 pyopencl-2024.2.1/pyopencl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3053 2024-05-07 14:22:45.000000 pyopencl-2024.2.1/pyopencl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 14:22:45.000000 pyopencl-2024.2.1/pyopencl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 14:22:44.000000 pyopencl-2024.2.1/pyopencl.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      204 2024-05-07 14:22:45.000000 pyopencl-2024.2.1/pyopencl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-07 14:22:45.000000 pyopencl-2024.2.1/pyopencl.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1939 2024-05-07 14:22:29.000000 pyopencl-2024.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-07 14:22:29.000000 pyopencl-2024.2.1/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-05-07 14:22:45.268943 pyopencl-2024.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     8648 2024-05-07 14:22:29.000000 pyopencl-2024.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:22:45.264943 pyopencl-2024.2.1/src/
+-rw-r--r--   0 runner    (1001) docker     (127)     2083 2024-05-07 14:22:29.000000 pyopencl-2024.2.1/src/bitlog.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2170 2024-05-07 14:22:29.000000 pyopencl-2024.2.1/src/bitlog.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4542 2024-05-07 14:22:29.000000 pyopencl-2024.2.1/src/clinfo_ext.h
+-rw-r--r--   0 runner    (1001) docker     (127)    11806 2024-05-07 14:22:29.000000 pyopencl-2024.2.1/src/mempool.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2109 2024-05-07 14:22:29.000000 pyopencl-2024.2.1/src/pyopencl_ext.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2348 2024-05-07 14:22:29.000000 pyopencl-2024.2.1/src/tools.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1805 2024-05-07 14:22:29.000000 pyopencl-2024.2.1/src/wrap_cl.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)   165179 2024-05-07 14:22:29.000000 pyopencl-2024.2.1/src/wrap_cl.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    10872 2024-05-07 14:22:29.000000 pyopencl-2024.2.1/src/wrap_cl_part_1.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    19945 2024-05-07 14:22:29.000000 pyopencl-2024.2.1/src/wrap_cl_part_2.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    38496 2024-05-07 14:22:29.000000 pyopencl-2024.2.1/src/wrap_constants.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     6579 2024-05-07 14:22:29.000000 pyopencl-2024.2.1/src/wrap_helpers.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    18776 2024-05-07 14:22:29.000000 pyopencl-2024.2.1/src/wrap_mempool.cpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:22:45.268943 pyopencl-2024.2.1/test/
+-rw-r--r--   0 runner    (1001) docker     (127)      792 2024-05-07 14:22:29.000000 pyopencl-2024.2.1/test/add-vectors-32.spv
+-rw-r--r--   0 runner    (1001) docker     (127)      952 2024-05-07 14:22:29.000000 pyopencl-2024.2.1/test/add-vectors-64.spv
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-07 14:22:29.000000 pyopencl-2024.2.1/test/empty-header.h
+-rw-r--r--   0 runner    (1001) docker     (127)    35331 2024-05-07 14:22:29.000000 pyopencl-2024.2.1/test/test_algorithm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    63792 2024-05-07 14:22:29.000000 pyopencl-2024.2.1/test/test_array.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3515 2024-05-07 14:22:29.000000 pyopencl-2024.2.1/test/test_arrays_in_structs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16184 2024-05-07 14:22:29.000000 pyopencl-2024.2.1/test/test_clmath.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2460 2024-05-07 14:22:29.000000 pyopencl-2024.2.1/test/test_clrandom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9776 2024-05-07 14:22:29.000000 pyopencl-2024.2.1/test/test_enqueue_copy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44638 2024-05-07 14:22:29.000000 pyopencl-2024.2.1/test/test_wrapper.py
```

### Comparing `pyopencl-2024.2/CITATION.cff` & `pyopencl-2024.2.1/CITATION.cff`

 * *Files identical despite different names*

### Comparing `pyopencl-2024.2/LICENSE` & `pyopencl-2024.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyopencl-2024.2/MANIFEST.in` & `pyopencl-2024.2.1/MANIFEST.in`

 * *Files 18% similar despite different names*

```diff
@@ -24,7 +24,9 @@
 include LICENSE
 include pytest.ini
 include CITATION.cff
 
 recursive-exclude _skbuild *
 
 recursive-include contrib *.vim *.py README
+
+include CMakeLists.txt
```

### Comparing `pyopencl-2024.2/PKG-INFO` & `pyopencl-2024.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyopencl
-Version: 2024.2
+Version: 2024.2.1
 Summary: Python wrapper for OpenCL
 Home-page: http://mathema.tician.de/software/pyopencl
 Author: Andreas Kloeckner
 Author-email: inform@tiker.net
 License: MIT
 Classifier: Environment :: Console
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `pyopencl-2024.2/README.rst` & `pyopencl-2024.2.1/README.rst`

 * *Files identical despite different names*

### Comparing `pyopencl-2024.2/README_SETUP.txt` & `pyopencl-2024.2.1/README_SETUP.txt`

 * *Files identical despite different names*

### Comparing `pyopencl-2024.2/aksetup_helper.py` & `pyopencl-2024.2.1/aksetup_helper.py`

 * *Files identical despite different names*

### Comparing `pyopencl-2024.2/contrib/cldis.py` & `pyopencl-2024.2.1/contrib/cldis.py`

 * *Files identical despite different names*

### Comparing `pyopencl-2024.2/contrib/fortran-to-opencl/README` & `pyopencl-2024.2.1/contrib/fortran-to-opencl/README`

 * *Files identical despite different names*

### Comparing `pyopencl-2024.2/contrib/fortran-to-opencl/translate.py` & `pyopencl-2024.2.1/contrib/fortran-to-opencl/translate.py`

 * *Files identical despite different names*

### Comparing `pyopencl-2024.2/contrib/pyopencl.vim` & `pyopencl-2024.2.1/contrib/pyopencl.vim`

 * *Files identical despite different names*

### Comparing `pyopencl-2024.2/doc/Makefile` & `pyopencl-2024.2.1/doc/Makefile`

 * *Files identical despite different names*

### Comparing `pyopencl-2024.2/doc/algorithm.rst` & `pyopencl-2024.2.1/doc/algorithm.rst`

 * *Files identical despite different names*

### Comparing `pyopencl-2024.2/doc/array.rst` & `pyopencl-2024.2.1/doc/array.rst`

 * *Files identical despite different names*

### Comparing `pyopencl-2024.2/doc/conf.py` & `pyopencl-2024.2.1/doc/conf.py`

 * *Files identical despite different names*

### Comparing `pyopencl-2024.2/doc/howto.rst` & `pyopencl-2024.2.1/doc/howto.rst`

 * *Files identical despite different names*

### Comparing `pyopencl-2024.2/doc/index.rst` & `pyopencl-2024.2.1/doc/index.rst`

 * *Files identical despite different names*

### Comparing `pyopencl-2024.2/doc/make_constants.py` & `pyopencl-2024.2.1/doc/make_constants.py`

 * *Files identical despite different names*

### Comparing `pyopencl-2024.2/doc/misc.rst` & `pyopencl-2024.2.1/doc/misc.rst`

 * *Files identical despite different names*

### Comparing `pyopencl-2024.2/doc/runtime.rst` & `pyopencl-2024.2.1/doc/runtime.rst`

 * *Files identical despite different names*

### Comparing `pyopencl-2024.2/doc/runtime_const.rst` & `pyopencl-2024.2.1/doc/runtime_const.rst`

 * *Files identical despite different names*

### Comparing `pyopencl-2024.2/doc/runtime_gl.rst` & `pyopencl-2024.2.1/doc/runtime_gl.rst`

 * *Files identical despite different names*

### Comparing `pyopencl-2024.2/doc/runtime_memory.rst` & `pyopencl-2024.2.1/doc/runtime_memory.rst`

 * *Files identical despite different names*

### Comparing `pyopencl-2024.2/doc/runtime_platform.rst` & `pyopencl-2024.2.1/doc/runtime_platform.rst`

 * *Files identical despite different names*

### Comparing `pyopencl-2024.2/doc/runtime_program.rst` & `pyopencl-2024.2.1/doc/runtime_program.rst`

 * *Files identical despite different names*

### Comparing `pyopencl-2024.2/doc/runtime_queue.rst` & `pyopencl-2024.2.1/doc/runtime_queue.rst`

 * *Files identical despite different names*

### Comparing `pyopencl-2024.2/doc/subst.rst` & `pyopencl-2024.2.1/doc/subst.rst`

 * *Files identical despite different names*

### Comparing `pyopencl-2024.2/doc/types.rst` & `pyopencl-2024.2.1/doc/types.rst`

 * *Files identical despite different names*

### Comparing `pyopencl-2024.2/examples/black-hole-accretion.py` & `pyopencl-2024.2.1/examples/black-hole-accretion.py`

 * *Files identical despite different names*

### Comparing `pyopencl-2024.2/examples/demo-struct-reduce.py` & `pyopencl-2024.2.1/examples/demo-struct-reduce.py`

 * *Files identical despite different names*

### Comparing `pyopencl-2024.2/examples/demo.py` & `pyopencl-2024.2.1/examples/demo.py`

 * *Files identical despite different names*

### Comparing `pyopencl-2024.2/examples/demo_array.py` & `pyopencl-2024.2.1/examples/demo_array.py`

 * *Files identical despite different names*

### Comparing `pyopencl-2024.2/examples/demo_array_svm.py` & `pyopencl-2024.2.1/examples/demo_array_svm.py`

 * *Files identical despite different names*

### Comparing `pyopencl-2024.2/examples/demo_elementwise.py` & `pyopencl-2024.2.1/examples/demo_elementwise.py`

 * *Files identical despite different names*

### Comparing `pyopencl-2024.2/examples/demo_elementwise_complex.py` & `pyopencl-2024.2.1/examples/demo_elementwise_complex.py`

 * *Files identical despite different names*

### Comparing `pyopencl-2024.2/examples/demo_mandelbrot.py` & `pyopencl-2024.2.1/examples/demo_mandelbrot.py`

 * *Files identical despite different names*

### Comparing `pyopencl-2024.2/examples/demo_meta_codepy.py` & `pyopencl-2024.2.1/examples/demo_meta_codepy.py`

 * *Files identical despite different names*

### Comparing `pyopencl-2024.2/examples/demo_meta_template.py` & `pyopencl-2024.2.1/examples/demo_meta_template.py`

 * *Files identical despite different names*

### Comparing `pyopencl-2024.2/examples/dump-performance.py` & `pyopencl-2024.2.1/examples/dump-performance.py`

 * *Files identical despite different names*

### Comparing `pyopencl-2024.2/examples/dump-properties.py` & `pyopencl-2024.2.1/examples/dump-properties.py`

 * *Files identical despite different names*

### Comparing `pyopencl-2024.2/examples/gl_interop_demo.py` & `pyopencl-2024.2.1/examples/gl_interop_demo.py`

 * *Files identical despite different names*

### Comparing `pyopencl-2024.2/examples/gl_particle_animation.py` & `pyopencl-2024.2.1/examples/gl_particle_animation.py`

 * *Files identical despite different names*

### Comparing `pyopencl-2024.2/examples/ipython-demo.ipynb` & `pyopencl-2024.2.1/examples/ipython-demo.ipynb`

 * *Files identical despite different names*

### Comparing `pyopencl-2024.2/examples/median-filter.py` & `pyopencl-2024.2.1/examples/median-filter.py`

 * *Files identical despite different names*

### Comparing `pyopencl-2024.2/examples/n-body.py` & `pyopencl-2024.2.1/examples/n-body.py`

 * *Files identical despite different names*

### Comparing `pyopencl-2024.2/examples/narray.py` & `pyopencl-2024.2.1/examples/narray.py`

 * *Files identical despite different names*

### Comparing `pyopencl-2024.2/examples/noisyImage.jpg` & `pyopencl-2024.2.1/examples/noisyImage.jpg`

 * *Files identical despite different names*

### Comparing `pyopencl-2024.2/examples/pi-monte-carlo.py` & `pyopencl-2024.2.1/examples/pi-monte-carlo.py`

 * *Files identical despite different names*

### Comparing `pyopencl-2024.2/examples/svm.py` & `pyopencl-2024.2.1/examples/svm.py`

 * *Files identical despite different names*

### Comparing `pyopencl-2024.2/examples/transpose.py` & `pyopencl-2024.2.1/examples/transpose.py`

 * *Files identical despite different names*

### Comparing `pyopencl-2024.2/pyopencl/__init__.py` & `pyopencl-2024.2.1/pyopencl/__init__.py`

 * *Files identical despite different names*

### Comparing `pyopencl-2024.2/pyopencl/_cluda.py` & `pyopencl-2024.2.1/pyopencl/_cluda.py`

 * *Files identical despite different names*

### Comparing `pyopencl-2024.2/pyopencl/_mymako.py` & `pyopencl-2024.2.1/pyopencl/_mymako.py`

 * *Files identical despite different names*

### Comparing `pyopencl-2024.2/pyopencl/algorithm.py` & `pyopencl-2024.2.1/pyopencl/algorithm.py`

 * *Files identical despite different names*

### Comparing `pyopencl-2024.2/pyopencl/array.py` & `pyopencl-2024.2.1/pyopencl/array.py`

 * *Files identical despite different names*

### Comparing `pyopencl-2024.2/pyopencl/bitonic_sort.py` & `pyopencl-2024.2.1/pyopencl/bitonic_sort.py`

 * *Files identical despite different names*

### Comparing `pyopencl-2024.2/pyopencl/bitonic_sort_templates.py` & `pyopencl-2024.2.1/pyopencl/bitonic_sort_templates.py`

 * *Files identical despite different names*

### Comparing `pyopencl-2024.2/pyopencl/cache.py` & `pyopencl-2024.2.1/pyopencl/cache.py`

 * *Files identical despite different names*

### Comparing `pyopencl-2024.2/pyopencl/capture_call.py` & `pyopencl-2024.2.1/pyopencl/capture_call.py`

 * *Files identical despite different names*

### Comparing `pyopencl-2024.2/pyopencl/characterize/__init__.py` & `pyopencl-2024.2.1/pyopencl/characterize/__init__.py`

 * *Files identical despite different names*

### Comparing `pyopencl-2024.2/pyopencl/characterize/performance.py` & `pyopencl-2024.2.1/pyopencl/characterize/performance.py`

 * *Files identical despite different names*

### Comparing `pyopencl-2024.2/pyopencl/cl/pyopencl-airy.cl` & `pyopencl-2024.2.1/pyopencl/cl/pyopencl-airy.cl`

 * *Files identical despite different names*

### Comparing `pyopencl-2024.2/pyopencl/cl/pyopencl-bessel-j-complex.cl` & `pyopencl-2024.2.1/pyopencl/cl/pyopencl-bessel-j-complex.cl`

 * *Files identical despite different names*

### Comparing `pyopencl-2024.2/pyopencl/cl/pyopencl-bessel-j.cl` & `pyopencl-2024.2.1/pyopencl/cl/pyopencl-bessel-j.cl`

 * *Files identical despite different names*

### Comparing `pyopencl-2024.2/pyopencl/cl/pyopencl-bessel-y.cl` & `pyopencl-2024.2.1/pyopencl/cl/pyopencl-bessel-y.cl`

 * *Files identical despite different names*

### Comparing `pyopencl-2024.2/pyopencl/cl/pyopencl-complex.h` & `pyopencl-2024.2.1/pyopencl/cl/pyopencl-complex.h`

 * *Files identical despite different names*

### Comparing `pyopencl-2024.2/pyopencl/cl/pyopencl-eval-tbl.cl` & `pyopencl-2024.2.1/pyopencl/cl/pyopencl-eval-tbl.cl`

 * *Files identical despite different names*

### Comparing `pyopencl-2024.2/pyopencl/cl/pyopencl-hankel-complex.cl` & `pyopencl-2024.2.1/pyopencl/cl/pyopencl-hankel-complex.cl`

 * *Files identical despite different names*

### Comparing `pyopencl-2024.2/pyopencl/cl/pyopencl-random123/array.h` & `pyopencl-2024.2.1/pyopencl/cl/pyopencl-random123/array.h`

 * *Files identical despite different names*

### Comparing `pyopencl-2024.2/pyopencl/cl/pyopencl-random123/openclfeatures.h` & `pyopencl-2024.2.1/pyopencl/cl/pyopencl-random123/openclfeatures.h`

 * *Files identical despite different names*

### Comparing `pyopencl-2024.2/pyopencl/cl/pyopencl-random123/philox.cl` & `pyopencl-2024.2.1/pyopencl/cl/pyopencl-random123/philox.cl`

 * *Files identical despite different names*

### Comparing `pyopencl-2024.2/pyopencl/cl/pyopencl-random123/threefry.cl` & `pyopencl-2024.2.1/pyopencl/cl/pyopencl-random123/threefry.cl`

 * *Files identical despite different names*

### Comparing `pyopencl-2024.2/pyopencl/clmath.py` & `pyopencl-2024.2.1/pyopencl/clmath.py`

 * *Files identical despite different names*

### Comparing `pyopencl-2024.2/pyopencl/clrandom.py` & `pyopencl-2024.2.1/pyopencl/clrandom.py`

 * *Files identical despite different names*

### Comparing `pyopencl-2024.2/pyopencl/cltypes.py` & `pyopencl-2024.2.1/pyopencl/cltypes.py`

 * *Files identical despite different names*

### Comparing `pyopencl-2024.2/pyopencl/compyte/array.py` & `pyopencl-2024.2.1/pyopencl/compyte/array.py`

 * *Files identical despite different names*

### Comparing `pyopencl-2024.2/pyopencl/compyte/dtypes.py` & `pyopencl-2024.2.1/pyopencl/compyte/dtypes.py`

 * *Files identical despite different names*

### Comparing `pyopencl-2024.2/pyopencl/compyte/ndarray/gen_elemwise.py` & `pyopencl-2024.2.1/pyopencl/compyte/ndarray/gen_elemwise.py`

 * *Files identical despite different names*

### Comparing `pyopencl-2024.2/pyopencl/compyte/ndarray/gen_reduction.py` & `pyopencl-2024.2.1/pyopencl/compyte/ndarray/gen_reduction.py`

 * *Files identical despite different names*

### Comparing `pyopencl-2024.2/pyopencl/compyte/ndarray/setup_opencl.py` & `pyopencl-2024.2.1/pyopencl/compyte/ndarray/setup_opencl.py`

 * *Files identical despite different names*

### Comparing `pyopencl-2024.2/pyopencl/compyte/ndarray/test_gpu_elemwise.py` & `pyopencl-2024.2.1/pyopencl/compyte/ndarray/test_gpu_elemwise.py`

 * *Files identical despite different names*

### Comparing `pyopencl-2024.2/pyopencl/compyte/ndarray/test_gpu_ndarray.py` & `pyopencl-2024.2.1/pyopencl/compyte/ndarray/test_gpu_ndarray.py`

 * *Files identical despite different names*

### Comparing `pyopencl-2024.2/pyopencl/elementwise.py` & `pyopencl-2024.2.1/pyopencl/elementwise.py`

 * *Files identical despite different names*

### Comparing `pyopencl-2024.2/pyopencl/invoker.py` & `pyopencl-2024.2.1/pyopencl/invoker.py`

 * *Files identical despite different names*

### Comparing `pyopencl-2024.2/pyopencl/ipython_ext.py` & `pyopencl-2024.2.1/pyopencl/ipython_ext.py`

 * *Files identical despite different names*

### Comparing `pyopencl-2024.2/pyopencl/reduction.py` & `pyopencl-2024.2.1/pyopencl/reduction.py`

 * *Files identical despite different names*

### Comparing `pyopencl-2024.2/pyopencl/scan.py` & `pyopencl-2024.2.1/pyopencl/scan.py`

 * *Files identical despite different names*

### Comparing `pyopencl-2024.2/pyopencl/tools.py` & `pyopencl-2024.2.1/pyopencl/tools.py`

 * *Files identical despite different names*

### Comparing `pyopencl-2024.2/pyopencl.egg-info/PKG-INFO` & `pyopencl-2024.2.1/pyopencl.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyopencl
-Version: 2024.2
+Version: 2024.2.1
 Summary: Python wrapper for OpenCL
 Home-page: http://mathema.tician.de/software/pyopencl
 Author: Andreas Kloeckner
 Author-email: inform@tiker.net
 License: MIT
 Classifier: Environment :: Console
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `pyopencl-2024.2/pyopencl.egg-info/SOURCES.txt` & `pyopencl-2024.2.1/pyopencl.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 CITATION.cff
+CMakeLists.txt
 LICENSE
 MANIFEST.in
 Makefile.in
 README.rst
 README_SETUP.txt
 aksetup_helper.py
 configure.py
```

### Comparing `pyopencl-2024.2/pyproject.toml` & `pyopencl-2024.2.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pyopencl-2024.2/setup.cfg` & `pyopencl-2024.2.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `pyopencl-2024.2/setup.py` & `pyopencl-2024.2.1/setup.py`

 * *Files identical despite different names*

### Comparing `pyopencl-2024.2/src/bitlog.cpp` & `pyopencl-2024.2.1/src/bitlog.cpp`

 * *Files identical despite different names*

### Comparing `pyopencl-2024.2/src/bitlog.hpp` & `pyopencl-2024.2.1/src/bitlog.hpp`

 * *Files identical despite different names*

### Comparing `pyopencl-2024.2/src/clinfo_ext.h` & `pyopencl-2024.2.1/src/clinfo_ext.h`

 * *Files identical despite different names*

### Comparing `pyopencl-2024.2/src/mempool.hpp` & `pyopencl-2024.2.1/src/mempool.hpp`

 * *Files identical despite different names*

### Comparing `pyopencl-2024.2/src/pyopencl_ext.h` & `pyopencl-2024.2.1/src/pyopencl_ext.h`

 * *Files identical despite different names*

### Comparing `pyopencl-2024.2/src/tools.hpp` & `pyopencl-2024.2.1/src/tools.hpp`

 * *Files identical despite different names*

### Comparing `pyopencl-2024.2/src/wrap_cl.cpp` & `pyopencl-2024.2.1/src/wrap_cl.cpp`

 * *Files identical despite different names*

### Comparing `pyopencl-2024.2/src/wrap_cl.hpp` & `pyopencl-2024.2.1/src/wrap_cl.hpp`

 * *Files identical despite different names*

### Comparing `pyopencl-2024.2/src/wrap_cl_part_1.cpp` & `pyopencl-2024.2.1/src/wrap_cl_part_1.cpp`

 * *Files identical despite different names*

### Comparing `pyopencl-2024.2/src/wrap_cl_part_2.cpp` & `pyopencl-2024.2.1/src/wrap_cl_part_2.cpp`

 * *Files identical despite different names*

### Comparing `pyopencl-2024.2/src/wrap_constants.cpp` & `pyopencl-2024.2.1/src/wrap_constants.cpp`

 * *Files identical despite different names*

### Comparing `pyopencl-2024.2/src/wrap_helpers.hpp` & `pyopencl-2024.2.1/src/wrap_helpers.hpp`

 * *Files identical despite different names*

### Comparing `pyopencl-2024.2/src/wrap_mempool.cpp` & `pyopencl-2024.2.1/src/wrap_mempool.cpp`

 * *Files identical despite different names*

### Comparing `pyopencl-2024.2/test/add-vectors-32.spv` & `pyopencl-2024.2.1/test/add-vectors-32.spv`

 * *Files identical despite different names*

### Comparing `pyopencl-2024.2/test/add-vectors-64.spv` & `pyopencl-2024.2.1/test/add-vectors-64.spv`

 * *Files identical despite different names*

### Comparing `pyopencl-2024.2/test/test_algorithm.py` & `pyopencl-2024.2.1/test/test_algorithm.py`

 * *Files identical despite different names*

### Comparing `pyopencl-2024.2/test/test_array.py` & `pyopencl-2024.2.1/test/test_array.py`

 * *Files identical despite different names*

### Comparing `pyopencl-2024.2/test/test_arrays_in_structs.py` & `pyopencl-2024.2.1/test/test_arrays_in_structs.py`

 * *Files identical despite different names*

### Comparing `pyopencl-2024.2/test/test_clmath.py` & `pyopencl-2024.2.1/test/test_clmath.py`

 * *Files identical despite different names*

### Comparing `pyopencl-2024.2/test/test_clrandom.py` & `pyopencl-2024.2.1/test/test_clrandom.py`

 * *Files identical despite different names*

### Comparing `pyopencl-2024.2/test/test_enqueue_copy.py` & `pyopencl-2024.2.1/test/test_enqueue_copy.py`

 * *Files identical despite different names*

### Comparing `pyopencl-2024.2/test/test_wrapper.py` & `pyopencl-2024.2.1/test/test_wrapper.py`

 * *Files identical despite different names*

