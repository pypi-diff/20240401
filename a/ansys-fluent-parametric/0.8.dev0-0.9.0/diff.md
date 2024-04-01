# Comparing `tmp/ansys_fluent_parametric-0.8.dev0.tar.gz` & `tmp/ansys_fluent_parametric-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ansys_fluent_parametric-0.8.dev0.tar", max compression
+gzip compressed data, was "ansys_fluent_parametric-0.9.0.tar", max compression
```

## Comparing `ansys_fluent_parametric-0.8.dev0.tar` & `ansys_fluent_parametric-0.9.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1089 2023-04-19 01:17:29.086752 ansys_fluent_parametric-0.8.dev0/LICENSE
--rw-r--r--   0        0        0     4503 2023-04-19 01:17:29.086752 ansys_fluent_parametric-0.8.dev0/README.rst
--rw-r--r--   0        0        0     1202 2023-04-19 01:17:29.090752 ansys_fluent_parametric-0.8.dev0/pyproject.toml
--rw-r--r--   0        0        0    24957 2023-04-19 01:17:29.478753 ansys_fluent_parametric-0.8.dev0/src/ansys/fluent/parametric/__init__.py
--rw-r--r--   0        0        0     9626 2023-04-19 01:17:29.090752 ansys_fluent_parametric-0.8.dev0/src/ansys/fluent/parametric/local/__init__.py
--rw-r--r--   0        0        0    10653 2023-04-19 01:17:29.090752 ansys_fluent_parametric-0.8.dev0/src/ansys/fluent/parametric/parameters.py
--rw-r--r--   0        0        0     5627 1970-01-01 00:00:00.000000 ansys_fluent_parametric-0.8.dev0/PKG-INFO
+-rw-r--r--   0        0        0     1089 2023-11-08 18:16:56.116758 ansys_fluent_parametric-0.9.0/LICENSE
+-rw-r--r--   0        0        0     4469 2023-11-08 18:16:56.116758 ansys_fluent_parametric-0.9.0/README.rst
+-rw-r--r--   0        0        0     1673 2023-11-08 18:16:56.120758 ansys_fluent_parametric-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0    26020 2023-11-08 18:16:56.412768 ansys_fluent_parametric-0.9.0/src/ansys/fluent/parametric/__init__.py
+-rw-r--r--   0        0        0     9620 2023-11-08 18:16:56.120758 ansys_fluent_parametric-0.9.0/src/ansys/fluent/parametric/local/__init__.py
+-rw-r--r--   0        0        0    10655 2023-11-08 18:16:56.120758 ansys_fluent_parametric-0.9.0/src/ansys/fluent/parametric/parameters.py
+-rw-r--r--   0        0        0     5624 1970-01-01 00:00:00.000000 ansys_fluent_parametric-0.9.0/PKG-INFO
```

### Comparing `ansys_fluent_parametric-0.8.dev0/LICENSE` & `ansys_fluent_parametric-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ansys_fluent_parametric-0.8.dev0/README.rst` & `ansys_fluent_parametric-0.9.0/README.rst`

 * *Files 5% similar despite different names*

```diff
@@ -6,69 +6,69 @@
    :target: https://docs.pyansys.com/
    :alt: PyAnsys
 
 .. |pypi| image:: https://img.shields.io/pypi/v/ansys-fluent-parametric.svg?logo=python&logoColor=white
    :target: https://pypi.org/project/ansys-fluent-parametric
    :alt: PyPI
 
-.. |GH-CI| image:: https://github.com/pyansys/pyfluent-parametric/actions/workflows/ci_cd.yml/badge.svg
-   :target: https://github.com/pyansys/pyfluent-parametric/actions/workflows/ci_cd.yml
+.. |GH-CI| image:: https://github.com/ansys/pyfluent-parametric/actions/workflows/ci_cd.yml/badge.svg
+   :target: https://github.com/ansys/pyfluent-parametric/actions/workflows/ci_cd.yml
    :alt: GH-CI
 
 .. |MIT| image:: https://img.shields.io/badge/License-MIT-yellow.svg
    :target: https://opensource.org/licenses/MIT
    :alt: MIT
 
 .. |black| image:: https://img.shields.io/badge/code%20style-black-000000.svg?style=flat
    :target: https://github.com/psf/black
    :alt: Black
 
