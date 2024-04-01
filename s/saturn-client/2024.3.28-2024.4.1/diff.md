# Comparing `tmp/saturn-client-2024.3.28.tar.gz` & `tmp/saturn-client-2024.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "saturn-client-2024.3.28.tar", last modified: Thu Mar 28 18:13:06 2024, max compression
+gzip compressed data, was "saturn-client-2024.4.1.tar", last modified: Mon Apr  1 18:15:00 2024, max compression
```

## Comparing `saturn-client-2024.3.28.tar` & `saturn-client-2024.4.1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 18:13:06.115163 saturn-client-2024.3.28/
--rw-r--r--   0 runner    (1001) docker     (127)     1506 2024-03-28 18:13:03.000000 saturn-client-2024.3.28/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      184 2024-03-28 18:13:03.000000 saturn-client-2024.3.28/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     6137 2024-03-28 18:13:06.115163 saturn-client-2024.3.28/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5125 2024-03-28 18:13:03.000000 saturn-client-2024.3.28/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-03-28 18:13:03.000000 saturn-client-2024.3.28/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 18:13:06.115163 saturn-client-2024.3.28/saturn_client/
--rw-r--r--   0 runner    (1001) docker     (127)      212 2024-03-28 18:13:03.000000 saturn-client-2024.3.28/saturn_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      502 2024-03-28 18:13:06.115163 saturn-client-2024.3.28/saturn_client/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 18:13:06.115163 saturn-client-2024.3.28/saturn_client/cli/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 18:13:03.000000 saturn-client-2024.3.28/saturn_client/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14178 2024-03-28 18:13:03.000000 saturn-client-2024.3.28/saturn_client/cli/commands.py
--rw-r--r--   0 runner    (1001) docker     (127)     4111 2024-03-28 18:13:03.000000 saturn-client-2024.3.28/saturn_client/cli/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    21211 2024-03-28 18:13:03.000000 saturn-client-2024.3.28/saturn_client/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     3842 2024-03-28 18:13:03.000000 saturn-client-2024.3.28/saturn_client/logs.py
--rw-r--r--   0 runner    (1001) docker     (127)     8121 2024-03-28 18:13:03.000000 saturn-client-2024.3.28/saturn_client/run.py
--rw-r--r--   0 runner    (1001) docker     (127)     1576 2024-03-28 18:13:03.000000 saturn-client-2024.3.28/saturn_client/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)      954 2024-03-28 18:13:03.000000 saturn-client-2024.3.28/saturn_client/tar_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 18:13:06.115163 saturn-client-2024.3.28/saturn_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6137 2024-03-28 18:13:06.000000 saturn-client-2024.3.28/saturn_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      594 2024-03-28 18:13:06.000000 saturn-client-2024.3.28/saturn_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-28 18:13:06.000000 saturn-client-2024.3.28/saturn_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-03-28 18:13:06.000000 saturn-client-2024.3.28/saturn_client.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-28 18:13:06.000000 saturn-client-2024.3.28/saturn_client.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-03-28 18:13:06.000000 saturn-client-2024.3.28/saturn_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-03-28 18:13:06.000000 saturn-client-2024.3.28/saturn_client.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      303 2024-03-28 18:13:06.115163 saturn-client-2024.3.28/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1510 2024-03-28 18:13:03.000000 saturn-client-2024.3.28/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)    68621 2024-03-28 18:13:03.000000 saturn-client-2024.3.28/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 18:15:00.676705 saturn-client-2024.4.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1506 2024-04-01 18:14:58.000000 saturn-client-2024.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-04-01 18:14:58.000000 saturn-client-2024.4.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-04-01 18:15:00.676705 saturn-client-2024.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-01 18:14:58.000000 saturn-client-2024.4.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-01 18:14:58.000000 saturn-client-2024.4.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 18:15:00.676705 saturn-client-2024.4.1/saturn_client/
+-rw-r--r--   0 runner    (1001) docker     (127)      212 2024-04-01 18:14:58.000000 saturn-client-2024.4.1/saturn_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      502 2024-04-01 18:15:00.676705 saturn-client-2024.4.1/saturn_client/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 18:15:00.672705 saturn-client-2024.4.1/saturn_client/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 18:14:58.000000 saturn-client-2024.4.1/saturn_client/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15635 2024-04-01 18:14:58.000000 saturn-client-2024.4.1/saturn_client/cli/commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4111 2024-04-01 18:14:58.000000 saturn-client-2024.4.1/saturn_client/cli/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24061 2024-04-01 18:14:58.000000 saturn-client-2024.4.1/saturn_client/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3842 2024-04-01 18:14:58.000000 saturn-client-2024.4.1/saturn_client/logs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8273 2024-04-01 18:14:58.000000 saturn-client-2024.4.1/saturn_client/run.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1576 2024-04-01 18:14:58.000000 saturn-client-2024.4.1/saturn_client/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)      954 2024-04-01 18:14:58.000000 saturn-client-2024.4.1/saturn_client/tar_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 18:15:00.672705 saturn-client-2024.4.1/saturn_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-04-01 18:15:00.000000 saturn-client-2024.4.1/saturn_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      594 2024-04-01 18:15:00.000000 saturn-client-2024.4.1/saturn_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 18:15:00.000000 saturn-client-2024.4.1/saturn_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-01 18:15:00.000000 saturn-client-2024.4.1/saturn_client.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 18:15:00.000000 saturn-client-2024.4.1/saturn_client.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-01 18:15:00.000000 saturn-client-2024.4.1/saturn_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-01 18:15:00.000000 saturn-client-2024.4.1/saturn_client.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-04-01 18:15:00.676705 saturn-client-2024.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1510 2024-04-01 18:14:58.000000 saturn-client-2024.4.1/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)    68621 2024-04-01 18:14:58.000000 saturn-client-2024.4.1/versioneer.py
```

### Comparing `saturn-client-2024.3.28/LICENSE` & `saturn-client-2024.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `saturn-client-2024.3.28/saturn_client/cli/commands.py` & `saturn-client-2024.4.1/saturn_client/cli/commands.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import json
 import logging
+import pprint
 
 from saturn_client.run import batch, setup_file_syncs, split
 
 import sys
 from os.path import join
 from typing import List, Optional
 from ruamel.yaml import YAML
@@ -17,15 +18,15 @@
     deserialize,
 )
 from saturn_client.core import (
     DataSource,
     ResourceStatus,
     SaturnConnection,
     ResourceType,
-    SaturnHTTPError,
+    SaturnHTTPError, ServerOptionTypes,
 )
 
 
 logging.basicConfig(level=logging.DEBUG)
 logging.getLogger("fsspec.generic").setLevel(logging.DEBUG)
 logging.getLogger("fsspec").setLevel(logging.DEBUG)
 logging.getLogger("fsspec.local").setLevel(logging.DEBUG)
@@ -417,42 +418,99 @@
     client = SaturnConnection()
     resource = client.get_resource(ResourceType.JOB, job_name, owner_name=owner)
     job_id = resource["state"]["id"]
     client.schedule(job_id, cron_schedule=cron_schedule, disable=disable)
     print_resource_op("Unscheduled" if disable else "Scheduled", ResourceType.JOB, job_name, owner)
 
 
+@cli.command("clone")
+@click.argument("resource_type")
+@click.argument("resource_name")
+@click.argument("new_resource_type")
+@click.argument("new_resource_name")
+@click.option(
+    "--command",
+    default=None,
+    required=False,
+)
+@click.option(
+    "--ide",
+    default=None,
+    required=False,
+)
+@click.option(
+    "--disk-space",
+    default=None,
+    required=False,
+)
+@click.option(
+    "--owner",
+    default=None,
+    required=False,
+    help="Resource owner name. Defaults to current auth identity.",
+)
+def clone_cli(
+    resource_type: str,
+    resource_name: str,
+    new_resource_type: str,
+    new_resource_name: str,
+    command: Optional[str] = None,
+    ide: Optional[str] = None,
+    disk_space: Optional[str] = None,
+    owner: Optional[str] = None,
+):
+    client = SaturnConnection()
+    client.clone(
+        resource_type,
+        resource_name,
+        new_resource_type,
+        new_resource_name,
+        command=command,
+        ide=ide,
+        disk_space=disk_space,
+        owner_name=owner,
+    )
+
+
 @cli.command("batch")
 @click.argument("input_file")
 def batch_cli(input_file):
     batch_info = deserialize(input_file)
     batch(batch_info)
 
+@cli.command("options")
+@click.option("--option-type", default=ServerOptionTypes.SIZES)
+@click.option("--glob")
+def options_cli(option_type: str = ServerOptionTypes.SIZES, glob: Optional[str] = None):
+    client = SaturnConnection()
+    results = client.list_options(option_type, glob=glob)
+    for r in results:
+        click.echo(pprint.pformat(r))
 
 @cli.command("split")
 @click.argument("recipe_template")
 @click.argument("batch_file")
-@click.argument("batch_size", type=int)
 @click.argument("local_commands_directory")
+@click.option("--batch-size", type=int, default=None)
 @click.option("--sync", multiple=True, default=[])
 @click.option("--remote-commands-directory", default=None)
 @click.option(
     "--skip-completed", is_flag=True, default=False, help="Whether to re-do completed runs"
 )
 @click.option(
     "--skip-failures", is_flag=True, default=False, help="Whether to re-do failed runs"
 )
 @click.option(
     "--max-jobs", help="maximum number of runs that will be scheduled", type=int, default=-1
 )
 def split_cli(
     recipe_template: str,
     batch_file: str,
-    batch_size: int,
     local_commands_directory: str,
+    batch_size: Optional[int] = None,
     sync: List[str] = [],
     remote_commands_directory: Optional[str] = None,
     skip_completed: bool = False,
     skip_failures: bool = False,
     max_jobs: int = -1,
 ):
     sync = list(sync)
@@ -467,17 +525,17 @@
         remote_commands_directory = local_commands_directory
     click.echo("splitting")
     include_completed = not skip_completed
     include_failures = not skip_failures
     split(
         recipe,
         batch_info,
-        batch_size,
         local_commands_directory,
         remote_commands_directory,
+        batch_size=batch_size,
         include_completed=include_completed,
         include_failures=include_failures,
         max_jobs=max_jobs,
     )
     sync.append(f"{local_commands_directory}:{remote_commands_directory}")
     setup_file_syncs(recipe, sync)
     with open(join(local_commands_directory, "recipe.yaml"), "w+") as f:
```

