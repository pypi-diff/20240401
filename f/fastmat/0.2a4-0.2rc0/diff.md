# Comparing `tmp/fastmat-0.2a4.tar.gz` & `tmp/fastmat-0.2rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/fastmat-0.2a4.tar", last modified: Fri Jan 18 18:35:31 2019, max compression
+gzip compressed data, was "fastmat-0.2rc0.tar", last modified: Wed Feb 17 11:29:15 2021, max compression
```

## Comparing `fastmat-0.2a4.tar` & `fastmat-0.2rc0.tar`

### file list

```diff
@@ -1,134 +1,153 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-01-18 18:35:31.000000 fastmat-0.2a4/
--rw-rw-r--   0 travis    (2000) travis    (2000)        6 2019-01-18 18:24:40.000000 fastmat-0.2a4/.version
--rwxrwxr-x   0 travis    (2000) travis    (2000)    11402 2019-01-18 18:24:40.000000 fastmat-0.2a4/LICENSE
--rwxrwxr-x   0 travis    (2000) travis    (2000)      241 2019-01-18 18:24:40.000000 fastmat-0.2a4/MANIFEST.in
--rw-rw-r--   0 travis    (2000) travis    (2000)     9281 2019-01-18 18:35:31.000000 fastmat-0.2a4/PKG-INFO
--rwxrwxr-x   0 travis    (2000) travis    (2000)     6944 2019-01-18 18:24:40.000000 fastmat-0.2a4/README.md
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-01-18 18:35:31.000000 fastmat-0.2a4/demo/
--rwxrwxr-x   0 travis    (2000) travis    (2000)     4549 2019-01-18 18:24:40.000000 fastmat-0.2a4/demo/compOmpIsta.py
--rwxrwxr-x   0 travis    (2000) travis    (2000)    30006 2019-01-18 18:24:40.000000 fastmat-0.2a4/demo/datenSAFT.mat
--rwxrwxr-x   0 travis    (2000) travis    (2000)     5780 2019-01-18 18:24:40.000000 fastmat-0.2a4/demo/datenSAFT.py
--rwxrwxr-x   0 travis    (2000) travis    (2000)     2959 2019-01-18 18:24:40.000000 fastmat-0.2a4/demo/edgeDetect.py
--rwxrwxr-x   0 travis    (2000) travis    (2000)     6894 2019-01-18 18:24:40.000000 fastmat-0.2a4/demo/head.png
--rwxrwxr-x   0 travis    (2000) travis    (2000)     4373 2019-01-18 18:24:40.000000 fastmat-0.2a4/demo/lowRankApprox.py
--rwxrwxr-x   0 travis    (2000) travis    (2000)    11137 2019-01-18 18:24:40.000000 fastmat-0.2a4/demo/matrixSAFT.py
--rwxrwxr-x   0 travis    (2000) travis    (2000)     4519 2019-01-18 18:24:40.000000 fastmat-0.2a4/demo/matrixSAFTmask.pyx
--rwxrwxr-x   0 travis    (2000) travis    (2000)     6719 2019-01-18 18:24:40.000000 fastmat-0.2a4/demo/sparseReco.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-01-18 18:35:31.000000 fastmat-0.2a4/doc/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-01-18 18:35:31.000000 fastmat-0.2a4/doc/algorithms/
--rw-rw-r--   0 travis    (2000) travis    (2000)      818 2019-01-18 18:24:40.000000 fastmat-0.2a4/doc/algorithms/Algorithm.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)      800 2019-01-18 18:24:40.000000 fastmat-0.2a4/doc/algorithms/FISTA.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)      796 2019-01-18 18:24:40.000000 fastmat-0.2a4/doc/algorithms/ISTA.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)      792 2019-01-18 18:24:40.000000 fastmat-0.2a4/doc/algorithms/OMP.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)      800 2019-01-18 18:24:40.000000 fastmat-0.2a4/doc/algorithms/STELA.rst
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-01-18 18:35:31.000000 fastmat-0.2a4/doc/classes/
--rw-rw-r--   0 travis    (2000) travis    (2000)      797 2019-01-18 18:24:40.000000 fastmat-0.2a4/doc/classes/BlockDiag.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)      785 2019-01-18 18:24:40.000000 fastmat-0.2a4/doc/classes/Blocks.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)      797 2019-01-18 18:24:40.000000 fastmat-0.2a4/doc/classes/Circulant.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)      777 2019-01-18 18:24:40.000000 fastmat-0.2a4/doc/classes/Diag.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)      801 2019-01-18 18:24:40.000000 fastmat-0.2a4/doc/classes/DiagBlocks.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)      773 2019-01-18 18:24:40.000000 fastmat-0.2a4/doc/classes/Eye.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)      789 2019-01-18 18:24:40.000000 fastmat-0.2a4/doc/classes/Fourier.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)      793 2019-01-18 18:24:40.000000 fastmat-0.2a4/doc/classes/Hadamard.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)      777 2019-01-18 18:24:40.000000 fastmat-0.2a4/doc/classes/Kron.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)      813 2019-01-18 18:24:40.000000 fastmat-0.2a4/doc/classes/LSFRCirculant.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)      789 2019-01-18 18:24:40.000000 fastmat-0.2a4/doc/classes/LowRank.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)      805 2019-01-18 18:24:40.000000 fastmat-0.2a4/doc/classes/MLCirculant.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)      801 2019-01-18 18:24:40.000000 fastmat-0.2a4/doc/classes/MLToeplitz.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)      809 2019-01-18 18:24:40.000000 fastmat-0.2a4/doc/classes/MLUltraSound.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)     1298 2019-01-18 18:24:40.000000 fastmat-0.2a4/doc/classes/Matrix.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)      781 2019-01-18 18:24:40.000000 fastmat-0.2a4/doc/classes/Outer.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)      801 2019-01-18 18:24:40.000000 fastmat-0.2a4/doc/classes/Parametric.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)      789 2019-01-18 18:24:40.000000 fastmat-0.2a4/doc/classes/Partial.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)      805 2019-01-18 18:24:40.000000 fastmat-0.2a4/doc/classes/Permutation.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)      801 2019-01-18 18:24:40.000000 fastmat-0.2a4/doc/classes/Polynomial.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)      789 2019-01-18 18:24:40.000000 fastmat-0.2a4/doc/classes/Product.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)      785 2019-01-18 18:24:40.000000 fastmat-0.2a4/doc/classes/Sparse.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)      773 2019-01-18 18:24:40.000000 fastmat-0.2a4/doc/classes/Sum.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)      793 2019-01-18 18:24:40.000000 fastmat-0.2a4/doc/classes/Toeplitz.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)      777 2019-01-18 18:24:40.000000 fastmat-0.2a4/doc/classes/Zero.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)     1760 2019-01-18 18:24:40.000000 fastmat-0.2a4/doc/classes.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)     4376 2019-01-18 18:24:40.000000 fastmat-0.2a4/doc/conf.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3033 2019-01-18 18:24:40.000000 fastmat-0.2a4/doc/index.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)     2347 2019-01-18 18:24:40.000000 fastmat-0.2a4/doc/scipy.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)      824 2019-01-18 18:24:40.000000 fastmat-0.2a4/doc/submod.rst
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-01-18 18:35:31.000000 fastmat-0.2a4/fastmat/
--rwxrwxr-x   0 travis    (2000) travis    (2000)     1166 2019-01-18 18:24:40.000000 fastmat-0.2a4/fastmat/BlockDiag.pxd
--rwxrwxr-x   0 travis    (2000) travis    (2000)     8908 2019-01-18 18:24:40.000000 fastmat-0.2a4/fastmat/BlockDiag.pyx
--rwxrwxr-x   0 travis    (2000) travis    (2000)     1750 2019-01-18 18:24:40.000000 fastmat-0.2a4/fastmat/Blocks.pxd
--rwxrwxr-x   0 travis    (2000) travis    (2000)    12189 2019-01-18 18:24:40.000000 fastmat-0.2a4/fastmat/Blocks.pyx
--rwxrwxr-x   0 travis    (2000) travis    (2000)     1355 2019-01-18 18:24:40.000000 fastmat-0.2a4/fastmat/Circulant.pxd
--rwxrwxr-x   0 travis    (2000) travis    (2000)    21895 2019-01-18 18:24:40.000000 fastmat-0.2a4/fastmat/Circulant.pyx
--rwxrwxr-x   0 travis    (2000) travis    (2000)     1385 2019-01-18 18:24:40.000000 fastmat-0.2a4/fastmat/Diag.pxd
--rwxrwxr-x   0 travis    (2000) travis    (2000)     6525 2019-01-18 18:24:40.000000 fastmat-0.2a4/fastmat/Diag.pyx
--rw-rw-r--   0 travis    (2000) travis    (2000)     1362 2019-01-18 18:24:40.000000 fastmat-0.2a4/fastmat/DiagBlocks.pxd
--rw-rw-r--   0 travis    (2000) travis    (2000)     6094 2019-01-18 18:24:40.000000 fastmat-0.2a4/fastmat/DiagBlocks.pyx
--rwxrwxr-x   0 travis    (2000) travis    (2000)     1092 2019-01-18 18:24:40.000000 fastmat-0.2a4/fastmat/Eye.pxd
--rwxrwxr-x   0 travis    (2000) travis    (2000)     4396 2019-01-18 18:24:40.000000 fastmat-0.2a4/fastmat/Eye.pyx
--rwxrwxr-x   0 travis    (2000) travis    (2000)     1528 2019-01-18 18:24:40.000000 fastmat-0.2a4/fastmat/Fourier.pxd
--rwxrwxr-x   0 travis    (2000) travis    (2000)     9846 2019-01-18 18:24:40.000000 fastmat-0.2a4/fastmat/Fourier.pyx
--rwxrwxr-x   0 travis    (2000) travis    (2000)     1407 2019-01-18 18:24:40.000000 fastmat-0.2a4/fastmat/Hadamard.pxd
--rwxrwxr-x   0 travis    (2000) travis    (2000)     9219 2019-01-18 18:24:40.000000 fastmat-0.2a4/fastmat/Hadamard.pyx
--rwxrwxr-x   0 travis    (2000) travis    (2000)     1267 2019-01-18 18:24:40.000000 fastmat-0.2a4/fastmat/Kron.pxd
--rwxrwxr-x   0 travis    (2000) travis    (2000)    15629 2019-01-18 18:24:40.000000 fastmat-0.2a4/fastmat/Kron.pyx
--rw-rw-r--   0 travis    (2000) travis    (2000)     1487 2019-01-18 18:24:40.000000 fastmat-0.2a4/fastmat/LFSRCirculant.pxd
--rw-rw-r--   0 travis    (2000) travis    (2000)    18972 2019-01-18 18:24:40.000000 fastmat-0.2a4/fastmat/LFSRCirculant.pyx
--rwxrwxr-x   0 travis    (2000) travis    (2000)     1436 2019-01-18 18:24:40.000000 fastmat-0.2a4/fastmat/LowRank.pxd
--rwxrwxr-x   0 travis    (2000) travis    (2000)     8361 2019-01-18 18:24:40.000000 fastmat-0.2a4/fastmat/LowRank.pyx
--rwxrwxr-x   0 travis    (2000) travis    (2000)     6692 2019-01-18 18:24:40.000000 fastmat-0.2a4/fastmat/Matrix.pxd
--rwxrwxr-x   0 travis    (2000) travis    (2000)    87196 2019-01-18 18:24:40.000000 fastmat-0.2a4/fastmat/Matrix.pyx
--rwxrwxr-x   0 travis    (2000) travis    (2000)     1649 2019-01-18 18:24:40.000000 fastmat-0.2a4/fastmat/Outer.pxd
--rwxrwxr-x   0 travis    (2000) travis    (2000)     7586 2019-01-18 18:24:40.000000 fastmat-0.2a4/fastmat/Outer.pyx
--rwxrwxr-x   0 travis    (2000) travis    (2000)     1908 2019-01-18 18:24:40.000000 fastmat-0.2a4/fastmat/Parametric.pxd
--rwxrwxr-x   0 travis    (2000) travis    (2000)    14132 2019-01-18 18:24:40.000000 fastmat-0.2a4/fastmat/Parametric.pyx
--rwxrwxr-x   0 travis    (2000) travis    (2000)     1313 2019-01-18 18:24:40.000000 fastmat-0.2a4/fastmat/Partial.pxd
--rwxrwxr-x   0 travis    (2000) travis    (2000)    13375 2019-01-18 18:24:40.000000 fastmat-0.2a4/fastmat/Partial.pyx
--rw-rw-r--   0 travis    (2000) travis    (2000)     1180 2019-01-18 18:24:40.000000 fastmat-0.2a4/fastmat/Permutation.pxd
--rw-rw-r--   0 travis    (2000) travis    (2000)     4508 2019-01-18 18:24:40.000000 fastmat-0.2a4/fastmat/Permutation.pyx
--rwxrwxr-x   0 travis    (2000) travis    (2000)     1407 2019-01-18 18:24:40.000000 fastmat-0.2a4/fastmat/Polynomial.pxd
--rwxrwxr-x   0 travis    (2000) travis    (2000)     7008 2019-01-18 18:24:40.000000 fastmat-0.2a4/fastmat/Polynomial.pyx
--rwxrwxr-x   0 travis    (2000) travis    (2000)     1242 2019-01-18 18:24:40.000000 fastmat-0.2a4/fastmat/Product.pxd
--rwxrwxr-x   0 travis    (2000) travis    (2000)    12473 2019-01-18 18:24:40.000000 fastmat-0.2a4/fastmat/Product.pyx
--rwxrwxr-x   0 travis    (2000) travis    (2000)     1318 2019-01-18 18:24:40.000000 fastmat-0.2a4/fastmat/Sparse.pxd
--rwxrwxr-x   0 travis    (2000) travis    (2000)     6885 2019-01-18 18:24:40.000000 fastmat-0.2a4/fastmat/Sparse.pyx
--rwxrwxr-x   0 travis    (2000) travis    (2000)     1155 2019-01-18 18:24:40.000000 fastmat-0.2a4/fastmat/Sum.pxd
--rwxrwxr-x   0 travis    (2000) travis    (2000)     7834 2019-01-18 18:24:40.000000 fastmat-0.2a4/fastmat/Sum.pyx
--rwxrwxr-x   0 travis    (2000) travis    (2000)     1592 2019-01-18 18:24:40.000000 fastmat-0.2a4/fastmat/Toeplitz.pxd
--rwxrwxr-x   0 travis    (2000) travis    (2000)    35078 2019-01-18 18:24:40.000000 fastmat-0.2a4/fastmat/Toeplitz.pyx
--rwxrwxr-x   0 travis    (2000) travis    (2000)     1097 2019-01-18 18:24:40.000000 fastmat-0.2a4/fastmat/Zero.pxd
--rwxrwxr-x   0 travis    (2000) travis    (2000)     4498 2019-01-18 18:24:40.000000 fastmat-0.2a4/fastmat/Zero.pyx
--rwxrwxr-x   0 travis    (2000) travis    (2000)     4059 2019-01-18 18:24:40.000000 fastmat-0.2a4/fastmat/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-01-18 18:35:31.000000 fastmat-0.2a4/fastmat/algorithms/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1056 2019-01-18 18:24:40.000000 fastmat-0.2a4/fastmat/algorithms/Algorithm.pxd
--rw-rw-r--   0 travis    (2000) travis    (2000)     5517 2019-01-18 18:24:40.000000 fastmat-0.2a4/fastmat/algorithms/Algorithm.pyx
--rw-rw-r--   0 travis    (2000) travis    (2000)     8831 2019-01-18 18:24:40.000000 fastmat-0.2a4/fastmat/algorithms/FISTA.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     8352 2019-01-18 18:24:40.000000 fastmat-0.2a4/fastmat/algorithms/ISTA.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1556 2019-01-18 18:24:40.000000 fastmat-0.2a4/fastmat/algorithms/OMP.pxd
--rw-rw-r--   0 travis    (2000) travis    (2000)    11368 2019-01-18 18:24:40.000000 fastmat-0.2a4/fastmat/algorithms/OMP.pyx
--rw-rw-r--   0 travis    (2000) travis    (2000)    11619 2019-01-18 18:24:40.000000 fastmat-0.2a4/fastmat/algorithms/STELA.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1222 2019-01-18 18:24:40.000000 fastmat-0.2a4/fastmat/algorithms/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-01-18 18:35:31.000000 fastmat-0.2a4/fastmat/core/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1228 2019-01-18 18:24:40.000000 fastmat-0.2a4/fastmat/core/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5965 2019-01-18 18:24:40.000000 fastmat-0.2a4/fastmat/core/calibration.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2314 2019-01-18 18:24:40.000000 fastmat-0.2a4/fastmat/core/cmath.pxd
--rw-rw-r--   0 travis    (2000) travis    (2000)    30826 2019-01-18 18:24:40.000000 fastmat-0.2a4/fastmat/core/cmath.pyx
--rw-rw-r--   0 travis    (2000) travis    (2000)     3894 2019-01-18 18:24:40.000000 fastmat-0.2a4/fastmat/core/resource.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1860 2019-01-18 18:24:40.000000 fastmat-0.2a4/fastmat/core/strides.pxd
--rw-rw-r--   0 travis    (2000) travis    (2000)    10176 2019-01-18 18:24:40.000000 fastmat-0.2a4/fastmat/core/strides.pyx
--rw-rw-r--   0 travis    (2000) travis    (2000)      874 2019-01-18 18:24:40.000000 fastmat-0.2a4/fastmat/core/types.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     4332 2019-01-18 18:24:40.000000 fastmat-0.2a4/fastmat/core/types.pxd
--rw-rw-r--   0 travis    (2000) travis    (2000)    10142 2019-01-18 18:24:40.000000 fastmat-0.2a4/fastmat/core/types.pyx
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-01-18 18:35:31.000000 fastmat-0.2a4/fastmat/inspect/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1167 2019-01-18 18:24:40.000000 fastmat-0.2a4/fastmat/inspect/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    24978 2019-01-18 18:24:40.000000 fastmat-0.2a4/fastmat/inspect/benchmark.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    30054 2019-01-18 18:24:40.000000 fastmat-0.2a4/fastmat/inspect/common.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    33370 2019-01-18 18:24:40.000000 fastmat-0.2a4/fastmat/inspect/test.py
--rwxrwxr-x   0 travis    (2000) travis    (2000)      247 2019-01-18 18:35:31.000000 fastmat-0.2a4/fastmat/version.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-01-18 18:35:31.000000 fastmat-0.2a4/fastmat.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)     9281 2019-01-18 18:35:31.000000 fastmat-0.2a4/fastmat.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)     2683 2019-01-18 18:35:31.000000 fastmat-0.2a4/fastmat.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2019-01-18 18:35:31.000000 fastmat-0.2a4/fastmat.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       56 2019-01-18 18:35:31.000000 fastmat-0.2a4/fastmat.egg-info/top_level.txt
--rwxrwxr-x   0 travis    (2000) travis    (2000)     7538 2019-01-18 18:24:40.000000 fastmat-0.2a4/makefile
--rwxrwxr-x   0 travis    (2000) travis    (2000)      220 2019-01-18 18:35:31.000000 fastmat-0.2a4/setup.cfg
--rwxrwxr-x   0 travis    (2000) travis    (2000)    11747 2019-01-18 18:24:40.000000 fastmat-0.2a4/setup.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-02-17 11:29:15.837078 fastmat-0.2rc0/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        7 2021-02-17 11:14:19.000000 fastmat-0.2rc0/.version
+-rwxrwxr-x   0 travis    (2000) travis    (2000)    11402 2021-02-17 11:14:19.000000 fastmat-0.2rc0/LICENSE
+-rwxrwxr-x   0 travis    (2000) travis    (2000)      241 2021-02-17 11:14:19.000000 fastmat-0.2rc0/MANIFEST.in
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9874 2021-02-17 11:29:15.837078 fastmat-0.2rc0/PKG-INFO
+-rwxrwxr-x   0 travis    (2000) travis    (2000)     7277 2021-02-17 11:14:19.000000 fastmat-0.2rc0/README.md
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-02-17 11:29:15.817078 fastmat-0.2rc0/doc/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-02-17 11:29:15.821078 fastmat-0.2rc0/doc/_static/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      235 2021-02-17 11:14:19.000000 fastmat-0.2rc0/doc/_static/custom.css
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-02-17 11:29:15.821078 fastmat-0.2rc0/doc/_static/gfx/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1150 2021-02-17 11:14:19.000000 fastmat-0.2rc0/doc/_static/gfx/logo_favicon.png
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5339 2021-02-17 11:14:19.000000 fastmat-0.2rc0/doc/_static/gfx/logo_long.png
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4965 2021-02-17 11:14:19.000000 fastmat-0.2rc0/doc/_static/gfx/logo_short.png
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-02-17 11:29:15.821078 fastmat-0.2rc0/doc/algorithms/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      818 2021-02-17 11:14:19.000000 fastmat-0.2rc0/doc/algorithms/Algorithm.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)      800 2021-02-17 11:14:19.000000 fastmat-0.2rc0/doc/algorithms/FISTA.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)      796 2021-02-17 11:14:19.000000 fastmat-0.2rc0/doc/algorithms/ISTA.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)      792 2021-02-17 11:14:19.000000 fastmat-0.2rc0/doc/algorithms/OMP.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)      800 2021-02-17 11:14:19.000000 fastmat-0.2rc0/doc/algorithms/STELA.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1102 2021-02-17 11:14:19.000000 fastmat-0.2rc0/doc/algorithms.rst
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-02-17 11:29:15.821078 fastmat-0.2rc0/doc/architecture/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      738 2021-02-17 11:14:19.000000 fastmat-0.2rc0/doc/architecture/algorithms.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)      935 2021-02-17 11:14:19.000000 fastmat-0.2rc0/doc/architecture/calibration.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)      914 2021-02-17 11:14:19.000000 fastmat-0.2rc0/doc/architecture/capi.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)      729 2021-02-17 11:14:19.000000 fastmat-0.2rc0/doc/architecture/classes.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1873 2021-02-17 11:14:19.000000 fastmat-0.2rc0/doc/architecture/scipy.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2173 2021-02-17 11:14:19.000000 fastmat-0.2rc0/doc/architecture/strides.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5844 2021-02-17 11:14:19.000000 fastmat-0.2rc0/doc/architecture/types.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)      944 2021-02-17 11:14:19.000000 fastmat-0.2rc0/doc/architecture.rst
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-02-17 11:29:15.825078 fastmat-0.2rc0/doc/classes/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      812 2021-02-17 11:14:19.000000 fastmat-0.2rc0/doc/classes/BlockDiag.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)      785 2021-02-17 11:14:19.000000 fastmat-0.2rc0/doc/classes/Blocks.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)      823 2021-02-17 11:14:19.000000 fastmat-0.2rc0/doc/classes/Circulant.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)      787 2021-02-17 11:14:19.000000 fastmat-0.2rc0/doc/classes/Diag.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)      811 2021-02-17 11:14:19.000000 fastmat-0.2rc0/doc/classes/DiagBlocks.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)      785 2021-02-17 11:14:19.000000 fastmat-0.2rc0/doc/classes/Eye.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)      791 2021-02-17 11:14:19.000000 fastmat-0.2rc0/doc/classes/Fourier.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)      795 2021-02-17 11:14:19.000000 fastmat-0.2rc0/doc/classes/Hadamard.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)      791 2021-02-17 11:14:19.000000 fastmat-0.2rc0/doc/classes/Kron.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)      817 2021-02-17 11:14:19.000000 fastmat-0.2rc0/doc/classes/LSFRCirculant.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)      793 2021-02-17 11:14:19.000000 fastmat-0.2rc0/doc/classes/LowRank.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)      795 2021-02-17 11:14:19.000000 fastmat-0.2rc0/doc/classes/Matrix.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)      785 2021-02-17 11:14:19.000000 fastmat-0.2rc0/doc/classes/Outer.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)      803 2021-02-17 11:14:19.000000 fastmat-0.2rc0/doc/classes/Parametric.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)      791 2021-02-17 11:14:19.000000 fastmat-0.2rc0/doc/classes/Partial.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)      807 2021-02-17 11:14:19.000000 fastmat-0.2rc0/doc/classes/Permutation.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)      803 2021-02-17 11:14:19.000000 fastmat-0.2rc0/doc/classes/Polynomial.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)      805 2021-02-17 11:14:19.000000 fastmat-0.2rc0/doc/classes/Product.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)      787 2021-02-17 11:14:19.000000 fastmat-0.2rc0/doc/classes/Sparse.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)      775 2021-02-17 11:14:19.000000 fastmat-0.2rc0/doc/classes/Sum.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)      819 2021-02-17 11:14:19.000000 fastmat-0.2rc0/doc/classes/Toeplitz.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1015 2021-02-17 11:14:19.000000 fastmat-0.2rc0/doc/classes/Transpose.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)      779 2021-02-17 11:14:19.000000 fastmat-0.2rc0/doc/classes/Zero.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1654 2021-02-17 11:14:19.000000 fastmat-0.2rc0/doc/classes.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4574 2021-02-17 11:14:19.000000 fastmat-0.2rc0/doc/conf.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-02-17 11:29:15.825078 fastmat-0.2rc0/doc/examples/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3837 2021-02-17 11:14:19.000000 fastmat-0.2rc0/doc/examples/compressed-sensing.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1081 2021-02-17 11:14:19.000000 fastmat-0.2rc0/doc/examples/compressed-sensing.rst
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-02-17 11:29:15.825078 fastmat-0.2rc0/doc/examples/example_scripts/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3081 2021-02-17 11:14:19.000000 fastmat-0.2rc0/doc/examples/example_scripts/cs_example.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1570 2021-02-17 11:14:19.000000 fastmat-0.2rc0/doc/examples/scipy-linear-operator.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)      851 2021-02-17 11:14:19.000000 fastmat-0.2rc0/doc/examples.rst
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-02-17 11:29:15.825078 fastmat-0.2rc0/doc/expansion/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      808 2021-02-17 11:14:19.000000 fastmat-0.2rc0/doc/expansion/implement.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)      818 2021-02-17 11:14:19.000000 fastmat-0.2rc0/doc/expansion/optimize.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1325 2021-02-17 11:14:19.000000 fastmat-0.2rc0/doc/expansion.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2842 2021-02-17 11:14:19.000000 fastmat-0.2rc0/doc/index.rst
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-02-17 11:29:15.825078 fastmat-0.2rc0/doc/inspection/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      794 2021-02-17 11:14:19.000000 fastmat-0.2rc0/doc/inspection/benchmark.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)      991 2021-02-17 11:14:19.000000 fastmat-0.2rc0/doc/inspection/test.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1968 2021-02-17 11:14:19.000000 fastmat-0.2rc0/doc/inspection.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1830 2021-02-17 11:14:19.000000 fastmat-0.2rc0/doc/references.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1522 2021-02-17 11:14:19.000000 fastmat-0.2rc0/doc/releases.rst
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-02-17 11:29:15.833078 fastmat-0.2rc0/fastmat/
+-rwxrwxr-x   0 travis    (2000) travis    (2000)     1166 2021-02-17 11:14:19.000000 fastmat-0.2rc0/fastmat/BlockDiag.pxd
+-rwxrwxr-x   0 travis    (2000) travis    (2000)     8994 2021-02-17 11:14:19.000000 fastmat-0.2rc0/fastmat/BlockDiag.pyx
+-rwxrwxr-x   0 travis    (2000) travis    (2000)     1750 2021-02-17 11:14:19.000000 fastmat-0.2rc0/fastmat/Blocks.pxd
+-rwxrwxr-x   0 travis    (2000) travis    (2000)    13286 2021-02-17 11:14:19.000000 fastmat-0.2rc0/fastmat/Blocks.pyx
+-rwxrwxr-x   0 travis    (2000) travis    (2000)     1355 2021-02-17 11:14:19.000000 fastmat-0.2rc0/fastmat/Circulant.pxd
+-rwxrwxr-x   0 travis    (2000) travis    (2000)    19586 2021-02-17 11:14:19.000000 fastmat-0.2rc0/fastmat/Circulant.pyx
+-rwxrwxr-x   0 travis    (2000) travis    (2000)     1385 2021-02-17 11:14:19.000000 fastmat-0.2rc0/fastmat/Diag.pxd
+-rwxrwxr-x   0 travis    (2000) travis    (2000)     6612 2021-02-17 11:14:19.000000 fastmat-0.2rc0/fastmat/Diag.pyx
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1362 2021-02-17 11:14:19.000000 fastmat-0.2rc0/fastmat/DiagBlocks.pxd
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6181 2021-02-17 11:14:19.000000 fastmat-0.2rc0/fastmat/DiagBlocks.pyx
+-rwxrwxr-x   0 travis    (2000) travis    (2000)     1092 2021-02-17 11:14:19.000000 fastmat-0.2rc0/fastmat/Eye.pxd
+-rwxrwxr-x   0 travis    (2000) travis    (2000)     4483 2021-02-17 11:14:19.000000 fastmat-0.2rc0/fastmat/Eye.pyx
+-rwxrwxr-x   0 travis    (2000) travis    (2000)     1528 2021-02-17 11:14:19.000000 fastmat-0.2rc0/fastmat/Fourier.pxd
+-rwxrwxr-x   0 travis    (2000) travis    (2000)    10431 2021-02-17 11:14:19.000000 fastmat-0.2rc0/fastmat/Fourier.pyx
+-rwxrwxr-x   0 travis    (2000) travis    (2000)     1407 2021-02-17 11:14:19.000000 fastmat-0.2rc0/fastmat/Hadamard.pxd
+-rwxrwxr-x   0 travis    (2000) travis    (2000)     9328 2021-02-17 11:14:19.000000 fastmat-0.2rc0/fastmat/Hadamard.pyx
+-rwxrwxr-x   0 travis    (2000) travis    (2000)     1267 2021-02-17 11:14:19.000000 fastmat-0.2rc0/fastmat/Kron.pxd
+-rwxrwxr-x   0 travis    (2000) travis    (2000)    15727 2021-02-17 11:14:19.000000 fastmat-0.2rc0/fastmat/Kron.pyx
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1494 2021-02-17 11:14:19.000000 fastmat-0.2rc0/fastmat/LFSRCirculant.pxd
+-rw-rw-r--   0 travis    (2000) travis    (2000)    19468 2021-02-17 11:14:19.000000 fastmat-0.2rc0/fastmat/LFSRCirculant.pyx
+-rwxrwxr-x   0 travis    (2000) travis    (2000)     1436 2021-02-17 11:14:19.000000 fastmat-0.2rc0/fastmat/LowRank.pxd
+-rwxrwxr-x   0 travis    (2000) travis    (2000)     8447 2021-02-17 11:14:19.000000 fastmat-0.2rc0/fastmat/LowRank.pyx
+-rwxrwxr-x   0 travis    (2000) travis    (2000)     7893 2021-02-17 11:14:19.000000 fastmat-0.2rc0/fastmat/Matrix.pxd
+-rwxrwxr-x   0 travis    (2000) travis    (2000)    94271 2021-02-17 11:14:19.000000 fastmat-0.2rc0/fastmat/Matrix.pyx
+-rwxrwxr-x   0 travis    (2000) travis    (2000)     1649 2021-02-17 11:14:19.000000 fastmat-0.2rc0/fastmat/Outer.pxd
+-rwxrwxr-x   0 travis    (2000) travis    (2000)     7672 2021-02-17 11:14:19.000000 fastmat-0.2rc0/fastmat/Outer.pyx
+-rwxrwxr-x   0 travis    (2000) travis    (2000)     1908 2021-02-17 11:14:19.000000 fastmat-0.2rc0/fastmat/Parametric.pxd
+-rwxrwxr-x   0 travis    (2000) travis    (2000)    14158 2021-02-17 11:14:19.000000 fastmat-0.2rc0/fastmat/Parametric.pyx
+-rwxrwxr-x   0 travis    (2000) travis    (2000)     1313 2021-02-17 11:14:19.000000 fastmat-0.2rc0/fastmat/Partial.pxd
+-rwxrwxr-x   0 travis    (2000) travis    (2000)    13878 2021-02-17 11:14:19.000000 fastmat-0.2rc0/fastmat/Partial.pyx
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1180 2021-02-17 11:14:19.000000 fastmat-0.2rc0/fastmat/Permutation.pxd
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4595 2021-02-17 11:14:19.000000 fastmat-0.2rc0/fastmat/Permutation.pyx
+-rwxrwxr-x   0 travis    (2000) travis    (2000)     1407 2021-02-17 11:14:19.000000 fastmat-0.2rc0/fastmat/Polynomial.pxd
+-rwxrwxr-x   0 travis    (2000) travis    (2000)     7095 2021-02-17 11:14:19.000000 fastmat-0.2rc0/fastmat/Polynomial.pyx
+-rwxrwxr-x   0 travis    (2000) travis    (2000)     1242 2021-02-17 11:14:19.000000 fastmat-0.2rc0/fastmat/Product.pxd
+-rwxrwxr-x   0 travis    (2000) travis    (2000)    12477 2021-02-17 11:14:19.000000 fastmat-0.2rc0/fastmat/Product.pyx
+-rwxrwxr-x   0 travis    (2000) travis    (2000)     1318 2021-02-17 11:14:19.000000 fastmat-0.2rc0/fastmat/Sparse.pxd
+-rwxrwxr-x   0 travis    (2000) travis    (2000)     6993 2021-02-17 11:14:19.000000 fastmat-0.2rc0/fastmat/Sparse.pyx
+-rwxrwxr-x   0 travis    (2000) travis    (2000)     1155 2021-02-17 11:14:19.000000 fastmat-0.2rc0/fastmat/Sum.pxd
+-rwxrwxr-x   0 travis    (2000) travis    (2000)     7930 2021-02-17 11:14:19.000000 fastmat-0.2rc0/fastmat/Sum.pyx
+-rwxrwxr-x   0 travis    (2000) travis    (2000)     1592 2021-02-17 11:14:19.000000 fastmat-0.2rc0/fastmat/Toeplitz.pxd
+-rwxrwxr-x   0 travis    (2000) travis    (2000)    34517 2021-02-17 11:14:19.000000 fastmat-0.2rc0/fastmat/Toeplitz.pyx
+-rwxrwxr-x   0 travis    (2000) travis    (2000)     1097 2021-02-17 11:14:19.000000 fastmat-0.2rc0/fastmat/Zero.pxd
+-rwxrwxr-x   0 travis    (2000) travis    (2000)     4585 2021-02-17 11:14:19.000000 fastmat-0.2rc0/fastmat/Zero.pyx
+-rwxrwxr-x   0 travis    (2000) travis    (2000)     3903 2021-02-17 11:14:19.000000 fastmat-0.2rc0/fastmat/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-02-17 11:29:15.837078 fastmat-0.2rc0/fastmat/algorithms/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1056 2021-02-17 11:14:19.000000 fastmat-0.2rc0/fastmat/algorithms/Algorithm.pxd
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5517 2021-02-17 11:14:19.000000 fastmat-0.2rc0/fastmat/algorithms/Algorithm.pyx
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8988 2021-02-17 11:14:19.000000 fastmat-0.2rc0/fastmat/algorithms/FISTA.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8508 2021-02-17 11:14:19.000000 fastmat-0.2rc0/fastmat/algorithms/ISTA.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1556 2021-02-17 11:14:19.000000 fastmat-0.2rc0/fastmat/algorithms/OMP.pxd
+-rw-rw-r--   0 travis    (2000) travis    (2000)    11505 2021-02-17 11:14:19.000000 fastmat-0.2rc0/fastmat/algorithms/OMP.pyx
+-rw-rw-r--   0 travis    (2000) travis    (2000)    12307 2021-02-17 11:14:19.000000 fastmat-0.2rc0/fastmat/algorithms/STELA.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      986 2021-02-17 11:14:19.000000 fastmat-0.2rc0/fastmat/algorithms/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-02-17 11:29:15.837078 fastmat-0.2rc0/fastmat/core/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      715 2021-02-17 11:14:19.000000 fastmat-0.2rc0/fastmat/core/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    11125 2021-02-17 11:14:19.000000 fastmat-0.2rc0/fastmat/core/calibration.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2180 2021-02-17 11:14:19.000000 fastmat-0.2rc0/fastmat/core/cmath.pxd
+-rw-rw-r--   0 travis    (2000) travis    (2000)    46858 2021-02-17 11:14:19.000000 fastmat-0.2rc0/fastmat/core/cmath.pyx
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5090 2021-02-17 11:14:19.000000 fastmat-0.2rc0/fastmat/core/resource.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1860 2021-02-17 11:14:19.000000 fastmat-0.2rc0/fastmat/core/strides.pxd
+-rw-rw-r--   0 travis    (2000) travis    (2000)    13788 2021-02-17 11:14:19.000000 fastmat-0.2rc0/fastmat/core/strides.pyx
+-rw-rw-r--   0 travis    (2000) travis    (2000)      874 2021-02-17 11:14:19.000000 fastmat-0.2rc0/fastmat/core/types.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4332 2021-02-17 11:14:19.000000 fastmat-0.2rc0/fastmat/core/types.pxd
+-rw-rw-r--   0 travis    (2000) travis    (2000)    13059 2021-02-17 11:14:19.000000 fastmat-0.2rc0/fastmat/core/types.pyx
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-02-17 11:29:15.837078 fastmat-0.2rc0/fastmat/inspect/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1167 2021-02-17 11:14:19.000000 fastmat-0.2rc0/fastmat/inspect/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    29947 2021-02-17 11:14:19.000000 fastmat-0.2rc0/fastmat/inspect/benchmark.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    35900 2021-02-17 11:14:19.000000 fastmat-0.2rc0/fastmat/inspect/common.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    40116 2021-02-17 11:14:19.000000 fastmat-0.2rc0/fastmat/inspect/test.py
+-rwxrwxr-x   0 travis    (2000) travis    (2000)      248 2021-02-17 11:28:58.000000 fastmat-0.2rc0/fastmat/version.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-02-17 11:29:15.833078 fastmat-0.2rc0/fastmat.egg-info/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9874 2021-02-17 11:28:58.000000 fastmat-0.2rc0/fastmat.egg-info/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3133 2021-02-17 11:29:15.000000 fastmat-0.2rc0/fastmat.egg-info/SOURCES.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2021-02-17 11:28:58.000000 fastmat-0.2rc0/fastmat.egg-info/dependency_links.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       56 2021-02-17 11:29:15.000000 fastmat-0.2rc0/fastmat.egg-info/top_level.txt
+-rwxrwxr-x   0 travis    (2000) travis    (2000)     7526 2021-02-17 11:14:19.000000 fastmat-0.2rc0/makefile
+-rwxrwxr-x   0 travis    (2000) travis    (2000)      220 2021-02-17 11:29:15.841078 fastmat-0.2rc0/setup.cfg
+-rwxrwxr-x   0 travis    (2000) travis    (2000)    12988 2021-02-17 11:14:19.000000 fastmat-0.2rc0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `fastmat-0.2a4/LICENSE` & `fastmat-0.2rc0/LICENSE`

 * *Files identical despite different names*

### Comparing `fastmat-0.2a4/PKG-INFO` & `fastmat-0.2rc0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: fastmat
-Version: 0.2a4
+Version: 0.2rc0
 Summary: fast linear transforms in Python
 Home-page: https://ems-tu-ilmenau.github.io/fastmat/
 Author: Christoph Wagner, Sebastian Semper, EMS group TU Ilmenau
 Author-email: christoph.wagner@tu-ilmenau.de
 License: Apache Software License
 Description: # fastmat
         [![Version](https://img.shields.io/pypi/v/fastmat.svg)](https://pypi.python.org/pypi/fastmat)
@@ -26,21 +26,26 @@
         Fastmat is a framework for handling large composed or structured matrices.
         It allows expressing and using them in a mathematically intuitive way while
         storing and handling them internally in an efficient way. This approach allows
         huge savings in computational time and memory requirements compared to using
         dense matrix representations.
         
         ### Dependencies
-        - Python >= 2.7 or >=3.4
+        - Python 2.7, Python >=3.4
         - Numpy >= 1.7
         - Scipy >= 1.0
         - Cython >= 0.29
         - soft dependencies:
             - matplotlib: for demos and tools that make use of plotting functions
         
+        ### Distribution
+        Binary wheels are provided for Python >=3.5 for linux, windows and mac, as well as for x86 and ARM architectures.
+        
+        For all systems, for which no wheels are provided, you may still install fastmat from the soruce distribution.
+        
         ### Authors & Contact Information
         - Sebastian Semper | sebastian.semper@tu-ilmenau.de
           Technische Universität Ilmenau, Institute for Mathematics, EMS Group
         - Christoph Wagner | christoph.wagner@tu-ilmenau.de
           Technische Universität Ilmenau, Institute for Information Technology, EMS Group
         - **<https://www.tu-ilmenau.de/it-ems/>**
         
@@ -72,14 +77,18 @@
         from the commandline by running one easy and straightforward command:
             `pip install fastmat`
         
         When installing with pip all dependencies of the package will be installed
         along. With release 0.1.1 python wheels will be offered for many versions
         greatly improving installation time and effort.
         
+        #### Bulding from source
+        
+        Building binaries has been developed and tested for the use
+        
         ### Manually installing from source
         - download the source distribution from our github repository:
             https://github.com/EMS-TU-Ilmenau/fastmat/archive/stable.zip
         - unpack its contents and navigate to the project root directory
         - run `pip install .` to install fastmat on your computer
         - you may also install fastmat without pip, using the offered makefile:
             * type `make install` to install fastmat on your computer
@@ -136,19 +145,23 @@
 Classifier: Framework :: IPython
 Classifier: Framework :: Jupyter
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX :: Linux
+Classifier: Operating System :: POSIX :: Other
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Topic :: Software Development :: Libraries
+Description-Content-Type: text/markdown
```

### Comparing `fastmat-0.2a4/README.md` & `fastmat-0.2rc0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -18,21 +18,26 @@
 Fastmat is a framework for handling large composed or structured matrices.
 It allows expressing and using them in a mathematically intuitive way while
 storing and handling them internally in an efficient way. This approach allows
 huge savings in computational time and memory requirements compared to using
 dense matrix representations.
 
 ### Dependencies
-- Python >= 2.7 or >=3.4
+- Python 2.7, Python >=3.4
 - Numpy >= 1.7
 - Scipy >= 1.0
 - Cython >= 0.29
 - soft dependencies:
     - matplotlib: for demos and tools that make use of plotting functions
 
+### Distribution
+Binary wheels are provided for Python >=3.5 for linux, windows and mac, as well as for x86 and ARM architectures.
+
+For all systems, for which no wheels are provided, you may still install fastmat from the soruce distribution.
+
 ### Authors & Contact Information
 - Sebastian Semper | sebastian.semper@tu-ilmenau.de
   Technische Universität Ilmenau, Institute for Mathematics, EMS Group
 - Christoph Wagner | christoph.wagner@tu-ilmenau.de
   Technische Universität Ilmenau, Institute for Information Technology, EMS Group
 - **<https://www.tu-ilmenau.de/it-ems/>**
 
@@ -64,14 +69,18 @@
 from the commandline by running one easy and straightforward command:
     `pip install fastmat`
 
 When installing with pip all dependencies of the package will be installed
 along. With release 0.1.1 python wheels will be offered for many versions
 greatly improving installation time and effort.
 
+#### Bulding from source
+
+Building binaries has been developed and tested for the use
+
 ### Manually installing from source
 - download the source distribution from our github repository:
     https://github.com/EMS-TU-Ilmenau/fastmat/archive/stable.zip
 - unpack its contents and navigate to the project root directory
 - run `pip install .` to install fastmat on your computer
 - you may also install fastmat without pip, using the offered makefile:
     * type `make install` to install fastmat on your computer
```

### Comparing `fastmat-0.2a4/doc/algorithms/Algorithm.rst` & `fastmat-0.2rc0/doc/algorithms/Algorithm.rst`

 * *Files identical despite different names*

### Comparing `fastmat-0.2a4/doc/algorithms/FISTA.rst` & `fastmat-0.2rc0/doc/algorithms/FISTA.rst`

 * *Files identical despite different names*

### Comparing `fastmat-0.2a4/doc/algorithms/ISTA.rst` & `fastmat-0.2rc0/doc/algorithms/ISTA.rst`

 * *Files identical despite different names*

### Comparing `fastmat-0.2a4/doc/algorithms/OMP.rst` & `fastmat-0.2rc0/doc/algorithms/OMP.rst`

 * *Files identical despite different names*

### Comparing `fastmat-0.2a4/doc/algorithms/STELA.rst` & `fastmat-0.2rc0/doc/algorithms/STELA.rst`

 * *Files identical despite different names*

### Comparing `fastmat-0.2a4/doc/classes/BlockDiag.rst` & `fastmat-0.2rc0/doc/classes/Blocks.rst`

 * *Files 3% similar despite different names*

```diff
@@ -9,16 +9,16 @@
 
     Unless required by applicable law or agreed to in writing, software
     distributed under the License is distributed on an "AS IS" BASIS,
     WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
     See the License for the specific language governing permissions and
     limitations under the License.
 
-.. _BlockDiag:
+.. _Blocks:
 
-BlockDiag Class
-===============
+Block Matrix
+============
 
-.. autoclass:: fastmat.BlockDiag
+.. autoclass:: fastmat.Blocks
     :members:
     :undoc-members:
     :show-inheritance:
```

### Comparing `fastmat-0.2a4/doc/classes/Blocks.rst` & `fastmat-0.2rc0/doc/classes/Sum.rst`

 * *Files 4% similar despite different names*

```diff
@@ -9,16 +9,16 @@
 
     Unless required by applicable law or agreed to in writing, software
     distributed under the License is distributed on an "AS IS" BASIS,
     WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
     See the License for the specific language governing permissions and
     limitations under the License.
 
-.. _Blocks:
+.. _Sum:
 
-Blocks Class
-============
+Matrix Sum
+==========
 
-.. autoclass:: fastmat.Blocks
+.. autoclass:: fastmat.Sum
     :members:
     :undoc-members:
     :show-inheritance:
```

### Comparing `fastmat-0.2a4/doc/classes/Circulant.rst` & `fastmat-0.2rc0/doc/classes/Kron.rst`

 * *Files 6% similar despite different names*

```diff
@@ -9,16 +9,16 @@
 
     Unless required by applicable law or agreed to in writing, software
     distributed under the License is distributed on an "AS IS" BASIS,
     WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
     See the License for the specific language governing permissions and
     limitations under the License.
 
-.. _Circulant:
+.. _Kron:
 
-Circulant Class
-===============
+Kronecker Product
+=================
 
-.. autoclass:: fastmat.Circulant
+.. autoclass:: fastmat.Kron
     :members:
     :undoc-members:
     :show-inheritance:
```

### Comparing `fastmat-0.2a4/doc/classes/Diag.rst` & `fastmat-0.2rc0/doc/classes/Diag.rst`

 * *Files 4% similar despite different names*

```diff
@@ -11,14 +11,14 @@
     distributed under the License is distributed on an "AS IS" BASIS,
     WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
     See the License for the specific language governing permissions and
     limitations under the License.
 
 .. _Diag:
 
-Diag Class
-==========
+Diagonal Matrix
+===============
 
 .. autoclass:: fastmat.Diag
     :members:
     :undoc-members:
     :show-inheritance:
```

### Comparing `fastmat-0.2a4/doc/classes/DiagBlocks.rst` & `fastmat-0.2rc0/doc/classes/Sparse.rst`

 * *Files 6% similar despite different names*

```diff
@@ -9,16 +9,16 @@
 
     Unless required by applicable law or agreed to in writing, software
     distributed under the License is distributed on an "AS IS" BASIS,
     WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
     See the License for the specific language governing permissions and
     limitations under the License.
 
-.. _DiagBlocks:
+.. _Sparse:
 
-DiagBlocks Class
-================
+Sparse Matrix
+=============
 
-.. autoclass:: fastmat.DiagBlocks
+.. autoclass:: fastmat.Sparse
     :members:
     :undoc-members:
     :show-inheritance:
```

### Comparing `fastmat-0.2a4/doc/classes/Eye.rst` & `fastmat-0.2rc0/doc/classes/Fourier.rst`

 * *Files 5% similar despite different names*

```diff
@@ -9,16 +9,16 @@
 
     Unless required by applicable law or agreed to in writing, software
     distributed under the License is distributed on an "AS IS" BASIS,
     WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
     See the License for the specific language governing permissions and
     limitations under the License.
 
-.. _Eye:
+.. _Fourier:
 
-Eye Class
-=========
+Fourier Matrix
+==============
 
-.. autoclass:: fastmat.Eye
+.. autoclass:: fastmat.Fourier
     :members:
     :undoc-members:
     :show-inheritance:
```

### Comparing `fastmat-0.2a4/doc/classes/Fourier.rst` & `fastmat-0.2rc0/doc/classes/Parametric.rst`

 * *Files 9% similar despite different names*

```diff
@@ -9,16 +9,16 @@
 
     Unless required by applicable law or agreed to in writing, software
     distributed under the License is distributed on an "AS IS" BASIS,
     WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
     See the License for the specific language governing permissions and
     limitations under the License.
 
-.. _Fourier:
+.. _Parametric:
 
-Fourier Class
-=============
+Parametric Matrix
+=================
 
-.. autoclass:: fastmat.Fourier
+.. autoclass:: fastmat.Parametric
     :members:
     :undoc-members:
     :show-inheritance:
```

### Comparing `fastmat-0.2a4/doc/classes/Hadamard.rst` & `fastmat-0.2rc0/doc/classes/LSFRCirculant.rst`

 * *Files 6% similar despite different names*

```diff
@@ -9,16 +9,16 @@
 
     Unless required by applicable law or agreed to in writing, software
     distributed under the License is distributed on an "AS IS" BASIS,
     WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
     See the License for the specific language governing permissions and
     limitations under the License.
 
-.. _Hadamard:
+.. _LFSRCirculant:
 
-Hadamard Class
-==============
+LFSR Circulant Matrix
+=====================
 
-.. autoclass:: fastmat.Hadamard
+.. autoclass:: fastmat.LFSRCirculant
     :members:
     :undoc-members:
     :show-inheritance:
```

### Comparing `fastmat-0.2a4/doc/classes/Kron.rst` & `fastmat-0.2rc0/doc/classes/Eye.rst`

 * *Files 4% similar despite different names*

```diff
@@ -9,16 +9,16 @@
 
     Unless required by applicable law or agreed to in writing, software
     distributed under the License is distributed on an "AS IS" BASIS,
     WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
     See the License for the specific language governing permissions and
     limitations under the License.
 
-.. _Kron:
+.. _Eye:
 
-Kron Class
-==========
+Identity Matrix
+===============
 
-.. autoclass:: fastmat.Kron
+.. autoclass:: fastmat.Eye
     :members:
     :undoc-members:
     :show-inheritance:
```

### Comparing `fastmat-0.2a4/doc/classes/LSFRCirculant.rst` & `fastmat-0.2rc0/doc/classes/Circulant.rst`

 * *Files 5% similar despite different names*

```diff
@@ -9,16 +9,16 @@
 
     Unless required by applicable law or agreed to in writing, software
     distributed under the License is distributed on an "AS IS" BASIS,
     WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
     See the License for the specific language governing permissions and
     limitations under the License.
 
-.. _LFSRCirculant:
+.. _Circulant:
 
-LFSRCirculant Class
-===================
+(Multilevel) Circulant Class
+============================
 
-.. autoclass:: fastmat.LFSRCirculant
+.. autoclass:: fastmat.Circulant
     :members:
     :undoc-members:
     :show-inheritance:
```

### Comparing `fastmat-0.2a4/doc/classes/LowRank.rst` & `fastmat-0.2rc0/doc/classes/Zero.rst`

 * *Files 5% similar despite different names*

```diff
@@ -9,16 +9,16 @@
 
     Unless required by applicable law or agreed to in writing, software
     distributed under the License is distributed on an "AS IS" BASIS,
     WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
     See the License for the specific language governing permissions and
     limitations under the License.
 
-.. _LowRank:
+.. _Zero:
 
-LowRank Class
-=============
+Zero Matrix
+===========
 
-.. autoclass:: fastmat.LowRank
+.. autoclass:: fastmat.Zero
     :members:
     :undoc-members:
     :show-inheritance:
```

### Comparing `fastmat-0.2a4/doc/classes/MLCirculant.rst` & `fastmat-0.2rc0/doc/classes/Matrix.rst`

 * *Files 19% similar despite different names*

```diff
@@ -9,16 +9,16 @@
 
     Unless required by applicable law or agreed to in writing, software
     distributed under the License is distributed on an "AS IS" BASIS,
     WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
     See the License for the specific language governing permissions and
     limitations under the License.
 
-.. _MLCirculant:
+.. _Matrix:
 
-MLCirculant Class
+Matrix Base Class
 =================
 
-.. autoclass:: fastmat.MLCirculant
+.. autoclass:: fastmat.Matrix
     :members:
     :undoc-members:
     :show-inheritance:
```

### Comparing `fastmat-0.2a4/doc/classes/MLToeplitz.rst` & `fastmat-0.2rc0/doc/expansion/implement.rst`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,21 @@
-..  Copyright 2018 Sebastian Semper, Christoph Wagner
-        https://www.tu-ilmenau.de/it-ems/
-
-    Licensed under the Apache License, Version 2.0 (the "License");
-    you may not use this file except in compliance with the License.
-    You may obtain a copy of the License at
-
-        http://www.apache.org/licenses/LICENSE-2.0
-
-    Unless required by applicable law or agreed to in writing, software
-    distributed under the License is distributed on an "AS IS" BASIS,
-    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-    See the License for the specific language governing permissions and
-    limitations under the License.
-
-.. _MLToeplitz:
-
-MLToeplitz Class
-================
-
-.. autoclass:: fastmat.MLToeplitz
-    :members:
-    :undoc-members:
-    :show-inheritance:
+..  Copyright 2016 Sebastian Semper, Christoph Wagner
+        https://www.tu-ilmenau.de/it-ems/
+
+    Licensed under the Apache License, Version 2.0 (the "License");
+    you may not use this file except in compliance with the License.
+    You may obtain a copy of the License at
+
+        http://www.apache.org/licenses/LICENSE-2.0
+
+    Unless required by applicable law or agreed to in writing, software
+    distributed under the License is distributed on an "AS IS" BASIS,
+    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+    See the License for the specific language governing permissions and
+    limitations under the License.
+
+.. _implementation:
+
+Developing Your own fastmat Matrix
+==================================
+
+To be delivered (somewhere in time).
```

### Comparing `fastmat-0.2a4/doc/classes/MLUltraSound.rst` & `fastmat-0.2rc0/doc/classes/Product.rst`

 * *Files 8% similar despite different names*

```diff
@@ -9,16 +9,16 @@
 
     Unless required by applicable law or agreed to in writing, software
     distributed under the License is distributed on an "AS IS" BASIS,
     WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
     See the License for the specific language governing permissions and
     limitations under the License.
 
-.. _MLUltraSound:
+.. _Product:
 
-MLUltraSound Class
-==================
+Matrix-Matrix Product
+=====================
 
-.. autoclass:: fastmat.MLUltraSound
+.. autoclass:: fastmat.Product
     :members:
     :undoc-members:
     :show-inheritance:
```

### Comparing `fastmat-0.2a4/doc/classes/Outer.rst` & `fastmat-0.2rc0/doc/classes/Permutation.rst`

 * *Files 10% similar despite different names*

```diff
@@ -9,16 +9,16 @@
 
     Unless required by applicable law or agreed to in writing, software
     distributed under the License is distributed on an "AS IS" BASIS,
     WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
     See the License for the specific language governing permissions and
     limitations under the License.
 
-.. _Outer:
+.. _Permutation:
 
-Outer Class
-===========
+Permutation Matrix
+==================
 
-.. autoclass:: fastmat.Outer
+.. autoclass:: fastmat.Permutation
     :members:
     :undoc-members:
     :show-inheritance:
```

### Comparing `fastmat-0.2a4/doc/classes/Parametric.rst` & `fastmat-0.2rc0/doc/classes/Partial.rst`

 * *Files 6% similar despite different names*

```diff
@@ -9,16 +9,16 @@
 
     Unless required by applicable law or agreed to in writing, software
     distributed under the License is distributed on an "AS IS" BASIS,
     WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
     See the License for the specific language governing permissions and
     limitations under the License.
 
-.. _Parametric:
+.. _Partial:
 
-Parametric Class
-================
+Partial Matrix
+==============
 
-.. autoclass:: fastmat.Parametric
+.. autoclass:: fastmat.Partial
     :members:
     :undoc-members:
     :show-inheritance:
```

### Comparing `fastmat-0.2a4/doc/classes/Partial.rst` & `fastmat-0.2rc0/doc/classes/Toeplitz.rst`

 * *Files 18% similar despite different names*

```diff
@@ -9,16 +9,16 @@
 
     Unless required by applicable law or agreed to in writing, software
     distributed under the License is distributed on an "AS IS" BASIS,
     WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
     See the License for the specific language governing permissions and
     limitations under the License.
 
-.. _Partial:
+.. _Toeplitz:
 
-Partial Class
-=============
+(Multilevel) Toeplitz Class
+===========================
 
-.. autoclass:: fastmat.Partial
+.. autoclass:: fastmat.Toeplitz
     :members:
     :undoc-members:
     :show-inheritance:
```

### Comparing `fastmat-0.2a4/doc/classes/Permutation.rst` & `fastmat-0.2rc0/doc/classes/Hadamard.rst`

 * *Files 8% similar despite different names*

```diff
@@ -9,16 +9,16 @@
 
     Unless required by applicable law or agreed to in writing, software
     distributed under the License is distributed on an "AS IS" BASIS,
     WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
     See the License for the specific language governing permissions and
     limitations under the License.
 
-.. _Permutation:
+.. _Hadamard:
 
-Permutation Class
-=================
+Hadamard Matrix
+===============
 
-.. autoclass:: fastmat.Permutation
+.. autoclass:: fastmat.Hadamard
     :members:
     :undoc-members:
     :show-inheritance:
```

### Comparing `fastmat-0.2a4/doc/classes/Polynomial.rst` & `fastmat-0.2rc0/doc/classes/Polynomial.rst`

 * *Files 18% similar despite different names*

```diff
@@ -11,14 +11,14 @@
     distributed under the License is distributed on an "AS IS" BASIS,
     WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
     See the License for the specific language governing permissions and
     limitations under the License.
 
 .. _Polynomial:
 
-Polynomial Class
-================
+Matrix Polynomial
+=================
 
 .. autoclass:: fastmat.Polynomial
     :members:
     :undoc-members:
     :show-inheritance:
```

### Comparing `fastmat-0.2a4/doc/classes/Product.rst` & `fastmat-0.2rc0/doc/classes/BlockDiag.rst`

 * *Files 6% similar despite different names*

```diff
@@ -9,16 +9,19 @@
 
     Unless required by applicable law or agreed to in writing, software
     distributed under the License is distributed on an "AS IS" BASIS,
     WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
     See the License for the specific language governing permissions and
     limitations under the License.
 
-.. _Product:
 
-Product Class
-=============
 
-.. autoclass:: fastmat.Product
+.. _BlockDiag:
+
+
+Block Diagonal Matrix
+=====================
+
+.. autoclass:: fastmat.BlockDiag
     :members:
     :undoc-members:
     :show-inheritance:
```

### Comparing `fastmat-0.2a4/doc/classes/Sparse.rst` & `fastmat-0.2rc0/doc/inspection/benchmark.rst`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,21 @@
-..  Copyright 2018 Sebastian Semper, Christoph Wagner
-        https://www.tu-ilmenau.de/it-ems/
-
-    Licensed under the Apache License, Version 2.0 (the "License");
-    you may not use this file except in compliance with the License.
-    You may obtain a copy of the License at
-
-        http://www.apache.org/licenses/LICENSE-2.0
-
-    Unless required by applicable law or agreed to in writing, software
-    distributed under the License is distributed on an "AS IS" BASIS,
-    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-    See the License for the specific language governing permissions and
-    limitations under the License.
-
-.. _Sparse:
-
-Sparse Class
-============
-
-.. autoclass:: fastmat.Sparse
-    :members:
-    :undoc-members:
-    :show-inheritance:
+..  Copyright 2016 Sebastian Semper, Christoph Wagner
+        https://www.tu-ilmenau.de/it-ems/
+
+    Licensed under the Apache License, Version 2.0 (the "License");
+    you may not use this file except in compliance with the License.
+    You may obtain a copy of the License at
+
+        http://www.apache.org/licenses/LICENSE-2.0
+
+    Unless required by applicable law or agreed to in writing, software
+    distributed under the License is distributed on an "AS IS" BASIS,
+    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+    See the License for the specific language governing permissions and
+    limitations under the License.
+
+.. _benchmarking:
+
+Benchmarking fastmat Classes
+============================
+
+To be delivered (somewhere in time).
```

### Comparing `fastmat-0.2a4/doc/classes/Sum.rst` & `fastmat-0.2rc0/doc/classes/LowRank.rst`

 * *Files 14% similar despite different names*

```diff
@@ -9,16 +9,16 @@
 
     Unless required by applicable law or agreed to in writing, software
     distributed under the License is distributed on an "AS IS" BASIS,
     WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
     See the License for the specific language governing permissions and
     limitations under the License.
 
-.. _Sum:
+.. _LowRank:
 
-Sum Class
-=========
+Low Rank Matrix
+===============
 
-.. autoclass:: fastmat.Sum
+.. autoclass:: fastmat.LowRank
     :members:
     :undoc-members:
     :show-inheritance:
```

### Comparing `fastmat-0.2a4/doc/classes/Toeplitz.rst` & `fastmat-0.2rc0/doc/classes/DiagBlocks.rst`

 * *Files 17% similar despite different names*

```diff
@@ -9,16 +9,16 @@
 
     Unless required by applicable law or agreed to in writing, software
     distributed under the License is distributed on an "AS IS" BASIS,
     WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
     See the License for the specific language governing permissions and
     limitations under the License.
 
-.. _Toeplitz:
+.. _DiagBlocks:
 
-Toeplitz Class
-==============
+Diagonal Block Matrix
+=====================
 
-.. autoclass:: fastmat.Toeplitz
+.. autoclass:: fastmat.DiagBlocks
     :members:
     :undoc-members:
     :show-inheritance:
```

### Comparing `fastmat-0.2a4/doc/classes/Zero.rst` & `fastmat-0.2rc0/doc/classes/Transpose.rst`

 * *Files 16% similar despite different names*

```diff
@@ -9,16 +9,26 @@
 
     Unless required by applicable law or agreed to in writing, software
     distributed under the License is distributed on an "AS IS" BASIS,
     WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
     See the License for the specific language governing permissions and
     limitations under the License.
 
-.. _Zero:
+.. _Transpose:
 
-Zero Class
-==========
+Transposition and Related Classes
+=================================
 
-.. autoclass:: fastmat.Zero
+.. autoclass:: fastmat.Transpose
+    :members:
+    :undoc-members:
+    :show-inheritance:
+
+.. autoclass:: fastmat.Hermitian
+    :members:
+    :undoc-members:
+    :show-inheritance:
+
+.. autoclass:: fastmat.Conjugate
     :members:
     :undoc-members:
     :show-inheritance:
```

### Comparing `fastmat-0.2a4/doc/classes.rst` & `fastmat-0.2rc0/doc/classes.rst`

 * *Files 24% similar despite different names*

```diff
@@ -9,44 +9,45 @@
 
     Unless required by applicable law or agreed to in writing, software
     distributed under the License is distributed on an "AS IS" BASIS,
     WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
     See the License for the specific language governing permissions and
     limitations under the License.
 
-.. _classes:
+###############
+  Class Index
+###############
+
+.. toctree::
+   :glob:
+   :hidden:
+
+   classes/*
 
-Classes
-=======
 
 Here we list the classes in the package for easy referencing and access.
 
  * :py:class:`fastmat.Matrix` base class, the mother of all matrices.
  * :py:class:`fastmat.BlockDiag`
  * :py:class:`fastmat.Blocks`
  * :py:class:`fastmat.Circulant`
  * :py:class:`fastmat.Conjugate`
  * :py:class:`fastmat.Diag`
  * :py:class:`fastmat.DiagBlocks`
  * :py:class:`fastmat.Eye`
  * :py:class:`fastmat.Fourier`
- * :py:class:`fastmat.Inverse`
  * :py:class:`fastmat.Hadamard`
  * :py:class:`fastmat.Hermitian`
  * :py:class:`fastmat.Kron`
  * :py:class:`fastmat.LFSRCirculant`
  * :py:class:`fastmat.LowRank`
- * :py:class:`fastmat.MLCirculant`
- * :py:class:`fastmat.MLToeplitz`
- * :py:class:`fastmat.MLUltraSound`
  * :py:class:`fastmat.Outer`
  * :py:class:`fastmat.Parametric`
  * :py:class:`fastmat.Partial`
  * :py:class:`fastmat.Permutation`
  * :py:class:`fastmat.Polynomial`
  * :py:class:`fastmat.Product`
- * :py:class:`fastmat.PseudoInverse`
  * :py:class:`fastmat.Sparse`
  * :py:class:`fastmat.Sum`
  * :py:class:`fastmat.Toeplitz`
  * :py:class:`fastmat.Transpose`
  * :py:class:`fastmat.Zero`
```

### Comparing `fastmat-0.2a4/doc/conf.py` & `fastmat-0.2rc0/doc/conf.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,36 +15,38 @@
 
 # If extensions (or modules to document with autodoc) are in another directory,
 # add these directories to sys.path here. If the directory is relative to the
 # documentation root, use os.path.abspath to make it absolute, like shown here.
 #
 import os
 import sys
-sys.path.append(os.path.abspath('../'))
-sys.path.append(os.path.abspath('../util'))
-sys.path.append(os.path.abspath('../fastmat'))
+print(sys.version)
+
+sys.path.insert(0, os.path.abspath('..'))
 import fastmat.version as fmv
 
 # -- General configuration ------------------------------------------------
 
 # If your documentation needs a minimal Sphinx version, state it here.
 #
 # needs_sphinx = '1.0'
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
 # ones.
 extensions = [
     'sphinx.ext.autodoc',
+    'sphinx.ext.autosectionlabel',
     'sphinx.ext.doctest',
     'sphinx.ext.todo',
     'sphinx.ext.coverage',
     'sphinx.ext.mathjax',
     'sphinx.ext.githubpages',
     'sphinx.ext.autosummary',
+	'matplotlib.sphinxext.plot_directive',
     'numpydoc'
     ]
 
 # Add any paths that contain templates here, relative to this directory.
 templates_path = ['_templates']
 
 # The suffix(es) of source filenames.
@@ -90,15 +92,22 @@
 
 
 # -- Options for HTML output ----------------------------------------------
 
 # The theme to use for HTML and HTML Help pages.  See the documentation for
 # a list of builtin themes.
 #
-html_theme = 'bizstyle'
+html_theme = 'sphinx_rtd_theme'
+
+html_theme_options = {
+    "collapse_navigation": False
+}
+
+html_logo = "_static/gfx/logo_short.png"
+html_favicon = "_static/gfx/logo_favicon.png"
 
 # Theme options are theme-specific and customize the look and feel of a theme
 # further.  For a list of options available for each theme, see the
 # documentation.
 #
 # html_theme_options = {}
 
@@ -133,7 +142,8 @@
     if name == "__init__":
         return False
     return skip
 
 
 def setup(app):
     app.connect("autodoc-skip-member", skip)
+    app.add_stylesheet('custom.css')
```

### Comparing `fastmat-0.2a4/doc/index.rst` & `fastmat-0.2rc0/doc/index.rst`

 * *Files 10% similar despite different names*

```diff
@@ -10,43 +10,45 @@
     Unless required by applicable law or agreed to in writing, software
     distributed under the License is distributed on an "AS IS" BASIS,
     WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
     See the License for the specific language governing permissions and
     limitations under the License.
 
 .. toctree::
-   :glob:
-   :maxdepth: 2
+   :maxdepth: -1
    :hidden:
 
-   classes/*
    classes
-   algorithms/*
-   scipy
-   submod
+   algorithms
+   architecture
+   expansion
+   inspection
+   examples
+   references
+   releases
+
+
+.. image:: _static/gfx/logo_long.png
+ :width: 300px
+ :alt: fastmat
+ :align: center
+ :class: pixelated
 
-.. automodule:: fastmat
-
-.. automodule:: fastmat.algorithms
-
-Auxiliary Submodules
---------------------
-
-To dig into the docu of our internals, have a look at :ref:`submod`.
+---------
 
+Introduction
+------------
 
-Scipy Interface
----------------
+.. automodule:: fastmat
 
-We have a very neat and simple interface to the linear Operators offered by SciPy, which also allow the same lazy evaluation as the fast mat classes. See :ref:`scipy` for further information.
 
 Publications
 ------------
 
-Since we created a package for scientific computing, it makes sense to use it for science. Below we list all publications, which make use of our package with varying degree. If you used fastmat in you publication, we are happy to reference it here:
+Since we created a package for scientific computing, it makes sense to use it for science. Below we list all publications, which make use of our package with varying degree. If made use of fastmat in your publication, we are happy to reference it here:
 
     - The White Paper: `Fast Linear Transforms in Python <https://arxiv.org/abs/1710.09578>`_
     - `Defect Detection from 3D Ultrasonic Measurements Using Matrix-free Sparse Recovery Algorithms <https://www.researchgate.net/publication/327768393_Defect_Detection_from_3D_Ultrasonic_Measurements_Using_Matrix-free_Sparse_Recovery_Algorithms>`_
     - `GPU-accelerated Matrix-Free 3D Ultrasound Reconstruction for Nondestructive Testing <https://www.researchgate.net/publication/328476659_GPU-accelerated_Matrix-Free_3D_Ultrasound_Reconstruction_for_Nondestructive_Testing>`_
 
 If you use fastmat in your own work we kindly ask you to cite the above mentioned white paper as an acknowledgement.
```

### Comparing `fastmat-0.2a4/doc/scipy.rst` & `fastmat-0.2rc0/doc/architecture/scipy.rst`

 * *Files 23% similar despite different names*

```diff
@@ -14,51 +14,32 @@
     limitations under the License.
 
 .. _scipy:
 
 SciPy Interface
 ===============
 
-Table of Contents
------------------
+Motivation
+----------
 
- * `Motivation`_
- * `Examples`_
+SciPy offers a large zoo of algorithms which exploit the possibility to pass a
+so called LinearOperator, which only provides methods for forward and backward
+transforms together with some simple properties like a datatype and shape
+parameters. This is exactly what we can provide for a specific instance of a
+fastmat Matrix. To this end, each fastmat Matrix has the (read only) property
+scipyLinearOperator, which provides a SciPy Linear operator realizing the
+transform specified by the fastmat object.
+
+This allows to combine fastmat and SciPy in the most efficient manner possible.
+Here, fastmat provides the simple and efficient description of a huge variety
+of linear operators, which can then be used neatly and trouble free in SciPy.
+
+Usage
+-----
+
+The interface is provided by the factory
+:py:meth:`fastmat.Matrix.scipyLinearOperator`, which returns an instance of
+:py:class:`scipy.sparse.linalg.LinearOperator`. All fastmat matrices can be
+used from `scipy` methods supporting this interface, offering a wide range of
+functionality -- by combining both worlds -- to the user.
 
-.. _`Motivation`:
-
-Motivation for a SciPy Interface
---------------------------------
-
-SciPy offers a large zoo of algorithms which exploit the possibility to pass a so called LinearOperator, which only provides methods for forward and backward transforms together with some simple properties like a datatype and shape parameters. This is exactly what we can provide for a specific instance of a fastmat Matrix. To this end, each fastmat Matrix has the (read only) property scipyLinearOperator, which provides a SciPy Linear operator realizing the transform specified by the fastmat object.
-
-This allows to combine fastmat and SciPy in the most efficient manner possible. Here, fastmat provides the simple and efficient description of a huge variety of linear operators, which can then be used neatly and trouble free in SciPy.
-
-
-.. _`Examples`:
-
-Examples
---------
-
-Solve a system of linear equations with preconditioning, where the preconditioner can also be provided as a LinearOperator.
-
->>> import fastmat as fm
->>> import numpy as np
->>> from scipy.sparse.linalg import cgs
->>>
->>> # diagonal matrix with no zeros
->>> d = np.random.uniform(1, 20, 2**numO)
->>>
->>> # fastmat object
->>> H = fm.Diag(d)
->>>
->>> # use the new property to generate a scipy linear operator
->>> Hs = H1.scipyLinearOperator
->>>
->>> # also generate a Preconditioning linear operator,
->>> # which in this case is the exact inverse
->>> Ms = fm.Diag(1.0 / d).scipyLinearOperator
->>>
->>> # get a baseline
->>> y = np.linalg.solve(H1.array, x)
->>> cgs(Hs, x, tol=1e-10)
->>> cgs(Hs, x, tol=1e-10, M=Ms)
+For a code example, see :ref:`example-scipy-linear-operator`.
```

### Comparing `fastmat-0.2a4/doc/submod.rst` & `fastmat-0.2rc0/doc/classes/Outer.rst`

 * *Files 17% similar despite different names*

```diff
@@ -1,27 +1,24 @@
-..  Copyright 2016 Sebastian Semper, Christoph Wagner
+..  Copyright 2018 Sebastian Semper, Christoph Wagner
         https://www.tu-ilmenau.de/it-ems/
 
     Licensed under the Apache License, Version 2.0 (the "License");
     you may not use this file except in compliance with the License.
     You may obtain a copy of the License at
 
         http://www.apache.org/licenses/LICENSE-2.0
 
     Unless required by applicable law or agreed to in writing, software
     distributed under the License is distributed on an "AS IS" BASIS,
     WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
     See the License for the specific language governing permissions and
     limitations under the License.
 
-.. _submod:
+.. _Outer:
 
-Submodules
-==========
+Outer Product
+=============
 
-.. automodule:: fastmat.core
-    :members:
-    :undoc-members:
-
-.. automodule:: fastmat.inspect
+.. autoclass:: fastmat.Outer
     :members:
     :undoc-members:
+    :show-inheritance:
```

### Comparing `fastmat-0.2a4/fastmat/BlockDiag.pxd` & `fastmat-0.2rc0/fastmat/BlockDiag.pxd`

 * *Files identical despite different names*

### Comparing `fastmat-0.2a4/fastmat/BlockDiag.pyx` & `fastmat-0.2rc0/fastmat/BlockDiag.pyx`

 * *Files 3% similar despite different names*

```diff
@@ -98,16 +98,17 @@
 
         Parameters
         ----------
         *matrices : :py:class:`fastmat.Matrix`
             The matrix instances to be put along the main diagonal of the block
             diagonal matrix, beginning at index (0, 0) with the first matrix.
 
-        **options :
-            See :py:meth:`fastmat.Matrix.__init__`.
+        **options : optional
+            Additional keyworded arguments. Supports all optional arguments
+            supported by :py:class:`fastmat.Matrix`.
         '''
         cdef intsize numRows = 0, numCols = 0
         cdef Matrix term
 
         self._content = matrices
 
         if len(matrices) < 1:
```

### Comparing `fastmat-0.2a4/fastmat/Blocks.pxd` & `fastmat-0.2rc0/fastmat/Blocks.pxd`

 * *Files identical despite different names*

### Comparing `fastmat-0.2a4/fastmat/Blocks.pyx` & `fastmat-0.2rc0/fastmat/Blocks.pyx`

 * *Files 6% similar despite different names*

```diff
@@ -73,30 +73,50 @@
             must form a consistent grid over all instances of the 2d iterable.
             The inner iterable defines one row of the block matrix whereas the
             outer iterable defines the stacking of these rows. All inner
             iterables must be of same length. Further, all matrix instances in
             a row must have equal height and all instances in a column must
             have equal width.
 
-        **options :
-            See :py:meth:`fastmat.Matrix.__init__`.
+        **options : optional
+            Additional keyworded arguments. Supports all optional arguments
+            supported by :py:class:`fastmat.Matrix`.
         '''
-        if not isinstance(arrMatrices, list):
+        if not isinstance(arrMatrices, (list, tuple)):
             raise ValueError("Blocks: Not a nested list of fastmat matrices.")
 
         if len(arrMatrices) < 1:
             raise ValueError("Blocks: Contains no matrices.")
 
         cdef intsize numRows = 0, numCols = 0
         cdef intsize ii, rr, cc
         cdef tuple row, firstRow
         cdef Matrix term
 
-        # initialize sizes and number of rows / cols
+        # initialize number of rows
         self._numRows = len(arrMatrices)
+
+        # check that the there actually are two layers of list containers
+        # and only then fastmat Matrix instances. However, we do not want
+        # to disencourage duck-typing by restricting to particular types
+        # of containers (i.e. lists). Therefore, if we encounter a Matrix
+        # instance directly at the second level, we should notify the user
+        # verbosely what exactly is wrong with that and how to fix it.
+        for rr, item in enumerate(arrMatrices):
+            if isinstance(item, Matrix):
+                raise TypeError(
+                    (
+                        "Blocks.row(%d) is of type %s. Instantiate Blocks " +
+                        "with a 2D structure of iterables (e.g. nested " +
+                        "lists) holding fastmat Matrix instances in their " +
+                        "second level."
+                    ) %(rr, repr(item))
+                )
+
+        # initialize number of columns
         self._numCols = len(arrMatrices[0])
         dataType = np.int8
 
         # generate transposed block structure, force tuples for backward()
         cdef list lst = [tuple(arrMatrices[rr]) for rr in range(self._numRows)]
         self._rows = tuple(lst)
         lst = [[] for _ in range(self._numCols)]
@@ -112,15 +132,18 @@
 
             # get number of rows from first elements in columns
             numRows += row[0].numRows
 
             # check for presence of enough blocks
             if len(row) != self._numCols:
                 raise ValueError(
-                    "Blocks.row(%d) has incompatible number of entries" %(rr))
+                    "Blocks.row(%d) has incompatible number of entries" %(
+                        rr,
+                    )
+                )
 
             # enumerate columns
             for cc in range(self._numCols):
                 term = row[cc]
 
                 # check for matching column height and width
                 if term.numRows != row[0].numRows:
```

### Comparing `fastmat-0.2a4/fastmat/Circulant.pxd` & `fastmat-0.2rc0/fastmat/Circulant.pxd`

 * *Files identical despite different names*

### Comparing `fastmat-0.2a4/fastmat/Circulant.pyx` & `fastmat-0.2rc0/fastmat/Circulant.pyx`

 * *Files 14% similar despite different names*

```diff
@@ -27,127 +27,60 @@
 from .Fourier cimport Fourier
 from .Diag cimport Diag
 from .Kron cimport Kron
 
 
 cdef class Circulant(Partial):
     r"""
-    Multilevel Circulant Matrices are not circulant by themselves, but consist
-    of multiply nested levels of circulant structures. To this end, let
-    :math:`d \geqslant 2`, :math:`n = [n_1, \dots, n_d]`,
-    :math:`n_{1-} = [n_1,\dots, n_{d-1}]` and :math:`m = [n_2,\dots, n_d]`.
-    Then, given a :math:`d`-dimensional complex sequence
-    :math:`c = [c_{k}]` for :math:`k \in \mathbb{N}^d`
-    a :math:`d`-level circulant matrix :math:`C_{n,d}` is recursively defined as
-
-    .. math::C_{n,d} =
-        \begin{bmatrix}
-        {C}_{[1,{m}],\ell}        & {C}_{[n_1,{m}],\ell}
-        & \dots     & {C}_{[2,{m}],\ell}  \\
-        {C}_{[2,{m}],\ell}        & {C}_{[1,{m}],\ell}
-        & \dots     & {C}_{[3,{m}],\ell}  \\
-        \vdots                              & \vdots
-        & \ddots    & \vdots                        \\
-        {C}_{[n_1,{m}],\ell}      & {C}_{[n_1 - 1,{m}],\ell}
-        & \dots     & {C}_{[1,{m}],\ell}  \\
-        \end{bmatrix}.
-
-    So for :math:`n = (2,2)` and :math:`c \in \mathbb{C}^{2 \times 2}` we get
-
-    .. math::
-        C_{[2,2],2} =
-        \begin{bmatrix}
-        C_{[1,2],1} & C_{[2,2],1} \\
-        C_{[2,2],1} & C_{[1,2],1}
-        \end{bmatrix}
-        =
-        \begin{bmatrix}
-        c_{1,1} & c_{1,2} & c_{2,1} & c_{2,2} \\
-        c_{1,2} & c_{1,1} & c_{2,2} & c_{2,1} \\
-        c_{2,1} & c_{2,2} & c_{1,1} & c_{1,2} \\
-        c_{2,2} & c_{2,1} & c_{1,2} & c_{1,1}
-        \end{bmatrix}.
-
-    The approach we follow here is similar to the Circulant matrix case. But
-    here, we have matrix, which is defined by a tensor of order d because of
-    its d-level nature. The remarkable thing is, that a very analogue thing as
-    to the Circulant case holds. We only have to calculate an d-dimensional
-    fourier transform on the defining tensor. then its vectorized version is
-    the spectrum of the d-level circulant matrix it defines. Another way to
-    view this, is that a kronecker product of fourier matrices diagonalizes
-    this d-level matrix. So, we have that
-
-            C = (F_n1 kron ... kron F_nd)^H
-                 * diag((F_n1 kron ... kron F_nd) * tenC)
-                 * (F_n1 kron ... kron F_nd)
-
-    As another performance improvement, we do not simply calculate the fourier
-    transform of tenC in every dimension, but instead we make use of the
-    bluestein algorithm in each dimension independently. as such the d-level
-    circulant matrix gets embedded into a larger d-level circulant matrix,
-    which is then more efficient in reducing the bottleneck of the FFTs. this
-    is why this matrix class is derived from Partial.
-
-    >>> # import the package
-    >>> import fastmat as fm
-    >>> import numpy as np
-    >>> # construct the
-    >>> # parameters
-    >>> n = 2
-    >>> l = 2
-    >>> c = np.arange(n ** l).reshape((n,n))
-    >>> # construct the matrix
-    >>> C = fm.MLCirculant(c)
-
-    This then yields
-
-    .. math::
-        c = \begin{bmatrix}
-            0 & 1 \\
-            2 & 3
-            \end{bmatrix}
-
-    and thus
-
-    .. math::
-        C = \begin{bmatrix}
-            0 & 1 & 2 & 3 \\
-            1 & 0 & 3 & 2 \\
-            2 & 3 & 0 & 1 \\
-            3 & 2 & 1 & 0
-            \end{bmatrix},
-
-    This class depends on ``fm.Fourier``, ``fm.Diag``, ``fm.Kron``,
-    ``fm.Product`` and ``fm.Partial``.
-
-    .. todo::
-        - save memory by not storing tenC but only its fourier transform
+    This class provides a very general implementation of circulant matrices,
+    which essentially realize a (possibly multidimensional) circular
+    convolution.
+
+    This type of matrix is highly structured. A two-level circulant
+    Matrix looks like:
+
+    >>> c_00 c_02 c_01   c_20 c_22 c_21   c_10 c_12 c_11
+    >>> c_01 c_00 c_02   c_21 c_20 c_22   c_11 c_10 c_12
+    >>> c_02 c_01 c_00   c_22 c_21 c_20   c_12 c_11 c_10
+    >>>
+    >>> c_10 c_12 c_11   c_00 c_02 c_01   c_20 c_22 c_21
+    >>> c_11 c_10 c_12   c_01 c_00 c_02   c_21 c_20 c_22
+    >>> c_12 c_11 c_10   c_02 c_01 c_00   c_22 c_21 c_20
+    >>>
+    >>> c_20 c_22 c_21   c_10 c_12 c_11   c_00 c_02 c_01
+    >>> c_21 c_20 c_22   c_11 c_10 c_12   c_01 c_00 c_02
+    >>> c_22 c_21 c_20   c_12 c_11 c_10   c_02 c_01 c_00
 
+    This shows that one can define an L-level Circulant matrix by a tensor
+    of order L. By design circulant matrices are always square matrices.
     """
 
     property tenC:
         r"""Return the matrix-defining column vector of the circulant matrix"""
 
         def __get__(self):
             return self._tenC
 
     def __init__(self, tenC, **options):
-        '''
-        Initialize Multilevel Circulant matrix instance.
+        '''Initialize Multilevel Circulant matrix instance.
+
+        Also see the special options of ``fastmat.Fourier``, which are
+        also supported by this matrix and the general options offered by
+        ``fastmat.Matrix.__init__``.
 
         Parameters
         ----------
         tenC : :py:class:`numpy.ndarray`
-            The generating nd-array defining the circulant tensor. The matrix
-            data type is determined by the data type of this array.
+            The generating nd-array tensor defining the circulant matrix. The
+            matrix data type is determined by the data type of this array.
 
-        **options:
-            See the special options of :py:class:`fastmat.Fourier`, which are
-            also supported by this matrix and the general options offered by
-            :py:meth:`fastmat.Matrix.__init__`.
+        **options : optional
+            Additional keyworded arguments. Supports all optional arguments
+            supported by :py:class:`fastmat.Matrix` and
+            :py:class:`fastmat.Fourier`.
         '''
         cdef intsize ii, nn, numRowsopt, size, minimalSize, paddedSize
 
         # collect matrix options
         cdef bint optimize = options.get('optimize', True)
         cdef int maxStage = options.get('maxStage', 4)
```

### Comparing `fastmat-0.2a4/fastmat/Diag.pxd` & `fastmat-0.2rc0/fastmat/Diag.pxd`

 * *Files identical despite different names*

### Comparing `fastmat-0.2a4/fastmat/Diag.pyx` & `fastmat-0.2rc0/fastmat/Diag.pyx`

 * *Files 3% similar despite different names*

```diff
@@ -75,16 +75,17 @@
         Initialize a Diag matrix instance.
 
         Parameters
         ----------
         vecD : :py:class:`numpy.ndarray`
             The generating vector of the diagonal entries of this matrix.
 
-        **options:
-            See :py:meth:`fastmat.Matrix.__init__`.
+        **options : optional
+            Additional keyworded arguments. Supports all optional arguments
+            supported by :py:class:`fastmat.Matrix`.
         '''
         # numRows is size of matrix (and of diagonal vector)
         numRows = len(vecD)
 
         # store diagonal entry vector as copy of vecD and complain if
         # dimension does not match
         self._vecD = _arrSqueezedCopy(vecD)
```

### Comparing `fastmat-0.2a4/fastmat/DiagBlocks.pxd` & `fastmat-0.2rc0/fastmat/DiagBlocks.pxd`

 * *Files identical despite different names*

### Comparing `fastmat-0.2a4/fastmat/DiagBlocks.pyx` & `fastmat-0.2rc0/fastmat/DiagBlocks.pyx`

 * *Files 6% similar despite different names*

```diff
@@ -71,16 +71,17 @@
         Parameters
         ----------
         tenDiags : :py:class:`numpy.ndarray`
             The generating 3d-array of the flattened diagonal tensor this
             matrix describes. The matrix data type is determined by the data
             type of this array.
 
-        **options:
-            See :py:meth:`fastmat.Matrix.__init__`.
+        **options : optional
+            Additional keyworded arguments. Supports all optional arguments
+            supported by :py:class:`fastmat.Matrix`.
         '''
 
         self._numDiagsRows = tenDiags.shape[0]
         self._numDiagsCols = tenDiags.shape[1]
         self._numDiagsSize = tenDiags.shape[2]
 
         cdef intsize numRows = self._numDiagsRows * self._numDiagsSize
```

### Comparing `fastmat-0.2a4/fastmat/Eye.pxd` & `fastmat-0.2rc0/fastmat/Eye.pxd`

 * *Files identical despite different names*

### Comparing `fastmat-0.2a4/fastmat/Eye.pyx` & `fastmat-0.2rc0/fastmat/Eye.pyx`

 * *Files 8% similar despite different names*

```diff
@@ -52,16 +52,17 @@
         Initialize Identity (Eye) matrix instance.
 
         Parameters
         ----------
         order : int
             Size of the desired identity matrix [order x order].
 
-        **options:
-            See :py:meth:`fastmat.Matrix.__init__`.
+        **options : optional
+            Additional keyworded arguments. Supports all optional arguments
+            supported by :py:class:`fastmat.Matrix`.
         '''
         self._initProperties(order, order, np.int8, **options)
 
     cpdef np.ndarray _getArray(Eye self):
         '''
         Return an explicit representation of the matrix as numpy-array.
         '''
```

### Comparing `fastmat-0.2a4/fastmat/Fourier.pxd` & `fastmat-0.2rc0/fastmat/Fourier.pxd`

 * *Files identical despite different names*

### Comparing `fastmat-0.2a4/fastmat/Fourier.pyx` & `fastmat-0.2rc0/fastmat/Fourier.pyx`

 * *Files 9% similar despite different names*

```diff
@@ -41,15 +41,15 @@
     >>> n = 4
     >>>
     >>> # construct the matrix
     >>> F = fm.Fourier(n)
 
     This yields a Fourier :math:`{\mathcal{F}}_4` matrix of size :math:`4`.
     As a library to provide the Fast Fourier Transform we used the one provided
-    by NumPy [1]_.
+    by NumPy.
 
     .. todo::
         - real valued transforms
     """
 
     property order:
         r"""Return the Order of the Fourier matrix.
@@ -65,40 +65,38 @@
         Initialize Fourier matrix instance.
 
         Parameters
         ----------
         order : int
             The order of the DFT matrix represented by this matrix instance.
 
-        **options:
-            See the list of special options below and
-            :py:meth:`fastmat.Matrix.__init__` for general options.
-
-        Options
-        -------
-        optimize : bool
+        optimize : bool, optional
             Allow application of the Bluestein algorithm for badly conditioned
             fourier transform orders.
 
             Defaults to True.
 
-        maxStage : int
+        maxStage : int, optional
             Specify the maximum butterfly element size for the FFT. Larger
             values can reduce the required order for the FFTs computed in the
             Bluestein case. However, increasing only makes sense as long as an
             efficient implementation of the butterfly structures exist in your
             BLAS.
 
             Defaults to 4, which is safe to assume on all architectures.
             However, most implementations support sizes of 5 and on some cpu
             architectures, also 7.
+
+        **options : optional
+            Additional optional keyworded arguments. Supports all optional
+            arguments supported by :py:class:`fastmat.Matrix`.
         '''
 
         cdef intsize paddedSize
-        cdef np.ndarray arrSamples, vecConv
+        cdef np.ndarray arrSamples, vecConv, arrArgument, arrBuffer
 
         cdef bint optimize = options.get('optimize', True)
         cdef int maxStage = options.get('maxStage', 4)
 
         if order < 1:
             raise ValueError("Fourier order cannot be smaller than 1.")
 
@@ -127,28 +125,36 @@
         # the presence (non-None) of self._vecConvHat controls the behaviour
         # of the forward() and backward() transforms.
         if self._numL > 0:
 
             # create the sampling grid
             arrSamples = np.linspace(0, self.order - 1, self.order)
 
-            # evaluate at these samples for the first numL elements
-            # of the vector
-            vecConv = _arrZero(1, self._numL, 1, np.NPY_COMPLEX128)
-            vecConv[: self.order] = np.exp(
-                +1j * (arrSamples ** 2) * np.pi / self.order)
+            # evaluate at these sample points for the first numL elements
+            # of the vector, also compose a premultiplication array for
+            # preprocessing input data prior to the convolution.
+            # Make use of trigonometric funtion symmetry for much faster
+            # compututation of the complex exponentials (compared to using
+            # np.exp(...) twice).
+            vecConv = _arrEmpty(1, self._numL, 1, np.NPY_COMPLEX128)
+            self._preMult = _arrEmpty(1, self.order, 0, np.NPY_COMPLEX128)
+            arrArgument = (arrSamples ** 2) * np.pi / self.order
+            arrBuffer = np.cos(arrArgument)
+            vecConv.real[:self.order] = arrBuffer
+            self._preMult[:] = arrBuffer
+            np.sin(arrArgument, out=arrBuffer)
+            vecConv.imag[:self.order] = arrBuffer
+            self._preMult[:] = -arrBuffer
 
             # now put a flipped version of the above at the very end to get
             # a circular convolution
             vecConv[self._numL - self.order + 1:] = vecConv[1:self.order][::-1]
 
-            # get a premultiplication array for preprocessing before the
-            # convolution
-            self._preMult = np.exp(
-                -1j * (arrSamples ** 2) * np.pi / self.order)
+            # ... and fill the remainder (in the middle of vecConv) with zeros
+            vecConv[self.order:self._numL - self.order + 1] = 0
 
             # transfer function of convolution
             self._vecConvHat = np.fft.fft(vecConv)
 
         # set properties of matrix
         self._initProperties(
             self._order, self._order, np.complex128, **options
```

### Comparing `fastmat-0.2a4/fastmat/Hadamard.pxd` & `fastmat-0.2rc0/fastmat/Hadamard.pxd`

 * *Files identical despite different names*

### Comparing `fastmat-0.2a4/fastmat/Hadamard.pyx` & `fastmat-0.2rc0/fastmat/Hadamard.pyx`

 * *Files 6% similar despite different names*

```diff
@@ -85,16 +85,16 @@
     >>>
     >>> # construct the matrix
     >>> H = fm.Hadamard(n)
 
     This yields a Hadamard matrix :math:`{\mathcal{H}}_4` of order :math:`4`,
     i.e. with :math:`16` rows and columns.
 
-    The algorithm we used is described in [2]_ and was implemented in
-    Cython [3]_.
+    The algorithm we used is described in :ref:`[2]<ref2>` and was implemented
+    in Cython :ref:`[3]<ref3>`.
     """
 
     property order:
         r"""Return the order of the hadamard matrix."""
 
         def __get__(self):
             return self._order
@@ -105,16 +105,17 @@
 
         Parameters
         ----------
         order : int
             The order of the Hadamard matrix to generate. The matrix data type
             is :py:class:`numpy.int8`
 
-        **options:
-            See :py:meth:`fastmat.Matrix.__init__`.
+        **options : optional
+            Optional keyworded arguments. Supports all optional arguments
+            supported by :py:class:`fastmat.Matrix`.
         '''
         if order < 1:
             raise ValueError("Hadamard: Order must be larger than 0.")
 
         cdef int maxOrder = sizeof(self.numRows) * 8 - 2
         if order > maxOrder:
             raise ValueError(
```

### Comparing `fastmat-0.2a4/fastmat/Kron.pxd` & `fastmat-0.2rc0/fastmat/Kron.pxd`

 * *Files identical despite different names*

### Comparing `fastmat-0.2a4/fastmat/Kron.pyx` & `fastmat-0.2rc0/fastmat/Kron.pyx`

 * *Files 2% similar despite different names*

```diff
@@ -42,16 +42,16 @@
         \begin{bmatrix}
             a_{11}  B    & \dots     & a_{1m}  B  \\
             \vdots       & \ddots    & \vdots     \\
             a_{n1}  B    & \dots     & a_{nm}  B
         \end{bmatrix}.
 
     We make use of a decomposition into a standard matrix product to speed up
-    the matrix-vector multiplication which is introduced in [4]_. This then
-    yields multiple benefits:
+    the matrix-vector multiplication which is introduced in :ref:`[4]<ref4>`.
+    This then yields multiple benefits:
 
         - It already brings down the complexity of the forward and backward
           projection if the factors :math:`A_i` have no fast transformations.
         - It is not necessary to compute the matrix representation of the
           product, which saves *a lot* of memory.
         - When fast transforms of the factors are available the calculations
           can be sped up further.
@@ -82,16 +82,17 @@
 
         Parameters
         ----------
         *matrices : :py:class:`fastmat.Matrix`
             The matrix instances to form a kronecker product of. Currently only
             square matrices are supported as kronecker product terms.
 
-        **options :
-            See :py:meth:`fastmat.Matrix.__init__`.
+        **options : optional
+            Additional keyworded arguments. Supports all optional arguments
+            supported by :py:class:`fastmat.Matrix`.
         '''
 
         cdef int ff, factorCount = len(matrices)
         cdef intsize numRows = 1
         cdef Matrix factor
 
         #check the number of matrices
```

### Comparing `fastmat-0.2a4/fastmat/LFSRCirculant.pxd` & `fastmat-0.2rc0/fastmat/LFSRCirculant.pxd`

 * *Files 6% similar despite different names*

```diff
@@ -22,16 +22,16 @@
 
 ctypedef np.uint32_t lfsrReg_t
 
 ################################################################################
 ################################################## class LfsrConv
 cdef class LFSRCirculant(Matrix):
 
-    cdef readonly int       size
-    cdef readonly lfsrReg_t taps
+    cdef readonly int       order
+    cdef readonly lfsrReg_t polynomial
     cdef readonly lfsrReg_t start
     cdef readonly lfsrReg_t period
 
     cdef public np.ndarray  _vecC
     cdef public np.ndarray  _states
 
     cdef np.ndarray _getStates(self)
```

### Comparing `fastmat-0.2a4/fastmat/LFSRCirculant.pyx` & `fastmat-0.2rc0/fastmat/LFSRCirculant.pyx`

 * *Files 10% similar despite different names*

```diff
@@ -24,44 +24,42 @@
 from .core.types cimport *
 from .core.cmath cimport *
 from .core.strides cimport *
 
 cdef inline np.int8_t lfsrOutBit(lfsrReg_t state) nogil:
     return (-1 if state & 1 else 1)
 
-cdef inline lfsrReg_t lfsrGenStep(lfsrReg_t state, lfsrReg_t taps,
+cdef inline lfsrReg_t lfsrGenStep(lfsrReg_t state, lfsrReg_t polynomial,
                                   lfsrReg_t mask) nogil:
-    cdef lfsrReg_t tmp = state & taps
+    cdef lfsrReg_t tmp = state & polynomial
     tmp ^= tmp >> 1
     tmp ^= tmp >> 2
     tmp = (tmp & 0x11111111) * 0x11111111
     if tmp & 0x10000000:
         state |= mask
 
     return state >> 1
 
-cdef inline lfsrReg_t lfsrTapStep(lfsrReg_t state, lfsrReg_t taps,
+cdef inline lfsrReg_t lfsrTapStep(lfsrReg_t state, lfsrReg_t polynomial,
                                   lfsrReg_t mask) nogil:
     state = state << 1
     if (state & mask) != 0:
-        state = state ^ (taps | mask)
+        state = state ^ (polynomial | mask)
 
     return state
 
 cdef class LFSRCirculant(Matrix):
     r"""
 
-
     Linear Feedback Shift Registers (LFSR) as implemented in this class are
     finite state machines generating sequences of symbols from the finite
     field :math:`F=[-1, +1]`. A shift register of size :math:`N` is a cascade
     of :math:`N` storage elements :math:`a_n` for :math:`n = 0,\dots,N-1`,
     each holding one symbol of :math:`F`. The state of the shift register is
-    defined by the states of :math:`a_0,\dots,a_{N-1}`.
-    [5]_
+    defined by the states of :math:`a_0,\dots,a_{N-1}`. :ref:`[5]<ref5>`
 
     The next state of the register is generated from the current state by
     moving the contents of each storage element to the next lower index by
     setting :math:`a_{n-1} = a_n` for :math:`n \geq 1`, hence the name shift
     register. The element :math:`a_0` of the current state is discarded
     completely in the next state. A subset :math:`T` of all storage elements
     with cardinality of 1 or greater is used for generating the next symbol
@@ -89,20 +87,19 @@
     :math:`a_n = +1` and :math:`r_n = 1` sets :math:`a_n = -1`. If no :math:`r`
     is given, it is assumed to be all-ones.
 
     >>> # import the package
     >>> import fastmat as fm
     >>>
     >>> # construct the parameter
-    >>> size = 4
-    >>> taps = 0b1001
-    >>> initial = 0b1010
+    >>> polynomial = 0b11001
+    >>> start = 0b1010
     >>>
     >>> # construct the matrix
-    >>> L = fm.LFSRCirculant(size, taps, initial)
+    >>> L = fm.LFSRCirculant(polynomial, start)
     >>> s = L.vecC
 
     This yields a Circulant matrix where the column-definition vector is the
     output of a LFSR of size 4, which is configured to generate a maximum
     length sequence of length 15 and a cyclic shift corresponding to the given
     initial state.
 
@@ -117,14 +114,32 @@
         & \vdots &    & \ddots &    \\
         -1 &   -1   & -1 &        & +1 \\
         \end{bmatrix}
 
     This class depends on ``Hadamard``.
     """
 
+    property size:
+        '''Deprecated. Will be removed in future releases'''
+        def __get__(self):
+            import warnings
+            warnings.warn(
+                'size is deprecated. WIll be removed in furure releases.',
+                FutureWarning
+            )
+            return self.order
+
+    property taps:
+        '''Deprecated. See .polynomial'''
+        def __get__(self):
+            import warnings
+            warnings.warn('taps is deprecated. Use polynomial.',
+                          FutureWarning)
+            return self.polynomial
+
     property vecC:
         r"""Return the sequence defining the circular convolution.
 
         *(read only)*
         """
 
         def __get__(self):
@@ -137,80 +152,77 @@
         *(read-only)*
         """
 
         def __get__(self):
             return (self._getStates() if self._states is None
                     else self._states)
 
-    def __init__(self, int regSize, taps, start, **options):
+    def __init__(self, polynomial, start, **options):
         '''
         Initialize a LFSR Circulant matrix instance.
 
         The definition vector of the circulant matrix is defined by the output
         [+1/-1] of a binary Linear Feedback Shift Register (LFSR) with the
         given defining parameters over one period.
 
         Parameters
         ----------
-        regSize : int
-            The size of the register, defined as the number of its storage
-            elements. Only positive, non-zero values up to 31 are allowed.
-
-        taps : int
-            The tap configuration word. Every set bit k in this value
-            corresponds to one feedback tap at storage element k of the
-            register or the monome x^k of the generating polynomial that forms
-            a cycle in the galois field GF2 of order `regSize`. The bit
-            corresponding to `regSize` is implicitly assumed to be set and
-            may or may not be contained in the `taps` definition word.
+        polynomial : int
+            The characteristic polynomial corresponding to the shift register
+            sequence. Every set bit k in this value corresponds to one feedback
+            tap at storage element k of the register or the monome x^k of the
+            characterisctic polynomial that forms a cycle in the galois field
+            GF2 of the order corresponding to the highest non-zero monome x^K
+            in the polynomial.
 
         start : int
             The initial value of the storage elements of the register.
 
-        **options :
-            See :py:meth:`fastmat.Matrix.__init__`.
+        **options : optional
+            Additional keyworded arguments. Supports all optional arguments
+            supported by :py:class:`fastmat.Matrix`.
+
+            All optional arguments will be passed on to all
+            :py:class:`fastmat.Matrix` instances that are generated during
+            initialization.
         '''
 
-        cdef lfsrReg_t mask = 1 << regSize
+        self.polynomial = polynomial
+        self.order = 0
+        cdef lfsrReg_t mask = 1
+        while (~mask & polynomial > mask):
+            mask <<=1
+            self.order += 1
+
+        mask = 1 << self.order
 
         # determine register size (determines order of embedded Hadamard)
-        self.taps = taps & (mask - 1)
-        self.size = regSize
         self.start = start & (mask - 1)
 
-        if self.size > 31 or self.size < 1:
-            raise ValueError("Register sizes only supported from 1 to 31.")
-
-        if self.taps > mask:
-            raise ValueError("Tap positions exceeding register size.")
-
-        if self.taps == 0:
-            raise ValueError("Register must feature at least one feedback tap.")
+        if self.order > 31 or self.order < 1:
+            raise ValueError("Only polynomials of order 1 to 31 are supported.")
 
         if self.start == 0:
-            raise ValueError("Register reset state must be non-zero.")
+            raise ValueError("Initial state must be non-zero.")
 
         # generate embedded Hadamard matrix
-        self._content = (Hadamard(self.size), )
+        self._content = (Hadamard(self.order), )
 
         # determine matrix size (square) by determining the period of the
         # sequence generated by the given register configuration
-        cdef lfsrReg_t state = lfsrGenStep(self.start, self.taps, mask)
+        cdef lfsrReg_t state = lfsrGenStep(self.start, self.polynomial, mask)
         cdef intsize period = 1
 
         while state != self.start:
-            state = lfsrGenStep(state, taps, mask)
+            state = lfsrGenStep(state, polynomial, mask)
             period += 1
             if period >= mask or state == 0:
                 raise ValueError(
                     "Register configuration produces invalid sequence.")
 
-        if period <= 1:
-            raise ValueError("Register produces static output.")
-
         self.period = period
 
         # extension note: it should be possible -- by properly tweaking the
         # involved permutation matrices -- to also construct a convolution
         # matrix of a section of the sequence. For that it might be neccessary
         # to have different starting values for the two polynomials generating
         # the actual permutation operations. If that turns out true, a fourth
@@ -265,52 +277,52 @@
 
     cdef np.ndarray _getStates(self):
         cdef intsize nn
         cdef np.ndarray arrStates
         cdef lfsrReg_t[:] mvStates
 
         cdef ntype typeStates = np.dtype(np.uint32).type_num
-        cdef lfsrReg_t mask = 1 << self.size
-        cdef lfsrReg_t taps = self.taps
+        cdef lfsrReg_t mask = 1 << self.order
+        cdef lfsrReg_t polynomial = self.polynomial
         cdef lfsrReg_t state = self.start
 
         arrStates = _arrEmpty(1, self.numRows, 1, typeStates)
         mvStates = arrStates
         for nn in range(self.numRows):
             mvStates[nn] = state & (mask - 1)
-            state = lfsrGenStep(state, taps, mask)
+            state = lfsrGenStep(state, polynomial, mask)
 
         self._states = arrStates
         return arrStates
 
     cdef np.ndarray _getVecC(self):
-        cdef lfsrReg_t mask = 1 << self.size
-        cdef lfsrReg_t taps = self.taps
+        cdef lfsrReg_t mask = 1 << self.order
+        cdef lfsrReg_t polynomial = self.polynomial
         cdef lfsrReg_t state = self.start
         cdef intsize nn
 
         cdef np.ndarray arrRes
         cdef np.int8_t[:] mvRes
         cdef ntype typeElement = np.dtype(np.int8).type_num
 
         arrRes = _arrEmpty(1, self.numRows, 1, typeElement)
         mvRes = arrRes
         for nn in range(self.numRows):
             mvRes[nn] = lfsrOutBit(state)
-            state = lfsrGenStep(state, taps, mask)
+            state = lfsrGenStep(state, polynomial, mask)
 
         self._vecC = arrRes
         return self._vecC
 
     cdef void _core(self, np.ndarray arrIn, np.ndarray arrOut,
                     bint flipIn, bint flipOut):
 
         cdef intsize ii, nn, N = arrIn.shape[0], M = arrIn.shape[1]
-        cdef lfsrReg_t state, mask  = 1 << self.size
-        cdef lfsrReg_t taps         = self.taps
+        cdef lfsrReg_t state, mask  = 1 << self.order
+        cdef lfsrReg_t polynomial   = self.polynomial
         cdef np.ndarray arrData
         cdef STRIDE_s strIn, strData, strOut
 
         # initialize data Array, no zero init required for maximum length seqs
         if N == mask - 1:
             arrData = _arrEmpty(2, mask, M, getNumpyType(arrIn), False)
         else:
@@ -350,15 +362,15 @@
         # However, index 0 will be mapped directly to the can as it literally
         # starts after the array data. After that however indexing begins with
         # the last row for index 1.
         if flipIn:
             strideFlipVectors(&strIn)
 
         for nn in range(0, N - 1):
-            state = lfsrGenStep(state, taps, mask)
+            state = lfsrGenStep(state, polynomial, mask)
             opCopyVector(&strData, state, &strIn, nn)
 
         # apply hadamard-walsh transform from arrData to arrData
         arrData = self._content[0].forward(arrData)
 
         # reinit slice as arrData has changed
         strideInit(&strData, arrData, 1)
@@ -375,15 +387,15 @@
         strideSliceVectors(&strOut, 1, -1, 1)        # equivalent to strOut[1:]
 
         # same addressing hack as above
         if flipOut:
             strideFlipVectors(&strOut)
 
         for nn in range(0, N - 1):
-            state = lfsrTapStep(state, taps, mask)
+            state = lfsrTapStep(state, polynomial, mask)
             opCopyVector(&strOut, nn, &strData, state)
 
     ############################################## class forward / backward
     cpdef _forwardC(self, np.ndarray arrX, np.ndarray arrRes,
                     ftype typeX, ftype typeRes):
         # dispatch input ndarray to type specialization
         self._core(arrX, arrRes, True, False)
@@ -393,25 +405,25 @@
         # dispatch input ndarray to type specialization
         self._core(arrX, arrRes, False, True)
 
     ############################################### class reference
     cpdef np.ndarray _reference(self):
         cdef np.ndarray arrRes, vecSequence
         cdef np.int8_t[:] mvSequence
-        cdef int ii, state, taps, mask, tmp, cnt
+        cdef int ii, state, polynomial, mask, tmp, cnt
 
         state = self.start
-        taps = self.taps
-        mask = 1 << self.size
+        polynomial = self.polynomial
+        mask = 1 << self.order
         vecSequence = np.empty((self.numRows, ), dtype=np.int8)
         mvSequence = vecSequence
         for ii in range(self.numRows):
             mvSequence[ii] = (state & 1) * -2 + 1
 
-            tmp = state & taps
+            tmp = state & polynomial
             cnt = 0
             while tmp:
                 cnt ^= 1
                 tmp &= tmp - 1
 
             if cnt:
                 state |= mask
@@ -426,56 +438,56 @@
 
     ############################################## class inspection, QM
     def _getTest(self):
         from .inspect import TEST, dynFormat
         return {
             TEST.COMMON: {
                 # define matrix sizes and parameters
-                'size'          : 4,
-                'taps'          : TEST.Permutation([0x9, 0x7]),
-                'start'         : TEST.Permutation([0x5, 0x1]),
-                'length'        : (lambda param: (15 if param['taps'] == 0x9
-                                                  else 7)),
-                TEST.NUM_ROWS   : 'length',
+                'polynomial'    : TEST.Permutation([0x19, 0x17]),
+                'start'         : TEST.Permutation([0xD, 0x1]),
+                'period'        : (
+                    lambda param: (15 if param['polynomial'] == 0x19 else 7)
+                ),
+                TEST.NUM_ROWS   : 'period',
                 TEST.NUM_COLS   : TEST.NUM_ROWS,
 
                 # define constructor for test instances and naming of test
                 TEST.OBJECT     : LFSRCirculant,
-                TEST.INITARGS   : ['size', 'taps', 'start'],
-                TEST.NAMINGARGS : dynFormat("%d:%x=%x", 'size', 'taps', 'start')
+                TEST.INITARGS   : ['polynomial', 'start'],
+                TEST.NAMINGARGS : dynFormat(
+                    "%x,%x", 'polynomial', 'start'
+                )
             },
             TEST.CLASS: {},
             TEST.TRANSFORMS: {}
         }
 
     def _getBenchmark(self):
         from .inspect import BENCH
 
         # specify tap configurations for various maximum-length-sequences
         # the list contains the tap configurations of registers corresponding
         # to a register size of the list index of the element + 1.
         db = {ll + 1: tt for ll, tt in enumerate([
-            0x1, 0x3, 0x3, 0x9, 0x05, 0x21, 0x09, 0xC3,
-            0x011, 0x081, 0x303, 0xC11, 0x0C41, 0x1803, 0x4001,
-            0xA011, 0x04001, 0x00801, 0x64001, 0x20001, 0x080001,
-            0x200001, 0x040001, 0xC20001, 0x0400001, 0x3100001, 0x6400001,
-            0x2000001, 0x08000001, 0x30000081, 0x10000001
+            0x3, 0x7, 0xB, 0x19, 0x25, 0x61, 0x89, 0x1C3,
+            0x211, 0x481, 0xB03, 0x1C11, 0x2C41, 0x5803, 0xC001,
+            0x1A011, 0x24001, 0x40801, 0xE4001, 0x120001, 0x280001,
+            0x600001, 0x840001, 0x1C20001, 0x2400001, 0x7100001, 0xE400001,
+            0x12000001, 0x28000001, 0x70000081, 0x90000001
         ])}
 
         return {
             BENCH.COMMON: {
                 BENCH.FUNC_GEN  : (
-                    lambda c: LFSRCirculant(c, db[c], 0xFFFFFFFF)
+                    lambda c: LFSRCirculant(db[c], 0xFFFFFFFF)
                 ),
                 BENCH.FUNC_SIZE : (lambda c: (2 ** c) - 1),
                 BENCH.FUNC_STEP : (lambda c: c + 1),
             },
             BENCH.FORWARD: {},
             BENCH.OVERHEAD: {},
             BENCH.DTYPES: {
                 BENCH.FUNC_GEN  : (
-                    lambda c, dt: LFSRCirculant(
-                        c, db[c], 0xFFFFFFFF, minType=dt
-                    )
+                    lambda c, dt: LFSRCirculant(db[c], 0xFFFFFFFF, minType=dt)
                 )
             }
         }
```

### Comparing `fastmat-0.2a4/fastmat/LowRank.pxd` & `fastmat-0.2rc0/fastmat/LowRank.pxd`

 * *Files identical despite different names*

### Comparing `fastmat-0.2a4/fastmat/LowRank.pyx` & `fastmat-0.2rc0/fastmat/LowRank.pyx`

 * *Files 2% similar despite different names*

```diff
@@ -112,16 +112,17 @@
             A 2d array corresponding to U of the singular value decomposition
             of the matrix.
 
         arrU : :py:class:`numpy.ndarray`
             A 2d array corresponding to V of the singular value decomposition
             of the matrix.
 
-        **options :
-            See :py:meth:`fastmat.Matrix.__init__`.
+        **options : optional
+            Additional keyworded arguments. Supports all optional arguments
+            supported by :py:class:`fastmat.Matrix`.
         '''
 
         # complain if dimension does not match
         if vecS.ndim != 1:
             raise ValueError(
                 "Singular value vector must have exactly one active dimension.")
```

### Comparing `fastmat-0.2a4/fastmat/Matrix.pxd` & `fastmat-0.2rc0/fastmat/Matrix.pxd`

 * *Files 14% similar despite different names*

```diff
@@ -77,18 +77,22 @@
     cdef public Matrix      _gram
     cdef public np.ndarray  _colNorms
     cdef public np.ndarray  _rowNorms
     cdef public Matrix      _colNormalized
     cdef public Matrix      _rowNormalized
     cdef public object      _largestEigenValue
     cdef public object      _largestSingularValue
-    cdef public object      _scipyLinearOperator
-    cdef public Matrix      _T
-    cdef public Matrix      _H
-    cdef public Matrix      _conj
+    # cache for largestSingularVectors
+    cdef public tuple       _largestSingularVectors
+    cdef public object      _scipyLinearOperator # interface to scipy
+    cdef public Matrix      _T                   # cache for transpose matrix
+    cdef public Matrix      _H                   # cache for adjunct matrix
+    cdef public Matrix      _conj                # cache for conjugate matrix
+    cdef public Matrix      _inverse             # cache for inv. matrix
+    cdef public Matrix      _pseudoInverse       # cache for ps. inv.  matrix
 
     cdef readonly intsize   numRows              # row-count of matrix
     cdef readonly intsize   numCols              # column-count of matrix
     cdef readonly ntype     numpyType            # numpy typenum
     cdef readonly ftype     fusedType            # fastmat fused typenum
     cdef readonly ftype     _minFusedType        # minimal fused type used
     #                                            # internally for transform
@@ -123,14 +127,16 @@
     cpdef np.ndarray _getColNorms(self)
     cpdef np.ndarray _getRowNorms(self)
     cpdef Matrix _getColNormalized(self)
     cpdef Matrix _getRowNormalized(self)
     cpdef Matrix _getT(self)
     cpdef Matrix _getH(self)
     cpdef Matrix _getConj(self)
+    cpdef Matrix _getInverse(self)
+    cpdef Matrix _getPseudoInverse(self)
 
     ############################################## computation profiling
     cpdef tuple _getComplexity(self)
     cdef void _initProfiles(self)
     cpdef _exploreNestedProfiles(self)
     cpdef tuple estimateRuntime(self, intsize numVectors=?)
 
@@ -155,7 +161,21 @@
 
 cdef Matrix getConjugate(Matrix)
 cdef class Conjugate(Matrix):
     cdef public Matrix _nested                   # nested fastmat baseclass
 
 cdef class Transpose(Hermitian):
     cdef public Matrix _nestedConj               # nested fastmat baseclass
+
+cdef class Inverse(Matrix):
+    cdef public Matrix _nested                   # nested fastmat baseclass
+    cdef object _linearOperator                  # nested linear operator
+    cdef object _solver                          # nested linear operator
+    cpdef np.ndarray _solveForward(self, np.ndarray)
+    cpdef np.ndarray _solveBackward(self, np.ndarray)
+
+cdef class PseudoInverse(Matrix):
+    cdef public Matrix _nested                   # nested fastmat baseclass
+    cdef object _linearOperator                  # nested linear operator
+    cdef object _solver                          # nested linear operator
+    cpdef np.ndarray _solveForward(self, np.ndarray)
+    cpdef np.ndarray _solveBackward(self, np.ndarray)
```

### Comparing `fastmat-0.2a4/fastmat/Matrix.pyx` & `fastmat-0.2rc0/fastmat/Matrix.pyx`

 * *Files 2% similar despite different names*

```diff
@@ -102,23 +102,23 @@
         Parameters
         ----------
         targetInstance : :py:class:`fastmat.Matrix`
             The fastmat matrix instance a call profile needs to be generated
             for.
 
         targetCall : callable
-            ?
+            TODO: Needs to be specified.
 
-        cplxAlg : int
+        cplxAlg : int, optional
             The complexity estimate for the transforms implemented in the
             matrix class of `targetInstance`.
 
             Defaults to 0.
 
-        cplxBypass : int
+        cplxBypass : int, optional
             The complexity estimate for the (bypass) transforms implemented in
             the :py:class:`fastmat.Matrix` base class.
 
             Defaults to 0.
         '''
 
         # store given complexity estimates in profile
@@ -287,15 +287,15 @@
 ################################################## class Matrix
 cdef class Matrix(object):
     r"""Matrix Base Class
 
 
     **Description:**
     The baseclass of all matrix classes in fastmat. It also serves as wrapper
-    around the standard Numpy Array [1]_.
+    around the standard Numpy Array :ref:`[1]<ref1>`.
     """
 
     ############################################## basic class properties
     property dtype:
         # r"""Report the matrix elements' data type
         #
         # *(read-only)*
@@ -808,16 +808,16 @@
         .. math::
              A =  U  \Sigma  V^{\rm H},
 
         where :math:`U` and :math:`V` are matrices of the appropriate
         dimensions. This is done via the so called power iteration of
         :math:`A^{\rm H} \cdot  A`.
 
-        - Input matrix :math:`A`, parameter :math:`0 < \varepsilon \ll 1` as a
-        stopping criterion
+        - Input matrix :math:`A`, parameter :math:`0 < \varepsilon \ll 1` as \
+          a stopping criterion
         - Output largest singular value :math:`\sigma_{\rm max}( A)`
 
         .. note::
             This algorithm performs well if the two largest singular values
             are not very close to each other on a relative scale. Otherwise
             it might get trouble converging properly.
 
@@ -1016,15 +1016,21 @@
         # accuracy of norms also when constructing meta classed of larger type
         diagType = np.float64
 
         # array that contains the norms of each column
         cdef np.ndarray arrNorms = np.empty(self.numCols, dtype=diagType)
 
         # number of elements we consider at once during normalization
-        cdef intsize numStrideSize = 256
+        # Scale chunk size to fit a memory buffer of at most 16M
+        cdef intsize numStrideSize = max(
+            1, min(
+                1024,
+                (16777216 // typeInfo[self.fusedType].dsize) // self.numRows
+            )
+        )
 
         cdef np.ndarray arrSelector = np.zeros(
             (self.numCols, min(numStrideSize, self.numCols)),
             dtype=diagType)
 
         cdef intsize ii
         for ii in range(0, self.numCols, numStrideSize):
@@ -1070,15 +1076,21 @@
         # accuracy of norms also when constructing meta classed of larger type
         diagType = np.float64
 
         # array that contains the norms of each column
         cdef np.ndarray arrNorms = np.empty(self.numRows, dtype=diagType)
 
         # number of elements we consider at once during normalization
-        cdef intsize numStrideSize = 256
+        # Scale chunk size to fit a memory buffer of at most 16M
+        cdef intsize numStrideSize = max(
+            1, min(
+                1024,
+                (16777216 // typeInfo[self.fusedType].dsize) // self.numCols
+            )
+        )
 
         cdef np.ndarray arrSelector = np.zeros(
             (self.numRows, min(numStrideSize, self.numRows)),
             dtype=diagType)
 
         cdef intsize ii
         for ii in range(0, self.numRows, numStrideSize):
@@ -1215,15 +1227,61 @@
         self._conj = self._getConj()
         return self._conj
 
     cpdef Matrix _getConj(self):
         '''Internally overloadable method for customizing self.getConj.'''
         return getConjugate(self)
 
-    ############################################## deprecated properties
+    property inverse:
+        r"""Return the inverse
+
+        *(read-only)*
+        """
+
+        def __get__(self):
+            if self._inverse is None:
+                return self.getInverse()
+            else:
+                return self._inverse
+
+    def getInverse(self):
+        r"""
+        Return the hermitian transpose of this matrix as fastmat matrix.
+        """
+        self._inverse = self._getInverse()
+        return self._inverse
+
+    cpdef Matrix _getInverse(self):
+        '''Internally overloadable method for self.inverse.'''
+        return Inverse(self)
+
+    property pseudoInverse:
+        r"""Return the moore penrose inverse
+
+        *(read-only)*
+        """
+
+        def __get__(self):
+            if self._pseudoInverse is None:
+                return self.getPseudoInverse()
+            else:
+                return self._pseudoInverse
+
+    def getPseudoInverse(self):
+        r"""
+        Return the hermitian transpose of this matrix as fastmat matrix.
+        """
+        self._pseudoInverse = self._getPseudoInverse()
+        return self._pseudoInverse
+
+    cpdef Matrix _getPseudoInverse(self):
+        '''Internally overloadable method for self.pseudoInverse.'''
+        return PseudoInverse(self)
+
+    ############################################## numN deprecation warning
     property numN:
         def __get__(self):
             import warnings
             warnings.warn('numN is deprecated. Use numRows.', FutureWarning)
             return self.numRows
 
     property numM:
@@ -1387,70 +1445,63 @@
 
         Parameters
         ----------
         arrMatrix : :py:class:`numpy.ndarray`
             A 2d array representing a dense matrix to be cast as a fastmat
             matrix.
 
-        **options:
-            See the list of general options below, that also apply to all other
-            fastmat matrix types.
-
-
-        options in `**options`
-        ----------------------
-        forceContiguousInput : bool
+        forceContiguousInput : bool, optional
             If set, the input array is forced to be contiguous in the style as
             specified by `fortranStyle`. If the input array already fulfils the
             requirement nothing is done.
 
-            Defaults to False
+            Defaults to False.
 
-        widenInputDatatype : bool
+        widenInputDatatype : bool, optional
             If set, the data type of the input array is promoted to at least
             match the output data type of the operation. Just like the
             `minType` option this parameter controls the accumulator width,
             however dynamically according to the output data type in this case.
 
-            Defaults to False
+            Defaults to False.
 
-        fortranStyle : bool
+        fortranStyle : bool, optional
             Control the style of contiguousity to be enforced by
             forceConfiguousInput. If this option is set to True, Fortran-style
             ordering (contiguous along columns) is enforced, if False C-Style
-            (contiguous along rows)
+            (contiguous along rows).
 
-            Defaults to True
+            Defaults to True.
 
-        minType : bool
+        minType : bool, optional
             Specify a minimum data type for the input array to a transform. The
             input array data type will be promoted to at least the data type
             specified in this option before performing the actual transforms.
             Using this option is strongly advised for cases where small data
             types of both input array and matrix could cause range overflows
             otherwise, as the output data type promotion rules do not consider
             avoiding accumulator overflows due to performance reasons.
 
-            Defaults to :py:`numpy.int8`
+            Defaults to :py:class:`numpy.int8`.
 
-        bypassAllow : bool
+        bypassAllow : bool, optional
             Allow bypassing the implemented :py:meth:`fastmat.Matrix.forward`
             and :py:meth:`fastmat.Matrix.backward` transforms with dense
             matrix-vector products if runtime estimates suggest this is faster
             than using the implemented transforms. This requires valid
             calibration data to be available for the class of the to-be-created
             instance itself and the :py:class:`fastmat.Matrix` base class at
             the time the new instance is created. If no valid performance
             calibration data exists this parameter is ignored and the
             implemented transforms will be used always.
 
             Defaults to the value set in the package-wide
             :py:class:`fastmat.flags` options.
 
-        bypassAutoArray : bool
+        bypassAutoArray : bool, optional
             Prevents the automatic generation of a dense matrix representation
             that would be used for bypassing the implemented transforms in case
             the performance profiles suggest this would be faster, if set to
             True. This is heavily advised if the matrix is unfeasibly large for
             a dense representation and does not feature fast transforms.
 
             Defaults to the value as set in the package-wide
@@ -1998,34 +2049,36 @@
                     TEST.OBJECT     : Matrix,
                     TEST.INITARGS   : (lambda param: [param['arrM']()]),
                     TEST.NAMINGARGS : dynFormat("%s", 'arrM')
                 },
                 TEST.CLASS: {},
                 TEST.TRANSFORMS: {}
             }
-        elif isinstance(self, (Hermitian, Conjugate, Transpose)):
+        elif isinstance(
+            self, (Hermitian, Conjugate, Transpose)
+        ):
             # Test code for the three Transposition classes that are also
             # defined in this submodule. As the Transpositions are directly
             # derived from the Matrix base class we can put the relevant code
             # directly in here and adapt it to work for all three classes.
 
             # Note that the resulting matrix shape differs for Hermitian and
             # Transpose so we must reflect this when specifying the shape of the
             # to-be-generated data array. As Permutations of a dimension is not
             # uncommon the corresponding fields must be linked in DATASHAPE
             numRows = 35
             numCols = 30
-            swap = isinstance(self, Conjugate)
+            swap = isinstance(self, (Conjugate))
             return {
                 TEST.COMMON: {
                     TEST.NUM_ROWS   : numRows,
-                    TEST.NUM_COLS   : TEST.Permutation([
-                        numCols, TEST.NUM_ROWS
-                    ]),
-                    'mType'         : TEST.Permutation(TEST.FEWTYPES),
+                    TEST.NUM_COLS   : TEST.Permutation(
+                        [numCols, TEST.NUM_ROWS]
+                    ),
+                    'mType'         : TEST.Permutation(TEST.FLOATTYPES),
                     TEST.PARAMALIGN : TEST.Permutation(TEST.ALLALIGNMENTS),
                     'arrM'          : TEST.ArrayGenerator({
                         TEST.DTYPE  : 'mType',
                         TEST.SHAPE  : (TEST.NUM_ROWS, TEST.NUM_COLS),
                         TEST.ALIGN  : TEST.PARAMALIGN
                     }),
                     TEST.DATASHAPE  : (TEST.NUM_COLS if swap else TEST.NUM_ROWS,
@@ -2035,14 +2088,49 @@
                     TEST.OBJECT     : self.__class__,
                     TEST.INITARGS   : (lambda param: [Matrix(param['arrM']())]),
                     TEST.NAMINGARGS : dynFormat("%s", 'arrM')
                 },
                 TEST.CLASS: {},
                 TEST.TRANSFORMS: {}
             }
+        elif isinstance(
+            self, (Inverse, PseudoInverse)
+        ):
+            # Test code for the two Inversion classes that are also
+            # defined in this submodule.
+            numRows = 10
+            numCols1 = 9
+            numCols2 = 11
+            square = isinstance(self, (Inverse))
+            return {
+                TEST.COMMON: {
+                    TEST.NUM_ROWS   : numRows,
+                    TEST.NUM_COLS   : (TEST.NUM_ROWS if square else
+                                       TEST.Permutation(
+                                           [numCols1, numCols2, TEST.NUM_ROWS]
+                                       )),
+                    'mType'         : TEST.Permutation(TEST.FLOATTYPES),
+                    TEST.PARAMALIGN : TEST.Permutation(TEST.ALLALIGNMENTS),
+                    'arrM'          : TEST.ArrayGenerator({
+                        TEST.DTYPE  : 'mType',
+                        TEST.SHAPE  : (TEST.NUM_ROWS, TEST.NUM_COLS),
+                        TEST.ALIGN  : TEST.PARAMALIGN
+                    }),
+                    TEST.DATASHAPE  : (TEST.NUM_ROWS, TEST.DATACOLS),
+                    TEST.DATASHAPE_T: (TEST.NUM_COLS, TEST.DATACOLS),
+                    TEST.OBJECT     : self.__class__,
+                    TEST.INITARGS   : (lambda param: [Matrix(param['arrM']())]),
+                    TEST.NAMINGARGS : dynFormat("%s", 'arrM'),
+                    TEST.TOL_POWER  : 10.0,
+                    TEST.TOL_MINEPS    : 1e-2,
+                    TEST.CHECK_DATATYPE: False
+                },
+                TEST.CLASS: {},
+                TEST.TRANSFORMS: {}
+            }
         else:
             # Any other class should go and define its own tests!
             return {}
 
     def _getBenchmark(self):
         '''Return benchmark configuration for this matrix class.'''
         from .inspect import BENCH
@@ -2060,15 +2148,17 @@
                 },
                 BENCH.DTYPES: {
                     BENCH.FUNC_GEN  :
                         (lambda c, dt: Matrix(np.zeros((2 ** c, 2 ** c),
                                                        dtype=dt)))
                 }
             }
-        elif isinstance(self, (Hermitian, Conjugate, Transpose)):
+        elif isinstance(
+            self, (Hermitian, Conjugate, Transpose, Inverse, PseudoInverse)
+        ):
             # Benchmark code for the three Transposition classes that are also
             # defined in this submodule. As the Transpositions are directly
             # derived from the Matrix base class we can put the relevant code
             # directly in here and adapt it to work for all three classes.
             # Also note, that we can use the Eye again as the property override
             # of Eye.{T,conj,H} does not grip if instantiated directly through
             # the class constructor
@@ -2249,21 +2339,21 @@
         cdef float complexity = self.numRows + self.numCols
         return (complexity, complexity)
 
     ############################################## class forward / backward
     cpdef _forwardC(self, np.ndarray arrX, np.ndarray arrRes,
                     ftype typeX, ftype typeRes):
         cdef np.ndarray arrInput = _conjugate(arrX)
-        self._nested.forwardC(arrInput, arrRes, typeX, typeRes)
+        self._nested._forwardC(arrInput, arrRes, typeX, typeRes)
         _conjugateInplace(arrRes)
 
     cpdef _backwardC(self, np.ndarray arrX, np.ndarray arrRes,
                      ftype typeX, ftype typeRes):
         cdef np.ndarray arrInput = _conjugate(arrX)
-        self._nested.backwardC(arrInput, arrRes, typeX, typeRes)
+        self._nested._backwardC(arrInput, arrRes, typeX, typeRes)
         _conjugateInplace(arrRes)
 
     cpdef np.ndarray _forward(self, np.ndarray arrX):
         cdef np.ndarray arrRes = self._nested._forward(_conjugate(arrX))
         _conjugateInplace(arrRes)
         return arrRes
 
@@ -2341,7 +2431,126 @@
 
     cpdef Matrix _getConj(self):
         return Hermitian(self._nestedConj)
 
     ########################################## references: test / benchmark
     cpdef np.ndarray _reference(self):
         return self._nestedConj._reference().T
+
+
+cdef class Inverse(Matrix):
+    r""" Inverse of a Matrix
+
+    This class is implemented by always solving a system of linear equations
+    in order to act out the forward transform of a given matrix.
+    """
+    ############################################## class methods
+
+    def __init__(self, Matrix matrix):
+        '''
+        Initialize an instance of an inverted matrix.
+
+        Parameters
+        ----------
+        matrix : :py:class:`fastmat.Matrix`
+            The matrix instance to be inverse.
+        '''
+        from scipy.sparse.linalg import lgmres
+
+        if not isinstance(matrix, Matrix):
+            raise TypeError("Inverse: Not a fastmat Matrix")
+
+        if matrix.shape[0] != matrix.shape[1]:
+            raise ValueError("Inverse: Matrix not square, so not invertible.")
+
+        self._nested = matrix
+        self._content = (matrix, )
+        self._cythonCall = False
+        self._initProperties(
+            matrix.shape[0],
+            matrix.shape[0],
+            np.promote_types(matrix.dtype, np.float32),
+            **matrix._getProperties()
+        )
+        self._linearOperator = matrix.scipyLinearOperator
+        self._solver = lgmres
+
+    cpdef np.ndarray _solveForward(self, np.ndarray arrX):
+        return self._solver(self._linearOperator, arrX, atol=1e-12)[0]
+
+    cpdef np.ndarray _solveBackward(self, np.ndarray arrX):
+        return self._solver(self._linearOperator.H, arrX, atol=1e-12)[0]
+
+    def __repr__(self):
+        return "<%s.(^-1)>" %(self._nested.__repr__())
+
+    cpdef np.ndarray _forward(self, np.ndarray arrX):
+        return np.apply_along_axis(
+            self._solveForward, 0, arrX
+        )
+
+    cpdef np.ndarray _backward(self, np.ndarray arrX):
+        return np.apply_along_axis(
+            self._solveBackward, 0, arrX
+        )
+
+    cpdef np.ndarray _reference(self):
+        import numpy.linalg as npl
+        return npl.inv(self._nested.reference())
+
+
+cdef class PseudoInverse(Matrix):
+    r""" Inverse of a Matrix
+
+    This class is implemented by always solving a system of linear equations
+    in order to act out the forward transform of a given matrix.
+    """
+    ############################################## class methods
+
+    def __init__(self, Matrix matrix):
+        '''
+        Initialize an instance of a pseudo inverse matrix.
+
+        Parameters
+        ----------
+        matrix : :py:class:`fastmat.Matrix`
+            The matrix instance that we want the pseudo inverse of.
+        '''
+        from scipy.sparse.linalg import lsqr
+
+        if not isinstance(matrix, Matrix):
+            raise TypeError("Inverse: Not a fastmat Matrix")
+
+        self._nested = matrix
+        self._content = (matrix, )
+        self._cythonCall = False
+        self._initProperties(
+            matrix.shape[1],
+            matrix.shape[0],
+            np.promote_types(matrix.dtype, np.float32),
+            **matrix._getProperties()
+        )
+        self._linearOperator = matrix.scipyLinearOperator
+        self._solver = lsqr
+
+    cpdef np.ndarray _solveForward(self, np.ndarray arrX):
+        return self._solver(self._linearOperator, arrX, atol=1e-12)[0]
+
+    cpdef np.ndarray _solveBackward(self, np.ndarray arrX):
+        return self._solver(self._linearOperator.H, arrX, atol=1e-12)[0]
+
+    def __repr__(self):
+        return "<%s.(^+)>" %(self._nested.__repr__())
+
+    cpdef np.ndarray _forward(self, np.ndarray arrX):
+        return np.apply_along_axis(
+            self._solveForward, 0, arrX
+        )
+
+    cpdef np.ndarray _backward(self, np.ndarray arrX):
+        return np.apply_along_axis(
+            self._solveBackward, 0, arrX
+        )
+
+    cpdef np.ndarray _reference(self):
+        import numpy.linalg as npl
+        return npl.pinv(self._nested.reference())
```

### Comparing `fastmat-0.2a4/fastmat/Outer.pxd` & `fastmat-0.2rc0/fastmat/Outer.pxd`

 * *Files identical despite different names*

### Comparing `fastmat-0.2a4/fastmat/Outer.pyx` & `fastmat-0.2rc0/fastmat/Outer.pyx`

 * *Files 5% similar despite different names*

```diff
@@ -89,16 +89,17 @@
         ----------
         arrV : :py:class:`numpy.ndarray`
             A 1d vector defining the column factors of the resulting matrix.
 
         arrH : :py:class:`numpy.ndarray`
             A 1d vector defining the row factors of the resulting matrix.
 
-        **options :
-            See :py:meth:`fastmat.Matrix.__init__`.
+        **options : optional
+            Additional keyworded arguments. Supports all optional arguments
+            supported by :py:class:`fastmat.Matrix`.
         '''
 
         # check dimensions
         vecV = _arrSqueezedCopy(vecV)
         vecH = _arrSqueezedCopy(vecH)
 
         if vecV.ndim != 1 or vecH.ndim != 1:
```

### Comparing `fastmat-0.2a4/fastmat/Parametric.pxd` & `fastmat-0.2rc0/fastmat/Parametric.pxd`

 * *Files identical despite different names*

### Comparing `fastmat-0.2a4/fastmat/Parametric.pyx` & `fastmat-0.2rc0/fastmat/Parametric.pyx`

 * *Files 7% similar despite different names*

```diff
@@ -74,19 +74,19 @@
         F = \begin{bmatrix}
         1 &   3 &  8 & 15 \\
         -3 &   0 &  5 & 12 \\
         -8 &  -5 &  0 &  7 \\
         -15 & -12 & -7 &  0
         \end{bmatrix}
 
-    We used Cython [3]_ to get an efficient implementation in order to reduce
-    computation time. Moreover, it is generally assumed the the defined
-    function is able to use row and column broadcasting during evaluation.
-    If this is not the case, one has to set the flag ``rangeAccess`` to
-    ``False``.
+    We used Cython :ref:`[3]<ref3>` to get an efficient implementation in order
+    to reduce computation time. Moreover, it is generally assumed the the
+    defined function is able to use row and column broadcasting during
+    evaluation. If this is not the case, one has to set the flag
+    ``rangeAccess`` to ``False``.
     """
 
     property vecY:
         r"""Return the support vector in Y dimension.
 
         *(read only)*
         """
@@ -124,31 +124,29 @@
 
         vecY : :py:class:`numpy.ndarray`
             A 1d vector mapping the matrix row index to the y-values of funF.
 
         funF : callable with arguments (x, y)
             A function returning the element at index (x, y).
 
-        **options:
-            See the list of special options below and
-            :py:meth:`fastmat.Matrix.__init__` for general options.
-
-        Options
-        -------
-        funDtype : :py:class:`numpy.dtype`
+        funDtype : :py:class:`numpy.dtype`, optional
             Data type of the values returned by funF
 
             Not specified by default (determine the datatype from the element
             at the first index funF(vecX[0], vecY[0]).
 
-        rangeAccess : bool
+        rangeAccess : bool, optional
             Allow passing row- and column vectors directly to funF. This can
             lead to significant speed-ups compared to single-element access.
 
             Defaults to True.
+
+        **options : optional
+            Additional optional keyworded arguments. Supports all optional
+            arguments supported by :py:class:`fastmat.Matrix`.
         '''
 
         # retrieve options
         funDtype = options.get('funDtype', None)
         rangeAccess = options.get('rangeAccess', True)
 
         # store flags
```

### Comparing `fastmat-0.2a4/fastmat/Partial.pxd` & `fastmat-0.2rc0/fastmat/Partial.pxd`

 * *Files identical despite different names*

### Comparing `fastmat-0.2a4/fastmat/Partial.pyx` & `fastmat-0.2rc0/fastmat/Partial.pyx`

 * *Files 5% similar despite different names*

```diff
@@ -101,38 +101,36 @@
         Initialize a Partial matrix instance.
 
         Parameters
         ----------
         mat : :py:class:`fastmat.Matrix`
             A fastmat matrix instance subject to partial access.
 
-        **options:
-            See the list of special options below and
-            :py:meth:`fastmat.Matrix.__init__` for general options.
-
-        Options
-        -------
-        N : :py:class:`numpy.ndarray`
+        rows : :py:class:`numpy.ndarray`, optional
             A 1d vector selecting rows of mat.
 
             If `N` is of type bool it's size must match the height of mat and
             the values of `N` corresponds to taking/dumping the corresponding
             row.
 
             If `N` is of type int it's values correspond to the indices of the
             rows of mat to select. The size of `N` then matches the height of
             the partialed matrix.
 
             Defaults to selecting all rows.
 
-        M : :py:class:`numpy.ndarray`
+        cols : :py:class:`numpy.ndarray`, optional
             A 1d vector selecting columns of mat. The behaviour is identical to
             `N`.
 
             Defaults to selecting all columns.
+
+        **options : optional
+            Additional optional keyworded arguments. Supports all optional
+            arguments supported by :py:class:`fastmat.Matrix`.
         '''
 
         # initialize matrix for full support (used anyway for checking)
         if not isinstance(mat, Matrix):
             raise ValueError("Partial: fastmat Matrix required.")
 
         self._content = (mat, )
@@ -163,14 +161,30 @@
                         "Partial: A %s index exceeds matrix dimensions." %(
                             nameDim, ))
 
                 return vecSelection
             else:
                 return None
 
+        if 'N' in options:
+            import warnings
+            warnings.warn(
+                'N=~ is deprecated in Partial.__init__(). Use rows=~.',
+                FutureWarning
+            )
+            options['rows'] = options['N']
+
+        if 'M' in options:
+            import warnings
+            warnings.warn(
+                'M=~ is deprecated in Partial.__init__() Use cols=~.',
+                FutureWarning
+            )
+            options['cols'] = options['M']
+
         self._rowSelection = checkSelection(
             options.get('rows', None), mat.numRows, 'row'
         )
         self._colSelection = checkSelection(
             options.get('cols', None), mat.numCols, 'col'
         )
```

### Comparing `fastmat-0.2a4/fastmat/Permutation.pxd` & `fastmat-0.2rc0/fastmat/Permutation.pxd`

 * *Files identical despite different names*

### Comparing `fastmat-0.2a4/fastmat/Permutation.pyx` & `fastmat-0.2rc0/fastmat/Permutation.pyx`

 * *Files 5% similar despite different names*

```diff
@@ -64,16 +64,17 @@
 
         Parameters
         ----------
         sigma : :py:class:`numpy.ndarray`
             A 1d vector of type int mapping the row indices to column indices
             uniquely.
 
-        **options:
-            See :py:meth:`fastmat.Matrix.__init__`.
+        **options : optional
+            Additional keyworded arguments. Supports all optional arguments
+            supported by :py:class:`fastmat.Matrix`.
         '''
         numRows = sigma.shape[0]
 
         if not np.allclose(np.sort(sigma), np.arange(numRows)):
             raise ValueError("Not a permutation.")
 
         self._sigma = sigma
```

### Comparing `fastmat-0.2a4/fastmat/Polynomial.pxd` & `fastmat-0.2rc0/fastmat/Polynomial.pxd`

 * *Files identical despite different names*

### Comparing `fastmat-0.2a4/fastmat/Polynomial.pyx` & `fastmat-0.2rc0/fastmat/Polynomial.pyx`

 * *Files 3% similar despite different names*

```diff
@@ -71,16 +71,17 @@
         ----------
         mat : :py:class:`fastmat.Matrix`
             A fastmat matrix instance subject to constructing the polynomial.
 
         coeff : :py:class:`numpy.ndarray`
             A 1d vector defining the polynomial coefficients.
 
-        **options:
-            See :py:meth:`fastmat.Matrix.__init__`.
+        **options : optional
+            Additional keyworded arguments. Supports all optional arguments
+            supported by :py:class:`fastmat.Matrix`.
         '''
 
         if mat.numRows != mat.numCols:
             raise ValueError("Polynomial: Matrix must be square.")
 
         dtype = np.promote_types(mat.dtype, coeff.dtype)
```

### Comparing `fastmat-0.2a4/fastmat/Product.pxd` & `fastmat-0.2rc0/fastmat/Product.pxd`

 * *Files identical despite different names*

### Comparing `fastmat-0.2a4/fastmat/Product.pyx` & `fastmat-0.2rc0/fastmat/Product.pyx`

 * *Files 2% similar despite different names*

```diff
@@ -56,26 +56,24 @@
 
         Parameters
         ----------
         *matrices : :py:class:`fastmat.Matrix` or scalar value
             The matrix instances to form a matrix-matrix product of. You may
             also specify scalar values.
 
-        **options:
-            See the list of special options below and
-            :py:meth:`fastmat.Matrix.__init__` for general options.
-
-        Options
-        -------
-        typeExpansion : bool
+        typeExpansion : bool, optional
             Expand the data type of input data to the data type specified with
             this paramter.
 
             Defaults to a floating-point expansion of the promoted type of all
             nested matrices' (and scalar values') data types.
+
+        **options : optional
+            Additional optional keyworded arguments. Supports all optional
+            arguments supported by :py:class:`fastmat.Matrix`.
         '''
 
         # evaluate options passed to Product
         debug = options.get('debug', False)
 
         # initialize product content to [1]
         lstFactors = []
```

### Comparing `fastmat-0.2a4/fastmat/Sparse.pxd` & `fastmat-0.2rc0/fastmat/Sparse.pxd`

 * *Files identical despite different names*

### Comparing `fastmat-0.2a4/fastmat/Sparse.pyx` & `fastmat-0.2rc0/fastmat/Sparse.pyx`

 * *Files 2% similar despite different names*

```diff
@@ -82,16 +82,16 @@
 
     .. note::
         The ``format`` specifier drastically influences performance during
         multiplication of these matrices. From our experience ``'csr'`` works
         best in these cases.
 
     For this matrix class we used the already tried and tested routines of
-    SciPy [1]_, so we merely provide a convenient wrapper to integrate nicely
-    into ``fastmat``.
+    SciPy :ref:`[1]<ref1>`, so we merely provide a convenient wrapper to
+    integrate nicely into ``fastmat``.
     """
 
     property spArray:
         r"""Return the scipy sparse matrix .
 
         *(read only)*
         """
@@ -115,16 +115,17 @@
         Initialize a Sparse matrix instance.
 
         Parameters
         ----------
         matSparse : :py:class:`scipy.sparse.spmatrix`
             A 2d scipy sparse matrix to be cast as a fastmat matrix.
 
-        **options:
-            See :py:meth:`fastmat.Matrix.__init__`.
+        **options : optional
+            Additional optional keyworded arguments. Supports all optional
+            arguments supported by :py:class:`fastmat.Matrix`.
         '''
         if not isinstance(matSparse, spmatrix):
             raise TypeError("Sparse: Use Matrix() for numpy ndarrays."
                             if isinstance(matSparse, np.ndarray)
                             else "Sparse: Matrix is not a scipy spmatrix")
 
         self._spArray = matSparse.tocsr()
```

### Comparing `fastmat-0.2a4/fastmat/Sum.pxd` & `fastmat-0.2rc0/fastmat/Sum.pxd`

 * *Files identical despite different names*

### Comparing `fastmat-0.2a4/fastmat/Sum.pyx` & `fastmat-0.2rc0/fastmat/Sum.pyx`

 * *Files 2% similar despite different names*

```diff
@@ -57,16 +57,17 @@
         Initialize a Sum matrix instance.
 
         Parameters
         ----------
         *matrices : :py:class:`fastmat.Matrix`
             The matrix instances to be summed.
 
-        **options:
-            See :py:meth:`fastmat.Matrix.__init__`.
+        **options : optional
+            Additional optional keyworded arguments. Supports all optional
+            arguments supported by :py:class:`fastmat.Matrix`.
         '''
         cpdef Matrix mat
 
         # Fold multiple levels of sums
         lstTerms = []
 
         def __addTerms(matrices):
```

### Comparing `fastmat-0.2a4/fastmat/Toeplitz.pxd` & `fastmat-0.2rc0/fastmat/Toeplitz.pxd`

 * *Files identical despite different names*

### Comparing `fastmat-0.2a4/fastmat/Toeplitz.pyx` & `fastmat-0.2rc0/fastmat/Toeplitz.pyx`

 * *Files 5% similar despite different names*

```diff
@@ -24,87 +24,38 @@
 from .Partial cimport Partial
 from .Product cimport Product
 from .Kron cimport Kron
 from .Fourier cimport Fourier
 from .Diag cimport Diag
 
 
-################################################################################
-################################################## class Toeplitz
 cdef class Toeplitz(Partial):
     r"""
-
-    A Toeplitz matrix :math:`T \in \mathbb{C}^{n \times m}` realizes the mapping
-
-    .. math::
-        x \mapsto  T \cdot  x,
-
-    where :math:`x \in C^n` and
-
-    .. math::
-        T = \begin{bmatrix}
-        t_1 & t_{-1} & \dots & t_{-(m-1)} \\
-        t_2 & t_1 & \ddots & t_{-(n-2)} \\
-        \vdots & \vdots & \ddots & \vdots \\
-        t_n & t_{n-1} & \dots & t_1
-        \end{bmatrix}.
-
-    This means that a Toeplitz matrix is uniquely defined by the
-    :math:`n + m - 1` values that are on the diagonals.
-
-    >>> # import the package
-    >>> import fastmat as fm
-    >>> import numpy as np
-    >>>
-    >>> # define the parameters
-    >>> d1 = np.array([1,0,3,6])
-    >>> d2 = np.array([5,7,9])
-    >>>
-    >>> # construct the transform
-    >>> T = fm.Toeplitz(d1,d2)
-
-    This yields
-
-    .. math::
-        d_1 = (1,0,3,6)^\mathrm{T}
-
-    .. math::
-        d_2 = (5,7,9)^\mathrm{T}
-
-    .. math::
-        T = \begin{bmatrix}
-        1 & 5 & 7 & 9 \\
-        0 & 1 & 5 & 7 \\
-        3 & 0 & 1 & 5 \\
-        6 & 3 & 0 & 1
-        \end{bmatrix}
-
-    Since the multiplication with a Toeplitz matrix makes use of the FFT, it
-    can be very slow, if the sum of the dimensions of :math:`d_1` and
-    :math:`d_2` are far away from a power of :math:`2`, :math:`3` or
-    :math:`4`. This can be alleviated if one applies smart zeropadding during
-    the transformation.
-    This can be activated as follows.
-
-    >>> # import the package
-    >>> import fastmat as fm
-    >>> import numpy as np
+    This class provides a very general implementation of Toeplitz matrices,
+    which essentially realize a (possibly multidimensional) non-circular
+    convolution.
+
+    This type of matrix is highly structured. A two-level Toeplitz
+    Matrix looks like:
+
+    >>> t_00 t_05 t_04 t_03   t_40 t_45 t_44 t_43   t_30 t_35 t_34 t_33
+    >>> t_01 t_00 t_05 t_04   t_41 t_40 t_45 t_44   t_31 t_30 t_35 t_34
+    >>> t_02 t_01 t_00 t_05   t_42 t_41 t_40 t_45   t_32 t_31 t_30 t_35
     >>>
-    >>> # define the parameters
-    >>> d1 = np.array([1,0,3,6])
-    >>> d2 = np.array([5,7,9])
+    >>> t_10 t_15 t_14 t_13   t_00 t_05 t_04 t_03   t_40 t_45 t_44 t_43
+    >>> t_11 t_10 t_15 t_14   t_01 t_00 t_05 t_04   t_41 t_40 t_45 t_44
+    >>> t_12 t_11 t_10 t_15   t_02 t_01 t_00 t_05   t_42 t_41 t_40 t_45
     >>>
-    >>> # construct the transform
-    >>> T = fm.Toeplitz(d1,d2,pad='true')
-
-    This yields the same matrix and transformation as above, but it might be
-    faster depending on the dimensions involved in the problem.
-
-    This class depends on ``Fourier``, ``Diag``, ``Product`` and
-    ``Partial``.
+    >>> t_20 t_25 t_24 t_23   t_10 t_15 t_14 t_13   t_00 t_05 t_04 t_03
+    >>> t_21 t_20 t_25 t_24   t_11 t_10 t_15 t_14   t_01 t_00 t_05 t_04
+    >>> t_22 t_21 t_20 t_25   t_12 t_11 t_10 t_15   t_02 t_01 t_00 t_05
+
+    This shows that one can define an L-level Toeplitz matrix by a tensor
+    of order L together with means of deciding the sizes ``n_1,...,n_L`` of
+    the individual levels.
     """
 
     property tenT:
         r"""Return the defining Tensor of Toeplitz matrix."""
 
         def __get__(self):
             return self._tenT
@@ -125,55 +76,55 @@
             warnings.warn('vecR is deprecated.', FutureWarning)
             return self._tenT[self._arrDimCols[0]:]
 
     def __init__(self, *args, **options):
         '''
         Initialize Toeplitz matrix instance.
 
-        Parameter for one-dimensional case
-        ----------------------------------
-        vecC : :py:class:`numpy.ndarray`
-            The generating column vector of the toeplitz matrix describing the
-            first column of the matrix.
-
-        vecR : :py:class:`numpy.ndarray`
-            The generating row vector of the toeplitz matrix excluding the
-            element corresponding to the first column, which is already defined
-            in `vecC`.
-
-        **options:
-            See below.
+        One either has to specify ``(vecC, vecR)`` or ``tenT`` with optinal
+        ``split`` argument.
 
-        Parameter for one-or-multi-dimensional case
-        -------------------------------------------
+        Parameters
+        ----------
         tenT : :py:class:`numpy.ndarray`
-            The generating nd-array defining the toeplitz tensor. The matrix
-            data type is determined by the data type of this array. In this
-            parameter variant the column- and row-defining vectors are given
-            in one single vector. The intersection point between these two
-            vectors is given in the `split` option.
-
-        **options:
-            See below.
-
-        Options
-        -------
-        split : :py:class:`numpy.ndarray`
-            A 1d vector specifying the split-point for row/column definition
-            of each vector. If this option is not specified each level
-            :math:`T \in \mathbb{C}^{d_i \times d_i}` with the corresponding
-            :math:`i` of `tenT` is assumed to have a square shape of size
-            dimension of `tenT` having :math:`d_i * 2 - 1` entries.
-
-            Defaults to a splitpoint vetor corresponding to all-square levels.
-
-
-        Also see the special options of :py:class:`fastmat.Fourier`, which are
-        also supported by this matrix and the general options offered by
-        :py:meth:`fastmat.Matrix.__init__`.
+            This is the most general way to define a (multilevel) Toeplitz
+            Matrix. The number of dimensions (length of .shape) determines
+            the number of levels. If `split` is not defined then tenT needs
+            to have odd size in each dimension, so that this results in a
+            square matrix. The handling of the indexing in direction of columns
+            follows the same reversed fashion as in the one-dimensional case
+            with `vecR`, but here naturally for each level.
+
+        split : :py:class:`numpy.ndarray`, optional
+            This vector needs to have as many elements as the number of elements
+            of `tenT.shape`. If it is specified it defines the number
+            of elements which are used to determine the number of rows of
+            each level. The rest of the elements are indexed in reverse order
+            in the same fashion as without split.
+
+
+        **options : optional
+            Additional keyworded arguments. Supports all optional arguments
+            supported by :py:class:`fastmat.Matrix` and
+            :py:class:`fastmat.Fourier`.
+
+            All optional arguments will be passed on to all
+            :py:class:`fastmat.Matrix` instances that are generated during
+            initialization.
+
+        Note:
+            For backward compatibility reasons it is still possible to
+            substitute the `tenT` argument by two 1D :py:class:`numpy.ndarray`
+            arrays `vecC` and `vecR` that describe the column- and row-defining
+            vectors in the single-level case respectively. The column-defining
+            vector describes the forst column of the resulting matrix and the
+            row-defining vector the first row except the (0,0) element (which
+            is already specified by the column-defining vector). Note that this
+            vector is indexed backwards in the sense that its first element is
+            the last element in the defined Toeplitz matrix.
         '''
 
         # The multidimensional implementation of this class exploits the fact
         # that one can embed a multilevel toeplitz matrix into a multilevel
         # circulant matrix so this initialization takes care of determining the
         # size of the resulting circulant matrix and the pattern how we embed
         # the toeplitz matrix into the circulant one moreover we exploit the
```

### Comparing `fastmat-0.2a4/fastmat/Zero.pxd` & `fastmat-0.2rc0/fastmat/Zero.pxd`

 * *Files identical despite different names*

### Comparing `fastmat-0.2a4/fastmat/Zero.pyx` & `fastmat-0.2rc0/fastmat/Zero.pyx`

 * *Files 5% similar despite different names*

```diff
@@ -51,16 +51,17 @@
         ----------
         numRows : int
             Height (row count) of the desired zero matrix.
 
         numCols : int
             Width (column count) of the desired zero matrix.
 
-        **options:
-            See :py:meth:`fastmat.Matrix.__init__`.
+        **options : optional
+            Additional keyworded arguments. Supports all optional arguments
+            supported by :py:class:`fastmat.Matrix`.
         '''
         # set properties of matrix
         self._initProperties(numRows, numCols, np.int8, **options)
 
     ############################################## class property override
     cpdef np.ndarray _getArray(self):
         return _arrZero(2, self.numRows, self.numCols, self.numpyType)
```

### Comparing `fastmat-0.2a4/fastmat/__init__.py` & `fastmat-0.2rc0/fastmat/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,21 +12,18 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 r"""
-Introduction
-------------
-
 In many fields of engineering linear transforms play a key role during modeling
 and solving real world problems. Often these linear transforms have an inherent
 structure which reduces the degrees of freedom in their parametrization.
-Moreover this structure allows to describe the action of a linear mapping on a
+Moreover, this structure allows to describe the action of a linear mapping on a
 given vector more efficiently than the general one.
 
 This structure can be exploited twofold. First, the storage of these transforms
 in form of matrices, on computers normally an array of numbers in
 :math:`\mathbb{C}` or :math:`\mathbb{R}`, might be unnecessary.
 So for each structure there is a more concise way of representation, which
 leads to a benefit in memory consumption when using these linear transforms.
@@ -46,24 +43,19 @@
 numbers, while the algorithms that make up the internals are highly adapted to
 the specific structure at hand. It provides you with a set of tools to work
 with linear transforms while hiding the algorithmic complexity and exposing the
 benefits in memory and calculation efficiency without too much overhead.
 
 This way you can worry about really urgent matters to you, like research and
 development of algorithms and leave the internals to fastmat.
-
-Types of Matrices
------------------
-
-If you want to find out, what types of structures we provide, have a look at
-the :ref:`classes`. There is a whole zoo of them!
 """
 
 # import fundamental types and classes first, also behavioural flags
 from .Matrix import Matrix, Hermitian, Conjugate, Transpose, flags
+from .Matrix import Inverse, PseudoInverse
 from .Product import Product
 
 # import all fastmat classes
 from .BlockDiag import BlockDiag
 from .Blocks import Blocks
 from .Circulant import Circulant
 from .Diag import Diag
```

### Comparing `fastmat-0.2a4/fastmat/algorithms/Algorithm.pxd` & `fastmat-0.2rc0/fastmat/algorithms/Algorithm.pxd`

 * *Files identical despite different names*

### Comparing `fastmat-0.2a4/fastmat/algorithms/Algorithm.pyx` & `fastmat-0.2rc0/fastmat/algorithms/Algorithm.pyx`

 * *Files 3% similar despite different names*

```diff
@@ -24,21 +24,18 @@
 from ..core.resource import getMemoryFootprint
 
 ################################################################################
 ################################################## class Algorithm
 cdef class Algorithm(object):
     r"""Algorithm Base Class
 
-
-    **Description:**
     The baseclass of all algorithms that operate on Matrices. This abstract
     baseclass introduces general framework concepts such as interfaces for
     parameter specification, algorithm execution, logging and callbacks.
 
-    DEMO:
     >>> algI = fma.ISTA(Fourier(10))
     >>> algI.cbResult = lambda i: print(i.arrResult)
     >>> algI.cbStep = lambda i: print(i.numStep)
     >>> algI.cbTrace = fma.Algorithm.snapshot
     >>> algI.process(np.ones(10) + np.random.randn(10))
     >>> plt.imshow(np.hstack((np.abs(tt.arrX) for tt in algI.trace)))
     >>> plt.show()
@@ -94,15 +91,16 @@
 #                self.__dict__ = {}
 #
 #            self.__dict__[attr] = val
 #            print("bla")
 
     def updateParameters(self, **kwargs):
         r"""
-        Update the parameters of the algorithm instance with **kwargs.
+        Update the parameters of the algorithm instance with the supllied
+        keyworded arguments.
 
         Apply the set of parameters specified in kwargs by iteratively passing
         them to setattr(self, ...). Specifying an parameter which does not have
         a mathing attribute in the algorithm class will cause an AttributeError
         to be raised.
         """
         for key, value in kwargs.items():
```

### Comparing `fastmat-0.2a4/fastmat/algorithms/FISTA.py` & `fastmat-0.2rc0/fastmat/algorithms/FISTA.py`

 * *Files 4% similar despite different names*

```diff
@@ -42,19 +42,19 @@
     >>> import fastmat as fm
     >>> import fastmat.algorithms as fma
     >>> # define the dimensions and the sparsity
     >>> n, k = 512, 3
     >>> # define the sampling positions
     >>> t = np.linspace(0, 20 * np.pi, n)
     >>> # construct the convolution matrix
-    >>> c = np.cos(2 * t)
+    >>> c = np.cos(2 * t) * np.exp(-t ** 2)
     >>> C = fm.Circulant(c)
     >>> # create the ground truth
     >>> x = np.zeros(n)
-    >>> x[npr.choice(range(n), k, replace=0)] = 1
+    >>> x[np.random.choice(range(n), k, replace=0)] = 1
     >>> b = C * x
     >>> # reconstruct it
     >>> fista = fma.FISTA(C, numLambda=0.005, numMaxSteps=100)
     >>> y = fista.process(b)
     >>> # test if they are close in the
     >>> # domain of C
     >>> print(npl.norm(C * y - b))
@@ -125,22 +125,25 @@
         # signals
         #     fmatA         - input system matrix
         #     arrB          - input data vector (measurements)
         #     numLambda     - balancing parameter in optimization problem
         #                     between data fidelity and sparsity
         #     numMaxSteps   - maximum number of steps to run
         #     numL          - step size during the conjugate gradient step
-        if arrB.ndim > 2:
+        if arrB.ndim > 2 or arrB.ndim < 1:
             raise ValueError("Only n x m arrays are supported for FISTA")
 
         if arrB.ndim == 1:
             self.arrB = arrB.reshape((-1, 1))
         else:
             self.arrB = arrB
 
+        if self.numMaxSteps <= 0:
+            raise ValueError("FISTA would like to do at least one step for you")
+
         # calculate the largest singular value to get the right step size
         self.numL = 1.0 / (self.fmatA.largestSingularValue ** 2)
         self.t = 1
 
         self.arrX = np.zeros(
             (self.fmatA.numCols, self.arrB.shape[1]),
             dtype=np.promote_types(np.float32, self.arrB.dtype)
```

### Comparing `fastmat-0.2a4/fastmat/algorithms/ISTA.py` & `fastmat-0.2rc0/fastmat/algorithms/ISTA.py`

 * *Files 4% similar despite different names*

```diff
@@ -43,19 +43,19 @@
     >>> import fastmat as fm
     >>> import fastmat.algorithms as fma
     >>> # define the dimensions and the sparsity
     >>> n, k = 512, 3
     >>> # define the sampling positions
     >>> t = np.linspace(0, 20 * np.pi, n)
     >>> # construct the convolution matrix
-    >>> c = np.cos(2 * t)
+    >>> c = np.cos(2 * t) * np.exp(-t ** 2)
     >>> C = fm.Circulant(c)
     >>> # create the ground truth
     >>> x = np.zeros(n)
-    >>> x[npr.choice(range(n), k, replace=0)] = 1
+    >>> x[np.random.choice(range(n), k, replace=0)] = 1
     >>> b = C * x
     >>> # reconstruct it
     >>> ista = fma.ISTA(C, numLambda=0.005, numMaxSteps=100)
     >>> y = ista.process(b)
     >>> # test if they are close in the
     >>> # domain of C
     >>> print(npl.norm(C * y - b))
@@ -125,22 +125,25 @@
     def _process(self, arrB):
         # fmatA         - input system matrix
         # arrB          - input data vector (measurements)
         # numLambda     - balancing parameter in optimization problem
         #                 between data fidelity and sparsity
         # numMaxSteps   - maximum number of steps to run
         # numL          - step size during the conjugate gradient step
-        if arrB.ndim > 2:
+        if arrB.ndim > 2 or arrB.ndim < 1:
             raise ValueError("Only n x m arrays are supported for ISTA")
 
         if arrB.ndim == 1:
             self.arrB = arrB.reshape((-1, 1))
         else:
             self.arrB = arrB
 
+        if self.numMaxSteps <= 0:
+            raise ValueError("ISTA would like to do at least one step for you")
+
         # calculate the largest singular value to get the right step size
         self.numL = 1.0 / (self.fmatA.largestSingularValue ** 2)
 
         self.arrX = np.zeros(
             (self.fmatA.numCols, self.arrB.shape[1]),
             dtype=np.promote_types(np.float32, self.arrB.dtype)
         )
```

### Comparing `fastmat-0.2a4/fastmat/algorithms/OMP.pxd` & `fastmat-0.2rc0/fastmat/algorithms/OMP.pxd`

 * *Files identical despite different names*

### Comparing `fastmat-0.2a4/fastmat/algorithms/OMP.pyx` & `fastmat-0.2rc0/fastmat/algorithms/OMP.pyx`

 * *Files 2% similar despite different names*

```diff
@@ -55,15 +55,15 @@
     >>> # define the sampling positions
     >>> t = np.linspace(0, 20 * np.pi, n)
     >>> # construct the convolution matrix
     >>> c = np.cos(2 * t)
     >>> C = fm.Circulant(c)
     >>> # create the ground truth
     >>> x = np.zeros(n)
-    >>> x[npr.choice(range(n), k, replace=0)] = 1
+    >>> x[np.random.choice(range(n), k, replace=0)] = 1
     >>> b = C * x
     >>> # reconstruct it
     >>> omp = fma.OMP(C, numMaxSteps=100)
     >>> y = omp.process(b)
     >>> # test if they are close in the
     >>> # domain of C
     >>> print(npl.norm(C * y - b))
@@ -128,22 +128,25 @@
         #     arrDiag         - array that contains column norms of fmatA
         #     numStrideSize   - size of strides during norm calculation
         #     numStrides      - number of whole strides to go through
         #     numPreSteps     - number of entries that do not fit in whole
         #                       strides
         #
 
-        if arrB.ndim > 2:
+        if arrB.ndim > 2 or arrB.ndim < 1:
             raise ValueError("Only n x m arrays are supported for OMP")
 
         if arrB.ndim == 1:
             self.arrB = arrB.reshape((-1, 1))
         else:
             self.arrB = arrB
 
+        if self.numMaxSteps <= 0:
+            raise ValueError("OMP would like to do at least one step for you")
+
         # get the number of vectors to operate on
         self.numN, self.numM, self.numL = \
             self.fmatA.numRows, self.fmatA.numCols, self.arrB.shape[1]
 
         self.fmatC = self.fmatA.colNormalized
 
         # determine return value data type
```

### Comparing `fastmat-0.2a4/fastmat/algorithms/STELA.py` & `fastmat-0.2rc0/fastmat/algorithms/STELA.py`

 * *Files 10% similar despite different names*

```diff
@@ -44,19 +44,19 @@
     >>> import fastmat as fm
     >>> import fastmat.algorithms as fma
     >>> # define the dimensions and the sparsity
     >>> n, k = 512, 3
     >>> # define the sampling positions
     >>> t = np.linspace(0, 20 * np.pi, n)
     >>> # construct the convolution matrix
-    >>> c = np.cos(2 * t)
+    >>> c = np.cos(2 * t) * np.exp(-t ** 2)
     >>> C = fm.Circulant(c)
     >>> # create the ground truth
     >>> x = np.zeros(n)
-    >>> x[npr.choice(range(n), k, replace=0)] = 1
+    >>> x[np.random.choice(range(n), k, replace=0)] = 1
     >>> b = C * x
     >>> # reconstruct it
     >>> stela = fma.STELA(C, numLambda=0.005, numMaxSteps=100)
     >>> y = stela.process(b)
     >>> # test if they are close in the
     >>> # domain of C
     >>> print(npl.norm(C * y - b))
@@ -122,31 +122,35 @@
         # arrM         - positive part of arrX - numAlpha
         # arrX         - vector to be thresholded
         # numAlpha     - thresholding threshold
         arrM = np.maximum(np.abs(arrX) - numAlpha, 0)
         return np.multiply((arrM / (arrM + numAlpha)), arrX)
 
     def _process(self, arrB):
-        if arrB.ndim > 2:
+        if arrB.ndim > 2 or arrB.ndim < 1:
             raise ValueError("Only n x m arrays are supported for STELA")
 
         if arrB.ndim == 1:
             self.arrB = arrB.reshape((-1, 1))
         else:
             self.arrB = arrB
 
-        dtypeType = np.promote_types(np.float32, self.arrB.dtype)
+        if self.numMaxSteps <= 0:
+            raise ValueError(
+                "STELA would like to do at least one step for you"
+            )
+
+        dtypeType = np.promote_types(np.float64, self.arrB.dtype)
 
         # step size
-        self.arrGamma = np.zeros(self.arrB.shape[1])
+        self.arrGamma = np.zeros(self.arrB.shape[1], dtype=dtypeType)
 
         # current state vector
         self.arrX = np.zeros(
-            (self.fmatA.numCols, self.arrB.shape[1]),
-            dtype=dtypeType
+            (self.fmatA.numCols, self.arrB.shape[1]), dtype=dtypeType
         )
 
         # current gradient
         self.arrGrad = np.zeros_like(self.arrX, dtype=dtypeType)
 
         # residual vector
         self.arrRes = (-self.arrB).astype(dtypeType)
@@ -155,103 +159,109 @@
         self.arrBx = np.zeros_like(self.arrX, dtype=dtypeType)
         self.arrABxx = np.zeros_like(self.arrB, dtype=dtypeType)
 
         # backprojection of the residual vector
         self.arrZ = self.fmatA.backward(self.arrRes)
 
         # squared norms of the system matrix
-        self.arrD = (
-            1. / self.fmatA.colNormalized._content[-1]._vecD ** 2
-        ).reshape((-1, 1))
+        self.arrD = (1.0 / self.fmatA._getColNorms() ** 2).reshape((-1, 1))
 
         # vector for the stopping criterion
         self.arrStop = np.ones(self.arrX.shape[1])
 
         # this vector keeps track of the still active measurements, where
         # we did not converge yet
-        self.arrActive = (np.ones(self.arrX.shape[1]) == 1)
+        self.arrActive = np.ones(self.arrX.shape[1]) == 1
 
         # start iterating
         for self.numStep in range(self.numMaxSteps):
 
             # some utility vector (the scaled gradient) (17)
             self.arrGrad = self.arrD * self.arrX - self.arrZ
 
             # calculate the stopping criterion
-            self.arrStop = np.linalg.norm(
-                self.arrZ - np.maximum(
+            arrDiff = np.maximum(
+                np.minimum(self.arrZ.real - self.arrX.real, +self.numLambda),
+                -self.numLambda,
+            )
+            if dtypeType == complex:
+                arrDiff = arrDiff + 1j * np.maximum(
                     np.minimum(
-                        self.arrZ - self.arrX,
-                        +self.numLambda
+                        self.arrZ.imag - self.arrX.imag, +self.numLambda
                     ),
-                    -self.numLambda
-                ),
-                axis=0
+                    -self.numLambda,
+                )
+            self.arrStop = np.linalg.norm(
+                self.arrZ - arrDiff,
+                axis=0,
             )
-
             # now check if we converged for any snapshot
             self.arrActive = self.arrStop > self.numMaxError
 
             # if no snapshot is active anymore, we can stop entirely
-            if (np.sum(self.arrActive) == 0):
+            if np.sum(self.arrActive) == 0:
                 return self.arrX
 
             # update of the intermediate vector (16)
-            self.arrBx[:, self.arrActive] = self.softThreshold(
-                self.arrGrad[:, self.arrActive],
-                self.numLambda
-            ) / self.arrD
+            self.arrBx[:, self.arrActive] = (
+                self.softThreshold(
+                    self.arrGrad[:, self.arrActive], self.numLambda
+                )
+                / self.arrD
+            )
 
             # cache some operations
             self.arrABxx[:, self.arrActive] = self.fmatA.forward(
                 self.arrBx[:, self.arrActive] - self.arrX[:, self.arrActive]
             )
 
             # we can do exact line search in this case (19)
             # axis=0 accounts for the fact, that we might have multiple
             # measurements at hand.
             self.arrGamma[self.arrActive] = np.maximum(
                 np.minimum(
-                    -(np.sum(
-                        np.multiply(
-                            self.arrRes[:, self.arrActive],
-                            self.arrABxx[:, self.arrActive]
-                        ),
-                        axis=0
-                    ) + self.numLambda * (
-                        np.sum(
-                            np.abs(
-                                self.arrBx[:, self.arrActive]
-                            ) - np.abs(
-                                self.arrX[:, self.arrActive]
-                            ),
-                            axis=0
+                    -(
+                        np.real(
+                            np.sum(
+                                np.multiply(
+                                    np.conj(self.arrRes[:, self.arrActive]),
+                                    self.arrABxx[:, self.arrActive],
+                                ),
+                                axis=0,
+                            )
                         )
-                    )) / np.sum(
-                        (self.arrABxx[:, self.arrActive] ** 2),
-                        axis=0
+                        + self.numLambda
+                        * (
+                            np.sum(
+                                np.abs(self.arrBx[:, self.arrActive])
+                                - np.abs(self.arrX[:, self.arrActive]),
+                                axis=0,
+                            )
+                        )
+                    )
+                    / np.sum(
+                        np.abs(self.arrABxx[:, self.arrActive]) ** 2, axis=0
                     ),
-                    1
+                    1,
                 ),
-                0
+                0,
             )
 
             # update step (5)
             self.arrX[:, self.arrActive] += (
-                self.arrBx[:, self.arrActive] -
-                self.arrX[:, self.arrActive]
-            ).dot(
-                np.diag(self.arrGamma[self.arrActive])
-            )
+                self.arrBx[:, self.arrActive] - self.arrX[:, self.arrActive]
+            ).dot(np.diag(self.arrGamma[self.arrActive]))
 
             # residual update (20)
-            self.arrRes[:, self.arrActive] += \
+            self.arrRes[:, self.arrActive] += (
                 self.arrGamma[self.arrActive] * self.arrABxx[:, self.arrActive]
-            self.arrZ[:, self.arrActive] = \
-                self.fmatA.backward(self.arrRes[:, self.arrActive])
+            )
+            self.arrZ[:, self.arrActive] = self.fmatA.backward(
+                self.arrRes[:, self.arrActive]
+            )
 
             self.handleCallback(self.cbStep)
             self.handleCallback(self.cbTrace)
 
         # return the unthresholded values for all non-zero support elements
         # if we did not converge in the given number of steps
         return self.arrX
@@ -263,72 +273,78 @@
         from ..Hadamard import Hadamard
         from ..Matrix import Matrix
 
         def testSTELA(test):
             # prepare vectors
             numCols = test[TEST.NUM_COLS]
             test[TEST.REFERENCE] = test[TEST.ALG_MATRIX].reference()
-            test[TEST.RESULT_REF] = np.hstack([
-                arrSparseTestDist(
-                    (numCols, 1),
-                    dtype=test[TEST.DATATYPE],
-                    density=1. * test['numK'] / numCols
-                ).toarray()
-                for nn in range(test[TEST.DATACOLS])
-            ])
+            test[TEST.RESULT_REF] = np.hstack(
+                [
+                    arrSparseTestDist(
+                        (numCols, 1),
+                        dtype=test[TEST.DATATYPE],
+                        density=1.0 * test["numK"] / numCols,
+                    ).toarray()
+                    for nn in range(test[TEST.DATACOLS])
+                ]
+            )
             test[TEST.RESULT_INPUT] = test[TEST.ALG_MATRIX].array.dot(
                 test[TEST.RESULT_REF]
             )
             test[TEST.RESULT_OUTPUT] = test[TEST.INSTANCE].process(
                 test[TEST.RESULT_INPUT]
             )
 
         return {
             TEST.ALGORITHM: {
-                'order'         : 6,
-                TEST.NUM_ROWS   : (lambda param: 3 * param['order']),
-                TEST.NUM_COLS   : (lambda param: 2 ** param['order']),
-                'numK'          : 'order',
-                'lambda'        : 0.1,
-                'maxSteps'      : 3,
-                TEST.ALG_MATRIX : lambda param:
-                    Product(Matrix(np.random.uniform(
-                        -100, 100, (getattr(param, TEST.NUM_COLS),
-                                    getattr(param, TEST.NUM_COLS))).astype(
-                                        param['typeA'])),
-                            Hadamard(param.order),
-                            typeExpansion=param['typeA']),
-                'typeA'         : TEST.Permutation(TEST.FLOATTYPES),
-
-                TEST.OBJECT     : STELA,
-                TEST.INITARGS   : [TEST.ALG_MATRIX],
-                TEST.INITKWARGS : {
-                    'numLambda'     : 'lambda',
-                    'numMaxSteps'   : 'maxSteps'
+                "order": 6,
+                TEST.NUM_ROWS: (lambda param: 3 * param["order"]),
+                TEST.NUM_COLS: (lambda param: 2 ** param["order"]),
+                "numK": "order",
+                "lambda": 0.1,
+                "maxSteps": 3,
+                TEST.ALG_MATRIX: lambda param: Product(
+                    Matrix(
+                        np.random.uniform(
+                            -100,
+                            100,
+                            (
+                                getattr(param, TEST.NUM_COLS),
+                                getattr(param, TEST.NUM_COLS),
+                            ),
+                        ).astype(param["typeA"])
+                    ),
+                    Hadamard(param.order),
+                    typeExpansion=param["typeA"],
+                ),
+                "typeA": TEST.Permutation(TEST.FLOATTYPES),
+                TEST.OBJECT: STELA,
+                TEST.INITARGS: [TEST.ALG_MATRIX],
+                TEST.INITKWARGS: {
+                    "numLambda": "lambda",
+                    "numMaxSteps": "maxSteps",
                 },
-
-                TEST.DATAALIGN  : TEST.ALIGNMENT.DONTCARE,
+                TEST.DATAALIGN: TEST.ALIGNMENT.DONTCARE,
                 TEST.INIT_VARIANT: TEST.IgnoreFunc(testSTELA),
-
-                'strTypeA'      : (lambda param: TEST.TYPENAME[param['typeA']]),
-                TEST.NAMINGARGS : dynFormat(
+                "strTypeA": (lambda param: TEST.TYPENAME[param["typeA"]]),
+                TEST.NAMINGARGS: dynFormat(
                     "(%dx%d)*Hadamard(%s)[%s]",
                     TEST.NUM_ROWS,
                     TEST.NUM_COLS,
-                    'order',
-                    'strTypeA'
+                    "order",
+                    "strTypeA",
                 ),
-
                 # matrix inversion always expands data type to floating-point
-                TEST.TYPE_PROMOTION: np.float32,
-                TEST.CHECK_PROXIMITY: False
+                TEST.TYPE_PROMOTION: np.float64,
+                TEST.CHECK_PROXIMITY: False,
             },
         }
 
     @staticmethod
     def _getBenchmark():
         return {}
 
     @staticmethod
     def _getDocumentation():
         from ..inspect import DOC
+
         return ""
```

### Comparing `fastmat-0.2a4/fastmat/algorithms/__init__.py` & `fastmat-0.2rc0/fastmat/algorithms/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -12,26 +12,16 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 r"""
-Algorithms
-^^^^^^^^^^
-
 We provide some algorithms, which make use of the speedups provided by fastmat
 to allow easy production use out of the box.
-
- * :py:class:`fastmat.algorithms.Algorithm`
- * :py:class:`fastmat.algorithms.ISTA`
- * :py:class:`fastmat.algorithms.FISTA`
- * :py:class:`fastmat.algorithms.OMP`
- * :py:class:`fastmat.algorithms.STELA`
-
 """
 # algorithms for sparse recovery
 
 from .Algorithm import Algorithm
 from .ISTA import ISTA
 from .OMP import OMP
 from .FISTA import FISTA
```

### Comparing `fastmat-0.2a4/fastmat/core/cmath.pxd` & `fastmat-0.2rc0/fastmat/core/cmath.pxd`

 * *Files 11% similar despite different names*

```diff
@@ -25,19 +25,14 @@
 
 ################################################## math routines
 
 ctypedef enum OP_MODE:
     MODE_MUL
     MODE_DOTROW
 
-cdef np.float64_t _norm(TYPE_ALL *, intsize)
-cdef np.float64_t _normMV(TYPE_ALL[:])
-cdef TYPE_ALL _corrMV(TYPE_ALL[:], TYPE_ALL[:])
-
-
 ################################################## complexity estimation
 cdef int _findFFTFactors(int, int, int, int)
 cpdef intsize _findOptimalFFTSize(intsize, int)
 cpdef float _getFFTComplexity(intsize)
 
 ################################################## Array generation routines
 cpdef np.ndarray _arrZero(int, intsize, intsize, ntype, bint fortranStyle=?)
```

### Comparing `fastmat-0.2a4/fastmat/core/strides.pxd` & `fastmat-0.2rc0/fastmat/core/strides.pxd`

 * *Files identical despite different names*

### Comparing `fastmat-0.2a4/fastmat/core/strides.pyx` & `fastmat-0.2rc0/fastmat/core/strides.pyx`

 * *Files 26% similar despite different names*

```diff
@@ -24,14 +24,31 @@
 
 from .types cimport *
 
 ################################################################################
 ###  Basic stride operations
 ################################################################################
 cdef void strideInit(STRIDE_s *stride, np.ndarray arr, np.uint8_t axis):
+    """Short summary.
+
+    Parameters
+    ----------
+    *stride : STRIDE_s
+        Description of parameter `*stride`.
+    arr : np.ndarray
+        Description of parameter `arr`.
+    axis : np.uint8_t
+        Description of parameter `axis`.
+
+    Returns
+    -------
+    void
+        Description of returned object.
+
+    """
     if axis > 1:
         raise ValueError("Striding operations support 2D-arrays only.")
 
     stride[0].dtype         = getFusedType(arr)
     if stride[0].dtype >= TYPE_INVALID:
         raise ValueError("Striding does not support given array data type.")
 
@@ -40,46 +57,124 @@
     stride[0].strideVector  = arr.strides[axis ^ 1]     # the other axis
     stride[0].numElements   = arr.shape[axis]           # array element count
     stride[0].numVectors    = arr.shape[axis ^ 1]       # vector count
     stride[0].sizeItem      = np.PyArray_ITEMSIZE(arr)  # size of one item
 
 
 cdef void strideCopy(STRIDE_s *strideDst, STRIDE_s *strideSrc):
+    """Short summary.
+
+    Parameters
+    ----------
+    *strideDst : STRIDE_s
+        Description of parameter `*strideDst`.
+    *strideSrc : STRIDE_s
+        Description of parameter `*strideSrc`.
+
+    Returns
+    -------
+    void
+        Description of returned object.
+
+    """
     memcpy(strideDst, strideSrc, sizeof(STRIDE_s))
 
 
 cdef void strideSliceVectors(STRIDE_s *stride,
                              intsize start, intsize stop, intsize step):
+    """Short summary.
+
+    Parameters
+    ----------
+    *stride : STRIDE_s
+        Description of parameter `*stride`.
+    start : intsize
+        Description of parameter `start`.
+    stop : intsize
+        Description of parameter `stop`.
+    step : intsize
+        Description of parameter `step`.
+
+    Returns
+    -------
+    void
+        Description of returned object.
+
+    """
     # CAUTION: NOT VERIFIED YET
     if start < 0:
         start = stride[0].numVectors
 
     if stop < 0:
         stop = stride[0].numVectors
 
     stride[0].base += start * stride[0].strideVector
     stride[0].numVectors = stop if step == 0 else (stop - start) // step
     stride[0].strideVector = stride[0].strideVector * step
 
 cdef void strideSliceElements(STRIDE_s *stride,
                               intsize start, intsize stop, intsize step):
+    """Short summary.
+
+    Parameters
+    ----------
+    *stride : STRIDE_s
+        Description of parameter `*stride`.
+    start : intsize
+        Description of parameter `start`.
+    stop : intsize
+        Description of parameter `stop`.
+    step : intsize
+        Description of parameter `step`.
+
+    Returns
+    -------
+    void
+        Description of returned object.
+
+    """
     if start < 0:
         start = stride[0].numElements
 
     if stop < 0:
         stop = stride[0].numElements
 
     stride[0].base += start * stride[0].strideElement
     stride[0].numElements = stop if step == 0 else (stop - start) // step
     stride[0].strideElement = stride[0].strideElement * step
 
 cdef void strideSubgridVector(STRIDE_s *stride,
                               intsize idxVector, intsize idxElement,
                               intsize steppingElements, intsize numElements,
                               intsize steppingVectors, intsize numVectors):
+    """Short summary.
+
+    Parameters
+    ----------
+    *stride : STRIDE_s
+        Description of parameter `*stride`.
+    idxVector : intsize
+        Description of parameter `idxVector`.
+    idxElement : intsize
+        Description of parameter `idxElement`.
+    steppingElements : intsize
+        Description of parameter `steppingElements`.
+    numElements : intsize
+        Description of parameter `numElements`.
+    steppingVectors : intsize
+        Description of parameter `steppingVectors`.
+    numVectors : intsize
+        Description of parameter `numVectors`.
+
+    Returns
+    -------
+    void
+        Description of returned object.
+
+    """
     # CAUTION: NOT VERIFIED YET
 
     # compute new base pointer (offset subgrid stride from current one)
     stride[0].base += (stride[0].strideElement * idxElement +
                        stride[0].strideVector * idxVector)
 
     # now compute new spans and strides for element and vector axes. Both of
@@ -87,33 +182,93 @@
     # This allows mapping butterfly operation slicing directly to a 2D stride!
     stride[0].strideVector = stride[0].strideElement * steppingVectors
     stride[0].strideElement = stride[0].strideElement * steppingElements
     stride[0].numElements = numElements
     stride[0].numVectors = numVectors
 
 cdef void strideFlipVectors(STRIDE_s *stride):
+    """Short summary.
+
+    Parameters
+    ----------
+    *stride : STRIDE_s
+        Description of parameter `*stride`.
+
+    Returns
+    -------
+    void
+        Description of returned object.
+
+    """
     stride[0].base += (stride[0].numVectors - 1) * stride[0].strideVector
     stride[0].strideVector = -stride[0].strideVector
 
 cdef void strideFlipElements(STRIDE_s *stride):
+    """Short summary.
+
+    Parameters
+    ----------
+    *stride : STRIDE_s
+        Description of parameter `*stride`.
+
+    Returns
+    -------
+    void
+        Description of returned object.
+
+    """
     stride[0].base += (stride[0].numElements - 1) * stride[0].strideElement
     stride[0].strideElement = -stride[0].strideElement
 
 cdef stridePrint(STRIDE_s *stride, text=''):
+    """Short summary.
+
+    Parameters
+    ----------
+    *stride : STRIDE_s
+        Description of parameter `*stride`.
+    text : type
+        Description of parameter `text`.
+
+    Returns
+    -------
+    type
+        Description of returned object.
+
+    """
     print("[%dx%d,%d] @ 0x%012X + %d * nn + %d * mm (%d Bytes) %s" %(
         stride[0].numElements, stride[0].numVectors, stride[0].dtype,
         <intsize> (stride[0].base),
         stride[0].strideElement, stride[0].strideVector, stride[0].sizeItem,
         ": %s" %(text, ) if len(text) > 0 else ""))
 
 ################################################################################
 ###  Operations with strides
 ################################################################################
 cdef opCopyVector(STRIDE_s *strideDst, intsize idxVectorDst,
                   STRIDE_s *strideSrc, intsize idxVectorSrc):
+    """Short summary.
+
+    Parameters
+    ----------
+    *strideDst : STRIDE_s
+        Description of parameter `*strideDst`.
+    idxVectorDst : intsize
+        Description of parameter `idxVectorDst`.
+    *strideSrc : STRIDE_s
+        Description of parameter `*strideSrc`.
+    idxVectorSrc : intsize
+        Description of parameter `idxVectorSrc`.
+
+    Returns
+    -------
+    type
+        Description of returned object.
+
+    """
     # CAUTION: NOT VERIFIED YET
 
     cdef intsize nn
     cdef intsize dstStride = strideDst[0].strideElement
     cdef intsize srcStride = strideSrc[0].strideElement
     cdef intsize numElements = strideDst[0].numElements
     cdef np.uint8_t sizeItem = strideDst[0].sizeItem
@@ -156,14 +311,29 @@
         for nn in range(numElements):
             memcpy(ptrDst, ptrSrc, sizeItem)
             ptrDst += dstStride
             ptrSrc += srcStride
 
 
 cdef opZeroVector(STRIDE_s *stride, intsize idxVector):
+    """Short summary.
+
+    Parameters
+    ----------
+    *stride : STRIDE_s
+        Description of parameter `*stride`.
+    idxVector : intsize
+        Description of parameter `idxVector`.
+
+    Returns
+    -------
+    type
+        Description of returned object.
+
+    """
     # CAUTION: NOT VERIFIED YET
     cdef intsize nn
     cdef char *ptr = stride[0].base + stride[0].strideVector * idxVector
     cdef intsize strideElement = stride[0].strideElement
     cdef intsize numElements = stride[0].numElements
     cdef np.uint8_t sizeItem = stride[0].sizeItem
 
@@ -193,14 +363,27 @@
             ptr += strideElement
     else:
         for nn in range(numElements):
             memset(ptr, 0, sizeItem)
             ptr += strideElement
 
 cdef opZeroVectors(STRIDE_s *stride):
+    """Short summary.
+
+    Parameters
+    ----------
+    *stride : STRIDE_s
+        Description of parameter `*stride`.
+
+    Returns
+    -------
+    type
+        Description of returned object.
+
+    """
     # CAUTION: NOT VERIFIED YET
     cdef intsize nn, mm, sizeChunk
     cdef np.uint8_t sizeItem = stride[0].sizeItem
     cdef intsize numElements = stride[0].numElements
     cdef intsize numVectors = stride[0].numVectors
     cdef intsize strideElement = stride[0].strideElement
     cdef intsize strideVector = stride[0].strideVector
```

### Comparing `fastmat-0.2a4/fastmat/core/types.h` & `fastmat-0.2rc0/fastmat/core/types.h`

 * *Files identical despite different names*

### Comparing `fastmat-0.2a4/fastmat/core/types.pxd` & `fastmat-0.2rc0/fastmat/core/types.pxd`

 * *Files identical despite different names*

### Comparing `fastmat-0.2a4/fastmat/inspect/__init__.py` & `fastmat-0.2rc0/fastmat/inspect/__init__.py`

 * *Files identical despite different names*

### Comparing `fastmat-0.2a4/fastmat/inspect/common.py` & `fastmat-0.2rc0/fastmat/inspect/benchmark.py`

 * *Files 22% similar despite different names*

```diff
@@ -11,832 +11,914 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-import copy
-import inspect
-import itertools
 import os
-import re
-import six
-import struct
 import numpy as np
-from scipy import sparse
-from platform import system as pfSystem
+from timeit import timeit
+import time
 
-from ..core.types import isInteger
-
-try:
-    from itertools import izip
-except ImportError:         # python 3.x
-    izip = zip
-
-currentOS = pfSystem()
+from .common import *
+from ..core.cmath import profileCall
+from ..core.resource import getMemoryFootprint
+from ..Matrix import Matrix
+from scipy.sparse.linalg import bicg
+from ..version import __version__
+
+
+################################################## BENCH CONSTANT-def class
+class BENCH(NAME):
+    """Short summary."""
+    FORWARD         = 'forward'
+    OVERHEAD        = 'overhead'
+    DTYPES          = 'dtypes'
+    PERFORMANCE     = 'performance'
+
+    FUNC_INIT       = 'funcInit'
+    FUNC_GEN        = 'funcConstr'
+    FUNC_SIZE       = 'funcSize'
+    FUNC_STEP       = 'funcStep'
+
+    STEP_START_K    = 'startK'
+    STEP_LOGSTEPS   = 'logSteps'
+    STEP_MINITEMS   = 'minItems'
+
+    LIMIT_MEMORY    = 'maxMem'
+    LIMIT_INIT      = 'maxInit'
+    LIMIT_ITER      = 'maxIter'
+    LIMIT_SIZE      = 'maxSize'
+
+    RESULT_MEMORY   = 'totalMem'
+    RESULT_INIT     = 'initTime'
+    RESULT_ITER     = 'iterTime'
+    RESULT_K        = 'K'
+    RESULT_SIZE     = 'numN'
+    RESULT_OVH_NESTED_F = 'ovhFwd'
+    RESULT_OVH_NESTED_B = 'ovhBwd'
+    RESULT_EFF_NESTED_F = 'effFwd'
+    RESULT_EFF_NESTED_B = 'effBwd'
+    RESULT_COMPLEXITY_F = 'cpxFwd'
+    RESULT_COMPLEXITY_B = 'cpxBwd'
+    RESULT_ESTIMATE_FWD = 'estFwd'
+    RESULT_ESTIMATE_BWD = 'estBwd'
+    RESULT_ITEMS    = '#'
+
+    MEAS_MINTIME    = 'measMinTime'
+    MEAS_MINREPS    = 'measMinReps'
+    MEAS_MINRUNS    = 'measMinRuns'
+    MEAS_COMPACT    = 'compactStats'
 
 
 ################################################################################
-################################################## CONSTANT definition classes
-class ALIGNMENT(object):
-    DONTCARE        = '-'
-    FCONT           = 'F'
-    CCONT           = 'C'
-    STRIDE          = 'S'
+##################################################  benchmark implementations
 
+################################################## weightedPercentile()
+def weightedPercentile(data, **options):
+    """Short summary.
 
-################################################################################
-################################################## Permutation funcs and classes
+    Parameters
+    ----------
+    data : type
+        Description of parameter `data`.
+    **options : type
+        Description of parameter `**options`.
+
+    Returns
+    -------
+    type
+        Description of returned object.
+
+    """
+    # """
+    # O(nlgn) implementation for weighted_percentile, with linear interpolation
+    # #between weights.
+    #
+    # date:       Aug 25 '16 @ 13:37
+    # user:       nayyrv [Aug 16 '15 @ 10:52]
+    # source:     www.stackoverflow.com/questions/
+    #                 21844024/weighted-percentile-using-numpy
+    # ``  This is my function, it give identical behaviour to `np.percentile(
+    #     np.repeat(data, weights), percentile)` With less memory overhead,
+    #     np.percentile is an O(n) implementation so it's potentially faster for
+    #     small weights. It has all the edge cases sorted out - it's an exace
+    #     solution. The interpolation answers above assume linear, when it's a
+    #     step for most of he case, except when the weight is 1.
+    #
+    #     Say we have data [1,2,3] with weights [3, 11, 7] and I want the
+    #     25% percentile. My ecdf is going to be [3, 10, 21] and I'm looking for
+    #     the 5th value. The interpolation will see [3, 1] and [10, 2] as the
+    #     matches and interpolate gving 1.28 despite being entirely in the
+    #     2nd bin with a value of 2.
+    # ``
+    #
+    # """
+    # extract options
+    percentile = np.array(options.get('percentile', [75, 25])) / 100.
+    weights = options.get('weights', None)
+
+    if weights is None:
+        weights=np.ones(data.shape)
+
+    dataIndSort=np.argsort(data)
+    dataSort=data[dataIndSort]
+    weights_sort=weights[dataIndSort]
+    ecdf=np.cumsum(weights_sort)
+    percentilePos=percentile * (weights.sum() - 1) + 1
+
+    # need the 1 offset at the end due to ecdf not starting at 0
+    locations=np.searchsorted(ecdf, percentilePos)
+    outPercentiles=np.zeros(percentilePos.shape)
+
+    for i, empiricalLocation in enumerate(locations):
+        # iterate across the requested outPercentiles
+        if ecdf[empiricalLocation - 1] == np.floor(percentilePos[i]):
+            # i.e. is the percentile in between two separate values
+            uppWeight=percentilePos[i] - ecdf[empiricalLocation - 1]
+            lowWeight=1 - uppWeight
 
-class AccessDict(dict):
-    def __getattr__(self, key):
-        if key in self:
-            return self[key]
+            outPercentiles[i]=lowWeight * dataSort[empiricalLocation - 1] + \
+                uppWeight * dataSort[empiricalLocation]
         else:
-            found = [kk for kk in sorted(self.keys())
-                     if kk.startswith(key)]
-            return ([self[kk] for kk in found] if len(found) > 2
-                    else (None if len(found) == 0
-                          else self[found[0]]))
-
-    def __repr__(self):
-        return str(self.keys())
-
-
-def convertToAccessDicts(level):
-    for key, value in level.items():
-        if isinstance(value, dict) and (value is not value):
-            level[key] = convertToAccessDicts(value)
-
-    return AccessDict(level)
-
-
-################################################## class uniqueNameDict
-class uniqueNameDict(dict):
-    '''
-    Modified dictionary: suffixes key names with integer to maintain uniqueness.
-    '''
-
-    def __setitem__(self, key, value):
-        index = 1
-        strKey = key
-        while True:
-            if strKey not in self:
-                break
-            index += 1
-            strKey = "%s_%03d" %(key, index)
-
-        dict.__setitem__(self, strKey, value)
-
-
-################################################## class paramDict
-reFormatString = re.compile(r'%\(.+\)')
-
-
-class paramDict(dict):
-
-    def __getattr__(self, key):
-        # evaluate nested format-string parameters, update format results
-        value, lastValue = super(paramDict, self).__getitem__(key), None
-
-        while id(lastValue) != id(value):
-            lastValue = value
-            if isinstance(value, str):
-                if value in self and value != key:
-                    value = getattr(self, value)
-                elif reFormatString.search(value):
-                    value = value %self
-
-            elif (inspect.isroutine(value) and
-                  not isinstance(value, IgnoreFunc)):
-                value = value(self)
-                self[key] = value
-
-        return value
-
+            # i.e. the percentile is entirely in one bin
+            outPercentiles[i]=dataSort[empiricalLocation]
 
-################################################## class Permutation
-class Permutation(list):
+    return outPercentiles
 
-    def __repr__(self):
-        return "%s(%s)" % (self.__class__.__name__,
-                           super(Permutation, self).__repr__())
 
-    def __str__(self):
-        return "%s(%s)" % (self.__class__.__name__,
-                           super(Permutation, self).__str__())
-
-
-################################################## class VariantPermutation
-class VariantPermutation(Permutation):
-    pass
-
-
-################################################## class IgnoreDict
-class IgnoreDict(dict):
-    pass
-
-
-################################################## class IgnoreFunc
-class IgnoreFunc(object):
-
-    def __init__(self, fun):
-        self._fun = fun
-
-    def __call__(self, *args, **kwargs):
-        return self._fun(*args, **kwargs)
-
-
-################################################## paramApplyDefaults()
-def paramApplyDefaults(
-    params,
-    templates=None,
-    templateKey=None,
-    extraArgs=None
+################################################## timingStats()
+def timingStats(
+    stats,
+    compactStats=False
 ):
+    """Short summary.
 
-    # have some defaults from templates
-    # first, fetch the template as defaults, then update with target,
-    # then assign the whole dict to target
-    result = {}
-    if templates is not None:
-        # 1. COMMON - section of templates (lowest-priority)
-        result.update(templates.get(NAME.COMMON, {}))
-        # 2. the templates-section corresponding to the templateKey
-        result.update(templates.get(templateKey, {}))
-        # 3. specific reference to a template by the 'template' key in params
-        if NAME.TEMPLATE in params:
-            result.update(templates.get(params[NAME.TEMPLATE], {}))
-
-    # 4. actual parameters (params)
-    result.update(params)
-
-    # 5. extraArgs (which usually come from command-line) (top-priority)
-    if extraArgs is not None:
-        for p in extraArgs:
-            for pp in list(p.split(',')):
-                tokens = pp.split('=')
-                if len(tokens) >= 2:
-                    string = "=".join(tokens[1:])
-                    try:
-                        val = int(string)
-                    except ValueError:
-                        try:
-                            val = float(string)
-                        except ValueError:
-                            val = string
-                    result[tokens[0]] = val
-
-    return paramDict(result)
+    Parameters
+    ----------
+    stats : type
+        Description of parameter `stats`.
+    compactStats : type
+        Description of parameter `compactStats`.
 
+    Returns
+    -------
+    type
+        Description of returned object.
 
-################################################## paramPermute()
-def paramPermute(dictionary, copy=True, PermutationClass=Permutation):
-    '''
-    Return a list of cartesian-product combination of all dictionary values
-    holding a Permutation list object. If copy is True, the resulting list will
-    be applied back to input dictionary copies before returning, resulting in
-    a list of copies with the permutation replacements being made on the input
-    dictionary. Parameter permutations must be indicated by wrapping a list in
-    a Permutation class instance.
+    """
     '''
-    # isolate the permutation parameters from the dictionary
-    parameters = {key: list(value)
-                  for key, value in dictionary.items()
-                  if isinstance(value, PermutationClass)}
-
-    # perform a cartesian product -> list of permuted instances
-    permutations = [dict(izip(parameters, x))
-                    for x in itertools.product(*six.itervalues(parameters))]
-    if len(permutations) == 1:
-        permutations = [{}]
-
-    # apply the permutations to the input dictionary (generating copies)
-    def dictCopyAndMerge(source, merge):
-        result = source.copy()
-        result.update(merge)
-        return paramDict(result)
-    return [dictCopyAndMerge(dictionary, permutation)
-            for permutation in permutations] if copy else permutations
-
+    Return the runtime statistics of the given list of measurements.
+    Each measurement is stored as such a tuple:
+    (averageRuntime, totalRuntime, numberRepetitions)
 
-################################################## paramDereferentiate()
-def paramDereferentiate(currentLevel, paramDict=None):
+    A dictionary with clearly named statistical properties is returned.
     '''
-    Replace all text value identifyers matching a target key name with the
-    key values it's pointing to allowing parameter links. Then, recurse through
-    an arbitrary depth of container types (dicts, lists, tuples) found in the
-    first stage, continuing dereferentiation.
-    Returns the modified currentLevel container.
-    '''
-    # set paramDict in first level, determine iterator for currentLevel
-    iterator = currentLevel.items() \
-        if isinstance(currentLevel, dict) else enumerate(currentLevel)
-    if paramDict is None:
-        paramDict = currentLevel
-
-    # STAGE 1: Replace all dictionary values matching a key name in paramDict
-    #          with the corresponding value of that paramDict-entry. Also build
-    #          a container list for stage two.
-    dictIterables = {}
-    for key, value in iterator:
-        if isinstance(value, (list, tuple, dict)):
-            dictIterables[key] = value
-        else:
-            if not isinstance(value, str):
-                continue
-            try:
-                paramValue = paramDict.get(value, None)
-                if (paramValue is not None and
-                        not isinstance(paramValue, Permutation)):
-                    currentLevel[key] = paramValue
-                    if isinstance(paramValue, (list, tuple, dict)):
-                        dictIterables[key] = paramValue
-            except TypeError:
-                continue
 
-    # STAGE 2: Crawl the containers found in stage 1, repeating the process.
-    #          Note that nested containers are copied in the process.
-    #          The parameter dictionary paramDict stays the same for all levels.
-    for key, iterable in dictIterables.items():
-        # copy the container to allow modification of values
-        newIterable = copy.copy(iterable)
-        if isinstance(iterable, tuple):
-            # cast the immutable tuple type to list allowing modifications, cast
-            # back to tuple afterwards
-            newIterable = list(newIterable)
-            paramDereferentiate(newIterable, paramDict)
-            newIterable = tuple(newIterable)
-        else:
-            paramDereferentiate(newIterable, paramDict)
-        # overwrite former iterable with new copy
-        currentLevel[key] = newIterable
+    # accumulate all individual stats
+    times=np.array([stat['avg'] for stat in stats], dtype=np.double)
+    weights=np.array([stat['cnt'] for stat in stats], dtype=np.double)
 
-    return currentLevel
+    # calculate som stats
+    reps=np.sum(weights)
+    avg=np.average(times, weights=weights)
+    minimum=np.min(times)
 
+    # prepare output
+    result={'min': minimum}
 
-################################################## paramEvaluate()
-def paramEvaluate(currentLevel, paramDict=None):
-    '''
-    Evaluate all functions found in currentLevel with paramDict as argument.
-    Repeat the process for nested containers.
-    Returns the modified currentLevel container.
-    '''
-    # set paramDict in first level, determine iterator for currentLevel
-    iterator = currentLevel.items() \
-        if isinstance(currentLevel, dict) else enumerate(currentLevel)
-    if paramDict is None:
-        paramDict = currentLevel
-
-    # STAGE 1: Evaluate the functions found in currentLevel. Also build a
-    #          container list for stage two.
-    dictIterables = {}
-    for key, value in iterator:
-        if isinstance(value, (list, tuple, dict)):
-            if not isinstance(value, IgnoreDict):
-                dictIterables[key] = value
-        elif inspect.isroutine(value):
-            currentLevel[key] = value(paramDict)
-
-    # STAGE 2: Crawl the containers found in stage 1, repeating the process
-    #          The parameter dictionary paramDict stays the same for all levels.
-    for key, iterable in dictIterables.items():
-        if isinstance(iterable, tuple):
-            # cast the immutable tuple type to list allowing modifications, cast
-            # back to tuple afterwards
-            newIterable = list(currentLevel[key])
-            paramEvaluate(newIterable, paramDict)
-            currentLevel[key] = tuple(newIterable)
-        else:
-            paramEvaluate(currentLevel[key], paramDict)
+    # if compactStats is True, skip further stats
+    if compactStats:
+        return result
 
-    return currentLevel
+    # calculate weighted variance
+    var=sum(weights * ((times - avg) ** 2)) / (reps * (1 - 1 / len(stats)))
 
+    # calculate quartiles
+    percs=[25, 75]
+    wp=weightedPercentile(times, percentile=percs, weights=weights)
 
-################################################## mergeDicts()
-# a little helper to safely merge two dictionaries
-def mergeDicts(a, b):
-    '''
-    Merge the dictionaries a and b such that entries in b have priority and the
-    input Dictionary a remains unchanged.
-    '''
-    c = a.copy()
-    c.update(b)
-    return c
+    result.update({'var': var, 'cnt': reps, 'min': minimum})
+    result.update({"p%d" %(percs[i]): wp[i] for i in range(len(percs))})
 
-################################################################################
-################################################## array generators, test distr.
+    return result
 
 
-################################################## arrTestDist()
-def arrTestDist(shape, dtype, center=0):
-    def _draw(shape):
-        '''
-        Draw a random floating-point number from a test distribution.
-        Remove the part around zero from the distribution and keep the distance
-        between minimal and maximal absolute values (dynamics) relatively small
-        '''
-        return (np.random.uniform(2., 1., size=shape) *
-                np.random.choice([-1, 1], shape))
+################################################## timeCall()
+def timeCall(call, *args, **options):
+    """Short summary.
 
-    if np.prod(shape) < 1:
-        return np.array([])
+    Parameters
+    ----------
+    call : type
+        Description of parameter `call`.
+    *args : type
+        Description of parameter `*args`.
+    **options : type
+        Description of parameter `**options`.
+
+    Returns
+    -------
+    type
+        Description of returned object.
+
+    """
+    '''
+    Return runtime statistics for execution of a parameterizable method call
+    specified by call(*args).
+
+    Behaviour of the measurements can be adjusted with these options:
+    minMeasTime       - minimum total time the evaluation shall take
+    minRepetitions    - minimum number of calls needed for evaluation
+    minRuns           - minimum number of single measurements (of one or more
+                      repetitions each) required
+    '''
+    stats=[]
+
+    # begin with one repetition and approach accumulated runtime (step[1])
+    num=1
+    step={'avg': 0., 'time': 0., 'cnt': num}
+    while step['time'] < (options[BENCH.MEAS_MINTIME] * num) / (num + 1) * 0.9:
+        step=profileCall(num, call, *args)
+        num=num * 2 if step['time'] < 1e-6 \
+            else max(1, int(options[BENCH.MEAS_MINTIME] / step['avg']))
+
+    # store as first run with [num] reps
+    stats.append(step)
+
+    # perform repeated measurement to reach at least MIN_ITERATIONS
+    runs=max(int(np.ceil((options[BENCH.MEAS_MINREPS] - num) / num)),
+             options[BENCH.MEAS_MINRUNS] - 1)
+    if runs > 0:
+        stats.extend([profileCall(num, call, *args) for ii in range(0, runs)])
+
+    return timingStats(stats, options[BENCH.MEAS_COMPACT])
+
+
+################################################## timeCalls()
+def timeCalls(calls, **options):
+    """Short summary.
 
-    if dtype in (np.int8, np.uint8, np.int16, np.uint16,
-                 np.int32, np.uint32, np.int64, np.uint64):
-        result = np.random.choice(
-            [center - 2, center - 1, center + 1, center + 2], shape).astype(
-                dtype)
-    else:
-        if dtype in (np.float32, np.float64):
-            result = _draw(shape).astype(dtype) + center
-        elif dtype in (np.complex64, np.complex128):
-            result = (_draw(shape) + np.real(center) +
-                      1j * (_draw(shape) + np.imag(center))).astype(dtype)
-        else:
-            raise TypeError("arrTestDist: unsupported type %s" % (dtype))
+    Parameters
+    ----------
+    calls : type
+        Description of parameter `calls`.
+    **options : type
+        Description of parameter `**options`.
+
+    Returns
+    -------
+    type
+        Description of returned object.
+
+    """
+    '''
+    wrapper for running test runtime measurements for a number of calls
+
+        target      - targeted resolution of measurement
+        calls       - list of dics describing each call with these entries:
+            > 'func'   (method pointer)
+            > 'args'   (*list of arguments)
+            > 'kwargs' (**dictionary of keyword-args)
+        options     - dictionary with parameters for measurements
+
+    A dictionary containing the measurement results of each call, preceded with
+    its call tag is returned. All returned keys will be in `camelCase`.
+    '''
+    return {'%s%s' % (tag, key.title()): value
+            for tag, call in calls.items()
+            for key, value in (
+                timeCall(call['func'], *(call['args']), **options)).items()}
 
-    # increase the largest element in magnitude a little bit more to avoid
-    # too close neighbours to the largest element in the distribution
-    # this helps at least largestSingularValue in Diag matrices to converge ;)
-    idxMax = np.unravel_index(np.abs(result).argmax(), result.shape)
-    if isInteger(dtype):
-        result[idxMax] += np.sign(result[idxMax])
-    else:
-        result[idxMax] *= 1.5
 
-    return result
+################################################################################
+##################################################  TESTS: specification
 
-################################################## arrSparseTestDist()
+################################################## testInitSolve()
+def testInitSolve(funcConstr, numSize, numN):
+    """Short summary.
 
+    Parameters
+    ----------
+    funcConstr : type
+        Description of parameter `funcConstr`.
+    numSize : type
+        Description of parameter `numSize`.
+    numN : type
+        Description of parameter `numN`.
+
+    Returns
+    -------
+    type
+        Description of returned object.
+
+    """
+
+    instance = funcConstr(numSize)
+    mem1 = instance.nbytes
+
+    func1 = lambda A, b: bicg(A, b)[0]
+    args1 = [
+        instance.scipyLinearOperator,
+        arrTestDist((numN, 1), instance.dtype)
+    ]
+    func2 = np.linalg.solve
+    args2 = [
+        instance._forwardReference(np.eye(numN)),
+        args1[1]
+    ]
+
+    if instance._forwardReferenceMatrix is None:
+        instance._forwardReferenceInit()
+
+    mem2 = instance.nbytesReference
+
+    return {
+        'fastmat': {
+            'func': func1,
+            'args': args1,
+            'Mem': mem1
+        },  'numpy': {
+            'func': func2,
+            'args': args2,
+            'Mem': mem2
+        }
+    }
+
+
+################################################## testInitForward()
+def testInitForward(funcConstr, numSize, numN):
+    """Short summary.
 
-def arrSparseTestDist(shape, dtype,
-                      density=0.1, center=0, compactFullyOccupied=False):
-    numSize = np.prod(shape)
-    if compactFullyOccupied:
-        # draw just enough samples randomly such that every row and column is
-        # occupied with at least one element. Ignore the density parameter
-        numElements = max(shape)
-
-        # draw mm and nn coordinates from coordinate space. Modulo operation
-        # wraps indices larger than the actual row or column dimension
-        suppX = np.mod(
-            np.random.choice(numElements, numElements, replace=False), shape[0])
-        suppY = np.mod(
-            np.random.choice(numElements, numElements, replace=False), shape[1])
-    else:
-        # draw a relative amount of samples randomly over vectorized index space
-        numElements = int(numSize * density)
-        supp = np.random.choice(np.arange(numSize), numElements, replace=False)
-        suppX = np.mod(supp, shape[0])
-        suppY = np.divide(supp, shape[0])
-
-    # determine the actual element values distributed over the sparse array
-    # from arrTestDist with a 1D-array spanning the required element count
-    arrElements = arrTestDist((numElements, ), dtype, center=center)
-
-    return sparse.coo_matrix(
-        (arrElements, (suppX, suppY)), shape=shape, dtype=dtype)
-
-
-################################################## arrAlign()
-def arrAlign(arr, alignment=ALIGNMENT.DONTCARE):
-    if alignment == ALIGNMENT.DONTCARE:
-        return np.asanyarray(arr)
-    elif alignment == ALIGNMENT.FCONT:
-        return np.asfortranarray(arr)
-    elif alignment == ALIGNMENT.CCONT:
-        return np.ascontiguousarray(arr)
-    elif alignment == ALIGNMENT.STRIDE:
-        # define spacing between elements
-        spacing = 3
-        # determine maximum value
-        try:
-            maxValue = np.iinfo(arr.dtype).max
-        except ValueError:
-            try:
-                maxValue = np.finfo(arr.dtype).max
-            except ValueError:
-                maxValue = 1.
-
-        # generate large random array with maximized data type utilization
-        arrFill = (maxValue * (np.random.rand(
-            *(dim * spacing for dim in arr.shape)) - 0.5)).astype(arr.dtype)
-
-        # fill-in the array data and return a view of the to-be-aligned array
-        arrPart = arrFill[(np.s_[1::spacing], ) * arrFill.ndim]
-        arrPart[:] = arr
-        return arrPart
-    else:
-        raise ValueError("Unknown alignment identificator '%s'" %(alignment))
+    Parameters
+    ----------
+    funcConstr : type
+        Description of parameter `funcConstr`.
+    numSize : type
+        Description of parameter `numSize`.
+    numN : type
+        Description of parameter `numN`.
+
+    Returns
+    -------
+    type
+        Description of returned object.
+
+    """
+    instance = funcConstr(numSize)
+    mem1 = instance.nbytes
+
+    func1 = instance.forward
+    func2 = instance._forwardReference
+
+    args = [arrTestDist((numN, 1), instance.dtype)]
+    mem2 = instance.nbytesReference
+
+    return {
+        'fastmat': {
+            'func': func1,
+            'args': args,
+            'Mem': mem1
+        }, 'fm10': {
+            'func': func1,
+            'args': [np.resize(args[0], (numN, 10))]
+        }, 'fm100': {
+            'func': func1,
+            'args': [np.resize(args[0], (numN, 100))]
+        }, 'numpy': {
+            'func': func2,
+            'args': args,
+            'Mem': mem2
+        }, 'np10': {
+            'func': func2,
+            'args': [np.resize(args[0], (numN, 10))]
+        }
+    }
+
+
+################################################## testInitOverhead()
+def testInitOverhead(funcConstr, numSize, numN):
+    """Short summary.
 
+    Parameters
+    ----------
+    funcConstr : type
+        Description of parameter `funcConstr`.
+    numSize : type
+        Description of parameter `numSize`.
+    numN : type
+        Description of parameter `numN`.
+
+    Returns
+    -------
+    type
+        Description of returned object.
+
+    """
+    instance = funcConstr(numSize)
+    mem = instance.nbytes
+
+    funcF = instance.forward
+    funcB = instance.backward
+
+    M = 1
+
+    args = [arrTestDist((numN, M), instance.dtype)]
+
+    profFwd, profBwd = instance.profileForward, instance.profileBackward
+    estFwd, estBwd = instance.estimateRuntime(M)
+
+    return {
+        'forward': {
+            'func': funcF,
+            'args': args,
+            'Mem': mem,
+            BENCH.RESULT_OVH_NESTED_F   : profFwd.timeNestedCallOverhead,
+            BENCH.RESULT_EFF_NESTED_F   : profFwd.timeNestedPerUnit,
+            BENCH.RESULT_COMPLEXITY_F   : profFwd.complexityAlg,
+            BENCH.RESULT_ESTIMATE_FWD   : estFwd
+        }, 'backward': {
+            'func': funcB,
+            'args': args,
+            'Mem': mem,
+            BENCH.RESULT_OVH_NESTED_B   : profBwd.timeNestedCallOverhead,
+            BENCH.RESULT_EFF_NESTED_B   : profBwd.timeNestedPerUnit,
+            BENCH.RESULT_COMPLEXITY_B   : profBwd.complexityAlg,
+            BENCH.RESULT_ESTIMATE_BWD   : estBwd
+        }
+    }
+
+
+################################################## testInitDtype()
+def testInitDtype(funcConstr, numSize, numN):
+    """Short summary.
 
-################################################## arrayGenerator
-class ArrayGenerator(dict):
+    Parameters
+    ----------
+    funcConstr : type
+        Description of parameter `funcConstr`.
+    numSize : type
+        Description of parameter `numSize`.
+    numN : type
+        Description of parameter `numN`.
+
+    Returns
+    -------
+    type
+        Description of returned object.
+
+    """
+    def generate(dtype):
+        instance=funcConstr(numSize, dtype)
+
+        # if no instance was created, tag this target as non-existant
+        if instance is None:
+            return None
+
+        # either a Matrix instance or a call tuple structure is returned
+        if isinstance(instance, Matrix):
+            return {
+                'func': instance.forward,
+                'args': [arrTestDist((numN, 1), dtype)],
+                'Mem': instance.nbytes
+            }
+        else:
+            return {
+                'func': instance[0],
+                'args': instance[1],
+                'Mem': instance[1][0].nbytes
+            }
+
+    # create instances for all datatypes listed
+    result={name: generate(dtype)
+            for dtype, name in NAME.TYPENAME.items() if dtype is not None}
 
-    @property
-    def forwardData(self):
-        if NAME.FWDATA not in self:
-            # generate random array and set specific alignment style
-            self[NAME.FWDATA] = arrAlign(
-                arrTestDist(self[NAME.SHAPE], self[NAME.DTYPE],
-                            center=self.get(NAME.CENTER, 0)),
-                alignment=self.get(NAME.ALIGN, ALIGNMENT.DONTCARE))
+    # prune None entries
+    result={key: val for key, val in result.items() if (val is not None)}
+    return result
 
-        return self[NAME.FWDATA]
 
-    @property
-    def backwardData(self):
-        if NAME.BWDATA not in self:
-            # generate random array and set specific alignment style
-            self[NAME.BWDATA] = arrAlign(
-                arrTestDist(self[NAME.SHAPE_T], self[NAME.DTYPE],
-                            center=self.get(NAME.CENTER, 0)),
-                alignment=self.get(NAME.ALIGN, ALIGNMENT.DONTCARE))
-
-        return self[NAME.BWDATA]
-
-    def __call__(self):
-        return self.forwardData
-
-    def __str__(self):
-        '''Compose a compact description of the represented array.'''
-        tags = []
-
-        # generate shape-token: check for both shape variants (fw and bw).
-        # if they differ, print both as "fw/bw", otherwise print the dim only
-        fwShape = self[NAME.SHAPE] if NAME.SHAPE in self else ()
-        bwShape = self[NAME.SHAPE_T] if NAME.SHAPE_T in self else ()
-
-        def printDim(fw, bw):
-            if fw is None:
-                return '-' if bw is None else str(bw)
-            else:
-                return (str(fw) if bw is None
-                        else "%s/%s" %(fw, bw) if (fw != bw) else str(fw))
-
-        strShape = 'x'.join([
-            printDim(fw, bw)
-            for fw, bw in six.moves.zip_longest(fwShape, bwShape)])
-        if len(strShape) > 0:
-            tags.append(strShape)
-
-        # print the data type of the array
-        value = self.get(NAME.DTYPE, '')
-        if isinstance(value, type):
-            tags.append(NAME.TYPENAME.get(value, str(value)))
-
-        value = self.get(NAME.ALIGN, None)
-        if value in NAME.ALLALIGNMENTS:
-            tags.append(value)
+################################################## testInitPerformance()
+def testInitPerformance(funcConstr, numSize, numN):
+    """Short summary.
 
-        return str("[%s]" % (','.join(tags)))
+    Parameters
+    ----------
+    funcConstr : type
+        Description of parameter `funcConstr`.
+    numSize : type
+        Description of parameter `numSize`.
+    numN : type
+        Description of parameter `numN`.
+
+    Returns
+    -------
+    type
+        Description of returned object.
+
+    """
+    func, args=funcConstr(numSize)
+    mem=args[0].nbytes
+
+    return {
+        'perf': {
+            'func': func,
+            'args': args,
+            'Mem': mem
+        }, 'perf10': {
+            'func': func,
+            'args': [args[0], np.resize(args[1],
+                                        (args[1].shape[0], 10))] + args[2:]
+        }
+    }
 
-    def __repr__(self):
-        return self.__str__()
 
 ################################################################################
-################################################## inspection routines
-
-
-def showContent(instance, seen=None, prefix=""):
-    '''
-    Print a readable dependency tree of fastmat class instances
+################################################## class BenchmarkRunner
+class Benchmark(Worker):
+    """Short summary.
 
     Parameters
     ----------
-    instance : :py:class:`fastmat.Matrix`
-        Matrix instance to get inspected
+    targetClass : type
+        Description of parameter `targetClass`.
+    **options : type
+        Description of parameter `**options`.
 
-    Notes
-    -----
-    The function outputs instance as top-level node and then walks through all
-    elements of instance.content, recursively calling itself with extended
-    prefix. To avoid endless loops, the function ensures the recursion is only
-    applied once to every element by keeping track already visited elements.
-
-    >>> showContent(Eye(4) * -1 * -1 + Eye(4) - Eye(4))
-    <Sum[4x4]:0x7fe447f40770>
-    +-<Product[4x4]:0x7fe447f3d188>
-    | +-<Eye[4x4]:0x7fe447f402b0>
-    +-<Eye[4x4]:0x7fe447f403e0>
-    +-<Product[4x4]:0x7fe447f3da10>
-      +-<Eye[4x4]:0x7fe447f40640>
-    '''
-    if seen is None:
-        seen = set([])
+    """
 
-    print((prefix[:-2] + "+-" if len(prefix) > 0 else "") + repr(instance))
-    if instance not in seen:
-        seen.add(instance)
-        last = len(instance)
-        for ii, item in enumerate(instance):
-            showContent(item, seen=seen,
-                        prefix=prefix + ("| " if ii < last - 1 else "  "))
+    def __init__(self, targetClass, **options):
 
-################################################################################
-################################################## CONSTANT definitions
+        # extract options
+        extraOptions = options.get('extraOptions', {})
 
+        # by default, enable verbosity for issues and isolate problems
+        self.cbStatus=self.printStatus
 
-################################################## class TypeDict
-class TypeDict(dict):
-    def __getitem__(self, key):
-        if key not in self:
-            key = key.type if isinstance(key, np.dtype) else None
-        return dict(self).get(key, '???')
-
-
-class COLOR():
-    '''Give escape format strings (color, face) a name.'''
-    END    = "\033[0m"
-    BOLD   = "\033[1m"
-    LINE   = "\033[4m"
-    RED    = "\033[91m"
-    GREEN  = "\033[92m"
-    YELLOW = "\033[93m"
-    BLUE   = "\033[94m"
-    PURPLE = "\033[95m"
-    AQUA   = "\033[96m"
-
-
-def fmtStr(string, color):
-    '''Print a string quoted by some format specifiers.'''
-    # colored output only supported with linux
-    return ("%s%s%s" %(color, string, COLOR.END)
-            if currentOS == 'Linux'
-            else string)
-
-
-def fmtGreen(string):
-    '''Print string in green.'''
-    return fmtStr(string, COLOR.GREEN)
-
-
-def fmtRed(string):
-    '''Print string in red.'''
-    return fmtStr(string, COLOR.RED)
-
-
-def fmtYellow(string):
-    '''Print string in yellow.'''
-    return fmtStr(string, COLOR.YELLOW)
-
-
-def fmtBold(string):
-    '''Print string in bold face.'''
-    return fmtStr(string, COLOR.BOLD)
-
-
-reAnsiEscape = None
-
-
-def fmtEscape(string):
-    '''Return a string with all ASCII escape sequences removed.'''
-    global reAnsiEscape
-    if reAnsiEscape is None:
-        reAnsiEscape = re.compile(r'\x1b[^m]*m')
-
-    return reAnsiEscape.sub('', string)
-
-
-def dynFormat(s, *keys):
-    return s.replace('%', '%%(%s)') % keys
-
-
-################################################## getConsoleSize()
-
-fallbackConsoleSize = (80, 25)
-if (currentOS in ['Linux', 'Darwin']) or currentOS.startswith('CYGWIN'):
-    import fcntl
-    import termios
-    # source: https://gist.github.com/jtriley/1108174
-
-    def getConsoleSize():
-        def ioctl_GWINSZ(fd):
-            try:
-                return struct.unpack(
-                    'hh', fcntl.ioctl(fd, termios.TIOCGWINSZ, '1234'))
-            except EnvironmentError:
-                return None
-
-        cr = ioctl_GWINSZ(0) or ioctl_GWINSZ(1) or ioctl_GWINSZ(2)
-        if not cr:
-            try:
-                fd = os.open(os.ctermid(), os.O_RDONLY)
-                cr = ioctl_GWINSZ(fd)
-                os.close(fd)
-            except EnvironmentError:
-                pass
-
-        if not cr:
-            try:
-                cr = (os.environ['LINES'], os.environ['COLUMNS'])
-            except (EnvironmentError, KeyError):
-                cr = fallbackConsoleSize
-
-        return int(cr[0]), int(cr[1])
-elif currentOS == 'Windows':
-    def getConsoleSize():
-        cr = fallbackConsoleSize
-        try:
-            from ctypes import windll, create_string_buffer
-            # stdin handle is -10
-            # stdout handle is -11
-            # stderr handle is -12
-            h = windll.kernel32.GetStdHandle(-12)
-            csbi = create_string_buffer(22)
-            res = windll.kernel32.GetConsoleScreenBufferInfo(h, csbi)
-            if res:
-                (left, top, right, bottom) = struct.unpack("10x4h4x", csbi.raw)
-                cr = (right - left, bottom - top)
-        except (ImportError, EnvironmentError):
-            pass
-
-        return cr
-else:
-    def getConsoleSize():
-        return fallbackConsoleSize
-
-
-################################################## worker's CONSTANT classes
-class NAME(object):
-    DATA            = 'data'
-    FWDATA          = 'dataForward'
-    BWDATA          = 'dataBackward'
-    DTYPE           = 'dtype'
-    SHAPE           = 'shape'
-    SHAPE_T         = 'shapeBackward'
-    ALIGN           = 'align'
-    CENTER          = 'center'
-    FORMAT          = 'format'
-    NAME            = 'name'
-
-    CLASS           = 'class'
-    TARGET          = 'target'
-    FILENAME        = 'filename'
-    CAPTION         = 'caption'
-    BENCHMARK       = 'bench'
-    DOCU            = 'docu'
-    TEST            = 'test'
-    COMMON          = 'common'
-    TEMPLATE        = 'template'
-    VARIANT         = 'variant'
-    RESULT          = 'result'
-    HEADER          = 'header'
-
-    TYPENAME        = TypeDict({
-        np.int8:       'i08', np.int16:      'i16', np.int32:      'i32',
-        np.int64:      'i64', np.float32:    'f32', np.float64:    'f64',
-        np.complex64:  'c32', np.complex128: 'c64', None:          '???'
-    })
-
-    ALLTYPES        = [np.int8, np.int16, np.int32, np.int64,
-                       np.float32, np.float64,
-                       np.complex64, np.complex128]
-    FEWTYPES        = [np.int32, np.float32, np.complex64]
-
-    SINGLETYPES     = [np.int32, np.int16, np.float32, np.complex64]
-    DOUBLETYPES     = [np.int64, np.float64, np.complex128]
-
-    INTTYPES        = [np.int8, np.int16, np.int32, np.int64]
-    FLOATTYPES      = [np.float32, np.float64]
-    COMPLEXTYPES    = [np.complex64, np.complex128]
-
-    LARGETYPES      = [np.int32, np.int64, np.float32, np.float64,
-                       np.complex64, np.complex128]
-
-    ALLALIGNMENTS   = [ALIGNMENT.FCONT, ALIGNMENT.CCONT, ALIGNMENT.STRIDE]
-
-    # repeat some of the definitions in this unit to allow compact imports
-    ALIGNMENT       = ALIGNMENT
-    ArrayGenerator  = ArrayGenerator
-    Permutation     = Permutation
-    IgnoreFunc      = IgnoreFunc
+        # define defaults
+        defaults={
+            BENCH.COMMON: {
+                # default naming of benchmark target
+                BENCH.NAME          : dynFormat(
+                    "%s.%s", NAME.CLASS, NAME.TARGET),
+                BENCH.CAPTION       : dynFormat("%s", BENCH.NAME),
+
+                # default benchmark abort criteria
+                BENCH.LIMIT_MEMORY  : 1e6,  # kilobytes
+                BENCH.LIMIT_INIT    : 1.,   # seconds
+                BENCH.LIMIT_ITER    : 1.,  # seconds for all targets combined
+                BENCH.LIMIT_SIZE    : 1e9,  # problem size
+
+                # default benchmark parameters
+                BENCH.STEP_START_K  : 1,
+                BENCH.STEP_MINITEMS : 5,
+
+                # default benchmark control functionals
+                BENCH.FUNC_INIT     : None,
+                BENCH.FUNC_GEN      : None,
+                BENCH.FUNC_SIZE     : (lambda k: k),
+                BENCH.FUNC_STEP     : (lambda k: k * 10 ** (1. / 12)),
+
+                # default benchmark timing parameters
+                BENCH.MEAS_MINTIME  : 0.003,
+                BENCH.MEAS_MINREPS  : 7,
+                BENCH.MEAS_MINRUNS  : 7,
+                BENCH.MEAS_COMPACT  : True
+            },
+            BENCH.FORWARD: {
+                BENCH.CAPTION       : dynFormat("%s (Multiplication)",
+                                                BENCH.NAME),
+                BENCH.FUNC_INIT     : testInitForward
+            },
+            BENCH.OVERHEAD: {
+                BENCH.CAPTION       : dynFormat("%s (call overhead)",
+                                                BENCH.NAME),
+                BENCH.FUNC_INIT     : testInitOverhead,
+                BENCH.FUNC_SIZE     : (lambda k: 2 ** k),
+                BENCH.FUNC_STEP     : (lambda k: k + 1)
+            },
+            BENCH.PERFORMANCE: {
+                BENCH.CAPTION       : dynFormat("%s (Algorithm performance)",
+                                                BENCH.NAME),
+                BENCH.FUNC_INIT     : testInitPerformance
+            },
+            BENCH.DTYPES: {
+                BENCH.CAPTION       : dynFormat("%s (impact of data type)",
+                                                BENCH.NAME),
+                BENCH.FUNC_INIT     : testInitDtype,
+                BENCH.FUNC_SIZE     : (lambda k: 2 ** k),
+                BENCH.FUNC_STEP     : (lambda k: k + 1)
+            }
+        }
+
+        # call parent initialization with Test-specific options
+        super(Benchmark, self).__init__(
+            targetClass, targetOptionMethod='_getBenchmark',
+            runnerDefaults=defaults, extraOptions=extraOptions)
+
+    def getResult(self, nameResult, *nameParams):
+        """Short summary.
+
+        Parameters
+        ----------
+        nameResult : type
+            Description of parameter `nameResult`.
+        *nameParams : type
+            Description of parameter `*nameParams`.
+
+        Returns
+        -------
+        type
+            Description of returned object.
+
+        """
+        result=self.results.get(nameResult)
+        header=result[BENCH.HEADER]
+        indices=[header.index(key)
+                 for key in (nameParams if len(nameParams) > 0 else header)]
+        return result[BENCH.RESULT][:, indices]
+
+    def _run(self, name, options):
+        """Short summary.
+
+        Parameters
+        ----------
+        name : type
+            Description of parameter `name`.
+        options : type
+            Description of parameter `options`.
+
+        Returns
+        -------
+        type
+            Description of returned object.
 
+        """
+        '''
+        Perform a runtime performance evaluation.
+        '''
+        # output benchmark title
+        self.emitStatus(fmtBold(">> %s" %(getattr(paramDict(options),
+                                                  BENCH.CAPTION))))
+
+        # perform the benchmarks
+        run, result, header={}, {}, None
+        result[BENCH.RESULT]=[]
+        valK, numN=options[BENCH.STEP_START_K], 0
+        numItems = 0
+        while (run.get(BENCH.RESULT_MEMORY, 1) < options[BENCH.LIMIT_MEMORY] and
+               run.get(BENCH.RESULT_INIT, 0.) < options[BENCH.LIMIT_INIT] and
+               run.get(BENCH.RESULT_ITER, 0.) < options[BENCH.LIMIT_ITER] and
+               run.get(BENCH.RESULT_SIZE, 1)  < options[BENCH.LIMIT_SIZE] or
+               numItems < options[BENCH.STEP_MINITEMS]):
+            # run test, init result dictionary for this run
+            run.clear()
+
+            # estimate next size
+            valK, lastValK=options[BENCH.FUNC_STEP](valK), valK
+            if valK == lastValK:
+                raise ValueError(
+                    "Stepping function caused endless loop: abort. [%s]" %(
+                        options))
+            numK=int(round(valK))
+            numN, lastNumN=options[BENCH.FUNC_SIZE](numK), numN
+
+            # if problem size did not change since last iter, skip
+            if lastNumN == numN:
+                #print("skipping %f (%d, %d)"%(valK, lastNumN, numN))
+                continue
+            run[BENCH.RESULT_SIZE] = numN
 
-################################################################################
-################################################## class Runner
-class Worker(object):
-    '''
-    options - dictionary structure containing options for multiple targets.
-    {   'nameOfTarget': {'parameter': 123,
-    'anotherParameter': 456
-    }, NAME.DEFAULTS:  {'parameter': default parameter unless overwritten
-    within the selected target
-    }}
+            # count number of elements in result to force minimal amount of
+            numItems += 1
 
-    results - output of each target's as specified in options
-    '''
+            ####################### construct test instance and init call list
+            calls={}
+            run[BENCH.RESULT_INIT]=timeit(
+                lambda : calls.update(options[BENCH.FUNC_INIT](
+                    options[BENCH.FUNC_GEN], numK, numN)),
+                number=1)
+
+            # determine total memory consumption of all call-related stuff and
+            # matrix memory consumption of each call target separately
+            totalMemUsed=getMemoryFootprint(calls) / 1e3
+            for tag, call in calls.items():
+                # memory consumption of each calls' matrix instance
+                if 'Mem' in call:
+                    memCall=call['Mem'] / 1e3
+                    totalMemUsed += memCall
+                    run["%sMem" %(tag)]=memCall
+
+                # copy effort columns if defined in testInitCalls
+                for key in [BENCH.RESULT_OVH_NESTED_F,
+                            BENCH.RESULT_OVH_NESTED_B,
+                            BENCH.RESULT_EFF_NESTED_F,
+                            BENCH.RESULT_EFF_NESTED_B,
+                            BENCH.RESULT_COMPLEXITY_F,
+                            BENCH.RESULT_COMPLEXITY_B,
+                            BENCH.RESULT_ESTIMATE_FWD,
+                            BENCH.RESULT_ESTIMATE_BWD]:
+                    if key in call:
+                        run[key] = call[key]
+
+            run[BENCH.RESULT_MEMORY]=totalMemUsed
+
+            # do one extra warm-up run before starting actual measurements
+            # to fetch and all required code and fetch data memory
+            timeCalls(calls, **options)
+
+            # determine runtime statistics and compose runs
+            # alongside, check timing limits
+#            run[BENCH.RESULT_ITER] = 0
+            iterTime = time.time()
+            run.update(timeCalls(calls, **options))
+#            for tag in calls.keys():
+#                run[BENCH.RESULT_ITER] += run["%sAvg" %(tag)]
+            run[BENCH.RESULT_ITER] = time.time() - iterTime
+
+            result[BENCH.RESULT].append(run.copy())
+
+            # format instant output
+            def formatToken(token):
+                try:
+                    # int or scientific notation
+                    return ("%10d" if isinstance(token, int)
+                            else "%10.3e") %(token)
+                except TypeError:
+                    # if that fails: make a string out of whatever it is
+                    return "%11s" %(token)
+
+            # print header in first iteration
+            if BENCH.HEADER not in result:
+                # determine
+                keys=set([key
+                          for step in result[BENCH.RESULT] for key in step])
+
+                # let some key names have priority in ordering of header.
+                priority=[BENCH.RESULT_SIZE, BENCH.RESULT_MEMORY,
+                          BENCH.RESULT_INIT, BENCH.RESULT_ITER]
+
+                # return the priority keys (in order of specification),
+                # followed by the other keys (alphabetically sorted)
+                result[BENCH.HEADER]=(
+                    [key for key in priority if key in keys] +
+                    [key for key in sorted(keys) if key not in priority])
+
+                # emit header status line (--> printing)
+                strHeader=" ".join([formatToken(f)
+                                    for f in result[BENCH.HEADER]])
+                self.emitStatus(strHeader + '\n' + '-' * len(strHeader))
+
+            # output runs in same order as header
+            row=['.'] * len(result[BENCH.HEADER])
+            for key in run.keys():
+                try:
+                    row[result[BENCH.HEADER].index(key)]=run[key]
+                except KeyError:
+                    pass
+
+            # print the whole stuff
+            self.emitStatus("[%s]" %(", ".join([formatToken(f) for f in row])))
+
+        # collate result dictionary structure to numpy array
+        res, header=result[BENCH.RESULT], result[BENCH.HEADER]
+        arrRes=np.zeros((len(res), len(header)), dtype=np.float64)
+        for ii, item in enumerate(res):
+            arrRes[ii, :]=np.array([item.get(key, np.NaN)
+                                    for key in header])
+        result[BENCH.RESULT]=arrRes
 
-    cbStatus=None
-    cbResult=None
-    target=None
+        return result
 
-    def __init__(self, targetClass, **options):
+    # control verbosity of _run() and printStatus()
+    @property
+    def verbosity(self):
+        return self.cbStatus == self.printStatus
+
+    @verbosity.setter
+    def verbosity(self, value):
+        self.cbStatus=self.printStatus if value is True else None
+
+    def printStatus(self, message):
+        print(message)
+
+    def getFilename(self, nameResult, path='', addVersionTag=True):
+        return os.path.join(path, "%s.%s%s.csv" %(
+            self.target.__class__.__name__, nameResult,
+            ".%s" %(__version__) if addVersionTag else ""))
+
+    def saveResult(self, nameResult, outPath='', addVersionTag=True,
+                   strFormat='%.6e', chrDelimiter=',', chrNewline=os.linesep):
+        """Short summary.
+
+        Parameters
+        ----------
+        nameResult : type
+            Description of parameter `nameResult`.
+        outPath : type
+            Description of parameter `outPath`.
+        addVersionTag : type
+            Description of parameter `addVersionTag`.
+        strFormat : type
+            Description of parameter `strFormat`.
+        chrDelimiter : type
+            Description of parameter `chrDelimiter`.
+        ' : type
+            Description of parameter `'`.
+        chrNewline : type
+            Description of parameter `chrNewline`.
+
+        Returns
+        -------
+        type
+            Description of returned object.
+
+        """
         '''
-        Setup an inspection environment on a fastmat class specified in target.
-        Along the way an empty instance of target will be created and aside
-        the default options, which may be specified in runnerDefaults, an
-        arbitrarily named method of target may be specified to return more
-        specific options when called.
-        extraOptions may be specified to overwrite any parameter with highest
-        priority.
-        Both extraOptions and runnerDefaults must be specified as a two-level
-        dictionary with the outer level specifying target names as keys and the
-        inner level the actual parameter for the target.
+        Print data table to csv file. The result is organized as a list of
+        dicts containing information in key=value pairs. The header will be
+        extracted from the keys of the result data dictionaries. If the file
+        does not exist it will be created.
         '''
-        # the test target is a fastmat class to be instantiated in the runners
-        if not inspect.isclass(targetClass):
-            raise ValueError("target in init of Runner must be a class type")
-
-        # set defaults for options
-        targetOptionMethod = options.get('targetOptionMethod', None)
-        runnerDefaults = options.get('runnerDefaults', {})
-        extraOptions = options.get('extraOptions', {})
-
-        self.target=targetClass.__new__(targetClass)
+        if nameResult not in self.results:
+            raise ValueError("No benchmark result of such name found")
 
-        # targetOptionMethod specifies a method name of target which will
-        # return a dictionary with class-specific options if called. If this
-        # functionality is not needed, targetOptionsMethod or runnerDefaults
-        # may be left to their default values.
-        targetOptionMethod=getattr(self.target, targetOptionMethod, None)
-        options={name: mergeDicts(target, extraOptions)
-                 for name, target in ({} if targetOptionMethod is None
-                                      else targetOptionMethod()).items()}
-
-        # determine keys for final output
-        keys=[name for name in options.keys() if name != NAME.COMMON]
-
-        # start with the defaults for the selected keys as a baseline
-        common=runnerDefaults.get(NAME.COMMON, {})
-        self.options={name: mergeDicts(common, runnerDefaults.get(name, {}))
-                      for name in keys}
-
-        # a NAME.TEMPLATE parameter in a target will cause the specified
-        # target to be extend by the default options of another target.
-        # Priority order: extraOptions > options > defaults > COMMON
-        for name, target in self.options.items():
-            template=(options[name][NAME.TEMPLATE]
-                      if name in options and NAME.TEMPLATE in options[name]
-                      else (runnerDefaults[name][NAME.TEMPLATE]
-                            if (name in runnerDefaults and
-                                NAME.TEMPLATE in runnerDefaults[name])
-                            else None))
-
-            if template is not None:
-                target.update(
-                    runnerDefaults.get(template, {}))
-
-        # now add our specific options from options and extraoptions
-        common=options.get(NAME.COMMON, {})
-        self.options={name: mergeDicts(self.options.get(name, {}),
-                                       mergeDicts(common, options[name]))
-                      for name in keys}
-
-        # finally, tag each target with its target name so that parameter links
-        # may address it over the key [NAME.TARGET]. Also, write down the name
-        # of the class in [NAME.CLASS]
-        for name, target in self.options.items():
-            target[NAME.TARGET]=name
-            target[NAME.CLASS]=targetClass.__name__
-
-        # initialize output
-        self.results=AccessDict({})
-
-    def emitStatus(self, *args):
-        if self.cbStatus is not None:
-            self.cbStatus(*args)
-
-    def emitResult(self, *args):
-        if self.cbResult is not None:
-            self.cbResult(*args)
+        result=self.results[nameResult]
+        arrResult=result[BENCH.RESULT]
+        lstHeader=result[BENCH.HEADER]
+
+        filename=self.getFilename(nameResult, path=outPath,
+                                  addVersionTag=addVersionTag)
+        # force existance of output file
+        dirname=os.path.dirname(filename)
+        if dirname != '' and not os.path.exists(dirname):
+            os.makedirs(dirname)
+
+        # save csv-file to memory
+        np.savetxt(filename, arrResult,
+                   header=chrDelimiter.join(lstHeader), comments='',
+                   fmt=strFormat, newline=chrNewline, delimiter=chrDelimiter)
+
+        return filename
+
+    def plotResult(self, nameResult, outPath='', addVersionTag=True,
+                   strFormat='%.6e', chrDelimiter=',', chrNewline=os.linesep):
+        """Short summary.
+
+        Parameters
+        ----------
+        nameResult : type
+            Description of parameter `nameResult`.
+        outPath : type
+            Description of parameter `outPath`.
+        addVersionTag : type
+            Description of parameter `addVersionTag`.
+        strFormat : type
+            Description of parameter `strFormat`.
+        chrDelimiter : type
+            Description of parameter `chrDelimiter`.
+        ' : type
+            Description of parameter `'`.
+        chrNewline : type
+            Description of parameter `chrNewline`.
+
+        Returns
+        -------
+        type
+            Description of returned object.
 
-    def run(self, *targetNames, **extraArgs):
+        """
         '''
-        Execute all selected targets by a list of targetNames.
-        If *targetNames is empty all targets will be run.
-        The output of each :math:`TARGET` will be written to
-        self.results[:math:`TARGET`]
+        Print data table to csv file. The result is organized as a list of
+        dicts containing information in key=value pairs. The header will be
+        extracted from the keys of the result data dictionaries. If the file
+        does not exist it will be created.
         '''
-        # determine console width
-        self.consoleWidth=getConsoleSize()[1]
+        if nameResult not in self.results:
+            raise ValueError("No benchmark result of such name found")
+
+        result=self.results[nameResult]
+        arrResult=result[BENCH.RESULT]
+
+        filename=self.getFilename(nameResult, path=outPath,
+                                  addVersionTag=addVersionTag)
 
-        if len(targetNames) == 0:
-            targetNames=self.options.keys()
+        filename = filename.replace('csv', 'png')
 
-        targets={name: self.options[name]
-                 for name in targetNames if name in self.options}
+        # force existance of output file
+        dirname=os.path.dirname(filename)
+        if dirname != '' and not os.path.exists(dirname):
+            os.makedirs(dirname)
 
-        for name, target in sorted(targets.items()):
-            options=target.copy()
+        import matplotlib.pyplot as plt
 
-            if len(extraArgs) > 0:
-                options.update(extraArgs)
+        plt.loglog(arrResult[:, 0], arrResult[:, 1:])
 
-            result = self._run(name, options)
+        plt.savefig(
+            filename,
+            dpi=300,
+            transparent=True,
+            bbox_inches='tight'
+        )
 
-            # make all result dicts of type accessDict for easy access
-            self.results[name] = convertToAccessDicts(result)
-            if self.cbResult is not None:
-                self.cbResult(name, result)
+        return filename
```

### Comparing `fastmat-0.2a4/fastmat/inspect/test.py` & `fastmat-0.2rc0/fastmat/inspect/common.py`

 * *Files 27% similar despite different names*

```diff
@@ -11,848 +11,1153 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+import copy
+import inspect
 import itertools
+import os
+import re
+import six
+import struct
 import numpy as np
-from pprint import pprint
+from scipy import sparse
+from platform import system as pfSystem
 
-from .common import *
-from ..core.types import getTypeEps, safeTypeExpansion
-from ..Matrix import Matrix
-from ..algorithms import Algorithm
-from ..Diag import Diag
-from ..Eye import Eye
-from ..Parametric import Parametric
-from ..Zero import Zero
+from ..core.types import isInteger
 
+try:
+    from itertools import izip
+except ImportError:         # python 3.x
+    izip = zip
 
-################################################## TEST CONSTANT-def class
-class TEST(NAME):
-    CLASS           = 'class'
-    TRANSFORMS      = 'transform'
-    ALGORITHM       = 'algorithm'
+currentOS = pfSystem()
 
-    OBJECT          = 'object'
-    ARGS            = 'testArgs'
-    KWARGS          = 'testKwargs'
-    NUM_ROWS        = 'numRows'
-    NUM_COLS        = 'numCols'
-    DATACOLS        = 'numVectors'
-    DATATYPE        = 'dataType'
-    DATASHAPE       = 'dataShape'
-    DATAALIGN       = 'dataAlign'
-    DATASHAPE_T     = 'dataShapeBackward'
-    DATAGEN         = 'dataGenerator'
-    DATACENTER      = 'dataDistCenter'
-    DATAARRAY       = 'arrData'
-    INIT            = 'init'
-    INITARGS        = 'args'
-    INITKWARGS      = 'kwargs'
-    INIT_VARIANT    = 'initVariant'
-    INSTANCE        = 'instance'
-    REFERENCE       = 'reference'
-    QUERY           = 'query'
-    NAMINGARGS      = 'namingArgs'
-    NAMING          = 'naming'
-    TOL_MINEPS      = 'tolMinEps'
-    TOL_POWER       = 'tolPower'
-    IGNORE          = 'ignore'
-    PARAMALIGN      = 'alignment'
-    RESULT_TOLERR   = 'testTolError'
-    RESULT_INPUT    = 'testInput'
-    RESULT_OUTPUT   = 'testOutput'
-    RESULT_REF      = 'testReference'
-    RESULT_IGNORED  = 'testResultIgnored'
-    RESULT_INFO     = 'testInfo'
-    RESULT_TYPE     = 'testResultType'
-    RESULT_PROX     = 'testResultProximity'
-    ALG             = 'algorithm'
-    ALG_MATRIX      = 'algorithmMatrix'
-    ALG_ARGS        = 'algorithmArgs'
-    ALG_KWARGS      = 'algorithmKwargs'
-    REFALG          = 'refAlgorithm'
-    REFALG_ARGS     = 'refAlgorithmArgs'
-    REFALG_KWARGS   = 'refAlgorithmKwargs'
-
-    CHECK_PROXIMITY = 'checkProximity'
-    CHECK_DATATYPE  = 'checkDataType'
-    TYPE_EXPECTED   = 'typeExpected'
-    TYPE_PROMOTION  = 'typePromotion'
 
 ################################################################################
-##################################################  test implementations
+################################################## CONSTANT definition classes
+class ALIGNMENT(object):
+    """Short summary."""
+    DONTCARE        = '-'
+    FCONT           = 'F'
+    CCONT           = 'C'
+    STRIDE          = 'S'
 
 
-################################################## tryQuery
-def tryQuery(nameTest, query, argument):
-    try:
-        return query(argument)
-    except Exception as e:
-        print("Exception %s in %s: %s" %(
-            repr(e), nameTest, query,
-        ))
-        pprint(argument)
-        raise e
-
-
-################################################## compareResults
-def compareResults(test, query):
-
-    def getOption(option, default):
-        return query.get(option, test.get(option, default))
-
-    arrOutput=query[TEST.RESULT_OUTPUT]
-    arrReference=query[TEST.RESULT_REF]
-    arrMatrix=test[TEST.REFERENCE]
-
-    # to extract the operation data type and shape when checking an algorithm
-    # we cannot get this information from TEST.INSTANCE as this then refers to
-    # the algorithm instance object itself and not to the matrix it operates
-    # on. We need to use the TEST.ALG_MATRIX as this holds the required matrix
-    # instance object used within the actual algorithm
-    instance = query[TEST.INSTANCE] = getOption(
-        TEST.ALG_MATRIX,
-        test[TEST.INSTANCE]
-    )
-
-    # get comparision options from test and query dicts. Priority has query
-    minimalType=np.dtype(getOption(TEST.TYPE_PROMOTION, np.int8))
-    expectedType=np.dtype(getOption(TEST.TYPE_EXPECTED,
-                                    np.promote_types(instance.dtype,
-                                                     minimalType)))
-    maxEps=getOption(TEST.TOL_MINEPS, 0.)
-    tolPower=getOption(TEST.TOL_POWER, 1.)
-    ignoreType=not getOption(TEST.CHECK_DATATYPE, True)
-    ignoreProximity=not getOption(TEST.CHECK_PROXIMITY, True)
-
-    # check if shapes match. If they do, check all elements
-    if arrOutput.shape != arrReference.shape:
-        query[TEST.RESULT] = False
-        query[TEST.RESULT_IGNORED] = False
-        query[TEST.RESULT_INFO] = fmtRed(
-            "%s!=%s" %(str(arrOutput.shape), str(arrReference.shape)))
-        return query
-
-    # if the query was not generated from input data, assume an int8-Eye-Matrix
-    if TEST.RESULT_INPUT in query:
-        arrInput=query[TEST.RESULT_INPUT]
-        # check that input vector actually contains energy
-        if np.linalg.norm(arrInput) == 0:
-            print("Test query data causing exception:")
-            pprint(query)
-            raise ValueError("All-zero input vector detected in test")
-
-        expectedType = np.promote_types(expectedType, arrInput.dtype)
-        maxEps = max(maxEps, getTypeEps(arrInput.dtype))
-
-    # compare returned output data type to expected (qType) to verify
-    # functionality of fastmat built-in type promotion mechanism
-    resultType = np.can_cast(arrOutput.dtype, expectedType, casting='no')
-
-    maxEps = max(maxEps,
-                 getTypeEps(np.promote_types(minimalType, instance.dtype)),
-                 getTypeEps(np.promote_types(minimalType, arrReference.dtype)))
-
-    # determine allowed tolerance maxima (allow accuracy degradation of chained
-    # operations by representing multiple stages by a power on operation count
-    # the test distribution function generates random arrays with their absolute
-    # element values in the range [0.4 .. 0.8]. This can be described by a
-    # `dynamics`-factor of 2 per computation stage (parameter TEST.TOL_POWER)
-    dynamics = 2.
-    maxDim = max(arrMatrix.shape + instance.shape)
-    tolError = 5 * dynamics * maxEps * (dynamics * np.sqrt(maxDim)) ** tolPower
-    query[TEST.RESULT_TOLERR] = tolError
-
-    maxRef = float(np.amax(np.abs(arrReference)))
-    maxDiff = float(np.amax(np.abs(arrOutput - arrReference)))
-    error = (maxDiff / maxRef if maxRef != 0 else maxDiff)
-    resultProximity=(error <= tolError) or (maxRef <= tolError)
-
-    # determine final result
-    query[TEST.RESULT] = (resultType and resultProximity)
-    # result ignored: whenever the main result is not true but an ignore in one
-    # of the tests would cause it to become true
-    query[TEST.RESULT_IGNORED] = ((resultType or ignoreType) and
-                                  (resultProximity or ignoreProximity) and
-                                  not query[TEST.RESULT])
-    query[TEST.RESULT_TYPE] = (resultType, ignoreType,
-                               arrOutput.dtype, expectedType)
-    query[TEST.RESULT_PROX] = (resultProximity, ignoreProximity, error, maxRef)
-
-    return query
-
-
-################################################## formatResult()
-def formatResult(result):
-    # if a result info was already generated, return this. Otherwise generate it
-    if TEST.RESULT_INFO in result:
-        return result[TEST.RESULT_INFO]
-
-    # fetch detailed results from result
-    resultType, ignoreType, outputType, expectedType=result[TEST.RESULT_TYPE]
-    resultProx, ignoreProx, error, maxRef=result[TEST.RESULT_PROX]
-
-    # format string output
-    if resultType:
-        strInfo=fmtGreen(NAME.TYPENAME[outputType])
-    elif ignoreType:
-        strInfo=fmtYellow(NAME.TYPENAME[outputType])
-    else:
-        strInfo=fmtRed("%s!=%s"% (NAME.TYPENAME[outputType],
-                                  NAME.TYPENAME[expectedType]))
+################################################################################
+################################################## Permutation funcs and classes
+
+class AccessDict(dict):
+    """Short summary."""
+    def __getattr__(self, key):
+        if key in self:
+            return self[key]
+        else:
+            found = [kk for kk in sorted(self.keys())
+                     if kk.startswith(key)]
+            return ([self[kk] for kk in found] if len(found) > 2
+                    else (None if len(found) == 0
+                          else self[found[0]]))
+
+    def __repr__(self):
+        return str(self.keys())
+
+
+def convertToAccessDicts(level):
+    """Short summary.
+
+    Parameters
+    ----------
+    level : type
+        Description of parameter `level`.
+
+    Returns
+    -------
+    type
+        Description of returned object.
+
+    """
+    for key, value in level.items():
+        if isinstance(value, dict) and (value is not value):
+            level[key] = convertToAccessDicts(value)
+
+    return AccessDict(level)
+
+
+################################################## class uniqueNameDict
+class uniqueNameDict(dict):
+    """Short summary."""
+    '''
+    Modified dictionary: suffixes key names with integer to maintain uniqueness.
+    '''
+
+    def __setitem__(self, key, value):
+        index = 1
+        strKey = key
+        while True:
+            if strKey not in self:
+                break
+            index += 1
+            strKey = "%s_%03d" %(key, index)
 
-    if not resultProx:
-        if error > 0 and maxRef > 0:
+        dict.__setitem__(self, strKey, value)
+
+
+################################################## class paramDict
+reFormatString = re.compile(r'%\(.+\)')
+
+
+class paramDict(dict):
+    """Short summary."""
+
+    def __getattr__(self, key):
+        # evaluate nested format-string parameters, update format results
+        value, lastValue = super(paramDict, self).__getitem__(key), None
+
+        while id(lastValue) != id(value):
+            lastValue = value
+            if isinstance(value, str):
+                if value in self and value != key:
+                    value = getattr(self, value)
+                elif reFormatString.search(value):
+                    value = value %self
+
+            elif (inspect.isroutine(value) and
+                  not isinstance(value, IgnoreFunc)):
+                value = value(self)
+                self[key] = value
+
+        return value
+
+
+################################################## class Permutation
+class Permutation(list):
+    """Short summary."""
+
+    def __repr__(self):
+        return "%s(%s)" % (self.__class__.__name__,
+                           super(Permutation, self).__repr__())
+
+    def __str__(self):
+        return "%s(%s)" % (self.__class__.__name__,
+                           super(Permutation, self).__str__())
+
+
+################################################## class VariantPermutation
+class VariantPermutation(Permutation):
+    pass
+
+
+################################################## class IgnoreDict
+class IgnoreDict(dict):
+    pass
+
+
+################################################## class IgnoreFunc
+class IgnoreFunc(object):
+
+    def __init__(self, fun):
+        self._fun = fun
+
+    def __call__(self, *args, **kwargs):
+        return self._fun(*args, **kwargs)
+
+
+################################################## paramApplyDefaults()
+def paramApplyDefaults(
+    params,
+    templates=None,
+    templateKey=None,
+    extraArgs=None
+):
+    """Short summary.
+
+    Parameters
+    ----------
+    params : type
+        Description of parameter `params`.
+    templates : type
+        Description of parameter `templates`.
+    templateKey : type
+        Description of parameter `templateKey`.
+    extraArgs : type
+        Description of parameter `extraArgs`.
+
+    Returns
+    -------
+    type
+        Description of returned object.
+
+    """
+
+    # have some defaults from templates
+    # first, fetch the template as defaults, then update with target,
+    # then assign the whole dict to target
+    result = {}
+    if templates is not None:
+        # 1. COMMON - section of templates (lowest-priority)
+        result.update(templates.get(NAME.COMMON, {}))
+        # 2. the templates-section corresponding to the templateKey
+        result.update(templates.get(templateKey, {}))
+        # 3. specific reference to a template by the 'template' key in params
+        if NAME.TEMPLATE in params:
+            result.update(templates.get(params[NAME.TEMPLATE], {}))
+
+    # 4. actual parameters (params)
+    result.update(params)
+
+    # 5. extraArgs (which usually come from command-line) (top-priority)
+    if extraArgs is not None:
+        for p in extraArgs:
+            for pp in list(p.split(',')):
+                tokens = pp.split('=')
+                if len(tokens) >= 2:
+                    string = "=".join(tokens[1:])
+                    try:
+                        val = int(string)
+                    except ValueError:
+                        try:
+                            val = float(string)
+                        except ValueError:
+                            val = string
+                    result[tokens[0]] = val
+
+    return paramDict(result)
+
+
+################################################## paramPermute()
+def paramPermute(dictionary, copy=True, PermutationClass=Permutation):
+    """Short summary.
+
+    Parameters
+    ----------
+    dictionary : type
+        Description of parameter `dictionary`.
+    copy : type
+        Description of parameter `copy`.
+    PermutationClass : type
+        Description of parameter `PermutationClass`.
+
+    Returns
+    -------
+    type
+        Description of returned object.
+
+    """
+    '''
+    Return a list of cartesian-product combination of all dictionary values
+    holding a Permutation list object. If copy is True, the resulting list will
+    be applied back to input dictionary copies before returning, resulting in
+    a list of copies with the permutation replacements being made on the input
+    dictionary. Parameter permutations must be indicated by wrapping a list in
+    a Permutation class instance.
+    '''
+    # isolate the permutation parameters from the dictionary
+    parameters = {key: list(value)
+                  for key, value in dictionary.items()
+                  if isinstance(value, PermutationClass)}
+
+    # perform a cartesian product -> list of permuted instances
+    permutations = [dict(izip(parameters, x))
+                    for x in itertools.product(*six.itervalues(parameters))]
+    if len(permutations) == 1:
+        permutations = [{}]
+
+    # apply the permutations to the input dictionary (generating copies)
+    def dictCopyAndMerge(source, merge):
+        result = source.copy()
+        result.update(merge)
+        return paramDict(result)
+    return [dictCopyAndMerge(dictionary, permutation)
+            for permutation in permutations] if copy else permutations
+
+
+################################################## paramDereferentiate()
+def paramDereferentiate(currentLevel, paramDict=None):
+    """Short summary.
+
+    Parameters
+    ----------
+    currentLevel : type
+        Description of parameter `currentLevel`.
+    paramDict : type
+        Description of parameter `paramDict`.
+
+    Returns
+    -------
+    type
+        Description of returned object.
+
+    """
+    '''
+    Replace all text value identifyers matching a target key name with the
+    key values it's pointing to allowing parameter links. Then, recurse through
+    an arbitrary depth of container types (dicts, lists, tuples) found in the
+    first stage, continuing dereferentiation.
+    Returns the modified currentLevel container.
+    '''
+    # set paramDict in first level, determine iterator for currentLevel
+    iterator = currentLevel.items() \
+        if isinstance(currentLevel, dict) else enumerate(currentLevel)
+    if paramDict is None:
+        paramDict = currentLevel
+
+    # STAGE 1: Replace all dictionary values matching a key name in paramDict
+    #          with the corresponding value of that paramDict-entry. Also build
+    #          a container list for stage two.
+    dictIterables = {}
+    for key, value in iterator:
+        if isinstance(value, (list, tuple, dict)):
+            dictIterables[key] = value
+        else:
+            if not isinstance(value, str):
+                continue
             try:
-                strDiff = "%+2.2d" %(
-                    int(min(99, np.round(np.log10(1. * error / maxRef)))))
-            except OverflowError:
-                strDiff = '---'
+                paramValue = paramDict.get(value, None)
+                if (paramValue is not None and
+                        not isinstance(paramValue, Permutation)):
+                    currentLevel[key] = paramValue
+                    if isinstance(paramValue, (list, tuple, dict)):
+                        dictIterables[key] = paramValue
+            except TypeError:
+                continue
+
+    # STAGE 2: Crawl the containers found in stage 1, repeating the process.
+    #          Note that nested containers are copied in the process.
+    #          The parameter dictionary paramDict stays the same for all levels.
+    for key, iterable in dictIterables.items():
+        # copy the container to allow modification of values
+        newIterable = copy.copy(iterable)
+        if isinstance(iterable, tuple):
+            # cast the immutable tuple type to list allowing modifications, cast
+            # back to tuple afterwards
+            newIterable = list(newIterable)
+            paramDereferentiate(newIterable, paramDict)
+            newIterable = tuple(newIterable)
+        else:
+            paramDereferentiate(newIterable, paramDict)
+        # overwrite former iterable with new copy
+        currentLevel[key] = newIterable
+
+    return currentLevel
+
+
+################################################## paramEvaluate()
+def paramEvaluate(currentLevel, paramDict=None):
+    """Short summary.
+
+    Parameters
+    ----------
+    currentLevel : type
+        Description of parameter `currentLevel`.
+    paramDict : type
+        Description of parameter `paramDict`.
+
+    Returns
+    -------
+    type
+        Description of returned object.
+
+    """
+    '''
+    Evaluate all functions found in currentLevel with paramDict as argument.
+    Repeat the process for nested containers.
+    Returns the modified currentLevel container.
+    '''
+    # set paramDict in first level, determine iterator for currentLevel
+    iterator = currentLevel.items() \
+        if isinstance(currentLevel, dict) else enumerate(currentLevel)
+    if paramDict is None:
+        paramDict = currentLevel
+
+    # STAGE 1: Evaluate the functions found in currentLevel. Also build a
+    #          container list for stage two.
+    dictIterables = {}
+    for key, value in iterator:
+        if isinstance(value, (list, tuple, dict)):
+            if not isinstance(value, IgnoreDict):
+                dictIterables[key] = value
+        elif inspect.isroutine(value):
+            currentLevel[key] = value(paramDict)
+
+    # STAGE 2: Crawl the containers found in stage 1, repeating the process
+    #          The parameter dictionary paramDict stays the same for all levels.
+    for key, iterable in dictIterables.items():
+        if isinstance(iterable, tuple):
+            # cast the immutable tuple type to list allowing modifications, cast
+            # back to tuple afterwards
+            newIterable = list(currentLevel[key])
+            paramEvaluate(newIterable, paramDict)
+            currentLevel[key] = tuple(newIterable)
         else:
-            strDiff = '000'
+            paramEvaluate(currentLevel[key], paramDict)
 
-        strInfo=strInfo + (fmtYellow if ignoreProx else fmtRed)(strDiff)
+    return currentLevel
 
-    return strInfo
 
+################################################## mergeDicts()
+# a little helper to safely merge two dictionaries
+def mergeDicts(a, b):
+    """Short summary.
+
+    Parameters
+    ----------
+    a : type
+        Description of parameter `a`.
+    b : type
+        Description of parameter `b`.
+
+    Returns
+    -------
+    type
+        Description of returned object.
+
+    """
+    '''
+    Merge the dictionaries a and b such that entries in b have priority and the
+    input Dictionary a remains unchanged.
+    '''
+    c = a.copy()
+    c.update(b)
+    return c
 
-################################################## initTest()
-def initTest(test):
-    # generate test object instance for given parameter set
-    test[TEST.INSTANCE] = test[TEST.OBJECT](
-        *test.get(TEST.INITARGS, ()),
-        **test.get(TEST.INITKWARGS, {}))
-
-    if isinstance(test[TEST.INSTANCE], Matrix):
-        # generate plain reference array
-        test[TEST.REFERENCE] = test[TEST.INSTANCE].reference()
-
-
-################################################## testFailDump()
-def testFailDump(test):
-    print("Test query causing the exception:")
-    pprint(test)
-
-
-################################################## testArrays()
-def testArrays(test):
-    query={TEST.RESULT_INPUT      : test[TEST.RESULT_INPUT],
-           TEST.RESULT_OUTPUT     : test[TEST.RESULT_OUTPUT],
-           TEST.RESULT_REF        : test[TEST.RESULT_REF]}
-    return compareResults(test, query)
-
-
-################################################## testForward()
-def testForward(test):
-    query={}
-    arrInput=query[TEST.RESULT_INPUT]=test[TEST.DATAARRAY].forwardData
-    arrInputCheck = arrInput.copy()
-    query[TEST.RESULT_OUTPUT]=test[TEST.INSTANCE].forward(arrInput)
-    if not np.array_equal(arrInput, arrInputCheck):
-        testFailDump(test)
-        raise ValueError(".forward() modified input array.")
-
-    query[TEST.RESULT_REF]=test[TEST.REFERENCE].dot(arrInput)
-    return compareResults(test, query)
-
-
-################################################## testBackward()
-def testBackward(test):
-    query={}
-    arrInput=query[TEST.RESULT_INPUT]=test[TEST.DATAARRAY].backwardData
-    arrInputCheck = arrInput.copy()
-    query[TEST.RESULT_OUTPUT]=test[TEST.INSTANCE].backward(arrInput)
-    if not np.array_equal(arrInput, arrInputCheck):
-        testFailDump(test)
-        raise ValueError(".backward() modified input array.")
-
-    query[TEST.RESULT_REF]=test[TEST.REFERENCE].T.conj().dot(arrInput)
-    return compareResults(test, query)
-
-
-################################################## testArray()
-def testArray(test):
-    query={}
-    instance=test[TEST.INSTANCE]
-    query[TEST.RESULT_OUTPUT]=instance.array
-    query[TEST.RESULT_REF]=test[TEST.REFERENCE].astype(instance.dtype)
-    return compareResults(test, query)
-
-
-################################################## testInterface()
-def testInterface(test):
-    query={}
-    instance=test[TEST.INSTANCE]
-    query[TEST.RESULT_OUTPUT] = (
-        instance - instance + (np.int8(-1) * instance * np.int8(-1)) +
-        instance - instance
-    ).array
-    query[TEST.RESULT_REF]=test[TEST.REFERENCE].astype(instance.dtype)
-    return compareResults(test, query)
-
-
-################################################## testGetItem()
-def testGetItem(test):
-    query={}
-    instance=test[TEST.INSTANCE]
-    arrOutput=np.zeros(instance.shape, instance.dtype)
-    for nn, mm in itertools.product(range(instance.numRows),
-                                    range(instance.numCols)):
-        arrOutput[nn, mm]=instance[nn, mm]
-    query[TEST.RESULT_OUTPUT]=arrOutput
-    query[TEST.RESULT_REF]=test[TEST.REFERENCE].astype(instance.dtype)
-    return compareResults(test, query)
-
-
-################################################## testGetColsSingle()
-def testGetColsSingle(test):
-    query = {}
-    instance = test[TEST.INSTANCE]
-    arrOutput = np.empty(instance.shape, instance.dtype)
-    for mm in range(instance.numCols):
-        vecCol = instance.getCols(mm)
-        if vecCol.ndim != 1:
-            print('testGetColsSingle', vecCol.shape, vecCol)
-            query[TEST.RESULT], query[TEST.RESULT_IGNORED] = False, False
-            query[TEST.RESULT_INFO] = fmtRed('!=(N,)')
-            return query
-
-        arrOutput[:, mm] = vecCol
-
-    query[TEST.RESULT_OUTPUT] = arrOutput
-    query[TEST.RESULT_REF] = test[TEST.REFERENCE].astype(instance.dtype)
-    return compareResults(test, query)
-
-
-################################################## testGetColsMultiple()
-def testGetColsMultiple(test):
-    query={}
-    instance=test[TEST.INSTANCE]
-    arrOutput=instance.getCols([c for c in range(instance.numCols)])
-    query[TEST.RESULT_OUTPUT]=arrOutput
-    query[TEST.RESULT_REF]=test[TEST.REFERENCE].astype(instance.dtype)
-    return compareResults(test, query)
-
-
-################################################## test: getRowsSingle
-def testGetRowsSingle(test):
-    query = {}
-    instance = test[TEST.INSTANCE]
-    arrOutput = np.empty((instance.numRows, instance.numCols), instance.dtype)
-    for nn in range(instance.numRows):
-        vecRow = instance.getRows(nn)
-        import sys
-        if vecRow.ndim != 1:
-            print('testGetRowsSingle', vecRow.shape, vecRow)
-            result, ignored = False, False
-            query[TEST.RESULT], query[TEST.RESULT_IGNORED] = False, False
-            query[TEST.RESULT_INFO] = fmtRed('!=(N,)')
-            return query
-
-        arrOutput[nn, :] = vecRow
-
-    query[TEST.RESULT_OUTPUT] = arrOutput
-    query[TEST.RESULT_REF] = test[TEST.REFERENCE].astype(instance.dtype)
-    return compareResults(test, query)
-
-
-################################################## test: getRowsMultiple
-def testGetRowsMultiple(test):
-    query={}
-    instance=test[TEST.INSTANCE]
-    arrOutput=instance.getRows([r for r in range(instance.numRows)])
-    query[TEST.RESULT_OUTPUT]=arrOutput
-    query[TEST.RESULT_REF]=test[TEST.REFERENCE].astype(instance.dtype)
-    return compareResults(test, query)
-
-
-################################################## test: column,rowNorms
-###                                            ### test: column,rowNormalized
-def _testNorms(test, funcTestcase, expectedType):
-    instance, reference = test[TEST.INSTANCE], test[TEST.REFERENCE]
-
-    # usually expect the normalized matrix to be promoted in type complexity
-    # due to division by column-norm during the process. However there exist
-    # matrices that treat the problem differently. Exclude the expected pro-
-    # motion for them.
-    query=({} if isinstance(instance, (Diag, Eye, Zero))
-           else {TEST.TYPE_EXPECTED: expectedType})
-
-    # ignore actual type of generated gram:
-    query[TEST.CHECK_DATATYPE] = False
-    query[TEST.TOL_MINEPS] = getTypeEps(safeTypeExpansion(instance.dtype))
-
-    try:
-        funcTestcase(query, instance, reference)
-        return compareResults(test, query)
-    except ValueError:
-        if isinstance(instance, Zero):
-            # failing normalization is expected for Zero matrix.
-            result, ignored=True, False
-        elif isinstance(instance, Parametric):
-            # Parametric normalization is excused for now (int8 trouble)
-            result, ignored=False, True
+################################################################################
+################################################## array generators, test distr.
+
+
+################################################## arrTestDist()
+def arrTestDist(shape, dtype, center=0):
+    """Short summary.
+
+    Parameters
+    ----------
+    shape : type
+        Description of parameter `shape`.
+    dtype : type
+        Description of parameter `dtype`.
+    center : type
+        Description of parameter `center`.
+
+    Returns
+    -------
+    type
+        Description of returned object.
+
+    """
+    def _draw(shape):
+        '''
+        Draw a random floating-point number from a test distribution.
+        Remove the part around zero from the distribution and keep the distance
+        between minimal and maximal absolute values (dynamics) relatively small
+        '''
+        return (np.random.uniform(2., 1., size=shape) *
+                np.random.choice([-1, 1], shape))
+
+    if np.prod(shape) < 1:
+        return np.array([])
+
+    if dtype in (np.int8, np.uint8, np.int16, np.uint16,
+                 np.int32, np.uint32, np.int64, np.uint64):
+        result = np.random.choice(
+            [center - 2, center - 1, center + 1, center + 2], shape).astype(
+                dtype)
+    else:
+        if dtype in (np.float32, np.float64):
+            result = _draw(shape).astype(dtype) + center
+        elif dtype in (np.complex64, np.complex128):
+            result = (_draw(shape) + np.real(center) +
+                      1j * (_draw(shape) + np.imag(center))).astype(dtype)
         else:
-            result, ignored=False, False
+            raise TypeError("arrTestDist: unsupported type %s" % (dtype))
+
+    # increase the largest element in magnitude a little bit more to avoid
+    # too close neighbours to the largest element in the distribution
+    # this helps at least largestSingularValue in Diag matrices to converge ;)
+    idxMax = np.unravel_index(np.abs(result).argmax(), result.shape)
+    if isInteger(dtype):
+        result[idxMax] += np.sign(result[idxMax])
+    else:
+        result[idxMax] *= 1.5
 
-        query[TEST.RESULT], query[TEST.RESULT_IGNORED] = result, ignored
-        query[TEST.RESULT_INFO] = '!RNK'
-        return query
-
-
-def testcolNorms(test):
-    def columnTestcase(query, instance, reference):
-        query[TEST.RESULT_OUTPUT] = instance.colNorms
-        query[TEST.RESULT_REF] = np.apply_along_axis(
-            np.linalg.norm, 0, reference
-        )
-
-    return _testNorms(test, columnTestcase, np.float64)
-
-
-def testRowNorms(test):
-    def rowTestcase(query, instance, reference):
-        query[TEST.RESULT_OUTPUT] = instance.rowNorms
-        query[TEST.RESULT_REF] = np.apply_along_axis(
-            np.linalg.norm, 1, reference
-        )
-
-    return _testNorms(test, rowTestcase, np.float64)
-
-
-def testcolNormsColNormalized(test):
-    def columnTestcase(query, instance, reference):
-        query[TEST.RESULT_OUTPUT] = instance.colNormalized.array
-        query[TEST.RESULT_REF] = np.einsum(
-            'ij,j->ij',
-            reference,
-            1. / np.apply_along_axis(np.linalg.norm, 0, reference))
-
-    return _testNorms(test, columnTestcase,
-                      np.promote_types(test[TEST.INSTANCE].dtype, np.float64))
-
-
-def testRowNormalized(test):
-    def rowTestcase(query, instance, reference):
-        query[TEST.RESULT_OUTPUT] = instance.rowNormalized.array
-        query[TEST.RESULT_REF] = np.einsum(
-            'i,ij->ij',
-            1. / np.apply_along_axis(np.linalg.norm, 1, reference),
-            reference)
-
-    return _testNorms(test, rowTestcase,
-                      np.promote_types(test[TEST.INSTANCE].dtype, np.float64))
-
-
-################################################## test: largestSV (property)
-def testLargestSV(test):
-    query={TEST.TYPE_EXPECTED: np.float64}
-    instance=test[TEST.INSTANCE]
-
-    # account for "extra computation stage" (gram) in largestSingularValue
-    query[TEST.TOL_POWER] = test.get(TEST.TOL_POWER, 1.) * 2
-    query[TEST.TOL_MINEPS] = getTypeEps(safeTypeExpansion(instance.dtype))
-
-    # determine reference result
-    largestSingularValue = np.linalg.svd(
-        test[TEST.REFERENCE],
-        compute_uv=False
-    )[0]
-
-    query[TEST.RESULT_REF] = np.array(
-        largestSingularValue,
-        dtype=np.promote_types(largestSingularValue.dtype, np.float32)
-    )
-
-    # largestSingularValue may not converge fast enough
-    # for a bad random starting point
-    # so retry some times before throwing up
-    for tries in range(9):
-        maxSteps=100. * 10. ** (tries / 2.)
-        query[TEST.RESULT_OUTPUT]=np.array(
-            instance.getLargestSingularValue())
-        result=compareResults(test, query)
-        if result[TEST.RESULT]:
-            break
     return result
 
+################################################## arrSparseTestDist()
 
-################################################## test: gram (property)
-def testGram(test):
-    instance, reference=test[TEST.INSTANCE], test[TEST.REFERENCE]
-
-    # usually expect the normalized matrix to be promoted in type complexity
-    # due to division by column-norm during the process. However there exist
-    # matrices that treat the problem differently. Exclude the expected pro-
-    # motion for them.
-    query=({} if isinstance(instance, (Diag, Eye, Zero))
-           else {TEST.TYPE_PROMOTION: np.float32})
-
-    # account for "extra computation stage" in gram
-    query[TEST.TOL_POWER]=test.get(TEST.TOL_POWER, 1.) * 2
-
-    query[TEST.RESULT_OUTPUT]=instance.gram.array
-    query[TEST.RESULT_REF]=reference.astype(
-        np.promote_types(np.float32, reference.dtype)).T.conj().dot(reference)
-
-    # ignore actual type of generated gram:
-    query[TEST.CHECK_DATATYPE]=False
-
-    return compareResults(test, query)
-
-
-################################################## test: T (property)
-def testTranspose(test):
-    query={}
-    instance=test[TEST.INSTANCE]
-    query[TEST.RESULT_OUTPUT]=instance.T.array
-    query[TEST.RESULT_REF]=test[TEST.REFERENCE].T
-    return compareResults(test, query)
-
-
-################################################## test: H (property)
-def testHermitian(test):
-    query={}
-    instance=test[TEST.INSTANCE]
-    query[TEST.RESULT_OUTPUT]=instance.H.array
-    query[TEST.RESULT_REF]=test[TEST.REFERENCE].T.conj()
-    return compareResults(test, query)
-
-
-################################################## test: conj (property)
-def testConjugate(test):
-    query={}
-    instance=test[TEST.INSTANCE]
-    query[TEST.RESULT_OUTPUT]=instance.conj.array
-    query[TEST.RESULT_REF]=test[TEST.REFERENCE].conj()
-    return compareResults(test, query)
-
-
-################################################## test: Algorithm
-def testAlgorithm(test):
-    # generate input data vector. As this one is needed for some algs, do one
-    # dereferentiation step on a complete dictionary, including test and result
-    query=test.copy()
-    arrInput, query[TEST.RESULT_INPUT]=query[TEST.DATAARRAY].forwardData
-    paramDereferentiate(query)
-
-    # now call the algorithm executor functions for FUT and reference
-    arrInputCheck = arrInput.copy()
-    query[TEST.RESULT_OUTPUT]=query[TEST.ALG](
-        *query.get(TEST.ALG_ARGS, ()),
-        **query.get(TEST.ALG_KWARGS, {}))
-    query[TEST.RESULT_REF]=query[TEST.REFALG](
-        *query.get(TEST.REFALG_ARGS,      query.get(TEST.ALG_ARGS, [])),
-        **query.get(TEST.REFALG_KWARGS,   query.get(TEST.ALG_KWARGS, {})))
-
-    if not np.array_equal(arrInput, arrInputCheck):
-        testFailDump(test)
-        raise ValueError("Algorithm modified input array.")
 
-    return compareResults(test, query)
+def arrSparseTestDist(shape, dtype,
+                      density=0.1, center=0, compactFullyOccupied=False):
+    """Short summary.
+
+    Parameters
+    ----------
+    shape : type
+        Description of parameter `shape`.
+    dtype : type
+        Description of parameter `dtype`.
+    density : type
+        Description of parameter `density`.
+    center : type
+        Description of parameter `center`.
+    compactFullyOccupied : type
+        Description of parameter `compactFullyOccupied`.
+
+    Returns
+    -------
+    type
+        Description of returned object.
+
+    """
+    numSize = np.prod(shape)
+    if compactFullyOccupied:
+        # draw just enough samples randomly such that every row and column is
+        # occupied with at least one element. Ignore the density parameter
+        numElements = max(shape)
+
+        # draw mm and nn coordinates from coordinate space. Modulo operation
+        # wraps indices larger than the actual row or column dimension
+        suppX = np.mod(
+            np.random.choice(numElements, numElements, replace=False), shape[0])
+        suppY = np.mod(
+            np.random.choice(numElements, numElements, replace=False), shape[1])
+    else:
+        # draw a relative amount of samples randomly over vectorized index space
+        numElements = int(numSize * density)
+        supp = np.random.choice(np.arange(numSize), numElements, replace=False)
+        suppX = np.mod(supp, shape[0])
+        suppY = np.divide(supp, shape[0])
+
+    # determine the actual element values distributed over the sparse array
+    # from arrTestDist with a 1D-array spanning the required element count
+    arrElements = arrTestDist((numElements, ), dtype, center=center)
+
+    return sparse.coo_matrix(
+        (arrElements, (suppX, suppY)), shape=shape, dtype=dtype)
+
+
+################################################## arrAlign()
+def arrAlign(arr, alignment=ALIGNMENT.DONTCARE):
+    """Short summary.
+
+    Parameters
+    ----------
+    arr : type
+        Description of parameter `arr`.
+    alignment : type
+        Description of parameter `alignment`.
+
+    Returns
+    -------
+    type
+        Description of returned object.
+
+    """
+    if alignment == ALIGNMENT.DONTCARE:
+        return np.asanyarray(arr)
+    elif alignment == ALIGNMENT.FCONT:
+        return np.asfortranarray(arr)
+    elif alignment == ALIGNMENT.CCONT:
+        return np.ascontiguousarray(arr)
+    elif alignment == ALIGNMENT.STRIDE:
+        # define spacing between elements
+        spacing = 3
+        # determine maximum value
+        try:
+            maxValue = np.iinfo(arr.dtype).max
+        except ValueError:
+            try:
+                maxValue = np.finfo(arr.dtype).max
+            except ValueError:
+                maxValue = 1.
+
+        # generate large random array with maximized data type utilization
+        arrFill = (maxValue * (np.random.rand(
+            *(dim * spacing for dim in arr.shape)) - 0.5)).astype(arr.dtype)
+
+        # fill-in the array data and return a view of the to-be-aligned array
+        arrPart = arrFill[(np.s_[1::spacing], ) * arrFill.ndim]
+        arrPart[:] = arr
+        return arrPart
+    else:
+        raise ValueError("Unknown alignment identificator '%s'" %(alignment))
 
 
+################################################## arrayGenerator
+class ArrayGenerator(dict):
+
+    @property
+    def forwardData(self):
+        if NAME.FWDATA not in self:
+            # generate random array and set specific alignment style
+            self[NAME.FWDATA] = arrAlign(
+                arrTestDist(self[NAME.SHAPE], self[NAME.DTYPE],
+                            center=self.get(NAME.CENTER, 0)),
+                alignment=self.get(NAME.ALIGN, ALIGNMENT.DONTCARE))
+
+        return self[NAME.FWDATA]
+
+    @property
+    def backwardData(self):
+        if NAME.BWDATA not in self:
+            # generate random array and set specific alignment style
+            self[NAME.BWDATA] = arrAlign(
+                arrTestDist(self[NAME.SHAPE_T], self[NAME.DTYPE],
+                            center=self.get(NAME.CENTER, 0)),
+                alignment=self.get(NAME.ALIGN, ALIGNMENT.DONTCARE))
+
+        return self[NAME.BWDATA]
+
+    def __call__(self):
+        return self.forwardData
+
+    def __str__(self):
+        '''Compose a compact description of the represented array.'''
+        tags = []
+
+        # generate shape-token: check for both shape variants (fw and bw).
+        # if they differ, print both as "fw/bw", otherwise print the dim only
+        fwShape = self[NAME.SHAPE] if NAME.SHAPE in self else ()
+        bwShape = self[NAME.SHAPE_T] if NAME.SHAPE_T in self else ()
+
+        def printDim(fw, bw):
+            if fw is None:
+                return '-' if bw is None else str(bw)
+            else:
+                return (str(fw) if bw is None
+                        else "%s/%s" %(fw, bw) if (fw != bw) else str(fw))
+
+        strShape = 'x'.join([
+            printDim(fw, bw)
+            for fw, bw in six.moves.zip_longest(fwShape, bwShape)])
+        if len(strShape) > 0:
+            tags.append(strShape)
+
+        # print the data type of the array
+        value = self.get(NAME.DTYPE, '')
+        if isinstance(value, type):
+            tags.append(NAME.TYPENAME.get(value, str(value)))
+
+        value = self.get(NAME.ALIGN, None)
+        if value in NAME.ALLALIGNMENTS:
+            tags.append(value)
+
+        return str("[%s]" % (','.join(tags)))
+
+    def __repr__(self):
+        return self.__str__()
+
 ################################################################################
-################################################## class TestRunner
-class Test(Worker):
+################################################## inspection routines
 
-    _verboseFull=False
 
-    def __init__(self, targetClass, **options):
+def showContent(instance, seen=None, prefix=""):
+    """Short summary.
 
-        # extract options
-        extraOptions = options.get('extraOptions',  {})
+    Parameters
+    ----------
+    instance : type
+        Description of parameter `instance`.
+    seen : type
+        Description of parameter `seen`.
+    prefix : type
+        Description of parameter `prefix`.
+
+    Returns
+    -------
+    type
+        Description of returned object.
+
+    """
+    '''
+    Print a readable dependency tree of fastmat class instances
+
+    Parameters
+    ----------
+    instance : :py:class:`fastmat.Matrix`
+        Matrix instance to get inspected
+
+    Notes
+    -----
+    The function outputs instance as top-level node and then walks through all
+    elements of instance.content, recursively calling itself with extended
+    prefix. To avoid endless loops, the function ensures the recursion is only
+    applied once to every element by keeping track already visited elements.
+
+    >>> showContent(Eye(4) * -1 * -1 + Eye(4) - Eye(4))
+    <Sum[4x4]:0x7fe447f40770>
+    +-<Product[4x4]:0x7fe447f3d188>
+    | +-<Eye[4x4]:0x7fe447f402b0>
+    +-<Eye[4x4]:0x7fe447f403e0>
+    +-<Product[4x4]:0x7fe447f3da10>
+      +-<Eye[4x4]:0x7fe447f40640>
+    '''
+    if seen is None:
+        seen = set([])
+
+    print((prefix[:-2] + "+-" if len(prefix) > 0 else "") + repr(instance))
+    if instance not in seen:
+        seen.add(instance)
+        last = len(instance)
+        for ii, item in enumerate(instance):
+            showContent(item, seen=seen,
+                        prefix=prefix + ("| " if ii < last - 1 else "  "))
 
-        # by default, enable verbosity for issues and isolate problems
-        self.cbStatus=self.printStatus
-        self.cbResult=self.findProblems
-
-        # initialize output collectors
-        self.problems = AccessDict({})
-        self.irregularities = AccessDict({})
-
-        # define test-specific defaults
-        defaults={
-            TEST.COMMON: {
-                NAME.NAME       : dynFormat("%s.%s", NAME.CLASS, NAME.TARGET),
-                TEST.NAMINGARGS : dynFormat(
-                    "[%dx%d]", TEST.NUM_ROWS, TEST.NUM_COLS
-                ),
-                TEST.NAMING     : dynFormat(
-                    "%s(%s)", NAME.CLASS, TEST.NAMINGARGS)
-
-            }, TEST.CLASS: {
-                # define tests
-                TEST.QUERY: IgnoreDict({
-                    'arr'   : testArray,
-                    'iface' : testInterface,
-                    'item'  : testGetItem,
-                    'gCs'   : testGetColsSingle,
-                    'gCm'   : testGetColsMultiple,
-                    'gRs'   : testGetRowsSingle,
-                    'gRm'   : testGetRowsMultiple,
-                    'CnVec' : testcolNorms,
-                    'RnVec' : testRowNorms,
-                    'CnMat' : testcolNormsColNormalized,
-                    'RnMat' : testRowNormalized,
-                    'lSV'   : testLargestSV,
-                    'gram'  : testGram,
-                    'T'     : testTranspose,
-                    'H'     : testHermitian,
-                    'conj'  : testConjugate
-                })
-
-            }, TEST.TRANSFORMS: {
-                # define default naming and captions
-                TEST.NAMING     : dynFormat(
-                    "%s(%s)*%s", NAME.CLASS, TEST.NAMINGARGS, TEST.DATAARRAY),
-
-                # define default arrB ArrayGenerator
-                TEST.DATACOLS   : Permutation([1, 5]),
-                TEST.DATATYPE   : VariantPermutation(TEST.ALLTYPES),
-                TEST.DATASHAPE  : (TEST.NUM_COLS, TEST.DATACOLS),
-                TEST.DATASHAPE_T: (TEST.NUM_ROWS, TEST.DATACOLS),
-                TEST.DATAALIGN  : VariantPermutation(TEST.ALLALIGNMENTS),
-                TEST.DATACENTER : 0,
-                TEST.DATAARRAY  : ArrayGenerator({
-                    NAME.DTYPE      : TEST.DATATYPE,
-                    NAME.SHAPE      : TEST.DATASHAPE,
-                    NAME.SHAPE_T    : TEST.DATASHAPE_T,
-                    NAME.ALIGN      : TEST.DATAALIGN,
-                    NAME.CENTER     : TEST.DATACENTER
-                }),
-
-                # define tests
-                TEST.QUERY      : IgnoreDict({
-                    'F'     : testForward,
-                    'B'     : testBackward,
-                })
-
-            }, TEST.ALGORITHM: {
-                # define default naming and captions
-                TEST.TOL_POWER  : 1.,
-                TEST.NAMING     : dynFormat(
-                    "%s(%s)*%s", NAME.CLASS, TEST.NAMINGARGS, TEST.DATAARRAY),
-
-                # define default arrB ArrayGenerator
-                TEST.DATACOLS   : Permutation([1, 5]),
-                TEST.DATATYPE   : VariantPermutation(TEST.LARGETYPES),
-                TEST.DATASHAPE  : (TEST.NUM_COLS, TEST.DATACOLS),
-                TEST.DATASHAPE_T: (TEST.NUM_ROWS, TEST.DATACOLS),
-                TEST.DATAALIGN  : VariantPermutation(TEST.ALLALIGNMENTS),
-                TEST.DATACENTER : 0,
-                TEST.DATAARRAY  : ArrayGenerator({
-                    NAME.DTYPE      : TEST.DATATYPE,
-                    NAME.SHAPE      : TEST.DATASHAPE,
-                    NAME.SHAPE_T    : TEST.DATASHAPE_T,
-                    NAME.ALIGN      : TEST.DATAALIGN,
-                    NAME.CENTER     : TEST.DATACENTER
-                }),
-
-                # define tests
-                TEST.QUERY: IgnoreDict({
-                    'arr'     : testArrays
-                })
-
-            }
-        }
-
-        # call parent initialization with Test-specific options
-        super(Test, self).__init__(
-            targetClass, targetOptionMethod='_getTest',
-            runnerDefaults=defaults, extraOptions=extraOptions)
-
-    def _runTest(self, name, options):
-
-        # build list of tests as complete permutation of parameter variations
-        tests=uniqueNameDict({})
-        lstTests=paramPermute(options)
-        for test in lstTests:
-            # prepare test dictionary (dereferentiate links, evaluate functions)
-            paramDereferentiate(test)
-            paramEvaluate(test)
-
-            # name each test instance from the key naming rule option ('naming')
-            # 'naming' is a format string, which selects its fields from the
-            # option dictionary made up by the target dictionary itself.
-            tests[getattr(test, TEST.NAMING, test[NAME.TARGET])]=test
-
-            # sanity-check proper definition of test target
-            obj=test.get(TEST.OBJECT, None)
-            if (obj is None or
-                    not issubclass(obj, (Matrix, Algorithm))):
-                raise ValueError("%s['%s'] not a fastmat class or test case." %(
-                    test.name, TEST.OBJECT))
-
-        # When done, convert tests back to regular dictionary, enabling editing
-        tests=dict(tests)
-
-        # allow a second level of Permutation for VariantPermutation instances
-        # determine variants of target and generate variant description tag name
-        lstVariantPermutations=[name for name, value in options.items()
-                                if isinstance(value, VariantPermutation)]
-        descrVariants=','.join(lstVariantPermutations)
-
-        # determine field lengths for nice printing of columns
-        lenName=max(map(len, tests.keys()))
-
-        # self.results is constructed as multi-level dictionary:
-        #     ~[target-name][test-name][variant-name][query-name]: results dict
-        # initialize result structure for [test-name] level
-        # create the [variant-level] dictionary as uniqueNameDict to prevent
-        # overwriting existing variant results with the same name
-        resultTarget={name: uniqueNameDict({}) for name in tests.keys()}
-
-        # iterate through tests
-        for nameTest, test in sorted(tests.items()):
-            # initialize instances and required stuff for each test
-            tryQuery(nameTest, initTest, test)
-
-            # get a pointer to the test result dictionary
-            resultTest=resultTarget[nameTest]
-
-            lstVariants=paramPermute(
-                test, PermutationClass=VariantPermutation)
-            variants=[paramDereferentiate(variant) for variant in lstVariants]
-            for variant in variants:
-                variant[NAME.VARIANT]=''.join(
-                    [NAME.TYPENAME[variant[key]]
-                     if isinstance(variant[key], type)
-                     else str(variant[key])
-                     for key in lstVariantPermutations])
-
-                # call variant initialization routine, if defined
-                if TEST.INIT_VARIANT in variant:
-                    variant[TEST.INIT_VARIANT](variant)
-
-                # execute test queries, collect results as [query-name] level
-                # and store in [variant-name] level into test result structure.
-                resultTest[variant[NAME.VARIANT]]={
-                    name: tryQuery(nameTest, query, variant)
-                    for name, query in test[TEST.QUERY].items()
-                }
-
-            self.emitStatus(nameTest, resultTest, lenName, descrVariants)
-
-        return resultTarget
-
-    def _run(self, name, options):
-
-        maxTries = 3
-        for numTry in range(maxTries):
-            resultTarget = self._runTest(name, options.copy())
-
-            result = all(all(all(resultQuery[TEST.RESULT] or
-                                 resultQuery[TEST.RESULT_IGNORED]
-                                 for resultQuery in resultVariant.values())
-                             for resultVariant in resultTest.values())
-                         for resultTest in resultTarget.values())
+################################################################################
+################################################## CONSTANT definitions
 
-            if result:
-                break
-            else:
-                print("Test %s.%s failed in during try #%d/%d.%s" %(
-                    options[NAME.CLASS], name, numTry + 1, maxTries,
-                    " Retrying ..." if numTry < maxTries - 1 else ""))
-
-        return resultTarget
-
-    def printStatus(self, nameTest, resultTest, lenName=-1, descrVariants=""):
-        # if full output isn't actually requested, crawl all query results in
-        # the hierarchy of this test for negative results. If none are found,
-        # skip printing.
-        if not self._verboseFull:
-            if all(all((query.get(TEST.RESULT, True) or
-                        query.get(TEST.IGNORE, False))
-                       for query in variant.values())
-                   for variant in resultTest.values()):
-                return
-
-        lenNameV=max(len(nameV) for nameV in resultTest.keys())
-        if lenName < 1:
-            lenName=len(nameTest)
-
-        # construct named prefix describing the test and its following variants
-        strPrefix="%-*s " %(lenName + len(descrVariants),
-                            nameTest + ":" + descrVariants)
-
-        # convert results to info strings
-        strQueries={nameV: ["%s:%s" %(nameQ, formatResult(query))
-                            for nameQ, query in sorted(variant.items())]
-                    for nameV, variant in resultTest.items()}
-
-        # determine print-lengths of query strings
-        lenQueries={nameV: [len(fmtEscape(strQuery)) for strQuery in variant]
-                    for nameV, variant in strQueries.items()}
-
-        # determine highest print-length for any query
-        maxLenQuery=max(max(variant) for variant in lenQueries.values())
-
-        # normalize string lengths in strQueries
-        for nameV, lengths in lenQueries.items():
-            strQueries[nameV]=["%s%s" %(strQueries[nameV][qq],
-                                        " " * (maxLenQuery - lenQuery))
-                               for qq, lenQuery in enumerate(lengths)]
-
-        # join query strings to form variant strings
-        strVariants=["%*s %s" %(lenNameV, nameV, " ".join(lstStr))
-                     for nameV, lstStr in sorted(strQueries.items())]
-
-        lenVariants=[len(fmtEscape(strV)) for strV in strVariants]
-        maxLenVariants=max(lenVariants)
-
-        # normalize string lengths in strVariants
-        strVariants=["%s%s" %(strV, " " * (maxLenVariants - lenVariants[vv]))
-                     for vv, strV in enumerate(strVariants)]
-        lenVariants=(0 if len(strVariants) == 0
-                     else len(fmtEscape(strVariants[0])))
-
-        # calculate amount of entries printable per line
-        width=self.consoleWidth
-        itemsPerLine=(
-            1 if width < 0
-            else max(1, ((width - len(strPrefix)) // (1 + lenVariants))))
-
-        for ii in range(0, len(strVariants), itemsPerLine):
-            print("%s|%s" %(strPrefix if ii == 0 else " " * len(strPrefix),
-                            " |".join(strVariants[ii: ii + itemsPerLine])))
 
-    # control verbosity of _run() and printStatus()
-    @property
-    def verbosity(self):
-        return self.cbStatus == self.printStatus, self._verboseFull
+################################################## class TypeDict
+class TypeDict(dict):
+    def __getitem__(self, key):
+        if key not in self:
+            key = key.type if isinstance(key, np.dtype) else None
+        return dict(self).get(key, '???')
+
+
+class COLOR():
+    '''Give escape format strings (color, face) a name.'''
+    END    = "\033[0m"
+    BOLD   = "\033[1m"
+    LINE   = "\033[4m"
+    RED    = "\033[91m"
+    GREEN  = "\033[92m"
+    YELLOW = "\033[93m"
+    BLUE   = "\033[94m"
+    PURPLE = "\033[95m"
+    AQUA   = "\033[96m"
+
+
+def fmtStr(string, color):
+    """Short summary.
+
+    Parameters
+    ----------
+    string : type
+        Description of parameter `string`.
+    color : type
+        Description of parameter `color`.
+
+    Returns
+    -------
+    type
+        Description of returned object.
+
+    """
+    '''Print a string quoted by some format specifiers.'''
+    # colored output only supported with linux
+    return ("%s%s%s" %(color, string, COLOR.END)
+            if currentOS == 'Linux'
+            else string)
+
+
+def fmtGreen(string):
+    """Short summary.
 
-    @verbosity.setter
-    def verbosity(self, value):
-        if isinstance(value, bool):
-            value=(value, )
-
-        if isinstance(value, tuple):
-            if len(value) >= 1:
-                self.cbStatus=(self.printStatus if value[0] is True
-                               else None)
-            if len(value) >= 2:
-                self._verboseFull=value[1]
-
-    def findProblems(self, nameTarget, targetResult):
-        # crawl all query results for problems and irregularities. Collect them
-        # if found. Also, construct a considerable name.
-        problems={}
-        irregularities={}
-        for nameT, test in sorted(targetResult.items()):
-            for nameV, variant in sorted(test.items()):
-                for nameQ, query in sorted(variant.items()):
-                    if not query.get(TEST.RESULT, False):
-                        nameTestQuery="%s%s.%s" %(nameT, nameV, nameQ)
-                        if query.get(TEST.RESULT_IGNORED, False):
-                            irregularities[nameTestQuery]=query
-                        else:
-                            problems[nameTestQuery]=query
+    Parameters
+    ----------
+    string : type
+        Description of parameter `string`.
 
-        self.problems[nameTarget] = convertToAccessDicts(problems)
-        self.irregularities[nameTarget] = convertToAccessDicts(irregularities)
+    Returns
+    -------
+    type
+        Description of returned object.
+
+    """
+    '''Print string in green.'''
+    return fmtStr(string, COLOR.GREEN)
+
+
+def fmtRed(string):
+    """Short summary.
+
+    Parameters
+    ----------
+    string : type
+        Description of parameter `string`.
+
+    Returns
+    -------
+    type
+        Description of returned object.
+
+    """
+    '''Print string in red.'''
+    return fmtStr(string, COLOR.RED)
+
+
+def fmtYellow(string):
+    """Short summary.
+
+    Parameters
+    ----------
+    string : type
+        Description of parameter `string`.
+
+    Returns
+    -------
+    type
+        Description of returned object.
+
+    """
+    '''Print string in yellow.'''
+    return fmtStr(string, COLOR.YELLOW)
+
+
+def fmtBold(string):
+    """Short summary.
+
+    Parameters
+    ----------
+    string : type
+        Description of parameter `string`.
+
+    Returns
+    -------
+    type
+        Description of returned object.
+
+    """
+    '''Print string in bold face.'''
+    return fmtStr(string, COLOR.BOLD)
+
+
+reAnsiEscape = None
+
+
+def fmtEscape(string):
+    """Short summary.
+
+    Parameters
+    ----------
+    string : type
+        Description of parameter `string`.
+
+    Returns
+    -------
+    type
+        Description of returned object.
+
+    """
+    '''Return a string with all ASCII escape sequences removed.'''
+    global reAnsiEscape
+    if reAnsiEscape is None:
+        reAnsiEscape = re.compile(r'\x1b[^m]*m')
+
+    return reAnsiEscape.sub('', string)
+
+
+def dynFormat(s, *keys):
+    """Short summary.
+
+    Parameters
+    ----------
+    s : type
+        Description of parameter `s`.
+    *keys : type
+        Description of parameter `*keys`.
+
+    Returns
+    -------
+    type
+        Description of returned object.
+
+    """
+    return s.replace('%', '%%(%s)') % keys
+
+
+################################################## getConsoleSize()
+
+fallbackConsoleSize = (80, 25)
+if (currentOS in ['Linux', 'Darwin']) or currentOS.startswith('CYGWIN'):
+    import fcntl
+    import termios
+    # source: https://gist.github.com/jtriley/1108174
+
+    def getConsoleSize():
+        def ioctl_GWINSZ(fd):
+            try:
+                return struct.unpack(
+                    'hh', fcntl.ioctl(fd, termios.TIOCGWINSZ, '1234'))
+            except EnvironmentError:
+                return None
+
+        cr = ioctl_GWINSZ(0) or ioctl_GWINSZ(1) or ioctl_GWINSZ(2)
+        if not cr:
+            try:
+                fd = os.open(os.ctermid(), os.O_RDONLY)
+                cr = ioctl_GWINSZ(fd)
+                os.close(fd)
+            except EnvironmentError:
+                pass
+
+        if not cr:
+            try:
+                cr = (os.environ['LINES'], os.environ['COLUMNS'])
+            except (EnvironmentError, KeyError):
+                cr = fallbackConsoleSize
+
+        return int(cr[0]), int(cr[1])
+elif currentOS == 'Windows':
+    def getConsoleSize():
+        cr = fallbackConsoleSize
+        try:
+            from ctypes import windll, create_string_buffer
+            # stdin handle is -10
+            # stdout handle is -11
+            # stderr handle is -12
+            h = windll.kernel32.GetStdHandle(-12)
+            csbi = create_string_buffer(22)
+            res = windll.kernel32.GetConsoleScreenBufferInfo(h, csbi)
+            if res:
+                (left, top, right, bottom) = struct.unpack("10x4h4x", csbi.raw)
+                cr = (right - left, bottom - top)
+        except (ImportError, EnvironmentError):
+            pass
+
+        return cr
+else:
+    def getConsoleSize():
+        return fallbackConsoleSize
+
+
+################################################## worker's CONSTANT classes
+class NAME(object):
+    DATA            = 'data'
+    FWDATA          = 'dataForward'
+    BWDATA          = 'dataBackward'
+    DTYPE           = 'dtype'
+    SHAPE           = 'shape'
+    SHAPE_T         = 'shapeBackward'
+    ALIGN           = 'align'
+    CENTER          = 'center'
+    FORMAT          = 'format'
+    NAME            = 'name'
+
+    CLASS           = 'class'
+    TARGET          = 'target'
+    FILENAME        = 'filename'
+    CAPTION         = 'caption'
+    BENCHMARK       = 'bench'
+    DOCU            = 'docu'
+    TEST            = 'test'
+    COMMON          = 'common'
+    TEMPLATE        = 'template'
+    VARIANT         = 'variant'
+    RESULT          = 'result'
+    HEADER          = 'header'
+
+    TYPENAME        = TypeDict({
+        np.int8:       'i08', np.int16:      'i16', np.int32:      'i32',
+        np.int64:      'i64', np.float32:    'f32', np.float64:    'f64',
+        np.complex64:  'c32', np.complex128: 'c64', None:          '???'
+    })
+
+    ALLTYPES        = [np.int8, np.int16, np.int32, np.int64,
+                       np.float32, np.float64,
+                       np.complex64, np.complex128]
+    FEWTYPES        = [np.int32, np.float32, np.complex64]
+
+    SINGLETYPES     = [np.int32, np.int16, np.float32, np.complex64]
+    DOUBLETYPES     = [np.int64, np.float64, np.complex128]
+
+    INTTYPES        = [np.int8, np.int16, np.int32, np.int64]
+    FLOATTYPES      = [np.float32, np.float64]
+    COMPLEXTYPES    = [np.complex64, np.complex128]
+
+    LARGETYPES      = [np.int32, np.int64, np.float32, np.float64,
+                       np.complex64, np.complex128]
+
+    ALLALIGNMENTS   = [ALIGNMENT.FCONT, ALIGNMENT.CCONT, ALIGNMENT.STRIDE]
+
+    # repeat some of the definitions in this unit to allow compact imports
+    ALIGNMENT       = ALIGNMENT
+    ArrayGenerator  = ArrayGenerator
+    Permutation     = Permutation
+    IgnoreFunc      = IgnoreFunc
+
+
+################################################################################
+################################################## class Runner
+class Worker(object):
+    """Short summary."""
+    '''
+    options - dictionary structure containing options for multiple targets.
+    {   'nameOfTarget': {'parameter': 123,
+    'anotherParameter': 456
+    }, NAME.DEFAULTS:  {'parameter': default parameter unless overwritten
+    within the selected target
+    }}
+
+    results - output of each target's as specified in options
+    '''
+
+    cbStatus=None
+    cbResult=None
+    target=None
+
+    def __init__(self, targetClass, **options):
+        """Short summary.
 
-        return self.problems[nameTarget]
+        Parameters
+        ----------
+        targetClass : type
+            Description of parameter `targetClass`.
+        **options : type
+            Description of parameter `**options`.
+
+        Returns
+        -------
+        type
+            Description of returned object.
+
+        """
+        '''
+        Setup an inspection environment on a fastmat class specified in target.
+        Along the way an empty instance of target will be created and aside
+        the default options, which may be specified in runnerDefaults, an
+        arbitrarily named method of target may be specified to return more
+        specific options when called.
+        extraOptions may be specified to overwrite any parameter with highest
+        priority.
+        Both extraOptions and runnerDefaults must be specified as a two-level
+        dictionary with the outer level specifying target names as keys and the
+        inner level the actual parameter for the target.
+        '''
+        # the test target is a fastmat class to be instantiated in the runners
+        if not inspect.isclass(targetClass):
+            raise ValueError("target in init of Runner must be a class type")
+
+        # set defaults for options
+        targetOptionMethod = options.get('targetOptionMethod', None)
+        runnerDefaults = options.get('runnerDefaults', {})
+        extraOptions = options.get('extraOptions', {})
+
+        self.target=targetClass.__new__(targetClass)
+
+        # targetOptionMethod specifies a method name of target which will
+        # return a dictionary with class-specific options if called. If this
+        # functionality is not needed, targetOptionsMethod or runnerDefaults
+        # may be left to their default values.
+        targetOptionMethod=getattr(self.target, targetOptionMethod, None)
+        options={name: mergeDicts(target, extraOptions)
+                 for name, target in ({} if targetOptionMethod is None
+                                      else targetOptionMethod()).items()}
+
+        # determine keys for final output
+        keys=[name for name in options.keys() if name != NAME.COMMON]
+
+        # start with the defaults for the selected keys as a baseline
+        common=runnerDefaults.get(NAME.COMMON, {})
+        self.options={name: mergeDicts(common, runnerDefaults.get(name, {}))
+                      for name in keys}
+
+        # a NAME.TEMPLATE parameter in a target will cause the specified
+        # target to be extend by the default options of another target.
+        # Priority order: extraOptions > options > defaults > COMMON
+        for name, target in self.options.items():
+            template=(options[name][NAME.TEMPLATE]
+                      if name in options and NAME.TEMPLATE in options[name]
+                      else (runnerDefaults[name][NAME.TEMPLATE]
+                            if (name in runnerDefaults and
+                                NAME.TEMPLATE in runnerDefaults[name])
+                            else None))
+
+            if template is not None:
+                target.update(
+                    runnerDefaults.get(template, {}))
+
+        # now add our specific options from options and extraoptions
+        common=options.get(NAME.COMMON, {})
+        self.options={name: mergeDicts(self.options.get(name, {}),
+                                       mergeDicts(common, options[name]))
+                      for name in keys}
+
+        # finally, tag each target with its target name so that parameter links
+        # may address it over the key [NAME.TARGET]. Also, write down the name
+        # of the class in [NAME.CLASS]
+        for name, target in self.options.items():
+            target[NAME.TARGET]=name
+            target[NAME.CLASS]=targetClass.__name__
+
+        # initialize output
+        self.results=AccessDict({})
+
+    def emitStatus(self, *args):
+        """Short summary.
+
+        Parameters
+        ----------
+        *args : type
+            Description of parameter `*args`.
+
+        Returns
+        -------
+        type
+            Description of returned object.
+
+        """
+        if self.cbStatus is not None:
+            self.cbStatus(*args)
+
+    def emitResult(self, *args):
+        """Short summary.
+
+        Parameters
+        ----------
+        *args : type
+            Description of parameter `*args`.
+
+        Returns
+        -------
+        type
+            Description of returned object.
+
+        """
+        if self.cbResult is not None:
+            self.cbResult(*args)
+
+    def run(self, *targetNames, **extraArgs):
+        """Short summary.
+
+        Parameters
+        ----------
+        *targetNames : type
+            Description of parameter `*targetNames`.
+        **extraArgs : type
+            Description of parameter `**extraArgs`.
+
+        Returns
+        -------
+        type
+            Description of returned object.
+
+        """
+        '''
+        Execute all selected targets by a list of targetNames.
+        If *targetNames is empty all targets will be run.
+        The output of each :math:`TARGET` will be written to
+        self.results[:math:`TARGET`]
+        '''
+        # determine console width
+        self.consoleWidth=getConsoleSize()[1]
+
+        if len(targetNames) == 0:
+            targetNames=self.options.keys()
+
+        targets={name: self.options[name]
+                 for name in targetNames if name in self.options}
+
+        for name, target in sorted(targets.items()):
+            options=target.copy()
+
+            if len(extraArgs) > 0:
+                options.update(extraArgs)
+
+            result = self._run(name, options)
+
+            # make all result dicts of type accessDict for easy access
+            self.results[name] = convertToAccessDicts(result)
+            if self.cbResult is not None:
+                self.cbResult(name, result)
```

### Comparing `fastmat-0.2a4/fastmat.egg-info/PKG-INFO` & `fastmat-0.2rc0/fastmat.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: fastmat
-Version: 0.2a4
+Version: 0.2rc0
 Summary: fast linear transforms in Python
 Home-page: https://ems-tu-ilmenau.github.io/fastmat/
 Author: Christoph Wagner, Sebastian Semper, EMS group TU Ilmenau
 Author-email: christoph.wagner@tu-ilmenau.de
 License: Apache Software License
 Description: # fastmat
         [![Version](https://img.shields.io/pypi/v/fastmat.svg)](https://pypi.python.org/pypi/fastmat)
@@ -26,21 +26,26 @@
         Fastmat is a framework for handling large composed or structured matrices.
         It allows expressing and using them in a mathematically intuitive way while
         storing and handling them internally in an efficient way. This approach allows
         huge savings in computational time and memory requirements compared to using
         dense matrix representations.
         
         ### Dependencies
-        - Python >= 2.7 or >=3.4
+        - Python 2.7, Python >=3.4
         - Numpy >= 1.7
         - Scipy >= 1.0
         - Cython >= 0.29
         - soft dependencies:
             - matplotlib: for demos and tools that make use of plotting functions
         
+        ### Distribution
+        Binary wheels are provided for Python >=3.5 for linux, windows and mac, as well as for x86 and ARM architectures.
+        
+        For all systems, for which no wheels are provided, you may still install fastmat from the soruce distribution.
+        
         ### Authors & Contact Information
         - Sebastian Semper | sebastian.semper@tu-ilmenau.de
           Technische Universität Ilmenau, Institute for Mathematics, EMS Group
         - Christoph Wagner | christoph.wagner@tu-ilmenau.de
           Technische Universität Ilmenau, Institute for Information Technology, EMS Group
         - **<https://www.tu-ilmenau.de/it-ems/>**
         
@@ -72,14 +77,18 @@
         from the commandline by running one easy and straightforward command:
             `pip install fastmat`
         
         When installing with pip all dependencies of the package will be installed
         along. With release 0.1.1 python wheels will be offered for many versions
         greatly improving installation time and effort.
         
+        #### Bulding from source
+        
+        Building binaries has been developed and tested for the use
+        
         ### Manually installing from source
         - download the source distribution from our github repository:
             https://github.com/EMS-TU-Ilmenau/fastmat/archive/stable.zip
         - unpack its contents and navigate to the project root directory
         - run `pip install .` to install fastmat on your computer
         - you may also install fastmat without pip, using the offered makefile:
             * type `make install` to install fastmat on your computer
@@ -136,19 +145,23 @@
 Classifier: Framework :: IPython
 Classifier: Framework :: Jupyter
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX :: Linux
+Classifier: Operating System :: POSIX :: Other
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Topic :: Software Development :: Libraries
+Description-Content-Type: text/markdown
```

### Comparing `fastmat-0.2a4/fastmat.egg-info/SOURCES.txt` & `fastmat-0.2rc0/fastmat.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -1,58 +1,71 @@
 .version
 LICENSE
 MANIFEST.in
 README.md
 makefile
 setup.cfg
 setup.py
-demo/compOmpIsta.py
-demo/datenSAFT.mat
-demo/datenSAFT.py
-demo/edgeDetect.py
-demo/head.png
-demo/lowRankApprox.py
-demo/matrixSAFT.py
-demo/matrixSAFTmask.pyx
-demo/sparseReco.py
+doc/algorithms.rst
+doc/architecture.rst
 doc/classes.rst
 doc/conf.py
+doc/examples.rst
+doc/expansion.rst
 doc/index.rst
-doc/scipy.rst
-doc/submod.rst
+doc/inspection.rst
+doc/references.rst
+doc/releases.rst
+doc/_static/custom.css
+doc/_static/gfx/logo_favicon.png
+doc/_static/gfx/logo_long.png
+doc/_static/gfx/logo_short.png
 doc/algorithms/Algorithm.rst
 doc/algorithms/FISTA.rst
 doc/algorithms/ISTA.rst
 doc/algorithms/OMP.rst
 doc/algorithms/STELA.rst
+doc/architecture/algorithms.rst
+doc/architecture/calibration.rst
+doc/architecture/capi.rst
+doc/architecture/classes.rst
+doc/architecture/scipy.rst
+doc/architecture/strides.rst
+doc/architecture/types.rst
 doc/classes/BlockDiag.rst
 doc/classes/Blocks.rst
 doc/classes/Circulant.rst
 doc/classes/Diag.rst
 doc/classes/DiagBlocks.rst
 doc/classes/Eye.rst
 doc/classes/Fourier.rst
 doc/classes/Hadamard.rst
 doc/classes/Kron.rst
 doc/classes/LSFRCirculant.rst
 doc/classes/LowRank.rst
-doc/classes/MLCirculant.rst
-doc/classes/MLToeplitz.rst
-doc/classes/MLUltraSound.rst
 doc/classes/Matrix.rst
 doc/classes/Outer.rst
 doc/classes/Parametric.rst
 doc/classes/Partial.rst
 doc/classes/Permutation.rst
 doc/classes/Polynomial.rst
 doc/classes/Product.rst
 doc/classes/Sparse.rst
 doc/classes/Sum.rst
 doc/classes/Toeplitz.rst
+doc/classes/Transpose.rst
 doc/classes/Zero.rst
+doc/examples/compressed-sensing.py
+doc/examples/compressed-sensing.rst
+doc/examples/scipy-linear-operator.rst
+doc/examples/example_scripts/cs_example.py
+doc/expansion/implement.rst
+doc/expansion/optimize.rst
+doc/inspection/benchmark.rst
+doc/inspection/test.rst
 fastmat/BlockDiag.pxd
 fastmat/BlockDiag.pyx
 fastmat/Blocks.pxd
 fastmat/Blocks.pyx
 fastmat/Circulant.pxd
 fastmat/Circulant.pyx
 fastmat/Diag.pxd
```

### Comparing `fastmat-0.2a4/makefile` & `fastmat-0.2rc0/makefile`

 * *Files 2% similar despite different names*

```diff
@@ -79,25 +79,25 @@
 
 # Filename for list of files installed during 'setup.py install'
 FILE_LIST=setup.files
 
 # MODE may be specified from command line for choosing install mode.
 
 # python version
-PYTHON=python
+PYTHON=python3
 
 ifeq ($(OS),Windows_NT)
 else
 
 # STYLE_FILES specifies the files touched during coding style operations
 STYLE_FILES=*.py fastmat/*.py fastmat/*.pyx fastmat/*.pxd\
 	fastmat/*/*.py fastmat/*/*.pyx fastmat/*/*.pxd
 
 # STYLE_IGNORES lists the errors to be skipped during style check
-STYLE_IGNORES=E26,E116,E203,E221,E222,E225,E227,E241,E402,E731,W504,W605
+STYLE_IGNORES=E26,E116,E203,E221,E222,E225,E227,E241,E402,E731,W504,W605,W503
 
 # TEST_OPTIONS allows passing extra options to tests during `testCode`target
 TEST_OPTIONS=-i
 
 # CODEBASE_FILES lists all source code files in codebase
 CODEBASE_FILES:=$(shell find .\
 		-name 'makefile' -o -name '*.tex' -o\
@@ -129,31 +129,31 @@
 else
 # Linux flavour
 	@cat $(FILE_LIST) | xargs rm -rf
 	@rm -f $(FILE_LIST)
 endif
 
 
-# target 'compile': Comile fastmat package locally.
+# target 'compile': Compile fastmat package locally.
 .PHONY: compile
 compile:
 	$(info * compiling fastmat package locally)
 	$(PYTHON) setup.py build_ext --inplace
 
 .PHONY: compile-coverage
 compile-coverage:
 	$(info * compiling fastmat package locally, with profiling and tracing)
 	$(PYTHON) setup.py build_ext --inplace --enable-cython-tracing
 
 
 # target 'doc': Compile documentation
 .PHONY: doc
 doc: | compile
-	$(info * building documentation: redirecting to './doc/make doc')
-	@$(PYTHON) setup.py build_doc
+	$(info * building documentation)
+	@$(PYTHON) setup.py build_doc $(OPTIONS) -E
 
 # targer 'debug': Debug package
 .PHONY: debug
 debug: | compile
 	$(info * debugging package)
 	$(PYTHON) -i -c '\
 		from numpy import *;\
```

### Comparing `fastmat-0.2a4/setup.py` & `fastmat-0.2rc0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -37,15 +37,18 @@
 
 def WARNING(string):
     print("\033[91mWARNING:\033[0m %s" % (string))
 
 
 def ERROR(string, e):
     print("\033[91mERROR:\033[0m %s" % (string))
-    raise e
+    if isinstance(e, int):
+        sys.exit(e)
+    else:
+        raise e
 
 
 def INFO(string):
     print("\033[96mINFO:\033[0m %s" % (string))
 
 
 # load setup and extensions from setuptools. If that fails, try distutils
@@ -178,19 +181,32 @@
 def doc_opts():
     '''
     Introduce a command-line setup target to generate the sphinx doc.
     '''
     try:
         from sphinx.setup_command import BuildDoc
     except ImportError:
-        return {}
+        ERROR("Unable to import Sphinx for building the docs", 1)
 
-    class OwnDoc(BuildDoc):
+    class OwnDoc(BuildDoc, object):
 
         def __init__(self, *args, **kwargs):
+            # check if we have the necessary sphinx add-ons installed
+            import pip
+            global sphinxRequires
+            failed = []
+            for requirement in sphinxRequires:
+                try:
+                    __import__(requirement)
+                except ImportError:
+                    failed.append(requirement)
+
+            if len(failed) > 0:
+                ERROR("Following pypi packages are missing: %s" %(failed, ), 1)
+
             super(OwnDoc, self).__init__(*args, **kwargs)
 
     return OwnDoc
 
 
 ##############################################################################
 ### The actual script. KEEP THE `import filter` ALIVE AT ALL TIMES
@@ -220,14 +236,24 @@
     )
 
     f = (open(fileName, 'r') if sys.version_info < (3, 0)
          else open(fileName, 'r', encoding='utf-8'))
     longDescription = f.read()
     f.close()
 
+    pypiName = os.path.join(
+        os.path.abspath(os.path.dirname(__file__)),
+        'pypi.md'
+    )
+
+    f = (open(fileName, 'r') if sys.version_info < (3, 0)
+         else open(fileName, 'r', encoding='utf-8'))
+    pypiDescription = f.read()
+    f.close()
+
     # Build for generic (legacy) architectures when enviroment variable
     # (FASTMAT_GENERIC) is defined
     if 'FASTMAT_GENERIC' in os.environ:
         marchFlag = '-march=x86-64'
         mtuneFlag = '-mtune=core2'
         WARNING("Building package for generic architectures")
     else:
@@ -270,51 +296,60 @@
         packageVersion,
         strPlatform)
     )
 
     # check if all requirements are met prior to actually calling setup()
     setupRequires = []
     installRequires = []
+    sphinxRequires = ['sphinx', 'sphinx_rtd_theme', 'numpydoc', 'matplotlib']
     checkRequirement(setupRequires, 'setuptools', 'setuptools>=18.0')
     checkRequirement(setupRequires, 'Cython', 'cython>=0.29')
-    checkRequirement(setupRequires, 'numpy', 'numpy>=1.7')
+    if sys.version_info < (3, 5):
+        checkRequirement(setupRequires, 'numpy', 'numpy<1.17')
+    else:
+        checkRequirement(setupRequires, 'numpy', 'numpy>=1.7')
+
     checkRequirement(installRequires, 'six', 'six')
     checkRequirement(installRequires, 'scipy', 'scipy>=1.0')
 
     print("Requirements for setup: %s" % (setupRequires))
     print("Requirements for install: %s" % (installRequires))
 
     # everything's set. Fire in the hole.
     setup(
         name=packageName,
         version=packageVersion,
         description='fast linear transforms in Python',
-        long_description=longDescription,
+        long_description=pypiDescription,
+        long_description_content_type='text/markdown',
         author='Christoph Wagner, Sebastian Semper, EMS group TU Ilmenau',
         author_email='christoph.wagner@tu-ilmenau.de',
         url='https://ems-tu-ilmenau.github.io/fastmat/',
         license='Apache Software License',
         classifiers=[
             'Development Status :: 5 - Production/Stable',
             'Framework :: IPython',
             'Framework :: Jupyter',
             'Intended Audience :: Science/Research',
             'License :: OSI Approved :: Apache Software License',
             'Natural Language :: English',
             'Operating System :: Microsoft :: Windows',
             'Operating System :: POSIX :: Linux',
+            'Operating System :: POSIX :: Other',
             'Operating System :: MacOS :: MacOS X',
             'Programming Language :: Python',
             'Programming Language :: Python :: 2',
             'Programming Language :: Python :: 2.7',
             'Programming Language :: Python :: 3',
             'Programming Language :: Python :: 3.4',
             'Programming Language :: Python :: 3.5',
             'Programming Language :: Python :: 3.6',
             'Programming Language :: Python :: 3.7',
+            'Programming Language :: Python :: 3.8',
+            'Programming Language :: Python :: 3.9',
             'Topic :: Scientific/Engineering',
             'Topic :: Scientific/Engineering :: Mathematics',
             'Topic :: Software Development :: Libraries'
         ],
         keywords='linear transforms efficient algorithms mathematics',
         setup_requires=setupRequires,
         install_requires=installRequires,
```

