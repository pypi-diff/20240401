# Comparing `tmp/profiles_rudderstack-0.9.3-py3-none-win_amd64.whl.zip` & `tmp/profiles_rudderstack-0.9.4-py3-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,24 +1,24 @@
-Zip file size: 23331 bytes, number of entries: 22
+Zip file size: 23439 bytes, number of entries: 22
 -rw-r--r--  2.0 unx        0 b- defN 23-Sep-21 17:38 profiles_rudderstack/__init__.py
 -rw-r--r--  2.0 unx      788 b- defN 23-Oct-17 18:14 profiles_rudderstack/contract.py
 -rw-r--r--  2.0 unx      935 b- defN 23-Oct-17 18:14 profiles_rudderstack/logger.py
--rw-r--r--  2.0 unx    12893 b- defN 23-Oct-17 18:14 profiles_rudderstack/material.py
+-rw-r--r--  2.0 unx    13452 b- defN 23-Nov-08 09:25 profiles_rudderstack/material.py
 -rw-r--r--  2.0 unx     1455 b- defN 23-Oct-17 18:14 profiles_rudderstack/model.py
 -rw-r--r--  2.0 unx     2905 b- defN 23-Oct-17 18:14 profiles_rudderstack/project.py
 -rw-r--r--  2.0 unx     1431 b- defN 23-Oct-17 18:14 profiles_rudderstack/recipe.py
 -rw-r--r--  2.0 unx     3655 b- defN 23-Oct-17 18:14 profiles_rudderstack/server.py
 -rw-r--r--  2.0 unx     9279 b- defN 23-Oct-17 18:14 profiles_rudderstack/service.py
 -rw-r--r--  2.0 unx      905 b- defN 23-Oct-17 18:14 profiles_rudderstack/utils.py
 -rw-r--r--  2.0 unx     1034 b- defN 23-Sep-21 17:38 profiles_rudderstack/wht_service.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Aug-23 07:52 profiles_rudderstack/tunnel/__init__.py
 -rw-r--r--  2.0 unx    15468 b- defN 23-Oct-17 18:14 profiles_rudderstack/tunnel/tunnel_pb2.py
 -rw-r--r--  2.0 unx    57968 b- defN 23-Oct-17 18:14 profiles_rudderstack/tunnel/tunnel_pb2_grpc.py
 -rw-r--r--  2.0 unx     1592 b- defN 23-Oct-17 18:14 profiles_rudderstack/wh/__init__.py
 -rw-r--r--  2.0 unx     3195 b- defN 23-Oct-17 18:14 profiles_rudderstack/wh/connector_base.py
 -rw-r--r--  2.0 unx     3314 b- defN 23-Oct-17 18:14 profiles_rudderstack/wh/redshift_connector.py
 -rw-r--r--  2.0 unx     2987 b- defN 23-Oct-17 18:14 profiles_rudderstack/wh/snowflake_connector.py
--rw-r--r--  2.0 unx      869 b- defN 23-Nov-01 10:55 profiles_rudderstack-0.9.3.dist-info/METADATA
--rw-r--r--  2.0 unx       98 b- defN 23-Nov-01 10:55 profiles_rudderstack-0.9.3.dist-info/WHEEL
--rw-r--r--  2.0 unx       21 b- defN 23-Nov-01 10:55 profiles_rudderstack-0.9.3.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     2003 b- defN 23-Nov-01 10:55 profiles_rudderstack-0.9.3.dist-info/RECORD
-22 files, 122795 bytes uncompressed, 20009 bytes compressed:  83.7%
+-rw-r--r--  2.0 unx      908 b- defN 23-Nov-08 09:48 profiles_rudderstack-0.9.4.dist-info/METADATA
+-rw-r--r--  2.0 unx       98 b- defN 23-Nov-08 09:48 profiles_rudderstack-0.9.4.dist-info/WHEEL
+-rw-r--r--  2.0 unx       21 b- defN 23-Nov-08 09:48 profiles_rudderstack-0.9.4.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     2003 b- defN 23-Nov-08 09:48 profiles_rudderstack-0.9.4.dist-info/RECORD
+22 files, 123393 bytes uncompressed, 20117 bytes compressed:  83.7%
```

## zipnote {}

```diff
@@ -48,20 +48,20 @@
 
 Filename: profiles_rudderstack/wh/redshift_connector.py
 Comment: 
 
 Filename: profiles_rudderstack/wh/snowflake_connector.py
 Comment: 
 
