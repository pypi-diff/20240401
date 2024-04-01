# Comparing `tmp/edx-submissions-3.6.0.tar.gz` & `tmp/edx-submissions-3.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edx-submissions-3.6.0.tar", last modified: Tue Aug  1 18:23:34 2023, max compression
+gzip compressed data, was "edx-submissions-3.7.0.tar", last modified: Mon Apr  1 14:54:04 2024, max compression
```

## Comparing `edx-submissions-3.6.0.tar` & `edx-submissions-3.7.0.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-01 18:23:34.090648 edx-submissions-3.6.0/
--rw-r--r--   0 runner    (1001) docker     (122)    35136 2023-08-01 18:23:25.000000 edx-submissions-3.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)      122 2023-08-01 18:23:25.000000 edx-submissions-3.6.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)      750 2023-08-01 18:23:34.090648 edx-submissions-3.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1793 2023-08-01 18:23:25.000000 edx-submissions-3.6.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-01 18:23:34.086647 edx-submissions-3.6.0/edx_submissions.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)      750 2023-08-01 18:23:34.000000 edx-submissions-3.6.0/edx_submissions.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1125 2023-08-01 18:23:34.000000 edx-submissions-3.6.0/edx_submissions.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-08-01 18:23:34.000000 edx-submissions-3.6.0/edx_submissions.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       75 2023-08-01 18:23:34.000000 edx-submissions-3.6.0/edx_submissions.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       12 2023-08-01 18:23:34.000000 edx-submissions-3.6.0/edx_submissions.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-01 18:23:34.086647 edx-submissions-3.6.0/requirements/
--rw-r--r--   0 runner    (1001) docker     (122)      206 2023-08-01 18:23:25.000000 edx-submissions-3.6.0/requirements/base.in
--rw-r--r--   0 runner    (1001) docker     (122)       91 2023-08-01 18:23:25.000000 edx-submissions-3.6.0/requirements/docs.in
--rw-r--r--   0 runner    (1001) docker     (122)      174 2023-08-01 18:23:25.000000 edx-submissions-3.6.0/requirements/test.in
--rw-r--r--   0 runner    (1001) docker     (122)      318 2023-08-01 18:23:34.090648 edx-submissions-3.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     2784 2023-08-01 18:23:25.000000 edx-submissions-3.6.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-01 18:23:34.090648 edx-submissions-3.6.0/submissions/
--rw-r--r--   0 runner    (1001) docker     (122)       71 2023-08-01 18:23:25.000000 edx-submissions-3.6.0/submissions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5170 2023-08-01 18:23:25.000000 edx-submissions-3.6.0/submissions/admin.py
--rw-r--r--   0 runner    (1001) docker     (122)    39479 2023-08-01 18:23:25.000000 edx-submissions-3.6.0/submissions/api.py
--rw-r--r--   0 runner    (1001) docker     (122)     2454 2023-08-01 18:23:25.000000 edx-submissions-3.6.0/submissions/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-01 18:23:34.090648 edx-submissions-3.6.0/submissions/management/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-08-01 18:23:25.000000 edx-submissions-3.6.0/submissions/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-01 18:23:34.090648 edx-submissions-3.6.0/submissions/management/commands/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-08-01 18:23:25.000000 edx-submissions-3.6.0/submissions/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6344 2023-08-01 18:23:25.000000 edx-submissions-3.6.0/submissions/management/commands/analyze_uploaded_file_sizes.py
--rw-r--r--   0 runner    (1001) docker     (122)     2828 2023-08-01 18:23:25.000000 edx-submissions-3.6.0/submissions/management/commands/update_submissions_uuids.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-01 18:23:34.090648 edx-submissions-3.6.0/submissions/migrations/
--rw-r--r--   0 runner    (1001) docker     (122)     3489 2023-08-01 18:23:25.000000 edx-submissions-3.6.0/submissions/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (122)     6745 2023-08-01 18:23:25.000000 edx-submissions-3.6.0/submissions/migrations/0001_squashed_0005_CreateTeamModel.py
--rw-r--r--   0 runner    (1001) docker     (122)      910 2023-08-01 18:23:25.000000 edx-submissions-3.6.0/submissions/migrations/0002_auto_20151119_0913.py
--rw-r--r--   0 runner    (1001) docker     (122)      658 2023-08-01 18:23:25.000000 edx-submissions-3.6.0/submissions/migrations/0002_team_submission_optional.py
--rw-r--r--   0 runner    (1001) docker     (122)      484 2023-08-01 18:23:25.000000 edx-submissions-3.6.0/submissions/migrations/0003_ensure_ascii.py
--rw-r--r--   0 runner    (1001) docker     (122)      400 2023-08-01 18:23:25.000000 edx-submissions-3.6.0/submissions/migrations/0003_submission_status.py
--rw-r--r--   0 runner    (1001) docker     (122)      375 2023-08-01 18:23:25.000000 edx-submissions-3.6.0/submissions/migrations/0004_remove_django_extensions.py
--rw-r--r--   0 runner    (1001) docker     (122)     2379 2023-08-01 18:23:25.000000 edx-submissions-3.6.0/submissions/migrations/0005_CreateTeamModel.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-08-01 18:23:25.000000 edx-submissions-3.6.0/submissions/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    20313 2023-08-01 18:23:25.000000 edx-submissions-3.6.0/submissions/models.py
--rw-r--r--   0 runner    (1001) docker     (122)     7303 2023-08-01 18:23:25.000000 edx-submissions-3.6.0/submissions/serializers.py
--rw-r--r--   0 runner    (1001) docker     (122)    18543 2023-08-01 18:23:25.000000 edx-submissions-3.6.0/submissions/team_api.py
--rw-r--r--   0 runner    (1001) docker     (122)     1469 2023-08-01 18:23:25.000000 edx-submissions-3.6.0/submissions/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 14:54:04.955906 edx-submissions-3.7.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    35136 2024-04-01 14:54:01.000000 edx-submissions-3.7.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-01 14:54:01.000000 edx-submissions-3.7.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      953 2024-04-01 14:54:04.955906 edx-submissions-3.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4842 2024-04-01 14:54:01.000000 edx-submissions-3.7.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 14:54:04.955906 edx-submissions-3.7.0/edx_submissions.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      953 2024-04-01 14:54:04.000000 edx-submissions-3.7.0/edx_submissions.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1129 2024-04-01 14:54:04.000000 edx-submissions-3.7.0/edx_submissions.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 14:54:04.000000 edx-submissions-3.7.0/edx_submissions.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-01 14:54:04.000000 edx-submissions-3.7.0/edx_submissions.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-01 14:54:04.000000 edx-submissions-3.7.0/edx_submissions.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 14:54:04.951906 edx-submissions-3.7.0/requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-01 14:54:01.000000 edx-submissions-3.7.0/requirements/base.in
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-01 14:54:01.000000 edx-submissions-3.7.0/requirements/docs.in
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2024-04-01 14:54:01.000000 edx-submissions-3.7.0/requirements/test.in
+-rw-r--r--   0 runner    (1001) docker     (127)      318 2024-04-01 14:54:04.955906 edx-submissions-3.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2846 2024-04-01 14:54:01.000000 edx-submissions-3.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 14:54:04.955906 edx-submissions-3.7.0/submissions/
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-01 14:54:01.000000 edx-submissions-3.7.0/submissions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5170 2024-04-01 14:54:01.000000 edx-submissions-3.7.0/submissions/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39466 2024-04-01 14:54:01.000000 edx-submissions-3.7.0/submissions/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2449 2024-04-01 14:54:01.000000 edx-submissions-3.7.0/submissions/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 14:54:04.955906 edx-submissions-3.7.0/submissions/management/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 14:54:01.000000 edx-submissions-3.7.0/submissions/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 14:54:04.955906 edx-submissions-3.7.0/submissions/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 14:54:01.000000 edx-submissions-3.7.0/submissions/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6344 2024-04-01 14:54:01.000000 edx-submissions-3.7.0/submissions/management/commands/analyze_uploaded_file_sizes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2828 2024-04-01 14:54:01.000000 edx-submissions-3.7.0/submissions/management/commands/update_submissions_uuids.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 14:54:04.955906 edx-submissions-3.7.0/submissions/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)     3489 2024-04-01 14:54:01.000000 edx-submissions-3.7.0/submissions/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6745 2024-04-01 14:54:01.000000 edx-submissions-3.7.0/submissions/migrations/0001_squashed_0005_CreateTeamModel.py
+-rw-r--r--   0 runner    (1001) docker     (127)      910 2024-04-01 14:54:01.000000 edx-submissions-3.7.0/submissions/migrations/0002_auto_20151119_0913.py
+-rw-r--r--   0 runner    (1001) docker     (127)      658 2024-04-01 14:54:01.000000 edx-submissions-3.7.0/submissions/migrations/0002_team_submission_optional.py
+-rw-r--r--   0 runner    (1001) docker     (127)      484 2024-04-01 14:54:01.000000 edx-submissions-3.7.0/submissions/migrations/0003_ensure_ascii.py
+-rw-r--r--   0 runner    (1001) docker     (127)      400 2024-04-01 14:54:01.000000 edx-submissions-3.7.0/submissions/migrations/0003_submission_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)      375 2024-04-01 14:54:01.000000 edx-submissions-3.7.0/submissions/migrations/0004_remove_django_extensions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2379 2024-04-01 14:54:01.000000 edx-submissions-3.7.0/submissions/migrations/0005_CreateTeamModel.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 14:54:01.000000 edx-submissions-3.7.0/submissions/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20313 2024-04-01 14:54:01.000000 edx-submissions-3.7.0/submissions/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7303 2024-04-01 14:54:01.000000 edx-submissions-3.7.0/submissions/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18543 2024-04-01 14:54:01.000000 edx-submissions-3.7.0/submissions/team_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1469 2024-04-01 14:54:01.000000 edx-submissions-3.7.0/submissions/views.py
```

### Comparing `edx-submissions-3.6.0/LICENSE` & `edx-submissions-3.7.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `edx-submissions-3.6.0/edx_submissions.egg-info/SOURCES.txt` & `edx-submissions-3.7.0/edx_submissions.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-LICENSE
+LICENSE.txt
 MANIFEST.in
 README.rst
 setup.cfg
 setup.py
 edx_submissions.egg-info/PKG-INFO
 edx_submissions.egg-info/SOURCES.txt
 edx_submissions.egg-info/dependency_links.txt
```

