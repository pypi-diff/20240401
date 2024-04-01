# Comparing `tmp/latynkatar-1.1.2.tar.gz` & `tmp/latynkatar-1.1.3.tar.gz`

## Comparing `latynkatar-1.1.2.tar` & `latynkatar-1.1.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0      757 2020-02-02 00:00:00.000000 latynkatar-1.1.2/Makefile
--rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 latynkatar-1.1.2/build-requirements.txt
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 latynkatar-1.1.2/requirements.txt
--rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 latynkatar-1.1.2/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 latynkatar-1.1.2/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0     1358 2020-02-02 00:00:00.000000 latynkatar-1.1.2/.github/workflows/code-tests.yml
--rw-r--r--   0        0        0     2099 2020-02-02 00:00:00.000000 latynkatar-1.1.2/.github/workflows/python-package.yml
--rw-r--r--   0        0        0      937 2020-02-02 00:00:00.000000 latynkatar-1.1.2/src/latynkatar/__init__.py
--rw-r--r--   0        0        0     4353 2020-02-02 00:00:00.000000 latynkatar-1.1.2/src/latynkatar/latynkatar.py
--rw-r--r--   0        0        0     1736 2020-02-02 00:00:00.000000 latynkatar-1.1.2/src/latynkatar/variables.py
--rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 latynkatar-1.1.2/tests/test_halosnyja.py
--rw-r--r--   0        0        0     5121 2020-02-02 00:00:00.000000 latynkatar-1.1.2/tests/test_tekst.py
--rw-r--r--   0        0        0     1186 2020-02-02 00:00:00.000000 latynkatar-1.1.2/tests/test_zyćnyja.py
--rw-r--r--   0        0        0   565399 2020-02-02 00:00:00.000000 latynkatar-1.1.2/tests/data/novaja_ziamla.txt
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 latynkatar-1.1.2/.gitignore
--rw-r--r--   0        0        0     7652 2020-02-02 00:00:00.000000 latynkatar-1.1.2/LICENSE
--rw-r--r--   0        0        0     2328 2020-02-02 00:00:00.000000 latynkatar-1.1.2/README.md
--rw-r--r--   0        0        0      949 2020-02-02 00:00:00.000000 latynkatar-1.1.2/pyproject.toml
--rw-r--r--   0        0        0     3217 2020-02-02 00:00:00.000000 latynkatar-1.1.2/PKG-INFO
+-rw-r--r--   0        0        0      779 2020-02-02 00:00:00.000000 latynkatar-1.1.3/Makefile
+-rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 latynkatar-1.1.3/build-requirements.txt
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 latynkatar-1.1.3/requirements.txt
+-rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 latynkatar-1.1.3/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 latynkatar-1.1.3/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0     1358 2020-02-02 00:00:00.000000 latynkatar-1.1.3/.github/workflows/code-tests.yml
+-rw-r--r--   0        0        0     2099 2020-02-02 00:00:00.000000 latynkatar-1.1.3/.github/workflows/python-package.yml
+-rw-r--r--   0        0        0      937 2020-02-02 00:00:00.000000 latynkatar-1.1.3/src/latynkatar/__init__.py
+-rw-r--r--   0        0        0     4003 2020-02-02 00:00:00.000000 latynkatar-1.1.3/src/latynkatar/latynkatar.py
+-rw-r--r--   0        0        0     1746 2020-02-02 00:00:00.000000 latynkatar-1.1.3/src/latynkatar/variables.py
+-rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 latynkatar-1.1.3/tests/test_halosnyja.py
+-rw-r--r--   0        0        0     5077 2020-02-02 00:00:00.000000 latynkatar-1.1.3/tests/test_tekst.py
+-rw-r--r--   0        0        0     1167 2020-02-02 00:00:00.000000 latynkatar-1.1.3/tests/test_zyćnyja.py
+-rw-r--r--   0        0        0   565399 2020-02-02 00:00:00.000000 latynkatar-1.1.3/tests/data/novaja_ziamla.txt
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 latynkatar-1.1.3/.gitignore
+-rw-r--r--   0        0        0     7652 2020-02-02 00:00:00.000000 latynkatar-1.1.3/LICENSE
+-rw-r--r--   0        0        0     2328 2020-02-02 00:00:00.000000 latynkatar-1.1.3/README.md
+-rw-r--r--   0        0        0      950 2020-02-02 00:00:00.000000 latynkatar-1.1.3/pyproject.toml
+-rw-r--r--   0        0        0     3217 2020-02-02 00:00:00.000000 latynkatar-1.1.3/PKG-INFO
```

### Comparing `latynkatar-1.1.2/Makefile` & `latynkatar-1.1.3/Makefile`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 venv:
 	python3 -m venv venv
 	./venv/bin/python3 -m pip install -r requirements.txt
 	
 test:
-	python3 -m pytest tests -lvv -ra
+	python3 -m pytest tests -lvv -ra --junitxml=output.xml
 
 test-env:
 	python3 -m venv test-venv
 	./test-venv/bin/python3 -m pip install -r requirements.txt
 
 package_test : test-env
 	./test-venv/bin/python3 -m pip install dist/*.whl
```

