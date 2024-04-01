# Comparing `tmp/pulumi_stripe-0.0.23.tar.gz` & `tmp/pulumi_stripe-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_stripe-0.0.23.tar", last modified: Mon Apr  1 14:47:03 2024, max compression
+gzip compressed data, was "pulumi_stripe-0.0.8.tar", last modified: Sun Aug 13 18:24:12 2023, max compression
```

## Comparing `pulumi_stripe-0.0.23.tar` & `pulumi_stripe-0.0.8.tar`

### file list

```diff
@@ -1,34 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 14:47:03.836001 pulumi_stripe-0.0.23/
--rw-r--r--   0 runner    (1001) docker     (127)     1730 2024-04-01 14:47:03.836001 pulumi_stripe-0.0.23/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1353 2024-04-01 14:47:03.000000 pulumi_stripe-0.0.23/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 14:47:03.836001 pulumi_stripe-0.0.23/pulumi_stripe/
--rw-r--r--   0 runner    (1001) docker     (127)     2662 2024-04-01 14:47:03.000000 pulumi_stripe-0.0.23/pulumi_stripe/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    67131 2024-04-01 14:47:03.000000 pulumi_stripe-0.0.23/pulumi_stripe/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     9283 2024-04-01 14:47:03.000000 pulumi_stripe-0.0.23/pulumi_stripe/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)    39329 2024-04-01 14:47:03.000000 pulumi_stripe-0.0.23/pulumi_stripe/card.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 14:47:03.836001 pulumi_stripe-0.0.23/pulumi_stripe/config/
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-01 14:47:03.000000 pulumi_stripe-0.0.23/pulumi_stripe/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      594 2024-04-01 14:47:03.000000 pulumi_stripe-0.0.23/pulumi_stripe/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (127)    36824 2024-04-01 14:47:03.000000 pulumi_stripe-0.0.23/pulumi_stripe/coupon.py
--rw-r--r--   0 runner    (1001) docker     (127)    39949 2024-04-01 14:47:03.000000 pulumi_stripe-0.0.23/pulumi_stripe/customer.py
--rw-r--r--   0 runner    (1001) docker     (127)    25601 2024-04-01 14:47:03.000000 pulumi_stripe-0.0.23/pulumi_stripe/file.py
--rw-r--r--   0 runner    (1001) docker     (127)    62981 2024-04-01 14:47:03.000000 pulumi_stripe-0.0.23/pulumi_stripe/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    30019 2024-04-01 14:47:03.000000 pulumi_stripe-0.0.23/pulumi_stripe/portal_configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)    59903 2024-04-01 14:47:03.000000 pulumi_stripe-0.0.23/pulumi_stripe/price.py
--rw-r--r--   0 runner    (1001) docker     (127)    40021 2024-04-01 14:47:03.000000 pulumi_stripe-0.0.23/pulumi_stripe/product.py
--rw-r--r--   0 runner    (1001) docker     (127)    28578 2024-04-01 14:47:03.000000 pulumi_stripe-0.0.23/pulumi_stripe/promotion_code.py
--rw-r--r--   0 runner    (1001) docker     (127)     4618 2024-04-01 14:47:03.000000 pulumi_stripe-0.0.23/pulumi_stripe/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-01 14:47:03.000000 pulumi_stripe-0.0.23/pulumi_stripe/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 14:47:03.000000 pulumi_stripe-0.0.23/pulumi_stripe/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    31922 2024-04-01 14:47:03.000000 pulumi_stripe-0.0.23/pulumi_stripe/shipping_rate.py
--rw-r--r--   0 runner    (1001) docker     (127)    33789 2024-04-01 14:47:03.000000 pulumi_stripe-0.0.23/pulumi_stripe/tax_rate.py
--rw-r--r--   0 runner    (1001) docker     (127)    24624 2024-04-01 14:47:03.000000 pulumi_stripe-0.0.23/pulumi_stripe/webhook_endpoint.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 14:47:03.836001 pulumi_stripe-0.0.23/pulumi_stripe.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1730 2024-04-01 14:47:03.000000 pulumi_stripe-0.0.23/pulumi_stripe.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      789 2024-04-01 14:47:03.000000 pulumi_stripe-0.0.23/pulumi_stripe.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 14:47:03.000000 pulumi_stripe-0.0.23/pulumi_stripe.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 14:47:03.000000 pulumi_stripe-0.0.23/pulumi_stripe.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-01 14:47:03.000000 pulumi_stripe-0.0.23/pulumi_stripe.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-01 14:47:03.000000 pulumi_stripe-0.0.23/pulumi_stripe.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-01 14:47:03.836001 pulumi_stripe-0.0.23/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1315 2024-04-01 14:47:03.000000 pulumi_stripe-0.0.23/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-13 18:24:12.687935 pulumi_stripe-0.0.8/
+-rw-r--r--   0 runner    (1001) docker     (123)    19518 2023-08-13 18:24:12.683935 pulumi_stripe-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    19136 2023-08-13 18:24:12.000000 pulumi_stripe-0.0.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-13 18:24:12.683935 pulumi_stripe-0.0.8/pulumi_stripe/
+-rw-r--r--   0 runner    (1001) docker     (123)     2321 2023-08-13 18:24:12.000000 pulumi_stripe-0.0.8/pulumi_stripe/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51017 2023-08-13 18:24:12.000000 pulumi_stripe-0.0.8/pulumi_stripe/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8081 2023-08-13 18:24:12.000000 pulumi_stripe-0.0.8/pulumi_stripe/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39173 2023-08-13 18:24:12.000000 pulumi_stripe-0.0.8/pulumi_stripe/card.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-13 18:24:12.683935 pulumi_stripe-0.0.8/pulumi_stripe/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-08-13 18:24:12.000000 pulumi_stripe-0.0.8/pulumi_stripe/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-08-13 18:24:12.000000 pulumi_stripe-0.0.8/pulumi_stripe/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34968 2023-08-13 18:24:12.000000 pulumi_stripe-0.0.8/pulumi_stripe/coupon.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39793 2023-08-13 18:24:12.000000 pulumi_stripe-0.0.8/pulumi_stripe/customer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48572 2023-08-13 18:24:12.000000 pulumi_stripe-0.0.8/pulumi_stripe/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28752 2023-08-13 18:24:12.000000 pulumi_stripe-0.0.8/pulumi_stripe/portal_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59761 2023-08-13 18:24:12.000000 pulumi_stripe-0.0.8/pulumi_stripe/price.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38046 2023-08-13 18:24:12.000000 pulumi_stripe-0.0.8/pulumi_stripe/product.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28422 2023-08-13 18:24:12.000000 pulumi_stripe-0.0.8/pulumi_stripe/promotion_code.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4618 2023-08-13 18:24:12.000000 pulumi_stripe-0.0.8/pulumi_stripe/provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-08-13 18:24:12.000000 pulumi_stripe-0.0.8/pulumi_stripe/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-13 18:24:12.000000 pulumi_stripe-0.0.8/pulumi_stripe/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    33633 2023-08-13 18:24:12.000000 pulumi_stripe-0.0.8/pulumi_stripe/tax_rate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24468 2023-08-13 18:24:12.000000 pulumi_stripe-0.0.8/pulumi_stripe/webhook_endpoint.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-13 18:24:12.683935 pulumi_stripe-0.0.8/pulumi_stripe.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    19518 2023-08-13 18:24:12.000000 pulumi_stripe-0.0.8/pulumi_stripe.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      736 2023-08-13 18:24:12.000000 pulumi_stripe-0.0.8/pulumi_stripe.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-13 18:24:12.000000 pulumi_stripe-0.0.8/pulumi_stripe.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-13 18:24:12.000000 pulumi_stripe-0.0.8/pulumi_stripe.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-08-13 18:24:12.000000 pulumi_stripe-0.0.8/pulumi_stripe.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-08-13 18:24:12.000000 pulumi_stripe-0.0.8/pulumi_stripe.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-13 18:24:12.687935 pulumi_stripe-0.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2145 2023-08-13 18:24:12.000000 pulumi_stripe-0.0.8/setup.py
```

### Comparing `pulumi_stripe-0.0.23/pulumi_stripe/__init__.py` & `pulumi_stripe-0.0.8/pulumi_stripe/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,21 +4,19 @@
 
 from . import _utilities
 import typing
 # Export this package's modules as members:
 from .card import *
 from .coupon import *
 from .customer import *
-from .file import *
 from .portal_configuration import *
 from .price import *
 from .product import *
 from .promotion_code import *
 from .provider import *
-from .shipping_rate import *
 from .tax_rate import *
 from .webhook_endpoint import *
 from ._inputs import *
 from . import outputs
 
 # Make subpackages available:
 if typing.TYPE_CHECKING:
@@ -52,22 +50,14 @@
   "fqn": "pulumi_stripe",
   "classes": {
    "stripe:index/customer:Customer": "Customer"
   }
  },
  {
   "pkg": "stripe",
-  "mod": "index/file",
-  "fqn": "pulumi_stripe",
-  "classes": {
-   "stripe:index/file:File": "File"
-  }
- },
- {
-  "pkg": "stripe",
   "mod": "index/portalConfiguration",
   "fqn": "pulumi_stripe",
   "classes": {
    "stripe:index/portalConfiguration:PortalConfiguration": "PortalConfiguration"
   }
  },
  {
@@ -92,22 +82,14 @@
   "fqn": "pulumi_stripe",
   "classes": {
    "stripe:index/promotionCode:PromotionCode": "PromotionCode"
   }
  },
  {
   "pkg": "stripe",
-  "mod": "index/shippingRate",
-  "fqn": "pulumi_stripe",
-  "classes": {
-   "stripe:index/shippingRate:ShippingRate": "ShippingRate"
-  }
- },
- {
-  "pkg": "stripe",
   "mod": "index/taxRate",
   "fqn": "pulumi_stripe",
   "classes": {
    "stripe:index/taxRate:TaxRate": "TaxRate"
   }
  },
  {
```

### Comparing `pulumi_stripe-0.0.23/pulumi_stripe/_inputs.py` & `pulumi_stripe-0.0.8/pulumi_stripe/_inputs.py`

 * *Files 16% similar despite different names*

```diff
@@ -6,16 +6,14 @@
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from . import _utilities
 
 __all__ = [
-    'FileLinkArgs',
-    'FileLinkDataArgs',
     'PortalConfigurationBusinessProfileArgs',
     'PortalConfigurationFeaturesArgs',
     'PortalConfigurationFeaturesCustomerUpdateArgs',
     'PortalConfigurationFeaturesInvoiceHistoryArgs',
     'PortalConfigurationFeaturesPaymentMethodUpdateArgs',
     'PortalConfigurationFeaturesSubscriptionCancelArgs',
     'PortalConfigurationFeaturesSubscriptionCancelCancellationReasonArgs',
@@ -26,221 +24,17 @@
     'PriceCurrencyOptionArgs',
     'PriceCurrencyOptionCustomUnitAmountArgs',
     'PriceCurrencyOptionTierArgs',
     'PriceRecurringArgs',
     'PriceTierArgs',
     'PriceTransformQuantityArgs',
     'PromotionCodeRestrictionsArgs',
-    'ShippingRateDeliveryEstimateArgs',
-    'ShippingRateDeliveryEstimateMaximumArgs',
-    'ShippingRateDeliveryEstimateMinimumArgs',
-    'ShippingRateFixedAmountArgs',
-    'ShippingRateFixedAmountCurrencyOptionArgs',
 ]
 
 @pulumi.input_type
-class FileLinkArgs:
-    def __init__(__self__, *,
-                 created: Optional[pulumi.Input[int]] = None,
-                 expired: Optional[pulumi.Input[bool]] = None,
-                 expires_at: Optional[pulumi.Input[int]] = None,
-                 id: Optional[pulumi.Input[str]] = None,
-                 livemode: Optional[pulumi.Input[bool]] = None,
-                 metadata: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
-                 object: Optional[pulumi.Input[str]] = None,
-                 url: Optional[pulumi.Input[str]] = None):
-        """
-        :param pulumi.Input[int] created: String. Time at which the object was created. Measured in seconds since the Unix epoch.
-        :param pulumi.Input[bool] expired: Bool. Returns if the link is already expired.
-        :param pulumi.Input[int] expires_at: Int. The link isn’t available after this future timestamp.
-        :param pulumi.Input[str] id: String. Unique identifier for the object.
-        :param pulumi.Input[bool] livemode: Bool. Has the value `true` if the object exists in live mode or the value `false` 
-               if the object exists in test mode.
-        :param pulumi.Input[Mapping[str, pulumi.Input[str]]] metadata: Map(String). Set of key-value pairs that you can attach to an object. 
-               This can be useful for storing additional information about the object in a structured format.
-        :param pulumi.Input[str] object: String. String representing the object’s type. Objects of the same type share the same value.
-        :param pulumi.Input[str] url: String. The publicly accessible URL to download the file.
-        """
-        if created is not None:
-            pulumi.set(__self__, "created", created)
-        if expired is not None:
-            pulumi.set(__self__, "expired", expired)
-        if expires_at is not None:
-            pulumi.set(__self__, "expires_at", expires_at)
-        if id is not None:
-            pulumi.set(__self__, "id", id)
-        if livemode is not None:
-            pulumi.set(__self__, "livemode", livemode)
-        if metadata is not None:
-            pulumi.set(__self__, "metadata", metadata)
-        if object is not None:
-            pulumi.set(__self__, "object", object)
-        if url is not None:
-            pulumi.set(__self__, "url", url)
-
-    @property
-    @pulumi.getter
-    def created(self) -> Optional[pulumi.Input[int]]:
-        """
-        String. Time at which the object was created. Measured in seconds since the Unix epoch.
-        """
-        return pulumi.get(self, "created")
-
-    @created.setter
-    def created(self, value: Optional[pulumi.Input[int]]):
-        pulumi.set(self, "created", value)
-
-    @property
-    @pulumi.getter
-    def expired(self) -> Optional[pulumi.Input[bool]]:
-        """
-        Bool. Returns if the link is already expired.
-        """
-        return pulumi.get(self, "expired")
-
-    @expired.setter
-    def expired(self, value: Optional[pulumi.Input[bool]]):
-        pulumi.set(self, "expired", value)
-
-    @property
-    @pulumi.getter(name="expiresAt")
-    def expires_at(self) -> Optional[pulumi.Input[int]]:
-        """
-        Int. The link isn’t available after this future timestamp.
-        """
-        return pulumi.get(self, "expires_at")
-
-    @expires_at.setter
-    def expires_at(self, value: Optional[pulumi.Input[int]]):
-        pulumi.set(self, "expires_at", value)
-
-    @property
-    @pulumi.getter
-    def id(self) -> Optional[pulumi.Input[str]]:
-        """
-        String. Unique identifier for the object.
-        """
-        return pulumi.get(self, "id")
-
-    @id.setter
-    def id(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "id", value)
-
-    @property
-    @pulumi.getter
-    def livemode(self) -> Optional[pulumi.Input[bool]]:
-        """
-        Bool. Has the value `true` if the object exists in live mode or the value `false` 
-        if the object exists in test mode.
-        """
-        return pulumi.get(self, "livemode")
-
-    @livemode.setter
-    def livemode(self, value: Optional[pulumi.Input[bool]]):
-        pulumi.set(self, "livemode", value)
-
-    @property
-    @pulumi.getter
-    def metadata(self) -> Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]:
-        """
-        Map(String). Set of key-value pairs that you can attach to an object. 
-        This can be useful for storing additional information about the object in a structured format.
-        """
-        return pulumi.get(self, "metadata")
-
-    @metadata.setter
-    def metadata(self, value: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]):
-        pulumi.set(self, "metadata", value)
-
-    @property
-    @pulumi.getter
-    def object(self) -> Optional[pulumi.Input[str]]:
-        """
-        String. String representing the object’s type. Objects of the same type share the same value.
-        """
-        return pulumi.get(self, "object")
-
-    @object.setter
-    def object(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "object", value)
-
-    @property
-    @pulumi.getter
-    def url(self) -> Optional[pulumi.Input[str]]:
-        """
-        String. The publicly accessible URL to download the file.
-        """
-        return pulumi.get(self, "url")
-
-    @url.setter
-    def url(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "url", value)
-
-
-@pulumi.input_type
-class FileLinkDataArgs:
-    def __init__(__self__, *,
-                 create: pulumi.Input[bool],
-                 expires_at: Optional[pulumi.Input[int]] = None,
-                 metadata: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None):
-        """
-        :param pulumi.Input[bool] create: Bool. Set this to `true` to create a file link for the newly created file. 
-               Creating a link is only possible when the file’s purpose is one of the following: `business_icon`, `business_logo`,
-               `customer_signature`, `dispute_evidence`, `pci_document`, `tax_document_user_upload`, or `terminal_reader_splashscreen`.
-        :param pulumi.Input[int] expires_at: Int. The link isn’t available after this future timestamp.
-        :param pulumi.Input[Mapping[str, pulumi.Input[str]]] metadata: Map(String). Set of key-value pairs that you can attach to an object. 
-               This can be useful for storing additional information about the object in a structured format.
-        """
-        pulumi.set(__self__, "create", create)
-        if expires_at is not None:
-            pulumi.set(__self__, "expires_at", expires_at)
-        if metadata is not None:
-            pulumi.set(__self__, "metadata", metadata)
-
-    @property
-    @pulumi.getter
-    def create(self) -> pulumi.Input[bool]:
-        """
-        Bool. Set this to `true` to create a file link for the newly created file. 
-        Creating a link is only possible when the file’s purpose is one of the following: `business_icon`, `business_logo`,
-        `customer_signature`, `dispute_evidence`, `pci_document`, `tax_document_user_upload`, or `terminal_reader_splashscreen`.
-        """
-        return pulumi.get(self, "create")
-
-    @create.setter
-    def create(self, value: pulumi.Input[bool]):
-        pulumi.set(self, "create", value)
-
-    @property
-    @pulumi.getter(name="expiresAt")
-    def expires_at(self) -> Optional[pulumi.Input[int]]:
-        """
-        Int. The link isn’t available after this future timestamp.
-        """
-        return pulumi.get(self, "expires_at")
-
-    @expires_at.setter
-    def expires_at(self, value: Optional[pulumi.Input[int]]):
-        pulumi.set(self, "expires_at", value)
-
-    @property
-    @pulumi.getter
-    def metadata(self) -> Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]:
-        """
-        Map(String). Set of key-value pairs that you can attach to an object. 
-        This can be useful for storing additional information about the object in a structured format.
-        """
-        return pulumi.get(self, "metadata")
-
-    @metadata.setter
-    def metadata(self, value: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]):
-        pulumi.set(self, "metadata", value)
-
-
-@pulumi.input_type
 class PortalConfigurationBusinessProfileArgs:
     def __init__(__self__, *,
                  headline: Optional[pulumi.Input[str]] = None,
                  privacy_policy_url: Optional[pulumi.Input[str]] = None,
                  terms_of_service_url: Optional[pulumi.Input[str]] = None):
         """
         :param pulumi.Input[str] headline: String. The messaging shown to customers in the portal.
@@ -396,26 +190,26 @@
 
 @pulumi.input_type
 class PortalConfigurationFeaturesCustomerUpdateArgs:
     def __init__(__self__, *,
                  enabled: pulumi.Input[bool],
                  allowed_updates: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None):
         """
-        :param pulumi.Input[bool] enabled: Bool. Whether the feature is enabled.
+        :param pulumi.Input[bool] enabled: Bool. Set to true to generate a shareable URL login_page.url that will take your customers to a hosted login page for the customer portal.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] allowed_updates: List(String). The types of customer updates that are supported [`name`, `email`, `address`, `shipping`, `phone`, `tax_id`]. When empty, customers are not updatable.
         """
         pulumi.set(__self__, "enabled", enabled)
         if allowed_updates is not None:
             pulumi.set(__self__, "allowed_updates", allowed_updates)
 
     @property
     @pulumi.getter
     def enabled(self) -> pulumi.Input[bool]:
         """
-        Bool. Whether the feature is enabled.
+        Bool. Set to true to generate a shareable URL login_page.url that will take your customers to a hosted login page for the customer portal.
         """
         return pulumi.get(self, "enabled")
 
     @enabled.setter
     def enabled(self, value: pulumi.Input[bool]):
         pulumi.set(self, "enabled", value)
 
@@ -433,45 +227,45 @@
 
 
 @pulumi.input_type
 class PortalConfigurationFeaturesInvoiceHistoryArgs:
     def __init__(__self__, *,
                  enabled: pulumi.Input[bool]):
         """
