# Comparing `tmp/payconpy-1.0.0.tar.gz` & `tmp/payconpy-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "payconpy-1.0.0.tar", last modified: Thu Mar 28 20:10:45 2024, max compression
+gzip compressed data, was "payconpy-1.1.0.tar", last modified: Mon Apr  1 13:53:37 2024, max compression
```

## Comparing `payconpy-1.0.0.tar` & `payconpy-1.1.0.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxrwxrwx   0        0        0        0 2024-03-28 20:10:45.054792 payconpy-1.0.0/
--rw-rw-rw-   0        0        0     1073 2024-03-28 18:34:30.000000 payconpy-1.0.0/LICENSE
--rw-rw-rw-   0        0        0      889 2024-03-28 20:10:45.044696 payconpy-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0      446 2024-03-28 18:37:05.000000 payconpy-1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2024-03-28 20:10:44.602057 payconpy-1.0.0/payconpy/
-drwxrwxrwx   0        0        0        0 2024-03-28 20:10:44.680370 payconpy-1.0.0/payconpy/femails/
--rw-rw-rw-   0        0        0       40 2024-03-28 18:29:40.000000 payconpy-1.0.0/payconpy/femails/__init__.py
--rw-rw-rw-   0        0        0     7021 2024-03-28 18:29:45.000000 payconpy-1.0.0/payconpy/femails/femails.py
-drwxrwxrwx   0        0        0        0 2024-03-28 20:10:44.698132 payconpy-1.0.0/payconpy/fexceptions/
--rw-rw-rw-   0        0        0       18 2023-09-12 12:27:01.000000 payconpy-1.0.0/payconpy/fexceptions/__init__.py
--rw-rw-rw-   0        0        0      602 2023-09-12 12:27:01.000000 payconpy-1.0.0/payconpy/fexceptions/exceptions.py
-drwxrwxrwx   0        0        0        0 2024-03-28 20:10:44.706619 payconpy-1.0.0/payconpy/fpdf/
--rw-rw-rw-   0        0        0       18 2023-09-12 12:27:01.000000 payconpy-1.0.0/payconpy/fpdf/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-28 20:10:44.724974 payconpy-1.0.0/payconpy/fpdf/focr/
--rw-rw-rw-   0        0        0      104 2024-03-28 18:29:53.000000 payconpy-1.0.0/payconpy/fpdf/focr/__init__.py
--rw-rw-rw-   0        0        0    11098 2024-03-28 19:02:26.000000 payconpy-1.0.0/payconpy/fpdf/focr/orc.py
-drwxrwxrwx   0        0        0        0 2024-03-28 20:10:44.743449 payconpy-1.0.0/payconpy/fpdf/pdfutils/
--rw-rw-rw-   0        0        0       18 2023-09-12 12:27:01.000000 payconpy-1.0.0/payconpy/fpdf/pdfutils/__init__.py
--rw-rw-rw-   0        0        0     3310 2024-03-28 18:06:39.000000 payconpy-1.0.0/payconpy/fpdf/pdfutils/pdfutils.py
-drwxrwxrwx   0        0        0        0 2024-03-28 20:10:44.761856 payconpy-1.0.0/payconpy/fpysimplegui/
--rw-rw-rw-   0        0        0       83 2023-09-12 12:27:01.000000 payconpy-1.0.0/payconpy/fpysimplegui/__init__.py
--rw-rw-rw-   0        0        0     4676 2024-03-28 17:58:49.000000 payconpy-1.0.0/payconpy/fpysimplegui/fpysimplegui.py
-drwxrwxrwx   0        0        0        0 2024-03-28 20:10:44.779392 payconpy-1.0.0/payconpy/fpython/
--rw-rw-rw-   0        0        0       25 2023-09-12 12:27:01.000000 payconpy-1.0.0/payconpy/fpython/__init__.py
--rw-rw-rw-   0        0        0    56234 2024-03-28 17:58:09.000000 payconpy-1.0.0/payconpy/fpython/fpython.py
-drwxrwxrwx   0        0        0        0 2024-03-28 20:10:44.879289 payconpy-1.0.0/payconpy/fregex/
--rw-rw-rw-   0        0        0       24 2023-09-12 12:27:01.000000 payconpy-1.0.0/payconpy/fregex/__init__.py
--rw-rw-rw-   0        0        0    10366 2024-03-28 17:52:21.000000 payconpy-1.0.0/payconpy/fregex/fregex.py
-drwxrwxrwx   0        0        0        0 2024-03-28 20:10:44.912795 payconpy-1.0.0/payconpy/fselenium/
--rw-rw-rw-   0        0        0       27 2023-09-12 12:27:01.000000 payconpy-1.0.0/payconpy/fselenium/__init__.py
--rw-rw-rw-   0        0        0    38581 2024-03-28 18:02:45.000000 payconpy-1.0.0/payconpy/fselenium/fselenium.py
-drwxrwxrwx   0        0        0        0 2024-03-28 20:10:44.936874 payconpy-1.0.0/payconpy/openai/
--rw-rw-rw-   0        0        0        0 2023-11-27 12:53:25.000000 payconpy-1.0.0/payconpy/openai/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-28 20:10:44.957335 payconpy-1.0.0/payconpy/openai/assistants/
--rw-rw-rw-   0        0        0        0 2023-11-27 12:53:25.000000 payconpy-1.0.0/payconpy/openai/assistants/__init__.py
--rw-rw-rw-   0        0        0     4085 2023-11-27 13:03:14.000000 payconpy-1.0.0/payconpy/openai/assistants/assistants.py
--rw-rw-rw-   0        0        0     4427 2023-11-27 14:53:41.000000 payconpy-1.0.0/payconpy/openai/get_cost.py
-drwxrwxrwx   0        0        0        0 2024-03-28 20:10:45.016251 payconpy-1.0.0/payconpy/utils/
--rw-rw-rw-   0        0        0        0 2023-11-27 12:53:25.000000 payconpy-1.0.0/payconpy/utils/__init__.py
--rw-rw-rw-   0        0        0   133129 2024-03-28 18:54:30.000000 payconpy-1.0.0/payconpy/utils/utils.py
-drwxrwxrwx   0        0        0        0 2024-03-28 20:10:44.666697 payconpy-1.0.0/payconpy.egg-info/
--rw-rw-rw-   0        0        0      889 2024-03-28 20:10:44.000000 payconpy-1.0.0/payconpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      896 2024-03-28 20:10:44.000000 payconpy-1.0.0/payconpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-28 20:10:44.000000 payconpy-1.0.0/payconpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      217 2024-03-28 20:10:44.000000 payconpy-1.0.0/payconpy.egg-info/requires.txt
--rw-rw-rw-   0        0        0      226 2024-03-28 20:10:44.000000 payconpy-1.0.0/payconpy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-03-28 20:10:45.055795 payconpy-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0     1992 2024-03-28 19:46:51.000000 payconpy-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-01 13:53:37.181572 payconpy-1.1.0/
+-rw-rw-rw-   0        0        0     1073 2024-03-28 18:34:30.000000 payconpy-1.1.0/LICENSE
+-rw-rw-rw-   0        0        0      889 2024-04-01 13:53:37.178408 payconpy-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0      446 2024-03-28 18:37:05.000000 payconpy-1.1.0/README.md
+drwxrwxrwx   0        0        0        0 2024-04-01 13:53:36.999882 payconpy-1.1.0/payconpy/
+drwxrwxrwx   0        0        0        0 2024-04-01 13:53:37.055515 payconpy-1.1.0/payconpy/femails/
+-rw-rw-rw-   0        0        0       40 2024-03-28 18:29:40.000000 payconpy-1.1.0/payconpy/femails/__init__.py
+-rw-rw-rw-   0        0        0     7021 2024-03-28 18:29:45.000000 payconpy-1.1.0/payconpy/femails/femails.py
+drwxrwxrwx   0        0        0        0 2024-04-01 13:53:37.067155 payconpy-1.1.0/payconpy/fexceptions/
+-rw-rw-rw-   0        0        0       18 2023-09-12 12:27:01.000000 payconpy-1.1.0/payconpy/fexceptions/__init__.py
+-rw-rw-rw-   0        0        0      602 2023-09-12 12:27:01.000000 payconpy-1.1.0/payconpy/fexceptions/exceptions.py
+drwxrwxrwx   0        0        0        0 2024-04-01 13:53:37.072311 payconpy-1.1.0/payconpy/fpdf/
+-rw-rw-rw-   0        0        0       18 2023-09-12 12:27:01.000000 payconpy-1.1.0/payconpy/fpdf/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-01 13:53:37.082553 payconpy-1.1.0/payconpy/fpdf/focr/
+-rw-rw-rw-   0        0        0      104 2024-03-28 18:29:53.000000 payconpy-1.1.0/payconpy/fpdf/focr/__init__.py
+-rw-rw-rw-   0        0        0    11098 2024-03-28 19:02:26.000000 payconpy-1.1.0/payconpy/fpdf/focr/orc.py
+drwxrwxrwx   0        0        0        0 2024-04-01 13:53:37.093170 payconpy-1.1.0/payconpy/fpdf/pdfutils/
+-rw-rw-rw-   0        0        0       18 2023-09-12 12:27:01.000000 payconpy-1.1.0/payconpy/fpdf/pdfutils/__init__.py
+-rw-rw-rw-   0        0        0     3310 2024-03-28 18:06:39.000000 payconpy-1.1.0/payconpy/fpdf/pdfutils/pdfutils.py
+drwxrwxrwx   0        0        0        0 2024-04-01 13:53:37.103078 payconpy-1.1.0/payconpy/fpysimplegui/
+-rw-rw-rw-   0        0        0       83 2023-09-12 12:27:01.000000 payconpy-1.1.0/payconpy/fpysimplegui/__init__.py
+-rw-rw-rw-   0        0        0     4676 2024-03-28 17:58:49.000000 payconpy-1.1.0/payconpy/fpysimplegui/fpysimplegui.py
+drwxrwxrwx   0        0        0        0 2024-04-01 13:53:37.114686 payconpy-1.1.0/payconpy/fpython/
+-rw-rw-rw-   0        0        0       25 2023-09-12 12:27:01.000000 payconpy-1.1.0/payconpy/fpython/__init__.py
+-rw-rw-rw-   0        0        0    56234 2024-03-28 17:58:09.000000 payconpy-1.1.0/payconpy/fpython/fpython.py
+drwxrwxrwx   0        0        0        0 2024-04-01 13:53:37.126410 payconpy-1.1.0/payconpy/fregex/
+-rw-rw-rw-   0        0        0       24 2023-09-12 12:27:01.000000 payconpy-1.1.0/payconpy/fregex/__init__.py
+-rw-rw-rw-   0        0        0    10366 2024-03-28 17:52:21.000000 payconpy-1.1.0/payconpy/fregex/fregex.py
+drwxrwxrwx   0        0        0        0 2024-04-01 13:53:37.137122 payconpy-1.1.0/payconpy/fselenium/
+-rw-rw-rw-   0        0        0       27 2023-09-12 12:27:01.000000 payconpy-1.1.0/payconpy/fselenium/__init__.py
+-rw-rw-rw-   0        0        0    40190 2024-03-28 20:51:18.000000 payconpy-1.1.0/payconpy/fselenium/fselenium.py
+drwxrwxrwx   0        0        0        0 2024-04-01 13:53:37.148860 payconpy-1.1.0/payconpy/openai/
+-rw-rw-rw-   0        0        0        0 2023-11-27 12:53:25.000000 payconpy-1.1.0/payconpy/openai/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-01 13:53:37.156086 payconpy-1.1.0/payconpy/openai/assistants/
+-rw-rw-rw-   0        0        0        0 2023-11-27 12:53:25.000000 payconpy-1.1.0/payconpy/openai/assistants/__init__.py
+-rw-rw-rw-   0        0        0     4085 2023-11-27 13:03:14.000000 payconpy-1.1.0/payconpy/openai/assistants/assistants.py
+-rw-rw-rw-   0        0        0     4427 2023-11-27 14:53:41.000000 payconpy-1.1.0/payconpy/openai/get_cost.py
+drwxrwxrwx   0        0        0        0 2024-04-01 13:53:37.168823 payconpy-1.1.0/payconpy/utils/
+-rw-rw-rw-   0        0        0        0 2023-11-27 12:53:25.000000 payconpy-1.1.0/payconpy/utils/__init__.py
+-rw-rw-rw-   0        0        0   133129 2024-03-28 18:54:30.000000 payconpy-1.1.0/payconpy/utils/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-01 13:53:37.045467 payconpy-1.1.0/payconpy.egg-info/
+-rw-rw-rw-   0        0        0      889 2024-04-01 13:53:36.000000 payconpy-1.1.0/payconpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      896 2024-04-01 13:53:36.000000 payconpy-1.1.0/payconpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-01 13:53:36.000000 payconpy-1.1.0/payconpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      202 2024-04-01 13:53:36.000000 payconpy-1.1.0/payconpy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0      226 2024-04-01 13:53:36.000000 payconpy-1.1.0/payconpy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-01 13:53:37.182099 payconpy-1.1.0/setup.cfg
+-rw-rw-rw-   0        0        0     1945 2024-04-01 13:53:27.000000 payconpy-1.1.0/setup.py
```

### Comparing `payconpy-1.0.0/LICENSE` & `payconpy-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `payconpy-1.0.0/PKG-INFO` & `payconpy-1.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: payconpy
-Version: 1.0.0
+Version: 1.1.0
 Summary: Funções Para Melhorar Desenvolvimento de Robôs com Selenium
 Home-page: https://github.com/githubpaycon/payconpy
 Author: Paycon Automações
 Author-email: fernanda.yamamoto@paycon.com.br
 License: MIT License
 Keywords: Funções Para Melhorar Desenvolvimento de Robôs com Selenium
 Description-Content-Type: text/markdown
```

