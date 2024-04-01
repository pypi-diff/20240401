# Comparing `tmp/nwb4fp-0.5.7.9.tar.gz` & `tmp/nwb4fp-0.5.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nwb4fp-0.5.7.9.tar", last modified: Mon Apr  1 11:17:20 2024, max compression
+gzip compressed data, was "nwb4fp-0.5.8.0.tar", last modified: Mon Apr  1 12:51:19 2024, max compression
```

## Comparing `nwb4fp-0.5.7.9.tar` & `nwb4fp-0.5.8.0.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxrwxrwx   0        0        0        0 2024-04-01 11:17:20.741835 nwb4fp-0.5.7.9/
--rw-rw-rw-   0        0        0     1089 2024-02-24 13:06:48.000000 nwb4fp-0.5.7.9/LICENSE
--rw-rw-rw-   0        0        0     5786 2024-04-01 11:17:20.735832 nwb4fp-0.5.7.9/PKG-INFO
--rw-rw-rw-   0        0        0     6901 2024-03-27 14:22:15.000000 nwb4fp-0.5.7.9/README.md
--rw-rw-rw-   0        0        0       42 2024-04-01 11:17:20.755835 nwb4fp-0.5.7.9/setup.cfg
--rw-rw-rw-   0        0        0      881 2024-04-01 11:17:18.000000 nwb4fp-0.5.7.9/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-01 11:17:20.125834 nwb4fp-0.5.7.9/src/
-drwxrwxrwx   0        0        0        0 2024-04-01 11:17:20.186834 nwb4fp-0.5.7.9/src/nwb4fp/
--rw-rw-rw-   0        0        0        0 2024-03-03 17:04:21.000000 nwb4fp-0.5.7.9/src/nwb4fp/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-01 11:17:20.130833 nwb4fp-0.5.7.9/src/nwb4fp/main/
--rw-rw-rw-   0        0        0        0 2024-03-08 16:12:29.000000 nwb4fp-0.5.7.9/src/nwb4fp/main/__init__.py
--rw-rw-rw-   0        0        0     3593 2024-03-29 11:35:18.000000 nwb4fp-0.5.7.9/src/nwb4fp/main/main_create_nwb.py
-drwxrwxrwx   0        0        0        0 2024-04-01 11:17:20.135834 nwb4fp-0.5.7.9/src/nwb4fp/postprocess/
--rw-rw-rw-   0        0        0    15551 2024-03-27 11:37:25.000000 nwb4fp-0.5.7.9/src/nwb4fp/postprocess/Get_positions.py
--rw-rw-rw-   0        0        0        0 2024-02-15 18:06:22.000000 nwb4fp-0.5.7.9/src/nwb4fp/postprocess/__init__.py
--rw-rw-rw-   0        0        0     1614 2024-02-21 21:21:29.000000 nwb4fp-0.5.7.9/src/nwb4fp/postprocess/add_wfcor.py
--rw-rw-rw-   0        0        0      470 2024-03-24 12:00:57.000000 nwb4fp-0.5.7.9/src/nwb4fp/postprocess/dlc_kinematic.py
--rw-rw-rw-   0        0        0     2485 2024-03-29 14:47:19.000000 nwb4fp-0.5.7.9/src/nwb4fp/postprocess/extract_wf.py
--rw-rw-rw-   0        0        0     1445 2024-03-03 15:56:30.000000 nwb4fp-0.5.7.9/src/nwb4fp/postprocess/get_potential_merge.py
--rw-rw-rw-   0        0        0     9544 2024-03-26 16:26:32.000000 nwb4fp-0.5.7.9/src/nwb4fp/postprocess/nwbPHYnOPHYS.py
--rw-rw-rw-   0        0        0    11864 2024-04-01 11:17:02.000000 nwb4fp-0.5.7.9/src/nwb4fp/postprocess/quality_metrix.py
-drwxrwxrwx   0        0        0        0 2024-04-01 11:17:20.140832 nwb4fp-0.5.7.9/src/nwb4fp/preprocess/
--rw-rw-rw-   0        0        0        0 2024-02-27 13:40:23.000000 nwb4fp-0.5.7.9/src/nwb4fp/preprocess/__init__.py
--rw-rw-rw-   0        0        0      459 2024-02-27 13:40:23.000000 nwb4fp-0.5.7.9/src/nwb4fp/preprocess/copy_file.py
--rw-rw-rw-   0        0        0      620 2024-02-27 13:40:23.000000 nwb4fp-0.5.7.9/src/nwb4fp/preprocess/down_sample.py
--rw-rw-rw-   0        0        0     6762 2024-03-05 12:39:24.000000 nwb4fp-0.5.7.9/src/nwb4fp/preprocess/down_sample_lfp.py
--rw-rw-rw-   0        0        0     3712 2024-02-27 13:40:23.000000 nwb4fp-0.5.7.9/src/nwb4fp/preprocess/extract_lfp.py
--rw-rw-rw-   0        0        0      148 2024-02-27 13:40:23.000000 nwb4fp-0.5.7.9/src/nwb4fp/preprocess/get_path.py
--rw-rw-rw-   0        0        0     1203 2024-02-27 13:40:23.000000 nwb4fp-0.5.7.9/src/nwb4fp/preprocess/load_data.py
--rw-rw-rw-   0        0        0      244 2024-02-27 13:40:23.000000 nwb4fp-0.5.7.9/src/nwb4fp/preprocess/run_phy.py
-drwxrwxrwx   0        0        0        0 2024-04-01 11:17:20.147839 nwb4fp-0.5.7.9/src/nwb4fp/test/
-drwxrwxrwx   0        0        0        0 2024-04-01 11:17:20.690834 nwb4fp-0.5.7.9/src/nwb4fp/test/run_scripts/
--rw-rw-rw-   0        0        0     1570 2024-03-30 17:18:32.000000 nwb4fp-0.5.7.9/src/nwb4fp/test/run_scripts/readnwb.py
--rw-rw-rw-   0        0        0     1472 2024-03-29 14:44:28.000000 nwb4fp-0.5.7.9/src/nwb4fp/test/run_scripts/readnwb_09PC.py
--rw-rw-rw-   0        0        0        0 2024-03-13 14:23:55.000000 nwb4fp-0.5.7.9/src/nwb4fp/test/run_scripts/test.py
-drwxrwxrwx   0        0        0        0 2024-04-01 11:17:20.200842 nwb4fp-0.5.7.9/src/nwb4fp.egg-info/
--rw-rw-rw-   0        0        0     5786 2024-04-01 11:17:19.000000 nwb4fp-0.5.7.9/src/nwb4fp.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1000 2024-04-01 11:17:20.000000 nwb4fp-0.5.7.9/src/nwb4fp.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-01 11:17:19.000000 nwb4fp-0.5.7.9/src/nwb4fp.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0     2916 2024-04-01 11:17:19.000000 nwb4fp-0.5.7.9/src/nwb4fp.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-04-01 11:17:19.000000 nwb4fp-0.5.7.9/src/nwb4fp.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-01 12:51:19.428459 nwb4fp-0.5.8.0/
+-rw-rw-rw-   0        0        0     1089 2024-02-24 13:06:48.000000 nwb4fp-0.5.8.0/LICENSE
+-rw-rw-rw-   0        0        0     5786 2024-04-01 12:51:19.378447 nwb4fp-0.5.8.0/PKG-INFO
+-rw-rw-rw-   0        0        0     6901 2024-03-27 14:22:15.000000 nwb4fp-0.5.8.0/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-01 12:51:19.585439 nwb4fp-0.5.8.0/setup.cfg
+-rw-rw-rw-   0        0        0      881 2024-04-01 12:48:51.000000 nwb4fp-0.5.8.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-01 12:51:12.724453 nwb4fp-0.5.8.0/src/
+drwxrwxrwx   0        0        0        0 2024-04-01 12:51:13.409455 nwb4fp-0.5.8.0/src/nwb4fp/
+-rw-rw-rw-   0        0        0        0 2024-03-03 17:04:21.000000 nwb4fp-0.5.8.0/src/nwb4fp/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-01 12:51:15.026447 nwb4fp-0.5.8.0/src/nwb4fp/main/
+-rw-rw-rw-   0        0        0        0 2024-03-08 16:12:29.000000 nwb4fp-0.5.8.0/src/nwb4fp/main/__init__.py
+-rw-rw-rw-   0        0        0     3593 2024-03-29 11:35:18.000000 nwb4fp-0.5.8.0/src/nwb4fp/main/main_create_nwb.py
+drwxrwxrwx   0        0        0        0 2024-04-01 12:51:16.923442 nwb4fp-0.5.8.0/src/nwb4fp/postprocess/
+-rw-rw-rw-   0        0        0    15551 2024-03-27 11:37:25.000000 nwb4fp-0.5.8.0/src/nwb4fp/postprocess/Get_positions.py
+-rw-rw-rw-   0        0        0        0 2024-02-15 18:06:22.000000 nwb4fp-0.5.8.0/src/nwb4fp/postprocess/__init__.py
+-rw-rw-rw-   0        0        0     1614 2024-02-21 21:21:29.000000 nwb4fp-0.5.8.0/src/nwb4fp/postprocess/add_wfcor.py
+-rw-rw-rw-   0        0        0      470 2024-03-24 12:00:57.000000 nwb4fp-0.5.8.0/src/nwb4fp/postprocess/dlc_kinematic.py
+-rw-rw-rw-   0        0        0     2485 2024-03-29 14:47:19.000000 nwb4fp-0.5.8.0/src/nwb4fp/postprocess/extract_wf.py
+-rw-rw-rw-   0        0        0     1445 2024-03-03 15:56:30.000000 nwb4fp-0.5.8.0/src/nwb4fp/postprocess/get_potential_merge.py
+-rw-rw-rw-   0        0        0     9544 2024-03-26 16:26:32.000000 nwb4fp-0.5.8.0/src/nwb4fp/postprocess/nwbPHYnOPHYS.py
+-rw-rw-rw-   0        0        0    11865 2024-04-01 12:48:41.000000 nwb4fp-0.5.8.0/src/nwb4fp/postprocess/quality_metrix.py
+drwxrwxrwx   0        0        0        0 2024-04-01 12:51:18.197452 nwb4fp-0.5.8.0/src/nwb4fp/preprocess/
+-rw-rw-rw-   0        0        0        0 2024-02-27 13:40:23.000000 nwb4fp-0.5.8.0/src/nwb4fp/preprocess/__init__.py
+-rw-rw-rw-   0        0        0      459 2024-02-27 13:40:23.000000 nwb4fp-0.5.8.0/src/nwb4fp/preprocess/copy_file.py
+-rw-rw-rw-   0        0        0      620 2024-02-27 13:40:23.000000 nwb4fp-0.5.8.0/src/nwb4fp/preprocess/down_sample.py
+-rw-rw-rw-   0        0        0     6762 2024-03-05 12:39:24.000000 nwb4fp-0.5.8.0/src/nwb4fp/preprocess/down_sample_lfp.py
+-rw-rw-rw-   0        0        0     3712 2024-02-27 13:40:23.000000 nwb4fp-0.5.8.0/src/nwb4fp/preprocess/extract_lfp.py
+-rw-rw-rw-   0        0        0      148 2024-02-27 13:40:23.000000 nwb4fp-0.5.8.0/src/nwb4fp/preprocess/get_path.py
+-rw-rw-rw-   0        0        0     1203 2024-02-27 13:40:23.000000 nwb4fp-0.5.8.0/src/nwb4fp/preprocess/load_data.py
+-rw-rw-rw-   0        0        0      244 2024-02-27 13:40:23.000000 nwb4fp-0.5.8.0/src/nwb4fp/preprocess/run_phy.py
+drwxrwxrwx   0        0        0        0 2024-04-01 12:51:12.895475 nwb4fp-0.5.8.0/src/nwb4fp/test/
+drwxrwxrwx   0        0        0        0 2024-04-01 12:51:19.110446 nwb4fp-0.5.8.0/src/nwb4fp/test/run_scripts/
+-rw-rw-rw-   0        0        0     1570 2024-03-30 17:18:32.000000 nwb4fp-0.5.8.0/src/nwb4fp/test/run_scripts/readnwb.py
+-rw-rw-rw-   0        0        0     1472 2024-03-29 14:44:28.000000 nwb4fp-0.5.8.0/src/nwb4fp/test/run_scripts/readnwb_09PC.py
+-rw-rw-rw-   0        0        0        0 2024-03-13 14:23:55.000000 nwb4fp-0.5.8.0/src/nwb4fp/test/run_scripts/test.py
+drwxrwxrwx   0        0        0        0 2024-04-01 12:51:14.541450 nwb4fp-0.5.8.0/src/nwb4fp.egg-info/
+-rw-rw-rw-   0        0        0     5786 2024-04-01 12:51:11.000000 nwb4fp-0.5.8.0/src/nwb4fp.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1000 2024-04-01 12:51:12.000000 nwb4fp-0.5.8.0/src/nwb4fp.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-01 12:51:11.000000 nwb4fp-0.5.8.0/src/nwb4fp.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0     2916 2024-04-01 12:51:11.000000 nwb4fp-0.5.8.0/src/nwb4fp.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-04-01 12:51:11.000000 nwb4fp-0.5.8.0/src/nwb4fp.egg-info/top_level.txt
```

### Comparing `nwb4fp-0.5.7.9/LICENSE` & `nwb4fp-0.5.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nwb4fp-0.5.7.9/PKG-INFO` & `nwb4fp-0.5.8.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nwb4fp
-Version: 0.5.7.9
+Version: 0.5.8.0
 Summary: Description of my package
 Home-page: https://github.com/sachuriga283/nwb4fp
 Author: sachuriga283
 Author-email: sachuriga.sachuriga@ntnu.no
 License-File: LICENSE
 Requires-Dist: aiobotocore==2.11.2
 Requires-Dist: aiohttp==3.9.3
