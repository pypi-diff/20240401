# Comparing `tmp/coursebox-0.1.8.tar.gz` & `tmp/coursebox-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "coursebox-0.1.8.tar", last modified: Fri Aug 12 09:55:01 2022, max compression
+gzip compressed data, was "coursebox-0.1.9.tar", last modified: Mon Jan  2 11:48:28 2023, max compression
```

## Comparing `coursebox-0.1.8.tar` & `coursebox-0.1.9.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxrwx   0        0        0        0 2022-08-12 09:55:01.798870 coursebox-0.1.8/
--rw-rw-rw-   0        0        0     1091 2022-08-12 08:38:24.000000 coursebox-0.1.8/LICENSE
--rw-rw-rw-   0        0        0     1643 2022-08-12 09:55:01.795870 coursebox-0.1.8/PKG-INFO
--rw-rw-rw-   0        0        0     1096 2022-08-12 08:38:24.000000 coursebox-0.1.8/README.md
--rw-rw-rw-   0        0        0      108 2022-08-12 08:38:24.000000 coursebox-0.1.8/pyproject.toml
--rw-rw-rw-   0        0        0       42 2022-08-12 09:55:01.800866 coursebox-0.1.8/setup.cfg
--rw-rw-rw-   0        0        0     1195 2022-08-12 09:54:22.000000 coursebox-0.1.8/setup.py
-drwxrwxrwx   0        0        0        0 2022-08-12 09:55:01.644246 coursebox-0.1.8/src/
-drwxrwxrwx   0        0        0        0 2022-08-12 09:55:01.685155 coursebox-0.1.8/src/coursebox/
--rw-rw-rw-   0        0        0      162 2022-08-12 08:38:24.000000 coursebox-0.1.8/src/coursebox/__init__.py
-drwxrwxrwx   0        0        0        0 2022-08-12 09:55:01.744997 coursebox-0.1.8/src/coursebox/book/
--rw-rw-rw-   0        0        0        0 2022-08-12 08:38:24.000000 coursebox-0.1.8/src/coursebox/book/__init__.py
--rw-rw-rw-   0        0        0    10717 2022-08-12 08:38:24.000000 coursebox-0.1.8/src/coursebox/book/exam_includer.py
-drwxrwxrwx   0        0        0        0 2022-08-12 09:55:01.774923 coursebox-0.1.8/src/coursebox/core/
--rw-rw-rw-   0        0        0        0 2022-08-12 08:38:24.000000 coursebox-0.1.8/src/coursebox/core/__init__.py
--rw-rw-rw-   0        0        0    13454 2022-08-12 08:38:24.000000 coursebox-0.1.8/src/coursebox/core/info.py
--rw-rw-rw-   0        0        0     4449 2022-08-12 08:53:33.000000 coursebox-0.1.8/src/coursebox/core/info_paths.py
--rw-rw-rw-   0        0        0    32911 2022-08-12 08:38:24.000000 coursebox-0.1.8/src/coursebox/core/projects.py
--rw-rw-rw-   0        0        0     9484 2022-08-12 08:38:24.000000 coursebox-0.1.8/src/coursebox/core/projects_info.py
--rw-rw-rw-   0        0        0     4497 2022-08-12 08:38:24.000000 coursebox-0.1.8/src/coursebox/core/projects_plagiarism.py
-drwxrwxrwx   0        0        0        0 2022-08-12 09:55:01.792882 coursebox-0.1.8/src/coursebox/material/
--rw-rw-rw-   0        0        0        0 2022-08-12 08:38:24.000000 coursebox-0.1.8/src/coursebox/material/__init__.py
--rw-rw-rw-   0        0        0    24127 2022-08-12 08:38:24.000000 coursebox-0.1.8/src/coursebox/material/homepage_lectures_exercises.py
--rw-rw-rw-   0        0        0     7385 2022-08-12 08:38:24.000000 coursebox-0.1.8/src/coursebox/material/lecture_questions.py
--rw-rw-rw-   0        0        0    17240 2022-08-12 08:38:24.000000 coursebox-0.1.8/src/coursebox/material/snipper.py
--rw-rw-rw-   0        0        0      975 2022-08-12 08:38:24.000000 coursebox-0.1.8/src/coursebox/setup_coursebox.py
--rw-rw-rw-   0        0        0     4136 2022-08-12 09:01:59.000000 coursebox-0.1.8/src/coursebox/thtools_base.py
-drwxrwxrwx   0        0        0        0 2022-08-12 09:55:01.741006 coursebox-0.1.8/src/coursebox.egg-info/
--rw-rw-rw-   0        0        0     1643 2022-08-12 09:55:01.000000 coursebox-0.1.8/src/coursebox.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      748 2022-08-12 09:55:01.000000 coursebox-0.1.8/src/coursebox.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-08-12 09:55:01.000000 coursebox-0.1.8/src/coursebox.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       86 2022-08-12 09:55:01.000000 coursebox-0.1.8/src/coursebox.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2022-08-12 09:55:01.000000 coursebox-0.1.8/src/coursebox.egg-info/top_level.txt
+drwxrwxr-x   0 tuhe      (1001) tuhe      (1001)        0 2023-01-02 11:48:28.311516 coursebox-0.1.9/
+-rw-rw-r--   0 tuhe      (1001) tuhe      (1001)     1073 2023-01-02 11:37:34.000000 coursebox-0.1.9/LICENSE
+-rw-rw-r--   0 tuhe      (1001) tuhe      (1001)     1596 2023-01-02 11:48:28.311516 coursebox-0.1.9/PKG-INFO
+-rw-rw-r--   0 tuhe      (1001) tuhe      (1001)     1066 2023-01-02 11:37:34.000000 coursebox-0.1.9/README.md
+-rw-rw-r--   0 tuhe      (1001) tuhe      (1001)      103 2023-01-02 11:37:34.000000 coursebox-0.1.9/pyproject.toml
+-rw-rw-r--   0 tuhe      (1001) tuhe      (1001)       38 2023-01-02 11:48:28.311516 coursebox-0.1.9/setup.cfg
+-rw-rw-r--   0 tuhe      (1001) tuhe      (1001)     1223 2023-01-02 11:47:08.000000 coursebox-0.1.9/setup.py
+drwxrwxr-x   0 tuhe      (1001) tuhe      (1001)        0 2023-01-02 11:48:28.307516 coursebox-0.1.9/src/
+drwxrwxr-x   0 tuhe      (1001) tuhe      (1001)        0 2023-01-02 11:48:28.307516 coursebox-0.1.9/src/coursebox/
+-rw-rw-r--   0 tuhe      (1001) tuhe      (1001)      156 2023-01-02 11:37:34.000000 coursebox-0.1.9/src/coursebox/__init__.py
+drwxrwxr-x   0 tuhe      (1001) tuhe      (1001)        0 2023-01-02 11:48:28.311516 coursebox-0.1.9/src/coursebox/book/
+-rw-rw-r--   0 tuhe      (1001) tuhe      (1001)        0 2023-01-02 11:37:34.000000 coursebox-0.1.9/src/coursebox/book/__init__.py
+-rw-rw-r--   0 tuhe      (1001) tuhe      (1001)    10448 2023-01-02 11:37:34.000000 coursebox-0.1.9/src/coursebox/book/exam_includer.py
+drwxrwxr-x   0 tuhe      (1001) tuhe      (1001)        0 2023-01-02 11:48:28.311516 coursebox-0.1.9/src/coursebox/core/
+-rw-rw-r--   0 tuhe      (1001) tuhe      (1001)        0 2023-01-02 11:37:34.000000 coursebox-0.1.9/src/coursebox/core/__init__.py
+-rw-rw-r--   0 tuhe      (1001) tuhe      (1001)    13091 2023-01-02 11:37:34.000000 coursebox-0.1.9/src/coursebox/core/info.py
+-rw-rw-r--   0 tuhe      (1001) tuhe      (1001)     4348 2023-01-02 11:37:34.000000 coursebox-0.1.9/src/coursebox/core/info_paths.py
+-rw-rw-r--   0 tuhe      (1001) tuhe      (1001)    32147 2023-01-02 11:37:34.000000 coursebox-0.1.9/src/coursebox/core/projects.py
+-rw-rw-r--   0 tuhe      (1001) tuhe      (1001)     9243 2023-01-02 11:43:58.000000 coursebox-0.1.9/src/coursebox/core/projects_info.py
+-rw-rw-r--   0 tuhe      (1001) tuhe      (1001)     4358 2023-01-02 11:37:34.000000 coursebox-0.1.9/src/coursebox/core/projects_plagiarism.py
+drwxrwxr-x   0 tuhe      (1001) tuhe      (1001)        0 2023-01-02 11:48:28.311516 coursebox-0.1.9/src/coursebox/material/
+-rw-rw-r--   0 tuhe      (1001) tuhe      (1001)        0 2023-01-02 11:37:34.000000 coursebox-0.1.9/src/coursebox/material/__init__.py
+-rw-rw-r--   0 tuhe      (1001) tuhe      (1001)    23502 2023-01-02 11:37:34.000000 coursebox-0.1.9/src/coursebox/material/homepage_lectures_exercises.py
+-rw-rw-r--   0 tuhe      (1001) tuhe      (1001)     7204 2023-01-02 11:37:34.000000 coursebox-0.1.9/src/coursebox/material/lecture_questions.py
+-rw-rw-r--   0 tuhe      (1001) tuhe      (1001)    16779 2023-01-02 11:37:34.000000 coursebox-0.1.9/src/coursebox/material/snipper.py
+-rw-rw-r--   0 tuhe      (1001) tuhe      (1001)      955 2023-01-02 11:37:34.000000 coursebox-0.1.9/src/coursebox/setup_coursebox.py
+-rw-rw-r--   0 tuhe      (1001) tuhe      (1001)     3982 2023-01-02 11:37:34.000000 coursebox-0.1.9/src/coursebox/thtools_base.py
+drwxrwxr-x   0 tuhe      (1001) tuhe      (1001)        0 2023-01-02 11:48:28.307516 coursebox-0.1.9/src/coursebox.egg-info/
+-rw-rw-r--   0 tuhe      (1001) tuhe      (1001)     1596 2023-01-02 11:48:28.000000 coursebox-0.1.9/src/coursebox.egg-info/PKG-INFO
+-rw-rw-r--   0 tuhe      (1001) tuhe      (1001)      748 2023-01-02 11:48:28.000000 coursebox-0.1.9/src/coursebox.egg-info/SOURCES.txt
+-rw-rw-r--   0 tuhe      (1001) tuhe      (1001)        1 2023-01-02 11:48:28.000000 coursebox-0.1.9/src/coursebox.egg-info/dependency_links.txt
+-rw-rw-r--   0 tuhe      (1001) tuhe      (1001)       86 2023-01-02 11:48:28.000000 coursebox-0.1.9/src/coursebox.egg-info/requires.txt
+-rw-rw-r--   0 tuhe      (1001) tuhe      (1001)       10 2023-01-02 11:48:28.000000 coursebox-0.1.9/src/coursebox.egg-info/top_level.txt
```

### Comparing `coursebox-0.1.8/LICENSE` & `coursebox-0.1.9/LICENSE`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-Copyright (c) 2018 The Python Packaging Authority
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+Copyright (c) 2018 The Python Packaging Authority
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
```