-Filename: profiles_rudderstack-0.9.3.dist-info/METADATA
+Filename: profiles_rudderstack-0.9.4.dist-info/METADATA
 Comment: 
 
-Filename: profiles_rudderstack-0.9.3.dist-info/WHEEL
+Filename: profiles_rudderstack-0.9.4.dist-info/WHEEL
 Comment: 
 
-Filename: profiles_rudderstack-0.9.3.dist-info/top_level.txt
+Filename: profiles_rudderstack-0.9.4.dist-info/top_level.txt
 Comment: 
 
-Filename: profiles_rudderstack-0.9.3.dist-info/RECORD
+Filename: profiles_rudderstack-0.9.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## profiles_rudderstack/material.py

```diff
@@ -1,22 +1,22 @@
 from typing import Optional, List, Dict, Iterator, Literal
 from google.protobuf import json_format
 from profiles_rudderstack.contract import Contract
 from profiles_rudderstack.utils import remap_credentials
 from profiles_rudderstack.logger import Logger
 from profiles_rudderstack.tunnel.tunnel_pb2_grpc import WhtServiceStub
 import profiles_rudderstack.tunnel.tunnel_pb2 as tunnel_pb2
-from snowflake.snowpark.session import Session
 from profiles_rudderstack.wh import ProfilesConnector
 from profiles_rudderstack.wh.connector_base import ConnectorBase
 import pandas as pd
 
 class WhtWarehouseClient:
     # Static props for caching, wh connection is same for all models in a pb project
-    __snowpark_sesion: Optional[Session] = None
+    __snowpark_sesion = None
+    snowpark_enabled: bool = True
     __wh_connection: Optional[ConnectorBase] = None
     __schema: Optional[str] = None
     __wh_type: Optional[Literal['snowflake', 'redshift']] = None
 
     def __init__(self, material_ref: int, wht_service: WhtServiceStub, is_null_ctx: bool) -> None:
         self.snowpark_session = WhtWarehouseClient.__snowpark_sesion
         self.wh_connection = WhtWarehouseClient.__wh_connection
@@ -30,19 +30,32 @@
         if not is_null_ctx and (WhtWarehouseClient.__snowpark_sesion is None and WhtWarehouseClient.__wh_connection is None):
             creds_response: tunnel_pb2.GetWarehouseCredentialsResponse = wht_service.GetWarehouseCredentials(tunnel_pb2.GetWarehouseCredentialsRequest(
                 material_ref=self.__material_ref,
             ))
             creds = json_format.MessageToDict(creds_response.credentials)
             self.schema = creds.get("schema", None)
             self.wh_type = creds.get("type", None)
-            # Use snowpark for snowflake, otherwise use warehouse connector
+
             if self.wh_type == "snowflake":
+                try:
+                    from snowflake.snowpark.session import Session
+                except ImportError:
+                    self.logger.warn("snowpark not installed, using warehouse connector instead")
+                    WhtWarehouseClient.snowpark_enabled = False
+            else:
+                WhtWarehouseClient.snowpark_enabled = False
+
+            # Use snowpark for snowflake, otherwise use warehouse connector
+            if WhtWarehouseClient.snowpark_enabled:
+                from snowflake.snowpark.session import Session
                 creds = remap_credentials(creds)
 
                 self.snowpark_session = Session.builder.configs(creds).create()
+            elif self.wh_type == "snowflake":
+                self.wh_connection = ProfilesConnector(creds)
             elif self.wh_type == "redshift":
                 s3_config = creds.get("s3", None)
                 if s3_config is None:
                     self.logger.warn("its recommended to provide s3 config in siteconfig to get added performance benefit in redshift (https://stackoverflow.com/questions/38402995/how-to-write-data-to-redshift-that-is-a-result-of-a-dataframe-created-in-python)")
                 
                 # json_format converts int to float, so we need to convert it back
                 creds.update({"port": int(creds.get("port", 0))})
@@ -52,15 +65,15 @@
             WhtWarehouseClient.__snowpark_sesion = self.snowpark_session
             WhtWarehouseClient.__wh_connection = self.wh_connection
             WhtWarehouseClient.__schema = self.schema
             WhtWarehouseClient.__wh_type = self.wh_type
         
 
     def query_sql_with_result(self, sql: str) -> pd.DataFrame:
-        if self.wh_type == "snowflake":
+        if WhtWarehouseClient.snowpark_enabled:
             return self.snowpark_session.sql(sql).to_pandas(block=True)
         else:
             return self.wh_connection.run_query(sql)
 
     def query_sql_without_result(self, sql: str):
         self.__wht_service.QuerySqlWithoutResult(tunnel_pb2.QuerySqlWithoutResultRequest(
             material_ref=self.__material_ref,
@@ -72,15 +85,15 @@
             material_ref=self.__material_ref,
             template=template,
         ))
 
     def write_df_to_table(self, df, table: str, append_if_exists: bool = False):
         table_name = table.upper()
         df.columns = df.columns.str.upper()
-        if self.wh_type == "snowflake":
+        if WhtWarehouseClient.snowpark_enabled:
             self.snowpark_session.write_pandas(df, table_name=table_name, auto_create_table=True, overwrite=False if append_if_exists else True)
         else:
             self.wh_connection.write_to_table(df, table_name, self.schema, if_exists="append" if append_if_exists else "replace")
 
 
 class WhtContext:
     def __init__(self, material_ref: int, wht_service: WhtServiceStub) -> None:
@@ -246,15 +259,15 @@
         """
         getSelectorSqlRes = self.__wht_service.GetSelectorSql(tunnel_pb2.GetSelectorSqlRequest(
             material_ref=self.__material_ref,
             columns=select_columns,
         ))
         select_query = getSelectorSqlRes.sql
 
-        if self.wht_ctx.client.wh_type == "snowflake":
+        if WhtWarehouseClient.snowpark_enabled:
             return self.wht_ctx.client.snowpark_session.sql(select_query).to_pandas(block=True)
         else:
             return self.wht_ctx.client.wh_connection.run_query(select_query)
         
     def get_table_data_batches(self, select_columns: Optional[List[str]] = None) -> Iterator[pd.DataFrame]:
         """Get the table data of the material in batches.
 
@@ -283,15 +296,15 @@
 
         Args:
             df (pd.DataFrame): DataFrame to be written
             append_if_exists (bool, optional): Append to the table if it exists. Defaults to False.
         """
         tableName = self.name()
         df.columns = df.columns.str.upper()
-        if self.wht_ctx.client.wh_type == "snowflake":
+        if WhtWarehouseClient.snowpark_enabled:
             self.wht_ctx.client.snowpark_session.write_pandas(df, table_name=tableName, auto_create_table=True, overwrite=False if append_if_exists else True)
         else:
             self.wht_ctx.client.wh_connection.write_to_table(df, tableName, self.wht_ctx.client.schema, if_exists="append" if append_if_exists else "replace")
     
     def execute_text_template(self, template: str) -> str:
         templateResponse: tunnel_pb2.ExecuteTextTemplateResponse = self.__wht_service.ExecuteTextTemplate(tunnel_pb2.ExecuteTextTemplateRequest(
             material_ref=self.__material_ref,
```

