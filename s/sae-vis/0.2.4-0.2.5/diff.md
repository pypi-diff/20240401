# Comparing `tmp/sae-vis-0.2.4.tar.gz` & `tmp/sae-vis-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sae-vis-0.2.4.tar", last modified: Sun Mar 31 14:47:28 2024, max compression
+gzip compressed data, was "sae-vis-0.2.5.tar", last modified: Mon Apr  1 10:11:25 2024, max compression
```

## Comparing `sae-vis-0.2.4.tar` & `sae-vis-0.2.5.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxrwxrwx   0        0        0        0 2024-03-31 14:47:28.932097 sae-vis-0.2.4/
--rw-rw-rw-   0        0        0       27 2024-02-21 04:51:02.000000 sae-vis-0.2.4/MANIFEST.in
--rw-rw-rw-   0        0        0      361 2024-03-31 14:47:28.932097 sae-vis-0.2.4/PKG-INFO
--rw-rw-rw-   0        0        0     2636 2024-03-29 09:56:38.000000 sae-vis-0.2.4/README.md
-drwxrwxrwx   0        0        0        0 2024-03-31 14:47:28.864236 sae-vis-0.2.4/sae_vis/
--rw-rw-rw-   0        0        0      165 2024-02-21 04:27:15.000000 sae-vis-0.2.4/sae_vis/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-31 14:47:28.905428 sae-vis-0.2.4/sae_vis/__pycache__/
--rw-rw-rw-   0        0        0      373 2024-02-21 16:51:55.000000 sae-vis-0.2.4/sae_vis/__pycache__/__init__.cpython-311.pyc
--rw-rw-rw-   0        0        0    23307 2024-03-30 20:39:51.000000 sae-vis-0.2.4/sae_vis/__pycache__/data_config_classes.cpython-311.pyc
--rw-rw-rw-   0        0        0    48089 2024-03-31 11:17:20.000000 sae-vis-0.2.4/sae_vis/__pycache__/data_fetching_fns.cpython-311.pyc
--rw-rw-rw-   0        0        0    57756 2024-03-30 20:39:51.000000 sae-vis-0.2.4/sae_vis/__pycache__/data_storing_fns.cpython-311.pyc
--rw-rw-rw-   0        0        0    13155 2024-03-30 20:39:51.000000 sae-vis-0.2.4/sae_vis/__pycache__/html_fns.cpython-311.pyc
--rw-rw-rw-   0        0        0    13355 2024-03-30 10:24:03.000000 sae-vis-0.2.4/sae_vis/__pycache__/model_fns.cpython-311.pyc
--rw-rw-rw-   0        0        0    46212 2024-03-31 13:12:51.000000 sae-vis-0.2.4/sae_vis/__pycache__/utils_fns.cpython-311.pyc
-drwxrwxrwx   0        0        0        0 2024-03-31 14:47:28.912645 sae-vis-0.2.4/sae_vis/css/
--rw-rw-rw-   0        0        0      796 2024-03-24 10:41:36.000000 sae-vis-0.2.4/sae_vis/css/dropdown.css
--rw-rw-rw-   0        0        0     1289 2024-03-17 20:10:53.000000 sae-vis-0.2.4/sae_vis/css/general.css
--rw-rw-rw-   0        0        0     1464 2024-03-17 15:54:46.000000 sae-vis-0.2.4/sae_vis/css/sequences.css
--rw-rw-rw-   0        0        0     1671 2024-03-17 18:07:59.000000 sae-vis-0.2.4/sae_vis/css/tables.css
--rw-rw-rw-   0        0        0    17143 2024-03-30 20:16:23.000000 sae-vis-0.2.4/sae_vis/data_config_classes.py
--rw-rw-rw-   0        0        0    47062 2024-03-31 11:16:12.000000 sae-vis-0.2.4/sae_vis/data_fetching_fns.py
--rw-rw-rw-   0        0        0    50059 2024-03-30 20:35:07.000000 sae-vis-0.2.4/sae_vis/data_storing_fns.py
-drwxrwxrwx   0        0        0        0 2024-03-31 14:47:28.920653 sae-vis-0.2.4/sae_vis/html/
--rw-rw-rw-   0        0        0      137 2024-03-17 17:41:09.000000 sae-vis-0.2.4/sae_vis/html/acts_histogram_template.html
--rw-rw-rw-   0        0        0       87 2024-03-17 17:41:07.000000 sae-vis-0.2.4/sae_vis/html/feature_tables_template.html
--rw-rw-rw-   0        0        0      125 2024-03-17 17:40:27.000000 sae-vis-0.2.4/sae_vis/html/logits_histogram_template.html
--rw-rw-rw-   0        0        0       78 2024-03-17 17:40:08.000000 sae-vis-0.2.4/sae_vis/html/logits_table_template.html
--rw-rw-rw-   0        0        0       79 2024-03-17 17:43:18.000000 sae-vis-0.2.4/sae_vis/html/sequences_group_template.html
--rw-rw-rw-   0        0        0    13674 2024-03-30 20:36:44.000000 sae-vis-0.2.4/sae_vis/html_fns.py
-drwxrwxrwx   0        0        0        0 2024-03-31 14:47:28.930903 sae-vis-0.2.4/sae_vis/js/
--rw-rw-rw-   0        0        0     4378 2024-03-24 10:12:02.000000 sae-vis-0.2.4/sae_vis/js/_createDropdownsScript.js
--rw-rw-rw-   0        0        0     3077 2024-03-24 09:43:39.000000 sae-vis-0.2.4/sae_vis/js/actsHistogramScript.js
--rw-rw-rw-   0        0        0     2961 2024-03-17 16:48:44.000000 sae-vis-0.2.4/sae_vis/js/featureTablesScript.js
--rw-rw-rw-   0        0        0      533 2024-03-17 19:15:57.000000 sae-vis-0.2.4/sae_vis/js/gridColumnTitlesScript.js
--rw-rw-rw-   0        0        0     3512 2024-03-24 09:43:08.000000 sae-vis-0.2.4/sae_vis/js/logitsHistogramScript.js
--rw-rw-rw-   0        0        0     2769 2024-03-17 16:48:34.000000 sae-vis-0.2.4/sae_vis/js/logitsTableScript.js
--rw-rw-rw-   0        0        0    10991 2024-03-24 09:55:09.000000 sae-vis-0.2.4/sae_vis/js/tokenScript.js
--rw-rw-rw-   0        0        0     8845 2024-03-30 10:21:52.000000 sae-vis-0.2.4/sae_vis/model_fns.py
--rw-rw-rw-   0        0        0    34976 2024-03-31 13:12:44.000000 sae-vis-0.2.4/sae_vis/utils_fns.py
-drwxrwxrwx   0        0        0        0 2024-03-31 14:47:28.892834 sae-vis-0.2.4/sae_vis.egg-info/
--rw-rw-rw-   0        0        0      361 2024-03-31 14:47:28.000000 sae-vis-0.2.4/sae_vis.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1244 2024-03-31 14:47:28.000000 sae-vis-0.2.4/sae_vis.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-31 14:47:28.000000 sae-vis-0.2.4/sae_vis.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       49 2024-03-31 14:47:28.000000 sae-vis-0.2.4/sae_vis.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-03-31 14:47:28.000000 sae-vis-0.2.4/sae_vis.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-03-31 14:47:28.933097 sae-vis-0.2.4/setup.cfg
--rw-rw-rw-   0        0        0      849 2024-03-31 14:47:26.000000 sae-vis-0.2.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-01 10:11:25.310586 sae-vis-0.2.5/
+-rw-rw-rw-   0        0        0       27 2024-02-21 04:51:02.000000 sae-vis-0.2.5/MANIFEST.in
+-rw-rw-rw-   0        0        0      361 2024-04-01 10:11:25.310586 sae-vis-0.2.5/PKG-INFO
+-rw-rw-rw-   0        0        0     2636 2024-03-29 09:56:38.000000 sae-vis-0.2.5/README.md
+drwxrwxrwx   0        0        0        0 2024-04-01 10:11:25.245586 sae-vis-0.2.5/sae_vis/
+-rw-rw-rw-   0        0        0      165 2024-02-21 04:27:15.000000 sae-vis-0.2.5/sae_vis/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-01 10:11:25.279586 sae-vis-0.2.5/sae_vis/__pycache__/
+-rw-rw-rw-   0        0        0      373 2024-02-21 16:51:55.000000 sae-vis-0.2.5/sae_vis/__pycache__/__init__.cpython-311.pyc
+-rw-rw-rw-   0        0        0    23307 2024-03-30 20:39:51.000000 sae-vis-0.2.5/sae_vis/__pycache__/data_config_classes.cpython-311.pyc
+-rw-rw-rw-   0        0        0    48089 2024-03-31 11:17:20.000000 sae-vis-0.2.5/sae_vis/__pycache__/data_fetching_fns.cpython-311.pyc
+-rw-rw-rw-   0        0        0    57756 2024-03-30 20:39:51.000000 sae-vis-0.2.5/sae_vis/__pycache__/data_storing_fns.cpython-311.pyc
+-rw-rw-rw-   0        0        0    13155 2024-03-30 20:39:51.000000 sae-vis-0.2.5/sae_vis/__pycache__/html_fns.cpython-311.pyc
+-rw-rw-rw-   0        0        0    13355 2024-03-30 10:24:03.000000 sae-vis-0.2.5/sae_vis/__pycache__/model_fns.cpython-311.pyc
+-rw-rw-rw-   0        0        0    46162 2024-03-31 15:33:46.000000 sae-vis-0.2.5/sae_vis/__pycache__/utils_fns.cpython-311.pyc
+drwxrwxrwx   0        0        0        0 2024-04-01 10:11:25.283586 sae-vis-0.2.5/sae_vis/css/
+-rw-rw-rw-   0        0        0      796 2024-03-24 10:41:36.000000 sae-vis-0.2.5/sae_vis/css/dropdown.css
+-rw-rw-rw-   0        0        0     1289 2024-03-17 20:10:53.000000 sae-vis-0.2.5/sae_vis/css/general.css
+-rw-rw-rw-   0        0        0     1464 2024-03-17 15:54:46.000000 sae-vis-0.2.5/sae_vis/css/sequences.css
+-rw-rw-rw-   0        0        0     1671 2024-03-17 18:07:59.000000 sae-vis-0.2.5/sae_vis/css/tables.css
+-rw-rw-rw-   0        0        0    17143 2024-03-30 20:16:23.000000 sae-vis-0.2.5/sae_vis/data_config_classes.py
+-rw-rw-rw-   0        0        0    47062 2024-03-31 11:16:12.000000 sae-vis-0.2.5/sae_vis/data_fetching_fns.py
+-rw-rw-rw-   0        0        0    50059 2024-03-30 20:35:07.000000 sae-vis-0.2.5/sae_vis/data_storing_fns.py
+drwxrwxrwx   0        0        0        0 2024-04-01 10:11:25.290587 sae-vis-0.2.5/sae_vis/html/
+-rw-rw-rw-   0        0        0      137 2024-03-17 17:41:09.000000 sae-vis-0.2.5/sae_vis/html/acts_histogram_template.html
+-rw-rw-rw-   0        0        0       87 2024-03-17 17:41:07.000000 sae-vis-0.2.5/sae_vis/html/feature_tables_template.html
+-rw-rw-rw-   0        0        0      125 2024-03-17 17:40:27.000000 sae-vis-0.2.5/sae_vis/html/logits_histogram_template.html
+-rw-rw-rw-   0        0        0       78 2024-03-17 17:40:08.000000 sae-vis-0.2.5/sae_vis/html/logits_table_template.html
+-rw-rw-rw-   0        0        0       79 2024-03-17 17:43:18.000000 sae-vis-0.2.5/sae_vis/html/sequences_group_template.html
+-rw-rw-rw-   0        0        0    13674 2024-04-01 09:31:33.000000 sae-vis-0.2.5/sae_vis/html_fns.py
+drwxrwxrwx   0        0        0        0 2024-04-01 10:11:25.309586 sae-vis-0.2.5/sae_vis/js/
+-rw-rw-rw-   0        0        0     4378 2024-03-24 10:12:02.000000 sae-vis-0.2.5/sae_vis/js/_createDropdownsScript.js
+-rw-rw-rw-   0        0        0     3077 2024-03-24 09:43:39.000000 sae-vis-0.2.5/sae_vis/js/actsHistogramScript.js
+-rw-rw-rw-   0        0        0     2961 2024-03-17 16:48:44.000000 sae-vis-0.2.5/sae_vis/js/featureTablesScript.js
+-rw-rw-rw-   0        0        0      533 2024-03-17 19:15:57.000000 sae-vis-0.2.5/sae_vis/js/gridColumnTitlesScript.js
+-rw-rw-rw-   0        0        0     3512 2024-03-24 09:43:08.000000 sae-vis-0.2.5/sae_vis/js/logitsHistogramScript.js
+-rw-rw-rw-   0        0        0     2769 2024-03-17 16:48:34.000000 sae-vis-0.2.5/sae_vis/js/logitsTableScript.js
+-rw-rw-rw-   0        0        0    10991 2024-03-24 09:55:09.000000 sae-vis-0.2.5/sae_vis/js/tokenScript.js
+-rw-rw-rw-   0        0        0     8967 2024-04-01 10:10:41.000000 sae-vis-0.2.5/sae_vis/model_fns.py
+-rw-rw-rw-   0        0        0    34980 2024-03-31 15:17:59.000000 sae-vis-0.2.5/sae_vis/utils_fns.py
+drwxrwxrwx   0        0        0        0 2024-04-01 10:11:25.268605 sae-vis-0.2.5/sae_vis.egg-info/
+-rw-rw-rw-   0        0        0      361 2024-04-01 10:11:25.000000 sae-vis-0.2.5/sae_vis.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1244 2024-04-01 10:11:25.000000 sae-vis-0.2.5/sae_vis.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-01 10:11:25.000000 sae-vis-0.2.5/sae_vis.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       49 2024-04-01 10:11:25.000000 sae-vis-0.2.5/sae_vis.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-04-01 10:11:25.000000 sae-vis-0.2.5/sae_vis.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-01 10:11:25.310586 sae-vis-0.2.5/setup.cfg
+-rw-rw-rw-   0        0        0      849 2024-04-01 10:11:14.000000 sae-vis-0.2.5/setup.py
```

### Comparing `sae-vis-0.2.4/README.md` & `sae-vis-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `sae-vis-0.2.4/sae_vis/__pycache__/data_config_classes.cpython-311.pyc` & `sae-vis-0.2.5/sae_vis/__pycache__/data_config_classes.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `sae-vis-0.2.4/sae_vis/__pycache__/data_fetching_fns.cpython-311.pyc` & `sae-vis-0.2.5/sae_vis/__pycache__/data_fetching_fns.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `sae-vis-0.2.4/sae_vis/__pycache__/data_storing_fns.cpython-311.pyc` & `sae-vis-0.2.5/sae_vis/__pycache__/data_storing_fns.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `sae-vis-0.2.4/sae_vis/__pycache__/html_fns.cpython-311.pyc` & `sae-vis-0.2.5/sae_vis/__pycache__/html_fns.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `sae-vis-0.2.4/sae_vis/__pycache__/model_fns.cpython-311.pyc` & `sae-vis-0.2.5/sae_vis/__pycache__/model_fns.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `sae-vis-0.2.4/sae_vis/__pycache__/utils_fns.cpython-311.pyc` & `sae-vis-0.2.5/sae_vis/__pycache__/utils_fns.cpython-311.pyc`

 * *Files 2% similar despite different names*

#### Python bytecode

```diff
@@ -1,10 +1,10 @@
 magic:    0xa70d0d0a
