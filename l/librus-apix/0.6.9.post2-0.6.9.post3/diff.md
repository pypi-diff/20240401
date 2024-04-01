# Comparing `tmp/librus_apix-0.6.9.post2.tar.gz` & `tmp/librus_apix-0.6.9.post3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "librus_apix-0.6.9.post2.tar", last modified: Tue Mar  5 00:20:55 2024, max compression
+gzip compressed data, was "librus_apix-0.6.9.post3.tar", last modified: Sun Mar 31 00:00:31 2024, max compression
```

## Comparing `librus_apix-0.6.9.post2.tar` & `librus_apix-0.6.9.post3.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 00:20:55.773251 librus_apix-0.6.9.post2/
--rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-03-05 00:20:51.000000 librus_apix-0.6.9.post2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      453 2024-03-05 00:20:55.773251 librus_apix-0.6.9.post2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3157 2024-03-05 00:20:51.000000 librus_apix-0.6.9.post2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 00:20:55.773251 librus_apix-0.6.9.post2/librus_apix/
--rw-r--r--   0 runner    (1001) docker     (127)      346 2024-03-05 00:20:51.000000 librus_apix-0.6.9.post2/librus_apix/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-03-05 00:20:51.000000 librus_apix-0.6.9.post2/librus_apix/announcements.py
--rw-r--r--   0 runner    (1001) docker     (127)     5296 2024-03-05 00:20:51.000000 librus_apix-0.6.9.post2/librus_apix/attendance.py
--rw-r--r--   0 runner    (1001) docker     (127)     3030 2024-03-05 00:20:51.000000 librus_apix-0.6.9.post2/librus_apix/completed_lessons.py
--rw-r--r--   0 runner    (1001) docker     (127)      211 2024-03-05 00:20:51.000000 librus_apix-0.6.9.post2/librus_apix/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     5859 2024-03-05 00:20:51.000000 librus_apix-0.6.9.post2/librus_apix/get_token.py
--rw-r--r--   0 runner    (1001) docker     (127)     9428 2024-03-05 00:20:51.000000 librus_apix-0.6.9.post2/librus_apix/grades.py
--rw-r--r--   0 runner    (1001) docker     (127)      381 2024-03-05 00:20:51.000000 librus_apix-0.6.9.post2/librus_apix/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2382 2024-03-05 00:20:51.000000 librus_apix-0.6.9.post2/librus_apix/homework.py
--rw-r--r--   0 runner    (1001) docker     (127)     2591 2024-03-05 00:20:51.000000 librus_apix-0.6.9.post2/librus_apix/messages.py
--rw-r--r--   0 runner    (1001) docker     (127)     3214 2024-03-05 00:20:51.000000 librus_apix-0.6.9.post2/librus_apix/schedule.py
--rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-03-05 00:20:51.000000 librus_apix-0.6.9.post2/librus_apix/student_information.py
--rw-r--r--   0 runner    (1001) docker     (127)     4094 2024-03-05 00:20:51.000000 librus_apix-0.6.9.post2/librus_apix/timetable.py
--rw-r--r--   0 runner    (1001) docker     (127)      852 2024-03-05 00:20:51.000000 librus_apix-0.6.9.post2/librus_apix/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 00:20:55.773251 librus_apix-0.6.9.post2/librus_apix.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      453 2024-03-05 00:20:55.000000 librus_apix-0.6.9.post2/librus_apix.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      585 2024-03-05 00:20:55.000000 librus_apix-0.6.9.post2/librus_apix.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-05 00:20:55.000000 librus_apix-0.6.9.post2/librus_apix.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-03-05 00:20:55.000000 librus_apix-0.6.9.post2/librus_apix.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-03-05 00:20:55.000000 librus_apix-0.6.9.post2/librus_apix.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-03-05 00:20:51.000000 librus_apix-0.6.9.post2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      613 2024-03-05 00:20:55.777251 librus_apix-0.6.9.post2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-05 00:20:51.000000 librus_apix-0.6.9.post2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 00:00:31.220137 librus_apix-0.6.9.post3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-03-31 00:00:29.000000 librus_apix-0.6.9.post3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-03-31 00:00:31.220137 librus_apix-0.6.9.post3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3157 2024-03-31 00:00:29.000000 librus_apix-0.6.9.post3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 00:00:31.220137 librus_apix-0.6.9.post3/librus_apix/
+-rw-r--r--   0 runner    (1001) docker     (127)      346 2024-03-31 00:00:29.000000 librus_apix-0.6.9.post3/librus_apix/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-03-31 00:00:29.000000 librus_apix-0.6.9.post3/librus_apix/announcements.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5296 2024-03-31 00:00:29.000000 librus_apix-0.6.9.post3/librus_apix/attendance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3030 2024-03-31 00:00:29.000000 librus_apix-0.6.9.post3/librus_apix/completed_lessons.py
+-rw-r--r--   0 runner    (1001) docker     (127)      211 2024-03-31 00:00:29.000000 librus_apix-0.6.9.post3/librus_apix/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5859 2024-03-31 00:00:29.000000 librus_apix-0.6.9.post3/librus_apix/get_token.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9541 2024-03-31 00:00:29.000000 librus_apix-0.6.9.post3/librus_apix/grades.py
+-rw-r--r--   0 runner    (1001) docker     (127)      381 2024-03-31 00:00:29.000000 librus_apix-0.6.9.post3/librus_apix/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2382 2024-03-31 00:00:29.000000 librus_apix-0.6.9.post3/librus_apix/homework.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2591 2024-03-31 00:00:29.000000 librus_apix-0.6.9.post3/librus_apix/messages.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3214 2024-03-31 00:00:29.000000 librus_apix-0.6.9.post3/librus_apix/schedule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-03-31 00:00:29.000000 librus_apix-0.6.9.post3/librus_apix/student_information.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4094 2024-03-31 00:00:29.000000 librus_apix-0.6.9.post3/librus_apix/timetable.py
+-rw-r--r--   0 runner    (1001) docker     (127)      852 2024-03-31 00:00:29.000000 librus_apix-0.6.9.post3/librus_apix/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 00:00:31.220137 librus_apix-0.6.9.post3/librus_apix.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-03-31 00:00:31.000000 librus_apix-0.6.9.post3/librus_apix.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      585 2024-03-31 00:00:31.000000 librus_apix-0.6.9.post3/librus_apix.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-31 00:00:31.000000 librus_apix-0.6.9.post3/librus_apix.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-03-31 00:00:31.000000 librus_apix-0.6.9.post3/librus_apix.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-03-31 00:00:31.000000 librus_apix-0.6.9.post3/librus_apix.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-03-31 00:00:29.000000 librus_apix-0.6.9.post3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      613 2024-03-31 00:00:31.224137 librus_apix-0.6.9.post3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-31 00:00:29.000000 librus_apix-0.6.9.post3/setup.py
```

### Comparing `librus_apix-0.6.9.post2/LICENSE` & `librus_apix-0.6.9.post3/LICENSE`

 * *Files identical despite different names*

### Comparing `librus_apix-0.6.9.post2/README.md` & `librus_apix-0.6.9.post3/README.md`

 * *Files identical despite different names*

### Comparing `librus_apix-0.6.9.post2/librus_apix/announcements.py` & `librus_apix-0.6.9.post3/librus_apix/announcements.py`

 * *Files identical despite different names*

### Comparing `librus_apix-0.6.9.post2/librus_apix/attendance.py` & `librus_apix-0.6.9.post3/librus_apix/attendance.py`

 * *Files identical despite different names*

### Comparing `librus_apix-0.6.9.post2/librus_apix/completed_lessons.py` & `librus_apix-0.6.9.post3/librus_apix/completed_lessons.py`

 * *Files identical despite different names*

### Comparing `librus_apix-0.6.9.post2/librus_apix/get_token.py` & `librus_apix-0.6.9.post3/librus_apix/get_token.py`

 * *Files identical despite different names*

### Comparing `librus_apix-0.6.9.post2/librus_apix/grades.py` & `librus_apix-0.6.9.post3/librus_apix/grades.py`

 * *Files 2% similar despite different names*

```diff
@@ -127,15 +127,15 @@
         teacher,
         weight,
     )
 
 
 def _extract_grades_numeric(table_rows):
     # list containing two dicts (for each semester)