-        :param pulumi.Input[bool] enabled: Bool. Whether the feature is enabled.
+        :param pulumi.Input[bool] enabled: Bool. Set to true to generate a shareable URL login_page.url that will take your customers to a hosted login page for the customer portal.
         """
         pulumi.set(__self__, "enabled", enabled)
 
     @property
     @pulumi.getter
     def enabled(self) -> pulumi.Input[bool]:
         """
-        Bool. Whether the feature is enabled.
+        Bool. Set to true to generate a shareable URL login_page.url that will take your customers to a hosted login page for the customer portal.
         """
         return pulumi.get(self, "enabled")
 
     @enabled.setter
     def enabled(self, value: pulumi.Input[bool]):
         pulumi.set(self, "enabled", value)
 
 
 @pulumi.input_type
 class PortalConfigurationFeaturesPaymentMethodUpdateArgs:
     def __init__(__self__, *,
                  enabled: pulumi.Input[bool]):
         """
-        :param pulumi.Input[bool] enabled: Bool. Whether the feature is enabled.
+        :param pulumi.Input[bool] enabled: Bool. Set to true to generate a shareable URL login_page.url that will take your customers to a hosted login page for the customer portal.
         """
         pulumi.set(__self__, "enabled", enabled)
 
     @property
     @pulumi.getter
     def enabled(self) -> pulumi.Input[bool]:
         """
-        Bool. Whether the feature is enabled.
+        Bool. Set to true to generate a shareable URL login_page.url that will take your customers to a hosted login page for the customer portal.
         """
         return pulumi.get(self, "enabled")
 
     @enabled.setter
     def enabled(self, value: pulumi.Input[bool]):
         pulumi.set(self, "enabled", value)
 
@@ -480,15 +274,15 @@
 class PortalConfigurationFeaturesSubscriptionCancelArgs:
     def __init__(__self__, *,
                  enabled: pulumi.Input[bool],
                  cancellation_reason: Optional[pulumi.Input['PortalConfigurationFeaturesSubscriptionCancelCancellationReasonArgs']] = None,
                  mode: Optional[pulumi.Input[str]] = None,
                  proration_behavior: Optional[pulumi.Input[str]] = None):
         """
-        :param pulumi.Input[bool] enabled: Bool. Whether the feature is enabled.
+        :param pulumi.Input[bool] enabled: Bool. Set to true to generate a shareable URL login_page.url that will take your customers to a hosted login page for the customer portal.
         :param pulumi.Input['PortalConfigurationFeaturesSubscriptionCancelCancellationReasonArgs'] cancellation_reason: List(Resource). Whether the cancellation reasons will be collected in the portal and which options are exposed to the customer. Details of this field is in Cancellation Reason.
         :param pulumi.Input[str] mode: String. Whether to cancel subscriptions immediately or at the end of the billing period. Valid value is either `immediately` or `at_period_end`
         :param pulumi.Input[str] proration_behavior: String. Whether to create prorations when canceling subscriptions. Possible values are `none` and `create_prorations`, which is only compatible with `mode=immediately`. No prorations are generated when canceling a subscription at the end of its natural billing period.
         """
         pulumi.set(__self__, "enabled", enabled)
         if cancellation_reason is not None:
             pulumi.set(__self__, "cancellation_reason", cancellation_reason)
@@ -497,15 +291,15 @@
         if proration_behavior is not None:
             pulumi.set(__self__, "proration_behavior", proration_behavior)
 
     @property
     @pulumi.getter
     def enabled(self) -> pulumi.Input[bool]:
         """
-        Bool. Whether the feature is enabled.
+        Bool. Set to true to generate a shareable URL login_page.url that will take your customers to a hosted login page for the customer portal.
         """
         return pulumi.get(self, "enabled")
 
     @enabled.setter
     def enabled(self, value: pulumi.Input[bool]):
         pulumi.set(self, "enabled", value)
 
@@ -584,24 +378,24 @@
 
 
 @pulumi.input_type
 class PortalConfigurationFeaturesSubscriptionPauseArgs:
     def __init__(__self__, *,
                  enabled: Optional[pulumi.Input[bool]] = None):
         """
-        :param pulumi.Input[bool] enabled: Bool. Whether the feature is enabled.
+        :param pulumi.Input[bool] enabled: Bool. Set to true to generate a shareable URL login_page.url that will take your customers to a hosted login page for the customer portal.
         """
         if enabled is not None:
             pulumi.set(__self__, "enabled", enabled)
 
     @property
     @pulumi.getter
     def enabled(self) -> Optional[pulumi.Input[bool]]:
         """
-        Bool. Whether the feature is enabled.
+        Bool. Set to true to generate a shareable URL login_page.url that will take your customers to a hosted login page for the customer portal.
         """
         return pulumi.get(self, "enabled")
 
     @enabled.setter
     def enabled(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "enabled", value)
 
@@ -611,15 +405,15 @@
     def __init__(__self__, *,
                  default_allowed_updates: pulumi.Input[Sequence[pulumi.Input[str]]],
                  enabled: pulumi.Input[bool],
                  products: pulumi.Input[Sequence[pulumi.Input['PortalConfigurationFeaturesSubscriptionUpdateProductArgs']]],
                  proration_behavior: Optional[pulumi.Input[str]] = None):
         """
         :param pulumi.Input[Sequence[pulumi.Input[str]]] default_allowed_updates: List(String). The types of subscription updates that are supported. When empty, subscriptions are not updatable. Supported values are `price`, `quantity`, and `promotion_code`.
-        :param pulumi.Input[bool] enabled: Bool. Whether the feature is enabled.
+        :param pulumi.Input[bool] enabled: Bool. Set to true to generate a shareable URL login_page.url that will take your customers to a hosted login page for the customer portal.
         :param pulumi.Input[Sequence[pulumi.Input['PortalConfigurationFeaturesSubscriptionUpdateProductArgs']]] products: List(Resource). The list of products that support subscription updates. See details Products.
         :param pulumi.Input[str] proration_behavior: String. Whether to create prorations when canceling subscriptions. Possible values are `none` and `create_prorations`, which is only compatible with `mode=immediately`. No prorations are generated when canceling a subscription at the end of its natural billing period.
         """
         pulumi.set(__self__, "default_allowed_updates", default_allowed_updates)
         pulumi.set(__self__, "enabled", enabled)
         pulumi.set(__self__, "products", products)
         if proration_behavior is not None:
@@ -637,15 +431,15 @@
     def default_allowed_updates(self, value: pulumi.Input[Sequence[pulumi.Input[str]]]):
         pulumi.set(self, "default_allowed_updates", value)
 
     @property
     @pulumi.getter
     def enabled(self) -> pulumi.Input[bool]:
         """
-        Bool. Whether the feature is enabled.
+        Bool. Set to true to generate a shareable URL login_page.url that will take your customers to a hosted login page for the customer portal.
         """
         return pulumi.get(self, "enabled")
 
     @enabled.setter
     def enabled(self, value: pulumi.Input[bool]):
         pulumi.set(self, "enabled", value)
 
@@ -714,15 +508,14 @@
 @pulumi.input_type
 class PortalConfigurationLoginPageArgs:
     def __init__(__self__, *,
                  enabled: Optional[pulumi.Input[bool]] = None,
                  url: Optional[pulumi.Input[str]] = None):
         """
         :param pulumi.Input[bool] enabled: Bool. Set to true to generate a shareable URL login_page.url that will take your customers to a hosted login page for the customer portal.
-        :param pulumi.Input[str] url: A shareable URL to the hosted portal login page. Your customers will be able to log in with their email and receive a link to their customer portal.
         """
         if enabled is not None:
             pulumi.set(__self__, "enabled", enabled)
         if url is not None:
             pulumi.set(__self__, "url", url)
 
     @property
@@ -736,17 +529,14 @@
     @enabled.setter
     def enabled(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "enabled", value)
 
     @property
     @pulumi.getter
     def url(self) -> Optional[pulumi.Input[str]]:
-        """
-        A shareable URL to the hosted portal login page. Your customers will be able to log in with their email and receive a link to their customer portal.
-        """
         return pulumi.get(self, "url")
 
     @url.setter
     def url(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "url", value)
 
 
@@ -767,15 +557,15 @@
         :param pulumi.Input[str] tax_behavior: String. Only required if a default tax behavior was not provided in the Stripe Tax settings. 
                Specifies whether the price is considered inclusive of taxes or exclusive of taxes.
                One of `inclusive`, `exclusive`, or `unspecified`.
                Once specified as either inclusive or exclusive, it cannot be changed.
         :param pulumi.Input[Sequence[pulumi.Input['PriceCurrencyOptionTierArgs']]] tiers: List(Resource). Each element represents a pricing tier. 
                This parameter requires `billing_scheme` to be set to `tiered`. This resource can be used more than once and follows
                the same fields as the root tiers block
-        :param pulumi.Input[int] unit_amount: Int. A positive integer in cents (or -1 for a free price) representing how much to charge.
+        :param pulumi.Input[int] unit_amount: Int. A positive integer in cents (or 0 for a free price) representing how much to charge.
         :param pulumi.Input[float] unit_amount_decimal: Float. Same as unit_amount, but accepts a decimal value in cents with at most 12
                decimal places. Only one of unit_amount and unit_amount_decimal can be set.
         """
         pulumi.set(__self__, "currency", currency)
         if custom_unit_amount is not None:
             pulumi.set(__self__, "custom_unit_amount", custom_unit_amount)
         if tax_behavior is not None:
@@ -842,15 +632,15 @@
     def tiers(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['PriceCurrencyOptionTierArgs']]]]):
         pulumi.set(self, "tiers", value)
 
     @property
     @pulumi.getter(name="unitAmount")
     def unit_amount(self) -> Optional[pulumi.Input[int]]:
         """
-        Int. A positive integer in cents (or -1 for a free price) representing how much to charge.
+        Int. A positive integer in cents (or 0 for a free price) representing how much to charge.
         """
         return pulumi.get(self, "unit_amount")
 
     @unit_amount.setter
     def unit_amount(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "unit_amount", value)
 
@@ -1044,15 +834,15 @@
                  usage_type: Optional[pulumi.Input[str]] = None):
         """
         :param pulumi.Input[str] interval: String. Specifies billing frequency. Either `day`, `week`, `month` or `year`.
         :param pulumi.Input[str] aggregate_usage: String. Specifies a usage of aggregation strategy for prices of `usage_type=metered`.
                Allowed values are `sum` for summing up all usage during a period, `last_during_period` for using the last usage
                record reported within a period, `last_ever` for using the last usage record ever (across period bounds) or `max`
                which uses the usage record with the maximum reported usage during a period.
-        :param pulumi.Input[int] interval_count: Int. This parameter is (Required) when interval value is set. The number of intervals between subscription billings. For
+        :param pulumi.Input[int] interval_count: Int. The number of intervals between subscription billings. For
                example, `interval=month` and `interval_count=3` bills every 3 months. Maximum of one year interval allowed (1 year,
                12 months, or 52 weeks).
         :param pulumi.Input[str] usage_type: String. Configures how the quantity per period should be determined. Can be either `metered`
                or `licensed`. `licensed` automatically bills the quantity set when adding it to a subscription. `metered` aggregates
                the total usage based on usage records. Defaults to `licensed`.
         """
         pulumi.set(__self__, "interval", interval)
@@ -1090,15 +880,15 @@
     def aggregate_usage(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "aggregate_usage", value)
 
     @property
     @pulumi.getter(name="intervalCount")
     def interval_count(self) -> Optional[pulumi.Input[int]]:
         """
-        Int. This parameter is (Required) when interval value is set. The number of intervals between subscription billings. For
+        Int. The number of intervals between subscription billings. For
         example, `interval=month` and `interval_count=3` bills every 3 months. Maximum of one year interval allowed (1 year,
         12 months, or 52 weeks).
         """
         return pulumi.get(self, "interval_count")
 
     @interval_count.setter
     def interval_count(self, value: Optional[pulumi.Input[int]]):
@@ -1299,230 +1089,7 @@
         return pulumi.get(self, "minimum_amount_currency")
 
     @minimum_amount_currency.setter
     def minimum_amount_currency(self, value: pulumi.Input[str]):
         pulumi.set(self, "minimum_amount_currency", value)
 
 
-@pulumi.input_type
-class ShippingRateDeliveryEstimateArgs:
-    def __init__(__self__, *,
-                 maximum: Optional[pulumi.Input['ShippingRateDeliveryEstimateMaximumArgs']] = None,
-                 minimum: Optional[pulumi.Input['ShippingRateDeliveryEstimateMinimumArgs']] = None):
-        """
-        :param pulumi.Input['ShippingRateDeliveryEstimateMaximumArgs'] maximum: List(Resource. The upper bound of the estimated range.
-               Please see Delivery Estimate Definition.
-        :param pulumi.Input['ShippingRateDeliveryEstimateMinimumArgs'] minimum: List(Resource). The lower bound of the estimated range. 
-               Please see Delivery Estimate Definition.
-        """
-        if maximum is not None:
-            pulumi.set(__self__, "maximum", maximum)
-        if minimum is not None:
-            pulumi.set(__self__, "minimum", minimum)
-
-    @property
-    @pulumi.getter
-    def maximum(self) -> Optional[pulumi.Input['ShippingRateDeliveryEstimateMaximumArgs']]:
-        """
-        List(Resource. The upper bound of the estimated range.
-        Please see Delivery Estimate Definition.
-        """
-        return pulumi.get(self, "maximum")
-
-    @maximum.setter
-    def maximum(self, value: Optional[pulumi.Input['ShippingRateDeliveryEstimateMaximumArgs']]):
-        pulumi.set(self, "maximum", value)
-
-    @property
-    @pulumi.getter
-    def minimum(self) -> Optional[pulumi.Input['ShippingRateDeliveryEstimateMinimumArgs']]:
-        """
-        List(Resource). The lower bound of the estimated range. 
-        Please see Delivery Estimate Definition.
-        """
-        return pulumi.get(self, "minimum")
-
-    @minimum.setter
-    def minimum(self, value: Optional[pulumi.Input['ShippingRateDeliveryEstimateMinimumArgs']]):
-        pulumi.set(self, "minimum", value)
-
-
-@pulumi.input_type
-class ShippingRateDeliveryEstimateMaximumArgs:
-    def __init__(__self__, *,
-                 unit: pulumi.Input[str],
-                 value: pulumi.Input[int]):
-        """
-        :param pulumi.Input[str] unit: String. A unit of time. Possible values `hour`, `day`, `business_day`, `week` and `month`.
-        :param pulumi.Input[int] value: Int. Must be greater than 0.
-        """
-        pulumi.set(__self__, "unit", unit)
-        pulumi.set(__self__, "value", value)
-
-    @property
-    @pulumi.getter
-    def unit(self) -> pulumi.Input[str]:
-        """
-        String. A unit of time. Possible values `hour`, `day`, `business_day`, `week` and `month`.
-        """
-        return pulumi.get(self, "unit")
-
-    @unit.setter
-    def unit(self, value: pulumi.Input[str]):
-        pulumi.set(self, "unit", value)
-
-    @property
-    @pulumi.getter
-    def value(self) -> pulumi.Input[int]:
-        """
-        Int. Must be greater than 0.
-        """
-        return pulumi.get(self, "value")
-
-    @value.setter
-    def value(self, value: pulumi.Input[int]):
-        pulumi.set(self, "value", value)
-
-
-@pulumi.input_type
-class ShippingRateDeliveryEstimateMinimumArgs:
-    def __init__(__self__, *,
-                 unit: pulumi.Input[str],
-                 value: pulumi.Input[int]):
-        """
-        :param pulumi.Input[str] unit: String. A unit of time. Possible values `hour`, `day`, `business_day`, `week` and `month`.
-        :param pulumi.Input[int] value: Int. Must be greater than 0.
-        """
-        pulumi.set(__self__, "unit", unit)
-        pulumi.set(__self__, "value", value)
-
-    @property
-    @pulumi.getter
-    def unit(self) -> pulumi.Input[str]:
-        """
-        String. A unit of time. Possible values `hour`, `day`, `business_day`, `week` and `month`.
-        """
-        return pulumi.get(self, "unit")
-
-    @unit.setter
-    def unit(self, value: pulumi.Input[str]):
-        pulumi.set(self, "unit", value)
-
-    @property
-    @pulumi.getter
-    def value(self) -> pulumi.Input[int]:
-        """
-        Int. Must be greater than 0.
-        """
-        return pulumi.get(self, "value")
-
-    @value.setter
-    def value(self, value: pulumi.Input[int]):
-        pulumi.set(self, "value", value)
-
-
-@pulumi.input_type
-class ShippingRateFixedAmountArgs:
-    def __init__(__self__, *,
-                 amount: pulumi.Input[int],
-                 currency: pulumi.Input[str],
-                 currency_options: Optional[pulumi.Input[Sequence[pulumi.Input['ShippingRateFixedAmountCurrencyOptionArgs']]]] = None):
-        """
-        :param pulumi.Input[int] amount: Int. A non-negative integer in cents representing how much to charge.
-        :param pulumi.Input[str] currency: String. Three-letter ISO currency code, in lowercase - [supported currencies](https://stripe.com/docs/currencies).
-        :param pulumi.Input[Sequence[pulumi.Input['ShippingRateFixedAmountCurrencyOptionArgs']]] currency_options: List(Resource). Please see argument details Currency Option
-        """
-        pulumi.set(__self__, "amount", amount)
-        pulumi.set(__self__, "currency", currency)
-        if currency_options is not None:
-            pulumi.set(__self__, "currency_options", currency_options)
-
-    @property
-    @pulumi.getter
-    def amount(self) -> pulumi.Input[int]:
-        """
-        Int. A non-negative integer in cents representing how much to charge.
-        """
-        return pulumi.get(self, "amount")
-
-    @amount.setter
-    def amount(self, value: pulumi.Input[int]):
-        pulumi.set(self, "amount", value)
-
-    @property
-    @pulumi.getter
-    def currency(self) -> pulumi.Input[str]:
-        """
-        String. Three-letter ISO currency code, in lowercase - [supported currencies](https://stripe.com/docs/currencies).
-        """
-        return pulumi.get(self, "currency")
-
-    @currency.setter
-    def currency(self, value: pulumi.Input[str]):
-        pulumi.set(self, "currency", value)
-
-    @property
-    @pulumi.getter(name="currencyOptions")
-    def currency_options(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['ShippingRateFixedAmountCurrencyOptionArgs']]]]:
-        """
-        List(Resource). Please see argument details Currency Option
-        """
-        return pulumi.get(self, "currency_options")
-
-    @currency_options.setter
-    def currency_options(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['ShippingRateFixedAmountCurrencyOptionArgs']]]]):
-        pulumi.set(self, "currency_options", value)
-
-
-@pulumi.input_type
-class ShippingRateFixedAmountCurrencyOptionArgs:
-    def __init__(__self__, *,
-                 amount: pulumi.Input[int],
-                 currency: pulumi.Input[str],
-                 tax_behavior: Optional[pulumi.Input[str]] = None):
-        """
-        :param pulumi.Input[int] amount: Int. (Required) Int. A non-negative integer in cents representing how much to charge.
-        :param pulumi.Input[str] currency: String. Three-letter ISO currency code, in lowercase - [supported currencies](https://stripe.com/docs/currencies).
-        :param pulumi.Input[str] tax_behavior: Specifies whether the rate is considered inclusive of taxes or exclusive of taxes. One of inclusive, exclusive, or unspecified.
-        """
-        pulumi.set(__self__, "amount", amount)
-        pulumi.set(__self__, "currency", currency)
-        if tax_behavior is not None:
-            pulumi.set(__self__, "tax_behavior", tax_behavior)
-
-    @property
-    @pulumi.getter
-    def amount(self) -> pulumi.Input[int]:
-        """
-        Int. (Required) Int. A non-negative integer in cents representing how much to charge.
-        """
-        return pulumi.get(self, "amount")
-
-    @amount.setter
-    def amount(self, value: pulumi.Input[int]):
-        pulumi.set(self, "amount", value)
-
-    @property
-    @pulumi.getter
-    def currency(self) -> pulumi.Input[str]:
-        """
-        String. Three-letter ISO currency code, in lowercase - [supported currencies](https://stripe.com/docs/currencies).
-        """
-        return pulumi.get(self, "currency")
-
-    @currency.setter
-    def currency(self, value: pulumi.Input[str]):
-        pulumi.set(self, "currency", value)
-
-    @property
-    @pulumi.getter(name="taxBehavior")
-    def tax_behavior(self) -> Optional[pulumi.Input[str]]:
-        """
-        Specifies whether the rate is considered inclusive of taxes or exclusive of taxes. One of inclusive, exclusive, or unspecified.
-        """
-        return pulumi.get(self, "tax_behavior")
-
-    @tax_behavior.setter
-    def tax_behavior(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "tax_behavior", value)
-
-
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `pulumi_stripe-0.0.23/pulumi_stripe/_utilities.py` & `pulumi_stripe-0.0.8/pulumi_stripe/_utilities.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,22 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
 
-import asyncio
-import importlib.metadata
 import importlib.util
 import inspect
 import json
 import os
+import pkg_resources
 import sys
 import typing
 
 import pulumi
 import pulumi.runtime
-from pulumi.runtime.sync_await import _sync_await
 
 from semver import VersionInfo as SemverVersion
 from parver import Version as PEP440Version
 
 
 def get_env(*args):
     for v in args:
@@ -68,15 +66,15 @@
     # pkg_resources uses setuptools to inspect the set of installed packages. We use it here to ask
     # for the currently installed version of the root package (i.e. us) and get its version.
 
     # Unfortunately, PEP440 and semver differ slightly in incompatible ways. The Pulumi engine expects
     # to receive a valid semver string when receiving requests from the language host, so it's our
     # responsibility as the library to convert our own PEP440 version into a valid semver string.
 
-    pep440_version_string = importlib.metadata.version(root_package)
+    pep440_version_string = pkg_resources.require(root_package)[0].version
     pep440_version = PEP440Version.parse(pep440_version_string)
     (major, minor, patch) = pep440_version.release
     prerelease = None
     if pep440_version.pre_tag == 'a':
         prerelease = f"alpha.{pep440_version.pre}"
     elif pep440_version.pre_tag == 'b':
         prerelease = f"beta.{pep440_version.pre}"
@@ -244,48 +242,9 @@
             'kwargs': bound_args.kwargs
         }).apply(lambda resolved_args: func(*resolved_args['args'],
                                             opts=opts,
                                             **resolved_args['kwargs']))
 
     return (lambda _: lifted_func)
 
-
-def call_plain(
-    tok: str,
-    props: pulumi.Inputs,
-    res: typing.Optional[pulumi.Resource] = None,
-    typ: typing.Optional[type] = None,
-) -> typing.Any:
-    """
-    Wraps pulumi.runtime.plain to force the output and return it plainly.
-    """
-
-    output = pulumi.runtime.call(tok, props, res, typ)
-
-    # Ingoring deps silently. They are typically non-empty, r.f() calls include r as a dependency.
-    result, known, secret, _ = _sync_await(asyncio.ensure_future(_await_output(output)))
-
-    problem = None
-    if not known:
-        problem = ' an unknown value'
-    elif secret:
-        problem = ' a secret value'
-
-    if problem:
-        raise AssertionError(
-            f"Plain resource method '{tok}' incorrectly returned {problem}. "
-            + "This is an error in the provider, please report this to the provider developer."
-        )
-
-    return result
-
-
-async def _await_output(o: pulumi.Output[typing.Any]) -> typing.Tuple[object, bool, bool, set]:
-    return (
-        await o._future,
-        await o._is_known,
-        await o._is_secret,
-        await o._resources,
-    )
-
 def get_plugin_download_url():
-	return "github://api.github.com/georgegebbett"
+	return None
```

