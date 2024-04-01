# Comparing `tmp/plotly3d-0.1.4.tar.gz` & `tmp/plotly3d-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plotly3d-0.1.4.tar", last modified: Sun Mar 31 22:12:04 2024, max compression
+gzip compressed data, was "plotly3d-0.2.0.tar", last modified: Mon Apr  1 21:03:19 2024, max compression
```

## Comparing `plotly3d-0.1.4.tar` & `plotly3d-0.2.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 xs272    (18671) krishnaswamy_smita (10612)        0 2024-03-31 22:12:04.659549 plotly3d-0.1.4/
--rw-rw-r--   0 xs272    (18671) krishnaswamy_smita (10612)     1058 2024-03-31 02:54:34.000000 plotly3d-0.1.4/LICENSE
--rw-r--r--   0 xs272    (18671) krishnaswamy_smita (10612)      275 2024-03-31 22:12:04.658347 plotly3d-0.1.4/PKG-INFO
--rw-rw-r--   0 xs272    (18671) krishnaswamy_smita (10612)      108 2024-03-31 03:14:09.000000 plotly3d-0.1.4/README.md
-drwxrwxr-x   0 xs272    (18671) krishnaswamy_smita (10612)        0 2024-03-31 22:12:04.651625 plotly3d-0.1.4/plotly3d/
--rw-rw-r--   0 xs272    (18671) krishnaswamy_smita (10612)        0 2024-03-31 02:49:53.000000 plotly3d-0.1.4/plotly3d/__init__.py
--rw-rw-r--   0 xs272    (18671) krishnaswamy_smita (10612)     1804 2024-03-31 22:09:54.000000 plotly3d-0.1.4/plotly3d/plot.py
-drwxrwxr-x   0 xs272    (18671) krishnaswamy_smita (10612)        0 2024-03-31 22:12:04.656701 plotly3d-0.1.4/plotly3d.egg-info/
--rw-r--r--   0 xs272    (18671) krishnaswamy_smita (10612)      275 2024-03-31 22:12:04.652770 plotly3d-0.1.4/plotly3d.egg-info/PKG-INFO
--rw-rw-r--   0 xs272    (18671) krishnaswamy_smita (10612)      223 2024-03-31 22:12:04.654106 plotly3d-0.1.4/plotly3d.egg-info/SOURCES.txt
--rw-rw-r--   0 xs272    (18671) krishnaswamy_smita (10612)        1 2024-03-31 22:12:04.655374 plotly3d-0.1.4/plotly3d.egg-info/dependency_links.txt
--rw-rw-r--   0 xs272    (18671) krishnaswamy_smita (10612)       20 2024-03-31 22:12:04.656045 plotly3d-0.1.4/plotly3d.egg-info/requires.txt
--rw-rw-r--   0 xs272    (18671) krishnaswamy_smita (10612)        9 2024-03-31 22:12:04.656855 plotly3d-0.1.4/plotly3d.egg-info/top_level.txt
--rw-rw-r--   0 xs272    (18671) krishnaswamy_smita (10612)       38 2024-03-31 22:12:04.659690 plotly3d-0.1.4/setup.cfg
--rw-rw-r--   0 xs272    (18671) krishnaswamy_smita (10612)      408 2024-03-31 22:10:54.000000 plotly3d-0.1.4/setup.py
+drwxrwxr-x   0 xs272    (18671) krishnaswamy_smita (10612)        0 2024-04-01 21:03:19.755547 plotly3d-0.2.0/
+-rw-rw-r--   0 xs272    (18671) krishnaswamy_smita (10612)     1058 2024-03-31 02:54:34.000000 plotly3d-0.2.0/LICENSE
+-rw-r--r--   0 xs272    (18671) krishnaswamy_smita (10612)      267 2024-04-01 21:03:19.754708 plotly3d-0.2.0/PKG-INFO
+-rw-rw-r--   0 xs272    (18671) krishnaswamy_smita (10612)      100 2024-04-01 03:31:03.000000 plotly3d-0.2.0/README.md
+drwxrwxr-x   0 xs272    (18671) krishnaswamy_smita (10612)        0 2024-04-01 21:03:19.750902 plotly3d-0.2.0/plotly3d/
+-rw-rw-r--   0 xs272    (18671) krishnaswamy_smita (10612)        0 2024-03-31 02:49:53.000000 plotly3d-0.2.0/plotly3d/__init__.py
+-rw-rw-r--   0 xs272    (18671) krishnaswamy_smita (10612)     5478 2024-04-01 20:59:47.000000 plotly3d-0.2.0/plotly3d/plot.py
+drwxrwxr-x   0 xs272    (18671) krishnaswamy_smita (10612)        0 2024-04-01 21:03:19.753977 plotly3d-0.2.0/plotly3d.egg-info/
+-rw-r--r--   0 xs272    (18671) krishnaswamy_smita (10612)      267 2024-04-01 21:03:19.751887 plotly3d-0.2.0/plotly3d.egg-info/PKG-INFO
+-rw-rw-r--   0 xs272    (18671) krishnaswamy_smita (10612)      223 2024-04-01 21:03:19.752411 plotly3d-0.2.0/plotly3d.egg-info/SOURCES.txt
+-rw-rw-r--   0 xs272    (18671) krishnaswamy_smita (10612)        1 2024-04-01 21:03:19.752960 plotly3d-0.2.0/plotly3d.egg-info/dependency_links.txt
+-rw-rw-r--   0 xs272    (18671) krishnaswamy_smita (10612)       20 2024-04-01 21:03:19.753485 plotly3d-0.2.0/plotly3d.egg-info/requires.txt
+-rw-rw-r--   0 xs272    (18671) krishnaswamy_smita (10612)        9 2024-04-01 21:03:19.754035 plotly3d-0.2.0/plotly3d.egg-info/top_level.txt
+-rw-rw-r--   0 xs272    (18671) krishnaswamy_smita (10612)       38 2024-04-01 21:03:19.755798 plotly3d-0.2.0/setup.cfg
+-rw-rw-r--   0 xs272    (18671) krishnaswamy_smita (10612)      400 2024-04-01 03:30:58.000000 plotly3d-0.2.0/setup.py
```

### Comparing `plotly3d-0.1.4/LICENSE` & `plotly3d-0.2.0/LICENSE`

 * *Files identical despite different names*