```

### Comparing `nwb4fp-0.5.7.9/README.md` & `nwb4fp-0.5.8.0/README.md`

 * *Files identical despite different names*

### Comparing `nwb4fp-0.5.7.9/setup.py` & `nwb4fp-0.5.8.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
             return [line.strip() for line in req if line.strip() and not line.startswith('#')]
     except UnicodeDecodeError:
         with open('requirements.txt', encoding='utf-16') as req:
             return [line.strip() for line in req if line.strip() and not line.startswith('#')]
 
 setup(
     name='nwb4fp',
-    version='0.5.7.9',
+    version='0.5.8.0',
     url='https://github.com/sachuriga283/nwb4fp',
     author='sachuriga283',
     author_email='sachuriga.sachuriga@ntnu.no',
     description='Description of my package',
     #packages=find_packages(./src/),    
     install_requires=read_requirements(),
 )
```

### Comparing `nwb4fp-0.5.7.9/src/nwb4fp/main/main_create_nwb.py` & `nwb4fp-0.5.8.0/src/nwb4fp/main/main_create_nwb.py`

 * *Files identical despite different names*

### Comparing `nwb4fp-0.5.7.9/src/nwb4fp/postprocess/Get_positions.py` & `nwb4fp-0.5.8.0/src/nwb4fp/postprocess/Get_positions.py`

 * *Files identical despite different names*

### Comparing `nwb4fp-0.5.7.9/src/nwb4fp/postprocess/add_wfcor.py` & `nwb4fp-0.5.8.0/src/nwb4fp/postprocess/add_wfcor.py`

 * *Files identical despite different names*

### Comparing `nwb4fp-0.5.7.9/src/nwb4fp/postprocess/extract_wf.py` & `nwb4fp-0.5.8.0/src/nwb4fp/postprocess/extract_wf.py`

 * *Files identical despite different names*

### Comparing `nwb4fp-0.5.7.9/src/nwb4fp/postprocess/get_potential_merge.py` & `nwb4fp-0.5.8.0/src/nwb4fp/postprocess/get_potential_merge.py`

 * *Files identical despite different names*

### Comparing `nwb4fp-0.5.7.9/src/nwb4fp/postprocess/nwbPHYnOPHYS.py` & `nwb4fp-0.5.8.0/src/nwb4fp/postprocess/nwbPHYnOPHYS.py`

 * *Files identical despite different names*

### Comparing `nwb4fp-0.5.7.9/src/nwb4fp/postprocess/quality_metrix.py` & `nwb4fp-0.5.8.0/src/nwb4fp/postprocess/quality_metrix.py`

 * *Files 0% similar despite different names*

```diff
@@ -222,12 +222,12 @@
     sex.export_to_phy(waveform_extractor=wf_all,
                       output_folder = path_iron,
                       remove_if_exists=True,
                       copy_binary=True)
 
     wfm.save(Path(path + "_manual/waveformsfm"), format='binary')
     wf_all.save(Path(path + "_manual/waveforms"), format='binary')
