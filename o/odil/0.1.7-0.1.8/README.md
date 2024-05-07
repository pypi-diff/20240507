# Comparing `tmp/odil-0.1.7.tar.gz` & `tmp/odil-0.1.8.tar.gz`

## Comparing `odil-0.1.7.tar` & `odil-0.1.8.tar`

### file list

```diff
@@ -1,58 +1,58 @@
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 odil-0.1.7/.style.yapf
--rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 odil-0.1.7/Makefile
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 odil-0.1.7/setup.cfg
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 odil-0.1.7/examples/.gitignore
--rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 odil-0.1.7/examples/README.md
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 odil-0.1.7/examples/basic/README.md
--rwxr-xr-x   0        0        0      753 2020-02-02 00:00:00.000000 odil-0.1.7/examples/basic/README.py
--rw-r--r--   0        0        0     6436 2020-02-02 00:00:00.000000 odil-0.1.7/examples/basic/fields.ipynb
--rwxr-xr-x   0        0        0     4449 2020-02-02 00:00:00.000000 odil-0.1.7/examples/basic/fields.py
--rw-r--r--   0        0        0     2233 2020-02-02 00:00:00.000000 odil-0.1.7/examples/heat/README.md
--rwxr-xr-x   0        0        0     1540 2020-02-02 00:00:00.000000 odil-0.1.7/examples/heat/README.py
--rwxr-xr-x   0        0        0    20973 2020-02-02 00:00:00.000000 odil-0.1.7/examples/heat/heat.py
--rwxr-xr-x   0        0        0     1657 2020-02-02 00:00:00.000000 odil-0.1.7/examples/heat/plot_train.py
--rwxr-xr-x   0        0        0     1909 2020-02-02 00:00:00.000000 odil-0.1.7/examples/heat/run
--rwxr-xr-x   0        0        0      369 2020-02-02 00:00:00.000000 odil-0.1.7/examples/heat/run_all
--rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 odil-0.1.7/examples/infer_constant/README.md
--rwxr-xr-x   0        0        0      785 2020-02-02 00:00:00.000000 odil-0.1.7/examples/infer_constant/README.py
--rwxr-xr-x   0        0        0     5972 2020-02-02 00:00:00.000000 odil-0.1.7/examples/infer_constant/infer_constant.py
--rw-r--r--   0        0        0      600 2020-02-02 00:00:00.000000 odil-0.1.7/examples/poisson/README.md
--rwxr-xr-x   0        0        0      729 2020-02-02 00:00:00.000000 odil-0.1.7/examples/poisson/README.py
--rwxr-xr-x   0        0        0     1415 2020-02-02 00:00:00.000000 odil-0.1.7/examples/poisson/plot_field.py
--rwxr-xr-x   0        0        0     1079 2020-02-02 00:00:00.000000 odil-0.1.7/examples/poisson/plot_train.py
--rwxr-xr-x   0        0        0     9851 2020-02-02 00:00:00.000000 odil-0.1.7/examples/poisson/poisson.py
--rwxr-xr-x   0        0        0      497 2020-02-02 00:00:00.000000 odil-0.1.7/examples/poisson/run
--rw-r--r--   0        0        0      659 2020-02-02 00:00:00.000000 odil-0.1.7/examples/velocity_from_tracer/README.md
--rwxr-xr-x   0        0        0      778 2020-02-02 00:00:00.000000 odil-0.1.7/examples/velocity_from_tracer/README.py
--rwxr-xr-x   0        0        0     8799 2020-02-02 00:00:00.000000 odil-0.1.7/examples/velocity_from_tracer/veltracer.py
--rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 odil-0.1.7/src/.gitignore
--rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 odil-0.1.7/src/odil/.gitignore
--rw-r--r--   0        0        0      980 2020-02-02 00:00:00.000000 odil-0.1.7/src/odil/__init__.py
--rw-r--r--   0        0        0    11735 2020-02-02 00:00:00.000000 odil-0.1.7/src/odil/backend.py
--rw-r--r--   0        0        0     2345 2020-02-02 00:00:00.000000 odil-0.1.7/src/odil/cache.py
--rw-r--r--   0        0        0    61549 2020-02-02 00:00:00.000000 odil-0.1.7/src/odil/core.py
--rw-r--r--   0        0        0     2766 2020-02-02 00:00:00.000000 odil-0.1.7/src/odil/core_min.py
--rw-r--r--   0        0        0     3660 2020-02-02 00:00:00.000000 odil-0.1.7/src/odil/history.py
--rw-r--r--   0        0        0     7985 2020-02-02 00:00:00.000000 odil-0.1.7/src/odil/io.py
--rw-r--r--   0        0        0     6482 2020-02-02 00:00:00.000000 odil-0.1.7/src/odil/linsolver.py
--rw-r--r--   0        0        0      787 2020-02-02 00:00:00.000000 odil-0.1.7/src/odil/odil.mplstyle
--rw-r--r--   0        0        0    12902 2020-02-02 00:00:00.000000 odil-0.1.7/src/odil/optimizer.py
--rw-r--r--   0        0        0    10077 2020-02-02 00:00:00.000000 odil-0.1.7/src/odil/plot.py
--rw-r--r--   0        0        0     2298 2020-02-02 00:00:00.000000 odil-0.1.7/src/odil/plotutil.py
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 odil-0.1.7/src/odil/requirements.txt
--rw-r--r--   0        0        0     2396 2020-02-02 00:00:00.000000 odil-0.1.7/src/odil/runtime.py
--rw-r--r--   0        0        0    19555 2020-02-02 00:00:00.000000 odil-0.1.7/src/odil/util.py
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 odil-0.1.7/tests/.gitignore
--rw-r--r--   0        0        0      671 2020-02-02 00:00:00.000000 odil-0.1.7/tests/Makefile
--rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 odil-0.1.7/tests/README.md
--rwxr-xr-x   0        0        0     2298 2020-02-02 00:00:00.000000 odil-0.1.7/tests/test_domain.py
--rwxr-xr-x   0        0        0      944 2020-02-02 00:00:00.000000 odil-0.1.7/tests/test_io.py
--rwxr-xr-x   0        0        0     1906 2020-02-02 00:00:00.000000 odil-0.1.7/tests/test_mg_interp.py
--rwxr-xr-x   0        0        0     2319 2020-02-02 00:00:00.000000 odil-0.1.7/tests/test_mg_restrict.py
--rwxr-xr-x   0        0        0     4898 2020-02-02 00:00:00.000000 odil-0.1.7/tests/test_newton.py
--rwxr-xr-x   0        0        0     3863 2020-02-02 00:00:00.000000 odil-0.1.7/tests/test_optimize.py
--rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 odil-0.1.7/.gitignore
--rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 odil-0.1.7/LICENSE
--rw-r--r--   0        0        0     3678 2020-02-02 00:00:00.000000 odil-0.1.7/README.md
--rw-r--r--   0        0        0      711 2020-02-02 00:00:00.000000 odil-0.1.7/pyproject.toml
--rw-r--r--   0        0        0     4315 2020-02-02 00:00:00.000000 odil-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 odil-0.1.8/.style.yapf
+-rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 odil-0.1.8/Makefile
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 odil-0.1.8/setup.cfg
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 odil-0.1.8/examples/.gitignore
+-rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 odil-0.1.8/examples/README.md
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 odil-0.1.8/examples/basic/README.md
+-rwxr-xr-x   0        0        0      753 2020-02-02 00:00:00.000000 odil-0.1.8/examples/basic/README.py
+-rw-r--r--   0        0        0     6436 2020-02-02 00:00:00.000000 odil-0.1.8/examples/basic/fields.ipynb
+-rwxr-xr-x   0        0        0     4449 2020-02-02 00:00:00.000000 odil-0.1.8/examples/basic/fields.py
+-rw-r--r--   0        0        0     2233 2020-02-02 00:00:00.000000 odil-0.1.8/examples/heat/README.md
+-rwxr-xr-x   0        0        0     1540 2020-02-02 00:00:00.000000 odil-0.1.8/examples/heat/README.py
+-rwxr-xr-x   0        0        0    20973 2020-02-02 00:00:00.000000 odil-0.1.8/examples/heat/heat.py
+-rwxr-xr-x   0        0        0     1657 2020-02-02 00:00:00.000000 odil-0.1.8/examples/heat/plot_train.py
+-rwxr-xr-x   0        0        0     1909 2020-02-02 00:00:00.000000 odil-0.1.8/examples/heat/run
+-rwxr-xr-x   0        0        0      369 2020-02-02 00:00:00.000000 odil-0.1.8/examples/heat/run_all
+-rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 odil-0.1.8/examples/infer_constant/README.md
+-rwxr-xr-x   0        0        0      785 2020-02-02 00:00:00.000000 odil-0.1.8/examples/infer_constant/README.py
+-rwxr-xr-x   0        0        0     5972 2020-02-02 00:00:00.000000 odil-0.1.8/examples/infer_constant/infer_constant.py
+-rw-r--r--   0        0        0      600 2020-02-02 00:00:00.000000 odil-0.1.8/examples/poisson/README.md
+-rwxr-xr-x   0        0        0      729 2020-02-02 00:00:00.000000 odil-0.1.8/examples/poisson/README.py
+-rwxr-xr-x   0        0        0     1415 2020-02-02 00:00:00.000000 odil-0.1.8/examples/poisson/plot_field.py
+-rwxr-xr-x   0        0        0     1079 2020-02-02 00:00:00.000000 odil-0.1.8/examples/poisson/plot_train.py
+-rwxr-xr-x   0        0        0     9857 2020-02-02 00:00:00.000000 odil-0.1.8/examples/poisson/poisson.py
+-rwxr-xr-x   0        0        0      497 2020-02-02 00:00:00.000000 odil-0.1.8/examples/poisson/run
+-rw-r--r--   0        0        0      659 2020-02-02 00:00:00.000000 odil-0.1.8/examples/velocity_from_tracer/README.md
+-rwxr-xr-x   0        0        0      778 2020-02-02 00:00:00.000000 odil-0.1.8/examples/velocity_from_tracer/README.py
+-rwxr-xr-x   0        0        0     8799 2020-02-02 00:00:00.000000 odil-0.1.8/examples/velocity_from_tracer/veltracer.py
+-rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 odil-0.1.8/src/.gitignore
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 odil-0.1.8/src/odil/.gitignore
+-rw-r--r--   0        0        0      980 2020-02-02 00:00:00.000000 odil-0.1.8/src/odil/__init__.py
+-rw-r--r--   0        0        0    11780 2020-02-02 00:00:00.000000 odil-0.1.8/src/odil/backend.py
+-rw-r--r--   0        0        0     2345 2020-02-02 00:00:00.000000 odil-0.1.8/src/odil/cache.py
+-rw-r--r--   0        0        0    61549 2020-02-02 00:00:00.000000 odil-0.1.8/src/odil/core.py
+-rw-r--r--   0        0        0     2766 2020-02-02 00:00:00.000000 odil-0.1.8/src/odil/core_min.py
+-rw-r--r--   0        0        0     3660 2020-02-02 00:00:00.000000 odil-0.1.8/src/odil/history.py
+-rw-r--r--   0        0        0     9008 2020-02-02 00:00:00.000000 odil-0.1.8/src/odil/io.py
+-rw-r--r--   0        0        0     6482 2020-02-02 00:00:00.000000 odil-0.1.8/src/odil/linsolver.py
+-rw-r--r--   0        0        0      787 2020-02-02 00:00:00.000000 odil-0.1.8/src/odil/odil.mplstyle
+-rw-r--r--   0        0        0    12902 2020-02-02 00:00:00.000000 odil-0.1.8/src/odil/optimizer.py
+-rw-r--r--   0        0        0    10077 2020-02-02 00:00:00.000000 odil-0.1.8/src/odil/plot.py
+-rw-r--r--   0        0        0     2298 2020-02-02 00:00:00.000000 odil-0.1.8/src/odil/plotutil.py
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 odil-0.1.8/src/odil/requirements.txt
+-rw-r--r--   0        0        0     2396 2020-02-02 00:00:00.000000 odil-0.1.8/src/odil/runtime.py
+-rw-r--r--   0        0        0    19555 2020-02-02 00:00:00.000000 odil-0.1.8/src/odil/util.py
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 odil-0.1.8/tests/.gitignore
+-rw-r--r--   0        0        0      671 2020-02-02 00:00:00.000000 odil-0.1.8/tests/Makefile
+-rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 odil-0.1.8/tests/README.md
+-rwxr-xr-x   0        0        0     2298 2020-02-02 00:00:00.000000 odil-0.1.8/tests/test_domain.py
+-rwxr-xr-x   0        0        0      946 2020-02-02 00:00:00.000000 odil-0.1.8/tests/test_io.py
+-rwxr-xr-x   0        0        0     1906 2020-02-02 00:00:00.000000 odil-0.1.8/tests/test_mg_interp.py
+-rwxr-xr-x   0        0        0     2319 2020-02-02 00:00:00.000000 odil-0.1.8/tests/test_mg_restrict.py
+-rwxr-xr-x   0        0        0     4898 2020-02-02 00:00:00.000000 odil-0.1.8/tests/test_newton.py
+-rwxr-xr-x   0        0        0     3863 2020-02-02 00:00:00.000000 odil-0.1.8/tests/test_optimize.py
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 odil-0.1.8/.gitignore
+-rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 odil-0.1.8/LICENSE
+-rw-r--r--   0        0        0     3373 2020-02-02 00:00:00.000000 odil-0.1.8/README.md
+-rw-r--r--   0        0        0      711 2020-02-02 00:00:00.000000 odil-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0     4010 2020-02-02 00:00:00.000000 odil-0.1.8/PKG-INFO
```

