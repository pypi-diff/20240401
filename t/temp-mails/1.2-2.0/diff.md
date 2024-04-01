# Comparing `tmp/temp_mails-1.2.tar.gz` & `tmp/temp_mails-2.0.tar.gz`

## Comparing `temp_mails-1.2.tar` & `temp_mails-2.0.tar`

### file list

```diff
@@ -1,25 +1,100 @@
--rw-r--r--   0        0        0      568 2020-02-02 00:00:00.000000 temp_mails-1.2/changelog
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 temp_mails-1.2/temp_mails/__init__.py
--rw-r--r--   0        0        0    45423 2020-02-02 00:00:00.000000 temp_mails-1.2/temp_mails/providers.py
--rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 temp_mails-1.2/tests/disposableemail_com.py
--rw-r--r--   0        0        0      513 2020-02-02 00:00:00.000000 temp_mails-1.2/tests/emailondeck_com.py
--rw-r--r--   0        0        0      669 2020-02-02 00:00:00.000000 temp_mails-1.2/tests/etempmail_net.py
--rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 temp_mails-1.2/tests/fakemail_net.py
--rw-r--r--   0        0        0      778 2020-02-02 00:00:00.000000 temp_mails-1.2/tests/generator_email.py
--rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 temp_mails-1.2/tests/internxt_doctcom.py
--rw-r--r--   0        0        0      513 2020-02-02 00:00:00.000000 temp_mails-1.2/tests/minuteinbox_com.py
--rw-r--r--   0        0        0      776 2020-02-02 00:00:00.000000 temp_mails-1.2/tests/mohamal_com.py
--rw-r--r--   0        0        0      779 2020-02-02 00:00:00.000000 temp_mails-1.2/tests/onesecmail_com.py
--rw-r--r--   0        0        0      779 2020-02-02 00:00:00.000000 temp_mails-1.2/tests/tempemail_email.py
--rw-r--r--   0        0        0      667 2020-02-02 00:00:00.000000 temp_mails-1.2/tests/tempmail_io.py
--rw-r--r--   0        0        0      513 2020-02-02 00:00:00.000000 temp_mails-1.2/tests/tempmail_org.py
--rw-r--r--   0        0        0      793 2020-02-02 00:00:00.000000 temp_mails-1.2/tests/tempmail_plus.py
--rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 temp_mails-1.2/tests/tempmailbox_com.py
--rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 temp_mails-1.2/tests/tenminemail_com.py
--rw-r--r--   0        0        0      383 2020-02-02 00:00:00.000000 temp_mails-1.2/tests/tenminuteemail_com.py
--rw-r--r--   0        0        0      408 2020-02-02 00:00:00.000000 temp_mails-1.2/tests/tenminutesemail_net.py
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 temp_mails-1.2/.gitignore
--rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 temp_mails-1.2/LICENSE
--rw-r--r--   0        0        0     2748 2020-02-02 00:00:00.000000 temp_mails-1.2/README.md
--rw-r--r--   0        0        0      769 2020-02-02 00:00:00.000000 temp_mails-1.2/pyproject.toml
--rw-r--r--   0        0        0     3388 2020-02-02 00:00:00.000000 temp_mails-1.2/PKG-INFO
+-rw-r--r--   0        0        0     2037 2020-02-02 00:00:00.000000 temp_mails-2.0/changelog
+-rw-r--r--   0        0        0     1975 2020-02-02 00:00:00.000000 temp_mails-2.0/temp_mails/__init__.py
+-rw-r--r--   0        0        0    34680 2020-02-02 00:00:00.000000 temp_mails-2.0/temp_mails/_constructors.py
+-rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 temp_mails-2.0/temp_mails/cloudtempmail_com.py
+-rw-r--r--   0        0        0      690 2020-02-02 00:00:00.000000 temp_mails-2.0/temp_mails/cryptogmail_com.py
+-rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 temp_mails-2.0/temp_mails/disposablemail_com.py
+-rw-r--r--   0        0        0     2368 2020-02-02 00:00:00.000000 temp_mails-2.0/temp_mails/emailondeck_com.py
+-rw-r--r--   0        0        0     2806 2020-02-02 00:00:00.000000 temp_mails-2.0/temp_mails/etempmail_com.py
+-rw-r--r--   0        0        0     1808 2020-02-02 00:00:00.000000 temp_mails-2.0/temp_mails/etempmail_net.py
+-rw-r--r--   0        0        0     1334 2020-02-02 00:00:00.000000 temp_mails-2.0/temp_mails/eztempmail_com.py
+-rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 temp_mails-2.0/temp_mails/fakemail_net.py
+-rw-r--r--   0        0        0     1893 2020-02-02 00:00:00.000000 temp_mails-2.0/temp_mails/fakermail_com.py
+-rw-r--r--   0        0        0     7434 2020-02-02 00:00:00.000000 temp_mails-2.0/temp_mails/generator_email.py
+-rw-r--r--   0        0        0     2903 2020-02-02 00:00:00.000000 temp_mails-2.0/temp_mails/guerillamail_com.py
+-rw-r--r--   0        0        0     1024 2020-02-02 00:00:00.000000 temp_mails-2.0/temp_mails/internxt_com.py
+-rw-r--r--   0        0        0     1693 2020-02-02 00:00:00.000000 temp_mails-2.0/temp_mails/luxusmail_org.py
+-rw-r--r--   0        0        0     4790 2020-02-02 00:00:00.000000 temp_mails-2.0/temp_mails/mail_tm.py
+-rw-r--r--   0        0        0     2801 2020-02-02 00:00:00.000000 temp_mails-2.0/temp_mails/mailhole_de.py
+-rw-r--r--   0        0        0     1661 2020-02-02 00:00:00.000000 temp_mails-2.0/temp_mails/mailtemp_uk.py
+-rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 temp_mails-2.0/temp_mails/minuteinbox_com.py
+-rw-r--r--   0        0        0     2656 2020-02-02 00:00:00.000000 temp_mails-2.0/temp_mails/mohamal_com.py
+-rw-r--r--   0        0        0     1692 2020-02-02 00:00:00.000000 temp_mails-2.0/temp_mails/mostakbile_com.py
+-rw-r--r--   0        0        0     4243 2020-02-02 00:00:00.000000 temp_mails-2.0/temp_mails/muellmail_com.py
+-rw-r--r--   0        0        0     1878 2020-02-02 00:00:00.000000 temp_mails-2.0/temp_mails/onesecmail_com.py
+-rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 temp_mails-2.0/temp_mails/tempail_com.py
+-rw-r--r--   0        0        0     1729 2020-02-02 00:00:00.000000 temp_mails-2.0/temp_mails/tempdashmail_gg.py
+-rw-r--r--   0        0        0     1769 2020-02-02 00:00:00.000000 temp_mails-2.0/temp_mails/tempemailfree_com.py
+-rw-r--r--   0        0        0     2692 2020-02-02 00:00:00.000000 temp_mails-2.0/temp_mails/tempinbox_com.py
+-rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 temp_mails-2.0/temp_mails/tempmail_email.py
+-rw-r--r--   0        0        0     1691 2020-02-02 00:00:00.000000 temp_mails-2.0/temp_mails/tempmail_gg.py
+-rw-r--r--   0        0        0     2285 2020-02-02 00:00:00.000000 temp_mails-2.0/temp_mails/tempmail_io.py
+-rw-r--r--   0        0        0     1710 2020-02-02 00:00:00.000000 temp_mails-2.0/temp_mails/tempmail_lol.py
+-rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 temp_mails-2.0/temp_mails/tempmail_net.py
+-rw-r--r--   0        0        0    11550 2020-02-02 00:00:00.000000 temp_mails-2.0/temp_mails/tempmail_ninja.py
+-rw-r--r--   0        0        0      444 2020-02-02 00:00:00.000000 temp_mails-2.0/temp_mails/tempmail_org.py
+-rw-r--r--   0        0        0     2043 2020-02-02 00:00:00.000000 temp_mails-2.0/temp_mails/tempmail_plus.py
+-rw-r--r--   0        0        0     2380 2020-02-02 00:00:00.000000 temp_mails-2.0/temp_mails/tempmailbox_com.py
+-rw-r--r--   0        0        0     4388 2020-02-02 00:00:00.000000 temp_mails-2.0/temp_mails/tempmails_net.py
+-rw-r--r--   0        0        0     3612 2020-02-02 00:00:00.000000 temp_mails-2.0/temp_mails/tempr_email.py
+-rw-r--r--   0        0        0      440 2020-02-02 00:00:00.000000 temp_mails-2.0/temp_mails/tenminemail_com.py
+-rw-r--r--   0        0        0     1187 2020-02-02 00:00:00.000000 temp_mails-2.0/temp_mails/tenminuteemail_com.py
+-rw-r--r--   0        0        0     1347 2020-02-02 00:00:00.000000 temp_mails-2.0/temp_mails/tenminutesemail_net.py
+-rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 temp_mails-2.0/temp_mails/tmail_ai.py
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 temp_mails-2.0/temp_mails/tmail_gg.py
+-rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 temp_mails-2.0/temp_mails/tmailor_com.py
+-rw-r--r--   0        0        0     2593 2020-02-02 00:00:00.000000 temp_mails-2.0/temp_mails/tmmail_com.py
+-rw-r--r--   0        0        0     4077 2020-02-02 00:00:00.000000 temp_mails-2.0/temp_mails/trashmail_com.py
+-rw-r--r--   0        0        0     1649 2020-02-02 00:00:00.000000 temp_mails-2.0/temp_mails/upxmail_com.py
+-rw-r--r--   0        0        0     4375 2020-02-02 00:00:00.000000 temp_mails-2.0/temp_mails/yopmail_com.py
+-rw-r--r--   0        0        0      517 2020-02-02 00:00:00.000000 temp_mails-2.0/tests/cloudtempmail_com.py
+-rw-r--r--   0        0        0      780 2020-02-02 00:00:00.000000 temp_mails-2.0/tests/cryptogmail_com.py
+-rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 temp_mails-2.0/tests/disposableemail_com.py
+-rw-r--r--   0        0        0      513 2020-02-02 00:00:00.000000 temp_mails-2.0/tests/emailondeck_com.py
+-rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 temp_mails-2.0/tests/etempmail_com.py
+-rw-r--r--   0        0        0      669 2020-02-02 00:00:00.000000 temp_mails-2.0/tests/etempmail_net.py
+-rw-r--r--   0        0        0      670 2020-02-02 00:00:00.000000 temp_mails-2.0/tests/eztempmail_com.py
+-rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 temp_mails-2.0/tests/fakemail_net.py
+-rw-r--r--   0        0        0      729 2020-02-02 00:00:00.000000 temp_mails-2.0/tests/fakermail_com.py
+-rw-r--r--   0        0        0      778 2020-02-02 00:00:00.000000 temp_mails-2.0/tests/generator_email.py
+-rw-r--r--   0        0        0      811 2020-02-02 00:00:00.000000 temp_mails-2.0/tests/guerillamail_com.py
+-rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 temp_mails-2.0/tests/internxt_com.py
+-rw-r--r--   0        0        0      669 2020-02-02 00:00:00.000000 temp_mails-2.0/tests/luxusmail_org.py
+-rw-r--r--   0        0        0      770 2020-02-02 00:00:00.000000 temp_mails-2.0/tests/mail_tm.py
+-rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 temp_mails-2.0/tests/mailhole_de.py
+-rw-r--r--   0        0        0      667 2020-02-02 00:00:00.000000 temp_mails-2.0/tests/mailtemp_uk.py
+-rw-r--r--   0        0        0      513 2020-02-02 00:00:00.000000 temp_mails-2.0/tests/minuteinbox_com.py
+-rw-r--r--   0        0        0      776 2020-02-02 00:00:00.000000 temp_mails-2.0/tests/mohamal_com.py
+-rw-r--r--   0        0        0      670 2020-02-02 00:00:00.000000 temp_mails-2.0/tests/mostakbile_com.py
+-rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 temp_mails-2.0/tests/muellmail_com.py
+-rw-r--r--   0        0        0      779 2020-02-02 00:00:00.000000 temp_mails-2.0/tests/onesecmail_com.py
+-rw-r--r--   0        0        0      511 2020-02-02 00:00:00.000000 temp_mails-2.0/tests/tempail_com.py
+-rw-r--r--   0        0        0      671 2020-02-02 00:00:00.000000 temp_mails-2.0/tests/tempdashmail_gg.py
+-rw-r--r--   0        0        0      673 2020-02-02 00:00:00.000000 temp_mails-2.0/tests/tempemailfree_com.py
+-rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 temp_mails-2.0/tests/tempinbox_com.py
+-rw-r--r--   0        0        0      779 2020-02-02 00:00:00.000000 temp_mails-2.0/tests/tempmail_email.py
+-rw-r--r--   0        0        0      667 2020-02-02 00:00:00.000000 temp_mails-2.0/tests/tempmail_gg.py
+-rw-r--r--   0        0        0      667 2020-02-02 00:00:00.000000 temp_mails-2.0/tests/tempmail_io.py
+-rw-r--r--   0        0        0      342 2020-02-02 00:00:00.000000 temp_mails-2.0/tests/tempmail_lol.py
+-rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 temp_mails-2.0/tests/tempmail_net.py
+-rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 temp_mails-2.0/tests/tempmail_ninja.py
+-rw-r--r--   0        0        0      513 2020-02-02 00:00:00.000000 temp_mails-2.0/tests/tempmail_org.py
+-rw-r--r--   0        0        0      793 2020-02-02 00:00:00.000000 temp_mails-2.0/tests/tempmail_plus.py
+-rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 temp_mails-2.0/tests/tempmailbox_com.py
+-rw-r--r--   0        0        0      778 2020-02-02 00:00:00.000000 temp_mails-2.0/tests/tempmails_net.py
+-rw-r--r--   0        0        0      806 2020-02-02 00:00:00.000000 temp_mails-2.0/tests/tempr_email.py
+-rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 temp_mails-2.0/tests/tenminemail_com.py
+-rw-r--r--   0        0        0      383 2020-02-02 00:00:00.000000 temp_mails-2.0/tests/tenminuteemail_com.py
+-rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 temp_mails-2.0/tests/tenminutesemail_net.py
+-rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 temp_mails-2.0/tests/tmail_ai.py
+-rw-r--r--   0        0        0      664 2020-02-02 00:00:00.000000 temp_mails-2.0/tests/tmail_gg.py
+-rw-r--r--   0        0        0      511 2020-02-02 00:00:00.000000 temp_mails-2.0/tests/tmailor_com.py
+-rw-r--r--   0        0        0      399 2020-02-02 00:00:00.000000 temp_mails-2.0/tests/tmmail_com.py
+-rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 temp_mails-2.0/tests/trashmail_com.py
+-rw-r--r--   0        0        0      667 2020-02-02 00:00:00.000000 temp_mails-2.0/tests/upxmail_com.py
+-rw-r--r--   0        0        0      806 2020-02-02 00:00:00.000000 temp_mails-2.0/tests/yopmail_com.py
+-rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 temp_mails-2.0/.gitignore
+-rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 temp_mails-2.0/LICENSE
+-rw-r--r--   0        0        0     4728 2020-02-02 00:00:00.000000 temp_mails-2.0/README.md
+-rw-r--r--   0        0        0      769 2020-02-02 00:00:00.000000 temp_mails-2.0/pyproject.toml
+-rw-r--r--   0        0        0     5332 2020-02-02 00:00:00.000000 temp_mails-2.0/PKG-INFO
```