### Comparing `coursebox-0.1.8/PKG-INFO` & `coursebox-0.1.9/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,47 +1,47 @@
-Metadata-Version: 2.1
-Name: coursebox
-Version: 0.1.8
-Summary: A course management system currently used at DTU
-Home-page: https://lab.compute.dtu.dk/tuhe/coursebox
-Author: Tue Herlau
-Author-email: tuhe@dtu.dk
-License: MIT
-Project-URL: Bug Tracker, https://lab.compute.dtu.dk/tuhe/coursebox/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# Coursebox DTU
-DTU course management software.
-
-## Installation
-```terminal
-pip install coursebox
-```
-## What it can do 
- - Single semester-dependent configuration file
- - Integrates with DTU Inside/DTU Learn
- - Distribution/evalauation of project reports in Learn-compatible format
- - Quiz-generation in DTU Learn/Beamer friendly format
- - Automatic website/syllabus generation 
- - Automatic generation of lectures handouts/exercises (you don't have to track dynamic content like dates/lecture titles; it is all in the configuration)
- - Easy compilation to 2/5 day formats (Continuous education)
-
-## Usage
-Coursebox requires a specific directory structure. It is easier to start with an existing course and adapt to your needs. Please contact me at tuhe@dtu.dk for more information.
-
-## Citing
-```bibtex
-@online{coursebox,
-	title={Coursebox (0.1.1): \texttt{pip install coursebox}},
-	url={https://lab.compute.dtu.dk/tuhe/coursebox},
-	urldate = {2021-09-07}, 
-	month={9},
-	publisher={Technical University of Denmark (DTU)},
-	author={Tue Herlau},
-	year={2021},
-}
-```
+Metadata-Version: 2.1
+Name: coursebox
+Version: 0.1.9
+Summary: A course management system currently used at DTU
+Home-page: https://lab.compute.dtu.dk/tuhe/coursebox
+Author: Tue Herlau
+Author-email: tuhe@dtu.dk
+License: MIT
+Project-URL: Bug Tracker, https://lab.compute.dtu.dk/tuhe/coursebox/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# Coursebox DTU
+DTU course management software.
+
+## Installation
+```terminal
+pip install coursebox
+```
+## What it can do 
+ - Single semester-dependent configuration file
+ - Integrates with DTU Inside/DTU Learn
+ - Distribution/evalauation of project reports in Learn-compatible format
+ - Quiz-generation in DTU Learn/Beamer friendly format
+ - Automatic website/syllabus generation 
+ - Automatic generation of lectures handouts/exercises (you don't have to track dynamic content like dates/lecture titles; it is all in the configuration)
+ - Easy compilation to 2/5 day formats (Continuous education)
+
+## Usage
+Coursebox requires a specific directory structure. It is easier to start with an existing course and adapt to your needs. Please contact me at tuhe@dtu.dk for more information.
+
+## Citing
+```bibtex
+@online{coursebox,
+	title={Coursebox (0.1.1): \texttt{pip install coursebox}},
+	url={https://lab.compute.dtu.dk/tuhe/coursebox},
+	urldate = {2021-09-07}, 
+	month={9},
+	publisher={Technical University of Denmark (DTU)},
+	author={Tue Herlau},
+	year={2021},
+}
+```
```

### Comparing `coursebox-0.1.8/README.md` & `coursebox-0.1.9/README.md`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,31 +1,31 @@
-# Coursebox DTU
-DTU course management software.
-
-## Installation
-```terminal
-pip install coursebox
-```
-## What it can do 
- - Single semester-dependent configuration file
- - Integrates with DTU Inside/DTU Learn
- - Distribution/evalauation of project reports in Learn-compatible format
- - Quiz-generation in DTU Learn/Beamer friendly format
- - Automatic website/syllabus generation 
- - Automatic generation of lectures handouts/exercises (you don't have to track dynamic content like dates/lecture titles; it is all in the configuration)
- - Easy compilation to 2/5 day formats (Continuous education)
-
-## Usage
-Coursebox requires a specific directory structure. It is easier to start with an existing course and adapt to your needs. Please contact me at tuhe@dtu.dk for more information.
-
-## Citing
-```bibtex
-@online{coursebox,
-	title={Coursebox (0.1.1): \texttt{pip install coursebox}},
-	url={https://lab.compute.dtu.dk/tuhe/coursebox},
-	urldate = {2021-09-07}, 
-	month={9},
-	publisher={Technical University of Denmark (DTU)},
-	author={Tue Herlau},
-	year={2021},
-}
+# Coursebox DTU
+DTU course management software.
+
+## Installation
+```terminal
+pip install coursebox
+```
+## What it can do 
+ - Single semester-dependent configuration file
+ - Integrates with DTU Inside/DTU Learn
+ - Distribution/evalauation of project reports in Learn-compatible format
+ - Quiz-generation in DTU Learn/Beamer friendly format
+ - Automatic website/syllabus generation 
+ - Automatic generation of lectures handouts/exercises (you don't have to track dynamic content like dates/lecture titles; it is all in the configuration)
+ - Easy compilation to 2/5 day formats (Continuous education)
+
+## Usage
+Coursebox requires a specific directory structure. It is easier to start with an existing course and adapt to your needs. Please contact me at tuhe@dtu.dk for more information.
+
+## Citing
+```bibtex
+@online{coursebox,
+	title={Coursebox (0.1.1): \texttt{pip install coursebox}},
+	url={https://lab.compute.dtu.dk/tuhe/coursebox},
+	urldate = {2021-09-07}, 
+	month={9},
+	publisher={Technical University of Denmark (DTU)},
+	author={Tue Herlau},
+	year={2021},
+}
 ```
```

### Comparing `coursebox-0.1.8/setup.py` & `coursebox-0.1.9/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,34 +1,38 @@
-# Use this guide:
-# https://packaging.python.org/tutorials/packaging-projects/
-# Use pipreqs.exe to get requirements list.
-# py -m build && twine upload dist/*
-
-import setuptools
-import pkg_resources
-
-with open("README.md", "r", encoding="utf-8") as fh:
-    long_description = fh.read()
-# beamer-slider
-setuptools.setup(
-    name="coursebox",
-    version="0.1.8",
-    author="Tue Herlau",
-    author_email="tuhe@dtu.dk",
-    description="A course management system currently used at DTU",
-    long_description=long_description,
-    long_description_content_type="text/markdown",
-    license="MIT",
-    url='https://lab.compute.dtu.dk/tuhe/coursebox',
-    project_urls={
-        "Bug Tracker": "https://lab.compute.dtu.dk/tuhe/coursebox/issues",
-    },
-    classifiers=[
-        "Programming Language :: Python :: 3",
-        "License :: OSI Approved :: MIT License",
-        "Operating System :: OS Independent",
-    ],
-    package_dir={"": "src"},
-    packages=setuptools.find_packages(where="src"),
-    python_requires=">=3.8",
-    install_requires=['numpy','pycode_similar','tika','openpyxl', 'xlwings','matplotlib','langdetect','beamer-slider','tinydb'],
-)
+# Use this guide:
+# https://packaging.python.org/tutorials/packaging-projects/
+# Use pipreqs.exe to get requirements list.
+"""
+Windows> py -m build && twine upload dist/*
+Linux> python -m build && twine upload dist/*
+
+"""
+
+import setuptools
+import pkg_resources
+
+with open("README.md", "r", encoding="utf-8") as fh:
+    long_description = fh.read()
+# beamer-slider
+setuptools.setup(
+    name="coursebox",
+    version="0.1.9",
+    author="Tue Herlau",
+    author_email="tuhe@dtu.dk",
+    description="A course management system currently used at DTU",
+    long_description=long_description,
+    long_description_content_type="text/markdown",
+    license="MIT",
+    url='https://lab.compute.dtu.dk/tuhe/coursebox',
+    project_urls={
+        "Bug Tracker": "https://lab.compute.dtu.dk/tuhe/coursebox/issues",
+    },
+    classifiers=[
+        "Programming Language :: Python :: 3",
+        "License :: OSI Approved :: MIT License",
+        "Operating System :: OS Independent",
+    ],
+    package_dir={"": "src"},
+    packages=setuptools.find_packages(where="src"),
+    python_requires=">=3.8",
+    install_requires=['numpy','pycode_similar','tika','openpyxl', 'xlwings','matplotlib','langdetect','beamer-slider','tinydb'],
+)
```

### Comparing `coursebox-0.1.8/src/coursebox/book/exam_includer.py` & `coursebox-0.1.9/src/coursebox/book/exam_includer.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,270 +1,270 @@
-# -*- coding: utf-8 -*-
-import shutil
-import os
-import re
-import ntpath
-import glob
-
-
-CDIR = os.path.dirname(os.path.realpath(__file__))
-CDIR = CDIR.replace('\\','/')
-os.chdir(CDIR)
-OUTPUT_TEX_BASE = CDIR + "/../Latex/Exams"
-
-nm = []
-def rec_input(fname) :
-    f = open(fname, "r")
-    dirname = os.path.dirname(fname)    
-    cc = f.readlines()
-    f.close()
-    for i in range(len(cc)):
-        m = re.search(r'\\input{([^}]*)\}', cc[i])
-        if m :
-            s = m.group(0)
-            fname2 = dirname + '/' + s[s.index('{')+1:s.index('}')]
-            xx, file_extension = os.path.splitext(fname2)     
-            if file_extension == ".tex" :
-                None
-            else:
-                fname2 = fname2 + ".tex"
-                            
-            s = rec_input(fname2)
-            cc[i] = s
-    
-    for (i,sc) in enumerate(cc) : 
-        if len(sc) >= 2 and sc[-2:] == '%\n' and not (len(sc) >= 3 and sc[-3:] == "\\%\n"): cc[i] = sc[:-2]
-    return ''.join(cc)
-
-
-def getgroups(s2,gstart,IncludeTags = False) : 
-    qs = [];
-    i2 = 0
-    while True :    
-        t1 = '\\begin{'+gstart+'}'
-        t2 = '\\end{'+gstart+'}'
-        i1 = s2.find(t1,i2)
-        if i1 < 0 : break
-        i2 = s2.find(t2,i1)        
-        
-        if IncludeTags :
-            d1 = 0
-            d2 = len(t2)
-        else:
-            d1 = len(t1)
-            d2 = 0
-        
-        s = s2[i1+d1:i2+d2] 
-        refs = tagfind(s,'ref')
-        refs = refs + tagfind(s,'cref')
-        
-        labels = tagfind(s,'label')        
-        if not labels : labels = [['','']]
-        
-        qs.append( [s.strip(),refs,labels] )
-    return qs
-    
-def tagfind(s,tag) :
-    tags = []
-    cp = re.compile(r'\\'+tag+'{(\S*)}')
-    for i in cp.finditer(s) : 
-        tags.append( [i.group(1), i.group(0)] ) 
-    return tags
-   
-def process_figures(fs, PREFIX, INPUT_TEX_BASE) :
-    fs = re.sub(r'\\begin{figure(}.*)', r'\\begin{figure}[H]',fs)
-    fs = re.sub(r'\\begin{table(}.*)', r'\\begin{table}[H]',fs)
-    rm = re.finditer(r'\\includegraphics(.*){([^}]*)}', fs)
-    fig_files = [] 
-    for i in rm : 
-        tex_source_name = i.groups(1)[1]
-        sourcefile = INPUT_TEX_BASE + tex_source_name.strip()
-        tex_dest_name = PREFIX+ntpath.basename(sourcefile)                  
-        fnc = glob.glob(sourcefile) + glob.glob(sourcefile+".pdf")+glob.glob(sourcefile+".png")
-        
-        sourcefile = fnc[0]        
-        xx, file_extension = os.path.splitext(sourcefile)                
-        
-        destfile = OUTPUT_TEX_BASE + "/"+tex_dest_name
-        if destfile.find(file_extension) < 0 : destfile = destfile+file_extension     
-        
-        fs = re.sub(r'\\includegraphics(.*){'+tex_source_name+'}', r'\\includegraphics\1{Exams/'+tex_dest_name+'}',fs)
-        fig_files.append([sourcefile,destfile])
-        
-        shutil.copy(sourcefile,destfile)
-    return fs
-    
-def process_question(PREFIX,INPUT_TEX_BASE,s2,question_number,figures_included) :
-    s2 = s2 + " "
-    Qs = getgroups(s2,'question')
-    Ts = getgroups(s2,'table',True)
-    Fs = getgroups(s2,'figure',True)
-    Eqs = getgroups(s2,'equation',True)
-    Als = getgroups(s2,'align',True)    
-    ELEMENTS = Ts + Fs + Eqs + Als
-    
-    pfix = []
-    eleminc = []
-    q = Qs[question_number-1]
-    referenced_labels = [r[0] for r in q[1]] # labels which we reference.         
-    referenced_labels = list(set(referenced_labels))
-    for rname in referenced_labels : 
-        pfix.append(rname)       
-        included_labels = [PREFIX + ll[0] for ll in q[2]]  + figures_included 
-        #print included_labels
-        if (PREFIX+rname) not in included_labels :                                 
-            l = [e[0] for e in ELEMENTS if e[2][0][0] == rname]   
-            eleminc.append(l[0])        
-            
-    solution = getgroups(q[0],'solution')[0][0]
-    sanswer = getgroups(q[0],'answer')[0][0]
-    answer = int(sanswer[1:2])
-    sanswer = sanswer[3:]
-    sanswer = "\\begin{enumerate}[label=\\Alph*]" + sanswer + "\\end{enumerate}"
-    
-    question_text = q[0][0:q[0].find('\\begin{answer}')]
-    question_text = question_text.strip() + "\n" + '\n'.join(eleminc) + '\n'+sanswer.strip()
-        
-    question_text = process_figures(question_text,PREFIX,INPUT_TEX_BASE)
-    question_text = question_text.replace("\\thecorrect\\", "ABCD"[answer-1]+" ")
-    for pf in pfix:
-        question_text = question_text.replace('{'+pf+'}', '{'+PREFIX+pf+'}')
-        solution = solution.replace('{'+pf+'}', '{'+PREFIX+pf+'}')
-        
-    solution = solution.replace("\\thecorrect\\", "ABCD"[answer-1]+" ")    
-    figures_included = figures_included + [PREFIX + rl for rl in referenced_labels]
-    
-    FOUT = OUTPUT_TEX_BASE + "/"+PREFIX[0:6]+str(question_number)+".tex"
-    f = open(FOUT,'w')
-    f.write(question_text.strip())
-    f.close()
-    
-    FOUT = OUTPUT_TEX_BASE + "/"+PREFIX[0:6]+str(question_number)+"sol.tex"
-    f = open(FOUT,'w')
-    f.write(solution.strip())
-    f.close()
-    return [question_text,solution,answer,figures_included]
-
-
-EXAM_INCLUDES = [[] for i in range(20)]
-if True :
-    # viz, hist, box, distance, sims 
-    EXAM_INCLUDES[2] = ['f2011q1', 'f2013q1','f2014q1',]    
-    EXAM_INCLUDES[3] = ['s2012q4','f2011q2', 'f2013q3','f2014q3','f2014q4','s2014q3',]      # PCA
-    
-    EXAM_INCLUDES[4] = ['f2014q10', 's2013Q18', 'f2013q18']  # Data, norms, variance, correlation, percentile.
-    EXAM_INCLUDES[5] = ['f2014q8','s2013q17', 'f2013q15'] # Bayes
-    EXAM_INCLUDES[6] = ['f2012q2', 'f2014Q2', 's2014q1'] # Visualization
-    
-    EXAM_INCLUDES[7] = ['s2013Q12', 's2014Q5', 'f2013q6', 'f2013q17','f2014q22']  # log. regression     
-    EXAM_INCLUDES[8] = ['f2013q14','f2013q13','f2014q9','f2014q21'] # TREES     
-    
-    EXAM_INCLUDES[9] = ['f2014q27', 's2013q13', 's2013q14', 'f2013q7','f2013q16','f2014q6','f2013q25','f2014q18',]  # overfitting, fw selection
-    
-    EXAM_INCLUDES[10] = ['f2013q9','f2014q23','f2014q12'] # KNN methods
-    EXAM_INCLUDES[11] = ['f2015q16', 'f2015q17', 'f2013q19', 'f2014q15'] # bayesian methods (classifier) + NB.    
-
-    EXAM_INCLUDES[12] = ['s2013q26']  # bias-variance, regularization. # PROBLEMS!
-    EXAM_INCLUDES[13] = ['f2013q23','f2014q5', 'f2013q12','f2014q19', ] # neural networks
-    
-    EXAM_INCLUDES[14] = ['f2014q24','f2014q25',]  # AUC, statistics (CIs)
-    EXAM_INCLUDES[15] = ['f2014q26', 'f2013q24',] # ensemble methods boosting
-    
-    ## PART 3
-    # Lecture 10   
-    EXAM_INCLUDES[16] = ['f2013q8','f2014q20','f2014q11','f2012q12'] # kmeans, hierarchical agglom
-    
-    #Lecture 11
-    EXAM_INCLUDES[17] = ['f2013q22','f2013q26', 'f2014q7',]     # EM/GMM
-    EXAM_INCLUDES[18] = ['f2013q11', 's2013q9','f2011q27', 'f2013q20','f2013q10','f2014q13','f2014q14'] # Density estimation
-
-    # Lecture 12    
-    EXAM_INCLUDES[19] = ['s2014q11', 's2014q12'] # Association rule learning
-
-AE = [b for e in EXAM_INCLUDES for b in e]
-for e in AE : 
-    if len([j for j in AE if j == e]) > 1 : 
-        print(e)
-    
-HOMEWORK_PROBLEMS = [[] for i in range(len(EXAM_INCLUDES))]
-# BKOCK 1
-HOMEWORK_PROBLEMS[2]= [(3,1), (2,1), (3,2)] # basic data and PCA
-HOMEWORK_PROBLEMS[3]= [(4,1), (4,2), (4,3)] # Measures of similarity and summary statistics.
-HOMEWORK_PROBLEMS[4]= [(5,1), (5,2), (6,1)] # Visualization, probabilities
-
-# BLOCK 2
-HOMEWORK_PROBLEMS[5]= [(8,1), (7,1), (7,2)] # Lecture 5, reg+trees
-HOMEWORK_PROBLEMS[6]= [(9,1), (9,2), (9,3)] # Lecture 6, crossval 
-HOMEWORK_PROBLEMS[7]= [(11,1), (11,2), (10,1)] # Lecture 7, KNN+Bayes+Naive-bayes.
-HOMEWORK_PROBLEMS[8]= [(13,1), (13,2), (13,3)] # Lecture 8, Bias/Var + Artificial NN.
-HOMEWORK_PROBLEMS[9]= [(14,1), (14,2), (15,1)] # Lecture 9, classimb/AUC + Ensemble
-
-# BLOCK 3
-HOMEWORK_PROBLEMS[10]= [(16,1), (16,2), (16,3)] # Lecture 9, classimb/AUC + Ensemble
-
-HOMEWORK_PROBLEMS[11]= [(18,1), (17,1), (17,2)] # Lecture 9, classimb/AUC + Ensemble
-HOMEWORK_PROBLEMS[12]= [(19,1), (16,2), (16,3)] # Lecture 9, classimb/AUC + Ensemble
-
-EXAM_BASE_DIR = CDIR+ "/../../Exam/"
-EXAM_TEX_CONTENT = {} 
-
-rr = '''
-\\newpage \\newgeometry{left=\PLLEFT,right=\PLRIGHT,top=\PLTOP,bottom=\PLBOTTOM} \\begin{multicols}{2}
-\\section*{Problems} \\addcontentsline{toc}{section}{Problems}
-%s \\end{multicols}
-\\restoregeometry  \\newpage '''
-
-if __name__ == "__main__":
-    for chap,ae in enumerate(EXAM_INCLUDES):
-        allq = []
-        allsol = []
-        adex = 0
-        figs_included = []
-        nstrings = []
-        if not ae : continue
-        sas = []
-        for qsin in ae : 
-            sem = qsin[0]
-            year = qsin[1:5]
-            q = int(qsin[6:])   
-            
-            SEML = "Spring" if sem=="s" else "Fall"
-            nstrings.append("%s %s question %i"%(SEML,year,q) )
-            
-            INPUT_TEX_BASE = EXAM_BASE_DIR + ("Exam %s %s/latex/"%(SEML,year))
-            if not os.path.isdir(INPUT_TEX_BASE) :
-                INPUT_TEX_BASE = EXAM_BASE_DIR + ("Exam %s %s/02450Exam%s%s/latex/"%(SEML,year,SEML,year))
-                        
-            exam_tex_file = INPUT_TEX_BASE + ("02450ex_%s%s_book.tex"%(SEML,year))
-            
-            if not os.path.isfile(exam_tex_file) :
-                exam_tex_file = INPUT_TEX_BASE + ("02450ex_%s%s.tex"%(SEML,year))
-            
-            FIG_PREFIX = qsin[0:6] + "c"+str(chap)
-            
-            if not EXAM_TEX_CONTENT.has_key(FIG_PREFIX) : 
-                EXAM_TEX_CONTENT[FIG_PREFIX] = rec_input(exam_tex_file)
-            s2 = EXAM_TEX_CONTENT[FIG_PREFIX]
-            
-            [qtext,qsol,adex,fi] = process_question(FIG_PREFIX,INPUT_TEX_BASE,s2,q,figs_included)
-            figs_included = figs_included + fi
-            sa = 'ABCD'[adex-1]
-            sas.append(sa)
-            # write joint solution file and joint answer thingy
-        
-        cq = ['\\begin{prob}\\label{c%iprob%i}\\textbf{%s:} \n \\input{Exams/%s}\\end{prob}'%(chap,qn+1,nstrings[qn],qs) for (qn,qs) in enumerate(ae)]
-        cq = '\n'.join(cq)
-        
-        cs = ['\\begin{sol}{c%iprob%i}\\textbf{The correct answer is %s:} \\input{Exams/%ssol}\\end{sol}'%(chap,qn+1,sas[qn],qs) for (qn,qs) in enumerate(ae)]
-        cs = '\n'.join(cs)
-        
-        ss = rr%cq       
-        FOUT = OUTPUT_TEX_BASE + "/c%iprob.tex"%chap
-        f = open(FOUT,'w')
-        f.write(ss)
-        f.close()
-
-        FOUT = OUTPUT_TEX_BASE + "/c%isol.tex"%chap
-        f = open(FOUT,'w')
-        f.write(cs)
-        f.close()
+# -*- coding: utf-8 -*-
+import shutil
+import os
+import re
+import ntpath
+import glob
+
+
+CDIR = os.path.dirname(os.path.realpath(__file__))
+CDIR = CDIR.replace('\\','/')
+os.chdir(CDIR)
+OUTPUT_TEX_BASE = CDIR + "/../Latex/Exams"
+
+nm = []
+def rec_input(fname) :
+    f = open(fname, "r")
+    dirname = os.path.dirname(fname)    
+    cc = f.readlines()
+    f.close()
+    for i in range(len(cc)):
+        m = re.search(r'\\input{([^}]*)\}', cc[i])
+        if m :
+            s = m.group(0)
+            fname2 = dirname + '/' + s[s.index('{')+1:s.index('}')]
+            xx, file_extension = os.path.splitext(fname2)     
+            if file_extension == ".tex" :
+                None
+            else:
+                fname2 = fname2 + ".tex"
+                            
+            s = rec_input(fname2)
+            cc[i] = s
+    
+    for (i,sc) in enumerate(cc) : 
+        if len(sc) >= 2 and sc[-2:] == '%\n' and not (len(sc) >= 3 and sc[-3:] == "\\%\n"): cc[i] = sc[:-2]
+    return ''.join(cc)
+
+
+def getgroups(s2,gstart,IncludeTags = False) : 
+    qs = [];
+    i2 = 0
+    while True :    
+        t1 = '\\begin{'+gstart+'}'
+        t2 = '\\end{'+gstart+'}'
+        i1 = s2.find(t1,i2)
+        if i1 < 0 : break
+        i2 = s2.find(t2,i1)        
+        
+        if IncludeTags :
+            d1 = 0
+            d2 = len(t2)
+        else:
+            d1 = len(t1)
+            d2 = 0
+        
+        s = s2[i1+d1:i2+d2] 
+        refs = tagfind(s,'ref')
+        refs = refs + tagfind(s,'cref')
+        
+        labels = tagfind(s,'label')        
+        if not labels : labels = [['','']]
+        
+        qs.append( [s.strip(),refs,labels] )
+    return qs
+    
+def tagfind(s,tag) :
+    tags = []
+    cp = re.compile(r'\\'+tag+'{(\S*)}')
+    for i in cp.finditer(s) : 
+        tags.append( [i.group(1), i.group(0)] ) 
+    return tags
+   
+def process_figures(fs, PREFIX, INPUT_TEX_BASE) :
+    fs = re.sub(r'\\begin{figure(}.*)', r'\\begin{figure}[H]',fs)
+    fs = re.sub(r'\\begin{table(}.*)', r'\\begin{table}[H]',fs)
+    rm = re.finditer(r'\\includegraphics(.*){([^}]*)}', fs)
+    fig_files = [] 
+    for i in rm : 
+        tex_source_name = i.groups(1)[1]
+        sourcefile = INPUT_TEX_BASE + tex_source_name.strip()
+        tex_dest_name = PREFIX+ntpath.basename(sourcefile)                  
+        fnc = glob.glob(sourcefile) + glob.glob(sourcefile+".pdf")+glob.glob(sourcefile+".png")
+        
+        sourcefile = fnc[0]        
+        xx, file_extension = os.path.splitext(sourcefile)                
+        
+        destfile = OUTPUT_TEX_BASE + "/"+tex_dest_name
+        if destfile.find(file_extension) < 0 : destfile = destfile+file_extension     
+        
+        fs = re.sub(r'\\includegraphics(.*){'+tex_source_name+'}', r'\\includegraphics\1{Exams/'+tex_dest_name+'}',fs)
+        fig_files.append([sourcefile,destfile])
+        
+        shutil.copy(sourcefile,destfile)
+    return fs
+    
+def process_question(PREFIX,INPUT_TEX_BASE,s2,question_number,figures_included) :
+    s2 = s2 + " "
+    Qs = getgroups(s2,'question')
+    Ts = getgroups(s2,'table',True)
+    Fs = getgroups(s2,'figure',True)
+    Eqs = getgroups(s2,'equation',True)
+    Als = getgroups(s2,'align',True)    
+    ELEMENTS = Ts + Fs + Eqs + Als
+    
+    pfix = []
+    eleminc = []
+    q = Qs[question_number-1]
+    referenced_labels = [r[0] for r in q[1]] # labels which we reference.         
+    referenced_labels = list(set(referenced_labels))
+    for rname in referenced_labels : 
+        pfix.append(rname)       
+        included_labels = [PREFIX + ll[0] for ll in q[2]]  + figures_included 
+        #print included_labels
+        if (PREFIX+rname) not in included_labels :                                 
+            l = [e[0] for e in ELEMENTS if e[2][0][0] == rname]   
+            eleminc.append(l[0])        
+            
+    solution = getgroups(q[0],'solution')[0][0]
+    sanswer = getgroups(q[0],'answer')[0][0]
+    answer = int(sanswer[1:2])
+    sanswer = sanswer[3:]
+    sanswer = "\\begin{enumerate}[label=\\Alph*]" + sanswer + "\\end{enumerate}"
+    
+    question_text = q[0][0:q[0].find('\\begin{answer}')]
+    question_text = question_text.strip() + "\n" + '\n'.join(eleminc) + '\n'+sanswer.strip()
+        
+    question_text = process_figures(question_text,PREFIX,INPUT_TEX_BASE)
+    question_text = question_text.replace("\\thecorrect\\", "ABCD"[answer-1]+" ")
+    for pf in pfix:
+        question_text = question_text.replace('{'+pf+'}', '{'+PREFIX+pf+'}')
+        solution = solution.replace('{'+pf+'}', '{'+PREFIX+pf+'}')
+        
+    solution = solution.replace("\\thecorrect\\", "ABCD"[answer-1]+" ")    
+    figures_included = figures_included + [PREFIX + rl for rl in referenced_labels]
+    
+    FOUT = OUTPUT_TEX_BASE + "/"+PREFIX[0:6]+str(question_number)+".tex"
+    f = open(FOUT,'w')
+    f.write(question_text.strip())
+    f.close()
+    
+    FOUT = OUTPUT_TEX_BASE + "/"+PREFIX[0:6]+str(question_number)+"sol.tex"
+    f = open(FOUT,'w')
+    f.write(solution.strip())
+    f.close()
+    return [question_text,solution,answer,figures_included]
+
+
+EXAM_INCLUDES = [[] for i in range(20)]
+if True :
+    # viz, hist, box, distance, sims 
+    EXAM_INCLUDES[2] = ['f2011q1', 'f2013q1','f2014q1',]    
+    EXAM_INCLUDES[3] = ['s2012q4','f2011q2', 'f2013q3','f2014q3','f2014q4','s2014q3',]      # PCA
+    
+    EXAM_INCLUDES[4] = ['f2014q10', 's2013Q18', 'f2013q18']  # Data, norms, variance, correlation, percentile.
+    EXAM_INCLUDES[5] = ['f2014q8','s2013q17', 'f2013q15'] # Bayes
+    EXAM_INCLUDES[6] = ['f2012q2', 'f2014Q2', 's2014q1'] # Visualization
+    
+    EXAM_INCLUDES[7] = ['s2013Q12', 's2014Q5', 'f2013q6', 'f2013q17','f2014q22']  # log. regression     
+    EXAM_INCLUDES[8] = ['f2013q14','f2013q13','f2014q9','f2014q21'] # TREES     
+    
+    EXAM_INCLUDES[9] = ['f2014q27', 's2013q13', 's2013q14', 'f2013q7','f2013q16','f2014q6','f2013q25','f2014q18',]  # overfitting, fw selection
+    
+    EXAM_INCLUDES[10] = ['f2013q9','f2014q23','f2014q12'] # KNN methods
+    EXAM_INCLUDES[11] = ['f2015q16', 'f2015q17', 'f2013q19', 'f2014q15'] # bayesian methods (classifier) + NB.    
+
+    EXAM_INCLUDES[12] = ['s2013q26']  # bias-variance, regularization. # PROBLEMS!
+    EXAM_INCLUDES[13] = ['f2013q23','f2014q5', 'f2013q12','f2014q19', ] # neural networks
+    
+    EXAM_INCLUDES[14] = ['f2014q24','f2014q25',]  # AUC, statistics (CIs)
+    EXAM_INCLUDES[15] = ['f2014q26', 'f2013q24',] # ensemble methods boosting
+    
+    ## PART 3
+    # Lecture 10   
+    EXAM_INCLUDES[16] = ['f2013q8','f2014q20','f2014q11','f2012q12'] # kmeans, hierarchical agglom
+    
+    #Lecture 11
+    EXAM_INCLUDES[17] = ['f2013q22','f2013q26', 'f2014q7',]     # EM/GMM
+    EXAM_INCLUDES[18] = ['f2013q11', 's2013q9','f2011q27', 'f2013q20','f2013q10','f2014q13','f2014q14'] # Density estimation
+
+    # Lecture 12    
+    EXAM_INCLUDES[19] = ['s2014q11', 's2014q12'] # Association rule learning
+
+AE = [b for e in EXAM_INCLUDES for b in e]
+for e in AE : 
+    if len([j for j in AE if j == e]) > 1 : 
+        print(e)
+    
+HOMEWORK_PROBLEMS = [[] for i in range(len(EXAM_INCLUDES))]
+# BKOCK 1
+HOMEWORK_PROBLEMS[2]= [(3,1), (2,1), (3,2)] # basic data and PCA
+HOMEWORK_PROBLEMS[3]= [(4,1), (4,2), (4,3)] # Measures of similarity and summary statistics.
+HOMEWORK_PROBLEMS[4]= [(5,1), (5,2), (6,1)] # Visualization, probabilities
+
+# BLOCK 2
+HOMEWORK_PROBLEMS[5]= [(8,1), (7,1), (7,2)] # Lecture 5, reg+trees
+HOMEWORK_PROBLEMS[6]= [(9,1), (9,2), (9,3)] # Lecture 6, crossval 
+HOMEWORK_PROBLEMS[7]= [(11,1), (11,2), (10,1)] # Lecture 7, KNN+Bayes+Naive-bayes.
+HOMEWORK_PROBLEMS[8]= [(13,1), (13,2), (13,3)] # Lecture 8, Bias/Var + Artificial NN.
+HOMEWORK_PROBLEMS[9]= [(14,1), (14,2), (15,1)] # Lecture 9, classimb/AUC + Ensemble
+
+# BLOCK 3
+HOMEWORK_PROBLEMS[10]= [(16,1), (16,2), (16,3)] # Lecture 9, classimb/AUC + Ensemble
+
+HOMEWORK_PROBLEMS[11]= [(18,1), (17,1), (17,2)] # Lecture 9, classimb/AUC + Ensemble
+HOMEWORK_PROBLEMS[12]= [(19,1), (16,2), (16,3)] # Lecture 9, classimb/AUC + Ensemble
+
+EXAM_BASE_DIR = CDIR+ "/../../Exam/"
+EXAM_TEX_CONTENT = {} 
+
+rr = '''
+\\newpage \\newgeometry{left=\PLLEFT,right=\PLRIGHT,top=\PLTOP,bottom=\PLBOTTOM} \\begin{multicols}{2}
+\\section*{Problems} \\addcontentsline{toc}{section}{Problems}
+%s \\end{multicols}
+\\restoregeometry  \\newpage '''
+
+if __name__ == "__main__":
+    for chap,ae in enumerate(EXAM_INCLUDES):
+        allq = []
+        allsol = []
+        adex = 0
+        figs_included = []
+        nstrings = []
+        if not ae : continue
+        sas = []
+        for qsin in ae : 
+            sem = qsin[0]
+            year = qsin[1:5]
+            q = int(qsin[6:])   
+            
+            SEML = "Spring" if sem=="s" else "Fall"
+            nstrings.append("%s %s question %i"%(SEML,year,q) )
+            
+            INPUT_TEX_BASE = EXAM_BASE_DIR + ("Exam %s %s/latex/"%(SEML,year))
+            if not os.path.isdir(INPUT_TEX_BASE) :
+                INPUT_TEX_BASE = EXAM_BASE_DIR + ("Exam %s %s/02450Exam%s%s/latex/"%(SEML,year,SEML,year))
+                        
+            exam_tex_file = INPUT_TEX_BASE + ("02450ex_%s%s_book.tex"%(SEML,year))
+            
+            if not os.path.isfile(exam_tex_file) :
+                exam_tex_file = INPUT_TEX_BASE + ("02450ex_%s%s.tex"%(SEML,year))
+            
+            FIG_PREFIX = qsin[0:6] + "c"+str(chap)
+            
+            if not EXAM_TEX_CONTENT.has_key(FIG_PREFIX) : 
+                EXAM_TEX_CONTENT[FIG_PREFIX] = rec_input(exam_tex_file)
+            s2 = EXAM_TEX_CONTENT[FIG_PREFIX]
+            
+            [qtext,qsol,adex,fi] = process_question(FIG_PREFIX,INPUT_TEX_BASE,s2,q,figs_included)
+            figs_included = figs_included + fi
+            sa = 'ABCD'[adex-1]
+            sas.append(sa)
+            # write joint solution file and joint answer thingy
+        
+        cq = ['\\begin{prob}\\label{c%iprob%i}\\textbf{%s:} \n \\input{Exams/%s}\\end{prob}'%(chap,qn+1,nstrings[qn],qs) for (qn,qs) in enumerate(ae)]
+        cq = '\n'.join(cq)
+        
+        cs = ['\\begin{sol}{c%iprob%i}\\textbf{The correct answer is %s:} \\input{Exams/%ssol}\\end{sol}'%(chap,qn+1,sas[qn],qs) for (qn,qs) in enumerate(ae)]
+        cs = '\n'.join(cs)
+        
+        ss = rr%cq       
+        FOUT = OUTPUT_TEX_BASE + "/c%iprob.tex"%chap
+        f = open(FOUT,'w')
+        f.write(ss)
+        f.close()
+
+        FOUT = OUTPUT_TEX_BASE + "/c%isol.tex"%chap
+        f = open(FOUT,'w')
+        f.write(cs)
+        f.close()
     print("All Done")
```

### Comparing `coursebox-0.1.8/src/coursebox/core/info.py` & `coursebox-0.1.9/src/coursebox/core/info.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,364 +1,364 @@
-from datetime import timedelta
-from datetime import datetime
-import coursebox
-# import thtools
-from coursebox.thtools_base import list_dict2dict_list
-# import jinjafy
-import openpyxl
-from coursebox.core.projects_info import populate_student_report_results
-from coursebox.core.info_paths import get_paths, semester_id, semester, year, today
-from coursebox.core.info_paths import core_conf
-# import six
-# import pybtex.database.input.bibtex
-# import pybtex.plugin
-# import io
-from line_profiler_pycharm import profile
-import time
-
-@profile
-def xlsx_to_dicts(xlsx_file,sheet=None, as_dict_list=False):
-    # print("Loading...", xlsx_file, sheet, as_dict_list)
-    t0 = time.time()
-    wb = openpyxl.load_workbook(xlsx_file, data_only=True, read_only=True)
-    if not sheet:
-        ws = wb.worksheets[0]
-    else:
-        ws = [ws for ws in wb.worksheets if ws.title == sheet]
-        if len(ws) < 1:
-            return None
-        else:
-            ws = ws.pop()
-    # print(time.time()-t0)
-    # dd = []
-    # key_cols = [j for j in range(ws.max_column) if ws.cell(row=1, column=j + 1).value is not None]
-    # print(time.time()-t0, ws.max_row)
-    # np.array([[i.value for i in j[1:5]] for j in ws.rows])
-
-    import numpy as np
-    A = np.array([[i.value for i in j] for j in ws.rows])
-    # print(time.time() - t0, ws.max_row, len(key_cols))
-
-
-    # for j in range(A.shape[1]):
-
-
-
-
-    a = 234
-
-    # for i in range(1, ws.max_row):
-    #     rdict = {}
-    #     if not any( [ws.cell(row=i+1, column=j+1).value is not None for j in key_cols] ):
-    #         continue
-    #     for j in key_cols:
-    #         key = ws.cell(row=1, column=j+1).value
-    #         if key is not None:
-    #             key = key.strip() if isinstance(key,str) else key
-    #             value = ws.cell(row=i + 1, column=j + 1).value
-    #             value = value.strip() if isinstance(value,str) else value
-    #             if isinstance(value, str):
-    #                 if value == 'True':
-    #                     value = True
-    #                 if value == 'False':
-    #                     value = False
-    #             rdict[key] = value
-    #     dd.append(rdict)
-
-    # print(time.time()-t0)
-
-    A = A[:, A[0] != None]
-    A = A[(A != None).sum(axis=1) > 0, :]
-
-    dd2 = []
-    for i in range(1, A.shape[0]):
-        A[A == 'True'] = True
-        A[A == 'False'] = False
-
-        d = dict(zip(A[0, :].tolist(), [a.strip() if isinstance(a,str) else a for a in A[i, :].tolist() ]))
-        dd2.append(d)
-
-    # print(time.time() - t0)
-    dd = dd2
-    # if dd != dd2:
-    #     for k in range(len(dd)):
-    #         if dd[k] != dd2[k]:
-    #             print(k)
-    #             print(dd)
-    #             print(dd2)
-    #     assert False
-    #     print("BAd!")
-    if as_dict_list:
-        dl = list_dict2dict_list(dd)
-        for k in dl.keys():
-            x = [v for v in dl[k].tolist() if v is not None]
-            if len(x) == 1: x = x.pop()
-            dl[k] = x
-        dd = dl
-    wb.close()
-    # print("xlsx2dicts", time.time()-t0)
-    return dd
-
-def get_enrolled_students():
-    paths = get_paths()
-    students = xlsx_to_dicts(paths['information.xlsx'], sheet='students')
-    students2 = {}
-    for s in students:
-        s2 = {}
-        if s['Study number']:
-            s['Username'] = s['Study number']
-        for k in s.keys():
-            k2 = k.lower().replace(" ", "")
-            if k2 == "studynumber": continue
-            if k2 == "username":
-                k2 = "id"
-                if not s[k] or len(s[k]) == 0:
-                    print("Bad study id: ")
-                    print(s)
-                    raise Exception("malformed course configuration file, bad student id")
-            s2[k2] = s[k]
-
-        id = s2['id']
-        students2[id] = s2
-    return students2
-
-def get_instructors():
-    paths = get_paths()
-    instructors = xlsx_to_dicts(paths['information.xlsx'], sheet='instructors')
-    return instructors
-
-def continuing_education():
-    return coursebox.core.info_paths.core_conf['continuing_education_mode']
-
-def first_day_of_class(info):
-    if continuing_education():
-        first_day_of_class = datetime(year=year(), month=info['first-month'], day=info['first-day'], hour=info['hour'][0], minute=info['minute'][0])
-    else:
-        mo_first = datetime(year=year(), month=1 if semester() == 'spring' else 8, day=1, hour=13, minute=0)
-        # scroll to monday
-        while mo_first.weekday() != 0: #strftime('%A') is not 'Monday':
-            mo_first += timedelta(days=1)
-        # add 4 weeks to get into 13 week period
-        for _ in range(4):
-            mo_first += timedelta(days=7)
-
-        dow = int(info.get('day_of_week', 1))
-        while mo_first.weekday() != dow:
-            mo_first += timedelta(days=1)
-
-        first_day_of_class = mo_first
-    return first_day_of_class
-
-
-def lectures(info, pensum=None):
-    ow = timedelta(days=7)
-    d = first_day_of_class(info)
-
-    holiday = int(info['holiday_week']) if "holiday_week" in info else (9 if semester() == "spring" else 6)
-    paths = get_paths()
-    lectures = []
-    lecture_info = xlsx_to_dicts(paths['information.xlsx'], sheet='lectures')
-
-    for lecture in lecture_info:
-        em = lecture["resources"]
-        r = []
-        if em:
-            ems = em.split("\n")
-            for e in ems:
-                e = e.strip()
-                url = e[:e.find(" ")]
-                description = e[e.find(" ") + 1:]
-                shorturl = url[:url.find("/",url.find("."))]
-                r.append( {'url': url, 'shorturl': shorturl, 'description': description})
-        lecture["resources"] = r
-        if pensum is not None:
-
-            rd, html = lecture['reading'], ""
-            while True:
-                i = rd.find("\\cite")
-                if i < 0: break
-                j = rd.find("}", i)
-                html += rd[:i]
-                cite = rd[i:j + 1]
-                rd = rd[j+1:]
-                if cite.find("[") > 0:
-                    sr = cite[cite.find("[")+1:cite.find("]")]
-                else:
-                    sr = None
-                key = cite[cite.find("{")+1:cite.find("}")]
-                html += "[<b>" + pensum[key]['label'] + "</b>" + (", " + sr if sr is not None else "") + "]"
-                pensum[key]['suggested'] = True
-            html += rd
-            lecture['reading_html'] = html
-
-    if continuing_education():
-        ice = xlsx_to_dicts(paths['information.xlsx'], sheet='ce', as_dict_list=True)
-        holiday = -1
-        dd = [ice['day'][i] - ice['day'][i-1] for i in range(1, len(ice['day']))]
-        dd.append(0)
-
-    for i in range(0, len(lecture_info)):
-        l = dict()
-        l['year'] = d.year
-        l['month'] = d.strftime('%B')
-        l['day'] = d.day
-        l['date'] = d
-        l['preceded_by_holiday'] = i == holiday
-        if not continuing_education():
-            d = d + ow
-            if i == holiday - 1: d = d + ow
-            if d.month == 5 and d.day == 8: # grundlovsdag
-                d += timedelta(days=4)
-        else:
-            d = d + timedelta(days=dd[i-0] if i > 1 else 0)
-            d = d.replace(hour=ice['hour'][i-1], minute=ice['minute'][i-1])
-
-        info = lecture_info[i]
-
-        ir = info.get('reading', "")
-        info['reading_long'] = ir.replace("C", "Chapter ") if ir else ""
-
-        hwp =  info['homework_problems']
-        info['homework_problems_long'] = hwp.replace("P", "Problem ") if hwp else ""
-        if info["learning_objectives"]:
-            info["learning_objectives"] = [s.strip() for s in info["learning_objectives"].split("\n")]
-        l.update(info)
-        lectures.append(l)
-    return lectures, pensum
-
-def get_forum(paths):
-    a = xlsx_to_dicts(paths['information.xlsx'], sheet='forum', as_dict_list=True)
-    if a is None:
-        return a
-    from collections import defaultdict
-    dd = defaultdict(lambda: [])
-    kk = list(a.keys())[0]
-    for i, k in enumerate(kk.split(",")):
-        k = k.replace("[", "")
-        k = k.replace("]", "")
-        k = k.split(" ")[0]
-        for v in a[kk]:
-            dd[k.lower()].append(v.split(",")[i])
-
-    n = len(list(dd.values())[0])
-    d2 = []
-    for i in range(n):
-        d2.append({k: v[i] for k, v in dd.items()})
-    return d2
-
-@profile
-def class_information():
-    course_number = core_conf['course_number']
-    piazza = 'https://piazza.com/dtu.dk/%s%s/%s' % (semester().lower(), year(), course_number)
-    paths = get_paths()
-    teachers = xlsx_to_dicts(paths['information.xlsx'], sheet='teachers')
-    students, all_groups = populate_student_report_results( get_enrolled_students() )
-    continuing_education_mode = core_conf['continuing_education_mode']
-    faq = xlsx_to_dicts(paths['information.xlsx'], sheet='faq')
-
-
-    d = {'year': year(),
-         'piazza': piazza, # deprecated.
-         'course_number': course_number,
-         'semester': semester(),
-         # 'reports_handout': [1,6], # Set in excel conf.
-         # 'reports_handin': [6, 11], # set in excel conf.
-         'semester_id': semester_id(),
-         'today': today(),
-         'instructors': get_instructors(),
-         'students': students,
-         'teachers': teachers,
-         "CE": continuing_education_mode,
-         "all_groups": all_groups,
-         "faq": faq,
-         'forum': get_forum(paths),
-         }
-
-    written_exam = xlsx_to_dicts(paths['information.xlsx'], sheet='exam', as_dict_list=True)
-    if "solution_q" in written_exam:
-        written_exam['solution'] = {n:a for n,a in zip( written_exam['solution_q'], written_exam['solution_a'] ) }
-
-    d['written_exam'] = written_exam
-
-    gi = xlsx_to_dicts(paths['information.xlsx'], sheet='general_information', as_dict_list=True)
-    for (k, v) in zip(gi['key'], gi['value']):
-        if v == 'True':
-            v = True
-        if v == 'False':
-            v= False
-        gi[k] = v
-    del gi['key']
-    del gi['value']
-
-    from snipper.load_citations import get_bibtex, get_aux
-    if "pensum_bib" in gi:
-        bibtex = get_bibtex(paths['02450public'] + "/" + gi['pensum_bib'])
-        # refs, nrefs = get_references(paths['02450public'] + "/" + gi['pensum_bib'], gi)
-        # d['references'], d['new_references'] = refs, nrefs
-        cmds = []
-        ls = lambda x: x if isinstance(x, list) else [x]
-        if 'tex_command' in gi:
-            for cmd, aux, display in zip(ls(gi['tex_command']), ls(gi['tex_aux']), ls(gi['tex_display'])):
-                cm = dict(command=cmd, aux=get_aux(paths['02450public'] + "/"+aux), output=display)
-                cmds.append(cm)
-
-                # ax = parse_aux(aux, bibtex=gi['bibtex'])
-                # for k in ax:
-                #     ax[k]['pyref'] = display % (ax[k]['nicelabel'],)
-                # newref[cmd] = ax
-        d['references'] = dict(bibtex=bibtex, commands=cmds)
-
-        # references = dict(bibtex=bibtex,
-        #                   # aux=auxfile,
-        #                   commands=[dict(command='\\aref2', output="(Assignment 2, %s)", aux=auxfile),
-        #                             dict(command='\\nref', output="\cite[%s]{herlau}", aux=auxfile),
-        #                             ])
-
-
-    else:
-        print("[info]", "No bibtex rereferences specified. Check configuration file. ")
-        d['references'] = dict(commands=[], bibtex={}) #['bibtex'] = None
-    d.update(gi)
-    # set first day of class if CE
-    if continuing_education_mode:
-        ice = xlsx_to_dicts(paths['information.xlsx'], sheet='ce', as_dict_list=True)
-        d.update(ice)
-
-    d['lectures'], d['references']['bibtex'] = lectures(info=d, pensum=d['references']['bibtex'])
-
-    d['first_day_of_class'] = first_day_of_class(info=d)
-    d['day_of_week_str'] = d['first_day_of_class'].strftime('%A')
-    if "piazza" in gi:
-        d['piazza'] = gi['piazza']
-
-    for k in ['freeze_report_evaluation', 'freeze_grades']:
-        freeze = gi[k]
-        freeze = freeze == "True" if isinstance(freeze, str) else freeze
-        freeze = freeze[0] if isinstance(freeze, list) else freeze
-        gi[k] = freeze
-
-    for k,v in core_conf.items():
-        d[k] = v
-
-    d['CE2'] = gi.get("days", 5) == 2 if continuing_education_mode else False
-    d['CE5'] = gi.get("days", 5) == 5 if continuing_education_mode else False
-
-    d['freeze_report_evaluation'] = d['freeze_report_evaluation'] == 'True'
-    d['freeze_grades'] = d['freeze_grades'] == 'True'
-
-    d['rooms'] = xlsx_to_dicts(paths['information.xlsx'], sheet='rooms')
-    fix_instructor_comma(d['rooms'], d['instructors'])
-
-    d['teams'] = xlsx_to_dicts(paths['information.xlsx'], sheet='teams')
-    fix_instructor_comma(d['teams'], d['instructors'])
-    return d
-
-def fix_instructor_comma(dd, instructors):
-    for r in dd:
-        ri_shortnames = [i.strip().lower() for i in r['instructors'].split(",")]
-        ri = []
-        for sn in ri_shortnames:
-            di = [i for i in instructors if i['shortname'] == sn ]
-            if not di:
-                print("Did not find shortname: " + sn + ". This seems bad.")
-            ri += di
+from datetime import timedelta
+from datetime import datetime
+import coursebox
+# import thtools
+from coursebox.thtools_base import list_dict2dict_list
+# import jinjafy
+import openpyxl
+from coursebox.core.projects_info import populate_student_report_results
+from coursebox.core.info_paths import get_paths, semester_id, semester, year, today
+from coursebox.core.info_paths import core_conf
+# import six
+# import pybtex.database.input.bibtex
+# import pybtex.plugin
+# import io
+from line_profiler_pycharm import profile
+import time
+
+@profile
+def xlsx_to_dicts(xlsx_file,sheet=None, as_dict_list=False):
+    # print("Loading...", xlsx_file, sheet, as_dict_list)
+    t0 = time.time()
+    wb = openpyxl.load_workbook(xlsx_file, data_only=True, read_only=True)
+    if not sheet:
+        ws = wb.worksheets[0]
+    else:
+        ws = [ws for ws in wb.worksheets if ws.title == sheet]
+        if len(ws) < 1:
+            return None
+        else:
+            ws = ws.pop()
+    # print(time.time()-t0)
+    # dd = []
+    # key_cols = [j for j in range(ws.max_column) if ws.cell(row=1, column=j + 1).value is not None]
+    # print(time.time()-t0, ws.max_row)
+    # np.array([[i.value for i in j[1:5]] for j in ws.rows])
+
+    import numpy as np
+    A = np.array([[i.value for i in j] for j in ws.rows])
+    # print(time.time() - t0, ws.max_row, len(key_cols))
+
+
+    # for j in range(A.shape[1]):
+
+
+
+
+    a = 234
+
+    # for i in range(1, ws.max_row):
+    #     rdict = {}
+    #     if not any( [ws.cell(row=i+1, column=j+1).value is not None for j in key_cols] ):
+    #         continue
+    #     for j in key_cols:
+    #         key = ws.cell(row=1, column=j+1).value
+    #         if key is not None:
+    #             key = key.strip() if isinstance(key,str) else key
+    #             value = ws.cell(row=i + 1, column=j + 1).value
+    #             value = value.strip() if isinstance(value,str) else value
+    #             if isinstance(value, str):
+    #                 if value == 'True':
+    #                     value = True
+    #                 if value == 'False':
+    #                     value = False
+    #             rdict[key] = value
+    #     dd.append(rdict)
+
+    # print(time.time()-t0)
+
+    A = A[:, A[0] != None]
+    A = A[(A != None).sum(axis=1) > 0, :]
+
+    dd2 = []
+    for i in range(1, A.shape[0]):
+        A[A == 'True'] = True
+        A[A == 'False'] = False
+
+        d = dict(zip(A[0, :].tolist(), [a.strip() if isinstance(a,str) else a for a in A[i, :].tolist() ]))
+        dd2.append(d)
+
+    # print(time.time() - t0)
+    dd = dd2
+    # if dd != dd2:
+    #     for k in range(len(dd)):
+    #         if dd[k] != dd2[k]:
+    #             print(k)
+    #             print(dd)
+    #             print(dd2)
+    #     assert False
+    #     print("BAd!")
+    if as_dict_list:
+        dl = list_dict2dict_list(dd)
+        for k in dl.keys():
+            x = [v for v in dl[k].tolist() if v is not None]
+            if len(x) == 1: x = x.pop()
+            dl[k] = x
+        dd = dl
+    wb.close()
+    # print("xlsx2dicts", time.time()-t0)
+    return dd
+
+def get_enrolled_students():
+    paths = get_paths()
+    students = xlsx_to_dicts(paths['information.xlsx'], sheet='students')
+    students2 = {}
+    for s in students:
+        s2 = {}
+        if s['Study number']:
+            s['Username'] = s['Study number']
+        for k in s.keys():
+            k2 = k.lower().replace(" ", "")
+            if k2 == "studynumber": continue
+            if k2 == "username":
+                k2 = "id"
+                if not s[k] or len(s[k]) == 0:
+                    print("Bad study id: ")
+                    print(s)
+                    raise Exception("malformed course configuration file, bad student id")
+            s2[k2] = s[k]
+
+        id = s2['id']
+        students2[id] = s2
+    return students2
+
+def get_instructors():
+    paths = get_paths()
+    instructors = xlsx_to_dicts(paths['information.xlsx'], sheet='instructors')
+    return instructors
+
+def continuing_education():
+    return coursebox.core.info_paths.core_conf['continuing_education_mode']
+
+def first_day_of_class(info):
+    if continuing_education():
+        first_day_of_class = datetime(year=year(), month=info['first-month'], day=info['first-day'], hour=info['hour'][0], minute=info['minute'][0])
+    else:
+        mo_first = datetime(year=year(), month=1 if semester() == 'spring' else 8, day=1, hour=13, minute=0)
+        # scroll to monday
+        while mo_first.weekday() != 0: #strftime('%A') is not 'Monday':
+            mo_first += timedelta(days=1)
+        # add 4 weeks to get into 13 week period
+        for _ in range(4):
+            mo_first += timedelta(days=7)
+
+        dow = int(info.get('day_of_week', 1))
+        while mo_first.weekday() != dow:
+            mo_first += timedelta(days=1)
+
+        first_day_of_class = mo_first
+    return first_day_of_class
+
+
+def lectures(info, pensum=None):
+    ow = timedelta(days=7)
+    d = first_day_of_class(info)
+
+    holiday = int(info['holiday_week']) if "holiday_week" in info else (9 if semester() == "spring" else 6)
+    paths = get_paths()
+    lectures = []
+    lecture_info = xlsx_to_dicts(paths['information.xlsx'], sheet='lectures')
+
+    for lecture in lecture_info:
+        em = lecture["resources"]
+        r = []
+        if em:
+            ems = em.split("\n")
+            for e in ems:
+                e = e.strip()
+                url = e[:e.find(" ")]
+                description = e[e.find(" ") + 1:]
+                shorturl = url[:url.find("/",url.find("."))]
+                r.append( {'url': url, 'shorturl': shorturl, 'description': description})
+        lecture["resources"] = r
+        if pensum is not None:
+
+            rd, html = lecture['reading'], ""
+            while True:
+                i = rd.find("\\cite")
+                if i < 0: break
+                j = rd.find("}", i)
+                html += rd[:i]
+                cite = rd[i:j + 1]
+                rd = rd[j+1:]
+                if cite.find("[") > 0:
+                    sr = cite[cite.find("[")+1:cite.find("]")]
+                else:
+                    sr = None
+                key = cite[cite.find("{")+1:cite.find("}")]
+                html += "[<b>" + pensum[key]['label'] + "</b>" + (", " + sr if sr is not None else "") + "]"
+                pensum[key]['suggested'] = True
+            html += rd
+            lecture['reading_html'] = html
+
+    if continuing_education():
+        ice = xlsx_to_dicts(paths['information.xlsx'], sheet='ce', as_dict_list=True)
+        holiday = -1
+        dd = [ice['day'][i] - ice['day'][i-1] for i in range(1, len(ice['day']))]
+        dd.append(0)
+
+    for i in range(0, len(lecture_info)):
+        l = dict()
+        l['year'] = d.year
+        l['month'] = d.strftime('%B')
+        l['day'] = d.day
+        l['date'] = d
+        l['preceded_by_holiday'] = i == holiday
+        if not continuing_education():
+            d = d + ow
+            if i == holiday - 1: d = d + ow
+            if d.month == 5 and d.day == 8: # grundlovsdag
+                d += timedelta(days=4)
+        else:
+            d = d + timedelta(days=dd[i-0] if i > 1 else 0)
+            d = d.replace(hour=ice['hour'][i-1], minute=ice['minute'][i-1])
+
+        info = lecture_info[i]
+
+        ir = info.get('reading', "")
+        info['reading_long'] = ir.replace("C", "Chapter ") if ir else ""
+
+        hwp =  info['homework_problems']
+        info['homework_problems_long'] = hwp.replace("P", "Problem ") if hwp else ""
+        if info["learning_objectives"]:
+            info["learning_objectives"] = [s.strip() for s in info["learning_objectives"].split("\n")]
+        l.update(info)
+        lectures.append(l)
+    return lectures, pensum
+
+def get_forum(paths):
+    a = xlsx_to_dicts(paths['information.xlsx'], sheet='forum', as_dict_list=True)
+    if a is None:
+        return a
+    from collections import defaultdict
+    dd = defaultdict(lambda: [])
+    kk = list(a.keys())[0]
+    for i, k in enumerate(kk.split(",")):
+        k = k.replace("[", "")
+        k = k.replace("]", "")
+        k = k.split(" ")[0]
+        for v in a[kk]:
+            dd[k.lower()].append(v.split(",")[i])
+
+    n = len(list(dd.values())[0])
+    d2 = []
+    for i in range(n):
+        d2.append({k: v[i] for k, v in dd.items()})
+    return d2
+
+@profile
+def class_information():
+    course_number = core_conf['course_number']
+    piazza = 'https://piazza.com/dtu.dk/%s%s/%s' % (semester().lower(), year(), course_number)
+    paths = get_paths()
+    teachers = xlsx_to_dicts(paths['information.xlsx'], sheet='teachers')
+    students, all_groups = populate_student_report_results( get_enrolled_students() )
+    continuing_education_mode = core_conf['continuing_education_mode']
+    faq = xlsx_to_dicts(paths['information.xlsx'], sheet='faq')
+
+
+    d = {'year': year(),
+         'piazza': piazza, # deprecated.
+         'course_number': course_number,
+         'semester': semester(),
+         # 'reports_handout': [1,6], # Set in excel conf.
+         # 'reports_handin': [6, 11], # set in excel conf.
+         'semester_id': semester_id(),
+         'today': today(),
+         'instructors': get_instructors(),
+         'students': students,
+         'teachers': teachers,
+         "CE": continuing_education_mode,
+         "all_groups": all_groups,
+         "faq": faq,
+         'forum': get_forum(paths),
+         }
+
+    written_exam = xlsx_to_dicts(paths['information.xlsx'], sheet='exam', as_dict_list=True)
+    if "solution_q" in written_exam:
+        written_exam['solution'] = {n:a for n,a in zip( written_exam['solution_q'], written_exam['solution_a'] ) }
+
+    d['written_exam'] = written_exam
+
+    gi = xlsx_to_dicts(paths['information.xlsx'], sheet='general_information', as_dict_list=True)
+    for (k, v) in zip(gi['key'], gi['value']):
+        if v == 'True':
+            v = True
+        if v == 'False':
+            v= False
+        gi[k] = v
+    del gi['key']
+    del gi['value']
+
+    from snipper.load_citations import get_bibtex, get_aux
+    if "pensum_bib" in gi:
+        bibtex = get_bibtex(paths['02450public'] + "/" + gi['pensum_bib'])
+        # refs, nrefs = get_references(paths['02450public'] + "/" + gi['pensum_bib'], gi)
+        # d['references'], d['new_references'] = refs, nrefs
+        cmds = []
+        ls = lambda x: x if isinstance(x, list) else [x]
+        if 'tex_command' in gi:
+            for cmd, aux, display in zip(ls(gi['tex_command']), ls(gi['tex_aux']), ls(gi['tex_display'])):
+                cm = dict(command=cmd, aux=get_aux(paths['02450public'] + "/"+aux), output=display)
+                cmds.append(cm)
+
+                # ax = parse_aux(aux, bibtex=gi['bibtex'])
+                # for k in ax:
+                #     ax[k]['pyref'] = display % (ax[k]['nicelabel'],)
+                # newref[cmd] = ax
+        d['references'] = dict(bibtex=bibtex, commands=cmds)
+
+        # references = dict(bibtex=bibtex,
+        #                   # aux=auxfile,
+        #                   commands=[dict(command='\\aref2', output="(Assignment 2, %s)", aux=auxfile),
+        #                             dict(command='\\nref', output="\cite[%s]{herlau}", aux=auxfile),
+        #                             ])
+
+
+    else:
+        print("[info]", "No bibtex rereferences specified. Check configuration file. ")
+        d['references'] = dict(commands=[], bibtex={}) #['bibtex'] = None
+    d.update(gi)
+    # set first day of class if CE
+    if continuing_education_mode:
+        ice = xlsx_to_dicts(paths['information.xlsx'], sheet='ce', as_dict_list=True)
+        d.update(ice)
+
+    d['lectures'], d['references']['bibtex'] = lectures(info=d, pensum=d['references']['bibtex'])
+
+    d['first_day_of_class'] = first_day_of_class(info=d)
+    d['day_of_week_str'] = d['first_day_of_class'].strftime('%A')
+    if "piazza" in gi:
+        d['piazza'] = gi['piazza']
+
+    for k in ['freeze_report_evaluation', 'freeze_grades']:
+        freeze = gi[k]
+        freeze = freeze == "True" if isinstance(freeze, str) else freeze
+        freeze = freeze[0] if isinstance(freeze, list) else freeze
+        gi[k] = freeze
+
+    for k,v in core_conf.items():
+        d[k] = v
+
+    d['CE2'] = gi.get("days", 5) == 2 if continuing_education_mode else False
+    d['CE5'] = gi.get("days", 5) == 5 if continuing_education_mode else False
+
+    d['freeze_report_evaluation'] = d['freeze_report_evaluation'] == 'True'
+    d['freeze_grades'] = d['freeze_grades'] == 'True'
+
+    d['rooms'] = xlsx_to_dicts(paths['information.xlsx'], sheet='rooms')
+    fix_instructor_comma(d['rooms'], d['instructors'])
+
+    d['teams'] = xlsx_to_dicts(paths['information.xlsx'], sheet='teams')
+    fix_instructor_comma(d['teams'], d['instructors'])
+    return d
+
+def fix_instructor_comma(dd, instructors):
+    for r in dd:
+        ri_shortnames = [i.strip().lower() for i in r['instructors'].split(",")]
+        ri = []
+        for sn in ri_shortnames:
+            di = [i for i in instructors if i['shortname'] == sn ]
+            if not di:
+                print("Did not find shortname: " + sn + ". This seems bad.")
+            ri += di
         r['instructors'] = ri
```

### Comparing `coursebox-0.1.8/src/coursebox/core/info_paths.py` & `coursebox-0.1.9/src/coursebox/core/info_paths.py`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,102 +1,102 @@
-# import thtools
-import os
-import shutil
-from datetime import datetime
-from warnings import warn
-
-# don't remove this one. Set by setup_toolbox
-core_conf = {}
-
-def get_paths():
-    cd = core_conf['working_dir']
-    cd = os.path.basename( os.path.dirname( os.path.dirname(cd) ) )
-    num = cd[:-6] # course number
-    CDIR = core_conf['working_dir']
-    course_number = core_conf['course_number']
-
-    root_02450public = os.path.normpath(CDIR + "/../..")
-    root_02450private = os.path.normpath(root_02450public + "/../%sprivate"%num)
-    root_02450instructors = os.path.normpath(root_02450private + "/../%sinstructors"%num)
-    root_02450students = os.path.normpath(root_02450private + "/../%sstudents" % num)
-
-    root_02450public = root_02450public.replace("\\", "/")
-    root_02450private = root_02450private.replace("\\", "/")
-
-    if not os.path.isdir(root_02450private):
-        root_02450private = f'{root_02450public}/{num}private'
-        warn('Private repository not found at the expected location.')
-        warn('Using mock info from resources folder at:')
-        warn(root_02450private)
-        # Tue: always overwrite semester path.
-        # semester_path = root_02450private +"/resources/mock_semesters/" + semester_id()
-    # else:
-    semester_path = root_02450private + "/semesters/" + semester_id()
-
-    if not os.path.isdir(semester_path):
-        os.makedirs(semester_path)
-
-    main_conf = semester_path + "/" + semester_id() + ".xlsx"
-    if not os.path.exists(main_conf):
-        main_conf = f"{semester_path}/{course_number}_{semester_id()}.xlsx"
-    if not os.path.exists(main_conf):
-        raise Exception("Main config file not found " + main_conf)
-
-    _files = []
-    sCE = "CE" if core_conf['continuing_education_mode'] else ""
-    paths ={'02450private': root_02450private,
-            '02450public': root_02450public,
-            '02450instructors': root_02450instructors,
-            '02450students': root_02450students,
-            'shared': root_02450public+"/shared",
-            'exams': root_02450private+"/Exam",
-            'course_number': course_number,
-            'semester': semester_path,
-            'information.xlsx': main_conf,
-            'homepage_template': "%s/WEB/index_partial.html"%root_02450public,
-            'homepage_out': "%s/WEB/%sindex.html"%(root_02450public, sCE),
-            'pdf_out': "%s/%spdf_out"%(root_02450public, sCE),
-            'instructor': root_02450public + "/Exercises",
-            'shared_latex_compilation_dir': root_02450public + "/Exercises/LatexCompilationDir/Latex",
-            'book': root_02450public + "/MLBOOK/Latex",
-            'lectures': root_02450public + "/Lectures",
-            'instructor_project_evaluations': "%s/project_evaluations_%s" % (root_02450instructors, semester_id()),
-            'project_evaluations_template.xlsx': root_02450private +"/ReportEvaluation/%s_project_template.xlsx"%num,
-            'collected_project_evaluations.xlsx': semester_path + "/"+course_number+"_project_" + semester_id() + ".xlsx",
-            'electronic_exam_handin_dir': semester_path + "/exam/electronic_handin",
-            'exam_results_template.xlsx': root_02450private +"/Exam/%s_results_TEMPLATE.xlsx"%num,
-            'exam_instructions': root_02450public + "/ExamInstructions",
-    }
-    if os.path.exists(os.path.dirname(paths['instructor_project_evaluations'])):
-        if not os.path.isdir(paths['instructor_project_evaluations']):
-            os.mkdir(paths['instructor_project_evaluations'])
-    else:
-        pass
-    for (key, loc, template) in _files:
-        if not os.path.exists(os.path.dirname(loc)):
-            os.makedirs(os.path.dirname(loc))
-        if not os.path.exists(loc):
-            shutil.copyfile(template, loc)
-        paths[key] = loc
-    return paths
-
-
-def semester():
-    continuing_education_mode = core_conf['continuing_education_mode']
-    continuing_education_month = core_conf['continuing_education_month']
-    semester = core_conf['semester']
-
-    if continuing_education_mode:
-        month = continuing_education_month.lower()
-        return month
-    else:
-        return semester.lower()
-
-def year():
-    return core_conf['year']
-
-def semester_id():
-    s = "CE" if core_conf['continuing_education_mode'] else ""
-    return "%s%i%s"%(s, year(), semester())
-
-def today():
+# import thtools
+import os
+import shutil
+from datetime import datetime
+from warnings import warn
+
+# don't remove this one. Set by setup_toolbox
+core_conf = {}
+
+def get_paths():
+    cd = core_conf['working_dir']
+    cd = os.path.basename( os.path.dirname( os.path.dirname(cd) ) )
+    num = cd[:-6] # course number
+    CDIR = core_conf['working_dir']
+    course_number = core_conf['course_number']
+
+    root_02450public = os.path.normpath(CDIR + "/../..")
+    root_02450private = os.path.normpath(root_02450public + "/../%sprivate"%num)
+    root_02450instructors = os.path.normpath(root_02450private + "/../%sinstructors"%num)
+    root_02450students = os.path.normpath(root_02450private + "/../%sstudents" % num)
+
+    root_02450public = root_02450public.replace("\\", "/")
+    root_02450private = root_02450private.replace("\\", "/")
+
+    if not os.path.isdir(root_02450private):
+        root_02450private = f'{root_02450public}/{num}private'
+        warn('Private repository not found at the expected location.')
+        warn('Using mock info from resources folder at:')
+        warn(root_02450private)
+        # Tue: always overwrite semester path.
+        # semester_path = root_02450private +"/resources/mock_semesters/" + semester_id()
+    # else:
+    semester_path = root_02450private + "/semesters/" + semester_id()
+
+    if not os.path.isdir(semester_path):
+        os.makedirs(semester_path)
+
+    main_conf = semester_path + "/" + semester_id() + ".xlsx"
+    if not os.path.exists(main_conf):
+        main_conf = f"{semester_path}/{course_number}_{semester_id()}.xlsx"
+    if not os.path.exists(main_conf):
+        raise Exception("Main config file not found " + main_conf)
+
+    _files = []
+    sCE = "CE" if core_conf['continuing_education_mode'] else ""
+    paths ={'02450private': root_02450private,
+            '02450public': root_02450public,
+            '02450instructors': root_02450instructors,
+            '02450students': root_02450students,
+            'shared': root_02450public+"/shared",
+            'exams': root_02450private+"/Exam",
+            'course_number': course_number,
+            'semester': semester_path,
+            'information.xlsx': main_conf,
+            'homepage_template': "%s/WEB/index_partial.html"%root_02450public,
+            'homepage_out': "%s/WEB/%sindex.html"%(root_02450public, sCE),
+            'pdf_out': "%s/%spdf_out"%(root_02450public, sCE),
+            'instructor': root_02450public + "/Exercises",
+            'shared_latex_compilation_dir': root_02450public + "/Exercises/LatexCompilationDir/Latex",
+            'book': root_02450public + "/MLBOOK/Latex",
+            'lectures': root_02450public + "/Lectures",
+            'instructor_project_evaluations': "%s/project_evaluations_%s" % (root_02450instructors, semester_id()),
+            'project_evaluations_template.xlsx': root_02450private +"/ReportEvaluation/%s_project_template.xlsx"%num,
+            'collected_project_evaluations.xlsx': semester_path + "/"+course_number+"_project_" + semester_id() + ".xlsx",
+            'electronic_exam_handin_dir': semester_path + "/exam/electronic_handin",
+            'exam_results_template.xlsx': root_02450private +"/Exam/%s_results_TEMPLATE.xlsx"%num,
+            'exam_instructions': root_02450public + "/ExamInstructions",
+    }
+    if os.path.exists(os.path.dirname(paths['instructor_project_evaluations'])):
+        if not os.path.isdir(paths['instructor_project_evaluations']):
+            os.mkdir(paths['instructor_project_evaluations'])
+    else:
+        pass
+    for (key, loc, template) in _files:
+        if not os.path.exists(os.path.dirname(loc)):
+            os.makedirs(os.path.dirname(loc))
+        if not os.path.exists(loc):
+            shutil.copyfile(template, loc)
+        paths[key] = loc
+    return paths
+
+
+def semester():
+    continuing_education_mode = core_conf['continuing_education_mode']
+    continuing_education_month = core_conf['continuing_education_month']
+    semester = core_conf['semester']
+
+    if continuing_education_mode:
+        month = continuing_education_month.lower()
+        return month
+    else:
+        return semester.lower()
+
+def year():
+    return core_conf['year']
+
+def semester_id():
+    s = "CE" if core_conf['continuing_education_mode'] else ""
+    return "%s%i%s"%(s, year(), semester())
+
+def today():
     return datetime.today()
```

### Comparing `coursebox-0.1.8/src/coursebox/core/projects.py` & `coursebox-0.1.9/src/coursebox/core/projects.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,764 +1,764 @@
-import re
-import tempfile
-import tika
-import os
-import shutil
-import openpyxl
-import numpy as np
-import itertools
-import math
-import glob
-from tika import parser
-from openpyxl.worksheet.datavalidation import DataValidation
-from openpyxl.utils import get_column_letter
-import matplotlib.pyplot as plt
-import langdetect
-import xlwings as xw
-from coursebox.core.projects_info import get_output_file, INSTRUCTOR_ROW, STUDENT_ID_ROW, parse_column
-from coursebox.core.projects_info import EVALUATION_ROW_END, EVALUATION_ROW_START, WEIGHT_ROW_START, RANGE_MIN_COL, DELTA_ALLOWED_ROW
-from coursebox.core.info import get_paths, class_information, semester_id
-from coursebox.core import projects_info
-from coursebox.core.projects_plagiarism import plagiarism_checker
-from jinjafy.cache import cache_contains_dir, cache_update_dir
-from jinjafy.plot.plot_helpers import get_colors
-import time
-from collections import defaultdict
-import zipfile
-import pandas as pd
-from slider.slide import recursive_tex_collect
-
-def get_dirs(zf):
-    zip = zipfile.ZipFile(zf)
-    fls = list(set([os.path.dirname(x) for x in zip.namelist()]))
-    fls = [f for f in fls if len(f) > 0]
-    return fls
-
-def fix_handins_fuckup(project_id=2):
-    """ Handle the problem with multiple hand-ins in DTU learn. """
-    paths = get_paths()
-    from coursebox.core.info import class_information
-    info = class_information()
-    zf = paths['instructor_project_evaluations'] + f"/zip{project_id}.zip"
-
-    tas = [i['shortname'] for i in info['instructors'] ]
-    ta_links = {i['shortname']: i for i in info['instructors']}
-
-    ta_reports = {}
-    for ta in tas:
-        fname = paths['instructor_project_evaluations']  + f"/project_{project_id}_{ta}.zip"
-        for r in get_dirs(fname):
-            if r in ta_reports:
-                raise Exception
-            ta_reports[r] = ta
-
-    fls = get_dirs(zf)
-    # fls = [f for f in zip.namelist() if not f.endswith("tml") and f.endswith("/")]
-    d = defaultdict(lambda: [])
-    for l in fls:
-        # print(l)
-        group_id = int(l.split("-")[2].strip().split(" ")[1])
-        date = l.split("-")[-1].strip().split(" ")
-        hm = date[-2]
-        if len(hm) < 4:
-            hm = "0" + hm
-        hm = hm[:2] + ":" + hm[2:]
-        date[-2] = hm
-        date = " ".join(date)
-        import datetime
-        date_time_obj = datetime.datetime.strptime(date, '%d %B, %Y %I:%M %p')
-
-        d[group_id].append( {'file': l, 'date': date_time_obj, 'ta': ta_reports[l], 'group_id': group_id } )
-
-    d = {k: v for k, v in d.items() if len(v)  > 1}
-
-    ta_do_not = defaultdict(lambda: [])
-    ta_do = defaultdict(lambda: [])
-    for group_id, reports in d.items():
-        recent = max( r['date'] for r in reports)
-        for r in reports:
-            if r['date'] == recent:
-                ta_do[r['ta']].append(r)
-            else:
-                ta_do_not[r['ta']].append(r)
-
-    fname = paths['instructor_project_evaluations'] + "/do_not_evaluate.txt"
-    with open(fname, 'w') as f:
-        for ta, reports in ta_do_not.items():
-            f.write(ta_links[ta ]['name'] + f" ({ta})" + "\n")
-            for r in reports:
-                f.write("DO NOT EVALUATE: " + r['file'] + "\n")
-            f.write("\n")
-            f.write("\n")
-    with open(fname, 'r') as f:
-        print(f.read())
-    return ta_do, ta_do_not
-
-
-def handle_projects(verbose=False, gather_main_xlsx_file=True, plagiarism_check=False):
-    paths = get_paths()
-    info = class_information()
-    if info['freeze_report_evaluation']:
-        print("> Report evaluations are FROZEN, meaning TA changes are no longer taken into account")
-        print("> grades, etc. now relies on report resource file:")
-        print(paths['collected_project_evaluations.xlsx'])
-    if info['CE']:
-        return
-    if plagiarism_check:
-        plagiarism_checker(paths, info)
-        return
-
-    instructor_path = paths['instructor_project_evaluations']
-    cache_changed_xlsx_files = False
-    if gather_main_xlsx_file:
-        cache_base = paths['instructor_project_evaluations']
-        if cache_contains_dir(cache_base,cache_base, pattern="*.xlsx") and os.path.exists(paths['collected_project_evaluations.xlsx']):
-            pass
-        else:
-            cache_changed_xlsx_files = True
-            gather_instructor_sheets(info)
-            print("> Done gathering main .xlsx file from instructor .xlsx files")
-            cache_update_dir(cache_base, cache_base, pattern="*.xlsx")
-            info = class_information()
-
-    zip1 = instructor_path + "/zip1.zip"
-    zip2 = instructor_path + "/zip2.zip"
-    zip3 = instructor_path + "/zip3.zip"
-    zips = [None, zip1, zip2, zip3]
-
-    for j,zf in enumerate(zips):
-        ifiles = get_instructor_xlsx_files(info, j)
-        ex =  [os.path.exists(f) for (f,_) in ifiles]
-        if any(ex) and not all(ex):
-            raise Exception("Partial list of instructor files") # ensure there are either no files or all files exist
-        instructor_files_exist = ex.pop()
-
-        if instructor_files_exist:
-            # if instructor files are there, we should do nothing
-            continue
-        else: # instructor files do not exist
-            if j == 0:
-                copy_populate_from_template(paths, info, sheet_number=j, zip_file=None)
-
-            elif os.path.exists(zf):
-                # make a copy of report template and populate it with groups obtained from previous report evaluation.
-                # all_groups = get_all_reports_from_collected_xlsx_file()
-                copy_populate_from_template(paths, info, sheet_number=j, zip_file=zf)
-                # distribute_zip_content(info, sheet=j, zf_base=zf)
-            else:
-                print("When available, please move downloaded copy of all reports from campusnet to destination:")
-                print(zf)
-
-    mkboxplots(info['students'],paths)
-
-    if cache_changed_xlsx_files:
-        # Recompute nag files if instructor xlsx files have been changed
-        compute_error_files(info, paths)
-    nags = []
-    fs = glob.glob(paths['instructor_project_evaluations'] + "/PARSE_ERRORS_*.txt")
-    for f in fs:
-        name = f.split("_").pop()[:-4]
-        if name != "transfer":
-            v = [i for i in info['instructors'] if i['shortname'] == name]
-            with open(f, "r") as file:
-                s = file.read()
-                nlines = len(s.split("\n"))
-            if len(v) == 0:
-                raise Exception("Empty instructor list. what the ...")
-
-            ins_email = v[0]['email']
-            nags.append((name, ins_email, nlines))
-    Nerrors = sum([n[-1] for n in nags])
-    if Nerrors > 0:
-        print("\n> %i errors. These instructors have parse errors (.txt)" % sum([n[-1] for n in nags]))
-        print("; ".join([email for (_, email, _) in nags]))
-        print(", ".join([name.capitalize() for (name, _, _) in nags]))
-        print("TA/Errors: " + ", ".join(["%s:%i" % (name.capitalize(), lines) for (name, _, lines) in nags]))
-        print("---")
-    else:
-        print("No parse errors found")
-
-
-def compute_error_files(info, paths):
-    print("Recomputing nag files...")
-    ERRORS = dict()
-    students = info['students']
-    for repn in range(3, -1, -1):
-        ifiles = get_instructor_xlsx_files(info, sheet=repn)
-        all_groups = []
-        for out, ins in ifiles:
-            if not os.path.exists(out):
-                continue
-
-            if not ins in ERRORS:
-                ERRORS[ins] = []
-
-            wb = openpyxl.load_workbook(out, data_only=True)
-            if len(wb.worksheets) > 1:
-                es = os.path.basename(out) + "> Entire workbook is malformed. Workbook must only contain a single sheet. Fix ASAP; aborting further operations."
-                ERRORS[ins].append(es)
-                continue
-
-            cls = []
-            for i in range(2, wb.worksheets[0].max_column + 1):
-                cp = projects_info.parse_column(wb.worksheets[0], report_number=repn, column=i)
-                if not cp['student_ids']:
-                    continue
-                cls.append(cp)
-
-            for g in cls:
-                gins = g.get('instructor')
-                err_label = "File: '%s', column with student ids: '%s'"%(os.path.basename(out), ', '.join(g['student_ids']))
-                if gins != ins:
-                    gins = "Null" if not gins else gins
-                    es = err_label +"> Corrupted sheet. Instructor name: '"  + gins + "' not found. Should perhaps be: '" + ins+"'?"
-                    print(es)
-                    ERRORS[ins].append(es)
-                    continue
-
-                if repn >= 1 and g.get("score", None) == None and len(g['student_ids'])>0:
-                    es = err_label + "> Report not scored."
-                    ERRORS[ins].append(es)
-
-                if repn >= 1 and len(g.get('student_ids', [])) > 0:
-                    if g.get('score', 0) is None:
-                        es = err_label + f"> Report does not have a score. The sheet may have been used incorrectly or fields are missing"
-                        ERRORS[ins].append(es)
-                    elif g.get("score", 0) < 0 or g.get("score", 0) > 4:
-                        es = err_label + f"> Report score is {g.get('score', 0)}. The report score has to be between 0 and 4; probably due to a too high value of 'Delta' in instructor sheet."
-                        ERRORS[ins].append(es)
-
-                if repn >= 1 and not g['comments'] and info['course_number'] != '02465':
-                    es = err_label + "> Incomplete report evaluation (missing comments field)"
-                    es += "Please fill out comments field in your excel sheet."
-                    ERRORS[ins].append(es)
-
-
-                if repn >= 1 and not g['approver_comments']  and info['course_number'] != '02465':
-                    es = err_label + "> Incomplete report evaluation (you are missing the approver comments field; can simply be set to 'ok')."
-                    ERRORS.get(g['approver'], []).append(es)
-
-                if g['missing_fields']:
-                    mf = g['missing_fields']
-                    es = err_label + "> Incomplete report evaluation (missing required evaluation-scoring field(s): '%s')."%(', '.join( [s for _,s in mf] ) ,)
-                    es += " Please fill out missing field in your excel sheet."
-                    ERRORS[ins].append(es)
-
-                for sid in g['student_ids']:
-                    # student = [student for student in students if student['id'] == sid]
-                    if repn >= 1 and sid not in students and False:
-                        # I disabled this since
-                        es = err_label + "> Student ID '%s' not found in registered students on campusnet. "%sid
-                        es += " To fix this, check if student is on campusnet under 'list of participants'; if he/she IS on campusnet, email me about the problem. " \
-                              + " Otherwise, simply delete extra students from sheet and send an email to all students in the group (the student likely dropped out of course)"
-
-                        ERRORS[ins].append( es )
-                        continue
-
-                    bad = [ (i, s, g) for (i,s,g) in all_groups if s == "sid"]
-                    if len(bad) > 0:
-                        i = bad[0][0]
-                        g2 = bad[0][2]
-
-                        es = err_label + "> Duplicate student ids for student: %s. " % (sid, )
-                        es += "Student is also found in sheet by instructor: " + i
-                        es += " in group with students: " + (", ".join( g2['student_ids'])) + ". "
-                        es += " Please ensure report only assigned to one instructor. "
-                        ERRORS[ins].append(es)
-                        continue
-
-                    all_groups.append( (ins, sid, g) )
-
-    ipath = paths['instructor_project_evaluations']
-    for f in glob.glob(ipath +"/PARSE_ERRORS_*.txt" ):
-        os.remove(f)
-
-    for ins in ERRORS:
-        if ERRORS[ins]:
-            ss = '\n'.join(ERRORS[ins])
-            with open(ipath +"/PARSE_ERRORS_" + ins + ".txt",'w') as f:
-                f.write(ss)
-
-
-def get_template():
-    paths = get_paths()
-    return paths['project_evaluations_template.xlsx']
-
-
-def get_instructor_xlsx_files(info, sheet):
-    ss = "groups" if sheet == 0 else "report_%i"%sheet
-    xlsx = []
-    ins_names = [ins['shortname'] for ins in info['instructors']]
-    ins_names.append("transfer")
-
-    paths = get_paths()
-    instructor_path = paths['instructor_project_evaluations']
-
-    for ins in ins_names:
-        ns = instructor_path + "/02450_"+semester_id()+"_" + ss + "_" + ins+".xlsx"
-        xlsx.append( (ns,ins) )
-    return xlsx
-
-
-def get_groups_from_learn_xslx_file(paths, sheet_number):
-    fname = f"{paths['instructor_project_evaluations']}/groups{sheet_number}.xlsx"
-    all_groups = []
-    if os.path.exists(fname):
-        # Reading from the groups{number}.xlsx group-id file exported from DTU learn. Note this file contains fuckups.
-        dg = defaultdict(list)
-        df = pd.read_excel(fname)
-        for uname, group_id in zip(df['Username'], df['Project groups']):
-            id = int(group_id.split(" ")[1])
-            if len(uname) == 7 and uname[0] == 's':
-                dg[id].append(uname)
-            else:
-                dg[id].append("DTU-LEARN-FUCKED-THIS-ID-UP-CHECK-ON-REPORT")
-
-        all_groups = [{'group_id': id, 'student_ids': students} for id, students in dg.items()]
-    return all_groups
-
-
-def group_id_from_file(file):
-    id = int(os.path.dirname(file).split(" - ")[1].split(" ")[1])
-    return id
-
-def search_projects(paths, sheet_number, patterns):
-    zip_files = [paths['instructor_project_evaluations'] + "/zip%d.zip" % sheet_number]
-    # print(zip_files)
-
-    all_groups = []
-    gps = defaultdict(list)
-    for zip_file in zip_files:
-        if os.path.exists(zip_file):
-            tmpdir = tempfile.TemporaryDirectory()
-            zipfile.ZipFile(zip_file).extractall(path=tmpdir.name)
-
-            # Read from PDF files:
-            pdfs = glob.glob(tmpdir.name + "/**/*.pdf", recursive=True)
-            for pdf in pdfs:
-                pdf_parsed = tika.parser.from_file(pdf)
-                id =group_id_from_file(pdf) # int(os.path.dirname(pdf).split(" - ")[1].split(" ")[1])
-                if pdf_parsed['content'] is None:
-                    students = []
-                    print("> Finding student ID. Warning: The pdf file", pdf, "appers to have no text content.")
-                else:
-                    students = re.findall('s\d\d\d\d\d\d', pdf_parsed['content'], flags=re.IGNORECASE)
-                gps[id] += students
-
-            # Collect from .tex files:
-
-            # recursive_tex_collect()
-            texs = glob.glob(tmpdir.name + "/**/*.tex", recursive=True)
-            for tex in texs:
-                id = group_id_from_file(tex)
-                tex_parsed = recursive_tex_collect(tex)
-                tex_parsed = "\n".join([(l[:l.find("%")] if "%" in l else l) for l in tex_parsed.splitlines()])
-                students = re.findall('s\d\d\d\d\d\d', tex_parsed, flags=re.IGNORECASE)
-                gps[id] += students
-
-    for id, students in gps.items():
-        all_groups.append({'group_id': id, 'student_ids': list(set(students))})
-    return all_groups
-
-
-def unpack_zip_file_recursively(zip_file, destination_dir):
-    """
-    Unpack the zip_file (extension: .zip) to the given directory.
-
-    If the folders in the zip file contains other zip/files, these are unpacked recursively.
-    """
-    # Unpack zip file recursively and flatten it.
-    zipfile.ZipFile(zip_file).extractall(path=destination_dir)
-    ls = glob.glob(destination_dir + "/*")
-    for f in ls:
-        if os.path.isdir(f):
-            zipfiles = glob.glob(f + "/*.zip")
-            for zp in zipfiles:
-                print("Unpacking student zip file>", zp)
-                zipfile.ZipFile(zp).extractall(path=os.path.dirname(zp) + "/")
-
-
-def copy_populate_from_template(paths, info, sheet_number,zip_file):
-    # Try to load group ids from the project pdf's
-    all_groups = search_projects(paths, sheet_number, r"s\d{6}")
-    # all_groups = get_groups_from_learn_xslx_file(paths, sheet_number)
-    if len(all_groups) == 0:
-        all_groups = projects_info.get_groups_from_report(repn=sheet_number-1) if sheet_number > 0 else []
-    # Hopefully this did the trick and we have the groups all grouped up.
-
-    # set up which TA approve which TA
-    if any( [i['language'] not in ["en", "any"] for i in info['instructors'] ]):
-        print(info['instructors'])
-        raise Exception("An instructor does not have a language set. Please fix in main configuration file")
-    langs = ["en", "any"]
-    ifiles = get_instructor_xlsx_files(info, sheet_number)
-    all_tas = {}
-    for la in langs:
-        tas = [i for i in info['instructors'] if i['language'] == la]
-        active_tas = [t for t in tas if t['maxreports'] > 0]
-        dead_tas = [t for t in tas if t['maxreports'] <= 0]
-
-        for j, ta in enumerate(active_tas):
-            sn = ta['shortname']
-            all_tas[sn] = ta
-            all_tas[sn]['approver'] = active_tas[(j + 1) % len(active_tas)]['shortname']
-            all_tas[sn]['handins'] = []
-
-        for j, ta in enumerate(dead_tas):
-            sn = ta['shortname']
-            all_tas[sn] = ta
-            all_tas[sn]['approver'] = sn # dead dude approves himself
-            all_tas[sn]['handins'] = []
-
-    all_tas['transfer'] = {'maxreports': 0, 'language': 'any', 'approver': 'transfer', 'handins': []}
-
-    for (fn, name) in ifiles:
-        all_tas[name]['ifile'] = fn
-
-    # how many groups per instructor should be preset. Larger for report 0 (group registration).
-    n_groups_per_instructor = 24 + (sheet_number == 0) * 26
-
-    if sheet_number > 0:
-        # zfd = zip_file[:-4]
-        # if not os.path.exists(zfd):
-        #     os.mkdir(zfd)
-        zfd = tempfile.TemporaryDirectory().name
-        # zipfile.ZipFile(zip_file).extractall(path=tmpdir.name)
-
-        unpack_zip_file_recursively(zip_file, destination_dir=zfd)
-        # get all report handins (i.e. directories)
-        ls = [l for l in glob.glob(zfd + "/*") if l[-3:] not in ["txt", "tml"]]
-
-        handins = []
-        handins_duplicated = [] # for duplicated handins. i.e. handins with existing student id's.
-        protected_ids = []
-        handins_MD5 = {}
-
-        group_id_counter = 1000
-        for l in ls:
-            pdf_md5 = None
-            lpdfs = glob.glob(l + "/*.pdf")
-            try:
-                group_id = int(os.path.basename(l).split("-")[2].strip().split(" ")[1])
-            except Exception as e:
-                group_id = group_id_counter
-                group_id_counter = group_id_counter + 1
-
-            if len(lpdfs) > 0:
-                pdf = lpdfs.pop()
-                try:
-                    raw = parser.from_file(pdf)
-                    if not 'content' in raw:
-                        print("parse error; unable to parse pdf content. File is probably a bit fucky")
-                        lang = "da"
-                    else:
-                        lang = langdetect.detect(raw['content'])
-                    print(lang + ": " + pdf)
-                    if lang != "en":
-                        lang = "da"
-                except Exception as e:
-                    print("Bad encoding")
-                    lang = "da"
-                # Compute MD5 hash of file:
-            else:
-                lang = "da"
-
-            hi = {'path': l, 'group_id': group_id, 'lang': lang, 'pdf_hash': pdf_md5}
-            handins.append(hi)
-
-        # fix error file about already handed in reports:
-        used_students = []
-        for h in handins:
-            gid = h['group_id']
-            # sid = h['student_id']
-            gws = []
-            for g in all_groups:
-                if g['group_id'] is not None and g['group_id'] == gid:
-                    # if sid in g['student_ids']:
-                    gws += [s for s in g["student_ids"] if s not in protected_ids + used_students]
-                    used_students += gws
-            h['group'] = gws
-
-        ta_report_langs = [(["any"], ["da"]), (["en", "any"], ["da", "en"])]
-
-        assigned_handins = []
-        for ta_l, ra_l in ta_report_langs:
-            for num, h in enumerate(handins):
-                if h['lang'] not in ra_l or num in assigned_handins:
-                    continue
-                assigned_handins.append(num)
-                TA_names = [k for k in all_tas if all_tas[k]['language'] in ta_l]
-                # compute number of groups per TA
-                nn = [len(all_tas[n]['handins']) + 100 * (all_tas[n]['maxreports'] <= len(all_tas[n]['handins'])) for n in TA_names]
-                i = np.argmin(nn)
-                all_tas[TA_names[i]]['handins'].append(h)
-
-        assert( sum([ len(all_tas[n]['handins']) for n in all_tas] ) == len(handins) )
-
-        # Saving report assignment summary to .txt file for later reference
-        summary_txt = "%s/report_%i_summary.txt"%(os.path.dirname(zip_file), sheet_number)
-        with open(summary_txt, 'w') as f:
-            ss = ["TA,    Approver,   number-of-reports,   group_ids,    Students"]
-            for ta in all_tas:
-                # for s in all_tas['niels']['students']
-                handins_students = [', '.join(ha['group']) for ha in all_tas[ta]['handins'] ]
-                handins_groups = ", ".join( [str(ha['group_id']) for ha in all_tas[ta]['handins'] ] )
-                nha = len(handins_students)
-                approver = all_tas[ta]['approver']
-                # handins_groups
-                ss.append(f'{ta}, {approver}, {nha},     ({handins_groups}),   ({", ".join(handins_students)})')
-            f.write('\n'.join(ss))
-
-    # write actual .xlsx files:
-    template = get_template()
-    for shortname in all_tas:
-        ifile = all_tas[shortname]['ifile']
-        corrector = all_tas[shortname]['approver']
-        if sheet_number > 0:
-            # Copy reports to directory (distribute amongst TAs)
-            # b_dir = os.path.dirname(zip_file)
-            ins_dir = "%s/project_%i_%s/"%(zfd, sheet_number, shortname)
-
-            if not os.path.exists(ins_dir):
-                os.mkdir(ins_dir)
-
-            for handin in all_tas[shortname]['handins']:
-                shutil.move(handin['path'], ins_dir)
-
-            shutil.make_archive(os.path.dirname(zip_file) +"/"+ os.path.basename(ins_dir[:-1]), 'zip', ins_dir)
-            time.sleep(2)
-            print("Removing tree of reports to clear up space...")
-            shutil.rmtree(ins_dir)
-
-        if os.path.exists(ifile):
-            raise Exception("File already exists")
-        shutil.copyfile(template, ifile)
-        wb = openpyxl.load_workbook(ifile)
-        for wdex, ws in enumerate(wb.worksheets):
-            if wdex != sheet_number:
-                wb.remove(ws)
-        ccol = 2
-        sheet = wb.worksheets[0]
-        if sheet_number > 0:
-            sheet = write_dropdown_sumprod_sheet(sheet)
-
-        handins_assigned_to_this_ta = all_tas[shortname]['handins']
-        for i in range(len(handins_assigned_to_this_ta) + n_groups_per_instructor):
-            sheet.cell(INSTRUCTOR_ROW, ccol + i).value = shortname
-            if sheet_number > 0:
-                if i < len(handins_assigned_to_this_ta):
-                    sheet.cell(STUDENT_ID_ROW -1, ccol + i).value = handins_assigned_to_this_ta[i]['group_id']
-                sheet.cell(INSTRUCTOR_ROW+1, ccol + i).value = corrector
-                if i < len(handins_assigned_to_this_ta ):
-                    gg = handins_assigned_to_this_ta[i]['group']
-
-                    for j,s in enumerate(gg):
-                        sheet.cell(STUDENT_ID_ROW+j, ccol+i).value = s
-        wb.save(ifile)
-        wb.close()
-    # clean up zip file directories; since it is a tmp file, we don't have to.
-    # if sheet_number > 0:
-    #     zfd = zip_file[:-4]
-    #     shutil.rmtree(zfd)
-
-def write_dropdown_sumprod_sheet(sheet):
-    ccol = 2
-    for i in range(300):    # write 300 columns of sumprod, dropdowns. Good for courses of size up to about 800 students
-        for j in range(EVALUATION_ROW_END - EVALUATION_ROW_START + 1):
-            jj = j + WEIGHT_ROW_START
-            min_value = sheet.cell(jj, RANGE_MIN_COL).value
-            max_value = sheet.cell(jj, RANGE_MIN_COL + 1).value
-            if max_value:
-
-                rng = range(min_value, max_value + 1) if min_value >= 0 else [j for j in np.linspace(min_value, max_value, 5).flat]
-                fml = '"' + ",".join([str(x) for x in rng]) + ',"'
-                if min_value < 0:
-                    fml = f"B{DELTA_ALLOWED_ROW}:N{DELTA_ALLOWED_ROW}"
-
-                data_val = DataValidation(type="list", formula1=fml, allow_blank=True)
-                sheet.add_data_validation(data_val)
-
-                my_cell = sheet.cell(j + EVALUATION_ROW_START, i + ccol)
-                data_val.add(my_cell)
-
-            cl1 = get_column_letter(i + ccol)
-            dfml1 = '%s%i:%s%i' % (cl1, EVALUATION_ROW_START, cl1, EVALUATION_ROW_END)
-            cl2 = get_column_letter(RANGE_MIN_COL - 1)
-            dfml2 = '$%s$%i:$%s$%i' % (
-            cl2, WEIGHT_ROW_START, cl2, WEIGHT_ROW_START + EVALUATION_ROW_END - EVALUATION_ROW_START)
-            fml2 = '=4*SUMPRODUCT(%s, %s)' % (dfml1, dfml2)
-            sheet[get_column_letter(i + ccol) + str(EVALUATION_ROW_END + 1)] = fml2
-    return sheet
-
-def distribute_zip_content(info, sheet, zf_base):
-    xs = get_instructor_xlsx_files(info, sheet)
-    for x, TAname in xs:
-        if not os.path.exists(x): continue
-        if TAname == "transfer": continue
-        wb = openpyxl.load_workbook(x)
-        ws_x = ([wb.worksheets[0]] + [ws for ws in wb.worksheets if ws.title == "Ark1"]).pop()
-        all_students = []
-        for col_ins in range(1, ws_x.max_column):
-            group = parse_column(ws_x, report_number=sheet, column=col_ins + 1)
-            all_students += group.get('student_ids', [])
-
-        import zipfile
-        b_dir = os.path.dirname(zf_base)
-        ins_dir = "%s/project_%i_%s/"%(b_dir, sheet, TAname)
-        if not os.path.exists(ins_dir): os.mkdir(ins_dir)
-
-        with zipfile.ZipFile(zf_base) as zf:
-            for cfile in zf.namelist():
-                for sid in all_students:
-                    if cfile.startswith(sid +'/'):
-                        zf.extract(cfile, ins_dir)
-
-        shutil.make_archive(ins_dir[:-1], 'zip', ins_dir)
-
-
-# Gather instructor sheets and save to main file
-def gather_instructor_sheets(info):
-    out = get_output_file()
-    print("Gathering instructor sheets and saving them to file: ")
-    print(" > %s"%out)
-    template = get_template()
-    shutil.copyfile(template, out)
-    ts = openpyxl.load_workbook(out)
-
-    for sheet in range(4):
-        xs = get_instructor_xlsx_files(info,sheet)
-        col_temp = 1
-
-        for x, TAname in xs:
-            if not os.path.exists(x): continue
-            wb = openpyxl.load_workbook(x)
-            ws_x = ([wb.worksheets[0]] + [ws for ws in wb.worksheets if ws.title == "Ark1"]).pop()
-            tagroups = 0
-
-            for col_ins in range(1,ws_x.max_column):
-                group = parse_column(ws_x, report_number=sheet,column=col_ins+1)
-
-                if len(group['student_ids']) > 0:
-                    for r in range(ws_x.max_row):
-                        if r > 50:
-                            continue # don't write the part about evaluating the sheet; the TAs tend to fuck that part up.
-                        dv = ws_x.cell(r+1, col_ins+1)
-                        ts.worksheets[sheet].cell(r+1, col_temp+1, dv.value)
-                    col_temp += 1
-                    tagroups += 1
-
-            if tagroups == 0 and not TAname == "transfer":
-                print("TA: " + TAname + " sheet %i; groups found: %i" % (sheet, tagroups))
-                pass
-
-            wb.close()
-        if sheet >= 1:
-            write_dropdown_sumprod_sheet(ts.worksheets[sheet] )
-
-    ts.save(out)
-    ts.close()
-    print("Collected xlsx instructor files. Using xlwings to load main worksheet, evaluate and save it")
-
-    book = xw.Book(out)
-    book.save(out)
-    book.close()
-
-
-def weave_distribute_groups(info, groups, handins, shortnames):
-    groups2 = []
-    BG = 0
-    set([g.get('instructor', "") for g in groups])
-    for sid in handins:
-        fg = []
-        all_used_students = list(itertools.chain.from_iterable([g['student_ids'] for g in groups2]))
-        for g in groups:
-            if sid in g['student_ids'] and not any(set(g['student_ids'] ) & set(all_used_students)) :
-                fg.append(g)
-        if len(fg) > 0:
-            groups2.append(fg.pop())
-        else:
-            groups2.append({'student_ids': [sid]})
-            BG += 1
-    print("Fair assigning groups. Group changes since last assignment: %i (if large -> bad TA sheet)"%BG)
-    groups2 = fair_assign(info, groups2, shortnames=shortnames)
-    return groups2
-
-
-def _ta_maxrep_by_name(info, shortname):
-    ins = [ii for ii in info['instructors'] if ii['shortname'] == shortname].pop()
-    return ins['maxreports']
-
-def fair_assign(info, groups, shortnames):
-    shortnames_no_transfer = shortnames[:-1]
-    groups_by_instructor = {i: [] for i in shortnames}
-    n_groups = len(groups)
-    MAX_groups_per_instructor = math.ceil( len(groups) / len(shortnames_no_transfer) )
-    # take initial set of groups and assign them to instructors
-    rem_groups = []
-    for g in groups:
-        found = False
-        if "instructor" in g:
-            i = g["instructor"].lower()
-            maxreps = _ta_maxrep_by_name(info, i)
-            if i in shortnames_no_transfer and len(groups_by_instructor[i]) < min([MAX_groups_per_instructor, maxreps]):
-                groups_by_instructor[i].append(g)
-                found = True
-        if not found:
-            rem_groups.append(g)
-    for g in rem_groups:
-        ls = [ len(groups_by_instructor[i]) if len(groups_by_instructor[i]) < _ta_maxrep_by_name(info, shortname=i) else 1000 for i in shortnames_no_transfer]
-        m = np.argmin(ls)
-        m = shortnames_no_transfer[m]
-        groups_by_instructor[m].append(g)
-    a = [len(groups_by_instructor[i]) for i in shortnames]
-    for i in shortnames:
-        print(i + " %i"%len(groups_by_instructor[i]))
-    if sum(a) != n_groups:
-        raise Exception("Group lost during fair group assignment!")
-    return groups_by_instructor
-
-def mkboxplots(students,paths):
-    iscores = dict()
-    for repn in range(1, 4):
-        for k in students:
-            s = students[k]
-            g = s['reports'][repn]
-            if g:
-                gs = g['score']
-                ins = g['instructor']
-                if gs:
-                    v = iscores.get(ins,[[], [], []])
-                    v[repn-1].append(gs)
-                    iscores[ins] = v
-
-    NI = len(iscores.keys())
-    cols = get_colors(max_colors=NI)
-
-    def set_box_color(bp, color):
-        plt.setp(bp['boxes'], color=color)
-        plt.setp(bp['whiskers'], color=color)
-        plt.setp(bp['caps'], color=color)
-        plt.setp(bp['medians'], color=color)
-
-    ticks = ['Report 1', 'Report 2', 'Report 3']
-    plt.figure()
-    bpl = []
-    dw = 0.8
-    lg = []
-    for dex,ins in enumerate(iscores):
-        data_a = iscores[ins]
-        pst = np.array(range(len(data_a))) * (dw*(NI+2) ) + dw*dex
-        db = plt.boxplot(data_a, positions=pst, sym='', widths=dw * 0.6/0.8)
-        set_box_color(db, cols[dex])
-        bpl.append(db)
-        lg.append(ins)
-    for dex,t in enumerate(lg):
-        plt.plot([], c=cols[dex], label=t)
-    plt.legend(loc='center left', bbox_to_anchor=(1, 0.5))
-    plt.xlim([-1, (NI+2) * dw * 3 + 1])
-    plt.xticks([ (i+0.5) *  dw * NI for i in range(len(ticks))], ticks)
-    plt.ylabel("Report score")
-    plt.tight_layout()
-    plt.savefig(paths['instructor_project_evaluations'] + '/TA_scores.pdf')
-    plt.savefig(os.path.dirname(paths['collected_project_evaluations.xlsx']) + '/TA_scores.pdf')
-    plt.show()
-    plt.savefig('boxcompare.png')
+import re
+import tempfile
+import tika
+import os
+import shutil
+import openpyxl
+import numpy as np
+import itertools
+import math
+import glob
+from tika import parser
+from openpyxl.worksheet.datavalidation import DataValidation
+from openpyxl.utils import get_column_letter
+import matplotlib.pyplot as plt
+import langdetect
+import xlwings as xw
+from coursebox.core.projects_info import get_output_file, INSTRUCTOR_ROW, STUDENT_ID_ROW, parse_column
+from coursebox.core.projects_info import EVALUATION_ROW_END, EVALUATION_ROW_START, WEIGHT_ROW_START, RANGE_MIN_COL, DELTA_ALLOWED_ROW
+from coursebox.core.info import get_paths, class_information, semester_id
+from coursebox.core import projects_info
+from coursebox.core.projects_plagiarism import plagiarism_checker
+from jinjafy.cache import cache_contains_dir, cache_update_dir
+from jinjafy.plot.plot_helpers import get_colors
+import time
+from collections import defaultdict
+import zipfile
+import pandas as pd
+from slider.slide import recursive_tex_collect
+
+def get_dirs(zf):
+    zip = zipfile.ZipFile(zf)
+    fls = list(set([os.path.dirname(x) for x in zip.namelist()]))
+    fls = [f for f in fls if len(f) > 0]
+    return fls
+
+def fix_handins_fuckup(project_id=2):
+    """ Handle the problem with multiple hand-ins in DTU learn. """
+    paths = get_paths()
+    from coursebox.core.info import class_information
+    info = class_information()
+    zf = paths['instructor_project_evaluations'] + f"/zip{project_id}.zip"
+
+    tas = [i['shortname'] for i in info['instructors'] ]
+    ta_links = {i['shortname']: i for i in info['instructors']}
+
+    ta_reports = {}
+    for ta in tas:
+        fname = paths['instructor_project_evaluations']  + f"/project_{project_id}_{ta}.zip"
+        for r in get_dirs(fname):
+            if r in ta_reports:
+                raise Exception
+            ta_reports[r] = ta
+
+    fls = get_dirs(zf)
+    # fls = [f for f in zip.namelist() if not f.endswith("tml") and f.endswith("/")]
+    d = defaultdict(lambda: [])
+    for l in fls:
+        # print(l)
+        group_id = int(l.split("-")[2].strip().split(" ")[1])
+        date = l.split("-")[-1].strip().split(" ")
+        hm = date[-2]
+        if len(hm) < 4:
+            hm = "0" + hm
+        hm = hm[:2] + ":" + hm[2:]
+        date[-2] = hm
+        date = " ".join(date)
+        import datetime
+        date_time_obj = datetime.datetime.strptime(date, '%d %B, %Y %I:%M %p')
+
+        d[group_id].append( {'file': l, 'date': date_time_obj, 'ta': ta_reports[l], 'group_id': group_id } )
+
+    d = {k: v for k, v in d.items() if len(v)  > 1}
+
+    ta_do_not = defaultdict(lambda: [])
+    ta_do = defaultdict(lambda: [])
+    for group_id, reports in d.items():
+        recent = max( r['date'] for r in reports)
+        for r in reports:
+            if r['date'] == recent:
+                ta_do[r['ta']].append(r)
+            else:
+                ta_do_not[r['ta']].append(r)
+
+    fname = paths['instructor_project_evaluations'] + "/do_not_evaluate.txt"
+    with open(fname, 'w') as f:
+        for ta, reports in ta_do_not.items():
+            f.write(ta_links[ta ]['name'] + f" ({ta})" + "\n")
+            for r in reports:
+                f.write("DO NOT EVALUATE: " + r['file'] + "\n")
+            f.write("\n")
+            f.write("\n")
+    with open(fname, 'r') as f:
+        print(f.read())
+    return ta_do, ta_do_not
+
+
+def handle_projects(verbose=False, gather_main_xlsx_file=True, plagiarism_check=False):
+    paths = get_paths()
+    info = class_information()
+    if info['freeze_report_evaluation']:
+        print("> Report evaluations are FROZEN, meaning TA changes are no longer taken into account")
+        print("> grades, etc. now relies on report resource file:")
+        print(paths['collected_project_evaluations.xlsx'])
+    if info['CE']:
+        return
+    if plagiarism_check:
+        plagiarism_checker(paths, info)
+        return
+
+    instructor_path = paths['instructor_project_evaluations']
+    cache_changed_xlsx_files = False
+    if gather_main_xlsx_file:
+        cache_base = paths['instructor_project_evaluations']
+        if cache_contains_dir(cache_base,cache_base, pattern="*.xlsx") and os.path.exists(paths['collected_project_evaluations.xlsx']):
+            pass
+        else:
+            cache_changed_xlsx_files = True
+            gather_instructor_sheets(info)
+            print("> Done gathering main .xlsx file from instructor .xlsx files")
+            cache_update_dir(cache_base, cache_base, pattern="*.xlsx")
+            info = class_information()
+
+    zip1 = instructor_path + "/zip1.zip"
+    zip2 = instructor_path + "/zip2.zip"
+    zip3 = instructor_path + "/zip3.zip"
+    zips = [None, zip1, zip2, zip3]
+
+    for j,zf in enumerate(zips):
+        ifiles = get_instructor_xlsx_files(info, j)
+        ex =  [os.path.exists(f) for (f,_) in ifiles]
+        if any(ex) and not all(ex):
+            raise Exception("Partial list of instructor files") # ensure there are either no files or all files exist
+        instructor_files_exist = ex.pop()
+
+        if instructor_files_exist:
+            # if instructor files are there, we should do nothing
+            continue
+        else: # instructor files do not exist
+            if j == 0:
+                copy_populate_from_template(paths, info, sheet_number=j, zip_file=None)
+
+            elif os.path.exists(zf):
+                # make a copy of report template and populate it with groups obtained from previous report evaluation.
+                # all_groups = get_all_reports_from_collected_xlsx_file()
+                copy_populate_from_template(paths, info, sheet_number=j, zip_file=zf)
+                # distribute_zip_content(info, sheet=j, zf_base=zf)
+            else:
+                print("When available, please move downloaded copy of all reports from campusnet to destination:")
+                print(zf)
+
+    mkboxplots(info['students'],paths)
+
+    if cache_changed_xlsx_files:
+        # Recompute nag files if instructor xlsx files have been changed
+        compute_error_files(info, paths)
+    nags = []
+    fs = glob.glob(paths['instructor_project_evaluations'] + "/PARSE_ERRORS_*.txt")
+    for f in fs:
+        name = f.split("_").pop()[:-4]
+        if name != "transfer":
+            v = [i for i in info['instructors'] if i['shortname'] == name]
+            with open(f, "r") as file:
+                s = file.read()
+                nlines = len(s.split("\n"))
+            if len(v) == 0:
+                raise Exception("Empty instructor list. what the ...")
+
+            ins_email = v[0]['email']
+            nags.append((name, ins_email, nlines))
+    Nerrors = sum([n[-1] for n in nags])
+    if Nerrors > 0:
+        print("\n> %i errors. These instructors have parse errors (.txt)" % sum([n[-1] for n in nags]))
+        print("; ".join([email for (_, email, _) in nags]))
+        print(", ".join([name.capitalize() for (name, _, _) in nags]))
+        print("TA/Errors: " + ", ".join(["%s:%i" % (name.capitalize(), lines) for (name, _, lines) in nags]))
+        print("---")
+    else:
+        print("No parse errors found")
+
+
+def compute_error_files(info, paths):
+    print("Recomputing nag files...")
+    ERRORS = dict()
+    students = info['students']
+    for repn in range(3, -1, -1):
+        ifiles = get_instructor_xlsx_files(info, sheet=repn)
+        all_groups = []
+        for out, ins in ifiles:
+            if not os.path.exists(out):
+                continue
+
+            if not ins in ERRORS:
+                ERRORS[ins] = []
+
+            wb = openpyxl.load_workbook(out, data_only=True)
+            if len(wb.worksheets) > 1:
+                es = os.path.basename(out) + "> Entire workbook is malformed. Workbook must only contain a single sheet. Fix ASAP; aborting further operations."
+                ERRORS[ins].append(es)
+                continue
+
+            cls = []
+            for i in range(2, wb.worksheets[0].max_column + 1):
+                cp = projects_info.parse_column(wb.worksheets[0], report_number=repn, column=i)
+                if not cp['student_ids']:
+                    continue
+                cls.append(cp)
+
+            for g in cls:
+                gins = g.get('instructor')
+                err_label = "File: '%s', column with student ids: '%s'"%(os.path.basename(out), ', '.join(g['student_ids']))
+                if gins != ins:
+                    gins = "Null" if not gins else gins
+                    es = err_label +"> Corrupted sheet. Instructor name: '"  + gins + "' not found. Should perhaps be: '" + ins+"'?"
+                    print(es)
+                    ERRORS[ins].append(es)
+                    continue
+
+                if repn >= 1 and g.get("score", None) == None and len(g['student_ids'])>0:
+                    es = err_label + "> Report not scored."
+                    ERRORS[ins].append(es)
+
+                if repn >= 1 and len(g.get('student_ids', [])) > 0:
+                    if g.get('score', 0) is None:
+                        es = err_label + f"> Report does not have a score. The sheet may have been used incorrectly or fields are missing"
+                        ERRORS[ins].append(es)
+                    elif g.get("score", 0) < 0 or g.get("score", 0) > 4:
+                        es = err_label + f"> Report score is {g.get('score', 0)}. The report score has to be between 0 and 4; probably due to a too high value of 'Delta' in instructor sheet."
+                        ERRORS[ins].append(es)
+
+                if repn >= 1 and not g['comments'] and info['course_number'] != '02465':
+                    es = err_label + "> Incomplete report evaluation (missing comments field)"
+                    es += "Please fill out comments field in your excel sheet."
+                    ERRORS[ins].append(es)
+
+
+                if repn >= 1 and not g['approver_comments']  and info['course_number'] != '02465':
+                    es = err_label + "> Incomplete report evaluation (you are missing the approver comments field; can simply be set to 'ok')."
+                    ERRORS.get(g['approver'], []).append(es)
+
+                if g['missing_fields']:
+                    mf = g['missing_fields']
+                    es = err_label + "> Incomplete report evaluation (missing required evaluation-scoring field(s): '%s')."%(', '.join( [s for _,s in mf] ) ,)
+                    es += " Please fill out missing field in your excel sheet."
+                    ERRORS[ins].append(es)
+
+                for sid in g['student_ids']:
+                    # student = [student for student in students if student['id'] == sid]
+                    if repn >= 1 and sid not in students and False:
+                        # I disabled this since
+                        es = err_label + "> Student ID '%s' not found in registered students on campusnet. "%sid
+                        es += " To fix this, check if student is on campusnet under 'list of participants'; if he/she IS on campusnet, email me about the problem. " \
+                              + " Otherwise, simply delete extra students from sheet and send an email to all students in the group (the student likely dropped out of course)"
+
+                        ERRORS[ins].append( es )
+                        continue
+
+                    bad = [ (i, s, g) for (i,s,g) in all_groups if s == "sid"]
+                    if len(bad) > 0:
+                        i = bad[0][0]
+                        g2 = bad[0][2]
+
+                        es = err_label + "> Duplicate student ids for student: %s. " % (sid, )
+                        es += "Student is also found in sheet by instructor: " + i
+                        es += " in group with students: " + (", ".join( g2['student_ids'])) + ". "
+                        es += " Please ensure report only assigned to one instructor. "
+                        ERRORS[ins].append(es)
+                        continue
+
+                    all_groups.append( (ins, sid, g) )
+
+    ipath = paths['instructor_project_evaluations']
+    for f in glob.glob(ipath +"/PARSE_ERRORS_*.txt" ):
+        os.remove(f)
+
+    for ins in ERRORS:
+        if ERRORS[ins]:
+            ss = '\n'.join(ERRORS[ins])
+            with open(ipath +"/PARSE_ERRORS_" + ins + ".txt",'w') as f:
+                f.write(ss)
+
+
+def get_template():
+    paths = get_paths()
+    return paths['project_evaluations_template.xlsx']
+
+
+def get_instructor_xlsx_files(info, sheet):
+    ss = "groups" if sheet == 0 else "report_%i"%sheet
+    xlsx = []
+    ins_names = [ins['shortname'] for ins in info['instructors']]
+    ins_names.append("transfer")
+
+    paths = get_paths()
+    instructor_path = paths['instructor_project_evaluations']
+
+    for ins in ins_names:
+        ns = instructor_path + "/02450_"+semester_id()+"_" + ss + "_" + ins+".xlsx"
+        xlsx.append( (ns,ins) )
+    return xlsx
+
+
+def get_groups_from_learn_xslx_file(paths, sheet_number):
+    fname = f"{paths['instructor_project_evaluations']}/groups{sheet_number}.xlsx"
+    all_groups = []
+    if os.path.exists(fname):
+        # Reading from the groups{number}.xlsx group-id file exported from DTU learn. Note this file contains fuckups.
+        dg = defaultdict(list)
+        df = pd.read_excel(fname)
+        for uname, group_id in zip(df['Username'], df['Project groups']):
+            id = int(group_id.split(" ")[1])
+            if len(uname) == 7 and uname[0] == 's':
+                dg[id].append(uname)
+            else:
+                dg[id].append("DTU-LEARN-FUCKED-THIS-ID-UP-CHECK-ON-REPORT")
+
+        all_groups = [{'group_id': id, 'student_ids': students} for id, students in dg.items()]
+    return all_groups
+
+
+def group_id_from_file(file):
+    id = int(os.path.dirname(file).split(" - ")[1].split(" ")[1])
+    return id
+
+def search_projects(paths, sheet_number, patterns):
+    zip_files = [paths['instructor_project_evaluations'] + "/zip%d.zip" % sheet_number]
+    # print(zip_files)
+
+    all_groups = []
+    gps = defaultdict(list)
+    for zip_file in zip_files:
+        if os.path.exists(zip_file):
+            tmpdir = tempfile.TemporaryDirectory()
+            zipfile.ZipFile(zip_file).extractall(path=tmpdir.name)
+
+            # Read from PDF files:
+            pdfs = glob.glob(tmpdir.name + "/**/*.pdf", recursive=True)
+            for pdf in pdfs:
+                pdf_parsed = tika.parser.from_file(pdf)
+                id =group_id_from_file(pdf) # int(os.path.dirname(pdf).split(" - ")[1].split(" ")[1])
+                if pdf_parsed['content'] is None:
+                    students = []
+                    print("> Finding student ID. Warning: The pdf file", pdf, "appers to have no text content.")
+                else:
+                    students = re.findall('s\d\d\d\d\d\d', pdf_parsed['content'], flags=re.IGNORECASE)
+                gps[id] += students
+
+            # Collect from .tex files:
+
+            # recursive_tex_collect()
+            texs = glob.glob(tmpdir.name + "/**/*.tex", recursive=True)
+            for tex in texs:
+                id = group_id_from_file(tex)
+                tex_parsed = recursive_tex_collect(tex)
+                tex_parsed = "\n".join([(l[:l.find("%")] if "%" in l else l) for l in tex_parsed.splitlines()])
+                students = re.findall('s\d\d\d\d\d\d', tex_parsed, flags=re.IGNORECASE)
+                gps[id] += students
+
+    for id, students in gps.items():
+        all_groups.append({'group_id': id, 'student_ids': list(set(students))})
+    return all_groups
+
+
+def unpack_zip_file_recursively(zip_file, destination_dir):
+    """
+    Unpack the zip_file (extension: .zip) to the given directory.
+
+    If the folders in the zip file contains other zip/files, these are unpacked recursively.
+    """
+    # Unpack zip file recursively and flatten it.
+    zipfile.ZipFile(zip_file).extractall(path=destination_dir)
+    ls = glob.glob(destination_dir + "/*")
+    for f in ls:
+        if os.path.isdir(f):
+            zipfiles = glob.glob(f + "/*.zip")
+            for zp in zipfiles:
+                print("Unpacking student zip file>", zp)
+                zipfile.ZipFile(zp).extractall(path=os.path.dirname(zp) + "/")
+
+
+def copy_populate_from_template(paths, info, sheet_number,zip_file):
+    # Try to load group ids from the project pdf's
+    all_groups = search_projects(paths, sheet_number, r"s\d{6}")
+    # all_groups = get_groups_from_learn_xslx_file(paths, sheet_number)
+    if len(all_groups) == 0:
+        all_groups = projects_info.get_groups_from_report(repn=sheet_number-1) if sheet_number > 0 else []
+    # Hopefully this did the trick and we have the groups all grouped up.
+
+    # set up which TA approve which TA
+    if any( [i['language'] not in ["en", "any"] for i in info['instructors'] ]):
+        print(info['instructors'])
+        raise Exception("An instructor does not have a language set. Please fix in main configuration file")
+    langs = ["en", "any"]
+    ifiles = get_instructor_xlsx_files(info, sheet_number)
+    all_tas = {}
+    for la in langs:
+        tas = [i for i in info['instructors'] if i['language'] == la]
+        active_tas = [t for t in tas if t['maxreports'] > 0]
+        dead_tas = [t for t in tas if t['maxreports'] <= 0]
+
+        for j, ta in enumerate(active_tas):
+            sn = ta['shortname']
+            all_tas[sn] = ta
+            all_tas[sn]['approver'] = active_tas[(j + 1) % len(active_tas)]['shortname']
+            all_tas[sn]['handins'] = []
+
+        for j, ta in enumerate(dead_tas):
+            sn = ta['shortname']
+            all_tas[sn] = ta
+            all_tas[sn]['approver'] = sn # dead dude approves himself
+            all_tas[sn]['handins'] = []
+
+    all_tas['transfer'] = {'maxreports': 0, 'language': 'any', 'approver': 'transfer', 'handins': []}
+
+    for (fn, name) in ifiles:
+        all_tas[name]['ifile'] = fn
+
+    # how many groups per instructor should be preset. Larger for report 0 (group registration).
+    n_groups_per_instructor = 24 + (sheet_number == 0) * 26
+
+    if sheet_number > 0:
+        # zfd = zip_file[:-4]
+        # if not os.path.exists(zfd):
+        #     os.mkdir(zfd)
+        zfd = tempfile.TemporaryDirectory().name
+        # zipfile.ZipFile(zip_file).extractall(path=tmpdir.name)
+
+        unpack_zip_file_recursively(zip_file, destination_dir=zfd)
+        # get all report handins (i.e. directories)
+        ls = [l for l in glob.glob(zfd + "/*") if l[-3:] not in ["txt", "tml"]]
+
+        handins = []
+        handins_duplicated = [] # for duplicated handins. i.e. handins with existing student id's.
+        protected_ids = []
+        handins_MD5 = {}
+
+        group_id_counter = 1000
+        for l in ls:
+            pdf_md5 = None
+            lpdfs = glob.glob(l + "/*.pdf")
+            try:
+                group_id = int(os.path.basename(l).split("-")[2].strip().split(" ")[1])
+            except Exception as e:
+                group_id = group_id_counter
+                group_id_counter = group_id_counter + 1
+
+            if len(lpdfs) > 0:
+                pdf = lpdfs.pop()
+                try:
+                    raw = parser.from_file(pdf)
+                    if not 'content' in raw:
+                        print("parse error; unable to parse pdf content. File is probably a bit fucky")
+                        lang = "da"
+                    else:
+                        lang = langdetect.detect(raw['content'])
+                    print(lang + ": " + pdf)
+                    if lang != "en":
+                        lang = "da"
+                except Exception as e:
+                    print("Bad encoding")
+                    lang = "da"
+                # Compute MD5 hash of file:
+            else:
+                lang = "da"
+
+            hi = {'path': l, 'group_id': group_id, 'lang': lang, 'pdf_hash': pdf_md5}
+            handins.append(hi)
+
+        # fix error file about already handed in reports:
+        used_students = []
+        for h in handins:
+            gid = h['group_id']
+            # sid = h['student_id']
+            gws = []
+            for g in all_groups:
+                if g['group_id'] is not None and g['group_id'] == gid:
+                    # if sid in g['student_ids']:
+                    gws += [s for s in g["student_ids"] if s not in protected_ids + used_students]
+                    used_students += gws
+            h['group'] = gws
+
+        ta_report_langs = [(["any"], ["da"]), (["en", "any"], ["da", "en"])]
+
+        assigned_handins = []
+        for ta_l, ra_l in ta_report_langs:
+            for num, h in enumerate(handins):
+                if h['lang'] not in ra_l or num in assigned_handins:
+                    continue
+                assigned_handins.append(num)
+                TA_names = [k for k in all_tas if all_tas[k]['language'] in ta_l]
+                # compute number of groups per TA
+                nn = [len(all_tas[n]['handins']) + 100 * (all_tas[n]['maxreports'] <= len(all_tas[n]['handins'])) for n in TA_names]
+                i = np.argmin(nn)
+                all_tas[TA_names[i]]['handins'].append(h)
+
+        assert( sum([ len(all_tas[n]['handins']) for n in all_tas] ) == len(handins) )
+
+        # Saving report assignment summary to .txt file for later reference
+        summary_txt = "%s/report_%i_summary.txt"%(os.path.dirname(zip_file), sheet_number)
+        with open(summary_txt, 'w') as f:
+            ss = ["TA,    Approver,   number-of-reports,   group_ids,    Students"]
+            for ta in all_tas:
+                # for s in all_tas['niels']['students']
+                handins_students = [', '.join(ha['group']) for ha in all_tas[ta]['handins'] ]
+                handins_groups = ", ".join( [str(ha['group_id']) for ha in all_tas[ta]['handins'] ] )
+                nha = len(handins_students)
+                approver = all_tas[ta]['approver']
+                # handins_groups
+                ss.append(f'{ta}, {approver}, {nha},     ({handins_groups}),   ({", ".join(handins_students)})')
+            f.write('\n'.join(ss))
+
+    # write actual .xlsx files:
+    template = get_template()
+    for shortname in all_tas:
+        ifile = all_tas[shortname]['ifile']
+        corrector = all_tas[shortname]['approver']
+        if sheet_number > 0:
+            # Copy reports to directory (distribute amongst TAs)
+            # b_dir = os.path.dirname(zip_file)
+            ins_dir = "%s/project_%i_%s/"%(zfd, sheet_number, shortname)
+
+            if not os.path.exists(ins_dir):
+                os.mkdir(ins_dir)
+
+            for handin in all_tas[shortname]['handins']:
+                shutil.move(handin['path'], ins_dir)
+
+            shutil.make_archive(os.path.dirname(zip_file) +"/"+ os.path.basename(ins_dir[:-1]), 'zip', ins_dir)
+            time.sleep(2)
+            print("Removing tree of reports to clear up space...")
+            shutil.rmtree(ins_dir)
+
+        if os.path.exists(ifile):
+            raise Exception("File already exists")
+        shutil.copyfile(template, ifile)
+        wb = openpyxl.load_workbook(ifile)
+        for wdex, ws in enumerate(wb.worksheets):
+            if wdex != sheet_number:
+                wb.remove(ws)
+        ccol = 2
+        sheet = wb.worksheets[0]
+        if sheet_number > 0:
+            sheet = write_dropdown_sumprod_sheet(sheet)
+
+        handins_assigned_to_this_ta = all_tas[shortname]['handins']
+        for i in range(len(handins_assigned_to_this_ta) + n_groups_per_instructor):
+            sheet.cell(INSTRUCTOR_ROW, ccol + i).value = shortname
+            if sheet_number > 0:
+                if i < len(handins_assigned_to_this_ta):
+                    sheet.cell(STUDENT_ID_ROW -1, ccol + i).value = handins_assigned_to_this_ta[i]['group_id']
+                sheet.cell(INSTRUCTOR_ROW+1, ccol + i).value = corrector
+                if i < len(handins_assigned_to_this_ta ):
+                    gg = handins_assigned_to_this_ta[i]['group']
+
+                    for j,s in enumerate(gg):
+                        sheet.cell(STUDENT_ID_ROW+j, ccol+i).value = s
+        wb.save(ifile)
+        wb.close()
+    # clean up zip file directories; since it is a tmp file, we don't have to.
+    # if sheet_number > 0:
+    #     zfd = zip_file[:-4]
+    #     shutil.rmtree(zfd)
+
+def write_dropdown_sumprod_sheet(sheet):
+    ccol = 2
+    for i in range(300):    # write 300 columns of sumprod, dropdowns. Good for courses of size up to about 800 students
+        for j in range(EVALUATION_ROW_END - EVALUATION_ROW_START + 1):
+            jj = j + WEIGHT_ROW_START
+            min_value = sheet.cell(jj, RANGE_MIN_COL).value
+            max_value = sheet.cell(jj, RANGE_MIN_COL + 1).value
+            if max_value:
+
+                rng = range(min_value, max_value + 1) if min_value >= 0 else [j for j in np.linspace(min_value, max_value, 5).flat]
+                fml = '"' + ",".join([str(x) for x in rng]) + ',"'
+                if min_value < 0:
+                    fml = f"B{DELTA_ALLOWED_ROW}:N{DELTA_ALLOWED_ROW}"
+
+                data_val = DataValidation(type="list", formula1=fml, allow_blank=True)
+                sheet.add_data_validation(data_val)
+
+                my_cell = sheet.cell(j + EVALUATION_ROW_START, i + ccol)
+                data_val.add(my_cell)
+
+            cl1 = get_column_letter(i + ccol)
+            dfml1 = '%s%i:%s%i' % (cl1, EVALUATION_ROW_START, cl1, EVALUATION_ROW_END)
+            cl2 = get_column_letter(RANGE_MIN_COL - 1)
+            dfml2 = '$%s$%i:$%s$%i' % (
+            cl2, WEIGHT_ROW_START, cl2, WEIGHT_ROW_START + EVALUATION_ROW_END - EVALUATION_ROW_START)
+            fml2 = '=4*SUMPRODUCT(%s, %s)' % (dfml1, dfml2)
+            sheet[get_column_letter(i + ccol) + str(EVALUATION_ROW_END + 1)] = fml2
+    return sheet
+
+def distribute_zip_content(info, sheet, zf_base):
+    xs = get_instructor_xlsx_files(info, sheet)
+    for x, TAname in xs:
+        if not os.path.exists(x): continue
+        if TAname == "transfer": continue
+        wb = openpyxl.load_workbook(x)
+        ws_x = ([wb.worksheets[0]] + [ws for ws in wb.worksheets if ws.title == "Ark1"]).pop()
+        all_students = []
+        for col_ins in range(1, ws_x.max_column):
+            group = parse_column(ws_x, report_number=sheet, column=col_ins + 1)
+            all_students += group.get('student_ids', [])
+
+        import zipfile
+        b_dir = os.path.dirname(zf_base)
+        ins_dir = "%s/project_%i_%s/"%(b_dir, sheet, TAname)
+        if not os.path.exists(ins_dir): os.mkdir(ins_dir)
+
+        with zipfile.ZipFile(zf_base) as zf:
+            for cfile in zf.namelist():
+                for sid in all_students:
+                    if cfile.startswith(sid +'/'):
+                        zf.extract(cfile, ins_dir)
+
+        shutil.make_archive(ins_dir[:-1], 'zip', ins_dir)
+
+
+# Gather instructor sheets and save to main file
+def gather_instructor_sheets(info):
+    out = get_output_file()
+    print("Gathering instructor sheets and saving them to file: ")
+    print(" > %s"%out)
+    template = get_template()
+    shutil.copyfile(template, out)
+    ts = openpyxl.load_workbook(out)
+
+    for sheet in range(4):
+        xs = get_instructor_xlsx_files(info,sheet)
+        col_temp = 1
+
+        for x, TAname in xs:
+            if not os.path.exists(x): continue
+            wb = openpyxl.load_workbook(x)
+            ws_x = ([wb.worksheets[0]] + [ws for ws in wb.worksheets if ws.title == "Ark1"]).pop()
+            tagroups = 0
+
+            for col_ins in range(1,ws_x.max_column):
+                group = parse_column(ws_x, report_number=sheet,column=col_ins+1)
+
+                if len(group['student_ids']) > 0:
+                    for r in range(ws_x.max_row):
+                        if r > 50:
+                            continue # don't write the part about evaluating the sheet; the TAs tend to fuck that part up.
+                        dv = ws_x.cell(r+1, col_ins+1)
+                        ts.worksheets[sheet].cell(r+1, col_temp+1, dv.value)
+                    col_temp += 1
+                    tagroups += 1
+
+            if tagroups == 0 and not TAname == "transfer":
+                print("TA: " + TAname + " sheet %i; groups found: %i" % (sheet, tagroups))
+                pass
+
+            wb.close()
+        if sheet >= 1:
+            write_dropdown_sumprod_sheet(ts.worksheets[sheet] )
+
+    ts.save(out)
+    ts.close()
+    print("Collected xlsx instructor files. Using xlwings to load main worksheet, evaluate and save it")
+
+    book = xw.Book(out)
+    book.save(out)
+    book.close()
+
+
+def weave_distribute_groups(info, groups, handins, shortnames):
+    groups2 = []
+    BG = 0
+    set([g.get('instructor', "") for g in groups])
+    for sid in handins:
+        fg = []
+        all_used_students = list(itertools.chain.from_iterable([g['student_ids'] for g in groups2]))
+        for g in groups:
+            if sid in g['student_ids'] and not any(set(g['student_ids'] ) & set(all_used_students)) :
+                fg.append(g)
+        if len(fg) > 0:
+            groups2.append(fg.pop())
+        else:
+            groups2.append({'student_ids': [sid]})
+            BG += 1
+    print("Fair assigning groups. Group changes since last assignment: %i (if large -> bad TA sheet)"%BG)
+    groups2 = fair_assign(info, groups2, shortnames=shortnames)
+    return groups2
+
+
+def _ta_maxrep_by_name(info, shortname):
+    ins = [ii for ii in info['instructors'] if ii['shortname'] == shortname].pop()
+    return ins['maxreports']
+
+def fair_assign(info, groups, shortnames):
+    shortnames_no_transfer = shortnames[:-1]
+    groups_by_instructor = {i: [] for i in shortnames}
+    n_groups = len(groups)
+    MAX_groups_per_instructor = math.ceil( len(groups) / len(shortnames_no_transfer) )
+    # take initial set of groups and assign them to instructors
+    rem_groups = []
+    for g in groups:
+        found = False
+        if "instructor" in g:
+            i = g["instructor"].lower()
+            maxreps = _ta_maxrep_by_name(info, i)
+            if i in shortnames_no_transfer and len(groups_by_instructor[i]) < min([MAX_groups_per_instructor, maxreps]):
+                groups_by_instructor[i].append(g)
+                found = True
+        if not found:
+            rem_groups.append(g)
+    for g in rem_groups:
+        ls = [ len(groups_by_instructor[i]) if len(groups_by_instructor[i]) < _ta_maxrep_by_name(info, shortname=i) else 1000 for i in shortnames_no_transfer]
+        m = np.argmin(ls)
+        m = shortnames_no_transfer[m]
+        groups_by_instructor[m].append(g)
+    a = [len(groups_by_instructor[i]) for i in shortnames]
+    for i in shortnames:
+        print(i + " %i"%len(groups_by_instructor[i]))
+    if sum(a) != n_groups:
+        raise Exception("Group lost during fair group assignment!")
+    return groups_by_instructor
+
+def mkboxplots(students,paths):
+    iscores = dict()
+    for repn in range(1, 4):
+        for k in students:
+            s = students[k]
+            g = s['reports'][repn]
+            if g:
+                gs = g['score']
+                ins = g['instructor']
+                if gs:
+                    v = iscores.get(ins,[[], [], []])
+                    v[repn-1].append(gs)
+                    iscores[ins] = v
+
+    NI = len(iscores.keys())
+    cols = get_colors(max_colors=NI)
+
+    def set_box_color(bp, color):
+        plt.setp(bp['boxes'], color=color)
+        plt.setp(bp['whiskers'], color=color)
+        plt.setp(bp['caps'], color=color)
+        plt.setp(bp['medians'], color=color)
+
+    ticks = ['Report 1', 'Report 2', 'Report 3']
+    plt.figure()
+    bpl = []
+    dw = 0.8
+    lg = []
+    for dex,ins in enumerate(iscores):
+        data_a = iscores[ins]
+        pst = np.array(range(len(data_a))) * (dw*(NI+2) ) + dw*dex
+        db = plt.boxplot(data_a, positions=pst, sym='', widths=dw * 0.6/0.8)
+        set_box_color(db, cols[dex])
+        bpl.append(db)
+        lg.append(ins)
+    for dex,t in enumerate(lg):
+        plt.plot([], c=cols[dex], label=t)
+    plt.legend(loc='center left', bbox_to_anchor=(1, 0.5))
+    plt.xlim([-1, (NI+2) * dw * 3 + 1])
+    plt.xticks([ (i+0.5) *  dw * NI for i in range(len(ticks))], ticks)
+    plt.ylabel("Report score")
+    plt.tight_layout()
+    plt.savefig(paths['instructor_project_evaluations'] + '/TA_scores.pdf')
+    plt.savefig(os.path.dirname(paths['collected_project_evaluations.xlsx']) + '/TA_scores.pdf')
+    plt.show()
+    plt.savefig('boxcompare.png')
```

### Comparing `coursebox-0.1.8/src/coursebox/core/projects_info.py` & `coursebox-0.1.9/src/coursebox/core/projects_info.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,255 +1,254 @@
-from coursebox.core.info_paths import get_paths
-import os
-import re
-import openpyxl
-import numpy as np
-from line_profiler_pycharm import profile
-
-INSTRUCTOR_ROW = 6
-INSTRUCTOR_CHECKER_ROW = 31
-STUDENT_ID_ROW = 3
-STARS_ROW = 26
-
-EVALUATION_ROW_START = 8
-EVALUATION_ROW_END = 40
-WEIGHT_ROW_START = 63
-RANGE_MIN_COL = 5
-
-DELTA_ALLOWED_ROW = 111 # The range of possible delta-values. Should be in an empty (new) row at bottom.
-
-
-def parse_column_student_ids(v):
-    sn = []
-    if v is not None:
-        if isinstance(v, int):
-            v = str(v)
-            v = "s" + ("0"*(6-len(v))) + v
-        v = v.lower()
-        o = re.findall(r'(s\d{6})', v)
-        for g in o:
-            sn.append(g)
-    return sn
-
-
-def parse_column_numpy(col, report_number, column):
-    """ Parse a column assuming it is defined as a numpy array.
-    This is the recommended method as it is much, much faster.
-    """
-    # ws = worksheet  # wb.worksheets[sheet]
-    sn = []
-    group_id = col[STUDENT_ID_ROW - 1-1] #).value
-
-    # col = ['' if col[0] is np.NAN else x for x in col]
-
-    for i in range(0, 3):
-        v = col[i + STUDENT_ID_ROW-1]#, column=column).value
-        sn += parse_column_student_ids(v)
-
-
-    instructor = col[INSTRUCTOR_ROW-1]#, column=column).value
-    approver = col[INSTRUCTOR_ROW+1-1]# , column=column).value
-
-    if instructor:
-        instructor = instructor.lower()
-    if approver:
-        approver = str(approver).lower()
-
-    content = None
-    comments = None
-    appr_comments = None
-    if report_number > 0 and sn:
-        N = 38
-        rarr = np.ndarray(shape=(N,1),dtype=np.object)
-        for j in range(N):
-
-            v = col[3 + STUDENT_ID_ROW+j-1]#, column=column).value
-            rarr[j,0] = v
-        content = rarr
-        comments = col[EVALUATION_ROW_END+5-1]# , column=column).value
-        appr_comments = col[EVALUATION_ROW_END+6-1]# , column=column).value
-
-    cgroup = {'column_j': column, 'student_ids': sn, 'instructor': instructor, "approver": approver, 'content': content,
-              "comments": comments, "approver_comments": appr_comments, 'missing_fields': [],
-              'group_id': group_id}
-
-    # Now, find errors... This involves first finding non-zero columns
-    if report_number > 0 and sn:
-        score = cgroup['content'][-3, 0]
-        cgroup['score'] = score
-        cgroup['pct'] = score2pct(score)
-
-        # if report_number == 3: # this obviously needs fixing for next semester.
-        #     raise Exception("No report number 3 anymore. ")
-        #     I = []
-        #     for i in range(42): # max number of evaluation fields (irrelevant)
-        #         v1 = col[WEIGHT_ROW_START+i-1, RANGE_MIN_COL-1]# ).value
-        #         v2 = col[WEIGHT_ROW_START+i-1, RANGE_MIN_COL+1-1]#).value
-        #         if (v1 == -1 and v2 == 1) or (v1 == 0 and v2 == 4):
-        #             I.append(i)
-        #         if v1 == -1 and v2 == 1:
-        #             # print("delta col")
-        #             break
-        #
-        #     for i in I:
-        #         w1 = worksheet.cell(row=WEIGHT_ROW_START + i, column=1).value
-        #         w3_ = worksheet.cell(row=INSTRUCTOR_ROW + i+2, column=1).value # should agree with label in w1
-        #         w2 = worksheet.cell(row=INSTRUCTOR_ROW + i+2, column=column).value
-        #         if w2 == None:
-        #             cgroup['missing_fields'].append( (i, w1) )
-        #             if report_number < 3:
-        #                 print("old report nr.")
-
-    return cgroup
-
-
-
-def parse_column(worksheet, report_number, column):
-    """ This is the old method. It is very slow. Use the numpy-version above.
-    """
-    ws = worksheet  # wb.worksheets[sheet]
-    sn = []
-    group_id = ws.cell(row=STUDENT_ID_ROW - 1, column=column).value
-
-    for i in range(0, 3):
-        v = ws.cell(row=i + STUDENT_ID_ROW, column=column).value
-        sn += parse_column_student_ids(v)
-
-    instructor = ws.cell(row=INSTRUCTOR_ROW, column=column).value
-    approver = ws.cell(row=INSTRUCTOR_ROW+1, column=column).value
-
-    if instructor:
-        instructor = instructor.lower()
-    if approver:
-        approver = str(approver).lower()
-
-    content = None
-    comments = None
-    appr_comments = None
-    if report_number > 0 and sn:
-        N = 38
-        rarr = np.ndarray(shape=(N,1),dtype=np.object)
-        for j in range(N):
-            v = ws.cell(row=3 + STUDENT_ID_ROW+j, column=column).value
-            rarr[j,0] = v
-        content = rarr
-        comments = ws.cell(row=EVALUATION_ROW_END+5, column=column).value
-        appr_comments = ws.cell(row=EVALUATION_ROW_END+6, column=column).value
-
-    cgroup = {'column_j': column, 'student_ids': sn, 'instructor': instructor, "approver": approver, 'content': content,
-              "comments": comments, "approver_comments": appr_comments, 'missing_fields': [],
-              'group_id': group_id}
-
-    # Now, find errors... This involves first finding non-zero columns
-    if report_number > 0 and sn:
-        score = cgroup['content'][-3, 0]
-        cgroup['score'] = score
-        cgroup['pct'] = score2pct(score)
-
-        if report_number == 3: # this obviously needs fixing for next semester.
-            raise Exception("No report number 3 anymore. ")
-            I = []
-            for i in range(42): # max number of evaluation fields (irrelevant)
-                v1 = worksheet.cell(row=WEIGHT_ROW_START+i, column=RANGE_MIN_COL).value
-                v2 = worksheet.cell(row=WEIGHT_ROW_START+i, column=RANGE_MIN_COL+1).value
-                if (v1 == -1 and v2 == 1) or (v1 == 0 and v2 == 4):
-                    I.append(i)
-                if v1 == -1 and v2 == 1:
-                    # print("delta col")
-                    break
-
-            for i in I:
-                w1 = worksheet.cell(row=WEIGHT_ROW_START + i, column=1).value
-                w3_ = worksheet.cell(row=INSTRUCTOR_ROW + i+2, column=1).value # should agree with label in w1
-                w2 = worksheet.cell(row=INSTRUCTOR_ROW + i+2, column=column).value
-                if w2 == None:
-                    cgroup['missing_fields'].append( (i, w1) )
-                    if report_number < 3:
-                        print("old report nr.")
-
-    return cgroup
-
-def score2pct(score):
-    if score is None:
-        return None
-    if isinstance(score, str):
-        return score
-    else:
-        pct = score / 4
-        return pct
-
-def get_output_file():
-    out = get_paths()['collected_project_evaluations.xlsx']
-    if not os.path.exists(os.path.dirname(out)):
-        os.mkdir(os.path.dirname(out))
-    return out
-
-def get_groups_from_report(repn):
-    cls = []
-    out = get_output_file()
-    print("> Loading student report scores from: %s" % out)
-    wb = openpyxl.load_workbook(out, data_only=True)
-    # Perhaps find non-empty cols (i.e. those with content)
-    maximal_groups = []
-    maximal_groups_students = []
-
-    for i in range(2, wb.worksheets[repn].max_column + 1):
-        cp = parse_column(wb.worksheets[repn], report_number=repn, column=i)
-        if len(cp['student_ids']) == 0 or cp['group_id'] is None:
-            continue
-        cls.append(cp)
-    return cls
-
-
-# @profile
-def populate_student_report_results(students):
-    # take students (list-of-dicts in the info format) and assign them the results from the reports.
-    out = get_output_file()
-    import time
-    t0 = time.time()
-    print("> Loading student report scores from: %s"%out)
-    if not os.path.exists(out):
-        return students, []
-
-    for k in students:
-        students[k]['reports'] = {i: None for i in range(4)}
-    import pandas as pd
-
-    wb = openpyxl.load_workbook(out, data_only=True, read_only=True)
-    # Perhaps find non-empty cols (i.e. those with content)
-    print("> time elapsed", time.time() - t0)
-    maximal_groups = []
-    maximal_groups_students = []
-
-    for repn in range(3, -1, -1):
-        cls = []
-        sheet = pd.read_excel(out, sheet_name=repn, index_col=None, header=None)
-        sheet = sheet.fillna('')
-        sheet = sheet.to_numpy()
-        # to_numpy()
-        for i in range(1,sheet.shape[1]):
-
-            # for i in range(2, wb.worksheets[repn].max_column + 1):
-            # print(i, wb.worksheets[repn].max_column)
-            # s = pd.read_excel(out, sheet_name=1)
-            cp = parse_column_numpy(sheet[:,i], report_number=repn, column=i)
-
-
-            # cp = parse_column(wb.worksheets[repn], report_number=repn, column=i)
-            if not cp['student_ids']:
-                break
-            cls.append(cp)
-
-        for g in cls:
-            for sid in g['student_ids']:
-                student = students.get(sid, None)
-                if student is None:
-                    if repn > 0:  # don't care about project 0 (group registration)
-                        print("Bad error: Student id %s not found. report evaluation malformed?"%sid)
-                else:
-                    # student = student.pop()
-                    student['reports'][repn] = g
-                    if sid not in maximal_groups_students:
-                        maximal_groups.append(g)
-                        maximal_groups_students += g['student_ids']
-    print("> time elapsed", time.time() -t0)
+from coursebox.core.info_paths import get_paths
+import os
+import re
+import openpyxl
+import numpy as np
+from line_profiler_pycharm import profile
+
+INSTRUCTOR_ROW = 6
+INSTRUCTOR_CHECKER_ROW = 31
+STUDENT_ID_ROW = 3
+STARS_ROW = 26
+
+EVALUATION_ROW_START = 8
+EVALUATION_ROW_END = 40
+WEIGHT_ROW_START = 63
+RANGE_MIN_COL = 5
+
+DELTA_ALLOWED_ROW = 111 # The range of possible delta-values. Should be in an empty (new) row at bottom.
+
+
+def parse_column_student_ids(v):
+    sn = []
+    if v is not None:
+        if isinstance(v, int):
+            v = str(v)
+            v = "s" + ("0"*(6-len(v))) + v
+        v = v.lower()
+        o = re.findall(r'(s\d{6})', v)
+        for g in o:
+            sn.append(g)
+    return sn
+
+
+def parse_column_numpy(col, report_number, column):
+    """ Parse a column assuming it is defined as a numpy array.
+    This is the recommended method as it is much, much faster.
+    """
+    # ws = worksheet  # wb.worksheets[sheet]
+    sn = []
+    group_id = col[STUDENT_ID_ROW - 1-1] #).value
+
+    # col = ['' if col[0] is np.NAN else x for x in col]
+
+    for i in range(0, 3):
+        v = col[i + STUDENT_ID_ROW-1]#, column=column).value
+        sn += parse_column_student_ids(v)
+
+
+    instructor = col[INSTRUCTOR_ROW-1]#, column=column).value
+    approver = col[INSTRUCTOR_ROW+1-1]# , column=column).value
+
+    if instructor:
+        instructor = instructor.lower()
+    if approver:
+        approver = str(approver).lower()
+
+    content = None
+    comments = None
+    appr_comments = None
+    if report_number > 0 and sn:
+        N = 38
+        rarr = np.ndarray(shape=(N,1),dtype=np.dtype(object))
+        for j in range(N):
+            v = col[3 + STUDENT_ID_ROW+j-1]#, column=column).value
+            rarr[j,0] = v
+        content = rarr
+        comments = col[EVALUATION_ROW_END+5-1]# , column=column).value
+        appr_comments = col[EVALUATION_ROW_END+6-1]# , column=column).value
+
+    cgroup = {'column_j': column, 'student_ids': sn, 'instructor': instructor, "approver": approver, 'content': content,
+              "comments": comments, "approver_comments": appr_comments, 'missing_fields': [],
+              'group_id': group_id}
+
+    # Now, find errors... This involves first finding non-zero columns
+    if report_number > 0 and sn:
+        score = cgroup['content'][-3, 0]
+        cgroup['score'] = score
+        cgroup['pct'] = score2pct(score)
+
+        # if report_number == 3: # this obviously needs fixing for next semester.
+        #     raise Exception("No report number 3 anymore. ")
+        #     I = []
+        #     for i in range(42): # max number of evaluation fields (irrelevant)
+        #         v1 = col[WEIGHT_ROW_START+i-1, RANGE_MIN_COL-1]# ).value
+        #         v2 = col[WEIGHT_ROW_START+i-1, RANGE_MIN_COL+1-1]#).value
+        #         if (v1 == -1 and v2 == 1) or (v1 == 0 and v2 == 4):
+        #             I.append(i)
+        #         if v1 == -1 and v2 == 1:
+        #             # print("delta col")
+        #             break
+        #
+        #     for i in I:
+        #         w1 = worksheet.cell(row=WEIGHT_ROW_START + i, column=1).value
+        #         w3_ = worksheet.cell(row=INSTRUCTOR_ROW + i+2, column=1).value # should agree with label in w1
+        #         w2 = worksheet.cell(row=INSTRUCTOR_ROW + i+2, column=column).value
+        #         if w2 == None:
+        #             cgroup['missing_fields'].append( (i, w1) )
+        #             if report_number < 3:
+        #                 print("old report nr.")
+
+    return cgroup
+
+
+
+def parse_column(worksheet, report_number, column):
+    """ This is the old method. It is very slow. Use the numpy-version above.
+    """
+    ws = worksheet  # wb.worksheets[sheet]
+    sn = []
+    group_id = ws.cell(row=STUDENT_ID_ROW - 1, column=column).value
+
+    for i in range(0, 3):
+        v = ws.cell(row=i + STUDENT_ID_ROW, column=column).value
+        sn += parse_column_student_ids(v)
+
+    instructor = ws.cell(row=INSTRUCTOR_ROW, column=column).value
+    approver = ws.cell(row=INSTRUCTOR_ROW+1, column=column).value
+
+    if instructor:
+        instructor = instructor.lower()
+    if approver:
+        approver = str(approver).lower()
+
+    content = None
+    comments = None
+    appr_comments = None
+    if report_number > 0 and sn:
+        N = 38
+        rarr = np.ndarray(shape=(N,1),dtype=np.dtype(object))
+        for j in range(N):
+            v = ws.cell(row=3 + STUDENT_ID_ROW+j, column=column).value
+            rarr[j,0] = v
+        content = rarr
+        comments = ws.cell(row=EVALUATION_ROW_END+5, column=column).value
+        appr_comments = ws.cell(row=EVALUATION_ROW_END+6, column=column).value
+
+    cgroup = {'column_j': column, 'student_ids': sn, 'instructor': instructor, "approver": approver, 'content': content,
+              "comments": comments, "approver_comments": appr_comments, 'missing_fields': [],
+              'group_id': group_id}
+
+    # Now, find errors... This involves first finding non-zero columns
+    if report_number > 0 and sn:
+        score = cgroup['content'][-3, 0]
+        cgroup['score'] = score
+        cgroup['pct'] = score2pct(score)
+
+        if report_number == 3: # this obviously needs fixing for next semester.
+            raise Exception("No report number 3 anymore. ")
+            I = []
+            for i in range(42): # max number of evaluation fields (irrelevant)
+                v1 = worksheet.cell(row=WEIGHT_ROW_START+i, column=RANGE_MIN_COL).value
+                v2 = worksheet.cell(row=WEIGHT_ROW_START+i, column=RANGE_MIN_COL+1).value
+                if (v1 == -1 and v2 == 1) or (v1 == 0 and v2 == 4):
+                    I.append(i)
+                if v1 == -1 and v2 == 1:
+                    # print("delta col")
+                    break
+
+            for i in I:
+                w1 = worksheet.cell(row=WEIGHT_ROW_START + i, column=1).value
+                w3_ = worksheet.cell(row=INSTRUCTOR_ROW + i+2, column=1).value # should agree with label in w1
+                w2 = worksheet.cell(row=INSTRUCTOR_ROW + i+2, column=column).value
+                if w2 == None:
+                    cgroup['missing_fields'].append( (i, w1) )
+                    if report_number < 3:
+                        print("old report nr.")
+
+    return cgroup
+
+def score2pct(score):
+    if score is None:
+        return None
+    if isinstance(score, str):
+        return score
+    else:
+        pct = score / 4
+        return pct
+
+def get_output_file():
+    out = get_paths()['collected_project_evaluations.xlsx']
+    if not os.path.exists(os.path.dirname(out)):
+        os.mkdir(os.path.dirname(out))
+    return out
+
+def get_groups_from_report(repn):
+    cls = []
+    out = get_output_file()
+    print("> Loading student report scores from: %s" % out)
+    wb = openpyxl.load_workbook(out, data_only=True)
+    # Perhaps find non-empty cols (i.e. those with content)
+    maximal_groups = []
+    maximal_groups_students = []
+
+    for i in range(2, wb.worksheets[repn].max_column + 1):
+        cp = parse_column(wb.worksheets[repn], report_number=repn, column=i)
+        if len(cp['student_ids']) == 0 or cp['group_id'] is None:
+            continue
+        cls.append(cp)
+    return cls
+
+
+# @profile
+def populate_student_report_results(students):
+    # take students (list-of-dicts in the info format) and assign them the results from the reports.
+    out = get_output_file()
+    import time
+    t0 = time.time()
+    print("> Loading student report scores from: %s"%out)
+    if not os.path.exists(out):
+        return students, []
+
+    for k in students:
+        students[k]['reports'] = {i: None for i in range(4)}
+    import pandas as pd
+
+    wb = openpyxl.load_workbook(out, data_only=True, read_only=True)
+    # Perhaps find non-empty cols (i.e. those with content)
+    print("> time elapsed", time.time() - t0)
+    maximal_groups = []
+    maximal_groups_students = []
+
+    for repn in range(3, -1, -1):
+        cls = []
+        sheet = pd.read_excel(out, sheet_name=repn, index_col=None, header=None)
+        sheet = sheet.fillna('')
+        sheet = sheet.to_numpy()
+        # to_numpy()
+        for i in range(1,sheet.shape[1]):
+
+            # for i in range(2, wb.worksheets[repn].max_column + 1):
+            # print(i, wb.worksheets[repn].max_column)
+            # s = pd.read_excel(out, sheet_name=1)
+            cp = parse_column_numpy(sheet[:,i], report_number=repn, column=i)
+
+
+            # cp = parse_column(wb.worksheets[repn], report_number=repn, column=i)
+            if not cp['student_ids']:
+                break
+            cls.append(cp)
+
+        for g in cls:
+            for sid in g['student_ids']:
+                student = students.get(sid, None)
+                if student is None:
+                    if repn > 0:  # don't care about project 0 (group registration)
+                        print("Bad error: Student id %s not found. report evaluation malformed?"%sid)
+                else:
+                    # student = student.pop()
+                    student['reports'][repn] = g
+                    if sid not in maximal_groups_students:
+                        maximal_groups.append(g)
+                        maximal_groups_students += g['student_ids']
+    print("> time elapsed", time.time() -t0)
     return students, maximal_groups
```

### Comparing `coursebox-0.1.8/src/coursebox/core/projects_plagiarism.py` & `coursebox-0.1.9/src/coursebox/core/projects_plagiarism.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,140 +1,140 @@
-from tinydb import TinyDB, Query
-import os
-import zipfile
-from tinydb import TinyDB, Query, where
-import glob
-import pycode_similar
-import numpy as np
-import matplotlib.pyplot as plt
-
-# Update for later: Add code to copy current .zip file content to special (archived) files. Then load these files into DB later.
-# Structure should be extended to include semester structure.
-
-def plagiarism_checker(paths,info):
-    db = insert_projects(paths,info)
-    for repn in range(1, 4):
-        d = [v for v in db if v['code'] and v['report-number'] == repn]
-        if len(d) == 0:
-            continue
-
-        M = np.zeros( shape = (len(d), len(d)) )
-        for i,d1 in enumerate(d):
-            for j, d2 in enumerate(d):
-                if i < j:
-                    x = compare(d1['code'],d2['code'])
-                    M[i,j] = x
-            print(i)
-
-        plt.imshow(M)
-        plt.colorbar()
-        plt.title("Report number %i"%repn)
-        plt.show()
-
-        aa = np.flip( np.argsort( M.ravel()),axis=0)[:10]
-        ii,jj = np.unravel_index(aa, M.shape)
-        for dx in range(len(aa)):
-            i = ii[dx]
-            j = jj[dx]
-            s1 = d[i]['code'].split("\n")
-            s2 = d[j]['code'].split("\n")
-
-            bp = os.path.dirname(paths['collected_project_evaluations.xlsx']) + "/plagiarism"
-            if not os.path.exists(bp):
-                os.mkdir(bp)
-            bp = bp + "/report_%i"%repn
-            if not os.path.exists(bp):
-                os.mkdir(bp)
-            dout = bp + "/%.2f_%i_%i"%(M[i,j], i,j)
-            if not os.path.exists(dout):
-                os.mkdir(dout)
-
-            with open(dout + "/s1.txt", 'w') as f:
-                mark(f, s1, s2)
-
-            with open(dout + "/s2.txt", 'w') as f:
-                mark(f, s2, s1)
-
-            with open(dout + "/sim.txt", 'w') as f:
-                ss = [s for s in s2 if s in s1]
-                f.write("\n".join(ss))
-
-def get_toolbox_lines(paths):
-    names = [("Matlab", "m"), ("Python", "py"), ("R", "R")]
-    all_code = []
-    dirs = ["/Tools/", "/Tools/02450Tools/",'/Scripts/']
-    for (n,ex) in names:
-        for d in dirs:
-            tb = paths['instructor'] +"/02450Toolbox_" + n +d
-            if not os.path.exists(tb):
-                continue
-            ls = glob.glob(tb +"/*." + ex)
-            for l in ls:
-                with open(l, 'r') as f:
-                    s = f.read()
-                    code = code2lines(s)
-                    all_code += code
-    return all_code
-
-
-def code2lines(s):
-    ls = s.split("\n")
-    ls = [l.strip() for l in ls]
-    ls = [l for l in ls if len(l) > 3
-          and not l.startswith("# In[")
-          and not l.startswith("hold")]
-    return ls
-
-
-def compare(s1, s2):
-    s1 = set(s1.split("\n"))
-    s2 = set( s2.split("\n") )
-    eps = 1e-6
-    x = 2*len(s1 & s2) / (len(s1) + len(s2) + eps)
-    return x
-
-
-
-def mark(f, s1, s2):
-    ss = [("[!] " + s if s in s2 else s) for s in s1]
-    f.write("\n".join(ss))
-
-
-def get_db_DEFUNCT(paths):
-    bp = os.path.dirname(paths['collected_project_evaluations.xlsx'])
-    bp = os.path.dirname(bp)
-    db = TinyDB(bp + '/plagiarism.json')
-    return db
-
-
-def insert_projects(paths,info):
-    toolbox_code =  get_toolbox_lines(paths)
-    db = []
-    for i in range(3):
-        zip_file = paths['instructor_project_evaluations'] + "/zip%i.zip"%(i+1)
-        if not os.path.exists(zip_file):
-            continue
-        proj = {}
-
-        zf = zipfile.ZipFile(zip_file)
-        ls = zf.namelist()
-        for l in ls:
-            j = l.find('/')
-            if j <= 0: continue
-            key = l[:j]
-            val = proj.get(key, [])
-            val.append(l)
-            proj[key] = val
-
-        for k in proj:
-            s = ""
-            for f in proj[k]:
-                if f.lower().endswith(".py") or f.lower().endswith(".m") or f.lower().endswith(".r"):
-                    file = zf.read(f).decode('utf-8', errors='ignore')
-                    s = s + "\n" + file
-            group_code_ = code2lines(s)
-            group_code = [l for l in group_code_ if l not in toolbox_code]
-            print([len(s.split("\n")), len(group_code_), len(group_code)])
-            s = "\n".join(group_code)
-            v = {'semester': info['semester_id'], 'report-number': i+1, 'student_id': k, 'code': s}
-            db.append(v)
+from tinydb import TinyDB, Query
+import os
+import zipfile
+from tinydb import TinyDB, Query, where
+import glob
+import pycode_similar
+import numpy as np
+import matplotlib.pyplot as plt
+
+# Update for later: Add code to copy current .zip file content to special (archived) files. Then load these files into DB later.
+# Structure should be extended to include semester structure.
+
+def plagiarism_checker(paths,info):
+    db = insert_projects(paths,info)
+    for repn in range(1, 4):
+        d = [v for v in db if v['code'] and v['report-number'] == repn]
+        if len(d) == 0:
+            continue
+
+        M = np.zeros( shape = (len(d), len(d)) )
+        for i,d1 in enumerate(d):
+            for j, d2 in enumerate(d):
+                if i < j:
+                    x = compare(d1['code'],d2['code'])
+                    M[i,j] = x
+            print(i)
+
+        plt.imshow(M)
+        plt.colorbar()
+        plt.title("Report number %i"%repn)
+        plt.show()
+
+        aa = np.flip( np.argsort( M.ravel()),axis=0)[:10]
+        ii,jj = np.unravel_index(aa, M.shape)
+        for dx in range(len(aa)):
+            i = ii[dx]
+            j = jj[dx]
+            s1 = d[i]['code'].split("\n")
+            s2 = d[j]['code'].split("\n")
+
+            bp = os.path.dirname(paths['collected_project_evaluations.xlsx']) + "/plagiarism"
+            if not os.path.exists(bp):
+                os.mkdir(bp)
+            bp = bp + "/report_%i"%repn
+            if not os.path.exists(bp):
+                os.mkdir(bp)
+            dout = bp + "/%.2f_%i_%i"%(M[i,j], i,j)
+            if not os.path.exists(dout):
+                os.mkdir(dout)
+
+            with open(dout + "/s1.txt", 'w') as f:
+                mark(f, s1, s2)
+
+            with open(dout + "/s2.txt", 'w') as f:
+                mark(f, s2, s1)
+
+            with open(dout + "/sim.txt", 'w') as f:
+                ss = [s for s in s2 if s in s1]
+                f.write("\n".join(ss))
+
+def get_toolbox_lines(paths):
+    names = [("Matlab", "m"), ("Python", "py"), ("R", "R")]
+    all_code = []
+    dirs = ["/Tools/", "/Tools/02450Tools/",'/Scripts/']
+    for (n,ex) in names:
+        for d in dirs:
+            tb = paths['instructor'] +"/02450Toolbox_" + n +d
+            if not os.path.exists(tb):
+                continue
+            ls = glob.glob(tb +"/*." + ex)
+            for l in ls:
+                with open(l, 'r') as f:
+                    s = f.read()
+                    code = code2lines(s)
+                    all_code += code
+    return all_code
+
+
+def code2lines(s):
+    ls = s.split("\n")
+    ls = [l.strip() for l in ls]
+    ls = [l for l in ls if len(l) > 3
+          and not l.startswith("# In[")
+          and not l.startswith("hold")]
+    return ls
+
+
+def compare(s1, s2):
+    s1 = set(s1.split("\n"))
+    s2 = set( s2.split("\n") )
+    eps = 1e-6
+    x = 2*len(s1 & s2) / (len(s1) + len(s2) + eps)
+    return x
+
+
+
+def mark(f, s1, s2):
+    ss = [("[!] " + s if s in s2 else s) for s in s1]
+    f.write("\n".join(ss))
+
+
+def get_db_DEFUNCT(paths):
+    bp = os.path.dirname(paths['collected_project_evaluations.xlsx'])
+    bp = os.path.dirname(bp)
+    db = TinyDB(bp + '/plagiarism.json')
+    return db
+
+
+def insert_projects(paths,info):
+    toolbox_code =  get_toolbox_lines(paths)
+    db = []
+    for i in range(3):
+        zip_file = paths['instructor_project_evaluations'] + "/zip%i.zip"%(i+1)
+        if not os.path.exists(zip_file):
+            continue
+        proj = {}
+
+        zf = zipfile.ZipFile(zip_file)
+        ls = zf.namelist()
+        for l in ls:
+            j = l.find('/')
+            if j <= 0: continue
+            key = l[:j]
+            val = proj.get(key, [])
+            val.append(l)
+            proj[key] = val
+
+        for k in proj:
+            s = ""
+            for f in proj[k]:
+                if f.lower().endswith(".py") or f.lower().endswith(".m") or f.lower().endswith(".r"):
+                    file = zf.read(f).decode('utf-8', errors='ignore')
+                    s = s + "\n" + file
+            group_code_ = code2lines(s)
+            group_code = [l for l in group_code_ if l not in toolbox_code]
+            print([len(s.split("\n")), len(group_code_), len(group_code)])
+            s = "\n".join(group_code)
+            v = {'semester': info['semester_id'], 'report-number': i+1, 'student_id': k, 'code': s}
+            db.append(v)
     return db
```

### Comparing `coursebox-0.1.8/src/coursebox/material/homepage_lectures_exercises.py` & `coursebox-0.1.9/src/coursebox/material/homepage_lectures_exercises.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,625 +1,625 @@
-# -*- coding: utf-8 -*-
-import shutil, os, glob
-from datetime import datetime, timedelta
-import calendar
-import pickle
-import time
-from line_profiler_pycharm import profile
-from coursebox.thtools_base import partition_list
-
-import slider
-from jinjafy import jinjafy_comment
-from jinjafy import jinjafy_template
-from coursebox.core.info_paths import get_paths
-from slider.legacy_importer import slide_to_image
-from slider.legacy_importer import li_import
-from slider.slide import set_svg_background_images
-from coursebox.book.exam_includer import HOMEWORK_PROBLEMS
-from coursebox.core.info import class_information
-from coursebox.material.lecture_questions import lecture_question_compiler
-from slider import latexmk
-import coursebox
-# from line_profiler_pycharm import profile
-
-def get_feedback_groups():
-    paths = get_paths()
-    feedback_file = paths['semester'] +"/feedback_groups.pkl"
-    if os.path.exists(feedback_file):
-        with open(feedback_file,'rb') as f:
-            fbg = pickle.load(f)
-    else:
-        fbg = dict()
-
-    info = class_information()
-    all_students = [id for id in info['students']]
-
-    now = datetime.today()
-    already_used = []
-    remaining_lectures = []
-    for lecture in info['lectures']:
-        lnum = lecture['number']
-        if lnum == 1: continue
-        if lecture['date'] < now and lnum in fbg:
-            already_used += fbg[lnum]
-            # already_used += g
-        else:
-            remaining_lectures.append(lnum)
-
-    project_groups = [g['student_ids'] for g in info['all_groups']]
-    # remove already_used from these groups
-    reduced_groups = [[id for id in pg if id not in already_used] for pg in project_groups]
-    reduced_groups = [rg for rg in reduced_groups if len(rg)>0]
-    # groups are now partitioned.
-    if len(remaining_lectures) > 0:
-        fbgs = partition_list(reduced_groups, len(remaining_lectures))
-        for gg in fbgs:
-            for g in gg:
-                already_used = already_used + g
-
-
-        lst = partition_list([s for s in all_students if s not in already_used], len(remaining_lectures))
-        for i in range(len(remaining_lectures)):
-            dg = []
-            for g in fbgs[i]: dg += g  # flatten the list
-            fbg[remaining_lectures[i]] = dg + lst[i]
-
-        sum( [len(v) for k,v in fbg.items() ]) - sum( [len( set(v)) for k,v in fbg.items() ])
-
-        with open(feedback_file, 'wb') as f:
-            pickle.dump(fbg,f)
-
-    for k in fbg:
-        g = fbg[k]
-        g2 = []
-        for s in g:
-
-            if s in info['students']:
-                dl = info['students'][s]['firstname'] + " " + info['students'][s]['lastname']
-                # dl = [ss['firstname']+" "+ss['lastname'] for ss in if ss['id'] == s]
-                if not dl:
-                    print("EMPTY LIST when making feedback groups. Probably an error in project correction sheets.")
-                    continue
-                g2.append(dl)
-        fbg[k] = g2
-    return fbg
-
-PRESENTATION = 0
-NOTES = 1
-HANDOUT = 2
-def make_lectures(week=None, mode=0, gather_pdf_out=True, gather_sixup=True, make_quizzes=True, dosvg=False, Linux=False):
-    """
-    Mode determines what is compiled into the pdfs. It can be:
-
-    mode = PRESENTATION = 0: What I use to present from
-    mode = NOTES = 1: Version containing notes (used for self-study)
-    mode = HANDOUT = 2: version handed out to students.
-    """
-    paths = get_paths()
-    if os.path.exists(paths['book']):
-        book_frontpage_png = paths['shared']+"/figures/book.png" #paths['lectures']+"/static/book.png"
-        slide_to_image(paths['book'] + "/02450_Book.pdf", book_frontpage_png, page_to_take=1)
-        shutil.copy(paths['book'] + "/book_preamble.tex", paths['shared'])
-    info = class_information()
-    jinjafy_shared_templates_dir(paths, info) # Compile templates in shared/templates
-    # course_number = info['course_number']
-    if isinstance(week, int):
-        week = [week]
-    all_pdfs = []
-    for lecture in info['lectures']:
-        w = lecture['number']
-        if week is not None and w not in week:
-            continue
-
-        ag = get_feedback_groups()
-
-        lecture['feedback_groups'] = ag.get(w, [])
-        info.update({'week': w})
-        info['lecture'] = lecture
-        info['lecture']['teacher'] = [t for t in info['teachers'] if t['initials'] == lecture['teacher_initials']].pop()
-
-        lecture_texdir = paths['lectures'] + '/Lecture_%s/Latex' % w
-        lecture_texfile =lecture_texdir + "/Lecture_%i.tex" % w
-
-        fix_shared(paths, output_dir=lecture_texdir, dosvg=dosvg)
-
-        if os.path.exists(lecture_texdir):
-            print("Latex directory found for lecture %i: %s"%(w,lecture_texdir))
-            lecture_texdir_generated = lecture_texdir +"/templates"
-            if not os.path.exists(lecture_texdir_generated):
-                # shutil.rmtree(lecture_texdir_generated)
-                # time.sleep(0.2)
-                os.mkdir(lecture_texdir_generated)
-
-        if mode == PRESENTATION:
-            info['slides_shownotes'] = False
-            info['slides_handout'] = False
-            odex = "/presentation"
-        elif mode == HANDOUT:
-            info['slides_shownotes'] = False
-            info['slides_handout'] = True
-            info['slides_showsolutions'] = False
-            odex = "/handout"
-        elif mode == NOTES:
-            info['slides_shownotes'] = True
-            info['slides_handout'] = True
-            odex = "/notes"
-        else:
-            raise Exception("Mode not recognized")
-
-        for f in glob.glob(paths['lectures'] + "/templates/*.tex"):
-            ex = "_partial.tex"
-            if f.endswith(ex):
-                jinjafy_template(info, file_in=f, file_out=lecture_texdir + "/templates/"+os.path.basename(f)[:-len(ex)] + ".tex")
-
-        # Fix questions.
-        qtarg = lecture_texdir + "/questions"
-        if not os.path.exists(qtarg):
-            os.mkdir(qtarg)
-        for f in glob.glob(paths['lectures'] + "/static/questions/*"):
-            shutil.copy(f, qtarg)
-
-        # Fix questions for this lecture
-        if make_quizzes:
-            lecture_question_compiler(paths, info, lecture_texfile)
-
-        pdf_out = slider.latexmk(lecture_texfile, Linux=Linux)
-        all_pdfs.append( (w,pdf_out))
-
-    handle_pdf_collection(paths, all_pdfs, gather_pdf_out=gather_pdf_out, gather_sixup=gather_sixup, odir=odex)
-
-
-def handle_pdf_collection(paths, all_pdfs, gather_pdf_out, gather_sixup, odir):
-    tmp_dir = paths['lectures'] + '/Collected/tmp'
-    if not os.path.exists(tmp_dir):
-        os.mkdir(tmp_dir)
-
-    collect_template = paths['lectures'] + "/Collected/lecture_collector_partial.tex"
-
-    for sixup in [False, True]:
-        if not gather_pdf_out: continue
-        if sixup and not gather_sixup: continue
-
-        pdf_compiled_all_6up = []
-        sixup_str = "-6up" if sixup else ""
-        for (week, _) in all_pdfs:
-            tv = {'week': week,
-                  'pdffiles': [paths['lectures'] + '/Lecture_%s/Latex/Lecture_%s.pdf' % (week, week)]}
-            if sixup:
-                tv['sixup'] = sixup
-                tex_out_sixup = tmp_dir + "/Lecture_%i%s.tex" % (week, sixup_str)
-                jinjafy_comment(data=tv, file_in=collect_template, file_out=tex_out_sixup, jinja_tag=None)
-                dpdf = tmp_dir + "/" + slider.latexmk(tex_out_sixup, shell=False, cleanup=True)
-            else:
-                dpdf = tv['pdffiles'][0]
-
-            pdf_compiled_all_6up.append(dpdf)
-
-        for dpdf in pdf_compiled_all_6up:
-            output_dir = paths['pdf_out'] + odir
-            if not os.path.exists(output_dir):
-                os.mkdir(output_dir)
-
-            # if not info['slides_showsolutions']:
-            #     odir += "/lectures_without_solutions"
-            # if not os.path.isdir(odir):
-            #     os.mkdir(odir)
-            #
-            shutil.copy(dpdf, output_dir + "/" + os.path.basename(dpdf))
-
-    for f in glob.glob(tmp_dir + "/*"):
-        os.remove(f)
-
-def compile_simple_files(paths, info, template_file_list, verbose=False):
-    jinjafy_shared_templates_dir(paths, info)
-    fix_shared(paths, output_dir=paths['shared_latex_compilation_dir'], verbose=verbose)
-    for fname,dd in template_file_list:
-        d2 = info.copy()
-        d2.update(dd)
-        file = os.path.basename(fname)
-        if file.endswith("_template.tex"):
-            file = file.replace("_template.tex", ".tex")
-        tex_out = paths['shared_latex_compilation_dir'] + "/" + file
-        jinjafy_template(data=d2, file_in=fname, file_out=tex_out, filters=get_filters(), template_searchpath=paths['instructor'])
-        latexmk(tex_out, pdf_out= paths['pdf_out'] + "/" + os.path.basename(tex_out)[:-4]+".pdf")
-
-# rec_fix_shared(shared_base=paths['shared'], output_dir=output_dir)
-import time
-# import dirsync
-# dirsync.sync(paths['shared'], output_dir, 'diff')
-
-
-# Do smarter fixin'
-from pathlib import Path
-
-from jinjafy.cache.simplecache import hash_file_
-
-@profile
-def get_hash_from_base(base):
-    if not os.path.exists(base + "/sharedcache.pkl"):
-        source = {}
-    else:
-        with open(base + "/sharedcache.pkl", 'rb') as f:
-            source = pickle.load(f)
-
-    actual_files = {}
-    for f in glob.glob(base + "/**", recursive=True):
-        if os.path.isdir(f):
-            continue
-        if f.endswith("sharedcache.pkl"):
-            continue
-        rel = os.path.relpath(f, base)
-
-        # d = dict(mtime=os.path.getmtime(f))
-        actual_files[rel] = dict(mtime=os.path.getmtime(f), hash=-1, modified=False)
-
-        if rel not in source or (actual_files[rel]['mtime'] != source[rel].get('mtime', -1)): # It has been modified, update hash
-            # print(rel, time.ctime(actual_files[rel]['mtime']), time.ctime(source[rel].get('mtime', -1)))
-            new_hash = hash_file_(f)
-            # actual_files[rel] = {}
-            actual_files[rel]['modified'] = new_hash != source.get(rel, {}).get('hash', -1)
-            actual_files[rel]['hash'] = new_hash
-        else:
-            actual_files[rel]['hash'] = source[rel]['hash']
-    return actual_files
-
-
-@profile
-def fix_shared(paths, output_dir, pdf2png=False,dosvg=True,verbose=False, compile_templates=True,shallow=True):
-    '''
-    Copy shared files into lecture directories
-    '''
-    cache_base = output_dir
-    from jinjafy.cache import cache_contains_file, cache_update_file
-    from slider.convert import svg2pdf, pdfcrop
-    from slider import convert
-    import filecmp
-
-    t0 = time.time()
-    shared_base = paths['shared']
-    output_dir = output_dir
-
-    import glob
-    # def get_cache_from_dir(shared_base):
-    # print("Beginning file cache..")
-
-
-    source = get_hash_from_base(shared_base)
-    target = get_hash_from_base(output_dir)
-
-    # update_source_cache = False
-    source_extra = {}
-    for rel in source:
-        if rel.endswith(".svg") and source[rel]['modified']:
-            pdf_file = svg2pdf(shared_base + "/"+rel, crop=True, text_to_path=True, verbose=True)
-            rel = os.path.relpath(pdf_file, shared_base)
-            source_extra[rel] = dict(mtime=os.path.getmtime(pdf_file), hash=hash_file_(pdf_file), modified=True)
-
-    for k, v in source_extra.items():
-        source[k] = v
-
-
-            # update_source_cache = True
-    # Perform sync here.
-    for rel in source:
-        if rel.endswith("_partial.tex"):
-            continue
-
-        if rel not in target or target[rel]['hash'] != source[rel]['hash']:
-            print(" -> ", output_dir + "/" + rel)
-            shutil.copy(shared_base +"/" + rel, output_dir + "/" + rel)
-            target[rel] = source[rel].copy()
-            target[rel]['modified'] = True
-            target[rel]['mtime'] = os.path.getmtime(output_dir + "/" + rel)
-
-    if pdf2png:
-        for rel in target:
-            if rel.endswith(".pdf") and target[rel]['modified']:
-                # print("pdf2png: ")
-                png = convert.pdf2png(output_dir + "/" + rel, verbose=True)
-                target[rel]['modified'] = False
-                target[rel]['hash'] = hash_file_(output_dir + "/" + rel)
-                target[rel]['mtime'] = os.path.getmtime(output_dir + "/" + rel)
-
-    # Save the cache.
-
-    with open(shared_base + "/sharedcache.pkl", 'wb') as f:
-        pickle.dump(source, f)
-
-    with open(output_dir + "/sharedcache.pkl", 'wb') as f:
-        pickle.dump(target, f)
-
-    print("fix_shared()", time.time() - t0)
-
-    #
-    # if pdf2png:
-    #     if f.endswith(".pdf") and pdf2png:
-    #         if verbose:
-    #             print("converting to png", f)
-    #         convert.pdf2png(of)
-    #
-    #     for f in source:
-    #         if f not in target:
-    #             print(f)
-    #         else:
-    #             if source[f]['hash'] != target[f]['hash']:
-    #                 print(f, f)
-    #
-    #
-    #
-    # a = 234
-    # # if rel not in source:
-    #
-    #     #     source[rel] = dict(mtime=os.path.getmtime(f), hash=hash_file_(f))
-    #     #
-    #
-    #
-    # # Everything has a hash/mtime that is up to date. Now look at target dir
-    #
-    # get_cache_from_dir(output_dir)
-    #
-    # # Get the corresponding output at destination:
-    #
-    #
-    #
-    #
-    #
-    #
-    # for path in Path(shared_base).rglob('*'):
-    #     print(path)
-    # a = 234
-    # def rec_fix_shared(shared_base, output_dir):
-    #     if dosvg:
-    #         for svg in glob.glob(shared_base+"/*.svg"):
-    #             # if not os.path.exists(shared_base + )
-    #             if not cache_contains_file(cache_base, svg):
-    #                 # if verbose:
-    #                 print("converting to pdf", svg)
-    #                 svg2pdf(svg,crop=True, text_to_path=True)
-    #                 cache_update_file(cache_base, svg)
-    #                 assert False
-    #
-    #     files = glob.glob(shared_base+"/*")
-    #     for f in files:
-    #         if f.endswith("cache.pkl"):
-    #             continue
-    #
-    #         if "templates" in f and f.endswith("_partial.tex"):
-    #             continue
-    #
-    #         if os.path.isdir(f):
-    #             od2 = output_dir + "/" + os.path.basename(f)
-    #             if not os.path.exists(od2):
-    #                 os.mkdir(od2)
-    #             rec_fix_shared(f, od2)
-    #         else:
-    #             of = output_dir + "/" + os.path.basename(f)
-    #             if not os.path.exists(of) or not filecmp.cmp(f, of,shallow=shallow):
-    #                 print(f"> fix_shared() -> {of}")
-    #                 shutil.copy(f, of)
-    #                 if f.endswith(".pdf") and pdf2png:
-    #                     if verbose:
-    #                         print("converting to png", f)
-    #                     convert.pdf2png(of)
-    #                 # cache_update_file(cache_base, f)
-    #
-    #         if verbose:
-    #             print(" done!")
-
-    # if pdf2png:
-    #     assert False
-
-
-
-    # get diff.
-
-    # directory_cmp = filecmp.dircmp(a=paths['shared'], b=output_dir)
-    # from filecmp import dircmp
-    # from filecmp import dircmp
-    # def print_diff_files(dcmp):
-    #     for name in dcmp.diff_files:
-    #         print("diff_file %s found in %s and %s" % (name, dcmp.left, dcmp.right))
-    #         print("")
-    #     for sub_dcmp in dcmp.subdirs.values():
-    #         print_diff_files(sub_dcmp)
-    #
-
-    # t0 = time.time()
-    # dcmp = dircmp(paths['shared'], output_dir)
-    # print_diff_files(dcmp)
-    # print("dircmp", time.time() - t0)
-    # directory_cmp.report()
-    # import time
-    # t0 = time.time()
-    # rec_fix_shared(shared_base=paths['shared'], output_dir=output_dir)
-    # import time
-    # # import dirsync
-    # # dirsync.sync(paths['shared'], output_dir, 'diff')
-    # print("mine", time.time() - t0)
-    a = 234
-
-
-def jinjafy_shared_templates_dir(paths, info):
-    tpd = paths['shared'] + "/templates"
-    for f in glob.glob(tpd + "/*.tex"):
-        print(f)
-        ex = "_partial.tex"
-        if f.endswith(ex):
-            jinjafy_template(info, file_in=f, file_out=f"{tpd}/{os.path.basename(f)[:-len(ex)]}.tex")
-
-
-def get_filters():
-    return {'safetex': safetex, 'tt': tt, 'bf': bf, 'verb': verb}
-
-def make_exercises_projects_tutors(week=None, only_exercises=False, make_exercises=True, make_projects=True, dosvg=False):
-    paths = get_paths()
-    filters = get_filters()
-    info = class_information()
-    course_number = info['course_number']
-    jinjafy_shared_templates_dir(paths, info) # Compile files in the shared/templates  directory.
-
-    if not only_exercises:  # Don't do any of this if we are in continuing education mode
-        for proj in range(len(info['reports_handin']) if not info['CE'] else 1):
-            info['project'] = proj+1
-            info['is_project'] = True
-            handout_week = info['reports_handout'][proj]
-            handin_week =info['reports_handin'][proj]
-
-            info['lecture'] = info['lectures'][ handout_week-1]
-            info['lecture_handin'] = info['lectures'][handin_week-1]
-
-            if info['CE']:
-                proj_base = paths['instructor'] + "/ExercisesShared/%sprojectCE_Base.tex"%(course_number, )
-                proj_tex_out = paths['instructor'] + "/Project/latex%i/%sprojectCE.tex" % (1,course_number,)
-            else:
-                proj_base = paths['instructor'] + "/ExercisesShared/%sproject%i_Base.tex" % (course_number,proj+1,)
-                proj_tex_out = paths['instructor'] + "/Project/latex%i/%sproject%i.tex" % (proj+1, course_number, proj+1)
-            info['week'] = -1
-
-            if not os.path.exists(proj_base):
-                continue
-
-            jinjafy_template(info, proj_base, file_out=proj_tex_out, filters=filters, template_searchpath=paths['instructor'])
-            fix_shared(paths, output_dir=os.path.dirname(proj_tex_out), dosvg=dosvg)
-            latexmk(proj_tex_out, pdf_out=paths['pdf_out'] + "/" + os.path.basename(proj_tex_out)[:-4] + ".pdf")
-
-    langs = ["Matlab", "Python", "R"]
-    info['is_project'] = False
-    for lang in langs:
-        if not make_exercises:
-            break
-        # Handle exercise 0 seperately:
-
-        ex0_date = info['lectures'][0]['date'] - timedelta(days=0 if info['CE'] else 7)
-        ex0 = { 'number': 0,
-                'date': ex0_date,
-                'year': ex0_date.year,
-                'month': calendar.month_name[ex0_date.month],
-                'day': ex0_date.day}
-        all_lectures = [ex0] + info['lectures'][:-1]
-
-        exercises_to_compile = all_lectures[week:week+1] if week != None else all_lectures
-
-        for lecture in exercises_to_compile: # not number 13.
-            w = lecture['number']
-            info['lecture'] = lecture
-            info['week'] = w
-
-            nicelang = lang.upper()
-            tb = '''<base-dir>/02450Toolbox_%s/''' % lang
-            if lang == "Matlab":
-                ext = "m"
-            elif lang == "Python":
-                ext = "py"
-            else:
-                ext = "R"
-
-            tv = {
-                  "lang": lang,
-                  "nicelang": nicelang,
-                  "tbscripts": tb + "Scripts/",
-                  "tbdata": tb + "Data/",
-                  "tbtools": tb + "Tools/",
-                  "tbname": '''02450Toolbox\_%s''' % lang,
-                  "tb": tb,
-                  "ext": ext,
-                  "tbsetup": tb + "setup.%s" % ext,
-                  "Python": lang == "Python",
-                  "Matlab": lang == "Matlab",
-                  "R": lang == "R",
-                  'HOMEWORK_PROBLEMS': HOMEWORK_PROBLEMS,
-                  }
-
-            # get lang dir
-            if not os.path.exists("%s/Exercises%s"%(paths['instructor'], lang)):
-                continue
-
-            info.update(tv)
-            ex_base =  "%s/ExercisesShared/%sex%i_Base.tex"%(paths['instructor'], course_number, w)
-            ex_tex_out = "%s/Exercises%s/Exercise%i/latex/%sex%i_%s.tex" % ( paths['instructor'], lang, w, course_number, w, lang)
-            # fbody = os.path.dirname(ex_tex_out) +f"/ex{w}_body.tex"
-
-            if os.path.exists(ex_base):
-                jinjafy_template(info, ex_base, file_out=ex_tex_out, filters=filters, template_searchpath=paths['instructor'])
-                fix_shared(paths, output_dir=os.path.dirname(ex_tex_out), dosvg=dosvg)
-                # mvfiles(shared_tex, os.path.dirname(ex_tex_out)+"/")
-                latexmk(ex_tex_out, pdf_out=paths['pdf_out']+"/" + os.path.basename(ex_tex_out)[:-4] + ".pdf")
-
-def mvfiles(source_dir, dest_dir):
-    src_files = os.listdir(source_dir)
-    for file_name in src_files:
-        full_file_name = os.path.join(source_dir, file_name)
-        if (os.path.isfile(full_file_name)):
-            shutil.copy(full_file_name, os.path.dirname(dest_dir))
-
-@profile
-def make_webpage(dosvg=True):
-    cinfo = class_information()
-    paths = get_paths()
-    fix_shared(paths, output_dir=os.path.dirname(paths['homepage_out']), pdf2png=True, dosvg=dosvg)
-    wdir = paths['homepage_template']
-    jinjafy_template(cinfo, file_in=wdir, file_out=paths['homepage_out'])
-    print("Instructors for course: ")
-    s = ""
-    for dex,i in enumerate(cinfo['instructors']):
-        if dex > 0:
-            s += "; "
-        s += i['email']
-
-    blrb = os.path.dirname(paths['homepage_template']) +"/homepage_widget_blurb_template.html"
-    if os.path.exists( blrb):
-        jinjafy_template(cinfo, file_in=blrb, file_out=blrb.replace("_template.html", ".html"))
-    print(s)
-
-
-# This should probably  be moved into jinjafy
-def tt(value):
-    return "\\texttt{" + value + "}"
-
-def bf(value):
-    return "\\textbf{" + value + "}"
-
-def verb(value):
-    return '\\verb"' + value + '"'
-
-def safetex(value):
-    return value.replace("_", "\_")
-
-def slide_converter(week=None, verbose=True, clean_temporary_files=False, copy_template_resource_files=True, fix_broken_osvg_files=False, **kwargs):
-    """ Legacy function. """
-    print("Checking if slides should be converted from odf -> pdf format..")
-    paths = get_paths()
-    info = class_information()
-    # week = [week] if week not isinstance(week, list) else []
-    week = week if week is None else [week] #[week] if not week is None else
-
-    for lecture in info['lectures']:
-        # for n in range(1,14):
-        n = lecture['number']
-        if week is not None and n not in week:
-            continue
-        ldir = "%s/Lecture_%i"%(paths['lectures'], n)
-        texdir = ldir +"/Latex"
-        print("Testing conversion between directories:\n   > %s -> %s"%(ldir, texdir))
-
-        if not os.path.exists(texdir):
-            os.mkdir(texdir)
-            pdf_in = "%s/Lecture_%i.pdf"%(ldir, n)
-            pdf_out = texdir +"/Lecture_%i.pdf"%n
-            shutil.copyfile(pdf_in, pdf_out)
-
-            print("operating...")
-            lecture_tex_out = li_import(pdf_out, output_dir=texdir)
-            print("Wrote new main file: " + lecture_tex_out)
-        else:
-            print("%s exists; no conversion possible. "% (texdir,))
-
-        print("Handling .svg conversion in slides..")
-        slide_tex_path = texdir +"/Lecture_%i.tex"%n
-        print("   > "+slide_tex_path)
-        set_svg_background_images(slide_tex_path,
-                                  verbose=verbose,
-                                  clean_temporary_files=clean_temporary_files,
-                                  copy_template_resource_files=copy_template_resource_files,
-                                  fix_broken_osvg_files=fix_broken_osvg_files, **kwargs)
-
-    print("Slides converted!")
+# -*- coding: utf-8 -*-
+import shutil, os, glob
+from datetime import datetime, timedelta
+import calendar
+import pickle
+import time
+from line_profiler_pycharm import profile
+from coursebox.thtools_base import partition_list
+
+import slider
+from jinjafy import jinjafy_comment
+from jinjafy import jinjafy_template
+from coursebox.core.info_paths import get_paths
+from slider.legacy_importer import slide_to_image
+from slider.legacy_importer import li_import
+from slider.slide import set_svg_background_images
+from coursebox.book.exam_includer import HOMEWORK_PROBLEMS
+from coursebox.core.info import class_information
+from coursebox.material.lecture_questions import lecture_question_compiler
+from slider import latexmk
+import coursebox
+# from line_profiler_pycharm import profile
+
+def get_feedback_groups():
+    paths = get_paths()
+    feedback_file = paths['semester'] +"/feedback_groups.pkl"
+    if os.path.exists(feedback_file):
+        with open(feedback_file,'rb') as f:
+            fbg = pickle.load(f)
+    else:
+        fbg = dict()
+
+    info = class_information()
+    all_students = [id for id in info['students']]
+
+    now = datetime.today()
+    already_used = []
+    remaining_lectures = []
+    for lecture in info['lectures']:
+        lnum = lecture['number']
+        if lnum == 1: continue
+        if lecture['date'] < now and lnum in fbg:
+            already_used += fbg[lnum]
+            # already_used += g
+        else:
+            remaining_lectures.append(lnum)
+
+    project_groups = [g['student_ids'] for g in info['all_groups']]
+    # remove already_used from these groups
+    reduced_groups = [[id for id in pg if id not in already_used] for pg in project_groups]
+    reduced_groups = [rg for rg in reduced_groups if len(rg)>0]
+    # groups are now partitioned.
+    if len(remaining_lectures) > 0:
+        fbgs = partition_list(reduced_groups, len(remaining_lectures))
+        for gg in fbgs:
+            for g in gg:
+                already_used = already_used + g
+
+
+        lst = partition_list([s for s in all_students if s not in already_used], len(remaining_lectures))
+        for i in range(len(remaining_lectures)):
+            dg = []
+            for g in fbgs[i]: dg += g  # flatten the list
+            fbg[remaining_lectures[i]] = dg + lst[i]
+
+        sum( [len(v) for k,v in fbg.items() ]) - sum( [len( set(v)) for k,v in fbg.items() ])
+
+        with open(feedback_file, 'wb') as f:
+            pickle.dump(fbg,f)
+
+    for k in fbg:
+        g = fbg[k]
+        g2 = []
+        for s in g:
+
+            if s in info['students']:
+                dl = info['students'][s]['firstname'] + " " + info['students'][s]['lastname']
+                # dl = [ss['firstname']+" "+ss['lastname'] for ss in if ss['id'] == s]
+                if not dl:
+                    print("EMPTY LIST when making feedback groups. Probably an error in project correction sheets.")
+                    continue
+                g2.append(dl)
+        fbg[k] = g2
+    return fbg
+
+PRESENTATION = 0
+NOTES = 1
+HANDOUT = 2
+def make_lectures(week=None, mode=0, gather_pdf_out=True, gather_sixup=True, make_quizzes=True, dosvg=False, Linux=False):
+    """
+    Mode determines what is compiled into the pdfs. It can be:
+
+    mode = PRESENTATION = 0: What I use to present from
+    mode = NOTES = 1: Version containing notes (used for self-study)
+    mode = HANDOUT = 2: version handed out to students.
+    """
+    paths = get_paths()
+    if os.path.exists(paths['book']):
+        book_frontpage_png = paths['shared']+"/figures/book.png" #paths['lectures']+"/static/book.png"
+        slide_to_image(paths['book'] + "/02450_Book.pdf", book_frontpage_png, page_to_take=1)
+        shutil.copy(paths['book'] + "/book_preamble.tex", paths['shared'])
+    info = class_information()
+    jinjafy_shared_templates_dir(paths, info) # Compile templates in shared/templates
+    # course_number = info['course_number']
+    if isinstance(week, int):
+        week = [week]
+    all_pdfs = []
+    for lecture in info['lectures']:
+        w = lecture['number']
+        if week is not None and w not in week:
+            continue
+
+        ag = get_feedback_groups()
+
+        lecture['feedback_groups'] = ag.get(w, [])
+        info.update({'week': w})
+        info['lecture'] = lecture
+        info['lecture']['teacher'] = [t for t in info['teachers'] if t['initials'] == lecture['teacher_initials']].pop()
+
+        lecture_texdir = paths['lectures'] + '/Lecture_%s/Latex' % w
+        lecture_texfile =lecture_texdir + "/Lecture_%i.tex" % w
+
+        fix_shared(paths, output_dir=lecture_texdir, dosvg=dosvg)
+
+        if os.path.exists(lecture_texdir):
+            print("Latex directory found for lecture %i: %s"%(w,lecture_texdir))
+            lecture_texdir_generated = lecture_texdir +"/templates"
+            if not os.path.exists(lecture_texdir_generated):
+                # shutil.rmtree(lecture_texdir_generated)
+                # time.sleep(0.2)
+                os.mkdir(lecture_texdir_generated)
+
+        if mode == PRESENTATION:
+            info['slides_shownotes'] = False
+            info['slides_handout'] = False
+            odex = "/presentation"
+        elif mode == HANDOUT:
+            info['slides_shownotes'] = False
+            info['slides_handout'] = True
+            info['slides_showsolutions'] = False
+            odex = "/handout"
+        elif mode == NOTES:
+            info['slides_shownotes'] = True
+            info['slides_handout'] = True
+            odex = "/notes"
+        else:
+            raise Exception("Mode not recognized")
+
+        for f in glob.glob(paths['lectures'] + "/templates/*.tex"):
+            ex = "_partial.tex"
+            if f.endswith(ex):
+                jinjafy_template(info, file_in=f, file_out=lecture_texdir + "/templates/"+os.path.basename(f)[:-len(ex)] + ".tex")
+
+        # Fix questions.
+        qtarg = lecture_texdir + "/questions"
+        if not os.path.exists(qtarg):
+            os.mkdir(qtarg)
+        for f in glob.glob(paths['lectures'] + "/static/questions/*"):
+            shutil.copy(f, qtarg)
+
+        # Fix questions for this lecture
+        if make_quizzes:
+            lecture_question_compiler(paths, info, lecture_texfile)
+
+        pdf_out = slider.latexmk(lecture_texfile, Linux=Linux)
+        all_pdfs.append( (w,pdf_out))
+
+    handle_pdf_collection(paths, all_pdfs, gather_pdf_out=gather_pdf_out, gather_sixup=gather_sixup, odir=odex)
+
+
+def handle_pdf_collection(paths, all_pdfs, gather_pdf_out, gather_sixup, odir):
+    tmp_dir = paths['lectures'] + '/Collected/tmp'
+    if not os.path.exists(tmp_dir):
+        os.mkdir(tmp_dir)
+
+    collect_template = paths['lectures'] + "/Collected/lecture_collector_partial.tex"
+
+    for sixup in [False, True]:
+        if not gather_pdf_out: continue
+        if sixup and not gather_sixup: continue
+
+        pdf_compiled_all_6up = []
+        sixup_str = "-6up" if sixup else ""
+        for (week, _) in all_pdfs:
+            tv = {'week': week,
+                  'pdffiles': [paths['lectures'] + '/Lecture_%s/Latex/Lecture_%s.pdf' % (week, week)]}
+            if sixup:
+                tv['sixup'] = sixup
+                tex_out_sixup = tmp_dir + "/Lecture_%i%s.tex" % (week, sixup_str)
+                jinjafy_comment(data=tv, file_in=collect_template, file_out=tex_out_sixup, jinja_tag=None)
+                dpdf = tmp_dir + "/" + slider.latexmk(tex_out_sixup, shell=False, cleanup=True)
+            else:
+                dpdf = tv['pdffiles'][0]
+
+            pdf_compiled_all_6up.append(dpdf)
+
+        for dpdf in pdf_compiled_all_6up:
+            output_dir = paths['pdf_out'] + odir
+            if not os.path.exists(output_dir):
+                os.mkdir(output_dir)
+
+            # if not info['slides_showsolutions']:
+            #     odir += "/lectures_without_solutions"
+            # if not os.path.isdir(odir):
+            #     os.mkdir(odir)
+            #
+            shutil.copy(dpdf, output_dir + "/" + os.path.basename(dpdf))
+
+    for f in glob.glob(tmp_dir + "/*"):
+        os.remove(f)
+
+def compile_simple_files(paths, info, template_file_list, verbose=False):
+    jinjafy_shared_templates_dir(paths, info)
+    fix_shared(paths, output_dir=paths['shared_latex_compilation_dir'], verbose=verbose)
+    for fname,dd in template_file_list:
+        d2 = info.copy()
+        d2.update(dd)
+        file = os.path.basename(fname)
+        if file.endswith("_template.tex"):
+            file = file.replace("_template.tex", ".tex")
+        tex_out = paths['shared_latex_compilation_dir'] + "/" + file
+        jinjafy_template(data=d2, file_in=fname, file_out=tex_out, filters=get_filters(), template_searchpath=paths['instructor'])
+        latexmk(tex_out, pdf_out= paths['pdf_out'] + "/" + os.path.basename(tex_out)[:-4]+".pdf")
+
+# rec_fix_shared(shared_base=paths['shared'], output_dir=output_dir)
+import time
+# import dirsync
+# dirsync.sync(paths['shared'], output_dir, 'diff')
+
+
+# Do smarter fixin'
+from pathlib import Path
+
+from jinjafy.cache.simplecache import hash_file_
+
+@profile
+def get_hash_from_base(base):
+    if not os.path.exists(base + "/sharedcache.pkl"):
+        source = {}
+    else:
+        with open(base + "/sharedcache.pkl", 'rb') as f:
+            source = pickle.load(f)
+
+    actual_files = {}
+    for f in glob.glob(base + "/**", recursive=True):
+        if os.path.isdir(f):
+            continue
+        if f.endswith("sharedcache.pkl"):
+            continue
+        rel = os.path.relpath(f, base)
+
+        # d = dict(mtime=os.path.getmtime(f))
+        actual_files[rel] = dict(mtime=os.path.getmtime(f), hash=-1, modified=False)
+
+        if rel not in source or (actual_files[rel]['mtime'] != source[rel].get('mtime', -1)): # It has been modified, update hash
+            # print(rel, time.ctime(actual_files[rel]['mtime']), time.ctime(source[rel].get('mtime', -1)))
+            new_hash = hash_file_(f)
+            # actual_files[rel] = {}
+            actual_files[rel]['modified'] = new_hash != source.get(rel, {}).get('hash', -1)
+            actual_files[rel]['hash'] = new_hash
+        else:
+            actual_files[rel]['hash'] = source[rel]['hash']
+    return actual_files
+
+
+@profile
+def fix_shared(paths, output_dir, pdf2png=False,dosvg=True,verbose=False, compile_templates=True,shallow=True):
+    '''
+    Copy shared files into lecture directories
+    '''
+    cache_base = output_dir
+    from jinjafy.cache import cache_contains_file, cache_update_file
+    from slider.convert import svg2pdf, pdfcrop
+    from slider import convert
+    import filecmp
+
+    t0 = time.time()
+    shared_base = paths['shared']
+    output_dir = output_dir
+
+    import glob
+    # def get_cache_from_dir(shared_base):
+    # print("Beginning file cache..")
+
+
+    source = get_hash_from_base(shared_base)
+    target = get_hash_from_base(output_dir)
+
+    # update_source_cache = False
+    source_extra = {}
+    for rel in source:
+        if rel.endswith(".svg") and source[rel]['modified']:
+            pdf_file = svg2pdf(shared_base + "/"+rel, crop=True, text_to_path=True, verbose=True)
+            rel = os.path.relpath(pdf_file, shared_base)
+            source_extra[rel] = dict(mtime=os.path.getmtime(pdf_file), hash=hash_file_(pdf_file), modified=True)
+
+    for k, v in source_extra.items():
+        source[k] = v
+
+
+            # update_source_cache = True
+    # Perform sync here.
+    for rel in source:
+        if rel.endswith("_partial.tex"):
+            continue
+
+        if rel not in target or target[rel]['hash'] != source[rel]['hash']:
+            print(" -> ", output_dir + "/" + rel)
+            shutil.copy(shared_base +"/" + rel, output_dir + "/" + rel)
+            target[rel] = source[rel].copy()
+            target[rel]['modified'] = True
+            target[rel]['mtime'] = os.path.getmtime(output_dir + "/" + rel)
+
+    if pdf2png:
+        for rel in target:
+            if rel.endswith(".pdf") and target[rel]['modified']:
+                # print("pdf2png: ")
+                png = convert.pdf2png(output_dir + "/" + rel, verbose=True)
+                target[rel]['modified'] = False
+                target[rel]['hash'] = hash_file_(output_dir + "/" + rel)
+                target[rel]['mtime'] = os.path.getmtime(output_dir + "/" + rel)
+
+    # Save the cache.
+
+    with open(shared_base + "/sharedcache.pkl", 'wb') as f:
+        pickle.dump(source, f)
+
+    with open(output_dir + "/sharedcache.pkl", 'wb') as f:
+        pickle.dump(target, f)
+
+    print("fix_shared()", time.time() - t0)
+
+    #
+    # if pdf2png:
+    #     if f.endswith(".pdf") and pdf2png:
+    #         if verbose:
+    #             print("converting to png", f)
+    #         convert.pdf2png(of)
+    #
+    #     for f in source:
+    #         if f not in target:
+    #             print(f)
+    #         else:
+    #             if source[f]['hash'] != target[f]['hash']:
+    #                 print(f, f)
+    #
+    #
+    #
+    # a = 234
+    # # if rel not in source:
+    #
+    #     #     source[rel] = dict(mtime=os.path.getmtime(f), hash=hash_file_(f))
+    #     #
+    #
+    #
+    # # Everything has a hash/mtime that is up to date. Now look at target dir
+    #
+    # get_cache_from_dir(output_dir)
+    #
+    # # Get the corresponding output at destination:
+    #
+    #
+    #
+    #
+    #
+    #
+    # for path in Path(shared_base).rglob('*'):
+    #     print(path)
+    # a = 234
+    # def rec_fix_shared(shared_base, output_dir):
+    #     if dosvg:
+    #         for svg in glob.glob(shared_base+"/*.svg"):
+    #             # if not os.path.exists(shared_base + )
+    #             if not cache_contains_file(cache_base, svg):
+    #                 # if verbose:
+    #                 print("converting to pdf", svg)
+    #                 svg2pdf(svg,crop=True, text_to_path=True)
+    #                 cache_update_file(cache_base, svg)
+    #                 assert False
+    #
+    #     files = glob.glob(shared_base+"/*")
+    #     for f in files:
+    #         if f.endswith("cache.pkl"):
+    #             continue
+    #
+    #         if "templates" in f and f.endswith("_partial.tex"):
+    #             continue
+    #
+    #         if os.path.isdir(f):
+    #             od2 = output_dir + "/" + os.path.basename(f)
+    #             if not os.path.exists(od2):
+    #                 os.mkdir(od2)
+    #             rec_fix_shared(f, od2)
+    #         else:
+    #             of = output_dir + "/" + os.path.basename(f)
+    #             if not os.path.exists(of) or not filecmp.cmp(f, of,shallow=shallow):
+    #                 print(f"> fix_shared() -> {of}")
+    #                 shutil.copy(f, of)
+    #                 if f.endswith(".pdf") and pdf2png:
+    #                     if verbose:
+    #                         print("converting to png", f)
+    #                     convert.pdf2png(of)
+    #                 # cache_update_file(cache_base, f)
+    #
+    #         if verbose:
+    #             print(" done!")
+
+    # if pdf2png:
+    #     assert False
+
+
+
+    # get diff.
+
+    # directory_cmp = filecmp.dircmp(a=paths['shared'], b=output_dir)
+    # from filecmp import dircmp
+    # from filecmp import dircmp
+    # def print_diff_files(dcmp):
+    #     for name in dcmp.diff_files:
+    #         print("diff_file %s found in %s and %s" % (name, dcmp.left, dcmp.right))
+    #         print("")
+    #     for sub_dcmp in dcmp.subdirs.values():
+    #         print_diff_files(sub_dcmp)
+    #
+
+    # t0 = time.time()
+    # dcmp = dircmp(paths['shared'], output_dir)
+    # print_diff_files(dcmp)
+    # print("dircmp", time.time() - t0)
+    # directory_cmp.report()
+    # import time
+    # t0 = time.time()
+    # rec_fix_shared(shared_base=paths['shared'], output_dir=output_dir)
+    # import time
+    # # import dirsync
+    # # dirsync.sync(paths['shared'], output_dir, 'diff')
+    # print("mine", time.time() - t0)
+    a = 234
+
+
+def jinjafy_shared_templates_dir(paths, info):
+    tpd = paths['shared'] + "/templates"
+    for f in glob.glob(tpd + "/*.tex"):
+        print(f)
+        ex = "_partial.tex"
+        if f.endswith(ex):
+            jinjafy_template(info, file_in=f, file_out=f"{tpd}/{os.path.basename(f)[:-len(ex)]}.tex")
+
+
+def get_filters():
+    return {'safetex': safetex, 'tt': tt, 'bf': bf, 'verb': verb}
+
+def make_exercises_projects_tutors(week=None, only_exercises=False, make_exercises=True, make_projects=True, dosvg=False):
+    paths = get_paths()
+    filters = get_filters()
+    info = class_information()
+    course_number = info['course_number']
+    jinjafy_shared_templates_dir(paths, info) # Compile files in the shared/templates  directory.
+
+    if not only_exercises:  # Don't do any of this if we are in continuing education mode
+        for proj in range(len(info['reports_handin']) if not info['CE'] else 1):
+            info['project'] = proj+1
+            info['is_project'] = True
+            handout_week = info['reports_handout'][proj]
+            handin_week =info['reports_handin'][proj]
+
+            info['lecture'] = info['lectures'][ handout_week-1]
+            info['lecture_handin'] = info['lectures'][handin_week-1]
+
+            if info['CE']:
+                proj_base = paths['instructor'] + "/ExercisesShared/%sprojectCE_Base.tex"%(course_number, )
+                proj_tex_out = paths['instructor'] + "/Project/latex%i/%sprojectCE.tex" % (1,course_number,)
+            else:
+                proj_base = paths['instructor'] + "/ExercisesShared/%sproject%i_Base.tex" % (course_number,proj+1,)
+                proj_tex_out = paths['instructor'] + "/Project/latex%i/%sproject%i.tex" % (proj+1, course_number, proj+1)
+            info['week'] = -1
+
+            if not os.path.exists(proj_base):
+                continue
+
+            jinjafy_template(info, proj_base, file_out=proj_tex_out, filters=filters, template_searchpath=paths['instructor'])
+            fix_shared(paths, output_dir=os.path.dirname(proj_tex_out), dosvg=dosvg)
+            latexmk(proj_tex_out, pdf_out=paths['pdf_out'] + "/" + os.path.basename(proj_tex_out)[:-4] + ".pdf")
+
+    langs = ["Matlab", "Python", "R"]
+    info['is_project'] = False
+    for lang in langs:
+        if not make_exercises:
+            break
+        # Handle exercise 0 seperately:
+
+        ex0_date = info['lectures'][0]['date'] - timedelta(days=0 if info['CE'] else 7)
+        ex0 = { 'number': 0,
+                'date': ex0_date,
+                'year': ex0_date.year,
+                'month': calendar.month_name[ex0_date.month],
+                'day': ex0_date.day}
+        all_lectures = [ex0] + info['lectures'][:-1]
+
+        exercises_to_compile = all_lectures[week:week+1] if week != None else all_lectures
+
+        for lecture in exercises_to_compile: # not number 13.
+            w = lecture['number']
+            info['lecture'] = lecture
+            info['week'] = w
+
+            nicelang = lang.upper()
+            tb = '''<base-dir>/02450Toolbox_%s/''' % lang
+            if lang == "Matlab":
+                ext = "m"
+            elif lang == "Python":
+                ext = "py"
+            else:
+                ext = "R"
+
+            tv = {
+                  "lang": lang,
+                  "nicelang": nicelang,
+                  "tbscripts": tb + "Scripts/",
+                  "tbdata": tb + "Data/",
+                  "tbtools": tb + "Tools/",
+                  "tbname": '''02450Toolbox\_%s''' % lang,
+                  "tb": tb,
+                  "ext": ext,
+                  "tbsetup": tb + "setup.%s" % ext,
+                  "Python": lang == "Python",
+                  "Matlab": lang == "Matlab",
+                  "R": lang == "R",
+                  'HOMEWORK_PROBLEMS': HOMEWORK_PROBLEMS,
+                  }
+
+            # get lang dir
+            if not os.path.exists("%s/Exercises%s"%(paths['instructor'], lang)):
+                continue
+
+            info.update(tv)
+            ex_base =  "%s/ExercisesShared/%sex%i_Base.tex"%(paths['instructor'], course_number, w)
+            ex_tex_out = "%s/Exercises%s/Exercise%i/latex/%sex%i_%s.tex" % ( paths['instructor'], lang, w, course_number, w, lang)
+            # fbody = os.path.dirname(ex_tex_out) +f"/ex{w}_body.tex"
+
+            if os.path.exists(ex_base):
+                jinjafy_template(info, ex_base, file_out=ex_tex_out, filters=filters, template_searchpath=paths['instructor'])
+                fix_shared(paths, output_dir=os.path.dirname(ex_tex_out), dosvg=dosvg)
+                # mvfiles(shared_tex, os.path.dirname(ex_tex_out)+"/")
+                latexmk(ex_tex_out, pdf_out=paths['pdf_out']+"/" + os.path.basename(ex_tex_out)[:-4] + ".pdf")
+
+def mvfiles(source_dir, dest_dir):
+    src_files = os.listdir(source_dir)
+    for file_name in src_files:
+        full_file_name = os.path.join(source_dir, file_name)
+        if (os.path.isfile(full_file_name)):
+            shutil.copy(full_file_name, os.path.dirname(dest_dir))
+
+@profile
+def make_webpage(dosvg=True):
+    cinfo = class_information()
+    paths = get_paths()
+    fix_shared(paths, output_dir=os.path.dirname(paths['homepage_out']), pdf2png=True, dosvg=dosvg)
+    wdir = paths['homepage_template']
+    jinjafy_template(cinfo, file_in=wdir, file_out=paths['homepage_out'])
+    print("Instructors for course: ")
+    s = ""
+    for dex,i in enumerate(cinfo['instructors']):
+        if dex > 0:
+            s += "; "
+        s += i['email']
+
+    blrb = os.path.dirname(paths['homepage_template']) +"/homepage_widget_blurb_template.html"
+    if os.path.exists( blrb):
+        jinjafy_template(cinfo, file_in=blrb, file_out=blrb.replace("_template.html", ".html"))
+    print(s)
+
+
+# This should probably  be moved into jinjafy
+def tt(value):
+    return "\\texttt{" + value + "}"
+
+def bf(value):
+    return "\\textbf{" + value + "}"
+
+def verb(value):
+    return '\\verb"' + value + '"'
+
+def safetex(value):
+    return value.replace("_", "\_")
+
+def slide_converter(week=None, verbose=True, clean_temporary_files=False, copy_template_resource_files=True, fix_broken_osvg_files=False, **kwargs):
+    """ Legacy function. """
+    print("Checking if slides should be converted from odf -> pdf format..")
+    paths = get_paths()
+    info = class_information()
+    # week = [week] if week not isinstance(week, list) else []
+    week = week if week is None else [week] #[week] if not week is None else
+
+    for lecture in info['lectures']:
+        # for n in range(1,14):
+        n = lecture['number']
+        if week is not None and n not in week:
+            continue
+        ldir = "%s/Lecture_%i"%(paths['lectures'], n)
+        texdir = ldir +"/Latex"
+        print("Testing conversion between directories:\n   > %s -> %s"%(ldir, texdir))
+
+        if not os.path.exists(texdir):
+            os.mkdir(texdir)
+            pdf_in = "%s/Lecture_%i.pdf"%(ldir, n)
+            pdf_out = texdir +"/Lecture_%i.pdf"%n
+            shutil.copyfile(pdf_in, pdf_out)
+
+            print("operating...")
+            lecture_tex_out = li_import(pdf_out, output_dir=texdir)
+            print("Wrote new main file: " + lecture_tex_out)
+        else:
+            print("%s exists; no conversion possible. "% (texdir,))
+
+        print("Handling .svg conversion in slides..")
+        slide_tex_path = texdir +"/Lecture_%i.tex"%n
+        print("   > "+slide_tex_path)
+        set_svg_background_images(slide_tex_path,
+                                  verbose=verbose,
+                                  clean_temporary_files=clean_temporary_files,
+                                  copy_template_resource_files=copy_template_resource_files,
+                                  fix_broken_osvg_files=fix_broken_osvg_files, **kwargs)
+
+    print("Slides converted!")
```

### Comparing `coursebox-0.1.8/src/coursebox/material/lecture_questions.py` & `coursebox-0.1.9/src/coursebox/material/lecture_questions.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,181 +1,181 @@
-import os
-import shutil
-import glob
-
-from jinjafy import jinjafy_template
-from slider import latexmk
-from coursebox.thtools_base import execute_command
-from slider.slide import slide_no_by_text, recursive_tex_apply
-from slider.legacy_importer import slide_to_image
-
-
-def lecture_question_compiler(paths, info, lecture_texfile):
-
-    lecture_latex_path = os.path.dirname(lecture_texfile)
-    lecture_pdffile = lecture_texfile[:-3] + "pdf"
-    # nosvg = lecture_pdffile[:-4] + "_NO_SVGS.pdf"
-    qpath = lecture_latex_path +"/questions"
-    if not os.path.exists(qpath):
-        os.mkdir(qpath)
-    all_questions_csv = []
-    png_out = None
-    for fn in glob.glob(qpath + "/*_base_*.tex"):
-        print(fn)
-        with open(fn, 'r') as f:
-            s = f.read()
-
-        qstart = s.find('\\begin{question}') + len("\\begin{question}")
-        qend = s.find('\\begin{solution}') #+ len('\\begin{solution}')
-        sstart = qend + len('\\begin{solution}')
-        send = s.find('\\end{solution}')
-
-        qes = s[qstart:qend]
-        sol = s[sstart:send]
-
-        a,b,c = os.path.basename(fn).split("_")
-        question_no = c.split(".")[0]
-        fout_q = qpath +"/"+a + "_" + c
-        fout_sol = qpath +"/"+ a + "_" + question_no+ "_sol.tex"
-
-        data = {'text': qes}
-        jinjafy_template(data=data, file_in=lecture_latex_path +"/questions/question_partial.tex", file_out=fout_q)
-        fout_q_pdf = qpath + "/" + latexmk(fout_q, cleanup=True)
-        execute_command(["pdfcrop", fout_q_pdf, fout_q_pdf])
-
-        # get "nice" .png file (or fallback)
-        tex = recursive_tex_apply(lecture_texfile)
-        tex = "\n".join([tex[k] for k in tex])
-        qtex = os.path.basename(fout_q)
-        dex = tex.find(qtex[:-4])
-
-
-        if dex >= 0:
-            j = tex[:dex].rfind("\\begin{frame}")
-            ol = tex[j:dex]
-            j1 = ol.find("\\osvg{")
-            j2 = ol.find("}",j1)
-
-            ol = ol[j1 + 6:j2]
-            # n = slide_no_by_text(nosvg, ol)
-            print(lecture_pdffile, ol)
-            n = slide_no_by_text(lecture_pdffile, ol)
-            if n < 0:
-                print("Question compiler: Question missing osvg label?")
-                dex = -1
-            else:
-                png_out = fout_q_pdf[:-4] + ".png"
-                print("png_out", png_out)
-                slide_to_image(lecture_pdffile, png_out, page_to_take=n)
-        if dex < 0:
-            execute_command(["pdftocairo", fout_q_pdf, fout_q_pdf[:-4], "-png"])
-            ls = glob.glob( fout_q_pdf[:-4] +"-*.png")
-            if len(ls) > 1:
-                print("Hacky, two files exist (bad/old png conversaion code", ls)
-                l2 = glob.glob(fout_q_pdf[:-4] + "-000*.png")[0]
-                os.remove(l2)
-                ls = glob.glob(fout_q_pdf[:-4] + "-*.png")
-
-
-            # print(ls)
-            if len(ls) != 1:
-                raise Exception("Multiple question png files found", ls)
-            png_out = ls[0] if ls else None
-            print("png_out b", png_out)
-
-        qdir = paths['pdf_out'] +"/quiz"
-        if not os.path.exists(qdir):
-            os.mkdir(qdir)
-        print("png_out c", png_out)
-        if png_out:
-            # a + "_" + c[:-4] + ".png"
-            # png_out2 = os.path.basename(lecture_texfile)[:-4] + "_"+os.path.basename(png_out)
-            png_out2 = os.path.basename(lecture_texfile)[:-4] + "_" + a + "_" + c[:-4] + ".png"
-            print("Copying quiz png> " + png_out2)
-            print("png_out d", png_out)
-            shutil.copyfile(png_out, qdir+"/" + png_out2)
-
-        data = {'text': sol}
-        jinjafy_template(data=data, file_in=lecture_latex_path +"/questions/question_partial.tex", file_out=fout_sol)
-        fout_sol_pdf = qpath + "/" + latexmk(fout_sol)
-        execute_command(["pdfcrop", fout_sol_pdf, fout_sol_pdf])
-
-        # Now make the cvx fileÆ
-        try:
-            ans = [l for l in qes.splitlines() if not l.strip().startswith("%") and r"\begin{answer}" in l].pop()
-        except IndexError as e:
-            print("Bad list pop", fn)
-            print(qes)
-            print(e)
-        correct = int( ans[ans.rfind("[")+1:ans.rfind("]")] )
-        answers = []
-
-        for j in range(5):
-            lbl = ([v + " is correct" for v in "ABCD"] + ["E: Don't know"] )[j]
-            points = "100" if j+1 == correct else "0"
-            answers.append( f"Option,{points},{lbl},," )
-
-        if png_out is not None:
-            l, n = os.path.basename(lecture_texfile[:-4]).split("_")
-            n = "0"+n if len(n) < 2 else n
-            csv_out = qdir + "/" + png_out2[:-3] + "csv"
-            lines = [ "NewQuestion,MC,"
-                      f"ID,{png_out2[:-4]}",
-                      f"Title,{l} {n}: Quiz {question_no}",
-                        f"QuestionText,Select correct option or Don't know,",
-                        f"Points,1,",
-                        f"Difficulty,1,",
-                        f"Image,images/quiz/{png_out2}"] +\
-                        answers
-                        # f"Hint,This is the hint text,,,",
-                        # f"Feedback,This is the feedback text,,,",
-                # ]
-            s = "\n".join(lines)
-            all_questions_csv.append(s)
-        print("Compiled question: %s"%(fout_q_pdf,))
-
-    if png_out:
-        s = "\n\n".join(all_questions_csv)
-        csv_base = qdir + "/dtulearn_csv"
-        if not os.path.isdir(csv_base):
-            os.mkdir(csv_base)
-        with open(csv_base + "/" + os.path.basename(lecture_pdffile)[:-3] + "csv", 'w') as f:
-            f.write(s)
-
-        """ 
-        //MULTIPLE CHOICE QUESTION TYPE,,
-        //Options must include text in column3,,
-        NewQuestion,MC,
-        ID,LECTURE05_question1
-        Title,Lecture 01: Quiz 1
-        QuestionText,This is thdfsklad fjasdklj fasdkl j text for MC1,
-        Points,1,
-        Difficulty,1,
-        Image,images/quizzes/Lecture_5_question_1.png
-        Option,100,This is the asdfsd correct answer,,This is feed sda fsdf asdf back for option 1
-        Option,0,This is asdfsadfsdfsadf answer 1,,This is feedback for option 2
-        Option,0,This is incorrect answer 2,,This is feedback for option 3
-        Option,0,This is partially correct,,This is feedback for option 4
-        Hint,This is the hint text,,,
-        Feedback,This is the feedback text,,,
-        """
-        # =======
-        print("Compiled question: %s"%(fout_q_pdf,))
-
-
-        """
-        //MULTIPLE CHOICE QUESTION TYPE,,
-        //Options must include text in column3,,
-        NewQuestion,MC,
-        ID,LECTURE05_question1
-        Title,Lecture 01: Quiz 1
-        QuestionText,This is thdfsklad fjasdklj fasdkl j text for MC1,
-        Points,1,
-        Difficulty,1,
-        Image,images/quizzes/Lecture_5_question_1.png
-        Option,100,This is the asdfsd correct answer,,This is feed sda fsdf asdf back for option 1
-        Option,0,This is asdfsadfsdfsadf answer 1,,This is feedback for option 2
-        Option,0,This is incorrect answer 2,,This is feedback for option 3
-        Option,0,This is partially correct,,This is feedback for option 4
-        Hint,This is the hint text,,,
-        Feedback,This is the feedback text,,,
-        """
+import os
+import shutil
+import glob
+
+from jinjafy import jinjafy_template
+from slider import latexmk
+from coursebox.thtools_base import execute_command
+from slider.slide import slide_no_by_text, recursive_tex_apply
+from slider.legacy_importer import slide_to_image
+
+
+def lecture_question_compiler(paths, info, lecture_texfile):
+
+    lecture_latex_path = os.path.dirname(lecture_texfile)
+    lecture_pdffile = lecture_texfile[:-3] + "pdf"
+    # nosvg = lecture_pdffile[:-4] + "_NO_SVGS.pdf"
+    qpath = lecture_latex_path +"/questions"
+    if not os.path.exists(qpath):
+        os.mkdir(qpath)
+    all_questions_csv = []
+    png_out = None
+    for fn in glob.glob(qpath + "/*_base_*.tex"):
+        print(fn)
+        with open(fn, 'r') as f:
+            s = f.read()
+
+        qstart = s.find('\\begin{question}') + len("\\begin{question}")
+        qend = s.find('\\begin{solution}') #+ len('\\begin{solution}')
+        sstart = qend + len('\\begin{solution}')
+        send = s.find('\\end{solution}')
+
+        qes = s[qstart:qend]
+        sol = s[sstart:send]
+
+        a,b,c = os.path.basename(fn).split("_")
+        question_no = c.split(".")[0]
+        fout_q = qpath +"/"+a + "_" + c
+        fout_sol = qpath +"/"+ a + "_" + question_no+ "_sol.tex"
+
+        data = {'text': qes}
+        jinjafy_template(data=data, file_in=lecture_latex_path +"/questions/question_partial.tex", file_out=fout_q)
+        fout_q_pdf = qpath + "/" + latexmk(fout_q, cleanup=True)
+        execute_command(["pdfcrop", fout_q_pdf, fout_q_pdf])
+
+        # get "nice" .png file (or fallback)
+        tex = recursive_tex_apply(lecture_texfile)
+        tex = "\n".join([tex[k] for k in tex])
+        qtex = os.path.basename(fout_q)
+        dex = tex.find(qtex[:-4])
+
+
+        if dex >= 0:
+            j = tex[:dex].rfind("\\begin{frame}")
+            ol = tex[j:dex]
+            j1 = ol.find("\\osvg{")
+            j2 = ol.find("}",j1)
+
+            ol = ol[j1 + 6:j2]
+            # n = slide_no_by_text(nosvg, ol)
+            print(lecture_pdffile, ol)
+            n = slide_no_by_text(lecture_pdffile, ol)
+            if n < 0:
+                print("Question compiler: Question missing osvg label?")
+                dex = -1
+            else:
+                png_out = fout_q_pdf[:-4] + ".png"
+                print("png_out", png_out)
+                slide_to_image(lecture_pdffile, png_out, page_to_take=n)
+        if dex < 0:
+            execute_command(["pdftocairo", fout_q_pdf, fout_q_pdf[:-4], "-png"])
+            ls = glob.glob( fout_q_pdf[:-4] +"-*.png")
+            if len(ls) > 1:
+                print("Hacky, two files exist (bad/old png conversaion code", ls)
+                l2 = glob.glob(fout_q_pdf[:-4] + "-000*.png")[0]
+                os.remove(l2)
+                ls = glob.glob(fout_q_pdf[:-4] + "-*.png")
+
+
+            # print(ls)
+            if len(ls) != 1:
+                raise Exception("Multiple question png files found", ls)
+            png_out = ls[0] if ls else None
+            print("png_out b", png_out)
+
+        qdir = paths['pdf_out'] +"/quiz"
+        if not os.path.exists(qdir):
+            os.mkdir(qdir)
+        print("png_out c", png_out)
+        if png_out:
+            # a + "_" + c[:-4] + ".png"
+            # png_out2 = os.path.basename(lecture_texfile)[:-4] + "_"+os.path.basename(png_out)
+            png_out2 = os.path.basename(lecture_texfile)[:-4] + "_" + a + "_" + c[:-4] + ".png"
+            print("Copying quiz png> " + png_out2)
+            print("png_out d", png_out)
+            shutil.copyfile(png_out, qdir+"/" + png_out2)
+
+        data = {'text': sol}
+        jinjafy_template(data=data, file_in=lecture_latex_path +"/questions/question_partial.tex", file_out=fout_sol)
+        fout_sol_pdf = qpath + "/" + latexmk(fout_sol)
+        execute_command(["pdfcrop", fout_sol_pdf, fout_sol_pdf])
+
+        # Now make the cvx fileÆ
+        try:
+            ans = [l for l in qes.splitlines() if not l.strip().startswith("%") and r"\begin{answer}" in l].pop()
+        except IndexError as e:
+            print("Bad list pop", fn)
+            print(qes)
+            print(e)
+        correct = int( ans[ans.rfind("[")+1:ans.rfind("]")] )
+        answers = []
+
+        for j in range(5):
+            lbl = ([v + " is correct" for v in "ABCD"] + ["E: Don't know"] )[j]
+            points = "100" if j+1 == correct else "0"
+            answers.append( f"Option,{points},{lbl},," )
+
+        if png_out is not None:
+            l, n = os.path.basename(lecture_texfile[:-4]).split("_")
+            n = "0"+n if len(n) < 2 else n
+            csv_out = qdir + "/" + png_out2[:-3] + "csv"
+            lines = [ "NewQuestion,MC,"
+                      f"ID,{png_out2[:-4]}",
+                      f"Title,{l} {n}: Quiz {question_no}",
+                        f"QuestionText,Select correct option or Don't know,",
+                        f"Points,1,",
+                        f"Difficulty,1,",
+                        f"Image,images/quiz/{png_out2}"] +\
+                        answers
+                        # f"Hint,This is the hint text,,,",
+                        # f"Feedback,This is the feedback text,,,",
+                # ]
+            s = "\n".join(lines)
+            all_questions_csv.append(s)
+        print("Compiled question: %s"%(fout_q_pdf,))
+
+    if png_out:
+        s = "\n\n".join(all_questions_csv)
+        csv_base = qdir + "/dtulearn_csv"
+        if not os.path.isdir(csv_base):
+            os.mkdir(csv_base)
+        with open(csv_base + "/" + os.path.basename(lecture_pdffile)[:-3] + "csv", 'w') as f:
+            f.write(s)
+
+        """ 
+        //MULTIPLE CHOICE QUESTION TYPE,,
+        //Options must include text in column3,,
+        NewQuestion,MC,
+        ID,LECTURE05_question1
+        Title,Lecture 01: Quiz 1
+        QuestionText,This is thdfsklad fjasdklj fasdkl j text for MC1,
+        Points,1,
+        Difficulty,1,
+        Image,images/quizzes/Lecture_5_question_1.png
+        Option,100,This is the asdfsd correct answer,,This is feed sda fsdf asdf back for option 1
+        Option,0,This is asdfsadfsdfsadf answer 1,,This is feedback for option 2
+        Option,0,This is incorrect answer 2,,This is feedback for option 3
+        Option,0,This is partially correct,,This is feedback for option 4
+        Hint,This is the hint text,,,
+        Feedback,This is the feedback text,,,
+        """
+        # =======
+        print("Compiled question: %s"%(fout_q_pdf,))
+
+
+        """
+        //MULTIPLE CHOICE QUESTION TYPE,,
+        //Options must include text in column3,,
+        NewQuestion,MC,
+        ID,LECTURE05_question1
+        Title,Lecture 01: Quiz 1
+        QuestionText,This is thdfsklad fjasdklj fasdkl j text for MC1,
+        Points,1,
+        Difficulty,1,
+        Image,images/quizzes/Lecture_5_question_1.png
+        Option,100,This is the asdfsd correct answer,,This is feed sda fsdf asdf back for option 1
+        Option,0,This is asdfsadfsdfsadf answer 1,,This is feedback for option 2
+        Option,0,This is incorrect answer 2,,This is feedback for option 3
+        Option,0,This is partially correct,,This is feedback for option 4
+        Hint,This is the hint text,,,
+        Feedback,This is the feedback text,,,
+        """
```

### Comparing `coursebox-0.1.8/src/coursebox/setup_coursebox.py` & `coursebox-0.1.9/src/coursebox/setup_coursebox.py`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-from coursebox.core import info_paths
-
-def setup_coursebox(working_dir, course_number="02450", semester='spring', year=2019,
-    slides_showsolutions=True,
-    slides_includelabels=False,
-    continuing_education_mode = False,
-    slides_shownotes=False,
-    continuing_education_month = "March", **kwargs):
-
-    info_paths.core_conf['working_dir'] = working_dir
-    info_paths.core_conf['course_number'] = course_number
-    info_paths.core_conf['semester'] = semester
-    info_paths.core_conf['year'] = year
-    info_paths.core_conf['slides_showsolutions'] = slides_showsolutions
-    info_paths.core_conf['slides_includelabels'] = slides_includelabels
-    info_paths.core_conf['continuing_education_mode'] = continuing_education_mode
-    info_paths.core_conf['continuing_education_month'] = continuing_education_month
-    info_paths.core_conf['slides_shownotes'] = slides_shownotes
-    for a, val in kwargs.items():
-        info_paths.core_conf[a] = val
+from coursebox.core import info_paths
+
+def setup_coursebox(working_dir, course_number="02450", semester='spring', year=2019,
+    slides_showsolutions=True,
+    slides_includelabels=False,
+    continuing_education_mode = False,
+    slides_shownotes=False,
+    continuing_education_month = "March", **kwargs):
+
+    info_paths.core_conf['working_dir'] = working_dir
+    info_paths.core_conf['course_number'] = course_number
+    info_paths.core_conf['semester'] = semester
+    info_paths.core_conf['year'] = year
+    info_paths.core_conf['slides_showsolutions'] = slides_showsolutions
+    info_paths.core_conf['slides_includelabels'] = slides_includelabels
+    info_paths.core_conf['continuing_education_mode'] = continuing_education_mode
+    info_paths.core_conf['continuing_education_month'] = continuing_education_month
+    info_paths.core_conf['slides_shownotes'] = slides_shownotes
+    for a, val in kwargs.items():
+        info_paths.core_conf[a] = val
```

### Comparing `coursebox-0.1.8/src/coursebox/thtools_base.py` & `coursebox-0.1.9/src/coursebox/thtools_base.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,155 +1,155 @@
-import os
-import platform
-import subprocess
-import inspect
-
-
-def is_win():
-    # if sys.platform()
-    return platform.uname()[0].startswith("Windows")
-
-
-def is_compute():
-    return platform.uname()[1] == "linuxterm1"
-
-
-def is_gbar():
-    return False
-
-def is_cogsys_cluster():
-    return platform.uname()[0] == "Linux" and os.path.exists("/dtu-compute") and not is_compute()
-
-def is_cluster():
-    return is_compute() or is_gbar() or is_cogsys_cluster()
-
-def get_system_name():
-    if is_win():
-        return "Win"
-    if is_compute():
-        return "thinlinc.compute.dtu.dk"
-    if is_cogsys_cluster():
-        return "cogys cluster"
-
-def execute_command(command, shell=True):
-    if not isinstance(command, list):
-        command = [command]
-    if not is_compute():
-        result = subprocess.run(command, stdout=subprocess.PIPE, shell=shell)
-        out = result.stdout
-    else:
-        out = subprocess.check_output(command, shell=shell)
-    s = out.decode("utf-8")
-    OK = True
-    return s, OK
-
-# def git_pull(repo_dir=None):
-#     import pbs # should switch to sh when it gets windows support.
-#     gitty = pbs.Command('git')
-#     # args = {}
-#     # if repo_dir is not None:
-#     #     kwargs = {'_cwd': repo_dir}
-#     # if repo_dir is not None:
-#     r = gitty("pull", _cwd=repo_dir)
-#     # else:
-#     #     r = gitty("pull")
-#     err = r.stderr
-#     if err is not None and err is not "":
-#         print("thtools_base.git_pull(), encountered error", err)
-
-
-# def git_commit_push(repo_dir=None, commit="default commit message from thtools farm"):
-#     import pbs
-#     gitty = pbs.Command('git')
-#     # probably it is a good idea to check the status
-#
-#     # repo_dir
-#
-#     r1 = gitty("add", ".", _cwd=repo_dir)
-#     try:
-#         r2 = gitty("commit", "-m'%s'"%commit, _cwd=repo_dir)
-#     except pbs.ErrorReturnCode_1:
-#         print("Error in git push!")
-#         # print(r2.stderr)
-#
-#     r3 = gitty("push",  _cwd=repo_dir)
-
-
-# Returns the base root of thtools
-# def thtools_root_dir():
-#     frame = inspect.stack()[0]
-#     module = inspect.getmodule(frame[0])
-#     file_in = os.path.dirname(module.__file__)
-#     return file_in
-
-
-def get_callstack(nback=2):
-    x = inspect.currentframe()
-    for j in range(nback):
-        x = x.f_back
-    ff = os.path.abspath(inspect.getfile(x))
-    return ff, x.f_lineno, x
-
-
-def caller_script_path():
-    frame = inspect.stack()[1]
-    module = inspect.getmodule(frame[0])
-    file_in = module.__file__
-    return file_in
-
-
-def pprint(d, indent=0):
-   for key, value in d.items():
-      print('\t' * indent + str(key))
-      if isinstance(value, dict):
-         pprint(value, indent+1)
-      else:
-         print('\t' * (indent+1) + str(value))
-
-def list_dict2dict_list(lst, along_new_axis=True):
-    import numpy as np
-    if not lst:
-        return dict()
-    dc = dict()
-    for key in lst[0].keys():
-        dc[key] = np.stack([l[key] for l in lst if key in l], axis=0)
-    if not along_new_axis:
-        raise Exception("Should probably implement new axis = false")
-    return dc
-
-
-def partition_list(I,K,randomize=False):
-    import numpy as np
-    J = np.arange(len(I))
-    if randomize:
-        J = np.random.permutation(J)
-
-    spl = np.array_split(J, K)
-    di = []
-    for chunk in spl:
-        x = []
-        for j in chunk:
-            x.append(I[j])
-        di.append(x)
-    return di
-
-
-def watermark_string(nback=2):
-
-    from datetime import datetime
-
-    tm =  datetime.now().strftime('%b-%d-%I:%M%p')
-    # for line in traceback.format_stack():
-    #     #     print(line.strip())
-    v = inspect.stack()
-    ss = []
-    j = 0
-    for i in range(len(v)):
-        if "plot_helpers.py" in v[i].filename: continue
-        ss.append( os.path.basename( v[i].filename) )
-        j = j + 1
-        if j > nback: break
-    # from thtools import execute_command
-    v, _ = execute_command("git rev-parse --short HEAD".split())
-
-    ss.append(tm)
-    return ('/'.join(ss) + f" @{v}").strip()
+import os
+import platform
+import subprocess
+import inspect
+
+
+def is_win():
+    # if sys.platform()
+    return platform.uname()[0].startswith("Windows")
+
+
+def is_compute():f
+    return platform.uname()[1] == "linuxterm1"
+
+
+def is_gbar():
+    return False
+
+def is_cogsys_cluster():
+    return platform.uname()[0] == "Linux" and os.path.exists("/dtu-compute") and not is_compute()
+
+def is_cluster():
+    return is_compute() or is_gbar() or is_cogsys_cluster()
+
+def get_system_name():
+    if is_win():
+        return "Win"
+    if is_compute():
+        return "thinlinc.compute.dtu.dk"
+    if is_cogsys_cluster():
+        return "cogys cluster"
+
+def execute_command(command, shell=True):
+    if not isinstance(command, list):
+        command = [command]
+    if not is_compute():
+        result = subprocess.run(command, stdout=subprocess.PIPE, shell=shell)
+        out = result.stdout
+    else:
+        out = subprocess.check_output(command, shell=shell)
+    s = out.decode("utf-8")
+    OK = True
+    return s, OK
+
+# def git_pull(repo_dir=None):
+#     import pbs # should switch to sh when it gets windows support.
+#     gitty = pbs.Command('git')
+#     # args = {}
+#     # if repo_dir is not None:
+#     #     kwargs = {'_cwd': repo_dir}
+#     # if repo_dir is not None:
+#     r = gitty("pull", _cwd=repo_dir)
+#     # else:
+#     #     r = gitty("pull")
+#     err = r.stderr
+#     if err is not None and err is not "":
+#         print("thtools_base.git_pull(), encountered error", err)
+
+
+# def git_commit_push(repo_dir=None, commit="default commit message from thtools farm"):
+#     import pbs
+#     gitty = pbs.Command('git')
+#     # probably it is a good idea to check the status
+#
+#     # repo_dir
+#
+#     r1 = gitty("add", ".", _cwd=repo_dir)
+#     try:
+#         r2 = gitty("commit", "-m'%s'"%commit, _cwd=repo_dir)
+#     except pbs.ErrorReturnCode_1:
+#         print("Error in git push!")
+#         # print(r2.stderr)
+#
+#     r3 = gitty("push",  _cwd=repo_dir)
+
+
+# Returns the base root of thtools
+# def thtools_root_dir():
+#     frame = inspect.stack()[0]
+#     module = inspect.getmodule(frame[0])
+#     file_in = os.path.dirname(module.__file__)
+#     return file_in
+
+
+def get_callstack(nback=2):
+    x = inspect.currentframe()
+    for j in range(nback):
+        x = x.f_back
+    ff = os.path.abspath(inspect.getfile(x))
+    return ff, x.f_lineno, x
+
+
+def caller_script_path():
+    frame = inspect.stack()[1]
+    module = inspect.getmodule(frame[0])
+    file_in = module.__file__
+    return file_in
+
+
+def pprint(d, indent=0):
+   for key, value in d.items():
+      print('\t' * indent + str(key))
+      if isinstance(value, dict):
+         pprint(value, indent+1)
+      else:
+         print('\t' * (indent+1) + str(value))
+
+def list_dict2dict_list(lst, along_new_axis=True):
+    import numpy as np
+    if not lst:
+        return dict()
+    dc = dict()
+    for key in lst[0].keys():
+        dc[key] = np.stack([l[key] for l in lst if key in l], axis=0)
+    if not along_new_axis:
+        raise Exception("Should probably implement new axis = false")
+    return dc
+
+
+def partition_list(I,K,randomize=False):
+    import numpy as np
+    J = np.arange(len(I))
+    if randomize:
+        J = np.random.permutation(J)
+
+    spl = np.array_split(J, K)
+    di = []
+    for chunk in spl:
+        x = []
+        for j in chunk:
+            x.append(I[j])
+        di.append(x)
+    return di
+
+
+def watermark_string(nback=2):
+
+    from datetime import datetime
+
+    tm =  datetime.now().strftime('%b-%d-%I:%M%p')
+    # for line in traceback.format_stack():
+    #     #     print(line.strip())
+    v = inspect.stack()
+    ss = []
+    j = 0
+    for i in range(len(v)):
+        if "plot_helpers.py" in v[i].filename: continue
+        ss.append( os.path.basename( v[i].filename) )
+        j = j + 1
+        if j > nback: break
+    # from thtools import execute_command
+    v, _ = execute_command("git rev-parse --short HEAD".split())
+
+    ss.append(tm)
+    return ('/'.join(ss) + f" @{v}").strip()
```

### Comparing `coursebox-0.1.8/src/coursebox.egg-info/PKG-INFO` & `coursebox-0.1.9/src/coursebox.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,47 +1,47 @@
-Metadata-Version: 2.1
-Name: coursebox
-Version: 0.1.8
-Summary: A course management system currently used at DTU
-Home-page: https://lab.compute.dtu.dk/tuhe/coursebox
-Author: Tue Herlau
-Author-email: tuhe@dtu.dk
-License: MIT
-Project-URL: Bug Tracker, https://lab.compute.dtu.dk/tuhe/coursebox/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# Coursebox DTU
-DTU course management software.
-
-## Installation
-```terminal
-pip install coursebox
-```
-## What it can do 
- - Single semester-dependent configuration file
- - Integrates with DTU Inside/DTU Learn
- - Distribution/evalauation of project reports in Learn-compatible format
- - Quiz-generation in DTU Learn/Beamer friendly format
- - Automatic website/syllabus generation 
- - Automatic generation of lectures handouts/exercises (you don't have to track dynamic content like dates/lecture titles; it is all in the configuration)
- - Easy compilation to 2/5 day formats (Continuous education)
-
-## Usage
-Coursebox requires a specific directory structure. It is easier to start with an existing course and adapt to your needs. Please contact me at tuhe@dtu.dk for more information.
-
-## Citing
-```bibtex
-@online{coursebox,
-	title={Coursebox (0.1.1): \texttt{pip install coursebox}},
-	url={https://lab.compute.dtu.dk/tuhe/coursebox},
-	urldate = {2021-09-07}, 
-	month={9},
-	publisher={Technical University of Denmark (DTU)},
-	author={Tue Herlau},
-	year={2021},
-}
-```
+Metadata-Version: 2.1
+Name: coursebox
+Version: 0.1.9
+Summary: A course management system currently used at DTU
+Home-page: https://lab.compute.dtu.dk/tuhe/coursebox
+Author: Tue Herlau
+Author-email: tuhe@dtu.dk
+License: MIT
+Project-URL: Bug Tracker, https://lab.compute.dtu.dk/tuhe/coursebox/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# Coursebox DTU
+DTU course management software.
+
+## Installation
+```terminal
+pip install coursebox
+```
+## What it can do 
+ - Single semester-dependent configuration file
+ - Integrates with DTU Inside/DTU Learn
+ - Distribution/evalauation of project reports in Learn-compatible format
+ - Quiz-generation in DTU Learn/Beamer friendly format
+ - Automatic website/syllabus generation 
+ - Automatic generation of lectures handouts/exercises (you don't have to track dynamic content like dates/lecture titles; it is all in the configuration)
+ - Easy compilation to 2/5 day formats (Continuous education)
+
+## Usage
+Coursebox requires a specific directory structure. It is easier to start with an existing course and adapt to your needs. Please contact me at tuhe@dtu.dk for more information.
+
+## Citing
+```bibtex
+@online{coursebox,
+	title={Coursebox (0.1.1): \texttt{pip install coursebox}},
+	url={https://lab.compute.dtu.dk/tuhe/coursebox},
+	urldate = {2021-09-07}, 
+	month={9},
+	publisher={Technical University of Denmark (DTU)},
+	author={Tue Herlau},
+	year={2021},
+}
+```
```

### Comparing `coursebox-0.1.8/src/coursebox.egg-info/SOURCES.txt` & `coursebox-0.1.9/src/coursebox.egg-info/SOURCES.txt`

 * *Files identical despite different names*

