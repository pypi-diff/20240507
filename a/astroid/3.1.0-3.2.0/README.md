# Comparing `tmp/astroid-3.1.0.tar.gz` & `tmp/astroid-3.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "astroid-3.1.0.tar", last modified: Fri Feb 23 16:28:02 2024, max compression
+gzip compressed data, was "astroid-3.2.0.tar", last modified: Tue May  7 11:58:15 2024, max compression
```

## Comparing `astroid-3.1.0.tar` & `astroid-3.2.0.tar`

### file list

```diff
@@ -1,344 +1,344 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 16:28:02.838840 astroid-3.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)     8315 2024-02-23 16:27:48.000000 astroid-3.1.0/CONTRIBUTORS.txt
--rw-r--r--   0 runner    (1001) docker     (127)    26516 2024-02-23 16:27:48.000000 astroid-3.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-02-23 16:27:48.000000 astroid-3.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4483 2024-02-23 16:28:02.838840 astroid-3.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2840 2024-02-23 16:27:48.000000 astroid-3.1.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 16:28:02.794840 astroid-3.1.0/astroid/
--rw-r--r--   0 runner    (1001) docker     (127)     4546 2024-02-23 16:27:48.000000 astroid-3.1.0/astroid/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      283 2024-02-23 16:27:48.000000 astroid-3.1.0/astroid/__pkginfo__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3033 2024-02-23 16:27:48.000000 astroid-3.1.0/astroid/_ast.py
--rw-r--r--   0 runner    (1001) docker     (127)     7026 2024-02-23 16:27:48.000000 astroid-3.1.0/astroid/_backport_stdlib_names.py
--rw-r--r--   0 runner    (1001) docker     (127)    12990 2024-02-23 16:27:48.000000 astroid-3.1.0/astroid/arguments.py
--rw-r--r--   0 runner    (1001) docker     (127)      729 2024-02-23 16:27:48.000000 astroid-3.1.0/astroid/astroid_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)    27145 2024-02-23 16:27:48.000000 astroid-3.1.0/astroid/bases.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 16:28:02.806840 astroid-3.1.0/astroid/brain/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-23 16:27:48.000000 astroid-3.1.0/astroid/brain/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1813 2024-02-23 16:27:48.000000 astroid-3.1.0/astroid/brain/brain_argparse.py
--rw-r--r--   0 runner    (1001) docker     (127)     3184 2024-02-23 16:27:48.000000 astroid-3.1.0/astroid/brain/brain_attrs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-02-23 16:27:48.000000 astroid-3.1.0/astroid/brain/brain_boto3.py
--rw-r--r--   0 runner    (1001) docker     (127)    37439 2024-02-23 16:27:48.000000 astroid-3.1.0/astroid/brain/brain_builtin_inference.py
--rw-r--r--   0 runner    (1001) docker     (127)     4490 2024-02-23 16:27:48.000000 astroid-3.1.0/astroid/brain/brain_collections.py
--rw-r--r--   0 runner    (1001) docker     (127)      915 2024-02-23 16:27:48.000000 astroid-3.1.0/astroid/brain/brain_crypt.py
--rw-r--r--   0 runner    (1001) docker     (127)     2720 2024-02-23 16:27:48.000000 astroid-3.1.0/astroid/brain/brain_ctypes.py
--rw-r--r--   0 runner    (1001) docker     (127)     3529 2024-02-23 16:27:48.000000 astroid-3.1.0/astroid/brain/brain_curses.py
--rw-r--r--   0 runner    (1001) docker     (127)    22206 2024-02-23 16:27:48.000000 astroid-3.1.0/astroid/brain/brain_dataclasses.py
--rw-r--r--   0 runner    (1001) docker     (127)      771 2024-02-23 16:27:48.000000 astroid-3.1.0/astroid/brain/brain_datetime.py
--rw-r--r--   0 runner    (1001) docker     (127)      819 2024-02-23 16:27:48.000000 astroid-3.1.0/astroid/brain/brain_dateutil.py
--rw-r--r--   0 runner    (1001) docker     (127)     2769 2024-02-23 16:27:48.000000 astroid-3.1.0/astroid/brain/brain_fstrings.py
--rw-r--r--   0 runner    (1001) docker     (127)     6390 2024-02-23 16:27:48.000000 astroid-3.1.0/astroid/brain/brain_functools.py
--rw-r--r--   0 runner    (1001) docker     (127)     7598 2024-02-23 16:27:48.000000 astroid-3.1.0/astroid/brain/brain_gi.py
--rw-r--r--   0 runner    (1001) docker     (127)     2873 2024-02-23 16:27:48.000000 astroid-3.1.0/astroid/brain/brain_hashlib.py
--rw-r--r--   0 runner    (1001) docker     (127)    10687 2024-02-23 16:27:48.000000 astroid-3.1.0/astroid/brain/brain_http.py
--rw-r--r--   0 runner    (1001) docker     (127)     1800 2024-02-23 16:27:48.000000 astroid-3.1.0/astroid/brain/brain_hypothesis.py
--rw-r--r--   0 runner    (1001) docker     (127)     1589 2024-02-23 16:27:48.000000 astroid-3.1.0/astroid/brain/brain_io.py
--rw-r--r--   0 runner    (1001) docker     (127)     2698 2024-02-23 16:27:48.000000 astroid-3.1.0/astroid/brain/brain_mechanize.py
--rw-r--r--   0 runner    (1001) docker     (127)     3260 2024-02-23 16:27:48.000000 astroid-3.1.0/astroid/brain/brain_multiprocessing.py
--rw-r--r--   0 runner    (1001) docker     (127)    23912 2024-02-23 16:27:48.000000 astroid-3.1.0/astroid/brain/brain_namedtuple_enum.py
--rw-r--r--   0 runner    (1001) docker     (127)     2402 2024-02-23 16:27:48.000000 astroid-3.1.0/astroid/brain/brain_nose.py
--rw-r--r--   0 runner    (1001) docker     (127)      885 2024-02-23 16:27:48.000000 astroid-3.1.0/astroid/brain/brain_numpy_core_einsumfunc.py
--rw-r--r--   0 runner    (1001) docker     (127)      792 2024-02-23 16:27:48.000000 astroid-3.1.0/astroid/brain/brain_numpy_core_fromnumeric.py
--rw-r--r--   0 runner    (1001) docker     (127)     1408 2024-02-23 16:27:48.000000 astroid-3.1.0/astroid/brain/brain_numpy_core_function_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     4400 2024-02-23 16:27:48.000000 astroid-3.1.0/astroid/brain/brain_numpy_core_multiarray.py
--rw-r--r--   0 runner    (1001) docker     (127)     1740 2024-02-23 16:27:48.000000 astroid-3.1.0/astroid/brain/brain_numpy_core_numeric.py
--rw-r--r--   0 runner    (1001) docker     (127)     8606 2024-02-23 16:27:48.000000 astroid-3.1.0/astroid/brain/brain_numpy_core_numerictypes.py
--rw-r--r--   0 runner    (1001) docker     (127)     4939 2024-02-23 16:27:48.000000 astroid-3.1.0/astroid/brain/brain_numpy_core_umath.py
--rw-r--r--   0 runner    (1001) docker     (127)      948 2024-02-23 16:27:48.000000 astroid-3.1.0/astroid/brain/brain_numpy_ma.py
--rw-r--r--   0 runner    (1001) docker     (127)     9066 2024-02-23 16:27:48.000000 astroid-3.1.0/astroid/brain/brain_numpy_ndarray.py
--rw-r--r--   0 runner    (1001) docker     (127)     3496 2024-02-23 16:27:48.000000 astroid-3.1.0/astroid/brain/brain_numpy_random_mtrand.py
--rw-r--r--   0 runner    (1001) docker     (127)     2553 2024-02-23 16:27:48.000000 astroid-3.1.0/astroid/brain/brain_numpy_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1610 2024-02-23 16:27:48.000000 astroid-3.1.0/astroid/brain/brain_pathlib.py
--rw-r--r--   0 runner    (1001) docker     (127)     2252 2024-02-23 16:27:48.000000 astroid-3.1.0/astroid/brain/brain_pkg_resources.py
--rw-r--r--   0 runner    (1001) docker     (127)     2270 2024-02-23 16:27:48.000000 astroid-3.1.0/astroid/brain/brain_pytest.py
--rw-r--r--   0 runner    (1001) docker     (127)     2874 2024-02-23 16:27:48.000000 astroid-3.1.0/astroid/brain/brain_qt.py
--rw-r--r--   0 runner    (1001) docker     (127)     3170 2024-02-23 16:27:48.000000 astroid-3.1.0/astroid/brain/brain_random.py
--rw-r--r--   0 runner    (1001) docker     (127)     3003 2024-02-23 16:27:48.000000 astroid-3.1.0/astroid/brain/brain_re.py
--rw-r--r--   0 runner    (1001) docker     (127)     3495 2024-02-23 16:27:48.000000 astroid-3.1.0/astroid/brain/brain_regex.py
--rw-r--r--   0 runner    (1001) docker     (127)     1920 2024-02-23 16:27:48.000000 astroid-3.1.0/astroid/brain/brain_responses.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2328 2024-02-23 16:27:48.000000 astroid-3.1.0/astroid/brain/brain_scipy_signal.py
--rw-r--r--   0 runner    (1001) docker     (127)     3932 2024-02-23 16:27:48.000000 astroid-3.1.0/astroid/brain/brain_signal.py
--rw-r--r--   0 runner    (1001) docker     (127)     7666 2024-02-23 16:27:48.000000 astroid-3.1.0/astroid/brain/brain_six.py
--rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-02-23 16:27:48.000000 astroid-3.1.0/astroid/brain/brain_sqlalchemy.py
--rw-r--r--   0 runner    (1001) docker     (127)     6554 2024-02-23 16:27:48.000000 astroid-3.1.0/astroid/brain/brain_ssl.py
--rw-r--r--   0 runner    (1001) docker     (127)     3048 2024-02-23 16:27:48.000000 astroid-3.1.0/astroid/brain/brain_subprocess.py
--rw-r--r--   0 runner    (1001) docker     (127)      922 2024-02-23 16:27:48.000000 astroid-3.1.0/astroid/brain/brain_threading.py
--rw-r--r--   0 runner    (1001) docker     (127)     2547 2024-02-23 16:27:48.000000 astroid-3.1.0/astroid/brain/brain_type.py
--rw-r--r--   0 runner    (1001) docker     (127)    16303 2024-02-23 16:27:48.000000 astroid-3.1.0/astroid/brain/brain_typing.py
--rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-02-23 16:27:48.000000 astroid-3.1.0/astroid/brain/brain_unittest.py
--rw-r--r--   0 runner    (1001) docker     (127)      727 2024-02-23 16:27:48.000000 astroid-3.1.0/astroid/brain/brain_uuid.py
--rw-r--r--   0 runner    (1001) docker     (127)     4364 2024-02-23 16:27:48.000000 astroid-3.1.0/astroid/brain/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)    18727 2024-02-23 16:27:48.000000 astroid-3.1.0/astroid/builder.py
--rw-r--r--   0 runner    (1001) docker     (127)      862 2024-02-23 16:27:48.000000 astroid-3.1.0/astroid/const.py
--rw-r--r--   0 runner    (1001) docker     (127)     5086 2024-02-23 16:27:48.000000 astroid-3.1.0/astroid/constraint.py
--rw-r--r--   0 runner    (1001) docker     (127)     6324 2024-02-23 16:27:48.000000 astroid-3.1.0/astroid/context.py
--rw-r--r--   0 runner    (1001) docker     (127)     8590 2024-02-23 16:27:48.000000 astroid-3.1.0/astroid/decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)    12786 2024-02-23 16:27:48.000000 astroid-3.1.0/astroid/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     9387 2024-02-23 16:27:48.000000 astroid-3.1.0/astroid/filter_statements.py
--rw-r--r--   0 runner    (1001) docker     (127)    11918 2024-02-23 16:27:48.000000 astroid-3.1.0/astroid/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     4598 2024-02-23 16:27:48.000000 astroid-3.1.0/astroid/inference_tip.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 16:28:02.806840 astroid-3.1.0/astroid/interpreter/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-23 16:27:48.000000 astroid-3.1.0/astroid/interpreter/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 16:28:02.806840 astroid-3.1.0/astroid/interpreter/_import/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-23 16:27:48.000000 astroid-3.1.0/astroid/interpreter/_import/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16568 2024-02-23 16:27:48.000000 astroid-3.1.0/astroid/interpreter/_import/spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     4417 2024-02-23 16:27:48.000000 astroid-3.1.0/astroid/interpreter/_import/util.py
--rw-r--r--   0 runner    (1001) docker     (127)     2515 2024-02-23 16:27:48.000000 astroid-3.1.0/astroid/interpreter/dunder_lookup.py
--rw-r--r--   0 runner    (1001) docker     (127)    34593 2024-02-23 16:27:48.000000 astroid-3.1.0/astroid/interpreter/objectmodel.py
--rw-r--r--   0 runner    (1001) docker     (127)    18066 2024-02-23 16:27:48.000000 astroid-3.1.0/astroid/manager.py
--rw-r--r--   0 runner    (1001) docker     (127)    23616 2024-02-23 16:27:48.000000 astroid-3.1.0/astroid/modutils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 16:28:02.806840 astroid-3.1.0/astroid/nodes/
--rw-r--r--   0 runner    (1001) docker     (127)     4744 2024-02-23 16:27:48.000000 astroid-3.1.0/astroid/nodes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    24111 2024-02-23 16:27:48.000000 astroid-3.1.0/astroid/nodes/_base_nodes.py
--rw-r--r--   0 runner    (1001) docker     (127)    26317 2024-02-23 16:27:48.000000 astroid-3.1.0/astroid/nodes/as_string.py
--rw-r--r--   0 runner    (1001) docker     (127)      807 2024-02-23 16:27:48.000000 astroid-3.1.0/astroid/nodes/const.py
--rw-r--r--   0 runner    (1001) docker     (127)   168997 2024-02-23 16:27:48.000000 astroid-3.1.0/astroid/nodes/node_classes.py
--rw-r--r--   0 runner    (1001) docker     (127)    27045 2024-02-23 16:27:48.000000 astroid-3.1.0/astroid/nodes/node_ng.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 16:28:02.810840 astroid-3.1.0/astroid/nodes/scoped_nodes/
--rw-r--r--   0 runner    (1001) docker     (127)     1229 2024-02-23 16:27:48.000000 astroid-3.1.0/astroid/nodes/scoped_nodes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7151 2024-02-23 16:27:48.000000 astroid-3.1.0/astroid/nodes/scoped_nodes/mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)   104466 2024-02-23 16:27:48.000000 astroid-3.1.0/astroid/nodes/scoped_nodes/scoped_nodes.py
--rw-r--r--   0 runner    (1001) docker     (127)     1181 2024-02-23 16:27:48.000000 astroid-3.1.0/astroid/nodes/scoped_nodes/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      433 2024-02-23 16:27:48.000000 astroid-3.1.0/astroid/nodes/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    13025 2024-02-23 16:27:48.000000 astroid-3.1.0/astroid/objects.py
--rw-r--r--   0 runner    (1001) docker     (127)    31691 2024-02-23 16:27:48.000000 astroid-3.1.0/astroid/protocols.py
--rw-r--r--   0 runner    (1001) docker     (127)    25314 2024-02-23 16:27:48.000000 astroid-3.1.0/astroid/raw_building.py
--rw-r--r--   0 runner    (1001) docker     (127)    71309 2024-02-23 16:27:48.000000 astroid-3.1.0/astroid/rebuilder.py
--rw-r--r--   0 runner    (1001) docker     (127)     2444 2024-02-23 16:27:48.000000 astroid-3.1.0/astroid/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     5849 2024-02-23 16:27:48.000000 astroid-3.1.0/astroid/transforms.py
--rw-r--r--   0 runner    (1001) docker     (127)     2748 2024-02-23 16:27:48.000000 astroid-3.1.0/astroid/typing.py
--rw-r--r--   0 runner    (1001) docker     (127)     4846 2024-02-23 16:27:48.000000 astroid-3.1.0/astroid/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 16:28:02.838840 astroid-3.1.0/astroid.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4483 2024-02-23 16:28:02.000000 astroid-3.1.0/astroid.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11043 2024-02-23 16:28:02.000000 astroid-3.1.0/astroid.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-23 16:28:02.000000 astroid-3.1.0/astroid.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-02-23 16:28:02.000000 astroid-3.1.0/astroid.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-02-23 16:28:02.000000 astroid-3.1.0/astroid.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3293 2024-02-23 16:27:48.000000 astroid-3.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-02-23 16:27:48.000000 astroid-3.1.0/requirements_dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)      211 2024-02-23 16:27:48.000000 astroid-3.1.0/requirements_full.txt
--rw-r--r--   0 runner    (1001) docker     (127)      128 2024-02-23 16:27:48.000000 astroid-3.1.0/requirements_minimal.txt
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-02-23 16:28:02.838840 astroid-3.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 16:28:02.814840 astroid-3.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-23 16:27:48.000000 astroid-3.1.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 16:28:02.818840 astroid-3.1.0/tests/brain/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-23 16:27:48.000000 astroid-3.1.0/tests/brain/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 16:28:02.822840 astroid-3.1.0/tests/brain/numpy/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-23 16:27:48.000000 astroid-3.1.0/tests/brain/numpy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1708 2024-02-23 16:27:48.000000 astroid-3.1.0/tests/brain/numpy/test_core_einsumfunc.py
--rw-r--r--   0 runner    (1001) docker     (127)     1629 2024-02-23 16:27:48.000000 astroid-3.1.0/tests/brain/numpy/test_core_fromnumeric.py
--rw-r--r--   0 runner    (1001) docker     (127)     1766 2024-02-23 16:27:48.000000 astroid-3.1.0/tests/brain/numpy/test_core_function_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     7681 2024-02-23 16:27:48.000000 astroid-3.1.0/tests/brain/numpy/test_core_multiarray.py
--rw-r--r--   0 runner    (1001) docker     (127)     2556 2024-02-23 16:27:48.000000 astroid-3.1.0/tests/brain/numpy/test_core_numeric.py
--rw-r--r--   0 runner    (1001) docker     (127)    11199 2024-02-23 16:27:48.000000 astroid-3.1.0/tests/brain/numpy/test_core_numerictypes.py
--rw-r--r--   0 runner    (1001) docker     (127)     7744 2024-02-23 16:27:48.000000 astroid-3.1.0/tests/brain/numpy/test_core_umath.py
--rw-r--r--   0 runner    (1001) docker     (127)     1494 2024-02-23 16:27:48.000000 astroid-3.1.0/tests/brain/numpy/test_ma.py
--rw-r--r--   0 runner    (1001) docker     (127)     4897 2024-02-23 16:27:48.000000 astroid-3.1.0/tests/brain/numpy/test_ndarray.py
--rw-r--r--   0 runner    (1001) docker     (127)     4525 2024-02-23 16:27:48.000000 astroid-3.1.0/tests/brain/numpy/test_random_mtrand.py
--rw-r--r--   0 runner    (1001) docker     (127)      734 2024-02-23 16:27:48.000000 astroid-3.1.0/tests/brain/test_argparse.py
--rw-r--r--   0 runner    (1001) docker     (127)     5502 2024-02-23 16:27:48.000000 astroid-3.1.0/tests/brain/test_attr.py
--rw-r--r--   0 runner    (1001) docker     (127)    63783 2024-02-23 16:27:48.000000 astroid-3.1.0/tests/brain/test_brain.py
--rw-r--r--   0 runner    (1001) docker     (127)     5073 2024-02-23 16:27:48.000000 astroid-3.1.0/tests/brain/test_builtin.py
--rw-r--r--   0 runner    (1001) docker     (127)     3489 2024-02-23 16:27:48.000000 astroid-3.1.0/tests/brain/test_ctypes.py
--rw-r--r--   0 runner    (1001) docker     (127)    35395 2024-02-23 16:27:48.000000 astroid-3.1.0/tests/brain/test_dataclasses.py
--rw-r--r--   0 runner    (1001) docker     (127)      897 2024-02-23 16:27:48.000000 astroid-3.1.0/tests/brain/test_dateutil.py
--rw-r--r--   0 runner    (1001) docker     (127)    18541 2024-02-23 16:27:48.000000 astroid-3.1.0/tests/brain/test_enum.py
--rw-r--r--   0 runner    (1001) docker     (127)     2707 2024-02-23 16:27:48.000000 astroid-3.1.0/tests/brain/test_hashlib.py
--rw-r--r--   0 runner    (1001) docker     (127)     4035 2024-02-23 16:27:48.000000 astroid-3.1.0/tests/brain/test_multiprocessing.py
--rw-r--r--   0 runner    (1001) docker     (127)    10754 2024-02-23 16:27:48.000000 astroid-3.1.0/tests/brain/test_named_tuple.py
--rw-r--r--   0 runner    (1001) docker     (127)     1687 2024-02-23 16:27:48.000000 astroid-3.1.0/tests/brain/test_nose.py
--rw-r--r--   0 runner    (1001) docker     (127)     2206 2024-02-23 16:27:48.000000 astroid-3.1.0/tests/brain/test_pathlib.py
--rw-r--r--   0 runner    (1001) docker     (127)      795 2024-02-23 16:27:48.000000 astroid-3.1.0/tests/brain/test_pytest.py
--rw-r--r--   0 runner    (1001) docker     (127)     3008 2024-02-23 16:27:48.000000 astroid-3.1.0/tests/brain/test_qt.py
--rw-r--r--   0 runner    (1001) docker     (127)     1788 2024-02-23 16:27:48.000000 astroid-3.1.0/tests/brain/test_regex.py
--rw-r--r--   0 runner    (1001) docker     (127)     1324 2024-02-23 16:27:48.000000 astroid-3.1.0/tests/brain/test_signal.py
--rw-r--r--   0 runner    (1001) docker     (127)     5480 2024-02-23 16:27:48.000000 astroid-3.1.0/tests/brain/test_six.py
--rw-r--r--   0 runner    (1001) docker     (127)     1626 2024-02-23 16:27:48.000000 astroid-3.1.0/tests/brain/test_ssl.py
--rw-r--r--   0 runner    (1001) docker     (127)     1796 2024-02-23 16:27:48.000000 astroid-3.1.0/tests/brain/test_threading.py
--rw-r--r--   0 runner    (1001) docker     (127)      730 2024-02-23 16:27:48.000000 astroid-3.1.0/tests/brain/test_typing.py
--rw-r--r--   0 runner    (1001) docker     (127)     1265 2024-02-23 16:27:48.000000 astroid-3.1.0/tests/brain/test_typing_extensions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1047 2024-02-23 16:27:48.000000 astroid-3.1.0/tests/brain/test_unittest.py
--rw-r--r--   0 runner    (1001) docker     (127)     2051 2024-02-23 16:27:48.000000 astroid-3.1.0/tests/resources.py
--rw-r--r--   0 runner    (1001) docker     (127)    35331 2024-02-23 16:27:48.000000 astroid-3.1.0/tests/test_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)    15433 2024-02-23 16:27:48.000000 astroid-3.1.0/tests/test_constraint.py
--rw-r--r--   0 runner    (1001) docker     (127)     3793 2024-02-23 16:27:48.000000 astroid-3.1.0/tests/test_decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)      642 2024-02-23 16:27:48.000000 astroid-3.1.0/tests/test_filter_statements.py
--rw-r--r--   0 runner    (1001) docker     (127)     3530 2024-02-23 16:27:48.000000 astroid-3.1.0/tests/test_group_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     9634 2024-02-23 16:27:48.000000 astroid-3.1.0/tests/test_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)   225024 2024-02-23 16:27:48.000000 astroid-3.1.0/tests/test_inference.py
--rw-r--r--   0 runner    (1001) docker     (127)    14712 2024-02-23 16:27:48.000000 astroid-3.1.0/tests/test_inference_calls.py
--rw-r--r--   0 runner    (1001) docker     (127)    34856 2024-02-23 16:27:48.000000 astroid-3.1.0/tests/test_lookup.py
--rw-r--r--   0 runner    (1001) docker     (127)    20070 2024-02-23 16:27:48.000000 astroid-3.1.0/tests/test_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)    22658 2024-02-23 16:27:48.000000 astroid-3.1.0/tests/test_modutils.py
--rw-r--r--   0 runner    (1001) docker     (127)    66136 2024-02-23 16:27:48.000000 astroid-3.1.0/tests/test_nodes.py
--rw-r--r--   0 runner    (1001) docker     (127)    55445 2024-02-23 16:27:48.000000 astroid-3.1.0/tests/test_nodes_lineno.py
--rw-r--r--   0 runner    (1001) docker     (127)     4167 2024-02-23 16:27:48.000000 astroid-3.1.0/tests/test_nodes_position.py
--rw-r--r--   0 runner    (1001) docker     (127)    27854 2024-02-23 16:27:48.000000 astroid-3.1.0/tests/test_object_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    21338 2024-02-23 16:27:48.000000 astroid-3.1.0/tests/test_objects.py
--rw-r--r--   0 runner    (1001) docker     (127)    16017 2024-02-23 16:27:48.000000 astroid-3.1.0/tests/test_protocols.py
--rw-r--r--   0 runner    (1001) docker     (127)    14453 2024-02-23 16:27:48.000000 astroid-3.1.0/tests/test_python3.py
--rw-r--r--   0 runner    (1001) docker     (127)     5910 2024-02-23 16:27:48.000000 astroid-3.1.0/tests/test_raw_building.py
--rw-r--r--   0 runner    (1001) docker     (127)    15094 2024-02-23 16:27:48.000000 astroid-3.1.0/tests/test_regrtest.py
--rw-r--r--   0 runner    (1001) docker     (127)    93585 2024-02-23 16:27:48.000000 astroid-3.1.0/tests/test_scoped_nodes.py
--rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-02-23 16:27:48.000000 astroid-3.1.0/tests/test_stdlib.py
--rw-r--r--   0 runner    (1001) docker     (127)     9826 2024-02-23 16:27:48.000000 astroid-3.1.0/tests/test_transforms.py
--rw-r--r--   0 runner    (1001) docker     (127)     2711 2024-02-23 16:27:48.000000 astroid-3.1.0/tests/test_type_params.py
--rw-r--r--   0 runner    (1001) docker     (127)     6459 2024-02-23 16:27:48.000000 astroid-3.1.0/tests/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 16:28:02.782840 astroid-3.1.0/tests/testdata/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 16:28:02.822840 astroid-3.1.0/tests/testdata/python3/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 16:28:02.822840 astroid-3.1.0/tests/testdata/python3/data/
--rw-r--r--   0 runner    (1001) docker     (127)     1222 2024-02-23 16:27:48.000000 astroid-3.1.0/tests/testdata/python3/data/MyPyPa-0.1.0-py2.5.egg
--rw-r--r--   0 runner    (1001) docker     (127)     1222 2024-02-23 16:27:48.000000 astroid-3.1.0/tests/testdata/python3/data/MyPyPa-0.1.0-py2.5.zip
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 16:28:02.826840 astroid-3.1.0/tests/testdata/python3/data/SSL1/
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-02-23 16:27:48.000000 astroid-3.1.0/tests/testdata/python3/data/SSL1/Connection1.py
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-02-23 16:27:48.000000 astroid-3.1.0/tests/testdata/python3/data/SSL1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-02-23 16:27:48.000000 astroid-3.1.0/tests/testdata/python3/data/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 16:28:02.826840 astroid-3.1.0/tests/testdata/python3/data/absimp/
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-02-23 16:27:48.000000 astroid-3.1.0/tests/testdata/python3/data/absimp/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 16:28:02.826840 astroid-3.1.0/tests/testdata/python3/data/absimp/sidepackage/
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-02-23 16:27:48.000000 astroid-3.1.0/tests/testdata/python3/data/absimp/sidepackage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-02-23 16:27:48.000000 astroid-3.1.0/tests/testdata/python3/data/absimp/string.py
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-02-23 16:27:48.000000 astroid-3.1.0/tests/testdata/python3/data/absimport.py
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-02-23 16:27:48.000000 astroid-3.1.0/tests/testdata/python3/data/all.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 16:28:02.826840 astroid-3.1.0/tests/testdata/python3/data/appl/
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-02-23 16:27:48.000000 astroid-3.1.0/tests/testdata/python3/data/appl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      261 2024-02-23 16:27:48.000000 astroid-3.1.0/tests/testdata/python3/data/appl/myConnection.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 16:28:02.826840 astroid-3.1.0/tests/testdata/python3/data/beyond_top_level/
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-02-23 16:27:48.000000 astroid-3.1.0/tests/testdata/python3/data/beyond_top_level/import_package.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 16:28:02.826840 astroid-3.1.0/tests/testdata/python3/data/beyond_top_level/namespace_package/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 16:28:02.826840 astroid-3.1.0/tests/testdata/python3/data/beyond_top_level/namespace_package/lower_level/
--rw-r--r--   0 runner    (1001) docker     (127)      114 2024-02-23 16:27:48.000000 astroid-3.1.0/tests/testdata/python3/data/beyond_top_level/namespace_package/lower_level/helper_function.py
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-02-23 16:27:48.000000 astroid-3.1.0/tests/testdata/python3/data/beyond_top_level/namespace_package/plugin_api.py
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-02-23 16:27:48.000000 astroid-3.1.0/tests/testdata/python3/data/beyond_top_level/namespace_package/top_level_function.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 16:28:02.782840 astroid-3.1.0/tests/testdata/python3/data/beyond_top_level_three/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 16:28:02.826840 astroid-3.1.0/tests/testdata/python3/data/beyond_top_level_three/double_name/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-23 16:27:48.000000 astroid-3.1.0/tests/testdata/python3/data/beyond_top_level_three/double_name/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 16:28:02.826840 astroid-3.1.0/tests/testdata/python3/data/beyond_top_level_three/module/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-23 16:27:48.000000 astroid-3.1.0/tests/testdata/python3/data/beyond_top_level_three/module/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 16:28:02.826840 astroid-3.1.0/tests/testdata/python3/data/beyond_top_level_three/module/double_name/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-23 16:27:48.000000 astroid-3.1.0/tests/testdata/python3/data/beyond_top_level_three/module/double_name/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-23 16:27:48.000000 astroid-3.1.0/tests/testdata/python3/data/beyond_top_level_three/module/double_name/function.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 16:28:02.826840 astroid-3.1.0/tests/testdata/python3/data/beyond_top_level_three/module/sub_module/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-23 16:27:48.000000 astroid-3.1.0/tests/testdata/python3/data/beyond_top_level_three/module/sub_module/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 16:28:02.826840 astroid-3.1.0/tests/testdata/python3/data/beyond_top_level_three/module/sub_module/sub_sub_module/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-23 16:27:48.000000 astroid-3.1.0/tests/testdata/python3/data/beyond_top_level_three/module/sub_module/sub_sub_module/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-02-23 16:27:48.000000 astroid-3.1.0/tests/testdata/python3/data/beyond_top_level_three/module/sub_module/sub_sub_module/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 16:28:02.826840 astroid-3.1.0/tests/testdata/python3/data/beyond_top_level_two/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-23 16:27:48.000000 astroid-3.1.0/tests/testdata/python3/data/beyond_top_level_two/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      163 2024-02-23 16:27:48.000000 astroid-3.1.0/tests/testdata/python3/data/beyond_top_level_two/a.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 16:28:02.826840 astroid-3.1.0/tests/testdata/python3/data/beyond_top_level_two/level1/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-02-23 16:27:48.000000 astroid-3.1.0/tests/testdata/python3/data/beyond_top_level_two/level1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-02-23 16:27:48.000000 astroid-3.1.0/tests/testdata/python3/data/beyond_top_level_two/level1/beyond_top_level_two.py
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-02-23 16:27:48.000000 astroid-3.1.0/tests/testdata/python3/data/conditional.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 16:28:02.826840 astroid-3.1.0/tests/testdata/python3/data/conditional_import/
--rw-r--r--   0 runner    (1001) docker     (127)      172 2024-02-23 16:27:48.000000 astroid-3.1.0/tests/testdata/python3/data/conditional_import/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 16:28:02.786840 astroid-3.1.0/tests/testdata/python3/data/contribute_to_namespace/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 16:28:02.826840 astroid-3.1.0/tests/testdata/python3/data/contribute_to_namespace/namespace_pep_420/
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-02-23 16:27:48.000000 astroid-3.1.0/tests/testdata/python3/data/contribute_to_namespace/namespace_pep_420/submodule.py
--rw-r--r--   0 runner    (1001) docker     (127)      217 2024-02-23 16:27:48.000000 astroid-3.1.0/tests/testdata/python3/data/descriptor_crash.py
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-02-23 16:27:48.000000 astroid-3.1.0/tests/testdata/python3/data/email.py
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-02-23 16:27:48.000000 astroid-3.1.0/tests/testdata/python3/data/fake_module_with_broken_getattr.py
--rw-r--r--   0 runner    (1001) docker     (127)      661 2024-02-23 16:27:48.000000 astroid-3.1.0/tests/testdata/python3/data/fake_module_with_warnings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 16:28:02.830840 astroid-3.1.0/tests/testdata/python3/data/find_test/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-23 16:27:48.000000 astroid-3.1.0/tests/testdata/python3/data/find_test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-23 16:27:48.000000 astroid-3.1.0/tests/testdata/python3/data/find_test/module.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-23 16:27:48.000000 astroid-3.1.0/tests/testdata/python3/data/find_test/module2.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-23 16:27:48.000000 astroid-3.1.0/tests/testdata/python3/data/find_test/noendingnewline.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-23 16:27:48.000000 astroid-3.1.0/tests/testdata/python3/data/find_test/nonregr.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 16:28:02.786840 astroid-3.1.0/tests/testdata/python3/data/foogle/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 16:28:02.830840 astroid-3.1.0/tests/testdata/python3/data/foogle/fax/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-23 16:27:48.000000 astroid-3.1.0/tests/testdata/python3/data/foogle/fax/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-02-23 16:27:48.000000 astroid-3.1.0/tests/testdata/python3/data/foogle/fax/a.py
--rw-r--r--   0 runner    (1001) docker     (127)      629 2024-02-23 16:27:48.000000 astroid-3.1.0/tests/testdata/python3/data/foogle_fax-0.12.5-py2.7-nspkg.pth
--rw-r--r--   0 runner    (1001) docker     (127)      421 2024-02-23 16:27:48.000000 astroid-3.1.0/tests/testdata/python3/data/format.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 16:28:02.830840 astroid-3.1.0/tests/testdata/python3/data/import_conflicting_names/
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-02-23 16:27:48.000000 astroid-3.1.0/tests/testdata/python3/data/import_conflicting_names/math.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 16:28:02.830840 astroid-3.1.0/tests/testdata/python3/data/import_setuptools_pep660/
--rw-r--r--   0 runner    (1001) docker     (127)     2709 2024-02-23 16:27:48.000000 astroid-3.1.0/tests/testdata/python3/data/import_setuptools_pep660/__editable___example_0_1_0_finder.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 16:28:02.830840 astroid-3.1.0/tests/testdata/python3/data/import_setuptools_pep660/example/
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-02-23 16:27:48.000000 astroid-3.1.0/tests/testdata/python3/data/import_setuptools_pep660/example/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 16:28:02.830840 astroid-3.1.0/tests/testdata/python3/data/import_setuptools_pep660/example/subpackage/
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-02-23 16:27:48.000000 astroid-3.1.0/tests/testdata/python3/data/import_setuptools_pep660/example/subpackage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-02-23 16:27:48.000000 astroid-3.1.0/tests/testdata/python3/data/invalid_encoding.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 16:28:02.830840 astroid-3.1.0/tests/testdata/python3/data/lmfp/
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-02-23 16:27:48.000000 astroid-3.1.0/tests/testdata/python3/data/lmfp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      170 2024-02-23 16:27:48.000000 astroid-3.1.0/tests/testdata/python3/data/lmfp/foo.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 16:28:02.830840 astroid-3.1.0/tests/testdata/python3/data/max_inferable_limit_for_classes/
--rw-r--r--   0 runner    (1001) docker     (127)      667 2024-02-23 16:27:48.000000 astroid-3.1.0/tests/testdata/python3/data/max_inferable_limit_for_classes/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 16:28:02.830840 astroid-3.1.0/tests/testdata/python3/data/max_inferable_limit_for_classes/nodes/
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-02-23 16:27:48.000000 astroid-3.1.0/tests/testdata/python3/data/max_inferable_limit_for_classes/nodes/roles.py
--rw-r--r--   0 runner    (1001) docker     (127)      459 2024-02-23 16:27:48.000000 astroid-3.1.0/tests/testdata/python3/data/max_inferable_limit_for_classes/other_funcs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 16:28:02.830840 astroid-3.1.0/tests/testdata/python3/data/metaclass_recursion/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-23 16:27:48.000000 astroid-3.1.0/tests/testdata/python3/data/metaclass_recursion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      614 2024-02-23 16:27:48.000000 astroid-3.1.0/tests/testdata/python3/data/metaclass_recursion/monkeypatch.py
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-02-23 16:27:48.000000 astroid-3.1.0/tests/testdata/python3/data/metaclass_recursion/parent.py
--rw-r--r--   0 runner    (1001) docker     (127)     1784 2024-02-23 16:27:48.000000 astroid-3.1.0/tests/testdata/python3/data/module.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 16:28:02.830840 astroid-3.1.0/tests/testdata/python3/data/module1abs/
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-02-23 16:27:48.000000 astroid-3.1.0/tests/testdata/python3/data/module1abs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-02-23 16:27:48.000000 astroid-3.1.0/tests/testdata/python3/data/module1abs/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     1949 2024-02-23 16:27:48.000000 astroid-3.1.0/tests/testdata/python3/data/module2.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 16:28:02.830840 astroid-3.1.0/tests/testdata/python3/data/module_dict_items_call/
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-02-23 16:27:48.000000 astroid-3.1.0/tests/testdata/python3/data/module_dict_items_call/models.py
--rw-r--r--   0 runner    (1001) docker     (127)      148 2024-02-23 16:27:48.000000 astroid-3.1.0/tests/testdata/python3/data/module_dict_items_call/test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 16:28:02.830840 astroid-3.1.0/tests/testdata/python3/data/namespace_pep_420/
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-02-23 16:27:48.000000 astroid-3.1.0/tests/testdata/python3/data/namespace_pep_420/module.py
--rw-r--r--   0 runner    (1001) docker     (127)      506 2024-02-23 16:27:48.000000 astroid-3.1.0/tests/testdata/python3/data/noendingnewline.py
--rw-r--r--   0 runner    (1001) docker     (127)     1010 2024-02-23 16:27:48.000000 astroid-3.1.0/tests/testdata/python3/data/nonregr.py
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-02-23 16:27:48.000000 astroid-3.1.0/tests/testdata/python3/data/notall.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 16:28:02.830840 astroid-3.1.0/tests/testdata/python3/data/notamodule/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-23 16:27:48.000000 astroid-3.1.0/tests/testdata/python3/data/notamodule/file.py
--rw-r--r--   0 runner    (1001) docker     (127)      823 2024-02-23 16:27:48.000000 astroid-3.1.0/tests/testdata/python3/data/operator_precedence.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 16:28:02.834840 astroid-3.1.0/tests/testdata/python3/data/package/
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-02-23 16:27:48.000000 astroid-3.1.0/tests/testdata/python3/data/package/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      172 2024-02-23 16:27:48.000000 astroid-3.1.0/tests/testdata/python3/data/package/absimport.py
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-02-23 16:27:48.000000 astroid-3.1.0/tests/testdata/python3/data/package/hello.py
--rw-r--r--   0 runner    (1001) docker     (127)     2242 2024-02-23 16:27:48.000000 astroid-3.1.0/tests/testdata/python3/data/package/import_package_subpackage_module.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 16:28:02.834840 astroid-3.1.0/tests/testdata/python3/data/package/subpackage/
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-02-23 16:27:48.000000 astroid-3.1.0/tests/testdata/python3/data/package/subpackage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-02-23 16:27:48.000000 astroid-3.1.0/tests/testdata/python3/data/package/subpackage/module.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 16:28:02.834840 astroid-3.1.0/tests/testdata/python3/data/parent_of_homonym/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-23 16:27:48.000000 astroid-3.1.0/tests/testdata/python3/data/parent_of_homonym/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 16:28:02.834840 astroid-3.1.0/tests/testdata/python3/data/parent_of_homonym/doc/
--rw-r--r--   0 runner    (1001) docker     (127)      160 2024-02-23 16:27:48.000000 astroid-3.1.0/tests/testdata/python3/data/parent_of_homonym/doc/README.md
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-23 16:27:48.000000 astroid-3.1.0/tests/testdata/python3/data/parent_of_homonym/doc/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 16:28:02.786840 astroid-3.1.0/tests/testdata/python3/data/path_pkg_resources_1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 16:28:02.834840 astroid-3.1.0/tests/testdata/python3/data/path_pkg_resources_1/package/
--rw-r--r--   0 runner    (1001) docker     (127)      165 2024-02-23 16:27:48.000000 astroid-3.1.0/tests/testdata/python3/data/path_pkg_resources_1/package/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-23 16:27:48.000000 astroid-3.1.0/tests/testdata/python3/data/path_pkg_resources_1/package/foo.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 16:28:02.786840 astroid-3.1.0/tests/testdata/python3/data/path_pkg_resources_2/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 16:28:02.834840 astroid-3.1.0/tests/testdata/python3/data/path_pkg_resources_2/package/
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-02-23 16:27:48.000000 astroid-3.1.0/tests/testdata/python3/data/path_pkg_resources_2/package/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-23 16:27:48.000000 astroid-3.1.0/tests/testdata/python3/data/path_pkg_resources_2/package/bar.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 16:28:02.786840 astroid-3.1.0/tests/testdata/python3/data/path_pkg_resources_3/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 16:28:02.834840 astroid-3.1.0/tests/testdata/python3/data/path_pkg_resources_3/package/
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-02-23 16:27:48.000000 astroid-3.1.0/tests/testdata/python3/data/path_pkg_resources_3/package/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-23 16:27:48.000000 astroid-3.1.0/tests/testdata/python3/data/path_pkg_resources_3/package/baz.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 16:28:02.786840 astroid-3.1.0/tests/testdata/python3/data/path_pkgutil_1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 16:28:02.834840 astroid-3.1.0/tests/testdata/python3/data/path_pkgutil_1/package/
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-02-23 16:27:48.000000 astroid-3.1.0/tests/testdata/python3/data/path_pkgutil_1/package/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-23 16:27:48.000000 astroid-3.1.0/tests/testdata/python3/data/path_pkgutil_1/package/foo.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 16:28:02.786840 astroid-3.1.0/tests/testdata/python3/data/path_pkgutil_2/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 16:28:02.834840 astroid-3.1.0/tests/testdata/python3/data/path_pkgutil_2/package/
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-02-23 16:27:48.000000 astroid-3.1.0/tests/testdata/python3/data/path_pkgutil_2/package/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-23 16:27:48.000000 astroid-3.1.0/tests/testdata/python3/data/path_pkgutil_2/package/bar.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 16:28:02.786840 astroid-3.1.0/tests/testdata/python3/data/path_pkgutil_3/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 16:28:02.834840 astroid-3.1.0/tests/testdata/python3/data/path_pkgutil_3/package/
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-02-23 16:27:48.000000 astroid-3.1.0/tests/testdata/python3/data/path_pkgutil_3/package/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-23 16:27:48.000000 astroid-3.1.0/tests/testdata/python3/data/path_pkgutil_3/package/baz.py
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-02-23 16:27:48.000000 astroid-3.1.0/tests/testdata/python3/data/recursion.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-23 16:27:48.000000 astroid-3.1.0/tests/testdata/python3/data/tmp__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 16:28:02.834840 astroid-3.1.0/tests/testdata/python3/data/unicode_package/
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-02-23 16:27:48.000000 astroid-3.1.0/tests/testdata/python3/data/unicode_package/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 16:28:02.834840 astroid-3.1.0/tests/testdata/python3/data/unicode_package/core/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-23 16:27:48.000000 astroid-3.1.0/tests/testdata/python3/data/unicode_package/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 16:28:02.834840 astroid-3.1.0/tests/testdata/python3/pyi_data/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-23 16:27:48.000000 astroid-3.1.0/tests/testdata/python3/pyi_data/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 16:28:02.838840 astroid-3.1.0/tests/testdata/python3/pyi_data/find_test/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-23 16:27:48.000000 astroid-3.1.0/tests/testdata/python3/pyi_data/find_test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-23 16:27:48.000000 astroid-3.1.0/tests/testdata/python3/pyi_data/find_test/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-23 16:27:48.000000 astroid-3.1.0/tests/testdata/python3/pyi_data/find_test/module.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-23 16:27:48.000000 astroid-3.1.0/tests/testdata/python3/pyi_data/find_test/module2.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-23 16:27:48.000000 astroid-3.1.0/tests/testdata/python3/pyi_data/find_test/noendingnewline.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-23 16:27:48.000000 astroid-3.1.0/tests/testdata/python3/pyi_data/find_test/nonregr.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-23 16:27:48.000000 astroid-3.1.0/tests/testdata/python3/pyi_data/module.py
--rw-r--r--   0 runner    (1001) docker     (127)     5306 2024-02-23 16:27:48.000000 astroid-3.1.0/tests/testdata/python3/recursion_error.py
--rw-r--r--   0 runner    (1001) docker     (127)      423 2024-02-23 16:27:48.000000 astroid-3.1.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 11:58:15.959415 astroid-3.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     8391 2024-05-07 11:58:06.000000 astroid-3.2.0/CONTRIBUTORS.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    26516 2024-05-07 11:58:06.000000 astroid-3.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-05-07 11:58:06.000000 astroid-3.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4483 2024-05-07 11:58:15.959415 astroid-3.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2840 2024-05-07 11:58:06.000000 astroid-3.2.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 11:58:15.923415 astroid-3.2.0/astroid/
+-rw-r--r--   0 runner    (1001) docker     (127)     4546 2024-05-07 11:58:06.000000 astroid-3.2.0/astroid/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      283 2024-05-07 11:58:06.000000 astroid-3.2.0/astroid/__pkginfo__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3033 2024-05-07 11:58:06.000000 astroid-3.2.0/astroid/_ast.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7026 2024-05-07 11:58:06.000000 astroid-3.2.0/astroid/_backport_stdlib_names.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12990 2024-05-07 11:58:06.000000 astroid-3.2.0/astroid/arguments.py
+-rw-r--r--   0 runner    (1001) docker     (127)      729 2024-05-07 11:58:06.000000 astroid-3.2.0/astroid/astroid_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27145 2024-05-07 11:58:06.000000 astroid-3.2.0/astroid/bases.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 11:58:15.931414 astroid-3.2.0/astroid/brain/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 11:58:06.000000 astroid-3.2.0/astroid/brain/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1813 2024-05-07 11:58:06.000000 astroid-3.2.0/astroid/brain/brain_argparse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3184 2024-05-07 11:58:06.000000 astroid-3.2.0/astroid/brain/brain_attrs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-05-07 11:58:06.000000 astroid-3.2.0/astroid/brain/brain_boto3.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37439 2024-05-07 11:58:06.000000 astroid-3.2.0/astroid/brain/brain_builtin_inference.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4490 2024-05-07 11:58:06.000000 astroid-3.2.0/astroid/brain/brain_collections.py
+-rw-r--r--   0 runner    (1001) docker     (127)      915 2024-05-07 11:58:06.000000 astroid-3.2.0/astroid/brain/brain_crypt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2720 2024-05-07 11:58:06.000000 astroid-3.2.0/astroid/brain/brain_ctypes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3529 2024-05-07 11:58:06.000000 astroid-3.2.0/astroid/brain/brain_curses.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22206 2024-05-07 11:58:06.000000 astroid-3.2.0/astroid/brain/brain_dataclasses.py
+-rw-r--r--   0 runner    (1001) docker     (127)      771 2024-05-07 11:58:06.000000 astroid-3.2.0/astroid/brain/brain_datetime.py
+-rw-r--r--   0 runner    (1001) docker     (127)      819 2024-05-07 11:58:06.000000 astroid-3.2.0/astroid/brain/brain_dateutil.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2769 2024-05-07 11:58:06.000000 astroid-3.2.0/astroid/brain/brain_fstrings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6390 2024-05-07 11:58:06.000000 astroid-3.2.0/astroid/brain/brain_functools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7598 2024-05-07 11:58:06.000000 astroid-3.2.0/astroid/brain/brain_gi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2873 2024-05-07 11:58:06.000000 astroid-3.2.0/astroid/brain/brain_hashlib.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10687 2024-05-07 11:58:06.000000 astroid-3.2.0/astroid/brain/brain_http.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1800 2024-05-07 11:58:06.000000 astroid-3.2.0/astroid/brain/brain_hypothesis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1589 2024-05-07 11:58:06.000000 astroid-3.2.0/astroid/brain/brain_io.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2698 2024-05-07 11:58:06.000000 astroid-3.2.0/astroid/brain/brain_mechanize.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3260 2024-05-07 11:58:06.000000 astroid-3.2.0/astroid/brain/brain_multiprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23912 2024-05-07 11:58:06.000000 astroid-3.2.0/astroid/brain/brain_namedtuple_enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2402 2024-05-07 11:58:06.000000 astroid-3.2.0/astroid/brain/brain_nose.py
+-rw-r--r--   0 runner    (1001) docker     (127)      885 2024-05-07 11:58:06.000000 astroid-3.2.0/astroid/brain/brain_numpy_core_einsumfunc.py
+-rw-r--r--   0 runner    (1001) docker     (127)      792 2024-05-07 11:58:06.000000 astroid-3.2.0/astroid/brain/brain_numpy_core_fromnumeric.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1408 2024-05-07 11:58:06.000000 astroid-3.2.0/astroid/brain/brain_numpy_core_function_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4400 2024-05-07 11:58:06.000000 astroid-3.2.0/astroid/brain/brain_numpy_core_multiarray.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1740 2024-05-07 11:58:06.000000 astroid-3.2.0/astroid/brain/brain_numpy_core_numeric.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8606 2024-05-07 11:58:06.000000 astroid-3.2.0/astroid/brain/brain_numpy_core_numerictypes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4939 2024-05-07 11:58:06.000000 astroid-3.2.0/astroid/brain/brain_numpy_core_umath.py
+-rw-r--r--   0 runner    (1001) docker     (127)      948 2024-05-07 11:58:06.000000 astroid-3.2.0/astroid/brain/brain_numpy_ma.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9066 2024-05-07 11:58:06.000000 astroid-3.2.0/astroid/brain/brain_numpy_ndarray.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3496 2024-05-07 11:58:06.000000 astroid-3.2.0/astroid/brain/brain_numpy_random_mtrand.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2553 2024-05-07 11:58:06.000000 astroid-3.2.0/astroid/brain/brain_numpy_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1610 2024-05-07 11:58:06.000000 astroid-3.2.0/astroid/brain/brain_pathlib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2252 2024-05-07 11:58:06.000000 astroid-3.2.0/astroid/brain/brain_pkg_resources.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2270 2024-05-07 11:58:06.000000 astroid-3.2.0/astroid/brain/brain_pytest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2874 2024-05-07 11:58:06.000000 astroid-3.2.0/astroid/brain/brain_qt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3170 2024-05-07 11:58:06.000000 astroid-3.2.0/astroid/brain/brain_random.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3003 2024-05-07 11:58:06.000000 astroid-3.2.0/astroid/brain/brain_re.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3495 2024-05-07 11:58:06.000000 astroid-3.2.0/astroid/brain/brain_regex.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1920 2024-05-07 11:58:06.000000 astroid-3.2.0/astroid/brain/brain_responses.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2328 2024-05-07 11:58:06.000000 astroid-3.2.0/astroid/brain/brain_scipy_signal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3932 2024-05-07 11:58:06.000000 astroid-3.2.0/astroid/brain/brain_signal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7666 2024-05-07 11:58:06.000000 astroid-3.2.0/astroid/brain/brain_six.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-05-07 11:58:06.000000 astroid-3.2.0/astroid/brain/brain_sqlalchemy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6554 2024-05-07 11:58:06.000000 astroid-3.2.0/astroid/brain/brain_ssl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3048 2024-05-07 11:58:06.000000 astroid-3.2.0/astroid/brain/brain_subprocess.py
+-rw-r--r--   0 runner    (1001) docker     (127)      922 2024-05-07 11:58:06.000000 astroid-3.2.0/astroid/brain/brain_threading.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2547 2024-05-07 11:58:06.000000 astroid-3.2.0/astroid/brain/brain_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16303 2024-05-07 11:58:06.000000 astroid-3.2.0/astroid/brain/brain_typing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-05-07 11:58:06.000000 astroid-3.2.0/astroid/brain/brain_unittest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      727 2024-05-07 11:58:06.000000 astroid-3.2.0/astroid/brain/brain_uuid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4364 2024-05-07 11:58:06.000000 astroid-3.2.0/astroid/brain/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18727 2024-05-07 11:58:06.000000 astroid-3.2.0/astroid/builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)      862 2024-05-07 11:58:06.000000 astroid-3.2.0/astroid/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5086 2024-05-07 11:58:06.000000 astroid-3.2.0/astroid/constraint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6324 2024-05-07 11:58:06.000000 astroid-3.2.0/astroid/context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8590 2024-05-07 11:58:06.000000 astroid-3.2.0/astroid/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12786 2024-05-07 11:58:06.000000 astroid-3.2.0/astroid/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9387 2024-05-07 11:58:06.000000 astroid-3.2.0/astroid/filter_statements.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11918 2024-05-07 11:58:06.000000 astroid-3.2.0/astroid/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4598 2024-05-07 11:58:06.000000 astroid-3.2.0/astroid/inference_tip.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 11:58:15.931414 astroid-3.2.0/astroid/interpreter/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 11:58:06.000000 astroid-3.2.0/astroid/interpreter/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 11:58:15.931414 astroid-3.2.0/astroid/interpreter/_import/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 11:58:06.000000 astroid-3.2.0/astroid/interpreter/_import/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17214 2024-05-07 11:58:06.000000 astroid-3.2.0/astroid/interpreter/_import/spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4702 2024-05-07 11:58:06.000000 astroid-3.2.0/astroid/interpreter/_import/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2515 2024-05-07 11:58:06.000000 astroid-3.2.0/astroid/interpreter/dunder_lookup.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34593 2024-05-07 11:58:06.000000 astroid-3.2.0/astroid/interpreter/objectmodel.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18280 2024-05-07 11:58:06.000000 astroid-3.2.0/astroid/manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23743 2024-05-07 11:58:06.000000 astroid-3.2.0/astroid/modutils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 11:58:15.931414 astroid-3.2.0/astroid/nodes/
+-rw-r--r--   0 runner    (1001) docker     (127)     4744 2024-05-07 11:58:06.000000 astroid-3.2.0/astroid/nodes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24111 2024-05-07 11:58:06.000000 astroid-3.2.0/astroid/nodes/_base_nodes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26317 2024-05-07 11:58:06.000000 astroid-3.2.0/astroid/nodes/as_string.py
+-rw-r--r--   0 runner    (1001) docker     (127)      807 2024-05-07 11:58:06.000000 astroid-3.2.0/astroid/nodes/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)   168997 2024-05-07 11:58:06.000000 astroid-3.2.0/astroid/nodes/node_classes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27045 2024-05-07 11:58:06.000000 astroid-3.2.0/astroid/nodes/node_ng.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 11:58:15.935414 astroid-3.2.0/astroid/nodes/scoped_nodes/
+-rw-r--r--   0 runner    (1001) docker     (127)     1229 2024-05-07 11:58:06.000000 astroid-3.2.0/astroid/nodes/scoped_nodes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7151 2024-05-07 11:58:06.000000 astroid-3.2.0/astroid/nodes/scoped_nodes/mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)   104912 2024-05-07 11:58:06.000000 astroid-3.2.0/astroid/nodes/scoped_nodes/scoped_nodes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1181 2024-05-07 11:58:06.000000 astroid-3.2.0/astroid/nodes/scoped_nodes/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      433 2024-05-07 11:58:06.000000 astroid-3.2.0/astroid/nodes/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13025 2024-05-07 11:58:06.000000 astroid-3.2.0/astroid/objects.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31691 2024-05-07 11:58:06.000000 astroid-3.2.0/astroid/protocols.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25314 2024-05-07 11:58:06.000000 astroid-3.2.0/astroid/raw_building.py
+-rw-r--r--   0 runner    (1001) docker     (127)    71309 2024-05-07 11:58:06.000000 astroid-3.2.0/astroid/rebuilder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2474 2024-05-07 11:58:06.000000 astroid-3.2.0/astroid/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5849 2024-05-07 11:58:06.000000 astroid-3.2.0/astroid/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2748 2024-05-07 11:58:06.000000 astroid-3.2.0/astroid/typing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4846 2024-05-07 11:58:06.000000 astroid-3.2.0/astroid/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 11:58:15.959415 astroid-3.2.0/astroid.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4483 2024-05-07 11:58:15.000000 astroid-3.2.0/astroid.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11043 2024-05-07 11:58:15.000000 astroid-3.2.0/astroid.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 11:58:15.000000 astroid-3.2.0/astroid.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-07 11:58:15.000000 astroid-3.2.0/astroid.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-07 11:58:15.000000 astroid-3.2.0/astroid.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3293 2024-05-07 11:58:06.000000 astroid-3.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-05-07 11:58:06.000000 astroid-3.2.0/requirements_dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      211 2024-05-07 11:58:06.000000 astroid-3.2.0/requirements_full.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-05-07 11:58:06.000000 astroid-3.2.0/requirements_minimal.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-05-07 11:58:15.959415 astroid-3.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 11:58:15.939415 astroid-3.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 11:58:06.000000 astroid-3.2.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 11:58:15.943415 astroid-3.2.0/tests/brain/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 11:58:06.000000 astroid-3.2.0/tests/brain/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 11:58:15.943415 astroid-3.2.0/tests/brain/numpy/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 11:58:06.000000 astroid-3.2.0/tests/brain/numpy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1708 2024-05-07 11:58:06.000000 astroid-3.2.0/tests/brain/numpy/test_core_einsumfunc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1629 2024-05-07 11:58:06.000000 astroid-3.2.0/tests/brain/numpy/test_core_fromnumeric.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1766 2024-05-07 11:58:06.000000 astroid-3.2.0/tests/brain/numpy/test_core_function_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7681 2024-05-07 11:58:06.000000 astroid-3.2.0/tests/brain/numpy/test_core_multiarray.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2556 2024-05-07 11:58:06.000000 astroid-3.2.0/tests/brain/numpy/test_core_numeric.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11199 2024-05-07 11:58:06.000000 astroid-3.2.0/tests/brain/numpy/test_core_numerictypes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7744 2024-05-07 11:58:06.000000 astroid-3.2.0/tests/brain/numpy/test_core_umath.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1494 2024-05-07 11:58:06.000000 astroid-3.2.0/tests/brain/numpy/test_ma.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4897 2024-05-07 11:58:06.000000 astroid-3.2.0/tests/brain/numpy/test_ndarray.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4525 2024-05-07 11:58:06.000000 astroid-3.2.0/tests/brain/numpy/test_random_mtrand.py
+-rw-r--r--   0 runner    (1001) docker     (127)      734 2024-05-07 11:58:06.000000 astroid-3.2.0/tests/brain/test_argparse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4987 2024-05-07 11:58:06.000000 astroid-3.2.0/tests/brain/test_attr.py
+-rw-r--r--   0 runner    (1001) docker     (127)    63783 2024-05-07 11:58:06.000000 astroid-3.2.0/tests/brain/test_brain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5073 2024-05-07 11:58:06.000000 astroid-3.2.0/tests/brain/test_builtin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3489 2024-05-07 11:58:06.000000 astroid-3.2.0/tests/brain/test_ctypes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35395 2024-05-07 11:58:06.000000 astroid-3.2.0/tests/brain/test_dataclasses.py
+-rw-r--r--   0 runner    (1001) docker     (127)      897 2024-05-07 11:58:06.000000 astroid-3.2.0/tests/brain/test_dateutil.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18541 2024-05-07 11:58:06.000000 astroid-3.2.0/tests/brain/test_enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2707 2024-05-07 11:58:06.000000 astroid-3.2.0/tests/brain/test_hashlib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4035 2024-05-07 11:58:06.000000 astroid-3.2.0/tests/brain/test_multiprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10754 2024-05-07 11:58:06.000000 astroid-3.2.0/tests/brain/test_named_tuple.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1687 2024-05-07 11:58:06.000000 astroid-3.2.0/tests/brain/test_nose.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2206 2024-05-07 11:58:06.000000 astroid-3.2.0/tests/brain/test_pathlib.py
+-rw-r--r--   0 runner    (1001) docker     (127)      795 2024-05-07 11:58:06.000000 astroid-3.2.0/tests/brain/test_pytest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3008 2024-05-07 11:58:06.000000 astroid-3.2.0/tests/brain/test_qt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1788 2024-05-07 11:58:06.000000 astroid-3.2.0/tests/brain/test_regex.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1324 2024-05-07 11:58:06.000000 astroid-3.2.0/tests/brain/test_signal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6067 2024-05-07 11:58:06.000000 astroid-3.2.0/tests/brain/test_six.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1626 2024-05-07 11:58:06.000000 astroid-3.2.0/tests/brain/test_ssl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1796 2024-05-07 11:58:06.000000 astroid-3.2.0/tests/brain/test_threading.py
+-rw-r--r--   0 runner    (1001) docker     (127)      730 2024-05-07 11:58:06.000000 astroid-3.2.0/tests/brain/test_typing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1265 2024-05-07 11:58:06.000000 astroid-3.2.0/tests/brain/test_typing_extensions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1047 2024-05-07 11:58:06.000000 astroid-3.2.0/tests/brain/test_unittest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-05-07 11:58:06.000000 astroid-3.2.0/tests/resources.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35331 2024-05-07 11:58:06.000000 astroid-3.2.0/tests/test_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15433 2024-05-07 11:58:06.000000 astroid-3.2.0/tests/test_constraint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3793 2024-05-07 11:58:06.000000 astroid-3.2.0/tests/test_decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)      642 2024-05-07 11:58:06.000000 astroid-3.2.0/tests/test_filter_statements.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3530 2024-05-07 11:58:06.000000 astroid-3.2.0/tests/test_group_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9634 2024-05-07 11:58:06.000000 astroid-3.2.0/tests/test_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)   226239 2024-05-07 11:58:06.000000 astroid-3.2.0/tests/test_inference.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14712 2024-05-07 11:58:06.000000 astroid-3.2.0/tests/test_inference_calls.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34856 2024-05-07 11:58:06.000000 astroid-3.2.0/tests/test_lookup.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20401 2024-05-07 11:58:06.000000 astroid-3.2.0/tests/test_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22964 2024-05-07 11:58:06.000000 astroid-3.2.0/tests/test_modutils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    66136 2024-05-07 11:58:06.000000 astroid-3.2.0/tests/test_nodes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    55445 2024-05-07 11:58:06.000000 astroid-3.2.0/tests/test_nodes_lineno.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4167 2024-05-07 11:58:06.000000 astroid-3.2.0/tests/test_nodes_position.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27854 2024-05-07 11:58:06.000000 astroid-3.2.0/tests/test_object_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21338 2024-05-07 11:58:06.000000 astroid-3.2.0/tests/test_objects.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16017 2024-05-07 11:58:06.000000 astroid-3.2.0/tests/test_protocols.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14453 2024-05-07 11:58:06.000000 astroid-3.2.0/tests/test_python3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5910 2024-05-07 11:58:06.000000 astroid-3.2.0/tests/test_raw_building.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15105 2024-05-07 11:58:06.000000 astroid-3.2.0/tests/test_regrtest.py
+-rw-r--r--   0 runner    (1001) docker     (127)    93585 2024-05-07 11:58:06.000000 astroid-3.2.0/tests/test_scoped_nodes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-05-07 11:58:06.000000 astroid-3.2.0/tests/test_stdlib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9826 2024-05-07 11:58:06.000000 astroid-3.2.0/tests/test_transforms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2711 2024-05-07 11:58:06.000000 astroid-3.2.0/tests/test_type_params.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6459 2024-05-07 11:58:06.000000 astroid-3.2.0/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 11:58:15.911414 astroid-3.2.0/tests/testdata/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 11:58:15.943415 astroid-3.2.0/tests/testdata/python3/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 11:58:15.947414 astroid-3.2.0/tests/testdata/python3/data/
+-rw-r--r--   0 runner    (1001) docker     (127)     1222 2024-05-07 11:58:06.000000 astroid-3.2.0/tests/testdata/python3/data/MyPyPa-0.1.0-py2.5.egg
+-rw-r--r--   0 runner    (1001) docker     (127)     1222 2024-05-07 11:58:06.000000 astroid-3.2.0/tests/testdata/python3/data/MyPyPa-0.1.0-py2.5.zip
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 11:58:15.947414 astroid-3.2.0/tests/testdata/python3/data/SSL1/
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-05-07 11:58:06.000000 astroid-3.2.0/tests/testdata/python3/data/SSL1/Connection1.py
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-07 11:58:06.000000 astroid-3.2.0/tests/testdata/python3/data/SSL1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-07 11:58:06.000000 astroid-3.2.0/tests/testdata/python3/data/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 11:58:15.947414 astroid-3.2.0/tests/testdata/python3/data/absimp/
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-07 11:58:06.000000 astroid-3.2.0/tests/testdata/python3/data/absimp/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 11:58:15.947414 astroid-3.2.0/tests/testdata/python3/data/absimp/sidepackage/
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-07 11:58:06.000000 astroid-3.2.0/tests/testdata/python3/data/absimp/sidepackage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-07 11:58:06.000000 astroid-3.2.0/tests/testdata/python3/data/absimp/string.py
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-07 11:58:06.000000 astroid-3.2.0/tests/testdata/python3/data/absimport.py
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-05-07 11:58:06.000000 astroid-3.2.0/tests/testdata/python3/data/all.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 11:58:15.951414 astroid-3.2.0/tests/testdata/python3/data/appl/
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-07 11:58:06.000000 astroid-3.2.0/tests/testdata/python3/data/appl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      261 2024-05-07 11:58:06.000000 astroid-3.2.0/tests/testdata/python3/data/appl/myConnection.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 11:58:15.951414 astroid-3.2.0/tests/testdata/python3/data/beyond_top_level/
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-05-07 11:58:06.000000 astroid-3.2.0/tests/testdata/python3/data/beyond_top_level/import_package.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 11:58:15.951414 astroid-3.2.0/tests/testdata/python3/data/beyond_top_level/namespace_package/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 11:58:15.951414 astroid-3.2.0/tests/testdata/python3/data/beyond_top_level/namespace_package/lower_level/
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-05-07 11:58:06.000000 astroid-3.2.0/tests/testdata/python3/data/beyond_top_level/namespace_package/lower_level/helper_function.py
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-05-07 11:58:06.000000 astroid-3.2.0/tests/testdata/python3/data/beyond_top_level/namespace_package/plugin_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-05-07 11:58:06.000000 astroid-3.2.0/tests/testdata/python3/data/beyond_top_level/namespace_package/top_level_function.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 11:58:15.911414 astroid-3.2.0/tests/testdata/python3/data/beyond_top_level_three/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 11:58:15.951414 astroid-3.2.0/tests/testdata/python3/data/beyond_top_level_three/double_name/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 11:58:06.000000 astroid-3.2.0/tests/testdata/python3/data/beyond_top_level_three/double_name/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 11:58:15.951414 astroid-3.2.0/tests/testdata/python3/data/beyond_top_level_three/module/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 11:58:06.000000 astroid-3.2.0/tests/testdata/python3/data/beyond_top_level_three/module/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 11:58:15.951414 astroid-3.2.0/tests/testdata/python3/data/beyond_top_level_three/module/double_name/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 11:58:06.000000 astroid-3.2.0/tests/testdata/python3/data/beyond_top_level_three/module/double_name/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 11:58:06.000000 astroid-3.2.0/tests/testdata/python3/data/beyond_top_level_three/module/double_name/function.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 11:58:15.951414 astroid-3.2.0/tests/testdata/python3/data/beyond_top_level_three/module/sub_module/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 11:58:06.000000 astroid-3.2.0/tests/testdata/python3/data/beyond_top_level_three/module/sub_module/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 11:58:15.951414 astroid-3.2.0/tests/testdata/python3/data/beyond_top_level_three/module/sub_module/sub_sub_module/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 11:58:06.000000 astroid-3.2.0/tests/testdata/python3/data/beyond_top_level_three/module/sub_module/sub_sub_module/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-07 11:58:06.000000 astroid-3.2.0/tests/testdata/python3/data/beyond_top_level_three/module/sub_module/sub_sub_module/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 11:58:15.951414 astroid-3.2.0/tests/testdata/python3/data/beyond_top_level_two/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 11:58:06.000000 astroid-3.2.0/tests/testdata/python3/data/beyond_top_level_two/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-05-07 11:58:06.000000 astroid-3.2.0/tests/testdata/python3/data/beyond_top_level_two/a.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 11:58:15.951414 astroid-3.2.0/tests/testdata/python3/data/beyond_top_level_two/level1/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-07 11:58:06.000000 astroid-3.2.0/tests/testdata/python3/data/beyond_top_level_two/level1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-07 11:58:06.000000 astroid-3.2.0/tests/testdata/python3/data/beyond_top_level_two/level1/beyond_top_level_two.py
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-07 11:58:06.000000 astroid-3.2.0/tests/testdata/python3/data/conditional.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 11:58:15.951414 astroid-3.2.0/tests/testdata/python3/data/conditional_import/
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-05-07 11:58:06.000000 astroid-3.2.0/tests/testdata/python3/data/conditional_import/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 11:58:15.911414 astroid-3.2.0/tests/testdata/python3/data/contribute_to_namespace/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 11:58:15.951414 astroid-3.2.0/tests/testdata/python3/data/contribute_to_namespace/namespace_pep_420/
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-07 11:58:06.000000 astroid-3.2.0/tests/testdata/python3/data/contribute_to_namespace/namespace_pep_420/submodule.py
+-rw-r--r--   0 runner    (1001) docker     (127)      217 2024-05-07 11:58:06.000000 astroid-3.2.0/tests/testdata/python3/data/descriptor_crash.py
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-07 11:58:06.000000 astroid-3.2.0/tests/testdata/python3/data/email.py
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-05-07 11:58:06.000000 astroid-3.2.0/tests/testdata/python3/data/fake_module_with_broken_getattr.py
+-rw-r--r--   0 runner    (1001) docker     (127)      661 2024-05-07 11:58:06.000000 astroid-3.2.0/tests/testdata/python3/data/fake_module_with_warnings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 11:58:15.951414 astroid-3.2.0/tests/testdata/python3/data/find_test/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 11:58:06.000000 astroid-3.2.0/tests/testdata/python3/data/find_test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 11:58:06.000000 astroid-3.2.0/tests/testdata/python3/data/find_test/module.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 11:58:06.000000 astroid-3.2.0/tests/testdata/python3/data/find_test/module2.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 11:58:06.000000 astroid-3.2.0/tests/testdata/python3/data/find_test/noendingnewline.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 11:58:06.000000 astroid-3.2.0/tests/testdata/python3/data/find_test/nonregr.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 11:58:15.911414 astroid-3.2.0/tests/testdata/python3/data/foogle/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 11:58:15.951414 astroid-3.2.0/tests/testdata/python3/data/foogle/fax/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 11:58:06.000000 astroid-3.2.0/tests/testdata/python3/data/foogle/fax/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-07 11:58:06.000000 astroid-3.2.0/tests/testdata/python3/data/foogle/fax/a.py
+-rw-r--r--   0 runner    (1001) docker     (127)      629 2024-05-07 11:58:06.000000 astroid-3.2.0/tests/testdata/python3/data/foogle_fax-0.12.5-py2.7-nspkg.pth
+-rw-r--r--   0 runner    (1001) docker     (127)      421 2024-05-07 11:58:06.000000 astroid-3.2.0/tests/testdata/python3/data/format.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 11:58:15.951414 astroid-3.2.0/tests/testdata/python3/data/import_conflicting_names/
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-07 11:58:06.000000 astroid-3.2.0/tests/testdata/python3/data/import_conflicting_names/math.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 11:58:15.951414 astroid-3.2.0/tests/testdata/python3/data/import_setuptools_pep660/
+-rw-r--r--   0 runner    (1001) docker     (127)     2709 2024-05-07 11:58:06.000000 astroid-3.2.0/tests/testdata/python3/data/import_setuptools_pep660/__editable___example_0_1_0_finder.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 11:58:15.951414 astroid-3.2.0/tests/testdata/python3/data/import_setuptools_pep660/example/
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-07 11:58:06.000000 astroid-3.2.0/tests/testdata/python3/data/import_setuptools_pep660/example/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 11:58:15.955415 astroid-3.2.0/tests/testdata/python3/data/import_setuptools_pep660/example/subpackage/
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-07 11:58:06.000000 astroid-3.2.0/tests/testdata/python3/data/import_setuptools_pep660/example/subpackage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-07 11:58:06.000000 astroid-3.2.0/tests/testdata/python3/data/invalid_encoding.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 11:58:15.955415 astroid-3.2.0/tests/testdata/python3/data/lmfp/
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-07 11:58:06.000000 astroid-3.2.0/tests/testdata/python3/data/lmfp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-05-07 11:58:06.000000 astroid-3.2.0/tests/testdata/python3/data/lmfp/foo.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 11:58:15.955415 astroid-3.2.0/tests/testdata/python3/data/max_inferable_limit_for_classes/
+-rw-r--r--   0 runner    (1001) docker     (127)      667 2024-05-07 11:58:06.000000 astroid-3.2.0/tests/testdata/python3/data/max_inferable_limit_for_classes/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 11:58:15.955415 astroid-3.2.0/tests/testdata/python3/data/max_inferable_limit_for_classes/nodes/
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-05-07 11:58:06.000000 astroid-3.2.0/tests/testdata/python3/data/max_inferable_limit_for_classes/nodes/roles.py
+-rw-r--r--   0 runner    (1001) docker     (127)      459 2024-05-07 11:58:06.000000 astroid-3.2.0/tests/testdata/python3/data/max_inferable_limit_for_classes/other_funcs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 11:58:15.955415 astroid-3.2.0/tests/testdata/python3/data/metaclass_recursion/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 11:58:06.000000 astroid-3.2.0/tests/testdata/python3/data/metaclass_recursion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      614 2024-05-07 11:58:06.000000 astroid-3.2.0/tests/testdata/python3/data/metaclass_recursion/monkeypatch.py
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-07 11:58:06.000000 astroid-3.2.0/tests/testdata/python3/data/metaclass_recursion/parent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1784 2024-05-07 11:58:06.000000 astroid-3.2.0/tests/testdata/python3/data/module.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 11:58:15.955415 astroid-3.2.0/tests/testdata/python3/data/module1abs/
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-07 11:58:06.000000 astroid-3.2.0/tests/testdata/python3/data/module1abs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-07 11:58:06.000000 astroid-3.2.0/tests/testdata/python3/data/module1abs/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1949 2024-05-07 11:58:06.000000 astroid-3.2.0/tests/testdata/python3/data/module2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 11:58:15.955415 astroid-3.2.0/tests/testdata/python3/data/module_dict_items_call/
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-07 11:58:06.000000 astroid-3.2.0/tests/testdata/python3/data/module_dict_items_call/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-05-07 11:58:06.000000 astroid-3.2.0/tests/testdata/python3/data/module_dict_items_call/test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 11:58:15.955415 astroid-3.2.0/tests/testdata/python3/data/namespace_pep_420/
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-07 11:58:06.000000 astroid-3.2.0/tests/testdata/python3/data/namespace_pep_420/module.py
+-rw-r--r--   0 runner    (1001) docker     (127)      506 2024-05-07 11:58:06.000000 astroid-3.2.0/tests/testdata/python3/data/noendingnewline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1010 2024-05-07 11:58:06.000000 astroid-3.2.0/tests/testdata/python3/data/nonregr.py
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-07 11:58:06.000000 astroid-3.2.0/tests/testdata/python3/data/notall.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 11:58:15.955415 astroid-3.2.0/tests/testdata/python3/data/notamodule/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 11:58:06.000000 astroid-3.2.0/tests/testdata/python3/data/notamodule/file.py
+-rw-r--r--   0 runner    (1001) docker     (127)      823 2024-05-07 11:58:06.000000 astroid-3.2.0/tests/testdata/python3/data/operator_precedence.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 11:58:15.955415 astroid-3.2.0/tests/testdata/python3/data/package/
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-05-07 11:58:06.000000 astroid-3.2.0/tests/testdata/python3/data/package/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-05-07 11:58:06.000000 astroid-3.2.0/tests/testdata/python3/data/package/absimport.py
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-07 11:58:06.000000 astroid-3.2.0/tests/testdata/python3/data/package/hello.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2242 2024-05-07 11:58:06.000000 astroid-3.2.0/tests/testdata/python3/data/package/import_package_subpackage_module.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 11:58:15.955415 astroid-3.2.0/tests/testdata/python3/data/package/subpackage/
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-07 11:58:06.000000 astroid-3.2.0/tests/testdata/python3/data/package/subpackage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-07 11:58:06.000000 astroid-3.2.0/tests/testdata/python3/data/package/subpackage/module.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 11:58:15.955415 astroid-3.2.0/tests/testdata/python3/data/parent_of_homonym/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 11:58:06.000000 astroid-3.2.0/tests/testdata/python3/data/parent_of_homonym/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 11:58:15.955415 astroid-3.2.0/tests/testdata/python3/data/parent_of_homonym/doc/
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-05-07 11:58:06.000000 astroid-3.2.0/tests/testdata/python3/data/parent_of_homonym/doc/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 11:58:06.000000 astroid-3.2.0/tests/testdata/python3/data/parent_of_homonym/doc/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 11:58:15.915414 astroid-3.2.0/tests/testdata/python3/data/path_pkg_resources_1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 11:58:15.955415 astroid-3.2.0/tests/testdata/python3/data/path_pkg_resources_1/package/
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-05-07 11:58:06.000000 astroid-3.2.0/tests/testdata/python3/data/path_pkg_resources_1/package/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 11:58:06.000000 astroid-3.2.0/tests/testdata/python3/data/path_pkg_resources_1/package/foo.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 11:58:15.915414 astroid-3.2.0/tests/testdata/python3/data/path_pkg_resources_2/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 11:58:15.959415 astroid-3.2.0/tests/testdata/python3/data/path_pkg_resources_2/package/
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-07 11:58:06.000000 astroid-3.2.0/tests/testdata/python3/data/path_pkg_resources_2/package/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 11:58:06.000000 astroid-3.2.0/tests/testdata/python3/data/path_pkg_resources_2/package/bar.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 11:58:15.915414 astroid-3.2.0/tests/testdata/python3/data/path_pkg_resources_3/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 11:58:15.959415 astroid-3.2.0/tests/testdata/python3/data/path_pkg_resources_3/package/
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-07 11:58:06.000000 astroid-3.2.0/tests/testdata/python3/data/path_pkg_resources_3/package/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 11:58:06.000000 astroid-3.2.0/tests/testdata/python3/data/path_pkg_resources_3/package/baz.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 11:58:15.915414 astroid-3.2.0/tests/testdata/python3/data/path_pkgutil_1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 11:58:15.959415 astroid-3.2.0/tests/testdata/python3/data/path_pkgutil_1/package/
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-07 11:58:06.000000 astroid-3.2.0/tests/testdata/python3/data/path_pkgutil_1/package/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 11:58:06.000000 astroid-3.2.0/tests/testdata/python3/data/path_pkgutil_1/package/foo.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 11:58:15.915414 astroid-3.2.0/tests/testdata/python3/data/path_pkgutil_2/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 11:58:15.959415 astroid-3.2.0/tests/testdata/python3/data/path_pkgutil_2/package/
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-07 11:58:06.000000 astroid-3.2.0/tests/testdata/python3/data/path_pkgutil_2/package/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 11:58:06.000000 astroid-3.2.0/tests/testdata/python3/data/path_pkgutil_2/package/bar.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 11:58:15.915414 astroid-3.2.0/tests/testdata/python3/data/path_pkgutil_3/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 11:58:15.959415 astroid-3.2.0/tests/testdata/python3/data/path_pkgutil_3/package/
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-07 11:58:06.000000 astroid-3.2.0/tests/testdata/python3/data/path_pkgutil_3/package/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 11:58:06.000000 astroid-3.2.0/tests/testdata/python3/data/path_pkgutil_3/package/baz.py
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-07 11:58:06.000000 astroid-3.2.0/tests/testdata/python3/data/recursion.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 11:58:06.000000 astroid-3.2.0/tests/testdata/python3/data/tmp__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 11:58:15.959415 astroid-3.2.0/tests/testdata/python3/data/unicode_package/
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-07 11:58:06.000000 astroid-3.2.0/tests/testdata/python3/data/unicode_package/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 11:58:15.959415 astroid-3.2.0/tests/testdata/python3/data/unicode_package/core/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 11:58:06.000000 astroid-3.2.0/tests/testdata/python3/data/unicode_package/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 11:58:15.959415 astroid-3.2.0/tests/testdata/python3/pyi_data/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 11:58:06.000000 astroid-3.2.0/tests/testdata/python3/pyi_data/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 11:58:15.959415 astroid-3.2.0/tests/testdata/python3/pyi_data/find_test/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 11:58:06.000000 astroid-3.2.0/tests/testdata/python3/pyi_data/find_test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 11:58:06.000000 astroid-3.2.0/tests/testdata/python3/pyi_data/find_test/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 11:58:06.000000 astroid-3.2.0/tests/testdata/python3/pyi_data/find_test/module.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 11:58:06.000000 astroid-3.2.0/tests/testdata/python3/pyi_data/find_test/module2.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 11:58:06.000000 astroid-3.2.0/tests/testdata/python3/pyi_data/find_test/noendingnewline.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 11:58:06.000000 astroid-3.2.0/tests/testdata/python3/pyi_data/find_test/nonregr.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 11:58:06.000000 astroid-3.2.0/tests/testdata/python3/pyi_data/module.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5306 2024-05-07 11:58:06.000000 astroid-3.2.0/tests/testdata/python3/recursion_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)      423 2024-05-07 11:58:06.000000 astroid-3.2.0/tox.ini
```

### Comparing `astroid-3.1.0/CONTRIBUTORS.txt` & `astroid-3.2.0/CONTRIBUTORS.txt`

 * *Files 1% similar despite different names*

```diff
@@ -200,7 +200,9 @@
 under this name, or we did not manage to find their commits in the history.
 
 - François Mockers
 - platings
 - carl
 - alain lefroy
 - Mark Gius
