# Comparing `tmp/AutoEis-0.0.8.tar.gz` & `tmp/AutoEis-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "D:\Personal Document\Studying in Canada\UOT-courses\Beta_AutoEis\dist\.tmp-8id36hxb\AutoEis-0.0.8.tar", last modified: Fri Apr 28 21:04:36 2023, max compression
+gzip compressed data, was "D:\Personal Document\Studying in Canada\UOT-courses\Beta_AutoEis\dist\.tmp-n3ge8uvk\AutoEis-0.0.9.tar", last modified: Mon May  1 20:44:34 2023, max compression
```

## Comparing `AutoEis-0.0.8.tar` & `AutoEis-0.0.9.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-04-28 21:04:36.163001 AutoEis-0.0.8/
-drwxrwxrwx   0        0        0        0 2023-04-28 21:04:36.138842 AutoEis-0.0.8/AutoEis/
--rw-rw-rw-   0        0        0    72648 2023-04-28 20:58:38.000000 AutoEis-0.0.8/AutoEis/AutoEIS.py
--rw-rw-rw-   0        0        0      289 2023-04-28 21:04:01.000000 AutoEis-0.0.8/AutoEis/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-28 21:04:36.157853 AutoEis-0.0.8/AutoEis.egg-info/
--rw-rw-rw-   0        0        0      645 2023-04-28 21:04:36.000000 AutoEis-0.0.8/AutoEis.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      234 2023-04-28 21:04:36.000000 AutoEis-0.0.8/AutoEis.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-28 21:04:36.000000 AutoEis-0.0.8/AutoEis.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      157 2023-04-28 21:04:36.000000 AutoEis-0.0.8/AutoEis.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-04-28 21:04:36.000000 AutoEis-0.0.8/AutoEis.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        0 2023-04-28 19:52:59.000000 AutoEis-0.0.8/LICENSE
--rw-rw-rw-   0        0        0      645 2023-04-28 21:04:36.161982 AutoEis-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0       13 2022-07-21 02:14:53.000000 AutoEis-0.0.8/README.md
--rw-rw-rw-   0        0        0       86 2023-04-28 20:17:09.000000 AutoEis-0.0.8/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-28 21:04:36.163001 AutoEis-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0     1717 2023-04-28 21:03:26.000000 AutoEis-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-01 20:44:34.474461 AutoEis-0.0.9/
+drwxrwxrwx   0        0        0        0 2023-05-01 20:44:34.435459 AutoEis-0.0.9/AutoEis/
+-rw-rw-rw-   0        0        0    78583 2023-05-01 20:41:35.000000 AutoEis-0.0.9/AutoEis/AutoEIS.py
+-rw-rw-rw-   0        0        0      289 2023-05-01 20:41:59.000000 AutoEis-0.0.9/AutoEis/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-01 20:44:34.466476 AutoEis-0.0.9/AutoEis.egg-info/
+-rw-rw-rw-   0        0        0      645 2023-05-01 20:44:34.000000 AutoEis-0.0.9/AutoEis.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      234 2023-05-01 20:44:34.000000 AutoEis-0.0.9/AutoEis.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-01 20:44:34.000000 AutoEis-0.0.9/AutoEis.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      157 2023-05-01 20:44:34.000000 AutoEis-0.0.9/AutoEis.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-05-01 20:44:34.000000 AutoEis-0.0.9/AutoEis.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        0 2023-04-28 19:52:59.000000 AutoEis-0.0.9/LICENSE
+-rw-rw-rw-   0        0        0      645 2023-05-01 20:44:34.471461 AutoEis-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0       13 2022-07-21 02:14:53.000000 AutoEis-0.0.9/README.md
+-rw-rw-rw-   0        0        0       86 2023-04-28 20:17:09.000000 AutoEis-0.0.9/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-01 20:44:34.474461 AutoEis-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0     1717 2023-05-01 20:42:26.000000 AutoEis-0.0.9/setup.py
```

### Comparing `AutoEis-0.0.8/AutoEis/AutoEIS.py` & `AutoEis-0.0.9/AutoEis/AutoEIS.py`

 * *Files 7% similar despite different names*

```diff
@@ -22,59 +22,88 @@
 
     # the packages for bayesian inference
     import arviz as az
     import numpyro
     from numpyro.diagnostics import hpdi
     import numpyro.distributions as dist
     from numpyro import handlers
-    from numpyro.infer import MCMC, NUTS,HMC,HMCECS,BarkerMH,HMCGibbs,DiscreteHMCGibbs
+    from numpyro.infer import MCMC, NUTS, HMC, HMCECS, BarkerMH, HMCGibbs, DiscreteHMCGibbs
     from numpyro.infer import Predictive