### Comparing `edx-submissions-3.6.0/setup.py` & `edx-submissions-3.7.0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -70,20 +70,21 @@
     description='An API for creating submissions and scores.',
     long_description="An API for creating and scoring submissions for the Open edX platform",
     url='http://github.com/openedx/edx-submissions.git',
     license='AGPL',
     classifiers=[
         'Development Status :: 3 - Alpha',
         'Framework :: Django',
-        'Framework :: Django :: 3.2',
-        'Framework :: Django :: 4.0',
+        'Framework :: Django :: 4.2',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: GNU Affero General Public License v3',
         'Operating System :: OS Independent',
         'Programming Language :: Python',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 3.11',
+        'Programming Language :: Python :: 3.12',
     ],
     packages=find_packages(include=['submissions*'], exclude=['*.test', '*.tests']),
     install_requires=load_requirements('requirements/base.in'),
     tests_require=load_requirements('requirements/test.in'),
 )
```

### Comparing `edx-submissions-3.6.0/submissions/admin.py` & `edx-submissions-3.7.0/submissions/admin.py`

 * *Files identical despite different names*

### Comparing `edx-submissions-3.6.0/submissions/api.py` & `edx-submissions-3.7.0/submissions/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -422,25 +422,27 @@
         submission = next(row_iter)  # pylint: disable= stop-iteration-return
         data = SubmissionSerializer(submission).data
         data['student_id'] = submission.student_item.student_id
         yield data
 
 
 def get_all_course_submission_information(course_id, item_type, read_replica=True):