### Comparing `odil-0.1.7/examples/basic/README.md` & `odil-0.1.8/examples/basic/README.md`

 * *Files identical despite different names*

### Comparing `odil-0.1.7/examples/basic/README.py` & `odil-0.1.8/examples/basic/README.py`

 * *Files identical despite different names*

### Comparing `odil-0.1.7/examples/basic/fields.ipynb` & `odil-0.1.8/examples/basic/fields.ipynb`

 * *Files identical despite different names*

### Comparing `odil-0.1.7/examples/basic/fields.py` & `odil-0.1.8/examples/basic/fields.py`

 * *Files identical despite different names*

### Comparing `odil-0.1.7/examples/heat/README.md` & `odil-0.1.8/examples/heat/README.md`

 * *Files identical despite different names*

### Comparing `odil-0.1.7/examples/heat/README.py` & `odil-0.1.8/examples/heat/README.py`

 * *Files identical despite different names*

### Comparing `odil-0.1.7/examples/heat/heat.py` & `odil-0.1.8/examples/heat/heat.py`

 * *Files identical despite different names*

### Comparing `odil-0.1.7/examples/heat/plot_train.py` & `odil-0.1.8/examples/heat/plot_train.py`

 * *Files identical despite different names*

### Comparing `odil-0.1.7/examples/heat/run` & `odil-0.1.8/examples/heat/run`

 * *Files identical despite different names*