### Comparing `payconpy-1.0.0/payconpy/femails/femails.py` & `payconpy-1.1.0/payconpy/femails/femails.py`

 * *Files identical despite different names*

### Comparing `payconpy-1.0.0/payconpy/fexceptions/exceptions.py` & `payconpy-1.1.0/payconpy/fexceptions/exceptions.py`

 * *Files identical despite different names*

### Comparing `payconpy-1.0.0/payconpy/fpdf/focr/orc.py` & `payconpy-1.1.0/payconpy/fpdf/focr/orc.py`

 * *Files identical despite different names*

### Comparing `payconpy-1.0.0/payconpy/fpdf/pdfutils/pdfutils.py` & `payconpy-1.1.0/payconpy/fpdf/pdfutils/pdfutils.py`

 * *Files identical despite different names*

### Comparing `payconpy-1.0.0/payconpy/fpysimplegui/fpysimplegui.py` & `payconpy-1.1.0/payconpy/fpysimplegui/fpysimplegui.py`

 * *Files identical despite different names*

### Comparing `payconpy-1.0.0/payconpy/fpython/fpython.py` & `payconpy-1.1.0/payconpy/fpython/fpython.py`

 * *Files identical despite different names*

### Comparing `payconpy-1.0.0/payconpy/fregex/fregex.py` & `payconpy-1.1.0/payconpy/fregex/fregex.py`

 * *Files identical despite different names*