### Comparing `latynkatar-1.1.2/.github/ISSUE_TEMPLATE/bug_report.md` & `latynkatar-1.1.3/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `latynkatar-1.1.2/.github/ISSUE_TEMPLATE/feature_request.md` & `latynkatar-1.1.3/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `latynkatar-1.1.2/.github/workflows/code-tests.yml` & `latynkatar-1.1.3/.github/workflows/code-tests.yml`

 * *Files identical despite different names*

### Comparing `latynkatar-1.1.2/.github/workflows/python-package.yml` & `latynkatar-1.1.3/.github/workflows/python-package.yml`

 * *Files identical despite different names*

### Comparing `latynkatar-1.1.2/src/latynkatar/__init__.py` & `latynkatar-1.1.3/src/latynkatar/__init__.py`

 * *Files identical despite different names*

### Comparing `latynkatar-1.1.2/src/latynkatar/latynkatar.py` & `latynkatar-1.1.3/src/latynkatar/latynkatar.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 """
 
 from .variables import (
     PRAVILY_KANVERTACYJ,
     HALOSNYJA,
     PRAVILY_KANVERTACYJ_Z_J,
     MOHUC_PAZNACZACCA_JAK_MIAKKIJA,
-    KLASICZNYJA_PRAWILY_KANVERTACYJI
+    KLASICZNYJA_PRAWILY_KANVERTACYJI,
 )
 
 
 def karvertavac_z_j(current_letter: str, previous_letter: str) -> str:
     if (
         not previous_letter
         or previous_letter.lower() in HALOSNYJA
@@ -43,77 +43,74 @@
     if (
         current_letter.lower() != "і"
         and previous_letter
         and previous_letter.lower() == "л"
     ):
         base = ""
 
-    converted_letter = set_correct_case(base + second_letter, current_letter)
+    converted_letter = base + second_letter
 
     return converted_letter
 
 
-def set_correct_case(converted_letter: str, current_letter: str) -> str:
-    return (
-        converted_letter if current_letter.islower() else converted_letter.capitalize()
-    )
-
-    
-def convert(text: str, classic:bool = False) -> str:
+def convert(text: str, classic: bool = False) -> str:
     converted_text = ""
     text_length = len(text)
+    biahuczyja_pravily = (
+        KLASICZNYJA_PRAWILY_KANVERTACYJI if classic else PRAVILY_KANVERTACYJ
+    )
     for index, current_letter in enumerate(text):
         converted_letter = ""
         if index > 0:
             previous_letter = text[index - 1]
         else:
             previous_letter = None
 
         if index < text_length - 1:
             next_letter = text[index + 1]
         else:
             next_letter = None
 
-        if current_letter.lower() in PRAVILY_KANVERTACYJ:
-            if classic:
-                converted_letter = KLASICZNYJA_PRAWILY_KANVERTACYJI[current_letter.lower()]
-            else:
-                converted_letter = PRAVILY_KANVERTACYJ[current_letter.lower()]
-
-            converted_letter = set_correct_case(converted_letter, current_letter)
+        if current_letter.lower() in biahuczyja_pravily:
+            converted_letter = biahuczyja_pravily[current_letter.lower()]
         elif current_letter.lower() == "л":
             if next_letter and next_letter.lower() in ("ь", "л") + tuple(
                 PRAVILY_KANVERTACYJ_Z_J.keys()
             ):
-                converted_letter = set_correct_case("l", current_letter)
+                converted_letter = "l"
             else:
-                converted_letter = set_correct_case("ł", current_letter)
+                converted_letter = "ł"
         # могуць змякчацца асобна ад галосных літар пасля іх (мяккі знак)
         elif current_letter.lower() in MOHUC_PAZNACZACCA_JAK_MIAKKIJA:
             hard, soft = MOHUC_PAZNACZACCA_JAK_MIAKKIJA[current_letter.lower()]
             if next_letter and next_letter.lower() == "ь":
-                converted_letter = set_correct_case(soft, current_letter)
+                converted_letter = soft
             else:
-                converted_letter = set_correct_case(hard, current_letter)
+                converted_letter = hard
         elif current_letter.lower() == "х":
-            converted_letter = set_correct_case("ch", current_letter)
+            converted_letter = "ch"
         elif current_letter.lower() == "ь" or current_letter.lower() == "'":
             pass
         # Перадаюцца праз i/j
         elif current_letter.lower() in PRAVILY_KANVERTACYJ_Z_J:
             converted_letter = karvertavac_z_j(current_letter, previous_letter)
         else:
             converted_letter = current_letter
 
+        converted_letter = (
+            converted_letter
+            if current_letter.islower()
+            else converted_letter.capitalize()
+        )
         converted_text += converted_letter
 
     return converted_text
 
 
 class Cyr2Lat:
     @classmethod
     def convert(cls, text: str) -> str:
         return convert(text=text, classic=False)
-    
+
     @classmethod
     def convert_classic(cls, text: str) -> str:
         return convert(text=text, classic=True)
```

### Comparing `latynkatar-1.1.2/src/latynkatar/variables.py` & `latynkatar-1.1.3/src/latynkatar/variables.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,20 +45,22 @@
     "р": "r",
     "т": "t",
     "ф": "f",
     "ч": "č",
     "ш": "š",
 }
 KLASICZNYJA_PRAWILY_KANVERTACYJI = dict(PRAVILY_KANVERTACYJ)
