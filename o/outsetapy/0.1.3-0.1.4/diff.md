# Comparing `tmp/outsetapy-0.1.3.tar.gz` & `tmp/outsetapy-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "outsetapy-0.1.3.tar", last modified: Fri Mar 29 18:37:02 2024, max compression
+gzip compressed data, was "outsetapy-0.1.4.tar", last modified: Mon Apr  1 15:51:44 2024, max compression
```

## Comparing `outsetapy-0.1.3.tar` & `outsetapy-0.1.4.tar`

### file list

```diff
@@ -1,86 +1,86 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 18:37:02.487078 outsetapy-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (127)      493 2024-03-29 18:37:02.487078 outsetapy-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      609 2024-03-29 18:36:57.000000 outsetapy-0.1.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-29 18:37:02.487078 outsetapy-0.1.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 18:37:02.471078 outsetapy-0.1.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 18:37:02.475078 outsetapy-0.1.3/src/outsetapy/
--rw-r--r--   0 runner    (1001) docker     (127)     1842 2024-03-29 18:36:57.000000 outsetapy-0.1.3/src/outsetapy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 18:37:02.475078 outsetapy-0.1.3/src/outsetapy/api/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-29 18:36:57.000000 outsetapy-0.1.3/src/outsetapy/api/__inti__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 18:37:02.475078 outsetapy-0.1.3/src/outsetapy/api/billing/
--rw-r--r--   0 runner    (1001) docker     (127)      550 2024-03-29 18:36:57.000000 outsetapy-0.1.3/src/outsetapy/api/billing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2309 2024-03-29 18:36:57.000000 outsetapy-0.1.3/src/outsetapy/api/billing/invoices.py
--rw-r--r--   0 runner    (1001) docker     (127)     1156 2024-03-29 18:36:57.000000 outsetapy-0.1.3/src/outsetapy/api/billing/plan_families.py
--rw-r--r--   0 runner    (1001) docker     (127)     1805 2024-03-29 18:36:57.000000 outsetapy-0.1.3/src/outsetapy/api/billing/plans.py
--rw-r--r--   0 runner    (1001) docker     (127)     5650 2024-03-29 18:36:57.000000 outsetapy-0.1.3/src/outsetapy/api/billing/subscriptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-03-29 18:36:57.000000 outsetapy-0.1.3/src/outsetapy/api/billing/transactions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2760 2024-03-29 18:36:57.000000 outsetapy-0.1.3/src/outsetapy/api/billing/usage.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 18:37:02.479078 outsetapy-0.1.3/src/outsetapy/api/crm/
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-03-29 18:36:57.000000 outsetapy-0.1.3/src/outsetapy/api/crm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6581 2024-03-29 18:36:57.000000 outsetapy-0.1.3/src/outsetapy/api/crm/accounts.py
--rw-r--r--   0 runner    (1001) docker     (127)     2576 2024-03-29 18:36:57.000000 outsetapy-0.1.3/src/outsetapy/api/crm/activities.py
--rw-r--r--   0 runner    (1001) docker     (127)     3626 2024-03-29 18:36:57.000000 outsetapy-0.1.3/src/outsetapy/api/crm/deals.py
--rw-r--r--   0 runner    (1001) docker     (127)     2593 2024-03-29 18:36:57.000000 outsetapy-0.1.3/src/outsetapy/api/crm/people.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 18:37:02.479078 outsetapy-0.1.3/src/outsetapy/api/marketing/
--rw-r--r--   0 runner    (1001) docker     (127)      225 2024-03-29 18:36:57.000000 outsetapy-0.1.3/src/outsetapy/api/marketing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3104 2024-03-29 18:36:57.000000 outsetapy-0.1.3/src/outsetapy/api/marketing/email_list_subscriptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 18:37:02.479078 outsetapy-0.1.3/src/outsetapy/api/support/
--rw-r--r--   0 runner    (1001) docker     (127)      153 2024-03-29 18:36:57.000000 outsetapy-0.1.3/src/outsetapy/api/support/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4065 2024-03-29 18:36:57.000000 outsetapy-0.1.3/src/outsetapy/api/support/cases.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 18:37:02.479078 outsetapy-0.1.3/src/outsetapy/api/user/
--rw-r--r--   0 runner    (1001) docker     (127)     1786 2024-03-29 18:36:57.000000 outsetapy-0.1.3/src/outsetapy/api/user/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      774 2024-03-29 18:36:57.000000 outsetapy-0.1.3/src/outsetapy/api/user/password.py
--rw-r--r--   0 runner    (1001) docker     (127)     1243 2024-03-29 18:36:57.000000 outsetapy-0.1.3/src/outsetapy/api/user/profile.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 18:37:02.479078 outsetapy-0.1.3/src/outsetapy/models/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-29 18:36:57.000000 outsetapy-0.1.3/src/outsetapy/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 18:37:02.483078 outsetapy-0.1.3/src/outsetapy/models/billing/
--rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-03-29 18:36:57.000000 outsetapy-0.1.3/src/outsetapy/models/billing/add_on.py
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-03-29 18:36:57.000000 outsetapy-0.1.3/src/outsetapy/models/billing/billing_add_on_type.py
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-03-29 18:36:57.000000 outsetapy-0.1.3/src/outsetapy/models/billing/billing_renewal_term.py
--rw-r--r--   0 runner    (1001) docker     (127)      141 2024-03-29 18:36:57.000000 outsetapy-0.1.3/src/outsetapy/models/billing/billing_transaction_type.py
--rw-r--r--   0 runner    (1001) docker     (127)      727 2024-03-29 18:36:57.000000 outsetapy-0.1.3/src/outsetapy/models/billing/charge_summary.py
--rw-r--r--   0 runner    (1001) docker     (127)      470 2024-03-29 18:36:57.000000 outsetapy-0.1.3/src/outsetapy/models/billing/invoice.py
--rw-r--r--   0 runner    (1001) docker     (127)      263 2024-03-29 18:36:57.000000 outsetapy-0.1.3/src/outsetapy/models/billing/invoice_display_item.py
--rw-r--r--   0 runner    (1001) docker     (127)     1259 2024-03-29 18:36:57.000000 outsetapy-0.1.3/src/outsetapy/models/billing/invoice_line_item.py
--rw-r--r--   0 runner    (1001) docker     (127)     2249 2024-03-29 18:36:57.000000 outsetapy-0.1.3/src/outsetapy/models/billing/plan.py
--rw-r--r--   0 runner    (1001) docker     (127)      293 2024-03-29 18:36:57.000000 outsetapy-0.1.3/src/outsetapy/models/billing/plan_add_on.py
--rw-r--r--   0 runner    (1001) docker     (127)      298 2024-03-29 18:36:57.000000 outsetapy-0.1.3/src/outsetapy/models/billing/plan_family.py
--rw-r--r--   0 runner    (1001) docker     (127)     1896 2024-03-29 18:36:57.000000 outsetapy-0.1.3/src/outsetapy/models/billing/subscription.py
--rw-r--r--   0 runner    (1001) docker     (127)      921 2024-03-29 18:36:57.000000 outsetapy-0.1.3/src/outsetapy/models/billing/subscription_add_on.py
--rw-r--r--   0 runner    (1001) docker     (127)      911 2024-03-29 18:36:57.000000 outsetapy-0.1.3/src/outsetapy/models/billing/transaction.py
--rw-r--r--   0 runner    (1001) docker     (127)      624 2024-03-29 18:36:57.000000 outsetapy-0.1.3/src/outsetapy/models/billing/usage_item.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 18:37:02.483078 outsetapy-0.1.3/src/outsetapy/models/crm/
--rw-r--r--   0 runner    (1001) docker     (127)     3783 2024-03-29 18:36:57.000000 outsetapy-0.1.3/src/outsetapy/models/crm/account.py
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-03-29 18:36:57.000000 outsetapy-0.1.3/src/outsetapy/models/crm/account_stage.py
--rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-03-29 18:36:57.000000 outsetapy-0.1.3/src/outsetapy/models/crm/activity.py
--rw-r--r--   0 runner    (1001) docker     (127)      802 2024-03-29 18:36:57.000000 outsetapy-0.1.3/src/outsetapy/models/crm/activity_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     1178 2024-03-29 18:36:57.000000 outsetapy-0.1.3/src/outsetapy/models/crm/deal.py
--rw-r--r--   0 runner    (1001) docker     (127)      751 2024-03-29 18:36:57.000000 outsetapy-0.1.3/src/outsetapy/models/crm/deal_person.py
--rw-r--r--   0 runner    (1001) docker     (127)      504 2024-03-29 18:36:57.000000 outsetapy-0.1.3/src/outsetapy/models/crm/deal_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)      569 2024-03-29 18:36:57.000000 outsetapy-0.1.3/src/outsetapy/models/crm/deal_pipeline_stage.py
--rw-r--r--   0 runner    (1001) docker     (127)      917 2024-03-29 18:36:57.000000 outsetapy-0.1.3/src/outsetapy/models/crm/person.py
--rw-r--r--   0 runner    (1001) docker     (127)      612 2024-03-29 18:36:57.000000 outsetapy-0.1.3/src/outsetapy/models/crm/person_account.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 18:37:02.483078 outsetapy-0.1.3/src/outsetapy/models/marketing/
--rw-r--r--   0 runner    (1001) docker     (127)     1776 2024-03-29 18:36:57.000000 outsetapy-0.1.3/src/outsetapy/models/marketing/email_list_person.py
--rw-r--r--   0 runner    (1001) docker     (127)      642 2024-03-29 18:36:57.000000 outsetapy-0.1.3/src/outsetapy/models/marketing/emaillist.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 18:37:02.483078 outsetapy-0.1.3/src/outsetapy/models/shared/
--rw-r--r--   0 runner    (1001) docker     (127)      800 2024-03-29 18:36:57.000000 outsetapy-0.1.3/src/outsetapy/models/shared/address.py
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-03-29 18:36:57.000000 outsetapy-0.1.3/src/outsetapy/models/shared/entity.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 18:37:02.483078 outsetapy-0.1.3/src/outsetapy/models/support/
--rw-r--r--   0 runner    (1001) docker     (127)     2535 2024-03-29 18:36:57.000000 outsetapy-0.1.3/src/outsetapy/models/support/case.py
--rw-r--r--   0 runner    (1001) docker     (127)     1054 2024-03-29 18:36:57.000000 outsetapy-0.1.3/src/outsetapy/models/support/case_history.py
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-03-29 18:36:57.000000 outsetapy-0.1.3/src/outsetapy/models/support/case_source.py
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-03-29 18:36:57.000000 outsetapy-0.1.3/src/outsetapy/models/support/case_status.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 18:37:02.483078 outsetapy-0.1.3/src/outsetapy/models/wrappers/
--rw-r--r--   0 runner    (1001) docker     (127)      343 2024-03-29 18:36:57.000000 outsetapy-0.1.3/src/outsetapy/models/wrappers/list.py
--rw-r--r--   0 runner    (1001) docker     (127)      817 2024-03-29 18:36:57.000000 outsetapy-0.1.3/src/outsetapy/models/wrappers/validation_error.py
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-03-29 18:36:57.000000 outsetapy-0.1.3/src/outsetapy/static.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 18:37:02.487078 outsetapy-0.1.3/src/outsetapy/util/
--rw-r--r--   0 runner    (1001) docker     (127)     1653 2024-03-29 18:36:57.000000 outsetapy-0.1.3/src/outsetapy/util/credentials.py
--rw-r--r--   0 runner    (1001) docker     (127)     2466 2024-03-29 18:36:57.000000 outsetapy-0.1.3/src/outsetapy/util/request.py
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-03-29 18:36:57.000000 outsetapy-0.1.3/src/outsetapy/util/store.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 18:37:02.487078 outsetapy-0.1.3/src/outsetapy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      493 2024-03-29 18:37:02.000000 outsetapy-0.1.3/src/outsetapy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2610 2024-03-29 18:37:02.000000 outsetapy-0.1.3/src/outsetapy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-29 18:37:02.000000 outsetapy-0.1.3/src/outsetapy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-03-29 18:37:02.000000 outsetapy-0.1.3/src/outsetapy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 15:51:44.970419 outsetapy-0.1.4/
+-rw-r--r--   0 runner    (1001) docker     (127)      493 2024-04-01 15:51:44.970419 outsetapy-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      609 2024-04-01 15:51:39.000000 outsetapy-0.1.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-01 15:51:44.970419 outsetapy-0.1.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 15:51:44.958419 outsetapy-0.1.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 15:51:44.962419 outsetapy-0.1.4/src/outsetapy/
+-rw-r--r--   0 runner    (1001) docker     (127)     1842 2024-04-01 15:51:39.000000 outsetapy-0.1.4/src/outsetapy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 15:51:44.962419 outsetapy-0.1.4/src/outsetapy/api/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 15:51:39.000000 outsetapy-0.1.4/src/outsetapy/api/__inti__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 15:51:44.962419 outsetapy-0.1.4/src/outsetapy/api/billing/
+-rw-r--r--   0 runner    (1001) docker     (127)      550 2024-04-01 15:51:39.000000 outsetapy-0.1.4/src/outsetapy/api/billing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2331 2024-04-01 15:51:39.000000 outsetapy-0.1.4/src/outsetapy/api/billing/invoices.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1167 2024-04-01 15:51:39.000000 outsetapy-0.1.4/src/outsetapy/api/billing/plan_families.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1816 2024-04-01 15:51:39.000000 outsetapy-0.1.4/src/outsetapy/api/billing/plans.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5802 2024-04-01 15:51:39.000000 outsetapy-0.1.4/src/outsetapy/api/billing/subscriptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-01 15:51:39.000000 outsetapy-0.1.4/src/outsetapy/api/billing/transactions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2782 2024-04-01 15:51:39.000000 outsetapy-0.1.4/src/outsetapy/api/billing/usage.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 15:51:44.962419 outsetapy-0.1.4/src/outsetapy/api/crm/
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-04-01 15:51:39.000000 outsetapy-0.1.4/src/outsetapy/api/crm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6933 2024-04-01 15:51:39.000000 outsetapy-0.1.4/src/outsetapy/api/crm/accounts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2598 2024-04-01 15:51:39.000000 outsetapy-0.1.4/src/outsetapy/api/crm/activities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3681 2024-04-01 15:51:39.000000 outsetapy-0.1.4/src/outsetapy/api/crm/deals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2593 2024-04-01 15:51:39.000000 outsetapy-0.1.4/src/outsetapy/api/crm/people.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 15:51:44.962419 outsetapy-0.1.4/src/outsetapy/api/marketing/
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-04-01 15:51:39.000000 outsetapy-0.1.4/src/outsetapy/api/marketing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3137 2024-04-01 15:51:39.000000 outsetapy-0.1.4/src/outsetapy/api/marketing/email_list_subscriptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 15:51:44.966419 outsetapy-0.1.4/src/outsetapy/api/support/
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2024-04-01 15:51:39.000000 outsetapy-0.1.4/src/outsetapy/api/support/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4109 2024-04-01 15:51:39.000000 outsetapy-0.1.4/src/outsetapy/api/support/cases.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 15:51:44.966419 outsetapy-0.1.4/src/outsetapy/api/user/
+-rw-r--r--   0 runner    (1001) docker     (127)     1786 2024-04-01 15:51:39.000000 outsetapy-0.1.4/src/outsetapy/api/user/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      785 2024-04-01 15:51:39.000000 outsetapy-0.1.4/src/outsetapy/api/user/password.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1265 2024-04-01 15:51:39.000000 outsetapy-0.1.4/src/outsetapy/api/user/profile.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 15:51:44.966419 outsetapy-0.1.4/src/outsetapy/models/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 15:51:39.000000 outsetapy-0.1.4/src/outsetapy/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 15:51:44.966419 outsetapy-0.1.4/src/outsetapy/models/billing/
+-rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-04-01 15:51:39.000000 outsetapy-0.1.4/src/outsetapy/models/billing/add_on.py
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-01 15:51:39.000000 outsetapy-0.1.4/src/outsetapy/models/billing/billing_add_on_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-01 15:51:39.000000 outsetapy-0.1.4/src/outsetapy/models/billing/billing_renewal_term.py
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-04-01 15:51:39.000000 outsetapy-0.1.4/src/outsetapy/models/billing/billing_transaction_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)      727 2024-04-01 15:51:39.000000 outsetapy-0.1.4/src/outsetapy/models/billing/charge_summary.py
+-rw-r--r--   0 runner    (1001) docker     (127)      470 2024-04-01 15:51:39.000000 outsetapy-0.1.4/src/outsetapy/models/billing/invoice.py
+-rw-r--r--   0 runner    (1001) docker     (127)      263 2024-04-01 15:51:39.000000 outsetapy-0.1.4/src/outsetapy/models/billing/invoice_display_item.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1259 2024-04-01 15:51:39.000000 outsetapy-0.1.4/src/outsetapy/models/billing/invoice_line_item.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2249 2024-04-01 15:51:39.000000 outsetapy-0.1.4/src/outsetapy/models/billing/plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)      293 2024-04-01 15:51:39.000000 outsetapy-0.1.4/src/outsetapy/models/billing/plan_add_on.py
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2024-04-01 15:51:39.000000 outsetapy-0.1.4/src/outsetapy/models/billing/plan_family.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2189 2024-04-01 15:51:39.000000 outsetapy-0.1.4/src/outsetapy/models/billing/subscription.py
+-rw-r--r--   0 runner    (1001) docker     (127)      921 2024-04-01 15:51:39.000000 outsetapy-0.1.4/src/outsetapy/models/billing/subscription_add_on.py
+-rw-r--r--   0 runner    (1001) docker     (127)      911 2024-04-01 15:51:39.000000 outsetapy-0.1.4/src/outsetapy/models/billing/transaction.py
+-rw-r--r--   0 runner    (1001) docker     (127)      624 2024-04-01 15:51:39.000000 outsetapy-0.1.4/src/outsetapy/models/billing/usage_item.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 15:51:44.970419 outsetapy-0.1.4/src/outsetapy/models/crm/
+-rw-r--r--   0 runner    (1001) docker     (127)     4012 2024-04-01 15:51:39.000000 outsetapy-0.1.4/src/outsetapy/models/crm/account.py
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-01 15:51:39.000000 outsetapy-0.1.4/src/outsetapy/models/crm/account_stage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-04-01 15:51:39.000000 outsetapy-0.1.4/src/outsetapy/models/crm/activity.py
+-rw-r--r--   0 runner    (1001) docker     (127)      802 2024-04-01 15:51:39.000000 outsetapy-0.1.4/src/outsetapy/models/crm/activity_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1178 2024-04-01 15:51:39.000000 outsetapy-0.1.4/src/outsetapy/models/crm/deal.py
+-rw-r--r--   0 runner    (1001) docker     (127)      751 2024-04-01 15:51:39.000000 outsetapy-0.1.4/src/outsetapy/models/crm/deal_person.py
+-rw-r--r--   0 runner    (1001) docker     (127)      504 2024-04-01 15:51:39.000000 outsetapy-0.1.4/src/outsetapy/models/crm/deal_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)      569 2024-04-01 15:51:39.000000 outsetapy-0.1.4/src/outsetapy/models/crm/deal_pipeline_stage.py
+-rw-r--r--   0 runner    (1001) docker     (127)      917 2024-04-01 15:51:39.000000 outsetapy-0.1.4/src/outsetapy/models/crm/person.py
+-rw-r--r--   0 runner    (1001) docker     (127)      612 2024-04-01 15:51:39.000000 outsetapy-0.1.4/src/outsetapy/models/crm/person_account.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 15:51:44.970419 outsetapy-0.1.4/src/outsetapy/models/marketing/
+-rw-r--r--   0 runner    (1001) docker     (127)     1776 2024-04-01 15:51:39.000000 outsetapy-0.1.4/src/outsetapy/models/marketing/email_list_person.py
+-rw-r--r--   0 runner    (1001) docker     (127)      642 2024-04-01 15:51:39.000000 outsetapy-0.1.4/src/outsetapy/models/marketing/emaillist.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 15:51:44.970419 outsetapy-0.1.4/src/outsetapy/models/shared/
+-rw-r--r--   0 runner    (1001) docker     (127)      800 2024-04-01 15:51:39.000000 outsetapy-0.1.4/src/outsetapy/models/shared/address.py
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-01 15:51:39.000000 outsetapy-0.1.4/src/outsetapy/models/shared/entity.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 15:51:44.970419 outsetapy-0.1.4/src/outsetapy/models/support/
+-rw-r--r--   0 runner    (1001) docker     (127)     2535 2024-04-01 15:51:39.000000 outsetapy-0.1.4/src/outsetapy/models/support/case.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1054 2024-04-01 15:51:39.000000 outsetapy-0.1.4/src/outsetapy/models/support/case_history.py
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-01 15:51:39.000000 outsetapy-0.1.4/src/outsetapy/models/support/case_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-01 15:51:39.000000 outsetapy-0.1.4/src/outsetapy/models/support/case_status.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 15:51:44.970419 outsetapy-0.1.4/src/outsetapy/models/wrappers/
+-rw-r--r--   0 runner    (1001) docker     (127)      343 2024-04-01 15:51:39.000000 outsetapy-0.1.4/src/outsetapy/models/wrappers/list.py
+-rw-r--r--   0 runner    (1001) docker     (127)      817 2024-04-01 15:51:39.000000 outsetapy-0.1.4/src/outsetapy/models/wrappers/validation_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-01 15:51:39.000000 outsetapy-0.1.4/src/outsetapy/static.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 15:51:44.970419 outsetapy-0.1.4/src/outsetapy/util/
+-rw-r--r--   0 runner    (1001) docker     (127)     1653 2024-04-01 15:51:39.000000 outsetapy-0.1.4/src/outsetapy/util/credentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2466 2024-04-01 15:51:39.000000 outsetapy-0.1.4/src/outsetapy/util/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-01 15:51:39.000000 outsetapy-0.1.4/src/outsetapy/util/store.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 15:51:44.970419 outsetapy-0.1.4/src/outsetapy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      493 2024-04-01 15:51:44.000000 outsetapy-0.1.4/src/outsetapy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2610 2024-04-01 15:51:44.000000 outsetapy-0.1.4/src/outsetapy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 15:51:44.000000 outsetapy-0.1.4/src/outsetapy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-01 15:51:44.000000 outsetapy-0.1.4/src/outsetapy.egg-info/top_level.txt
```

### Comparing `outsetapy-0.1.3/pyproject.toml` & `outsetapy-0.1.4/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "outsetapy"
-version = "0.1.3"
+version = "0.1.4"
 
 authors = [
   { name="Roborian, Inc", email="info@roborian.com" },
 ]
 description = "A SDK for building applications with Outseta"
 readme = "README.md"
 requires-python = ">=3.8"
