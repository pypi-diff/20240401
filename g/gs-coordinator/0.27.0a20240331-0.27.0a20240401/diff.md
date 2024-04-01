# Comparing `tmp/gs_coordinator-0.27.0a20240331-py2.py3-none-macosx_12_0_x86_64.whl.zip` & `tmp/gs_coordinator-0.27.0a20240401-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,50 +1,40 @@
-Zip file size: 102179 bytes, number of entries: 48
-drwxr-xr-x  2.0 unx        0 b- stor 24-Mar-31 20:57 graphscope_runtime/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Mar-31 20:57 gs_coordinator-0.27.0a20240331.dist-info/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Mar-31 20:57 gscoordinator/
--rw-r--r--  2.0 unx      694 b- defN 24-Mar-31 19:45 graphscope_runtime/__init__.py
--rw-rw-r--  2.0 unx     3451 b- defN 24-Mar-31 20:57 gs_coordinator-0.27.0a20240331.dist-info/RECORD
--rw-r--r--  2.0 unx      140 b- defN 24-Mar-31 20:50 gs_coordinator-0.27.0a20240331.dist-info/WHEEL
--rw-r--r--  2.0 unx       33 b- defN 24-Mar-31 20:50 gs_coordinator-0.27.0a20240331.dist-info/top_level.txt
--rw-r--r--  2.0 unx    23840 b- defN 24-Mar-31 20:50 gs_coordinator-0.27.0a20240331.dist-info/METADATA
-drwxr-xr-x  2.0 unx        0 b- stor 24-Mar-31 20:57 gscoordinator/template/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Mar-31 20:57 gscoordinator/servicer/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Mar-31 20:57 gscoordinator/builtin/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Mar-31 20:57 gscoordinator/hook/
--rw-r--r--  2.0 unx    54960 b- defN 24-Mar-31 19:45 gscoordinator/kubernetes_launcher.py
--rw-r--r--  2.0 unx     5450 b- defN 24-Mar-31 19:45 gscoordinator/coordinator.py
--rw-r--r--  2.0 unx     5702 b- defN 24-Mar-31 19:45 gscoordinator/dag_manager.py
--rw-r--r--  2.0 unx     1045 b- defN 24-Mar-31 19:45 gscoordinator/version.py
--rw-r--r--  2.0 unx     6950 b- defN 24-Mar-31 19:45 gscoordinator/monitor.py
--rw-r--r--  2.0 unx    43296 b- defN 24-Mar-31 19:45 gscoordinator/op_executor.py
--rw-r--r--  2.0 unx     2653 b- defN 24-Mar-31 19:45 gscoordinator/object_manager.py
--rw-r--r--  2.0 unx     4351 b- defN 24-Mar-31 19:45 gscoordinator/operator_launcher.py
--rw-r--r--  2.0 unx      343 b- defN 24-Mar-31 19:45 gscoordinator/constants.py
--rw-r--r--  2.0 unx      990 b- defN 24-Mar-31 19:45 gscoordinator/__init__.py
--rw-r--r--  2.0 unx    21916 b- defN 24-Mar-31 19:45 gscoordinator/cluster_builder.py
--rw-r--r--  2.0 unx    22198 b- defN 24-Mar-31 19:45 gscoordinator/local_launcher.py
--rw-r--r--  2.0 unx     2975 b- defN 24-Mar-31 19:45 gscoordinator/launch_graphlearn_torch.py
--rw-r--r--  2.0 unx       16 b- defN 24-Mar-31 19:51 gscoordinator/VERSION
--rw-r--r--  2.0 unx    80235 b- defN 24-Mar-31 19:45 gscoordinator/utils.py
--rw-r--r--  2.0 unx     4091 b- defN 24-Mar-31 19:45 gscoordinator/io_utils.py
--rw-r--r--  2.0 unx     5372 b- defN 24-Mar-31 19:45 gscoordinator/launcher.py
--rw-r--r--  2.0 unx     2494 b- defN 24-Mar-31 19:45 gscoordinator/launch_graphlearn.py
--rw-r--r--  2.0 unx       77 b- defN 24-Mar-31 19:45 gscoordinator/__main__.py
--rw-r--r--  2.0 unx      646 b- defN 24-Mar-31 19:45 gscoordinator/template/__init__.py
--rw-r--r--  2.0 unx     4340 b- defN 24-Mar-31 19:45 gscoordinator/template/pregel.pxd.template
--rw-r--r--  2.0 unx     4957 b- defN 24-Mar-31 19:45 gscoordinator/template/pie.pxd.template
--rw-r--r--  2.0 unx    22656 b- defN 24-Mar-31 19:45 gscoordinator/template/CMakeLists.template
-drwxr-xr-x  2.0 unx        0 b- stor 24-Mar-31 20:57 gscoordinator/servicer/graphscope_one/
--rw-r--r--  2.0 unx      707 b- defN 24-Mar-31 19:45 gscoordinator/servicer/__init__.py
--rw-r--r--  2.0 unx    24792 b- defN 24-Mar-31 19:45 gscoordinator/servicer/graphscope_one/service.py
--rw-r--r--  2.0 unx      646 b- defN 24-Mar-31 19:45 gscoordinator/servicer/graphscope_one/__init__.py
-drwxr-xr-x  2.0 unx        0 b- stor 24-Mar-31 20:57 gscoordinator/builtin/app/
--rw-r--r--  2.0 unx      646 b- defN 24-Mar-31 19:45 gscoordinator/builtin/__init__.py
--rw-r--r--  2.0 unx    25282 b- defN 24-Mar-31 19:45 gscoordinator/builtin/app/.gs_conf.yaml
--rw-r--r--  2.0 unx     5715 b- defN 24-Mar-31 20:50 gscoordinator/builtin/app/builtin_app.gar
--rw-r--r--  2.0 unx      646 b- defN 24-Mar-31 19:45 gscoordinator/builtin/app/__init__.py
-drwxr-xr-x  2.0 unx        0 b- stor 24-Mar-31 20:57 gscoordinator/hook/prestop/
--rw-r--r--  2.0 unx      646 b- defN 24-Mar-31 19:45 gscoordinator/hook/__init__.py
--rw-r--r--  2.0 unx      646 b- defN 24-Mar-31 19:45 gscoordinator/hook/prestop/__init__.py
--rw-r--r--  2.0 unx     1560 b- defN 24-Mar-31 19:45 gscoordinator/hook/prestop/__main__.py
-48 files, 387157 bytes uncompressed, 95387 bytes compressed:  75.4%
+Zip file size: 100902 bytes, number of entries: 38
+-rw-r--r--  2.0 unx      694 b- defN 24-Apr-01 19:01 graphscope_runtime/__init__.py
+-rw-r--r--  2.0 unx       16 b- defN 24-Apr-01 19:03 gscoordinator/VERSION
+-rw-r--r--  2.0 unx      990 b- defN 24-Apr-01 19:01 gscoordinator/__init__.py
+-rw-r--r--  2.0 unx       77 b- defN 24-Apr-01 19:01 gscoordinator/__main__.py
+-rw-r--r--  2.0 unx    21916 b- defN 24-Apr-01 19:01 gscoordinator/cluster_builder.py
+-rw-r--r--  2.0 unx      343 b- defN 24-Apr-01 19:01 gscoordinator/constants.py
+-rw-r--r--  2.0 unx     5450 b- defN 24-Apr-01 19:01 gscoordinator/coordinator.py
+-rw-r--r--  2.0 unx     5702 b- defN 24-Apr-01 19:01 gscoordinator/dag_manager.py
+-rw-r--r--  2.0 unx     4091 b- defN 24-Apr-01 19:01 gscoordinator/io_utils.py
+-rw-r--r--  2.0 unx    54960 b- defN 24-Apr-01 19:01 gscoordinator/kubernetes_launcher.py
+-rw-r--r--  2.0 unx     2494 b- defN 24-Apr-01 19:01 gscoordinator/launch_graphlearn.py
+-rw-r--r--  2.0 unx     2975 b- defN 24-Apr-01 19:01 gscoordinator/launch_graphlearn_torch.py
+-rw-r--r--  2.0 unx     5372 b- defN 24-Apr-01 19:01 gscoordinator/launcher.py
+-rw-r--r--  2.0 unx    22198 b- defN 24-Apr-01 19:01 gscoordinator/local_launcher.py
+-rw-r--r--  2.0 unx     6950 b- defN 24-Apr-01 19:01 gscoordinator/monitor.py
+-rw-r--r--  2.0 unx     2653 b- defN 24-Apr-01 19:01 gscoordinator/object_manager.py
+-rw-r--r--  2.0 unx    43296 b- defN 24-Apr-01 19:01 gscoordinator/op_executor.py
+-rw-r--r--  2.0 unx     4351 b- defN 24-Apr-01 19:01 gscoordinator/operator_launcher.py
+-rw-r--r--  2.0 unx    80235 b- defN 24-Apr-01 19:01 gscoordinator/utils.py
+-rw-r--r--  2.0 unx     1045 b- defN 24-Apr-01 19:01 gscoordinator/version.py
+-rw-r--r--  2.0 unx      646 b- defN 24-Apr-01 19:01 gscoordinator/builtin/__init__.py
+-rw-r--r--  2.0 unx    25282 b- defN 24-Apr-01 19:01 gscoordinator/builtin/app/.gs_conf.yaml
+-rw-r--r--  2.0 unx      646 b- defN 24-Apr-01 19:01 gscoordinator/builtin/app/__init__.py
+-rw-r--r--  2.0 unx     5264 b- defN 24-Apr-01 20:00 gscoordinator/builtin/app/builtin_app.gar
+-rw-r--r--  2.0 unx      646 b- defN 24-Apr-01 19:01 gscoordinator/hook/__init__.py
+-rw-r--r--  2.0 unx      646 b- defN 24-Apr-01 19:01 gscoordinator/hook/prestop/__init__.py
+-rw-r--r--  2.0 unx     1560 b- defN 24-Apr-01 19:01 gscoordinator/hook/prestop/__main__.py
+-rw-r--r--  2.0 unx      707 b- defN 24-Apr-01 19:01 gscoordinator/servicer/__init__.py
+-rw-r--r--  2.0 unx      646 b- defN 24-Apr-01 19:01 gscoordinator/servicer/graphscope_one/__init__.py
+-rw-r--r--  2.0 unx    24792 b- defN 24-Apr-01 19:01 gscoordinator/servicer/graphscope_one/service.py
+-rw-r--r--  2.0 unx    22656 b- defN 24-Apr-01 19:01 gscoordinator/template/CMakeLists.template
+-rw-r--r--  2.0 unx      646 b- defN 24-Apr-01 19:01 gscoordinator/template/__init__.py
+-rw-r--r--  2.0 unx     4957 b- defN 24-Apr-01 19:01 gscoordinator/template/pie.pxd.template
+-rw-r--r--  2.0 unx     4340 b- defN 24-Apr-01 19:01 gscoordinator/template/pregel.pxd.template
+-rw-r--r--  2.0 unx    23840 b- defN 24-Apr-01 20:00 gs_coordinator-0.27.0a20240401.dist-info/METADATA
+-rw-r--r--  2.0 unx      110 b- defN 24-Apr-01 20:00 gs_coordinator-0.27.0a20240401.dist-info/WHEEL
+-rw-r--r--  2.0 unx       33 b- defN 24-Apr-01 20:00 gs_coordinator-0.27.0a20240401.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     3413 b- defN 24-Apr-01 20:00 gs_coordinator-0.27.0a20240401.dist-info/RECORD
+38 files, 386638 bytes uncompressed, 95374 bytes compressed:  75.3%
```

## zipnote {}

```diff
@@ -1,145 +1,115 @@
-Filename: graphscope_runtime/
-Comment: 
-
-Filename: gs_coordinator-0.27.0a20240331.dist-info/
-Comment: 
-
-Filename: gscoordinator/
-Comment: 
-
 Filename: graphscope_runtime/__init__.py
 Comment: 
 
