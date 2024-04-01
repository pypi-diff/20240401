# Comparing `tmp/stigg_api_client-1.98.0.tar.gz` & `tmp/stigg_api_client-1.98.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stigg_api_client-1.98.0.tar", max compression
+gzip compressed data, was "stigg_api_client-1.98.1.tar", max compression
```

## Comparing `stigg_api_client-1.98.0.tar` & `stigg_api_client-1.98.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     5127 2024-03-31 12:49:33.702471 stigg_api_client-1.98.0/LICENSE
--rw-r--r--   0        0        0     2479 2024-03-31 12:49:33.702471 stigg_api_client-1.98.0/README.md
--rw-r--r--   0        0        0      509 2024-03-31 12:50:09.546068 stigg_api_client-1.98.0/pyproject.toml
--rw-r--r--   0        0        0       44 2024-03-31 12:49:33.702471 stigg_api_client-1.98.0/stigg/__init__.py
--rw-r--r--   0        0        0     3721 2024-03-31 12:49:33.702471 stigg_api_client-1.98.0/stigg/client.py
--rw-r--r--   0        0        0        0 2024-03-31 12:50:07.858088 stigg_api_client-1.98.0/stigg/generated/__init__.py
--rw-r--r--   0        0        0    67627 2024-03-31 12:50:08.222084 stigg_api_client-1.98.0/stigg/generated/operations.py
--rw-r--r--   0        0        0   568537 2024-03-31 12:50:08.082085 stigg_api_client-1.98.0/stigg/generated/schema.py
--rw-r--r--   0        0        0     3197 1970-01-01 00:00:00.000000 stigg_api_client-1.98.0/PKG-INFO
+-rw-r--r--   0        0        0     5127 2024-03-31 14:16:59.295047 stigg_api_client-1.98.1/LICENSE
+-rw-r--r--   0        0        0     2479 2024-03-31 14:16:59.295047 stigg_api_client-1.98.1/README.md
+-rw-r--r--   0        0        0      509 2024-03-31 14:17:35.567407 stigg_api_client-1.98.1/pyproject.toml
+-rw-r--r--   0        0        0       44 2024-03-31 14:16:59.295047 stigg_api_client-1.98.1/stigg/__init__.py
+-rw-r--r--   0        0        0     3721 2024-03-31 14:16:59.299047 stigg_api_client-1.98.1/stigg/client.py
+-rw-r--r--   0        0        0        0 2024-03-31 14:17:33.863392 stigg_api_client-1.98.1/stigg/generated/__init__.py
+-rw-r--r--   0        0        0    68286 2024-03-31 14:17:34.227395 stigg_api_client-1.98.1/stigg/generated/operations.py
+-rw-r--r--   0        0        0   569085 2024-03-31 14:17:34.079394 stigg_api_client-1.98.1/stigg/generated/schema.py
+-rw-r--r--   0        0        0     3197 1970-01-01 00:00:00.000000 stigg_api_client-1.98.1/PKG-INFO
```

### Comparing `stigg_api_client-1.98.0/LICENSE` & `stigg_api_client-1.98.1/LICENSE`

 * *Files identical despite different names*

### Comparing `stigg_api_client-1.98.0/README.md` & `stigg_api_client-1.98.1/README.md`

 * *Files identical despite different names*

### Comparing `stigg_api_client-1.98.0/stigg/client.py` & `stigg_api_client-1.98.1/stigg/client.py`

 * *Files identical despite different names*

### Comparing `stigg_api_client-1.98.0/stigg/generated/operations.py` & `stigg_api_client-1.98.1/stigg/generated/operations.py`

 * *Files 1% similar despite different names*

```diff
@@ -188,14 +188,15 @@
     _frag = sgqlc.operation.Fragment(_schema.PlanCompatiblePackageGroups, 'PlanCompatiblePackageGroupsFragment')
     _frag.package_group_id()
     _frag.display_name()
     _frag_addons = _frag.addons()
     _frag_addons.__fragment__(fragment_addon_fragment())
     _frag_options = _frag.options()
     _frag_options.min_items()
+    _frag_options.free_items()
     return _frag
 
 
 def fragment_customer_resource_fragment():
     _frag = sgqlc.operation.Fragment(_schema.CustomerResource, 'CustomerResourceFragment')
     _frag.resource_id()
     return _frag