### Comparing `pulumi_stripe-0.0.23/pulumi_stripe/card.py` & `pulumi_stripe-0.0.8/pulumi_stripe/card.py`

 * *Files 1% similar despite different names*

```diff
@@ -484,15 +484,14 @@
                  metadata: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  number: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_stripe as stripe
 
         # card for the customer
         card_card = stripe.Card("cardCard",
             customer=stripe_customer["customer"]["id"],
@@ -512,15 +511,14 @@
                 "line2": "Apartment 401",
                 "city": "Sydney",
                 "state": "NSW",
                 "zip": "2000",
                 "country": "Australia",
             })
         ```
-        <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] address: Map(String). Address map with fields related to the address: `line1`, `line2`, `city`, `state`
                , `zip` and `country`.
         :param pulumi.Input[str] customer: String. The customer that this card belongs to.
         :param pulumi.Input[int] cvc: Int. Card security code. Highly recommended to always include this value, but it's required only
@@ -537,15 +535,14 @@
     def __init__(__self__,
                  resource_name: str,
                  args: CardArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_stripe as stripe
 
         # card for the customer
         card_card = stripe.Card("cardCard",
             customer=stripe_customer["customer"]["id"],
@@ -565,15 +562,14 @@
                 "line2": "Apartment 401",
                 "city": "Sydney",
                 "state": "NSW",
                 "zip": "2000",
                 "country": "Australia",
             })
         ```
-        <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
         :param CardArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
```

### Comparing `pulumi_stripe-0.0.23/pulumi_stripe/config/vars.py` & `pulumi_stripe-0.0.8/pulumi_stripe/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumi_stripe-0.0.23/pulumi_stripe/coupon.py` & `pulumi_stripe-0.0.8/pulumi_stripe/coupon.py`

 * *Files 2% similar despite different names*

```diff
@@ -433,40 +433,14 @@
 
         A coupon contains information about a percent-off or amount-off discount you might want to apply to a customer.
 
         A coupon has either a `percent_off` or an `amount_off` and `currency`. If you set an `amount_off`, that amount will be subtracted from any invoice’s subtotal.
 
         For example, an invoice with a subtotal of $100 will have a final total of $0 if a coupon with an amount_off of 20000 is applied to it and an invoice with a subtotal of $300 will have a final total of $100 if a coupon with an amount_off of 20000 is applied to it.
 
-        ## Example Usage
-
-        <!--Start PulumiCodeChooser -->
-        ```python
-        import pulumi
-        import pulumi_stripe as stripe
-
-        # coupon for the amount off discount
-        coupon_coupon = stripe.Coupon("couponCoupon",
-            amount_off=1000,
-            currency="aud",
-            duration="once",
-            max_redemptions=10)
-        # coupon for the percentage off discount
-        coupon_index_coupon_coupon = stripe.Coupon("couponIndex/couponCoupon",
-            percent_off=33.3,
-            duration="forever")
-        # coupon with limitation to a date and the product only
-        coupon_stripe_index_coupon_coupon = stripe.Coupon("couponStripeIndex/couponCoupon",
-            amount_off=2000,
-            duration="once",
-            redeem_by="2025-07-23T03:27:06+00:00",
-            applies_tos=[stripe_product["product"]["id"]])
-        ```
-        <!--End PulumiCodeChooser -->
-
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[int] amount_off: Int. Amount (in the currency specified) that will be taken off the subtotal of any invoices for this customer.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] applies_tos: List(String). A list of product IDs this coupon applies to.
         :param pulumi.Input[str] coupon_id: String. Unique string of your choice that will be used to identify this coupon when applying it to a customer.
         :param pulumi.Input[str] currency: String. Required if `amount_off` has been set, the three-letter ISO code for the currency of the amount to take off.
         :param pulumi.Input[str] duration: String. Describes how long a customer who applies this coupon will get the discount. One of `forever`, `once`, and `repeating`.
@@ -488,40 +462,14 @@
 
         A coupon contains information about a percent-off or amount-off discount you might want to apply to a customer.
 
         A coupon has either a `percent_off` or an `amount_off` and `currency`. If you set an `amount_off`, that amount will be subtracted from any invoice’s subtotal.
 
         For example, an invoice with a subtotal of $100 will have a final total of $0 if a coupon with an amount_off of 20000 is applied to it and an invoice with a subtotal of $300 will have a final total of $100 if a coupon with an amount_off of 20000 is applied to it.
 
-        ## Example Usage
-
-        <!--Start PulumiCodeChooser -->
-        ```python
-        import pulumi
-        import pulumi_stripe as stripe
-
-        # coupon for the amount off discount
-        coupon_coupon = stripe.Coupon("couponCoupon",
-            amount_off=1000,
-            currency="aud",
-            duration="once",
-            max_redemptions=10)
-        # coupon for the percentage off discount
-        coupon_index_coupon_coupon = stripe.Coupon("couponIndex/couponCoupon",
-            percent_off=33.3,
-            duration="forever")
-        # coupon with limitation to a date and the product only
-        coupon_stripe_index_coupon_coupon = stripe.Coupon("couponStripeIndex/couponCoupon",
-            amount_off=2000,
-            duration="once",
-            redeem_by="2025-07-23T03:27:06+00:00",
-            applies_tos=[stripe_product["product"]["id"]])
-        ```
-        <!--End PulumiCodeChooser -->
-
         :param str resource_name: The name of the resource.
         :param CouponArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
         resource_args, opts = _utilities.get_resource_args_opts(CouponArgs, pulumi.ResourceOptions, *args, **kwargs)
```

### Comparing `pulumi_stripe-0.0.23/pulumi_stripe/customer.py` & `pulumi_stripe-0.0.8/pulumi_stripe/customer.py`

 * *Files 1% similar despite different names*

```diff
@@ -449,15 +449,14 @@
         With this resource, you can create a customer - [Stripe API customer documentation](https://stripe.com/docs/api/customers).
 
         Customer objects allow you to perform recurring charges, and to track multiple charges,
         that are associated with the same customer.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_stripe as stripe
 
         # A customer with other details
         customer = stripe.Customer("customer",
             balance=10000,
@@ -478,15 +477,14 @@
                 "line2": "Apartment 401",
                 "name": "Lukas Aron",
                 "phone": "+610123456789",
                 "postal_code": "2000",
                 "state": "New South Wales",
             })
         ```
-        <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] address: Map(String). The customer’s address, for all individual fields see: Address Fields.
         :param pulumi.Input[int] balance: Int. Current balance, if any, being stored on the customer. If negative, the customer has credit to apply to their next invoice. If positive, the customer has an amount owed that will be added to their next invoice. The balance does not refer to any unpaid invoices; it solely takes into account amounts that have yet to be successfully applied to any invoice. This balance is only taken into account as invoices are finalized.
         :param pulumi.Input[str] description: String. An arbitrary string that you can attach to a customer object. It is displayed alongside the customer in the dashboard.
         :param pulumi.Input[str] email: String. Customer’s email address. It’s displayed alongside the customer in your dashboard and can be useful for searching and tracking. This may be up to 512 characters.
@@ -509,15 +507,14 @@
         With this resource, you can create a customer - [Stripe API customer documentation](https://stripe.com/docs/api/customers).
 
         Customer objects allow you to perform recurring charges, and to track multiple charges,
         that are associated with the same customer.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_stripe as stripe
 
         # A customer with other details
         customer = stripe.Customer("customer",
             balance=10000,
@@ -538,15 +535,14 @@
                 "line2": "Apartment 401",
                 "name": "Lukas Aron",
                 "phone": "+610123456789",
                 "postal_code": "2000",
                 "state": "New South Wales",
             })
         ```
-        <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
         :param CustomerArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
```

### Comparing `pulumi_stripe-0.0.23/pulumi_stripe/outputs.py` & `pulumi_stripe-0.0.8/pulumi_stripe/outputs.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,16 +7,14 @@
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from . import _utilities
 from . import outputs
 
 __all__ = [
-    'FileLink',
-    'FileLinkData',
     'PortalConfigurationBusinessProfile',
     'PortalConfigurationFeatures',
     'PortalConfigurationFeaturesCustomerUpdate',
     'PortalConfigurationFeaturesInvoiceHistory',
     'PortalConfigurationFeaturesPaymentMethodUpdate',
     'PortalConfigurationFeaturesSubscriptionCancel',
     'PortalConfigurationFeaturesSubscriptionCancelCancellationReason',
@@ -27,211 +25,17 @@
     'PriceCurrencyOption',
     'PriceCurrencyOptionCustomUnitAmount',
     'PriceCurrencyOptionTier',
     'PriceRecurring',
     'PriceTier',
     'PriceTransformQuantity',
     'PromotionCodeRestrictions',
-    'ShippingRateDeliveryEstimate',
-    'ShippingRateDeliveryEstimateMaximum',
-    'ShippingRateDeliveryEstimateMinimum',
-    'ShippingRateFixedAmount',
-    'ShippingRateFixedAmountCurrencyOption',
 ]
 
 @pulumi.output_type
-class FileLink(dict):
-    @staticmethod
-    def __key_warning(key: str):
-        suggest = None
-        if key == "expiresAt":
-            suggest = "expires_at"
-
-        if suggest:
-            pulumi.log.warn(f"Key '{key}' not found in FileLink. Access the value via the '{suggest}' property getter instead.")
-
-    def __getitem__(self, key: str) -> Any:
-        FileLink.__key_warning(key)
-        return super().__getitem__(key)
-
-    def get(self, key: str, default = None) -> Any:
-        FileLink.__key_warning(key)
-        return super().get(key, default)
-
-    def __init__(__self__, *,
-                 created: Optional[int] = None,
-                 expired: Optional[bool] = None,
-                 expires_at: Optional[int] = None,
-                 id: Optional[str] = None,
-                 livemode: Optional[bool] = None,
-                 metadata: Optional[Mapping[str, str]] = None,
-                 object: Optional[str] = None,
-                 url: Optional[str] = None):
-        """
-        :param int created: String. Time at which the object was created. Measured in seconds since the Unix epoch.
-        :param bool expired: Bool. Returns if the link is already expired.
-        :param int expires_at: Int. The link isn’t available after this future timestamp.
-        :param str id: String. Unique identifier for the object.
-        :param bool livemode: Bool. Has the value `true` if the object exists in live mode or the value `false` 
-               if the object exists in test mode.
-        :param Mapping[str, str] metadata: Map(String). Set of key-value pairs that you can attach to an object. 
-               This can be useful for storing additional information about the object in a structured format.
-        :param str object: String. String representing the object’s type. Objects of the same type share the same value.
-        :param str url: String. The publicly accessible URL to download the file.
-        """
-        if created is not None:
-            pulumi.set(__self__, "created", created)
-        if expired is not None:
-            pulumi.set(__self__, "expired", expired)
-        if expires_at is not None:
-            pulumi.set(__self__, "expires_at", expires_at)
-        if id is not None:
-            pulumi.set(__self__, "id", id)
-        if livemode is not None:
-            pulumi.set(__self__, "livemode", livemode)
-        if metadata is not None:
-            pulumi.set(__self__, "metadata", metadata)
-        if object is not None:
-            pulumi.set(__self__, "object", object)
-        if url is not None:
-            pulumi.set(__self__, "url", url)
-
-    @property
-    @pulumi.getter
-    def created(self) -> Optional[int]:
-        """
-        String. Time at which the object was created. Measured in seconds since the Unix epoch.
-        """
-        return pulumi.get(self, "created")
-
-    @property
-    @pulumi.getter
-    def expired(self) -> Optional[bool]:
-        """
-        Bool. Returns if the link is already expired.
-        """
-        return pulumi.get(self, "expired")
-
-    @property
-    @pulumi.getter(name="expiresAt")
-    def expires_at(self) -> Optional[int]:
-        """
-        Int. The link isn’t available after this future timestamp.
-        """
-        return pulumi.get(self, "expires_at")
-
-    @property
-    @pulumi.getter
-    def id(self) -> Optional[str]:
-        """
-        String. Unique identifier for the object.
-        """
-        return pulumi.get(self, "id")
-
-    @property
-    @pulumi.getter
-    def livemode(self) -> Optional[bool]:
-        """
-        Bool. Has the value `true` if the object exists in live mode or the value `false` 
-        if the object exists in test mode.
-        """
-        return pulumi.get(self, "livemode")
-
-    @property
-    @pulumi.getter
-    def metadata(self) -> Optional[Mapping[str, str]]:
-        """
-        Map(String). Set of key-value pairs that you can attach to an object. 
-        This can be useful for storing additional information about the object in a structured format.
-        """
-        return pulumi.get(self, "metadata")
-
-    @property
-    @pulumi.getter
-    def object(self) -> Optional[str]:
-        """
-        String. String representing the object’s type. Objects of the same type share the same value.
-        """
-        return pulumi.get(self, "object")
-
-    @property
-    @pulumi.getter
-    def url(self) -> Optional[str]:
-        """
-        String. The publicly accessible URL to download the file.
-        """
-        return pulumi.get(self, "url")
-
-
-@pulumi.output_type
-class FileLinkData(dict):
-    @staticmethod
-    def __key_warning(key: str):
-        suggest = None
-        if key == "expiresAt":
-            suggest = "expires_at"
-
-        if suggest:
-            pulumi.log.warn(f"Key '{key}' not found in FileLinkData. Access the value via the '{suggest}' property getter instead.")
-
-    def __getitem__(self, key: str) -> Any:
-        FileLinkData.__key_warning(key)
-        return super().__getitem__(key)
-
-    def get(self, key: str, default = None) -> Any:
-        FileLinkData.__key_warning(key)
-        return super().get(key, default)
-
-    def __init__(__self__, *,
-                 create: bool,
-                 expires_at: Optional[int] = None,
-                 metadata: Optional[Mapping[str, str]] = None):
-        """
-        :param bool create: Bool. Set this to `true` to create a file link for the newly created file. 
-               Creating a link is only possible when the file’s purpose is one of the following: `business_icon`, `business_logo`,
-               `customer_signature`, `dispute_evidence`, `pci_document`, `tax_document_user_upload`, or `terminal_reader_splashscreen`.
-        :param int expires_at: Int. The link isn’t available after this future timestamp.
-        :param Mapping[str, str] metadata: Map(String). Set of key-value pairs that you can attach to an object. 
-               This can be useful for storing additional information about the object in a structured format.
-        """
-        pulumi.set(__self__, "create", create)
-        if expires_at is not None:
-            pulumi.set(__self__, "expires_at", expires_at)
-        if metadata is not None:
-            pulumi.set(__self__, "metadata", metadata)
-
-    @property
-    @pulumi.getter
-    def create(self) -> bool:
-        """
-        Bool. Set this to `true` to create a file link for the newly created file. 
-        Creating a link is only possible when the file’s purpose is one of the following: `business_icon`, `business_logo`,
-        `customer_signature`, `dispute_evidence`, `pci_document`, `tax_document_user_upload`, or `terminal_reader_splashscreen`.
-        """
-        return pulumi.get(self, "create")
-
-    @property
-    @pulumi.getter(name="expiresAt")
-    def expires_at(self) -> Optional[int]:
-        """
-        Int. The link isn’t available after this future timestamp.
-        """
-        return pulumi.get(self, "expires_at")
-
-    @property
-    @pulumi.getter
-    def metadata(self) -> Optional[Mapping[str, str]]:
-        """
-        Map(String). Set of key-value pairs that you can attach to an object. 
-        This can be useful for storing additional information about the object in a structured format.
-        """
-        return pulumi.get(self, "metadata")
-
-
-@pulumi.output_type
 class PortalConfigurationBusinessProfile(dict):
     @staticmethod
     def __key_warning(key: str):
         suggest = None
         if key == "privacyPolicyUrl":
             suggest = "privacy_policy_url"
         elif key == "termsOfServiceUrl":
@@ -414,26 +218,26 @@
         PortalConfigurationFeaturesCustomerUpdate.__key_warning(key)
         return super().get(key, default)
 
     def __init__(__self__, *,
                  enabled: bool,
                  allowed_updates: Optional[Sequence[str]] = None):
         """
-        :param bool enabled: Bool. Whether the feature is enabled.
+        :param bool enabled: Bool. Set to true to generate a shareable URL login_page.url that will take your customers to a hosted login page for the customer portal.
         :param Sequence[str] allowed_updates: List(String). The types of customer updates that are supported [`name`, `email`, `address`, `shipping`, `phone`, `tax_id`]. When empty, customers are not updatable.
         """
         pulumi.set(__self__, "enabled", enabled)
         if allowed_updates is not None:
             pulumi.set(__self__, "allowed_updates", allowed_updates)
 
     @property
     @pulumi.getter
     def enabled(self) -> bool:
         """
-        Bool. Whether the feature is enabled.
+        Bool. Set to true to generate a shareable URL login_page.url that will take your customers to a hosted login page for the customer portal.
         """
         return pulumi.get(self, "enabled")
 
     @property
     @pulumi.getter(name="allowedUpdates")
     def allowed_updates(self) -> Optional[Sequence[str]]:
         """
@@ -443,41 +247,41 @@
 
 
 @pulumi.output_type
 class PortalConfigurationFeaturesInvoiceHistory(dict):
     def __init__(__self__, *,
                  enabled: bool):
         """
-        :param bool enabled: Bool. Whether the feature is enabled.
+        :param bool enabled: Bool. Set to true to generate a shareable URL login_page.url that will take your customers to a hosted login page for the customer portal.
         """
         pulumi.set(__self__, "enabled", enabled)
 
     @property
     @pulumi.getter
     def enabled(self) -> bool:
         """