-.. |pre-commit| image:: https://results.pre-commit.ci/badge/github/pyansys/pyfluent-parametric/main.svg
-   :target: https://results.pre-commit.ci/latest/github/pyansys/pyfluent-parametric/main
+.. |pre-commit| image:: https://results.pre-commit.ci/badge/github/ansys/pyfluent-parametric/main.svg
+   :target: https://results.pre-commit.ci/latest/github/ansys/pyfluent-parametric/main
    :alt: pre-commit.ci status
 
 Overview
 --------
 PyFluent-Parametric provides Pythonic access to Ansys Fluent's parametric
 workflows.
 
 Documentation and issues
 ------------------------
 For comprehensive information on PyFluent-Parametric, see the latest
-release `documentation <https://fluentparametric.docs.pyansys.com>`_.
+release `documentation <https://parametric.fluent.docs.pyansys.com>`_.
 
-On the `PyFluent-Parametric Issues <https://github.com/pyansys/pyfluent-parametric/issues>`_,
+On the `PyFluent-Parametric Issues <https://github.com/ansys/pyfluent-parametric/issues>`_,
 you can create issues to submit questions, report bugs, and request new features. To reach
-the PyAnsys support team, email `pyansys.support@ansys.com <pyansys.support@ansys.com>`_.
+the project support team, email `pyansys.core@ansys.com <pyansys.core@ansys.com>`_.
 
 Installation
 ------------
-The ``ansys-fluent-parametric`` package currently supports Python 3.7 through Python
-3.10 on Windows and Linux.
+The ``ansys-fluent-parametric`` package currently supports Python 3.9 through Python
+3.11 on Windows and Linux.
 
 Install the latest release from `PyPI
 <https://pypi.org/project/ansys-fluent-parametric/>`_ with:
 
 .. code:: console
 
    pip install ansys-fluent-parametric
 
 Alternatively, install the latest from `GitHub
-<https://github.com/pyansys/pyfluent-parametric>`_ with:
+<https://github.com/ansys/pyfluent-parametric>`_ with:
 
 .. code:: console
 
-   pip install git+https://github.com/pyansys/pyfluent-parametric.git
+   pip install git+https://github.com/ansys/pyfluent-parametric.git
 
 If you plan on doing local *development* of PyFluent with Git, install
 with:
 
 .. code:: console
 
-   git clone https://github.com/pyansys/pyfluent-parametric.git
+   git clone https://github.com/ansys/pyfluent-parametric.git
    cd pyfluent-parametric
    pip install pip -U
    pip install -e .
 
 Dependencies
 ------------
 You must have a locally-installed, licensed copy of Ansys to run Fluent. The
@@ -85,15 +85,15 @@
 the PyFluent-Parametric documentation.
 
 .. code:: python
 
    import ansys.fluent.core as pyfluent
    from ansys.fluent.parametric import ParametricStudy
    solver_session = pyfluent.launch_fluent(mode="solver")
-   study = ParametricStudy(solver_session.parametric_studies).initialize()
+   study = ParametricStudy(solver_session.parametric_studies)
    input_parameters_update = study.design_points["Base DP"].input_parameters
    input_parameters_update["inlet1_vel"] = 0.5
    study.design_points["Base DP"].input_parameters = input_parameters_update
    study.update_current_design_point()
    print(study.design_points["Base DP"].output_parameters)
 
 License and acknowledgments
```

### Comparing `ansys_fluent_parametric-0.8.dev0/pyproject.toml` & `ansys_fluent_parametric-0.9.0/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,37 +1,41 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 # Check https://python-poetry.org/docs/pyproject/ for all available sections
 name = "ansys-fluent-parametric"
-version = "0.8.dev0"
+version = "0.9.0"
 description = "A python wrapper for Ansys Fluent parametric workflows"
 license = "MIT"
 authors = ["ANSYS, Inc. <ansys.support@ansys.com>"]
 maintainers = ["PyAnsys developers <pyansys.maintainers@ansys.com>"]
 readme = "README.rst"
