# Comparing `tmp/autoreviewer-0.0.4.tar.gz` & `tmp/autoreviewer-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autoreviewer-0.0.4.tar", last modified: Thu Jan 25 09:25:00 2024, max compression
+gzip compressed data, was "autoreviewer-0.0.5.tar", last modified: Mon Apr  1 19:47:55 2024, max compression
```

## Comparing `autoreviewer-0.0.4.tar` & `autoreviewer-0.0.5.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2024-01-25 09:25:00.426612 autoreviewer-0.0.4/
--rw-r--r--   0 cthoyt     (501) staff       (20)     1076 2023-08-27 19:16:47.000000 autoreviewer-0.0.4/LICENSE
--rw-r--r--   0 cthoyt     (501) staff       (20)      382 2023-08-27 19:16:47.000000 autoreviewer-0.0.4/MANIFEST.in
--rw-r--r--   0 cthoyt     (501) staff       (20)     8807 2024-01-25 09:25:00.426539 autoreviewer-0.0.4/PKG-INFO
--rw-r--r--   0 cthoyt     (501) staff       (20)     7015 2024-01-16 10:19:34.000000 autoreviewer-0.0.4/README.md
-drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2024-01-25 09:25:00.420751 autoreviewer-0.0.4/docs/
-drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2024-01-25 09:25:00.422414 autoreviewer-0.0.4/docs/source/
--rw-r--r--   0 cthoyt     (501) staff       (20)      241 2023-08-27 19:16:47.000000 autoreviewer-0.0.4/docs/source/cli.rst
--rw-r--r--   0 cthoyt     (501) staff       (20)     7028 2024-01-25 09:25:00.000000 autoreviewer-0.0.4/docs/source/conf.py
--rw-r--r--   0 cthoyt     (501) staff       (20)     1815 2023-08-27 19:16:47.000000 autoreviewer-0.0.4/docs/source/index.rst
--rw-r--r--   0 cthoyt     (501) staff       (20)      529 2023-08-27 19:16:47.000000 autoreviewer-0.0.4/docs/source/installation.rst
--rw-r--r--   0 cthoyt     (501) staff       (20)       59 2023-08-27 19:16:47.000000 autoreviewer-0.0.4/docs/source/usage.rst
--rw-r--r--   0 cthoyt     (501) staff       (20)      360 2023-08-27 19:16:47.000000 autoreviewer-0.0.4/pyproject.toml
--rw-r--r--   0 cthoyt     (501) staff       (20)     2369 2024-01-25 09:25:00.427039 autoreviewer-0.0.4/setup.cfg
-drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2024-01-25 09:25:00.420954 autoreviewer-0.0.4/src/
-drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2024-01-25 09:25:00.423173 autoreviewer-0.0.4/src/autoreviewer/
--rw-r--r--   0 cthoyt     (501) staff       (20)       96 2023-08-27 19:16:47.000000 autoreviewer-0.0.4/src/autoreviewer/__init__.py
--rw-r--r--   0 cthoyt     (501) staff       (20)      329 2023-08-27 19:16:47.000000 autoreviewer-0.0.4/src/autoreviewer/__main__.py
--rw-r--r--   0 cthoyt     (501) staff       (20)     7098 2024-01-25 09:14:56.000000 autoreviewer-0.0.4/src/autoreviewer/api.py
--rw-r--r--   0 cthoyt     (501) staff       (20)     1724 2024-01-25 09:17:57.000000 autoreviewer-0.0.4/src/autoreviewer/cli.py
-drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2024-01-25 09:25:00.425530 autoreviewer-0.0.4/src/autoreviewer/jcheminf/
--rw-r--r--   0 cthoyt     (501) staff       (20)       43 2023-08-27 19:16:47.000000 autoreviewer-0.0.4/src/autoreviewer/jcheminf/__init__.py
--rw-r--r--   0 cthoyt     (501) staff       (20)       97 2023-08-27 19:16:47.000000 autoreviewer-0.0.4/src/autoreviewer/jcheminf/__main__.py
--rw-r--r--   0 cthoyt     (501) staff       (20)   227345 2024-01-15 15:44:51.000000 autoreviewer-0.0.4/src/autoreviewer/jcheminf/analysis.tsv
--rw-r--r--   0 cthoyt     (501) staff       (20)   178242 2024-01-15 15:14:40.000000 autoreviewer-0.0.4/src/autoreviewer/jcheminf/doi_to_github.tsv
--rw-r--r--   0 cthoyt     (501) staff       (20)     8521 2024-01-16 10:17:06.000000 autoreviewer-0.0.4/src/autoreviewer/jcheminf/jcheminf_pilot.py
--rw-r--r--   0 cthoyt     (501) staff       (20)   220611 2024-01-16 18:32:47.000000 autoreviewer-0.0.4/src/autoreviewer/jcheminf/jcheminf_summary.png
--rw-r--r--   0 cthoyt     (501) staff       (20)     3058 2024-01-16 18:32:46.000000 autoreviewer-0.0.4/src/autoreviewer/jcheminf/summarize.py
--rw-r--r--   0 cthoyt     (501) staff       (20)        1 2023-08-27 19:16:47.000000 autoreviewer-0.0.4/src/autoreviewer/py.typed
-drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2024-01-25 09:25:00.425662 autoreviewer-0.0.4/src/autoreviewer/templates/
--rw-r--r--   0 cthoyt     (501) staff       (20)    10234 2024-01-15 10:17:21.000000 autoreviewer-0.0.4/src/autoreviewer/templates/review.md
--rw-r--r--   0 cthoyt     (501) staff       (20)     6847 2024-01-25 09:22:23.000000 autoreviewer-0.0.4/src/autoreviewer/utils.py
--rw-r--r--   0 cthoyt     (501) staff       (20)     1024 2024-01-25 09:25:00.000000 autoreviewer-0.0.4/src/autoreviewer/version.py
-drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2024-01-25 09:25:00.426084 autoreviewer-0.0.4/src/autoreviewer.egg-info/
--rw-r--r--   0 cthoyt     (501) staff       (20)     8807 2024-01-25 09:25:00.000000 autoreviewer-0.0.4/src/autoreviewer.egg-info/PKG-INFO
--rw-r--r--   0 cthoyt     (501) staff       (20)     1000 2024-01-25 09:25:00.000000 autoreviewer-0.0.4/src/autoreviewer.egg-info/SOURCES.txt
--rw-r--r--   0 cthoyt     (501) staff       (20)        1 2024-01-25 09:25:00.000000 autoreviewer-0.0.4/src/autoreviewer.egg-info/dependency_links.txt
--rw-r--r--   0 cthoyt     (501) staff       (20)       90 2024-01-25 09:25:00.000000 autoreviewer-0.0.4/src/autoreviewer.egg-info/entry_points.txt
--rw-r--r--   0 cthoyt     (501) staff       (20)        1 2023-08-29 10:38:18.000000 autoreviewer-0.0.4/src/autoreviewer.egg-info/not-zip-safe
--rw-r--r--   0 cthoyt     (501) staff       (20)      221 2024-01-25 09:25:00.000000 autoreviewer-0.0.4/src/autoreviewer.egg-info/requires.txt
--rw-r--r--   0 cthoyt     (501) staff       (20)       13 2024-01-25 09:25:00.000000 autoreviewer-0.0.4/src/autoreviewer.egg-info/top_level.txt
-drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2024-01-25 09:25:00.425887 autoreviewer-0.0.4/tests/
--rw-r--r--   0 cthoyt     (501) staff       (20)       62 2023-08-27 19:16:47.000000 autoreviewer-0.0.4/tests/__init__.py
--rw-r--r--   0 cthoyt     (501) staff       (20)      406 2023-08-27 19:16:47.000000 autoreviewer-0.0.4/tests/test_version.py
+drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2024-04-01 19:47:55.106169 autoreviewer-0.0.5/
+-rw-r--r--   0 cthoyt     (501) staff       (20)     1076 2023-08-27 19:16:47.000000 autoreviewer-0.0.5/LICENSE
+-rw-r--r--   0 cthoyt     (501) staff       (20)      382 2023-08-27 19:16:47.000000 autoreviewer-0.0.5/MANIFEST.in
+-rw-r--r--   0 cthoyt     (501) staff       (20)     8865 2024-04-01 19:47:55.106082 autoreviewer-0.0.5/PKG-INFO
+-rw-r--r--   0 cthoyt     (501) staff       (20)     7015 2024-01-16 10:19:34.000000 autoreviewer-0.0.5/README.md
+drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2024-04-01 19:47:55.097536 autoreviewer-0.0.5/docs/
+drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2024-04-01 19:47:55.099354 autoreviewer-0.0.5/docs/source/
+-rw-r--r--   0 cthoyt     (501) staff       (20)      241 2023-08-27 19:16:47.000000 autoreviewer-0.0.5/docs/source/cli.rst
+-rw-r--r--   0 cthoyt     (501) staff       (20)     7028 2024-04-01 19:47:54.000000 autoreviewer-0.0.5/docs/source/conf.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)     1815 2023-08-27 19:16:47.000000 autoreviewer-0.0.5/docs/source/index.rst
+-rw-r--r--   0 cthoyt     (501) staff       (20)      529 2023-08-27 19:16:47.000000 autoreviewer-0.0.5/docs/source/installation.rst
+-rw-r--r--   0 cthoyt     (501) staff       (20)       59 2023-08-27 19:16:47.000000 autoreviewer-0.0.5/docs/source/usage.rst
+-rw-r--r--   0 cthoyt     (501) staff       (20)      360 2023-08-27 19:16:47.000000 autoreviewer-0.0.5/pyproject.toml
+-rw-r--r--   0 cthoyt     (501) staff       (20)     2416 2024-04-01 19:47:55.106574 autoreviewer-0.0.5/setup.cfg
+drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2024-04-01 19:47:55.097684 autoreviewer-0.0.5/src/
+drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2024-04-01 19:47:55.100820 autoreviewer-0.0.5/src/autoreviewer/
+-rw-r--r--   0 cthoyt     (501) staff       (20)       96 2023-08-27 19:16:47.000000 autoreviewer-0.0.5/src/autoreviewer/__init__.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)      329 2023-08-27 19:16:47.000000 autoreviewer-0.0.5/src/autoreviewer/__main__.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)     7229 2024-04-01 19:35:59.000000 autoreviewer-0.0.5/src/autoreviewer/api.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)     1838 2024-04-01 19:37:40.000000 autoreviewer-0.0.5/src/autoreviewer/cli.py
+drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2024-04-01 19:47:55.104697 autoreviewer-0.0.5/src/autoreviewer/jcheminf/
+-rw-r--r--   0 cthoyt     (501) staff       (20)       43 2023-08-27 19:16:47.000000 autoreviewer-0.0.5/src/autoreviewer/jcheminf/__init__.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)       97 2023-08-27 19:16:47.000000 autoreviewer-0.0.5/src/autoreviewer/jcheminf/__main__.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)   227345 2024-01-15 15:44:51.000000 autoreviewer-0.0.5/src/autoreviewer/jcheminf/analysis.tsv
+-rw-r--r--   0 cthoyt     (501) staff       (20)   178242 2024-01-15 15:14:40.000000 autoreviewer-0.0.5/src/autoreviewer/jcheminf/doi_to_github.tsv
+-rw-r--r--   0 cthoyt     (501) staff       (20)     8521 2024-01-16 10:17:06.000000 autoreviewer-0.0.5/src/autoreviewer/jcheminf/jcheminf_pilot.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)   220611 2024-01-16 18:32:47.000000 autoreviewer-0.0.5/src/autoreviewer/jcheminf/jcheminf_summary.png
+-rw-r--r--   0 cthoyt     (501) staff       (20)     3058 2024-01-16 18:32:46.000000 autoreviewer-0.0.5/src/autoreviewer/jcheminf/summarize.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)        1 2023-08-27 19:16:47.000000 autoreviewer-0.0.5/src/autoreviewer/py.typed
+drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2024-04-01 19:47:55.104924 autoreviewer-0.0.5/src/autoreviewer/templates/
+-rw-r--r--   0 cthoyt     (501) staff       (20)    10234 2024-01-15 10:17:21.000000 autoreviewer-0.0.5/src/autoreviewer/templates/review.md
+-rw-r--r--   0 cthoyt     (501) staff       (20)     7814 2024-04-01 19:42:59.000000 autoreviewer-0.0.5/src/autoreviewer/utils.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)     1024 2024-04-01 19:47:54.000000 autoreviewer-0.0.5/src/autoreviewer/version.py
+drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2024-04-01 19:47:55.105565 autoreviewer-0.0.5/src/autoreviewer.egg-info/
+-rw-r--r--   0 cthoyt     (501) staff       (20)     8865 2024-04-01 19:47:55.000000 autoreviewer-0.0.5/src/autoreviewer.egg-info/PKG-INFO
+-rw-r--r--   0 cthoyt     (501) staff       (20)     1000 2024-04-01 19:47:55.000000 autoreviewer-0.0.5/src/autoreviewer.egg-info/SOURCES.txt
+-rw-r--r--   0 cthoyt     (501) staff       (20)        1 2024-04-01 19:47:55.000000 autoreviewer-0.0.5/src/autoreviewer.egg-info/dependency_links.txt
+-rw-r--r--   0 cthoyt     (501) staff       (20)       90 2024-04-01 19:47:55.000000 autoreviewer-0.0.5/src/autoreviewer.egg-info/entry_points.txt
+-rw-r--r--   0 cthoyt     (501) staff       (20)        1 2023-08-29 10:38:18.000000 autoreviewer-0.0.5/src/autoreviewer.egg-info/not-zip-safe
+-rw-r--r--   0 cthoyt     (501) staff       (20)      228 2024-04-01 19:47:55.000000 autoreviewer-0.0.5/src/autoreviewer.egg-info/requires.txt
+-rw-r--r--   0 cthoyt     (501) staff       (20)       13 2024-04-01 19:47:55.000000 autoreviewer-0.0.5/src/autoreviewer.egg-info/top_level.txt
+drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2024-04-01 19:47:55.105349 autoreviewer-0.0.5/tests/
+-rw-r--r--   0 cthoyt     (501) staff       (20)       62 2023-08-27 19:16:47.000000 autoreviewer-0.0.5/tests/__init__.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)      406 2023-08-27 19:16:47.000000 autoreviewer-0.0.5/tests/test_version.py
```

### Comparing `autoreviewer-0.0.4/LICENSE` & `autoreviewer-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `autoreviewer-0.0.4/PKG-INFO` & `autoreviewer-0.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autoreviewer
-Version: 0.0.4
+Version: 0.0.5
 Summary: Automate scientific software review
 Home-page: https://github.com/cthoyt/autoreviewer
 Download-URL: https://github.com/cthoyt/autoreviewer/releases
 Author: Charles Tapley Hoyt
 Author-email: cthoyt@gmail.com
 Maintainer: Charles Tapley Hoyt
 Maintainer-email: cthoyt@gmail.com
@@ -19,14 +19,15 @@
 Classifier: Operating System :: OS Independent
 Classifier: Framework :: Pytest
 Classifier: Framework :: tox
 Classifier: Framework :: Sphinx
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: more_itertools
 Requires-Dist: tqdm
 Requires-Dist: click
@@ -34,15 +35,15 @@
 Requires-Dist: jinja2
 Requires-Dist: ebooklib
 Requires-Dist: requests
 Requires-Dist: pandas
 Requires-Dist: dateutils
 Requires-Dist: beautifulsoup4
 Requires-Dist: tabulate
-Requires-Dist: pystow
+Requires-Dist: pystow>=0.5.4
 Requires-Dist: ratelimit
 Requires-Dist: black
 Requires-Dist: pyroma
 Provides-Extra: tests
 Requires-Dist: pytest; extra == "tests"
 Requires-Dist: coverage; extra == "tests"
 Provides-Extra: docs
```

