# Comparing `tmp/tf_policy_validator-0.0.5.tar.gz` & `tmp/tf_policy_validator-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tf_policy_validator-0.0.5.tar", max compression
+gzip compressed data, was "tf_policy_validator-0.0.6.tar", max compression
```

## Comparing `tf_policy_validator-0.0.5.tar` & `tf_policy_validator-0.0.6.tar`

### file list

```diff
@@ -1,51 +1,51 @@
--rw-r--r--   0        0        0      927 2024-03-19 18:27:02.699105 tf_policy_validator-0.0.5/LICENSE
--rw-r--r--   0        0        0    12410 2024-03-19 18:27:02.699410 tf_policy_validator-0.0.5/README.md
--rw-r--r--   0        0        0        0 2024-03-19 18:27:02.699540 tf_policy_validator-0.0.5/iam_check/__init__.py
--rw-r--r--   0        0        0      207 2024-03-19 18:27:02.699737 tf_policy_validator-0.0.5/iam_check/application_error.py
--rw-r--r--   0        0        0     3257 2024-03-19 18:27:02.699881 tf_policy_validator-0.0.5/iam_check/argument_actions.py
--rw-r--r--   0        0        0      971 2024-03-19 18:27:02.700006 tf_policy_validator-0.0.5/iam_check/client.py
--rw-r--r--   0        0        0     5023 2024-03-19 18:27:02.700389 tf_policy_validator-0.0.5/iam_check/config/default.yaml
--rw-r--r--   0        0        0     1764 2024-03-19 18:27:02.700143 tf_policy_validator-0.0.5/iam_check/config.py
--rw-r--r--   0        0        0     7165 2024-03-19 18:27:02.700603 tf_policy_validator-0.0.5/iam_check/doc/example_report_1.md
--rw-r--r--   0        0        0     3960 2024-03-19 18:27:02.700717 tf_policy_validator-0.0.5/iam_check/doc/example_report_2.md
--rw-r--r--   0        0        0     2544 2024-03-19 18:27:02.700831 tf_policy_validator-0.0.5/iam_check/doc/example_report_3.md
--rw-r--r--   0        0        0    11266 2024-03-19 18:27:02.701064 tf_policy_validator-0.0.5/iam_check/iam_check.py
--rw-r--r--   0        0        0     1106 2024-03-19 18:27:02.701260 tf_policy_validator-0.0.5/iam_check/lib/__init__.py
--rw-r--r--   0        0        0      258 2024-03-19 18:27:02.701393 tf_policy_validator-0.0.5/iam_check/lib/account_config.py
--rw-r--r--   0        0        0     2850 2024-03-19 18:27:02.701519 tf_policy_validator-0.0.5/iam_check/lib/findings.py
--rw-r--r--   0        0        0      350 2024-03-19 18:27:02.701628 tf_policy_validator-0.0.5/iam_check/lib/iamCheck.py
--rw-r--r--   0        0        0    10434 2024-03-19 18:27:02.701806 tf_policy_validator-0.0.5/iam_check/lib/iamPolicy.py
--rw-r--r--   0        0        0    10094 2024-03-19 18:27:02.701993 tf_policy_validator-0.0.5/iam_check/lib/iamcheck_AccessAnalyzer.py
--rw-r--r--   0        0        0     5198 2024-03-19 18:27:02.702125 tf_policy_validator-0.0.5/iam_check/lib/reporter.py
--rw-r--r--   0        0        0    20014 2024-03-19 18:27:02.702270 tf_policy_validator-0.0.5/iam_check/lib/tfPlan.py
--rw-r--r--   0        0        0     1666 2024-03-19 18:27:02.702453 tf_policy_validator-0.0.5/iam_check/parameters.py
--rw-r--r--   0        0        0       38 2024-03-19 18:27:02.702565 tf_policy_validator-0.0.5/iam_check/pytest.ini
--rw-r--r--   0        0        0        0 2024-03-19 18:27:02.702653 tf_policy_validator-0.0.5/iam_check/test/__init__.py
--rw-r--r--   0        0        0     1458 2024-03-19 18:27:02.702767 tf_policy_validator-0.0.5/iam_check/test/aws_iam_policy.tf
--rw-r--r--   0        0        0       61 2024-03-19 18:27:02.702923 tf_policy_validator-0.0.5/iam_check/test/iam_policy/findings.json
--rw-r--r--   0        0        0     1458 2024-03-19 18:27:02.703048 tf_policy_validator-0.0.5/iam_check/test/iam_policy/test.tf
--rw-r--r--   0        0        0     8277 2024-03-19 18:27:02.703201 tf_policy_validator-0.0.5/iam_check/test/iam_policy/test_plan.json
--rw-r--r--   0        0        0     4437 2024-03-19 18:27:02.703409 tf_policy_validator-0.0.5/iam_check/test/identity_policies/identity_findings.json
--rw-r--r--   0        0        0      205 2024-03-19 18:27:02.703521 tf_policy_validator-0.0.5/iam_check/test/identity_policies/identity_reference_policy.json
--rw-r--r--   0        0        0     3038 2024-03-19 18:27:02.703621 tf_policy_validator-0.0.5/iam_check/test/identity_policies/test.tf
--rw-r--r--   0        0        0    15609 2024-03-19 18:27:02.703781 tf_policy_validator-0.0.5/iam_check/test/identity_policies/test_plan.json
--rw-r--r--   0        0        0      781 2024-03-19 18:27:02.703939 tf_policy_validator-0.0.5/iam_check/test/multiple_policies/identity_findings.json
--rw-r--r--   0        0        0      299 2024-03-19 18:27:02.704017 tf_policy_validator-0.0.5/iam_check/test/multiple_policies/identity_reference_policy.json
--rw-r--r--   0        0        0      816 2024-03-19 18:27:02.704110 tf_policy_validator-0.0.5/iam_check/test/multiple_policies/resource_findings.json
--rw-r--r--   0        0        0      197 2024-03-19 18:27:02.704200 tf_policy_validator-0.0.5/iam_check/test/multiple_policies/resource_reference_policy.json
--rw-r--r--   0        0        0     1240 2024-03-19 18:27:02.704292 tf_policy_validator-0.0.5/iam_check/test/multiple_policies/test.tf
--rw-r--r--   0        0        0     8765 2024-03-19 18:27:02.704418 tf_policy_validator-0.0.5/iam_check/test/multiple_policies/test_plan.json
--rw-r--r--   0        0        0      111 2024-03-19 18:27:02.704503 tf_policy_validator-0.0.5/iam_check/test/provider.tf
--rw-r--r--   0        0        0      798 2024-03-19 18:27:02.704644 tf_policy_validator-0.0.5/iam_check/test/role_inline_assume_policy/identity_findings.json
--rw-r--r--   0        0        0      237 2024-03-19 18:27:02.704744 tf_policy_validator-0.0.5/iam_check/test/role_inline_assume_policy/identity_reference_policy.json
--rw-r--r--   0        0        0      783 2024-03-19 18:27:02.704822 tf_policy_validator-0.0.5/iam_check/test/role_inline_assume_policy/resource_findings.json
--rw-r--r--   0        0        0      178 2024-03-19 18:27:02.704892 tf_policy_validator-0.0.5/iam_check/test/role_inline_assume_policy/resource_reference_policy.json
--rw-r--r--   0        0        0      724 2024-03-19 18:27:02.704977 tf_policy_validator-0.0.5/iam_check/test/role_inline_assume_policy/test.tf
--rw-r--r--   0        0        0     2520 2024-03-19 18:27:02.705049 tf_policy_validator-0.0.5/iam_check/test/role_inline_assume_policy/test_plan.json
--rw-r--r--   0        0        0     2299 2024-03-19 18:27:02.705121 tf_policy_validator-0.0.5/iam_check/test/test_accessAnalyzer.py
--rw-r--r--   0        0        0      244 2024-03-19 18:27:02.705188 tf_policy_validator-0.0.5/iam_check/test/test_policy.json
--rw-r--r--   0        0        0     8277 2024-03-19 18:27:02.705299 tf_policy_validator-0.0.5/iam_check/test/test_policy_accessanalyzer.json
--rw-r--r--   0        0        0     1061 2024-03-19 18:27:02.705372 tf_policy_validator-0.0.5/iam_check/test/test_tf_plan.py
--rw-r--r--   0        0        0      810 2024-03-19 18:27:02.705485 tf_policy_validator-0.0.5/iam_check/tools/regex_patterns.py
--rw-r--r--   0        0        0     1121 2024-03-25 18:15:50.703476 tf_policy_validator-0.0.5/pyproject.toml
--rw-r--r--   0        0        0    13358 1970-01-01 00:00:00.000000 tf_policy_validator-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0      927 2024-04-01 18:17:55.606823 tf_policy_validator-0.0.6/LICENSE
+-rw-r--r--   0        0        0    12410 2024-04-01 18:17:55.606823 tf_policy_validator-0.0.6/README.md
+-rw-r--r--   0        0        0        0 2024-04-01 18:17:55.606823 tf_policy_validator-0.0.6/iam_check/__init__.py
+-rw-r--r--   0        0        0      207 2024-04-01 18:17:55.606823 tf_policy_validator-0.0.6/iam_check/application_error.py
+-rw-r--r--   0        0        0     3257 2024-04-01 18:17:55.606823 tf_policy_validator-0.0.6/iam_check/argument_actions.py
+-rw-r--r--   0        0        0      971 2024-04-01 18:17:55.606823 tf_policy_validator-0.0.6/iam_check/client.py
+-rw-r--r--   0        0        0     5023 2024-04-01 18:17:55.606823 tf_policy_validator-0.0.6/iam_check/config/default.yaml
+-rw-r--r--   0        0        0     1764 2024-04-01 18:17:55.606823 tf_policy_validator-0.0.6/iam_check/config.py
+-rw-r--r--   0        0        0     7165 2024-04-01 18:17:55.606823 tf_policy_validator-0.0.6/iam_check/doc/example_report_1.md
+-rw-r--r--   0        0        0     3960 2024-04-01 18:17:55.606823 tf_policy_validator-0.0.6/iam_check/doc/example_report_2.md
+-rw-r--r--   0        0        0     2544 2024-04-01 18:17:55.606823 tf_policy_validator-0.0.6/iam_check/doc/example_report_3.md
+-rw-r--r--   0        0        0    11266 2024-04-01 18:17:55.606823 tf_policy_validator-0.0.6/iam_check/iam_check.py
+-rw-r--r--   0        0        0     1106 2024-04-01 18:17:55.606823 tf_policy_validator-0.0.6/iam_check/lib/__init__.py
+-rw-r--r--   0        0        0      258 2024-04-01 18:17:55.606823 tf_policy_validator-0.0.6/iam_check/lib/account_config.py
+-rw-r--r--   0        0        0     2850 2024-04-01 18:17:55.606823 tf_policy_validator-0.0.6/iam_check/lib/findings.py
+-rw-r--r--   0        0        0      350 2024-04-01 18:17:55.606823 tf_policy_validator-0.0.6/iam_check/lib/iamCheck.py
+-rw-r--r--   0        0        0    10434 2024-04-01 18:17:55.606823 tf_policy_validator-0.0.6/iam_check/lib/iamPolicy.py
+-rw-r--r--   0        0        0    10094 2024-04-01 18:17:55.606823 tf_policy_validator-0.0.6/iam_check/lib/iamcheck_AccessAnalyzer.py
+-rw-r--r--   0        0        0     5198 2024-04-01 18:17:55.606823 tf_policy_validator-0.0.6/iam_check/lib/reporter.py
+-rw-r--r--   0        0        0    20014 2024-04-01 18:17:55.606823 tf_policy_validator-0.0.6/iam_check/lib/tfPlan.py
+-rw-r--r--   0        0        0     1666 2024-04-01 18:17:55.606823 tf_policy_validator-0.0.6/iam_check/parameters.py
+-rw-r--r--   0        0        0       38 2024-04-01 18:17:55.606823 tf_policy_validator-0.0.6/iam_check/pytest.ini
+-rw-r--r--   0        0        0        0 2024-04-01 18:17:55.606823 tf_policy_validator-0.0.6/iam_check/test/__init__.py
+-rw-r--r--   0        0        0     1458 2024-04-01 18:17:55.606823 tf_policy_validator-0.0.6/iam_check/test/aws_iam_policy.tf
+-rw-r--r--   0        0        0       61 2024-04-01 18:17:55.606823 tf_policy_validator-0.0.6/iam_check/test/iam_policy/findings.json
+-rw-r--r--   0        0        0     1458 2024-04-01 18:17:55.606823 tf_policy_validator-0.0.6/iam_check/test/iam_policy/test.tf
+-rw-r--r--   0        0        0     8277 2024-04-01 18:17:55.610823 tf_policy_validator-0.0.6/iam_check/test/iam_policy/test_plan.json
+-rw-r--r--   0        0        0     4437 2024-04-01 18:17:55.610823 tf_policy_validator-0.0.6/iam_check/test/identity_policies/identity_findings.json
+-rw-r--r--   0        0        0      205 2024-04-01 18:17:55.610823 tf_policy_validator-0.0.6/iam_check/test/identity_policies/identity_reference_policy.json
+-rw-r--r--   0        0        0     3038 2024-04-01 18:17:55.610823 tf_policy_validator-0.0.6/iam_check/test/identity_policies/test.tf
+-rw-r--r--   0        0        0    15609 2024-04-01 18:17:55.610823 tf_policy_validator-0.0.6/iam_check/test/identity_policies/test_plan.json
+-rw-r--r--   0        0        0      781 2024-04-01 18:17:55.610823 tf_policy_validator-0.0.6/iam_check/test/multiple_policies/identity_findings.json
+-rw-r--r--   0        0        0      299 2024-04-01 18:17:55.610823 tf_policy_validator-0.0.6/iam_check/test/multiple_policies/identity_reference_policy.json
+-rw-r--r--   0        0        0      816 2024-04-01 18:17:55.610823 tf_policy_validator-0.0.6/iam_check/test/multiple_policies/resource_findings.json
+-rw-r--r--   0        0        0      197 2024-04-01 18:17:55.610823 tf_policy_validator-0.0.6/iam_check/test/multiple_policies/resource_reference_policy.json
+-rw-r--r--   0        0        0     1240 2024-04-01 18:17:55.610823 tf_policy_validator-0.0.6/iam_check/test/multiple_policies/test.tf
+-rw-r--r--   0        0        0     8765 2024-04-01 18:17:55.610823 tf_policy_validator-0.0.6/iam_check/test/multiple_policies/test_plan.json
+-rw-r--r--   0        0        0      111 2024-04-01 18:17:55.610823 tf_policy_validator-0.0.6/iam_check/test/provider.tf
+-rw-r--r--   0        0        0      798 2024-04-01 18:17:55.610823 tf_policy_validator-0.0.6/iam_check/test/role_inline_assume_policy/identity_findings.json
+-rw-r--r--   0        0        0      237 2024-04-01 18:17:55.610823 tf_policy_validator-0.0.6/iam_check/test/role_inline_assume_policy/identity_reference_policy.json
+-rw-r--r--   0        0        0      783 2024-04-01 18:17:55.610823 tf_policy_validator-0.0.6/iam_check/test/role_inline_assume_policy/resource_findings.json
+-rw-r--r--   0        0        0      178 2024-04-01 18:17:55.610823 tf_policy_validator-0.0.6/iam_check/test/role_inline_assume_policy/resource_reference_policy.json
+-rw-r--r--   0        0        0      724 2024-04-01 18:17:55.610823 tf_policy_validator-0.0.6/iam_check/test/role_inline_assume_policy/test.tf
+-rw-r--r--   0        0        0     2520 2024-04-01 18:17:55.610823 tf_policy_validator-0.0.6/iam_check/test/role_inline_assume_policy/test_plan.json
+-rw-r--r--   0        0        0     2299 2024-04-01 18:17:55.610823 tf_policy_validator-0.0.6/iam_check/test/test_accessAnalyzer.py
+-rw-r--r--   0        0        0      244 2024-04-01 18:17:55.610823 tf_policy_validator-0.0.6/iam_check/test/test_policy.json
+-rw-r--r--   0        0        0     8277 2024-04-01 18:17:55.610823 tf_policy_validator-0.0.6/iam_check/test/test_policy_accessanalyzer.json
+-rw-r--r--   0        0        0     1061 2024-04-01 18:17:55.610823 tf_policy_validator-0.0.6/iam_check/test/test_tf_plan.py
+-rw-r--r--   0        0        0      810 2024-04-01 18:17:55.610823 tf_policy_validator-0.0.6/iam_check/tools/regex_patterns.py
+-rw-r--r--   0        0        0     1121 2024-04-01 18:17:55.610823 tf_policy_validator-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0    13358 1970-01-01 00:00:00.000000 tf_policy_validator-0.0.6/PKG-INFO
```

### Comparing `tf_policy_validator-0.0.5/LICENSE` & `tf_policy_validator-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `tf_policy_validator-0.0.5/README.md` & `tf_policy_validator-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `tf_policy_validator-0.0.5/iam_check/argument_actions.py` & `tf_policy_validator-0.0.6/iam_check/argument_actions.py`

 * *Files identical despite different names*

### Comparing `tf_policy_validator-0.0.5/iam_check/client.py` & `tf_policy_validator-0.0.6/iam_check/client.py`

 * *Files identical despite different names*

### Comparing `tf_policy_validator-0.0.5/iam_check/config/default.yaml` & `tf_policy_validator-0.0.6/iam_check/config/default.yaml`

 * *Files identical despite different names*

### Comparing `tf_policy_validator-0.0.5/iam_check/config.py` & `tf_policy_validator-0.0.6/iam_check/config.py`

 * *Files identical despite different names*

### Comparing `tf_policy_validator-0.0.5/iam_check/doc/example_report_1.md` & `tf_policy_validator-0.0.6/iam_check/doc/example_report_1.md`

 * *Files identical despite different names*

### Comparing `tf_policy_validator-0.0.5/iam_check/doc/example_report_2.md` & `tf_policy_validator-0.0.6/iam_check/doc/example_report_2.md`

 * *Files identical despite different names*

### Comparing `tf_policy_validator-0.0.5/iam_check/doc/example_report_3.md` & `tf_policy_validator-0.0.6/iam_check/doc/example_report_3.md`

 * *Files identical despite different names*

### Comparing `tf_policy_validator-0.0.5/iam_check/iam_check.py` & `tf_policy_validator-0.0.6/iam_check/iam_check.py`

 * *Files identical despite different names*

### Comparing `tf_policy_validator-0.0.5/iam_check/lib/__init__.py` & `tf_policy_validator-0.0.6/iam_check/lib/__init__.py`

 * *Files identical despite different names*

### Comparing `tf_policy_validator-0.0.5/iam_check/lib/findings.py` & `tf_policy_validator-0.0.6/iam_check/lib/findings.py`

 * *Files identical despite different names*

### Comparing `tf_policy_validator-0.0.5/iam_check/lib/iamPolicy.py` & `tf_policy_validator-0.0.6/iam_check/lib/iamPolicy.py`

 * *Files identical despite different names*

### Comparing `tf_policy_validator-0.0.5/iam_check/lib/iamcheck_AccessAnalyzer.py` & `tf_policy_validator-0.0.6/iam_check/lib/iamcheck_AccessAnalyzer.py`

 * *Files identical despite different names*

### Comparing `tf_policy_validator-0.0.5/iam_check/lib/reporter.py` & `tf_policy_validator-0.0.6/iam_check/lib/reporter.py`

 * *Files identical despite different names*

### Comparing `tf_policy_validator-0.0.5/iam_check/lib/tfPlan.py` & `tf_policy_validator-0.0.6/iam_check/lib/tfPlan.py`

 * *Files identical despite different names*

### Comparing `tf_policy_validator-0.0.5/iam_check/parameters.py` & `tf_policy_validator-0.0.6/iam_check/parameters.py`

 * *Files identical despite different names*

### Comparing `tf_policy_validator-0.0.5/iam_check/test/aws_iam_policy.tf` & `tf_policy_validator-0.0.6/iam_check/test/aws_iam_policy.tf`

 * *Files identical despite different names*

### Comparing `tf_policy_validator-0.0.5/iam_check/test/iam_policy/test.tf` & `tf_policy_validator-0.0.6/iam_check/test/iam_policy/test.tf`

 * *Files identical despite different names*

### Comparing `tf_policy_validator-0.0.5/iam_check/test/iam_policy/test_plan.json` & `tf_policy_validator-0.0.6/iam_check/test/iam_policy/test_plan.json`

 * *Files identical despite different names*

### Comparing `tf_policy_validator-0.0.5/iam_check/test/identity_policies/identity_findings.json` & `tf_policy_validator-0.0.6/iam_check/test/identity_policies/identity_findings.json`

 * *Files identical despite different names*

### Comparing `tf_policy_validator-0.0.5/iam_check/test/identity_policies/test.tf` & `tf_policy_validator-0.0.6/iam_check/test/identity_policies/test.tf`

 * *Files identical despite different names*

### Comparing `tf_policy_validator-0.0.5/iam_check/test/identity_policies/test_plan.json` & `tf_policy_validator-0.0.6/iam_check/test/identity_policies/test_plan.json`

 * *Files identical despite different names*

### Comparing `tf_policy_validator-0.0.5/iam_check/test/multiple_policies/identity_findings.json` & `tf_policy_validator-0.0.6/iam_check/test/multiple_policies/identity_findings.json`

 * *Files identical despite different names*

### Comparing `tf_policy_validator-0.0.5/iam_check/test/multiple_policies/resource_findings.json` & `tf_policy_validator-0.0.6/iam_check/test/multiple_policies/resource_findings.json`

 * *Files identical despite different names*

### Comparing `tf_policy_validator-0.0.5/iam_check/test/multiple_policies/test.tf` & `tf_policy_validator-0.0.6/iam_check/test/multiple_policies/test.tf`

 * *Files identical despite different names*

### Comparing `tf_policy_validator-0.0.5/iam_check/test/multiple_policies/test_plan.json` & `tf_policy_validator-0.0.6/iam_check/test/multiple_policies/test_plan.json`

 * *Files identical despite different names*

### Comparing `tf_policy_validator-0.0.5/iam_check/test/role_inline_assume_policy/identity_findings.json` & `tf_policy_validator-0.0.6/iam_check/test/role_inline_assume_policy/identity_findings.json`

 * *Files identical despite different names*

### Comparing `tf_policy_validator-0.0.5/iam_check/test/role_inline_assume_policy/resource_findings.json` & `tf_policy_validator-0.0.6/iam_check/test/role_inline_assume_policy/resource_findings.json`

 * *Files identical despite different names*

### Comparing `tf_policy_validator-0.0.5/iam_check/test/role_inline_assume_policy/test.tf` & `tf_policy_validator-0.0.6/iam_check/test/role_inline_assume_policy/test.tf`

 * *Files identical despite different names*

### Comparing `tf_policy_validator-0.0.5/iam_check/test/role_inline_assume_policy/test_plan.json` & `tf_policy_validator-0.0.6/iam_check/test/role_inline_assume_policy/test_plan.json`

 * *Files identical despite different names*

### Comparing `tf_policy_validator-0.0.5/iam_check/test/test_accessAnalyzer.py` & `tf_policy_validator-0.0.6/iam_check/test/test_accessAnalyzer.py`

 * *Files identical despite different names*

### Comparing `tf_policy_validator-0.0.5/iam_check/test/test_policy_accessanalyzer.json` & `tf_policy_validator-0.0.6/iam_check/test/test_policy_accessanalyzer.json`

 * *Files identical despite different names*

### Comparing `tf_policy_validator-0.0.5/iam_check/test/test_tf_plan.py` & `tf_policy_validator-0.0.6/iam_check/test/test_tf_plan.py`

 * *Files identical despite different names*

### Comparing `tf_policy_validator-0.0.5/iam_check/tools/regex_patterns.py` & `tf_policy_validator-0.0.6/iam_check/tools/regex_patterns.py`

 * *Files identical despite different names*

### Comparing `tf_policy_validator-0.0.5/pyproject.toml` & `tf_policy_validator-0.0.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tf-policy-validator"
-version = "0.0.5"
+version = "0.0.6"
 description = "A command line tool that validates AWS IAM Policies in a Terraform template against AWS IAM best practices"
 authors = ["Policy Validator Maintainers <terraform-policy-validator@amazon.com>"]
 readme = "README.md"
 packages = [{include = "iam_check"}]
 license = "MIT-0"
 keywords = ["amazon", "aws", "aws-samples", "eks", "kubernetes", "upgrade", "iam_check"]
 classifiers = [
```

### Comparing `tf_policy_validator-0.0.5/PKG-INFO` & `tf_policy_validator-0.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tf-policy-validator
-Version: 0.0.5
+Version: 0.0.6
 Summary: A command line tool that validates AWS IAM Policies in a Terraform template against AWS IAM best practices
 License: MIT-0
 Keywords: amazon,aws,aws-samples,eks,kubernetes,upgrade,iam_check
 Author: Policy Validator Maintainers
 Author-email: terraform-policy-validator@amazon.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved
```

