# Comparing `tmp/gawseed-tcorex-1.1.tar.gz` & `tmp/gawseed_tcorex-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gawseed-tcorex-1.1.tar", last modified: Mon Mar  7 22:28:09 2022, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `gawseed-tcorex-1.1.tar` & `gawseed_tcorex-1.1.1.tar`

### file list

```diff
@@ -1,33 +1,22 @@
-drwxrwxr-x   0 hardaker  (2174) hardaker  (2174)        0 2022-03-07 22:28:09.820534 gawseed-tcorex-1.1/
--rw-rw-r--   0 hardaker  (2174) hardaker  (2174)    34522 2020-05-05 19:45:58.000000 gawseed-tcorex-1.1/LICENSE
--rw-rw-r--   0 hardaker  (2174) hardaker  (2174)    15167 2022-03-07 22:28:09.819534 gawseed-tcorex-1.1/PKG-INFO
--rw-rw-r--   0 hardaker  (2174) hardaker  (2174)    12209 2022-03-07 22:24:20.000000 gawseed-tcorex-1.1/README.md
-drwxrwxr-x   0 hardaker  (2174) hardaker  (2174)        0 2022-03-07 22:28:09.817534 gawseed-tcorex-1.1/gawseed_tcorex.egg-info/
--rw-rw-r--   0 hardaker  (2174) hardaker  (2174)    15167 2022-03-07 22:28:09.000000 gawseed-tcorex-1.1/gawseed_tcorex.egg-info/PKG-INFO
--rw-rw-r--   0 hardaker  (2174) hardaker  (2174)      690 2022-03-07 22:28:09.000000 gawseed-tcorex-1.1/gawseed_tcorex.egg-info/SOURCES.txt
--rw-rw-r--   0 hardaker  (2174) hardaker  (2174)        1 2022-03-07 22:28:09.000000 gawseed-tcorex-1.1/gawseed_tcorex.egg-info/dependency_links.txt
--rw-rw-r--   0 hardaker  (2174) hardaker  (2174)      161 2022-03-07 22:28:09.000000 gawseed-tcorex-1.1/gawseed_tcorex.egg-info/entry_points.txt
--rw-rw-r--   0 hardaker  (2174) hardaker  (2174)       40 2022-03-07 22:28:09.000000 gawseed-tcorex-1.1/gawseed_tcorex.egg-info/requires.txt
--rw-rw-r--   0 hardaker  (2174) hardaker  (2174)        7 2022-03-07 22:28:09.000000 gawseed-tcorex-1.1/gawseed_tcorex.egg-info/top_level.txt
--rw-rw-r--   0 hardaker  (2174) hardaker  (2174)       38 2022-03-07 22:28:09.820534 gawseed-tcorex-1.1/setup.cfg
--rw-rw-r--   0 hardaker  (2174) hardaker  (2174)     1602 2022-03-07 22:28:03.000000 gawseed-tcorex-1.1/setup.py
-drwxrwxr-x   0 hardaker  (2174) hardaker  (2174)        0 2022-03-07 22:28:09.818534 gawseed-tcorex-1.1/tcorex/
--rw-rw-r--   0 hardaker  (2174) hardaker  (2174)      138 2020-05-05 19:45:58.000000 gawseed-tcorex-1.1/tcorex/__init__.py
--rw-rw-r--   0 hardaker  (2174) hardaker  (2174)    10671 2022-03-02 21:45:21.000000 gawseed-tcorex-1.1/tcorex/base.py
--rw-rw-r--   0 hardaker  (2174) hardaker  (2174)    10212 2022-03-02 21:56:19.000000 gawseed-tcorex-1.1/tcorex/corex.py
--rw-rw-r--   0 hardaker  (2174) hardaker  (2174)     6582 2022-03-02 17:45:54.000000 gawseed-tcorex-1.1/tcorex/covariance.py
-drwxrwxr-x   0 hardaker  (2174) hardaker  (2174)        0 2022-03-07 22:28:09.818534 gawseed-tcorex-1.1/tcorex/experiments/
--rw-rw-r--   0 hardaker  (2174) hardaker  (2174)        0 2020-05-05 19:45:58.000000 gawseed-tcorex-1.1/tcorex/experiments/__init__.py
--rw-rw-r--   0 hardaker  (2174) hardaker  (2174)    24618 2022-03-02 17:46:06.000000 gawseed-tcorex-1.1/tcorex/experiments/baselines.py
--rw-rw-r--   0 hardaker  (2174) hardaker  (2174)    19677 2022-03-02 17:46:37.000000 gawseed-tcorex-1.1/tcorex/experiments/data.py
--rw-rw-r--   0 hardaker  (2174) hardaker  (2174)     3460 2022-03-02 17:46:52.000000 gawseed-tcorex-1.1/tcorex/experiments/fmri_utils.py
--rw-rw-r--   0 hardaker  (2174) hardaker  (2174)      193 2020-05-05 19:45:58.000000 gawseed-tcorex-1.1/tcorex/experiments/misc.py
--rw-rw-r--   0 hardaker  (2174) hardaker  (2174)      926 2022-03-02 17:47:02.000000 gawseed-tcorex-1.1/tcorex/experiments/vis_utils.py
--rw-rw-r--   0 hardaker  (2174) hardaker  (2174)      403 2022-03-02 05:02:51.000000 gawseed-tcorex-1.1/tcorex/plot_utils.py
--rw-rw-r--   0 hardaker  (2174) hardaker  (2174)    12572 2022-03-02 17:46:23.000000 gawseed-tcorex-1.1/tcorex/tcorex.py
--rw-rw-r--   0 hardaker  (2174) hardaker  (2174)    13446 2022-03-02 17:45:59.000000 gawseed-tcorex-1.1/tcorex/tcorex_learnable.py
-drwxrwxr-x   0 hardaker  (2174) hardaker  (2174)        0 2022-03-07 22:28:09.819534 gawseed-tcorex-1.1/tcorex/tools/
--rw-rw-r--   0 hardaker  (2174) hardaker  (2174)        0 2022-03-02 04:34:57.000000 gawseed-tcorex-1.1/tcorex/tools/__init__.py
--rw-rw-r--   0 hardaker  (2174) hardaker  (2174)     2953 2022-03-04 18:00:54.000000 gawseed-tcorex-1.1/tcorex/tools/tcorex_changepoints.py
--rw-rw-r--   0 hardaker  (2174) hardaker  (2174)     5758 2022-03-04 18:38:47.000000 gawseed-tcorex-1.1/tcorex/tools/tcorex_cli.py
--rw-rw-r--   0 hardaker  (2174) hardaker  (2174)     2434 2022-03-02 17:53:12.000000 gawseed-tcorex-1.1/tcorex/tools/tcorex_plot.py
+-rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 gawseed_tcorex-1.1.1/gawseed_tcorex/__init__.py
+-rw-r--r--   0        0        0    10671 2020-02-02 00:00:00.000000 gawseed_tcorex-1.1.1/gawseed_tcorex/base.py
+-rw-r--r--   0        0        0    10212 2020-02-02 00:00:00.000000 gawseed_tcorex-1.1.1/gawseed_tcorex/corex.py
+-rw-r--r--   0        0        0     6582 2020-02-02 00:00:00.000000 gawseed_tcorex-1.1.1/gawseed_tcorex/covariance.py
+-rw-r--r--   0        0        0      403 2020-02-02 00:00:00.000000 gawseed_tcorex-1.1.1/gawseed_tcorex/plot_utils.py
+-rw-r--r--   0        0        0    12574 2020-02-02 00:00:00.000000 gawseed_tcorex-1.1.1/gawseed_tcorex/tcorex.py
+-rw-r--r--   0        0        0    13446 2020-02-02 00:00:00.000000 gawseed_tcorex-1.1.1/gawseed_tcorex/tcorex_learnable.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gawseed_tcorex-1.1.1/gawseed_tcorex/experiments/__init__.py
+-rw-r--r--   0        0        0    24618 2020-02-02 00:00:00.000000 gawseed_tcorex-1.1.1/gawseed_tcorex/experiments/baselines.py
+-rw-r--r--   0        0        0    19677 2020-02-02 00:00:00.000000 gawseed_tcorex-1.1.1/gawseed_tcorex/experiments/data.py
+-rw-r--r--   0        0        0     3460 2020-02-02 00:00:00.000000 gawseed_tcorex-1.1.1/gawseed_tcorex/experiments/fmri_utils.py
+-rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 gawseed_tcorex-1.1.1/gawseed_tcorex/experiments/misc.py
+-rw-r--r--   0        0        0      926 2020-02-02 00:00:00.000000 gawseed_tcorex-1.1.1/gawseed_tcorex/experiments/vis_utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gawseed_tcorex-1.1.1/gawseed_tcorex/tools/__init__.py
+-rw-r--r--   0        0        0     2950 2020-02-02 00:00:00.000000 gawseed_tcorex-1.1.1/gawseed_tcorex/tools/tcorex_changepoints.py
+-rw-r--r--   0        0        0     5687 2020-02-02 00:00:00.000000 gawseed_tcorex-1.1.1/gawseed_tcorex/tools/tcorex_cli.py
+-rw-r--r--   0        0        0     2450 2020-02-02 00:00:00.000000 gawseed_tcorex-1.1.1/gawseed_tcorex/tools/tcorex_plot.py
+-rw-r--r--   0        0        0     1220 2020-02-02 00:00:00.000000 gawseed_tcorex-1.1.1/.gitignore
+-rw-r--r--   0        0        0    34522 2020-02-02 00:00:00.000000 gawseed_tcorex-1.1.1/LICENSE
+-rw-r--r--   0        0        0    12396 2020-02-02 00:00:00.000000 gawseed_tcorex-1.1.1/README.md
+-rw-r--r--   0        0        0     1545 2020-02-02 00:00:00.000000 gawseed_tcorex-1.1.1/pyproject.toml
+-rw-r--r--   0        0        0    13382 2020-02-02 00:00:00.000000 gawseed_tcorex-1.1.1/PKG-INFO
```

