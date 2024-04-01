# Comparing `tmp/fredquery-0.0.48.tar.gz` & `tmp/fredquery-0.0.49.tar.gz`

## Comparing `fredquery-0.0.48.tar` & `fredquery-0.0.49.tar`

### file list

```diff
@@ -1,28 +1,26 @@
--rw-r--r--   0        0        0  4120769 2020-02-02 00:00:00.000000 fredquery-0.0.48/Ploteg0.ipynb
--rwxr-xr-x   0        0        0      417 2020-02-02 00:00:00.000000 fredquery-0.0.48/genusage.sh
--rw-r--r--   0        0        0     4131 2020-02-02 00:00:00.000000 fredquery-0.0.48/notes.txt
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 fredquery-0.0.48/requirements.txt
--rw-r--r--   0        0        0  4120769 2020-02-02 00:00:00.000000 fredquery-0.0.48/.ipynb_checkpoints/Ploteg0-checkpoint.ipynb
--rw-r--r--   0        0        0    20480 2020-02-02 00:00:00.000000 fredquery-0.0.48/src/fredquery/.fredplot.py.swp
--rw-r--r--   0        0        0    20480 2020-02-02 00:00:00.000000 fredquery-0.0.48/src/fredquery/.fredplotseries.py.swp
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 fredquery-0.0.48/src/fredquery/__about__.py
--rw-r--r--   0        0        0      334 2020-02-02 00:00:00.000000 fredquery-0.0.48/src/fredquery/__init__.py
--rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 fredquery-0.0.48/src/fredquery/aa2csv.py
--rw-r--r--   0        0        0     2701 2020-02-02 00:00:00.000000 fredquery-0.0.48/src/fredquery/aa2html.py
--rw-r--r--   0        0        0    11541 2020-02-02 00:00:00.000000 fredquery-0.0.48/src/fredquery/fredcategories.py
--rw-r--r--   0        0        0     4201 2020-02-02 00:00:00.000000 fredquery-0.0.48/src/fredquery/fredplot.py
--rw-r--r--   0        0        0     5293 2020-02-02 00:00:00.000000 fredquery-0.0.48/src/fredquery/fredplotseries.py
--rw-r--r--   0        0        0    10143 2020-02-02 00:00:00.000000 fredquery-0.0.48/src/fredquery/fredreleases.py
--rw-r--r--   0        0        0    11104 2020-02-02 00:00:00.000000 fredquery-0.0.48/src/fredquery/fredseries.py
--rw-r--r--   0        0        0    12113 2020-02-02 00:00:00.000000 fredquery-0.0.48/src/fredquery/fredsources.py
--rw-r--r--   0        0        0     9449 2020-02-02 00:00:00.000000 fredquery-0.0.48/src/fredquery/fredtags.py
--rw-r--r--   0        0        0     1847 2020-02-02 00:00:00.000000 fredquery-0.0.48/src/fredquery/query.py
--rw-r--r--   0        0        0     1722 2020-02-02 00:00:00.000000 fredquery-0.0.48/src/fredquery/xmlstr2aa.py
--rwxr-xr-x   0        0        0     2546 2020-02-02 00:00:00.000000 fredquery-0.0.48/tests/p.sh
--rwxr-xr-x   0        0        0      341 2020-02-02 00:00:00.000000 fredquery-0.0.48/tests/plot.sh
--rwxr-xr-x   0        0        0      558 2020-02-02 00:00:00.000000 fredquery-0.0.48/tests/s.sh
--rwxr-xr-x   0        0        0     2228 2020-02-02 00:00:00.000000 fredquery-0.0.48/tests/x.sh
--rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 fredquery-0.0.48/LICENSE.txt
--rw-r--r--   0        0        0     7938 2020-02-02 00:00:00.000000 fredquery-0.0.48/README.md
--rw-r--r--   0        0        0     2419 2020-02-02 00:00:00.000000 fredquery-0.0.48/pyproject.toml
--rw-r--r--   0        0        0     8959 2020-02-02 00:00:00.000000 fredquery-0.0.48/PKG-INFO
+-rw-r--r--   0        0        0  4120769 2020-02-02 00:00:00.000000 fredquery-0.0.49/Ploteg0.ipynb
+-rwxr-xr-x   0        0        0      417 2020-02-02 00:00:00.000000 fredquery-0.0.49/genusage.sh
+-rw-r--r--   0        0        0     4131 2020-02-02 00:00:00.000000 fredquery-0.0.49/notes.txt
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 fredquery-0.0.49/requirements.txt
+-rw-r--r--   0        0        0  4120769 2020-02-02 00:00:00.000000 fredquery-0.0.49/.ipynb_checkpoints/Ploteg0-checkpoint.ipynb
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 fredquery-0.0.49/src/fredquery/__about__.py
+-rw-r--r--   0        0        0      334 2020-02-02 00:00:00.000000 fredquery-0.0.49/src/fredquery/__init__.py
+-rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 fredquery-0.0.49/src/fredquery/aa2csv.py
+-rw-r--r--   0        0        0     2701 2020-02-02 00:00:00.000000 fredquery-0.0.49/src/fredquery/aa2html.py
+-rw-r--r--   0        0        0    11541 2020-02-02 00:00:00.000000 fredquery-0.0.49/src/fredquery/fredcategories.py
+-rw-r--r--   0        0        0     4201 2020-02-02 00:00:00.000000 fredquery-0.0.49/src/fredquery/fredplot.py
+-rw-r--r--   0        0        0     5293 2020-02-02 00:00:00.000000 fredquery-0.0.49/src/fredquery/fredplotseries.py
+-rw-r--r--   0        0        0    10143 2020-02-02 00:00:00.000000 fredquery-0.0.49/src/fredquery/fredreleases.py
+-rw-r--r--   0        0        0    11104 2020-02-02 00:00:00.000000 fredquery-0.0.49/src/fredquery/fredseries.py
+-rw-r--r--   0        0        0    12113 2020-02-02 00:00:00.000000 fredquery-0.0.49/src/fredquery/fredsources.py
+-rw-r--r--   0        0        0     9601 2020-02-02 00:00:00.000000 fredquery-0.0.49/src/fredquery/fredtags.py
+-rw-r--r--   0        0        0     1847 2020-02-02 00:00:00.000000 fredquery-0.0.49/src/fredquery/query.py
+-rw-r--r--   0        0        0     1722 2020-02-02 00:00:00.000000 fredquery-0.0.49/src/fredquery/xmlstr2aa.py
+-rwxr-xr-x   0        0        0     2546 2020-02-02 00:00:00.000000 fredquery-0.0.49/tests/p.sh
+-rwxr-xr-x   0        0        0      341 2020-02-02 00:00:00.000000 fredquery-0.0.49/tests/plot.sh
+-rwxr-xr-x   0        0        0      558 2020-02-02 00:00:00.000000 fredquery-0.0.49/tests/s.sh
+-rwxr-xr-x   0        0        0     2228 2020-02-02 00:00:00.000000 fredquery-0.0.49/tests/x.sh
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 fredquery-0.0.49/LICENSE.txt
+-rw-r--r--   0        0        0     7938 2020-02-02 00:00:00.000000 fredquery-0.0.49/README.md
+-rw-r--r--   0        0        0     2419 2020-02-02 00:00:00.000000 fredquery-0.0.49/pyproject.toml
+-rw-r--r--   0        0        0     8959 2020-02-02 00:00:00.000000 fredquery-0.0.49/PKG-INFO
```