-moddate:  0x4c610966 (Sun Mar 31 13:12:44 2024 UTC)
-files sz: 34976
+moddate:  0xa77e0966 (Sun Mar 31 15:17:59 2024 UTC)
+files sz: 34980
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 13
    flags     : 0
    code
       0x9700640064016c006d015a016d025a026d035a030100640064026c046d
@@ -12,97 +12,97 @@
       0c6d0d5a0d6d0e5a0e6d0f5a0f0100640064036c105a10640064036c115a
       11640064046c116d125a120100640064036c135a14640064056c156d165a
       160100640064066c176d175a170100640064076c186d195a196d1a5a1a01
       00640064086c1b6d1c5a1c0100640064036c1d5a1d640064096c1e6d1e5a
       1e0100640064036c1f5a1f640064036c205a206400640a6c216d225a2201
       000200650f640ba6010000ab0100000000000000005a23640c65116a2400
       000000000000006602640d84045a2565146a2600000000000000005a2765
-      28640e6b02000000005a296489640f652a64106506652b19000000000000
-      0000006604641184055a2c09000900648a64146501651264156602190000
+      28640e6b02000000005a296487640f652a64106506652b19000000000000
+      0000006604641184055a2c09000900648864146501651264156602190000
       000000000000006416652d6417652a64186505652d652d66021900000000
       0000000000640c650265126419660219000000000000000000660a641a84
       055a2e641b652d641c652d640c65026512641c6602190000000000000000
-      006606641d84045a2f0900648b641465016512641e660219000000000000
+      006606641d84045a2f09006489641465016512641e660219000000000000
       0000006416652d641f650565306530660219000000000000000000641865
       05652d652d660219000000000000000000640c6502651264196602190000
-      00000000000000660a642084055a31648c6422652a640c650d652d653265
+      00000000000000660a642084055a31648a6422652a640c650d652d653265
       2d190000000000000000007a0700006701652b6532652b19000000000000
       0000007a0700006602190000000000000000006604642384055a33642464
       256426642764286429642a642b642c642d9c095a34642e642f6430643164
-      32643364349c065a356435643664379c025a3669006534a5016536a50164
-      3864316901a5015a37648d6439652b6422652a640c652b6606643a84055a
-      386439652b640c652b6604643b84045a39650c643c650d652d6532652d19
-      0000000000000000007a0700006701652b6532652b190000000000000000
-      007a070000660219000000000000000000643d652d640c652b6606643e84
-      04a6000000ab0000000000000000005a3a650c643c650d652d6532652d19
-      0000000000000000007a0700006701652b6532652b190000000000000000
-      007a070000660219000000000000000000643d6509652d19000000000000
-      000000640c6509652b190000000000000000006606643f8404a6000000ab
-      0000000000000000005a3a643c650d652d6532652d190000000000000000
-      007a0700006701652b6532652b190000000000000000007a070000660219
-      000000000000000000643d6507652d6509652d1900000000000000000065
-      116a120000000000000000660319000000000000000000640c652b650b7a
-      0700006606644084045a3a02004700644184006442a6020000ab02000000
-      00000000005a3b644384005a3c6444652b640c6505652b652b6602190000
-      000000000000006604644584045a3d0900648e6414650965301900000000
-      00000000006447652d6448650a644919000000000000000000640c650965
-      30190000000000000000006608644a84055a3e644b644c6702644d670264
-      4c644e6702644f6702644e6450670264516702645064526702644f670264
-      5264536702644d670267055a3f644b645067026451670264506452670264
-      4f6702645264536702644d670267035a40651c6519020047006454840064
-      55a6020000ab020000000000000000a6000000ab000000000000000000a6
-      000000ab0000000000000000005a416529900172ae02006525a6000000ab
-      0000000000000000005a2464565a42020065116a43000000000000000002
-      0065116a4400000000000000006542a6010000ab010000000000000000a0
-      450000000000000000000000000000000000000000020065116a44000000
-      00000000006542a6010000ab01000000000000000064576b000000000064
-      4ba6020000ab020000000000000000020065116a44000000000000000065
-      42a6010000ab0100000000000000006702a6010000ab0100000000000000
-      00a04600000000000000000000000000000000000000006524a6010000ab
-      0100000000000000005a476541a048000000000000000000000000000000
-      00000000006547a6010000ab0100000000000000005a490200654a645802
-      00654b6459840065496a4c00000000000000004400a6000000ab00000000
-      0000000000a6010000ab010000000000000000645a9b049d02a6010000ab
-      01000000000000000001000200654a645b6547a04d000000000000000000
-      0000000000000000000000a6000000ab000000000000000000645a9b0464
-      5c9d03a6010000ab0100000000000000000100020065116a4e0000000000
-      0000006700645da2016700645ea2016702a6010000ab0100000000000000
-      00a04600000000000000000000000000000000000000006524a6010000ab
-      0100000000000000005a4f6549a050000000000000000000000000000000
-      0000000000654fa6010000ab0100000000000000005c0200005a515a5202
-      00654a645fa6010000ab010000000000000000010002006553654f640019
-      000000000000000000655164001900000000000000000065526400190000
-      00000000000000a6030000ab03000000000000000044005d235c0300005a
-      545a555a560200654a6460655464619b04646265569b0064636555646465
-      5664657a0a00009b0064669d039b049d06a6010000ab0100000000000000
-      0001008c240200654a6467a6010000ab0100000000000000000100020065
-      53654f646819000000000000000000655164681900000000000000000065
-      52646819000000000000000000a6030000ab03000000000000000044005d
-      235c0300005a545a555a560200654a6460655464619b04646265569b0064
-      6365556464655664657a0a00009b0064669d039b049d06a6010000ab0100
-      0000000000000001008c246469652b646a652b646b652b640c6557652b65
-      2b6602190000000000000000006608646c84045a5865297238646d5a5964
-      6e5a5a646f5a5b0200654a020065586559655a655ba6030000ab03000000
-      0000000000a6010000ab010000000000000000010064705a5964715a5a64
-      725a5b0200654a020065586559655a655ba6030000ab0300000000000000
-      00a6010000ab01000000000000000001000900648c6473652b6474652b64
-      75652a640c652b6608647684055a5c648f6478655d6479655d647a652b64
-      0c655d6608647b84055a5e652972830200655e6468646569016451644f69
-      01a6020000ab0200000000000000006465644f647c9c026b020000000073
-      024a0082010200655e646864656451644f67026901690164686451645164
-      4f670269016901a6020000ab02000000000000000064686451644f670264
-      51644f6702647d9c0269016b020000000073024a0082010200655e641464
-      7e647f64686901690169016414647e64806465690169016901a6020000ab
-      0200000000000000006414647e6468646564819c02690169016b02000000
-      0073024a0082010200655e6414646864656702690164146451644f670269
-      01a6020000ab020000000000000000641467006482a20169016b02000000
-      0073024a00820102004700648384006484a6020000ab0200000000000000
-      005a5f651c651902004700648584006486a6020000ab0200000000000000
-      00a6000000ab000000000000000000a6000000ab0000000000000000005a
-      60648c6487652a640c6530652d7a0700006604648884055a6164035300
+      329c045a356433643464359c025a3669006534a5016536a5016436642f69
+      01a5015a37648b6437652b6422652a640c652b6606643884055a38643765
+      2b640c652b6604643984045a39650c643a650d652d6532652d1900000000
+      00000000007a0700006701652b6532652b190000000000000000007a0700
+      00660219000000000000000000643b652d640c652b6606643c8404a60000
+      00ab0000000000000000005a3a650c643a650d652d6532652d1900000000
+      00000000007a0700006701652b6532652b190000000000000000007a0700
+      00660219000000000000000000643b6509652d1900000000000000000064
+      0c6509652b190000000000000000006606643d8404a6000000ab00000000
+      00000000005a3a643a650d652d6532652d190000000000000000007a0700
+      006701652b6532652b190000000000000000007a07000066021900000000
+      0000000000643b6507652d6509652d1900000000000000000065116a1200
+      00000000000000660319000000000000000000640c652b650b7a07000066
+      06643e84045a3a02004700643f84006440a6020000ab0200000000000000
+      005a3b644184005a3c6442652b640c6505652b652b660219000000000000
+      0000006604644384045a3d0900648c641465096530190000000000000000
+      006445652d6446650a644719000000000000000000640c65096530190000
+      000000000000006608644884055a3e6449644a6702644b6702644a644c67
+      02644d6702644c644e6702644f6702644e64506702644d67026450645167
+      02644b670267055a3f6449644e6702644f6702644e64506702644d670264
+      5064516702644b670267035a40651c651902004700645284006453a60200
+      00ab020000000000000000a6000000ab000000000000000000a6000000ab
+      0000000000000000005a416529900172ae02006525a6000000ab00000000
+      00000000005a2464545a42020065116a430000000000000000020065116a
+      4400000000000000006542a6010000ab010000000000000000a045000000
+      0000000000000000000000000000000000020065116a4400000000000000
+      006542a6010000ab01000000000000000064556b00000000006449a60200
+      00ab020000000000000000020065116a4400000000000000006542a60100
+      00ab0100000000000000006702a6010000ab010000000000000000a04600
+      000000000000000000000000000000000000006524a6010000ab01000000
+      00000000005a476541a04800000000000000000000000000000000000000
+      006547a6010000ab0100000000000000005a490200654a64560200654b64
+      57840065496a4c00000000000000004400a6000000ab0000000000000000
+      00a6010000ab01000000000000000064589b049d02a6010000ab01000000
+      000000000001000200654a64596547a04d00000000000000000000000000
+      00000000000000a6000000ab00000000000000000064589b04645a9d03a6
+      010000ab0100000000000000000100020065116a4e000000000000000067
+      00645ba2016700645ca2016702a6010000ab010000000000000000a04600
+      000000000000000000000000000000000000006524a6010000ab01000000
+      00000000005a4f6549a05000000000000000000000000000000000000000
+      00654fa6010000ab0100000000000000005c0200005a515a520200654a64
+      5da6010000ab010000000000000000010002006553654f64001900000000
+      000000000065516400190000000000000000006552640019000000000000
+      000000a6030000ab03000000000000000044005d235c0300005a545a555a
+      560200654a645e6554645f9b04646065569b00646165556462655664637a
+      0a00009b0064649d039b049d06a6010000ab01000000000000000001008c
+      240200654a6465a6010000ab010000000000000000010002006553654f64
+      661900000000000000000065516466190000000000000000006552646619
+      000000000000000000a6030000ab03000000000000000044005d235c0300
+      005a545a555a560200654a645e6554645f9b04646065569b006461655564
+      62655664637a0a00009b0064649d039b049d06a6010000ab010000000000
+      00000001008c246467652b6468652b6469652b640c6557652b652b660219
+      0000000000000000006608646a84045a5865297238646b5a59646c5a5a64
+      6d5a5b0200654a020065586559655a655ba6030000ab0300000000000000
+      00a6010000ab0100000000000000000100646e5a59646f5a5a64705a5b02
+      00654a020065586559655a655ba6030000ab030000000000000000a60100
+      00ab01000000000000000001000900648a6471652b6472652b6473652a64
+      0c652b6608647484055a5c648d6476655d6477655d6478652b640c655d66
+      08647984055a5e652972830200655e646664636901644f644d6901a60200
+      00ab0200000000000000006463644d647a9c026b020000000073024a0082
+      010200655e64666463644f644d6702690169016466644f644f644d670269
+      016901a6020000ab0200000000000000006466644f644d6702644f644d67
+      02647b9c0269016b020000000073024a0082010200655e6414647c647d64
+      666901690169016414647c647e6463690169016901a6020000ab02000000
+      00000000006414647c64666463647f9c02690169016b020000000073024a
+      0082010200655e641464666463670269016414644f644d67026901a60200
+      00ab020000000000000000641467006480a20169016b020000000073024a
+      00820102004700648184006482a6020000ab0200000000000000005a5f65
+      1c651902004700648384006484a6020000ab020000000000000000a60000
+      00ab000000000000000000a6000000ab0000000000000000005a60648a64
+      85652a640c6530652d7a0700006604648684055a6164035300
      0           0 RESUME                   0
    
      3           2 LOAD_CONST               0 (0)
                  4 LOAD_CONST               1 (('Float', 'Int', 'Bool'))
                  6 IMPORT_NAME              0 (jaxtyping)
                  8 IMPORT_FROM              1 (Float)
                 10 STORE_NAME               1 (Float)
