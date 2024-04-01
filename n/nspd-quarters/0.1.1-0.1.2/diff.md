# Comparing `tmp/nspd_quarters-0.1.1-py3-none-any.whl.zip` & `tmp/nspd_quarters-0.1.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 3104 bytes, number of entries: 7
+Zip file size: 3068 bytes, number of entries: 7
 -rw-rw-rw-  2.0 fat        0 b- defN 24-Mar-27 11:07 nspd_package_q/__init__.py
--rw-rw-rw-  2.0 fat     2871 b- defN 24-Mar-27 12:15 nspd_package_q/nspd_q.py
--rw-rw-rw-  2.0 fat      300 b- defN 24-Mar-27 12:18 nspd_quarters-0.1.1.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-Mar-27 12:18 nspd_quarters-0.1.1.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       62 b- defN 24-Mar-27 12:18 nspd_quarters-0.1.1.dist-info/entry_points.txt
--rw-rw-rw-  2.0 fat       15 b- defN 24-Mar-27 12:18 nspd_quarters-0.1.1.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      583 b- defN 24-Mar-27 12:18 nspd_quarters-0.1.1.dist-info/RECORD
-7 files, 3923 bytes uncompressed, 2054 bytes compressed:  47.6%
+-rw-rw-rw-  2.0 fat     2871 b- defN 24-Apr-01 10:28 nspd_package_q/nspd_q.py
+-rw-rw-rw-  2.0 fat      230 b- defN 24-Apr-01 10:32 nspd_quarters-0.1.2.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-01 10:32 nspd_quarters-0.1.2.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       61 b- defN 24-Apr-01 10:32 nspd_quarters-0.1.2.dist-info/entry_points.txt
+-rw-rw-rw-  2.0 fat       15 b- defN 24-Apr-01 10:32 nspd_quarters-0.1.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      583 b- defN 24-Apr-01 10:32 nspd_quarters-0.1.2.dist-info/RECORD
+7 files, 3852 bytes uncompressed, 2018 bytes compressed:  47.6%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: nspd_package_q/__init__.py
 Comment: 
 
 Filename: nspd_package_q/nspd_q.py
 Comment: 
 
-Filename: nspd_quarters-0.1.1.dist-info/METADATA
+Filename: nspd_quarters-0.1.2.dist-info/METADATA
 Comment: 
 
-Filename: nspd_quarters-0.1.1.dist-info/WHEEL
+Filename: nspd_quarters-0.1.2.dist-info/WHEEL
 Comment: 
 
-Filename: nspd_quarters-0.1.1.dist-info/entry_points.txt
+Filename: nspd_quarters-0.1.2.dist-info/entry_points.txt
 Comment: 
 
-Filename: nspd_quarters-0.1.1.dist-info/top_level.txt
+Filename: nspd_quarters-0.1.2.dist-info/top_level.txt
 Comment: 
 
-Filename: nspd_quarters-0.1.1.dist-info/RECORD
+Filename: nspd_quarters-0.1.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## nspd_package_q/nspd_q.py

```diff
@@ -9,15 +9,15 @@
 def parse_args():
     parser = argparse.ArgumentParser(description='Fetch and save data from nspd.gov.ru.')
     parser.add_argument('--num', required=True, help='Кадастровый номер')
     parser.add_argument('--output_directory', required=True, help='Путь к директории для сохранения файлов')
     return parser.parse_args()
 
 def collect_data(num, output_filename, url, headers):
-    pageNumber = 1
+    pageNumber = 0
     pageSize = 25
     cad_nums = []  # Собираем номера в список
     while True:
         data = {"text": num, "pageNumber": pageNumber, "pageSize": pageSize}
         response = requests.post(url, headers=headers, json=data, verify=False)
         if response.status_code == 200:
             response_data = response.json()
```

## Comparing `nspd_quarters-0.1.1.dist-info/RECORD` & `nspd_quarters-0.1.2.dist-info/RECORD`

 * *Files 22% similar despite different names*

```diff
@@ -1,7 +1,7 @@
 nspd_package_q/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-nspd_package_q/nspd_q.py,sha256=mKnPSiWAyDGch7Rd1ELA3PZL1txxIHAHU50nTKd4QUo,2871
-nspd_quarters-0.1.1.dist-info/METADATA,sha256=VmxpVYonWlr-EuBp76Ya9f5G_l_oPQ-al5EeJ83RhFw,300
-nspd_quarters-0.1.1.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-nspd_quarters-0.1.1.dist-info/entry_points.txt,sha256=bZdv4CcArJRZGtJoyDQru13sVmynmXl8k_LHD5I6-hY,62
-nspd_quarters-0.1.1.dist-info/top_level.txt,sha256=voPGfhvc-LItPUQ7CTM2meyhpslqryka6__ilgQ3zgY,15
-nspd_quarters-0.1.1.dist-info/RECORD,,
+nspd_package_q/nspd_q.py,sha256=T2nJ1WBOn1I2h77UikB-mk94rjJXfgPGu85morK-pFo,2871
+nspd_quarters-0.1.2.dist-info/METADATA,sha256=RDsekYufgyvqDsAPG_Q-KlyIOCMycTI8zJfSIJZ2mYo,230
+nspd_quarters-0.1.2.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+nspd_quarters-0.1.2.dist-info/entry_points.txt,sha256=zahfZutk91fC-PNLeqPbhoGPzFY8o6pCOsk0hpzeIxs,61
+nspd_quarters-0.1.2.dist-info/top_level.txt,sha256=voPGfhvc-LItPUQ7CTM2meyhpslqryka6__ilgQ3zgY,15
+nspd_quarters-0.1.2.dist-info/RECORD,,
```

