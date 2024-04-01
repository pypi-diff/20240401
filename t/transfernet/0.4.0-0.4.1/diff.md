# Comparing `tmp/transfernet-0.4.0.tar.gz` & `tmp/transfernet-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "transfernet-0.4.0.tar", last modified: Fri Mar 29 17:59:44 2024, max compression
+gzip compressed data, was "transfernet-0.4.1.tar", last modified: Mon Apr  1 14:37:31 2024, max compression
```

## Comparing `transfernet-0.4.0.tar` & `transfernet-0.4.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 17:59:44.485091 transfernet-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-03-29 17:59:39.000000 transfernet-0.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1376 2024-03-29 17:59:44.485091 transfernet-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      759 2024-03-29 17:59:39.000000 transfernet-0.4.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-29 17:59:44.485091 transfernet-0.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1538 2024-03-29 17:59:39.000000 transfernet-0.4.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 17:59:44.481091 transfernet-0.4.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 17:59:44.481091 transfernet-0.4.0/src/transfernet/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-29 17:59:39.000000 transfernet-0.4.0/src/transfernet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1800 2024-03-29 17:59:40.000000 transfernet-0.4.0/src/transfernet/datasets.py
--rw-r--r--   0 runner    (1001) docker     (127)     2824 2024-03-29 17:59:40.000000 transfernet-0.4.0/src/transfernet/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     5308 2024-03-29 17:59:40.000000 transfernet-0.4.0/src/transfernet/plots.py
--rw-r--r--   0 runner    (1001) docker     (127)     8369 2024-03-29 17:59:40.000000 transfernet-0.4.0/src/transfernet/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 17:59:44.485091 transfernet-0.4.0/src/transfernet.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1376 2024-03-29 17:59:44.000000 transfernet-0.4.0/src/transfernet.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      370 2024-03-29 17:59:44.000000 transfernet-0.4.0/src/transfernet.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-29 17:59:44.000000 transfernet-0.4.0/src/transfernet.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-03-29 17:59:44.000000 transfernet-0.4.0/src/transfernet.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-03-29 17:59:44.000000 transfernet-0.4.0/src/transfernet.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 17:59:44.485091 transfernet-0.4.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1968 2024-03-29 17:59:40.000000 transfernet-0.4.0/tests/test_run.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 14:37:31.739861 transfernet-0.4.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-04-01 14:37:27.000000 transfernet-0.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1376 2024-04-01 14:37:31.739861 transfernet-0.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      759 2024-04-01 14:37:27.000000 transfernet-0.4.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-01 14:37:31.739861 transfernet-0.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1538 2024-04-01 14:37:27.000000 transfernet-0.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 14:37:31.735861 transfernet-0.4.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 14:37:31.739861 transfernet-0.4.1/src/transfernet/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 14:37:27.000000 transfernet-0.4.1/src/transfernet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1800 2024-04-01 14:37:28.000000 transfernet-0.4.1/src/transfernet/datasets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2824 2024-04-01 14:37:28.000000 transfernet-0.4.1/src/transfernet/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5414 2024-04-01 14:37:28.000000 transfernet-0.4.1/src/transfernet/plots.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8369 2024-04-01 14:37:28.000000 transfernet-0.4.1/src/transfernet/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 14:37:31.739861 transfernet-0.4.1/src/transfernet.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1376 2024-04-01 14:37:31.000000 transfernet-0.4.1/src/transfernet.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      370 2024-04-01 14:37:31.000000 transfernet-0.4.1/src/transfernet.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 14:37:31.000000 transfernet-0.4.1/src/transfernet.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-01 14:37:31.000000 transfernet-0.4.1/src/transfernet.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-01 14:37:31.000000 transfernet-0.4.1/src/transfernet.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 14:37:31.739861 transfernet-0.4.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1968 2024-04-01 14:37:28.000000 transfernet-0.4.1/tests/test_run.py
```

### Comparing `transfernet-0.4.0/LICENSE` & `transfernet-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `transfernet-0.4.0/PKG-INFO` & `transfernet-0.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: transfernet
-Version: 0.4.0
+Version: 0.4.1
 Summary: Deep learning transfer learning.
 Home-page: https://github.com/leschultz/transfernet.git
 Author: Lane E. Schultz
 Author-email: laneenriqueschultz@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

 * *error from `html2text {}`:*

 * *File "/tmp/diffoscope_j2uth84y_/tmpzavvuqx7_TarContainer/0/2", line 43, column 0: CDATA terminal not found*

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: transfernet Version: 0.4.0 Summary: Deep learning
+Metadata-Version: 2.1 Name: transfernet Version: 0.4.1 Summary: Deep learning
 transfer learning. Home-page: https://github.com/leschultz/transfernet.git
 Author: Lane E. Schultz Author-email: laneenriqueschultz@gmail.com Classifier:
 Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT
 License Classifier: Operating System :: OS Independent Requires-Python: >=3.10
 Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
 matplotlib Requires-Dist: scikit-learn Requires-Dist: pandas Requires-Dist:
 pymatgen Requires-Dist: numpy Requires-Dist: pytest Requires-Dist: torch #
```

