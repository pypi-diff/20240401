# Comparing `tmp/par_run-0.1.2.tar.gz` & `tmp/par_run-0.1.3.tar.gz`

## Comparing `par_run-0.1.2.tar` & `par_run-0.1.3.tar`

### file list

```diff
@@ -1,36 +1,36 @@
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 par_run-0.1.2/.python-version
--rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 par_run-0.1.2/commands.ini
--rw-r--r--   0        0        0     3781 2020-02-02 00:00:00.000000 par_run-0.1.2/requirements-dev.lock
--rw-r--r--   0        0        0     1469 2020-02-02 00:00:00.000000 par_run-0.1.2/requirements.lock
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 par_run-0.1.2/.reports/html/.gitignore
--rw-r--r--   0        0        0    21865 2020-02-02 00:00:00.000000 par_run-0.1.2/.reports/html/coverage_html.js
--rw-r--r--   0        0        0     4988 2020-02-02 00:00:00.000000 par_run-0.1.2/.reports/html/d_417a353b6036f046___init___py.html
--rw-r--r--   0        0        0    78275 2020-02-02 00:00:00.000000 par_run-0.1.2/.reports/html/d_417a353b6036f046_cli_py.html
--rw-r--r--   0        0        0   106323 2020-02-02 00:00:00.000000 par_run-0.1.2/.reports/html/d_417a353b6036f046_executor_py.html
--rw-r--r--   0        0        0    46396 2020-02-02 00:00:00.000000 par_run-0.1.2/.reports/html/d_417a353b6036f046_web_cli_py.html
--rw-r--r--   0        0        0    23925 2020-02-02 00:00:00.000000 par_run-0.1.2/.reports/html/d_417a353b6036f046_web_py.html
--rw-r--r--   0        0        0     1732 2020-02-02 00:00:00.000000 par_run-0.1.2/.reports/html/favicon_32.png
--rw-r--r--   0        0        0     4813 2020-02-02 00:00:00.000000 par_run-0.1.2/.reports/html/index.html
--rw-r--r--   0        0        0     9004 2020-02-02 00:00:00.000000 par_run-0.1.2/.reports/html/keybd_closed.png
--rw-r--r--   0        0        0     9003 2020-02-02 00:00:00.000000 par_run-0.1.2/.reports/html/keybd_open.png
--rw-r--r--   0        0        0     1333 2020-02-02 00:00:00.000000 par_run-0.1.2/.reports/html/status.json
--rw-r--r--   0        0        0    12394 2020-02-02 00:00:00.000000 par_run-0.1.2/.reports/html/style.css
--rw-r--r--   0        0        0      684 2020-02-02 00:00:00.000000 par_run-0.1.2/.vscode/launch.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 par_run-0.1.2/py_tests/__init__.py
--rw-r--r--   0        0        0      654 2020-02-02 00:00:00.000000 par_run-0.1.2/py_tests/conftest.py
--rw-r--r--   0        0        0    14099 2020-02-02 00:00:00.000000 par_run-0.1.2/py_tests/test_cli.py
--rw-r--r--   0        0        0    13799 2020-02-02 00:00:00.000000 par_run-0.1.2/py_tests/test_executor.py
--rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 par_run-0.1.2/py_tests/test_main.py
--rw-r--r--   0        0        0     4514 2020-02-02 00:00:00.000000 par_run-0.1.2/py_tests/test_web.py
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 par_run-0.1.2/src/par_run/__init__.py
--rw-r--r--   0        0        0     8649 2020-02-02 00:00:00.000000 par_run-0.1.2/src/par_run/cli.py
--rw-r--r--   0        0        0    11823 2020-02-02 00:00:00.000000 par_run-0.1.2/src/par_run/executor.py
--rw-r--r--   0        0        0     2147 2020-02-02 00:00:00.000000 par_run-0.1.2/src/par_run/web.py
--rw-r--r--   0        0        0     4317 2020-02-02 00:00:00.000000 par_run-0.1.2/src/par_run/static/css/style.css
--rw-r--r--   0        0        0     8623 2020-02-02 00:00:00.000000 par_run-0.1.2/src/par_run/static/js/app.js
--rw-r--r--   0        0        0     2087 2020-02-02 00:00:00.000000 par_run-0.1.2/src/par_run/templates/index.html
--rw-r--r--   0        0        0     3098 2020-02-02 00:00:00.000000 par_run-0.1.2/.gitignore
--rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 par_run-0.1.2/LICENSE
--rw-r--r--   0        0        0     1447 2020-02-02 00:00:00.000000 par_run-0.1.2/README.md
--rw-r--r--   0        0        0     1883 2020-02-02 00:00:00.000000 par_run-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     1991 2020-02-02 00:00:00.000000 par_run-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 par_run-0.1.3/.python-version
+-rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 par_run-0.1.3/commands.ini
+-rw-r--r--   0        0        0     3781 2020-02-02 00:00:00.000000 par_run-0.1.3/requirements-dev.lock
+-rw-r--r--   0        0        0     1469 2020-02-02 00:00:00.000000 par_run-0.1.3/requirements.lock
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 par_run-0.1.3/.reports/html/.gitignore
+-rw-r--r--   0        0        0    21865 2020-02-02 00:00:00.000000 par_run-0.1.3/.reports/html/coverage_html.js
+-rw-r--r--   0        0        0     4988 2020-02-02 00:00:00.000000 par_run-0.1.3/.reports/html/d_417a353b6036f046___init___py.html
+-rw-r--r--   0        0        0    78275 2020-02-02 00:00:00.000000 par_run-0.1.3/.reports/html/d_417a353b6036f046_cli_py.html
+-rw-r--r--   0        0        0   106323 2020-02-02 00:00:00.000000 par_run-0.1.3/.reports/html/d_417a353b6036f046_executor_py.html
+-rw-r--r--   0        0        0    46396 2020-02-02 00:00:00.000000 par_run-0.1.3/.reports/html/d_417a353b6036f046_web_cli_py.html
+-rw-r--r--   0        0        0    23925 2020-02-02 00:00:00.000000 par_run-0.1.3/.reports/html/d_417a353b6036f046_web_py.html
+-rw-r--r--   0        0        0     1732 2020-02-02 00:00:00.000000 par_run-0.1.3/.reports/html/favicon_32.png
+-rw-r--r--   0        0        0     4813 2020-02-02 00:00:00.000000 par_run-0.1.3/.reports/html/index.html
+-rw-r--r--   0        0        0     9004 2020-02-02 00:00:00.000000 par_run-0.1.3/.reports/html/keybd_closed.png
+-rw-r--r--   0        0        0     9003 2020-02-02 00:00:00.000000 par_run-0.1.3/.reports/html/keybd_open.png
+-rw-r--r--   0        0        0     1333 2020-02-02 00:00:00.000000 par_run-0.1.3/.reports/html/status.json
+-rw-r--r--   0        0        0    12394 2020-02-02 00:00:00.000000 par_run-0.1.3/.reports/html/style.css
+-rw-r--r--   0        0        0      684 2020-02-02 00:00:00.000000 par_run-0.1.3/.vscode/launch.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 par_run-0.1.3/py_tests/__init__.py
+-rw-r--r--   0        0        0      654 2020-02-02 00:00:00.000000 par_run-0.1.3/py_tests/conftest.py
+-rw-r--r--   0        0        0    14099 2020-02-02 00:00:00.000000 par_run-0.1.3/py_tests/test_cli.py
+-rw-r--r--   0        0        0    13799 2020-02-02 00:00:00.000000 par_run-0.1.3/py_tests/test_executor.py
+-rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 par_run-0.1.3/py_tests/test_main.py
+-rw-r--r--   0        0        0     4514 2020-02-02 00:00:00.000000 par_run-0.1.3/py_tests/test_web.py
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 par_run-0.1.3/src/par_run/__init__.py
+-rw-r--r--   0        0        0     8649 2020-02-02 00:00:00.000000 par_run-0.1.3/src/par_run/cli.py
+-rw-r--r--   0        0        0    11823 2020-02-02 00:00:00.000000 par_run-0.1.3/src/par_run/executor.py
+-rw-r--r--   0        0        0     2147 2020-02-02 00:00:00.000000 par_run-0.1.3/src/par_run/web.py
+-rw-r--r--   0        0        0     4317 2020-02-02 00:00:00.000000 par_run-0.1.3/src/par_run/static/css/style.css
+-rw-r--r--   0        0        0     8623 2020-02-02 00:00:00.000000 par_run-0.1.3/src/par_run/static/js/app.js
+-rw-r--r--   0        0        0     2087 2020-02-02 00:00:00.000000 par_run-0.1.3/src/par_run/templates/index.html
+-rw-r--r--   0        0        0     3098 2020-02-02 00:00:00.000000 par_run-0.1.3/.gitignore
+-rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 par_run-0.1.3/LICENSE
+-rw-r--r--   0        0        0     1408 2020-02-02 00:00:00.000000 par_run-0.1.3/README.md
+-rw-r--r--   0        0        0     2629 2020-02-02 00:00:00.000000 par_run-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     2769 2020-02-02 00:00:00.000000 par_run-0.1.3/PKG-INFO
```