### Comparing `odil-0.1.7/examples/infer_constant/README.md` & `odil-0.1.8/examples/infer_constant/README.md`

 * *Files identical despite different names*

### Comparing `odil-0.1.7/examples/infer_constant/README.py` & `odil-0.1.8/examples/infer_constant/README.py`

 * *Files identical despite different names*

### Comparing `odil-0.1.7/examples/infer_constant/infer_constant.py` & `odil-0.1.8/examples/infer_constant/infer_constant.py`

 * *Files identical despite different names*

### Comparing `odil-0.1.7/examples/poisson/README.md` & `odil-0.1.8/examples/poisson/README.md`

 * *Files identical despite different names*

### Comparing `odil-0.1.7/examples/poisson/README.py` & `odil-0.1.8/examples/poisson/README.py`

 * *Files identical despite different names*

### Comparing `odil-0.1.7/examples/poisson/plot_field.py` & `odil-0.1.8/examples/poisson/plot_field.py`

 * *Files identical despite different names*

### Comparing `odil-0.1.7/examples/poisson/plot_train.py` & `odil-0.1.8/examples/poisson/plot_train.py`

 * *Files identical despite different names*

### Comparing `odil-0.1.7/examples/poisson/poisson.py` & `odil-0.1.8/examples/poisson/poisson.py`

 * *Files 1% similar despite different names*

