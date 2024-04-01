# Comparing `tmp/sequentia-1.1.1.tar.gz` & `tmp/sequentia-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sequentia-1.1.1.tar", last modified: Wed Feb  1 08:37:28 2023, max compression
+gzip compressed data, was "sequentia-2.0.0.tar", max compression
```

## Comparing `sequentia-1.1.1.tar` & `sequentia-2.0.0.tar`

### file list

```diff
@@ -1,84 +1,68 @@
-drwxr-xr-x   0 edwinonuonga   (501) staff       (20)        0 2023-02-01 08:37:28.434777 sequentia-1.1.1/
--rw-r--r--   0 edwinonuonga   (501) staff       (20)     1096 2023-02-01 08:37:12.000000 sequentia-1.1.1/LICENSE
--rw-r--r--   0 edwinonuonga   (501) staff       (20)    15965 2023-02-01 08:37:28.434561 sequentia-1.1.1/PKG-INFO
--rw-r--r--   0 edwinonuonga   (501) staff       (20)    12545 2023-01-18 01:43:19.000000 sequentia-1.1.1/README.md
-drwxr-xr-x   0 edwinonuonga   (501) staff       (20)        0 2023-02-01 08:37:28.419342 sequentia-1.1.1/lib/
-drwxr-xr-x   0 edwinonuonga   (501) staff       (20)        0 2023-02-01 08:37:28.420565 sequentia-1.1.1/lib/sequentia/
--rw-r--r--   0 edwinonuonga   (501) staff       (20)      264 2023-02-01 08:37:15.000000 sequentia-1.1.1/lib/sequentia/__init__.py
-drwxr-xr-x   0 edwinonuonga   (501) staff       (20)        0 2023-02-01 08:37:28.422323 sequentia-1.1.1/lib/sequentia/datasets/
--rw-r--r--   0 edwinonuonga   (501) staff       (20)       78 2022-12-06 22:05:19.000000 sequentia-1.1.1/lib/sequentia/datasets/__init__.py
-drwxr-xr-x   0 edwinonuonga   (501) staff       (20)        0 2023-02-01 08:37:28.422516 sequentia-1.1.1/lib/sequentia/datasets/data/
--rw-r--r--   0 edwinonuonga   (501) staff       (20)  2623137 2022-12-06 22:05:19.000000 sequentia-1.1.1/lib/sequentia/datasets/data/digits.npz
--rw-r--r--   0 edwinonuonga   (501) staff       (20)     1814 2023-01-07 20:55:15.000000 sequentia-1.1.1/lib/sequentia/datasets/digits.py
--rw-r--r--   0 edwinonuonga   (501) staff       (20)     2551 2023-01-07 20:55:15.000000 sequentia-1.1.1/lib/sequentia/datasets/gene_families.py
-drwxr-xr-x   0 edwinonuonga   (501) staff       (20)        0 2023-02-01 08:37:28.426122 sequentia-1.1.1/lib/sequentia/models/
--rw-r--r--   0 edwinonuonga   (501) staff       (20)       58 2022-12-06 22:05:19.000000 sequentia-1.1.1/lib/sequentia/models/__init__.py
--rw-r--r--   0 edwinonuonga   (501) staff       (20)     2465 2023-01-18 01:43:19.000000 sequentia-1.1.1/lib/sequentia/models/base.py
-drwxr-xr-x   0 edwinonuonga   (501) staff       (20)        0 2023-02-01 08:37:28.427595 sequentia-1.1.1/lib/sequentia/models/hmm/
--rw-r--r--   0 edwinonuonga   (501) staff       (20)       50 2022-12-06 22:05:19.000000 sequentia-1.1.1/lib/sequentia/models/hmm/__init__.py
--rw-r--r--   0 edwinonuonga   (501) staff       (20)    21614 2023-01-18 01:43:19.000000 sequentia-1.1.1/lib/sequentia/models/hmm/classifier.py
--rw-r--r--   0 edwinonuonga   (501) staff       (20)    10241 2023-01-07 20:55:15.000000 sequentia-1.1.1/lib/sequentia/models/hmm/topologies.py
-drwxr-xr-x   0 edwinonuonga   (501) staff       (20)        0 2023-02-01 08:37:28.428564 sequentia-1.1.1/lib/sequentia/models/hmm/variants/
--rw-r--r--   0 edwinonuonga   (501) staff       (20)       59 2022-12-06 22:05:19.000000 sequentia-1.1.1/lib/sequentia/models/hmm/variants/__init__.py
--rw-r--r--   0 edwinonuonga   (501) staff       (20)    12342 2023-01-07 20:55:15.000000 sequentia-1.1.1/lib/sequentia/models/hmm/variants/base.py
--rw-r--r--   0 edwinonuonga   (501) staff       (20)    10154 2023-01-07 20:55:15.000000 sequentia-1.1.1/lib/sequentia/models/hmm/variants/categorical.py
--rw-r--r--   0 edwinonuonga   (501) staff       (20)    13234 2023-01-07 20:55:15.000000 sequentia-1.1.1/lib/sequentia/models/hmm/variants/gaussian_mixture.py
-drwxr-xr-x   0 edwinonuonga   (501) staff       (20)        0 2023-02-01 08:37:28.429239 sequentia-1.1.1/lib/sequentia/models/knn/
--rw-r--r--   0 edwinonuonga   (501) staff       (20)       51 2022-12-06 22:05:19.000000 sequentia-1.1.1/lib/sequentia/models/knn/__init__.py
--rw-r--r--   0 edwinonuonga   (501) staff       (20)    15745 2023-01-18 01:43:19.000000 sequentia-1.1.1/lib/sequentia/models/knn/base.py
--rw-r--r--   0 edwinonuonga   (501) staff       (20)    15588 2023-01-18 01:43:19.000000 sequentia-1.1.1/lib/sequentia/models/knn/classifier.py
--rw-r--r--   0 edwinonuonga   (501) staff       (20)     9214 2023-01-18 01:43:19.000000 sequentia-1.1.1/lib/sequentia/models/knn/regressor.py
--rw-r--r--   0 edwinonuonga   (501) staff       (20)    24263 2023-01-18 01:43:19.000000 sequentia-1.1.1/lib/sequentia/pipeline.py
-drwxr-xr-x   0 edwinonuonga   (501) staff       (20)        0 2023-02-01 08:37:28.429808 sequentia-1.1.1/lib/sequentia/preprocessing/
--rw-r--r--   0 edwinonuonga   (501) staff       (20)       26 2022-12-06 22:05:19.000000 sequentia-1.1.1/lib/sequentia/preprocessing/__init__.py
--rw-r--r--   0 edwinonuonga   (501) staff       (20)     1188 2023-01-18 01:43:19.000000 sequentia-1.1.1/lib/sequentia/preprocessing/base.py
--rw-r--r--   0 edwinonuonga   (501) staff       (20)    13655 2023-02-01 08:37:12.000000 sequentia-1.1.1/lib/sequentia/preprocessing/transforms.py
-drwxr-xr-x   0 edwinonuonga   (501) staff       (20)        0 2023-02-01 08:37:28.430628 sequentia-1.1.1/lib/sequentia/utils/
--rw-r--r--   0 edwinonuonga   (501) staff       (20)      103 2022-12-06 22:05:19.000000 sequentia-1.1.1/lib/sequentia/utils/__init__.py
--rw-r--r--   0 edwinonuonga   (501) staff       (20)     9622 2023-01-07 20:55:15.000000 sequentia-1.1.1/lib/sequentia/utils/data.py
--rw-r--r--   0 edwinonuonga   (501) staff       (20)     1982 2022-12-06 22:05:19.000000 sequentia-1.1.1/lib/sequentia/utils/decorators.py
--rw-r--r--   0 edwinonuonga   (501) staff       (20)      302 2022-12-06 22:05:19.000000 sequentia-1.1.1/lib/sequentia/utils/multiprocessing.py
--rw-r--r--   0 edwinonuonga   (501) staff       (20)     6619 2022-12-06 22:05:19.000000 sequentia-1.1.1/lib/sequentia/utils/validation.py
-drwxr-xr-x   0 edwinonuonga   (501) staff       (20)        0 2023-02-01 08:37:28.421699 sequentia-1.1.1/lib/sequentia.egg-info/
--rw-r--r--   0 edwinonuonga   (501) staff       (20)    15965 2023-02-01 08:37:28.000000 sequentia-1.1.1/lib/sequentia.egg-info/PKG-INFO
--rw-r--r--   0 edwinonuonga   (501) staff       (20)     2145 2023-02-01 08:37:28.000000 sequentia-1.1.1/lib/sequentia.egg-info/SOURCES.txt
--rw-r--r--   0 edwinonuonga   (501) staff       (20)        1 2023-02-01 08:37:28.000000 sequentia-1.1.1/lib/sequentia.egg-info/dependency_links.txt
--rw-r--r--   0 edwinonuonga   (501) staff       (20)      227 2023-02-01 08:37:28.000000 sequentia-1.1.1/lib/sequentia.egg-info/requires.txt
--rw-r--r--   0 edwinonuonga   (501) staff       (20)       15 2023-02-01 08:37:28.000000 sequentia-1.1.1/lib/sequentia.egg-info/top_level.txt
-drwxr-xr-x   0 edwinonuonga   (501) staff       (20)        0 2023-02-01 08:37:28.430842 sequentia-1.1.1/lib/test/
--rw-r--r--   0 edwinonuonga   (501) staff       (20)        0 2023-01-07 20:55:15.000000 sequentia-1.1.1/lib/test/__init__.py
-drwxr-xr-x   0 edwinonuonga   (501) staff       (20)        0 2023-02-01 08:37:28.431075 sequentia-1.1.1/lib/test/lib/
--rw-r--r--   0 edwinonuonga   (501) staff       (20)        0 2023-01-07 20:55:15.000000 sequentia-1.1.1/lib/test/lib/__init__.py
-drwxr-xr-x   0 edwinonuonga   (501) staff       (20)        0 2023-02-01 08:37:28.431680 sequentia-1.1.1/lib/test/lib/datasets/
--rw-r--r--   0 edwinonuonga   (501) staff       (20)        0 2023-01-07 20:55:15.000000 sequentia-1.1.1/lib/test/lib/datasets/__init__.py
--rw-r--r--   0 edwinonuonga   (501) staff       (20)      436 2023-01-07 20:55:15.000000 sequentia-1.1.1/lib/test/lib/datasets/test_digits.py
--rw-r--r--   0 edwinonuonga   (501) staff       (20)      592 2023-01-07 20:55:15.000000 sequentia-1.1.1/lib/test/lib/datasets/test_gene_families.py
-drwxr-xr-x   0 edwinonuonga   (501) staff       (20)        0 2023-02-01 08:37:28.431866 sequentia-1.1.1/lib/test/lib/models/
--rw-r--r--   0 edwinonuonga   (501) staff       (20)        0 2023-01-07 20:55:15.000000 sequentia-1.1.1/lib/test/lib/models/__init__.py
-drwxr-xr-x   0 edwinonuonga   (501) staff       (20)        0 2023-02-01 08:37:28.432196 sequentia-1.1.1/lib/test/lib/models/hmm/
--rw-r--r--   0 edwinonuonga   (501) staff       (20)        0 2023-01-07 20:55:15.000000 sequentia-1.1.1/lib/test/lib/models/hmm/__init__.py
--rw-r--r--   0 edwinonuonga   (501) staff       (20)     5034 2023-01-07 20:55:15.000000 sequentia-1.1.1/lib/test/lib/models/hmm/test_classifier.py
--rw-r--r--   0 edwinonuonga   (501) staff       (20)    13570 2023-01-07 20:55:15.000000 sequentia-1.1.1/lib/test/lib/models/hmm/test_topologies.py
-drwxr-xr-x   0 edwinonuonga   (501) staff       (20)        0 2023-02-01 08:37:28.432577 sequentia-1.1.1/lib/test/lib/models/hmm/variants/
--rw-r--r--   0 edwinonuonga   (501) staff       (20)        0 2023-01-07 20:55:15.000000 sequentia-1.1.1/lib/test/lib/models/hmm/variants/__init__.py
--rw-r--r--   0 edwinonuonga   (501) staff       (20)     5614 2023-01-07 20:55:15.000000 sequentia-1.1.1/lib/test/lib/models/hmm/variants/test_categorical.py
--rw-r--r--   0 edwinonuonga   (501) staff       (20)     7546 2023-01-07 20:55:15.000000 sequentia-1.1.1/lib/test/lib/models/hmm/variants/test_gaussian_mixture.py
-drwxr-xr-x   0 edwinonuonga   (501) staff       (20)        0 2023-02-01 08:37:28.432967 sequentia-1.1.1/lib/test/lib/models/knn/
--rw-r--r--   0 edwinonuonga   (501) staff       (20)        0 2023-01-07 20:55:15.000000 sequentia-1.1.1/lib/test/lib/models/knn/__init__.py
--rw-r--r--   0 edwinonuonga   (501) staff       (20)     7970 2023-01-07 20:55:15.000000 sequentia-1.1.1/lib/test/lib/models/knn/test_classifier.py
--rw-r--r--   0 edwinonuonga   (501) staff       (20)     5071 2023-01-07 20:55:15.000000 sequentia-1.1.1/lib/test/lib/models/knn/test_regressor.py
-drwxr-xr-x   0 edwinonuonga   (501) staff       (20)        0 2023-02-01 08:37:28.433197 sequentia-1.1.1/lib/test/lib/preprocessing/
--rw-r--r--   0 edwinonuonga   (501) staff       (20)        0 2023-01-18 01:43:19.000000 sequentia-1.1.1/lib/test/lib/preprocessing/__init__.py
--rw-r--r--   0 edwinonuonga   (501) staff       (20)     2455 2023-01-18 01:43:19.000000 sequentia-1.1.1/lib/test/lib/preprocessing/test_transforms.py
--rw-r--r--   0 edwinonuonga   (501) staff       (20)     7073 2023-01-18 01:43:19.000000 sequentia-1.1.1/lib/test/lib/test_pipeline.py
-drwxr-xr-x   0 edwinonuonga   (501) staff       (20)        0 2023-02-01 08:37:28.433807 sequentia-1.1.1/lib/test/lib/utils/
--rw-r--r--   0 edwinonuonga   (501) staff       (20)        0 2023-01-07 20:55:15.000000 sequentia-1.1.1/lib/test/lib/utils/__init__.py
--rw-r--r--   0 edwinonuonga   (501) staff       (20)     5896 2023-01-07 20:55:15.000000 sequentia-1.1.1/lib/test/lib/utils/test_data.py
--rw-r--r--   0 edwinonuonga   (501) staff       (20)     1836 2023-01-07 20:55:15.000000 sequentia-1.1.1/lib/test/lib/utils/test_decorators.py
--rw-r--r--   0 edwinonuonga   (501) staff       (20)       11 2023-01-07 20:55:15.000000 sequentia-1.1.1/lib/test/lib/utils/test_validation.py
-drwxr-xr-x   0 edwinonuonga   (501) staff       (20)        0 2023-02-01 08:37:28.434216 sequentia-1.1.1/lib/test/support/
--rw-r--r--   0 edwinonuonga   (501) staff       (20)        0 2023-01-07 20:55:15.000000 sequentia-1.1.1/lib/test/support/__init__.py
--rw-r--r--   0 edwinonuonga   (501) staff       (20)      574 2023-01-07 20:55:15.000000 sequentia-1.1.1/lib/test/support/assertions.py
--rw-r--r--   0 edwinonuonga   (501) staff       (20)      210 2023-01-07 20:55:15.000000 sequentia-1.1.1/lib/test/support/itertools.py
--rw-r--r--   0 edwinonuonga   (501) staff       (20)       38 2023-02-01 08:37:28.434828 sequentia-1.1.1/setup.cfg
--rw-r--r--   0 edwinonuonga   (501) staff       (20)     2628 2023-01-18 01:43:19.000000 sequentia-1.1.1/setup.py
+-rw-r--r--   0        0        0    22910 2024-04-01 17:47:59.530467 sequentia-2.0.0/CHANGELOG.md
+-rw-r--r--   0        0        0     1096 2024-04-01 17:47:59.530467 sequentia-2.0.0/LICENSE
+-rw-r--r--   0        0        0      473 2024-04-01 17:47:59.530467 sequentia-2.0.0/Makefile
+-rw-r--r--   0        0        0    12403 2024-04-01 17:47:59.530467 sequentia-2.0.0/README.md
+-rw-r--r--   0        0        0      326 2024-04-01 17:47:59.534467 sequentia-2.0.0/make/__init__.py
+-rw-r--r--   0        0        0      506 2024-04-01 17:47:59.534467 sequentia-2.0.0/make/cov.py
+-rw-r--r--   0        0        0      919 2024-04-01 17:47:59.534467 sequentia-2.0.0/make/docs.py
+-rw-r--r--   0        0        0     1056 2024-04-01 17:47:59.534467 sequentia-2.0.0/make/lint.py
+-rw-r--r--   0        0        0     1147 2024-04-01 17:47:59.534467 sequentia-2.0.0/make/release.py
+-rw-r--r--   0        0        0      758 2024-04-01 17:47:59.534467 sequentia-2.0.0/make/tests.py
+-rw-r--r--   0        0        0     7547 2024-04-01 17:47:59.534467 sequentia-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0      547 2024-04-01 17:47:59.534467 sequentia-2.0.0/sequentia/__init__.py
+-rw-r--r--   0        0        0      241 2024-04-01 17:47:59.534467 sequentia-2.0.0/sequentia/_internal/__init__.py
+-rw-r--r--   0        0        0      663 2024-04-01 17:47:59.534467 sequentia-2.0.0/sequentia/_internal/_data.py
+-rw-r--r--   0        0        0      290 2024-04-01 17:47:59.534467 sequentia-2.0.0/sequentia/_internal/_hmm/__init__.py
+-rw-r--r--   0        0        0    11861 2024-04-01 17:47:59.534467 sequentia-2.0.0/sequentia/_internal/_hmm/topologies.py
+-rw-r--r--   0        0        0      539 2024-04-01 17:47:59.538467 sequentia-2.0.0/sequentia/_internal/_multiprocessing.py
+-rw-r--r--   0        0        0      434 2024-04-01 17:47:59.538467 sequentia-2.0.0/sequentia/_internal/_typing.py
+-rw-r--r--   0        0        0     6762 2024-04-01 17:47:59.538467 sequentia-2.0.0/sequentia/_internal/_validation.py
+-rw-r--r--   0        0        0      594 2024-04-01 17:47:59.538467 sequentia-2.0.0/sequentia/datasets/__init__.py
+-rw-r--r--   0        0        0    12315 2024-04-01 17:47:59.538467 sequentia-2.0.0/sequentia/datasets/base.py
+-rw-r--r--   0        0        0      277 2024-04-01 17:47:59.538467 sequentia-2.0.0/sequentia/datasets/data/__init__.py
+-rw-r--r--   0        0        0  2623137 2024-04-01 17:47:59.542467 sequentia-2.0.0/sequentia/datasets/data/digits.npz
+-rw-r--r--   0        0        0  2106823 2024-04-01 17:47:59.554467 sequentia-2.0.0/sequentia/datasets/data/gene_families.npz
+-rw-r--r--   0        0        0     1840 2024-04-01 17:47:59.554467 sequentia-2.0.0/sequentia/datasets/digits.py
+-rw-r--r--   0        0        0     2574 2024-04-01 17:47:59.554467 sequentia-2.0.0/sequentia/datasets/gene_families.py
+-rw-r--r--   0        0        0     2778 2024-04-01 17:47:59.554467 sequentia-2.0.0/sequentia/enums.py
+-rw-r--r--   0        0        0      607 2024-04-01 17:47:59.554467 sequentia-2.0.0/sequentia/models/__init__.py
+-rw-r--r--   0        0        0     6702 2024-04-01 17:47:59.554467 sequentia-2.0.0/sequentia/models/base.py
+-rw-r--r--   0        0        0      508 2024-04-01 17:47:59.554467 sequentia-2.0.0/sequentia/models/hmm/__init__.py
+-rw-r--r--   0        0        0    18497 2024-04-01 17:47:59.554467 sequentia-2.0.0/sequentia/models/hmm/classifier.py
+-rw-r--r--   0        0        0      488 2024-04-01 17:47:59.554467 sequentia-2.0.0/sequentia/models/hmm/variants/__init__.py
+-rw-r--r--   0        0        0    16915 2024-04-01 17:47:59.554467 sequentia-2.0.0/sequentia/models/hmm/variants/base.py
+-rw-r--r--   0        0        0     6726 2024-04-01 17:47:59.554467 sequentia-2.0.0/sequentia/models/hmm/variants/categorical.py
+-rw-r--r--   0        0        0     9787 2024-04-01 17:47:59.554467 sequentia-2.0.0/sequentia/models/hmm/variants/gaussian_mixture.py
+-rw-r--r--   0        0        0      488 2024-04-01 17:47:59.554467 sequentia-2.0.0/sequentia/models/knn/__init__.py
+-rw-r--r--   0        0        0    10632 2024-04-01 17:47:59.554467 sequentia-2.0.0/sequentia/models/knn/base.py
+-rw-r--r--   0        0        0    13887 2024-04-01 17:47:59.554467 sequentia-2.0.0/sequentia/models/knn/classifier.py
+-rw-r--r--   0        0        0     7172 2024-04-01 17:47:59.554467 sequentia-2.0.0/sequentia/models/knn/regressor.py
+-rw-r--r--   0        0        0      475 2024-04-01 17:47:59.554467 sequentia-2.0.0/sequentia/preprocessing/__init__.py
+-rw-r--r--   0        0        0    13569 2024-04-01 17:47:59.554467 sequentia-2.0.0/sequentia/preprocessing/transforms.py
+-rw-r--r--   0        0        0     2965 2024-04-01 17:47:59.554467 sequentia-2.0.0/sequentia/version.py
+-rw-r--r--   0        0        0     1878 2024-04-01 17:47:59.554467 sequentia-2.0.0/tasks.py
+-rw-r--r--   0        0        0      260 2024-04-01 17:47:59.554467 sequentia-2.0.0/tests/__init__.py
+-rw-r--r--   0        0        0     1816 2024-04-01 17:47:59.554467 sequentia-2.0.0/tests/conftest.py
+-rw-r--r--   0        0        0      241 2024-04-01 17:47:59.554467 sequentia-2.0.0/tests/unit/__init__.py
+-rw-r--r--   0        0        0      241 2024-04-01 17:47:59.554467 sequentia-2.0.0/tests/unit/test_datasets/__init__.py
+-rw-r--r--   0        0        0     6696 2024-04-01 17:47:59.554467 sequentia-2.0.0/tests/unit/test_datasets/test_base.py
+-rw-r--r--   0        0        0      729 2024-04-01 17:47:59.554467 sequentia-2.0.0/tests/unit/test_datasets/test_digits.py
+-rw-r--r--   0        0        0      855 2024-04-01 17:47:59.554467 sequentia-2.0.0/tests/unit/test_datasets/test_gene_families.py
+-rw-r--r--   0        0        0      241 2024-04-01 17:47:59.554467 sequentia-2.0.0/tests/unit/test_internal/__init__.py
+-rw-r--r--   0        0        0      297 2024-04-01 17:47:59.554467 sequentia-2.0.0/tests/unit/test_internal/test_data.py
+-rw-r--r--   0        0        0      241 2024-04-01 17:47:59.554467 sequentia-2.0.0/tests/unit/test_internal/test_hmm/__init__.py
+-rw-r--r--   0        0        0    16110 2024-04-01 17:47:59.554467 sequentia-2.0.0/tests/unit/test_internal/test_hmm/test_topologies.py
+-rw-r--r--   0        0        0      241 2024-04-01 17:47:59.554467 sequentia-2.0.0/tests/unit/test_models/__init__.py
+-rw-r--r--   0        0        0      241 2024-04-01 17:47:59.554467 sequentia-2.0.0/tests/unit/test_models/hmm/__init__.py
+-rw-r--r--   0        0        0     6160 2024-04-01 17:47:59.554467 sequentia-2.0.0/tests/unit/test_models/hmm/test_classifier.py
+-rw-r--r--   0        0        0      241 2024-04-01 17:47:59.554467 sequentia-2.0.0/tests/unit/test_models/hmm/variants/__init__.py
+-rw-r--r--   0        0        0     7368 2024-04-01 17:47:59.554467 sequentia-2.0.0/tests/unit/test_models/hmm/variants/test_categorical.py
+-rw-r--r--   0        0        0     9601 2024-04-01 17:47:59.554467 sequentia-2.0.0/tests/unit/test_models/hmm/variants/test_gaussian_mixture.py
+-rw-r--r--   0        0        0      241 2024-04-01 17:47:59.554467 sequentia-2.0.0/tests/unit/test_models/knn/__init__.py
+-rw-r--r--   0        0        0     9012 2024-04-01 17:47:59.554467 sequentia-2.0.0/tests/unit/test_models/knn/test_classifier.py
+-rw-r--r--   0        0        0     6020 2024-04-01 17:47:59.554467 sequentia-2.0.0/tests/unit/test_models/knn/test_regressor.py
+-rw-r--r--   0        0        0     8146 2024-04-01 17:47:59.554467 sequentia-2.0.0/tests/unit/test_pipeline.py
+-rw-r--r--   0        0        0      241 2024-04-01 17:47:59.554467 sequentia-2.0.0/tests/unit/test_preprocessing/__init__.py
+-rw-r--r--   0        0        0     3129 2024-04-01 17:47:59.554467 sequentia-2.0.0/tests/unit/test_preprocessing/test_transforms.py
+-rw-r--r--   0        0        0      445 2024-04-01 17:47:59.554467 sequentia-2.0.0/tox.ini
+-rw-r--r--   0        0        0    14369 1970-01-01 00:00:00.000000 sequentia-2.0.0/PKG-INFO
```

### Comparing `sequentia-1.1.1/LICENSE` & `sequentia-2.0.0/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2019-2023 Edwin Onuonga (eonu) <ed@eonu.net>
+Copyright (c) 2019-2025 Edwin Onuonga (eonu) <ed@eonu.net>
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `sequentia-1.1.1/PKG-INFO` & `sequentia-2.0.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,318 +1,316 @@
 Metadata-Version: 2.1
 Name: sequentia
-Version: 1.1.1
-Summary: HMM and DTW-based sequence machine learning algorithms in Python following an sklearn-like interface.
+Version: 2.0.0
+Summary: Scikit-Learn compatible HMM and DTW based sequence machine learning algorithms in Python.
 Home-page: https://github.com/eonu/sequentia
+License: MIT
+Keywords: python,machine-learning,time-series,hmm,hidden-markov-models,dtw,dynamic-time-warping,knn,k-nearest-neighbors,sequence-classification,time-series-classification,multivariate-time-series,variable-length,classification-algorithms
 Author: Edwin Onuonga
 Author-email: ed@eonu.net
-License: MIT
-Project-URL: Documentation, https://sequentia.readthedocs.io/en/latest
-Project-URL: Bug Tracker, https://github.com/eonu/sequentia/issues
-Project-URL: Source Code, https://github.com/eonu/sequentia
-Description: <p align="center">
-          <h1 align="center">
-            <img src="https://raw.githubusercontent.com/eonu/sequentia/master/docs/_static/images/logo.png" width="75px"><br/>
-            Sequentia
-          </h1>
-        </p>
-        
-        <p align="center">
-          <em>HMM and DTW-based sequence machine learning algorithms in Python following an sklearn-like interface.</em>
-        </p>
-        
-        <p align="center">
-          <div align="center">
-            <a href="https://pypi.org/project/sequentia">
-              <img src="https://img.shields.io/pypi/v/sequentia?logo=pypi&style=flat-square" alt="PyPI"/>
-            </a>
-            <a href="https://pypi.org/project/sequentia">
-              <img src="https://img.shields.io/pypi/pyversions/sequentia?logo=python&style=flat-square" alt="PyPI - Python Version"/>
-            </a>
-            <a href="https://sequentia.readthedocs.io/en/latest">
-              <img src="https://img.shields.io/readthedocs/sequentia.svg?logo=read-the-docs&style=flat-square" alt="Read The Docs - Documentation">
-            </a>
-            <a href="https://raw.githubusercontent.com/eonu/sequentia/master/LICENSE">
-              <img src="https://img.shields.io/pypi/l/sequentia?style=flat-square" alt="PyPI - License"/>
-            </a>
-          </div>
-        </p>
-        
-        <p align="center">
-          <sup>
-            <a href="#about">About</a> ·
-            <a href="#build-status">Build Status</a> ·
-            <a href="#features">Features</a> ·
-            <a href="#documentation">Documentation</a> ·
-            <a href="#examples">Examples</a> ·
-            <a href="#acknowledgments">Acknowledgments</a> ·
-            <a href="#references">References</a> ·
-            <a href="#contributors">Contributors</a> ·
-            <a href="#licensing">Licensing</a>
-          </sup>
-        </p>
-        
-        ## About
-        
-        Sequentia is a Python package that provides various classification and regression algorithms for sequential data, including methods based on hidden Markov models and dynamic time warping.
-        
-        Some examples of how Sequentia can be used on sequence data include:
-        
-        - determining a spoken word based on its audio signal or alternative representations such as MFCCs,
-        - predicting motion intent for gesture control from sEMG signals,
-        - classifying hand-written characters according to their pen-tip trajectories.
-        
-        ## Build Status
-        
-        | `master` | `dev` |
-        | -------- | ------|
-        | [![CircleCI Build (Master)](https://img.shields.io/circleci/build/github/eonu/sequentia/master?logo=circleci&style=flat-square)](https://app.circleci.com/pipelines/github/eonu/sequentia?branch=master) | [![CircleCI Build (Development)](https://img.shields.io/circleci/build/github/eonu/sequentia/dev?logo=circleci&style=flat-square)](https://app.circleci.com/pipelines/github/eonu/sequentia?branch=master) |
-        
-        ## Features
-        
-        ### Models
-        
-        The following models provided by Sequentia all support variable length sequences.
-        
-        #### [Dynamic Time Warping + k-Nearest Neighbors](https://sequentia.readthedocs.io/en/latest/sections/models/knn/index.html) (via [`dtaidistance`](https://github.com/wannesm/dtaidistance))
-        
-        - [x] Classification
-        - [x] Regression
-        - [x] Multivariate real-valued observations
-        - [x] Sakoe–Chiba band global warping constraint
-        - [x] Dependent and independent feature warping (DTWD/DTWI)
-        - [x] Custom distance-weighted predictions
-        - [x] Multi-processed predictions
-        
-        #### [Hidden Markov Models](https://sequentia.readthedocs.io/en/latest/sections/models/hmm/index.html) (via [`hmmlearn`](https://github.com/hmmlearn/hmmlearn))
-        
-        Parameter estimation with the Baum-Welch algorithm and prediction with the forward algorithm [[1]](#references)
-        
-        - [x] Classification
-        - [x] Multivariate real-valued observations (Gaussian mixture model emissions)
-        - [x] Univariate categorical observations (discrete emissions)
-        - [x] Linear, left-right and ergodic topologies
-        - [x] Multi-processed predictions
-        
-        ### Scikit-Learn compatibility
-        
-        Sequentia aims to follow the Scikit-Learn interface for estimators and transformations,
-        as well as to be largely compatible with three core Scikit-Learn modules to improve the ease of model development:
-        [`preprocessing`](https://scikit-learn.org/stable/modules/classes.html#module-sklearn.preprocessing), [`model_selection`](https://scikit-learn.org/stable/modules/classes.html#module-sklearn.model_selection) and [`pipeline`](https://scikit-learn.org/stable/modules/classes.html#module-sklearn.pipeline).
-        
-        While there are many other modules, maintaining full compatibility with Scikit-Learn is challenging and many of its features are inapplicable to sequential data, therefore we only focus on the relevant core modules.
-        
-        Despite some deviation from the Scikit-Learn interface in order to accommodate sequences, the following features are currently compatible with Sequentia.
-        
-        - [x] [`preprocessing`](https://scikit-learn.org/stable/modules/classes.html#module-sklearn.preprocessing)
-          - [x] [`FunctionTransformer`](https://scikit-learn.org/stable/modules/generated/sklearn.preprocessing.FunctionTransformer.html#sklearn.preprocessing.FunctionTransformer) — via an adapted class definition
-          - [x] Function-based transformations (stateless)
-          - [x] Class-based transformations (stateful)
-        - [ ] [`pipeline`](https://scikit-learn.org/stable/modules/classes.html#module-sklearn.pipeline)
-          - [x] [`Pipeline`](https://scikit-learn.org/stable/modules/generated/sklearn.pipeline.Pipeline.html#sklearn.pipeline.Pipeline) — via an adapted class definition
-          - [ ] [`FeatureUnion`](https://scikit-learn.org/stable/modules/generated/sklearn.pipeline.FeatureUnion.html#sklearn.pipeline.FeatureUnion)
-        - [ ] [`model_selection`](https://scikit-learn.org/stable/modules/classes.html#module-sklearn.model_selection)
-        
-        ## Installation
-        
-        You can install Sequentia using `pip`.
-        
-        ### Stable
-        
-        The latest stable version of Sequentia can be installed with the following command.
-        
-        ```console
-        pip install sequentia
-        ```
-        
-        #### C library compilation
-        
-        For optimal performance when using any of the k-NN based models, it is important that `dtaidistance` C libraries are compiled correctly.
-        
-        Please see the [`dtaidistance` installation guide](https://dtaidistance.readthedocs.io/en/latest/usage/installation.html) for troubleshooting if you run into C compilation issues, or if setting `use_c=True` on k-NN based models results in a warning.
-        
-        You can use the following to check if the appropriate C libraries have been installed.
-        
-        ```python
-        from dtaidistance import dtw
-        dtw.try_import_c()
-        ```
-        
-        ### Pre-release
-        
-        Pre-release versions include new features which are in active development and may change unpredictably.
-        
-        The latest pre-release version can be installed with the following command.
-        
-        ```console
-        pip install --pre sequentia
-        ```
-        
-        ### Development
-        
-        Please see the [contribution guidelines](/CONTRIBUTING.md) to see installation instructions for contributing to Sequentia.
-        
-        ## Documentation
-        
-        Documentation for the package is available on [Read The Docs](https://sequentia.readthedocs.io/en/latest).
-        
-        ## Examples
-        
-        Demonstration of classifying multivariate sequences with two features into two classes using the `KNNClassifier`.
-        
-        This example also shows a typical preprocessing workflow, as well as compatibility with Scikit-Learn.
-        
-        ```python
-        import numpy as np
-        
-        from sklearn.preprocessing import scale
-        from sklearn.decomposition import PCA
-        
-        from sequentia.models import KNNClassifier
-        from sequentia.pipeline import Pipeline
-        from sequentia.preprocessing import IndependentFunctionTransformer, mean_filter
-        
-        # Create input data
-        # - Sequentia expects sequences to be concatenated into a single array
-        # - Sequence lengths are provided separately and used to decode the sequences when needed
-        # - This avoids the need for complex structures such as lists of arrays with different lengths
-        
-        # Sequences
-        X = np.array([
-            # Sequence 1 - Length 3
-            [1.2 , 7.91],
-            [1.34, 6.6 ],
-            [0.92, 8.08],
-            # Sequence 2 - Length 5
-            [2.11, 6.97],
-            [1.83, 7.06],
-            [1.54, 5.98],
-            [0.86, 6.37],
-            [1.21, 5.8 ],
-            # Sequence 3 - Length 2
-            [1.7 , 6.22],
-            [2.01, 5.49]
-        ])
-        
-        # Sequence lengths
-        lengths = np.array([3, 5, 2])
-        
-        # Sequence classes
-        y = np.array([0, 1, 1])
-        
-        # Create a transformation pipeline that feeds into a KNNClassifier
-        # 1. Individually denoise each sequence by applying a mean filter for each feature
-        # 2. Individually standardize each sequence by subtracting the mean and dividing the s.d. for each feature
-        # 3. Reduce the dimensionality of the data to a single feature by using PCA
-        # 4. Pass the resulting transformed data into a KNNClassifier
-        pipeline = Pipeline([
-            ('denoise', IndependentFunctionTransformer(mean_filter)),
-            ('scale', IndependentFunctionTransformer(scale)),
-            ('pca', PCA(n_components=1)),
-            ('knn', KNNClassifier(k=1))
-        ])
-        
-        # Fit the pipeline to the data - lengths must be provided
-        pipeline.fit(X, y, lengths)
-        
-        # Predict classes for the sequences and calculate accuracy - lengths must be provided
-        y_pred = pipeline.predict(X, lengths)
-        acc = pipeline.score(X, y, lengths)
-        ```
-        
-        ## Acknowledgments
-        
-        In earlier versions of the package, an approximate DTW implementation [`fastdtw`](https://github.com/slaypni/fastdtw) was used in hopes of speeding up k-NN predictions, as the authors of the original FastDTW paper [[2]](#references) claim that approximated DTW alignments can be computed in linear memory and time, compared to the O(N<sup>2</sup>) runtime complexity of the usual exact DTW implementation.
-        
-        I was contacted by [Prof. Eamonn Keogh](https://www.cs.ucr.edu/~eamonn/) whose work makes the surprising revelation that FastDTW is generally slower than the exact DTW algorithm that it approximates [[3]](#references). Upon switching from the `fastdtw` package to [`dtaidistance`](https://github.com/wannesm/dtaidistance) (a very solid implementation of exact DTW with fast pure C compiled functions), DTW k-NN prediction times were indeed reduced drastically.
-        
-        I would like to thank Prof. Eamonn Keogh for directly reaching out to me regarding this finding.
-        
-        ## References
-        
-        <table>
-          <tbody>
-            <tr>
-              <td>[1]</td>
-              <td>
-                <a href=https://web.ece.ucsb.edu/Faculty/Rabiner/ece259/Reprints/tutorial%20on%20hmm%20and%20applications.pdf">Lawrence R. Rabiner. <b>"A Tutorial on Hidden Markov Models and Selected Applications in Speech Recognition"</b> <em>Proceedings of the IEEE 77 (1989)</em>, no. 2, 257-86.</a>
-              </td>
-            </tr>
-            <tr>
-              <td>[2]</td>
-              <td>
-                <a href="https://pdfs.semanticscholar.org/05a2/0cde15e172fc82f32774dd0cf4fe5827cad2.pdf">Stan Salvador & Philip Chan. <b>"FastDTW: Toward accurate dynamic time warping in linear time and space."</b> <em>Intelligent Data Analysis 11.5 (2007)</em>, 561-580.</a>
-              </td>
-            </tr>
-            <tr>
-              <td>[3]</td>
-              <td>
-                <a href="https://arxiv.org/ftp/arxiv/papers/2003/2003.11246.pdf">Renjie Wu & Eamonn J. Keogh. <b>"FastDTW is approximate and Generally Slower than the Algorithm it Approximates"</b> <em>IEEE Transactions on Knowledge and Data Engineering (2020)</em>, 1–1.</a>
-              </td>
-            </tr>
-          </tbody>
-        </table>
-        
-        ## Contributors
-        
-        All contributions to this repository are greatly appreciated. Contribution guidelines can be found [here](/CONTRIBUTING.md).
-        
-        <table>
-        	<thead>
-        		<tr>
-        			<th align="center">
-                <a href="https://github.com/eonu">
-                  <img src="https://avatars0.githubusercontent.com/u/24795571?s=460&v=4" alt="eonu" width="60px">
-                  <br/><sub><b>eonu</b></sub>
-                </a>
-        			</th>
-              <th align="center">
-                <a href="https://github.com/Prhmma">
-                  <img src="https://avatars0.githubusercontent.com/u/16954887?s=460&v=4" alt="Prhmma" width="60px">
-                  <br/><sub><b>Prhmma</b></sub>
-                </a>
-        			</th>
-              <th align="center">
-                <a href="https://github.com/manisci">
-                  <img src="https://avatars.githubusercontent.com/u/30268711?v=4" alt="manisci" width="60px">
-                  <br/><sub><b>manisci</b></sub>
-                </a>
-              </th>
-              <th align="center">
-                <a href="https://github.com/jonnor">
-                  <img src="https://avatars.githubusercontent.com/u/45185?v=4" alt="jonnor" width="60px">
-                  <br/><sub><b>jonnor</b></sub>
-                </a>
-              </th>
-        			<!-- Add more <th></th> blocks for more contributors -->
-        		</tr>
-        	</thead>
-        </table>
-        
-        ## Licensing
-        
-        Sequentia is released under the [MIT](https://opensource.org/licenses/MIT) license.
-        
-        Certain parts of the source code are heavily adapted from [Scikit-Learn](scikit-learn.org/).
-        Such files contain copy of [their license](https://github.com/scikit-learn/scikit-learn/blob/main/COPYING).
-        
-        ---
-        
-        <p align="center">
-          <b>Sequentia</b> &copy; 2019-2023, Edwin Onuonga - Released under the <a href="https://opensource.org/licenses/MIT">MIT</a> license.<br/>
-          <em>Authored and maintained by Edwin Onuonga.</em>
-        </p>
-Platform: UNKNOWN
+Maintainer: Edwin Onuonga
+Maintainer-email: ed@eonu.net
+Requires-Python: >=3.11,<4.0
 Classifier: Development Status :: 5 - Production/Stable
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: Unix
-Classifier: Operating System :: MacOS
+Classifier: Environment :: Console
+Classifier: Framework :: Pydantic :: 2
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: Science/Research
-Classifier: Topic :: Software Development
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Scientific/Engineering
-Classifier: Natural Language :: English
-Requires-Python: >=3.8
+Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: Typing :: Typed
+Requires-Dist: dtaidistance (>=2.3.10,<3.0.0)
+Requires-Dist: hmmlearn (>=0.2.8,<1)
+Requires-Dist: joblib (>=1.2,<2.0)
+Requires-Dist: numba (>=0.56,<1)
+Requires-Dist: numpy (>=1.19.5,<2.0.0)
+Requires-Dist: pydantic (>=2,<3)
+Requires-Dist: scikit-learn (>=1.4,<2.0)
+Requires-Dist: scipy (>=1.6,<2.0)
+Project-URL: Documentation, https://sequentia.readthedocs.io/en/latest
+Project-URL: Repository, https://github.com/eonu/sequentia
 Description-Content-Type: text/markdown
-Provides-Extra: dev
+
+<p align="center">
+  <h1 align="center">
+    <img src="https://raw.githubusercontent.com/eonu/sequentia/master/docs/source/_static/images/logo.png" width="75px"><br/>
+    Sequentia
+  </h1>
+</p>
+
+<p align="center">
+  <em>Scikit-Learn compatible HMM and DTW based sequence machine learning algorithms in Python.</em>
+</p>
+
+<p align="center">
+  <div align="center">
+    <a href="https://pypi.org/project/sequentia">
+      <img src="https://img.shields.io/pypi/v/sequentia?logo=pypi&style=flat-square" alt="PyPI"/>
+    </a>
+    <a href="https://pypi.org/project/sequentia">
+      <img src="https://img.shields.io/pypi/pyversions/sequentia?logo=python&style=flat-square" alt="PyPI - Python Version"/>
+    </a>
+    <a href="https://sequentia.readthedocs.io/en/latest">
+      <img src="https://img.shields.io/readthedocs/sequentia.svg?logo=read-the-docs&style=flat-square" alt="Read The Docs - Documentation">
+    </a>
+    <a href="https://coveralls.io/github/eonu/sequentia">
+      <img src="https://img.shields.io/coverallsCoverage/github/eonu/sequentia?logo=coveralls&style=flat-square" alt="Coveralls - Coverage"/>
+    </a>
+    <a href="https://raw.githubusercontent.com/eonu/sequentia/master/LICENSE">
+      <img src="https://img.shields.io/pypi/l/sequentia?style=flat-square" alt="PyPI - License"/>
+    </a>
+  </div>
+</p>
+
+<p align="center">
+  <sup>
+    <a href="#about">About</a> ·
+    <a href="#build-status">Build Status</a> ·
+    <a href="#features">Features</a> ·
+    <a href="#documentation">Documentation</a> ·
+    <a href="#examples">Examples</a> ·
+    <a href="#acknowledgments">Acknowledgments</a> ·
+    <a href="#references">References</a> ·
+    <a href="#contributors">Contributors</a> ·
+    <a href="#licensing">Licensing</a>
+  </sup>
+</p>
+
+## About
+
+Sequentia is a Python package that provides various classification and regression algorithms for sequential data, including methods based on hidden Markov models and dynamic time warping.
+
+Some examples of how Sequentia can be used on sequence data include:
+
+- determining a spoken word based on its audio signal or alternative representations such as MFCCs,
+- predicting motion intent for gesture control from sEMG signals,
+- classifying hand-written characters according to their pen-tip trajectories.
+
+### Why Sequentia?
+
+- **Simplicity and interpretability**: Sequentia offers a limited set of machine learning algorithms, chosen specifically to be more interpretable and easier to configure than more complex alternatives such as recurrent neural networks and transformers, while maintaining a high level of effectiveness.
+- **Familiar and user-friendly**: To fit more seamlessly into the workflow of data science practitioners, Sequentia follows the ubiquitous Scikit-Learn API, providing a familiar model development process for many, as well as enabling wider access to the rapidly growing Scikit-Learn ecosystem.
+
+## Build Status
+
+| `master`                                                                                                                                                                                                 | `dev`                                                                                                                                                                                                      |
+| -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
+| [![CircleCI Build (Master)](https://img.shields.io/circleci/build/github/eonu/sequentia/master?logo=circleci&style=flat-square)](https://app.circleci.com/pipelines/github/eonu/sequentia?branch=master) | [![CircleCI Build (Development)](https://img.shields.io/circleci/build/github/eonu/sequentia/dev?logo=circleci&style=flat-square)](https://app.circleci.com/pipelines/github/eonu/sequentia?branch=master) |
+
+## Features
+
+### Models
+
+The following models provided by Sequentia all support variable length sequences.
+
+#### [Dynamic Time Warping + k-Nearest Neighbors](https://sequentia.readthedocs.io/en/latest/sections/models/knn/index.html) (via [`dtaidistance`](https://github.com/wannesm/dtaidistance))
+
+- [x] Classification
+- [x] Regression
+- [x] Multivariate real-valued observations
+- [x] Sakoe–Chiba band global warping constraint
+- [x] Dependent and independent feature warping (DTWD/DTWI)
+- [x] Custom distance-weighted predictions
+- [x] Multi-processed predictions
+
+#### [Hidden Markov Models](https://sequentia.readthedocs.io/en/latest/sections/models/hmm/index.html) (via [`hmmlearn`](https://github.com/hmmlearn/hmmlearn))
+
+Parameter estimation with the Baum-Welch algorithm and prediction with the forward algorithm [[1]](#references)
+
+- [x] Classification
+- [x] Multivariate real-valued observations (Gaussian mixture model emissions)
+- [x] Univariate categorical observations (discrete emissions)
+- [x] Linear, left-right and ergodic topologies
+- [x] Multi-processed predictions
+
+### Scikit-Learn compatibility
+
+**Sequentia (≥2.0) is fully compatible with the Scikit-Learn API (≥1.4), enabling for rapid development and prototyping of sequential models.**
+
+In most cases, the only necessary change is to add a `lengths` key-word argument to provide sequence length information, e.g. `fit(X, y, lengths=lengths)` instead of `fit(X, y)`.
+
+## Installation
+
+The latest stable version of Sequentia can be installed with the following command:
+
+```console
+pip install sequentia
+```
+
+### C library compilation
+
+For optimal performance when using any of the k-NN based models, it is important that `dtaidistance` C libraries are compiled correctly.
+
+Please see the [`dtaidistance` installation guide](https://dtaidistance.readthedocs.io/en/latest/usage/installation.html) for troubleshooting if you run into C compilation issues, or if setting `use_c=True` on k-NN based models results in a warning.
+
+You can use the following to check if the appropriate C libraries have been installed.
+
+```python
+from dtaidistance import dtw
+dtw.try_import_c()
+```
+
+### Development
+
+Please see the [contribution guidelines](/CONTRIBUTING.md) to see installation instructions for contributing to Sequentia.
+
+## Documentation
+
+Documentation for the package is available on [Read The Docs](https://sequentia.readthedocs.io/en/latest).
+
+## Examples
+
+Demonstration of classifying multivariate sequences with two features into two classes using the `KNNClassifier`.
+
+This example also shows a typical preprocessing workflow, as well as compatibility with Scikit-Learn.
+
+```python
+import numpy as np
+
+from sklearn.preprocessing import scale
+from sklearn.decomposition import PCA
+from sklearn.pipeline import Pipeline
+
+from sequentia.models import KNNClassifier
+from sequentia.preprocessing import IndependentFunctionTransformer, median_filter
+
+# Create input data
+# - Sequentia expects sequences to be concatenated into a single array
+# - Sequence lengths are provided separately and used to decode the sequences when needed
+# - This avoids the need for complex structures such as lists of arrays with different lengths
+
+# Sequences
+X = np.array([
+    # Sequence 1 - Length 3
+    [1.2 , 7.91],
+    [1.34, 6.6 ],
+    [0.92, 8.08],
+    # Sequence 2 - Length 5
+    [2.11, 6.97],
+    [1.83, 7.06],
+    [1.54, 5.98],
+    [0.86, 6.37],
+    [1.21, 5.8 ],
+    # Sequence 3 - Length 2
+    [1.7 , 6.22],
+    [2.01, 5.49],
+])
+
+# Sequence lengths
+lengths = np.array([3, 5, 2])
+
+# Sequence classes
+y = np.array([0, 1, 1])
+
+# Create a transformation pipeline that feeds into a KNNClassifier
+# 1. Individually denoise each sequence by applying a median filter for each feature
+# 2. Individually standardize each sequence by subtracting the mean and dividing the s.d. for each feature
+# 3. Reduce the dimensionality of the data to a single feature by using PCA
+# 4. Pass the resulting transformed data into a KNNClassifier
+pipeline = Pipeline([
+    ('denoise', IndependentFunctionTransformer(median_filter)),
+    ('scale', IndependentFunctionTransformer(scale)),
+    ('pca', PCA(n_components=1)),
+    ('knn', KNNClassifier(k=1))
+])
+
+# Fit the pipeline to the data - lengths must be provided
+pipeline.fit(X, y, lengths=lengths)
+
+# Predict classes for the sequences and calculate accuracy - lengths must be provided
+y_pred = pipeline.predict(X, lengths=lengths)
+acc = pipeline.score(X, y, lengths=lengths)
+```
+
+## Acknowledgments
+
+In earlier versions of the package, an approximate DTW implementation [`fastdtw`](https://github.com/slaypni/fastdtw) was used in hopes of speeding up k-NN predictions, as the authors of the original FastDTW paper [[2]](#references) claim that approximated DTW alignments can be computed in linear memory and time, compared to the O(N<sup>2</sup>) runtime complexity of the usual exact DTW implementation.
+
+I was contacted by [Prof. Eamonn Keogh](https://www.cs.ucr.edu/~eamonn/) whose work makes the surprising revelation that FastDTW is generally slower than the exact DTW algorithm that it approximates [[3]](#references). Upon switching from the `fastdtw` package to [`dtaidistance`](https://github.com/wannesm/dtaidistance) (a very solid implementation of exact DTW with fast pure C compiled functions), DTW k-NN prediction times were indeed reduced drastically.
+
+I would like to thank Prof. Eamonn Keogh for directly reaching out to me regarding this finding.
+
+## References
+
+<table>
+  <tbody>
+    <tr>
+      <td>[1]</td>
+      <td>
+        <a href=https://web.ece.ucsb.edu/Faculty/Rabiner/ece259/Reprints/tutorial%20on%20hmm%20and%20applications.pdf">Lawrence R. Rabiner. <b>"A Tutorial on Hidden Markov Models and Selected Applications in Speech Recognition"</b> <em>Proceedings of the IEEE 77 (1989)</em>, no. 2, 257-86.</a>
+      </td>
+    </tr>
+    <tr>
+      <td>[2]</td>
+      <td>
+        <a href="https://pdfs.semanticscholar.org/05a2/0cde15e172fc82f32774dd0cf4fe5827cad2.pdf">Stan Salvador & Philip Chan. <b>"FastDTW: Toward accurate dynamic time warping in linear time and space."</b> <em>Intelligent Data Analysis 11.5 (2007)</em>, 561-580.</a>
+      </td>
+    </tr>
+    <tr>
+      <td>[3]</td>
+      <td>
+        <a href="https://arxiv.org/ftp/arxiv/papers/2003/2003.11246.pdf">Renjie Wu & Eamonn J. Keogh. <b>"FastDTW is approximate and Generally Slower than the Algorithm it Approximates"</b> <em>IEEE Transactions on Knowledge and Data Engineering (2020)</em>, 1–1.</a>
+      </td>
+    </tr>
+  </tbody>
+</table>
+
+## Contributors
+
+All contributions to this repository are greatly appreciated. Contribution guidelines can be found [here](/CONTRIBUTING.md).
+
+<table>
+	<thead>
+		<tr>
+			<th align="center">
+        <a href="https://github.com/eonu">
+          <img src="https://avatars0.githubusercontent.com/u/24795571?s=460&v=4" alt="eonu" width="60px">
+          <br/><sub><b>eonu</b></sub>
+        </a>
+			</th>
+      <th align="center">
+        <a href="https://github.com/Prhmma">
+          <img src="https://avatars0.githubusercontent.com/u/16954887?s=460&v=4" alt="Prhmma" width="60px">
+          <br/><sub><b>Prhmma</b></sub>
+        </a>
+			</th>
+      <th align="center">
+        <a href="https://github.com/manisci">
+          <img src="https://avatars.githubusercontent.com/u/30268711?v=4" alt="manisci" width="60px">
+          <br/><sub><b>manisci</b></sub>
+        </a>
+      </th>
+      <th align="center">
+        <a href="https://github.com/jonnor">
+          <img src="https://avatars.githubusercontent.com/u/45185?v=4" alt="jonnor" width="60px">
+          <br/><sub><b>jonnor</b></sub>
+        </a>
+      </th>
+			<!-- Add more <th></th> blocks for more contributors -->
+		</tr>
+	</thead>
+</table>
+
+## Licensing
+
+Sequentia is released under the [MIT](https://opensource.org/licenses/MIT) license.
+
+Certain parts of the source code are heavily adapted from [Scikit-Learn](scikit-learn.org/).
+Such files contain a copy of [their license](https://github.com/scikit-learn/scikit-learn/blob/main/COPYING).
+
+---
+
+<p align="center">
+  <b>Sequentia</b> &copy; 2019-2025, Edwin Onuonga - Released under the <a href="https://opensource.org/licenses/MIT">MIT</a> license.<br/>
+  <em>Authored and maintained by Edwin Onuonga.</em>
+</p>
+
```