### Comparing `par_run-0.1.2/requirements-dev.lock` & `par_run-0.1.3/requirements-dev.lock`

 * *Files identical despite different names*

### Comparing `par_run-0.1.2/requirements.lock` & `par_run-0.1.3/requirements.lock`

 * *Files identical despite different names*

### Comparing `par_run-0.1.2/.reports/html/coverage_html.js` & `par_run-0.1.3/.reports/html/coverage_html.js`

 * *Files identical despite different names*

### Comparing `par_run-0.1.2/.reports/html/d_417a353b6036f046___init___py.html` & `par_run-0.1.3/.reports/html/d_417a353b6036f046___init___py.html`

 * *Files 2% similar despite different names*

```diff
@@ -61,15 +61,15 @@
         </h2>
         <p class="text">
             <a id="prevFileLink" class="nav" href="index.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_417a353b6036f046_cli_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.4.4">coverage.py v7.4.4</a>,
-            created at 2024-03-28 13:21 -0400
+            created at 2024-04-01 07:45 -0400
         </p>
         <aside class="hidden">
             <button type="button" class="button_next_chunk" data-shortcut="j"/>
             <button type="button" class="button_prev_chunk" data-shortcut="k"/>
             <button type="button" class="button_top_of_page" data-shortcut="0"/>
             <button type="button" class="button_first_chunk" data-shortcut="1"/>
             <button type="button" class="button_prev_file" data-shortcut="["/>
@@ -78,23 +78,23 @@
             <button type="button" class="button_show_hide_help" data-shortcut="?"/>
         </aside>
     </div>
 </header>
 <main id="source">
     <p class="pln"><span class="n"><a id="t1" href="#t1">1</a></span><span class="t"><span class="str">"""Main module for the py_runner package."""</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t2" href="#t2">2</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t3" href="#t3">3</a></span><span class="t"><span class="nam">__version__</span> <span class="op">=</span> <span class="str">"0.1.1"</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t3" href="#t3">3</a></span><span class="t"><span class="nam">__version__</span> <span class="op">=</span> <span class="str">"0.1.2"</span>&nbsp;</span><span class="r"></span></p>
 </main>
 <footer>
     <div class="content">
         <p>
             <a id="prevFileLink" class="nav" href="index.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_417a353b6036f046_cli_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.4.4">coverage.py v7.4.4</a>,
-            created at 2024-03-28 13:21 -0400
+            created at 2024-04-01 07:45 -0400
         </p>
     </div>
 </footer>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -5,14 +5,14 @@
 j k   next/prev highlighted chunk
 0   (zero) top of page
 1   (one) first highlighted chunk
 [ ]   prev/next file
 u   up to the index
 ?   show/hide this help
 ********** 11 ssttaatteemmeennttss ?  11 rruunn 00 mmiissssiinngg 00 eexxcclluuddeedd **********
-_«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._4_._4, created at 2024-03-
-28 13:21 -0400
+_«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._4_._4, created at 2024-04-
+01 07:45 -0400
 _1"""Main module for the py_runner package.""" 
 _2 
-_3__version__ = "0.1.1" 
-_«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._4_._4, created at 2024-03-
-28 13:21 -0400
+_3__version__ = "0.1.2" 
+_«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._4_._4, created at 2024-04-
+01 07:45 -0400
```

