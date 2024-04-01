# Comparing `tmp/phenomApis-0.0.8.tar.gz` & `tmp/phenomApis-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "phenomApis-0.0.8.tar", last modified: Mon Nov 27 09:14:32 2023, max compression
+gzip compressed data, was "phenomApis-0.0.9.tar", last modified: Mon Nov 27 10:49:40 2023, max compression
```

## Comparing `phenomApis-0.0.8.tar` & `phenomApis-0.0.9.tar`

### file list

```diff
@@ -1,112 +1,141 @@
-drwxr-xr-x   0 hemanthkumar  (1001) hemanthkumar  (1001)        0 2023-11-27 09:14:32.900135 phenomApis-0.0.8/
--rw-r--r--   0 hemanthkumar  (1001) hemanthkumar  (1001)     1062 2023-11-21 11:14:01.000000 phenomApis-0.0.8/LICENSE
--rw-r--r--   0 hemanthkumar  (1001) hemanthkumar  (1001)      650 2023-11-27 09:14:32.896135 phenomApis-0.0.8/PKG-INFO
-drwxr-xr-x   0 hemanthkumar  (1001) hemanthkumar  (1001)        0 2023-11-27 09:14:32.844135 phenomApis-0.0.8/phenom/
--rw-r--r--   0 hemanthkumar  (1001) hemanthkumar  (1001)        0 2023-11-23 16:51:34.000000 phenomApis-0.0.8/phenom/__init__.py
-drwxr-xr-x   0 hemanthkumar  (1001) hemanthkumar  (1001)        0 2023-11-27 09:14:32.844135 phenomApis-0.0.8/phenom/api/
--rw-r--r--   0 hemanthkumar  (1001) hemanthkumar  (1001)        0 2023-11-23 16:28:16.000000 phenomApis-0.0.8/phenom/api/__init__.py
-drwxr-xr-x   0 hemanthkumar  (1001) hemanthkumar  (1001)        0 2023-11-27 09:14:32.844135 phenomApis-0.0.8/phenom/api/aisourcing/
--rw-r--r--   0 hemanthkumar  (1001) hemanthkumar  (1001)     1413 2023-11-27 06:27:57.000000 phenomApis-0.0.8/phenom/api/aisourcing/__init__.py
--rw-r--r--   0 hemanthkumar  (1001) hemanthkumar  (1001)     9103 2023-11-27 06:29:01.000000 phenomApis-0.0.8/phenom/api/aisourcing/ai_matching_api.py
-drwxr-xr-x   0 hemanthkumar  (1001) hemanthkumar  (1001)        0 2023-11-27 09:14:32.848135 phenomApis-0.0.8/phenom/api/aisourcing/models/
--rw-r--r--   0 hemanthkumar  (1001) hemanthkumar  (1001)     1300 2023-11-27 06:27:57.000000 phenomApis-0.0.8/phenom/api/aisourcing/models/__init__.py
--rw-r--r--   0 hemanthkumar  (1001) hemanthkumar  (1001)     3624 2023-11-27 06:14:39.000000 phenomApis-0.0.8/phenom/api/aisourcing/models/error_response.py
--rw-r--r--   0 hemanthkumar  (1001) hemanthkumar  (1001)     4480 2023-11-27 06:14:39.000000 phenomApis-0.0.8/phenom/api/aisourcing/models/fit_score_request.py
--rw-r--r--   0 hemanthkumar  (1001) hemanthkumar  (1001)     3684 2023-11-27 06:14:39.000000 phenomApis-0.0.8/phenom/api/aisourcing/models/fitscore_bad_request.py
--rw-r--r--   0 hemanthkumar  (1001) hemanthkumar  (1001)     3715 2023-11-27 06:14:39.000000 phenomApis-0.0.8/phenom/api/aisourcing/models/fitscore_response.py
--rw-r--r--   0 hemanthkumar  (1001) hemanthkumar  (1001)     7573 2023-11-27 06:14:39.000000 phenomApis-0.0.8/phenom/api/aisourcing/models/fitscore_response_result.py
--rw-r--r--   0 hemanthkumar  (1001) hemanthkumar  (1001)     4752 2023-11-27 06:14:39.000000 phenomApis-0.0.8/phenom/api/aisourcing/models/fitscore_response_skill_gap.py
--rw-r--r--   0 hemanthkumar  (1001) hemanthkumar  (1001)     3790 2023-11-27 06:14:39.000000 phenomApis-0.0.8/phenom/api/aisourcing/models/preferred_locations.py
--rw-r--r--   0 hemanthkumar  (1001) hemanthkumar  (1001)     3640 2023-11-27 06:14:39.000000 phenomApis-0.0.8/phenom/api/aisourcing/models/preferred_locations_latlong.py
--rw-r--r--   0 hemanthkumar  (1001) hemanthkumar  (1001)     3383 2023-11-27 06:14:39.000000 phenomApis-0.0.8/phenom/api/aisourcing/models/skill_matching_bad_request.py
--rw-r--r--   0 hemanthkumar  (1001) hemanthkumar  (1001)     3407 2023-11-27 06:14:39.000000 phenomApis-0.0.8/phenom/api/aisourcing/models/skill_matching_error_response.py
--rw-r--r--   0 hemanthkumar  (1001) hemanthkumar  (1001)     4195 2023-11-27 06:14:39.000000 phenomApis-0.0.8/phenom/api/aisourcing/models/skill_matching_response.py
--rw-r--r--   0 hemanthkumar  (1001) hemanthkumar  (1001)     5544 2023-11-27 06:14:39.000000 phenomApis-0.0.8/phenom/api/aisourcing/models/user_profile_fit_score.py
-drwxr-xr-x   0 hemanthkumar  (1001) hemanthkumar  (1001)        0 2023-11-27 09:14:32.848135 phenomApis-0.0.8/phenom/api/exsearch/
--rw-r--r--   0 hemanthkumar  (1001) hemanthkumar  (1001)     1955 2023-11-24 06:50:15.000000 phenomApis-0.0.8/phenom/api/exsearch/__init__.py
--rw-r--r--   0 hemanthkumar  (1001) hemanthkumar  (1001)    11764 2023-11-24 06:50:15.000000 phenomApis-0.0.8/phenom/api/exsearch/employees_api.py
--rw-r--r--   0 hemanthkumar  (1001) hemanthkumar  (1001)     4459 2023-11-24 06:50:15.000000 phenomApis-0.0.8/phenom/api/exsearch/mentor_api.py
-drwxr-xr-x   0 hemanthkumar  (1001) hemanthkumar  (1001)        0 2023-11-27 09:14:32.864135 phenomApis-0.0.8/phenom/api/exsearch/models/
--rw-r--r--   0 hemanthkumar  (1001) hemanthkumar  (1001)     1794 2023-11-24 06:10:38.000000 phenomApis-0.0.8/phenom/api/exsearch/models/__init__.py
--rw-r--r--   0 hemanthkumar  (1001) hemanthkumar  (1001)     3641 2023-11-23 12:05:51.000000 phenomApis-0.0.8/phenom/api/exsearch/models/aggregations_node.py
--rw-r--r--   0 hemanthkumar  (1001) hemanthkumar  (1001)     4855 2023-11-23 12:05:51.000000 phenomApis-0.0.8/phenom/api/exsearch/models/bad_request.py
--rw-r--r--   0 hemanthkumar  (1001) hemanthkumar  (1001)     4335 2023-11-23 12:05:51.000000 phenomApis-0.0.8/phenom/api/exsearch/models/common_node.py
--rw-r--r--   0 hemanthkumar  (1001) hemanthkumar  (1001)     7451 2023-11-23 12:05:51.000000 phenomApis-0.0.8/phenom/api/exsearch/models/employee_node.py
--rw-r--r--   0 hemanthkumar  (1001) hemanthkumar  (1001)     6594 2023-11-23 12:05:51.000000 phenomApis-0.0.8/phenom/api/exsearch/models/employee_search_request.py
--rw-r--r--   0 hemanthkumar  (1001) hemanthkumar  (1001)     4538 2023-11-23 12:05:51.000000 phenomApis-0.0.8/phenom/api/exsearch/models/employee_search_response.py
--rw-r--r--   0 hemanthkumar  (1001) hemanthkumar  (1001)     3965 2023-11-23 12:05:51.000000 phenomApis-0.0.8/phenom/api/exsearch/models/employee_search_response_data.py
--rw-r--r--   0 hemanthkumar  (1001) hemanthkumar  (1001)     4826 2023-11-23 12:05:51.000000 phenomApis-0.0.8/phenom/api/exsearch/models/employee_type_ahead_agg_request.py
--rw-r--r--   0 hemanthkumar  (1001) hemanthkumar  (1001)     3936 2023-11-23 12:05:51.000000 phenomApis-0.0.8/phenom/api/exsearch/models/employee_type_ahead_request.py
--rw-r--r--   0 hemanthkumar  (1001) hemanthkumar  (1001)     3814 2023-11-23 12:05:51.000000 phenomApis-0.0.8/phenom/api/exsearch/models/employee_typeahead_agg_response.py
--rw-r--r--   0 hemanthkumar  (1001) hemanthkumar  (1001)     5224 2023-11-23 12:05:51.000000 phenomApis-0.0.8/phenom/api/exsearch/models/employee_typeahead_response.py
--rw-r--r--   0 hemanthkumar  (1001) hemanthkumar  (1001)     3277 2023-11-23 12:05:51.000000 phenomApis-0.0.8/phenom/api/exsearch/models/employee_typeahead_response_data.py
--rw-r--r--   0 hemanthkumar  (1001) hemanthkumar  (1001)     4915 2023-11-23 12:05:51.000000 phenomApis-0.0.8/phenom/api/exsearch/models/error_response.py
--rw-r--r--   0 hemanthkumar  (1001) hemanthkumar  (1001)     4147 2023-11-23 12:05:51.000000 phenomApis-0.0.8/phenom/api/exsearch/models/facets_node.py
--rw-r--r--   0 hemanthkumar  (1001) hemanthkumar  (1001)     3619 2023-11-23 12:05:51.000000 phenomApis-0.0.8/phenom/api/exsearch/models/filters_node.py
--rw-r--r--   0 hemanthkumar  (1001) hemanthkumar  (1001)     3912 2023-11-23 12:05:51.000000 phenomApis-0.0.8/phenom/api/exsearch/models/mentor_type_ahead_request.py
--rw-r--r--   0 hemanthkumar  (1001) hemanthkumar  (1001)     3823 2023-11-23 12:05:51.000000 phenomApis-0.0.8/phenom/api/exsearch/models/mentor_typeahead_response.py
--rw-r--r--   0 hemanthkumar  (1001) hemanthkumar  (1001)     4316 2023-11-23 12:05:51.000000 phenomApis-0.0.8/phenom/api/exsearch/models/tab_info_node.py
-drwxr-xr-x   0 hemanthkumar  (1001) hemanthkumar  (1001)        0 2023-11-27 09:14:32.868135 phenomApis-0.0.8/phenom/api/prediction/
--rw-r--r--   0 hemanthkumar  (1001) hemanthkumar  (1001)      809 2023-11-24 06:33:31.000000 phenomApis-0.0.8/phenom/api/prediction/__init__.py
-drwxr-xr-x   0 hemanthkumar  (1001) hemanthkumar  (1001)        0 2023-11-27 09:14:32.868135 phenomApis-0.0.8/phenom/api/prediction/models/
--rw-r--r--   0 hemanthkumar  (1001) hemanthkumar  (1001)      697 2023-11-24 06:33:31.000000 phenomApis-0.0.8/phenom/api/prediction/models/__init__.py
--rw-r--r--   0 hemanthkumar  (1001) hemanthkumar  (1001)     3586 2023-11-21 13:13:54.000000 phenomApis-0.0.8/phenom/api/prediction/models/bad_request.py
--rw-r--r--   0 hemanthkumar  (1001) hemanthkumar  (1001)     3622 2023-11-21 13:13:54.000000 phenomApis-0.0.8/phenom/api/prediction/models/error_response.py
--rw-r--r--   0 hemanthkumar  (1001) hemanthkumar  (1001)     5605 2023-11-21 13:13:54.000000 phenomApis-0.0.8/phenom/api/prediction/models/fyf_skill_request.py
--rw-r--r--   0 hemanthkumar  (1001) hemanthkumar  (1001)     5075 2023-11-21 13:13:54.000000 phenomApis-0.0.8/phenom/api/prediction/models/fyf_skill_response.py
--rw-r--r--   0 hemanthkumar  (1001) hemanthkumar  (1001)     3544 2023-11-21 13:13:54.000000 phenomApis-0.0.8/phenom/api/prediction/models/skill_result.py
--rw-r--r--   0 hemanthkumar  (1001) hemanthkumar  (1001)     3035 2023-11-21 13:13:54.000000 phenomApis-0.0.8/phenom/api/prediction/models/skill_results.py
--rw-r--r--   0 hemanthkumar  (1001) hemanthkumar  (1001)     4452 2023-11-24 06:50:15.000000 phenomApis-0.0.8/phenom/api/prediction/prediction_api.py
-drwxr-xr-x   0 hemanthkumar  (1001) hemanthkumar  (1001)        0 2023-11-27 09:14:32.872135 phenomApis-0.0.8/phenom/api/resumeparser/
--rw-r--r--   0 hemanthkumar  (1001) hemanthkumar  (1001)     2209 2023-11-23 16:32:42.000000 phenomApis-0.0.8/phenom/api/resumeparser/__init__.py
-drwxr-xr-x   0 hemanthkumar  (1001) hemanthkumar  (1001)        0 2023-11-27 09:14:32.884135 phenomApis-0.0.8/phenom/api/resumeparser/models/
--rw-r--r--   0 hemanthkumar  (1001) hemanthkumar  (1001)     2087 2023-11-23 16:33:39.000000 phenomApis-0.0.8/phenom/api/resumeparser/models/__init__.py
--rw-r--r--   0 hemanthkumar  (1001) hemanthkumar  (1001)     3952 2023-11-23 16:33:59.000000 phenomApis-0.0.8/phenom/api/resumeparser/models/error_response.py
--rw-r--r--   0 hemanthkumar  (1001) hemanthkumar  (1001)     6143 2023-11-21 11:21:50.000000 phenomApis-0.0.8/phenom/api/resumeparser/models/error_response_errors.py
--rw-r--r--   0 hemanthkumar  (1001) hemanthkumar  (1001)     3171 2023-11-21 11:21:50.000000 phenomApis-0.0.8/phenom/api/resumeparser/models/resume_file_request.py
--rw-r--r--   0 hemanthkumar  (1001) hemanthkumar  (1001)     3920 2023-11-21 11:21:50.000000 phenomApis-0.0.8/phenom/api/resumeparser/models/resume_request.py
--rw-r--r--   0 hemanthkumar  (1001) hemanthkumar  (1001)     5992 2023-11-23 16:34:10.000000 phenomApis-0.0.8/phenom/api/resumeparser/models/resume_response.py
--rw-r--r--   0 hemanthkumar  (1001) hemanthkumar  (1001)     3497 2023-11-23 16:34:57.000000 phenomApis-0.0.8/phenom/api/resumeparser/models/resume_response_data.py
--rw-r--r--   0 hemanthkumar  (1001) hemanthkumar  (1001)    17639 2023-11-23 16:35:31.000000 phenomApis-0.0.8/phenom/api/resumeparser/models/resume_response_data_resumedata.py
--rw-r--r--   0 hemanthkumar  (1001) hemanthkumar  (1001)     8742 2023-11-21 11:21:50.000000 phenomApis-0.0.8/phenom/api/resumeparser/models/resume_response_data_resumedata_educationhistory.py
--rw-r--r--   0 hemanthkumar  (1001) hemanthkumar  (1001)     9109 2023-11-21 11:21:50.000000 phenomApis-0.0.8/phenom/api/resumeparser/models/resume_response_data_resumedata_experiencesummary.py
--rw-r--r--   0 hemanthkumar  (1001) hemanthkumar  (1001)     4060 2023-11-21 11:21:50.000000 phenomApis-0.0.8/phenom/api/resumeparser/models/resume_response_data_resumedata_internetaddress.py
--rw-r--r--   0 hemanthkumar  (1001) hemanthkumar  (1001)     4232 2023-11-21 11:21:50.000000 phenomApis-0.0.8/phenom/api/resumeparser/models/resume_response_data_resumedata_mobile.py
--rw-r--r--   0 hemanthkumar  (1001) hemanthkumar  (1001)     5762 2023-11-21 11:21:50.000000 phenomApis-0.0.8/phenom/api/resumeparser/models/resume_response_data_resumedata_personname.py
--rw-r--r--   0 hemanthkumar  (1001) hemanthkumar  (1001)     7208 2023-11-21 11:21:50.000000 phenomApis-0.0.8/phenom/api/resumeparser/models/resume_response_data_resumedata_postaladdress.py
--rw-r--r--   0 hemanthkumar  (1001) hemanthkumar  (1001)     5902 2023-11-21 11:21:50.000000 phenomApis-0.0.8/phenom/api/resumeparser/models/resume_response_data_resumedata_skilltaxonomy.py
--rw-r--r--   0 hemanthkumar  (1001) hemanthkumar  (1001)     9325 2023-11-21 11:21:51.000000 phenomApis-0.0.8/phenom/api/resumeparser/models/resume_response_data_resumedata_workhistory.py
--rw-r--r--   0 hemanthkumar  (1001) hemanthkumar  (1001)     8212 2023-11-24 06:50:15.000000 phenomApis-0.0.8/phenom/api/resumeparser/resume_parsing_api.py
-drwxr-xr-x   0 hemanthkumar  (1001) hemanthkumar  (1001)        0 2023-11-27 09:14:32.884135 phenomApis-0.0.8/phenom/api/search/
--rw-r--r--   0 hemanthkumar  (1001) hemanthkumar  (1001)     1375 2023-11-27 09:03:03.000000 phenomApis-0.0.8/phenom/api/search/__init__.py
--rw-r--r--   0 hemanthkumar  (1001) hemanthkumar  (1001)     8529 2023-11-27 09:04:17.000000 phenomApis-0.0.8/phenom/api/search/jobs_api.py
-drwxr-xr-x   0 hemanthkumar  (1001) hemanthkumar  (1001)        0 2023-11-27 09:14:32.888135 phenomApis-0.0.8/phenom/api/search/models/
--rw-r--r--   0 hemanthkumar  (1001) hemanthkumar  (1001)     1176 2023-11-27 09:01:59.000000 phenomApis-0.0.8/phenom/api/search/models/__init__.py
--rw-r--r--   0 hemanthkumar  (1001) hemanthkumar  (1001)     3643 2023-11-27 08:58:02.000000 phenomApis-0.0.8/phenom/api/search/models/bad_request.py
--rw-r--r--   0 hemanthkumar  (1001) hemanthkumar  (1001)     3679 2023-11-27 08:58:02.000000 phenomApis-0.0.8/phenom/api/search/models/error_response.py
--rw-r--r--   0 hemanthkumar  (1001) hemanthkumar  (1001)     5317 2023-11-27 08:58:02.000000 phenomApis-0.0.8/phenom/api/search/models/job_node.py
--rw-r--r--   0 hemanthkumar  (1001) hemanthkumar  (1001)     3721 2023-11-27 08:58:02.000000 phenomApis-0.0.8/phenom/api/search/models/job_titles_response.py
--rw-r--r--   0 hemanthkumar  (1001) hemanthkumar  (1001)     3192 2023-11-27 08:58:02.000000 phenomApis-0.0.8/phenom/api/search/models/job_titles_response_data.py
--rw-r--r--   0 hemanthkumar  (1001) hemanthkumar  (1001)     4563 2023-11-27 08:58:02.000000 phenomApis-0.0.8/phenom/api/search/models/job_titles_response_data_titles.py
--rw-r--r--   0 hemanthkumar  (1001) hemanthkumar  (1001)     5040 2023-11-27 08:58:02.000000 phenomApis-0.0.8/phenom/api/search/models/location_data.py
--rw-r--r--   0 hemanthkumar  (1001) hemanthkumar  (1001)    10387 2023-11-27 08:58:02.000000 phenomApis-0.0.8/phenom/api/search/models/refine_search_request.py
--rw-r--r--   0 hemanthkumar  (1001) hemanthkumar  (1001)     5213 2023-11-27 08:58:02.000000 phenomApis-0.0.8/phenom/api/search/models/refine_search_request_facets.py
--rw-r--r--   0 hemanthkumar  (1001) hemanthkumar  (1001)     3766 2023-11-27 08:58:02.000000 phenomApis-0.0.8/phenom/api/search/models/refine_search_response.py
--rw-r--r--   0 hemanthkumar  (1001) hemanthkumar  (1001)     3116 2023-11-27 08:58:02.000000 phenomApis-0.0.8/phenom/api/search/models/refine_search_response_data.py
-drwxr-xr-x   0 hemanthkumar  (1001) hemanthkumar  (1001)        0 2023-11-27 09:14:32.896135 phenomApis-0.0.8/phenom/commons/
--rw-r--r--   0 hemanthkumar  (1001) hemanthkumar  (1001)        0 2023-10-25 06:34:37.000000 phenomApis-0.0.8/phenom/commons/__init__.py
--rw-r--r--   0 hemanthkumar  (1001) hemanthkumar  (1001)    23936 2023-11-24 06:50:15.000000 phenomApis-0.0.8/phenom/commons/api_client.py
--rw-r--r--   0 hemanthkumar  (1001) hemanthkumar  (1001)     1382 2023-11-27 09:06:15.000000 phenomApis-0.0.8/phenom/commons/authorization.py
--rw-r--r--   0 hemanthkumar  (1001) hemanthkumar  (1001)     7574 2023-11-24 06:05:16.000000 phenomApis-0.0.8/phenom/commons/configuration.py
--rw-r--r--   0 hemanthkumar  (1001) hemanthkumar  (1001)     1473 2023-10-20 07:05:34.000000 phenomApis-0.0.8/phenom/commons/get_token.py
--rw-r--r--   0 hemanthkumar  (1001) hemanthkumar  (1001)    12769 2023-11-08 11:23:40.000000 phenomApis-0.0.8/phenom/commons/rest.py
-drwxr-xr-x   0 hemanthkumar  (1001) hemanthkumar  (1001)        0 2023-11-27 09:14:32.896135 phenomApis-0.0.8/phenomApis.egg-info/
--rw-r--r--   0 hemanthkumar  (1001) hemanthkumar  (1001)      650 2023-11-27 09:14:32.000000 phenomApis-0.0.8/phenomApis.egg-info/PKG-INFO
--rw-r--r--   0 hemanthkumar  (1001) hemanthkumar  (1001)     4441 2023-11-27 09:14:32.000000 phenomApis-0.0.8/phenomApis.egg-info/SOURCES.txt
--rw-r--r--   0 hemanthkumar  (1001) hemanthkumar  (1001)        1 2023-11-27 09:14:32.000000 phenomApis-0.0.8/phenomApis.egg-info/dependency_links.txt
--rw-r--r--   0 hemanthkumar  (1001) hemanthkumar  (1001)       60 2023-11-27 09:14:32.000000 phenomApis-0.0.8/phenomApis.egg-info/requires.txt
--rw-r--r--   0 hemanthkumar  (1001) hemanthkumar  (1001)       12 2023-11-27 09:14:32.000000 phenomApis-0.0.8/phenomApis.egg-info/top_level.txt
--rw-r--r--   0 hemanthkumar  (1001) hemanthkumar  (1001)       38 2023-11-27 09:14:32.900135 phenomApis-0.0.8/setup.cfg
--rw-r--r--   0 hemanthkumar  (1001) hemanthkumar  (1001)      879 2023-11-27 09:09:23.000000 phenomApis-0.0.8/setup.py
-drwxr-xr-x   0 hemanthkumar  (1001) hemanthkumar  (1001)        0 2023-11-27 09:14:32.896135 phenomApis-0.0.8/test/
--rw-r--r--   0 hemanthkumar  (1001) hemanthkumar  (1001)        0 2023-11-27 09:09:06.000000 phenomApis-0.0.8/test/__init__.py
+drwxr-xr-x   0 hemanthkumar  (1001) hemanthkumar  (1001)        0 2023-11-27 10:49:40.615926 phenomApis-0.0.9/
+-rw-r--r--   0 hemanthkumar  (1001) hemanthkumar  (1001)     1062 2023-11-21 11:14:01.000000 phenomApis-0.0.9/LICENSE
+-rw-r--r--   0 hemanthkumar  (1001) hemanthkumar  (1001)      650 2023-11-27 10:49:40.611925 phenomApis-0.0.9/PKG-INFO
+drwxr-xr-x   0 hemanthkumar  (1001) hemanthkumar  (1001)        0 2023-11-27 10:49:40.571925 phenomApis-0.0.9/phenom/
+-rw-r--r--   0 hemanthkumar  (1001) hemanthkumar  (1001)        0 2023-11-23 16:51:34.000000 phenomApis-0.0.9/phenom/__init__.py
+drwxr-xr-x   0 hemanthkumar  (1001) hemanthkumar  (1001)        0 2023-11-27 10:49:40.575926 phenomApis-0.0.9/phenom/api/
+-rw-r--r--   0 hemanthkumar  (1001) hemanthkumar  (1001)        0 2023-11-27 10:42:27.000000 phenomApis-0.0.9/phenom/api/__init__.py
+drwxr-xr-x   0 hemanthkumar  (1001) hemanthkumar  (1001)        0 2023-11-27 10:49:40.575926 phenomApis-0.0.9/phenom/api/aisourcing/
+-rw-r--r--   0 hemanthkumar  (1001) hemanthkumar  (1001)     1312 2023-11-27 10:42:26.000000 phenomApis-0.0.9/phenom/api/aisourcing/__init__.py
+-rw-r--r--   0 hemanthkumar  (1001) hemanthkumar  (1001)     8820 2023-11-27 10:42:26.000000 phenomApis-0.0.9/phenom/api/aisourcing/ai_matching_api.py
+drwxr-xr-x   0 hemanthkumar  (1001) hemanthkumar  (1001)        0 2023-11-27 10:49:40.575926 phenomApis-0.0.9/phenom/api/aisourcing/models/
+-rw-r--r--   0 hemanthkumar  (1001) hemanthkumar  (1001)     1199 2023-11-27 10:42:26.000000 phenomApis-0.0.9/phenom/api/aisourcing/models/__init__.py
+-rw-r--r--   0 hemanthkumar  (1001) hemanthkumar  (1001)     3397 2023-11-27 10:42:26.000000 phenomApis-0.0.9/phenom/api/aisourcing/models/error_response.py
+-rw-r--r--   0 hemanthkumar  (1001) hemanthkumar  (1001)     4253 2023-11-27 10:42:26.000000 phenomApis-0.0.9/phenom/api/aisourcing/models/fit_score_request.py
+-rw-r--r--   0 hemanthkumar  (1001) hemanthkumar  (1001)     3457 2023-11-27 10:42:26.000000 phenomApis-0.0.9/phenom/api/aisourcing/models/fitscore_bad_request.py
+-rw-r--r--   0 hemanthkumar  (1001) hemanthkumar  (1001)     3488 2023-11-27 10:42:26.000000 phenomApis-0.0.9/phenom/api/aisourcing/models/fitscore_response.py
+-rw-r--r--   0 hemanthkumar  (1001) hemanthkumar  (1001)     7346 2023-11-27 10:42:26.000000 phenomApis-0.0.9/phenom/api/aisourcing/models/fitscore_response_result.py
+-rw-r--r--   0 hemanthkumar  (1001) hemanthkumar  (1001)     4525 2023-11-27 10:42:26.000000 phenomApis-0.0.9/phenom/api/aisourcing/models/fitscore_response_skill_gap.py
+-rw-r--r--   0 hemanthkumar  (1001) hemanthkumar  (1001)     3563 2023-11-27 10:42:26.000000 phenomApis-0.0.9/phenom/api/aisourcing/models/preferred_locations.py
+-rw-r--r--   0 hemanthkumar  (1001) hemanthkumar  (1001)     3413 2023-11-27 10:42:26.000000 phenomApis-0.0.9/phenom/api/aisourcing/models/preferred_locations_latlong.py
+-rw-r--r--   0 hemanthkumar  (1001) hemanthkumar  (1001)     3156 2023-11-27 10:42:26.000000 phenomApis-0.0.9/phenom/api/aisourcing/models/skill_matching_bad_request.py
+-rw-r--r--   0 hemanthkumar  (1001) hemanthkumar  (1001)     3180 2023-11-27 10:42:26.000000 phenomApis-0.0.9/phenom/api/aisourcing/models/skill_matching_error_response.py
+-rw-r--r--   0 hemanthkumar  (1001) hemanthkumar  (1001)     3968 2023-11-27 10:42:26.000000 phenomApis-0.0.9/phenom/api/aisourcing/models/skill_matching_response.py
+-rw-r--r--   0 hemanthkumar  (1001) hemanthkumar  (1001)     5317 2023-11-27 10:42:26.000000 phenomApis-0.0.9/phenom/api/aisourcing/models/user_profile_fit_score.py
+drwxr-xr-x   0 hemanthkumar  (1001) hemanthkumar  (1001)        0 2023-11-27 10:49:40.575926 phenomApis-0.0.9/phenom/api/exsearch/
+-rw-r--r--   0 hemanthkumar  (1001) hemanthkumar  (1001)     1854 2023-11-27 10:42:27.000000 phenomApis-0.0.9/phenom/api/exsearch/__init__.py
+-rw-r--r--   0 hemanthkumar  (1001) hemanthkumar  (1001)    11481 2023-11-27 10:42:27.000000 phenomApis-0.0.9/phenom/api/exsearch/employees_api.py
+-rw-r--r--   0 hemanthkumar  (1001) hemanthkumar  (1001)     4176 2023-11-27 10:42:27.000000 phenomApis-0.0.9/phenom/api/exsearch/mentor_api.py
+drwxr-xr-x   0 hemanthkumar  (1001) hemanthkumar  (1001)        0 2023-11-27 10:49:40.579926 phenomApis-0.0.9/phenom/api/exsearch/models/
+-rw-r--r--   0 hemanthkumar  (1001) hemanthkumar  (1001)     1693 2023-11-27 10:42:27.000000 phenomApis-0.0.9/phenom/api/exsearch/models/__init__.py
+-rw-r--r--   0 hemanthkumar  (1001) hemanthkumar  (1001)     3414 2023-11-27 10:42:27.000000 phenomApis-0.0.9/phenom/api/exsearch/models/aggregations_node.py
+-rw-r--r--   0 hemanthkumar  (1001) hemanthkumar  (1001)     4628 2023-11-27 10:42:27.000000 phenomApis-0.0.9/phenom/api/exsearch/models/bad_request.py
+-rw-r--r--   0 hemanthkumar  (1001) hemanthkumar  (1001)     4108 2023-11-27 10:42:27.000000 phenomApis-0.0.9/phenom/api/exsearch/models/common_node.py
+-rw-r--r--   0 hemanthkumar  (1001) hemanthkumar  (1001)     7224 2023-11-27 10:42:27.000000 phenomApis-0.0.9/phenom/api/exsearch/models/employee_node.py
+-rw-r--r--   0 hemanthkumar  (1001) hemanthkumar  (1001)     6367 2023-11-27 10:42:27.000000 phenomApis-0.0.9/phenom/api/exsearch/models/employee_search_request.py
+-rw-r--r--   0 hemanthkumar  (1001) hemanthkumar  (1001)     4311 2023-11-27 10:42:27.000000 phenomApis-0.0.9/phenom/api/exsearch/models/employee_search_response.py
+-rw-r--r--   0 hemanthkumar  (1001) hemanthkumar  (1001)     3738 2023-11-27 10:42:27.000000 phenomApis-0.0.9/phenom/api/exsearch/models/employee_search_response_data.py
+-rw-r--r--   0 hemanthkumar  (1001) hemanthkumar  (1001)     4599 2023-11-27 10:42:27.000000 phenomApis-0.0.9/phenom/api/exsearch/models/employee_type_ahead_agg_request.py
+-rw-r--r--   0 hemanthkumar  (1001) hemanthkumar  (1001)     3709 2023-11-27 10:42:27.000000 phenomApis-0.0.9/phenom/api/exsearch/models/employee_type_ahead_request.py
+-rw-r--r--   0 hemanthkumar  (1001) hemanthkumar  (1001)     3587 2023-11-27 10:42:27.000000 phenomApis-0.0.9/phenom/api/exsearch/models/employee_typeahead_agg_response.py
+-rw-r--r--   0 hemanthkumar  (1001) hemanthkumar  (1001)     4997 2023-11-27 10:42:27.000000 phenomApis-0.0.9/phenom/api/exsearch/models/employee_typeahead_response.py
+-rw-r--r--   0 hemanthkumar  (1001) hemanthkumar  (1001)     3050 2023-11-27 10:42:27.000000 phenomApis-0.0.9/phenom/api/exsearch/models/employee_typeahead_response_data.py
+-rw-r--r--   0 hemanthkumar  (1001) hemanthkumar  (1001)     4688 2023-11-27 10:42:27.000000 phenomApis-0.0.9/phenom/api/exsearch/models/error_response.py
+-rw-r--r--   0 hemanthkumar  (1001) hemanthkumar  (1001)     3920 2023-11-27 10:42:27.000000 phenomApis-0.0.9/phenom/api/exsearch/models/facets_node.py
+-rw-r--r--   0 hemanthkumar  (1001) hemanthkumar  (1001)     3392 2023-11-27 10:42:27.000000 phenomApis-0.0.9/phenom/api/exsearch/models/filters_node.py
+-rw-r--r--   0 hemanthkumar  (1001) hemanthkumar  (1001)     3685 2023-11-27 10:42:27.000000 phenomApis-0.0.9/phenom/api/exsearch/models/mentor_type_ahead_request.py
+-rw-r--r--   0 hemanthkumar  (1001) hemanthkumar  (1001)     3596 2023-11-27 10:42:27.000000 phenomApis-0.0.9/phenom/api/exsearch/models/mentor_typeahead_response.py
+-rw-r--r--   0 hemanthkumar  (1001) hemanthkumar  (1001)     4089 2023-11-27 10:42:27.000000 phenomApis-0.0.9/phenom/api/exsearch/models/tab_info_node.py
+drwxr-xr-x   0 hemanthkumar  (1001) hemanthkumar  (1001)        0 2023-11-27 10:49:40.579926 phenomApis-0.0.9/phenom/api/jobparser/
+-rw-r--r--   0 hemanthkumar  (1001) hemanthkumar  (1001)      899 2023-11-27 10:42:26.000000 phenomApis-0.0.9/phenom/api/jobparser/__init__.py
+-rw-r--r--   0 hemanthkumar  (1001) hemanthkumar  (1001)     4272 2023-11-27 10:42:26.000000 phenomApis-0.0.9/phenom/api/jobparser/job_parsing_api.py
+drwxr-xr-x   0 hemanthkumar  (1001) hemanthkumar  (1001)        0 2023-11-27 10:49:40.583926 phenomApis-0.0.9/phenom/api/jobparser/models/
+-rw-r--r--   0 hemanthkumar  (1001) hemanthkumar  (1001)      684 2023-11-27 10:42:27.000000 phenomApis-0.0.9/phenom/api/jobparser/models/__init__.py
+-rw-r--r--   0 hemanthkumar  (1001) hemanthkumar  (1001)     3109 2023-11-27 10:42:27.000000 phenomApis-0.0.9/phenom/api/jobparser/models/jd_request.py
+-rw-r--r--   0 hemanthkumar  (1001) hemanthkumar  (1001)    18088 2023-11-27 10:42:27.000000 phenomApis-0.0.9/phenom/api/jobparser/models/job_response.py
+-rw-r--r--   0 hemanthkumar  (1001) hemanthkumar  (1001)     3110 2023-11-27 10:42:26.000000 phenomApis-0.0.9/phenom/api/jobparser/models/trigger400_response.py
+-rw-r--r--   0 hemanthkumar  (1001) hemanthkumar  (1001)     5777 2023-11-27 10:42:27.000000 phenomApis-0.0.9/phenom/api/jobparser/models/trigger400_response_response.py
+drwxr-xr-x   0 hemanthkumar  (1001) hemanthkumar  (1001)        0 2023-11-27 10:49:40.583926 phenomApis-0.0.9/phenom/api/prediction/
+-rw-r--r--   0 hemanthkumar  (1001) hemanthkumar  (1001)      708 2023-11-27 10:42:26.000000 phenomApis-0.0.9/phenom/api/prediction/__init__.py
+drwxr-xr-x   0 hemanthkumar  (1001) hemanthkumar  (1001)        0 2023-11-27 10:49:40.587926 phenomApis-0.0.9/phenom/api/prediction/models/
+-rw-r--r--   0 hemanthkumar  (1001) hemanthkumar  (1001)      596 2023-11-27 10:42:26.000000 phenomApis-0.0.9/phenom/api/prediction/models/__init__.py
+-rw-r--r--   0 hemanthkumar  (1001) hemanthkumar  (1001)     3359 2023-11-27 10:42:26.000000 phenomApis-0.0.9/phenom/api/prediction/models/bad_request.py
+-rw-r--r--   0 hemanthkumar  (1001) hemanthkumar  (1001)     3395 2023-11-27 10:42:26.000000 phenomApis-0.0.9/phenom/api/prediction/models/error_response.py
+-rw-r--r--   0 hemanthkumar  (1001) hemanthkumar  (1001)     5378 2023-11-27 10:42:26.000000 phenomApis-0.0.9/phenom/api/prediction/models/fyf_skill_request.py
+-rw-r--r--   0 hemanthkumar  (1001) hemanthkumar  (1001)     4848 2023-11-27 10:42:26.000000 phenomApis-0.0.9/phenom/api/prediction/models/fyf_skill_response.py
+-rw-r--r--   0 hemanthkumar  (1001) hemanthkumar  (1001)     3317 2023-11-27 10:42:26.000000 phenomApis-0.0.9/phenom/api/prediction/models/skill_result.py
+-rw-r--r--   0 hemanthkumar  (1001) hemanthkumar  (1001)     2808 2023-11-27 10:42:26.000000 phenomApis-0.0.9/phenom/api/prediction/models/skill_results.py
+-rw-r--r--   0 hemanthkumar  (1001) hemanthkumar  (1001)     4169 2023-11-27 10:42:26.000000 phenomApis-0.0.9/phenom/api/prediction/prediction_api.py
+drwxr-xr-x   0 hemanthkumar  (1001) hemanthkumar  (1001)        0 2023-11-27 10:49:40.587926 phenomApis-0.0.9/phenom/api/recomendation/
+-rw-r--r--   0 hemanthkumar  (1001) hemanthkumar  (1001)     1961 2023-11-27 10:42:26.000000 phenomApis-0.0.9/phenom/api/recomendation/__init__.py
+drwxr-xr-x   0 hemanthkumar  (1001) hemanthkumar  (1001)        0 2023-11-27 10:49:40.595926 phenomApis-0.0.9/phenom/api/recomendation/models/
+-rw-r--r--   0 hemanthkumar  (1001) hemanthkumar  (1001)     1754 2023-11-27 10:42:26.000000 phenomApis-0.0.9/phenom/api/recomendation/models/__init__.py
+-rw-r--r--   0 hemanthkumar  (1001) hemanthkumar  (1001)     3413 2023-11-27 10:42:26.000000 phenomApis-0.0.9/phenom/api/recomendation/models/bad_request.py
+-rw-r--r--   0 hemanthkumar  (1001) hemanthkumar  (1001)     3449 2023-11-27 10:42:26.000000 phenomApis-0.0.9/phenom/api/recomendation/models/error_response.py
+-rw-r--r--   0 hemanthkumar  (1001) hemanthkumar  (1001)     5087 2023-11-27 10:42:26.000000 phenomApis-0.0.9/phenom/api/recomendation/models/job_node.py
+-rw-r--r--   0 hemanthkumar  (1001) hemanthkumar  (1001)     6655 2023-11-27 10:42:26.000000 phenomApis-0.0.9/phenom/api/recomendation/models/job_recommendation.py
+-rw-r--r--   0 hemanthkumar  (1001) hemanthkumar  (1001)     3506 2023-11-27 10:42:26.000000 phenomApis-0.0.9/phenom/api/recomendation/models/near_by_jobs_response.py
+-rw-r--r--   0 hemanthkumar  (1001) hemanthkumar  (1001)     2990 2023-11-27 10:42:26.000000 phenomApis-0.0.9/phenom/api/recomendation/models/near_by_jobs_response_data.py
+-rw-r--r--   0 hemanthkumar  (1001) hemanthkumar  (1001)     3615 2023-11-27 10:42:26.000000 phenomApis-0.0.9/phenom/api/recomendation/models/preferred_locations.py
+-rw-r--r--   0 hemanthkumar  (1001) hemanthkumar  (1001)     3465 2023-11-27 10:42:26.000000 phenomApis-0.0.9/phenom/api/recomendation/models/preferred_locations_latlong.py
+-rw-r--r--   0 hemanthkumar  (1001) hemanthkumar  (1001)     4359 2023-11-27 10:42:26.000000 phenomApis-0.0.9/phenom/api/recomendation/models/profile_matching_response.py
+-rw-r--r--   0 hemanthkumar  (1001) hemanthkumar  (1001)     9189 2023-11-27 10:42:26.000000 phenomApis-0.0.9/phenom/api/recomendation/models/profile_matching_response_jobs.py
+-rw-r--r--   0 hemanthkumar  (1001) hemanthkumar  (1001)     5919 2023-11-27 10:42:26.000000 phenomApis-0.0.9/phenom/api/recomendation/models/profile_matching_response_location_data.py
+-rw-r--r--   0 hemanthkumar  (1001) hemanthkumar  (1001)     4689 2023-11-27 10:42:26.000000 phenomApis-0.0.9/phenom/api/recomendation/models/profile_matching_response_skill_gap.py
+-rw-r--r--   0 hemanthkumar  (1001) hemanthkumar  (1001)     5430 2023-11-27 10:42:26.000000 phenomApis-0.0.9/phenom/api/recomendation/models/similar_jobs_request.py
+-rw-r--r--   0 hemanthkumar  (1001) hemanthkumar  (1001)     3521 2023-11-27 10:42:26.000000 phenomApis-0.0.9/phenom/api/recomendation/models/similar_jobs_response.py
+-rw-r--r--   0 hemanthkumar  (1001) hemanthkumar  (1001)     3118 2023-11-27 10:42:26.000000 phenomApis-0.0.9/phenom/api/recomendation/models/similar_jobs_response_data.py
+-rw-r--r--   0 hemanthkumar  (1001) hemanthkumar  (1001)     5955 2023-11-27 10:42:26.000000 phenomApis-0.0.9/phenom/api/recomendation/models/similar_jobs_response_data_similar_jobs.py
+-rw-r--r--   0 hemanthkumar  (1001) hemanthkumar  (1001)     5920 2023-11-27 10:42:26.000000 phenomApis-0.0.9/phenom/api/recomendation/models/user_profile.py
+-rw-r--r--   0 hemanthkumar  (1001) hemanthkumar  (1001)    12754 2023-11-27 10:42:26.000000 phenomApis-0.0.9/phenom/api/recomendation/recommendations_api.py
+drwxr-xr-x   0 hemanthkumar  (1001) hemanthkumar  (1001)        0 2023-11-27 10:49:40.595926 phenomApis-0.0.9/phenom/api/resumeparser/
+-rw-r--r--   0 hemanthkumar  (1001) hemanthkumar  (1001)     2108 2023-11-27 10:42:27.000000 phenomApis-0.0.9/phenom/api/resumeparser/__init__.py
+drwxr-xr-x   0 hemanthkumar  (1001) hemanthkumar  (1001)        0 2023-11-27 10:49:40.599926 phenomApis-0.0.9/phenom/api/resumeparser/models/
+-rw-r--r--   0 hemanthkumar  (1001) hemanthkumar  (1001)     1986 2023-11-27 10:42:27.000000 phenomApis-0.0.9/phenom/api/resumeparser/models/__init__.py
+-rw-r--r--   0 hemanthkumar  (1001) hemanthkumar  (1001)     3725 2023-11-27 10:42:27.000000 phenomApis-0.0.9/phenom/api/resumeparser/models/error_response.py
+-rw-r--r--   0 hemanthkumar  (1001) hemanthkumar  (1001)     5916 2023-11-27 10:42:27.000000 phenomApis-0.0.9/phenom/api/resumeparser/models/error_response_errors.py
+-rw-r--r--   0 hemanthkumar  (1001) hemanthkumar  (1001)     2944 2023-11-27 10:42:27.000000 phenomApis-0.0.9/phenom/api/resumeparser/models/resume_file_request.py
+-rw-r--r--   0 hemanthkumar  (1001) hemanthkumar  (1001)     3693 2023-11-27 10:42:27.000000 phenomApis-0.0.9/phenom/api/resumeparser/models/resume_request.py
+-rw-r--r--   0 hemanthkumar  (1001) hemanthkumar  (1001)     5765 2023-11-27 10:42:27.000000 phenomApis-0.0.9/phenom/api/resumeparser/models/resume_response.py
+-rw-r--r--   0 hemanthkumar  (1001) hemanthkumar  (1001)     3270 2023-11-27 10:42:27.000000 phenomApis-0.0.9/phenom/api/resumeparser/models/resume_response_data.py
+-rw-r--r--   0 hemanthkumar  (1001) hemanthkumar  (1001)    17412 2023-11-27 10:42:27.000000 phenomApis-0.0.9/phenom/api/resumeparser/models/resume_response_data_resumedata.py
+-rw-r--r--   0 hemanthkumar  (1001) hemanthkumar  (1001)     8515 2023-11-27 10:42:27.000000 phenomApis-0.0.9/phenom/api/resumeparser/models/resume_response_data_resumedata_educationhistory.py
+-rw-r--r--   0 hemanthkumar  (1001) hemanthkumar  (1001)     8882 2023-11-27 10:42:27.000000 phenomApis-0.0.9/phenom/api/resumeparser/models/resume_response_data_resumedata_experiencesummary.py
+-rw-r--r--   0 hemanthkumar  (1001) hemanthkumar  (1001)     3833 2023-11-27 10:42:27.000000 phenomApis-0.0.9/phenom/api/resumeparser/models/resume_response_data_resumedata_internetaddress.py
+-rw-r--r--   0 hemanthkumar  (1001) hemanthkumar  (1001)     4005 2023-11-27 10:42:27.000000 phenomApis-0.0.9/phenom/api/resumeparser/models/resume_response_data_resumedata_mobile.py
+-rw-r--r--   0 hemanthkumar  (1001) hemanthkumar  (1001)     5535 2023-11-27 10:42:27.000000 phenomApis-0.0.9/phenom/api/resumeparser/models/resume_response_data_resumedata_personname.py
+-rw-r--r--   0 hemanthkumar  (1001) hemanthkumar  (1001)     6981 2023-11-27 10:42:27.000000 phenomApis-0.0.9/phenom/api/resumeparser/models/resume_response_data_resumedata_postaladdress.py
+-rw-r--r--   0 hemanthkumar  (1001) hemanthkumar  (1001)     5675 2023-11-27 10:42:27.000000 phenomApis-0.0.9/phenom/api/resumeparser/models/resume_response_data_resumedata_skilltaxonomy.py
+-rw-r--r--   0 hemanthkumar  (1001) hemanthkumar  (1001)     9098 2023-11-27 10:42:27.000000 phenomApis-0.0.9/phenom/api/resumeparser/models/resume_response_data_resumedata_workhistory.py
+-rw-r--r--   0 hemanthkumar  (1001) hemanthkumar  (1001)     7929 2023-11-27 10:42:27.000000 phenomApis-0.0.9/phenom/api/resumeparser/resume_parsing_api.py
+drwxr-xr-x   0 hemanthkumar  (1001) hemanthkumar  (1001)        0 2023-11-27 10:49:40.599926 phenomApis-0.0.9/phenom/api/search/
+-rw-r--r--   0 hemanthkumar  (1001) hemanthkumar  (1001)     1274 2023-11-27 10:42:27.000000 phenomApis-0.0.9/phenom/api/search/__init__.py
+-rw-r--r--   0 hemanthkumar  (1001) hemanthkumar  (1001)     8246 2023-11-27 10:42:27.000000 phenomApis-0.0.9/phenom/api/search/jobs_api.py
+drwxr-xr-x   0 hemanthkumar  (1001) hemanthkumar  (1001)        0 2023-11-27 10:49:40.611925 phenomApis-0.0.9/phenom/api/search/models/
+-rw-r--r--   0 hemanthkumar  (1001) hemanthkumar  (1001)     1075 2023-11-27 10:42:27.000000 phenomApis-0.0.9/phenom/api/search/models/__init__.py
+-rw-r--r--   0 hemanthkumar  (1001) hemanthkumar  (1001)     3416 2023-11-27 10:42:27.000000 phenomApis-0.0.9/phenom/api/search/models/bad_request.py
+-rw-r--r--   0 hemanthkumar  (1001) hemanthkumar  (1001)     3452 2023-11-27 10:42:27.000000 phenomApis-0.0.9/phenom/api/search/models/error_response.py
+-rw-r--r--   0 hemanthkumar  (1001) hemanthkumar  (1001)     5090 2023-11-27 10:42:27.000000 phenomApis-0.0.9/phenom/api/search/models/job_node.py
+-rw-r--r--   0 hemanthkumar  (1001) hemanthkumar  (1001)     3494 2023-11-27 10:42:27.000000 phenomApis-0.0.9/phenom/api/search/models/job_titles_response.py
+-rw-r--r--   0 hemanthkumar  (1001) hemanthkumar  (1001)     2965 2023-11-27 10:42:27.000000 phenomApis-0.0.9/phenom/api/search/models/job_titles_response_data.py
+-rw-r--r--   0 hemanthkumar  (1001) hemanthkumar  (1001)     4336 2023-11-27 10:42:27.000000 phenomApis-0.0.9/phenom/api/search/models/job_titles_response_data_titles.py
+-rw-r--r--   0 hemanthkumar  (1001) hemanthkumar  (1001)     4813 2023-11-27 10:42:27.000000 phenomApis-0.0.9/phenom/api/search/models/location_data.py
+-rw-r--r--   0 hemanthkumar  (1001) hemanthkumar  (1001)    10160 2023-11-27 10:42:27.000000 phenomApis-0.0.9/phenom/api/search/models/refine_search_request.py
+-rw-r--r--   0 hemanthkumar  (1001) hemanthkumar  (1001)     4986 2023-11-27 10:42:27.000000 phenomApis-0.0.9/phenom/api/search/models/refine_search_request_facets.py
+-rw-r--r--   0 hemanthkumar  (1001) hemanthkumar  (1001)     3539 2023-11-27 10:42:27.000000 phenomApis-0.0.9/phenom/api/search/models/refine_search_response.py
+-rw-r--r--   0 hemanthkumar  (1001) hemanthkumar  (1001)     2889 2023-11-27 10:42:27.000000 phenomApis-0.0.9/phenom/api/search/models/refine_search_response_data.py
+drwxr-xr-x   0 hemanthkumar  (1001) hemanthkumar  (1001)        0 2023-11-27 10:49:40.611925 phenomApis-0.0.9/phenom/commons/
+-rw-r--r--   0 hemanthkumar  (1001) hemanthkumar  (1001)        0 2023-10-25 06:34:37.000000 phenomApis-0.0.9/phenom/commons/__init__.py
+-rw-r--r--   0 hemanthkumar  (1001) hemanthkumar  (1001)    23936 2023-11-24 06:50:15.000000 phenomApis-0.0.9/phenom/commons/api_client.py
+-rw-r--r--   0 hemanthkumar  (1001) hemanthkumar  (1001)     1793 2023-11-27 10:40:36.000000 phenomApis-0.0.9/phenom/commons/authorization.py
+-rw-r--r--   0 hemanthkumar  (1001) hemanthkumar  (1001)     7574 2023-11-24 06:05:16.000000 phenomApis-0.0.9/phenom/commons/configuration.py
+-rw-r--r--   0 hemanthkumar  (1001) hemanthkumar  (1001)     1473 2023-10-20 07:05:34.000000 phenomApis-0.0.9/phenom/commons/get_token.py
+-rw-r--r--   0 hemanthkumar  (1001) hemanthkumar  (1001)    12769 2023-11-08 11:23:40.000000 phenomApis-0.0.9/phenom/commons/rest.py
+drwxr-xr-x   0 hemanthkumar  (1001) hemanthkumar  (1001)        0 2023-11-27 10:49:40.611925 phenomApis-0.0.9/phenomApis.egg-info/
+-rw-r--r--   0 hemanthkumar  (1001) hemanthkumar  (1001)      650 2023-11-27 10:49:40.000000 phenomApis-0.0.9/phenomApis.egg-info/PKG-INFO
+-rw-r--r--   0 hemanthkumar  (1001) hemanthkumar  (1001)     5866 2023-11-27 10:49:40.000000 phenomApis-0.0.9/phenomApis.egg-info/SOURCES.txt
+-rw-r--r--   0 hemanthkumar  (1001) hemanthkumar  (1001)        1 2023-11-27 10:49:40.000000 phenomApis-0.0.9/phenomApis.egg-info/dependency_links.txt
+-rw-r--r--   0 hemanthkumar  (1001) hemanthkumar  (1001)       60 2023-11-27 10:49:40.000000 phenomApis-0.0.9/phenomApis.egg-info/requires.txt
+-rw-r--r--   0 hemanthkumar  (1001) hemanthkumar  (1001)        7 2023-11-27 10:49:40.000000 phenomApis-0.0.9/phenomApis.egg-info/top_level.txt
+-rw-r--r--   0 hemanthkumar  (1001) hemanthkumar  (1001)       38 2023-11-27 10:49:40.615926 phenomApis-0.0.9/setup.cfg
+-rw-r--r--   0 hemanthkumar  (1001) hemanthkumar  (1001)      879 2023-11-27 10:49:37.000000 phenomApis-0.0.9/setup.py
```

### Comparing `phenomApis-0.0.8/LICENSE` & `phenomApis-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `phenomApis-0.0.8/PKG-INFO` & `phenomApis-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phenomApis
-Version: 0.0.8
+Version: 0.0.9
 Summary: phenomApis
 Author: phenom
 Author-email: 8297991468h@gmail.com
 Keywords: resumeparser,exsearch
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `phenomApis-0.0.8/phenom/api/aisourcing/__init__.py` & `phenomApis-0.0.9/phenom/api/aisourcing/models/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,27 +1,21 @@
 # coding: utf-8
 
 # flake8: noqa