+- Jérome Perrin <perrinjerome@gmail.com>
+- Jamie Scott <jamie@jami.org.uk>
```

### Comparing `astroid-3.1.0/LICENSE` & `astroid-3.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `astroid-3.1.0/PKG-INFO` & `astroid-3.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: astroid
-Version: 3.1.0
+Version: 3.2.0
 Summary: An abstract syntax tree for Python with inference support.
 License: LGPL-2.1-or-later
 Project-URL: Docs, https://pylint.readthedocs.io/projects/astroid/en/latest/
 Project-URL: Source Code, https://github.com/pylint-dev/astroid
 Project-URL: Bug tracker, https://github.com/pylint-dev/astroid/issues
 Project-URL: Discord server, https://discord.gg/Egy6P8AMB5
 Keywords: static code analysis,python,abstract syntax tree
```

### Comparing `astroid-3.1.0/README.rst` & `astroid-3.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `astroid-3.1.0/astroid/__init__.py` & `astroid-3.2.0/astroid/__init__.py`

 * *Files identical despite different names*

### Comparing `astroid-3.1.0/astroid/_ast.py` & `astroid-3.2.0/astroid/_ast.py`

 * *Files identical despite different names*

### Comparing `astroid-3.1.0/astroid/_backport_stdlib_names.py` & `astroid-3.2.0/astroid/_backport_stdlib_names.py`

 * *Files identical despite different names*