@@ -240,15 +240,15 @@
                266 STORE_NAME              39 (Arr)
    
     44         268 LOAD_NAME               40 (__name__)
                270 LOAD_CONST              14 ('__main__')
                272 COMPARE_OP               2 (==)
                278 STORE_NAME              41 (MAIN)
    
-    48         280 LOAD_CONST             137 ((None,))
+    48         280 LOAD_CONST             135 ((None,))
                282 LOAD_CONST              15 ('verbose')
                284 LOAD_NAME               42 (bool)
                286 LOAD_CONST              16 ('desc')
                288 LOAD_NAME                6 (Optional)
                290 LOAD_NAME               43 (str)
                292 BINARY_SUBSCR
                302 BUILD_TUPLE              4
@@ -256,15 +256,15 @@
                306 MAKE_FUNCTION            5 (defaults, annotations)
                308 STORE_NAME              44 (create_iterator)
    
     59         310 NOP
    
     60         312 NOP
    
-    56         314 LOAD_CONST             138 ((True, (5, -5)))
+    56         314 LOAD_CONST             136 ((True, (5, -5)))
                316 LOAD_CONST              20 ('x')
    
     57         318 LOAD_NAME                1 (Float)
                320 LOAD_NAME               18 (Tensor)
                322 LOAD_CONST              21 ('rows cols')
                324 BUILD_TUPLE              2
                326 BINARY_SUBSCR
@@ -311,15 +311,15 @@
                420 BUILD_TUPLE              6
                422 LOAD_CONST              29 (<code object sample_unique_indices, file "C:\Users\calsm\Documents\AI Alignment\sae-vis\sae_vis\utils_fns.py", line 86>)
                424 MAKE_FUNCTION            4 (annotations)
                426 STORE_NAME              47 (sample_unique_indices)
    
    102         428 NOP
    
-    98         430 LOAD_CONST             139 (((5, -5),))
+    98         430 LOAD_CONST             137 (((5, -5),))
                432 LOAD_CONST              20 ('x')
    
     99         434 LOAD_NAME                1 (Float)
                436 LOAD_NAME               18 (Tensor)
                438 LOAD_CONST              30 ('batch seq')
                440 BUILD_TUPLE              2
                442 BINARY_SUBSCR
@@ -353,15 +353,15 @@
                506 BINARY_SUBSCR
    
     98         516 BUILD_TUPLE             10
                518 LOAD_CONST              32 (<code object random_range_indices, file "C:\Users\calsm\Documents\AI Alignment\sae-vis\sae_vis\utils_fns.py", line 98>)
                520 MAKE_FUNCTION            5 (defaults, annotations)
                522 STORE_NAME              49 (random_range_indices)
    
-   157         524 LOAD_CONST             140 ((False,))
+   157         524 LOAD_CONST             138 ((False,))
                526 LOAD_CONST              34 ('html')
                528 LOAD_NAME               42 (bool)
                530 LOAD_CONST              12 ('return')
                532 LOAD_NAME               13 (Callable)
                534 LOAD_NAME               45 (int)
                536 LOAD_NAME               50 (list)
                538 LOAD_NAME               45 (int)
@@ -398,816 +398,812 @@
    
    193         612 LOAD_CONST              44 ('&#125;')
    
    184         614 LOAD_CONST              45 (('\\', '<', '>', ')', '(', '[', ']', '{', '}'))
                616 BUILD_CONST_KEY_MAP      9
                618 STORE_NAME              52 (HTML_CHARS)
    
-   196         620 LOAD_CONST              46 ('&ndash;')
+   198         620 LOAD_CONST              46 ('&#8203;')
    
-   197         622 LOAD_CONST              47 ('&rsquo;')
+   199         622 LOAD_CONST              47 ('&nbsp;')
    
-   198         624 LOAD_CONST              48 ('&#8203;')
+   200         624 LOAD_CONST              48 ('&bsol;n')
    
-   199         626 LOAD_CONST              49 ('&nbsp;')
+   201         626 LOAD_CONST              49 ('&bsol;t')
    
-   200         628 LOAD_CONST              50 ('&bsol;n')
+   195         628 LOAD_CONST              50 (('âĢĭ', 'Ġ', 'Ċ', 'ĉ'))
+               630 BUILD_CONST_KEY_MAP      4
+               632 STORE_NAME              53 (HTML_ANOMALIES)
    
-   201         630 LOAD_CONST              51 ('&bsol;t')
+   204         634 LOAD_CONST              51 ('&apos;')
    
-   195         632 LOAD_CONST              52 (('âĢĶ', 'âĢĻ', 'âĢĭ', 'Ġ', 'Ċ', 'ĉ'))
-               634 BUILD_CONST_KEY_MAP      6
-               636 STORE_NAME              53 (HTML_ANOMALIES)
+   205         636 LOAD_CONST              52 ('&quot;')
    
-   204         638 LOAD_CONST              53 ('&apos;')
+   203         638 LOAD_CONST              53 (("'", '"'))
+               640 BUILD_CONST_KEY_MAP      2
+               642 STORE_NAME              54 (HTML_QUOTES)
    
-   205         640 LOAD_CONST              54 ('&quot;')
-   
-   203         642 LOAD_CONST              55 (("'", '"'))
-               644 BUILD_CONST_KEY_MAP      2
-               646 STORE_NAME              54 (HTML_QUOTES)
-   
-   207         648 BUILD_MAP                0
-               650 LOAD_NAME               52 (HTML_CHARS)
+   207         644 BUILD_MAP                0
+               646 LOAD_NAME               52 (HTML_CHARS)
+               648 DICT_UPDATE              1
+               650 LOAD_NAME               54 (HTML_QUOTES)
                652 DICT_UPDATE              1
-               654 LOAD_NAME               54 (HTML_QUOTES)
-               656 DICT_UPDATE              1
-               658 LOAD_CONST              56 (' ')
-               660 LOAD_CONST              49 ('&nbsp;')
-               662 BUILD_MAP                1
-               664 DICT_UPDATE              1
-               666 STORE_NAME              55 (HTML_ALL)
-   
-   209         668 LOAD_CONST             141 ((True,))
-               670 LOAD_CONST              57 ('str_tok')
-               672 LOAD_NAME               43 (str)
-               674 LOAD_CONST              34 ('html')
-               676 LOAD_NAME               42 (bool)
-               678 LOAD_CONST              12 ('return')
-               680 LOAD_NAME               43 (str)
-               682 BUILD_TUPLE              6
-               684 LOAD_CONST              58 (<code object process_str_tok, file "C:\Users\calsm\Documents\AI Alignment\sae-vis\sae_vis\utils_fns.py", line 209>)
-               686 MAKE_FUNCTION            5 (defaults, annotations)
-               688 STORE_NAME              56 (process_str_tok)
-   
-   238         690 LOAD_CONST              57 ('str_tok')
+               654 LOAD_CONST              54 (' ')
+               656 LOAD_CONST              47 ('&nbsp;')
+               658 BUILD_MAP                1
+               660 DICT_UPDATE              1
+               662 STORE_NAME              55 (HTML_ALL)
+   
+   209         664 LOAD_CONST             139 ((True,))
+               666 LOAD_CONST              55 ('str_tok')
+               668 LOAD_NAME               43 (str)
+               670 LOAD_CONST              34 ('html')
+               672 LOAD_NAME               42 (bool)
+               674 LOAD_CONST              12 ('return')
+               676 LOAD_NAME               43 (str)
+               678 BUILD_TUPLE              6
+               680 LOAD_CONST              56 (<code object process_str_tok, file "C:\Users\calsm\Documents\AI Alignment\sae-vis\sae_vis\utils_fns.py", line 209>)
+               682 MAKE_FUNCTION            5 (defaults, annotations)
+               684 STORE_NAME              56 (process_str_tok)
+   
+   238         686 LOAD_CONST              55 ('str_tok')
+               688 LOAD_NAME               43 (str)
+               690 LOAD_CONST              12 ('return')
                692 LOAD_NAME               43 (str)
-               694 LOAD_CONST              12 ('return')
-               696 LOAD_NAME               43 (str)
-               698 BUILD_TUPLE              4
-               700 LOAD_CONST              59 (<code object unprocess_str_tok, file "C:\Users\calsm\Documents\AI Alignment\sae-vis\sae_vis\utils_fns.py", line 238>)
-               702 MAKE_FUNCTION            4 (annotations)
-               704 STORE_NAME              57 (unprocess_str_tok)
-   
-   252         706 LOAD_NAME               12 (overload)
-   
-   253         708 LOAD_CONST              60 ('decode_fn')
-   
-   254         710 LOAD_NAME               13 (Callable)
+               694 BUILD_TUPLE              4
+               696 LOAD_CONST              57 (<code object unprocess_str_tok, file "C:\Users\calsm\Documents\AI Alignment\sae-vis\sae_vis\utils_fns.py", line 238>)
+               698 MAKE_FUNCTION            4 (annotations)
+               700 STORE_NAME              57 (unprocess_str_tok)
+   
+   252         702 LOAD_NAME               12 (overload)
+   
+   253         704 LOAD_CONST              58 ('decode_fn')
+   
+   254         706 LOAD_NAME               13 (Callable)
+               708 LOAD_NAME               45 (int)
+               710 LOAD_NAME               50 (list)
                712 LOAD_NAME               45 (int)
-               714 LOAD_NAME               50 (list)
-               716 LOAD_NAME               45 (int)
-               718 BINARY_SUBSCR
-               728 BINARY_OP                7 (|)
-               732 BUILD_LIST               1
+               714 BINARY_SUBSCR
+               724 BINARY_OP                7 (|)
+               728 BUILD_LIST               1
+               730 LOAD_NAME               43 (str)
+               732 LOAD_NAME               50 (list)
                734 LOAD_NAME               43 (str)
-               736 LOAD_NAME               50 (list)
-               738 LOAD_NAME               43 (str)
-               740 BINARY_SUBSCR
-               750 BINARY_OP                7 (|)
-               754 BUILD_TUPLE              2
-               756 BINARY_SUBSCR
+               736 BINARY_SUBSCR
+               746 BINARY_OP                7 (|)
+               750 BUILD_TUPLE              2
+               752 BINARY_SUBSCR
    
-   253         766 LOAD_CONST              61 ('tokens')
+   253         762 LOAD_CONST              59 ('tokens')
    
-   255         768 LOAD_NAME               45 (int)
+   255         764 LOAD_NAME               45 (int)
    
-   253         770 LOAD_CONST              12 ('return')
+   253         766 LOAD_CONST              12 ('return')
    
-   256         772 LOAD_NAME               43 (str)
+   256         768 LOAD_NAME               43 (str)
    
-   253         774 BUILD_TUPLE              6
-               776 LOAD_CONST              62 (<code object to_str_tokens, file "C:\Users\calsm\Documents\AI Alignment\sae-vis\sae_vis\utils_fns.py", line 252>)
-               778 MAKE_FUNCTION            4 (annotations)
+   253         770 BUILD_TUPLE              6
+               772 LOAD_CONST              60 (<code object to_str_tokens, file "C:\Users\calsm\Documents\AI Alignment\sae-vis\sae_vis\utils_fns.py", line 252>)
+               774 MAKE_FUNCTION            4 (annotations)
    
-   252         780 PRECALL                  0
-               784 CALL                     0
+   252         776 PRECALL                  0
+               780 CALL                     0
    
-   253         794 STORE_NAME              58 (to_str_tokens)
+   253         790 STORE_NAME              58 (to_str_tokens)
    
-   259         796 LOAD_NAME               12 (overload)
+   259         792 LOAD_NAME               12 (overload)
    
-   260         798 LOAD_CONST              60 ('decode_fn')
+   260         794 LOAD_CONST              58 ('decode_fn')
    
-   261         800 LOAD_NAME               13 (Callable)
+   261         796 LOAD_NAME               13 (Callable)
+               798 LOAD_NAME               45 (int)
+               800 LOAD_NAME               50 (list)
                802 LOAD_NAME               45 (int)
-               804 LOAD_NAME               50 (list)
-               806 LOAD_NAME               45 (int)
-               808 BINARY_SUBSCR
-               818 BINARY_OP                7 (|)
-               822 BUILD_LIST               1
+               804 BINARY_SUBSCR
+               814 BINARY_OP                7 (|)
+               818 BUILD_LIST               1
+               820 LOAD_NAME               43 (str)
+               822 LOAD_NAME               50 (list)
                824 LOAD_NAME               43 (str)
-               826 LOAD_NAME               50 (list)
-               828 LOAD_NAME               43 (str)
-               830 BINARY_SUBSCR
-               840 BINARY_OP                7 (|)
-               844 BUILD_TUPLE              2
-               846 BINARY_SUBSCR
+               826 BINARY_SUBSCR
+               836 BINARY_OP                7 (|)
+               840 BUILD_TUPLE              2
+               842 BINARY_SUBSCR
    
-   260         856 LOAD_CONST              61 ('tokens')
+   260         852 LOAD_CONST              59 ('tokens')
    
-   262         858 LOAD_NAME                9 (List)
-               860 LOAD_NAME               45 (int)
-               862 BINARY_SUBSCR
+   262         854 LOAD_NAME                9 (List)
+               856 LOAD_NAME               45 (int)
+               858 BINARY_SUBSCR
    