### Comparing `fredquery-0.0.48/Ploteg0.ipynb` & `fredquery-0.0.49/Ploteg0.ipynb`

 * *Files identical despite different names*

### Comparing `fredquery-0.0.48/notes.txt` & `fredquery-0.0.49/notes.txt`

 * *Files identical despite different names*

### Comparing `fredquery-0.0.48/.ipynb_checkpoints/Ploteg0-checkpoint.ipynb` & `fredquery-0.0.49/.ipynb_checkpoints/Ploteg0-checkpoint.ipynb`

 * *Files identical despite different names*

### Comparing `fredquery-0.0.48/src/fredquery/aa2html.py` & `fredquery-0.0.49/src/fredquery/aa2html.py`

 * *Files identical despite different names*

### Comparing `fredquery-0.0.48/src/fredquery/fredcategories.py` & `fredquery-0.0.49/src/fredquery/fredcategories.py`

 * *Files identical despite different names*

### Comparing `fredquery-0.0.48/src/fredquery/fredplot.py` & `fredquery-0.0.49/src/fredquery/fredplot.py`

 * *Files identical despite different names*

### Comparing `fredquery-0.0.48/src/fredquery/fredplotseries.py` & `fredquery-0.0.49/src/fredquery/fredplotseries.py`

 * *Files identical despite different names*