-
 """
     aisourcing-api
 
     AI Matching apis   # noqa: E501
 
-    OpenAPI spec version: 1.0.0
     
-    Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
-# import apis into sdk package
-from phenom.api.aisourcing.ai_matching_api import AIMatchingApi
-# import ApiClient
-# import models into sdk package
+# import models into model package
 from phenom.api.aisourcing.models.error_response import ErrorResponse
 from phenom.api.aisourcing.models.fit_score_request import FitScoreRequest
 from phenom.api.aisourcing.models.fitscore_bad_request import FitscoreBadRequest
 from phenom.api.aisourcing.models.fitscore_response import FitscoreResponse
 from phenom.api.aisourcing.models.fitscore_response_result import FitscoreResponseResult
 from phenom.api.aisourcing.models.fitscore_response_skill_gap import FitscoreResponseSkillGap
 from phenom.api.aisourcing.models.preferred_locations import PreferredLocations
```

### Comparing `phenomApis-0.0.8/phenom/api/aisourcing/ai_matching_api.py` & `phenomApis-0.0.9/phenom/api/aisourcing/ai_matching_api.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,35 +1,28 @@
 # coding: utf-8
 
 """
     aisourcing-api
 
     AI Matching apis   # noqa: E501
 
-    OpenAPI spec version: 1.0.0
     