-   260         872 LOAD_CONST              12 ('return')
+   260         868 LOAD_CONST              12 ('return')
    
-   263         874 LOAD_NAME                9 (List)
-               876 LOAD_NAME               43 (str)
-               878 BINARY_SUBSCR
+   263         870 LOAD_NAME                9 (List)
+               872 LOAD_NAME               43 (str)
+               874 BINARY_SUBSCR
    
-   260         888 BUILD_TUPLE              6
-               890 LOAD_CONST              63 (<code object to_str_tokens, file "C:\Users\calsm\Documents\AI Alignment\sae-vis\sae_vis\utils_fns.py", line 259>)
-               892 MAKE_FUNCTION            4 (annotations)
+   260         884 BUILD_TUPLE              6
+               886 LOAD_CONST              61 (<code object to_str_tokens, file "C:\Users\calsm\Documents\AI Alignment\sae-vis\sae_vis\utils_fns.py", line 259>)
+               888 MAKE_FUNCTION            4 (annotations)
    
-   259         894 PRECALL                  0
-               898 CALL                     0
+   259         890 PRECALL                  0
+               894 CALL                     0
    
-   260         908 STORE_NAME              58 (to_str_tokens)
+   260         904 STORE_NAME              58 (to_str_tokens)
    
-   266         910 LOAD_CONST              60 ('decode_fn')
+   266         906 LOAD_CONST              58 ('decode_fn')
    
-   267         912 LOAD_NAME               13 (Callable)
+   267         908 LOAD_NAME               13 (Callable)
+               910 LOAD_NAME               45 (int)
+               912 LOAD_NAME               50 (list)
                914 LOAD_NAME               45 (int)
-               916 LOAD_NAME               50 (list)
-               918 LOAD_NAME               45 (int)
-               920 BINARY_SUBSCR
-               930 BINARY_OP                7 (|)
-               934 BUILD_LIST               1
+               916 BINARY_SUBSCR
+               926 BINARY_OP                7 (|)
+               930 BUILD_LIST               1
+               932 LOAD_NAME               43 (str)
+               934 LOAD_NAME               50 (list)
                936 LOAD_NAME               43 (str)
-               938 LOAD_NAME               50 (list)
-               940 LOAD_NAME               43 (str)
-               942 BINARY_SUBSCR
-               952 BINARY_OP                7 (|)
-               956 BUILD_TUPLE              2
-               958 BINARY_SUBSCR
-   
-   266         968 LOAD_CONST              61 ('tokens')
-   
-   268         970 LOAD_NAME                7 (Union)
+               938 BINARY_SUBSCR
+               948 BINARY_OP                7 (|)
+               952 BUILD_TUPLE              2
+               954 BINARY_SUBSCR
+   
+   266         964 LOAD_CONST              59 ('tokens')
+   
+   268         966 LOAD_NAME                7 (Union)
+               968 LOAD_NAME               45 (int)
+               970 LOAD_NAME                9 (List)
                972 LOAD_NAME               45 (int)
-               974 LOAD_NAME                9 (List)
-               976 LOAD_NAME               45 (int)
-               978 BINARY_SUBSCR
-               988 LOAD_NAME               17 (torch)
-               990 LOAD_ATTR               18 (Tensor)
-              1000 BUILD_TUPLE              3
-              1002 BINARY_SUBSCR
-   
-   266        1012 LOAD_CONST              12 ('return')
-   
-   269        1014 LOAD_NAME               43 (str)
-              1016 LOAD_NAME               11 (Any)
-              1018 BINARY_OP                7 (|)
-   
-   266        1022 BUILD_TUPLE              6
-              1024 LOAD_CONST              64 (<code object to_str_tokens, file "C:\Users\calsm\Documents\AI Alignment\sae-vis\sae_vis\utils_fns.py", line 266>)
-              1026 MAKE_FUNCTION            4 (annotations)
-              1028 STORE_NAME              58 (to_str_tokens)
-   
-   290        1030 PUSH_NULL
-              1032 LOAD_BUILD_CLASS
-              1034 LOAD_CONST              65 (<code object TopK, file "C:\Users\calsm\Documents\AI Alignment\sae-vis\sae_vis\utils_fns.py", line 290>)
-              1036 MAKE_FUNCTION            0
-              1038 LOAD_CONST              66 ('TopK')
-              1040 PRECALL                  2
-              1044 CALL                     2
-              1054 STORE_NAME              59 (TopK)
-   
-   366        1056 LOAD_CONST              67 (<code object merge_lists, file "C:\Users\calsm\Documents\AI Alignment\sae-vis\sae_vis\utils_fns.py", line 366>)
-              1058 MAKE_FUNCTION            0
-              1060 STORE_NAME              60 (merge_lists)
-   
-   374        1062 LOAD_CONST              68 ('html_content')
-              1064 LOAD_NAME               43 (str)
-              1066 LOAD_CONST              12 ('return')
-              1068 LOAD_NAME                5 (Tuple)
-              1070 LOAD_NAME               43 (str)
-              1072 LOAD_NAME               43 (str)
-              1074 BUILD_TUPLE              2
-              1076 BINARY_SUBSCR
-              1086 BUILD_TUPLE              4
-              1088 LOAD_CONST              69 (<code object extract_and_remove_scripts, file "C:\Users\calsm\Documents\AI Alignment\sae-vis\sae_vis\utils_fns.py", line 374>)
-              1090 MAKE_FUNCTION            4 (annotations)
-              1092 STORE_NAME              61 (extract_and_remove_scripts)
-   
-   398        1094 NOP
-   
-   395        1096 LOAD_CONST             142 (('left',))
-              1098 LOAD_CONST              20 ('x')
-   
-   396        1100 LOAD_NAME                9 (List)
-              1102 LOAD_NAME               48 (float)
-              1104 BINARY_SUBSCR
-   
-   395        1114 LOAD_CONST              71 ('n')
-   
-   397        1116 LOAD_NAME               45 (int)
-   
-   395        1118 LOAD_CONST              72 ('side')
-   
-   398        1120 LOAD_NAME               10 (Literal)
-              1122 LOAD_CONST              73 (('left', 'right'))
-              1124 BINARY_SUBSCR
-   
-   395        1134 LOAD_CONST              12 ('return')
-   
-   399        1136 LOAD_NAME                9 (List)
-              1138 LOAD_NAME               48 (float)
-              1140 BINARY_SUBSCR
-   
-   395        1150 BUILD_TUPLE              8
-              1152 LOAD_CONST              74 (<code object pad_with_zeros, file "C:\Users\calsm\Documents\AI Alignment\sae-vis\sae_vis\utils_fns.py", line 395>)
-              1154 MAKE_FUNCTION            5 (defaults, annotations)
-              1156 STORE_NAME              62 (pad_with_zeros)
-   
-   417        1158 LOAD_CONST              75 (0.0)
-              1160 LOAD_CONST              76 (0.01)
+               974 BINARY_SUBSCR
+               984 LOAD_NAME               17 (torch)
+               986 LOAD_ATTR               18 (Tensor)
+               996 BUILD_TUPLE              3
+               998 BINARY_SUBSCR
+   
+   266        1008 LOAD_CONST              12 ('return')
+   
+   269        1010 LOAD_NAME               43 (str)
+              1012 LOAD_NAME               11 (Any)
+              1014 BINARY_OP                7 (|)
+   
+   266        1018 BUILD_TUPLE              6
+              1020 LOAD_CONST              62 (<code object to_str_tokens, file "C:\Users\calsm\Documents\AI Alignment\sae-vis\sae_vis\utils_fns.py", line 266>)
+              1022 MAKE_FUNCTION            4 (annotations)
+              1024 STORE_NAME              58 (to_str_tokens)
+   
+   290        1026 PUSH_NULL
+              1028 LOAD_BUILD_CLASS
+              1030 LOAD_CONST              63 (<code object TopK, file "C:\Users\calsm\Documents\AI Alignment\sae-vis\sae_vis\utils_fns.py", line 290>)
+              1032 MAKE_FUNCTION            0
+              1034 LOAD_CONST              64 ('TopK')
+              1036 PRECALL                  2
+              1040 CALL                     2
+              1050 STORE_NAME              59 (TopK)
+   
+   366        1052 LOAD_CONST              65 (<code object merge_lists, file "C:\Users\calsm\Documents\AI Alignment\sae-vis\sae_vis\utils_fns.py", line 366>)
+              1054 MAKE_FUNCTION            0
+              1056 STORE_NAME              60 (merge_lists)
+   
+   374        1058 LOAD_CONST              66 ('html_content')
+              1060 LOAD_NAME               43 (str)
+              1062 LOAD_CONST              12 ('return')
+              1064 LOAD_NAME                5 (Tuple)
+              1066 LOAD_NAME               43 (str)
+              1068 LOAD_NAME               43 (str)
+              1070 BUILD_TUPLE              2
+              1072 BINARY_SUBSCR
+              1082 BUILD_TUPLE              4
+              1084 LOAD_CONST              67 (<code object extract_and_remove_scripts, file "C:\Users\calsm\Documents\AI Alignment\sae-vis\sae_vis\utils_fns.py", line 374>)
+              1086 MAKE_FUNCTION            4 (annotations)
+              1088 STORE_NAME              61 (extract_and_remove_scripts)
+   
+   398        1090 NOP
+   
+   395        1092 LOAD_CONST             140 (('left',))
+              1094 LOAD_CONST              20 ('x')
+   
+   396        1096 LOAD_NAME                9 (List)
+              1098 LOAD_NAME               48 (float)
+              1100 BINARY_SUBSCR
+   
+   395        1110 LOAD_CONST              69 ('n')
+   
+   397        1112 LOAD_NAME               45 (int)
+   
+   395        1114 LOAD_CONST              70 ('side')
+   
+   398        1116 LOAD_NAME               10 (Literal)
+              1118 LOAD_CONST              71 (('left', 'right'))
+              1120 BINARY_SUBSCR
+   
+   395        1130 LOAD_CONST              12 ('return')
+   
+   399        1132 LOAD_NAME                9 (List)
+              1134 LOAD_NAME               48 (float)
+              1136 BINARY_SUBSCR
+   
+   395        1146 BUILD_TUPLE              8
+              1148 LOAD_CONST              72 (<code object pad_with_zeros, file "C:\Users\calsm\Documents\AI Alignment\sae-vis\sae_vis\utils_fns.py", line 395>)
+              1150 MAKE_FUNCTION            5 (defaults, annotations)
+              1152 STORE_NAME              62 (pad_with_zeros)
+   
+   417        1154 LOAD_CONST              73 (0.0)
+              1156 LOAD_CONST              74 (0.01)
+              1158 BUILD_LIST               2
+              1160 LOAD_CONST              75 (5)
               1162 BUILD_LIST               2
-              1164 LOAD_CONST              77 (5)
-              1166 BUILD_LIST               2
    
-   418        1168 LOAD_CONST              76 (0.01)
-              1170 LOAD_CONST              78 (0.05)
+   418        1164 LOAD_CONST              74 (0.01)
+              1166 LOAD_CONST              76 (0.05)
+              1168 BUILD_LIST               2
+              1170 LOAD_CONST              77 (4)
               1172 BUILD_LIST               2
-              1174 LOAD_CONST              79 (4)
-              1176 BUILD_LIST               2
    
-   419        1178 LOAD_CONST              78 (0.05)
-              1180 LOAD_CONST              80 (0.95)
+   419        1174 LOAD_CONST              76 (0.05)
+              1176 LOAD_CONST              78 (0.95)
+              1178 BUILD_LIST               2
+              1180 LOAD_CONST              79 (3)
               1182 BUILD_LIST               2
-              1184 LOAD_CONST              81 (3)
-              1186 BUILD_LIST               2
    
-   420        1188 LOAD_CONST              80 (0.95)
-              1190 LOAD_CONST              82 (0.99)
+   420        1184 LOAD_CONST              78 (0.95)
+              1186 LOAD_CONST              80 (0.99)
+              1188 BUILD_LIST               2
+              1190 LOAD_CONST              77 (4)
               1192 BUILD_LIST               2
-              1194 LOAD_CONST              79 (4)
-              1196 BUILD_LIST               2
    
-   421        1198 LOAD_CONST              82 (0.99)
-              1200 LOAD_CONST              83 (1.0)
+   421        1194 LOAD_CONST              80 (0.99)
+              1196 LOAD_CONST              81 (1.0)
+              1198 BUILD_LIST               2
+              1200 LOAD_CONST              75 (5)
               1202 BUILD_LIST               2
-              1204 LOAD_CONST              77 (5)
-              1206 BUILD_LIST               2
    
-   416        1208 BUILD_LIST               5
-              1210 STORE_NAME              63 (SYMMETRIC_RANGES_AND_PRECISIONS)
+   416        1204 BUILD_LIST               5
+              1206 STORE_NAME              63 (SYMMETRIC_RANGES_AND_PRECISIONS)
    
-   424        1212 LOAD_CONST              75 (0.0)
-              1214 LOAD_CONST              80 (0.95)
+   424        1208 LOAD_CONST              73 (0.0)
+              1210 LOAD_CONST              78 (0.95)
+              1212 BUILD_LIST               2
+              1214 LOAD_CONST              79 (3)
               1216 BUILD_LIST               2
-              1218 LOAD_CONST              81 (3)
-              1220 BUILD_LIST               2
    
-   425        1222 LOAD_CONST              80 (0.95)
-              1224 LOAD_CONST              82 (0.99)
+   425        1218 LOAD_CONST              78 (0.95)
+              1220 LOAD_CONST              80 (0.99)
+              1222 BUILD_LIST               2
+              1224 LOAD_CONST              77 (4)
               1226 BUILD_LIST               2
-              1228 LOAD_CONST              79 (4)
-              1230 BUILD_LIST               2
    