-        Bool. Whether the feature is enabled.
+        Bool. Set to true to generate a shareable URL login_page.url that will take your customers to a hosted login page for the customer portal.
         """
         return pulumi.get(self, "enabled")
 
 
 @pulumi.output_type
 class PortalConfigurationFeaturesPaymentMethodUpdate(dict):
     def __init__(__self__, *,
                  enabled: bool):
         """
-        :param bool enabled: Bool. Whether the feature is enabled.
+        :param bool enabled: Bool. Set to true to generate a shareable URL login_page.url that will take your customers to a hosted login page for the customer portal.
         """
         pulumi.set(__self__, "enabled", enabled)
 
     @property
     @pulumi.getter
     def enabled(self) -> bool:
         """
-        Bool. Whether the feature is enabled.
+        Bool. Set to true to generate a shareable URL login_page.url that will take your customers to a hosted login page for the customer portal.
         """
         return pulumi.get(self, "enabled")
 
 
 @pulumi.output_type
 class PortalConfigurationFeaturesSubscriptionCancel(dict):
     @staticmethod
@@ -501,15 +305,15 @@
 
     def __init__(__self__, *,
                  enabled: bool,
                  cancellation_reason: Optional['outputs.PortalConfigurationFeaturesSubscriptionCancelCancellationReason'] = None,
                  mode: Optional[str] = None,
                  proration_behavior: Optional[str] = None):
         """
-        :param bool enabled: Bool. Whether the feature is enabled.
+        :param bool enabled: Bool. Set to true to generate a shareable URL login_page.url that will take your customers to a hosted login page for the customer portal.
         :param 'PortalConfigurationFeaturesSubscriptionCancelCancellationReasonArgs' cancellation_reason: List(Resource). Whether the cancellation reasons will be collected in the portal and which options are exposed to the customer. Details of this field is in Cancellation Reason.
         :param str mode: String. Whether to cancel subscriptions immediately or at the end of the billing period. Valid value is either `immediately` or `at_period_end`
         :param str proration_behavior: String. Whether to create prorations when canceling subscriptions. Possible values are `none` and `create_prorations`, which is only compatible with `mode=immediately`. No prorations are generated when canceling a subscription at the end of its natural billing period.
         """
         pulumi.set(__self__, "enabled", enabled)
         if cancellation_reason is not None:
             pulumi.set(__self__, "cancellation_reason", cancellation_reason)
@@ -518,15 +322,15 @@
         if proration_behavior is not None:
             pulumi.set(__self__, "proration_behavior", proration_behavior)
 
     @property
     @pulumi.getter
     def enabled(self) -> bool:
         """
-        Bool. Whether the feature is enabled.
+        Bool. Set to true to generate a shareable URL login_page.url that will take your customers to a hosted login page for the customer portal.
         """
         return pulumi.get(self, "enabled")
 
     @property
     @pulumi.getter(name="cancellationReason")
     def cancellation_reason(self) -> Optional['outputs.PortalConfigurationFeaturesSubscriptionCancelCancellationReason']:
         """
@@ -581,24 +385,24 @@
 
 
 @pulumi.output_type
 class PortalConfigurationFeaturesSubscriptionPause(dict):
     def __init__(__self__, *,
                  enabled: Optional[bool] = None):
         """
-        :param bool enabled: Bool. Whether the feature is enabled.
+        :param bool enabled: Bool. Set to true to generate a shareable URL login_page.url that will take your customers to a hosted login page for the customer portal.
         """
         if enabled is not None:
             pulumi.set(__self__, "enabled", enabled)
 
     @property
     @pulumi.getter
     def enabled(self) -> Optional[bool]:
         """
-        Bool. Whether the feature is enabled.
+        Bool. Set to true to generate a shareable URL login_page.url that will take your customers to a hosted login page for the customer portal.
         """
         return pulumi.get(self, "enabled")
 
 
 @pulumi.output_type
 class PortalConfigurationFeaturesSubscriptionUpdate(dict):
     @staticmethod
@@ -623,15 +427,15 @@
     def __init__(__self__, *,
                  default_allowed_updates: Sequence[str],
                  enabled: bool,
                  products: Sequence['outputs.PortalConfigurationFeaturesSubscriptionUpdateProduct'],
                  proration_behavior: Optional[str] = None):
         """
         :param Sequence[str] default_allowed_updates: List(String). The types of subscription updates that are supported. When empty, subscriptions are not updatable. Supported values are `price`, `quantity`, and `promotion_code`.
-        :param bool enabled: Bool. Whether the feature is enabled.
+        :param bool enabled: Bool. Set to true to generate a shareable URL login_page.url that will take your customers to a hosted login page for the customer portal.
         :param Sequence['PortalConfigurationFeaturesSubscriptionUpdateProductArgs'] products: List(Resource). The list of products that support subscription updates. See details Products.
         :param str proration_behavior: String. Whether to create prorations when canceling subscriptions. Possible values are `none` and `create_prorations`, which is only compatible with `mode=immediately`. No prorations are generated when canceling a subscription at the end of its natural billing period.
         """
         pulumi.set(__self__, "default_allowed_updates", default_allowed_updates)
         pulumi.set(__self__, "enabled", enabled)
         pulumi.set(__self__, "products", products)
         if proration_behavior is not None:
@@ -645,15 +449,15 @@
         """
         return pulumi.get(self, "default_allowed_updates")
 
     @property
     @pulumi.getter
     def enabled(self) -> bool:
         """
-        Bool. Whether the feature is enabled.
+        Bool. Set to true to generate a shareable URL login_page.url that will take your customers to a hosted login page for the customer portal.
         """
         return pulumi.get(self, "enabled")
 
     @property
     @pulumi.getter
     def products(self) -> Sequence['outputs.PortalConfigurationFeaturesSubscriptionUpdateProduct']:
         """
@@ -702,15 +506,14 @@
 @pulumi.output_type
 class PortalConfigurationLoginPage(dict):
     def __init__(__self__, *,
                  enabled: Optional[bool] = None,
                  url: Optional[str] = None):
         """
         :param bool enabled: Bool. Set to true to generate a shareable URL login_page.url that will take your customers to a hosted login page for the customer portal.
-        :param str url: A shareable URL to the hosted portal login page. Your customers will be able to log in with their email and receive a link to their customer portal.
         """
         if enabled is not None:
             pulumi.set(__self__, "enabled", enabled)
         if url is not None:
             pulumi.set(__self__, "url", url)
 
     @property
@@ -720,17 +523,14 @@
         Bool. Set to true to generate a shareable URL login_page.url that will take your customers to a hosted login page for the customer portal.
         """
         return pulumi.get(self, "enabled")
 
     @property
     @pulumi.getter
     def url(self) -> Optional[str]:
-        """
-        A shareable URL to the hosted portal login page. Your customers will be able to log in with their email and receive a link to their customer portal.
-        """
         return pulumi.get(self, "url")
 
 
 @pulumi.output_type
 class PriceCurrencyOption(dict):
     @staticmethod
     def __key_warning(key: str):
@@ -770,15 +570,15 @@
         :param str tax_behavior: String. Only required if a default tax behavior was not provided in the Stripe Tax settings. 
                Specifies whether the price is considered inclusive of taxes or exclusive of taxes.
                One of `inclusive`, `exclusive`, or `unspecified`.
                Once specified as either inclusive or exclusive, it cannot be changed.
         :param Sequence['PriceCurrencyOptionTierArgs'] tiers: List(Resource). Each element represents a pricing tier. 
                This parameter requires `billing_scheme` to be set to `tiered`. This resource can be used more than once and follows
                the same fields as the root tiers block
-        :param int unit_amount: Int. A positive integer in cents (or -1 for a free price) representing how much to charge.
+        :param int unit_amount: Int. A positive integer in cents (or 0 for a free price) representing how much to charge.
         :param float unit_amount_decimal: Float. Same as unit_amount, but accepts a decimal value in cents with at most 12
                decimal places. Only one of unit_amount and unit_amount_decimal can be set.
         """
         pulumi.set(__self__, "currency", currency)
         if custom_unit_amount is not None:
             pulumi.set(__self__, "custom_unit_amount", custom_unit_amount)
         if tax_behavior is not None:
@@ -829,15 +629,15 @@
         """
         return pulumi.get(self, "tiers")
 
     @property
     @pulumi.getter(name="unitAmount")
     def unit_amount(self) -> Optional[int]:
         """
-        Int. A positive integer in cents (or -1 for a free price) representing how much to charge.
+        Int. A positive integer in cents (or 0 for a free price) representing how much to charge.
         """
         return pulumi.get(self, "unit_amount")
 
     @property
     @pulumi.getter(name="unitAmountDecimal")
     def unit_amount_decimal(self) -> Optional[float]:
         """
@@ -1033,15 +833,15 @@
                  usage_type: Optional[str] = None):
         """
         :param str interval: String. Specifies billing frequency. Either `day`, `week`, `month` or `year`.
         :param str aggregate_usage: String. Specifies a usage of aggregation strategy for prices of `usage_type=metered`.
                Allowed values are `sum` for summing up all usage during a period, `last_during_period` for using the last usage
                record reported within a period, `last_ever` for using the last usage record ever (across period bounds) or `max`
                which uses the usage record with the maximum reported usage during a period.
-        :param int interval_count: Int. This parameter is (Required) when interval value is set. The number of intervals between subscription billings. For
+        :param int interval_count: Int. The number of intervals between subscription billings. For
                example, `interval=month` and `interval_count=3` bills every 3 months. Maximum of one year interval allowed (1 year,
                12 months, or 52 weeks).
         :param str usage_type: String. Configures how the quantity per period should be determined. Can be either `metered`
                or `licensed`. `licensed` automatically bills the quantity set when adding it to a subscription. `metered` aggregates
                the total usage based on usage records. Defaults to `licensed`.
         """
         pulumi.set(__self__, "interval", interval)
@@ -1071,15 +871,15 @@
         """
         return pulumi.get(self, "aggregate_usage")
 
     @property
     @pulumi.getter(name="intervalCount")
     def interval_count(self) -> Optional[int]:
         """
