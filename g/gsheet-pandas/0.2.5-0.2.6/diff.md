# Comparing `tmp/gsheet_pandas-0.2.5-py3-none-any.whl.zip` & `tmp/gsheet_pandas-0.2.6-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 6243 bytes, number of entries: 9
--rw-r--r--  2.0 unx      108 b- defN 23-Oct-03 11:35 gsheet_pandas/__init__.py
--rw-r--r--  2.0 unx     1726 b- defN 23-Oct-03 11:35 gsheet_pandas/tests.py
--rw-r--r--  2.0 unx        0 b- defN 23-Oct-03 11:35 gsheet_pandas/adapter/__init__.py
--rw-r--r--  2.0 unx     5517 b- defN 23-Oct-03 11:35 gsheet_pandas/adapter/connection.py
--rw-r--r--  2.0 unx     1069 b- defN 23-Oct-03 11:36 gsheet_pandas-0.2.5.dist-info/LICENSE
--rw-r--r--  2.0 unx     3945 b- defN 23-Oct-03 11:36 gsheet_pandas-0.2.5.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Oct-03 11:36 gsheet_pandas-0.2.5.dist-info/WHEEL
--rw-r--r--  2.0 unx       14 b- defN 23-Oct-03 11:36 gsheet_pandas-0.2.5.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      755 b- defN 23-Oct-03 11:36 gsheet_pandas-0.2.5.dist-info/RECORD
-9 files, 13226 bytes uncompressed, 4929 bytes compressed:  62.7%
+Zip file size: 6817 bytes, number of entries: 9
+-rw-r--r--  2.0 unx      108 b- defN 24-Apr-01 10:37 gsheet_pandas/__init__.py
+-rw-r--r--  2.0 unx     2191 b- defN 24-Apr-01 10:37 gsheet_pandas/tests.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-01 10:37 gsheet_pandas/adapter/__init__.py
+-rw-r--r--  2.0 unx     7694 b- defN 24-Apr-01 10:37 gsheet_pandas/adapter/connection.py
+-rw-r--r--  2.0 unx     1069 b- defN 24-Apr-01 10:38 gsheet_pandas-0.2.6.dist-info/LICENSE
+-rw-r--r--  2.0 unx     3905 b- defN 24-Apr-01 10:38 gsheet_pandas-0.2.6.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-01 10:38 gsheet_pandas-0.2.6.dist-info/WHEEL
+-rw-r--r--  2.0 unx       14 b- defN 24-Apr-01 10:38 gsheet_pandas-0.2.6.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      755 b- defN 24-Apr-01 10:38 gsheet_pandas-0.2.6.dist-info/RECORD
+9 files, 15828 bytes uncompressed, 5503 bytes compressed:  65.2%
```

## zipnote {}

```diff
@@ -6,23 +6,23 @@
 
 Filename: gsheet_pandas/adapter/__init__.py
 Comment: 
 
 Filename: gsheet_pandas/adapter/connection.py
 Comment: 
 
-Filename: gsheet_pandas-0.2.5.dist-info/LICENSE
+Filename: gsheet_pandas-0.2.6.dist-info/LICENSE
 Comment: 
 
-Filename: gsheet_pandas-0.2.5.dist-info/METADATA
+Filename: gsheet_pandas-0.2.6.dist-info/METADATA
 Comment: 
 
-Filename: gsheet_pandas-0.2.5.dist-info/WHEEL
+Filename: gsheet_pandas-0.2.6.dist-info/WHEEL
 Comment: 
 
-Filename: gsheet_pandas-0.2.5.dist-info/top_level.txt
+Filename: gsheet_pandas-0.2.6.dist-info/top_level.txt
 Comment: 
 
-Filename: gsheet_pandas-0.2.5.dist-info/RECORD
+Filename: gsheet_pandas-0.2.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## gsheet_pandas/__init__.py

