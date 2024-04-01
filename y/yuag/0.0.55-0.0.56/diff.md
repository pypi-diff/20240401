# Comparing `tmp/yuag-0.0.55.tar.gz` & `tmp/yuag-0.0.56.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yuag-0.0.55.tar", last modified: Fri Mar  8 22:39:54 2024, max compression
+gzip compressed data, was "yuag-0.0.56.tar", last modified: Mon Apr  1 19:46:57 2024, max compression
```

## Comparing `yuag-0.0.55.tar` & `yuag-0.0.56.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2024-03-08 22:39:54.176893 yuag-0.0.55/
--rw-rw-rw-   0        0        0       52 2024-03-08 22:39:54.173897 yuag-0.0.55/PKG-INFO
--rw-rw-rw-   0        0        0       42 2024-03-08 22:39:54.177890 yuag-0.0.55/setup.cfg
--rw-rw-rw-   0        0        0      249 2024-03-08 22:39:17.000000 yuag-0.0.55/setup.py
-drwxrwxrwx   0        0        0        0 2024-03-08 22:39:54.147909 yuag-0.0.55/yuag/
--rw-rw-rw-   0        0        0       19 2023-12-13 14:25:00.000000 yuag-0.0.55/yuag/__init__.py
--rw-rw-rw-   0        0        0    29873 2024-03-08 22:39:29.000000 yuag-0.0.55/yuag/yuag.py
-drwxrwxrwx   0        0        0        0 2024-03-08 22:39:54.170894 yuag-0.0.55/yuag.egg-info/
--rw-rw-rw-   0        0        0       52 2024-03-08 22:39:53.000000 yuag-0.0.55/yuag.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      150 2024-03-08 22:39:53.000000 yuag-0.0.55/yuag.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-08 22:39:53.000000 yuag-0.0.55/yuag.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2024-03-08 22:39:53.000000 yuag-0.0.55/yuag.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-01 19:46:57.559835 yuag-0.0.56/
+-rw-rw-rw-   0        0        0       52 2024-04-01 19:46:57.557836 yuag-0.0.56/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2024-04-01 19:46:57.560835 yuag-0.0.56/setup.cfg
+-rw-rw-rw-   0        0        0      249 2024-04-01 19:46:45.000000 yuag-0.0.56/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-01 19:46:57.521391 yuag-0.0.56/yuag/
+-rw-rw-rw-   0        0        0       19 2024-04-01 19:46:40.000000 yuag-0.0.56/yuag/__init__.py
+-rw-rw-rw-   0        0        0    32906 2024-04-01 19:46:33.000000 yuag-0.0.56/yuag/yuag.py
+drwxrwxrwx   0        0        0        0 2024-04-01 19:46:57.556839 yuag-0.0.56/yuag.egg-info/
+-rw-rw-rw-   0        0        0       52 2024-04-01 19:46:57.000000 yuag-0.0.56/yuag.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      150 2024-04-01 19:46:57.000000 yuag-0.0.56/yuag.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-01 19:46:57.000000 yuag-0.0.56/yuag.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2024-04-01 19:46:57.000000 yuag-0.0.56/yuag.egg-info/top_level.txt
```

### Comparing `yuag-0.0.55/yuag/yuag.py` & `yuag-0.0.56/yuag/yuag.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,32 +1,242 @@
+'''
+مكتبة yuag
+-----------------
+\n\n
+
+دليل لدوال المكتبة\n
+يمكنك الدخول على كل دالة لمعرفة تفاصيلها\n
+
+دوال عامة:
+-----------------
+```
+wait()
+clear()
+detect_lang()
+rangeNum()
+```
+\n\n
+
+دوال للملفات:
+-----------------
+```
+filesIn()
+rename_file()
+saveFile()
+readFile()
+readJSON()
+saveJson()
+savePdf()
+copy_file()
+move_file()
+delete_file()
+delete_folder()
+```
+\n\n
+
+دوال للمصفوفات:
+-----------------
+```
+equalArr()
+allIndexInArr()
+inArr()
+onSide()
+fillArr()
+removeFromArr()
+RemoveDuplicates()
+sumArr()
+minusArr()
+makeColumnArr()
+convertRowToCol()
+addArr()
+delArr()
+sliceArr()
+reverseArr()
+search2D()
+convert2D()
+rotate2DArr()
+insertInArr()
+convertTxt()
+searchIn_decodeNum()
+searchInObjArr()
+```
+\n\n
+
+دوال للقواميس:
+-----------------
+```
+equalObject()
+getObjectKeys()
+addToObject()
+```
+\n\n
+
+دوال لل json:
+-----------------
+```
+combine_json_files()
+uncombine_json_file()
+```
+\n\n
+
+دوال لملفات القراء:
+-----------------
+```
+combine_pdf_files()
+```
+\n\n
+
+دوال النصوص:
+-----------------
+```
+decodeNum()
+right()
+left()
+mid()
+split()
+removeSpaces()
+replaceText()
+```
+\n\n
+
+دوال للأرقام:
+-----------------
+```
+makeZeroNum()
+```
+\n\n
+
+دوال التقسيم:
+-----------------
+```
+separate_text()
+separate_arr()
+separate_obj()
+```
+\n\n
+
+دوال الترجمة:
+-----------------
+```
+translate_text()
+translate_arr()
+translate_obj()
+```
+\n\n
+
+دوال فصل هيكل الصفحة:
+-----------------
+```
+decode_html_in_text()
+decode_html_in_arr()
+decode_html_in_obj()
+```
+\n\n
+
+دوال لوحة المفاتيح:
+-----------------
+```
+write()
+press()
+unpress()
+```
+\n\n
+
+دوال الفارة:
+-----------------
+```
+getMousePosition()
+getMousePositions()
+click()
+right_click()
+move()
+```
+\n\n
+
+دوال ذكاء اصطناعي:
+-----------------
+```
+chatGPT()
+```
+\n\n
+
+دوال استخراج البينات من المواقع beautiful soup:
+-----------------
+```
+get_soup()
+get_redirected_url()
+innerText()
+innerHTML()
+```
+\n\n
+
+دوال استخراج البينات من المواقع selenium:
+-----------------
+```
+makeFirefoxDriver()
+driverToSoup()
+```
+\n\n
+
+دوال تحويل الملفات لروابط:
+-----------------
+```
+imageLink_to_dataurl()
+videoFile_to_dataurl()
+```
+\n\n
+
+رسالة الإنتهاء:
+-----------------
+```
+doneMessage()
+```
+'''
+
 import mouse
 import keyboard
 import requests
 from bs4 import BeautifulSoup
 from selenium import webdriver
 from selenium.webdriver.common.by import By
 import time