#### html2text {}

```diff
@@ -1,31 +1,32 @@
-Metadata-Version: 2.1 Name: autoreviewer Version: 0.0.4 Summary: Automate
+Metadata-Version: 2.1 Name: autoreviewer Version: 0.0.5 Summary: Automate
 scientific software review Home-page: https://github.com/cthoyt/autoreviewer
 Download-URL: https://github.com/cthoyt/autoreviewer/releases Author: Charles
 Tapley Hoyt Author-email: cthoyt@gmail.com Maintainer: Charles Tapley Hoyt
 Maintainer-email: cthoyt@gmail.com License: MIT Project-URL: Bug Tracker,
 https://github.com/cthoyt/autoreviewer/issues Project-URL: Source Code, https:/
 /github.com/cthoyt/autoreviewer Keywords: snekpack,cookiecutter Classifier:
 Development Status :: 1 - Planning Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers Classifier: License :: OSI Approved
 :: MIT License Classifier: Operating System :: OS Independent Classifier:
 Framework :: Pytest Classifier: Framework :: tox Classifier: Framework ::
 Sphinx Classifier: Programming Language :: Python Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3 :: Only Requires-Python: >=3.10
-Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
-more_itertools Requires-Dist: tqdm Requires-Dist: click Requires-Dist:
-more_click Requires-Dist: jinja2 Requires-Dist: ebooklib Requires-Dist:
-requests Requires-Dist: pandas Requires-Dist: dateutils Requires-Dist:
-beautifulsoup4 Requires-Dist: tabulate Requires-Dist: pystow Requires-Dist:
-ratelimit Requires-Dist: black Requires-Dist: pyroma Provides-Extra: tests
-Requires-Dist: pytest; extra == "tests" Requires-Dist: coverage; extra ==
-"tests" Provides-Extra: docs Requires-Dist: sphinx; extra == "docs" Requires-
-Dist: sphinx-rtd-theme; extra == "docs" Requires-Dist: sphinx-click; extra ==
-"docs" Requires-Dist: sphinx_automodapi; extra == "docs"
+Classifier: Programming Language :: Python :: 3.12 Classifier: Programming
+Language :: Python :: 3 :: Only Requires-Python: >=3.10 Description-Content-
+Type: text/markdown License-File: LICENSE Requires-Dist: more_itertools
+Requires-Dist: tqdm Requires-Dist: click Requires-Dist: more_click Requires-
+Dist: jinja2 Requires-Dist: ebooklib Requires-Dist: requests Requires-Dist:
+pandas Requires-Dist: dateutils Requires-Dist: beautifulsoup4 Requires-Dist:
+tabulate Requires-Dist: pystow>=0.5.4 Requires-Dist: ratelimit Requires-Dist:
+black Requires-Dist: pyroma Provides-Extra: tests Requires-Dist: pytest; extra
+== "tests" Requires-Dist: coverage; extra == "tests" Provides-Extra: docs
+Requires-Dist: sphinx; extra == "docs" Requires-Dist: sphinx-rtd-theme; extra
+== "docs" Requires-Dist: sphinx-click; extra == "docs" Requires-Dist:
+sphinx_automodapi; extra == "docs"
                           ************ AAuuttooRReevviieewweerr ************
   _[_T_e_s_t_s_]_[_P_y_P_I_]_[_P_y_P_I_ _-_ _P_y_t_h_o_n_ _V_e_r_s_i_o_n_]_[_P_y_P_I_ _-_ _L_i_c_e_n_s_e_]_[_D_o_c_u_m_e_n_t_a_t_i_o_n_ _S_t_a_t_u_s_]
     _[_C_o_d_e_c_o_v_ _s_t_a_t_u_s_]_[_C_o_o_k_i_e_c_u_t_t_e_r_ _t_e_m_p_l_a_t_e_ _f_r_o_m_ _@_c_t_h_o_y_t_]_[_C_o_d_e_ _s_t_y_l_e_:_ _b_l_a_c_k_]
                             _[_C_o_n_t_r_i_b_u_t_o_r_ _C_o_v_e_n_a_n_t_]
 Scientists often do the same bad stuff. Automate giving feedback during peer
 review for Python packages. Goals: 1. Given a GitHub repository, automate
 finding common issues such as - No setup.py/setup.cfg/pyproject.toml - No
```