@@ -960,15 +961,15 @@
     _frag.pricing_type()
     _frag_default_trial_config = _frag.default_trial_config()
     _frag_default_trial_config.duration()
     _frag_default_trial_config.units()
     _frag_compatible_addons = _frag.compatible_addons()
     _frag_compatible_addons.__fragment__(fragment_mock_paywall_addon_fragment())
     _frag_compatible_package_groups = _frag.compatible_package_groups()
-    _frag_compatible_package_groups.__fragment__(fragment_mock_paywall_package_group_fragment())
+    _frag_compatible_package_groups.__fragment__(fragment_mock_paywall_plan_compatible_package_groups_fragment())
     return _frag
 
 
 def fragment_mock_paywall_package_entitlement_fragment():
     _frag = sgqlc.operation.Fragment(_schema.Entitlement, 'MockPaywallPackageEntitlementFragment')
     _frag.usage_limit()
     _frag.has_unlimited_usage()
@@ -1023,32 +1024,45 @@
     _frag_feature.feature_units()
     _frag_feature.feature_units_plural()
     _frag_feature.display_name()
     _frag_feature.description()
     return _frag
 
 
-def fragment_mock_paywall_package_group_fragment():
-    _frag = sgqlc.operation.Fragment(_schema.PaywallPackageGroup, 'MockPaywallPackageGroupFragment')
+def fragment_mock_paywall_plan_compatible_package_groups_fragment():
+    _frag = sgqlc.operation.Fragment(_schema.PaywallPlanCompatiblePackageGroup, 'MockPaywallPlanCompatiblePackageGroupsFragment')
     _frag.package_group_id()
     _frag.display_name()
     _frag.description()
-    _frag_compatible_addons = _frag.compatible_addons()
-    _frag_compatible_addons.__fragment__(fragment_mock_paywall_addon_fragment())
+    _frag_addons = _frag.addons()
+    _frag_addons.__fragment__(fragment_mock_paywall_addon_fragment())
+    _frag_options = _frag.options()
+    _frag_options.min_items()
+    _frag_options.free_items()
+    return _frag
+
+
+def fragment_mock_paywall_addon_dependency_fragment():
+    _frag = sgqlc.operation.Fragment(_schema.PaywallAddon, 'MockPaywallAddonDependencyFragment')
+    _frag.ref_id()
+    _frag.display_name()
+    _frag.description()
     return _frag
 
 
 def fragment_mock_paywall_addon_fragment():
     _frag = sgqlc.operation.Fragment(_schema.PaywallAddon, 'MockPaywallAddonFragment')
     _frag.ref_id()
     _frag.display_name()
     _frag.description()
     _frag.additional_meta_data()
     _frag.billing_id()
     _frag.max_quantity()
+    _frag_dependencies = _frag.dependencies()
+    _frag_dependencies.__fragment__(fragment_mock_paywall_addon_dependency_fragment())
     _frag_entitlements = _frag.entitlements()
     _frag_entitlements.__fragment__(fragment_mock_paywall_package_entitlement_fragment())
     _frag_prices = _frag.prices()
     _frag_prices.__fragment__(fragment_mock_paywall_price_fragment())
     _frag.pricing_type()
     return _frag
 
@@ -1184,17 +1198,18 @@
     entitlement_fragment = fragment_entitlement_fragment()
     entitlement_usage_updated = fragment_entitlement_usage_updated()
     entitlements_updated_payload = fragment_entitlements_updated_payload()
     feature_fragment = fragment_feature_fragment()
     font_variant_fragment = fragment_font_variant_fragment()
     immediate_subscription_preview_invoice_fragment = fragment_immediate_subscription_preview_invoice_fragment()
     layout_configuration_fragment = fragment_layout_configuration_fragment()
+    mock_paywall_addon_dependency_fragment = fragment_mock_paywall_addon_dependency_fragment()
     mock_paywall_addon_fragment = fragment_mock_paywall_addon_fragment()
     mock_paywall_package_entitlement_fragment = fragment_mock_paywall_package_entitlement_fragment()
