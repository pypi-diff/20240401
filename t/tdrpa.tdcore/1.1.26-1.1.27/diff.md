# Comparing `tmp/tdrpa.tdcore-1.1.26-py39-none-win_amd64.whl.zip` & `tmp/tdrpa.tdcore-1.1.27-py39-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,16 +1,16 @@
-Zip file size: 495802 bytes, number of entries: 14
--rw-rw-rw-  2.0 fat   640000 b- defN 24-Apr-01 05:34 tdrpa/bot.exe
--rw-rw-rw-  2.0 fat   591872 b- defN 24-Apr-01 05:34 tdrpa/tdcore.cp39-win_amd64.pyd
+Zip file size: 497875 bytes, number of entries: 14
+-rw-rw-rw-  2.0 fat   640000 b- defN 24-Apr-01 13:39 tdrpa/bot.exe
+-rw-rw-rw-  2.0 fat   594944 b- defN 24-Apr-01 13:40 tdrpa/tdcore.cp39-win_amd64.pyd
 -rw-rw-rw-  2.0 fat    11357 b- defN 23-Jan-16 01:15 tdrpa/tdcore-license/LICENSE
 -rw-rw-rw-  2.0 fat     1473 b- defN 23-Sep-05 03:08 tdrpa/tdcore-license/infi.systray/LICENSE.txt
 -rw-rw-rw-  2.0 fat     1064 b- defN 23-Sep-05 03:09 tdrpa/tdcore-license/keyboard/LICENSE.txt
 -rw-rw-rw-  2.0 fat     1548 b- defN 23-Sep-05 03:10 tdrpa/tdcore-license/psutil/LICENSE.txt
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Aug-30 09:52 tdrpa/tdcore-license/pywin32/none
 -rw-rw-rw-  2.0 fat    10142 b- defN 23-Sep-05 03:11 tdrpa/tdcore-license/requests/LICENSE.txt
 -rw-rw-rw-  2.0 fat     1060 b- defN 23-Sep-05 03:12 tdrpa/tdcore-license/tzlocal/LICENSE.txt
 -rw-rw-rw-  2.0 fat    11336 b- defN 23-Sep-05 03:13 tdrpa/tdcore-license/uiautomation/LICENSE.txt
--rw-rw-rw-  2.0 fat      638 b- defN 24-Apr-01 05:34 tdrpa.tdcore-1.1.26.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-01 05:34 tdrpa.tdcore-1.1.26.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        6 b- defN 24-Apr-01 05:34 tdrpa.tdcore-1.1.26.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     1250 b- defN 24-Apr-01 05:34 tdrpa.tdcore-1.1.26.dist-info/RECORD
-14 files, 1271838 bytes uncompressed, 493700 bytes compressed:  61.2%
+-rw-rw-rw-  2.0 fat      638 b- defN 24-Apr-01 13:40 tdrpa.tdcore-1.1.27.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-01 13:40 tdrpa.tdcore-1.1.27.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        6 b- defN 24-Apr-01 13:40 tdrpa.tdcore-1.1.27.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     1250 b- defN 24-Apr-01 13:40 tdrpa.tdcore-1.1.27.dist-info/RECORD
+14 files, 1274910 bytes uncompressed, 495773 bytes compressed:  61.1%
```

## zipnote {}

```diff
@@ -24,20 +24,20 @@
 
 Filename: tdrpa/tdcore-license/tzlocal/LICENSE.txt
 Comment: 
 
 Filename: tdrpa/tdcore-license/uiautomation/LICENSE.txt
 Comment: 
 
-Filename: tdrpa.tdcore-1.1.26.dist-info/METADATA
+Filename: tdrpa.tdcore-1.1.27.dist-info/METADATA
 Comment: 
 
-Filename: tdrpa.tdcore-1.1.26.dist-info/WHEEL
+Filename: tdrpa.tdcore-1.1.27.dist-info/WHEEL
 Comment: 
 
-Filename: tdrpa.tdcore-1.1.26.dist-info/top_level.txt
+Filename: tdrpa.tdcore-1.1.27.dist-info/top_level.txt
 Comment: 
 
-Filename: tdrpa.tdcore-1.1.26.dist-info/RECORD
+Filename: tdrpa.tdcore-1.1.27.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## tdrpa/bot.exe

### objdump

```diff
@@ -6,15 +6,15 @@
 Characteristics 0x22e
 	executable
 	line numbers stripped
 	symbols stripped
 	large address aware
 	debugging information removed
 
-Time/Date		Mon Apr  1 05:34:12 2024
+Time/Date		Mon Apr  1 13:39:57 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	2
 MinorLinkerVersion	41
 SizeOfCode		0000000000078c00
 SizeOfInitializedData	000000000009c000
 SizeOfUninitializedData	0000000000003400
 AddressOfEntryPoint	00000000000010f6
@@ -27,15 +27,15 @@
 MajorImageVersion	0
 MinorImageVersion	0
 MajorSubsystemVersion	5
 MinorSubsystemVersion	2
 Win32Version		00000000
 SizeOfImage		000a7000
 SizeOfHeaders		00000400
-CheckSum		00094cae
+CheckSum		0009be87
 Subsystem		00000002	(Windows GUI)
 DllCharacteristics	00000160
 					HIGH_ENTROPY_VA
 					DYNAMIC_BASE
 					NX_COMPAT
 SizeOfStackReserve	0000000000968000
 SizeOfStackCommit	0000000000001000
```

## Comparing `tdrpa.tdcore-1.1.26.dist-info/METADATA` & `tdrpa.tdcore-1.1.27.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tdrpa.tdcore
-Version: 1.1.26
+Version: 1.1.27
 Summary: RPA SDK for software developers. Supports Python3.7+, Windows x64
 Home-page: https://tdrpa.thingswell.cn
 Author: tdrpa
 Author-email: armstrong.wang@gmail.com
 License: Apache 2.0
 Keywords: RPA,tdRPA,uiautomation,uia
 Platform: Windows Only
```