```diff
@@ -1,5 +1,5 @@
 from .adapter.connection import DriveConnection, setup
 
 
-__version__ = '0.1.8'
+__version__ = '0.2.6'
 __author__ = 'Iakov Kaiumov'
```

## gsheet_pandas/tests.py

```diff
@@ -5,53 +5,67 @@
 from pathlib import Path
 
 import pandas as pd
 
 from adapter import connection
 import dotenv
 
-
 BASE_DIR = Path(__file__).resolve().parent.parent
 dotenv.load_dotenv(BASE_DIR / '.env')
 
-table_name = os.getenv('table_name')
+spreadsheet_id = os.getenv('table_name')
 sheet_name = os.getenv('sheet_name')
 
 
+data_dir = Path(__file__).resolve().parent.parent / 'data'
+
+
 class TestConnectionMethods(unittest.TestCase):
+    @staticmethod
+    def _get_drive() -> connection.DriveConnection:
+        return connection.DriveConnection(
+            credentials_dir=data_dir / 'credentials.json',
+            token_dir=data_dir / 'token.json'
+        )
+
+    def test_list_sheets(self):
+        drive = self._get_drive()
+        sheets = drive.get_sheets_names(spreadsheet_id)
+        self.assertEqual(sheets, ['test', 'test2'])
+
+    def test_create_sheet(self):
+        drive = self._get_drive()
+        _id = drive.create_sheet(spreadsheet_id=spreadsheet_id, sheet_name='test2')
+        self.assertIsNone(_id)
 
     def test_connection_class(self):
-        data_dir = Path(__file__).resolve().parent.parent / 'data'
-        drive = connection.DriveConnection(credentials_dir=data_dir / 'credentials.json', token_dir=data_dir / 'token.json')
-
-        df = drive.download(drive_table=table_name, sheet_name=sheet_name)
+        drive = self._get_drive()
+        df = drive.download(spreadsheet_id=spreadsheet_id, sheet_name=sheet_name)
 
         new_column_value = str(random.random())
         df['column1'] = new_column_value
 
-        drive.upload(df, drive_table=table_name, sheet_name=sheet_name)
+        drive.upload(df, spreadsheet_id=spreadsheet_id, sheet_name=sheet_name)
 
-        df = drive.download(drive_table=table_name, sheet_name=sheet_name)
+        df = drive.download(spreadsheet_id=spreadsheet_id, sheet_name=sheet_name)
 
         values = df['column1'].values.tolist()
         for value in values:
             self.assertEqual(value, new_column_value)
 
     def test_pandas_extension(self):
-        data_dir = Path(__file__).resolve().parent.parent / 'data'
-
         connection.setup(credentials_dir=data_dir / 'credentials.json', token_dir=data_dir / 'token.json')
 
-        df = pd.from_gsheet(drive_table=table_name, sheet_name=sheet_name)
+        df = pd.from_gsheet(spreadsheet_id=spreadsheet_id, sheet_name=sheet_name)
         new_column_value = str(random.random())
         df['column1'] = new_column_value
 
-        df.to_gsheet(drive_table=table_name, sheet_name=sheet_name)
+        df.to_gsheet(spreadsheet_id=spreadsheet_id, sheet_name=sheet_name)
 
-        df = pd.from_gsheet(drive_table=table_name, sheet_name=sheet_name)
+        df = pd.from_gsheet(spreadsheet_id=spreadsheet_id, sheet_name=sheet_name)
         values = df['column1'].values.tolist()
         for value in values:
             self.assertEqual(value, new_column_value)
 
 
 if __name__ == '__main__':
     unittest.main()
```

## gsheet_pandas/adapter/connection.py

