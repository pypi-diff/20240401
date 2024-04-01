# Comparing `tmp/pyerrors-2.8.2.tar.gz` & `tmp/pyerrors-2.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyerrors-2.8.2.tar", last modified: Fri Jun  2 14:10:51 2023, max compression
+gzip compressed data, was "pyerrors-2.9.0.tar", last modified: Thu Jul 20 10:49:12 2023, max compression
```

## Comparing `pyerrors-2.8.2.tar` & `pyerrors-2.9.0.tar`

### file list

```diff
@@ -1,118 +1,121 @@
-drwxrwxr-x   0 fjosw     (1000) fjosw     (1000)        0 2023-06-02 14:10:51.055575 pyerrors-2.8.2/
-drwxrwxr-x   0 fjosw     (1000) fjosw     (1000)        0 2023-06-02 14:10:51.039575 pyerrors-2.8.2/.github/
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)      113 2023-03-21 12:48:56.000000 pyerrors-2.8.2/.github/CODEOWNERS
-drwxrwxr-x   0 fjosw     (1000) fjosw     (1000)        0 2023-06-02 14:10:51.039575 pyerrors-2.8.2/.github/ISSUE_TEMPLATE/
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     1051 2023-03-21 12:48:56.000000 pyerrors-2.8.2/.github/ISSUE_TEMPLATE/bug-report.yml
-drwxrwxr-x   0 fjosw     (1000) fjosw     (1000)        0 2023-06-02 14:10:51.039575 pyerrors-2.8.2/.github/workflows/
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)      386 2023-03-21 12:48:56.000000 pyerrors-2.8.2/.github/workflows/binder.yml
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)      737 2023-03-21 12:48:56.000000 pyerrors-2.8.2/.github/workflows/codeql.yml
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     1012 2023-03-21 12:48:56.000000 pyerrors-2.8.2/.github/workflows/docs.yml
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     1022 2023-03-21 12:48:56.000000 pyerrors-2.8.2/.github/workflows/examples.yml
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)      547 2023-03-21 12:48:56.000000 pyerrors-2.8.2/.github/workflows/flake8.yml
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     1043 2023-06-02 14:05:30.000000 pyerrors-2.8.2/.github/workflows/pytest.yml
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)      211 2023-03-21 12:48:56.000000 pyerrors-2.8.2/.gitignore
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)    16879 2023-06-02 14:06:35.000000 pyerrors-2.8.2/CHANGELOG.md
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     1278 2023-06-02 10:22:14.000000 pyerrors-2.8.2/CITATION.cff
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     1842 2023-03-21 12:48:56.000000 pyerrors-2.8.2/CONTRIBUTING.md
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     1070 2023-03-11 21:38:08.000000 pyerrors-2.8.2/LICENSE
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     2705 2023-06-02 14:10:51.055575 pyerrors-2.8.2/PKG-INFO
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     1610 2023-06-02 14:05:30.000000 pyerrors-2.8.2/README.md
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)        0 2023-03-11 21:38:08.000000 pyerrors-2.8.2/conftest.py
-drwxrwxr-x   0 fjosw     (1000) fjosw     (1000)        0 2023-06-02 14:10:51.043575 pyerrors-2.8.2/examples/
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)    87858 2023-03-21 12:48:56.000000 pyerrors-2.8.2/examples/01_basic_example.ipynb
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)    62623 2023-03-21 12:48:56.000000 pyerrors-2.8.2/examples/02_correlators.ipynb
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)    97653 2023-03-21 12:48:56.000000 pyerrors-2.8.2/examples/03_pcac_example.ipynb
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)   129847 2023-03-21 12:48:56.000000 pyerrors-2.8.2/examples/04_fit_example.ipynb
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     9053 2023-03-11 21:38:08.000000 pyerrors-2.8.2/examples/05_matrix_operations.ipynb
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)    30851 2023-03-21 12:48:56.000000 pyerrors-2.8.2/examples/06_gevp.ipynb
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)    10604 2023-03-21 12:48:56.000000 pyerrors-2.8.2/examples/07_data_management.ipynb
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)    21826 2023-03-21 12:48:56.000000 pyerrors-2.8.2/examples/08_combined_fit_example.ipynb
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)      757 2023-03-11 21:38:08.000000 pyerrors-2.8.2/examples/base_style.mplstyle
-drwxrwxr-x   0 fjosw     (1000) fjosw     (1000)        0 2023-06-02 14:10:51.047575 pyerrors-2.8.2/examples/data/
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     7407 2023-03-11 21:38:08.000000 pyerrors-2.8.2/examples/data/correlator_test.json.gz
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)    15009 2023-03-11 21:38:08.000000 pyerrors-2.8.2/examples/data/f_A.json.gz
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)    15072 2023-03-11 21:38:08.000000 pyerrors-2.8.2/examples/data/f_P.json.gz
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)   266539 2023-03-11 21:38:08.000000 pyerrors-2.8.2/examples/data/matrix_correlator.json.gz
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)   266778 2023-03-11 21:38:08.000000 pyerrors-2.8.2/examples/data/matrix_correlator_V1V1.json.gz
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)   266803 2023-03-11 21:38:08.000000 pyerrors-2.8.2/examples/data/matrix_correlator_V2V2.json.gz
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)   266702 2023-03-11 21:38:08.000000 pyerrors-2.8.2/examples/data/matrix_correlator_V3V3.json.gz
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     8575 2023-03-11 21:38:08.000000 pyerrors-2.8.2/examples/json_schema.json
-drwxrwxr-x   0 fjosw     (1000) fjosw     (1000)        0 2023-06-02 14:10:51.047575 pyerrors-2.8.2/pyerrors/
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)    29950 2023-06-02 10:22:14.000000 pyerrors-2.8.2/pyerrors/__init__.py
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)    57481 2023-06-02 10:22:14.000000 pyerrors-2.8.2/pyerrors/correlators.py
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     3609 2023-06-02 10:22:14.000000 pyerrors-2.8.2/pyerrors/covobs.py
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     2909 2023-03-21 12:48:56.000000 pyerrors-2.8.2/pyerrors/dirac.py
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)    30996 2023-03-21 12:48:56.000000 pyerrors-2.8.2/pyerrors/fits.py
-drwxrwxr-x   0 fjosw     (1000) fjosw     (1000)        0 2023-06-02 14:10:51.051575 pyerrors-2.8.2/pyerrors/input/
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)      579 2023-06-02 10:22:14.000000 pyerrors-2.8.2/pyerrors/input/__init__.py
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)    25145 2023-03-21 12:48:56.000000 pyerrors-2.8.2/pyerrors/input/bdio.py
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)    30920 2023-06-02 10:22:14.000000 pyerrors-2.8.2/pyerrors/input/dobs.py
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)    19262 2023-06-02 10:22:14.000000 pyerrors-2.8.2/pyerrors/input/hadrons.py
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)    26602 2023-06-02 10:22:14.000000 pyerrors-2.8.2/pyerrors/input/json.py
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     8064 2023-06-02 10:22:14.000000 pyerrors-2.8.2/pyerrors/input/misc.py
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)    50595 2023-06-02 10:22:14.000000 pyerrors-2.8.2/pyerrors/input/openQCD.py
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     6691 2023-06-02 10:22:14.000000 pyerrors-2.8.2/pyerrors/input/pandas.py
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)    16290 2023-06-01 13:18:57.000000 pyerrors-2.8.2/pyerrors/input/sfcf.py
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     2257 2023-06-02 10:22:14.000000 pyerrors-2.8.2/pyerrors/input/utils.py
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)    10177 2023-03-11 21:38:08.000000 pyerrors-2.8.2/pyerrors/linalg.py
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     5381 2023-03-21 12:48:56.000000 pyerrors-2.8.2/pyerrors/misc.py
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     2273 2023-03-21 12:48:56.000000 pyerrors-2.8.2/pyerrors/mpm.py
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)    67936 2023-06-02 14:05:35.000000 pyerrors-2.8.2/pyerrors/obs.py
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     1466 2023-03-21 12:48:56.000000 pyerrors-2.8.2/pyerrors/roots.py
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)       22 2023-06-02 14:06:00.000000 pyerrors-2.8.2/pyerrors/version.py
-drwxrwxr-x   0 fjosw     (1000) fjosw     (1000)        0 2023-06-02 14:10:51.047575 pyerrors-2.8.2/pyerrors.egg-info/
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     2705 2023-06-02 14:10:51.000000 pyerrors-2.8.2/pyerrors.egg-info/PKG-INFO
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     2700 2023-06-02 14:10:51.000000 pyerrors-2.8.2/pyerrors.egg-info/SOURCES.txt
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)        1 2023-06-02 14:10:51.000000 pyerrors-2.8.2/pyerrors.egg-info/dependency_links.txt
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)      202 2023-06-02 14:10:51.000000 pyerrors-2.8.2/pyerrors.egg-info/requires.txt
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)        9 2023-06-02 14:10:51.000000 pyerrors-2.8.2/pyerrors.egg-info/top_level.txt
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)      100 2023-03-21 12:48:56.000000 pyerrors-2.8.2/pyproject.toml
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)       38 2023-06-02 14:10:51.055575 pyerrors-2.8.2/setup.cfg
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     1888 2023-06-02 14:05:30.000000 pyerrors-2.8.2/setup.py
-drwxrwxr-x   0 fjosw     (1000) fjosw     (1000)        0 2023-06-02 14:10:51.051575 pyerrors-2.8.2/tests/
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     1159 2023-03-11 21:38:08.000000 pyerrors-2.8.2/tests/benchmark_test.py
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)    17752 2023-03-21 12:48:56.000000 pyerrors-2.8.2/tests/correlators_test.py
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     3470 2023-03-11 21:38:08.000000 pyerrors-2.8.2/tests/covobs_test.py
-drwxrwxr-x   0 fjosw     (1000) fjosw     (1000)        0 2023-06-02 14:10:51.039575 pyerrors-2.8.2/tests/data/
-drwxrwxr-x   0 fjosw     (1000) fjosw     (1000)        0 2023-06-02 14:10:51.055575 pyerrors-2.8.2/tests/data/openqcd_test/
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)    38800 2023-03-21 12:48:56.000000 pyerrors-2.8.2/tests/data/openqcd_test/ms5_xsf_T24L16r1.ms5_xsf_dd.dat
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)    38800 2023-03-21 12:48:56.000000 pyerrors-2.8.2/tests/data/openqcd_test/ms5_xsf_T24L16r2.ms5_xsf_dd.dat
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)    38800 2023-03-21 12:48:56.000000 pyerrors-2.8.2/tests/data/openqcd_test/ms5_xsf_T24L16r3.ms5_xsf_dd.dat
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)    87320 2023-03-11 21:38:08.000000 pyerrors-2.8.2/tests/data/openqcd_test/openqcd2r1.ms.dat
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     2076 2023-03-11 21:38:08.000000 pyerrors-2.8.2/tests/data/openqcd_test/openqcd2r1.ms1.dat
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)   157504 2023-03-11 21:38:08.000000 pyerrors-2.8.2/tests/data/openqcd_test/sfqcdr1.gfms.dat
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)      252 2023-03-11 21:38:08.000000 pyerrors-2.8.2/tests/data/openqcd_test/sfqcdr1.rwms.dat
-drwxrwxr-x   0 fjosw     (1000) fjosw     (1000)        0 2023-06-02 14:10:51.039575 pyerrors-2.8.2/tests/data/sfcf_test/
-drwxrwxr-x   0 fjosw     (1000) fjosw     (1000)        0 2023-06-02 14:10:51.039575 pyerrors-2.8.2/tests/data/sfcf_test/broken_data_c/
-drwxrwxr-x   0 fjosw     (1000) fjosw     (1000)        0 2023-06-02 14:10:51.055575 pyerrors-2.8.2/tests/data/sfcf_test/broken_data_c/data_c_r0/
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     8712 2023-03-21 12:48:56.000000 pyerrors-2.8.2/tests/data/sfcf_test/broken_data_c/data_c_r0/data_c_r0_n1
-drwxrwxr-x   0 fjosw     (1000) fjosw     (1000)        0 2023-06-02 14:10:51.055575 pyerrors-2.8.2/tests/data/sfcf_test/data_a/
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)    24665 2023-03-11 21:38:08.000000 pyerrors-2.8.2/tests/data/sfcf_test/data_a/data_a_r0.F_V0
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)    14670 2023-03-11 21:38:08.000000 pyerrors-2.8.2/tests/data/sfcf_test/data_a/data_a_r0.f_1
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     9090 2023-03-11 21:38:08.000000 pyerrors-2.8.2/tests/data/sfcf_test/data_a/data_a_r0.f_A
-drwxrwxr-x   0 fjosw     (1000) fjosw     (1000)        0 2023-06-02 14:10:51.039575 pyerrors-2.8.2/tests/data/sfcf_test/data_c/
-drwxrwxr-x   0 fjosw     (1000) fjosw     (1000)        0 2023-06-02 14:10:51.055575 pyerrors-2.8.2/tests/data/sfcf_test/data_c/data_c_r0/
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     8918 2023-03-11 21:38:08.000000 pyerrors-2.8.2/tests/data/sfcf_test/data_c/data_c_r0/data_c_r0_n1
-drwxrwxr-x   0 fjosw     (1000) fjosw     (1000)        0 2023-06-02 14:10:51.039575 pyerrors-2.8.2/tests/data/sfcf_test/data_o/
-drwxrwxr-x   0 fjosw     (1000) fjosw     (1000)        0 2023-06-02 14:10:51.039575 pyerrors-2.8.2/tests/data/sfcf_test/data_o/test_r0/
-drwxrwxr-x   0 fjosw     (1000) fjosw     (1000)        0 2023-06-02 14:10:51.055575 pyerrors-2.8.2/tests/data/sfcf_test/data_o/test_r0/cfg1/
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     4926 2023-03-11 21:38:08.000000 pyerrors-2.8.2/tests/data/sfcf_test/data_o/test_r0/cfg1/F_V0
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     2927 2023-03-11 21:38:08.000000 pyerrors-2.8.2/tests/data/sfcf_test/data_o/test_r0/cfg1/f_1
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     1811 2023-03-11 21:38:08.000000 pyerrors-2.8.2/tests/data/sfcf_test/data_o/test_r0/cfg1/f_A
-drwxrwxr-x   0 fjosw     (1000) fjosw     (1000)        0 2023-06-02 14:10:51.055575 pyerrors-2.8.2/tests/data/sfcf_test/param/
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)   142045 2023-03-11 21:38:08.000000 pyerrors-2.8.2/tests/data/sfcf_test/param/out.out
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     1661 2023-03-11 21:38:08.000000 pyerrors-2.8.2/tests/data/sfcf_test/param/parameters_a
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     1661 2023-03-11 21:38:08.000000 pyerrors-2.8.2/tests/data/sfcf_test/param/parameters_c
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     1661 2023-03-11 21:38:08.000000 pyerrors-2.8.2/tests/data/sfcf_test/param/parameters_o
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     1885 2023-03-11 21:38:08.000000 pyerrors-2.8.2/tests/dirac_test.py
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)    44785 2023-03-21 12:48:56.000000 pyerrors-2.8.2/tests/fits_test.py
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)    15556 2023-06-02 10:22:14.000000 pyerrors-2.8.2/tests/json_io_test.py
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)    14226 2023-03-21 12:48:56.000000 pyerrors-2.8.2/tests/linalg_test.py
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)      543 2023-03-21 12:48:56.000000 pyerrors-2.8.2/tests/misc_test.py
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)      314 2023-03-11 21:38:08.000000 pyerrors-2.8.2/tests/mpm_test.py
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)    46473 2023-06-02 14:05:35.000000 pyerrors-2.8.2/tests/obs_test.py
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     9253 2023-06-02 10:22:14.000000 pyerrors-2.8.2/tests/openQCD_in_test.py
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)    11768 2023-06-02 14:05:30.000000 pyerrors-2.8.2/tests/pandas_test.py
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     1262 2023-03-21 12:48:56.000000 pyerrors-2.8.2/tests/roots_test.py
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     6431 2023-06-01 13:14:45.000000 pyerrors-2.8.2/tests/sfcf_in_test.py
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     1415 2023-06-02 10:22:14.000000 pyerrors-2.8.2/tests/utils_in_test.py
+drwxrwxr-x   0 fjosw     (1000) fjosw     (1000)        0 2023-07-20 10:49:12.652145 pyerrors-2.9.0/
+drwxrwxr-x   0 fjosw     (1000) fjosw     (1000)        0 2023-07-20 10:49:12.640144 pyerrors-2.9.0/.github/
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)      113 2023-03-21 12:48:56.000000 pyerrors-2.9.0/.github/CODEOWNERS
+drwxrwxr-x   0 fjosw     (1000) fjosw     (1000)        0 2023-07-20 10:49:12.640144 pyerrors-2.9.0/.github/ISSUE_TEMPLATE/
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     1051 2023-07-14 08:50:25.000000 pyerrors-2.9.0/.github/ISSUE_TEMPLATE/bug-report.yml
+drwxrwxr-x   0 fjosw     (1000) fjosw     (1000)        0 2023-07-20 10:49:12.640144 pyerrors-2.9.0/.github/workflows/
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)      386 2023-03-21 12:48:56.000000 pyerrors-2.9.0/.github/workflows/binder.yml
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)      737 2023-03-21 12:48:56.000000 pyerrors-2.9.0/.github/workflows/codeql.yml
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     1012 2023-03-21 12:48:56.000000 pyerrors-2.9.0/.github/workflows/docs.yml
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     1022 2023-07-14 08:50:25.000000 pyerrors-2.9.0/.github/workflows/examples.yml
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)      547 2023-07-14 08:50:25.000000 pyerrors-2.9.0/.github/workflows/flake8.yml
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)      984 2023-07-20 10:42:21.000000 pyerrors-2.9.0/.github/workflows/pytest.yml
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)      211 2023-07-14 08:50:25.000000 pyerrors-2.9.0/.gitignore
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)    17449 2023-07-20 10:42:21.000000 pyerrors-2.9.0/CHANGELOG.md
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     1278 2023-07-14 08:50:25.000000 pyerrors-2.9.0/CITATION.cff
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     1913 2023-07-20 10:42:21.000000 pyerrors-2.9.0/CONTRIBUTING.md
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     1070 2023-03-11 21:38:08.000000 pyerrors-2.9.0/LICENSE
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     3555 2023-07-20 10:49:12.652145 pyerrors-2.9.0/PKG-INFO
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     2510 2023-07-20 10:42:21.000000 pyerrors-2.9.0/README.md
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)        0 2023-03-11 21:38:08.000000 pyerrors-2.9.0/conftest.py
+drwxrwxr-x   0 fjosw     (1000) fjosw     (1000)        0 2023-07-20 10:49:12.640144 pyerrors-2.9.0/examples/
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)    87858 2023-03-21 12:48:56.000000 pyerrors-2.9.0/examples/01_basic_example.ipynb
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)    62623 2023-03-21 12:48:56.000000 pyerrors-2.9.0/examples/02_correlators.ipynb
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)    97653 2023-03-21 12:48:56.000000 pyerrors-2.9.0/examples/03_pcac_example.ipynb
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)   129847 2023-03-21 12:48:56.000000 pyerrors-2.9.0/examples/04_fit_example.ipynb
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     8399 2023-07-20 10:42:21.000000 pyerrors-2.9.0/examples/05_matrix_operations.ipynb
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)    30851 2023-03-21 12:48:56.000000 pyerrors-2.9.0/examples/06_gevp.ipynb
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)    10604 2023-03-21 12:48:56.000000 pyerrors-2.9.0/examples/07_data_management.ipynb
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)    21826 2023-07-14 08:50:25.000000 pyerrors-2.9.0/examples/08_combined_fit_example.ipynb
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)      757 2023-03-11 21:38:08.000000 pyerrors-2.9.0/examples/base_style.mplstyle
+drwxrwxr-x   0 fjosw     (1000) fjosw     (1000)        0 2023-07-20 10:49:12.644144 pyerrors-2.9.0/examples/data/
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     7407 2023-03-11 21:38:08.000000 pyerrors-2.9.0/examples/data/correlator_test.json.gz
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)    15009 2023-03-11 21:38:08.000000 pyerrors-2.9.0/examples/data/f_A.json.gz
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)    15072 2023-03-11 21:38:08.000000 pyerrors-2.9.0/examples/data/f_P.json.gz
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)   266539 2023-03-11 21:38:08.000000 pyerrors-2.9.0/examples/data/matrix_correlator.json.gz
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)   266778 2023-03-11 21:38:08.000000 pyerrors-2.9.0/examples/data/matrix_correlator_V1V1.json.gz
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)   266803 2023-03-11 21:38:08.000000 pyerrors-2.9.0/examples/data/matrix_correlator_V2V2.json.gz
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)   266702 2023-03-11 21:38:08.000000 pyerrors-2.9.0/examples/data/matrix_correlator_V3V3.json.gz
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     8575 2023-03-11 21:38:08.000000 pyerrors-2.9.0/examples/json_schema.json
+drwxrwxr-x   0 fjosw     (1000) fjosw     (1000)        0 2023-07-20 10:49:12.644144 pyerrors-2.9.0/pyerrors/
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)    30245 2023-07-20 10:42:21.000000 pyerrors-2.9.0/pyerrors/__init__.py
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)    62136 2023-07-20 10:42:21.000000 pyerrors-2.9.0/pyerrors/correlators.py
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     3609 2023-07-14 08:50:25.000000 pyerrors-2.9.0/pyerrors/covobs.py
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     2909 2023-03-21 12:48:56.000000 pyerrors-2.9.0/pyerrors/dirac.py
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)    31388 2023-07-20 10:42:21.000000 pyerrors-2.9.0/pyerrors/fits.py
+drwxrwxr-x   0 fjosw     (1000) fjosw     (1000)        0 2023-07-20 10:49:12.644144 pyerrors-2.9.0/pyerrors/input/
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)      579 2023-07-14 08:50:25.000000 pyerrors-2.9.0/pyerrors/input/__init__.py
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)    25145 2023-03-21 12:48:56.000000 pyerrors-2.9.0/pyerrors/input/bdio.py
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)    30920 2023-07-14 08:50:25.000000 pyerrors-2.9.0/pyerrors/input/dobs.py
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)    21402 2023-07-20 10:42:21.000000 pyerrors-2.9.0/pyerrors/input/hadrons.py
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)    26602 2023-07-14 08:50:25.000000 pyerrors-2.9.0/pyerrors/input/json.py
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     8064 2023-07-14 08:50:25.000000 pyerrors-2.9.0/pyerrors/input/misc.py
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)    50595 2023-07-14 08:50:25.000000 pyerrors-2.9.0/pyerrors/input/openQCD.py
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     6691 2023-07-14 08:50:25.000000 pyerrors-2.9.0/pyerrors/input/pandas.py
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)    16329 2023-07-20 10:42:21.000000 pyerrors-2.9.0/pyerrors/input/sfcf.py
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     2257 2023-07-14 08:50:25.000000 pyerrors-2.9.0/pyerrors/input/utils.py
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     2962 2023-07-20 10:42:21.000000 pyerrors-2.9.0/pyerrors/integrate.py
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)    10177 2023-06-21 09:05:46.000000 pyerrors-2.9.0/pyerrors/linalg.py
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     5381 2023-07-14 08:50:25.000000 pyerrors-2.9.0/pyerrors/misc.py
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     2273 2023-03-21 12:48:56.000000 pyerrors-2.9.0/pyerrors/mpm.py
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)    71601 2023-07-20 10:42:21.000000 pyerrors-2.9.0/pyerrors/obs.py
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     1466 2023-03-21 12:48:56.000000 pyerrors-2.9.0/pyerrors/roots.py
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)       22 2023-07-20 10:42:21.000000 pyerrors-2.9.0/pyerrors/version.py
+drwxrwxr-x   0 fjosw     (1000) fjosw     (1000)        0 2023-07-20 10:49:12.644144 pyerrors-2.9.0/pyerrors.egg-info/
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     3555 2023-07-20 10:49:12.000000 pyerrors-2.9.0/pyerrors.egg-info/PKG-INFO
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     2784 2023-07-20 10:49:12.000000 pyerrors-2.9.0/pyerrors.egg-info/SOURCES.txt
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)        1 2023-07-20 10:49:12.000000 pyerrors-2.9.0/pyerrors.egg-info/dependency_links.txt
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)      214 2023-07-20 10:49:12.000000 pyerrors-2.9.0/pyerrors.egg-info/requires.txt
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)        9 2023-07-20 10:49:12.000000 pyerrors-2.9.0/pyerrors.egg-info/top_level.txt
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)      100 2023-03-21 12:48:56.000000 pyerrors-2.9.0/pyproject.toml
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)       38 2023-07-20 10:49:12.652145 pyerrors-2.9.0/setup.cfg
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     1855 2023-07-20 10:42:21.000000 pyerrors-2.9.0/setup.py
+drwxrwxr-x   0 fjosw     (1000) fjosw     (1000)        0 2023-07-20 10:49:12.648145 pyerrors-2.9.0/tests/
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     1159 2023-03-11 21:38:08.000000 pyerrors-2.9.0/tests/benchmark_test.py
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)    23385 2023-07-20 10:42:21.000000 pyerrors-2.9.0/tests/correlators_test.py
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     3470 2023-03-11 21:38:08.000000 pyerrors-2.9.0/tests/covobs_test.py
+drwxrwxr-x   0 fjosw     (1000) fjosw     (1000)        0 2023-07-20 10:49:12.648145 pyerrors-2.9.0/tests/data/
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)    49713 2023-07-14 08:50:25.000000 pyerrors-2.9.0/tests/data/compute_drho_fails.json.gz
+drwxrwxr-x   0 fjosw     (1000) fjosw     (1000)        0 2023-07-20 10:49:12.648145 pyerrors-2.9.0/tests/data/openqcd_test/
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)    38800 2023-07-14 08:50:25.000000 pyerrors-2.9.0/tests/data/openqcd_test/ms5_xsf_T24L16r1.ms5_xsf_dd.dat
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)    38800 2023-07-14 08:50:25.000000 pyerrors-2.9.0/tests/data/openqcd_test/ms5_xsf_T24L16r2.ms5_xsf_dd.dat
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)    38800 2023-07-14 08:50:25.000000 pyerrors-2.9.0/tests/data/openqcd_test/ms5_xsf_T24L16r3.ms5_xsf_dd.dat
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)    87320 2023-03-11 21:38:08.000000 pyerrors-2.9.0/tests/data/openqcd_test/openqcd2r1.ms.dat
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     2076 2023-03-11 21:38:08.000000 pyerrors-2.9.0/tests/data/openqcd_test/openqcd2r1.ms1.dat
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)   157504 2023-03-11 21:38:08.000000 pyerrors-2.9.0/tests/data/openqcd_test/sfqcdr1.gfms.dat
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)      252 2023-03-11 21:38:08.000000 pyerrors-2.9.0/tests/data/openqcd_test/sfqcdr1.rwms.dat
+drwxrwxr-x   0 fjosw     (1000) fjosw     (1000)        0 2023-07-20 10:49:12.636144 pyerrors-2.9.0/tests/data/sfcf_test/
+drwxrwxr-x   0 fjosw     (1000) fjosw     (1000)        0 2023-07-20 10:49:12.636144 pyerrors-2.9.0/tests/data/sfcf_test/broken_data_c/
+drwxrwxr-x   0 fjosw     (1000) fjosw     (1000)        0 2023-07-20 10:49:12.648145 pyerrors-2.9.0/tests/data/sfcf_test/broken_data_c/data_c_r0/
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     8712 2023-07-14 08:50:25.000000 pyerrors-2.9.0/tests/data/sfcf_test/broken_data_c/data_c_r0/data_c_r0_n1
+drwxrwxr-x   0 fjosw     (1000) fjosw     (1000)        0 2023-07-20 10:49:12.648145 pyerrors-2.9.0/tests/data/sfcf_test/data_a/
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)    24665 2023-03-11 21:38:08.000000 pyerrors-2.9.0/tests/data/sfcf_test/data_a/data_a_r0.F_V0
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)    14670 2023-03-11 21:38:08.000000 pyerrors-2.9.0/tests/data/sfcf_test/data_a/data_a_r0.f_1
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     9090 2023-03-11 21:38:08.000000 pyerrors-2.9.0/tests/data/sfcf_test/data_a/data_a_r0.f_A
+drwxrwxr-x   0 fjosw     (1000) fjosw     (1000)        0 2023-07-20 10:49:12.636144 pyerrors-2.9.0/tests/data/sfcf_test/data_c/
+drwxrwxr-x   0 fjosw     (1000) fjosw     (1000)        0 2023-07-20 10:49:12.648145 pyerrors-2.9.0/tests/data/sfcf_test/data_c/data_c_r0/
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     8918 2023-03-11 21:38:08.000000 pyerrors-2.9.0/tests/data/sfcf_test/data_c/data_c_r0/data_c_r0_n1
+drwxrwxr-x   0 fjosw     (1000) fjosw     (1000)        0 2023-07-20 10:49:12.636144 pyerrors-2.9.0/tests/data/sfcf_test/data_o/
+drwxrwxr-x   0 fjosw     (1000) fjosw     (1000)        0 2023-07-20 10:49:12.636144 pyerrors-2.9.0/tests/data/sfcf_test/data_o/test_r0/
+drwxrwxr-x   0 fjosw     (1000) fjosw     (1000)        0 2023-07-20 10:49:12.648145 pyerrors-2.9.0/tests/data/sfcf_test/data_o/test_r0/cfg1/
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     4926 2023-03-11 21:38:08.000000 pyerrors-2.9.0/tests/data/sfcf_test/data_o/test_r0/cfg1/F_V0
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     2927 2023-03-11 21:38:08.000000 pyerrors-2.9.0/tests/data/sfcf_test/data_o/test_r0/cfg1/f_1
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     1811 2023-03-11 21:38:08.000000 pyerrors-2.9.0/tests/data/sfcf_test/data_o/test_r0/cfg1/f_A
+drwxrwxr-x   0 fjosw     (1000) fjosw     (1000)        0 2023-07-20 10:49:12.652145 pyerrors-2.9.0/tests/data/sfcf_test/param/
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)   142045 2023-03-11 21:38:08.000000 pyerrors-2.9.0/tests/data/sfcf_test/param/out.out
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     1661 2023-03-11 21:38:08.000000 pyerrors-2.9.0/tests/data/sfcf_test/param/parameters_a
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     1661 2023-03-11 21:38:08.000000 pyerrors-2.9.0/tests/data/sfcf_test/param/parameters_c
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     1661 2023-03-11 21:38:08.000000 pyerrors-2.9.0/tests/data/sfcf_test/param/parameters_o
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     1885 2023-03-11 21:38:08.000000 pyerrors-2.9.0/tests/dirac_test.py
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)    45426 2023-07-20 10:42:21.000000 pyerrors-2.9.0/tests/fits_test.py
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     1625 2023-07-20 10:42:21.000000 pyerrors-2.9.0/tests/integrate_test.py
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)    15556 2023-07-14 08:50:25.000000 pyerrors-2.9.0/tests/json_io_test.py
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)    14226 2023-07-20 10:42:21.000000 pyerrors-2.9.0/tests/linalg_test.py
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)      592 2023-07-20 10:42:21.000000 pyerrors-2.9.0/tests/misc_test.py
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)      314 2023-06-21 09:05:46.000000 pyerrors-2.9.0/tests/mpm_test.py
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)    47863 2023-07-20 10:42:21.000000 pyerrors-2.9.0/tests/obs_test.py
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     9253 2023-07-14 08:50:25.000000 pyerrors-2.9.0/tests/openQCD_in_test.py
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)    11681 2023-07-20 10:42:21.000000 pyerrors-2.9.0/tests/pandas_test.py
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     1262 2023-03-21 12:48:56.000000 pyerrors-2.9.0/tests/roots_test.py
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     6431 2023-07-14 08:50:25.000000 pyerrors-2.9.0/tests/sfcf_in_test.py
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     1415 2023-07-14 08:50:25.000000 pyerrors-2.9.0/tests/utils_in_test.py
```

### Comparing `pyerrors-2.8.2/.github/ISSUE_TEMPLATE/bug-report.yml` & `pyerrors-2.9.0/.github/ISSUE_TEMPLATE/bug-report.yml`

 * *Files identical despite different names*

### Comparing `pyerrors-2.8.2/.github/workflows/codeql.yml` & `pyerrors-2.9.0/.github/workflows/codeql.yml`

 * *Files identical despite different names*

### Comparing `pyerrors-2.8.2/.github/workflows/docs.yml` & `pyerrors-2.9.0/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `pyerrors-2.8.2/.github/workflows/examples.yml` & `pyerrors-2.9.0/.github/workflows/examples.yml`

 * *Files identical despite different names*