-    Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import re  # noqa: F401
 
 # python 2 and python 3 compatibility library
 import six
 
 from phenom.commons.api_client import ApiClient
 
 
 class AIMatchingApi(object):
-    """NOTE: This class is auto generated by the swagger code generator program.
-
-    Do not edit the class manually.
-    Ref: https://github.com/swagger-api/swagger-codegen
-    """
 
     base_path = "/aisourcing"
 
     def __init__(self, token, gateway_url, apikey, api_client=None):
         if api_client is None:
             api_client = ApiClient(gateway_url + self.base_path, apikey, token)
         self.api_client = api_client
```

### Comparing `phenomApis-0.0.8/phenom/api/aisourcing/models/__init__.py` & `phenomApis-0.0.9/phenom/api/aisourcing/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 # coding: utf-8
 
 # flake8: noqa
+
 """
     aisourcing-api
 
     AI Matching apis   # noqa: E501
 
-    OpenAPI spec version: 1.0.0
     
-    Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
-# import models into model package
+# import apis into sdk package
+from phenom.api.aisourcing.ai_matching_api import AIMatchingApi
+# import ApiClient
+# import models into sdk package
 from phenom.api.aisourcing.models.error_response import ErrorResponse
 from phenom.api.aisourcing.models.fit_score_request import FitScoreRequest
 from phenom.api.aisourcing.models.fitscore_bad_request import FitscoreBadRequest
 from phenom.api.aisourcing.models.fitscore_response import FitscoreResponse
 from phenom.api.aisourcing.models.fitscore_response_result import FitscoreResponseResult
 from phenom.api.aisourcing.models.fitscore_response_skill_gap import FitscoreResponseSkillGap
 from phenom.api.aisourcing.models.preferred_locations import PreferredLocations
```

### Comparing `phenomApis-0.0.8/phenom/api/aisourcing/models/error_response.py` & `phenomApis-0.0.9/phenom/api/aisourcing/models/error_response.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,29 +1,23 @@
 # coding: utf-8
 
 """
     aisourcing-api
 
     AI Matching apis   # noqa: E501
 