### Comparing `fredquery-0.0.48/src/fredquery/fredreleases.py` & `fredquery-0.0.49/src/fredquery/fredreleases.py`

 * *Files identical despite different names*

### Comparing `fredquery-0.0.48/src/fredquery/fredseries.py` & `fredquery-0.0.49/src/fredquery/fredseries.py`

 * *Files identical despite different names*

### Comparing `fredquery-0.0.48/src/fredquery/fredsources.py` & `fredquery-0.0.49/src/fredquery/fredsources.py`

 * *Files identical despite different names*

### Comparing `fredquery-0.0.48/src/fredquery/fredtags.py` & `fredquery-0.0.49/src/fredquery/fredtags.py`

 * *Files 2% similar despite different names*

```diff
@@ -210,14 +210,15 @@
         resp = self.uq.query(url)
         rstr = resp.read().decode('utf-8')
                #  print(rstr)
         aa = self.xa.xmlstr2aa(rstr)
         aa[0].append('url')
         for i in range(1, len(aa) ):
             id = aa[i][0]
+            id = re.sub(' ', '+', id) # some environments don't like spaces
             url = '%s?series_id=%s&api_key=FRED_API_KEY' % (self.tsurl, id)
             aa[i].append(url)
         self.tagdict[0] = aa
 
 def main():
 
     argp = argparse.ArgumentParser(description='collect and report stlouisfed.org FRED tags and/or their series')
@@ -265,14 +266,17 @@
                 fp = open(ofn, 'w')
             except Exception as e:
                 print('%s: %s' % (ofn, e) )
                 sys.exit()
 
     ft = FREDTags()
 
+    if args.tagname:
+        args.tagname = re.sub(' ', '+', args.tagname)
+
     if args.observations:
         if not args.directory:
             argp.print_help() 
             sys.exit()
         if args.tagname:
             ft.getseriesfortnm(args.tagname)
             ft.getandreportobservations(odir=args.directory)
```

### Comparing `fredquery-0.0.48/src/fredquery/query.py` & `fredquery-0.0.49/src/fredquery/query.py`

 * *Files identical despite different names*

### Comparing `fredquery-0.0.48/src/fredquery/xmlstr2aa.py` & `fredquery-0.0.49/src/fredquery/xmlstr2aa.py`

 * *Files identical despite different names*

### Comparing `fredquery-0.0.48/tests/p.sh` & `fredquery-0.0.49/tests/p.sh`

 * *Files identical despite different names*

### Comparing `fredquery-0.0.48/tests/s.sh` & `fredquery-0.0.49/tests/s.sh`

 * *Files identical despite different names*

### Comparing `fredquery-0.0.48/tests/x.sh` & `fredquery-0.0.49/tests/x.sh`

 * *Files identical despite different names*

### Comparing `fredquery-0.0.48/LICENSE.txt` & `fredquery-0.0.49/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `fredquery-0.0.48/README.md` & `fredquery-0.0.49/README.md`

 * *Files identical despite different names*

### Comparing `fredquery-0.0.48/pyproject.toml` & `fredquery-0.0.49/pyproject.toml`

 * *Files identical despite different names*

### Comparing `fredquery-0.0.48/PKG-INFO` & `fredquery-0.0.49/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fredquery
-Version: 0.0.48
+Version: 0.0.49
 Summary: Downloads various stlouisfed.org FRED files to CSV files and creates plots based on category, release, series, source, or tag
 Project-URL: Documentation, https://github.com/dfwcnj/fredquery#readme
 Project-URL: Issues, https://github.com/dfwcnj/fredquery/issues
 Project-URL: Source, https://github.com/dfwcnj/fredquery
 Author-email: Don Caldwell <dfwcnj@gmail.com>
 License-Expression: MIT
 License-File: LICENSE.txt
```