-    mock_paywall_package_group_fragment = fragment_mock_paywall_package_group_fragment()
+    mock_paywall_plan_compatible_package_groups_fragment = fragment_mock_paywall_plan_compatible_package_groups_fragment()
     mock_paywall_plan_fragment = fragment_mock_paywall_plan_fragment()
     mock_paywall_price_fragment = fragment_mock_paywall_price_fragment()
     overage_price_fragment = fragment_overage_price_fragment()
     package_entitlement_fragment = fragment_package_entitlement_fragment()
     package_published_payload = fragment_package_published_payload()
     paywall_calculated_price_points_fragment = fragment_paywall_calculated_price_points_fragment()
     paywall_configuration_fragment = fragment_paywall_configuration_fragment()
```

### Comparing `stigg_api_client-1.98.0/stigg/generated/schema.py` & `stigg_api_client-1.98.1/stigg/generated/schema.py`

 * *Files 0% similar despite different names*

```diff
@@ -6978,17 +6978,18 @@
     paywall_calculated_price_points = sgqlc.types.Field(sgqlc.types.list_of(sgqlc.types.non_null('PaywallPricePoint')), graphql_name='paywallCalculatedPricePoints')
     plans = sgqlc.types.Field(sgqlc.types.non_null(sgqlc.types.list_of(sgqlc.types.non_null('Plan'))), graphql_name='plans')
     resource = sgqlc.types.Field(CustomerResource, graphql_name='resource')
 
 
 class PaywallAddon(sgqlc.types.Type):
     __schema__ = schema
-    __field_names__ = ('additional_meta_data', 'billing_id', 'description', 'display_name', 'entitlements', 'max_quantity', 'prices', 'pricing_type', 'ref_id')
+    __field_names__ = ('additional_meta_data', 'billing_id', 'dependencies', 'description', 'display_name', 'entitlements', 'max_quantity', 'prices', 'pricing_type', 'ref_id')
     additional_meta_data = sgqlc.types.Field(JSON, graphql_name='additionalMetaData')
     billing_id = sgqlc.types.Field(String, graphql_name='billingId')
+    dependencies = sgqlc.types.Field(sgqlc.types.list_of(sgqlc.types.non_null('PaywallAddon')), graphql_name='dependencies')
     description = sgqlc.types.Field(String, graphql_name='description')
     display_name = sgqlc.types.Field(sgqlc.types.non_null(String), graphql_name='displayName')
     entitlements = sgqlc.types.Field(sgqlc.types.non_null(sgqlc.types.list_of(sgqlc.types.non_null(Entitlement))), graphql_name='entitlements')
     max_quantity = sgqlc.types.Field(Float, graphql_name='maxQuantity')
     prices = sgqlc.types.Field(sgqlc.types.non_null(sgqlc.types.list_of(sgqlc.types.non_null('PaywallPrice'))), graphql_name='prices')
     pricing_type = sgqlc.types.Field(PricingType, graphql_name='pricingType')
     ref_id = sgqlc.types.Field(sgqlc.types.non_null(String), graphql_name='refId')
@@ -7032,42 +7033,50 @@
     __field_names__ = ('alignment', 'plan_margin', 'plan_padding', 'plan_width')
     alignment = sgqlc.types.Field(Alignment, graphql_name='alignment')
     plan_margin = sgqlc.types.Field(Float, graphql_name='planMargin')
     plan_padding = sgqlc.types.Field(Float, graphql_name='planPadding')
     plan_width = sgqlc.types.Field(Float, graphql_name='planWidth')
 
 
-class PaywallPackageGroup(sgqlc.types.Type):
-    __schema__ = schema
-    __field_names__ = ('compatible_addons', 'description', 'display_name', 'package_group_id')
-    compatible_addons = sgqlc.types.Field(sgqlc.types.list_of(sgqlc.types.non_null(PaywallAddon)), graphql_name='compatibleAddons')
-    description = sgqlc.types.Field(String, graphql_name='description')
-    display_name = sgqlc.types.Field(sgqlc.types.non_null(String), graphql_name='displayName')
-    package_group_id = sgqlc.types.Field(sgqlc.types.non_null(String), graphql_name='packageGroupId')
-
-
 class PaywallPlan(sgqlc.types.Type):
     __schema__ = schema
     __field_names__ = ('additional_meta_data', 'base_plan', 'billing_id', 'compatible_addons', 'compatible_package_groups', 'default_trial_config', 'description', 'display_name', 'entitlements', 'inherited_entitlements', 'prices', 'pricing_type', 'product', 'ref_id')
     additional_meta_data = sgqlc.types.Field(JSON, graphql_name='additionalMetaData')
     base_plan = sgqlc.types.Field(PaywallBasePlan, graphql_name='basePlan')
     billing_id = sgqlc.types.Field(String, graphql_name='billingId')
     compatible_addons = sgqlc.types.Field(sgqlc.types.list_of(sgqlc.types.non_null(PaywallAddon)), graphql_name='compatibleAddons')