-    from numpyro.infer.util import log_likelihood,log_density
+    from numpyro.infer.util import log_likelihood, log_density
 
     from IPython.display import set_matplotlib_formats
     import jax.numpy as jnp
     from jax import random, vmap
     from jax.scipy.special import logsumexp
     import jax
 
     # the package for storage
     import dill
 
     # the package for ignoring warnings
     import warnings
-    warnings.filterwarnings('ignore') # ignore the warnings
+
+    warnings.filterwarnings('ignore')  # ignore the warnings
 
     # the packages for calling julia file/function in python
     from julia import Julia
 
 except ImportError:
     import pip
-    pip.main(["install","--user","matplotlib","numpy","json","pandas","impedance","arviz","numpyro","jax","dill","julia"])
 
+    pip.main(
+        ["install", "--user", "matplotlib", "numpy", "json", "pandas", "impedance", "arviz", "numpyro", "jax", "dill",
+         "julia"])
 
-def set_julia(julia_executable_path: 'str') -> 'Julia object':
 
+def set_julia(julia_executable_path: 'str') -> 'Julia object':
     """Set the julia environment in python
 
         Parameter
         ---------
         julia_executable_path:str
             path of julia executable file (julia.exe) in your computer
 
     """
     # define the path of julia program
-    julia_path = r"D:\Julia-1.7.2\bin\julia.exe"  # path of julia executable file (julia.exe)
-
+    julia_path = julia_executable_path  # path of julia executable file (julia.exe)
     j = Julia(runtime=julia_path)
     return j
 
 
+def initialize_julia():
+    # import julia's basic packages via PyCall
+    from julia import Pkg
+    from julia import Base
+    # install the required packages
+    Base.ENV["PYTHON"] = sys.executable
+    Pkg.build("PyCall")
+    Pkg.add("EquivalentCircuits")
+    Pkg.add("DelimitedFiles")
+    Pkg.add("StringEncodings")
+    Pkg.add('Pandas')
+    Pkg.add('DataFrames')
+    pass
+
+
+def import_julia():
+
+    """Install the julia's dependencies"""
+
+    from julia import Pkg
+    from julia import Base
+    from julia import EquivalentCircuits as ec
+    from julia import DelimitedFiles
+    from julia import StringEncodings
+    from julia import Pandas
+    from julia import DataFrames
+    return ec,DataFrames,Pandas,Base
 
-def set_parameter():
 
+def set_parameter():
     """Set the parameters of figures"""
 
     # set the parameters for plots
     plt.rcParams['figure.figsize'] = (19.6, 10.8)
 
     # set the parameters for plots
     az.style.use("arviz-darkgrid")
@@ -94,14 +123,15 @@
 
 
 
 def reset_storage():
 
     """Reset the working path as the original data path (Please run me when you encountered file loading error)
     """
+
     for i in range(2):
         os.chdir(os.path.abspath(os.path.dirname(os.getcwd())))
     pass
 
 
 
 def load_data(data_path: 'str') -> 'pd.DataFrame':
@@ -435,15 +465,14 @@
 
     if len(Zdf_mask) / len(Z) <= 0.6:
         print(
             'Warning: the KK validation dropped too many information. Please consider to increase the threshold a little bit.')
     return Zdf_mask, ohmic_resistance, RMSE_value
 
 
-
 def save_processed_data(input_name: 'string', data_stored: 'pd.DataFrame') -> 'string':
     """ Store the processed EIS data in a .csv file
 
         Parameters:
         -----------
         input_name: str
             the data path of the given EIS data
@@ -474,14 +503,55 @@
         file_name = input_name.split(".pkl")[0]
     data_stored.to_csv(folder_name + '//' + folder_name + '_processed' + ".csv", header=None, index=False)
 
     data_stored.to_csv('temp' + ".csv", header=None, index=False)
     return file_name + ".csv"
 
 
+def ECM_generation(processed_data: 'pd.DataFrame', times: 'int' = 100, head: 'int' = 12, save: 'bool' = True):
+    """Generate ECMs via evolutionary algorithms
+
+        Parameters:
+        ------------
+        processed_data:pd.DataFrame
+            the processed data after KK validation
+
+        times:int
+            the number of times the ECM generation process is performed (default = 100)
+
+        head:int
+            the complexity of ECM search space (default = 12)
+
+        save:bool
+            determine to save the results file or not
+
+        Return:
+        ------------
+         df_results:pd.DataFrame
+            the dataframe that stores ECM solutions generated by the evolutionar algorithm
+    """
+    ec, jl_df, jl_pd, jl_Base = import_julia()
+
+    ECM_solution = []
+    for i in range(times):
+        circuit_i = ec.circuit_evolution(np.array(processed_data['Zreal']) + 1j * np.array(processed_data['Zimag']),
+                                         np.array(processed_data['freq']), head=head, terminals="RLP")
+        if circuit_i != jl_Base.nothing:
+            ECM_solution.append(circuit_i)
+    df_results = jl_pd.DataFrame(jl_df.DataFrame(ECM_solution))
+    if len(df_results) == 0:
+        print('Warning: No plausible ECM is found. Please consider to enlarge the search space.')
+        return
+    for i in range(len(df_results)):
+        df_results['Parameters'][i] = jl_Base.string(df_results['Parameters'][i])
+    if save:
+        df_results.to_csv('df_circuits.csv', index=False)
+    return df_results
+
+
 def load_results(file_path: 'string') -> 'pd.DataFrame':
     """ load the ECMs results generated by the julia program and convert it to pd.DataFrame
 
         Parameters:
         -----------
         file_path: str
             the file path of ECMs results