-Filename: gs_coordinator-0.27.0a20240331.dist-info/RECORD
-Comment: 
-
-Filename: gs_coordinator-0.27.0a20240331.dist-info/WHEEL
-Comment: 
-
-Filename: gs_coordinator-0.27.0a20240331.dist-info/top_level.txt
-Comment: 
-
-Filename: gs_coordinator-0.27.0a20240331.dist-info/METADATA
-Comment: 
-
-Filename: gscoordinator/template/
+Filename: gscoordinator/VERSION
 Comment: 
 
-Filename: gscoordinator/servicer/
+Filename: gscoordinator/__init__.py
 Comment: 
 
-Filename: gscoordinator/builtin/
+Filename: gscoordinator/__main__.py
 Comment: 
 
-Filename: gscoordinator/hook/
+Filename: gscoordinator/cluster_builder.py
 Comment: 
 
-Filename: gscoordinator/kubernetes_launcher.py
+Filename: gscoordinator/constants.py
 Comment: 
 
 Filename: gscoordinator/coordinator.py
 Comment: 
 
 Filename: gscoordinator/dag_manager.py
 Comment: 
 
-Filename: gscoordinator/version.py
-Comment: 
-
-Filename: gscoordinator/monitor.py
+Filename: gscoordinator/io_utils.py
 Comment: 
 