-        Int. This parameter is (Required) when interval value is set. The number of intervals between subscription billings. For
+        Int. The number of intervals between subscription billings. For
         example, `interval=month` and `interval_count=3` bills every 3 months. Maximum of one year interval allowed (1 year,
         12 months, or 52 weeks).
         """
         return pulumi.get(self, "interval_count")
 
     @property
     @pulumi.getter(name="usageType")
@@ -1295,216 +1095,7 @@
     def minimum_amount_currency(self) -> str:
         """
         String. Three-letter ISO code for `minimum_amount`.
         """
         return pulumi.get(self, "minimum_amount_currency")
 
 
-@pulumi.output_type
-class ShippingRateDeliveryEstimate(dict):
-    def __init__(__self__, *,
-                 maximum: Optional['outputs.ShippingRateDeliveryEstimateMaximum'] = None,
-                 minimum: Optional['outputs.ShippingRateDeliveryEstimateMinimum'] = None):
-        """
-        :param 'ShippingRateDeliveryEstimateMaximumArgs' maximum: List(Resource. The upper bound of the estimated range.
-               Please see Delivery Estimate Definition.
-        :param 'ShippingRateDeliveryEstimateMinimumArgs' minimum: List(Resource). The lower bound of the estimated range. 
-               Please see Delivery Estimate Definition.
-        """
-        if maximum is not None:
-            pulumi.set(__self__, "maximum", maximum)
-        if minimum is not None:
-            pulumi.set(__self__, "minimum", minimum)
-
-    @property
-    @pulumi.getter
-    def maximum(self) -> Optional['outputs.ShippingRateDeliveryEstimateMaximum']:
-        """
-        List(Resource. The upper bound of the estimated range.
-        Please see Delivery Estimate Definition.
-        """
-        return pulumi.get(self, "maximum")
-
-    @property
-    @pulumi.getter
-    def minimum(self) -> Optional['outputs.ShippingRateDeliveryEstimateMinimum']:
-        """
-        List(Resource). The lower bound of the estimated range. 
-        Please see Delivery Estimate Definition.
-        """
-        return pulumi.get(self, "minimum")
-
-
-@pulumi.output_type
-class ShippingRateDeliveryEstimateMaximum(dict):
-    def __init__(__self__, *,
-                 unit: str,
-                 value: int):
-        """
-        :param str unit: String. A unit of time. Possible values `hour`, `day`, `business_day`, `week` and `month`.
-        :param int value: Int. Must be greater than 0.
-        """
-        pulumi.set(__self__, "unit", unit)
-        pulumi.set(__self__, "value", value)
-
-    @property
-    @pulumi.getter
-    def unit(self) -> str:
-        """
-        String. A unit of time. Possible values `hour`, `day`, `business_day`, `week` and `month`.
-        """
-        return pulumi.get(self, "unit")
-
-    @property
-    @pulumi.getter
-    def value(self) -> int:
-        """
-        Int. Must be greater than 0.
-        """
-        return pulumi.get(self, "value")
-
-
-@pulumi.output_type
-class ShippingRateDeliveryEstimateMinimum(dict):
-    def __init__(__self__, *,
-                 unit: str,
-                 value: int):
-        """
-        :param str unit: String. A unit of time. Possible values `hour`, `day`, `business_day`, `week` and `month`.
-        :param int value: Int. Must be greater than 0.
-        """
-        pulumi.set(__self__, "unit", unit)
-        pulumi.set(__self__, "value", value)
-
-    @property
-    @pulumi.getter
-    def unit(self) -> str:
-        """
-        String. A unit of time. Possible values `hour`, `day`, `business_day`, `week` and `month`.
-        """
-        return pulumi.get(self, "unit")
-
-    @property
-    @pulumi.getter
-    def value(self) -> int:
-        """
-        Int. Must be greater than 0.
-        """
-        return pulumi.get(self, "value")
-
-
-@pulumi.output_type
-class ShippingRateFixedAmount(dict):
-    @staticmethod
-    def __key_warning(key: str):
-        suggest = None
-        if key == "currencyOptions":
-            suggest = "currency_options"
-
-        if suggest:
-            pulumi.log.warn(f"Key '{key}' not found in ShippingRateFixedAmount. Access the value via the '{suggest}' property getter instead.")
-
-    def __getitem__(self, key: str) -> Any:
-        ShippingRateFixedAmount.__key_warning(key)
-        return super().__getitem__(key)
-
-    def get(self, key: str, default = None) -> Any:
-        ShippingRateFixedAmount.__key_warning(key)
-        return super().get(key, default)
-
-    def __init__(__self__, *,
-                 amount: int,
-                 currency: str,
-                 currency_options: Optional[Sequence['outputs.ShippingRateFixedAmountCurrencyOption']] = None):
-        """
-        :param int amount: Int. A non-negative integer in cents representing how much to charge.
-        :param str currency: String. Three-letter ISO currency code, in lowercase - [supported currencies](https://stripe.com/docs/currencies).
-        :param Sequence['ShippingRateFixedAmountCurrencyOptionArgs'] currency_options: List(Resource). Please see argument details Currency Option
-        """
-        pulumi.set(__self__, "amount", amount)
-        pulumi.set(__self__, "currency", currency)
-        if currency_options is not None:
-            pulumi.set(__self__, "currency_options", currency_options)
-
-    @property
-    @pulumi.getter
-    def amount(self) -> int:
-        """
-        Int. A non-negative integer in cents representing how much to charge.
-        """
-        return pulumi.get(self, "amount")
-
-    @property
-    @pulumi.getter
-    def currency(self) -> str:
-        """
-        String. Three-letter ISO currency code, in lowercase - [supported currencies](https://stripe.com/docs/currencies).
-        """
-        return pulumi.get(self, "currency")
-
-    @property
-    @pulumi.getter(name="currencyOptions")
-    def currency_options(self) -> Optional[Sequence['outputs.ShippingRateFixedAmountCurrencyOption']]:
-        """
-        List(Resource). Please see argument details Currency Option
-        """
-        return pulumi.get(self, "currency_options")
-
-
-@pulumi.output_type
-class ShippingRateFixedAmountCurrencyOption(dict):
-    @staticmethod
-    def __key_warning(key: str):
-        suggest = None
-        if key == "taxBehavior":
-            suggest = "tax_behavior"
-
-        if suggest:
-            pulumi.log.warn(f"Key '{key}' not found in ShippingRateFixedAmountCurrencyOption. Access the value via the '{suggest}' property getter instead.")
-
-    def __getitem__(self, key: str) -> Any:
-        ShippingRateFixedAmountCurrencyOption.__key_warning(key)
-        return super().__getitem__(key)
-
-    def get(self, key: str, default = None) -> Any:
-        ShippingRateFixedAmountCurrencyOption.__key_warning(key)
-        return super().get(key, default)
-
-    def __init__(__self__, *,
-                 amount: int,
-                 currency: str,
-                 tax_behavior: Optional[str] = None):
-        """
-        :param int amount: Int. (Required) Int. A non-negative integer in cents representing how much to charge.
-        :param str currency: String. Three-letter ISO currency code, in lowercase - [supported currencies](https://stripe.com/docs/currencies).
-        :param str tax_behavior: Specifies whether the rate is considered inclusive of taxes or exclusive of taxes. One of inclusive, exclusive, or unspecified.
-        """
-        pulumi.set(__self__, "amount", amount)
-        pulumi.set(__self__, "currency", currency)
-        if tax_behavior is not None:
-            pulumi.set(__self__, "tax_behavior", tax_behavior)
-
-    @property
-    @pulumi.getter
-    def amount(self) -> int:
-        """
-        Int. (Required) Int. A non-negative integer in cents representing how much to charge.
-        """
-        return pulumi.get(self, "amount")
-
-    @property
-    @pulumi.getter
-    def currency(self) -> str:
-        """
-        String. Three-letter ISO currency code, in lowercase - [supported currencies](https://stripe.com/docs/currencies).
-        """
-        return pulumi.get(self, "currency")
-
-    @property
-    @pulumi.getter(name="taxBehavior")
-    def tax_behavior(self) -> Optional[str]:
-        """
-        Specifies whether the rate is considered inclusive of taxes or exclusive of taxes. One of inclusive, exclusive, or unspecified.
-        """
-        return pulumi.get(self, "tax_behavior")
-
-
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `pulumi_stripe-0.0.23/pulumi_stripe/portal_configuration.py` & `pulumi_stripe-0.0.8/pulumi_stripe/portal_configuration.py`

 * *Files 3% similar despite different names*

```diff
@@ -118,37 +118,33 @@
 @pulumi.input_type
 class _PortalConfigurationState:
     def __init__(__self__, *,
                  active: Optional[pulumi.Input[bool]] = None,
                  business_profile: Optional[pulumi.Input['PortalConfigurationBusinessProfileArgs']] = None,
                  default_return_url: Optional[pulumi.Input[str]] = None,
                  features: Optional[pulumi.Input['PortalConfigurationFeaturesArgs']] = None,
-                 is_default: Optional[pulumi.Input[bool]] = None,
                  login_page: Optional[pulumi.Input['PortalConfigurationLoginPageArgs']] = None,
                  metadata: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None):
         """
         Input properties used for looking up and filtering PortalConfiguration resources.
         :param pulumi.Input[bool] active: Bool. Whether the configuration is active and can be used to create portal sessions. (On create it is always set as `true`)
         :param pulumi.Input['PortalConfigurationBusinessProfileArgs'] business_profile: List(Resource). The business information shown to customers in the portal. More details in Business Profile section
         :param pulumi.Input[str] default_return_url: String. The default URL to redirect customers to when they click on the portal’s link to return to your website. This can be overriden when creating the session.
         :param pulumi.Input['PortalConfigurationFeaturesArgs'] features: List(Resource). Information about the features available in the portal. Feature section described in Feature section
-        :param pulumi.Input[bool] is_default: Bool. Whether the configuration is the default.
         :param pulumi.Input['PortalConfigurationLoginPageArgs'] login_page: List(Resource). The hosted login page for this configuration. See details in Login Page Section.
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] metadata: Map(String). Set of key-value pairs that you can attach to an object. This can be useful for storing additional information about the object in a structured format.
         """
         if active is not None:
             pulumi.set(__self__, "active", active)
         if business_profile is not None:
             pulumi.set(__self__, "business_profile", business_profile)
         if default_return_url is not None:
             pulumi.set(__self__, "default_return_url", default_return_url)
         if features is not None:
             pulumi.set(__self__, "features", features)
-        if is_default is not None:
-            pulumi.set(__self__, "is_default", is_default)
         if login_page is not None:
             pulumi.set(__self__, "login_page", login_page)
         if metadata is not None:
             pulumi.set(__self__, "metadata", metadata)
 
     @property
     @pulumi.getter
@@ -195,26 +191,14 @@
         return pulumi.get(self, "features")
 
     @features.setter
     def features(self, value: Optional[pulumi.Input['PortalConfigurationFeaturesArgs']]):
         pulumi.set(self, "features", value)
 
     @property
-    @pulumi.getter(name="isDefault")
-    def is_default(self) -> Optional[pulumi.Input[bool]]:
-        """
-        Bool. Whether the configuration is the default.
-        """
-        return pulumi.get(self, "is_default")
-
-    @is_default.setter
-    def is_default(self, value: Optional[pulumi.Input[bool]]):
-        pulumi.set(self, "is_default", value)
-
-    @property
     @pulumi.getter(name="loginPage")
     def login_page(self) -> Optional[pulumi.Input['PortalConfigurationLoginPageArgs']]:
         """
         List(Resource). The hosted login page for this configuration. See details in Login Page Section.
         """
         return pulumi.get(self, "login_page")
 
@@ -256,15 +240,14 @@
 
         > Removal of the Customer Portal isn't supported through the Stripe SDK. The best practice, which this provider follows,
         is to deactivate the Customer Portal by marking it as inactive on destroy, which indicates that resource is no longer
         available.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_stripe as stripe
 
         # A billing portal using all the available options
         portal_configuration = stripe.PortalConfiguration("portalConfiguration",
             business_profile=stripe.PortalConfigurationBusinessProfileArgs(
@@ -328,15 +311,14 @@
                     proration_behavior="none",
                 )],
             ),
             metadata={
                 "foo": "bar",
             })
         ```
-        <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[bool] active: Bool. Whether the configuration is active and can be used to create portal sessions. (On create it is always set as `true`)
         :param pulumi.Input[pulumi.InputType['PortalConfigurationBusinessProfileArgs']] business_profile: List(Resource). The business information shown to customers in the portal. More details in Business Profile section
         :param pulumi.Input[str] default_return_url: String. The default URL to redirect customers to when they click on the portal’s link to return to your website. This can be overriden when creating the session.
         :param pulumi.Input[pulumi.InputType['PortalConfigurationFeaturesArgs']] features: List(Resource). Information about the features available in the portal. Feature section described in Feature section
@@ -358,15 +340,14 @@
 
         > Removal of the Customer Portal isn't supported through the Stripe SDK. The best practice, which this provider follows,
         is to deactivate the Customer Portal by marking it as inactive on destroy, which indicates that resource is no longer
         available.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_stripe as stripe
 
         # A billing portal using all the available options
         portal_configuration = stripe.PortalConfiguration("portalConfiguration",
             business_profile=stripe.PortalConfigurationBusinessProfileArgs(
@@ -430,15 +411,14 @@
                     proration_behavior="none",
                 )],
             ),
             metadata={
                 "foo": "bar",
             })
         ```
-        <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
         :param PortalConfigurationArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
@@ -472,56 +452,52 @@
             __props__.__dict__["business_profile"] = business_profile
             __props__.__dict__["default_return_url"] = default_return_url
             if features is None and not opts.urn:
                 raise TypeError("Missing required property 'features'")
             __props__.__dict__["features"] = features
             __props__.__dict__["login_page"] = login_page
             __props__.__dict__["metadata"] = metadata
-            __props__.__dict__["is_default"] = None
         super(PortalConfiguration, __self__).__init__(
             'stripe:index/portalConfiguration:PortalConfiguration',
             resource_name,
             __props__,
             opts)
 
     @staticmethod
     def get(resource_name: str,
             id: pulumi.Input[str],
             opts: Optional[pulumi.ResourceOptions] = None,
             active: Optional[pulumi.Input[bool]] = None,
             business_profile: Optional[pulumi.Input[pulumi.InputType['PortalConfigurationBusinessProfileArgs']]] = None,
             default_return_url: Optional[pulumi.Input[str]] = None,
             features: Optional[pulumi.Input[pulumi.InputType['PortalConfigurationFeaturesArgs']]] = None,
-            is_default: Optional[pulumi.Input[bool]] = None,
             login_page: Optional[pulumi.Input[pulumi.InputType['PortalConfigurationLoginPageArgs']]] = None,
             metadata: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None) -> 'PortalConfiguration':
         """
         Get an existing PortalConfiguration resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[bool] active: Bool. Whether the configuration is active and can be used to create portal sessions. (On create it is always set as `true`)
         :param pulumi.Input[pulumi.InputType['PortalConfigurationBusinessProfileArgs']] business_profile: List(Resource). The business information shown to customers in the portal. More details in Business Profile section
         :param pulumi.Input[str] default_return_url: String. The default URL to redirect customers to when they click on the portal’s link to return to your website. This can be overriden when creating the session.
         :param pulumi.Input[pulumi.InputType['PortalConfigurationFeaturesArgs']] features: List(Resource). Information about the features available in the portal. Feature section described in Feature section
-        :param pulumi.Input[bool] is_default: Bool. Whether the configuration is the default.
         :param pulumi.Input[pulumi.InputType['PortalConfigurationLoginPageArgs']] login_page: List(Resource). The hosted login page for this configuration. See details in Login Page Section.
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] metadata: Map(String). Set of key-value pairs that you can attach to an object. This can be useful for storing additional information about the object in a structured format.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
         __props__ = _PortalConfigurationState.__new__(_PortalConfigurationState)
 
         __props__.__dict__["active"] = active
         __props__.__dict__["business_profile"] = business_profile
         __props__.__dict__["default_return_url"] = default_return_url
         __props__.__dict__["features"] = features
-        __props__.__dict__["is_default"] = is_default
         __props__.__dict__["login_page"] = login_page
         __props__.__dict__["metadata"] = metadata
         return PortalConfiguration(resource_name, opts=opts, __props__=__props__)
 
     @property
     @pulumi.getter
     def active(self) -> pulumi.Output[Optional[bool]]:
@@ -551,22 +527,14 @@
     def features(self) -> pulumi.Output['outputs.PortalConfigurationFeatures']:
         """
         List(Resource). Information about the features available in the portal. Feature section described in Feature section
         """
         return pulumi.get(self, "features")
 
     @property
-    @pulumi.getter(name="isDefault")
-    def is_default(self) -> pulumi.Output[bool]:
-        """
-        Bool. Whether the configuration is the default.
-        """
-        return pulumi.get(self, "is_default")
-
-    @property
     @pulumi.getter(name="loginPage")
     def login_page(self) -> pulumi.Output['outputs.PortalConfigurationLoginPage']:
         """
         List(Resource). The hosted login page for this configuration. See details in Login Page Section.
         """
         return pulumi.get(self, "login_page")
```

### Comparing `pulumi_stripe-0.0.23/pulumi_stripe/price.py` & `pulumi_stripe-0.0.8/pulumi_stripe/price.py`

 * *Files 0% similar despite different names*

```diff
@@ -659,20 +659,19 @@
 
         Different physical goods or levels of service should be represented by products, and pricing options should be
         represented by prices. This approach lets you change prices without having to change your provisioning scheme.
 
         For example, you might have a single "gold" product that has prices for $10/month, $100/year, and €9 once.
 
         > Removal of the price isn't supported through the Stripe SDK. The best practice, which this provider follows,
-        is to archive the price by marking it as inactive on destroy, which indicates that the price is no longer
+        is to archive the price by marking it as inactive on destroy, which indicates that the price is not longer
         available for purchase.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_stripe as stripe
 
         # basic price for the product
         price_price = stripe.Price("pricePrice",
             product=stripe_product["product"]["id"],
@@ -706,26 +705,24 @@
                 ),
                 stripe.PriceTierArgs(
                     up_to=100,
                     unit_amount=300,
                 ),
                 stripe.PriceTierArgs(
                     up_to=-1,
-                    unit_amount_decimal=100.5,
+                    unit_amount=100.5,
                 ),
             ],
             recurring=stripe.PriceRecurringArgs(
                 interval="week",
                 aggregate_usage="sum",
                 interval_count=2,
                 usage_type="metered",
             ))
         ```
-        <!--End PulumiCodeChooser -->
-
         ## Note on updating prices
 
         Once created, you can update the `active`, `metadata`, `nickname`, `lookup_key`, `tax_behaviour` (only if unspecified)
         and `transfer_lookup_key` attributes.
 
         Other attribute edits will trigger a destroy action (archival) and creation of a new price entry.
 
@@ -780,20 +777,19 @@
 
         Different physical goods or levels of service should be represented by products, and pricing options should be
         represented by prices. This approach lets you change prices without having to change your provisioning scheme.
 
         For example, you might have a single "gold" product that has prices for $10/month, $100/year, and €9 once.
 
         > Removal of the price isn't supported through the Stripe SDK. The best practice, which this provider follows,
-        is to archive the price by marking it as inactive on destroy, which indicates that the price is no longer
+        is to archive the price by marking it as inactive on destroy, which indicates that the price is not longer
         available for purchase.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_stripe as stripe
 
         # basic price for the product
         price_price = stripe.Price("pricePrice",
             product=stripe_product["product"]["id"],
@@ -827,26 +823,24 @@
                 ),
                 stripe.PriceTierArgs(
                     up_to=100,
                     unit_amount=300,
                 ),
                 stripe.PriceTierArgs(
                     up_to=-1,
-                    unit_amount_decimal=100.5,
+                    unit_amount=100.5,
                 ),
             ],
             recurring=stripe.PriceRecurringArgs(
                 interval="week",
                 aggregate_usage="sum",
                 interval_count=2,
                 usage_type="metered",
             ))
         ```
-        <!--End PulumiCodeChooser -->
-
         ## Note on updating prices
 
         Once created, you can update the `active`, `metadata`, `nickname`, `lookup_key`, `tax_behaviour` (only if unspecified)
         and `transfer_lookup_key` attributes.
 
         Other attribute edits will trigger a destroy action (archival) and creation of a new price entry.
 
@@ -1011,15 +1005,15 @@
         """
         Bool. Whether the price can be used for new purchases. Defaults to `true`.
         """
         return pulumi.get(self, "active")
 
     @property
     @pulumi.getter(name="billingScheme")
-    def billing_scheme(self) -> pulumi.Output[str]:
+    def billing_scheme(self) -> pulumi.Output[Optional[str]]:
         """
         String. Describes how to compute the price per period. Either `per_unit` or `tiered`
         . `per_unit` indicates that the fixed amount (specified in `unit_amount` or `unit_amount_decimal`) will be charged per
         unit in quantity (for prices with `usage_type=licensed`), or per unit of total usage (for prices
         with `usage_type=metered`). `tiered` indicates that the unit pricing will be computed using a tiering strategy as
         defined using the `tiers` and `tiers_mode` attributes.
         """
@@ -1140,23 +1134,23 @@
         String. One of `one_time` or `recurring` depending on whether the price is for a one-time purchase or a
         recurring (subscription) purchase.
         """
         return pulumi.get(self, "type")
 
     @property
     @pulumi.getter(name="unitAmount")
-    def unit_amount(self) -> pulumi.Output[int]:
+    def unit_amount(self) -> pulumi.Output[Optional[int]]:
         """
         Int. A positive integer in cents (or `-1` for a free
         price) representing how much to charge.
         """
         return pulumi.get(self, "unit_amount")
 
     @property
     @pulumi.getter(name="unitAmountDecimal")
-    def unit_amount_decimal(self) -> pulumi.Output[float]:
+    def unit_amount_decimal(self) -> pulumi.Output[Optional[float]]:
         """
         Float. Same as `unit_amount`, but accepts a decimal value in cents with at most 12
         decimal places. Only one of `unit_amount` and `unit_amount_decimal` can be set.
         """
         return pulumi.get(self, "unit_amount_decimal")
```

### Comparing `pulumi_stripe-0.0.23/pulumi_stripe/product.py` & `pulumi_stripe-0.0.8/pulumi_stripe/product.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,30 +12,28 @@
 __all__ = ['ProductArgs', 'Product']
 
 @pulumi.input_type
 class ProductArgs:
     def __init__(__self__, *,
                  active: Optional[pulumi.Input[bool]] = None,
                  description: Optional[pulumi.Input[str]] = None,
-                 features: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  images: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  metadata: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  package_dimensions: Optional[pulumi.Input[Mapping[str, pulumi.Input[float]]]] = None,
                  product_id: Optional[pulumi.Input[str]] = None,
                  shippable: Optional[pulumi.Input[bool]] = None,
                  statement_descriptor: Optional[pulumi.Input[str]] = None,
                  tax_code: Optional[pulumi.Input[str]] = None,
                  unit_label: Optional[pulumi.Input[str]] = None,
                  url: Optional[pulumi.Input[str]] = None):
         """
         The set of arguments for constructing a Product resource.
         :param pulumi.Input[bool] active: Bool. Whether the product is currently available for purchase. Defaults to `true`.
         :param pulumi.Input[str] description: String. The product’s description, meant to be displayable to the customer. Use this field to optionally store a long form explanation of the product being sold for your own rendering purposes.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] features: List(String). A list of up to 15 features for this product. These are displayed in pricing tables.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] images: List(String). A list of up to 8 URLs of images for this product, meant to be displayable to the customer.
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] metadata: Map(String). Set of key-value pairs that you can attach to an object. This can be useful for storing additional information about the object in a structured format.
         :param pulumi.Input[str] name: String. The product’s name, meant to be displayable to the customer. Whenever this product is sold via a subscription, name will show up on associated invoice line item descriptions.
         :param pulumi.Input[Mapping[str, pulumi.Input[float]]] package_dimensions: Map(Float). The dimensions of this product for shipping purposes. When used these fields are required: `height`,`length`,`width` and `weight`; the precision is 2 decimal places.
         :param pulumi.Input[str] product_id: String. The bespoke unique identifier for the object.
         :param pulumi.Input[bool] shippable: Bool. Whether this product is shipped (i.e., physical goods).
         :param pulumi.Input[str] statement_descriptor: String. An arbitrary string to be displayed on your customer’s credit card or bank statement. While most banks display this information consistently, some may display it incorrectly or not at all. This may be up to 22 characters. The statement description may not include `<`,` >`, `\\`, `"`, `’` characters, and will appear on your customer’s statement in capital letters. Non-ASCII characters are automatically stripped. It must contain at least one letter.
@@ -43,16 +41,14 @@
         :param pulumi.Input[str] unit_label: String. A label that represents units of this product in Stripe and on customers’ receipts and invoices. When set, this will be included in associated invoice line item descriptions.
         :param pulumi.Input[str] url: String. A URL of a publicly-accessible webpage for this product.
         """
         if active is not None:
             pulumi.set(__self__, "active", active)
         if description is not None:
             pulumi.set(__self__, "description", description)
-        if features is not None:
-            pulumi.set(__self__, "features", features)
         if images is not None:
             pulumi.set(__self__, "images", images)
         if metadata is not None:
             pulumi.set(__self__, "metadata", metadata)
         if name is not None:
             pulumi.set(__self__, "name", name)
         if package_dimensions is not None:
@@ -92,26 +88,14 @@
 
     @description.setter
     def description(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "description", value)
 
     @property
     @pulumi.getter
-    def features(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
-        """
-        List(String). A list of up to 15 features for this product. These are displayed in pricing tables.
-        """
-        return pulumi.get(self, "features")
-
-    @features.setter
-    def features(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
-        pulumi.set(self, "features", value)
-
-    @property
-    @pulumi.getter
     def images(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
         List(String). A list of up to 8 URLs of images for this product, meant to be displayable to the customer.
         """
         return pulumi.get(self, "images")
 
     @images.setter
@@ -228,30 +212,28 @@
 
 
 @pulumi.input_type
 class _ProductState:
     def __init__(__self__, *,
                  active: Optional[pulumi.Input[bool]] = None,
                  description: Optional[pulumi.Input[str]] = None,
-                 features: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  images: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  metadata: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  package_dimensions: Optional[pulumi.Input[Mapping[str, pulumi.Input[float]]]] = None,
                  product_id: Optional[pulumi.Input[str]] = None,
                  shippable: Optional[pulumi.Input[bool]] = None,
                  statement_descriptor: Optional[pulumi.Input[str]] = None,
                  tax_code: Optional[pulumi.Input[str]] = None,
                  unit_label: Optional[pulumi.Input[str]] = None,
                  url: Optional[pulumi.Input[str]] = None):
         """
         Input properties used for looking up and filtering Product resources.
         :param pulumi.Input[bool] active: Bool. Whether the product is currently available for purchase. Defaults to `true`.
         :param pulumi.Input[str] description: String. The product’s description, meant to be displayable to the customer. Use this field to optionally store a long form explanation of the product being sold for your own rendering purposes.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] features: List(String). A list of up to 15 features for this product. These are displayed in pricing tables.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] images: List(String). A list of up to 8 URLs of images for this product, meant to be displayable to the customer.
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] metadata: Map(String). Set of key-value pairs that you can attach to an object. This can be useful for storing additional information about the object in a structured format.
         :param pulumi.Input[str] name: String. The product’s name, meant to be displayable to the customer. Whenever this product is sold via a subscription, name will show up on associated invoice line item descriptions.
         :param pulumi.Input[Mapping[str, pulumi.Input[float]]] package_dimensions: Map(Float). The dimensions of this product for shipping purposes. When used these fields are required: `height`,`length`,`width` and `weight`; the precision is 2 decimal places.
         :param pulumi.Input[str] product_id: String. The bespoke unique identifier for the object.
         :param pulumi.Input[bool] shippable: Bool. Whether this product is shipped (i.e., physical goods).
         :param pulumi.Input[str] statement_descriptor: String. An arbitrary string to be displayed on your customer’s credit card or bank statement. While most banks display this information consistently, some may display it incorrectly or not at all. This may be up to 22 characters. The statement description may not include `<`,` >`, `\\`, `"`, `’` characters, and will appear on your customer’s statement in capital letters. Non-ASCII characters are automatically stripped. It must contain at least one letter.
@@ -259,16 +241,14 @@
         :param pulumi.Input[str] unit_label: String. A label that represents units of this product in Stripe and on customers’ receipts and invoices. When set, this will be included in associated invoice line item descriptions.
         :param pulumi.Input[str] url: String. A URL of a publicly-accessible webpage for this product.
         """
         if active is not None:
             pulumi.set(__self__, "active", active)
         if description is not None:
             pulumi.set(__self__, "description", description)
-        if features is not None:
-            pulumi.set(__self__, "features", features)
         if images is not None:
             pulumi.set(__self__, "images", images)
         if metadata is not None:
             pulumi.set(__self__, "metadata", metadata)
         if name is not None:
             pulumi.set(__self__, "name", name)
         if package_dimensions is not None:
@@ -308,26 +288,14 @@
 
     @description.setter
     def description(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "description", value)
 
     @property
     @pulumi.getter