```

### Comparing `outsetapy-0.1.3/src/outsetapy/__init__.py` & `outsetapy-0.1.4/src/outsetapy/__init__.py`

 * *Files identical despite different names*

### Comparing `outsetapy-0.1.3/src/outsetapy/api/billing/__init__.py` & `outsetapy-0.1.4/src/outsetapy/api/billing/__init__.py`

 * *Files identical despite different names*

### Comparing `outsetapy-0.1.3/src/outsetapy/api/billing/invoices.py` & `outsetapy-0.1.4/src/outsetapy/api/billing/invoices.py`

 * *Files 9% similar despite different names*

```diff
@@ -29,30 +29,30 @@
 
     async def get_by_id(self, invoice_id: str) -> Invoice:
         request = Request(
             self.store, f"billing/invoices/{invoice_id}"
         ).authenticate_as_server()
         response = request.get()
         if not response.ok:
-            raise response
+            raise Exception(response)
         return response.json()
 
     async def get_all(self, options: dict = {}) -> List[Invoice]:
         has_more = True
         results = []
         while has_more:
             request = Request(self.store, "billing/invoices").authenticate_as_server()
             if "limit" in options:
                 request.with_params({"limit": str(options["limit"])})
             if "offset" in options:
                 request.with_params({"offset": str(options["offset"])})
 
             response = request.get()
             if not response.ok:
-                raise response
+                raise Exception(response)
 
             json_response = response.json()
             results += json_response["items"]
             has_more = hasMoreResults(json_response)
             options["offset"] = (
                 json_response["metadata"]["offset"] + json_response["metadata"]["limit"]
             )
```

### Comparing `outsetapy-0.1.3/src/outsetapy/api/billing/plan_families.py` & `outsetapy-0.1.4/src/outsetapy/api/billing/plan_families.py`

 * *Files 20% similar despite different names*

```diff
@@ -16,15 +16,15 @@
             if "limit" in options:
                 request.with_params({"limit": str(options["limit"])})
             if "offset" in options:
                 request.with_params({"offset": str(options["offset"])})
 
             response = request.get()
             if not response.ok:
-                raise response
+                raise Exception(response)
 
             json_response = response.json()
             results += json_response["items"]
             has_more = hasMoreResults(json_response)
             options["offset"] = (
                 json_response["metadata"]["offset"] + json_response["metadata"]["limit"]
             )
```

### Comparing `outsetapy-0.1.3/src/outsetapy/api/billing/plans.py` & `outsetapy-0.1.4/src/outsetapy/api/billing/plans.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,15 +38,15 @@
                 request.with_params({"offset": str(offset)})
             if plan_family:
                 request.with_params({"PlanFamily.Uid": plan_family.Uid})
 
             response = request.get()
 
             if not response.ok:
-                raise response
+                raise Exception(response)
             json_response = response.json()
             results += json_response["items"]
             has_more = hasMoreResults(json_response)
             offset = (
                 json_response["metadata"]["offset"] + json_response["metadata"]["limit"]
             )
```

### Comparing `outsetapy-0.1.3/src/outsetapy/api/billing/subscriptions.py` & `outsetapy-0.1.4/src/outsetapy/api/billing/subscriptions.py`

 * *Files 7% similar despite different names*

```diff
@@ -23,70 +23,70 @@
         self.__dict__ = subscription
 
 
 class Subscriptions:
     def __init__(self, store: Store):
         self.store = store
 
-    async def get_all(self, options: dict = {}) -> List[PlanFamily]:
+    async def get_all(self, options: dict = {}) -> List[Subscription]:
         has_more = True
         results = []
         while has_more:
             request = Request(self.store, "billing/subscriptions")
             if "limit" in options:
                 request.with_params({"limit": str(options["limit"])})
             if "offset" in options:
                 request.with_params({"offset": str(options["offset"])})
 
             response = request.get()
             if not response.ok:
-                raise response
+                raise Exception(response)
 
             json_response = response.json()
             results += json_response["items"]
             has_more = hasMoreResults(json_response)
             options["offset"] = (
                 json_response["metadata"]["offset"] + json_response["metadata"]["limit"]
             )
 