```diff
@@ -213,15 +213,15 @@
         ax.set_xlabel('x')
         ax.set_ylabel('rhs')
         plotutil.savefig(fig, "rhs" + suff, pad_inches=0.01)
         plt.close(fig)
 
     if args.dump_xmf and ndim in [2, 3]:
         u = domain.field(state, key)
-        path = key + '{}.xmf'.format(suff)
+        path = key + '{}.xdmf2'.format(suff)
         write_field(u, key, path, domain, args.cellbased)
         paths.append(path)
 
     if args.dump_data:
         x = domain.points()
         u = domain.field(state, key)
         path = "data{}.pickle".format(suff)
@@ -296,16 +296,16 @@
     state = domain.init_state(state)
 
     extra = argparse.Namespace()
     extra.ref_u = ref_u
     extra.rhs = rhs
     extra.args = args
     if args.plot:
-        write_field(extra.ref_u, 'u', 'ref_u.xmf', domain, cellbased)
-        write_field(extra.rhs, 'rhs', 'rhs.xmf', domain, cellbased)
+        write_field(extra.ref_u, 'u', 'ref_u.xdmf2', domain, cellbased)
+        write_field(extra.rhs, 'rhs', 'rhs.xdmf2', domain, cellbased)
 
     problem = odil.Problem(operator, domain, extra)
     return problem, state
 
 
 def main():
     args = parse_args()
```