### Comparing `pyerrors-2.8.2/.github/workflows/flake8.yml` & `pyerrors-2.9.0/.github/workflows/flake8.yml`

 * *Files identical despite different names*

### Comparing `pyerrors-2.8.2/.github/workflows/pytest.yml` & `pyerrors-2.9.0/.github/workflows/pytest.yml`

 * *Files 6% similar despite different names*

```diff
@@ -12,20 +12,18 @@
 jobs:
   pytest:
     runs-on: ${{ matrix.os }}
     strategy:
       fail-fast: false
       matrix:
         os: [ubuntu-latest]
-        python-version: ["3.7", "3.8", "3.9", "3.10", "3.11"]
+        python-version: ["3.8", "3.9", "3.10", "3.11"]
         include:
           - os: macos-latest
-            python-version: 3.9
-          - os: windows-latest
-            python-version: 3.9
+            python-version: "3.10"
 
     steps:
       - name: Checkout source
         uses: actions/checkout@v3
 
       - name: Setup python
         uses: actions/setup-python@v4
@@ -41,8 +39,8 @@
           pip install pytest-cov
           pip install pytest-benchmark
           pip install hypothesis
           pip install py
           pip freeze
 
       - name: Run tests
-        run: pytest --cov=pyerrors -vv
+        run: pytest --cov=pyerrors -vv -Werror
```

