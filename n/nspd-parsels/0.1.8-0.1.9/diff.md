# Comparing `tmp/nspd_parsels-0.1.8-py3-none-any.whl.zip` & `tmp/nspd_parsels-0.1.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 3350 bytes, number of entries: 7
+Zip file size: 3314 bytes, number of entries: 7
 -rw-rw-rw-  2.0 fat        0 b- defN 24-Mar-27 11:07 nspd_package_p/__init__.py
--rw-rw-rw-  2.0 fat     3773 b- defN 24-Mar-27 13:01 nspd_package_p/nspd_p.py
--rw-rw-rw-  2.0 fat      299 b- defN 24-Mar-27 13:09 nspd_parsels-0.1.8.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-Mar-27 13:09 nspd_parsels-0.1.8.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       61 b- defN 24-Mar-27 13:09 nspd_parsels-0.1.8.dist-info/entry_points.txt
--rw-rw-rw-  2.0 fat       15 b- defN 24-Mar-27 13:09 nspd_parsels-0.1.8.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      578 b- defN 24-Mar-27 13:09 nspd_parsels-0.1.8.dist-info/RECORD
-7 files, 4818 bytes uncompressed, 2310 bytes compressed:  52.1%
+-rw-rw-rw-  2.0 fat     3773 b- defN 24-Apr-01 10:39 nspd_package_p/nspd_p.py
+-rw-rw-rw-  2.0 fat      229 b- defN 24-Apr-01 10:42 nspd_parsels-0.1.9.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-01 10:42 nspd_parsels-0.1.9.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       60 b- defN 24-Apr-01 10:42 nspd_parsels-0.1.9.dist-info/entry_points.txt
+-rw-rw-rw-  2.0 fat       15 b- defN 24-Apr-01 10:42 nspd_parsels-0.1.9.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      578 b- defN 24-Apr-01 10:42 nspd_parsels-0.1.9.dist-info/RECORD
+7 files, 4747 bytes uncompressed, 2274 bytes compressed:  52.1%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: nspd_package_p/__init__.py
 Comment: 
 
 Filename: nspd_package_p/nspd_p.py
 Comment: 
 
-Filename: nspd_parsels-0.1.8.dist-info/METADATA
+Filename: nspd_parsels-0.1.9.dist-info/METADATA
 Comment: 
 
-Filename: nspd_parsels-0.1.8.dist-info/WHEEL
+Filename: nspd_parsels-0.1.9.dist-info/WHEEL
 Comment: 
 
-Filename: nspd_parsels-0.1.8.dist-info/entry_points.txt
+Filename: nspd_parsels-0.1.9.dist-info/entry_points.txt
 Comment: 
 
-Filename: nspd_parsels-0.1.8.dist-info/top_level.txt
+Filename: nspd_parsels-0.1.9.dist-info/top_level.txt
 Comment: 
 
-Filename: nspd_parsels-0.1.8.dist-info/RECORD
+Filename: nspd_parsels-0.1.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## nspd_package_p/nspd_p.py

```diff
@@ -18,15 +18,15 @@
         with open(output_filename, 'a') as file:
             for cad_num in cad_nums:
                 file.write(f"{cad_num}\n")
         logging.info(f"Данные по классу {class_name} добавлены в файл: {output_filename}")
 
 def collect_data(quarter, headers, results_by_class):
     url = 'https://nspd.gov.ru/map_api/s_search/search'
-    pageNumber = 1
+    pageNumber = 0
     pageSize = 25
 
     while True:
         data = {"text": quarter, "pageNumber": pageNumber, "pageSize": pageSize}
         response = requests.post(url, data=json.dumps(data), headers=headers, verify=False)
         if response.status_code == 200:
             response_data = response.json()
```