-    OpenAPI spec version: 1.0.0
     
-    Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 class ErrorResponse(object):
-    """NOTE: This class is auto generated by the swagger code generator program.
-
-    Do not edit the class manually.
-    """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
```

### Comparing `phenomApis-0.0.8/phenom/api/aisourcing/models/fit_score_request.py` & `phenomApis-0.0.9/phenom/api/aisourcing/models/fit_score_request.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,23 @@
 # coding: utf-8
 
 """
     aisourcing-api
 
     AI Matching apis   # noqa: E501
 
-    OpenAPI spec version: 1.0.0
     
-    Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 class FitScoreRequest(object):
-    """NOTE: This class is auto generated by the swagger code generator program.
-
-    Do not edit the class manually.
-    """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
```

### Comparing `phenomApis-0.0.8/phenom/api/aisourcing/models/fitscore_bad_request.py` & `phenomApis-0.0.9/phenom/api/exsearch/models/facets_node.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,97 +1,117 @@
 # coding: utf-8
 
 """
-    aisourcing-api
+    ex-search-api
 
-    AI Matching apis   # noqa: E501
+    These APIs helps to search and suggest based on keyword among employee profiles  # noqa: E501
 
-    OpenAPI spec version: 1.0.0
     
-    Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class FitscoreBadRequest(object):
-    """NOTE: This class is auto generated by the swagger code generator program.
-
-    Do not edit the class manually.
-    """
+class FacetsNode(object):
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
-        'status': 'str',
-        'message': 'str'
+        'field': 'str',
+        'key': 'str',
+        'value': 'object'
     }
 
     attribute_map = {
-        'status': 'status',
-        'message': 'message'
+        'field': 'field',
+        'key': 'key',
+        'value': 'value'
     }
 
-    def __init__(self, status=None, message=None):  # noqa: E501
-        """FitscoreBadRequest - a model defined in Swagger"""  # noqa: E501
-        self._status = None
-        self._message = None
+    def __init__(self, field=None, key=None, value=None):  # noqa: E501
+        """FacetsNode - a model defined in Swagger"""  # noqa: E501
+        self._field = None
+        self._key = None
+        self._value = None
         self.discriminator = None
-        if status is not None:
-            self.status = status
-        if message is not None:
-            self.message = message
+        if field is not None:
+            self.field = field
+        if key is not None:
+            self.key = key
+        if value is not None:
+            self.value = value
 
     @property
-    def status(self):
-        """Gets the status of this FitscoreBadRequest.  # noqa: E501
+    def field(self):
+        """Gets the field of this FacetsNode.  # noqa: E501
 
 
-        :return: The status of this FitscoreBadRequest.  # noqa: E501
+        :return: The field of this FacetsNode.  # noqa: E501
         :rtype: str
         """
-        return self._status
+        return self._field
 
-    @status.setter
-    def status(self, status):
-        """Sets the status of this FitscoreBadRequest.
+    @field.setter
+    def field(self, field):
+        """Sets the field of this FacetsNode.
 
 
-        :param status: The status of this FitscoreBadRequest.  # noqa: E501
+        :param field: The field of this FacetsNode.  # noqa: E501
         :type: str
         """
 
-        self._status = status
+        self._field = field
 
     @property
-    def message(self):
-        """Gets the message of this FitscoreBadRequest.  # noqa: E501
+    def key(self):
+        """Gets the key of this FacetsNode.  # noqa: E501
 
 
-        :return: The message of this FitscoreBadRequest.  # noqa: E501
+        :return: The key of this FacetsNode.  # noqa: E501
         :rtype: str
         """
-        return self._message
+        return self._key
 
-    @message.setter
-    def message(self, message):
-        """Sets the message of this FitscoreBadRequest.
+    @key.setter
+    def key(self, key):
+        """Sets the key of this FacetsNode.
 
 
-        :param message: The message of this FitscoreBadRequest.  # noqa: E501
+        :param key: The key of this FacetsNode.  # noqa: E501
         :type: str
         """
 
-        self._message = message
+        self._key = key
+
+    @property
+    def value(self):
+        """Gets the value of this FacetsNode.  # noqa: E501
+
+
+        :return: The value of this FacetsNode.  # noqa: E501
+        :rtype: object
+        """
+        return self._value
+
+    @value.setter
+    def value(self, value):
+        """Sets the value of this FacetsNode.
+
+
+        :param value: The value of this FacetsNode.  # noqa: E501
+        :type: object
+        """
+
+        self._value = value
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
             value = getattr(self, attr)
@@ -106,15 +126,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(FitscoreBadRequest, dict):
+        if issubclass(FacetsNode, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -122,15 +142,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, FitscoreBadRequest):
+        if not isinstance(other, FacetsNode):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `phenomApis-0.0.8/phenom/api/aisourcing/models/fitscore_response.py` & `phenomApis-0.0.9/phenom/api/aisourcing/models/fitscore_response.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,29 +1,23 @@
 # coding: utf-8
 
 """
     aisourcing-api
 
     AI Matching apis   # noqa: E501
 
-    OpenAPI spec version: 1.0.0
     
-    Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 class FitscoreResponse(object):
-    """NOTE: This class is auto generated by the swagger code generator program.
-
-    Do not edit the class manually.
-    """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
```

### Comparing `phenomApis-0.0.8/phenom/api/aisourcing/models/fitscore_response_result.py` & `phenomApis-0.0.9/phenom/api/aisourcing/models/fitscore_response_result.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,29 +1,23 @@
 # coding: utf-8
 
 """
     aisourcing-api
 
     AI Matching apis   # noqa: E501
 
-    OpenAPI spec version: 1.0.0
     
-    Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 class FitscoreResponseResult(object):
-    """NOTE: This class is auto generated by the swagger code generator program.
-
-    Do not edit the class manually.
-    """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
```

### Comparing `phenomApis-0.0.8/phenom/api/aisourcing/models/fitscore_response_skill_gap.py` & `phenomApis-0.0.9/phenom/api/aisourcing/models/fitscore_response_skill_gap.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,23 @@
 # coding: utf-8
 
 """
     aisourcing-api
 
     AI Matching apis   # noqa: E501
 
-    OpenAPI spec version: 1.0.0
     
-    Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 class FitscoreResponseSkillGap(object):
-    """NOTE: This class is auto generated by the swagger code generator program.
-
-    Do not edit the class manually.
-    """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
```

### Comparing `phenomApis-0.0.8/phenom/api/aisourcing/models/preferred_locations.py` & `phenomApis-0.0.9/phenom/api/aisourcing/models/preferred_locations.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,23 @@
 # coding: utf-8
 
 """
     aisourcing-api
 
     AI Matching apis   # noqa: E501
 
-    OpenAPI spec version: 1.0.0
     
-    Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 class PreferredLocations(object):
-    """NOTE: This class is auto generated by the swagger code generator program.
-
-    Do not edit the class manually.
-    """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
```

### Comparing `phenomApis-0.0.8/phenom/api/aisourcing/models/preferred_locations_latlong.py` & `phenomApis-0.0.9/phenom/api/aisourcing/models/preferred_locations_latlong.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,29 +1,23 @@
 # coding: utf-8
 
 """
     aisourcing-api
 
     AI Matching apis   # noqa: E501
 
-    OpenAPI spec version: 1.0.0
     
-    Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 class PreferredLocationsLatlong(object):
-    """NOTE: This class is auto generated by the swagger code generator program.
-
-    Do not edit the class manually.
-    """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
```

### Comparing `phenomApis-0.0.8/phenom/api/aisourcing/models/skill_matching_bad_request.py` & `phenomApis-0.0.9/phenom/api/aisourcing/models/skill_matching_bad_request.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,29 +1,23 @@
 # coding: utf-8
 
 """
     aisourcing-api
 
     AI Matching apis   # noqa: E501
 
-    OpenAPI spec version: 1.0.0
     
-    Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 class SkillMatchingBadRequest(object):
-    """NOTE: This class is auto generated by the swagger code generator program.
-
-    Do not edit the class manually.
-    """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
```

### Comparing `phenomApis-0.0.8/phenom/api/aisourcing/models/skill_matching_error_response.py` & `phenomApis-0.0.9/phenom/api/aisourcing/models/skill_matching_error_response.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,29 +1,23 @@
 # coding: utf-8
 
 """
     aisourcing-api
 
     AI Matching apis   # noqa: E501
 
-    OpenAPI spec version: 1.0.0
     
-    Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 class SkillMatchingErrorResponse(object):
-    """NOTE: This class is auto generated by the swagger code generator program.
-
-    Do not edit the class manually.
-    """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
```

### Comparing `phenomApis-0.0.8/phenom/api/aisourcing/models/skill_matching_response.py` & `phenomApis-0.0.9/phenom/api/aisourcing/models/skill_matching_response.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,29 +1,23 @@
 # coding: utf-8
 
 """
     aisourcing-api
 
     AI Matching apis   # noqa: E501
 
-    OpenAPI spec version: 1.0.0
     
-    Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 class SkillMatchingResponse(object):
-    """NOTE: This class is auto generated by the swagger code generator program.
-
-    Do not edit the class manually.
-    """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
```

### Comparing `phenomApis-0.0.8/phenom/api/aisourcing/models/user_profile_fit_score.py` & `phenomApis-0.0.9/phenom/api/aisourcing/models/user_profile_fit_score.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,29 +1,23 @@
 # coding: utf-8
 
 """
     aisourcing-api
 
     AI Matching apis   # noqa: E501
 
-    OpenAPI spec version: 1.0.0
     
-    Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 class UserProfileFitScore(object):
-    """NOTE: This class is auto generated by the swagger code generator program.
-
-    Do not edit the class manually.
-    """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
```

### Comparing `phenomApis-0.0.8/phenom/api/exsearch/__init__.py` & `phenomApis-0.0.9/phenom/api/exsearch/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,17 +3,15 @@
 # flake8: noqa
 
 """
     ex-search-api
 
     These APIs helps to search and suggest based on keyword among employee profiles  # noqa: E501
 
-    OpenAPI spec version: 1.0.0
     
-    Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 # import apis into sdk package
 from phenom.api.exsearch.employees_api import EmployeesApi
 from phenom.api.exsearch.mentor_api import MentorApi
```

### Comparing `phenomApis-0.0.8/phenom/api/exsearch/employees_api.py` & `phenomApis-0.0.9/phenom/api/exsearch/employees_api.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,35 +1,28 @@
 # coding: utf-8
 
 """
     ex-search-api
 
     These APIs helps to search and suggest based on keyword among employee profiles  # noqa: E501
 
-    OpenAPI spec version: 1.0.0
     
-    Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import re  # noqa: F401
 
 # python 2 and python 3 compatibility library
 import six
 
 from phenom.commons.api_client import ApiClient
 
 
 class EmployeesApi(object):
-    """NOTE: This class is auto generated by the swagger code generator program.
-
-    Do not edit the class manually.
-    Ref: https://github.com/swagger-api/swagger-codegen
-    """
 
     base_path = "/employees-api/v1/employees/search"  # your base path
 
     def __init__(self, token, gateway_url, apikey, api_client=None):
         if api_client is None:
             api_client = ApiClient(gateway_url + self.base_path, apikey, token)
         self.api_client = api_client
```

### Comparing `phenomApis-0.0.8/phenom/api/exsearch/mentor_api.py` & `phenomApis-0.0.9/phenom/api/jobparser/job_parsing_api.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,73 +1,68 @@
 # coding: utf-8
 
 """
-    ex-search-api
+    job-parser-api
 
-    These APIs helps to search and suggest based on keyword among employee profiles  # noqa: E501
+    The process of extracting important information from the raw job description is called Job Parsing. This information can include things like job titles, required skills, required experience, job duties, and qualifications.  # noqa: E501
 
-    OpenAPI spec version: 1.0.0
     
-    Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import re  # noqa: F401
 
 # python 2 and python 3 compatibility library
 import six
 
 from phenom.commons.api_client import ApiClient
 
 
-class MentorApi(object):
-    """NOTE: This class is auto generated by the swagger code generator program.
+class JobParsingApi(object):
 
-    Do not edit the class manually.
-    Ref: https://github.com/swagger-api/swagger-codegen
-    """
+    base_path = "/parser/job"
 
-    def __init__(self, api_client=None):
+    def __init__(self, token, gateway_url, apikey, api_client=None):
         if api_client is None:
-            api_client = ApiClient()
+            api_client = ApiClient(gateway_url + self.base_path, apikey, token)
         self.api_client = api_client
 
-    def suggest_mentors(self, body, **kwargs):  # noqa: E501
-        """Mentor TypeAhead Suggestions  # noqa: E501
+    def parse_job(self, body, **kwargs):  # noqa: E501
+        """Job Parsing  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.suggest_mentors(body, async_req=True)
+        >>> thread = api.parse_job(body, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
-        :param MentorTypeAheadRequest body: (required)
-        :return: MentorTypeaheadResponse
+        :param JDRequest body: (required)
+        :return: JobResponse
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
         if kwargs.get('async_req'):
-            return self.suggest_mentors_with_http_info(body, **kwargs)  # noqa: E501
+            return self.parse_job_with_http_info(body, **kwargs)  # noqa: E501
         else:
-            (data) = self.suggest_mentors_with_http_info(body, **kwargs)  # noqa: E501
+            (data) = self.parse_job_with_http_info(body, **kwargs)  # noqa: E501
             return data
 
-    def suggest_mentors_with_http_info(self, body, **kwargs):  # noqa: E501
-        """Mentor TypeAhead Suggestions  # noqa: E501
+    def parse_job_with_http_info(self, body, **kwargs):  # noqa: E501
+        """Job Parsing  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.suggest_mentors_with_http_info(body, async_req=True)
+        >>> thread = api.parse_job_with_http_info(body, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
-        :param MentorTypeAheadRequest body: (required)
-        :return: MentorTypeaheadResponse
+        :param JDRequest body: (required)
+        :return: JobResponse
                  If the method is called asynchronously,
                  returns the request thread.
         """
 
         all_params = ['body']  # noqa: E501
         all_params.append('async_req')
         all_params.append('_return_http_data_only')
@@ -75,22 +70,22 @@
         all_params.append('_request_timeout')
 
         params = locals()
         for key, val in six.iteritems(params['kwargs']):
             if key not in all_params:
                 raise TypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method suggest_mentors" % key
+                    " to method parse_job" % key
                 )
             params[key] = val
         del params['kwargs']
         # verify the required parameter 'body' is set
         if ('body' not in params or
                 params['body'] is None):
-            raise ValueError("Missing the required parameter `body` when calling `suggest_mentors`")  # noqa: E501
+            raise ValueError("Missing the required parameter `body` when calling `parse_job`")  # noqa: E501
 
         collection_formats = {}
 
         path_params = {}
 
         query_params = []
 
