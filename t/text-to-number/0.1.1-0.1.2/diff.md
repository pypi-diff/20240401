# Comparing `tmp/text_to_number-0.1.1.tar.gz` & `tmp/text_to_number-0.1.2.tar.gz`

## Comparing `text_to_number-0.1.1.tar` & `text_to_number-0.1.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 text_to_number-0.1.1/src/text_to_number/__init__.py
--rw-r--r--   0        0        0     4425 2020-02-02 00:00:00.000000 text_to_number-0.1.1/src/text_to_number/core.py
--rw-r--r--   0        0        0     1980 2020-02-02 00:00:00.000000 text_to_number-0.1.1/.gitignore
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 text_to_number-0.1.1/LICENSE
--rw-r--r--   0        0        0      990 2020-02-02 00:00:00.000000 text_to_number-0.1.1/README.md
--rw-r--r--   0        0        0      876 2020-02-02 00:00:00.000000 text_to_number-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     3065 2020-02-02 00:00:00.000000 text_to_number-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 text_to_number-0.1.2/src/text_to_number/__init__.py
+-rw-r--r--   0        0        0     4470 2020-02-02 00:00:00.000000 text_to_number-0.1.2/src/text_to_number/core.py
+-rw-r--r--   0        0        0     1980 2020-02-02 00:00:00.000000 text_to_number-0.1.2/.gitignore
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 text_to_number-0.1.2/LICENSE
+-rw-r--r--   0        0        0      990 2020-02-02 00:00:00.000000 text_to_number-0.1.2/README.md
+-rw-r--r--   0        0        0      876 2020-02-02 00:00:00.000000 text_to_number-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     3065 2020-02-02 00:00:00.000000 text_to_number-0.1.2/PKG-INFO
```

### Comparing `text_to_number-0.1.1/src/text_to_number/core.py` & `text_to_number-0.1.2/src/text_to_number/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -91,15 +91,16 @@
                             current = 1
                         num += current * value
                         current = 0
                         
         num += current  # Add any remaining integer part
         num += decimal_fraction  # Add the decimal fraction part
         
-        return str(num)
+        return str(int(num)) if decimal_fraction == 0 else str(num)
+
 
     # Enhance the pattern to potentially match decimal expressions
     pattern = r'\b(' + '|'.join(english.keys()) + r'|\bpoint\b)(?:[\s-]+(' + '|'.join(english.keys()) + r'|\bpoint\b))*\b'
     regex = re.compile(pattern, re.IGNORECASE)
 
     new_text = regex.sub(convert_number_phrase_to_number, text)
     return new_text
```

### Comparing `text_to_number-0.1.1/.gitignore` & `text_to_number-0.1.2/.gitignore`

 * *Files identical despite different names*

### Comparing `text_to_number-0.1.1/LICENSE` & `text_to_number-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `text_to_number-0.1.1/README.md` & `text_to_number-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `text_to_number-0.1.1/pyproject.toml` & `text_to_number-0.1.2/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "text-to-number"
-version = "0.1.1"
+version = "0.1.2"
 description = "A package to convert text numbers into integers."
 authors = [
     {name = "Soham Padia", email = "sohampadia10@gmail.com"},
 ]
 license = {file = "LICENSE"}
 readme = "README.md"
 requires-python = ">=3.6"
```

### Comparing `text_to_number-0.1.1/PKG-INFO` & `text_to_number-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: text-to-number
-Version: 0.1.1
+Version: 0.1.2
 Summary: A package to convert text numbers into integers.
 Project-URL: homepage, https://github.com/soham-padia/textToInt
 Project-URL: repository, https://github.com/soham-padia/textToInt
 Project-URL: documentation, https://github.com/soham-padia/textToInt/wiki
 Author-email: Soham Padia <sohampadia10@gmail.com>
 License: MIT License
```

