# Comparing `tmp/gha_ci_detector-0.0.2.tar.gz` & `tmp/gha_ci_detector-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gha_ci_detector-0.0.2.tar", max compression
+gzip compressed data, was "gha_ci_detector-0.0.3.tar", max compression
```

## Comparing `gha_ci_detector-0.0.2.tar` & `gha_ci_detector-0.0.3.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0      563 2024-03-20 12:03:21.639794 gha_ci_detector-0.0.2/pyproject.toml
--rw-r--r--   0        0        0      764 2024-03-20 10:21:06.293790 gha_ci_detector-0.0.2/src/gha_ci_detector/Job.py
--rw-r--r--   0        0        0     1522 2024-03-20 11:55:54.208580 gha_ci_detector-0.0.2/src/gha_ci_detector/Runner.py
--rw-r--r--   0        0        0      917 2024-03-19 13:51:24.401222 gha_ci_detector-0.0.2/src/gha_ci_detector/Step.py
--rw-r--r--   0        0        0      794 2024-03-20 10:21:06.317789 gha_ci_detector-0.0.2/src/gha_ci_detector/Workflow.py
--rw-r--r--   0        0        0      262 2024-03-19 14:46:16.945400 gha_ci_detector-0.0.2/src/gha_ci_detector/__init__.py
--rw-r--r--   0        0        0      176 2024-03-20 11:54:37.560360 gha_ci_detector-0.0.2/src/gha_ci_detector/__main__.py
--rw-r--r--   0        0        0     1474 2024-03-20 10:21:46.052619 gha_ci_detector-0.0.2/src/gha_ci_detector/cli.py
--rw-r--r--   0        0        0    15035 2024-03-20 11:56:12.492635 gha_ci_detector-0.0.2/src/gha_ci_detector/smell_detector.py
--rw-r--r--   0        0        0      477 2024-03-20 09:04:15.699729 gha_ci_detector-0.0.2/src/gha_ci_detector/util.py
--rw-r--r--   0        0        0      669 1970-01-01 00:00:00.000000 gha_ci_detector-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0      563 2024-04-01 10:13:51.793371 gha_ci_detector-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0      796 2024-03-20 12:29:49.514364 gha_ci_detector-0.0.3/src/gha_ci_detector/Job.py
+-rw-r--r--   0        0        0     1522 2024-03-20 11:55:54.208580 gha_ci_detector-0.0.3/src/gha_ci_detector/Runner.py
+-rw-r--r--   0        0        0     1296 2024-03-22 10:11:11.790929 gha_ci_detector-0.0.3/src/gha_ci_detector/Step.py
+-rw-r--r--   0        0        0     1425 2024-03-22 10:04:39.072487 gha_ci_detector-0.0.3/src/gha_ci_detector/Workflow.py
+-rw-r--r--   0        0        0      262 2024-03-19 14:46:16.945400 gha_ci_detector-0.0.3/src/gha_ci_detector/__init__.py
+-rw-r--r--   0        0        0      176 2024-03-20 11:54:37.560360 gha_ci_detector-0.0.3/src/gha_ci_detector/__main__.py
+-rw-r--r--   0        0        0     1474 2024-03-20 10:21:46.052619 gha_ci_detector-0.0.3/src/gha_ci_detector/cli.py
+-rw-r--r--   0        0        0    15998 2024-03-22 10:13:36.595844 gha_ci_detector-0.0.3/src/gha_ci_detector/smell_detector.py
+-rw-r--r--   0        0        0      511 2024-03-20 12:29:08.222242 gha_ci_detector-0.0.3/src/gha_ci_detector/util.py
+-rw-r--r--   0        0        0      669 1970-01-01 00:00:00.000000 gha_ci_detector-0.0.3/PKG-INFO
```

### Comparing `gha_ci_detector-0.0.2/pyproject.toml` & `gha_ci_detector-0.0.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name="gha-ci-detector"
-version="0.0.2"
+version="0.0.3"
 authors = [
     "Cedric Willekens <cedric@willekens.dev>"
 ]
 description = "A tool created to detect CI Smells as part of a master thesis at the TU Delft. "
 
 [tool.poetry.dependencies]
 python = "^3.8"
```

### Comparing `gha_ci_detector-0.0.2/src/gha_ci_detector/Job.py` & `gha_ci_detector-0.0.3/src/gha_ci_detector/Job.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from typing import Optional
+
 from gha_ci_detector.Step import Step
 
 
 class Job:
     def __init__(self, name, yaml):
         self.name = name
         self.yaml: dict = yaml
@@ -13,15 +15,15 @@
         if "steps" in self.yaml.keys():
             return list(map(lambda x: Step(x), self.yaml["steps"]))
         else:
             return [Step({
                 "uses": self.yaml["uses"]
             })]
 
