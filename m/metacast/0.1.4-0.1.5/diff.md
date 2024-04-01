# Comparing `tmp/metacast-0.1.4.tar.gz` & `tmp/metacast-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metacast-0.1.4.tar", last modified: Wed Mar 13 17:32:20 2024, max compression
+gzip compressed data, was "metacast-0.1.5.tar", last modified: Mon Apr  1 15:32:14 2024, max compression
```

## Comparing `metacast-0.1.4.tar` & `metacast-0.1.5.tar`

### file list

```diff
@@ -1,25 +1,31 @@
-drwxrwxrwx   0        0        0        0 2024-03-13 17:32:20.789810 metacast-0.1.4/
--rw-rw-rw-   0        0        0    11558 2024-02-06 18:05:16.000000 metacast-0.1.4/LICENSE
--rw-rw-rw-   0        0        0    16758 2024-03-13 17:32:20.789810 metacast-0.1.4/PKG-INFO
--rw-rw-rw-   0        0        0     2102 2024-03-12 15:46:36.000000 metacast-0.1.4/README.md
--rw-rw-rw-   0        0        0     1727 2024-03-13 17:29:33.000000 metacast-0.1.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-03-13 17:32:20.789810 metacast-0.1.4/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-03-13 17:32:20.733851 metacast-0.1.4/src/
-drwxrwxrwx   0        0        0        0 2024-03-13 17:32:20.741892 metacast-0.1.4/src/metacast/
--rw-rw-rw-   0        0        0      182 2024-03-08 19:04:18.000000 metacast-0.1.4/src/metacast/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-13 17:32:20.773857 metacast-0.1.4/src/metacast/event_handling/
--rw-rw-rw-   0        0        0      294 2024-03-07 21:04:00.000000 metacast-0.1.4/src/metacast/event_handling/__init__.py
--rw-rw-rw-   0        0        0    19545 2024-03-08 20:02:15.000000 metacast-0.1.4/src/metacast/event_handling/event_que.py
--rw-rw-rw-   0        0        0    16658 2024-03-08 20:02:15.000000 metacast-0.1.4/src/metacast/event_handling/events.py
--rw-rw-rw-   0        0        0     8574 2024-03-08 20:02:15.000000 metacast-0.1.4/src/metacast/infection_seeding.py
--rw-rw-rw-   0        0        0    56629 2024-03-12 20:03:28.000000 metacast-0.1.4/src/metacast/metacaster.py
-drwxrwxrwx   0        0        0        0 2024-03-13 17:32:20.788707 metacast-0.1.4/src/metacast/sensitivity_analyses/
--rw-rw-rw-   0        0        0      205 2024-03-06 21:30:12.000000 metacast-0.1.4/src/metacast/sensitivity_analyses/__init__.py
--rw-rw-rw-   0        0        0     7589 2024-03-08 19:12:55.000000 metacast-0.1.4/src/metacast/sensitivity_analyses/asses_lh_sample_size.py
--rw-rw-rw-   0        0        0    10834 2024-03-13 15:18:48.000000 metacast-0.1.4/src/metacast/sensitivity_analyses/lhs_and_prcc.py
-drwxrwxrwx   0        0        0        0 2024-03-13 17:32:20.789810 metacast-0.1.4/src/metacast.egg-info/
--rw-rw-rw-   0        0        0    16758 2024-03-13 17:32:20.000000 metacast-0.1.4/src/metacast.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      570 2024-03-13 17:32:20.000000 metacast-0.1.4/src/metacast.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-13 17:32:20.000000 metacast-0.1.4/src/metacast.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      152 2024-03-13 17:32:20.000000 metacast-0.1.4/src/metacast.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-03-13 17:32:20.000000 metacast-0.1.4/src/metacast.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-01 15:32:14.562534 metacast-0.1.5/
+-rw-rw-rw-   0        0        0    11558 2024-02-06 18:05:16.000000 metacast-0.1.5/LICENSE
+-rw-rw-rw-   0        0        0    16780 2024-04-01 15:32:14.562534 metacast-0.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0     2124 2024-03-20 13:05:30.000000 metacast-0.1.5/README.md
+-rw-rw-rw-   0        0        0     1727 2024-04-01 15:21:48.000000 metacast-0.1.5/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-01 15:32:14.562534 metacast-0.1.5/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-01 15:32:14.467898 metacast-0.1.5/src/
+-rw-rw-rw-   0        0        0       93 2024-03-09 15:41:48.000000 metacast-0.1.5/src/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-01 15:32:14.477881 metacast-0.1.5/src/metacast/
+-rw-rw-rw-   0        0        0      182 2024-03-08 19:04:18.000000 metacast-0.1.5/src/metacast/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-01 15:32:14.514810 metacast-0.1.5/src/metacast/event_handling/
+-rw-rw-rw-   0        0        0      294 2024-03-22 15:45:05.000000 metacast-0.1.5/src/metacast/event_handling/__init__.py
+-rw-rw-rw-   0        0        0    19539 2024-03-22 16:18:53.000000 metacast-0.1.5/src/metacast/event_handling/event_que.py
+-rw-rw-rw-   0        0        0    16504 2024-03-22 16:18:53.000000 metacast-0.1.5/src/metacast/event_handling/events.py
+-rw-rw-rw-   0        0        0     8665 2024-03-30 20:17:49.000000 metacast-0.1.5/src/metacast/infection_seeding.py
+-rw-rw-rw-   0        0        0    58134 2024-03-30 20:14:06.000000 metacast-0.1.5/src/metacast/metacaster.py
+drwxrwxrwx   0        0        0        0 2024-04-01 15:32:14.531575 metacast-0.1.5/src/metacast/sensitivity_analyses/
+-rw-rw-rw-   0        0        0      205 2024-03-06 21:30:12.000000 metacast-0.1.5/src/metacast/sensitivity_analyses/__init__.py
+-rw-rw-rw-   0        0        0     7589 2024-03-08 19:12:55.000000 metacast-0.1.5/src/metacast/sensitivity_analyses/asses_lh_sample_size.py
+-rw-rw-rw-   0        0        0    10834 2024-03-13 15:18:48.000000 metacast-0.1.5/src/metacast/sensitivity_analyses/lhs_and_prcc.py
+drwxrwxrwx   0        0        0        0 2024-04-01 15:32:14.558020 metacast-0.1.5/src/metacast.egg-info/
+-rw-rw-rw-   0        0        0    16780 2024-04-01 15:32:14.000000 metacast-0.1.5/src/metacast.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      694 2024-04-01 15:32:14.000000 metacast-0.1.5/src/metacast.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-01 15:32:14.000000 metacast-0.1.5/src/metacast.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      152 2024-04-01 15:32:14.000000 metacast-0.1.5/src/metacast.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2024-04-01 15:32:14.000000 metacast-0.1.5/src/metacast.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-01 15:32:14.558020 metacast-0.1.5/tests/
+-rw-rw-rw-   0        0        0    13638 2024-03-30 21:34:47.000000 metacast-0.1.5/tests/test_event_que.py
+-rw-rw-rw-   0        0        0     2138 2024-03-21 20:21:54.000000 metacast-0.1.5/tests/test_infection_seeding.py
+-rw-rw-rw-   0        0        0     4152 2024-03-30 21:29:33.000000 metacast-0.1.5/tests/test_lhs_and_prcc.py
+-rw-rw-rw-   0        0        0     5489 2024-03-30 21:09:46.000000 metacast-0.1.5/tests/test_metacaster.py
```

### Comparing `metacast-0.1.4/LICENSE` & `metacast-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `metacast-0.1.4/PKG-INFO` & `metacast-0.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metacast
-Version: 0.1.4
+Version: 0.1.5
 Summary: A package for broadcasting epidemiological and ecological models over meta-populations.
 Author-email: Martin Grunnill <m.d.grunnill@gmail.com>
 Maintainer-email: Martin Grunnill <m.d.grunnill@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
@@ -273,12 +273,12 @@
 ### Installing via pip
 **Note** this should also install required packages.
 ```
 pip install metacast
 ```
 
 ## Usage
-See jupyter notebooks in demonstration directory of homepage:
+See jupyter notebooks in demonstration directory of the projects GitGub repository:
 [https://github.com/m-d-grunnill/MetaCast/tree/main/demonstrations](https://github.com/m-d-grunnill/MetaCast/tree/main/demonstrations)
 
 ## Documentation
 [https://metacast.readthedocs.io/en/latest/index.html](https://metacast.readthedocs.io/en/latest/index.html)
```

