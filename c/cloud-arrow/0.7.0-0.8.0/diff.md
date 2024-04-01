# Comparing `tmp/cloud-arrow-0.7.0.tar.gz` & `tmp/cloud-arrow-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cloud-arrow-0.7.0.tar", last modified: Wed Mar 13 16:36:47 2024, max compression
+gzip compressed data, was "cloud-arrow-0.8.0.tar", last modified: Mon Apr  1 11:33:58 2024, max compression
```

## Comparing `cloud-arrow-0.7.0.tar` & `cloud-arrow-0.8.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0        0        0        0 2024-03-13 16:36:47.628391 cloud-arrow-0.7.0/
--rw-rw-rw-   0        0        0    35821 2023-10-31 09:54:53.000000 cloud-arrow-0.7.0/LICENSE
--rw-rw-rw-   0        0        0    21352 2024-03-13 16:36:47.628391 cloud-arrow-0.7.0/PKG-INFO
--rw-rw-rw-   0        0        0    20674 2024-03-13 11:15:37.000000 cloud-arrow-0.7.0/README.md
-drwxrwxrwx   0        0        0        0 2024-03-13 16:36:47.605509 cloud-arrow-0.7.0/cloud/
--rw-rw-rw-   0        0        0      146 2023-11-21 12:15:43.000000 cloud-arrow-0.7.0/cloud/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-13 16:36:47.609853 cloud-arrow-0.7.0/cloud/adls/
--rw-rw-rw-   0        0        0       31 2023-12-28 08:23:41.000000 cloud-arrow-0.7.0/cloud/adls/__init__.py
--rw-rw-rw-   0        0        0     2359 2024-01-03 10:09:58.000000 cloud-arrow-0.7.0/cloud/adls/adls.py
-drwxrwxrwx   0        0        0        0 2024-03-13 16:36:47.614412 cloud-arrow-0.7.0/cloud/core/
--rw-rw-rw-   0        0        0      140 2023-12-28 08:23:41.000000 cloud-arrow-0.7.0/cloud/core/__init__.py
--rw-rw-rw-   0        0        0    19299 2024-03-12 09:16:12.000000 cloud-arrow-0.7.0/cloud/core/core.py
-drwxrwxrwx   0        0        0        0 2024-03-13 16:36:47.617986 cloud-arrow-0.7.0/cloud/gcsfs/
--rw-rw-rw-   0        0        0       31 2023-12-28 08:23:41.000000 cloud-arrow-0.7.0/cloud/gcsfs/__init__.py
--rw-rw-rw-   0        0        0     1780 2023-12-28 08:23:41.000000 cloud-arrow-0.7.0/cloud/gcsfs/gcsfs.py
-drwxrwxrwx   0        0        0        0 2024-03-13 16:36:47.621184 cloud-arrow-0.7.0/cloud/local/
--rw-rw-rw-   0        0        0        0 2023-12-28 08:23:41.000000 cloud-arrow-0.7.0/cloud/local/__init__.py
--rw-rw-rw-   0        0        0      733 2023-12-28 08:23:41.000000 cloud-arrow-0.7.0/cloud/local/local.py
-drwxrwxrwx   0        0        0        0 2024-03-13 16:36:47.627355 cloud-arrow-0.7.0/cloud_arrow.egg-info/
--rw-rw-rw-   0        0        0    21352 2024-03-13 16:36:47.000000 cloud-arrow-0.7.0/cloud_arrow.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      402 2024-03-13 16:36:47.000000 cloud-arrow-0.7.0/cloud_arrow.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-13 16:36:47.000000 cloud-arrow-0.7.0/cloud_arrow.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       76 2024-03-13 16:36:47.000000 cloud-arrow-0.7.0/cloud_arrow.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-03-13 16:36:47.000000 cloud-arrow-0.7.0/cloud_arrow.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2024-03-13 16:36:47.629417 cloud-arrow-0.7.0/setup.cfg
--rw-rw-rw-   0        0        0     1165 2024-03-12 09:16:43.000000 cloud-arrow-0.7.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-01 11:33:58.143248 cloud-arrow-0.8.0/
+-rw-rw-rw-   0        0        0    35821 2023-10-31 09:54:53.000000 cloud-arrow-0.8.0/LICENSE
+-rw-rw-rw-   0        0        0    21484 2024-04-01 11:33:58.143248 cloud-arrow-0.8.0/PKG-INFO
+-rw-rw-rw-   0        0        0    20806 2024-04-01 11:26:49.000000 cloud-arrow-0.8.0/README.md
+drwxrwxrwx   0        0        0        0 2024-04-01 11:33:58.107363 cloud-arrow-0.8.0/cloud/
+-rw-rw-rw-   0        0        0      162 2024-04-01 09:25:18.000000 cloud-arrow-0.8.0/cloud/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-01 11:33:58.110377 cloud-arrow-0.8.0/cloud/adls/
+-rw-rw-rw-   0        0        0       31 2023-12-28 08:23:41.000000 cloud-arrow-0.8.0/cloud/adls/__init__.py
+-rw-rw-rw-   0        0        0     2359 2024-01-03 10:09:58.000000 cloud-arrow-0.8.0/cloud/adls/adls.py
+drwxrwxrwx   0        0        0        0 2024-04-01 11:33:58.113387 cloud-arrow-0.8.0/cloud/core/
+-rw-rw-rw-   0        0        0      140 2023-12-28 08:23:41.000000 cloud-arrow-0.8.0/cloud/core/__init__.py
+-rw-rw-rw-   0        0        0    19143 2024-03-27 13:40:37.000000 cloud-arrow-0.8.0/cloud/core/core.py
+drwxrwxrwx   0        0        0        0 2024-04-01 11:33:58.118507 cloud-arrow-0.8.0/cloud/gcsfs/
+-rw-rw-rw-   0        0        0       31 2023-12-28 08:23:41.000000 cloud-arrow-0.8.0/cloud/gcsfs/__init__.py
+-rw-rw-rw-   0        0        0     1780 2023-12-28 08:23:41.000000 cloud-arrow-0.8.0/cloud/gcsfs/gcsfs.py
+drwxrwxrwx   0        0        0        0 2024-04-01 11:33:58.122047 cloud-arrow-0.8.0/cloud/local/
+-rw-rw-rw-   0        0        0        0 2023-12-28 08:23:41.000000 cloud-arrow-0.8.0/cloud/local/__init__.py
+-rw-rw-rw-   0        0        0      733 2023-12-28 08:23:41.000000 cloud-arrow-0.8.0/cloud/local/local.py
+drwxrwxrwx   0        0        0        0 2024-04-01 11:33:58.141057 cloud-arrow-0.8.0/cloud_arrow.egg-info/
+-rw-rw-rw-   0        0        0    21484 2024-04-01 11:33:57.000000 cloud-arrow-0.8.0/cloud_arrow.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      402 2024-04-01 11:33:57.000000 cloud-arrow-0.8.0/cloud_arrow.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-01 11:33:57.000000 cloud-arrow-0.8.0/cloud_arrow.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       76 2024-04-01 11:33:57.000000 cloud-arrow-0.8.0/cloud_arrow.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-04-01 11:33:57.000000 cloud-arrow-0.8.0/cloud_arrow.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2024-04-01 11:33:58.144302 cloud-arrow-0.8.0/setup.cfg
+-rw-rw-rw-   0        0        0     1165 2024-04-01 09:28:01.000000 cloud-arrow-0.8.0/setup.py
```

### Comparing `cloud-arrow-0.7.0/LICENSE` & `cloud-arrow-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cloud-arrow-0.7.0/PKG-INFO` & `cloud-arrow-0.8.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloud-arrow
-Version: 0.7.0
+Version: 0.8.0
 Summary: Python library to provide an Unified cloud storage API for reading and writing parquet and  deltalake files from/to the main cloud provider's object storage using the arrow format
 Home-page: https://github.com/a24lorie/Cloud-Arrow
 Author-email: a24lorie@gmail.com, nachorodriguez79@gmail.com
 License: GNU
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pyarrow
@@ -17,15 +17,15 @@
 Requires-Dist: azure-identity
 Requires-Dist: fsspec
 Requires-Dist: deltalake
 
 <p style="text-align: center;">
    Feb 2024 <br/>
    Alfredo Lorie Bernardo, Ignacio Rodriguez Sanchez <br/>