### Comparing `par_run-0.1.2/.reports/html/d_417a353b6036f046_cli_py.html` & `par_run-0.1.3/.reports/html/d_417a353b6036f046_cli_py.html`

 * *Files identical despite different names*

### Comparing `par_run-0.1.2/.reports/html/d_417a353b6036f046_executor_py.html` & `par_run-0.1.3/.reports/html/d_417a353b6036f046_executor_py.html`

 * *Files identical despite different names*

### Comparing `par_run-0.1.2/.reports/html/d_417a353b6036f046_web_cli_py.html` & `par_run-0.1.3/.reports/html/d_417a353b6036f046_web_cli_py.html`

 * *Files identical despite different names*

### Comparing `par_run-0.1.2/.reports/html/d_417a353b6036f046_web_py.html` & `par_run-0.1.3/.reports/html/d_417a353b6036f046_web_py.html`

 * *Files identical despite different names*

### Comparing `par_run-0.1.2/.reports/html/favicon_32.png` & `par_run-0.1.3/.reports/html/favicon_32.png`

 * *Files identical despite different names*

### Comparing `par_run-0.1.2/.reports/html/index.html` & `par_run-0.1.3/.reports/html/index.html`

 * *Files 0% similar despite different names*

```diff
@@ -41,15 +41,15 @@
             </div>
         </aside>
         <form id="filter_container">
             <input id="filter" type="text" value="" placeholder="filter..." />
         </form>
         <p class="text">
             <a class="nav" href="https://coverage.readthedocs.io/en/7.4.4">coverage.py v7.4.4</a>,
-            created at 2024-03-31 17:11 -0400
+            created at 2024-04-01 07:45 -0400
         </p>
     </div>
 </header>
 <main id="index">
     <table class="index" data-sortable>
         <thead>
             <tr class="tablehead" title="Click to sort">
@@ -104,15 +104,15 @@
         No items found using the specified filter.
     </p>
 </main>
 <footer>
     <div class="content">
         <p>
             <a class="nav" href="https://coverage.readthedocs.io/en/7.4.4">coverage.py v7.4.4</a>,
-            created at 2024-03-31 17:11 -0400
+            created at 2024-04-01 07:45 -0400
         </p>
     </div>
     <aside class="hidden">
         <a id="prevFileLink" class="nav" href="d_417a353b6036f046_web_py.html"/>
         <a id="nextFileLink" class="nav" href="d_417a353b6036f046___init___py.html"/>
         <button type="button" class="button_prev_file" data-shortcut="["/>
         <button type="button" class="button_next_file" data-shortcut="]"/>
```