### Comparing `saturn-client-2024.3.28/saturn_client/cli/utils.py` & `saturn-client-2024.4.1/saturn_client/cli/utils.py`

 * *Files identical despite different names*

### Comparing `saturn-client-2024.3.28/saturn_client/core.py` & `saturn-client-2024.4.1/saturn_client/core.py`

 * *Files 10% similar despite different names*

```diff
@@ -26,34 +26,14 @@
 
 log = logging.getLogger("saturn-client")
 if log.level == logging.NOTSET:
     logging.basicConfig()
     log.setLevel(logging.INFO)
 
 
-class FSCallback(FileOpCallback):
-    def __init__(self, *args, **kwargs):
-        super().__init__(*args, **kwargs)
-        self.exclude_globs = kwargs.pop("exclude_globs", [])
-
-    def wrap(self, iterable):
-        for item in iterable:
-            source, dest = item
-            skip = False
-            for exclude_glob in self.exclude_globs:
-                if fnmatch(source, exclude_glob):
-                    skip = True
-                    break
-            if skip:
-                continue
-            else:
-                self.relative_update()
-                yield item
-
-
 def utcnow() -> str:
     return dt.datetime.now(tz=dt.timezone.utc).isoformat()
 
 
 class SaturnError(Exception):
     def __init__(self, message):
         super().__init__(message)
@@ -105,14 +85,24 @@
             # Check if value was pluralized
             resource_type = resource_type[:-1]
             if resource_type in types:
                 return resource_type
         raise SaturnError(f'resource type "{value}" not found')
 
 
+class ServerOptionTypes:
+    AUTO_SHUTOFF = "auto_shutoff"
+    DISK_SPACE = "disk_space"
+    SIZES = "sizes"
+
+    @classmethod
+    def values(cls) -> List[str]:
+        return [cls.AUTO_SHUTOFF, cls.DISK_SPACE, cls.SIZES]
+
+
 class ResourceStatus:
     """
     Enum for resource statuses
     """
 
     PENDING = "pending"
     RUNNING = "running"
@@ -222,14 +212,32 @@
             Get from ``/api/user/token``
         """
         self.settings = Settings(url, api_token)
 
         # test connection to raise errors early
         self._saturn_version = self._get_saturn_version()
 
+    def list_options(self, option_type: str, glob: Optional[str] = None) -> List:
+        if option_type not in ServerOptionTypes.values():
+            raise ValueError(f"unknown option {option_type}. must be one of {ServerOptionTypes.values()}")
+        url = urljoin(self.url, "api/info/servers")
+        response = requests.get(url, headers=self.settings.headers)
+        if not response.ok:
+            raise SaturnHTTPError.from_response(response)
+        results = response.json()[option_type]
+        if option_type != ServerOptionTypes.SIZES:
+            if glob:
+                results = [x for x in results if fnmatch(x, glob)]
+        else:
+            results = results.values()
+            if glob:
+                results = [x for x in results if fnmatch(x["name"], glob)]
+            results = sorted(results, key=lambda x: (x['gpu'], x['cores']))
+        return results
+
     @property
     def orgs(self) -> List[Dict[str, Any]]:
         url = urljoin(self.url, "api/orgs")
         response = requests.get(url, headers=self.settings.headers)
         if not response.ok:
             raise ValueError(response.reason)
         return response.json()["orgs"]
@@ -536,14 +544,24 @@
         url = urljoin(self.url, "api/recipes")
         response = requests.put(url, headers=self.settings.headers, json=recipe_dict)
         if not response.ok:
             raise SaturnHTTPError.from_response(response)
         result = response.json()
         return result
 
+    def create(self, recipe_dict: Dict[str, Any], enforce_unknown=True) -> Dict[str, Any]:
+        url = urljoin(self.url, "api/recipes")
+        params = {"enforce_unknown": "true" if enforce_unknown else "false"}
+        url = f"{url}?{urlencode(params)}"
+        response = requests.post(url, headers=self.settings.headers, json=recipe_dict)
+        if not response.ok:
+            raise SaturnHTTPError.from_response(response)
+        result = response.json()
+        return result
+
     def start(self, resource_type: str, resource_id: str, debug_mode: bool = False):
         url_name = ResourceType.get_url_name(resource_type)
         url = urljoin(self.url, f"api/{url_name}/{resource_id}/start")
         data = {"debug_mode": True} if debug_mode else None
         response = requests.post(url, headers=self.settings.headers, json=data)
         if not response.ok:
             raise SaturnHTTPError.from_response(response)
@@ -587,7 +605,51 @@
                 raise SaturnHTTPError.from_response(response)
 
         url = urljoin(f"{base_url}/", "unschedule" if disable else "schedule")
         response = requests.post(url, headers=self.settings.headers)
         if not response.ok:
             raise SaturnHTTPError.from_response(response)
         return response.json()
+
+    def clone(
+        self,
+        resource_type: str,
+        resource_name: str,
+        new_resource_type: str,
+        new_resource_name: str,
+        command: Optional[str] = None,
+        ide: Optional[str] = None,
+        disk_space: Optional[str] = None,
+        owner_name: Optional[str] = None,
+    ):
+        recipe = self.get_resource(
+            resource_type, resource_name, owner_name=owner_name, as_template=True
+        )
+        routes = recipe["spec"].get("routes")
+        if routes:
+            default_port = 8000 if recipe["type"] == "deployment" else 8888
+            routes = [x for x in routes if x["container_port"] != default_port]
+            if recipe["type"] == "workspace":
+                for r in routes:
+                    if r["visibility"] != "owner" and r["visibility"] != "org":
+                        r["visibility"] = "org"
+            recipe["spec"]["routes"] = routes
+
+        viewers = recipe["spec"].get("viewers")
+        if viewers:
+            viewers = [
+                x for x in viewers if x.get("route", {}).get("container_port", None) != default_port
+            ]
+            recipe["spec"]["viewers"] = viewers
+        recipe["spec"]["name"] = new_resource_name
+        recipe["type"] = new_resource_type
+        if recipe["type"] in {"deployment", "job"}:
+            recipe["spec"]["command"] = command
+        if recipe["type"] == "job":
+            recipe["spec"]["start_dind"] = False
+        if resource_type != "workspace" and new_resource_type == "workspace":
+            for repo in recipe["spec"]["git_repositories"]:
+                repo["on_restart"] = "preserve changes"
+        if resource_type == "workspace":
+            recipe["spec"]["ide"] = ide
+            recipe["spec"]["disk_space"] = disk_space
+        return self.create(recipe, enforce_unknown=False)
```