-from googletrans import Translator
-from langdetect import detect
 import os
 import json
 import re
 import base64
-import PyPDF2
-import openai
 import shutil
 
+
+
+# استدعاء المكتبات
+def PyPDF2():
+    import PyPDF2
+    return PyPDF2
+
+def Translator():
+    from googletrans import Translator
+    return Translator
+
+    from langdetect import detect
+
+def openai():
+    import openai
+    return openai
+
 # global defs
 def wait(wait_time: int = 1):
     time.sleep(wait_time)
 
 def clear():
     os.system("cls")
 
 def detect_lang(text: str, detectOrSrc: int = 0):
+    from googletrans import Translator
+    from langdetect import detect
+    
     try:
         if detectOrSrc == 0: return detect(text)
         else: return Translator().translate(text).src
     except:
         return 404
 
 def rangeNum(num, range_or_while_method = 0):
@@ -554,14 +764,16 @@
 
     # حفظ الملفات
     for key in combined_data:
         saveJson({key:combined_data[key]}, eval(files), indent, encoding)
 
 # pdf defs
 def combine_pdf_files(files_names: list, output_file_path: str, encoding: str = "utf-8"):
+    import PyPDF2
+
     merger = PyPDF2.PdfMerger()
 
     for pdf in files_names:
         merger.append(pdf)
 
     savePdf(merger, output_file_path, encoding)
 
@@ -710,14 +922,17 @@
         else:
             new_obj[key] = item
     
     return new_obj
 
 # translate defs
 def translate_text(text, target_language: str ="en", not_langs: list = [], detectOrSrc: int = 0):
+    from googletrans import Translator
+    from langdetect import detect
+    
     translator = Translator()
 
     if not_langs == []:
         if text:
             textArr = []
             for i in text.split("\n"):
                 if i != "":
@@ -874,14 +1089,17 @@
 # keyboard defs
 def write(text: str, delay: float = 0, restore_state_after: bool = True, exact: bool | None = None):
     keyboard.write(text, delay, restore_state_after, exact)
 
 def press(hot_key):
     keyboard.press(hot_key)
 
+def unpress(hot_key):
+    keyboard.release(hot_key)
+
 # mouse defs
 def getMousePosition():
     return [mouse.get_position()[0], mouse.get_position()[1]]
 
 def getMousePositions(saveKey: str ="g", breakKey: str ="0"):
     all = []
 
@@ -903,14 +1121,16 @@
     mouse.right_click()
 
 def move(x: int, y: int, absolute: bool = True, duration: int = 0):
     mouse.move(x, y, absolute, duration)
 
 # chatGPT
 def chatGPT(user_question: str, api_key: str):
+    import openai
+
     openai.api_key = api_key
 
     response = openai.ChatCompletion.create(
         model = "gpt-3.5-turbo",
         messages = [
             {
                 "role": "user",
```