### Comparing `pyerrors-2.8.2/CHANGELOG.md` & `pyerrors-2.9.0/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,27 @@
 # Changelog
 
 All notable changes to this project will be documented in this file.
 
+## [2.9.0] - 2023-07-20
+### Added
+- Vectorized `gamma_method` added which can be applied to lists or arrays of pyerrors objects.
+- Wrapper for numerical integration of `Obs` valued functions with `Obs` valued intervals.
+- Bootstrap import and export added.
+- `matmul` overloaded for `Corr` class.
+- More options for initializing `Corr` objects added.
+- General Hadrons hdf5 reader added.
+- New variant of second_derivative.
+- CObs formatting added.
+- Comparisons for `Corr` class added.
+
+### Changed
+- support for python<3.8 was dropped and dependencies were updated.
+
+
 ## [2.8.2] - 2023-06-02
 ### Fixed
 - Another bug appearing in an edge case of `_compute_drho` fixed.
 
 ## [2.8.1] - 2023-06-01
 ### Fixed
 - `input.pandas` can now deal with columns that only have `None` entries.
```

### Comparing `pyerrors-2.8.2/CITATION.cff` & `pyerrors-2.9.0/CITATION.cff`

 * *Files identical despite different names*

### Comparing `pyerrors-2.8.2/CONTRIBUTING.md` & `pyerrors-2.9.0/CONTRIBUTING.md`

 * *Files 9% similar despite different names*

```diff
@@ -15,23 +15,21 @@
 After committing your changes please send a pull requests to the `develop` branch. A guide on how to create a pull request can be found [here](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/proposing-changes-to-your-work-with-pull-requests/creating-a-pull-request).
 
 ### Documentation
 Please add docstrings to any new function, class or method you implement. The documentation is automatically generated from these docstrings. We follow the [numpydoc style](https://numpydoc.readthedocs.io/en/latest/format.html) for docstrings. The startpage of the documentation is generated from the docstring of `pyerrors/__init__.py`.
 
 ### Tests
 When implementing a new feature or fixing a bug please add meaningful tests to the files in the `tests` directory which cover the new code.
+We follow the [PEP8](https://peps.python.org/pep-0008/) code style which is checked by `flake8`.
 For all pull requests tests are executed for the most recent python releases via
 ```
-pytest
+pytest -vv -Werror
 pytest --nbmake examples/*.ipynb
+flake8 --ignore=E501,W503 --exclude=__init__.py pyerrors
 ```
-requiring `pytest`, `pytest-cov`, `pytest-benchmark`, `hypothesis` and `nbmake`. To install the test dependencies one can run `pip install pyerrors[test]`
+The tests require `pytest`, `pytest-cov`, `pytest-benchmark`, `hypothesis`, `nbmake` and `flake8`. To install the test dependencies one can run `pip install pyerrors[test]`.
+Please make sure that all tests pass for a new pull requests.
 
 To get a coverage report in html run
 ```
 pytest --cov=pyerrors --cov-report html
 ```
-The linter `flake8` is executed with the command
-```
-flake8 --ignore=E501,W503 --exclude=__init__.py pyerrors
-```
-Please make sure that all tests pass for a new pull requests.
```

### Comparing `pyerrors-2.8.2/LICENSE` & `pyerrors-2.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyerrors-2.8.2/PKG-INFO` & `pyerrors-2.9.0/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,48 +1,31 @@
-Metadata-Version: 2.1
-Name: pyerrors
-Version: 2.8.2
-Summary: Error propagation and statistical analysis for Monte Carlo simulations
-Home-page: https://github.com/fjosw/pyerrors
-Author: Fabian Joswig
-Author-email: fabian.joswig@ed.ac.uk
-License: MIT
-Project-URL: Documentation, https://fjosw.github.io/pyerrors/pyerrors.html
-Project-URL: Bug Tracker, https://github.com/fjosw/pyerrors/issues
-Project-URL: Changelog, https://github.com/fjosw/pyerrors/blob/master/CHANGELOG.md
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Topic :: Scientific/Engineering :: Physics
-Requires-Python: >=3.7.0
-Description-Content-Type: text/markdown
-Provides-Extra: test
-License-File: LICENSE
-
-[![pytest](https://github.com/fjosw/pyerrors/actions/workflows/pytest.yml/badge.svg)](https://github.com/fjosw/pyerrors/actions/workflows/pytest.yml) [![](https://img.shields.io/badge/python-3.7+-blue.svg)](https://www.python.org/downloads/) [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT) [![arXiv](https://img.shields.io/badge/arXiv-2209.14371-b31b1b.svg)](https://arxiv.org/abs/2209.14371) [![DOI](https://img.shields.io/badge/DOI-10.1016%2Fj.cpc.2023.108750-blue)](https://doi.org/10.1016/j.cpc.2023.108750)
+[![pytest](https://github.com/fjosw/pyerrors/actions/workflows/pytest.yml/badge.svg)](https://github.com/fjosw/pyerrors/actions/workflows/pytest.yml) [![](https://img.shields.io/badge/python-3.8+-blue.svg)](https://www.python.org/downloads/) [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT) [![arXiv](https://img.shields.io/badge/arXiv-2209.14371-b31b1b.svg)](https://arxiv.org/abs/2209.14371) [![DOI](https://img.shields.io/badge/DOI-10.1016%2Fj.cpc.2023.108750-blue)](https://doi.org/10.1016/j.cpc.2023.108750)
 # pyerrors
 `pyerrors` is a python framework for error computation and propagation of Markov chain Monte Carlo data from lattice field theory and statistical mechanics simulations.
 
 - **Documentation:** https://fjosw.github.io/pyerrors/pyerrors.html
 - **Examples:** https://github.com/fjosw/pyerrors/tree/develop/examples
+- **Ask a question:** https://github.com/fjosw/pyerrors/discussions/new?category=q-a
+- **Changelog:** https://github.com/fjosw/pyerrors/blob/develop/CHANGELOG.md
 - **Bug reports:** https://github.com/fjosw/pyerrors/issues
 
 ## Installation
 Install the most recent release using pip and [pypi](https://pypi.org/project/pyerrors/):
 ```bash
-pip install pyerrors     # Fresh install
-pip install -U pyerrors  # Update
+python -m pip install pyerrors     # Fresh install
+python -m pip install -U pyerrors  # Update
 ```
 Install the most recent release using conda and [conda-forge](https://anaconda.org/conda-forge/pyerrors):
 ```bash
 conda install -c conda-forge pyerrors  # Fresh install
 conda update -c conda-forge pyerrors   # Update
 ```
 
 ## Contributing
 We appreciate all contributions to the code, the documentation and the examples. If you want to get involved please have a look at our [contribution guideline](https://github.com/fjosw/pyerrors/blob/develop/CONTRIBUTING.md).
+
+## Citing pyerrors
+If you use `pyerrors` for research that leads to a publication we suggest citing the following papers:
+- Fabian Joswig, Simon Kuberski, Justus T. Kuhlmann, Jan Neuendorf, *pyerrors: a python framework for error analysis of Monte Carlo data*. Comput.Phys.Commun. 288 (2023) 108750.
+- Ulli Wolff, *Monte Carlo errors with less errors*. Comput.Phys.Commun. 156 (2004) 143-153, Comput.Phys.Commun. 176 (2007) 383 (erratum).
+- Alberto Ramos, *Automatic differentiation for error analysis of Monte Carlo data*. Comput.Phys.Commun. 238 (2019) 19-35.
+- Stefan Schaefer, Rainer Sommer, Francesco Virotta, *Critical slowing down and error analysis in lattice QCD simulations*. Nucl.Phys.B 845 (2011) 93-119.
```

### Comparing `pyerrors-2.8.2/examples/01_basic_example.ipynb` & `pyerrors-2.9.0/examples/01_basic_example.ipynb`

 * *Files identical despite different names*

### Comparing `pyerrors-2.8.2/examples/02_correlators.ipynb` & `pyerrors-2.9.0/examples/02_correlators.ipynb`

 * *Files identical despite different names*

### Comparing `pyerrors-2.8.2/examples/03_pcac_example.ipynb` & `pyerrors-2.9.0/examples/03_pcac_example.ipynb`

 * *Files identical despite different names*

### Comparing `pyerrors-2.8.2/examples/04_fit_example.ipynb` & `pyerrors-2.9.0/examples/04_fit_example.ipynb`

 * *Files identical despite different names*

### Comparing `pyerrors-2.8.2/examples/05_matrix_operations.ipynb` & `pyerrors-2.9.0/examples/05_matrix_operations.ipynb`

 * *Files 10% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9955336824733376%*

 * *Differences: {"'cells'": "{0: {'source': {insert: [(1, 'import numpy as np')], delete: [2, 1]}}, 2: {'outputs': "*

 * *            "{0: {'text': ['[[4.10(20) -1.00(10)]\\n', ' [-1.00(10) 1.000(10)]]\\n']}}}, 5: "*

 * *            "{'outputs': {0: {'text': ['[[17.81 -5.1]\\n', ' [-5.1 2.0]]\\n']}}}, 7: {'outputs': "*

 * *            "{0: {'text': ['[[4.1 -1.0]\\n', ' [-1.0 1.0]]\\n']}}}, 9: {'outputs': {0: {'text': "*

 * *            "['[[78.12099999999998 -22.909999999999997]\\n', ' [-22.909999999999997 7.1]]\\n']}}}, "*

 * *            "11: {' […]*

```diff
@@ -3,16 +3,15 @@
         {
             "cell_type": "code",
             "execution_count": 1,
             "metadata": {},
             "outputs": [],
             "source": [
                 "import pyerrors as pe\n",
-                "import numpy as np\n",
-                "import scipy"
+                "import numpy as np"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "As an example we look at a symmetric 2x2 matrix which positive semidefinte and has an error on all entries"
@@ -23,16 +22,16 @@
             "execution_count": 2,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "[[Obs[4.10(20)] Obs[-1.00(10)]]\n",
-                        " [Obs[-1.00(10)] Obs[1.000(10)]]]\n"
+                        "[[4.10(20) -1.00(10)]\n",
+                        " [-1.00(10) 1.000(10)]]\n"
                     ]
                 }
             ],
             "source": [
                 "obs11 = pe.pseudo_Obs(4.1, 0.2, 'e1')\n",
                 "obs22 = pe.pseudo_Obs(1, 0.01, 'e1')\n",
                 "obs12 = pe.pseudo_Obs(-1, 0.1, 'e1')\n",
@@ -59,16 +58,16 @@
             "execution_count": 3,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "[[Obs[17.81] Obs[-5.1]]\n",
-                        " [Obs[-5.1] Obs[2.0]]]\n"
+                        "[[17.81 -5.1]\n",
+                        " [-5.1 2.0]]\n"
                     ]
                 }
             ],
             "source": [
                 "print(matrix @ matrix)"
             ]
         },
@@ -84,16 +83,16 @@
             "execution_count": 4,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "[[Obs[4.1] Obs[-1.0]]\n",
-                        " [Obs[-1.0] Obs[1.0]]]\n"
+                        "[[4.1 -1.0]\n",
+                        " [-1.0 1.0]]\n"
                     ]
                 }
             ],
             "source": [
                 "print(matrix @ np.identity(2))"
             ]
         },
@@ -109,16 +108,16 @@
             "execution_count": 5,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "[[Obs[78.12099999999998] Obs[-22.909999999999997]]\n",
-                        " [Obs[-22.909999999999997] Obs[7.1]]]\n"
+                        "[[78.12099999999998 -22.909999999999997]\n",
+                        " [-22.909999999999997 7.1]]\n"
                     ]
                 }
             ],
             "source": [
                 "print(pe.linalg.matmul(matrix, matrix, matrix))  # Equivalent to matrix @ matrix @ matrix but faster for large matrices"
             ]
         },
@@ -134,16 +133,16 @@
             "execution_count": 6,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "[[Obs[30.161857460980094] Obs[-1.1752011936438014]]\n",
-                        " [Obs[-1.1752011936438014] Obs[1.1752011936438014]]]\n"
+                        "[[30.16185746098009 -1.1752011936438014]\n",
+                        " [-1.1752011936438014 1.1752011936438014]]\n"
                     ]
                 }
             ],
             "source": [
                 "print(np.sinh(matrix))"
             ]
         },
@@ -159,24 +158,23 @@
             "execution_count": 7,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "[Obs[2.00(40)] Obs[1.00(10)]]\n"
+                        "[2.00(40) 1.00(10)]\n"
                     ]
                 }
             ],
             "source": [
                 "vec1 = pe.pseudo_Obs(2, 0.4, 'e1')\n",
                 "vec2 = pe.pseudo_Obs(1, 0.1, 'e1')\n",
                 "vector = np.asarray([vec1, vec2])\n",
-                "for (i), entry in np.ndenumerate(vector):\n",
-                "    entry.gamma_method()\n",
+                "pe.gm(vector)\n",
                 "print(vector)"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
@@ -188,22 +186,21 @@
             "execution_count": 8,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "[Obs[7.2(1.7)] Obs[-1.00(46)]]\n"
+                        "[7.2(1.7) -1.00(45)]\n"
                     ]
                 }
             ],
             "source": [
                 "product = matrix @ vector\n",
-                "for (i), entry in np.ndenumerate(product):\n",
-                "    entry.gamma_method()\n",
+                "pe.gm(product)\n",
                 "print(product)"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
@@ -241,23 +238,22 @@
             "execution_count": 10,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "[[Obs[2.025(49)] Obs[0.0]]\n",
-                        " [Obs[-0.494(50)] Obs[0.870(29)]]]\n"
+                        "[[2.025(49) 0.0]\n",
+                        " [-0.494(50) 0.870(29)]]\n"
                     ]
                 }
             ],
             "source": [
                 "cholesky = pe.linalg.cholesky(matrix)\n",
-                "for (i, j), entry in np.ndenumerate(cholesky):\n",
-                "    entry.gamma_method()\n",
+                "pe.gm(cholesky)\n",
                 "print(cholesky)"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
@@ -269,16 +265,16 @@
             "execution_count": 11,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "[[Obs[-8.881784197001252e-16] Obs[0.0]]\n",
-                        " [Obs[0.0] Obs[0.0]]]\n"
+                        "[[-8.881784197001252e-16 0.0]\n",
+                        " [0.0 0.0]]\n"
                     ]
                 }
             ],
             "source": [
                 "check = cholesky @ cholesky.T\n",
                 "print(check - matrix)"
             ]
@@ -295,26 +291,25 @@
             "execution_count": 12,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "[[Obs[0.494(12)] Obs[0.0]]\n",
-                        " [Obs[0.280(40)] Obs[1.150(39)]]]\n",
+                        "[[0.494(12) 0.0]\n",
+                        " [0.280(40) 1.150(38)]]\n",
                         "Check:\n",