### Comparing `odil-0.1.7/examples/velocity_from_tracer/README.md` & `odil-0.1.8/examples/velocity_from_tracer/README.md`

 * *Files identical despite different names*

### Comparing `odil-0.1.7/examples/velocity_from_tracer/README.py` & `odil-0.1.8/examples/velocity_from_tracer/README.py`

 * *Files identical despite different names*

### Comparing `odil-0.1.7/examples/velocity_from_tracer/veltracer.py` & `odil-0.1.8/examples/velocity_from_tracer/veltracer.py`

 * *Files identical despite different names*

### Comparing `odil-0.1.7/src/odil/__init__.py` & `odil-0.1.8/src/odil/__init__.py`

 * *Files identical despite different names*

### Comparing `odil-0.1.7/src/odil/backend.py` & `odil-0.1.8/src/odil/backend.py`

 * *Files 1% similar despite different names*

```diff
@@ -101,14 +101,15 @@
 
         if jax:
             self.stop_gradient = jax.lax.stop_gradient
             self.broadcast_to = jax.numpy.broadcast_to
             self.jit_wrap = lambda **kwargs: partial(jax.jit, **kwargs)
         else:
             self.broadcast_to = mod.broadcast_to
+            self.stop_gradient = lambda x: x
 
         def convolution(input, filters, strides, padding):
             '''
             input: n-dimensional input array
             filters: n-dimiensional kernel
             strides: `int` or sequence of n integers
             '''
```

### Comparing `odil-0.1.7/src/odil/cache.py` & `odil-0.1.8/src/odil/cache.py`

 * *Files identical despite different names*

### Comparing `odil-0.1.7/src/odil/core.py` & `odil-0.1.8/src/odil/core.py`

 * *Files identical despite different names*

### Comparing `odil-0.1.7/src/odil/core_min.py` & `odil-0.1.8/src/odil/core_min.py`

 * *Files identical despite different names*

### Comparing `odil-0.1.7/src/odil/history.py` & `odil-0.1.8/src/odil/history.py`

 * *Files identical despite different names*

### Comparing `odil-0.1.7/src/odil/io.py` & `odil-0.1.8/src/odil/io.py`

 * *Files 11% similar despite different names*