-   version 0.7.0
+   version 0.8.0
 </p>
 
 # Cloud Arrow
 Python Library to read and write Parquet and Deltalake files from the main Cloud Providers 
 Object-Store and Local Filesystem
 
 ## Introduction
@@ -273,20 +273,21 @@
 ```
 
 ## Writing Data
 To write files to ADLSGen2, GCSFS or the Local Filesystem use the **object_storage** instance configured. 
 The Cloud Arrow library provides an unified and consistence experience across all the filesystem implementations 
 to write parquet files or delta-lake tables, the following method is available for writing:
 
-* write(data, file_format, path, write_options: WriteOptions)
+* write(data, file_format, path, basename_template, write_options: WriteOptions)
 1. **data**: (*Required*) - Can be one of pandas.DataFrame, pyarrow.Dataset, Table/RecordBatch, RecordBatchReader, list of \
                    Table/RecordBatch, or iterable of RecordBatch 
 2. **file_format**: (*Required*) - Can be one of "parquet" or "deltalake"
 3. **path**:  (*Required*)  - The object storage location to the dataset (can be a single file name or directory name)
-4. **write_options** - Required - Options to write the files including: 
+4. **basename_template** (*Optional*) - A template string used to generate basenames of written data files.
+5. **write_options** - (*Required*) - Options to write the files including: 
     ```
     WriteOptions 
     |     * partitions: List of the names of columns to split the dataset. 
     |     * compression_codec: Allow to specify the compression codec (None, snappy, sz4, brotli, gzip, zstd)
     └─── ParquetWriteOptions
             *  existing_data_behavior: Can be one of ['error', 'overwrite_or_ignore', 'delete_matching']              
     └─── DeltaLakeWriteOptions