-    """ For the given course, get all student items of the given item type, all the submissions for those itemes,
+    """
+    For the given course, get all student items of the given item type, all the submissions for those itemes,
     and the latest scores for each item. If a submission was given a score that is not the latest score for the
     relevant student item, it will still be included but without score.
 
     Args:
         course_id (str): The course that we are getting submissions from.
         item_type (str): The type of items that we are getting submissions for.
         read_replica (bool): Try to use the database's read replica if it's available.
 
     Yields:
         A tuple of three dictionaries representing:
+
         (1) a student item with the following fields:
             student_id
             course_id
             student_item
             item_type
         (2) a submission with the following fields:
             student_item
@@ -481,15 +483,16 @@
             StudentItemSerializer(student_item).data,
             SubmissionSerializer(submission).data,
             serialized_score
         )
 
 
 def get_top_submissions(course_id, item_id, item_type, number_of_top_scores, use_cache=True, read_replica=True):
-    """Get a number of top scores for an assessment based on a particular student item
+    """
+    Get a number of top scores for an assessment based on a particular student item
 
     This function will return top scores for the piece of assessment.
     It will consider only the latest and greater than 0 score for a piece of assessment.
     A score is only calculated for a student item if it has completed the workflow for
     a particular assessment module.
 
     In general, users of top submissions can tolerate some latency