-Filename: gscoordinator/op_executor.py
+Filename: gscoordinator/kubernetes_launcher.py
 Comment: 
 
-Filename: gscoordinator/object_manager.py
+Filename: gscoordinator/launch_graphlearn.py
 Comment: 
 
-Filename: gscoordinator/operator_launcher.py
+Filename: gscoordinator/launch_graphlearn_torch.py
 Comment: 
 
-Filename: gscoordinator/constants.py
+Filename: gscoordinator/launcher.py
 Comment: 
 
-Filename: gscoordinator/__init__.py
+Filename: gscoordinator/local_launcher.py
 Comment: 
 
-Filename: gscoordinator/cluster_builder.py
+Filename: gscoordinator/monitor.py
 Comment: 
 
-Filename: gscoordinator/local_launcher.py
+Filename: gscoordinator/object_manager.py
 Comment: 
 
-Filename: gscoordinator/launch_graphlearn_torch.py
+Filename: gscoordinator/op_executor.py
 Comment: 
 
-Filename: gscoordinator/VERSION
+Filename: gscoordinator/operator_launcher.py
 Comment: 
 
 Filename: gscoordinator/utils.py
 Comment: 
 
-Filename: gscoordinator/io_utils.py
-Comment: 
-
-Filename: gscoordinator/launcher.py
+Filename: gscoordinator/version.py
 Comment: 
 
-Filename: gscoordinator/launch_graphlearn.py
+Filename: gscoordinator/builtin/__init__.py
 Comment: 
 
-Filename: gscoordinator/__main__.py
+Filename: gscoordinator/builtin/app/.gs_conf.yaml
 Comment: 
 
-Filename: gscoordinator/template/__init__.py
+Filename: gscoordinator/builtin/app/__init__.py
 Comment: 
 
-Filename: gscoordinator/template/pregel.pxd.template
+Filename: gscoordinator/builtin/app/builtin_app.gar
 Comment: 
 
-Filename: gscoordinator/template/pie.pxd.template
+Filename: gscoordinator/hook/__init__.py
 Comment: 
 
-Filename: gscoordinator/template/CMakeLists.template
+Filename: gscoordinator/hook/prestop/__init__.py
 Comment: 
 
-Filename: gscoordinator/servicer/graphscope_one/
+Filename: gscoordinator/hook/prestop/__main__.py
 Comment: 
 
 Filename: gscoordinator/servicer/__init__.py
 Comment: 
 
-Filename: gscoordinator/servicer/graphscope_one/service.py
-Comment: 
-
 Filename: gscoordinator/servicer/graphscope_one/__init__.py
 Comment: 
 
-Filename: gscoordinator/builtin/app/
+Filename: gscoordinator/servicer/graphscope_one/service.py
 Comment: 
 
-Filename: gscoordinator/builtin/__init__.py
+Filename: gscoordinator/template/CMakeLists.template
 Comment: 
 
-Filename: gscoordinator/builtin/app/.gs_conf.yaml
+Filename: gscoordinator/template/__init__.py
 Comment: 
 
-Filename: gscoordinator/builtin/app/builtin_app.gar
+Filename: gscoordinator/template/pie.pxd.template
 Comment: 
 
-Filename: gscoordinator/builtin/app/__init__.py
+Filename: gscoordinator/template/pregel.pxd.template
 Comment: 
 
-Filename: gscoordinator/hook/prestop/
+Filename: gs_coordinator-0.27.0a20240401.dist-info/METADATA
 Comment: 
 