```diff
@@ -49,17 +49,19 @@
     xmfpath: path to xmf metadata file
     '''
     meta = parse_raw_xmf(xmfpath)
     dtype = {4: np.float32, 8: np.float64}[meta['precision']]
     u = np.fromfile(meta['rawpath'], dtype).reshape(meta['count'])
     return u, meta
 
+
 def read_raw(xmfpath):
     return read_raw_with_xmf(xmfpath)
 
+
 def write_raw_xmf(xmfpath,
                   rawpath,
                   count,
                   spacing=(1, 1, 1),
                   name=None,
                   precision=8,
                   cell=True):
@@ -174,31 +176,37 @@
     write_raw_xmf(xmfpath, rawrelpath, u.shape, spacing, name, precision, cell)
     u.tofile(rawpath)
     return xmfpath
 
 
 def write_vtk_poly(fout,
                    points,
-                   polygons,
+                   polygons=None,
+                   lines=None,
                    point_fields=None,
                    cell_fields=None,
+                   tcoords=None,
                    comment="",
                    fmt='%.16g'):
     """
     Writes polygons to ASCII legacy VTK file.
     fout: `str` or file-like
         Path to output legacy VTK file or file-like object.
     points: `numpy.ndarray`, shape (npoints, 3)
         3D points.
     polygons: `list` [`list` [ `int` ]], shape (ncells, ...)
         Polygons as lists of indices in `points`.
+    lines: `list` [`list` [ `int` ]], shape (nlines, ...)
+        Lines as lists of indices in `points`.
     point_fields: `dict` from `str` to array of shape (npoints,)
         Mapping from names to arrays storing scalar fields on points.
     cell_fields: `dict` from `str` to array of shape (ncells,)
         Mapping from names to arrays storing scalar fields on cells.
+    tcoords: `numpy.ndarray`, shape (npoints, 2)
+        Array storing texture coordinates of the points.
     """
     path = None
     if type(fout) is str:
         path = fout
         fout = open(path, 'wb')
 
     def write(data):
@@ -216,44 +224,60 @@
 
     # Write points.
     npoints = len(points)
     write("POINTS {:} float\n".format(npoints))
     np.savetxt(fout, points, fmt=fmt)
 
     # Write cells.
-    ncells = len(polygons)
-    num_poly_data = len(polygons) + sum([len(p) for p in polygons])
-    write("POLYGONS {:} {:}\n".format(ncells, num_poly_data))
-    for p in polygons:
-        write(' '.join(map(str, [len(p)] + p)) + '\n')
+    if polygons is not None:
+        ncells = len(polygons)
+        cells_data_size = len(polygons) + sum([len(p) for p in polygons])
+        write("POLYGONS {:} {:}\n".format(ncells, cells_data_size))
+        for p in polygons:
+            write(' '.join(map(str, [len(p)] + p)) + '\n')
+
+    # Write lines.
+    if lines is not None:
+        nlines = len(lines)
+        lines_data_size = len(lines) + sum([len(p) for p in lines])
+        write("LINES {:} {:}\n".format(nlines, lines_data_size))
+        for p in lines:
+            write(' '.join(map(str, [len(p)] + p)) + '\n')
 
-    # Write point fields.
-    if point_fields is None:
-        point_fields = dict()
-    if point_fields:
+    # Write point data header.
+    if point_fields is not None or tcoords is not None:
         write("\nPOINT_DATA {:}\n".format(npoints))
-    for name, array in point_fields.items():
-        array = np.reshape(array, -1)
-        if array.size != npoints:
-            raise RuntimeError(
-                f"Expected equal array.size={array.size} and npoints={npoints}"
-            )
-        write("SCALARS {:} float\n".format(name))
-        write("LOOKUP_TABLE default\n")
-        np.savetxt(fout, array, fmt=fmt)
+
+    # Write point fields.
+    if point_fields is not None:
+        for name, array in point_fields.items():
+            array = np.reshape(array, -1)
+            if array.size != npoints:
+                raise RuntimeError(
+                    f"Expected equal array.size={array.size} and npoints={npoints}"
+                )
+            write("SCALARS {:} float\n".format(name))
+            write("LOOKUP_TABLE default\n")
+            np.savetxt(fout, array, fmt=fmt)
+
+    # Write texture coordinates.
+    if tcoords is not None:
+        if tcoords.shape != (npoints, 2):
+            raise RuntimeError("Expected array.shape=({}, 2), got {}".format(
+                npoints, tcoords.shape))
+        write("TEXTURE_COORDINATES {} 2 float\n".format('tcoords'))
+        np.savetxt(fout, tcoords, fmt=fmt)
 
     # Write cell fields.
-    if cell_fields is None:
-        cell_fields = dict()
-    if cell_fields:
+    if cell_fields is not None:
         write("\nCELL_DATA {:}\n".format(ncells))
-    for name, array in cell_fields.items():
-        array = np.reshape(array, -1)
-        if array.size != ncells:
-            raise RuntimeError(
-                f"Expected equal array.size={array.size} and ncells={ncells}")
-        write("SCALARS {:} float\n".format(name))
-        write("LOOKUP_TABLE default\n")
-        np.savetxt(fout, array, fmt=fmt)
+        for name, array in cell_fields.items():
+            array = np.reshape(array, -1)
+            if array.size != ncells:
+                raise RuntimeError(
+                    f"Expected equal array.size={array.size} and ncells={ncells}")
+            write("SCALARS {:} float\n".format(name))
+            write("LOOKUP_TABLE default\n")
+            np.savetxt(fout, array, fmt=fmt)
 
     if path:
         fout.close()
```