#### html2text {}

```diff
@@ -1,16 +1,16 @@
 ************ CCoovveerraaggee rreeppoorrtt:: 9922%% ************
 ??[Show/hide keyboard shortcuts]
 Shortcuts on this page
 n s m x c   change column sorting
 [ ]   prev/next file
 ?   show/hide this help
 [                    ]
-_c_o_v_e_r_a_g_e_._p_y_ _v_7_._4_._4, created at 2024-03-31 17:11 -0400
+_c_o_v_e_r_a_g_e_._p_y_ _v_7_._4_._4, created at 2024-04-01 07:45 -0400
 MMoodduullee                  ssttaatteemmeennttss mmiissssiinngg eexxcclluuddeedd ccoovveerraaggee
 _s_r_c_/_p_a_r___r_u_n_/_____i_n_i_t_____._p_y 1          0       0        100%
 _s_r_c_/_p_a_r___r_u_n_/_c_l_i_._p_y      162        15      2        91%
 _s_r_c_/_p_a_r___r_u_n_/_e_x_e_c_u_t_o_r_._p_y 203        5       7        98%
 _s_r_c_/_p_a_r___r_u_n_/_w_e_b_._p_y      41         12      0        71%
 Total                   407        32      9        92%
 No items found using the specified filter.
-_c_o_v_e_r_a_g_e_._p_y_ _v_7_._4_._4, created at 2024-03-31 17:11 -0400
+_c_o_v_e_r_a_g_e_._p_y_ _v_7_._4_._4, created at 2024-04-01 07:45 -0400
```

### Comparing `par_run-0.1.2/.reports/html/keybd_closed.png` & `par_run-0.1.3/.reports/html/keybd_closed.png`

 * *Files identical despite different names*

### Comparing `par_run-0.1.2/.reports/html/keybd_open.png` & `par_run-0.1.3/.reports/html/keybd_open.png`

 * *Files identical despite different names*

### Comparing `par_run-0.1.2/.reports/html/status.json` & `par_run-0.1.3/.reports/html/status.json`

 * *Files 13% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9974999999999999%*

 * *Differences: {"'files'": "{'d_417a353b6036f046___init___py': {'hash': 'ccb563545275a070316909877460bbb9'}}"}*

```diff
@@ -1,11 +1,11 @@
 {
     "files": {
         "d_417a353b6036f046___init___py": {
-            "hash": "3360c7272c7f978ac5e04a54c9964205",
+            "hash": "ccb563545275a070316909877460bbb9",
             "index": {
                 "html_filename": "d_417a353b6036f046___init___py.html",
                 "nums": [
                     0,
                     1,
                     1,
                     0,
```

### Comparing `par_run-0.1.2/.reports/html/style.css` & `par_run-0.1.3/.reports/html/style.css`

 * *Files identical despite different names*

### Comparing `par_run-0.1.2/.vscode/launch.json` & `par_run-0.1.3/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `par_run-0.1.2/py_tests/conftest.py` & `par_run-0.1.3/py_tests/conftest.py`

 * *Files identical despite different names*

### Comparing `par_run-0.1.2/py_tests/test_cli.py` & `par_run-0.1.3/py_tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `par_run-0.1.2/py_tests/test_executor.py` & `par_run-0.1.3/py_tests/test_executor.py`

 * *Files identical despite different names*