-   426        1232 LOAD_CONST              82 (0.99)
-              1234 LOAD_CONST              83 (1.0)
+   426        1228 LOAD_CONST              80 (0.99)
+              1230 LOAD_CONST              81 (1.0)
+              1232 BUILD_LIST               2
+              1234 LOAD_CONST              75 (5)
               1236 BUILD_LIST               2
-              1238 LOAD_CONST              77 (5)
-              1240 BUILD_LIST               2
    
-   423        1242 BUILD_LIST               3
-              1244 STORE_NAME              64 (ASYMMETRIC_RANGES_AND_PRECISIONS)
+   423        1238 BUILD_LIST               3
+              1240 STORE_NAME              64 (ASYMMETRIC_RANGES_AND_PRECISIONS)
    
-   430        1246 LOAD_NAME               28 (dataclass_json)
+   430        1242 LOAD_NAME               28 (dataclass_json)
    
-   431        1248 LOAD_NAME               25 (dataclass)
-   
-   432        1250 PUSH_NULL
-              1252 LOAD_BUILD_CLASS
-              1254 LOAD_CONST              84 (<code object QuantileCalculator, file "C:\Users\calsm\Documents\AI Alignment\sae-vis\sae_vis\utils_fns.py", line 430>)
-              1256 MAKE_FUNCTION            0
-              1258 LOAD_CONST              85 ('QuantileCalculator')
-              1260 PRECALL                  2
-              1264 CALL                     2
-   
-   431        1274 PRECALL                  0
-              1278 CALL                     0
-   
-   430        1288 PRECALL                  0
-              1292 CALL                     0
-   
-   432        1302 STORE_NAME              65 (QuantileCalculator)
-   
-   556        1304 LOAD_NAME               41 (MAIN)
-              1306 EXTENDED_ARG             1
-              1308 POP_JUMP_FORWARD_IF_FALSE   430 (to 2170)
-   
-   559        1310 PUSH_NULL
-              1312 LOAD_NAME               37 (get_device)
-              1314 PRECALL                  0
-              1318 CALL                     0
-              1328 STORE_NAME              36 (device)
-   
-   560        1330 LOAD_CONST              86 (100000)
-              1332 STORE_NAME              66 (N)
-   
-   561        1334 PUSH_NULL
-              1336 LOAD_NAME               17 (torch)
-              1338 LOAD_ATTR               67 (stack)
-              1348 PUSH_NULL
-              1350 LOAD_NAME               17 (torch)
-              1352 LOAD_ATTR               68 (rand)
-              1362 LOAD_NAME               66 (N)
-              1364 PRECALL                  1
-              1368 CALL                     1
-              1378 LOAD_METHOD             69 (masked_fill)
-              1400 PUSH_NULL
-              1402 LOAD_NAME               17 (torch)
-              1404 LOAD_ATTR               68 (rand)
-              1414 LOAD_NAME               66 (N)
-              1416 PRECALL                  1
-              1420 CALL                     1
-              1430 LOAD_CONST              87 (0.5)
-              1432 COMPARE_OP               0 (<)
-              1438 LOAD_CONST              75 (0.0)
-              1440 PRECALL                  2
-              1444 CALL                     2
-              1454 PUSH_NULL
-              1456 LOAD_NAME               17 (torch)
-              1458 LOAD_ATTR               68 (rand)
-              1468 LOAD_NAME               66 (N)
-              1470 PRECALL                  1
-              1474 CALL                     1
-              1484 BUILD_LIST               2
-              1486 PRECALL                  1
-              1490 CALL                     1
-              1500 LOAD_METHOD             70 (to)
-              1522 LOAD_NAME               36 (device)
-              1524 PRECALL                  1
-              1528 CALL                     1
-              1538 STORE_NAME              71 (data)
-   
-   562        1540 LOAD_NAME               65 (QuantileCalculator)
-              1542 LOAD_METHOD             72 (from_data)
-              1564 LOAD_NAME               71 (data)
-              1566 PRECALL                  1
-              1570 CALL                     1
-              1580 STORE_NAME              73 (qc)
-   
-   563        1582 PUSH_NULL
-              1584 LOAD_NAME               74 (print)
-              1586 LOAD_CONST              88 ('Total datapoints stored = ')
-              1588 PUSH_NULL
-              1590 LOAD_NAME               75 (sum)
-              1592 LOAD_CONST              89 (<code object <genexpr>, file "C:\Users\calsm\Documents\AI Alignment\sae-vis\sae_vis\utils_fns.py", line 563>)
-              1594 MAKE_FUNCTION            0
-              1596 LOAD_NAME               73 (qc)
-              1598 LOAD_ATTR               76 (quantile_data)
-              1608 GET_ITER
-              1610 PRECALL                  0
-              1614 CALL                     0
-              1624 PRECALL                  1
-              1628 CALL                     1
-              1638 LOAD_CONST              90 ('_')
-              1640 FORMAT_VALUE             4 (with format)
-              1642 BUILD_STRING             2
-              1644 PRECALL                  1
-              1648 CALL                     1
-              1658 POP_TOP
-   
-   564        1660 PUSH_NULL
-              1662 LOAD_NAME               74 (print)
-              1664 LOAD_CONST              91 ('Total datapoints used to compute quantiles = ')
-              1666 LOAD_NAME               71 (data)
-              1668 LOAD_METHOD             77 (numel)
-              1690 PRECALL                  0
-              1694 CALL                     0
-              1704 LOAD_CONST              90 ('_')
-              1706 FORMAT_VALUE             4 (with format)
-              1708 LOAD_CONST              92 ('\n')
-              1710 BUILD_STRING             3
-              1712 PRECALL                  1
-              1716 CALL                     1
-              1726 POP_TOP
-   
-   567        1728 PUSH_NULL
-              1730 LOAD_NAME               17 (torch)
-              1732 LOAD_ATTR               78 (tensor)
-              1742 BUILD_LIST               0
-              1744 LOAD_CONST              93 ((0.0, 0.005, 0.02, 0.25))
-              1746 LIST_EXTEND              1
-              1748 BUILD_LIST               0
-              1750 LOAD_CONST              94 ((0.75, 0.98, 0.995, 1.0))
-              1752 LIST_EXTEND              1
-              1754 BUILD_LIST               2
-              1756 PRECALL                  1
-              1760 CALL                     1
-              1770 LOAD_METHOD             70 (to)
-              1792 LOAD_NAME               36 (device)
-              1794 PRECALL                  1
-              1798 CALL                     1
-              1808 STORE_NAME              79 (values)
-   
-   568        1810 LOAD_NAME               73 (qc)
-              1812 LOAD_METHOD             80 (get_quantile)
-              1834 LOAD_NAME               79 (values)
-              1836 PRECALL                  1
-              1840 CALL                     1
-              1850 UNPACK_SEQUENCE          2
-              1854 STORE_NAME              81 (quantiles)
-              1856 STORE_NAME              82 (precisions)
-   
-   570        1858 PUSH_NULL
-              1860 LOAD_NAME               74 (print)
-              1862 LOAD_CONST              95 ('When 50% of data is 0, and 50% is Unif[0, 1]')
-              1864 PRECALL                  1
-              1868 CALL                     1
-              1878 POP_TOP
-   
-   571        1880 PUSH_NULL
-              1882 LOAD_NAME               83 (zip)
-              1884 LOAD_NAME               79 (values)
-              1886 LOAD_CONST               0 (0)
-              1888 BINARY_SUBSCR
-              1898 LOAD_NAME               81 (quantiles)
-              1900 LOAD_CONST               0 (0)
-              1902 BINARY_SUBSCR
-              1912 LOAD_NAME               82 (precisions)
-              1914 LOAD_CONST               0 (0)
-              1916 BINARY_SUBSCR
-              1926 PRECALL                  3
-              1930 CALL                     3
-              1940 GET_ITER
-           >> 1942 FOR_ITER                35 (to 2014)
-              1944 UNPACK_SEQUENCE          3
-              1948 STORE_NAME              84 (v)
-              1950 STORE_NAME              85 (q)
-              1952 STORE_NAME              86 (p)
-   
-   572        1954 PUSH_NULL
-              1956 LOAD_NAME               74 (print)
-              1958 LOAD_CONST              96 ('Value: ')
-              1960 LOAD_NAME               84 (v)
-              1962 LOAD_CONST              97 ('.3f')
-              1964 FORMAT_VALUE             4 (with format)
-              1966 LOAD_CONST              98 (', Precision: ')
-              1968 LOAD_NAME               86 (p)
-              1970 FORMAT_VALUE             0
-              1972 LOAD_CONST              99 (', Quantile: ')
-              1974 LOAD_NAME               85 (q)
-              1976 LOAD_CONST             100 ('.')
-              1978 LOAD_NAME               86 (p)
-              1980 LOAD_CONST             101 (2)
-              1982 BINARY_OP               10 (-)
-              1986 FORMAT_VALUE             0
-              1988 LOAD_CONST             102 ('%')
-              1990 BUILD_STRING             3
-              1992 FORMAT_VALUE             4 (with format)
-              1994 BUILD_STRING             6
-              1996 PRECALL                  1
-              2000 CALL                     1
-              2010 POP_TOP
-              2012 JUMP_BACKWARD           36 (to 1942)
-   
-   573     >> 2014 PUSH_NULL
-              2016 LOAD_NAME               74 (print)
-              2018 LOAD_CONST             103 ('\nWhen 100% of data is Unif[0, 1]')
-              2020 PRECALL                  1
-              2024 CALL                     1
-              2034 POP_TOP
-   
-   574        2036 PUSH_NULL
-              2038 LOAD_NAME               83 (zip)
-              2040 LOAD_NAME               79 (values)
-              2042 LOAD_CONST             104 (1)
-              2044 BINARY_SUBSCR
-              2054 LOAD_NAME               81 (quantiles)
-              2056 LOAD_CONST             104 (1)
-              2058 BINARY_SUBSCR
-              2068 LOAD_NAME               82 (precisions)
-              2070 LOAD_CONST             104 (1)
-              2072 BINARY_SUBSCR
-              2082 PRECALL                  3
-              2086 CALL                     3
-              2096 GET_ITER
-           >> 2098 FOR_ITER                35 (to 2170)
-              2100 UNPACK_SEQUENCE          3
-              2104 STORE_NAME              84 (v)
-              2106 STORE_NAME              85 (q)
-              2108 STORE_NAME              86 (p)
-   
-   575        2110 PUSH_NULL
-              2112 LOAD_NAME               74 (print)
-              2114 LOAD_CONST              96 ('Value: ')
-              2116 LOAD_NAME               84 (v)
-              2118 LOAD_CONST              97 ('.3f')
-              2120 FORMAT_VALUE             4 (with format)
-              2122 LOAD_CONST              98 (', Precision: ')
-              2124 LOAD_NAME               86 (p)
-              2126 FORMAT_VALUE             0
-              2128 LOAD_CONST              99 (', Quantile: ')
-              2130 LOAD_NAME               85 (q)
-              2132 LOAD_CONST             100 ('.')
-              2134 LOAD_NAME               86 (p)
-              2136 LOAD_CONST             101 (2)
-              2138 BINARY_OP               10 (-)
-              2142 FORMAT_VALUE             0
-              2144 LOAD_CONST             102 ('%')
-              2146 BUILD_STRING             3
-              2148 FORMAT_VALUE             4 (with format)
-              2150 BUILD_STRING             6
-              2152 PRECALL                  1
-              2156 CALL                     1
-              2166 POP_TOP
-              2168 JUMP_BACKWARD           36 (to 2098)
-   
-   581     >> 2170 LOAD_CONST             105 ('input_string')
-   
-   582        2172 LOAD_NAME               43 (str)
-   
-   581        2174 LOAD_CONST             106 ('str1')
-   
-   583        2176 LOAD_NAME               43 (str)
-   
-   581        2178 LOAD_CONST             107 ('str2')
-   
-   584        2180 LOAD_NAME               43 (str)
-   
-   581        2182 LOAD_CONST              12 ('return')
-   
-   585        2184 LOAD_NAME               87 (tuple)
-              2186 LOAD_NAME               43 (str)
-              2188 LOAD_NAME               43 (str)
-              2190 BUILD_TUPLE              2
-              2192 BINARY_SUBSCR
-   
-   581        2202 BUILD_TUPLE              8
-              2204 LOAD_CONST             108 (<code object split_string, file "C:\Users\calsm\Documents\AI Alignment\sae-vis\sae_vis\utils_fns.py", line 581>)
-              2206 MAKE_FUNCTION            4 (annotations)
-              2208 STORE_NAME              88 (split_string)
-   
-   597        2210 LOAD_NAME               41 (MAIN)
-              2212 POP_JUMP_FORWARD_IF_FALSE    56 (to 2326)
-   
-   598        2214 LOAD_CONST             109 ('The quick brown fox jumps over the lazy dog')
-              2216 STORE_NAME              89 (input_string)
-   
-   599        2218 LOAD_CONST             110 ('quick')
-              2220 STORE_NAME              90 (str1)
-   
-   600        2222 LOAD_CONST             111 ('jumps')
-              2224 STORE_NAME              91 (str2)
-   
-   601        2226 PUSH_NULL
-              2228 LOAD_NAME               74 (print)
-              2230 PUSH_NULL
-              2232 LOAD_NAME               88 (split_string)
-              2234 LOAD_NAME               89 (input_string)
-              2236 LOAD_NAME               90 (str1)
-              2238 LOAD_NAME               91 (str2)
-              2240 PRECALL                  3
-              2244 CALL                     3
-              2254 PRECALL                  1
-              2258 CALL                     1
-              2268 POP_TOP
-   
-   603        2270 LOAD_CONST             112 ('Before table <!-- Logits table --> Table <!-- Logits histogram --> After table')
-              2272 STORE_NAME              89 (input_string)
-   
-   604        2274 LOAD_CONST             113 ('<!-- Logits table -->')
-              2276 STORE_NAME              90 (str1)
-   
-   605        2278 LOAD_CONST             114 ('<!-- Logits histogram -->')
-              2280 STORE_NAME              91 (str2)
-   
-   606        2282 PUSH_NULL
-              2284 LOAD_NAME               74 (print)
-              2286 PUSH_NULL
-              2288 LOAD_NAME               88 (split_string)
-              2290 LOAD_NAME               89 (input_string)
-              2292 LOAD_NAME               90 (str1)
-              2294 LOAD_NAME               91 (str2)
-              2296 PRECALL                  3
-              2300 CALL                     3
-              2310 PRECALL                  1
-              2314 CALL                     1
-              2324 POP_TOP
-   
-   615     >> 2326 NOP
-   
-   612        2328 LOAD_CONST             140 ((False,))
-              2330 LOAD_CONST             115 ('text')
-   
-   613        2332 LOAD_NAME               43 (str)
-   
-   612        2334 LOAD_CONST             116 ('prefix')
-   
-   614        2336 LOAD_NAME               43 (str)
-   
-   612        2338 LOAD_CONST             117 ('first_line_indented')
-   
-   615        2340 LOAD_NAME               42 (bool)
-   
-   612        2342 LOAD_CONST              12 ('return')
-   
-   616        2344 LOAD_NAME               43 (str)
-   
-   612        2346 BUILD_TUPLE              8
-              2348 LOAD_CONST             118 (<code object apply_indent, file "C:\Users\calsm\Documents\AI Alignment\sae-vis\sae_vis\utils_fns.py", line 612>)
-              2350 MAKE_FUNCTION            5 (defaults, annotations)
-              2352 STORE_NAME              92 (apply_indent)
+   431        1244 LOAD_NAME               25 (dataclass)
    
