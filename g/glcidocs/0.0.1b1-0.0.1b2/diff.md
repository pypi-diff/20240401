# Comparing `tmp/glcidocs-0.0.1b1.tar.gz` & `tmp/glcidocs-0.0.1b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "glcidocs-0.0.1b1.tar", last modified: Mon Apr  1 16:26:53 2024, max compression
+gzip compressed data, was "glcidocs-0.0.1b2.tar", last modified: Mon Apr  1 16:32:43 2024, max compression
```

## Comparing `glcidocs-0.0.1b1.tar` & `glcidocs-0.0.1b2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2024-04-01 16:26:53.967270 glcidocs-0.0.1b1/
--rw-rw-rw-   0        0        0     1092 2024-03-29 11:49:25.000000 glcidocs-0.0.1b1/LICENSE
--rw-rw-rw-   0        0        0       25 2024-04-01 16:26:26.000000 glcidocs-0.0.1b1/MANIFEST.in
--rw-rw-rw-   0        0        0      544 2024-04-01 16:26:53.967270 glcidocs-0.0.1b1/PKG-INFO
--rw-rw-rw-   0        0        0     3225 2024-04-01 16:26:26.000000 glcidocs-0.0.1b1/README.md
--rw-rw-rw-   0        0        0       88 2024-04-01 16:26:26.000000 glcidocs-0.0.1b1/pyproject.toml
--rw-rw-rw-   0        0        0      782 2024-04-01 16:26:53.982895 glcidocs-0.0.1b1/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-01 16:26:53.941343 glcidocs-0.0.1b1/src/
-drwxrwxrwx   0        0        0        0 2024-04-01 16:26:53.967270 glcidocs-0.0.1b1/src/glcidocs/
--rw-rw-rw-   0        0        0     1509 2024-04-01 16:26:26.000000 glcidocs-0.0.1b1/src/glcidocs/__init__.py
--rw-rw-rw-   0        0        0      491 2024-04-01 16:26:26.000000 glcidocs-0.0.1b1/src/glcidocs/__main__.py
--rw-rw-rw-   0        0        0     2105 2024-04-01 16:26:26.000000 glcidocs-0.0.1b1/src/glcidocs/docsgen.py
--rw-rw-rw-   0        0        0       86 2024-04-01 16:26:26.000000 glcidocs-0.0.1b1/src/glcidocs/errors.py
--rw-rw-rw-   0        0        0     3795 2024-04-01 16:26:26.000000 glcidocs-0.0.1b1/src/glcidocs/pipelineparser.py
-drwxrwxrwx   0        0        0        0 2024-04-01 16:26:53.967270 glcidocs-0.0.1b1/src/glcidocs.egg-info/
--rw-rw-rw-   0        0        0      544 2024-04-01 16:26:53.000000 glcidocs-0.0.1b1/src/glcidocs.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      361 2024-04-01 16:26:53.000000 glcidocs-0.0.1b1/src/glcidocs.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-01 16:26:53.000000 glcidocs-0.0.1b1/src/glcidocs.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-04-01 16:26:53.000000 glcidocs-0.0.1b1/src/glcidocs.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0        9 2024-04-01 16:26:53.000000 glcidocs-0.0.1b1/src/glcidocs.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-01 16:32:43.157328 glcidocs-0.0.1b2/
+-rw-rw-rw-   0        0        0     1092 2024-03-29 11:49:25.000000 glcidocs-0.0.1b2/LICENSE
+-rw-rw-rw-   0        0        0       25 2024-04-01 16:26:26.000000 glcidocs-0.0.1b2/MANIFEST.in
+-rw-rw-rw-   0        0        0     3773 2024-04-01 16:32:43.157328 glcidocs-0.0.1b2/PKG-INFO
+-rw-rw-rw-   0        0        0     3225 2024-04-01 16:26:26.000000 glcidocs-0.0.1b2/README.md
+-rw-rw-rw-   0        0        0       88 2024-04-01 16:26:26.000000 glcidocs-0.0.1b2/pyproject.toml
+-rw-rw-rw-   0        0        0      769 2024-04-01 16:32:43.169259 glcidocs-0.0.1b2/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-01 16:32:43.138449 glcidocs-0.0.1b2/src/
+drwxrwxrwx   0        0        0        0 2024-04-01 16:32:43.157328 glcidocs-0.0.1b2/src/glcidocs/
+-rw-rw-rw-   0        0        0     1509 2024-04-01 16:32:25.000000 glcidocs-0.0.1b2/src/glcidocs/__init__.py
+-rw-rw-rw-   0        0        0      491 2024-04-01 16:26:26.000000 glcidocs-0.0.1b2/src/glcidocs/__main__.py
+-rw-rw-rw-   0        0        0     2105 2024-04-01 16:26:26.000000 glcidocs-0.0.1b2/src/glcidocs/docsgen.py
+-rw-rw-rw-   0        0        0       86 2024-04-01 16:26:26.000000 glcidocs-0.0.1b2/src/glcidocs/errors.py
+-rw-rw-rw-   0        0        0     3795 2024-04-01 16:26:26.000000 glcidocs-0.0.1b2/src/glcidocs/pipelineparser.py
+drwxrwxrwx   0        0        0        0 2024-04-01 16:32:43.157328 glcidocs-0.0.1b2/src/glcidocs.egg-info/
+-rw-rw-rw-   0        0        0     3773 2024-04-01 16:32:43.000000 glcidocs-0.0.1b2/src/glcidocs.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      361 2024-04-01 16:32:43.000000 glcidocs-0.0.1b2/src/glcidocs.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-01 16:32:43.000000 glcidocs-0.0.1b2/src/glcidocs.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-04-01 16:26:53.000000 glcidocs-0.0.1b2/src/glcidocs.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0        9 2024-04-01 16:32:43.000000 glcidocs-0.0.1b2/src/glcidocs.egg-info/top_level.txt
```

### Comparing `glcidocs-0.0.1b1/LICENSE` & `glcidocs-0.0.1b2/LICENSE`

 * *Files identical despite different names*

### Comparing `glcidocs-0.0.1b1/README.md` & `glcidocs-0.0.1b2/README.md`

 * *Files identical despite different names*

### Comparing `glcidocs-0.0.1b1/setup.cfg` & `glcidocs-0.0.1b2/setup.cfg`

 * *Files 17% similar despite different names*

```diff
@@ -8,42 +8,42 @@
 00000070: 6e2e 6d75 6472 6f63 6840 7072 6f74 6f6e  n.mudroch@proton
 00000080: 2e6d 650d 0a64 6573 6372 6970 7469 6f6e  .me..description
 00000090: 203d 2053 696d 706c 6520 6765 6e65 7261   = Simple genera
 000000a0: 746f 7220 6f66 2067 6974 6c61 6220 6369  tor of gitlab ci
 000000b0: 2066 696c 6520 646f 6375 6d65 6e74 6174   file documentat
 000000c0: 696f 6e0d 0a6c 6f6e 675f 6465 7363 7269  ion..long_descri
 000000d0: 7074 696f 6e20 3d20 6669 6c65 3a20 5245  ption = file: RE