@@ -110,21 +105,21 @@
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json'])  # noqa: E501
 
         # Authentication setting
         auth_settings = []  # noqa: E501
 
         return self.api_client.call_api(
-            '/suggestions/mentor', 'POST',
+            '/v1/parse', 'POST',
             path_params,
             query_params,
             header_params,
             body=body_params,
             post_params=form_params,
             files=local_var_files,
-            response_type='MentorTypeaheadResponse',  # noqa: E501
+            response_type='JobResponse',  # noqa: E501
             auth_settings=auth_settings,
             async_req=params.get('async_req'),
             _return_http_data_only=params.get('_return_http_data_only'),
             _preload_content=params.get('_preload_content', True),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
```

### Comparing `phenomApis-0.0.8/phenom/api/exsearch/models/__init__.py` & `phenomApis-0.0.9/phenom/api/exsearch/models/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,17 +2,15 @@
 
 # flake8: noqa
 """
     ex-search-api
 
     These APIs helps to search and suggest based on keyword among employee profiles  # noqa: E501
 
-    OpenAPI spec version: 1.0.0
     
-    Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 # import models into model package
 from phenom.api.exsearch.models.aggregations_node import AggregationsNode
 from phenom.api.exsearch.models.bad_request import BadRequest
```

### Comparing `phenomApis-0.0.8/phenom/api/exsearch/models/aggregations_node.py` & `phenomApis-0.0.9/phenom/api/exsearch/models/aggregations_node.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,29 +1,23 @@
 # coding: utf-8
 
 """
     ex-search-api
 
     These APIs helps to search and suggest based on keyword among employee profiles  # noqa: E501
 
-    OpenAPI spec version: 1.0.0
     
-    Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 class AggregationsNode(object):
-    """NOTE: This class is auto generated by the swagger code generator program.
-
-    Do not edit the class manually.
-    """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
```

### Comparing `phenomApis-0.0.8/phenom/api/exsearch/models/bad_request.py` & `phenomApis-0.0.9/phenom/api/exsearch/models/bad_request.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,29 +1,23 @@
 # coding: utf-8
 
 """
     ex-search-api
 
     These APIs helps to search and suggest based on keyword among employee profiles  # noqa: E501
 
-    OpenAPI spec version: 1.0.0
     
-    Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 class BadRequest(object):
-    """NOTE: This class is auto generated by the swagger code generator program.
-
-    Do not edit the class manually.
-    """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
```

### Comparing `phenomApis-0.0.8/phenom/api/exsearch/models/common_node.py` & `phenomApis-0.0.9/phenom/api/exsearch/models/common_node.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,29 +1,23 @@
 # coding: utf-8
 
 """
     ex-search-api
 
     These APIs helps to search and suggest based on keyword among employee profiles  # noqa: E501
 
-    OpenAPI spec version: 1.0.0
     
-    Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 class CommonNode(object):
-    """NOTE: This class is auto generated by the swagger code generator program.
-
-    Do not edit the class manually.
-    """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
```

### Comparing `phenomApis-0.0.8/phenom/api/exsearch/models/employee_node.py` & `phenomApis-0.0.9/phenom/api/exsearch/models/employee_node.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,23 @@
 # coding: utf-8
 
 """
     ex-search-api
 
     These APIs helps to search and suggest based on keyword among employee profiles  # noqa: E501
 
-    OpenAPI spec version: 1.0.0
     
-    Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 class EmployeeNode(object):
-    """NOTE: This class is auto generated by the swagger code generator program.
-
-    Do not edit the class manually.
-    """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
```

### Comparing `phenomApis-0.0.8/phenom/api/exsearch/models/employee_search_request.py` & `phenomApis-0.0.9/phenom/api/exsearch/models/employee_search_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,23 @@
 # coding: utf-8
 
 """
     ex-search-api
 
     These APIs helps to search and suggest based on keyword among employee profiles  # noqa: E501
 
-    OpenAPI spec version: 1.0.0
     
-    Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 class EmployeeSearchRequest(object):
-    """NOTE: This class is auto generated by the swagger code generator program.
-
-    Do not edit the class manually.
-    """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
```

### Comparing `phenomApis-0.0.8/phenom/api/exsearch/models/employee_search_response.py` & `phenomApis-0.0.9/phenom/api/exsearch/models/employee_search_response.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,29 +1,23 @@
 # coding: utf-8
 
 """
     ex-search-api
 
     These APIs helps to search and suggest based on keyword among employee profiles  # noqa: E501
 
-    OpenAPI spec version: 1.0.0
     
-    Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 class EmployeeSearchResponse(object):
-    """NOTE: This class is auto generated by the swagger code generator program.
-
-    Do not edit the class manually.
-    """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
```

### Comparing `phenomApis-0.0.8/phenom/api/exsearch/models/employee_search_response_data.py` & `phenomApis-0.0.9/phenom/api/exsearch/models/employee_search_response_data.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,29 +1,23 @@
 # coding: utf-8
 
 """
     ex-search-api
 
     These APIs helps to search and suggest based on keyword among employee profiles  # noqa: E501
 
-    OpenAPI spec version: 1.0.0
     
-    Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 class EmployeeSearchResponseData(object):
-    """NOTE: This class is auto generated by the swagger code generator program.
-
-    Do not edit the class manually.
-    """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
```

### Comparing `phenomApis-0.0.8/phenom/api/exsearch/models/employee_type_ahead_agg_request.py` & `phenomApis-0.0.9/phenom/api/exsearch/models/employee_type_ahead_agg_request.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,29 +1,23 @@
 # coding: utf-8
 
 """
     ex-search-api
 
     These APIs helps to search and suggest based on keyword among employee profiles  # noqa: E501
 
-    OpenAPI spec version: 1.0.0
     
-    Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 class EmployeeTypeAheadAggRequest(object):
-    """NOTE: This class is auto generated by the swagger code generator program.
-
-    Do not edit the class manually.
-    """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
```

### Comparing `phenomApis-0.0.8/phenom/api/exsearch/models/employee_type_ahead_request.py` & `phenomApis-0.0.9/phenom/api/exsearch/models/employee_type_ahead_request.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,29 +1,23 @@
 # coding: utf-8
 
 """
     ex-search-api
 
     These APIs helps to search and suggest based on keyword among employee profiles  # noqa: E501
 
-    OpenAPI spec version: 1.0.0
     
-    Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 class EmployeeTypeAheadRequest(object):
-    """NOTE: This class is auto generated by the swagger code generator program.
-
-    Do not edit the class manually.
-    """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
```

### Comparing `phenomApis-0.0.8/phenom/api/exsearch/models/employee_typeahead_agg_response.py` & `phenomApis-0.0.9/phenom/api/exsearch/models/employee_typeahead_agg_response.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,29 +1,23 @@
 # coding: utf-8
 
 """
     ex-search-api
 
     These APIs helps to search and suggest based on keyword among employee profiles  # noqa: E501
 
-    OpenAPI spec version: 1.0.0
     
-    Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 class EmployeeTypeaheadAggResponse(object):
-    """NOTE: This class is auto generated by the swagger code generator program.
-
-    Do not edit the class manually.
-    """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
```

### Comparing `phenomApis-0.0.8/phenom/api/exsearch/models/employee_typeahead_response.py` & `phenomApis-0.0.9/phenom/api/exsearch/models/error_response.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,52 +1,46 @@
 # coding: utf-8
 
 """
     ex-search-api
 
     These APIs helps to search and suggest based on keyword among employee profiles  # noqa: E501
 
-    OpenAPI spec version: 1.0.0
     
-    Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class EmployeeTypeaheadResponse(object):
-    """NOTE: This class is auto generated by the swagger code generator program.
-
-    Do not edit the class manually.
-    """
+class ErrorResponse(object):
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
         'status': 'int',
         'hits': 'int',
         'total_hits': 'int',
-        'data': 'EmployeeTypeaheadResponseData'
+        'data': 'object'
     }
 
     attribute_map = {
         'status': 'status',
         'hits': 'hits',
         'total_hits': 'totalHits',
         'data': 'data'
     }
 
     def __init__(self, status=None, hits=None, total_hits=None, data=None):  # noqa: E501
-        """EmployeeTypeaheadResponse - a model defined in Swagger"""  # noqa: E501
+        """ErrorResponse - a model defined in Swagger"""  # noqa: E501
         self._status = None
         self._hits = None
         self._total_hits = None
         self._data = None
         self.discriminator = None
         if status is not None:
             self.status = status
@@ -55,92 +49,92 @@
         if total_hits is not None:
             self.total_hits = total_hits
         if data is not None:
             self.data = data
 
     @property
     def status(self):
-        """Gets the status of this EmployeeTypeaheadResponse.  # noqa: E501
+        """Gets the status of this ErrorResponse.  # noqa: E501
 
 
-        :return: The status of this EmployeeTypeaheadResponse.  # noqa: E501
+        :return: The status of this ErrorResponse.  # noqa: E501
         :rtype: int
         """
         return self._status
 
     @status.setter
     def status(self, status):
-        """Sets the status of this EmployeeTypeaheadResponse.
+        """Sets the status of this ErrorResponse.
 
 
-        :param status: The status of this EmployeeTypeaheadResponse.  # noqa: E501
+        :param status: The status of this ErrorResponse.  # noqa: E501
         :type: int
         """
 
         self._status = status
 
     @property
     def hits(self):
-        """Gets the hits of this EmployeeTypeaheadResponse.  # noqa: E501
+        """Gets the hits of this ErrorResponse.  # noqa: E501
 
 
-        :return: The hits of this EmployeeTypeaheadResponse.  # noqa: E501
+        :return: The hits of this ErrorResponse.  # noqa: E501
         :rtype: int
         """
         return self._hits
 
     @hits.setter
     def hits(self, hits):
-        """Sets the hits of this EmployeeTypeaheadResponse.
+        """Sets the hits of this ErrorResponse.
 
 
-        :param hits: The hits of this EmployeeTypeaheadResponse.  # noqa: E501
+        :param hits: The hits of this ErrorResponse.  # noqa: E501
         :type: int
         """
 
         self._hits = hits
 
     @property
     def total_hits(self):
-        """Gets the total_hits of this EmployeeTypeaheadResponse.  # noqa: E501
+        """Gets the total_hits of this ErrorResponse.  # noqa: E501
 
 
-        :return: The total_hits of this EmployeeTypeaheadResponse.  # noqa: E501
+        :return: The total_hits of this ErrorResponse.  # noqa: E501
         :rtype: int
         """
         return self._total_hits
 
     @total_hits.setter
     def total_hits(self, total_hits):
-        """Sets the total_hits of this EmployeeTypeaheadResponse.
+        """Sets the total_hits of this ErrorResponse.
 
 
-        :param total_hits: The total_hits of this EmployeeTypeaheadResponse.  # noqa: E501
+        :param total_hits: The total_hits of this ErrorResponse.  # noqa: E501
         :type: int
         """
 
         self._total_hits = total_hits
 
     @property
     def data(self):
-        """Gets the data of this EmployeeTypeaheadResponse.  # noqa: E501
+        """Gets the data of this ErrorResponse.  # noqa: E501
 
 
-        :return: The data of this EmployeeTypeaheadResponse.  # noqa: E501
-        :rtype: EmployeeTypeaheadResponseData
+        :return: The data of this ErrorResponse.  # noqa: E501
+        :rtype: object
         """
         return self._data
 
     @data.setter
     def data(self, data):
-        """Sets the data of this EmployeeTypeaheadResponse.
+        """Sets the data of this ErrorResponse.
 
 
-        :param data: The data of this EmployeeTypeaheadResponse.  # noqa: E501
-        :type: EmployeeTypeaheadResponseData
+        :param data: The data of this ErrorResponse.  # noqa: E501
+        :type: object
         """
 
         self._data = data
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
@@ -158,15 +152,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(EmployeeTypeaheadResponse, dict):
+        if issubclass(ErrorResponse, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -174,15 +168,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, EmployeeTypeaheadResponse):
+        if not isinstance(other, ErrorResponse):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `phenomApis-0.0.8/phenom/api/exsearch/models/employee_typeahead_response_data.py` & `phenomApis-0.0.9/phenom/api/search/models/refine_search_response_data.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,71 +1,65 @@
 # coding: utf-8
 
 """
-    ex-search-api
+    search-api
 
-    These APIs helps to search and suggest based on keyword among employee profiles  # noqa: E501
+    These APIs helps to search and suggest based on keyword among available jobs  # noqa: E501
 
-    OpenAPI spec version: 1.0.0
     
-    Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class EmployeeTypeaheadResponseData(object):
-    """NOTE: This class is auto generated by the swagger code generator program.
-
-    Do not edit the class manually.
-    """
+class RefineSearchResponseData(object):
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
-        'employees': 'list[EmployeeNode]'
+        'jobs': 'list[JobNode]'
     }
 
     attribute_map = {
-        'employees': 'employees'
+        'jobs': 'jobs'
     }
 
-    def __init__(self, employees=None):  # noqa: E501
-        """EmployeeTypeaheadResponseData - a model defined in Swagger"""  # noqa: E501
-        self._employees = None
+    def __init__(self, jobs=None):  # noqa: E501
+        """RefineSearchResponseData - a model defined in Swagger"""  # noqa: E501
+        self._jobs = None
         self.discriminator = None
-        if employees is not None:
-            self.employees = employees
+        if jobs is not None:
+            self.jobs = jobs
 
     @property
-    def employees(self):
-        """Gets the employees of this EmployeeTypeaheadResponseData.  # noqa: E501
+    def jobs(self):
+        """Gets the jobs of this RefineSearchResponseData.  # noqa: E501
 
 
-        :return: The employees of this EmployeeTypeaheadResponseData.  # noqa: E501
-        :rtype: list[EmployeeNode]
+        :return: The jobs of this RefineSearchResponseData.  # noqa: E501
+        :rtype: list[JobNode]
         """
-        return self._employees
+        return self._jobs
 
-    @employees.setter
-    def employees(self, employees):
-        """Sets the employees of this EmployeeTypeaheadResponseData.
+    @jobs.setter
+    def jobs(self, jobs):
+        """Sets the jobs of this RefineSearchResponseData.
 
 
-        :param employees: The employees of this EmployeeTypeaheadResponseData.  # noqa: E501
-        :type: list[EmployeeNode]
+        :param jobs: The jobs of this RefineSearchResponseData.  # noqa: E501
+        :type: list[JobNode]
         """
 
-        self._employees = employees
+        self._jobs = jobs
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
             value = getattr(self, attr)
@@ -80,15 +74,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(EmployeeTypeaheadResponseData, dict):
+        if issubclass(RefineSearchResponseData, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -96,15 +90,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, EmployeeTypeaheadResponseData):
+        if not isinstance(other, RefineSearchResponseData):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `phenomApis-0.0.8/phenom/api/exsearch/models/error_response.py` & `phenomApis-0.0.9/phenom/api/prediction/models/fyf_skill_response.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,150 +1,145 @@
 # coding: utf-8
 
 """
-    ex-search-api
+    prediction-api
 
-    These APIs helps to search and suggest based on keyword among employee profiles  # noqa: E501
+    Prediction api   # noqa: E501
 
-    OpenAPI spec version: 1.0.0
     
-    Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class ErrorResponse(object):
-    """NOTE: This class is auto generated by the swagger code generator program.
-
-    Do not edit the class manually.
-    """
+class FYFSkillResponse(object):
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
-        'status': 'int',
-        'hits': 'int',
+        'status': 'str',
         'total_hits': 'int',
-        'data': 'object'
+        'data': 'SkillResults',
+        'message': 'str'
     }
 
     attribute_map = {
         'status': 'status',
-        'hits': 'hits',
         'total_hits': 'totalHits',
-        'data': 'data'
+        'data': 'data',
+        'message': 'message'
     }
 
-    def __init__(self, status=None, hits=None, total_hits=None, data=None):  # noqa: E501
-        """ErrorResponse - a model defined in Swagger"""  # noqa: E501
+    def __init__(self, status=None, total_hits=None, data=None, message=None):  # noqa: E501
+        """FYFSkillResponse - a model defined in Swagger"""  # noqa: E501
         self._status = None
-        self._hits = None
         self._total_hits = None
         self._data = None
+        self._message = None
         self.discriminator = None
-        if status is not None:
-            self.status = status
-        if hits is not None:
-            self.hits = hits
+        self.status = status
         if total_hits is not None:
             self.total_hits = total_hits
         if data is not None:
             self.data = data
+        if message is not None:
+            self.message = message
 
     @property
     def status(self):
-        """Gets the status of this ErrorResponse.  # noqa: E501
+        """Gets the status of this FYFSkillResponse.  # noqa: E501
 
 
-        :return: The status of this ErrorResponse.  # noqa: E501
-        :rtype: int
+        :return: The status of this FYFSkillResponse.  # noqa: E501
+        :rtype: str
         """
         return self._status
 
     @status.setter
     def status(self, status):
-        """Sets the status of this ErrorResponse.
+        """Sets the status of this FYFSkillResponse.
 
 
-        :param status: The status of this ErrorResponse.  # noqa: E501
-        :type: int
+        :param status: The status of this FYFSkillResponse.  # noqa: E501
+        :type: str
         """
+        if status is None:
+            raise ValueError("Invalid value for `status`, must not be `None`")  # noqa: E501
 
         self._status = status
 
     @property
-    def hits(self):
-        """Gets the hits of this ErrorResponse.  # noqa: E501
-
-
-        :return: The hits of this ErrorResponse.  # noqa: E501
-        :rtype: int
-        """
-        return self._hits
-
-    @hits.setter
-    def hits(self, hits):
-        """Sets the hits of this ErrorResponse.
-
-
-        :param hits: The hits of this ErrorResponse.  # noqa: E501
-        :type: int
-        """
-
-        self._hits = hits
-
-    @property
     def total_hits(self):
-        """Gets the total_hits of this ErrorResponse.  # noqa: E501
+        """Gets the total_hits of this FYFSkillResponse.  # noqa: E501
 
 
-        :return: The total_hits of this ErrorResponse.  # noqa: E501
+        :return: The total_hits of this FYFSkillResponse.  # noqa: E501
         :rtype: int
         """
         return self._total_hits
 
     @total_hits.setter
     def total_hits(self, total_hits):
-        """Sets the total_hits of this ErrorResponse.
+        """Sets the total_hits of this FYFSkillResponse.
 
 
-        :param total_hits: The total_hits of this ErrorResponse.  # noqa: E501
+        :param total_hits: The total_hits of this FYFSkillResponse.  # noqa: E501
         :type: int
         """
 
         self._total_hits = total_hits
 
     @property
     def data(self):
-        """Gets the data of this ErrorResponse.  # noqa: E501
+        """Gets the data of this FYFSkillResponse.  # noqa: E501
 
 
-        :return: The data of this ErrorResponse.  # noqa: E501
-        :rtype: object
+        :return: The data of this FYFSkillResponse.  # noqa: E501
+        :rtype: SkillResults
         """
         return self._data
 
     @data.setter
     def data(self, data):
-        """Sets the data of this ErrorResponse.
+        """Sets the data of this FYFSkillResponse.
 
 
-        :param data: The data of this ErrorResponse.  # noqa: E501
-        :type: object
+        :param data: The data of this FYFSkillResponse.  # noqa: E501
+        :type: SkillResults
         """
 
         self._data = data
 
+    @property
+    def message(self):
+        """Gets the message of this FYFSkillResponse.  # noqa: E501
+
+
+        :return: The message of this FYFSkillResponse.  # noqa: E501
+        :rtype: str
+        """
+        return self._message
+
+    @message.setter
+    def message(self, message):
+        """Sets the message of this FYFSkillResponse.
+
+
+        :param message: The message of this FYFSkillResponse.  # noqa: E501
+        :type: str
+        """
+
+        self._message = message
+
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
             value = getattr(self, attr)
             if isinstance(value, list):
@@ -158,15 +153,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(ErrorResponse, dict):
+        if issubclass(FYFSkillResponse, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -174,15 +169,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, ErrorResponse):
+        if not isinstance(other, FYFSkillResponse):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `phenomApis-0.0.8/phenom/api/exsearch/models/facets_node.py` & `phenomApis-0.0.9/phenom/api/exsearch/models/filters_node.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,120 +1,88 @@
 # coding: utf-8
 
 """
     ex-search-api
 
     These APIs helps to search and suggest based on keyword among employee profiles  # noqa: E501
 
-    OpenAPI spec version: 1.0.0
     
-    Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class FacetsNode(object):
-    """NOTE: This class is auto generated by the swagger code generator program.
-
-    Do not edit the class manually.
-    """
+class FiltersNode(object):
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
         'field': 'str',
-        'key': 'str',
-        'value': 'object'
+        'value': 'list[str]'
     }
 
     attribute_map = {
         'field': 'field',
-        'key': 'key',
         'value': 'value'
     }
 