### Comparing `astroid-3.1.0/astroid/arguments.py` & `astroid-3.2.0/astroid/arguments.py`

 * *Files identical despite different names*

### Comparing `astroid-3.1.0/astroid/astroid_manager.py` & `astroid-3.2.0/astroid/astroid_manager.py`

 * *Files identical despite different names*

### Comparing `astroid-3.1.0/astroid/bases.py` & `astroid-3.2.0/astroid/bases.py`

 * *Files identical despite different names*

### Comparing `astroid-3.1.0/astroid/brain/brain_argparse.py` & `astroid-3.2.0/astroid/brain/brain_argparse.py`

 * *Files identical despite different names*

### Comparing `astroid-3.1.0/astroid/brain/brain_attrs.py` & `astroid-3.2.0/astroid/brain/brain_attrs.py`

 * *Files identical despite different names*

### Comparing `astroid-3.1.0/astroid/brain/brain_boto3.py` & `astroid-3.2.0/astroid/brain/brain_boto3.py`

 * *Files identical despite different names*

### Comparing `astroid-3.1.0/astroid/brain/brain_builtin_inference.py` & `astroid-3.2.0/astroid/brain/brain_builtin_inference.py`

 * *Files identical despite different names*

### Comparing `astroid-3.1.0/astroid/brain/brain_collections.py` & `astroid-3.2.0/astroid/brain/brain_collections.py`

 * *Files identical despite different names*