-KLASICZNYJA_PRAWILY_KANVERTACYJI.update({
+KLASICZNYJA_PRAWILY_KANVERTACYJI.update(
+    {
         "ч": "cz",
         "ш": "sz",
         "ж": "ż",
         "в": "w",
-})
+    }
+)
 PRAVILY_KANVERTACYJ_Z_J = {
     "е": "e",
     "ё": "o",
     "і": "",
     "ю": "u",
     "я": "a",
 }
```

### Comparing `latynkatar-1.1.2/tests/test_tekst.py` & `latynkatar-1.1.3/tests/test_tekst.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # Try to import from module, else import from the source code
 try:
     from latynkatar import Cyr2Lat
 except ModuleNotFoundError:
     from src.latynkatar import Cyr2Lat
-    
+
 from time import monotonic
 
 # Узор узяты з часопіса PAMYŁKA:
 # https://github.com/PAMYLKA-ZIN/pamylka-number-3/tree/main/PAMYLKA_ZIN_3_FOR_SHARING
 PRYKŁAD_PAMYŁKA = """Вітаем цябе, чытачу!
 Гэта трэці нумар PAMYŁKA ZIN!
 Мы вельмі цешымся, што да каманды стваральнікаў працягваюць далучацца
@@ -123,25 +123,25 @@
     assert Cyr2Lat.convert_classic(PRYKŁAD_BAHDANOVIČ) == UZOR_BAHDANOVIČ_KLASICZNY
 
 
 def test_novaj_ziamloju():
     start = monotonic()
     _ = Cyr2Lat.convert(NOVAJA_ZIAMLA)
     finish = monotonic()
-    
+
     time_required = finish - start
-    
+
     print(start, finish, time_required)
-    
+
     assert time_required < 0.5
-        
-        
+
+
 def test_novaj_ziamloju_klasicny():
     start = monotonic()
     _ = Cyr2Lat.convert_classic(NOVAJA_ZIAMLA)
     finish = monotonic()
-    
+
     time_required = finish - start
-    
+
     print(start, finish, time_required)
-    
+
     assert time_required < 0.5
```

### Comparing `latynkatar-1.1.2/tests/test_zyćnyja.py` & `latynkatar-1.1.3/tests/test_zyćnyja.py`

 * *Files 20% similar despite different names*

```diff
@@ -3,34 +3,43 @@
     from latynkatar import Cyr2Lat
 except ModuleNotFoundError:
     from src.latynkatar import Cyr2Lat
 
 
 def test_l():
     assert Cyr2Lat.convert("ЛаЭлЯЛуЛіЛюЛЁлЕлЬ лЛя") == "ŁaElAŁuLiLuLOlEl lLa"
-    
+
+
 def test_ch():
     assert Cyr2Lat.convert("ХаХу ХЫВАХххххх Хіх") == "ChaChu ChYVAChchchchchch Chich"
-    
+
+
 def test_sz():
     assert Cyr2Lat.convert_classic("ШашуШышшшшшшш") == "SzaszuSzyszszszszszszsz"
 
+
 def test_š():
     assert Cyr2Lat.convert("ШашуШышшшшшшш") == "ŠašuŠyššššššš"
 
+
 def test_cz():
     assert Cyr2Lat.convert_classic("чАЧыЧУ") == "czACzyCzU"
-    
+
+
 def test_č():
     assert Cyr2Lat.convert("чАЧыЧУ") == "čAČyČU"
-    
+
+
 def test_ż():
     assert Cyr2Lat.convert_classic("жУрАвІнЫЖэЖЫ") == "żUrAwInYŻeŻY"
-    
+
+
 def test_ž():
     assert Cyr2Lat.convert("жУрАвІнЫЖэЖЫ") == "žUrAvInYŽeŽY"
-    
+
+
 def test_w():
     assert Cyr2Lat.convert_classic("войт і Ваявода") == "wojt i Wajawoda"
-    
+
+
 def test_v():
     assert Cyr2Lat.convert("войт і Ваявода") == "vojt i Vajavoda"
```

### Comparing `latynkatar-1.1.2/tests/data/novaja_ziamla.txt` & `latynkatar-1.1.3/tests/data/novaja_ziamla.txt`

 * *Files identical despite different names*

### Comparing `latynkatar-1.1.2/LICENSE` & `latynkatar-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `latynkatar-1.1.2/README.md` & `latynkatar-1.1.3/README.md`

 * *Files identical despite different names*

### Comparing `latynkatar-1.1.2/pyproject.toml` & `latynkatar-1.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "latynkatar"
-version = "1.1.2"
+version = "1.1.3"
 authors = [
   { name="Andrej Zacharevicz", email="zahar.by@gmail.com" },
 ]
 description = """EN: Simple and small package to convert belarussian cyrillic text to a modern (the one with ž, č, š and v) and classic (the one with ż, cz, sz and w) latin .
 
 BE: Просты і невялікі пакет для канвертацыі беларускай кірыліцы ў сучасную (з ž, č, š і v) і класічную (з ż, cz, sz і w) лацінку."""
 readme = "README.md"
@@ -17,8 +17,8 @@
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)",
     "Operating System :: OS Independent",
 ]
 
 [project.urls]
 Homepage = "https://github.com/measles/latynkatar"
-Issues = "https://github.com/measles/latynkatar/issues"
+Issues = "https://github.com/measles/latynkatar/issues"
```

### Comparing `latynkatar-1.1.2/PKG-INFO` & `latynkatar-1.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: latynkatar
-Version: 1.1.2
+Version: 1.1.3
 Summary: EN: Simple and small package to convert belarussian cyrillic text to a modern (the one with ž, č, š and v) and classic (the one with ż, cz, sz and w) latin .  BE: Просты і невялікі пакет для канвертацыі беларускай кірыліцы ў сучасную (з ž, č, š і v) і класічную (з ż, cz, sz і w) лацінку.
 Project-URL: Homepage, https://github.com/measles/latynkatar
 Project-URL: Issues, https://github.com/measles/latynkatar/issues
 Author-email: Andrej Zacharevicz <zahar.by@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Operating System :: OS Independent
```