@@ -1513,16 +1583,45 @@
 
     error_term = abs(y_true - y_pred)
     absolute_error_percentage = error_term / abs(y_true)
     mean_absolute_error_percentage = (100 / len(y_true)) * sum(absolute_error_percentage)
     return mean_absolute_error_percentage
 
 
+def convert_text(text: 'string'):
+    """ Visualize circuit string (convert the string of ECMs to figures)
+
+        Parameter:
+        ----------
+        text:str
+            a circuit string of ECM
+
+        Returns
+        ---------
+        circuit_figure:lcapy.figure
+            a figure that represent the given ECM
+
+    """
+
+    from lcapy import R, C, L
+    from lcapy import CPE as P
+    # replace square brackets with parentheses
+    text = text.replace('[', '(').replace(']', ')')
+    # replace commas with vertical bars
+    text = text.replace(',', '|')
+    # replace dashes with plus signs
+    text = text.replace('-', '+')
+    # surround all numbers with parentheses
+    text = re.sub(r'([A-Z])(\d+)', r'\1("\1\2")', text)
+    circuit_figure = eval(text).draw(style='american')
+    return circuit_figure
+
+
 def Bayesian_inference(data: 'pd.DataFrame', df: 'pd.DataFrame', data_path: 'string', plot: 'bool' = True,
-                       save: 'bool' = True) -> 'pd.DataFrame':
+                       save: 'bool' = True, ECM_figure=False) -> 'pd.DataFrame':
     """ Doing the bayesian inference of each circuit
 
         Parameters:
         -----------
         data: pd.DataFrame
             the dataframe that stores data after pre-processing (3 column expected)
             column 1: frequency
@@ -1611,16 +1710,23 @@
         name_i = names[i]
         expression_str_i = expressions_strs[i].replace("np.", "jnp.")
         function_i = eval(f"lambda X,F:{expression_str_i}")
 
         # create a new folder to store these results
         mkdir(folder_name + f'\\{circuit_name_i}')
         os.chdir(folder_name + f'\\{circuit_name_i}')
+
         print(f"Circuit {i}:{circuit_name_i} composed of components ({name_i}) with values ({value_i})")
 
+        if plot:
+            if ECM_figure:
+                convert_text(circuit_name_i)
+                if save:
+                    plt.savefig(f'Equivalent circuit model.png', dpi=300);
+
         ECM_data = function_i(value_i, freq)
         ECMs_data.append(ECM_data)
 
         print("Julia circuit's fitting")
 
         r2_value = float(r2_calculator(Zreal + 1j * Zimag, ECM_data))
         print(f"r2_value:{r2_value}")
@@ -1908,45 +2014,113 @@
     #             json.dum`bp(df_dict,file_obj)
     # load data:
     # with open('file.pkl', 'rb') as f:
     #     input_dict = dill.load(f)
     return df
 
 
-def ECMs_fitting(impedance: 'np.array', freq: 'np.array', data_path: 'string') -> 'pd.DataFrame':
+def EIS_auto(impedance: 'np.array', freq: 'np.array', data_path: 'string', iter_number: 'int' = 100) -> 'pd.DataFrame':
     """ The main function to automate whole EIS analysis by ECMs+ BI
 
         Parameters:
         -----------
         impedance: np.array
             the impedance data
 
         freq: np.array
             the frequencies of the impedance data
 
         data_path: str
             the data path of the impedance data
 