### Comparing `metacast-0.1.4/README.md` & `metacast-0.1.5/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -39,12 +39,12 @@
 ### Installing via pip
 **Note** this should also install required packages.
 ```
 pip install metacast
 ```
 
 ## Usage
-See jupyter notebooks in demonstration directory of homepage:
+See jupyter notebooks in demonstration directory of the projects GitGub repository:
 [https://github.com/m-d-grunnill/MetaCast/tree/main/demonstrations](https://github.com/m-d-grunnill/MetaCast/tree/main/demonstrations)
 
 ## Documentation
 [https://metacast.readthedocs.io/en/latest/index.html](https://metacast.readthedocs.io/en/latest/index.html)
```

### Comparing `metacast-0.1.4/pyproject.toml` & `metacast-0.1.5/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -3,15 +3,15 @@
     "setuptools >= 61.0",
     "wheel >= 0.38"
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "metacast"
-version = "0.1.4"
+version = "0.1.5"
 dependencies = [
     "numpy >= 1.26.3",
     "pandas >= 2.1.4",
     "scipy >= 1.11.4",
     "pingouin >= 0.5.4",
     "tqdm >= 4.66.1",
     "dask >= 2024.2.1",
```

### Comparing `metacast-0.1.4/src/metacast/event_handling/event_que.py` & `metacast-0.1.5/src/metacast/event_handling/event_que.py`

 * *Files 0% similar despite different names*

```diff
@@ -160,15 +160,15 @@
         Returns
         -------
         Nothing
         """
         event_names = self._event_names_checker(event_names)
         for event_name in event_names:
             event = self._events[event_name]
-            event.make_event_a_nullevent()
+            event._do_nothing = True
 
     def get_event_names(self):
         """
         Return list of event names.
         Returns
         -------
         List of strings
```

### Comparing `metacast-0.1.4/src/metacast/event_handling/events.py` & `metacast-0.1.5/src/metacast/event_handling/events.py`

 * *Files 1% similar despite different names*

```diff
@@ -72,20 +72,14 @@
 
         Returns
         -------
         Nothing
         """
         pass
 
-    def make_event_a_nullevent(self):
-        self._do_nothing = True
-
-    def undo_make_event_a_nullevent(self):
-        self._do_nothing = False
-
 
 
 class ValueFactorProportionChangeEvent(BaseEvent):
     """
     Parent event for events that involve changing a value or values.
 
     Parameters & Attributes
```

### Comparing `metacast-0.1.4/src/metacast/infection_seeding.py` & `metacast-0.1.5/src/metacast/infection_seeding.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,33 +11,33 @@
     
 """
 from numbers import Number
 import numpy as np
 import math
 
 class _InfectionBranch:
-    """
-    Makes multinomial draws for selecting which stage of an infection pathway to place infected hosts.
-    Calculates normalised weighting of an infection branch's states, based on inverse outflow for states.
-
-    Parameters & Attributes
-    -----------------------
-    name : string
-        Name of branch.
-    outflows: dictionary {str or ints: string}
-        Keys are name or number given to state. Values are name given to parameter.
-
-    Methods
-    -------
-    calculate_weighting(parameters)
-        Calculate normalised weighting for each state.
-    seed_infections(self, n, parameters)
-        Make multinomial draw to select infectious stages of this branch to seed infection into.
-
-    """
+    # """
+    # Makes multinomial draws for selecting which stage of an infection pathway to place infected hosts.
+    # Calculates normalised weighting of an infection branch's states, based on inverse outflow for states.
+    #
+    # Parameters & Attributes
+    # -----------------------
+    # name : string
+    #     Name of branch.
+    # outflows: dictionary {str or ints: string}
+    #     Keys are name or number given to state. Values are name given to parameter.
+    #
+    # Methods
+    # -------
+    # calculate_weighting(parameters)
+    #     Calculate normalised weighting for each state.
+    # seed_infections(self, n, parameters)
+    #     Make multinomial draw to select infectious stages of this branch to seed infection into.
+    #
+    # """
     def __init__(self, name, outflows):
         if not isinstance(name, str):
             raise TypeError('name argument should be a string.')
         self.name = name
         outflows_err_msg = ('outflows argument should be a dictionary,'+
                             ' with keys being strings or integers and values being string.')
         if not isinstance(outflows,dict):
@@ -156,29 +156,29 @@
         ----------
         seed : int (>0)
 
         """
         self.rng = np.random.default_rng(seed)
 
     def _seed_branches(self, n, branch_probability):
-        """
-        Make multinomial draw for which infection branch to place a host.
-
-        Parameters
-        ----------
-        n : int
-            Number of infections to seed.
-        branch_probability : dict {string, float}
-            Probability of being on each infection branch.
-
-        Returns
-        -------
-        draw_dict : dict {str: int}
-            Keys are branches values are number of infections on branch.
-        """
+        # """
+        # Make multinomial draw for which infection branch to place a host.
+        #
+        # Parameters
+        # ----------
+        # n : int
+        #     Number of infections to seed.
+        # branch_probability : dict {string, float}
+        #     Probability of being on each infection branch.
+        #
+        # Returns
+        # -------
+        # draw_dict : dict {str: int}
+        #     Keys are branches values are number of infections on branch.
+        # """
         if self.rng is None:
             rng = np.random.default_rng()
         else:
             rng = self.rng
         pvals = list(branch_probability.values())
         branches = list(branch_probability.keys())
         draw = rng.multinomial(n=n, pvals=pvals, size=1)
```

### Comparing `metacast-0.1.4/src/metacast/metacaster.py` & `metacast-0.1.5/src/metacast/metacaster.py`

 * *Files 3% similar despite different names*

```diff
@@ -35,31 +35,32 @@
         raise TypeError(str(string) + ' should be of type string.')
 
     check_list = eval('self.' + list_strings)
     if string not in check_list:
         raise ValueError(string + ' is not one of the predefined model ' + list_strings + ': ' +
                          ','.join(check_list[:-1]) + ' and ' + check_list[:-1] + '.')
 
+
 def _nested_dict_values(d):
     return [index for sub_d in d.values() for index in sub_d.values()]
 
 
 def _unionise_dict_of_lists(dict_of_lists):
-    """
-    Merge dictionary value lists into a list of unique values.
-
-    Parameters
-    ----------
-    dict_of_lists : dictionay of lists
-
-    Returns
-    -------
-    list
-        Merged unique list values.
-    """
+    # """
+    # Merge dictionary value lists into a list of unique values.
+    #
+    # Parameters
+    # ----------
+    # dict_of_lists : dictionay of lists
+    #
+    # Returns
+    # -------
+    # list
+    #     Merged unique list values.
+    # """
     return list(set().union(*dict_of_lists.values()))
 
 
 def _is_iterable_of_unique_elements(object):
     if not isinstance(object, Iterable):
         return False
     elif len(object) > len(set(object)):
@@ -91,16 +92,16 @@
 class MetaCaster:
     """
     Class for setting up and simulating multidimensional metapopulation models.
 
     Can simulate models on its own if given model_attributes and subpop_model arguments at initialisation.
     Alternatively these can be defined as attributes of MetaCaster subclass.
 
-    Parameters
-    ----------
+    Parameters & Attributes
+    -----------------------
     dimensions : int, collection of unique strings, list/tuple of ints, list/tuple of collections of unique strings OR list/tuple of dictionaries (transfer dictionaries)
         If int :
             This creates a one dimension metapopulation structure with range(scaffold) used to label subpopulations
             in dimensions attribute.
         If list/tuple/set of unique strings:
             This creates a one dimension metapopulation structure with entries used to label subpopulations
              in dimensions attribute.
@@ -121,37 +122,29 @@
                      length and the same length as the from_coordinates entries.
                 states: list of strings or string
                     Host states which will transition between subpopulations. Single entry of 'all' value
                     means all the available model states transition between subpopulations. Alternatively a list of
                     specific states can be given.
                 parameter : string
                     Name given to parameter that is responsible for flow of hosts transferring between subpopulations.
-            Optional key value pairs:
-                piecewise targets: list, tuple, numpy.Array or pandas.Series
-                    Targets for piecewise estimation of parameter that is responsible for flow of hosts transitions
-                    between clusters and vaccine groups (see method group_transfer).
+
     subpop_model : callable function/class method
         Method used to model subpopulation:
             Required arguments: 'y', 'y_deltas', 'parameters' and 'states_index'.
             Possible additional arguments: 'coordinates', 'subpop_suffix', 'foi' or 't'.
-    other_model_attributes : kwargs
-        Named arguments are attributes to be set. Alternatively these attributes can be set in a subclass of MetaCaster.
-
-    Attributes
-    ----------
     states : list of strings
         States used in model.
-    observed_states : list of strings
+    observed_states : string or list of strings , optional
         Observed states. Useful for obtaining results or fitting (e.g. Cumulative incidence).
-    infected_states : list of strings
+    infected_states : list of strings , optional
         Infected states (not necessarily infectious).
-    infectious_states : list of strings
+    infectious_states : string or list of strings , optional if not given value(s) for infected_states used
         Infectious states. These states contribute to force of infection. If None no force of infection is
         caluculated when running model (within ode method).
-    symptomatic_states : list of strings
+    symptomatic_states : string or list of strings , optional if not given value(s) for infected_states used
         Symptomatic states. NOTE any state in the list self.infectious_states but NOT in this list has its transmission
         modified by self.asymptomatic_transmission_modifier (see method calculate_fois).
     transmission_term_prefix : string, default 'beta'
         Prefix of subpopulation term used in calculating forces of infection, default term is 'beta' (see method
         calculate_fois).
     population_term_prefix : string, default 'N'
         Prefix of subpopulation term used as denominator in calculating force of infection (see method calculate_fois).
@@ -163,14 +156,24 @@
         asymptomatic_transmission_modifier's place when using method calculating_fois.
     universal_params : list of strings
         A list of all the parameters that are NOT:
         - directly to do with transmission
         - subpopulation specific (sub_pop_params).
     subpop_params : list of strings, or if axis/dimensions > 1 a dictionary {int: lists of strings}
          A list of all the parameters that axis/dimensions specific but NOT directly to do with transmission.
+    foi_population_focus : string or None (default None)
+        If None a subpopulations force of infection is not divided by  the total population of a subpopulation.
+        If 'i' a subpopulations force of infection is divided by the total population of subpopulation 'i',
+        i.e. its own population (the population that is being transmitted to).
+        If 'j' a subpopulations force of infection for each interacting subpopulation is divided by the total
+        population of subpopulation 'j', i.e. the subpopulation it is interacting with (the population that is being
+        transmitted from).
+
+    Attributes
+    ----------
     parameter_names : list of strings
         The names of all the parameters.
     population_terms : list of strings
         Subpopulation population terms used in calculating force of infection (see method calculate_fois).
     transmission_terms :  list of strings
         The transmission terms for each subpopulation (see method calculate_fois).
     subpop_interaction_terms : list of strings
@@ -189,37 +192,32 @@
         Each entry outlines parameters responsible for flows between subpopulations.
     all_states_index : dictionary
         Keys are all the states values are the associated indexes for use with numpy.arrays.
     state_index : dictionary {tuple of strings or ints: {string : int}}
         First level: keys are the subpopulation coordinates are another dictionary.
             Second level: keys are the states and values (ints) are the associated indexes for use with
                           numpy.arrays.
-    infected_states_index_list : list of ints
-        A list of the indexes of infected states.
+    infected_states_indexes : dictionary {tuple of strings or ints: [int]}
+        Keys are the subpopulation coordinates values are a list of indexes for infected states.
+    exposed_states_indexes : dictionary {tuple of strings or ints: [int]}
+        Keys are the subpopulation coordinates values are a list of indexes for infected but not infectious states.
     infectious_symptomatic_indexes : dictionary {tuple of strings or ints: [int]}
-        Keys are the subpopulation coordinates are a list of indexes for infectious and symptomatic states.
+        Keys are the subpopulation coordinates values are a list of indexes for infectious and symptomatic states.
     infectious_asymptomatic_indexes : dictionary {tuple of strings or ints: [int]}
-        Keys are the subpopulation coordinates are a list of indexes for infectious and asymptomatic states.
+        Keys are the subpopulation coordinates values are a list of indexes for infectious and asymptomatic states.
     infectious_and_symptomatic_states : list of stings
         A list of infectious and symptomatic states.
     infectious_and_asymptomatic_states : list of stings
         A list of infectious and asymptomatic states.
     total_states : int
         Total number of states in model.
     subpop_coordinates : list [tuples of ints/strings]
         Coordinates of all subpopulations.
     subpop_suffixes : list of stings
         Suffixes to appended to parameters specific to subpopulations.
-    _foi_population_focus : string or None (default None)
-        If None a subpopulations force of infection is not divided by  the total population of a subpopulation.
-        If 'i' a subpopulations force of infection is divided by the total population of subpopulation 'i',
-        i.e. its own population (the population that is being transmitted to).
-        If 'j' a subpopulations force of infection for each interacting subpopulation is divided by the total
-        population of subpopulation 'j', i.e. the subpopulation it is interacting with (the population that is being
-        transmitted from).
 
     Methods
     -------
     set_structure(self, scaffold, foi_population_focus=None)
         Set metapopulation structure using scaffold.
     ode(self, y, t, *parameters):
         Evaluate the ODE given states (y), time (t) and parameters
@@ -233,67 +231,132 @@
 
     Notes
     -----
     I have tried to use notation find in:
         Keeling, M. J., & Rohani, P. (2008). Metapopulations. In Modeling Infectious Diseases in Humans and Animals
         (pp. 237–240). Princeton University Press.
     """
-    states = None
-    infected_states = None
-    infectious_states = infected_states
-    symptomatic_states = infected_states
-    observed_states = None
-    transmission_term_prefix = 'beta'
-    subpop_interaction_prefix = 'rho'
-    population_term_prefix = 'N'
-    _foi_population_focus = None
-    asymptomatic_transmission_modifier = None
-    universal_params = None
     _dimensions = []
-    subpop_params = None  # does not include transmission term beta.
     _subpop_model = None
-    len = 0
+    _foi_population_focus = None
 
-    def __init__(self, dimensions, subpop_model=None, **other_model_attributes):
-        if other_model_attributes:
-            for name, value in other_model_attributes.items():
-                if not hasattr(self, name):
-                    raise AssertionError(name + 'is not a model attribute.')
-                setattr(self, name, value)
+    def __init__(self,
+                 dimensions,
+                 subpop_model,
+                 states,
+                 infected_states=None,
+                 infectious_states=None,
+                 symptomatic_states=None,
+                 observed_states=None,
+                 universal_params=None,
+                 subpop_params=None,
+                 foi_population_focus=None,
+                 transmission_term_prefix='beta',
+                 subpop_interaction_prefix='rho',
+                 population_term_prefix='N',
+                 asymptomatic_transmission_modifier=None
+                 ):
+        self.subpop_model = subpop_model
+        self.foi_population_focus = foi_population_focus
+        if not _is_set_like_of_strings(states):
+            raise TypeError("states should be a collection of unique strings.")
+        self.states = states
+
+        if isinstance(infected_states,str):
+            self.infected_states = [infected_states]
+        elif infected_states is None:
+            self.infected_states = []
+        elif _is_set_like_of_strings(infected_states):
+            self.infected_states = infected_states
+        else:
+            raise TypeError("If not None infected_states should be a collection of unique strings.")
+
+        if isinstance(infectious_states, str):
+            self.infectious_states = [infectious_states]
+        elif infectious_states is None:
+            self.infectious_states = infected_states
+        elif _is_set_like_of_strings(infectious_states):
+            self.infectious_states = infectious_states
+        else:
+            raise TypeError("If not None infectious_states should be a collection of unique strings.")
+
+        if isinstance(symptomatic_states, str):
+            self.symptomatic_states = [symptomatic_states]
+        elif symptomatic_states is None:
+            self.symptomatic_states = infected_states
+        elif _is_set_like_of_strings(symptomatic_states):
+            self.symptomatic_states = symptomatic_states
+        else:
+            raise TypeError("If not None symptomatic_states should be a collection of unique strings.")
+
+        if isinstance(observed_states, str):
+            self.observed_states = [observed_states]
+        elif observed_states is None:
+            self.observed_states = []
+        elif _is_set_like_of_strings(observed_states):
+            self.observed_states = observed_states
+        else:
+            raise TypeError("If not None observed_states should be a collection of unique strings.")
 
         if self.states is None:
             raise AssertionError('Model attribute "states" needs to be defined at initialisation of MetaCaster,' +
                                  ' or given as an attribute of a child class of MetaCaster.')
 
-        if self.universal_params is None and self.subpop_params is None:
+        if universal_params is None and subpop_params is None:
             raise AssertionError('At least one of the model attributes "universal_params" or "subpop_params" ' +
                                  'needs to be defined at initialisation of MetaCaster,' +
                                  ' or given as an attribute of a child class of MetaCaster.')
 
-        for model_attribute in ['states',
-                                'infected_states',
-                                'infectious_states',
-                                'symptomatic_states',
-                                'observed_states',
-                                'universal_params',
-                                'subpop_params']:
-            if eval('self.' + model_attribute) is not None:
-                if not _is_set_like_of_strings(eval('self.' + model_attribute)):
-                    raise TypeError('Model attribute "' +
-                                    model_attribute +
-                                    '" should be a collection of unique strings.')
-
-        if subpop_model is not None:
-            self.subpop_model = subpop_model
-
-        if type(self) == MetaCaster and other_model_attributes==False and subpop_model is None:
-            raise AssertionError('MetaCaster is not meant to run models without other_model_attributes and subpop_model.' +
-                                 ' Child classes of MetaCaster can if coded with other_model_attributes and subpop_model.' +
-                                 '\nIf unfamiliar with class inheritance look  up:\n' +
-                                 ' https://www.w3schools.com/python/python_inheritance.asp.')
+        if universal_params is None:
+            self.universal_params = []
+        elif _is_set_like_of_strings(universal_params):
+            self.universal_params = universal_params
+        else:
+            raise TypeError("If not None universal_params should be a collection of unique strings.")
+        if subpop_params is None:
+            self.subpop_params = []
+        elif _is_set_like_of_strings(subpop_params):
+            self.subpop_params = subpop_params
+        else:
+            raise TypeError("If not None subpop_params should be a collection of unique strings.")
+
+        if not isinstance(transmission_term_prefix, str):
+            raise TypeError('transmission_term_prefix should be a string.')
+        if transmission_term_prefix in self.subpop_params:
+            raise ValueError('transmission_term_prefix should not be one of the values in subpop_params.')
+        if transmission_term_prefix in self.universal_params:
+            raise ValueError('transmission_term_prefix should not be one of the values in universal_params.')
+        self.transmission_term_prefix = transmission_term_prefix
+
+        if not isinstance(subpop_interaction_prefix, str):
+            raise TypeError('subpop_interaction_prefix should be a string.')
+        if subpop_interaction_prefix in self.subpop_params:
+            raise ValueError('subpop_interaction_prefix should not be one of the values in subpop_params.')
+        if subpop_interaction_prefix in self.universal_params:
+            raise ValueError('subpop_interaction_prefix should not be one of the values in universal_params.')
+        self.subpop_interaction_prefix = subpop_interaction_prefix
+
+        if not isinstance(population_term_prefix, str):
+            raise TypeError('population_term_prefix should be a string.')
+        if population_term_prefix in self.subpop_params:
+            raise ValueError('population_term_prefix should not be one of the values in subpop_params.')
+        if population_term_prefix in self.universal_params:
+            raise ValueError('population_term_prefix should not be one of the values in universal_params.')
+        self.population_term_prefix = population_term_prefix
+
+        if asymptomatic_transmission_modifier is not None:
+            if not isinstance(asymptomatic_transmission_modifier, str):
+                raise TypeError('asymptomatic_transmission_modifier should be a string or None.')
+            if asymptomatic_transmission_modifier in self.subpop_params:
+                raise ValueError(
+                    'If not None asymptomatic_transmission_modifier should not be one of the values in subpop_params.')
+            if asymptomatic_transmission_modifier in self.universal_params:
+                raise ValueError(
+                    'If not None asymptomatic_transmission_modifier should not be one of the values in universal_params.')
+        self.asymptomatic_transmission_modifier = asymptomatic_transmission_modifier
         self.dimensions = dimensions
 
     def subpop_transfer(self, y, y_deltas, t, from_coordinates, parameters):
         """
         Calculates the transfers of people from a subpopulation to all other subpopulations.
 
         Parameters
@@ -314,71 +377,51 @@
         y_deltas : numpy.array
             Store of delta (derivative) of variables in y which this method adds/subtracts to.
 
         """
         if from_coordinates in self.subpop_transfer_dict:
             from_state_index_dict = self.state_index[from_coordinates]
             for group_transfer in self.subpop_transfer_dict[from_coordinates]:
-                parameter = group_transfer['parameter']
-                if 'piecewise targets' in group_transfer:
-                    # This section allows for the piecewise estimation of a people being transferred between groups.
-                    if t in self.piecewise_est_param_values[parameter]:
-                        param_val = self.piecewise_est_param_values[parameter][t]
-                    else:
-                        index_of_t = int(t) + 1
-                        total_being_tranfered = group_transfer['piecewise targets'][index_of_t]
-                        if total_being_tranfered == 0:  # No point in calculations if no one is being vaccinated.
-                            param_val = 0
-                        else:
-                            from_states_index = [from_state_index_dict[state] for state in group_transfer['states']]
-                            total_avialable = y[from_states_index].sum()
-                            param_val = self._instantaneous_transfer(total_being_tranfered,
-                                                                     total_avialable, t)
-
-                        self.piecewise_est_param_values[parameter][t] = param_val
-                else:
-                    param_val = parameters[parameter]
-
                 to_coordinates = group_transfer['to_coordinates']
                 to_state_index_dict = self.state_index[to_coordinates]
                 for state in group_transfer['states']:
                     from_index = from_state_index_dict[state]
                     to_index = to_state_index_dict[state]
-                    transferring = param_val * y[from_index]
+                    transferring = parameters[group_transfer['parameter']] * y[from_index]
                     y_deltas[from_index] -= transferring
                     y_deltas[to_index] += transferring
 
         return y_deltas
 
     def ode(self, y, t, *parameters):
         """
         Evaluate the ODE given states (y), time (t) and parameters
 
-
         Parameters
         ----------
         y : numpy.array
             State variables.
         t : float
             Time.
         parameters : floats
-            Parameter values.
+            Parameter values. **NOTE* these values must be given in the same order as the instance attribute
+            parameter_names.
 
         Returns
         -------
         y_delta: `numpy.ndarray`
             Deltas of state variables at time point t.
         """
         if self.subpop_model is None:
             raise AssertionError('subpop_model needs to set before simulations can run.')
 
         subpop_model = self.subpop_model
         subpop_model_arg_names = getfullargspec(subpop_model)[0]
-        parameters = dict(zip(self.non_piece_wise_params_names, parameters))
-        if self.infectious_states is not None:
+        parameters = dict(zip(self.parameter_names, parameters))
+        if self.infectious_states:
             fois = self.calculate_fois(y, parameters, t)
         y_deltas = np.zeros(self.total_states)
         for coordinates in self.subpop_coordinates:
             y_deltas = self.subpop_transfer(y, y_deltas, t, coordinates, parameters)
             if self.infectious_states is not None:
                 foi = fois[coordinates]  # force of infection experienced by this specific cluster.
 
@@ -480,17 +523,23 @@
         axis : int default = 0
             Axis on which coordinate is found.
 
         Returns
         -------
         nested dict: {tuple of int/str: {str: int}}
         """
-        selected_coordinates = [coordinates
-                                for coordinates in self.subpop_coordinates
-                                if coordinates[axis] == coordinate]
+        if axis+1 > len(self):
+            raise ValueError('Axis is out of bounds, i.e. axis +1 is greater then this MetaCaster instance\'s length.')
+
+        if len(self) == 1:
+            selected_coordinates = coordinate
+        else:
+            selected_coordinates = [coordinates
+                                    for coordinates in self.subpop_coordinates
+                                    if coordinates[axis] == coordinate]
         return {coordinates: sub_dict
                 for coordinates, sub_dict in self.state_index.items()
                 if coordinates in selected_coordinates}
 
     def get_indexes_of_coordinate(self, coordinate, axis=0):
         """
         Fetch a list of indices for all states for given coordinate on axis.
@@ -533,31 +582,31 @@
             return '_[' + coordinates + ']'
         elif isinstance(coordinates, int):
             return '_[' + str(coordinates) + ']'
         else:
             raise TypeError('All coordinates must be either string or integers, or lists/tuples of those types.')
 
     def _instantaneous_transfer(self, population_transitioning, population, t=None):
-        """
-        Calculate instantaneous rate needed to reduce population by population transitioning to another compartment.
-
-        Parameters
-        ----------
-        population_transitioning : float
-            Population moving between compartments.
-        population : float
-            Population from which transition is taking place.
-        t : float
-            Time at t. Used in generating an error specific to simulating models using this class.
-
-        Returns
-        -------
-        float
-            Instantaneous rate of change for the time t.
-        """
+        # """
+        # Calculate instantaneous rate needed to reduce population by population transitioning to another compartment.
+        #
+        # Parameters
+        # ----------
+        # population_transitioning : float
+        #     Population moving between compartments.
+        # population : float
+        #     Population from which transition is taking place.
+        # t : float
+        #     Time at t. Used in generating an error specific to simulating models using this class.
+        #
+        # Returns
+        # -------
+        # float
+        #     Instantaneous rate of change for the time t.
+        # """
         if population_transitioning > population:
             error_msg = "population_transitioning (" + str(
                 population_transitioning) + ") is greater than population (" + str(population)
             if t is None:
                 error_msg += ').'
             else:
                 error_msg += '), at time ' + str(t) + ').'
@@ -587,15 +636,14 @@
             Key word arguments to pass to scipy.integrate.odeint.
 
         Returns
         -------
         solution: pandas.DataFrame
             Multi-index columns are  clusters by vaccine groups by states.
         """
-        self.piecewise_est_param_values = {param: {} for param in self.params_estimated_via_piecewise_method}
         # INTEGRATE!!! (shout it out loud, in Dalek voice)
         # determine the number of output we want
         args = tuple(self.parameters.values())
         # The if else statement below is for use with DOK matrix version of the Jacobian see sileneced section below.
         # if self.dok_jacobian is None: # May or may not of defined the models Jacobian
         #     solution, output = scipy.integrate.odeint(self.ode,
         #                                               x0, t, args=args,
@@ -699,18 +747,14 @@
                          length and the same length as the from_coordinates entries.
                     states: list of strings or string
                         Host states which will transition between subpopulations. Single entry of 'all' value
                         means all the available model states transition between subpopulations. Alternatively a list of
                         specific states can be given.
                     parameter : string
                         Name given to parameter that is responsible for flow of hosts transferring between subpopulations.
-                Optional key value pairs:
-                    piecewise targets: list, tuple, numpy.Array or pandas.Series
-                        Targets for piecewise estimation of parameter that is responsible for flow of hosts transitions
-                        between clusters and vaccine groups (see method group_transfer).
 
         Returns
         -------
         None
 
         Notes: Attributes Altered
         -------------------------
@@ -736,20 +780,22 @@
             Each entry outlines parameters responsible for flows between subpopulations.
         all_states_index : dictionary
             Keys are all the states values are the associated indexes for use with numpy.arrays.
         state_index : dictionary {tuple of strings or ints: {string : int}}
             First level: keys are the subpopulation coordinates are another dictionary.
                 Second level: keys are the states and values (ints) are the associated indexes for use with
                               numpy.arrays.
-        infected_states_index_list : list of ints
-            A list of the indexes of infected states.
+        infected_states_indexes : dictionary {tuple of strings or ints: [int]}
+            Keys are the subpopulation coordinates values are a list of indexes for infected states.
+        exposed_states_indexes : dictionary {tuple of strings or ints: [int]}
+            Keys are the subpopulation coordinates values are a list of indexes for infected but not infectious states.
         infectious_symptomatic_indexes : dictionary {tuple of strings or ints: [int]}
-            Keys are the subpopulation coordinates are a list of indexes for infectious and symptomatic states.
+            Keys are the subpopulation coordinates values are a list of indexes for infectious and symptomatic states.
         infectious_asymptomatic_indexes : dictionary {tuple of strings or ints: [int]}
-            Keys are the subpopulation coordinates are a list of indexes for infectious and asymptomatic states.
+            Keys are the subpopulation coordinates values are a list of indexes for infectious and asymptomatic states.
         infectious_and_symptomatic_states : list of stings
             A list of infectious and symptomatic states.
         infectious_and_asymptomatic_states : list of stings
             A list of infectious and asymptomatic states.
         total_states : int
             Total number of states in model.
         subpop_coordinates : list [tuples of ints/strings]
@@ -758,15 +804,14 @@
             Suffixes to appended to parameters specific to subpopulations.
         """
         self.parameter_names = set(self.universal_params)
         if self.asymptomatic_transmission_modifier is not None:
             self.parameter_names.add(self.asymptomatic_transmission_modifier)
 
         #### Using Scaffold to define dimensions ####
-        self.params_estimated_via_piecewise_method = []
         self.subpop_transfer_dict = {}
         self.subpop_transition_params_dict = {}
         if isinstance(dimensions, (list, tuple)) and all(isinstance(item, dict) for item in dimensions):
             for count, group_transfer in enumerate(dimensions):
                 if 'from_coordinates' not in group_transfer:
                     raise ValueError(
                         'If scaffold is a list of subpopulation transfer dictionaries it must have a "from_coordinates"' +
@@ -866,56 +911,49 @@
                 entry['parameter'] = parameter
                 if parameter not in self.subpop_transition_params_dict:
                     self.subpop_transition_params_dict[parameter] = []
                 self.subpop_transition_params_dict[parameter].append({key: value for key, value in
                                                                       group_transfer.items()
                                                                       if key != 'parameter'})
                 self.parameter_names.add(parameter)
-                if 'piecewise targets' in group_transfer:
-                    self.params_estimated_via_piecewise_method.append(parameter)
-                    if isinstance(group_transfer['piecewise targets'], pd.Series):
-                        entry['piecewise targets'] = group_transfer['piecewise targets'].to_numpy()
-                    elif isinstance(group_transfer['piecewise targets'], (list, tuple)):
-                        entry['piecewise targets'] = np.array(group_transfer['piecewise targets'])
-                    elif isinstance(group_transfer['piecewise targets'], np.ndarray):
-                        entry['piecewise targets'] = group_transfer['piecewise targets']
 
                 accepted_keys = list(entry.keys()) + ['from_coordinates']
                 for key in group_transfer.keys():
                     if key not in accepted_keys:
                         raise ValueError('Subpopulation transfer dictionary [' +
                                          str(count) +
                                          '] of scaffold has an unrecognised entry (' + key + ').')
 
                 self.subpop_transfer_dict[from_coordinates].append(entry)
         elif (isinstance(dimensions, (list, tuple)) and
               all(_is_set_like_of_strings(item) for item in dimensions)):
             self._dimensions = [set(item) for item in dimensions]
         elif (isinstance(dimensions, (list, tuple)) and
               all(isinstance(item, int) for item in dimensions)):
-            self._dimensions = [set(*range(num)) for num in dimensions]
+            self._dimensions = [set(range(num)) for num in dimensions]
         elif isinstance(dimensions, (list, tuple)) and _is_set_like_of_strings(dimensions):
             self._dimensions = [set(dimensions)]
         elif isinstance(dimensions, set) and all(isinstance(item, str) for item in dimensions):
             self._dimensions = [dimensions]
         elif isinstance(dimensions, int):
-            self._dimensions = [set(*range(int))]
+            self._dimensions = [set(range(int))]
         else:
             raise TypeError('scaffold is not supported.')
 
         #### Definining States based on new Dimensions ####
         self.infectious_and_symptomatic_states = [state for state in self.infectious_states
                                                   if state in self.symptomatic_states]
         self.infectious_and_asymptomatic_states = [state for state in self.infectious_states
                                                    if state not in self.symptomatic_states]
         self.all_states_index = {}
         self.state_index = {}
         self.infectious_symptomatic_indexes = {}
         self.infectious_asymptomatic_indexes = {}
-        self.infected_states_index_list = []
+        self.exposed_states_indexes = {}
+        self.infected_states_indexes = {}
         # populating index dictionaries
         index = 0
         self.subpop_coordinates = []
         self.subpop_suffixes = []
         if len(self) == 1:
             axis_equals_1 = True
         else:
@@ -925,24 +963,29 @@
             self.subpop_suffixes.append(subpop_suffix)
             if axis_equals_1:
                 coordinates = coordinates[0]
             self.subpop_coordinates.append(coordinates)
             self.state_index[coordinates] = {}
             self.infectious_symptomatic_indexes[coordinates] = []
             self.infectious_asymptomatic_indexes[coordinates] = []
+            self.exposed_states_indexes[coordinates] = []
+            self.infected_states_indexes[coordinates] = []
             for state in self.states:
                 all_state_index_key = state + subpop_suffix
                 self.all_states_index[all_state_index_key] = index
                 self.state_index[coordinates][state] = index
                 if state in self.infectious_and_symptomatic_states:
                     self.infectious_symptomatic_indexes[coordinates].append(index)
                 if state in self.infectious_and_asymptomatic_states:
                     self.infectious_asymptomatic_indexes[coordinates].append(index)
                 if state in self.infected_states:
-                    self.infected_states_index_list.append(index)
+                    self.infected_states_indexes[coordinates].append(index)
+                if state in self.infected_states and state not in self.infectious_states:
+                    self.exposed_states_indexes[coordinates].append(index)
+
                 index += 1
 
         self.state_index['observed_states'] = {}
         for state in self.observed_states:
             self.all_states_index[state] = index
             self.state_index['observed_states'][state] = index
             index += 1
@@ -981,19 +1024,16 @@
             self.population_terms = [self.population_term_prefix + subpop_suffix
                                      for subpop_suffix in self.subpop_suffixes]
             self.parameter_names.update(self.population_terms)
 
         self.parameter_names.update(self.transmission_terms)
         self.total_subpops = len(self.subpop_coordinates)
         self.parameter_names = sorted(self.parameter_names)
-        non_piece_wise_params_names = set(self.parameter_names) - set(self.params_estimated_via_piecewise_method)
-        self.non_piece_wise_params_names = sorted(list(non_piece_wise_params_names))
         self._parameters = None
         self.total_parameters = len(self.parameter_names)
-        self.piecewise_est_param_values = None
 
     @property
     def foi_population_focus(self):
         return self._foi_population_focus
 
     @foi_population_focus.setter
     def foi_population_focus(self, foi_population_focus):
@@ -1048,48 +1088,44 @@
             'y', 'parameters', 'coordinates', 't'.
 
         Returns
         -------
         Nothing
         """
         if not isinstance(parameters, dict):
-            raise TypeError('Currently non non_piecewise_params must be entered as a dict.')
+            raise TypeError('Currently parameters must be entered as a dict.')
         # we assume that the key of the dictionary is a string and
         # the value can be a single value or a distribution
 
         for param_name, value in parameters.items():
             if param_name not in self.parameter_names:
                 raise ValueError(param_name + ' is not a name given to a parameter for this model.')
-            if param_name in self.params_estimated_via_piecewise_method:
-                raise AssertionError(param_name + ' was set as a parameter to be estimated via piecewise estimiation ' +
-                                     'at the initialization of this model.')
             if callable(value):
                 function_arg_names = getfullargspec(value)[0]
                 if any(args not in ['model', 'y', 'parameters', 'coordinates', 't'] for args in function_arg_names):
                     raise ValueError(param_name +
                                      " is a function but not a population_term but does not have all of the arguments" +
                                      " 'model', 'y', 'parameters', 'coordinates' or 't'.")
             elif not isinstance(value, Number):
                 raise TypeError(param_name + ' should be a number type.')
         params_not_given = [param for param in self.parameter_names
-                            if param not in
-                            list(parameters.keys()) + self.params_estimated_via_piecewise_method]
+                            if param not in parameters]
         if params_not_given:
             raise Exception(', '.join(params_not_given) +
                             " are/is missing from parameters for model (see self.all_parameters).")
-        # this must be sorted alphanumerically.
-        self._parameters = {key: value for key, value in sorted(parameters.items())}
+        # this must be sorted in the same order as parameter_names (i.e. alphanumerically).
+        self._parameters = {parameter: parameters[parameter] for parameter in self.parameter_names}
 
     @property
     def shape(self):
         """
         Number of entries in each axis of the metapopulation model.
 
         Returns
         -------
         tuple of ints
         """
-        return (len(axis) for axis in self._dimensions)
+        return tuple(len(axis) for axis in self._dimensions)
 
 
 if __name__ == "__main__":
     pass
```

### Comparing `metacast-0.1.4/src/metacast/sensitivity_analyses/asses_lh_sample_size.py` & `metacast-0.1.5/src/metacast/sensitivity_analyses/asses_lh_sample_size.py`

 * *Files identical despite different names*

### Comparing `metacast-0.1.4/src/metacast/sensitivity_analyses/lhs_and_prcc.py` & `metacast-0.1.5/src/metacast/sensitivity_analyses/lhs_and_prcc.py`

 * *Files identical despite different names*

### Comparing `metacast-0.1.4/src/metacast.egg-info/PKG-INFO` & `metacast-0.1.5/src/metacast.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metacast
-Version: 0.1.4
+Version: 0.1.5
 Summary: A package for broadcasting epidemiological and ecological models over meta-populations.
 Author-email: Martin Grunnill <m.d.grunnill@gmail.com>
 Maintainer-email: Martin Grunnill <m.d.grunnill@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
@@ -273,12 +273,12 @@
 ### Installing via pip
 **Note** this should also install required packages.
 ```
 pip install metacast
 ```
 
 ## Usage
-See jupyter notebooks in demonstration directory of homepage:
+See jupyter notebooks in demonstration directory of the projects GitGub repository:
 [https://github.com/m-d-grunnill/MetaCast/tree/main/demonstrations](https://github.com/m-d-grunnill/MetaCast/tree/main/demonstrations)
 
 ## Documentation
 [https://metacast.readthedocs.io/en/latest/index.html](https://metacast.readthedocs.io/en/latest/index.html)
```

