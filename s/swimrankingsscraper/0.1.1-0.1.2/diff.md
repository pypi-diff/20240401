# Comparing `tmp/swimrankingsscraper-0.1.1.tar.gz` & `tmp/swimrankingsscraper-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "swimrankingsscraper-0.1.1.tar", last modified: Tue Jan 30 08:22:55 2024, max compression
+gzip compressed data, was "swimrankingsscraper-0.1.2.tar", last modified: Mon Apr  1 18:13:25 2024, max compression
```

## Comparing `swimrankingsscraper-0.1.1.tar` & `swimrankingsscraper-0.1.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 08:22:55.364193 swimrankingsscraper-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-01-30 08:22:40.000000 swimrankingsscraper-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      986 2024-01-30 08:22:55.364193 swimrankingsscraper-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      431 2024-01-30 08:22:40.000000 swimrankingsscraper-0.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-30 08:22:55.364193 swimrankingsscraper-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-01-30 08:22:40.000000 swimrankingsscraper-0.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 08:22:55.364193 swimrankingsscraper-0.1.1/swimrankingsscraper/
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-01-30 08:22:40.000000 swimrankingsscraper-0.1.1/swimrankingsscraper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    35325 2024-01-30 08:22:40.000000 swimrankingsscraper-0.1.1/swimrankingsscraper/swimrankingsscraper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 08:22:55.364193 swimrankingsscraper-0.1.1/swimrankingsscraper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      986 2024-01-30 08:22:55.000000 swimrankingsscraper-0.1.1/swimrankingsscraper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      349 2024-01-30 08:22:55.000000 swimrankingsscraper-0.1.1/swimrankingsscraper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-30 08:22:55.000000 swimrankingsscraper-0.1.1/swimrankingsscraper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-01-30 08:22:55.000000 swimrankingsscraper-0.1.1/swimrankingsscraper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-01-30 08:22:55.000000 swimrankingsscraper-0.1.1/swimrankingsscraper.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 08:22:55.364193 swimrankingsscraper-0.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    22660 2024-01-30 08:22:40.000000 swimrankingsscraper-0.1.1/tests/test_swimrankingsscraper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 18:13:25.322904 swimrankingsscraper-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-01 18:13:08.000000 swimrankingsscraper-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      986 2024-04-01 18:13:25.322904 swimrankingsscraper-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      431 2024-04-01 18:13:08.000000 swimrankingsscraper-0.1.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-01 18:13:25.322904 swimrankingsscraper-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-04-01 18:13:08.000000 swimrankingsscraper-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 18:13:25.322904 swimrankingsscraper-0.1.2/swimrankingsscraper/
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-01 18:13:08.000000 swimrankingsscraper-0.1.2/swimrankingsscraper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35478 2024-04-01 18:13:08.000000 swimrankingsscraper-0.1.2/swimrankingsscraper/swimrankingsscraper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 18:13:25.322904 swimrankingsscraper-0.1.2/swimrankingsscraper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      986 2024-04-01 18:13:25.000000 swimrankingsscraper-0.1.2/swimrankingsscraper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      349 2024-04-01 18:13:25.000000 swimrankingsscraper-0.1.2/swimrankingsscraper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 18:13:25.000000 swimrankingsscraper-0.1.2/swimrankingsscraper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-01 18:13:25.000000 swimrankingsscraper-0.1.2/swimrankingsscraper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-01 18:13:25.000000 swimrankingsscraper-0.1.2/swimrankingsscraper.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 18:13:25.322904 swimrankingsscraper-0.1.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    22660 2024-04-01 18:13:08.000000 swimrankingsscraper-0.1.2/tests/test_swimrankingsscraper.py
```

### Comparing `swimrankingsscraper-0.1.1/LICENSE` & `swimrankingsscraper-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `swimrankingsscraper-0.1.1/PKG-INFO` & `swimrankingsscraper-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swimrankingsscraper
-Version: 0.1.1
+Version: 0.1.2
 Summary: A scraper for swimrankings.net
 Home-page: https://swimrankingsscraper.readthedocs.io/
 Author: Bas Neeleman
 Author-email: bas@neeleman-mail.nl
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `swimrankingsscraper-0.1.1/setup.py` & `swimrankingsscraper-0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 with open(path.join(here, 'README.md')) as f:
     long_description = f.read()
 
 
 setup(
     name='swimrankingsscraper',
-    version='0.1.1',
+    version='0.1.2',
     description='A scraper for swimrankings.net',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://swimrankingsscraper.readthedocs.io/',
     author='Bas Neeleman',
     author_email='bas@neeleman-mail.nl',
     license='MIT',
```

### Comparing `swimrankingsscraper-0.1.1/swimrankingsscraper/swimrankingsscraper.py` & `swimrankingsscraper-0.1.2/swimrankingsscraper/swimrankingsscraper.py`

 * *Files 0% similar despite different names*

```diff
@@ -566,27 +566,29 @@
             tables = soup.find_all('table', {'class': 'meetResult'})
         except AttributeError:
             return []
         results = []
         for row in tables[race_id-1].find_all('tr', {'class': ['meetResult0', 'meetResult1']}):
             name_cell = row.find('td', {'class': 'name'})
             name = name_cell.find('a').get_text(strip=True)
+            name_url = name_cell.find('a')['href']
+            athlete_id = parse_qs(urlparse(name_url).query)['athleteId'][0]
             club_cell = row.find_all('td', {'class': 'name'})[1]
             club_name = club_cell.find('a').get_text(strip=True)
             time_cell = row.find('td', {'class': 'swimtime'})
             time = time_cell.find('a').get_text(strip=True)
             try:
                 split_times_rough = time_cell.find('a')['onmouseover']
             except KeyError:
                 split_times_rough = ""
             pattern = r"<td class=\\'split1\\'>(.*?)<\/td>"
             split_times = re.findall(pattern, split_times_rough)
             result_url = time_cell.find('a')['href']
             result_id = parse_qs(urlparse(result_url).query)['id'][0]
-            results.append({'result_id': result_id, 'name': name, 'club_name': club_name, 'time': time, 'split_times': split_times})
+            results.append({'result_id': result_id, 'athlete_id': athlete_id, 'name': name, 'club_name': club_name, 'time': time, 'split_times': split_times})
         return results
 
 
 
 
 class Result(ScraperMixin):
     """
```

### Comparing `swimrankingsscraper-0.1.1/swimrankingsscraper.egg-info/PKG-INFO` & `swimrankingsscraper-0.1.2/swimrankingsscraper.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swimrankingsscraper
-Version: 0.1.1
+Version: 0.1.2
 Summary: A scraper for swimrankings.net
 Home-page: https://swimrankingsscraper.readthedocs.io/
 Author: Bas Neeleman
 Author-email: bas@neeleman-mail.nl
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `swimrankingsscraper-0.1.1/tests/test_swimrankingsscraper.py` & `swimrankingsscraper-0.1.2/tests/test_swimrankingsscraper.py`

 * *Files identical despite different names*