### Comparing `astroid-3.1.0/astroid/brain/brain_crypt.py` & `astroid-3.2.0/astroid/brain/brain_crypt.py`

 * *Files identical despite different names*

### Comparing `astroid-3.1.0/astroid/brain/brain_ctypes.py` & `astroid-3.2.0/astroid/brain/brain_ctypes.py`

 * *Files identical despite different names*

### Comparing `astroid-3.1.0/astroid/brain/brain_curses.py` & `astroid-3.2.0/astroid/brain/brain_curses.py`

 * *Files identical despite different names*

### Comparing `astroid-3.1.0/astroid/brain/brain_dataclasses.py` & `astroid-3.2.0/astroid/brain/brain_dataclasses.py`

 * *Files identical despite different names*

### Comparing `astroid-3.1.0/astroid/brain/brain_datetime.py` & `astroid-3.2.0/astroid/brain/brain_datetime.py`

 * *Files identical despite different names*

### Comparing `astroid-3.1.0/astroid/brain/brain_dateutil.py` & `astroid-3.2.0/astroid/brain/brain_dateutil.py`

 * *Files identical despite different names*

### Comparing `astroid-3.1.0/astroid/brain/brain_fstrings.py` & `astroid-3.2.0/astroid/brain/brain_fstrings.py`

 * *Files identical despite different names*