-    def features(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
-        """
-        List(String). A list of up to 15 features for this product. These are displayed in pricing tables.
-        """
-        return pulumi.get(self, "features")
-
-    @features.setter
-    def features(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
-        pulumi.set(self, "features", value)
-
-    @property
-    @pulumi.getter
     def images(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
         List(String). A list of up to 8 URLs of images for this product, meant to be displayable to the customer.
         """
         return pulumi.get(self, "images")
 
     @images.setter
@@ -446,47 +414,48 @@
 class Product(pulumi.CustomResource):
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  active: Optional[pulumi.Input[bool]] = None,
                  description: Optional[pulumi.Input[str]] = None,
-                 features: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  images: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  metadata: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  package_dimensions: Optional[pulumi.Input[Mapping[str, pulumi.Input[float]]]] = None,
                  product_id: Optional[pulumi.Input[str]] = None,
                  shippable: Optional[pulumi.Input[bool]] = None,
                  statement_descriptor: Optional[pulumi.Input[str]] = None,
                  tax_code: Optional[pulumi.Input[str]] = None,
                  unit_label: Optional[pulumi.Input[str]] = None,
                  url: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
+        With this resource, you can create a product - [Stripe API product documentation](https://stripe.com/docs/api/products).
+
+        Products describe the specific goods or services you offer to your customers. For example,
+        you might offer a Standard and Premium version of your goods or service; each version would be a separate Product.
+
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_stripe as stripe
 
         # the most basic product
         product = stripe.Product("product",
             description="fantastic product",
             unit_label="piece",
             url="https://www.terraform.io")
         ```
-        <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[bool] active: Bool. Whether the product is currently available for purchase. Defaults to `true`.
         :param pulumi.Input[str] description: String. The product’s description, meant to be displayable to the customer. Use this field to optionally store a long form explanation of the product being sold for your own rendering purposes.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] features: List(String). A list of up to 15 features for this product. These are displayed in pricing tables.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] images: List(String). A list of up to 8 URLs of images for this product, meant to be displayable to the customer.
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] metadata: Map(String). Set of key-value pairs that you can attach to an object. This can be useful for storing additional information about the object in a structured format.
         :param pulumi.Input[str] name: String. The product’s name, meant to be displayable to the customer. Whenever this product is sold via a subscription, name will show up on associated invoice line item descriptions.
         :param pulumi.Input[Mapping[str, pulumi.Input[float]]] package_dimensions: Map(Float). The dimensions of this product for shipping purposes. When used these fields are required: `height`,`length`,`width` and `weight`; the precision is 2 decimal places.
         :param pulumi.Input[str] product_id: String. The bespoke unique identifier for the object.
         :param pulumi.Input[bool] shippable: Bool. Whether this product is shipped (i.e., physical goods).
         :param pulumi.Input[str] statement_descriptor: String. An arbitrary string to be displayed on your customer’s credit card or bank statement. While most banks display this information consistently, some may display it incorrectly or not at all. This may be up to 22 characters. The statement description may not include `<`,` >`, `\\`, `"`, `’` characters, and will appear on your customer’s statement in capital letters. Non-ASCII characters are automatically stripped. It must contain at least one letter.
@@ -497,28 +466,31 @@
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
                  args: Optional[ProductArgs] = None,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
+        With this resource, you can create a product - [Stripe API product documentation](https://stripe.com/docs/api/products).
+
+        Products describe the specific goods or services you offer to your customers. For example,
+        you might offer a Standard and Premium version of your goods or service; each version would be a separate Product.
+
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_stripe as stripe
 
         # the most basic product
         product = stripe.Product("product",
             description="fantastic product",
             unit_label="piece",
             url="https://www.terraform.io")
         ```
-        <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
         :param ProductArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
@@ -529,15 +501,14 @@
             __self__._internal_init(resource_name, *args, **kwargs)
 
     def _internal_init(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  active: Optional[pulumi.Input[bool]] = None,
                  description: Optional[pulumi.Input[str]] = None,
-                 features: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  images: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  metadata: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  package_dimensions: Optional[pulumi.Input[Mapping[str, pulumi.Input[float]]]] = None,
                  product_id: Optional[pulumi.Input[str]] = None,
                  shippable: Optional[pulumi.Input[bool]] = None,
                  statement_descriptor: Optional[pulumi.Input[str]] = None,
@@ -551,15 +522,14 @@
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = ProductArgs.__new__(ProductArgs)
 
             __props__.__dict__["active"] = active
             __props__.__dict__["description"] = description
-            __props__.__dict__["features"] = features
             __props__.__dict__["images"] = images
             __props__.__dict__["metadata"] = metadata
             __props__.__dict__["name"] = name
             __props__.__dict__["package_dimensions"] = package_dimensions
             __props__.__dict__["product_id"] = product_id
             __props__.__dict__["shippable"] = shippable
             __props__.__dict__["statement_descriptor"] = statement_descriptor
@@ -574,15 +544,14 @@
 
     @staticmethod
     def get(resource_name: str,
             id: pulumi.Input[str],
             opts: Optional[pulumi.ResourceOptions] = None,
             active: Optional[pulumi.Input[bool]] = None,
             description: Optional[pulumi.Input[str]] = None,
-            features: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
             images: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
             metadata: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
             name: Optional[pulumi.Input[str]] = None,
             package_dimensions: Optional[pulumi.Input[Mapping[str, pulumi.Input[float]]]] = None,
             product_id: Optional[pulumi.Input[str]] = None,
             shippable: Optional[pulumi.Input[bool]] = None,
             statement_descriptor: Optional[pulumi.Input[str]] = None,
@@ -594,15 +563,14 @@
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[bool] active: Bool. Whether the product is currently available for purchase. Defaults to `true`.
         :param pulumi.Input[str] description: String. The product’s description, meant to be displayable to the customer. Use this field to optionally store a long form explanation of the product being sold for your own rendering purposes.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] features: List(String). A list of up to 15 features for this product. These are displayed in pricing tables.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] images: List(String). A list of up to 8 URLs of images for this product, meant to be displayable to the customer.
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] metadata: Map(String). Set of key-value pairs that you can attach to an object. This can be useful for storing additional information about the object in a structured format.
         :param pulumi.Input[str] name: String. The product’s name, meant to be displayable to the customer. Whenever this product is sold via a subscription, name will show up on associated invoice line item descriptions.
         :param pulumi.Input[Mapping[str, pulumi.Input[float]]] package_dimensions: Map(Float). The dimensions of this product for shipping purposes. When used these fields are required: `height`,`length`,`width` and `weight`; the precision is 2 decimal places.
         :param pulumi.Input[str] product_id: String. The bespoke unique identifier for the object.
         :param pulumi.Input[bool] shippable: Bool. Whether this product is shipped (i.e., physical goods).
         :param pulumi.Input[str] statement_descriptor: String. An arbitrary string to be displayed on your customer’s credit card or bank statement. While most banks display this information consistently, some may display it incorrectly or not at all. This may be up to 22 characters. The statement description may not include `<`,` >`, `\\`, `"`, `’` characters, and will appear on your customer’s statement in capital letters. Non-ASCII characters are automatically stripped. It must contain at least one letter.
@@ -612,15 +580,14 @@
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
         __props__ = _ProductState.__new__(_ProductState)
 
         __props__.__dict__["active"] = active
         __props__.__dict__["description"] = description
-        __props__.__dict__["features"] = features
         __props__.__dict__["images"] = images
         __props__.__dict__["metadata"] = metadata
         __props__.__dict__["name"] = name
         __props__.__dict__["package_dimensions"] = package_dimensions
         __props__.__dict__["product_id"] = product_id
         __props__.__dict__["shippable"] = shippable
         __props__.__dict__["statement_descriptor"] = statement_descriptor
@@ -643,22 +610,14 @@
         """
         String. The product’s description, meant to be displayable to the customer. Use this field to optionally store a long form explanation of the product being sold for your own rendering purposes.
         """
         return pulumi.get(self, "description")
 
     @property
     @pulumi.getter
-    def features(self) -> pulumi.Output[Optional[Sequence[str]]]:
-        """
-        List(String). A list of up to 15 features for this product. These are displayed in pricing tables.
-        """
-        return pulumi.get(self, "features")
-
-    @property
-    @pulumi.getter
     def images(self) -> pulumi.Output[Optional[Sequence[str]]]:
         """
         List(String). A list of up to 8 URLs of images for this product, meant to be displayable to the customer.
         """
         return pulumi.get(self, "images")
 
     @property
```

### Comparing `pulumi_stripe-0.0.23/pulumi_stripe/promotion_code.py` & `pulumi_stripe-0.0.8/pulumi_stripe/promotion_code.py`

 * *Files 1% similar despite different names*

```diff
@@ -303,15 +303,14 @@
 
         A Promotion Code represents a customer-redeemable code for a coupon. It can be used to create multiple codes for a single coupon.
 
         > Removal of the promotion code isn't supported through the Stripe SDK.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_stripe as stripe
 
         # promotion code for the coupon
         code_promotion_code = stripe.PromotionCode("codePromotionCode",
             coupon=stripe_coupon["coupon"]["id"],
@@ -333,15 +332,14 @@
             code="FREE",
             restrictions=stripe.PromotionCodeRestrictionsArgs(
                 first_time_transaction=True,
                 minimum_amount=100,
                 minimum_amount_currency="aud",
             ))
         ```
-        <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[bool] active: Bool. Whether the promotion code is currently active. Defaults to `true`.
         :param pulumi.Input[str] code: String. The customer-facing code. Regardless of case, this code must be unique across all active promotion codes for a specific customer. If left blank, we will generate one automatically.
         :param pulumi.Input[str] coupon: String. The coupon for this promotion code.
         :param pulumi.Input[str] customer: String. The customer that this promotion code can be used by. If not set, the promotion code can be used by all customers.
@@ -361,15 +359,14 @@
 
         A Promotion Code represents a customer-redeemable code for a coupon. It can be used to create multiple codes for a single coupon.
 
         > Removal of the promotion code isn't supported through the Stripe SDK.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_stripe as stripe
 
         # promotion code for the coupon
         code_promotion_code = stripe.PromotionCode("codePromotionCode",
             coupon=stripe_coupon["coupon"]["id"],
@@ -391,15 +388,14 @@
             code="FREE",
             restrictions=stripe.PromotionCodeRestrictionsArgs(
                 first_time_transaction=True,
                 minimum_amount=100,
                 minimum_amount_currency="aud",
             ))
         ```
-        <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
         :param PromotionCodeArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
```

### Comparing `pulumi_stripe-0.0.23/pulumi_stripe/provider.py` & `pulumi_stripe-0.0.8/pulumi_stripe/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_stripe-0.0.23/pulumi_stripe/shipping_rate.py` & `pulumi_stripe-0.0.8/pulumi_stripe/tax_rate.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,265 +4,328 @@
 
 import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from . import _utilities
-from . import outputs
-from ._inputs import *
 
-__all__ = ['ShippingRateArgs', 'ShippingRate']
+__all__ = ['TaxRateArgs', 'TaxRate']
 
 @pulumi.input_type
-class ShippingRateArgs:
+class TaxRateArgs:
     def __init__(__self__, *,
                  display_name: pulumi.Input[str],
-                 fixed_amount: pulumi.Input['ShippingRateFixedAmountArgs'],
+                 inclusive: pulumi.Input[bool],
+                 percentage: pulumi.Input[float],
                  active: Optional[pulumi.Input[bool]] = None,
-                 delivery_estimates: Optional[pulumi.Input[Sequence[pulumi.Input['ShippingRateDeliveryEstimateArgs']]]] = None,
+                 country: Optional[pulumi.Input[str]] = None,
+                 description: Optional[pulumi.Input[str]] = None,
+                 jurisdiction: Optional[pulumi.Input[str]] = None,
                  metadata: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
-                 tax_behavior: Optional[pulumi.Input[str]] = None,
-                 tax_code: Optional[pulumi.Input[str]] = None,
-                 type: Optional[pulumi.Input[str]] = None):
-        """
-        The set of arguments for constructing a ShippingRate resource.
-        :param pulumi.Input[str] display_name: String. The name of the shipping rate, meant to be displayable to the customer. 
-               This will appear on CheckoutSessions.
-        :param pulumi.Input['ShippingRateFixedAmountArgs'] fixed_amount: List(Resource). Describes a fixed amount to charge for shipping. 
-               Must be present if type is `fixed_amount`. For details of individual arguments see Fixed Amount.
-        :param pulumi.Input[bool] active: Bool. Whether the shipping rate is active (can't be used when creating). Defaults to `true`.
-        :param pulumi.Input[Sequence[pulumi.Input['ShippingRateDeliveryEstimateArgs']]] delivery_estimates: List(Resource). The estimated range for how long shipping will take, 
-               meant to be displayable to the customer. This will appear on CheckoutSessions.
-               For details please see Delivery Estimate.
-        :param pulumi.Input[Mapping[str, pulumi.Input[str]]] metadata: Map(String). Set of key-value pairs that you can attach to an object. This can be useful for
-               storing additional information about the object in a structured format.
-        :param pulumi.Input[str] tax_behavior: Specifies whether the rate is considered inclusive of taxes or exclusive of taxes. One of inclusive, exclusive, or
-               unspecified.
-        :param pulumi.Input[str] tax_code: String. A tax code ID. The Shipping tax code is `txcd_92010001`.
-        :param pulumi.Input[str] type: String. The type of calculation to use on the shipping rate. Can only be `fixed_amount` for now.
+                 state: Optional[pulumi.Input[str]] = None,
+                 tax_type: Optional[pulumi.Input[str]] = None):
+        """
+        The set of arguments for constructing a TaxRate resource.
+        :param pulumi.Input[str] display_name: String. The display name of the tax rate, which will be shown to users.
+        :param pulumi.Input[bool] inclusive: Bool. This specifies if the tax rate is inclusive or exclusive.
+               * `percentage ` - (Required) Float. This represents the tax rate percent out of 100.
+        :param pulumi.Input[float] percentage: This represents the tax rate percent out of 100.
+        :param pulumi.Input[bool] active: Bool. Flag determining whether the tax rate is active or inactive (archived). Inactive tax rates cannot be used with new applications or Checkout Sessions, but will still work for subscriptions and invoices that already have it set.
+        :param pulumi.Input[str] country: String. Two-letter country code (ISO 3166-1 alpha-2).
+        :param pulumi.Input[str] description: String. An arbitrary string attached to the tax rate for your internal use only. It will not be visible to your customers.
+        :param pulumi.Input[str] jurisdiction: String. The jurisdiction for the tax rate. You can use this label field for tax reporting purposes. It also appears on your customer’s invoice.
+        :param pulumi.Input[Mapping[str, pulumi.Input[str]]] metadata: Map(String). Set of key-value pairs that you can attach to an object. This can be useful for storing additional information about the object in a structured format. Individual keys can be unset by posting an empty value to them. All keys can be unset by posting an empty value to metadata.
+        :param pulumi.Input[str] state: String. ISO 3166-2 subdivision code, without country prefix. For example, “NY” for New York, United States.
+        :param pulumi.Input[str] tax_type: String. The high-level tax type, such as vat or sales_tax.
         """
         pulumi.set(__self__, "display_name", display_name)
-        pulumi.set(__self__, "fixed_amount", fixed_amount)
+        pulumi.set(__self__, "inclusive", inclusive)
+        pulumi.set(__self__, "percentage", percentage)
         if active is not None:
             pulumi.set(__self__, "active", active)
-        if delivery_estimates is not None:
-            pulumi.set(__self__, "delivery_estimates", delivery_estimates)
+        if country is not None:
+            pulumi.set(__self__, "country", country)
+        if description is not None:
+            pulumi.set(__self__, "description", description)
+        if jurisdiction is not None:
+            pulumi.set(__self__, "jurisdiction", jurisdiction)
         if metadata is not None:
             pulumi.set(__self__, "metadata", metadata)
-        if tax_behavior is not None:
-            pulumi.set(__self__, "tax_behavior", tax_behavior)
-        if tax_code is not None:
-            pulumi.set(__self__, "tax_code", tax_code)
-        if type is not None:
-            pulumi.set(__self__, "type", type)
+        if state is not None:
+            pulumi.set(__self__, "state", state)
+        if tax_type is not None:
+            pulumi.set(__self__, "tax_type", tax_type)
 
     @property
     @pulumi.getter(name="displayName")
     def display_name(self) -> pulumi.Input[str]:
         """
-        String. The name of the shipping rate, meant to be displayable to the customer. 
-        This will appear on CheckoutSessions.
+        String. The display name of the tax rate, which will be shown to users.
         """
         return pulumi.get(self, "display_name")
 
     @display_name.setter
     def display_name(self, value: pulumi.Input[str]):
         pulumi.set(self, "display_name", value)
 
     @property
-    @pulumi.getter(name="fixedAmount")
-    def fixed_amount(self) -> pulumi.Input['ShippingRateFixedAmountArgs']:
+    @pulumi.getter
+    def inclusive(self) -> pulumi.Input[bool]:
         """
-        List(Resource). Describes a fixed amount to charge for shipping. 
-        Must be present if type is `fixed_amount`. For details of individual arguments see Fixed Amount.
+        Bool. This specifies if the tax rate is inclusive or exclusive.
+        * `percentage ` - (Required) Float. This represents the tax rate percent out of 100.
         """
-        return pulumi.get(self, "fixed_amount")
+        return pulumi.get(self, "inclusive")
 
-    @fixed_amount.setter
-    def fixed_amount(self, value: pulumi.Input['ShippingRateFixedAmountArgs']):
-        pulumi.set(self, "fixed_amount", value)
+    @inclusive.setter
+    def inclusive(self, value: pulumi.Input[bool]):
+        pulumi.set(self, "inclusive", value)
+
+    @property
+    @pulumi.getter
+    def percentage(self) -> pulumi.Input[float]:
+        """
+        This represents the tax rate percent out of 100.
+        """
+        return pulumi.get(self, "percentage")
+
+    @percentage.setter
+    def percentage(self, value: pulumi.Input[float]):
+        pulumi.set(self, "percentage", value)
 
     @property
     @pulumi.getter
     def active(self) -> Optional[pulumi.Input[bool]]:
         """
-        Bool. Whether the shipping rate is active (can't be used when creating). Defaults to `true`.
+        Bool. Flag determining whether the tax rate is active or inactive (archived). Inactive tax rates cannot be used with new applications or Checkout Sessions, but will still work for subscriptions and invoices that already have it set.
         """
         return pulumi.get(self, "active")
 
     @active.setter
     def active(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "active", value)
 
     @property
-    @pulumi.getter(name="deliveryEstimates")
-    def delivery_estimates(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['ShippingRateDeliveryEstimateArgs']]]]:
+    @pulumi.getter
+    def country(self) -> Optional[pulumi.Input[str]]:
         """
-        List(Resource). The estimated range for how long shipping will take, 
-        meant to be displayable to the customer. This will appear on CheckoutSessions.
-        For details please see Delivery Estimate.
-        """
-        return pulumi.get(self, "delivery_estimates")
-
-    @delivery_estimates.setter
-    def delivery_estimates(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['ShippingRateDeliveryEstimateArgs']]]]):
-        pulumi.set(self, "delivery_estimates", value)
+        String. Two-letter country code (ISO 3166-1 alpha-2).
+        """
+        return pulumi.get(self, "country")
+
+    @country.setter
+    def country(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "country", value)
 
     @property
     @pulumi.getter
-    def metadata(self) -> Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]:
+    def description(self) -> Optional[pulumi.Input[str]]:
         """
-        Map(String). Set of key-value pairs that you can attach to an object. This can be useful for
-        storing additional information about the object in a structured format.
+        String. An arbitrary string attached to the tax rate for your internal use only. It will not be visible to your customers.
         """
-        return pulumi.get(self, "metadata")
+        return pulumi.get(self, "description")
 
-    @metadata.setter
-    def metadata(self, value: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]):
-        pulumi.set(self, "metadata", value)
+    @description.setter
+    def description(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "description", value)
 
     @property
-    @pulumi.getter(name="taxBehavior")
-    def tax_behavior(self) -> Optional[pulumi.Input[str]]:
+    @pulumi.getter
+    def jurisdiction(self) -> Optional[pulumi.Input[str]]:
         """
-        Specifies whether the rate is considered inclusive of taxes or exclusive of taxes. One of inclusive, exclusive, or
-        unspecified.
+        String. The jurisdiction for the tax rate. You can use this label field for tax reporting purposes. It also appears on your customer’s invoice.
         """
-        return pulumi.get(self, "tax_behavior")
+        return pulumi.get(self, "jurisdiction")
 
-    @tax_behavior.setter
-    def tax_behavior(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "tax_behavior", value)
+    @jurisdiction.setter
+    def jurisdiction(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "jurisdiction", value)
 
     @property
-    @pulumi.getter(name="taxCode")
-    def tax_code(self) -> Optional[pulumi.Input[str]]:
+    @pulumi.getter
+    def metadata(self) -> Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]:
         """
-        String. A tax code ID. The Shipping tax code is `txcd_92010001`.
+        Map(String). Set of key-value pairs that you can attach to an object. This can be useful for storing additional information about the object in a structured format. Individual keys can be unset by posting an empty value to them. All keys can be unset by posting an empty value to metadata.
         """
-        return pulumi.get(self, "tax_code")
+        return pulumi.get(self, "metadata")
 
-    @tax_code.setter
-    def tax_code(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "tax_code", value)
+    @metadata.setter
+    def metadata(self, value: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]):
+        pulumi.set(self, "metadata", value)
 
     @property
     @pulumi.getter
-    def type(self) -> Optional[pulumi.Input[str]]:
+    def state(self) -> Optional[pulumi.Input[str]]:
+        """
+        String. ISO 3166-2 subdivision code, without country prefix. For example, “NY” for New York, United States.
+        """
+        return pulumi.get(self, "state")
+
+    @state.setter
+    def state(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "state", value)
+
+    @property
+    @pulumi.getter(name="taxType")
+    def tax_type(self) -> Optional[pulumi.Input[str]]:
         """