-    def __init__(self, field=None, key=None, value=None):  # noqa: E501
-        """FacetsNode - a model defined in Swagger"""  # noqa: E501
+    def __init__(self, field=None, value=None):  # noqa: E501
+        """FiltersNode - a model defined in Swagger"""  # noqa: E501
         self._field = None
-        self._key = None
         self._value = None
         self.discriminator = None
         if field is not None:
             self.field = field
-        if key is not None:
-            self.key = key
         if value is not None:
             self.value = value
 
     @property
     def field(self):
-        """Gets the field of this FacetsNode.  # noqa: E501
+        """Gets the field of this FiltersNode.  # noqa: E501
 
 
-        :return: The field of this FacetsNode.  # noqa: E501
+        :return: The field of this FiltersNode.  # noqa: E501
         :rtype: str
         """
         return self._field
 
     @field.setter
     def field(self, field):
-        """Sets the field of this FacetsNode.
+        """Sets the field of this FiltersNode.
 
 
-        :param field: The field of this FacetsNode.  # noqa: E501
+        :param field: The field of this FiltersNode.  # noqa: E501
         :type: str
         """
 
         self._field = field
 
     @property
-    def key(self):
-        """Gets the key of this FacetsNode.  # noqa: E501
-
-
-        :return: The key of this FacetsNode.  # noqa: E501
-        :rtype: str
-        """
-        return self._key
-
-    @key.setter
-    def key(self, key):
-        """Sets the key of this FacetsNode.
-
-
-        :param key: The key of this FacetsNode.  # noqa: E501
-        :type: str
-        """
-
-        self._key = key
-
-    @property
     def value(self):
-        """Gets the value of this FacetsNode.  # noqa: E501
+        """Gets the value of this FiltersNode.  # noqa: E501
 
 
-        :return: The value of this FacetsNode.  # noqa: E501
-        :rtype: object
+        :return: The value of this FiltersNode.  # noqa: E501
+        :rtype: list[str]
         """
         return self._value
 
     @value.setter
     def value(self, value):
-        """Sets the value of this FacetsNode.
+        """Sets the value of this FiltersNode.
 
 
-        :param value: The value of this FacetsNode.  # noqa: E501
-        :type: object
+        :param value: The value of this FiltersNode.  # noqa: E501
+        :type: list[str]
         """
 
         self._value = value
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
@@ -132,15 +100,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(FacetsNode, dict):
+        if issubclass(FiltersNode, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -148,15 +116,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, FacetsNode):
+        if not isinstance(other, FiltersNode):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `phenomApis-0.0.8/phenom/api/exsearch/models/filters_node.py` & `phenomApis-0.0.9/phenom/api/exsearch/models/tab_info_node.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,97 +1,117 @@
 # coding: utf-8
 
 """
     ex-search-api
 
     These APIs helps to search and suggest based on keyword among employee profiles  # noqa: E501
 
-    OpenAPI spec version: 1.0.0
     
-    Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class FiltersNode(object):
-    """NOTE: This class is auto generated by the swagger code generator program.
-
-    Do not edit the class manually.
-    """
+class TabInfoNode(object):
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
-        'field': 'str',
-        'value': 'list[str]'
+        'key': 'str',
+        'type': 'str',
+        'mutual_history': 'bool'
     }
 
     attribute_map = {
-        'field': 'field',
-        'value': 'value'
+        'key': 'key',
+        'type': 'type',
+        'mutual_history': 'mutualHistory'
     }
 
-    def __init__(self, field=None, value=None):  # noqa: E501
-        """FiltersNode - a model defined in Swagger"""  # noqa: E501
-        self._field = None
-        self._value = None
+    def __init__(self, key=None, type=None, mutual_history=None):  # noqa: E501
+        """TabInfoNode - a model defined in Swagger"""  # noqa: E501
+        self._key = None
+        self._type = None
+        self._mutual_history = None
         self.discriminator = None
-        if field is not None:
-            self.field = field
-        if value is not None:
-            self.value = value
+        if key is not None:
+            self.key = key
+        if type is not None:
+            self.type = type
+        if mutual_history is not None:
+            self.mutual_history = mutual_history
+
+    @property
+    def key(self):
+        """Gets the key of this TabInfoNode.  # noqa: E501
+
+
+        :return: The key of this TabInfoNode.  # noqa: E501
+        :rtype: str
+        """
+        return self._key
+
+    @key.setter
+    def key(self, key):
+        """Sets the key of this TabInfoNode.
+
+
+        :param key: The key of this TabInfoNode.  # noqa: E501
+        :type: str
+        """
+
+        self._key = key
 
     @property
-    def field(self):
-        """Gets the field of this FiltersNode.  # noqa: E501
+    def type(self):
+        """Gets the type of this TabInfoNode.  # noqa: E501
 
 
-        :return: The field of this FiltersNode.  # noqa: E501
+        :return: The type of this TabInfoNode.  # noqa: E501
         :rtype: str
         """
-        return self._field
+        return self._type
 
-    @field.setter
-    def field(self, field):
-        """Sets the field of this FiltersNode.
+    @type.setter
+    def type(self, type):
+        """Sets the type of this TabInfoNode.
 
 
-        :param field: The field of this FiltersNode.  # noqa: E501
+        :param type: The type of this TabInfoNode.  # noqa: E501
         :type: str
         """
 
-        self._field = field
+        self._type = type
 
     @property
-    def value(self):
-        """Gets the value of this FiltersNode.  # noqa: E501
+    def mutual_history(self):
+        """Gets the mutual_history of this TabInfoNode.  # noqa: E501
 
 
-        :return: The value of this FiltersNode.  # noqa: E501
-        :rtype: list[str]
+        :return: The mutual_history of this TabInfoNode.  # noqa: E501
+        :rtype: bool
         """
-        return self._value
+        return self._mutual_history
 
-    @value.setter
-    def value(self, value):
-        """Sets the value of this FiltersNode.
+    @mutual_history.setter
+    def mutual_history(self, mutual_history):
+        """Sets the mutual_history of this TabInfoNode.
 
 
-        :param value: The value of this FiltersNode.  # noqa: E501
-        :type: list[str]
+        :param mutual_history: The mutual_history of this TabInfoNode.  # noqa: E501
+        :type: bool
         """
 
-        self._value = value
+        self._mutual_history = mutual_history
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
             value = getattr(self, attr)
@@ -106,15 +126,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(FiltersNode, dict):
+        if issubclass(TabInfoNode, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -122,15 +142,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, FiltersNode):
+        if not isinstance(other, TabInfoNode):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `phenomApis-0.0.8/phenom/api/exsearch/models/mentor_type_ahead_request.py` & `phenomApis-0.0.9/phenom/api/exsearch/models/mentor_type_ahead_request.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,29 +1,23 @@
 # coding: utf-8
 
 """
     ex-search-api
 
     These APIs helps to search and suggest based on keyword among employee profiles  # noqa: E501
 
-    OpenAPI spec version: 1.0.0
     
-    Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 class MentorTypeAheadRequest(object):
-    """NOTE: This class is auto generated by the swagger code generator program.
-
-    Do not edit the class manually.
-    """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
```

### Comparing `phenomApis-0.0.8/phenom/api/exsearch/models/mentor_typeahead_response.py` & `phenomApis-0.0.9/phenom/api/exsearch/models/mentor_typeahead_response.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,29 +1,23 @@
 # coding: utf-8
 
 """
     ex-search-api
 
     These APIs helps to search and suggest based on keyword among employee profiles  # noqa: E501
 
-    OpenAPI spec version: 1.0.0
     
-    Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 class MentorTypeaheadResponse(object):
-    """NOTE: This class is auto generated by the swagger code generator program.
-
-    Do not edit the class manually.
-    """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
```

### Comparing `phenomApis-0.0.8/phenom/api/prediction/__init__.py` & `phenomApis-0.0.9/phenom/api/prediction/models/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,26 +1,20 @@
 # coding: utf-8
 
 # flake8: noqa
-
 """
     prediction-api
 
     Prediction api   # noqa: E501
 
-    OpenAPI spec version: 1.0.0
     
-    Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
-# import apis into sdk package
-from phenom.api.prediction.prediction_api import PredictionApi
-# import ApiClient
-# import models into sdk package
+# import models into model package
 from phenom.api.prediction.models.bad_request import BadRequest
 from phenom.api.prediction.models.error_response import ErrorResponse
 from phenom.api.prediction.models.fyf_skill_request import FYFSkillRequest
 from phenom.api.prediction.models.fyf_skill_response import FYFSkillResponse
 from phenom.api.prediction.models.skill_result import SkillResult
 from phenom.api.prediction.models.skill_results import SkillResults
```

### Comparing `phenomApis-0.0.8/phenom/api/prediction/models/bad_request.py` & `phenomApis-0.0.9/phenom/api/search/models/bad_request.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,29 +1,23 @@
 # coding: utf-8
 
 """
-    prediction-api
+    search-api
 
-    Prediction api   # noqa: E501
+    These APIs helps to search and suggest based on keyword among available jobs  # noqa: E501
 
-    OpenAPI spec version: 1.0.0
     
-    Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 class BadRequest(object):
-    """NOTE: This class is auto generated by the swagger code generator program.
-
-    Do not edit the class manually.
-    """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
```

### Comparing `phenomApis-0.0.8/phenom/api/prediction/models/error_response.py` & `phenomApis-0.0.9/phenom/api/recomendation/models/error_response.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,29 +1,23 @@
 # coding: utf-8
 
 """
-    prediction-api
+    recommendations-api
 
-    Prediction api   # noqa: E501
+    Profile Based Job recommendations, Similar Jobs and Near By Jobs  # noqa: E501
 
-    OpenAPI spec version: 1.0.0
     
-    Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 class ErrorResponse(object):
-    """NOTE: This class is auto generated by the swagger code generator program.
-
-    Do not edit the class manually.
-    """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
```

### Comparing `phenomApis-0.0.8/phenom/api/prediction/models/fyf_skill_request.py` & `phenomApis-0.0.9/phenom/api/prediction/models/fyf_skill_request.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,29 +1,23 @@
 # coding: utf-8
 
 """
     prediction-api
 
     Prediction api   # noqa: E501
 
-    OpenAPI spec version: 1.0.0
     
-    Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 class FYFSkillRequest(object):
-    """NOTE: This class is auto generated by the swagger code generator program.
-
-    Do not edit the class manually.
-    """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
```

### Comparing `phenomApis-0.0.8/phenom/api/prediction/models/fyf_skill_response.py` & `phenomApis-0.0.9/phenom/api/exsearch/models/employee_typeahead_response.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,150 +1,143 @@
 # coding: utf-8
 
 """
-    prediction-api
+    ex-search-api
 
-    Prediction api   # noqa: E501
+    These APIs helps to search and suggest based on keyword among employee profiles  # noqa: E501
 
-    OpenAPI spec version: 1.0.0
     
-    Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class FYFSkillResponse(object):
-    """NOTE: This class is auto generated by the swagger code generator program.
-
-    Do not edit the class manually.
-    """
+class EmployeeTypeaheadResponse(object):
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
-        'status': 'str',
+        'status': 'int',
+        'hits': 'int',
         'total_hits': 'int',
-        'data': 'SkillResults',
-        'message': 'str'
+        'data': 'EmployeeTypeaheadResponseData'
     }
 
     attribute_map = {
         'status': 'status',
+        'hits': 'hits',
         'total_hits': 'totalHits',
-        'data': 'data',
-        'message': 'message'
+        'data': 'data'
     }
 
-    def __init__(self, status=None, total_hits=None, data=None, message=None):  # noqa: E501
-        """FYFSkillResponse - a model defined in Swagger"""  # noqa: E501
+    def __init__(self, status=None, hits=None, total_hits=None, data=None):  # noqa: E501
+        """EmployeeTypeaheadResponse - a model defined in Swagger"""  # noqa: E501
         self._status = None
+        self._hits = None
         self._total_hits = None
         self._data = None
-        self._message = None
         self.discriminator = None
-        self.status = status
+        if status is not None:
+            self.status = status
+        if hits is not None:
+            self.hits = hits
         if total_hits is not None:
             self.total_hits = total_hits
         if data is not None:
             self.data = data
-        if message is not None:
-            self.message = message
 
     @property
     def status(self):
-        """Gets the status of this FYFSkillResponse.  # noqa: E501
+        """Gets the status of this EmployeeTypeaheadResponse.  # noqa: E501
 
 
-        :return: The status of this FYFSkillResponse.  # noqa: E501
-        :rtype: str
+        :return: The status of this EmployeeTypeaheadResponse.  # noqa: E501
+        :rtype: int
         """
         return self._status
 
     @status.setter
     def status(self, status):
-        """Sets the status of this FYFSkillResponse.
+        """Sets the status of this EmployeeTypeaheadResponse.
 
 
-        :param status: The status of this FYFSkillResponse.  # noqa: E501
-        :type: str
+        :param status: The status of this EmployeeTypeaheadResponse.  # noqa: E501
+        :type: int
         """
-        if status is None:
-            raise ValueError("Invalid value for `status`, must not be `None`")  # noqa: E501
 
         self._status = status
 
     @property
-    def total_hits(self):
-        """Gets the total_hits of this FYFSkillResponse.  # noqa: E501
+    def hits(self):
+        """Gets the hits of this EmployeeTypeaheadResponse.  # noqa: E501
 
 
-        :return: The total_hits of this FYFSkillResponse.  # noqa: E501
+        :return: The hits of this EmployeeTypeaheadResponse.  # noqa: E501
         :rtype: int
         """
-        return self._total_hits
+        return self._hits
 
-    @total_hits.setter
-    def total_hits(self, total_hits):
-        """Sets the total_hits of this FYFSkillResponse.
+    @hits.setter
+    def hits(self, hits):
+        """Sets the hits of this EmployeeTypeaheadResponse.
 
 
-        :param total_hits: The total_hits of this FYFSkillResponse.  # noqa: E501
+        :param hits: The hits of this EmployeeTypeaheadResponse.  # noqa: E501
         :type: int
         """
 
-        self._total_hits = total_hits
+        self._hits = hits
 
     @property
-    def data(self):
-        """Gets the data of this FYFSkillResponse.  # noqa: E501
+    def total_hits(self):
+        """Gets the total_hits of this EmployeeTypeaheadResponse.  # noqa: E501
 
 
-        :return: The data of this FYFSkillResponse.  # noqa: E501
-        :rtype: SkillResults
+        :return: The total_hits of this EmployeeTypeaheadResponse.  # noqa: E501
+        :rtype: int
         """
-        return self._data
+        return self._total_hits
 
-    @data.setter
-    def data(self, data):
-        """Sets the data of this FYFSkillResponse.
+    @total_hits.setter
+    def total_hits(self, total_hits):
+        """Sets the total_hits of this EmployeeTypeaheadResponse.
 
 
-        :param data: The data of this FYFSkillResponse.  # noqa: E501
-        :type: SkillResults
+        :param total_hits: The total_hits of this EmployeeTypeaheadResponse.  # noqa: E501
+        :type: int
         """
 
-        self._data = data
+        self._total_hits = total_hits
 
     @property
-    def message(self):
-        """Gets the message of this FYFSkillResponse.  # noqa: E501
+    def data(self):
+        """Gets the data of this EmployeeTypeaheadResponse.  # noqa: E501
 
 
-        :return: The message of this FYFSkillResponse.  # noqa: E501
-        :rtype: str
+        :return: The data of this EmployeeTypeaheadResponse.  # noqa: E501
+        :rtype: EmployeeTypeaheadResponseData
         """
-        return self._message
+        return self._data
 
-    @message.setter
-    def message(self, message):
-        """Sets the message of this FYFSkillResponse.
+    @data.setter
+    def data(self, data):
+        """Sets the data of this EmployeeTypeaheadResponse.
 
 
-        :param message: The message of this FYFSkillResponse.  # noqa: E501
-        :type: str
+        :param data: The data of this EmployeeTypeaheadResponse.  # noqa: E501
+        :type: EmployeeTypeaheadResponseData
         """
 
-        self._message = message
+        self._data = data
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
             value = getattr(self, attr)
@@ -159,15 +152,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(FYFSkillResponse, dict):
+        if issubclass(EmployeeTypeaheadResponse, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -175,15 +168,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, FYFSkillResponse):
+        if not isinstance(other, EmployeeTypeaheadResponse):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `phenomApis-0.0.8/phenom/api/prediction/models/skill_result.py` & `phenomApis-0.0.9/phenom/api/prediction/models/skill_result.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,29 +1,23 @@
 # coding: utf-8
 
 """
     prediction-api
 
     Prediction api   # noqa: E501
 
-    OpenAPI spec version: 1.0.0
     
-    Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 class SkillResult(object):
-    """NOTE: This class is auto generated by the swagger code generator program.
-
-    Do not edit the class manually.
-    """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
```

### Comparing `phenomApis-0.0.8/phenom/api/prediction/models/skill_results.py` & `phenomApis-0.0.9/phenom/api/prediction/models/skill_results.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,29 +1,23 @@
 # coding: utf-8
 
 """
     prediction-api
 
     Prediction api   # noqa: E501
 
-    OpenAPI spec version: 1.0.0
     
-    Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 class SkillResults(object):
-    """NOTE: This class is auto generated by the swagger code generator program.
-
-    Do not edit the class manually.
-    """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
```

### Comparing `phenomApis-0.0.8/phenom/api/prediction/prediction_api.py` & `phenomApis-0.0.9/phenom/api/prediction/prediction_api.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,35 +1,28 @@
 # coding: utf-8
 
 """
     prediction-api
 
     Prediction api   # noqa: E501
 
-    OpenAPI spec version: 1.0.0
     
-    Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import re  # noqa: F401
 
 # python 2 and python 3 compatibility library
 import six
 
 from phenom.commons.api_client import ApiClient
 
 
 class PredictionApi(object):
-    """NOTE: This class is auto generated by the swagger code generator program.
-
-    Do not edit the class manually.
-    Ref: https://github.com/swagger-api/swagger-codegen
-    """
 
     base_path = "/prediction"
 
     def __init__(self, token, gateway_url, apikey, api_client=None):
         if api_client is None:
             api_client = ApiClient(gateway_url + self.base_path, apikey, token)
         self.api_client = api_client
```

### Comparing `phenomApis-0.0.8/phenom/api/resumeparser/__init__.py` & `phenomApis-0.0.9/phenom/api/resumeparser/models/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,28 +1,21 @@
 # coding: utf-8
 
 # flake8: noqa
