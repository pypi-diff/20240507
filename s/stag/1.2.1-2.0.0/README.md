# Comparing `tmp/stag-1.2.1.tar.gz` & `tmp/stag-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stag-1.2.1.tar", last modified: Wed Mar 22 14:34:30 2023, max compression
+gzip compressed data, was "stag-2.0.0.tar", last modified: Tue May  7 10:47:59 2024, max compression
```

## Comparing `stag-1.2.1.tar` & `stag-2.0.0.tar`

### file list

```diff
@@ -1,1786 +1,72 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 14:34:30.665841 stag-1.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-03-22 14:34:02.000000 stag-1.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-03-22 14:34:02.000000 stag-1.2.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      757 2023-03-22 14:34:30.665841 stag-1.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-03-22 14:34:02.000000 stag-1.2.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-22 14:34:30.665841 stag-1.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2870 2023-03-22 14:34:02.000000 stag-1.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 14:34:30.489841 stag-1.2.1/stag/
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-03-22 14:34:02.000000 stag-1.2.1/stag/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8429 2023-03-22 14:34:02.000000 stag-1.2.1/stag/cluster.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 14:34:30.497841 stag-1.2.1/stag/eigen-3.3.9/
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-03-22 14:34:02.000000 stag-1.2.1/stag/eigen-3.3.9/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-03-22 14:34:02.000000 stag-1.2.1/stag/eigen-3.3.9/.hgeol
--rw-r--r--   0 runner    (1001) docker     (123)    24537 2023-03-22 14:34:02.000000 stag-1.2.1/stag/eigen-3.3.9/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-03-22 14:34:02.000000 stag-1.2.1/stag/eigen-3.3.9/COPYING.BSD
--rw-r--r--   0 runner    (1001) docker     (123)    35147 2023-03-22 14:34:02.000000 stag-1.2.1/stag/eigen-3.3.9/COPYING.GPL
--rw-r--r--   0 runner    (1001) docker     (123)    26530 2023-03-22 14:34:02.000000 stag-1.2.1/stag/eigen-3.3.9/COPYING.LGPL
--rw-r--r--   0 runner    (1001) docker     (123)     2246 2023-03-22 14:34:02.000000 stag-1.2.1/stag/eigen-3.3.9/COPYING.MINPACK
--rw-r--r--   0 runner    (1001) docker     (123)    16726 2023-03-22 14:34:02.000000 stag-1.2.1/stag/eigen-3.3.9/COPYING.MPL2
--rw-r--r--   0 runner    (1001) docker     (123)      779 2023-03-22 14:34:02.000000 stag-1.2.1/stag/eigen-3.3.9/COPYING.README
--rw-r--r--   0 runner    (1001) docker     (123)      527 2023-03-22 14:34:02.000000 stag-1.2.1/stag/eigen-3.3.9/CTestConfig.cmake
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-03-22 14:34:02.000000 stag-1.2.1/stag/eigen-3.3.9/CTestCustom.cmake.in
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 14:34:30.501841 stag-1.2.1/stag/eigen-3.3.9/Eigen/
--rw-r--r--   0 runner    (1001) docker     (123)      694 2023-03-22 14:34:02.000000 stag-1.2.1/stag/eigen-3.3.9/Eigen/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-03-22 14:34:02.000000 stag-1.2.1/stag/eigen-3.3.9/Eigen/Cholesky
--rw-r--r--   0 runner    (1001) docker     (123)     1900 2023-03-22 14:34:02.000000 stag-1.2.1/stag/eigen-3.3.9/Eigen/CholmodSupport
--rw-r--r--   0 runner    (1001) docker     (123)    18103 2023-03-22 14:34:02.000000 stag-1.2.1/stag/eigen-3.3.9/Eigen/Core
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-03-22 14:34:02.000000 stag-1.2.1/stag/eigen-3.3.9/Eigen/Dense
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-03-22 14:34:02.000000 stag-1.2.1/stag/eigen-3.3.9/Eigen/Eigen
--rw-r--r--   0 runner    (1001) docker     (123)     1822 2023-03-22 14:34:02.000000 stag-1.2.1/stag/eigen-3.3.9/Eigen/Eigenvalues
--rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-03-22 14:34:02.000000 stag-1.2.1/stag/eigen-3.3.9/Eigen/Geometry
--rw-r--r--   0 runner    (1001) docker     (123)      874 2023-03-22 14:34:02.000000 stag-1.2.1/stag/eigen-3.3.9/Eigen/Householder
--rw-r--r--   0 runner    (1001) docker     (123)     2083 2023-03-22 14:34:02.000000 stag-1.2.1/stag/eigen-3.3.9/Eigen/IterativeLinearSolvers
--rw-r--r--   0 runner    (1001) docker     (123)      939 2023-03-22 14:34:02.000000 stag-1.2.1/stag/eigen-3.3.9/Eigen/Jacobi
--rw-r--r--   0 runner    (1001) docker     (123)     1433 2023-03-22 14:34:02.000000 stag-1.2.1/stag/eigen-3.3.9/Eigen/LU
--rw-r--r--   0 runner    (1001) docker     (123)      991 2023-03-22 14:34:02.000000 stag-1.2.1/stag/eigen-3.3.9/Eigen/MetisSupport
--rw-r--r--   0 runner    (1001) docker     (123)     2483 2023-03-22 14:34:02.000000 stag-1.2.1/stag/eigen-3.3.9/Eigen/OrderingMethods
--rw-r--r--   0 runner    (1001) docker     (123)     1676 2023-03-22 14:34:02.000000 stag-1.2.1/stag/eigen-3.3.9/Eigen/PaStiXSupport
--rwxr-xr-x   0 runner    (1001) docker     (123)     1116 2023-03-22 14:34:02.000000 stag-1.2.1/stag/eigen-3.3.9/Eigen/PardisoSupport
--rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-03-22 14:34:02.000000 stag-1.2.1/stag/eigen-3.3.9/Eigen/QR
--rw-r--r--   0 runner    (1001) docker     (123)      945 2023-03-22 14:34:02.000000 stag-1.2.1/stag/eigen-3.3.9/Eigen/QtAlignedMalloc
--rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-03-22 14:34:02.000000 stag-1.2.1/stag/eigen-3.3.9/Eigen/SPQRSupport
--rw-r--r--   0 runner    (1001) docker     (123)     1629 2023-03-22 14:34:02.000000 stag-1.2.1/stag/eigen-3.3.9/Eigen/SVD
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-03-22 14:34:02.000000 stag-1.2.1/stag/eigen-3.3.9/Eigen/Sparse
--rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-03-22 14:34:02.000000 stag-1.2.1/stag/eigen-3.3.9/Eigen/SparseCholesky
--rw-r--r--   0 runner    (1001) docker     (123)     2240 2023-03-22 14:34:02.000000 stag-1.2.1/stag/eigen-3.3.9/Eigen/SparseCore
--rw-r--r--   0 runner    (1001) docker     (123)     1713 2023-03-22 14:34:02.000000 stag-1.2.1/stag/eigen-3.3.9/Eigen/SparseLU
--rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-03-22 14:34:02.000000 stag-1.2.1/stag/eigen-3.3.9/Eigen/SparseQR
--rw-r--r--   0 runner    (1001) docker     (123)      797 2023-03-22 14:34:02.000000 stag-1.2.1/stag/eigen-3.3.9/Eigen/StdDeque
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-03-22 14:34:02.000000 stag-1.2.1/stag/eigen-3.3.9/Eigen/StdList
--rw-r--r--   0 runner    (1001) docker     (123)      803 2023-03-22 14:34:02.000000 stag-1.2.1/stag/eigen-3.3.9/Eigen/StdVector
--rw-r--r--   0 runner    (1001) docker     (123)     2243 2023-03-22 14:34:02.000000 stag-1.2.1/stag/eigen-3.3.9/Eigen/SuperLUSupport
--rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-03-22 14:34:02.000000 stag-1.2.1/stag/eigen-3.3.9/Eigen/UmfPackSupport
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 14:34:30.485841 stag-1.2.1/stag/eigen-3.3.9/Eigen/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 14:34:30.501841 stag-1.2.1/stag/eigen-3.3.9/Eigen/src/Cholesky/
--rw-r--r--   0 runner    (1001) docker     (123)    24480 2023-03-22 14:34:02.000000 stag-1.2.1/stag/eigen-3.3.9/Eigen/src/Cholesky/LDLT.h
--rw-r--r--   0 runner    (1001) docker     (123)    18395 2023-03-22 14:34:02.000000 stag-1.2.1/stag/eigen-3.3.9/Eigen/src/Cholesky/LLT.h
--rw-r--r--   0 runner    (1001) docker     (123)     3974 2023-03-22 14:34:02.000000 stag-1.2.1/stag/eigen-3.3.9/Eigen/src/Cholesky/LLT_LAPACKE.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 14:34:30.501841 stag-1.2.1/stag/eigen-3.3.9/Eigen/src/CholmodSupport/
--rw-r--r--   0 runner    (1001) docker     (123)    22307 2023-03-22 14:34:02.000000 stag-1.2.1/stag/eigen-3.3.9/Eigen/src/CholmodSupport/CholmodSupport.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 14:34:30.509841 stag-1.2.1/stag/eigen-3.3.9/Eigen/src/Core/
--rw-r--r--   0 runner    (1001) docker     (123)    12115 2023-03-22 14:34:02.000000 stag-1.2.1/stag/eigen-3.3.9/Eigen/src/Core/Array.h
--rw-r--r--   0 runner    (1001) docker     (123)     8237 2023-03-22 14:34:02.000000 stag-1.2.1/stag/eigen-3.3.9/Eigen/src/Core/ArrayBase.h
--rw-r--r--   0 runner    (1001) docker     (123)     6775 2023-03-22 14:34:02.000000 stag-1.2.1/stag/eigen-3.3.9/Eigen/src/Core/ArrayWrapper.h
--rw-r--r--   0 runner    (1001) docker     (123)     2720 2023-03-22 14:34:02.000000 stag-1.2.1/stag/eigen-3.3.9/Eigen/src/Core/Assign.h
--rw-r--r--   0 runner    (1001) docker     (123)    38153 2023-03-22 14:34:02.000000 stag-1.2.1/stag/eigen-3.3.9/Eigen/src/Core/AssignEvaluator.h
--rwxr-xr-x   0 runner    (1001) docker     (123)    12479 2023-03-22 14:34:02.000000 stag-1.2.1/stag/eigen-3.3.9/Eigen/src/Core/Assign_MKL.h
--rw-r--r--   0 runner    (1001) docker     (123)    13910 2023-03-22 14:34:02.000000 stag-1.2.1/stag/eigen-3.3.9/Eigen/src/Core/BandMatrix.h
--rw-r--r--   0 runner    (1001) docker     (123)    18064 2023-03-22 14:34:02.000000 stag-1.2.1/stag/eigen-3.3.9/Eigen/src/Core/Block.h
--rw-r--r--   0 runner    (1001) docker     (123)     4249 2023-03-22 14:34:02.000000 stag-1.2.1/stag/eigen-3.3.9/Eigen/src/Core/BooleanRedux.h
--rw-r--r--   0 runner    (1001) docker     (123)     5689 2023-03-22 14:34:02.000000 stag-1.2.1/stag/eigen-3.3.9/Eigen/src/Core/CommaInitializer.h
--rw-r--r--   0 runner    (1001) docker     (123)     6990 2023-03-22 14:34:02.000000 stag-1.2.1/stag/eigen-3.3.9/Eigen/src/Core/ConditionEstimator.h
--rw-r--r--   0 runner    (1001) docker     (123)    62197 2023-03-22 14:34:02.000000 stag-1.2.1/stag/eigen-3.3.9/Eigen/src/Core/CoreEvaluators.h
--rw-r--r--   0 runner    (1001) docker     (123)     4525 2023-03-22 14:34:02.000000 stag-1.2.1/stag/eigen-3.3.9/Eigen/src/Core/CoreIterators.h
--rw-r--r--   0 runner    (1001) docker     (123)     7593 2023-03-22 14:34:02.000000 stag-1.2.1/stag/eigen-3.3.9/Eigen/src/Core/CwiseBinaryOp.h
--rw-r--r--   0 runner    (1001) docker     (123)    31424 2023-03-22 14:34:02.000000 stag-1.2.1/stag/eigen-3.3.9/Eigen/src/Core/CwiseNullaryOp.h
--rw-r--r--   0 runner    (1001) docker     (123)     8256 2023-03-22 14:34:02.000000 stag-1.2.1/stag/eigen-3.3.9/Eigen/src/Core/CwiseTernaryOp.h
--rw-r--r--   0 runner    (1001) docker     (123)     3877 2023-03-22 14:34:02.000000 stag-1.2.1/stag/eigen-3.3.9/Eigen/src/Core/CwiseUnaryOp.h
--rw-r--r--   0 runner    (1001) docker     (123)     5366 2023-03-22 14:34:02.000000 stag-1.2.1/stag/eigen-3.3.9/Eigen/src/Core/CwiseUnaryView.h
--rw-r--r--   0 runner    (1001) docker     (123)    27551 2023-03-22 14:34:02.000000 stag-1.2.1/stag/eigen-3.3.9/Eigen/src/Core/DenseBase.h
--rw-r--r--   0 runner    (1001) docker     (123)    24212 2023-03-22 14:34:02.000000 stag-1.2.1/stag/eigen-3.3.9/Eigen/src/Core/DenseCoeffsBase.h
--rw-r--r--   0 runner    (1001) docker     (123)    22205 2023-03-22 14:34:02.000000 stag-1.2.1/stag/eigen-3.3.9/Eigen/src/Core/DenseStorage.h
--rw-r--r--   0 runner    (1001) docker     (123)     9597 2023-03-22 14:34:02.000000 stag-1.2.1/stag/eigen-3.3.9/Eigen/src/Core/Diagonal.h
--rw-r--r--   0 runner    (1001) docker     (123)    12666 2023-03-22 14:34:02.000000 stag-1.2.1/stag/eigen-3.3.9/Eigen/src/Core/DiagonalMatrix.h
--rw-r--r--   0 runner    (1001) docker     (123)      970 2023-03-22 14:34:02.000000 stag-1.2.1/stag/eigen-3.3.9/Eigen/src/Core/DiagonalProduct.h
--rw-r--r--   0 runner    (1001) docker     (123)    11507 2023-03-22 14:34:02.000000 stag-1.2.1/stag/eigen-3.3.9/Eigen/src/Core/Dot.h
--rw-r--r--   0 runner    (1001) docker     (123)     5619 2023-03-22 14:34:02.000000 stag-1.2.1/stag/eigen-3.3.9/Eigen/src/Core/EigenBase.h
--rw-r--r--   0 runner    (1001) docker     (123)     4769 2023-03-22 14:34:02.000000 stag-1.2.1/stag/eigen-3.3.9/Eigen/src/Core/ForceAlignedAccess.h
--rw-r--r--   0 runner    (1001) docker     (123)     5705 2023-03-22 14:34:02.000000 stag-1.2.1/stag/eigen-3.3.9/Eigen/src/Core/Fuzzy.h
--rw-r--r--   0 runner    (1001) docker     (123)    21123 2023-03-22 14:34:02.000000 stag-1.2.1/stag/eigen-3.3.9/Eigen/src/Core/GeneralProduct.h
--rw-r--r--   0 runner    (1001) docker     (123)    22069 2023-03-22 14:34:02.000000 stag-1.2.1/stag/eigen-3.3.9/Eigen/src/Core/GenericPacketMath.h
--rw-r--r--   0 runner    (1001) docker     (123)    10222 2023-03-22 14:34:02.000000 stag-1.2.1/stag/eigen-3.3.9/Eigen/src/Core/GlobalFunctions.h
--rw-r--r--   0 runner    (1001) docker     (123)     7076 2023-03-22 14:34:02.000000 stag-1.2.1/stag/eigen-3.3.9/Eigen/src/Core/IO.h
--rw-r--r--   0 runner    (1001) docker     (123)     3519 2023-03-22 14:34:02.000000 stag-1.2.1/stag/eigen-3.3.9/Eigen/src/Core/Inverse.h
--rw-r--r--   0 runner    (1001) docker     (123)     7239 2023-03-22 14:34:02.000000 stag-1.2.1/stag/eigen-3.3.9/Eigen/src/Core/Map.h
--rw-r--r--   0 runner    (1001) docker     (123)    11212 2023-03-22 14:34:02.000000 stag-1.2.1/stag/eigen-3.3.9/Eigen/src/Core/MapBase.h
--rw-r--r--   0 runner    (1001) docker     (123)    41000 2023-03-22 14:34:02.000000 stag-1.2.1/stag/eigen-3.3.9/Eigen/src/Core/MathFunctions.h
--rw-r--r--   0 runner    (1001) docker     (123)     3369 2023-03-22 14:34:02.000000 stag-1.2.1/stag/eigen-3.3.9/Eigen/src/Core/MathFunctionsImpl.h
--rw-r--r--   0 runner    (1001) docker     (123)    19067 2023-03-22 14:34:02.000000 stag-1.2.1/stag/eigen-3.3.9/Eigen/src/Core/Matrix.h
--rw-r--r--   0 runner    (1001) docker     (123)    23276 2023-03-22 14:34:02.000000 stag-1.2.1/stag/eigen-3.3.9/Eigen/src/Core/MatrixBase.h
--rw-r--r--   0 runner    (1001) docker     (123)     3400 2023-03-22 14:34:02.000000 stag-1.2.1/stag/eigen-3.3.9/Eigen/src/Core/NestByValue.h
--rw-r--r--   0 runner    (1001) docker     (123)     3582 2023-03-22 14:34:02.000000 stag-1.2.1/stag/eigen-3.3.9/Eigen/src/Core/NoAlias.h
--rw-r--r--   0 runner    (1001) docker     (123)     9234 2023-03-22 14:34:02.000000 stag-1.2.1/stag/eigen-3.3.9/Eigen/src/Core/NumTraits.h
--rw-r--r--   0 runner    (1001) docker     (123)    20694 2023-03-22 14:34:02.000000 stag-1.2.1/stag/eigen-3.3.9/Eigen/src/Core/PermutationMatrix.h
--rw-r--r--   0 runner    (1001) docker     (123)    45354 2023-03-22 14:34:02.000000 stag-1.2.1/stag/eigen-3.3.9/Eigen/src/Core/PlainObjectBase.h
--rw-r--r--   0 runner    (1001) docker     (123)     7235 2023-03-22 14:34:02.000000 stag-1.2.1/stag/eigen-3.3.9/Eigen/src/Core/Product.h
--rw-r--r--   0 runner    (1001) docker     (123)    51070 2023-03-22 14:34:02.000000 stag-1.2.1/stag/eigen-3.3.9/Eigen/src/Core/ProductEvaluators.h
--rw-r--r--   0 runner    (1001) docker     (123)     6379 2023-03-22 14:34:02.000000 stag-1.2.1/stag/eigen-3.3.9/Eigen/src/Core/Random.h
--rw-r--r--   0 runner    (1001) docker     (123)    17852 2023-03-22 14:34:02.000000 stag-1.2.1/stag/eigen-3.3.9/Eigen/src/Core/Redux.h
--rw-r--r--   0 runner    (1001) docker     (123)    12844 2023-03-22 14:34:02.000000 stag-1.2.1/stag/eigen-3.3.9/Eigen/src/Core/Ref.h
--rw-r--r--   0 runner    (1001) docker     (123)     5595 2023-03-22 14:34:02.000000 stag-1.2.1/stag/eigen-3.3.9/Eigen/src/Core/Replicate.h
--rw-r--r--   0 runner    (1001) docker     (123)     4200 2023-03-22 14:34:02.000000 stag-1.2.1/stag/eigen-3.3.9/Eigen/src/Core/ReturnByValue.h
--rw-r--r--   0 runner    (1001) docker     (123)     7073 2023-03-22 14:34:02.000000 stag-1.2.1/stag/eigen-3.3.9/Eigen/src/Core/Reverse.h
--rw-r--r--   0 runner    (1001) docker     (123)     6020 2023-03-22 14:34:02.000000 stag-1.2.1/stag/eigen-3.3.9/Eigen/src/Core/Select.h
--rw-r--r--   0 runner    (1001) docker     (123)    14245 2023-03-22 14:34:02.000000 stag-1.2.1/stag/eigen-3.3.9/Eigen/src/Core/SelfAdjointView.h
--rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-03-22 14:34:02.000000 stag-1.2.1/stag/eigen-3.3.9/Eigen/src/Core/SelfCwiseBinaryOp.h
--rw-r--r--   0 runner    (1001) docker     (123)     6795 2023-03-22 14:34:02.000000 stag-1.2.1/stag/eigen-3.3.9/Eigen/src/Core/Solve.h
--rw-r--r--   0 runner    (1001) docker     (123)     9208 2023-03-22 14:34:02.000000 stag-1.2.1/stag/eigen-3.3.9/Eigen/src/Core/SolveTriangular.h
--rw-r--r--   0 runner    (1001) docker     (123)     4365 2023-03-22 14:34:02.000000 stag-1.2.1/stag/eigen-3.3.9/Eigen/src/Core/SolverBase.h
--rw-r--r--   0 runner    (1001) docker     (123)     7692 2023-03-22 14:34:02.000000 stag-1.2.1/stag/eigen-3.3.9/Eigen/src/Core/StableNorm.h
--rw-r--r--   0 runner    (1001) docker     (123)     3865 2023-03-22 14:34:02.000000 stag-1.2.1/stag/eigen-3.3.9/Eigen/src/Core/Stride.h
--rw-r--r--   0 runner    (1001) docker     (123)     2683 2023-03-22 14:34:02.000000 stag-1.2.1/stag/eigen-3.3.9/Eigen/src/Core/Swap.h
--rw-r--r--   0 runner    (1001) docker     (123)    14856 2023-03-22 14:34:02.000000 stag-1.2.1/stag/eigen-3.3.9/Eigen/src/Core/Transpose.h
--rw-r--r--   0 runner    (1001) docker     (123)    13092 2023-03-22 14:34:02.000000 stag-1.2.1/stag/eigen-3.3.9/Eigen/src/Core/Transpositions.h
--rw-r--r--   0 runner    (1001) docker     (123)    37304 2023-03-22 14:34:02.000000 stag-1.2.1/stag/eigen-3.3.9/Eigen/src/Core/TriangularMatrix.h
--rw-r--r--   0 runner    (1001) docker     (123)     3462 2023-03-22 14:34:02.000000 stag-1.2.1/stag/eigen-3.3.9/Eigen/src/Core/VectorBlock.h
--rw-r--r--   0 runner    (1001) docker     (123)    29441 2023-03-22 14:34:02.000000 stag-1.2.1/stag/eigen-3.3.9/Eigen/src/Core/VectorwiseOp.h
--rw-r--r--   0 runner    (1001) docker     (123)     8074 2023-03-22 14:34:02.000000 stag-1.2.1/stag/eigen-3.3.9/Eigen/src/Core/Visitor.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 14:34:30.477841 stag-1.2.1/stag/eigen-3.3.9/Eigen/src/Core/arch/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 14:34:30.509841 stag-1.2.1/stag/eigen-3.3.9/Eigen/src/Core/arch/AVX/
--rw-r--r--   0 runner    (1001) docker     (123)    18037 2023-03-22 14:34:02.000000 stag-1.2.1/stag/eigen-3.3.9/Eigen/src/Core/arch/AVX/Complex.h
--rw-r--r--   0 runner    (1001) docker     (123)    17776 2023-03-22 14:34:02.000000 stag-1.2.1/stag/eigen-3.3.9/Eigen/src/Core/arch/AVX/MathFunctions.h
--rw-r--r--   0 runner    (1001) docker     (123)    27841 2023-03-22 14:34:02.000000 stag-1.2.1/stag/eigen-3.3.9/Eigen/src/Core/arch/AVX/PacketMath.h
--rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-03-22 14:34:02.000000 stag-1.2.1/stag/eigen-3.3.9/Eigen/src/Core/arch/AVX/TypeCasting.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 14:34:30.509841 stag-1.2.1/stag/eigen-3.3.9/Eigen/src/Core/arch/AVX512/
--rw-r--r--   0 runner    (1001) docker     (123)    15528 2023-03-22 14:34:02.000000 stag-1.2.1/stag/eigen-3.3.9/Eigen/src/Core/arch/AVX512/MathFunctions.h
--rw-r--r--   0 runner    (1001) docker     (123)    50865 2023-03-22 14:34:02.000000 stag-1.2.1/stag/eigen-3.3.9/Eigen/src/Core/arch/AVX512/PacketMath.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 14:34:30.513841 stag-1.2.1/stag/eigen-3.3.9/Eigen/src/Core/arch/AltiVec/
--rw-r--r--   0 runner    (1001) docker     (123)    16443 2023-03-22 14:34:02.000000 stag-1.2.1/stag/eigen-3.3.9/Eigen/src/Core/arch/AltiVec/Complex.h
--rw-r--r--   0 runner    (1001) docker     (123)    10797 2023-03-22 14:34:02.000000 stag-1.2.1/stag/eigen-3.3.9/Eigen/src/Core/arch/AltiVec/MathFunctions.h
--rwxr-xr-x   0 runner    (1001) docker     (123)    37671 2023-03-22 14:34:02.000000 stag-1.2.1/stag/eigen-3.3.9/Eigen/src/Core/arch/AltiVec/PacketMath.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 14:34:30.517841 stag-1.2.1/stag/eigen-3.3.9/Eigen/src/Core/arch/CUDA/
--rw-r--r--   0 runner    (1001) docker     (123)     4240 2023-03-22 14:34:02.000000 stag-1.2.1/stag/eigen-3.3.9/Eigen/src/Core/arch/CUDA/Complex.h
--rw-r--r--   0 runner    (1001) docker     (123)    23547 2023-03-22 14:34:02.000000 stag-1.2.1/stag/eigen-3.3.9/Eigen/src/Core/arch/CUDA/Half.h
--rw-r--r--   0 runner    (1001) docker     (123)     2387 2023-03-22 14:34:02.000000 stag-1.2.1/stag/eigen-3.3.9/Eigen/src/Core/arch/CUDA/MathFunctions.h
--rw-r--r--   0 runner    (1001) docker     (123)    10744 2023-03-22 14:34:02.000000 stag-1.2.1/stag/eigen-3.3.9/Eigen/src/Core/arch/CUDA/PacketMath.h
--rw-r--r--   0 runner    (1001) docker     (123)    35476 2023-03-22 14:34:02.000000 stag-1.2.1/stag/eigen-3.3.9/Eigen/src/Core/arch/CUDA/PacketMathHalf.h
--rw-r--r--   0 runner    (1001) docker     (123)     5509 2023-03-22 14:34:02.000000 stag-1.2.1/stag/eigen-3.3.9/Eigen/src/Core/arch/CUDA/TypeCasting.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 14:34:30.517841 stag-1.2.1/stag/eigen-3.3.9/Eigen/src/Core/arch/Default/
--rw-r--r--   0 runner    (1001) docker     (123)     1989 2023-03-22 14:34:02.000000 stag-1.2.1/stag/eigen-3.3.9/Eigen/src/Core/arch/Default/ConjHelper.h
--rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-03-22 14:34:02.000000 stag-1.2.1/stag/eigen-3.3.9/Eigen/src/Core/arch/Default/Settings.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 14:34:30.517841 stag-1.2.1/stag/eigen-3.3.9/Eigen/src/Core/arch/NEON/
--rw-r--r--   0 runner    (1001) docker     (123)    17706 2023-03-22 14:34:02.000000 stag-1.2.1/stag/eigen-3.3.9/Eigen/src/Core/arch/NEON/Complex.h
--rw-r--r--   0 runner    (1001) docker     (123)     2846 2023-03-22 14:34:02.000000 stag-1.2.1/stag/eigen-3.3.9/Eigen/src/Core/arch/NEON/MathFunctions.h
--rw-r--r--   0 runner    (1001) docker     (123)    28726 2023-03-22 14:34:02.000000 stag-1.2.1/stag/eigen-3.3.9/Eigen/src/Core/arch/NEON/PacketMath.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 14:34:30.517841 stag-1.2.1/stag/eigen-3.3.9/Eigen/src/Core/arch/SSE/
--rw-r--r--   0 runner    (1001) docker     (123)    19426 2023-03-22 14:34:02.000000 stag-1.2.1/stag/eigen-3.3.9/Eigen/src/Core/arch/SSE/Complex.h
--rw-r--r--   0 runner    (1001) docker     (123)    18888 2023-03-22 14:34:02.000000 stag-1.2.1/stag/eigen-3.3.9/Eigen/src/Core/arch/SSE/MathFunctions.h
--rwxr-xr-x   0 runner    (1001) docker     (123)    35843 2023-03-22 14:34:02.000000 stag-1.2.1/stag/eigen-3.3.9/Eigen/src/Core/arch/SSE/PacketMath.h
--rw-r--r--   0 runner    (1001) docker     (123)     1759 2023-03-22 14:34:02.000000 stag-1.2.1/stag/eigen-3.3.9/Eigen/src/Core/arch/SSE/TypeCasting.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 14:34:30.517841 stag-1.2.1/stag/eigen-3.3.9/Eigen/src/Core/arch/ZVector/
--rw-r--r--   0 runner    (1001) docker     (123)    15366 2023-03-22 14:34:02.000000 stag-1.2.1/stag/eigen-3.3.9/Eigen/src/Core/arch/ZVector/Complex.h
--rw-r--r--   0 runner    (1001) docker     (123)     4418 2023-03-22 14:34:02.000000 stag-1.2.1/stag/eigen-3.3.9/Eigen/src/Core/arch/ZVector/MathFunctions.h
--rwxr-xr-x   0 runner    (1001) docker     (123)    32283 2023-03-22 14:34:02.000000 stag-1.2.1/stag/eigen-3.3.9/Eigen/src/Core/arch/ZVector/PacketMath.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 14:34:30.517841 stag-1.2.1/stag/eigen-3.3.9/Eigen/src/Core/functors/
--rw-r--r--   0 runner    (1001) docker     (123)     6284 2023-03-22 14:34:02.000000 stag-1.2.1/stag/eigen-3.3.9/Eigen/src/Core/functors/AssignmentFunctors.h
--rw-r--r--   0 runner    (1001) docker     (123)    18263 2023-03-22 14:34:02.000000 stag-1.2.1/stag/eigen-3.3.9/Eigen/src/Core/functors/BinaryFunctors.h
--rw-r--r--   0 runner    (1001) docker     (123)     8229 2023-03-22 14:34:02.000000 stag-1.2.1/stag/eigen-3.3.9/Eigen/src/Core/functors/NullaryFunctors.h
--rw-r--r--   0 runner    (1001) docker     (123)     4400 2023-03-22 14:34:02.000000 stag-1.2.1/stag/eigen-3.3.9/Eigen/src/Core/functors/StlFunctors.h
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-03-22 14:34:02.000000 stag-1.2.1/stag/eigen-3.3.9/Eigen/src/Core/functors/TernaryFunctors.h
--rw-r--r--   0 runner    (1001) docker     (123)    27946 2023-03-22 14:34:02.000000 stag-1.2.1/stag/eigen-3.3.9/Eigen/src/Core/functors/UnaryFunctors.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 14:34:30.521841 stag-1.2.1/stag/eigen-3.3.9/Eigen/src/Core/products/
--rw-r--r--   0 runner    (1001) docker     (123)    81646 2023-03-22 14:34:02.000000 stag-1.2.1/stag/eigen-3.3.9/Eigen/src/Core/products/GeneralBlockPanelKernel.h
--rw-r--r--   0 runner    (1001) docker     (123)    18887 2023-03-22 14:34:02.000000 stag-1.2.1/stag/eigen-3.3.9/Eigen/src/Core/products/GeneralMatrixMatrix.h
--rw-r--r--   0 runner    (1001) docker     (123)    15898 2023-03-22 14:34:02.000000 stag-1.2.1/stag/eigen-3.3.9/Eigen/src/Core/products/GeneralMatrixMatrixTriangular.h
--rw-r--r--   0 runner    (1001) docker     (123)     6937 2023-03-22 14:34:02.000000 stag-1.2.1/stag/eigen-3.3.9/Eigen/src/Core/products/GeneralMatrixMatrixTriangular_BLAS.h
--rw-r--r--   0 runner    (1001) docker     (123)     5106 2023-03-22 14:34:02.000000 stag-1.2.1/stag/eigen-3.3.9/Eigen/src/Core/products/GeneralMatrixMatrix_BLAS.h
--rw-r--r--   0 runner    (1001) docker     (123)    26808 2023-03-22 14:34:02.000000 stag-1.2.1/stag/eigen-3.3.9/Eigen/src/Core/products/GeneralMatrixVector.h
--rw-r--r--   0 runner    (1001) docker     (123)     6368 2023-03-22 14:34:02.000000 stag-1.2.1/stag/eigen-3.3.9/Eigen/src/Core/products/GeneralMatrixVector_BLAS.h
--rw-r--r--   0 runner    (1001) docker     (123)     4934 2023-03-22 14:34:02.000000 stag-1.2.1/stag/eigen-3.3.9/Eigen/src/Core/products/Parallelizer.h
--rw-r--r--   0 runner    (1001) docker     (123)    20103 2023-03-22 14:34:02.000000 stag-1.2.1/stag/eigen-3.3.9/Eigen/src/Core/products/SelfadjointMatrixMatrix.h
--rw-r--r--   0 runner    (1001) docker     (123)    11570 2023-03-22 14:34:02.000000 stag-1.2.1/stag/eigen-3.3.9/Eigen/src/Core/products/SelfadjointMatrixMatrix_BLAS.h
--rw-r--r--   0 runner    (1001) docker     (123)     9901 2023-03-22 14:34:02.000000 stag-1.2.1/stag/eigen-3.3.9/Eigen/src/Core/products/SelfadjointMatrixVector.h
--rw-r--r--   0 runner    (1001) docker     (123)     5209 2023-03-22 14:34:02.000000 stag-1.2.1/stag/eigen-3.3.9/Eigen/src/Core/products/SelfadjointMatrixVector_BLAS.h
--rw-r--r--   0 runner    (1001) docker     (123)     6162 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/Eigen/src/Core/products/SelfadjointProduct.h
--rw-r--r--   0 runner    (1001) docker     (123)     4066 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/Eigen/src/Core/products/SelfadjointRank2Update.h
--rw-r--r--   0 runner    (1001) docker     (123)    20879 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/Eigen/src/Core/products/TriangularMatrixMatrix.h
--rw-r--r--   0 runner    (1001) docker     (123)    13867 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/Eigen/src/Core/products/TriangularMatrixMatrix_BLAS.h
--rw-r--r--   0 runner    (1001) docker     (123)    14722 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/Eigen/src/Core/products/TriangularMatrixVector.h
--rw-r--r--   0 runner    (1001) docker     (123)    10571 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/Eigen/src/Core/products/TriangularMatrixVector_BLAS.h
--rw-r--r--   0 runner    (1001) docker     (123)    14540 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/Eigen/src/Core/products/TriangularSolverMatrix.h
--rw-r--r--   0 runner    (1001) docker     (123)     6707 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/Eigen/src/Core/products/TriangularSolverMatrix_BLAS.h
--rw-r--r--   0 runner    (1001) docker     (123)     5741 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/Eigen/src/Core/products/TriangularSolverVector.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 14:34:30.521841 stag-1.2.1/stag/eigen-3.3.9/Eigen/src/Core/util/
--rwxr-xr-x   0 runner    (1001) docker     (123)    19307 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/Eigen/src/Core/util/BlasUtil.h
--rw-r--r--   0 runner    (1001) docker     (123)    21579 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/Eigen/src/Core/util/Constants.h
--rwxr-xr-x   0 runner    (1001) docker     (123)     4360 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/Eigen/src/Core/util/DisableStupidWarnings.h
--rw-r--r--   0 runner    (1001) docker     (123)    14094 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/Eigen/src/Core/util/ForwardDeclarations.h
--rwxr-xr-x   0 runner    (1001) docker     (123)     4026 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/Eigen/src/Core/util/MKL_support.h
--rw-r--r--   0 runner    (1001) docker     (123)    38322 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/Eigen/src/Core/util/Macros.h
--rw-r--r--   0 runner    (1001) docker     (123)    40579 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/Eigen/src/Core/util/Memory.h
--rwxr-xr-x   0 runner    (1001) docker     (123)    21356 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/Eigen/src/Core/util/Meta.h
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/Eigen/src/Core/util/NonMPL2.h
--rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/Eigen/src/Core/util/ReenableStupidWarnings.h
--rw-r--r--   0 runner    (1001) docker     (123)    10518 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/Eigen/src/Core/util/StaticAssert.h
--rw-r--r--   0 runner    (1001) docker     (123)    34903 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/Eigen/src/Core/util/XprHelper.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 14:34:30.521841 stag-1.2.1/stag/eigen-3.3.9/Eigen/src/Eigenvalues/
--rw-r--r--   0 runner    (1001) docker     (123)    12558 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/Eigen/src/Eigenvalues/ComplexEigenSolver.h
--rw-r--r--   0 runner    (1001) docker     (123)    17273 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/Eigen/src/Eigenvalues/ComplexSchur.h
--rw-r--r--   0 runner    (1001) docker     (123)     4178 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/Eigen/src/Eigenvalues/ComplexSchur_LAPACKE.h
--rw-r--r--   0 runner    (1001) docker     (123)    22944 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/Eigen/src/Eigenvalues/EigenSolver.h
--rw-r--r--   0 runner    (1001) docker     (123)    17176 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/Eigen/src/Eigenvalues/GeneralizedEigenSolver.h
--rw-r--r--   0 runner    (1001) docker     (123)     9715 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/Eigen/src/Eigenvalues/GeneralizedSelfAdjointEigenSolver.h
--rw-r--r--   0 runner    (1001) docker     (123)    14351 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/Eigen/src/Eigenvalues/HessenbergDecomposition.h
--rw-r--r--   0 runner    (1001) docker     (123)     5539 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/Eigen/src/Eigenvalues/MatrixBaseEigenvalues.h
--rw-r--r--   0 runner    (1001) docker     (123)    23586 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/Eigen/src/Eigenvalues/RealQZ.h
--rw-r--r--   0 runner    (1001) docker     (123)    20749 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/Eigen/src/Eigenvalues/RealSchur.h
--rw-r--r--   0 runner    (1001) docker     (123)     3650 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/Eigen/src/Eigenvalues/RealSchur_LAPACKE.h
--rw-r--r--   0 runner    (1001) docker     (123)    33705 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/Eigen/src/Eigenvalues/SelfAdjointEigenSolver.h
--rw-r--r--   0 runner    (1001) docker     (123)     4104 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/Eigen/src/Eigenvalues/SelfAdjointEigenSolver_LAPACKE.h
--rw-r--r--   0 runner    (1001) docker     (123)    22444 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/Eigen/src/Eigenvalues/Tridiagonalization.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 14:34:30.525841 stag-1.2.1/stag/eigen-3.3.9/Eigen/src/Geometry/
--rw-r--r--   0 runner    (1001) docker     (123)    14815 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/Eigen/src/Geometry/AlignedBox.h
--rw-r--r--   0 runner    (1001) docker     (123)     8423 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/Eigen/src/Geometry/AngleAxis.h
--rw-r--r--   0 runner    (1001) docker     (123)     3639 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/Eigen/src/Geometry/EulerAngles.h
--rw-r--r--   0 runner    (1001) docker     (123)    20539 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/Eigen/src/Geometry/Homogeneous.h
--rw-r--r--   0 runner    (1001) docker     (123)    11961 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/Eigen/src/Geometry/Hyperplane.h
--rw-r--r--   0 runner    (1001) docker     (123)     8949 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/Eigen/src/Geometry/OrthoMethods.h
--rw-r--r--   0 runner    (1001) docker     (123)     8308 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/Eigen/src/Geometry/ParametrizedLine.h
--rw-r--r--   0 runner    (1001) docker     (123)    32704 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/Eigen/src/Geometry/Quaternion.h
--rw-r--r--   0 runner    (1001) docker     (123)     6877 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/Eigen/src/Geometry/Rotation2D.h
--rw-r--r--   0 runner    (1001) docker     (123)     8063 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/Eigen/src/Geometry/RotationBase.h
--rw-r--r--   0 runner    (1001) docker     (123)     6331 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/Eigen/src/Geometry/Scaling.h
--rw-r--r--   0 runner    (1001) docker     (123)    60555 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/Eigen/src/Geometry/Transform.h
--rw-r--r--   0 runner    (1001) docker     (123)     7664 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/Eigen/src/Geometry/Translation.h
--rw-r--r--   0 runner    (1001) docker     (123)     6190 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/Eigen/src/Geometry/Umeyama.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 14:34:30.525841 stag-1.2.1/stag/eigen-3.3.9/Eigen/src/Geometry/arch/
--rw-r--r--   0 runner    (1001) docker     (123)     5387 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/Eigen/src/Geometry/arch/Geometry_SSE.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 14:34:30.525841 stag-1.2.1/stag/eigen-3.3.9/Eigen/src/Householder/
--rw-r--r--   0 runner    (1001) docker     (123)     4481 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/Eigen/src/Householder/BlockHouseholder.h
--rw-r--r--   0 runner    (1001) docker     (123)     5345 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/Eigen/src/Householder/Householder.h
--rw-r--r--   0 runner    (1001) docker     (123)    20603 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/Eigen/src/Householder/HouseholderSequence.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 14:34:30.525841 stag-1.2.1/stag/eigen-3.3.9/Eigen/src/IterativeLinearSolvers/
--rw-r--r--   0 runner    (1001) docker     (123)     6755 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/Eigen/src/IterativeLinearSolvers/BasicPreconditioners.h
--rw-r--r--   0 runner    (1001) docker     (123)     7253 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/Eigen/src/IterativeLinearSolvers/BiCGSTAB.h
--rw-r--r--   0 runner    (1001) docker     (123)     9289 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/Eigen/src/IterativeLinearSolvers/ConjugateGradient.h
--rw-r--r--   0 runner    (1001) docker     (123)    15062 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/Eigen/src/IterativeLinearSolvers/IncompleteCholesky.h
--rw-r--r--   0 runner    (1001) docker     (123)    15234 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/Eigen/src/IterativeLinearSolvers/IncompleteLUT.h
--rw-r--r--   0 runner    (1001) docker     (123)    11527 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/Eigen/src/IterativeLinearSolvers/IterativeSolverBase.h
--rw-r--r--   0 runner    (1001) docker     (123)     7762 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/Eigen/src/IterativeLinearSolvers/LeastSquareConjugateGradient.h
--rw-r--r--   0 runner    (1001) docker     (123)     4158 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/Eigen/src/IterativeLinearSolvers/SolveWithGuess.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 14:34:30.525841 stag-1.2.1/stag/eigen-3.3.9/Eigen/src/Jacobi/
--rw-r--r--   0 runner    (1001) docker     (123)    15902 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/Eigen/src/Jacobi/Jacobi.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 14:34:30.525841 stag-1.2.1/stag/eigen-3.3.9/Eigen/src/LU/
--rw-r--r--   0 runner    (1001) docker     (123)     3057 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/Eigen/src/LU/Determinant.h
--rw-r--r--   0 runner    (1001) docker     (123)    32803 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/Eigen/src/LU/FullPivLU.h
--rw-r--r--   0 runner    (1001) docker     (123)    15064 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/Eigen/src/LU/InverseImpl.h
--rw-r--r--   0 runner    (1001) docker     (123)    21538 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/Eigen/src/LU/PartialPivLU.h
--rw-r--r--   0 runner    (1001) docker     (123)     3555 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/Eigen/src/LU/PartialPivLU_LAPACKE.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 14:34:30.525841 stag-1.2.1/stag/eigen-3.3.9/Eigen/src/LU/arch/
--rw-r--r--   0 runner    (1001) docker     (123)    13662 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/Eigen/src/LU/arch/Inverse_SSE.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 14:34:30.525841 stag-1.2.1/stag/eigen-3.3.9/Eigen/src/MetisSupport/
--rw-r--r--   0 runner    (1001) docker     (123)     4588 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/Eigen/src/MetisSupport/MetisSupport.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 14:34:30.525841 stag-1.2.1/stag/eigen-3.3.9/Eigen/src/OrderingMethods/
--rw-r--r--   0 runner    (1001) docker     (123)    16396 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/Eigen/src/OrderingMethods/Amd.h
--rw-r--r--   0 runner    (1001) docker     (123)    62266 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/Eigen/src/OrderingMethods/Eigen_Colamd.h
--rw-r--r--   0 runner    (1001) docker     (123)     5229 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/Eigen/src/OrderingMethods/Ordering.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 14:34:30.529841 stag-1.2.1/stag/eigen-3.3.9/Eigen/src/PaStiXSupport/
--rw-r--r--   0 runner    (1001) docker     (123)    22248 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/Eigen/src/PaStiXSupport/PaStiXSupport.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 14:34:30.529841 stag-1.2.1/stag/eigen-3.3.9/Eigen/src/PardisoSupport/
--rw-r--r--   0 runner    (1001) docker     (123)    20060 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/Eigen/src/PardisoSupport/PardisoSupport.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 14:34:30.529841 stag-1.2.1/stag/eigen-3.3.9/Eigen/src/QR/
--rw-r--r--   0 runner    (1001) docker     (123)    24881 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/Eigen/src/QR/ColPivHouseholderQR.h
--rw-r--r--   0 runner    (1001) docker     (123)     4662 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/Eigen/src/QR/ColPivHouseholderQR_LAPACKE.h
--rw-r--r--   0 runner    (1001) docker     (123)    20805 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/Eigen/src/QR/CompleteOrthogonalDecomposition.h
--rw-r--r--   0 runner    (1001) docker     (123)    25478 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/Eigen/src/QR/FullPivHouseholderQR.h
--rw-r--r--   0 runner    (1001) docker     (123)    14022 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/Eigen/src/QR/HouseholderQR.h
--rw-r--r--   0 runner    (1001) docker     (123)     2993 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/Eigen/src/QR/HouseholderQR_LAPACKE.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 14:34:30.529841 stag-1.2.1/stag/eigen-3.3.9/Eigen/src/SPQRSupport/
--rw-r--r--   0 runner    (1001) docker     (123)    11405 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/Eigen/src/SPQRSupport/SuiteSparseQRSupport.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 14:34:30.529841 stag-1.2.1/stag/eigen-3.3.9/Eigen/src/SVD/
--rw-r--r--   0 runner    (1001) docker     (123)    49870 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/Eigen/src/SVD/BDCSVD.h
--rw-r--r--   0 runner    (1001) docker     (123)    32949 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/Eigen/src/SVD/JacobiSVD.h
--rw-r--r--   0 runner    (1001) docker     (123)     5099 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/Eigen/src/SVD/JacobiSVD_LAPACKE.h
--rw-r--r--   0 runner    (1001) docker     (123)    12752 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/Eigen/src/SVD/SVDBase.h
--rw-r--r--   0 runner    (1001) docker     (123)    15957 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/Eigen/src/SVD/UpperBidiagonalization.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 14:34:30.529841 stag-1.2.1/stag/eigen-3.3.9/Eigen/src/SparseCholesky/
--rw-r--r--   0 runner    (1001) docker     (123)    24017 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/Eigen/src/SparseCholesky/SimplicialCholesky.h
--rw-r--r--   0 runner    (1001) docker     (123)     6912 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/Eigen/src/SparseCholesky/SimplicialCholesky_impl.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 14:34:30.533841 stag-1.2.1/stag/eigen-3.3.9/Eigen/src/SparseCore/
--rw-r--r--   0 runner    (1001) docker     (123)    10670 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/Eigen/src/SparseCore/AmbiVector.h
--rw-r--r--   0 runner    (1001) docker     (123)     8164 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/Eigen/src/SparseCore/CompressedStorage.h
--rw-r--r--   0 runner    (1001) docker     (123)    13178 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/Eigen/src/SparseCore/ConservativeSparseSparseProduct.h
--rw-r--r--   0 runner    (1001) docker     (123)     2191 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/Eigen/src/SparseCore/MappedSparseMatrix.h
--rw-r--r--   0 runner    (1001) docker     (123)     8080 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/Eigen/src/SparseCore/SparseAssign.h
--rw-r--r--   0 runner    (1001) docker     (123)    25592 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/Eigen/src/SparseCore/SparseBlock.h
--rw-r--r--   0 runner    (1001) docker     (123)     6485 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/Eigen/src/SparseCore/SparseColEtree.h
--rw-r--r--   0 runner    (1001) docker     (123)    12720 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/Eigen/src/SparseCore/SparseCompressedBase.h
--rw-r--r--   0 runner    (1001) docker     (123)    25840 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/Eigen/src/SparseCore/SparseCwiseBinaryOp.h
--rw-r--r--   0 runner    (1001) docker     (123)     4737 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/Eigen/src/SparseCore/SparseCwiseUnaryOp.h
--rw-r--r--   0 runner    (1001) docker     (123)    12487 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/Eigen/src/SparseCore/SparseDenseProduct.h
--rw-r--r--   0 runner    (1001) docker     (123)     5808 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/Eigen/src/SparseCore/SparseDiagonalProduct.h
--rw-r--r--   0 runner    (1001) docker     (123)     3080 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/Eigen/src/SparseCore/SparseDot.h
--rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/Eigen/src/SparseCore/SparseFuzzy.h
--rw-r--r--   0 runner    (1001) docker     (123)    12589 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/Eigen/src/SparseCore/SparseMap.h
--rw-r--r--   0 runner    (1001) docker     (123)    52401 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/Eigen/src/SparseCore/SparseMatrix.h
--rw-r--r--   0 runner    (1001) docker     (123)    17923 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/Eigen/src/SparseCore/SparseMatrixBase.h
--rw-r--r--   0 runner    (1001) docker     (123)     7329 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/Eigen/src/SparseCore/SparsePermutation.h
--rw-r--r--   0 runner    (1001) docker     (123)     7049 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/Eigen/src/SparseCore/SparseProduct.h
--rw-r--r--   0 runner    (1001) docker     (123)     1699 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/Eigen/src/SparseCore/SparseRedux.h
--rw-r--r--   0 runner    (1001) docker     (123)    15492 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/Eigen/src/SparseCore/SparseRef.h
--rw-r--r--   0 runner    (1001) docker     (123)    25721 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/Eigen/src/SparseCore/SparseSelfAdjointView.h
--rw-r--r--   0 runner    (1001) docker     (123)     4424 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/Eigen/src/SparseCore/SparseSolverBase.h
--rw-r--r--   0 runner    (1001) docker     (123)     8704 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/Eigen/src/SparseCore/SparseSparseProductWithPruning.h
--rw-r--r--   0 runner    (1001) docker     (123)     3175 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/Eigen/src/SparseCore/SparseTranspose.h
--rw-r--r--   0 runner    (1001) docker     (123)     6437 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/Eigen/src/SparseCore/SparseTriangularView.h
--rw-r--r--   0 runner    (1001) docker     (123)     6602 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/Eigen/src/SparseCore/SparseUtil.h
--rw-r--r--   0 runner    (1001) docker     (123)    14831 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/Eigen/src/SparseCore/SparseVector.h
--rw-r--r--   0 runner    (1001) docker     (123)     8127 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/Eigen/src/SparseCore/SparseView.h
--rw-r--r--   0 runner    (1001) docker     (123)     9657 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/Eigen/src/SparseCore/TriangularSolver.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 14:34:30.533841 stag-1.2.1/stag/eigen-3.3.9/Eigen/src/SparseLU/
--rw-r--r--   0 runner    (1001) docker     (123)    27844 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/Eigen/src/SparseLU/SparseLU.h
--rw-r--r--   0 runner    (1001) docker     (123)     4303 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/Eigen/src/SparseLU/SparseLUImpl.h
--rw-r--r--   0 runner    (1001) docker     (123)     7601 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/Eigen/src/SparseLU/SparseLU_Memory.h
--rw-r--r--   0 runner    (1001) docker     (123)     4974 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/Eigen/src/SparseLU/SparseLU_Structs.h
--rw-r--r--   0 runner    (1001) docker     (123)    10022 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/Eigen/src/SparseLU/SparseLU_SupernodalMatrix.h
--rw-r--r--   0 runner    (1001) docker     (123)     2049 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/Eigen/src/SparseLU/SparseLU_Utils.h
--rw-r--r--   0 runner    (1001) docker     (123)     6712 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/Eigen/src/SparseLU/SparseLU_column_bmod.h
--rw-r--r--   0 runner    (1001) docker     (123)     6582 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/Eigen/src/SparseLU/SparseLU_column_dfs.h
--rw-r--r--   0 runner    (1001) docker     (123)     3681 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/Eigen/src/SparseLU/SparseLU_copy_to_ucol.h
--rw-r--r--   0 runner    (1001) docker     (123)    10216 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/Eigen/src/SparseLU/SparseLU_gemm_kernel.h
--rw-r--r--   0 runner    (1001) docker     (123)     4181 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/Eigen/src/SparseLU/SparseLU_heap_relax_snode.h
--rw-r--r--   0 runner    (1001) docker     (123)     5723 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/Eigen/src/SparseLU/SparseLU_kernel_bmod.h
--rw-r--r--   0 runner    (1001) docker     (123)     8486 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/Eigen/src/SparseLU/SparseLU_panel_bmod.h
--rw-r--r--   0 runner    (1001) docker     (123)     9028 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/Eigen/src/SparseLU/SparseLU_panel_dfs.h
--rw-r--r--   0 runner    (1001) docker     (123)     4979 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/Eigen/src/SparseLU/SparseLU_pivotL.h
--rw-r--r--   0 runner    (1001) docker     (123)     4545 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/Eigen/src/SparseLU/SparseLU_pruneL.h
--rw-r--r--   0 runner    (1001) docker     (123)     2889 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/Eigen/src/SparseLU/SparseLU_relax_snode.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 14:34:30.533841 stag-1.2.1/stag/eigen-3.3.9/Eigen/src/SparseQR/
--rw-r--r--   0 runner    (1001) docker     (123)    28373 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/Eigen/src/SparseQR/SparseQR.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 14:34:30.533841 stag-1.2.1/stag/eigen-3.3.9/Eigen/src/StlSupport/
--rw-r--r--   0 runner    (1001) docker     (123)     5279 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/Eigen/src/StlSupport/StdDeque.h
--rw-r--r--   0 runner    (1001) docker     (123)     4147 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/Eigen/src/StlSupport/StdList.h
--rw-r--r--   0 runner    (1001) docker     (123)     5330 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/Eigen/src/StlSupport/StdVector.h
--rw-r--r--   0 runner    (1001) docker     (123)     2809 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/Eigen/src/StlSupport/details.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 14:34:30.533841 stag-1.2.1/stag/eigen-3.3.9/Eigen/src/SuperLUSupport/
--rw-r--r--   0 runner    (1001) docker     (123)    34345 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/Eigen/src/SuperLUSupport/SuperLUSupport.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 14:34:30.533841 stag-1.2.1/stag/eigen-3.3.9/Eigen/src/UmfPackSupport/
--rw-r--r--   0 runner    (1001) docker     (123)    17202 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/Eigen/src/UmfPackSupport/UmfPackSupport.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 14:34:30.537841 stag-1.2.1/stag/eigen-3.3.9/Eigen/src/misc/
--rw-r--r--   0 runner    (1001) docker     (123)     2913 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/Eigen/src/misc/Image.h
--rw-r--r--   0 runner    (1001) docker     (123)     2742 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/Eigen/src/misc/Kernel.h
--rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/Eigen/src/misc/RealSvd2x2.h
--rw-r--r--   0 runner    (1001) docker     (123)    30560 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/Eigen/src/misc/blas.h
--rw-r--r--   0 runner    (1001) docker     (123)     7834 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/Eigen/src/misc/lapack.h
--rwxr-xr-x   0 runner    (1001) docker     (123)  1058368 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/Eigen/src/misc/lapacke.h
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/Eigen/src/misc/lapacke_mangling.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 14:34:30.537841 stag-1.2.1/stag/eigen-3.3.9/Eigen/src/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)    13166 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/Eigen/src/plugins/ArrayCwiseBinaryOps.h
--rw-r--r--   0 runner    (1001) docker     (123)    16929 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/Eigen/src/plugins/ArrayCwiseUnaryOps.h
--rw-r--r--   0 runner    (1001) docker     (123)    37403 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/Eigen/src/plugins/BlockMethods.h
--rw-r--r--   0 runner    (1001) docker     (123)     4828 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/Eigen/src/plugins/CommonCwiseBinaryOps.h
--rw-r--r--   0 runner    (1001) docker     (123)     5621 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/Eigen/src/plugins/CommonCwiseUnaryOps.h
--rw-r--r--   0 runner    (1001) docker     (123)     6375 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/Eigen/src/plugins/MatrixCwiseBinaryOps.h
--rw-r--r--   0 runner    (1001) docker     (123)     2937 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/Eigen/src/plugins/MatrixCwiseUnaryOps.h
--rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/INSTALL
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 14:34:30.541841 stag-1.2.1/stag/eigen-3.3.9/bench/
--rw-r--r--   0 runner    (1001) docker     (123)     3932 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/bench/BenchSparseUtil.h
--rw-r--r--   0 runner    (1001) docker     (123)     4392 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/bench/BenchTimer.h
--rw-r--r--   0 runner    (1001) docker     (123)     2529 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/bench/BenchUtil.h
--rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/bench/README.txt
--rw-r--r--   0 runner    (1001) docker     (123)    28983 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/bench/analyze-blocking-sizes.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/bench/basicbench.cxxlist
--rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/bench/basicbenchmark.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1669 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/bench/basicbenchmark.h
--rw-r--r--   0 runner    (1001) docker     (123)     6313 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/bench/benchBlasGemm.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3534 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/bench/benchCholesky.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     5788 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/bench/benchEigenSolver.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2806 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/bench/benchFFT.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3598 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/bench/benchGeometry.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     5193 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/bench/benchVecAdd.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    10885 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/bench/bench_gemm.cpp
--rwxr-xr-x   0 runner    (1001) docker     (123)      618 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/bench/bench_multi_compilers.sh
--rw-r--r--   0 runner    (1001) docker     (123)    11652 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/bench/bench_norm.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2159 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/bench/bench_reverse.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/bench/bench_sum.cpp
--rwxr-xr-x   0 runner    (1001) docker     (123)      651 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/bench/bench_unrolling
--rw-r--r--   0 runner    (1001) docker     (123)    22259 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/bench/benchmark-blocking-sizes.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      790 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/bench/benchmark.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      835 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/bench/benchmarkSlice.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      640 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/bench/benchmarkX.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      605 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/bench/benchmarkXcwise.cpp
--rwxr-xr-x   0 runner    (1001) docker     (123)     1209 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/bench/benchmark_suite
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 14:34:30.541841 stag-1.2.1/stag/eigen-3.3.9/bench/btl/
--rw-r--r--   0 runner    (1001) docker     (123)     2869 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/bench/btl/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)    18109 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/bench/btl/COPYING
--rw-r--r--   0 runner    (1001) docker     (123)     6447 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/bench/btl/README
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 14:34:30.541841 stag-1.2.1/stag/eigen-3.3.9/bench/btl/actions/
--rw-r--r--   0 runner    (1001) docker     (123)     3374 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/bench/btl/actions/action_aat_product.hh
--rw-r--r--   0 runner    (1001) docker     (123)     3354 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/bench/btl/actions/action_ata_product.hh
--rw-r--r--   0 runner    (1001) docker     (123)     3670 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/bench/btl/actions/action_atv_product.hh
--rw-r--r--   0 runner    (1001) docker     (123)     3371 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/bench/btl/actions/action_axpby.hh
--rw-r--r--   0 runner    (1001) docker     (123)     3340 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/bench/btl/actions/action_axpy.hh
--rw-r--r--   0 runner    (1001) docker     (123)     3202 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/bench/btl/actions/action_cholesky.hh
--rw-r--r--   0 runner    (1001) docker     (123)     3460 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/bench/btl/actions/action_ger.hh
--rw-r--r--   0 runner    (1001) docker     (123)     5598 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/bench/btl/actions/action_hessenberg.hh
--rw-r--r--   0 runner    (1001) docker     (123)     3151 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/bench/btl/actions/action_lu_decomp.hh
--rw-r--r--   0 runner    (1001) docker     (123)     3598 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/bench/btl/actions/action_lu_solve.hh
--rw-r--r--   0 runner    (1001) docker     (123)     3886 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/bench/btl/actions/action_matrix_matrix_product.hh
--rw-r--r--   0 runner    (1001) docker     (123)     3982 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/bench/btl/actions/action_matrix_matrix_product_bis.hh
--rw-r--r--   0 runner    (1001) docker     (123)     3989 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/bench/btl/actions/action_matrix_vector_product.hh
--rw-r--r--   0 runner    (1001) docker     (123)     3188 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/bench/btl/actions/action_partial_lu.hh
--rw-r--r--   0 runner    (1001) docker     (123)     3019 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/bench/btl/actions/action_rot.hh
--rw-r--r--   0 runner    (1001) docker     (123)     3691 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/bench/btl/actions/action_symv.hh
--rw-r--r--   0 runner    (1001) docker     (123)     3664 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/bench/btl/actions/action_syr2.hh
--rw-r--r--   0 runner    (1001) docker     (123)     3425 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/bench/btl/actions/action_trisolve.hh
--rw-r--r--   0 runner    (1001) docker     (123)     4061 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/bench/btl/actions/action_trisolve_matrix.hh
--rw-r--r--   0 runner    (1001) docker     (123)     3907 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/bench/btl/actions/action_trmm.hh
--rw-r--r--   0 runner    (1001) docker     (123)      467 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/bench/btl/actions/basic_actions.hh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 14:34:30.545841 stag-1.2.1/stag/eigen-3.3.9/bench/btl/cmake/
--rw-r--r--   0 runner    (1001) docker     (123)      932 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/bench/btl/cmake/FindACML.cmake
--rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/bench/btl/cmake/FindATLAS.cmake
--rw-r--r--   0 runner    (1001) docker     (123)      815 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/bench/btl/cmake/FindBLAZE.cmake
--rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/bench/btl/cmake/FindBlitz.cmake
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/bench/btl/cmake/FindCBLAS.cmake
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/bench/btl/cmake/FindGMM.cmake
--rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/bench/btl/cmake/FindMKL.cmake
--rw-r--r--   0 runner    (1001) docker     (123)      819 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/bench/btl/cmake/FindMTL4.cmake
--rw-r--r--   0 runner    (1001) docker     (123)      622 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/bench/btl/cmake/FindOPENBLAS.cmake
--rw-r--r--   0 runner    (1001) docker     (123)     2372 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/bench/btl/cmake/FindPackageHandleStandardArgs.cmake
--rw-r--r--   0 runner    (1001) docker     (123)      832 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/bench/btl/cmake/FindTvmet.cmake
--rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/bench/btl/cmake/MacroOptionalAddSubdirectory.cmake
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 14:34:30.545841 stag-1.2.1/stag/eigen-3.3.9/bench/btl/data/
--rw-r--r--   0 runner    (1001) docker     (123)      869 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/bench/btl/data/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/bench/btl/data/action_settings.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2224 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/bench/btl/data/gnuplot_common_settings.hh
--rwxr-xr-x   0 runner    (1001) docker     (123)     2065 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/bench/btl/data/go_mean
--rw-r--r--   0 runner    (1001) docker     (123)     5306 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/bench/btl/data/mean.cxx
--rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/bench/btl/data/mk_gnuplot_script.sh
--rw-r--r--   0 runner    (1001) docker     (123)      929 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/bench/btl/data/mk_mean_script.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)     1742 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/bench/btl/data/mk_new_gnuplot.sh
--rw-r--r--   0 runner    (1001) docker     (123)      974 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/bench/btl/data/perlib_plot_settings.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3425 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/bench/btl/data/regularize.cxx
--rw-r--r--   0 runner    (1001) docker     (123)     5112 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/bench/btl/data/smooth.cxx
--rwxr-xr-x   0 runner    (1001) docker     (123)     1687 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/bench/btl/data/smooth_all.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 14:34:30.545841 stag-1.2.1/stag/eigen-3.3.9/bench/btl/generic_bench/
--rw-r--r--   0 runner    (1001) docker     (123)     4827 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/bench/btl/generic_bench/bench.hh
--rw-r--r--   0 runner    (1001) docker     (123)     1916 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/bench/btl/generic_bench/bench_parameter.hh
--rw-r--r--   0 runner    (1001) docker     (123)     6748 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/bench/btl/generic_bench/btl.hh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 14:34:30.545841 stag-1.2.1/stag/eigen-3.3.9/bench/btl/generic_bench/init/
--rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/bench/btl/generic_bench/init/init_function.hh
--rw-r--r--   0 runner    (1001) docker     (123)     2295 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/bench/btl/generic_bench/init/init_matrix.hh
--rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/bench/btl/generic_bench/init/init_vector.hh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 14:34:30.545841 stag-1.2.1/stag/eigen-3.3.9/bench/btl/generic_bench/static/
--rw-r--r--   0 runner    (1001) docker     (123)     2278 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/bench/btl/generic_bench/static/bench_static.hh
--rw-r--r--   0 runner    (1001) docker     (123)     1948 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/bench/btl/generic_bench/static/intel_bench_fixed_size.hh
--rw-r--r--   0 runner    (1001) docker     (123)     2222 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/bench/btl/generic_bench/static/static_size_generator.hh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 14:34:30.545841 stag-1.2.1/stag/eigen-3.3.9/bench/btl/generic_bench/timers/
--rw-r--r--   0 runner    (1001) docker     (123)     2305 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/bench/btl/generic_bench/timers/STL_perf_analyzer.hh
--rw-r--r--   0 runner    (1001) docker     (123)     2522 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/bench/btl/generic_bench/timers/STL_timer.hh
--rw-r--r--   0 runner    (1001) docker     (123)     1994 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/bench/btl/generic_bench/timers/mixed_perf_analyzer.hh
--rw-r--r--   0 runner    (1001) docker     (123)     2938 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/bench/btl/generic_bench/timers/portable_perf_analyzer.hh
--rw-r--r--   0 runner    (1001) docker     (123)     3534 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/bench/btl/generic_bench/timers/portable_perf_analyzer_old.hh
--rwxr-xr-x   0 runner    (1001) docker     (123)     3534 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/bench/btl/generic_bench/timers/portable_timer.hh
--rw-r--r--   0 runner    (1001) docker     (123)     2927 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/bench/btl/generic_bench/timers/x86_perf_analyzer.hh
--rw-r--r--   0 runner    (1001) docker     (123)     5294 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/bench/btl/generic_bench/timers/x86_timer.hh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 14:34:30.545841 stag-1.2.1/stag/eigen-3.3.9/bench/btl/generic_bench/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/bench/btl/generic_bench/utils/size_lin_log.hh
--rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/bench/btl/generic_bench/utils/size_log.hh
--rw-r--r--   0 runner    (1001) docker     (123)     2745 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/bench/btl/generic_bench/utils/utilities.h
--rw-r--r--   0 runner    (1001) docker     (123)     2213 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/bench/btl/generic_bench/utils/xy_file.hh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 14:34:30.485841 stag-1.2.1/stag/eigen-3.3.9/bench/btl/libs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 14:34:30.545841 stag-1.2.1/stag/eigen-3.3.9/bench/btl/libs/BLAS/
--rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/bench/btl/libs/BLAS/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)    35158 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/bench/btl/libs/BLAS/blas.h
--rw-r--r--   0 runner    (1001) docker     (123)     2891 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/bench/btl/libs/BLAS/blas_interface.hh
--rw-r--r--   0 runner    (1001) docker     (123)     4811 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/bench/btl/libs/BLAS/blas_interface_impl.hh
--rw-r--r--   0 runner    (1001) docker     (123)     1634 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/bench/btl/libs/BLAS/c_interface_base.h
--rw-r--r--   0 runner    (1001) docker     (123)     2963 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/bench/btl/libs/BLAS/main.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 14:34:30.545841 stag-1.2.1/stag/eigen-3.3.9/bench/btl/libs/STL/
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/bench/btl/libs/STL/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5838 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/bench/btl/libs/STL/STL_interface.hh
--rw-r--r--   0 runner    (1001) docker     (123)     1828 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/bench/btl/libs/STL/main.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 14:34:30.549841 stag-1.2.1/stag/eigen-3.3.9/bench/btl/libs/blaze/
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/bench/btl/libs/blaze/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4012 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/bench/btl/libs/blaze/blaze_interface.hh
--rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/bench/btl/libs/blaze/main.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 14:34:30.549841 stag-1.2.1/stag/eigen-3.3.9/bench/btl/libs/blitz/
--rw-r--r--   0 runner    (1001) docker     (123)      424 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/bench/btl/libs/blitz/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5364 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/bench/btl/libs/blitz/blitz_LU_solve_interface.hh
--rw-r--r--   0 runner    (1001) docker     (123)     4129 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/bench/btl/libs/blitz/blitz_interface.hh
--rw-r--r--   0 runner    (1001) docker     (123)     1962 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/bench/btl/libs/blitz/btl_blitz.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1393 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/bench/btl/libs/blitz/btl_tiny_blitz.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3100 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/bench/btl/libs/blitz/tiny_blitz_interface.hh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 14:34:30.549841 stag-1.2.1/stag/eigen-3.3.9/bench/btl/libs/eigen2/
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/bench/btl/libs/eigen2/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1664 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/bench/btl/libs/eigen2/btl_tiny_eigen2.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     5151 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/bench/btl/libs/eigen2/eigen2_interface.hh
--rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/bench/btl/libs/eigen2/main_adv.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/bench/btl/libs/eigen2/main_linear.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/bench/btl/libs/eigen2/main_matmat.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/bench/btl/libs/eigen2/main_vecmat.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 14:34:30.549841 stag-1.2.1/stag/eigen-3.3.9/bench/btl/libs/eigen3/
--rw-r--r--   0 runner    (1001) docker     (123)     3292 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/bench/btl/libs/eigen3/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1664 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/bench/btl/libs/eigen3/btl_tiny_eigen3.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     8077 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/bench/btl/libs/eigen3/eigen3_interface.hh
--rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/bench/btl/libs/eigen3/main_adv.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/bench/btl/libs/eigen3/main_linear.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/bench/btl/libs/eigen3/main_matmat.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/bench/btl/libs/eigen3/main_vecmat.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 14:34:30.549841 stag-1.2.1/stag/eigen-3.3.9/bench/btl/libs/gmm/
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/bench/btl/libs/gmm/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5364 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/bench/btl/libs/gmm/gmm_LU_solve_interface.hh
--rw-r--r--   0 runner    (1001) docker     (123)     4174 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/bench/btl/libs/gmm/gmm_interface.hh
--rw-r--r--   0 runner    (1001) docker     (123)     2113 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/bench/btl/libs/gmm/main.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 14:34:30.549841 stag-1.2.1/stag/eigen-3.3.9/bench/btl/libs/mtl4/
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/bench/btl/libs/mtl4/.kdbgrc.main
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/bench/btl/libs/mtl4/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/bench/btl/libs/mtl4/main.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     5364 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/bench/btl/libs/mtl4/mtl4_LU_solve_interface.hh
--rw-r--r--   0 runner    (1001) docker     (123)     4210 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/bench/btl/libs/mtl4/mtl4_interface.hh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 14:34:30.549841 stag-1.2.1/stag/eigen-3.3.9/bench/btl/libs/tensors/
--rw-r--r--   0 runner    (1001) docker     (123)     2155 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/bench/btl/libs/tensors/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)      671 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/bench/btl/libs/tensors/main_linear.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      624 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/bench/btl/libs/tensors/main_matmat.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      624 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/bench/btl/libs/tensors/main_vecmat.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3190 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/bench/btl/libs/tensors/tensor_interface.hh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 14:34:30.549841 stag-1.2.1/stag/eigen-3.3.9/bench/btl/libs/tvmet/
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/bench/btl/libs/tvmet/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/bench/btl/libs/tvmet/main.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3017 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/bench/btl/libs/tvmet/tvmet_interface.hh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 14:34:30.549841 stag-1.2.1/stag/eigen-3.3.9/bench/btl/libs/ublas/
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/bench/btl/libs/ublas/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1785 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/bench/btl/libs/ublas/main.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4342 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/bench/btl/libs/ublas/ublas_interface.hh
--rw-r--r--   0 runner    (1001) docker     (123)     3269 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/bench/check_cache_queries.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     6416 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/bench/dense_solvers.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     7244 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/bench/eig33.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3307 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/bench/geometry.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 14:34:30.485841 stag-1.2.1/stag/eigen-3.3.9/bench/perf_monitoring/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 14:34:30.553841 stag-1.2.1/stag/eigen-3.3.9/bench/perf_monitoring/gemm/
--rw-r--r--   0 runner    (1001) docker     (123)     3786 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/bench/perf_monitoring/gemm/changesets.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/bench/perf_monitoring/gemm/gemm.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/bench/perf_monitoring/gemm/gemm_settings.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2368 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/bench/perf_monitoring/gemm/lazy_gemm.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/bench/perf_monitoring/gemm/lazy_gemm_settings.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)      991 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/bench/perf_monitoring/gemm/make_plot.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)     3290 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/bench/perf_monitoring/gemm/run.sh
--rw-r--r--   0 runner    (1001) docker     (123)     3232 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/bench/product_threshold.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     6006 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/bench/quat_slerp.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/bench/quatmul.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     6260 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/bench/sparse_cholesky.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     5101 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/bench/sparse_dense_product.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3011 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/bench/sparse_lu.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     8999 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/bench/sparse_product.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3358 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/bench/sparse_randomsetter.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    13761 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/bench/sparse_setter.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2347 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/bench/sparse_transpose.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     6114 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/bench/sparse_trisolver.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 14:34:30.553841 stag-1.2.1/stag/eigen-3.3.9/bench/spbench/
--rw-r--r--   0 runner    (1001) docker     (123)     2939 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/bench/spbench/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3974 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/bench/spbench/sp_solver.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/bench/spbench/spbench.dtd
--rw-r--r--   0 runner    (1001) docker     (123)     3302 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/bench/spbench/spbenchsolver.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    17717 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/bench/spbench/spbenchsolver.h
--rw-r--r--   0 runner    (1001) docker     (123)     3825 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/bench/spbench/spbenchstyle.h
--rw-r--r--   0 runner    (1001) docker     (123)     2830 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/bench/spbench/test_sparseLU.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     6096 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/bench/spmv.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 14:34:30.553841 stag-1.2.1/stag/eigen-3.3.9/bench/tensors/
--rw-r--r--   0 runner    (1001) docker     (123)     2220 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/bench/tensors/README
--rw-r--r--   0 runner    (1001) docker     (123)     1585 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/bench/tensors/benchmark.h
--rw-r--r--   0 runner    (1001) docker     (123)     6834 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/bench/tensors/benchmark_main.cc
--rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/bench/tensors/contraction_benchmarks_cpu.cc
--rw-r--r--   0 runner    (1001) docker     (123)    16193 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/bench/tensors/tensor_benchmarks.h
--rw-r--r--   0 runner    (1001) docker     (123)     6264 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/bench/tensors/tensor_benchmarks_cpu.cc
--rw-r--r--   0 runner    (1001) docker     (123)     3381 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/bench/tensors/tensor_benchmarks_fp16_gpu.cu
--rw-r--r--   0 runner    (1001) docker     (123)     3373 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/bench/tensors/tensor_benchmarks_gpu.cu
--rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/bench/tensors/tensor_benchmarks_sycl.cc
--rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/bench/vdw_new.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 14:34:30.553841 stag-1.2.1/stag/eigen-3.3.9/blas/
--rw-r--r--   0 runner    (1001) docker     (123)     3614 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/blas/BandTriangularSolver.h
--rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/blas/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/blas/GeneralRank1Update.h
--rw-r--r--   0 runner    (1001) docker     (123)     2036 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/blas/PackedSelfadjointProduct.h
--rw-r--r--   0 runner    (1001) docker     (123)     3165 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/blas/PackedTriangularMatrixVector.h
--rw-r--r--   0 runner    (1001) docker     (123)     3191 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/blas/PackedTriangularSolverVector.h
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/blas/README.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/blas/Rank2Update.h
--rw-r--r--   0 runner    (1001) docker     (123)     4361 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/blas/common.h
--rw-r--r--   0 runner    (1001) docker     (123)      647 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/blas/complex_double.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      646 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/blas/complex_single.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/blas/double.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 14:34:30.557841 stag-1.2.1/stag/eigen-3.3.9/blas/f2c/
--rw-r--r--   0 runner    (1001) docker     (123)    15108 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/blas/f2c/chbmv.c
--rw-r--r--   0 runner    (1001) docker     (123)    13026 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/blas/f2c/chpmv.c
--rw-r--r--   0 runner    (1001) docker     (123)     2310 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/blas/f2c/complexdots.c
--rw-r--r--   0 runner    (1001) docker     (123)    18944 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/blas/f2c/ctbmv.c
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/blas/f2c/d_cnjg.c
--rw-r--r--   0 runner    (1001) docker     (123)      657 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/blas/f2c/datatypes.h
--rw-r--r--   0 runner    (1001) docker     (123)     4968 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/blas/f2c/drotm.c
--rw-r--r--   0 runner    (1001) docker     (123)     6193 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/blas/f2c/drotmg.c
--rw-r--r--   0 runner    (1001) docker     (123)    10188 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/blas/f2c/dsbmv.c
--rw-r--r--   0 runner    (1001) docker     (123)     8075 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/blas/f2c/dspmv.c
--rw-r--r--   0 runner    (1001) docker     (123)    11656 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/blas/f2c/dtbmv.c
--rw-r--r--   0 runner    (1001) docker     (123)     2976 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/blas/f2c/lsame.c
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/blas/f2c/r_cnjg.c
--rw-r--r--   0 runner    (1001) docker     (123)     4902 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/blas/f2c/srotm.c
--rw-r--r--   0 runner    (1001) docker     (123)     6056 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/blas/f2c/srotmg.c
--rw-r--r--   0 runner    (1001) docker     (123)    10210 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/blas/f2c/ssbmv.c
--rw-r--r--   0 runner    (1001) docker     (123)     8051 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/blas/f2c/sspmv.c
--rw-r--r--   0 runner    (1001) docker     (123)    11642 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/blas/f2c/stbmv.c
--rw-r--r--   0 runner    (1001) docker     (123)    15144 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/blas/f2c/zhbmv.c
--rw-r--r--   0 runner    (1001) docker     (123)    13060 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/blas/f2c/zhpmv.c
--rw-r--r--   0 runner    (1001) docker     (123)    18972 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/blas/f2c/ztbmv.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 14:34:30.557841 stag-1.2.1/stag/eigen-3.3.9/blas/fortran/
--rw-r--r--   0 runner    (1001) docker     (123)      979 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/blas/fortran/complexdots.f
--rw-r--r--   0 runner    (1001) docker     (123)     4956 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/blas/level1_cplx_impl.h
--rw-r--r--   0 runner    (1001) docker     (123)     4559 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/blas/level1_impl.h
--rw-r--r--   0 runner    (1001) docker     (123)     3617 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/blas/level1_real_impl.h
--rw-r--r--   0 runner    (1001) docker     (123)    12223 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/blas/level2_cplx_impl.h
--rw-r--r--   0 runner    (1001) docker     (123)    25172 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/blas/level2_impl.h
--rw-r--r--   0 runner    (1001) docker     (123)    10499 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/blas/level2_real_impl.h
--rw-r--r--   0 runner    (1001) docker     (123)    38043 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/blas/level3_impl.h
--rw-r--r--   0 runner    (1001) docker     (123)      757 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/blas/single.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 14:34:30.561841 stag-1.2.1/stag/eigen-3.3.9/blas/testing/
--rw-r--r--   0 runner    (1001) docker     (123)      964 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/blas/testing/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)    32109 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/blas/testing/cblat1.f
--rw-r--r--   0 runner    (1001) docker     (123)     1546 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/blas/testing/cblat2.dat
--rw-r--r--   0 runner    (1001) docker     (123)   116657 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/blas/testing/cblat2.f
--rw-r--r--   0 runner    (1001) docker     (123)     1046 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/blas/testing/cblat3.dat
--rw-r--r--   0 runner    (1001) docker     (123)   131550 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/blas/testing/cblat3.f
--rw-r--r--   0 runner    (1001) docker     (123)    44819 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/blas/testing/dblat1.f
--rw-r--r--   0 runner    (1001) docker     (123)     1466 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/blas/testing/dblat2.dat
--rw-r--r--   0 runner    (1001) docker     (123)   112335 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/blas/testing/dblat2.f
--rw-r--r--   0 runner    (1001) docker     (123)      882 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/blas/testing/dblat3.dat
--rw-r--r--   0 runner    (1001) docker     (123)   104262 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/blas/testing/dblat3.f
--rwxr-xr-x   0 runner    (1001) docker     (123)     1016 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/blas/testing/runblastest.sh
--rw-r--r--   0 runner    (1001) docker     (123)    43388 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/blas/testing/sblat1.f
--rw-r--r--   0 runner    (1001) docker     (123)     1466 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/blas/testing/sblat2.dat
--rw-r--r--   0 runner    (1001) docker     (123)   112251 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/blas/testing/sblat2.f
--rw-r--r--   0 runner    (1001) docker     (123)      882 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/blas/testing/sblat3.dat
--rw-r--r--   0 runner    (1001) docker     (123)   104172 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/blas/testing/sblat3.f
--rw-r--r--   0 runner    (1001) docker     (123)    32114 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/blas/testing/zblat1.f
--rw-r--r--   0 runner    (1001) docker     (123)     1546 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/blas/testing/zblat2.dat
--rw-r--r--   0 runner    (1001) docker     (123)   117003 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/blas/testing/zblat2.f
--rw-r--r--   0 runner    (1001) docker     (123)     1046 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/blas/testing/zblat3.dat
--rw-r--r--   0 runner    (1001) docker     (123)   131995 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/blas/testing/zblat3.f
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/blas/xerbla.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 14:34:30.561841 stag-1.2.1/stag/eigen-3.3.9/cmake/
--rw-r--r--   0 runner    (1001) docker     (123)      769 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/cmake/Eigen3Config.cmake.in
--rw-r--r--   0 runner    (1001) docker     (123)     1397 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/cmake/Eigen3ConfigLegacy.cmake.in
--rw-r--r--   0 runner    (1001) docker     (123)     2825 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/cmake/EigenConfigureTesting.cmake
--rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/cmake/EigenDetermineOSVersion.cmake
--rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/cmake/EigenDetermineVSServicePack.cmake
--rw-r--r--   0 runner    (1001) docker     (123)    26793 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/cmake/EigenTesting.cmake
--rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/cmake/EigenUninstall.cmake
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/cmake/FindAdolc.cmake
--rw-r--r--   0 runner    (1001) docker     (123)    43820 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/cmake/FindBLAS.cmake
--rw-r--r--   0 runner    (1001) docker     (123)    13031 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/cmake/FindBLASEXT.cmake
--rw-r--r--   0 runner    (1001) docker     (123)     2572 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/cmake/FindCholmod.cmake
--rw-r--r--   0 runner    (1001) docker     (123)     9003 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/cmake/FindComputeCpp.cmake
--rw-r--r--   0 runner    (1001) docker     (123)     2842 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/cmake/FindEigen2.cmake
--rw-r--r--   0 runner    (1001) docker     (123)     3501 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/cmake/FindEigen3.cmake
--rw-r--r--   0 runner    (1001) docker     (123)     2757 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/cmake/FindFFTW.cmake
--rw-r--r--   0 runner    (1001) docker     (123)     2943 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/cmake/FindGLEW.cmake
--rw-r--r--   0 runner    (1001) docker     (123)      554 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/cmake/FindGMP.cmake
--rw-r--r--   0 runner    (1001) docker     (123)     5035 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/cmake/FindGSL.cmake
--rw-r--r--   0 runner    (1001) docker     (123)      909 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/cmake/FindGoogleHash.cmake
--rw-r--r--   0 runner    (1001) docker     (123)    11857 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/cmake/FindHWLOC.cmake
--rw-r--r--   0 runner    (1001) docker     (123)     9909 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/cmake/FindLAPACK.cmake
--rw-r--r--   0 runner    (1001) docker     (123)     2845 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/cmake/FindMPFR.cmake
--rw-r--r--   0 runner    (1001) docker     (123)     8963 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/cmake/FindMetis.cmake
--rw-r--r--   0 runner    (1001) docker     (123)    14450 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/cmake/FindPTSCOTCH.cmake
--rw-r--r--   0 runner    (1001) docker     (123)    23207 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/cmake/FindPastix.cmake
--rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/cmake/FindSPQR.cmake
--rw-r--r--   0 runner    (1001) docker     (123)    12010 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/cmake/FindScotch.cmake
--rw-r--r--   0 runner    (1001) docker     (123)     2243 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/cmake/FindStandardMathLibrary.cmake
--rw-r--r--   0 runner    (1001) docker     (123)     2299 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/cmake/FindSuperLU.cmake
--rw-r--r--   0 runner    (1001) docker     (123)     1735 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/cmake/FindUmfpack.cmake
--rw-r--r--   0 runner    (1001) docker     (123)      936 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/cmake/RegexUtils.cmake
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/cmake/UseEigen3.cmake
--rw-r--r--   0 runner    (1001) docker     (123)     2413 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/cmake/language_support.cmake
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 14:34:30.485841 stag-1.2.1/stag/eigen-3.3.9/debug/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 14:34:30.561841 stag-1.2.1/stag/eigen-3.3.9/debug/gdb/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/debug/gdb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6547 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/debug/gdb/printers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 14:34:30.561841 stag-1.2.1/stag/eigen-3.3.9/debug/msvc/
--rw-r--r--   0 runner    (1001) docker     (123)    11661 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/debug/msvc/eigen.natvis
--rw-r--r--   0 runner    (1001) docker     (123)     7566 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/debug/msvc/eigen_autoexp_part.dat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 14:34:30.561841 stag-1.2.1/stag/eigen-3.3.9/demos/
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/demos/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 14:34:30.565841 stag-1.2.1/stag/eigen-3.3.9/demos/mandelbrot/
--rw-r--r--   0 runner    (1001) docker     (123)      486 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/demos/mandelbrot/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/demos/mandelbrot/README
--rw-r--r--   0 runner    (1001) docker     (123)     7509 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/demos/mandelbrot/mandelbrot.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1888 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/demos/mandelbrot/mandelbrot.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 14:34:30.565841 stag-1.2.1/stag/eigen-3.3.9/demos/mix_eigen_and_c/
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/demos/mix_eigen_and_c/README
--rw-r--r--   0 runner    (1001) docker     (123)     4158 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/demos/mix_eigen_and_c/binary_library.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3345 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/demos/mix_eigen_and_c/binary_library.h
--rw-r--r--   0 runner    (1001) docker     (123)     1616 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/demos/mix_eigen_and_c/example.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 14:34:30.565841 stag-1.2.1/stag/eigen-3.3.9/demos/opengl/
--rw-r--r--   0 runner    (1001) docker     (123)      695 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/demos/opengl/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)      403 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/demos/opengl/README
--rw-r--r--   0 runner    (1001) docker     (123)     5981 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/demos/opengl/camera.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3435 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/demos/opengl/camera.h
--rw-r--r--   0 runner    (1001) docker     (123)     3974 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/demos/opengl/gpuhelper.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     7177 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/demos/opengl/gpuhelper.h
--rw-r--r--   0 runner    (1001) docker     (123)     3927 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/demos/opengl/icosphere.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      869 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/demos/opengl/icosphere.h
--rw-r--r--   0 runner    (1001) docker     (123)    19192 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/demos/opengl/quaternion_demo.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2635 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/demos/opengl/quaternion_demo.h
--rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/demos/opengl/trackball.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      943 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/demos/opengl/trackball.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 14:34:30.569841 stag-1.2.1/stag/eigen-3.3.9/doc/
--rw-r--r--   0 runner    (1001) docker     (123)    12377 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/A05_PortingFrom2To3.dox
--rw-r--r--   0 runner    (1001) docker     (123)    10274 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/AsciiQuickReference.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2425 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/B01_Experimental.dox
--rw-r--r--   0 runner    (1001) docker     (123)     4853 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6332 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/ClassHierarchy.dox
--rw-r--r--   0 runner    (1001) docker     (123)    16511 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/CoeffwiseMathFunctionsTable.dox
--rw-r--r--   0 runner    (1001) docker     (123)     4423 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/CustomizingEigen_CustomScalar.dox
--rw-r--r--   0 runner    (1001) docker     (123)     1337 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/CustomizingEigen_InheritingMatrix.dox
--rw-r--r--   0 runner    (1001) docker     (123)     3658 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/CustomizingEigen_NullaryExpr.dox
--rw-r--r--   0 runner    (1001) docker     (123)     3658 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/CustomizingEigen_Plugins.dox
--rw-r--r--   0 runner    (1001) docker     (123)     5022 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/DenseDecompositionBenchmark.dox
--rw-r--r--   0 runner    (1001) docker     (123)    85853 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/Doxyfile.in
--rw-r--r--   0 runner    (1001) docker     (123)     8355 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/Eigen_Silly_Professor_64x64.png
--rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/FixedSizeVectorizable.dox
--rw-r--r--   0 runner    (1001) docker     (123)    13452 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/FunctionsTakingEigenTypes.dox
--rw-r--r--   0 runner    (1001) docker     (123)     5429 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/HiPerformance.dox
--rw-r--r--   0 runner    (1001) docker     (123)     3797 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/InplaceDecomposition.dox
--rw-r--r--   0 runner    (1001) docker     (123)    30239 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/InsideEigenExample.dox
--rw-r--r--   0 runner    (1001) docker     (123)     2791 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/LeastSquares.dox
--rw-r--r--   0 runner    (1001) docker     (123)     6551 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/Manual.dox
--rw-r--r--   0 runner    (1001) docker     (123)      758 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/MatrixfreeSolverExample.dox
--rw-r--r--   0 runner    (1001) docker     (123)     5610 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/NewExpressionType.dox
--rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/Overview.dox
--rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/PassingByValue.dox
--rw-r--r--   0 runner    (1001) docker     (123)     6290 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/Pitfalls.dox
--rw-r--r--   0 runner    (1001) docker     (123)    13440 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/PreprocessorDirectives.dox
--rw-r--r--   0 runner    (1001) docker     (123)    29069 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/QuickReference.dox
--rw-r--r--   0 runner    (1001) docker     (123)     6577 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/QuickStartGuide.dox
--rw-r--r--   0 runner    (1001) docker     (123)    19614 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/SparseLinearSystems.dox
--rw-r--r--   0 runner    (1001) docker     (123)     8313 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/SparseQuickReference.dox
--rw-r--r--   0 runner    (1001) docker     (123)     3424 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/StlContainers.dox
--rw-r--r--   0 runner    (1001) docker     (123)     4119 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/StorageOrders.dox
--rw-r--r--   0 runner    (1001) docker     (123)     6212 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/StructHavingEigenMembers.dox
--rw-r--r--   0 runner    (1001) docker     (123)     6156 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/TemplateKeyword.dox
--rw-r--r--   0 runner    (1001) docker     (123)    10269 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/TopicAliasing.dox
--rw-r--r--   0 runner    (1001) docker     (123)     5285 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/TopicAssertions.dox
--rw-r--r--   0 runner    (1001) docker     (123)     1642 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/TopicCMakeGuide.dox
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/TopicEigenExpressionTemplates.dox
--rw-r--r--   0 runner    (1001) docker     (123)     6314 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/TopicLazyEvaluation.dox
--rw-r--r--   0 runner    (1001) docker     (123)     8806 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/TopicLinearAlgebraDecompositions.dox
--rw-r--r--   0 runner    (1001) docker     (123)     2666 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/TopicMultithreading.dox
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/TopicResizing.dox
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/TopicScalarTypes.dox
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/TopicVectorization.dox
--rw-r--r--   0 runner    (1001) docker     (123)     6900 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/TutorialAdvancedInitialization.dox
--rw-r--r--   0 runner    (1001) docker     (123)     8523 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/TutorialArrayClass.dox
--rw-r--r--   0 runner    (1001) docker     (123)     7823 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/TutorialBlockOperations.dox
--rw-r--r--   0 runner    (1001) docker     (123)     9730 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/TutorialGeometry.dox
--rw-r--r--   0 runner    (1001) docker     (123)    11202 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/TutorialLinearAlgebra.dox
--rw-r--r--   0 runner    (1001) docker     (123)     3986 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/TutorialMapClass.dox
--rw-r--r--   0 runner    (1001) docker     (123)     9865 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/TutorialMatrixArithmetic.dox
--rw-r--r--   0 runner    (1001) docker     (123)    12421 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/TutorialMatrixClass.dox
--rw-r--r--   0 runner    (1001) docker     (123)    12006 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/TutorialReductionsVisitorsBroadcasting.dox
--rw-r--r--   0 runner    (1001) docker     (123)     1910 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/TutorialReshapeSlicing.dox
--rw-r--r--   0 runner    (1001) docker     (123)    20478 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/TutorialSparse.dox
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/TutorialSparse_example_details.dox
--rw-r--r--   0 runner    (1001) docker     (123)     6888 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/UnalignedArrayAssert.dox
--rw-r--r--   0 runner    (1001) docker     (123)     6633 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/UsingBlasLapackBackends.dox
--rw-r--r--   0 runner    (1001) docker     (123)     6020 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/UsingIntelMKL.dox
--rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/UsingNVCC.dox
--rw-r--r--   0 runner    (1001) docker     (123)     2924 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/WrongStackAlignment.dox
--rw-r--r--   0 runner    (1001) docker     (123)     8006 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/eigen_navtree_hacks.js
--rw-r--r--   0 runner    (1001) docker     (123)     4409 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/eigendoxy.css
--rw-r--r--   0 runner    (1001) docker     (123)      680 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/eigendoxy_footer.html.in
--rw-r--r--   0 runner    (1001) docker     (123)     2521 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/eigendoxy_header.html.in
--rw-r--r--   0 runner    (1001) docker     (123)     5337 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/eigendoxy_layout.xml.in
--rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/eigendoxy_tabs.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 14:34:30.577841 stag-1.2.1/stag/eigen-3.3.9/doc/examples/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/examples/.krazy
--rw-r--r--   0 runner    (1001) docker     (123)      685 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/examples/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)      766 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/examples/CustomizingEigen_Inheritance.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/examples/Cwise_erf.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/examples/Cwise_erfc.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/examples/Cwise_lgamma.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/examples/DenseBase_middleCols_int.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/examples/DenseBase_middleRows_int.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/examples/DenseBase_template_int_middleCols.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/examples/DenseBase_template_int_middleRows.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/examples/QuickStart_example.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/examples/QuickStart_example2_dynamic.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/examples/QuickStart_example2_fixed.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      677 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/examples/TemplateKeyword_flexible.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      508 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/examples/TemplateKeyword_simple.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1589 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/examples/TutorialInplaceLU.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      622 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/examples/TutorialLinAlgComputeTwice.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/examples/TutorialLinAlgExComputeSolveError.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/examples/TutorialLinAlgExSolveColPivHouseholderQR.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/examples/TutorialLinAlgExSolveLDLT.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      348 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/examples/TutorialLinAlgInverseDeterminant.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/examples/TutorialLinAlgRankRevealing.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/examples/TutorialLinAlgSVDSolve.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      534 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/examples/TutorialLinAlgSelfAdjointEigenSolver.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      377 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/examples/TutorialLinAlgSetThreshold.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      466 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/examples/Tutorial_ArrayClass_accessors.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      400 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/examples/Tutorial_ArrayClass_addition.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/examples/Tutorial_ArrayClass_cwise_other.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      444 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/examples/Tutorial_ArrayClass_interop.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      591 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/examples/Tutorial_ArrayClass_interop_matrix.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/examples/Tutorial_ArrayClass_mult.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      523 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/examples/Tutorial_BlockOperations_block_assignment.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/examples/Tutorial_BlockOperations_colrow.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      448 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/examples/Tutorial_BlockOperations_corner.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/examples/Tutorial_BlockOperations_print_block.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      348 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/examples/Tutorial_BlockOperations_vector.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      401 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/examples/Tutorial_PartialLU_solve.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      440 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/examples/Tutorial_ReductionsVisitorsBroadcasting_broadcast_1nn.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/examples/Tutorial_ReductionsVisitorsBroadcasting_broadcast_simple.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      361 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/examples/Tutorial_ReductionsVisitorsBroadcasting_broadcast_simple_rowwise.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/examples/Tutorial_ReductionsVisitorsBroadcasting_colwise.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/examples/Tutorial_ReductionsVisitorsBroadcasting_maxnorm.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/examples/Tutorial_ReductionsVisitorsBroadcasting_reductions_bool.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/examples/Tutorial_ReductionsVisitorsBroadcasting_reductions_norm.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/examples/Tutorial_ReductionsVisitorsBroadcasting_reductions_operatornorm.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/examples/Tutorial_ReductionsVisitorsBroadcasting_rowwise.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      531 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/examples/Tutorial_ReductionsVisitorsBroadcasting_visitors.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      680 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/examples/Tutorial_simple_example_dynamic_size.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/examples/Tutorial_simple_example_fixed_size.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/examples/class_Block.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/examples/class_CwiseBinaryOp.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      561 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/examples/class_CwiseUnaryOp.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/examples/class_CwiseUnaryOp_ptrfun.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/examples/class_FixedBlock.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      673 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/examples/class_FixedVectorBlock.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/examples/class_VectorBlock.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      418 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/examples/function_taking_eigenbase.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/examples/function_taking_ref.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/examples/make_circulant.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/examples/make_circulant.cpp.entry
--rw-r--r--   0 runner    (1001) docker     (123)      948 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/examples/make_circulant.cpp.evaluator
--rw-r--r--   0 runner    (1001) docker     (123)      591 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/examples/make_circulant.cpp.expression
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/examples/make_circulant.cpp.main
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/examples/make_circulant.cpp.preamble
--rw-r--r--   0 runner    (1001) docker     (123)      605 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/examples/make_circulant.cpp.traits
--rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/examples/make_circulant2.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4275 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/examples/matrixfree_cg.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2438 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/examples/nullary_indexing.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      471 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/examples/tut_arithmetic_add_sub.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/examples/tut_arithmetic_dot_cross.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/examples/tut_arithmetic_matrix_mul.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      529 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/examples/tut_arithmetic_redux_basic.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/examples/tut_arithmetic_scalar_mul_div.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/examples/tut_matrix_coefficient_accessors.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/examples/tut_matrix_resize.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/examples/tut_matrix_resize_fixed_size.cpp
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/ftv2node.png
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/ftv2pnode.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 14:34:30.609841 stag-1.2.1/stag/eigen-3.3.9/doc/snippets/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/snippets/.krazy
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/snippets/AngleAxis_mimic_euler.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/snippets/BiCGSTAB_simple.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      406 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/snippets/BiCGSTAB_step_by_step.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/snippets/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/snippets/ColPivHouseholderQR_solve.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      792 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/snippets/ComplexEigenSolver_compute.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/snippets/ComplexEigenSolver_eigenvalues.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/snippets/ComplexEigenSolver_eigenvectors.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/snippets/ComplexSchur_compute.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/snippets/ComplexSchur_matrixT.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/snippets/ComplexSchur_matrixU.cpp
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/snippets/Cwise_abs.cpp
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/snippets/Cwise_abs2.cpp
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/snippets/Cwise_acos.cpp
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/snippets/Cwise_arg.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/snippets/Cwise_array_power_array.cpp
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/snippets/Cwise_asin.cpp
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/snippets/Cwise_atan.cpp
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/snippets/Cwise_boolean_and.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/snippets/Cwise_boolean_not.cpp
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/snippets/Cwise_boolean_or.cpp
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/snippets/Cwise_boolean_xor.cpp
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/snippets/Cwise_ceil.cpp
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/snippets/Cwise_cos.cpp
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/snippets/Cwise_cosh.cpp
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/snippets/Cwise_cube.cpp
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/snippets/Cwise_equal_equal.cpp
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/snippets/Cwise_exp.cpp
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/snippets/Cwise_floor.cpp
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/snippets/Cwise_greater.cpp
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/snippets/Cwise_greater_equal.cpp
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/snippets/Cwise_inverse.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/snippets/Cwise_isFinite.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/snippets/Cwise_isInf.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/snippets/Cwise_isNaN.cpp
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/snippets/Cwise_less.cpp
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/snippets/Cwise_less_equal.cpp
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/snippets/Cwise_log.cpp
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/snippets/Cwise_log10.cpp
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/snippets/Cwise_max.cpp
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/snippets/Cwise_min.cpp
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/snippets/Cwise_minus.cpp
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/snippets/Cwise_minus_equal.cpp
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/snippets/Cwise_not_equal.cpp
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/snippets/Cwise_plus.cpp
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/snippets/Cwise_plus_equal.cpp
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/snippets/Cwise_pow.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/snippets/Cwise_product.cpp
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/snippets/Cwise_quotient.cpp
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/snippets/Cwise_round.cpp
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/snippets/Cwise_scalar_power_array.cpp
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/snippets/Cwise_sign.cpp
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/snippets/Cwise_sin.cpp
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/snippets/Cwise_sinh.cpp
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/snippets/Cwise_slash_equal.cpp
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/snippets/Cwise_sqrt.cpp
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/snippets/Cwise_square.cpp
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/snippets/Cwise_tan.cpp
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/snippets/Cwise_tanh.cpp
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/snippets/Cwise_times_equal.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/snippets/DenseBase_LinSpaced.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      420 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/snippets/DenseBase_LinSpacedInt.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/snippets/DenseBase_LinSpaced_seq.cpp
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/snippets/DenseBase_setLinSpaced.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/snippets/DirectionWise_hnormalized.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/snippets/DirectionWise_replicate.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/snippets/DirectionWise_replicate_int.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      800 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/snippets/EigenSolver_EigenSolver_MatrixType.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      361 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/snippets/EigenSolver_compute.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/snippets/EigenSolver_eigenvalues.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/snippets/EigenSolver_eigenvectors.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/snippets/EigenSolver_pseudoEigenvectors.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/snippets/FullPivHouseholderQR_solve.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/snippets/FullPivLU_image.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/snippets/FullPivLU_kernel.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/snippets/FullPivLU_solve.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      456 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/snippets/GeneralizedEigenSolver.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      339 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/snippets/HessenbergDecomposition_compute.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/snippets/HessenbergDecomposition_matrixH.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/snippets/HessenbergDecomposition_packedMatrix.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/snippets/HouseholderQR_householderQ.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/snippets/HouseholderQR_solve.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/snippets/HouseholderSequence_HouseholderSequence.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      603 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/snippets/IOFormat.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      614 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/snippets/JacobiSVD_basic.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/snippets/Jacobi_makeGivens.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      292 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/snippets/Jacobi_makeJacobi.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/snippets/LLT_example.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      456 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/snippets/LLT_solve.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/snippets/LeastSquaresNormalEquations.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/snippets/LeastSquaresQR.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/snippets/Map_general_stride.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/snippets/Map_inner_stride.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/snippets/Map_outer_stride.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/snippets/Map_placement_new.cpp
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/snippets/Map_simple.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/snippets/MatrixBase_adjoint.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      523 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/snippets/MatrixBase_all.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/snippets/MatrixBase_applyOnTheLeft.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      292 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/snippets/MatrixBase_applyOnTheRight.cpp
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/snippets/MatrixBase_array.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/snippets/MatrixBase_array_const.cpp
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/snippets/MatrixBase_asDiagonal.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/snippets/MatrixBase_block_int_int.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/snippets/MatrixBase_block_int_int_int_int.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/snippets/MatrixBase_bottomLeftCorner_int_int.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/snippets/MatrixBase_bottomRightCorner_int_int.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/snippets/MatrixBase_bottomRows_int.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/snippets/MatrixBase_cast.cpp
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/snippets/MatrixBase_col.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/snippets/MatrixBase_colwise.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/snippets/MatrixBase_computeInverseAndDetWithCheck.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/snippets/MatrixBase_computeInverseWithCheck.cpp
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/snippets/MatrixBase_cwiseAbs.cpp
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/snippets/MatrixBase_cwiseAbs2.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/snippets/MatrixBase_cwiseEqual.cpp
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/snippets/MatrixBase_cwiseInverse.cpp
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/snippets/MatrixBase_cwiseMax.cpp
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/snippets/MatrixBase_cwiseMin.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/snippets/MatrixBase_cwiseNotEqual.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/snippets/MatrixBase_cwiseProduct.cpp
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/snippets/MatrixBase_cwiseQuotient.cpp
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/snippets/MatrixBase_cwiseSign.cpp
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/snippets/MatrixBase_cwiseSqrt.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/snippets/MatrixBase_diagonal.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      270 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/snippets/MatrixBase_diagonal_int.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/snippets/MatrixBase_diagonal_template_int.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/snippets/MatrixBase_eigenvalues.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/snippets/MatrixBase_end_int.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      467 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/snippets/MatrixBase_eval.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/snippets/MatrixBase_fixedBlock_int_int.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      376 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/snippets/MatrixBase_hnormalized.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      486 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/snippets/MatrixBase_homogeneous.cpp
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/snippets/MatrixBase_identity.cpp
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/snippets/MatrixBase_identity_int_int.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/snippets/MatrixBase_inverse.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/snippets/MatrixBase_isDiagonal.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/snippets/MatrixBase_isIdentity.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/snippets/MatrixBase_isOnes.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      293 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/snippets/MatrixBase_isOrthogonal.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/snippets/MatrixBase_isUnitary.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/snippets/MatrixBase_isZero.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/snippets/MatrixBase_leftCols_int.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/snippets/MatrixBase_noalias.cpp
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/snippets/MatrixBase_ones.cpp
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/snippets/MatrixBase_ones_int.cpp
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/snippets/MatrixBase_ones_int_int.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/snippets/MatrixBase_operatorNorm.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/snippets/MatrixBase_prod.cpp
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/snippets/MatrixBase_random.cpp
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/snippets/MatrixBase_random_int.cpp
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/snippets/MatrixBase_random_int_int.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/snippets/MatrixBase_replicate.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/snippets/MatrixBase_replicate_int_int.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      407 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/snippets/MatrixBase_reverse.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/snippets/MatrixBase_rightCols_int.cpp
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/snippets/MatrixBase_row.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/snippets/MatrixBase_rowwise.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/snippets/MatrixBase_segment_int_int.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/snippets/MatrixBase_select.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      361 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/snippets/MatrixBase_selfadjointView.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/snippets/MatrixBase_set.cpp
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/snippets/MatrixBase_setIdentity.cpp
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/snippets/MatrixBase_setOnes.cpp
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/snippets/MatrixBase_setRandom.cpp
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/snippets/MatrixBase_setZero.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/snippets/MatrixBase_start_int.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/snippets/MatrixBase_template_int_bottomRows.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/snippets/MatrixBase_template_int_end.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/snippets/MatrixBase_template_int_int_block_int_int_int_int.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/snippets/MatrixBase_template_int_int_bottomLeftCorner.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/snippets/MatrixBase_template_int_int_bottomLeftCorner_int_int.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/snippets/MatrixBase_template_int_int_bottomRightCorner.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      304 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/snippets/MatrixBase_template_int_int_bottomRightCorner_int_int.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/snippets/MatrixBase_template_int_int_topLeftCorner.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      292 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/snippets/MatrixBase_template_int_int_topLeftCorner_int_int.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/snippets/MatrixBase_template_int_int_topRightCorner.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/snippets/MatrixBase_template_int_int_topRightCorner_int_int.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/snippets/MatrixBase_template_int_leftCols.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/snippets/MatrixBase_template_int_rightCols.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/snippets/MatrixBase_template_int_segment.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/snippets/MatrixBase_template_int_start.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/snippets/MatrixBase_template_int_topRows.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/snippets/MatrixBase_topLeftCorner_int_int.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/snippets/MatrixBase_topRightCorner_int_int.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/snippets/MatrixBase_topRows_int.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      414 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/snippets/MatrixBase_transpose.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/snippets/MatrixBase_triangularView.cpp
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/snippets/MatrixBase_zero.cpp
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/snippets/MatrixBase_zero_int.cpp
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/snippets/MatrixBase_zero_int_int.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/snippets/Matrix_Map_stride.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/snippets/Matrix_resize_NoChange_int.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/snippets/Matrix_resize_int.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/snippets/Matrix_resize_int_NoChange.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      407 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/snippets/Matrix_resize_int_int.cpp
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/snippets/Matrix_setConstant_int.cpp
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/snippets/Matrix_setConstant_int_int.cpp
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/snippets/Matrix_setIdentity_int_int.cpp
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/snippets/Matrix_setOnes_int.cpp
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/snippets/Matrix_setOnes_int_int.cpp
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/snippets/Matrix_setRandom_int.cpp
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/snippets/Matrix_setRandom_int_int.cpp
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/snippets/Matrix_setZero_int.cpp
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/snippets/Matrix_setZero_int_int.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/snippets/PartialPivLU_solve.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/snippets/PartialRedux_count.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/snippets/PartialRedux_maxCoeff.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/snippets/PartialRedux_minCoeff.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/snippets/PartialRedux_norm.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/snippets/PartialRedux_prod.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/snippets/PartialRedux_squaredNorm.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/snippets/PartialRedux_sum.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      819 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/snippets/RealQZ_compute.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      429 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/snippets/RealSchur_RealSchur_MatrixType.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/snippets/RealSchur_compute.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/snippets/SelfAdjointEigenSolver_SelfAdjointEigenSolver.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      816 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/snippets/SelfAdjointEigenSolver_SelfAdjointEigenSolver_MatrixType.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      826 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/snippets/SelfAdjointEigenSolver_SelfAdjointEigenSolver_MatrixType2.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      365 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/snippets/SelfAdjointEigenSolver_compute_MatrixType.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/snippets/SelfAdjointEigenSolver_compute_MatrixType2.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/snippets/SelfAdjointEigenSolver_eigenvalues.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/snippets/SelfAdjointEigenSolver_eigenvectors.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/snippets/SelfAdjointEigenSolver_operatorInverseSqrt.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/snippets/SelfAdjointEigenSolver_operatorSqrt.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/snippets/SelfAdjointView_eigenvalues.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/snippets/SelfAdjointView_operatorNorm.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/snippets/SparseMatrix_coeffs.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/snippets/TopicAliasing_block.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      270 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/snippets/TopicAliasing_block_correct.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      591 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/snippets/TopicAliasing_cwise.cpp
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/snippets/TopicAliasing_mult1.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/snippets/TopicAliasing_mult2.cpp
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/snippets/TopicAliasing_mult3.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/snippets/TopicAliasing_mult4.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/snippets/TopicAliasing_mult5.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/snippets/TopicStorageOrders_example.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      520 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/snippets/Triangular_solve.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/snippets/Tridiagonalization_Tridiagonalization_MatrixType.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/snippets/Tridiagonalization_compute.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/snippets/Tridiagonalization_decomposeInPlace.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      552 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/snippets/Tridiagonalization_diagonal.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/snippets/Tridiagonalization_householderCoefficients.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/snippets/Tridiagonalization_packedMatrix.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/snippets/Tutorial_AdvancedInitialization_Block.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/snippets/Tutorial_AdvancedInitialization_CommaTemporary.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/snippets/Tutorial_AdvancedInitialization_Join.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/snippets/Tutorial_AdvancedInitialization_LinSpaced.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      878 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/snippets/Tutorial_AdvancedInitialization_ThreeWays.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/snippets/Tutorial_AdvancedInitialization_Zero.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/snippets/Tutorial_Map_rowmajor.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      896 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/snippets/Tutorial_Map_using.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/snippets/Tutorial_ReshapeMat2Mat.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/snippets/Tutorial_ReshapeMat2Vec.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/snippets/Tutorial_SlicingCol.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/snippets/Tutorial_SlicingVec.cpp
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/snippets/Tutorial_commainit_01.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/snippets/Tutorial_commainit_01b.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/snippets/Tutorial_commainit_02.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/snippets/Tutorial_solve_matrix_inverse.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/snippets/Tutorial_solve_multiple_rhs.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      368 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/snippets/Tutorial_solve_reuse_decomposition.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/snippets/Tutorial_solve_singular.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/snippets/Tutorial_solve_triangular.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/snippets/Tutorial_solve_triangular_inplace.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/snippets/VectorwiseOp_homogeneous.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/snippets/Vectorwise_reverse.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      732 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/snippets/class_FullPivLU.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      506 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/snippets/compile_snippet.cpp.in
--rw-r--r--   0 runner    (1001) docker     (123)      468 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/snippets/tut_arithmetic_redux_minmax.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/snippets/tut_arithmetic_transpose_aliasing.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/snippets/tut_arithmetic_transpose_conjugate.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/snippets/tut_arithmetic_transpose_inplace.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/snippets/tut_matrix_assignment_resizing.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 14:34:30.609841 stag-1.2.1/stag/eigen-3.3.9/doc/special_examples/
--rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/special_examples/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/special_examples/Tutorial_sparse_example.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/special_examples/Tutorial_sparse_example_details.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/special_examples/random_cpp11.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2544 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/doc/tutorial.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/eigen3.pc.in
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 14:34:30.613841 stag-1.2.1/stag/eigen-3.3.9/failtest/
--rw-r--r--   0 runner    (1001) docker     (123)     2791 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/failtest/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/failtest/bdcsvd_int.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/failtest/block_nonconst_ctor_on_const_xpr_0.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/failtest/block_nonconst_ctor_on_const_xpr_1.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/failtest/block_nonconst_ctor_on_const_xpr_2.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/failtest/block_on_const_type_actually_const_0.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/failtest/block_on_const_type_actually_const_1.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/failtest/colpivqr_int.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/failtest/const_qualified_block_method_retval_0.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/failtest/const_qualified_block_method_retval_1.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/failtest/const_qualified_diagonal_method_retval.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/failtest/const_qualified_transpose_method_retval.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/failtest/cwiseunaryview_nonconst_ctor_on_const_xpr.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/failtest/cwiseunaryview_on_const_type_actually_const.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/failtest/diagonal_nonconst_ctor_on_const_xpr.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/failtest/diagonal_on_const_type_actually_const.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/failtest/eigensolver_cplx.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/failtest/eigensolver_int.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/failtest/failtest_sanity_check.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/failtest/fullpivlu_int.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/failtest/fullpivqr_int.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/failtest/jacobisvd_int.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/failtest/ldlt_int.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/failtest/llt_int.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/failtest/map_nonconst_ctor_on_const_ptr_0.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/failtest/map_nonconst_ctor_on_const_ptr_1.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      270 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/failtest/map_nonconst_ctor_on_const_ptr_2.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/failtest/map_nonconst_ctor_on_const_ptr_3.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/failtest/map_nonconst_ctor_on_const_ptr_4.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/failtest/map_on_const_type_actually_const_0.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/failtest/map_on_const_type_actually_const_1.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/failtest/partialpivlu_int.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/failtest/qr_int.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/failtest/ref_1.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/failtest/ref_2.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/failtest/ref_3.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/failtest/ref_4.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/failtest/ref_5.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/failtest/selfadjointview_nonconst_ctor_on_const_xpr.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/failtest/selfadjointview_on_const_type_actually_const.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      302 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/failtest/sparse_ref_1.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/failtest/sparse_ref_2.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/failtest/sparse_ref_3.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/failtest/sparse_ref_4.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/failtest/sparse_ref_5.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/failtest/sparse_storage_mismatch.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/failtest/swap_1.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/failtest/swap_2.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/failtest/ternary_1.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/failtest/ternary_2.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/failtest/transpose_nonconst_ctor_on_const_xpr.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/failtest/transpose_on_const_type_actually_const.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/failtest/triangularview_nonconst_ctor_on_const_xpr.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/failtest/triangularview_on_const_type_actually_const.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 14:34:30.617841 stag-1.2.1/stag/eigen-3.3.9/lapack/
--rw-r--r--   0 runner    (1001) docker     (123)    10970 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/lapack/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/lapack/cholesky.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2831 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/lapack/clacgv.f
--rw-r--r--   0 runner    (1001) docker     (123)     2340 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/lapack/cladiv.f
--rw-r--r--   0 runner    (1001) docker     (123)     6295 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/lapack/clarf.f
--rw-r--r--   0 runner    (1001) docker     (123)    23424 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/lapack/clarfb.f
--rw-r--r--   0 runner    (1001) docker     (123)     5344 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/lapack/clarfg.f
--rw-r--r--   0 runner    (1001) docker     (123)    10450 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/lapack/clarft.f
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/lapack/complex_double.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      577 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/lapack/complex_single.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2969 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/lapack/dladiv.f
--rw-r--r--   0 runner    (1001) docker     (123)     5259 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/lapack/dlamch.f
--rw-r--r--   0 runner    (1001) docker     (123)     2514 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/lapack/dlapy2.f
--rw-r--r--   0 runner    (1001) docker     (123)     2737 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/lapack/dlapy3.f
--rw-r--r--   0 runner    (1001) docker     (123)     6167 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/lapack/dlarf.f
--rw-r--r--   0 runner    (1001) docker     (123)    22749 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/lapack/dlarfb.f
--rw-r--r--   0 runner    (1001) docker     (123)     4946 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/lapack/dlarfg.f
--rw-r--r--   0 runner    (1001) docker     (123)    10222 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/lapack/dlarft.f
--rw-r--r--   0 runner    (1001) docker     (123)      562 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/lapack/double.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/lapack/dsecnd_NONE.f
--rw-r--r--   0 runner    (1001) docker     (123)     1826 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/lapack/eigenvalues.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2957 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/lapack/ilaclc.f
--rw-r--r--   0 runner    (1001) docker     (123)     2997 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/lapack/ilaclr.f
--rw-r--r--   0 runner    (1001) docker     (123)     2952 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/lapack/iladlc.f
--rw-r--r--   0 runner    (1001) docker     (123)     3000 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/lapack/iladlr.f
--rw-r--r--   0 runner    (1001) docker     (123)     2941 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/lapack/ilaslc.f
--rw-r--r--   0 runner    (1001) docker     (123)     2988 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/lapack/ilaslr.f
--rw-r--r--   0 runner    (1001) docker     (123)     2962 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/lapack/ilazlc.f
--rw-r--r--   0 runner    (1001) docker     (123)     3010 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/lapack/ilazlr.f
--rw-r--r--   0 runner    (1001) docker     (123)      877 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/lapack/lapack_common.h
--rw-r--r--   0 runner    (1001) docker     (123)     2655 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/lapack/lu.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1258 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/lapack/second_NONE.f
--rw-r--r--   0 runner    (1001) docker     (123)      561 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/lapack/single.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2897 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/lapack/sladiv.f
--rw-r--r--   0 runner    (1001) docker     (123)     5261 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/lapack/slamch.f
--rw-r--r--   0 runner    (1001) docker     (123)     2490 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/lapack/slapy2.f
--rw-r--r--   0 runner    (1001) docker     (123)     2701 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/lapack/slapy3.f
--rw-r--r--   0 runner    (1001) docker     (123)     6117 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/lapack/slarf.f
--rw-r--r--   0 runner    (1001) docker     (123)    22727 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/lapack/slarfb.f
--rw-r--r--   0 runner    (1001) docker     (123)     4908 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/lapack/slarfg.f
--rw-r--r--   0 runner    (1001) docker     (123)    10183 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/lapack/slarft.f
--rw-r--r--   0 runner    (1001) docker     (123)     4891 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/lapack/svd.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2839 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/lapack/zlacgv.f
--rw-r--r--   0 runner    (1001) docker     (123)     2364 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/lapack/zladiv.f
--rw-r--r--   0 runner    (1001) docker     (123)     6278 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/lapack/zlarf.f
--rw-r--r--   0 runner    (1001) docker     (123)    23498 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/lapack/zlarfb.f
--rw-r--r--   0 runner    (1001) docker     (123)     5359 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/lapack/zlarfg.f
--rw-r--r--   0 runner    (1001) docker     (123)    10453 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/lapack/zlarft.f
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 14:34:30.621841 stag-1.2.1/stag/eigen-3.3.9/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/scripts/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1566 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/scripts/cdashtesting.cmake.in
--rwxr-xr-x   0 runner    (1001) docker     (123)      670 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/scripts/check.in
--rwxr-xr-x   0 runner    (1001) docker     (123)       44 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/scripts/debug.in
--rw-r--r--   0 runner    (1001) docker     (123)     6384 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/scripts/eigen_gen_credits.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      738 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/scripts/eigen_gen_docs
--rwxr-xr-x   0 runner    (1001) docker     (123)       46 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/scripts/release.in
--rw-r--r--   0 runner    (1001) docker     (123)     2368 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/scripts/relicense.py
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/signature_of_eigen3_matrix_library
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 14:34:30.633841 stag-1.2.1/stag/eigen-3.3.9/test/
--rw-r--r--   0 runner    (1001) docker     (123)    12229 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/test/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     8251 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/test/adjoint.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    19209 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/test/array_cwise.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    12295 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/test/array_for_matrix.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      953 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/test/array_of_string.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2334 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/test/array_replicate.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4877 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/test/array_reverse.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2424 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/test/bandmatrix.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    10604 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/test/basicstuff.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4275 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/test/bdcsvd.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/test/bicgstab.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    11602 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/test/block.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     5534 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/test/boostmultiprec.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/test/bug1213.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/test/bug1213.h
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/test/bug1213_main.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    17757 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/test/cholesky.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2686 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/test/cholmod_support.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2923 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/test/commainitializer.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/test/conjugate_gradient.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4280 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/test/conservative_resize.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2554 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/test/constructor.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     6440 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/test/corners.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/test/ctorleak.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     5345 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/test/cuda_basic.cu
--rw-r--r--   0 runner    (1001) docker     (123)     3368 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/test/cuda_common.h
--rw-r--r--   0 runner    (1001) docker     (123)     5054 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/test/denseLM.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2579 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/test/dense_storage.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2267 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/test/determinant.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4107 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/test/diagonal.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     7157 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/test/diagonalmatrices.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2221 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/test/dontalign.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4630 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/test/dynalloc.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2188 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/test/eigen2support.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     6212 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/test/eigensolver_complex.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4038 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/test/eigensolver_generalized_real.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     6172 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/test/eigensolver_generic.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    11023 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/test/eigensolver_selfadjoint.cpp
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/test/evaluator_common.h
--rw-r--r--   0 runner    (1001) docker     (123)    19757 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/test/evaluators.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3669 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/test/exceptions.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     5248 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/test/fastmath.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1866 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/test/first_aligned.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     5584 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/test/geo_alignedbox.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3554 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/test/geo_eulerangles.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     5462 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/test/geo_homogeneous.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     7556 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/test/geo_hyperplane.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4830 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/test/geo_orthomethods.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3916 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/test/geo_parametrizedline.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    11125 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/test/geo_quaternion.cpp
--rwxr-xr-x   0 runner    (1001) docker     (123)    25326 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/test/geo_transformations.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    10819 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/test/half_float.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2396 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/test/hessenberg.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     5940 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/test/householder.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2572 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/test/incomplete_cholesky.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3872 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/test/inplace_decomposition.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     5688 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/test/integer_types.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4205 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/test/inverse.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/test/is_same_dense.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2725 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/test/jacobi.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     5453 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/test/jacobisvd.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     6089 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/test/linearstructure.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/test/lscg.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     9867 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/test/lu.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    31942 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/test/main.h
--rw-r--r--   0 runner    (1001) docker     (123)     7940 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/test/mapped_matrix.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     7300 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/test/mapstaticmethods.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    10112 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/test/mapstride.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4715 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/test/meta.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      743 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/test/metis_support.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1781 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/test/miscmatrices.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    17752 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/test/mixingtypes.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/test/mpl2only.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4369 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/test/nesting_ops.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     8713 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/test/nomalloc.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    11724 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/test/nullary.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1704 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/test/numext.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    24039 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/test/packetmath.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      947 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/test/pardiso_support.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1894 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/test/pastix_support.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     6298 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/test/permutationmatrices.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3196 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/test/prec_inverse_4x4.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    11826 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/test/product.h
--rw-r--r--   0 runner    (1001) docker     (123)    14544 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/test/product_extra.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4352 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/test/product_large.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4439 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/test/product_mmtr.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     8803 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/test/product_notemporary.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3502 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/test/product_selfadjoint.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    11857 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/test/product_small.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     6125 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/test/product_symm.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     7848 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/test/product_syrk.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     6913 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/test/product_trmm.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4242 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/test/product_trmv.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     6094 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/test/product_trsolve.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4586 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/test/qr.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    12543 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/test/qr_colpivoting.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     5242 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/test/qr_fullpivoting.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4613 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/test/qtvector.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4365 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/test/rand.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3094 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/test/real_qz.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     7906 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/test/redux.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    11718 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/test/ref.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/test/resize.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4306 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/test/rvalue_types.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3561 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/test/schur_complex.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3956 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/test/schur_real.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2411 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/test/selfadjoint.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2147 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/test/simplicial_cholesky.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2051 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/test/sizeof.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2631 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/test/sizeoverflow.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2125 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/test/smallvectors.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     6396 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/test/sparse.h
--rw-r--r--   0 runner    (1001) docker     (123)     4732 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/test/sparseLM.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    26098 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/test/sparse_basic.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    11867 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/test/sparse_block.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     9989 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/test/sparse_permutations.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    25566 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/test/sparse_product.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     6117 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/test/sparse_ref.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    19059 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/test/sparse_solver.h
--rw-r--r--   0 runner    (1001) docker     (123)     4691 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/test/sparse_solvers.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     5079 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/test/sparse_vector.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1783 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/test/sparselu.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3815 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/test/sparseqr.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1754 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/test/special_numbers.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/test/spqr_support.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     8474 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/test/stable_norm.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4252 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/test/stddeque.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4772 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/test/stddeque_overload.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4224 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/test/stdlist.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     5886 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/test/stdlist_overload.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     5150 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/test/stdvector.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     5048 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/test/stdvector_overload.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      948 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/test/superlu_support.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    17971 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/test/svd_common.h
--rw-r--r--   0 runner    (1001) docker     (123)     4050 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/test/svd_fill.h
--rw-r--r--   0 runner    (1001) docker     (123)     2974 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/test/swap.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     9470 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/test/triangular.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     5853 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/test/umeyama.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      991 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/test/umfpack_support.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     5857 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/test/unalignedassert.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2134 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/test/unalignedcount.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/test/upperbidiagonalization.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    20436 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/test/vectorization_logic.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     8627 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/test/vectorwiseop.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3994 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/test/visitor.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3384 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/test/zerosized.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 14:34:30.633841 stag-1.2.1/stag/eigen-3.3.9/unsupported/
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/unsupported/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 14:34:30.633841 stag-1.2.1/stag/eigen-3.3.9/unsupported/Eigen/
--rw-r--r--   0 runner    (1001) docker     (123)     4241 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/unsupported/Eigen/AdolcForward
--rw-r--r--   0 runner    (1001) docker     (123)     6095 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/unsupported/Eigen/AlignedVector3
--rw-r--r--   0 runner    (1001) docker     (123)      905 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/unsupported/Eigen/ArpackSupport
--rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/unsupported/Eigen/AutoDiff
--rw-r--r--   0 runner    (1001) docker     (123)     5505 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/unsupported/Eigen/BVH
--rw-r--r--   0 runner    (1001) docker     (123)      603 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/unsupported/Eigen/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 14:34:30.637841 stag-1.2.1/stag/eigen-3.3.9/unsupported/Eigen/CXX11/
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/unsupported/Eigen/CXX11/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4313 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/unsupported/Eigen/CXX11/Tensor
--rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/unsupported/Eigen/CXX11/TensorSymmetry
--rw-r--r--   0 runner    (1001) docker     (123)     1743 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/unsupported/Eigen/CXX11/ThreadPool
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 14:34:30.485841 stag-1.2.1/stag/eigen-3.3.9/unsupported/Eigen/CXX11/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 14:34:30.641841 stag-1.2.1/stag/eigen-3.3.9/unsupported/Eigen/CXX11/src/Tensor/
--rw-r--r--   0 runner    (1001) docker     (123)    60362 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/unsupported/Eigen/CXX11/src/Tensor/README.md
--rw-r--r--   0 runner    (1001) docker     (123)    20561 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/unsupported/Eigen/CXX11/src/Tensor/Tensor.h
--rw-r--r--   0 runner    (1001) docker     (123)    11022 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/unsupported/Eigen/CXX11/src/Tensor/TensorArgMax.h
--rw-r--r--   0 runner    (1001) docker     (123)     7676 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/unsupported/Eigen/CXX11/src/Tensor/TensorAssign.h
--rw-r--r--   0 runner    (1001) docker     (123)    49692 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/unsupported/Eigen/CXX11/src/Tensor/TensorBase.h
--rw-r--r--   0 runner    (1001) docker     (123)    14286 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/unsupported/Eigen/CXX11/src/Tensor/TensorBroadcasting.h
--rw-r--r--   0 runner    (1001) docker     (123)    14755 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/unsupported/Eigen/CXX11/src/Tensor/TensorChipping.h
--rw-r--r--   0 runner    (1001) docker     (123)    14653 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/unsupported/Eigen/CXX11/src/Tensor/TensorConcatenation.h
--rw-r--r--   0 runner    (1001) docker     (123)    26680 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/unsupported/Eigen/CXX11/src/Tensor/TensorContraction.h
--rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/unsupported/Eigen/CXX11/src/Tensor/TensorContractionBlocking.h
--rw-r--r--   0 runner    (1001) docker     (123)    62023 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/unsupported/Eigen/CXX11/src/Tensor/TensorContractionCuda.h
--rw-r--r--   0 runner    (1001) docker     (123)    18786 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/unsupported/Eigen/CXX11/src/Tensor/TensorContractionMapper.h
--rw-r--r--   0 runner    (1001) docker     (123)    44052 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/unsupported/Eigen/CXX11/src/Tensor/TensorContractionThreadPool.h
--rw-r--r--   0 runner    (1001) docker     (123)    11006 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/unsupported/Eigen/CXX11/src/Tensor/TensorConversion.h
--rw-r--r--   0 runner    (1001) docker     (123)    47585 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/unsupported/Eigen/CXX11/src/Tensor/TensorConvolution.h
--rw-r--r--   0 runner    (1001) docker     (123)     8443 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/unsupported/Eigen/CXX11/src/Tensor/TensorCostModel.h
--rw-r--r--   0 runner    (1001) docker     (123)    11445 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/unsupported/Eigen/CXX11/src/Tensor/TensorCustomOp.h
--rw-r--r--   0 runner    (1001) docker     (123)     2570 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/unsupported/Eigen/CXX11/src/Tensor/TensorDevice.h
--rw-r--r--   0 runner    (1001) docker     (123)    11080 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/unsupported/Eigen/CXX11/src/Tensor/TensorDeviceCuda.h
--rw-r--r--   0 runner    (1001) docker     (123)     2474 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/unsupported/Eigen/CXX11/src/Tensor/TensorDeviceDefault.h
--rw-r--r--   0 runner    (1001) docker     (123)     5196 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/unsupported/Eigen/CXX11/src/Tensor/TensorDeviceSycl.h
--rw-r--r--   0 runner    (1001) docker     (123)     9937 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/unsupported/Eigen/CXX11/src/Tensor/TensorDeviceThreadPool.h
--rw-r--r--   0 runner    (1001) docker     (123)     7674 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/unsupported/Eigen/CXX11/src/Tensor/TensorDimensionList.h
--rw-r--r--   0 runner    (1001) docker     (123)    15529 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/unsupported/Eigen/CXX11/src/Tensor/TensorDimensions.h
--rw-r--r--   0 runner    (1001) docker     (123)     6560 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/unsupported/Eigen/CXX11/src/Tensor/TensorEvalTo.h
--rw-r--r--   0 runner    (1001) docker     (123)    25305 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/unsupported/Eigen/CXX11/src/Tensor/TensorEvaluator.h
--rw-r--r--   0 runner    (1001) docker     (123)    10248 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/unsupported/Eigen/CXX11/src/Tensor/TensorExecutor.h
--rw-r--r--   0 runner    (1001) docker     (123)    14694 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/unsupported/Eigen/CXX11/src/Tensor/TensorExpr.h
--rw-r--r--   0 runner    (1001) docker     (123)    23299 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/unsupported/Eigen/CXX11/src/Tensor/TensorFFT.h
--rw-r--r--   0 runner    (1001) docker     (123)    14916 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/unsupported/Eigen/CXX11/src/Tensor/TensorFixedSize.h
--rw-r--r--   0 runner    (1001) docker     (123)     6595 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/unsupported/Eigen/CXX11/src/Tensor/TensorForcedEval.h
--rw-r--r--   0 runner    (1001) docker     (123)     5412 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/unsupported/Eigen/CXX11/src/Tensor/TensorForwardDeclarations.h
--rw-r--r--   0 runner    (1001) docker     (123)    14625 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/unsupported/Eigen/CXX11/src/Tensor/TensorFunctors.h
--rw-r--r--   0 runner    (1001) docker     (123)     6341 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/unsupported/Eigen/CXX11/src/Tensor/TensorGenerator.h
--rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/unsupported/Eigen/CXX11/src/Tensor/TensorGlobalFunctions.h
--rw-r--r--   0 runner    (1001) docker     (123)     2560 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/unsupported/Eigen/CXX11/src/Tensor/TensorIO.h
--rw-r--r--   0 runner    (1001) docker     (123)    23098 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/unsupported/Eigen/CXX11/src/Tensor/TensorImagePatch.h
--rw-r--r--   0 runner    (1001) docker     (123)    25810 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/unsupported/Eigen/CXX11/src/Tensor/TensorIndexList.h
--rw-r--r--   0 runner    (1001) docker     (123)     8430 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/unsupported/Eigen/CXX11/src/Tensor/TensorInflation.h
--rw-r--r--   0 runner    (1001) docker     (123)     2716 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/unsupported/Eigen/CXX11/src/Tensor/TensorInitializer.h
--rw-r--r--   0 runner    (1001) docker     (123)     8527 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/unsupported/Eigen/CXX11/src/Tensor/TensorIntDiv.h
--rw-r--r--   0 runner    (1001) docker     (123)     7354 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/unsupported/Eigen/CXX11/src/Tensor/TensorLayoutSwap.h
--rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/unsupported/Eigen/CXX11/src/Tensor/TensorMacros.h
--rw-r--r--   0 runner    (1001) docker     (123)    13527 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/unsupported/Eigen/CXX11/src/Tensor/TensorMap.h
--rw-r--r--   0 runner    (1001) docker     (123)     5309 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/unsupported/Eigen/CXX11/src/Tensor/TensorMeta.h
--rw-r--r--   0 runner    (1001) docker     (123)    34277 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/unsupported/Eigen/CXX11/src/Tensor/TensorMorphing.h
--rw-r--r--   0 runner    (1001) docker     (123)    15746 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/unsupported/Eigen/CXX11/src/Tensor/TensorPadding.h
--rw-r--r--   0 runner    (1001) docker     (123)    10687 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/unsupported/Eigen/CXX11/src/Tensor/TensorPatch.h
--rw-r--r--   0 runner    (1001) docker     (123)     9298 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/unsupported/Eigen/CXX11/src/Tensor/TensorRandom.h
--rw-r--r--   0 runner    (1001) docker     (123)    33938 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/unsupported/Eigen/CXX11/src/Tensor/TensorReduction.h
--rw-r--r--   0 runner    (1001) docker     (123)    30324 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/unsupported/Eigen/CXX11/src/Tensor/TensorReductionCuda.h
--rw-r--r--   0 runner    (1001) docker     (123)    14052 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/unsupported/Eigen/CXX11/src/Tensor/TensorReductionSycl.h
--rw-r--r--   0 runner    (1001) docker     (123)    13633 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/unsupported/Eigen/CXX11/src/Tensor/TensorRef.h
--rw-r--r--   0 runner    (1001) docker     (123)    10527 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/unsupported/Eigen/CXX11/src/Tensor/TensorReverse.h
--rw-r--r--   0 runner    (1001) docker     (123)     9941 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/unsupported/Eigen/CXX11/src/Tensor/TensorScan.h
--rw-r--r--   0 runner    (1001) docker     (123)     9489 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/unsupported/Eigen/CXX11/src/Tensor/TensorShuffling.h
--rw-r--r--   0 runner    (1001) docker     (123)     5100 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/unsupported/Eigen/CXX11/src/Tensor/TensorStorage.h
--rw-r--r--   0 runner    (1001) docker     (123)    13196 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/unsupported/Eigen/CXX11/src/Tensor/TensorStriding.h
--rw-r--r--   0 runner    (1001) docker     (123)     2446 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/unsupported/Eigen/CXX11/src/Tensor/TensorSycl.h
--rw-r--r--   0 runner    (1001) docker     (123)     5046 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/unsupported/Eigen/CXX11/src/Tensor/TensorSyclConvertToDeviceExpression.h
--rw-r--r--   0 runner    (1001) docker     (123)    11561 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/unsupported/Eigen/CXX11/src/Tensor/TensorSyclExprConstructor.h
--rw-r--r--   0 runner    (1001) docker     (123)    12530 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/unsupported/Eigen/CXX11/src/Tensor/TensorSyclExtractAccessor.h
--rw-r--r--   0 runner    (1001) docker     (123)     9699 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/unsupported/Eigen/CXX11/src/Tensor/TensorSyclExtractFunctors.h
--rw-r--r--   0 runner    (1001) docker     (123)     5288 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/unsupported/Eigen/CXX11/src/Tensor/TensorSyclLeafCount.h
--rw-r--r--   0 runner    (1001) docker     (123)     6692 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/unsupported/Eigen/CXX11/src/Tensor/TensorSyclPlaceHolderExpr.h
--rw-r--r--   0 runner    (1001) docker     (123)     3090 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/unsupported/Eigen/CXX11/src/Tensor/TensorSyclRun.h
--rw-r--r--   0 runner    (1001) docker     (123)     9752 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/unsupported/Eigen/CXX11/src/Tensor/TensorSyclTuple.h
--rw-r--r--   0 runner    (1001) docker     (123)     9454 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/unsupported/Eigen/CXX11/src/Tensor/TensorTraits.h
--rw-r--r--   0 runner    (1001) docker     (123)     7522 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/unsupported/Eigen/CXX11/src/Tensor/TensorUInt128.h
--rw-r--r--   0 runner    (1001) docker     (123)    28192 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/unsupported/Eigen/CXX11/src/Tensor/TensorVolumePatch.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 14:34:30.641841 stag-1.2.1/stag/eigen-3.3.9/unsupported/Eigen/CXX11/src/TensorSymmetry/
--rw-r--r--   0 runner    (1001) docker     (123)    10857 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/unsupported/Eigen/CXX11/src/TensorSymmetry/DynamicSymmetry.h
--rw-r--r--   0 runner    (1001) docker     (123)     9086 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/unsupported/Eigen/CXX11/src/TensorSymmetry/StaticSymmetry.h
--rw-r--r--   0 runner    (1001) docker     (123)    13021 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/unsupported/Eigen/CXX11/src/TensorSymmetry/Symmetry.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 14:34:30.641841 stag-1.2.1/stag/eigen-3.3.9/unsupported/Eigen/CXX11/src/TensorSymmetry/util/
--rw-r--r--   0 runner    (1001) docker     (123)    21047 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/unsupported/Eigen/CXX11/src/TensorSymmetry/util/TemplateGroupTheory.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 14:34:30.645841 stag-1.2.1/stag/eigen-3.3.9/unsupported/Eigen/CXX11/src/ThreadPool/
--rw-r--r--   0 runner    (1001) docker     (123)     8705 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/unsupported/Eigen/CXX11/src/ThreadPool/EventCount.h
--rw-r--r--   0 runner    (1001) docker     (123)     9419 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/unsupported/Eigen/CXX11/src/ThreadPool/NonBlockingThreadPool.h
--rw-r--r--   0 runner    (1001) docker     (123)     8450 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/unsupported/Eigen/CXX11/src/ThreadPool/RunQueue.h
--rw-r--r--   0 runner    (1001) docker     (123)     4323 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/unsupported/Eigen/CXX11/src/ThreadPool/SimpleThreadPool.h
--rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/unsupported/Eigen/CXX11/src/ThreadPool/ThreadEnvironment.h
--rw-r--r--   0 runner    (1001) docker     (123)      801 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/unsupported/Eigen/CXX11/src/ThreadPool/ThreadLocal.h
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/unsupported/Eigen/CXX11/src/ThreadPool/ThreadPoolInterface.h
--rw-r--r--   0 runner    (1001) docker     (123)      715 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/unsupported/Eigen/CXX11/src/ThreadPool/ThreadYield.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 14:34:30.645841 stag-1.2.1/stag/eigen-3.3.9/unsupported/Eigen/CXX11/src/util/
--rw-r--r--   0 runner    (1001) docker     (123)    22317 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/unsupported/Eigen/CXX11/src/util/CXX11Meta.h
--rw-r--r--   0 runner    (1001) docker     (123)     4137 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/unsupported/Eigen/CXX11/src/util/CXX11Workarounds.h
--rw-r--r--   0 runner    (1001) docker     (123)     8298 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/unsupported/Eigen/CXX11/src/util/EmulateArray.h
--rw-r--r--   0 runner    (1001) docker     (123)     9377 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/unsupported/Eigen/CXX11/src/util/EmulateCXX11Meta.h
--rw-r--r--   0 runner    (1001) docker     (123)     3760 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/unsupported/Eigen/CXX11/src/util/MaxSizeVector.h
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/unsupported/Eigen/EulerAngles
--rw-r--r--   0 runner    (1001) docker     (123)    13979 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/unsupported/Eigen/FFT
--rw-r--r--   0 runner    (1001) docker     (123)     1295 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/unsupported/Eigen/IterativeSolvers
--rw-r--r--   0 runner    (1001) docker     (123)      944 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/unsupported/Eigen/KroneckerProduct
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/unsupported/Eigen/LevenbergMarquardt
--rw-r--r--   0 runner    (1001) docker     (123)     7413 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/unsupported/Eigen/MPRealSupport
--rw-r--r--   0 runner    (1001) docker     (123)    17776 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/unsupported/Eigen/MatrixFunctions
--rw-r--r--   0 runner    (1001) docker     (123)      586 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/unsupported/Eigen/MoreVectorization
--rw-r--r--   0 runner    (1001) docker     (123)     5776 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/unsupported/Eigen/NonLinearOptimization
--rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/unsupported/Eigen/NumericalDiff
--rw-r--r--   0 runner    (1001) docker     (123)    19066 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/unsupported/Eigen/OpenGLSupport
--rw-r--r--   0 runner    (1001) docker     (123)     4770 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/unsupported/Eigen/Polynomials
--rw-r--r--   0 runner    (1001) docker     (123)      912 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/unsupported/Eigen/Skyline
--rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/unsupported/Eigen/SparseExtra
--rw-r--r--   0 runner    (1001) docker     (123)     1574 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/unsupported/Eigen/SpecialFunctions
--rw-r--r--   0 runner    (1001) docker     (123)      871 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/unsupported/Eigen/Splines
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 14:34:30.489841 stag-1.2.1/stag/eigen-3.3.9/unsupported/Eigen/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 14:34:30.645841 stag-1.2.1/stag/eigen-3.3.9/unsupported/Eigen/src/AutoDiff/
--rw-r--r--   0 runner    (1001) docker     (123)     3150 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/unsupported/Eigen/src/AutoDiff/AutoDiffJacobian.h
--rwxr-xr-x   0 runner    (1001) docker     (123)    29061 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/unsupported/Eigen/src/AutoDiff/AutoDiffScalar.h
--rw-r--r--   0 runner    (1001) docker     (123)     9029 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/unsupported/Eigen/src/AutoDiff/AutoDiffVector.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 14:34:30.645841 stag-1.2.1/stag/eigen-3.3.9/unsupported/Eigen/src/BVH/
--rw-r--r--   0 runner    (1001) docker     (123)    12976 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/unsupported/Eigen/src/BVH/BVAlgorithms.h
--rw-r--r--   0 runner    (1001) docker     (123)     9166 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/unsupported/Eigen/src/BVH/KdBVH.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 14:34:30.645841 stag-1.2.1/stag/eigen-3.3.9/unsupported/Eigen/src/Eigenvalues/
--rw-r--r--   0 runner    (1001) docker     (123)    29062 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/unsupported/Eigen/src/Eigenvalues/ArpackSelfAdjointEigenSolver.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 14:34:30.645841 stag-1.2.1/stag/eigen-3.3.9/unsupported/Eigen/src/EulerAngles/
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/unsupported/Eigen/src/EulerAngles/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)    16755 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/unsupported/Eigen/src/EulerAngles/EulerAngles.h
--rw-r--r--   0 runner    (1001) docker     (123)    11467 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/unsupported/Eigen/src/EulerAngles/EulerSystem.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 14:34:30.645841 stag-1.2.1/stag/eigen-3.3.9/unsupported/Eigen/src/FFT/
--rw-r--r--   0 runner    (1001) docker     (123)     9269 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/unsupported/Eigen/src/FFT/ei_fftw_impl.h
--rw-r--r--   0 runner    (1001) docker     (123)    12275 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/unsupported/Eigen/src/FFT/ei_kissfft_impl.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 14:34:30.645841 stag-1.2.1/stag/eigen-3.3.9/unsupported/Eigen/src/IterativeSolvers/
--rw-r--r--   0 runner    (1001) docker     (123)     5379 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/unsupported/Eigen/src/IterativeSolvers/ConstrainedConjGrad.h
--rw-r--r--   0 runner    (1001) docker     (123)    17769 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/unsupported/Eigen/src/IterativeSolvers/DGMRES.h
--rw-r--r--   0 runner    (1001) docker     (123)    10442 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/unsupported/Eigen/src/IterativeSolvers/GMRES.h
--rw-r--r--   0 runner    (1001) docker     (123)     2520 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/unsupported/Eigen/src/IterativeSolvers/IncompleteLU.h
--rw-r--r--   0 runner    (1001) docker     (123)     5354 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/unsupported/Eigen/src/IterativeSolvers/IterationController.h
--rw-r--r--   0 runner    (1001) docker     (123)    13264 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/unsupported/Eigen/src/IterativeSolvers/MINRES.h
--rw-r--r--   0 runner    (1001) docker     (123)     5739 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/unsupported/Eigen/src/IterativeSolvers/Scaling.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 14:34:30.645841 stag-1.2.1/stag/eigen-3.3.9/unsupported/Eigen/src/KroneckerProduct/
--rw-r--r--   0 runner    (1001) docker     (123)    10230 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/unsupported/Eigen/src/KroneckerProduct/KroneckerTensorProduct.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 14:34:30.645841 stag-1.2.1/stag/eigen-3.3.9/unsupported/Eigen/src/LevenbergMarquardt/
--rw-r--r--   0 runner    (1001) docker     (123)     2194 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/unsupported/Eigen/src/LevenbergMarquardt/CopyrightMINPACK.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2443 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/unsupported/Eigen/src/LevenbergMarquardt/LMcovar.h
--rw-r--r--   0 runner    (1001) docker     (123)     6648 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/unsupported/Eigen/src/LevenbergMarquardt/LMonestep.h
--rw-r--r--   0 runner    (1001) docker     (123)     5039 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/unsupported/Eigen/src/LevenbergMarquardt/LMpar.h
--rw-r--r--   0 runner    (1001) docker     (123)     6804 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/unsupported/Eigen/src/LevenbergMarquardt/LMqrsolv.h
--rw-r--r--   0 runner    (1001) docker     (123)    13292 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/unsupported/Eigen/src/LevenbergMarquardt/LevenbergMarquardt.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 14:34:30.645841 stag-1.2.1/stag/eigen-3.3.9/unsupported/Eigen/src/MatrixFunctions/
--rw-r--r--   0 runner    (1001) docker     (123)    16666 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/unsupported/Eigen/src/MatrixFunctions/MatrixExponential.h
--rw-r--r--   0 runner    (1001) docker     (123)    23257 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/unsupported/Eigen/src/MatrixFunctions/MatrixFunction.h
--rw-r--r--   0 runner    (1001) docker     (123)    17427 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/unsupported/Eigen/src/MatrixFunctions/MatrixLogarithm.h
--rw-r--r--   0 runner    (1001) docker     (123)    23511 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/unsupported/Eigen/src/MatrixFunctions/MatrixPower.h
--rw-r--r--   0 runner    (1001) docker     (123)    14405 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/unsupported/Eigen/src/MatrixFunctions/MatrixSquareRoot.h
--rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/unsupported/Eigen/src/MatrixFunctions/StemFunction.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 14:34:30.645841 stag-1.2.1/stag/eigen-3.3.9/unsupported/Eigen/src/MoreVectorization/
--rw-r--r--   0 runner    (1001) docker     (123)     3035 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/unsupported/Eigen/src/MoreVectorization/MathFunctions.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 14:34:30.649841 stag-1.2.1/stag/eigen-3.3.9/unsupported/Eigen/src/NonLinearOptimization/
--rw-r--r--   0 runner    (1001) docker     (123)    19828 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/unsupported/Eigen/src/NonLinearOptimization/HybridNonLinearSolver.h
--rw-r--r--   0 runner    (1001) docker     (123)    22135 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/unsupported/Eigen/src/NonLinearOptimization/LevenbergMarquardt.h
--rw-r--r--   0 runner    (1001) docker     (123)     1864 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/unsupported/Eigen/src/NonLinearOptimization/chkder.h
--rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/unsupported/Eigen/src/NonLinearOptimization/covar.h
--rw-r--r--   0 runner    (1001) docker     (123)     3297 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/unsupported/Eigen/src/NonLinearOptimization/dogleg.h
--rw-r--r--   0 runner    (1001) docker     (123)     2225 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/unsupported/Eigen/src/NonLinearOptimization/fdjac1.h
--rw-r--r--   0 runner    (1001) docker     (123)     9111 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/unsupported/Eigen/src/NonLinearOptimization/lmpar.h
--rw-r--r--   0 runner    (1001) docker     (123)     3263 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/unsupported/Eigen/src/NonLinearOptimization/qrsolv.h
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/unsupported/Eigen/src/NonLinearOptimization/r1mpyq.h
--rw-r--r--   0 runner    (1001) docker     (123)     3082 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/unsupported/Eigen/src/NonLinearOptimization/r1updt.h
--rw-r--r--   0 runner    (1001) docker     (123)     1362 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/unsupported/Eigen/src/NonLinearOptimization/rwupdt.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 14:34:30.649841 stag-1.2.1/stag/eigen-3.3.9/unsupported/Eigen/src/NumericalDiff/
--rw-r--r--   0 runner    (1001) docker     (123)     4020 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/unsupported/Eigen/src/NumericalDiff/NumericalDiff.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 14:34:30.649841 stag-1.2.1/stag/eigen-3.3.9/unsupported/Eigen/src/Polynomials/
--rw-r--r--   0 runner    (1001) docker     (123)     7836 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/unsupported/Eigen/src/Polynomials/Companion.h
--rw-r--r--   0 runner    (1001) docker     (123)    15683 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/unsupported/Eigen/src/Polynomials/PolynomialSolver.h
--rw-r--r--   0 runner    (1001) docker     (123)     4806 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/unsupported/Eigen/src/Polynomials/PolynomialUtils.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 14:34:30.649841 stag-1.2.1/stag/eigen-3.3.9/unsupported/Eigen/src/Skyline/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/unsupported/Eigen/src/Skyline/SkylineInplaceLU.h
--rw-r--r--   0 runner    (1001) docker     (123)    31065 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/unsupported/Eigen/src/Skyline/SkylineMatrix.h
--rw-r--r--   0 runner    (1001) docker     (123)     7745 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/unsupported/Eigen/src/Skyline/SkylineMatrixBase.h
--rw-r--r--   0 runner    (1001) docker     (123)    10853 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/unsupported/Eigen/src/Skyline/SkylineProduct.h
--rw-r--r--   0 runner    (1001) docker     (123)     7969 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/unsupported/Eigen/src/Skyline/SkylineStorage.h
--rw-r--r--   0 runner    (1001) docker     (123)     3153 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/unsupported/Eigen/src/Skyline/SkylineUtil.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 14:34:30.649841 stag-1.2.1/stag/eigen-3.3.9/unsupported/Eigen/src/SparseExtra/
--rw-r--r--   0 runner    (1001) docker     (123)     4260 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/unsupported/Eigen/src/SparseExtra/BlockOfDynamicSparseMatrix.h
--rw-r--r--   0 runner    (1001) docker     (123)    40316 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/unsupported/Eigen/src/SparseExtra/BlockSparseMatrix.h
--rw-r--r--   0 runner    (1001) docker     (123)    13744 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/unsupported/Eigen/src/SparseExtra/DynamicSparseMatrix.h
--rw-r--r--   0 runner    (1001) docker     (123)     7696 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/unsupported/Eigen/src/SparseExtra/MarketIO.h
--rw-r--r--   0 runner    (1001) docker     (123)     7568 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/unsupported/Eigen/src/SparseExtra/MatrixMarketIterator.h
--rw-r--r--   0 runner    (1001) docker     (123)    11788 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/unsupported/Eigen/src/SparseExtra/RandomSetter.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 14:34:30.649841 stag-1.2.1/stag/eigen-3.3.9/unsupported/Eigen/src/SpecialFunctions/
--rw-r--r--   0 runner    (1001) docker     (123)     5441 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/unsupported/Eigen/src/SpecialFunctions/SpecialFunctionsArrayAPI.h
--rw-r--r--   0 runner    (1001) docker     (123)     7907 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/unsupported/Eigen/src/SpecialFunctions/SpecialFunctionsFunctors.h
--rw-r--r--   0 runner    (1001) docker     (123)     2261 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/unsupported/Eigen/src/SpecialFunctions/SpecialFunctionsHalf.h
--rw-r--r--   0 runner    (1001) docker     (123)    42539 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/unsupported/Eigen/src/SpecialFunctions/SpecialFunctionsImpl.h
--rw-r--r--   0 runner    (1001) docker     (123)     2709 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/unsupported/Eigen/src/SpecialFunctions/SpecialFunctionsPacketMath.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 14:34:30.489841 stag-1.2.1/stag/eigen-3.3.9/unsupported/Eigen/src/SpecialFunctions/arch/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 14:34:30.649841 stag-1.2.1/stag/eigen-3.3.9/unsupported/Eigen/src/SpecialFunctions/arch/CUDA/
--rw-r--r--   0 runner    (1001) docker     (123)     4528 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/unsupported/Eigen/src/SpecialFunctions/arch/CUDA/CudaSpecialFunctions.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 14:34:30.649841 stag-1.2.1/stag/eigen-3.3.9/unsupported/Eigen/src/Splines/
--rw-r--r--   0 runner    (1001) docker     (123)    18315 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/unsupported/Eigen/src/Splines/Spline.h
--rw-r--r--   0 runner    (1001) docker     (123)    16400 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/unsupported/Eigen/src/Splines/SplineFitting.h
--rw-r--r--   0 runner    (1001) docker     (123)     4300 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/unsupported/Eigen/src/Splines/SplineFwd.h
--rw-r--r--   0 runner    (1001) docker     (123)     1875 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/unsupported/README.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 14:34:30.649841 stag-1.2.1/stag/eigen-3.3.9/unsupported/bench/
--rw-r--r--   0 runner    (1001) docker     (123)     3905 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/unsupported/bench/bench_svd.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 14:34:30.649841 stag-1.2.1/stag/eigen-3.3.9/unsupported/doc/
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/unsupported/doc/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)      830 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/unsupported/doc/Overview.dox
--rw-r--r--   0 runner    (1001) docker     (123)     5283 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/unsupported/doc/eigendoxy_layout.xml.in
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 14:34:30.653841 stag-1.2.1/stag/eigen-3.3.9/unsupported/doc/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     2108 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/unsupported/doc/examples/BVH_Example.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      667 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/unsupported/doc/examples/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/unsupported/doc/examples/EulerAngles.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2522 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/unsupported/doc/examples/FFT.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/unsupported/doc/examples/MatrixExponential.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      469 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/unsupported/doc/examples/MatrixFunction.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/unsupported/doc/examples/MatrixLogarithm.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/unsupported/doc/examples/MatrixPower.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      424 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/unsupported/doc/examples/MatrixPower_optimal.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      508 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/unsupported/doc/examples/MatrixSine.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      524 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/unsupported/doc/examples/MatrixSinh.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      434 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/unsupported/doc/examples/MatrixSquareRoot.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2392 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/unsupported/doc/examples/PolynomialSolver1.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      635 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/unsupported/doc/examples/PolynomialUtils1.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 14:34:30.653841 stag-1.2.1/stag/eigen-3.3.9/unsupported/doc/snippets/
--rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/unsupported/doc/snippets/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 14:34:30.661841 stag-1.2.1/stag/eigen-3.3.9/unsupported/test/
--rw-r--r--   0 runner    (1001) docker     (123)     7182 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/unsupported/test/BVH.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     9538 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/unsupported/test/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6481 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/unsupported/test/EulerAngles.cpp
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/unsupported/test/FFT.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     9225 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/unsupported/test/FFTW.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    64589 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/unsupported/test/NonLinearOptimization.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2850 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/unsupported/test/NumericalDiff.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2300 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/unsupported/test/alignedvector3.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    10980 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/unsupported/test/autodiff.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2934 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/unsupported/test/autodiff_scalar.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3992 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/unsupported/test/cxx11_eventcount.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    18732 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/unsupported/test/cxx11_meta.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3085 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/unsupported/test/cxx11_non_blocking_thread_pool.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     7016 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/unsupported/test/cxx11_runqueue.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     9142 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/unsupported/test/cxx11_tensor_argmax.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     8904 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/unsupported/test/cxx11_tensor_argmax_cuda.cu
--rw-r--r--   0 runner    (1001) docker     (123)     9699 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/unsupported/test/cxx11_tensor_assign.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2538 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/unsupported/test/cxx11_tensor_broadcast_sycl.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     5296 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/unsupported/test/cxx11_tensor_broadcasting.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2470 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/unsupported/test/cxx11_tensor_cast_float16_cuda.cu
--rw-r--r--   0 runner    (1001) docker     (123)     2991 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/unsupported/test/cxx11_tensor_casts.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    13040 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/unsupported/test/cxx11_tensor_chipping.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/unsupported/test/cxx11_tensor_comparisons.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     5270 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/unsupported/test/cxx11_tensor_complex_cuda.cu
--rw-r--r--   0 runner    (1001) docker     (123)     2758 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/unsupported/test/cxx11_tensor_complex_cwise_ops_cuda.cu
--rw-r--r--   0 runner    (1001) docker     (123)     4289 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/unsupported/test/cxx11_tensor_concatenation.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1652 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/unsupported/test/cxx11_tensor_const.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     7280 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/unsupported/test/cxx11_tensor_contract_cuda.cu
--rw-r--r--   0 runner    (1001) docker     (123)    21118 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/unsupported/test/cxx11_tensor_contraction.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     5362 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/unsupported/test/cxx11_tensor_convolution.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    46749 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/unsupported/test/cxx11_tensor_cuda.cu
--rw-r--r--   0 runner    (1001) docker     (123)     2510 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/unsupported/test/cxx11_tensor_custom_index.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3203 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/unsupported/test/cxx11_tensor_custom_op.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    13374 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/unsupported/test/cxx11_tensor_device.cu
--rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/unsupported/test/cxx11_tensor_device_sycl.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2099 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/unsupported/test/cxx11_tensor_dimension.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      991 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/unsupported/test/cxx11_tensor_empty.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     8407 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/unsupported/test/cxx11_tensor_expr.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    12770 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/unsupported/test/cxx11_tensor_fft.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     7234 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/unsupported/test/cxx11_tensor_fixed_size.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2159 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/unsupported/test/cxx11_tensor_forced_eval.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2755 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/unsupported/test/cxx11_tensor_forced_eval_sycl.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2250 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/unsupported/test/cxx11_tensor_generator.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     5934 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/unsupported/test/cxx11_tensor_ifft.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    33556 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/unsupported/test/cxx11_tensor_image_patch.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    18746 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/unsupported/test/cxx11_tensor_index_list.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2101 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/unsupported/test/cxx11_tensor_inflation.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4121 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/unsupported/test/cxx11_tensor_intdiv.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3269 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/unsupported/test/cxx11_tensor_io.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/unsupported/test/cxx11_tensor_layout_swap.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      942 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/unsupported/test/cxx11_tensor_lvalue.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     6707 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/unsupported/test/cxx11_tensor_map.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      985 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/unsupported/test/cxx11_tensor_math.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1493 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/unsupported/test/cxx11_tensor_mixed_indices.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    15732 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/unsupported/test/cxx11_tensor_morphing.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1829 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/unsupported/test/cxx11_tensor_notification.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2885 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/unsupported/test/cxx11_tensor_of_complex.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2422 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/unsupported/test/cxx11_tensor_of_const_values.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    21449 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/unsupported/test/cxx11_tensor_of_float16_cuda.cu
--rw-r--r--   0 runner    (1001) docker     (123)     3758 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/unsupported/test/cxx11_tensor_of_strings.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2644 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/unsupported/test/cxx11_tensor_padding.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     5491 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/unsupported/test/cxx11_tensor_patch.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/unsupported/test/cxx11_tensor_random.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2354 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/unsupported/test/cxx11_tensor_random_cuda.cu
--rw-r--r--   0 runner    (1001) docker     (123)    14383 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/unsupported/test/cxx11_tensor_reduction.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     5457 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/unsupported/test/cxx11_tensor_reduction_cuda.cu
--rw-r--r--   0 runner    (1001) docker     (123)     4935 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/unsupported/test/cxx11_tensor_reduction_sycl.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     6714 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/unsupported/test/cxx11_tensor_ref.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     5277 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/unsupported/test/cxx11_tensor_reverse.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/unsupported/test/cxx11_tensor_roundings.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2970 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/unsupported/test/cxx11_tensor_scan.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2566 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/unsupported/test/cxx11_tensor_scan_cuda.cu
--rw-r--r--   0 runner    (1001) docker     (123)     6229 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/unsupported/test/cxx11_tensor_shuffling.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     9616 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/unsupported/test/cxx11_tensor_simple.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3016 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/unsupported/test/cxx11_tensor_striding.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1888 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/unsupported/test/cxx11_tensor_sugar.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     5799 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/unsupported/test/cxx11_tensor_sycl.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    59071 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/unsupported/test/cxx11_tensor_symmetry.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    12691 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/unsupported/test/cxx11_tensor_thread_pool.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     5718 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/unsupported/test/cxx11_tensor_uint128.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4599 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/unsupported/test/cxx11_tensor_volume_patch.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/unsupported/test/dgmres.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3810 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/unsupported/test/forward_adolc.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/unsupported/test/gmres.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     9096 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/unsupported/test/kronecker_product.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    55496 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/unsupported/test/levenberg_marquardt.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4409 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/unsupported/test/matrix_exponential.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     7523 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/unsupported/test/matrix_function.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2106 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/unsupported/test/matrix_functions.h
--rw-r--r--   0 runner    (1001) docker     (123)     7150 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/unsupported/test/matrix_power.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/unsupported/test/matrix_square_root.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/unsupported/test/minres.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 14:34:30.661841 stag-1.2.1/stag/eigen-3.3.9/unsupported/test/mpreal/
--rw-r--r--   0 runner    (1001) docker     (123)   118239 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/unsupported/test/mpreal/mpreal.h
--rw-r--r--   0 runner    (1001) docker     (123)     2375 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/unsupported/test/mpreal_support.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    10588 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/unsupported/test/openglsupport.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     7478 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/unsupported/test/polynomialsolver.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3574 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/unsupported/test/polynomialutils.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     5352 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/unsupported/test/sparse_extra.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    16332 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/unsupported/test/special_functions.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     8521 2023-03-22 14:34:03.000000 stag-1.2.1/stag/eigen-3.3.9/unsupported/test/splines.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    22376 2023-03-22 14:34:03.000000 stag-1.2.1/stag/graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     3931 2023-03-22 14:34:03.000000 stag-1.2.1/stag/graphio.py
--rw-r--r--   0 runner    (1001) docker     (123)     8983 2023-03-22 14:34:03.000000 stag-1.2.1/stag/neo4j.py
--rw-r--r--   0 runner    (1001) docker     (123)     6717 2023-03-22 14:34:03.000000 stag-1.2.1/stag/random.py
--rw-r--r--   0 runner    (1001) docker     (123)     6244 2023-03-22 14:34:03.000000 stag-1.2.1/stag/spectrum.py
--rw-r--r--   0 runner    (1001) docker     (123)    26722 2023-03-22 14:34:03.000000 stag-1.2.1/stag/stag_internal.py
--rw-r--r--   0 runner    (1001) docker     (123)   773830 2023-03-22 14:34:03.000000 stag-1.2.1/stag/stag_internal_wrap.cxx
--rw-r--r--   0 runner    (1001) docker     (123)     2606 2023-03-22 14:34:03.000000 stag-1.2.1/stag/stag_internal_wrap.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 14:34:30.661841 stag-1.2.1/stag/stag_lib/
--rw-r--r--   0 runner    (1001) docker     (123)     5442 2023-03-22 14:34:03.000000 stag-1.2.1/stag/stag_lib/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     2788 2023-03-22 14:34:03.000000 stag-1.2.1/stag/stag_lib/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 14:34:30.665841 stag-1.2.1/stag/stag_lib/KMeansRex/
--rw-r--r--   0 runner    (1001) docker     (123)     7033 2023-03-22 14:34:03.000000 stag-1.2.1/stag/stag_lib/KMeansRex/KMeansRexCore.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      642 2023-03-22 14:34:03.000000 stag-1.2.1/stag/stag_lib/KMeansRex/KMeansRexCore.h
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-03-22 14:34:03.000000 stag-1.2.1/stag/stag_lib/KMeansRex/KMeansRexCoreInterface.h
--rw-r--r--   0 runner    (1001) docker     (123)     8041 2023-03-22 14:34:03.000000 stag-1.2.1/stag/stag_lib/KMeansRex/mersenneTwister2002.h
--rw-r--r--   0 runner    (1001) docker     (123)    14143 2023-03-22 14:34:03.000000 stag-1.2.1/stag/stag_lib/cluster.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     8055 2023-03-22 14:34:03.000000 stag-1.2.1/stag/stag_lib/cluster.h
--rw-r--r--   0 runner    (1001) docker     (123)    21726 2023-03-22 14:34:03.000000 stag-1.2.1/stag/stag_lib/graph.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    20437 2023-03-22 14:34:03.000000 stag-1.2.1/stag/stag_lib/graph.h
--rw-r--r--   0 runner    (1001) docker     (123)    23902 2023-03-22 14:34:03.000000 stag-1.2.1/stag/stag_lib/graphio.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4858 2023-03-22 14:34:03.000000 stag-1.2.1/stag/stag_lib/graphio.h
--rw-r--r--   0 runner    (1001) docker     (123)    15499 2023-03-22 14:34:03.000000 stag-1.2.1/stag/stag_lib/random.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     7718 2023-03-22 14:34:03.000000 stag-1.2.1/stag/stag_lib/random.h
--rw-r--r--   0 runner    (1001) docker     (123)     4481 2023-03-22 14:34:03.000000 stag-1.2.1/stag/stag_lib/spectrum.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     7701 2023-03-22 14:34:03.000000 stag-1.2.1/stag/stag_lib/spectrum.h
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-03-22 14:34:03.000000 stag-1.2.1/stag/stag_lib/stag.h
--rw-r--r--   0 runner    (1001) docker     (123)      642 2023-03-22 14:34:03.000000 stag-1.2.1/stag/stag_lib/stagConfig.cmake.in
--rw-r--r--   0 runner    (1001) docker     (123)     5937 2023-03-22 14:34:03.000000 stag-1.2.1/stag/stag_lib/utility.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4111 2023-03-22 14:34:03.000000 stag-1.2.1/stag/stag_lib/utility.h
--rw-r--r--   0 runner    (1001) docker     (123)     2665 2023-03-22 14:34:03.000000 stag-1.2.1/stag/utility.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 14:34:30.497841 stag-1.2.1/stag.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      757 2023-03-22 14:34:30.000000 stag-1.2.1/stag.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    85404 2023-03-22 14:34:30.000000 stag-1.2.1/stag.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-22 14:34:30.000000 stag-1.2.1/stag.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-22 14:34:30.000000 stag-1.2.1/stag.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-03-22 14:34:30.000000 stag-1.2.1/stag.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 14:34:30.665841 stag-1.2.1/test/
--rw-r--r--   0 runner    (1001) docker     (123)     4976 2023-03-22 14:34:03.000000 stag-1.2.1/test/test_clustering.py
--rw-r--r--   0 runner    (1001) docker     (123)    11359 2023-03-22 14:34:03.000000 stag-1.2.1/test/test_graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     4723 2023-03-22 14:34:03.000000 stag-1.2.1/test/test_graphio.py
--rw-r--r--   0 runner    (1001) docker     (123)     2374 2023-03-22 14:34:03.000000 stag-1.2.1/test/test_random.py
--rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-03-22 14:34:03.000000 stag-1.2.1/test/test_spectrum.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 10:47:59.916824 stag-2.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-05-07 10:47:32.000000 stag-2.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-05-07 10:47:32.000000 stag-2.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      757 2024-05-07 10:47:59.916824 stag-2.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1162 2024-05-07 10:47:32.000000 stag-2.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 10:47:59.916824 stag-2.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3051 2024-05-07 10:47:32.000000 stag-2.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 10:47:59.908824 stag-2.0.0/stag/
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-07 10:47:32.000000 stag-2.0.0/stag/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14835 2024-05-07 10:47:32.000000 stag-2.0.0/stag/cluster.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1728 2024-05-07 10:47:32.000000 stag-2.0.0/stag/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24731 2024-05-07 10:47:32.000000 stag-2.0.0/stag/graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3917 2024-05-07 10:47:32.000000 stag-2.0.0/stag/graphio.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10119 2024-05-07 10:47:32.000000 stag-2.0.0/stag/kde.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6501 2024-05-07 10:47:32.000000 stag-2.0.0/stag/lsh.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8983 2024-05-07 10:47:32.000000 stag-2.0.0/stag/neo4j.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6753 2024-05-07 10:47:32.000000 stag-2.0.0/stag/random.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7321 2024-05-07 10:47:32.000000 stag-2.0.0/stag/spectrum.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24949 2024-05-07 10:47:32.000000 stag-2.0.0/stag/stag_internal.py
+-rw-r--r--   0 runner    (1001) docker     (127)   602218 2024-05-07 10:47:32.000000 stag-2.0.0/stag/stag_internal_wrap.cxx
+-rw-r--r--   0 runner    (1001) docker     (127)     2432 2024-05-07 10:47:32.000000 stag-2.0.0/stag/stag_internal_wrap.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 10:47:59.912824 stag-2.0.0/stag/stag_lib/
+-rw-r--r--   0 runner    (1001) docker     (127)     8222 2024-05-07 10:47:32.000000 stag-2.0.0/stag/stag_lib/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3622 2024-05-07 10:47:32.000000 stag-2.0.0/stag/stag_lib/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 10:47:59.912824 stag-2.0.0/stag/stag_lib/KMeansRex/
+-rw-r--r--   0 runner    (1001) docker     (127)     8566 2024-05-07 10:47:32.000000 stag-2.0.0/stag/stag_lib/KMeansRex/KMeansRexCore.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2242 2024-05-07 10:47:32.000000 stag-2.0.0/stag/stag_lib/KMeansRex/KMeansRexCore.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1858 2024-05-07 10:47:32.000000 stag-2.0.0/stag/stag_lib/KMeansRex/KMeansRexCoreInterface.h
+-rw-r--r--   0 runner    (1001) docker     (127)     8041 2024-05-07 10:47:32.000000 stag-2.0.0/stag/stag_lib/KMeansRex/mersenneTwister2002.h
+-rw-r--r--   0 runner    (1001) docker     (127)    35496 2024-05-07 10:47:32.000000 stag-2.0.0/stag/stag_lib/cluster.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    14705 2024-05-07 10:47:32.000000 stag-2.0.0/stag/stag_lib/cluster.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6058 2024-05-07 10:47:32.000000 stag-2.0.0/stag/stag_lib/data.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3581 2024-05-07 10:47:32.000000 stag-2.0.0/stag/stag_lib/data.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1622 2024-05-07 10:47:32.000000 stag-2.0.0/stag/stag_lib/definitions.h
+-rw-r--r--   0 runner    (1001) docker     (127)    31852 2024-05-07 10:47:32.000000 stag-2.0.0/stag/stag_lib/graph.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    23858 2024-05-07 10:47:32.000000 stag-2.0.0/stag/stag_lib/graph.h
+-rw-r--r--   0 runner    (1001) docker     (127)    23897 2024-05-07 10:47:32.000000 stag-2.0.0/stag/stag_lib/graphio.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4858 2024-05-07 10:47:32.000000 stag-2.0.0/stag/stag_lib/graphio.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 10:47:59.916824 stag-2.0.0/stag/stag_lib/indicators/
+-rw-r--r--   0 runner    (1001) docker     (127)   112777 2024-05-07 10:47:32.000000 stag-2.0.0/stag/stag_lib/indicators/indicators.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    26184 2024-05-07 10:47:32.000000 stag-2.0.0/stag/stag_lib/kde.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    13432 2024-05-07 10:47:32.000000 stag-2.0.0/stag/stag_lib/kde.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6638 2024-05-07 10:47:32.000000 stag-2.0.0/stag/stag_lib/lsh.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     8260 2024-05-07 10:47:32.000000 stag-2.0.0/stag/stag_lib/lsh.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 10:47:59.916824 stag-2.0.0/stag/stag_lib/multithreading/
+-rw-r--r--   0 runner    (1001) docker     (127)     9514 2024-05-07 10:47:32.000000 stag-2.0.0/stag/stag_lib/multithreading/ctpl_stl.h
+-rw-r--r--   0 runner    (1001) docker     (127)    15750 2024-05-07 10:47:32.000000 stag-2.0.0/stag/stag_lib/random.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     8022 2024-05-07 10:47:32.000000 stag-2.0.0/stag/stag_lib/random.h
+-rw-r--r--   0 runner    (1001) docker     (127)     7250 2024-05-07 10:47:32.000000 stag-2.0.0/stag/stag_lib/spectrum.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     8147 2024-05-07 10:47:32.000000 stag-2.0.0/stag/stag_lib/spectrum.h
+-rw-r--r--   0 runner    (1001) docker     (127)      387 2024-05-07 10:47:32.000000 stag-2.0.0/stag/stag_lib/stag.h
+-rw-r--r--   0 runner    (1001) docker     (127)      642 2024-05-07 10:47:32.000000 stag-2.0.0/stag/stag_lib/stagConfig.cmake.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5934 2024-05-07 10:47:32.000000 stag-2.0.0/stag/stag_lib/utility.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4196 2024-05-07 10:47:32.000000 stag-2.0.0/stag/stag_lib/utility.h
+-rw-r--r--   0 runner    (1001) docker     (127)    12889 2024-05-07 10:47:32.000000 stag-2.0.0/stag/utility.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 10:47:59.912824 stag-2.0.0/stag.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      757 2024-05-07 10:47:59.000000 stag-2.0.0/stag.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1439 2024-05-07 10:47:59.000000 stag-2.0.0/stag.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 10:47:59.000000 stag-2.0.0/stag.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 10:47:59.000000 stag-2.0.0/stag.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-07 10:47:59.000000 stag-2.0.0/stag.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 10:47:59.916824 stag-2.0.0/test/
+-rw-r--r--   0 runner    (1001) docker     (127)    10092 2024-05-07 10:47:32.000000 stag-2.0.0/test/test_clustering.py
+-rw-r--r--   0 runner    (1001) docker     (127)      451 2024-05-07 10:47:32.000000 stag-2.0.0/test/test_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21190 2024-05-07 10:47:32.000000 stag-2.0.0/test/test_graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5051 2024-05-07 10:47:32.000000 stag-2.0.0/test/test_graphio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5121 2024-05-07 10:47:32.000000 stag-2.0.0/test/test_kde.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4758 2024-05-07 10:47:32.000000 stag-2.0.0/test/test_lsh.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1950 2024-05-07 10:47:32.000000 stag-2.0.0/test/test_performance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2408 2024-05-07 10:47:32.000000 stag-2.0.0/test/test_random.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1537 2024-05-07 10:47:32.000000 stag-2.0.0/test/test_spectrum.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15763 2024-05-07 10:47:32.000000 stag-2.0.0/test/test_utility.py
```

### Comparing `stag-1.2.1/LICENSE` & `stag-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `stag-1.2.1/PKG-INFO` & `stag-2.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stag
-Version: 1.2.1
+Version: 2.0.0
 Summary: STAG: Spectral Toolkit of Algorithms for Graphs
 Home-page: https://staglibrary.io
 Author: Peter Macgregor
 Author-email: <macgregor.pr@gmail.com>
 License: UNKNOWN
 Keywords: python,spectral,graph,algorithms,clustering,cheeger
 Platform: UNKNOWN
```

### Comparing `stag-1.2.1/README.md` & `stag-2.0.0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # STAGPy - Spectral Toolkit of Algorithms for Graphs
 
 [![Test](https://github.com/staglibrary/stagpy/actions/workflows/github-actions-test.yml/badge.svg?branch=main)](https://github.com/staglibrary/stagpy/actions/workflows/github-actions-test.yml)
 [![Build](https://github.com/staglibrary/stagpy/actions/workflows/github-actions-release.yml/badge.svg)](https://github.com/staglibrary/stagpy/actions/workflows/github-actions-release.yml)
 [![Docs](https://github.com/staglibrary/stagpy/actions/workflows/github-actions-docs.yml/badge.svg)](https://github.com/staglibrary/stagpy/actions/workflows/github-actions-docs.yml)
+[![Performance](https://github.com/staglibrary/stagpy/actions/workflows/github-actions-benchmark.yml/badge.svg)](https://staglibrary.github.io/stagpy/dev/bench/)
 
 STAG is a library providing efficient spectral algorithms for the analysis of massive graphs. STAGPy is a python wrapper around the underlying C++ library which provides convenient methods for learning on graphs in python.
 
 ## Project Status
 
 The project is under active development; more information and documentation can be found here, and [our website](http://staglibrary.io).
```

### Comparing `stag-1.2.1/setup.py` & `stag-2.0.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import platform
 
 from setuptools import setup, find_packages
 from distutils.core import setup, Extension
 
 import numpy
 
-VERSION = '1.2.1'
+VERSION = '2.0.0'
 DESCRIPTION = 'STAG: Spectral Toolkit of Algorithms for Graphs'
 LONG_DESCRIPTION =\
     "This library provides several methods and algorithms relating to spectral graph theory in python."
 URL = "https://staglibrary.io"
 
 # Depending on the build platform, the required compiler flags are slightly
 # different.
@@ -32,17 +32,20 @@
                          sources=["stag/stag_internal_wrap.cxx",
                                   "stag/stag_lib/graph.cpp",
                                   "stag/stag_lib/random.cpp",
                                   "stag/stag_lib/graphio.cpp",
                                   "stag/stag_lib/cluster.cpp",
                                   "stag/stag_lib/utility.cpp",
                                   "stag/stag_lib/spectrum.cpp",
+                                  "stag/stag_lib/data.cpp",
+                                  "stag/stag_lib/lsh.cpp",
+                                  "stag/stag_lib/kde.cpp",
                                   "stag/stag_lib/KMeansRex/KMeansRexCore.cpp"
                                   ],
-                         include_dirs=["stag/eigen-3.3.9",
+                         include_dirs=["stag/eigen-3.4.0",
                                        "stag/spectra-1.0.1",
                                        "stag/stag_lib",
                                        "stag/stag_lib/KMeansRex",
                                        numpy_path
                                        ],
                          extra_compile_args=compile_args)]
```

### Comparing `stag-1.2.1/stag/eigen-3.3.9/COPYING.BSD` & `stag-2.0.0/stag/stag_lib/KMeansRex/KMeansRexCoreInterface.h`

 * *Files 26% similar despite different names*

```diff
@@ -1,26 +1,39 @@
 /*
- Copyright (c) 2011, Intel Corporation. All rights reserved.
+This file is released under the GPL license, with the following additional
+requirements.
 
- Redistribution and use in source and binary forms, with or without modification,
- are permitted provided that the following conditions are met:
+Copyright (c) 2013-2015, Michael C. Hughes
+All rights reserved.
 
- * Redistributions of source code must retain the above copyright notice, this
-   list of conditions and the following disclaimer.
- * Redistributions in binary form must reproduce the above copyright notice,
+Redistribution and use in source and binary forms, with or without modification,
+are permitted provided that the following conditions are met:
+
+1. Redistributions of source code must retain the above copyright notice,
+   this list of conditions and the following disclaimer.
+
+2. Redistributions in binary form must reproduce the above copyright notice,
    this list of conditions and the following disclaimer in the documentation
    and/or other materials provided with the distribution.
- * Neither the name of Intel Corporation nor the names of its contributors may
-   be used to endorse or promote products derived from this software without
+
+3. Neither the name of the copyright holder nor the names of its contributors
+   may be used to endorse or promote products derived from this software without
    specific prior written permission.
 
- THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS" AND
- ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED
- WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
- DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT OWNER OR CONTRIBUTORS BE LIABLE FOR
- ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES
- (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES;
- LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON
- ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT
- (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
- SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
-*/
+THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS" AND
+ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED
+WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE DISCLAIMED.
+IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE FOR ANY DIRECT,
+INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING,
+BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE,
+DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF
+LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE
+OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF
+ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+ */
+#pragma once
+
+extern "C" {
+	void RunKMeans(double *X_IN,  int N,  int D, int K, int Niter, \
+	           int seed, char* initname, double *Mu_OUT, double *Z_OUT);
+	void SampleRowsPlusPlus(double *X_IN,  int N,  int D, int K, int seed, double *Mu_OUT);
+}
```

### Comparing `stag-1.2.1/stag/eigen-3.3.9/unsupported/Eigen/CXX11/src/ThreadPool/NonBlockingThreadPool.h` & `stag-2.0.0/stag/stag_lib/multithreading/ctpl_stl.h`

 * *Files 24% similar despite different names*

```diff
@@ -1,274 +1,248 @@
-// This file is part of Eigen, a lightweight C++ template library
-// for linear algebra.
-//
-// Copyright (C) 2016 Dmitry Vyukov <dvyukov@google.com>
-//
-// This Source Code Form is subject to the terms of the Mozilla
-// Public License v. 2.0. If a copy of the MPL was not distributed
-// with this file, You can obtain one at http://mozilla.org/MPL/2.0/.
-
-#ifndef EIGEN_CXX11_THREADPOOL_NONBLOCKING_THREAD_POOL_H
-#define EIGEN_CXX11_THREADPOOL_NONBLOCKING_THREAD_POOL_H
-
-
-namespace Eigen {
-
-template <typename Environment>
-class NonBlockingThreadPoolTempl : public Eigen::ThreadPoolInterface {
- public:
-  typedef typename Environment::Task Task;
-  typedef RunQueue<Task, 1024> Queue;
-
-  NonBlockingThreadPoolTempl(int num_threads, Environment env = Environment())
-      : env_(env),
-        threads_(num_threads),
-        queues_(num_threads),
-        coprimes_(num_threads),
-        waiters_(num_threads),
-        blocked_(0),
-        spinning_(0),
-        done_(false),
-        ec_(waiters_) {
-    waiters_.resize(num_threads);
-
-    // Calculate coprimes of num_threads.
-    // Coprimes are used for a random walk over all threads in Steal
-    // and NonEmptyQueueIndex. Iteration is based on the fact that if we take
-    // a walk starting thread index t and calculate num_threads - 1 subsequent
-    // indices as (t + coprime) % num_threads, we will cover all threads without
-    // repetitions (effectively getting a presudo-random permutation of thread
-    // indices).
-    for (int i = 1; i <= num_threads; i++) {
-      unsigned a = i;
-      unsigned b = num_threads;
-      // If GCD(a, b) == 1, then a and b are coprimes.
-      while (b != 0) {
-        unsigned tmp = a;
-        a = b;
-        b = tmp % b;
-      }
-      if (a == 1) {
-        coprimes_.push_back(i);
-      }
-    }
-    for (int i = 0; i < num_threads; i++) {
-      queues_.push_back(new Queue());
-    }
-    for (int i = 0; i < num_threads; i++) {
-      threads_.push_back(env_.CreateThread([this, i]() { WorkerLoop(i); }));
-    }
-  }
+/*
+  Copyright (C) 2014 by Vitaliy Vitsentiy
 
-  ~NonBlockingThreadPoolTempl() {
-    done_ = true;
-    // Now if all threads block without work, they will start exiting.
-    // But note that threads can continue to work arbitrary long,
-    // block, submit new work, unblock and otherwise live full life.
-    ec_.Notify(true);
-
-    // Join threads explicitly to avoid destruction order issues.
-    for (size_t i = 0; i < threads_.size(); i++) delete threads_[i];
-    for (size_t i = 0; i < threads_.size(); i++) delete queues_[i];
-  }
-
-  void Schedule(std::function<void()> fn) {
-    Task t = env_.CreateTask(std::move(fn));
-    PerThread* pt = GetPerThread();
-    if (pt->pool == this) {
-      // Worker thread of this pool, push onto the thread's queue.
-      Queue* q = queues_[pt->thread_id];
-      t = q->PushFront(std::move(t));
-    } else {
-      // A free-standing thread (or worker of another pool), push onto a random
-      // queue.
-      Queue* q = queues_[Rand(&pt->rand) % queues_.size()];
-      t = q->PushBack(std::move(t));
-    }
-    // Note: below we touch this after making w available to worker threads.
-    // Strictly speaking, this can lead to a racy-use-after-free. Consider that
-    // Schedule is called from a thread that is neither main thread nor a worker
-    // thread of this pool. Then, execution of w directly or indirectly
-    // completes overall computations, which in turn leads to destruction of
-    // this. We expect that such scenario is prevented by program, that is,
-    // this is kept alive while any threads can potentially be in Schedule.
-    if (!t.f)
-      ec_.Notify(false);
-    else
-      env_.ExecuteTask(t);  // Push failed, execute directly.
-  }
-
-  int NumThreads() const final {
-    return static_cast<int>(threads_.size());
-  }
-
-  int CurrentThreadId() const final {
-    const PerThread* pt =
-        const_cast<NonBlockingThreadPoolTempl*>(this)->GetPerThread();
-    if (pt->pool == this) {
-      return pt->thread_id;
-    } else {
-      return -1;
+  This file is released under the GPL license.
+
+  See https://github.com/vit-vit/CTPL.
+*/
+
+
+#ifndef __ctpl_stl_thread_pool_H__
+#define __ctpl_stl_thread_pool_H__
+
+#include <functional>
+#include <thread>
+#include <atomic>
+#include <vector>
+#include <memory>
+#include <exception>
+#include <future>
+#include <mutex>
+#include <queue>
+
+
+
+// thread pool to run user's functors with signature
+//      ret func(int id, other_params)
+// where id is the index of the thread that runs the functor
+// ret is some return type
+
+/*
+ * \cond
+ */
+
+namespace ctpl {
+
+    namespace detail {
+        template <typename T>
+        class Queue {
+        public:
+            bool push(T const & value) {
+                std::unique_lock<std::mutex> lock(this->mutex);
+                this->q.push(value);
+                return true;
+            }
+            // deletes the retrieved element, do not use for non integral types
+            bool pop(T & v) {
+                std::unique_lock<std::mutex> lock(this->mutex);
+                if (this->q.empty())
+                    return false;
+                v = this->q.front();
+                this->q.pop();
+                return true;
+            }
+            bool empty() {
+                std::unique_lock<std::mutex> lock(this->mutex);
+                return this->q.empty();
+            }
+        private:
+            std::queue<T> q;
+            std::mutex mutex;
+        };
     }
-  }
 
- private:
-  typedef typename Environment::EnvThread Thread;
+    class thread_pool {
+
+    public:
+
+        thread_pool() { this->init(); }
+        thread_pool(int nThreads) { this->init(); this->resize(nThreads); }
+
+        // the destructor waits for all the functions in the queue to be finished
+        ~thread_pool() {
+            this->stop(true);
+        }
 
-  struct PerThread {
-    constexpr PerThread() : pool(NULL), rand(0), thread_id(-1) { }
-    NonBlockingThreadPoolTempl* pool;  // Parent pool, or null for normal threads.
-    uint64_t rand;  // Random generator state.
-    int thread_id;  // Worker thread index in pool.
-  };
-
-  Environment env_;
-  MaxSizeVector<Thread*> threads_;
-  MaxSizeVector<Queue*> queues_;
-  MaxSizeVector<unsigned> coprimes_;
-  MaxSizeVector<EventCount::Waiter> waiters_;
-  std::atomic<unsigned> blocked_;
-  std::atomic<bool> spinning_;
-  std::atomic<bool> done_;
-  EventCount ec_;
-
-  // Main worker thread loop.
-  void WorkerLoop(int thread_id) {
-    PerThread* pt = GetPerThread();
-    pt->pool = this;
-    pt->rand = std::hash<std::thread::id>()(std::this_thread::get_id());
-    pt->thread_id = thread_id;
-    Queue* q = queues_[thread_id];
-    EventCount::Waiter* waiter = &waiters_[thread_id];
-    for (;;) {
-      Task t = q->PopFront();
-      if (!t.f) {
-        t = Steal();
-        if (!t.f) {
-          // Leave one thread spinning. This reduces latency.
-          // TODO(dvyukov): 1000 iterations is based on fair dice roll, tune it.
-          // Also, the time it takes to attempt to steal work 1000 times depends
-          // on the size of the thread pool. However the speed at which the user
-          // of the thread pool submit tasks is independent of the size of the
-          // pool. Consider a time based limit instead.
-          if (!spinning_ && !spinning_.exchange(true)) {
-            for (int i = 0; i < 1000 && !t.f; i++) {
-              t = Steal();
+        // get the number of running threads in the pool
+        int size() { return static_cast<int>(this->threads.size()); }
+
+        // number of idle threads
+        int n_idle() { return this->nWaiting; }
+        std::thread & get_thread(int i) { return *this->threads[i]; }
+
+        // change the number of threads in the pool
+        // should be called from one thread, otherwise be careful to not interleave, also with this->stop()
+        // nThreads must be >= 0
+        void resize(int nThreads) {
+            if (!this->isStop && !this->isDone) {
+                int oldNThreads = static_cast<int>(this->threads.size());
+                if (oldNThreads <= nThreads) {  // if the number of threads is increased
+                    this->threads.resize(nThreads);
+                    this->flags.resize(nThreads);
+
+                    for (int i = oldNThreads; i < nThreads; ++i) {
+                        this->flags[i] = std::make_shared<std::atomic<bool>>(false);
+                        this->set_thread(i);
+                    }
+                }
+                else {  // the number of threads is decreased
+                    for (int i = oldNThreads - 1; i >= nThreads; --i) {
+                        *this->flags[i] = true;  // this thread will finish
+                        this->threads[i]->detach();
+                    }
+                    {
+                        // stop the detached threads that were waiting
+                        std::unique_lock<std::mutex> lock(this->mutex);
+                        this->cv.notify_all();
+                    }
+                    this->threads.resize(nThreads);  // safe to delete because the threads are detached
+                    this->flags.resize(nThreads);  // safe to delete because the threads have copies of shared_ptr of the flags, not originals
+                }
+            }
+        }
+
+        // empty the queue
+        void clear_queue() {
+            std::function<void(int id)> * _f;
+            while (this->q.pop(_f))
+                delete _f; // empty the queue
+        }
+
+        // pops a functional wrapper to the original function
+        std::function<void(int)> pop() {
+            std::function<void(int id)> * _f = nullptr;
+            this->q.pop(_f);
+            std::unique_ptr<std::function<void(int id)>> func(_f); // at return, delete the function even if an exception occurred
+            std::function<void(int)> f;
+            if (_f)
+                f = *_f;
+            return f;
+        }
+
+        // wait for all computing threads to finish and stop all threads
+        // may be called asynchronously to not pause the calling thread while waiting
+        // if isWait == true, all the functions in the queue are run, otherwise the queue is cleared without running the functions
+        void stop(bool isWait = false) {
+            if (!isWait) {
+                if (this->isStop)
+                    return;
+                this->isStop = true;
+                for (int i = 0, n = this->size(); i < n; ++i) {
+                    *this->flags[i] = true;  // command the threads to stop
+                }
+                this->clear_queue();  // empty the queue
+            }
+            else {
+                if (this->isDone || this->isStop)
+                    return;
+                this->isDone = true;  // give the waiting threads a command to finish
+            }
+            {
+                std::unique_lock<std::mutex> lock(this->mutex);
+                this->cv.notify_all();  // stop all waiting threads
             }
-            spinning_ = false;
-          }
-          if (!t.f) {
-            if (!WaitForWork(waiter, &t)) {
-              return;
+            for (int i = 0; i < static_cast<int>(this->threads.size()); ++i) {  // wait for the computing threads to finish
+                    if (this->threads[i]->joinable())
+                        this->threads[i]->join();
             }
-          }
+            // if there were no threads in the pool but some functors in the queue, the functors are not deleted by the threads
+            // therefore delete them here
+            this->clear_queue();
+            this->threads.clear();
+            this->flags.clear();
         }
-      }
-      if (t.f) {
-        env_.ExecuteTask(t);
-      }
-    }
-  }
 
-  // Steal tries to steal work from other worker threads in best-effort manner.
-  Task Steal() {
-    PerThread* pt = GetPerThread();
-    const size_t size = queues_.size();
-    unsigned r = Rand(&pt->rand);
-    unsigned inc = coprimes_[r % coprimes_.size()];
-    unsigned victim = r % size;
-    for (unsigned i = 0; i < size; i++) {
-      Task t = queues_[victim]->PopBack();
-      if (t.f) {
-        return t;
-      }
-      victim += inc;
-      if (victim >= size) {
-        victim -= size;
-      }
-    }
-    return Task();
-  }
+        template<typename F, typename... Rest>
+        auto push(F && f, Rest&&... rest) ->std::future<decltype(f(0, rest...))> {
+            auto pck = std::make_shared<std::packaged_task<decltype(f(0, rest...))(int)>>(
+                std::bind(std::forward<F>(f), std::placeholders::_1, std::forward<Rest>(rest)...)
+                );
+            auto _f = new std::function<void(int id)>([pck](int id) {
+                (*pck)(id);
+            });
+            this->q.push(_f);
+            std::unique_lock<std::mutex> lock(this->mutex);
+            this->cv.notify_one();
+            return pck->get_future();
+        }
+
+        // run the user's function that excepts argument int - id of the running thread. returned value is templatized
+        // operator returns std::future, where the user can get the result and rethrow the catched exceptins
+        template<typename F>
+        auto push(F && f) ->std::future<decltype(f(0))> {
+            auto pck = std::make_shared<std::packaged_task<decltype(f(0))(int)>>(std::forward<F>(f));
+            auto _f = new std::function<void(int id)>([pck](int id) {
+                (*pck)(id);
+            });
+            this->q.push(_f);
+            std::unique_lock<std::mutex> lock(this->mutex);
+            this->cv.notify_one();
+            return pck->get_future();
+        }
 
-  // WaitForWork blocks until new work is available (returns true), or if it is
-  // time to exit (returns false). Can optionally return a task to execute in t
-  // (in such case t.f != nullptr on return).
-  bool WaitForWork(EventCount::Waiter* waiter, Task* t) {
-    eigen_assert(!t->f);
-    // We already did best-effort emptiness check in Steal, so prepare for
-    // blocking.
-    ec_.Prewait(waiter);
-    // Now do a reliable emptiness check.
-    int victim = NonEmptyQueueIndex();
-    if (victim != -1) {
-      ec_.CancelWait(waiter);
-      *t = queues_[victim]->PopBack();
-      return true;
-    }
-    // Number of blocked threads is used as termination condition.
-    // If we are shutting down and all worker threads blocked without work,
-    // that's we are done.
-    blocked_++;
-    if (done_ && blocked_ == threads_.size()) {
-      ec_.CancelWait(waiter);
-      // Almost done, but need to re-check queues.
-      // Consider that all queues are empty and all worker threads are preempted
-      // right after incrementing blocked_ above. Now a free-standing thread
-      // submits work and calls destructor (which sets done_). If we don't
-      // re-check queues, we will exit leaving the work unexecuted.
-      if (NonEmptyQueueIndex() != -1) {
-        // Note: we must not pop from queues before we decrement blocked_,
-        // otherwise the following scenario is possible. Consider that instead
-        // of checking for emptiness we popped the only element from queues.
-        // Now other worker threads can start exiting, which is bad if the
-        // work item submits other work. So we just check emptiness here,
-        // which ensures that all worker threads exit at the same time.
-        blocked_--;
-        return true;
-      }
-      // Reached stable termination state.
-      ec_.Notify(true);
-      return false;
-    }
-    ec_.CommitWait(waiter);
-    blocked_--;
-    return true;
-  }
-
-  int NonEmptyQueueIndex() {
-    PerThread* pt = GetPerThread();
-    const size_t size = queues_.size();
-    unsigned r = Rand(&pt->rand);
-    unsigned inc = coprimes_[r % coprimes_.size()];
-    unsigned victim = r % size;
-    for (unsigned i = 0; i < size; i++) {
-      if (!queues_[victim]->Empty()) {
-        return victim;
-      }
-      victim += inc;
-      if (victim >= size) {
-        victim -= size;
-      }
-    }
-    return -1;
-  }
 
-  static EIGEN_STRONG_INLINE PerThread* GetPerThread() {
-    EIGEN_THREAD_LOCAL PerThread per_thread_;
-    PerThread* pt = &per_thread_;
-    return pt;
-  }
-
-  static EIGEN_STRONG_INLINE unsigned Rand(uint64_t* state) {
-    uint64_t current = *state;
-    // Update the internal state
-    *state = current * 6364136223846793005ULL + 0xda3e39cb94b95bdbULL;
-    // Generate the random output (using the PCG-XSH-RS scheme)
-    return static_cast<unsigned>((current ^ (current >> 22)) >> (22 + (current >> 61)));
-  }
-};
+    private:
+
+        // deleted
+        thread_pool(const thread_pool &);// = delete;
+        thread_pool(thread_pool &&);// = delete;
+        thread_pool & operator=(const thread_pool &);// = delete;
+        thread_pool & operator=(thread_pool &&);// = delete;
+
+        void set_thread(int i) {
+            std::shared_ptr<std::atomic<bool>> flag(this->flags[i]); // a copy of the shared ptr to the flag
+            auto f = [this, i, flag/* a copy of the shared ptr to the flag */]() {
+                std::atomic<bool> & _flag = *flag;
+                std::function<void(int id)> * _f;
+                bool isPop = this->q.pop(_f);
+                while (true) {
+                    while (isPop) {  // if there is anything in the queue
+                        std::unique_ptr<std::function<void(int id)>> func(_f); // at return, delete the function even if an exception occurred
+                        (*_f)(i);
+                        if (_flag)
+                            return;  // the thread is wanted to stop, return even if the queue is not empty yet
+                        else
+                            isPop = this->q.pop(_f);
+                    }
+                    // the queue is empty here, wait for the next command
+                    std::unique_lock<std::mutex> lock(this->mutex);
+                    ++this->nWaiting;
+                    this->cv.wait(lock, [this, &_f, &isPop, &_flag](){ isPop = this->q.pop(_f); return isPop || this->isDone || _flag; });
+                    --this->nWaiting;
+                    if (!isPop)
+                        return;  // if the queue is empty and this->isDone == true or *flag then return
+                }
+            };
+            this->threads[i].reset(new std::thread(f)); // compiler may not support std::make_unique()
+        }
 
-typedef NonBlockingThreadPoolTempl<StlThreadEnvironment> NonBlockingThreadPool;
+        void init() { this->nWaiting = 0; this->isStop = false; this->isDone = false; }
 
-}  // namespace Eigen
+        std::vector<std::unique_ptr<std::thread>> threads;
+        std::vector<std::shared_ptr<std::atomic<bool>>> flags;
+        detail::Queue<std::function<void(int id)> *> q;
+        std::atomic<bool> isDone;
+        std::atomic<bool> isStop;
+        std::atomic<int> nWaiting;  // how many threads are waiting
+
+        std::mutex mutex;
+        std::condition_variable cv;
+    };
+
+}
+
+/*
+ * \endcond
+ */
 
-#endif  // EIGEN_CXX11_THREADPOOL_NONBLOCKING_THREAD_POOL_H
+#endif // __ctpl_stl_thread_pool_H__
```

### Comparing `stag-1.2.1/stag/graph.py` & `stag-2.0.0/stag/graph.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 """
 Graph object definitions and standard constructors.
 """
 import networkx
 from abc import ABC, abstractmethod
-from typing import List
-import inspect
+from typing import List, Union
 
 import scipy.sparse
+import numpy as np
 
+import stag.utility
 from . import stag_internal
 from . import utility
 
 
 class Edge(object):
     """
     An object representing a weighted edge in a graph.
@@ -30,17 +31,17 @@
         ## The weight of the edge
         self.weight = weight
 
         ##
         # \cond
         ##
         self.internal_edge = stag_internal.edge()
-        self.internal_edge.v1 = v1
-        self.internal_edge.v2 = v2
-        self.internal_edge.weight = weight
+        self.internal_edge.__setattr__("v1", v1)
+        self.internal_edge.__setattr__("v2", v2)
+        self.internal_edge.__setattr__("weight", weight)
         ##
         # \endcond
         ##
 
     ##
     # \cond
     ##
@@ -121,50 +122,52 @@
         @param v the ID of some vertex in the graph
         @return a list of stag.graph.Edge objects containing the neighbourhood
                 of v
         """
         pass
 
     @abstractmethod
-    def neighbors_unweighted(self, v: int) -> List[int]:
+    def neighbors_unweighted(self, v: int) -> np.ndarray:
         """
         Given a vertex v, return a list of neighbors of v.
 
         The weights of edges to the neighbors are not returned by this method.
 
         @param v the ID of some vertex in the graph
-        @return a list of vertex IDs giving the neighbours of v
+        @return an array of vertex IDs giving the neighbours of v
         """
         pass
 
-    def degrees(self, vertices: List[int]) -> List[float]:
+    @abstractmethod
+    def degrees(self, vertices: np.ndarray) -> np.ndarray:
         """
         Given a list of vertices, return a list of their weighted degrees.
 
         When developing implementations of the stag.graph.LocalGraph class,
         providing an efficient method of returning a list of degrees will
         improve the performance of local clustering algorithms.
 
         @param vertices a list of IDs representing the vertices to be queried
-        @return a list of degrees
+        @return an array of degrees
         """
-        return [self.degree(v) for v in vertices]
+        pass
 
-    def degrees_unweighted(self, vertices: List[int]) -> List[int]:
+    @abstractmethod
+    def degrees_unweighted(self, vertices: np.ndarray) -> np.ndarray:
         """
         Given a list of vertices, return a list of their unweighted degrees.
 
         When developing implementations of the stag.graph.LocalGraph class,
         providing an efficient method of returning a list of degrees will
         improve the performance of local clustering algorithms.
 
         @param vertices a list of IDs representing the vertices to be queried
-        @return a list of unweighted degrees
+        @return an array of unweighted degrees
         """
-        return [self.degree_unweighted(v) for v in vertices]
+        pass
 
     @abstractmethod
     def vertex_exists(self, v: int) -> bool:
         r"""
         Given a vertex ID, returns true or false to indicate whether the vertex exists
         in the graph.
 
@@ -206,15 +209,15 @@
 
 ##
 # \endcond
 ##
 
 
 class AdjacencyListLocalGraph(LocalGraph):
-    """
+    r"""
     \brief A local graph backed by an adjacency list file on disk.
 
     The graph is loaded into memory in a local way only. That is, an adjacency
     list data structure is constructed in memory as node neighbours are queried.
     If a node is not found in the cached adjacency list, then the neighbours of
     the node are queried from the adjacency list on disk. This allows for local
     algorithms to be executed on very large graphs stored on disk without
@@ -263,197 +266,193 @@
 
     def degree_unweighted(self, v: int) -> int:
         return self.internal_graph.degree_unweighted(v)
 
     def neighbors(self, v: int) -> List[Edge]:
         return self.internal_graph.neighbors(v)
 
-    def neighbors_unweighted(self, v: int) -> List[int]:
+    def neighbors_unweighted(self, v: int) -> np.ndarray:
         return self.internal_graph.neighbors_unweighted(v)
 
     def vertex_exists(self, v: int) -> bool:
         return self.internal_graph.vertex_exists(v)
 
+    @utility.convert_ndarrays
+    def degrees(self, vertices: np.ndarray) -> np.ndarray:
+        return self.internal_graph.degrees(vertices)
+
+    @utility.convert_ndarrays
+    def degrees_unweighted(self, vertices: np.ndarray) -> np.ndarray:
+        return self.internal_graph.degrees_unweighted(vertices)
 
 
 class Graph(LocalGraph):
     """
     \brief The core object used to represent graphs for use with the library.
 
     Graphs are always constructed from sparse matrices, and this is the internal
     representation used as well.
     Vertices of the graph are always referred to by their unique integer index.
     This index corresponds to the position of the vertex in the stored adjacency
     matrix of the graph.
+
+    This class supports graphs with positive edge weights. Self-loops are
+    permitted.
     """
 
-    def __init__(self, adj_mat: scipy.sparse.spmatrix,
-                 internal_graph: stag_internal.Graph = None):
+    def __init__(self, mat: Union[scipy.sparse.spmatrix, stag.utility.SprsMat]):
         r"""
-        Initialise the graph with an adjacency matrix.
+        Initialise the graph with a sparse matrix.
+
+        The provided matrix should correspond either to the adjacency matrix or
+        Laplacian matrix of the graph. STAG will automatically detect whether
+        the provided matrix is an adjacency matrix or a Laplacian matrix.
         
         For example:
 
         \code{python}
         >>> import stag.graph
-        >>> import scipy.sparse
+        >>> import stag.utility
         >>>
-        >>> adj_mat = scipy.sparse.csc_matrix([[0, 1, 1, 1],
-        ...                                    [1, 0, 1, 1],
-        ...                                    [1, 1, 0, 1],
-        ...                                    [1, 1, 1, 0]])
+        >>> adj_mat = stag.utility.SprsMat([[0, 1, 1, 1],
+        ...                                 [1, 0, 1, 1],
+        ...                                 [1, 1, 0, 1],
+        ...                                 [1, 1, 1, 0]])
         >>> g = stag.graph.Graph(adj_mat)
         \endcode
 
-        @param adj_mat A sparse scipy matrix, such as ``scipy.sparse.csc_matrix``.
-        @param internal_graph (optional) specify a STAG C++ graph object to
-                              initialise with. Use this only if you understand
-                              the internal workings of the STAG library.
+        @param mat A sparse scipy matrix or a stag.utility.SprsMat object
         """
         # Call the LocalGraph initialisation method - it is important that this
         # is called first. This is because we override the internal_graph
         # object in the current constructor.
         super().__init__()
 
         ##
         # \cond
         # Do not document the internal implementation of the graph object
         ##
 
         # This class is essentially a thin wrapper around the stag_internal library, written in C++.
-        if internal_graph is None:
-            # Initialise the internal graph object with the provided adjacency matrix.
-            adj_mat_csr = adj_mat.tocsr()
-            outer_starts = stag_internal.vectorl(adj_mat_csr.indptr.tolist())
-            inner_indices = stag_internal.vectorl(adj_mat_csr.indices.tolist())
-            values = stag_internal.vectord(adj_mat_csr.data.tolist())
-            self.internal_graph: stag_internal.Graph = stag_internal.Graph(outer_starts, inner_indices, values)
+        if isinstance(mat, stag_internal.Graph):
+            # The initializer was called with an internal graph object.
+            self.internal_graph: stag_internal.Graph = mat
         else:
-            # The initialiser was called with an internal graph object.
-            self.internal_graph: stag_internal.Graph = internal_graph
+            # Initialise the internal graph object with the provided matrix.
+            if type(mat) is not stag.utility.SprsMat:
+                mat = stag.utility.SprsMat(mat)
+            self.internal_graph: stag_internal.Graph = stag_internal.Graph(mat.internal_sprsmat)
 
         ##
         # \endcond
         ##
 
-    @utility.return_sparse_matrix
-    def adjacency(self) -> scipy.sparse.csc_matrix:
+    def adjacency(self) -> stag.utility.SprsMat:
         """
         Return the sparse adjacency matrix of the graph.
 
-        @return a ``scipy.sparse.csc_matrix`` representing the graph adjacency matrix
+        @return a ``stag.utility.SprsMat`` representing the graph adjacency matrix
         """
-        return self.internal_graph.adjacency()
+        adj = utility.SprsMat(self.internal_graph.adjacency())
+        adj.__parent = self
+        return adj
 
-    @utility.return_sparse_matrix
-    def laplacian(self) -> scipy.sparse.csc_matrix:
+    def laplacian(self) -> stag.utility.SprsMat:
         """
         Construct the Laplacian matrix of the graph.
 
         The Laplacian matrix is defined by
 
         \f[
             L = D - A
         \f]
 
         where \f$D\f$ is the diagonal matrix of vertex degrees
         and \f$A\f$ is the adjacency matrix of the graph.
 
-        @return a ``scipy.sparse.csc_matrix`` representing the graph Laplacian
-        """
-        return self.internal_graph.laplacian()
-
-    @utility.return_sparse_matrix
-    def normalised_laplacian(self) -> scipy.sparse.csc_matrix:
-        r"""
-        Construct the normalised Laplacian matrix of the graph.
-
-        The normalised Laplacian matrix is defined by
-
-        \f[
-            \mathcal{L} = D^{-1/2} L D^{-1/2}
-        \f]
-
-        where \f$D\f$ is the diagonal matrix of vertex degrees and \f$L\f$
-        is the Laplacian matrix of the graph.
-
-        @return a ``scipy.sparse.csc_matrix`` representing the normalised Laplacian
+        @return a ``stag.utility.SprsMat`` representing the graph Laplacian
         """
-        return self.internal_graph.normalised_laplacian()
+        lap = utility.SprsMat(self.internal_graph.laplacian())
+        lap.__parent = self
+        return lap
 
-    @utility.return_sparse_matrix
-    def normalised_laplacian(self) -> scipy.sparse.csc_matrix:
+    def normalised_laplacian(self) -> stag.utility.SprsMat:
         r"""
         Construct the normalised Laplacian matrix of the graph.
 
         The normalised Laplacian matrix is defined by
 
         \f[
             \mathcal{L} = D^{-1/2} L D^{-1/2}
         \f]
 
         where \f$D\f$ is the diagonal matrix of vertex degrees and \f$L\f$
         is the Laplacian matrix of the graph.
 
-        @return a ``scipy.sparse.csc_matrix`` representing the normalised Laplacian
+        @return a ``stag.utility.SprsMat`` representing the normalised Laplacian
         """
-        return self.internal_graph.normalised_laplacian()
+        lap = utility.SprsMat(self.internal_graph.normalised_laplacian())
+        lap.__parent = self
+        return lap
 
-    @utility.return_sparse_matrix
-    def signless_laplacian(self) -> scipy.sparse.csc_matrix:
+    def signless_laplacian(self) -> stag.utility.SprsMat:
         """
         Construct the signless Laplacian matrix of the graph.
 
         The signless Laplacian matrix is defined by
 
         \f[
             J = D + A
         \f]
 
         where \f$D\f$ is the diagonal matrix of vertex degrees
         and \f$A\f$ is the adjacency matrix of the graph.
 
-        @return a ``scipy.sparse.csc_matrix`` representing the signless graph Laplacian
+        @return a ``stag.utility.SprsMat`` representing the signless graph Laplacian
         """
-        return self.internal_graph.signless_laplacian()
+        signless_lap = utility.SprsMat(self.internal_graph.signless_laplacian())
+        signless_lap.__parent = self
+        return signless_lap
 
-    @utility.return_sparse_matrix
-    def normalised_signless_laplacian(self) -> scipy.sparse.csc_matrix:
+    def normalised_signless_laplacian(self) -> stag.utility.SprsMat:
         r"""
         Construct the normalised signless Laplacian matrix of the graph.
 
         The normalised signless Laplacian matrix is defined by
 
         \f[
             \mathcal{J} = D^{-1/2} J D^{-1/2}
         \f]
 
         where \f$D\f$ is the diagonal matrix of vertex degrees and \f$J\f$
         is the signless Laplacian matrix of the graph.
 
-        @return a ``scipy.sparse.csc_matrix`` representing the normalised signless Laplacian
+        @return a ``stag.utility.SprsMat`` representing the normalised signless Laplacian
         """
-        return self.internal_graph.normalised_signless_laplacian()
+        signless_lap = utility.SprsMat(
+            self.internal_graph.normalised_signless_laplacian())
+        signless_lap.__parent = self
+        return signless_lap
 
-    @utility.return_sparse_matrix
-    def degree_matrix(self) -> scipy.sparse.csc_matrix:
+    def degree_matrix(self) -> stag.utility.SprsMat:
         r"""
         The degree matrix of the graph.
 
         The degree matrix \f$D \in \mathbb{R}^{n \\times n}\f$
         is a diagonal matrix such that \f$D(i, i) = \mathrm{deg}(i)\f$
         where \f$\mathrm{deg}(i)\f$ is the degree of vertex \f$i\f$ and
         \f$n\f$ is the number of vertices in the graph.
 
-        @return a ``scipy.sparse.csc_matrix`` representing the degree matrix
+        @return a ``stag.utility.SprsMat`` representing the degree matrix
         """
-        return self.internal_graph.degree_matrix()
+        deg_mat = utility.SprsMat(self.internal_graph.degree_matrix())
+        deg_mat.__parent = self
+        return deg_mat
     
-    @utility.return_sparse_matrix
-    def inverse_degree_matrix(self) -> scipy.sparse.csc_matrix:
+    def inverse_degree_matrix(self) -> stag.utility.SprsMat:
         r"""
         The inverse degree matrix of the graph.
 
         The degree matrix \f$D^{-1} \in \mathbb{R}^{n \times n}\f$
         is a diagonal matrix such that
 
         \f[
@@ -464,36 +463,39 @@
                     \end{array}
                 \right.
         \f]
 
         where \f$\mathrm{deg}(i)\f$ is the degree of vertex \f$i\f$ and
         \f$n\f$ is the number of vertices in the graph.
 
-        @return a ``scipy.sparse.csc_matrix`` representing the inverse degree matrix
+        @return a ``stag.utility.SprsMat`` representing the inverse degree matrix
         """
-        return self.internal_graph.inverse_degree_matrix()
-    
-    @utility.return_sparse_matrix
-    def lazy_random_walk_matrix(self) -> scipy.sparse.csc_matrix:
+        inv_deg_mat = utility.SprsMat(self.internal_graph.inverse_degree_matrix())
+        inv_deg_mat.__parent = self
+        return inv_deg_mat
+
+    def lazy_random_walk_matrix(self) -> stag.utility.SprsMat:
         """
         The lazy random walk matrix of the graph.
 
         The lazy random walk matrix is defined by
 
         \f[
             W = \frac 1 2 I + \frac 1 2 A D^{-1}
         \f]
 
         where \f$I\f$ is the identity matrix, \f$A\f$ is the graph adjacency
         matrix and \f$D\f$ is the degree matrix of the graph.
 
-        @return a ``scipy.sparse.csc_matrix`` representing the lazy random walk
+        @return a ``stag.utility.SprsMat`` representing the lazy random walk
                 matrix
         """
-        return self.internal_graph.lazy_random_walk_matrix()
+        rw_mat = utility.SprsMat(self.internal_graph.lazy_random_walk_matrix())
+        rw_mat.__parent = self
+        return rw_mat
 
     def total_volume(self) -> float:
         r"""
         The volume of the graph.
 
         The volume of a graph \f$G = (V, E, w)\f$ is defined by
 
@@ -525,24 +527,94 @@
         """
         The number of edges in the graph.
 
         This method ignores the weights of the edges.
         """
         return self.internal_graph.number_of_edges()
 
+    def add_edge(self, i: int, j: int, w: float):
+        """
+        Add an edge to the graph.
+
+        The edge goes from node \f$i\f$ to node \f$j\f$, and is added with
+        weight \f$w\f$. If there is already an edge from \f$i\f$ to \f$j\f$,
+        then \f$w\f$ is added to its weight.
+
+        If either of \f$i\f$ of \f$j\f$ are larger than the number of nodes
+        in the graph, the graph is resized to have enough nodes.
+        """
+        self.internal_graph.add_edge(i, j, w)
+
+    def remove_edge(self, i: int, j: int):
+        """
+        Remove an edge from the graph.
+
+        Remove any edge between nodes \f$i\f$ and \f$j\f$.
+        """
+        self.internal_graph.remove_edge(i, j)
+
+    def has_self_loops(self) -> bool:
+        """Returns a boolean indicating whether this graph contains self loops."""
+        return self.internal_graph.has_self_loops()
+
+    def is_connected(self) -> bool:
+        """
+        Returns a boolean indicating whether the graph is connected.
+
+        The running time of this method is \f$O(m)\f$ where \f$m\f$ is the
+        number of edges in the graph.
+        """
+        return self.internal_graph.is_connected()
+
+    @utility.convert_ndarrays
+    def subgraph(self, vertices: np.ndarray) -> 'Graph':
+        r"""
+        Construct and return a subgraph of this graph.
+
+        Note that the vertex indices will be changed in the subgraph.
+
+        @param vertices the vertices in the induced subgraph
+        @return a new stag.graph.Graph object representing the subgraph induced
+                by the given vertices
+        """
+        new_int_graph = self.internal_graph.subgraph(vertices)
+        return Graph(new_int_graph)
+
+    def disjoint_union(self, other: 'Graph') -> 'Graph':
+        r"""
+        Construct and return the disjoint union of this graph and another.
+
+        The disjoint union of two graphs \f$G\f$ and \f$H\f$ is a graph
+        containing \f$G\f$ and \f$H\f$ as disconnected subgraphs.
+
+        @param other the other graph to be combined with this one
+        @return a new stag.graph.Graph object representing the union of this
+                graph with the other one
+        """
+        new_int_graph = self.internal_graph.disjoint_union(other.internal_graph)
+        return Graph(new_int_graph)
+
     def degree(self, v: int) -> float:
         return self.internal_graph.degree(v)
 
     def degree_unweighted(self, v: int) -> int:
         return self.internal_graph.degree_unweighted(v)
 
+    @utility.convert_ndarrays
+    def degrees(self, vertices: np.ndarray) -> np.ndarray:
+        return self.internal_graph.degrees(vertices)
+
+    @utility.convert_ndarrays
+    def degrees_unweighted(self, vertices: np.ndarray) -> np.ndarray:
+        return self.internal_graph.degrees_unweighted(vertices)
+
     def neighbors(self, v: int) -> List[Edge]:
-        return self.internal_graph.neighbors(v)
+        return [Edge(a, b, c) for (a, b, c) in self.internal_graph.neighbors(v)]
 
-    def neighbors_unweighted(self, v: int) -> List[int]:
+    def neighbors_unweighted(self, v: int) -> np.ndarray:
         return self.internal_graph.neighbors_unweighted(v)
 
     def vertex_exists(self, v: int) -> bool:
         return self.internal_graph.vertex_exists(v)
 
     ##
     # \cond
@@ -552,49 +624,54 @@
         #
         # IMPORTANT NOTE
         # Checking whether two graphs are the same is thought to be a 'difficult'
         # problem, and so this method does not really check for mathematical equivalence.
         # Rather, we just check that the adjacency matrices are the same. As such, this method
         # should not be relied on to test for graph isomorphism!
         #
-
-        # Check basic size information about the two graphs first
-        if self.number_of_vertices() != other.number_of_vertices():
-            return False
-
-        if self.number_of_edges() != other.number_of_edges():
-            return False
-
-        # Check that the data vectors of the graph adjacency matrices are equal.
-        a1 = self.internal_graph.adjacency()
-        a2 = other.internal_graph.adjacency()
-        if stag_internal.sprsMatOuterStarts(a1) != stag_internal.sprsMatOuterStarts(a2):
-            return False
-        if stag_internal.sprsMatInnerIndices(a1) != stag_internal.sprsMatInnerIndices(a2):
-            return False
-        return stag_internal.sprsMatValues(a1) == stag_internal.sprsMatValues(a2)
+        if type(other) == Graph:
+            return self.internal_graph == other.internal_graph
+        else:
+            return NotImplemented
 
     def __ne__(self, other):
         return not self.__eq__(other)
 
+    def __add__(self, other):
+        if isinstance(other, Graph):
+            if other.number_of_vertices() != self.number_of_vertices():
+                raise ValueError("Number of vertices must be equal.")
+            return Graph(self.adjacency() + other.adjacency())
+        else:
+            return NotImplemented
+
+    def __mul__(self, other):
+        if isinstance(other, (int, float)):
+            return Graph(other * self.adjacency())
+        else:
+            return NotImplemented
+
+    def __rmul__(self, other):
+        return self.__mul__(other)
+
     ##
     # \endcond
     ##
 
     def to_networkx(self) -> networkx.Graph:
         """
         Construct a networkx graph object which is equivalent to this STAG graph.
 
         See the
         [networkx documentation](https://networkx.org/documentation/stable/reference/classes/graph.html).
         """
-        return networkx.Graph(self.adjacency())
+        return networkx.Graph(self.adjacency().to_scipy())
 
     def draw(self, **kwargs):
-        """
+        r"""
         Plot the graph with matplotlib.
 
         This uses the networkx draw method and accepts any the keyword arguments
         will be passed through directly.
 
         \par Example
 
@@ -605,81 +682,70 @@
         myGraph.draw()
         plt.show()
         \endcode
         """
         netx_graph = self.to_networkx()
         networkx.draw(netx_graph, **kwargs)
 
-##
-# \cond
-# A decorator which transforms a graph returned from the C++ library to the
-# python Graph object.
-##
-def return_graph(func):
-    def decorated_function(*args, **kwargs):
-        swig_graph = func(*args, **kwargs)
-        return Graph(None, internal_graph=swig_graph)
-
-    # Set the metadata of the returned function to match the original.
-    # This is used when generating the documentation
-    decorated_function.__doc__ = func.__doc__
-    decorated_function.__module__ = func.__module__
-    decorated_function.__signature__ = inspect.signature(func)
-
-    return decorated_function
-
-##
-# \endcond
-##
 
-@return_graph
 def cycle_graph(n) -> Graph:
     """
     Construct a cycle graph on n vertices.
 
     @param n the number of vertices in the constructed graph
     @return a stag.graph.Graph object representing a cycle graph
     """
-    return stag_internal.cycle_graph(n)
+    return Graph(stag_internal.cycle_graph(n))
 
 
-@return_graph
 def complete_graph(n) -> Graph:
     """
     Construct a complete graph on n vertices.
 
     @param n the number of vertices in the constructed graph
     @return a stag.graph.Graph object representing a complete graph
     """
-    return stag_internal.complete_graph(n)
+    return Graph(stag_internal.complete_graph(n))
 
 
-@return_graph
 def barbell_graph(n) -> Graph:
     """
     Construct a barbell graph. The barbell graph consists of 2 cliques on n
     vertices, connected by a single edge.
 
     @param n the number of vertices in each of the two cliques.
              The returned graph will have \f$2n\f$ vertices.
     @return a stag.graph.Graph object representing the barbell graph
     """
-    return stag_internal.barbell_graph(n)
+    return Graph(stag_internal.barbell_graph(n))
 
 
-@return_graph
 def star_graph(n) -> Graph:
     """
     Construct a star graph. The star graph consists of one central vertex
     connected by an edge to n-1 outer vertices.
 
     @param n the number of vertices in the constructed graph
     @return a stag.graph.Graph object representing the star graph
     """
-    return stag_internal.star_graph(n)
+    return Graph(stag_internal.star_graph(n))
+
+
+def identity_graph(n) -> Graph:
+    r"""
+    Construct the identity graph. The identity graph consists of \f$n\f$
+    vertices, each with a self-loop of weight \f$1\f$.
+
+    Both the adjacency matrix and Laplacian matrix of the identity graph are
+    equal to the identity matrix.
+
+    @param n the number of vertices in the constructed graph
+    @return a stag.graph.Graph object representing the identity graph
+    """
+    return Graph(stag_internal.identity_graph(n))
 
 
 def from_networkx(netx_graph: networkx.Graph,
                   edge_weight_attribute: str = "weight"):
     """
     Given a networkx graph, convert it to a stag.graph.Graph object.
```

### Comparing `stag-1.2.1/stag/graphio.py` & `stag-2.0.0/stag/graphio.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 """
 Read and write graphs to disk.
 """
 from . import stag_internal
 from . import graph
 
 
-@graph.return_graph
 def load_edgelist(filename: str) -> graph.Graph:
     """
     Load a graph from an edgelist file.
 
     We define an edgelist file in the following way.
       - Any lines beginning with '#' or '//' are ignored
       - Any blank lines are ignored
@@ -31,28 +30,27 @@
     2, 0, 0.5
     \endcode
 
     @param filename the name of the edgelist file to be loaded
     @return stag.graph.Graph object
     @throws runtime_error if the file doesn't exist or cannot be parsed as an edgelist
     """
-    return stag_internal.load_edgelist(filename)
+    return graph.Graph(stag_internal.load_edgelist(filename))
 
 
 def save_edgelist(g: graph.Graph, filename: str):
     """
     Save a graph as an edgelist file.
 
     @param g the graph object to be saved
     @param filename the name of the file to save the edgelist data to
     """
     stag_internal.save_edgelist(g.internal_graph, filename)
 
 
-@graph.return_graph
 def load_adjacencylist(filename: str) -> graph.Graph:
     r"""
      Load a graph from an adjacencylist file.
 
     The adjacency list file format is defined in the following way.
       - Any lines beginning with `#` or `//` are ignored
       - Any blank lines are ignored
@@ -84,15 +82,15 @@
     in a 'local' way without reading the entire graph into memory.
 
     @param filename the name of the adjacency list file to be loaded
     @return stag.graph.Graph object
     @throws runtime_error if the file doesn't exist or cannot be parsed as
             an adjacency list
     """
-    return stag_internal.load_adjacencylist(filename)
+    return graph.Graph(stag_internal.load_adjacencylist(filename))
 
 
 def save_adjacencylist(g: graph.Graph, filename: str):
     r"""
     Save a graph as an adjacency list file.
 
     @param g the graph object to be saved.
```

### Comparing `stag-1.2.1/stag/neo4j.py` & `stag-2.0.0/stag/neo4j.py`

 * *Files identical despite different names*

### Comparing `stag-1.2.1/stag/random.py` & `stag-2.0.0/stag/random.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 """
 Construct graphs from random models.
 """
 import numpy as np
-from typing import List
+from typing import Union
 from . import stag_internal
 from . import graph
 from . import utility
 
 
-@graph.return_graph
 def sbm(n: int, k: int, p: float, q: float, exact: bool = False) -> graph.Graph:
     r"""
     Generate a graph from the symmetric stochastic block model.
 
     Every cluster has the same number of vertices. For large enough values of
     \f$n\f$, this method samples from an approximate stochastic block model by
     default which significantly speeds up the execution time.
@@ -27,19 +26,19 @@
     @param k the number of clusters. Vertices are split evenly between clusters
     @param p the probability of including an edge inside a cluster.
     @param q the probability of including an edge between two clusters.
     @param exact (optional) whether to use the exact probability distribution
                   or an approximation.
     @return the randomly generated stag.graph.Graph
     """
-    return stag_internal.sbm(n, k, p, q, exact)
+    return graph.Graph(stag_internal.sbm(n, k, p, q, exact))
 
 
-@graph.return_graph
-def general_sbm(cluster_sizes: List[int],
+@utility.convert_ndarrays
+def general_sbm(cluster_sizes: np.ndarray,
                 probabilities: np.ndarray,
                 exact: bool = False) -> graph.Graph:
     r"""
     Generate a graph from the general stochastic block model.
 
     The `cluster_sizes` list specifies the number of vertices in each
     generated cluster.
@@ -60,62 +59,61 @@
     \par Example
 
     \code{python}
     import numpy as np
     import stag.graph
     import stag.random
 
-    cluster_sizes = [100, 20, 10]
+    cluster_sizes = np.asarray([100, 20, 10])
     prob_mat = np.asarray([[0.4, 0.1, 0.1],
                            [0.1, 0.7, 0],
                            [0.1, 0, 1]])
     my_graph = stag.random.general_sbm(cluster_sizes, prob_mat)
     print(my_graph.adjacency())
     \endcode
 
-    @param cluster_sizes a list of length \f$k\f$ with the number of vertices
+    @param cluster_sizes an array of length \f$k\f$ with the number of vertices
                          in each cluster.
     @param probabilities a \f$k \times k\f$ numpy matrix with the inter-cluster
                          probabilities.
     @param exact (optional) whether to use the exact probability distribution.
                  Default: false.
-    @return the randomly generated graph
+    @return the randomly generated stag.graph.Graph
     """
-    return stag_internal.general_sbm(stag_internal.vectorl(cluster_sizes),
-                                     probabilities.astype(float),
-                                     exact)
+    return graph.Graph(stag_internal.general_sbm(
+        cluster_sizes, utility.DenseMat(probabilities).internal_densemat, exact))
 
 
+@utility.convert_ndarrays
 def general_sbm_edgelist(filename: str,
-                         cluster_sizes: List[int],
+                         cluster_sizes: np.ndarray,
                          probabilities: np.ndarray,
-                         exact: bool = False):
+                         exact: bool = False) -> graph.Graph:
     r"""
     Generate a graph from the general stochastic block model and save the
     resulting graph as an edgelist file.
 
     This method uses only constant memory since the graph can be streamed to
     disk while it is being generated.
 
     @param filename the edgelist file to save the graph to
     @param cluster_sizes a list of length \f$k\f$ with the number of vertices in
                          each cluster.
     @param probabilities a \f$k \times k\f$ matrix with the inter-cluster
                          probabilities.
     @param exact (optional) whether to use the exact probability distribution.
                  Default: false.
+    @return the randomly generated stag.graph.Graph
     """
-    cluster_sizes = utility.possibly_convert_ndarray(cluster_sizes)
     return stag_internal.general_sbm_edgelist(filename,
-                                              stag_internal.vectorl(cluster_sizes),
-                                              probabilities.astype(float),
+                                              cluster_sizes,
+                                              utility.DenseMat(probabilities).internal_densemat,
                                               exact)
 
 
-@graph.return_graph
 def erdos_renyi(n: int, p: float, exact: bool = False) -> graph.Graph:
     r"""
     Generate a graph from the Erdos-Renyi model.
 
     For large values of \f$n\f$, this method will use an approximate version of the
     random model with running time \f$O(\mathrm{nnz})\f$ where \f$\mathrm{nnz}\f$
     is the number of edges in the sampled graph.
@@ -124,18 +122,18 @@
     will be used, with running time \f$O(n^2)\f$.
 
     @param n the number of vertices in the graph.
     @param p the probability of including each edge.
     @param exact (optional) whether to sample from the exact model.
     @return the randomly generated stag.graph.Graph
     """
-    return stag_internal.erdos_renyi(n, p, exact)
+    return graph.Graph(stag_internal.erdos_renyi(n, p, exact))
 
 
-def sbm_gt_labels(n: int, k: int) -> List[int]:
+def sbm_gt_labels(n: int, k: int) -> np.ndarray:
     r"""
     Construct a vector with the ground truth labels for a graph drawn from the
     symmetric stochastic block model.
 
     \par Example
 
     \code{python}
@@ -144,41 +142,43 @@
 
     n = 6
     k = 3
     myGraph = stag.random.sbm(n, k, 0.8, 0.1)
 
     gt_labels = stag.random.sbm_gt_labels(n, k)
 
-    # gt_labels is the list [0, 0, 1, 1, 2, 2].
+    # gt_labels is the numpy array [0, 0, 1, 1, 2, 2].
     \endcode
 
     @param n the number of vertices in the graph
     @param k the number of clusters
-    @return a list of integers containing the ground truth labels for the
+    @return an array of integers containing the ground truth labels for the
             vertices in the graph.
     """
-    return list(stag_internal.sbm_gt_labels(n, k))
+    return stag_internal.sbm_gt_labels(n, k)
 
 
-def general_sbm_gt_labels(cluster_sizes: List[int]) -> List[int]:
+@utility.convert_ndarrays
+def general_sbm_gt_labels(cluster_sizes: np.ndarray) -> np.ndarray:
     r"""
     Construct a vector with the ground truth labels for a graph drawn from the
     general stochastic block model.
 
     \par Example
 
     \code{python}
     import stag.graph
     import stag.random
+    import numpy as np
 
-    cluster_sizes = [4, 2]
+    cluster_sizes = np.asarray([4, 2])
     gt_labels = stag.random.general_sbm_gt_labels(cluster_sizes)
 
-    # gt_labels is the list [0, 0, 0, 0, 1, 1]
+    # gt_labels is the numpy array [0, 0, 0, 0, 1, 1]
     \endcode
 
     @param cluster_sizes a list of length \f$k\f$ with the number of vertices
                          in each cluster.
-    @return a vector containing the ground truth labels for the vertices in the
+    @return an array containing the ground truth labels for the vertices in the
             graph.
     """
-    return list(stag_internal.general_sbm_gt_labels(stag_internal.vectorl(cluster_sizes)))
+    return stag_internal.general_sbm_gt_labels(cluster_sizes)
```

### Comparing `stag-1.2.1/stag/stag_internal_wrap.h` & `stag-2.0.0/stag/stag_internal_wrap.h`

 * *Files 14% similar despite different names*

```diff
@@ -15,21 +15,21 @@
 #include <string>
 
 
 class SwigDirector_LocalGraph : public stag::LocalGraph, public Swig::Director {
 
 public:
     SwigDirector_LocalGraph(PyObject *self);
-    virtual double degree(stag_int v);
-    virtual stag_int degree_unweighted(stag_int v);
-    virtual std::vector< stag::edge, std::allocator< stag::edge > > neighbors(stag_int v);
-    virtual std::vector< stag_int, std::allocator< stag_int > > neighbors_unweighted(stag_int v);
-    virtual std::vector< double, std::allocator< double > > degrees(std::vector< stag_int, std::allocator< stag_int > > vertices);
-    virtual std::vector< stag_int, std::allocator< stag_int > > degrees_unweighted(std::vector< stag_int, std::allocator< stag_int > > vertices);
-    virtual bool vertex_exists(stag_int v);
+    virtual StagReal degree(StagInt v);
+    virtual StagInt degree_unweighted(StagInt v);
+    virtual std::vector< stag::edge > neighbors(StagInt v);
+    virtual std::vector< StagInt > neighbors_unweighted(StagInt v);
+    virtual std::vector< StagReal > degrees(std::vector< StagInt > vertices);
+    virtual std::vector< StagInt > degrees_unweighted(std::vector< StagInt > vertices);
+    virtual bool vertex_exists(StagInt v);
     virtual ~SwigDirector_LocalGraph();
 
 /* Internal director utilities */
 public:
     bool swig_get_inner(const char *swig_protected_method_name) const {
       std::map<std::string, bool>::const_iterator iv = swig_inner.find(swig_protected_method_name);
       return (iv != swig_inner.end() ? iv->second : false);
```

### Comparing `stag-1.2.1/stag/stag_lib/CMakeLists.txt` & `stag-2.0.0/stag/stag_lib/CMakeLists.txt`

 * *Files 20% similar despite different names*

```diff
@@ -4,30 +4,39 @@
         stag.h
         graph.h
         utility.h
         graphio.h
         random.h
         cluster.h
         spectrum.h
+        lsh.h
+        kde.h
+        definitions.h
+        data.h
         )
 
 set(HEADER_FILES
         ${STAG_PUBLIC_HEADERS}
         KMeansRex/KMeansRexCore.h
         KMeansRex/KMeansRexCoreInterface.h
         KMeansRex/mersenneTwister2002.h
+        multithreading/ctpl_stl.h
+        indicators/indicators.hpp
         )
 
 set(SOURCE_FILES
-        graph.cpp
         utility.cpp
+        graph.cpp
         graphio.cpp
         random.cpp
-        cluster.cpp
         spectrum.cpp
+        cluster.cpp
+        lsh.cpp
+        kde.cpp
+        data.cpp
         KMeansRex/KMeansRexCore.cpp
         )
 
 # Generate correct files on windows
 set(CMAKE_WINDOWS_EXPORT_ALL_SYMBOLS ON)
 
 # Find and include the Eigen library
@@ -38,36 +47,48 @@
 # Find and include the Spectra library
 find_package(Spectra 1.0.1 REQUIRED)
 get_property(SPECTRA_INCLUDE_DIR TARGET Spectra::Spectra
              PROPERTY INTERFACE_INCLUDE_DIRECTORIES)
 message(STATUS "[stag] Found Spectra: ${SPECTRA_INCLUDE_DIR}")
 include_directories(${SPECTRA_INCLUDE_DIR})
 
+set(THREADS_PREFER_PTHREAD_FLAG ON)
+find_package(Threads REQUIRED)
+message(STATUS "[stag] Found Threads")
+
 #####################################
 # Define the STAG library
 #####################################
 # We would like to define two version of the library: shared and static.
 # In order to do this, we first build an 'object' library which compiles the
 # sources into object files.
 add_library(stag_object OBJECT ${SOURCE_FILES} ${HEADER_FILES})
 set_property(TARGET stag_object PROPERTY POSITION_INDEPENDENT_CODE 1)
 
 # Build the shared library which will be installed
 add_library(stag SHARED $<TARGET_OBJECTS:stag_object>)
 set_target_properties(stag PROPERTIES PREFIX "")
-set_target_properties(stag PROPERTIES PUBLIC_HEADER "${STAG_PUBLIC_HEADERS}")
+target_link_libraries(stag PRIVATE Threads::Threads)
 
 # Define a static version of the STAG library for the stagtools
 add_library(stag_static STATIC $<TARGET_OBJECTS:stag_object>)
+target_link_libraries(stag_static PRIVATE Threads::Threads)
 
 # Configure the compiler options to error on warnings
 if(MSVC)
+    message(STATUS "[stag] Compiling for Windows.")
     set(_COMPILE_OPTS /W4)
 else()
-    set(_COMPILE_OPTS -Werror -Wall -Wextra)
+    if (CMAKE_BUILD_TYPE STREQUAL "Release" OR CMAKE_BUILD_TYPE STREQUAL "RELEASE")
+        message(STATUS "[stag] Enabling compiler optimisations.")
+        set(_COMPILE_OPTS -Wall -Wextra -O3)
+    else()
+        message(STATUS "[stag] Disabling compiler optimisations.")
+        set(_COMPILE_OPTS -Wall -Wextra)
+    endif()
 endif()
 message(STATUS "[stag] Set compiler options: ${_COMPILE_OPTS}")
 target_compile_options(stag_object PRIVATE "${_COMPILE_OPTS}")
 target_compile_options(stag PRIVATE "${_COMPILE_OPTS}")
 target_compile_options(stag_static PRIVATE "${_COMPILE_OPTS}")
 
 ######################################
@@ -75,13 +96,18 @@
 ######################################
 include(CMakePackageConfigHelpers)
 
 configure_package_config_file("${CMAKE_CURRENT_LIST_DIR}/stagConfig.cmake.in"
                               "${CMAKE_CURRENT_BINARY_DIR}/stagConfig.cmake"
                               INSTALL_DESTINATION lib/stag)
 
+# Install the STAG shared library.
 install(TARGETS stag
-        LIBRARY DESTINATION lib/stag
-        PUBLIC_HEADER DESTINATION include/stag)
+        LIBRARY DESTINATION lib/stag)
+
+# Install the STAG headers, maintaining the directory structure.
+install(DIRECTORY "${CMAKE_SOURCE_DIR}/stag_lib/"
+        DESTINATION "include/stag"
+        FILES_MATCHING PATTERN "*.h")
 
 install(FILES "${CMAKE_CURRENT_BINARY_DIR}/stagConfig.cmake"
         DESTINATION lib/stag)
```

### Comparing `stag-1.2.1/stag/stag_lib/KMeansRex/KMeansRexCore.cpp` & `stag-2.0.0/stag/stag_lib/KMeansRex/KMeansRexCore.cpp`

 * *Files 14% similar despite different names*

```diff
@@ -24,17 +24,45 @@
 External "C" function interfaces (for calling from Python)
 * RunKMeans          : compute cluster centers and assignments via lloyd
 * SampleRowsPlusPlus : get just a plusplus initialization
 
 Dependencies:
   mersenneTwister2002.c : random number generator
 
-Author: Mike Hughes (www.michaelchughes.com)
-Date:   2 April 2013
-*/
+This file is released under the GPL license, with the following additional
+requirements.
+
+Copyright (c) 2013-2015, Michael C. Hughes
+All rights reserved.
+
+Redistribution and use in source and binary forms, with or without modification,
+are permitted provided that the following conditions are met:
+
+1. Redistributions of source code must retain the above copyright notice,
+   this list of conditions and the following disclaimer.
+
+2. Redistributions in binary form must reproduce the above copyright notice,
+   this list of conditions and the following disclaimer in the documentation
+   and/or other materials provided with the distribution.
+
+3. Neither the name of the copyright holder nor the names of its contributors
+   may be used to endorse or promote products derived from this software without
+   specific prior written permission.
+
+THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS" AND
+ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED
+WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE DISCLAIMED.
+IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE FOR ANY DIRECT,
+INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING,
+BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE,
+DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF
+LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE
+OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF
+ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+ */
 
 #include <iostream>
 #include "KMeansRexCoreInterface.h"
 #include "mersenneTwister2002.h"
 #include "Eigen/Dense"
 
 using namespace Eigen;
```

### Comparing `stag-1.2.1/stag/stag_lib/KMeansRex/mersenneTwister2002.h` & `stag-2.0.0/stag/stag_lib/KMeansRex/mersenneTwister2002.h`

 * *Files identical despite different names*

### Comparing `stag-1.2.1/stag/stag_lib/cluster.h` & `stag-2.0.0/stag/stag_lib/spectrum.h`

 * *Files 24% similar despite different names*

```diff
@@ -1,215 +1,219 @@
-//
-// Graph clustering algorithms based on spectral methods.
-//
-// This file is provided as part of the STAG library and released under the MIT
-// license.
-//
+/*
+   This file is provided as part of the STAG library and released under the GPL
+   license.
+*/
 
 /**
- * @file cluster.h
- * \brief Algorithms for finding clusters in graphs.
+ * @file spectrum.h
+ * \brief Methods for computing eigenvalues and eigenvectors of graph matrices.
  *
- * The two key clustering methods provided by this module are stag::spectral_cluster and stag::local_cluster.
+ * For applications in spectral graph theory, we are interested in the spectrum
+ * of the Graph adjacency and Laplacian matrix spectrums.
+ *
+ * Moreover, for each matrix, we are usually interested in the extreme
+ * eigenvalues at one end of the spectrum or the other.
+ *
+ * As such, this module provides methods for computing the extreme eigenvalues
+ * and eigenvectors of normalised or unnormalised adjacency or Laplacian matrix
+ * of some graph.
+ *
+ * We limit ourselves to these cases as this is the most common application in
+ * spectral Graph theory, and these matrices are 'well-behaved' for the solver
+ * algorithms. If you'd like to compute the spectrum of a more general matrix,
+ * you could consider using the Spectra C++ library directly.
  */
 
-#ifndef STAG_TEST_CLUSTER_H
-#define STAG_TEST_CLUSTER_H
+#ifndef STAG_TEST_SPECTRUM_H
+#define STAG_TEST_SPECTRUM_H
+
+// Standard C++ libraries
+#include <tuple>
 
-#include <vector>
+// Other libraries
+#include <Eigen/Core>
+#include <Spectra/SymEigsSolver.h>
+#include <Spectra/SymEigsShiftSolver.h>
+#include <Spectra/MatOp/SparseSymMatProd.h>
+#include <Spectra/MatOp/SparseSymShiftSolve.h>
 
-#include <graph.h>
+// STAG modules
+#include "graph.h"
 
 namespace stag {
+  /**
+   * \cond
+   * The spectra operation for multiplying the SprsMat type
+   *
+   * Undocumented by doxygen.
+   */
+  typedef Spectra::SparseSymMatProd<StagReal, Eigen::Upper, Eigen::ColMajor, StagInt> SprsMatProdOp;
+  typedef Spectra::SparseSymShiftSolve<StagReal, Eigen::Upper, Eigen::ColMajor, StagInt> SprsMatShiftSolveOp;
+  /**
+   * \endcond
+   */
 
   /**
-   * Spectral clustering algorithm.
+   * A convenience type for returning eigenvalues and eigenvectors together.
+   */
+  typedef std::tuple<Eigen::VectorXd, Eigen::MatrixXd> EigenSystem;
+
+  /**
+   * When computing eigenvectors and eigenvalues, we always compute the values
+   * at one end of the spectrum or the other.
    *
-   * This is a simple graph clustering method, which provides a clustering of the entire graph.
-   * To use spectral clustering, simply pass a `stag::Graph` object
-   * and the number of clusters you would like to find.
+   * The EigenSortRule is used to specify whether to compute the largest or
+   * smallest eigenvalues.
+   */
+  enum EigenSortRule {Largest, Smallest};
+
+  /**
+   * When computing eigenvectors and eigenvalues, these values are used to
+   * specify which Graph matrix we are using to compute the spectrum.
+   */
+  enum GraphMatrix {Adjacency, Laplacian, NormalisedLaplacian};
+
+  /**
+   * Compute the eigenvalues and eigenvectors of a graph matrix.
+   *
+   * Computes a given number of eigenvectors at one end of the spectrum of a
+   * graph matrix.
+   *
+   * The following example demonstrates how to compute the 3 largest eigenvectors
+   * and eigenvalues of the normalised laplacian of a cycle graph.
    *
    * \code{.cpp}
-   *     #include <iostream>
+   *     #include <Spectra/SymEigsSolver.h>
    *     #include <stag/graph.h>
-   *     #include <stag/cluster.h>
+   *     #include <stag/spectrum.h>
    *
    *     int main() {
-   *       stag::Graph myGraph = stag::barbell_graph(10);
-   *       std::vector<stag_int> clusters = stag::spectral_cluster(&myGraph, 2);
+   *       // Create a cycle graph
+   *       stag::Graph myGraph = stag::cycle_graph(10);
+   *
+   *       // Compute a few eigenvalues and eigenvectors
+   *       StagInt k = 3;
+   *       stag::EigenSystem eigensystem = stag::compute_eigensystem(
+   *           myGraph, stag::GraphMatrix::NormalisedLaplacian,
+   *           k, stag::EigenSortRule::Largest);
    *
-   *       for (auto c : clusters) {
-   *         std::cout << c << ", ";
-   *       }
-   *       std::cout << std::endl;
+   *       Eigen::VectorXd eigenvalues = get<0>(eigensystem);
+   *       Eigen::MatrixXd eigenvectors = get<1>(eigensystem);
    *
    *       return 0;
    *     }
    * \endcode
-   * 
-   * The spectral clustering algorithm has the following steps.
-   *   - Compute the \f$k\f$ smallest eigenvectors of the normalised Laplacian matrix.
-   *   - Embed the vertices into \f$\mathbb{R}^k\f$ according to the eigenvectors.
-   *   - Cluster the vertices into \f$k\f$ clusters using a \f$k\f$-means clustering algorithm.
    *
-   * @param graph the graph object to be clustered
-   * @param k the number of clusters to find. Should be less than \f$n/2\f$.
-   * @return a vector giving the cluster membership for each vertex in the graph
-   *
-   * \par References
-   * A. Ng, M. Jordan, Y. Weiss.
-   * On spectral clustering: Analysis and an algorithm. NeurIPS'01
+   * @param g the graph on which to operate
+   * @param mat which graph matrix to use to compute the spectrum
+   * @param num_eigs the number of eigenvalues and eigenvectors to compute
+   * @param which a stag::EigenSortRule value indicating which eigenvectors to return
+   * @returns a stag::EigenSystem object containing the computed eigenvalues and eigenvectors
+   * @throws std::runtime_error if the eigenvalue calculation does not converge
    */
-  std::vector<stag_int> spectral_cluster(stag::Graph* graph, stag_int k);
-
+  stag::EigenSystem compute_eigensystem(stag::Graph* g,
+                                        stag::GraphMatrix mat,
+                                        StagInt num_eigs,
+                                        stag::EigenSortRule which);
 
   /**
-   * Local clustering algorithm based on personalised Pagerank.
-   *
-   * Given a graph and starting vertex, return a cluster which is close to the
-   * starting vertex.
+   * Compute the eigenvectors of a graph matrix.
    *
-   * This method uses the ACL local clustering algorithm.
+   * If you would like to calculate the eigenvectors and eigenvalues together, then
+   * you should instead use stag::compute_eigensystem.
    *
-   * @param graph a graph object implementing the LocalGraph interface
-   * @param seed_vertex the starting vertex in the graph
-   * @param target_volume the approximate volume of the cluster you would like to find
-   * @return a vector containing the indices of vectors considered to be in the
-   *         same cluster as the seed_vertex.
-   *
-   * \par References
-   * R. Andersen, F. Chung, K. Lang.
-   * Local graph partitioning using pagerank vectors. FOCS'06
+   * @param g the graph on which to operate
+   * @param mat which graph matrix to use to compute the spectrum
+   * @param num_eigs the number of eigenvectors to compute
+   * @param which a stag::EigenSortRule value indicating which eigenvectors to return
+   * @returns an Eigen::MatrixXd object containing the computed eigenvectors
+   * @throws std::runtime_error if the eigenvector calculation does not converge
    */
-  std::vector<stag_int> local_cluster(stag::LocalGraph* graph, stag_int seed_vertex, double target_volume);
+  Eigen::MatrixXd compute_eigenvectors(stag::Graph* g,
+                                       stag::GraphMatrix mat,
+                                       StagInt num_eigs,
+                                       stag::EigenSortRule which);
 
   /**
-   * The ACL local clustering algorithm. Given a graph and starting vertex,
-   * return a cluster close to the starting vertex, constructed in a local way.
+   * Compute the eigenvalues of a graph matrix.
    *
-   * The locality parameter is passed as the alpha parameter in the personalised
-   * Pagerank calculation.
+   * Computes a given number of eigenvalues at one end of the spectrum of a
+   * graph matrix.
    *
-   * @param graph a graph object implementing the LocalGraph interface
-   * @param seed_vertex the starting vertex in the graph
-   * @param locality a value in \f$[0, 1]\f$ indicating how 'local' the cluster should
-   *                 be. A value of \f$1\f$ will return only the seed vertex,
-   *                 and a value of \f$0\f$ will explore the whole graph.
-   * @param error (optional) - the acceptable error in the calculation of the approximate
-   *                           pagerank. Default \f$0.001\f$.
-   * @return a vector containing the indices of vectors considered to be in the
-   *         same cluster as the seed_vertex.
+   * If you would like to calculate the eigenvectors and eigenvalues together, then
+   * you should instead use stag::compute_eigensystem.
    *
-   * \par References
-   * R. Andersen, F. Chung, K. Lang.
-   * Local graph partitioning using pagerank vectors. FOCS'06
+   * @param g the graph on which to operate
+   * @param mat which graph matrix to use to compute the spectrum
+   * @param num_eigs the number of eigenvalues to compute
+   * @param which a stag::EigenSortRule value indicating which eigenvalues to return
+   * @returns an Eigen::VectorXd object containing the computed eigenvalues
+   * @throws std::runtime_error if the eigenvalue calculation does not converge
    */
-  std::vector<stag_int> local_cluster_acl(stag::LocalGraph* graph, stag_int seed_vertex, double locality, double error);
+  Eigen::VectorXd compute_eigenvalues(stag::Graph* g,
+                                      stag::GraphMatrix mat,
+                                      StagInt num_eigs,
+                                      stag::EigenSortRule which);
 
   /**
-   * \overload
-   */
-  std::vector<stag_int> local_cluster_acl(stag::LocalGraph* graph, stag_int seed_vertex, double locality);
-
-  /**
-   * Compute the approximate Pagerank vector.
+   * Apply the power method to compute the dominant eigenvector of a matrix.
    *
-   * The parameters seed_vector, alpha, and epsilon are used as described in the ACL paper.
+   * Given a matrix \f$M\f$, an initial vector \f$v_0\f$, and a number of
+   * iterations \f$t\f$, the power method calculates the vector
    *
-   * Note that the dimension of the returned vectors may not match the correct
-   * number of vertices in the graph provided since the approximate
-   * Pagerank is computed locally.
-   *
-   * @param graph a stag::LocalGraph object
-   * @param seed_vector the seed vector of the personalised Pagerank
-   * @param alpha the locality parameter of the personalised Pagerank
-   * @param epsilon the error parameter of the personalised Pagerank
-   * @return A tuple of sparse column vectors corresponding to
-   *          - p: the approximate Pagerank vector
-   *          - r: the residual vector
+   * \f[
+   *    v_t = M^t v_0,
+   * \f]
    *
-   *         By the definition of approximate Pagerank, it holds that
-   *            p + ppr(r, alpha) = ppr(s, alpha).
+   * which is close to the eigenvector of \f$M\f$ with largest eigenvalue.
    *
-   * @throws std::invalid_argument if the provided seed_vector is not a column vector.
+   * The running time of the power method is \f$O(t \cdot \mathrm{nnz}(M))\f$, where
+   * \f$\mathrm{nnz}(M)\f$ is the number of non-zero elements in the matrix \f$M\f$.
    *
-   * \par References
-   * R. Andersen, F. Chung, K. Lang.
-   * Local graph partitioning using pagerank vectors. FOCS'06
+   * @param mat the matrix \f$M\f$ on which to operate.
+   * @param num_iterations (optional) the number of iterations of the power
+   *                       method to apply. It this argument is omitted,
+   *                       \f$O(\log(n))\f$ iterations are used which results
+   *                       in a vector whose Rayleigh quotient is a \f$(1 - \epsilon)\f$
+   *                       approximation of the dominant eigenvalue.
+   * @param initial_vector (optional) the initial vector to use for the power
+   *                       iteration. If this argument is omitted, a random unit
+   *                       vector will be used.
+   * @return the vector \f$v_t\f$ computed by repeated multiplication with \f$M\f$.
    */
-  std::tuple<SprsMat, SprsMat> approximate_pagerank(stag::LocalGraph* graph,
-                                                    SprsMat &seed_vector,
-                                                    double alpha,
-                                                    double epsilon);
+  Eigen::VectorXd power_method(const SprsMat* mat, StagInt num_iterations,
+                               Eigen::VectorXd initial_vector);
 
   /**
-   * Find the sweep set of the given vector with the minimum conductance.
-   *
-   * First, sort the vector such that \f$v_1<= \ldots <= v_n\f$. Then let
-   *
-   * \f[
-   *     S_i = \{v_j : j <= i\}
-   * \f]
-   *
-   * and return the set of original indices corresponding to
-   *
-   * \f[
-   *     \mathrm{argmin}_i \phi(S_i)
-   * \f]
-   *
-   * where \f$\phi(S)\f$ is the conductance of \f$S\f$.
-   *
-   * This method is expected to be run on vectors whose support is much less
-   * than the total size of the graph. If the total volume of the support of vec
-   * is larger than half of the volume of an entire graph, then this method may
-   * return unexpected results.
-   *
-   * Note that the caller is responsible for any required normalisation of the
-   * input vector. In particular, this method does not normalise the vector by
-   * the node degrees.
-   *
-   * @param graph a stag::LocalGraph object
-   * @param vec the vector to sweep over
-   * @return a vector containing the indices of vec which give the minimum
-   *         conductance in the given graph
+   * \overload
    */
-  std::vector<stag_int> sweep_set_conductance(stag::LocalGraph* graph,
-                                              SprsMat& vec);
+  Eigen::VectorXd power_method(const SprsMat* mat, StagInt num_iterations);
 
   /**
-   * Compute the Adjusted Rand Index between two label vectors.
-   *
-   * @param gt_labels the ground truth labels for the dataset
-   * @param labels the candidate labels whose ARI should be calculated
-   * @return the ARI between the two labels vectors
-   *
-   * \par References
-   * W. M. Rand.
-   * Objective criteria for the evaluation of clustering methods.
-   * Journal of the American Statistical Association. 66 (336): 846–850. 1971.
+   * \overload
+   */
+  Eigen::VectorXd power_method(const SprsMat* mat,
+                               Eigen::VectorXd initial_vector);
+
+  /**
+   * \overload
    */
-  double adjusted_rand_index(std::vector<stag_int>& gt_labels,
-                             std::vector<stag_int>& labels);
+  Eigen::VectorXd power_method(const SprsMat* mat);
 
   /**
-   * Compute the conductance of the given cluster in a graph.
+   * Compute the Rayleigh quotient of the given vector and matrix.
    *
-   * Given a graph \f$G = (V, E)\f$, the conductance of \f$S \subseteq V\f$
-   * is defined to be
+   * Given a matrix \f$M\f$, the Rayleigh quotient of vector \f$v\f$ is
    *
    * \f[
-   *    \phi(S) = \frac{w(S, V \setminus S)}{\mathrm{vol}(S)},
+   *    R(M, v) = \frac{v^\top M v}{v^\top v}.
    * \f]
    *
-   * where \f$\mathrm{vol}(S) = \sum_{v \in S} \mathrm{deg}(v)\f$ is the volume
-   * of \f$S\f$ and \f$w(S, V \setminus S)\f$ is the total weight of edges crossing
-   * the cut between \f$S\f$ and \f$V \setminus S\f$.
-   *
-   * @param graph a stag::LocalGraph object representing \f$G\f$.
-   * @param cluster a vector of node IDs in \f$S\f$.
-   * @return the conductance \f$\phi_G(S)\f$.
+   * @param mat a sparse matrix \f$M \in \mathbb{R}^{n \times n}\f$.
+   * @param vec a vector \f$v \in \mathbb{R}^n\f$.
+   * @return the Rayleigh quotient \f$R(M, v)\f$.
    */
-  double conductance(stag::LocalGraph* graph,
-                     std::vector<stag_int>& cluster);
+  StagReal rayleigh_quotient(const SprsMat* mat, Eigen::VectorXd& vec);
 }
 
-#endif //STAG_TEST_CLUSTER_H
+
+#endif //STAG_TEST_SPECTRUM_H
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `stag-1.2.1/stag/stag_lib/graph.cpp` & `stag-2.0.0/stag/stag_lib/graph.cpp`

 * *Files 25% similar despite different names*

```diff
@@ -1,52 +1,140 @@
-//
-// This file is provided as part of the STAG library and released under the MIT
-// license.
-//
+/*
+   This file is provided as part of the STAG library and released under the GPL
+   license.
+*/
 #include <stdexcept>
 #include <fstream>
 #include <unordered_map>
+#include <unordered_set>
+#include <set>
 #include "graph.h"
 #include "utility.h"
 #include "graphio.h"
+#include "cluster.h"
 
 
 //------------------------------------------------------------------------------
 // Graph Object Constructors
 //------------------------------------------------------------------------------
+/**
+ * Given a matrix, which is either an adjacency matrix OR a Laplacian matrix,
+ * return the adjacency matrix of the graph.
+ *
+ * Throws a std::domain_error if the provided matrix doesn't look like an
+ * adjacency matrix or Laplacian matrix of an unsigned graph.
+ */
+SprsMat adjacency_from_adj_or_lap(const SprsMat& matrix) {
+  // Since we support only graphs with positive edge weights,
+  // we can just check for negative entries in the matrix. If the matrix contains
+  // negative entries, then it must be the Laplacian. Otherwise, we take it to
+  // be an adjacency matrix.
+  //
+  // If we find a negative entry, then we check the following properties of the
+  // Laplacian matrix:
+  //    - no positive off-diagonal entries
+  //    - diagonal entries are non-negative
+  //    - matrix is diagonally dominant
+  SprsMat adjacency_matrix(matrix.rows(), matrix.cols());
+  bool found_negative_value = false;
+  bool positive_off_diagonal_value = false;
+  bool diagonally_dominant = true;
+  for (int k = 0; k < matrix.outerSize() ; ++k) {
+    StagReal col_total = 0;
+    for (SprsMat::InnerIterator it(matrix, k); it; ++it) {
+      col_total += it.value();
+      if (it.value() < 0) {
+        found_negative_value = true;
+      } else {
+        if (it.row() != it.col()) positive_off_diagonal_value = true;
+      }
+    }
+    if (col_total < 0) diagonally_dominant = false;
+  }
 
-stag::Graph::Graph(const SprsMat& adjacency_matrix) {
-  // Load the adjacency matrix into this object.
-  adjacency_matrix_ = adjacency_matrix;
-  adjacency_matrix_.makeCompressed();
+  if (found_negative_value) {
+    // Check that the matrix is diagonally dominant and has no positive
+    // off-diagonal entries.
+    if (positive_off_diagonal_value) throw std::domain_error("Off-diagonal entries should be all negative or all positive.");
+    if (!diagonally_dominant) throw std::domain_error("Laplacian matrix should be diagonally dominant.");
+
+    // The adjacency matrix is D - L
+    // First set it to negative the Laplacian, and then update the diagonal
+    // entries.
+    adjacency_matrix = -matrix;
+
+    // The self-loop weights are equal to the difference between the diagonal
+    // entry of the Laplacian and the rest of the entries in the row/column
+    Eigen::VectorXd self_loop_weights = matrix * Eigen::VectorXd::Ones(matrix.cols());
+    for (auto i = 0; i < matrix.cols(); i++) {
+      adjacency_matrix.coeffRef(i, i) = self_loop_weights.coeff(i);
+    }
+  } else {
+    adjacency_matrix = matrix;
+  }
+  // Due to floating-point errors, we sometimes see tiny floats showing up
+  // in place of zeros. We don't want to introduce self-loops with tiny weights
+  // so we set these to 0.
+  adjacency_matrix.prune([](const StagInt& row, const StagInt& col, const StagReal& value)
+                          {
+                            (void) row;
+                            (void) col;
+                            return value > EPSILON;
+                          });
+
+  return adjacency_matrix;
+}
+
+stag::Graph::Graph(const SprsMat& matrix) {
+  // Get the adjacency matrix from the provided (adjacency or Laplacian) matrix
+  adjacency_matrix_ = adjacency_from_adj_or_lap(matrix);
 
   // The number of vertices is the dimensions of the adjacency matrix
   number_of_vertices_ = adjacency_matrix_.outerSize();
 
+  // Check whether the graph has any self-loops
+  has_self_loops_ = false;
+  for (auto i = 0; i < number_of_vertices_; i++) {
+    if (adjacency_matrix_.coeff(i, i) != 0) {
+      has_self_loops_ = true;
+      break;
+    }
+  }
+
   // Set the flags to indicate which matrices have been initialised.
   lap_init_ = false;
   signless_lap_init_ = false;
   signless_norm_lap_init_ = false;
   deg_init_ = false;
   inv_deg_init_ = false;
   norm_lap_init_ = false;
   lazy_rand_walk_init_ = false;
 
   // Check that the graph is configured correctly
   self_test_();
 }
 
-stag::Graph::Graph(std::vector<stag_int> &outerStarts, std::vector<stag_int> &innerIndices,
-                   std::vector<double> &values) {
+stag::Graph::Graph(std::vector<StagInt> &outerStarts, std::vector<StagInt> &innerIndices,
+                   std::vector<StagReal> &values) {
   // Map the provided data vectors to the sparse matrix type.
-  adjacency_matrix_ = stag::sprsMatFromVectors(outerStarts, innerIndices, values);
+  SprsMat matrix = stag::sprsMatFromVectors(outerStarts, innerIndices, values);
+  adjacency_matrix_ = adjacency_from_adj_or_lap(matrix);
 
   // The number of vertices is the dimensions of the adjacency matrix
   number_of_vertices_ = adjacency_matrix_.outerSize();
 
+  // Check whether the graph has any self-loops
+  has_self_loops_ = false;
+  for (auto i = 0; i < number_of_vertices_; i++) {
+    if (adjacency_matrix_.coeff(i, i) != 0) {
+      has_self_loops_ = true;
+      break;
+    }
+  }
+
   // Set the flags to indicate which matrices have been initialised.
   lap_init_ = false;
   signless_lap_init_ = false;
   signless_norm_lap_init_ = false;
   deg_init_ = false;
   inv_deg_init_ = false;
   norm_lap_init_ = false;
@@ -95,32 +183,119 @@
 }
 
 const SprsMat* stag::Graph::lazy_random_walk_matrix() {
   initialise_lazy_random_walk_matrix_();
   return &lazy_random_walk_matrix_;
 }
 
-double stag::Graph::total_volume() {
-  Eigen::VectorXd degrees = adjacency_matrix_ * Eigen::VectorXd::Ones(adjacency_matrix_.cols());
-  return degrees.sum();
+StagReal stag::Graph::total_volume() {
+  // We will compute the total volume from the degree matrix of the graph.
+  initialise_degree_matrix_();
+
+  StagReal vol = 0;
+  for (int k = 0; k < degree_matrix_.outerSize() ; ++k) {
+    for (SprsMat::InnerIterator it(degree_matrix_, k); it; ++it) {
+      vol += it.value();
+    }
+  }
+
+  return vol;
 }
 
-double stag::Graph::average_degree() {
+StagReal stag::Graph::average_degree() {
   return total_volume() / number_of_vertices_;
 }
 
-stag_int stag::Graph::number_of_vertices() const {
+StagInt stag::Graph::number_of_vertices() const {
   return number_of_vertices_;
 }
 
-stag_int stag::Graph::number_of_edges() const {
-  return adjacency_matrix_.nonZeros() / 2;
+StagInt stag::Graph::number_of_edges() const {
+  StagInt nnz = adjacency_matrix_.nonZeros();
+
+  if (has_self_loops_) {
+    // If there are self loops in the graph, then we need to count the non-zeros
+    // on the diagonal twice.
+    for (auto i = 0; i < number_of_vertices_; i++) {
+      if (adjacency_matrix_.coeff(i, i) != 0) nnz++;
+    }
+
+    // Now, we have counted every edge twice.
+    return nnz / 2;
+  } else {
+    // If there are no self loops in the graph, then the number of edges is
+    // half the number of non-zero elements in the adjacency matrix.
+    return nnz / 2;
+  }
 }
 
-void stag::Graph::check_vertex_argument(stag_int v) {
+void stag::Graph::add_edge(StagInt i, StagInt j, StagReal w) {
+  number_of_vertices_ = MAX(number_of_vertices_, MAX(i, j) + 1);
+  adjacency_matrix_.conservativeResize(number_of_vertices_, number_of_vertices_);
+  adjacency_matrix_.coeffRef(i, j) += w;
+  adjacency_matrix_.coeffRef(j, i) += w;
+  adjacency_matrix_.makeCompressed();
+
+  if (i == j) {
+    has_self_loops_ = true;
+  }
+
+  // Set the flags to indicate which matrices have been initialised.
+  lap_init_ = false;
+  signless_lap_init_ = false;
+  signless_norm_lap_init_ = false;
+  deg_init_ = false;
+  inv_deg_init_ = false;
+  norm_lap_init_ = false;
+  lazy_rand_walk_init_ = false;
+}
+
+void stag::Graph::remove_edge(StagInt i, StagInt j) {
+  if (i >= number_of_vertices_ || j >= number_of_vertices_) return;
+
+  adjacency_matrix_.coeffRef(i, j) = 0;
+  adjacency_matrix_.coeffRef(j, i) = 0;
+  adjacency_matrix_.prune(0.0);
+  adjacency_matrix_.makeCompressed();
+
+  if (i == j) {
+    assert(has_self_loops_);
+
+    // If we removed a self-loop, we need to check whether there is still
+    // a self loop.
+    has_self_loops_ = false;
+    for (auto i = 0; i < number_of_vertices_; i++) {
+      if (adjacency_matrix_.coeff(i, i) != 0) {
+        has_self_loops_ = true;
+        break;
+      }
+    }
+  }
+
+  // Set the flags to indicate which matrices have been initialised.
+  lap_init_ = false;
+  signless_lap_init_ = false;
+  signless_norm_lap_init_ = false;
+  deg_init_ = false;
+  inv_deg_init_ = false;
+  norm_lap_init_ = false;
+  lazy_rand_walk_init_ = false;
+}
+
+bool stag::Graph::has_self_loops() const {
+  return has_self_loops_;
+}
+
+bool stag::Graph::is_connected() {
+  if ((StagInt) stag::connected_component(this, 0).size()
+        == number_of_vertices_) return true;
+  return false;
+}
+
+void stag::Graph::check_vertex_argument(StagInt v) const {
   // Check that the value is smaller than the number of vertices
   if (v >= number_of_vertices_) {
     throw std::invalid_argument("Specified vertex index too large.");
   }
 
   // Check that the specified vertex is not negative
   if (v < 0) {
@@ -128,91 +303,175 @@
   }
 }
 
 //------------------------------------------------------------------------------
 // Local Graph Methods
 //------------------------------------------------------------------------------
 
-std::vector<double> stag::Graph::degrees(std::vector<stag_int> vertices) {
-    std::vector<double> degrees;
+std::vector<StagReal> stag::Graph::degrees(std::vector<StagInt> vertices) {
+    std::vector<StagReal> degrees;
 
-    for (stag_int v : vertices) {
+    for (StagInt v : vertices) {
         degrees.emplace_back(degree(v));
     }
 
     return degrees;
 }
 
-std::vector<stag_int> stag::Graph::degrees_unweighted(
-        std::vector<stag_int> vertices) {
-    std::vector<stag_int> degrees;
+std::vector<StagInt> stag::Graph::degrees_unweighted(
+        std::vector<StagInt> vertices) {
+    std::vector<StagInt> degrees;
 
-    for (stag_int v : vertices) {
+    for (StagInt v : vertices) {
         degrees.emplace_back(degree_unweighted(v));
     }
 
     return degrees;
 }
 
 
-double stag::Graph::degree(stag_int v) {
+StagReal stag::Graph::degree(StagInt v) {
   check_vertex_argument(v);
 
   // For now, we can be a little lazy and use the degree matrix. Once this is
   // initialised, then checking degree is constant time.
   initialise_degree_matrix_();
   return degree_matrix_.coeff(v, v);
 }
 
-stag_int stag::Graph::degree_unweighted(stag_int v) {
+StagInt stag::Graph::degree_unweighted(StagInt v) {
   check_vertex_argument(v);
 
   // The combinatorical degree of a vertex is equal to the number of non-zero
-  // entries in its adjacency matrix row.
-  const stag_int *indexPtr = adjacency_matrix_.outerIndexPtr();
-  stag_int rowStart = *(indexPtr + v);
-  stag_int nextRowStart = *(indexPtr + v + 1);
-  return nextRowStart - rowStart;
+  // entries in its adjacency matrix row, plus 1 if there is a self-loop.
+  const StagInt *indexPtr = adjacency_matrix_.outerIndexPtr();
+  StagInt rowStart = *(indexPtr + v);
+  StagInt nextRowStart = *(indexPtr + v + 1);
+  StagInt self_loop = 0;
+  if (adjacency_matrix_.coeff(v, v) != 0) self_loop = 1;
+
+  return nextRowStart - rowStart + self_loop;
 }
 
-std::vector<stag::edge> stag::Graph::neighbors(stag_int v) {
+std::vector<stag::edge> stag::Graph::neighbors(StagInt v) {
   check_vertex_argument(v);
 
   // Iterate through the non-zero entries in the vth row of the adjacency matrix
-  const double *weights = adjacency_matrix_.valuePtr();
-  const stag_int *innerIndices = adjacency_matrix_.innerIndexPtr();
-  const stag_int *rowStarts = adjacency_matrix_.outerIndexPtr();
-  stag_int vRowStart = *(rowStarts + v);
-  stag_int degree_unw = degree_unweighted(v);
+  const StagReal *weights = adjacency_matrix_.valuePtr();
+  const StagInt *innerIndices = adjacency_matrix_.innerIndexPtr();
+  const StagInt *rowStarts = adjacency_matrix_.outerIndexPtr();
+  StagInt vRowStart = *(rowStarts + v);
+  StagInt degree_unw = degree_unweighted(v);
+
+  // If there is a self-loop, then we have to subtract one from the unweighted
+  // degree.
+  StagInt self_loop = 0;
+  if (adjacency_matrix_.coeff(v, v) != 0) self_loop = 1;
 
   std::vector<stag::edge> edges;
-  for (stag_int i = 0; i < degree_unw; i++) {
+  for (StagInt i = 0; i < degree_unw - self_loop; i++) {
     if (*(weights + vRowStart + i) != 0) {
       edges.push_back({v, *(innerIndices + vRowStart + i), *(weights + vRowStart + i)});
     }
   }
 
   return edges;
 }
 
-std::vector<stag_int> stag::Graph::neighbors_unweighted(stag_int v) {
+std::vector<StagInt> stag::Graph::neighbors_unweighted(StagInt v) {
   check_vertex_argument(v);
 
   // Return the non-zero indices in the vth row of the adjacency matrix
-  const stag_int *innerIndices = adjacency_matrix_.innerIndexPtr();
-  const stag_int *rowStarts = adjacency_matrix_.outerIndexPtr();
-  stag_int vRowStart = *(rowStarts + v);
-  stag_int degree = degree_unweighted(v);
-  return {innerIndices + vRowStart, innerIndices + vRowStart + degree};
+  const StagInt *innerIndices = adjacency_matrix_.innerIndexPtr();
+  const StagInt *rowStarts = adjacency_matrix_.outerIndexPtr();
+  StagInt vRowStart = *(rowStarts + v);
+  StagInt degree = degree_unweighted(v);
+
+  // If there is a self-loop, then we have to subtract one from the unweighted
+  // degree.
+  StagInt self_loop = 0;
+  if (adjacency_matrix_.coeff(v, v) != 0) self_loop = 1;
+
+  return {innerIndices + vRowStart, innerIndices + vRowStart + degree - self_loop};
 }
 
-bool stag::Graph::vertex_exists(stag_int v) {
+bool stag::Graph::vertex_exists(StagInt v) {
   return v >= 0 && v < number_of_vertices_;
 }
 
+stag::Graph stag::Graph::subgraph(std::vector<StagInt>& vertices) {
+  // Convert the vector of vertices to a set, and construct the map from old
+  // vertex ID to the new one.
+  std::unordered_set<StagInt> vertex_set;
+  std::unordered_map<StagInt, StagInt> old_to_new_id;
+  StagInt next_id = 0;
+  for (StagInt v : vertices) {
+    if (!vertex_set.contains(v)) {
+      vertex_set.insert(v);
+      old_to_new_id.insert({v, next_id});
+      next_id++;
+    }
+  }
+
+  // Construct the non-zero entries in the new adjacency matrix
+  std::vector<EdgeTriplet> non_zero_entries;
+  for (StagInt v : vertex_set) {
+    for (stag::edge e : neighbors(v)) {
+      if (e.v2 >= v && vertex_set.contains(e.v2)) {
+        non_zero_entries.emplace_back(
+            old_to_new_id[v], old_to_new_id[e.v2], e.weight);
+
+        // Add the symmetric entry to the adjacency matrix only if this is
+        // not a self-loop.
+        if (e.v2 > v) {
+          non_zero_entries.emplace_back(
+              old_to_new_id[e.v2], old_to_new_id[v], e.weight);
+        }
+      }
+    }
+  }
+
+  // Construct the final adjacency matrix
+  SprsMat adj_mat((StagInt) vertex_set.size(), (StagInt) vertex_set.size());
+  adj_mat.setFromTriplets(non_zero_entries.begin(), non_zero_entries.end());
+  return stag::Graph(adj_mat);
+}
+
+stag::Graph stag::Graph::disjoint_union(Graph& other) {
+  // Get the adjacency matrix data from this graph
+  std::vector<StagReal> values = stag::sprsMatValues(&adjacency_matrix_);
+  std::vector<StagInt> innerIndices = stag::sprsMatInnerIndices(&adjacency_matrix_);
+  std::vector<StagInt> outerStarts = stag::sprsMatOuterStarts(&adjacency_matrix_);
+
+  // Get the adjacency matrix data from the other graph
+  SprsMat other_adj = *other.adjacency();
+  std::vector<StagReal> other_values = stag::sprsMatValues(&other_adj);
+  std::vector<StagInt> other_innerIndices = stag::sprsMatInnerIndices(&other_adj);
+  std::vector<StagInt> other_outerStarts = stag::sprsMatOuterStarts(&other_adj);
+
+  // We will extend the matrix data vectors with the data from the other graph
+  values.reserve(values.size() + distance(other_values.begin(),
+                                          other_values.end()));
+  values.insert(values.end(), other_values.begin(), other_values.end());
+
+  StagInt start_offset = outerStarts.at(outerStarts.size() - 1);
+  for (StagInt other_start : other_outerStarts) {
+    if (other_start != 0) {
+      outerStarts.push_back(other_start + start_offset);
+    }
+  }
+
+  StagInt inner_offset = number_of_vertices_;
+  for (StagInt other_inner : other_innerIndices) {
+    innerIndices.push_back(other_inner + inner_offset);
+  }
+
+  return {outerStarts, innerIndices, values};
+}
+
 //------------------------------------------------------------------------------
 // Graph Object Private Methods
 //------------------------------------------------------------------------------
 
 void stag::Graph::self_test_() {
   // Check that the adjacency matrix is symmetric.
   if (!stag::isSymmetric(&adjacency_matrix_)) {
@@ -259,15 +518,15 @@
 
   // Ensure that the degree matrix is initialised
   initialise_degree_matrix_();
 
   // Construct the inverse degree matrix
   SprsMat sqrt_inv_deg_mat(number_of_vertices_, number_of_vertices_);
   std::vector<EdgeTriplet> non_zero_entries;
-  for (stag_int i = 0; i < number_of_vertices_; i++) {
+  for (StagInt i = 0; i < number_of_vertices_; i++) {
     non_zero_entries.emplace_back(i, i, 1 / sqrt(degree_matrix_.coeff(i, i)));
   }
   sqrt_inv_deg_mat.setFromTriplets(non_zero_entries.begin(), non_zero_entries.end());
 
   // The normalised laplacian is defined by I - D^{-1/2} A D^{-1/2}
   SprsMat identity_matrix(number_of_vertices_, number_of_vertices_);
   identity_matrix.setIdentity();
@@ -285,15 +544,15 @@
 
   // Ensure that the degree matrix is initialised
   initialise_degree_matrix_();
 
   // Construct the inverse degree matrix
   SprsMat sqrt_inv_deg_mat(number_of_vertices_, number_of_vertices_);
   std::vector<EdgeTriplet> non_zero_entries;
-  for (stag_int i = 0; i < number_of_vertices_; i++) {
+  for (StagInt i = 0; i < number_of_vertices_; i++) {
     non_zero_entries.emplace_back(i, i, 1 / sqrt(degree_matrix_.coeff(i, i)));
   }
   sqrt_inv_deg_mat.setFromTriplets(non_zero_entries.begin(), non_zero_entries.end());
 
   // The normalised signless laplacian is defined by I + D^{-1/2} A D^{-1/2}
   SprsMat identity_matrix(number_of_vertices_, number_of_vertices_);
   identity_matrix.setIdentity();
@@ -306,18 +565,20 @@
 
 void stag::Graph::initialise_degree_matrix_() {
   // If the degree matrix has already been initialised, then we do not
   // initialise it again.
   if (deg_init_) return;
 
   // Construct the vertex degrees.
-  Eigen::VectorXd degrees = adjacency_matrix_ * Eigen::VectorXd::Ones(adjacency_matrix_.cols());
+  Eigen::VectorXd simple_degrees = adjacency_matrix_ * Eigen::VectorXd::Ones(adjacency_matrix_.cols());
   degree_matrix_ = SprsMat(adjacency_matrix_.cols(), adjacency_matrix_.cols());
-  for (stag_int i = 0; i < adjacency_matrix_.cols(); i++) {
-    degree_matrix_.insert(i, i) = degrees[i];
+  for (StagInt i = 0; i < adjacency_matrix_.cols(); i++) {
+    // If there is a self-loop on this vertex, then we count its weight twice
+    // for the vertex degree.
+    degree_matrix_.insert(i, i) = simple_degrees[i] + adjacency_matrix_.coeff(i, i);
   }
 
   // Compress the degree matrix storage, and set the initialised flag
   degree_matrix_.makeCompressed();
   deg_init_ = true;
 }
 
@@ -325,15 +586,15 @@
   // If the inverse degree matrix has already been initialised, then we do not
   // initialise it again.
   if (inv_deg_init_) return;
 
   // We will construct the inverse degree matrix from the degree matrix itself
   initialise_degree_matrix_();
   inverse_degree_matrix_ = SprsMat(adjacency_matrix_.cols(), adjacency_matrix_.cols());
-  for (stag_int i = 0; i < adjacency_matrix_.cols(); i++) {
+  for (StagInt i = 0; i < adjacency_matrix_.cols(); i++) {
     inverse_degree_matrix_.insert(i, i) = 1./degree_matrix_.coeff(i, i);
   }
 
   // Compress the degree matrix storage, and set the initialised flag
   inverse_degree_matrix_.makeCompressed();
   inv_deg_init_ = true;
 }
@@ -378,15 +639,15 @@
 bool stag::operator!=(const stag::edge &lhs, const stag::edge &rhs) {
   return !(lhs == rhs);
 }
 
 //------------------------------------------------------------------------------
 // Adjacency List Local Graph
 //------------------------------------------------------------------------------
-stag_int stag::AdjacencyListLocalGraph::goto_next_content_line() {
+StagInt stag::AdjacencyListLocalGraph::goto_next_content_line() {
   std::string current_line;
 
   // Read the current line, discarding it. This leaves the file pointer at the
   // beginning of a line.
   std::streampos current_loc = is_.tellg();
   if (current_loc != 0) stag::safeGetline(is_, current_line);
 
@@ -406,15 +667,15 @@
       stag::safeGetline(is_, current_line);
     }
 
     // Check if this line is a valid content line.
     size_t split_pos = current_line.find(':');
     if (split_pos != std::string::npos) {
       std::string token = current_line.substr(0, split_pos);
-      stag_int source_node_id = std::stoi(token);
+      StagInt source_node_id = std::stoi(token);
 
       // We found a content line, reset the position of the reader to the start
       // of the line and return the node id.
       is_.seekg(current_loc);
       return source_node_id;
     }
   }
@@ -434,28 +695,28 @@
   }
 
   // Get the length of the file in bytes.
   is_.seekg(0, std::ios::end);
   end_of_file_ = is_.tellg();
 }
 
-void stag::AdjacencyListLocalGraph::find_vertex(stag_int v) {
+void stag::AdjacencyListLocalGraph::find_vertex(StagInt v) {
   // Set the maximum and minimum ranges of the file to search
   std::streampos range_min = 0;
   std::streampos range_max = end_of_file_;
 
   // Perform a binary search for the target node
-  stag_int current_id;
+  StagInt current_id;
   bool found_target = false;
   while (!found_target) {
     // If min is greater than max, then we have failed to find our target point
     if (range_min > range_max) throw std::runtime_error("Couldn't find node in adjacencylist file.");
 
     // Search half-way between the search points.
-    stag_int search_point = floor((range_max + range_min) / 2);
+    StagInt search_point = floor((range_max + range_min) / 2);
 
     // Check whether this point has been searched before
     if (fileloc_to_node_id_.find(search_point) != fileloc_to_node_id_.end()) {
       // We have searched this point before
       current_id = fileloc_to_node_id_[search_point];
 
       // If this is the point we're looking for, make sure that the file pointer
@@ -478,15 +739,15 @@
       range_max = search_point - std::streamoff(1);
     } else {
       range_min = search_point + std::streamoff(1);
     }
   }
 }
 
-std::vector<stag::edge> stag::AdjacencyListLocalGraph::neighbors(stag_int v) {
+std::vector<stag::edge> stag::AdjacencyListLocalGraph::neighbors(StagInt v) {
   // If we have searched for this vertex before, just returned the cached copy.
   if (node_id_to_edgelist_.find(v) != node_id_to_edgelist_.end()) {
     return node_id_to_edgelist_[v];
   }
 
   // First, find the target vertex in the adjacencylist file.
   find_vertex(v);
@@ -500,54 +761,56 @@
 
   // Update our internal edgelist.
   node_id_to_edgelist_[v] = edges;
 
   return edges;
 }
 
-std::vector<stag_int> stag::AdjacencyListLocalGraph::neighbors_unweighted(stag_int v) {
+std::vector<StagInt> stag::AdjacencyListLocalGraph::neighbors_unweighted(StagInt v) {
   auto edges = neighbors(v);
-  std::vector<stag_int> unweighted_neighbors;
+  std::vector<StagInt> unweighted_neighbors;
   for (stag::edge e : edges) {
     unweighted_neighbors.push_back(e.v2);
   }
   return unweighted_neighbors;
 }
 
-double stag::AdjacencyListLocalGraph::degree(stag_int v) {
+StagReal stag::AdjacencyListLocalGraph::degree(StagInt v) {
   auto edges = neighbors(v);
-  double deg = 0;
+  StagReal deg = 0;
   for (stag::edge e : edges) {
-    deg += e.weight;
+    // Self-loops count twice towards the degree
+    if (e.v2 == v) deg += 2 * e.weight;
+    else deg += e.weight;
   }
   return deg;
 }
 
-stag_int stag::AdjacencyListLocalGraph::degree_unweighted(stag_int v) {
+StagInt stag::AdjacencyListLocalGraph::degree_unweighted(StagInt v) {
   auto edges = neighbors(v);
   return edges.size();
 }
 
-std::vector<double> stag::AdjacencyListLocalGraph::degrees(std::vector<stag_int> vertices) {
-  std::vector<double> degs;
+std::vector<StagReal> stag::AdjacencyListLocalGraph::degrees(std::vector<StagInt> vertices) {
+  std::vector<StagReal> degs;
   for (auto v : vertices) {
     degs.push_back(degree(v));
   }
   return degs;
 }
 
-std::vector<stag_int> stag::AdjacencyListLocalGraph::degrees_unweighted(std::vector<stag_int> vertices) {
-  std::vector<stag_int> degs;
+std::vector<StagInt> stag::AdjacencyListLocalGraph::degrees_unweighted(std::vector<StagInt> vertices) {
+  std::vector<StagInt> degs;
   for (auto v : vertices) {
     degs.push_back(degree_unweighted(v));
   }
   return degs;
 }
 
-bool stag::AdjacencyListLocalGraph::vertex_exists(stag_int v) {
+bool stag::AdjacencyListLocalGraph::vertex_exists(StagInt v) {
   try {
     find_vertex(v);
     return true;
   } catch (std::runtime_error& e) {
     return false;
   }
 }
@@ -555,51 +818,51 @@
 stag::AdjacencyListLocalGraph::~AdjacencyListLocalGraph() {
   is_.close();
 }
 
 //------------------------------------------------------------------------------
 // Standard Graph Constructors
 //------------------------------------------------------------------------------
-stag::Graph stag::cycle_graph(stag_int n) {
+stag::Graph stag::cycle_graph(StagInt n) {
   if (n < 2) throw std::invalid_argument("Number of vertices must be at least 2.");
 
   SprsMat adj_mat(n, n);
   std::vector<EdgeTriplet> non_zero_entries;
-  for (stag_int i = 0; i < n; i++) {
+  for (StagInt i = 0; i < n; i++) {
     non_zero_entries.emplace_back(i, (i + n + 1) % n, 1);
     non_zero_entries.emplace_back(i, (i + n - 1) % n, 1);
   }
   adj_mat.setFromTriplets(non_zero_entries.begin(), non_zero_entries.end());
   return stag::Graph(adj_mat);
 }
 
-stag::Graph stag::complete_graph(stag_int n) {
+stag::Graph stag::complete_graph(StagInt n) {
   if (n < 2) throw std::invalid_argument("Number of vertices must be at least 2.");
 
   SprsMat adj_mat(n, n);
   std::vector<EdgeTriplet> non_zero_entries;
-  for (stag_int i = 0; i < n; i++) {
-    for (stag_int j = 0; j < n; j++) {
+  for (StagInt i = 0; i < n; i++) {
+    for (StagInt j = 0; j < n; j++) {
       if (i != j) {
         non_zero_entries.emplace_back(i, j, 1);
       }
     }
   }
   adj_mat.setFromTriplets(non_zero_entries.begin(), non_zero_entries.end());
   return stag::Graph(adj_mat);
 }
 
-stag::Graph stag::barbell_graph(stag_int n) {
+stag::Graph stag::barbell_graph(StagInt n) {
   if (n < 2) throw std::invalid_argument("Number of vertices must be at least 2.");
 
   // Construct the non-zero entries in the complete blocks of the adjacency
   // matrix
   std::vector<EdgeTriplet> non_zero_entries;
-  for (stag_int i = 0; i < n; i++) {
-    for (stag_int j = 0; j < n; j++) {
+  for (StagInt i = 0; i < n; i++) {
+    for (StagInt j = 0; j < n; j++) {
       if (i != j) {
         non_zero_entries.emplace_back(i, j, 1);
         non_zero_entries.emplace_back(n + i, n + j, 1);
       }
     }
   }
 
@@ -609,22 +872,40 @@
 
   // Construct the final adjacency matrix
   SprsMat adj_mat(2 * n, 2 * n);
   adj_mat.setFromTriplets(non_zero_entries.begin(), non_zero_entries.end());
   return stag::Graph(adj_mat);
 }
 
-stag::Graph stag::star_graph(stag_int n) {
+stag::Graph stag::star_graph(StagInt n) {
   if (n < 2) throw std::invalid_argument("Number of vertices must be at least 2.");
 
   // Construct the non-zero entries in the adjacency matrix
   std::vector<EdgeTriplet> non_zero_entries;
-  for (stag_int i = 1; i < n; i++) {
+  for (StagInt i = 1; i < n; i++) {
     non_zero_entries.emplace_back(0, i, 1);
     non_zero_entries.emplace_back(i, 0, 1);
   }
 
   // Construct the final adjacency matrix
   SprsMat adj_mat(n, n);
   adj_mat.setFromTriplets(non_zero_entries.begin(), non_zero_entries.end());
   return stag::Graph(adj_mat);
 }
+
+stag::Graph stag::identity_graph(StagInt n) {
+  if (n < 1) throw std::invalid_argument("Number of vertices must be at least 1.");
+
+  SprsMat adj_mat(n, n);
+  adj_mat.setIdentity();
+  return stag::Graph(adj_mat);
+}
+
+//------------------------------------------------------------------------------
+// Other operators
+//------------------------------------------------------------------------------
+stag::Graph stag::operator+(const stag::Graph& lhs, const stag::Graph& rhs) {
+  if (lhs.number_of_vertices() != rhs.number_of_vertices())
+    throw std::invalid_argument("Number of vertices must match.");
+
+  return stag::Graph(*lhs.adjacency() + *rhs.adjacency());
+}
```

### Comparing `stag-1.2.1/stag/stag_lib/graph.h` & `stag-2.0.0/stag/stag_lib/graph.h`

 * *Files 13% similar despite different names*

```diff
@@ -1,83 +1,46 @@
-//
-// Definitions related to the core Graph object used to represent graphs within
-// the library.
-//
-// This file is provided as part of the STAG library and released under the MIT
-// license.
-//
+/*
+   This file is provided as part of the STAG library and released under the GPL
+   license.
+*/
 
 /**
  * @file graph.h
  * \brief Core graph class definitions and constructors.
  */
 
 #ifndef STAG_LIBRARY_H
 #define STAG_LIBRARY_H
 
-#include <Eigen/Sparse>
 #include <vector>
 #include <fstream>
 #include <unordered_map>
 
+#include "definitions.h"
 
-/**
- * The integer type used throughout the library.
- */
-typedef long long stag_int;
-
-/**
- * The fundamental datatype used in this library is the sparse matrix.
- * We use the `Eigen::SparseMatrix` class in column-major format.
- */
-typedef Eigen::SparseMatrix<double, Eigen::ColMajor, stag_int> SprsMat;
-
-/**
- *  Occasionally, it is more efficient to use a dense matrix, such as when
- *  the matrix is very small.
- *
- *  In this case, we use the `Eigen::MatrixXd` class.
- */
-typedef Eigen::MatrixXd DenseMat;
-
-/**
- * An Eigen::Triplet representing an edge in a graph. Stores the row, column, and value
- * of an entry in a graph adjacency matrix.
- */
-typedef Eigen::Triplet<double, stag_int> EdgeTriplet;
-
-/**
- * \cond
- */
-// Redefine the eigen index type to be the same as stag_int
-#undef EIGEN_DEFAULT_DENSE_INDEX_TYPE
-#define EIGEN_DEFAULT_DENSE_INDEX_TYPE stag_int
-/**
- * \endcond
- */
 
 namespace stag {
   /**
    * \brief A structure representing a weighted edge in a graph.
    */
   struct edge {
     /**
      * The first vertex in the edge.
      */
-    stag_int v1;
+    StagInt v1;
 
     /**
      * The second vertex in the edge.
      */
-    stag_int v2;
+    StagInt v2;
 
     /**
      * The weight of the edge.
      */
-    double weight;
+    StagReal weight;
   };
 
   /**
    * \brief An abstract class which defines methods for exploring the
    * local neighborhood of vertices in a graph.
    *
    * To maximise the performance of the local algorithms using this class,
@@ -85,76 +48,79 @@
    * if querying the neighbors of a vertex requires accessing the disk, then
    * the result should be cached.
    */
   class LocalGraph {
     public:
       /**
        * Given a vertex v, return its weighted degree.
+       *
+       * A self-loop of weight \f$1\f$ contributes \f$2\f$ to the vertex's
+       * degree.
        */
-      virtual double degree(stag_int v) = 0;
+      virtual StagReal degree(StagInt v) = 0;
 
       /**
        * Given a vertex v, return its unweighted degree. That is, the number
        * of neighbors of v, ignoring the edge weights.
        */
-      virtual stag_int degree_unweighted(stag_int v) = 0;
+      virtual StagInt degree_unweighted(StagInt v) = 0;
 
       /**
        * Given a vertex v, return a vector of edges representing the
        * neighborhood of v.
        *
        * The returned edges will all have the ordering (v, x) such that
        * edge.v = v.
        *
        * @param v an int representing some vertex in the graph
        * @return an edge vector containing the neighborhood information
        */
-      virtual std::vector<edge> neighbors(stag_int v) = 0;
+      virtual std::vector<edge> neighbors(StagInt v) = 0;
 
       /**
        * Given a vertex v, return a vector containing the neighbors of v.
        *
        * The weights of edges to the neighbors are not returned by this method.
        *
        * @param v an int representing some vertex in the graph
        * @return an int vector giving the neighbors of v
        */
-      virtual std::vector<stag_int> neighbors_unweighted(stag_int v) = 0;
+      virtual std::vector<StagInt> neighbors_unweighted(StagInt v) = 0;
 
       /**
        * Given a list of vertices, return the degrees of each vertex in the
        * list.
        *
        * Providing a method for computing the degrees 'in bulk' increases the
        * efficiency of algorithms on graphs which are not stored directly in
        * memory.
        *
        * @param vertices a vector of ints representing the vertices to be
        *                 queried.
        * @return a vector of degrees
        */
-      virtual std::vector<double> degrees(std::vector<stag_int> vertices) = 0;
+      virtual std::vector<StagReal> degrees(std::vector<StagInt> vertices) = 0;
 
       /**
        * Given a list of vertices, return their unweighted degrees.
        *
        * @param vertices a vector of ints representing the vertices to be
        *                 queried.
        * @return a vector of integer degrees
        */
-      virtual std::vector<stag_int> degrees_unweighted(std::vector<stag_int> vertices) = 0;
+      virtual std::vector<StagInt> degrees_unweighted(std::vector<StagInt> vertices) = 0;
 
       /**
        * Given a vertex ID, returns true or false to indicate whether the vertex exists
        * in the graph.
        *
        * @param v the vertex index to check
        * @return a boolean indicating whether there exists a vertex with the given index
        */
-       virtual bool vertex_exists(stag_int v) = 0;
+       virtual bool vertex_exists(StagInt v) = 0;
 
       /**
        * Destructor for the LocalGraph object.
        */
       virtual ~LocalGraph() = default;
   };
 
@@ -162,30 +128,38 @@
    * \brief The core object used to represent graphs for use with the library.
    *
    * Graphs are always constructed from sparse matrices, and this is the internal
    * representation used as well.
    * Vertices of the graph are always referred to by their unique integer index.
    * This index corresponds to the position of the vertex in the stored adjacency
    * matrix of the graph.
+   *
+   * This class supports graphs with positive edge weights. Self-loops are
+   * permitted.
    */
   class Graph : public LocalGraph {
     public:
       /**
        * Create a graph from an Eigen matrix.
        *
+       * The provided matrix should correspond either to the
+       * adjacency matrix or Laplacian matrix of the graph. STAG will
+       * automatically detect whether the provided matrix is an adjacency matrix
+       * or a Laplacian matrix.
+       *
        * \par Example
        *
        * \code{cpp}
        * #include <iostream>
        * #include <stag/graph.h>
        *
        * int main() {
        *   // Construct a sparse matrix representing the
        *   // triangle graph adjacency matrix.
-       *   stag_int n = 3;
+       *   StagInt n = 3;
        *   SprsMat adj(n, n);
        *   adj.coeffRef(0, 1) = 1;
        *   adj.coeffRef(0, 2) = 1;
        *   adj.coeffRef(1, 0) = 1;
        *   adj.coeffRef(1, 2) = 1;
        *   adj.coeffRef(2, 0) = 1;
        *   adj.coeffRef(2, 1) = 1;
@@ -196,21 +170,22 @@
        *   // Display the adjacency matrix of the graph
        *   std::cout << *myGraph.adjacency() << std::endl;
        *
        *   return 0;
        * }
        * \endcode
        *
-       * The provided adjacency matrix must be symmetric.
+       * The provided matrix must be symmetric, and may include
+       * self-loops.
        *
-       * @param adjacency_matrix the sparse eigen matrix representing the adjacency matrix
-       *               of the graph.
-       * @throws domain_error if the adjacency matrix is not symmetric
+       * @param matrix the sparse eigen matrix representing the adjacency matrix
+       *               or Laplacian matrix of the graph.
+       * @throws domain_error if the provided matrix is not symmetric
        */
-      explicit Graph(const SprsMat& adjacency_matrix);
+      explicit Graph(const SprsMat& matrix);
 
       /**
        * Create a graph from raw arrays describing a CSC sparse matrix.
        *
        * To use this constructor, you should understand the CSC sparse matrix
        * format. Note that this library uses the ColMajor format from the Eigen
        * library.
@@ -219,16 +194,16 @@
        *
        * @param outerStarts the indices of the start of each row in the CSR
        *                    matrix
        * @param innerIndices the column indices of each non-zero element in the
        *                     matrix
        * @param values the values of each non-zero element in the matrix
        */
-      Graph(std::vector<stag_int> &outerStarts, std::vector<stag_int> &innerIndices,
-            std::vector<double> &values);
+      Graph(std::vector<StagInt> &outerStarts, std::vector<StagInt> &innerIndices,
+            std::vector<StagReal> &values);
 
       /**
        * Return the sparse adjacency matrix of the graph.
        *
        * @return a sparse Eigen matrix representing the graph adjacency matrix.
        */
       const SprsMat* adjacency() const;
@@ -345,46 +320,108 @@
       /**
        * The total volume of the graph.
        *
        * The volume is defined as the sum of the node degrees.
        *
        * @return the graph's volume.
        */
-      double total_volume();
+      StagReal total_volume();
 
       /**
        * The average degree of the graph.
        *
        * This is defined as the sum of the node degrees divided by the number of nodes.
        *
        * @return the graph's average degree.
        */
-      double average_degree();
+      StagReal average_degree();
 
       /**
        * The number of vertices in the graph.
        */
-      stag_int number_of_vertices() const;
+      StagInt number_of_vertices() const;
 
       /**
        * The number of edges in the graph.
        *
        * This is defined based on the number of non-zero elements in the
        * adjacency matrix, and ignores the weights of the edges.
        */
-       stag_int number_of_edges() const;
+       StagInt number_of_edges() const;
+
+       /**
+        * Add an edge to the graph.
+        *
+        * The edge goes from node i to node j, and is added with weight w.
+        * If there is already an edge from i to j, then w is added to
+        * its weight.
+        *
+        * If either of \f$i\f$ or \f$j\f$ are larger than the number
+        * of nodes in the graph, the graph is resized to have enough nodes.
+        *
+        * @param i
+        * @param j
+        * @param w
+        */
+       void add_edge(StagInt i, StagInt j, StagReal w);
+
+       /**
+        * Remove an edge from the graph.
+        *
+        * Remove any edge between nodes \f$i\f$ and \f$j\f$.
+        *
+        * @param i
+        * @param j
+        */
+       void remove_edge(StagInt i, StagInt j);
+
+       /**
+        * Returns a boolean indicating whether this graph contains self loops.
+        */
+       bool has_self_loops() const;
+
+       /**
+        * Returns a boolean indicating whether the graph is connected.
+        *
+        * The running time of this method is \f$O(m)\f$, where \f$m\f$ is the
+        * number of edges in the graph.
+        */
+       bool is_connected();
+
+       /**
+        * Construct and return a subgraph of this graph.
+        *
+        * Note that the vertex indices will be changed in the subgraph.
+        *
+        * @param vertices the vertices in the induced subgraph
+        * @return a new stag::Graph object representing the subgraph induced by
+        *         the given vertices
+        */
+       Graph subgraph(std::vector<StagInt>& vertices);
+
+       /**
+        * Construct and return the disjoint union of this graph and another.
+        *
+        * The disjoint union of two graphs \f$G\f$ and \f$H\f$ is a graph
+        * containing \f$G\f$ and \f$H\f$ as disconnected subgraphs.
+        *
+        * @param other the other graph to be combined with this one
+        * @return a new stag::Graph object representing the union of this graph
+        *         with the other one
+        */
+       Graph disjoint_union(Graph& other);
 
        // Override the abstract methods in the LocalGraph base class.
-       double degree(stag_int v) override;
-       stag_int degree_unweighted(stag_int v) override;
-       std::vector<edge> neighbors(stag_int v) override;
-       std::vector<stag_int> neighbors_unweighted(stag_int v) override;
-       std::vector<double> degrees(std::vector<stag_int> vertices) override;
-       std::vector<stag_int> degrees_unweighted(std::vector<stag_int> vertices) override;
-       bool vertex_exists(stag_int v) override;
+       StagReal degree(StagInt v) override;
+       StagInt degree_unweighted(StagInt v) override;
+       std::vector<edge> neighbors(StagInt v) override;
+       std::vector<StagInt> neighbors_unweighted(StagInt v) override;
+       std::vector<StagReal> degrees(std::vector<StagInt> vertices) override;
+       std::vector<StagInt> degrees_unweighted(std::vector<StagInt> vertices) override;
+       bool vertex_exists(StagInt v) override;
        ~Graph() override = default;
 
     private:
       /**
        * Initialise the laplacian matrix of the graph if it has not been
        * initialised yet.
        */
@@ -392,15 +429,15 @@
 
       /**
        * Initialise the signless Laplacian matrix of the graph if it has not been
        * initialised yet.
        */
       void initialise_signless_laplacian_();
 
-    /**
+      /**
        * Initialise the normalised Laplacian matrix of the graph is it has not
        * been initialised yet.
        */
       void initialise_normalised_laplacian_();
 
       /**
        * Initialise the signless Laplacian matrix of the graph if it has not been
@@ -441,28 +478,31 @@
 
       /**
        * Check the validity of a method argument which is supposed to refer
        * to a vertex in the graph.
        *
        * @throws std::invalid_argument if the check does not pass
        */
-       void check_vertex_argument(stag_int v);
+       void check_vertex_argument(StagInt v) const;
 
        /**
         * \endcond
         */
 
       // The number of vertices in the constructed graph.
-      stag_int number_of_vertices_;
+      StagInt number_of_vertices_;
 
       // The ground truth definition of the graph object is the adjacency
       // matrix, stored in a sparse format. The adj_init_ variable is used to
       // indicate whether the matrix has been initialised yet.
       SprsMat adjacency_matrix_;
 
+      // Whether the graph has self loops
+      bool has_self_loops_;
+
       // The laplacian matrix of the graph. The lap_init_ variable is used to
       // indicate whether the matrix has been initialised yet.
       bool lap_init_;
       SprsMat laplacian_matrix_;
 
       // The signless Laplacian matrix of the graph.
       bool signless_lap_init_;
@@ -490,35 +530,14 @@
 
       // The lazy random walk matrix of the graph. The lazy_rand_walk_init_ variable
       // is used to indicate whether the matrix has been initialised yet.
       bool lazy_rand_walk_init_;
       SprsMat lazy_random_walk_matrix_;
   };
 
-  /**
-   * \cond
-   * Do not generate documentation for operator definitions.
-   */
-
-  /**
-   * Define equality for two graphs. Two graphs are equal iff their adjacency
-   * matrices are equal
-   */
-  bool operator==(const Graph& lhs, const Graph& rhs);
-  bool operator!=(const Graph& lhs, const Graph& rhs);
-
-  /**
-   * Define equality for edges.
-   */
-  bool operator==(const edge& lhs, const edge& rhs);
-  bool operator!=(const edge& lhs, const edge& rhs);
-
-  /**
-   * \endcond
-   */
 
   /**
    * \brief A local graph backed by an adjacency list file on disk.
    *
    * The graph is loaded into memory in a local way only. That is, an adjacency
    * list data structure is constructed in memory as node neighbours are queried.
    * If a node is not found in the cached adjacency list, then the neighbours of
@@ -544,95 +563,181 @@
      * use by this object.
      *
      * @param filename the name of the adjacencylist file which defines the graph
      */
     AdjacencyListLocalGraph(const std::string& filename);
 
     // Override the abstract methods in the LocalGraph base class.
-    double degree(stag_int v) override;
-    stag_int degree_unweighted(stag_int v) override;
-    std::vector<edge> neighbors(stag_int v) override;
-    std::vector<stag_int> neighbors_unweighted(stag_int v) override;
-    std::vector<double> degrees(std::vector<stag_int> vertices) override;
-    std::vector<stag_int> degrees_unweighted(std::vector<stag_int> vertices) override;
-    bool vertex_exists(stag_int v) override;
+    StagReal degree(StagInt v) override;
+    StagInt degree_unweighted(StagInt v) override;
+    std::vector<edge> neighbors(StagInt v) override;
+    std::vector<StagInt> neighbors_unweighted(StagInt v) override;
+    std::vector<StagReal> degrees(std::vector<StagInt> vertices) override;
+    std::vector<StagInt> degrees_unweighted(std::vector<StagInt> vertices) override;
+    bool vertex_exists(StagInt v) override;
     ~AdjacencyListLocalGraph() override;
 
   private:
     /**
      * Move the ifstream head to the start of the next content line, and return
      * the ID of the corresponding node.
      *
      * If there is no content line before the end of the file, return -1 and
      * set the ifstream head to the end of the file.
      *
      * @return the node ID of the next content line
      */
-    stag_int goto_next_content_line();
+    StagInt goto_next_content_line();
 
     /**
      * Perform a binary search to find the given vertex in the adjacencylist
      * file.
      *
      * If the vertex v is defined, the input stream pointer will be pointing
      * at the start of the corresponding content line.
      *
      * If the vertex does not exist, will throw a runtime exception.
      *
      * @param v the vertex to search for
      */
-    void find_vertex(stag_int v);
+    void find_vertex(StagInt v);
 
     // The input file stream corresponding to the adjacencylist file backing
     // this graph. The implementation makes random access to this file to
     // read the vertex adjacency information.
     std::ifstream is_;
     std::streampos end_of_file_;
 
     // In order to increase the efficiency of looking up neighbourhood
     // information in the graph, we cache the node ids corresponding to certain
     // locations in the file. The cached locations will correspond to the binary
     // search locations for the nodes we've queried.
-    std::unordered_map<stag_int, stag_int> fileloc_to_node_id_;
+    std::unordered_map<StagInt, StagInt> fileloc_to_node_id_;
 
     // We also store the full adjacency list of the graph queried so far.
-    std::unordered_map<stag_int, std::vector<edge>> node_id_to_edgelist_;
+    std::unordered_map<StagInt, std::vector<edge>> node_id_to_edgelist_;
   };
 
   /**
    * Construct a cycle graph on n vertices.
    *
    * @param n the number of vertices in the constructed graph
    * @return a stag::Graph object representing a cycle graph
    */
-  stag::Graph cycle_graph(stag_int n);
+  stag::Graph cycle_graph(StagInt n);
 
   /**
    * Construct a complete graph on n vertices.
    *
    * @param n the number of vertices in the constructed graph
    * @return a stag::Graph object representing a complete graph
    */
-  stag::Graph complete_graph(stag_int n);
+  stag::Graph complete_graph(StagInt n);
 
   /**
    * Construct a barbell graph. The barbell graph consists of 2 cliques on n
    * vertices, connected by a single edge.
    *
    * @param n the number of vertices in each of the two cliques.
    *          The returned graph will have \f$2n\f$ vertices.
    * @return a stag::Graph object representing the barbell graph
    */
-  stag::Graph barbell_graph(stag_int n);
+  stag::Graph barbell_graph(StagInt n);
 
   /**
    * Construct a star graph. The star graph consists of one central vertex
    * connected by an edge to n-1 outer vertices.
    *
    * @param n the number of vertices in the constructed graph
    * @return a stag::Graph object representing the star graph
    */
-   stag::Graph star_graph(stag_int n);
+   stag::Graph star_graph(StagInt n);
+
+  /**
+   * Construct the 'identity graph'. The identity graph consists of \f$n\f$
+   * vertices, each with a self-loop of weight 1.
+   *
+   * Both the adjacency matrix and Laplacian matrix of the identity graph are
+   * equal to the identity matrix.
+   *
+   * @param n the number of vertices in the constructed graph
+   * @return a stag::Graph object representing the identity graph
+   */
+  stag::Graph identity_graph(StagInt n);
+
+  /**
+   * \cond
+   * Do not generate documentation for operator definitions.
+   */
+
+  /**
+   * Define equality for two graphs. Two graphs are equal iff their adjacency
+   * matrices are equal
+   */
+  bool operator==(const Graph& lhs, const Graph& rhs);
+  bool operator!=(const Graph& lhs, const Graph& rhs);
+
+  /**
+   * Define equality for edges.
+   */
+  bool operator==(const edge& lhs, const edge& rhs);
+  bool operator!=(const edge& lhs, const edge& rhs);
+
+  /**
+   * \endcond
+   */
 
+  /**
+   * Multiplying a graph by a scalar is equivalent to multiplying the weight
+   * of each edge by the given value.
+   *
+   * For example, the following code creates a complete graph with edges of
+   * weight 2.
+   *
+   * \code{.cpp}
+   *     #include <stag/graph.h>
+   *
+   *     int main() {
+   *       stag::Graph myGraph = 2 * stag::complete_graph(10);
+   *
+   *       return 0;
+   *     }
+   * \endcode
+   *
+   */
+  template <typename Scalar>
+  stag::Graph operator*(Scalar lhs, const stag::Graph& rhs) {
+    const SprsMat new_adj = lhs * *rhs.adjacency();
+    return stag::Graph(new_adj);
+  }
+
+  /**
+   * \overload
+   */
+  template <typename Scalar>
+  stag::Graph operator*(const stag::Graph& lhs, Scalar rhs) {
+    const SprsMat new_adj = rhs * *lhs.adjacency();
+    return stag::Graph(new_adj);
+  }
+
+  /**
+   * Adding two graphs is equivalent to adding their adjacency matrices.
+   *
+   * The graphs must have the same number of vertices. For example, the following
+   * code adds a complete graph and a cycle graph on \f$5\f$ vertices.
+   *
+   * \code{.cpp}
+   *    #include <stag/graph.h>
+   *
+   *    int main() {
+   *        stag::Graph myGraph = stag::complete_graph(5) + stag::cycle_graph(5);
+   *
+   *        return 0;
+   *    }
+   * \endcode
+   *
+   * @throws std::invalud_argument if the graphs have different sizes.
+   */
+  stag::Graph operator+(const stag::Graph& lhs, const stag::Graph& rhs);
 }
-#endif //STAG_LIBRARY_H
 
+#endif //STAG_LIBRARY_H
```

### Comparing `stag-1.2.1/stag/stag_lib/graphio.cpp` & `stag-2.0.0/stag/stag_lib/graphio.cpp`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-//
-// This file is provided as part of the STAG library and released under the MIT
-// license.
-//
+/*
+   This file is provided as part of the STAG library and released under the GPL
+   license.
+*/
 #include <iostream>
 #include <fstream>
 #include <stdexcept>
 #include <filesystem>
 
 #include "graph.h"
 #include "utility.h"
@@ -22,18 +22,18 @@
 stag::edge parse_edgelist_content_line(std::string line) {
   // List the possible delimiters for the elements on the line
   std::vector<std::string> delimiters{",", " ", "\t"};
 
   // Split the line to extract the edge information
   // The weight defaults to 1 if it is not otherwise updated by the information
   // in the line.
-  int num_tokens_found = 0;
-  int u = -1;
-  int v = -1;
-  double weight = 1;
+  StagUInt num_tokens_found = 0;
+  StagInt u = -1;
+  StagInt v = -1;
+  StagReal weight = 1;
 
   // Try splitting by each delimiter in turn
   size_t split_pos = 0;
   std::string token;
   for (const std::string &delimiter: delimiters) {
     // If we have not found any delimiters of the previous types yet,
     // then try this one.
@@ -97,15 +97,15 @@
   }
 
   // We will construct a vector of triples in order to construct the final
   // adjacency matrix
   std::vector<EdgeTriplet> non_zero_entries;
 
   // Read the file in one line at a time
-  stag_int number_of_vertices = 0;
+  StagInt number_of_vertices = 0;
   std::string line;
   stag::edge this_edge;
   while (stag::safeGetline(is, line)) {
     if (line[0] != '#' && line[0] != '/' && line.length() > 0) {
       try {
         // This line of the input file isn't a comment, parse it.
         this_edge = parse_edgelist_content_line(line);
@@ -214,16 +214,16 @@
 
 /**
  * Get the number of lines and maximum ID in an edgelist file.
  *
  * This has running time O(n) where n is the number of lines in the edgelist
  * file.
  */
-void get_edgelist_lines_and_nodes(std::string& filename, stag_int& lines,
-                                  stag_int& max_id) {
+void get_edgelist_lines_and_nodes(std::string& filename, StagInt& lines,
+                                  StagInt& max_id) {
   // Open the input file
   std::ifstream is(filename);
   if (!is.is_open()) {
     throw std::runtime_error(std::strerror(errno));
   }
 
   // Find the number of lines and the maximum node ID in the edgelist file
@@ -256,24 +256,24 @@
 }
 
 /**
  * A structure representing an interval for the quicksort algorithm for edgelist
  * files.
  */
 struct EdgelistSortInterval {
-  stag_int start_line;
-  stag_int end_line;
-  stag_int min_id;
-  stag_int max_id;
+  StagInt start_line;
+  StagInt end_line;
+  StagInt min_id;
+  StagInt max_id;
 };
 
 void stag::sort_edgelist(std::string &filename) {
   // Find the number of lines and the maximum node ID in the edgelist file
-  stag_int max_id = 0;
-  stag_int num_lines = 0;
+  StagInt max_id = 0;
+  StagInt num_lines = 0;
   get_edgelist_lines_and_nodes(filename, num_lines, max_id);
 
   // Initialise the vector of quicksort intervals
   std::vector<EdgelistSortInterval> intervals;
   intervals.push_back({0, num_lines - 1, 0, max_id});
 
   // Iterate the quicksort algorithm until there are no intervals left.
@@ -285,46 +285,46 @@
 
     // Open the edgelist file as input
     std::ifstream ifs(filename);
     if (!ifs.is_open()) throw std::runtime_error(std::strerror(errno));
 
     // Throughout the algorithm, we must maintain a record of which line of the
     // input and output file we are pointing at.
-    stag_int current_input_line = 0;
-    stag_int current_output_line = 0;
+    StagInt current_input_line = 0;
+    StagInt current_output_line = 0;
 
     // For each pass through the input file, output any header comment lines
     // verbatim
     bool written_content = false;
 
     // For each interval, we will iterate over that portion of the input file
     // twice.
     std::string line;
     stag::edge this_edge;
     std::vector<EdgelistSortInterval> new_intervals;
     for (EdgelistSortInterval interval : intervals) {
       // The pivot index is half-way between the max and min.
-      stag_int double_pivot = interval.min_id + interval.max_id;
+      StagInt double_pivot = interval.min_id + interval.max_id;
       assert(double_pivot > 2 * interval.min_id);
       assert(double_pivot < 2 * interval.max_id);
 
       // First iteration: looking for edges with node_ids less than the pivot
       while (current_input_line < interval.start_line) {
         // Write out every line up to the start point.
         stag::safeGetline(ifs, line);
         os << line << std::endl;
         current_output_line++;
         current_input_line++;
       }
       std::streampos start_loc = ifs.tellg();
       assert(current_input_line == interval.start_line);
 
-      stag_int new_interval_start = current_output_line;
-      stag_int new_interval_min_id = interval.max_id;
-      stag_int new_interval_max_id = interval.min_id;
+      StagInt new_interval_start = current_output_line;
+      StagInt new_interval_min_id = interval.max_id;
+      StagInt new_interval_max_id = interval.min_id;
 
       while (current_input_line < interval.end_line) {
         stag::safeGetline(ifs, line);
         current_input_line++;
 
         if (line[0] != '#' && line[0] != '/' && line.length() > 0) {
           try {
@@ -349,15 +349,15 @@
             os << line << std::endl;
             current_output_line++;
           }
         }
       }
 
       assert(new_interval_max_id >= new_interval_min_id);
-      stag_int new_interval_end = current_output_line;
+      StagInt new_interval_end = current_output_line;
       if (new_interval_end - new_interval_start > 1 &&
           new_interval_max_id > new_interval_min_id) {
         new_intervals.push_back({new_interval_start,
                                  new_interval_end,
                                  new_interval_min_id,
                                  new_interval_max_id});
       }
@@ -428,17 +428,17 @@
   }
 }
 
 //------------------------------------------------------------------------------
 // Adjacency List processing
 //------------------------------------------------------------------------------
 
-stag::edge parse_adjacencylist_edge(std::string token, stag_int source_node) {
-  stag_int neighbour;
-  double weight;
+stag::edge parse_adjacencylist_edge(std::string token, StagInt source_node) {
+  StagInt neighbour;
+  StagReal weight;
 
   // Try to split on ':' to get a weight
   size_t split_pos = token.find(':');
   if (split_pos == std::string::npos) {
     // There is no colon, so the entire token should be parseable as an integer
     // and this is an edge with weight 1.
     neighbour = std::stoi(token);
@@ -466,15 +466,15 @@
 
   // Begin by finding the ID of the node at the start of the line
   size_t split_pos = line.find(':');
   if (split_pos == std::string::npos) {
     throw std::invalid_argument("Couldn't extract ID on adjacencylist line.");
   }
   std::string token = line.substr(0, split_pos);
-  stag_int source_node_id = std::stoi(token);
+  StagInt source_node_id = std::stoi(token);
   line.erase(0, split_pos + 1);
 
   // Now, repeatedly split the rest of the line on spaces to find the neighbours.
   while ((split_pos = line.find(' ')) != std::string::npos) {
     token = line.substr(0, split_pos);
     line.erase(0, split_pos + 1);
     if (token.length() == 0) continue;
@@ -508,15 +508,15 @@
   }
 
   // We will construct a vector of triples in order to construct the final
   // adjacency matrix
   std::vector<EdgeTriplet> non_zero_entries;
 
   // Read the file in one line at a time
-  stag_int number_of_vertices = 0;
+  StagInt number_of_vertices = 0;
   std::string line;
   std::vector<stag::edge> neighbours;
   while (stag::safeGetline(is, line)) {
     if (line[0] != '#' && line[0] != '/' && line.length() > 0) {
       try {
         // This line of the input file isn't a comment, parse it.
         neighbours = stag::parse_adjacencylist_content_line(line);
@@ -565,15 +565,15 @@
   os << "#" << std::endl;
   os << "# This file is formatted as a STAG adjacency list. For more information," << std::endl;
   os << "# see the STAG documentation." << std::endl;
   os << "#" << std::endl;
 
   // Iterate through the nodes in the graph, and write
   // the adjacencylist file
-  for (stag_int node = 0; node < graph.number_of_vertices(); node++) {
+  for (StagInt node = 0; node < graph.number_of_vertices(); node++) {
     os << node << ":";
 
     for (stag::edge e: graph.neighbors(node)) {
       os << " " << e.v2 << ":" << e.weight;
     }
 
     os << std::endl;
@@ -640,15 +640,15 @@
   std::ofstream os(adjacencylist_fname);
 
   // We will include any comments up until the first content line.
   // This preserves 'header' information as a comment.
   bool written_content = false;
 
   // Iterate through the edgelist file
-  stag_int current_node = -1;
+  StagInt current_node = -1;
   std::string line;
   while (stag::safeGetline(is, line)) {
     if (line[0] != '#' && line[0] != '/' && line.length() > 0) {
       try {
         // This line of the input file isn't a comment, parse it.
         stag::edge this_edge = parse_edgelist_content_line(line);
         written_content = true;
```

### Comparing `stag-1.2.1/stag/stag_lib/graphio.h` & `stag-2.0.0/stag/stag_lib/graphio.h`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,26 @@
-//
-// This file is provided as part of the STAG library and released under the MIT
-// license.
-//
+/*
+   This file is provided as part of the STAG library and released under the GPL
+   license.
+*/
 
 /**
  * @file graphio.h
  * \brief Methods for reading and writing graphs to disk.
  *
  * For an introduction to the file formats supported by STAG, see
  * [Graph File Formats](@ref file-formats).
  */
 
 #ifndef STAG_TEST_GRAPHIO_H
 #define STAG_TEST_GRAPHIO_H
 
 #include <string>
 
-#include <graph.h>
+#include "graph.h"
 
 namespace stag {
   /**
    * Load a graph from an edgelist file.
    *
    * We define an edgelist file in the following way.
    *   - Any lines beginning with '#' or '//' are ignored
```

### Comparing `stag-1.2.1/stag/stag_lib/random.cpp` & `stag-2.0.0/stag/stag_lib/random.cpp`

 * *Files 8% similar despite different names*

```diff
@@ -1,57 +1,69 @@
-//
-// This file is provided as part of the STAG library and released under the MIT
-// license.
-//
-#include <random>
+/*
+   This file is provided as part of the STAG library and released under the GPL
+   license.
+*/
 #include <iostream>
 
 #include "random.h"
 #include "graph.h"
 
+std::random_device dev_g;
+std::mt19937_64 rng_g(dev_g());
+
+std::mt19937_64* stag::get_global_rng() {
+  return &rng_g;
+}
+
+std::mt19937_64 stag::create_rng() {
+  std::random_device local_dev;
+  std::mt19937_64 local_rng(local_dev());
+  return local_rng;
+}
+
 /**
  * Get an upper estimate on the number of neighbours of each node in a
  * graph generated from the stochastic block model.
  *
  * This will be used to pre-allocate the memory of the adjacency matrix as we
  * construct the graph.
  *
  * @param cluster_sizes a vector of length \f$k\f$ with the number of vertices
  *                      in each cluster.
  * @param probabilities a \f$k \times k\f$ matrix with the inter-cluster
  *                      probabilities.
  * @return an Eigen vector with the neighbour estimates.
  */
-Eigen::VectorXi estimate_sbm_neighbours(std::vector<stag_int>& cluster_sizes,
+Eigen::VectorXi estimate_sbm_neighbours(std::vector<StagInt>& cluster_sizes,
                                         DenseMat probabilities) {
   // Get the total number of vertices in the graph
-  auto k = (stag_int) cluster_sizes.size();
-  stag_int n = 0;
-  for (stag_int s : cluster_sizes) n += s;
+  auto k = (StagInt) cluster_sizes.size();
+  StagInt n = 0;
+  for (StagInt s : cluster_sizes) n += s;
 
   // Create the vector which we'll return
   Eigen::VectorXi neighbours(n);
 
   // Compute the expected number of neighbours for a node in each cluster
   // This is basically the matrix product of probabilities with cluster_sizes
   Eigen::VectorXi cluster_neighbours(k);
   for (auto i = 0; i < k; i++) {
-    stag_int this_cluster_neighbours = 0;
+    StagInt this_cluster_neighbours = 0;
     for (auto j = 0; j < k; j++) {
       this_cluster_neighbours += cluster_sizes.at(j) * probabilities(i, j);
     }
 
     // Add a safety factor of 2
     cluster_neighbours.coeffRef(i) = 2 * this_cluster_neighbours;
   }
 
   // Now add the neighbour estimates for each actual node
-  stag_int current_idx = 0;
-  for (stag_int i = 0; i < k; i++) {
-    for (stag_int j = 0; j < cluster_sizes.at(i); j++) {
+  StagInt current_idx = 0;
+  for (StagInt i = 0; i < k; i++) {
+    for (StagInt j = 0; j < cluster_sizes.at(i); j++) {
       neighbours.coeffRef(current_idx) = cluster_neighbours(i);
       current_idx++;
     }
   }
 
   return neighbours;
 }
@@ -69,35 +81,36 @@
  * @param other_cluster_vertices the number of vertices in the 'target' cluster
  * @param this_cluster_start_idx the index of the first vertex in the 'source' cluster
  * @param other_cluster_start_idx the index of the first vertex in the 'target' cluster
  * @param p the probability of including each edge.
  */
 void sample_edges_directly(SprsMat* adj_mat,
                            std::ostream* edgelist_os,
-                           stag_int cluster_idx,
-                           stag_int other_cluster_idx,
-                           stag_int this_cluster_vertices,
-                           stag_int other_cluster_vertices,
-                           stag_int this_cluster_start_idx,
-                           stag_int other_cluster_start_idx,
-                           double p) {
+                           StagInt cluster_idx,
+                           StagInt other_cluster_idx,
+                           StagInt this_cluster_vertices,
+                           StagInt other_cluster_vertices,
+                           StagInt this_cluster_start_idx,
+                           StagInt other_cluster_start_idx,
+                           StagReal p) {
+  // Validate the function inputs
+  assert(0 <= p && p <= 1);
+
   // Prepare the random number generator
-  std::random_device dev;
-  std::mt19937 prng(dev());
   std::bernoulli_distribution sampleDist(p);
 
-  for (stag_int i = this_cluster_start_idx;
+  for (StagInt i = this_cluster_start_idx;
       i < this_cluster_start_idx + this_cluster_vertices; i++) {
-    for (stag_int j = other_cluster_start_idx;
+    for (StagInt j = other_cluster_start_idx;
         j < other_cluster_start_idx + other_cluster_vertices; j++) {
       // If we are in the same cluster, then don't double sample
       if (cluster_idx == other_cluster_idx && j <= i) continue;
 
       // Toss a coin
-      if (sampleDist(prng)) {
+      if (sampleDist(*stag::get_global_rng())) {
         if (adj_mat != nullptr) {
           adj_mat->insert(i, j) = 1;
           adj_mat->insert(j, i) = 1;
         }
         if (edgelist_os != nullptr) {
           *edgelist_os << i << " " << j << " " << 1 << std::endl;
         }
@@ -116,111 +129,109 @@
  * @param other_cluster_vertices the number of vertices in the 'target' cluster
  * @param this_cluster_start_idx the index of the first vertex in the 'source' cluster
  * @param other_cluster_start_idx the index of the first vertex in the 'target' cluster
  * @param p
  */
 void sample_edges_binomial(SprsMat* adj_mat,
                            std::ostream* edgelist_os,
-                           stag_int this_cluster_vertices,
-                           stag_int other_cluster_vertices,
-                           stag_int this_cluster_start_idx,
-                           stag_int other_cluster_start_idx,
-                           double p) {
+                           StagInt this_cluster_vertices,
+                           StagInt other_cluster_vertices,
+                           StagInt this_cluster_start_idx,
+                           StagInt other_cluster_start_idx,
+                           StagReal p) {
   // Validate the function inputs
   assert(0 <= p && p <= 1);
 
   // Get the total number of possible edges and the expected number of edges
-  stag_int max_edges = this_cluster_vertices * other_cluster_vertices;
+  StagInt max_edges = this_cluster_vertices * other_cluster_vertices;
   if (this_cluster_start_idx == other_cluster_start_idx) max_edges /= 2;
-  double expected_num_edges = p * ((double) max_edges);
+  StagReal expected_num_edges = p * ((StagReal) max_edges);
 
   // If the exppected number of edges is 0, don't do anything
   if (expected_num_edges < 1) {
     return;
   }
 
   // Prepare the random number generator. We will approximate the binomial
   // distribution with the normal distribution
-  std::random_device dev;
-  std::mt19937 prng(dev());
   assert(sqrt(1 - p) * expected_num_edges > 0);
-  std::normal_distribution<double> numEdgesDist(expected_num_edges,
-                                                sqrt((1 - p) * expected_num_edges));
-  std::uniform_int_distribution<stag_int> thisVertexDist(0, this_cluster_vertices - 1);
-  std::uniform_int_distribution<stag_int> otherVertexDist(0, other_cluster_vertices - 1);
+  std::normal_distribution<StagReal> numEdgesDist(expected_num_edges,
+                                                  sqrt((1 - p) * expected_num_edges));
+  std::uniform_int_distribution<StagInt> thisVertexDist(0, this_cluster_vertices - 1);
+  std::uniform_int_distribution<StagInt> otherVertexDist(0, other_cluster_vertices - 1);
 
   // Decide how many edges to sample based on the 'binomial' distribution
-  auto raw_sample = (stag_int) floor(numEdgesDist(prng));
-  stag_int numEdges = std::max((stag_int) 0, std::min(max_edges, raw_sample));
+  auto raw_sample = (StagInt) floor(numEdgesDist(*stag::get_global_rng()));
+  StagInt numEdges = std::max((StagInt) 0, std::min(max_edges, raw_sample));
 
   // Sample the specific vertices
-  stag_int randU = 0;
-  stag_int randV = 0;
-  for (stag_int i = 0; i < numEdges; i++) {
+  StagInt randU = 0;
+  StagInt randV = 0;
+  for (StagInt i = 0; i < numEdges; i++) {
     // Choose two random vertices in the cluster
     randU = 0;
     randV = 0;
     while (randU == randV) {
       // Ignore the edge if u and v are identical
-      randU = this_cluster_start_idx + thisVertexDist(prng);
-      randV = other_cluster_start_idx + otherVertexDist(prng);
+      randU = this_cluster_start_idx + thisVertexDist(*stag::get_global_rng());
+      randV = other_cluster_start_idx + otherVertexDist(*stag::get_global_rng());
     }
 
     // Add this vertex to the adjacency matrix
     if (adj_mat != nullptr) {
       adj_mat->coeffRef(randU, randV)++;
       adj_mat->coeffRef(randV, randU)++;
     }
     if (edgelist_os != nullptr) {
       *edgelist_os << randU << " " << randV << " " << 1 << std::endl;
     }
   }
 }
 
-stag::Graph stag::sbm(stag_int n, stag_int k, double p, double q) {
+stag::Graph stag::sbm(StagInt n, StagInt k, StagReal p, StagReal q) {
   return stag::sbm(n, k, p, q, false);
 }
 
-stag::Graph stag::sbm(stag_int n, stag_int k, double p, double q, bool exact) {
+stag::Graph stag::sbm(StagInt n, StagInt k, StagReal p, StagReal q, bool exact) {
   if (n < 1) throw std::invalid_argument("Number of vertices must be at least 1.");
   if (k < 1 || k > n/2) {
     throw std::invalid_argument("Number of clusters must be between 1 and n/2.");
   }
   if (p < 0 || p > 1) {
     throw std::invalid_argument("p must be between 0 and 1.");
   }
   if (q < 0 || q > 1) {
     throw std::invalid_argument("q must be between 0 and 1.");
   }
 
   // Create the cluster size vector and probabilities matrix
-  std::vector<stag_int> cluster_sizes;
+  std::vector<StagInt> cluster_sizes;
   DenseMat probabilities(k, k);
   for (auto i = 0; i < k; i++) {
-    cluster_sizes.push_back(floor(((double) n) / ((double) k)));
+    cluster_sizes.push_back(floor(((StagReal) n) / ((StagReal) k)));
     probabilities(i, i) = p;
 
     for (auto j = i + 1; j < k; j++) {
       probabilities(i, j) = q;
       probabilities(j, i) = q;
     }
   }
 
   return general_sbm(cluster_sizes, probabilities, exact);
 }
 
 void general_sbm_internal(SprsMat* adj_mat,
                           std::ostream* edgelist_os,
-                          std::vector<stag_int>& cluster_sizes,
+                          std::vector<StagInt>& cluster_sizes,
                           DenseMat& probabilities, bool exact) {
   // The number of clusters is the length of the cluster_sizes vector
-  stag_int k = cluster_sizes.size();
+  StagInt k = cluster_sizes.size();
 
   // Check that the input parameters make sense.
-  for (stag_int size : cluster_sizes) {
+  for (StagInt size : cluster_sizes) {
     if (size < 1) throw std::invalid_argument("Number of vertices in each cluster must be at least 1.");
   }
   if (probabilities.rows() != k || probabilities.cols() != k) {
     throw std::invalid_argument("Probability matrix must be of size k * k.");
   }
   for (auto i = 0; i < k; i++) {
     for (auto j = 0; j < k; j++) {
@@ -235,27 +246,27 @@
   if (adj_mat != nullptr) {
     Eigen::VectorXi neighbour_estimates = estimate_sbm_neighbours(cluster_sizes,
                                                                   probabilities);
     adj_mat->reserve(neighbour_estimates);
   }
 
   // Iterate through the clusters
-  stag_int this_cluster_start_idx = 0;
-  for (stag_int cluster_idx = 0; cluster_idx < k; cluster_idx++) {
+  StagInt this_cluster_start_idx = 0;
+  for (StagInt cluster_idx = 0; cluster_idx < k; cluster_idx++) {
     // Get the number of vertices in the current cluster
-    stag_int this_cluster_vertices = cluster_sizes.at(cluster_idx);
+    StagInt this_cluster_vertices = cluster_sizes.at(cluster_idx);
 
-    stag_int other_cluster_start_idx = this_cluster_start_idx;
-    for (stag_int other_cluster_idx = cluster_idx;
+    StagInt other_cluster_start_idx = this_cluster_start_idx;
+    for (StagInt other_cluster_idx = cluster_idx;
          other_cluster_idx < k; other_cluster_idx++){
       // Get the number of vertices in the other cluster
-      stag_int other_cluster_vertices = cluster_sizes.at(other_cluster_idx);
+      StagInt other_cluster_vertices = cluster_sizes.at(other_cluster_idx);
 
       // Get the sampling probability between the two clusters
-      double prob = probabilities(cluster_idx, other_cluster_idx);
+      StagReal prob = probabilities(cluster_idx, other_cluster_idx);
 
       // Sample the edges between this cluster and the other cluster
       if (this_cluster_vertices * other_cluster_vertices >= 10000 &&
             prob < 0.5 && !exact) {
         // For small probabilities, use the 'binomial trick' for sampling
         sample_edges_binomial(adj_mat,
                               edgelist_os,
@@ -285,69 +296,69 @@
     this_cluster_start_idx += this_cluster_vertices;
   }
 
   // Finally, construct and return the graph.
   if (adj_mat != nullptr) adj_mat->makeCompressed();
 }
 
-stag::Graph stag::general_sbm(std::vector<stag_int> &cluster_sizes,
+stag::Graph stag::general_sbm(std::vector<StagInt> &cluster_sizes,
                               DenseMat &probabilities, bool exact) {
-  stag_int n = 0;
+  StagInt n = 0;
   for (auto s : cluster_sizes) n += s;
 
   // Initialise a sparse adjacency matrix, and use a null pointer for the
   // edgelist file. This ensures that the general_sbm_internal method
   // writes the generated graph to the adjacency matrix and does not write
   // the graph to disk.
   SprsMat adj_mat(n, n);
   std::ostream* edgelist_os = nullptr;
 
   general_sbm_internal(&adj_mat, edgelist_os, cluster_sizes,
                        probabilities, exact);
   return stag::Graph(adj_mat);
 }
 
-stag::Graph stag::general_sbm(std::vector<stag_int>& cluster_sizes,
+stag::Graph stag::general_sbm(std::vector<StagInt>& cluster_sizes,
                               DenseMat& probabilities) {
   return stag::general_sbm(cluster_sizes, probabilities, false);
 }
 
-stag::Graph stag::erdos_renyi(stag_int n, double p) {
+stag::Graph stag::erdos_renyi(StagInt n, StagReal p) {
   return stag::erdos_renyi(n, p, false);
 }
 
-stag::Graph stag::erdos_renyi(stag_int n, double p, bool exact) {
+stag::Graph stag::erdos_renyi(StagInt n, StagReal p, bool exact) {
   return stag::sbm(n, 1, p, 0, exact);
 }
 
 void stag::general_sbm_edgelist(std::string &filename,
-                                std::vector<stag_int> &cluster_sizes,
+                                std::vector<StagInt> &cluster_sizes,
                                 DenseMat &probabilities,
                                 bool exact) {
   SprsMat* adj_mat = nullptr;
   std::ofstream os(filename);
 
   // If the file could not be opened, throw an exception
   if (!os.is_open()) {
     throw std::runtime_error(std::strerror(errno));
   }
 
   // Write a header to the output stream giving the parameters of the
   // SBM model.
-  stag_int k = cluster_sizes.size();
-  stag_int n = 0;
+  StagInt k = cluster_sizes.size();
+  StagInt n = 0;
   for (auto size: cluster_sizes) n += size;
   os << "# This graph was generated from a stochastic block model with the ";
   os << "following parameters." << std::endl;
   os << "#    n = " << n << std::endl;
   os << "#    k = " << k << std::endl;
 
   if (k <= 20) {
     os << "#    cluster sizes = ";
-    for (stag_int size : cluster_sizes) os << size << " ";
+    for (StagInt size : cluster_sizes) os << size << " ";
     os << std::endl;
     os << "#    probability matrix = " << std::endl;
     for (auto i = 0; i < k; i++) {
       os << "#        ";
       for (auto j = 0; j < k; j++) {
         os << probabilities.coeffRef(i, j) << " ";
       }
@@ -361,42 +372,42 @@
   general_sbm_internal(adj_mat, &os, cluster_sizes, probabilities, exact);
 
   // Close the file output stream.
   os.close();
 }
 
 void stag::general_sbm_edgelist(std::string &filename,
-                                std::vector<stag_int> &cluster_sizes,
+                                std::vector<StagInt> &cluster_sizes,
                                 DenseMat &probabilities) {
   stag::general_sbm_edgelist(filename, cluster_sizes, probabilities, false);
 }
 
-std::vector<stag_int> stag::sbm_gt_labels(stag_int n, stag_int k) {
+std::vector<StagInt> stag::sbm_gt_labels(StagInt n, StagInt k) {
   if (n < 1) throw std::invalid_argument("Number of vertices must be at least 1.");
   if (k < 1 || k > n/2) {
     throw std::invalid_argument("Number of clusters must be between 1 and n/2.");
   }
 
   // Create the cluster size vector
-  std::vector<stag_int> cluster_sizes;
+  std::vector<StagInt> cluster_sizes;
   for (auto i = 0; i < k; i++) {
-    cluster_sizes.push_back(floor(((double) n) / ((double) k)));
+    cluster_sizes.push_back(floor(((StagReal) n) / ((StagReal) k)));
   }
 
   return general_sbm_gt_labels(cluster_sizes);
 }
 
-std::vector<stag_int> stag::general_sbm_gt_labels(std::vector<stag_int>& cluster_sizes) {
-  for (stag_int size : cluster_sizes) {
+std::vector<StagInt> stag::general_sbm_gt_labels(std::vector<StagInt>& cluster_sizes) {
+  for (StagInt size : cluster_sizes) {
     if (size < 1) throw std::invalid_argument("Number of vertices in each cluster must be at least 1.");
   }
 
-  std::vector<stag_int> labels;
+  std::vector<StagInt> labels;
 
-  stag_int current_cluster = 0;
+  StagInt current_cluster = 0;
   for (auto this_size : cluster_sizes) {
     for (auto j = 0; j < this_size; j++) {
       labels.push_back(current_cluster);
     }
     current_cluster++;
   }
```

### Comparing `stag-1.2.1/stag/stag_lib/random.h` & `stag-2.0.0/stag/stag_lib/random.h`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,41 @@
-//
-// Methods for generating graphs from random models.
-//
-// This file is provided as part of the STAG library and released under the MIT
-// license.
-//
+/*
+   This file is provided as part of the STAG library and released under the GPL
+   license.
+*/
 
 /**
  * @file random.h
  * \brief Methods for generating graphs from random graph models
  */
 
 #ifndef STAG_TEST_RANDOM_H
 #define STAG_TEST_RANDOM_H
 
+#include <random>
 #include "graph.h"
 
 namespace stag {
+
+  /**
+   * \cond
+   * Get the random number generator that is common to the main thread of the
+   * program.
+   */
+  std::mt19937_64* get_global_rng();
+
+  /**
+   * Create a random number generator, for example, for use within sub-threads
+   * of the main program.
+   */
+  std::mt19937_64 create_rng();
+  /**
+   * \endcond
+   */
+
   /**
    * Generate a graph from the symmetric stochastic block model.
    *
    * Generates a graph with \f$n\f$ vertices, divided into \f$k\f$ evenly-sized
    * clusters.
    * For each pair of vertices \f$u\f$ and \f$v\f$, the probability of including
    * the edge \f$\{u, v\}\f$ in the graph is
@@ -41,20 +57,20 @@
    * @param n the number of vertices in the graph
    * @param k the number of clusters; vertices are split evenly between clusters
    * @param p the probability of including each edge inside a cluster
    * @param q the probability of including each edge between two clusters
    * @param exact (optional) whether to use the exact probability distribution. Default: false.
    * @return the randomly generated graph
    */
-  Graph sbm(stag_int n, stag_int k, double p, double q, bool exact);
+  Graph sbm(StagInt n, StagInt k, StagReal p, StagReal q, bool exact);
 
   /**
    * @overload
    */
-  Graph sbm(stag_int n, stag_int k, double p, double q);
+  Graph sbm(StagInt n, StagInt k, StagReal p, StagReal q);
 
   /**
    * Generate a graph from the general stochastic block model.
    *
    * The `cluster_sizes` vector specifies the number of vertices in each
    * generated cluster.
    * Let \f$k\f$ be the length of the cluster_sizes vector.
@@ -74,36 +90,36 @@
    * \par Example
    *
    * \code{cpp}
    * #include <stag/graph.h>
    * #include <stag/random.h>
    *
    * int main() {
-   *   std::vector<stag_int> cluster_sizes = {100, 20, 10};
+   *   std::vector<StagInt> cluster_sizes = {100, 20, 10};
    *   DenseMat prob_mat {{0.4, 0.1, 0.1}, {0.1, 0.7, 0}, {0.1, 0, 1}};
    *   stag::Graph myGraph = stag::general_sbm(cluster_sizes, prob_mat);
    *   std::cout << *myGraph.adjacency() << std::endl;
    *   return 0;
    * }
    * \endcode
    *
    * @param cluster_sizes a vector of length \f$k\f$ with the number of vertices
    *                      in each cluster.
    * @param probabilities a \f$k \times k\f$ matrix with the inter-cluster
    *                      probabilities.
    * @param exact (optional) whether to use the exact probability distribution. Default: false.
    * @return the randomly generated graph
    */
-  Graph general_sbm(std::vector<stag_int>& cluster_sizes,
+  Graph general_sbm(std::vector<StagInt>& cluster_sizes,
                     DenseMat& probabilities, bool exact);
 
   /**
    * @overload
    */
-  Graph general_sbm(std::vector<stag_int>& cluster_sizes,
+  Graph general_sbm(std::vector<StagInt>& cluster_sizes,
                     DenseMat& probabilities);
 
   /**
    * Generate a graph from the general stochastic block model and save the
    * resulting graph as an edgelist file.
    *
    * This method uses only constant memory since the graph can be streamed to
@@ -113,22 +129,22 @@
    * @param cluster_sizes a vector of length \f$k\f$ with the number of vertices
    *                      in each cluster.
    * @param probabilities a \f$k \times k\f$ matrix with the inter-cluster
    *                      probabilities.
    * @param exact (optional) whether to use the exact probability distribution. Default: false.
    */
   void general_sbm_edgelist(std::string& filename,
-                            std::vector<stag_int>& cluster_sizes,
+                            std::vector<StagInt>& cluster_sizes,
                             DenseMat& probabilities, bool exact);
 
   /**
    * @overload
    */
   void general_sbm_edgelist(std::string& filename,
-                            std::vector<stag_int>& cluster_sizes,
+                            std::vector<StagInt>& cluster_sizes,
                             DenseMat& probabilities);
 
   /**
    * Generate a graph from the Erdos-Renyi model.
    *
    * Generates a graph with \f$n\f$ vertices. For each pair of vertices \f$u\f$ and
    * \f$v\f$, the edge \f$\{u, v\}\f$ is included in the graph with probability \f$p\f$.
@@ -141,20 +157,20 @@
    * will be used, with running time \f$O(n^2)\f$.
    *
    * @param n the number of vertices in the graph
    * @param p the probability of including each edge
    * @param exact (optional) whether to sample from the exact model. Default: false.
    * @return the randomly generated graph
    */
-  Graph erdos_renyi(stag_int n, double p, bool exact);
+  Graph erdos_renyi(StagInt n, StagReal p, bool exact);
 
   /**
    * \overload
    */
-  Graph erdos_renyi(stag_int n, double p);
+  Graph erdos_renyi(StagInt n, StagReal p);
 
   /**
    * Construct a vector with the ground truth labels for a graph drawn from the
    * symmetric stochastic block model.
    *
    * \par Example
    *
@@ -177,15 +193,15 @@
    *
    *
    * @param n the number of vertices in the graph
    * @param k the number of clusters
    * @return a vector containing the ground truth labels for the vertices in the
    *         graph.
    */
-  std::vector<stag_int> sbm_gt_labels(stag_int n, stag_int k);
+  std::vector<StagInt> sbm_gt_labels(StagInt n, StagInt k);
 
   /**
    * Construct a vector with the ground truth labels for a graph drawn from the
    * general stochastic block model.
    *
    * \par Example
    *
@@ -207,11 +223,11 @@
    * \endcode
    *
    * @param cluster_sizes a vector of length \f$k\f$ with the number of vertices
    *                      in each cluster.
    * @return a vector containing the ground truth labels for the vertices in the
    *         graph.
    */
-  std::vector<stag_int> general_sbm_gt_labels(std::vector<stag_int>& cluster_sizes);
+  std::vector<StagInt> general_sbm_gt_labels(std::vector<StagInt>& cluster_sizes);
 }
 
 #endif //STAG_TEST_RANDOM_H
```

### Comparing `stag-1.2.1/stag/stag_lib/stagConfig.cmake.in` & `stag-2.0.0/stag/stag_lib/stagConfig.cmake.in`

 * *Files identical despite different names*

### Comparing `stag-1.2.1/stag/stag_lib/utility.cpp` & `stag-2.0.0/stag/stag_lib/utility.cpp`

 * *Files 8% similar despite different names*

```diff
@@ -1,86 +1,86 @@
-//
-// This file is provided as part of the STAG library and released under the MIT
-// license.
-//
+/*
+   This file is provided as part of the STAG library and released under the GPL
+   license.
+*/
 #include <iterator>
 #include <filesystem>
 #include "utility.h"
 
-std::vector<stag_int> stag::sprsMatInnerIndices(const SprsMat *matrix) {
+std::vector<StagInt> stag::sprsMatInnerIndices(const SprsMat *matrix) {
   // Make sure that the given matrix is compressed
   assert(matrix->isCompressed());
 
   // Return the required indices vector
-  const stag_int *indexPtr = matrix->innerIndexPtr();
-  stag_int nonZeros = matrix->nonZeros();
+  const StagInt *indexPtr = matrix->innerIndexPtr();
+  StagInt nonZeros = matrix->nonZeros();
   return {indexPtr, indexPtr + nonZeros};
 }
 
-std::vector<stag_int> stag::sprsMatOuterStarts(const SprsMat* matrix) {
+std::vector<StagInt> stag::sprsMatOuterStarts(const SprsMat* matrix) {
   // Make sure that the given matrix is compressed
   assert(matrix->isCompressed());
 
   // Return the required indices vector
-  const stag_int *indexPtr = matrix->outerIndexPtr();
-  stag_int outerSize = matrix->outerSize();
+  const StagInt *indexPtr = matrix->outerIndexPtr();
+  StagInt outerSize = matrix->outerSize();
   return {indexPtr, indexPtr + outerSize + 1};
 }
 
-std::vector<double> stag::sprsMatValues(const SprsMat* matrix) {
+std::vector<StagReal> stag::sprsMatValues(const SprsMat* matrix) {
   // Make sure that the given matrix is compressed
   assert(matrix->isCompressed());
 
   // Return the required indices vector
-  const double *valuePtr = matrix->valuePtr();
-  stag_int nonZeros = matrix->nonZeros();
+  const StagReal *valuePtr = matrix->valuePtr();
+  StagInt nonZeros = matrix->nonZeros();
   return {valuePtr, valuePtr + nonZeros};
 }
 
-std::vector<double> stag::sprsMatToVec(const SprsMat* matrix) {
+std::vector<StagReal> stag::sprsMatToVec(const SprsMat* matrix) {
   // If the number of dimensions is not given, use the dimension of the sparse
   // matrix.
   return stag::sprsMatToVec(matrix, matrix->rows());
 }
 
-std::vector<double> stag::sprsMatToVec(const SprsMat* matrix, stag_int n) {
+std::vector<StagReal> stag::sprsMatToVec(const SprsMat* matrix, StagInt n) {
   if (n < 1) throw std::invalid_argument("Dimension n must be at least 1.");
 
   // Initialise the solution vector.
-  std::vector<double> dense_vec;
+  std::vector<StagReal> dense_vec;
 
-  for (stag_int i = 0; i < n; i++) {
+  for (StagInt i = 0; i < n; i++) {
     if (i < matrix->rows()) {
       // Get the i-th entry of the sparse matrix
       dense_vec.push_back(matrix->coeff(i, 0));
     } else {
       // If the sparse matrix is not long enough, fill the vector with 0s.
       dense_vec.push_back(0);
     }
   }
   return dense_vec;
 }
 
-SprsMat stag::sprsMatFromVectors(std::vector<stag_int>& column_starts,
-                                 std::vector<stag_int>& row_indices,
-                                 std::vector<double>& values) {
+SprsMat stag::sprsMatFromVectors(std::vector<StagInt>& column_starts,
+                                 std::vector<StagInt>& row_indices,
+                                 std::vector<StagReal>& values) {
   // The length of the row_indices and values vectors should be the same
   if (row_indices.size() != values.size()) {
     throw std::invalid_argument("Sparse matrix indices and values array length mismatch.");
   }
 
   // The last value in the column_starts vector should be equal to the length
   // of the data vectors.
-  if (column_starts.back() != (stag_int) row_indices.size()) {
+  if (column_starts.back() != (StagInt) row_indices.size()) {
     throw std::invalid_argument("Final column starts entry should equal size of data vectors.");
   }
 
-  SprsMat constructed_mat = Eigen::Map<SprsMat>((stag_int) column_starts.size() - 1,
-                                                (stag_int) column_starts.size() - 1,
-                                                (stag_int) values.size(),
+  SprsMat constructed_mat = Eigen::Map<SprsMat>((StagInt) column_starts.size() - 1,
+                                                (StagInt) column_starts.size() - 1,
+                                                (StagInt) values.size(),
                                                 column_starts.data(),
                                                 row_indices.data(),
                                                 values.data());
   constructed_mat.makeCompressed();
   return constructed_mat;
 }
```

### Comparing `stag-1.2.1/stag/stag_lib/utility.h` & `stag-2.0.0/stag/stag_lib/utility.h`

 * *Files 5% similar despite different names*

```diff
@@ -1,84 +1,94 @@
-//
-// Definitions of utility methods for dealing with sparse matrices.
-//
-// This file is provided as part of the STAG library and released under the MIT
-// license.
-//
+/*
+   This file is provided as part of the STAG library and released under the GPL
+   license.
+*/
 
 /**
  * @file utility.h
  * \brief Various helper methods for working with the STAG library.
  */
 
 #ifndef STAG_TEST_UTILITY_H
 #define STAG_TEST_UTILITY_H
 
 #include <iostream>
 
 #include "graph.h"
 
+/**
+ * \cond
+ */
+#ifndef NDEBUG
+#  define LOG_DEBUG(x) do { std::cerr << x; } while (0)
+#else
+#  define LOG_DEBUG(x)
+#endif
+/**
+ * \endcond
+ */
+
 namespace stag {
 
   /**
    * Given a sparse matrix, return the values vector, compatible with the CSC
    * format of other libraries.
    */
-  std::vector<double> sprsMatValues(const SprsMat *matrix);
+  std::vector<StagReal> sprsMatValues(const SprsMat *matrix);
 
   /**
    * Given a sparse matrix, return the InnerIndices vector, compatible with the
    * CSC format of other libraries.
    */
-  std::vector<stag_int> sprsMatInnerIndices(const SprsMat *matrix);
+  std::vector<StagInt> sprsMatInnerIndices(const SprsMat *matrix);
 
   /**
    * Given a sparse matrix, return the OuterStarts vector, compatible with the
    * CSC format of other libraries.
    */
-  std::vector<stag_int> sprsMatOuterStarts(const SprsMat *matrix);
+  std::vector<StagInt> sprsMatOuterStarts(const SprsMat *matrix);
 
   /**
    * Given a sparse 'matrix' with only one column, convert it to a dense vector.
    *
    * @param matrix - the sparse vector to convert
    * @param n (optional) - the dimension of the dense vector to construct
    * @return a vector
    */
-   std::vector<double> sprsMatToVec(const SprsMat *matrix, stag_int n);
+   std::vector<StagReal> sprsMatToVec(const SprsMat *matrix, StagInt n);
 
    /**
     * \overload
     */
-   std::vector<double> sprsMatToVec(const SprsMat *matrix);
+   std::vector<StagReal> sprsMatToVec(const SprsMat *matrix);
 
    /**
     * Construct a sparse matrix from the CSC data vectors.
     *
     * For documentation on the format of the data vectors, please see the
     * documentation for the Eigen sparse matrix object.
     *
     * This method does not perform any error checking on the provided
     * vectors. The caller is responsible for ensuring that the provided data
     * vectors are well-formed.
     */
-   SprsMat sprsMatFromVectors(std::vector<stag_int>& column_starts,
-                              std::vector<stag_int>& row_indices,
-                              std::vector<double>& values);
+   SprsMat sprsMatFromVectors(std::vector<StagInt>& column_starts,
+                              std::vector<StagInt>& row_indices,
+                              std::vector<StagReal>& values);
 
    /**
     * Add two vectors together element-wise.
     */
    template <typename T>
    std::vector<T> addVectors(std::vector<T>& v1, std::vector<T>& v2) {
-     auto length = (stag_int) std::max(v1.size(), v2.size());
+     auto length = (StagInt) std::max(v1.size(), v2.size());
      std::vector<T> ans;
      T this_entry;
 
-     for (stag_int i = 0; i < length; i++) {
+     for (StagInt i = 0; i < length; i++) {
        this_entry = 0;
        if (v1.size() > i) this_entry += v1.at(i);
        if (v2.size() > i) this_entry += v2.at(i);
        ans.push_back(this_entry);
      }
 
      return ans;
```

### Comparing `stag-1.2.1/stag.egg-info/PKG-INFO` & `stag-2.0.0/stag.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stag
-Version: 1.2.1
+Version: 2.0.0
 Summary: STAG: Spectral Toolkit of Algorithms for Graphs
 Home-page: https://staglibrary.io
 Author: Peter Macgregor
 Author-email: <macgregor.pr@gmail.com>
 License: UNKNOWN
 Keywords: python,spectral,graph,algorithms,clustering,cheeger
 Platform: UNKNOWN
```

### Comparing `stag-1.2.1/test/test_graphio.py` & `stag-2.0.0/test/test_graphio.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Tests for handling reading and writing graphs to disk.
 """
+import pytest
 import scipy as sp
 import scipy.sparse
 from context import stag
 import stag.graph
 import stag.random
 import stag.graphio
 
@@ -14,94 +15,94 @@
     # TEST 1 #
     ##########
     # Let's load the different test graphs, and check that we get what we'd expect.
     expected_adj_mat = sp.sparse.csc_matrix([[0, 1, 1],
                                              [1, 0, 1],
                                              [1, 1, 0]])
     graph = stag.graphio.load_edgelist("data/test1.edgelist")
-    adj_mat_diff = (graph.adjacency() - expected_adj_mat)
+    adj_mat_diff = (graph.adjacency().to_scipy() - expected_adj_mat)
     adj_mat_diff.eliminate_zeros()
     assert adj_mat_diff.nnz == 0
 
     # Now save and reload the graph and check that the adjacency matrix has not changed
     stag.graphio.save_edgelist(graph, "data/temp.edgelist")
     graph = stag.graphio.load_edgelist("data/temp.edgelist")
-    adj_mat_diff = (graph.adjacency() - expected_adj_mat)
+    adj_mat_diff = (graph.adjacency().to_scipy() - expected_adj_mat)
     adj_mat_diff.eliminate_zeros()
     assert adj_mat_diff.nnz == 0
 
     ##########
     # TEST 2 #
     ##########
     expected_adj_mat = sp.sparse.csc_matrix([[0, 0.5, 0.5],
                                              [0.5, 0, 1],
                                              [0.5, 1, 0]])
     graph = stag.graphio.load_edgelist("data/test2.edgelist")
-    adj_mat_diff = (graph.adjacency() - expected_adj_mat)
+    adj_mat_diff = (graph.adjacency().to_scipy() - expected_adj_mat)
     adj_mat_diff.eliminate_zeros()
     assert adj_mat_diff.nnz == 0
 
     # Now save and reload the graph and check that the adjacency matrix has not changed
     stag.graphio.save_edgelist(graph, "data/temp.edgelist")
     graph = stag.graphio.load_edgelist("data/temp.edgelist")
-    adj_mat_diff = (graph.adjacency() - expected_adj_mat)
+    adj_mat_diff = (graph.adjacency().to_scipy() - expected_adj_mat)
     adj_mat_diff.eliminate_zeros()
     assert adj_mat_diff.nnz == 0
 
     ##########
     # TEST 3 #
     ##########
     expected_adj_mat = sp.sparse.csc_matrix([[0, 1, 0.5],
                                              [1, 0, 1],
                                              [0.5, 1, 0]])
     graph = stag.graphio.load_edgelist("data/test3.edgelist")
-    adj_mat_diff = (graph.adjacency() - expected_adj_mat)
+    adj_mat_diff = (graph.adjacency().to_scipy() - expected_adj_mat)
     adj_mat_diff.eliminate_zeros()
     assert adj_mat_diff.nnz == 0
 
     # Now save and reload the graph and check that the adjacency matrix has not changed
     stag.graphio.save_edgelist(graph, "data/temp.edgelist")
     graph = stag.graphio.load_edgelist("data/temp.edgelist")
-    adj_mat_diff = (graph.adjacency() - expected_adj_mat)
+    adj_mat_diff = (graph.adjacency().to_scipy() - expected_adj_mat)
     adj_mat_diff.eliminate_zeros()
     assert adj_mat_diff.nnz == 0
 
     ##########
     # TEST 4 #
     ##########
     expected_adj_mat = sp.sparse.csc_matrix([[0, 1, 0.5],
                                              [1, 0, 1],
                                              [0.5, 1, 0]])
     graph = stag.graphio.load_edgelist("data/test4.edgelist")
-    adj_mat_diff = (graph.adjacency() - expected_adj_mat)
+    adj_mat_diff = (graph.adjacency().to_scipy() - expected_adj_mat)
     adj_mat_diff.eliminate_zeros()
     assert adj_mat_diff.nnz == 0
 
     # Now save and reload the graph and check that the adjacency matrix has not changed
     stag.graphio.save_edgelist(graph, "data/temp.edgelist")
     graph = stag.graphio.load_edgelist("data/temp.edgelist")
-    adj_mat_diff = (graph.adjacency() - expected_adj_mat)
+    adj_mat_diff = (graph.adjacency().to_scipy() - expected_adj_mat)
     adj_mat_diff.eliminate_zeros()
     assert adj_mat_diff.nnz == 0
 
     ##########
     # TEST 5 #
     ##########
     expected_adj_mat = sp.sparse.csc_matrix([[0, 0.5, 0.5],
                                              [0.5, 0, 1],
                                              [0.5, 1, 0]])
     graph = stag.graphio.load_edgelist("data/test5.edgelist")
-    adj_mat_diff = (graph.adjacency() - expected_adj_mat)
+    adj_mat_diff = (graph.adjacency().to_scipy() - expected_adj_mat)
     adj_mat_diff.eliminate_zeros()
     assert adj_mat_diff.nnz == 0
 
     # Now save and reload the graph and check that the adjacency matrix has not changed
     stag.graphio.save_edgelist(graph, "data/temp.edgelist")
     graph = stag.graphio.load_edgelist("data/temp.edgelist")
-    adj_mat_diff = (graph.adjacency() - expected_adj_mat)
+    adj_mat_diff = (graph.adjacency().to_scipy() - expected_adj_mat)
     adj_mat_diff.eliminate_zeros()
     assert adj_mat_diff.nnz == 0
 
 
 def test_adjacencylist():
     edgelist_fname = "data/test3.edgelist"
     adjlist_fname = "data/temp.al"
@@ -115,7 +116,15 @@
     adj_g = stag.graphio.load_adjacencylist(adjlist_fname)
     assert edge_g == adj_g
 
     # Then, convert the adjacency list back to an edgelist
     stag.graphio.adjacencylist_to_edgelist(adjlist_fname, temp_edgelist_fname)
     edge_g = stag.graphio.load_edgelist(temp_edgelist_fname)
     assert edge_g == adj_g
+
+
+def test_bad_directory():
+    g = stag.graph.complete_graph(10)
+    bad_filename = "/bad/path/file.edgelist"
+
+    with pytest.raises(AttributeError):
+        stag.graphio.save_edgelist(g, bad_filename)
```

### Comparing `stag-1.2.1/test/test_random.py` & `stag-2.0.0/test/test_random.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     n = 2000
     p = 0.8
     q = 0.2
     graph = stag.random.sbm(n, 4, p, q, exact=True)
     assert graph.number_of_vertices() == 2000
 
     # The adjacency matrix should be symmetric
-    sym_diff = (graph.adjacency() - graph.adjacency().transpose())
+    sym_diff = (graph.adjacency().to_scipy() - graph.adjacency().to_scipy().transpose())
     sym_diff.eliminate_zeros()
     assert sym_diff.nnz == 0
 
     # The number of edges should be about
     # n * ((n/4) * p + (3 * n/4) * q)
     assert abs((graph.total_volume() / (n * ((n/4) * p + (3 * n/4) * q))) - 1) <= 0.1
 
@@ -52,21 +52,21 @@
     assert abs((graph.total_volume() / (int(2 * 0.1 * (n * (n - 1)) / 2) + n)) - 1) <= 0.1
 
 
 def test_sbm_gt_labels():
     n = 6
     k = 3
     labels = stag.random.sbm_gt_labels(n, k)
-    assert labels == [0, 0, 1, 1, 2, 2]
+    assert list(labels) == [0, 0, 1, 1, 2, 2]
 
 
 def test_general_sbm_gt_labels():
     cluster_sizes = [4, 2]
     gt_labels = stag.random.general_sbm_gt_labels(cluster_sizes)
-    assert gt_labels == [0, 0, 0, 0, 1, 1]
+    assert list(gt_labels) == [0, 0, 0, 0, 1, 1]
 
 
 def test_edgelist_sbm():
     edgelist_filename = "data/temp.el"
     cluster_sizes = [10, 100]
     probabilities = np.asarray([[0.9, 0.1],
                                 [0.1, 0.9]])
```

### Comparing `stag-1.2.1/test/test_spectrum.py` & `stag-2.0.0/test/test_spectrum.py`

 * *Files 19% similar despite different names*

```diff
@@ -7,32 +7,39 @@
 import stag.graph
 import stag.cluster
 import stag.random
 import stag.spectrum
 
 def test_power_method():
     g = stag.graph.complete_graph(3)
-    lap = g.laplacian()
+    lap = g.laplacian().to_scipy()
     assert(lap.shape == (3, 3))
     vec = np.asarray([[0, 1, 0]]).T
     assert vec.shape == (3, 1)
 
     newvec = stag.spectrum.power_method(lap,
                                         num_iterations=2,
                                         initial_vector=vec)
 
     assert np.allclose(newvec, np.asarray([[-1/math.sqrt(6),
                                              2/math.sqrt(6),
                                             -1/math.sqrt(6)]]).T, atol=0.00001)
 
     g = stag.graph.cycle_graph(10)
-    lap = g.normalised_laplacian()
+    lap = g.normalised_laplacian().to_scipy()
     dominant_eigvec = stag.spectrum.power_method(lap, num_iterations=1000)
     assert abs(2 - stag.spectrum.rayleigh_quotient(lap, dominant_eigvec)) < 0.0001
 
 
 def test_eigensystem():
-    g = stag.graph.complete_graph(4)
-    lap = g.laplacian()
-    eigval, eigvec = stag.spectrum.compute_eigensystem(lap, 1)
-    assert np.allclose(eigval, np.asarray([0]))
-    assert np.allclose(eigvec, np.asarray([[1/2, 1/2, 1/2, 1/2]]).T)
+    g = stag.graph.complete_graph(10)
+    eigval, eigvec = stag.spectrum.compute_eigensystem(
+        g, 'NormalisedLaplacian', 4, 'Smallest')
+    assert np.allclose(min(eigval), np.asarray([0]))
+    assert(eigvec[:, np.argmin(eigval)][3] == pytest.approx(1 / math.sqrt(10)))
+
+
+def test_real_eigenvalues():
+    g = stag.random.sbm(1000, 2, 0.1, 0.01)
+    eigvals = stag.spectrum.compute_eigenvalues(
+        g, 'NormalisedLaplacian', 4, 'Smallest')
+    assert(eigvals.dtype == np.dtype('float'))
```