-    def get_if(self) -> str | None:
+    def get_if(self) -> Optional[str]:
         if "if" in self.yaml.keys():
             return self.yaml["if"]
         else:
             return None
 
     def __str__(self):
         return "Job: \n" + self.name + " " + str(self.yaml) + "\n"
```

### Comparing `gha_ci_detector-0.0.2/src/gha_ci_detector/Runner.py` & `gha_ci_detector-0.0.3/src/gha_ci_detector/Runner.py`

 * *Files identical despite different names*

### Comparing `gha_ci_detector-0.0.2/src/gha_ci_detector/Workflow.py` & `gha_ci_detector-0.0.3/src/gha_ci_detector/Workflow.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from typing import Optional
+
 import gha_ci_detector.util as util
 from gha_ci_detector.Job import Job
 
 
 class Workflow:
     def __init__(self, file_content: str, name: str = ""):
         self.file_content: str = file_content
@@ -17,12 +19,27 @@
     def get_jobs(self) -> list[Job]:
         jobs = self.yaml['jobs']
         return list(map(lambda x: Job(x, self.yaml['jobs'][x]), jobs))
 
     def get_keys(self) -> list[str]:
         return list(self.yaml.keys())
 
-    def get_on(self) -> dict | None:
+    def get_on(self) -> Optional[dict]:
         if 'on' in self.yaml.keys():
             return self.yaml["on"]
         else:
             return None
+
+    def __get_stripped_lines(self) -> list[str]:
+        return list(map(lambda x: x.strip(), self.file_content.split("\n")))
+
+    def __get_lines_without_spaces(self) -> list[str]:
+        return list(map(lambda x: x.replace(" ", ""), self.__get_stripped_lines()))
+
+    def get_line_number(self, line: str, use_whitespace: bool = True) -> Optional[int]:
+        try:
+            if use_whitespace:
+                return self.__get_stripped_lines().index(line)
+            else:
+                return self.__get_lines_without_spaces().index(line)
+        except ValueError:
+            return -1
```

### Comparing `gha_ci_detector-0.0.2/src/gha_ci_detector/cli.py` & `gha_ci_detector-0.0.3/src/gha_ci_detector/cli.py`

 * *Files identical despite different names*

### Comparing `gha_ci_detector-0.0.2/src/gha_ci_detector/smell_detector.py` & `gha_ci_detector-0.0.3/src/gha_ci_detector/smell_detector.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import re
+from typing import Optional
 
 from yamllint import linter, config
 
 from gha_ci_detector.Job import Job
 from gha_ci_detector.Step import Step
 from gha_ci_detector.Workflow import Workflow
 
@@ -108,35 +109,39 @@
     """
     Runs on should use a fixed version and not 'latest'
     :param workflow:
     :return:
     """
     lines = workflow.file_content.split("\n")
     runs_on_lines = list(filter(lambda x: "runs-on" in x and "latest" in x, lines))
-    if len(runs_on_lines) > 0:
-        workflow.smells.add("Use fixed version for runs-on argument")
+    for line in runs_on_lines:
+        line_nr = lines.index(line)
+        workflow.smells.add(f"Use fixed version for runs-on argument (line {line_nr})")
 
 
 def use_specific_version_instead_of_dynamic(workflow: Workflow) -> None:
     """
     Check if a version is updated to contain more dots or is changed from latest to something
     else or is updated to be a hash value
     Using tags is as versions for actions is a known security problem
     :param workflow:
     :return:
     """
     lines = workflow.file_content.split("\n")
     uses_lines = filter(lambda x: "uses:" in x, lines)
     for line in uses_lines:
+        line_nr = lines.index(line)
         versions = line.split("@")
         if len(versions) == 1:
-            workflow.smells.add("Use commit hash instead of tags for action versions")
+            workflow.smells.add(f"Use commit hash instead of tags for action versions (line "
+                                f"{line_nr})")
             continue
         if "v" in versions[1] or "." in versions[1]:
-            workflow.smells.add("Use commit hash instead of tags for action versions")
+            workflow.smells.add(f"Use commit hash instead of tags for action versions (line "
+                                f"{line_nr})")
 
 
 def action_should_have_timeout(workflow: Workflow) -> None:
     """
     TODO: Try to compile a list of actions on github which tend to run long?
           Or try to compile a list of actions which access the outside world?
           Differentiate between jobs having a timeout and steps having a timeout.
@@ -149,15 +154,15 @@
             workflow.smells.add("Avoid jobs without timeouts")
 
 
 def use_cache_from_setup(workflow: Workflow) -> None:
     """
     Many setup/install actions such as `setup-node` already provide a cache for the downloaded libraries
     Should it be desirable to have the cache param even when they are not yet doing caching?
