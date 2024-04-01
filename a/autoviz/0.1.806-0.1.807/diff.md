# Comparing `tmp/autoviz-0.1.806.tar.gz` & `tmp/autoviz-0.1.807.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autoviz-0.1.806.tar", last modified: Wed Feb 14 15:13:45 2024, max compression
+gzip compressed data, was "autoviz-0.1.807.tar", last modified: Mon Apr  1 13:09:10 2024, max compression
```

## Comparing `autoviz-0.1.806.tar` & `autoviz-0.1.807.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0 ram       (1000) ram       (1000)        0 2024-02-14 15:13:45.394959 autoviz-0.1.806/
--rwxrwxrwx   0 ram       (1000) ram       (1000)    17082 2024-02-14 15:13:45.379336 autoviz-0.1.806/PKG-INFO
--rwxrwxrwx   0 ram       (1000) ram       (1000)    14860 2023-12-21 13:48:42.000000 autoviz-0.1.806/README.md
-drwxrwxrwx   0 ram       (1000) ram       (1000)        0 2024-02-14 15:13:45.256947 autoviz-0.1.806/autoviz/
--rwxrwxrwx   0 ram       (1000) ram       (1000)    34934 2023-12-21 13:21:06.000000 autoviz-0.1.806/autoviz/AutoViz_Class.py
--rwxrwxrwx   0 ram       (1000) ram       (1000)    64234 2024-02-14 14:56:02.000000 autoviz-0.1.806/autoviz/AutoViz_Holo.py
--rwxrwxrwx   0 ram       (1000) ram       (1000)    24022 2023-12-13 03:22:44.000000 autoviz-0.1.806/autoviz/AutoViz_NLP.py
--rwxrwxrwx   0 ram       (1000) ram       (1000)   117348 2024-01-23 16:03:14.000000 autoviz-0.1.806/autoviz/AutoViz_Utils.py
--rwxrwxrwx   0 ram       (1000) ram       (1000)      875 2024-02-14 15:03:44.000000 autoviz-0.1.806/autoviz/__init__.py
--rwxrwxrwx   0 ram       (1000) ram       (1000)      404 2024-02-14 14:56:44.000000 autoviz-0.1.806/autoviz/__version__.py
--rwxrwxrwx   0 ram       (1000) ram       (1000)    18388 2023-12-13 13:13:08.000000 autoviz-0.1.806/autoviz/classify_method.py
-drwxrwxrwx   0 ram       (1000) ram       (1000)        0 2024-02-14 15:13:45.363700 autoviz-0.1.806/autoviz.egg-info/
--rwxrwxrwx   0 ram       (1000) ram       (1000)    17082 2024-02-14 15:13:44.000000 autoviz-0.1.806/autoviz.egg-info/PKG-INFO
--rwxrwxrwx   0 ram       (1000) ram       (1000)      339 2024-02-14 15:13:44.000000 autoviz-0.1.806/autoviz.egg-info/SOURCES.txt
--rwxrwxrwx   0 ram       (1000) ram       (1000)        1 2024-02-14 15:13:44.000000 autoviz-0.1.806/autoviz.egg-info/dependency_links.txt
--rwxrwxrwx   0 ram       (1000) ram       (1000)      253 2024-02-14 15:13:44.000000 autoviz-0.1.806/autoviz.egg-info/requires.txt
--rwxrwxrwx   0 ram       (1000) ram       (1000)        8 2024-02-14 15:13:44.000000 autoviz-0.1.806/autoviz.egg-info/top_level.txt
--rwxrwxrwx   0 ram       (1000) ram       (1000)       38 2024-02-14 15:13:45.394959 autoviz-0.1.806/setup.cfg
--rwxrwxrwx   0 ram       (1000) ram       (1000)     1208 2024-02-14 15:13:29.000000 autoviz-0.1.806/setup.py
+drwxrwxrwx   0 ram       (1000) ram       (1000)        0 2024-04-01 13:09:10.208059 autoviz-0.1.807/
+-rwxrwxrwx   0 ram       (1000) ram       (1000)    17919 2024-04-01 13:09:10.208059 autoviz-0.1.807/PKG-INFO
+-rwxrwxrwx   0 ram       (1000) ram       (1000)    15585 2024-03-30 12:37:03.000000 autoviz-0.1.807/README.md
+drwxrwxrwx   0 ram       (1000) ram       (1000)        0 2024-04-01 13:09:10.076928 autoviz-0.1.807/autoviz/
+-rwxrwxrwx   0 ram       (1000) ram       (1000)    34934 2024-04-01 12:36:55.000000 autoviz-0.1.807/autoviz/AutoViz_Class.py
+-rwxrwxrwx   0 ram       (1000) ram       (1000)    64541 2024-04-01 13:04:24.000000 autoviz-0.1.807/autoviz/AutoViz_Holo.py
+-rwxrwxrwx   0 ram       (1000) ram       (1000)    24022 2024-04-01 11:59:10.000000 autoviz-0.1.807/autoviz/AutoViz_NLP.py
+-rwxrwxrwx   0 ram       (1000) ram       (1000)   117357 2024-04-01 13:05:47.000000 autoviz-0.1.807/autoviz/AutoViz_Utils.py
+-rwxrwxrwx   0 ram       (1000) ram       (1000)      875 2024-04-01 11:59:10.000000 autoviz-0.1.807/autoviz/__init__.py
+-rwxrwxrwx   0 ram       (1000) ram       (1000)      404 2024-04-01 11:59:10.000000 autoviz-0.1.807/autoviz/__version__.py
+-rwxrwxrwx   0 ram       (1000) ram       (1000)    18388 2024-04-01 11:59:10.000000 autoviz-0.1.807/autoviz/classify_method.py
+drwxrwxrwx   0 ram       (1000) ram       (1000)        0 2024-04-01 13:09:10.176813 autoviz-0.1.807/autoviz.egg-info/
+-rwxrwxrwx   0 ram       (1000) ram       (1000)    17919 2024-04-01 13:09:09.000000 autoviz-0.1.807/autoviz.egg-info/PKG-INFO
+-rwxrwxrwx   0 ram       (1000) ram       (1000)      339 2024-04-01 13:09:09.000000 autoviz-0.1.807/autoviz.egg-info/SOURCES.txt
+-rwxrwxrwx   0 ram       (1000) ram       (1000)        1 2024-04-01 13:09:09.000000 autoviz-0.1.807/autoviz.egg-info/dependency_links.txt
+-rwxrwxrwx   0 ram       (1000) ram       (1000)      254 2024-04-01 13:09:09.000000 autoviz-0.1.807/autoviz.egg-info/requires.txt
+-rwxrwxrwx   0 ram       (1000) ram       (1000)        8 2024-04-01 13:09:09.000000 autoviz-0.1.807/autoviz.egg-info/top_level.txt
+-rwxrwxrwx   0 ram       (1000) ram       (1000)       38 2024-04-01 13:09:10.208059 autoviz-0.1.807/setup.cfg
+-rwxrwxrwx   0 ram       (1000) ram       (1000)     2737 2024-03-31 23:49:00.000000 autoviz-0.1.807/setup.py
```

### Comparing `autoviz-0.1.806/PKG-INFO` & `autoviz-0.1.807/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autoviz
-Version: 0.1.806
+Version: 0.1.807
 Summary: Automatically Visualize any dataset, any size with a single line of code
 Home-page: https://github.com/AutoViML/AutoViz.git
 Author: Ram Seshadri
 License: Apache License 2.0
 Description: # AutoViz: The One-Line Automatic Data Visualization Library
         
         ![logo](images/logo.png)
@@ -37,27 +37,25 @@
         <li><a href="#disclaimer">Disclaimer</a></li>
         </ul>
         
         ## Latest
         The latest updates about `autoviz` library can be found in <a href="https://github.com/AutoViML/AutoViz/blob/master/updates.md">Updates page</a>.
         
         ## ImportantAnnouncement
-        ### Starting with version 0.1.801, an important Update Regarding Dependency Management
-        We're excited to announce a significant update to AutoViz that enhances compatibility with various Python versions and streamlines dependency management!
-        <li>Modular Dependency Loading: AutoViz now uses a more flexible approach for importing visualization libraries starting with version `0.1.801`. This means you only need to install certain dependencies (like hvplot and holoviews) if you plan to use specific backends (e.g., bokeh). This change significantly reduces installation issues for users on newer Python versions such as 3.10 and higher.</li>
-        
-        <li>Improved Backend Support: Depending on your Python environment, AutoViz dynamically adjusts to use compatible visualization libraries, ensuring a smoother user experience. Requirements:
-                "holoviews>=1.14.9",
-                "bokeh>=2.4.2",
-                "hvplot>=0.7.3",
-                "panel>=0.12.6".
-        </li>
+        ### Starting with version 0.1.807, an important update regarding Python Version Management
+        <li>We're excited to announce we've made significant updates to our `setup.py` script to dynamically manage dependencies based on your Python version. This means that when you install AutoViz, the installation process will automatically select versions of dependencies such as HoloViews, Bokeh, and hvPlot that are best suited to your specific Python environment.
+        
+        For `Python versions below 3.10`, AutoViz will use versions of its dependencies known to be stable and compatible with older Python versions.
+        
+        For `Python 3.10`, the script has been configured to use updated dependencies that address specific fixes and enhancements relevant to this version.
+        
+        For `Python 3.11 and newer versions`, setup.py ensures compatibility by selecting library versions that support the latest Python features and fixes, including critical updates made in HoloViews for Python 3.11 support.</li>
         
         ### What Does This Mean for You?
-        <li>Easier Installation: If you've faced challenges installing AutoViz due to dependency conflicts, this update is for you. Now, you can install AutoViz without needing to install all its visualization dependencies upfront.</li>
+        <li><b>Easier Installation</b>: This approach allows AutoViz to leverage the latest advancements in our dependencies while maintaining robust support for older Python versions. The installation process is seamless—simply run pip install . in the AutoViz directory, and the script takes care of the rest, tailoring the installation to your environment.</li>
         
         <li>Tailored Usage: Choose the visualization backend that works best for your environment. AutoViz will handle the rest, importing necessary libraries as needed.</li>
         
         <li>Seamless Compatibility: Users on the latest Python versions (like 3.11 and 3.12) can now enjoy a hassle-free AutoViz experience.</li>
         
         ### How to Update?
         Simply pull the latest version of AutoViz (0.1.801 and higher) from the pip repository. The modular dependency system will be automatically applied.
@@ -97,17 +95,35 @@
         ```sh
         cd <AutoViz_Destination>
         git clone git@github.com:AutoViML/AutoViz.git
         # or download and unzip https://github.com/AutoViML/AutoViz/archive/master.zip
         conda create -n <your_env_name> python=3.7 anaconda
         conda activate <your_env_name> # ON WINDOWS: `source activate <your_env_name>`
         cd AutoViz
+        ```
+        For Python versions below 3.10, install dependencies as follows:
+        
+        ```
         pip install -r requirements.txt
         ```
         