@@ -502,15 +505,15 @@
         item_type (str): The type of item to retrieve
         number_of_top_scores (int): The number of scores to return, greater than 0 and no
         more than 100.
 
     Kwargs:
         use_cache (bool): If true, check the cache before retrieving querying the database.
         read_replica (bool): If true, attempt to use the read replica database.
-            If no read replica is available, use the default database.
+        If no read replica is available, use the default database.
 
     Returns:
         topscores (dict): The top scores for the assessment for the student item.
             An empty array if there are no scores or all scores are 0.
 
     Raises:
         SubmissionNotFoundError: Raised when a submission cannot be found for
@@ -802,27 +805,28 @@
             'student_id': student_id,
         }
     )
 
 
 def set_score(submission_uuid, points_earned, points_possible,
               annotation_creator=None, annotation_type=None, annotation_reason=None):
-    """Set a score for a particular submission.
+    """
+    Set a score for a particular submission.
 
     Sets the score for a particular submission. This score is calculated
     externally to the API.
 
     Args:
         submission_uuid (str): UUID for the submission (must exist).
         points_earned (int): The earned points for this submission.
         points_possible (int): The total points possible for this particular student item.
 
         annotation_creator (str): An optional field for recording who gave this particular score
-        annotation_type (str): An optional field for recording what type of annotation should be created,
-                                e.g. "staff_override".
+        annotation_type (str): An optional field for recording what type of
+        annotation should be created, e.g. "staff_override".
         annotation_reason (str): An optional field for recording why this score was set to its value.
 
     Returns:
         None
 
     Raises:
         SubmissionInternalError: Thrown if there was an internal error while
```

### Comparing `edx-submissions-3.6.0/submissions/errors.py` & `edx-submissions-3.7.0/submissions/errors.py`

 * *Files 0% similar despite different names*

```diff
@@ -63,16 +63,16 @@
         self.args += (self.field_errors,)
 
     def __repr__(self):
         """
         Show the field errors upon output.
         """
         return (
-            f'{self.__class__.__name__}'  # pylint: disable=no-member
-            f'(msg="{self.message}", field_errors={self.field_errors})'
+            # pylint: disable=no-member
+            f'{self.__class__.__name__}(msg="{self.message}", field_errors={self.field_errors})'
         )
 
 
 class DuplicateTeamSubmissionsError(Exception):
     """ An error that is raised when duplicate team submissions are detected. """
```

### Comparing `edx-submissions-3.6.0/submissions/management/commands/analyze_uploaded_file_sizes.py` & `edx-submissions-3.7.0/submissions/management/commands/analyze_uploaded_file_sizes.py`

 * *Files identical despite different names*

### Comparing `edx-submissions-3.6.0/submissions/management/commands/update_submissions_uuids.py` & `edx-submissions-3.7.0/submissions/management/commands/update_submissions_uuids.py`

 * *Files identical despite different names*

### Comparing `edx-submissions-3.6.0/submissions/migrations/0001_initial.py` & `edx-submissions-3.7.0/submissions/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `edx-submissions-3.6.0/submissions/migrations/0001_squashed_0005_CreateTeamModel.py` & `edx-submissions-3.7.0/submissions/migrations/0001_squashed_0005_CreateTeamModel.py`

 * *Files identical despite different names*

### Comparing `edx-submissions-3.6.0/submissions/migrations/0002_auto_20151119_0913.py` & `edx-submissions-3.7.0/submissions/migrations/0002_auto_20151119_0913.py`

 * *Files identical despite different names*

### Comparing `edx-submissions-3.6.0/submissions/migrations/0002_team_submission_optional.py` & `edx-submissions-3.7.0/submissions/migrations/0002_team_submission_optional.py`

 * *Files identical despite different names*

### Comparing `edx-submissions-3.6.0/submissions/migrations/0005_CreateTeamModel.py` & `edx-submissions-3.7.0/submissions/migrations/0005_CreateTeamModel.py`

 * *Files identical despite different names*

### Comparing `edx-submissions-3.6.0/submissions/models.py` & `edx-submissions-3.7.0/submissions/models.py`

 * *Files identical despite different names*

### Comparing `edx-submissions-3.6.0/submissions/serializers.py` & `edx-submissions-3.7.0/submissions/serializers.py`

 * *Files identical despite different names*

### Comparing `edx-submissions-3.6.0/submissions/team_api.py` & `edx-submissions-3.7.0/submissions/team_api.py`

 * *Files identical despite different names*

### Comparing `edx-submissions-3.6.0/submissions/views.py` & `edx-submissions-3.7.0/submissions/views.py`

 * *Files identical despite different names*