```

### Comparing `cloud-arrow-0.7.0/README.md` & `cloud-arrow-0.8.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 <p style="text-align: center;">
    Feb 2024 <br/>
    Alfredo Lorie Bernardo, Ignacio Rodriguez Sanchez <br/>
-   version 0.7.0
+   version 0.8.0
 </p>
 
 # Cloud Arrow
 Python Library to read and write Parquet and Deltalake files from the main Cloud Providers 
 Object-Store and Local Filesystem
 
 ## Introduction
@@ -253,20 +253,21 @@
 ```
 
 ## Writing Data
 To write files to ADLSGen2, GCSFS or the Local Filesystem use the **object_storage** instance configured. 
 The Cloud Arrow library provides an unified and consistence experience across all the filesystem implementations 
 to write parquet files or delta-lake tables, the following method is available for writing:
 
-* write(data, file_format, path, write_options: WriteOptions)
+* write(data, file_format, path, basename_template, write_options: WriteOptions)
 1. **data**: (*Required*) - Can be one of pandas.DataFrame, pyarrow.Dataset, Table/RecordBatch, RecordBatchReader, list of \
                    Table/RecordBatch, or iterable of RecordBatch 
 2. **file_format**: (*Required*) - Can be one of "parquet" or "deltalake"
 3. **path**:  (*Required*)  - The object storage location to the dataset (can be a single file name or directory name)
-4. **write_options** - Required - Options to write the files including: 
+4. **basename_template** (*Optional*) - A template string used to generate basenames of written data files.
+5. **write_options** - (*Required*) - Options to write the files including: 
     ```
     WriteOptions 
     |     * partitions: List of the names of columns to split the dataset. 
     |     * compression_codec: Allow to specify the compression codec (None, snappy, sz4, brotli, gzip, zstd)
     └─── ParquetWriteOptions
             *  existing_data_behavior: Can be one of ['error', 'overwrite_or_ignore', 'delete_matching']              
     └─── DeltaLakeWriteOptions
```

### Comparing `cloud-arrow-0.7.0/cloud/adls/adls.py` & `cloud-arrow-0.8.0/cloud/adls/adls.py`

 * *Files identical despite different names*

### Comparing `cloud-arrow-0.7.0/cloud/core/core.py` & `cloud-arrow-0.8.0/cloud/core/core.py`

 * *Files 3% similar despite different names*

```diff
@@ -453,27 +453,32 @@
         return self.read_to_arrow_table(
             file_format=file_format,
             path=path,
             partitioning=partitioning,
             filters=filters
         ).to_pandas()
 
-    def write(self, data, file_format, path, write_options: WriteOptions):
+    def write(self, data, file_format, path, basename_template, write_options: WriteOptions):
         """
         :param data: pandas.DataFrame, pyarrow.Dataset, Table/RecordBatch, RecordBatchReader, list of \
                     Table/RecordBatch, or iterable of RecordBatch
 
         :param file_format: str
             Currently "parquet", "deltalake" supported.
         :param path: str
             Path pointing to a single file:
                 Open a Dataset from a single file.
             Path pointing to a directory:
                 The directory gets discovered recursively according to a
                 partitioning scheme if given.
+        :param basename_template : str, optional
+            A template string used to generate basenames of written data files.
+            The token '{i}' will be replaced with an automatically incremented
+            integer. If not specified, it defaults to
+            "part-{i}." + format.default_extname
         :param write_options:
         """
 
         def convert_pandas_to_arrow_table(dataframe):
             if isinstance(dataframe, pd.DataFrame):
                 return pa.Table.from_pandas(dataframe)
             else:
@@ -497,14 +502,15 @@
                                    partition_cols: {write_options.partitions}
                                """)
 
             pa.dataset.write_dataset(
                 data=pyarr_data,
                 format=file_format,
                 filesystem=filesystem,
+                basename_template=basename_template,
                 base_dir=self._get_filesystem_base_path(path=path),
                 partitioning=write_options.partitions,
                 existing_data_behavior=write_options.existing_data_behavior(),
                 file_options=ds.ParquetFileFormat().make_write_options(
                     compression=write_options.compression_codec
                 )
             )
@@ -516,23 +522,7 @@
                 file_options=ds.ParquetFileFormat().make_write_options(
                     compression=write_options.compression_codec
                 ),
                 storage_options=self._get_deltalake_storage_options(),
                 mode=write_options.existing_data_behavior()
             )
 
-
-
-    def write_batch(self, batch, file_format, path, write_options: WriteOptions):
-        """
-        :param table
-
-        :param file_format: str
-            Currently "parquet", "deltalake" supported.
-        :param path: str
-            Path pointing to a single file:
-                Open a Dataset from a single file.
-            Path pointing to a directory:
-                The directory gets discovered recursively according to a
-                partitioning scheme if given.
-        :param write_options:
-        """
```

### Comparing `cloud-arrow-0.7.0/cloud/gcsfs/gcsfs.py` & `cloud-arrow-0.8.0/cloud/gcsfs/gcsfs.py`

 * *Files identical despite different names*

### Comparing `cloud-arrow-0.7.0/cloud/local/local.py` & `cloud-arrow-0.8.0/cloud/local/local.py`

 * *Files identical despite different names*

### Comparing `cloud-arrow-0.7.0/cloud_arrow.egg-info/PKG-INFO` & `cloud-arrow-0.8.0/cloud_arrow.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloud-arrow
-Version: 0.7.0
+Version: 0.8.0
 Summary: Python library to provide an Unified cloud storage API for reading and writing parquet and  deltalake files from/to the main cloud provider's object storage using the arrow format
 Home-page: https://github.com/a24lorie/Cloud-Arrow
 Author-email: a24lorie@gmail.com, nachorodriguez79@gmail.com
 License: GNU
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pyarrow
@@ -17,15 +17,15 @@
 Requires-Dist: azure-identity
 Requires-Dist: fsspec
 Requires-Dist: deltalake
 
 <p style="text-align: center;">
    Feb 2024 <br/>
    Alfredo Lorie Bernardo, Ignacio Rodriguez Sanchez <br/>
-   version 0.7.0
+   version 0.8.0
 </p>
 
 # Cloud Arrow
 Python Library to read and write Parquet and Deltalake files from the main Cloud Providers 
 Object-Store and Local Filesystem
 
 ## Introduction
@@ -273,20 +273,21 @@
 ```
 
 ## Writing Data
 To write files to ADLSGen2, GCSFS or the Local Filesystem use the **object_storage** instance configured. 
 The Cloud Arrow library provides an unified and consistence experience across all the filesystem implementations 
 to write parquet files or delta-lake tables, the following method is available for writing:
 
-* write(data, file_format, path, write_options: WriteOptions)
+* write(data, file_format, path, basename_template, write_options: WriteOptions)
 1. **data**: (*Required*) - Can be one of pandas.DataFrame, pyarrow.Dataset, Table/RecordBatch, RecordBatchReader, list of \
                    Table/RecordBatch, or iterable of RecordBatch 
 2. **file_format**: (*Required*) - Can be one of "parquet" or "deltalake"
 3. **path**:  (*Required*)  - The object storage location to the dataset (can be a single file name or directory name)
-4. **write_options** - Required - Options to write the files including: 
+4. **basename_template** (*Optional*) - A template string used to generate basenames of written data files.
+5. **write_options** - (*Required*) - Options to write the files including: 
     ```
     WriteOptions 
     |     * partitions: List of the names of columns to split the dataset. 
     |     * compression_codec: Allow to specify the compression codec (None, snappy, sz4, brotli, gzip, zstd)
     └─── ParquetWriteOptions
             *  existing_data_behavior: Can be one of ['error', 'overwrite_or_ignore', 'delete_matching']              
     └─── DeltaLakeWriteOptions
```

### Comparing `cloud-arrow-0.7.0/setup.py` & `cloud-arrow-0.8.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='cloud-arrow',
-    version='0.7.0',
+    version='0.8.0',
     authors='Alfredo Lorie, Ignacio Rodriguez',
     author_email='a24lorie@gmail.com, nachorodriguez79@gmail.com',
     description="""Python library to provide an Unified cloud storage API for reading and writing parquet and  deltalake files from/to the main cloud provider's object storage using the arrow format""",
     long_description=open('README.md', encoding='UTF-8').read(),
     long_description_content_type='text/markdown',
     license='GNU',
     url='https://github.com/a24lorie/Cloud-Arrow',
```