+        iter_number:int
+            the number of times the ECM generation is performed
+
         Return:
         -------
         results: pd.DataFrame
             the dataframe that stored effective ECMs after filtering and corresponding BI results (12 columns)
     """
 
+    # set the plotting style
+    set_parameter()
+    ec, jl_df, jl_pd, jl_Base = import_julia()
+
     # preprocessing + store preprocessed data
-    data_processed, ohmic_resistance = pre_processing(impedance, freq, 0.05, data_path)
+    print('Data_processing')
+    data_processed, ohmic_resistance, RMSE = pre_processing(impedance, freq, 0.05, data_path)
     path_data_preprocessed = save_processed_data(input_name=data_path, data_stored=data_processed)
 
     # call julia program
-    run_julia = j.include('test_julia.jl')
+    print('ECM generation in process')
+    df_results = ECM_generation(processed_data=data_processed, times=iter_number)
+    # an alternative method: direcly call julia script - this might be faster
+    # run_julia = j.include('test_julia.jl')
+
+    # load the results - 1.from the results file
+    # path_results = "df_results.csv"
+    # df_circuits = load_results(file_path = path_results)
 
     # load the results
+    df_circuits = split_components(df_results)
+    df_circuits = capacitance_filter(df_circuits)
+    df_circuits = series_filter(df_circuits)
+    df_circuits = ohmic_resistance_filter(df_circuits, ohmic_resistance)
+    df_circuits = generate_mathematical_expression(df_circuits)
+    new_df = combine_expression(df_circuits)
+    new_df = calculate_length(new_df)
+    new_df = split_variables(new_df)
+    results = Bayesian_inference(data=data_processed, data_path=data_path, df=new_df)
+    return results
+
+
+def EIS_auto_script(impedance: 'np.array', freq: 'np.array', data_path: 'string',
+                    iter_number: 'int' = 100) -> 'pd.DataFrame':
+    """ The main function to automate whole EIS analysis by ECMs+ BI
+
+        Parameters:
+        -----------
+        impedance: np.array
+            the impedance data
+
+        freq: np.array
+            the frequencies of the impedance data
+
+        data_path: str
+            the data path of the impedance data
+
+        iter_number:int
+            the number of times the ECM generation is performed
+
+        Return:
+        -------
+        results: pd.DataFrame
+            the dataframe that stored effective ECMs after filtering and corresponding BI results (12 columns)
+    """
+
+    # set the plotting style
+    set_parameter()
+    ec, jl_df, jl_pd, jl_Base = import_julia()
+
+    # preprocessing + store preprocessed data
+    print('Data_processing')
+    data_processed, ohmic_resistance, RMSE = pre_processing(impedance, freq, 0.05, data_path)
+    path_data_preprocessed = save_processed_data(input_name=data_path, data_stored=data_processed)
+
+    # ECM generation
+    print('ECM generation in process')
+    # an alternative method: direcly call julia script - this might be faster
+    run_julia = j.include('test_julia.jl')
+
+    # load the results - 1.from the results file
     path_results = "df_results.csv"
     df_circuits = load_results(file_path=path_results)
-    df_circuits = split_components(df_circuits)
+
+    # load the results
+    df_circuits = split_components(df_results)
     df_circuits = capacitance_filter(df_circuits)
     df_circuits = series_filter(df_circuits)
     df_circuits = ohmic_resistance_filter(df_circuits, ohmic_resistance)
     df_circuits = generate_mathematical_expression(df_circuits)
     new_df = combine_expression(df_circuits)
     new_df = calculate_length(new_df)
     new_df = split_variables(new_df)
```

### Comparing `AutoEis-0.0.8/AutoEis.egg-info/PKG-INFO` & `AutoEis-0.0.9/AutoEis.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AutoEis
-Version: 0.0.8
+Version: 0.0.9
 Summary: A demo package to assist EIS analysis by automatically proposing statistically plausible ECM
 Home-page: 
 Author: Runze zhang, Robert Black, Jason Hattrick-Simpers*
 Author-email: runzee.zhang@mail.utoronto.ca
 Keywords: Electrochemical impedance spectroscopy,equivalent circuit models,Bayesian inference,evolutionary algorithm
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `AutoEis-0.0.8/PKG-INFO` & `AutoEis-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AutoEis
-Version: 0.0.8
+Version: 0.0.9
 Summary: A demo package to assist EIS analysis by automatically proposing statistically plausible ECM
 Home-page: 
 Author: Runze zhang, Robert Black, Jason Hattrick-Simpers*
 Author-email: runzee.zhang@mail.utoronto.ca
 Keywords: Electrochemical impedance spectroscopy,equivalent circuit models,Bayesian inference,evolutionary algorithm
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `AutoEis-0.0.8/setup.py` & `AutoEis-0.0.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.0.8'
+VERSION = '0.0.9'
 DESCRIPTION = 'A demo package to assist EIS analysis by automatically proposing statistically plausible ECM'
 LONG_DESCRIPTION = 'AutoEIS is a novel tool designed to aid EIS analysis by automatically prioritizing statistically optimal ECM by combining evolutionary algorithms and Bayesian inference.'
 
 # Setting up
 setup(
     name="AutoEis",
     version= VERSION,
```