### Comparing `temp_mails-1.2/tests/disposableemail_com.py` & `temp_mails-2.0/tests/disposableemail_com.py`

 * *Files identical despite different names*

### Comparing `temp_mails-1.2/tests/emailondeck_com.py` & `temp_mails-2.0/tests/emailondeck_com.py`

 * *Files identical despite different names*

### Comparing `temp_mails-1.2/tests/etempmail_net.py` & `temp_mails-2.0/tests/etempmail_net.py`

 * *Files identical despite different names*

### Comparing `temp_mails-1.2/tests/fakemail_net.py` & `temp_mails-2.0/tests/fakemail_net.py`

 * *Files identical despite different names*

### Comparing `temp_mails-1.2/tests/generator_email.py` & `temp_mails-2.0/tests/generator_email.py`

 * *Files identical despite different names*

### Comparing `temp_mails-1.2/tests/minuteinbox_com.py` & `temp_mails-2.0/tests/minuteinbox_com.py`

 * *Files identical despite different names*

### Comparing `temp_mails-1.2/tests/mohamal_com.py` & `temp_mails-2.0/tests/mohamal_com.py`

 * *Files identical despite different names*

### Comparing `temp_mails-1.2/tests/onesecmail_com.py` & `temp_mails-2.0/tests/onesecmail_com.py`

 * *Files identical despite different names*

