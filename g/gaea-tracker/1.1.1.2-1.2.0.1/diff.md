# Comparing `tmp/gaea_tracker-1.1.1.2-py3-none-any.whl.zip` & `tmp/gaea_tracker-1.2.0.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 5738 bytes, number of entries: 8
--rw-r--r--  2.0 unx      213 b- defN 24-Mar-25 11:22 gaea_tracker/__init__.py
--rw-r--r--  2.0 unx     1654 b- defN 24-Mar-25 11:22 gaea_tracker/aim_tracker.py
--rw-r--r--  2.0 unx     7146 b- defN 24-Mar-25 11:22 gaea_tracker/experiment_tracker.py
--rw-r--r--  2.0 unx     1459 b- defN 24-Mar-25 11:22 gaea_tracker/mlflow_tracker.py
--rw-r--r--  2.0 unx     1745 b- defN 24-Mar-25 11:23 gaea_tracker-1.1.1.2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Mar-25 11:23 gaea_tracker-1.1.1.2.dist-info/WHEEL
--rw-r--r--  2.0 unx       13 b- defN 24-Mar-25 11:23 gaea_tracker-1.1.1.2.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      668 b- defN 24-Mar-25 11:23 gaea_tracker-1.1.1.2.dist-info/RECORD
-8 files, 12990 bytes uncompressed, 4566 bytes compressed:  64.8%
+Zip file size: 5823 bytes, number of entries: 8
+-rw-r--r--  2.0 unx      213 b- defN 24-Apr-01 13:21 gaea_tracker/__init__.py
+-rw-r--r--  2.0 unx     1654 b- defN 24-Apr-01 13:21 gaea_tracker/aim_tracker.py
+-rw-r--r--  2.0 unx     7573 b- defN 24-Apr-01 13:21 gaea_tracker/experiment_tracker.py
+-rw-r--r--  2.0 unx     1459 b- defN 24-Apr-01 13:21 gaea_tracker/mlflow_tracker.py
+-rw-r--r--  2.0 unx     1745 b- defN 24-Apr-01 13:30 gaea_tracker-1.2.0.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-01 13:30 gaea_tracker-1.2.0.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       13 b- defN 24-Apr-01 13:30 gaea_tracker-1.2.0.1.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      668 b- defN 24-Apr-01 13:30 gaea_tracker-1.2.0.1.dist-info/RECORD
+8 files, 13417 bytes uncompressed, 4651 bytes compressed:  65.3%
```

## zipnote {}

```diff
@@ -6,20 +6,20 @@
 
 Filename: gaea_tracker/experiment_tracker.py
 Comment: 
 
 Filename: gaea_tracker/mlflow_tracker.py
 Comment: 
 
-Filename: gaea_tracker-1.1.1.2.dist-info/METADATA
+Filename: gaea_tracker-1.2.0.1.dist-info/METADATA
 Comment: 
 
-Filename: gaea_tracker-1.1.1.2.dist-info/WHEEL
+Filename: gaea_tracker-1.2.0.1.dist-info/WHEEL
 Comment: 
 
-Filename: gaea_tracker-1.1.1.2.dist-info/top_level.txt
+Filename: gaea_tracker-1.2.0.1.dist-info/top_level.txt
 Comment: 
 
-Filename: gaea_tracker-1.1.1.2.dist-info/RECORD
+Filename: gaea_tracker-1.2.0.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## gaea_tracker/experiment_tracker.py

