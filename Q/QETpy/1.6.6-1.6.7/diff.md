# Comparing `tmp/QETpy-1.6.6.tar.gz` & `tmp/QETpy-1.6.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "QETpy-1.6.6.tar", last modified: Fri Mar 29 03:35:10 2024, max compression
+gzip compressed data, was "QETpy-1.6.7.tar", last modified: Mon Apr  1 21:22:48 2024, max compression
```

## Comparing `QETpy-1.6.6.tar` & `QETpy-1.6.7.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 03:35:10.695135 QETpy-1.6.6/
--rw-r--r--   0 runner    (1001) docker     (127)    35147 2024-03-29 03:35:00.000000 QETpy-1.6.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3095 2024-03-29 03:35:10.695135 QETpy-1.6.6/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 03:35:10.695135 QETpy-1.6.6/QETpy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3095 2024-03-29 03:35:10.000000 QETpy-1.6.6/QETpy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1230 2024-03-29 03:35:10.000000 QETpy-1.6.6/QETpy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-29 03:35:10.000000 QETpy-1.6.6/QETpy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-29 03:35:10.000000 QETpy-1.6.6/QETpy.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-03-29 03:35:10.000000 QETpy-1.6.6/QETpy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-03-29 03:35:10.000000 QETpy-1.6.6/QETpy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2595 2024-03-29 03:35:00.000000 QETpy-1.6.6/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-03-29 03:35:00.000000 QETpy-1.6.6/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 03:35:10.683135 QETpy-1.6.6/qetpy/
--rw-r--r--   0 runner    (1001) docker     (127)      172 2024-03-29 03:35:00.000000 QETpy-1.6.6/qetpy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-03-29 03:35:00.000000 QETpy-1.6.6/qetpy/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 03:35:10.687135 QETpy-1.6.6/qetpy/core/
--rw-r--r--   0 runner    (1001) docker     (127)      335 2024-03-29 03:35:00.000000 QETpy-1.6.6/qetpy/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10395 2024-03-29 03:35:00.000000 QETpy-1.6.6/qetpy/core/_de_pileup.py
--rw-r--r--   0 runner    (1001) docker     (127)    87160 2024-03-29 03:35:00.000000 QETpy-1.6.6/qetpy/core/_fitting.py
--rw-r--r--   0 runner    (1001) docker     (127)    30711 2024-03-29 03:35:00.000000 QETpy-1.6.6/qetpy/core/_ibis.py
--rw-r--r--   0 runner    (1001) docker     (127)    16779 2024-03-29 03:35:00.000000 QETpy-1.6.6/qetpy/core/_iv.py
--rw-r--r--   0 runner    (1001) docker     (127)    24673 2024-03-29 03:35:00.000000 QETpy-1.6.6/qetpy/core/_noise.py
--rw-r--r--   0 runner    (1001) docker     (127)     7018 2024-03-29 03:35:00.000000 QETpy-1.6.6/qetpy/core/_of_1_chan_2_template.py
--rw-r--r--   0 runner    (1001) docker     (127)    19023 2024-03-29 03:35:00.000000 QETpy-1.6.6/qetpy/core/_of_1x1.py
--rw-r--r--   0 runner    (1001) docker     (127)    14077 2024-03-29 03:35:00.000000 QETpy-1.6.6/qetpy/core/_of_1x2.py
--rw-r--r--   0 runner    (1001) docker     (127)    37123 2024-03-29 03:35:00.000000 QETpy-1.6.6/qetpy/core/_of_base.py
--rw-r--r--   0 runner    (1001) docker     (127)    33151 2024-03-29 03:35:00.000000 QETpy-1.6.6/qetpy/core/_of_nonlin.py
--rw-r--r--   0 runner    (1001) docker     (127)    49337 2024-03-29 03:35:00.000000 QETpy-1.6.6/qetpy/core/_of_nsmb.py
--rw-r--r--   0 runner    (1001) docker     (127)     7816 2024-03-29 03:35:00.000000 QETpy-1.6.6/qetpy/core/_of_pileup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 03:35:10.691135 QETpy-1.6.6/qetpy/core/didv/
--rw-r--r--   0 runner    (1001) docker     (127)      141 2024-03-29 03:35:00.000000 QETpy-1.6.6/qetpy/core/didv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    53708 2024-03-29 03:35:00.000000 QETpy-1.6.6/qetpy/core/didv/_base_didv.py
--rw-r--r--   0 runner    (1001) docker     (127)    50469 2024-03-29 03:35:00.000000 QETpy-1.6.6/qetpy/core/didv/_didv.py
--rw-r--r--   0 runner    (1001) docker     (127)    15659 2024-03-29 03:35:00.000000 QETpy-1.6.6/qetpy/core/didv/_didv_priors.py
--rw-r--r--   0 runner    (1001) docker     (127)    27549 2024-03-29 03:35:00.000000 QETpy-1.6.6/qetpy/core/didv/_plot_didv.py
--rw-r--r--   0 runner    (1001) docker     (127)    16506 2024-03-29 03:35:00.000000 QETpy-1.6.6/qetpy/core/didv/_templates_didv.py
--rw-r--r--   0 runner    (1001) docker     (127)    57711 2024-03-29 03:35:00.000000 QETpy-1.6.6/qetpy/core/didv/_uncertainties_didv.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 03:35:10.691135 QETpy-1.6.6/qetpy/cut/
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-03-29 03:35:00.000000 QETpy-1.6.6/qetpy/cut/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    83142 2024-03-29 03:35:00.000000 QETpy-1.6.6/qetpy/cut/_cut.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 03:35:10.691135 QETpy-1.6.6/qetpy/plotting/
--rw-r--r--   0 runner    (1001) docker     (127)      155 2024-03-29 03:35:00.000000 QETpy-1.6.6/qetpy/plotting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7747 2024-03-29 03:35:00.000000 QETpy-1.6.6/qetpy/plotting/_fitting_plotting.py
--rw-r--r--   0 runner    (1001) docker     (127)    10935 2024-03-29 03:35:00.000000 QETpy-1.6.6/qetpy/plotting/_ibis_plotting.py
--rw-r--r--   0 runner    (1001) docker     (127)    10861 2024-03-29 03:35:00.000000 QETpy-1.6.6/qetpy/plotting/_iv_plotting.py
--rw-r--r--   0 runner    (1001) docker     (127)    36746 2024-03-29 03:35:00.000000 QETpy-1.6.6/qetpy/plotting/_noise_plotting.py
--rw-r--r--   0 runner    (1001) docker     (127)     5406 2024-03-29 03:35:00.000000 QETpy-1.6.6/qetpy/plotting/_of_nsmb_plotting.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 03:35:10.691135 QETpy-1.6.6/qetpy/sim/
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-03-29 03:35:00.000000 QETpy-1.6.6/qetpy/sim/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    28269 2024-03-29 03:35:00.000000 QETpy-1.6.6/qetpy/sim/_sim.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 03:35:10.691135 QETpy-1.6.6/qetpy/utils/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-03-29 03:35:00.000000 QETpy-1.6.6/qetpy/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    42912 2024-03-29 03:35:00.000000 QETpy-1.6.6/qetpy/utils/_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-29 03:35:10.695135 QETpy-1.6.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2426 2024-03-29 03:35:00.000000 QETpy-1.6.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 03:35:10.695135 QETpy-1.6.6/test/
--rw-r--r--   0 runner    (1001) docker     (127)     3212 2024-03-29 03:35:01.000000 QETpy-1.6.6/test/test_cut.py
--rw-r--r--   0 runner    (1001) docker     (127)     3926 2024-03-29 03:35:01.000000 QETpy-1.6.6/test/test_detcal.py
--rw-r--r--   0 runner    (1001) docker     (127)     4843 2024-03-29 03:35:01.000000 QETpy-1.6.6/test/test_didv.py
--rw-r--r--   0 runner    (1001) docker     (127)    10974 2024-03-29 03:35:01.000000 QETpy-1.6.6/test/test_fitting.py
--rw-r--r--   0 runner    (1001) docker     (127)     2693 2024-03-29 03:35:01.000000 QETpy-1.6.6/test/test_ibis.py
--rw-r--r--   0 runner    (1001) docker     (127)     6500 2024-03-29 03:35:01.000000 QETpy-1.6.6/test/test_ofnsmb.py
--rw-r--r--   0 runner    (1001) docker     (127)     6389 2024-03-29 03:35:01.000000 QETpy-1.6.6/test/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 21:22:48.699291 QETpy-1.6.7/
+-rw-r--r--   0 runner    (1001) docker     (127)    35147 2024-04-01 21:22:39.000000 QETpy-1.6.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3095 2024-04-01 21:22:48.699291 QETpy-1.6.7/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 21:22:48.699291 QETpy-1.6.7/QETpy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3095 2024-04-01 21:22:48.000000 QETpy-1.6.7/QETpy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1230 2024-04-01 21:22:48.000000 QETpy-1.6.7/QETpy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 21:22:48.000000 QETpy-1.6.7/QETpy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 21:22:48.000000 QETpy-1.6.7/QETpy.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-01 21:22:48.000000 QETpy-1.6.7/QETpy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-01 21:22:48.000000 QETpy-1.6.7/QETpy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2595 2024-04-01 21:22:39.000000 QETpy-1.6.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-01 21:22:40.000000 QETpy-1.6.7/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 21:22:48.691291 QETpy-1.6.7/qetpy/
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-04-01 21:22:40.000000 QETpy-1.6.7/qetpy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-01 21:22:40.000000 QETpy-1.6.7/qetpy/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 21:22:48.691291 QETpy-1.6.7/qetpy/core/
+-rw-r--r--   0 runner    (1001) docker     (127)      335 2024-04-01 21:22:40.000000 QETpy-1.6.7/qetpy/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10395 2024-04-01 21:22:40.000000 QETpy-1.6.7/qetpy/core/_de_pileup.py
+-rw-r--r--   0 runner    (1001) docker     (127)    87160 2024-04-01 21:22:40.000000 QETpy-1.6.7/qetpy/core/_fitting.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30711 2024-04-01 21:22:40.000000 QETpy-1.6.7/qetpy/core/_ibis.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16779 2024-04-01 21:22:40.000000 QETpy-1.6.7/qetpy/core/_iv.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24673 2024-04-01 21:22:40.000000 QETpy-1.6.7/qetpy/core/_noise.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7018 2024-04-01 21:22:40.000000 QETpy-1.6.7/qetpy/core/_of_1_chan_2_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19023 2024-04-01 21:22:40.000000 QETpy-1.6.7/qetpy/core/_of_1x1.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14077 2024-04-01 21:22:40.000000 QETpy-1.6.7/qetpy/core/_of_1x2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37123 2024-04-01 21:22:40.000000 QETpy-1.6.7/qetpy/core/_of_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33151 2024-04-01 21:22:40.000000 QETpy-1.6.7/qetpy/core/_of_nonlin.py
+-rw-r--r--   0 runner    (1001) docker     (127)    49337 2024-04-01 21:22:40.000000 QETpy-1.6.7/qetpy/core/_of_nsmb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7816 2024-04-01 21:22:40.000000 QETpy-1.6.7/qetpy/core/_of_pileup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 21:22:48.695291 QETpy-1.6.7/qetpy/core/didv/
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-04-01 21:22:40.000000 QETpy-1.6.7/qetpy/core/didv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    53553 2024-04-01 21:22:40.000000 QETpy-1.6.7/qetpy/core/didv/_base_didv.py
+-rw-r--r--   0 runner    (1001) docker     (127)    50353 2024-04-01 21:22:40.000000 QETpy-1.6.7/qetpy/core/didv/_didv.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15699 2024-04-01 21:22:40.000000 QETpy-1.6.7/qetpy/core/didv/_didv_priors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27771 2024-04-01 21:22:40.000000 QETpy-1.6.7/qetpy/core/didv/_plot_didv.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16506 2024-04-01 21:22:40.000000 QETpy-1.6.7/qetpy/core/didv/_templates_didv.py
+-rw-r--r--   0 runner    (1001) docker     (127)    57711 2024-04-01 21:22:40.000000 QETpy-1.6.7/qetpy/core/didv/_uncertainties_didv.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 21:22:48.695291 QETpy-1.6.7/qetpy/cut/
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-01 21:22:40.000000 QETpy-1.6.7/qetpy/cut/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    83142 2024-04-01 21:22:40.000000 QETpy-1.6.7/qetpy/cut/_cut.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 21:22:48.695291 QETpy-1.6.7/qetpy/plotting/
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2024-04-01 21:22:40.000000 QETpy-1.6.7/qetpy/plotting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7747 2024-04-01 21:22:40.000000 QETpy-1.6.7/qetpy/plotting/_fitting_plotting.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10935 2024-04-01 21:22:40.000000 QETpy-1.6.7/qetpy/plotting/_ibis_plotting.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10861 2024-04-01 21:22:40.000000 QETpy-1.6.7/qetpy/plotting/_iv_plotting.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36746 2024-04-01 21:22:40.000000 QETpy-1.6.7/qetpy/plotting/_noise_plotting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5406 2024-04-01 21:22:40.000000 QETpy-1.6.7/qetpy/plotting/_of_nsmb_plotting.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 21:22:48.695291 QETpy-1.6.7/qetpy/sim/
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-01 21:22:40.000000 QETpy-1.6.7/qetpy/sim/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28269 2024-04-01 21:22:40.000000 QETpy-1.6.7/qetpy/sim/_sim.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 21:22:48.699291 QETpy-1.6.7/qetpy/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-01 21:22:40.000000 QETpy-1.6.7/qetpy/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42909 2024-04-01 21:22:40.000000 QETpy-1.6.7/qetpy/utils/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-01 21:22:48.699291 QETpy-1.6.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2426 2024-04-01 21:22:40.000000 QETpy-1.6.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 21:22:48.699291 QETpy-1.6.7/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     3212 2024-04-01 21:22:41.000000 QETpy-1.6.7/test/test_cut.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3926 2024-04-01 21:22:41.000000 QETpy-1.6.7/test/test_detcal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3747 2024-04-01 21:22:41.000000 QETpy-1.6.7/test/test_didv.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10974 2024-04-01 21:22:41.000000 QETpy-1.6.7/test/test_fitting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2693 2024-04-01 21:22:41.000000 QETpy-1.6.7/test/test_ibis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6500 2024-04-01 21:22:41.000000 QETpy-1.6.7/test/test_ofnsmb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6389 2024-04-01 21:22:41.000000 QETpy-1.6.7/test/test_utils.py
```

### Comparing `QETpy-1.6.6/LICENSE` & `QETpy-1.6.7/LICENSE`

 * *Files identical despite different names*

### Comparing `QETpy-1.6.6/PKG-INFO` & `QETpy-1.6.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: QETpy
-Version: 1.6.6
+Version: 1.6.7
 Summary: TES Detector Calibration and Analysis Python Tools
 Home-page: https://github.com/spice-herald/QETpy
 Author: Samuel Watkins, Caleb Fink
 Author-email: samwatkins@berkeley.edu, cwfink@berkeley.edu
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
```

### Comparing `QETpy-1.6.6/QETpy.egg-info/PKG-INFO` & `QETpy-1.6.7/QETpy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: QETpy
-Version: 1.6.6
+Version: 1.6.7
 Summary: TES Detector Calibration and Analysis Python Tools
 Home-page: https://github.com/spice-herald/QETpy
 Author: Samuel Watkins, Caleb Fink
 Author-email: samwatkins@berkeley.edu, cwfink@berkeley.edu
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
```

### Comparing `QETpy-1.6.6/QETpy.egg-info/SOURCES.txt` & `QETpy-1.6.7/QETpy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `QETpy-1.6.6/README.md` & `QETpy-1.6.7/README.md`

 * *Files identical despite different names*