### Comparing `autoreviewer-0.0.4/README.md` & `autoreviewer-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `autoreviewer-0.0.4/docs/source/conf.py` & `autoreviewer-0.0.5/docs/source/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 # -- Project information -----------------------------------------------------
 
 project = "autoreviewer"
 copyright = f"{date.today().year}, Charles Tapley Hoyt"
 author = "Charles Tapley Hoyt"
 
 # The full version, including alpha/beta/rc tags.
-release = "0.0.4"
+release = "0.0.5"
 
 # The short X.Y version.
 parsed_version = re.match(
     "(?P<major>\d+)\.(?P<minor>\d+)\.(?P<patch>\d+)(?:-(?P<release>[0-9A-Za-z-]+(?:\.[0-9A-Za-z-]+)*))?(?:\+(?P<build>[0-9A-Za-z-]+(?:\.[0-9A-Za-z-]+)*))?",
     release,
 )
 version = parsed_version.expand("\g<major>.\g<minor>.\g<patch>")
```

### Comparing `autoreviewer-0.0.4/docs/source/index.rst` & `autoreviewer-0.0.5/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `autoreviewer-0.0.4/docs/source/installation.rst` & `autoreviewer-0.0.5/docs/source/installation.rst`

 * *Files identical despite different names*

### Comparing `autoreviewer-0.0.4/setup.cfg` & `autoreviewer-0.0.5/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = autoreviewer
-version = 0.0.4
+version = 0.0.5
 description = Automate scientific software review
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/cthoyt/autoreviewer
 download_url = https://github.com/cthoyt/autoreviewer/releases
 project_urls = 
 	Bug Tracker = https://github.com/cthoyt/autoreviewer/issues