### Comparing `temp_mails-1.2/tests/tempemail_email.py` & `temp_mails-2.0/tests/tempmail_email.py`

 * *Files identical despite different names*

### Comparing `temp_mails-1.2/tests/tempmail_io.py` & `temp_mails-2.0/tests/tempmail_io.py`

 * *Files identical despite different names*

### Comparing `temp_mails-1.2/tests/tempmail_org.py` & `temp_mails-2.0/tests/tempmail_org.py`

 * *Files identical despite different names*

### Comparing `temp_mails-1.2/tests/tempmail_plus.py` & `temp_mails-2.0/tests/tempmail_plus.py`

 * *Files identical despite different names*

### Comparing `temp_mails-1.2/LICENSE` & `temp_mails-2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `temp_mails-1.2/pyproject.toml` & `temp_mails-2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = [ "hatchling",]
 build-backend = "hatchling.build"
 
 [project]
 name = "temp-mails"
-version = "1.2"
+version = "2.0"
 description = "A basic wrapper around various temp mail sites, aiming to provide an almost identical api for every site. The main purpose of this is to provide an easy way to quickly register an account on various sites and then discard the email."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [ "Programming Language :: Python :: 3", "License :: OSI Approved :: MIT License", "Operating System :: OS Independent",]
 [[project.authors]]
 name = "bertigert"
 email = "bertiger@riseup.net"
```

