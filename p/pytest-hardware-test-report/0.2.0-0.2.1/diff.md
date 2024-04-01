# Comparing `tmp/pytest_hardware_test_report-0.2.0.tar.gz` & `tmp/pytest_hardware_test_report-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest_hardware_test_report-0.2.0.tar", max compression
+gzip compressed data, was "pytest_hardware_test_report-0.2.1.tar", max compression
```

## Comparing `pytest_hardware_test_report-0.2.0.tar` & `pytest_hardware_test_report-0.2.1.tar`

### file list

```diff
@@ -1,6 +1,7 @@
--rw-r--r--   0        0        0    13411 2024-03-31 18:09:04.543932 pytest_hardware_test_report-0.2.0/README.md
--rw-r--r--   0        0        0     1563 2024-03-31 18:09:04.543932 pytest_hardware_test_report-0.2.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-03-31 18:09:04.543932 pytest_hardware_test_report-0.2.0/pytest_htr/__init__.py
--rw-r--r--   0        0        0    17352 2024-03-31 18:09:04.543932 pytest_hardware_test_report-0.2.0/pytest_htr/plugin.py
--rw-r--r--   0        0        0     3470 2024-03-31 18:09:04.543932 pytest_hardware_test_report-0.2.0/pytest_htr/serialize.py
--rw-r--r--   0        0        0    14629 1970-01-01 00:00:00.000000 pytest_hardware_test_report-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1070 2024-04-01 19:06:53.136486 pytest_hardware_test_report-0.2.1/LICENSE
+-rw-r--r--   0        0        0    15410 2024-04-01 19:06:53.136486 pytest_hardware_test_report-0.2.1/README.md
+-rw-r--r--   0        0        0     1567 2024-04-01 19:06:53.136486 pytest_hardware_test_report-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-01 19:06:53.136486 pytest_hardware_test_report-0.2.1/pytest_htr/__init__.py
+-rw-r--r--   0        0        0    17250 2024-04-01 19:06:53.136486 pytest_hardware_test_report-0.2.1/pytest_htr/plugin.py
+-rw-r--r--   0        0        0     3470 2024-04-01 19:06:53.136486 pytest_hardware_test_report-0.2.1/pytest_htr/serialize.py
+-rw-r--r--   0        0        0    16681 1970-01-01 00:00:00.000000 pytest_hardware_test_report-0.2.1/PKG-INFO
```

### Comparing `pytest_hardware_test_report-0.2.0/README.md` & `pytest_hardware_test_report-0.2.1/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -9,30 +9,36 @@
 It can report a summary, test details, captured output, logs, exception tracebacks and more. Additionally, you can use the available fixtures and hooks to [add metadata](#metadata) and [customize](#modifying-the-report) the report as you like.
 
 ## Table of contents
 
 * [Installation](#installation)
 * [Options](#options)
 * [Usage](#usage)
-   * [Metadata](#metadata)
-   * [Modifying the report](#modifying-the-report)
-   * [Direct invocation](#direct-invocation)
-* [Format](#format)
-   * [Summary](#summary)
-   * [Environment](#environment)
-   * [Collectors](#collectors)
-   * [Tests](#tests)
-   * [Test stage](#test-stage)
-   * [Log](#log)
-   * [Warnings](#warnings)
+  * [Fixtures](#fixtures)
+    * [json_dut](#json_dut)
+    * [json_equipment](#json_equipment)
+    * [json_metadata](#json_metadata)
+  * [Advanced Usage](#advanced-usage)
+    * [DUT](#dut)
+    * [Equipment](#equipment)
+    * [Metadata](#metadata)
+    * [Modifying the report](#modifying-the-report)
+  * [Direct invocation](#direct-invocation)
+  * [Format](#format)
+  * [Summary](#summary)
+  * [Environment](#environment)
+  * [Tests](#tests)
+  * [Test stage](#test-stage)
+  * [Log](#log)
+  * [Warnings](#warnings)
 * [Related tools](#related-tools)
 
 ## Installation
 
-```
+```bash
 pip install pytest-hardware-test-report --upgrade 
 ```
 
 ## Options
 
 | Option | Description |
 | --- | --- |
@@ -52,68 +58,119 @@
 $ cat .report.json
 {"created": 1518371686.7981803, ... "tests":[{"nodeid": "test_foo.py", "outcome": "passed", ...}, ...]}
 ```
 
 If you just need to know how many tests passed or failed and don't care about details, you can produce a summary only:
 
 ```bash
-$ pytest --json-report --json-report-summary
+pytest --hw-test-report --hw-test-report-summary
 ```
 
 Many fields can be omitted to keep the report size small. E.g., this will leave out keywords and stdout/stderr output:
 
 ```bash
-$ pytest --json-report --json-report-omit keywords streams
+pytest --hw-test-report --hw-test-report-omit keywords streams
 ```
 
 If you don't like to have the report saved, you can specify `none` as the target file name:
 
 ```bash
-$ pytest --json-report --json-report-file none
+pytest --hw-test-report --hw-test-report-file none
 ```
 
-## Advanced usage
+### Fixtures
+
+#### json_dut
+
+To record information about the device under test in the report you can use the `json_dut` [test fixture](https://docs.pytest.org/en/stable/fixture.html). This also works if your DUT is, itself, a fixture:
+
+```python
+@pytest.fixture(name="dut")
+def dut_fixture(json_dut):
+    json_dut['serial no'] = 1234567
+    json_dut['version'] = 1.0.0
+    dut = setup_dut()
+    yield dut
+    dut.teardown()
+```
+
+#### json_equipment
 
-### Metadata
+To record information about any test equipment you may use in the report you can use the `json_equipment` [test fixture](https://docs.pytest.org/en/stable/fixture.html):
+
+```python
+def equipment1(json_equipment):
+    json_equipment['equipment1'] = {'manufacturer': 'Test Inc.', 'Model': 'Testomatic 300'}
+```
+
+#### json_metadata
 
 The easiest way to add your own metadata to a test item is by using the `json_metadata` [test fixture](https://docs.pytest.org/en/stable/fixture.html):
 
 ```python
 def test_something(json_metadata):
     json_metadata['foo'] = {"some": "thing"}
     json_metadata['bar'] = 123
 ```
 
-Or use the `pytest_json_runtest_metadata` [hook](https://docs.pytest.org/en/stable/reference.html#hooks) (in your `conftest.py`) to add metadata based on the current test run. The dict returned will automatically be merged with any existing metadata. E.g., this adds the start and stop time of each test's `call` stage:
+## Advanced usage
+
+### Hooks
+
+If you're using a `pytest_json_*` hook although the plugin is not installed or not active (not using `--json-report`), pytest doesn't recognize it and may fail with an internal error like this:
+
+```bash
+INTERNALERROR> pluggy.manager.PluginValidationError: unknown hook 'pytest_json_runtest_metadata' in plugin <module 'conftest' from 'conftest.py'>
+```
+
+You can avoid this by declaring the hook implementation optional:
 
 ```python
+import pytest
+@pytest.hookimpl(optionalhook=True)
 def pytest_json_runtest_metadata(item, call):
-    if call.when != 'call':
+    ...
+```
+
+#### DUT
+
+Or use the `pytest_json_runtest_dut` [hook](https://docs.pytest.org/en/stable/reference.html#hooks) (in your `conftest.py`) to add metadata based on the current test run. The dict returned will automatically be merged with any existing metadata. E.g., this adds the start and stop time of each test's `setup` stage:
+
+```python
+def pytest_json_runtest_dut(item, call):
+    if call.when != 'setup':
         return {}
     return {'start': call.start, 'stop': call.stop}
 ```
 
-Also, you could add metadata using [pytest-metadata's `--metadata` switch](https://github.com/pytest-dev/pytest-metadata#additional-metadata) which will add metadata to the report's `environment` section, but not to a specific test item. You need to make sure all your metadata is JSON-serializable.
+#### Equipment
 
-### A note on hooks
+Or use the `pytest_json_runtest_equipment` [hook](https://docs.pytest.org/en/stable/reference.html#hooks) (in your `conftest.py`) to add metadata based on the current test run. The dict returned will automatically be merged with any existing metadata. E.g., this adds the start and stop time of each test's `setup` stage:
 
-If you're using a `pytest_json_*` hook although the plugin is not installed or not active (not using `--json-report`), pytest doesn't recognize it and may fail with an internal error like this:
-```
-INTERNALERROR> pluggy.manager.PluginValidationError: unknown hook 'pytest_json_runtest_metadata' in plugin <module 'conftest' from 'conftest.py'>
+```python
+def pytest_json_runtest_equipment(item, call):
+    if call.when != 'setup':
+        return {}
+    return {'start': call.start, 'stop': call.stop}
 ```
-You can avoid this by declaring the hook implementation optional:
+
+#### Metadata
+
+Or use the `pytest_json_runtest_metadata` [hook](https://docs.pytest.org/en/stable/reference.html#hooks) (in your `conftest.py`) to add metadata based on the current test run. The dict returned will automatically be merged with any existing metadata. E.g., this adds the start and stop time of each test's `call` stage:
 
 ```python
-import pytest
-@pytest.hookimpl(optionalhook=True)
 def pytest_json_runtest_metadata(item, call):
-    ...
+    if call.when != 'call':
+        return {}
+    return {'start': call.start, 'stop': call.stop}
 ```
 
-### Modifying the report
+Also, you could add metadata using [pytest-metadata's `--metadata` switch](https://github.com/pytest-dev/pytest-metadata#additional-metadata) which will add metadata to the report's `environment` section, but not to a specific test item. You need to make sure all your metadata is JSON-serializable.
+
+#### Modifying the report
 
 You can modify the entire report before it's saved by using the `pytest_json_modifyreport` hook.
 
 Just implement the hook in your `conftest.py`, e.g.:
 
 ```python
 def pytest_json_modifyreport(json_report):
@@ -143,91 +200,90 @@
 You can use the plugin when invoking `pytest.main()` directly from code:
 
 ```python
 import pytest
 from pytest_htr.plugin import JSONReport
 
 plugin = JSONReport()
-pytest.main(['--json-report-file=none', 'test_foo.py'], plugins=[plugin])
+pytest.main(['--hw-test-report-file=none', 'test_foo.py'], plugins=[plugin])
 ```
 
 You can then access the `report` object:
 
 ```python
 print(plugin.report)
 ```
 
 And save the report manually:
 
 ```python
 plugin.save_report('/tmp/my_report.json')
 ```
 
-
 ## Format
 
-The JSON report contains metadata of the session, a summary, collectors, tests and warnings. You can find a sample report in [`sample_report.json`](sample_report.json).
+The JSON report contains metadata of the session, a summary, tests and warnings. You can find a sample report in [`sample_report.json`](sample_report.json).
 
 | Key | Description |
 | --- | --- |
 | `created` | Report creation date. (Unix time) |
 | `duration` | Session duration in seconds. |
 | `exitcode` | Process exit code as listed [in the pytest docs](https://docs.pytest.org/en/latest/usage.html#possible-exit-codes). The exit code is a quick way to tell if any tests failed, an internal error occurred, etc. |
 | `root` | Absolute root path from which the session was started. |
 | `environment` | [Environment](#environment) entry. |
 | `summary` | [Summary](#summary) entry. |
-| `tests` | [Tests](#tests) entry. (absent if `--json-report-summary`)  |
-| `warnings` | [Warnings](#warnings) entry. (absent if `--json-report-summary` or if no warnings)  |
+| `tests` | [Tests](#tests) entry. (absent if `--hw-test-report-summary`)  |
+| `warnings` | [Warnings](#warnings) entry. (absent if `--hw-test-report-summary` or if no warnings)  |
 
-#### Example
+### Format Example
 
 ```python
 {
     "created": 1518371686.7981803,
     "duration": 0.1235666275024414,
     "exitcode": 1,
     "root": "/path/to/tests",
     "environment": ENVIRONMENT,
     "summary": SUMMARY,
     "tests": TESTS,
     "warnings": WARNINGS,
 }
 ```
 
-### Summary
+## Summary
 
 Number of outcomes per category and the total number of test items.
 
 | Key | Description |
 | --- | --- |
 |  `collected` | Total number of tests collected. |
 |  `total` | Total number of tests run. |
 |  `deselected` | Total number of tests deselected. (absent if number is 0) |
 | `<outcome>` | Number of tests with that outcome. (absent if number is 0) |
 
-#### Example
+### Summary Example
 
 ```python
 {
     "collected": 10,
     "passed": 2,
     "failed": 3,
     "xfailed": 1,
     "xpassed": 1,
     "error": 2,
     "skipped": 1,
     "total": 10
 }
 ```
 
-### Environment
+## Environment
 
 The environment section is provided by [pytest-metadata](https://github.com/pytest-dev/pytest-metadata). All metadata given by that plugin will be added here, so you need to make sure it is JSON-serializable.
 
-#### Example
+### Environment Example
 
 ```python
 {
     "Python": "3.6.4",
     "Platform": "Linux-4.56.78-9-ARCH-x86_64-with-arch",
     "Packages": {
         "pytest": "3.4.0",
@@ -241,28 +297,28 @@
         "forked": "0.2",
         "cov": "2.5.1"
     },
     "foo": "bar", # Custom metadata entry passed via pytest-metadata
 }
 ```
 
-### Tests
+## Tests
 
 A list of test nodes. Each completed test stage produces a stage object (`setup`, `call`, `teardown`) with its own `outcome`.
 
 | Key | Description |
 | --- | --- |
 | `nodeid` | ID of the test node. |
 | `outcome` | Outcome of the test run. |
 | `DUT` | DUT item. (absent if not present) |
 | `equipment` | equipment item. (absent if not present) |
 | `{setup, call, teardown}` | [Test stage](#test-stage) entry. To find the error in a failed test you need to check all stages. (absent if stage didn't run) |
 | `metadata` | [Metadata](#metadata) item. (absent if no metadata) |
 
-#### Example
+### Tests Example
 
 ```python
 [
     {
         "nodeid": "test_foo.py::test_fail",
         "outcome": "failed",
         "DUT": {
@@ -283,31 +339,30 @@
             "foo": "bar",
         }
     },
     ...
 ]
 ```
 
-
-### Test stage
+## Test stage
 
 A test stage item.
 
 | Key | Description |
 | --- | --- |
 | `duration` | Duration of the test stage in seconds. |
 | `outcome` | Outcome of the test stage. (can be different from the overall test outcome) |
 | `crash` | Crash entry. (absent if no error occurred) |
 | `traceback` | List of traceback entries. (absent if no error occurred; affected by `--tb` option) |
 | `stdout` | Standard output. (absent if none available) |
 | `stderr` | Standard error. (absent if none available) |
 | `log` | [Log](#log) entry. (absent if none available) |
 | `longrepr` | Representation of the error. (absent if no error occurred; format affected by `--tb` option) |
 
-#### Example
+### Test stage Example
 
 ```python
 {
     "duration": 0.00018835067749023438,
     "outcome": "failed",
     "crash": {
         "path": "/path/to/tests/test_foo.py",
@@ -339,21 +394,21 @@
     "stdout": "foo\nbar\n",
     "stderr": "baz\n",
     "log": LOG,
     "longrepr": "def test_fail_nested():\n ..."
 }
 ```
 
-### Log
+## Log
 
 A list of log records. The fields of a log record are the [`logging.LogRecord` attributes](https://docs.python.org/3/library/logging.html#logrecord-attributes), with the exception that the fields `exc_info` and `args` are always empty and `msg` contains the formatted log message.
 
 You can apply [`logging.makeLogRecord()`](https://docs.python.org/3/library/logging.html#logging.makeLogRecord)  on a log record to convert it back to a `logging.LogRecord` object.
 
-#### Example
+### Log Example
 
 ```python
 [
     {
         "name": "root",
         "msg": "This is a warning.",
         "args": null,
@@ -375,39 +430,38 @@
         "processName": "MainProcess",
         "process": 31481
     },
     ...
 ]
 ```
 
-
-### Warnings
+## Warnings
 
 A list of warnings that occurred during the session. (See the [pytest docs on warnings](https://docs.pytest.org/en/latest/warnings.html).)
 
 | Key | Description |
 | --- | --- |
 | `filename` | File name. |
 | `lineno` | Line number. |
 | `message` | Warning message. |
 | `when` | When the warning was captured. (`"config"`, `"collect"` or `"runtest"` as listed [here](https://docs.pytest.org/en/latest/reference.html#_pytest.hookspec.pytest_warning_captured)) |
 
-#### Example
+### Warnings Example
 
 ```python
 [
     {
         "code": "C1",
         "path": "/path/to/tests/test_foo.py",
         "nodeid": "test_foo.py::TestFoo",
         "message": "cannot collect test class 'TestFoo' because it has a __init__ constructor"
     }
 ]
 ```
 
 ## Related tools
 
--[pytest-json-report](https://github.com/numirias/pytest-json-report) Heavily inspired by this plugin. It is more suited for pure software testing but i have borrow large ammounts of code from there.
+* [pytest-json-report](https://github.com/numirias/pytest-json-report) Heavily inspired by this plugin. It is more suited for pure software testing but i have borrow large ammounts of code from there.
 
-- [pytest-json](https://github.com/mattcl/pytest-json) has some great features but appears to be unmaintained. I borrowed some ideas and test cases from there.
+* [pytest-json](https://github.com/mattcl/pytest-json) has some great features but appears to be unmaintained. I borrowed some ideas and test cases from there.
 
-- [tox has a switch](http://tox.readthedocs.io/en/latest/example/result.html) to create a JSON report including a test result summary. However, it just provides the overall outcome without any per-test details.
+* [tox has a switch](http://tox.readthedocs.io/en/latest/example/result.html) to create a JSON report including a test result summary. However, it just provides the overall outcome without any per-test details.
```

### Comparing `pytest_hardware_test_report-0.2.0/pyproject.toml` & `pytest_hardware_test_report-0.2.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [tool.poetry]
 name = "pytest-hardware-test-report"
-version = "0.2.0"
+version = "0.2.1"
 description = "A simple plugin to use with pytest"
 authors = [
     "Matthew Trott <trottmpq@gmail.com>"
 ]
 maintainers = [
     "Matthew Trott <trottmpq@gmail.com>"
 ]
 readme = "README.md"
-license = "MIT"
+license = "LICENSE"
 packages = [
     {include = "pytest_htr"}
 ]
 classifiers = [
     "Framework :: Pytest",
     "Development Status :: 4 - Beta",
     "Intended Audience :: Developers",
```

### Comparing `pytest_hardware_test_report-0.2.0/pytest_htr/plugin.py` & `pytest_hardware_test_report-0.2.1/pytest_htr/plugin.py`

 * *Files 1% similar despite different names*

```diff
@@ -242,17 +242,15 @@
             created=datetime.datetime.fromtimestamp(time.time()).isoformat(),
             duration=time.time() - self._start_time,
             exitcode=session.exitstatus,
             root=str(session.fspath),
             environment=self._config.stash.get(metadata_key, {}),
             summary=serialize.make_summary(self._json_tests, **summary_data),
         )
-        if not self._config.option.json_report_summary:
-            # if self._json_collectors:
-            #     json_report["collectors"] = self._json_collectors
+        if not self._config.option.hw_test_report_summary:
             json_report["tests"] = list(self._json_tests.values())
             if self._json_warnings:
                 json_report["warnings"] = self._json_warnings
 
         self._config.hook.pytest_json_modifyreport(json_report=json_report)
         # After the session has finished, other scripts may want to use report
         # object directly
@@ -434,15 +432,15 @@
         "--hw-test-report-omit",
         default=[],
         nargs="+",
         help="list of fields to omit in the report "
         "(choose from: log, traceback, streams, warnings)",
     )
     group.addoption(
-        "--json-report-summary",
+        "--hw-test-report-summary",
         default=False,
         action="store_true",
         help="only create a summary without per-test details",
     )
     group.addoption(
         "--hw-test-report-indent",
         type=int,
```

### Comparing `pytest_hardware_test_report-0.2.0/pytest_htr/serialize.py` & `pytest_hardware_test_report-0.2.1/pytest_htr/serialize.py`

 * *Files identical despite different names*

### Comparing `pytest_hardware_test_report-0.2.0/PKG-INFO` & `pytest_hardware_test_report-0.2.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: pytest-hardware-test-report
-Version: 0.2.0
+Version: 0.2.1
 Summary: A simple plugin to use with pytest
-License: MIT
+License: LICENSE
 Author: Matthew Trott
 Author-email: trottmpq@gmail.com
 Maintainer: Matthew Trott
 Maintainer-email: trottmpq@gmail.com
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: Pytest
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
+Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
@@ -39,30 +40,36 @@
 It can report a summary, test details, captured output, logs, exception tracebacks and more. Additionally, you can use the available fixtures and hooks to [add metadata](#metadata) and [customize](#modifying-the-report) the report as you like.
 
 ## Table of contents
 
 * [Installation](#installation)
 * [Options](#options)
 * [Usage](#usage)
-   * [Metadata](#metadata)
-   * [Modifying the report](#modifying-the-report)
-   * [Direct invocation](#direct-invocation)
-* [Format](#format)
-   * [Summary](#summary)
-   * [Environment](#environment)
-   * [Collectors](#collectors)
-   * [Tests](#tests)
-   * [Test stage](#test-stage)
-   * [Log](#log)
-   * [Warnings](#warnings)
+  * [Fixtures](#fixtures)
+    * [json_dut](#json_dut)
+    * [json_equipment](#json_equipment)
+    * [json_metadata](#json_metadata)
+  * [Advanced Usage](#advanced-usage)
+    * [DUT](#dut)
+    * [Equipment](#equipment)
+    * [Metadata](#metadata)
+    * [Modifying the report](#modifying-the-report)
+  * [Direct invocation](#direct-invocation)
+  * [Format](#format)
+  * [Summary](#summary)
+  * [Environment](#environment)
+  * [Tests](#tests)
+  * [Test stage](#test-stage)
+  * [Log](#log)
+  * [Warnings](#warnings)
 * [Related tools](#related-tools)
 
 ## Installation
 
-```
+```bash
 pip install pytest-hardware-test-report --upgrade 
 ```
 
 ## Options
 
 | Option | Description |
 | --- | --- |
@@ -82,68 +89,119 @@
 $ cat .report.json
 {"created": 1518371686.7981803, ... "tests":[{"nodeid": "test_foo.py", "outcome": "passed", ...}, ...]}
 ```
 
 If you just need to know how many tests passed or failed and don't care about details, you can produce a summary only:
 
 ```bash
-$ pytest --json-report --json-report-summary
+pytest --hw-test-report --hw-test-report-summary
 ```
 
 Many fields can be omitted to keep the report size small. E.g., this will leave out keywords and stdout/stderr output:
 
 ```bash
-$ pytest --json-report --json-report-omit keywords streams
+pytest --hw-test-report --hw-test-report-omit keywords streams
 ```
 
 If you don't like to have the report saved, you can specify `none` as the target file name:
 
 ```bash
-$ pytest --json-report --json-report-file none
+pytest --hw-test-report --hw-test-report-file none
 ```
 
-## Advanced usage
+### Fixtures
+
+#### json_dut
+
+To record information about the device under test in the report you can use the `json_dut` [test fixture](https://docs.pytest.org/en/stable/fixture.html). This also works if your DUT is, itself, a fixture:
+
+```python
+@pytest.fixture(name="dut")
+def dut_fixture(json_dut):
+    json_dut['serial no'] = 1234567
+    json_dut['version'] = 1.0.0
+    dut = setup_dut()
+    yield dut
+    dut.teardown()
+```
+
+#### json_equipment
 
-### Metadata
+To record information about any test equipment you may use in the report you can use the `json_equipment` [test fixture](https://docs.pytest.org/en/stable/fixture.html):
+
+```python
+def equipment1(json_equipment):
+    json_equipment['equipment1'] = {'manufacturer': 'Test Inc.', 'Model': 'Testomatic 300'}
+```
+
+#### json_metadata
 
 The easiest way to add your own metadata to a test item is by using the `json_metadata` [test fixture](https://docs.pytest.org/en/stable/fixture.html):
 
 ```python
 def test_something(json_metadata):
     json_metadata['foo'] = {"some": "thing"}
     json_metadata['bar'] = 123
 ```
 
-Or use the `pytest_json_runtest_metadata` [hook](https://docs.pytest.org/en/stable/reference.html#hooks) (in your `conftest.py`) to add metadata based on the current test run. The dict returned will automatically be merged with any existing metadata. E.g., this adds the start and stop time of each test's `call` stage:
+## Advanced usage
+
+### Hooks
+
+If you're using a `pytest_json_*` hook although the plugin is not installed or not active (not using `--json-report`), pytest doesn't recognize it and may fail with an internal error like this:
+
+```bash
+INTERNALERROR> pluggy.manager.PluginValidationError: unknown hook 'pytest_json_runtest_metadata' in plugin <module 'conftest' from 'conftest.py'>
+```
+
+You can avoid this by declaring the hook implementation optional:
 
 ```python
+import pytest
+@pytest.hookimpl(optionalhook=True)
 def pytest_json_runtest_metadata(item, call):
-    if call.when != 'call':
+    ...
+```
+
+#### DUT
+
+Or use the `pytest_json_runtest_dut` [hook](https://docs.pytest.org/en/stable/reference.html#hooks) (in your `conftest.py`) to add metadata based on the current test run. The dict returned will automatically be merged with any existing metadata. E.g., this adds the start and stop time of each test's `setup` stage:
+
+```python
+def pytest_json_runtest_dut(item, call):
+    if call.when != 'setup':
         return {}
     return {'start': call.start, 'stop': call.stop}
 ```
 
-Also, you could add metadata using [pytest-metadata's `--metadata` switch](https://github.com/pytest-dev/pytest-metadata#additional-metadata) which will add metadata to the report's `environment` section, but not to a specific test item. You need to make sure all your metadata is JSON-serializable.
+#### Equipment
 
-### A note on hooks
+Or use the `pytest_json_runtest_equipment` [hook](https://docs.pytest.org/en/stable/reference.html#hooks) (in your `conftest.py`) to add metadata based on the current test run. The dict returned will automatically be merged with any existing metadata. E.g., this adds the start and stop time of each test's `setup` stage:
 
-If you're using a `pytest_json_*` hook although the plugin is not installed or not active (not using `--json-report`), pytest doesn't recognize it and may fail with an internal error like this:
-```
-INTERNALERROR> pluggy.manager.PluginValidationError: unknown hook 'pytest_json_runtest_metadata' in plugin <module 'conftest' from 'conftest.py'>
+```python
+def pytest_json_runtest_equipment(item, call):
+    if call.when != 'setup':
+        return {}
+    return {'start': call.start, 'stop': call.stop}
 ```
-You can avoid this by declaring the hook implementation optional:
+
+#### Metadata
+
+Or use the `pytest_json_runtest_metadata` [hook](https://docs.pytest.org/en/stable/reference.html#hooks) (in your `conftest.py`) to add metadata based on the current test run. The dict returned will automatically be merged with any existing metadata. E.g., this adds the start and stop time of each test's `call` stage:
 
 ```python
-import pytest
-@pytest.hookimpl(optionalhook=True)
 def pytest_json_runtest_metadata(item, call):
-    ...
+    if call.when != 'call':
+        return {}
+    return {'start': call.start, 'stop': call.stop}
 ```
 
-### Modifying the report
+Also, you could add metadata using [pytest-metadata's `--metadata` switch](https://github.com/pytest-dev/pytest-metadata#additional-metadata) which will add metadata to the report's `environment` section, but not to a specific test item. You need to make sure all your metadata is JSON-serializable.
+
+#### Modifying the report
 
 You can modify the entire report before it's saved by using the `pytest_json_modifyreport` hook.
 
 Just implement the hook in your `conftest.py`, e.g.:
 
 ```python
 def pytest_json_modifyreport(json_report):
@@ -173,91 +231,90 @@
 You can use the plugin when invoking `pytest.main()` directly from code:
 
 ```python
 import pytest
 from pytest_htr.plugin import JSONReport
 
 plugin = JSONReport()
-pytest.main(['--json-report-file=none', 'test_foo.py'], plugins=[plugin])
+pytest.main(['--hw-test-report-file=none', 'test_foo.py'], plugins=[plugin])
 ```
 
 You can then access the `report` object:
 
 ```python
 print(plugin.report)
 ```
 
 And save the report manually:
 
 ```python
 plugin.save_report('/tmp/my_report.json')
 ```
 
-
 ## Format
 
-The JSON report contains metadata of the session, a summary, collectors, tests and warnings. You can find a sample report in [`sample_report.json`](sample_report.json).
+The JSON report contains metadata of the session, a summary, tests and warnings. You can find a sample report in [`sample_report.json`](sample_report.json).
 
 | Key | Description |
 | --- | --- |
 | `created` | Report creation date. (Unix time) |
 | `duration` | Session duration in seconds. |
 | `exitcode` | Process exit code as listed [in the pytest docs](https://docs.pytest.org/en/latest/usage.html#possible-exit-codes). The exit code is a quick way to tell if any tests failed, an internal error occurred, etc. |
 | `root` | Absolute root path from which the session was started. |
 | `environment` | [Environment](#environment) entry. |
 | `summary` | [Summary](#summary) entry. |
-| `tests` | [Tests](#tests) entry. (absent if `--json-report-summary`)  |
-| `warnings` | [Warnings](#warnings) entry. (absent if `--json-report-summary` or if no warnings)  |
+| `tests` | [Tests](#tests) entry. (absent if `--hw-test-report-summary`)  |
+| `warnings` | [Warnings](#warnings) entry. (absent if `--hw-test-report-summary` or if no warnings)  |
 
-#### Example
+### Format Example
 
 ```python
 {
     "created": 1518371686.7981803,
     "duration": 0.1235666275024414,
     "exitcode": 1,
     "root": "/path/to/tests",
     "environment": ENVIRONMENT,
     "summary": SUMMARY,
     "tests": TESTS,
     "warnings": WARNINGS,
 }
 ```
 
-### Summary
+## Summary
 
 Number of outcomes per category and the total number of test items.
 
 | Key | Description |
 | --- | --- |
 |  `collected` | Total number of tests collected. |
 |  `total` | Total number of tests run. |
 |  `deselected` | Total number of tests deselected. (absent if number is 0) |
 | `<outcome>` | Number of tests with that outcome. (absent if number is 0) |
 
-#### Example
+### Summary Example
 
 ```python
 {
     "collected": 10,
     "passed": 2,
     "failed": 3,
     "xfailed": 1,
     "xpassed": 1,
     "error": 2,
     "skipped": 1,
     "total": 10
 }
 ```
 
-### Environment
+## Environment
 
 The environment section is provided by [pytest-metadata](https://github.com/pytest-dev/pytest-metadata). All metadata given by that plugin will be added here, so you need to make sure it is JSON-serializable.
 
-#### Example
+### Environment Example
 
 ```python
 {
     "Python": "3.6.4",
     "Platform": "Linux-4.56.78-9-ARCH-x86_64-with-arch",
     "Packages": {
         "pytest": "3.4.0",
@@ -271,28 +328,28 @@
         "forked": "0.2",
         "cov": "2.5.1"
     },
     "foo": "bar", # Custom metadata entry passed via pytest-metadata
 }
 ```
 
-### Tests
+## Tests
 
 A list of test nodes. Each completed test stage produces a stage object (`setup`, `call`, `teardown`) with its own `outcome`.
 
 | Key | Description |
 | --- | --- |
 | `nodeid` | ID of the test node. |
 | `outcome` | Outcome of the test run. |
 | `DUT` | DUT item. (absent if not present) |
 | `equipment` | equipment item. (absent if not present) |
 | `{setup, call, teardown}` | [Test stage](#test-stage) entry. To find the error in a failed test you need to check all stages. (absent if stage didn't run) |
 | `metadata` | [Metadata](#metadata) item. (absent if no metadata) |
 
-#### Example
+### Tests Example
 
 ```python
 [
     {
         "nodeid": "test_foo.py::test_fail",
         "outcome": "failed",
         "DUT": {
@@ -313,31 +370,30 @@
             "foo": "bar",
         }
     },
     ...
 ]
 ```
 
-
-### Test stage
+## Test stage
 
 A test stage item.
 
 | Key | Description |
 | --- | --- |
 | `duration` | Duration of the test stage in seconds. |
 | `outcome` | Outcome of the test stage. (can be different from the overall test outcome) |
 | `crash` | Crash entry. (absent if no error occurred) |
 | `traceback` | List of traceback entries. (absent if no error occurred; affected by `--tb` option) |
 | `stdout` | Standard output. (absent if none available) |
 | `stderr` | Standard error. (absent if none available) |
 | `log` | [Log](#log) entry. (absent if none available) |
 | `longrepr` | Representation of the error. (absent if no error occurred; format affected by `--tb` option) |
 
-#### Example
+### Test stage Example
 
 ```python
 {
     "duration": 0.00018835067749023438,
     "outcome": "failed",
     "crash": {
         "path": "/path/to/tests/test_foo.py",
@@ -369,21 +425,21 @@
     "stdout": "foo\nbar\n",
     "stderr": "baz\n",
     "log": LOG,
     "longrepr": "def test_fail_nested():\n ..."
 }
 ```
 
-### Log
+## Log
 
 A list of log records. The fields of a log record are the [`logging.LogRecord` attributes](https://docs.python.org/3/library/logging.html#logrecord-attributes), with the exception that the fields `exc_info` and `args` are always empty and `msg` contains the formatted log message.
 
 You can apply [`logging.makeLogRecord()`](https://docs.python.org/3/library/logging.html#logging.makeLogRecord)  on a log record to convert it back to a `logging.LogRecord` object.
 
-#### Example
+### Log Example
 
 ```python
 [
     {
         "name": "root",
         "msg": "This is a warning.",
         "args": null,
@@ -405,40 +461,39 @@
         "processName": "MainProcess",
         "process": 31481
     },
     ...
 ]
 ```
 
-
-### Warnings
+## Warnings
 
 A list of warnings that occurred during the session. (See the [pytest docs on warnings](https://docs.pytest.org/en/latest/warnings.html).)
 
 | Key | Description |
 | --- | --- |
 | `filename` | File name. |
 | `lineno` | Line number. |
 | `message` | Warning message. |
 | `when` | When the warning was captured. (`"config"`, `"collect"` or `"runtest"` as listed [here](https://docs.pytest.org/en/latest/reference.html#_pytest.hookspec.pytest_warning_captured)) |
 
-#### Example
+### Warnings Example
 
 ```python
 [
     {
         "code": "C1",
         "path": "/path/to/tests/test_foo.py",
         "nodeid": "test_foo.py::TestFoo",
         "message": "cannot collect test class 'TestFoo' because it has a __init__ constructor"
     }
 ]
 ```
 
 ## Related tools
 
--[pytest-json-report](https://github.com/numirias/pytest-json-report) Heavily inspired by this plugin. It is more suited for pure software testing but i have borrow large ammounts of code from there.
+* [pytest-json-report](https://github.com/numirias/pytest-json-report) Heavily inspired by this plugin. It is more suited for pure software testing but i have borrow large ammounts of code from there.
 
-- [pytest-json](https://github.com/mattcl/pytest-json) has some great features but appears to be unmaintained. I borrowed some ideas and test cases from there.
+* [pytest-json](https://github.com/mattcl/pytest-json) has some great features but appears to be unmaintained. I borrowed some ideas and test cases from there.
 
-- [tox has a switch](http://tox.readthedocs.io/en/latest/example/result.html) to create a JSON report including a test result summary. However, it just provides the overall outcome without any per-test details.
+* [tox has a switch](http://tox.readthedocs.io/en/latest/example/result.html) to create a JSON report including a test result summary. However, it just provides the overall outcome without any per-test details.
```