### Comparing `saturn-client-2024.3.28/saturn_client/logs.py` & `saturn-client-2024.4.1/saturn_client/logs.py`

 * *Files identical despite different names*

### Comparing `saturn-client-2024.3.28/saturn_client/run.py` & `saturn-client-2024.4.1/saturn_client/run.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import uuid
 from concurrent.futures import ThreadPoolExecutor, Future
 from dataclasses import dataclass, asdict
 
 from os.path import join, exists
 import os
 from tempfile import NamedTemporaryFile
-from typing import List, Dict, Tuple
+from typing import List, Dict, Tuple, Optional
 
 import click
 import fsspec
 from cytoolz import partition_all
 from fsspec.generic import GenericFileSystem
 from ruamel.yaml import YAML
 import fsspec.generic
@@ -144,17 +144,17 @@
             failures.append(r)
     return incomplete, failures, completed
 
 
 def split(
     recipe: Dict,
     batch_dict: Dict,
-    batch_size: int,
     local_commands_directory: str,
     remote_commands_directory: str,
+    batch_size: Optional[int] = None,
     include_completed: bool = False,
     include_failures: bool = False,
     max_jobs: int = -1,
 ) -> None:
     batch = Batch.from_dict(batch_dict)
     to_execute = []
     if not include_completed or not include_failures:
@@ -173,21 +173,25 @@
             click.echo(f"skipping {len(completed)} completed runs")
     else:
         click.echo(f"including {len(batch.runs)} runs")
         to_execute.extend(batch.runs)
     if max_jobs > 0:
         click.echo(f"found {len(to_execute)}. Only keeping {max_jobs}")
         to_execute = to_execute[:max_jobs]
-    chunks = partition_all(batch_size, to_execute)
+    if batch_size is None:
+        batch_size_int = batch.nprocs * 3
+    else:
+        batch_size_int = batch_size
+    chunks = partition_all(batch_size_int, to_execute)
     output_batch_files = []
     os.makedirs(local_commands_directory, exist_ok=True)
     for idx, chunk in enumerate(chunks):
         fpath = join(local_commands_directory, f"{idx}.json")
         remote_fpath = join(remote_commands_directory, f"{idx}.json")
-        sub = Batch(nprocs=batch.nprocs, runs=chunk, remote_output_path=batch.remote_output_path)
+        sub = Batch(nprocs=batch.nprocs, runs=list(chunk), remote_output_path=batch.remote_output_path)
         with open(fpath, "w+") as f:
             json.dump(asdict(sub), f)
         output_batch_files.append(remote_fpath)
     recipe["spec"]["command"] = [f"sc batch {x}" for x in output_batch_files]
 
 
 def setup_file_syncs(recipe: Dict, sync: List[str]) -> None:
```

### Comparing `saturn-client-2024.3.28/saturn_client/settings.py` & `saturn-client-2024.4.1/saturn_client/settings.py`

 * *Files identical despite different names*

### Comparing `saturn-client-2024.3.28/saturn_client/tar_utils.py` & `saturn-client-2024.4.1/saturn_client/tar_utils.py`

 * *Files identical despite different names*

### Comparing `saturn-client-2024.3.28/saturn_client.egg-info/SOURCES.txt` & `saturn-client-2024.4.1/saturn_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `saturn-client-2024.3.28/setup.py` & `saturn-client-2024.4.1/setup.py`

 * *Files identical despite different names*

### Comparing `saturn-client-2024.3.28/versioneer.py` & `saturn-client-2024.4.1/versioneer.py`

 * *Files identical despite different names*