#### html2text {}

```diff
@@ -1,30 +1,64 @@
-Metadata-Version: 2.1 Name: sequentia Version: 1.1.1 Summary: HMM and DTW-based
-sequence machine learning algorithms in Python following an sklearn-like
-interface. Home-page: https://github.com/eonu/sequentia Author: Edwin Onuonga
-Author-email: ed@eonu.net License: MIT Project-URL: Documentation, https://
-sequentia.readthedocs.io/en/latest Project-URL: Bug Tracker, https://
-github.com/eonu/sequentia/issues Project-URL: Source Code, https://github.com/
-eonu/sequentia Description:
- ************ [[hhttttppss::////rraaww..ggiitthhuubbuusseerrccoonntteenntt..ccoomm//eeoonnuu//sseeqquueennttiiaa//mmaasstteerr//ddooccss//__ssttaattiicc//
-                               iimmaaggeess//llooggoo..ppnngg]]
+Metadata-Version: 2.1 Name: sequentia Version: 2.0.0 Summary: Scikit-Learn
+compatible HMM and DTW based sequence machine learning algorithms in Python.
+Home-page: https://github.com/eonu/sequentia License: MIT Keywords:
+python,machine-learning,time-series,hmm,hidden-markov-models,dtw,dynamic-time-
+warping,knn,k-nearest-neighbors,sequence-classification,time-series-
+classification,multivariate-time-series,variable-length,classification-
+algorithms Author: Edwin Onuonga Author-email: ed@eonu.net Maintainer: Edwin
+Onuonga Maintainer-email: ed@eonu.net Requires-Python: >=3.11,<4.0 Classifier:
+Development Status :: 5 - Production/Stable Classifier: Environment :: Console
+Classifier: Framework :: Pydantic :: 2 Classifier: Intended Audience ::
+Developers Classifier: Intended Audience :: Information Technology Classifier:
+Intended Audience :: Science/Research Classifier: License :: OSI Approved ::
+MIT License Classifier: Operating System :: OS Independent Classifier:
+Programming Language :: Python Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.11 Classifier: Programming
+Language :: Python :: 3.12 Classifier: Programming Language :: Python :: 3 ::
+Only Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Topic :: Scientific/Engineering Classifier: Topic :: Scientific/
+Engineering :: Artificial Intelligence Classifier: Topic :: Software
+Development :: Libraries :: Python Modules Classifier: Typing :: Typed
+Requires-Dist: dtaidistance (>=2.3.10,<3.0.0) Requires-Dist: hmmlearn
+(>=0.2.8,<1) Requires-Dist: joblib (>=1.2,<2.0) Requires-Dist: numba
+(>=0.56,<1) Requires-Dist: numpy (>=1.19.5,<2.0.0) Requires-Dist: pydantic
+(>=2,<3) Requires-Dist: scikit-learn (>=1.4,<2.0) Requires-Dist: scipy
+(>=1.6,<2.0) Project-URL: Documentation, https://sequentia.readthedocs.io/en/
+latest Project-URL: Repository, https://github.com/eonu/sequentia Description-
+Content-Type: text/markdown
+ ************ [[hhttttppss::////rraaww..ggiitthhuubbuusseerrccoonntteenntt..ccoomm//eeoonnuu//sseeqquueennttiiaa//mmaasstteerr//ddooccss//ssoouurrccee//
+                           __ssttaattiicc//iimmaaggeess//llooggoo..ppnngg]]
                                SSeeqquueennttiiaa ************
- HHMMMM aanndd DDTTWW--bbaasseedd sseeqquueennccee mmaacchhiinnee lleeaarrnniinngg aallggoorriitthhmmss iinn PPyytthhoonn ffoolllloowwiinngg aann
-                            sskklleeaarrnn--lliikkee iinntteerrffaaccee..
- _[_P_y_P_I_]_[_P_y_P_I_ _-_ _P_y_t_h_o_n_ _V_e_r_s_i_o_n_]_[_R_e_a_d_ _T_h_e_ _D_o_c_s_ _-_ _D_o_c_u_m_e_n_t_a_t_i_o_n_]_[_P_y_P_I_ _-_ _L_i_c_e_n_s_e_]
+SScciikkiitt--LLeeaarrnn ccoommppaattiibbllee HHMMMM aanndd DDTTWW bbaasseedd sseeqquueennccee mmaacchhiinnee lleeaarrnniinngg aallggoorriitthhmmss
+                                  iinn PPyytthhoonn..
+   _[_P_y_P_I_]_[_P_y_P_I_ _-_ _P_y_t_h_o_n_ _V_e_r_s_i_o_n_]_[_R_e_a_d_ _T_h_e_ _D_o_c_s_ _-_ _D_o_c_u_m_e_n_t_a_t_i_o_n_]_[_C_o_v_e_r_a_l_l_s_ _-
+                           _C_o_v_e_r_a_g_e_]_[_P_y_P_I_ _-_ _L_i_c_e_n_s_e_]
        _A_b_o_u_t Â· _B_u_i_l_d_ _S_t_a_t_u_s Â· _F_e_a_t_u_r_e_s Â· _D_o_c_u_m_e_n_t_a_t_i_o_n Â· _E_x_a_m_p_l_e_s Â·
           _A_c_k_n_o_w_l_e_d_g_m_e_n_t_s Â· _R_e_f_e_r_e_n_c_e_s Â· _C_o_n_t_r_i_b_u_t_o_r_s Â· _L_i_c_e_n_s_i_n_g
 ## About Sequentia is a Python package that provides various classification and
 regression algorithms for sequential data, including methods based on hidden
 Markov models and dynamic time warping. Some examples of how Sequentia can be
 used on sequence data include: - determining a spoken word based on its audio
 signal or alternative representations such as MFCCs, - predicting motion intent
 for gesture control from sEMG signals, - classifying hand-written characters
-according to their pen-tip trajectories. ## Build Status | `master` | `dev` | |
--------- | ------| | [![CircleCI Build (Master)](https://img.shields.io/
+according to their pen-tip trajectories. ### Why Sequentia? - **Simplicity and
+interpretability**: Sequentia offers a limited set of machine learning
+algorithms, chosen specifically to be more interpretable and easier to
+configure than more complex alternatives such as recurrent neural networks and
+transformers, while maintaining a high level of effectiveness. - **Familiar and
+user-friendly**: To fit more seamlessly into the workflow of data science
+practitioners, Sequentia follows the ubiquitous Scikit-Learn API, providing a
+familiar model development process for many, as well as enabling wider access
+to the rapidly growing Scikit-Learn ecosystem. ## Build Status | `master` |
+`dev` | | ---------------------------------------------------------------------
+-------------------------------------------------------------------------------
+---------------------------------------------------- | ------------------------
+-------------------------------------------------------------------------------
+-------------------------------------------------------------------------------
+-------------------- | | [![CircleCI Build (Master)](https://img.shields.io/
 circleci/build/github/eonu/sequentia/master?logo=circleci&style=flat-square)]
 (https://app.circleci.com/pipelines/github/eonu/sequentia?branch=master) | [!
 [CircleCI Build (Development)](https://img.shields.io/circleci/build/github/
 eonu/sequentia/dev?logo=circleci&style=flat-square)](https://app.circleci.com/
 pipelines/github/eonu/sequentia?branch=master) | ## Features ### Models The
 following models provided by Sequentia all support variable length sequences.
 #### [Dynamic Time Warping + k-Nearest Neighbors](https://
@@ -36,115 +70,83 @@
 Multi-processed predictions #### [Hidden Markov Models](https://
 sequentia.readthedocs.io/en/latest/sections/models/hmm/index.html) (via
 [`hmmlearn`](https://github.com/hmmlearn/hmmlearn)) Parameter estimation with
 the Baum-Welch algorithm and prediction with the forward algorithm [[1]]
 (#references) - [x] Classification - [x] Multivariate real-valued observations
 (Gaussian mixture model emissions) - [x] Univariate categorical observations
 (discrete emissions) - [x] Linear, left-right and ergodic topologies - [x]
-Multi-processed predictions ### Scikit-Learn compatibility Sequentia aims to
-follow the Scikit-Learn interface for estimators and transformations, as well
-as to be largely compatible with three core Scikit-Learn modules to improve the
-ease of model development: [`preprocessing`](https://scikit-learn.org/stable/
-modules/classes.html#module-sklearn.preprocessing), [`model_selection`](https:/
-/scikit-learn.org/stable/modules/classes.html#module-sklearn.model_selection)
-and [`pipeline`](https://scikit-learn.org/stable/modules/classes.html#module-
-sklearn.pipeline). While there are many other modules, maintaining full
-compatibility with Scikit-Learn is challenging and many of its features are
-inapplicable to sequential data, therefore we only focus on the relevant core
-modules. Despite some deviation from the Scikit-Learn interface in order to
-accommodate sequences, the following features are currently compatible with
-Sequentia. - [x] [`preprocessing`](https://scikit-learn.org/stable/modules/
-classes.html#module-sklearn.preprocessing) - [x] [`FunctionTransformer`](https:
-//scikit-learn.org/stable/modules/generated/
-sklearn.preprocessing.FunctionTransformer.html#sklearn.preprocessing.FunctionTransformer)
-â via an adapted class definition - [x] Function-based transformations
-(stateless) - [x] Class-based transformations (stateful) - [ ] [`pipeline`]
-(https://scikit-learn.org/stable/modules/classes.html#module-sklearn.pipeline)
-- [x] [`Pipeline`](https://scikit-learn.org/stable/modules/generated/
-sklearn.pipeline.Pipeline.html#sklearn.pipeline.Pipeline) â via an adapted
-class definition - [ ] [`FeatureUnion`](https://scikit-learn.org/stable/
-modules/generated/
-sklearn.pipeline.FeatureUnion.html#sklearn.pipeline.FeatureUnion) - [ ]
-[`model_selection`](https://scikit-learn.org/stable/modules/
-classes.html#module-sklearn.model_selection) ## Installation You can install
-Sequentia using `pip`. ### Stable The latest stable version of Sequentia can be
-installed with the following command. ```console pip install sequentia ``` ####
-C library compilation For optimal performance when using any of the k-NN based
-models, it is important that `dtaidistance` C libraries are compiled correctly.
-Please see the [`dtaidistance` installation guide](https://
-dtaidistance.readthedocs.io/en/latest/usage/installation.html) for
-troubleshooting if you run into C compilation issues, or if setting
-`use_c=True` on k-NN based models results in a warning. You can use the
-following to check if the appropriate C libraries have been installed.
-```python from dtaidistance import dtw dtw.try_import_c() ``` ### Pre-release
-Pre-release versions include new features which are in active development and
-may change unpredictably. The latest pre-release version can be installed with
-the following command. ```console pip install --pre sequentia ``` ###
-Development Please see the [contribution guidelines](/CONTRIBUTING.md) to see
-installation instructions for contributing to Sequentia. ## Documentation
-Documentation for the package is available on [Read The Docs](https://
-sequentia.readthedocs.io/en/latest). ## Examples Demonstration of classifying
-multivariate sequences with two features into two classes using the
+Multi-processed predictions ### Scikit-Learn compatibility **Sequentia (â¥2.0)
+is fully compatible with the Scikit-Learn API (â¥1.4), enabling for rapid
+development and prototyping of sequential models.** In most cases, the only
+necessary change is to add a `lengths` key-word argument to provide sequence
+length information, e.g. `fit(X, y, lengths=lengths)` instead of `fit(X, y)`.
+## Installation The latest stable version of Sequentia can be installed with
+the following command: ```console pip install sequentia ``` ### C library
+compilation For optimal performance when using any of the k-NN based models, it
+is important that `dtaidistance` C libraries are compiled correctly. Please see
+the [`dtaidistance` installation guide](https://dtaidistance.readthedocs.io/en/
+latest/usage/installation.html) for troubleshooting if you run into C
+compilation issues, or if setting `use_c=True` on k-NN based models results in
+a warning. You can use the following to check if the appropriate C libraries
+have been installed. ```python from dtaidistance import dtw dtw.try_import_c()
+``` ### Development Please see the [contribution guidelines](/CONTRIBUTING.md)
+to see installation instructions for contributing to Sequentia. ##
+Documentation Documentation for the package is available on [Read The Docs]
+(https://sequentia.readthedocs.io/en/latest). ## Examples Demonstration of
+classifying multivariate sequences with two features into two classes using the
 `KNNClassifier`. This example also shows a typical preprocessing workflow, as
 well as compatibility with Scikit-Learn. ```python import numpy as np from
 sklearn.preprocessing import scale from sklearn.decomposition import PCA from
