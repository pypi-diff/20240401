# Comparing `tmp/ml_dtypes-0.3.2.tar.gz` & `tmp/ml_dtypes-0.4.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ml_dtypes-0.3.2.tar", last modified: Wed Jan  3 18:51:56 2024, max compression
+gzip compressed data, was "ml_dtypes-0.4.0b1.tar", last modified: Tue Mar 12 19:54:44 2024, max compression
```

## Comparing `ml_dtypes-0.3.2.tar` & `ml_dtypes-0.4.0b1.tar`

### file list

```diff
@@ -1,240 +1,240 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-03 18:51:56.184369 ml_dtypes-0.3.2/
--rw-r--r--   0 runner    (1001) docker     (127)      301 2024-01-03 18:51:44.000000 ml_dtypes-0.3.2/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-01-03 18:51:44.000000 ml_dtypes-0.3.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    16726 2024-01-03 18:51:44.000000 ml_dtypes-0.3.2/LICENSE.eigen
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-01-03 18:51:44.000000 ml_dtypes-0.3.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    19733 2024-01-03 18:51:56.184369 ml_dtypes-0.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6148 2024-01-03 18:51:44.000000 ml_dtypes-0.3.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-03 18:51:56.148369 ml_dtypes-0.3.2/ml_dtypes/
--rw-r--r--   0 runner    (1001) docker     (127)     1629 2024-01-03 18:51:44.000000 ml_dtypes-0.3.2/ml_dtypes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13506 2024-01-03 18:51:44.000000 ml_dtypes-0.3.2/ml_dtypes/_finfo.py
--rw-r--r--   0 runner    (1001) docker     (127)     1589 2024-01-03 18:51:44.000000 ml_dtypes-0.3.2/ml_dtypes/_iinfo.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-03 18:51:56.152369 ml_dtypes-0.3.2/ml_dtypes/_src/
--rw-r--r--   0 runner    (1001) docker     (127)     4370 2024-01-03 18:51:44.000000 ml_dtypes-0.3.2/ml_dtypes/_src/common.h
--rw-r--r--   0 runner    (1001) docker     (127)    34136 2024-01-03 18:51:44.000000 ml_dtypes-0.3.2/ml_dtypes/_src/custom_float.h
--rw-r--r--   0 runner    (1001) docker     (127)    12843 2024-01-03 18:51:44.000000 ml_dtypes-0.3.2/ml_dtypes/_src/dtypes.cc
--rw-r--r--   0 runner    (1001) docker     (127)    25957 2024-01-03 18:51:44.000000 ml_dtypes-0.3.2/ml_dtypes/_src/int4_numpy.h
--rw-r--r--   0 runner    (1001) docker     (127)      909 2024-01-03 18:51:44.000000 ml_dtypes-0.3.2/ml_dtypes/_src/numpy.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1577 2024-01-03 18:51:44.000000 ml_dtypes-0.3.2/ml_dtypes/_src/numpy.h
--rw-r--r--   0 runner    (1001) docker     (127)    19888 2024-01-03 18:51:44.000000 ml_dtypes-0.3.2/ml_dtypes/_src/ufuncs.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-03 18:51:56.152369 ml_dtypes-0.3.2/ml_dtypes/include/
--rw-r--r--   0 runner    (1001) docker     (127)    51693 2024-01-03 18:51:44.000000 ml_dtypes-0.3.2/ml_dtypes/include/float8.h
--rw-r--r--   0 runner    (1001) docker     (127)    10028 2024-01-03 18:51:44.000000 ml_dtypes-0.3.2/ml_dtypes/include/int4.h
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-03 18:51:44.000000 ml_dtypes-0.3.2/ml_dtypes/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-03 18:51:56.152369 ml_dtypes-0.3.2/ml_dtypes.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    19733 2024-01-03 18:51:56.000000 ml_dtypes-0.3.2/ml_dtypes.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10642 2024-01-03 18:51:56.000000 ml_dtypes-0.3.2/ml_dtypes.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-03 18:51:56.000000 ml_dtypes-0.3.2/ml_dtypes.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      195 2024-01-03 18:51:56.000000 ml_dtypes-0.3.2/ml_dtypes.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-01-03 18:51:56.000000 ml_dtypes-0.3.2/ml_dtypes.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1768 2024-01-03 18:51:44.000000 ml_dtypes-0.3.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-03 18:51:56.184369 ml_dtypes-0.3.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2264 2024-01-03 18:51:44.000000 ml_dtypes-0.3.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-03 18:51:56.144369 ml_dtypes-0.3.2/third_party/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-03 18:51:56.144369 ml_dtypes-0.3.2/third_party/eigen/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-03 18:51:56.152369 ml_dtypes-0.3.2/third_party/eigen/Eigen/
--rw-r--r--   0 runner    (1001) docker     (127)    13374 2024-01-03 18:51:46.000000 ml_dtypes-0.3.2/third_party/eigen/Eigen/Core
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-03 18:51:56.148369 ml_dtypes-0.3.2/third_party/eigen/Eigen/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-03 18:51:56.164369 ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/
--rw-r--r--   0 runner    (1001) docker     (127)    10790 2024-01-03 18:51:46.000000 ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/ArithmeticSequence.h
--rw-r--r--   0 runner    (1001) docker     (127)    16400 2024-01-03 18:51:46.000000 ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/Array.h
--rw-r--r--   0 runner    (1001) docker     (127)     8252 2024-01-03 18:51:46.000000 ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/ArrayBase.h
--rw-r--r--   0 runner    (1001) docker     (127)     6878 2024-01-03 18:51:46.000000 ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/ArrayWrapper.h
--rw-r--r--   0 runner    (1001) docker     (127)     2774 2024-01-03 18:51:46.000000 ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/Assign.h
--rw-r--r--   0 runner    (1001) docker     (127)    41912 2024-01-03 18:51:46.000000 ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/AssignEvaluator.h
--rw-r--r--   0 runner    (1001) docker     (127)    12508 2024-01-03 18:51:46.000000 ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/Assign_MKL.h
--rw-r--r--   0 runner    (1001) docker     (127)    14072 2024-01-03 18:51:46.000000 ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/BandMatrix.h
--rw-r--r--   0 runner    (1001) docker     (127)    19246 2024-01-03 18:51:46.000000 ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/Block.h
--rw-r--r--   0 runner    (1001) docker     (127)     6092 2024-01-03 18:51:46.000000 ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/CommaInitializer.h
--rw-r--r--   0 runner    (1001) docker     (127)     7070 2024-01-03 18:51:46.000000 ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/ConditionEstimator.h
--rw-r--r--   0 runner    (1001) docker     (127)    63843 2024-01-03 18:51:46.000000 ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/CoreEvaluators.h
--rw-r--r--   0 runner    (1001) docker     (127)     4781 2024-01-03 18:51:46.000000 ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/CoreIterators.h
--rw-r--r--   0 runner    (1001) docker     (127)     7756 2024-01-03 18:51:46.000000 ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/CwiseBinaryOp.h
--rw-r--r--   0 runner    (1001) docker     (127)    37759 2024-01-03 18:51:46.000000 ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/CwiseNullaryOp.h
--rw-r--r--   0 runner    (1001) docker     (127)     8034 2024-01-03 18:51:46.000000 ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/CwiseTernaryOp.h
--rw-r--r--   0 runner    (1001) docker     (127)     3926 2024-01-03 18:51:46.000000 ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/CwiseUnaryOp.h
--rw-r--r--   0 runner    (1001) docker     (127)     6274 2024-01-03 18:51:46.000000 ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/CwiseUnaryView.h
--rw-r--r--   0 runner    (1001) docker     (127)    32035 2024-01-03 18:51:46.000000 ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/DenseBase.h
--rw-r--r--   0 runner    (1001) docker     (127)    24436 2024-01-03 18:51:46.000000 ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/DenseCoeffsBase.h
--rw-r--r--   0 runner    (1001) docker     (127)    28937 2024-01-03 18:51:46.000000 ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/DenseStorage.h
--rw-r--r--   0 runner    (1001) docker     (127)     9601 2024-01-03 18:51:46.000000 ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/Diagonal.h
--rw-r--r--   0 runner    (1001) docker     (127)    18129 2024-01-03 18:51:46.000000 ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/DiagonalMatrix.h
--rw-r--r--   0 runner    (1001) docker     (127)     1024 2024-01-03 18:51:46.000000 ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/DiagonalProduct.h
--rw-r--r--   0 runner    (1001) docker     (127)    11413 2024-01-03 18:51:46.000000 ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/Dot.h
--rw-r--r--   0 runner    (1001) docker     (127)     5877 2024-01-03 18:51:46.000000 ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/EigenBase.h
--rw-r--r--   0 runner    (1001) docker     (127)     4886 2024-01-03 18:51:46.000000 ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/ForceAlignedAccess.h
--rw-r--r--   0 runner    (1001) docker     (127)     5813 2024-01-03 18:51:46.000000 ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/Fuzzy.h
--rw-r--r--   0 runner    (1001) docker     (127)    21625 2024-01-03 18:51:46.000000 ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/GeneralProduct.h
--rw-r--r--   0 runner    (1001) docker     (127)    49384 2024-01-03 18:51:46.000000 ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/GenericPacketMath.h
--rw-r--r--   0 runner    (1001) docker     (127)    12188 2024-01-03 18:51:46.000000 ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/GlobalFunctions.h
--rw-r--r--   0 runner    (1001) docker     (127)     8402 2024-01-03 18:51:46.000000 ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/IO.h
--rw-r--r--   0 runner    (1001) docker     (127)    10698 2024-01-03 18:51:46.000000 ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/IndexedView.h
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-01-03 18:51:46.000000 ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/InternalHeaderCheck.h
--rw-r--r--   0 runner    (1001) docker     (127)     3510 2024-01-03 18:51:46.000000 ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/Inverse.h
--rw-r--r--   0 runner    (1001) docker     (127)     7127 2024-01-03 18:51:46.000000 ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/Map.h
--rw-r--r--   0 runner    (1001) docker     (127)    11209 2024-01-03 18:51:46.000000 ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/MapBase.h
--rw-r--r--   0 runner    (1001) docker     (127)    61532 2024-01-03 18:51:46.000000 ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/MathFunctions.h
--rw-r--r--   0 runner    (1001) docker     (127)    13345 2024-01-03 18:51:46.000000 ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/MathFunctionsImpl.h
--rw-r--r--   0 runner    (1001) docker     (127)    24419 2024-01-03 18:51:46.000000 ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/Matrix.h
--rw-r--r--   0 runner    (1001) docker     (127)    23983 2024-01-03 18:51:46.000000 ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/MatrixBase.h
--rw-r--r--   0 runner    (1001) docker     (127)     3095 2024-01-03 18:51:46.000000 ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/NestByValue.h
--rw-r--r--   0 runner    (1001) docker     (127)     3656 2024-01-03 18:51:46.000000 ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/NoAlias.h
--rw-r--r--   0 runner    (1001) docker     (127)    13346 2024-01-03 18:51:46.000000 ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/NumTraits.h
--rw-r--r--   0 runner    (1001) docker     (127)     9281 2024-01-03 18:51:46.000000 ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/PartialReduxEvaluator.h
--rw-r--r--   0 runner    (1001) docker     (127)    20771 2024-01-03 18:51:46.000000 ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/PermutationMatrix.h
--rw-r--r--   0 runner    (1001) docker     (127)    48620 2024-01-03 18:51:46.000000 ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/PlainObjectBase.h
--rw-r--r--   0 runner    (1001) docker     (127)     7314 2024-01-03 18:51:46.000000 ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/Product.h
--rw-r--r--   0 runner    (1001) docker     (127)    55121 2024-01-03 18:51:46.000000 ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/ProductEvaluators.h
--rw-r--r--   0 runner    (1001) docker     (127)     7748 2024-01-03 18:51:46.000000 ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/Random.h
--rw-r--r--   0 runner    (1001) docker     (127)    19216 2024-01-03 18:51:46.000000 ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/Redux.h
--rw-r--r--   0 runner    (1001) docker     (127)    17769 2024-01-03 18:51:46.000000 ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/Ref.h
--rw-r--r--   0 runner    (1001) docker     (127)     5635 2024-01-03 18:51:46.000000 ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/Replicate.h
--rw-r--r--   0 runner    (1001) docker     (127)    16983 2024-01-03 18:51:46.000000 ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/Reshaped.h
--rw-r--r--   0 runner    (1001) docker     (127)     4317 2024-01-03 18:51:46.000000 ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/ReturnByValue.h
--rw-r--r--   0 runner    (1001) docker     (127)     7552 2024-01-03 18:51:46.000000 ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/Reverse.h
--rw-r--r--   0 runner    (1001) docker     (127)     7760 2024-01-03 18:51:46.000000 ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/Select.h
--rw-r--r--   0 runner    (1001) docker     (127)    14908 2024-01-03 18:51:46.000000 ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/SelfAdjointView.h
--rw-r--r--   0 runner    (1001) docker     (127)     1733 2024-01-03 18:51:46.000000 ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/SelfCwiseBinaryOp.h
--rw-r--r--   0 runner    (1001) docker     (127)    16006 2024-01-03 18:51:46.000000 ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/SkewSymmetricMatrix3.h
--rw-r--r--   0 runner    (1001) docker     (127)     6902 2024-01-03 18:51:46.000000 ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/Solve.h
--rw-r--r--   0 runner    (1001) docker     (127)     9332 2024-01-03 18:51:46.000000 ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/SolveTriangular.h
--rw-r--r--   0 runner    (1001) docker     (127)     5967 2024-01-03 18:51:46.000000 ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/SolverBase.h
--rw-r--r--   0 runner    (1001) docker     (127)     8689 2024-01-03 18:51:46.000000 ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/StableNorm.h
--rw-r--r--   0 runner    (1001) docker     (127)    21245 2024-01-03 18:51:46.000000 ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/StlIterators.h
--rw-r--r--   0 runner    (1001) docker     (127)     4450 2024-01-03 18:51:46.000000 ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/Stride.h
--rw-r--r--   0 runner    (1001) docker     (127)     2801 2024-01-03 18:51:46.000000 ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/Swap.h
--rw-r--r--   0 runner    (1001) docker     (127)    17669 2024-01-03 18:51:46.000000 ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/Transpose.h
--rw-r--r--   0 runner    (1001) docker     (127)    13603 2024-01-03 18:51:46.000000 ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/Transpositions.h
--rw-r--r--   0 runner    (1001) docker     (127)    38143 2024-01-03 18:51:46.000000 ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/TriangularMatrix.h
--rw-r--r--   0 runner    (1001) docker     (127)     3461 2024-01-03 18:51:46.000000 ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/VectorBlock.h
--rw-r--r--   0 runner    (1001) docker     (127)    35183 2024-01-03 18:51:46.000000 ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/VectorwiseOp.h
--rw-r--r--   0 runner    (1001) docker     (127)    35231 2024-01-03 18:51:46.000000 ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/Visitor.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-03 18:51:56.148369 ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/arch/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-03 18:51:56.168369 ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/arch/AVX/
--rw-r--r--   0 runner    (1001) docker     (127)    14975 2024-01-03 18:51:46.000000 ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/arch/AVX/Complex.h
--rw-r--r--   0 runner    (1001) docker     (127)     6568 2024-01-03 18:51:46.000000 ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/arch/AVX/MathFunctions.h
--rw-r--r--   0 runner    (1001) docker     (127)    83727 2024-01-03 18:51:46.000000 ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/arch/AVX/PacketMath.h
--rw-r--r--   0 runner    (1001) docker     (127)     2604 2024-01-03 18:51:46.000000 ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/arch/AVX/TypeCasting.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-03 18:51:56.168369 ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/arch/AVX512/
--rw-r--r--   0 runner    (1001) docker     (127)    15797 2024-01-03 18:51:46.000000 ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/arch/AVX512/Complex.h
--rw-r--r--   0 runner    (1001) docker     (127)    47758 2024-01-03 18:51:46.000000 ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/arch/AVX512/GemmKernel.h
--rw-r--r--   0 runner    (1001) docker     (127)     9597 2024-01-03 18:51:46.000000 ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/arch/AVX512/MathFunctions.h
--rw-r--r--   0 runner    (1001) docker     (127)   110036 2024-01-03 18:51:46.000000 ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/arch/AVX512/PacketMath.h
--rw-r--r--   0 runner    (1001) docker     (127)    26497 2024-01-03 18:51:46.000000 ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/arch/AVX512/PacketMathFP16.h
--rw-r--r--   0 runner    (1001) docker     (127)    56830 2024-01-03 18:51:46.000000 ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/arch/AVX512/TrsmKernel.h
--rw-r--r--   0 runner    (1001) docker     (127)     6072 2024-01-03 18:51:46.000000 ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/arch/AVX512/TypeCasting.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-03 18:51:56.168369 ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/arch/AltiVec/
--rw-r--r--   0 runner    (1001) docker     (127)    20546 2024-01-03 18:51:46.000000 ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/arch/AltiVec/Complex.h
--rw-r--r--   0 runner    (1001) docker     (127)     3685 2024-01-03 18:51:46.000000 ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/arch/AltiVec/MathFunctions.h
--rw-r--r--   0 runner    (1001) docker     (127)   129018 2024-01-03 18:51:46.000000 ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/arch/AltiVec/MatrixProduct.h
--rw-r--r--   0 runner    (1001) docker     (127)     6719 2024-01-03 18:51:46.000000 ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/arch/AltiVec/MatrixProductCommon.h
--rw-r--r--   0 runner    (1001) docker     (127)    28128 2024-01-03 18:51:46.000000 ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/arch/AltiVec/MatrixProductMMA.h
--rw-r--r--   0 runner    (1001) docker     (127)    15819 2024-01-03 18:51:46.000000 ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/arch/AltiVec/MatrixProductMMAbfloat16.h
--rw-r--r--   0 runner    (1001) docker     (127)    91478 2024-01-03 18:51:46.000000 ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/arch/AltiVec/MatrixVectorProduct.h
--rw-r--r--   0 runner    (1001) docker     (127)   119359 2024-01-03 18:51:46.000000 ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/arch/AltiVec/PacketMath.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-03 18:51:56.172369 ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/arch/Default/
--rw-r--r--   0 runner    (1001) docker     (127)    34597 2024-01-03 18:51:46.000000 ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/arch/Default/BFloat16.h
--rw-r--r--   0 runner    (1001) docker     (127)     5291 2024-01-03 18:51:46.000000 ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/arch/Default/ConjHelper.h
--rw-r--r--   0 runner    (1001) docker     (127)    94749 2024-01-03 18:51:46.000000 ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/arch/Default/GenericPacketMathFunctions.h
--rw-r--r--   0 runner    (1001) docker     (127)     4764 2024-01-03 18:51:46.000000 ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/arch/Default/GenericPacketMathFunctionsFwd.h
--rw-r--r--   0 runner    (1001) docker     (127)    39550 2024-01-03 18:51:46.000000 ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/arch/Default/Half.h
--rw-r--r--   0 runner    (1001) docker     (127)     1746 2024-01-03 18:51:46.000000 ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/arch/Default/Settings.h
--rw-r--r--   0 runner    (1001) docker     (127)     3534 2024-01-03 18:51:46.000000 ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/arch/Default/TypeCasting.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-03 18:51:56.172369 ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/arch/GPU/
--rw-r--r--   0 runner    (1001) docker     (127)    17981 2024-01-03 18:51:46.000000 ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/arch/GPU/Complex.h
--rw-r--r--   0 runner    (1001) docker     (127)     2735 2024-01-03 18:51:46.000000 ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/arch/GPU/MathFunctions.h
--rw-r--r--   0 runner    (1001) docker     (127)    58287 2024-01-03 18:51:46.000000 ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/arch/GPU/PacketMath.h
--rw-r--r--   0 runner    (1001) docker     (127)     9694 2024-01-03 18:51:46.000000 ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/arch/GPU/Tuple.h
--rw-r--r--   0 runner    (1001) docker     (127)     2297 2024-01-03 18:51:46.000000 ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/arch/GPU/TypeCasting.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-03 18:51:56.148369 ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/arch/HIP/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-03 18:51:56.172369 ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/arch/HIP/hcc/
--rw-r--r--   0 runner    (1001) docker     (127)      691 2024-01-03 18:51:46.000000 ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/arch/HIP/hcc/math_constants.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-03 18:51:56.172369 ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/arch/MSA/
--rw-r--r--   0 runner    (1001) docker     (127)    17448 2024-01-03 18:51:46.000000 ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/arch/MSA/Complex.h
--rw-r--r--   0 runner    (1001) docker     (127)    16053 2024-01-03 18:51:46.000000 ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/arch/MSA/MathFunctions.h
--rw-r--r--   0 runner    (1001) docker     (127)    33649 2024-01-03 18:51:46.000000 ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/arch/MSA/PacketMath.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-03 18:51:56.172369 ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/arch/NEON/
--rw-r--r--   0 runner    (1001) docker     (127)    22034 2024-01-03 18:51:46.000000 ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/arch/NEON/Complex.h
--rw-r--r--   0 runner    (1001) docker     (127)     9906 2024-01-03 18:51:46.000000 ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/arch/NEON/GeneralBlockPanelKernel.h
--rw-r--r--   0 runner    (1001) docker     (127)     4834 2024-01-03 18:51:46.000000 ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/arch/NEON/MathFunctions.h
--rw-r--r--   0 runner    (1001) docker     (127)   194432 2024-01-03 18:51:46.000000 ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/arch/NEON/PacketMath.h
--rw-r--r--   0 runner    (1001) docker     (127)    51898 2024-01-03 18:51:46.000000 ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/arch/NEON/TypeCasting.h
--rw-r--r--   0 runner    (1001) docker     (127)     1886 2024-01-03 18:51:46.000000 ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/arch/NEON/UnaryFunctors.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-03 18:51:56.172369 ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/arch/SSE/
--rw-r--r--   0 runner    (1001) docker     (127)    13550 2024-01-03 18:51:46.000000 ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/arch/SSE/Complex.h
--rw-r--r--   0 runner    (1001) docker     (127)     5016 2024-01-03 18:51:46.000000 ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/arch/SSE/MathFunctions.h
--rw-r--r--   0 runner    (1001) docker     (127)    72921 2024-01-03 18:51:46.000000 ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/arch/SSE/PacketMath.h
--rw-r--r--   0 runner    (1001) docker     (127)     3938 2024-01-03 18:51:46.000000 ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/arch/SSE/TypeCasting.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-03 18:51:56.176369 ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/arch/SVE/
--rw-r--r--   0 runner    (1001) docker     (127)     1169 2024-01-03 18:51:46.000000 ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/arch/SVE/MathFunctions.h
--rw-r--r--   0 runner    (1001) docker     (127)    21184 2024-01-03 18:51:46.000000 ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/arch/SVE/PacketMath.h
--rw-r--r--   0 runner    (1001) docker     (127)     1391 2024-01-03 18:51:46.000000 ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/arch/SVE/TypeCasting.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-03 18:51:56.176369 ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/arch/SYCL/
--rw-r--r--   0 runner    (1001) docker     (127)     7468 2024-01-03 18:51:46.000000 ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/arch/SYCL/InteropHeaders.h
--rw-r--r--   0 runner    (1001) docker     (127)    12579 2024-01-03 18:51:46.000000 ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/arch/SYCL/MathFunctions.h
--rw-r--r--   0 runner    (1001) docker     (127)    16205 2024-01-03 18:51:46.000000 ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/arch/SYCL/PacketMath.h
--rw-r--r--   0 runner    (1001) docker     (127)    21994 2024-01-03 18:51:46.000000 ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/arch/SYCL/SyclMemoryModel.h
--rw-r--r--   0 runner    (1001) docker     (127)     2669 2024-01-03 18:51:46.000000 ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/arch/SYCL/TypeCasting.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-03 18:51:56.176369 ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/arch/ZVector/
--rw-r--r--   0 runner    (1001) docker     (127)    16373 2024-01-03 18:51:46.000000 ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/arch/ZVector/Complex.h
--rw-r--r--   0 runner    (1001) docker     (127)     7927 2024-01-03 18:51:46.000000 ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/arch/ZVector/MathFunctions.h
--rw-r--r--   0 runner    (1001) docker     (127)    36916 2024-01-03 18:51:46.000000 ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/arch/ZVector/PacketMath.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-03 18:51:56.176369 ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/functors/
--rw-r--r--   0 runner    (1001) docker     (127)     6454 2024-01-03 18:51:46.000000 ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/functors/AssignmentFunctors.h
--rw-r--r--   0 runner    (1001) docker     (127)    31940 2024-01-03 18:51:46.000000 ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/functors/BinaryFunctors.h
--rw-r--r--   0 runner    (1001) docker     (127)     9534 2024-01-03 18:51:46.000000 ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/functors/NullaryFunctors.h
--rw-r--r--   0 runner    (1001) docker     (127)     4009 2024-01-03 18:51:46.000000 ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/functors/StlFunctors.h
--rw-r--r--   0 runner    (1001) docker     (127)     1786 2024-01-03 18:51:46.000000 ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/functors/TernaryFunctors.h
--rw-r--r--   0 runner    (1001) docker     (127)    45622 2024-01-03 18:51:46.000000 ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/functors/UnaryFunctors.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-03 18:51:56.180369 ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/products/
--rw-r--r--   0 runner    (1001) docker     (127)   140899 2024-01-03 18:51:46.000000 ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/products/GeneralBlockPanelKernel.h
--rw-r--r--   0 runner    (1001) docker     (127)    19832 2024-01-03 18:51:46.000000 ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/products/GeneralMatrixMatrix.h
--rw-r--r--   0 runner    (1001) docker     (127)    15819 2024-01-03 18:51:46.000000 ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/products/GeneralMatrixMatrixTriangular.h
--rw-r--r--   0 runner    (1001) docker     (127)     6973 2024-01-03 18:51:46.000000 ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/products/GeneralMatrixMatrixTriangular_BLAS.h
--rw-r--r--   0 runner    (1001) docker     (127)     5143 2024-01-03 18:51:46.000000 ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/products/GeneralMatrixMatrix_BLAS.h
--rw-r--r--   0 runner    (1001) docker     (127)    21745 2024-01-03 18:51:46.000000 ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/products/GeneralMatrixVector.h
--rw-r--r--   0 runner    (1001) docker     (127)     6405 2024-01-03 18:51:46.000000 ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/products/GeneralMatrixVector_BLAS.h
--rw-r--r--   0 runner    (1001) docker     (127)     5252 2024-01-03 18:51:46.000000 ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/products/Parallelizer.h
--rw-r--r--   0 runner    (1001) docker     (127)    21343 2024-01-03 18:51:46.000000 ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/products/SelfadjointMatrixMatrix.h
--rw-r--r--   0 runner    (1001) docker     (127)    11607 2024-01-03 18:51:46.000000 ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/products/SelfadjointMatrixMatrix_BLAS.h
--rw-r--r--   0 runner    (1001) docker     (127)     9893 2024-01-03 18:51:46.000000 ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/products/SelfadjointMatrixVector.h
--rw-r--r--   0 runner    (1001) docker     (127)     5246 2024-01-03 18:51:46.000000 ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/products/SelfadjointMatrixVector_BLAS.h
--rw-r--r--   0 runner    (1001) docker     (127)     6131 2024-01-03 18:51:46.000000 ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/products/SelfadjointProduct.h
--rw-r--r--   0 runner    (1001) docker     (127)     4077 2024-01-03 18:51:46.000000 ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/products/SelfadjointRank2Update.h
--rw-r--r--   0 runner    (1001) docker     (127)    20980 2024-01-03 18:51:46.000000 ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/products/TriangularMatrixMatrix.h
--rw-r--r--   0 runner    (1001) docker     (127)    13904 2024-01-03 18:51:46.000000 ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/products/TriangularMatrixMatrix_BLAS.h
--rw-r--r--   0 runner    (1001) docker     (127)    14886 2024-01-03 18:51:46.000000 ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/products/TriangularMatrixVector.h
--rw-r--r--   0 runner    (1001) docker     (127)    10608 2024-01-03 18:51:46.000000 ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/products/TriangularMatrixVector_BLAS.h
--rw-r--r--   0 runner    (1001) docker     (127)    19090 2024-01-03 18:51:46.000000 ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/products/TriangularSolverMatrix.h
--rw-r--r--   0 runner    (1001) docker     (127)     6744 2024-01-03 18:51:46.000000 ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/products/TriangularSolverMatrix_BLAS.h
--rw-r--r--   0 runner    (1001) docker     (127)     5779 2024-01-03 18:51:46.000000 ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/products/TriangularSolverVector.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-03 18:51:56.184369 ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/util/
--rw-r--r--   0 runner    (1001) docker     (127)     6211 2024-01-03 18:51:46.000000 ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/util/Assert.h
--rw-r--r--   0 runner    (1001) docker     (127)    26278 2024-01-03 18:51:46.000000 ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/util/BlasUtil.h
--rw-r--r--   0 runner    (1001) docker     (127)    19362 2024-01-03 18:51:46.000000 ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/util/ConfigureVectorization.h
--rw-r--r--   0 runner    (1001) docker     (127)    22214 2024-01-03 18:51:46.000000 ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/util/Constants.h
--rw-r--r--   0 runner    (1001) docker     (127)     6223 2024-01-03 18:51:46.000000 ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/util/DisableStupidWarnings.h
--rw-r--r--   0 runner    (1001) docker     (127)    15929 2024-01-03 18:51:46.000000 ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/util/ForwardDeclarations.h
--rw-r--r--   0 runner    (1001) docker     (127)     6273 2024-01-03 18:51:46.000000 ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/util/IndexedViewHelper.h
--rw-r--r--   0 runner    (1001) docker     (127)     9567 2024-01-03 18:51:46.000000 ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/util/IntegralConstant.h
--rw-r--r--   0 runner    (1001) docker     (127)     4305 2024-01-03 18:51:46.000000 ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/util/MKL_support.h
--rw-r--r--   0 runner    (1001) docker     (127)    48039 2024-01-03 18:51:46.000000 ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/util/Macros.h
--rw-r--r--   0 runner    (1001) docker     (127)    49577 2024-01-03 18:51:46.000000 ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/util/Memory.h
--rw-r--r--   0 runner    (1001) docker     (127)    20264 2024-01-03 18:51:46.000000 ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/util/Meta.h
--rw-r--r--   0 runner    (1001) docker     (127)     1387 2024-01-03 18:51:46.000000 ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/util/ReenableStupidWarnings.h
--rw-r--r--   0 runner    (1001) docker     (127)     1463 2024-01-03 18:51:46.000000 ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/util/ReshapedHelper.h
--rw-r--r--   0 runner    (1001) docker     (127)     7810 2024-01-03 18:51:46.000000 ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/util/Serializer.h
--rw-r--r--   0 runner    (1001) docker     (127)     5496 2024-01-03 18:51:46.000000 ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/util/StaticAssert.h
--rw-r--r--   0 runner    (1001) docker     (127)     9854 2024-01-03 18:51:46.000000 ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/util/SymbolicIndex.h
--rw-r--r--   0 runner    (1001) docker     (127)    35298 2024-01-03 18:51:46.000000 ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/util/XprHelper.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-03 18:51:56.184369 ml_dtypes-0.3.2/third_party/eigen/Eigen/src/plugins/
--rw-r--r--   0 runner    (1001) docker     (127)    13721 2024-01-03 18:51:46.000000 ml_dtypes-0.3.2/third_party/eigen/Eigen/src/plugins/ArrayCwiseBinaryOps.h
--rw-r--r--   0 runner    (1001) docker     (127)    22938 2024-01-03 18:51:46.000000 ml_dtypes-0.3.2/third_party/eigen/Eigen/src/plugins/ArrayCwiseUnaryOps.h
--rw-r--r--   0 runner    (1001) docker     (127)    58948 2024-01-03 18:51:46.000000 ml_dtypes-0.3.2/third_party/eigen/Eigen/src/plugins/BlockMethods.h
--rw-r--r--   0 runner    (1001) docker     (127)     6281 2024-01-03 18:51:46.000000 ml_dtypes-0.3.2/third_party/eigen/Eigen/src/plugins/CommonCwiseBinaryOps.h
--rw-r--r--   0 runner    (1001) docker     (127)     5927 2024-01-03 18:51:46.000000 ml_dtypes-0.3.2/third_party/eigen/Eigen/src/plugins/CommonCwiseUnaryOps.h
--rw-r--r--   0 runner    (1001) docker     (127)    12022 2024-01-03 18:51:46.000000 ml_dtypes-0.3.2/third_party/eigen/Eigen/src/plugins/IndexedViewMethods.h
--rw-r--r--   0 runner    (1001) docker     (127)      137 2024-01-03 18:51:46.000000 ml_dtypes-0.3.2/third_party/eigen/Eigen/src/plugins/InternalHeaderCheck.h
--rw-r--r--   0 runner    (1001) docker     (127)    16947 2024-01-03 18:51:46.000000 ml_dtypes-0.3.2/third_party/eigen/Eigen/src/plugins/MatrixCwiseBinaryOps.h
--rw-r--r--   0 runner    (1001) docker     (127)     4105 2024-01-03 18:51:46.000000 ml_dtypes-0.3.2/third_party/eigen/Eigen/src/plugins/MatrixCwiseUnaryOps.h
--rw-r--r--   0 runner    (1001) docker     (127)     6891 2024-01-03 18:51:46.000000 ml_dtypes-0.3.2/third_party/eigen/Eigen/src/plugins/ReshapedMethods.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 19:54:44.103574 ml_dtypes-0.4.0b1/
+-rw-r--r--   0 runner    (1001) docker     (127)      301 2024-03-12 19:54:35.000000 ml_dtypes-0.4.0b1/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-03-12 19:54:35.000000 ml_dtypes-0.4.0b1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    16726 2024-03-12 19:54:35.000000 ml_dtypes-0.4.0b1/LICENSE.eigen
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-03-12 19:54:35.000000 ml_dtypes-0.4.0b1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    19735 2024-03-12 19:54:44.103574 ml_dtypes-0.4.0b1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6148 2024-03-12 19:54:35.000000 ml_dtypes-0.4.0b1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 19:54:44.067574 ml_dtypes-0.4.0b1/ml_dtypes/
+-rw-r--r--   0 runner    (1001) docker     (127)     1631 2024-03-12 19:54:35.000000 ml_dtypes-0.4.0b1/ml_dtypes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13506 2024-03-12 19:54:35.000000 ml_dtypes-0.4.0b1/ml_dtypes/_finfo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1589 2024-03-12 19:54:35.000000 ml_dtypes-0.4.0b1/ml_dtypes/_iinfo.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 19:54:44.067574 ml_dtypes-0.4.0b1/ml_dtypes/_src/
+-rw-r--r--   0 runner    (1001) docker     (127)     4370 2024-03-12 19:54:35.000000 ml_dtypes-0.4.0b1/ml_dtypes/_src/common.h
+-rw-r--r--   0 runner    (1001) docker     (127)    34972 2024-03-12 19:54:35.000000 ml_dtypes-0.4.0b1/ml_dtypes/_src/custom_float.h
+-rw-r--r--   0 runner    (1001) docker     (127)    12843 2024-03-12 19:54:35.000000 ml_dtypes-0.4.0b1/ml_dtypes/_src/dtypes.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    26816 2024-03-12 19:54:35.000000 ml_dtypes-0.4.0b1/ml_dtypes/_src/int4_numpy.h
+-rw-r--r--   0 runner    (1001) docker     (127)      909 2024-03-12 19:54:35.000000 ml_dtypes-0.4.0b1/ml_dtypes/_src/numpy.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1577 2024-03-12 19:54:35.000000 ml_dtypes-0.4.0b1/ml_dtypes/_src/numpy.h
+-rw-r--r--   0 runner    (1001) docker     (127)    19888 2024-03-12 19:54:35.000000 ml_dtypes-0.4.0b1/ml_dtypes/_src/ufuncs.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 19:54:44.067574 ml_dtypes-0.4.0b1/ml_dtypes/include/
+-rw-r--r--   0 runner    (1001) docker     (127)    51693 2024-03-12 19:54:35.000000 ml_dtypes-0.4.0b1/ml_dtypes/include/float8.h
+-rw-r--r--   0 runner    (1001) docker     (127)    10028 2024-03-12 19:54:35.000000 ml_dtypes-0.4.0b1/ml_dtypes/include/int4.h
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-12 19:54:35.000000 ml_dtypes-0.4.0b1/ml_dtypes/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 19:54:44.067574 ml_dtypes-0.4.0b1/ml_dtypes.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    19735 2024-03-12 19:54:44.000000 ml_dtypes-0.4.0b1/ml_dtypes.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10642 2024-03-12 19:54:44.000000 ml_dtypes-0.4.0b1/ml_dtypes.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-12 19:54:44.000000 ml_dtypes-0.4.0b1/ml_dtypes.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2024-03-12 19:54:44.000000 ml_dtypes-0.4.0b1/ml_dtypes.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-03-12 19:54:44.000000 ml_dtypes-0.4.0b1/ml_dtypes.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1633 2024-03-12 19:54:35.000000 ml_dtypes-0.4.0b1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-12 19:54:44.103574 ml_dtypes-0.4.0b1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2264 2024-03-12 19:54:35.000000 ml_dtypes-0.4.0b1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 19:54:44.063574 ml_dtypes-0.4.0b1/third_party/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 19:54:44.063574 ml_dtypes-0.4.0b1/third_party/eigen/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 19:54:44.067574 ml_dtypes-0.4.0b1/third_party/eigen/Eigen/
+-rw-r--r--   0 runner    (1001) docker     (127)    13374 2024-03-12 19:54:38.000000 ml_dtypes-0.4.0b1/third_party/eigen/Eigen/Core
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 19:54:44.063574 ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 19:54:44.079574 ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/
+-rw-r--r--   0 runner    (1001) docker     (127)    10790 2024-03-12 19:54:38.000000 ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/ArithmeticSequence.h
+-rw-r--r--   0 runner    (1001) docker     (127)    16400 2024-03-12 19:54:38.000000 ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/Array.h
+-rw-r--r--   0 runner    (1001) docker     (127)     8252 2024-03-12 19:54:38.000000 ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/ArrayBase.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6878 2024-03-12 19:54:38.000000 ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/ArrayWrapper.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2774 2024-03-12 19:54:38.000000 ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/Assign.h
+-rw-r--r--   0 runner    (1001) docker     (127)    41912 2024-03-12 19:54:38.000000 ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/AssignEvaluator.h
+-rw-r--r--   0 runner    (1001) docker     (127)    12508 2024-03-12 19:54:38.000000 ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/Assign_MKL.h
+-rw-r--r--   0 runner    (1001) docker     (127)    14072 2024-03-12 19:54:38.000000 ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/BandMatrix.h
+-rw-r--r--   0 runner    (1001) docker     (127)    19246 2024-03-12 19:54:38.000000 ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/Block.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6092 2024-03-12 19:54:38.000000 ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/CommaInitializer.h
+-rw-r--r--   0 runner    (1001) docker     (127)     7070 2024-03-12 19:54:38.000000 ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/ConditionEstimator.h
+-rw-r--r--   0 runner    (1001) docker     (127)    63843 2024-03-12 19:54:38.000000 ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/CoreEvaluators.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4781 2024-03-12 19:54:38.000000 ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/CoreIterators.h
+-rw-r--r--   0 runner    (1001) docker     (127)     7756 2024-03-12 19:54:38.000000 ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/CwiseBinaryOp.h
+-rw-r--r--   0 runner    (1001) docker     (127)    37759 2024-03-12 19:54:38.000000 ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/CwiseNullaryOp.h
+-rw-r--r--   0 runner    (1001) docker     (127)     8034 2024-03-12 19:54:38.000000 ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/CwiseTernaryOp.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3926 2024-03-12 19:54:38.000000 ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/CwiseUnaryOp.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6274 2024-03-12 19:54:38.000000 ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/CwiseUnaryView.h
+-rw-r--r--   0 runner    (1001) docker     (127)    32035 2024-03-12 19:54:38.000000 ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/DenseBase.h
+-rw-r--r--   0 runner    (1001) docker     (127)    24436 2024-03-12 19:54:38.000000 ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/DenseCoeffsBase.h
+-rw-r--r--   0 runner    (1001) docker     (127)    28937 2024-03-12 19:54:38.000000 ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/DenseStorage.h
+-rw-r--r--   0 runner    (1001) docker     (127)     9601 2024-03-12 19:54:38.000000 ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/Diagonal.h
+-rw-r--r--   0 runner    (1001) docker     (127)    18129 2024-03-12 19:54:38.000000 ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/DiagonalMatrix.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1024 2024-03-12 19:54:38.000000 ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/DiagonalProduct.h
+-rw-r--r--   0 runner    (1001) docker     (127)    11413 2024-03-12 19:54:38.000000 ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/Dot.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5877 2024-03-12 19:54:38.000000 ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/EigenBase.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4886 2024-03-12 19:54:38.000000 ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/ForceAlignedAccess.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5813 2024-03-12 19:54:38.000000 ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/Fuzzy.h
+-rw-r--r--   0 runner    (1001) docker     (127)    21625 2024-03-12 19:54:38.000000 ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/GeneralProduct.h
+-rw-r--r--   0 runner    (1001) docker     (127)    49384 2024-03-12 19:54:38.000000 ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/GenericPacketMath.h
+-rw-r--r--   0 runner    (1001) docker     (127)    12188 2024-03-12 19:54:38.000000 ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/GlobalFunctions.h
+-rw-r--r--   0 runner    (1001) docker     (127)     8402 2024-03-12 19:54:38.000000 ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/IO.h
+-rw-r--r--   0 runner    (1001) docker     (127)    10698 2024-03-12 19:54:38.000000 ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/IndexedView.h
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-03-12 19:54:38.000000 ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/InternalHeaderCheck.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3510 2024-03-12 19:54:38.000000 ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/Inverse.h
+-rw-r--r--   0 runner    (1001) docker     (127)     7127 2024-03-12 19:54:38.000000 ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/Map.h
+-rw-r--r--   0 runner    (1001) docker     (127)    11209 2024-03-12 19:54:38.000000 ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/MapBase.h
+-rw-r--r--   0 runner    (1001) docker     (127)    61532 2024-03-12 19:54:38.000000 ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/MathFunctions.h
+-rw-r--r--   0 runner    (1001) docker     (127)    13345 2024-03-12 19:54:38.000000 ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/MathFunctionsImpl.h
+-rw-r--r--   0 runner    (1001) docker     (127)    24419 2024-03-12 19:54:38.000000 ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/Matrix.h
+-rw-r--r--   0 runner    (1001) docker     (127)    23983 2024-03-12 19:54:38.000000 ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/MatrixBase.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3095 2024-03-12 19:54:38.000000 ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/NestByValue.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3656 2024-03-12 19:54:38.000000 ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/NoAlias.h
+-rw-r--r--   0 runner    (1001) docker     (127)    13346 2024-03-12 19:54:38.000000 ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/NumTraits.h
+-rw-r--r--   0 runner    (1001) docker     (127)     9281 2024-03-12 19:54:38.000000 ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/PartialReduxEvaluator.h
+-rw-r--r--   0 runner    (1001) docker     (127)    20771 2024-03-12 19:54:38.000000 ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/PermutationMatrix.h
+-rw-r--r--   0 runner    (1001) docker     (127)    48620 2024-03-12 19:54:38.000000 ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/PlainObjectBase.h
+-rw-r--r--   0 runner    (1001) docker     (127)     7314 2024-03-12 19:54:38.000000 ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/Product.h
+-rw-r--r--   0 runner    (1001) docker     (127)    55121 2024-03-12 19:54:38.000000 ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/ProductEvaluators.h
+-rw-r--r--   0 runner    (1001) docker     (127)     7748 2024-03-12 19:54:38.000000 ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/Random.h
+-rw-r--r--   0 runner    (1001) docker     (127)    19216 2024-03-12 19:54:38.000000 ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/Redux.h
+-rw-r--r--   0 runner    (1001) docker     (127)    17769 2024-03-12 19:54:38.000000 ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/Ref.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5635 2024-03-12 19:54:38.000000 ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/Replicate.h
+-rw-r--r--   0 runner    (1001) docker     (127)    16983 2024-03-12 19:54:38.000000 ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/Reshaped.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4317 2024-03-12 19:54:38.000000 ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/ReturnByValue.h
+-rw-r--r--   0 runner    (1001) docker     (127)     7552 2024-03-12 19:54:38.000000 ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/Reverse.h
+-rw-r--r--   0 runner    (1001) docker     (127)     7760 2024-03-12 19:54:38.000000 ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/Select.h
+-rw-r--r--   0 runner    (1001) docker     (127)    14908 2024-03-12 19:54:38.000000 ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/SelfAdjointView.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1733 2024-03-12 19:54:38.000000 ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/SelfCwiseBinaryOp.h
+-rw-r--r--   0 runner    (1001) docker     (127)    16006 2024-03-12 19:54:38.000000 ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/SkewSymmetricMatrix3.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6902 2024-03-12 19:54:38.000000 ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/Solve.h
+-rw-r--r--   0 runner    (1001) docker     (127)     9332 2024-03-12 19:54:38.000000 ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/SolveTriangular.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5967 2024-03-12 19:54:38.000000 ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/SolverBase.h
+-rw-r--r--   0 runner    (1001) docker     (127)     8689 2024-03-12 19:54:38.000000 ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/StableNorm.h
+-rw-r--r--   0 runner    (1001) docker     (127)    21245 2024-03-12 19:54:38.000000 ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/StlIterators.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4450 2024-03-12 19:54:38.000000 ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/Stride.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2801 2024-03-12 19:54:38.000000 ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/Swap.h
+-rw-r--r--   0 runner    (1001) docker     (127)    17669 2024-03-12 19:54:38.000000 ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/Transpose.h
+-rw-r--r--   0 runner    (1001) docker     (127)    13603 2024-03-12 19:54:38.000000 ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/Transpositions.h
+-rw-r--r--   0 runner    (1001) docker     (127)    38143 2024-03-12 19:54:38.000000 ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/TriangularMatrix.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3461 2024-03-12 19:54:38.000000 ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/VectorBlock.h
+-rw-r--r--   0 runner    (1001) docker     (127)    35183 2024-03-12 19:54:38.000000 ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/VectorwiseOp.h
+-rw-r--r--   0 runner    (1001) docker     (127)    35231 2024-03-12 19:54:38.000000 ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/Visitor.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 19:54:44.063574 ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/arch/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 19:54:44.083574 ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/arch/AVX/
+-rw-r--r--   0 runner    (1001) docker     (127)    14975 2024-03-12 19:54:38.000000 ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/arch/AVX/Complex.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6568 2024-03-12 19:54:38.000000 ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/arch/AVX/MathFunctions.h
+-rw-r--r--   0 runner    (1001) docker     (127)    83727 2024-03-12 19:54:38.000000 ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/arch/AVX/PacketMath.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2604 2024-03-12 19:54:38.000000 ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/arch/AVX/TypeCasting.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 19:54:44.083574 ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/arch/AVX512/
+-rw-r--r--   0 runner    (1001) docker     (127)    15797 2024-03-12 19:54:38.000000 ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/arch/AVX512/Complex.h
+-rw-r--r--   0 runner    (1001) docker     (127)    47758 2024-03-12 19:54:38.000000 ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/arch/AVX512/GemmKernel.h
+-rw-r--r--   0 runner    (1001) docker     (127)     9597 2024-03-12 19:54:38.000000 ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/arch/AVX512/MathFunctions.h
+-rw-r--r--   0 runner    (1001) docker     (127)   110036 2024-03-12 19:54:38.000000 ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/arch/AVX512/PacketMath.h
+-rw-r--r--   0 runner    (1001) docker     (127)    26497 2024-03-12 19:54:38.000000 ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/arch/AVX512/PacketMathFP16.h
+-rw-r--r--   0 runner    (1001) docker     (127)    56830 2024-03-12 19:54:38.000000 ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/arch/AVX512/TrsmKernel.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6072 2024-03-12 19:54:38.000000 ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/arch/AVX512/TypeCasting.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 19:54:44.083574 ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/arch/AltiVec/
+-rw-r--r--   0 runner    (1001) docker     (127)    20546 2024-03-12 19:54:38.000000 ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/arch/AltiVec/Complex.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3685 2024-03-12 19:54:38.000000 ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/arch/AltiVec/MathFunctions.h
+-rw-r--r--   0 runner    (1001) docker     (127)   129018 2024-03-12 19:54:38.000000 ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/arch/AltiVec/MatrixProduct.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6719 2024-03-12 19:54:38.000000 ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/arch/AltiVec/MatrixProductCommon.h
+-rw-r--r--   0 runner    (1001) docker     (127)    28128 2024-03-12 19:54:38.000000 ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/arch/AltiVec/MatrixProductMMA.h
+-rw-r--r--   0 runner    (1001) docker     (127)    15819 2024-03-12 19:54:38.000000 ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/arch/AltiVec/MatrixProductMMAbfloat16.h
+-rw-r--r--   0 runner    (1001) docker     (127)    91478 2024-03-12 19:54:38.000000 ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/arch/AltiVec/MatrixVectorProduct.h
+-rw-r--r--   0 runner    (1001) docker     (127)   119359 2024-03-12 19:54:38.000000 ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/arch/AltiVec/PacketMath.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 19:54:44.087574 ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/arch/Default/
+-rw-r--r--   0 runner    (1001) docker     (127)    34597 2024-03-12 19:54:38.000000 ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/arch/Default/BFloat16.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5291 2024-03-12 19:54:38.000000 ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/arch/Default/ConjHelper.h
+-rw-r--r--   0 runner    (1001) docker     (127)    94749 2024-03-12 19:54:38.000000 ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/arch/Default/GenericPacketMathFunctions.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4764 2024-03-12 19:54:38.000000 ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/arch/Default/GenericPacketMathFunctionsFwd.h
+-rw-r--r--   0 runner    (1001) docker     (127)    39550 2024-03-12 19:54:38.000000 ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/arch/Default/Half.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1746 2024-03-12 19:54:38.000000 ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/arch/Default/Settings.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3534 2024-03-12 19:54:38.000000 ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/arch/Default/TypeCasting.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 19:54:44.087574 ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/arch/GPU/
+-rw-r--r--   0 runner    (1001) docker     (127)    17981 2024-03-12 19:54:38.000000 ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/arch/GPU/Complex.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2735 2024-03-12 19:54:38.000000 ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/arch/GPU/MathFunctions.h
+-rw-r--r--   0 runner    (1001) docker     (127)    58287 2024-03-12 19:54:38.000000 ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/arch/GPU/PacketMath.h
+-rw-r--r--   0 runner    (1001) docker     (127)     9694 2024-03-12 19:54:38.000000 ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/arch/GPU/Tuple.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2297 2024-03-12 19:54:38.000000 ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/arch/GPU/TypeCasting.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 19:54:44.063574 ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/arch/HIP/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 19:54:44.087574 ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/arch/HIP/hcc/
+-rw-r--r--   0 runner    (1001) docker     (127)      691 2024-03-12 19:54:38.000000 ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/arch/HIP/hcc/math_constants.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 19:54:44.087574 ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/arch/MSA/
+-rw-r--r--   0 runner    (1001) docker     (127)    17448 2024-03-12 19:54:38.000000 ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/arch/MSA/Complex.h
+-rw-r--r--   0 runner    (1001) docker     (127)    16053 2024-03-12 19:54:38.000000 ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/arch/MSA/MathFunctions.h
+-rw-r--r--   0 runner    (1001) docker     (127)    33649 2024-03-12 19:54:38.000000 ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/arch/MSA/PacketMath.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 19:54:44.087574 ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/arch/NEON/
+-rw-r--r--   0 runner    (1001) docker     (127)    22034 2024-03-12 19:54:38.000000 ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/arch/NEON/Complex.h
+-rw-r--r--   0 runner    (1001) docker     (127)     9906 2024-03-12 19:54:38.000000 ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/arch/NEON/GeneralBlockPanelKernel.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4834 2024-03-12 19:54:38.000000 ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/arch/NEON/MathFunctions.h
+-rw-r--r--   0 runner    (1001) docker     (127)   194432 2024-03-12 19:54:38.000000 ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/arch/NEON/PacketMath.h
+-rw-r--r--   0 runner    (1001) docker     (127)    51898 2024-03-12 19:54:38.000000 ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/arch/NEON/TypeCasting.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1886 2024-03-12 19:54:38.000000 ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/arch/NEON/UnaryFunctors.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 19:54:44.091574 ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/arch/SSE/
+-rw-r--r--   0 runner    (1001) docker     (127)    13550 2024-03-12 19:54:38.000000 ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/arch/SSE/Complex.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5016 2024-03-12 19:54:38.000000 ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/arch/SSE/MathFunctions.h
+-rw-r--r--   0 runner    (1001) docker     (127)    72921 2024-03-12 19:54:38.000000 ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/arch/SSE/PacketMath.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3938 2024-03-12 19:54:38.000000 ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/arch/SSE/TypeCasting.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 19:54:44.091574 ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/arch/SVE/
+-rw-r--r--   0 runner    (1001) docker     (127)     1169 2024-03-12 19:54:38.000000 ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/arch/SVE/MathFunctions.h
+-rw-r--r--   0 runner    (1001) docker     (127)    21184 2024-03-12 19:54:38.000000 ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/arch/SVE/PacketMath.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1391 2024-03-12 19:54:38.000000 ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/arch/SVE/TypeCasting.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 19:54:44.091574 ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/arch/SYCL/
+-rw-r--r--   0 runner    (1001) docker     (127)     7468 2024-03-12 19:54:38.000000 ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/arch/SYCL/InteropHeaders.h
+-rw-r--r--   0 runner    (1001) docker     (127)    12579 2024-03-12 19:54:38.000000 ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/arch/SYCL/MathFunctions.h
+-rw-r--r--   0 runner    (1001) docker     (127)    16205 2024-03-12 19:54:38.000000 ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/arch/SYCL/PacketMath.h
+-rw-r--r--   0 runner    (1001) docker     (127)    21994 2024-03-12 19:54:38.000000 ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/arch/SYCL/SyclMemoryModel.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2669 2024-03-12 19:54:38.000000 ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/arch/SYCL/TypeCasting.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 19:54:44.091574 ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/arch/ZVector/
+-rw-r--r--   0 runner    (1001) docker     (127)    16373 2024-03-12 19:54:38.000000 ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/arch/ZVector/Complex.h
+-rw-r--r--   0 runner    (1001) docker     (127)     7927 2024-03-12 19:54:38.000000 ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/arch/ZVector/MathFunctions.h
+-rw-r--r--   0 runner    (1001) docker     (127)    36916 2024-03-12 19:54:38.000000 ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/arch/ZVector/PacketMath.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 19:54:44.091574 ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/functors/
+-rw-r--r--   0 runner    (1001) docker     (127)     6454 2024-03-12 19:54:38.000000 ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/functors/AssignmentFunctors.h
+-rw-r--r--   0 runner    (1001) docker     (127)    31940 2024-03-12 19:54:38.000000 ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/functors/BinaryFunctors.h
+-rw-r--r--   0 runner    (1001) docker     (127)     9534 2024-03-12 19:54:38.000000 ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/functors/NullaryFunctors.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4009 2024-03-12 19:54:38.000000 ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/functors/StlFunctors.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1786 2024-03-12 19:54:38.000000 ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/functors/TernaryFunctors.h
+-rw-r--r--   0 runner    (1001) docker     (127)    45622 2024-03-12 19:54:38.000000 ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/functors/UnaryFunctors.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 19:54:44.095574 ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/products/
+-rw-r--r--   0 runner    (1001) docker     (127)   140899 2024-03-12 19:54:38.000000 ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/products/GeneralBlockPanelKernel.h
+-rw-r--r--   0 runner    (1001) docker     (127)    19832 2024-03-12 19:54:38.000000 ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/products/GeneralMatrixMatrix.h
+-rw-r--r--   0 runner    (1001) docker     (127)    15819 2024-03-12 19:54:38.000000 ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/products/GeneralMatrixMatrixTriangular.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6973 2024-03-12 19:54:38.000000 ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/products/GeneralMatrixMatrixTriangular_BLAS.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5143 2024-03-12 19:54:38.000000 ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/products/GeneralMatrixMatrix_BLAS.h
+-rw-r--r--   0 runner    (1001) docker     (127)    21745 2024-03-12 19:54:38.000000 ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/products/GeneralMatrixVector.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6405 2024-03-12 19:54:38.000000 ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/products/GeneralMatrixVector_BLAS.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5252 2024-03-12 19:54:38.000000 ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/products/Parallelizer.h
+-rw-r--r--   0 runner    (1001) docker     (127)    21343 2024-03-12 19:54:38.000000 ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/products/SelfadjointMatrixMatrix.h
+-rw-r--r--   0 runner    (1001) docker     (127)    11607 2024-03-12 19:54:38.000000 ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/products/SelfadjointMatrixMatrix_BLAS.h
+-rw-r--r--   0 runner    (1001) docker     (127)     9893 2024-03-12 19:54:38.000000 ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/products/SelfadjointMatrixVector.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5246 2024-03-12 19:54:38.000000 ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/products/SelfadjointMatrixVector_BLAS.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6131 2024-03-12 19:54:38.000000 ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/products/SelfadjointProduct.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4077 2024-03-12 19:54:38.000000 ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/products/SelfadjointRank2Update.h
+-rw-r--r--   0 runner    (1001) docker     (127)    20980 2024-03-12 19:54:38.000000 ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/products/TriangularMatrixMatrix.h
+-rw-r--r--   0 runner    (1001) docker     (127)    13904 2024-03-12 19:54:38.000000 ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/products/TriangularMatrixMatrix_BLAS.h
+-rw-r--r--   0 runner    (1001) docker     (127)    14886 2024-03-12 19:54:38.000000 ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/products/TriangularMatrixVector.h
+-rw-r--r--   0 runner    (1001) docker     (127)    10608 2024-03-12 19:54:38.000000 ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/products/TriangularMatrixVector_BLAS.h
+-rw-r--r--   0 runner    (1001) docker     (127)    19090 2024-03-12 19:54:38.000000 ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/products/TriangularSolverMatrix.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6744 2024-03-12 19:54:38.000000 ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/products/TriangularSolverMatrix_BLAS.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5779 2024-03-12 19:54:38.000000 ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/products/TriangularSolverVector.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 19:54:44.099574 ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/util/
+-rw-r--r--   0 runner    (1001) docker     (127)     6211 2024-03-12 19:54:38.000000 ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/util/Assert.h
+-rw-r--r--   0 runner    (1001) docker     (127)    26278 2024-03-12 19:54:38.000000 ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/util/BlasUtil.h
+-rw-r--r--   0 runner    (1001) docker     (127)    19362 2024-03-12 19:54:38.000000 ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/util/ConfigureVectorization.h
+-rw-r--r--   0 runner    (1001) docker     (127)    22214 2024-03-12 19:54:38.000000 ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/util/Constants.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6223 2024-03-12 19:54:38.000000 ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/util/DisableStupidWarnings.h
+-rw-r--r--   0 runner    (1001) docker     (127)    15929 2024-03-12 19:54:38.000000 ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/util/ForwardDeclarations.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6273 2024-03-12 19:54:38.000000 ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/util/IndexedViewHelper.h
+-rw-r--r--   0 runner    (1001) docker     (127)     9567 2024-03-12 19:54:38.000000 ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/util/IntegralConstant.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4305 2024-03-12 19:54:38.000000 ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/util/MKL_support.h
+-rw-r--r--   0 runner    (1001) docker     (127)    48039 2024-03-12 19:54:38.000000 ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/util/Macros.h
+-rw-r--r--   0 runner    (1001) docker     (127)    49577 2024-03-12 19:54:38.000000 ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/util/Memory.h
+-rw-r--r--   0 runner    (1001) docker     (127)    20264 2024-03-12 19:54:38.000000 ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/util/Meta.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1387 2024-03-12 19:54:38.000000 ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/util/ReenableStupidWarnings.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1463 2024-03-12 19:54:38.000000 ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/util/ReshapedHelper.h
+-rw-r--r--   0 runner    (1001) docker     (127)     7810 2024-03-12 19:54:38.000000 ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/util/Serializer.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5496 2024-03-12 19:54:38.000000 ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/util/StaticAssert.h
+-rw-r--r--   0 runner    (1001) docker     (127)     9854 2024-03-12 19:54:38.000000 ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/util/SymbolicIndex.h
+-rw-r--r--   0 runner    (1001) docker     (127)    35298 2024-03-12 19:54:38.000000 ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/util/XprHelper.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 19:54:44.103574 ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)    13721 2024-03-12 19:54:38.000000 ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/plugins/ArrayCwiseBinaryOps.h
+-rw-r--r--   0 runner    (1001) docker     (127)    22938 2024-03-12 19:54:38.000000 ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/plugins/ArrayCwiseUnaryOps.h
+-rw-r--r--   0 runner    (1001) docker     (127)    58948 2024-03-12 19:54:38.000000 ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/plugins/BlockMethods.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6281 2024-03-12 19:54:38.000000 ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/plugins/CommonCwiseBinaryOps.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5927 2024-03-12 19:54:38.000000 ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/plugins/CommonCwiseUnaryOps.h
+-rw-r--r--   0 runner    (1001) docker     (127)    12022 2024-03-12 19:54:38.000000 ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/plugins/IndexedViewMethods.h
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-03-12 19:54:38.000000 ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/plugins/InternalHeaderCheck.h
+-rw-r--r--   0 runner    (1001) docker     (127)    16947 2024-03-12 19:54:38.000000 ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/plugins/MatrixCwiseBinaryOps.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4105 2024-03-12 19:54:38.000000 ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/plugins/MatrixCwiseUnaryOps.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6891 2024-03-12 19:54:38.000000 ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/plugins/ReshapedMethods.h
```

### Comparing `ml_dtypes-0.3.2/LICENSE` & `ml_dtypes-0.4.0b1/LICENSE`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.3.2/LICENSE.eigen` & `ml_dtypes-0.4.0b1/LICENSE.eigen`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.3.2/PKG-INFO` & `ml_dtypes-0.4.0b1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ml_dtypes
-Version: 0.3.2
+Version: 0.4.0b1
 Author-email: ml_dtypes authors <ml_dtypes@google.com>
 License: 
                                          Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `ml_dtypes-0.3.2/README.md` & `ml_dtypes-0.4.0b1/README.md`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.3.2/ml_dtypes/__init__.py` & `ml_dtypes-0.4.0b1/ml_dtypes/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-__version__ = '0.3.2'  # Keep in sync with pyproject.toml:version