-Filename: gscoordinator/hook/__init__.py
+Filename: gs_coordinator-0.27.0a20240401.dist-info/WHEEL
 Comment: 
 
-Filename: gscoordinator/hook/prestop/__init__.py
+Filename: gs_coordinator-0.27.0a20240401.dist-info/top_level.txt
 Comment: 
 
-Filename: gscoordinator/hook/prestop/__main__.py
+Filename: gs_coordinator-0.27.0a20240401.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## filetype from file(1)

```diff
@@ -1 +1 @@
-Zip archive data, at least v2.0 to extract, compression method=store
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## gscoordinator/VERSION

```diff
@@ -1 +1 @@
-0.27.0a20240331
+0.27.0a20240401
```

## gscoordinator/builtin/app/builtin_app.gar

### zipinfo {}

```diff
@@ -1,5 +1,5 @@
-Zip file size: 5715 bytes, number of entries: 3
--rw-r--r--  2.0 unx    25282 b- defN 24-Mar-31 19:45 .gs_conf.yaml
--rw-r--r--  2.0 unx      646 b- defN 24-Mar-31 19:45 __init__.py
--rw-r--r--  2.0 unx     2733 b- defN 24-Mar-31 20:50 builtin_app.zip
-3 files, 28661 bytes uncompressed, 5387 bytes compressed:  81.2%
+Zip file size: 5264 bytes, number of entries: 3
+-rw-r--r--  2.0 unx    25282 b- defN 24-Apr-02 03:01 .gs_conf.yaml
+-rw-r--r--  2.0 unx     2282 b- defN 24-Apr-02 04:00 builtin_app.zip
+-rw-r--r--  2.0 unx      646 b- defN 24-Apr-02 03:01 __init__.py
+3 files, 28210 bytes uncompressed, 4936 bytes compressed:  82.5%
```

### zipnote «TEMP»/diffoscope_e3ey3vpx_/tmpf6m0b231_.zip

```diff
@@ -1,10 +1,10 @@
 Filename: .gs_conf.yaml
 Comment: 
 
-Filename: __init__.py
+Filename: builtin_app.zip
 Comment: 
 
-Filename: builtin_app.zip
+Filename: __init__.py
 Comment: 
 
 Zip file comment:
```

### builtin_app.zip

 * *Command `'zipinfo {}'` failed with exit code 9. Standard output:*

 * *    Archive:  /tmp/diffoscope_e3ey3vpx_/tmpfjebi5ct_ZipContainer/builtin_app.zip*

 * *    […]*

 * *Archive contents identical but files differ, possibly due to different compression levels. Falling back to binary comparison.*

```diff
@@ -1,8 +1,8 @@
-00000000: 504b 0304 1400 0000 0800 a39d 7f58 f458  PK...........X.X
+00000000: 504b 0304 1400 0000 0800 3a18 8258 f458  PK........:..X.X
 00000010: 240e bf08 0000 c262 0000 0d00 0000 2e67  $......b.......g
 00000020: 735f 636f 6e66 2e79 616d 6ccd 9c5b 739b  s_conf.yaml..[s.
 00000030: 3814 80df f757 e40f b0cc a46f 7973 48b3  8....W.....oysH.
 00000040: cd34 693d 71ba bbb3 2f8c 0c8a ad8d 0c2c  .4i=q.../......,
 00000050: 126e dd5f bf47 0299 8b01 1fd9 a9c5 431c  .n._.G........C.
 00000060: 8fd1 b97c 3aba 1c09 01c9 b29b dfae aebc  ...|:...........
 00000070: 2bc2 57e9 cd55 4656 3427 c91b fc74 7525  +.W..UFV4'...tu%
@@ -136,36 +136,8 @@
 00000870: 2125 402b ac1e 5f08 826f c71e 6068 a369  !%@+.._..o..`h.i
 00000880: f56e b6d0 6df6 d0b1 63fb d2cd e00e 662d  .n..m...c.....f-
 00000890: eeea 00ce e813 4f6d 1e37 3774 8445 7816  ......Om.77t.Ex.
 000008a0: e8f0 0837 e111 56e1 59e0 c323 5c85 6799  ...7..V.Y..#\.g.
 000008b0: 3350 826f 71ba 38b6 cde9 c2ee a86c 7a92  3P.oq.8......lz.
 000008c0: 1640 7726 5dda 4dc0 403c cc52 9658 6414  .@w&].M.@<.R.Xd.
 000008d0: 859c 2b01 ec58 5e48 4f1b 704a 67f3 e067  ..+..X^HO.pJg..g
-000008e0: c587 8dde 1ef0 2201 fc1f 504b 0304 1400  ......"...PK....
-000008f0: 0000 0800 a39d 7f58 7cbd 2df0 9a01 0000  .......X|.-.....
-00000900: 8602 0000 0b00 0000 5f5f 696e 6974 5f5f  ........__init__
-00000910: 2e70 7965 9241 6fdb 300c 85ef fd15 6fc9  .pye.Ao.0.....o.
-00000920: 651b 9238 c82e 4377 f2d2 6c35 1638 409c  e..8..Cw..l5.8@.
-00000930: aee8 51b6 699b 8023 6992 5c37 ff7e 949b  ..Q.i..#i.\7.~..
-00000940: 012d a68b 20f1 f1e9 23a9 f907 2483 7749  .-.. ...#...$.wI
-00000950: c93a 21fd 0c7b 099d d15f 6ee6 587e 5ea2  .:!..{..._n.X~^.
-00000960: 3235 ebf6 1643 6896 5fe3 cdcd 5c22 5b63  25...Ch._...\"[c
-00000970: 2f8e db2e 60b3 deac 91f6 5caa 52e1 a733  /...`.....\.R..3
-00000980: 83c5 bde9 630e f67c e640 f56a cad8 7345  ....c..|.@.j..sE
-00000990: da53 8d41 d7e4 103a 426a 5525 db35 b2c0  .S.A...:BjU%.5..
-000009a0: 6f72 9e8d c666 b5c6 c728 985d 43b3 4fdf  or...f...(.]C.O.
-000009b0: c4e1 6206 9cd5 05da 040c 9ec4 823d 1aee  ..b..........=..
-000009c0: 09f4 5291 0d60 2db4 67db b3d2 1561 e4d0  ..R..`-.g....a..
-000009d0: 4dcf 5c4d 0403 4f57 0b53 0625 6a25 7a2b  M.\M..OW.S.%j%z+
-000009e0: a7e6 ad0e 2a4c c071 7521 d8db 2419 c771  ....*L.qu!..$..q
-000009f0: a526 d895 716d d2bf 0a7d b2cf b6bb bcd8  .&..qm...}......
-00000a00: 2d05 784a 79d0 3d79 0f47 7f06 7652 6a79  -.xJy.=y.G..vRjy
-00000a10: 81b2 c253 a952 287b 35c2 38a8 d691 c482  ...S.R({5.8.....
-00000a20: 89bc a3e3 20ad 5ac0 9b26 8cca 91b8 d4ec  .... .Z..&......
-00000a30: 83e3 7208 ef9a f58f 4e6a 7e2b 9076 298d  ..r.....Nj~+.v).
-00000a40: 595a 202b 66f8 9e16 59b1 108f c7ec 747f  YZ +f...Y.....t.
-00000a50: 7838 e131 3d1e d3fc 94ed 0a1c 8ed8 1ef2  x8.1=...........
-00000a60: bbec 941d 7239 fd40 9a3f e157 96df 2d40  ....r9.@.?.W..-@
-00000a70: d22a 7986 5eac 8bfc 02c9 b18d d3e8 5010  .*y.^.........P.
-00000a80: bd03 68cc 2b90 b754 71c3 95d4 a5db 41b5  ..h.+..Tq.....A.
-00000a90: 84d6 3c93 d371 f296 dc99 7d1c a617 bc5a  ..<..q....}....Z
-00000aa0: 5cfa f817 5498 6efe 2b2a fe90 bf         \...T.n.+*...
+000008e0: c587 8dde 1ef0 2201 fc1f                 ......"...
```

#### builtin_app.zip

```diff
@@ -1,8 +1,8 @@
-00000000: 504b 0304 1400 0000 0800 a39d 7f58 f458  PK...........X.X
+00000000: 504b 0304 1400 0000 0800 3a18 8258 f458  PK........:..X.X
 00000010: 240e bf08 0000 c262 0000 0d00 0000 2e67  $......b.......g
 00000020: 735f 636f 6e66 2e79 616d 6ccd 9c5b 739b  s_conf.yaml..[s.
 00000030: 3814 80df f757 e40f b0cc a46f 7973 48b3  8....W.....oysH.
 00000040: cd34 693d 71ba bbb3 2f8c 0c8a ad8d 0c2c  .4i=q.../......,
 00000050: 126e dd5f bf47 0299 8b01 1fd9 a9c5 431c  .n._.G........C.
 00000060: 8fd1 b97c 3aba 1c09 01c9 b29b dfae aebc  ...|:...........
 00000070: 2bc2 57e9 cd55 4656 3427 c91b fc74 7525  +.W..UFV4'...tu%
@@ -136,36 +136,8 @@
 00000870: 2125 402b ac1e 5f08 826f c71e 6068 a369  !%@+.._..o..`h.i
 00000880: f56e b6d0 6df6 d0b1 63fb d2cd e00e 662d  .n..m...c.....f-
 00000890: eeea 00ce e813 4f6d 1e37 3774 8445 7816  ......Om.77t.Ex.
 000008a0: e8f0 0837 e111 56e1 59e0 c323 5c85 6799  ...7..V.Y..#\.g.
 000008b0: 3350 826f 71ba 38b6 cde9 c2ee a86c 7a92  3P.oq.8......lz.
 000008c0: 1640 7726 5dda 4dc0 403c cc52 9658 6414  .@w&].M.@<.R.Xd.
 000008d0: 859c 2b01 ec58 5e48 4f1b 704a 67f3 e067  ..+..X^HO.pJg..g
