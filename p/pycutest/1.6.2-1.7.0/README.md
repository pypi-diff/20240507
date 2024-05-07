# Comparing `tmp/pycutest-1.6.2.tar.gz` & `tmp/pycutest-1.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycutest-1.6.2.tar", last modified: Tue Apr  9 07:31:03 2024, max compression
+gzip compressed data, was "pycutest-1.7.0.tar", last modified: Tue May  7 09:28:36 2024, max compression
```

## Comparing `pycutest-1.6.2.tar` & `pycutest-1.7.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 07:31:03.615249 pycutest-1.6.2/
--rw-r--r--   0 runner    (1001) docker     (127)    35147 2024-04-09 07:30:57.000000 pycutest-1.6.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     9723 2024-04-09 07:31:03.615249 pycutest-1.6.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8023 2024-04-09 07:30:57.000000 pycutest-1.6.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 07:31:03.615249 pycutest-1.6.2/pycutest/
--rw-r--r--   0 runner    (1001) docker     (127)     1579 2024-04-09 07:30:57.000000 pycutest-1.6.2/pycutest/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14879 2024-04-09 07:30:57.000000 pycutest-1.6.2/pycutest/build_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)    75292 2024-04-09 07:30:57.000000 pycutest-1.6.2/pycutest/c_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     2518 2024-04-09 07:30:57.000000 pycutest-1.6.2/pycutest/install_scripts.py
--rw-r--r--   0 runner    (1001) docker     (127)    45385 2024-04-09 07:30:57.000000 pycutest-1.6.2/pycutest/problem_class.py
--rw-r--r--   0 runner    (1001) docker     (127)     4126 2024-04-09 07:30:57.000000 pycutest-1.6.2/pycutest/python_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)    11613 2024-04-09 07:30:57.000000 pycutest-1.6.2/pycutest/sifdecode_extras.py
--rw-r--r--   0 runner    (1001) docker     (127)     4237 2024-04-09 07:30:57.000000 pycutest-1.6.2/pycutest/system_paths.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 07:31:03.615249 pycutest-1.6.2/pycutest.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9723 2024-04-09 07:31:03.000000 pycutest-1.6.2/pycutest.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      402 2024-04-09 07:31:03.000000 pycutest-1.6.2/pycutest.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 07:31:03.000000 pycutest-1.6.2/pycutest.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-09 07:31:03.000000 pycutest-1.6.2/pycutest.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-09 07:31:03.000000 pycutest-1.6.2/pycutest.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1884 2024-04-09 07:30:57.000000 pycutest-1.6.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 07:31:03.615249 pycutest-1.6.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 09:28:36.532824 pycutest-1.7.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    35147 2024-05-07 09:28:30.000000 pycutest-1.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     9813 2024-05-07 09:28:36.532824 pycutest-1.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8113 2024-05-07 09:28:30.000000 pycutest-1.7.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 09:28:36.532824 pycutest-1.7.0/pycutest/
+-rw-r--r--   0 runner    (1001) docker     (127)     1579 2024-05-07 09:28:30.000000 pycutest-1.7.0/pycutest/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14879 2024-05-07 09:28:30.000000 pycutest-1.7.0/pycutest/build_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)    80660 2024-05-07 09:28:30.000000 pycutest-1.7.0/pycutest/c_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2518 2024-05-07 09:28:30.000000 pycutest-1.7.0/pycutest/install_scripts.py
+-rw-r--r--   0 runner    (1001) docker     (127)    50368 2024-05-07 09:28:30.000000 pycutest-1.7.0/pycutest/problem_class.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4126 2024-05-07 09:28:30.000000 pycutest-1.7.0/pycutest/python_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11613 2024-05-07 09:28:30.000000 pycutest-1.7.0/pycutest/sifdecode_extras.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4237 2024-05-07 09:28:30.000000 pycutest-1.7.0/pycutest/system_paths.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 09:28:36.532824 pycutest-1.7.0/pycutest.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9813 2024-05-07 09:28:36.000000 pycutest-1.7.0/pycutest.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      402 2024-05-07 09:28:36.000000 pycutest-1.7.0/pycutest.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 09:28:36.000000 pycutest-1.7.0/pycutest.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-07 09:28:36.000000 pycutest-1.7.0/pycutest.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-07 09:28:36.000000 pycutest-1.7.0/pycutest.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1884 2024-05-07 09:28:30.000000 pycutest-1.7.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 09:28:36.532824 pycutest-1.7.0/setup.cfg
```

### Comparing `pycutest-1.6.2/LICENSE` & `pycutest-1.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pycutest-1.6.2/PKG-INFO` & `pycutest-1.7.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycutest
-Version: 1.6.2
+Version: 1.7.0
 Summary: A Python wrapper to the CUTEst optimization test environment
 Author-email: Jaroslav Fowkes <jaroslav.fowkes@maths.ox.ac.uk>, Lindon Roberts <lindon.roberts@sydney.edu.au>
 Maintainer-email: Jaroslav Fowkes <jaroslav.fowkes@maths.ox.ac.uk>, Lindon Roberts <lindon.roberts@sydney.edu.au>
 License: GPL-3.0-or-later
 Project-URL: Homepage, https://github.com/jfowkes/pycutest/
 Project-URL: Download, https://github.com/jfowkes/pycutest/releases/
 Project-URL: Bug Tracker, https://github.com/jfowkes/pycutest/issues/