### Comparing `astroid-3.1.0/astroid/brain/brain_functools.py` & `astroid-3.2.0/astroid/brain/brain_functools.py`

 * *Files identical despite different names*

### Comparing `astroid-3.1.0/astroid/brain/brain_gi.py` & `astroid-3.2.0/astroid/brain/brain_gi.py`

 * *Files identical despite different names*

### Comparing `astroid-3.1.0/astroid/brain/brain_hashlib.py` & `astroid-3.2.0/astroid/brain/brain_hashlib.py`

 * *Files identical despite different names*

### Comparing `astroid-3.1.0/astroid/brain/brain_http.py` & `astroid-3.2.0/astroid/brain/brain_http.py`

 * *Files identical despite different names*

### Comparing `astroid-3.1.0/astroid/brain/brain_hypothesis.py` & `astroid-3.2.0/astroid/brain/brain_hypothesis.py`

 * *Files identical despite different names*

### Comparing `astroid-3.1.0/astroid/brain/brain_io.py` & `astroid-3.2.0/astroid/brain/brain_io.py`

 * *Files identical despite different names*

### Comparing `astroid-3.1.0/astroid/brain/brain_mechanize.py` & `astroid-3.2.0/astroid/brain/brain_mechanize.py`

 * *Files identical despite different names*