-    :param change:
+    :param workflow:
     :return:
     """
     cacheable_actions = ["actions/setup-python", "actions/setup-java", "actions/setup-node"]
     for job in workflow.get_jobs():
         is_cachable_action = False
         is_cache_action = False
         for index, step in enumerate(job.get_steps()):
@@ -183,15 +188,16 @@
                 workflow.smells.add("Avoid executing  scheduled workflows on forks")
 
 
 def use_name_for_step(workflow: Workflow) -> None:
     for job in workflow.get_jobs():
         for step in job.get_steps():
             if "name" not in step.yaml.keys():
-                workflow.smells.add("Use names for run steps")
+                (start, end) = step.get_line_numbers(workflow.get_line_number)
+                workflow.smells.add(f"Use names for run steps (lines {start}:{end})")
 
 
 def stop_workflows_for_old_commit(workflow: Workflow) -> None:
     """
     TODO: How to differentiate between branch and PR?
           Should this apply for every kind of workflow?
     :param workflow:
@@ -205,44 +211,50 @@
 
 def upload_artifact_must_have_if(workflow: Workflow) -> None:
     for job in workflow.get_jobs():
         for step in job.get_steps():
             if "uses" in step.yaml.keys() and ("actions/upload-artifact" in step.yaml["uses"] or
                                                "coverallsapp/github-action" in step.yaml["uses"]):
                 if step.get_if() is None:
-                    workflow.smells.add("Use 'if' for upload-artifact action")
+                    stripped = step.yaml["uses"].strip()
+                    line_nr = workflow.get_line_number(f"uses: {stripped}".replace(" ", ""),
+                                                       use_whitespace=False)
+                    workflow.smells.add(f"Use 'if' for upload-artifact action (line {line_nr})")
                 else:
                     if not (("github.repository" in step.get_if() or "github.repository_owner"
                              in step.get_if()) and (
                                     job.get_if() is not None and (
                                     "github.repository" in job.get_if()
                                     or "github.repository_owner" in job.get_if()))):
                         workflow.smells.add("Avoid uploading artifacts on forks")
             elif step.get_name() is not None and "upload" in step.get_name().lower():
                 if (step.get_if() is None) or not (("github.repository" in step.get_if() or
                                                     "github.repository_owner"
                                                     in step.get_if()) and (
                                                            job.get_if() is not None and (
                                                            "github.repository" in job.get_if()
                                                            or "github.repository_owner" in job.get_if()))):
-                    workflow.smells.add("Avoid uploading artifacts on forks")
+                    (start, end) = step.get_line_numbers(workflow.get_line_number)
+                    workflow.smells.add(f"Avoid uploading artifacts on forks (line {start}:{end})")
 
 
 def multi_line_steps(workflow: Workflow) -> None:
     """
     TODO: This smell still needs to be renamed
     :param workflow:
     :return:
     """
     for job in workflow.get_jobs():
         for step in job.get_steps():
             if "run" in step.yaml.keys():
                 run = step.yaml["run"]
                 if "\n" in run or "&&" in run:
-                    workflow.smells.add("Steps should only perform a single command")
+                    line_nr = workflow.get_line_number(run.split("\n")[0])
+                    workflow.smells.add(f"Steps should only perform a single command (line "
+                                        f"{line_nr})")
 
 
 def comment_in_workflow(workflow: Workflow) -> None:
     source_code = workflow.file_content
     if not source_code.startswith("#"):
         workflow.smells.add("Avoid workflows without comments")
 
@@ -300,24 +312,26 @@
             if "run" in step.yaml.keys():
                 run = step.yaml["run"]
                 lines = run.split("\n")
                 for l in lines:
                     if "install" in l:
                         version = re.search("(==[0-9]+.[0-9]+.[0-9]+)", l)
                         if version is None:
-                            workflow.smells.add("Avoid installing packages without version")
+                            line_nr = workflow.get_line_number(l.strip())
+                            workflow.smells.add("Avoid installing packages without version (line "
+                                                f"{line_nr})")
 
 
 def running_workflow_through_bot(workflow: Workflow) -> None:
     for job in workflow.get_jobs():
         if job.get_if() is None or "github.actor !=" in job.get_if():
             workflow.smells.add("Avoid running workflow when a bot has made a change in the repo")
 
 
-def detect_yaml_duplication(workflows: list[Workflow]) -> str | None:
+def detect_yaml_duplication(workflows: list[Workflow]) -> Optional[str]:
     jobs = {}
     for w in workflows:
         for j in w.get_jobs():
             key = w.name + "-" + j.name
             step_list = []
             for index in range(0, len(j.get_steps()) - 2):
                 step_list.append([j.get_steps()[index], j.get_steps()[index + 1], j.get_steps()[
```

### Comparing `gha_ci_detector-0.0.2/PKG-INFO` & `gha_ci_detector-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gha-ci-detector
-Version: 0.0.2
+Version: 0.0.3
 Summary: A tool created to detect CI Smells as part of a master thesis at the TU Delft. 
 Author: Cedric Willekens
 Author-email: cedric@willekens.dev
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