@@ -44,14 +44,15 @@
 Full details on how to use PyCUTEst are available in the `documentation <https://jfowkes.github.io/pycutest/>`_, and a brief summary of the package's goals is available in the `PyCUTEst journal article <https://doi.org/10.21105/joss.04377>`_.
 
 Requirements
 ------------
 PyCUTEst requires the following software to be installed:
 
 * Python 3 (http://www.python.org/)
+* Python 3 Headers (:code:`apt install python3-dev` on Ubuntu, already included on macOS)
 * CUTEst (see below)
 
 **Please Note:** Currently PyCUTEst only supports Mac and Linux. For Windows 10 (or later), PyCUTEst can be used through the `Windows Subsystem for Linux <https://docs.microsoft.com/en-us/windows/wsl/>`_, following the Linux installation instructions.
 
 Installing CUTEst on Linux
 --------------------------
 These instructions do not include installation of the MATLAB interface. You will need to install four packages: archdefs, SIFDecode, CUTEst and MASTSIF. To keep things simple, install all four packages in the same directory:
```

### Comparing `pycutest-1.6.2/README.rst` & `pycutest-1.7.0/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 Full details on how to use PyCUTEst are available in the `documentation <https://jfowkes.github.io/pycutest/>`_, and a brief summary of the package's goals is available in the `PyCUTEst journal article <https://doi.org/10.21105/joss.04377>`_.
 
 Requirements
 ------------
 PyCUTEst requires the following software to be installed:
 
 * Python 3 (http://www.python.org/)
+* Python 3 Headers (:code:`apt install python3-dev` on Ubuntu, already included on macOS)
 * CUTEst (see below)
 
 **Please Note:** Currently PyCUTEst only supports Mac and Linux. For Windows 10 (or later), PyCUTEst can be used through the `Windows Subsystem for Linux <https://docs.microsoft.com/en-us/windows/wsl/>`_, following the Linux installation instructions.
 
 Installing CUTEst on Linux
 --------------------------
 These instructions do not include installation of the MATLAB interface. You will need to install four packages: archdefs, SIFDecode, CUTEst and MASTSIF. To keep things simple, install all four packages in the same directory:
```

### Comparing `pycutest-1.6.2/pycutest/__init__.py` & `pycutest-1.7.0/pycutest/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # Set PyCUTEst version number
-__version__ = '1.6.2'
+__version__ = '1.7.0'
 
 # Define submodules to expose on wildcard imports
 __all__ = []
 
 from .build_interface import import_problem, clear_cache, all_cached_problems
 __all__ += ['import_problem', 'clear_cache', 'all_cached_problems']
```

### Comparing `pycutest-1.6.2/pycutest/build_interface.py` & `pycutest-1.7.0/pycutest/build_interface.py`

 * *Files identical despite different names*

### Comparing `pycutest-1.6.2/pycutest/c_interface.py` & `pycutest-1.7.0/pycutest/c_interface.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,14 +48,16 @@
 static PyObject *cutest_lag(PyObject *self, PyObject *args);
 static PyObject *cutest_lagjac(PyObject *self, PyObject *args);
 static PyObject *cutest_jprod(PyObject *self, PyObject *args);
 static PyObject *cutest_hess(PyObject *self, PyObject *args);
 static PyObject *cutest_ihess(PyObject *self, PyObject *args);
 static PyObject *cutest_hprod(PyObject *self, PyObject *args);
 static PyObject *cutest_gradhess(PyObject *self, PyObject *args);
+static PyObject *cutest_sobj(PyObject *self, PyObject *args);
+static PyObject *cutest_sgrad(PyObject *self, PyObject *args);
 static PyObject *cutest_scons(PyObject *self, PyObject *args);
 static PyObject *cutest_slagjac(PyObject *self, PyObject *args);
 static PyObject *cutest_sphess(PyObject *self, PyObject *args);
 static PyObject *cutest_isphess(PyObject *self, PyObject *args);
 static PyObject *cutest_gradsphess(PyObject *self, PyObject *args);
 static PyObject *cutest_report(PyObject *self, PyObject *args);
 static PyObject *cutest_terminate(PyObject *self, PyObject *args);
@@ -137,14 +139,33 @@
     pos=0;
     while (PyDict_Next(dict, &pos, &key, &value)) {
         Py_XDECREF(value);
     }
     return dict;
 }
 
+/* Extract sparse gradient in form of NumPy arrays */
+void extract_sparse_gradient(npy_int nnzg, npy_int *si, npy_double *sv, PyArrayObject **Mgi, PyArrayObject **Mgv) {
+    npy_double *gv;
+    npy_int *gi, i;
+    npy_intp dims[1];
+
+    /* Alocate and fill objective gradient data,
+       convert indices from FORTRAN to C. */
+    dims[0]=nnzg;
+    *Mgi=(PyArrayObject *)PyArray_SimpleNew(1, dims, NPY_INT);
+    *Mgv=(PyArrayObject *)PyArray_SimpleNew(1, dims, NPY_DOUBLE);
+    gi=(npy_int *)PyArray_DATA(*Mgi);
+    gv=(npy_double *)PyArray_DATA(*Mgv);
+    for(i=0;i<nnzg;i++) {
+        gi[i]=si[i]-1;
+        gv[i]=sv[i];
+    }
+}
+
 /* Extract sparse gradient and Jacobian in form of NumPy arrays */
 void extract_sparse_gradient_jacobian(npy_int nnzjplusno, npy_int *sji, npy_int *sjfi, npy_double *sjv,
         PyArrayObject **Mgi, PyArrayObject **Mgv, PyArrayObject **MJi, PyArrayObject **MJfi, PyArrayObject **MJv) {
     npy_double *gv, *Jv;
     npy_int *gi, *Ji, *Jfi, nnzg, i, jg, jj;
     npy_intp dims[1];
 
@@ -657,15 +678,15 @@
     }
 }
 
 
 PyDoc_STRVAR(cutest_grad_doc,
 "Returns the gradient of the objective or gradient of the i-th constraint at x.\n"
 "\n"
-"g=grad(x)   -- objective gradient\n"       
+"g=grad(x)   -- objective gradient\n"
 "g=grad(x,i) -- i-th constraint gradient\n"
 "\n"
 "Input\n"
 "x -- 1D array of length n with the values of variables\n"
 "i -- integer index of constraint (between 0 and m-1)\n"
 "\n"
 "Output\n"
@@ -1395,14 +1416,148 @@
     } else {
         CUTEST_ugrdh((integer *)&status, (integer *)&CUTEst_nvar, x, g, (integer *)&CUTEst_nvar, H);
         return Py_BuildValue("OO", Mg, MH);
     }
 }
 
 