### Comparing `payconpy-1.0.0/payconpy/fselenium/fselenium.py` & `payconpy-1.1.0/payconpy/fselenium/fselenium.py`

 * *Files 2% similar despite different names*

```diff
@@ -991,7 +991,42 @@
     sleep(sleep_request)
     soup = BeautifulSoup(r.content, 'html5lib')
     if no_escape_sequence:
         return soup.find(tag_name).text.replace('\n', '').replace(u'\xa0', u' ')
     else:
         return soup.find(tag_name).text.replace(u'\xa0', u' ')
 
+def espera_input_limpa_e_envia_send_keys_action_chains(wdw:WebDriverWait, keys : str, locator : tuple, in_dom=False) -> None:
+    from selenium.common.exceptions import StaleElementReferenceException
+    """
+    ### Função espera pelo input ou textarea indicado pelo locator, limpa ele e envia os dados
+
+    Args:
+        driver (WebDriver): Seu webdriver
+        wdw (WebDriverWait): WebDriverWait criado em seu código
+        keys (str): Sua string para enviar no input ou textarea
+        locator (tuple): Tupla que contém a forma e o caminho do elemento (By.CSS_SELECTOR, '#myelementid')
+        click (bool): Clica ou não no elemento
+    """
+    driver = wdw._driver
+    try:
+        if in_dom:
+            wdw.until(EC.presence_of_element_located(locator))
+        else:
+            wdw.until(EC.element_to_be_clickable(locator))
+            
+        element = driver.find_element(By.CSS_SELECTOR, 'input[class*="rich-inslider-field-right rich-inslider-field"]')
+        ActionChains(driver).click(element).perform()
+        element.send_keys(Keys.CONTROL + "a")
+        element.send_keys(Keys.DELETE)
+        for char in keys:
+            element.send_keys(char)
+    except StaleElementReferenceException:
+        if in_dom:
+            wdw.until(EC.presence_of_element_located(locator))
+        else:
+            wdw.until(EC.element_to_be_clickable(locator))
+        ActionChains(driver).click(element).perform()
+        element.send_keys(Keys.CONTROL + "a")
+        element.send_keys(Keys.DELETE)
+        for char in keys:
+            element.send_keys(char)
```