### Comparing `QETpy-1.6.6/qetpy/core/_de_pileup.py` & `QETpy-1.6.7/qetpy/core/_de_pileup.py`

 * *Files identical despite different names*

### Comparing `QETpy-1.6.6/qetpy/core/_fitting.py` & `QETpy-1.6.7/qetpy/core/_fitting.py`

 * *Files identical despite different names*

### Comparing `QETpy-1.6.6/qetpy/core/_ibis.py` & `QETpy-1.6.7/qetpy/core/_ibis.py`

 * *Files identical despite different names*

### Comparing `QETpy-1.6.6/qetpy/core/_iv.py` & `QETpy-1.6.7/qetpy/core/_iv.py`

 * *Files identical despite different names*

### Comparing `QETpy-1.6.6/qetpy/core/_noise.py` & `QETpy-1.6.7/qetpy/core/_noise.py`

 * *Files identical despite different names*

### Comparing `QETpy-1.6.6/qetpy/core/_of_1_chan_2_template.py` & `QETpy-1.6.7/qetpy/core/_of_1_chan_2_template.py`

 * *Files identical despite different names*

### Comparing `QETpy-1.6.6/qetpy/core/_of_1x1.py` & `QETpy-1.6.7/qetpy/core/_of_1x1.py`

 * *Files identical despite different names*

### Comparing `QETpy-1.6.6/qetpy/core/_of_1x2.py` & `QETpy-1.6.7/qetpy/core/_of_1x2.py`

 * *Files identical despite different names*

### Comparing `QETpy-1.6.6/qetpy/core/_of_base.py` & `QETpy-1.6.7/qetpy/core/_of_base.py`

 * *Files identical despite different names*

### Comparing `QETpy-1.6.6/qetpy/core/_of_nonlin.py` & `QETpy-1.6.7/qetpy/core/_of_nonlin.py`

 * *Files identical despite different names*

### Comparing `QETpy-1.6.6/qetpy/core/_of_nsmb.py` & `QETpy-1.6.7/qetpy/core/_of_nsmb.py`

 * *Files identical despite different names*

### Comparing `QETpy-1.6.6/qetpy/core/_of_pileup.py` & `QETpy-1.6.7/qetpy/core/_of_pileup.py`

 * *Files identical despite different names*

### Comparing `QETpy-1.6.6/qetpy/core/didv/_base_didv.py` & `QETpy-1.6.7/qetpy/core/didv/_base_didv.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import warnings
 import numpy as np
 from numpy import pi
 from scipy.optimize import least_squares, fsolve
 from qetpy.utils import fft, ifft, fftfreq, rfftfreq
 from qetpy.utils import resample_data
-
+import copy
 
 __all__ = [
     "stdcomplex",
     "compleximpedance",
     "complexadmittance",
     "squarewaveresponse",
     "get_i0",
@@ -458,15 +458,14 @@
         else:
             raise ValueError('ERROR: i0 variable offset not found in '
                              '"ivsweep_result" dictionary!')
 
         # current IV variable offset
         if lgc_calibration_on is False:
             i0_variable_offset = output_offset * output_gain/closed_loop_norm
-            
         else:
             if calibration_dict is None:
                 raise ValueError('ERROR: must include calibration_dict if '
                                  'lgc_calibration_on is True (i.e. being used)!'
                                  'Check offset dicts')
                                  
             elif (output_gain != 50):
@@ -788,27 +787,24 @@
         'rl': rl,
         'ibias': ibias,
         'rn': rn,
     }
     
     return bias_parameter_dict
     