+        For Python 3.10, please use:
+        
+        ```
+        pip install -r requirements-py310.txt
+        ```
+        
+        For Python 3.11 and above, it's recommended to use:
+        
+        ```
+        pip install -r requirements-py311.txt
+        ```
+        
+        These requirement files ensure that AutoViz works seamlessly with your Python environment by installing compatible versions of libraries like HoloViews, Bokeh, and hvPlot. Please select the requirement file that corresponds to your Python version to enjoy a smooth experience with AutoViz.</li>
+        
         ## Usage
         Discover how to use AutoViz in this Medium article.
         
         In the AutoViz directory, open a Jupyter Notebook or open a command palette (terminal) and use the following code to instantiate the AutoViz_Class. You can simply run this code step by step:
         
         ```python
         from autoviz import AutoViz_Class
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: autoviz Version: 0.1.806 Summary: Automatically
+Metadata-Version: 2.1 Name: autoviz Version: 0.1.807 Summary: Automatically
 Visualize any dataset, any size with a single line of code Home-page: https://
 github.com/AutoViML/AutoViz.git Author: Ram Seshadri License: Apache License
 2.0 Description: # AutoViz: The One-Line Automatic Data Visualization Library !
 [logo](images/logo.png) Unlock the power of **AutoViz** to visualize any
 dataset, any size, with just a single line of code! Plus, now you can get a
 quick assessment of your dataset's quality and fix DQ issues through the FixDQ
 () function. [![Pepy Downloads](https://pepy.tech/badge/autoviz)](https://
@@ -28,32 +28,34 @@
     * _E_x_a_m_p_l_e_s_ _o_f_ _u_s_i_n_g_ _A_u_t_o_V_i_z
     * _M_a_i_n_t_a_i_n_e_r_s
     * _C_o_n_t_r_i_b_u_t_i_n_g
     * _L_i_c_e_n_s_e
     * _T_i_p_s_ _f_o_r_ _u_s_i_n_g_ _A_u_t_o_V_i_z
     * _D_i_s_c_l_a_i_m_e_r
 ## Latest The latest updates about `autoviz` library can be found in _U_p_d_a_t_e_s
-_p_a_g_e. ## ImportantAnnouncement ### Starting with version 0.1.801, an important
-Update Regarding Dependency Management We're excited to announce a significant
-update to AutoViz that enhances compatibility with various Python versions and
-streamlines dependency management!
-Modular Dependency Loading: AutoViz now uses a more flexible approach for
-importing visualization libraries starting with version `0.1.801`. This means
-you only need to install certain dependencies (like hvplot and holoviews) if
-you plan to use specific backends (e.g., bokeh). This change significantly
-reduces installation issues for users on newer Python versions such as 3.10 and
-higher.
-Improved Backend Support: Depending on your Python environment, AutoViz
-dynamically adjusts to use compatible visualization libraries, ensuring a
-smoother user experience. Requirements: "holoviews>=1.14.9", "bokeh>=2.4.2",
-"hvplot>=0.7.3", "panel>=0.12.6".
+_p_a_g_e. ## ImportantAnnouncement ### Starting with version 0.1.807, an important
+update regarding Python Version Management
+We're excited to announce we've made significant updates to our `setup.py`
+script to dynamically manage dependencies based on your Python version. This
+means that when you install AutoViz, the installation process will
+automatically select versions of dependencies such as HoloViews, Bokeh, and
+hvPlot that are best suited to your specific Python environment. For `Python
+versions below 3.10`, AutoViz will use versions of its dependencies known to be
+stable and compatible with older Python versions. For `Python 3.10`, the script
+has been configured to use updated dependencies that address specific fixes and
+enhancements relevant to this version. For `Python 3.11 and newer versions`,
+setup.py ensures compatibility by selecting library versions that support the
+latest Python features and fixes, including critical updates made in HoloViews
+for Python 3.11 support.
 ### What Does This Mean for You?
-Easier Installation: If you've faced challenges installing AutoViz due to
-dependency conflicts, this update is for you. Now, you can install AutoViz
-without needing to install all its visualization dependencies upfront.
+EEaassiieerr IInnssttaallllaattiioonn: This approach allows AutoViz to leverage the latest
+advancements in our dependencies while maintaining robust support for older
+Python versions. The installation process is seamlessâsimply run pip install
+. in the AutoViz directory, and the script takes care of the rest, tailoring
+the installation to your environment.
 Tailored Usage: Choose the visualization backend that works best for your
 environment. AutoViz will handle the rest, importing necessary libraries as
 needed.
 Seamless Compatibility: Users on the latest Python versions (like 3.11 and
 3.12) can now enjoy a hassle-free AutoViz experience.
 ### How to Update? Simply pull the latest version of AutoViz (0.1.801 and
 higher) from the pip repository. The modular dependency system will be
@@ -93,107 +95,114 @@
       helps you fix DQ issues with a single line of code using the FixDQ()
       function
 ## Installation **Prerequisites** - [Anaconda](https://docs.anaconda.com/
 anaconda/install/) Create a new environment and install the required
 dependencies to clone AutoViz: **From PyPi:** ```sh cd git clone
 git@github.com:AutoViML/AutoViz.git # or download and unzip https://github.com/
 AutoViML/AutoViz/archive/master.zip conda create -n python=3.7 anaconda conda
