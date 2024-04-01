# Comparing `tmp/pvp-backend-api-0.6.tar.gz` & `tmp/pvp-backend-api-0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pvp-backend-api-0.6.tar", last modified: Mon Apr  1 09:10:46 2024, max compression
+gzip compressed data, was "pvp-backend-api-0.7.tar", last modified: Mon Apr  1 10:31:57 2024, max compression
```

## Comparing `pvp-backend-api-0.6.tar` & `pvp-backend-api-0.7.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2024-04-01 09:10:46.603510 pvp-backend-api-0.6/
--rw-rw-rw-   0        0        0      328 2024-04-01 09:10:46.600634 pvp-backend-api-0.6/PKG-INFO
--rw-rw-rw-   0        0        0        0 2024-03-19 10:00:22.000000 pvp-backend-api-0.6/README.md
-drwxrwxrwx   0        0        0        0 2024-04-01 09:10:46.565276 pvp-backend-api-0.6/pvp_api/
--rw-rw-rw-   0        0        0      268 2024-03-27 04:37:14.000000 pvp-backend-api-0.6/pvp_api/__init__.py
--rw-rw-rw-   0        0        0     1424 2024-03-27 04:32:41.000000 pvp-backend-api-0.6/pvp_api/generator.py
-drwxrwxrwx   0        0        0        0 2024-04-01 09:10:46.569988 pvp-backend-api-0.6/pvp_api_pe_decomposition/
--rw-rw-rw-   0        0        0      280 2024-03-31 09:11:23.000000 pvp-backend-api-0.6/pvp_api_pe_decomposition/__init__.py
--rw-rw-rw-   0        0        0    16209 2024-04-01 09:09:46.000000 pvp-backend-api-0.6/pvp_api_pe_decomposition/pe_decomposition.py
-drwxrwxrwx   0        0        0        0 2024-04-01 09:10:46.572010 pvp-backend-api-0.6/pvp_api_scenario_library/
--rw-rw-rw-   0        0        0      291 2024-03-27 04:40:13.000000 pvp-backend-api-0.6/pvp_api_scenario_library/__init__.py
--rw-rw-rw-   0        0        0     1432 2024-03-27 04:33:23.000000 pvp-backend-api-0.6/pvp_api_scenario_library/scenario_library.py
-drwxrwxrwx   0        0        0        0 2024-04-01 09:10:46.597410 pvp-backend-api-0.6/pvp_backend_api.egg-info/
--rw-rw-rw-   0        0        0      328 2024-04-01 09:10:46.000000 pvp-backend-api-0.6/pvp_backend_api.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      490 2024-04-01 09:10:46.000000 pvp-backend-api-0.6/pvp_backend_api.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-01 09:10:46.000000 pvp-backend-api-0.6/pvp_backend_api.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      233 2024-04-01 09:10:46.000000 pvp-backend-api-0.6/pvp_backend_api.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        6 2024-04-01 09:10:46.000000 pvp-backend-api-0.6/pvp_backend_api.egg-info/requires.txt
--rw-rw-rw-   0        0        0       77 2024-04-01 09:10:46.000000 pvp-backend-api-0.6/pvp_backend_api.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-01 09:10:46.600634 pvp-backend-api-0.6/pvp_create_project/
--rw-rw-rw-   0        0        0      976 2024-04-01 08:51:06.000000 pvp-backend-api-0.6/pvp_create_project/__init__.py
--rw-rw-rw-   0        0        0       42 2024-04-01 09:10:46.603510 pvp-backend-api-0.6/setup.cfg
--rw-rw-rw-   0        0        0      766 2024-04-01 09:10:42.000000 pvp-backend-api-0.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-01 10:31:57.683365 pvp-backend-api-0.7/
+-rw-rw-rw-   0        0        0      328 2024-04-01 10:31:57.682346 pvp-backend-api-0.7/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2024-03-19 10:00:22.000000 pvp-backend-api-0.7/README.md
+drwxrwxrwx   0        0        0        0 2024-04-01 10:31:57.648070 pvp-backend-api-0.7/pvp_api/
+-rw-rw-rw-   0        0        0      268 2024-03-27 04:37:14.000000 pvp-backend-api-0.7/pvp_api/__init__.py
+-rw-rw-rw-   0        0        0     1424 2024-03-27 04:32:41.000000 pvp-backend-api-0.7/pvp_api/generator.py
+drwxrwxrwx   0        0        0        0 2024-04-01 10:31:57.651721 pvp-backend-api-0.7/pvp_api_pe_decomposition/
+-rw-rw-rw-   0        0        0      280 2024-03-31 09:11:23.000000 pvp-backend-api-0.7/pvp_api_pe_decomposition/__init__.py
+-rw-rw-rw-   0        0        0    16068 2024-04-01 10:31:09.000000 pvp-backend-api-0.7/pvp_api_pe_decomposition/pe_decomposition.py
+drwxrwxrwx   0        0        0        0 2024-04-01 10:31:57.655286 pvp-backend-api-0.7/pvp_api_scenario_library/
+-rw-rw-rw-   0        0        0      291 2024-03-27 04:40:13.000000 pvp-backend-api-0.7/pvp_api_scenario_library/__init__.py
+-rw-rw-rw-   0        0        0     1432 2024-03-27 04:33:23.000000 pvp-backend-api-0.7/pvp_api_scenario_library/scenario_library.py
+drwxrwxrwx   0        0        0        0 2024-04-01 10:31:57.678839 pvp-backend-api-0.7/pvp_backend_api.egg-info/
+-rw-rw-rw-   0        0        0      328 2024-04-01 10:31:57.000000 pvp-backend-api-0.7/pvp_backend_api.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      490 2024-04-01 10:31:57.000000 pvp-backend-api-0.7/pvp_backend_api.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-01 10:31:57.000000 pvp-backend-api-0.7/pvp_backend_api.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      233 2024-04-01 10:31:57.000000 pvp-backend-api-0.7/pvp_backend_api.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        6 2024-04-01 10:31:57.000000 pvp-backend-api-0.7/pvp_backend_api.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       77 2024-04-01 10:31:57.000000 pvp-backend-api-0.7/pvp_backend_api.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-01 10:31:57.679842 pvp-backend-api-0.7/pvp_create_project/
+-rw-rw-rw-   0        0        0      976 2024-04-01 08:51:06.000000 pvp-backend-api-0.7/pvp_create_project/__init__.py
+-rw-rw-rw-   0        0        0       42 2024-04-01 10:31:57.683365 pvp-backend-api-0.7/setup.cfg
+-rw-rw-rw-   0        0        0      766 2024-04-01 10:31:54.000000 pvp-backend-api-0.7/setup.py
```

### Comparing `pvp-backend-api-0.6/pvp_api/generator.py` & `pvp-backend-api-0.7/pvp_api/generator.py`

 * *Files identical despite different names*

### Comparing `pvp-backend-api-0.6/pvp_api_pe_decomposition/pe_decomposition.py` & `pvp-backend-api-0.7/pvp_api_pe_decomposition/pe_decomposition.py`

 * *Files 1% similar despite different names*

```diff
@@ -238,15 +238,15 @@
     merged_input_and_walkrate_df=pd.merge(grouped_data,walkrate_calculated_dataframe_for_skus,on=merging_col_list,how='left')
     merged_input_and_walkrate_df[net_elasticity_col_name]=merged_input_and_walkrate_df[walkrate_col_name]*merged_input_and_walkrate_df[pe_col_name]
     merged_input_and_walkrate_df[gross_internal_col_name]=merged_input_and_walkrate_df[pe_col_name]-merged_input_and_walkrate_df[net_elasticity_col_name]
     return merged_input_and_walkrate_df
 '''
 
     api_method_template='''