-def get_tes_bias_parameters_dict_infinite_loop_gain(poles, params, cov,
+def get_tes_bias_parameters_dict_infinite_loop_gain(params, cov,
                                                     ibias, ibias_err,
                                                     rsh, rp, rn=None):
     """
     Gets and returns a dictonary of i0, v0, r0, and p0 with uncertainties
     using the infinte loop gain approximation
     
     Parameters
     ----------
-    
-    poles : int 
-        the number of poles of the dIdV fit
-
+  
     params : dict
         The parameters (A, B, tau_1, etc.) of the previous dIdV fit.
                
     cov : matrix
         The covariance matrix for the params, starting with the A, B
         components.
         
@@ -829,24 +825,28 @@
     -------
     bias_parameters_dict : dict
         A dictonary of bias parameters and uncertainties, including i0, r0,
         v0, and p0
         
     """
 
-    if (poles !=2 and poles !=3):
-        raise ValueError('ERROR: Number of poles should be 2 or 3!')
-
+    # check dimension
+    num_params = cov.shape[0]
+    if len(params.keys()) != num_params:
+        raise ValueError('ERROR: inconsistent number of '
+                         'parameters with covariance '
+                         'matrix shape')
+    
     # Rload
     rl = rp + rsh
 
     # r0
     dvdi0 = None
     r0_jac = None
-    if poles == 2:
+    if num_params == 5:
         dvdi0 =  params['A'] +  params['B']
         r0_jac = np.asarray([1, 1, 0, 0, 0])
     else:
         dvdi0 =  params['A'] + params['B']/(1-params['C'])
         r0_jac = np.asarray([1, 1, 1, 0, 0, 0, 0])
         
     r0 = abs(dvdi0) + rl
@@ -854,20 +854,18 @@
     
     i0 = ibias * rsh / (r0 + rl)
     i0_err = ((ibias_err * rsh / (r0 + rl))**2 + (r0_err * ibias * rsh * (rl + r0)**-2)**2)**0.5
     
     
     v0, v0_err = _get_v0(i0, i0_err, ibias, ibias_err, rsh, rp)
     p0, p0_err = _get_p0(i0, i0_err, v0, v0_err)
-
     
     if rn is None:
         rn = np.nan
-
-    
+ 
     bias_parameter_dict = {
         'i0': i0,
         'i0_err': i0_err,
         'v0': v0,
         'v0_err': v0_err,
         'r0': r0,
         'r0_err': r0_err,
@@ -997,19 +995,19 @@
         self._tmean = None
         self._zeroinds = None
         self._didvstd = None
         self._didvmean = None
         self._offset = None
         self._offset_err = None
 
-        self._1poleresult = None
-        self._2poleresult = None
-        self._3poleresult = None
-
 
+        # container to store all the results
+        # key = model poles (1, 2, 3) 
+        self._fit_results = {1:None, 2:None, 3:None}
+        
     @staticmethod
     def _onepoleimpedance(freq, A, tau2):
         """
         Function to calculate the impedance (dvdi) of a TES with the
         1-pole fit.
 
         """
@@ -1439,16 +1437,20 @@
             taup, taum, taun = fsolve(threepoleequations, (tau1, tau2, tau3))
             falltimes = np.array([taup, taum, taun])
 
         else:
             print("Wrong number of input parameters, returning zero...")
             falltimes = np.zeros(1)
 
-        # return fall times sorted from shortest to longest
-        return np.sort(falltimes)
+        # fall times sorted from shortest to longest
+        falltimes = np.sort(falltimes)
+        if falltimes[0] == 0:
+            falltimes = np.concatenate((falltimes[1:], [0]))
+
+        return falltimes
 
 
     def processtraces(self):
         """
         This method processes the traces loaded to the DIDV class
         object. This sets up the object for fitting.
 
@@ -1519,15 +1521,15 @@
                 self._sgamp,
                 self._sgfreq,
                 self._dutycycle,
             )[1]
             didvs.append(didvi)
 
         #convert to numpy structure
-        didvs=np.array(didvs)
+        didvs = np.array(didvs)
 
         # get rid of any NaNs, as these will break the fit 
         cut = np.logical_not(np.isnan(didvs).any(axis=1))
 
         self._traces = self._traces[cut]
         didvs = didvs[cut]
 
@@ -1558,69 +1560,50 @@
 
     def get_list_fitted_poles(self):
         """
         Function to return a list of poles that 
         have been fitted
 
         """
-
-        list_of_poles = []
-        if self._1poleresult is not None:
-            list_of_poles.append(1)
-        if self._2poleresult is not None:
-            list_of_poles.append(2)
-        if self._3poleresult is not None:
-            list_of_poles.append(3)
-
+        keys = list(self._fit_results.keys())
+        list_of_poles = list()
+        for poles in keys:
+            if self._fit_results[poles] is not None:
+                list_of_poles.append(poles)
+                
         return list_of_poles 
 
         
-    def fitresult(self, poles):
+    def fitresult(self, poles=None):
         """
         Function for returning a dictionary containing the relevant
         results from the specified fit.
 
         Parameters
         ----------
-        poles : int
+        poles : int, optional
             The number of poles (fall times) in the fit, from which the
             results will be returned. Should be 1, 2, or 3.
+            if None, return all models (dictionary with keys = poles)
 
         Returns
         -------
         result : dict
             A dictionary containing the fitted parameters, the error of
             each parameter (from the diagonal of the covariance
             matrix), the full covariance matrix, the physical fall
             times, and the cost (i.e. chi-square) of the fit.
 
         """
 
-        if poles == 1:
-            if self._1poleresult is None:
-                warnings.warn(
-                    "The 1-pole fit has not been run, "
-                    "returning an empty dict."
-                )
-                return dict()
-
-            return self._1poleresult
-
-        if poles == 2:
-            if self._2poleresult is None:
-                warnings.warn(
-                    "The 2-pole fit has not been run, "
-                    "returning an empty dict."
-                )
-                return dict()
-
-            return self._2poleresult
-
-        if poles == 3:
-            if self._3poleresult is None:
+        if poles is None:
+            return copy.deepcopy(self._fit_results)
+        else:
+            if poles not in self._fit_results:
                 warnings.warn(
-                    "The 3-pole fit has not been run, "
-                    "returning an empty dict."
+                    f'The {poles}-pole fit has not been run, '
+                    f'returning an empty dict.'
                 )
                 return dict()
-
-            return self._3poleresult
+            else :
+                return copy.deepcopy(self._fit_results[poles])
+
```

### Comparing `QETpy-1.6.6/qetpy/core/didv/_didv.py` & `QETpy-1.6.7/qetpy/core/didv/_didv.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 import numpy as np
 from scipy.optimize import least_squares, fsolve
 from ._base_didv import _BaseDIDV, complexadmittance, get_i0, get_ibias
 from ._base_didv import get_tes_bias_parameters_dict, get_tes_bias_parameters_dict_infinite_loop_gain
 from ._plot_didv import _PlotDIDV
 from ._uncertainties_didv import get_smallsignalparams_cov, get_smallsignalparams_sigmas
 from qetpy.utils import fft, ifft, fftfreq, rfftfreq
+import copy
+import warnings
+warnings.simplefilter('default')
 
 
 __all__ = [
     "didvinitfromdata",
     "DIDV",
 ]
 
@@ -565,26 +568,26 @@
             # Convert to didv falltimes
             falltimes1 = DIDV._findpolefalltimes(fitparams1)
 
             # cost: divide by NDOF
             fitcost1 /= (np.sum(fit_freqs)-len(fitparams1))
             
             # store as dictionary
-            self._1poleresult = DIDV._fitresult(
+            self._fit_results[1] = DIDV._fitresult(
                 poles,
                 fitparams1,
                 fitcov1,
                 falltimes1,
                 fitcost1,
                 lgcfix=lgcfix,
             )
 
             # store offset 
-            self._1poleresult['offset'] = self._offset
-            self._1poleresult['offset_err'] = self._offset_err
+            self._fit_results[1]['offset'] = self._offset
+            self._fit_results[1]['offset_err'] = self._offset_err
 
             # calculate small signal parameters
             # (lgc_ssp_light only used for 3-poles)
             self._calc_ssp(1)
             
             
 
@@ -618,21 +621,18 @@
                 if intau10 is not None:
                     tau10 = intau10
                 if intau20 is not None:
                     tau20 = intau20
                 if indt is not None:
                     dt0 = indt
 
-
             # loopgainsub1   
             if guess_isloopgainsub1 is not None:
                 isloopgainsub1 = guess_isloopgainsub1
-                
-                
-
+       
             # 2 pole fitting
             fitparams2, fitcov2, fitcost2 = DIDV._fitdidv(
                 self._freq[fit_freqs],
                 self._didvmean[fit_freqs],
                 yerr=self._didvstd[fit_freqs],
                 A0=A0,
                 B0=B0,
@@ -649,39 +649,69 @@
                 loss=loss,
                 ftol=ftol,
                 xtol=xtol,
             )
 
             # cost: divide by NDOF
             fitcost2 = fitcost2/(np.sum(fit_freqs)-len(fitparams2))
-           
+
+            # Convert to a 3-pole model with  C=0  and tau3=0
+
+            # 1)  fit parameters
+            indices = [2, 4]
+            fitparams2 = np.insert(fitparams2, [2,4], 0)
+            
+            if lgcfix is not None:
+                if isinstance(lgcfix, list):
+                    lgcfix.insert(2, True)
+                    lgcfix.insert(5, True)
+                elif isinstance(lgcfix, np.ndarray):
+                    lgcfix = np.insert(lgcfix, [2,4], 0)
+                    
+            # 2) cov
+                
+            # Insert a row of zeros at index 2
+            intermediate_cov2 = np.insert(fitcov2, 2, 0, axis=0)
+            # Insert a column of zeros at index 2
+            intermediate_cov2 = np.insert(intermediate_cov2, 2, 0, axis=1) 
+
+            # For tau3, insert zeros at index 5
+            # Now index 5 for rows
+            final_cov2 = np.insert(intermediate_cov2, 5, 0, axis=0)
+            # And index 5 for columns
+            final_cov2 = np.insert(final_cov2, 5, 0, axis=1) 
+
+
             # Convert to didv falltimes
             falltimes2 = DIDV._findpolefalltimes(fitparams2)
-
+                     
             # store as dictionary
-            self._2poleresult = DIDV._fitresult(
+            self._fit_results[2] = DIDV._fitresult(
                 poles,
                 fitparams2,
-                fitcov2,
+                final_cov2,
                 falltimes2,
                 fitcost2,
                 lgcfix=lgcfix)
 
             # store a few more parameters
-            self._2poleresult['offset'] = self._offset
-            self._2poleresult['offset_err'] = self._offset_err
+            self._fit_results[2]['offset'] = self._offset
+            self._fit_results[2]['offset_err'] = self._offset_err
 
             # calculate small signal parameter
             # (lgc_ssp_light only used for 3-poles)
-            self._calc_ssp(2)
-                            
+            self._calc_ssp(2,
+                           biasparams_dict=biasparams_dict,
+                           lgc_ssp_light=lgc_ssp_light)
 
         elif poles==3:
-            
-            if self._2poleresult is None:
+
+            if (self._fit_results[2] is None
+                or 'param' not in self._fit_results[2]):
+                
                 # Guess the 3-pole fit starting parameters from
                 # 2-pole fit guess
                 A0, B0, tau10, tau20 = DIDV._guessdidvparams(
                     self._tmean,
                     self._tmean[self._flatinds],
                     self._sgamp,
                     self._rsh,
@@ -690,21 +720,21 @@
                 B0 = -abs(B0)
                 C0 = -0.05
                 tau10 = -abs(tau10)
                 tau30 = 1.0e-3
                 dt0 = self._dt0
                 
             else:
-                A0 = self._2poleresult['params']['A']
-                B0 = -abs(self._2poleresult['params']['B'])
+                A0 = self._fit_results[2]['params']['A']
+                B0 = -abs(self._fit_results[2]['params']['B'])
                 C0 = -0.05
-                tau10 = -abs(self._2poleresult['params']['tau1']) 
-                tau20 = self._2poleresult['params']['tau2']
+                tau10 = -abs(self._fit_results[2]['params']['tau1']) 
+                tau20 = self._fit_results[2]['params']['tau2']
                 tau30 = 1.0e-3
-                dt0 = self._2poleresult['params']['dt']
+                dt0 = self._fit_results[2]['params']['dt']
 
 
             # is loop gain < 1
             isloopgainsub1 = DIDV._guessdidvparams(
                 self._tmean,
                 self._tmean[self._flatinds],
                 self._sgamp,
@@ -731,20 +761,17 @@
                 if intau20 is not None:
                     tau20 = intau20
                 if intau30 is not None:
                     tau30 = intau30 
                 if indt is not None:
                     dt0 = indt
 
-
             # loopgainsub1   
             if guess_isloopgainsub1 is not None:
                 isloopgainsub1 = guess_isloopgainsub1
-
-
             
             # 3 pole fitting
             fitparams3, fitcov3, fitcost3 = DIDV._fitdidv(
                 self._freq[fit_freqs],
                 self._didvmean[fit_freqs],
                 yerr=self._didvstd[fit_freqs],
                 A0=A0,
@@ -765,72 +792,86 @@
                 ftol=ftol,
                 xtol=xtol,
             )
 
             # cost: divide by NDOF
             fitcost3 = fitcost3/(np.sum(fit_freqs)-len(fitparams3))
             
-
-            
             # Convert to didv falltimes
             falltimes3 = DIDV._findpolefalltimes(fitparams3)
 
-            self._3poleresult = DIDV._fitresult(
+            # store results
+            self._fit_results[3] = DIDV._fitresult(
                 poles,
                 fitparams3,
                 fitcov3,
                 falltimes3,
                 fitcost3,
                 lgcfix=lgcfix,
             )
 
-             # store offset 
-            self._3poleresult['offset'] = self._offset
-            self._3poleresult['offset_err'] = self._offset_err
-
+            # store offset 
+            self._fit_results[3]['offset'] = self._offset
+            self._fit_results[3]['offset_err'] = self._offset_err
+            
             # small signal parameters
             self._calc_ssp(
                 3,
                 biasparams_dict=biasparams_dict,
                 lgc_ssp_light=lgc_ssp_light
             )
 
         else:
             raise ValueError("The number of poles should be 1, 2, or 3.")
 
 
     def calc_smallsignal_params(self, ivsweep_results,
+                                poles=None,
                                 calc_true_current=False,
                                 tes_bias=None,
                                 close_loop_norm=None,
                                 output_variable_gain=None,
                                 output_variable_offset=None,
                                 inf_loop_gain_approx='auto',
                                 lgc_verbose=True,
                                 lgc_diagnostics=False):
         """
         Calculate small signal parametres and their uncertainties 
-        using results from  ivsweep.  If calc_true_current=True, 
-        I0 is recalculated using the measured offset  
+        using results from  ivsweep (I0 or Ioffset).  
+        If calc_true_current=True, I0 is recalculated using the measured offset  
         """
 
-        
-        # 3 poles
-        calc_3poles = False
-        if self._3poleresult is not None:
-            if  'params' not in  self._3poleresult.keys():
-                raise ValueError(f'ERROR: 3-poles fit needs to be done first!')
-            calc_3poles = True
-        
-        calc_2poles = False
-        if self._2poleresult is not None:
-            if  'params' not in  self._2poleresult.keys():
-                raise ValueError(f'ERROR: 2-poles fit needs to be done first!')
-            calc_2poles = True
-        
+        # check which models have been fitted (2 and/or 3 poles)
+        model_list  = list()
+
+        if poles is not None:
+            if (self._fit_results[poles] is None
+                or 'params' not in  self._fit_results[poles]):
+                raise ValueError(f'ERROR: {poles}-poles fit needs to be done first!')
+            else:
+                model_list.append(poles)
+        else:
+            if self._fit_results[2] is not None:
+                if  'params' not in  self._fit_results[2]:
+                    raise ValueError(f'ERROR: 2-poles fit needs to be done first!')
+                else:
+                    model_list.append(2)
+              
+            if self._fit_results[3] is not None:
+                if  'params' not in self._fit_results[3]:
+                    raise ValueError(f'ERROR: 3-poles fit needs to be done first!')
+                else:
+                    model_list.append(3)
+
+        if not model_list:
+            print('WARNING: No fit have been done. Doing nothing...')
+            return
+                
+
+        # True bias calculation
         
         # check ivsweep results and convert to dictionary
         if not isinstance(ivsweep_results, dict):
             raise ValueError(f'ERROR: "ivsweep_results" should be a dictionary!')
         
         required_parameters = ['rp']
         if calc_true_current:
@@ -854,16 +895,14 @@
                                  '"ivsweep_results" dictionary!')
 
             # tes bias
             if tes_bias is None:
                 raise ValueError(f'ERROR: "tes_bias" parameter (QET bias) '
                                  'required when calculating true current')
 
-
-
         # initialize  bias parameters dict
         biasparams_dict = ivsweep_results.copy()
         biasparams_dict['biasparams_type'] = 'external_current'
         
         rp = ivsweep_results['rp']
         rn = None
         if 'rn' in  ivsweep_results:
@@ -890,15 +929,15 @@
             i0, i0_err = get_i0(self._offset, self._offset_err,
                                 ivsweep_results,
                                 output_variable_offset,
                                 close_loop_norm,
                                 output_variable_gain,
                                 lgc_invert_offset=lgc_invert_offset,
                                 lgc_diagnostics=lgc_diagnostics)
-    
+
             # calculate true ibias (QET bias)
             ibias, ibias_err = get_ibias(tes_bias, ivsweep_results,
                                          lgc_diagnostics=lgc_diagnostics)
 
         
             # recalculate v0, r0 with true current and store in dictionary
             biasparams_dict = get_tes_bias_parameters_dict(
@@ -907,180 +946,147 @@
             
             biasparams_dict['biasparams_type'] = 'true_current'
        
         self._r0 = biasparams_dict['r0']
         self._rp = biasparams_dict['rp']
 
 
-        # calculate small signal parameters with proper bias parameters
-        if calc_2poles:
-            self._calc_ssp(2,
-                           biasparams_dict=biasparams_dict.copy(),
-                           lgc_ssp_light=False)
+        # calculate small signal parameters
+        
+        # loop poles
+        for model_poles in model_list:
 
-        if calc_3poles:
-            self._calc_ssp(3,
+            print(f'INFO: Calculating small signal parameters '
+                  f'for {model_poles}-poles model ')
+            
+            # calc
+            self._calc_ssp(model_poles,
                            biasparams_dict=biasparams_dict.copy(),
                            lgc_ssp_light=True)
-
-
-        # Check if infinite loop gain needs to be done
-        # if inf_loop_gain_approx == 'auto' AND lopp gain negative
-        #     -> automatically make approximation that loop gain infinite 
             
+            # Check if infinite loop gain needs to be done
+            # if inf_loop_gain_approx == 'auto' AND lopp gain negative
+            #     -> automatically make approximation that loop gain infinite 
 
-        # 2-poles
-        if calc_2poles:
-
+            results = copy.deepcopy(self._fit_results[model_poles])
+                            
             # check if infinite loop gain needs to be done
             set_infinite_loop_gain = inf_loop_gain_approx
             if inf_loop_gain_approx == 'auto':
                 
-                if self._2poleresult['smallsignalparams']['l'] < 0:
+                if results['smallsignalparams']['l'] < 0:
                     if lgc_verbose:
-                        print('INFO: Loop gain is negative for 2-poles fit. '
-                              'Will use infinite loop gain approximation!')
+                        print(f'INFO: Loop gain is negative '
+                              f'for {model_poles}-poles fit. Will '
+                              f'use infinite loop gain approximation!')
+                        
                     set_infinite_loop_gain = True
                 else:
                     set_infinite_loop_gain = False
                     
             if set_infinite_loop_gain:
 
                 if lgc_verbose:
-                    print('INFO: Calculating bias parameters with infinite loop gain '
-                          'approximation for 2-poles fit!')
-                                
-                params =  self._2poleresult['params']
-                cov =  self._2poleresult['cov']
+                    print(f'INFO: Calculating bias parameters '
+                          f'with infinite loop gain approximation '
+                          f'for {model_poles}-poles fit!')
 
-                biasparams_dict_2poles = get_tes_bias_parameters_dict_infinite_loop_gain(
-                    2, params, cov, ibias, ibias_err, self._rsh, rp, rn=rn
+                params =  results['params']
+                cov =  results['cov']
+                
+                biasparams_dict_inf = get_tes_bias_parameters_dict_infinite_loop_gain(
+                    params, cov, ibias, ibias_err, self._rsh, rp, rn=rn
                 )
 
-                biasparams_dict_2poles['biasparams_type'] = 'infinite_lgain_current'
+                biasparams_dict_inf['biasparams_type'] = 'infinite_lgain_current'
                 
-                # re-assign r0
-                self._r0 = biasparams_dict_2poles['r0']
+                # re-assign r0 
+                self._r0 = biasparams_dict_inf['r0']
 
                 # re-calculate small signal parameters
                 # with proper bias paramaters
-                self._calc_ssp(2,
-                               biasparams_dict=biasparams_dict_2poles,
-                               lgc_ssp_light=False)
-
-        # 3-poles
-        if calc_3poles:
-            
-            # check if infinite loop gain needs to be done
-            set_infinite_loop_gain = inf_loop_gain_approx
-            if inf_loop_gain_approx == 'auto':
-                
-                if self._3poleresult['smallsignalparams']['l'] < 0:
-                    if lgc_verbose:
-                        print('INFO: Loop gain is negative for 3-poles fit. '
-                              'Will use infinite loop gain approximation!')
-                    set_infinite_loop_gain = True
-                else:
-                    set_infinite_loop_gain = False
-                    
-            if set_infinite_loop_gain:
-                
-                if lgc_verbose:
-                    print('INFO: Calculating bias parameters with infinite loop gain '
-                          'approximation for 3-poles fit!')
-                
-                
-                params =  self._3poleresult['params']
-                cov =  self._3poleresult['cov']
-
-                biasparams_dict_3poles = get_tes_bias_parameters_dict_infinite_loop_gain(
-                    3, params, cov, ibias, ibias_err, self._rsh, rp, rn=rn
-                )
-                
-                biasparams_dict_3poles['biasparams_type'] = 'infinite_lgain_current'
-                
-                # re-assign r0 (overwrite 2-poles)
-                self._r0 = biasparams_dict_3poles['r0']
-
-                # calculate small signal parameters
-                # with proper bias paramaters
-                self._calc_ssp(3,
-                               biasparams_dict=biasparams_dict_3poles,
+                self._calc_ssp(model_poles,
+                               biasparams_dict=biasparams_dict_inf,
                                lgc_ssp_light=True)
-
                 
-
-
         
-    def calc_bias_params_infinite_loop_gain(self, poles=3,
+    def calc_bias_params_infinite_loop_gain(self, poles=None,
                                             tes_bias=None,
                                             tes_bias_err=0,
                                             rp=None):
         """
         Calculate I0,R0,V0, P0 with infinite loop gain 
         approximation and store in fit result
         """
 
+        model_list  = list()
 
-        # get fit results
-        if poles == 2:
-            if self._2poleresult is None:
-                raise ValueError(
-                    'ERROR: The 2-pole fit has not been run'
-                )
-            results = self._2poleresult
+        if poles is not None:
+            if (self._fit_results[poles] is None
+                or 'params' not in  self._fit_results[poles]):
+                raise ValueError(f'ERROR: {poles}-poles fit needs to be done first!')
+            else:
+                model_list.append(poles)
+        else:
+            if self._fit_results[2] is not None:
+                if  'params' not in  self._fit_results[2]:
+                    raise ValueError(f'ERROR: 2-poles fit needs to be done first!')
+                else:
+                    model_list.append(2)
+              
+            if self._fit_results[3] is not None:
+                if  'params' not in self._fit_results[3]:
+                    raise ValueError(f'ERROR: 3-poles fit needs to be done first!')
+                else:
+                    model_list.append(3)
+                    
+        if not model_list:
+            print('WARNING: No fit have been done. Doing nothing...')
+            return
+        
+        # loop poles
+        for model_poles in model_list:
             
-        elif  poles == 3:
-            if self._3poleresult is None:
-                raise ValueError(
-                    'ERROR: The 2-pole fit has not been run'
-                )
-            results = self._3poleresult
-
-
-        # check if ibias available
-        if tes_bias is None:
+            results = copy.deepcopy(self._fit_results[model_poles])
+            
+            # check if ibias available
+            if tes_bias is None:
 
-            if ('biasparams' not in results.keys()
-                or 'ibias' not in results['biasparams']):
-                raise ValueError(
-                    'ERROR: Unable to find tes bias (ibias)!'
-                    ' It needs to be provided.'
-                )
+                if ('biasparams' not in results.keys()
+                    or 'ibias' not in results['biasparams']):
+                    raise ValueError(
+                        'ERROR: Unable to find tes bias (ibias)!'
+                        ' It needs to be provided.'
+                    )
             
-            tes_bias = results['biasparams']['ibias']
-            if 'ibias_err' in results['biasparams']:
-                tes_bias_err = results['biasparams']['ibias_err']
+                tes_bias = results['biasparams']['ibias']
+                if 'ibias_err' in results['biasparams']:
+                    tes_bias_err = results['biasparams']['ibias_err']
           
 
-        # Rp
-        if rp is None:
-            if self._rp is None:
-                raise ValueError(
-                    'ERROR: Unable to find rp!'
-                    ' It needs to be provided.'
-                )
-            rp = self._rp
+            # Rp
+            if rp is None:
+                if self._rp is None:
+                    raise ValueError(
+                        'ERROR: Unable to find rp!'
+                        ' It needs to be provided.'
+                    )
+                rp = self._rp
 
             
-        results['biasparams_infinite_lgain'] = (
-            get_tes_bias_parameters_dict_infinite_loop_gain(
-                poles,
-                results['params'], results['cov'],
-                tes_bias, tes_bias_err,
-                self._rsh, rp
+            results['biasparams_infinite_lgain'] = (
+                get_tes_bias_parameters_dict_infinite_loop_gain(
+                    results['params'], results['cov'],
+                    tes_bias, tes_bias_err,
+                    self._rsh, rp
+                )
             )
-        )
-            
-        # replace results
-        if poles == 2:
-            self._2poleresult  = results
-        elif  poles == 3:
-            self._3poleresult = results
-                      
+
+            self._fit_results[model_poles] = results
+                                  
     def dofit_with_true_current(self, offset_dict,
                                 output_offset, closed_loop_norm, output_gain,
                                 ibias_metadata,
                                 bounds=None, guess=None,
                                 inf_loop_gain_approx=False,
                                 inf_loop_gain_limit=False,
                                 lgc_calibration_on=False,
@@ -1142,14 +1148,19 @@
             
         result3: fitresult_dict
             3 pole fit result with biasparams calculated, and the smallsignalparams
             correctly calculated from the r0 calculated for the biasparams
         
         """
 
+        warnings.warn(
+            'WARNING: "dofit_with_true_current(..)" function is deprecated. '
+            'Use "calc_smallsignal_params(.., calc_true_current=True,...)" '
+            'instead.')
+  
         self._rp = offset_dict['rp']
 
         rsh = self._rsh
         rp = self._rp
 
         offset = self._offset
         offset_err = self._offset_err
@@ -1162,31 +1173,33 @@
         i0, i0_err = get_i0(offset, offset_err, offset_dict, output_offset,
                             closed_loop_norm, output_gain, lgc_diagnostics=lgcdiagnostics,
                             lgc_calibration_on=lgc_calibration_on, calibration_dict=calibration_dict)
         ibias, ibias_err = get_ibias(ibias_metadata, offset_dict, lgc_diagnostics=lgcdiagnostics)
         biasparams_dict = get_tes_bias_parameters_dict(i0, i0_err, ibias, ibias_err, rsh, rp)
         
         if inf_loop_gain_approx:
-            biasparams_dict = get_tes_bias_parameters_dict_infinite_loop_gain(3, 
-                self._3poleresult['params'], self._3poleresult['cov'],
-                ibias, ibias_err, rsh, rp)
+            biasparams_dict = get_tes_bias_parameters_dict_infinite_loop_gain( 
+                self._fit_results[3]['params'], self._fit_results[3]['cov'],
+                ibias, ibias_err, rsh, rp
+            )
         
         self._r0 = biasparams_dict['r0']
 
         result3 = self.dofit(3, bounds=bounds, guess_params=guess,
                              biasparams_dict=biasparams_dict,
                              lgc_ssp_light=True)
                              
         if inf_loop_gain_limit:
-            if self._3poleresult['smallsignalparams']['l'] < 0:
-                biasparams_dict = get_tes_bias_parameters_dict_infinite_loop_gain(3, 
-                    self._3poleresult['params'], 
-                    self._3poleresult['cov'], i0, 
+            if self._fit_results[3]['smallsignalparams']['l'] < 0:
+                biasparams_dict = get_tes_bias_parameters_dict_infinite_loop_gain( 
+                    self._fit_results[3]['params'], 
+                    self._fit_results[3]['cov'], i0, 
                     i0_err, ibias, ibias_err, 
                     rsh, rp)
+                
                 result3 = self.dofit(3, bounds=bounds,
                                      guess_params=guess,
                                      biasparams_dict=biasparams_dict,
                                      lgc_ssp_light=True)
                              
         return result3
     
@@ -1221,54 +1234,38 @@
             result['cov'] = cov
             result['errors'] = {
                 'A': errors[0],
                 'tau2': errors[1],
                 'dt': errors[2],
             }
 
-        if poles == 2:
-            result['params'] = {
-                'A': params[0],
-                'B': params[1],
-                'tau1': params[2],
-                'tau2': params[3],
-                'dt': params[4],
-            }
-            
-            result['cov'] = cov
-            result['errors'] = {
-                'A': errors[0],
-                'B': errors[1],
-                'tau1': errors[2],
-                'tau2': errors[3],
-                'dt': errors[4],
-            }
+        elif (poles == 2 or poles == 3):
 
-        if poles == 3:
             result['params'] = {
                 'A': params[0],
                 'B': params[1],
                 'C': params[2],
                 'tau1': params[3],
                 'tau2': params[4],
                 'tau3': params[5],
                 'dt': params[6],
             }
+            
             result['cov'] = cov
+            
             result['errors'] = {
                 'A': errors[0],
                 'B': errors[1],
                 'C': errors[2],
                 'tau1': errors[3],
                 'tau2': errors[4],
                 'tau3': errors[5],
                 'dt': errors[6],
             }
 
-          
         # other params
         result['falltimes'] = falltimes
         result['cost'] = cost
       
         return result
 
     
@@ -1289,134 +1286,112 @@
                 self._rp = biasparams_dict['rp']
             
 
         
         # 1-poles fit 
         if poles == 1:
             
-            if self._1poleresult is None:
+            if self._fit_results[1] is None:
                 raise ValueError(
                     'ERROR: No 1-poles fit done! Unable to '
                     'calculate small signal parameters ')
             
             smallsignalparams = DIDV._converttotesvalues(
-                self._1poleresult['params_array'],
+                self._fit_results[1]['params_array'],
                 self._rsh, self._r0, self._rp
             )
 
-            self._1poleresult['smallsignalparams'] = {
+            self._fit_results[1]['smallsignalparams'] = {
                 'rsh': smallsignalparams[0],
                 'rp': smallsignalparams[1],
                 'L': smallsignalparams[2],
                 'dt': smallsignalparams[3],
             }
             
-            self._1poleresult['didv0'] = (
-                complexadmittance(0, **self._1poleresult['smallsignalparams']).real
+            self._fit_results[1]['didv0'] = (
+                complexadmittance(0, **self._fit_results[1]['smallsignalparams']).real
             )
 
             # store bias params
             if  biasparams_dict is not None:  
-                self._1poleresult['biasparams'] = biasparams_dict.copy()
+                self._fit_results[1]['biasparams'] = biasparams_dict.copy()
             else:
-                self._1poleresult['biasparams'] = None
+                self._fit_results[1]['biasparams'] = None
                         
             
-        # 2-poles fit     
-        if poles == 2:
-                              
-            if self._2poleresult is None:
-                raise ValueError(
-                    'ERROR: No 2-poles fit done! Unable to '
-                    'calculate small signal parameters ')
-
-            smallsignalparams = DIDV._converttotesvalues(
-                self._2poleresult['params_array'],
-                self._rsh, self._r0, self._rp
-            )
-
-
-            self._2poleresult['smallsignalparams'] = {
-                'rsh': smallsignalparams[0],
-                'rp': smallsignalparams[1],
-                'r0': smallsignalparams[2],
-                'beta': smallsignalparams[3],
-                'l': smallsignalparams[4],
-                'L': smallsignalparams[5],
-                'tau0': smallsignalparams[6],
-                'dt': smallsignalparams[7],
-            }
-                              
-            self._2poleresult['didv0'] = (
-                complexadmittance(0, **self._2poleresult['smallsignalparams']).real
-            )              
-
-            # store also bias params
-            if  biasparams_dict is not None:  
-                self._2poleresult['biasparams'] = biasparams_dict.copy()
-            else:
-                self._2poleresult['biasparams'] = None
-                
-            
-        if poles == 3:
+        # 2-poles and 3-poles fit     
+        if poles == 2 or poles == 3:
 
-            if self._3poleresult is None:
+            # get result dictionary
+            if (self._fit_results[poles] is None
+                or 'params_array' not in self._fit_results[poles]):
                 raise ValueError(
-                    'ERROR: No 3-poles fit done! Unable to '
-                    'calculate small signal parameters ')
+                    f'ERROR: No {poles}-poles fit done! Unable to '
+                    f'calculate small signal parameters ')
+            
+            # results 
+            results = copy.deepcopy(self._fit_results[poles])
 
+            
+            # convert fit parameterts to smallsignalparams
             smallsignalparams = DIDV._converttotesvalues(
-                self._3poleresult['params_array'],
+                results['params_array'],
                 self._rsh, self._r0, self._rp
             )
 
-            
-            self._3poleresult['smallsignalparams'] = {
+            results['smallsignalparams'] = {
                 'rsh': smallsignalparams[0],
                 'rp': smallsignalparams[1],
                 'r0': smallsignalparams[2],
                 'beta': smallsignalparams[3],
                 'l': smallsignalparams[4],
                 'L': smallsignalparams[5],
                 'tau0': smallsignalparams[6],
                 'gratio': smallsignalparams[7],
                 'tau3': smallsignalparams[8],
                 'dt': smallsignalparams[9],
             }
-            
-            self._3poleresult['didv0'] = (
-                complexadmittance(0, **self._3poleresult['smallsignalparams']).real
-            )   
-                        
+
+                                          
+            results['didv0'] = (
+                complexadmittance(0, **results['smallsignalparams']).real
+            )              
+
             # store bias params
             if  biasparams_dict is not None:  
-                self._3poleresult['biasparams'] = biasparams_dict.copy()
+                results['biasparams'] = biasparams_dict.copy()
             else:
-                self._3poleresult['biasparams'] = None
-          
+                results['biasparams'] = None
+                
             # calculate small signal parameters cov/sigmas
             if lgc_ssp_light:
 
                 if biasparams_dict is None:
                     raise ValueError(
                         'ERROR: "biasparams_dict" required when '
                         'lgc_ssp_light=True'
                     )
 
-                ssp_light_cov = get_smallsignalparams_cov(self._3poleresult)
-                ssp_light_sigmas = get_smallsignalparams_sigmas(self._3poleresult)
+                ssp_light_cov = get_smallsignalparams_cov(results)
+                ssp_light_sigmas = get_smallsignalparams_sigmas(results)
 
                 # store
                 ssp_light_vals = {
                     'beta': smallsignalparams[3],
                     'l': smallsignalparams[4],
                     'L': smallsignalparams[5],
                     'tau0': smallsignalparams[6],
                     'gratio': smallsignalparams[7],
                 }
                 
-                self._3poleresult['ssp_light'] = {
+                results['ssp_light'] = {
                     'vals': ssp_light_vals,
                     'cov': ssp_light_cov,
                     'sigmas': ssp_light_sigmas,
                 }
+
+
+            # store results internally
+            self._fit_results[poles] = results
+            
                 
+
```

### Comparing `QETpy-1.6.6/qetpy/core/didv/_didv_priors.py` & `QETpy-1.6.7/qetpy/core/didv/_didv_priors.py`

 * *Files 8% similar despite different names*

```diff
@@ -372,31 +372,32 @@
         )
 
         falltimes = DIDVPriors._findpolefalltimes(
             DIDVPriors._convertfromtesvalues(params),
         )
 
         if poles == 1:
-            self._1poleresult = DIDVPriors._fitresult(
+            self._fit_results[1] = DIDVPriors._fitresult(
                 poles, params, cov, falltimes, cost,
             )
-            self._1poleresult['priors'] = priors
-            self._1poleresult['priorscov'] = priorscov
+            self._fit_results[1]['priors'] = priors
+            self._fit_results[1]['priorscov'] = priorscov
+            
         elif poles == 2:
-            self._2poleresult = DIDVPriors._fitresult(
+            self._fit_results[2] = DIDVPriors._fitresult(
                 poles, params, cov, falltimes, cost,
             )
-            self._2poleresult['priors'] = priors
-            self._2poleresult['priorscov'] = priorscov
+            self._fit_results[2]['priors'] = priors
+            self._fit_results[2]['priorscov'] = priorscov
         elif poles == 3:
-            self._3poleresult = DIDVPriors._fitresult(
+            self._fit_results[3] = DIDVPriors._fitresult(
                 poles, params, cov, falltimes, cost,
             )
-            self._3poleresult['priors'] = priors
-            self._3poleresult['priorscov'] = priorscov
+            self._fit_results[3]['priors'] = priors
+            self._fit_results[3]['priorscov'] = priorscov
 
 
     @staticmethod
     def _fitresult(poles, params, cov, falltimes, cost):
         """
         Function for converting data from different fit results to a
         results dictionary.
```

### Comparing `QETpy-1.6.6/qetpy/core/didv/_plot_didv.py` & `QETpy-1.6.7/qetpy/core/didv/_plot_didv.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import numpy as np
 import matplotlib.pyplot as plt
 from scipy.fftpack import fft, ifft, fftfreq
 
-
 from ._base_didv import squarewaveresponse, complexadmittance
 from qetpy.utils import lowpassfilter
 
 
 class _PlotDIDV(object):
     """Class that contains all plotting functions for DIDV."""
 
@@ -17,22 +16,22 @@
 
         """
 
         cost_lambda = lambda x: x['cost'] if x is not None else None
         dt_lambda = lambda x: x['params']['dt'] if x is not None else None
 
         cost_vals = [
-            cost_lambda(self._1poleresult),
-            cost_lambda(self._2poleresult),
-            cost_lambda(self._3poleresult),
+            cost_lambda(self._fit_results[1]),
+            cost_lambda(self._fit_results[2]),
+            cost_lambda(self._fit_results[3]),
         ]
         dt_vals = [
-            dt_lambda(self._1poleresult),
-            dt_lambda(self._2poleresult),
-            dt_lambda(self._3poleresult),
+            dt_lambda(self._fit_results[1]),
+            dt_lambda(self._fit_results[2]),
+            dt_lambda(self._fit_results[3]),
         ]
         if all(fv is None for fv in cost_vals):
             best_time_offset = 0
         else:
             min_cost_idx = min(
                 (val, ii) for ii, val in enumerate(
                     cost_vals
@@ -127,107 +126,109 @@
                 color='purple',
                 alpha=0.7,
                 label='Mean, dIdV Frequencies Only',
             )
 
                 
 
-        if (self._1poleresult is not None) and (1 in poleslist):
-            if 'smallsignalparams' in self._1poleresult:
+        if (self._fit_results[1] is not None) and (1 in poleslist):
+            if 'smallsignalparams' in self._fit_results[1]:
                 key = 'smallsignalparams'
             else:
                 key = 'params'
             didvfit1_timedomain = squarewaveresponse(
                 self._time,
                 self._sgamp,
                 self._sgfreq,
                 self._dutycycle,
-                **self._1poleresult[key],
+                **self._fit_results[1][key],
             )
             
             if lp_cutoff is not None:
                 lp_1poleresult = lowpassfilter(didvfit1_timedomain,
                                          lp_cutoff, fs=self._fs, order=2)
                 ax.plot(
-                    (self._time + self._1poleresult['params']['dt']) * 1e6,
+                    (self._time + self._fit_results[1]['params']['dt']) * 1e6,
                     lp_1poleresult * 1e6,
                     color='magenta',
                     alpha=0.9,
                     label='1-Pole Fit-filtered',
                 )
             
             elif lp_cutoff is None:
                 ax.plot(
-                    (self._time + self._1poleresult['params']['dt']) * 1e6,
+                    (self._time + self._fit_results[1]['params']['dt']) * 1e6,
                     didvfit1_timedomain * 1e6,
                     color='magenta',
                     alpha=0.9,
                     label='1-Pole Fit',
                 )    
             
-        if (self._2poleresult is not None) and (2 in poleslist):
-            if 'smallsignalparams' in self._2poleresult:
+        if (self._fit_results[2] is not None) and (2 in poleslist):
+            if 'smallsignalparams' in self._fit_results[2]:
                 key = 'smallsignalparams'
             else:
                 key = 'params'
             didvfit2_timedomain = squarewaveresponse(
                 self._time,
                 self._sgamp,
                 self._sgfreq,
                 self._dutycycle,
-                **self._2poleresult[key],
+                **self._fit_results[2][key],
             )
             
             if lp_cutoff is not None:
                 lp_2poleresult = lowpassfilter(didvfit2_timedomain,
-                                         lp_cutoff, fs=self._fs, order=2)
+                                               lp_cutoff, fs=self._fs,
+                                               order=2)
                 ax.plot(
-                    (self._time + self._2poleresult['params']['dt']) * 1e6,
+                    (self._time + self._fit_results[2]['params']['dt']) * 1e6,
                     lp_2poleresult * 1e6,
                     color='green',
                     alpha=0.9,
                     label='2-Pole Fit-filtered',
                 )
                 
             elif lp_cutoff is None:
                 ax.plot(
-                    (self._time + self._2poleresult['params']['dt']) * 1e6,
+                    (self._time + self._fit_results[2]['params']['dt']) * 1e6,
                     didvfit2_timedomain * 1e6,
                     color='green',
                     alpha=0.9,
                     label='2-Pole Fit',
                 )
 
-        if (self._3poleresult is not None) and (3 in poleslist):
-            if 'smallsignalparams' in self._3poleresult:
+        if (self._fit_results[3] is not None) and (3 in poleslist):
+            if 'smallsignalparams' in self._fit_results[3]:
                 key = 'smallsignalparams'
             else:
                 key = 'params'
             didvfit3_timedomain = squarewaveresponse(
                 self._time,
                 self._sgamp,
                 self._sgfreq,
                 self._dutycycle,
-                **self._3poleresult[key],
+                **self._fit_results[3][key],
             )
             
             if lp_cutoff is not None:
                 lp_3poleresult = lowpassfilter(didvfit3_timedomain,
-                                         lp_cutoff, fs=self._fs, order=2)
+                                               lp_cutoff, fs=self._fs,
+                                               order=2)
                 ax.plot(
-                    (self._time + self._3poleresult['params']['dt']) * 1e6,
+                    (self._time + self._fit_results[3]['params']['dt']) * 1e6,
                     lp_3poleresult * 1e6,
                     color='orange',
                     alpha=0.9,
                     label='3-Pole Fit-filtered',
                 )
                 
             elif lp_cutoff is None:
                 ax.plot(
-                    (self._time + self._3poleresult['params']['dt']) * 1e6,
+                    (self._time + self._fit_results[3]['params']['dt']) * 1e6,
                     didvfit3_timedomain * 1e6,
                     color='orange',
                     alpha=0.9,
                     label='3-Pole Fit',
                 )
 
         ax.set_xlabel('Time ($\mu$s)')
@@ -511,51 +512,51 @@
         ax.plot(
             self._freq[plotinds],
             function((self._didvmean - self._didvstd) * time_phase)[plotinds],
             color='black',
             alpha=0.1,
         )
 
-        if (self._1poleresult is not None) and (1 in poleslist):
-            if 'smallsignalparams' in self._1poleresult:
+        if (self._fit_results[1] is not None) and (1 in poleslist):
+            if 'smallsignalparams' in self._fit_results[1]:
                 key = 'smallsignalparams'
             else:
                 key = 'params'
             didvfit1_freqdomain = complexadmittance(
-                self._freq, **self._1poleresult[key],
+                self._freq, **self._fit_results[1][key],
             )
             ax.plot(
                 self._freq[fitinds],
                 function(didvfit1_freqdomain)[fitinds],
                 color='magenta',
                 label='1-Pole Fit',
             )
 
-        if (self._2poleresult is not None) and (2 in poleslist):
-            if 'smallsignalparams' in self._2poleresult:
+        if (self._fit_results[2] is not None) and (2 in poleslist):
+            if 'smallsignalparams' in self._fit_results[2]:
                 key = 'smallsignalparams'
             else:
                 key = 'params'
             didvfit2_freqdomain = complexadmittance(
-                self._freq, **self._2poleresult[key],
+                self._freq, **self._fit_results[2][key],
             )
             ax.plot(
                 self._freq[fitinds],
                 function(didvfit2_freqdomain)[fitinds],
                 color='green',
                 label='2-Pole Fit',
             )
 
-        if (self._3poleresult is not None) and (3 in poleslist):
-            if 'smallsignalparams' in self._3poleresult:
+        if (self._fit_results[3] is not None) and (3 in poleslist):
+            if 'smallsignalparams' in self._fit_results[3]:
                 key = 'smallsignalparams'
             else:
                 key = 'params'
             didvfit3_freqdomain = complexadmittance(
-                self._freq, **self._3poleresult[key],
+                self._freq, **self._fit_results[3][key],
             )
             ax.plot(
                 self._freq[fitinds],
                 function(didvfit3_freqdomain)[fitinds],
                 color='orange',
                 label='3-Pole Fit',
             )
@@ -721,51 +722,51 @@
             np.real(1 / (self._didvmean * time_phase))[plotinds],
             np.imag(1 / (self._didvmean * time_phase))[plotinds],
             color='blue',
             label='Mean',
             s=5,
         )
 
-        if (self._1poleresult is not None) and (1 in poleslist):
-            if 'smallsignalparams' in self._1poleresult:
+        if (self._fit_results[1] is not None) and (1 in poleslist):
+            if 'smallsignalparams' in self._fit_results[1]:
                 key = 'smallsignalparams'
             else:
                 key = 'params'
             didvfit1_freqdomain = complexadmittance(
-                self._freq, **self._1poleresult[key],
+                self._freq, **self._fit_results[1][key],
             )
             ax.plot(
                 np.real(1 / didvfit1_freqdomain)[fitinds],
                 np.imag(1 / didvfit1_freqdomain)[fitinds],
                 color='magenta',
                 label='1-Pole Fit',
             )
 
-        if (self._2poleresult is not None) and (2 in poleslist):
-            if 'smallsignalparams' in self._2poleresult:
+        if (self._fit_results[2] is not None) and (2 in poleslist):
+            if 'smallsignalparams' in self._fit_results[2]:
                 key = 'smallsignalparams'
             else:
                 key = 'params'
             didvfit2_freqdomain = complexadmittance(
-                self._freq, **self._2poleresult[key],
+                self._freq, **self._fit_results[2][key],
             )
             ax.plot(
                 np.real(1 / didvfit2_freqdomain)[fitinds],
                 np.imag(1 / didvfit2_freqdomain)[fitinds],
                 color='green',
                 label='2-Pole Fit',
             )
 
-        if (self._3poleresult is not None) and (3 in poleslist):
-            if 'smallsignalparams' in self._3poleresult:
+        if (self._fit_results[3] is not None) and (3 in poleslist):
+            if 'smallsignalparams' in self._fit_results[3]:
                 key = 'smallsignalparams'
             else:
                 key = 'params'
             didvfit3_freqdomain = complexadmittance(
-                self._freq, **self._3poleresult[key],
+                self._freq, **self._fit_results[3][key],
             )
             ax.plot(
                 np.real(1 / didvfit3_freqdomain)[fitinds],
                 np.imag(1 / didvfit3_freqdomain)[fitinds],
                 color='orange',
                 label='3-Pole Fit',
             )
```

### Comparing `QETpy-1.6.6/qetpy/core/didv/_templates_didv.py` & `QETpy-1.6.7/qetpy/core/didv/_templates_didv.py`

 * *Files identical despite different names*

### Comparing `QETpy-1.6.6/qetpy/core/didv/_uncertainties_didv.py` & `QETpy-1.6.7/qetpy/core/didv/_uncertainties_didv.py`

 * *Files identical despite different names*

### Comparing `QETpy-1.6.6/qetpy/cut/_cut.py` & `QETpy-1.6.7/qetpy/cut/_cut.py`

 * *Files identical despite different names*

### Comparing `QETpy-1.6.6/qetpy/plotting/_fitting_plotting.py` & `QETpy-1.6.7/qetpy/plotting/_fitting_plotting.py`

 * *Files identical despite different names*

### Comparing `QETpy-1.6.6/qetpy/plotting/_ibis_plotting.py` & `QETpy-1.6.7/qetpy/plotting/_ibis_plotting.py`

 * *Files identical despite different names*

### Comparing `QETpy-1.6.6/qetpy/plotting/_iv_plotting.py` & `QETpy-1.6.7/qetpy/plotting/_iv_plotting.py`

 * *Files identical despite different names*

### Comparing `QETpy-1.6.6/qetpy/plotting/_noise_plotting.py` & `QETpy-1.6.7/qetpy/plotting/_noise_plotting.py`

 * *Files identical despite different names*

### Comparing `QETpy-1.6.6/qetpy/plotting/_of_nsmb_plotting.py` & `QETpy-1.6.7/qetpy/plotting/_of_nsmb_plotting.py`

 * *Files identical despite different names*

### Comparing `QETpy-1.6.6/qetpy/sim/_sim.py` & `QETpy-1.6.7/qetpy/sim/_sim.py`

 * *Files identical despite different names*

### Comparing `QETpy-1.6.6/qetpy/utils/_utils.py` & `QETpy-1.6.7/qetpy/utils/_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,17 +5,14 @@
 from sympy.ntheory import factorrat
 from sympy.core.symbol import S
 
 # global variable for the fft, fftfreq and
 # ifft functions
 FFT_MODULE = 'scipy'
 
-
-
-
 __all__ = [
     "make_decreasing",
     "calc_offset",
     "lowpassfilter",
     "align_traces",
     "get_offset_from_muon",
     "powertrace_simple",
```

### Comparing `QETpy-1.6.6/setup.py` & `QETpy-1.6.7/setup.py`

 * *Files identical despite different names*

### Comparing `QETpy-1.6.6/test/test_cut.py` & `QETpy-1.6.7/test/test_cut.py`

 * *Files identical despite different names*

### Comparing `QETpy-1.6.6/test/test_detcal.py` & `QETpy-1.6.7/test/test_detcal.py`

 * *Files identical despite different names*

### Comparing `QETpy-1.6.6/test/test_didv.py` & `QETpy-1.6.7/test/test_didv.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import qetpy as qp
 import numpy as np
 import pytest
 
 
-def _initialize_didv(poles, priors, sgfreq=100, autoresample=False):
+def _initialize_didv(poles, sgfreq=100, autoresample=False):
     """Function for initializing dIdV data"""
     np.random.seed(0)
 
     rsh = 5e-3
     rbias_sg = 20000
     fs = 625e3
     sgamp = 0.009381 / rbias_sg
@@ -32,67 +32,36 @@
 
     psd_test = np.ones(int(4 * fs / sgfreq)) / tracegain**2 / 1e4
     rawnoise = qp.gen_noise(psd_test, fs=fs, ntraces=300)
 
     t = np.arange(rawnoise.shape[-1]) / fs
     didv_response = qp.squarewaveresponse(
         t, sgamp, sgfreq, **true_params,
+
     )
     rawtraces = didv_response + rawnoise
 
-    if priors:
-        if poles == 1:
-            dim = 4
-        elif poles == 2:
-            dim = 8
-        elif poles == 3:
-            dim = 10
-        priors = np.zeros(dim)
-        priorscov = np.zeros((dim, dim))
-
-        priors[0] = true_params['rsh']
-        priorscov[0, 0] = (0.1 * priors[0])**2
-        priors[1] = true_params['rp']
-        priorscov[1, 1] = (0.1 * priors[1])**2
-
-        if poles != 1:
-            priors[2] = true_params['r0']
-            priorscov[2, 2] = (0.1 * priors[2])**2
-
-        didvfit = qp.DIDVPriors(
-            rawtraces,
-            fs,
-            sgfreq,
-            sgamp,
-            rsh,
-            tracegain=1.0,
-            dt0=-1e-6,
-            autoresample=autoresample,
-        )
-        if poles == 1:
-            didvfit.processtraces()
-            didvfit.plot_full_trace()
-        assert didvfit.fitresult(poles) == dict()
-        didvfit.dofit(poles, priors, priorscov)
-    else:
-        didvfit = qp.DIDV(
-            rawtraces,
-            fs,
-            sgfreq,
-            sgamp,
-            rsh,
-            tracegain=1.0,
-            r0=true_params['r0'],
-            rp=true_params['rp'],
-            dt0=-1e-6 - 1 / (2 * sgfreq),
-            add180phase=True,
-            autoresample=autoresample,
-        )
-        assert didvfit.fitresult(poles) == dict()
-        didvfit.dofit(poles)
+    # didv fit
+    
+    didvfit = qp.DIDV(
+        rawtraces,
+        fs,
+        sgfreq,
+        sgamp,
+        rsh,
+        tracegain=1.0,
+        r0=true_params['r0'],
+        rp=true_params['rp'],
+        dt0=-1e-6 - 1 / (2 * sgfreq),
+        add180phase=True,
+        autoresample=autoresample,
+    )
+    
+    didvfit.dofit(poles)
+    assert isinstance(didvfit.fitresult(poles), dict)
 
     _run_plotting_suite(didvfit, poles)
 
     return didvfit, true_params
 
 
 def _run_plotting_suite(didvfit, poles):
@@ -164,24 +133,24 @@
 
     assert didvfit._rawtraces.shape[-1] == expected_length
 
 
 def test_didv():
     """Function for testing the DIDV and DIDVPriors classes."""
 
+
     poles = [1, 2, 3]
-    priors = [True, False]
-    keys = ['params', 'smallsignalparams']
 
     for pole in poles:
-        for key, prior in zip(keys, priors):
-            didvfit, true_params = _initialize_didv(pole, prior)
-            assert np.isclose(
-                qp.complexadmittance(
-                    1e4, **didvfit.fitresult(pole)[key],
-                ),
-                qp.complexadmittance(
-                    1e4, **true_params,
-                ),
-                rtol=1e-2,
-            )
+        didvfit, true_params = _initialize_didv(pole)
+            
+        assert np.isclose(
+            qp.complexadmittance(
+                1e4, **didvfit.fitresult(pole)['smallsignalparams'],
+            ),
+            qp.complexadmittance(
+                1e4, **true_params,
+            ),
+            rtol=1e-2,
+        )
 
+
```

### Comparing `QETpy-1.6.6/test/test_fitting.py` & `QETpy-1.6.7/test/test_fitting.py`

 * *Files identical despite different names*

### Comparing `QETpy-1.6.6/test/test_ibis.py` & `QETpy-1.6.7/test/test_ibis.py`

 * *Files identical despite different names*

### Comparing `QETpy-1.6.6/test/test_ofnsmb.py` & `QETpy-1.6.7/test/test_ofnsmb.py`

 * *Files identical despite different names*

### Comparing `QETpy-1.6.6/test/test_utils.py` & `QETpy-1.6.7/test/test_utils.py`

 * *Files identical despite different names*