### Comparing `astroid-3.1.0/astroid/brain/brain_multiprocessing.py` & `astroid-3.2.0/astroid/brain/brain_multiprocessing.py`

 * *Files identical despite different names*

### Comparing `astroid-3.1.0/astroid/brain/brain_namedtuple_enum.py` & `astroid-3.2.0/astroid/brain/brain_namedtuple_enum.py`

 * *Files identical despite different names*

### Comparing `astroid-3.1.0/astroid/brain/brain_nose.py` & `astroid-3.2.0/astroid/brain/brain_nose.py`

 * *Files identical despite different names*

### Comparing `astroid-3.1.0/astroid/brain/brain_numpy_core_einsumfunc.py` & `astroid-3.2.0/astroid/brain/brain_numpy_core_einsumfunc.py`

 * *Files identical despite different names*

### Comparing `astroid-3.1.0/astroid/brain/brain_numpy_core_fromnumeric.py` & `astroid-3.2.0/astroid/brain/brain_numpy_core_fromnumeric.py`

 * *Files identical despite different names*

### Comparing `astroid-3.1.0/astroid/brain/brain_numpy_core_function_base.py` & `astroid-3.2.0/astroid/brain/brain_numpy_core_function_base.py`

 * *Files identical despite different names*

### Comparing `astroid-3.1.0/astroid/brain/brain_numpy_core_multiarray.py` & `astroid-3.2.0/astroid/brain/brain_numpy_core_multiarray.py`

 * *Files identical despite different names*

### Comparing `astroid-3.1.0/astroid/brain/brain_numpy_core_numeric.py` & `astroid-3.2.0/astroid/brain/brain_numpy_core_numeric.py`

 * *Files identical despite different names*

### Comparing `astroid-3.1.0/astroid/brain/brain_numpy_core_numerictypes.py` & `astroid-3.2.0/astroid/brain/brain_numpy_core_numerictypes.py`

 * *Files identical despite different names*

### Comparing `astroid-3.1.0/astroid/brain/brain_numpy_core_umath.py` & `astroid-3.2.0/astroid/brain/brain_numpy_core_umath.py`

 * *Files identical despite different names*

### Comparing `astroid-3.1.0/astroid/brain/brain_numpy_ma.py` & `astroid-3.2.0/astroid/brain/brain_numpy_ma.py`

 * *Files identical despite different names*

### Comparing `astroid-3.1.0/astroid/brain/brain_numpy_ndarray.py` & `astroid-3.2.0/astroid/brain/brain_numpy_ndarray.py`

 * *Files identical despite different names*

### Comparing `astroid-3.1.0/astroid/brain/brain_numpy_random_mtrand.py` & `astroid-3.2.0/astroid/brain/brain_numpy_random_mtrand.py`

 * *Files identical despite different names*

### Comparing `astroid-3.1.0/astroid/brain/brain_numpy_utils.py` & `astroid-3.2.0/astroid/brain/brain_numpy_utils.py`

 * *Files identical despite different names*

### Comparing `astroid-3.1.0/astroid/brain/brain_pathlib.py` & `astroid-3.2.0/astroid/brain/brain_pathlib.py`

 * *Files identical despite different names*

### Comparing `astroid-3.1.0/astroid/brain/brain_pkg_resources.py` & `astroid-3.2.0/astroid/brain/brain_pkg_resources.py`

 * *Files identical despite different names*

### Comparing `astroid-3.1.0/astroid/brain/brain_pytest.py` & `astroid-3.2.0/astroid/brain/brain_pytest.py`

 * *Files identical despite different names*

### Comparing `astroid-3.1.0/astroid/brain/brain_qt.py` & `astroid-3.2.0/astroid/brain/brain_qt.py`

 * *Files identical despite different names*

### Comparing `astroid-3.1.0/astroid/brain/brain_random.py` & `astroid-3.2.0/astroid/brain/brain_random.py`

 * *Files identical despite different names*

### Comparing `astroid-3.1.0/astroid/brain/brain_re.py` & `astroid-3.2.0/astroid/brain/brain_re.py`

 * *Files identical despite different names*

### Comparing `astroid-3.1.0/astroid/brain/brain_regex.py` & `astroid-3.2.0/astroid/brain/brain_regex.py`

 * *Files identical despite different names*

### Comparing `astroid-3.1.0/astroid/brain/brain_responses.py` & `astroid-3.2.0/astroid/brain/brain_responses.py`

 * *Files identical despite different names*

### Comparing `astroid-3.1.0/astroid/brain/brain_scipy_signal.py` & `astroid-3.2.0/astroid/brain/brain_scipy_signal.py`

 * *Files identical despite different names*

### Comparing `astroid-3.1.0/astroid/brain/brain_signal.py` & `astroid-3.2.0/astroid/brain/brain_signal.py`

 * *Files identical despite different names*

### Comparing `astroid-3.1.0/astroid/brain/brain_six.py` & `astroid-3.2.0/astroid/brain/brain_six.py`

 * *Files identical despite different names*

### Comparing `astroid-3.1.0/astroid/brain/brain_sqlalchemy.py` & `astroid-3.2.0/astroid/brain/brain_sqlalchemy.py`

 * *Files identical despite different names*

### Comparing `astroid-3.1.0/astroid/brain/brain_ssl.py` & `astroid-3.2.0/astroid/brain/brain_ssl.py`

 * *Files identical despite different names*

### Comparing `astroid-3.1.0/astroid/brain/brain_subprocess.py` & `astroid-3.2.0/astroid/brain/brain_subprocess.py`

 * *Files identical despite different names*

### Comparing `astroid-3.1.0/astroid/brain/brain_threading.py` & `astroid-3.2.0/astroid/brain/brain_threading.py`

 * *Files identical despite different names*

### Comparing `astroid-3.1.0/astroid/brain/brain_type.py` & `astroid-3.2.0/astroid/brain/brain_type.py`

 * *Files identical despite different names*

### Comparing `astroid-3.1.0/astroid/brain/brain_typing.py` & `astroid-3.2.0/astroid/brain/brain_typing.py`

 * *Files identical despite different names*

### Comparing `astroid-3.1.0/astroid/brain/brain_unittest.py` & `astroid-3.2.0/astroid/brain/brain_unittest.py`

 * *Files identical despite different names*

### Comparing `astroid-3.1.0/astroid/brain/brain_uuid.py` & `astroid-3.2.0/astroid/brain/brain_uuid.py`

 * *Files identical despite different names*

### Comparing `astroid-3.1.0/astroid/brain/helpers.py` & `astroid-3.2.0/astroid/brain/helpers.py`

 * *Files identical despite different names*

### Comparing `astroid-3.1.0/astroid/builder.py` & `astroid-3.2.0/astroid/builder.py`

 * *Files identical despite different names*

### Comparing `astroid-3.1.0/astroid/const.py` & `astroid-3.2.0/astroid/const.py`

 * *Files identical despite different names*

### Comparing `astroid-3.1.0/astroid/constraint.py` & `astroid-3.2.0/astroid/constraint.py`

 * *Files identical despite different names*

### Comparing `astroid-3.1.0/astroid/context.py` & `astroid-3.2.0/astroid/context.py`

 * *Files identical despite different names*

### Comparing `astroid-3.1.0/astroid/decorators.py` & `astroid-3.2.0/astroid/decorators.py`

 * *Files identical despite different names*

### Comparing `astroid-3.1.0/astroid/exceptions.py` & `astroid-3.2.0/astroid/exceptions.py`

 * *Files identical despite different names*

### Comparing `astroid-3.1.0/astroid/filter_statements.py` & `astroid-3.2.0/astroid/filter_statements.py`

 * *Files identical despite different names*

### Comparing `astroid-3.1.0/astroid/helpers.py` & `astroid-3.2.0/astroid/helpers.py`

 * *Files identical despite different names*

### Comparing `astroid-3.1.0/astroid/inference_tip.py` & `astroid-3.2.0/astroid/inference_tip.py`

 * *Files identical despite different names*

### Comparing `astroid-3.1.0/astroid/interpreter/_import/spec.py` & `astroid-3.2.0/astroid/interpreter/_import/spec.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,16 @@
 import importlib.util
 import os
 import pathlib
 import sys
 import types
 import warnings
 import zipimport
-from collections.abc import Iterator, Sequence
+from collections.abc import Iterable, Iterator, Sequence
+from functools import lru_cache
 from pathlib import Path
 from typing import Any, Literal, NamedTuple, Protocol
 
 from astroid.const import PY310_PLUS
 from astroid.modutils import EXT_LIB_DIRS
 
 from . import util
@@ -156,17 +157,22 @@
                         location=getattr(spec.loader_state, "filename", None),
                         type=ModuleType.PY_FROZEN,
                     )
             except ValueError:
                 pass
             submodule_path = sys.path
 
+        # We're looping on pyi first because if a pyi exists there's probably a reason
+        # (i.e. the code is hard or impossible to parse), so we take pyi into account
+        # But we're not quite ready to do this for numpy, see https://github.com/pylint-dev/astroid/pull/2375
+        suffixes = (".pyi", ".py", importlib.machinery.BYTECODE_SUFFIXES[0])
+        numpy_suffixes = (".py", ".pyi", importlib.machinery.BYTECODE_SUFFIXES[0])
         for entry in submodule_path:
             package_directory = os.path.join(entry, modname)
-            for suffix in (".py", ".pyi", importlib.machinery.BYTECODE_SUFFIXES[0]):
+            for suffix in numpy_suffixes if "numpy" in entry else suffixes:
                 package_file_name = "__init__" + suffix
                 file_path = os.path.join(package_directory, package_file_name)
                 if os.path.isfile(file_path):
                     return ModuleSpec(
                         name=modname,
                         location=package_directory,
                         type=ModuleType.PKG_DIRECTORY,
@@ -419,15 +425,15 @@
                     spec.submodule_search_locations,
                 ),
             )
 
     raise ImportError(f"No module named {'.'.join(module_parts)}")
 
 
-def find_spec(modpath: list[str], path: Sequence[str] | None = None) -> ModuleSpec:
+def find_spec(modpath: Iterable[str], path: Iterable[str] | None = None) -> ModuleSpec:
     """Find a spec for the given module.
 
     :type modpath: list or tuple
     :param modpath:
       split module's name (i.e name of a module or package split
       on '.'), with leading empty strings for explicit relative import
 
@@ -436,18 +442,23 @@
       optional list of path where the module or package should be
       searched (use sys.path if nothing or None is given)
 
     :rtype: ModuleSpec
     :return: A module spec, which describes how the module was
              found and where.
     """
+    return _find_spec(tuple(modpath), tuple(path) if path else None)
+
+
+@lru_cache(maxsize=1024)
+def _find_spec(module_path: tuple, path: tuple) -> ModuleSpec:
     _path = path or sys.path
 
     # Need a copy for not mutating the argument.
-    modpath = modpath[:]
+    modpath = list(module_path)
 
     submodule_path = None
     module_parts = modpath[:]
     processed: list[str] = []
 
     while modpath:
         modname = modpath.pop(0)
```

### Comparing `astroid-3.1.0/astroid/interpreter/_import/util.py` & `astroid-3.2.0/astroid/interpreter/_import/util.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,14 +8,19 @@
 import sys
 from functools import lru_cache
 from importlib._bootstrap_external import _NamespacePath
 from importlib.util import _find_spec_from_path  # type: ignore[attr-defined]
 
 from astroid.const import IS_PYPY
 
+if sys.version_info >= (3, 11):
+    from importlib.machinery import NamespaceLoader
+else:
+    from importlib._bootstrap_external import _NamespaceLoader as NamespaceLoader
+
 
 @lru_cache(maxsize=4096)
 def is_namespace(modname: str) -> bool:
     from astroid.modutils import (  # pylint: disable=import-outside-toplevel
         EXT_LIB_DIRS,
         STD_LIB_DIRS,
     )
@@ -97,8 +102,11 @@
                 return False
             last_submodule_search_locations = found_spec.submodule_search_locations
 
     return (
         found_spec is not None
         and found_spec.submodule_search_locations is not None
         and found_spec.origin is None
+        and (
+            found_spec.loader is None or isinstance(found_spec.loader, NamespaceLoader)
+        )
     )
```

### Comparing `astroid-3.1.0/astroid/interpreter/dunder_lookup.py` & `astroid-3.2.0/astroid/interpreter/dunder_lookup.py`

 * *Files identical despite different names*

### Comparing `astroid-3.1.0/astroid/interpreter/objectmodel.py` & `astroid-3.2.0/astroid/interpreter/objectmodel.py`

 * *Files identical despite different names*

### Comparing `astroid-3.1.0/astroid/manager.py` & `astroid-3.2.0/astroid/manager.py`

 * *Files 4% similar despite different names*

```diff
@@ -55,25 +55,27 @@
         "astroid_cache": {},
         "_mod_file_cache": {},
         "_failed_import_hooks": [],
         "always_load_extensions": False,
         "optimize_ast": False,
         "max_inferable_values": 100,
         "extension_package_whitelist": set(),
+        "module_denylist": set(),
         "_transform": TransformVisitor(),
     }
 
     def __init__(self) -> None:
         # NOTE: cache entries are added by the [re]builder
         self.astroid_cache = AstroidManager.brain["astroid_cache"]
         self._mod_file_cache = AstroidManager.brain["_mod_file_cache"]
         self._failed_import_hooks = AstroidManager.brain["_failed_import_hooks"]
         self.extension_package_whitelist = AstroidManager.brain[
             "extension_package_whitelist"
         ]
+        self.module_denylist = AstroidManager.brain["module_denylist"]
         self._transform = AstroidManager.brain["_transform"]
 
     @property
     def always_load_extensions(self) -> bool:
         return AstroidManager.brain["always_load_extensions"]
 
     @always_load_extensions.setter