+__version__ = '0.4.0b1'  # Keep in sync with pyproject.toml:version
 __all__ = [
     '__version__',
     'bfloat16',
     'finfo',
     'float8_e4m3b11fnuz',
     'float8_e4m3fn',
     'float8_e4m3fnuz',
```

### Comparing `ml_dtypes-0.3.2/ml_dtypes/_finfo.py` & `ml_dtypes-0.4.0b1/ml_dtypes/_finfo.py`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.3.2/ml_dtypes/_iinfo.py` & `ml_dtypes-0.4.0b1/ml_dtypes/_iinfo.py`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.3.2/ml_dtypes/_src/common.h` & `ml_dtypes-0.4.0b1/ml_dtypes/_src/common.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.3.2/ml_dtypes/_src/custom_float.h` & `ml_dtypes-0.4.0b1/ml_dtypes/_src/custom_float.h`

 * *Files 2% similar despite different names*

```diff
@@ -31,21 +31,25 @@
 #include <memory>   // NOLINT
 #include <sstream>  // NOLINT
 #include <vector>   // NOLINT
 // Place `<locale>` before <Python.h> to avoid a build failure in macOS.
 #include <Python.h>
 
 #include "Eigen/Core"
-#include "_src/common.h" // NOLINT
+#include "_src/common.h"  // NOLINT
 #include "_src/ufuncs.h"  // NOLINT
 
 #undef copysign  // TODO(ddunleavy): temporary fix for Windows bazel build
                  // Possible this has to do with numpy.h being included before
                  // system headers and in bfloat16.{cc,h}?
 
+#if NPY_ABI_VERSION < 0x02000000
+#define PyArray_DescrProto PyArray_Descr
+#endif
+
 namespace ml_dtypes {
 
 template <typename T>
 struct CustomFloatType {
   static int Dtype() { return npy_type; }
 
   // Registered numpy type ID. Global variable populated by the registration
@@ -55,21 +59,26 @@
   // Pointer to the python type object we are using. This is either a pointer
   // to type, if we choose to register it, or to the python type
   // registered by another system into NumPy.
   static PyObject* type_ptr;
 
   static PyNumberMethods number_methods;
   static PyArray_ArrFuncs arr_funcs;
-  static PyArray_Descr npy_descr;
+  static PyArray_DescrProto npy_descr_proto;
+  static PyArray_Descr* npy_descr;
 };
 
 template <typename T>
 int CustomFloatType<T>::npy_type = NPY_NOTYPE;
 template <typename T>
 PyObject* CustomFloatType<T>::type_ptr = nullptr;
+template <typename T>
+PyArray_DescrProto CustomFloatType<T>::npy_descr_proto;
+template <typename T>
+PyArray_Descr* CustomFloatType<T>::npy_descr = nullptr;
 
 // Representation of a Python custom float object.
 template <typename T>
 struct PyCustomFloat {
   PyObject_HEAD;  // Python object header
   T value;
 };
@@ -393,32 +402,34 @@
 }
 
 // Numpy support
 template <typename T>
 PyArray_ArrFuncs CustomFloatType<T>::arr_funcs;
 
 template <typename T>
-PyArray_Descr CustomFloatType<T>::npy_descr = {
-    PyObject_HEAD_INIT(nullptr)
-    /*typeobj=*/nullptr,  // Filled in later
-    /*kind=*/TypeDescriptor<T>::kNpyDescrKind,
-    /*type=*/TypeDescriptor<T>::kNpyDescrType,
-    /*byteorder=*/TypeDescriptor<T>::kNpyDescrByteorder,
-    /*flags=*/NPY_NEEDS_PYAPI | NPY_USE_SETITEM,
-    /*type_num=*/0,
-    /*elsize=*/sizeof(T),
-    /*alignment=*/alignof(T),
-    /*subarray=*/nullptr,
-    /*fields=*/nullptr,
-    /*names=*/nullptr,
-    /*f=*/&CustomFloatType<T>::arr_funcs,
-    /*metadata=*/nullptr,
-    /*c_metadata=*/nullptr,
-    /*hash=*/-1,  // -1 means "not computed yet".
-};
+PyArray_DescrProto GetCustomFloatDescrProto() {
+  return {
+      PyObject_HEAD_INIT(nullptr)
+      /*typeobj=*/nullptr,  // Filled in later
+      /*kind=*/TypeDescriptor<T>::kNpyDescrKind,
+      /*type=*/TypeDescriptor<T>::kNpyDescrType,
+      /*byteorder=*/TypeDescriptor<T>::kNpyDescrByteorder,
+      /*flags=*/NPY_NEEDS_PYAPI | NPY_USE_SETITEM,
+      /*type_num=*/0,
+      /*elsize=*/sizeof(T),
+      /*alignment=*/alignof(T),
+      /*subarray=*/nullptr,
+      /*fields=*/nullptr,
+      /*names=*/nullptr,
+      /*f=*/&CustomFloatType<T>::arr_funcs,
+      /*metadata=*/nullptr,
+      /*c_metadata=*/nullptr,
+      /*hash=*/-1,  // -1 means "not computed yet".
+  };
+}
 
 // Implementations of NumPy array methods.
 
 template <typename T>
 PyObject* NPyCustomFloat_GetItem(void* data, void* arr) {
   T x;
   memcpy(&x, data, sizeof(T));
@@ -624,16 +635,16 @@
 template <typename T, typename OtherT>
 bool RegisterCustomFloatCast(int numpy_type = TypeDescriptor<OtherT>::Dtype()) {
   PyArray_Descr* descr = PyArray_DescrFromType(numpy_type);
   if (PyArray_RegisterCastFunc(descr, TypeDescriptor<T>::Dtype(),
                                NPyCast<OtherT, T>) < 0) {
     return false;
   }
-  if (PyArray_RegisterCastFunc(&CustomFloatType<T>::npy_descr,
-                               numpy_type, NPyCast<T, OtherT>) < 0) {
+  if (PyArray_RegisterCastFunc(CustomFloatType<T>::npy_descr, numpy_type,
+                               NPyCast<T, OtherT>) < 0) {
     return false;
   }
   return true;
 }
 
 template <typename T>
 bool RegisterFloatCasts() {
@@ -693,35 +704,35 @@
     return false;
   }
   if (!RegisterCustomFloatCast<T, std::complex<long double>>(NPY_CLONGDOUBLE)) {
     return false;
   }
 
   // Safe casts from T to other types
-  if (PyArray_RegisterCanCast(&TypeDescriptor<T>::npy_descr, NPY_FLOAT,
+  if (PyArray_RegisterCanCast(TypeDescriptor<T>::npy_descr, NPY_FLOAT,
                               NPY_NOSCALAR) < 0) {
     return false;
   }
-  if (PyArray_RegisterCanCast(&TypeDescriptor<T>::npy_descr, NPY_DOUBLE,
+  if (PyArray_RegisterCanCast(TypeDescriptor<T>::npy_descr, NPY_DOUBLE,
                               NPY_NOSCALAR) < 0) {
     return false;
   }
-  if (PyArray_RegisterCanCast(&TypeDescriptor<T>::npy_descr, NPY_LONGDOUBLE,
+  if (PyArray_RegisterCanCast(TypeDescriptor<T>::npy_descr, NPY_LONGDOUBLE,
                               NPY_NOSCALAR) < 0) {
     return false;
   }
-  if (PyArray_RegisterCanCast(&TypeDescriptor<T>::npy_descr, NPY_CFLOAT,
+  if (PyArray_RegisterCanCast(TypeDescriptor<T>::npy_descr, NPY_CFLOAT,
                               NPY_NOSCALAR) < 0) {
     return false;
   }
-  if (PyArray_RegisterCanCast(&TypeDescriptor<T>::npy_descr, NPY_CDOUBLE,
+  if (PyArray_RegisterCanCast(TypeDescriptor<T>::npy_descr, NPY_CDOUBLE,
                               NPY_NOSCALAR) < 0) {
     return false;
   }
-  if (PyArray_RegisterCanCast(&TypeDescriptor<T>::npy_descr, NPY_CLONGDOUBLE,
+  if (PyArray_RegisterCanCast(TypeDescriptor<T>::npy_descr, NPY_CLONGDOUBLE,
                               NPY_NOSCALAR) < 0) {
     return false;
   }
 
   // Safe casts to T from other types
   if (PyArray_RegisterCanCast(PyArray_DescrFromType(NPY_BOOL),
                               TypeDescriptor<T>::Dtype(), NPY_NOSCALAR) < 0) {
@@ -917,44 +928,54 @@
   arr_funcs.nonzero = NPyCustomFloat_NonZero<T>;
   arr_funcs.fill = NPyCustomFloat_Fill<T>;
   arr_funcs.dotfunc = NPyCustomFloat_DotFunc<T>;
   arr_funcs.compare = NPyCustomFloat_CompareFunc<T>;
   arr_funcs.argmax = NPyCustomFloat_ArgMaxFunc<T>;
   arr_funcs.argmin = NPyCustomFloat_ArgMinFunc<T>;
 
-#if PY_VERSION_HEX < 0x030900A4 && !defined(Py_SET_TYPE)
-  Py_TYPE(&CustomFloatType<T>::npy_descr) = &PyArrayDescr_Type;
-#else
-  Py_SET_TYPE(&CustomFloatType<T>::npy_descr, &PyArrayDescr_Type);
-#endif
-  TypeDescriptor<T>::npy_descr.typeobj = type;
-
-  TypeDescriptor<T>::npy_type =
-      PyArray_RegisterDataType(&CustomFloatType<T>::npy_descr);
-  if (TypeDescriptor<T>::Dtype() < 0) {
+  // This is messy, but that's because the NumPy 2.0 API transition is messy.
+  // Before 2.0, NumPy assumes we'll keep the descriptor passed in to
+  // RegisterDataType alive, because it stores its pointer.
+  // After 2.0, the proto and descriptor types diverge, and NumPy allocates
+  // and manages the lifetime of the descriptor itself.
+  PyArray_DescrProto& descr_proto = CustomFloatType<T>::npy_descr_proto;
+  descr_proto = GetCustomFloatDescrProto<T>();
+  Py_SET_TYPE(&descr_proto, &PyArrayDescr_Type);
+  descr_proto.typeobj = type;
+
+  TypeDescriptor<T>::npy_type = PyArray_RegisterDataType(&descr_proto);
+  if (TypeDescriptor<T>::npy_type < 0) {
     return false;
   }
 
+  // TODO(phawkins): We intentionally leak the pointer to the descriptor.
+  // Implement a better module destructor to handle this.
+  CustomFloatType<T>::npy_descr =
+      PyArray_DescrFromType(TypeDescriptor<T>::npy_type);
+
   Safe_PyObjectPtr typeDict_obj =
       make_safe(PyObject_GetAttrString(numpy, "sctypeDict"));
   if (!typeDict_obj) return false;
   // Add the type object to `numpy.typeDict`: that makes
   // `numpy.dtype(type_name)` work.
   if (PyDict_SetItemString(typeDict_obj.get(), TypeDescriptor<T>::kTypeName,
                            TypeDescriptor<T>::type_ptr) < 0) {
     return false;
   }
 
   // Support dtype(type_name)
-  if (PyObject_SetAttrString(TypeDescriptor<T>::type_ptr, "dtype",
-                             reinterpret_cast<PyObject*>(
-                                 &CustomFloatType<T>::npy_descr)) <
-      0) {
+  if (PyObject_SetAttrString(
+          TypeDescriptor<T>::type_ptr, "dtype",
+          reinterpret_cast<PyObject*>(CustomFloatType<T>::npy_descr)) < 0) {
     return false;
   }
 
   return RegisterFloatCasts<T>() && RegisterFloatUFuncs<T>(numpy);
 }
 
 }  // namespace ml_dtypes
 
+#if NPY_ABI_VERSION < 0x02000000
+#undef PyArray_DescrProto
+#endif
+
 #endif  // ML_DTYPES_CUSTOM_FLOAT_H_
```

### Comparing `ml_dtypes-0.3.2/ml_dtypes/_src/dtypes.cc` & `ml_dtypes-0.4.0b1/ml_dtypes/_src/dtypes.cc`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.3.2/ml_dtypes/_src/int4_numpy.h` & `ml_dtypes-0.4.0b1/ml_dtypes/_src/int4_numpy.h`

 * *Files 2% similar despite different names*

```diff
@@ -25,14 +25,18 @@
 // clang-format on
 
 #include "Eigen/Core"
 #include "_src/common.h"  // NOLINT
 #include "_src/ufuncs.h"  // NOLINT
 #include "include/int4.h"
 
+#if NPY_ABI_VERSION < 0x02000000
+#define PyArray_DescrProto PyArray_Descr
+#endif
+
 namespace ml_dtypes {
 
 constexpr char kOutOfRange[] = "out of range value cannot be converted to int4";
 
 template <typename T>
 struct Int4TypeDescriptor {
   static int Dtype() { return npy_type; }
@@ -44,21 +48,26 @@
   // Pointer to the python type object we are using. This is either a pointer
   // to type, if we choose to register it, or to the python type
   // registered by another system into NumPy.
   static PyObject* type_ptr;
 
   static PyNumberMethods number_methods;
   static PyArray_ArrFuncs arr_funcs;
-  static PyArray_Descr npy_descr;
+  static PyArray_DescrProto npy_descr_proto;
+  static PyArray_Descr* npy_descr;
 };
 
 template <typename T>
 int Int4TypeDescriptor<T>::npy_type = NPY_NOTYPE;
 template <typename T>
 PyObject* Int4TypeDescriptor<T>::type_ptr = nullptr;
+template <typename T>
+PyArray_DescrProto Int4TypeDescriptor<T>::npy_descr_proto;
+template <typename T>
+PyArray_Descr* Int4TypeDescriptor<T>::npy_descr = nullptr;
 
 // Representation of a Python custom integer object.
 template <typename T>
 struct PyInt4 {
   PyObject_HEAD;  // Python object header
   T value;
 };
@@ -402,32 +411,34 @@
 }
 
 // Numpy support
 template <typename T>
 PyArray_ArrFuncs Int4TypeDescriptor<T>::arr_funcs;
 
 template <typename T>
-PyArray_Descr Int4TypeDescriptor<T>::npy_descr = {
-    PyObject_HEAD_INIT(nullptr)
-    /*typeobj=*/nullptr,  // Filled in later
-    /*kind=*/TypeDescriptor<T>::kNpyDescrKind,
-    /*type=*/TypeDescriptor<T>::kNpyDescrType,
-    /*byteorder=*/TypeDescriptor<T>::kNpyDescrByteorder,
-    /*flags=*/NPY_NEEDS_PYAPI | NPY_USE_SETITEM,
-    /*type_num=*/0,
-    /*elsize=*/sizeof(T),
-    /*alignment=*/alignof(T),
-    /*subarray=*/nullptr,
-    /*fields=*/nullptr,
-    /*names=*/nullptr,
-    /*f=*/&Int4TypeDescriptor<T>::arr_funcs,
-    /*metadata=*/nullptr,
-    /*c_metadata=*/nullptr,
-    /*hash=*/-1,  // -1 means "not computed yet".
-};
+PyArray_DescrProto GetInt4DescrProto() {
+  return {
+      PyObject_HEAD_INIT(nullptr)
+      /*typeobj=*/nullptr,  // Filled in later
+      /*kind=*/TypeDescriptor<T>::kNpyDescrKind,
+      /*type=*/TypeDescriptor<T>::kNpyDescrType,
+      /*byteorder=*/TypeDescriptor<T>::kNpyDescrByteorder,
+      /*flags=*/NPY_NEEDS_PYAPI | NPY_USE_SETITEM,
+      /*type_num=*/0,
+      /*elsize=*/sizeof(T),
+      /*alignment=*/alignof(T),
+      /*subarray=*/nullptr,
+      /*fields=*/nullptr,
+      /*names=*/nullptr,
+      /*f=*/&Int4TypeDescriptor<T>::arr_funcs,
+      /*metadata=*/nullptr,
+      /*c_metadata=*/nullptr,
+      /*hash=*/-1,  // -1 means "not computed yet".
+  };
+}
 
 // Implementations of NumPy array methods.
 
 template <typename T>
 PyObject* NPyInt4_GetItem(void* data, void* arr) {
   T x;
   memcpy(&x, data, sizeof(T));
@@ -602,15 +613,15 @@
 template <typename T, typename OtherT>
 bool RegisterCustomIntCast(int numpy_type = TypeDescriptor<OtherT>::Dtype()) {
   PyArray_Descr* descr = PyArray_DescrFromType(numpy_type);
   if (PyArray_RegisterCastFunc(descr, TypeDescriptor<T>::Dtype(),
                                IntegerCast<OtherT, T>) < 0) {
     return false;
   }
-  if (PyArray_RegisterCastFunc(&Int4TypeDescriptor<T>::npy_descr, numpy_type,
+  if (PyArray_RegisterCastFunc(Int4TypeDescriptor<T>::npy_descr, numpy_type,
                                IntegerCast<T, OtherT>) < 0) {
     return false;
   }
   return true;
 }
 
 template <typename T>
@@ -670,74 +681,74 @@
     return false;
   }
   if (!RegisterCustomIntCast<T, std::complex<long double>>(NPY_CLONGDOUBLE)) {
     return false;
   }
 
   // Safe casts from T to other types
-  if (PyArray_RegisterCanCast(&TypeDescriptor<T>::npy_descr, NPY_INT8,
+  if (PyArray_RegisterCanCast(TypeDescriptor<T>::npy_descr, NPY_INT8,
                               NPY_NOSCALAR) < 0) {
     return false;
   }
-  if (PyArray_RegisterCanCast(&TypeDescriptor<T>::npy_descr, NPY_INT16,
+  if (PyArray_RegisterCanCast(TypeDescriptor<T>::npy_descr, NPY_INT16,
                               NPY_NOSCALAR) < 0) {
     return false;
   }
-  if (PyArray_RegisterCanCast(&TypeDescriptor<T>::npy_descr, NPY_INT32,
+  if (PyArray_RegisterCanCast(TypeDescriptor<T>::npy_descr, NPY_INT32,
                               NPY_NOSCALAR) < 0) {
     return false;
   }
-  if (PyArray_RegisterCanCast(&TypeDescriptor<T>::npy_descr, NPY_INT64,
+  if (PyArray_RegisterCanCast(TypeDescriptor<T>::npy_descr, NPY_INT64,
                               NPY_NOSCALAR) < 0) {
     return false;
   }
 
   if (std::is_same_v<uint4, T>) {
-    if (PyArray_RegisterCanCast(&TypeDescriptor<T>::npy_descr, NPY_UINT8,
+    if (PyArray_RegisterCanCast(TypeDescriptor<T>::npy_descr, NPY_UINT8,
                                 NPY_NOSCALAR) < 0) {
       return false;
     }
-    if (PyArray_RegisterCanCast(&TypeDescriptor<T>::npy_descr, NPY_UINT16,
+    if (PyArray_RegisterCanCast(TypeDescriptor<T>::npy_descr, NPY_UINT16,
                                 NPY_NOSCALAR) < 0) {
       return false;
     }
-    if (PyArray_RegisterCanCast(&TypeDescriptor<T>::npy_descr, NPY_UINT32,
+    if (PyArray_RegisterCanCast(TypeDescriptor<T>::npy_descr, NPY_UINT32,
                                 NPY_NOSCALAR) < 0) {
       return false;
     }
-    if (PyArray_RegisterCanCast(&TypeDescriptor<T>::npy_descr, NPY_UINT64,
+    if (PyArray_RegisterCanCast(TypeDescriptor<T>::npy_descr, NPY_UINT64,
                                 NPY_NOSCALAR) < 0) {
       return false;
     }
   }
-  if (PyArray_RegisterCanCast(&TypeDescriptor<T>::npy_descr, NPY_HALF,
+  if (PyArray_RegisterCanCast(TypeDescriptor<T>::npy_descr, NPY_HALF,
                               NPY_NOSCALAR) < 0) {
     return false;
   }
-  if (PyArray_RegisterCanCast(&TypeDescriptor<T>::npy_descr, NPY_FLOAT,
+  if (PyArray_RegisterCanCast(TypeDescriptor<T>::npy_descr, NPY_FLOAT,
                               NPY_NOSCALAR) < 0) {
     return false;
   }
-  if (PyArray_RegisterCanCast(&TypeDescriptor<T>::npy_descr, NPY_DOUBLE,
+  if (PyArray_RegisterCanCast(TypeDescriptor<T>::npy_descr, NPY_DOUBLE,
                               NPY_NOSCALAR) < 0) {
     return false;
   }
-  if (PyArray_RegisterCanCast(&TypeDescriptor<T>::npy_descr, NPY_LONGDOUBLE,
+  if (PyArray_RegisterCanCast(TypeDescriptor<T>::npy_descr, NPY_LONGDOUBLE,
                               NPY_NOSCALAR) < 0) {
     return false;
   }
-  if (PyArray_RegisterCanCast(&TypeDescriptor<T>::npy_descr, NPY_CFLOAT,
+  if (PyArray_RegisterCanCast(TypeDescriptor<T>::npy_descr, NPY_CFLOAT,
                               NPY_NOSCALAR) < 0) {
     return false;
   }
-  if (PyArray_RegisterCanCast(&TypeDescriptor<T>::npy_descr, NPY_CDOUBLE,
+  if (PyArray_RegisterCanCast(TypeDescriptor<T>::npy_descr, NPY_CDOUBLE,
                               NPY_NOSCALAR) < 0) {
     return false;
   }
-  if (PyArray_RegisterCanCast(&TypeDescriptor<T>::npy_descr, NPY_CLONGDOUBLE,
+  if (PyArray_RegisterCanCast(TypeDescriptor<T>::npy_descr, NPY_CLONGDOUBLE,
                               NPY_NOSCALAR) < 0) {
     return false;
   }
 
   // Safe casts to T from other types
   if (PyArray_RegisterCanCast(PyArray_DescrFromType(NPY_BOOL),
                               TypeDescriptor<T>::Dtype(), NPY_NOSCALAR) < 0) {
@@ -817,43 +828,53 @@
   arr_funcs.nonzero = NPyInt4_NonZero<T>;
   arr_funcs.fill = NPyInt4_Fill<T>;
   arr_funcs.dotfunc = NPyInt4_DotFunc<T>;
   arr_funcs.compare = NPyInt4_CompareFunc<T>;
   arr_funcs.argmax = NPyInt4_ArgMaxFunc<T>;
   arr_funcs.argmin = NPyInt4_ArgMinFunc<T>;
 
-#if PY_VERSION_HEX < 0x030900A4 && !defined(Py_SET_TYPE)
-  Py_TYPE(&Int4TypeDescriptor<T>::npy_descr) = &PyArrayDescr_Type;
-#else
-  Py_SET_TYPE(&Int4TypeDescriptor<T>::npy_descr, &PyArrayDescr_Type);
-#endif
-  TypeDescriptor<T>::npy_descr.typeobj = type;
-
-  TypeDescriptor<T>::npy_type =
-      PyArray_RegisterDataType(&Int4TypeDescriptor<T>::npy_descr);
-  if (TypeDescriptor<T>::Dtype() < 0) {
-    return false;
-  }
+  // This is messy, but that's because the NumPy 2.0 API transition is messy.
+  // Before 2.0, NumPy assumes we'll keep the descriptor passed in to
+  // RegisterDataType alive, because it stores its pointer.
+  // After 2.0, the proto and descriptor types diverge, and NumPy allocates
+  // and manages the lifetime of the descriptor itself.
+  PyArray_DescrProto& descr_proto = Int4TypeDescriptor<T>::npy_descr_proto;
+  descr_proto = GetInt4DescrProto<T>();
+  Py_SET_TYPE(&descr_proto, &PyArrayDescr_Type);
+  descr_proto.typeobj = type;
+
+  TypeDescriptor<T>::npy_type = PyArray_RegisterDataType(&descr_proto);
+  if (TypeDescriptor<T>::npy_type < 0) {
+    return false;
+  }
+  // TODO(phawkins): We intentionally leak the pointer to the descriptor.
+  // Implement a better module destructor to handle this.
+  Int4TypeDescriptor<T>::npy_descr =
+      PyArray_DescrFromType(TypeDescriptor<T>::npy_type);
 
   Safe_PyObjectPtr typeDict_obj =
       make_safe(PyObject_GetAttrString(numpy, "sctypeDict"));
   if (!typeDict_obj) return false;
   // Add the type object to `numpy.typeDict`: that makes
   // `numpy.dtype(type_name)` work.
   if (PyDict_SetItemString(typeDict_obj.get(), TypeDescriptor<T>::kTypeName,
                            TypeDescriptor<T>::type_ptr) < 0) {
     return false;
   }
 
   // Support dtype(type_name)
   if (PyObject_SetAttrString(
           TypeDescriptor<T>::type_ptr, "dtype",
-          reinterpret_cast<PyObject*>(&Int4TypeDescriptor<T>::npy_descr)) < 0) {
+          reinterpret_cast<PyObject*>(Int4TypeDescriptor<T>::npy_descr)) < 0) {
     return false;
   }
 
   return RegisterInt4Casts<T>() && RegisterInt4UFuncs<T>(numpy);
 }
 
 }  // namespace ml_dtypes
 
+#if NPY_ABI_VERSION < 0x02000000
+#undef PyArray_DescrProto
+#endif
+
 #endif  // ML_DTYPES_INT4_NUMPY_H_
```

### Comparing `ml_dtypes-0.3.2/ml_dtypes/_src/numpy.cc` & `ml_dtypes-0.4.0b1/ml_dtypes/_src/numpy.cc`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.3.2/ml_dtypes/_src/numpy.h` & `ml_dtypes-0.4.0b1/ml_dtypes/_src/numpy.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.3.2/ml_dtypes/_src/ufuncs.h` & `ml_dtypes-0.4.0b1/ml_dtypes/_src/ufuncs.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.3.2/ml_dtypes/include/float8.h` & `ml_dtypes-0.4.0b1/ml_dtypes/include/float8.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.3.2/ml_dtypes/include/int4.h` & `ml_dtypes-0.4.0b1/ml_dtypes/include/int4.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.3.2/ml_dtypes.egg-info/PKG-INFO` & `ml_dtypes-0.4.0b1/ml_dtypes.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ml-dtypes
-Version: 0.3.2
+Version: 0.4.0b1
 Author-email: ml_dtypes authors <ml_dtypes@google.com>
 License: 
                                          Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `ml_dtypes-0.3.2/ml_dtypes.egg-info/SOURCES.txt` & `ml_dtypes-0.4.0b1/ml_dtypes.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.3.2/pyproject.toml` & `ml_dtypes-0.4.0b1/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "ml_dtypes"
-version = "0.3.2"  # Keep in sync with ml_dtypes/__init__.py:__version__
+version = "0.4.0b1"  # Keep in sync with ml_dtypes/__init__.py:__version__
 description = ""
 readme = "README.md"
 requires-python = ">=3.9"
 license = {file = "LICENSE"}
 authors = [{name = "ml_dtypes authors", email="ml_dtypes@google.com"}]
 classifiers = [
     "Programming Language :: Python :: 3",
@@ -44,18 +44,16 @@
 line-length = 80
 preview = true
 pyink-indentation = 2
 pyink-use-majority-quotes = true
 
 [build-system]
 requires = [
-    # Build with oldest supported numpy for each Python version.
-    "numpy~=1.21.2; python_version<'3.11'",
-    "numpy~=1.23.3; python_version>='3.11' and python_version<'3.12'",
-    "numpy~=1.26.0; python_version>='3.12'",
+    # TODO(jakevdp): update this to 2.0.0rc1 before final release
+    "numpy==2.0.0b1",
     "setuptools~=68.1.0",
 ]
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools]
 packages = ["ml_dtypes"]
 include-package-data = false
```

### Comparing `ml_dtypes-0.3.2/setup.py` & `ml_dtypes-0.4.0b1/setup.py`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.3.2/third_party/eigen/Eigen/Core` & `ml_dtypes-0.4.0b1/third_party/eigen/Eigen/Core`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/ArithmeticSequence.h` & `ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/ArithmeticSequence.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/Array.h` & `ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/Array.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/ArrayBase.h` & `ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/ArrayBase.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/ArrayWrapper.h` & `ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/ArrayWrapper.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/Assign.h` & `ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/Assign.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/AssignEvaluator.h` & `ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/AssignEvaluator.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/Assign_MKL.h` & `ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/Assign_MKL.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/BandMatrix.h` & `ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/BandMatrix.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/Block.h` & `ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/Block.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/CommaInitializer.h` & `ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/CommaInitializer.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/ConditionEstimator.h` & `ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/ConditionEstimator.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/CoreEvaluators.h` & `ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/CoreEvaluators.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/CoreIterators.h` & `ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/CoreIterators.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/CwiseBinaryOp.h` & `ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/CwiseBinaryOp.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/CwiseNullaryOp.h` & `ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/CwiseNullaryOp.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/CwiseTernaryOp.h` & `ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/CwiseTernaryOp.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/CwiseUnaryOp.h` & `ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/CwiseUnaryOp.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/CwiseUnaryView.h` & `ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/CwiseUnaryView.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/DenseBase.h` & `ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/DenseBase.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/DenseCoeffsBase.h` & `ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/DenseCoeffsBase.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/DenseStorage.h` & `ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/DenseStorage.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/Diagonal.h` & `ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/Diagonal.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/DiagonalMatrix.h` & `ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/DiagonalMatrix.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/DiagonalProduct.h` & `ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/DiagonalProduct.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/Dot.h` & `ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/Dot.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/EigenBase.h` & `ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/EigenBase.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/ForceAlignedAccess.h` & `ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/ForceAlignedAccess.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/Fuzzy.h` & `ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/Fuzzy.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/GeneralProduct.h` & `ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/GeneralProduct.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/GenericPacketMath.h` & `ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/GenericPacketMath.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/GlobalFunctions.h` & `ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/GlobalFunctions.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/IO.h` & `ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/IO.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/IndexedView.h` & `ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/IndexedView.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/Inverse.h` & `ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/Inverse.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/Map.h` & `ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/Map.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/MapBase.h` & `ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/MapBase.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/MathFunctions.h` & `ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/MathFunctions.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/MathFunctionsImpl.h` & `ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/MathFunctionsImpl.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/Matrix.h` & `ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/Matrix.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/MatrixBase.h` & `ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/MatrixBase.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/NestByValue.h` & `ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/NestByValue.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/NoAlias.h` & `ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/NoAlias.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/NumTraits.h` & `ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/NumTraits.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/PartialReduxEvaluator.h` & `ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/PartialReduxEvaluator.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/PermutationMatrix.h` & `ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/PermutationMatrix.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/PlainObjectBase.h` & `ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/PlainObjectBase.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/Product.h` & `ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/Product.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/ProductEvaluators.h` & `ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/ProductEvaluators.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/Random.h` & `ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/Random.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/Redux.h` & `ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/Redux.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/Ref.h` & `ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/Ref.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/Replicate.h` & `ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/Replicate.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/Reshaped.h` & `ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/Reshaped.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/ReturnByValue.h` & `ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/ReturnByValue.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/Reverse.h` & `ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/Reverse.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/Select.h` & `ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/Select.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/SelfAdjointView.h` & `ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/SelfAdjointView.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/SelfCwiseBinaryOp.h` & `ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/SelfCwiseBinaryOp.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/SkewSymmetricMatrix3.h` & `ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/SkewSymmetricMatrix3.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/Solve.h` & `ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/Solve.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/SolveTriangular.h` & `ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/SolveTriangular.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/SolverBase.h` & `ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/SolverBase.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/StableNorm.h` & `ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/StableNorm.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/StlIterators.h` & `ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/StlIterators.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/Stride.h` & `ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/Stride.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/Swap.h` & `ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/Swap.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/Transpose.h` & `ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/Transpose.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/Transpositions.h` & `ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/Transpositions.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/TriangularMatrix.h` & `ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/TriangularMatrix.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/VectorBlock.h` & `ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/VectorBlock.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/VectorwiseOp.h` & `ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/VectorwiseOp.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/Visitor.h` & `ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/Visitor.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/arch/AVX/Complex.h` & `ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/arch/AVX/Complex.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/arch/AVX/MathFunctions.h` & `ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/arch/AVX/MathFunctions.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/arch/AVX/PacketMath.h` & `ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/arch/AVX/PacketMath.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/arch/AVX/TypeCasting.h` & `ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/arch/AVX/TypeCasting.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/arch/AVX512/Complex.h` & `ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/arch/AVX512/Complex.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/arch/AVX512/GemmKernel.h` & `ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/arch/AVX512/GemmKernel.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/arch/AVX512/MathFunctions.h` & `ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/arch/AVX512/MathFunctions.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/arch/AVX512/PacketMath.h` & `ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/arch/AVX512/PacketMath.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/arch/AVX512/PacketMathFP16.h` & `ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/arch/AVX512/PacketMathFP16.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/arch/AVX512/TrsmKernel.h` & `ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/arch/AVX512/TrsmKernel.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/arch/AVX512/TypeCasting.h` & `ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/arch/AVX512/TypeCasting.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/arch/AltiVec/Complex.h` & `ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/arch/AltiVec/Complex.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/arch/AltiVec/MathFunctions.h` & `ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/arch/AltiVec/MathFunctions.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/arch/AltiVec/MatrixProduct.h` & `ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/arch/AltiVec/MatrixProduct.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/arch/AltiVec/MatrixProductCommon.h` & `ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/arch/AltiVec/MatrixProductCommon.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/arch/AltiVec/MatrixProductMMA.h` & `ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/arch/AltiVec/MatrixProductMMA.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/arch/AltiVec/MatrixProductMMAbfloat16.h` & `ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/arch/AltiVec/MatrixProductMMAbfloat16.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/arch/AltiVec/MatrixVectorProduct.h` & `ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/arch/AltiVec/MatrixVectorProduct.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/arch/AltiVec/PacketMath.h` & `ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/arch/AltiVec/PacketMath.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/arch/Default/BFloat16.h` & `ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/arch/Default/BFloat16.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/arch/Default/ConjHelper.h` & `ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/arch/Default/ConjHelper.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/arch/Default/GenericPacketMathFunctions.h` & `ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/arch/Default/GenericPacketMathFunctions.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/arch/Default/GenericPacketMathFunctionsFwd.h` & `ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/arch/Default/GenericPacketMathFunctionsFwd.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/arch/Default/Half.h` & `ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/arch/Default/Half.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/arch/Default/Settings.h` & `ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/arch/Default/Settings.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/arch/Default/TypeCasting.h` & `ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/arch/Default/TypeCasting.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/arch/GPU/Complex.h` & `ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/arch/GPU/Complex.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/arch/GPU/MathFunctions.h` & `ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/arch/GPU/MathFunctions.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/arch/GPU/PacketMath.h` & `ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/arch/GPU/PacketMath.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/arch/GPU/Tuple.h` & `ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/arch/GPU/Tuple.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/arch/GPU/TypeCasting.h` & `ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/arch/GPU/TypeCasting.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/arch/HIP/hcc/math_constants.h` & `ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/arch/HIP/hcc/math_constants.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/arch/MSA/Complex.h` & `ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/arch/MSA/Complex.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/arch/MSA/MathFunctions.h` & `ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/arch/MSA/MathFunctions.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/arch/MSA/PacketMath.h` & `ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/arch/MSA/PacketMath.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/arch/NEON/Complex.h` & `ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/arch/NEON/Complex.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/arch/NEON/GeneralBlockPanelKernel.h` & `ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/arch/NEON/GeneralBlockPanelKernel.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/arch/NEON/MathFunctions.h` & `ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/arch/NEON/MathFunctions.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/arch/NEON/PacketMath.h` & `ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/arch/NEON/PacketMath.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/arch/NEON/TypeCasting.h` & `ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/arch/NEON/TypeCasting.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/arch/NEON/UnaryFunctors.h` & `ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/arch/NEON/UnaryFunctors.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/arch/SSE/Complex.h` & `ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/arch/SSE/Complex.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/arch/SSE/MathFunctions.h` & `ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/arch/SSE/MathFunctions.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/arch/SSE/PacketMath.h` & `ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/arch/SSE/PacketMath.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/arch/SSE/TypeCasting.h` & `ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/arch/SSE/TypeCasting.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/arch/SVE/MathFunctions.h` & `ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/arch/SVE/MathFunctions.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/arch/SVE/PacketMath.h` & `ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/arch/SVE/PacketMath.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/arch/SVE/TypeCasting.h` & `ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/arch/SVE/TypeCasting.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/arch/SYCL/InteropHeaders.h` & `ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/arch/SYCL/InteropHeaders.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/arch/SYCL/MathFunctions.h` & `ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/arch/SYCL/MathFunctions.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/arch/SYCL/PacketMath.h` & `ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/arch/SYCL/PacketMath.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/arch/SYCL/SyclMemoryModel.h` & `ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/arch/SYCL/SyclMemoryModel.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/arch/SYCL/TypeCasting.h` & `ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/arch/SYCL/TypeCasting.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/arch/ZVector/Complex.h` & `ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/arch/ZVector/Complex.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/arch/ZVector/MathFunctions.h` & `ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/arch/ZVector/MathFunctions.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/arch/ZVector/PacketMath.h` & `ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/arch/ZVector/PacketMath.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/functors/AssignmentFunctors.h` & `ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/functors/AssignmentFunctors.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/functors/BinaryFunctors.h` & `ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/functors/BinaryFunctors.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/functors/NullaryFunctors.h` & `ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/functors/NullaryFunctors.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/functors/StlFunctors.h` & `ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/functors/StlFunctors.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/functors/TernaryFunctors.h` & `ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/functors/TernaryFunctors.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/functors/UnaryFunctors.h` & `ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/functors/UnaryFunctors.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/products/GeneralBlockPanelKernel.h` & `ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/products/GeneralBlockPanelKernel.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/products/GeneralMatrixMatrix.h` & `ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/products/GeneralMatrixMatrix.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/products/GeneralMatrixMatrixTriangular.h` & `ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/products/GeneralMatrixMatrixTriangular.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/products/GeneralMatrixMatrixTriangular_BLAS.h` & `ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/products/GeneralMatrixMatrixTriangular_BLAS.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/products/GeneralMatrixMatrix_BLAS.h` & `ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/products/GeneralMatrixMatrix_BLAS.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/products/GeneralMatrixVector.h` & `ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/products/GeneralMatrixVector.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/products/GeneralMatrixVector_BLAS.h` & `ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/products/GeneralMatrixVector_BLAS.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/products/Parallelizer.h` & `ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/products/Parallelizer.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/products/SelfadjointMatrixMatrix.h` & `ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/products/SelfadjointMatrixMatrix.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/products/SelfadjointMatrixMatrix_BLAS.h` & `ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/products/SelfadjointMatrixMatrix_BLAS.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/products/SelfadjointMatrixVector.h` & `ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/products/SelfadjointMatrixVector.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/products/SelfadjointMatrixVector_BLAS.h` & `ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/products/SelfadjointMatrixVector_BLAS.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/products/SelfadjointProduct.h` & `ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/products/SelfadjointProduct.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/products/SelfadjointRank2Update.h` & `ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/products/SelfadjointRank2Update.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/products/TriangularMatrixMatrix.h` & `ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/products/TriangularMatrixMatrix.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/products/TriangularMatrixMatrix_BLAS.h` & `ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/products/TriangularMatrixMatrix_BLAS.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/products/TriangularMatrixVector.h` & `ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/products/TriangularMatrixVector.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/products/TriangularMatrixVector_BLAS.h` & `ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/products/TriangularMatrixVector_BLAS.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/products/TriangularSolverMatrix.h` & `ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/products/TriangularSolverMatrix.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/products/TriangularSolverMatrix_BLAS.h` & `ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/products/TriangularSolverMatrix_BLAS.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/products/TriangularSolverVector.h` & `ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/products/TriangularSolverVector.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/util/Assert.h` & `ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/util/Assert.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/util/BlasUtil.h` & `ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/util/BlasUtil.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/util/ConfigureVectorization.h` & `ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/util/ConfigureVectorization.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/util/Constants.h` & `ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/util/Constants.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/util/DisableStupidWarnings.h` & `ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/util/DisableStupidWarnings.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/util/ForwardDeclarations.h` & `ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/util/ForwardDeclarations.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/util/IndexedViewHelper.h` & `ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/util/IndexedViewHelper.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/util/IntegralConstant.h` & `ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/util/IntegralConstant.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/util/MKL_support.h` & `ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/util/MKL_support.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/util/Macros.h` & `ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/util/Macros.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/util/Memory.h` & `ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/util/Memory.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/util/Meta.h` & `ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/util/Meta.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/util/ReenableStupidWarnings.h` & `ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/util/ReenableStupidWarnings.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/util/ReshapedHelper.h` & `ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/util/ReshapedHelper.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/util/Serializer.h` & `ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/util/Serializer.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/util/StaticAssert.h` & `ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/util/StaticAssert.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/util/SymbolicIndex.h` & `ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/util/SymbolicIndex.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.3.2/third_party/eigen/Eigen/src/Core/util/XprHelper.h` & `ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/Core/util/XprHelper.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.3.2/third_party/eigen/Eigen/src/plugins/ArrayCwiseBinaryOps.h` & `ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/plugins/ArrayCwiseBinaryOps.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.3.2/third_party/eigen/Eigen/src/plugins/ArrayCwiseUnaryOps.h` & `ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/plugins/ArrayCwiseUnaryOps.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.3.2/third_party/eigen/Eigen/src/plugins/BlockMethods.h` & `ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/plugins/BlockMethods.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.3.2/third_party/eigen/Eigen/src/plugins/CommonCwiseBinaryOps.h` & `ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/plugins/CommonCwiseBinaryOps.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.3.2/third_party/eigen/Eigen/src/plugins/CommonCwiseUnaryOps.h` & `ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/plugins/CommonCwiseUnaryOps.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.3.2/third_party/eigen/Eigen/src/plugins/IndexedViewMethods.h` & `ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/plugins/IndexedViewMethods.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.3.2/third_party/eigen/Eigen/src/plugins/MatrixCwiseBinaryOps.h` & `ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/plugins/MatrixCwiseBinaryOps.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.3.2/third_party/eigen/Eigen/src/plugins/MatrixCwiseUnaryOps.h` & `ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/plugins/MatrixCwiseUnaryOps.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.3.2/third_party/eigen/Eigen/src/plugins/ReshapedMethods.h` & `ml_dtypes-0.4.0b1/third_party/eigen/Eigen/src/plugins/ReshapedMethods.h`

 * *Files identical despite different names*