-    # key of each semester dict is subject, in each subject there is list of grades 
+    # key of each semester dict is subject, in each subject there is list of grades
     sem_grades: List[Dict[str, List[Grade]]] = [{}, {}]
     avg_grades = defaultdict(list)
 
     for box in table_rows:
         if box.select_one("td[class='center micro screen-only']") is None:
             # row without grade data - skip
             continue
@@ -147,15 +147,16 @@
         average_grades = list(map(lambda x: x.text, box.select("td.right")))
         semesters = [semester_grades[1:4], semester_grades[4:7]]
         subject = _handle_subject(semester_grades)
         for sem, semester in enumerate(semesters):
             if subject not in sem_grades[sem]:
                 sem_grades[sem][subject] = []
             for sg in semester:
-                grade_a = sg.select("td[class!='center'] > span.grade-box > a")
+                grade_a_improved = sg.select("td[class!='center'] > span > span.grade-box > a")
+                grade_a = sg.select("td[class!='center'] > span.grade-box > a") + grade_a_improved
                 for a in grade_a:
                     (
                         _grade,
                         date,
                         href,
                         desc,
                         counts,
@@ -249,15 +250,15 @@
         if parse_next_row:
             parse_next_row = False
             paragraphs = box.find_all("p")
             text_list = [ par.text.strip() for par in paragraphs ]
             summary_desc = "\n".join(text_list).strip()
             found_grade = True
             # description found - break
-            # There is no more grades for now (for first semester). Maybe there will be grade for 
+            # There is no more grades for now (for first semester). Maybe there will be grade for
             # second semester, but the format (structure) of web page is unknown for the moment.
             # #TODO: implement the case for second semester (in future)
             break
 
         header = box.select_one("th")
         if header:
             # header row found - next row will contain the description
```

### Comparing `librus_apix-0.6.9.post2/librus_apix/homework.py` & `librus_apix-0.6.9.post3/librus_apix/homework.py`

 * *Files identical despite different names*

### Comparing `librus_apix-0.6.9.post2/librus_apix/messages.py` & `librus_apix-0.6.9.post3/librus_apix/messages.py`

 * *Files identical despite different names*

### Comparing `librus_apix-0.6.9.post2/librus_apix/schedule.py` & `librus_apix-0.6.9.post3/librus_apix/schedule.py`

 * *Files identical despite different names*

### Comparing `librus_apix-0.6.9.post2/librus_apix/student_information.py` & `librus_apix-0.6.9.post3/librus_apix/student_information.py`

 * *Files identical despite different names*

### Comparing `librus_apix-0.6.9.post2/librus_apix/timetable.py` & `librus_apix-0.6.9.post3/librus_apix/timetable.py`

 * *Files identical despite different names*

### Comparing `librus_apix-0.6.9.post2/librus_apix/urls.py` & `librus_apix-0.6.9.post3/librus_apix/urls.py`

 * *Files identical despite different names*

### Comparing `librus_apix-0.6.9.post2/librus_apix.egg-info/SOURCES.txt` & `librus_apix-0.6.9.post3/librus_apix.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `librus_apix-0.6.9.post2/setup.cfg` & `librus_apix-0.6.9.post3/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [darglint]
 strictness = long
 docstring_style = google
 
 [metadata]
 name = librus_apix
-version = 0.6.9-2
+version = 0.6.9-3
 license = MIT
 description = Web Scraper for Librus Synergia
 long_description = ""
 author = Pascal Jodłowski
 url = https://github.com/poroknights/librus-apix
 keywords = librus, scraper, api, synergia
 classifiers =
```