-000000e0: 4144 4d45 2e6d 6420 4348 414e 4745 4c4f  ADME.md CHANGELO
-000000f0: 472e 6d64 0d0a 6c6f 6e67 5f64 6573 6372  G.md..long_descr
-00000100: 6970 7469 6f6e 5f63 6f6e 7465 6e74 5f74  iption_content_t
-00000110: 7970 6520 3d20 7465 7874 2f6d 6172 6b64  ype = text/markd
-00000120: 6f77 6e0d 0a6b 6579 776f 7264 7320 3d20  own..keywords = 
-00000130: 6769 746c 6162 2c20 7069 7065 6c69 6e65  gitlab, pipeline
-00000140: 2c20 646f 6375 6d65 6e74 6174 696f 6e2c  , documentation,
-00000150: 2063 692f 6364 2c20 6769 746c 6162 2d63   ci/cd, gitlab-c
-00000160: 690d 0a6c 6963 656e 7365 203d 204d 4954  i..license = MIT
-00000170: 0d0a 7572 6c20 3d20 6874 7470 733a 2f2f  ..url = https://
-00000180: 6769 7468 7562 2e63 6f6d 2f6d 6172 7469  github.com/marti
-00000190: 6e33 3536 2f67 6974 6c61 622d 6369 2d64  n356/gitlab-ci-d
-000001a0: 6f63 730d 0a63 6c61 7373 6966 6965 7273  ocs..classifiers
-000001b0: 203d 200d 0a09 5072 6f67 7261 6d6d 696e   = ...Programmin
-000001c0: 6720 4c61 6e67 7561 6765 203a 3a20 5079  g Language :: Py
-000001d0: 7468 6f6e 203a 3a20 330d 0a09 4f70 6572  thon :: 3...Oper
-000001e0: 6174 696e 6720 5379 7374 656d 203a 3a20  ating System :: 
-000001f0: 4f53 2049 6e64 6570 656e 6465 6e74 0d0a  OS Independent..
-00000200: 094c 6963 656e 7365 203a 3a20 4f53 4920  .License :: OSI 
-00000210: 4170 7072 6f76 6564 203a 3a20 4d49 5420  Approved :: MIT 
-00000220: 4c69 6365 6e73 650d 0a0d 0a5b 6f70 7469  License....[opti
-00000230: 6f6e 735d 0d0a 7a69 705f 7361 6665 203d  ons]..zip_safe =
-00000240: 2046 616c 7365 0d0a 696e 636c 7564 655f   False..include_
-00000250: 7061 636b 6167 655f 6461 7461 203d 2054  package_data = T
-00000260: 7275 650d 0a70 6163 6b61 6765 7320 3d20  rue..packages = 
-00000270: 6669 6e64 3a0d 0a70 7974 686f 6e5f 7265  find:..python_re
-00000280: 7175 6972 6573 203d 203e 3d33 2e38 0d0a  quires = >=3.8..
-00000290: 0d0a 5b6f 7074 696f 6e73 2e70 6163 6b61  ..[options.packa
-000002a0: 6765 732e 6669 6e64 5d0d 0a77 6865 7265  ges.find]..where
-000002b0: 203d 2073 7263 0d0a 6578 636c 7564 6520   = src..exclude 
-000002c0: 3d20 0d0a 0965 7861 6d70 6c65 732a 0d0a  = ...examples*..
-000002d0: 0964 6f63 732a 0d0a 0974 6573 7473 2e2a  .docs*...tests.*
-000002e0: 0d0a 0d0a 5b65 6767 5f69 6e66 6f5d 0d0a  ....[egg_info]..
-000002f0: 7461 675f 6275 696c 6420 3d20 0d0a 7461  tag_build = ..ta
-00000300: 675f 6461 7465 203d 2030 0d0a 0d0a       g_date = 0....
+000000e0: 4144 4d45 2e6d 640d 0a6c 6f6e 675f 6465  ADME.md..long_de
+000000f0: 7363 7269 7074 696f 6e5f 636f 6e74 656e  scription_conten
+00000100: 745f 7479 7065 203d 2074 6578 742f 6d61  t_type = text/ma
+00000110: 726b 646f 776e 0d0a 6b65 7977 6f72 6473  rkdown..keywords
+00000120: 203d 2067 6974 6c61 622c 2070 6970 656c   = gitlab, pipel
+00000130: 696e 652c 2064 6f63 756d 656e 7461 7469  ine, documentati
+00000140: 6f6e 2c20 6369 2f63 642c 2067 6974 6c61  on, ci/cd, gitla
+00000150: 622d 6369 0d0a 6c69 6365 6e73 6520 3d20  b-ci..license = 
+00000160: 4d49 540d 0a75 726c 203d 2068 7474 7073  MIT..url = https
+00000170: 3a2f 2f67 6974 6875 622e 636f 6d2f 6d61  ://github.com/ma
+00000180: 7274 696e 3335 362f 6769 746c 6162 2d63  rtin356/gitlab-c
+00000190: 692d 646f 6373 0d0a 636c 6173 7369 6669  i-docs..classifi
+000001a0: 6572 7320 3d20 0d0a 0950 726f 6772 616d  ers = ...Program
+000001b0: 6d69 6e67 204c 616e 6775 6167 6520 3a3a  ming Language ::
+000001c0: 2050 7974 686f 6e20 3a3a 2033 0d0a 094f   Python :: 3...O
+000001d0: 7065 7261 7469 6e67 2053 7973 7465 6d20  perating System 
+000001e0: 3a3a 204f 5320 496e 6465 7065 6e64 656e  :: OS Independen
+000001f0: 740d 0a09 4c69 6365 6e73 6520 3a3a 204f  t...License :: O
+00000200: 5349 2041 7070 726f 7665 6420 3a3a 204d  SI Approved :: M
+00000210: 4954 204c 6963 656e 7365 0d0a 0d0a 5b6f  IT License....[o
+00000220: 7074 696f 6e73 5d0d 0a7a 6970 5f73 6166  ptions]..zip_saf
+00000230: 6520 3d20 4661 6c73 650d 0a69 6e63 6c75  e = False..inclu
+00000240: 6465 5f70 6163 6b61 6765 5f64 6174 6120  de_package_data 
+00000250: 3d20 5472 7565 0d0a 7061 636b 6167 6573  = True..packages
+00000260: 203d 2066 696e 643a 0d0a 7079 7468 6f6e   = find:..python
+00000270: 5f72 6571 7569 7265 7320 3d20 3e3d 332e  _requires = >=3.
+00000280: 380d 0a0d 0a5b 6f70 7469 6f6e 732e 7061  8....[options.pa
+00000290: 636b 6167 6573 2e66 696e 645d 0d0a 7768  ckages.find]..wh
+000002a0: 6572 6520 3d20 7372 630d 0a65 7863 6c75  ere = src..exclu
+000002b0: 6465 203d 200d 0a09 6578 616d 706c 6573  de = ...examples
+000002c0: 2a0d 0a09 646f 6373 2a0d 0a09 7465 7374  *...docs*...test
+000002d0: 732e 2a0d 0a0d 0a5b 6567 675f 696e 666f  s.*....[egg_info
+000002e0: 5d0d 0a74 6167 5f62 7569 6c64 203d 200d  ]..tag_build = .
+000002f0: 0a74 6167 5f64 6174 6520 3d20 300d 0a0d  .tag_date = 0...
+00000300: 0a                                       .
```

### Comparing `glcidocs-0.0.1b1/src/glcidocs/__init__.py` & `glcidocs-0.0.1b2/src/glcidocs/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from pathlib import Path
 from typing import List
 from glcidocs.pipelineparser import CiFileParser
 from glcidocs.docsgen import HTMLBuilder
 
 
-__version__ = '0.0.1-beta.1'
+__version__ = '0.0.1-beta.2'
 
 
 def read_doc_file(file_path: str|Path) -> List[str]:
     with open(file_path, 'r') as f:
         return [line for line in f]
```

### Comparing `glcidocs-0.0.1b1/src/glcidocs/docsgen.py` & `glcidocs-0.0.1b2/src/glcidocs/docsgen.py`

 * *Files identical despite different names*

### Comparing `glcidocs-0.0.1b1/src/glcidocs/pipelineparser.py` & `glcidocs-0.0.1b2/src/glcidocs/pipelineparser.py`

 * *Files identical despite different names*