### Comparing `payconpy-1.0.0/payconpy/openai/assistants/assistants.py` & `payconpy-1.1.0/payconpy/openai/assistants/assistants.py`

 * *Files identical despite different names*

### Comparing `payconpy-1.0.0/payconpy/openai/get_cost.py` & `payconpy-1.1.0/payconpy/openai/get_cost.py`

 * *Files identical despite different names*

### Comparing `payconpy-1.0.0/payconpy/utils/utils.py` & `payconpy-1.1.0/payconpy/utils/utils.py`

 * *Files identical despite different names*

### Comparing `payconpy-1.0.0/payconpy.egg-info/PKG-INFO` & `payconpy-1.1.0/payconpy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: payconpy
-Version: 1.0.0
+Version: 1.1.0
 Summary: Funções Para Melhorar Desenvolvimento de Robôs com Selenium
 Home-page: https://github.com/githubpaycon/payconpy
 Author: Paycon Automações
 Author-email: fernanda.yamamoto@paycon.com.br
 License: MIT License
 Keywords: Funções Para Melhorar Desenvolvimento de Robôs com Selenium
 Description-Content-Type: text/markdown
```

### Comparing `payconpy-1.0.0/payconpy.egg-info/SOURCES.txt` & `payconpy-1.1.0/payconpy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `payconpy-1.0.0/setup.py` & `payconpy-1.1.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import os
 from setuptools import setup
 
-version = '1.0.0'
+version = '1.1.0'
 
 with open("README.md", "r", encoding='utf-8') as fh:
     readme = fh.read()
     setup(
         name='payconpy',
         version=version,
         url='https://github.com/githubpaycon/payconpy',
@@ -36,23 +36,21 @@
             'selenium',
             'bs4',
             'requests',
             'html5lib',
             'webdriver-manager',
             'pretty-html-table',
             'PySimpleGUI==4.60.0',
-            'winotify',
             'xlsxwriter',
             'pandas',
             'sqlalchemy',
             'rich',
             'pyinstaller==5.12.0',
             # for ocr
             'opencv-python==4.8.1.78',
-            'gdown',
             'pytesseract',
             'PyMuPDF',
         ],
         extras_require={
             'openai': [ # for chatpdf
                 'openai',
             ],
```