## Comparing `profiles_rudderstack-0.9.3.dist-info/METADATA` & `profiles_rudderstack-0.9.4.dist-info/METADATA`

 * *Files 8% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 Metadata-Version: 2.1
 Name: profiles-rudderstack
-Version: 0.9.3
+Version: 0.9.4
 Summary: UNKNOWN
 Home-page: https://www.rudderstack.com/
 Author: rudderstack
 Author-email: shubhammehra@rudderstack.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: MacOS
-Requires-Python: >=3.8, <=3.10
+Requires-Python: >=3.8
 Requires-Dist: grpcio (>=1.56.2)
 Requires-Dist: grpc-interceptor (>=0.15.2)
 Requires-Dist: protobuf (>=4.24.0)
 Requires-Dist: pandas (>=1.5.3)
-Requires-Dist: snowflake-snowpark-python (>=0.10.0)
 Requires-Dist: sqlalchemy-redshift (>=0.8.14)
 Requires-Dist: snowflake-sqlalchemy (>=1.4.7)
 Requires-Dist: pandas-redshift (>=2.0.5)
 Requires-Dist: snowflake-connector-python[pandas]
-Requires-Dist: profiles-rudderstack-bin (==0.9.3)
+Requires-Dist: profiles-rudderstack-bin (==0.9.4)
+Provides-Extra: snowpark
+Requires-Dist: snowflake-snowpark-python (>=0.10.0) ; extra == 'snowpark'
 
 UNKNOWN