```diff
@@ -1,26 +1,26 @@
-from __future__ import print_function
-
 import datetime
+import logging
 import os.path
 import socket
 from pathlib import Path
 
+import googleapiclient
 import pandas as pd
 from pandas import Timestamp
 from pandas._libs.lib import Decimal
 
 from google.auth.transport.requests import Request
 from google.oauth2.credentials import Credentials
 from google.oauth2 import service_account
 from google_auth_oauthlib.flow import InstalledAppFlow
 from googleapiclient.discovery import build
 from googleapiclient.errors import HttpError
 
-
+logger = logging.getLogger('gsheet-pandas')
 timeout_in_sec = 60 * 1
 socket.setdefaulttimeout(timeout_in_sec)
 
 
 SCOPES = ['https://www.googleapis.com/auth/spreadsheets', 'https://www.googleapis.com/auth/drive']
 DEFAULT_RANGE_NAME = '!A1:ZZ900000'
 
@@ -78,15 +78,15 @@
         else:
             creds = self._get_user_creds()
 
         try:
             service = build(service_name, service_version, credentials=creds)
             return service
         except HttpError as err:
-            print(err)
+            logger.error(err)
             return None
 
     def get_all_files_in_folder(self, folder_id):
         files = []
         try:
             page_token = None
             while True:
@@ -99,23 +99,33 @@
 
                 files.extend(response.get('files', []))
                 page_token = response.get('nextPageToken', None)
                 if page_token is None:
                     break
 
         except HttpError as e:
-            print(f'get_all_files_in_folder: An error occurred - {e}')
             raise e
         return files
 
-    def download(self, drive_table: str, sheet_name: str, range_name: str = DEFAULT_RANGE_NAME,
+    def download(self,
+                 spreadsheet_id: str,
+                 sheet_name: str,
+                 range_name: str = DEFAULT_RANGE_NAME,
                  header: int | None = 0) -> pd.DataFrame:
+        """
+        Downloads Google Spreadsheet as Pandas DataFrame
+        :param spreadsheet_id: spreadsheet id
+        :param sheet_name: sheet name
+        :param range_name: range name (default is !A1:ZZ900000)
+        :param header: index of header row
+        :return dataframe
+        """
         service = self._get_service()
         sheet = self._get_service().spreadsheets()
-        result = sheet.values().get(spreadsheetId=drive_table, range=sheet_name + range_name).execute()
+        result = sheet.values().get(spreadsheetId=spreadsheet_id, range=sheet_name + range_name).execute()
         values = result.get('values', [])
         service.close()
         if not values:
             raise Exception('Empty data')
 
         if header is None:
             return pd.DataFrame(values)
@@ -130,30 +140,78 @@
         if len(df.columns) > len(columns):
             columns += [f'Unknown {i}' for i in range(len(df.columns) - len(columns))]
         df.columns = columns
         return df
 
     def upload(self,
                df: pd.DataFrame,
-               drive_table: str,
+               spreadsheet_id: str,
                sheet_name: str,
                range_name: str = DEFAULT_RANGE_NAME,
-               drop_columns: bool = False):
+               drop_columns: bool = False) -> None:
+        """
+        Uploads Pandas DataFrame to the Google Spreadsheet
+        :param df: Pandas DataFrame
+        :param spreadsheet_id: spreadsheet id
+        :param sheet_name: sheet name
+        :param range_name: range name (default is !A1:ZZ900000)
+        :param drop_columns: whether to drop DataFrame columns or not
+        """
         try:
             df = _fix_dtypes(df)
             values = df.T.reset_index().T.values.tolist()
             if drop_columns:
                 values = df.values.tolist()
             service = self._get_service()
             service.spreadsheets().values().update(
-                spreadsheetId=drive_table,
+                spreadsheetId=spreadsheet_id,
                 valueInputOption='RAW',
                 range=sheet_name + range_name,
                 body=dict(majorDimension='ROWS', values=values),
             ).execute()
             service.close()
         except socket.timeout as e:
-            print(f'pandas_to_sheet: Error: {e}')
             raise e
         except Exception as e:
-            print(f'pandas_to_sheet: Error: {e}')
             raise e
+
+    def get_sheets_names(self, spreadsheet_id: str) -> list[str]:
+        """
+        Get sheets names for spreadsheet
+        :param spreadsheet_id: spreadsheet id
+        :return: list of names
+        """
+        service = self._get_service()
+        sheet_metadata = service.spreadsheets().get(spreadsheetId=spreadsheet_id).execute()
+        sheets = sheet_metadata.get('sheets', '')
+        return [sheet.get("properties", {}).get("title") for sheet in sheets]
+
+    def create_sheet(self, spreadsheet_id: str, sheet_name: str) -> int | None:
+        """
+        Creates new sheet in existing spreadsheet
+        :param spreadsheet_id: spreadsheet id
+        :param sheet_name: new sheet's name
+        :return: new sheet id if success, None if sheet exists
+        """
+        service = self._get_service()
+        batch_update_spreadsheet_request_body = {
+            "requests": [
+                {
+                    "addSheet": {
+                        "properties": {
+                            "title": sheet_name,
+                        }
+                    }
+                }
+            ]
+        }
+
+        request = service.spreadsheets().batchUpdate(spreadsheetId=spreadsheet_id,
+                                                     body=batch_update_spreadsheet_request_body)
+        try:
+            response = request.execute()
+        except googleapiclient.errors.HttpError as e:
+            if e.status_code == 400:
+                return None
+            raise e
+        service.close()
+        return response['replies'][0]['addSheet']['properties']['sheetId']
```