-repository = "https://github.com/pyansys/pyfluent-parametric"
+repository = "https://github.com/ansys/pyfluent-parametric"
 classifiers = [
     "Development Status :: 4 - Beta",
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 packages = [
     { include = "ansys", from = "src" },
 ]
 
 [tool.poetry.dependencies]
-python = ">=3.7,<4.0"
-importlib-metadata = {version = "^4.0", python = "<3.8"}
-ansys-fluent-core = "~=0.13.dev0"
+python = ">=3.9,<4.0"
+ansys-fluent-core = "~=0.18"
 h5py = ">=3.7.0"
 
+[tool.poetry.urls]
+"Documentation" = "https://parametric.fluent.docs.pyansys.com/"
+"Source" = "https://github.com/ansys/pyfluent-parametric"
+"Tracker" = "https://github.com/ansys/pyfluent-parametric/issues"
+
 [tool.black]
 line-length = 88
 
 [tool.isort]
 profile = "black"
 force_sort_within_sections = true
 line_length = 88
@@ -39,7 +43,22 @@
 src_paths = ["doc", "src", "tests"]
 
 [tool.coverage.run]
 source = ["ansys.fluent"]
 
 [tool.coverage.report]
 show_missing = true
+
+[tool.pytest.ini_options]
+testpaths = ["tests"]
+addopts = """
+-v
+--cov=ansys.fluent
+--cov-report html:cov_html
+--cov-config=.coveragerc
+--durations=0
+--show-capture=all
+"""
+markers = [
+    "fluent_version(version): Run tests based on Fluent version specification",
+    "self_hosted: Tests that will run on self-hosted machines"
+]
```

### Comparing `ansys_fluent_parametric-0.8.dev0/src/ansys/fluent/parametric/__init__.py` & `ansys_fluent_parametric-0.9.0/src/ansys/fluent/parametric/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 Example
 -------
 >>> from ansys.fluent.parametric import ParametricStudy
 
 Instantiate the study from a Fluent session that has already read a case:
 
->>> study1 = ParametricStudy(session.parametric_studies).initialize()
+>>> study1 = ParametricStudy(session.parametric_studies)
 
 Access and modify the input parameters of the base design point:
 
 >>> ip = study1.design_points["Base DP"].input_parameters
 >>> ip['vel_hot'] = 0.2
 >>> study1.design_points["Base DP"].input_parameters = ip
 
@@ -49,28 +49,28 @@
 >>> from ansys.fluent.parametric import ParametricSession
 >>> session1 = ParametricSession(case_filepath="elbow_params_2.cas.h5")
 >>> session1.studies['elbow_params_2-Solve'].design_points['Base DP'].input_parameters  # noqa: E501
 >>> study2 = session1.new_study()
 >>> session2 = ParametricSession(project_filepath="nozzle_para_named.flprj")
 """
 import logging
-from pathlib import Path
+from pathlib import Path, PurePosixPath, PureWindowsPath
 import tempfile
 from typing import Any, Dict, List, Optional
 
 import ansys.fluent.core as pyfluent
 
 logger = logging.getLogger("ansys.fluent")
 
 try:
     import importlib.metadata as importlib_metadata
 except ModuleNotFoundError:
     import importlib_metadata
 
-_VERSION_INFO = "Build date: April 19, 2023 01:17 UTC ShaID: 5f527ac"
+_VERSION_INFO = "Build date: November 08, 2023 18:16 UTC ShaID: e3d6af6"
 __version__ = importlib_metadata.version(__name__.replace(".", "-"))
 
 
 def version_info() -> str:
     """Method returning the version of PyFluent being used.
 
     Returns
@@ -146,79 +146,84 @@
 
     A parametric study is used to parametrize design points in a Fluent solver
     set up. This class provides the ability to run Fluent for a series of
     design points and access or modify input and output parameters.
 
     Parameters
     ----------
-    parametric_studies :
-
+    parametric_studies : Session.parametric_studies
+        ``parametric_studies`` object of a Fluent session.
     session : Session, optional
         Connected Fluent session. The default is ``None``.
     name : str, optional
         Name of the parametric study. The default is ``None``.
     design_points : Dict[str, DesignPoint], optional
         Dictionary of design points under the parametric study by name.
         The default is ``None``.
+    initialize : bool, optional
+        Whether to initialize the parametric study. The default is ``True``.
     """
 
     def __init__(
         self,
         parametric_studies,
         session=None,
         name: Optional[str] = None,
         design_points: Dict[str, DesignPoint] = None,
+        initialize: Optional[bool] = True,
     ):
         self._parametric_studies = parametric_studies
         self.session = (
             session if session is not None else (_shared_parametric_study_registry())
         )
         self.name = name
         self.design_points = {}
         if design_points is not None:
             self.design_points = design_points
         self.project_filepath = None
         self.session.register_study(self)
+        if initialize:
+            if self._parametric_studies.initialize.is_active():
+                self.project_filepath = Path(
+                    tempfile.mkdtemp(
+                        prefix="project-",
+                        suffix=".cffdb",
+                        dir=str(Path.cwd()),  # TODO: should be cwd of server
+                    )
+                )
+                self.project_filepath.rmdir()
+                old_study_names = self._parametric_studies.get_object_names()
+                self._parametric_studies.initialize(
+                    project_filename=self.project_filepath.stem
+                )
+                new_study_names = self._parametric_studies.get_object_names()
+                self.name = set(new_study_names).difference(set(old_study_names)).pop()
+                base_design_point = DesignPoint(
+                    BASE_DP_NAME,
+                    self._parametric_studies[self.name],
+                )
+                self.design_points = {BASE_DP_NAME: base_design_point}
+                self.session.current_study_name = self.name
+            else:
+                logging.error("Initialize is not available.")
 
     def get_all_studies(self) -> Dict[str, "ParametricStudy"]:
         """Get all currently active studies.
 
         Returns
         -------
         Dict[str, "ParametricStudy"]
             Dictionary of all currently active studies.
         """
         return {v.name: v for _, v in self.session._all_studies.items()}
 
-    def initialize(self) -> "ParametricStudy":
-        """Initialize the parametric study."""
-        if self._parametric_studies.initialize.is_active():
-            self.project_filepath = Path(
-                tempfile.mkdtemp(
-                    prefix="project-",
-                    suffix=".cffdb",
-                    dir=str(Path.cwd()),  # TODO: should be cwd of server
-                )
-            )
-            self.project_filepath.rmdir()
-            old_study_names = self._parametric_studies.get_object_names()
-            self._parametric_studies.initialize(
-                project_filename=self.project_filepath.stem
-            )
-            new_study_names = self._parametric_studies.get_object_names()
-            self.name = set(new_study_names).difference(set(old_study_names)).pop()
-            base_design_point = DesignPoint(
-                BASE_DP_NAME,
-                self._parametric_studies[self.name],
-            )
-            self.design_points = {BASE_DP_NAME: base_design_point}
-            self.session.current_study_name = self.name
-            return self
-        else:
-            logging.error("Initialize is not available.")
+    def reset_study_registry(self):
+        """Reset parametric studies registry."""
+        self.session.clear_registry()
+        self.session.register_study(self)
 
     def rename(self, new_name: str) -> None:
         """Rename the parametric study.
 
         Parameters
         ----------
         new_name : str
@@ -269,15 +274,19 @@
         else:
             base_design_point = DesignPoint(
                 BASE_DP_NAME,
                 self._parametric_studies[clone_name],
             )
             clone_design_points = {BASE_DP_NAME: base_design_point}
         clone = ParametricStudy(
-            self._parametric_studies, self.session, clone_name, clone_design_points
+            self._parametric_studies,
+            self.session,
+            clone_name,
+            clone_design_points,
+            initialize=False,
         )
         self.session.current_study_name = clone.name
         return clone
 
     def delete(self) -> None:
         """Delete the parametric study."""
         if self.is_current:
@@ -503,21 +512,28 @@
         Parameters
         ----------
         project_filepath : str, optional
             Project filename. The default is ``"default.flprj"``.
         load_case : bool, optional
             Whether to load the current case. The default ``True``.
         """
+        if (
+            not PureWindowsPath(project_filepath).is_absolute()
+            or not PurePosixPath(project_filepath).is_absolute()
+        ):
+            project_filepath = str(Path(project_filepath).resolve())
         self._parametric_project.open(
-            project_filename=str(Path(project_filepath).resolve()),
+            project_filename=project_filepath,
             load_case=load_case,
         )
         self.project_filepath = project_filepath
         for study_name in self._parametric_studies.get_object_names():
-            study = ParametricStudy(self._parametric_studies, self.session, study_name)
+            study = ParametricStudy(
+                self._parametric_studies, self.session, study_name, initialize=False
+            )
             dps_settings = self._parametric_studies[study_name].design_points
             for dp_name in dps_settings.get_object_names():
                 study.design_points[dp_name] = DesignPoint(
                     dp_name, self._parametric_studies[study_name]
                 )
 
     def save(self) -> None:
@@ -584,14 +600,17 @@
     def __init__(self):
         self._all_studies: Dict[int, "ParametricStudy"] = {}
         self.current_study_name = None
 
     def register_study(self, study):
         self._all_studies[id(study)] = study
 
+    def clear_registry(self):
+        self._all_studies = {}
+
 
 class ParametricSession(ParametricStudyRegistry):
     """Provides for encapsulating studies and projects.
 
     Attributes
     ----------
     studies : Dict[str, ParametricStudy]
@@ -615,42 +634,47 @@
 
     def __init__(
         self,
         case_filepath: str = None,
         project_filepath: str = None,
         launcher: Any = ParametricSessionLauncher(),
         start_transcript: bool = False,
+        initialize: bool = True,
     ):
         """Instantiate a ParametricSession.
 
         Parameters
         ----------
         case_filepath : str, optional
             Case file name. The default is ``None``.
         project_filepath : str, optional
             Project file name. The default is ``None``.
         launcher : _type_, optional
             Fluent launcher. The default is ``ParametricSessionLauncher()``.
         start_transcript : bool, optional
             Whether to start streaming of a Fluent transcript. The default
             is ``False``.
+        initialize : bool, optional
+            Whether to initialize the ParametricStudy instances created. Default is ``True``.
         """
         super().__init__()
         self.studies = {}
         self.project = None
         self._session = launcher()
         self.scheme_eval = self._session.scheme_eval.scheme_eval
         self.scheme_eval(
             "(set parametric-study-dependents-manager " "save-project-at-exit? #f)"
         )
         if not start_transcript:
             self.stop_transcript()
         if case_filepath is not None:
             self._session.file.read(file_name=case_filepath, file_type="case")
-            study = ParametricStudy(self._session.parametric_studies, self).initialize()
+            study = ParametricStudy(
+                self._session.parametric_studies, self, initialize=initialize
+            )
             self.studies[study.name] = study
             self.project = ParametricProject(
                 parametric_project=self._session.file.parametric_project,
                 parametric_studies=self._session.parametric_studies,
                 project_filepath=str(study.project_filepath),
                 open_project=False,
                 session=self,
@@ -660,15 +684,17 @@
                 parametric_project=self._session.file.parametric_project,
                 parametric_studies=self._session.parametric_studies,
                 project_filepath=project_filepath,
                 session=self,
             )
             studies_settings = self._session.parametric_studies
             for study_name in studies_settings.get_object_names():
-                study = ParametricStudy(studies_settings, self, study_name)
+                study = ParametricStudy(
+                    studies_settings, self, study_name, initialize=initialize
+                )
                 dps_settings = studies_settings[study_name].design_points
                 for dp_name in dps_settings.get_object_names():
                     study.design_points[dp_name] = DesignPoint(
                         dp_name, studies_settings[study_name]
                     )
                 self.studies[study_name] = study
             self.current_study_name = self._session.current_parametric_study()
@@ -721,19 +747,19 @@
         return self
 
     def __exit__(self, exc_type: Any, exc_val: Any, exc_tb: Any):
         self._session.exit()
 
     def start_transcript(self) -> None:
         """Start streaming of a Fluent transcript."""
-        self._session.start_transcript()
+        self._session.transcript.start()
 
     def stop_transcript(self) -> None:
         """Stop streaming of a Fluent transcript."""
-        self._session.stop_transcript()
+        self._session.transcript.stop()
 
 
 def _shared_parametric_study_registry():
     if _shared_parametric_study_registry.instance is None:
         _shared_parametric_study_registry.instance = ParametricStudyRegistry()
     return _shared_parametric_study_registry.instance
```

### Comparing `ansys_fluent_parametric-0.8.dev0/src/ansys/fluent/parametric/local/__init__.py` & `ansys_fluent_parametric-0.9.0/src/ansys/fluent/parametric/local/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 
 """
 
 from math import ceil
 from typing import Any, Dict, Union
 
 from ansys.fluent.core.filereader.casereader import CaseReader
-from ansys.fluent.core.utils.async_execution import asynchronous
+from ansys.fluent.core.utils.execution import asynchronous
 
 from ansys.fluent.parametric import (
     BASE_DP_NAME,
     ParametricSession,
     ParametricSessionLauncher,
 )
```

### Comparing `ansys_fluent_parametric-0.8.dev0/src/ansys/fluent/parametric/parameters.py` & `ansys_fluent_parametric-0.9.0/src/ansys/fluent/parametric/parameters.py`

 * *Files 1% similar despite different names*

```diff
@@ -162,19 +162,19 @@
         Returns
         -------
         str
             Unit label of the Fluent input parameter.
 
         """
         value = str(self[name])
-        value_split = value.split(maxsplit=1)
+        value_split = value.split("[", maxsplit=1)
         if len(value_split) == 1:
             return ""
         else:
-            return value_split[1].lstrip("[").rstrip("]")
+            return value_split[-1].strip().rstrip("]")
 
     def __setitem__(self, name: str, value: V) -> None:
         """Set value of an input parameter.
 
         Parameters
         ----------
         name : str
```

### Comparing `ansys_fluent_parametric-0.8.dev0/PKG-INFO` & `ansys_fluent_parametric-0.9.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,101 +1,101 @@
 Metadata-Version: 2.1
 Name: ansys-fluent-parametric
-Version: 0.8.dev0
+Version: 0.9.0
 Summary: A python wrapper for Ansys Fluent parametric workflows
-Home-page: https://github.com/pyansys/pyfluent-parametric
+Home-page: https://github.com/ansys/pyfluent-parametric
 License: MIT
 Author: ANSYS, Inc.
 Author-email: ansys.support@ansys.com
 Maintainer: PyAnsys developers
 Maintainer-email: pyansys.maintainers@ansys.com
-Requires-Python: >=3.7,<4.0
+Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3
-Requires-Dist: ansys-fluent-core (>=0.13.dev0,<1.0)
+Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: ansys-fluent-core (>=0.18,<1.0)
 Requires-Dist: h5py (>=3.7.0)
-Requires-Dist: importlib-metadata (>=4.0,<5.0) ; python_version < "3.8"
-Project-URL: Repository, https://github.com/pyansys/pyfluent-parametric
+Project-URL: Documentation, https://parametric.fluent.docs.pyansys.com/
+Project-URL: Repository, https://github.com/ansys/pyfluent-parametric
+Project-URL: Source, https://github.com/ansys/pyfluent-parametric
+Project-URL: Tracker, https://github.com/ansys/pyfluent-parametric/issues
 Description-Content-Type: text/x-rst
 
 PyFluent-Parametric
 ===================
 |pyansys| |pypi| |GH-CI| |MIT| |black| |pre-commit|
 
 .. |pyansys| image:: https://img.shields.io/badge/Py-Ansys-ffc107.svg?logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABAAAAAQCAIAAACQkWg2AAABDklEQVQ4jWNgoDfg5mD8vE7q/3bpVyskbW0sMRUwofHD7Dh5OBkZGBgW7/3W2tZpa2tLQEOyOzeEsfumlK2tbVpaGj4N6jIs1lpsDAwMJ278sveMY2BgCA0NFRISwqkhyQ1q/Nyd3zg4OBgYGNjZ2ePi4rB5loGBhZnhxTLJ/9ulv26Q4uVk1NXV/f///////69du4Zdg78lx//t0v+3S88rFISInD59GqIH2esIJ8G9O2/XVwhjzpw5EAam1xkkBJn/bJX+v1365hxxuCAfH9+3b9/+////48cPuNehNsS7cDEzMTAwMMzb+Q2u4dOnT2vWrMHu9ZtzxP9vl/69RVpCkBlZ3N7enoDXBwEAAA+YYitOilMVAAAAAElFTkSuQmCC
    :target: https://docs.pyansys.com/
    :alt: PyAnsys
 
 .. |pypi| image:: https://img.shields.io/pypi/v/ansys-fluent-parametric.svg?logo=python&logoColor=white
    :target: https://pypi.org/project/ansys-fluent-parametric
    :alt: PyPI
 
-.. |GH-CI| image:: https://github.com/pyansys/pyfluent-parametric/actions/workflows/ci_cd.yml/badge.svg
-   :target: https://github.com/pyansys/pyfluent-parametric/actions/workflows/ci_cd.yml
+.. |GH-CI| image:: https://github.com/ansys/pyfluent-parametric/actions/workflows/ci_cd.yml/badge.svg
+   :target: https://github.com/ansys/pyfluent-parametric/actions/workflows/ci_cd.yml
    :alt: GH-CI
 
 .. |MIT| image:: https://img.shields.io/badge/License-MIT-yellow.svg
    :target: https://opensource.org/licenses/MIT
    :alt: MIT
 
 .. |black| image:: https://img.shields.io/badge/code%20style-black-000000.svg?style=flat
    :target: https://github.com/psf/black
    :alt: Black
 
-.. |pre-commit| image:: https://results.pre-commit.ci/badge/github/pyansys/pyfluent-parametric/main.svg
-   :target: https://results.pre-commit.ci/latest/github/pyansys/pyfluent-parametric/main
+.. |pre-commit| image:: https://results.pre-commit.ci/badge/github/ansys/pyfluent-parametric/main.svg
+   :target: https://results.pre-commit.ci/latest/github/ansys/pyfluent-parametric/main
    :alt: pre-commit.ci status
 
 Overview
 --------
 PyFluent-Parametric provides Pythonic access to Ansys Fluent's parametric
 workflows.
 
 Documentation and issues
 ------------------------
 For comprehensive information on PyFluent-Parametric, see the latest
-release `documentation <https://fluentparametric.docs.pyansys.com>`_.
+release `documentation <https://parametric.fluent.docs.pyansys.com>`_.
 
-On the `PyFluent-Parametric Issues <https://github.com/pyansys/pyfluent-parametric/issues>`_,
+On the `PyFluent-Parametric Issues <https://github.com/ansys/pyfluent-parametric/issues>`_,
 you can create issues to submit questions, report bugs, and request new features. To reach
-the PyAnsys support team, email `pyansys.support@ansys.com <pyansys.support@ansys.com>`_.
+the project support team, email `pyansys.core@ansys.com <pyansys.core@ansys.com>`_.
 
 Installation
 ------------
-The ``ansys-fluent-parametric`` package currently supports Python 3.7 through Python
-3.10 on Windows and Linux.
+The ``ansys-fluent-parametric`` package currently supports Python 3.9 through Python
+3.11 on Windows and Linux.
 
 Install the latest release from `PyPI
 <https://pypi.org/project/ansys-fluent-parametric/>`_ with:
 
 .. code:: console
 
    pip install ansys-fluent-parametric
 
 Alternatively, install the latest from `GitHub
-<https://github.com/pyansys/pyfluent-parametric>`_ with:
+<https://github.com/ansys/pyfluent-parametric>`_ with:
 
 .. code:: console
 
-   pip install git+https://github.com/pyansys/pyfluent-parametric.git
+   pip install git+https://github.com/ansys/pyfluent-parametric.git
 
 If you plan on doing local *development* of PyFluent with Git, install
 with:
 
 .. code:: console
 
-   git clone https://github.com/pyansys/pyfluent-parametric.git
+   git clone https://github.com/ansys/pyfluent-parametric.git
    cd pyfluent-parametric
    pip install pip -U
    pip install -e .
 
 Dependencies
 ------------
 You must have a locally-installed, licensed copy of Ansys to run Fluent. The
@@ -112,15 +112,15 @@
 the PyFluent-Parametric documentation.
 
 .. code:: python
 
    import ansys.fluent.core as pyfluent
    from ansys.fluent.parametric import ParametricStudy
    solver_session = pyfluent.launch_fluent(mode="solver")
-   study = ParametricStudy(solver_session.parametric_studies).initialize()
+   study = ParametricStudy(solver_session.parametric_studies)
    input_parameters_update = study.design_points["Base DP"].input_parameters
    input_parameters_update["inlet1_vel"] = 0.5
    study.design_points["Base DP"].input_parameters = input_parameters_update
    study.update_current_design_point()
    print(study.design_points["Base DP"].output_parameters)
 
 License and acknowledgments
```