### Comparing `gawseed-tcorex-1.1/LICENSE` & `gawseed_tcorex-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `gawseed-tcorex-1.1/PKG-INFO` & `gawseed_tcorex-1.1.1/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,314 +1,332 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: gawseed-tcorex
-Version: 1.1
+Version: 1.1.1
 Summary: Correlation Explanation Methods
-Home-page: https://github.com/gawseed/T-CorEx
-Author: Hrayr Harutyunyan
-Author-email: harhro@gmail.com
-License: GNU Affero General Public License v3.0
-Description: # Purpose
-        
-        The T-Corex algorithm is designed to identify changes in correlation
-        in datasets of large signals.  Given windows of signals.
-        
-        This package modifies the [original implementation] Hrayr Harutyunyan to
-        add documentation and CLI tools.
-        
-        [original implementation]: https://github.com/hrayrhar/T-CorEx
-        
-        # Usage
-        
-        ## Installation
-        
-        Install with `pip` (or `pipx`):
-        
-        ```
-        pip3 install gawseed-tcorex
-        ```
-        
-        ## Analysis
-        
-        To analyze a temporal time-series of data in a csv file, run tcorex 
-        similar to:
-        
-        ```
-        tcorex -w 30 -n 100 -w 30 -g .1 -l .5 input_data.csv output.pkl
-        ```
-        
-        Discussion and help with selecting parameters is discussed below.
-        
-        ## Displaying results
-        
-        To list the correlations within each window, use
-        `tcorex-changepoints` on the resulting pkl file:
-        
-        ```
-        tcorex-changepoints output.pkl
-        ```
-        
-        To show a graph of which time periods had the highest rate of
-        correlation changes, use `tcorex-plot`:
-        
-        ```
-        tcorex-plot -o changes output.pkl
-        ```
-        
-        ## Picking algorithm parameters
-        
-        ### Number of latent factors (-n)
-        
-        Look at the number of signals you have, and if you have a lot there
-        should be more latent factors.  If
-        you pick a value too low, then all the signals will appear to be
-        correlated even when they are not.  If you pick a value which is too
-        large, only an identity matrix will be produced and all the signals
-        will appear independent.  Typically start with a roughly small value
-        and raise it to improve results with respect to signals that are
-        actually related.
-        
-        The number of latent factors should be roughly 2 order of magnitudes
-        lower (IE *number_of_signals/100*).
-        
-        ### Window size (-w)
-        
-        The algorithm is designed to look for changes in correlations between
-        two windows.
-        
-        The window size indicates how frequently changes will happen to
-        attempt to find changes between different window sizes.  If the window
-        is too small, then the accuracy will be reduced and more correlations
-        will be found as signals always appear similar at some point when
-        broken into small chunks.  If the window is too large, then no changes
-        will be easily detected because the difference between varying signals
-        will appear large.  When windows are large, you also lose track about
-        where correlation changes actually happen because the change point can
-        be anywhere in the window.
-        
-        ### Gamma
-        
-        Range: 0.1-10
-        
-        The Gamma value sets the decay rate for sample weights.  Bigger values
-        will result in more data being included, which is good for smaller
-        datasets.  If enough data is present, then low values should be used.
-        
-        ### L1 regularization strength
-        
-        Higher L1 values are better better for signals with rapid changes
-        
-        ### L2
-        
-        Better for smooth time series.  There is no current CLI option for this.
-        
-        # Correlation Explanation Methods
-        
-        Official implementation of linear correlation explanation (linear CorEx) and temporal correlation explanation (T-CorEx) methods.
-        
-        #### Linear CorEx
-        Linear CorEx searches for independent latent factors that explain all correlations between observed variables, while also biasing
-        the model selection towards modular latent factor models – directed latent factor graphical models
-        where each observed variable has a single latent variable as its only parent.
-        This is useful for covariance estimation, clustering related variables, and dimensionality reduction, especially in the high-dimensional and under-sampled regime.
-        The complete description of the method is presented in NeurIPS 2019 [paper](https://papers.nips.cc/paper/9691-fast-structure-learning-with-modular-regularization) *"Fast structure learning with modular regularization"* by Greg Ver Steeg, Hrayr Harutyunyan, Daniel Moyer, and Aram Galstyan.
-        If you want to cite this paper, please use the following BibTex entry:
-        ```text
-        @incollection{NIPS2019_9691,
-        title = {Fast structure learning with modular regularization},
-        author = {Ver Steeg, Greg and Harutyunyan, Hrayr and Moyer, Daniel and Galstyan, Aram},
-        booktitle = {Advances in Neural Information Processing Systems 32},
-        editor = {H. Wallach and H. Larochelle and A. Beygelzimer and F. d\textquotesingle Alch\'{e}-Buc and E. Fox and R. Garnett},
-        pages = {15567--15577},
-        year = {2019},
-        publisher = {Curran Associates, Inc.},
-        url = {http://papers.nips.cc/paper/9691-fast-structure-learning-with-modular-regularization.pdf}
-        }
-        ```
-        
-        **Note:** Greg Ver Steeg has an alternative implementation of linear CorEx, which is available at [github.com/gregversteeg/LinearCorex](https://github.com/gregversteeg/LinearCorex).
-        That implementation uses a quazi-Newton optimization method for learning the model parameters. 
-        In contrast, the implementation provided in this repository uses ADAM optimizer.
-        This latter implementation utilizes GPUs better, and can converge to slightly better objective values if the input data is highly non-modular.
-        Nevertheless, we highly encourage to take a look at the alternative implementation.
-        
-        #### T-CorEx
-        T-CorEx is a method for covariance estimation from temporal data.
-        It trains a linear CorEx for each time period,
-        while employing two regularization techniques to enforce temporal consistency of estimates.
-        The method is introduced in the [paper](https://arxiv.org/abs/1905.13276) *"Efficient Covariance Estimation from Temporal Data"* by Hrayr Harutunyan, Daniel Moyer, Hrant Khachatrian, Greg Ver Steeg, and Aram Galstyan.
-        If you want to cite this paper, please use the following BibTex entry:
-        ```text
-        @article{tcorex,
-          title={Efficient Covariance Estimation from Temporal Data},
-          author={Harutyunyan, Hrayr and Moyer, Daniel and Khachatrian, Hrant and Steeg, Greg Ver and Galstyan, Aram},
-          journal={arXiv preprint arXiv:1905.13276},
-          year={2019}
-        }
-        ```
-        
-        
-        Both linear CorEx and T-CorEx have linear time and memory complexity with respect to the number of observed variables and can be applied to high-dimensional datasets.
-        For example, it takes less than an hour on a moderate PC to estimate the covariance structure for time series with 100K variables using T-CorEx.
-        Both methods are implemented in PyTorch and can run on CPUs and GPUs.
-        
-        
-        ## Requirements and Installation
-        The code is writen in Python 3, but should run on Python 2 as well.
-        The dependencies are the following: 
-        * numpy, scipy, tqdm, PyTorch
-        * [optional] nibabel (for fMRI experiments)
-        * [optional] nose (for tests)
-        * [optional] sklearn, regain, TVGL, linearcorex, pandas (for running comparisions)
-        * [optional] matplotlib and nilearn (for visualizations)
-        
-        To install the code, run the following command:
-        ```text
-        python setup.py install
-        ```
-        
-        ## Description
-        The main method for linear CorEx is the class `tcorex.Corex`, and that of T-CorEx is 'tcorex.TCorex'.
-        The complete description of parameters of these classes can be found in the corresponding docstrings.
-        While there are many parameters (especially for T-CorEx), in general only a couple of them need to be tuned (others are set to their "best" values).
-        Those parameters are:
-        
-        
-        | Parameter | Linear CorEx | T-CorEx | Description |    
-        |:---------|---|---|:---|   
-        | `m` | + | + | The number of latent variables. Usually this is much smaller than the number of observed variables. |  
-        | `l1` | - | + | A non-negative real number specifying the coefficient of l1 temporal regularization.|  
-        | `gamma` | - | + | A real number in [0,1]. This argument controls the sample weights. The samples of time period t' will have weight w_t(t')=gamma^\|t' - t\| when estimating quantities for time period t. Smaller values are used for very dynamic time series.|  
-        
-        
-        ## Usage
-        
-        Run the following command for a sample run of TCorex. 
-        ```bash
-        python -m examples.sample_run
-        ```
-        
-        The code is shown below:
-        ``` python 
-        from __future__ import print_function
-        from __future__ import absolute_import
-        
-        from tcorex.experiments.data import load_modular_sudden_change
-        from tcorex.experiments import baselines
-        from tcorex import base
-        from tcorex import TCorex
-        from tcorex import covariance as cov_utils
-        
-        import numpy as np
-        import matplotlib
-        matplotlib.use('agg')
-        from matplotlib import pyplot as plt
-        
-        
-        def main():
-            nv = 32         # number of observed variables
-            m = 4           # number of hidden variables
-            nt = 10         # number of time periods
-            train_cnt = 16  # number of training samples for each time period
-            val_cnt = 4     # number of validation samples for each time period
-        
-            # Generate some data with a sudden change in the middle.
-            data, ground_truth_sigma = load_modular_sudden_change(nv=nv, m=m, nt=nt, ns=(train_cnt + val_cnt))
-        
-            # Split it into train and validation.
-            train_data = [X[:train_cnt] for X in data]
-            val_data = [X[train_cnt:] for X in data]
-        
-            # NOTE: the load_modular_sudden_change function above creates data where the time axis
-            # is already divided into time periods. If your data is not divided into time periods
-            # you can use the following procedure to do that:
-            # bucketed_data, index_to_bucket = make_buckets(data, window=train_cnt + val_cnt, stride='full')
-            # where the make_buckets function can be found at tcorex.experiments.data
-        
-            # The core method we have is the tcorex.TCorex class.
-            tc = TCorex(nt=nt,
-                        nv=nv,
-                        n_hidden=m,
-                        max_iter=500,
-                        device='cpu',  # for GPU set 'cuda',
-                        l1=0.3,        # coefficient of temporal regularization term
-                        gamma=0.3,     # parameter that controls sample weights
-                        verbose=1,     # 0, 1, 2
-                        )
-        
-            # Fit the parameters of T-CorEx.
-            tc.fit(train_data)
-        
-            # We can compute the clusters of observed variables for each time period.
-            t = 8
-            clusters = tc.clusters()
-            print("Clusters at time period {}: {}".format(t, clusters[t]))
-        
-            # We can get an estimate of the covariance matrix for each time period.
-            # When normed=True, estimates of the correlation matrices will be returned.
-            covs = tc.get_covariance()
-        
-            # We can visualize the covariance matrices.
-            fig, ax = plt.subplots(1, figsize=(5, 5))
-            im = ax.imshow(covs[t])
-            fig.colorbar(im)
-            ax.set_title("Estimated covariance matrix\nat time period {}".format(t))
-            fig.savefig('covariance-matrix.png')
-        
-            # It is usually useful to compute the inverse correlation matrices,
-            # since this matrices can be interpreted as adjacency matrices of
-            # Markov random fields.
-            cors = tc.get_covariance(normed=True)
-            inv_cors = [np.linalg.inv(x) for x in cors]
-        
-            # We can visualize the thresholded inverse correlation matrices.
-            fig, ax = plt.subplots(1, figsize=(5, 5))
-            thresholded_inv_cor = np.abs(inv_cors[t]) > 0.05
-            ax.imshow(thresholded_inv_cor)
-            ax.set_title("Thresholded inverse correlation\nmatrix at time period {}".format(t))
-            fig.savefig('thresholded-inverse-correlation-matrix.png')
-        
-            # We can also plot the Frobenius norm of the differences of inverse
-            # correlation matrices of  neighboring time periods. This is helpful
-            # for detecting the sudden change points of the system.
-            diffs = cov_utils.diffs(inv_cors)
-            fig, ax = plt.subplots(1, figsize=(5, 5))
-            ax.plot(diffs)
-            ax.set_xlabel('t')
-            ax.set_ylabel('$||\Sigma^{-1}_{t+1} - \Sigma^{-1}_{t}||_2$')
-            ax.set_title("Frobenius norms of differences between\ninverse correlation matrices")
-            fig.savefig('inv-correlation-difference-norms.png')
-        
-            # We can also do grid search on a hyperparameter grid the following way.
-            # NOTE: this can take time!
-            baseline, grid = (baselines.TCorex(tcorex=TCorex, name='T-Corex'), {
-                'nv': nv,
-                'n_hidden': m,
-                'max_iter': 500,
-                'device': 'cpu',
-                'l1': [0.0, 0.03, 0.3, 3.0],
-                'gamma': [1e-6, 0.3, 0.5, 0.8]
-            })
-        
-            best_score, best_params, best_covs, best_method, all_results = baseline.select(train_data, val_data, grid)
-            tc = best_method  # this is the model that performed the best on the validation data, you can use it as above
-            base.save(tc, 'best_method.pkl')
-        
-        
-        if __name__ == '__main__':
-            main()
-        ```
-        
-        
-        
-Platform: UNKNOWN
-Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Classifier: Topic :: Scientific/Engineering :: Information Analysis
-Classifier: Topic :: Scientific/Engineering :: Mathematics
+Project-URL: Homepage, https://github.com/gawseed/T-CorEx
+Author-email: Hrayr Harutyunyan <harhro@gmail.com>
+License-Expression: AGPL-3.0
+License-File: LICENSE
+Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: GNU Affero General Public License v3
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
+Classifier: Topic :: Scientific/Engineering :: Information Analysis
+Classifier: Topic :: Scientific/Engineering :: Mathematics
+Requires-Dist: linearcorex==0.52
+Requires-Dist: matplotlib>=2.2.2
+Requires-Dist: nibabel>=2.3.1
+Requires-Dist: nilearn>=0.4.2
+Requires-Dist: nose>=1.3.7
+Requires-Dist: numpy>=1.14.2
+Requires-Dist: pandas>=0.23.4
+Requires-Dist: regain==0.1.7
+Requires-Dist: scikit-learn
+Requires-Dist: scikit-learn>=0.20.0
+Requires-Dist: scipy>=1.1.0
+Requires-Dist: torch>=1.0
+Requires-Dist: tqdm>=4.26
 Description-Content-Type: text/markdown
-License-File: LICENSE
+
+# Purpose
+
+The T-Corex algorithm is designed to identify changes in correlation
+in datasets of large signals.  Given windows of signals.
+
+This package modifies the [original implementation] Hrayr Harutyunyan to
+add documentation and CLI tools.
+
+[original implementation]: https://github.com/hrayrhar/T-CorEx
+
+# Usage
+
+## Installation
+
+Install with `pip` (or `pipx`):
+
+```
+pip3 install gawseed-tcorex
+```
+
+## Analysis
+
+To analyze a temporal time-series of data in a csv file, run tcorex 
+similar to:
+
+```
+tcorex -w 30 -n 100 -w 30 -g .1 -l .5 input_data.csv output.pkl
+```
+
+Discussion and help with selecting parameters is discussed below.
+
+The CSV file should have a header row, and the default columns to use
+are *timestamp*, *key* and *value* but may be changed with
+`--time-column`, `-k` and `-v`.
+
+## Displaying results
+
+To list the correlations within each window, use
+`tcorex-changepoints` on the resulting pkl file:
+
+```
+tcorex-changepoints output.pkl
+```
+
+To show a graph of which time periods had the highest rate of
+correlation changes, use `tcorex-plot`:
+
+```
+tcorex-plot -o changes output.pkl
+```
+
+## Picking algorithm parameters
+
+### Number of latent factors (-n)
+
+Look at the number of signals you have, and if you have a lot there
+should be more latent factors.  If
+you pick a value too low, then all the signals will appear to be
+correlated even when they are not.  If you pick a value which is too
+large, only an identity matrix will be produced and all the signals
+will appear independent.  Typically start with a roughly small value
+and raise it to improve results with respect to signals that are
+actually related.
+
+The number of latent factors should be roughly 2 order of magnitudes
+lower (IE *number_of_signals/100*).
+
+### Window size (-w)
+
+The algorithm is designed to look for changes in correlations between
+two windows.
+
+The window size indicates how frequently changes will happen to
+attempt to find changes between different window sizes.  If the window
+is too small, then the accuracy will be reduced and more correlations
+will be found as signals always appear similar at some point when
+broken into small chunks.  If the window is too large, then no changes
+will be easily detected because the difference between varying signals
+will appear large.  When windows are large, you also lose track about
+where correlation changes actually happen because the change point can
+be anywhere in the window.
+
+### Gamma
+
+Range: 0.1 - 10
+
+The Gamma value sets the decay rate for sample weights.  Bigger values
+will result in more data being included, which is good for smaller
+datasets.  If enough data is present, then low values should be used.
+
+### L1 regularization strength
+
+Range: 0 - 1.0
+
+Higher L1 values are better better for signals with rapid changes.
+
+### L2
+
+Better for smooth time series.  There is no current CLI option for this.
+
+# Correlation Explanation Methods
+
+Official implementation of linear correlation explanation (linear CorEx) and temporal correlation explanation (T-CorEx) methods.
+
+#### Linear CorEx
+Linear CorEx searches for independent latent factors that explain all correlations between observed variables, while also biasing
+the model selection towards modular latent factor models – directed latent factor graphical models
+where each observed variable has a single latent variable as its only parent.
+This is useful for covariance estimation, clustering related variables, and dimensionality reduction, especially in the high-dimensional and under-sampled regime.
+The complete description of the method is presented in NeurIPS 2019 [paper](https://papers.nips.cc/paper/9691-fast-structure-learning-with-modular-regularization) *"Fast structure learning with modular regularization"* by Greg Ver Steeg, Hrayr Harutyunyan, Daniel Moyer, and Aram Galstyan.
+If you want to cite this paper, please use the following BibTex entry:
+```text
+@incollection{NIPS2019_9691,
+title = {Fast structure learning with modular regularization},
+author = {Ver Steeg, Greg and Harutyunyan, Hrayr and Moyer, Daniel and Galstyan, Aram},
+booktitle = {Advances in Neural Information Processing Systems 32},
+editor = {H. Wallach and H. Larochelle and A. Beygelzimer and F. d\textquotesingle Alch\'{e}-Buc and E. Fox and R. Garnett},
+pages = {15567--15577},
+year = {2019},
+publisher = {Curran Associates, Inc.},
+url = {http://papers.nips.cc/paper/9691-fast-structure-learning-with-modular-regularization.pdf}
+}
+```
+
+**Note:** Greg Ver Steeg has an alternative implementation of linear CorEx, which is available at [github.com/gregversteeg/LinearCorex](https://github.com/gregversteeg/LinearCorex).
+That implementation uses a quazi-Newton optimization method for learning the model parameters. 
+In contrast, the implementation provided in this repository uses ADAM optimizer.
+This latter implementation utilizes GPUs better, and can converge to slightly better objective values if the input data is highly non-modular.
+Nevertheless, we highly encourage to take a look at the alternative implementation.
+
+#### T-CorEx
+T-CorEx is a method for covariance estimation from temporal data.
+It trains a linear CorEx for each time period,
+while employing two regularization techniques to enforce temporal consistency of estimates.
+The method is introduced in the [paper](https://arxiv.org/abs/1905.13276) *"Efficient Covariance Estimation from Temporal Data"* by Hrayr Harutunyan, Daniel Moyer, Hrant Khachatrian, Greg Ver Steeg, and Aram Galstyan.
+If you want to cite this paper, please use the following BibTex entry:
+```text
+@article{tcorex,
+  title={Efficient Covariance Estimation from Temporal Data},
+  author={Harutyunyan, Hrayr and Moyer, Daniel and Khachatrian, Hrant and Steeg, Greg Ver and Galstyan, Aram},
+  journal={arXiv preprint arXiv:1905.13276},
+  year={2019}
+}
+```
+
+
+Both linear CorEx and T-CorEx have linear time and memory complexity with respect to the number of observed variables and can be applied to high-dimensional datasets.
+For example, it takes less than an hour on a moderate PC to estimate the covariance structure for time series with 100K variables using T-CorEx.
+Both methods are implemented in PyTorch and can run on CPUs and GPUs.
+
+
+## Requirements and Installation
+The code is writen in Python 3, but should run on Python 2 as well.
+The dependencies are the following: 
+* numpy, scipy, tqdm, PyTorch
+* [optional] nibabel (for fMRI experiments)
+* [optional] nose (for tests)
+* [optional] sklearn, regain, TVGL, linearcorex, pandas (for running comparisions)
+* [optional] matplotlib and nilearn (for visualizations)
+
+To install the code, run the following command:
+```text
+python setup.py install
+```
+
+## Description
+The main method for linear CorEx is the class `tcorex.Corex`, and that of T-CorEx is 'tcorex.TCorex'.
+The complete description of parameters of these classes can be found in the corresponding docstrings.
+While there are many parameters (especially for T-CorEx), in general only a couple of them need to be tuned (others are set to their "best" values).
+Those parameters are:
+
+
+| Parameter | Linear CorEx | T-CorEx | Description |    
+|:---------|---|---|:---|   
+| `m` | + | + | The number of latent variables. Usually this is much smaller than the number of observed variables. |  
+| `l1` | - | + | A non-negative real number specifying the coefficient of l1 temporal regularization.|  
+| `gamma` | - | + | A real number in [0,1]. This argument controls the sample weights. The samples of time period t' will have weight w_t(t')=gamma^\|t' - t\| when estimating quantities for time period t. Smaller values are used for very dynamic time series.|  
+
+
+## Usage
+
+Run the following command for a sample run of TCorex. 
+```bash
+python -m examples.sample_run
+```
+
+The code is shown below:
+``` python 
+from __future__ import print_function
+from __future__ import absolute_import
+
+from tcorex.experiments.data import load_modular_sudden_change
+from tcorex.experiments import baselines
+from tcorex import base
+from tcorex import TCorex
+from tcorex import covariance as cov_utils
+
+import numpy as np
+import matplotlib
+matplotlib.use('agg')
+from matplotlib import pyplot as plt
+
+
+def main():
+    nv = 32         # number of observed variables
+    m = 4           # number of hidden variables
+    nt = 10         # number of time periods
+    train_cnt = 16  # number of training samples for each time period
+    val_cnt = 4     # number of validation samples for each time period
+
+    # Generate some data with a sudden change in the middle.
+    data, ground_truth_sigma = load_modular_sudden_change(nv=nv, m=m, nt=nt, ns=(train_cnt + val_cnt))
+
+    # Split it into train and validation.
+    train_data = [X[:train_cnt] for X in data]
+    val_data = [X[train_cnt:] for X in data]
+
+    # NOTE: the load_modular_sudden_change function above creates data where the time axis
+    # is already divided into time periods. If your data is not divided into time periods
+    # you can use the following procedure to do that:
+    # bucketed_data, index_to_bucket = make_buckets(data, window=train_cnt + val_cnt, stride='full')
+    # where the make_buckets function can be found at tcorex.experiments.data
+
+    # The core method we have is the tcorex.TCorex class.
+    tc = TCorex(nt=nt,
+                nv=nv,
+                n_hidden=m,
+                max_iter=500,
+                device='cpu',  # for GPU set 'cuda',
+                l1=0.3,        # coefficient of temporal regularization term
+                gamma=0.3,     # parameter that controls sample weights
+                verbose=1,     # 0, 1, 2
+                )
+
+    # Fit the parameters of T-CorEx.
+    tc.fit(train_data)
+
+    # We can compute the clusters of observed variables for each time period.
+    t = 8
+    clusters = tc.clusters()
+    print("Clusters at time period {}: {}".format(t, clusters[t]))
+
+    # We can get an estimate of the covariance matrix for each time period.
+    # When normed=True, estimates of the correlation matrices will be returned.
+    covs = tc.get_covariance()
+
+    # We can visualize the covariance matrices.
+    fig, ax = plt.subplots(1, figsize=(5, 5))
+    im = ax.imshow(covs[t])
+    fig.colorbar(im)
+    ax.set_title("Estimated covariance matrix\nat time period {}".format(t))
+    fig.savefig('covariance-matrix.png')
+
+    # It is usually useful to compute the inverse correlation matrices,
+    # since this matrices can be interpreted as adjacency matrices of
+    # Markov random fields.
+    cors = tc.get_covariance(normed=True)
+    inv_cors = [np.linalg.inv(x) for x in cors]
+
+    # We can visualize the thresholded inverse correlation matrices.
+    fig, ax = plt.subplots(1, figsize=(5, 5))
+    thresholded_inv_cor = np.abs(inv_cors[t]) > 0.05
+    ax.imshow(thresholded_inv_cor)
+    ax.set_title("Thresholded inverse correlation\nmatrix at time period {}".format(t))
+    fig.savefig('thresholded-inverse-correlation-matrix.png')
+
+    # We can also plot the Frobenius norm of the differences of inverse
+    # correlation matrices of  neighboring time periods. This is helpful
+    # for detecting the sudden change points of the system.
+    diffs = cov_utils.diffs(inv_cors)
+    fig, ax = plt.subplots(1, figsize=(5, 5))
+    ax.plot(diffs)
+    ax.set_xlabel('t')
+    ax.set_ylabel('$||\Sigma^{-1}_{t+1} - \Sigma^{-1}_{t}||_2$')
+    ax.set_title("Frobenius norms of differences between\ninverse correlation matrices")
+    fig.savefig('inv-correlation-difference-norms.png')
+
+    # We can also do grid search on a hyperparameter grid the following way.
+    # NOTE: this can take time!
+    baseline, grid = (baselines.TCorex(tcorex=TCorex, name='T-Corex'), {
+        'nv': nv,
+        'n_hidden': m,
+        'max_iter': 500,
+        'device': 'cpu',
+        'l1': [0.0, 0.03, 0.3, 3.0],
+        'gamma': [1e-6, 0.3, 0.5, 0.8]
+    })
+
+    best_score, best_params, best_covs, best_method, all_results = baseline.select(train_data, val_data, grid)
+    tc = best_method  # this is the model that performed the best on the validation data, you can use it as above
+    base.save(tc, 'best_method.pkl')
+
+
+if __name__ == '__main__':
+    main()
+```
+
+
```

### Comparing `gawseed-tcorex-1.1/README.md` & `gawseed_tcorex-1.1.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -25,14 +25,18 @@
 
 ```
 tcorex -w 30 -n 100 -w 30 -g .1 -l .5 input_data.csv output.pkl
 ```
 
 Discussion and help with selecting parameters is discussed below.
 
+The CSV file should have a header row, and the default columns to use
+are *timestamp*, *key* and *value* but may be changed with
+`--time-column`, `-k` and `-v`.
+
 ## Displaying results
 
 To list the correlations within each window, use
 `tcorex-changepoints` on the resulting pkl file:
 
 ```
 tcorex-changepoints output.pkl
@@ -74,23 +78,25 @@
 will be easily detected because the difference between varying signals
 will appear large.  When windows are large, you also lose track about
 where correlation changes actually happen because the change point can
 be anywhere in the window.
 
 ### Gamma
 
-Range: 0.1-10
+Range: 0.1 - 10
 
 The Gamma value sets the decay rate for sample weights.  Bigger values
 will result in more data being included, which is good for smaller
 datasets.  If enough data is present, then low values should be used.
 
 ### L1 regularization strength
 
-Higher L1 values are better better for signals with rapid changes
+Range: 0 - 1.0
+
+Higher L1 values are better better for signals with rapid changes.
 
 ### L2
 
 Better for smooth time series.  There is no current CLI option for this.
 
 # Correlation Explanation Methods
```

### Comparing `gawseed-tcorex-1.1/tcorex/base.py` & `gawseed_tcorex-1.1.1/gawseed_tcorex/base.py`

 * *Files identical despite different names*

### Comparing `gawseed-tcorex-1.1/tcorex/corex.py` & `gawseed_tcorex-1.1.1/gawseed_tcorex/corex.py`

 * *Files identical despite different names*

### Comparing `gawseed-tcorex-1.1/tcorex/covariance.py` & `gawseed_tcorex-1.1.1/gawseed_tcorex/covariance.py`

 * *Files identical despite different names*

### Comparing `gawseed-tcorex-1.1/tcorex/experiments/baselines.py` & `gawseed_tcorex-1.1.1/gawseed_tcorex/experiments/baselines.py`

 * *Files identical despite different names*

### Comparing `gawseed-tcorex-1.1/tcorex/experiments/data.py` & `gawseed_tcorex-1.1.1/gawseed_tcorex/experiments/data.py`

 * *Files identical despite different names*

### Comparing `gawseed-tcorex-1.1/tcorex/experiments/fmri_utils.py` & `gawseed_tcorex-1.1.1/gawseed_tcorex/experiments/fmri_utils.py`

 * *Files identical despite different names*

### Comparing `gawseed-tcorex-1.1/tcorex/experiments/vis_utils.py` & `gawseed_tcorex-1.1.1/gawseed_tcorex/experiments/vis_utils.py`

 * *Files identical despite different names*

### Comparing `gawseed-tcorex-1.1/tcorex/tcorex.py` & `gawseed_tcorex-1.1.1/gawseed_tcorex/tcorex.py`

 * *Files 0% similar despite different names*

```diff
@@ -49,15 +49,15 @@
                                      pretrained_weights=pretrained_weights, device=device, stopping_len=stopping_len,
                                      verbose=verbose, optimizer_class=optimizer_class,
                                      optimizer_params=optimizer_params)
         self.l1 = l1
         self.l2 = l2
         self.reg_type = reg_type
         self.init = init
-        self.gamma = np.float(gamma)
+        self.gamma = np.float32(gamma)
         self.max_sample_count = max_sample_cnt
         self.weighted_obj = weighted_obj
 
         # initialize later
         self.window_len = None
 
         # define the weights of the model
```

### Comparing `gawseed-tcorex-1.1/tcorex/tcorex_learnable.py` & `gawseed_tcorex-1.1.1/gawseed_tcorex/tcorex_learnable.py`

 * *Files identical despite different names*

### Comparing `gawseed-tcorex-1.1/tcorex/tools/tcorex_changepoints.py` & `gawseed_tcorex-1.1.1/gawseed_tcorex/tools/tcorex_changepoints.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,15 +42,15 @@
     columns = statistics['df.columns']
     df_index = pd.to_datetime(statistics['df.index'])
     time_delta = df_index[1] - df_index[0]
     nt = len(mis)
     m, nv = mis[0].shape
 
     for t in range(nt):
-        indices = np.zeros((nv,), dtype=np.bool)
+        indices = np.zeros((nv,), dtype=bool)
         for j in range(m):
             cur_topk = np.argsort(-mis[t][j])[:args.topk]
             for idx in cur_topk:
                 indices[idx] = True
         F = factorizations[t][:, indices]
         sigma = F.T.dot(F)
         cells = []
```

### Comparing `gawseed-tcorex-1.1/tcorex/tools/tcorex_cli.py` & `gawseed_tcorex-1.1.1/gawseed_tcorex/tools/tcorex_cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -81,15 +81,15 @@
 
     info("Saving to {}".format(args.output_path))
     pickle.dump(results, args.output_path)
 
 
 def run_tcorex(df, window_size, n_hidden, gamma, l1, max_iterations, device):
 
-    data = np.array(df).astype(np.float)
+    data = np.array(df).astype(np.float32)
 
     # standardize the data
     scaler = StandardScaler()
     data = scaler.fit_transform(data)
 
     # cut the tail for the data
     reminder = data.shape[0] % window_size
@@ -138,26 +138,24 @@
     df.index = pd.to_datetime(df.index, unit='s')
     min_gap = df.index[1] - df.index[0]
     for i in range(len(df.index) - 1):
         assert df.index[i] < df.index[i + 1]
         min_gap = min(min_gap, df.index[i + 1] - df.index[i])
 
     df = df.reindex(index=pd.date_range(df.index[0], df.index[-1],
-                                        freq=df.index[1] - df.index[0]),
-                    labels=time_column)
+                                        freq=df.index[1] - df.index[0]))
     df = df.fillna(0)
 
     return df
 
 
 def load_and_pivot_table(filename, time_column, key, value_column): 
     # load the data
     debug("Reading from {}".format(filename))
     df = pd.read_csv(filename,
                      dtype={'count': np.int32, 'timestamp': np.int32,
                             'key': str})
-    import pdb ; pdb.set_trace()
-    return pivot_table(df, key, value_column, time_column)
+    return pivot_table(df, time_column, key, value_column)
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `gawseed-tcorex-1.1/tcorex/tools/tcorex_plot.py` & `gawseed_tcorex-1.1.1/gawseed_tcorex/tools/tcorex_plot.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 """
 import pandas as pd
 import numpy as np
 import argparse
 import pickle
 import sys
 import os
-import tcorex.plot_utils
+import gawseed_tcorex.plot_utils
 from logging import info, debug, warn
 
 import matplotlib
 matplotlib.use('agg')
 from matplotlib import pyplot as plt
 import seaborn as sns
 sns.set_style("whitegrid")
@@ -32,15 +32,15 @@
     parser.add_argument('statistics_path', type=str,
                         help='path to a T-CorEx statistics file (output from tcorex)')
 
 
     args = parser.parse_args()
 
     # import needed modules from ml-tools
-    tcorex.plot_utils.set_style(plt)
+    gawseed.tcorex.plot_utils.set_style(plt)
 
     # import needed tools from T-CorEx code
     from tcorex.covariance import frob_diffs_given_factors
 
     # load the saved statistics
     with open(args.statistics_path, 'rb') as f:
         statistics = pickle.load(f)
```