### Comparing `odil-0.1.7/src/odil/linsolver.py` & `odil-0.1.8/src/odil/linsolver.py`

 * *Files identical despite different names*

### Comparing `odil-0.1.7/src/odil/odil.mplstyle` & `odil-0.1.8/src/odil/odil.mplstyle`

 * *Files identical despite different names*

### Comparing `odil-0.1.7/src/odil/optimizer.py` & `odil-0.1.8/src/odil/optimizer.py`

 * *Files identical despite different names*

### Comparing `odil-0.1.7/src/odil/plot.py` & `odil-0.1.8/src/odil/plot.py`

 * *Files identical despite different names*

### Comparing `odil-0.1.7/src/odil/plotutil.py` & `odil-0.1.8/src/odil/plotutil.py`

 * *Files identical despite different names*

### Comparing `odil-0.1.7/src/odil/runtime.py` & `odil-0.1.8/src/odil/runtime.py`

 * *Files identical despite different names*

### Comparing `odil-0.1.7/src/odil/util.py` & `odil-0.1.8/src/odil/util.py`

 * *Files identical despite different names*

### Comparing `odil-0.1.7/tests/Makefile` & `odil-0.1.8/tests/Makefile`

 * *Files identical despite different names*

### Comparing `odil-0.1.7/tests/test_domain.py` & `odil-0.1.8/tests/test_domain.py`

 * *Files identical despite different names*

### Comparing `odil-0.1.7/tests/test_io.py` & `odil-0.1.8/tests/test_io.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import odil
 import numpy as np
 
 class TestIO(unittest.TestCase):
 
     def test_raw_xmf(self):
         name = "foo"
-        xmfpath = "data.xmf"
+        xmfpath = "data.xdmf2"
         nx, ny, nz = 3, 4, 5
         lx, ly, lz = 4, 5, 6
         for dtype in [np.float32, np.float64]:
             u_src = np.linspace(0, 1, nx * ny * nz).reshape(
                 (nz, ny, nx)).astype(dtype)
             spacing = (lx / nx, ly / ny, lz / nz)
             odil.write_raw_with_xmf(u_src, xmfpath, spacing=spacing, name=name)
```

### Comparing `odil-0.1.7/tests/test_mg_interp.py` & `odil-0.1.8/tests/test_mg_interp.py`

 * *Files identical despite different names*

### Comparing `odil-0.1.7/tests/test_mg_restrict.py` & `odil-0.1.8/tests/test_mg_restrict.py`

 * *Files identical despite different names*

### Comparing `odil-0.1.7/tests/test_newton.py` & `odil-0.1.8/tests/test_newton.py`

 * *Files identical despite different names*

### Comparing `odil-0.1.7/tests/test_optimize.py` & `odil-0.1.8/tests/test_optimize.py`

 * *Files identical despite different names*

### Comparing `odil-0.1.7/LICENSE` & `odil-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `odil-0.1.7/README.md` & `odil-0.1.8/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -33,32 +33,28 @@
 ## Using GPU
 
 To enable GPU support, provide a non-empty list of devices in `CUDA_VISIBLE_DEVICES`.
 Values `CUDA_VISIBLE_DEVICES=` and `CUDA_VISIBLE_DEVICES=-1` disable GPU support.
 
 ## Developers
 
-ODIL is developed by researchers at [Harvard University](https://cse-lab.seas.harvard.edu/)
+ODIL is developed by researchers at [Harvard University](https://cse-lab.seas.harvard.edu)
 
-* [Petr Karnakov](https://cse-lab.seas.harvard.edu/people/petr-karnakov)
-  [<img src="https://cselab.github.io/odil/media/twitter.png" height=16>](https://twitter.com/pkarnakov)
-  [<img src="https://cselab.github.io/odil/media/youtube.png" height=16>](https://www.youtube.com/@pkarnakov)
+* [Petr Karnakov](https://pkarnakov.com)
 * [Sergey Litvinov](https://cse-lab.seas.harvard.edu/people/sergey-litvinov)
 
 advised by
 
 * [Prof. Petros Koumoutsakos](https://cse-lab.seas.harvard.edu/people/petros-koumoutsakos)
 
 ## Publications
 
 1. Karnakov P, Litvinov S, Koumoutsakos P. Solving inverse problems in physics
    by optimizing a discrete loss: Fast and accurate learning without neural networks. PNAS Nexus, 2024.
    [DOI:10.1093/pnasnexus/pgae005](https://doi.org/10.1093/pnasnexus/pgae005)
-   [arXiv:2205.04611](https://arxiv.org/abs/2205.04611)
-
 
 2. Karnakov P, Litvinov S, Koumoutsakos P. Flow reconstruction by
    multiresolution optimization of a discrete loss with automatic
    differentiation. Eur. Phys. J, 2023.
    [DOI:10.1140/epje/s10189-023-00313-7](https://doi.org/10.1140/epje/s10189-023-00313-7)
    [arXiv:2303.04679](https://arxiv.org/abs/2303.04679)
    [slides](https://cselab.github.io/odil/slides/usc_workshop.pdf)
```