@@ -24,14 +24,15 @@
 	Operating System :: OS Independent
 	Framework :: Pytest
 	Framework :: tox
 	Framework :: Sphinx
 	Programming Language :: Python
 	Programming Language :: Python :: 3.10
 	Programming Language :: Python :: 3.11
+	Programming Language :: Python :: 3.12
 	Programming Language :: Python :: 3 :: Only
 keywords = 
 	snekpack
 	cookiecutter
 
 [options]
 install_requires = 
@@ -42,15 +43,15 @@
 	jinja2
 	ebooklib
 	requests
 	pandas
 	dateutils
 	beautifulsoup4
 	tabulate
-	pystow
+	pystow>=0.5.4
 	ratelimit
 	black
 	pyroma
 zip_safe = false
 include_package_data = True
 python_requires = >=3.10
 packages = find:
```

### Comparing `autoreviewer-0.0.4/src/autoreviewer/api.py` & `autoreviewer-0.0.5/src/autoreviewer/api.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,14 +17,15 @@
     check_no_scripts,
     get_default_branch,
     get_has_issues,
     get_is_fork,
     get_license,
     get_programming_language,
     get_readme,
+    get_repo_path,
     get_setup_config,
     remote_check_black_github,
     remote_check_pyroma,
 )
 
 HERE = Path(__file__).parent.resolve()
 TEMPLATES = HERE.joinpath("templates")