-from Pe-Decom-Calculation.pe_decom_calculation import filter_dataframe_based_on_col_values, filter_dataframe_on_time_period,group_input_dataframe,calculate_volume_mix,calculate_sm_grid_X_vol_mix,normalize_sm_grid_X_vol_mix,calculate_walkrate_of_skus_for_given_manufacturer,calculate_net_elasticity_and_gross_internal
+from pe_decom_calculation import filter_dataframe_based_on_col_values, filter_dataframe_on_time_period,group_input_dataframe,calculate_volume_mix,calculate_sm_grid_X_vol_mix,normalize_sm_grid_X_vol_mix,calculate_walkrate_of_skus_for_given_manufacturer,calculate_net_elasticity_and_gross_internal
 import pandas as pd
 def run_pe_decom_calculation():
     sm_grid=pd.read_csv('sm_grid.csv')
     input_file=pd.read_csv('input_data1.csv')
     input_data=input_file
     #input_file=filter_dataframe_based_on_col_values(input_file,{})
     filtered_file_on_time_pd=filter_dataframe_on_time_period(input_file,'year','month',0,4)
@@ -259,23 +259,21 @@
     net_easticity_df=calculate_net_elasticity_and_gross_internal(input_data,walkrate_calculated_df,['chain_final','description_material','marca','tipo','size','tier','category'],{'pe':'mean','ppp':'mean'},['description_material'],'gross_internal','pe','net_elasticity','walkrate')
     return net_easticity_df
 
 print(run_pe_decom_calculation())
 '''
     # Ensure output directory exists
     os.makedirs(output_path, exist_ok=True)
-    os.makedirs('Pe-Decom-Calculation', exist_ok=True)
-    # Write template to the specified path
 
-    calculation_function_template_file = os.path.join(output_path, "Pe-Decom-Calculation/pe_decom_calculation.py")
+    calculation_function_template_file = os.path.join(output_path, "pe_decom_calculation.py")
     with open(calculation_function_template_file, "w") as file:
         file.write(calculation_function_template)
     print(f"PVP PE DECOM Calculation template generated at: pe_decom_calculation")
 
-    api_method_template_file = os.path.join(output_path, "view.py")
+    api_method_template_file = os.path.join(output_path, "views.py")
     if os.path.exists(api_method_template_file):
         with open(api_method_template_file, "a") as file:
             file.write(api_method_template)
     else:
         with open(api_method_template_file, "w") as file:
             file.write(api_method_template)
     print(f"PVP PE DECOM api template generated at: view")
```

### Comparing `pvp-backend-api-0.6/pvp_api_scenario_library/scenario_library.py` & `pvp-backend-api-0.7/pvp_api_scenario_library/scenario_library.py`

 * *Files identical despite different names*

### Comparing `pvp-backend-api-0.6/pvp_create_project/__init__.py` & `pvp-backend-api-0.7/pvp_create_project/__init__.py`

 * *Files identical despite different names*

### Comparing `pvp-backend-api-0.6/setup.py` & `pvp-backend-api-0.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # setup.py
 
 from setuptools import setup, find_packages
 
 setup(
     name='pvp-backend-api',
-    version='0.6',
+    version='0.7',
     packages=find_packages(),
     install_requires=[
         'click',
     ],
     entry_points='''
         [console_scripts]
         pvp-api=pvp_api:cli
```