-        String. The type of calculation to use on the shipping rate. Can only be `fixed_amount` for now.
+        String. The high-level tax type, such as vat or sales_tax.
         """
-        return pulumi.get(self, "type")
+        return pulumi.get(self, "tax_type")
 
-    @type.setter
-    def type(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "type", value)
+    @tax_type.setter
+    def tax_type(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "tax_type", value)
 
 
 @pulumi.input_type
-class _ShippingRateState:
+class _TaxRateState:
     def __init__(__self__, *,
                  active: Optional[pulumi.Input[bool]] = None,
-                 delivery_estimates: Optional[pulumi.Input[Sequence[pulumi.Input['ShippingRateDeliveryEstimateArgs']]]] = None,
+                 country: Optional[pulumi.Input[str]] = None,
+                 created: Optional[pulumi.Input[int]] = None,
+                 description: Optional[pulumi.Input[str]] = None,
                  display_name: Optional[pulumi.Input[str]] = None,
-                 fixed_amount: Optional[pulumi.Input['ShippingRateFixedAmountArgs']] = None,
+                 inclusive: Optional[pulumi.Input[bool]] = None,
+                 jurisdiction: Optional[pulumi.Input[str]] = None,
                  livemode: Optional[pulumi.Input[bool]] = None,
                  metadata: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
-                 tax_behavior: Optional[pulumi.Input[str]] = None,
-                 tax_code: Optional[pulumi.Input[str]] = None,
-                 type: Optional[pulumi.Input[str]] = None):
-        """
-        Input properties used for looking up and filtering ShippingRate resources.
-        :param pulumi.Input[bool] active: Bool. Whether the shipping rate is active (can't be used when creating). Defaults to `true`.
-        :param pulumi.Input[Sequence[pulumi.Input['ShippingRateDeliveryEstimateArgs']]] delivery_estimates: List(Resource). The estimated range for how long shipping will take, 
-               meant to be displayable to the customer. This will appear on CheckoutSessions.
-               For details please see Delivery Estimate.
-        :param pulumi.Input[str] display_name: String. The name of the shipping rate, meant to be displayable to the customer. 
-               This will appear on CheckoutSessions.
-        :param pulumi.Input['ShippingRateFixedAmountArgs'] fixed_amount: List(Resource). Describes a fixed amount to charge for shipping. 
-               Must be present if type is `fixed_amount`. For details of individual arguments see Fixed Amount.
+                 object: Optional[pulumi.Input[str]] = None,
+                 percentage: Optional[pulumi.Input[float]] = None,
+                 state: Optional[pulumi.Input[str]] = None,
+                 tax_type: Optional[pulumi.Input[str]] = None):
+        """
+        Input properties used for looking up and filtering TaxRate resources.
+        :param pulumi.Input[bool] active: Bool. Flag determining whether the tax rate is active or inactive (archived). Inactive tax rates cannot be used with new applications or Checkout Sessions, but will still work for subscriptions and invoices that already have it set.
+        :param pulumi.Input[str] country: String. Two-letter country code (ISO 3166-1 alpha-2).
+        :param pulumi.Input[int] created: Int. Time at which the object was created. Measured in seconds since the Unix epoch.
+        :param pulumi.Input[str] description: String. An arbitrary string attached to the tax rate for your internal use only. It will not be visible to your customers.
+        :param pulumi.Input[str] display_name: String. The display name of the tax rate, which will be shown to users.
+        :param pulumi.Input[bool] inclusive: Bool. This specifies if the tax rate is inclusive or exclusive.
+               * `percentage ` - (Required) Float. This represents the tax rate percent out of 100.
+        :param pulumi.Input[str] jurisdiction: String. The jurisdiction for the tax rate. You can use this label field for tax reporting purposes. It also appears on your customer’s invoice.
         :param pulumi.Input[bool] livemode: Bool. Has the value true if the object exists in live mode or the value false if the object exists in test mode.
-        :param pulumi.Input[Mapping[str, pulumi.Input[str]]] metadata: Map(String). Set of key-value pairs that you can attach to an object. This can be useful for
-               storing additional information about the object in a structured format.
-        :param pulumi.Input[str] tax_behavior: Specifies whether the rate is considered inclusive of taxes or exclusive of taxes. One of inclusive, exclusive, or
-               unspecified.
-        :param pulumi.Input[str] tax_code: String. A tax code ID. The Shipping tax code is `txcd_92010001`.
-        :param pulumi.Input[str] type: String. The type of calculation to use on the shipping rate. Can only be `fixed_amount` for now.
+        :param pulumi.Input[Mapping[str, pulumi.Input[str]]] metadata: Map(String). Set of key-value pairs that you can attach to an object. This can be useful for storing additional information about the object in a structured format. Individual keys can be unset by posting an empty value to them. All keys can be unset by posting an empty value to metadata.
+        :param pulumi.Input[str] object: String. String representing the object’s type. Objects of the same type share the same value.
+        :param pulumi.Input[float] percentage: This represents the tax rate percent out of 100.
+        :param pulumi.Input[str] state: String. ISO 3166-2 subdivision code, without country prefix. For example, “NY” for New York, United States.
+        :param pulumi.Input[str] tax_type: String. The high-level tax type, such as vat or sales_tax.
         """
         if active is not None:
             pulumi.set(__self__, "active", active)
-        if delivery_estimates is not None:
-            pulumi.set(__self__, "delivery_estimates", delivery_estimates)
+        if country is not None:
+            pulumi.set(__self__, "country", country)
+        if created is not None:
+            pulumi.set(__self__, "created", created)
+        if description is not None:
+            pulumi.set(__self__, "description", description)
         if display_name is not None:
             pulumi.set(__self__, "display_name", display_name)
-        if fixed_amount is not None:
-            pulumi.set(__self__, "fixed_amount", fixed_amount)
+        if inclusive is not None:
+            pulumi.set(__self__, "inclusive", inclusive)
+        if jurisdiction is not None:
+            pulumi.set(__self__, "jurisdiction", jurisdiction)
         if livemode is not None:
             pulumi.set(__self__, "livemode", livemode)
         if metadata is not None:
             pulumi.set(__self__, "metadata", metadata)
-        if tax_behavior is not None:
-            pulumi.set(__self__, "tax_behavior", tax_behavior)
-        if tax_code is not None:
-            pulumi.set(__self__, "tax_code", tax_code)
-        if type is not None:
-            pulumi.set(__self__, "type", type)
+        if object is not None:
+            pulumi.set(__self__, "object", object)
+        if percentage is not None:
+            pulumi.set(__self__, "percentage", percentage)
+        if state is not None:
+            pulumi.set(__self__, "state", state)
+        if tax_type is not None:
+            pulumi.set(__self__, "tax_type", tax_type)
 
     @property
     @pulumi.getter
     def active(self) -> Optional[pulumi.Input[bool]]:
         """
-        Bool. Whether the shipping rate is active (can't be used when creating). Defaults to `true`.
+        Bool. Flag determining whether the tax rate is active or inactive (archived). Inactive tax rates cannot be used with new applications or Checkout Sessions, but will still work for subscriptions and invoices that already have it set.
         """
         return pulumi.get(self, "active")
 
     @active.setter
     def active(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "active", value)
 
     @property
-    @pulumi.getter(name="deliveryEstimates")
-    def delivery_estimates(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['ShippingRateDeliveryEstimateArgs']]]]:
+    @pulumi.getter
+    def country(self) -> Optional[pulumi.Input[str]]:
+        """
+        String. Two-letter country code (ISO 3166-1 alpha-2).
+        """
+        return pulumi.get(self, "country")
+
+    @country.setter
+    def country(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "country", value)
+
+    @property
+    @pulumi.getter
+    def created(self) -> Optional[pulumi.Input[int]]:
+        """
+        Int. Time at which the object was created. Measured in seconds since the Unix epoch.
+        """
+        return pulumi.get(self, "created")
+
+    @created.setter
+    def created(self, value: Optional[pulumi.Input[int]]):
+        pulumi.set(self, "created", value)
+
+    @property
+    @pulumi.getter
+    def description(self) -> Optional[pulumi.Input[str]]:
         """
-        List(Resource). The estimated range for how long shipping will take, 
-        meant to be displayable to the customer. This will appear on CheckoutSessions.
-        For details please see Delivery Estimate.
-        """
-        return pulumi.get(self, "delivery_estimates")
-
-    @delivery_estimates.setter
-    def delivery_estimates(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['ShippingRateDeliveryEstimateArgs']]]]):
-        pulumi.set(self, "delivery_estimates", value)
+        String. An arbitrary string attached to the tax rate for your internal use only. It will not be visible to your customers.
+        """
+        return pulumi.get(self, "description")
+
+    @description.setter
+    def description(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "description", value)
 
     @property
     @pulumi.getter(name="displayName")
     def display_name(self) -> Optional[pulumi.Input[str]]:
         """
-        String. The name of the shipping rate, meant to be displayable to the customer. 
-        This will appear on CheckoutSessions.
+        String. The display name of the tax rate, which will be shown to users.
         """
         return pulumi.get(self, "display_name")
 
     @display_name.setter
     def display_name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "display_name", value)
 
     @property
-    @pulumi.getter(name="fixedAmount")
-    def fixed_amount(self) -> Optional[pulumi.Input['ShippingRateFixedAmountArgs']]:
+    @pulumi.getter
+    def inclusive(self) -> Optional[pulumi.Input[bool]]:
         """
-        List(Resource). Describes a fixed amount to charge for shipping. 
-        Must be present if type is `fixed_amount`. For details of individual arguments see Fixed Amount.
+        Bool. This specifies if the tax rate is inclusive or exclusive.
+        * `percentage ` - (Required) Float. This represents the tax rate percent out of 100.
         """
-        return pulumi.get(self, "fixed_amount")
+        return pulumi.get(self, "inclusive")
 
-    @fixed_amount.setter
-    def fixed_amount(self, value: Optional[pulumi.Input['ShippingRateFixedAmountArgs']]):
-        pulumi.set(self, "fixed_amount", value)
+    @inclusive.setter
+    def inclusive(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "inclusive", value)
+
+    @property
+    @pulumi.getter
+    def jurisdiction(self) -> Optional[pulumi.Input[str]]:
+        """
+        String. The jurisdiction for the tax rate. You can use this label field for tax reporting purposes. It also appears on your customer’s invoice.
+        """
+        return pulumi.get(self, "jurisdiction")
+
+    @jurisdiction.setter
+    def jurisdiction(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "jurisdiction", value)
 
     @property
     @pulumi.getter
     def livemode(self) -> Optional[pulumi.Input[bool]]:
         """
         Bool. Has the value true if the object exists in live mode or the value false if the object exists in test mode.
         """
@@ -272,383 +335,370 @@
     def livemode(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "livemode", value)
 
     @property
     @pulumi.getter
     def metadata(self) -> Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]:
         """
-        Map(String). Set of key-value pairs that you can attach to an object. This can be useful for
-        storing additional information about the object in a structured format.
+        Map(String). Set of key-value pairs that you can attach to an object. This can be useful for storing additional information about the object in a structured format. Individual keys can be unset by posting an empty value to them. All keys can be unset by posting an empty value to metadata.
         """
         return pulumi.get(self, "metadata")
 
     @metadata.setter
     def metadata(self, value: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]):
         pulumi.set(self, "metadata", value)
 
     @property
-    @pulumi.getter(name="taxBehavior")
-    def tax_behavior(self) -> Optional[pulumi.Input[str]]:
+    @pulumi.getter
+    def object(self) -> Optional[pulumi.Input[str]]:
         """
-        Specifies whether the rate is considered inclusive of taxes or exclusive of taxes. One of inclusive, exclusive, or
-        unspecified.
+        String. String representing the object’s type. Objects of the same type share the same value.
         """
-        return pulumi.get(self, "tax_behavior")
+        return pulumi.get(self, "object")
 
-    @tax_behavior.setter
-    def tax_behavior(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "tax_behavior", value)
+    @object.setter
+    def object(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "object", value)
 
     @property
-    @pulumi.getter(name="taxCode")
-    def tax_code(self) -> Optional[pulumi.Input[str]]:
+    @pulumi.getter
+    def percentage(self) -> Optional[pulumi.Input[float]]:
         """
-        String. A tax code ID. The Shipping tax code is `txcd_92010001`.
+        This represents the tax rate percent out of 100.
         """
-        return pulumi.get(self, "tax_code")
+        return pulumi.get(self, "percentage")
 
-    @tax_code.setter
-    def tax_code(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "tax_code", value)
+    @percentage.setter
+    def percentage(self, value: Optional[pulumi.Input[float]]):
+        pulumi.set(self, "percentage", value)
 
     @property
     @pulumi.getter
-    def type(self) -> Optional[pulumi.Input[str]]:
+    def state(self) -> Optional[pulumi.Input[str]]:
         """
-        String. The type of calculation to use on the shipping rate. Can only be `fixed_amount` for now.
+        String. ISO 3166-2 subdivision code, without country prefix. For example, “NY” for New York, United States.
         """
-        return pulumi.get(self, "type")
+        return pulumi.get(self, "state")
 
-    @type.setter
-    def type(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "type", value)
+    @state.setter
+    def state(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "state", value)
+
+    @property
+    @pulumi.getter(name="taxType")
+    def tax_type(self) -> Optional[pulumi.Input[str]]:
+        """
+        String. The high-level tax type, such as vat or sales_tax.
+        """
+        return pulumi.get(self, "tax_type")
+
+    @tax_type.setter
+    def tax_type(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "tax_type", value)
 
 
-class ShippingRate(pulumi.CustomResource):
+class TaxRate(pulumi.CustomResource):
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  active: Optional[pulumi.Input[bool]] = None,
-                 delivery_estimates: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ShippingRateDeliveryEstimateArgs']]]]] = None,
+                 country: Optional[pulumi.Input[str]] = None,
+                 description: Optional[pulumi.Input[str]] = None,
                  display_name: Optional[pulumi.Input[str]] = None,
-                 fixed_amount: Optional[pulumi.Input[pulumi.InputType['ShippingRateFixedAmountArgs']]] = None,
+                 inclusive: Optional[pulumi.Input[bool]] = None,
+                 jurisdiction: Optional[pulumi.Input[str]] = None,
                  metadata: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
-                 tax_behavior: Optional[pulumi.Input[str]] = None,
-                 tax_code: Optional[pulumi.Input[str]] = None,
-                 type: Optional[pulumi.Input[str]] = None,
+                 percentage: Optional[pulumi.Input[float]] = None,
+                 state: Optional[pulumi.Input[str]] = None,
+                 tax_type: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
-        With this resource, you can create a shipping rate - [Stripe API shipping rate documentation](https://stripe.com/docs/api/shipping_rates).
+        With this resource, you can create a tax rate - [Stripe API tax rate  documentation](https://stripe.com/docs/api/tax_rates).
 
-        Shipping rates let you display various shipping options—like standard, express, and overnight—with more accurate delivery estimates.
-        Charge your customer for shipping using different Stripe products, some of which require coding.
-
-        > Removal of the shipping rate isn't supported through the Stripe SDK. The best practice, which this provider follows,
-        is to archive the shipping rate by marking it as inactive on destroy, which indicates that the shipping rate is no longer
-        available.
+        Tax rates can be applied to invoices, subscriptions and Checkout Sessions to collect tax.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_stripe as stripe
 
-        # shipping rate with delivery estimate
-        shipping_rate = stripe.ShippingRate("shippingRate",
-            delivery_estimates=[stripe.ShippingRateDeliveryEstimateArgs(
-                maximum=stripe.ShippingRateDeliveryEstimateMaximumArgs(
-                    unit="day",
-                    value=4,
-                ),
-                minimum=stripe.ShippingRateDeliveryEstimateMinimumArgs(
-                    unit="hour",
-                    value=24,
-                ),
-            )],
-            display_name="shipping rate",
-            fixed_amount=stripe.ShippingRateFixedAmountArgs(
-                amount=1000,
-                currency="aud",
-            ))
-        # shipping rate with currency options
-        # !!! Currency options have to be sorted alphabetically 
-        # !!! by the currency field
-        shipping = stripe.ShippingRate("shipping",
-            display_name="shipping rate",
-            fixed_amount=stripe.ShippingRateFixedAmountArgs(
-                amount=1000,
-                currency="aud",
-                currency_options=[
-                    stripe.ShippingRateFixedAmountCurrencyOptionArgs(
-                        amount=350,
-                        currency="eur",
-                    ),
-                    stripe.ShippingRateFixedAmountCurrencyOptionArgs(
-                        amount=500,
-                        currency="usd",
-                    ),
-                ],
-            ))
+        tax_rate = stripe.TaxRate("taxRate",
+            active=True,
+            country="AU",
+            description="GST Australia",
+            display_name="GST",
+            inclusive=True,
+            jurisdiction="AU",
+            metadata={},
+            percentage=10,
+            state="",
+            tax_type="")
         ```
-        <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
-        :param pulumi.Input[bool] active: Bool. Whether the shipping rate is active (can't be used when creating). Defaults to `true`.
-        :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ShippingRateDeliveryEstimateArgs']]]] delivery_estimates: List(Resource). The estimated range for how long shipping will take, 
-               meant to be displayable to the customer. This will appear on CheckoutSessions.
-               For details please see Delivery Estimate.
-        :param pulumi.Input[str] display_name: String. The name of the shipping rate, meant to be displayable to the customer. 
-               This will appear on CheckoutSessions.
-        :param pulumi.Input[pulumi.InputType['ShippingRateFixedAmountArgs']] fixed_amount: List(Resource). Describes a fixed amount to charge for shipping. 
-               Must be present if type is `fixed_amount`. For details of individual arguments see Fixed Amount.
-        :param pulumi.Input[Mapping[str, pulumi.Input[str]]] metadata: Map(String). Set of key-value pairs that you can attach to an object. This can be useful for
-               storing additional information about the object in a structured format.
-        :param pulumi.Input[str] tax_behavior: Specifies whether the rate is considered inclusive of taxes or exclusive of taxes. One of inclusive, exclusive, or
-               unspecified.
-        :param pulumi.Input[str] tax_code: String. A tax code ID. The Shipping tax code is `txcd_92010001`.
-        :param pulumi.Input[str] type: String. The type of calculation to use on the shipping rate. Can only be `fixed_amount` for now.
+        :param pulumi.Input[bool] active: Bool. Flag determining whether the tax rate is active or inactive (archived). Inactive tax rates cannot be used with new applications or Checkout Sessions, but will still work for subscriptions and invoices that already have it set.
+        :param pulumi.Input[str] country: String. Two-letter country code (ISO 3166-1 alpha-2).
+        :param pulumi.Input[str] description: String. An arbitrary string attached to the tax rate for your internal use only. It will not be visible to your customers.
+        :param pulumi.Input[str] display_name: String. The display name of the tax rate, which will be shown to users.
+        :param pulumi.Input[bool] inclusive: Bool. This specifies if the tax rate is inclusive or exclusive.
+               * `percentage ` - (Required) Float. This represents the tax rate percent out of 100.
+        :param pulumi.Input[str] jurisdiction: String. The jurisdiction for the tax rate. You can use this label field for tax reporting purposes. It also appears on your customer’s invoice.
+        :param pulumi.Input[Mapping[str, pulumi.Input[str]]] metadata: Map(String). Set of key-value pairs that you can attach to an object. This can be useful for storing additional information about the object in a structured format. Individual keys can be unset by posting an empty value to them. All keys can be unset by posting an empty value to metadata.
+        :param pulumi.Input[float] percentage: This represents the tax rate percent out of 100.
+        :param pulumi.Input[str] state: String. ISO 3166-2 subdivision code, without country prefix. For example, “NY” for New York, United States.
+        :param pulumi.Input[str] tax_type: String. The high-level tax type, such as vat or sales_tax.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
-                 args: ShippingRateArgs,
+                 args: TaxRateArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
-        With this resource, you can create a shipping rate - [Stripe API shipping rate documentation](https://stripe.com/docs/api/shipping_rates).
-
-        Shipping rates let you display various shipping options—like standard, express, and overnight—with more accurate delivery estimates.
-        Charge your customer for shipping using different Stripe products, some of which require coding.
+        With this resource, you can create a tax rate - [Stripe API tax rate  documentation](https://stripe.com/docs/api/tax_rates).
 
-        > Removal of the shipping rate isn't supported through the Stripe SDK. The best practice, which this provider follows,
-        is to archive the shipping rate by marking it as inactive on destroy, which indicates that the shipping rate is no longer
-        available.
+        Tax rates can be applied to invoices, subscriptions and Checkout Sessions to collect tax.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_stripe as stripe
 
-        # shipping rate with delivery estimate
-        shipping_rate = stripe.ShippingRate("shippingRate",
-            delivery_estimates=[stripe.ShippingRateDeliveryEstimateArgs(
-                maximum=stripe.ShippingRateDeliveryEstimateMaximumArgs(
-                    unit="day",
-                    value=4,
-                ),
-                minimum=stripe.ShippingRateDeliveryEstimateMinimumArgs(
-                    unit="hour",
-                    value=24,
-                ),
-            )],
-            display_name="shipping rate",
-            fixed_amount=stripe.ShippingRateFixedAmountArgs(
-                amount=1000,
-                currency="aud",
-            ))
-        # shipping rate with currency options
-        # !!! Currency options have to be sorted alphabetically 
-        # !!! by the currency field
-        shipping = stripe.ShippingRate("shipping",
-            display_name="shipping rate",
-            fixed_amount=stripe.ShippingRateFixedAmountArgs(
-                amount=1000,
-                currency="aud",
-                currency_options=[
-                    stripe.ShippingRateFixedAmountCurrencyOptionArgs(
-                        amount=350,
-                        currency="eur",
-                    ),
-                    stripe.ShippingRateFixedAmountCurrencyOptionArgs(
-                        amount=500,
-                        currency="usd",
-                    ),
-                ],
-            ))
+        tax_rate = stripe.TaxRate("taxRate",
+            active=True,
+            country="AU",
+            description="GST Australia",
+            display_name="GST",
+            inclusive=True,
+            jurisdiction="AU",
+            metadata={},
+            percentage=10,
+            state="",
+            tax_type="")
         ```
-        <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
-        :param ShippingRateArgs args: The arguments to use to populate this resource's properties.
+        :param TaxRateArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
-        resource_args, opts = _utilities.get_resource_args_opts(ShippingRateArgs, pulumi.ResourceOptions, *args, **kwargs)
+        resource_args, opts = _utilities.get_resource_args_opts(TaxRateArgs, pulumi.ResourceOptions, *args, **kwargs)
         if resource_args is not None:
             __self__._internal_init(resource_name, opts, **resource_args.__dict__)
         else:
             __self__._internal_init(resource_name, *args, **kwargs)
 
     def _internal_init(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  active: Optional[pulumi.Input[bool]] = None,
-                 delivery_estimates: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ShippingRateDeliveryEstimateArgs']]]]] = None,
+                 country: Optional[pulumi.Input[str]] = None,
+                 description: Optional[pulumi.Input[str]] = None,
                  display_name: Optional[pulumi.Input[str]] = None,
-                 fixed_amount: Optional[pulumi.Input[pulumi.InputType['ShippingRateFixedAmountArgs']]] = None,
+                 inclusive: Optional[pulumi.Input[bool]] = None,
+                 jurisdiction: Optional[pulumi.Input[str]] = None,
                  metadata: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
-                 tax_behavior: Optional[pulumi.Input[str]] = None,
-                 tax_code: Optional[pulumi.Input[str]] = None,
-                 type: Optional[pulumi.Input[str]] = None,
+                 percentage: Optional[pulumi.Input[float]] = None,
+                 state: Optional[pulumi.Input[str]] = None,
+                 tax_type: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
-            __props__ = ShippingRateArgs.__new__(ShippingRateArgs)
+            __props__ = TaxRateArgs.__new__(TaxRateArgs)
 
             __props__.__dict__["active"] = active
-            __props__.__dict__["delivery_estimates"] = delivery_estimates
+            __props__.__dict__["country"] = country
+            __props__.__dict__["description"] = description
             if display_name is None and not opts.urn:
                 raise TypeError("Missing required property 'display_name'")
             __props__.__dict__["display_name"] = display_name
-            if fixed_amount is None and not opts.urn:
-                raise TypeError("Missing required property 'fixed_amount'")
-            __props__.__dict__["fixed_amount"] = fixed_amount
+            if inclusive is None and not opts.urn:
+                raise TypeError("Missing required property 'inclusive'")
+            __props__.__dict__["inclusive"] = inclusive
+            __props__.__dict__["jurisdiction"] = jurisdiction
             __props__.__dict__["metadata"] = metadata
-            __props__.__dict__["tax_behavior"] = tax_behavior
-            __props__.__dict__["tax_code"] = tax_code
-            __props__.__dict__["type"] = type
+            if percentage is None and not opts.urn:
+                raise TypeError("Missing required property 'percentage'")
+            __props__.__dict__["percentage"] = percentage
+            __props__.__dict__["state"] = state
+            __props__.__dict__["tax_type"] = tax_type
+            __props__.__dict__["created"] = None
             __props__.__dict__["livemode"] = None
-        super(ShippingRate, __self__).__init__(
-            'stripe:index/shippingRate:ShippingRate',
+            __props__.__dict__["object"] = None
+        super(TaxRate, __self__).__init__(
+            'stripe:index/taxRate:TaxRate',
             resource_name,
             __props__,
             opts)
 
     @staticmethod
     def get(resource_name: str,
             id: pulumi.Input[str],
             opts: Optional[pulumi.ResourceOptions] = None,
             active: Optional[pulumi.Input[bool]] = None,
-            delivery_estimates: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ShippingRateDeliveryEstimateArgs']]]]] = None,
+            country: Optional[pulumi.Input[str]] = None,
+            created: Optional[pulumi.Input[int]] = None,
+            description: Optional[pulumi.Input[str]] = None,
             display_name: Optional[pulumi.Input[str]] = None,
-            fixed_amount: Optional[pulumi.Input[pulumi.InputType['ShippingRateFixedAmountArgs']]] = None,
+            inclusive: Optional[pulumi.Input[bool]] = None,
+            jurisdiction: Optional[pulumi.Input[str]] = None,
             livemode: Optional[pulumi.Input[bool]] = None,
             metadata: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
-            tax_behavior: Optional[pulumi.Input[str]] = None,
-            tax_code: Optional[pulumi.Input[str]] = None,
-            type: Optional[pulumi.Input[str]] = None) -> 'ShippingRate':
+            object: Optional[pulumi.Input[str]] = None,
+            percentage: Optional[pulumi.Input[float]] = None,
+            state: Optional[pulumi.Input[str]] = None,
+            tax_type: Optional[pulumi.Input[str]] = None) -> 'TaxRate':
         """