-                        "[[Obs[1.0] Obs[0.0]]\n",
-                        " [Obs[0.0] Obs[1.0]]]\n"
+                        "[[1.0 0.0]\n",
+                        " [0.0 1.0]]\n"
                     ]
                 }
             ],
             "source": [
                 "inv = pe.linalg.inv(cholesky)\n",
-                "for (i, j), entry in np.ndenumerate(inv):\n",
-                "    entry.gamma_method()\n",
+                "pe.gm(inv)\n",
                 "print(inv)\n",
                 "print('Check:')\n",
                 "check_inv = cholesky @ inv\n",
                 "print(check_inv)"
             ]
         },
         {
@@ -331,29 +326,27 @@
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "Eigenvalues:\n",
-                        "[Obs[0.705(57)] Obs[4.39(19)]]\n",
+                        "[0.705(56) 4.39(20)]\n",
                         "Eigenvectors:\n",
-                        "[[Obs[-0.283(26)] Obs[-0.9592(75)]]\n",
-                        " [Obs[-0.9592(75)] Obs[0.283(26)]]]\n"
+                        "[[-0.283(26) -0.9592(75)]\n",
+                        " [-0.9592(75) 0.283(26)]]\n"
                     ]
                 }
             ],
             "source": [
                 "e, v = pe.linalg.eigh(matrix)\n",
-                "for (i), entry in np.ndenumerate(e):\n",
-                "    entry.gamma_method()\n",
+                "pe.gm(e)\n",
                 "print('Eigenvalues:')\n",
                 "print(e)\n",
-                "for (i, j), entry in np.ndenumerate(v):\n",
-                "    entry.gamma_method()\n",
+                "pe.gm(v)\n",
                 "print('Eigenvectors:')\n",
                 "print(v)"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
@@ -367,17 +360,17 @@
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "Check eigenvector 1\n",
-                        "[Obs[-5.551115123125783e-17] Obs[0.0]]\n",
+                        "[-5.551115123125783e-17 0.0]\n",
                         "Check eigenvector 2\n",
-                        "[Obs[0.0] Obs[-2.220446049250313e-16]]\n"
+                        "[0.0 -2.220446049250313e-16]\n"
                     ]
                 }
             ],
             "source": [
                 "for i in range(2):\n",
                 "    print('Check eigenvector', i + 1)\n",
                 "    print(matrix @ v[:, i] - v[:, i] * e[i])"
@@ -403,13 +396,13 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.8.10"
+            "version": "3.11.0"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 4
 }