@@ -160,43 +161,46 @@
         return False
     for line in text.splitlines():
         if line.startswith("#") and "installation" in line.lower():
             return True
     return False
 
 
-def review(owner: str, name: str) -> Results:
+def review(owner: str, name: str, *, cache: bool = True) -> Results:
     """Review a repository."""
-    repo = f"{owner}/{name}"
     branch = get_default_branch(owner, name)
+
+    # Get the repository, and re-cache if necessary
+    get_repo_path(owner, name, cache=cache)
+
     is_blackened = remote_check_black_github(owner, name)
 
-    readme_name, readme_text = get_readme(repo=repo, branch=branch)
+    readme_name, readme_text = get_readme(owner, name, branch=branch)
     readme_type = README_MAP[readme_name]
     if readme_type is None:
         has_zenodo = False
         has_installation_docs = False
     elif readme_type == "markdown":
         has_zenodo = readme_text is not None and (
             "https://zenodo.org/badge/DOI/10.5281/" in readme_text
             or "https://zenodo.org/badge/latestdoi/" in readme_text
         )
         has_installation_docs = _has_markdown_installation(readme_text)
     elif readme_type == "rst":
         has_zenodo = False
         has_installation_docs = False
-        tqdm.write(f"README was RST, assuming missing zenodo/installation docs: {repo}")
+        tqdm.write(f"README was RST, assuming missing zenodo/installation docs: {owner}/{name}")
     elif readme_type == "txt":
         has_zenodo = False
         has_installation_docs = False
-        tqdm.write(f"README was TXT, assuming missing zenodo/installation docs: {repo}")
+        tqdm.write(f"README was TXT, assuming missing zenodo/installation docs: {owner}/{name}")
     else:
         raise TypeError
 