### Comparing `par_run-0.1.2/py_tests/test_web.py` & `par_run-0.1.3/py_tests/test_web.py`

 * *Files identical despite different names*

### Comparing `par_run-0.1.2/src/par_run/cli.py` & `par_run-0.1.3/src/par_run/cli.py`

 * *Files identical despite different names*

### Comparing `par_run-0.1.2/src/par_run/executor.py` & `par_run-0.1.3/src/par_run/executor.py`

 * *Files identical despite different names*

### Comparing `par_run-0.1.2/src/par_run/web.py` & `par_run-0.1.3/src/par_run/web.py`

 * *Files identical despite different names*

### Comparing `par_run-0.1.2/src/par_run/static/css/style.css` & `par_run-0.1.3/src/par_run/static/css/style.css`

 * *Files identical despite different names*

### Comparing `par_run-0.1.2/src/par_run/static/js/app.js` & `par_run-0.1.3/src/par_run/static/js/app.js`

 * *Files identical despite different names*

### Comparing `par_run-0.1.2/src/par_run/templates/index.html` & `par_run-0.1.3/src/par_run/templates/index.html`

 * *Files identical despite different names*

### Comparing `par_run-0.1.2/.gitignore` & `par_run-0.1.3/.gitignore`

 * *Files identical despite different names*

### Comparing `par_run-0.1.2/LICENSE` & `par_run-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `par_run-0.1.2/README.md` & `par_run-0.1.3/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 # par-run
 [![License: MIT](https://img.shields.io/badge/license-MIT-C06524)](https://github.com/nazq/par-run/blob/main/LICENSE)
-![PyPI - Python Version](https://img.shields.io/pypi/pyversions/par-run)
-![Python Version from PEP 621 TOML](https://img.shields.io/python/required-version-toml?tomlFilePath=https://github.com/nazq/par-run/blob/main/pyproject.toml)
-
+[![PyPI version](https://badge.fury.io/py/par-run.svg)](https://badge.fury.io/py/par-run)
+[![Python Versions](https://img.shields.io/pypi/pyversions/par-run)](https://pypi.org/project/par-run/)
 
 Ever needed to run groups of long-ish running commands in parallel groups? Then this is for you. par-run gives both a CLI and web interface to running groups of commands in parallel.  
 
 ## Getting Started
 
 ```shell
 pip install par-run
```

### Comparing `par_run-0.1.2/pyproject.toml` & `par_run-0.1.3/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,23 +1,43 @@
 [project]
 name = "par-run"
-version = "0.1.2"
+version = "0.1.3"
 description = "Parallel command runner"
 license = "MIT"
 authors = [
     { name = "Naz Quadri", email = "naz.quadri@gmail.com" }
 ]
+classifiers = [
+    'Development Status :: 4 - Beta',
+    'Intended Audience :: Developers',
+    'License :: OSI Approved :: MIT License',
+    'Natural Language :: English',
+    'Programming Language :: Python :: 3',
+    'Programming Language :: Python :: 3.7',
+    'Programming Language :: Python :: 3.8',
+    'Programming Language :: Python :: 3.9',
+    'Programming Language :: Python :: 3.10',
+    'Programming Language :: Python :: 3.11',
+    'Programming Language :: Python :: 3.12',
+]
 dependencies = [
     "rich>=13.0.0",
     "typer>=0.9.0",
     "pydantic>=2.0.0",
 ]
 readme = "README.md"
 requires-python = ">= 3.9"
 
+[project.urls]
+Homepage = "https://github.com/nazq/par-run"
+Documentation = "https://github.com/nazq/par-run"
+Repository = "https://github.com/nazq/par-run"
+Issues = "https://github.com/nazq/par-run/issues"
+Changelog = "https://github.com/nazq/par-run"
+
 [project.optional-dependencies]
 web = [
     "fastapi>=0.100.0",
     "uvicorn[standard]>=0.29.0",
     "jinja2>=3.0.0",
     "psutil>=5.9.0",
 ]
@@ -55,15 +75,15 @@
 packages = [
     "src/par_run",
     "static",
     "templates",
 ]
 
 [tool.bumpversion]
-current_version = "0.1.2"
+current_version = "0.1.3"
 commit = true
 tag = true
 tag_name = "{new_version}"
 tag_message = "Version {new_version}"
 message = "Bump version: {current_version} → {new_version}"
 allow_dirty = true
 parse = """(?P<major>\\d+)\\.(?P<minor>\\d+)\\.(?P<patch>\\d+)"""
```