## Comparing `gsheet_pandas-0.2.5.dist-info/LICENSE` & `gsheet_pandas-0.2.6.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `gsheet_pandas-0.2.5.dist-info/METADATA` & `gsheet_pandas-0.2.6.dist-info/METADATA`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gsheet-pandas
-Version: 0.2.5
+Version: 0.2.6
 Summary: Download and upload pandas dataframes to the Google sheets
 Home-page: https://github.com/iakov-kaiumov/gsheet-pandas
 Author: Iakov Kaiumov
 Author-email: kaiumov.iag@phystech.edu
 License: MIT License
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -59,23 +59,23 @@
                     token_dir=secret_path / 'token.json')
 ```
 
 To download dataframe:
 ```python
 import pandas as pd
 
-df = pd.from_gsheet(drive_table=table_name, 
+df = pd.from_gsheet(spreadsheet_id, 
                     sheet_name=sheet_name,
                     range_name='!A1:C100') # Range in Sheets; Optional
 ```
 Default `range_name` is `'!A1:ZZ900000'`.
 
 To upload dataframe:
 ```python
-df.to_gsheet(drive_table=table_name, 
+df.to_gsheet(spreadsheet_id, 
              sheet_name=sheet_name,
              range_name='!B1:ZZ900000', # Range in Sheets; Optional
              drop_columns=False) # Upload column names or not; Optional
 ```
 
 ### DriveConnection instance
 First, init DriveConnection instance:
@@ -84,22 +84,22 @@
 secret_path = Path('/path/to/my/secrets/').resolve()
 drive = DriveConnection(credentials_dir=secret_path / 'credentials.json', 
                         token_dir=secret_path / 'token.json')
 ```
 
 To download dataframe:
 ```python
-df = drive.download(drive_table=table_name, 
+df = drive.download(spreadsheet_id, 
                     sheet_name=sheet_name,
                     range_name='!A1:C100', # Range in Sheets; Optional
                     header=0) # Column row
 ```
 Default `range_name` is `'!A1:ZZ900000'`.
 
 To upload dataframe:
 ```python
 df = drive.upload(df,
-                    drive_table=table_name, 
-                    sheet_name=sheet_name,
-                    range_name='!B1:ZZ900000', # Range in Sheets; Optional
-                    drop_columns=False) # Upload column names or not; Optional
+                  spreadsheet_id, 
+                  sheet_name=sheet_name,
+                  range_name='!B1:ZZ900000', # Range in Sheets; Optional
+                  drop_columns=False) # Upload column names or not; Optional
 ```
```