-    setup_name, setup_text = get_setup_config(repo=repo, branch=branch)
+    setup_name, setup_text = get_setup_config(owner, name, branch=branch)
     has_setup = setup_name is not None
 
     license_name = get_license(owner, name)
 
     pyroma_score, pyroma_failures = remote_check_pyroma(owner, name)
     has_issues = get_has_issues(owner, name)
     language = get_programming_language(owner, name)
```

### Comparing `autoreviewer-0.0.4/src/autoreviewer/cli.py` & `autoreviewer-0.0.5/src/autoreviewer/cli.py`

 * *Files 10% similar despite different names*

```diff
@@ -32,25 +32,26 @@
 @click.argument("name_or_url")
 @click.option(
     "--path",
     type=click.Path(),
     help="A custom path to the output file, otherwise outputs in the current directory",
 )
 @click.option("--open", is_flag=True, help="If set, opens the PDF")
-def main(name_or_url: str, path: Path | None, open: bool):
+@click.option("--no-cache", is_flag=True, help="If set, uses the existing cache")
+def main(name_or_url: str, path: Path | None, open: bool, no_cache: bool) -> None:
     """CLI for autoreviewer."""
     owner, repo, *_ = (
         name_or_url.removeprefix("https://github.com/").removesuffix(".git").rstrip("/").split("/")
     )
-    repo_clean = repo.lower().replace("_", "-")
-    results = review(owner, repo)
+    repo = repo.lower().replace("_", "-")
+    results = review(owner, repo, cache=not no_cache)
     if path is not None:
         results.write_pandoc(path)
     else:
-        path = Path.cwd().joinpath(f"{repo_clean}-review.pdf")
+        path = Path.cwd().joinpath(f"{repo}-review.pdf")
         results.write_pandoc(path)
         click.echo(f"Wrote review PDF to {path}")
     if open:
         subprocess.call(["open", path.as_posix()])
 
 
 if __name__ == "__main__":
```

### Comparing `autoreviewer-0.0.4/src/autoreviewer/jcheminf/analysis.tsv` & `autoreviewer-0.0.5/src/autoreviewer/jcheminf/analysis.tsv`

 * *Files identical despite different names*

### Comparing `autoreviewer-0.0.4/src/autoreviewer/jcheminf/doi_to_github.tsv` & `autoreviewer-0.0.5/src/autoreviewer/jcheminf/doi_to_github.tsv`

 * *Files identical despite different names*

### Comparing `autoreviewer-0.0.4/src/autoreviewer/jcheminf/jcheminf_pilot.py` & `autoreviewer-0.0.5/src/autoreviewer/jcheminf/jcheminf_pilot.py`

 * *Files identical despite different names*

### Comparing `autoreviewer-0.0.4/src/autoreviewer/jcheminf/jcheminf_summary.png` & `autoreviewer-0.0.5/src/autoreviewer/jcheminf/jcheminf_summary.png`

 * *Files identical despite different names*

### Comparing `autoreviewer-0.0.4/src/autoreviewer/jcheminf/summarize.py` & `autoreviewer-0.0.5/src/autoreviewer/jcheminf/summarize.py`

 * *Files identical despite different names*

### Comparing `autoreviewer-0.0.4/src/autoreviewer/templates/review.md` & `autoreviewer-0.0.5/src/autoreviewer/templates/review.md`

 * *Files identical despite different names*

### Comparing `autoreviewer-0.0.4/src/autoreviewer/utils.py` & `autoreviewer-0.0.5/src/autoreviewer/utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 """Utilities."""
 
 import hashlib
 import json
+import shutil
 import subprocess
 from contextlib import redirect_stderr, redirect_stdout
 from functools import lru_cache
 from pathlib import Path
+from textwrap import dedent
 from typing import Any, Optional
 
 import pystow
 import requests
 from pyroma import projectdata, ratings
 from ratelimit import rate_limited
 from tqdm import tqdm
@@ -36,15 +38,31 @@
     params: Optional[dict[str, Any]] = None,
     token: str | None = None,
 ) -> requests.Response:
     """Request an endpoint from the GitHub API."""
     if token is None:
         # Load the GitHub access token via PyStow. We'll
         # need it, so we don't hit the rate limit
-        token = pystow.get_config("github", "token", raise_on_missing=True)
+        try:
+            token = pystow.get_config("github", "token", raise_on_missing=True)
+        except pystow.config_api.ConfigError as e:
+            msg = dedent(
+                """\
+
+            You'll need to get a GitHub Personal Access Token using the following tutorial:
+            https://docs.github.com/en/authentication/keeping-your-account-and-data-secure/managing-your-personal-access-tokens
+
+            Then, you'll need to set it in a place where PyStow can read it.
+            Here's the information from the configuration error above:
+
+            {}
+            """
+            ).format(e)
+            raise ValueError(msg)
+
     headers = {
         "Authorization": f"token {token}",
     }
     if accept:
         headers["Accept"] = accept
     return requests.get(url, headers=headers, params=params)
 
@@ -62,73 +80,89 @@
     return res_json
 
 
 ResTup = tuple[str, str] | tuple[None, None]
 
 
 def get_file(
-    repo: str, name: str | list[str], *, branch: str = "main", desc: str | None = None
+    owner: str,
+    repo: str,
+    filenames: str | list[str],
+    *,
+    branch: str = "main",
+    desc: str | None = None,
 ) -> ResTup:
     """Get the file name and text, if available."""