### Comparing `odil-0.1.7/pyproject.toml` & `odil-0.1.8/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "odil"
-version = "0.1.7"
+version = "0.1.8"
 authors = [
     { name="Petr Karnakov", email="pkarnakov@gmail.com" },
     { name="Sergey Litvinov", email="slitvinov@gmail.com" },
 ]
 description = "ODIL (Optimizing a DIscrete Loss) is a framework for solving inverse problems for differential equations"
 readme = "README.md"
 dependencies = [
```

### Comparing `odil-0.1.7/PKG-INFO` & `odil-0.1.8/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: odil
-Version: 0.1.7
+Version: 0.1.8
 Summary: ODIL (Optimizing a DIscrete Loss) is a framework for solving inverse problems for differential equations
 Project-URL: Homepage, https://github.com/cselab/odil
 Project-URL: Issues, https://github.com/cselab/odil/issues
 Author-email: Petr Karnakov <pkarnakov@gmail.com>, Sergey Litvinov <slitvinov@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -49,32 +49,28 @@
 ## Using GPU
 
 To enable GPU support, provide a non-empty list of devices in `CUDA_VISIBLE_DEVICES`.
 Values `CUDA_VISIBLE_DEVICES=` and `CUDA_VISIBLE_DEVICES=-1` disable GPU support.
 
 ## Developers
 
-ODIL is developed by researchers at [Harvard University](https://cse-lab.seas.harvard.edu/)
+ODIL is developed by researchers at [Harvard University](https://cse-lab.seas.harvard.edu)
 
-* [Petr Karnakov](https://cse-lab.seas.harvard.edu/people/petr-karnakov)
-  [<img src="https://cselab.github.io/odil/media/twitter.png" height=16>](https://twitter.com/pkarnakov)
-  [<img src="https://cselab.github.io/odil/media/youtube.png" height=16>](https://www.youtube.com/@pkarnakov)
+* [Petr Karnakov](https://pkarnakov.com)
 * [Sergey Litvinov](https://cse-lab.seas.harvard.edu/people/sergey-litvinov)
 
 advised by
 
 * [Prof. Petros Koumoutsakos](https://cse-lab.seas.harvard.edu/people/petros-koumoutsakos)
 
 ## Publications
 
 1. Karnakov P, Litvinov S, Koumoutsakos P. Solving inverse problems in physics
    by optimizing a discrete loss: Fast and accurate learning without neural networks. PNAS Nexus, 2024.
    [DOI:10.1093/pnasnexus/pgae005](https://doi.org/10.1093/pnasnexus/pgae005)
-   [arXiv:2205.04611](https://arxiv.org/abs/2205.04611)
-
 
 2. Karnakov P, Litvinov S, Koumoutsakos P. Flow reconstruction by
    multiresolution optimization of a discrete loss with automatic
    differentiation. Eur. Phys. J, 2023.
    [DOI:10.1140/epje/s10189-023-00313-7](https://doi.org/10.1140/epje/s10189-023-00313-7)
    [arXiv:2303.04679](https://arxiv.org/abs/2303.04679)
    [slides](https://cselab.github.io/odil/slides/usc_workshop.pdf)
```