-    compatible_package_groups = sgqlc.types.Field(sgqlc.types.list_of(sgqlc.types.non_null(PaywallPackageGroup)), graphql_name='compatiblePackageGroups')
+    compatible_package_groups = sgqlc.types.Field(sgqlc.types.list_of(sgqlc.types.non_null('PaywallPlanCompatiblePackageGroup')), graphql_name='compatiblePackageGroups')
     default_trial_config = sgqlc.types.Field(DefaultTrialConfig, graphql_name='defaultTrialConfig')
     description = sgqlc.types.Field(String, graphql_name='description')
     display_name = sgqlc.types.Field(sgqlc.types.non_null(String), graphql_name='displayName')
     entitlements = sgqlc.types.Field(sgqlc.types.list_of(sgqlc.types.non_null(Entitlement)), graphql_name='entitlements')
     inherited_entitlements = sgqlc.types.Field(sgqlc.types.list_of(sgqlc.types.non_null(Entitlement)), graphql_name='inheritedEntitlements')
     prices = sgqlc.types.Field(sgqlc.types.non_null(sgqlc.types.list_of(sgqlc.types.non_null('PaywallPrice'))), graphql_name='prices')
     pricing_type = sgqlc.types.Field(PricingType, graphql_name='pricingType')
     product = sgqlc.types.Field(sgqlc.types.non_null('PaywallProduct'), graphql_name='product')
     ref_id = sgqlc.types.Field(sgqlc.types.non_null(String), graphql_name='refId')
 
 
+class PaywallPlanCompatiblePackageGroup(sgqlc.types.Type):
+    __schema__ = schema
+    __field_names__ = ('addons', 'description', 'display_name', 'options', 'package_group_id')
+    addons = sgqlc.types.Field(sgqlc.types.list_of(sgqlc.types.non_null(PaywallAddon)), graphql_name='addons')
+    description = sgqlc.types.Field(String, graphql_name='description')
+    display_name = sgqlc.types.Field(sgqlc.types.non_null(String), graphql_name='displayName')
+    options = sgqlc.types.Field(sgqlc.types.non_null('PaywallPlanCompatiblePackageGroupOptions'), graphql_name='options')
+    package_group_id = sgqlc.types.Field(sgqlc.types.non_null(String), graphql_name='packageGroupId')
+
+
+class PaywallPlanCompatiblePackageGroupOptions(sgqlc.types.Type):
+    __schema__ = schema
+    __field_names__ = ('free_items', 'min_items')
+    free_items = sgqlc.types.Field(Float, graphql_name='freeItems')
+    min_items = sgqlc.types.Field(Float, graphql_name='minItems')
+
+
 class PaywallPrice(sgqlc.types.Type):
     __schema__ = schema
     __field_names__ = ('billing_country_code', 'billing_id', 'billing_model', 'billing_period', 'feature', 'feature_id', 'max_unit_quantity', 'min_unit_quantity', 'price', 'tiers', 'tiers_mode')
     billing_country_code = sgqlc.types.Field(String, graphql_name='billingCountryCode')
     billing_id = sgqlc.types.Field(String, graphql_name='billingId')
     billing_model = sgqlc.types.Field(sgqlc.types.non_null(BillingModel), graphql_name='billingModel')
     billing_period = sgqlc.types.Field(sgqlc.types.non_null(BillingPeriod), graphql_name='billingPeriod')
```

### Comparing `stigg_api_client-1.98.0/PKG-INFO` & `stigg_api_client-1.98.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stigg-api-client
-Version: 1.98.0
+Version: 1.98.1
 Summary: 
 License: STIGG SDK LICENSE
 Author: Stigg
 Author-email: support@stigg.io
 Requires-Python: >=3.7,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