```

### Comparing `pyerrors-2.8.2/examples/06_gevp.ipynb` & `pyerrors-2.9.0/examples/06_gevp.ipynb`

 * *Files identical despite different names*

### Comparing `pyerrors-2.8.2/examples/07_data_management.ipynb` & `pyerrors-2.9.0/examples/07_data_management.ipynb`

 * *Files identical despite different names*

### Comparing `pyerrors-2.8.2/examples/08_combined_fit_example.ipynb` & `pyerrors-2.9.0/examples/08_combined_fit_example.ipynb`

 * *Files identical despite different names*

### Comparing `pyerrors-2.8.2/examples/base_style.mplstyle` & `pyerrors-2.9.0/examples/base_style.mplstyle`

 * *Files identical despite different names*

### Comparing `pyerrors-2.8.2/examples/data/correlator_test.json.gz` & `pyerrors-2.9.0/examples/data/correlator_test.json.gz`

 * *Files identical despite different names*

### Comparing `pyerrors-2.8.2/examples/data/f_A.json.gz` & `pyerrors-2.9.0/examples/data/f_A.json.gz`

 * *Files identical despite different names*

### Comparing `pyerrors-2.8.2/examples/data/f_P.json.gz` & `pyerrors-2.9.0/examples/data/f_P.json.gz`

 * *Files identical despite different names*

### Comparing `pyerrors-2.8.2/examples/data/matrix_correlator.json.gz` & `pyerrors-2.9.0/examples/data/matrix_correlator.json.gz`

 * *Files identical despite different names*

### Comparing `pyerrors-2.8.2/examples/data/matrix_correlator_V1V1.json.gz` & `pyerrors-2.9.0/examples/data/matrix_correlator_V1V1.json.gz`

 * *Files identical despite different names*

### Comparing `pyerrors-2.8.2/examples/data/matrix_correlator_V2V2.json.gz` & `pyerrors-2.9.0/examples/data/matrix_correlator_V2V2.json.gz`

 * *Files identical despite different names*

### Comparing `pyerrors-2.8.2/examples/data/matrix_correlator_V3V3.json.gz` & `pyerrors-2.9.0/examples/data/matrix_correlator_V3V3.json.gz`

 * *Files identical despite different names*

### Comparing `pyerrors-2.8.2/examples/json_schema.json` & `pyerrors-2.9.0/examples/json_schema.json`

 * *Files identical despite different names*

### Comparing `pyerrors-2.8.2/pyerrors/__init__.py` & `pyerrors-2.9.0/pyerrors/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,26 +23,27 @@
 
 There exist similar publicly available implementations of gamma method error analysis suites in [Fortran](https://gitlab.ift.uam-csic.es/alberto/aderrors), [Julia](https://gitlab.ift.uam-csic.es/alberto/aderrors.jl) and [Python](https://github.com/mbruno46/pyobs).
 
 ## Installation
 
 Install the most recent release using pip and [pypi](https://pypi.org/project/pyerrors/):
 ```bash
-pip install pyerrors     # Fresh install
-pip install -U pyerrors  # Update
+python -m pip install pyerrors     # Fresh install
+python -m pip install -U pyerrors  # Update
 ```
 Install the most recent release using conda and [conda-forge](https://anaconda.org/conda-forge/pyerrors):
 ```bash
 conda install -c conda-forge pyerrors  # Fresh install
 conda update -c conda-forge pyerrors   # Update
 ```
 Install the current `develop` version:
 ```bash
-pip install git+https://github.com/fjosw/pyerrors.git@develop
+python -m pip install -U --no-deps --force-reinstall git+https://github.com/fjosw/pyerrors.git@develop
 ```
+(Also works for any feature branch).
 
 ## Basic example
 
 ```python
 import numpy as np
 import pyerrors as pe
 
@@ -104,14 +105,15 @@
 my_sum.details()
 > Result	 1.70000000e+00 +/- 5.72046658e-01 +/- 7.56746598e-02 (33.650%)
 >  t_int	 2.71422900e+00 +/- 6.40320983e-01 S = 2.00
 > 1000 samples in 1 ensemble:
 >   · Ensemble 'ensemble_name' : 1000 configurations (from 1 to 1000)
 
 ```
+The `gamma_method` is not automatically called after every intermediate step in order to prevent computational overhead.
 
 We use the following definition of the integrated autocorrelation time established in [Madras & Sokal 1988](https://link.springer.com/article/10.1007/BF01022990)
 $$\tau_\mathrm{int}=\frac{1}{2}+\sum_{t=1}^{W}\rho(t)\geq \frac{1}{2}\,.$$
 The window $W$ is determined via the automatic windowing procedure described in [arXiv:hep-lat/0306017](https://arxiv.org/abs/hep-lat/0306017).
 The standard value for the parameter $S$ of this automatic windowing procedure is $S=2$. Other values for $S$ can be passed to the `gamma_method` as parameter.
 
 ```python
@@ -301,15 +303,15 @@
 print(my_derived_cobs)
 > (1.668(23)+0.0j)
 ```
 
 # The `Covobs` class
 In many projects, auxiliary data that is not based on Monte Carlo chains enters. Examples are experimentally determined mesons masses which are used to set the scale or renormalization constants. These numbers come with an error that has to be propagated through the analysis. The `Covobs` class allows to define such quantities in `pyerrors`. Furthermore, external input might consist of correlated quantities. An example are the parameters of an interpolation formula, which are defined via mean values and a covariance matrix between all parameters. The contribution of the interpolation formula to the error of a derived quantity therefore might depend on the complete covariance matrix.
 
-This concept is built into the definition of `Covobs`. In `pyerrors`, external input is defined by $M$ mean values, a $M\times M$ covariance matrix, where $M=1$ is permissible, and a name that uniquely identifies the covariance matrix. Below, we define the pion mass, based on its mean value and error, 134.9768(5). Note, that the square of the error enters `cov_Obs`, since the second argument of this function is the covariance matrix of the `Covobs`.
+This concept is built into the definition of `Covobs`. In `pyerrors`, external input is defined by $M$ mean values, a $M\times M$ covariance matrix, where $M=1$ is permissible, and a name that uniquely identifies the covariance matrix. Below, we define the pion mass, based on its mean value and error, 134.9768(5). **Note, that the square of the error enters `cov_Obs`**, since the second argument of this function is the covariance matrix of the `Covobs`.
 
 ```python
 import pyerrors.obs as pe
 
 mpi = pe.cov_Obs(134.9768, 0.0005**2, 'pi^0 mass')
 mpi.gamma_method()
 mpi.details()
@@ -383,19 +385,20 @@
 def func(a, x):
     (x1, x2) = x
     return a[0] * x1 ** 2 + a[1] * x2
 ```
 
 `pyerrors` also supports correlated fits which can be triggered via the parameter `correlated_fit=True`.
 Details about how the required covariance matrix is estimated can be found in `pyerrors.obs.covariance`.
+Direct visualizations of the performed fits can be triggered via `resplot=True` or `qqplot=True`.
 
-Direct visualizations of the performed fits can be triggered via `resplot=True` or `qqplot=True`. For all available options see `pyerrors.fits.least_squares`.
+For all available options including combined fits to multiple datasets see `pyerrors.fits.least_squares`.
 
 ## Total least squares fits
-`pyerrors` can also fit data with errors on both the dependent and independent variables using the total least squares method also referred to orthogonal distance regression as implemented in [scipy](https://docs.scipy.org/doc/scipy/reference/odr.html), see `pyerrors.fits.least_squares`. The syntax is identical to the standard least squares case, the only difference being that `x` also has to be a `list` or `numpy.array` of `Obs`.
+`pyerrors` can also fit data with errors on both the dependent and independent variables using the total least squares method also referred to as orthogonal distance regression as implemented in [scipy](https://docs.scipy.org/doc/scipy/reference/odr.html), see `pyerrors.fits.least_squares`. The syntax is identical to the standard least squares case, the only difference being that `x` also has to be a `list` or `numpy.array` of `Obs`.
 
 For the full API see `pyerrors.fits` for fits and `pyerrors.roots` for finding roots of functions.
 
 # Matrix operations
 `pyerrors` provides wrappers for `Obs`- and `CObs`-valued matrix operations based on `numpy.linalg`. The supported functions include:
 - `inv` for the matrix inverse.
 - `cholseky` for the Cholesky decomposition.
@@ -479,9 +482,10 @@
 from .fits import *
 from .misc import *
 from . import dirac
 from . import input
 from . import linalg
 from . import mpm
 from . import roots
+from . import integrate
 
 from .version import __version__
```

### Comparing `pyerrors-2.8.2/pyerrors/correlators.py` & `pyerrors-2.9.0/pyerrors/correlators.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,91 +7,113 @@
 from .obs import Obs, reweight, correlate, CObs
 from .misc import dump_object, _assert_equal_properties
 from .fits import least_squares
 from .roots import find_root
 
 
 class Corr:
-    """The class for a correlator (time dependent sequence of pe.Obs).
+    r"""The class for a correlator (time dependent sequence of pe.Obs).
 
     Everything, this class does, can be achieved using lists or arrays of Obs.
     But it is simply more convenient to have a dedicated object for correlators.
     One often wants to add or multiply correlators of the same length at every timeslice and it is inconvenient
     to iterate over all timeslices for every operation. This is especially true, when dealing with matrices.
 
-    The correlator can have two types of content: An Obs at every timeslice OR a GEVP
-    matrix at every timeslice. Other dependency (eg. spatial) are not supported.
+    The correlator can have two types of content: An Obs at every timeslice OR a matrix at every timeslice.
+    Other dependency (eg. spatial) are not supported.
 
+    The Corr class can also deal with missing measurements or paddings for fixed boundary conditions.
+    The missing entries are represented via the `None` object.
+
+    Initialization
+    --------------
+    A simple correlator can be initialized with a list or a one-dimensional array of `Obs` or `Cobs`
+    ```python
+    corr11 = pe.Corr([obs1, obs2])
+    corr11 = pe.Corr(np.array([obs1, obs2]))
+    ```
+    A matrix-valued correlator can either be initialized via a two-dimensional array of `Corr` objects
+    ```python
+    matrix_corr = pe.Corr(np.array([[corr11, corr12], [corr21, corr22]]))
+    ```
+    or alternatively via a three-dimensional array of `Obs` or `CObs` of shape (T, N, N) where T is
+    the temporal extent of the correlator and N is the dimension of the matrix.
     """
 
     __slots__ = ["content", "N", "T", "tag", "prange"]
 
     def __init__(self, data_input, padding=[0, 0], prange=None):
         """ Initialize a Corr object.
 
         Parameters
         ----------
         data_input : list or array
-            list of Obs or list of arrays of Obs or array of Corrs
+            list of Obs or list of arrays of Obs or array of Corrs (see class docstring for details).
         padding : list, optional
             List with two entries where the first labels the padding
             at the front of the correlator and the second the padding
             at the back.
         prange : list, optional
             List containing the first and last timeslice of the plateau
-            region indentified for this correlator.
+            region identified for this correlator.
         """
 
         if isinstance(data_input, np.ndarray):
-
-            # This only works, if the array fulfills the conditions below
-            if not len(data_input.shape) == 2 and data_input.shape[0] == data_input.shape[1]:
-                raise Exception("Incompatible array shape")
-            if not all([isinstance(item, Corr) for item in data_input.flatten()]):
-                raise Exception("If the input is an array, its elements must be of type pe.Corr")
-            if not all([item.N == 1 for item in data_input.flatten()]):
-                raise Exception("Can only construct matrix correlator from single valued correlators")
-            if not len(set([item.T for item in data_input.flatten()])) == 1:
-                raise Exception("All input Correlators must be defined over the same timeslices.")
-
-            T = data_input[0, 0].T
-            N = data_input.shape[0]
-            input_as_list = []
-            for t in range(T):
-                if any([(item.content[t] is None) for item in data_input.flatten()]):
-                    if not all([(item.content[t] is None) for item in data_input.flatten()]):
-                        warnings.warn("Input ill-defined at different timeslices. Conversion leads to data loss!", RuntimeWarning)
-                    input_as_list.append(None)
-                else:
-                    array_at_timeslace = np.empty([N, N], dtype="object")
-                    for i in range(N):
-                        for j in range(N):
-                            array_at_timeslace[i, j] = data_input[i, j][t]
-                    input_as_list.append(array_at_timeslace)
-            data_input = input_as_list
+            if data_input.ndim == 1:
+                data_input = list(data_input)
+            elif data_input.ndim == 2:
+                if not data_input.shape[0] == data_input.shape[1]:
+                    raise ValueError("Array needs to be square.")
+                if not all([isinstance(item, Corr) for item in data_input.flatten()]):
+                    raise ValueError("If the input is an array, its elements must be of type pe.Corr.")
+                if not all([item.N == 1 for item in data_input.flatten()]):
+                    raise ValueError("Can only construct matrix correlator from single valued correlators.")
+                if not len(set([item.T for item in data_input.flatten()])) == 1:
+                    raise ValueError("All input Correlators must be defined over the same timeslices.")
+
+                T = data_input[0, 0].T
+                N = data_input.shape[0]
+                input_as_list = []
+                for t in range(T):
+                    if any([(item.content[t] is None) for item in data_input.flatten()]):
+                        if not all([(item.content[t] is None) for item in data_input.flatten()]):
+                            warnings.warn("Input ill-defined at different timeslices. Conversion leads to data loss.!", RuntimeWarning)
+                        input_as_list.append(None)
+                    else:
+                        array_at_timeslace = np.empty([N, N], dtype="object")
+                        for i in range(N):
+                            for j in range(N):
+                                array_at_timeslace[i, j] = data_input[i, j][t]
+                        input_as_list.append(array_at_timeslace)
+                data_input = input_as_list
+            elif data_input.ndim == 3:
+                if not data_input.shape[1] == data_input.shape[2]:
+                    raise ValueError("Array needs to be square.")
+                data_input = list(data_input)
+            else:
+                raise ValueError("Arrays with ndim>3 not supported.")
 
         if isinstance(data_input, list):
 
             if all([isinstance(item, (Obs, CObs)) or item is None for item in data_input]):
                 _assert_equal_properties([o for o in data_input if o is not None])
                 self.content = [np.asarray([item]) if item is not None else None for item in data_input]
                 self.N = 1
-
             elif all([isinstance(item, np.ndarray) or item is None for item in data_input]) and any([isinstance(item, np.ndarray) for item in data_input]):
                 self.content = data_input
                 noNull = [a for a in self.content if not (a is None)]  # To check if the matrices are correct for all undefined elements
                 self.N = noNull[0].shape[0]
                 if self.N > 1 and noNull[0].shape[0] != noNull[0].shape[1]:
-                    raise Exception("Smearing matrices are not NxN")
+                    raise ValueError("Smearing matrices are not NxN.")
                 if (not all([item.shape == noNull[0].shape for item in noNull])):
-                    raise Exception("Items in data_input are not of identical shape." + str(noNull))
+                    raise ValueError("Items in data_input are not of identical shape." + str(noNull))
             else:
-                raise Exception("data_input contains item of wrong type")
+                raise TypeError("'data_input' contains item of wrong type.")
         else:
-            raise Exception("Data input was not given as list or correct array")
+            raise TypeError("Data input was not given as list or correct array.")
 
         self.tag = None
 
         # An undefined timeslice is represented by the None object
         self.content = [None] * padding[0] + self.content + [None] * padding[1]
         self.T = len(self.content)
         self.prange = prange
@@ -216,15 +238,15 @@
         if (all([x is None for x in newcontent])):
             raise Exception("Corr could not be symmetrized: No redundant values")
         return Corr(newcontent, prange=self.prange)
 
     def anti_symmetric(self):
         """Anti-symmetrize the correlator around x0=0."""
         if self.N != 1:
-            raise Exception('anti_symmetric cannot be safely applied to multi-dimensional correlators.')
+            raise TypeError('anti_symmetric cannot be safely applied to multi-dimensional correlators.')
         if self.T % 2 != 0:
             raise Exception("Can not symmetrize odd T")
 
         test = 1 * self
         test.gamma_method()
         if not all([o.is_zero_within_error(3) for o in test.content[0]]):
             warnings.warn("Correlator does not seem to be anti-symmetric around x0=0.", RuntimeWarning)
@@ -238,26 +260,38 @@
         if (all([x is None for x in newcontent])):
             raise Exception("Corr could not be symmetrized: No redundant values")
         return Corr(newcontent, prange=self.prange)
 
     def is_matrix_symmetric(self):
         """Checks whether a correlator matrices is symmetric on every timeslice."""
         if self.N == 1:
-            raise Exception("Only works for correlator matrices.")
+            raise TypeError("Only works for correlator matrices.")
         for t in range(self.T):
             if self[t] is None:
                 continue
             for i in range(self.N):
                 for j in range(i + 1, self.N):
                     if self[t][i, j] is self[t][j, i]:
                         continue
                     if hash(self[t][i, j]) != hash(self[t][j, i]):
                         return False
         return True
 
+    def trace(self):
+        """Calculates the per-timeslice trace of a correlator matrix."""
+        if self.N == 1:
+            raise ValueError("Only works for correlator matrices.")
+        newcontent = []
+        for t in range(self.T):
+            if _check_for_none(self, self.content[t]):
+                newcontent.append(None)
+            else:
+                newcontent.append(np.trace(self.content[t]))
+        return Corr(newcontent)
+
     def matrix_symmetric(self):
         """Symmetrizes the correlator matrices on every timeslice."""
         if self.N == 1:
             raise Exception("Trying to symmetrize a correlator matrix, that already has N=1.")
         if self.is_matrix_symmetric():
             return 1.0 * self
         else:
@@ -401,15 +435,15 @@
         """Periodically shift the correlator by dt timeslices
 
         Parameters
         ----------
         dt : int
             number of timeslices
         """
-        return Corr(list(np.roll(np.array(self.content, dtype=object), dt)))
+        return Corr(list(np.roll(np.array(self.content, dtype=object), dt, axis=0)))
 
     def reverse(self):
         """Reverse the time ordering of the Corr"""
         return Corr(self.content[:: -1])
 
     def thin(self, spacing=2, offset=0):
         """Thin out a correlator to suppress correlations
@@ -484,15 +518,15 @@
     def T_symmetry(self, partner, parity=+1):
         """Return the time symmetry average of the correlator and its partner
 
         Parameters
         ----------
         partner : Corr
             Time symmetry partner of the Corr
-        partity : int
+        parity : int
             Parity quantum number of the correlator, can be +1 or -1
         """
         if self.N != 1:
             raise Exception("T_symmetry only implemented for one-dimensional correlators.")
         if not isinstance(partner, Corr):
             raise Exception("T partner has to be a Corr object.")
         if parity not in [+1, -1]:
@@ -573,34 +607,52 @@
                 raise Exception("Log is undefined at all timeslices")
             logcorr = Corr(newcontent)
             return self * logcorr.deriv('symmetric')
         else:
             raise Exception("Unknown variant.")
 
     def second_deriv(self, variant="symmetric"):
-        """Return the second derivative of the correlator with respect to x0.
+        r"""Return the second derivative of the correlator with respect to x0.
 
         Parameters
         ----------
         variant : str
             decides which definition of the finite differences derivative is used.
-            Available choice: symmetric, improved, log, default: symmetric
+            Available choice:
+                - symmetric (default)
+                    $$\tilde{\partial}^2_0 f(x_0) = f(x_0+1)-2f(x_0)+f(x_0-1)$$
+                - big_symmetric
+                    $$\partial^2_0 f(x_0) = \frac{f(x_0+2)-2f(x_0)+f(x_0-2)}{4}$$
+                - improved
+                    $$\partial^2_0 f(x_0) = \frac{-f(x_0+2) + 16 * f(x_0+1) - 30 * f(x_0) + 16 * f(x_0-1) - f(x_0-2)}{12}$$
+                - log
+                    $$f(x) = \tilde{\partial}^2_0 log(f(x_0))+(\tilde{\partial}_0 log(f(x_0)))^2$$
         """
         if self.N != 1:
             raise Exception("second_deriv only implemented for one-dimensional correlators.")
         if variant == "symmetric":
             newcontent = []
             for t in range(1, self.T - 1):
                 if (self.content[t - 1] is None) or (self.content[t + 1] is None):
                     newcontent.append(None)
                 else:
                     newcontent.append((self.content[t + 1] - 2 * self.content[t] + self.content[t - 1]))
             if (all([x is None for x in newcontent])):
                 raise Exception("Derivative is undefined at all timeslices")
             return Corr(newcontent, padding=[1, 1])
+        elif variant == "big_symmetric":
+            newcontent = []
+            for t in range(2, self.T - 2):
+                if (self.content[t - 2] is None) or (self.content[t + 2] is None):
+                    newcontent.append(None)
+                else:
+                    newcontent.append((self.content[t + 2] - 2 * self.content[t] + self.content[t - 2]) / 4)
+            if (all([x is None for x in newcontent])):
+                raise Exception("Derivative is undefined at all timeslices")
+            return Corr(newcontent, padding=[2, 2])
         elif variant == "improved":
             newcontent = []
             for t in range(2, self.T - 2):
                 if (self.content[t - 2] is None) or (self.content[t - 1] is None) or (self.content[t] is None) or (self.content[t + 1] is None) or (self.content[t + 2] is None):
                     newcontent.append(None)
                 else:
                     newcontent.append((1 / 12) * (-self.content[t + 2] + 16 * self.content[t + 1] - 30 * self.content[t] + 16 * self.content[t - 1] - self.content[t - 2]))
@@ -624,16 +676,16 @@
     def m_eff(self, variant='log', guess=1.0):
         """Returns the effective mass of the correlator as correlator object
 
         Parameters
         ----------
         variant : str
             log : uses the standard effective mass log(C(t) / C(t+1))
-            cosh, periodic : Use periodicitiy of the correlator by solving C(t) / C(t+1) = cosh(m * (t - T/2)) / cosh(m * (t + 1 - T/2)) for m.
-            sinh : Use anti-periodicitiy of the correlator by solving C(t) / C(t+1) = sinh(m * (t - T/2)) / sinh(m * (t + 1 - T/2)) for m.
+            cosh, periodic : Use periodicity of the correlator by solving C(t) / C(t+1) = cosh(m * (t - T/2)) / cosh(m * (t + 1 - T/2)) for m.
+            sinh : Use anti-periodicity of the correlator by solving C(t) / C(t+1) = sinh(m * (t - T/2)) / sinh(m * (t + 1 - T/2)) for m.
             See, e.g., arXiv:1205.5380
             arccosh : Uses the explicit form of the symmetrized correlator (not recommended)
             logsym: uses the symmetric effective mass log(C(t-1) / C(t+1))/2
         guess : float
             guess for the root finder, only relevant for the root variant
         """
         if self.N != 1:
@@ -976,38 +1028,45 @@
         content_string = ""
         content_string += "Corr T=" + str(self.T) + " N=" + str(self.N) + "\n"  # +" filled with"+ str(type(self.content[0][0])) there should be a good solution here
 
         if self.tag is not None:
             content_string += "Description: " + self.tag + "\n"
         if self.N != 1:
             return content_string
-        if isinstance(self[0], CObs):
-            return content_string
 
         if print_range[1]:
             print_range[1] += 1
         content_string += 'x0/a\tCorr(x0/a)\n------------------\n'
         for i, sub_corr in enumerate(self.content[print_range[0]:print_range[1]]):
             if sub_corr is None:
                 content_string += str(i + print_range[0]) + '\n'
             else:
                 content_string += str(i + print_range[0])
                 for element in sub_corr:
-                    content_string += '\t' + ' ' * int(element >= 0) + str(element)
+                    content_string += f"\t{element:+2}"
                 content_string += '\n'
         return content_string
 
     def __str__(self):
         return self.__repr__()
 
     # We define the basic operations, that can be performed with correlators.
     # While */+- get defined here, they only work for Corr*Obs and not Obs*Corr.
     # This is because Obs*Corr checks Obs.__mul__ first and does not catch an exception.
     # One could try and tell Obs to check if the y in __mul__ is a Corr and
 
+    __array_priority__ = 10000
+
+    def __eq__(self, y):
+        if isinstance(y, Corr):
+            comp = np.asarray(y.content, dtype=object)
+        else:
+            comp = np.asarray(y)
+        return np.asarray(self.content, dtype=object) == comp
+
     def __add__(self, y):
         if isinstance(y, Corr):
             if ((self.N != y.N) or (self.T != y.T)):
                 raise Exception("Addition of Corrs with different shape")
             newcontent = []
             for t in range(self.T):
                 if _check_for_none(self, self.content[t]) or _check_for_none(y, y.content[t]):
@@ -1056,14 +1115,57 @@
             if y.shape == (self.T,):
                 return Corr(list((np.array(self.content).T * y).T))
             else:
                 raise ValueError("operands could not be broadcast together")
         else:
             raise TypeError("Corr * wrong type")
 
+    def __matmul__(self, y):
+        if isinstance(y, np.ndarray):
+            if y.ndim != 2 or y.shape[0] != y.shape[1]:
+                raise ValueError("Can only multiply correlators by square matrices.")
+            if not self.N == y.shape[0]:
+                raise ValueError("matmul: mismatch of matrix dimensions")
+            newcontent = []
+            for t in range(self.T):
+                if _check_for_none(self, self.content[t]):
+                    newcontent.append(None)
+                else:
+                    newcontent.append(self.content[t] @ y)
+            return Corr(newcontent)
+        elif isinstance(y, Corr):
+            if not self.N == y.N:
+                raise ValueError("matmul: mismatch of matrix dimensions")
+            newcontent = []
+            for t in range(self.T):
+                if _check_for_none(self, self.content[t]) or _check_for_none(y, y.content[t]):
+                    newcontent.append(None)
+                else:
+                    newcontent.append(self.content[t] @ y.content[t])
+            return Corr(newcontent)
+
+        else:
+            return NotImplemented
+
+    def __rmatmul__(self, y):
+        if isinstance(y, np.ndarray):
+            if y.ndim != 2 or y.shape[0] != y.shape[1]:
+                raise ValueError("Can only multiply correlators by square matrices.")
+            if not self.N == y.shape[0]:
+                raise ValueError("matmul: mismatch of matrix dimensions")
+            newcontent = []
+            for t in range(self.T):
+                if _check_for_none(self, self.content[t]):
+                    newcontent.append(None)
+                else:
+                    newcontent.append(y @ self.content[t])
+            return Corr(newcontent)
+        else:
+            return NotImplemented
+
     def __truediv__(self, y):
         if isinstance(y, Corr):
             if not ((self.N == 1 or y.N == 1 or self.N == y.N) and self.T == y.T):
                 raise Exception("Multiplication of Corr object requires N=N or N=1 and T=T")
             newcontent = []
             for t in range(self.T):
                 if _check_for_none(self, self.content[t]) or _check_for_none(y, y.content[t]):
```

### Comparing `pyerrors-2.8.2/pyerrors/covobs.py` & `pyerrors-2.9.0/pyerrors/covobs.py`

 * *Files identical despite different names*

### Comparing `pyerrors-2.8.2/pyerrors/dirac.py` & `pyerrors-2.9.0/pyerrors/dirac.py`

 * *Files identical despite different names*

### Comparing `pyerrors-2.8.2/pyerrors/fits.py` & `pyerrors-2.9.0/pyerrors/fits.py`

 * *Files 2% similar despite different names*

```diff
@@ -226,14 +226,20 @@
             else:
                 break
         else:
             raise RuntimeError("Fit function (key=" + key + ") is not valid.")
         n_parms_ls.append(n_loc)
 
     n_parms = max(n_parms_ls)
+
+    if len(key_ls) > 1:
+        for key in key_ls:
+            if np.asarray(yd[key]).shape != funcd[key](np.arange(n_parms), xd[key]).shape:
+                raise ValueError(f"Fit function {key} returns the wrong shape ({funcd[key](np.arange(n_parms), xd[key]).shape} instead of {xd[key].shape})\nIf the fit function is just a constant you could try adding x*0 to get the correct shape.")
+
     if not silent:
         print('Fit with', n_parms, 'parameter' + 's' * (n_parms > 1))
 
     if priors is not None:
         if isinstance(priors, (list, np.ndarray)):
             if n_parms != len(priors):
                 raise ValueError("'priors' does not have the correct length.")
```

### Comparing `pyerrors-2.8.2/pyerrors/input/__init__.py` & `pyerrors-2.9.0/pyerrors/input/__init__.py`

 * *Files identical despite different names*

### Comparing `pyerrors-2.8.2/pyerrors/input/bdio.py` & `pyerrors-2.9.0/pyerrors/input/bdio.py`

 * *Files identical despite different names*

### Comparing `pyerrors-2.8.2/pyerrors/input/dobs.py` & `pyerrors-2.9.0/pyerrors/input/dobs.py`

 * *Files identical despite different names*

### Comparing `pyerrors-2.8.2/pyerrors/input/hadrons.py` & `pyerrors-2.9.0/pyerrors/input/hadrons.py`

 * *Files 10% similar despite different names*

```diff
@@ -50,82 +50,139 @@
         idx = idl
     else:
         raise Exception("Configurations are not evenly spaced. Provide an idl if you want to proceed with this set of configurations.")
 
     return filtered_files, idx
 
 
-def read_meson_hd5(path, filestem, ens_id, meson='meson_0', idl=None, gammas=None):
-    r'''Read hadrons meson hdf5 file and extract the meson labeled 'meson'
+def read_hd5(filestem, ens_id, group, attrs=None, idl=None, part="real"):
+    r'''Read hadrons hdf5 file and extract entry based on attributes.
 
     Parameters
     -----------------
-    path : str
-        path to the files to read
     filestem : str
-        namestem of the files to read
+        Full namestem of the files to read, including the full path.
     ens_id : str
         name of the ensemble, required for internal bookkeeping
-    meson : str
-        label of the meson to be extracted, standard value meson_0 which
-        corresponds to the pseudoscalar pseudoscalar two-point function.
-    gammas : tuple of strings
-        Instrad of a meson label one can also provide a tuple of two strings
-        indicating the gamma matrices at source and sink.
-        ("Gamma5", "Gamma5") corresponds to the pseudoscalar pseudoscalar
-        two-point function. The gammas argument dominateds over meson.
+    group : str
+        label of the group to be extracted.
+    attrs : dict or int
+        Dictionary containing the attributes. For example
+        ```python
+        attrs = {"gamma_snk": "Gamma5",
+                 "gamma_src": "Gamma5"}
+         ```
+        Alternatively an integer can be specified to identify the sub group.
+        This is discouraged as the order in the file is not guaranteed.
     idl : range
         If specified only configurations in the given range are read in.
+    part: str
+        string specifying whether to extract the real part ('real'),
+        the imaginary part ('imag') or a complex correlator ('complex').
+        Default 'real'.
 
     Returns
     -------
     corr : Corr
         Correlator of the source sink combination in question.
     '''
 
+    path_obj = Path(filestem)
+    path = path_obj.parent.as_posix()
+    filestem = path_obj.stem
+
     files, idx = _get_files(path, filestem, idl)
 
-    tree = meson.rsplit('_')[0]
-    if gammas is not None:
+    if isinstance(attrs, dict):
         h5file = h5py.File(path + '/' + files[0], "r")
-        found_meson = None
-        for key in h5file[tree].keys():
-            if gammas[0] == h5file[tree][key].attrs["gamma_snk"][0].decode() and h5file[tree][key].attrs["gamma_src"][0].decode() == gammas[1]:
-                found_meson = key
-                break
+        entry = None
+        for key in h5file[group].keys():
+            if attrs.items() <= {k: v[0].decode() for k, v in h5file[group][key].attrs.items()}.items():
+                if entry is None:
+                    entry = key
+                else:
+                    raise ValueError("More than one fitting entry found. More constraint on attributes needed.")
         h5file.close()
-        if found_meson:
-            meson = found_meson
-        else:
-            raise Exception("Source Sink combination " + str(gammas) + " not found.")
+        if entry is None:
+            raise ValueError(f"Entry with attributes {attrs} not found.")
+    elif isinstance(attrs, int):
+        entry = group + f"_{attrs}"
+    else:
+        raise TypeError("Invalid type for 'attrs'. Needs to be dict or int.")
 
     corr_data = []
     infos = []
     for hd5_file in files:
         h5file = h5py.File(path + '/' + hd5_file, "r")
-        if not tree + '/' + meson in h5file:
-            raise Exception("Entry '" + meson + "' not contained in the files.")
-        raw_data = h5file[tree + '/' + meson + '/corr']
-        real_data = raw_data[:]["re"].astype(np.double)
+        if not group + '/' + entry in h5file:
+            raise Exception("Entry '" + entry + "' not contained in the files.")
+        raw_data = h5file[group + '/' + entry + '/corr']
+        real_data = raw_data[:].view("complex")
         corr_data.append(real_data)
         if not infos:
-            for k, i in h5file[tree + '/' + meson].attrs.items():
+            for k, i in h5file[group + '/' + entry].attrs.items():
                 infos.append(k + ': ' + i[0].decode())
         h5file.close()
     corr_data = np.array(corr_data)
 
-    l_obs = []
-    for c in corr_data.T:
-        l_obs.append(Obs([c], [ens_id], idl=[idx]))
+    if part == "complex":
+        l_obs = []
+        for c in corr_data.T:
+            l_obs.append(CObs(Obs([c.real], [ens_id], idl=[idx]),
+                              Obs([c.imag], [ens_id], idl=[idx])))
+    else:
+        corr_data = getattr(corr_data, part)
+        l_obs = []
+        for c in corr_data.T:
+            l_obs.append(Obs([c], [ens_id], idl=[idx]))
 
     corr = Corr(l_obs)
     corr.tag = r", ".join(infos)
     return corr
 
 
+def read_meson_hd5(path, filestem, ens_id, meson='meson_0', idl=None, gammas=None):
+    r'''Read hadrons meson hdf5 file and extract the meson labeled 'meson'
+
+    Parameters
+    -----------------
+    path : str
+        path to the files to read
+    filestem : str
+        namestem of the files to read
+    ens_id : str
+        name of the ensemble, required for internal bookkeeping
+    meson : str
+        label of the meson to be extracted, standard value meson_0 which
+        corresponds to the pseudoscalar pseudoscalar two-point function.
+    gammas : tuple of strings
+        Instrad of a meson label one can also provide a tuple of two strings
+        indicating the gamma matrices at sink and source (gamma_snk, gamma_src).
+        ("Gamma5", "Gamma5") corresponds to the pseudoscalar pseudoscalar
+        two-point function. The gammas argument dominateds over meson.
+    idl : range
+        If specified only configurations in the given range are read in.
+
+    Returns
+    -------
+    corr : Corr
+        Correlator of the source sink combination in question.
+    '''
+    if gammas is None:
+        attrs = int(meson.rsplit('_', 1)[-1])
+    else:
+        if len(gammas) != 2:
+            raise ValueError("'gammas' needs to have exactly two entries")
+        attrs = {"gamma_snk": gammas[0],
+                 "gamma_src": gammas[1]}
+    return read_hd5(filestem=path + "/" + filestem, ens_id=ens_id,
+                    group=meson.rsplit('_', 1)[0], attrs=attrs, idl=idl,
+                    part="real")
+
+
 def _extract_real_arrays(path, files, tree, keys):
     corr_data = {}
     for key in keys:
         corr_data[key] = []
     for hd5_file in files:
         h5file = h5py.File(path + '/' + hd5_file, "r")
         for key in keys:
```

### Comparing `pyerrors-2.8.2/pyerrors/input/json.py` & `pyerrors-2.9.0/pyerrors/input/json.py`

 * *Files identical despite different names*

### Comparing `pyerrors-2.8.2/pyerrors/input/misc.py` & `pyerrors-2.9.0/pyerrors/input/misc.py`

 * *Files identical despite different names*

### Comparing `pyerrors-2.8.2/pyerrors/input/openQCD.py` & `pyerrors-2.9.0/pyerrors/input/openQCD.py`

 * *Files identical despite different names*

### Comparing `pyerrors-2.8.2/pyerrors/input/pandas.py` & `pyerrors-2.9.0/pyerrors/input/pandas.py`

 * *Files identical despite different names*

### Comparing `pyerrors-2.8.2/pyerrors/input/sfcf.py` & `pyerrors-2.9.0/pyerrors/input/sfcf.py`

 * *Files 0% similar despite different names*

```diff
@@ -282,36 +282,34 @@
             pattern += '\nwf_2      ' + str(wf2)
     return pattern
 
 
 def _find_correlator(file_name, version, pattern, b2b, silent=False):
     T = 0
 
-    file = open(file_name, "r")
+    with open(file_name, "r") as my_file:
+
+        content = my_file.read()
+        match = re.search(pattern, content)
+        if match:
+            if version == "0.0":
+                start_read = content.count('\n', 0, match.start()) + 1
+                T = content.count('\n', start_read)
+            else:
+                start_read = content.count('\n', 0, match.start()) + 5 + b2b
+                end_match = re.search(r'\n\s*\n', content[match.start():])
+                T = content[match.start():].count('\n', 0, end_match.start()) - 4 - b2b
+            if not T > 0:
+                raise ValueError("Correlator with pattern\n" + pattern + "\nis empty!")
+            if not silent:
+                print(T, 'entries, starting to read in line', start_read)
 
-    content = file.read()
-    match = re.search(pattern, content)
-    if match:
-        if version == "0.0":
-            start_read = content.count('\n', 0, match.start()) + 1
-            T = content.count('\n', start_read)
         else:
-            start_read = content.count('\n', 0, match.start()) + 5 + b2b
-            end_match = re.search(r'\n\s*\n', content[match.start():])
-            T = content[match.start():].count('\n', 0, end_match.start()) - 4 - b2b
-        if not T > 0:
-            raise ValueError("Correlator with pattern\n" + pattern + "\nis empty!")
-        if not silent:
-            print(T, 'entries, starting to read in line', start_read)
-
-    else:
-        file.close()
-        raise ValueError('Correlator with pattern\n' + pattern + '\nnot found.')
+            raise ValueError('Correlator with pattern\n' + pattern + '\nnot found.')
 
-    file.close()
     return start_read, T
 
 
 def _read_compact_file(rep_path, config_file, start_read, T, b2b, name, im):
     with open(rep_path + config_file) as fp:
         lines = fp.readlines()
         # check, if the correlator is in fact
```

### Comparing `pyerrors-2.8.2/pyerrors/input/utils.py` & `pyerrors-2.9.0/pyerrors/input/utils.py`

 * *Files identical despite different names*

### Comparing `pyerrors-2.8.2/pyerrors/linalg.py` & `pyerrors-2.9.0/pyerrors/linalg.py`

 * *Files identical despite different names*

### Comparing `pyerrors-2.8.2/pyerrors/misc.py` & `pyerrors-2.9.0/pyerrors/misc.py`

 * *Files identical despite different names*

### Comparing `pyerrors-2.8.2/pyerrors/mpm.py` & `pyerrors-2.9.0/pyerrors/mpm.py`

 * *Files identical despite different names*

### Comparing `pyerrors-2.8.2/pyerrors/obs.py` & `pyerrors-2.9.0/pyerrors/obs.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import warnings
 import hashlib
 import pickle
 import numpy as np
 import autograd.numpy as anp  # Thinly-wrapped numpy
+import scipy
 from autograd import jacobian
 import matplotlib.pyplot as plt
 from scipy.stats import skew, skewtest, kurtosis, kurtosistest
 import numdifftools as nd
 from itertools import groupby
 from .covobs import Covobs
 
@@ -623,15 +624,15 @@
         fig1, ax1 = plt.subplots()
         ax1.pie(sizes, labels=labels, startangle=90, normalize=True)
         ax1.axis('equal')
         plt.draw()
         if save:
             fig1.savefig(save)
 
-        return dict(zip(self.e_names, sizes))
+        return dict(zip(labels, sizes))
 
     def dump(self, filename, datatype="json.gz", description="", **kwargs):
         """Dump the Obs to a file 'name' of chosen format.
 
         Parameters
         ----------
         filename : str
@@ -680,14 +681,57 @@
         n = full_data.size
         mean = self.value
         tmp_jacks = np.zeros(n + 1)
         tmp_jacks[0] = mean
         tmp_jacks[1:] = (n * mean - full_data) / (n - 1)
         return tmp_jacks
 
+    def export_bootstrap(self, samples=500, random_numbers=None, save_rng=None):
+        """Export bootstrap samples from the Obs
+
+        Parameters
+        ----------
+        samples : int
+            Number of bootstrap samples to generate.
+        random_numbers : np.ndarray
+            Array of shape (samples, length) containing the random numbers to generate the bootstrap samples.
+            If not provided the bootstrap samples are generated bashed on the md5 hash of the enesmble name.
+        save_rng : str
+            Save the random numbers to a file if a path is specified.
+
+        Returns
+        -------
+        numpy.ndarray
+            Returns a numpy array of length N + 1 where N is the number of samples
+            for the given ensemble and replicum. The zeroth entry of the array contains
+            the mean value of the Obs, entries 1 to N contain the N import_bootstrap samples
+            derived from the Obs. The current implementation only works for observables
+            defined on exactly one ensemble and replicum. The derived bootstrap samples
+            should agree with samples from a full bootstrap analysis up to O(1/N).
+        """
+        if len(self.names) != 1:
+            raise Exception("'export_boostrap' is only implemented for Obs defined on one ensemble and replicum.")
+
+        name = self.names[0]
+        length = self.N
+
+        if random_numbers is None:
+            seed = int(hashlib.md5(name.encode()).hexdigest(), 16) & 0xFFFFFFFF
+            rng = np.random.default_rng(seed)
+            random_numbers = rng.integers(0, length, size=(samples, length))
+
+        if save_rng is not None:
+            np.savetxt(save_rng, random_numbers, fmt='%i')
+
+        proj = np.vstack([np.bincount(o, minlength=length) for o in random_numbers]) / length
+        ret = np.zeros(samples + 1)
+        ret[0] = self.value
+        ret[1:] = proj @ (self.deltas[name] + self.r_values[name])
+        return ret
+
     def __float__(self):
         return float(self.value)
 
     def __repr__(self):
         return 'Obs[' + str(self) + ']'
 
     def __str__(self):
@@ -725,19 +769,18 @@
     def __gt__(self, other):
         return self.value > other
 
     def __ge__(self, other):
         return self.value >= other
 
     def __eq__(self, other):
+        if other is None:
+            return False
         return (self - other).is_zero()
 
-    def __ne__(self, other):
-        return not (self - other).is_zero()
-
     # Overload math operations
     def __add__(self, y):
         if isinstance(y, Obs):
             return derived_observable(lambda x, **kwargs: x[0] + x[1], [self, y], man_grad=[1, 1])
         else:
             if isinstance(y, np.ndarray):
                 return np.array([self + o for o in y])
@@ -975,14 +1018,33 @@
 
     def __str__(self):
         return '(' + str(self.real) + int(self.imag >= 0.0) * '+' + str(self.imag) + 'j)'
 
     def __repr__(self):
         return 'CObs[' + str(self) + ']'
 
+    def __format__(self, format_type):
+        if format_type == "":
+            significance = 2
+            format_type = "2"
+        else:
+            significance = int(float(format_type.replace("+", "").replace("-", "")))
+        return f"({self.real:{format_type}}{self.imag:+{significance}}j)"
+
+
+def gamma_method(x, **kwargs):
+    """Vectorized version of the gamma_method applicable to lists or arrays of Obs.
+
+    See docstring of pe.Obs.gamma_method for details.
+    """
+    return np.vectorize(lambda o: o.gm(**kwargs))(x)
+
+
+gm = gamma_method
+
 
 def _format_uncertainty(value, dvalue, significance=2):
     """Creates a string of a value and its error in paranthesis notation, e.g., 13.02(45)"""
     if dvalue == 0.0 or (not np.isfinite(dvalue)):
         return str(value)
     if not isinstance(significance, int):
         raise TypeError("significance needs to be an integer.")
@@ -1546,14 +1608,44 @@
     samples = jacks[1:] @ prj
     mean = np.mean(samples)
     new_obs = Obs([samples - mean], [name], idl=idl, means=[mean])
     new_obs._value = jacks[0]
     return new_obs
 
 
+def import_bootstrap(boots, name, random_numbers):
+    """Imports bootstrap samples and returns an Obs
+
+    Parameters
+    ----------
+    boots : numpy.ndarray
+        numpy array containing the mean value as zeroth entry and
+        the N bootstrap samples as first to Nth entry.
+    name : str
+        name of the ensemble the samples are defined on.
+    random_numbers : np.ndarray
+        Array of shape (samples, length) containing the random numbers to generate the bootstrap samples,
+        where samples is the number of bootstrap samples and length is the length of the original Monte Carlo
+        chain to be reconstructed.
+    """
+    samples, length = random_numbers.shape
+    if samples != len(boots) - 1:
+        raise ValueError("Random numbers do not have the correct shape.")
+
+    if samples < length:
+        raise ValueError("Obs can't be reconstructed if there are fewer bootstrap samples than Monte Carlo data points.")
+
+    proj = np.vstack([np.bincount(o, minlength=length) for o in random_numbers]) / length
+
+    samples = scipy.linalg.lstsq(proj, boots[1:])[0]
+    ret = Obs([samples], [name])
+    ret._value = boots[0]
+    return ret
+
+
 def merge_obs(list_of_obs):
     """Combine all observables in list_of_obs into one new observable
 
     Parameters
     ----------
     list_of_obs : list
         list of the Obs object to be combined
```

### Comparing `pyerrors-2.8.2/pyerrors/roots.py` & `pyerrors-2.9.0/pyerrors/roots.py`

 * *Files identical despite different names*

### Comparing `pyerrors-2.8.2/pyerrors.egg-info/SOURCES.txt` & `pyerrors-2.9.0/pyerrors.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -33,14 +33,15 @@
 examples/data/matrix_correlator_V2V2.json.gz
 examples/data/matrix_correlator_V3V3.json.gz
 pyerrors/__init__.py
 pyerrors/correlators.py
 pyerrors/covobs.py
 pyerrors/dirac.py
 pyerrors/fits.py
+pyerrors/integrate.py
 pyerrors/linalg.py
 pyerrors/misc.py
 pyerrors/mpm.py
 pyerrors/obs.py
 pyerrors/roots.py
 pyerrors/version.py
 pyerrors.egg-info/PKG-INFO
@@ -59,24 +60,26 @@
 pyerrors/input/sfcf.py
 pyerrors/input/utils.py
 tests/benchmark_test.py
 tests/correlators_test.py
 tests/covobs_test.py
 tests/dirac_test.py
 tests/fits_test.py
+tests/integrate_test.py
 tests/json_io_test.py
 tests/linalg_test.py
 tests/misc_test.py
 tests/mpm_test.py
 tests/obs_test.py
 tests/openQCD_in_test.py
 tests/pandas_test.py
 tests/roots_test.py
 tests/sfcf_in_test.py
 tests/utils_in_test.py
+tests/data/compute_drho_fails.json.gz
 tests/data/openqcd_test/ms5_xsf_T24L16r1.ms5_xsf_dd.dat
 tests/data/openqcd_test/ms5_xsf_T24L16r2.ms5_xsf_dd.dat
 tests/data/openqcd_test/ms5_xsf_T24L16r3.ms5_xsf_dd.dat
 tests/data/openqcd_test/openqcd2r1.ms.dat
 tests/data/openqcd_test/openqcd2r1.ms1.dat
 tests/data/openqcd_test/sfqcdr1.gfms.dat
 tests/data/openqcd_test/sfqcdr1.rwms.dat
```

### Comparing `pyerrors-2.8.2/setup.py` & `pyerrors-2.9.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -20,23 +20,22 @@
         'Bug Tracker':   'https://github.com/fjosw/pyerrors/issues',
         'Changelog' :    'https://github.com/fjosw/pyerrors/blob/master/CHANGELOG.md'
       },
       author='Fabian Joswig',
       author_email='fabian.joswig@ed.ac.uk',
       license="MIT",
       packages=find_packages(),
-      python_requires='>=3.7.0',
-      install_requires=['numpy>=1.21,<1.25', 'autograd>=1.5', 'numdifftools>=0.9.41', 'matplotlib>=3.5', 'scipy>=1.7', 'iminuit>=2.17', 'h5py>=3.8', 'lxml>=4.9', 'python-rapidjson>=1.9', 'pandas>=1.1'],
-      extras_require={'test': ['pytest', 'pytest-cov', 'pytest-benchmark', 'hypothesis']},
+      python_requires='>=3.8.0',
+      install_requires=['numpy>=1.24', 'autograd>=1.6.2', 'numdifftools>=0.9.41', 'matplotlib>=3.7', 'scipy>=1.10', 'iminuit>=2.21', 'h5py>=3.8', 'lxml>=4.9', 'python-rapidjson>=1.10', 'pandas>=2.0'],
+      extras_require={'test': ['pytest', 'pytest-cov', 'pytest-benchmark', 'hypothesis', 'nbmake', 'flake8']},
       classifiers=[
           'Development Status :: 5 - Production/Stable',
           'Intended Audience :: Science/Research',
           'License :: OSI Approved :: MIT License',
           'Programming Language :: Python :: 3',
-          'Programming Language :: Python :: 3.7',
           'Programming Language :: Python :: 3.8',
           'Programming Language :: Python :: 3.9',
           'Programming Language :: Python :: 3.10',
           'Programming Language :: Python :: 3.11',
           'Topic :: Scientific/Engineering :: Physics'
       ],
      )
```

### Comparing `pyerrors-2.8.2/tests/benchmark_test.py` & `pyerrors-2.9.0/tests/benchmark_test.py`

 * *Files identical despite different names*

### Comparing `pyerrors-2.8.2/tests/correlators_test.py` & `pyerrors-2.9.0/tests/correlators_test.py`

 * *Files 14% similar despite different names*

```diff
@@ -54,20 +54,24 @@
         corr.symmetric()
     with pytest.warns(RuntimeWarning):
         corr.anti_symmetric()
 
     for pad in [0, 2]:
         corr = pe.Corr(corr_content, padding=[pad, pad])
         corr.roll(np.random.randint(100))
-        corr.deriv(variant="forward")
         corr.deriv(variant="symmetric")
+        corr.deriv(variant="forward")
+        corr.deriv(variant="backward")
         corr.deriv(variant="improved")
+        corr.deriv(variant="log")
         corr.deriv().deriv()
         corr.second_deriv(variant="symmetric")
+        corr.second_deriv(variant="big_symmetric")
         corr.second_deriv(variant="improved")
+        corr.second_deriv(variant="log")
         corr.second_deriv().second_deriv()
 
     for i, e in enumerate(corr.content):
         corr.content[i] = None
 
     for func in [pe.Corr.deriv, pe.Corr.second_deriv]:
         for variant in ["symmetric", "improved", "forward", "gibberish", None]:
@@ -562,7 +566,186 @@
     for corr in [pe.Corr([obs[0] + 8, obs[1], obs[2], obs[3]]),
                  pe.Corr([obs[0] + 8, obs[1], obs[2], None]),
                  pe.Corr([None, obs[1], obs[2], obs[3]])]:
         scorr = corr.symmetric()
         assert scorr[1] == scorr[3]
         assert scorr[2] == corr[2]
         assert scorr[0] == corr[0]
+
+
+def test_corr_array_ndim1_init():
+    y = [pe.pseudo_Obs(2 + np.random.normal(0.0, 0.1), .1, 't') for i in np.arange(5)]
+    cc1 = pe.Corr(y)
+    cc2 = pe.Corr(np.array(y))
+    assert np.all([o1 == o2 for o1, o2 in zip(cc1, cc2)])
+
+
+def test_corr_array_ndim3_init():
+    y = np.array([pe.pseudo_Obs(np.random.normal(2.0, 0.1), .1, 't') for i in np.arange(12)]).reshape(3, 2, 2)
+    tt1 = pe.Corr(list(y))
+    tt2 = pe.Corr(y)
+    tt3 = pe.Corr(np.array([pe.Corr(o) for o in y.reshape(3, 4).T]).reshape(2, 2))
+    assert np.all([o1 == o2 for o1, o2 in zip(tt1, tt2)])
+    assert np.all([o1 == o2 for o1, o2 in zip(tt1, tt3)])
+    assert tt1.T == y.shape[0]
+    assert tt1.N == y.shape[1] == y.shape[2]
+
+    with pytest.raises(ValueError):
+        pe.Corr(y.reshape(6, 2, 1))
+
+
+def test_two_matrix_corr_inits():
+    T = 4
+    rn = lambda : np.random.normal(0.5, 0.1)
+
+    # Generate T random CObs in a list
+    list_of_timeslices =[]
+    for i in range(T):
+        re = pe.pseudo_Obs(rn(), rn(), "test")
+        im = pe.pseudo_Obs(rn(), rn(), "test")
+        list_of_timeslices.append(pe.CObs(re, im))
+
+    # First option: Correlator of matrix of correlators
+    corr = pe.Corr(list_of_timeslices)
+    mat_corr1 = pe.Corr(np.array([[corr, corr], [corr, corr]]))
+
+    # Second option: Correlator of list of arrays per timeslice
+    list_of_arrays = [np.array([[elem, elem], [elem, elem]]) for elem in list_of_timeslices]
+    mat_corr2 = pe.Corr(list_of_arrays)
+
+    for el in mat_corr1 - mat_corr2:
+        assert np.all(el == 0)
+
+
+def test_matmul_overloading():
+    N = 4
+    rn = lambda : np.random.normal(0.5, 0.1)
+
+    # Generate N^2 random CObs and assemble them in an array
+    ll =[]
+    for i in range(N ** 2):
+        re = pe.pseudo_Obs(rn(), rn(), "test")
+        im = pe.pseudo_Obs(rn(), rn(), "test")
+        ll.append(pe.CObs(re, im))
+    mat = np.array(ll).reshape(N, N)
+
+    # Multiply with gamma matrix
+    corr = pe.Corr([mat] * 4, padding=[0, 1])
+
+    # __matmul__
+    mcorr = corr @ pe.dirac.gammaX
+    comp = mat @ pe.dirac.gammaX
+    for i in range(4):
+        assert np.all(mcorr[i] == comp)
+
+    # __rmatmul__
+    mcorr = pe.dirac.gammaX @ corr
+    comp = pe.dirac.gammaX @ mat
+    for i in range(4):
+        assert np.all(mcorr[i] == comp)
+
+    test_mat = pe.dirac.gamma5 + pe.dirac.gammaX
+    icorr = corr @ test_mat @ np.linalg.inv(test_mat)
+    tt = corr - icorr
+    for i in range(4):
+        assert np.all(tt[i] == 0)
+
+    # associative property
+    tt = (corr.real @ pe.dirac.gammaX + corr.imag @ (pe.dirac.gammaX * 1j)) - corr @ pe.dirac.gammaX
+    for el in tt:
+        if el is not None:
+            assert np.all(el == 0)
+
+    corr2 = corr @ corr
+    for i in range(4):
+        np.all(corr2[i] == corr[i] @ corr[i])
+
+
+def test_matrix_trace():
+    N = 4
+    rn = lambda : np.random.normal(0.5, 0.1)
+
+    # Generate N^2 random CObs and assemble them in an array
+    ll =[]
+    for i in range(N ** 2):
+        re = pe.pseudo_Obs(rn(), rn(), "test")
+        im = pe.pseudo_Obs(rn(), rn(), "test")
+        ll.append(pe.CObs(re, im))
+    mat = np.array(ll).reshape(N, N)
+
+    corr = pe.Corr([mat] * 4)
+
+    # Explicitly check trace
+    for el in corr.trace():
+        el == np.sum(np.diag(mat))
+
+    # Trace is cyclic
+    for one, two in zip((pe.dirac.gammaX @ corr).trace(), (corr @ pe.dirac.gammaX).trace()):
+        assert np.all(one == two)
+
+    # Antisymmetric matrices are traceless.
+    mat = (mat - mat.T) / 2
+    corr = pe.Corr([mat] * 4)
+    for el in corr.trace():
+        assert el == 0
+
+
+    with pytest.raises(ValueError):
+        corr.item(0, 0).trace()
+
+
+def test_corr_roll():
+    T = 4
+    rn = lambda : np.random.normal(0.5, 0.1)
+
+    ll = []
+    for i in range(T):
+        re = pe.pseudo_Obs(rn(), rn(), "test")
+        im = pe.pseudo_Obs(rn(), rn(), "test")
+        ll.append(pe.CObs(re, im))
+
+    # Rolling by T should produce the same correlator
+    corr = pe.Corr(ll)
+    tt = corr - corr.roll(T)
+    for el in tt:
+        assert np.all(el == 0)
+
+    mcorr = pe.Corr(np.array([[corr, corr + 0.1], [corr - 0.1, 2 * corr]]))
+    tt = mcorr.roll(T) - mcorr
+    for el in tt:
+        assert np.all(el == 0)
+
+
+def test_correlator_comparison():
+    scorr = pe.Corr([pe.pseudo_Obs(0.3, 0.1, "test") for o in range(4)])
+    mcorr = pe.Corr(np.array([[scorr, scorr], [scorr, scorr]]))
+    for corr in [scorr, mcorr]:
+        assert (corr == corr).all()
+        assert np.all(corr == 1 * corr)
+        assert np.all(corr == (1 + 1e-16) * corr)
+        assert not np.all(corr == (1 + 1e-5) * corr)
+        assert np.all(corr == 1 / (1 / corr))
+        assert np.all(corr - corr == 0)
+        assert np.all(corr * 0 == 0)
+        assert np.all(0 * corr == 0)
+        assert np.all(0 * corr + scorr[2] == scorr[2])
+        assert np.all(-corr == 0 - corr)
+        assert np.all(corr ** 2 == corr * corr)
+    acorr = pe.Corr([scorr[0]] * 6)
+    assert np.all(acorr == scorr[0])
+    assert not np.all(acorr == scorr[1])
+
+    mcorr[1][0, 1] = None
+    assert not np.all(mcorr == pe.Corr(np.array([[scorr, scorr], [scorr, scorr]])))
+
+    pcorr = pe.Corr([pe.pseudo_Obs(0.25, 0.1, "test") for o in range(2)], padding=[1, 1])
+    assert np.all(pcorr == pcorr)
+    assert np.all(1 * pcorr == pcorr)
+
+
+def test_corr_item():
+    corr_aa = _gen_corr(1)
+    corr_ab = 0.5 * corr_aa
+
+    corr_mat = pe.Corr(np.array([[corr_aa, corr_ab], [corr_ab, corr_aa]]))
+    corr_mat.item(0, 0)
+    assert corr_mat[0].item(0, 1) == corr_mat.item(0, 1)[0]
```

### Comparing `pyerrors-2.8.2/tests/covobs_test.py` & `pyerrors-2.9.0/tests/covobs_test.py`

 * *Files identical despite different names*

### Comparing `pyerrors-2.8.2/tests/data/openqcd_test/ms5_xsf_T24L16r1.ms5_xsf_dd.dat` & `pyerrors-2.9.0/tests/data/openqcd_test/ms5_xsf_T24L16r1.ms5_xsf_dd.dat`

 * *Files identical despite different names*

### Comparing `pyerrors-2.8.2/tests/data/openqcd_test/ms5_xsf_T24L16r2.ms5_xsf_dd.dat` & `pyerrors-2.9.0/tests/data/openqcd_test/ms5_xsf_T24L16r2.ms5_xsf_dd.dat`

 * *Files identical despite different names*

### Comparing `pyerrors-2.8.2/tests/data/openqcd_test/ms5_xsf_T24L16r3.ms5_xsf_dd.dat` & `pyerrors-2.9.0/tests/data/openqcd_test/ms5_xsf_T24L16r3.ms5_xsf_dd.dat`

 * *Files identical despite different names*

### Comparing `pyerrors-2.8.2/tests/data/openqcd_test/openqcd2r1.ms.dat` & `pyerrors-2.9.0/tests/data/openqcd_test/openqcd2r1.ms.dat`

 * *Files identical despite different names*

### Comparing `pyerrors-2.8.2/tests/data/openqcd_test/openqcd2r1.ms1.dat` & `pyerrors-2.9.0/tests/data/openqcd_test/openqcd2r1.ms1.dat`

 * *Files identical despite different names*

### Comparing `pyerrors-2.8.2/tests/data/openqcd_test/sfqcdr1.gfms.dat` & `pyerrors-2.9.0/tests/data/openqcd_test/sfqcdr1.gfms.dat`

 * *Files identical despite different names*

### Comparing `pyerrors-2.8.2/tests/data/sfcf_test/broken_data_c/data_c_r0/data_c_r0_n1` & `pyerrors-2.9.0/tests/data/sfcf_test/broken_data_c/data_c_r0/data_c_r0_n1`

 * *Files identical despite different names*

### Comparing `pyerrors-2.8.2/tests/data/sfcf_test/data_a/data_a_r0.F_V0` & `pyerrors-2.9.0/tests/data/sfcf_test/data_a/data_a_r0.F_V0`

 * *Files identical despite different names*

### Comparing `pyerrors-2.8.2/tests/data/sfcf_test/data_a/data_a_r0.f_1` & `pyerrors-2.9.0/tests/data/sfcf_test/data_a/data_a_r0.f_1`

 * *Files identical despite different names*

### Comparing `pyerrors-2.8.2/tests/data/sfcf_test/data_a/data_a_r0.f_A` & `pyerrors-2.9.0/tests/data/sfcf_test/data_a/data_a_r0.f_A`

 * *Files identical despite different names*

### Comparing `pyerrors-2.8.2/tests/data/sfcf_test/data_c/data_c_r0/data_c_r0_n1` & `pyerrors-2.9.0/tests/data/sfcf_test/data_c/data_c_r0/data_c_r0_n1`

 * *Files identical despite different names*

### Comparing `pyerrors-2.8.2/tests/data/sfcf_test/data_o/test_r0/cfg1/F_V0` & `pyerrors-2.9.0/tests/data/sfcf_test/data_o/test_r0/cfg1/F_V0`

 * *Files identical despite different names*

### Comparing `pyerrors-2.8.2/tests/data/sfcf_test/data_o/test_r0/cfg1/f_1` & `pyerrors-2.9.0/tests/data/sfcf_test/data_o/test_r0/cfg1/f_1`

 * *Files identical despite different names*

### Comparing `pyerrors-2.8.2/tests/data/sfcf_test/data_o/test_r0/cfg1/f_A` & `pyerrors-2.9.0/tests/data/sfcf_test/data_o/test_r0/cfg1/f_A`

 * *Files identical despite different names*

### Comparing `pyerrors-2.8.2/tests/data/sfcf_test/param/out.out` & `pyerrors-2.9.0/tests/data/sfcf_test/param/out.out`

 * *Files identical despite different names*

### Comparing `pyerrors-2.8.2/tests/data/sfcf_test/param/parameters_a` & `pyerrors-2.9.0/tests/data/sfcf_test/param/parameters_a`

 * *Files identical despite different names*

### Comparing `pyerrors-2.8.2/tests/data/sfcf_test/param/parameters_c` & `pyerrors-2.9.0/tests/data/sfcf_test/param/parameters_c`

 * *Files identical despite different names*

### Comparing `pyerrors-2.8.2/tests/data/sfcf_test/param/parameters_o` & `pyerrors-2.9.0/tests/data/sfcf_test/param/parameters_o`

 * *Files identical despite different names*

### Comparing `pyerrors-2.8.2/tests/dirac_test.py` & `pyerrors-2.9.0/tests/dirac_test.py`

 * *Files identical despite different names*

### Comparing `pyerrors-2.8.2/tests/fits_test.py` & `pyerrors-2.9.0/tests/fits_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -231,31 +231,31 @@
         assert np.isclose(out.dof, out_corr.dof)
         assert np.isclose(out.chisquare_by_dof, out_corr.chisquare_by_dof)
         assert (out[0] - out_corr[0]).is_zero(atol=1e-4)
         assert (out[1] - out_corr[1]).is_zero(atol=1e-4)
 
 
 def test_linear_fit_guesses():
-    for err in [10, 0.1, 0.001]:
+    for err in [1.2, 0.1, 0.001]:
         xvals = []
         yvals = []
         for x in range(1, 8, 2):
             xvals.append(x)
-            yvals.append(pe.pseudo_Obs(x + np.random.normal(0.0, err), err, 'test1') + pe.pseudo_Obs(0, err / 100, 'test2', samples=87))
+            yvals.append(pe.pseudo_Obs(x + np.random.normal(0.0, err), err, 'test1') + pe.pseudo_Obs(0, err / 97, 'test2', samples=87))
         lin_func = lambda a, x: a[0] + a[1] * x
         with pytest.raises(Exception):
             pe.least_squares(xvals, yvals, lin_func)
         [o.gamma_method() for o in yvals]
         with pytest.raises(Exception):
             pe.least_squares(xvals, yvals, lin_func, initial_guess=[5])
 
         bad_guess = pe.least_squares(xvals, yvals, lin_func, initial_guess=[999, 999])
         good_guess = pe.least_squares(xvals, yvals, lin_func, initial_guess=[0, 1])
         assert np.isclose(bad_guess.chisquare, good_guess.chisquare, atol=1e-8)
-        assert np.all([(go - ba).is_zero(atol=1e-6) for (go, ba) in zip(good_guess, bad_guess)])
+        assert np.all([(go - ba).is_zero(atol=5e-5) for (go, ba) in zip(good_guess, bad_guess)])
 
 
 def test_total_least_squares():
     dim = 10 + int(30 * np.random.rand())
     x = np.arange(dim) + np.random.normal(0.0, 0.15, dim)
     xerr = 0.1 + 0.1 * np.random.rand(dim)
     y = 2 * np.exp(-0.06 * x) + np.random.normal(0.0, 0.15, dim)
@@ -1139,14 +1139,31 @@
             cd.append(fr.chisquare_by_dof)
 
     assert np.allclose(dof, [0, 1, 1, 2])
     assert cd[0] != cd[0]  # Check for nan
     assert np.all(np.array(cd[1:]) > 0)
 
 
+def test_combined_fit_constant_shape():
+    N1 = 16
+    N2 = 10
+    x = {"a": np.arange(N1),
+         "": np.arange(N2)}
+    y = {"a": [pe.pseudo_Obs(o + np.random.normal(0.0, 0.1), 0.1, "test") for o in range(N1)],
+         "": [pe.pseudo_Obs(o + np.random.normal(0.0, 0.1), 0.1, "test") for o in range(N2)]}
+    funcs = {"a": lambda a, x: a[0] + a[1] * x,
+             "": lambda a, x: a[1]}
+    with pytest.raises(ValueError):
+        pe.fits.least_squares(x, y, funcs, method='migrad')
+
+    funcs = {"a": lambda a, x: a[0] + a[1] * x,
+             "": lambda a, x: a[1] + x * 0}
+    pe.fits.least_squares(x, y, funcs, method='migrad')
+
+
 def fit_general(x, y, func, silent=False, **kwargs):
     """Performs a non-linear fit to y = func(x) and returns a list of Obs corresponding to the fit parameters.
 
     Plausibility of the results should be checked. To control the numerical differentiation
     the kwargs of numdifftools.step_generators.MaxStepGenerator can be used.
 
     func has to be of the form
```

### Comparing `pyerrors-2.8.2/tests/json_io_test.py` & `pyerrors-2.9.0/tests/json_io_test.py`

 * *Files identical despite different names*

### Comparing `pyerrors-2.8.2/tests/linalg_test.py` & `pyerrors-2.9.0/tests/linalg_test.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -10,17 +10,17 @@
 def get_real_matrix(dimension):
     base_matrix = np.empty((dimension, dimension), dtype=object)
     for (n, m), entry in np.ndenumerate(base_matrix):
         exponent_real = np.random.normal(0, 1)
         exponent_imag = np.random.normal(0, 1)
         base_matrix[n, m] = pe.Obs([np.random.normal(1.0, 0.1, 100)], ['t'])
 
-
     return base_matrix
 
+
 def get_complex_matrix(dimension):
     base_matrix = np.empty((dimension, dimension), dtype=object)
     for (n, m), entry in np.ndenumerate(base_matrix):
         exponent_real = np.random.normal(0, 1)
         exponent_imag = np.random.normal(0, 1)
         base_matrix[n, m] = pe.CObs(pe.Obs([np.random.normal(1.0, 0.1, 100)], ['t']),
                                     pe.Obs([np.random.normal(1.0, 0.1, 100)], ['t']))
@@ -105,15 +105,14 @@
     def _perform_complex_check(arr):
         [o.gamma_method() for o in arr]
         assert np.all([o.real.is_zero_within_error(0.001) for o in arr])
         assert np.all([o.real.dvalue < 0.001 for o in arr])
         assert np.all([o.imag.is_zero_within_error(0.001) for o in arr])
         assert np.all([o.imag.dvalue < 0.001 for o in arr])
 
-
     tt = [get_real_matrix(4), get_real_matrix(3)]
     q = np.tensordot(tt[0], tt[1], 0)
     c1 = tt[1] @ q
     c2 = pe.linalg.einsum('ij,abjd->abid', tt[1], q)
     check1 = c1 - c2
     _perform_real_check(check1.ravel())
     check2 = np.trace(tt[0]) - pe.linalg.einsum('ii', tt[0])
@@ -351,7 +350,8 @@
 
 
 def test_complex_matrix_real_entries():
     my_mat = get_complex_matrix(4)
     my_mat[0, 1] = 4
     my_mat[2, 0] = pe.Obs([np.random.normal(1.0, 0.1, 100)], ['t'])
     assert np.all((my_mat @ pe.linalg.inv(my_mat) - np.identity(4)) == 0)
+
```

### Comparing `pyerrors-2.8.2/tests/misc_test.py` & `pyerrors-2.9.0/tests/misc_test.py`

 * *Files 14% similar despite different names*

```diff
@@ -14,7 +14,11 @@
 
     for xerr in [2, None]:
         for yerr in [0.1, None]:
             pe.errorbar(x_float, y_obs, marker="x", ms=2, xerr=xerr, yerr=yerr)
             pe.errorbar(x_obs, y_obs, marker="x", ms=2, xerr=xerr, yerr=yerr)
 
     plt.close('all')
+
+
+def test_print_config():
+    pe.print_config()
```

### Comparing `pyerrors-2.8.2/tests/obs_test.py` & `pyerrors-2.9.0/tests/obs_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-import autograd.numpy as np
+import numpy as np
+import autograd.numpy as anp
 import os
 import copy
 import matplotlib.pyplot as plt
 import pyerrors as pe
 import pytest
 from hypothesis import given, strategies as st
 
@@ -98,14 +99,15 @@
 
 
 def test_comparison():
     value1 = np.random.normal(0, 100)
     test_obs1 = pe.pseudo_Obs(value1, 0.1, 't')
     value2 = np.random.normal(0, 100)
     test_obs2 = pe.pseudo_Obs(value2, 0.1, 't')
+    assert test_obs1 != None
     assert (value1 > value2) == (test_obs1 > test_obs2)
     assert (value1 < value2) == (test_obs1 < test_obs2)
     assert (value1 >= value2) == (test_obs1 >= test_obs2)
     assert (value1 <= value2) == (test_obs1 <= test_obs2)
     assert test_obs1 >= test_obs1
     assert test_obs2 <= test_obs2
     assert test_obs1 == test_obs1
@@ -122,17 +124,17 @@
 
 def test_function_overloading():
     a = pe.pseudo_Obs(17, 2.9, 'e1')
     b = pe.pseudo_Obs(4, 0.8, 'e1')
 
     fs = [lambda x: x[0] + x[1], lambda x: x[1] + x[0], lambda x: x[0] - x[1], lambda x: x[1] - x[0],
           lambda x: x[0] * x[1], lambda x: x[1] * x[0], lambda x: x[0] / x[1], lambda x: x[1] / x[0],
-          lambda x: np.exp(x[0]), lambda x: np.sin(x[0]), lambda x: np.cos(x[0]), lambda x: np.tan(x[0]),
-          lambda x: np.log(x[0]), lambda x: np.sqrt(np.abs(x[0])),
-          lambda x: np.sinh(x[0]), lambda x: np.cosh(x[0]), lambda x: np.tanh(x[0])]
+          lambda x: anp.exp(x[0]), lambda x: anp.sin(x[0]), lambda x: anp.cos(x[0]), lambda x: anp.tan(x[0]),
+          lambda x: anp.log(x[0]), lambda x: anp.sqrt(anp.abs(x[0])),
+          lambda x: anp.sinh(x[0]), lambda x: anp.cosh(x[0]), lambda x: anp.tanh(x[0])]
 
     for i, f in enumerate(fs):
         t1 = f([a, b])
         t2 = pe.derived_observable(f, [a, b])
         c = t2 - t1
         assert c.is_zero()
 
@@ -302,17 +304,17 @@
 
 
 def test_derived_observables():
     # Construct pseudo Obs with random shape
     test_obs = pe.pseudo_Obs(2, 0.1 * (1 + np.random.rand()), 't', int(1000 * (1 + np.random.rand())))
 
     # Check if autograd and numgrad give the same result
-    d_Obs_ad = pe.derived_observable(lambda x, **kwargs: x[0] * x[1] * np.sin(x[0] * x[1]), [test_obs, test_obs])
+    d_Obs_ad = pe.derived_observable(lambda x, **kwargs: x[0] * x[1] * anp.sin(x[0] * x[1]), [test_obs, test_obs])
     d_Obs_ad.gamma_method()
-    d_Obs_fd = pe.derived_observable(lambda x, **kwargs: x[0] * x[1] * np.sin(x[0] * x[1]), [test_obs, test_obs], num_grad=True)
+    d_Obs_fd = pe.derived_observable(lambda x, **kwargs: x[0] * x[1] * anp.sin(x[0] * x[1]), [test_obs, test_obs], num_grad=True)
     d_Obs_fd.gamma_method()
 
     assert d_Obs_ad == d_Obs_fd
     assert np.abs(4.0 * np.sin(4.0) - d_Obs_ad.value) < 1000 * np.finfo(np.float64).eps * np.abs(d_Obs_ad.value)
     assert np.abs(d_Obs_ad.dvalue-d_Obs_fd.dvalue) < 1000 * np.finfo(np.float64).eps * d_Obs_ad.dvalue
 
     i_am_one = pe.derived_observable(lambda x, **kwargs: x[0] / x[1], [d_Obs_ad, d_Obs_ad])
@@ -1090,14 +1092,28 @@
     full_data = np.random.normal(1.105, 0.021, 754)
     my_obs = pe.Obs([full_data], ['test'])
     my_jacks = my_obs.export_jackknife()
     reconstructed_obs = pe.import_jackknife(my_jacks, 'test')
     assert my_obs == reconstructed_obs
 
 
+def test_import_bootstrap():
+    seed = 4321
+    samples = 1234
+    length = 820
+    name = "test"
+
+    rng = np.random.default_rng(seed)
+    random_numbers = rng.integers(0, length, size=(samples, length))
+    obs = pe.pseudo_Obs(2.447, 0.14, name, length)
+    boots = obs.export_bootstrap(1234, random_numbers=random_numbers)
+    re_obs = pe.import_bootstrap(boots, name, random_numbers=random_numbers)
+    assert obs == re_obs
+
+
 def test_reduce_deltas():
     idx_old = range(1, 101)
     deltas = [float(i) for i in idx_old]
     idl = [
         range(2, 26, 2),
         range(1, 101),
         np.arange(1, 101),
@@ -1265,25 +1281,55 @@
     assert pe.obs._format_uncertainty(0.548, 2.48497, 2) == '0.5(2.5)'
     assert pe.obs._format_uncertainty(0.548, 2.48497, 4) == '0.548(2.485)'
     assert pe.obs._format_uncertainty(0.548, 20078.3, 9) == '0.5480(20078.3000)'
     pe.obs._format_uncertainty(np.NaN, 1)
     pe.obs._format_uncertainty(1, np.NaN)
     pe.obs._format_uncertainty(np.NaN, np.inf)
 
+
 def test_format():
     o1 = pe.pseudo_Obs(0.348, 0.0123, "test")
     assert o1.__format__("+3") == '+0.3480(123)'
     assert o1.__format__("+2") == '+0.348(12)'
     assert o1.__format__(" 2") == ' 0.348(12)'
 
+
 def test_f_string_obs():
     o1 = pe.pseudo_Obs(0.348, 0.0123, "test")
     print(f"{o1}")
     print(f"{o1:3}")
     print(f"{o1:+3}")
     print(f"{o1:-1}")
     print(f"{o1: 8}")
 
+
+def test_f_string_cobs():
+    o_real = pe.pseudo_Obs(0.348, 0.0123, "test")
+    o_imag = pe.pseudo_Obs(0.348, 0.0123, "test")
+    o1 = pe.CObs(o_real, o_imag)
+    print(f"{o1}")
+    print(f"{o1:3}")
+    print(f"{o1:+3}")
+    print(f"{o1:-1}")
+    print(f"{o1: 8}")
+
+
 def test_compute_drho_fails():
     obs = pe.input.json.load_json("tests/data/compute_drho_fails.json.gz")
     obs.gm()
     assert np.isclose(obs.dvalue, 0.0022150779611891094)
+
+
+def test_vec_gm():
+    obs = pe.misc.gen_correlated_data(np.arange(3), np.array([[0.0364    , 0.03627262, 0.03615699],
+           [0.03627262, 0.03688438, 0.03674798],
+           [0.03615699, 0.03674798, 0.03732882]]), "qq", 3.8, 1000)
+    pe.gm(obs[0], S=0)
+    assert obs[0].S["qq"] == 0
+    pe.gm(obs, S=1.3)
+    assert np.all(np.vectorize(lambda x: x.S["qq"])(obs) == 1.3)
+    aa = np.array([obs, obs, obs])
+    pe.gamma_method(aa, S=2.2)
+    assert np.all(np.vectorize(lambda x: x.S["qq"])(aa) == 2.20)
+    cc = pe.Corr(obs)
+    pe.gm(cc, S=4.12)
+    assert np.all(np.vectorize(lambda x: x.S["qq"])(cc.content) == 4.12)
```

### Comparing `pyerrors-2.8.2/tests/openQCD_in_test.py` & `pyerrors-2.9.0/tests/openQCD_in_test.py`

 * *Files identical despite different names*

### Comparing `pyerrors-2.8.2/tests/pandas_test.py` & `pyerrors-2.9.0/tests/pandas_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,18 +42,17 @@
                "float": -0.01,
                "Obs1": pe.pseudo_Obs(87, 21, "test_ensemble"),
                "Obs2": pe.pseudo_Obs(-87, 21, "test_ensemble2")}
     my_df = pd.DataFrame([my_dict] * 4)
     my_df.loc[1, "int"] = np.nan
 
     for gz in [True, False]:
-        pe.input.pandas.dump_df(my_df, (tmp_path / 'df_output').as_posix(), gz=gz)
-        reconstructed_df = pe.input.pandas.load_df((tmp_path / 'df_output').as_posix(), auto_gamma=True, gz=gz)
         with pytest.warns(UserWarning, match="nan value in column int will be replaced by None"):
-            warnings.warn("nan value in column int will be replaced by None", UserWarning)
+            pe.input.pandas.dump_df(my_df, (tmp_path / 'df_output').as_posix(), gz=gz)
+        reconstructed_df = pe.input.pandas.load_df((tmp_path / 'df_output').as_posix(), auto_gamma=True, gz=gz)
         assert reconstructed_df.loc[1, "int"] is None
         assert np.all(reconstructed_df.loc[:, "float"] == my_df.loc[:, "float"])
         assert np.all(reconstructed_df.loc[:, "Obs1"] == my_df.loc[:, "Obs1"])
         assert np.all(reconstructed_df.loc[:, "Obs2"] == my_df.loc[:, "Obs2"])
 
 
 def test_null_second_line_df_export_import(tmp_path):
```

### Comparing `pyerrors-2.8.2/tests/roots_test.py` & `pyerrors-2.9.0/tests/roots_test.py`

 * *Files identical despite different names*

### Comparing `pyerrors-2.8.2/tests/sfcf_in_test.py` & `pyerrors-2.9.0/tests/sfcf_in_test.py`

 * *Files identical despite different names*

### Comparing `pyerrors-2.8.2/tests/utils_in_test.py` & `pyerrors-2.9.0/tests/utils_in_test.py`

 * *Files identical despite different names*