-    if isinstance(name, str):
-        name = [name]
+    if isinstance(filenames, str):
+        filenames = [filenames]
 
-    owner, repo_name = repo.split("/")
-    directory = pystow.join("github", owner, repo_name)
+    directory = pystow.join("github", owner, repo)
     if directory.exists() and any(directory.iterdir()):
-        for n in name:
-            p = directory.joinpath(n)
+        for filename in filenames:
+            p = directory.joinpath(filename)
             if p.is_file():
-                return n, p.read_text()
+                return filename, p.read_text()
         return None, None
 
-    base_url = f"https://raw.githubusercontent.com/{repo}/{branch}"
-    for n in tqdm(name, leave=False, desc=desc, disable=True):
-        url = f"{base_url}/{n}"
+    base_url = f"https://raw.githubusercontent.com/{owner}/{repo}/{branch}"
+    for filename in tqdm(filenames, leave=False, desc=desc, disable=True):
+        url = f"{base_url}/{filename}"
         with logging_redirect_tqdm():
             res = requests.get(
                 url, timeout=1
             )  # timeout is short since these are small, simple files
         if res.status_code == 200:
-            return n, res.text
+            return filename, res.text
     return None, None
 
 
 @lru_cache
-def get_readme(repo: str, branch: str = "main") -> ResTup:
+def get_readme(owner: str, repo: str, branch: str = "main") -> ResTup:
     """Get the readme file name and text, if available."""
     return get_file(
-        repo, branch=branch, name=["README.md", "README.rst", "README.txt"], desc="Finding README"
+        owner,
+        repo,
+        branch=branch,
+        filenames=["README.md", "README.rst", "README.txt"],
+        desc="Finding README",
     )
 
 
 @lru_cache
-def get_setup_config(repo: str, branch: str = "main") -> ResTup:
+def get_setup_config(owner: str, repo: str, branch: str = "main") -> ResTup:
     """Get the setup configuration file name and text, if available."""
     return get_file(
+        owner,
         repo,
         branch=branch,
-        name=["setup.cfg", "setup.py", "pyproject.toml"],
+        filenames=["setup.cfg", "setup.py", "pyproject.toml"],
         desc="Finding setup conf.",
     )
 
 
 @lru_cache
-def get_license_file(repo: str, branch: str = "main") -> ResTup:
+def get_license_file(owner: str, repo: str, branch: str = "main") -> ResTup:
     """Get the license file name and text, if available."""
     return get_file(
-        repo, branch=branch, name=["LICENSE", "LICENSE.md", "LICENSE.rst"], desc="Finding license"
+        owner,
+        repo,
+        branch=branch,
+        filenames=["LICENSE", "LICENSE.md", "LICENSE.rst"],
+        desc="Finding license",
     )
 
 
-def get_repo_path(owner: str, repo: str) -> Path | None:
+def get_repo_path(owner: str, repo: str, *, cache: bool = True) -> Path | None:
     """Clone a repository from GitHub locally inside the PyStow folder."""
     directory = pystow.join("github", owner, repo)
     if directory.is_dir():
-        if any(directory.iterdir()):  # check not empty
+        if not cache:
+            # Delete the directory and start over
+            shutil.rmtree(directory)
+        elif any(directory.iterdir()):  # check not empty
             return directory
     url = f"https://github.com/{owner}/{repo}"
     try:
         subprocess.check_call(["git", "clone", "--depth", "1", url, directory.as_posix()])
     except subprocess.CalledProcessError:
         return None
     return directory
```

### Comparing `autoreviewer-0.0.4/src/autoreviewer/version.py` & `autoreviewer-0.0.5/src/autoreviewer/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 __all__ = [
     "VERSION",
     "get_version",
     "get_git_hash",
 ]
 