@@ -196,14 +198,16 @@
         """Given a module name, return the astroid object."""
         if modname is None:
             raise AstroidBuildingError("No module name given.")
         # Sometimes we don't want to use the cache. For example, when we're
         # importing a module with the same name as the file that is importing
         # we want to fallback on the import system to make sure we get the correct
         # module.
+        if modname in self.module_denylist:
+            raise AstroidImportError(f"Skipping ignored module {modname!r}")
         if modname in self.astroid_cache and use_cache:
             return self.astroid_cache[modname]
         if modname == "__main__":
             return self._build_stub_module(modname)
         if context_file:
             old_cwd = os.getcwd()
             os.chdir(os.path.dirname(context_file))
@@ -301,15 +305,14 @@
             value = self._mod_file_cache[(modname, contextfile)]
         except KeyError:
             try:
                 value = file_info_from_modpath(
                     modname.split("."), context_file=contextfile
                 )
             except ImportError as e:
-                # pylint: disable-next=redefined-variable-type
                 value = AstroidImportError(
                     "Failed to import module {modname} with error:\n{error}.",
                     modname=modname,
                     # we remove the traceback here to save on memory usage (since these exceptions are cached)
                     error=e.with_traceback(None),
                 )
             self._mod_file_cache[(modname, contextfile)] = value
@@ -398,16 +401,15 @@
                 "Unexpected error while retrieving name for {class_repr}:\n{error}",
                 cls=klass,
                 class_repr=safe_repr(klass),
             ) from exc
         # take care, on living object __module__ is regularly wrong :(
         modastroid = self.ast_from_module_name(modname)
         if klass is obj:
-            for inferred in modastroid.igetattr(name, context):
-                yield inferred
+            yield from modastroid.igetattr(name, context)
         else:
             for inferred in modastroid.igetattr(name, context):
                 yield inferred.instantiate_class()
 
     def register_failed_import_hook(self, hook: Callable[[str], nodes.Module]) -> None:
         """Registers a hook to resolve imports that cannot be found otherwise.
 
@@ -436,14 +438,15 @@
         """Clear the underlying caches, bootstrap the builtins module and
         re-register transforms.
         """
         # import here because of cyclic imports
         # pylint: disable=import-outside-toplevel
         from astroid.brain.helpers import register_all_brains
         from astroid.inference_tip import clear_inference_tip_cache
+        from astroid.interpreter._import.spec import _find_spec
         from astroid.interpreter.objectmodel import ObjectModel
         from astroid.nodes._base_nodes import LookupMixIn
         from astroid.nodes.scoped_nodes import ClassDef
 
         clear_inference_tip_cache()
         _invalidate_cache()  # inference context cache
 
@@ -453,14 +456,15 @@
 
         for lru_cache in (
             LookupMixIn.lookup,
             _cache_normalize_path_,
             util.is_namespace,
             ObjectModel.attributes,
             ClassDef._metaclass_lookup_attribute,
+            _find_spec,
         ):
             lru_cache.cache_clear()  # type: ignore[attr-defined]
 
         self.bootstrap()
 
         # Reload brain plugins. During initialisation this is done in astroid.manager.py
         register_all_brains(self)
```

### Comparing `astroid-3.1.0/astroid/modutils.py` & `astroid-3.2.0/astroid/modutils.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,18 +40,18 @@
 else:
     from astroid._backport_stdlib_names import stdlib_module_names
 
 logger = logging.getLogger(__name__)
 
 
 if sys.platform.startswith("win"):
-    PY_SOURCE_EXTS = ("py", "pyw", "pyi")
+    PY_SOURCE_EXTS = ("pyi", "pyw", "py")
     PY_COMPILED_EXTS = ("dll", "pyd")
 else:
-    PY_SOURCE_EXTS = ("py", "pyi")
+    PY_SOURCE_EXTS = ("pyi", "py")
     PY_COMPILED_EXTS = ("so",)
 
 
 # TODO: Adding `platstdlib` is a fix for a workaround in virtualenv. At some point we should
 # revisit whether this is still necessary. See https://github.com/pylint-dev/astroid/pull/1323.
 STD_LIB_DIRS = {sysconfig.get_path("stdlib"), sysconfig.get_path("platstdlib")}
 
@@ -495,15 +495,15 @@
 
     :return: the absolute path of the source file if it exists
     """
     filename = os.path.abspath(_path_from_filename(filename))
     base, orig_ext = os.path.splitext(filename)
     if orig_ext == ".pyi" and os.path.exists(f"{base}{orig_ext}"):
         return f"{base}{orig_ext}"
-    for ext in PY_SOURCE_EXTS:
+    for ext in PY_SOURCE_EXTS if "numpy" not in filename else reversed(PY_SOURCE_EXTS):
         source_path = f"{base}.{ext}"
         if os.path.exists(source_path):
             return source_path
     if include_no_ext and not orig_ext and os.path.exists(base):
         return base
     raise NoSourceFile(filename)
 
@@ -667,15 +667,16 @@
 
 
 def _has_init(directory: str) -> str | None:
     """If the given directory has a valid __init__ file, return its path,
     else return None.
     """
     mod_or_pack = os.path.join(directory, "__init__")
-    for ext in (*PY_SOURCE_EXTS, "pyc", "pyo"):
+    exts = reversed(PY_SOURCE_EXTS) if "numpy" in directory else PY_SOURCE_EXTS
+    for ext in (*exts, "pyc", "pyo"):
         if os.path.exists(mod_or_pack + "." + ext):
             return mod_or_pack + "." + ext
     return None
 
 
 def is_namespace(specobj: spec.ModuleSpec) -> bool:
     return specobj.type == spec.ModuleType.PY_NAMESPACE
```

### Comparing `astroid-3.1.0/astroid/nodes/__init__.py` & `astroid-3.2.0/astroid/nodes/__init__.py`

 * *Files identical despite different names*

### Comparing `astroid-3.1.0/astroid/nodes/_base_nodes.py` & `astroid-3.2.0/astroid/nodes/_base_nodes.py`

 * *Files identical despite different names*

### Comparing `astroid-3.1.0/astroid/nodes/as_string.py` & `astroid-3.2.0/astroid/nodes/as_string.py`

 * *Files identical despite different names*

### Comparing `astroid-3.1.0/astroid/nodes/const.py` & `astroid-3.2.0/astroid/nodes/const.py`

 * *Files identical despite different names*

### Comparing `astroid-3.1.0/astroid/nodes/node_classes.py` & `astroid-3.2.0/astroid/nodes/node_classes.py`

 * *Files identical despite different names*

### Comparing `astroid-3.1.0/astroid/nodes/node_ng.py` & `astroid-3.2.0/astroid/nodes/node_ng.py`

 * *Files identical despite different names*

### Comparing `astroid-3.1.0/astroid/nodes/scoped_nodes/__init__.py` & `astroid-3.2.0/astroid/nodes/scoped_nodes/__init__.py`

 * *Files identical despite different names*

### Comparing `astroid-3.1.0/astroid/nodes/scoped_nodes/mixin.py` & `astroid-3.2.0/astroid/nodes/scoped_nodes/mixin.py`

 * *Files identical despite different names*

### Comparing `astroid-3.1.0/astroid/nodes/scoped_nodes/scoped_nodes.py` & `astroid-3.2.0/astroid/nodes/scoped_nodes/scoped_nodes.py`

 * *Files 1% similar despite different names*

```diff
@@ -2504,20 +2504,29 @@
         try:
             attributes = self.getattr(name, context, class_context=class_context)
             # If we have more than one attribute, make sure that those starting from
             # the second one are from the same scope. This is to account for modifications
             # to the attribute happening *after* the attribute's definition (e.g. AugAssigns on lists)
             if len(attributes) > 1:
                 first_attr, attributes = attributes[0], attributes[1:]
-                first_scope = first_attr.scope()
+                first_scope = first_attr.parent.scope()
                 attributes = [first_attr] + [
                     attr
                     for attr in attributes
                     if attr.parent and attr.parent.scope() == first_scope
                 ]
+            functions = [attr for attr in attributes if isinstance(attr, FunctionDef)]
+            if functions:
+                # Prefer only the last function, unless a property is involved.
+                last_function = functions[-1]
+                attributes = [
+                    a
+                    for a in attributes
+                    if a not in functions or a is last_function or bases._is_property(a)
+                ]
 
             for inferred in bases._infer_stmts(attributes, context, frame=self):
                 # yield Uninferable object instead of descriptors when necessary
                 if not isinstance(inferred, node_classes.Const) and isinstance(
                     inferred, bases.Instance
                 ):
                     try:
```

### Comparing `astroid-3.1.0/astroid/nodes/scoped_nodes/utils.py` & `astroid-3.2.0/astroid/nodes/scoped_nodes/utils.py`

 * *Files identical despite different names*

### Comparing `astroid-3.1.0/astroid/objects.py` & `astroid-3.2.0/astroid/objects.py`

 * *Files identical despite different names*

### Comparing `astroid-3.1.0/astroid/protocols.py` & `astroid-3.2.0/astroid/protocols.py`

 * *Files identical despite different names*

### Comparing `astroid-3.1.0/astroid/raw_building.py` & `astroid-3.2.0/astroid/raw_building.py`

 * *Files identical despite different names*

### Comparing `astroid-3.1.0/astroid/rebuilder.py` & `astroid-3.2.0/astroid/rebuilder.py`

 * *Files identical despite different names*

### Comparing `astroid-3.1.0/astroid/test_utils.py` & `astroid-3.2.0/astroid/test_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -70,8 +70,9 @@
     # with other tests :
     m.__dict__ = {}
     m._failed_import_hooks = []
     m.astroid_cache = {}
     m._mod_file_cache = {}
     m._transform = transforms.TransformVisitor()
     m.extension_package_whitelist = set()
+    m.module_denylist = set()
     return m
```

### Comparing `astroid-3.1.0/astroid/transforms.py` & `astroid-3.2.0/astroid/transforms.py`

 * *Files identical despite different names*

### Comparing `astroid-3.1.0/astroid/typing.py` & `astroid-3.2.0/astroid/typing.py`

 * *Files identical despite different names*

### Comparing `astroid-3.1.0/astroid/util.py` & `astroid-3.2.0/astroid/util.py`

 * *Files identical despite different names*

### Comparing `astroid-3.1.0/astroid.egg-info/PKG-INFO` & `astroid-3.2.0/astroid.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: astroid
-Version: 3.1.0
+Version: 3.2.0
 Summary: An abstract syntax tree for Python with inference support.
 License: LGPL-2.1-or-later
 Project-URL: Docs, https://pylint.readthedocs.io/projects/astroid/en/latest/
 Project-URL: Source Code, https://github.com/pylint-dev/astroid
 Project-URL: Bug tracker, https://github.com/pylint-dev/astroid/issues
 Project-URL: Discord server, https://discord.gg/Egy6P8AMB5
 Keywords: static code analysis,python,abstract syntax tree
```

### Comparing `astroid-3.1.0/astroid.egg-info/SOURCES.txt` & `astroid-3.2.0/astroid.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `astroid-3.1.0/pyproject.toml` & `astroid-3.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `astroid-3.1.0/tests/brain/numpy/test_core_einsumfunc.py` & `astroid-3.2.0/tests/brain/numpy/test_core_einsumfunc.py`

 * *Files identical despite different names*

### Comparing `astroid-3.1.0/tests/brain/numpy/test_core_fromnumeric.py` & `astroid-3.2.0/tests/brain/numpy/test_core_fromnumeric.py`

 * *Files identical despite different names*

### Comparing `astroid-3.1.0/tests/brain/numpy/test_core_function_base.py` & `astroid-3.2.0/tests/brain/numpy/test_core_function_base.py`

 * *Files identical despite different names*

### Comparing `astroid-3.1.0/tests/brain/numpy/test_core_multiarray.py` & `astroid-3.2.0/tests/brain/numpy/test_core_multiarray.py`

 * *Files identical despite different names*

### Comparing `astroid-3.1.0/tests/brain/numpy/test_core_numeric.py` & `astroid-3.2.0/tests/brain/numpy/test_core_numeric.py`

 * *Files identical despite different names*

### Comparing `astroid-3.1.0/tests/brain/numpy/test_core_numerictypes.py` & `astroid-3.2.0/tests/brain/numpy/test_core_numerictypes.py`

 * *Files identical despite different names*

### Comparing `astroid-3.1.0/tests/brain/numpy/test_core_umath.py` & `astroid-3.2.0/tests/brain/numpy/test_core_umath.py`

 * *Files identical despite different names*

### Comparing `astroid-3.1.0/tests/brain/numpy/test_ma.py` & `astroid-3.2.0/tests/brain/numpy/test_ma.py`

 * *Files identical despite different names*

### Comparing `astroid-3.1.0/tests/brain/numpy/test_ndarray.py` & `astroid-3.2.0/tests/brain/numpy/test_ndarray.py`

 * *Files identical despite different names*

### Comparing `astroid-3.1.0/tests/brain/numpy/test_random_mtrand.py` & `astroid-3.2.0/tests/brain/numpy/test_random_mtrand.py`

 * *Files identical despite different names*

### Comparing `astroid-3.1.0/tests/brain/test_argparse.py` & `astroid-3.2.0/tests/brain/test_argparse.py`

 * *Files identical despite different names*

### Comparing `astroid-3.1.0/tests/brain/test_attr.py` & `astroid-3.2.0/tests/brain/test_attr.py`

 * *Files 3% similar despite different names*

```diff
@@ -86,15 +86,15 @@
         for name in ("f", "g", "h", "i", "j", "k", "l", "m"):
             should_be_unknown = next(module.getattr(name)[0].infer()).getattr("d")[0]
             self.assertIsInstance(should_be_unknown, astroid.Unknown)
 
     def test_attrs_transform(self) -> None:
         """Test brain for decorators of the 'attrs' package.
 
-        Package added support for 'attrs' a long side 'attr' in v21.3.0.
+        Package added support for 'attrs' alongside 'attr' in v21.3.0.
         See: https://github.com/python-attrs/attrs/releases/tag/21.3.0
         """
         module = astroid.parse(
             """
         import attrs
         from attrs import field, mutable, frozen, define
         from attrs import mutable as my_mutable
@@ -149,44 +149,20 @@
         l = Eggs(d=1)
         l.d['answer'] = 42
 
 
         @frozen
         class Legs:
             d = attrs.field(default=attrs.Factory(dict))
-
-        m = Legs(d=1)
-        m.d['answer'] = 42
-
-        @define
-        class FooBar:
-            d = attrs.field(default=attrs.Factory(dict))
-
-        n = FooBar(d=1)
-        n.d['answer'] = 42
-
-        @mutable
-        class BarFoo:
-            d = attrs.field(default=attrs.Factory(dict))
-
-        o = BarFoo(d=1)
-        o.d['answer'] = 42
-
-        @my_mutable
-        class FooFoo:
-            d = attrs.field(default=attrs.Factory(dict))
-
-        p = FooFoo(d=1)
-        p.d['answer'] = 42
         """
         )
 
-        for name in ("f", "g", "h", "i", "j", "k", "l", "m", "n", "o", "p"):
+        for name in ("f", "g", "h", "i", "j", "k", "l"):
             should_be_unknown = next(module.getattr(name)[0].infer()).getattr("d")[0]
-            self.assertIsInstance(should_be_unknown, astroid.Unknown)
+            self.assertIsInstance(should_be_unknown, astroid.Unknown, name)
 
     def test_special_attributes(self) -> None:
         """Make sure special attrs attributes exist"""
 
         code = """
         import attr
```

### Comparing `astroid-3.1.0/tests/brain/test_brain.py` & `astroid-3.2.0/tests/brain/test_brain.py`

 * *Files identical despite different names*

### Comparing `astroid-3.1.0/tests/brain/test_builtin.py` & `astroid-3.2.0/tests/brain/test_builtin.py`

 * *Files identical despite different names*

### Comparing `astroid-3.1.0/tests/brain/test_ctypes.py` & `astroid-3.2.0/tests/brain/test_ctypes.py`

 * *Files identical despite different names*

### Comparing `astroid-3.1.0/tests/brain/test_dataclasses.py` & `astroid-3.2.0/tests/brain/test_dataclasses.py`

 * *Files identical despite different names*

### Comparing `astroid-3.1.0/tests/brain/test_dateutil.py` & `astroid-3.2.0/tests/brain/test_dateutil.py`

 * *Files identical despite different names*

### Comparing `astroid-3.1.0/tests/brain/test_enum.py` & `astroid-3.2.0/tests/brain/test_enum.py`

 * *Files identical despite different names*

### Comparing `astroid-3.1.0/tests/brain/test_hashlib.py` & `astroid-3.2.0/tests/brain/test_hashlib.py`

 * *Files identical despite different names*

### Comparing `astroid-3.1.0/tests/brain/test_multiprocessing.py` & `astroid-3.2.0/tests/brain/test_multiprocessing.py`

 * *Files identical despite different names*

### Comparing `astroid-3.1.0/tests/brain/test_named_tuple.py` & `astroid-3.2.0/tests/brain/test_named_tuple.py`

 * *Files identical despite different names*

### Comparing `astroid-3.1.0/tests/brain/test_nose.py` & `astroid-3.2.0/tests/brain/test_nose.py`

 * *Files identical despite different names*

### Comparing `astroid-3.1.0/tests/brain/test_pathlib.py` & `astroid-3.2.0/tests/brain/test_pathlib.py`

 * *Files identical despite different names*

### Comparing `astroid-3.1.0/tests/brain/test_pytest.py` & `astroid-3.2.0/tests/brain/test_pytest.py`

 * *Files identical despite different names*

### Comparing `astroid-3.1.0/tests/brain/test_qt.py` & `astroid-3.2.0/tests/brain/test_qt.py`

 * *Files identical despite different names*

### Comparing `astroid-3.1.0/tests/brain/test_regex.py` & `astroid-3.2.0/tests/brain/test_regex.py`

 * *Files identical despite different names*

### Comparing `astroid-3.1.0/tests/brain/test_signal.py` & `astroid-3.2.0/tests/brain/test_signal.py`

 * *Files identical despite different names*

### Comparing `astroid-3.1.0/tests/brain/test_six.py` & `astroid-3.2.0/tests/brain/test_six.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,14 +25,16 @@
         ast_nodes = builder.extract_node(
             """
         import six
         six.moves.http_client #@
         six.moves.urllib_parse #@
         six.moves.urllib_error #@
         six.moves.urllib.request #@