-   639        2354 LOAD_CONST             143 (('',))
-              2356 LOAD_CONST             120 ('dict1')
+   432        1246 PUSH_NULL
+              1248 LOAD_BUILD_CLASS
+              1250 LOAD_CONST              82 (<code object QuantileCalculator, file "C:\Users\calsm\Documents\AI Alignment\sae-vis\sae_vis\utils_fns.py", line 430>)
+              1252 MAKE_FUNCTION            0
+              1254 LOAD_CONST              83 ('QuantileCalculator')
+              1256 PRECALL                  2
+              1260 CALL                     2
+   
+   431        1270 PRECALL                  0
+              1274 CALL                     0
+   
+   430        1284 PRECALL                  0
+              1288 CALL                     0
+   
+   432        1298 STORE_NAME              65 (QuantileCalculator)
+   
+   556        1300 LOAD_NAME               41 (MAIN)
+              1302 EXTENDED_ARG             1
+              1304 POP_JUMP_FORWARD_IF_FALSE   430 (to 2166)
+   
+   559        1306 PUSH_NULL
+              1308 LOAD_NAME               37 (get_device)
+              1310 PRECALL                  0
+              1314 CALL                     0
+              1324 STORE_NAME              36 (device)
+   
+   560        1326 LOAD_CONST              84 (100000)
+              1328 STORE_NAME              66 (N)
+   
+   561        1330 PUSH_NULL
+              1332 LOAD_NAME               17 (torch)
+              1334 LOAD_ATTR               67 (stack)
+              1344 PUSH_NULL
+              1346 LOAD_NAME               17 (torch)
+              1348 LOAD_ATTR               68 (rand)
+              1358 LOAD_NAME               66 (N)
+              1360 PRECALL                  1
+              1364 CALL                     1
+              1374 LOAD_METHOD             69 (masked_fill)
+              1396 PUSH_NULL
+              1398 LOAD_NAME               17 (torch)
+              1400 LOAD_ATTR               68 (rand)
+              1410 LOAD_NAME               66 (N)
+              1412 PRECALL                  1
+              1416 CALL                     1
+              1426 LOAD_CONST              85 (0.5)
+              1428 COMPARE_OP               0 (<)
+              1434 LOAD_CONST              73 (0.0)
+              1436 PRECALL                  2
+              1440 CALL                     2
+              1450 PUSH_NULL
+              1452 LOAD_NAME               17 (torch)
+              1454 LOAD_ATTR               68 (rand)
+              1464 LOAD_NAME               66 (N)
+              1466 PRECALL                  1
+              1470 CALL                     1
+              1480 BUILD_LIST               2
+              1482 PRECALL                  1
+              1486 CALL                     1
+              1496 LOAD_METHOD             70 (to)
+              1518 LOAD_NAME               36 (device)
+              1520 PRECALL                  1
+              1524 CALL                     1
+              1534 STORE_NAME              71 (data)
+   
+   562        1536 LOAD_NAME               65 (QuantileCalculator)
+              1538 LOAD_METHOD             72 (from_data)
+              1560 LOAD_NAME               71 (data)
+              1562 PRECALL                  1
+              1566 CALL                     1
+              1576 STORE_NAME              73 (qc)
+   
+   563        1578 PUSH_NULL
+              1580 LOAD_NAME               74 (print)
+              1582 LOAD_CONST              86 ('Total datapoints stored = ')
+              1584 PUSH_NULL
+              1586 LOAD_NAME               75 (sum)
+              1588 LOAD_CONST              87 (<code object <genexpr>, file "C:\Users\calsm\Documents\AI Alignment\sae-vis\sae_vis\utils_fns.py", line 563>)
+              1590 MAKE_FUNCTION            0
+              1592 LOAD_NAME               73 (qc)
+              1594 LOAD_ATTR               76 (quantile_data)
+              1604 GET_ITER
+              1606 PRECALL                  0
+              1610 CALL                     0
+              1620 PRECALL                  1
+              1624 CALL                     1
+              1634 LOAD_CONST              88 ('_')
+              1636 FORMAT_VALUE             4 (with format)
+              1638 BUILD_STRING             2
+              1640 PRECALL                  1
+              1644 CALL                     1
+              1654 POP_TOP
+   
+   564        1656 PUSH_NULL
+              1658 LOAD_NAME               74 (print)
+              1660 LOAD_CONST              89 ('Total datapoints used to compute quantiles = ')
+              1662 LOAD_NAME               71 (data)
+              1664 LOAD_METHOD             77 (numel)
+              1686 PRECALL                  0
+              1690 CALL                     0
+              1700 LOAD_CONST              88 ('_')
+              1702 FORMAT_VALUE             4 (with format)
+              1704 LOAD_CONST              90 ('\n')
+              1706 BUILD_STRING             3
+              1708 PRECALL                  1
+              1712 CALL                     1
+              1722 POP_TOP
+   
+   567        1724 PUSH_NULL
+              1726 LOAD_NAME               17 (torch)
+              1728 LOAD_ATTR               78 (tensor)
+              1738 BUILD_LIST               0
+              1740 LOAD_CONST              91 ((0.0, 0.005, 0.02, 0.25))
+              1742 LIST_EXTEND              1
+              1744 BUILD_LIST               0
+              1746 LOAD_CONST              92 ((0.75, 0.98, 0.995, 1.0))
+              1748 LIST_EXTEND              1
+              1750 BUILD_LIST               2
+              1752 PRECALL                  1
+              1756 CALL                     1
+              1766 LOAD_METHOD             70 (to)
+              1788 LOAD_NAME               36 (device)
+              1790 PRECALL                  1
+              1794 CALL                     1
+              1804 STORE_NAME              79 (values)
+   
+   568        1806 LOAD_NAME               73 (qc)
+              1808 LOAD_METHOD             80 (get_quantile)
+              1830 LOAD_NAME               79 (values)
+              1832 PRECALL                  1
+              1836 CALL                     1
+              1846 UNPACK_SEQUENCE          2
+              1850 STORE_NAME              81 (quantiles)
+              1852 STORE_NAME              82 (precisions)
+   
+   570        1854 PUSH_NULL
+              1856 LOAD_NAME               74 (print)
+              1858 LOAD_CONST              93 ('When 50% of data is 0, and 50% is Unif[0, 1]')
+              1860 PRECALL                  1
+              1864 CALL                     1
+              1874 POP_TOP
+   
+   571        1876 PUSH_NULL
+              1878 LOAD_NAME               83 (zip)
+              1880 LOAD_NAME               79 (values)
+              1882 LOAD_CONST               0 (0)
+              1884 BINARY_SUBSCR
+              1894 LOAD_NAME               81 (quantiles)
+              1896 LOAD_CONST               0 (0)
+              1898 BINARY_SUBSCR
+              1908 LOAD_NAME               82 (precisions)
+              1910 LOAD_CONST               0 (0)
+              1912 BINARY_SUBSCR
+              1922 PRECALL                  3
+              1926 CALL                     3
+              1936 GET_ITER
+           >> 1938 FOR_ITER                35 (to 2010)
+              1940 UNPACK_SEQUENCE          3
+              1944 STORE_NAME              84 (v)
+              1946 STORE_NAME              85 (q)
+              1948 STORE_NAME              86 (p)
+   
+   572        1950 PUSH_NULL
+              1952 LOAD_NAME               74 (print)
+              1954 LOAD_CONST              94 ('Value: ')
+              1956 LOAD_NAME               84 (v)
+              1958 LOAD_CONST              95 ('.3f')
+              1960 FORMAT_VALUE             4 (with format)
+              1962 LOAD_CONST              96 (', Precision: ')
+              1964 LOAD_NAME               86 (p)
+              1966 FORMAT_VALUE             0
+              1968 LOAD_CONST              97 (', Quantile: ')
+              1970 LOAD_NAME               85 (q)
+              1972 LOAD_CONST              98 ('.')
+              1974 LOAD_NAME               86 (p)
+              1976 LOAD_CONST              99 (2)
+              1978 BINARY_OP               10 (-)
+              1982 FORMAT_VALUE             0
+              1984 LOAD_CONST             100 ('%')
+              1986 BUILD_STRING             3
+              1988 FORMAT_VALUE             4 (with format)
+              1990 BUILD_STRING             6
+              1992 PRECALL                  1
+              1996 CALL                     1
+              2006 POP_TOP
+              2008 JUMP_BACKWARD           36 (to 1938)
+   
+   573     >> 2010 PUSH_NULL
+              2012 LOAD_NAME               74 (print)
+              2014 LOAD_CONST             101 ('\nWhen 100% of data is Unif[0, 1]')
+              2016 PRECALL                  1
+              2020 CALL                     1
+              2030 POP_TOP
+   
+   574        2032 PUSH_NULL
+              2034 LOAD_NAME               83 (zip)
+              2036 LOAD_NAME               79 (values)
+              2038 LOAD_CONST             102 (1)
+              2040 BINARY_SUBSCR
+              2050 LOAD_NAME               81 (quantiles)
+              2052 LOAD_CONST             102 (1)
+              2054 BINARY_SUBSCR
+              2064 LOAD_NAME               82 (precisions)
+              2066 LOAD_CONST             102 (1)
+              2068 BINARY_SUBSCR
+              2078 PRECALL                  3
+              2082 CALL                     3
+              2092 GET_ITER
+           >> 2094 FOR_ITER                35 (to 2166)
+              2096 UNPACK_SEQUENCE          3
+              2100 STORE_NAME              84 (v)
+              2102 STORE_NAME              85 (q)
+              2104 STORE_NAME              86 (p)
+   
+   575        2106 PUSH_NULL
+              2108 LOAD_NAME               74 (print)
+              2110 LOAD_CONST              94 ('Value: ')
+              2112 LOAD_NAME               84 (v)
+              2114 LOAD_CONST              95 ('.3f')
+              2116 FORMAT_VALUE             4 (with format)
+              2118 LOAD_CONST              96 (', Precision: ')
+              2120 LOAD_NAME               86 (p)
+              2122 FORMAT_VALUE             0
+              2124 LOAD_CONST              97 (', Quantile: ')
+              2126 LOAD_NAME               85 (q)
+              2128 LOAD_CONST              98 ('.')
+              2130 LOAD_NAME               86 (p)
+              2132 LOAD_CONST              99 (2)
+              2134 BINARY_OP               10 (-)
+              2138 FORMAT_VALUE             0
+              2140 LOAD_CONST             100 ('%')
+              2142 BUILD_STRING             3
+              2144 FORMAT_VALUE             4 (with format)
+              2146 BUILD_STRING             6
+              2148 PRECALL                  1
+              2152 CALL                     1
+              2162 POP_TOP
+              2164 JUMP_BACKWARD           36 (to 2094)
+   
+   581     >> 2166 LOAD_CONST             103 ('input_string')
+   
+   582        2168 LOAD_NAME               43 (str)
+   
+   581        2170 LOAD_CONST             104 ('str1')
+   
+   583        2172 LOAD_NAME               43 (str)
+   
+   581        2174 LOAD_CONST             105 ('str2')
+   
+   584        2176 LOAD_NAME               43 (str)
+   
+   581        2178 LOAD_CONST              12 ('return')
+   
+   585        2180 LOAD_NAME               87 (tuple)
+              2182 LOAD_NAME               43 (str)
+              2184 LOAD_NAME               43 (str)
+              2186 BUILD_TUPLE              2
+              2188 BINARY_SUBSCR
+   
+   581        2198 BUILD_TUPLE              8
+              2200 LOAD_CONST             106 (<code object split_string, file "C:\Users\calsm\Documents\AI Alignment\sae-vis\sae_vis\utils_fns.py", line 581>)
+              2202 MAKE_FUNCTION            4 (annotations)
+              2204 STORE_NAME              88 (split_string)
+   
+   597        2206 LOAD_NAME               41 (MAIN)
+              2208 POP_JUMP_FORWARD_IF_FALSE    56 (to 2322)
+   
+   598        2210 LOAD_CONST             107 ('The quick brown fox jumps over the lazy dog')
+              2212 STORE_NAME              89 (input_string)
+   
+   599        2214 LOAD_CONST             108 ('quick')
+              2216 STORE_NAME              90 (str1)
+   
+   600        2218 LOAD_CONST             109 ('jumps')
+              2220 STORE_NAME              91 (str2)
+   
+   601        2222 PUSH_NULL
+              2224 LOAD_NAME               74 (print)
+              2226 PUSH_NULL
+              2228 LOAD_NAME               88 (split_string)
+              2230 LOAD_NAME               89 (input_string)
+              2232 LOAD_NAME               90 (str1)
+              2234 LOAD_NAME               91 (str2)
+              2236 PRECALL                  3
+              2240 CALL                     3
+              2250 PRECALL                  1
+              2254 CALL                     1
+              2264 POP_TOP
+   
+   603        2266 LOAD_CONST             110 ('Before table <!-- Logits table --> Table <!-- Logits histogram --> After table')
+              2268 STORE_NAME              89 (input_string)
+   
+   604        2270 LOAD_CONST             111 ('<!-- Logits table -->')
+              2272 STORE_NAME              90 (str1)
+   
+   605        2274 LOAD_CONST             112 ('<!-- Logits histogram -->')
+              2276 STORE_NAME              91 (str2)
+   
+   606        2278 PUSH_NULL
+              2280 LOAD_NAME               74 (print)
+              2282 PUSH_NULL
+              2284 LOAD_NAME               88 (split_string)
+              2286 LOAD_NAME               89 (input_string)
+              2288 LOAD_NAME               90 (str1)
+              2290 LOAD_NAME               91 (str2)
+              2292 PRECALL                  3
+              2296 CALL                     3
+              2306 PRECALL                  1
+              2310 CALL                     1
+              2320 POP_TOP
+   
+   615     >> 2322 NOP
+   
+   612        2324 LOAD_CONST             138 ((False,))
+              2326 LOAD_CONST             113 ('text')
+   
+   613        2328 LOAD_NAME               43 (str)
+   
+   612        2330 LOAD_CONST             114 ('prefix')
+   
+   614        2332 LOAD_NAME               43 (str)
+   
+   612        2334 LOAD_CONST             115 ('first_line_indented')
+   
+   615        2336 LOAD_NAME               42 (bool)
+   
+   612        2338 LOAD_CONST              12 ('return')
+   
+   616        2340 LOAD_NAME               43 (str)
+   
+   612        2342 BUILD_TUPLE              8
+              2344 LOAD_CONST             116 (<code object apply_indent, file "C:\Users\calsm\Documents\AI Alignment\sae-vis\sae_vis\utils_fns.py", line 612>)
+              2346 MAKE_FUNCTION            5 (defaults, annotations)
+              2348 STORE_NAME              92 (apply_indent)
+   
+   639        2350 LOAD_CONST             141 (('',))
+              2352 LOAD_CONST             118 ('dict1')
+              2354 LOAD_NAME               93 (dict)
+              2356 LOAD_CONST             119 ('dict2')
               2358 LOAD_NAME               93 (dict)