```diff
@@ -32,14 +32,15 @@
             experiment_kind: str = "Aim",
             project_name: str = None):
         self.windmill_client = windmill_client
         self._experiment_name = experiment_name
         self.config_param = {}
         self._work_dir = ""
         self._job_work_dir = ""
+        self._extra_work_dir = ""
         self._project_name = project_name
         self._job_kind = "train"
 
         self._job_name = None
         if self._project_name is not None:
             self._job_name = self._get_windmill_job()
         # 如果run name为空，则job name作为run name
@@ -88,14 +89,21 @@
     def work_dir(self):
         """
         Get work dir.
         """
         return self._work_dir
 
     @property
+    def extra_work_dir(self):
+        """
+        Get extra work dir.
+        """
+        return self._extra_work_dir
+
+    @property
     def job_work_dir(self):
         """
         Get work dir.
         """
         return self._job_work_dir
 
     @property
@@ -132,39 +140,43 @@
                                                 local_name=local_name)
         experiment_runs = response.experimentRuns
         if experiment_runs is None:
             experiment_runs = {}
         experiment_runs.update({self.job_kind: run_id})
         self.windmill_client.update_job(workspace_id=workspace_id,
                                         project_name=project_name,
+                                        display_name=response.displayName,
                                         local_name=local_name,
                                         experiment_runs=experiment_runs)
 
     def _get_windmill_job(self):
         """
         Get windmill job.
         """
         project_instance = parse_project_name(self.project_name)
         workspace_id, project_name = project_instance.workspace_id, project_instance.local_name
         if "PF_RUN_ID" in os.environ and "PF_STEP_NAME" in os.environ:
             paddleflow_run_id = os.environ["PF_RUN_ID"]
             self._job_kind = os.environ["PF_STEP_NAME"]
             self._work_dir = os.environ["PF_WORK_DIR"]
+            self._extra_work_dir = os.environ["PF_EXTRA_WORK_DIR"]
             response = self.windmill_client.get_job(workspace_id=workspace_id,
                                                     project_name=project_name,
                                                     local_name=paddleflow_run_id,
                                                     naming_kind="runID")
             assert response.name is not None, \
                 f"The job name is empty, " \
                 f"please check your request workspace_id={workspace_id} project_name={project_name} " \
                 f"local_name={paddleflow_run_id} naming_kind=runID, " \
                 f"response is {response}"
             name = response.name
             self.config_param = {"org_id": response.orgID, "project_name": response.projectName}
             self._job_work_dir = os.path.join(self.work_dir, name, self._job_kind)
+            if not os.path.exists(self._job_work_dir):
+                os.makedirs(self._job_work_dir, exist_ok=True)
         else:
             self.config_param = {"org_id": "", "project_name": ""}
             name = ""
             self._work_dir = ""
             self._job_work_dir = ""
 
         return name
```

## Comparing `gaea_tracker-1.1.1.2.dist-info/METADATA` & `gaea_tracker-1.2.0.1.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gaea-tracker
-Version: 1.1.1.2
+Version: 1.2.0.1
 Summary: A common tracker library.
 Home-page: https://console.cloud.baidu-int.com/devops/icode/repos/baidu/mlops/gaea-operator/tree/master
 Author: liuyawen03
 Author-email: liuyawen03@baidu.com
 License: MIT
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

## Comparing `gaea_tracker-1.1.1.2.dist-info/RECORD` & `gaea_tracker-1.2.0.1.dist-info/RECORD`

 * *Files 22% similar despite different names*

```diff
@@ -1,8 +1,8 @@
 gaea_tracker/__init__.py,sha256=W_LJdwsPO-i_I_labqmA9UtINpc16H_xrUMtH3BgJrg,213
 gaea_tracker/aim_tracker.py,sha256=B8WcwJPQC6hKy-NMeZOYY6rQ4-cER_2j0zrxdPcNlxQ,1654
-gaea_tracker/experiment_tracker.py,sha256=3MlocwH1L3Lb26bG3_NbehqpjPCz2SrZKKZOJqw2qTs,7146
+gaea_tracker/experiment_tracker.py,sha256=ULDYol1gwQZK2JjOAVgNJonZC3x5-bojh0nI76gOfXo,7573
 gaea_tracker/mlflow_tracker.py,sha256=iSHBX25D1K5Ss1Jnhyq_2q9KAeizhOz_LTXIVcU3OXE,1459
-gaea_tracker-1.1.1.2.dist-info/METADATA,sha256=yD92iP2MjXJyd-6W3CGcm60nxx3rvQROYEVm_xVtUAk,1745
-gaea_tracker-1.1.1.2.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-gaea_tracker-1.1.1.2.dist-info/top_level.txt,sha256=puBG5QOAqx9ZaALXFt41yG0oBynhWzrKEJOMgH__hYw,13
-gaea_tracker-1.1.1.2.dist-info/RECORD,,
+gaea_tracker-1.2.0.1.dist-info/METADATA,sha256=eINhu9r2iQZ16cgJyRPxltiiArs25xtGM61LXtKAZrE,1745
+gaea_tracker-1.2.0.1.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+gaea_tracker-1.2.0.1.dist-info/top_level.txt,sha256=puBG5QOAqx9ZaALXFt41yG0oBynhWzrKEJOMgH__hYw,13
+gaea_tracker-1.2.0.1.dist-info/RECORD,,
```