+PyDoc_STRVAR(cutest_sobj_doc,
+"Returns the value of objective and its sparse gradient at x (constrained problems only).\n"
+"\n"
+"f=sobj(x)\n"
+"(f, gi, gv)=sobj(x, gradFlag)\n"
+"\n"
+"Input\n"
+"x        -- 1D array of length n with the values of variables\n"
+"gradFlag -- if given the function returns f and gi,gv; can be anything\n"
+"\n"
+"Output\n"
+"f -- float holding the value of the function at x\n"
+"gi  -- 1D array of integers holding the indices (0 .. n-1) of nonzero\n"
+"       elements in the sparse gradient vector\n"
+"gv  -- 1D array holding the values of nonzero elements in the sparse gradient\n"
+"       vector. Has the same length as gi.\n"
+"\n"
+"CUTEst tools used: CUTEST_cofsg\n"
+);
+
+static PyObject *cutest_sobj(PyObject *self, PyObject *args) {
+    PyArrayObject *arg1, *Mgi, *Mgv;
+    PyObject *arg2;
+    doublereal *x, *sv;
+    doublereal f;
+    npy_int *si;
+    npy_int nnzg, nzero=0;
+
+    if (!check_setup())
+        return NULL;
+
+    if (CUTEst_ncon == 0) {
+        PyErr_SetString(PyExc_Exception, "For unconstrained problems please use obj()");
+        return NULL;
+    }
+
+    if (!PyArg_ParseTuple(args, "O|O", &arg1, &arg2))
+        return NULL;
+
+    /* Check if x is double and of correct length and shape */
+    if (!(PyArray_Check(arg1) && PyArray_ISFLOAT(arg1) && PyArray_TYPE(arg1)==NPY_DOUBLE && PyArray_NDIM(arg1)==1 && PyArray_DIM(arg1, 0)==CUTEst_nvar)) {
+        PyErr_SetString(PyExc_Exception, "Argument 1 must be a 1D double array of length nvar");
+        return NULL;
+    }
+
+    x=(npy_double *)PyArray_DATA(arg1);
+    if (PyObject_Length(args)==1) {
+        CUTEST_cofsg((integer *)&status, (integer *)&CUTEst_nvar, x, &f, (integer *)&nnzg, (integer *)&nzero, NULL, NULL, &somethingFalse);
+        return Py_BuildValue("d", f);
+    } else {
+        si=(npy_int *)malloc(CUTEst_nvar*sizeof(npy_int));
+        sv=(npy_double *)malloc(CUTEst_nvar*sizeof(npy_double));
+
+        CUTEST_cofsg((integer *)&status, (integer *)&CUTEst_nvar, x, &f, (integer *)&nnzg, (integer *)&CUTEst_nvar, sv, (integer *)si, &somethingTrue);
+
+        extract_sparse_gradient(nnzg, si, sv, (PyArrayObject **)&Mgi, (PyArrayObject **)&Mgv);
+
+        free(si);
+        free(sv);
+
+        return Py_BuildValue("dOO", f, Mgi, Mgv);
+    }
+}
+
+
+PyDoc_STRVAR(cutest_sgrad_doc,
+"Returns the sparse gradient of the objective or gradient of the i-th constraint at x (constrained problems only).\n"
+"\n"
+"(gi, gv)=sgrad(x)   -- objective gradient\n"
+"(gi, gv)=sgrad(x,i) -- i-th constraint gradient\n"
+"\n"
+"Input\n"
+"x -- 1D array of length n with the values of variables\n"
+"i -- integer index of constraint (between 0 and m-1)\n"
+"\n"
+"Output\n"
+"gi  -- 1D array of integers holding the indices (0 .. n-1) of nonzero\n"
+"       elements in the sparse gradient vector\n"
+"gv  -- 1D array holding the values of nonzero elements in the sparse gradient\n"
+"       vector. Has the same length as gi.\n"
+"\n"
+"CUTEst tools used: CUTEST_cisgr\n"
+);
+
+static PyObject *cutest_sgrad(PyObject *self, PyObject *args) {
+    PyArrayObject *arg1, *Mgi, *Mgv;
+    doublereal *x, *sv;
+    int index;
+    npy_int *si;
+    npy_int icon, nnzg;
+
+    if (!check_setup())
+        return NULL;
+
+    if (CUTEst_ncon == 0) {
+        PyErr_SetString(PyExc_Exception, "For unconstrained problems please use grad()");
+        return NULL;
+    }
+
+    if (!PyArg_ParseTuple(args, "O|i", &arg1, &index))
+        return NULL;
+
+    /* Check if x is double and of correct length and shape */
+    if (!(PyArray_Check(arg1) && PyArray_ISFLOAT(arg1) && PyArray_TYPE(arg1)==NPY_DOUBLE && PyArray_NDIM(arg1)==1 && PyArray_DIM(arg1, 0)==CUTEst_nvar)) {
+        PyErr_SetString(PyExc_Exception, "Argument 1 must be a 1D double array of length nvar");
+        return NULL;
+    }
+
+    /* Check index */
+    if (PyObject_Length(args)>1) {
+        if (index<0 || index>=CUTEst_ncon) {
+            PyErr_SetString(PyExc_Exception, "Argument 2 must be between 0 and ncon-1");
+            return NULL;
+        }
+        icon=index+1;
+    } else {
+        icon=0;
+    }
+
+    x=(npy_double *)PyArray_DATA(arg1);
+    si=(npy_int *)malloc(CUTEst_nvar*sizeof(npy_int));
+    sv=(npy_double *)malloc(CUTEst_nvar*sizeof(npy_double));
+
+    CUTEST_cisgr((integer *)&status, (integer *)&CUTEst_nvar, (integer *)&icon, x, (integer *)&nnzg, (integer *)&CUTEst_nvar, sv, (integer *)si);
+
+    extract_sparse_gradient(nnzg, si, sv, (PyArrayObject **)&Mgi, (PyArrayObject **)&Mgv);
+
+    free(si);
+    free(sv);
+
+    return Py_BuildValue("OO", Mgi, Mgv);
+}
+
+
 PyDoc_STRVAR(cutest_scons_doc,
 "Returns the value of constraints and the sparse Jacobian of constraints at x.\n"
 "\n"
 "(c, Jvi, Jfi, Jv)=scons(x) -- Jacobian of constraints\n"
 "(ci, gi, gv)=scons(x, i)   -- i-th constraint and its gradient\n"
 "\n"
 "Input\n"
@@ -2005,14 +2160,16 @@
     {"lag", cutest_lag, METH_VARARGS, cutest_lag_doc},
     {"lagjac", cutest_lagjac, METH_VARARGS, cutest_lagjac_doc},
     {"jprod", cutest_jprod, METH_VARARGS, cutest_jprod_doc},
     {"hess", cutest_hess, METH_VARARGS, cutest_hess_doc},
     {"ihess", cutest_ihess, METH_VARARGS, cutest_ihess_doc},
     {"hprod", cutest_hprod, METH_VARARGS, cutest_hprod_doc},
     {"gradhess", cutest_gradhess, METH_VARARGS, cutest_gradhess_doc},
+    {"sobj", cutest_sobj, METH_VARARGS, cutest_sobj_doc},
+    {"sgrad", cutest_sgrad, METH_VARARGS, cutest_sgrad_doc},
     {"scons", cutest_scons, METH_VARARGS, cutest_scons_doc},
     {"slagjac", cutest_slagjac, METH_VARARGS, cutest_slagjac_doc},
     {"sphess", cutest_sphess, METH_VARARGS, cutest_sphess_doc},
     {"isphess", cutest_isphess, METH_VARARGS, cutest_isphess_doc},
     {"gradsphess", cutest_gradsphess, METH_VARARGS, cutest_gradsphess_doc},
     {"report", cutest_report, METH_VARARGS, cutest_report_doc},
     {"terminate", cutest_terminate, METH_VARARGS, cutest_terminate_doc},
```

### Comparing `pycutest-1.6.2/pycutest/install_scripts.py` & `pycutest-1.7.0/pycutest/install_scripts.py`

 * *Files identical despite different names*

### Comparing `pycutest-1.6.2/pycutest/problem_class.py` & `pycutest-1.7.0/pycutest/problem_class.py`

 * *Files 9% similar despite different names*

```diff
@@ -658,15 +658,139 @@
         if self.m > 0:
             g, J, H = self._module.gradhess(self.free_to_all(x), v, gradient_of_lagrangian)
             return self.all_to_free(g), J[:, self.idx_free], H[self.idx_free][:, self.idx_free]
         else:
             g, H = self._module.gradhess(self.free_to_all(x))
             return self.all_to_free(g), H[self.idx_free][:, self.idx_free]
 
-    # scons() wrapper (private)
+    # sobj() wrapper (private)
+    def __sobj(self, x, gradFlag=False):
+        """Returns the value of the objective and optionally its sparse gradient at x.
+           Only works on constrained problems due to the inherent design of CUTEst.
+
+        f=__sobj(x)            -- objective value
+        (f, g)=__sobj(x, True) -- objective value and sparse objective gradient
+
+        Input
+        x        -- 1D array of length n with the values of variables
+        gradFlag -- boolean flag. If True the gradient of the objective is returned. Default is False
+
+        Output
+        f -- float holding the value of the objective function at x
+        g -- a scipy.sparse.coo_matrix of size 1-by-n_full holding the gradient of objective at x
+
+        This function is a wrapper for sobj().
+        """
+
+        if gradFlag:
+            (f, gi, gv)=self._module.sobj(x, gradFlag)
+            return (f, coo_matrix((gv, (np.zeros(len(gv)), gi)), shape=(1, self.n_full)))
+        else:
+            f=self._module.sobj(x)
+            return f
+
+    def sobj(self, x, gradient=False):
+        """
+        Evaluate the objective (and optionally its sparse gradient).
+
+        .. code-block:: python
+
+            # objective
+            f    = problem.obj(x)
+            # objective and gradient
+            f, g = problem.obj(x, gradient=True)
+
+        The vector g is of type scipy.sparse.coo_matrix.
+        For unconstrained problems, g is formed from a dense matrix due to CUTEst limitations.
+
+        For small problems, problem.obj returns dense matrices.
+
+        This calls CUTEst routine CUTEst_uofg or CUTEST_cofsg.
+
+        :param x: input vector
+        :type x: numpy.ndarray with shape (n,)
+        :param gradient: whether to return objective and gradient, or just objective (default=False; i.e. objective only)
+        :type gradient: bool, optional
+        :return: objective value f, or tuple (f,g) of objective and sparse gradient at x
+        :rtype: float or (float, scipy.sparse.coo_matrix(n,))
+        """
+        self.check_input_x(x)
+        if self.m <= 0: # unconstrained problem (convert dense obj)
+            if gradient:
+                f, g = self.obj(x, True) # fixed/free variables already handled
+                return f, coo_matrix(g)  # inefficient but CUTEst gives us no choice
+            else:
+                return self.obj(x)
+        else: # constrained problem (use sobj wrapper)
+            if gradient:
+                f, g = self.__sobj(self.free_to_all(x), True)
+                return f, sparse_vec_extract_indices(g, self.idx_free)
+            else:
+                f = self.__sobj(self.free_to_all(x))
+                return f
+
+    # sgrad() wrapper
+    def __sgrad(self, x, i=None):
+        """Returns the sparse gradient of the objective or gradient of the i-th constraint at x.
+           Only works on constrained problems due to the inherent design of CUTEst.
+
+        g=__sgrad(x)    -- objective gradient
+        g=__sgrad(x, i) -- i-th constraint gradient
+
+        Input
+        x -- 1D array of length n with the values of variables
+        i -- integer index of constraint (between 0 and m-1)
+
+        Output
+        g -- a scipy.sparse.coo_matrix of size 1-by-n_full holding the gradient of objective at x or
+            the gradient of i-th constraint at x
+
+        This function is a wrapper for sgrad().
+        """
+
+        if i is None:
+            (gi, gv)=self._module.sgrad(x)
+        else:
+            (gi, gv)=self._module.sgrad(x, i)
+        return coo_matrix((gv, (np.zeros(len(gv)), gi)), shape=(1, self.n_full))
+
+    def sgrad(self, x, index=None):
+        """
+        Evaluate the sparse gradient of the objective function or sparse gradient of the i-th constraint.
+
+        .. code-block:: python
+
+            # gradient of objective
+            g = problem.grad(x)
+            # gradient of i-th constraint
+            g = problem.grad(x, index=i)
+
+        The vector g is of type scipy.sparse.coo_matrix.
+        For unconstrained problems, g is formed from a dense matrix due to CUTEst limitations.
+
+        For small problems, problem.grad returns dense matrices.
+
+        This calls CUTEst routine CUTEst_ugr or CUTEST_cisgr.
+
+        :param x: input vector
+        :type x: numpy.ndarray with shape (n,)
+        :param index: which constraint to evaluate. Must be in 0..self.m-1.
+        :type index: int, optional
+        :return: sparse gradient of objective or sparse gradient of i-th constraint at x
+        :rtype: scipy.sparse.coo_matrix(n,)
+        """
+        self.check_input_x(x)
+        if self.m <= 0: # unconstrained problem (convert dense grad)
+            g = self.grad(x, index) # fixed/free variables already handled
+            return coo_matrix(g)   # inefficient but CUTEst gives us no choice
+        else: # constrained problem (use sgrad wrapper)
+            g = self.__sgrad(self.free_to_all(x), index)
+            return sparse_vec_extract_indices(g, self.idx_free)
+
+    # scons() wrapper
     def __scons(self, x, i=None):
         """Returns the value of constraints and
         the sparse Jacobian of constraints at x.
 
         (c, J)=__scons(x)      -- Jacobian of constraints
         (ci, gi)=__scons(x, i) -- i-th constraint and its gradient
 
@@ -934,23 +1058,23 @@
         return sparse_mat_extract_rows_and_columns(H, self.idx_free, self.idx_free)
 
     # gradsphess() wrapper (private)
     def __gradsphess(self, x, v=None, lagrFlag=False):
         """Returns the sparse Hessian of the Lagrangian, the sparse Jacobian of
         constraints, and the gradient of the objective or Lagrangian.
 
-        (g, H)=__gradsphess(x)              -- unconstrained problems
-        (g, J, H)=__gradsphess(x, v, gradl) -- constrained problems
+        (g, H)=__gradsphess(x)                 -- unconstrained problems
+        (g, J, H)=__gradsphess(x, v, lagrFlag) -- constrained problems
 
         Input
-        x     -- 1D array of length n with the values of variables
-        v     -- 1D array of length m with the values of Lagrange multipliers
-        gradl -- boolean flag. If False the gradient of the objective is returned,
-                if True the gradient of the Lagrangian is returned.
-                Default is False
+        x        -- 1D array of length n with the values of variables
+        v        -- 1D array of length m with the values of Lagrange multipliers
+        lagrFlag -- boolean flag. If False the gradient of the objective is returned,
+                    if True the gradient of the Lagrangian is returned.
+                    Default is False
 
         Output
         g -- a scipy.sparse.coo_matrix of size 1-by-n_full holding the gradient of objective at x or
             the gradient of Lagrangian at (x, v)
         J -- a scipy.sparse.coo_matrix of size m-by-n_full holding the sparse Jacobian
             of constraints at x
         H -- a scipy.sparse.coo_matrix of size n_full-by-n_full holding the sparse Hessian
```

### Comparing `pycutest-1.6.2/pycutest/python_interface.py` & `pycutest-1.7.0/pycutest/python_interface.py`

 * *Files identical despite different names*

### Comparing `pycutest-1.6.2/pycutest/sifdecode_extras.py` & `pycutest-1.7.0/pycutest/sifdecode_extras.py`

 * *Files identical despite different names*

### Comparing `pycutest-1.6.2/pycutest/system_paths.py` & `pycutest-1.7.0/pycutest/system_paths.py`

 * *Files identical despite different names*

### Comparing `pycutest-1.6.2/pycutest.egg-info/PKG-INFO` & `pycutest-1.7.0/pycutest.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycutest
-Version: 1.6.2
+Version: 1.7.0
 Summary: A Python wrapper to the CUTEst optimization test environment
 Author-email: Jaroslav Fowkes <jaroslav.fowkes@maths.ox.ac.uk>, Lindon Roberts <lindon.roberts@sydney.edu.au>
 Maintainer-email: Jaroslav Fowkes <jaroslav.fowkes@maths.ox.ac.uk>, Lindon Roberts <lindon.roberts@sydney.edu.au>
 License: GPL-3.0-or-later
 Project-URL: Homepage, https://github.com/jfowkes/pycutest/
 Project-URL: Download, https://github.com/jfowkes/pycutest/releases/
 Project-URL: Bug Tracker, https://github.com/jfowkes/pycutest/issues/
@@ -44,14 +44,15 @@
 Full details on how to use PyCUTEst are available in the `documentation <https://jfowkes.github.io/pycutest/>`_, and a brief summary of the package's goals is available in the `PyCUTEst journal article <https://doi.org/10.21105/joss.04377>`_.
 
 Requirements
 ------------
 PyCUTEst requires the following software to be installed:
 
 * Python 3 (http://www.python.org/)
+* Python 3 Headers (:code:`apt install python3-dev` on Ubuntu, already included on macOS)
 * CUTEst (see below)
 
 **Please Note:** Currently PyCUTEst only supports Mac and Linux. For Windows 10 (or later), PyCUTEst can be used through the `Windows Subsystem for Linux <https://docs.microsoft.com/en-us/windows/wsl/>`_, following the Linux installation instructions.
 
 Installing CUTEst on Linux
 --------------------------
 These instructions do not include installation of the MATLAB interface. You will need to install four packages: archdefs, SIFDecode, CUTEst and MASTSIF. To keep things simple, install all four packages in the same directory:
```

### Comparing `pycutest-1.6.2/pyproject.toml` & `pycutest-1.7.0/pyproject.toml`

 * *Files identical despite different names*