-VERSION = "0.0.4"
+VERSION = "0.0.5"
 
 
 def get_git_hash() -> str:
     """Get the :mod:`autoreviewer` git hash."""
     with open(os.devnull, "w") as devnull:
         try:
             ret = check_output(  # noqa: S603,S607
```

### Comparing `autoreviewer-0.0.4/src/autoreviewer.egg-info/PKG-INFO` & `autoreviewer-0.0.5/src/autoreviewer.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autoreviewer
-Version: 0.0.4
+Version: 0.0.5
 Summary: Automate scientific software review
 Home-page: https://github.com/cthoyt/autoreviewer
 Download-URL: https://github.com/cthoyt/autoreviewer/releases
 Author: Charles Tapley Hoyt
 Author-email: cthoyt@gmail.com
 Maintainer: Charles Tapley Hoyt
 Maintainer-email: cthoyt@gmail.com
@@ -19,14 +19,15 @@
 Classifier: Operating System :: OS Independent
 Classifier: Framework :: Pytest
 Classifier: Framework :: tox
 Classifier: Framework :: Sphinx
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: more_itertools
 Requires-Dist: tqdm
 Requires-Dist: click
@@ -34,15 +35,15 @@
 Requires-Dist: jinja2
 Requires-Dist: ebooklib
 Requires-Dist: requests
 Requires-Dist: pandas
 Requires-Dist: dateutils
 Requires-Dist: beautifulsoup4
 Requires-Dist: tabulate
-Requires-Dist: pystow
+Requires-Dist: pystow>=0.5.4
 Requires-Dist: ratelimit
 Requires-Dist: black
 Requires-Dist: pyroma
 Provides-Extra: tests
 Requires-Dist: pytest; extra == "tests"
 Requires-Dist: coverage; extra == "tests"
 Provides-Extra: docs
```

#### html2text {}

```diff
@@ -1,31 +1,32 @@
-Metadata-Version: 2.1 Name: autoreviewer Version: 0.0.4 Summary: Automate
+Metadata-Version: 2.1 Name: autoreviewer Version: 0.0.5 Summary: Automate
 scientific software review Home-page: https://github.com/cthoyt/autoreviewer
 Download-URL: https://github.com/cthoyt/autoreviewer/releases Author: Charles
 Tapley Hoyt Author-email: cthoyt@gmail.com Maintainer: Charles Tapley Hoyt
 Maintainer-email: cthoyt@gmail.com License: MIT Project-URL: Bug Tracker,
 https://github.com/cthoyt/autoreviewer/issues Project-URL: Source Code, https:/
 /github.com/cthoyt/autoreviewer Keywords: snekpack,cookiecutter Classifier:
 Development Status :: 1 - Planning Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers Classifier: License :: OSI Approved
 :: MIT License Classifier: Operating System :: OS Independent Classifier:
 Framework :: Pytest Classifier: Framework :: tox Classifier: Framework ::
 Sphinx Classifier: Programming Language :: Python Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3 :: Only Requires-Python: >=3.10
-Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
-more_itertools Requires-Dist: tqdm Requires-Dist: click Requires-Dist:
-more_click Requires-Dist: jinja2 Requires-Dist: ebooklib Requires-Dist:
-requests Requires-Dist: pandas Requires-Dist: dateutils Requires-Dist:
-beautifulsoup4 Requires-Dist: tabulate Requires-Dist: pystow Requires-Dist:
-ratelimit Requires-Dist: black Requires-Dist: pyroma Provides-Extra: tests
-Requires-Dist: pytest; extra == "tests" Requires-Dist: coverage; extra ==
-"tests" Provides-Extra: docs Requires-Dist: sphinx; extra == "docs" Requires-
-Dist: sphinx-rtd-theme; extra == "docs" Requires-Dist: sphinx-click; extra ==
-"docs" Requires-Dist: sphinx_automodapi; extra == "docs"
+Classifier: Programming Language :: Python :: 3.12 Classifier: Programming
+Language :: Python :: 3 :: Only Requires-Python: >=3.10 Description-Content-
+Type: text/markdown License-File: LICENSE Requires-Dist: more_itertools
+Requires-Dist: tqdm Requires-Dist: click Requires-Dist: more_click Requires-
+Dist: jinja2 Requires-Dist: ebooklib Requires-Dist: requests Requires-Dist:
+pandas Requires-Dist: dateutils Requires-Dist: beautifulsoup4 Requires-Dist:
+tabulate Requires-Dist: pystow>=0.5.4 Requires-Dist: ratelimit Requires-Dist:
+black Requires-Dist: pyroma Provides-Extra: tests Requires-Dist: pytest; extra
+== "tests" Requires-Dist: coverage; extra == "tests" Provides-Extra: docs
+Requires-Dist: sphinx; extra == "docs" Requires-Dist: sphinx-rtd-theme; extra
+== "docs" Requires-Dist: sphinx-click; extra == "docs" Requires-Dist:
+sphinx_automodapi; extra == "docs"
                           ************ AAuuttooRReevviieewweerr ************
   _[_T_e_s_t_s_]_[_P_y_P_I_]_[_P_y_P_I_ _-_ _P_y_t_h_o_n_ _V_e_r_s_i_o_n_]_[_P_y_P_I_ _-_ _L_i_c_e_n_s_e_]_[_D_o_c_u_m_e_n_t_a_t_i_o_n_ _S_t_a_t_u_s_]
     _[_C_o_d_e_c_o_v_ _s_t_a_t_u_s_]_[_C_o_o_k_i_e_c_u_t_t_e_r_ _t_e_m_p_l_a_t_e_ _f_r_o_m_ _@_c_t_h_o_y_t_]_[_C_o_d_e_ _s_t_y_l_e_:_ _b_l_a_c_k_]
                             _[_C_o_n_t_r_i_b_u_t_o_r_ _C_o_v_e_n_a_n_t_]
 Scientists often do the same bad stuff. Automate giving feedback during peer
 review for Python packages. Goals: 1. Given a GitHub repository, automate
 finding common issues such as - No setup.py/setup.cfg/pyproject.toml - No
```

### Comparing `autoreviewer-0.0.4/src/autoreviewer.egg-info/SOURCES.txt` & `autoreviewer-0.0.5/src/autoreviewer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

