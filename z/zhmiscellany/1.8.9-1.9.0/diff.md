# Comparing `tmp/zhmiscellany-1.8.9-py3-none-any.whl.zip` & `tmp/zhmiscellany-1.9.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 19371 bytes, number of entries: 19
+Zip file size: 19391 bytes, number of entries: 19
 -rw-rw-rw-  2.0 fat      215 b- defN 23-Nov-12 21:09 zhmiscellany/__init__.py
 -rw-rw-rw-  2.0 fat     6520 b- defN 23-Dec-08 14:13 zhmiscellany/_discord_supportfuncs.py
 -rw-rw-rw-  2.0 fat      673 b- defN 23-Nov-05 00:34 zhmiscellany/_misc_supportfuncs.py
 -rw-rw-rw-  2.0 fat       59 b- defN 23-Dec-03 10:35 zhmiscellany/_py_resources.py
 -rw-rw-rw-  2.0 fat        8 b- defN 23-Nov-01 16:36 zhmiscellany/_state.py
 -rw-rw-rw-  2.0 fat       81 b- defN 23-Nov-01 22:45 zhmiscellany/dict.py
 -rw-rw-rw-  2.0 fat    15608 b- defN 24-Mar-07 15:37 zhmiscellany/discord.py
@@ -10,12 +10,12 @@
 -rw-rw-rw-  2.0 fat      338 b- defN 23-Oct-31 21:16 zhmiscellany/image.py
 -rw-rw-rw-  2.0 fat      854 b- defN 23-Nov-14 14:55 zhmiscellany/list.py
 -rw-rw-rw-  2.0 fat      632 b- defN 23-Nov-18 07:12 zhmiscellany/math.py
 -rw-rw-rw-  2.0 fat     4435 b- defN 24-Mar-30 18:10 zhmiscellany/misc.py
 -rw-rw-rw-  2.0 fat     1595 b- defN 24-Mar-03 05:51 zhmiscellany/netio.py
 -rw-rw-rw-  2.0 fat      761 b- defN 24-Feb-12 17:09 zhmiscellany/processing.py
 -rw-rw-rw-  2.0 fat     2412 b- defN 23-Nov-18 07:28 zhmiscellany/string.py
--rw-rw-rw-  2.0 fat    18671 b- defN 24-Mar-30 18:11 zhmiscellany-1.8.9.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-Mar-30 18:11 zhmiscellany-1.8.9.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       13 b- defN 24-Mar-30 18:11 zhmiscellany-1.8.9.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     1523 b- defN 24-Mar-30 18:11 zhmiscellany-1.8.9.dist-info/RECORD
-19 files, 58746 bytes uncompressed, 16887 bytes compressed:  71.3%
+-rw-rw-rw-  2.0 fat    18715 b- defN 24-Apr-01 20:24 zhmiscellany-1.9.0.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-01 20:24 zhmiscellany-1.9.0.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       13 b- defN 24-Apr-01 20:24 zhmiscellany-1.9.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     1523 b- defN 24-Apr-01 20:24 zhmiscellany-1.9.0.dist-info/RECORD
+19 files, 58790 bytes uncompressed, 16907 bytes compressed:  71.2%
```

## zipnote {}

```diff
@@ -39,20 +39,20 @@
 
 Filename: zhmiscellany/processing.py
 Comment: 
 
 Filename: zhmiscellany/string.py
 Comment: 
 
-Filename: zhmiscellany-1.8.9.dist-info/METADATA
+Filename: zhmiscellany-1.9.0.dist-info/METADATA
 Comment: 
 
-Filename: zhmiscellany-1.8.9.dist-info/WHEEL
+Filename: zhmiscellany-1.9.0.dist-info/WHEEL
 Comment: 
 
-Filename: zhmiscellany-1.8.9.dist-info/top_level.txt
+Filename: zhmiscellany-1.9.0.dist-info/top_level.txt
 Comment: 
 
-Filename: zhmiscellany-1.8.9.dist-info/RECORD
+Filename: zhmiscellany-1.9.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `zhmiscellany-1.8.9.dist-info/METADATA` & `zhmiscellany-1.9.0.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zhmiscellany
-Version: 1.8.9
+Version: 1.9.0
 Summary: A collection of useful/interesting python libraries made by zh.
 Home-page: https://discord.gg/ThBBAuueVJ
 Author: zh
 Author-email: imnotgivingmyemailjustaddmeondiscordmydiscordisz_h_@zh.com
 Project-URL: Bug Tracker, https://github.com/zen-ham/zhmiscellany/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -12,14 +12,15 @@
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Requires-Dist: pycryptodome >=0
 Requires-Dist: pywin32 >=0
 Requires-Dist: discum ==1.1.0
 Requires-Dist: Requests >=0
 Requires-Dist: pytesseract >=0
+Requires-Dist: random-header-generator >=0
 
 `zhmiscellany`,
 ===
 
 An organized collection of unique and useful functions/classes/modules.
 ---
```

## Comparing `zhmiscellany-1.8.9.dist-info/RECORD` & `zhmiscellany-1.9.0.dist-info/RECORD`

 * *Files 8% similar despite different names*

```diff
@@ -9,11 +9,11 @@
 zhmiscellany/image.py,sha256=uOXFcGG1FhvNeCU7dm6DYxefh6suiL8qg8qtAVyezew,338
 zhmiscellany/list.py,sha256=2kqsscSFXEanmEdR1NuwWaf2l8nPTDUgRyrfL1snoRg,854
 zhmiscellany/math.py,sha256=v2WmHdKrwsrY08E6yUgb0nPHbTuyrljRdgUMw5uqu3U,632
 zhmiscellany/misc.py,sha256=n82JEmQSfU8gX-QTRET3ys6cRuU-DDJjkQFyMMH-5Yg,4435
 zhmiscellany/netio.py,sha256=-nUiO3I5nnTZLezt3IOcs2jWPJ-uiWxJXNZRcTEV8ZA,1595
 zhmiscellany/processing.py,sha256=pE2LVtaZwBvWgd6Xx0S_ZT0WhcKr6GtBhjAfbAflSYo,761
 zhmiscellany/string.py,sha256=2xL_rbJeiGH14k_JkXWUp-oBN30Ltl9-bZk0eHUPltA,2412
-zhmiscellany-1.8.9.dist-info/METADATA,sha256=Qxo3TdmWGh0W49ulhwTzvyaOtvVDrD5Z-OlN1PTS2R0,18671
-zhmiscellany-1.8.9.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-zhmiscellany-1.8.9.dist-info/top_level.txt,sha256=ioDtsrevCI52rTxZntMPljRIBsZs73tD0hI00HektiE,13
-zhmiscellany-1.8.9.dist-info/RECORD,,
+zhmiscellany-1.9.0.dist-info/METADATA,sha256=_RGpPURy62YToKmbOA4ZwZBCj2PFY5D-xQ1UOjkLHTY,18715
+zhmiscellany-1.9.0.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+zhmiscellany-1.9.0.dist-info/top_level.txt,sha256=ioDtsrevCI52rTxZntMPljRIBsZs73tD0hI00HektiE,13
+zhmiscellany-1.9.0.dist-info/RECORD,,
```