-    divide_wf(path_iron,sort_merge)
+    #divide_wf(path_iron,sort_merge)
 
     print("completet!!!!_export_to_phy_part")
 if __name__ == "__main__":
     main()
```

### Comparing `nwb4fp-0.5.7.9/src/nwb4fp/preprocess/down_sample.py` & `nwb4fp-0.5.8.0/src/nwb4fp/preprocess/down_sample.py`

 * *Files identical despite different names*

### Comparing `nwb4fp-0.5.7.9/src/nwb4fp/preprocess/down_sample_lfp.py` & `nwb4fp-0.5.8.0/src/nwb4fp/preprocess/down_sample_lfp.py`

 * *Files identical despite different names*

### Comparing `nwb4fp-0.5.7.9/src/nwb4fp/preprocess/extract_lfp.py` & `nwb4fp-0.5.8.0/src/nwb4fp/preprocess/extract_lfp.py`

 * *Files identical despite different names*

### Comparing `nwb4fp-0.5.7.9/src/nwb4fp/preprocess/load_data.py` & `nwb4fp-0.5.8.0/src/nwb4fp/preprocess/load_data.py`

 * *Files identical despite different names*

### Comparing `nwb4fp-0.5.7.9/src/nwb4fp/test/run_scripts/readnwb.py` & `nwb4fp-0.5.8.0/src/nwb4fp/test/run_scripts/readnwb.py`

 * *Files identical despite different names*

### Comparing `nwb4fp-0.5.7.9/src/nwb4fp/test/run_scripts/readnwb_09PC.py` & `nwb4fp-0.5.8.0/src/nwb4fp/test/run_scripts/readnwb_09PC.py`

 * *Files identical despite different names*

### Comparing `nwb4fp-0.5.7.9/src/nwb4fp.egg-info/PKG-INFO` & `nwb4fp-0.5.8.0/src/nwb4fp.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nwb4fp
-Version: 0.5.7.9
+Version: 0.5.8.0
 Summary: Description of my package
 Home-page: https://github.com/sachuriga283/nwb4fp
 Author: sachuriga283
 Author-email: sachuriga.sachuriga@ntnu.no
 License-File: LICENSE
 Requires-Dist: aiobotocore==2.11.2
 Requires-Dist: aiohttp==3.9.3
```

### Comparing `nwb4fp-0.5.7.9/src/nwb4fp.egg-info/SOURCES.txt` & `nwb4fp-0.5.8.0/src/nwb4fp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nwb4fp-0.5.7.9/src/nwb4fp.egg-info/requires.txt` & `nwb4fp-0.5.8.0/src/nwb4fp.egg-info/requires.txt`

 * *Files identical despite different names*

