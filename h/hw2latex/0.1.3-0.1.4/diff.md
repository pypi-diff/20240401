# Comparing `tmp/hw2latex-0.1.3.tar.gz` & `tmp/hw2latex-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hw2latex-0.1.3.tar", max compression
+gzip compressed data, was "hw2latex-0.1.4.tar", max compression
```

## Comparing `hw2latex-0.1.3.tar` & `hw2latex-0.1.4.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0        0 2024-03-31 09:50:35.051839 hw2latex-0.1.3/hw2latex/__init__.py
--rw-r--r--   0        0        0     1322 2024-04-01 11:55:14.958135 hw2latex-0.1.3/hw2latex/hw2latex.py
--rw-r--r--   0        0        0      312 2024-04-01 12:07:31.672714 hw2latex-0.1.3/pyproject.toml
--rw-r--r--   0        0        0       31 2024-03-31 09:53:53.735976 hw2latex-0.1.3/README.md
--rw-r--r--   0        0        0      397 1970-01-01 00:00:00.000000 hw2latex-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-03-31 09:50:35.051839 hw2latex-0.1.4/hw2latex/__init__.py
+-rw-r--r--   0        0        0     1308 2024-04-01 12:18:10.878620 hw2latex-0.1.4/hw2latex/hw2latex.py
+-rw-r--r--   0        0        0      312 2024-04-01 12:20:47.157634 hw2latex-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0       31 2024-03-31 09:53:53.735976 hw2latex-0.1.4/README.md
+-rw-r--r--   0        0        0      397 1970-01-01 00:00:00.000000 hw2latex-0.1.4/PKG-INFO
```

### Comparing `hw2latex-0.1.3/hw2latex/hw2latex.py` & `hw2latex-0.1.4/hw2latex/hw2latex.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,23 +8,23 @@
     # Заполнение таблицы данными
     for row in data:
         latex_code += " & ".join(map(str, row)) + " \\\\ \n"
         latex_code += "\\hline\n"
 
     # Завершение таблицы
     latex_code += "\\end{tabular}\n"
-    latex_code += "\\caption{Пример таблицы}\n"
+    latex_code += "\\caption{Exemple_table}\n"
     latex_code += "\\label{tab:example}\n"
     latex_code += "\\end{table}\n"
 
     return latex_code
 
 
 def imagetolatex(image_path, caption='exemple_image'):
-    latex_code = f"""
+    latex_code = r"""
 \\begin{{figure}}
     \\centering
     \\includegraphics[width=0.5\textwidth]{{{image_path}}}
     \\caption{{{caption}}}
     \\label{{fig:image}}
 \\end{{figure}}
 """
```