-        Get an existing ShippingRate resource's state with the given name, id, and optional extra
+        Get an existing TaxRate resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
-        :param pulumi.Input[bool] active: Bool. Whether the shipping rate is active (can't be used when creating). Defaults to `true`.
-        :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ShippingRateDeliveryEstimateArgs']]]] delivery_estimates: List(Resource). The estimated range for how long shipping will take, 
-               meant to be displayable to the customer. This will appear on CheckoutSessions.
-               For details please see Delivery Estimate.
-        :param pulumi.Input[str] display_name: String. The name of the shipping rate, meant to be displayable to the customer. 
-               This will appear on CheckoutSessions.
-        :param pulumi.Input[pulumi.InputType['ShippingRateFixedAmountArgs']] fixed_amount: List(Resource). Describes a fixed amount to charge for shipping. 
-               Must be present if type is `fixed_amount`. For details of individual arguments see Fixed Amount.
+        :param pulumi.Input[bool] active: Bool. Flag determining whether the tax rate is active or inactive (archived). Inactive tax rates cannot be used with new applications or Checkout Sessions, but will still work for subscriptions and invoices that already have it set.
+        :param pulumi.Input[str] country: String. Two-letter country code (ISO 3166-1 alpha-2).
+        :param pulumi.Input[int] created: Int. Time at which the object was created. Measured in seconds since the Unix epoch.
+        :param pulumi.Input[str] description: String. An arbitrary string attached to the tax rate for your internal use only. It will not be visible to your customers.
+        :param pulumi.Input[str] display_name: String. The display name of the tax rate, which will be shown to users.
+        :param pulumi.Input[bool] inclusive: Bool. This specifies if the tax rate is inclusive or exclusive.
+               * `percentage ` - (Required) Float. This represents the tax rate percent out of 100.
+        :param pulumi.Input[str] jurisdiction: String. The jurisdiction for the tax rate. You can use this label field for tax reporting purposes. It also appears on your customer’s invoice.
         :param pulumi.Input[bool] livemode: Bool. Has the value true if the object exists in live mode or the value false if the object exists in test mode.
-        :param pulumi.Input[Mapping[str, pulumi.Input[str]]] metadata: Map(String). Set of key-value pairs that you can attach to an object. This can be useful for
-               storing additional information about the object in a structured format.
-        :param pulumi.Input[str] tax_behavior: Specifies whether the rate is considered inclusive of taxes or exclusive of taxes. One of inclusive, exclusive, or
-               unspecified.
-        :param pulumi.Input[str] tax_code: String. A tax code ID. The Shipping tax code is `txcd_92010001`.
-        :param pulumi.Input[str] type: String. The type of calculation to use on the shipping rate. Can only be `fixed_amount` for now.
+        :param pulumi.Input[Mapping[str, pulumi.Input[str]]] metadata: Map(String). Set of key-value pairs that you can attach to an object. This can be useful for storing additional information about the object in a structured format. Individual keys can be unset by posting an empty value to them. All keys can be unset by posting an empty value to metadata.
+        :param pulumi.Input[str] object: String. String representing the object’s type. Objects of the same type share the same value.
+        :param pulumi.Input[float] percentage: This represents the tax rate percent out of 100.
+        :param pulumi.Input[str] state: String. ISO 3166-2 subdivision code, without country prefix. For example, “NY” for New York, United States.
+        :param pulumi.Input[str] tax_type: String. The high-level tax type, such as vat or sales_tax.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
-        __props__ = _ShippingRateState.__new__(_ShippingRateState)
+        __props__ = _TaxRateState.__new__(_TaxRateState)
 
         __props__.__dict__["active"] = active
-        __props__.__dict__["delivery_estimates"] = delivery_estimates
+        __props__.__dict__["country"] = country
+        __props__.__dict__["created"] = created
+        __props__.__dict__["description"] = description
         __props__.__dict__["display_name"] = display_name
-        __props__.__dict__["fixed_amount"] = fixed_amount
+        __props__.__dict__["inclusive"] = inclusive
+        __props__.__dict__["jurisdiction"] = jurisdiction
         __props__.__dict__["livemode"] = livemode
         __props__.__dict__["metadata"] = metadata
-        __props__.__dict__["tax_behavior"] = tax_behavior
-        __props__.__dict__["tax_code"] = tax_code
-        __props__.__dict__["type"] = type
-        return ShippingRate(resource_name, opts=opts, __props__=__props__)
+        __props__.__dict__["object"] = object
+        __props__.__dict__["percentage"] = percentage
+        __props__.__dict__["state"] = state
+        __props__.__dict__["tax_type"] = tax_type
+        return TaxRate(resource_name, opts=opts, __props__=__props__)
 
     @property
     @pulumi.getter
     def active(self) -> pulumi.Output[Optional[bool]]:
         """
-        Bool. Whether the shipping rate is active (can't be used when creating). Defaults to `true`.
+        Bool. Flag determining whether the tax rate is active or inactive (archived). Inactive tax rates cannot be used with new applications or Checkout Sessions, but will still work for subscriptions and invoices that already have it set.
         """
         return pulumi.get(self, "active")
 
     @property
-    @pulumi.getter(name="deliveryEstimates")
-    def delivery_estimates(self) -> pulumi.Output[Optional[Sequence['outputs.ShippingRateDeliveryEstimate']]]:
+    @pulumi.getter
+    def country(self) -> pulumi.Output[Optional[str]]:
         """
-        List(Resource). The estimated range for how long shipping will take, 
-        meant to be displayable to the customer. This will appear on CheckoutSessions.
-        For details please see Delivery Estimate.
+        String. Two-letter country code (ISO 3166-1 alpha-2).
         """
-        return pulumi.get(self, "delivery_estimates")
+        return pulumi.get(self, "country")
+
+    @property
+    @pulumi.getter
+    def created(self) -> pulumi.Output[int]:
+        """
+        Int. Time at which the object was created. Measured in seconds since the Unix epoch.
+        """
+        return pulumi.get(self, "created")
+
+    @property
+    @pulumi.getter
+    def description(self) -> pulumi.Output[Optional[str]]:
+        """
+        String. An arbitrary string attached to the tax rate for your internal use only. It will not be visible to your customers.
+        """
+        return pulumi.get(self, "description")
 
     @property
     @pulumi.getter(name="displayName")
     def display_name(self) -> pulumi.Output[str]:
         """
-        String. The name of the shipping rate, meant to be displayable to the customer. 
-        This will appear on CheckoutSessions.
+        String. The display name of the tax rate, which will be shown to users.
         """
         return pulumi.get(self, "display_name")
 
     @property
-    @pulumi.getter(name="fixedAmount")
-    def fixed_amount(self) -> pulumi.Output['outputs.ShippingRateFixedAmount']:
+    @pulumi.getter
+    def inclusive(self) -> pulumi.Output[bool]:
+        """
+        Bool. This specifies if the tax rate is inclusive or exclusive.
+        * `percentage ` - (Required) Float. This represents the tax rate percent out of 100.
+        """
+        return pulumi.get(self, "inclusive")
+
+    @property
+    @pulumi.getter
+    def jurisdiction(self) -> pulumi.Output[Optional[str]]:
         """
-        List(Resource). Describes a fixed amount to charge for shipping. 
-        Must be present if type is `fixed_amount`. For details of individual arguments see Fixed Amount.
+        String. The jurisdiction for the tax rate. You can use this label field for tax reporting purposes. It also appears on your customer’s invoice.
         """
-        return pulumi.get(self, "fixed_amount")
+        return pulumi.get(self, "jurisdiction")
 
     @property
     @pulumi.getter
     def livemode(self) -> pulumi.Output[bool]:
         """
         Bool. Has the value true if the object exists in live mode or the value false if the object exists in test mode.
         """
         return pulumi.get(self, "livemode")
 
     @property
     @pulumi.getter
     def metadata(self) -> pulumi.Output[Optional[Mapping[str, str]]]:
         """
-        Map(String). Set of key-value pairs that you can attach to an object. This can be useful for
-        storing additional information about the object in a structured format.
+        Map(String). Set of key-value pairs that you can attach to an object. This can be useful for storing additional information about the object in a structured format. Individual keys can be unset by posting an empty value to them. All keys can be unset by posting an empty value to metadata.
         """
         return pulumi.get(self, "metadata")
 
     @property
-    @pulumi.getter(name="taxBehavior")
-    def tax_behavior(self) -> pulumi.Output[Optional[str]]:
+    @pulumi.getter
+    def object(self) -> pulumi.Output[str]:
         """
-        Specifies whether the rate is considered inclusive of taxes or exclusive of taxes. One of inclusive, exclusive, or
-        unspecified.
+        String. String representing the object’s type. Objects of the same type share the same value.
         """
-        return pulumi.get(self, "tax_behavior")
+        return pulumi.get(self, "object")
 
     @property
-    @pulumi.getter(name="taxCode")
-    def tax_code(self) -> pulumi.Output[Optional[str]]:
+    @pulumi.getter
+    def percentage(self) -> pulumi.Output[float]:
         """
-        String. A tax code ID. The Shipping tax code is `txcd_92010001`.
+        This represents the tax rate percent out of 100.
         """
-        return pulumi.get(self, "tax_code")
+        return pulumi.get(self, "percentage")
 
     @property
     @pulumi.getter
-    def type(self) -> pulumi.Output[Optional[str]]:
+    def state(self) -> pulumi.Output[Optional[str]]:
+        """
+        String. ISO 3166-2 subdivision code, without country prefix. For example, “NY” for New York, United States.
+        """
+        return pulumi.get(self, "state")
+
+    @property
+    @pulumi.getter(name="taxType")
+    def tax_type(self) -> pulumi.Output[Optional[str]]:
         """
-        String. The type of calculation to use on the shipping rate. Can only be `fixed_amount` for now.
+        String. The high-level tax type, such as vat or sales_tax.
         """
-        return pulumi.get(self, "type")
+        return pulumi.get(self, "tax_type")
```

### Comparing `pulumi_stripe-0.0.23/pulumi_stripe/webhook_endpoint.py` & `pulumi_stripe-0.0.8/pulumi_stripe/webhook_endpoint.py`

 * *Files 0% similar despite different names*

```diff
@@ -281,28 +281,26 @@
         """
         With this resource, you can create a webhook endpoint - [Stripe API webhook endpoint documentation](https://stripe.com/docs/api/webhook_endpoints).
 
         You can configure webhook endpoints via the API to be notified about events that happen in your Stripe account or connected accounts.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_stripe as stripe
 
         webhook = stripe.WebhookEndpoint("webhook",
             description="example of webhook",
             enabled_events=[
                 "customer.subscription.created",
                 "customer.subscription.updated",
             ],
             url="https://webhook-url-consumer.com")
         ```
-        <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] api_version: String. Events sent to this endpoint will be generated with this Stripe Version instead of your account’s default Stripe Version.
         :param pulumi.Input[bool] connect: Bool. Whether this endpoint should receive events from connected accounts (`true`), or from your account (`false`). Defaults to `false`.
         :param pulumi.Input[str] description: String. Description of what the webhook is used for.
         :param pulumi.Input[bool] disabled: Bool. Disable the webhook endpoint if set to `true`. Can be used only for modification already existing webhook endpoint.
@@ -319,28 +317,26 @@
         """
         With this resource, you can create a webhook endpoint - [Stripe API webhook endpoint documentation](https://stripe.com/docs/api/webhook_endpoints).
 
         You can configure webhook endpoints via the API to be notified about events that happen in your Stripe account or connected accounts.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_stripe as stripe
 
         webhook = stripe.WebhookEndpoint("webhook",
             description="example of webhook",
             enabled_events=[
                 "customer.subscription.created",
                 "customer.subscription.updated",
             ],
             url="https://webhook-url-consumer.com")
         ```
-        <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
         :param WebhookEndpointArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
```

### Comparing `pulumi_stripe-0.0.23/pulumi_stripe.egg-info/SOURCES.txt` & `pulumi_stripe-0.0.8/pulumi_stripe.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -2,24 +2,22 @@
 setup.py
 pulumi_stripe/__init__.py
 pulumi_stripe/_inputs.py
 pulumi_stripe/_utilities.py
 pulumi_stripe/card.py
 pulumi_stripe/coupon.py
 pulumi_stripe/customer.py
-pulumi_stripe/file.py
 pulumi_stripe/outputs.py
 pulumi_stripe/portal_configuration.py
 pulumi_stripe/price.py
 pulumi_stripe/product.py
 pulumi_stripe/promotion_code.py
 pulumi_stripe/provider.py
 pulumi_stripe/pulumi-plugin.json
 pulumi_stripe/py.typed
-pulumi_stripe/shipping_rate.py
 pulumi_stripe/tax_rate.py
 pulumi_stripe/webhook_endpoint.py
 pulumi_stripe.egg-info/PKG-INFO
 pulumi_stripe.egg-info/SOURCES.txt
 pulumi_stripe.egg-info/dependency_links.txt
 pulumi_stripe.egg-info/not-zip-safe
 pulumi_stripe.egg-info/requires.txt
```

### Comparing `pulumi_stripe-0.0.23/setup.py` & `pulumi_stripe-0.0.8/setup.py`

 * *Files 27% similar despite different names*

```diff
@@ -4,29 +4,52 @@
 
 import errno
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = "0.0.23"
+VERSION = "0.0.8"
+PLUGIN_VERSION = "0.0.8"
+
+class InstallPluginCommand(install):
+    def run(self):
+        install.run(self)
+        try:
+            check_call(['pulumi', 'plugin', 'install', 'resource', 'stripe', PLUGIN_VERSION])
+        except OSError as error:
+            if error.errno == errno.ENOENT:
+                print(f"""
+                There was an error installing the stripe resource provider plugin.
+                It looks like `pulumi` is not installed on your system.
+                Please visit https://pulumi.com/ to install the Pulumi CLI.
+                You may try manually installing the plugin by running
+                `pulumi plugin install resource stripe {PLUGIN_VERSION}`
+                """)
+            else:
+                raise
+
+
 def readme():
     try:
         with open('README.md', encoding='utf-8') as f:
             return f.read()
     except FileNotFoundError:
         return "stripe Pulumi Package - Development Version"
 
 
 setup(name='pulumi_stripe',
-      python_requires='>=3.8',
+      python_requires='>=3.7',
       version=VERSION,
-      description="A Pulumi package for creating and managing Stripe resources.",
+      description="A Pulumi package for creating and managing stripe cloud resources.",
       long_description=readme(),
       long_description_content_type='text/markdown',
+      cmdclass={
+          'install': InstallPluginCommand,
+      },
       keywords='pulumi stripe category/cloud',
       url='https://www.pulumi.com',
       project_urls={
           'Repository': 'https://github.com/georgegebbett/pulumi-stripe'
       },
       license='Apache-2.0',
       packages=find_packages(),
```