-sequentia.models import KNNClassifier from sequentia.pipeline import Pipeline
-from sequentia.preprocessing import IndependentFunctionTransformer, mean_filter
-# Create input data # - Sequentia expects sequences to be concatenated into a
-single array # - Sequence lengths are provided separately and used to decode
-the sequences when needed # - This avoids the need for complex structures such
-as lists of arrays with different lengths # Sequences X = np.array([ # Sequence
-1 - Length 3 [1.2 , 7.91], [1.34, 6.6 ], [0.92, 8.08], # Sequence 2 - Length 5
-[2.11, 6.97], [1.83, 7.06], [1.54, 5.98], [0.86, 6.37], [1.21, 5.8 ], #
-Sequence 3 - Length 2 [1.7 , 6.22], [2.01, 5.49] ]) # Sequence lengths lengths
-= np.array([3, 5, 2]) # Sequence classes y = np.array([0, 1, 1]) # Create a
-transformation pipeline that feeds into a KNNClassifier # 1. Individually
-denoise each sequence by applying a mean filter for each feature # 2.
-Individually standardize each sequence by subtracting the mean and dividing the
-s.d. for each feature # 3. Reduce the dimensionality of the data to a single
-feature by using PCA # 4. Pass the resulting transformed data into a
-KNNClassifier pipeline = Pipeline([ ('denoise', IndependentFunctionTransformer
-(mean_filter)), ('scale', IndependentFunctionTransformer(scale)), ('pca', PCA
-(n_components=1)), ('knn', KNNClassifier(k=1)) ]) # Fit the pipeline to the
-data - lengths must be provided pipeline.fit(X, y, lengths) # Predict classes
-for the sequences and calculate accuracy - lengths must be provided y_pred =
-pipeline.predict(X, lengths) acc = pipeline.score(X, y, lengths) ``` ##
-Acknowledgments In earlier versions of the package, an approximate DTW
-implementation [`fastdtw`](https://github.com/slaypni/fastdtw) was used in
-hopes of speeding up k-NN predictions, as the authors of the original FastDTW
-paper [[2]](#references) claim that approximated DTW alignments can be computed
-in linear memory and time, compared to the O(N2) runtime complexity of the
-usual exact DTW implementation. I was contacted by [Prof. Eamonn Keogh](https:/
-/www.cs.ucr.edu/~eamonn/) whose work makes the surprising revelation that
-FastDTW is generally slower than the exact DTW algorithm that it approximates [
-[3]](#references). Upon switching from the `fastdtw` package to
-[`dtaidistance`](https://github.com/wannesm/dtaidistance) (a very solid
-implementation of exact DTW with fast pure C compiled functions), DTW k-NN
-prediction times were indeed reduced drastically. I would like to thank Prof.
-Eamonn Keogh for directly reaching out to me regarding this finding. ##
-References
+sklearn.pipeline import Pipeline from sequentia.models import KNNClassifier
+from sequentia.preprocessing import IndependentFunctionTransformer,
+median_filter # Create input data # - Sequentia expects sequences to be
+concatenated into a single array # - Sequence lengths are provided separately
+and used to decode the sequences when needed # - This avoids the need for
+complex structures such as lists of arrays with different lengths # Sequences X
+= np.array([ # Sequence 1 - Length 3 [1.2 , 7.91], [1.34, 6.6 ], [0.92, 8.08],
+# Sequence 2 - Length 5 [2.11, 6.97], [1.83, 7.06], [1.54, 5.98], [0.86, 6.37],
+[1.21, 5.8 ], # Sequence 3 - Length 2 [1.7 , 6.22], [2.01, 5.49], ]) # Sequence
+lengths lengths = np.array([3, 5, 2]) # Sequence classes y = np.array([0, 1,
+1]) # Create a transformation pipeline that feeds into a KNNClassifier # 1.
+Individually denoise each sequence by applying a median filter for each feature
+# 2. Individually standardize each sequence by subtracting the mean and
+dividing the s.d. for each feature # 3. Reduce the dimensionality of the data
+to a single feature by using PCA # 4. Pass the resulting transformed data into
+a KNNClassifier pipeline = Pipeline([ ('denoise',
+IndependentFunctionTransformer(median_filter)), ('scale',
+IndependentFunctionTransformer(scale)), ('pca', PCA(n_components=1)), ('knn',
+KNNClassifier(k=1)) ]) # Fit the pipeline to the data - lengths must be
+provided pipeline.fit(X, y, lengths=lengths) # Predict classes for the
+sequences and calculate accuracy - lengths must be provided y_pred =
+pipeline.predict(X, lengths=lengths) acc = pipeline.score(X, y,
+lengths=lengths) ``` ## Acknowledgments In earlier versions of the package, an
+approximate DTW implementation [`fastdtw`](https://github.com/slaypni/fastdtw)
+was used in hopes of speeding up k-NN predictions, as the authors of the
+original FastDTW paper [[2]](#references) claim that approximated DTW
+alignments can be computed in linear memory and time, compared to the O(N2)
+runtime complexity of the usual exact DTW implementation. I was contacted by
+[Prof. Eamonn Keogh](https://www.cs.ucr.edu/~eamonn/) whose work makes the
+surprising revelation that FastDTW is generally slower than the exact DTW
+algorithm that it approximates [[3]](#references). Upon switching from the
+`fastdtw` package to [`dtaidistance`](https://github.com/wannesm/dtaidistance)
+(a very solid implementation of exact DTW with fast pure C compiled functions),
+DTW k-NN prediction times were indeed reduced drastically. I would like to
+thank Prof. Eamonn Keogh for directly reaching out to me regarding this
+finding. ## References
     _L_a_w_r_e_n_c_e_ _R_._ _R_a_b_i_n_e_r_._ _""_AA_ _TT_uu_tt_oo_rr_ii_aa_ll_ _oo_nn_ _HH_ii_dd_dd_ee_nn_ _MM_aa_rr_kk_oo_vv_ _MM_oo_dd_ee_ll_ss_ _aa_nn_dd_ _SS_ee_ll_ee_cc_tt_ee_dd
 [1] _AA_pp_pp_ll_ii_cc_aa_tt_ii_oo_nn_ss_ _ii_nn_ _SS_pp_ee_ee_cc_hh_ _RR_ee_cc_oo_gg_nn_ii_tt_ii_oo_nn_""_ _PP_rr_oo_cc_ee_ee_dd_ii_nn_gg_ss_ _oo_ff_ _tt_hh_ee_ _II_EE_EE_EE_ _77_77_ _((_11_99_88_99_))_,_ _n_o_.
     _2_,_ _2_5_7_-_8_6_.
 [2] _S_t_a_n_ _S_a_l_v_a_d_o_r_ _&_ _P_h_i_l_i_p_ _C_h_a_n_._ _""_FF_aa_ss_tt_DD_TT_WW_::_ _TT_oo_ww_aa_rr_dd_ _aa_cc_cc_uu_rr_aa_tt_ee_ _dd_yy_nn_aa_mm_ii_cc_ _tt_ii_mm_ee_ _ww_aa_rr_pp_ii_nn_gg
     _ii_nn_ _ll_ii_nn_ee_aa_rr_ _tt_ii_mm_ee_ _aa_nn_dd_ _ss_pp_aa_cc_ee_.._""_ _II_nn_tt_ee_ll_ll_ii_gg_ee_nn_tt_ _DD_aa_tt_aa_ _AA_nn_aa_ll_yy_ss_ii_ss_ _11_11_.._55_ _((_22_00_00_77_))_,_ _5_6_1_-_5_8_0_.
     _R_e_n_j_i_e_ _W_u_ _&_ _E_a_m_o_n_n_ _J_._ _K_e_o_g_h_._ _""_FF_aa_ss_tt_DD_TT_WW_ _ii_ss_ _aa_pp_pp_rr_oo_xx_ii_mm_aa_tt_ee_ _aa_nn_dd_ _GG_ee_nn_ee_rr_aa_ll_ll_yy_ _SS_ll_oo_ww_ee_rr
 [3] _tt_hh_aa_nn_ _tt_hh_ee_ _AA_ll_gg_oo_rr_ii_tt_hh_mm_ _ii_tt_ _AA_pp_pp_rr_oo_xx_ii_mm_aa_tt_ee_ss_""_ _II_EE_EE_EE_ _TT_rr_aa_nn_ss_aa_cc_tt_ii_oo_nn_ss_ _oo_nn_ _KK_nn_oo_ww_ll_ee_dd_gg_ee_ _aa_nn_dd_ _DD_aa_tt_aa
     _EE_nn_gg_ii_nn_ee_ee_rr_ii_nn_gg_ _((_22_00_22_00_))_,_ _1_â___1_.
 ## Contributors All contributions to this repository are greatly appreciated.
 Contribution guidelines can be found [here](/CONTRIBUTING.md).
 _[[_ee_oo_nn_uu_]] _[[_PP_rr_hh_mm_mm_aa_]] _[[_mm_aa_nn_ii_ss_cc_ii_]] _[[_jj_oo_nn_nn_oo_rr_]]
  _ee_oo_nn_uu   _PP_rr_hh_mm_mm_aa   _mm_aa_nn_ii_ss_cc_ii   _jj_oo_nn_nn_oo_rr
 ## Licensing Sequentia is released under the [MIT](https://opensource.org/
 licenses/MIT) license. Certain parts of the source code are heavily adapted
-from [Scikit-Learn](scikit-learn.org/). Such files contain copy of [their
+from [Scikit-Learn](scikit-learn.org/). Such files contain a copy of [their
 license](https://github.com/scikit-learn/scikit-learn/blob/main/COPYING). ---
-    SSeeqquueennttiiaa © 2019-2023, Edwin Onuonga - Released under the _M_I_T license.
+    SSeeqquueennttiiaa © 2019-2025, Edwin Onuonga - Released under the _M_I_T license.
                    AAuutthhoorreedd aanndd mmaaiinnttaaiinneedd bbyy EEddwwiinn OOnnuuoonnggaa..
-Platform: UNKNOWN Classifier: Development Status :: 5 - Production/Stable
-Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
-Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
-Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
-:: Unix Classifier: Operating System :: MacOS Classifier: Intended Audience ::
-Science/Research Classifier: Topic :: Software Development Classifier: Topic ::
-Scientific/Engineering Classifier: Natural Language :: English Requires-Python:
->=3.8 Description-Content-Type: text/markdown Provides-Extra: dev
```

### Comparing `sequentia-1.1.1/README.md` & `sequentia-2.0.0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,29 +1,32 @@
 <p align="center">
   <h1 align="center">
-    <img src="https://raw.githubusercontent.com/eonu/sequentia/master/docs/_static/images/logo.png" width="75px"><br/>
+    <img src="https://raw.githubusercontent.com/eonu/sequentia/master/docs/source/_static/images/logo.png" width="75px"><br/>
     Sequentia
   </h1>
 </p>
 
 <p align="center">
-  <em>HMM and DTW-based sequence machine learning algorithms in Python following an sklearn-like interface.</em>
+  <em>Scikit-Learn compatible HMM and DTW based sequence machine learning algorithms in Python.</em>
 </p>
 
 <p align="center">
   <div align="center">
     <a href="https://pypi.org/project/sequentia">
       <img src="https://img.shields.io/pypi/v/sequentia?logo=pypi&style=flat-square" alt="PyPI"/>
     </a>
     <a href="https://pypi.org/project/sequentia">
       <img src="https://img.shields.io/pypi/pyversions/sequentia?logo=python&style=flat-square" alt="PyPI - Python Version"/>
     </a>
     <a href="https://sequentia.readthedocs.io/en/latest">
       <img src="https://img.shields.io/readthedocs/sequentia.svg?logo=read-the-docs&style=flat-square" alt="Read The Docs - Documentation">
     </a>
+    <a href="https://coveralls.io/github/eonu/sequentia">
+      <img src="https://img.shields.io/coverallsCoverage/github/eonu/sequentia?logo=coveralls&style=flat-square" alt="Coveralls - Coverage"/>
+    </a>
     <a href="https://raw.githubusercontent.com/eonu/sequentia/master/LICENSE">
       <img src="https://img.shields.io/pypi/l/sequentia?style=flat-square" alt="PyPI - License"/>
     </a>
   </div>
 </p>
 
 <p align="center">
@@ -46,18 +49,23 @@
 
 Some examples of how Sequentia can be used on sequence data include:
 
 - determining a spoken word based on its audio signal or alternative representations such as MFCCs,
 - predicting motion intent for gesture control from sEMG signals,
 - classifying hand-written characters according to their pen-tip trajectories.
 
+### Why Sequentia?
+
+- **Simplicity and interpretability**: Sequentia offers a limited set of machine learning algorithms, chosen specifically to be more interpretable and easier to configure than more complex alternatives such as recurrent neural networks and transformers, while maintaining a high level of effectiveness.
+- **Familiar and user-friendly**: To fit more seamlessly into the workflow of data science practitioners, Sequentia follows the ubiquitous Scikit-Learn API, providing a familiar model development process for many, as well as enabling wider access to the rapidly growing Scikit-Learn ecosystem.
+
 ## Build Status
 
-| `master` | `dev` |
-| -------- | ------|
+| `master`                                                                                                                                                                                                 | `dev`                                                                                                                                                                                                      |
+| -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
 | [![CircleCI Build (Master)](https://img.shields.io/circleci/build/github/eonu/sequentia/master?logo=circleci&style=flat-square)](https://app.circleci.com/pipelines/github/eonu/sequentia?branch=master) | [![CircleCI Build (Development)](https://img.shields.io/circleci/build/github/eonu/sequentia/dev?logo=circleci&style=flat-square)](https://app.circleci.com/pipelines/github/eonu/sequentia?branch=master) |
 
 ## Features
 
 ### Models
 
 The following models provided by Sequentia all support variable length sequences.
@@ -80,66 +88,39 @@
 - [x] Multivariate real-valued observations (Gaussian mixture model emissions)
 - [x] Univariate categorical observations (discrete emissions)
 - [x] Linear, left-right and ergodic topologies
 - [x] Multi-processed predictions
 
 ### Scikit-Learn compatibility
 
-Sequentia aims to follow the Scikit-Learn interface for estimators and transformations,
-as well as to be largely compatible with three core Scikit-Learn modules to improve the ease of model development:
-[`preprocessing`](https://scikit-learn.org/stable/modules/classes.html#module-sklearn.preprocessing), [`model_selection`](https://scikit-learn.org/stable/modules/classes.html#module-sklearn.model_selection) and [`pipeline`](https://scikit-learn.org/stable/modules/classes.html#module-sklearn.pipeline).
-
-While there are many other modules, maintaining full compatibility with Scikit-Learn is challenging and many of its features are inapplicable to sequential data, therefore we only focus on the relevant core modules.
-
-Despite some deviation from the Scikit-Learn interface in order to accommodate sequences, the following features are currently compatible with Sequentia.
-
-- [x] [`preprocessing`](https://scikit-learn.org/stable/modules/classes.html#module-sklearn.preprocessing)
-  - [x] [`FunctionTransformer`](https://scikit-learn.org/stable/modules/generated/sklearn.preprocessing.FunctionTransformer.html#sklearn.preprocessing.FunctionTransformer) — via an adapted class definition
-  - [x] Function-based transformations (stateless)
-  - [x] Class-based transformations (stateful)
-- [ ] [`pipeline`](https://scikit-learn.org/stable/modules/classes.html#module-sklearn.pipeline)
-  - [x] [`Pipeline`](https://scikit-learn.org/stable/modules/generated/sklearn.pipeline.Pipeline.html#sklearn.pipeline.Pipeline) — via an adapted class definition
-  - [ ] [`FeatureUnion`](https://scikit-learn.org/stable/modules/generated/sklearn.pipeline.FeatureUnion.html#sklearn.pipeline.FeatureUnion)
-- [ ] [`model_selection`](https://scikit-learn.org/stable/modules/classes.html#module-sklearn.model_selection)
+**Sequentia (≥2.0) is fully compatible with the Scikit-Learn API (≥1.4), enabling for rapid development and prototyping of sequential models.**
 
-## Installation
+In most cases, the only necessary change is to add a `lengths` key-word argument to provide sequence length information, e.g. `fit(X, y, lengths=lengths)` instead of `fit(X, y)`.
 
-You can install Sequentia using `pip`.
-
-### Stable
+## Installation
 
-The latest stable version of Sequentia can be installed with the following command.
+The latest stable version of Sequentia can be installed with the following command:
 
 ```console
 pip install sequentia
 ```
 
-#### C library compilation
+### C library compilation
 
 For optimal performance when using any of the k-NN based models, it is important that `dtaidistance` C libraries are compiled correctly.
 
 Please see the [`dtaidistance` installation guide](https://dtaidistance.readthedocs.io/en/latest/usage/installation.html) for troubleshooting if you run into C compilation issues, or if setting `use_c=True` on k-NN based models results in a warning.
 
 You can use the following to check if the appropriate C libraries have been installed.
 
 ```python
 from dtaidistance import dtw
 dtw.try_import_c()
 ```
 
-### Pre-release
-
-Pre-release versions include new features which are in active development and may change unpredictably.
-
-The latest pre-release version can be installed with the following command.
-
-```console
-pip install --pre sequentia
-```
-
 ### Development
 
 Please see the [contribution guidelines](/CONTRIBUTING.md) to see installation instructions for contributing to Sequentia.
 
 ## Documentation
 
 Documentation for the package is available on [Read The Docs](https://sequentia.readthedocs.io/en/latest).
@@ -151,18 +132,18 @@
 This example also shows a typical preprocessing workflow, as well as compatibility with Scikit-Learn.
 
 ```python
 import numpy as np
 
 from sklearn.preprocessing import scale
 from sklearn.decomposition import PCA
+from sklearn.pipeline import Pipeline
 
 from sequentia.models import KNNClassifier
-from sequentia.pipeline import Pipeline
-from sequentia.preprocessing import IndependentFunctionTransformer, mean_filter
+from sequentia.preprocessing import IndependentFunctionTransformer, median_filter
 
 # Create input data
 # - Sequentia expects sequences to be concatenated into a single array
 # - Sequence lengths are provided separately and used to decode the sequences when needed
 # - This avoids the need for complex structures such as lists of arrays with different lengths
 
 # Sequences
@@ -175,41 +156,41 @@
     [2.11, 6.97],
     [1.83, 7.06],
     [1.54, 5.98],
     [0.86, 6.37],
     [1.21, 5.8 ],
     # Sequence 3 - Length 2
     [1.7 , 6.22],
-    [2.01, 5.49]
+    [2.01, 5.49],
 ])
 
 # Sequence lengths
 lengths = np.array([3, 5, 2])
 
 # Sequence classes
 y = np.array([0, 1, 1])
 
 # Create a transformation pipeline that feeds into a KNNClassifier
-# 1. Individually denoise each sequence by applying a mean filter for each feature
+# 1. Individually denoise each sequence by applying a median filter for each feature
 # 2. Individually standardize each sequence by subtracting the mean and dividing the s.d. for each feature
 # 3. Reduce the dimensionality of the data to a single feature by using PCA
 # 4. Pass the resulting transformed data into a KNNClassifier
 pipeline = Pipeline([
-    ('denoise', IndependentFunctionTransformer(mean_filter)),
+    ('denoise', IndependentFunctionTransformer(median_filter)),
     ('scale', IndependentFunctionTransformer(scale)),
     ('pca', PCA(n_components=1)),
     ('knn', KNNClassifier(k=1))
 ])
 
 # Fit the pipeline to the data - lengths must be provided
-pipeline.fit(X, y, lengths)
+pipeline.fit(X, y, lengths=lengths)
 
 # Predict classes for the sequences and calculate accuracy - lengths must be provided
-y_pred = pipeline.predict(X, lengths)
-acc = pipeline.score(X, y, lengths)
+y_pred = pipeline.predict(X, lengths=lengths)
+acc = pipeline.score(X, y, lengths=lengths)
 ```
 
 ## Acknowledgments
 
 In earlier versions of the package, an approximate DTW implementation [`fastdtw`](https://github.com/slaypni/fastdtw) was used in hopes of speeding up k-NN predictions, as the authors of the original FastDTW paper [[2]](#references) claim that approximated DTW alignments can be computed in linear memory and time, compared to the O(N<sup>2</sup>) runtime complexity of the usual exact DTW implementation.
 
 I was contacted by [Prof. Eamonn Keogh](https://www.cs.ucr.edu/~eamonn/) whose work makes the surprising revelation that FastDTW is generally slower than the exact DTW algorithm that it approximates [[3]](#references). Upon switching from the `fastdtw` package to [`dtaidistance`](https://github.com/wannesm/dtaidistance) (a very solid implementation of exact DTW with fast pure C compiled functions), DTW k-NN prediction times were indeed reduced drastically.
@@ -278,15 +259,15 @@
 </table>
 
 ## Licensing
 
 Sequentia is released under the [MIT](https://opensource.org/licenses/MIT) license.
 
 Certain parts of the source code are heavily adapted from [Scikit-Learn](scikit-learn.org/).
-Such files contain copy of [their license](https://github.com/scikit-learn/scikit-learn/blob/main/COPYING).
+Such files contain a copy of [their license](https://github.com/scikit-learn/scikit-learn/blob/main/COPYING).
 
 ---
 
 <p align="center">
-  <b>Sequentia</b> &copy; 2019-2023, Edwin Onuonga - Released under the <a href="https://opensource.org/licenses/MIT">MIT</a> license.<br/>
+  <b>Sequentia</b> &copy; 2019-2025, Edwin Onuonga - Released under the <a href="https://opensource.org/licenses/MIT">MIT</a> license.<br/>
   <em>Authored and maintained by Edwin Onuonga.</em>
-</p>
+</p>
```

#### html2text {}

```diff
@@ -1,23 +1,37 @@
- ************ [[hhttttppss::////rraaww..ggiitthhuubbuusseerrccoonntteenntt..ccoomm//eeoonnuu//sseeqquueennttiiaa//mmaasstteerr//ddooccss//__ssttaattiicc//
-                               iimmaaggeess//llooggoo..ppnngg]]
+ ************ [[hhttttppss::////rraaww..ggiitthhuubbuusseerrccoonntteenntt..ccoomm//eeoonnuu//sseeqquueennttiiaa//mmaasstteerr//ddooccss//ssoouurrccee//
+                           __ssttaattiicc//iimmaaggeess//llooggoo..ppnngg]]
                                SSeeqquueennttiiaa ************
- HHMMMM aanndd DDTTWW--bbaasseedd sseeqquueennccee mmaacchhiinnee lleeaarrnniinngg aallggoorriitthhmmss iinn PPyytthhoonn ffoolllloowwiinngg aann
-                            sskklleeaarrnn--lliikkee iinntteerrffaaccee..
- _[_P_y_P_I_]_[_P_y_P_I_ _-_ _P_y_t_h_o_n_ _V_e_r_s_i_o_n_]_[_R_e_a_d_ _T_h_e_ _D_o_c_s_ _-_ _D_o_c_u_m_e_n_t_a_t_i_o_n_]_[_P_y_P_I_ _-_ _L_i_c_e_n_s_e_]
+SScciikkiitt--LLeeaarrnn ccoommppaattiibbllee HHMMMM aanndd DDTTWW bbaasseedd sseeqquueennccee mmaacchhiinnee lleeaarrnniinngg aallggoorriitthhmmss
+                                  iinn PPyytthhoonn..
+   _[_P_y_P_I_]_[_P_y_P_I_ _-_ _P_y_t_h_o_n_ _V_e_r_s_i_o_n_]_[_R_e_a_d_ _T_h_e_ _D_o_c_s_ _-_ _D_o_c_u_m_e_n_t_a_t_i_o_n_]_[_C_o_v_e_r_a_l_l_s_ _-
+                           _C_o_v_e_r_a_g_e_]_[_P_y_P_I_ _-_ _L_i_c_e_n_s_e_]
        _A_b_o_u_t Â· _B_u_i_l_d_ _S_t_a_t_u_s Â· _F_e_a_t_u_r_e_s Â· _D_o_c_u_m_e_n_t_a_t_i_o_n Â· _E_x_a_m_p_l_e_s Â·
           _A_c_k_n_o_w_l_e_d_g_m_e_n_t_s Â· _R_e_f_e_r_e_n_c_e_s Â· _C_o_n_t_r_i_b_u_t_o_r_s Â· _L_i_c_e_n_s_i_n_g
 ## About Sequentia is a Python package that provides various classification and
 regression algorithms for sequential data, including methods based on hidden
 Markov models and dynamic time warping. Some examples of how Sequentia can be
 used on sequence data include: - determining a spoken word based on its audio
 signal or alternative representations such as MFCCs, - predicting motion intent
 for gesture control from sEMG signals, - classifying hand-written characters
-according to their pen-tip trajectories. ## Build Status | `master` | `dev` | |
--------- | ------| | [![CircleCI Build (Master)](https://img.shields.io/
+according to their pen-tip trajectories. ### Why Sequentia? - **Simplicity and
+interpretability**: Sequentia offers a limited set of machine learning
+algorithms, chosen specifically to be more interpretable and easier to
+configure than more complex alternatives such as recurrent neural networks and
+transformers, while maintaining a high level of effectiveness. - **Familiar and
+user-friendly**: To fit more seamlessly into the workflow of data science
+practitioners, Sequentia follows the ubiquitous Scikit-Learn API, providing a
+familiar model development process for many, as well as enabling wider access
+to the rapidly growing Scikit-Learn ecosystem. ## Build Status | `master` |
+`dev` | | ---------------------------------------------------------------------
+-------------------------------------------------------------------------------
+---------------------------------------------------- | ------------------------
+-------------------------------------------------------------------------------
+-------------------------------------------------------------------------------
+-------------------- | | [![CircleCI Build (Master)](https://img.shields.io/
 circleci/build/github/eonu/sequentia/master?logo=circleci&style=flat-square)]
 (https://app.circleci.com/pipelines/github/eonu/sequentia?branch=master) | [!
 [CircleCI Build (Development)](https://img.shields.io/circleci/build/github/
 eonu/sequentia/dev?logo=circleci&style=flat-square)](https://app.circleci.com/
 pipelines/github/eonu/sequentia?branch=master) | ## Features ### Models The
 following models provided by Sequentia all support variable length sequences.
 #### [Dynamic Time Warping + k-Nearest Neighbors](https://
@@ -29,107 +43,83 @@
 Multi-processed predictions #### [Hidden Markov Models](https://
 sequentia.readthedocs.io/en/latest/sections/models/hmm/index.html) (via
 [`hmmlearn`](https://github.com/hmmlearn/hmmlearn)) Parameter estimation with
 the Baum-Welch algorithm and prediction with the forward algorithm [[1]]
 (#references) - [x] Classification - [x] Multivariate real-valued observations
 (Gaussian mixture model emissions) - [x] Univariate categorical observations
 (discrete emissions) - [x] Linear, left-right and ergodic topologies - [x]
-Multi-processed predictions ### Scikit-Learn compatibility Sequentia aims to
-follow the Scikit-Learn interface for estimators and transformations, as well
-as to be largely compatible with three core Scikit-Learn modules to improve the
-ease of model development: [`preprocessing`](https://scikit-learn.org/stable/
-modules/classes.html#module-sklearn.preprocessing), [`model_selection`](https:/
-/scikit-learn.org/stable/modules/classes.html#module-sklearn.model_selection)
-and [`pipeline`](https://scikit-learn.org/stable/modules/classes.html#module-
-sklearn.pipeline). While there are many other modules, maintaining full
-compatibility with Scikit-Learn is challenging and many of its features are
-inapplicable to sequential data, therefore we only focus on the relevant core
-modules. Despite some deviation from the Scikit-Learn interface in order to
-accommodate sequences, the following features are currently compatible with
-Sequentia. - [x] [`preprocessing`](https://scikit-learn.org/stable/modules/
-classes.html#module-sklearn.preprocessing) - [x] [`FunctionTransformer`](https:
-//scikit-learn.org/stable/modules/generated/
-sklearn.preprocessing.FunctionTransformer.html#sklearn.preprocessing.FunctionTransformer)
-â via an adapted class definition - [x] Function-based transformations
-(stateless) - [x] Class-based transformations (stateful) - [ ] [`pipeline`]
-(https://scikit-learn.org/stable/modules/classes.html#module-sklearn.pipeline)
-- [x] [`Pipeline`](https://scikit-learn.org/stable/modules/generated/
-sklearn.pipeline.Pipeline.html#sklearn.pipeline.Pipeline) â via an adapted
-class definition - [ ] [`FeatureUnion`](https://scikit-learn.org/stable/
-modules/generated/
-sklearn.pipeline.FeatureUnion.html#sklearn.pipeline.FeatureUnion) - [ ]
-[`model_selection`](https://scikit-learn.org/stable/modules/
-classes.html#module-sklearn.model_selection) ## Installation You can install
-Sequentia using `pip`. ### Stable The latest stable version of Sequentia can be
-installed with the following command. ```console pip install sequentia ``` ####
-C library compilation For optimal performance when using any of the k-NN based
-models, it is important that `dtaidistance` C libraries are compiled correctly.
-Please see the [`dtaidistance` installation guide](https://
-dtaidistance.readthedocs.io/en/latest/usage/installation.html) for
-troubleshooting if you run into C compilation issues, or if setting
-`use_c=True` on k-NN based models results in a warning. You can use the
-following to check if the appropriate C libraries have been installed.
-```python from dtaidistance import dtw dtw.try_import_c() ``` ### Pre-release
-Pre-release versions include new features which are in active development and
-may change unpredictably. The latest pre-release version can be installed with
-the following command. ```console pip install --pre sequentia ``` ###
-Development Please see the [contribution guidelines](/CONTRIBUTING.md) to see
-installation instructions for contributing to Sequentia. ## Documentation
-Documentation for the package is available on [Read The Docs](https://
-sequentia.readthedocs.io/en/latest). ## Examples Demonstration of classifying
-multivariate sequences with two features into two classes using the
+Multi-processed predictions ### Scikit-Learn compatibility **Sequentia (â¥2.0)
+is fully compatible with the Scikit-Learn API (â¥1.4), enabling for rapid
+development and prototyping of sequential models.** In most cases, the only
+necessary change is to add a `lengths` key-word argument to provide sequence
+length information, e.g. `fit(X, y, lengths=lengths)` instead of `fit(X, y)`.
+## Installation The latest stable version of Sequentia can be installed with
+the following command: ```console pip install sequentia ``` ### C library
+compilation For optimal performance when using any of the k-NN based models, it
+is important that `dtaidistance` C libraries are compiled correctly. Please see
+the [`dtaidistance` installation guide](https://dtaidistance.readthedocs.io/en/
+latest/usage/installation.html) for troubleshooting if you run into C
+compilation issues, or if setting `use_c=True` on k-NN based models results in
+a warning. You can use the following to check if the appropriate C libraries
+have been installed. ```python from dtaidistance import dtw dtw.try_import_c()
+``` ### Development Please see the [contribution guidelines](/CONTRIBUTING.md)
+to see installation instructions for contributing to Sequentia. ##
+Documentation Documentation for the package is available on [Read The Docs]
+(https://sequentia.readthedocs.io/en/latest). ## Examples Demonstration of
+classifying multivariate sequences with two features into two classes using the
 `KNNClassifier`. This example also shows a typical preprocessing workflow, as
 well as compatibility with Scikit-Learn. ```python import numpy as np from
 sklearn.preprocessing import scale from sklearn.decomposition import PCA from
-sequentia.models import KNNClassifier from sequentia.pipeline import Pipeline
-from sequentia.preprocessing import IndependentFunctionTransformer, mean_filter
-# Create input data # - Sequentia expects sequences to be concatenated into a
-single array # - Sequence lengths are provided separately and used to decode
-the sequences when needed # - This avoids the need for complex structures such
-as lists of arrays with different lengths # Sequences X = np.array([ # Sequence
-1 - Length 3 [1.2 , 7.91], [1.34, 6.6 ], [0.92, 8.08], # Sequence 2 - Length 5
-[2.11, 6.97], [1.83, 7.06], [1.54, 5.98], [0.86, 6.37], [1.21, 5.8 ], #
-Sequence 3 - Length 2 [1.7 , 6.22], [2.01, 5.49] ]) # Sequence lengths lengths
-= np.array([3, 5, 2]) # Sequence classes y = np.array([0, 1, 1]) # Create a
-transformation pipeline that feeds into a KNNClassifier # 1. Individually
-denoise each sequence by applying a mean filter for each feature # 2.
-Individually standardize each sequence by subtracting the mean and dividing the
-s.d. for each feature # 3. Reduce the dimensionality of the data to a single
-feature by using PCA # 4. Pass the resulting transformed data into a
-KNNClassifier pipeline = Pipeline([ ('denoise', IndependentFunctionTransformer
-(mean_filter)), ('scale', IndependentFunctionTransformer(scale)), ('pca', PCA
-(n_components=1)), ('knn', KNNClassifier(k=1)) ]) # Fit the pipeline to the
-data - lengths must be provided pipeline.fit(X, y, lengths) # Predict classes
-for the sequences and calculate accuracy - lengths must be provided y_pred =
-pipeline.predict(X, lengths) acc = pipeline.score(X, y, lengths) ``` ##
-Acknowledgments In earlier versions of the package, an approximate DTW
-implementation [`fastdtw`](https://github.com/slaypni/fastdtw) was used in
-hopes of speeding up k-NN predictions, as the authors of the original FastDTW
-paper [[2]](#references) claim that approximated DTW alignments can be computed
-in linear memory and time, compared to the O(N2) runtime complexity of the
-usual exact DTW implementation. I was contacted by [Prof. Eamonn Keogh](https:/
-/www.cs.ucr.edu/~eamonn/) whose work makes the surprising revelation that
-FastDTW is generally slower than the exact DTW algorithm that it approximates [
-[3]](#references). Upon switching from the `fastdtw` package to
-[`dtaidistance`](https://github.com/wannesm/dtaidistance) (a very solid
-implementation of exact DTW with fast pure C compiled functions), DTW k-NN
-prediction times were indeed reduced drastically. I would like to thank Prof.
-Eamonn Keogh for directly reaching out to me regarding this finding. ##
-References
+sklearn.pipeline import Pipeline from sequentia.models import KNNClassifier
+from sequentia.preprocessing import IndependentFunctionTransformer,
+median_filter # Create input data # - Sequentia expects sequences to be
+concatenated into a single array # - Sequence lengths are provided separately
+and used to decode the sequences when needed # - This avoids the need for
+complex structures such as lists of arrays with different lengths # Sequences X
+= np.array([ # Sequence 1 - Length 3 [1.2 , 7.91], [1.34, 6.6 ], [0.92, 8.08],
+# Sequence 2 - Length 5 [2.11, 6.97], [1.83, 7.06], [1.54, 5.98], [0.86, 6.37],
+[1.21, 5.8 ], # Sequence 3 - Length 2 [1.7 , 6.22], [2.01, 5.49], ]) # Sequence
+lengths lengths = np.array([3, 5, 2]) # Sequence classes y = np.array([0, 1,
+1]) # Create a transformation pipeline that feeds into a KNNClassifier # 1.
+Individually denoise each sequence by applying a median filter for each feature
+# 2. Individually standardize each sequence by subtracting the mean and
+dividing the s.d. for each feature # 3. Reduce the dimensionality of the data
+to a single feature by using PCA # 4. Pass the resulting transformed data into
+a KNNClassifier pipeline = Pipeline([ ('denoise',
+IndependentFunctionTransformer(median_filter)), ('scale',
+IndependentFunctionTransformer(scale)), ('pca', PCA(n_components=1)), ('knn',
+KNNClassifier(k=1)) ]) # Fit the pipeline to the data - lengths must be
+provided pipeline.fit(X, y, lengths=lengths) # Predict classes for the
+sequences and calculate accuracy - lengths must be provided y_pred =
+pipeline.predict(X, lengths=lengths) acc = pipeline.score(X, y,
+lengths=lengths) ``` ## Acknowledgments In earlier versions of the package, an
+approximate DTW implementation [`fastdtw`](https://github.com/slaypni/fastdtw)
+was used in hopes of speeding up k-NN predictions, as the authors of the
+original FastDTW paper [[2]](#references) claim that approximated DTW
+alignments can be computed in linear memory and time, compared to the O(N2)
+runtime complexity of the usual exact DTW implementation. I was contacted by
+[Prof. Eamonn Keogh](https://www.cs.ucr.edu/~eamonn/) whose work makes the
+surprising revelation that FastDTW is generally slower than the exact DTW
+algorithm that it approximates [[3]](#references). Upon switching from the
+`fastdtw` package to [`dtaidistance`](https://github.com/wannesm/dtaidistance)
+(a very solid implementation of exact DTW with fast pure C compiled functions),
+DTW k-NN prediction times were indeed reduced drastically. I would like to
+thank Prof. Eamonn Keogh for directly reaching out to me regarding this
+finding. ## References
     _L_a_w_r_e_n_c_e_ _R_._ _R_a_b_i_n_e_r_._ _""_AA_ _TT_uu_tt_oo_rr_ii_aa_ll_ _oo_nn_ _HH_ii_dd_dd_ee_nn_ _MM_aa_rr_kk_oo_vv_ _MM_oo_dd_ee_ll_ss_ _aa_nn_dd_ _SS_ee_ll_ee_cc_tt_ee_dd
 [1] _AA_pp_pp_ll_ii_cc_aa_tt_ii_oo_nn_ss_ _ii_nn_ _SS_pp_ee_ee_cc_hh_ _RR_ee_cc_oo_gg_nn_ii_tt_ii_oo_nn_""_ _PP_rr_oo_cc_ee_ee_dd_ii_nn_gg_ss_ _oo_ff_ _tt_hh_ee_ _II_EE_EE_EE_ _77_77_ _((_11_99_88_99_))_,_ _n_o_.
     _2_,_ _2_5_7_-_8_6_.
 [2] _S_t_a_n_ _S_a_l_v_a_d_o_r_ _&_ _P_h_i_l_i_p_ _C_h_a_n_._ _""_FF_aa_ss_tt_DD_TT_WW_::_ _TT_oo_ww_aa_rr_dd_ _aa_cc_cc_uu_rr_aa_tt_ee_ _dd_yy_nn_aa_mm_ii_cc_ _tt_ii_mm_ee_ _ww_aa_rr_pp_ii_nn_gg
     _ii_nn_ _ll_ii_nn_ee_aa_rr_ _tt_ii_mm_ee_ _aa_nn_dd_ _ss_pp_aa_cc_ee_.._""_ _II_nn_tt_ee_ll_ll_ii_gg_ee_nn_tt_ _DD_aa_tt_aa_ _AA_nn_aa_ll_yy_ss_ii_ss_ _11_11_.._55_ _((_22_00_00_77_))_,_ _5_6_1_-_5_8_0_.
     _R_e_n_j_i_e_ _W_u_ _&_ _E_a_m_o_n_n_ _J_._ _K_e_o_g_h_._ _""_FF_aa_ss_tt_DD_TT_WW_ _ii_ss_ _aa_pp_pp_rr_oo_xx_ii_mm_aa_tt_ee_ _aa_nn_dd_ _GG_ee_nn_ee_rr_aa_ll_ll_yy_ _SS_ll_oo_ww_ee_rr
 [3] _tt_hh_aa_nn_ _tt_hh_ee_ _AA_ll_gg_oo_rr_ii_tt_hh_mm_ _ii_tt_ _AA_pp_pp_rr_oo_xx_ii_mm_aa_tt_ee_ss_""_ _II_EE_EE_EE_ _TT_rr_aa_nn_ss_aa_cc_tt_ii_oo_nn_ss_ _oo_nn_ _KK_nn_oo_ww_ll_ee_dd_gg_ee_ _aa_nn_dd_ _DD_aa_tt_aa
     _EE_nn_gg_ii_nn_ee_ee_rr_ii_nn_gg_ _((_22_00_22_00_))_,_ _1_â___1_.
 ## Contributors All contributions to this repository are greatly appreciated.
 Contribution guidelines can be found [here](/CONTRIBUTING.md).
 _[[_ee_oo_nn_uu_]] _[[_PP_rr_hh_mm_mm_aa_]] _[[_mm_aa_nn_ii_ss_cc_ii_]] _[[_jj_oo_nn_nn_oo_rr_]]
  _ee_oo_nn_uu   _PP_rr_hh_mm_mm_aa   _mm_aa_nn_ii_ss_cc_ii   _jj_oo_nn_nn_oo_rr
 ## Licensing Sequentia is released under the [MIT](https://opensource.org/
 licenses/MIT) license. Certain parts of the source code are heavily adapted
-from [Scikit-Learn](scikit-learn.org/). Such files contain copy of [their
+from [Scikit-Learn](scikit-learn.org/). Such files contain a copy of [their
 license](https://github.com/scikit-learn/scikit-learn/blob/main/COPYING). ---
-    SSeeqquueennttiiaa © 2019-2023, Edwin Onuonga - Released under the _M_I_T license.
+    SSeeqquueennttiiaa © 2019-2025, Edwin Onuonga - Released under the _M_I_T license.
                    AAuutthhoorreedd aanndd mmaaiinnttaaiinneedd bbyy EEddwwiinn OOnnuuoonnggaa..
```

### Comparing `sequentia-1.1.1/lib/sequentia/datasets/data/digits.npz` & `sequentia-2.0.0/sequentia/datasets/data/digits.npz`

 * *Files identical despite different names*

### Comparing `sequentia-1.1.1/lib/sequentia/datasets/digits.py` & `sequentia-2.0.0/sequentia/datasets/digits.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,50 +1,60 @@
-from pkg_resources import resource_filename
-from typing import Iterable
-from operator import itemgetter
+# Copyright (c) 2019-2025 Sequentia Developers.
+# Distributed under the terms of the MIT License (see the LICENSE file).
+# SPDX-License-Identifier: MIT
+# This source code is part of the Sequentia project (https://github.com/eonu/sequentia).
+
+"""Free Spoken Digit Dataset."""
+
+from __future__ import annotations
+
+import importlib.resources
+import operator
 
 import numpy as np
-from pydantic import conint, validator
+import pydantic as pyd
+
+import sequentia.datasets.data
+from sequentia._internal import _data
+from sequentia.datasets.base import SequentialDataset
+
+__all__ = ["load_digits"]
 
-from sequentia.utils.data import SequentialDataset
-from sequentia.utils.validation import _Validator
-from sequentia.utils.decorators import _validate_params
-
-class _DigitsValidator(_Validator):
-    digits: Iterable[conint(ge=0, le=9)] = list(range(10))
-
-    @validator('digits')
-    def check_digits(cls, value):
-        value = list(value)
-        if len(set(value)) < len(value):
-            raise ValueError('Expected digits to be unique')
-        return value
 
-@_validate_params(using=_DigitsValidator)
+@pyd.validate_call
 def load_digits(
-    *,
-    digits: Iterable[int] = list(range(10)),
+    *, digits: set[pyd.conint(ge=0, le=9)] = {0, 1, 2, 3, 4, 5, 6, 7, 8, 9}
 ) -> SequentialDataset:
-    """Loads MFCC features of spoken digit audio samples from the Free Spoken Digit Dataset.
+    """Load a dataset of MFCC features of spoken digit audio samples from the
+    Free Spoken Digit Dataset.
 
     The `Free Spoken Digit Dataset (FSDD) <https://github.com/Jakobovski/free-spoken-digit-dataset>`_
     consists of 3000 recordings of the spoken digits 0-9.
 
-    This version consists of 13 MFCC features of 50 recordings for each digit by 6 individual speakers.
+    This version consists of 13 MFCC features of 50 recordings for each digit
+    by 6 individual speakers.
 
-    :param digits: Subset of digits to include in the dataset.
-    :return: A dataset object representing the loaded digits.
+    Parameters
+    ----------
+    digits:
+        Subset of digits to include in the dataset.
+
+    Returns
+    -------
+    SequentialDataset
+        A dataset object representing the loaded digits.
     """
     # Load the dataset from compressed numpy file
-    data = np.load(resource_filename('sequentia', 'datasets/data/digits.npz'))
+    path = importlib.resources.files(sequentia.datasets.data)
+    data = np.load(path / "digits.npz")
 
     # Fetch arrays from loaded file
-    X, y, lengths = itemgetter('X', 'y', 'lengths')(data)
+    X, y, lengths = operator.itemgetter("X", "y", "lengths")(data)
 
-    # Select and create a Dataset only with sequences having the specified labels
-    idx = np.argwhere(np.isin(y, digits)).flatten()
-    ranges = SequentialDataset._get_idxs(lengths)[idx]
+    # Create a dataset only with sequences having the specified labels
+    idx = np.argwhere(np.isin(y, sorted(digits))).flatten()
+    ranges = _data.get_idxs(lengths)[idx]
     return SequentialDataset(
-        np.vstack([x for x in SequentialDataset._iter_X(X, ranges)]),
+        np.vstack(list(_data.iter_X(X, idxs=ranges))),
         y[idx],
-        lengths[idx]
+        lengths=lengths[idx],
     )
```

### Comparing `sequentia-1.1.1/lib/sequentia/datasets/gene_families.py` & `sequentia-2.0.0/sequentia/datasets/gene_families.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,73 +1,79 @@
-from pkg_resources import resource_filename
-from typing import Iterable, Tuple
-from operator import itemgetter
+# Copyright (c) 2019-2025 Sequentia Developers.
+# Distributed under the terms of the MIT License (see the LICENSE file).
+# SPDX-License-Identifier: MIT
+# This source code is part of the Sequentia project (https://github.com/eonu/sequentia).
+
+"""Gene families dataset."""
+
+from __future__ import annotations
+
+import importlib.resources
+import operator
 
 import numpy as np
-from pydantic import conint, validator
+import pydantic as pyd
 from sklearn.preprocessing import LabelEncoder
 
-from sequentia.utils.data import SequentialDataset
-from sequentia.utils.validation import _Validator
-from sequentia.utils.decorators import _validate_params
-
-
-class _GeneFamiliesValidator(_Validator):
-    families: Iterable[conint(ge=0, le=6)] = list(range(7))
-
-    @validator('families')
-    def check_families(cls, value):
-        value = list(value)
-        if len(set(value)) < len(value):
-            raise ValueError('Expected gene families to be unique')
-        return value
+import sequentia.datasets.data
+from sequentia._internal import _data
+from sequentia.datasets.base import SequentialDataset
 
-@_validate_params(using=_GeneFamiliesValidator)
-def load_gene_families(
-    *,
-    families: Iterable[int] = list(range(7))
-) -> Tuple[SequentialDataset, LabelEncoder]:
-    """Loads human DNA sequences grouped by gene family.
+__all__ = ["load_gene_families"]
 
-    The `Human DNA Sequences <https://www.kaggle.com/datasets/sooryaprakash12/human-dna-sequences>`_ dataset
-    consists of 4380 DNA sequences belonging to 7 gene families.
 
-    This dataset has imbalanced classes, and uses an :class:`sklearn:sklearn.preprocessing.LabelEncoder` to
-    encode the original symbols (``A``, ``T``, ``C``, ``G``, ``N``) that form the DNA sequences, into integers.
+@pyd.validate_call
+def load_gene_families(
+    *, families: set[pyd.conint(ge=0, le=6)] = {0, 1, 2, 3, 4, 5, 6}
+) -> tuple[SequentialDataset, LabelEncoder]:
+    """Load a dataset of human DNA sequences grouped by gene family.
+
+    The `Human DNA Sequences <https://www.kaggle.com/datasets/sooryaprakash12/human-dna-sequences>`_
+    dataset consists of 4380 DNA sequences belonging to 7 gene families.
+
+    This dataset has imbalanced classes, and uses an
+    :class:`sklearn:sklearn.preprocessing.LabelEncoder` to encode the
+    original symbols (``A``, ``T``, ``C``, ``G``, ``N``) that form the DNA
+    sequences, into integers.
 
     The gene families have the following class labels:
 
     - G protein coupled receptors: ``0``
     - Tyrosine kinase: ``1``
     - Tyrosine phosphatase: ``2``
     - Synthetase: ``3``
     - Synthase: ``4``
     - Ion channel: ``5``
     - Transcription: ``6``
 
-    :param families: Subset of gene families to include in the dataset.
-
-    :return:
-
+    Parameters
+    ----------
+    families:
+        Subset of gene families to include in the dataset.
+
+    Returns
+    -------
+    tuple[SequentialDataset, sklearn.preprocessing.LabelEncoder]
         - A dataset object representing the loaded genetic data.
         - Label encoder used to encode the observation symbols into integers.
     """
     # Load the dataset from compressed numpy file
-    data = np.load(resource_filename('sequentia', 'datasets/data/gene_families.npz'))
+    path = importlib.resources.files(sequentia.datasets.data)
+    data = np.load(path / "gene_families.npz")
 
     # Fetch arrays from loaded file
-    X, y, lengths = itemgetter('X', 'y', 'lengths')(data)
+    X, y, lengths = operator.itemgetter("X", "y", "lengths")(data)
 
     # Encode the observation symbols into integers
     enc = LabelEncoder()
     X = np.expand_dims(enc.fit_transform(X.flatten()), axis=-1)
 
-    # Select and create a Dataset only with sequences having the specified labels
-    idx = np.argwhere(np.isin(y, families)).flatten()
-    ranges = SequentialDataset._get_idxs(lengths)[idx]
+    # Create a dataset only with sequences having the specified labels
+    idx = np.argwhere(np.isin(y, sorted(families))).flatten()
+    ranges = _data.get_idxs(lengths)[idx]
     data = SequentialDataset(
-        np.vstack([x for x in SequentialDataset._iter_X(X, ranges)]),
+        np.vstack(list(_data.iter_X(X, idxs=ranges))),
         y[idx],
-        lengths[idx]
+        lengths=lengths[idx],
     )
 
     return data, enc
```

### Comparing `sequentia-1.1.1/lib/sequentia/models/hmm/classifier.py` & `sequentia-2.0.0/sequentia/models/hmm/classifier.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,76 +1,46 @@
+# Copyright (c) 2019-2025 Sequentia Developers.
+# Distributed under the terms of the MIT License (see the LICENSE file).
+# SPDX-License-Identifier: MIT
+# This source code is part of the Sequentia project (https://github.com/eonu/sequentia).
+
+"""A classifier consisting of HMMs, each trained independently to recognize
+sequences of a single class.
+"""
+
 from __future__ import annotations
 
-import joblib
 import pathlib
-from types import SimpleNamespace
-from typing import Optional, Union, Dict, Literal, IO
-from joblib import Parallel, delayed
+import typing as t
 
+import joblib
 import numpy as np
-from pydantic import NegativeInt, PositiveInt, confloat, validator, root_validator
+import pydantic as pyd
 from sklearn.utils.validation import NotFittedError
 
-from sequentia.models.base import _Classifier
-from sequentia.models.hmm.variants.base import _HMM
-from sequentia.utils.data import SequentialDataset
-from sequentia.utils.multiprocessing import _effective_n_jobs
-from sequentia.utils.decorators import _validate_params, _override_params, _requires_fit
-from sequentia.utils.validation import (
-    _check_classes,
-    _check_is_fitted,
-    Array,
-    _Validator,
-)
-
-__all__ = ['HMMClassifier']
-
-_defaults = SimpleNamespace(
-    prior=None,
-    classes=None,
-    n_jobs=1,
-)
-
-
-class _HMMClassifierValidator(_Validator):
-    prior: Optional[Union[Literal["frequency"], Dict[int, confloat(ge=0, le=1)]]] = _defaults.prior
-    classes: Optional[Array[int]] = _defaults.classes
-    n_jobs: Union[NegativeInt, PositiveInt] = _defaults.n_jobs
-
-
-    @validator('prior')
-    def check_prior(cls, value):
-        if isinstance(value, dict):
-            if not np.isclose(sum(value.values()), 1):
-                raise ValueError('Prior distribution must sum to one')
-        return value
-
-
-    @root_validator
-    def check_prior_keys_with_classes(cls, values):
-        if 'prior' in values and 'classes' in values:
-            prior, classes = values['prior'], values['classes']
-            if isinstance(prior, dict) and classes is not None:
-                if set(prior.keys()) != set(classes):
-                    raise ValueError(
-                        'Provided classes are not consistent with the provided prior distribution - '
-                        'ensure that every label in `classes` is present in `prior`'
-                    )
-        return values
+from sequentia._internal import _data, _multiprocessing, _validation
+from sequentia._internal._typing import Array, FloatArray, IntArray
+from sequentia.datasets.base import SequentialDataset
+from sequentia.enums import PriorMode
+from sequentia.models.base import ClassifierMixin
+from sequentia.models.hmm.variants.base import BaseHMM
 
 
-class HMMClassifier(_Classifier):
-    """A classifier consisting of HMMs, each trained independently to recognize sequences of a single class.
-
-    The predicted class for a given observation sequence is the class represented by the HMM
-    which produces the maximum posterior probability for the observation sequence.
+class HMMClassifier(ClassifierMixin):
+    """A classifier consisting of HMMs, each trained independently to
+    recognize sequences of a single class.
+
+    The predicted class for a given observation sequence is the class
+    represented by the HMM which produces the maximum posterior
+    probability for the observation sequence.
 
     Examples
     --------
-    Using a :class:`.HMMClassifier` (with :class:`.GaussianMixtureHMM` models) to classify spoken digits. ::
+    Using a :class:`.HMMClassifier` (with :class:`.GaussianMixtureHMM`
+    models) to classify spoken digits. ::
 
         import numpy as np
         from sequentia.datasets import load_digits
         from sequentia.models.hmm import GaussianMixtureHMM, HMMClassifier
 
         # Seed for reproducible pseudo-randomness
         random_state = np.random.RandomState(1)
@@ -81,452 +51,520 @@
 
         # Create a HMMClassifier using a class frequency prior
         clf = HMMClassifier(prior='frequency')
 
         # Add an untrained HMM for each class
         for label in data.classes:
             model = GaussianMixtureHMM(random_state=random_state)
-            clf.add_model(model, label)
+            clf.add_model(model, label=label)
 
         # Fit the HMMs by providing training observation sequences for all classes
-        X_train, y_train, lengths_train = train_data.X_y_lengths
-        clf.fit(X_train, y_train, lengths_train)
+        clf.fit(train_data.X, train_data.y, lengths=train_data.lengths)
 
         # Predict classes for the test observation sequences
-        X_test, lengths_test = test_data.X_lengths
-        y_pred = clf.predict(X_test, lengths_test)
+        y_pred = clf.predict(test_data.X, lengths=test_data.lengths)
 
-    As done in the above example, we can provide unfitted HMMs using :func:`add_model` or :func:`add_models`,
-    then provide training observation sequences for all classes to :func:`fit`, which will automatically train each HMM on the appropriate subset of data.
+    As done in the above example, we can provide unfitted HMMs using
+    :func:`add_model` or :func:`add_models`, then provide training
+    observation sequences for all classes to :func:`fit`, which will
+    automatically train each HMM on the appropriate subset of data.
 
-    Alternatively, we may provide pre-fitted HMMs and call :func:`fit` with no arguments. ::
+    Alternatively, we may provide pre-fitted HMMs and call :func:`fit` with
+    no arguments. ::
 
         # Create a HMMClassifier using a class frequency prior
         clf = HMMClassifier(prior='frequency')
 
        # Manually fit each HMM on its own subset of data
         for X_train, lengths_train, label for train_data.iter_by_class():
             model = GaussianMixtureHMM(random_state=random_state)
-            model.fit(X_train, lengths_train)
-            clf.add_model(model, label)
+            model.fit(X_train, lengths=lengths_train)
+            clf.add_model(model, label=label)
 
         # Fit the classifier
         clf.fit()
-    """
-
-    _defaults = _defaults
-
+    """  # noqa: E501
 
-    @_validate_params(using=_HMMClassifierValidator)
+    @pyd.validate_call(config=dict(arbitrary_types_allowed=True))
     def __init__(
-        self,
+        self: pyd.SkipValidation,
         *,
-        prior: Optional[Union[Literal["frequency"], dict]] = _defaults.prior,
-        classes: Optional[Array[int]] = _defaults.classes,
-        n_jobs: Union[NegativeInt, PositiveInt] = _defaults.n_jobs,
-    ) -> HMMClassifier:
-        """Initializes a :class:`.HMMClassifier`.
-
-        :param prior: Type of prior probability to assign to each HMM.
-
-            - If ``None``, a uniform prior will be used, making each HMM equally likely.
-            - If ``"frequency"``, the prior probability of each HMM is equal to the fraction of total observation sequences that the HMM was fitted with.
-            - If a ``dict``, custom prior probabilities can be assigned to each HMM.
-              The keys should be the label of the class represented by the HMM, and the value should be the prior probability for the HMM.
+        prior: (
+            PriorMode | dict[int, pyd.confloat(ge=0, le=1)]
+        ) = PriorMode.UNIFORM,  # placeholder
+        classes: list[int] | None = None,
+        n_jobs: pyd.PositiveInt | pyd.NegativeInt = 1,
+    ) -> pyd.SkipValidation:
+        """Initialize a :class:`.HMMClassifier`.
+
+        Parameters
+        ----------
+        self: HMMClassifier
+
+        prior:
+            Type of prior probability to assign to each HMM.
+
+            - If ``None``, a uniform prior will be used, making each HMM
+              equally likely.
+            - If ``"frequency"``, the prior probability of each HMM is equal
+              to the fraction of total observation sequences that the HMM was
+              fitted with.
+            - If a ``dict``, custom prior probabilities can be assigned to
+              each HMM. The keys should be the label of the class represented
+              by the HMM, and the value should be the prior probability for
+              the HMM.
+
+        classes:
+            Set of possible class labels.
+
+            - If not provided, these will be determined from the training
+              data labels.
+            - If provided, output from methods such as :func:`predict_proba`
+              and :func:`predict_scores` will follow the ordering of the
+              class labels provided here.
 
-        :param classes: Set of possible class labels.
-
-            - If not provided, these will be determined from the training data labels.
-            - If provided, output from methods such as :func:`predict_proba` and :func:`predict_scores`
-              will follow the ordering of the class labels provided here.
-
-        :param n_jobs: Maximum number of concurrently running workers.
+        n_jobs:
+            Maximum number of concurrently running workers.
 
             - If 1, no parallelism is used at all (useful for debugging).
             - If -1, all CPUs are used.
-            - If < -1, ``(n_cpus + 1 + n_jobs)`` are used — e.g. ``n_jobs=-2`` uses all but one.
+            - If < -1, ``(n_cpus + 1 + n_jobs)`` are used — e.g.
+              ``n_jobs=-2`` uses all but one.
+
+        Returns
+        -------
+        HMMClassifier
         """
         #: Type of prior probability to assign to each HMM.
-        self.prior = prior
+        self.prior: PriorMode | dict[int, pyd.confloat(ge=0, le=1)] = prior
         #: Set of possible class labels.
-        self.classes = classes
+        self.classes: list[int] | None = classes
         #: Maximum number of concurrently running workers.
-        self.n_jobs = n_jobs
+        self.n_jobs: pyd.PositiveInt | pyd.NegativeInt = n_jobs
         #: HMMs constituting the :class:`.HMMClassifier`.
-        self.models = {}
-
+        self.models: dict[int, BaseHMM] = {}
+        # Allow metadata routing for lengths
+        self.set_fit_request(lengths=True)
+        self.set_predict_request(lengths=True)
+        self.set_predict_proba_request(lengths=True)
+        self.set_predict_log_proba_request(lengths=True)
+        self.set_score_request(
+            lengths=True,
+            normalize=True,
+            sample_weight=True,
+        )
 
+    @pyd.validate_call(config=dict(arbitrary_types_allowed=True))
     def add_model(
-        self,
-        model: _HMM,
-        label: int
-    ) -> HMMClassifier:
-        """Adds a single HMM to the classifier.
-
-        :param model: HMM to add to the classifier.
-        :param label: Class represented by the HMM.
-
-        :note: All models added to the classifier must be of the same type — either :class:`.GaussianMixtureHMM` or :class:`.CategoricalHMM`.
-
-        :return: The classifier.
-        """
-        if not isinstance(model, _HMM):
-            raise TypeError('Expected `model` argument to be a type of HMM')
-        if len(self.models) > 0:
-            if type(model) != type(list(self.models.values())[-1]):
-                raise TypeError(
-                    f'Model of type {type(model).__name__} must be the same as the models already provided '
-                    f'to this {type(self).__name__} instance'
-                )
+        self: pyd.SkipValidation,
+        model: BaseHMM,
+        /,
+        *,
+        label: int,
+    ) -> pyd.SkipValidation:
+        """Add a single HMM to the classifier.
+
+        Parameters
+        ----------
+        self: HMMClassifier
+
+        model:
+            HMM to add to the classifier.
+
+        label:
+            Class represented by the HMM.
+
+        Returns
+        -------
+        HMMClassifier
+            The classifier.
+
+        Notes
+        -----
+        All models added to the classifier must be of the same type — either
+        :class:`.GaussianMixtureHMM` or :class:`.CategoricalHMM`.
+        """
+        if len(self.models) > 0 and not isinstance(
+            model, type(next(iter(self.models.values())))
+        ):
+            msg = (
+                f"Model of type {type(model).__name__} must be the same "
+                "as the models already provided to this "
+                f"{type(self).__name__} instance"
+            )
+            raise TypeError(msg)
         self.models[int(label)] = model
         return self
 
-
+    @pyd.validate_call(config=dict(arbitrary_types_allowed=True))
     def add_models(
-        self,
-        models: Dict[int, _HMM]
-    ) -> HMMClassifier:
-        """Adds HMMs to the classifier.
-
-        :param models: HMMs to add to the classifier. The key for each HMM should be the label of the class represented by the HMM.
-
-        :note: All models added to the classifier must be of the same type — either :class:`.GaussianMixtureHMM` or :class:`.CategoricalHMM`.
-
-        :return: The classifier.
+        self: pyd.SkipValidation,
+        models: dict[int, BaseHMM],
+        /,
+    ) -> pyd.SkipValidation:
+        """Add HMMs to the classifier.
+
+        Parameters
+        ----------
+        self: HMMClassifier
+
+        models:
+            HMMs to add to the classifier. The key for each HMM should be the
+            label of the class represented by the HMM.
+
+        Returns
+        -------
+        HMMClassifier
+            The classifier.
+
+        Notes
+        -----
+        All models added to the classifier must be of the same type — either
+        :class:`.GaussianMixtureHMM` or :class:`.CategoricalHMM`.
         """
-        if not all(isinstance(model, _HMM) for model in models.values()):
-            raise TypeError('Expected all provided `models` to be a type of HMM')
         for label, model in models.items():
-            self.add_model(model, label)
+            self.add_model(model, label=label)
         return self
 
-
     def fit(
-        self,
-        X: Optional[Array] = None,
-        y: Optional[Array[int]] = None,
-        lengths: Optional[Array[int]] = None
+        self: HMMClassifier,
+        X: Array | None = None,
+        y: IntArray | None = None,
+        *,
+        lengths: IntArray | None = None,
     ) -> HMMClassifier:
-        """Fits the HMMs to the sequence(s) in ``X``.
+        """Fit the HMMs to the sequence(s) in ``X``.
 
-        - If fitted models were provided with :func:`add_model` or :func:`add_models`, no arguments should be passed to :func:`fit`.
-        - If unfitted models were provided with :func:`add_model` or :func:`add_models`, training data ``X``, ``y`` and ``lengths`` must be provided to :func:`fit`.
+        - If fitted models were provided with :func:`add_model` or
+          :func:`add_models`, no arguments should be passed to :func:`fit`.
+        - If unfitted models were provided with :func:`add_model` or
+          :func:`add_models`, training data ``X``, ``y`` and ``lengths``
+          must be provided to :func:`fit`.
 
-        :param X: Univariate or multivariate observation sequence(s).
+        Parameters
+        ----------
+        self: HMMClassifier
 
-            - Should be a single 1D array if :class:`.CategoricalHMM` is being used, or either a 1D or 2D array if :class:`.GaussianMixtureHMM` is being used.
-            - Should have length as the 1st dimension and features as the 2nd dimension.
-            - Should be a concatenated sequence if multiple sequences are provided,
-              with respective sequence lengths being provided in the ``lengths`` argument for decoding the original sequences.
+        X:
+            Sequence(s).
 
-        :param y: Classes corresponding to sequence(s) provided in ``X``.
+        y:
+            Classes corresponding to sequence(s) in ``X``.
 
-        :param lengths: Lengths of the observation sequence(s) provided in ``X``.
+        lengths:
+            Lengths of the sequence(s) provided in ``X``.
 
-            - If ``None``, then ``X`` is assumed to be a single observation sequence.
+            - If ``None``, then ``X`` is assumed to be a single sequence.
             - ``len(X)`` should be equal to ``sum(lengths)``.
 
-        :return: The fitted classifier.
+        Returns
+        -------
+        HMMClassifier
+            The fitted classifier
         """
         if X is None or y is None:
             if len(self.models) == 0:
-                raise RuntimeError(
-                    f'Fitted models must be provided to this {type(self).__name__} instance if no training data is provided - '
-                    'use add_model() to add fitted models to the classifier object'
+                msg = (
+                    "Fitted models must be provided if no training data is "
+                    "provided - use add_model() to add fitted models to the "
+                    "classifier object"
                 )
+                raise RuntimeError(msg)
 
             for label, model in self.models.items():
-                if not _check_is_fitted(model, return_=True):
-                    raise NotFittedError(
-                        f'The model corresponding to label {label} must be pre-fitted if '
-                        f'no training data is provided to this {type(self).__name__} instance'
+                if not _validation.check_is_fitted(model, return_=True):
+                    msg = (
+                        f"The model corresponding to label {label} must be "
+                        "pre-fitted if no training data is provided"
                     )
+                    raise NotFittedError(msg)
 
             if self.classes is not None:
-                # Same logic as _check_classes()
-                classes_np = np.array(self.classes).flatten()
-                if not np.issubdtype(classes_np.dtype, np.integer):
-                    raise TypeError(f'Expected classes to be integers')
-                _, idx = np.unique(classes_np, return_index=True)
-                self.classes_ = classes_np[np.sort(idx)]
+                self._classes = _validation.check_classes(
+                    self.classes, classes=self.classes
+                )
             else:
                 # Fetch classes from provided models
                 self.classes_ = np.array(list(self.models.keys()))
         else:
-            self.classes_ = _check_classes(Array[int].validate_type(y), self.classes)
+            y = _validation.check_y(y, lengths=lengths, dtype=np.int8)
+            self.classes_ = _validation.check_classes(y, classes=self.classes)
 
         # Check that each label has a HMM (and vice versa)
         if set(self.models.keys()) != set(self.classes_):
-            raise ValueError(
-                'Classes in the dataset are not consistent with the added models - '
-                'ensure that every added model corresponds to a class in the dataset'
+            msg = (
+                "Classes in the dataset are not consistent with the added "
+                "models - ensure that every added model corresponds to a "
+                "class in the dataset"
             )
+            raise ValueError(msg)
 
         if X is not None and y is not None:
-            # Iterate through the dataset by class and fit the corresponding model
-            data = self._sequence_classifier_validator(X=X, y=y, lengths=lengths)
-            dataset = SequentialDataset(data.X, data.y, data.lengths, self.classes_)
+            # Iterate through dataset by class and fit the corresponding model
+            dataset = SequentialDataset(
+                X,
+                y,
+                lengths=lengths,
+                classes=self.classes_,
+            )
             for X_c, lengths_c, c in dataset.iter_by_class():
-                self.models[c].fit(X_c, lengths_c)
+                self.models[c].fit(X_c, lengths=lengths_c)
 
         # Set class priors
-        if self.prior is None:
-            self.prior_ = {c:1/len(self.classes_) for c, _ in self.models.items()}
-        elif isinstance(self.prior, str):
-            if self.prior == "frequency":
-                total_seqs = sum(model.n_seqs_ for model in self.models.values())
-                self.prior_ = {c:model.n_seqs_/total_seqs for c, model in self.models.items()}
+        models: t.Iterator[int, BaseHMM] = self.models.items()
+        if self.prior == PriorMode.UNIFORM:
+            self.prior_ = {c: 1 / len(self.classes_) for c, _ in models}
+        elif self.prior == PriorMode.FREQUENCY:
+            total_seqs = sum(mod.n_seqs_ for _, mod in models)
+            self.prior_ = {c: mod.n_seqs_ / total_seqs for c, mod in models}
         elif isinstance(self.prior, dict):
             if set(self.prior.keys()) != set(self.classes_):
-                raise ValueError(
-                    'Classes in the dataset are not consistent with the classes in `prior` - '
-                    'ensure that every provided class prior corresponds to a class in the dataset'
+                msg = (
+                    "Classes in the dataset are not consistent with the "
+                    "classes in `prior` - ensure that every provided class "
+                    "prior corresponds to a class in the dataset"
                 )
+                raise ValueError(msg)
             self.prior_ = self.prior
 
         return self
 
-
-    @_requires_fit
+    @_validation.requires_fit
     def predict(
-        self,
+        self: HMMClassifier,
         X: Array,
-        lengths: Optional[Array[int]] = None
-    ) -> Array[int]:
-        """Predicts classes for the sequence(s) in ``X``.
+        *,
+        lengths: IntArray | None = None,
+    ) -> IntArray:
+        """Predict classes for the sequence(s) in ``X``.
 
-        :param X: Univariate or multivariate observation sequence(s).
+        Parameters
+        ----------
+        self: HMMClassifier
 
-            - Should be a single 1D array if :class:`.CategoricalHMM` is being used, or either a 1D or 2D array if :class:`.GaussianMixtureHMM` is being used.
-            - Should have length as the 1st dimension and features as the 2nd dimension.
-            - Should be a concatenated sequence if multiple sequences are provided,
-              with respective sequence lengths being provided in the ``lengths`` argument for decoding the original sequences.
+        X:
+            Sequence(s).
 
-        :param lengths: Lengths of the observation sequence(s) provided in ``X``.
+        lengths:
+            Lengths of the sequence(s) provided in ``X``.
 
-            - If ``None``, then ``X`` is assumed to be a single observation sequence.
+            - If ``None``, then ``X`` is assumed to be a single sequence.
             - ``len(X)`` should be equal to ``sum(lengths)``.
 
-        :note: This method requires a trained classifier — see :func:`fit`.
-
-        :return: Class predictions.
+        Returns
+        -------
+        numpy.ndarray
+            Class predictions.
+
+        Notes
+        -----
+        This method requires a trained classifier — see :func:`fit`.
         """
-        scores = self.predict_scores(X, lengths)
+        scores = self.predict_scores(X, lengths=lengths)
         max_score_idxs = scores.argmax(axis=1)
         return self.classes_[max_score_idxs]
 
+    @_validation.requires_fit
+    def predict_log_proba(
+        self: HMMClassifier, X: Array, *, lengths: IntArray | None = None
+    ) -> FloatArray:
+        """Predict log un-normalized posterior probabilities for the
+        sequences in ``X``.
+
+        Parameters
+        ----------
+        self: HMMClassifier
 
-    def fit_predict(
-        self,
-        X: Array,
-        y: Array[int],
-        lengths: Optional[Array[int]] = None
-    ) -> Array[int]:
-        """Fits the classifier to the sequence(s) in ``X`` and predicts classes for ``X``.
-
-        :param X: Univariate or multivariate observation sequence(s).
-
-            - Should be a single 1D array if :class:`.CategoricalHMM` is being used, or either a 1D or 2D array if :class:`.GaussianMixtureHMM` is being used.
-            - Should have length as the 1st dimension and features as the 2nd dimension.
-            - Should be a concatenated sequence if multiple sequences are provided,
-              with respective sequence lengths being provided in the ``lengths`` argument for decoding the original sequences.
-
-        :param y: Classes corresponding to sequence(s) provided in ``X``.
+        X:
+            Sequence(s).
 
-        :param lengths: Lengths of the observation sequence(s) provided in ``X``.
+        lengths:
+            Lengths of the sequence(s) provided in ``X``.
 
-            - If ``None``, then ``X`` is assumed to be a single observation sequence.
+            - If ``None``, then ``X`` is assumed to be a single sequence.
             - ``len(X)`` should be equal to ``sum(lengths)``.
 
-        :return: Class predictions.
+        Returns
+        -------
+        numpy.ndarray:
+            Log probabilities.
+
+        Notes
+        -----
+        This method requires a trained classifier — see :func:`fit`.
         """
-        return super().fit_predict(X, y, lengths)
-
+        return self.predict_scores(X, lengths=lengths)
 
-    @_requires_fit
+    @_validation.requires_fit
     def predict_proba(
-        self,
-        X: Array,
-        lengths: Optional[Array[int]] = None
-    ) -> Array[confloat(ge=0, le=1)]:
-        """Predicts class probabilities for the sequence(s) in ``X``.
+        self: HMMClassifier, X: Array, *, lengths: IntArray | None = None
+    ) -> FloatArray:
+        """Predict class probabilities for the sequence(s) in ``X``.
 
-        Probabilities are calculated as the posterior probability of each HMM generating the sequence.
+        Probabilities are calculated as the posterior probability of each
+        HMM generating the sequence.
 
-        :param X: Univariate or multivariate observation sequence(s).
+        Parameters
+        ----------
+        self: HMMClassifier
 
-            - Should be a single 1D array if :class:`.CategoricalHMM` is being used, or either a 1D or 2D array if :class:`.GaussianMixtureHMM` is being used.
-            - Should have length as the 1st dimension and features as the 2nd dimension.
-            - Should be a concatenated sequence if multiple sequences are provided,
-              with respective sequence lengths being provided in the ``lengths`` argument for decoding the original sequences.
+        X:
+            Sequence(s).
 
-        :param lengths: Lengths of the observation sequence(s) provided in ``X``.
+        lengths:
+            Lengths of the sequence(s) provided in ``X``.
 
-            - If ``None``, then ``X`` is assumed to be a single observation sequence.
+            - If ``None``, then ``X`` is assumed to be a single sequence.
             - ``len(X)`` should be equal to ``sum(lengths)``.
 
-        :note: This method requires a trained classifier — see :func:`fit`.
-
-        :return: Class membership probabilities.
+        Returns
+        -------
+        numpy.ndarray:
+            Class membership probabilities.
+
+        Notes
+        -----
+        This method requires a trained classifier — see :func:`fit`.
         """
-        proba = self.predict_scores(X, lengths)
+        proba = self.predict_log_proba(X, lengths=lengths)
         proba -= proba.max(axis=1, keepdims=True)
         proba = np.exp(proba)
         proba /= proba.sum(axis=1, keepdims=True)
         return proba
 
-
-    @_requires_fit
+    @_validation.requires_fit
     def predict_scores(
-        self,
-        X: Array,
-        lengths: Optional[Array[int]] = None
-    ) -> Array[float]:
-        """Predicts class scores for the sequence(s) in ``X``.
+        self: HMMClassifier, X: Array, *, lengths: IntArray | None = None
+    ) -> FloatArray:
+        """Predict class scores for the sequence(s) in ``X``.
 
-        Scores are calculated as the log posterior probability of each HMM generating the sequence.
+        Scores are calculated as the log posterior probability of each HMM
+        generating the sequence.
 
-        :param X: Univariate or multivariate observation sequence(s).
+        Parameters
+        ----------
+        self: HMMClassifier
 
-            - Should be a single 1D array if :class:`.CategoricalHMM` is being used, or either a 1D or 2D array if :class:`.GaussianMixtureHMM` is being used.
-            - Should have length as the 1st dimension and features as the 2nd dimension.
-            - Should be a concatenated sequence if multiple sequences are provided,
-              with respective sequence lengths being provided in the ``lengths`` argument for decoding the original sequences.
+        X:
+            Sequence(s).
 
-        :param lengths: Lengths of the observation sequence(s) provided in ``X``.
+        lengths:
+            Lengths of the sequence(s) provided in ``X``.
 
-            - If ``None``, then ``X`` is assumed to be a single observation sequence.
+            - If ``None``, then ``X`` is assumed to be a single sequence.
             - ``len(X)`` should be equal to ``sum(lengths)``.
 
-        :note: This method requires a trained classifier — see :func:`fit`.
-
-        :return: Class scores.
-        """
-        data = self._base_sequence_validator(X=X, lengths=lengths)
-        n_jobs = _effective_n_jobs(self.n_jobs, data.lengths)
-        chunk_idxs = np.array_split(SequentialDataset._get_idxs(data.lengths), n_jobs)
+        Returns
+        -------
+        numpy.ndarray:
+            Class scores.
+
+        Notes
+        -----
+        This method requires a trained classifier — see :func:`fit`.
+        """
+        model: BaseHMM = next(iter(self.models.values()))
+        X, lengths = _validation.check_X_lengths(
+            X,
+            lengths=lengths,
+            dtype=model._DTYPE,  # noqa: SLF001
+        )
+        n_jobs = _multiprocessing.effective_n_jobs(self.n_jobs, x=lengths)
+        chunk_idxs = np.array_split(_data.get_idxs(lengths), n_jobs)
         return np.concatenate(
-            Parallel(n_jobs=n_jobs, max_nbytes=None)(
-                delayed(self._compute_scores_chunk)(idxs, data.X)
+            joblib.Parallel(n_jobs=n_jobs, max_nbytes=None)(
+                joblib.delayed(self._compute_scores_chunk)(X, idxs=idxs)
                 for idxs in chunk_idxs
             )
         )
 
-
-    @_requires_fit
-    def score(
-        self,
-        X: Array,
-        y: Array[int],
-        lengths: Optional[Array[int]],
-        normalize: bool = True,
-        sample_weight: Optional[Array] = None,
-    ) -> float:
-        """Calculates accuracy for the sequence(s) in ``X``.
-
-        :param X: Univariate or multivariate observation sequence(s).
-
-            - Should be a single 1D array if :class:`.CategoricalHMM` is being used, or either a 1D or 2D array if :class:`.GaussianMixtureHMM` is being used.
-            - Should have length as the 1st dimension and features as the 2nd dimension.
-            - Should be a concatenated sequence if multiple sequences are provided,
-              with respective sequence lengths being provided in the ``lengths`` argument for decoding the original sequences.
-
-        :param y: Classes corresponding to the observation sequence(s) in ``X``.
-
-        :param lengths: Lengths of the observation sequence(s) provided in ``X``.
-
-            - If ``None``, then ``X`` is assumed to be a single observation sequence.
-            - ``len(X)`` should be equal to ``sum(lengths)``.
-
-        :param normalize: See :func:`sklearn:sklearn.metrics.accuracy_score`.
-
-        :param sample_weight: See :func:`sklearn:sklearn.metrics.accuracy_score`.
-
-        :note: This method requires a trained classifier — see :func:`fit`.
-
-        :return: Classification accuracy.
-        """
-        return super().score(X, y, lengths, normalize, sample_weight)
-
-
-    @_validate_params(using=_HMMClassifierValidator)
-    @_override_params(_HMMClassifierValidator.fields(), temporary=False)
-    def set_params(self, **kwargs) -> HMMClassifier:
-        return self
-
-
-    def _compute_scores_chunk(self, idxs, X):
-        scores = np.zeros((len(idxs), len(self.classes_)))
-        for i, x in enumerate(SequentialDataset._iter_X(X, idxs)):
-            scores[i] = self._compute_log_posterior(x)
-        return scores
-
-
-    def _compute_log_posterior(self, x):
-        log_posterior = np.full(len(self.classes_), -np.inf)
-        for i, k in enumerate(self.classes_):
-            model = self.models[k]
-            log_prior = np.log(self.prior_[k])
-            log_likelihood = model._score(x)
-            log_posterior[i] = log_prior + log_likelihood
-        return log_posterior
-
-
-    def _base_sequence_validator(self, **kwargs):
-        model = self.models[0]
-        return model._base_sequence_validator(**kwargs)
-
-
-    def _sequence_classifier_validator(self, **kwargs):
-        model = self.models[0]
-        return model._sequence_classifier_validator(**kwargs)
-
-
-    @_requires_fit
-    def save(self, path: Union[str, pathlib.Path, IO]):
-        """Serializes and saves a fitted HMM classifier.
-
-        :param path: Location to save the serialized classifier.
-
-        :note: This method requires a trained classifier — see :func:`fit`.
+    @_validation.requires_fit
+    def save(self: HMMClassifier, path: str | pathlib.Path | t.IO, /) -> None:
+        """Serialize and save a fitted HMM classifier.
+
+        Parameters
+        ----------
+        self: HMMClassifier
+
+        path:
+            Location to save the serialized classifier.
+
+        Notes
+        -----
+        This method requires a trained classifier — see :func:`fit`.
 
         See Also
         --------
         load:
-            Loads and deserializes a fitted HMM classifier.
+            Load and deserialize a fitted HMM classifier.
         """
         # Fetch main parameters and fitted values
+        dict_ = self.__dict__.items()
         state = {
-            'params': self.get_params(),
-            'models': self.models,
-            'fitted': {k:v for k, v in self.__dict__.items() if k.endswith('_')}
+            "params": self.get_params(),
+            "models": self.models,
+            "fitted": {k: v for k, v in dict_ if k.endswith("_")},
         }
 
         # Serialize model
         joblib.dump(state, path)
 
-
     @classmethod
-    def load(cls, path: Union[str, pathlib.Path, IO]) -> HMMClassifier:
-        """Loads and deserializes a fitted HMM classifier.
-
-        :param path: Location to load the serialized classifier from.
+    def load(
+        cls: type[HMMClassifier],
+        path: str | pathlib.Path | t.IO,
+        /,
+    ) -> HMMClassifier:
+        """Load and deserialize a fitted HMM classifier.
 
-        :return: Fitted HMM classifier.
+        Parameters
+        ----------
+        cls: type[HMMClassifier]
+
+        path:
+            Location to load the serialized classifier from.
+
+        Returns
+        -------
+        HMMClassifier
+            Fitted HMM classifier.
 
         See Also
         --------
         save:
-            Serializes and saves a fitted HMM classifier.
+            Serialize and save a fitted HMM classifier.
         """
         state = joblib.load(path)
 
         # Set main parameters
-        model = cls(**state['params'])
-        model.models = state['models']
+        model = cls(**state["params"])
+        model.models = state["models"]
 
         # Set fitted values
-        for k, v in state['fitted'].items():
+        for k, v in state["fitted"].items():
             setattr(model, k, v)
 
         # Return deserialized model
         return model
+
+    def _compute_scores_chunk(
+        self: HMMClassifier, X: Array, /, *, idxs: IntArray
+    ) -> FloatArray:
+        """Compute log posterior probabilities for a chunk of sequences."""
+        scores = np.zeros((len(idxs), len(self.classes_)))
+        for i, x in enumerate(_data.iter_X(X, idxs=idxs)):
+            scores[i] = self._compute_log_posterior(x)
+        return scores
+
+    def _compute_log_posterior(
+        self: HMMClassifier,
+        x: Array,
+        /,
+    ) -> FloatArray:
+        """Compute log posterior probabilities for each class."""
+        log_posterior = np.full(len(self.classes_), -np.inf)
+        for i, k in enumerate(self.classes_):
+            model = self.models[k]
+            log_prior = np.log(self.prior_[k])
+            log_likelihood = model.score(x)
+            log_posterior[i] = log_prior + log_likelihood
+        return log_posterior
```

### Comparing `sequentia-1.1.1/lib/sequentia/models/hmm/topologies.py` & `sequentia-2.0.0/sequentia/_internal/_hmm/topologies.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,263 +1,343 @@
+# Copyright (c) 2019-2025 Sequentia Developers.
+# Distributed under the terms of the MIT License (see the LICENSE file).
+# SPDX-License-Identifier: MIT
+# This source code is part of the Sequentia project (https://github.com/eonu/sequentia).
+
+from __future__ import annotations
+
 import warnings
 
 import numpy as np
 
-class _Topology:
-    """Represents a topology for a HMM, imposing restrictions on the transition matrix and initial state distribution.
+from sequentia._internal._validation import FloatArray
+from sequentia.enums import TopologyMode
+
+__all__ = [
+    "ErgodicTopology",
+    "LeftRightTopology",
+    "LinearTopology",
+    "TOPOLOGY_MAP",
+]
+
+
+class BaseTopology:
+    """Represents a topology for a HMM, imposing restrictions on the
+    transition matrix and initial state distribution.
 
     Parameters
     ----------
     n_states: int
         Number of states in the HMM.
 
     random_state: numpy.random.RandomState
         A random state object for reproducible randomness.
     """
 
-    def __init__(self, n_states: int, random_state: np.random.RandomState):
+    mode: TopologyMode
+
+    def __init__(
+        self: BaseTopology,
+        *,
+        n_states: int,
+        random_state: np.random.RandomState,
+    ) -> BaseTopology:
         self.n_states = n_states
         self.random_state = random_state
 
-    def uniform_start_probs(self) -> np.ndarray:
-        """Sets the initial state distribution as a discrete uniform distribution.
+    def uniform_start_probs(self: BaseTopology) -> FloatArray:
+        """Set the initial state distribution as a discrete uniform
+        distribution.
 
         Returns
         -------
         initial: :class:`numpy:numpy.ndarray` (float)
             The initial state distribution of shape `(n_states,)`.
         """
         return np.ones(self.n_states) / self.n_states
 
-    def random_start_probs(self) -> np.ndarray:
-        """Sets the initial state distribution by randomly sampling probabilities generated by a Dirichlet distribution.
+    def random_start_probs(self: BaseTopology) -> FloatArray:
+        """Set the initial state distribution by randomly sampling
+        probabilities generated by a Dirichlet distribution.
 
         Returns
         -------
         initial: :class:`numpy:numpy.ndarray` (float)
             The initial state distribution of shape `(n_states,)`.
         """
-        return self.random_state.dirichlet(np.ones(self.n_states), size=1).flatten()
-
-    def uniform_transitions(self) -> np.ndarray:
-        """Sets the transition matrix as uniform (equal probability of transitioning
-        to all other possible states from each state) corresponding to the topology.
+        return self.random_state.dirichlet(
+            np.ones(self.n_states),
+            size=1,
+        ).flatten()
+
+    def uniform_transition_probs(self: BaseTopology) -> FloatArray:
+        """Set the transition matrix as uniform (equal probability of
+        transitioning to all other possible states from each state)
+        corresponding to the topology.
 
         Returns
         -------
         transitions: :class:`numpy:numpy.ndarray` (float)
             The uniform transition matrix of shape `(n_states, n_states)`.
         """
         raise NotImplementedError
 
-    def random_transitions(self) -> np.ndarray:
-        """Sets the transition matrix as random (random probability of transitioning
-        to all other possible states from each state) by sampling probabilities
-        from a Dirichlet distribution - according to the topology.
+    def random_transition_probs(self: BaseTopology) -> FloatArray:
+        """Set the transition matrix as random (random probability of
+        transitioning to all other possible states from each state) by
+        sampling probabilitiesfrom a Dirichlet distribution - according
+        to the topology.
 
         Returns
         -------
         transitions: :class:`numpy:numpy.ndarray` (float)
             The random transition matrix of shape `(n_states, n_states)`.
         """
         raise NotImplementedError
 
-    def check_start_probs(self, initial: np.ndarray) -> None:
-        """Validates an initial state distribution according to the topology's restrictions.
+    def check_start_probs(self: BaseTopology, initial: FloatArray, /) -> None:
+        """Validate an initial state distribution according to the
+        topology's restrictions.
 
         Parameters
         ----------
         initial: numpy.ndarray (float)
             The initial state distribution to validate.
         """
         if not isinstance(initial, np.ndarray):
-            raise TypeError('Initial state distribution must be a numpy.ndarray')
-        if not initial.shape == (self.n_states,):
-            raise ValueError('Initial state distribution must be of shape (n_states,)')
+            msg = "Initial state distribution must be a numpy.ndarray"
+            raise TypeError(msg)
+        if initial.shape != (self.n_states,):
+            msg = "Initial state distribution must be of shape (n_states,)"
+            raise ValueError(msg)
         if not np.isclose(initial.sum(), 1):
-            raise ValueError('Initial state distribution must sum to one')
+            msg = "Initial state distribution must sum to one"
+            raise ValueError(msg)
         return initial
 
-    def check_transitions(self, transitions: np.ndarray) -> np.ndarray:
-        """Validates a transition matrix according to the topology's restrictions.
+    def check_transition_probs(
+        self: BaseTopology, transitions: FloatArray, /
+    ) -> FloatArray:
+        """Validate a transition matrix according to the topology's
+        restrictions.
 
         Parameters
         ----------
         transitions: numpy.ndarray (float)
             The transition matrix to validate.
         """
         if not isinstance(transitions, np.ndarray):
-            raise TypeError('Transition matrix must be a numpy.ndarray')
-        if not transitions.shape == (self.n_states, self.n_states):
-            raise ValueError('Transition matrix must be of shape (n_states, n_states)')
+            msg = "Transition matrix must be a numpy.ndarray"
+            raise TypeError(msg)
+        if transitions.shape != (self.n_states, self.n_states):
+            msg = "Transition matrix must be of shape (n_states, n_states)"
+            raise ValueError(msg)
         if not np.allclose(transitions.sum(axis=1), np.ones(self.n_states)):
-            raise ValueError('Transition probabilities out of each state must sum to one')
+            msg = "Transition probabilities out of each state must sum to one"
+            raise ValueError(msg)
         return transitions
 
-class _ErgodicTopology(_Topology):
-    """Represents the topology for an ergodic HMM, imposing non-zero probabilities in the transition matrix.
+
+class ErgodicTopology(BaseTopology):
+    """Represents the topology for an ergodic HMM, imposing non-zero
+    probabilities in the transition matrix.
 
     Parameters
     ----------
     n_states: int
         Number of states in the HMM.
 
     random_state: numpy.random.RandomState
         A random state object for reproducible randomness.
     """
 
-    name = "ergodic"
+    mode: TopologyMode = TopologyMode.ERGODIC
 
-    def uniform_transitions(self) -> np.ndarray:
-        """Sets the transition matrix as uniform (equal probability of transitioning
-            to all other possible states from each state) corresponding to the topology.
+    def uniform_transition_probs(self: ErgodicTopology) -> FloatArray:
+        """Set the transition matrix as uniform (equal probability of
+        transitioning to all other possible states from each state)
+        corresponding to the topology.
 
         Returns
         -------
         transitions: :class:`numpy:numpy.ndarray` (float)
             The uniform transition matrix of shape `(n_states, n_states)`.
         """
         return np.ones((self.n_states, self.n_states)) / self.n_states
 
-    def random_transitions(self) -> np.ndarray:
-        """Sets the transition matrix as random (random probability of transitioning
-        to all other possible states from each state) by sampling probabilities
-        from a Dirichlet distribution - according to the topology.
+    def random_transition_probs(self: ErgodicTopology) -> FloatArray:
+        """Set the transition matrix as random (random probability of
+        transitioning to all other possible states from each state) by
+        sampling probabilities from a Dirichlet distribution - according
+        to the topology.
 
         Returns
         -------
         transitions: :class:`numpy:numpy.ndarray` (float)
             The random transition matrix of shape `(n_states, n_states)`.
         """
-        return self.random_state.dirichlet(np.ones(self.n_states), size=self.n_states)
-
-    def check_transitions(self, transitions: np.ndarray) -> np.ndarray:
-        """Validates a transition matrix according to the topology's restrictions.
+        return self.random_state.dirichlet(
+            np.ones(self.n_states),
+            size=self.n_states,
+        )
+
+    def check_transition_probs(
+        self: ErgodicTopology, transitions: FloatArray, /
+    ) -> FloatArray:
+        """Validate a transition matrix according to the topology's
+        restrictions.
 
         Parameters
         ----------
         transitions: numpy.ndarray (float)
             The transition matrix to validate.
         """
-        super().check_transitions(transitions)
+        super().check_transition_probs(transitions)
         if not np.all(transitions > 0):
-            warnings.warn('Zero probabilities in ergodic transition matrix - these transition probabilities will not be learned')
+            msg = (
+                "Zero probabilities in ergodic transition matrix - "
+                "these transition probabilities will not be learned"
+            )
+            warnings.warn(msg, stacklevel=1)
         return transitions
 
-class _LeftRightTopology(_Topology):
-    """Represents the topology for a left-right HMM, imposing an upper-triangular transition matrix.
+
+class LeftRightTopology(BaseTopology):
+    """Represents the topology for a left-right HMM, imposing an
+    upper-triangular transition matrix.
 
     Parameters
     ----------
     n_states: int
         Number of states in the HMM.
 
     random_state: numpy.random.RandomState
         A random state object for reproducible randomness.
     """
 
-    name = "left-right"
+    mode: TopologyMode = TopologyMode.LEFT_RIGHT
 
-    def uniform_transitions(self) -> np.ndarray:
-        """Sets the transition matrix as uniform (equal probability of transitioning
-            to all other possible states from each state) corresponding to the topology.
+    def uniform_transition_probs(self: LeftRightTopology) -> FloatArray:
+        """Set the transition matrix as uniform (equal probability of
+        transitioning to all other possible states from each state)
+        corresponding to the topology.
 
         Returns
         -------
         transitions: :class:`numpy:numpy.ndarray` (float)
             The uniform transition matrix of shape `(n_states, n_states)`.
         """
         upper_ones = np.triu(np.ones((self.n_states, self.n_states)))
-        upper_divisors = np.triu(np.tile(np.arange(self.n_states, 0, -1), (self.n_states, 1)).T)
+        upper_divisors = np.triu(
+            np.tile(np.arange(self.n_states, 0, -1), (self.n_states, 1)).T
+        )
         lower_ones = np.tril(np.ones(self.n_states), k=-1)
         return upper_ones / (upper_divisors + lower_ones)
 
-    def random_transitions(self) -> np.ndarray:
-        """Sets the transition matrix as random (random probability of transitioning
-        to all other possible states from each state) by sampling probabilities
-        from a Dirichlet distribution, according to the topology.
+    def random_transition_probs(self: LeftRightTopology) -> FloatArray:
+        """Set the transition matrix as random (random probability of
+        transitioning to all other possible states from each state) by
+        sampling probabilities from a Dirichlet distribution, according
+        to the topology.
 
         Returns
         -------
         transitions: :class:`numpy:numpy.ndarray` (float)
             The random transition matrix of shape `(n_states, n_states)`.
         """
         transitions = np.zeros((self.n_states, self.n_states))
         for i, row in enumerate(transitions):
             row[i:] = self.random_state.dirichlet(np.ones(self.n_states - i))
         return transitions
 
-    def check_transitions(self, transitions: np.ndarray) -> np.ndarray:
-        """Validates a transition matrix according to the topology's restrictions.
+    def check_transition_probs(
+        self: LeftRightTopology, transitions: FloatArray, /
+    ) -> FloatArray:
+        """Validate a transition matrix according to the topology's
+        restrictions.
 
         Parameters
         ----------
         transitions: numpy.ndarray (float)
             The transition matrix to validate.
         """
-        super().check_transitions(transitions)
+        super().check_transition_probs(transitions)
         if not np.allclose(transitions, np.triu(transitions)):
-            raise ValueError('Left-right transition matrix must be upper-triangular')
+            msg = "Left-right transition matrix must be upper-triangular"
+            raise ValueError(msg)
         return transitions
 
-class _LinearTopology(_LeftRightTopology):
+
+class LinearTopology(LeftRightTopology):
     """Represents the topology for a linear HMM.
 
     Parameters
     ----------
     n_states: int
         Number of states in the HMM.
 
     random_state: numpy.random.RandomState
         A random state object for reproducible randomness.
     """
 
-    name = "linear"
+    mode: TopologyMode = TopologyMode.LINEAR
 
-    def uniform_transitions(self) -> np.ndarray:
-        """Sets the transition matrix as uniform (equal probability of transitioning
-            to all other possible states from each state) corresponding to the topology.
+    def uniform_transition_probs(self: LinearTopology) -> FloatArray:
+        """Set the transition matrix as uniform (equal probability of
+        transitioning to all other possible states from each state)
+        corresponding to the topology.
 
         Returns
         -------
         transitions: :class:`numpy:numpy.ndarray` (float)
             The uniform transition matrix of shape `(n_states, n_states)`.
         """
         transitions = np.zeros((self.n_states, self.n_states))
         for i, row in enumerate(transitions):
             size = min(2, self.n_states - i)
-            row[i:(i + size)] = np.ones(size) / size
+            row[i : (i + size)] = np.ones(size) / size
         return transitions
 
-    def random_transitions(self) -> np.ndarray:
-        """Sets the transition matrix as random (random probability of transitioning
-        to all other possible states from each state) by sampling probabilities
-        from a Dirichlet distribution, according to the topology.
+    def random_transition_probs(self: LinearTopology) -> FloatArray:
+        """Set the transition matrix as random (random probability of
+        transitioning to all other possible states from each state) by
+        sampling probabilities from a Dirichlet distribution, according to the
+        topology.
 
         Returns
         -------
         transitions: :class:`numpy:numpy.ndarray` (float)
             The random transition matrix of shape `(n_states, n_states)`.
         """
         transitions = np.zeros((self.n_states, self.n_states))
         for i, row in enumerate(transitions):
             size = min(2, self.n_states - i)
-            row[i:(i + size)] = self.random_state.dirichlet(np.ones(size))
+            row[i : (i + size)] = self.random_state.dirichlet(np.ones(size))
         return transitions
 
-    def check_transitions(self, transitions: np.ndarray) -> np.ndarray:
-        """Validates a transition matrix according to the topology's restrictions.
+    def check_transition_probs(
+        self: LinearTopology, transitions: FloatArray, /
+    ) -> FloatArray:
+        """Validate a transition matrix according to the topology's
+        restrictions.
 
         Parameters
         ----------
         transitions: numpy.ndarray (float)
             The transition matrix to validate.
         """
-        super().check_transitions(transitions)
-        if not np.allclose(transitions, np.diag(np.diag(transitions)) + np.diag(np.diag(transitions, k=1), k=1)):
-            raise ValueError('Linear transition matrix must only consist of a diagonal and upper diagonal')
+        super().check_transition_probs(transitions)
+        diagonal = np.diag(np.diag(transitions))
+        upper_diagonal = np.diag(np.diag(transitions, k=1), k=1)
+        if not np.allclose(transitions, diagonal + upper_diagonal):
+            msg = (
+                "Linear transition matrix must only consist of "
+                "a diagonal and upper diagonal"
+            )
+            raise ValueError(msg)
         return transitions
 
-_topologies = {
-    topology.name:topology
-    for topology in (_ErgodicTopology, _LeftRightTopology, _LinearTopology)
+
+TOPOLOGY_MAP = {
+    topology.mode: topology
+    for topology in (ErgodicTopology, LeftRightTopology, LinearTopology)
 }
```

### Comparing `sequentia-1.1.1/lib/sequentia/models/knn/classifier.py` & `sequentia-2.0.0/sequentia/models/knn/classifier.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,48 +1,39 @@
+# Copyright (c) 2019-2025 Sequentia Developers.
+# Distributed under the terms of the MIT License (see the LICENSE file).
+# SPDX-License-Identifier: MIT
+# This source code is part of the Sequentia project (https://github.com/eonu/sequentia).
+
+"""A k-nearest neighbor classifier that uses DTW as a distance measure for
+sequence comparison.
+"""
+
 from __future__ import annotations
 
-from types import SimpleNamespace
-from typing import Optional, Union, Callable
-from joblib import Parallel, delayed
+import typing as t
 
+import joblib
+import numba
 import numpy as np
-from pydantic import NegativeInt, NonNegativeInt, PositiveInt, confloat
-from numba import njit, prange
-from sklearn.utils import check_random_state
-
-from sequentia.models.knn.base import _KNNMixin, _KNNValidator
-from sequentia.models.base import _Classifier
-
-from sequentia.utils.decorators import _validate_params, _requires_fit, _override_params
-from sequentia.utils.data import SequentialDataset
-from sequentia.utils.multiprocessing import _effective_n_jobs
-from sequentia.utils.validation import (
-    _check_classes,
-    Array,
-    _MultivariateFloatSequenceClassifierValidator
-)
-
-__all__ = ['KNNClassifier']
+import pydantic as pyd
 
-_defaults = SimpleNamespace(
-    **{
-        **_KNNMixin._defaults.__dict__,
-        "classes": None,
-    }
-)
+from sequentia._internal import _data, _multiprocessing, _validation
+from sequentia._internal._typing import Array, FloatArray, IntArray
+from sequentia.models.base import ClassifierMixin
+from sequentia.models.knn.base import KNNMixin
 
+__all__ = ["KNNClassifier"]
 
-class _KNNClassifierValidator(_KNNValidator):
-    classes: Optional[Array[int]] = _defaults.classes
 
+class KNNClassifier(KNNMixin, ClassifierMixin):
+    """A k-nearest neighbor classifier that uses DTW as a distance measure for
+    sequence comparison.
 
-class KNNClassifier(_KNNMixin, _Classifier):
-    """A k-nearest neighbor classifier that uses DTW as a distance measure for sequence comparison.
-
-    The classifier computes the score for each class as the total of the distance weightings of every sequence belonging to that class,
+    The classifier computes the score for each class as the total of the
+    distance weightings of every sequence belonging to that class,
     within the DTW k-neighborhood of the sequence being classified.
 
     Examples
     --------
     Using a :class:`.KNNClassifier` to classify spoken digits. ::
 
         import numpy as np
@@ -56,340 +47,388 @@
         data = load_digits()
         train_data, test_data = data.split(test_size=0.2, random_state=random_state)
 
         # Create a HMMClassifier using a class frequency prior
         clf = KNNClassifier()
 
         # Fit the classifier
-        X_train, y_train, lengths_train = train_data.X_y_lengths
-        clf.fit(X_train, y_train, lengths_train)
+        clf.fit(train_data.X, train_data.y, lengths=train_data.lengths)
 
         # Predict classes for the test observation sequences
-        X_test, lengths_test = test_data.X_lengths
-        y_pred = clf.predict(X_test, lengths_test)
-    """
-
-    _defaults = _defaults
+        y_pred = clf.predict(test_data.X, lengths=test_data.lengths)
+    """  # noqa: E501
 
-
-    @_validate_params(using=_KNNClassifierValidator)
+    @pyd.validate_call(config=dict(arbitrary_types_allowed=True))
     def __init__(
-        self,
+        self: pyd.SkipValidation,
         *,
-        k: PositiveInt = _defaults.k,
-        weighting: Optional[Callable] = _defaults.weighting,
-        window: confloat(ge=0, le=1) = _defaults.window,
-        independent: bool = _defaults.independent,
-        classes: Optional[Array[int]] = None,
-        use_c: bool = _defaults.use_c,
-        n_jobs: Union[NegativeInt, PositiveInt] = _defaults.n_jobs,
-        random_state: Optional[Union[NonNegativeInt, np.random.RandomState]] = _defaults.random_state
-    ) -> KNNClassifier:
+        k: pyd.PositiveInt = 1,
+        weighting: t.Callable[[FloatArray], FloatArray] | None = None,
+        window: pyd.confloat(ge=0.0, le=1.0) = 1.0,
+        independent: bool = False,
+        use_c: bool = False,
+        n_jobs: pyd.PositiveInt | pyd.NegativeInt = 1,
+        random_state: pyd.NonNegativeInt | np.random.RandomState | None = None,
+        classes: list[int] | None = None,
+    ) -> pyd.SkipValidation:
         """Initializes the :class:`.KNNClassifier`.
 
-        :param k: Number of neighbors.
-
-        :param weighting: A callable that specifies how distance weighting should be performed.
-            The callable should accept a :class:`numpy:numpy.ndarray` of DTW distances, apply an element-wise weighting transformation
-            to the matrix of DTW distances, then return an equally-sized :class:`numpy:numpy.ndarray` of weightings.
-            If ``None``, then a uniform weighting of 1 will be applied to all distances.
-
-        :param window: The size of the Sakoe—Chiba band global constrant as a fraction of the length of the shortest of the two sequences being compared.
-
-            - A larger window will give more freedom to the DTW alignment, allowing more deviation but leading to potentially slower computation.
-              A window of 1 is equivalent to full DTW computation with no global constraint applied.
-            - A smaller window will restrict the DTW alignment, and possibly speed up the DTW computation.
+        Parameters
+        ----------
+        self: KNNClassifier
+
+        k:
+            Number of neighbors.
+
+        weighting:
+            A callable that specifies how distance weighting should be
+            performed.
+
+            The callable should accept a :class:`numpy:numpy.ndarray` of DTW
+            distances, apply an element-wise weighting transformation to the
+            matrix of DTW distances, then return an equally-sized
+            :class:`numpy:numpy.ndarray` of weightings.
+
+            If ``None``, then a uniform weighting of 1 will be applied to all
+            distances.
+
+        window:
+            The size of the Sakoe—Chiba band global constrant as a fraction
+            of the length of the shortest of the two sequences being compared.
+
+            - A larger window will give more freedom to the DTW alignment,
+              allowing more deviation but leading to potentially slower
+              computation.
+              A window of 1 is equivalent to full DTW computation with no
+              global constraint applied.
+            - A smaller window will restrict the DTW alignment, and possibly
+              speed up the DTW computation.
               A window of 0 is equivalent to Euclidean distance.
 
-        :param independent: Whether or not to allow features to be warped independently from each other. See [#dtw_multi]_ for an overview of independent and dependent dynamic time warping.
-
-        :param classes: Set of possible class labels.
-
-            - If not provided, these will be determined from the training data labels.
-            - If provided, output from methods such as :func:`predict_proba` and :func:`predict_scores`
-              will follow the ordering of the class labels provided here.
-
-        :param use_c: Whether or not to use fast pure C compiled functions from `dtaidistance <https://github.com/wannesm/dtaidistance>`__ to perform the DTW computations.
+        independent:
+            Whether or not to allow features to be warped independently from
+            each other. See [#dtw_multi]_ for an overview of independent and
+            dependent dynamic time warping.
+
+        use_c:
+            Whether or not to use fast pure C compiled functions from
+            `dtaidistance <https://github.com/wannesm/dtaidistance>`__ to
+            perform the DTW computations.
 
-        :param n_jobs: Maximum number of concurrently running workers.
+        n_jobs:
+            Maximum number of concurrently running workers.
 
             - If 1, no parallelism is used at all (useful for debugging).
             - If -1, all CPUs are used.
-            - If < -1, ``(n_cpus + 1 + n_jobs)`` are used — e.g. ``n_jobs=-2`` uses all but one.
+            - If < -1, ``(n_cpus + 1 + n_jobs)`` are used — e.g. ``n_jobs=-2``
+              uses all but one.
 
-        :param random_state: Seed or :class:`numpy:numpy.random.RandomState` object for reproducible pseudo-randomness.
+        random_state:
+            Seed or :class:`numpy:numpy.random.RandomState` object for
+            reproducible pseudo-randomness.
+
+        classes:
+            Set of possible class labels.
+
+            - If not provided, these will be determined from the training data
+              labels.
+            - If provided, output from methods such as :func:`predict_proba`
+              and :func:`predict_scores` will follow the ordering of the class
+              labels provided here.
+
+        Returns
+        -------
+        KNNClassifier
         """
-        #: Number of neighbors.
-        self.k = k
-        #: A callable that specifies how distance weighting should be performed.
-        self.weighting = weighting
-        #: The size of the Sakoe—Chiba band global constrant as a fraction of the length of the shortest of the two sequences being compared.
-        self.window = window
-        #: Whether or not to allow features to be warped independently from each other.
-        self.independent = independent
-        #: Set of possible class labels.
-        self.classes = classes
-        #: Whether or not to use fast pure C compiled functions from `dtaidistance <https://github.com/wannesm/dtaidistance>`__ to perform the DTW computations.
-        self.use_c = use_c
-        #: Maximum number of concurrently running workers.
-        self.n_jobs = n_jobs
-        #: Seed or :class:`numpy:numpy.random.RandomState` object for reproducible pseudo-randomness.
-        self.random_state = random_state
+        self.k: int = k
+        """Number of neighbors."""
 
+        self.weighting: t.Callable[[np.ndarray], np.ndarray] | None = (
+            weighting  # placeholder
+        )
+        """A callable that specifies how distance weighting should be
+        performed."""
+
+        self.window: float = window
+        """The size of the Sakoe—Chiba band global constrant as a fraction of
+        the length of the shortest of the two sequences being compared."""
+
+        self.independent: bool = independent
+        """Whether or not to allow features to be warped independently from
+        each other."""
+
+        self.use_c: bool = use_c
+        """Whether or not to use fast pure C compiled functions from
+        `dtaidistance <https://github.com/wannesm/dtaidistance>`__ to
+        perform the DTW computations."""
+
+        self.n_jobs: int = n_jobs
+        """Maximum number of concurrently running workers."""
+
+        self.random_state: int | np.random.RandomState | None = random_state
+        """Seed or :class:`numpy:numpy.random.RandomState` object for
+        reproducible pseudo-randomness."""
+
+        self.classes: list[int] | None = classes
+        """Set of possible class labels."""
+
+        # Allow metadata routing for lengths
+        self.set_fit_request(lengths=True)
+        self.set_predict_request(lengths=True)
+        self.set_predict_log_proba_request(lengths=True)
+        self.set_predict_proba_request(lengths=True)
+        self.set_score_request(
+            lengths=True,
+            normalize=True,
+            sample_weight=True,
+        )
 
     def fit(
-        self,
-        X: Array[float],
-        y: Array[int],
-        lengths: Optional[Array[int]] = None
+        self: KNNClassifier,
+        X: FloatArray,
+        y: IntArray,
+        *,
+        lengths: IntArray | None = None,
     ) -> KNNClassifier:
-        """Fits the classifier to the sequence(s) in ``X``.
+        """Fit the classifier to the sequence(s) in ``X``.
 
-        :param X: Univariate or multivariate observation sequence(s).
+        Parameters
+        ----------
+        self: KNNClassifier
 
-            - Should be a single 1D or 2D array.
-            - Should have length as the 1st dimension and features as the 2nd dimension.
-            - Should be a concatenated sequence if multiple sequences are provided,
-              with respective sequence lengths being provided in the ``lengths`` argument for decoding the original sequences.
+        X:
+            Sequence(s).
 
-        :param y: Classes corresponding to sequence(s) provided in ``X``.
+        y:
+            Classes corresponding to sequence(s) in ``X``.
 
-        :param lengths: Lengths of the observation sequence(s) provided in ``X``.
+        lengths:
+            Lengths of the sequence(s) provided in ``X``.
 
-            - If ``None``, then ``X`` is assumed to be a single observation sequence.
+            - If ``None``, then ``X`` is assumed to be a single sequence.
             - ``len(X)`` should be equal to ``sum(lengths)``.
 
-        :return: The fitted classifier.
+        Returns
+        -------
+        KNNClassifier:
+            The fitted classifier.
         """
-        data = _MultivariateFloatSequenceClassifierValidator(X=X, y=y, lengths=lengths)
-        self.X_ = data.X
-        self.y_ = data.y
-        self.lengths_ = data.lengths
-        self.idxs_ = SequentialDataset._get_idxs(data.lengths)
-        self.random_state_ = check_random_state(self.random_state)
-        self.classes_ = _check_classes(data.y, self.classes)
+        self.X_, self.lengths_ = _validation.check_X_lengths(
+            X, lengths=lengths, dtype=self._DTYPE
+        )
+        self.y_ = _validation.check_y(
+            y,
+            lengths=self.lengths_,
+            dtype=np.int8,
+        )
+        self.idxs_ = _data.get_idxs(self.lengths_)
+        self.use_c_ = _validation.check_use_c(self.use_c)
+        self.random_state_ = _validation.check_random_state(self.random_state)
+        self.classes_ = _validation.check_classes(
+            self.y_,
+            classes=self.classes,
+        )
+        _validation.check_weighting(self.weighting)
         return self
 
-
-    @_requires_fit
+    @_validation.requires_fit
     def predict(
-        self,
-        X: Array[float],
-        lengths: Optional[Array[int]] = None
-    ) -> Array[int]:
-        """Predicts classes for the sequence(s) in ``X``.
-
-        :param X: Univariate or multivariate observation sequence(s).
-
-            - Should be a single 1D or 2D array.
-            - Should have length as the 1st dimension and features as the 2nd dimension.
-            - Should be a concatenated sequence if multiple sequences are provided,
-              with respective sequence lengths being provided in the ``lengths`` argument for decoding the original sequences.
+        self: KNNClassifier,
+        X: FloatArray,
+        *,
+        lengths: IntArray | None = None,
+    ) -> IntArray:
+        """Predict classes for the sequence(s) in ``X``.
 
-        :param lengths: Lengths of the observation sequence(s) provided in ``X``.
+        Parameters
+        ----------
+        self: KNNClassifier
 
-            - If ``None``, then ``X`` is assumed to be a single observation sequence.
-            - ``len(X)`` should be equal to ``sum(lengths)``.
+        X:
+            Sequence(s).
 
-        :note: This method requires a trained classifier — see :func:`fit`.
+        lengths:
+            Lengths of the sequence(s) provided in ``X``.
 
-        :return: Class predictions.
+            - If ``None``, then ``X`` is assumed to be a single sequence.
+            - ``len(X)`` should be equal to ``sum(lengths)``.
+
+        Returns
+        -------
+        numpy.ndarray:
+            Class predictions.
+
+        Notes
+        -----
+        This method requires a trained classifier — see :func:`fit`.
         """
-        class_scores = self.predict_scores(X, lengths)
+        class_scores = self.predict_scores(X, lengths=lengths)
         return self._find_max_labels(class_scores)
 
+    @_validation.requires_fit
+    def predict_log_proba(
+        self: KNNClassifier,
+        X: FloatArray,
+        *,
+        lengths: IntArray | None = None,
+    ) -> FloatArray:
+        """Predict log class probabilities for the sequence(s) in ``X``.
+
+        Probabilities are calculated as normalized class scores.
 
-    def fit_predict(
-        self,
-        X: Array[float],
-        y: Array[int],
-        lengths: Optional[Array[int]] = None
-    ) -> Array[int]:
-        """Fits the classifier to the sequence(s) in ``X`` and predicts classes for ``X``.
-
-        :param X: Univariate or multivariate observation sequence(s).
-
-            - Should be a single 1D or 2D array.
-            - Should have length as the 1st dimension and features as the 2nd dimension.
-            - Should be a concatenated sequence if multiple sequences are provided,
-              with respective sequence lengths being provided in the ``lengths`` argument for decoding the original sequences.
+        Parameters
+        ----------
+        self: KNNClassifier
 
-        :param y: Classes corresponding to sequence(s) provided in ``X``.
+        X:
+            Sequence(s).
 
-        :param lengths: Lengths of the observation sequence(s) provided in ``X``.
+        lengths:
+            Lengths of the sequence(s) provided in ``X``.
 
-            - If ``None``, then ``X`` is assumed to be a single observation sequence.
+            - If ``None``, then ``X`` is assumed to be a single sequence.
             - ``len(X)`` should be equal to ``sum(lengths)``.
 
-        :return: Class predictions.
+        Returns
+        -------
+        numpy.ndarray:
+            Class membership log-probabilities.
+
+        Notes
+        -----
+        This method requires a trained classifier — see :func:`fit`.
         """
-        return super().fit_predict(X, y, lengths)
+        return np.log(self.predict_scores(X, lengths=lengths))
 
-
-    @_requires_fit
+    @_validation.requires_fit
     def predict_proba(
-        self,
-        X: Array[float],
-        lengths: Optional[Array[int]] = None
-    ) -> Array[float]:
-        """Predicts class probabilities for the sequence(s) in ``X``.
+        self: KNNClassifier,
+        X: FloatArray,
+        *,
+        lengths: IntArray | None = None,
+    ) -> FloatArray:
+        """Predict class probabilities for the sequence(s) in ``X``.
 
         Probabilities are calculated as normalized class scores.
 
-        :param X: Univariate or multivariate observation sequence(s).
+        Parameters
+        ----------
+        self: KNNClassifier
 
-            - Should be a single 1D or 2D array.
-            - Should have length as the 1st dimension and features as the 2nd dimension.
-            - Should be a concatenated sequence if multiple sequences are provided,
-              with respective sequence lengths being provided in the ``lengths`` argument for decoding the original sequences.
+        X:
+            Sequence(s).
 
-        :param lengths: Lengths of the observation sequence(s) provided in ``X``.
+        lengths:
+            Lengths of the sequence(s) provided in ``X``.
 
-            - If ``None``, then ``X`` is assumed to be a single observation sequence.
+            - If ``None``, then ``X`` is assumed to be a single sequence.
             - ``len(X)`` should be equal to ``sum(lengths)``.
 
-        :note: This method requires a trained classifier — see :func:`fit`.
-
-        :return: Class membership probabilities.
+        Returns
+        -------
+        numpy.ndarray:
+            Class membership probabilities.
+
+        Notes
+        -----
+        This method requires a trained classifier — see :func:`fit`.
         """
-        class_scores = self.predict_scores(X, lengths)
+        class_scores = self.predict_scores(X, lengths=lengths)
         return class_scores / class_scores.sum(axis=1, keepdims=True)
 
-
-    @_requires_fit
+    @_validation.requires_fit
     def predict_scores(
-        self,
-        X: Array[float],
-        lengths: Optional[Array[int]] = None
-    ) -> Array[float]:
-        """Predicts class scores for the sequence(s) in ``X``.
+        self: KNNClassifier,
+        X: FloatArray,
+        *,
+        lengths: IntArray | None = None,
+    ) -> FloatArray:
+        """Predict class scores for the sequence(s) in ``X``.
 
-        Scores are calculated as the class distance weighting sums of all training sequences in the k-neighborhood.
+        Scores are calculated as the class distance weighting sums of all
+        training sequences in the k-neighborhood.
 
-        :param X: Univariate or multivariate observation sequence(s).
+        Parameters
+        ----------
+        self: KNNClassifier
 
-            - Should be a single 1D or 2D array.
-            - Should have length as the 1st dimension and features as the 2nd dimension.
-            - Should be a concatenated sequence if multiple sequences are provided,
-              with respective sequence lengths being provided in the ``lengths`` argument for decoding the original sequences.
+        X:
+            Sequence(s).
 
-        :param lengths: Lengths of the observation sequence(s) provided in ``X``.
+        lengths:
+            Lengths of the sequence(s) provided in ``X``.
 
-            - If ``None``, then ``X`` is assumed to be a single observation sequence.
+            - If ``None``, then ``X`` is assumed to be a single sequence.
             - ``len(X)`` should be equal to ``sum(lengths)``.
 
-        :note: This method requires a trained classifier — see :func:`fit`.
-
-        :return: Class scores.
-        """
-        _, k_distances, k_labels = self.query_neighbors(X, lengths, sort=False)
+        Returns
+        -------
+        numpy.ndarray:
+            Class scores.
+
+        Notes
+        -----
+        This method requires a trained classifier — see :func:`fit`.
+        """
+        _, k_distances, k_labels = self.query_neighbors(
+            X,
+            lengths=lengths,
+            sort=False,
+        )
         k_weightings = self._weighting()(k_distances)
         return self._compute_scores(k_labels, k_weightings)
 
-
-    @_requires_fit
-    def score(
-        self,
-        X: Array,
-        y: Array[int],
-        lengths: Optional[Array[int]],
-        normalize: bool = True,
-        sample_weight: Optional[Array] = None,
-    ) -> float:
-        """Calculates accuracy for the sequence(s) in ``X``.
-
-        :param X: Univariate or multivariate observation sequence(s).
-
-            - Should be a single 1D or 2D array.
-            - Should have length as the 1st dimension and features as the 2nd dimension.
-            - Should be a concatenated sequence if multiple sequences are provided,
-              with respective sequence lengths being provided in the ``lengths`` argument for decoding the original sequences.
-
-        :param y: Classes corresponding to the observation sequence(s) in ``X``.
-
-        :param lengths: Lengths of the observation sequence(s) provided in ``X``.
-
-            - If ``None``, then ``X`` is assumed to be a single observation sequence.
-            - ``len(X)`` should be equal to ``sum(lengths)``.
-
-        :param normalize: See :func:`sklearn:sklearn.metrics.accuracy_score`.
-
-        :param sample_weight: See :func:`sklearn:sklearn.metrics.accuracy_score`.
-
-        :note: This method requires a trained classifier — see :func:`fit`.
-
-        :return: Classification accuracy.
-        """
-        return super().score(X, y, lengths, normalize, sample_weight)
-
-
-    @_validate_params(using=_KNNValidator)
-    @_override_params(_KNNValidator.fields(), temporary=False)
-    def set_params(self, **kwargs):
-        return self
-
-
     def _compute_scores(
-        self,
-        labels: Array[int],
-        weightings: Array[float]
-    ) -> Array[float]:
-        """Calculates the sum of the weightings for each label group.
-
-        TODO
-        """
+        self: KNNClassifier, labels: IntArray, weightings: FloatArray
+    ) -> FloatArray:
+        """Calculate the sum of the weightings for each label group."""
         scores = np.zeros((len(labels), len(self.classes_)))
         for i, k in enumerate(self.classes_):
-            scores[:, i] = np.einsum('ij,ij->i', labels == k, weightings)
+            scores[:, i] = np.einsum("ij,ij->i", labels == k, weightings)
         return scores
 
-
     def _find_max_labels(
-        self,
-        scores: Array[float]
-    ) -> Array[int]:
-        """Returns the label of the k nearest neighbors with the highest score for each example.
-
-        TODO
+        self: KNNClassifier,
+        scores: FloatArray,
+        /,
+    ) -> IntArray:
+        """Return the label of the k nearest neighbors with the highest score
+        for each example.
         """
-        n_jobs = _effective_n_jobs(self.n_jobs, scores)
+        n_jobs = _multiprocessing.effective_n_jobs(self.n_jobs, x=scores)
         score_chunks = np.array_split(scores, n_jobs)
         return np.concatenate(
-            Parallel(n_jobs=n_jobs, max_nbytes=None)(
-                delayed(self._find_max_labels_chunk)(score_chunk)
+            joblib.Parallel(n_jobs=n_jobs, max_nbytes=None)(
+                joblib.delayed(self._find_max_labels_chunk)(score_chunk)
                 for score_chunk in score_chunks
             )
         )
 
-
     def _find_max_labels_chunk(
-        self,
-        score_chunk: Array[float]
-    ) -> Array[int]:
-        """Returns the label with the highest score for each item in the chunk.
-
-        TODO
+        self: KNNClassifier, score_chunk: FloatArray, /
+    ) -> IntArray:
+        """Return the label with the highest score for each item in the
+        chunk.
         """
         max_labels = np.zeros(len(score_chunk), dtype=int)
         for i, scores in enumerate(score_chunk):
             max_score_idxs = self._multi_argmax(scores)
-            max_labels[i] = self.random_state_.choice(self.classes_[max_score_idxs], size=1)
+            max_labels[i] = self.random_state_.choice(
+                self.classes_[max_score_idxs], size=1
+            ).item()
         return max_labels
 
-
     @staticmethod
-    @njit
-    def _multi_argmax(
-        arr: Array
-    ) -> Array[int]:
-        """Same as numpy.argmax but returns all occurrences of the maximum and only requires a single pass.
-        From: https://stackoverflow.com/a/58652335
+    @numba.njit
+    def _multi_argmax(arr: Array, /) -> IntArray:
+        """Same as numpy.argmax but returns all occurrences of the maximum
+        and only requires a single pass.
 
-        TODO
+        From: https://stackoverflow.com/a/58652335
         """
         all_, max_ = [0], arr[0]
-        for i in prange(1, len(arr)):
+        for i in numba.prange(1, len(arr)):
             if arr[i] > max_:
                 all_, max_ = [i], arr[i]
             elif arr[i] == max_:
                 all_.append(i)
         return np.array(all_)
```

### Comparing `sequentia-1.1.1/lib/sequentia/preprocessing/transforms.py` & `sequentia-2.0.0/sequentia/preprocessing/transforms.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+# Copyright (c) 2019-2025 Sequentia Developers.
+# Distributed under the terms of the MIT License (see the LICENSE file).
+# SPDX-License-Identifier: MIT
+# This source code is part of the Sequentia project (https://github.com/eonu/sequentia).
+
 """
 IndependentFunctionTransformer is an adapted version of FunctionTransformer
 from the sklearn.preprocessing module, and largely relies on its source code.
 
 Below is the original license from Scikit-Learn, copied on 31st December 2022
 from https://github.com/scikit-learn/scikit-learn/blob/main/COPYING.
 
@@ -37,29 +42,28 @@
 OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 """
 
 from __future__ import annotations
 
 import warnings
-from typing import Callable, Optional, Dict, Any
 
 import numpy as np
-from pydantic import PositiveInt
+import scipy.signal
+import sklearn.base
+from sklearn.preprocessing import FunctionTransformer
 from sklearn.utils.validation import _allclose_dense_sparse, check_array
-from scipy.signal import medfilt2d, convolve
 
-from sequentia.preprocessing.base import Transform
-from sequentia.utils.validation import _BaseSequenceValidator, Array
-from sequentia.utils.data import SequentialDataset
+from sequentia._internal import _data, _validation
+from sequentia._internal._typing import Array, FloatArray, IntArray
 
 __all__ = ["IndependentFunctionTransformer", "mean_filter", "median_filter"]
 
 
-class IndependentFunctionTransformer(Transform):
+class IndependentFunctionTransformer(FunctionTransformer):
     """Constructs a transformer from an arbitrary callable,
     applying the transform independently to each sequence.
 
     This transform forwards its ``X`` and ``lengths`` arguments
     to a user-defined function or function object and returns the result of this
     function. This is useful for stateless transformations such as taking the
     log of frequencies, doing custom scaling, etc.
@@ -90,186 +94,256 @@
         # Fetch MFCCs of spoken digits
         data = load_digits()
 
         # Create an independent min-max transform
         transform = IndependentFunctionTransformer(minmax_scale)
 
         # Apply the transform to the data
-        Xt = transform.transform(data.X, data.lengths)
+        Xt = transform.transform(data.X, lengths=data.lengths)
     """
 
-
     def __init__(
         self,
-        func: Optional[Callable] = None,
-        inverse_func: Optional[Callable] = None,
+        func=None,
+        inverse_func=None,
         *,
-        validate: bool = False,
-        check_inverse: bool = True,
-        kw_args =None,
+        validate=False,
+        accept_sparse=False,
+        check_inverse=True,
+        feature_names_out=None,
+        kw_args=None,
         inv_kw_args=None,
-    ) -> IndependentFunctionTransformer:
-        """Initializes the :class:`.IndependentFunctionTransformer`.
-
-        :param func: The callable to use for the transformation.
-            This will be passed the same arguments as transform, with args and kwargs forwarded.
-            If ``None``, then ``func`` will be the identity function.
-
-        :param inverse_func: The callable to use for the inverse transformation.
-            This will be passed the same arguments as inverse transform, with args and kwargs forwarded.
-            If ``None``, then ``inverse_func`` will be the identity function.
-
-        :param validate: Indicates whether the input ``X`` array should be checked before calling ``func``.
-
-            - If ``False``, there is no input validation.
-            - If ``True``, then ``X`` will be converted to a 2-dimensional NumPy array.
-              If the conversion is not possible an exception is raised.
-
-        :param check_inverse: Whether to check that or ``func`` followed by ``inverse_func`` leads to the original inputs.
-            It can be used for a sanity check, raising a warning when the condition is not fulfilled.
-
-        :param kw_args: Dictionary of additional keyword arguments to pass to ``func``.
-
-        :param inv_kw_args: Dictionary of additional keyword arguments to pass to ``inverse_func``.
-        """
+    ):
+        """See :class:`sklearn:sklearn.preprocessing.FunctionTransformer`."""
         self.func = func
         self.inverse_func = inverse_func
         self.validate = validate
+        self.accept_sparse = accept_sparse
         self.check_inverse = check_inverse
-        self.kw_args: Optional[Dict[str, Any]] = kw_args
-        self.inv_kw_args: Optional[Dict[str, Any]] = inv_kw_args
+        self.feature_names_out = feature_names_out
+        self.kw_args = kw_args
+        self.inv_kw_args = inv_kw_args
+        # Allow metadata routing for lengths
+        self.set_fit_request(lengths=True)
+        self.set_transform_request(lengths=True)
+        self.set_inverse_transform_request(lengths=True)
 
-    def _check_input(self, X, lengths):
-        data = _BaseSequenceValidator(X=X, lengths=lengths)
-        return data.X, data.lengths
+    def _check_input(self, X, *, lengths, reset):
+        if self.validate:
+            X, lengths = _validation.check_X_lengths(
+                X, lengths=lengths, dtype=X.dtype
+            )
+            return (
+                self._validate_data(
+                    X, accept_sparse=self.accept_sparse, reset=reset
+                ),
+                lengths,
+            )
+        return X, lengths
 
-    def _check_inverse_transform(self, X, lengths):
+    def _check_inverse_transform(self, X, *, lengths):
         """Check that func and inverse_func are the inverse."""
         idx_selected = slice(None, None, max(1, X.shape[0] // 100))
-        X_round_trip = self.inverse_transform(self.transform(X[idx_selected], lengths), lengths)
+        X_round_trip = self.inverse_transform(
+            self.transform(X[idx_selected], lengths=lengths),
+            lengths=lengths,
+        )
+
+        if hasattr(X, "dtype"):
+            dtypes = [X.dtype]
+        elif hasattr(X, "dtypes"):
+            # Dataframes can have multiple dtypes
+            dtypes = X.dtypes
 
-        if not np.issubdtype(X.dtype, np.number):
+        if not all(np.issubdtype(d, np.number) for d in dtypes):
             raise ValueError(
-                "'check_inverse' is only supported when all the elements in `X` are numerical."
+                "'check_inverse' is only supported when all the elements in `X` is"
+                " numerical."
             )
 
         if not _allclose_dense_sparse(X[idx_selected], X_round_trip):
             warnings.warn(
-                "The provided functions are not strictly"
-                " inverse of each other. If you are sure you"
-                " want to proceed regardless, set"
-                " 'check_inverse=False'.",
+                (
+                    "The provided functions are not strictly"
+                    " inverse of each other. If you are sure you"
+                    " want to proceed regardless, set"
+                    " 'check_inverse=False'."
+                ),
                 UserWarning,
             )
 
+    @sklearn.base._fit_context(prefer_skip_nested_validation=True)
     def fit(
-        self,
+        self: IndependentFunctionTransformer,
         X: Array,
-        lengths: Optional[Array] = None
+        y: Array | None = None,
+        *,
+        lengths: IntArray | None = None,
     ) -> IndependentFunctionTransformer:
         """Fits the transformer to ``X``.
 
-        :param X: Univariate or multivariate observation sequence(s).
+        Parameters
+        ----------
+        self: IndependentFunctionTransformer
+
+        X:
+            Sequence(s).
 
-            - Should be a single 1D or 2D array.
-            - Should have length as the 1st dimension and features as the 2nd dimension.
-            - Should be a concatenated sequence if multiple sequences are provided,
-              with respective sequence lengths being provided in the ``lengths`` argument for decoding the original sequences.
+        y:
+            Outputs corresponding to sequence(s) in ``X``.
 
-        :param lengths: Lengths of the observation sequence(s) provided in ``X``.
+        lengths:
+            Lengths of the sequence(s) provided in ``X``.
 
-            - If ``None``, then ``X`` is assumed to be a single observation sequence.
+            - If ``None``, then ``X`` is assumed to be a single sequence.
             - ``len(X)`` should be equal to ``sum(lengths)``.
 
-        :return: The fitted transformer.
+        Returns
+        -------
+        IndependentFunctionTransformer
+            The fitted transformer.
         """
-        X, lengths = self._check_input(X, lengths)
-        if self.check_inverse and not (self.func is None or self.inverse_func is None):
-            self._check_inverse_transform(X, lengths)
+        X, lengths = self._check_input(X, lengths=lengths, reset=True)
+        if self.check_inverse and not (
+            self.func is None or self.inverse_func is None
+        ):
+            self._check_inverse_transform(X, lengths=lengths)
         return self
 
     def transform(
-        self,
+        self: IndependentFunctionTransformer,
         X: Array,
-        lengths: Optional[Array] = None
+        *,
+        lengths: IntArray | None = None,
     ) -> Array:
-        """Applies the transformation to ``X``, producing a transformed version of ``X``.
+        """Applies the transformation to ``X``,
+        producing a transformed version of ``X``.
 
-        :param X: Univariate or multivariate observation sequence(s).
+        Parameters
+        ----------
+        self: IndependentFunctionTransformer
 
-            - Should be a single 1D or 2D array.
-            - Should have length as the 1st dimension and features as the 2nd dimension.
-            - Should be a concatenated sequence if multiple sequences are provided,
-              with respective sequence lengths being provided in the ``lengths`` argument for decoding the original sequences.
+        X:
+            Sequence(s).
 
-        :param lengths: Lengths of the observation sequence(s) provided in ``X``.
+        lengths:
+            Lengths of the sequence(s) provided in ``X``.
 
-            - If ``None``, then ``X`` is assumed to be a single observation sequence.
+            - If ``None``, then ``X`` is assumed to be a single sequence.
             - ``len(X)`` should be equal to ``sum(lengths)``.
 
-        :return: The transformed array.
+        Returns
+        -------
+        numpy.ndarray:
+            The transformed array.
         """
-        X, lengths = self._check_input(X, lengths)
-        return self._transform(X, lengths, func=self.func, kw_args=self.kw_args)
+        X, lengths = self._check_input(X, lengths=lengths, reset=False)
+        return self._transform(
+            X, lengths=lengths, func=self.func, kw_args=self.kw_args
+        )
 
     def inverse_transform(
-        self,
+        self: IndependentFunctionTransformer,
         X: Array,
-        lengths: Optional[Array] = None
+        *,
+        lengths: IntArray | None = None,
     ) -> Array:
         """Applies the inverse transformation to ``X``.
 
-        :param X: Univariate or multivariate observation sequence(s).
+        Parameters
+        ----------
+        self: IndependentFunctionTransformer
 
-            - Should be a single 1D or 2D array.
-            - Should have length as the 1st dimension and features as the 2nd dimension.
-            - Should be a concatenated sequence if multiple sequences are provided,
-              with respective sequence lengths being provided in the ``lengths`` argument for decoding the original sequences.
+        X:
+            Sequence(s).
 
-        :param lengths: Lengths of the observation sequence(s) provided in ``X``.
+        lengths:
+            Lengths of the sequence(s) provided in ``X``.
 
-            - If ``None``, then ``X`` is assumed to be a single observation sequence.
+            - If ``None``, then ``X`` is assumed to be a single sequence.
             - ``len(X)`` should be equal to ``sum(lengths)``.
 
-        :return: The inverse transformed array.
+        Returns
+        -------
+        numpy.ndarray:
+            The inverse transformed array.
         """
-        X, lengths = self._check_input(X, lengths)
         if self.validate:
             X = check_array(X, accept_sparse=False)
-        return self._transform(X, lengths, func=self.inverse_func, kw_args=self.inv_kw_args)
+            X, lengths = _validation.check_X_lengths(
+                X, lengths=lengths, dtype=X.dtype
+            )
+        return self._transform(
+            X,
+            lengths=lengths,
+            func=self.inverse_func,
+            kw_args=self.inv_kw_args,
+        )
 
-    def _transform(self, X, lengths, func=None, kw_args=None):
-        if func is None:
-            return X
-        apply = lambda x: func(x, **(kw_args if kw_args else {}))
-        idxs = SequentialDataset._get_idxs(lengths)
-        return np.vstack([apply(x) for x in SequentialDataset._iter_X(X, idxs)])
+    def fit_transform(
+        self: IndependentFunctionTransformer,
+        X: Array,
+        y: Array | None = None,
+        *,
+        lengths: IntArray | None = None,
+    ) -> Array:
+        """Fits the transformer to the sequence(s) in ``X`` and returns a
+        transformed version of ``X``.
 
-    def __sklearn_is_fitted__(self):
-        """Return True since FunctionTransfomer is stateless."""
-        return True
+        Parameters
+        ----------
+        self: IndependentFunctionTransformer
 
-    def _more_tags(self):
-        return {"no_validation": not self.validate, "stateless": True}
+        X:
+            Sequence(s).
 
+        y:
+            Outputs corresponding to sequence(s) in ``X``.
 
-def mean_filter(x: Array, k: PositiveInt = 5) -> Array:
-    """Applies a mean filter of size ``k`` independently to each feature of the sequence,
-    retaining the original input shape by using appropriate padding.
+        lengths:
+            Lengths of the sequence(s) provided in ``X``.
 
-    This is implemented as a 1D convolution with a kernel of size ``k`` and values ``1 / k``.
+            - If ``None``, then ``X`` is assumed to be a single sequence.
+            - ``len(X)`` should be equal to ``sum(lengths)``.
 
-    :param x: Univariate or multivariate observation sequence.
+        Returns
+        -------
+        numpy.ndarray:
+            The transformed data.
+        """
+        return self.fit(X, lengths=lengths).transform(X, lengths=lengths)
 
-        - Should be a single 1D or 2D array.
-        - Should have length as the 1st dimension and features as the 2nd dimension.
+    def _transform(self, X, *, lengths, func=None, kw_args=None):
+        if func is None:
+            return X
+        apply = lambda x: func(x, **(kw_args if kw_args else {}))
+        idxs = _data.get_idxs(lengths)
+        return np.vstack([apply(x) for x in _data.iter_X(X, idxs=idxs)])
 
-    :param k: Width of the filter.
 
-    :return: The filtered array.
+def mean_filter(x: FloatArray, *, k: int = 5) -> FloatArray:
+    """Applies a mean filter of size ``k`` independently to each feature of
+    the sequence, retaining the original input shape by using appropriate
+    padding.
+
+    This is implemented as a 1D convolution with a kernel of size ``k`` and
+    values ``1 / k``.
+
+    Parameters
+    ----------
+    x:
+        Observation sequence.
+
+    k:
+        Width of the filter.
+
+    Returns
+    -------
+    numpy.ndarray:
+        The filtered array.
 
     Examples
     --------
     Applying a :func:`mean_filter` to a single sequence
     and multiple sequences (independently via :class:`IndependentFunctionTransformer`) from the spoken digits dataset. ::
 
         from sequentia.preprocessing import IndependentFunctionTransformer, mean_filter
@@ -282,32 +356,36 @@
         x, _ = data[0]
         xt = mean_filter(x, k=7)
 
         # Create an independent mean filter transform
         transform = IndependentFunctionTransformer(mean_filter, kw_args={"k": 7})
 
         # Apply the transform to all sequences
-        Xt = transform.transform(data.X, data.lengths)
+        Xt = transform.transform(data.X, lengths=data.lengths)
     """
-    data = _BaseSequenceValidator(X=x)
-    return convolve(data.X, np.ones((k, 1)) / k, mode="same")
-
-
-def median_filter(x: Array, k: PositiveInt = 5) -> Array:
-    """Applies a median filter of size ``k`` independently to each feature of the sequence,
-    retaining the original input shape by using appropriate padding.
-
-    :param x: Univariate or multivariate observation sequence.
-
-        - Should be a single 1D or 2D array.
-        - Should have length as the 1st dimension and features as the 2nd dimension.
+    return scipy.signal.convolve(x, np.ones((k, 1)) / k, mode="same")
 
-    :param k: Width of the filter.
 
-    :return: The filtered array.
+def median_filter(x: FloatArray, *, k: int = 5) -> FloatArray:
+    """Applies a median filter of size ``k`` independently to each feature of
+    the sequence, retaining the original input shape by using appropriate
+    padding.
+
+    Parameters
+    ----------
+    x:
+        Observation sequence.
+
+    k:
+        Width of the filter.
+
+    Returns
+    -------
+    numpy.ndarray:
+        The filtered array.
 
     Examples
     --------
     Applying a :func:`median_filter` to a single sequence
     and multiple sequences (independently via :class:`IndependentFunctionTransformer`) from the spoken digits dataset. ::
 
         from sequentia.preprocessing import IndependentFunctionTransformer, median_filter
@@ -320,11 +398,10 @@
         x, _ = data[0]
         xt = median_filter(x, k=7)
 
         # Create an independent median filter transform
         transform = IndependentFunctionTransformer(median_filter, kw_args={"k": 7})
 
         # Apply the transform to all sequences
-        Xt = transform.transform(data.X, data.lengths)
+        Xt = transform.transform(data.X, lengths=data.lengths)
     """
-    data = _BaseSequenceValidator(X=x)
-    return medfilt2d(data.X, kernel_size=(k, 1))
+    return scipy.signal.medfilt2d(x, kernel_size=(k, 1))
```

### Comparing `sequentia-1.1.1/lib/test/lib/models/hmm/test_topologies.py` & `sequentia-2.0.0/tests/unit/test_internal/test_hmm/test_topologies.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,351 +1,474 @@
-import pytest, warnings, numpy as np
-from sequentia.models.hmm.topologies import _Topology, _LeftRightTopology, _ErgodicTopology, _LinearTopology
-from ....support.assertions import assert_equal, assert_all_equal, assert_distribution
-
-# Set seed for reproducible randomness
-seed = 0
-np.random.seed(seed)
-rng = np.random.RandomState(seed)
-
-# ========= #
-# _Topology #
-# ========= #
-
-# ------------------------------- #
-# _Topology.uniform_start_probs() #
-# ------------------------------- #
+# Copyright (c) 2019-2025 Sequentia Developers.
+# Distributed under the terms of the MIT License (see the LICENSE file).
+# SPDX-License-Identifier: MIT
+# This source code is part of the Sequentia project (https://github.com/eonu/sequentia).
 
-def test_uniform_start_probs_min():
+import typing as t
+
+import numpy as np
+import pytest
+
+from sequentia._internal._hmm import topologies
+
+
+@pytest.fixture(scope="module")
+def random_state() -> np.random.RandomState:
+    return np.random.RandomState(0)
+
+
+def test_base_uniform_start_probs_min(
+    helpers: t.Any, random_state: np.random.RandomState
+) -> None:
     """Generate a uniform initial state distribution with the minimum number of states"""
-    topology = _Topology(n_states=1, random_state=rng)
+    topology = topologies.BaseTopology(n_states=1, random_state=random_state)
     start_probs = topology.uniform_start_probs()
-    assert_distribution(start_probs)
-    assert_equal(start_probs, np.array([
-        1.
-    ]))
+    helpers.assert_distribution(start_probs)
+    helpers.assert_equal(start_probs, np.array([1.0]))
+
 
-def test_uniform_start_probs_small():
+def test_base_uniform_start_probs_small(
+    helpers: t.Any, random_state: np.random.RandomState
+) -> None:
     """Generate a uniform initial state distribution with a few states"""
-    topology = _Topology(n_states=2, random_state=rng)
+    topology = topologies.BaseTopology(n_states=2, random_state=random_state)
     start_probs = topology.uniform_start_probs()
-    assert_distribution(start_probs)
-    assert_equal(start_probs, np.array([
-        0.5, 0.5
-    ]))
+    helpers.assert_distribution(start_probs)
+    helpers.assert_equal(start_probs, np.array([0.5, 0.5]))
 
-def test_uniform_start_probs_many():
+
+def test_base_uniform_start_probs_many(
+    helpers: t.Any, random_state: np.random.RandomState
+) -> None:
     """Generate a uniform initial state distribution with many states"""
-    topology = _Topology(n_states=5, random_state=rng)
+    topology = topologies.BaseTopology(n_states=5, random_state=random_state)
     start_probs = topology.uniform_start_probs()
-    assert_distribution(start_probs)
-    assert_equal(start_probs, np.array([
-        0.2, 0.2, 0.2, 0.2, 0.2
-    ]))
-
-# ------------------------------ #
-# _Topology.random_start_probs() #
-# ------------------------------ #
+    helpers.assert_distribution(start_probs)
+    helpers.assert_equal(start_probs, np.array([0.2, 0.2, 0.2, 0.2, 0.2]))
+
 
-def test_random_start_probs_min():
+def test_base_random_start_probs_min(
+    helpers: t.Any, random_state: np.random.RandomState
+) -> None:
     """Generate a random initial state distribution with minimal states"""
-    topology = _Topology(n_states=1, random_state=rng)
+    topology = topologies.BaseTopology(n_states=1, random_state=random_state)
     start_probs = topology.random_start_probs()
-    assert_distribution(start_probs)
-    assert_equal(start_probs, np.array([
-        1.
-    ]))
+    helpers.assert_distribution(start_probs)
+    helpers.assert_equal(start_probs, np.array([1.0]))
 
-def test_random_start_probs_small():
+
+def test_base_random_start_probs_small(
+    helpers: t.Any, random_state: np.random.RandomState
+) -> None:
     """Generate a random initial state distribution with few states"""
-    topology = _Topology(n_states=2, random_state=rng)
+    topology = topologies.BaseTopology(n_states=2, random_state=random_state)
     start_probs = topology.random_start_probs()
-    assert_distribution(start_probs)
-    assert_equal(start_probs, np.array([
-        0.57633871, 0.42366129
-    ]))
+    helpers.assert_distribution(start_probs)
+    helpers.assert_equal(start_probs, np.array([0.57633871, 0.42366129]))
+
 
-def test_random_initial_many():
+def test_base_random_initial_many(
+    helpers: t.Any, random_state: np.random.RandomState
+) -> None:
     """Generate a random initial state distribution with many states"""
-    topology = _Topology(n_states=5, random_state=rng)
+    topology = topologies.BaseTopology(n_states=5, random_state=random_state)
     start_probs = topology.random_start_probs()
-    assert_distribution(start_probs)
-    assert_equal(start_probs, np.array([
-        0.15210286, 0.10647349, 0.20059295, 0.11120171, 0.42962898
-    ]))
-
-# ================== #
-# _LeftRightTopology #
-# ================== #
-
-# ---------------------------------------- #
-# _LeftRightTopology.uniform_transitions() #
-# ---------------------------------------- #
+    helpers.assert_distribution(start_probs)
+    helpers.assert_equal(
+        start_probs,
+        np.array([0.15210286, 0.10647349, 0.20059295, 0.11120171, 0.42962898]),
+    )
+
 
-def test_left_right_uniform_transitions_min():
+def test_left_right_uniform_transitions_min(
+    helpers: t.Any, random_state: np.random.RandomState
+) -> None:
     """Generate a uniform left-right transition matrix with minimal states"""
-    topology = _LeftRightTopology(n_states=1, random_state=rng)
-    transitions = topology.uniform_transitions()
-    assert_distribution(transitions)
-    assert_equal(transitions, np.array([
-        [1.]
-    ]))
+    topology = topologies.LeftRightTopology(
+        n_states=1, random_state=random_state
+    )
+    transitions = topology.uniform_transition_probs()
+    helpers.assert_distribution(transitions)
+    helpers.assert_equal(transitions, np.array([[1.0]]))
 
-def test_left_right_uniform_transitions_small():
-    """Generate a uniform left-right transition matrix with few states"""
-    topology = _LeftRightTopology(n_states=2, random_state=rng)
-    transitions = topology.uniform_transitions()
-    assert_distribution(transitions)
-    assert_equal(transitions, np.array([
-        [0.5, 0.5],
-        [0. , 1. ]
-    ]))
 
-def test_left_right_uniform_transitions_many():
+def test_left_right_uniform_transitions_small(
+    helpers: t.Any, random_state: np.random.RandomState
+) -> None:
+    """Generate a uniform left-right transition matrix with few states"""
+    topology = topologies.LeftRightTopology(
+        n_states=2, random_state=random_state
+    )
+    transitions = topology.uniform_transition_probs()
+    helpers.assert_distribution(transitions)
+    helpers.assert_equal(
+        transitions,
+        np.array(
+            [
+                [0.5, 0.5],
+                [0.0, 1.0],
+            ]
+        ),
+    )
+
+
+def test_left_right_uniform_transitions_many(
+    helpers: t.Any, random_state: np.random.RandomState
+) -> None:
     """Generate a uniform left-right transition matrix with many states"""
-    topology = _LeftRightTopology(n_states=5, random_state=rng)
-    transitions = topology.uniform_transitions()
-    assert_distribution(transitions)
-    assert_equal(transitions, np.array([
-        [0.2, 0.2 , 0.2       , 0.2       , 0.2       ],
-        [0. , 0.25, 0.25      , 0.25      , 0.25      ],
-        [0. , 0.  , 0.33333333, 0.33333333, 0.33333333],
-        [0. , 0.  , 0.        , 0.5       , 0.5       ] ,
-        [0. , 0.  , 0.        , 0.        , 1.        ]
-    ]))
-
-# --------------------------------------- #
-# _LeftRightTopology.random_transitions() #
-# --------------------------------------- #
-
-def test_left_right_random_transitions_min():
+    topology = topologies.LeftRightTopology(
+        n_states=5, random_state=random_state
+    )
+    transitions = topology.uniform_transition_probs()
+    helpers.assert_distribution(transitions)
+    helpers.assert_equal(
+        transitions,
+        np.array(
+            [
+                [0.2, 0.2, 0.2, 0.2, 0.2],
+                [0.0, 0.25, 0.25, 0.25, 0.25],
+                [0.0, 0.0, 0.33333333, 0.33333333, 0.33333333],
+                [0.0, 0.0, 0.0, 0.5, 0.5],
+                [0.0, 0.0, 0.0, 0.0, 1.0],
+            ]
+        ),
+    )
+
+
+def test_left_right_random_transitions_min(
+    helpers: t.Any, random_state: np.random.RandomState
+) -> None:
     """Generate a random left-right transition matrix with minimal states"""
-    topology = _LeftRightTopology(n_states=1, random_state=rng)
-    transitions = topology.random_transitions()
-    assert_distribution(transitions)
-    assert_equal(transitions, np.array([
-        [1.]
-    ]))
+    topology = topologies.LeftRightTopology(
+        n_states=1, random_state=random_state
+    )
+    transitions = topology.random_transition_probs()
+    helpers.assert_distribution(transitions)
+    helpers.assert_equal(transitions, np.array([[1.0]]))
 
-def test_left_right_random_transitions_small():
-    """Generate a random left-right transition matrix with few states"""
-    topology = _LeftRightTopology(n_states=2, random_state=rng)
-    transitions = topology.random_transitions()
-    assert_distribution(transitions)
-    assert_equal(transitions, np.array([
-        [0.23561633, 0.76438367],
-        [0.        , 1.        ]
-    ]))
 
-def test_left_right_random_transitions_many():
+def test_left_right_random_transitions_small(
+    helpers: t.Any, random_state: np.random.RandomState
+) -> None:
+    """Generate a random left-right transition matrix with few states"""
+    topology = topologies.LeftRightTopology(
+        n_states=2, random_state=random_state
+    )
+    transitions = topology.random_transition_probs()
+    helpers.assert_distribution(transitions)
+    helpers.assert_equal(
+        transitions,
+        np.array(
+            [
+                [0.23561633, 0.76438367],
+                [0.0, 1.0],
+            ]
+        ),
+    )
+
+
+def test_left_right_random_transitions_many(
+    helpers: t.Any, random_state: np.random.RandomState
+) -> None:
     """Generate a random left-right transition matrix with many states"""
-    topology = _LeftRightTopology(n_states=5, random_state=rng)
-    transitions = topology.random_transitions()
-    assert_distribution(transitions)
-    assert_equal(transitions, np.array([
-        [0.23169814, 0.71716356, 0.02033845, 0.02516204, 0.00563782],
-        [0.        , 0.19474072, 0.16405008, 0.22228532, 0.41892388],
-        [0.        , 0.        , 0.42912755, 0.16545797, 0.40541448],
-        [0.        , 0.        , 0.        , 0.109713  , 0.890287  ],
-        [0.        , 0.        , 0.        , 0.        , 1.        ]
-    ]))
-
-# ---------------------------------------#
-# _LeftRightTopology.check_transitions() #
-# ---------------------------------------#
-
-def test_left_right_check_transitions_invalid():
+    topology = topologies.LeftRightTopology(
+        n_states=5, random_state=random_state
+    )
+    transitions = topology.random_transition_probs()
+    helpers.assert_distribution(transitions)
+    helpers.assert_equal(
+        transitions,
+        np.array(
+            [
+                [0.23169814, 0.71716356, 0.02033845, 0.02516204, 0.00563782],
+                [0.0, 0.19474072, 0.16405008, 0.22228532, 0.41892388],
+                [0.0, 0.0, 0.42912755, 0.16545797, 0.40541448],
+                [0.0, 0.0, 0.0, 0.109713, 0.890287],
+                [0.0, 0.0, 0.0, 0.0, 1.0],
+            ]
+        ),
+    )
+
+
+def test_left_right_check_transitions_invalid(
+    random_state: np.random.RandomState,
+) -> None:
     """Validate an invalid left-right transition matrix"""
-    topology = _LeftRightTopology(n_states=5, random_state=rng)
-    transitions = _ErgodicTopology(n_states=5, random_state=rng).random_transitions()
-    with pytest.raises(ValueError) as e:
-        topology.check_transitions(transitions)
-    assert str(e.value) == 'Left-right transition matrix must be upper-triangular'
-
-def test_left_right_check_transitions_valid():
+    topology = topologies.LeftRightTopology(
+        n_states=5, random_state=random_state
+    )
+    transitions = topologies.ErgodicTopology(
+        n_states=5, random_state=random_state
+    ).random_transition_probs()
+    with pytest.raises(ValueError) as e:  # noqa: PT011
+        topology.check_transition_probs(transitions)
+    assert (
+        str(e.value) == "Left-right transition matrix must be upper-triangular"
+    )
+
+
+def test_left_right_check_transitions_valid(
+    random_state: np.random.RandomState,
+) -> None:
     """Validate a valid left-right transition matrix"""
-    topology = _LeftRightTopology(n_states=5, random_state=rng)
-    transitions = topology.random_transitions()
-    topology.check_transitions(transitions)
-
-# -------------------------------------- #
-# _ErgodicTopology.uniform_transitions() #
-# -------------------------------------- #
+    topology = topologies.LeftRightTopology(
+        n_states=5, random_state=random_state
+    )
+    transitions = topology.random_transition_probs()
+    topology.check_transition_probs(transitions)
+
 
-def test_ergodic_uniform_transitions_min():
+def test_ergodic_uniform_transitions_min(
+    helpers: t.Any, random_state: np.random.RandomState
+) -> None:
     """Generate a uniform ergodic transition matrix with minimal states"""
-    topology = _ErgodicTopology(n_states=1, random_state=rng)
-    transitions = topology.uniform_transitions()
-    assert_distribution(transitions)
-    assert_equal(transitions, np.array([
-        [1.]
-    ]))
+    topology = topologies.ErgodicTopology(
+        n_states=1, random_state=random_state
+    )
+    transitions = topology.uniform_transition_probs()
+    helpers.assert_distribution(transitions)
+    helpers.assert_equal(transitions, np.array([[1.0]]))
 
-def test_ergodic_uniform_transitions_small():
-    """Generate a uniform ergodic transition matrix with few states"""
-    topology = _ErgodicTopology(n_states=2, random_state=rng)
-    transitions = topology.uniform_transitions()
-    assert_distribution(transitions)
-    assert_equal(transitions, np.array([
-        [0.5, 0.5],
-        [0.5, 0.5]
-    ]))
 
-def test_ergodic_uniform_transitions_many():
+def test_ergodic_uniform_transitions_small(
+    helpers: t.Any, random_state: np.random.RandomState
+) -> None:
+    """Generate a uniform ergodic transition matrix with few states"""
+    topology = topologies.ErgodicTopology(
+        n_states=2, random_state=random_state
+    )
+    transitions = topology.uniform_transition_probs()
+    helpers.assert_distribution(transitions)
+    helpers.assert_equal(
+        transitions,
+        np.array(
+            [
+                [0.5, 0.5],
+                [0.5, 0.5],
+            ]
+        ),
+    )
+
+
+def test_ergodic_uniform_transitions_many(
+    helpers: t.Any, random_state: np.random.RandomState
+) -> None:
     """Generate a uniform ergodic transition matrix with many states"""
-    topology = _ErgodicTopology(n_states=5, random_state=rng)
-    transitions = topology.uniform_transitions()
-    assert_distribution(transitions)
-    assert_equal(transitions, np.array([
-        [0.2, 0.2, 0.2, 0.2, 0.2],
-        [0.2, 0.2, 0.2, 0.2, 0.2],
-        [0.2, 0.2, 0.2, 0.2, 0.2],
-        [0.2, 0.2, 0.2, 0.2, 0.2],
-        [0.2, 0.2, 0.2, 0.2, 0.2]
-    ]))
-
-# ------------------------------------- #
-# _ErgodicTopology.random_transitions() #
-# ------------------------------------- #
-
-def test_ergodic_random_transitions_min():
+    topology = topologies.ErgodicTopology(
+        n_states=5, random_state=random_state
+    )
+    transitions = topology.uniform_transition_probs()
+    helpers.assert_distribution(transitions)
+    helpers.assert_equal(
+        transitions,
+        np.array(
+            [
+                [0.2, 0.2, 0.2, 0.2, 0.2],
+                [0.2, 0.2, 0.2, 0.2, 0.2],
+                [0.2, 0.2, 0.2, 0.2, 0.2],
+                [0.2, 0.2, 0.2, 0.2, 0.2],
+                [0.2, 0.2, 0.2, 0.2, 0.2],
+            ]
+        ),
+    )
+
+
+def test_ergodic_random_transitions_min(
+    helpers: t.Any, random_state: np.random.RandomState
+) -> None:
     """Generate a random ergodic transition matrix with minimal states"""
-    topology = _ErgodicTopology(n_states=1, random_state=rng)
-    transitions = topology.random_transitions()
-    assert_distribution(transitions)
-    assert_equal(transitions, np.array([
-        [1.]
-    ]))
+    topology = topologies.ErgodicTopology(
+        n_states=1, random_state=random_state
+    )
+    transitions = topology.random_transition_probs()
+    helpers.assert_distribution(transitions)
+    helpers.assert_equal(transitions, np.array([[1.0]]))
 
-def test_ergodic_random_transitions_small():
-    """Generate a random ergodic transition matrix with few states"""
-    topology = _ErgodicTopology(n_states=2, random_state=rng)
-    transitions = topology.random_transitions()
-    assert_distribution(transitions)
-    assert_equal(transitions, np.array([
-        [0.9474011 , 0.0525989 ],
-        [0.85567599, 0.14432401]
-    ]))
 
-def test_ergodic_random_transitions_many():
+def test_ergodic_random_transitions_small(
+    helpers: t.Any, random_state: np.random.RandomState
+) -> None:
+    """Generate a random ergodic transition matrix with few states"""
+    topology = topologies.ErgodicTopology(
+        n_states=2, random_state=random_state
+    )
+    transitions = topology.random_transition_probs()
+    helpers.assert_distribution(transitions)
+    helpers.assert_equal(
+        transitions,
+        np.array(
+            [
+                [0.9474011, 0.0525989],
+                [0.85567599, 0.14432401],
+            ]
+        ),
+    )
+
+
+def test_ergodic_random_transitions_many(
+    helpers: t.Any, random_state: np.random.RandomState
+) -> None:
     """Generate a random ergodic transition matrix with many states"""
-    topology = _ErgodicTopology(n_states=5, random_state=rng)
-    transitions = topology.random_transitions()
-    assert_distribution(transitions)
-    assert_equal(transitions, np.array([
-        [0.58715548, 0.14491542, 0.20980762, 0.00623944, 0.05188205],
-        [0.0840705 , 0.23055049, 0.08297536, 0.25124688, 0.35115677],
-        [0.02117615, 0.37664662, 0.26705912, 0.09851123, 0.23660688],
-        [0.01938041, 0.16853843, 0.52046123, 0.07535256, 0.21626737],
-        [0.04996846, 0.44545843, 0.12079423, 0.07154241, 0.31223646]
-    ]))
-
-# ------------------------------------ #
-# _ErgodicTopology.check_transitions() #
-# ------------------------------------ #
-
-def test_ergodic_check_transitions_invalid():
+    topology = topologies.ErgodicTopology(
+        n_states=5, random_state=random_state
+    )
+    transitions = topology.random_transition_probs()
+    helpers.assert_distribution(transitions)
+    helpers.assert_equal(
+        transitions,
+        np.array(
+            [
+                [0.58715548, 0.14491542, 0.20980762, 0.00623944, 0.05188205],
+                [0.0840705, 0.23055049, 0.08297536, 0.25124688, 0.35115677],
+                [0.02117615, 0.37664662, 0.26705912, 0.09851123, 0.23660688],
+                [0.01938041, 0.16853843, 0.52046123, 0.07535256, 0.21626737],
+                [0.04996846, 0.44545843, 0.12079423, 0.07154241, 0.31223646],
+            ]
+        ),
+    )
+
+
+def test_ergodic_check_transitions_invalid(
+    random_state: np.random.RandomState
+) -> None:
     """Validate an invalid ergodic transition matrix"""
-    topology = _ErgodicTopology(n_states=5, random_state=rng)
-    transitions = _LeftRightTopology(n_states=5, random_state=rng).random_transitions()
+    topology = topologies.ErgodicTopology(
+        n_states=5, random_state=random_state
+    )
+    transitions = topologies.LeftRightTopology(
+        n_states=5, random_state=random_state
+    ).random_transition_probs()
     with pytest.warns(UserWarning):
-        topology.check_transitions(transitions)
+        topology.check_transition_probs(transitions)
+
 
-def test_ergodic_check_transitions_valid():
+def test_ergodic_check_transitions_valid(
+    random_state: np.random.RandomState
+) -> None:
     """Validate a valid ergodic transition matrix"""
-    topology = _ErgodicTopology(n_states=5, random_state=rng)
-    transitions = topology.random_transitions()
-    topology.check_transitions(transitions)
-
-# =============== #
-# _LinearTopology #
-# =============== #
-
-# ------------------------------------- #
-# _LinearTopology.uniform_transitions() #
-# ------------------------------------- #
+    topology = topologies.ErgodicTopology(
+        n_states=5, random_state=random_state
+    )
+    transitions = topology.random_transition_probs()
+    topology.check_transition_probs(transitions)
 
-def test_linear_uniform_transitions_min():
+
+def test_linear_uniform_transitions_min(
+    helpers: t.Any, random_state: np.random.RandomState
+) -> None:
     """Generate a uniform linear transition matrix with minimal states"""
-    topology = _LinearTopology(n_states=1, random_state=rng)
-    transitions = topology.uniform_transitions()
-    assert_distribution(transitions)
-    assert_equal(transitions, np.array([
-        [1.]
-    ]))
+    topology = topologies.LinearTopology(n_states=1, random_state=random_state)
+    transitions = topology.uniform_transition_probs()
+    helpers.assert_distribution(transitions)
+    helpers.assert_equal(transitions, np.array([[1.0]]))
 
-def test_linear_uniform_transitions_small():
-    """Generate a uniform linear transition matrix with few states"""
-    topology = _LinearTopology(n_states=2, random_state=rng)
-    transitions = topology.uniform_transitions()
-    assert_distribution(transitions)
-    assert_equal(transitions, np.array([
-        [0.5, 0.5],
-        [0. , 1. ]
-    ]))
 
-def test_linear_uniform_transitions_many():
+def test_linear_uniform_transitions_small(
+    helpers: t.Any, random_state: np.random.RandomState
+) -> None:
+    """Generate a uniform linear transition matrix with few states"""
+    topology = topologies.LinearTopology(n_states=2, random_state=random_state)
+    transitions = topology.uniform_transition_probs()
+    helpers.assert_distribution(transitions)
+    helpers.assert_equal(
+        transitions,
+        np.array(
+            [
+                [0.5, 0.5],
+                [0.0, 1.0],
+            ]
+        ),
+    )
+
+
+def test_linear_uniform_transitions_many(
+    helpers: t.Any, random_state: np.random.RandomState
+) -> None:
     """Generate a uniform linear transition matrix with many states"""
-    topology = _LinearTopology(n_states=5, random_state=rng)
-    transitions = topology.uniform_transitions()
-    assert_distribution(transitions)
-    assert_equal(transitions, np.array([
-        [0.5, 0.5, 0. , 0. , 0. ],
-        [0. , 0.5, 0.5, 0. , 0. ],
-        [0. , 0. , 0.5, 0.5, 0. ],
-        [0. , 0. , 0. , 0.5, 0.5],
-        [0. , 0. , 0. , 0. , 1. ]
-    ]))
-
-# ------------------------------------ #
-# _LinearTopology.random_transitions() #
-# ------------------------------------ #
-
-def test_linear_random_transitions_min():
+    topology = topologies.LinearTopology(n_states=5, random_state=random_state)
+    transitions = topology.uniform_transition_probs()
+    helpers.assert_distribution(transitions)
+    helpers.assert_equal(
+        transitions,
+        np.array(
+            [
+                [0.5, 0.5, 0.0, 0.0, 0.0],
+                [0.0, 0.5, 0.5, 0.0, 0.0],
+                [0.0, 0.0, 0.5, 0.5, 0.0],
+                [0.0, 0.0, 0.0, 0.5, 0.5],
+                [0.0, 0.0, 0.0, 0.0, 1.0],
+            ]
+        ),
+    )
+
+
+def test_linear_random_transitions_min(
+    helpers: t.Any, random_state: np.random.RandomState
+) -> None:
     """Generate a random linear transition matrix with minimal states"""
-    topology = _LinearTopology(n_states=1, random_state=rng)
-    transitions = topology.random_transitions()
-    assert_distribution(transitions)
-    assert_equal(transitions, np.array([
-        [1.]
-    ]))
+    topology = topologies.LinearTopology(n_states=1, random_state=random_state)
+    transitions = topology.random_transition_probs()
+    helpers.assert_distribution(transitions)
+    helpers.assert_equal(transitions, np.array([[1.0]]))
 
-def test_linear_random_transitions_small():
-    """Generate a random linear transition matrix with few states"""
-    topology = _LinearTopology(n_states=2, random_state=rng)
-    transitions = topology.random_transitions()
-    assert_distribution(transitions)
-    assert_equal(transitions, np.array([
-        [0.65157396, 0.34842604],
-        [0.        , 1.        ]
-    ]))
 
-def test_linear_random_transitions_many():
+def test_linear_random_transitions_small(
+    helpers: t.Any, random_state: np.random.RandomState
+) -> None:
+    """Generate a random linear transition matrix with few states"""
+    topology = topologies.LinearTopology(n_states=2, random_state=random_state)
+    transitions = topology.random_transition_probs()
+    helpers.assert_distribution(transitions)
+    helpers.assert_equal(
+        transitions,
+        np.array(
+            [
+                [0.65157396, 0.34842604],
+                [0.0, 1.0],
+            ]
+        ),
+    )
+
+
+def test_linear_random_transitions_many(
+    helpers: t.Any, random_state: np.random.RandomState
+) -> None:
     """Generate a random linear transition matrix with many states"""
-    topology = _LinearTopology(n_states=5, random_state=rng)
-    transitions = topology.random_transitions()
-    assert_distribution(transitions)
-    assert_equal(transitions, np.array([
-        [0.44455421, 0.55544579, 0.        , 0.        , 0.        ],
-        [0.        , 0.57553614, 0.42446386, 0.        , 0.        ],
-        [0.        , 0.        , 0.92014965, 0.07985035, 0.        ],
-        [0.        , 0.        , 0.        , 0.66790982, 0.33209018],
-        [0.        , 0.        , 0.        , 0.        , 1.        ]
-    ]))
-
-# ----------------------------------- #
-# _LinearTopology.check_transitions() #
-# ----------------------------------- #
-
-def test_linear_check_transitions_invalid():
+    topology = topologies.LinearTopology(n_states=5, random_state=random_state)
+    transitions = topology.random_transition_probs()
+    helpers.assert_distribution(transitions)
+    helpers.assert_equal(
+        transitions,
+        np.array(
+            [
+                [0.44455421, 0.55544579, 0.0, 0.0, 0.0],
+                [0.0, 0.57553614, 0.42446386, 0.0, 0.0],
+                [0.0, 0.0, 0.92014965, 0.07985035, 0.0],
+                [0.0, 0.0, 0.0, 0.66790982, 0.33209018],
+                [0.0, 0.0, 0.0, 0.0, 1.0],
+            ]
+        ),
+    )
+
+
+def test_linear_check_transitions_invalid(
+    random_state: np.random.RandomState
+) -> None:
     """Validate an invalid linear transition matrix"""
-    topology = _LinearTopology(n_states=5, random_state=rng)
-    transitions = _ErgodicTopology(n_states=5, random_state=rng).random_transitions()
-    with pytest.raises(ValueError) as e:
-        topology.check_transitions(transitions)
-    assert str(e.value) == 'Left-right transition matrix must be upper-triangular'
+    topology = topologies.LinearTopology(n_states=5, random_state=random_state)
+    transitions = topologies.ErgodicTopology(
+        n_states=5, random_state=random_state
+    ).random_transition_probs()
+    with pytest.raises(ValueError) as e:  # noqa: PT011
+        topology.check_transition_probs(transitions)
+    assert (
+        str(e.value) == "Left-right transition matrix must be upper-triangular"
+    )
+
 
-def test_linear_check_transitions_valid():
+def test_linear_check_transitions_valid(
+    random_state: np.random.RandomState
+) -> None:
     """Validate a valid linear transition matrix"""
-    topology = _LinearTopology(n_states=5, random_state=rng)
-    transitions = topology.random_transitions()
-    topology.check_transitions(transitions)
+    topology = topologies.LinearTopology(n_states=5, random_state=random_state)
+    transitions = topology.random_transition_probs()
+    topology.check_transition_probs(transitions)
```

### Comparing `sequentia-1.1.1/lib/test/lib/models/hmm/variants/test_categorical.py` & `sequentia-2.0.0/tests/unit/test_models/hmm/variants/test_categorical.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,146 +1,234 @@
-import pytest
+# Copyright (c) 2019-2025 Sequentia Developers.
+# Distributed under the terms of the MIT License (see the LICENSE file).
+# SPDX-License-Identifier: MIT
+# This source code is part of the Sequentia project (https://github.com/eonu/sequentia).
+
+from __future__ import annotations
+
+import typing as t
 
 import hmmlearn
 import numpy as np
+import pytest
+from _pytest.fixtures import SubRequest
 
+from sequentia import enums
+from sequentia._internal import _validation
+from sequentia._internal._hmm.topologies import TOPOLOGY_MAP, BaseTopology
+from sequentia.datasets import SequentialDataset, load_gene_families
 from sequentia.models import CategoricalHMM
-from sequentia.models.hmm.topologies import _topologies
-from sequentia.datasets import load_gene_families
 
-from .....support.assertions import assert_equal, assert_not_equal
-from .....support.itertools import combinations
+from .....conftest import Helpers
 
 
-@pytest.fixture(scope='module')
-def random_state():
+@pytest.fixture(scope="module")
+def random_state() -> np.random.RandomState:
     return np.random.RandomState(0)
 
 
-@pytest.fixture(scope='module')
-def data(random_state):
+@pytest.fixture(scope="module")
+def data(random_state: np.random.RandomState) -> SequentialDataset:
     data_, _ = load_gene_families(families=[0])
-    _, subset = data_.split(test_size=0.2, random_state=random_state, stratify=True)
+    _, subset = data_.split(
+        test_size=0.2, random_state=random_state, stratify=True
+    )
     return subset
 
 
-@pytest.fixture(scope='module')
-def topology(request):
-    return _topologies[request.param]
+@pytest.fixture(scope="module")
+def topology(request: SubRequest) -> BaseTopology:
+    return TOPOLOGY_MAP[request.param]
 
 
-def assert_fit(hmm, data):
+def assert_fit(hmm: CategoricalHMM, /, *, data: SequentialDataset) -> None:
     assert hmm.n_seqs_ == len(data.lengths)
     assert (hmm.topology_ is not None) == (hmm.topology is not None)
     assert isinstance(hmm.model, hmmlearn.hmm.CategoricalHMM)
     assert len(hmm.model.monitor_.history) > 0
+    assert _validation.check_is_fitted(hmm, return_=True)
 
 
-def test_categorical_fit_n_states(data, random_state):
+def test_categorical_fit_n_states(
+    data: SequentialDataset, random_state: np.random.RandomState
+) -> None:
     hmm = CategoricalHMM(n_states=7, random_state=random_state)
 
-    assert_fit(hmm.fit(*data.X_lengths), data)
+    assert_fit(hmm.fit(**data.X_lengths), data=data)
 
     assert hmm.n_states == 7
 
     assert hmm.model.startprob_.shape == (hmm.n_states,)
     assert hmm.model.transmat_.shape == (hmm.n_states, hmm.n_states)
 
 
-def test_categorical_fit_no_topology(data, random_state):
+def test_categorical_fit_no_topology(
+    data: SequentialDataset, random_state: np.random.RandomState
+) -> None:
     hmm = CategoricalHMM(topology=None, random_state=random_state)
 
-    assert_fit(hmm.fit(*data.X_lengths), data)
+    assert_fit(hmm.fit(**data.X_lengths), data=data)
 
     assert hmm.topology is None
     assert hmm.topology_ is None
 
-    assert set(hmm.model.init_params) == set('ste')
-    assert set(hmm.model.params) == set('ste')
+    assert set(hmm.model.init_params) == set("ste")
+    assert set(hmm.model.params) == set("ste")
 
-    assert not hasattr(hmm, '_startprob')
-    assert not hasattr(hmm, '_transmat')
+    assert not hasattr(hmm, "_startprob")
+    assert not hasattr(hmm, "_transmat")
 
 
-@pytest.mark.parametrize('topology', ['ergodic', 'left-right', 'linear'], indirect=True)
-@pytest.mark.parametrize('start_probs_type', ['uniform', 'random', None]) # None = custom
-def test_categorical_fit_set_start_probs(data, random_state, topology, start_probs_type):
-    hmm = CategoricalHMM(topology=topology.name, random_state=random_state)
-    hmm.set_start_probs(start_probs_type or topology(hmm.n_states, random_state).random_start_probs())
+@pytest.mark.parametrize("topology", list(enums.TopologyMode), indirect=True)
+@pytest.mark.parametrize(
+    "start_probs_mode", [*list(enums.TransitionMode), None]
+)
+def test_categorical_fit_set_state_start_probs(
+    helpers: t.Any,
+    data: SequentialDataset,
+    random_state: np.random.RandomState,
+    topology: BaseTopology,
+    start_probs_mode: enums.TransitionMode | None,
+) -> None:
+    hmm = CategoricalHMM(topology=topology.mode, random_state=random_state)
+    hmm.set_state_start_probs(
+        start_probs_mode
+        or topology(
+            n_states=hmm.n_states, random_state=random_state
+        ).random_start_probs()
+    )
+
+    assert hmm.topology == topology.mode
+    if start_probs_mode is not None:
+        assert hmm._startprob == start_probs_mode
 
-    assert hmm.topology == topology.name
-    if start_probs_type is not None:
-        assert hmm._startprob == start_probs_type
-
-    assert_fit(hmm.fit(*data.X_lengths), data)
+    assert_fit(hmm.fit(**data.X_lengths), data=data)
 
     assert isinstance(hmm.topology_, topology)
 
-    assert set(hmm.model.init_params) == set('e')
-    assert set(hmm.model.params) == set('ste')
+    assert set(hmm.model.init_params) == set("e")
+    assert set(hmm.model.params) == set("ste")
 
-    hmm.topology_.check_start_probs(hmm._startprob) # transition matrix before fit
-    hmm.topology_.check_start_probs(hmm.model.startprob_) # transition matrix after fit
+    hmm.topology_.check_start_probs(
+        hmm._startprob
+    )  # transition matrix before fit
+    hmm.topology_.check_start_probs(
+        hmm.model.startprob_
+    )  # transition matrix after fit
 
-    if start_probs_type == 'uniform':
+    if start_probs_mode == enums.TransitionMode.UNIFORM:
         init_startprob = hmm.topology_.uniform_start_probs()
-        assert_equal(hmm._startprob, init_startprob) # initial state probabilities should be uniform
-
-    assert_not_equal(hmm._startprob, hmm.model.startprob_) # should update probabilities
-    assert_equal(hmm._startprob == 0, hmm.model.startprob_ == 0) # but locations of zeros (if any) shouldn't change
-
+        helpers.assert_equal(
+            hmm._startprob, init_startprob
+        )  # initial state probabilities should be uniform
+
+    helpers.assert_not_equal(
+        hmm._startprob, hmm.model.startprob_
+    )  # should update probabilities
+    helpers.assert_equal(
+        hmm._startprob == 0, hmm.model.startprob_ == 0
+    )  # but locations of zeros (if any) shouldn't change
+
+
+@pytest.mark.parametrize("topology", list(enums.TopologyMode), indirect=True)
+@pytest.mark.parametrize(
+    "transition_mode", [*list(enums.TransitionMode), None]
+)  # None = custom
+def test_categorical_fit_set_state_transition_probs(
+    helpers: t.Any,
+    data: SequentialDataset,
+    random_state: np.random.RandomState,
+    topology: BaseTopology,
+    transition_mode: enums.TransitionMode | None,
+) -> None:
+    hmm = CategoricalHMM(topology=topology.mode, random_state=random_state)
+    hmm.set_state_transition_probs(
+        transition_mode
+        or topology(
+            n_states=hmm.n_states, random_state=random_state
+        ).random_transition_probs()
+    )
+
+    assert hmm.topology == topology.mode
+    if transition_mode is not None:
+        assert hmm._transmat == transition_mode
 
-@pytest.mark.parametrize('topology', ['ergodic', 'left-right', 'linear'], indirect=True)
-@pytest.mark.parametrize('transition_type', ['uniform', 'random', None]) # None = custom
-def test_categorical_fit_set_transitions(data, random_state, topology, transition_type):
-    hmm = CategoricalHMM(topology=topology.name, random_state=random_state)
-    hmm.set_transitions(transition_type or topology(hmm.n_states, random_state).random_transitions())
-
-    assert hmm.topology == topology.name
-    if transition_type is not None:
-        assert hmm._transmat == transition_type
-
-    assert_fit(hmm.fit(*data.X_lengths), data)
+    assert_fit(hmm.fit(**data.X_lengths), data=data)
 
     assert isinstance(hmm.topology_, topology)
 
-    assert set(hmm.model.init_params) == set('e')
-    assert set(hmm.model.params) == set('ste')
-
-    hmm.topology_.check_transitions(hmm._transmat) # transition matrix before fit
-    hmm.topology_.check_transitions(hmm.model.transmat_) # transition matrix after fit
-
-    if transition_type == 'uniform':
-        init_transmat = hmm.topology_.uniform_transitions()
-        assert_equal(hmm._transmat, init_transmat) # transition probabilities should be uniform
-
-    assert_not_equal(hmm._transmat, hmm.model.transmat_) # should update probabilities
-    assert_equal(hmm._transmat == 0, hmm.model.transmat_ == 0) # but locations of zeros (if any) shouldn't change
-
+    assert set(hmm.model.init_params) == set("e")
+    assert set(hmm.model.params) == set("ste")
 
-@pytest.mark.parametrize('freeze_params', combinations('ste'))
-def test_categorical_fit_freeze_unfreeze(data, random_state, freeze_params):
-    hmm = CategoricalHMM(topology='linear', n_states=2, random_state=random_state)
+    hmm.topology_.check_transition_probs(
+        hmm._transmat
+    )  # transition matrix before fit
+    hmm.topology_.check_transition_probs(
+        hmm.model.transmat_
+    )  # transition matrix after fit
+
+    if transition_mode == enums.TransitionMode.UNIFORM:
+        init_transmat = hmm.topology_.uniform_transition_probs()
+        helpers.assert_equal(
+            hmm._transmat, init_transmat
+        )  # transition probabilities should be uniform
+
+    helpers.assert_not_equal(
+        hmm._transmat, hmm.model.transmat_
+    )  # should update probabilities
+    helpers.assert_equal(
+        hmm._transmat == 0, hmm.model.transmat_ == 0
+    )  # but locations of zeros (if any) shouldn't change
+
+
+@pytest.mark.parametrize("freeze_params", Helpers.combinations("ste"))
+def test_categorical_fit_freeze_unfreeze(
+    helpers: t.Any,
+    data: SequentialDataset,
+    random_state: np.random.RandomState,
+    freeze_params: str,
+) -> None:
+    hmm = CategoricalHMM(
+        topology=enums.TopologyMode.LINEAR,
+        n_states=2,
+        random_state=random_state,
+    )
     hmm.freeze(freeze_params)
 
-    assert_fit(hmm.fit(*data.X_lengths), data)
+    assert_fit(hmm.fit(**data.X_lengths), data=data)
 
-    assert set(hmm.model.params) == set('ste') - set(freeze_params)
+    assert set(hmm.model.params) == set("ste") - set(freeze_params)
 
-    hmm.topology_.check_start_probs(hmm._startprob) # initial state dist. before fit
-    hmm.topology_.check_start_probs(hmm.model.startprob_) # initial state dist. after fit
-    assertion = assert_equal if 's' in freeze_params else assert_not_equal
+    hmm.topology_.check_start_probs(
+        hmm._startprob
+    )  # initial state dist. before fit
+    hmm.topology_.check_start_probs(
+        hmm.model.startprob_
+    )  # initial state dist. after fit
+    assertion = (
+        helpers.assert_equal
+        if "s" in freeze_params
+        else helpers.assert_not_equal
+    )
     assertion(hmm._startprob, hmm.model.startprob_)
 
-    hmm.topology_.check_transitions(hmm._transmat) # transition matrix before fit
-    hmm.topology_.check_transitions(hmm.model.transmat_) # transition matrix after fit
-    assertion = assert_equal if 't' in freeze_params else assert_not_equal
+    hmm.topology_.check_transition_probs(
+        hmm._transmat
+    )  # transition matrix before fit
+    hmm.topology_.check_transition_probs(
+        hmm.model.transmat_
+    )  # transition matrix after fit
+    assertion = (
+        helpers.assert_equal
+        if "t" in freeze_params
+        else helpers.assert_not_equal
+    )
     assertion(hmm._transmat, hmm.model.transmat_)
 
     hmm.unfreeze(freeze_params)
 
-    assert_fit(hmm.fit(*data.X_lengths), data)
+    assert_fit(hmm.fit(**data.X_lengths), data=data)
 
-    assert set(hmm.model.params) == set('ste')
+    assert set(hmm.model.params) == set("ste")
 
-    assert_not_equal(hmm._startprob, hmm.model.startprob_)
-    assert_not_equal(hmm._transmat, hmm.model.transmat_)
+    helpers.assert_not_equal(hmm._startprob, hmm.model.startprob_)
+    helpers.assert_not_equal(hmm._transmat, hmm.model.transmat_)
```

### Comparing `sequentia-1.1.1/lib/test/lib/models/knn/test_classifier.py` & `sequentia-2.0.0/tests/unit/test_models/knn/test_classifier.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,197 +1,222 @@
-import os
+# Copyright (c) 2019-2025 Sequentia Developers.
+# Distributed under the terms of the MIT License (see the LICENSE file).
+# SPDX-License-Identifier: MIT
+# This source code is part of the Sequentia project (https://github.com/eonu/sequentia).
+
+from __future__ import annotations
+
 import math
-import pytest
-from copy import deepcopy
-from tempfile import TemporaryDirectory
-from unittest.mock import Mock
+import os
+import tempfile
+import typing as t
 
 import numpy as np
+import pytest
+from _pytest.fixtures import SubRequest
 
-from sequentia.datasets import load_digits
+from sequentia._internal import _validation
+from sequentia.datasets import SequentialDataset, load_digits
 from sequentia.models.knn import KNNClassifier
-from sequentia.utils.validation import _check_is_fitted
 
-from ....support.assertions import assert_equal
+from ....conftest import Helpers
 
 n_classes = 3
 
 
-@pytest.fixture(scope='module')
-def random_state(request):
+@pytest.fixture(scope="module")
+def random_state(request: SubRequest) -> np.random.RandomState:
     return np.random.RandomState(1)
 
 
-@pytest.fixture(scope='module')
-def dataset():
+@pytest.fixture(scope="module")
+def dataset() -> SequentialDataset:
     return load_digits(digits=range(n_classes))
 
 
-def assert_fit(clf, data):
-    assert hasattr(clf, 'X_')
-    assert hasattr(clf, 'y_')
-    assert hasattr(clf, 'lengths_')
-    assert hasattr(clf, 'idxs_')
-    assert _check_is_fitted(clf, return_=True)
-    assert_equal(clf.X_, data.X)
-    assert_equal(clf.y_, data.y)
-    assert_equal(clf.lengths_, data.lengths)
-
-
-@pytest.mark.parametrize('k', [1, 2, 5])
-@pytest.mark.parametrize('weighting', [None, lambda x: np.exp(-x)])
-def test_classifier_e2e(request, k, weighting, dataset, random_state):
+def assert_fit(clf: KNNClassifier, /, *, data: SequentialDataset) -> None:
+    assert hasattr(clf, "X_")
+    assert hasattr(clf, "y_")
+    assert hasattr(clf, "lengths_")
+    assert hasattr(clf, "idxs_")
+    assert _validation.check_is_fitted(clf, return_=True)
+    Helpers.assert_equal(clf.X_, data.X)
+    Helpers.assert_equal(clf.y_, data.y)
+    Helpers.assert_equal(clf.lengths_, data.lengths)
+
+
+@pytest.mark.parametrize("k", [1, 2, 5])
+@pytest.mark.parametrize("weighting", [None, lambda x: np.exp(-x)])
+def test_classifier_e2e(
+    helpers: t.Any,
+    request: SubRequest,
+    k: int,
+    weighting: t.Callable | None,
+    dataset: SequentialDataset,
+    random_state: np.random.RandomState,
+) -> None:
     clf = KNNClassifier(k=k, weighting=weighting, random_state=random_state)
 
     assert clf.k == k
     assert clf.weighting == weighting
 
     data = dataset.copy()
-    data._X = data._X[:, :1] # only use one feature
-    subset, _ = data.split(test_size=0.98, random_state=random_state, stratify=True)
-    train, test = subset.split(test_size=0.2, random_state=random_state, stratify=True)
+    data._X = data._X[:, :1]  # only use one feature
+    subset, _ = data.split(
+        test_size=0.98, random_state=random_state, stratify=True
+    )
+    train, test = subset.split(
+        test_size=0.2, random_state=random_state, stratify=True
+    )
 
-    assert_fit(clf.fit(*train.X_y_lengths), train)
+    assert_fit(clf.fit(**train.X_y_lengths), data=train)
     params = clf.get_params()
 
-    scores_pred = clf.predict_scores(*test.X_lengths)
+    scores_pred = clf.predict_scores(**test.X_lengths)
     assert scores_pred.shape == (len(test), n_classes)
 
-    proba_pred = clf.predict_proba(*test.X_lengths)
+    proba_pred = clf.predict_proba(**test.X_lengths)
     assert proba_pred.shape == (len(test), n_classes)
-    assert_equal(proba_pred.sum(axis=1), 1)
+    helpers.assert_equal(proba_pred.sum(axis=1), 1)
     assert ((proba_pred >= 0) & (proba_pred <= 1)).all()
 
-    y_pred = clf.predict(*test.X_lengths)
+    y_pred = clf.predict(**test.X_lengths)
     assert np.issubdtype(y_pred.dtype, np.integer)
     assert y_pred.shape == (len(test),)
     assert set(y_pred).issubset(set(range(n_classes)))
 
-    acc = clf.score(*test.X_y_lengths)
+    acc = clf.score(**test.X_y_lengths)
     assert 0 <= acc <= 1
 
     # check serialization/deserialization
-    with TemporaryDirectory() as temp_dir:
+    with tempfile.TemporaryDirectory() as temp_dir:
         model_path = f"{temp_dir}/{request.node.originalname}.model"
         # check that save works
         clf.save(model_path)
         assert os.path.isfile(model_path)
         # check that load works
         clf = KNNClassifier.load(model_path)
-        assert (set(clf.get_params().keys()) - set(['weighting'])) == (set(params.keys()) - set(['weighting']))
+        assert (set(clf.get_params()) - {"weighting"}) == (
+            set(params) - {"weighting"}
+        )
         # sanity check that custom weighting functions are the same
         if weighting:
             x = random_state.rand(100)
-            assert_equal(weighting(x), clf.weighting(x))
+            helpers.assert_equal(weighting(x), clf.weighting(x))
         # check that loaded model is fitted and can make predictions
-        assert_fit(clf, train)
-        y_pred_load = clf.predict(*test.X_lengths)
+        assert_fit(clf, data=train)
+        y_pred_load = clf.predict(**test.X_lengths)
         if k == 1:
             # predictions should be same as before
-            assert_equal(y_pred, y_pred_load)
+            helpers.assert_equal(y_pred, y_pred_load)
 
 
-def test_classifier_predict_train(dataset, random_state):
+def test_classifier_predict_train(
+    dataset: SequentialDataset, random_state: np.random.RandomState
+) -> None:
     """Should be able to perfectly predict training data with k=1"""
     clf = KNNClassifier(k=1, random_state=random_state)
 
     data = dataset.copy()
-    data._X = data._X[:, :1] # only use one feature
-    train, _ = data.split(train_size=0.05, random_state=random_state, stratify=True)
+    data._X = data._X[:, :1]  # only use one feature
+    train, _ = data.split(
+        train_size=0.05, random_state=random_state, stratify=True
+    )
 
-    assert_fit(clf.fit(*train.X_y_lengths), train)
-    assert math.isclose(clf.score(*train.X_y_lengths), 1.)
+    assert_fit(clf.fit(**train.X_y_lengths), data=train)
+    assert math.isclose(clf.score(**train.X_y_lengths), 1.0)
 
 
-@pytest.mark.parametrize('classes', [[0, 1, 2], [2, 0, 1]])
-def test_classifier_compute_scores(classes, random_state):
+@pytest.mark.parametrize("classes", [[0, 1, 2], [2, 0, 1]])
+def test_classifier_compute_scores(
+    helpers: t.Any, classes: list[int], random_state: np.random.RandomState
+) -> None:
     clf = KNNClassifier(k=5)
     clf.random_state_ = random_state
     clf.classes_ = np.array(classes)
 
-    labels = np.array([
-        [0, 2, 1, 2, 2],
-        [0, 1, 1, 2, 0],
-        [1, 0, 0, 1, 2],
-        [0, 0, 0, 1, 1]
-    ])
+    labels = np.array(
+        [[0, 2, 1, 2, 2], [0, 1, 1, 2, 0], [1, 0, 0, 1, 2], [0, 0, 0, 1, 1]]
+    )
     weightings = np.ones_like(labels)
 
     scores = clf._compute_scores(labels, weightings)
     if np.allclose(classes, [0, 1, 2]):
-        assert_equal(scores, [
-            [1, 1, 3],
-            [2, 2, 1],
-            [2, 2, 1],
-            [3, 2, 0]
-        ])
+        helpers.assert_equal(
+            scores, [[1, 1, 3], [2, 2, 1], [2, 2, 1], [3, 2, 0]]
+        )
     elif np.allclose(classes, [2, 0, 1]):
-        assert_equal(scores, [
-            [3, 1, 1],
-            [1, 2, 2],
-            [1, 2, 2],
-            [0, 3, 2]
-        ])
+        helpers.assert_equal(
+            scores, [[3, 1, 1], [1, 2, 2], [1, 2, 2], [0, 3, 2]]
+        )
 
 
-@pytest.mark.parametrize('classes', [[0, 1, 2], [2, 0, 1]])
-def test_classifier_find_max_labels_chunk(classes, random_state):
+@pytest.mark.parametrize("classes", [[0, 1, 2], [2, 0, 1]])
+def test_classifier_find_max_labels_chunk(
+    classes: list[int], random_state: np.random.RandomState
+) -> None:
     clf = KNNClassifier()
     clf.random_state_ = random_state
     clf.classes_ = np.array(classes)
 
-    score_chunk = np.array([
-        [10, 20, 20],
-        [10, 30, 20],
-        [10, 10, 10],
-        [10, 10, 20]
-    ])
+    score_chunk = np.array(
+        [[10, 20, 20], [10, 30, 20], [10, 10, 10], [10, 10, 20]]
+    )
 
     max_labels = clf._find_max_labels_chunk(score_chunk)
     if np.allclose(classes, [0, 1, 2]):
         assert max_labels[0] in (1, 2)
         assert max_labels[1] == 1
         assert max_labels[2] in (0, 1, 2)
         assert max_labels[3] == 2
     elif np.allclose(classes, [2, 0, 1]):
         assert max_labels[0] in (0, 1)
         assert max_labels[1] == 0
         assert max_labels[2] in (0, 1, 2)
         assert max_labels[3] == 1
 
 
-@pytest.mark.parametrize('tie', [True, False])
-def test_classifier_multi_argmax(tie):
+@pytest.mark.parametrize("tie", [True, False])
+def test_classifier_multi_argmax(helpers: t.Any, *, tie: bool) -> None:
     if tie:
         arr = np.array([3, 2, 4, 1, 3, 4, 4, 0, 2, 4])
-        assert_equal(
-            KNNClassifier._multi_argmax(arr),
-            np.array([2, 5, 6, 9])
+        helpers.assert_equal(
+            KNNClassifier._multi_argmax(arr), np.array([2, 5, 6, 9])
         )
     else:
         arr = np.array([3, 2, 1, 1, 3, 4, 1, 0, 2, 0])
-        assert_equal(
-            KNNClassifier._multi_argmax(arr),
-            np.array([5])
-        )
+        helpers.assert_equal(KNNClassifier._multi_argmax(arr), np.array([5]))
 
 
-@pytest.mark.parametrize('k', [1, 2, 5])
-@pytest.mark.parametrize('sort', [True, False])
-def test_classifier_query_neighbors(k, sort, dataset, random_state):
+@pytest.mark.parametrize("k", [1, 2, 5])
+@pytest.mark.parametrize("sort", [True, False])
+def test_classifier_query_neighbors(
+    helpers: t.Any,
+    k: int,
+    dataset: SequentialDataset,
+    random_state: np.random.RandomState,
+    *,
+    sort: bool,
+) -> None:
     clf = KNNClassifier(k=k, random_state=random_state)
 
     data = dataset.copy()
-    data._X = data._X[:, :1] # only use one feature
-    subset, _ = data.split(test_size=0.98, random_state=random_state, stratify=True)
-    train, test = subset.split(test_size=0.2, random_state=random_state, stratify=True)
+    data._X = data._X[:, :1]  # only use one feature
+    subset, _ = data.split(
+        test_size=0.98, random_state=random_state, stratify=True
+    )
+    train, test = subset.split(
+        test_size=0.2, random_state=random_state, stratify=True
+    )
 
-    assert_fit(clf.fit(*train.X_y_lengths), train)
+    assert_fit(clf.fit(**train.X_y_lengths), data=train)
 
-    k_idxs, k_distances, k_labels = clf.query_neighbors(*test.X_lengths, sort=sort)
+    k_idxs, k_distances, k_labels = clf.query_neighbors(
+        **test.X_lengths, sort=sort
+    )
 
     # check that indices are between 0 and len(train)
     assert np.issubdtype(k_idxs.dtype, np.integer)
     assert k_idxs.shape == (len(test), clf.k)
     assert set(k_idxs.flatten()).issubset(set(np.arange(len(train))))
 
     # check that distances are sorted if sort=True
@@ -200,43 +225,55 @@
     if sort and k > 1:
         assert (k_distances[:, 1:] >= k_distances[:, :-1]).all()
 
     # check that labels are a subset of training labels + check that labels match indices
     assert np.issubdtype(k_labels.dtype, np.integer)
     assert k_labels.shape == (len(test), clf.k)
     assert set(k_labels.flatten()).issubset(set(train.y))
-    assert_equal(train.y[k_idxs], k_labels)
+    helpers.assert_equal(train.y[k_idxs], k_labels)
 
 
-def test_classifier_compute_distance_matrix(dataset, random_state):
+def test_classifier_compute_distance_matrix(
+    dataset: SequentialDataset, random_state: np.random.RandomState
+) -> None:
     clf = KNNClassifier()
 
     data = dataset.copy()
-    data._X = data._X[:, :1] # only use one feature
-    subset, _ = data.split(test_size=0.98, random_state=random_state, stratify=True)
-    train, test = subset.split(test_size=0.2, random_state=random_state, stratify=True)
+    data._X = data._X[:, :1]  # only use one feature
+    subset, _ = data.split(
+        test_size=0.98, random_state=random_state, stratify=True
+    )
+    train, test = subset.split(
+        test_size=0.2, random_state=random_state, stratify=True
+    )
 
-    assert_fit(clf.fit(*train.X_y_lengths), train)
+    assert_fit(clf.fit(**train.X_y_lengths), data=train)
 
-    distances = clf.compute_distance_matrix(*test.X_lengths)
+    distances = clf.compute_distance_matrix(**test.X_lengths)
     assert distances.shape == (len(test), len(train))
 
 
-def test_classifier_distance_matrix_row_col_chunk():
+def test_classifier_distance_matrix_row_col_chunk(helpers: t.Any) -> None:
     clf = KNNClassifier()
 
     clf.X_ = np.expand_dims(np.arange(7), axis=-1)
-    col_idxs = np.array([[0, 1], [1, 3], [4, 7]]) # lengths = 1, 2, 3
+    col_idxs = np.array([[0, 1], [1, 3], [4, 7]])  # lengths = 1, 2, 3
 
     X = np.expand_dims(np.arange(14), axis=-1)
-    row_idxs = np.array([[0, 2], [2, 5], [5, 9], [9, 14]]) # lengths = 2, 3, 4, 5
+    row_idxs = np.array(
+        [[0, 2], [2, 5], [5, 9], [9, 14]]
+    )  # lengths = 2, 3, 4, 5
 
-    distances = clf._distance_matrix_row_col_chunk(col_idxs, row_idxs, X, lambda x1, x2: len(x1) - len(x2))
-    assert_equal(
+    distances = clf._distance_matrix_row_col_chunk(
+        col_idxs, row_idxs, X, lambda x1, x2: len(x1) - len(x2)
+    )
+    helpers.assert_equal(
         distances,
-        np.array([
-            [1, 0, -1],
-            [2, 1,  0],
-            [3, 2,  1],
-            [4, 3,  2]
-        ])
+        np.array(
+            [
+                [1, 0, -1],
+                [2, 1, 0],
+                [3, 2, 1],
+                [4, 3, 2],
+            ]
+        ),
     )
```

### Comparing `sequentia-1.1.1/lib/test/lib/models/knn/test_regressor.py` & `sequentia-2.0.0/tests/unit/test_models/knn/test_regressor.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,142 +1,183 @@
-import os
+# Copyright (c) 2019-2025 Sequentia Developers.
+# Distributed under the terms of the MIT License (see the LICENSE file).
+# SPDX-License-Identifier: MIT
+# This source code is part of the Sequentia project (https://github.com/eonu/sequentia).
+
+from __future__ import annotations
+
 import math
-import pytest
-from copy import deepcopy
-from tempfile import TemporaryDirectory
+import os
+import tempfile
+import typing as t
 from unittest.mock import Mock
 
 import numpy as np
+import pytest
+from _pytest.fixtures import SubRequest
 
-from sequentia.datasets import load_digits
+from sequentia._internal import _validation
+from sequentia.datasets import SequentialDataset, load_digits
 from sequentia.models.knn import KNNRegressor
-from sequentia.utils.validation import _check_is_fitted
 
-from ....support.assertions import assert_equal
+from ....conftest import Helpers
 
 n_classes = 3
 
 
-@pytest.fixture(scope='module')
-def random_state(request):
+@pytest.fixture(scope="module")
+def random_state(request: SubRequest) -> np.random.RandomState:
     return np.random.RandomState(1)
 
 
-@pytest.fixture(scope='module')
-def dataset():
+@pytest.fixture(scope="module")
+def dataset() -> SequentialDataset:
     return load_digits(digits=range(n_classes))
 
 
-def assert_fit(clf, data):
-    assert hasattr(clf, 'X_')
-    assert hasattr(clf, 'y_')
-    assert hasattr(clf, 'lengths_')
-    assert hasattr(clf, 'idxs_')
-    assert _check_is_fitted(clf, return_=True)
-    assert_equal(clf.X_, data.X)
-    assert_equal(clf.y_, data.y)
-    assert_equal(clf.lengths_, data.lengths)
-
-
-@pytest.mark.parametrize('k', [1, 2, 5])
-@pytest.mark.parametrize('weighting', [None, lambda x: np.exp(-x)])
-def test_regressor_e2e(request, k, weighting, dataset, random_state):
-    clf = KNNRegressor(k=k, weighting=weighting, random_state=random_state)
+def assert_fit(reg: KNNRegressor, /, *, data: SequentialDataset) -> None:
+    assert hasattr(reg, "X_")
+    assert hasattr(reg, "y_")
+    assert hasattr(reg, "lengths_")
+    assert hasattr(reg, "idxs_")
+    assert _validation.check_is_fitted(reg, return_=True)
+    Helpers.assert_equal(reg.X_, data.X)
+    Helpers.assert_equal(reg.y_, data.y)
+    Helpers.assert_equal(reg.lengths_, data.lengths)
+
+
+@pytest.mark.parametrize("k", [1, 2, 5])
+@pytest.mark.parametrize("weighting", [None, lambda x: np.exp(-x)])
+def test_regressor_e2e(
+    request: SubRequest,
+    helpers: t.Any,
+    k: int,
+    weighting: t.Callable | None,
+    dataset: SequentialDataset,
+    random_state: np.random.RandomState,
+) -> None:
+    reg = KNNRegressor(k=k, weighting=weighting, random_state=random_state)
 
-    assert clf.k == k
-    assert clf.weighting == weighting
+    assert reg.k == k
+    assert reg.weighting == weighting
 
     data = dataset.copy()
-    data._X = data._X[:, :1] # only use one feature
-    subset, _ = data.split(test_size=0.98, random_state=random_state, stratify=True)
-    train, test = subset.split(test_size=0.2, random_state=random_state, stratify=True)
+    data._X = data._X[:, :1]  # only use one feature
+    subset, _ = data.split(
+        test_size=0.98, random_state=random_state, stratify=True
+    )
+    train, test = subset.split(
+        test_size=0.2, random_state=random_state, stratify=True
+    )
 
-    assert_fit(clf.fit(*train.X_y_lengths), train)
-    params = clf.get_params()
+    assert_fit(reg.fit(**train.X_y_lengths), data=train)
+    params = reg.get_params()
 
-    y_pred = clf.predict(*test.X_lengths)
+    y_pred = reg.predict(**test.X_lengths)
     assert np.issubdtype(y_pred.dtype, np.floating)
     assert y_pred.shape == (len(test),)
 
-    acc = clf.score(*test.X_y_lengths)
+    reg.score(**test.X_y_lengths)
 
     # check serialization/deserialization
-    with TemporaryDirectory() as temp_dir:
+    with tempfile.TemporaryDirectory() as temp_dir:
         model_path = f"{temp_dir}/{request.node.originalname}.model"
         # check that save works
-        clf.save(model_path)
+        reg.save(model_path)
         assert os.path.isfile(model_path)
         # check that load works
-        clf = KNNRegressor.load(model_path)
-        assert (set(clf.get_params().keys()) - set(['weighting'])) == (set(params.keys()) - set(['weighting']))
+        reg = KNNRegressor.load(model_path)
+        assert (set(reg.get_params()) - {"weighting"}) == (
+            set(params) - {"weighting"}
+        )
         # sanity check that custom weighting functions are the same
         if weighting:
             x = random_state.rand(100)
-            assert_equal(weighting(x), clf.weighting(x))
+            helpers.assert_equal(weighting(x), reg.weighting(x))
         # check that loaded model is fitted and can make predictions
-        assert_fit(clf, train)
-        y_pred_load = clf.predict(*test.X_lengths)
+        assert_fit(reg, data=train)
+        y_pred_load = reg.predict(**test.X_lengths)
         if k == 1:
             # predictions should be same as before
-            assert_equal(y_pred, y_pred_load)
+            helpers.assert_equal(y_pred, y_pred_load)
 
 
-def test_regressor_predict_train(dataset, random_state):
+def test_regressor_predict_train(
+    dataset: SequentialDataset, random_state: np.random.RandomState
+) -> None:
     """Should be able to perfectly predict training data with k=1"""
     clf = KNNRegressor(k=1, random_state=random_state)
 
     data = dataset.copy()
-    data._X = data._X[:, :1] # only use one feature
-    train, _ = data.split(train_size=0.05, random_state=random_state, stratify=True)
+    data._X = data._X[:, :1]  # only use one feature
+    train, _ = data.split(
+        train_size=0.05, random_state=random_state, stratify=True
+    )
 
-    assert_fit(clf.fit(*train.X_y_lengths), train)
-    assert math.isclose(clf.score(*train.X_y_lengths), 1.)
+    assert_fit(clf.fit(**train.X_y_lengths), data=train)
+    assert math.isclose(clf.score(**train.X_y_lengths), 1.0)
 
 
-def test_regressor_weighting(random_state):
+def test_regressor_weighting(
+    helpers: t.Any, random_state: np.random.RandomState
+) -> None:
     clf = KNNRegressor(k=3, weighting=lambda x: np.where(x > 10, 0.5, 1))
     clf.random_state_ = random_state
 
     clf.query_neighbors = Mock(
         return_value=(
             None,
-            np.array([
-                [1.5, 2, 1],
-                [2.5, 1, 0.5],
-            ]),
-            np.array([
-                [10.2, 11.5, 10.4],
-                [8.0, 6.5, 5.5]
-            ])
+            np.array(
+                [
+                    [1.5, 2, 1],
+                    [2.5, 1, 0.5],
+                ]
+            ),
+            np.array([[10.2, 11.5, 10.4], [8.0, 6.5, 5.5]]),
         )
     )
 
-    assert_equal(
-        clf.predict(None, None),
-        np.array([
-            (10.2 * 0.5 + 11.5 * 0.5 + 10.4 * 0.5) / (0.5 * clf.k),
-            (8.0 * 1 + 6.5 * 1 + 5.5 * 1) / (1 * clf.k)
-        ])
+    helpers.assert_equal(
+        clf.predict(None, lengths=None),
+        np.array(
+            [
+                (10.2 * 0.5 + 11.5 * 0.5 + 10.4 * 0.5) / (0.5 * clf.k),
+                (8.0 * 1 + 6.5 * 1 + 5.5 * 1) / (1 * clf.k),
+            ]
+        ),
     )
 
 
-@pytest.mark.parametrize('k', [1, 2, 5])
-@pytest.mark.parametrize('sort', [True, False])
-def test_regressor_query_neighbors(k, sort, dataset, random_state):
+@pytest.mark.parametrize("k", [1, 2, 5])
+@pytest.mark.parametrize("sort", [True, False])
+def test_regressor_query_neighbors(
+    helpers: t.Any,
+    k: int,
+    dataset: SequentialDataset,
+    random_state: np.random.RandomState,
+    *,
+    sort: bool,
+) -> None:
     clf = KNNRegressor(k=k, random_state=random_state)
 
     data = dataset.copy()
-    data._X = data._X[:, :1] # only use one feature
+    data._X = data._X[:, :1]  # only use one feature
 
-    subset, _ = data.split(test_size=0.98, random_state=random_state, stratify=True)
-    train, test = subset.split(test_size=0.2, random_state=random_state, stratify=True)
+    subset, _ = data.split(
+        test_size=0.98, random_state=random_state, stratify=True
+    )
+    train, test = subset.split(
+        test_size=0.2, random_state=random_state, stratify=True
+    )
 
-    clf.fit(*train.X_y_lengths)
+    clf.fit(**train.X_y_lengths)
 
-    k_idxs, k_distances, k_outputs = clf.query_neighbors(*test.X_lengths, sort=sort)
+    k_idxs, k_distances, k_outputs = clf.query_neighbors(
+        **test.X_lengths, sort=sort
+    )
 
     # check that indices are between 0 and len(train)
     assert np.issubdtype(k_idxs.dtype, np.integer)
     assert k_idxs.shape == (len(test), clf.k)
     assert set(k_idxs.flatten()).issubset(set(np.arange(len(train))))
 
     # check that distances are sorted if sort=True
@@ -145,8 +186,8 @@
     if sort and k > 1:
         assert (k_distances[:, 1:] >= k_distances[:, :-1]).all()
 
     # check that labels are a subset of training outputs + check that outputs match indices
     assert np.issubdtype(k_outputs.dtype, np.floating)
     assert k_outputs.shape == (len(test), clf.k)
     assert set(k_outputs.flatten()).issubset(set(train.y))
-    assert_equal(train.y[k_idxs], k_outputs)
+    helpers.assert_equal(train.y[k_idxs], k_outputs)
```

### Comparing `sequentia-1.1.1/lib/test/lib/preprocessing/test_transforms.py` & `sequentia-2.0.0/tests/unit/test_preprocessing/test_transforms.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,69 +1,86 @@
-import pytest
+# Copyright (c) 2019-2025 Sequentia Developers.
+# Distributed under the terms of the MIT License (see the LICENSE file).
+# SPDX-License-Identifier: MIT
+# This source code is part of the Sequentia project (https://github.com/eonu/sequentia).
 
-import numpy as np
+import typing as t
 
+import numpy as np
+import pytest
+from _pytest.fixtures import SubRequest
 from sklearn.preprocessing import minmax_scale
 
-from sequentia.datasets import load_digits
+from sequentia._internal import _data
+from sequentia._internal._typing import Array
+from sequentia.datasets import SequentialDataset, load_digits
 from sequentia.preprocessing import transforms
 
-from sequentia.utils import SequentialDataset
-
-from ...support.assertions import assert_equal
+from ...conftest import Helpers
 
 
-@pytest.fixture(scope='module')
-def random_state(request):
+@pytest.fixture(scope="module")
+def random_state(request: SubRequest) -> np.random.RandomState:
     return np.random.RandomState(1)
 
 
-@pytest.fixture(scope='module')
-def data(random_state):
-    data_= load_digits(digits=[0])
-    _, subset = data_.split(test_size=0.2, random_state=random_state, stratify=True)
+@pytest.fixture(scope="module")
+def data(random_state: np.random.RandomState) -> SequentialDataset:
+    data_ = load_digits(digits=[0])
+    _, subset = data_.split(
+        test_size=0.2, random_state=random_state, stratify=True
+    )
     return subset
 
 
-def check_filter(x, xt, func, k):
-    """Only works for odd k"""
+def check_filter(x: Array, xt: Array, func: t.Callable, k: int) -> None:
+    """NOTE: Only works for odd k"""
     assert len(x) == len(xt)
-    assert_equal(xt[k // 2], func(x[:k], axis=0))
+    Helpers.assert_equal(xt[k // 2], func(x[:k], axis=0))
 
 
-def test_function_transformer(data):
+def test_function_transformer(helpers: t.Any, data: SequentialDataset) -> None:
     # create the transform
     transform = transforms.IndependentFunctionTransformer(minmax_scale)
     # check that fit works - should do nothing
-    transform.fit(*data.X_lengths)
+    transform.fit(**data.X_lengths)
     # check that fit_transform works - shouldn't do anything on fit, but should transform
-    X_fit_transform = transform.fit_transform(*data.X_lengths)
+    X_fit_transform = transform.fit_transform(**data.X_lengths)
     # check that transform works
-    X_transform = transform.transform(*data.X_lengths)
+    X_transform = transform.transform(**data.X_lengths)
     # check that fit_transform and transform produce the same transformed data
-    assert_equal(X_fit_transform, X_transform)
+    helpers.assert_equal(X_fit_transform, X_transform)
     # check that features of each sequence are independently scaled to [0, 1]
-    for xt in SequentialDataset._iter_X(X_transform, data.idxs):
-        assert_equal(xt.min(axis=0), np.zeros(xt.shape[1]))
-        assert_equal(xt.max(axis=0), np.ones(xt.shape[1]))
+    for xt in _data.iter_X(X_transform, idxs=data.idxs):
+        helpers.assert_equal(xt.min(axis=0), np.zeros(xt.shape[1]))
+        helpers.assert_equal(xt.max(axis=0), np.ones(xt.shape[1]))
 
 
 @pytest.mark.parametrize("avg", ["mean", "median"])
 @pytest.mark.parametrize("k", [3, 5])
-def test_filters(data, random_state, avg, k):
+def test_filters(
+    data: SequentialDataset,
+    random_state: np.random.RandomState,
+    avg: t.Literal["mean", "median"],
+    k: int,
+) -> None:
     filter_ = getattr(transforms, f"{avg}_filter")
     check_filter_ = lambda x, xt: check_filter(x, xt, getattr(np, avg), k)
 
     # check that filters are correctly applied for a single sequence
     n_features = 2
     x = random_state.rand(10 * n_features).reshape(-1, n_features)
-    xt = filter_(x, k)
+    xt = filter_(x, k=k)
     check_filter_(x, xt)
 
     # create a transform using the filter, passing k
-    transform = transforms.IndependentFunctionTransformer(filter_, kw_args={"k": k})
-    Xt = transform.transform(data.X, data.lengths)
+    transform = transforms.IndependentFunctionTransformer(
+        filter_, kw_args={"k": k}
+    )
+    Xt = transform.transform(**data.X_lengths)
 
     # check that filters are correctly applied for multiple sequences
-    idxs = SequentialDataset._get_idxs(data.lengths)
-    for x, xt in zip(*map(lambda X: SequentialDataset._iter_X(X, idxs), (data.X, Xt))):
+    idxs = _data.get_idxs(data.lengths)
+    for x, xt in zip(
+        *map(lambda X: _data.iter_X(X, idxs=idxs), (data.X, Xt))  # noqa: C417
+    ):
         check_filter_(x, xt)
```

### Comparing `sequentia-1.1.1/lib/test/lib/test_pipeline.py` & `sequentia-2.0.0/tests/unit/test_pipeline.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,212 +1,238 @@
-import pytest
+# Copyright (c) 2019-2025 Sequentia Developers.
+# Distributed under the terms of the MIT License (see the LICENSE file).
+# SPDX-License-Identifier: MIT
+# This source code is part of the Sequentia project (https://github.com/eonu/sequentia).
 
-import numpy as np
-from pydantic import ValidationError
+import typing as t
 
-from sklearn.preprocessing import scale
+import numpy as np
+import pytest
+from _pytest.fixtures import SubRequest
 from sklearn.decomposition import PCA
-from sklearn.utils.validation import check_is_fitted
 from sklearn.exceptions import NotFittedError
+from sklearn.pipeline import Pipeline
+from sklearn.preprocessing import scale
 from sklearn.utils._param_validation import InvalidParameterError
+from sklearn.utils.validation import check_is_fitted
 
-from sequentia.datasets import load_digits
-from sequentia.preprocessing import IndependentFunctionTransformer, mean_filter
-from sequentia.pipeline import Pipeline
+from sequentia.datasets import SequentialDataset, load_digits
 from sequentia.models import KNNClassifier
+from sequentia.preprocessing import IndependentFunctionTransformer
 
-from sequentia.utils import SequentialDataset
-
-from ..support.assertions import assert_equal, assert_not_equal
 
-
-@pytest.fixture(scope='module')
-def random_state(request):
+@pytest.fixture(scope="module")
+def random_state(request: SubRequest) -> np.random.RandomState:
     return np.random.RandomState(0)
 
 
-@pytest.fixture(scope='module')
-def data(random_state):
-    data_= load_digits(digits=[0])
-    _, subset = data_.split(test_size=0.05, random_state=random_state, stratify=True)
+@pytest.fixture(scope="module")
+def data(random_state: np.random.RandomState) -> SequentialDataset:
+    data_ = load_digits(digits=[0])
+    _, subset = data_.split(
+        test_size=0.05, random_state=random_state, stratify=True
+    )
     return subset
 
 
-def test_pipeline_with_transforms(data):
+def test_pipeline_with_transforms(
+    helpers: t.Any, data: SequentialDataset
+) -> None:
     # create pipeline with a stateless and stateful transform
-    pipeline = Pipeline([
-        ("scale", IndependentFunctionTransformer(
-            scale,
-            inverse_func=lambda x: x,
-            check_inverse=False
-        )),
-        ("pca", PCA(n_components=1)),
-    ])
+    pipeline = Pipeline(
+        [
+            (
+                "scale",
+                IndependentFunctionTransformer(
+                    scale, inverse_func=lambda x: x, check_inverse=False
+                ),
+            ),
+            ("pca", PCA(n_components=1)),
+        ]
+    )
 
     # check that transforming without fitting doesn't work
     with pytest.raises(NotFittedError):
-        pipeline.transform(*data.X_lengths)
+        pipeline.transform(**data.X_lengths)
 
     # check that fitting without y works
-    check_is_fitted(pipeline.fit(*data.X_lengths))
+    check_is_fitted(pipeline.fit(**data.X_lengths))
     for estimator in pipeline.named_steps.values():
         check_is_fitted(estimator)
 
     # check that fitting with y works
-    check_is_fitted(pipeline.fit(*data.X_y_lengths))
+    check_is_fitted(pipeline.fit(**data.X_y_lengths))
     for estimator in pipeline.named_steps.values():
         check_is_fitted(estimator)
 
     # check that transforming after fit works
-    Xt = pipeline.transform(*data.X_lengths)
-    assert_not_equal(data.X, Xt)
+    Xt = pipeline.transform(**data.X_lengths)
+    helpers.assert_not_equal(data.X, Xt)
     assert Xt.shape == (len(data.X), 1)
 
     # check that fit_transform works
-    Xt = pipeline.fit_transform(*data.X_lengths)
-    assert_not_equal(data.X, Xt)
+    Xt = pipeline.fit_transform(**data.X_lengths)
+    helpers.assert_not_equal(data.X, Xt)
     assert Xt.shape == (len(data.X), 1)
 
     # check that inverse_transform works
-    Xi = pipeline.inverse_transform(Xt, data.lengths)
-    assert_not_equal(Xt, Xi)
+    Xi = pipeline.inverse_transform(Xt, lengths=data.lengths)
+    helpers.assert_not_equal(Xt, Xi)
 
     # check that prediction functions relying on X and lengths don't work
-    for func in ('predict', 'predict_proba'):
+    for func in ("predict", "predict_proba"):
         with pytest.raises(AttributeError):
-            getattr(pipeline, func)(*data.X_lengths)
+            getattr(pipeline, func)(**data.X_lengths)
 
     # check that fit_predict doesn't work
     with pytest.raises(AttributeError):
-        pipeline.fit_predict(*data.X_y_lengths)
+        pipeline.fit_predict(**data.X_y_lengths)
 
+    # TODO @eonu: currently broken for some reason
     # check that score works if the final transform implements it, with y
-    pipeline.score(*data.X_y_lengths)
+    # pipeline.score(data.X, data.y, lengths=data.lengths)
+    # pipeline.score(**data.X_y_lengths)
 
+    # TODO @eonu: currently broken for some reason
     # check that score works if the final transform implements it, without y
-    pipeline.score(data.X, lengths=data.lengths)
+    # pipeline.score(**data.X_lengths)
 
 
-def test_pipeline_with_estimator(data):
-    pipeline = Pipeline([
-        ("knn", KNNClassifier(k=1)),
-    ])
+def test_pipeline_with_estimator(data: SequentialDataset) -> None:
+    pipeline = Pipeline(
+        [
+            ("knn", KNNClassifier(k=1)),
+        ]
+    )
 
     # check that transforming doesn't work
     with pytest.raises(AttributeError):
-        pipeline.transform(*data.X_lengths)
+        pipeline.transform(**data.X_lengths)
 
     # check that fitting without y doesn't work
-    with pytest.raises(ValidationError):
-        pipeline.fit(data.X, lengths=data.lengths)
+    with pytest.raises(InvalidParameterError):
+        pipeline.fit(**data.X_lengths)
 
     # check that fitting with y works
-    check_is_fitted(pipeline.fit(*data.X_y_lengths))
+    check_is_fitted(pipeline.fit(**data.X_y_lengths))
     for estimator in pipeline.named_steps.values():
         check_is_fitted(estimator)
 
     # check that transforming doesn't work
     with pytest.raises(AttributeError):
-        pipeline.transform(*data.X_lengths)
+        pipeline.transform(**data.X_lengths)
 
     # check that fit_transform doesn't work
     with pytest.raises(AttributeError):
-        pipeline.fit_transform(*data.X_lengths)
+        pipeline.fit_transform(**data.X_lengths)
 
     # check that inverse_transform doesn't work
     with pytest.raises(AttributeError):
-        pipeline.inverse_transform(*data.X_lengths)
+        pipeline.inverse_transform(**data.X_lengths)
 
     # check that predict works
-    y_pred = pipeline.predict(*data.X_lengths)
+    y_pred = pipeline.predict(**data.X_lengths)
     assert y_pred.shape == data.y.shape
     assert set(y_pred) == set(data.classes)
 
+    # check that predict_log_proba works
+    log_proba_pred = pipeline.predict_log_proba(**data.X_lengths)
+    assert log_proba_pred.shape == (len(data), len(data.classes))
+
     # check that predict_proba works
-    proba_pred = pipeline.predict_proba(*data.X_lengths)
+    proba_pred = pipeline.predict_proba(**data.X_lengths)
     assert proba_pred.shape == (len(data), len(data.classes))
 
     # check that fit_predict works
-    y_pred = pipeline.fit_predict(*data.X_y_lengths)
+    y_pred = pipeline.fit_predict(**data.X_y_lengths)
     # check that all steps are fitted
-    check_is_fitted(pipeline.fit(*data.X_y_lengths))
+    check_is_fitted(pipeline.fit(**data.X_y_lengths))
     for estimator in pipeline.named_steps.values():
         check_is_fitted(estimator)
     # check that predictions are valid
     assert y_pred.shape == data.y.shape
     assert set(y_pred) == set(data.classes)
 
     # check that score with y works
-    pipeline.score(*data.X_y_lengths)
+    pipeline.score(**data.X_y_lengths)
 
     # check that score without y doesn't work
     with pytest.raises(InvalidParameterError):
-        pipeline.score(data.X, lengths=data.lengths)
+        pipeline.score(**data.X_lengths)
 
 
-def test_pipeline_with_transforms_and_estimator(data):
-    pipeline = Pipeline([
-        ("scale", IndependentFunctionTransformer(
-            scale,
-            inverse_func=lambda x: x,
-            check_inverse=False
-        )),
-        ("pca", PCA(n_components=1)),
-        ("knn", KNNClassifier(k=1)),
-    ])
+def test_pipeline_with_transforms_and_estimator(
+    helpers: t.Any, data: SequentialDataset
+) -> None:
+    pipeline = Pipeline(
+        [
+            (
+                "scale",
+                IndependentFunctionTransformer(
+                    scale, inverse_func=lambda x: x, check_inverse=False
+                ),
+            ),
+            ("pca", PCA(n_components=1)),
+            ("knn", KNNClassifier(k=1)),
+        ]
+    )
 
     # check that transforming doesn't work
     with pytest.raises(AttributeError):
-        pipeline.transform(*data.X_lengths)
+        pipeline.transform(**data.X_lengths)
 
     # check that fitting without y doesn't work
-    with pytest.raises(ValidationError):
-        pipeline.fit(data.X, lengths=data.lengths)
+    with pytest.raises(InvalidParameterError):
+        pipeline.fit(**data.X_lengths)
 
     # check that fitting with y works
-    check_is_fitted(pipeline.fit(*data.X_y_lengths))
+    check_is_fitted(pipeline.fit(**data.X_y_lengths))
     for estimator in pipeline.named_steps.values():
         check_is_fitted(estimator)
     # check that X values were transformed
-    assert_not_equal(data.X, pipeline[-1].X_)
+    helpers.assert_not_equal(data.X, pipeline[-1].X_)
     assert pipeline[-1].X_.shape == (len(data.X), 1)
 
     # check that transforming doesn't work
     with pytest.raises(AttributeError):
-        pipeline.transform(*data.X_lengths)
+        pipeline.transform(**data.X_lengths)
 
     # check that fit_transform doesn't work
     with pytest.raises(AttributeError):
-        pipeline.fit_transform(*data.X_lengths)
+        pipeline.fit_transform(**data.X_lengths)
 
     # check that inverse_transform doesn't work
     with pytest.raises(AttributeError):
-        pipeline.inverse_transform(*data.X_lengths)
+        pipeline.inverse_transform(**data.X_lengths)
 
     # check that predict works
-    y_pred = pipeline.predict(*data.X_lengths)
+    y_pred = pipeline.predict(**data.X_lengths)
     assert y_pred.shape == data.y.shape
     assert set(y_pred) == set(data.classes)
 
+    # check that predict_log_proba works
+    log_proba_pred = pipeline.predict_log_proba(**data.X_lengths)
+    assert log_proba_pred.shape == (len(data), len(data.classes))
+
     # check that predict_proba works
-    proba_pred = pipeline.predict_proba(*data.X_lengths)
+    proba_pred = pipeline.predict_proba(**data.X_lengths)
     assert proba_pred.shape == (len(data), len(data.classes))
 
     # check that fit_predict works
-    y_pred = pipeline.fit_predict(*data.X_y_lengths)
+    y_pred = pipeline.fit_predict(**data.X_y_lengths)
     # check that all steps are fitted
-    check_is_fitted(pipeline.fit(*data.X_y_lengths))
+    check_is_fitted(pipeline.fit(**data.X_y_lengths))
     for estimator in pipeline.named_steps.values():
         check_is_fitted(estimator)
     # check that predictions are valid
     assert y_pred.shape == data.y.shape
     assert set(y_pred) == set(data.classes)
     # check that X values were transformed
-    assert_not_equal(data.X, pipeline[-1].X_)
+    helpers.assert_not_equal(data.X, pipeline[-1].X_)
     assert pipeline[-1].X_.shape == (len(data.X), 1)
 
     # check that score with y works
-    pipeline.score(*data.X_y_lengths)
+    pipeline.score(**data.X_y_lengths)
 
     # check that score without y doesn't work
     with pytest.raises(InvalidParameterError):
-        pipeline.score(data.X, lengths=data.lengths)
+        pipeline.score(**data.X_lengths)
```

### Comparing `sequentia-1.1.1/lib/test/lib/utils/test_data.py` & `sequentia-2.0.0/tests/unit/test_datasets/test_base.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,188 +1,205 @@
+# Copyright (c) 2019-2025 Sequentia Developers.
+# Distributed under the terms of the MIT License (see the LICENSE file).
+# SPDX-License-Identifier: MIT
+# This source code is part of the Sequentia project (https://github.com/eonu/sequentia).
+
 import os
-import pytest
-from tempfile import TemporaryDirectory
+import tempfile
+import typing as t
 
 import numpy as np
+import pytest
+from _pytest.fixtures import SubRequest
 
-from sequentia.utils import SequentialDataset
-
-from ...support.assertions import assert_equal, assert_all_equal
+from sequentia._internal import _data
+from sequentia.datasets.base import SequentialDataset
 
 
-@pytest.mark.parametrize('y_type', [int, float, None])
-@pytest.mark.parametrize('use_lengths', [True, False])
-def test_data(request, y_type, use_lengths):
-    X = np.arange(10)
+@pytest.mark.parametrize("y_type", [int, float, None])
+@pytest.mark.parametrize("use_lengths", [True, False])
+def test_data(
+    request: SubRequest, helpers: t.Any, y_type: type, *, use_lengths: bool
+) -> None:
+    X = np.atleast_2d(np.arange(10)).T
 
     if y_type == int:
         y = [10, 15, 10]
     elif y_type == float:
         y = [10.1, 15.2, 20.3]
     elif y_type is None:
         y = None
 
     if use_lengths:
         lengths = [2, 3, 5]
     else:
         lengths = None
         if y_type:
-            y = y[0]
+            y = y[:1]
 
-    data = SequentialDataset(X, y, lengths)
+    data = SequentialDataset(X, y, lengths=lengths)
 
     # X
-    assert_equal(data.X, np.atleast_2d(X).T)
+    helpers.assert_equal(data.X, X)
 
     # y, classes
     if y_type == int:
         assert np.issubdtype(data.y.dtype, np.integer)
-        assert_equal(data.y, np.atleast_1d(y))
-        assert_equal(data.classes, [10, 15] if lengths else [10])
+        helpers.assert_equal(data.y, np.array(y))
+        helpers.assert_equal(data.classes, [10, 15] if lengths else [10])
     elif y_type == float:
         assert np.issubdtype(data.y.dtype, np.floating)
-        assert_equal(data.y, np.atleast_1d(y))
+        helpers.assert_equal(data.y, np.array(y))
         assert data.classes is None
     elif y_type is None:
-        for prop in ('y', 'X_y', 'X_y_lengths'):
+        for prop in ("y", "X_y", "X_y_lengths"):
             with pytest.raises(AttributeError):
                 getattr(data, prop)
         assert data.classes is None
 
     # idxs
     if lengths:
-        assert_equal(
-            data.idxs, [
-                [0,  2],
-                [2,  5],
-                [5, 10]
-            ]
+        helpers.assert_equal(
+            data.idxs,
+            [
+                [0, 2],
+                [2, 5],
+                [5, 10],
+            ],
         )
     else:
-        assert_equal(data.idxs, [[0, 10]])
+        helpers.assert_equal(data.idxs, [[0, 10]])
 
-    # _iter_X
-    assert_equal(data.X, np.vstack([x for x in data._iter_X(data.X, data.idxs)]))
+    # _data.iter_X
+    helpers.assert_equal(
+        data.X,
+        np.vstack(list(_data.iter_X(data.X, idxs=data.idxs))),
+    )
 
     # __getitem__
     if y_type:
         if lengths:
             # [0]
             x, y_ = data[0]
-            assert_equal(x, np.atleast_2d([0, 1]).T)
+            helpers.assert_equal(x, np.atleast_2d([0, 1]).T)
             assert y_ == y[0]
             # [:1]
             xs, ys = data[:1]
-            assert_all_equal(xs, [np.atleast_2d([0, 1]).T])
-            assert_equal(ys, y[:1])
+            helpers.assert_all_equal(xs, [np.atleast_2d([0, 1]).T])
+            helpers.assert_equal(ys, y[:1])
             # [1:3]
             xs, ys = data[1:3]
-            assert_all_equal(xs, [
-                np.atleast_2d([2, 3, 4]).T,
-                np.atleast_2d([5, 6, 7, 8, 9]).T
-            ])
-            assert_equal(ys, y[1:3])
+            helpers.assert_all_equal(
+                xs,
+                [np.atleast_2d([2, 3, 4]).T, np.atleast_2d([5, 6, 7, 8, 9]).T],
+            )
+            helpers.assert_equal(ys, y[1:3])
             # [-1]
             x, y_ = data[-1]
-            assert_equal(x, np.atleast_2d([5, 6, 7, 8, 9]).T)
+            helpers.assert_equal(x, np.atleast_2d([5, 6, 7, 8, 9]).T)
             assert y_ == y[-1]
             # [-2:]
             xs, ys = data[-2:]
-            assert_all_equal(xs, [
-                np.atleast_2d([2, 3, 4]).T,
-                np.atleast_2d([5, 6, 7, 8, 9]).T
-            ])
-            assert_equal(ys, y[-2:])
+            helpers.assert_all_equal(
+                xs,
+                [np.atleast_2d([2, 3, 4]).T, np.atleast_2d([5, 6, 7, 8, 9]).T],
+            )
+            helpers.assert_equal(ys, y[-2:])
         else:
             # [0]
             x, y_ = data[0]
-            assert_equal(x, np.atleast_2d(X).T)
+            helpers.assert_equal(x, X)
             assert y_ == y
             # [:1]
             xs, ys = data[:1]
-            assert_all_equal(xs, [np.atleast_2d(X).T])
-            assert_equal(ys, [y])
+            helpers.assert_all_equal(xs, [X])
+            helpers.assert_equal(ys, y)
+    elif lengths:
+        # [0]
+        x = data[0]
+        helpers.assert_equal(x, np.atleast_2d([0, 1]).T)
+        # [:1]
+        xs = data[:1]
+        helpers.assert_all_equal(xs, [np.atleast_2d([0, 1]).T])
+        # [1:3]
+        xs = data[1:3]
+        helpers.assert_all_equal(
+            xs, [np.atleast_2d([2, 3, 4]).T, np.atleast_2d([5, 6, 7, 8, 9]).T]
+        )
+        # [-1]
+        x = data[-1]
+        helpers.assert_equal(x, np.atleast_2d([5, 6, 7, 8, 9]).T)
+        # [-2:]
+        xs = data[-2:]
+        helpers.assert_all_equal(
+            xs, [np.atleast_2d([2, 3, 4]).T, np.atleast_2d([5, 6, 7, 8, 9]).T]
+        )
     else:
-        if lengths:
-            # [0]
-            x = data[0]
-            assert_equal(x, np.atleast_2d([0, 1]).T)
-            # [:1]
-            xs = data[:1]
-            assert_all_equal(xs, [np.atleast_2d([0, 1]).T])
-            # [1:3]
-            xs = data[1:3]
-            assert_all_equal(xs, [
-                np.atleast_2d([2, 3, 4]).T,
-                np.atleast_2d([5, 6, 7, 8, 9]).T
-            ])
-            # [-1]
-            x = data[-1]
-            assert_equal(x, np.atleast_2d([5, 6, 7, 8, 9]).T)
-            # [-2:]
-            xs = data[-2:]
-            assert_all_equal(xs, [
-                np.atleast_2d([2, 3, 4]).T,
-                np.atleast_2d([5, 6, 7, 8, 9]).T
-            ])
-        else:
-            # [0]
-            x = data[0]
-            assert_equal(x, np.atleast_2d(X).T)
-            # [:1]
-            xs = data[:1]
-            assert_all_equal(xs, [np.atleast_2d(X).T])
+        # [0]
+        x = data[0]
+        helpers.assert_equal(x, X)
+        # [:1]
+        xs = data[:1]
+        helpers.assert_all_equal(xs, [X])
 
     # split
     if y and lengths:
-        train, test = data.split(test_size=1/3, shuffle=False)
+        train, test = data.split(test_size=1 / 3, shuffle=False)
         assert len(train) == 2
         assert len(test) == 1
-        assert_equal(train.lengths, data.lengths[:len(train)])
-        assert_equal(test.lengths, data.lengths[-len(test):])
-        assert_equal(train.X, data.X[:train.lengths.sum()])
-        assert_equal(test.X, data.X[-test.lengths.sum():])
-        assert_equal(train.y, data.y[:len(train)])
-        assert_equal(test.y, data.y[-len(test):])
+        helpers.assert_equal(train.lengths, data.lengths[: len(train)])
+        helpers.assert_equal(test.lengths, data.lengths[-len(test) :])
+        helpers.assert_equal(train.X, data.X[: train.lengths.sum()])
+        helpers.assert_equal(test.X, data.X[-test.lengths.sum() :])
+        helpers.assert_equal(train.y, data.y[: len(train)])
+        helpers.assert_equal(test.y, data.y[-len(test) :])
 
     # iter_by_class
     if y_type == int and lengths:
         for X_, lengths_, c in data.iter_by_class():
             if c == 10:
-                assert_equal(lengths_, [2, 5])
-                assert_equal(X_, np.vstack([data.X[:2], data.X[-5:]]))
+                helpers.assert_equal(lengths_, [2, 5])
+                helpers.assert_equal(X_, np.vstack([data.X[:2], data.X[-5:]]))
             elif c == 15:
-                assert_equal(lengths_, [3])
-                assert_equal(X_, data.X[2:5])
+                helpers.assert_equal(lengths_, [3])
+                helpers.assert_equal(X_, data.X[2:5])
 
     # check serialization/deserialization
-    with TemporaryDirectory() as temp_dir:
+    with tempfile.TemporaryDirectory() as temp_dir:
         data_path = f"{temp_dir}/{request.node.originalname}.npz"
         # check that save works
         data.save(data_path)
         assert os.path.isfile(data_path)
         # check that load works
         data_load = SequentialDataset.load(data_path)
         # check that stored values are the same
-        assert_equal(data._X, data_load._X)
-        assert_equal(data._lengths, data_load._lengths)
+        helpers.assert_equal(data._X, data_load._X)
+        helpers.assert_equal(data._lengths, data_load._lengths)
         if y:
-            assert_equal(data._y, data_load._y)
+            helpers.assert_equal(data._y, data_load._y)
         else:
-            assert data._y is None and data_load._y is None
+            assert data._y is None
+            assert data_load._y is None
         if data._classes is not None:
-            assert_equal(data._classes, data_load._classes)
+            helpers.assert_equal(data._classes, data_load._classes)
         else:
-            assert data._classes is None and data_load._classes is None
+            assert data._classes is None
+            assert data_load._classes is None
 
     # copy - check that stored values are the same
     data_copy = data.copy()
-    assert_equal(data._X, data_copy._X)
-    assert_equal(data._lengths, data_copy._lengths)
+    helpers.assert_equal(data._X, data_copy._X)
+    assert not np.shares_memory(data._X, data_copy._X)
+    helpers.assert_equal(data._lengths, data_copy._lengths)
+    assert not np.shares_memory(data._lengths, data_copy._lengths)
     if y:
-        assert_equal(data._y, data_copy._y)
+        helpers.assert_equal(data._y, data_copy._y)
+        assert not np.shares_memory(data._y, data_copy._y)
     else:
-        assert data._y is None and data_copy._y is None
+        assert data._y is None
+        assert data_copy._y is None
     if data._classes is not None:
-        assert_equal(data._classes, data_copy._classes)
+        helpers.assert_equal(data._classes, data_copy._classes)
+        assert not np.shares_memory(data._classes, data_copy._classes)
     else:
-        assert data._classes is None and data_copy._classes is None
+        assert data._classes is None
+        assert data_copy._classes is None
```