-
 """
     resume-parser-api
 
     The Resume Parser extracts important information of a candidate such as candidate's name, contact information, email id, education, work experience, and skills, etc. from the resume using Deep learning models.  # noqa: E501
 
-    OpenAPI spec version: 1.0.0
     
-    Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
-# import apis into sdk package
-from phenom.api.resumeparser.resume_parsing_api import ResumeParsingApi
-# import ApiClient
-
-# import models into sdk package
+# import models into model package
 from phenom.api.resumeparser.models.error_response import ErrorResponse
 from phenom.api.resumeparser.models.error_response_errors import ErrorResponseErrors
 from phenom.api.resumeparser.models.resume_file_request import ResumeFileRequest
 from phenom.api.resumeparser.models.resume_request import ResumeRequest
 from phenom.api.resumeparser.models.resume_response import ResumeResponse
 from phenom.api.resumeparser.models.resume_response_data import ResumeResponseData
 from phenom.api.resumeparser.models.resume_response_data_resumedata import ResumeResponseDataResumedata
```

### Comparing `phenomApis-0.0.8/phenom/api/resumeparser/models/__init__.py` & `phenomApis-0.0.9/phenom/api/resumeparser/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 # coding: utf-8
 
 # flake8: noqa
+
 """
     resume-parser-api
 
     The Resume Parser extracts important information of a candidate such as candidate's name, contact information, email id, education, work experience, and skills, etc. from the resume using Deep learning models.  # noqa: E501
 
-    OpenAPI spec version: 1.0.0
     
-    Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
-# import models into model package
+# import apis into sdk package
+from phenom.api.resumeparser.resume_parsing_api import ResumeParsingApi
+# import ApiClient
+
+# import models into sdk package
 from phenom.api.resumeparser.models.error_response import ErrorResponse
 from phenom.api.resumeparser.models.error_response_errors import ErrorResponseErrors
 from phenom.api.resumeparser.models.resume_file_request import ResumeFileRequest
 from phenom.api.resumeparser.models.resume_request import ResumeRequest
 from phenom.api.resumeparser.models.resume_response import ResumeResponse
 from phenom.api.resumeparser.models.resume_response_data import ResumeResponseData
 from phenom.api.resumeparser.models.resume_response_data_resumedata import ResumeResponseDataResumedata
```

### Comparing `phenomApis-0.0.8/phenom/api/resumeparser/models/error_response.py` & `phenomApis-0.0.9/phenom/api/resumeparser/models/error_response.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,31 +1,25 @@
 # coding: utf-8
 
 """
     resume-parser-api
 
     The Resume Parser extracts important information of a candidate such as candidate's name, contact information, email id, education, work experience, and skills, etc. from the resume using Deep learning models.  # noqa: E501
 
-    OpenAPI spec version: 1.0.0
     
-    Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 from phenom.api.resumeparser.models.error_response_errors import ErrorResponseErrors  # noqa: F401,E501
 
 
 class ErrorResponse(object):
-    """NOTE: This class is auto generated by the swagger code generator program.
-
-    Do not edit the class manually.
-    """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
```

### Comparing `phenomApis-0.0.8/phenom/api/resumeparser/models/error_response_errors.py` & `phenomApis-0.0.9/phenom/api/resumeparser/models/error_response_errors.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,30 +1,24 @@
 # coding: utf-8
 
 """
     resume-parser-api
 
     The Resume Parser extracts important information of a candidate such as candidate's name, contact information, email id, education, work experience, and skills, etc. from the resume using Deep learning models.  # noqa: E501
 
-    OpenAPI spec version: 1.0.0
     
-    Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 
 class ErrorResponseErrors(object):
-    """NOTE: This class is auto generated by the swagger code generator program.
-
-    Do not edit the class manually.
-    """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
```

### Comparing `phenomApis-0.0.8/phenom/api/resumeparser/models/resume_file_request.py` & `phenomApis-0.0.9/phenom/api/resumeparser/models/resume_file_request.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,30 +1,24 @@
 # coding: utf-8
 
 """
     resume-parser-api
 
     The Resume Parser extracts important information of a candidate such as candidate's name, contact information, email id, education, work experience, and skills, etc. from the resume using Deep learning models.  # noqa: E501
 
-    OpenAPI spec version: 1.0.0
     
-    Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 
 class ResumeFileRequest(object):
-    """NOTE: This class is auto generated by the swagger code generator program.
-
-    Do not edit the class manually.
-    """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
```

### Comparing `phenomApis-0.0.8/phenom/api/resumeparser/models/resume_request.py` & `phenomApis-0.0.9/phenom/api/resumeparser/models/resume_request.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,30 +1,24 @@
 # coding: utf-8
 
 """
     resume-parser-api
 
     The Resume Parser extracts important information of a candidate such as candidate's name, contact information, email id, education, work experience, and skills, etc. from the resume using Deep learning models.  # noqa: E501
 
-    OpenAPI spec version: 1.0.0
     
-    Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 
 class ResumeRequest(object):
-    """NOTE: This class is auto generated by the swagger code generator program.
-
-    Do not edit the class manually.
-    """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
```

### Comparing `phenomApis-0.0.8/phenom/api/resumeparser/models/resume_response.py` & `phenomApis-0.0.9/phenom/api/resumeparser/models/resume_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,31 +1,25 @@
 # coding: utf-8
 
 """
     resume-parser-api
 
     The Resume Parser extracts important information of a candidate such as candidate's name, contact information, email id, education, work experience, and skills, etc. from the resume using Deep learning models.  # noqa: E501
 
-    OpenAPI spec version: 1.0.0
     
-    Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 from phenom.api.resumeparser.models.resume_response_data import ResumeResponseData  # noqa: F401,E501
 
 
 class ResumeResponse(object):
-    """NOTE: This class is auto generated by the swagger code generator program.
-
-    Do not edit the class manually.
-    """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
```

### Comparing `phenomApis-0.0.8/phenom/api/resumeparser/models/resume_response_data.py` & `phenomApis-0.0.9/phenom/api/resumeparser/models/resume_response_data_resumedata_internetaddress.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,73 +1,92 @@
 # coding: utf-8
 
 """
     resume-parser-api
 
     The Resume Parser extracts important information of a candidate such as candidate's name, contact information, email id, education, work experience, and skills, etc. from the resume using Deep learning models.  # noqa: E501
 
-    OpenAPI spec version: 1.0.0
     
-    Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
-from phenom.api.resumeparser.models.resume_response_data_resumedata import ResumeResponseDataResumedata  # noqa: F401,E501
 
 
-class ResumeResponseData(object):
-    """NOTE: This class is auto generated by the swagger code generator program.
-
-    Do not edit the class manually.
-    """
+class ResumeResponseDataResumedataInternetaddress(object):
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
-        'resumedata': 'ResumeResponseDataResumedata'
+        'type': 'str',
+        'url': 'str'
     }
 
     attribute_map = {
-        'resumedata': 'resumedata'
+        'type': 'type',
+        'url': 'url'
     }
 
-    def __init__(self, resumedata=None):  # noqa: E501
-        """ResumeResponseData - a model defined in Swagger"""  # noqa: E501
-        self._resumedata = None
+    def __init__(self, type=None, url=None):  # noqa: E501
+        """ResumeResponseDataResumedataInternetaddress - a model defined in Swagger"""  # noqa: E501
+        self._type = None
+        self._url = None
         self.discriminator = None
-        if resumedata is not None:
-            self.resumedata = resumedata
+        if type is not None:
+            self.type = type
+        if url is not None:
+            self.url = url
+
+    @property
+    def type(self):
+        """Gets the type of this ResumeResponseDataResumedataInternetaddress.  # noqa: E501
+
+
+        :return: The type of this ResumeResponseDataResumedataInternetaddress.  # noqa: E501
+        :rtype: str
+        """
+        return self._type
+
+    @type.setter
+    def type(self, type):
+        """Sets the type of this ResumeResponseDataResumedataInternetaddress.
+
+
+        :param type: The type of this ResumeResponseDataResumedataInternetaddress.  # noqa: E501
+        :type: str
+        """
+
+        self._type = type
 
     @property
-    def resumedata(self):
-        """Gets the resumedata of this ResumeResponseData.  # noqa: E501
+    def url(self):
+        """Gets the url of this ResumeResponseDataResumedataInternetaddress.  # noqa: E501
 
 
-        :return: The resumedata of this ResumeResponseData.  # noqa: E501
-        :rtype: ResumeResponseDataResumedata
+        :return: The url of this ResumeResponseDataResumedataInternetaddress.  # noqa: E501
+        :rtype: str
         """
-        return self._resumedata
+        return self._url
 
-    @resumedata.setter
-    def resumedata(self, resumedata):
-        """Sets the resumedata of this ResumeResponseData.
+    @url.setter
+    def url(self, url):
+        """Sets the url of this ResumeResponseDataResumedataInternetaddress.
 
 
-        :param resumedata: The resumedata of this ResumeResponseData.  # noqa: E501
-        :type: ResumeResponseDataResumedata
+        :param url: The url of this ResumeResponseDataResumedataInternetaddress.  # noqa: E501
+        :type: str
         """
 
-        self._resumedata = resumedata
+        self._url = url
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
             value = getattr(self, attr)
@@ -82,15 +101,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(ResumeResponseData, dict):
+        if issubclass(ResumeResponseDataResumedataInternetaddress, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -98,15 +117,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, ResumeResponseData):
+        if not isinstance(other, ResumeResponseDataResumedataInternetaddress):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `phenomApis-0.0.8/phenom/api/resumeparser/models/resume_response_data_resumedata.py` & `phenomApis-0.0.9/phenom/api/resumeparser/models/resume_response_data_resumedata.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 # coding: utf-8
 
 """
     resume-parser-api
 
     The Resume Parser extracts important information of a candidate such as candidate's name, contact information, email id, education, work experience, and skills, etc. from the resume using Deep learning models.  # noqa: E501
 
-    OpenAPI spec version: 1.0.0
     
-    Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 from phenom.api.resumeparser.models.resume_response_data_resumedata_educationhistory import ResumeResponseDataResumedataEducationhistory  # noqa: F401,E501
@@ -21,18 +19,14 @@
 from phenom.api.resumeparser.models.resume_response_data_resumedata_personname import ResumeResponseDataResumedataPersonname  # noqa: F401,E501
 from phenom.api.resumeparser.models.resume_response_data_resumedata_postaladdress import ResumeResponseDataResumedataPostaladdress  # noqa: F401,E501
 from phenom.api.resumeparser.models.resume_response_data_resumedata_skilltaxonomy import ResumeResponseDataResumedataSkilltaxonomy  # noqa: F401,E501
 from phenom.api.resumeparser.models.resume_response_data_resumedata_workhistory import ResumeResponseDataResumedataWorkhistory  # noqa: F401,E501
 
 
 class ResumeResponseDataResumedata(object):
-    """NOTE: This class is auto generated by the swagger code generator program.
-
-    Do not edit the class manually.
-    """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
```

### Comparing `phenomApis-0.0.8/phenom/api/resumeparser/models/resume_response_data_resumedata_educationhistory.py` & `phenomApis-0.0.9/phenom/api/resumeparser/models/resume_response_data_resumedata_educationhistory.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,30 +1,24 @@
 # coding: utf-8
 
 """
     resume-parser-api
 
     The Resume Parser extracts important information of a candidate such as candidate's name, contact information, email id, education, work experience, and skills, etc. from the resume using Deep learning models.  # noqa: E501
 
-    OpenAPI spec version: 1.0.0
     
-    Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 
 class ResumeResponseDataResumedataEducationhistory(object):
-    """NOTE: This class is auto generated by the swagger code generator program.
-
-    Do not edit the class manually.
-    """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
```

### Comparing `phenomApis-0.0.8/phenom/api/resumeparser/models/resume_response_data_resumedata_experiencesummary.py` & `phenomApis-0.0.9/phenom/api/resumeparser/models/resume_response_data_resumedata_experiencesummary.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,30 +1,24 @@
 # coding: utf-8
 
 """
     resume-parser-api
 
     The Resume Parser extracts important information of a candidate such as candidate's name, contact information, email id, education, work experience, and skills, etc. from the resume using Deep learning models.  # noqa: E501
 
-    OpenAPI spec version: 1.0.0
     
-    Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 
 class ResumeResponseDataResumedataExperiencesummary(object):
-    """NOTE: This class is auto generated by the swagger code generator program.
-
-    Do not edit the class manually.
-    """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
```

### Comparing `phenomApis-0.0.8/phenom/api/resumeparser/models/resume_response_data_resumedata_mobile.py` & `phenomApis-0.0.9/phenom/api/resumeparser/models/resume_response_data_resumedata_mobile.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,30 +1,24 @@
 # coding: utf-8
 
 """
     resume-parser-api
 
     The Resume Parser extracts important information of a candidate such as candidate's name, contact information, email id, education, work experience, and skills, etc. from the resume using Deep learning models.  # noqa: E501
 
-    OpenAPI spec version: 1.0.0
     
-    Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 
 class ResumeResponseDataResumedataMobile(object):
-    """NOTE: This class is auto generated by the swagger code generator program.
-
-    Do not edit the class manually.
-    """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
```

### Comparing `phenomApis-0.0.8/phenom/api/resumeparser/models/resume_response_data_resumedata_personname.py` & `phenomApis-0.0.9/phenom/api/resumeparser/models/resume_response_data_resumedata_personname.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,30 +1,24 @@
 # coding: utf-8
 
 """
     resume-parser-api
 
     The Resume Parser extracts important information of a candidate such as candidate's name, contact information, email id, education, work experience, and skills, etc. from the resume using Deep learning models.  # noqa: E501
 
-    OpenAPI spec version: 1.0.0
     
-    Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 
 class ResumeResponseDataResumedataPersonname(object):
-    """NOTE: This class is auto generated by the swagger code generator program.
-
-    Do not edit the class manually.
-    """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
```

### Comparing `phenomApis-0.0.8/phenom/api/resumeparser/models/resume_response_data_resumedata_postaladdress.py` & `phenomApis-0.0.9/phenom/api/resumeparser/models/resume_response_data_resumedata_postaladdress.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,30 +1,24 @@
 # coding: utf-8
 
 """
     resume-parser-api
 
     The Resume Parser extracts important information of a candidate such as candidate's name, contact information, email id, education, work experience, and skills, etc. from the resume using Deep learning models.  # noqa: E501
 
-    OpenAPI spec version: 1.0.0
     
-    Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 
 class ResumeResponseDataResumedataPostaladdress(object):
-    """NOTE: This class is auto generated by the swagger code generator program.
-
-    Do not edit the class manually.
-    """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
```

### Comparing `phenomApis-0.0.8/phenom/api/resumeparser/models/resume_response_data_resumedata_skilltaxonomy.py` & `phenomApis-0.0.9/phenom/api/resumeparser/models/resume_response_data_resumedata_skilltaxonomy.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,30 +1,24 @@
 # coding: utf-8
 
 """
     resume-parser-api
 
     The Resume Parser extracts important information of a candidate such as candidate's name, contact information, email id, education, work experience, and skills, etc. from the resume using Deep learning models.  # noqa: E501
 
-    OpenAPI spec version: 1.0.0
     
-    Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 
 class ResumeResponseDataResumedataSkilltaxonomy(object):
-    """NOTE: This class is auto generated by the swagger code generator program.
-
-    Do not edit the class manually.
-    """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
```

### Comparing `phenomApis-0.0.8/phenom/api/resumeparser/models/resume_response_data_resumedata_workhistory.py` & `phenomApis-0.0.9/phenom/api/resumeparser/models/resume_response_data_resumedata_workhistory.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,30 +1,24 @@
 # coding: utf-8
 
 """
     resume-parser-api
 
     The Resume Parser extracts important information of a candidate such as candidate's name, contact information, email id, education, work experience, and skills, etc. from the resume using Deep learning models.  # noqa: E501
 
-    OpenAPI spec version: 1.0.0
     
-    Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 
 class ResumeResponseDataResumedataWorkhistory(object):
-    """NOTE: This class is auto generated by the swagger code generator program.
-
-    Do not edit the class manually.
-    """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
```

### Comparing `phenomApis-0.0.8/phenom/api/resumeparser/resume_parsing_api.py` & `phenomApis-0.0.9/phenom/api/resumeparser/resume_parsing_api.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,34 +1,27 @@
 # coding: utf-8
 
 """
     resume-parser-api
 
     The Resume Parser extracts important information of a candidate such as candidate's name, contact information, email id, education, work experience, and skills, etc. from the resume using Deep learning models.  # noqa: E501
 
-    OpenAPI spec version: 1.0.0
     
-    Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import re  # noqa: F401
 
 # python 2 and python 3 compatibility library
 import six
 
 from phenom.commons.api_client import ApiClient
 
 class ResumeParsingApi(object):
-    """NOTE: This class is auto generated by the swagger code generator program.
-
-    Do not edit the class manually.
-    Ref: https://github.com/swagger-api/swagger-codegen
-    """
 
     base_path = "/parser/resume"
 
     def __init__(self, token, gateway_url, apikey, api_client=None):
         if api_client is None:
             api_client = ApiClient(gateway_url + self.base_path, apikey, token)
         self.api_client = api_client
```

### Comparing `phenomApis-0.0.8/phenom/api/search/__init__.py` & `phenomApis-0.0.9/phenom/api/search/models/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,29 +1,21 @@
 # coding: utf-8
 
 # flake8: noqa
-
 """
     search-api
 
     These APIs helps to search and suggest based on keyword among available jobs  # noqa: E501
 
-    OpenAPI spec version: 1.0.0
     
-    Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
-# import apis into sdk package
-from phenom.api.search.jobs_api import JobsApi
-# import ApiClient
-from phenom.commons.api_client import ApiClient
-from phenom.commons.configuration import Configuration
-# import models into sdk package
+# import models into model package
 from phenom.api.search.models.bad_request import BadRequest
 from phenom.api.search.models.error_response import ErrorResponse
 from phenom.api.search.models.job_node import JobNode
 from phenom.api.search.models.job_titles_response import JobTitlesResponse
 from phenom.api.search.models.job_titles_response_data import JobTitlesResponseData
 from phenom.api.search.models.job_titles_response_data_titles import JobTitlesResponseDataTitles
 from phenom.api.search.models.location_data import LocationData
```

### Comparing `phenomApis-0.0.8/phenom/api/search/jobs_api.py` & `phenomApis-0.0.9/phenom/api/search/jobs_api.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,35 +1,28 @@
 # coding: utf-8
 
 """
     search-api
 
     These APIs helps to search and suggest based on keyword among available jobs  # noqa: E501
 
-    OpenAPI spec version: 1.0.0
     
-    Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import re  # noqa: F401
 
 # python 2 and python 3 compatibility library
 import six
 
 from phenom.commons.api_client import ApiClient
 
 
 class JobsApi(object):