-        return [PlanFamily(json_obj) for json_obj in results]
+        return [Subscription(json_obj, self.store) for json_obj in results]
 
     async def get(self, uid: str, options: dict = {}) -> Subscription:
         request = Request(
             self.store, f"billing/subscriptions/{uid}"
         ).authenticate_as_server()
 
         if "fields" in options:
             request.with_params({"fields": options["fields"]})
         else:
             request.with_params({"fields": "*,Account.Uid,Plan.Uid"})
 
         response = request.get()
 
         if not response.ok:
-            raise response
+            raise Exception(response)
         json_response = response.json()
-        return Subscription(json_response)
+        return Subscription(json_response, self.store)
 
     async def add(
         self, subscription: dict
     ) -> Subscription:
         request = (
             Request(self.store, "billing/subscriptions/firsttimesubscription")
             .authenticate_as_server()
             .with_body(subscription)
         )
         response = await request.put()
 
         if response.status == 400:
             raise ValidationError(response.json())
         elif response.ok:
-            return Subscription(response.json())
+            return Subscription(response.json(), self.store)
         else:
-            raise response
+            raise Exception(response)
 
     async def preview_add(
         self, subscription: dict
     ) -> ChargeSummary | ValidationError[Subscription]:
         request = (
             Request(self.store, "billing/subscriptions/compute-charge-summary")
             .authenticate_as_server()
@@ -95,15 +95,15 @@
         response = await request.post()
 
         if response.status == 400:
             raise ValidationError(response.json())
         elif response.ok:
             return ChargeSummary(response.json())
         else:
-            raise response
+            raise Exception(response)
 
     async def update(
         self, subscription: dict
     ) -> Subscription | ValidationError[Subscription]:
         request = (
             Request(
                 self.store,
@@ -113,17 +113,17 @@
             .with_body(subscription)
         )
         response = await request.put()
 
         if response.status == 400:
             raise ValidationError(response.json())
         elif response.ok:
-            return Subscription(response.json())
+            return Subscription(response.json(), self.store)
         else:
-            raise response
+            raise Exception(response)
 
     async def preview_update(
         self, subscription: dict
     ) -> ChargeSummary | ValidationError[Subscription]:
         request = (
             Request(
                 self.store,
@@ -135,15 +135,15 @@
         response = await request.put()
 
         if response.status == 400:
             raise ValidationError(response.json())
         elif response.ok:
             return ChargeSummary(response.json())
         else:
-            raise response
+            raise Exception(response)
 
     async def set_subscription_upgrade_required(
         self, subscription: dict
     ) -> Subscription | ValidationError[None]:
         request = (
             Request(
                 self.store,
@@ -153,25 +153,25 @@
             .with_body(subscription)
         )
         response = await request.put()
 
         if response.status == 400:
             raise ValidationError(response.json())
         elif response.ok:
-            return Subscription(response.json())
+            return Subscription(response.json(), self.store)
         else:
-            raise response
+            raise Exception(response)
 
     async def change_trial_to_subscribed(
         self, uid: str
     ) -> None | ValidationError[Account]:
         request = Request(
             self.store, f"billing/subscriptions/{uid}/changetrialtosubscribed"
         ).authenticate_as_server()
         response = await request.put()
 
         if response.status == 400:
             raise Exception(response.json())
         elif response.ok:
             return None
         else:
-            raise response
+            raise Exception(response)
```

### Comparing `outsetapy-0.1.3/src/outsetapy/api/billing/transactions.py` & `outsetapy-0.1.4/src/outsetapy/api/billing/transactions.py`

 * *Files identical despite different names*

### Comparing `outsetapy-0.1.3/src/outsetapy/api/billing/usage.py` & `outsetapy-0.1.4/src/outsetapy/api/billing/usage.py`

 * *Files 6% similar despite different names*

```diff
@@ -56,15 +56,15 @@
                             "Account"
                         ].Uid
                     }
                 )
 
             response = request.get()
             if not response.ok:
-                raise response
+                raise Exception(response)
 
             json_response = response.json()
             results += json_response["items"]
             has_more = hasMoreResults(json_response)
             options["offset"] = (
                 json_response["metadata"]["offset"] + json_response["metadata"]["limit"]
             )
@@ -85,8 +85,8 @@
         response = await request.post()
 
         if response.status == 400:
             raise Exception(response.json())
         elif response.ok:
             return response.json()
         else:
-            raise response
+            raise Exception(response)
```

### Comparing `outsetapy-0.1.3/src/outsetapy/api/crm/accounts.py` & `outsetapy-0.1.4/src/outsetapy/api/crm/accounts.py`

 * *Files 4% similar despite different names*

```diff
@@ -31,43 +31,44 @@
             if "offset" in options:
                 request.with_params({"offset": str(options["offset"])})
             if "accountStage" in options:
                 request.with_params({"AccountStage": str(options["accountStage"])})
 
             response = request.get()
             if not response.ok:
-                raise response
+                raise Exception(response)
 
             json_response = response.json()
             results += json_response["items"]
             has_more = hasMoreResults(json_response)
             options["offset"] = (
                 json_response["metadata"]["offset"] + json_response["metadata"]["limit"]
             )
 
-        return [Account(json_obj) for json_obj in results]
+        return [Account(json_obj, self.store) for json_obj in results]
 
     async def get(self, uid: str, options: dict = {}) -> Account:
         request = (
             Request(self.store, f"crm/accounts/{uid}")
             .authenticate_as_server()
             .with_params(
                 {
                     "fields": options.get(
-                        "fields", "*,PersonAccount.*,PersonAccount.Person.Uid"
+                        # "fields", "*,PersonAccount.*,PersonAccount.Person.Uid"
+                        "fields", "*,PersonAccount.*,BillingAddress.*,MailingAddress.*,PersonAccount.Person.Uid,CurrentSubscription.Uid,LatestSubscription.Uid, PrimarySubscription.Uid, PrimaryContact.*"
                     )
                 }
             )
         )
         response = request.get()
 
         if not response.ok:
-            raise response
+            raise Exception(response)
         response_json = response.json()
-        return Account(response_json)
+        return Account(response_json, self.store)
 
     async def add(
         self, account: dict, options: dict = {}
     ) -> Union[Account, ValidationError[Account]]:
         request = (
             Request(self.store, "crm/accounts")
             .authenticate_as_server()
@@ -82,17 +83,17 @@
         )
         response = await request.post()
 
         if response.status == 400:
             raise Exception(response.json())
         elif response.ok:
             response_json = response.json()
-            return Account(response_json)
+            return Account(response_json, self.store)
         else:
-            raise response
+            raise Exception(response)
 
     async def update(
         self, account: dict, options: dict = {}
     ) -> Union[Account, ValidationError[Account]]:
         request = (
             Request(self.store, f'crm/accounts/{account["Uid"]}')
             .authenticate_as_server()
@@ -107,17 +108,17 @@
         )
         response = await request.put()
 
         if response.status == 400:
             raise Exception(response.json())
         elif response.ok:
             response_json = response.json()
-            return Account(response_json)
+            return Account(response_json, self.store)
         else:
-            raise response
+            raise Exception(response)
 
     async def cancel(self, cancellation: dict) -> Union[None, ValidationError[Account]]:
         request = (
             Request(
                 self.store,
                 f'crm/accounts/cancellation/{cancellation["Account"]["Uid"]}',
             )
@@ -128,22 +129,22 @@
         response = await request.put()
 
         if response.status == 400:
             raise Exception(response.json())
         elif response.ok:
             return None
         else:
-            raise response
+            raise Exception(response)
 
     async def delete(self, uid: str) -> None:
         request = Request(self.store, f"crm/accounts/{uid}").authenticate_as_server()
         response = await request.delete()
 
         if not response.ok:
-            raise response
+            raise Exception(response)
         return None
 
     async def extend_trial(
         self, uid: str, date: datetime
     ) -> Union[None, ValidationError[Subscription]]:
         request = (
             Request(self.store, f"crm/accounts/{uid}/extend-trial")
@@ -153,45 +154,45 @@
         response = await request.put()
 
         if response.status == 400:
             raise Exception(response.json())
         elif response.ok:
             return None
         else:
-            raise response
+            raise Exception(response)
 
     async def remove_cancellation(
         self, uid: str
     ) -> Union[None, ValidationError[Account]]:
         request = Request(
             self.store, f"crm/accounts/{uid}/remove-cancellation"
         ).authenticate_as_server()
         response = await request.put()
 
         if response.status == 400:
             raise Exception(response.json())
         elif response.ok:
             return None
         else:
-            raise response
+            raise Exception(response)
 
     async def expire_current_subscription(
         self, uid: str
     ) -> Union[None, ValidationError[Subscription]]:
         request = Request(
             self.store, f"crm/accounts/{uid}/expire-current-subscription"
         ).authenticate_as_server()
         response = await request.put()
 
         if response.status == 400:
             raise Exception(response.json())
         elif response.ok:
             return None
         else:
-            raise response
+            raise Exception(response)
 
 
 class AccountAdd(dict):
     def __init__(self, name: str, account_stage: AccountStage, **kwargs):
         super().__init__(**kwargs)
         self["Name"] = name
         self["AccountStage"] = account_stage
```

### Comparing `outsetapy-0.1.3/src/outsetapy/api/crm/activities.py` & `outsetapy-0.1.4/src/outsetapy/api/crm/activities.py`

 * *Files 8% similar despite different names*

```diff
@@ -42,15 +42,15 @@
                 results += json_response["items"]
                 has_more = hasMoreResults(json_response)
                 options["offset"] = (
                     json_response["metadata"]["offset"]
                     + json_response["metadata"]["limit"]
                 )
             else:
-                raise response
+                raise Exception(response)
 
         return [Activity(json_obj) for json_obj in results]
 
     async def add(
         self, activity: dict, options: dict = {}
     ) -> Union[Activity, ValidationError[None]]:
         request = (
@@ -63,15 +63,15 @@
 
         if response.status == 400:
             raise Exception(response.json())
         elif response.ok:
             json_response = response.json()
             return Activity(json_response)
         else:
-            raise response
+            raise Exception(response)
 
 
 class ActivityAdd:
     pass
 
 
 # todo! check this line
```

### Comparing `outsetapy-0.1.3/src/outsetapy/api/crm/deals.py` & `outsetapy-0.1.4/src/outsetapy/api/crm/deals.py`

 * *Files 9% similar despite different names*

```diff
@@ -38,15 +38,15 @@
             if "deal_pipeline_stage" in options:
                 request.with_params(
                     {"DealPipelineStage.Uid": options["deal_pipeline_stage"]}
                 )
 
             response = request.get()
             if not response.ok:
-                raise response
+                raise Exception(response)
 
             json_response = response.json()
             results += json_response["items"]
             has_more = hasMoreResults(json_response)
             options["offset"] = (
                 json_response["metadata"]["offset"] + json_response["metadata"]["limit"]
             )
@@ -59,15 +59,15 @@
             .with_params({"fields": fields or Deals.DEFAULT_FIELDS})
             .authenticate_as_server()
         )
 
         response = request.get()
 
         if not response.ok:
-            raise response
+            raise Exception(response)
 
         json_response = response.json()
         return Deal(**json_response)
 
     async def add(
         self, deal: DealAdd, fields=None
     ) -> Union[Deal, ValidationError[Deal]]:
@@ -82,15 +82,15 @@
 
         if response.status == 400:
             raise Exception(response.json())
         elif response.ok:
             json_response = response.json()
             return Deal(**json_response)
         else:
-            raise response
+            raise Exception(response)
 
     async def update(
         self, deal: DealUpdate, fields=None
     ) -> Union[Deal, ValidationError[Deal]]:
         request = (
             Request(self.store, f"crm/deals/{deal.Uid}")
             .with_params({"fields": fields or Deals.DEFAULT_FIELDS})
@@ -102,18 +102,18 @@
 
         if response.status == 400:
             raise Exception(response.json())
         elif response.ok:
             json_response = response.json()
             return Deal(**json_response)
         else:
-            raise response
+            raise Exception(response)
 
     async def delete(self, uid: str) -> None:
         request = Request(self.store, f"crm/deals/{uid}").authenticate_as_server()
 
         response = await request.delete()
 
         if not response.ok:
-            raise response
+            raise Exception(response)
 
         return None
```

### Comparing `outsetapy-0.1.3/src/outsetapy/api/crm/people.py` & `outsetapy-0.1.4/src/outsetapy/api/crm/people.py`

 * *Files identical despite different names*

### Comparing `outsetapy-0.1.3/src/outsetapy/api/marketing/email_list_subscriptions.py` & `outsetapy-0.1.4/src/outsetapy/api/marketing/email_list_subscriptions.py`

 * *Files 4% similar despite different names*

```diff
@@ -33,15 +33,15 @@
                 request.with_params({"limit": str(options["limit"])})
             if "offset" in options:
                 request.with_params({"offset": str(options["offset"])})
 
             response = request.get()
 
             if not response.ok:
-                raise response
+                raise Exception(response)
 
             json_response = response.json()
             results += json_response
             has_more = hasMoreResults(json_response)
             options["offset"] = (
                 json_response["metadata"]["offset"] + json_response["metadata"]["limit"]
             )
@@ -67,25 +67,25 @@
         response = await request.post()
 
         if response.status == 400:
             raise ValidationError(response.json())
         elif response.ok:
             return None
         else:
-            raise response
+            raise Exception(response)
 
     async def delete(self, subscription: dict) -> None:
         request = Request(
             self.store,
             f'email/lists/{subscription["EmailList"]["Uid"]}/subscriptions/{subscription["Person"]["Uid"]}',
         ).authenticate_as_server()
         response = await request.delete()
 
         if not response.ok:
-            raise response
+            raise Exception(response)
         return None
 
 
 class SubscriptionAdd(EmailListPerson):
     EmailList: EmailList
     Person: Person
```

### Comparing `outsetapy-0.1.3/src/outsetapy/api/support/cases.py` & `outsetapy-0.1.4/src/outsetapy/api/support/cases.py`

 * *Files 13% similar despite different names*

```diff
@@ -36,15 +36,15 @@
                     request.with_params({"FromPerson.Uid": from_person["Uid"]})
                 elif "Email" in from_person:
                     request.with_params({"FromPerson.Email": from_person["Email"]})
 
             response = request.get()
 
             if not response.ok:
-                raise response
+                raise Exception(response)
 
             response_json = response.json()
             results += response_json["items"]
             has_more = hasMoreResults(response_json)
             options["offset"] = (
                 response_json["metadata"]["offset"] + response_json["metadata"]["limit"]
             )
@@ -72,40 +72,40 @@
 
         if response.status == 400:
             raise Exception(response.json())
         elif response.ok:
             response_json = response.json()
             return Case(response_json)
         else:
-            raise response
+            raise Exception(response)
 
     async def add_reply_from_agent(self, reply: dict) -> None:
         request = (
             Request(self.store, f"support/cases/{reply['Case']['Uid']}/replies")
             .authenticate_as_server()
             .with_body(reply)
         )
 
         response = await request.post()
 
         if not response.ok:
-            raise response
+            raise Exception(response)
 
     async def add_reply_from_client(self, reply: dict) -> CaseHistory:
         request = Request(
             self.store,
             f"support/cases/{reply['Case']['Uid']}/clientresponse/{reply['Comment']}",
         ).authenticate_as_server()
 
         response = await request.post()
 
         if response.ok:
             return CaseHistory(response.json())
         else:
-            raise response
+            raise Exception(response)
 
 
 class CaseAdd:
     def __init__(self, new_case: dict):
         self.FromPerson = new_case["FromPerson"]
         self.Subject = new_case["Subject"]
         self.Body = new_case["Body"]
```

### Comparing `outsetapy-0.1.3/src/outsetapy/api/user/__init__.py` & `outsetapy-0.1.4/src/outsetapy/api/user/__init__.py`

 * *Files identical despite different names*

### Comparing `outsetapy-0.1.3/src/outsetapy/api/user/password.py` & `outsetapy-0.1.4/src/outsetapy/api/user/password.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,8 +18,8 @@
         response = await request.put()
 
         if response.status == 400:
             raise ValidationError(response.json())
         elif response.ok:
             return None
         else:
-            raise response
+            raise Exception(response)
```

### Comparing `outsetapy-0.1.3/src/outsetapy/api/user/profile.py` & `outsetapy-0.1.4/src/outsetapy/api/user/profile.py`

 * *Files 14% similar despite different names*

```diff
@@ -19,15 +19,15 @@
         request = Request(self.store, "profile").authenticate_as_user()
         if fields:
             request.with_params({"fields": fields})
 
         response = request.get()
 
         if not response.ok:
-            raise response
+            raise Exception(response)
         return Person(response.json())
 
     async def update(
         self, profile: ProfileUpdate
     ) -> Union[Person, ValidationError[Person]]:
         request = (
             Request(self.store, "profile").authenticate_as_user().with_body(profile)
@@ -35,8 +35,8 @@
         response = await request.put()
 
         if response.status == 400:
             raise Exception(response.json())
         elif response.ok:
             return Person(response.json())
         else:
-            raise response
+            raise Exception(response)
```

### Comparing `outsetapy-0.1.3/src/outsetapy/models/billing/add_on.py` & `outsetapy-0.1.4/src/outsetapy/models/billing/add_on.py`

 * *Files identical despite different names*

### Comparing `outsetapy-0.1.3/src/outsetapy/models/billing/charge_summary.py` & `outsetapy-0.1.4/src/outsetapy/models/billing/charge_summary.py`

 * *Files identical despite different names*

### Comparing `outsetapy-0.1.3/src/outsetapy/models/billing/invoice_line_item.py` & `outsetapy-0.1.4/src/outsetapy/models/billing/invoice_line_item.py`

 * *Files identical despite different names*

### Comparing `outsetapy-0.1.3/src/outsetapy/models/billing/plan.py` & `outsetapy-0.1.4/src/outsetapy/models/billing/plan.py`

 * *Files identical despite different names*

### Comparing `outsetapy-0.1.3/src/outsetapy/models/billing/subscription_add_on.py` & `outsetapy-0.1.4/src/outsetapy/models/billing/subscription_add_on.py`

 * *Files identical despite different names*

### Comparing `outsetapy-0.1.3/src/outsetapy/models/billing/transaction.py` & `outsetapy-0.1.4/src/outsetapy/models/billing/transaction.py`

 * *Files identical despite different names*

### Comparing `outsetapy-0.1.3/src/outsetapy/models/billing/usage_item.py` & `outsetapy-0.1.4/src/outsetapy/models/billing/usage_item.py`

 * *Files identical despite different names*

### Comparing `outsetapy-0.1.3/src/outsetapy/models/crm/account.py` & `outsetapy-0.1.4/src/outsetapy/models/crm/account.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,37 +1,25 @@
 from datetime import datetime
+import importlib
+from outsetapy.util.store import Store
 from outsetapy.models.shared.address import Address
-
-
-class Deal:
-    def __init__(self, deal_id: str, deal_name: str):
-        self.deal_id = deal_id
-        self.deal_name = deal_name
-
-
-class PersonAccount:
-    def __init__(self, person_id: str, person_name: str):
-        self.person_id = person_id
-        self.person_name = person_name
-
-
-class AccountStage:
-    def __init__(self, stage_id: str, stage_name: str):
-        self.stage_id = stage_id
-        self.stage_name = stage_name
+from .deal import Deal
+from .person_account import PersonAccount
+from .account_stage import AccountStage
 
 
 class Subscription:
     def __init__(self, subscription_id: str, subscription_name: str):
         self.subscription_id = subscription_id
         self.subscription_name = subscription_name
 
 
 class Account:
-    def __init__(self, data: object):
+    def __init__(self, data: object, store: Store):
+        self.__store = store
         self.Name = None
         self.ClientIdentifier = None
         self.IsDemo = False
         self.BillingAddress = Address("", "", "", "")
         self.MailingAddress = Address("", "", "", "")
         self.AccountStage = AccountStage("", "")
         self.PaymentInformation = None
@@ -45,15 +33,14 @@
         self.AccountSpecificPageUrl4 = ""
         self.AccountSpecificPageUrl5 = ""
         self.RewardFulReferralId = None
         self.HasLoggedIn = False
         self.AccountStageLabel = ""
         self.DomainName = None
         self.LatestSubscription = None
-        self.CurrentSubscription = None
         self.PrimaryContact = None
         self.PrimarySubscription = None
         self.RecaptchaToken = None
         self.LifetimeRevenue = 0
         self.Uid = ""
         self.Created = datetime.now()
         self.Updated = datetime.now()
@@ -77,17 +64,26 @@
             self.AccountSpecificPageUrl4 = data["AccountSpecificPageUrl4"]
             self.AccountSpecificPageUrl5 = data["AccountSpecificPageUrl5"]
             self.RewardFulReferralId = data["RewardFulReferralId"]
             self.HasLoggedIn = data["HasLoggedIn"]
             self.AccountStageLabel = data["AccountStageLabel"]
             self.DomainName = data["DomainName"]
             self.LatestSubscription = data["LatestSubscription"]
-            self.CurrentSubscription = data["CurrentSubscription"]
+            if "CurrentSubscription" in data and data["CurrentSubscription"] and "Uid" in data["CurrentSubscription"]:
+                self._current_subscription = data["CurrentSubscription"]['Uid']
+            else:
+                self._current_subscription = None
             self.PrimaryContact = data["PrimaryContact"]
             self.PrimarySubscription = data["PrimarySubscription"]
             self.RecaptchaToken = data["RecaptchaToken"]
             self.LifetimeRevenue = data["LifetimeRevenue"]
             self.Uid = data["Uid"]
             self.Created = data["Created"]
             self.Updated = data["Updated"]
         elif "_objectType" in data:
             raise Exception(f"Invalid object type: {data['_objectType']}")
+        
+    @property
+    async def CurrentSubscription(self):
+        subscription_api = importlib.import_module("outsetapy.api.billing.subscriptions").Subscriptions(self.__store)
+        CurrentSubscription = await subscription_api.get(self._current_subscription)
+        return CurrentSubscription
```

### Comparing `outsetapy-0.1.3/src/outsetapy/models/crm/activity.py` & `outsetapy-0.1.4/src/outsetapy/models/crm/activity.py`

 * *Files identical despite different names*

### Comparing `outsetapy-0.1.3/src/outsetapy/models/crm/activity_type.py` & `outsetapy-0.1.4/src/outsetapy/models/crm/activity_type.py`

 * *Files identical despite different names*

### Comparing `outsetapy-0.1.3/src/outsetapy/models/crm/deal.py` & `outsetapy-0.1.4/src/outsetapy/models/crm/deal.py`

 * *Files identical despite different names*

### Comparing `outsetapy-0.1.3/src/outsetapy/models/crm/deal_person.py` & `outsetapy-0.1.4/src/outsetapy/models/crm/deal_person.py`

 * *Files identical despite different names*

### Comparing `outsetapy-0.1.3/src/outsetapy/models/crm/deal_pipeline_stage.py` & `outsetapy-0.1.4/src/outsetapy/models/crm/deal_pipeline_stage.py`

 * *Files identical despite different names*

### Comparing `outsetapy-0.1.3/src/outsetapy/models/crm/person.py` & `outsetapy-0.1.4/src/outsetapy/models/crm/person.py`

 * *Files identical despite different names*

### Comparing `outsetapy-0.1.3/src/outsetapy/models/crm/person_account.py` & `outsetapy-0.1.4/src/outsetapy/models/crm/person_account.py`

 * *Files identical despite different names*

### Comparing `outsetapy-0.1.3/src/outsetapy/models/marketing/email_list_person.py` & `outsetapy-0.1.4/src/outsetapy/models/marketing/email_list_person.py`

 * *Files identical despite different names*

### Comparing `outsetapy-0.1.3/src/outsetapy/models/marketing/emaillist.py` & `outsetapy-0.1.4/src/outsetapy/models/marketing/emaillist.py`

 * *Files identical despite different names*

### Comparing `outsetapy-0.1.3/src/outsetapy/models/shared/address.py` & `outsetapy-0.1.4/src/outsetapy/models/shared/address.py`

 * *Files identical despite different names*

### Comparing `outsetapy-0.1.3/src/outsetapy/models/support/case.py` & `outsetapy-0.1.4/src/outsetapy/models/support/case.py`

 * *Files identical despite different names*

### Comparing `outsetapy-0.1.3/src/outsetapy/models/support/case_history.py` & `outsetapy-0.1.4/src/outsetapy/models/support/case_history.py`

 * *Files identical despite different names*

### Comparing `outsetapy-0.1.3/src/outsetapy/models/wrappers/validation_error.py` & `outsetapy-0.1.4/src/outsetapy/models/wrappers/validation_error.py`

 * *Files identical despite different names*

### Comparing `outsetapy-0.1.3/src/outsetapy/util/credentials.py` & `outsetapy-0.1.4/src/outsetapy/util/credentials.py`

 * *Files identical despite different names*

### Comparing `outsetapy-0.1.3/src/outsetapy/util/request.py` & `outsetapy-0.1.4/src/outsetapy/util/request.py`

 * *Files identical despite different names*

### Comparing `outsetapy-0.1.3/src/outsetapy.egg-info/SOURCES.txt` & `outsetapy-0.1.4/src/outsetapy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