-000008e0: c587 8dde 1ef0 2201 fc1f 504b 0304 1400  ......"...PK....
-000008f0: 0000 0800 a39d 7f58 7cbd 2df0 9a01 0000  .......X|.-.....
-00000900: 8602 0000 0b00 0000 5f5f 696e 6974 5f5f  ........__init__
-00000910: 2e70 7965 9241 6fdb 300c 85ef fd15 6fc9  .pye.Ao.0.....o.
-00000920: 651b 9238 c82e 4377 f2d2 6c35 1638 409c  e..8..Cw..l5.8@.
-00000930: aee8 51b6 699b 8023 6992 5c37 ff7e 949b  ..Q.i..#i.\7.~..
-00000940: 012d a68b 20f1 f1e9 23a9 f907 2483 7749  .-.. ...#...$.wI
-00000950: c93a 21fd 0c7b 099d d15f 6ee6 587e 5ea2  .:!..{..._n.X~^.
-00000960: 3235 ebf6 1643 6896 5fe3 cdcd 5c22 5b63  25...Ch._...\"[c
-00000970: 2f8e db2e 60b3 deac 91f6 5caa 52e1 a733  /...`.....\.R..3
-00000980: 83c5 bde9 630e f67c e640 f56a cad8 7345  ....c..|.@.j..sE
-00000990: da53 8d41 d7e4 103a 426a 5525 db35 b2c0  .S.A...:BjU%.5..
-000009a0: 6f72 9e8d c666 b5c6 c728 985d 43b3 4fdf  or...f...(.]C.O.
-000009b0: c4e1 6206 9cd5 05da 040c 9ec4 823d 1aee  ..b..........=..
-000009c0: 09f4 5291 0d60 2db4 67db b3d2 1561 e4d0  ..R..`-.g....a..
-000009d0: 4dcf 5c4d 0403 4f57 0b53 0625 6a25 7a2b  M.\M..OW.S.%j%z+
-000009e0: a7e6 ad0e 2a4c c071 7521 d8db 2419 c771  ....*L.qu!..$..q
-000009f0: a526 d895 716d d2bf 0a7d b2cf b6bb bcd8  .&..qm...}......
-00000a00: 2d05 784a 79d0 3d79 0f47 7f06 7652 6a79  -.xJy.=y.G..vRjy
-00000a10: 81b2 c253 a952 287b 35c2 38a8 d691 c482  ...S.R({5.8.....
-00000a20: 89bc a3e3 20ad 5ac0 9b26 8cca 91b8 d4ec  .... .Z..&......
-00000a30: 83e3 7208 ef9a f58f 4e6a 7e2b 9076 298d  ..r.....Nj~+.v).
-00000a40: 595a 202b 66f8 9e16 59b1 108f c7ec 747f  YZ +f...Y.....t.
-00000a50: 7838 e131 3d1e d3fc 94ed 0a1c 8ed8 1ef2  x8.1=...........
-00000a60: bbec 941d 7239 fd40 9a3f e157 96df 2d40  ....r9.@.?.W..-@
-00000a70: d22a 7986 5eac 8bfc 02c9 b18d d3e8 5010  .*y.^.........P.
-00000a80: bd03 68cc 2b90 b754 71c3 95d4 a5db 41b5  ..h.+..Tq.....A.
-00000a90: 84d6 3c93 d371 f296 dc99 7d1c a617 bc5a  ..<..q....}....Z
-00000aa0: 5cfa f817 5498 6efe 2b2a fe90 bf         \...T.n.+*...
+000008e0: c587 8dde 1ef0 2201 fc1f                 ......"...
```

## Comparing `gs_coordinator-0.27.0a20240331.dist-info/RECORD` & `gs_coordinator-0.27.0a20240401.dist-info/RECORD`

 * *Files 13% similar despite different names*

```diff
@@ -1,38 +1,38 @@
-graphscope_runtime/__init__.py,sha256=w_Me0NHI5zy8GitMCD7mzOi0Qz7ZfeE2zUI5wGfZIyM,694
-gs_coordinator-0.27.0a20240331.dist-info/RECORD,,
-gs_coordinator-0.27.0a20240331.dist-info/WHEEL,sha256=EACXjPwsYzxTpWW_PsZniqQc4RzZfXb_Ir_SpN_ifuM,140
-gs_coordinator-0.27.0a20240331.dist-info/top_level.txt,sha256=GiJfpWt7WpC-H1BxUy5V39G7WAtPut6eqH3yAciJhqQ,33
-gs_coordinator-0.27.0a20240331.dist-info/METADATA,sha256=9_b0FLasTDRHv0mzDvpCxsxLFsKtNkhqnnwoLQ5-vag,23840
-gscoordinator/kubernetes_launcher.py,sha256=8cvqbR2M_l5ppj25B9OvaBw4dyaK-Ez7XSN7Sd-ZBMI,54960
-gscoordinator/coordinator.py,sha256=JxvRRQVngJD5jT014qgMdrlIS4XBBLSG5NjXcCJvQ2E,5450
-gscoordinator/dag_manager.py,sha256=qA88ACSe97ANR02viegLksZ3vkVJdASK_hsNVZj9ieg,5702
-gscoordinator/version.py,sha256=bS71qRjwM-xk4LAFTExdiWJOaJEXaeNdlJYCAqtD98U,1045
-gscoordinator/monitor.py,sha256=8nfT_UfQ8UeYGqpNDxoK0Dw9vWTbVSI-W6pFZy4Lq0A,6950
-gscoordinator/op_executor.py,sha256=x59Mrg9wOfyFT7nRuizc21DESo_KTOllnQpGEninxrk,43296
-gscoordinator/object_manager.py,sha256=e-5KcWigw8VM9o1WSMZ9BIQHIATvWD4gCXfiZVjPR6U,2653
-gscoordinator/operator_launcher.py,sha256=e9LuVPw3gfUFHxjO0vYuthpAMgCI0TYWOWbTE8yxD6s,4351
-gscoordinator/constants.py,sha256=FxXDGCJ6vQ9LyKBGUW45jvdlRPRgtQkwxTuqh1S3tBQ,343
-gscoordinator/__init__.py,sha256=nUqENyB6dtqMgYfbJjblAdV2nemmlsaTMp_yTteBnOw,990
-gscoordinator/cluster_builder.py,sha256=RE29hMZIGiyQpA0xagzs9hggQ6en61uMdR7KbnCDoqI,21916
-gscoordinator/local_launcher.py,sha256=8zx3bxaB9pQUv4X07-hq-IpoSllOUxNCMJNvvDWuSOo,22198
-gscoordinator/launch_graphlearn_torch.py,sha256=euyryABQwNKAm0OpguRpn6EZNA20j6f0xVFa-KukRwE,2975
-gscoordinator/VERSION,sha256=lmi4wa9gUnxUhUMNFEU5YSFKPP-hZOoT5NzuNHSx8Zg,16
-gscoordinator/utils.py,sha256=orWfdjfQ3NL5ex6XB1VvfBhxyOqlRFR6OSMOE3jgmcE,80235
-gscoordinator/io_utils.py,sha256=8lxUPh-DfBj4yPIAPY9ovv2Iweg7MG8V77LscRlPM8o,4091
-gscoordinator/launcher.py,sha256=Nn6zrfo1ycuB-Msj5_Slx9MDQO8C2Zqd6_-MpJXiQA0,5372
-gscoordinator/launch_graphlearn.py,sha256=91UC3ECqfVLbF4nsxYxORWLiHGRTjbVMjwiRNM9ZjLI,2494
-gscoordinator/__main__.py,sha256=pfC-UJ0gz8i-p1lGAs2jBB8zALAz6PaBokLa9v6AYQ4,77
-gscoordinator/template/__init__.py,sha256=TsAsMQRDcEJ9nRXDAeF-pJPapJrZPwVeb-TxxVp42aY,646
-gscoordinator/template/pregel.pxd.template,sha256=Eh4tESR8KlmM30Mcw-eIUfiQNeadDj3WWGCUzkIsT2M,4340
-gscoordinator/template/pie.pxd.template,sha256=-hYphyhUzTnyQELecGEsCK_S-fEXLWGiTV91-gDqAU8,4957
-gscoordinator/template/CMakeLists.template,sha256=EqTx-5CWuZ6bf6lUhGZ8Hwu6s3AANu-cScKpjxm4ndw,22656
-gscoordinator/servicer/__init__.py,sha256=i0VzRn8z0PsDlQj3oZzOsii2qVSk-vcZQzFtbse9fVo,707
-gscoordinator/servicer/graphscope_one/service.py,sha256=IS1zquyYhLBn4dSGyYCNJz1GKuz5EHO4ityrvG5JHD4,24792
-gscoordinator/servicer/graphscope_one/__init__.py,sha256=hSEiV3pYv8wKgo6KzUx0p4563wJ1on2osrFZxZ4pT2o,646
-gscoordinator/builtin/__init__.py,sha256=TsAsMQRDcEJ9nRXDAeF-pJPapJrZPwVeb-TxxVp42aY,646
-gscoordinator/builtin/app/.gs_conf.yaml,sha256=gWoCXtVzGb1xks9ioQ5WfYMnFPRJGiq9Cb-w3oF8SVA,25282
-gscoordinator/builtin/app/builtin_app.gar,sha256=mFPp2fpfk2xv_d-_9sBS5QJaarqME-f2_2AmYuNDe38,5715
-gscoordinator/builtin/app/__init__.py,sha256=TsAsMQRDcEJ9nRXDAeF-pJPapJrZPwVeb-TxxVp42aY,646
-gscoordinator/hook/__init__.py,sha256=jzzLJxC1gBgRLMb4xzX6vucYuNdosuWOtZKRj7Cal_o,646
-gscoordinator/hook/prestop/__init__.py,sha256=jzzLJxC1gBgRLMb4xzX6vucYuNdosuWOtZKRj7Cal_o,646
-gscoordinator/hook/prestop/__main__.py,sha256=1FmS0g2hwl85NPMOtbAvW_IGn4GFnldmjbSSwaj9GrE,1560
+graphscope_runtime/__init__.py,sha256=w_Me0NHI5zy8GitMCD7mzOi0Qz7ZfeE2zUI5wGfZIyM,694
+gscoordinator/VERSION,sha256=5H8IfbvFQA3D2DxKwtgeI7teV2KusNJ7E4pjycDcyQE,16
+gscoordinator/__init__.py,sha256=nUqENyB6dtqMgYfbJjblAdV2nemmlsaTMp_yTteBnOw,990
+gscoordinator/__main__.py,sha256=pfC-UJ0gz8i-p1lGAs2jBB8zALAz6PaBokLa9v6AYQ4,77
+gscoordinator/cluster_builder.py,sha256=RE29hMZIGiyQpA0xagzs9hggQ6en61uMdR7KbnCDoqI,21916
+gscoordinator/constants.py,sha256=FxXDGCJ6vQ9LyKBGUW45jvdlRPRgtQkwxTuqh1S3tBQ,343
+gscoordinator/coordinator.py,sha256=JxvRRQVngJD5jT014qgMdrlIS4XBBLSG5NjXcCJvQ2E,5450
+gscoordinator/dag_manager.py,sha256=qA88ACSe97ANR02viegLksZ3vkVJdASK_hsNVZj9ieg,5702
+gscoordinator/io_utils.py,sha256=8lxUPh-DfBj4yPIAPY9ovv2Iweg7MG8V77LscRlPM8o,4091
+gscoordinator/kubernetes_launcher.py,sha256=8cvqbR2M_l5ppj25B9OvaBw4dyaK-Ez7XSN7Sd-ZBMI,54960
+gscoordinator/launch_graphlearn.py,sha256=91UC3ECqfVLbF4nsxYxORWLiHGRTjbVMjwiRNM9ZjLI,2494
+gscoordinator/launch_graphlearn_torch.py,sha256=euyryABQwNKAm0OpguRpn6EZNA20j6f0xVFa-KukRwE,2975
+gscoordinator/launcher.py,sha256=Nn6zrfo1ycuB-Msj5_Slx9MDQO8C2Zqd6_-MpJXiQA0,5372
+gscoordinator/local_launcher.py,sha256=8zx3bxaB9pQUv4X07-hq-IpoSllOUxNCMJNvvDWuSOo,22198
+gscoordinator/monitor.py,sha256=8nfT_UfQ8UeYGqpNDxoK0Dw9vWTbVSI-W6pFZy4Lq0A,6950
+gscoordinator/object_manager.py,sha256=e-5KcWigw8VM9o1WSMZ9BIQHIATvWD4gCXfiZVjPR6U,2653
+gscoordinator/op_executor.py,sha256=x59Mrg9wOfyFT7nRuizc21DESo_KTOllnQpGEninxrk,43296
+gscoordinator/operator_launcher.py,sha256=e9LuVPw3gfUFHxjO0vYuthpAMgCI0TYWOWbTE8yxD6s,4351
+gscoordinator/utils.py,sha256=orWfdjfQ3NL5ex6XB1VvfBhxyOqlRFR6OSMOE3jgmcE,80235
+gscoordinator/version.py,sha256=bS71qRjwM-xk4LAFTExdiWJOaJEXaeNdlJYCAqtD98U,1045
+gscoordinator/builtin/__init__.py,sha256=TsAsMQRDcEJ9nRXDAeF-pJPapJrZPwVeb-TxxVp42aY,646
+gscoordinator/builtin/app/.gs_conf.yaml,sha256=gWoCXtVzGb1xks9ioQ5WfYMnFPRJGiq9Cb-w3oF8SVA,25282
+gscoordinator/builtin/app/__init__.py,sha256=TsAsMQRDcEJ9nRXDAeF-pJPapJrZPwVeb-TxxVp42aY,646
+gscoordinator/builtin/app/builtin_app.gar,sha256=LuWyxWowYPt5HGIO3GmKcirUWyPCajDHRN8H7GK4TgY,5264
+gscoordinator/hook/__init__.py,sha256=jzzLJxC1gBgRLMb4xzX6vucYuNdosuWOtZKRj7Cal_o,646
+gscoordinator/hook/prestop/__init__.py,sha256=jzzLJxC1gBgRLMb4xzX6vucYuNdosuWOtZKRj7Cal_o,646
+gscoordinator/hook/prestop/__main__.py,sha256=1FmS0g2hwl85NPMOtbAvW_IGn4GFnldmjbSSwaj9GrE,1560
+gscoordinator/servicer/__init__.py,sha256=i0VzRn8z0PsDlQj3oZzOsii2qVSk-vcZQzFtbse9fVo,707
+gscoordinator/servicer/graphscope_one/__init__.py,sha256=hSEiV3pYv8wKgo6KzUx0p4563wJ1on2osrFZxZ4pT2o,646
+gscoordinator/servicer/graphscope_one/service.py,sha256=IS1zquyYhLBn4dSGyYCNJz1GKuz5EHO4ityrvG5JHD4,24792
+gscoordinator/template/CMakeLists.template,sha256=EqTx-5CWuZ6bf6lUhGZ8Hwu6s3AANu-cScKpjxm4ndw,22656
+gscoordinator/template/__init__.py,sha256=TsAsMQRDcEJ9nRXDAeF-pJPapJrZPwVeb-TxxVp42aY,646
+gscoordinator/template/pie.pxd.template,sha256=-hYphyhUzTnyQELecGEsCK_S-fEXLWGiTV91-gDqAU8,4957
+gscoordinator/template/pregel.pxd.template,sha256=Eh4tESR8KlmM30Mcw-eIUfiQNeadDj3WWGCUzkIsT2M,4340
+gs_coordinator-0.27.0a20240401.dist-info/METADATA,sha256=gztRSyjwVc3e3aHGZGiDDaoA7_7W3TOhf7RpAs-Unpk,23840
+gs_coordinator-0.27.0a20240401.dist-info/WHEEL,sha256=-G_t0oGuE7UD0DrSpVZnq1hHMBV9DD2XkS5v7XpmTnk,110
+gs_coordinator-0.27.0a20240401.dist-info/top_level.txt,sha256=GiJfpWt7WpC-H1BxUy5V39G7WAtPut6eqH3yAciJhqQ,33
+gs_coordinator-0.27.0a20240401.dist-info/RECORD,,
```

## Comparing `gs_coordinator-0.27.0a20240331.dist-info/METADATA` & `gs_coordinator-0.27.0a20240401.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gs-coordinator
-Version: 0.27.0a20240331
+Version: 0.27.0a20240401
 Home-page: https://github.com/alibaba/GraphScope
 Author: GraphScope Team, Damo Academy
 Author-email: graphscope@alibaba-inc.com
 License: Apache License 2.0
 Keywords: GraphScope,Graph Computations
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -26,15 +26,15 @@
 Requires-Dist: grpcio-tools >=1.49
 Requires-Dist: kubernetes >=24.2.0
 Requires-Dist: protobuf >=4
 Requires-Dist: PyYAML
 Requires-Dist: prometheus-client >=0.14.1
 Requires-Dist: packaging
 Requires-Dist: tqdm
-Requires-Dist: graphscope-client ==0.27.0a20240331
+Requires-Dist: graphscope-client ==0.27.0a20240401
 Requires-Dist: vineyard >=0.16.3 ; sys_platform != "win32"
 Requires-Dist: vineyard-io >=0.16.3 ; sys_platform != "win32"
 Provides-Extra: dev
 Requires-Dist: black >=23.3.0 ; extra == 'dev'
 Requires-Dist: flake8 ==4.0.1 ; extra == 'dev'
 Requires-Dist: isort ==5.10.1 ; extra == 'dev'
 Requires-Dist: setuptools ==65.7.0 ; extra == 'dev'
```