-    """NOTE: This class is auto generated by the swagger code generator program.
-
-    Do not edit the class manually.
-    Ref: https://github.com/swagger-api/swagger-codegen
-    """
 
     base_path = "/jobs-api/v1/jobs/search"
 
     def __init__(self, token, gateway_url, apikey, api_client=None):
         if api_client is None:
             api_client = ApiClient(gateway_url + self.base_path, apikey, token)
         self.api_client = api_client
```

### Comparing `phenomApis-0.0.8/phenom/api/search/models/__init__.py` & `phenomApis-0.0.9/phenom/api/search/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,23 +1,27 @@
 # coding: utf-8
 
 # flake8: noqa
+
 """
     search-api
 
     These APIs helps to search and suggest based on keyword among available jobs  # noqa: E501
 
-    OpenAPI spec version: 1.0.0
     
-    Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
-# import models into model package
+# import apis into sdk package
+from phenom.api.search.jobs_api import JobsApi
+# import ApiClient
+from phenom.commons.api_client import ApiClient
+from phenom.commons.configuration import Configuration
+# import models into sdk package
 from phenom.api.search.models.bad_request import BadRequest
 from phenom.api.search.models.error_response import ErrorResponse
 from phenom.api.search.models.job_node import JobNode
 from phenom.api.search.models.job_titles_response import JobTitlesResponse
 from phenom.api.search.models.job_titles_response_data import JobTitlesResponseData
 from phenom.api.search.models.job_titles_response_data_titles import JobTitlesResponseDataTitles
 from phenom.api.search.models.location_data import LocationData
```

### Comparing `phenomApis-0.0.8/phenom/api/search/models/error_response.py` & `phenomApis-0.0.9/phenom/api/search/models/error_response.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,29 +1,23 @@
 # coding: utf-8
 
 """
     search-api
 
     These APIs helps to search and suggest based on keyword among available jobs  # noqa: E501
 
-    OpenAPI spec version: 1.0.0
     
-    Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 class ErrorResponse(object):
-    """NOTE: This class is auto generated by the swagger code generator program.
-
-    Do not edit the class manually.
-    """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
```

### Comparing `phenomApis-0.0.8/phenom/api/search/models/job_node.py` & `phenomApis-0.0.9/phenom/api/search/models/job_node.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,29 +1,23 @@
 # coding: utf-8
 
 """
     search-api
 
     These APIs helps to search and suggest based on keyword among available jobs  # noqa: E501
 
-    OpenAPI spec version: 1.0.0
     
-    Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 class JobNode(object):
-    """NOTE: This class is auto generated by the swagger code generator program.
-
-    Do not edit the class manually.
-    """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
```

### Comparing `phenomApis-0.0.8/phenom/api/search/models/job_titles_response.py` & `phenomApis-0.0.9/phenom/api/search/models/refine_search_response.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,94 +1,88 @@
 # coding: utf-8
 
 """
     search-api
 
     These APIs helps to search and suggest based on keyword among available jobs  # noqa: E501
 
-    OpenAPI spec version: 1.0.0
     
-    Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class JobTitlesResponse(object):
-    """NOTE: This class is auto generated by the swagger code generator program.
-
-    Do not edit the class manually.
-    """
+class RefineSearchResponse(object):
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
         'status': 'str',
-        'data': 'JobTitlesResponseData'
+        'data': 'RefineSearchResponseData'
     }
 
     attribute_map = {
         'status': 'status',
         'data': 'data'
     }
 
     def __init__(self, status=None, data=None):  # noqa: E501
-        """JobTitlesResponse - a model defined in Swagger"""  # noqa: E501
+        """RefineSearchResponse - a model defined in Swagger"""  # noqa: E501
         self._status = None
         self._data = None
         self.discriminator = None
         if status is not None:
             self.status = status
         if data is not None:
             self.data = data
 
     @property
     def status(self):
-        """Gets the status of this JobTitlesResponse.  # noqa: E501
+        """Gets the status of this RefineSearchResponse.  # noqa: E501
 
 
-        :return: The status of this JobTitlesResponse.  # noqa: E501
+        :return: The status of this RefineSearchResponse.  # noqa: E501
         :rtype: str
         """
         return self._status
 
     @status.setter
     def status(self, status):
-        """Sets the status of this JobTitlesResponse.
+        """Sets the status of this RefineSearchResponse.
 
 
-        :param status: The status of this JobTitlesResponse.  # noqa: E501
+        :param status: The status of this RefineSearchResponse.  # noqa: E501
         :type: str
         """
 
         self._status = status
 
     @property
     def data(self):
-        """Gets the data of this JobTitlesResponse.  # noqa: E501
+        """Gets the data of this RefineSearchResponse.  # noqa: E501
 
 
-        :return: The data of this JobTitlesResponse.  # noqa: E501
-        :rtype: JobTitlesResponseData
+        :return: The data of this RefineSearchResponse.  # noqa: E501
+        :rtype: RefineSearchResponseData
         """
         return self._data
 
     @data.setter
     def data(self, data):
-        """Sets the data of this JobTitlesResponse.
+        """Sets the data of this RefineSearchResponse.
 
 
-        :param data: The data of this JobTitlesResponse.  # noqa: E501
-        :type: JobTitlesResponseData
+        :param data: The data of this RefineSearchResponse.  # noqa: E501
+        :type: RefineSearchResponseData
         """
 
         self._data = data
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
@@ -106,15 +100,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(JobTitlesResponse, dict):
+        if issubclass(RefineSearchResponse, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -122,15 +116,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, JobTitlesResponse):
+        if not isinstance(other, RefineSearchResponse):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `phenomApis-0.0.8/phenom/api/search/models/job_titles_response_data.py` & `phenomApis-0.0.9/phenom/api/search/models/job_titles_response_data.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,29 +1,23 @@
 # coding: utf-8
 
 """
     search-api
 
     These APIs helps to search and suggest based on keyword among available jobs  # noqa: E501
 
-    OpenAPI spec version: 1.0.0
     
-    Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 class JobTitlesResponseData(object):
-    """NOTE: This class is auto generated by the swagger code generator program.
-
-    Do not edit the class manually.
-    """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
```

### Comparing `phenomApis-0.0.8/phenom/api/search/models/job_titles_response_data_titles.py` & `phenomApis-0.0.9/phenom/api/search/models/job_titles_response_data_titles.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,29 +1,23 @@
 # coding: utf-8
 
 """
     search-api
 
     These APIs helps to search and suggest based on keyword among available jobs  # noqa: E501
 
-    OpenAPI spec version: 1.0.0
     
-    Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 class JobTitlesResponseDataTitles(object):
-    """NOTE: This class is auto generated by the swagger code generator program.
-
-    Do not edit the class manually.
-    """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
```

### Comparing `phenomApis-0.0.8/phenom/api/search/models/location_data.py` & `phenomApis-0.0.9/phenom/api/search/models/location_data.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,29 +1,23 @@
 # coding: utf-8
 
 """
     search-api
 
     These APIs helps to search and suggest based on keyword among available jobs  # noqa: E501
 
-    OpenAPI spec version: 1.0.0
     
-    Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 class LocationData(object):
-    """NOTE: This class is auto generated by the swagger code generator program.
-
-    Do not edit the class manually.
-    """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
```

### Comparing `phenomApis-0.0.8/phenom/api/search/models/refine_search_request.py` & `phenomApis-0.0.9/phenom/api/search/models/refine_search_request.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,23 @@
 # coding: utf-8
 
 """
     search-api
 
     These APIs helps to search and suggest based on keyword among available jobs  # noqa: E501
 
-    OpenAPI spec version: 1.0.0
     
-    Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 class RefineSearchRequest(object):
-    """NOTE: This class is auto generated by the swagger code generator program.
-
-    Do not edit the class manually.
-    """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
```

### Comparing `phenomApis-0.0.8/phenom/api/search/models/refine_search_request_facets.py` & `phenomApis-0.0.9/phenom/api/search/models/refine_search_request_facets.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,29 +1,23 @@
 # coding: utf-8
 
 """
     search-api
 
     These APIs helps to search and suggest based on keyword among available jobs  # noqa: E501
 
-    OpenAPI spec version: 1.0.0
     
-    Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 class RefineSearchRequestFacets(object):
-    """NOTE: This class is auto generated by the swagger code generator program.
-
-    Do not edit the class manually.
-    """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
```

### Comparing `phenomApis-0.0.8/phenom/api/search/models/refine_search_response.py` & `phenomApis-0.0.9/phenom/api/recomendation/models/similar_jobs_response.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,94 +1,88 @@
 # coding: utf-8
 
 """
-    search-api
+    recommendations-api
 
-    These APIs helps to search and suggest based on keyword among available jobs  # noqa: E501
+    Profile Based Job recommendations, Similar Jobs and Near By Jobs  # noqa: E501
 
-    OpenAPI spec version: 1.0.0
     
-    Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class RefineSearchResponse(object):
-    """NOTE: This class is auto generated by the swagger code generator program.
-
-    Do not edit the class manually.
-    """
+class SimilarJobsResponse(object):
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
         'status': 'str',
-        'data': 'RefineSearchResponseData'
+        'data': 'SimilarJobsResponseData'
     }
 
     attribute_map = {
         'status': 'status',
         'data': 'data'
     }
 
     def __init__(self, status=None, data=None):  # noqa: E501
-        """RefineSearchResponse - a model defined in Swagger"""  # noqa: E501
+        """SimilarJobsResponse - a model defined in Swagger"""  # noqa: E501
         self._status = None
         self._data = None
         self.discriminator = None
         if status is not None:
             self.status = status
         if data is not None:
             self.data = data
 
     @property
     def status(self):
-        """Gets the status of this RefineSearchResponse.  # noqa: E501
+        """Gets the status of this SimilarJobsResponse.  # noqa: E501
 
 
-        :return: The status of this RefineSearchResponse.  # noqa: E501
+        :return: The status of this SimilarJobsResponse.  # noqa: E501
         :rtype: str
         """
         return self._status
 
     @status.setter
     def status(self, status):
-        """Sets the status of this RefineSearchResponse.
+        """Sets the status of this SimilarJobsResponse.
 
 
-        :param status: The status of this RefineSearchResponse.  # noqa: E501
+        :param status: The status of this SimilarJobsResponse.  # noqa: E501
         :type: str
         """
 
         self._status = status
 
     @property
     def data(self):
-        """Gets the data of this RefineSearchResponse.  # noqa: E501
+        """Gets the data of this SimilarJobsResponse.  # noqa: E501
 
 
-        :return: The data of this RefineSearchResponse.  # noqa: E501
-        :rtype: RefineSearchResponseData
+        :return: The data of this SimilarJobsResponse.  # noqa: E501
+        :rtype: SimilarJobsResponseData
         """
         return self._data
 
     @data.setter
     def data(self, data):
-        """Sets the data of this RefineSearchResponse.
+        """Sets the data of this SimilarJobsResponse.
 
 
-        :param data: The data of this RefineSearchResponse.  # noqa: E501
-        :type: RefineSearchResponseData
+        :param data: The data of this SimilarJobsResponse.  # noqa: E501
+        :type: SimilarJobsResponseData
         """
 
         self._data = data
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
@@ -106,15 +100,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(RefineSearchResponse, dict):
+        if issubclass(SimilarJobsResponse, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -122,15 +116,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, RefineSearchResponse):
+        if not isinstance(other, SimilarJobsResponse):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `phenomApis-0.0.8/phenom/api/search/models/refine_search_response_data.py` & `phenomApis-0.0.9/phenom/api/recomendation/models/near_by_jobs_response_data.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,71 +1,65 @@
 # coding: utf-8
 
 """
-    search-api
+    recommendations-api
 
-    These APIs helps to search and suggest based on keyword among available jobs  # noqa: E501
+    Profile Based Job recommendations, Similar Jobs and Near By Jobs  # noqa: E501
 
-    OpenAPI spec version: 1.0.0
     
-    Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class RefineSearchResponseData(object):
-    """NOTE: This class is auto generated by the swagger code generator program.
-
-    Do not edit the class manually.
-    """
+class NearByJobsResponseData(object):
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
-        'jobs': 'list[JobNode]'
+        'nearbyjobs': 'list[JobNode]'
     }
 
     attribute_map = {
-        'jobs': 'jobs'
+        'nearbyjobs': 'nearbyjobs'
     }
 
-    def __init__(self, jobs=None):  # noqa: E501
-        """RefineSearchResponseData - a model defined in Swagger"""  # noqa: E501
-        self._jobs = None
+    def __init__(self, nearbyjobs=None):  # noqa: E501
+        """NearByJobsResponseData - a model defined in Swagger"""  # noqa: E501
+        self._nearbyjobs = None
         self.discriminator = None
-        if jobs is not None:
-            self.jobs = jobs
+        if nearbyjobs is not None:
+            self.nearbyjobs = nearbyjobs
 
     @property
-    def jobs(self):
-        """Gets the jobs of this RefineSearchResponseData.  # noqa: E501
+    def nearbyjobs(self):
+        """Gets the nearbyjobs of this NearByJobsResponseData.  # noqa: E501
 
 
-        :return: The jobs of this RefineSearchResponseData.  # noqa: E501
+        :return: The nearbyjobs of this NearByJobsResponseData.  # noqa: E501
         :rtype: list[JobNode]
         """
-        return self._jobs
+        return self._nearbyjobs
 
-    @jobs.setter
-    def jobs(self, jobs):
-        """Sets the jobs of this RefineSearchResponseData.
+    @nearbyjobs.setter
+    def nearbyjobs(self, nearbyjobs):
+        """Sets the nearbyjobs of this NearByJobsResponseData.
 
 
-        :param jobs: The jobs of this RefineSearchResponseData.  # noqa: E501
+        :param nearbyjobs: The nearbyjobs of this NearByJobsResponseData.  # noqa: E501
         :type: list[JobNode]
         """
 
-        self._jobs = jobs
+        self._nearbyjobs = nearbyjobs
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
             value = getattr(self, attr)
@@ -80,15 +74,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(RefineSearchResponseData, dict):
+        if issubclass(NearByJobsResponseData, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -96,15 +90,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, RefineSearchResponseData):
+        if not isinstance(other, NearByJobsResponseData):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `phenomApis-0.0.8/phenom/commons/api_client.py` & `phenomApis-0.0.9/phenom/commons/api_client.py`

 * *Files identical despite different names*

### Comparing `phenomApis-0.0.8/phenom/commons/configuration.py` & `phenomApis-0.0.9/phenom/commons/configuration.py`

 * *Files identical despite different names*

### Comparing `phenomApis-0.0.8/phenom/commons/get_token.py` & `phenomApis-0.0.9/phenom/commons/get_token.py`

 * *Files identical despite different names*

### Comparing `phenomApis-0.0.8/phenom/commons/rest.py` & `phenomApis-0.0.9/phenom/commons/rest.py`

 * *Files identical despite different names*

### Comparing `phenomApis-0.0.8/phenomApis.egg-info/PKG-INFO` & `phenomApis-0.0.9/phenomApis.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phenomApis
-Version: 0.0.8
+Version: 0.0.9
 Summary: phenomApis
 Author: phenom
 Author-email: 8297991468h@gmail.com
 Keywords: resumeparser,exsearch
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `phenomApis-0.0.8/phenomApis.egg-info/SOURCES.txt` & `phenomApis-0.0.9/phenomApis.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -35,23 +35,50 @@
 phenom/api/exsearch/models/employee_typeahead_response_data.py
 phenom/api/exsearch/models/error_response.py
 phenom/api/exsearch/models/facets_node.py
 phenom/api/exsearch/models/filters_node.py
 phenom/api/exsearch/models/mentor_type_ahead_request.py
 phenom/api/exsearch/models/mentor_typeahead_response.py
 phenom/api/exsearch/models/tab_info_node.py
+phenom/api/jobparser/__init__.py
+phenom/api/jobparser/job_parsing_api.py
+phenom/api/jobparser/models/__init__.py
+phenom/api/jobparser/models/jd_request.py
+phenom/api/jobparser/models/job_response.py
+phenom/api/jobparser/models/trigger400_response.py
+phenom/api/jobparser/models/trigger400_response_response.py
 phenom/api/prediction/__init__.py
 phenom/api/prediction/prediction_api.py
 phenom/api/prediction/models/__init__.py
 phenom/api/prediction/models/bad_request.py
 phenom/api/prediction/models/error_response.py
 phenom/api/prediction/models/fyf_skill_request.py
 phenom/api/prediction/models/fyf_skill_response.py
 phenom/api/prediction/models/skill_result.py
 phenom/api/prediction/models/skill_results.py
+phenom/api/recomendation/__init__.py
+phenom/api/recomendation/recommendations_api.py
+phenom/api/recomendation/models/__init__.py
+phenom/api/recomendation/models/bad_request.py
+phenom/api/recomendation/models/error_response.py
+phenom/api/recomendation/models/job_node.py
+phenom/api/recomendation/models/job_recommendation.py
+phenom/api/recomendation/models/near_by_jobs_response.py
+phenom/api/recomendation/models/near_by_jobs_response_data.py
+phenom/api/recomendation/models/preferred_locations.py
+phenom/api/recomendation/models/preferred_locations_latlong.py
+phenom/api/recomendation/models/profile_matching_response.py
+phenom/api/recomendation/models/profile_matching_response_jobs.py
+phenom/api/recomendation/models/profile_matching_response_location_data.py
+phenom/api/recomendation/models/profile_matching_response_skill_gap.py
+phenom/api/recomendation/models/similar_jobs_request.py
+phenom/api/recomendation/models/similar_jobs_response.py
+phenom/api/recomendation/models/similar_jobs_response_data.py
+phenom/api/recomendation/models/similar_jobs_response_data_similar_jobs.py
+phenom/api/recomendation/models/user_profile.py
 phenom/api/resumeparser/__init__.py
 phenom/api/resumeparser/resume_parsing_api.py
 phenom/api/resumeparser/models/__init__.py
 phenom/api/resumeparser/models/error_response.py
 phenom/api/resumeparser/models/error_response_errors.py
 phenom/api/resumeparser/models/resume_file_request.py
 phenom/api/resumeparser/models/resume_request.py
@@ -86,9 +113,8 @@
 phenom/commons/configuration.py
 phenom/commons/get_token.py
 phenom/commons/rest.py
 phenomApis.egg-info/PKG-INFO
 phenomApis.egg-info/SOURCES.txt
 phenomApis.egg-info/dependency_links.txt
 phenomApis.egg-info/requires.txt
-phenomApis.egg-info/top_level.txt
-test/__init__.py
+phenomApis.egg-info/top_level.txt
```

### Comparing `phenomApis-0.0.8/setup.py` & `phenomApis-0.0.9/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 
-VERSION = '0.0.8'
+VERSION = '0.0.9'
 DESCRIPTION = 'phenomApis'
 LONG_DESCRIPTION = 'A package to access phenom apis'
 
 # Setting up
 setup(
     name="phenomApis",
     version=VERSION,
```