### Comparing `transfernet-0.4.0/README.md` & `transfernet-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `transfernet-0.4.0/setup.py` & `transfernet-0.4.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 # Package information
 name = 'transfernet'
-version = '0.4.0'  # Need to increment every time to push to PyPI
+version = '0.4.1'  # Need to increment every time to push to PyPI
 description = 'Deep learning transfer learning.'
 url = 'https://github.com/leschultz/transfernet.git'
 author = 'Lane E. Schultz'
 author_email = 'laneenriqueschultz@gmail.com'
 python_requires = '>=3.10'
 classifiers = ['Programming Language :: Python :: 3',
                'License :: OSI Approved :: MIT License',
```

### Comparing `transfernet-0.4.0/src/transfernet/datasets.py` & `transfernet-0.4.1/src/transfernet/datasets.py`

 * *Files identical despite different names*

### Comparing `transfernet-0.4.0/src/transfernet/models.py` & `transfernet-0.4.1/src/transfernet/models.py`

 * *Files identical despite different names*

### Comparing `transfernet-0.4.0/src/transfernet/plots.py` & `transfernet-0.4.1/src/transfernet/plots.py`

 * *Files 8% similar despite different names*

```diff
@@ -97,18 +97,19 @@
                               bbox_to_anchor=(0.5, 0.5)
                               )
     ax_legend.spines['top'].set_visible(False)
     ax_legend.spines['bottom'].set_visible(False)
     ax_legend.spines['left'].set_visible(False)
     ax_legend.spines['right'].set_visible(False)
 
-    fig.savefig(save, bbox_inches='tight')
+    fig.savefig(save, bbox_inches='tight', dpi=400)
     fig_legend.savefig(
                        save.replace('.png', '_legend.png'),
                        bbox_inches='tight',
+                       dpi=400,
                        )
 
     pl.close(fig)
     pl.close(fig_legend)
 
     data = {}
     data[r'$RMSE$'] = float(rmse)
@@ -175,14 +176,15 @@
         ax.set_ylabel('Mean Average Error')
 
         fig.tight_layout()
         name = save_dir+'_{}'.format(group)
         fig.savefig(
                     name+'.png',
                     bbox_inches='tight',
+                    dpi=400,
                     )
 
         # Legend by itself
         fig_legend, ax_legend = pl.subplots()
         ax_legend.axis(False)
         legend = ax_legend.legend(
                                   *ax.get_legend_handles_labels(),
@@ -194,14 +196,15 @@
         ax_legend.spines['bottom'].set_visible(False)
         ax_legend.spines['left'].set_visible(False)
         ax_legend.spines['right'].set_visible(False)
 
         fig_legend.savefig(
                            name+'_legend.png',
                            bbox_inches='tight',
+                           dpi=400,
                            )
 
         data = {}
         data['mae'] = values['mae'].tolist()
         data['epoch'] = values['epoch'].tolist()
 
         with open(name+'.json', 'w') as handle:
```

### Comparing `transfernet-0.4.0/src/transfernet/utils.py` & `transfernet-0.4.1/src/transfernet/utils.py`

 * *Files identical despite different names*

### Comparing `transfernet-0.4.0/src/transfernet.egg-info/PKG-INFO` & `transfernet-0.4.1/src/transfernet.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: transfernet
-Version: 0.4.0
+Version: 0.4.1
 Summary: Deep learning transfer learning.
 Home-page: https://github.com/leschultz/transfernet.git
 Author: Lane E. Schultz
 Author-email: laneenriqueschultz@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

 * *error from `html2text {}`:*

 * *File "/tmp/diffoscope_j2uth84y_/tmpzavvuqx7_TarContainer/0/14", line 43, column 0: CDATA terminal not found*

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: transfernet Version: 0.4.0 Summary: Deep learning
+Metadata-Version: 2.1 Name: transfernet Version: 0.4.1 Summary: Deep learning
 transfer learning. Home-page: https://github.com/leschultz/transfernet.git
 Author: Lane E. Schultz Author-email: laneenriqueschultz@gmail.com Classifier:
 Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT
 License Classifier: Operating System :: OS Independent Requires-Python: >=3.10
 Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
 matplotlib Requires-Dist: scikit-learn Requires-Dist: pandas Requires-Dist:
 pymatgen Requires-Dist: numpy Requires-Dist: pytest Requires-Dist: torch #
```

### Comparing `transfernet-0.4.0/tests/test_run.py` & `transfernet-0.4.1/tests/test_run.py`

 * *Files identical despite different names*