-activate # ON WINDOWS: `source activate ` cd AutoViz pip install -
-r requirements.txt ``` ## Usage Discover how to use AutoViz in this Medium
-article. In the AutoViz directory, open a Jupyter Notebook or open a command
-palette (terminal) and use the following code to instantiate the AutoViz_Class.
-You can simply run this code step by step: ```python from autoviz import
-AutoViz_Class AV = AutoViz_Class() dft = AV.AutoViz(filename) ``` AutoViz can
-use any input either filename (in CSV, txt, or JSON format) or a pandas
-dataframe. If you have a large dataset, you can set the `max_rows_analyzed` and
-`max_cols_analyzed` arguments to speed up the visualization by asking autoviz
-to sample your dataset. AutoViz can also create charts in multiple formats
-using the `chart_format` setting: - If `chart_format ='png'` or `'svg'` or
-`'jpg'`: Matplotlib charts are plotted inline. * Can be saved locally (using
-`verbose=2` setting) or displayed (`verbose=1`) in Jupyter Notebooks. * This is
-the default behavior for AutoViz. - If `chart_format='bokeh'`: Interactive
-Bokeh charts are plotted in Jupyter Notebooks. - If `chart_format='server'`,
-dashboards will pop up for each kind of chart on your browser. - If
-`chart_format='html'`, interactive Bokeh charts will be created and silently
-saved as HTML files under the `AutoViz_Plots` directory (under working folder)
-or any other directory that you specify using the `save_plot_dir` setting
-(during input). ## API Arguments for `AV.AutoViz()` method: - `filename`: Use
-an empty string ("") if there's no associated filename and you want to use a
-dataframe. In that case, using the `dfte` argument for the dataframe. Otherwise
-provide a filename and leave `dfte` argument with an empty string. Only one of
-them can be used. - `sep`: File separator (comma, semi-colon, tab, or any
-column-separating value) if you use a filename above. - `depVar`: Target
-variable in your dataset; set it as an empty string if not applicable. -
-`dfte`: name of the pandas dataframe for plotting charts; leave it as empty
-string if using a filename. - `header`: set the row number of the header row in
-your file (0 for the first row). Otherwise leave it as 0. - `verbose`: 0 for
-minimal info and charts, 1 for more info and charts, or 2 for saving charts
-locally without display. - `lowess`: Use regression lines for each pair of
-continuous variables against the target variable in small datasets; avoid using
-for large datasets (>100,000 rows). - `chart_format`: 'svg', 'png', 'jpg',
-'bokeh', 'server', or 'html' for displaying or saving charts in various
-formats, depending on the verbose option. - `max_rows_analyzed`: Limit the max
-number of rows to use for visualization when dealing with very large datasets
-(millions of rows). A statistically valid sample will be used by autoviz.
-Default is 150000 rows. - `max_cols_analyzed`: Limit the number of continuous
-variables to be analyzed. Defaul is 30 columns. - `save_plot_dir`: Directory
-for saving plots. Default is None, which saves plots under the current
-directory in a subfolder named AutoViz_Plots. If the save_plot_dir doesn't
-exist, it will be created. ## Examples Here are some examples to help you get
-started with AutoViz. If you need full jupyter notebooks with code samples they
-can be found in [examples](https://github.com/AutoViML/AutoViz/tree/master/
-Examples) folder. ### Example 1: Visualize a CSV file with a target variable
-```python from autoviz import AutoViz_Class AV = AutoViz_Class() filename =
-"your_file.csv" target_variable = "your_target_variable" dft = AV.AutoViz
-( filename, sep=",", depVar=target_variable, dfte=None, header=0, verbose=1,
-lowess=False, chart_format="svg", max_rows_analyzed=150000,
-max_cols_analyzed=30, save_plot_dir=None ) ``` ![var_charts](images/
-var_charts.JPG) ### Example 2: Visualize a Pandas DataFrame without a target
-variable: ```python import pandas as pd from autoviz import AutoViz_Class AV =
-AutoViz_Class() data = {'col1': [1, 2, 3, 4, 5], 'col2': [5, 4, 3, 2, 1]} df =
-pd.DataFrame(data) dft = AV.AutoViz( "", sep=",", depVar="", dfte=df, header=0,
-verbose=1, lowess=False, chart_format="server", max_rows_analyzed=150000,
-max_cols_analyzed=30, save_plot_dir=None ) ``` ![server_charts](images/
-server_charts.JPG) ### Example 3: Generate interactive Bokeh charts and save
-them as HTML files in a custom directory ```python from autoviz import
+activate # ON WINDOWS: `source activate ` cd AutoViz ``` For Python versions
+below 3.10, install dependencies as follows: ``` pip install -
+r requirements.txt ``` For Python 3.10, please use: ``` pip install -
+r requirements-py310.txt ``` For Python 3.11 and above, it's recommended to
+use: ``` pip install -r requirements-py311.txt ``` These requirement files
+ensure that AutoViz works seamlessly with your Python environment by installing
+compatible versions of libraries like HoloViews, Bokeh, and hvPlot. Please
+select the requirement file that corresponds to your Python version to enjoy a
+smooth experience with AutoViz.
+## Usage Discover how to use AutoViz in this Medium article. In the AutoViz
+directory, open a Jupyter Notebook or open a command palette (terminal) and use
+the following code to instantiate the AutoViz_Class. You can simply run this
+code step by step: ```python from autoviz import AutoViz_Class AV =
+AutoViz_Class() dft = AV.AutoViz(filename) ``` AutoViz can use any input either
+filename (in CSV, txt, or JSON format) or a pandas dataframe. If you have a
+large dataset, you can set the `max_rows_analyzed` and `max_cols_analyzed`
+arguments to speed up the visualization by asking autoviz to sample your
+dataset. AutoViz can also create charts in multiple formats using the
+`chart_format` setting: - If `chart_format ='png'` or `'svg'` or `'jpg'`:
+Matplotlib charts are plotted inline. * Can be saved locally (using `verbose=2`
+setting) or displayed (`verbose=1`) in Jupyter Notebooks. * This is the default
+behavior for AutoViz. - If `chart_format='bokeh'`: Interactive Bokeh charts are
+plotted in Jupyter Notebooks. - If `chart_format='server'`, dashboards will pop
+up for each kind of chart on your browser. - If `chart_format='html'`,
+interactive Bokeh charts will be created and silently saved as HTML files under
+the `AutoViz_Plots` directory (under working folder) or any other directory
+that you specify using the `save_plot_dir` setting (during input). ## API
+Arguments for `AV.AutoViz()` method: - `filename`: Use an empty string ("") if
+there's no associated filename and you want to use a dataframe. In that case,
+using the `dfte` argument for the dataframe. Otherwise provide a filename and
+leave `dfte` argument with an empty string. Only one of them can be used. -
+`sep`: File separator (comma, semi-colon, tab, or any column-separating value)
+if you use a filename above. - `depVar`: Target variable in your dataset; set
+it as an empty string if not applicable. - `dfte`: name of the pandas dataframe
+for plotting charts; leave it as empty string if using a filename. - `header`:
+set the row number of the header row in your file (0 for the first row).
+Otherwise leave it as 0. - `verbose`: 0 for minimal info and charts, 1 for more
+info and charts, or 2 for saving charts locally without display. - `lowess`:
+Use regression lines for each pair of continuous variables against the target
+variable in small datasets; avoid using for large datasets (>100,000 rows). -
+`chart_format`: 'svg', 'png', 'jpg', 'bokeh', 'server', or 'html' for
+displaying or saving charts in various formats, depending on the verbose
+option. - `max_rows_analyzed`: Limit the max number of rows to use for
+visualization when dealing with very large datasets (millions of rows). A
+statistically valid sample will be used by autoviz. Default is 150000 rows. -
+`max_cols_analyzed`: Limit the number of continuous variables to be analyzed.
+Defaul is 30 columns. - `save_plot_dir`: Directory for saving plots. Default is
+None, which saves plots under the current directory in a subfolder named
+AutoViz_Plots. If the save_plot_dir doesn't exist, it will be created. ##
+Examples Here are some examples to help you get started with AutoViz. If you
+need full jupyter notebooks with code samples they can be found in [examples]
+(https://github.com/AutoViML/AutoViz/tree/master/Examples) folder. ### Example
+1: Visualize a CSV file with a target variable ```python from autoviz import
 AutoViz_Class AV = AutoViz_Class() filename = "your_file.csv" target_variable =
-"your_target_variable" custom_plot_dir = "your_custom_plot_directory" dft =
-AV.AutoViz( filename, sep=",", depVar=target_variable, dfte=None, header=0,
-verbose=2, lowess=False, chart_format="bokeh", max_rows_analyzed=150000,
-max_cols_analyzed=30, save_plot_dir=custom_plot_dir ) ``` ![bokeh_charts]
-(images/bokeh_charts.JPG) These examples should give you an idea of how to use
-AutoViz with different scenarios and settings. By tailoring the options and
-settings, you can generate visualizations that best suit your needs, whether
-you're working with large datasets, interactive charts, or simply exploring the
-relationships between variables. ## Maintainers AutoViz is actively maintained
-and improved by a team of dedicated developers. If you have any questions,
-suggestions, or issues, feel free to reach out to the maintainers: -
-[@AutoViML](https://github.com/AutoViML) - [@morenoh149](https://github.com/
-morenoh149) - [@hironroy](https://github.com/hironroy) ## Contributing We
-welcome contributions from the community! If you're interested in contributing
-to AutoViz, please follow these steps: - Fork the repository on GitHub. - Clone
-your fork and create a new branch for your feature or bugfix. - Commit your
-changes to the new branch, ensuring that you follow coding standards and write
-appropriate tests. - Push your changes to your fork on GitHub. - Submit a pull
-request to the main repository, detailing your changes and referencing any
-related issues. See [the contributing file](contributing.md)! ## License
-AutoViz is released under the Apache License, Version 2.0. By using AutoViz,
-you agree to the terms and conditions specified in the license. ## Tips Here
-are some additional tips and reminders to help you make the most of the
-library: - **Make sure to regularly upgrade AutoViz** to benefit from the
-latest features, bug fixes, and improvements. You can update it using pip
-install --upgrade autoviz. - **AutoViz is highly customizable, so don't
-hesitate to explore and experiment with various settings**, such as
-chart_format, verbose, and max_rows_analyzed. This will allow you to create
-visualizations that better suit your specific needs and preferences. -
-**Remember to delete the AutoViz_Plots directory (or any custom directory you
-specified) periodically** if you used the verbose=2 option, as it can
-accumulate a large number of saved charts over time. - **For further guidance
-or inspiration, check out the _M_e_d_i_u_m_ _a_r_t_i_c_l_e on AutoViz**, as well as other
-online resources and tutorials.
+"your_target_variable" dft = AV.AutoViz( filename, sep=",",
+depVar=target_variable, dfte=None, header=0, verbose=1, lowess=False,
+chart_format="svg", max_rows_analyzed=150000, max_cols_analyzed=30,
+save_plot_dir=None ) ``` ![var_charts](images/var_charts.JPG) ### Example 2:
+Visualize a Pandas DataFrame without a target variable: ```python import pandas
+as pd from autoviz import AutoViz_Class AV = AutoViz_Class() data = {'col1':
+[1, 2, 3, 4, 5], 'col2': [5, 4, 3, 2, 1]} df = pd.DataFrame(data) dft =
+AV.AutoViz( "", sep=",", depVar="", dfte=df, header=0, verbose=1, lowess=False,
+chart_format="server", max_rows_analyzed=150000, max_cols_analyzed=30,
+save_plot_dir=None ) ``` ![server_charts](images/server_charts.JPG) ### Example
+3: Generate interactive Bokeh charts and save them as HTML files in a custom
+directory ```python from autoviz import AutoViz_Class AV = AutoViz_Class()
+filename = "your_file.csv" target_variable = "your_target_variable"
+custom_plot_dir = "your_custom_plot_directory" dft = AV.AutoViz( filename,
+sep=",", depVar=target_variable, dfte=None, header=0, verbose=2, lowess=False,
+chart_format="bokeh", max_rows_analyzed=150000, max_cols_analyzed=30,
+save_plot_dir=custom_plot_dir ) ``` ![bokeh_charts](images/bokeh_charts.JPG)
+These examples should give you an idea of how to use AutoViz with different
+scenarios and settings. By tailoring the options and settings, you can generate
+visualizations that best suit your needs, whether you're working with large
+datasets, interactive charts, or simply exploring the relationships between
+variables. ## Maintainers AutoViz is actively maintained and improved by a team
+of dedicated developers. If you have any questions, suggestions, or issues,
+feel free to reach out to the maintainers: - [@AutoViML](https://github.com/
+AutoViML) - [@morenoh149](https://github.com/morenoh149) - [@hironroy](https://
+github.com/hironroy) ## Contributing We welcome contributions from the
+community! If you're interested in contributing to AutoViz, please follow these
+steps: - Fork the repository on GitHub. - Clone your fork and create a new
+branch for your feature or bugfix. - Commit your changes to the new branch,
+ensuring that you follow coding standards and write appropriate tests. - Push
+your changes to your fork on GitHub. - Submit a pull request to the main
+repository, detailing your changes and referencing any related issues. See [the
+contributing file](contributing.md)! ## License AutoViz is released under the
+Apache License, Version 2.0. By using AutoViz, you agree to the terms and
+conditions specified in the license. ## Tips Here are some additional tips and
+reminders to help you make the most of the library: - **Make sure to regularly
+upgrade AutoViz** to benefit from the latest features, bug fixes, and
+improvements. You can update it using pip install --upgrade autoviz. -
+**AutoViz is highly customizable, so don't hesitate to explore and experiment
+with various settings**, such as chart_format, verbose, and max_rows_analyzed.
+This will allow you to create visualizations that better suit your specific
+needs and preferences. - **Remember to delete the AutoViz_Plots directory (or
+any custom directory you specified) periodically** if you used the verbose=2
+option, as it can accumulate a large number of saved charts over time. - **For
+further guidance or inspiration, check out the _M_e_d_i_u_m_ _a_r_t_i_c_l_e on AutoViz**, as
+well as other online resources and tutorials.
     * AutoViz will visualize any sized file using a statistically valid sample.
     * COMMA is the default separator in the file, but you can change it.
     * Assumes the first row as the header in the file, but this can be changed.
 - **By leveraging AutoViz's powerful and flexible features**, you can
 streamline your data visualization process and gain valuable insights more
 efficiently. Happy visualizing! ## DISCLAIMER This project is not an official
 Google project. It is not supported by Google, and Google specifically
```

### Comparing `autoviz-0.1.806/README.md` & `autoviz-0.1.807/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -30,27 +30,25 @@
 <li><a href="#disclaimer">Disclaimer</a></li>
 </ul>
 
 ## Latest
 The latest updates about `autoviz` library can be found in <a href="https://github.com/AutoViML/AutoViz/blob/master/updates.md">Updates page</a>.
 
 ## ImportantAnnouncement
-### Starting with version 0.1.801, an important Update Regarding Dependency Management
-We're excited to announce a significant update to AutoViz that enhances compatibility with various Python versions and streamlines dependency management!
-<li>Modular Dependency Loading: AutoViz now uses a more flexible approach for importing visualization libraries starting with version `0.1.801`. This means you only need to install certain dependencies (like hvplot and holoviews) if you plan to use specific backends (e.g., bokeh). This change significantly reduces installation issues for users on newer Python versions such as 3.10 and higher.</li>
-
-<li>Improved Backend Support: Depending on your Python environment, AutoViz dynamically adjusts to use compatible visualization libraries, ensuring a smoother user experience. Requirements:
-        "holoviews>=1.14.9",
-        "bokeh>=2.4.2",
-        "hvplot>=0.7.3",
-        "panel>=0.12.6".
-</li>
+### Starting with version 0.1.807, an important update regarding Python Version Management
+<li>We're excited to announce we've made significant updates to our `setup.py` script to dynamically manage dependencies based on your Python version. This means that when you install AutoViz, the installation process will automatically select versions of dependencies such as HoloViews, Bokeh, and hvPlot that are best suited to your specific Python environment.
+
+For `Python versions below 3.10`, AutoViz will use versions of its dependencies known to be stable and compatible with older Python versions.
+
+For `Python 3.10`, the script has been configured to use updated dependencies that address specific fixes and enhancements relevant to this version.
+
+For `Python 3.11 and newer versions`, setup.py ensures compatibility by selecting library versions that support the latest Python features and fixes, including critical updates made in HoloViews for Python 3.11 support.</li>
 
 ### What Does This Mean for You?
-<li>Easier Installation: If you've faced challenges installing AutoViz due to dependency conflicts, this update is for you. Now, you can install AutoViz without needing to install all its visualization dependencies upfront.</li>
+<li><b>Easier Installation</b>: This approach allows AutoViz to leverage the latest advancements in our dependencies while maintaining robust support for older Python versions. The installation process is seamless—simply run pip install . in the AutoViz directory, and the script takes care of the rest, tailoring the installation to your environment.</li>
 
 <li>Tailored Usage: Choose the visualization backend that works best for your environment. AutoViz will handle the rest, importing necessary libraries as needed.</li>
 
 <li>Seamless Compatibility: Users on the latest Python versions (like 3.11 and 3.12) can now enjoy a hassle-free AutoViz experience.</li>
 
 ### How to Update?
 Simply pull the latest version of AutoViz (0.1.801 and higher) from the pip repository. The modular dependency system will be automatically applied.
@@ -90,17 +88,35 @@
 ```sh
 cd <AutoViz_Destination>
 git clone git@github.com:AutoViML/AutoViz.git
 # or download and unzip https://github.com/AutoViML/AutoViz/archive/master.zip
 conda create -n <your_env_name> python=3.7 anaconda
 conda activate <your_env_name> # ON WINDOWS: `source activate <your_env_name>`
 cd AutoViz
+```
+For Python versions below 3.10, install dependencies as follows:
+
+```
 pip install -r requirements.txt
 ```
 
+For Python 3.10, please use:
+
+```
+pip install -r requirements-py310.txt
+```
+
+For Python 3.11 and above, it's recommended to use:
+
+```
+pip install -r requirements-py311.txt
+```
+
+These requirement files ensure that AutoViz works seamlessly with your Python environment by installing compatible versions of libraries like HoloViews, Bokeh, and hvPlot. Please select the requirement file that corresponds to your Python version to enjoy a smooth experience with AutoViz.</li>
+
 ## Usage
 Discover how to use AutoViz in this Medium article.
 
 In the AutoViz directory, open a Jupyter Notebook or open a command palette (terminal) and use the following code to instantiate the AutoViz_Class. You can simply run this code step by step:
 
 ```python
 from autoviz import AutoViz_Class
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

#### html2text {}

```diff
@@ -25,32 +25,34 @@
     * _E_x_a_m_p_l_e_s_ _o_f_ _u_s_i_n_g_ _A_u_t_o_V_i_z
     * _M_a_i_n_t_a_i_n_e_r_s
     * _C_o_n_t_r_i_b_u_t_i_n_g
     * _L_i_c_e_n_s_e
     * _T_i_p_s_ _f_o_r_ _u_s_i_n_g_ _A_u_t_o_V_i_z
     * _D_i_s_c_l_a_i_m_e_r
 ## Latest The latest updates about `autoviz` library can be found in _U_p_d_a_t_e_s
-_p_a_g_e. ## ImportantAnnouncement ### Starting with version 0.1.801, an important
-Update Regarding Dependency Management We're excited to announce a significant
-update to AutoViz that enhances compatibility with various Python versions and
-streamlines dependency management!
-Modular Dependency Loading: AutoViz now uses a more flexible approach for
-importing visualization libraries starting with version `0.1.801`. This means
-you only need to install certain dependencies (like hvplot and holoviews) if
-you plan to use specific backends (e.g., bokeh). This change significantly
-reduces installation issues for users on newer Python versions such as 3.10 and
-higher.
-Improved Backend Support: Depending on your Python environment, AutoViz
-dynamically adjusts to use compatible visualization libraries, ensuring a
-smoother user experience. Requirements: "holoviews>=1.14.9", "bokeh>=2.4.2",
-"hvplot>=0.7.3", "panel>=0.12.6".
+_p_a_g_e. ## ImportantAnnouncement ### Starting with version 0.1.807, an important
+update regarding Python Version Management
+We're excited to announce we've made significant updates to our `setup.py`
+script to dynamically manage dependencies based on your Python version. This
+means that when you install AutoViz, the installation process will
+automatically select versions of dependencies such as HoloViews, Bokeh, and
+hvPlot that are best suited to your specific Python environment. For `Python
+versions below 3.10`, AutoViz will use versions of its dependencies known to be
+stable and compatible with older Python versions. For `Python 3.10`, the script
+has been configured to use updated dependencies that address specific fixes and
+enhancements relevant to this version. For `Python 3.11 and newer versions`,
+setup.py ensures compatibility by selecting library versions that support the
+latest Python features and fixes, including critical updates made in HoloViews
+for Python 3.11 support.
 ### What Does This Mean for You?
-Easier Installation: If you've faced challenges installing AutoViz due to
-dependency conflicts, this update is for you. Now, you can install AutoViz
-without needing to install all its visualization dependencies upfront.
+EEaassiieerr IInnssttaallllaattiioonn: This approach allows AutoViz to leverage the latest
+advancements in our dependencies while maintaining robust support for older
+Python versions. The installation process is seamlessâsimply run pip install
+. in the AutoViz directory, and the script takes care of the rest, tailoring
+the installation to your environment.
 Tailored Usage: Choose the visualization backend that works best for your
 environment. AutoViz will handle the rest, importing necessary libraries as
 needed.
 Seamless Compatibility: Users on the latest Python versions (like 3.11 and
 3.12) can now enjoy a hassle-free AutoViz experience.
 ### How to Update? Simply pull the latest version of AutoViz (0.1.801 and
 higher) from the pip repository. The modular dependency system will be
@@ -90,107 +92,114 @@
       helps you fix DQ issues with a single line of code using the FixDQ()
       function
 ## Installation **Prerequisites** - [Anaconda](https://docs.anaconda.com/
 anaconda/install/) Create a new environment and install the required
 dependencies to clone AutoViz: **From PyPi:** ```sh cd git clone
 git@github.com:AutoViML/AutoViz.git # or download and unzip https://github.com/
 AutoViML/AutoViz/archive/master.zip conda create -n python=3.7 anaconda conda
-activate # ON WINDOWS: `source activate ` cd AutoViz pip install -
-r requirements.txt ``` ## Usage Discover how to use AutoViz in this Medium
-article. In the AutoViz directory, open a Jupyter Notebook or open a command
-palette (terminal) and use the following code to instantiate the AutoViz_Class.
-You can simply run this code step by step: ```python from autoviz import
-AutoViz_Class AV = AutoViz_Class() dft = AV.AutoViz(filename) ``` AutoViz can
-use any input either filename (in CSV, txt, or JSON format) or a pandas
-dataframe. If you have a large dataset, you can set the `max_rows_analyzed` and
-`max_cols_analyzed` arguments to speed up the visualization by asking autoviz
-to sample your dataset. AutoViz can also create charts in multiple formats
-using the `chart_format` setting: - If `chart_format ='png'` or `'svg'` or
-`'jpg'`: Matplotlib charts are plotted inline. * Can be saved locally (using
-`verbose=2` setting) or displayed (`verbose=1`) in Jupyter Notebooks. * This is
-the default behavior for AutoViz. - If `chart_format='bokeh'`: Interactive
-Bokeh charts are plotted in Jupyter Notebooks. - If `chart_format='server'`,
-dashboards will pop up for each kind of chart on your browser. - If
-`chart_format='html'`, interactive Bokeh charts will be created and silently
-saved as HTML files under the `AutoViz_Plots` directory (under working folder)
-or any other directory that you specify using the `save_plot_dir` setting
-(during input). ## API Arguments for `AV.AutoViz()` method: - `filename`: Use
-an empty string ("") if there's no associated filename and you want to use a
-dataframe. In that case, using the `dfte` argument for the dataframe. Otherwise
-provide a filename and leave `dfte` argument with an empty string. Only one of
-them can be used. - `sep`: File separator (comma, semi-colon, tab, or any
-column-separating value) if you use a filename above. - `depVar`: Target
-variable in your dataset; set it as an empty string if not applicable. -
-`dfte`: name of the pandas dataframe for plotting charts; leave it as empty
-string if using a filename. - `header`: set the row number of the header row in
-your file (0 for the first row). Otherwise leave it as 0. - `verbose`: 0 for
-minimal info and charts, 1 for more info and charts, or 2 for saving charts
-locally without display. - `lowess`: Use regression lines for each pair of
-continuous variables against the target variable in small datasets; avoid using
-for large datasets (>100,000 rows). - `chart_format`: 'svg', 'png', 'jpg',
-'bokeh', 'server', or 'html' for displaying or saving charts in various
-formats, depending on the verbose option. - `max_rows_analyzed`: Limit the max
-number of rows to use for visualization when dealing with very large datasets
-(millions of rows). A statistically valid sample will be used by autoviz.
-Default is 150000 rows. - `max_cols_analyzed`: Limit the number of continuous
-variables to be analyzed. Defaul is 30 columns. - `save_plot_dir`: Directory
-for saving plots. Default is None, which saves plots under the current
-directory in a subfolder named AutoViz_Plots. If the save_plot_dir doesn't
-exist, it will be created. ## Examples Here are some examples to help you get
-started with AutoViz. If you need full jupyter notebooks with code samples they
-can be found in [examples](https://github.com/AutoViML/AutoViz/tree/master/
-Examples) folder. ### Example 1: Visualize a CSV file with a target variable
-```python from autoviz import AutoViz_Class AV = AutoViz_Class() filename =
-"your_file.csv" target_variable = "your_target_variable" dft = AV.AutoViz
-( filename, sep=",", depVar=target_variable, dfte=None, header=0, verbose=1,
-lowess=False, chart_format="svg", max_rows_analyzed=150000,
-max_cols_analyzed=30, save_plot_dir=None ) ``` ![var_charts](images/
-var_charts.JPG) ### Example 2: Visualize a Pandas DataFrame without a target
-variable: ```python import pandas as pd from autoviz import AutoViz_Class AV =
-AutoViz_Class() data = {'col1': [1, 2, 3, 4, 5], 'col2': [5, 4, 3, 2, 1]} df =
-pd.DataFrame(data) dft = AV.AutoViz( "", sep=",", depVar="", dfte=df, header=0,
-verbose=1, lowess=False, chart_format="server", max_rows_analyzed=150000,
-max_cols_analyzed=30, save_plot_dir=None ) ``` ![server_charts](images/
-server_charts.JPG) ### Example 3: Generate interactive Bokeh charts and save
-them as HTML files in a custom directory ```python from autoviz import
+activate # ON WINDOWS: `source activate ` cd AutoViz ``` For Python versions
+below 3.10, install dependencies as follows: ``` pip install -
+r requirements.txt ``` For Python 3.10, please use: ``` pip install -
+r requirements-py310.txt ``` For Python 3.11 and above, it's recommended to
+use: ``` pip install -r requirements-py311.txt ``` These requirement files
+ensure that AutoViz works seamlessly with your Python environment by installing
+compatible versions of libraries like HoloViews, Bokeh, and hvPlot. Please
+select the requirement file that corresponds to your Python version to enjoy a
+smooth experience with AutoViz.
+## Usage Discover how to use AutoViz in this Medium article. In the AutoViz
+directory, open a Jupyter Notebook or open a command palette (terminal) and use
+the following code to instantiate the AutoViz_Class. You can simply run this
+code step by step: ```python from autoviz import AutoViz_Class AV =
+AutoViz_Class() dft = AV.AutoViz(filename) ``` AutoViz can use any input either
+filename (in CSV, txt, or JSON format) or a pandas dataframe. If you have a
+large dataset, you can set the `max_rows_analyzed` and `max_cols_analyzed`
+arguments to speed up the visualization by asking autoviz to sample your
+dataset. AutoViz can also create charts in multiple formats using the
+`chart_format` setting: - If `chart_format ='png'` or `'svg'` or `'jpg'`:
+Matplotlib charts are plotted inline. * Can be saved locally (using `verbose=2`
+setting) or displayed (`verbose=1`) in Jupyter Notebooks. * This is the default
+behavior for AutoViz. - If `chart_format='bokeh'`: Interactive Bokeh charts are
+plotted in Jupyter Notebooks. - If `chart_format='server'`, dashboards will pop
+up for each kind of chart on your browser. - If `chart_format='html'`,
+interactive Bokeh charts will be created and silently saved as HTML files under
+the `AutoViz_Plots` directory (under working folder) or any other directory
+that you specify using the `save_plot_dir` setting (during input). ## API
+Arguments for `AV.AutoViz()` method: - `filename`: Use an empty string ("") if
+there's no associated filename and you want to use a dataframe. In that case,
+using the `dfte` argument for the dataframe. Otherwise provide a filename and
+leave `dfte` argument with an empty string. Only one of them can be used. -
+`sep`: File separator (comma, semi-colon, tab, or any column-separating value)
+if you use a filename above. - `depVar`: Target variable in your dataset; set
+it as an empty string if not applicable. - `dfte`: name of the pandas dataframe
+for plotting charts; leave it as empty string if using a filename. - `header`:
+set the row number of the header row in your file (0 for the first row).
+Otherwise leave it as 0. - `verbose`: 0 for minimal info and charts, 1 for more
+info and charts, or 2 for saving charts locally without display. - `lowess`:
+Use regression lines for each pair of continuous variables against the target
+variable in small datasets; avoid using for large datasets (>100,000 rows). -
+`chart_format`: 'svg', 'png', 'jpg', 'bokeh', 'server', or 'html' for
+displaying or saving charts in various formats, depending on the verbose
+option. - `max_rows_analyzed`: Limit the max number of rows to use for
+visualization when dealing with very large datasets (millions of rows). A
+statistically valid sample will be used by autoviz. Default is 150000 rows. -
+`max_cols_analyzed`: Limit the number of continuous variables to be analyzed.
+Defaul is 30 columns. - `save_plot_dir`: Directory for saving plots. Default is
+None, which saves plots under the current directory in a subfolder named
+AutoViz_Plots. If the save_plot_dir doesn't exist, it will be created. ##
+Examples Here are some examples to help you get started with AutoViz. If you
+need full jupyter notebooks with code samples they can be found in [examples]
+(https://github.com/AutoViML/AutoViz/tree/master/Examples) folder. ### Example
+1: Visualize a CSV file with a target variable ```python from autoviz import
 AutoViz_Class AV = AutoViz_Class() filename = "your_file.csv" target_variable =
-"your_target_variable" custom_plot_dir = "your_custom_plot_directory" dft =
-AV.AutoViz( filename, sep=",", depVar=target_variable, dfte=None, header=0,
-verbose=2, lowess=False, chart_format="bokeh", max_rows_analyzed=150000,
-max_cols_analyzed=30, save_plot_dir=custom_plot_dir ) ``` ![bokeh_charts]
-(images/bokeh_charts.JPG) These examples should give you an idea of how to use
-AutoViz with different scenarios and settings. By tailoring the options and
-settings, you can generate visualizations that best suit your needs, whether
-you're working with large datasets, interactive charts, or simply exploring the
-relationships between variables. ## Maintainers AutoViz is actively maintained
-and improved by a team of dedicated developers. If you have any questions,
-suggestions, or issues, feel free to reach out to the maintainers: -
-[@AutoViML](https://github.com/AutoViML) - [@morenoh149](https://github.com/
-morenoh149) - [@hironroy](https://github.com/hironroy) ## Contributing We
-welcome contributions from the community! If you're interested in contributing
-to AutoViz, please follow these steps: - Fork the repository on GitHub. - Clone
-your fork and create a new branch for your feature or bugfix. - Commit your
-changes to the new branch, ensuring that you follow coding standards and write
-appropriate tests. - Push your changes to your fork on GitHub. - Submit a pull
-request to the main repository, detailing your changes and referencing any
-related issues. See [the contributing file](contributing.md)! ## License
-AutoViz is released under the Apache License, Version 2.0. By using AutoViz,
-you agree to the terms and conditions specified in the license. ## Tips Here
-are some additional tips and reminders to help you make the most of the
-library: - **Make sure to regularly upgrade AutoViz** to benefit from the
-latest features, bug fixes, and improvements. You can update it using pip
-install --upgrade autoviz. - **AutoViz is highly customizable, so don't
-hesitate to explore and experiment with various settings**, such as
-chart_format, verbose, and max_rows_analyzed. This will allow you to create
-visualizations that better suit your specific needs and preferences. -
-**Remember to delete the AutoViz_Plots directory (or any custom directory you
-specified) periodically** if you used the verbose=2 option, as it can
-accumulate a large number of saved charts over time. - **For further guidance
-or inspiration, check out the _M_e_d_i_u_m_ _a_r_t_i_c_l_e on AutoViz**, as well as other
-online resources and tutorials.
+"your_target_variable" dft = AV.AutoViz( filename, sep=",",
+depVar=target_variable, dfte=None, header=0, verbose=1, lowess=False,
+chart_format="svg", max_rows_analyzed=150000, max_cols_analyzed=30,
+save_plot_dir=None ) ``` ![var_charts](images/var_charts.JPG) ### Example 2:
+Visualize a Pandas DataFrame without a target variable: ```python import pandas
+as pd from autoviz import AutoViz_Class AV = AutoViz_Class() data = {'col1':
+[1, 2, 3, 4, 5], 'col2': [5, 4, 3, 2, 1]} df = pd.DataFrame(data) dft =
+AV.AutoViz( "", sep=",", depVar="", dfte=df, header=0, verbose=1, lowess=False,
+chart_format="server", max_rows_analyzed=150000, max_cols_analyzed=30,
+save_plot_dir=None ) ``` ![server_charts](images/server_charts.JPG) ### Example
+3: Generate interactive Bokeh charts and save them as HTML files in a custom
+directory ```python from autoviz import AutoViz_Class AV = AutoViz_Class()
+filename = "your_file.csv" target_variable = "your_target_variable"
+custom_plot_dir = "your_custom_plot_directory" dft = AV.AutoViz( filename,
+sep=",", depVar=target_variable, dfte=None, header=0, verbose=2, lowess=False,
+chart_format="bokeh", max_rows_analyzed=150000, max_cols_analyzed=30,
+save_plot_dir=custom_plot_dir ) ``` ![bokeh_charts](images/bokeh_charts.JPG)
+These examples should give you an idea of how to use AutoViz with different
+scenarios and settings. By tailoring the options and settings, you can generate
+visualizations that best suit your needs, whether you're working with large
+datasets, interactive charts, or simply exploring the relationships between
+variables. ## Maintainers AutoViz is actively maintained and improved by a team
+of dedicated developers. If you have any questions, suggestions, or issues,
+feel free to reach out to the maintainers: - [@AutoViML](https://github.com/
+AutoViML) - [@morenoh149](https://github.com/morenoh149) - [@hironroy](https://
+github.com/hironroy) ## Contributing We welcome contributions from the
+community! If you're interested in contributing to AutoViz, please follow these
+steps: - Fork the repository on GitHub. - Clone your fork and create a new
+branch for your feature or bugfix. - Commit your changes to the new branch,
+ensuring that you follow coding standards and write appropriate tests. - Push
+your changes to your fork on GitHub. - Submit a pull request to the main
+repository, detailing your changes and referencing any related issues. See [the
+contributing file](contributing.md)! ## License AutoViz is released under the
+Apache License, Version 2.0. By using AutoViz, you agree to the terms and
+conditions specified in the license. ## Tips Here are some additional tips and
+reminders to help you make the most of the library: - **Make sure to regularly
+upgrade AutoViz** to benefit from the latest features, bug fixes, and
+improvements. You can update it using pip install --upgrade autoviz. -
+**AutoViz is highly customizable, so don't hesitate to explore and experiment
+with various settings**, such as chart_format, verbose, and max_rows_analyzed.
+This will allow you to create visualizations that better suit your specific
+needs and preferences. - **Remember to delete the AutoViz_Plots directory (or
+any custom directory you specified) periodically** if you used the verbose=2
+option, as it can accumulate a large number of saved charts over time. - **For
+further guidance or inspiration, check out the _M_e_d_i_u_m_ _a_r_t_i_c_l_e on AutoViz**, as
+well as other online resources and tutorials.
     * AutoViz will visualize any sized file using a statistically valid sample.
     * COMMA is the default separator in the file, but you can change it.
     * Assumes the first row as the header in the file, but this can be changed.
 - **By leveraging AutoViz's powerful and flexible features**, you can
 streamline your data visualization process and gain valuable insights more
 efficiently. Happy visualizing! ## DISCLAIMER This project is not an official
 Google project. It is not supported by Google, and Google specifically
```

### Comparing `autoviz-0.1.806/autoviz/AutoViz_Class.py` & `autoviz-0.1.807/autoviz/AutoViz_Class.py`

 * *Files identical despite different names*

### Comparing `autoviz-0.1.806/autoviz/AutoViz_Holo.py` & `autoviz-0.1.807/autoviz/AutoViz_Holo.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,17 +12,19 @@
 def warn(*args, **kwargs):
     pass
 warnings.warn = warn
 ########################################
 import logging
 logging.getLogger("param").setLevel(logging.ERROR)
 import warnings 
-#warnings.simplefilter(action='ignore', category=BokehUserWarning)
-warnings.filterwarnings("ignore")
 from sklearn.exceptions import DataConversionWarning
+warnings.filterwarnings("ignore")
+### These Bokeh warnings are useless => leave them alone for now!
+### from bokeh.util.warnings import BokehUserWarning
+## warnings.simplefilter(action='ignore', category=BokehUserWarning) 
 warnings.filterwarnings(action='ignore', category=DataConversionWarning)
 ####################################################################################
 import matplotlib
 matplotlib.use('agg')
 import matplotlib.pyplot as plt
 # from matplotlib import io
 import io
@@ -49,15 +51,15 @@
 from xgboost.sklearn import XGBClassifier
 from xgboost.sklearn import XGBRegressor
 import os
 # If specific functions/classes are needed from your own modules
 from .classify_method import classify_columns
 ##########################################################################################
 def ensure_hvplot_imported():
-    global hv, opts, pn, pnw, INLINE, classify_columns
+    global hv, opts, pn, pnw, INLINE
     try:
         # Import main modules
         import hvplot.pandas
         import holoviews as hv
         import panel as pn
         from bokeh.resources import INLINE
         from bokeh.util.warnings import BokehUserWarning 
@@ -207,14 +209,15 @@
             drawobj2 = draw_pair_scatters_hv(dfin, nums, problem_type, chart_format, dep,
                            classes, lowess, mk_dir, verbose)
             ls_objects.append(drawobj2)
     drawobj3 = draw_distplot_hv(dfin, cats, nums, chart_format, problem_type, dep, classes, mk_dir, verbose)
     ls_objects.append(drawobj3)
     ### kdeplot is the only time you send in ls_objects since it has to be returned with 2 objects ###
     try:
+        #### This KDE draws only the distribution of the target variable!
         drawobj4 = draw_kdeplot_hv(dfin, cats, nums, chart_format, problem_type, dep, ls_objects, mk_dir, verbose)
         if not drawobj4:
             ### if it is not blank, then treat it as ls_objects ###
             ls_objects = copy.deepcopy(drawobj4)
     except:
         ### This KDE plot errors a lot due to DynamicMaps of holoviews being buggy, so better to skip it!
         print('KDE plot is erroring due to problems with DynamicMaps. Hence it is skipped')
@@ -318,44 +321,47 @@
     imgdata_list = list()
     N = len(nums)
     cols = 2
     plot_name = 'kde_plots'
     width_size = 600
     height_size = 400
     hv_all = None
+    transparent = 0.5
+    color='lightblue'
     ########################################################################################
     def return_dynamic_objects(dfout, dep, title='Distribution of Target variable'):
         width_size = 600
         height_size = 400
         pdf1 = pd.DataFrame(dfout[dep].value_counts().reset_index())
         pdf2 = pd.DataFrame(dfout[dep].value_counts(1).reset_index())
         drawobj41 = pdf1.hvplot(kind='bar', color='lightblue', title=title).opts(
                         height=height_size, width=width_size,xrotation=70)
         drawobj42 = pdf2.hvplot(kind='bar', color='lightgreen', title=title)
         return (drawobj41+drawobj42)
-
+    
     if problem_type.endswith('Classification'):
         colors = cycle('brycgkbyrcmgkbyrcmgkbyrcmgkbyr')
         dmap = hv.DynamicMap(return_dynamic_objects(dfin, dep, title='Percent Distribution of Target variable'
                         ).opts(shared_axes=False).opts(title='Histogram and KDE of Target = %s' %dep)).opts(
                             height=height_size, width=width_size)
         dmap.opts(framewise=True,axiswise=True) ## both must be True for your charts to have dynamically varying axes!
-        hv_all = pn.panel.HoloViews(dmap)#, sizing_mode="stretch_both")
+        hv_all = pn.pane.HoloViews(dmap)#, sizing_mode="stretch_both")
         #ls_objects.append(drawobj41)
         #ls_objects.append(drawobj42)
     else:
         if not isinstance(dep, list):
             ### it means dep is a string ###
             if dep == '':
                 ### there is no target variable to draw ######
                 return ls_objects
             else:
-                dmap = hv.DynamicMap(return_dynamic_objects(dfin, dep, title=f'Histogram and KDE of Target = {dep}')).opts(width=width_size)
-                dmap.opts(framewise=True,axiswise=True) ## both must be True for your charts to have dynamically varying axes!
-                hv_all = pn.panel.HoloViews(dmap)
+                dmap = hv.Distribution(dfin[dep]).opts(color=color,
+                                        height=height_size, width=width_size, alpha=transparent,
+                                    title='KDE (Distribution) Plot of Target Variable')
+                hv_all = pn.pane.HoloViews(dmap)
                 #ls_objects.append(drawobj41)
                 #ls_objects.append(drawobj42)
     #### In this case we are using multiple objects in panel ###
     ##### Save all the chart objects here ##############
     if verbose == 2:
         imgdata_list = append_panels(hv_all, imgdata_list, chart_format)
         image_count += 1
@@ -875,28 +881,30 @@
         else:
             iter_limit = max(number_in_each_row, int(df_p.shape[1]/5+0.5))
         #print('Current number of Numeric Variables = %d ' %(df_p.shape[1],))
         ###### This is for looping over variables 10 at a time only ##########################
         drawobjv_list = [] ## this keeps track of the actual values
         drawobj_list = [] ## this keeps track of the names
         counter = 0
+        string_size = 10
         for i in range(0,df_p.shape[1],iter_limit):
             new_end = i+iter_limit
             #print('i = ',i,"new end = ", new_end)
             if i == 0:
                 title_string = 'using first %d variables...' %(iter_limit)
                 #print(title_string )
             else:
                 title_string = 'using next %d variables...' %(iter_limit)
                 #print(title_string )
             conti = nums[i:new_end]
             ######################### Add Standard Scaling here ##################################
+            short_conti = [x[:string_size] for x in conti]
             from sklearn.preprocessing import StandardScaler
             SS = StandardScaler()
-            data = pd.DataFrame(SS.fit_transform(dft[conti]),columns=conti)
+            data = pd.DataFrame(SS.fit_transform(dft[conti]),columns=short_conti)
             var_name = 'drawobjv_list['+str(counter)+']'
             drawobj_list.append(var_name)
             drawobjv_list.append(var_name)
             drawobj = data.hvplot(kind='violin', label='Violin Plot %s (Standard Scaled)' %title_string,
                                    rot=70  #height=height_size,width=width_size
                                  )
             drawobjv_list[counter] = drawobj
```

### Comparing `autoviz-0.1.806/autoviz/AutoViz_NLP.py` & `autoviz-0.1.807/autoviz/AutoViz_NLP.py`

 * *Files identical despite different names*

### Comparing `autoviz-0.1.806/autoviz/AutoViz_Utils.py` & `autoviz-0.1.807/autoviz/AutoViz_Utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -745,15 +745,15 @@
     dft = dft[:]
     classes = copy.deepcopy(classes)
     colors = cycle('brycgkbyrcmgkbyrcmgkbyrcmgkbyr')
     imgdata_list = list()
     width_size = 15  #### this is to control the width of chart as well as number of categories to display
     height_size = 5
     gap = 0.4 #### This controls the space between rows  ######
-    pdb.set_trace()
+    
     if dep is None or dep=='' or problem_type == 'Regression':
         image_count = 0
         transparent = 0.7
         ######### This is for cases where there is No Target or Dependent Variable ########
         if problem_type == 'Regression':
             if isinstance(dep,list):
                 conti += dep
@@ -1648,25 +1648,28 @@
             dfte = dfte[list(dfte.columns[~dfte.columns.duplicated(keep='first')])]
         return dfte
     else:
         print('Dataname input must be a filename with path to that file or a Dataframe')
         return None
 ##########################################################################################
 import copy
+import pdb
 def classify_print_vars(filename,sep, max_rows_analyzed, max_cols_analyzed,
                         depVar='',dfte=None, header=0,verbose=0):
     corr_limit = 0.7  ### This limit represents correlation above this, vars will be removed
     
     start_time=time.time()
+    
     if filename:
         dataname = copy.deepcopy(filename)
         parse_dates = True
     else:
         dataname = copy.deepcopy(dfte)
         parse_dates = False
+    
     dfte = load_file_dataframe(dataname, sep=sep, header=header, verbose=verbose, 
                     nrows=max_rows_analyzed, parse_dates=parse_dates)
     
     orig_preds = [x for x in list(dfte) if x not in [depVar]]
     #################    CLASSIFY  COLUMNS   HERE    ######################
     if len(dfte) >= 100000:
         dfte_small = dfte.sample(n=10000, random_state=99)
```

### Comparing `autoviz-0.1.806/autoviz/__init__.py` & `autoviz-0.1.807/autoviz/__init__.py`

 * *Files identical despite different names*

### Comparing `autoviz-0.1.806/autoviz/classify_method.py` & `autoviz-0.1.807/autoviz/classify_method.py`

 * *Files identical despite different names*

### Comparing `autoviz-0.1.806/autoviz.egg-info/PKG-INFO` & `autoviz-0.1.807/autoviz.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autoviz
-Version: 0.1.806
+Version: 0.1.807
 Summary: Automatically Visualize any dataset, any size with a single line of code
 Home-page: https://github.com/AutoViML/AutoViz.git
 Author: Ram Seshadri
 License: Apache License 2.0
 Description: # AutoViz: The One-Line Automatic Data Visualization Library
         
         ![logo](images/logo.png)
@@ -37,27 +37,25 @@
         <li><a href="#disclaimer">Disclaimer</a></li>
         </ul>
         
         ## Latest
         The latest updates about `autoviz` library can be found in <a href="https://github.com/AutoViML/AutoViz/blob/master/updates.md">Updates page</a>.
         
         ## ImportantAnnouncement
-        ### Starting with version 0.1.801, an important Update Regarding Dependency Management
-        We're excited to announce a significant update to AutoViz that enhances compatibility with various Python versions and streamlines dependency management!
-        <li>Modular Dependency Loading: AutoViz now uses a more flexible approach for importing visualization libraries starting with version `0.1.801`. This means you only need to install certain dependencies (like hvplot and holoviews) if you plan to use specific backends (e.g., bokeh). This change significantly reduces installation issues for users on newer Python versions such as 3.10 and higher.</li>
-        
-        <li>Improved Backend Support: Depending on your Python environment, AutoViz dynamically adjusts to use compatible visualization libraries, ensuring a smoother user experience. Requirements:
-                "holoviews>=1.14.9",
-                "bokeh>=2.4.2",
-                "hvplot>=0.7.3",
-                "panel>=0.12.6".
-        </li>
+        ### Starting with version 0.1.807, an important update regarding Python Version Management
+        <li>We're excited to announce we've made significant updates to our `setup.py` script to dynamically manage dependencies based on your Python version. This means that when you install AutoViz, the installation process will automatically select versions of dependencies such as HoloViews, Bokeh, and hvPlot that are best suited to your specific Python environment.
+        
+        For `Python versions below 3.10`, AutoViz will use versions of its dependencies known to be stable and compatible with older Python versions.
+        
+        For `Python 3.10`, the script has been configured to use updated dependencies that address specific fixes and enhancements relevant to this version.
+        
+        For `Python 3.11 and newer versions`, setup.py ensures compatibility by selecting library versions that support the latest Python features and fixes, including critical updates made in HoloViews for Python 3.11 support.</li>
         
         ### What Does This Mean for You?
-        <li>Easier Installation: If you've faced challenges installing AutoViz due to dependency conflicts, this update is for you. Now, you can install AutoViz without needing to install all its visualization dependencies upfront.</li>
+        <li><b>Easier Installation</b>: This approach allows AutoViz to leverage the latest advancements in our dependencies while maintaining robust support for older Python versions. The installation process is seamless—simply run pip install . in the AutoViz directory, and the script takes care of the rest, tailoring the installation to your environment.</li>
         
         <li>Tailored Usage: Choose the visualization backend that works best for your environment. AutoViz will handle the rest, importing necessary libraries as needed.</li>
         
         <li>Seamless Compatibility: Users on the latest Python versions (like 3.11 and 3.12) can now enjoy a hassle-free AutoViz experience.</li>
         
         ### How to Update?
         Simply pull the latest version of AutoViz (0.1.801 and higher) from the pip repository. The modular dependency system will be automatically applied.
@@ -97,17 +95,35 @@
         ```sh
         cd <AutoViz_Destination>
         git clone git@github.com:AutoViML/AutoViz.git
         # or download and unzip https://github.com/AutoViML/AutoViz/archive/master.zip
         conda create -n <your_env_name> python=3.7 anaconda
         conda activate <your_env_name> # ON WINDOWS: `source activate <your_env_name>`
         cd AutoViz
+        ```
+        For Python versions below 3.10, install dependencies as follows:
+        
+        ```
         pip install -r requirements.txt
         ```
         
+        For Python 3.10, please use:
+        
+        ```
+        pip install -r requirements-py310.txt
+        ```
+        
+        For Python 3.11 and above, it's recommended to use:
+        
+        ```
+        pip install -r requirements-py311.txt
+        ```
+        
+        These requirement files ensure that AutoViz works seamlessly with your Python environment by installing compatible versions of libraries like HoloViews, Bokeh, and hvPlot. Please select the requirement file that corresponds to your Python version to enjoy a smooth experience with AutoViz.</li>
+        
         ## Usage
         Discover how to use AutoViz in this Medium article.
         
         In the AutoViz directory, open a Jupyter Notebook or open a command palette (terminal) and use the following code to instantiate the AutoViz_Class. You can simply run this code step by step:
         
         ```python
         from autoviz import AutoViz_Class
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: autoviz Version: 0.1.806 Summary: Automatically
+Metadata-Version: 2.1 Name: autoviz Version: 0.1.807 Summary: Automatically
 Visualize any dataset, any size with a single line of code Home-page: https://
 github.com/AutoViML/AutoViz.git Author: Ram Seshadri License: Apache License
 2.0 Description: # AutoViz: The One-Line Automatic Data Visualization Library !
 [logo](images/logo.png) Unlock the power of **AutoViz** to visualize any
 dataset, any size, with just a single line of code! Plus, now you can get a
 quick assessment of your dataset's quality and fix DQ issues through the FixDQ
 () function. [![Pepy Downloads](https://pepy.tech/badge/autoviz)](https://
@@ -28,32 +28,34 @@
     * _E_x_a_m_p_l_e_s_ _o_f_ _u_s_i_n_g_ _A_u_t_o_V_i_z
     * _M_a_i_n_t_a_i_n_e_r_s
     * _C_o_n_t_r_i_b_u_t_i_n_g
     * _L_i_c_e_n_s_e
     * _T_i_p_s_ _f_o_r_ _u_s_i_n_g_ _A_u_t_o_V_i_z
     * _D_i_s_c_l_a_i_m_e_r
 ## Latest The latest updates about `autoviz` library can be found in _U_p_d_a_t_e_s
-_p_a_g_e. ## ImportantAnnouncement ### Starting with version 0.1.801, an important
-Update Regarding Dependency Management We're excited to announce a significant
-update to AutoViz that enhances compatibility with various Python versions and
-streamlines dependency management!
-Modular Dependency Loading: AutoViz now uses a more flexible approach for
-importing visualization libraries starting with version `0.1.801`. This means
-you only need to install certain dependencies (like hvplot and holoviews) if
-you plan to use specific backends (e.g., bokeh). This change significantly
-reduces installation issues for users on newer Python versions such as 3.10 and
-higher.
-Improved Backend Support: Depending on your Python environment, AutoViz
-dynamically adjusts to use compatible visualization libraries, ensuring a
-smoother user experience. Requirements: "holoviews>=1.14.9", "bokeh>=2.4.2",
-"hvplot>=0.7.3", "panel>=0.12.6".
+_p_a_g_e. ## ImportantAnnouncement ### Starting with version 0.1.807, an important
+update regarding Python Version Management
+We're excited to announce we've made significant updates to our `setup.py`
+script to dynamically manage dependencies based on your Python version. This
+means that when you install AutoViz, the installation process will
+automatically select versions of dependencies such as HoloViews, Bokeh, and
+hvPlot that are best suited to your specific Python environment. For `Python
+versions below 3.10`, AutoViz will use versions of its dependencies known to be
+stable and compatible with older Python versions. For `Python 3.10`, the script
+has been configured to use updated dependencies that address specific fixes and
+enhancements relevant to this version. For `Python 3.11 and newer versions`,
+setup.py ensures compatibility by selecting library versions that support the
+latest Python features and fixes, including critical updates made in HoloViews
+for Python 3.11 support.
 ### What Does This Mean for You?
-Easier Installation: If you've faced challenges installing AutoViz due to
-dependency conflicts, this update is for you. Now, you can install AutoViz
-without needing to install all its visualization dependencies upfront.
+EEaassiieerr IInnssttaallllaattiioonn: This approach allows AutoViz to leverage the latest
+advancements in our dependencies while maintaining robust support for older
+Python versions. The installation process is seamlessâsimply run pip install
+. in the AutoViz directory, and the script takes care of the rest, tailoring
+the installation to your environment.
 Tailored Usage: Choose the visualization backend that works best for your
 environment. AutoViz will handle the rest, importing necessary libraries as
 needed.
 Seamless Compatibility: Users on the latest Python versions (like 3.11 and
 3.12) can now enjoy a hassle-free AutoViz experience.
 ### How to Update? Simply pull the latest version of AutoViz (0.1.801 and
 higher) from the pip repository. The modular dependency system will be
@@ -93,107 +95,114 @@
       helps you fix DQ issues with a single line of code using the FixDQ()
       function
 ## Installation **Prerequisites** - [Anaconda](https://docs.anaconda.com/
 anaconda/install/) Create a new environment and install the required
 dependencies to clone AutoViz: **From PyPi:** ```sh cd git clone
 git@github.com:AutoViML/AutoViz.git # or download and unzip https://github.com/
 AutoViML/AutoViz/archive/master.zip conda create -n python=3.7 anaconda conda
-activate # ON WINDOWS: `source activate ` cd AutoViz pip install -
-r requirements.txt ``` ## Usage Discover how to use AutoViz in this Medium
-article. In the AutoViz directory, open a Jupyter Notebook or open a command
-palette (terminal) and use the following code to instantiate the AutoViz_Class.
-You can simply run this code step by step: ```python from autoviz import
-AutoViz_Class AV = AutoViz_Class() dft = AV.AutoViz(filename) ``` AutoViz can
-use any input either filename (in CSV, txt, or JSON format) or a pandas
-dataframe. If you have a large dataset, you can set the `max_rows_analyzed` and
-`max_cols_analyzed` arguments to speed up the visualization by asking autoviz
-to sample your dataset. AutoViz can also create charts in multiple formats
-using the `chart_format` setting: - If `chart_format ='png'` or `'svg'` or
-`'jpg'`: Matplotlib charts are plotted inline. * Can be saved locally (using
-`verbose=2` setting) or displayed (`verbose=1`) in Jupyter Notebooks. * This is
-the default behavior for AutoViz. - If `chart_format='bokeh'`: Interactive
-Bokeh charts are plotted in Jupyter Notebooks. - If `chart_format='server'`,
-dashboards will pop up for each kind of chart on your browser. - If
-`chart_format='html'`, interactive Bokeh charts will be created and silently
-saved as HTML files under the `AutoViz_Plots` directory (under working folder)
-or any other directory that you specify using the `save_plot_dir` setting
-(during input). ## API Arguments for `AV.AutoViz()` method: - `filename`: Use
-an empty string ("") if there's no associated filename and you want to use a
-dataframe. In that case, using the `dfte` argument for the dataframe. Otherwise
-provide a filename and leave `dfte` argument with an empty string. Only one of
-them can be used. - `sep`: File separator (comma, semi-colon, tab, or any
-column-separating value) if you use a filename above. - `depVar`: Target
-variable in your dataset; set it as an empty string if not applicable. -
-`dfte`: name of the pandas dataframe for plotting charts; leave it as empty
-string if using a filename. - `header`: set the row number of the header row in
-your file (0 for the first row). Otherwise leave it as 0. - `verbose`: 0 for
-minimal info and charts, 1 for more info and charts, or 2 for saving charts
-locally without display. - `lowess`: Use regression lines for each pair of
-continuous variables against the target variable in small datasets; avoid using
-for large datasets (>100,000 rows). - `chart_format`: 'svg', 'png', 'jpg',
-'bokeh', 'server', or 'html' for displaying or saving charts in various
-formats, depending on the verbose option. - `max_rows_analyzed`: Limit the max
-number of rows to use for visualization when dealing with very large datasets
-(millions of rows). A statistically valid sample will be used by autoviz.
-Default is 150000 rows. - `max_cols_analyzed`: Limit the number of continuous
-variables to be analyzed. Defaul is 30 columns. - `save_plot_dir`: Directory
-for saving plots. Default is None, which saves plots under the current
-directory in a subfolder named AutoViz_Plots. If the save_plot_dir doesn't
-exist, it will be created. ## Examples Here are some examples to help you get
-started with AutoViz. If you need full jupyter notebooks with code samples they
-can be found in [examples](https://github.com/AutoViML/AutoViz/tree/master/
-Examples) folder. ### Example 1: Visualize a CSV file with a target variable
-```python from autoviz import AutoViz_Class AV = AutoViz_Class() filename =
-"your_file.csv" target_variable = "your_target_variable" dft = AV.AutoViz
-( filename, sep=",", depVar=target_variable, dfte=None, header=0, verbose=1,
-lowess=False, chart_format="svg", max_rows_analyzed=150000,
-max_cols_analyzed=30, save_plot_dir=None ) ``` ![var_charts](images/
-var_charts.JPG) ### Example 2: Visualize a Pandas DataFrame without a target
-variable: ```python import pandas as pd from autoviz import AutoViz_Class AV =
-AutoViz_Class() data = {'col1': [1, 2, 3, 4, 5], 'col2': [5, 4, 3, 2, 1]} df =
-pd.DataFrame(data) dft = AV.AutoViz( "", sep=",", depVar="", dfte=df, header=0,
-verbose=1, lowess=False, chart_format="server", max_rows_analyzed=150000,
-max_cols_analyzed=30, save_plot_dir=None ) ``` ![server_charts](images/
-server_charts.JPG) ### Example 3: Generate interactive Bokeh charts and save
-them as HTML files in a custom directory ```python from autoviz import
+activate # ON WINDOWS: `source activate ` cd AutoViz ``` For Python versions
+below 3.10, install dependencies as follows: ``` pip install -
+r requirements.txt ``` For Python 3.10, please use: ``` pip install -
+r requirements-py310.txt ``` For Python 3.11 and above, it's recommended to
+use: ``` pip install -r requirements-py311.txt ``` These requirement files
+ensure that AutoViz works seamlessly with your Python environment by installing
+compatible versions of libraries like HoloViews, Bokeh, and hvPlot. Please
+select the requirement file that corresponds to your Python version to enjoy a
+smooth experience with AutoViz.
+## Usage Discover how to use AutoViz in this Medium article. In the AutoViz
+directory, open a Jupyter Notebook or open a command palette (terminal) and use
+the following code to instantiate the AutoViz_Class. You can simply run this
+code step by step: ```python from autoviz import AutoViz_Class AV =
+AutoViz_Class() dft = AV.AutoViz(filename) ``` AutoViz can use any input either
+filename (in CSV, txt, or JSON format) or a pandas dataframe. If you have a
+large dataset, you can set the `max_rows_analyzed` and `max_cols_analyzed`
+arguments to speed up the visualization by asking autoviz to sample your
+dataset. AutoViz can also create charts in multiple formats using the
+`chart_format` setting: - If `chart_format ='png'` or `'svg'` or `'jpg'`:
+Matplotlib charts are plotted inline. * Can be saved locally (using `verbose=2`
+setting) or displayed (`verbose=1`) in Jupyter Notebooks. * This is the default
+behavior for AutoViz. - If `chart_format='bokeh'`: Interactive Bokeh charts are
+plotted in Jupyter Notebooks. - If `chart_format='server'`, dashboards will pop
+up for each kind of chart on your browser. - If `chart_format='html'`,
+interactive Bokeh charts will be created and silently saved as HTML files under
+the `AutoViz_Plots` directory (under working folder) or any other directory
+that you specify using the `save_plot_dir` setting (during input). ## API
+Arguments for `AV.AutoViz()` method: - `filename`: Use an empty string ("") if
+there's no associated filename and you want to use a dataframe. In that case,
+using the `dfte` argument for the dataframe. Otherwise provide a filename and
+leave `dfte` argument with an empty string. Only one of them can be used. -
+`sep`: File separator (comma, semi-colon, tab, or any column-separating value)
+if you use a filename above. - `depVar`: Target variable in your dataset; set
+it as an empty string if not applicable. - `dfte`: name of the pandas dataframe
+for plotting charts; leave it as empty string if using a filename. - `header`:
+set the row number of the header row in your file (0 for the first row).
+Otherwise leave it as 0. - `verbose`: 0 for minimal info and charts, 1 for more
+info and charts, or 2 for saving charts locally without display. - `lowess`:
+Use regression lines for each pair of continuous variables against the target
+variable in small datasets; avoid using for large datasets (>100,000 rows). -
+`chart_format`: 'svg', 'png', 'jpg', 'bokeh', 'server', or 'html' for
+displaying or saving charts in various formats, depending on the verbose
+option. - `max_rows_analyzed`: Limit the max number of rows to use for
+visualization when dealing with very large datasets (millions of rows). A
+statistically valid sample will be used by autoviz. Default is 150000 rows. -
+`max_cols_analyzed`: Limit the number of continuous variables to be analyzed.
+Defaul is 30 columns. - `save_plot_dir`: Directory for saving plots. Default is
+None, which saves plots under the current directory in a subfolder named
+AutoViz_Plots. If the save_plot_dir doesn't exist, it will be created. ##
+Examples Here are some examples to help you get started with AutoViz. If you
+need full jupyter notebooks with code samples they can be found in [examples]
+(https://github.com/AutoViML/AutoViz/tree/master/Examples) folder. ### Example
+1: Visualize a CSV file with a target variable ```python from autoviz import
 AutoViz_Class AV = AutoViz_Class() filename = "your_file.csv" target_variable =
-"your_target_variable" custom_plot_dir = "your_custom_plot_directory" dft =
-AV.AutoViz( filename, sep=",", depVar=target_variable, dfte=None, header=0,
-verbose=2, lowess=False, chart_format="bokeh", max_rows_analyzed=150000,
-max_cols_analyzed=30, save_plot_dir=custom_plot_dir ) ``` ![bokeh_charts]
-(images/bokeh_charts.JPG) These examples should give you an idea of how to use
-AutoViz with different scenarios and settings. By tailoring the options and
-settings, you can generate visualizations that best suit your needs, whether
-you're working with large datasets, interactive charts, or simply exploring the
-relationships between variables. ## Maintainers AutoViz is actively maintained
-and improved by a team of dedicated developers. If you have any questions,
-suggestions, or issues, feel free to reach out to the maintainers: -
-[@AutoViML](https://github.com/AutoViML) - [@morenoh149](https://github.com/
-morenoh149) - [@hironroy](https://github.com/hironroy) ## Contributing We
-welcome contributions from the community! If you're interested in contributing
-to AutoViz, please follow these steps: - Fork the repository on GitHub. - Clone
-your fork and create a new branch for your feature or bugfix. - Commit your
-changes to the new branch, ensuring that you follow coding standards and write
-appropriate tests. - Push your changes to your fork on GitHub. - Submit a pull
-request to the main repository, detailing your changes and referencing any
-related issues. See [the contributing file](contributing.md)! ## License
-AutoViz is released under the Apache License, Version 2.0. By using AutoViz,
-you agree to the terms and conditions specified in the license. ## Tips Here
-are some additional tips and reminders to help you make the most of the
-library: - **Make sure to regularly upgrade AutoViz** to benefit from the
-latest features, bug fixes, and improvements. You can update it using pip
-install --upgrade autoviz. - **AutoViz is highly customizable, so don't
-hesitate to explore and experiment with various settings**, such as
-chart_format, verbose, and max_rows_analyzed. This will allow you to create
-visualizations that better suit your specific needs and preferences. -
-**Remember to delete the AutoViz_Plots directory (or any custom directory you
-specified) periodically** if you used the verbose=2 option, as it can
-accumulate a large number of saved charts over time. - **For further guidance
-or inspiration, check out the _M_e_d_i_u_m_ _a_r_t_i_c_l_e on AutoViz**, as well as other
-online resources and tutorials.
+"your_target_variable" dft = AV.AutoViz( filename, sep=",",
+depVar=target_variable, dfte=None, header=0, verbose=1, lowess=False,
+chart_format="svg", max_rows_analyzed=150000, max_cols_analyzed=30,
+save_plot_dir=None ) ``` ![var_charts](images/var_charts.JPG) ### Example 2:
+Visualize a Pandas DataFrame without a target variable: ```python import pandas
+as pd from autoviz import AutoViz_Class AV = AutoViz_Class() data = {'col1':
+[1, 2, 3, 4, 5], 'col2': [5, 4, 3, 2, 1]} df = pd.DataFrame(data) dft =
+AV.AutoViz( "", sep=",", depVar="", dfte=df, header=0, verbose=1, lowess=False,
+chart_format="server", max_rows_analyzed=150000, max_cols_analyzed=30,
+save_plot_dir=None ) ``` ![server_charts](images/server_charts.JPG) ### Example
+3: Generate interactive Bokeh charts and save them as HTML files in a custom
+directory ```python from autoviz import AutoViz_Class AV = AutoViz_Class()
+filename = "your_file.csv" target_variable = "your_target_variable"
+custom_plot_dir = "your_custom_plot_directory" dft = AV.AutoViz( filename,
+sep=",", depVar=target_variable, dfte=None, header=0, verbose=2, lowess=False,
+chart_format="bokeh", max_rows_analyzed=150000, max_cols_analyzed=30,
+save_plot_dir=custom_plot_dir ) ``` ![bokeh_charts](images/bokeh_charts.JPG)
+These examples should give you an idea of how to use AutoViz with different
+scenarios and settings. By tailoring the options and settings, you can generate
+visualizations that best suit your needs, whether you're working with large
+datasets, interactive charts, or simply exploring the relationships between
+variables. ## Maintainers AutoViz is actively maintained and improved by a team
+of dedicated developers. If you have any questions, suggestions, or issues,
+feel free to reach out to the maintainers: - [@AutoViML](https://github.com/
+AutoViML) - [@morenoh149](https://github.com/morenoh149) - [@hironroy](https://
+github.com/hironroy) ## Contributing We welcome contributions from the
+community! If you're interested in contributing to AutoViz, please follow these
+steps: - Fork the repository on GitHub. - Clone your fork and create a new
+branch for your feature or bugfix. - Commit your changes to the new branch,
+ensuring that you follow coding standards and write appropriate tests. - Push
+your changes to your fork on GitHub. - Submit a pull request to the main
+repository, detailing your changes and referencing any related issues. See [the
+contributing file](contributing.md)! ## License AutoViz is released under the
+Apache License, Version 2.0. By using AutoViz, you agree to the terms and
+conditions specified in the license. ## Tips Here are some additional tips and
+reminders to help you make the most of the library: - **Make sure to regularly
+upgrade AutoViz** to benefit from the latest features, bug fixes, and
+improvements. You can update it using pip install --upgrade autoviz. -
+**AutoViz is highly customizable, so don't hesitate to explore and experiment
+with various settings**, such as chart_format, verbose, and max_rows_analyzed.
+This will allow you to create visualizations that better suit your specific
+needs and preferences. - **Remember to delete the AutoViz_Plots directory (or
+any custom directory you specified) periodically** if you used the verbose=2
+option, as it can accumulate a large number of saved charts over time. - **For
+further guidance or inspiration, check out the _M_e_d_i_u_m_ _a_r_t_i_c_l_e on AutoViz**, as
+well as other online resources and tutorials.
     * AutoViz will visualize any sized file using a statistically valid sample.
     * COMMA is the default separator in the file, but you can change it.
     * Assumes the first row as the header in the file, but this can be changed.
 - **By leveraging AutoViz's powerful and flexible features**, you can
 streamline your data visualization process and gain valuable insights more
 efficiently. Happy visualizing! ## DISCLAIMER This project is not an official
 Google project. It is not supported by Google, and Google specifically
```