-              2360 LOAD_CONST             121 ('dict2')
-              2362 LOAD_NAME               93 (dict)
-              2364 LOAD_CONST             122 ('path')
-              2366 LOAD_NAME               43 (str)
-              2368 LOAD_CONST              12 ('return')
-              2370 LOAD_NAME               93 (dict)
-              2372 BUILD_TUPLE              8
-              2374 LOAD_CONST             123 (<code object deep_union, file "C:\Users\calsm\Documents\AI Alignment\sae-vis\sae_vis\utils_fns.py", line 639>)
-              2376 MAKE_FUNCTION            5 (defaults, annotations)
-              2378 STORE_NAME              94 (deep_union)
-   
-   701        2380 LOAD_NAME               41 (MAIN)
-              2382 POP_JUMP_FORWARD_IF_FALSE   131 (to 2646)
-   
-   703        2384 PUSH_NULL
-              2386 LOAD_NAME               94 (deep_union)
-              2388 LOAD_CONST             104 (1)
-              2390 LOAD_CONST             101 (2)
-              2392 BUILD_MAP                1
-              2394 LOAD_CONST              81 (3)
-              2396 LOAD_CONST              79 (4)
-              2398 BUILD_MAP                1
-              2400 PRECALL                  2
-              2404 CALL                     2
-              2414 LOAD_CONST             101 (2)
-              2416 LOAD_CONST              79 (4)
-              2418 LOAD_CONST             124 ((1, 3))
-              2420 BUILD_CONST_KEY_MAP      2
-              2422 COMPARE_OP               2 (==)
-              2428 POP_JUMP_FORWARD_IF_TRUE     2 (to 2434)
-              2430 LOAD_ASSERTION_ERROR
-              2432 RAISE_VARARGS            1
-   
-   706     >> 2434 PUSH_NULL
-              2436 LOAD_NAME               94 (deep_union)
-   
-   707        2438 LOAD_CONST             104 (1)
-              2440 LOAD_CONST             101 (2)
-              2442 LOAD_CONST              81 (3)
-              2444 LOAD_CONST              79 (4)
-              2446 BUILD_LIST               2
-              2448 BUILD_MAP                1
-              2450 BUILD_MAP                1
-   
-   708        2452 LOAD_CONST             104 (1)
-              2454 LOAD_CONST              81 (3)
-              2456 LOAD_CONST              81 (3)
-              2458 LOAD_CONST              79 (4)
-              2460 BUILD_LIST               2
-              2462 BUILD_MAP                1
-              2464 BUILD_MAP                1
-   
-   706        2466 PRECALL                  2
-              2470 CALL                     2
-   
-   709        2480 LOAD_CONST             104 (1)
-              2482 LOAD_CONST              81 (3)
-              2484 LOAD_CONST              79 (4)
-              2486 BUILD_LIST               2
-              2488 LOAD_CONST              81 (3)
-              2490 LOAD_CONST              79 (4)
-              2492 BUILD_LIST               2
-              2494 LOAD_CONST             125 ((2, 3))
-              2496 BUILD_CONST_KEY_MAP      2
-              2498 BUILD_MAP                1
-   
-   706        2500 COMPARE_OP               2 (==)
-              2506 POP_JUMP_FORWARD_IF_TRUE     2 (to 2512)
-              2508 LOAD_ASSERTION_ERROR
-              2510 RAISE_VARARGS            1
-   
-   712     >> 2512 PUSH_NULL
-              2514 LOAD_NAME               94 (deep_union)
-   
-   713        2516 LOAD_CONST              20 ('x')
-              2518 LOAD_CONST             126 ('y')
-              2520 LOAD_CONST             127 ('z')
-              2522 LOAD_CONST             104 (1)
+              2360 LOAD_CONST             120 ('path')
+              2362 LOAD_NAME               43 (str)
+              2364 LOAD_CONST              12 ('return')
+              2366 LOAD_NAME               93 (dict)
+              2368 BUILD_TUPLE              8
+              2370 LOAD_CONST             121 (<code object deep_union, file "C:\Users\calsm\Documents\AI Alignment\sae-vis\sae_vis\utils_fns.py", line 639>)
+              2372 MAKE_FUNCTION            5 (defaults, annotations)
+              2374 STORE_NAME              94 (deep_union)
+   
+   701        2376 LOAD_NAME               41 (MAIN)
+              2378 POP_JUMP_FORWARD_IF_FALSE   131 (to 2642)
+   
+   703        2380 PUSH_NULL
+              2382 LOAD_NAME               94 (deep_union)
+              2384 LOAD_CONST             102 (1)
+              2386 LOAD_CONST              99 (2)
+              2388 BUILD_MAP                1
+              2390 LOAD_CONST              79 (3)
+              2392 LOAD_CONST              77 (4)
+              2394 BUILD_MAP                1
+              2396 PRECALL                  2
+              2400 CALL                     2
+              2410 LOAD_CONST              99 (2)
+              2412 LOAD_CONST              77 (4)
+              2414 LOAD_CONST             122 ((1, 3))
+              2416 BUILD_CONST_KEY_MAP      2
+              2418 COMPARE_OP               2 (==)
+              2424 POP_JUMP_FORWARD_IF_TRUE     2 (to 2430)
+              2426 LOAD_ASSERTION_ERROR
+              2428 RAISE_VARARGS            1
+   
+   706     >> 2430 PUSH_NULL
+              2432 LOAD_NAME               94 (deep_union)
+   
+   707        2434 LOAD_CONST             102 (1)
+              2436 LOAD_CONST              99 (2)
+              2438 LOAD_CONST              79 (3)
+              2440 LOAD_CONST              77 (4)
+              2442 BUILD_LIST               2
+              2444 BUILD_MAP                1
+              2446 BUILD_MAP                1
+   
+   708        2448 LOAD_CONST             102 (1)
+              2450 LOAD_CONST              79 (3)
+              2452 LOAD_CONST              79 (3)
+              2454 LOAD_CONST              77 (4)
+              2456 BUILD_LIST               2
+              2458 BUILD_MAP                1
+              2460 BUILD_MAP                1
+   
+   706        2462 PRECALL                  2
+              2466 CALL                     2
+   
+   709        2476 LOAD_CONST             102 (1)
+              2478 LOAD_CONST              79 (3)
+              2480 LOAD_CONST              77 (4)
+              2482 BUILD_LIST               2
+              2484 LOAD_CONST              79 (3)
+              2486 LOAD_CONST              77 (4)
+              2488 BUILD_LIST               2
+              2490 LOAD_CONST             123 ((2, 3))
+              2492 BUILD_CONST_KEY_MAP      2
+              2494 BUILD_MAP                1
+   
+   706        2496 COMPARE_OP               2 (==)
+              2502 POP_JUMP_FORWARD_IF_TRUE     2 (to 2508)
+              2504 LOAD_ASSERTION_ERROR
+              2506 RAISE_VARARGS            1
+   
+   712     >> 2508 PUSH_NULL
+              2510 LOAD_NAME               94 (deep_union)
+   
+   713        2512 LOAD_CONST              20 ('x')
+              2514 LOAD_CONST             124 ('y')
+              2516 LOAD_CONST             125 ('z')
+              2518 LOAD_CONST             102 (1)
+              2520 BUILD_MAP                1
+              2522 BUILD_MAP                1
               2524 BUILD_MAP                1
-              2526 BUILD_MAP                1
-              2528 BUILD_MAP                1
    
-   714        2530 LOAD_CONST              20 ('x')
-              2532 LOAD_CONST             126 ('y')
-              2534 LOAD_CONST             128 ('w')
-              2536 LOAD_CONST             101 (2)
+   714        2526 LOAD_CONST              20 ('x')
+              2528 LOAD_CONST             124 ('y')
+              2530 LOAD_CONST             126 ('w')
+              2532 LOAD_CONST              99 (2)
+              2534 BUILD_MAP                1
+              2536 BUILD_MAP                1
               2538 BUILD_MAP                1
-              2540 BUILD_MAP                1
-              2542 BUILD_MAP                1
    
-   712        2544 PRECALL                  2
-              2548 CALL                     2
+   712        2540 PRECALL                  2
+              2544 CALL                     2
    