+        from six.moves import StringIO
+        StringIO #@
         """
         )
         assert isinstance(ast_nodes, list)
         http_client = next(ast_nodes[0].infer())
         self.assertIsInstance(http_client, nodes.Module)
         self.assertEqual(http_client.name, "http.client")
 
@@ -60,14 +62,26 @@
         urlopen = next(urllib_request.igetattr("urlopen"))
         urlretrieve = next(urllib_request.igetattr("urlretrieve"))
         self.assertIsInstance(urlopen, nodes.FunctionDef)
         self.assertEqual(urlopen.qname(), "urllib.request.urlopen")
         self.assertIsInstance(urlretrieve, nodes.FunctionDef)
         self.assertEqual(urlretrieve.qname(), "urllib.request.urlretrieve")
 
+        StringIO = next(ast_nodes[4].infer())
+        self.assertIsInstance(StringIO, nodes.ClassDef)
+        self.assertEqual(StringIO.qname(), "_io.StringIO")
+        self.assertTrue(StringIO.callable())
+
+    def test_attribute_access_with_six_moves_imported(self) -> None:
+        astroid.MANAGER.clear_cache()
+        astroid.MANAGER._mod_file_cache.clear()
+        import six.moves  # type: ignore[import]  # pylint: disable=import-outside-toplevel,unused-import,redefined-outer-name
+
+        self.test_attribute_access()
+
     def test_from_imports(self) -> None:
         ast_node = builder.extract_node(
             """
         from six.moves import http_client
         http_client.HTTPSConnection #@
         """
         )
```

### Comparing `astroid-3.1.0/tests/brain/test_ssl.py` & `astroid-3.2.0/tests/brain/test_ssl.py`

 * *Files identical despite different names*

### Comparing `astroid-3.1.0/tests/brain/test_threading.py` & `astroid-3.2.0/tests/brain/test_threading.py`

 * *Files identical despite different names*

### Comparing `astroid-3.1.0/tests/brain/test_typing.py` & `astroid-3.2.0/tests/brain/test_typing.py`

 * *Files identical despite different names*

### Comparing `astroid-3.1.0/tests/brain/test_typing_extensions.py` & `astroid-3.2.0/tests/brain/test_typing_extensions.py`

 * *Files identical despite different names*

### Comparing `astroid-3.1.0/tests/brain/test_unittest.py` & `astroid-3.2.0/tests/brain/test_unittest.py`

 * *Files identical despite different names*

### Comparing `astroid-3.1.0/tests/test_builder.py` & `astroid-3.2.0/tests/test_builder.py`

 * *Files identical despite different names*

### Comparing `astroid-3.1.0/tests/test_constraint.py` & `astroid-3.2.0/tests/test_constraint.py`

 * *Files identical despite different names*

### Comparing `astroid-3.1.0/tests/test_decorators.py` & `astroid-3.2.0/tests/test_decorators.py`

 * *Files identical despite different names*

### Comparing `astroid-3.1.0/tests/test_filter_statements.py` & `astroid-3.2.0/tests/test_filter_statements.py`

 * *Files identical despite different names*

### Comparing `astroid-3.1.0/tests/test_group_exceptions.py` & `astroid-3.2.0/tests/test_group_exceptions.py`

 * *Files identical despite different names*

### Comparing `astroid-3.1.0/tests/test_helpers.py` & `astroid-3.2.0/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `astroid-3.1.0/tests/test_inference.py` & `astroid-3.2.0/tests/test_inference.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     nodes,
     objects,
     test_utils,
     util,
 )
 from astroid import decorators as decoratorsmod
 from astroid.arguments import CallSite
-from astroid.bases import BoundMethod, Instance, UnboundMethod, UnionType
+from astroid.bases import BoundMethod, Generator, Instance, UnboundMethod, UnionType
 from astroid.builder import AstroidBuilder, _extract_single_node, extract_node, parse
 from astroid.const import IS_PYPY, PY39_PLUS, PY310_PLUS, PY312_PLUS
 from astroid.context import CallContext, InferenceContext
 from astroid.exceptions import (
     AstroidTypeError,
     AttributeInferenceError,
     InferenceError,
@@ -4317,14 +4317,61 @@
         # possible to infer the subscript directly. It is the difference
         # between these two cases that led to the discovery of the cause of the
         # bug in https://github.com/pylint-dev/astroid/issues/904
         inferred = next(attr_node.infer())
         assert isinstance(inferred, nodes.Const)
         assert inferred.value == 123
 
+    def test_infer_method_empty_body(self) -> None:
+        # https://github.com/PyCQA/astroid/issues/1015
+        node = extract_node(
+            """
+            class A:
+                def foo(self): ...
+
+            A().foo()  #@
+        """
+        )
+        inferred = next(node.infer())
+        assert isinstance(inferred, nodes.Const)
+        assert inferred.value is None
+
+    def test_infer_method_overload(self) -> None:
+        # https://github.com/PyCQA/astroid/issues/1015
+        node = extract_node(
+            """
+            class A:
+                def foo(self): ...
+
+                def foo(self):
+                    yield
+
+            A().foo()  #@
+        """
+        )
+        inferred = list(node.infer())
+        assert len(inferred) == 1
+        assert isinstance(inferred[0], Generator)
+
+    def test_infer_function_under_if(self) -> None:
+        node = extract_node(
+            """
+        if 1 in [1]:
+            def func():
+                return 42
+        else:
+            def func():
+                return False
+
+        func()  #@
+        """
+        )
+        inferred = list(node.inferred())
+        assert [const.value for const in inferred] == [42, False]
+
     def test_delayed_attributes_without_slots(self) -> None:
         ast_node = extract_node(
             """
         class A(object):
             __slots__ = ('a', )
         a = A()
         a.teta = 24
```

### Comparing `astroid-3.1.0/tests/test_inference_calls.py` & `astroid-3.2.0/tests/test_inference_calls.py`

 * *Files identical despite different names*

### Comparing `astroid-3.1.0/tests/test_lookup.py` & `astroid-3.2.0/tests/test_lookup.py`

 * *Files identical despite different names*

### Comparing `astroid-3.1.0/tests/test_manager.py` & `astroid-3.2.0/tests/test_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,20 +32,19 @@
 
 def _get_file_from_object(obj) -> str:
     if IS_JYTHON:
         return obj.__file__.split("$py.class")[0] + ".py"
     return obj.__file__
 
 
-class AstroidManagerTest(
-    resources.SysPathSetup, resources.AstroidCacheSetupMixin, unittest.TestCase
-):
+class AstroidManagerTest(resources.SysPathSetup, unittest.TestCase):
     def setUp(self) -> None:
         super().setUp()
         self.manager = test_utils.brainless_manager()
+        self.manager.clear_cache()
 
     def test_ast_from_file(self) -> None:
         filepath = unittest.__file__
         ast = self.manager.ast_from_file(filepath)
         self.assertEqual(ast.name, "unittest")
         self.assertIn("unittest", self.manager.astroid_cache)
 
@@ -379,18 +378,26 @@
         stdlib_math = next(module.body[1].value.args[0].infer())
         assert self.manager.astroid_cache["math"] != stdlib_math
 
     def test_raises_exception_for_empty_modname(self) -> None:
         with pytest.raises(AstroidBuildingError):
             self.manager.ast_from_module_name(None)
 
+    def test_denied_modules_raise(self) -> None:
+        self.manager.module_denylist.add("random")
+        with pytest.raises(AstroidImportError, match="random"):
+            self.manager.ast_from_module_name("random")
+        # and module not in the deny list shouldn't raise
+        self.manager.ast_from_module_name("math")
 
-class IsolatedAstroidManagerTest(resources.AstroidCacheSetupMixin, unittest.TestCase):
+
+class IsolatedAstroidManagerTest(unittest.TestCase):
     def test_no_user_warning(self):
         mgr = manager.AstroidManager()
+        self.addCleanup(mgr.clear_cache)
         with warnings.catch_warnings():
             warnings.filterwarnings("error", category=UserWarning)
             mgr.ast_from_module_name("setuptools")
             mgr.ast_from_module_name("pip")
 
 
 class BorgAstroidManagerTC(unittest.TestCase):
```

### Comparing `astroid-3.1.0/tests/test_modutils.py` & `astroid-3.2.0/tests/test_modutils.py`

 * *Files 0% similar despite different names*

```diff
@@ -37,14 +37,15 @@
     return modutils._path_from_filename(obj.__file__)
 
 
 class ModuleFileTest(unittest.TestCase):
     package = "mypypa"
 
     def tearDown(self) -> None:
+        astroid.MANAGER.clear_cache()
         for k in list(sys.path_importer_cache):
             if "MyPyPa" in k:
                 del sys.path_importer_cache[k]
 
     def test_find_zipped_module(self) -> None:
         found_spec = spec.find_spec(
             [self.package], [resources.find("data/MyPyPa-0.1.0-py2.5.zip")]
@@ -286,19 +287,26 @@
         self.assertEqual(
             modutils.get_source_file(os.path.__file__), os.path.normpath(filename)
         )
 
     def test_raise(self) -> None:
         self.assertRaises(modutils.NoSourceFile, modutils.get_source_file, "whatever")
 
-    def test_(self) -> None:
+    def test_pyi(self) -> None:
         package = resources.find("pyi_data")
         module = os.path.join(package, "__init__.pyi")
         self.assertEqual(modutils.get_source_file(module), os.path.normpath(module))
 
+    def test_pyi_preferred(self) -> None:
+        package = resources.find("pyi_data/find_test")
+        module = os.path.join(package, "__init__.py")
+        self.assertEqual(
+            modutils.get_source_file(module), os.path.normpath(module) + "i"
+        )
+
 
 class IsStandardModuleTest(resources.SysPathSetup, unittest.TestCase):
     """
     Return true if the module may be considered as a module from the standard
     library.
     """
```

### Comparing `astroid-3.1.0/tests/test_nodes.py` & `astroid-3.2.0/tests/test_nodes.py`

 * *Files identical despite different names*

### Comparing `astroid-3.1.0/tests/test_nodes_lineno.py` & `astroid-3.2.0/tests/test_nodes_lineno.py`

 * *Files identical despite different names*

### Comparing `astroid-3.1.0/tests/test_nodes_position.py` & `astroid-3.2.0/tests/test_nodes_position.py`

 * *Files identical despite different names*

### Comparing `astroid-3.1.0/tests/test_object_model.py` & `astroid-3.2.0/tests/test_object_model.py`

 * *Files identical despite different names*

### Comparing `astroid-3.1.0/tests/test_objects.py` & `astroid-3.2.0/tests/test_objects.py`

 * *Files identical despite different names*

### Comparing `astroid-3.1.0/tests/test_protocols.py` & `astroid-3.2.0/tests/test_protocols.py`

 * *Files identical despite different names*

### Comparing `astroid-3.1.0/tests/test_python3.py` & `astroid-3.2.0/tests/test_python3.py`

 * *Files identical despite different names*

### Comparing `astroid-3.1.0/tests/test_raw_building.py` & `astroid-3.2.0/tests/test_raw_building.py`

 * *Files identical despite different names*

### Comparing `astroid-3.1.0/tests/test_regrtest.py` & `astroid-3.2.0/tests/test_regrtest.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,18 +22,19 @@
     import numpy  # pylint: disable=unused-import
 except ImportError:
     HAS_NUMPY = False
 else:
     HAS_NUMPY = True
 
 
-class NonRegressionTests(resources.AstroidCacheSetupMixin, unittest.TestCase):
+class NonRegressionTests(unittest.TestCase):
     def setUp(self) -> None:
         sys.path.insert(0, resources.find("data"))
         MANAGER.always_load_extensions = True
+        self.addCleanup(MANAGER.clear_cache)
 
     def tearDown(self) -> None:
         MANAGER.always_load_extensions = False
         sys.path.pop(0)
         sys.path_importer_cache.pop(resources.find("data"), None)
 
     def test_manager_instance_attributes_reference_global_MANAGER(self) -> None:
```

### Comparing `astroid-3.1.0/tests/test_scoped_nodes.py` & `astroid-3.2.0/tests/test_scoped_nodes.py`

 * *Files identical despite different names*

### Comparing `astroid-3.1.0/tests/test_stdlib.py` & `astroid-3.2.0/tests/test_stdlib.py`

 * *Files identical despite different names*

### Comparing `astroid-3.1.0/tests/test_transforms.py` & `astroid-3.2.0/tests/test_transforms.py`

 * *Files identical despite different names*

### Comparing `astroid-3.1.0/tests/test_type_params.py` & `astroid-3.2.0/tests/test_type_params.py`

 * *Files identical despite different names*

### Comparing `astroid-3.1.0/tests/test_utils.py` & `astroid-3.2.0/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `astroid-3.1.0/tests/testdata/python3/data/MyPyPa-0.1.0-py2.5.egg` & `astroid-3.2.0/tests/testdata/python3/data/MyPyPa-0.1.0-py2.5.egg`

 * *Files identical despite different names*

### Comparing `astroid-3.1.0/tests/testdata/python3/data/MyPyPa-0.1.0-py2.5.zip` & `astroid-3.2.0/tests/testdata/python3/data/MyPyPa-0.1.0-py2.5.zip`

 * *Files identical despite different names*

### Comparing `astroid-3.1.0/tests/testdata/python3/data/fake_module_with_warnings.py` & `astroid-3.2.0/tests/testdata/python3/data/fake_module_with_warnings.py`

 * *Files identical despite different names*

### Comparing `astroid-3.1.0/tests/testdata/python3/data/foogle_fax-0.12.5-py2.7-nspkg.pth` & `astroid-3.2.0/tests/testdata/python3/data/foogle_fax-0.12.5-py2.7-nspkg.pth`

 * *Files identical despite different names*

### Comparing `astroid-3.1.0/tests/testdata/python3/data/import_setuptools_pep660/__editable___example_0_1_0_finder.py` & `astroid-3.2.0/tests/testdata/python3/data/import_setuptools_pep660/__editable___example_0_1_0_finder.py`

 * *Files identical despite different names*

### Comparing `astroid-3.1.0/tests/testdata/python3/data/max_inferable_limit_for_classes/main.py` & `astroid-3.2.0/tests/testdata/python3/data/max_inferable_limit_for_classes/main.py`

 * *Files identical despite different names*

### Comparing `astroid-3.1.0/tests/testdata/python3/data/max_inferable_limit_for_classes/nodes/roles.py` & `astroid-3.2.0/tests/testdata/python3/data/max_inferable_limit_for_classes/nodes/roles.py`

 * *Files identical despite different names*

### Comparing `astroid-3.1.0/tests/testdata/python3/data/metaclass_recursion/monkeypatch.py` & `astroid-3.2.0/tests/testdata/python3/data/metaclass_recursion/monkeypatch.py`

 * *Files identical despite different names*

### Comparing `astroid-3.1.0/tests/testdata/python3/data/module.py` & `astroid-3.2.0/tests/testdata/python3/data/module.py`

 * *Files identical despite different names*

### Comparing `astroid-3.1.0/tests/testdata/python3/data/module2.py` & `astroid-3.2.0/tests/testdata/python3/data/module2.py`

 * *Files identical despite different names*

### Comparing `astroid-3.1.0/tests/testdata/python3/data/nonregr.py` & `astroid-3.2.0/tests/testdata/python3/data/nonregr.py`

 * *Files identical despite different names*

### Comparing `astroid-3.1.0/tests/testdata/python3/data/operator_precedence.py` & `astroid-3.2.0/tests/testdata/python3/data/operator_precedence.py`

 * *Files identical despite different names*

### Comparing `astroid-3.1.0/tests/testdata/python3/data/package/import_package_subpackage_module.py` & `astroid-3.2.0/tests/testdata/python3/data/package/import_package_subpackage_module.py`

 * *Files identical despite different names*

### Comparing `astroid-3.1.0/tests/testdata/python3/recursion_error.py` & `astroid-3.2.0/tests/testdata/python3/recursion_error.py`

 * *Files identical despite different names*
