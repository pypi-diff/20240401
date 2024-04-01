# Comparing `tmp/shapelets-0.2.tar.gz` & `tmp/shapelets-1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/shapelets-0.2.tar", last modified: Wed Mar 30 13:24:56 2016, max compression
+gzip compressed data, was "shapelets-1.0.tar", last modified: Mon Apr  1 12:27:47 2024, max compression
```

## Comparing `shapelets-0.2.tar` & `shapelets-1.0.tar`

### file list

```diff
@@ -1,33 +1,41 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2016-03-30 13:24:56.000000 shapelets-0.2/
--rwxrwxr-x   0 griffin   (1000) griffin   (1000)     1399 2016-03-30 13:09:42.000000 shapelets-0.2/setup.py
--rw-r--r--   0 root         (0) root         (0)      821 2016-03-30 13:24:56.000000 shapelets-0.2/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2016-03-30 13:24:56.000000 shapelets-0.2/shapelets.egg-info/
--rw-r--r--   0 root         (0) root         (0)      821 2016-03-30 13:24:56.000000 shapelets-0.2/shapelets.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)        1 2016-03-30 13:24:56.000000 shapelets-0.2/shapelets.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      620 2016-03-30 13:24:56.000000 shapelets-0.2/shapelets.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)       10 2016-03-30 13:24:56.000000 shapelets-0.2/shapelets.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2016-03-30 13:24:56.000000 shapelets-0.2/scripts/
--rwxrwxr-x   0 griffin   (1000) griffin   (1000)    20749 2016-03-30 13:15:27.000000 shapelets-0.2/scripts/fitShapelet.py
--rwxrwxr-x   0 griffin   (1000) griffin   (1000)     9766 2016-03-30 13:14:58.000000 shapelets-0.2/scripts/solveShapelet.py
--rwxrwxr-x   0 griffin   (1000) griffin   (1000)     9741 2016-03-30 13:00:36.000000 shapelets-0.2/scripts/insertShapelet.py
--rwxrwxr-x   0 griffin   (1000) griffin   (1000)     2871 2015-06-04 08:44:01.000000 shapelets-0.2/scripts/plotCoeffs.py
--rwxrwxr-x   0 griffin   (1000) griffin   (1000)     6518 2015-05-29 09:33:49.000000 shapelets-0.2/scripts/plotShapelets.py
--rwxrwxr-x   0 griffin   (1000) griffin   (1000)     1569 2015-06-01 10:44:14.000000 shapelets-0.2/scripts/plotImg.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2016-03-30 13:24:56.000000 shapelets-0.2/shapelets/
--rw-rw-r--   0 griffin   (1000) griffin   (1000)    18997 2015-06-01 12:49:06.000000 shapelets-0.2/shapelets/decomp.py
--rw-rw-r--   0 griffin   (1000) griffin   (1000)     6212 2015-06-02 14:39:57.000000 shapelets-0.2/shapelets/conv.py
--rw-rw-r--   0 griffin   (1000) griffin   (1000)     1571 2015-05-13 15:16:48.000000 shapelets-0.2/shapelets/tests.py
--rw-rw-r--   0 griffin   (1000) griffin   (1000)     9133 2015-06-01 12:18:04.000000 shapelets-0.2/shapelets/shapelet.py
--rw-rw-r--   0 griffin   (1000) griffin   (1000)    10143 2015-06-01 12:18:12.000000 shapelets-0.2/shapelets/measure.py
--rw-rw-r--   0 griffin   (1000) griffin   (1000)     6971 2015-06-01 12:10:52.000000 shapelets-0.2/shapelets/img.py
--rw-rw-r--   0 griffin   (1000) griffin   (1000)     9758 2016-03-30 13:08:23.000000 shapelets-0.2/shapelets/fileio.py
--rw-rw-r--   0 griffin   (1000) griffin   (1000)     2479 2015-05-13 15:16:48.000000 shapelets-0.2/shapelets/fshapelet.py
--rw-rw-r--   0 griffin   (1000) griffin   (1000)       97 2015-06-02 09:24:00.000000 shapelets-0.2/shapelets/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2016-03-30 13:24:56.000000 shapelets-0.2/shapelets/phs/
--rw-rw-r--   0 griffin   (1000) griffin   (1000)    20771 2016-03-30 13:01:27.000000 shapelets-0.2/shapelets/phs/ClassMS.py
--rw-rw-r--   0 griffin   (1000) griffin   (1000)     1060 2015-05-26 07:06:37.000000 shapelets-0.2/shapelets/phs/ModColor.py
--rw-rw-r--   0 griffin   (1000) griffin   (1000)      441 2015-05-26 07:06:37.000000 shapelets-0.2/shapelets/phs/rad2hmsdms.py
--rw-rw-r--   0 griffin   (1000) griffin   (1000)     1552 2016-03-30 13:02:02.000000 shapelets-0.2/shapelets/phs/ModRotate.py
--rw-rw-r--   0 griffin   (1000) griffin   (1000)      282 2015-05-26 07:06:37.000000 shapelets-0.2/shapelets/phs/reformat.py
--rw-rw-r--   0 griffin   (1000) griffin   (1000)      131 2015-05-26 07:08:32.000000 shapelets-0.2/shapelets/phs/__init__.py
--rw-r--r--   0 root         (0) root         (0)       59 2016-03-30 13:24:56.000000 shapelets-0.2/setup.cfg
+drwxrwxr-x   0 nasser    (1000) nasser    (1000)        0 2024-04-01 12:27:47.682821 shapelets-1.0/
+-rw-rw-r--   0 nasser    (1000) nasser    (1000)      121 2024-03-19 17:11:15.000000 shapelets-1.0/AUTHORS.md
+-rw-rw-r--   0 nasser    (1000) nasser    (1000)    26526 2023-03-12 20:57:22.000000 shapelets-1.0/LICENSE
+-rw-r--r--   0 nasser    (1000) nasser    (1000)    31817 2024-04-01 12:27:47.682821 shapelets-1.0/PKG-INFO
+-rw-rw-r--   0 nasser    (1000) nasser    (1000)     4281 2024-03-19 17:12:44.000000 shapelets-1.0/README.md
+-rw-rw-r--   0 nasser    (1000) nasser    (1000)       90 2023-03-12 20:58:29.000000 shapelets-1.0/pyproject.toml
+-rw-rw-r--   0 nasser    (1000) nasser    (1000)     1163 2024-04-01 12:27:47.682821 shapelets-1.0/setup.cfg
+drwxrwxr-x   0 nasser    (1000) nasser    (1000)        0 2024-04-01 12:27:47.678821 shapelets-1.0/shapelets/
+-rw-rw-r--   0 nasser    (1000) nasser    (1000)     6731 2024-04-01 12:11:51.000000 shapelets-1.0/shapelets/__init__.py
+-rw-rw-r--   0 nasser    (1000) nasser    (1000)     4345 2024-03-19 17:11:15.000000 shapelets-1.0/shapelets/_entry_points.py
+-rw-rw-r--   0 nasser    (1000) nasser    (1000)     7512 2024-03-19 17:11:15.000000 shapelets-1.0/shapelets/_run.py
+drwxrwxr-x   0 nasser    (1000) nasser    (1000)        0 2024-04-01 12:27:47.678821 shapelets-1.0/shapelets/astronomy/
+-rw-rw-r--   0 nasser    (1000) nasser    (1000)     1981 2023-11-15 23:55:24.000000 shapelets-1.0/shapelets/astronomy/__init__.py
+-rw-rw-r--   0 nasser    (1000) nasser    (1000)    12668 2024-03-19 17:11:15.000000 shapelets-1.0/shapelets/astronomy/galaxy.py
+-rw-rw-r--   0 nasser    (1000) nasser    (1000)    11847 2024-03-19 17:11:15.000000 shapelets-1.0/shapelets/astronomy/misc.py
+drwxrwxr-x   0 nasser    (1000) nasser    (1000)        0 2024-04-01 12:27:47.678821 shapelets-1.0/shapelets/discrete_transform/
+-rw-rw-r--   0 nasser    (1000) nasser    (1000)     1768 2023-03-12 21:05:17.000000 shapelets-1.0/shapelets/discrete_transform/__init__.py
+drwxrwxr-x   0 nasser    (1000) nasser    (1000)        0 2024-04-01 12:27:47.682821 shapelets-1.0/shapelets/docs/
+-rw-rw-r--   0 nasser    (1000) nasser    (1000)     4184 2024-04-01 12:11:51.000000 shapelets-1.0/shapelets/docs/WSL_support.py
+-rw-rw-r--   0 nasser    (1000) nasser    (1000)     2162 2024-04-01 12:11:51.000000 shapelets-1.0/shapelets/docs/__init__.py
+-rw-rw-r--   0 nasser    (1000) nasser    (1000)     2816 2024-04-01 12:11:51.000000 shapelets-1.0/shapelets/docs/custom_commands.py
+-rw-rw-r--   0 nasser    (1000) nasser    (1000)     7234 2024-04-01 12:11:51.000000 shapelets-1.0/shapelets/docs/example_1.py
+-rw-rw-r--   0 nasser    (1000) nasser    (1000)     7003 2024-04-01 12:11:51.000000 shapelets-1.0/shapelets/docs/example_2.py
+-rw-rw-r--   0 nasser    (1000) nasser    (1000)     6543 2024-04-01 12:11:51.000000 shapelets-1.0/shapelets/docs/example_3.py
+-rw-rw-r--   0 nasser    (1000) nasser    (1000)     7211 2024-04-01 12:11:51.000000 shapelets-1.0/shapelets/docs/example_4.py
+-rw-rw-r--   0 nasser    (1000) nasser    (1000)     4547 2024-04-01 12:11:51.000000 shapelets-1.0/shapelets/docs/installation_guide.py
+-rw-rw-r--   0 nasser    (1000) nasser    (1000)     2764 2024-04-01 12:11:51.000000 shapelets-1.0/shapelets/docs/package_interface.py
+-rw-rw-r--   0 nasser    (1000) nasser    (1000)    13422 2024-03-19 17:11:15.000000 shapelets-1.0/shapelets/functions.py
+drwxrwxr-x   0 nasser    (1000) nasser    (1000)        0 2024-04-01 12:27:47.682821 shapelets-1.0/shapelets/self_assembly/
+-rw-rw-r--   0 nasser    (1000) nasser    (1000)     2004 2023-11-15 23:55:24.000000 shapelets-1.0/shapelets/self_assembly/__init__.py
+-rw-rw-r--   0 nasser    (1000) nasser    (1000)    14659 2024-03-19 17:11:15.000000 shapelets-1.0/shapelets/self_assembly/misc.py
+-rw-rw-r--   0 nasser    (1000) nasser    (1000)    22223 2024-03-19 17:11:15.000000 shapelets-1.0/shapelets/self_assembly/quant.py
+-rw-rw-r--   0 nasser    (1000) nasser    (1000)     7638 2024-03-19 17:11:15.000000 shapelets-1.0/shapelets/self_assembly/wavelength.py
+drwxrwxr-x   0 nasser    (1000) nasser    (1000)        0 2024-04-01 12:27:47.682821 shapelets-1.0/shapelets.egg-info/
+-rw-r--r--   0 nasser    (1000) nasser    (1000)    31817 2024-04-01 12:27:47.000000 shapelets-1.0/shapelets.egg-info/PKG-INFO
+-rw-rw-r--   0 nasser    (1000) nasser    (1000)      921 2024-04-01 12:27:47.000000 shapelets-1.0/shapelets.egg-info/SOURCES.txt
+-rw-rw-r--   0 nasser    (1000) nasser    (1000)        1 2024-04-01 12:27:47.000000 shapelets-1.0/shapelets.egg-info/dependency_links.txt
+-rw-rw-r--   0 nasser    (1000) nasser    (1000)      121 2024-04-01 12:27:47.000000 shapelets-1.0/shapelets.egg-info/entry_points.txt
+-rw-rw-r--   0 nasser    (1000) nasser    (1000)        1 2024-01-09 18:39:05.000000 shapelets-1.0/shapelets.egg-info/not-zip-safe
+-rw-rw-r--   0 nasser    (1000) nasser    (1000)       97 2024-04-01 12:27:47.000000 shapelets-1.0/shapelets.egg-info/requires.txt
+-rw-rw-r--   0 nasser    (1000) nasser    (1000)       10 2024-04-01 12:27:47.000000 shapelets-1.0/shapelets.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