-   715        2558 LOAD_CONST              20 ('x')
-              2560 LOAD_CONST             126 ('y')
-              2562 LOAD_CONST             104 (1)
-              2564 LOAD_CONST             101 (2)
-              2566 LOAD_CONST             129 (('z', 'w'))
-              2568 BUILD_CONST_KEY_MAP      2
-              2570 BUILD_MAP                1
-              2572 BUILD_MAP                1
-   
-   712        2574 COMPARE_OP               2 (==)
-              2580 POP_JUMP_FORWARD_IF_TRUE     2 (to 2586)
-              2582 LOAD_ASSERTION_ERROR
-              2584 RAISE_VARARGS            1
-   
-   718     >> 2586 PUSH_NULL
-              2588 LOAD_NAME               94 (deep_union)
-   
-   719        2590 LOAD_CONST              20 ('x')
-              2592 LOAD_CONST             104 (1)
-              2594 LOAD_CONST             101 (2)
-              2596 BUILD_LIST               2
-              2598 BUILD_MAP                1
-   
-   720        2600 LOAD_CONST              20 ('x')
-              2602 LOAD_CONST              81 (3)
-              2604 LOAD_CONST              79 (4)
-              2606 BUILD_LIST               2
-              2608 BUILD_MAP                1
-   
-   718        2610 PRECALL                  2
-              2614 CALL                     2
-   
-   721        2624 LOAD_CONST              20 ('x')
-              2626 BUILD_LIST               0
-              2628 LOAD_CONST             130 ((1, 2, 3, 4))
-              2630 LIST_EXTEND              1
-              2632 BUILD_MAP                1
-   
-   718        2634 COMPARE_OP               2 (==)
-              2640 POP_JUMP_FORWARD_IF_TRUE     2 (to 2646)
-              2642 LOAD_ASSERTION_ERROR
-              2644 RAISE_VARARGS            1
-   
-   727     >> 2646 PUSH_NULL
-              2648 LOAD_BUILD_CLASS
-              2650 LOAD_CONST             131 (<code object BatchedCorrCoef, file "C:\Users\calsm\Documents\AI Alignment\sae-vis\sae_vis\utils_fns.py", line 727>)
-              2652 MAKE_FUNCTION            0
-              2654 LOAD_CONST             132 ('BatchedCorrCoef')
-              2656 PRECALL                  2
-              2660 CALL                     2
-              2670 STORE_NAME              95 (BatchedCorrCoef)
-   
-   819        2672 LOAD_NAME               28 (dataclass_json)
-   
-   820        2674 LOAD_NAME               25 (dataclass)
-   
-   821        2676 PUSH_NULL
-              2678 LOAD_BUILD_CLASS
-              2680 LOAD_CONST             133 (<code object HistogramData, file "C:\Users\calsm\Documents\AI Alignment\sae-vis\sae_vis\utils_fns.py", line 819>)
-              2682 MAKE_FUNCTION            0
-              2684 LOAD_CONST             134 ('HistogramData')
-              2686 PRECALL                  2
-              2690 CALL                     2
-   
-   820        2700 PRECALL                  0
-              2704 CALL                     0
-   
-   819        2714 PRECALL                  0
-              2718 CALL                     0
-   
-   821        2728 STORE_NAME              96 (HistogramData)
-   
-   907        2730 LOAD_CONST             140 ((False,))
-              2732 LOAD_CONST             135 ('abs')
-              2734 LOAD_NAME               42 (bool)
-              2736 LOAD_CONST              12 ('return')
-              2738 LOAD_NAME               48 (float)
-              2740 LOAD_NAME               45 (int)
-              2742 BINARY_OP                7 (|)
-              2746 BUILD_TUPLE              4
-              2748 LOAD_CONST             136 (<code object max_or_1, file "C:\Users\calsm\Documents\AI Alignment\sae-vis\sae_vis\utils_fns.py", line 907>)
-              2750 MAKE_FUNCTION            5 (defaults, annotations)
-              2752 STORE_NAME              97 (max_or_1)
-              2754 LOAD_CONST               3 (None)
-              2756 RETURN_VALUE
+   715        2554 LOAD_CONST              20 ('x')
+              2556 LOAD_CONST             124 ('y')
+              2558 LOAD_CONST             102 (1)
+              2560 LOAD_CONST              99 (2)
+              2562 LOAD_CONST             127 (('z', 'w'))
+              2564 BUILD_CONST_KEY_MAP      2
+              2566 BUILD_MAP                1
+              2568 BUILD_MAP                1
+   
+   712        2570 COMPARE_OP               2 (==)
+              2576 POP_JUMP_FORWARD_IF_TRUE     2 (to 2582)
+              2578 LOAD_ASSERTION_ERROR
+              2580 RAISE_VARARGS            1
+   
+   718     >> 2582 PUSH_NULL
+              2584 LOAD_NAME               94 (deep_union)
+   
+   719        2586 LOAD_CONST              20 ('x')
+              2588 LOAD_CONST             102 (1)
+              2590 LOAD_CONST              99 (2)
+              2592 BUILD_LIST               2
+              2594 BUILD_MAP                1
+   
+   720        2596 LOAD_CONST              20 ('x')
+              2598 LOAD_CONST              79 (3)
+              2600 LOAD_CONST              77 (4)
+              2602 BUILD_LIST               2
+              2604 BUILD_MAP                1
+   
+   718        2606 PRECALL                  2
+              2610 CALL                     2
+   
+   721        2620 LOAD_CONST              20 ('x')
+              2622 BUILD_LIST               0
+              2624 LOAD_CONST             128 ((1, 2, 3, 4))
+              2626 LIST_EXTEND              1
+              2628 BUILD_MAP                1
+   
+   718        2630 COMPARE_OP               2 (==)
+              2636 POP_JUMP_FORWARD_IF_TRUE     2 (to 2642)
+              2638 LOAD_ASSERTION_ERROR
+              2640 RAISE_VARARGS            1
+   
+   727     >> 2642 PUSH_NULL
+              2644 LOAD_BUILD_CLASS
+              2646 LOAD_CONST             129 (<code object BatchedCorrCoef, file "C:\Users\calsm\Documents\AI Alignment\sae-vis\sae_vis\utils_fns.py", line 727>)
+              2648 MAKE_FUNCTION            0
+              2650 LOAD_CONST             130 ('BatchedCorrCoef')
+              2652 PRECALL                  2
+              2656 CALL                     2
+              2666 STORE_NAME              95 (BatchedCorrCoef)
+   
+   819        2668 LOAD_NAME               28 (dataclass_json)
+   
+   820        2670 LOAD_NAME               25 (dataclass)
+   
+   821        2672 PUSH_NULL
+              2674 LOAD_BUILD_CLASS
+              2676 LOAD_CONST             131 (<code object HistogramData, file "C:\Users\calsm\Documents\AI Alignment\sae-vis\sae_vis\utils_fns.py", line 819>)
+              2678 MAKE_FUNCTION            0
+              2680 LOAD_CONST             132 ('HistogramData')
+              2682 PRECALL                  2
+              2686 CALL                     2
+   
+   820        2696 PRECALL                  0
+              2700 CALL                     0
+   
+   819        2710 PRECALL                  0
+              2714 CALL                     0
+   
+   821        2724 STORE_NAME              96 (HistogramData)
+   
+   907        2726 LOAD_CONST             138 ((False,))
+              2728 LOAD_CONST             133 ('abs')
+              2730 LOAD_NAME               42 (bool)
+              2732 LOAD_CONST              12 ('return')
+              2734 LOAD_NAME               48 (float)
+              2736 LOAD_NAME               45 (int)
+              2738 BINARY_OP                7 (|)
+              2742 BUILD_TUPLE              4
+              2744 LOAD_CONST             134 (<code object max_or_1, file "C:\Users\calsm\Documents\AI Alignment\sae-vis\sae_vis\utils_fns.py", line 907>)
+              2746 MAKE_FUNCTION            5 (defaults, annotations)
+              2748 STORE_NAME              97 (max_or_1)
+              2750 LOAD_CONST               3 (None)
+              2752 RETURN_VALUE
    consts
       0
       ('Float', 'Int', 'Bool')
       ('Tuple', 'Optional', 'Union', 'Dict', 'List', 'Literal', 'Any', 'overload', 'Callable', 'Type', 'TypeVar')
       None
       ('Tensor',)
       ('PreTrainedTokenizerFast',)
@@ -1799,21 +1795,19 @@
       '&#41;'
       '&#40;'
       '&#91;'
       '&#93;'
       '&#123;'
       '&#125;'
       ('\\', '<', '>', ')', '(', '[', ']', '{', '}')
-      '&ndash;'
-      '&rsquo;'
       '&#8203;'
       '&nbsp;'
       '&bsol;n'
       '&bsol;t'
-      ('âĢĶ', 'âĢĻ', 'âĢĭ', 'Ġ', 'Ċ', 'ĉ')
+      ('âĢĭ', 'Ġ', 'Ċ', 'ĉ')
       '&apos;'
       '&quot;'
       ("'", '"')
       ' '
       'str_tok'
       code
          argcount  : 2
@@ -5492,18 +5486,18 @@
    filename   'C:\\Users\\calsm\\Documents\\AI Alignment\\sae-vis\\sae_vis\\utils_fns.py'
    name       '<module>'
    firstlineno 1
    lnotab
       0x00ff020314013401080108010c0108010c010c0110010c0108010c0108
       0108020c021607160f0e020c041e0b020102fc040112ff020202fe020302
       fd020412fc020512fb081e241002fc040112ff020202fe020312fd020412
-      fc020512fb083b481c0201020102010201020102010201020102f7060c02
-      01020102010201020102fa0609020102fe06041402161d100e0201020138
-      ff020202fe020302fd06ff0e0102060201020138ff02020efe02030efd06
-      ff0e010206020138ff02022afe020308fd08181a4c0608201802fd04010e
-      ff020202fe02030efd02040efc08160a010a010a010a010afb04080a010a
-      010afd04070201020118ff0eff0e02027c060314010401ce012a014e0144
-      035201300216014a013c0116014a013c06020102ff020202fe020302fd02
-      0412fc081004010401040104012c020401040104012c0902fd040102ff02
-      0202fe020302fd020402fc081b1a3e0402320304010e010efe0e0314fd0c
-      0604010e010efe0e0310fd0c0604010a010afe0e030afd0c091a5c020102
-      0118ff0eff0e020256
+      fc020512fb083b481c0201020102010201020102010201020102f7060e02
+      010201020102fa0609020102fe06041402161d100e0201020138ff020202
+      fe020302fd06ff0e0102060201020138ff02020efe02030efd06ff0e0102
+      06020138ff02022afe020308fd08181a4c0608201802fd04010eff020202
+      fe02030efd02040efc08160a010a010a010a010afb04080a010a010afd04
+      070201020118ff0eff0e02027c060314010401ce012a014e014403520130
+      0216014a013c0116014a013c06020102ff020202fe020302fd020412fc08
+      1004010401040104012c020401040104012c0902fd040102ff020202fe02
+      0302fd020402fc081b1a3e0402320304010e010efe0e0314fd0c0604010e
+      010efe0e0310fd0c0604010a010afe0e030afd0c091a5c0201020118ff0e
+      ff0e020256
```

### Comparing `sae-vis-0.2.4/sae_vis/css/dropdown.css` & `sae-vis-0.2.5/sae_vis/css/dropdown.css`

 * *Files identical despite different names*

### Comparing `sae-vis-0.2.4/sae_vis/css/general.css` & `sae-vis-0.2.5/sae_vis/css/general.css`

 * *Files identical despite different names*

### Comparing `sae-vis-0.2.4/sae_vis/css/sequences.css` & `sae-vis-0.2.5/sae_vis/css/sequences.css`

 * *Files identical despite different names*

### Comparing `sae-vis-0.2.4/sae_vis/css/tables.css` & `sae-vis-0.2.5/sae_vis/css/tables.css`

 * *Files identical despite different names*

### Comparing `sae-vis-0.2.4/sae_vis/data_config_classes.py` & `sae-vis-0.2.5/sae_vis/data_config_classes.py`

 * *Files identical despite different names*

### Comparing `sae-vis-0.2.4/sae_vis/data_fetching_fns.py` & `sae-vis-0.2.5/sae_vis/data_fetching_fns.py`

 * *Files identical despite different names*

### Comparing `sae-vis-0.2.4/sae_vis/data_storing_fns.py` & `sae-vis-0.2.5/sae_vis/data_storing_fns.py`

 * *Files identical despite different names*

### Comparing `sae-vis-0.2.4/sae_vis/html_fns.py` & `sae-vis-0.2.5/sae_vis/html_fns.py`

 * *Files identical despite different names*

### Comparing `sae-vis-0.2.4/sae_vis/js/_createDropdownsScript.js` & `sae-vis-0.2.5/sae_vis/js/_createDropdownsScript.js`

 * *Files identical despite different names*

### Comparing `sae-vis-0.2.4/sae_vis/js/actsHistogramScript.js` & `sae-vis-0.2.5/sae_vis/js/actsHistogramScript.js`

 * *Files identical despite different names*

### Comparing `sae-vis-0.2.4/sae_vis/js/featureTablesScript.js` & `sae-vis-0.2.5/sae_vis/js/featureTablesScript.js`

 * *Files identical despite different names*

### Comparing `sae-vis-0.2.4/sae_vis/js/gridColumnTitlesScript.js` & `sae-vis-0.2.5/sae_vis/js/gridColumnTitlesScript.js`

 * *Files identical despite different names*

### Comparing `sae-vis-0.2.4/sae_vis/js/logitsHistogramScript.js` & `sae-vis-0.2.5/sae_vis/js/logitsHistogramScript.js`

 * *Files identical despite different names*

### Comparing `sae-vis-0.2.4/sae_vis/js/logitsTableScript.js` & `sae-vis-0.2.5/sae_vis/js/logitsTableScript.js`

 * *Files identical despite different names*

### Comparing `sae-vis-0.2.4/sae_vis/js/tokenScript.js` & `sae-vis-0.2.5/sae_vis/js/tokenScript.js`

 * *Files identical despite different names*

### Comparing `sae-vis-0.2.4/sae_vis/model_fns.py` & `sae-vis-0.2.5/sae_vis/model_fns.py`

 * *Files 3% similar despite different names*

```diff
@@ -181,15 +181,18 @@
                 (self.hook_point, self.hook_fn_store_act),
                 (self.hook_point_resid_final, self.hook_fn_store_act)
             ]
         )
 
         # The hook functions work by storing data in model's hook context, so we pop them back out
         activation: Tensor = self.model.hook_dict[self.hook_point].ctx.pop("activation")
-        residual: Tensor = self.model.hook_dict[self.hook_point_resid_final].ctx.pop("activation")
+        if self.hook_point_resid_final == self.hook_point:
+            residual: Tensor = activation
+        else:
+            residual: Tensor = self.model.hook_dict[self.hook_point_resid_final].ctx.pop("activation")
 
         if return_logits:
             return output, residual, activation
         return residual, activation
 
     def hook_fn_store_act(self, activation: torch.Tensor, hook: HookPoint):
         hook.ctx["activation"] = activation
```

### Comparing `sae-vis-0.2.4/sae_vis/utils_fns.py` & `sae-vis-0.2.5/sae_vis/utils_fns.py`

 * *Files 0% similar despite different names*

```diff
@@ -189,16 +189,16 @@
     "(": "&#40;",
     "[": "&#91;",
     "]": "&#93;",
     "{": "&#123;",
     "}": "&#125;",
 }
 HTML_ANOMALIES = {
-    "âĢĶ": "&ndash;",
-    "âĢĻ": "&rsquo;",
+    # "âĢĶ": "&ndash;",
+    # "âĢĻ": "&rsquo;",
     "âĢĭ": "&#8203;",
     "Ġ": "&nbsp;",
     "Ċ": "&bsol;n",
     "ĉ": "&bsol;t",
 }
 HTML_QUOTES = {
     "'": "&apos;",
```

### Comparing `sae-vis-0.2.4/sae_vis.egg-info/SOURCES.txt` & `sae-vis-0.2.5/sae_vis.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sae-vis-0.2.4/setup.py` & `sae-vis-0.2.5/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name = 'sae-vis',
-    version = '0.2.4',
+    version = '0.2.5',
     packages = find_packages(),
     install_requires = [
         'torch',
         'einops',
         'datasets',
         'dataclasses-json',
         'jaxtyping',
```