```

## Comparing `profiles_rudderstack-0.9.3.dist-info/RECORD` & `profiles_rudderstack-0.9.4.dist-info/RECORD`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 profiles_rudderstack/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 profiles_rudderstack/contract.py,sha256=Rx0EGQtL4lTsNn_R785wOOhBbo-Lr59bq86Id2MO_bA,788
 profiles_rudderstack/logger.py,sha256=oZ_ywk0KAl2ZX30-w_x1OILw5GuRSzLFVvJ7v4KBwyI,935
-profiles_rudderstack/material.py,sha256=XzsBS8KMxzeqbn1su7NdpAQTUSRov1Zqo2FOLyEdAxM,12893
+profiles_rudderstack/material.py,sha256=2KwQBywt8pTVWhOlYLvs8nd_kCD5oD_rzHoH7QxQHNg,13452
 profiles_rudderstack/model.py,sha256=tAaJc-le3ruKKpAWVq4nBiW7v0RwP404jHcUUHht2Sc,1455
 profiles_rudderstack/project.py,sha256=4AcG14OdU4lUf5akIVscJc_3N263VSWUeHaRwUMy9Oo,2905
 profiles_rudderstack/recipe.py,sha256=qz6SZzsjltc8_u8F_a0RgFXtZbn4oLhnWe3aO9CJcBs,1431
 profiles_rudderstack/server.py,sha256=kV50giIEC0P-KJN0eUgpyZMUIJvMtPnwLq8s03GDAYs,3655
 profiles_rudderstack/service.py,sha256=at8WoKKNFiQWvjJEUKBNL5X_qpOGNOSxYV3uteoMW6M,9279
 profiles_rudderstack/utils.py,sha256=9eEjlUlbXDE2qK0vBE-5F4b7aUudHD-T6_mptPcGEO4,905
 profiles_rudderstack/wht_service.py,sha256=bFBbletNUYsINL9K9PXDEbNuzRYIBE5Fz9ne7QF9Y0Y,1034
 profiles_rudderstack/tunnel/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 profiles_rudderstack/tunnel/tunnel_pb2.py,sha256=2cNeHvuOP8Qtyrv1zaVjBVqX7ZmtSlPlUKYEO5pdmd0,15468
 profiles_rudderstack/tunnel/tunnel_pb2_grpc.py,sha256=MySW8FJzYubJ5LnwuNH--Ukn3FN5vsJeUlVFz_1XS-E,57968
 profiles_rudderstack/wh/__init__.py,sha256=Mk6sdHl5yEqQ-ByFpcd3lSGcsdMAcDJG2KOyrqhxaTM,1592
 profiles_rudderstack/wh/connector_base.py,sha256=NwDC7WaIJVq7NatfilhDqeC5HM007CkB7FvzVQ_6xrw,3195
 profiles_rudderstack/wh/redshift_connector.py,sha256=FdbPi8J04V2f37O-JQ1RIFk0-bYGxQ-Qw4nJzWu2aE0,3314
 profiles_rudderstack/wh/snowflake_connector.py,sha256=VcCSp8CYj2kKZCcrrfvu5QEfN7mBjMXrghBM5lqu2mo,2987
-profiles_rudderstack-0.9.3.dist-info/METADATA,sha256=W88JqxqM_pDwv5T4V4BTLxmtutGX8NFZQstrSv4uFJw,869
-profiles_rudderstack-0.9.3.dist-info/WHEEL,sha256=WoE84lFhzpl5kFoOWeOKUr67l1o9c9Tie8ccxFQmzBU,98
-profiles_rudderstack-0.9.3.dist-info/top_level.txt,sha256=1KAKMSAqL6g-gl7L87s0v1bUONdPtlJA4vx_nZuvWNo,21
-profiles_rudderstack-0.9.3.dist-info/RECORD,,
+profiles_rudderstack-0.9.4.dist-info/METADATA,sha256=DCctFsBZ6y1NKB-Qq2d8Um4NrrFOTb-RSdt-1FbxkgI,908
+profiles_rudderstack-0.9.4.dist-info/WHEEL,sha256=WoE84lFhzpl5kFoOWeOKUr67l1o9c9Tie8ccxFQmzBU,98
+profiles_rudderstack-0.9.4.dist-info/top_level.txt,sha256=1KAKMSAqL6g-gl7L87s0v1bUONdPtlJA4vx_nZuvWNo,21
+profiles_rudderstack-0.9.4.dist-info/RECORD,,
```

