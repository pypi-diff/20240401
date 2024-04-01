# Comparing `tmp/pm4pyminimal-2.7.9.3.tar.gz` & `tmp/pm4pyminimal-2.7.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pm4pyminimal-2.7.9.3.tar", last modified: Tue Jan 16 10:11:43 2024, max compression
+gzip compressed data, was "pm4pyminimal-2.7.9.4.tar", last modified: Mon Jan 29 06:15:34 2024, max compression
```

## Comparing `pm4pyminimal-2.7.9.3.tar` & `pm4pyminimal-2.7.9.4.tar`

### file list

```diff
@@ -1,1804 +1,1804 @@
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:43.188238 pm4pyminimal-2.7.9.3/
--rw-rw-rw-   0        0        0    34817 2023-12-11 09:33:50.000000 pm4pyminimal-2.7.9.3/LICENSE
--rw-rw-rw-   0        0        0       29 2024-01-04 13:34:19.000000 pm4pyminimal-2.7.9.3/MANIFEST.in
--rw-rw-rw-   0        0        0     3369 2024-01-16 10:11:43.186243 pm4pyminimal-2.7.9.3/PKG-INFO
--rw-rw-rw-   0        0        0     2790 2024-01-16 10:10:16.000000 pm4pyminimal-2.7.9.3/README.md
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:39.836766 pm4pyminimal-2.7.9.3/pm4py/
--rw-rw-rw-   0        0        0     7677 2024-01-16 10:09:19.000000 pm4pyminimal-2.7.9.3/pm4py/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:39.839893 pm4pyminimal-2.7.9.3/pm4py/algo/
--rw-rw-rw-   0        0        0      854 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:39.841888 pm4pyminimal-2.7.9.3/pm4py/algo/analysis/
--rw-rw-rw-   0        0        0      833 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/analysis/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:39.847872 pm4pyminimal-2.7.9.3/pm4py/algo/analysis/extended_marking_equation/
--rw-rw-rw-   0        0        0      802 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/analysis/extended_marking_equation/__init__.py
--rw-rw-rw-   0        0        0     3588 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/analysis/extended_marking_equation/algorithm.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:39.853531 pm4pyminimal-2.7.9.3/pm4py/algo/analysis/extended_marking_equation/variants/
--rw-rw-rw-   0        0        0      810 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/analysis/extended_marking_equation/variants/__init__.py
--rw-rw-rw-   0        0        0    21448 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/analysis/extended_marking_equation/variants/classic.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:39.863515 pm4pyminimal-2.7.9.3/pm4py/algo/analysis/marking_equation/
--rw-rw-rw-   0        0        0      794 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/analysis/marking_equation/__init__.py
--rw-rw-rw-   0        0        0     2689 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/analysis/marking_equation/algorithm.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:39.869136 pm4pyminimal-2.7.9.3/pm4py/algo/analysis/marking_equation/variants/
--rw-rw-rw-   0        0        0      801 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/analysis/marking_equation/variants/__init__.py
--rw-rw-rw-   0        0        0    11636 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/analysis/marking_equation/variants/classic.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:39.877034 pm4pyminimal-2.7.9.3/pm4py/algo/analysis/woflan/
--rw-rw-rw-   0        0        0      836 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/analysis/woflan/__init__.py
--rw-rw-rw-   0        0        0    32308 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/analysis/woflan/algorithm.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:39.883325 pm4pyminimal-2.7.9.3/pm4py/algo/analysis/woflan/graphs/
--rw-rw-rw-   0        0        0      868 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/analysis/woflan/graphs/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:39.889660 pm4pyminimal-2.7.9.3/pm4py/algo/analysis/woflan/graphs/minimal_coverability_graph/
--rw-rw-rw-   0        0        0      835 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/analysis/woflan/graphs/minimal_coverability_graph/__init__.py
--rw-rw-rw-   0        0        0     7988 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/analysis/woflan/graphs/minimal_coverability_graph/minimal_coverability_graph.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:39.896641 pm4pyminimal-2.7.9.3/pm4py/algo/analysis/woflan/graphs/reachability_graph/
--rw-rw-rw-   0        0        0      819 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/analysis/woflan/graphs/reachability_graph/__init__.py
--rw-rw-rw-   0        0        0     2451 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/analysis/woflan/graphs/reachability_graph/reachability_graph.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:39.903791 pm4pyminimal-2.7.9.3/pm4py/algo/analysis/woflan/graphs/restricted_coverability_graph/
--rw-rw-rw-   0        0        0      841 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/analysis/woflan/graphs/restricted_coverability_graph/__init__.py
--rw-rw-rw-   0        0        0     4061 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/analysis/woflan/graphs/restricted_coverability_graph/restricted_coverability_graph.py
--rw-rw-rw-   0        0        0     5745 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/analysis/woflan/graphs/utility.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:39.914871 pm4pyminimal-2.7.9.3/pm4py/algo/analysis/woflan/not_well_handled_pairs/
--rw-rw-rw-   0        0        0      820 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/analysis/woflan/not_well_handled_pairs/__init__.py
--rw-rw-rw-   0        0        0     2632 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/analysis/woflan/not_well_handled_pairs/not_well_handled_pairs.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:39.931869 pm4pyminimal-2.7.9.3/pm4py/algo/analysis/woflan/place_invariants/
--rw-rw-rw-   0        0        0      849 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/analysis/woflan/place_invariants/__init__.py
--rw-rw-rw-   0        0        0     4300 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/analysis/woflan/place_invariants/place_invariants.py
--rw-rw-rw-   0        0        0     3668 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/analysis/woflan/place_invariants/s_component.py
--rw-rw-rw-   0        0        0     1098 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/analysis/woflan/place_invariants/uniform_invariant.py
--rw-rw-rw-   0        0        0     8333 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/analysis/woflan/place_invariants/utility.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:39.936860 pm4pyminimal-2.7.9.3/pm4py/algo/analysis/workflow_net/
--rw-rw-rw-   0        0        0      800 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/analysis/workflow_net/__init__.py
--rw-rw-rw-   0        0        0     1542 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/analysis/workflow_net/algorithm.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:39.943051 pm4pyminimal-2.7.9.3/pm4py/algo/analysis/workflow_net/variants/
--rw-rw-rw-   0        0        0      799 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/analysis/workflow_net/variants/__init__.py
--rw-rw-rw-   0        0        0     3243 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/analysis/workflow_net/variants/petri_net.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:39.946044 pm4pyminimal-2.7.9.3/pm4py/algo/anonymization/
--rw-rw-rw-   0        0        0      979 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/anonymization/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:39.950170 pm4pyminimal-2.7.9.3/pm4py/algo/anonymization/pripel/
--rw-rw-rw-   0        0        0      807 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/anonymization/pripel/__init__.py
--rw-rw-rw-   0        0        0     3170 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/anonymization/pripel/algorithm.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:39.962402 pm4pyminimal-2.7.9.3/pm4py/algo/anonymization/pripel/util/
--rw-rw-rw-   0        0        0    13889 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/anonymization/pripel/util/AttributeAnonymizer.py
--rw-rw-rw-   0        0        0    14468 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/anonymization/pripel/util/TraceMatcher.py
--rw-rw-rw-   0        0        0      837 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/anonymization/pripel/util/__init__.py
--rw-rw-rw-   0        0        0     1754 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/anonymization/pripel/util/trace_levenshtein.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:39.967389 pm4pyminimal-2.7.9.3/pm4py/algo/anonymization/pripel/variants/
--rw-rw-rw-   0        0        0      797 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/anonymization/pripel/variants/__init__.py
--rw-rw-rw-   0        0        0     5291 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/anonymization/pripel/variants/pripel.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:39.970524 pm4pyminimal-2.7.9.3/pm4py/algo/anonymization/trace_variant_query/
--rw-rw-rw-   0        0        0      820 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/anonymization/trace_variant_query/__init__.py
--rw-rw-rw-   0        0        0     3980 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/anonymization/trace_variant_query/algorithm.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:39.978503 pm4pyminimal-2.7.9.3/pm4py/algo/anonymization/trace_variant_query/util/
--rw-rw-rw-   0        0        0      839 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/anonymization/trace_variant_query/util/__init__.py
--rw-rw-rw-   0        0        0     6862 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/anonymization/trace_variant_query/util/behavioralAppropriateness.py
--rw-rw-rw-   0        0        0     1323 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/anonymization/trace_variant_query/util/exp_mech.py
--rw-rw-rw-   0        0        0     1687 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/anonymization/trace_variant_query/util/util.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:39.984612 pm4pyminimal-2.7.9.3/pm4py/algo/anonymization/trace_variant_query/variants/
--rw-rw-rw-   0        0        0      817 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/anonymization/trace_variant_query/variants/__init__.py
--rw-rw-rw-   0        0        0     7691 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/anonymization/trace_variant_query/variants/laplace.py
--rw-rw-rw-   0        0        0    11329 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/anonymization/trace_variant_query/variants/sacofa.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:39.986606 pm4pyminimal-2.7.9.3/pm4py/algo/clustering/
--rw-rw-rw-   0        0        0      734 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/clustering/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:39.990846 pm4pyminimal-2.7.9.3/pm4py/algo/clustering/profiles/
--rw-rw-rw-   0        0        0      798 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/clustering/profiles/__init__.py
--rw-rw-rw-   0        0        0     2118 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/clustering/profiles/algorithm.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:39.995832 pm4pyminimal-2.7.9.3/pm4py/algo/clustering/profiles/variants/
--rw-rw-rw-   0        0        0      804 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/clustering/profiles/variants/__init__.py
--rw-rw-rw-   0        0        0     3544 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/clustering/profiles/variants/sklearn_profiles.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:39.998930 pm4pyminimal-2.7.9.3/pm4py/algo/clustering/trace_attribute_driven/
--rw-rw-rw-   0        0        0     1060 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/clustering/trace_attribute_driven/__init__.py
--rw-rw-rw-   0        0        0     4705 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/clustering/trace_attribute_driven/algorithm.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:40.002920 pm4pyminimal-2.7.9.3/pm4py/algo/clustering/trace_attribute_driven/dfg/
--rw-rw-rw-   0        0        0      805 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/clustering/trace_attribute_driven/dfg/__init__.py
--rw-rw-rw-   0        0        0     3989 2024-01-02 13:29:21.000000 pm4pyminimal-2.7.9.3/pm4py/algo/clustering/trace_attribute_driven/dfg/dfg_dist.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:40.006909 pm4pyminimal-2.7.9.3/pm4py/algo/clustering/trace_attribute_driven/leven_dist/
--rw-rw-rw-   0        0        0      819 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/clustering/trace_attribute_driven/leven_dist/__init__.py
--rw-rw-rw-   0        0        0     5473 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/clustering/trace_attribute_driven/leven_dist/leven_dist_calc.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:40.011023 pm4pyminimal-2.7.9.3/pm4py/algo/clustering/trace_attribute_driven/linkage_method/
--rw-rw-rw-   0        0        0      819 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/clustering/trace_attribute_driven/linkage_method/__init__.py
--rw-rw-rw-   0        0        0    13583 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/clustering/trace_attribute_driven/linkage_method/linkage_avg.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:40.015012 pm4pyminimal-2.7.9.3/pm4py/algo/clustering/trace_attribute_driven/merge_log/
--rw-rw-rw-   0        0        0      812 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/clustering/trace_attribute_driven/merge_log/__init__.py
--rw-rw-rw-   0        0        0     4290 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/clustering/trace_attribute_driven/merge_log/merge_log.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:40.021104 pm4pyminimal-2.7.9.3/pm4py/algo/clustering/trace_attribute_driven/util/
--rw-rw-rw-   0        0        0      824 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/clustering/trace_attribute_driven/util/__init__.py
--rw-rw-rw-   0        0        0     3396 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/clustering/trace_attribute_driven/util/evaluation.py
--rw-rw-rw-   0        0        0    15776 2024-01-02 13:29:21.000000 pm4pyminimal-2.7.9.3/pm4py/algo/clustering/trace_attribute_driven/util/filter_subsets.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:40.033510 pm4pyminimal-2.7.9.3/pm4py/algo/clustering/trace_attribute_driven/variants/
--rw-rw-rw-   0        0        0      855 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/clustering/trace_attribute_driven/variants/__init__.py
--rw-rw-rw-   0        0        0    18463 2024-01-02 13:29:21.000000 pm4pyminimal-2.7.9.3/pm4py/algo/clustering/trace_attribute_driven/variants/act_dist_calc.py
--rw-rw-rw-   0        0        0     6806 2024-01-02 13:29:21.000000 pm4pyminimal-2.7.9.3/pm4py/algo/clustering/trace_attribute_driven/variants/logslice_dist.py
--rw-rw-rw-   0        0        0     6329 2024-01-02 13:29:21.000000 pm4pyminimal-2.7.9.3/pm4py/algo/clustering/trace_attribute_driven/variants/sim_calc.py
--rw-rw-rw-   0        0        0    15790 2024-01-02 13:29:21.000000 pm4pyminimal-2.7.9.3/pm4py/algo/clustering/trace_attribute_driven/variants/suc_dist_calc.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:40.035512 pm4pyminimal-2.7.9.3/pm4py/algo/comparison/
--rw-rw-rw-   0        0        0      851 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/comparison/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:40.039901 pm4pyminimal-2.7.9.3/pm4py/algo/comparison/petrinet/
--rw-rw-rw-   0        0        0      803 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/comparison/petrinet/__init__.py
--rw-rw-rw-   0        0        0     6719 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/comparison/petrinet/element_usage_comparison.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:40.042893 pm4pyminimal-2.7.9.3/pm4py/algo/conformance/
--rw-rw-rw-   0        0        0      946 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/conformance/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:40.045884 pm4pyminimal-2.7.9.3/pm4py/algo/conformance/alignments/
--rw-rw-rw-   0        0        0      822 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/conformance/alignments/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:40.049002 pm4pyminimal-2.7.9.3/pm4py/algo/conformance/alignments/decomposed/
--rw-rw-rw-   0        0        0      812 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/conformance/alignments/decomposed/__init__.py
--rw-rw-rw-   0        0        0     2018 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/conformance/alignments/decomposed/algorithm.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:40.053988 pm4pyminimal-2.7.9.3/pm4py/algo/conformance/alignments/decomposed/variants/
--rw-rw-rw-   0        0        0      818 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/conformance/alignments/decomposed/variants/__init__.py
--rw-rw-rw-   0        0        0    19051 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/conformance/alignments/decomposed/variants/recompos_maximal.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:40.057978 pm4pyminimal-2.7.9.3/pm4py/algo/conformance/alignments/dfg/
--rw-rw-rw-   0        0        0      805 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/conformance/alignments/dfg/__init__.py
--rw-rw-rw-   0        0        0     1956 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/conformance/alignments/dfg/algorithm.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:40.062075 pm4pyminimal-2.7.9.3/pm4py/algo/conformance/alignments/dfg/variants/
--rw-rw-rw-   0        0        0      802 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/conformance/alignments/dfg/variants/__init__.py
--rw-rw-rw-   0        0        0    24120 2024-01-15 12:00:43.000000 pm4pyminimal-2.7.9.3/pm4py/algo/conformance/alignments/dfg/variants/classic.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:40.066066 pm4pyminimal-2.7.9.3/pm4py/algo/conformance/alignments/edit_distance/
--rw-rw-rw-   0        0        0      815 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/conformance/alignments/edit_distance/__init__.py
--rw-rw-rw-   0        0        0     1876 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/conformance/alignments/edit_distance/algorithm.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:40.070163 pm4pyminimal-2.7.9.3/pm4py/algo/conformance/alignments/edit_distance/variants/
--rw-rw-rw-   0        0        0      818 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/conformance/alignments/edit_distance/variants/__init__.py
--rw-rw-rw-   0        0        0    11234 2024-01-02 13:29:21.000000 pm4pyminimal-2.7.9.3/pm4py/algo/conformance/alignments/edit_distance/variants/edit_distance.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:40.074152 pm4pyminimal-2.7.9.3/pm4py/algo/conformance/alignments/petri_net/
--rw-rw-rw-   0        0        0      818 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/conformance/alignments/petri_net/__init__.py
--rw-rw-rw-   0        0        0    16964 2024-01-15 12:00:43.000000 pm4pyminimal-2.7.9.3/pm4py/algo/conformance/alignments/petri_net/algorithm.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:40.078142 pm4pyminimal-2.7.9.3/pm4py/algo/conformance/alignments/petri_net/utils/
--rw-rw-rw-   0        0        0      812 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/conformance/alignments/petri_net/utils/__init__.py
--rw-rw-rw-   0        0        0     2896 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/conformance/alignments/petri_net/utils/log_enrichment.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:40.095297 pm4pyminimal-2.7.9.3/pm4py/algo/conformance/alignments/petri_net/variants/
--rw-rw-rw-   0        0        0      925 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/conformance/alignments/petri_net/variants/__init__.py
--rw-rw-rw-   0        0        0    27553 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/conformance/alignments/petri_net/variants/dijkstra_less_memory.py
--rw-rw-rw-   0        0        0    17167 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/conformance/alignments/petri_net/variants/dijkstra_no_heuristics.py
--rw-rw-rw-   0        0        0    23651 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/conformance/alignments/petri_net/variants/discounted_a_star.py
--rw-rw-rw-   0        0        0    23429 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/conformance/alignments/petri_net/variants/generator_dijkstra_less_memory.py
--rw-rw-rw-   0        0        0    17357 2024-01-02 13:29:21.000000 pm4pyminimal-2.7.9.3/pm4py/algo/conformance/alignments/petri_net/variants/generator_dijkstra_no_heuristics.py
--rw-rw-rw-   0        0        0    23978 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/conformance/alignments/petri_net/variants/state_equation_a_star.py
--rw-rw-rw-   0        0        0    27872 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/conformance/alignments/petri_net/variants/tweaked_state_equation_a_star.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:40.099444 pm4pyminimal-2.7.9.3/pm4py/algo/conformance/alignments/process_tree/
--rw-rw-rw-   0        0        0      820 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/conformance/alignments/process_tree/__init__.py
--rw-rw-rw-   0        0        0     2203 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/conformance/alignments/process_tree/algorithm.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:40.105428 pm4pyminimal-2.7.9.3/pm4py/algo/conformance/alignments/process_tree/util/
--rw-rw-rw-   0        0        0      870 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/conformance/alignments/process_tree/util/__init__.py
--rw-rw-rw-   0        0        0     3355 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/conformance/alignments/process_tree/util/search_graph_pt_frequency_annotation.py
--rw-rw-rw-   0        0        0    15712 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/conformance/alignments/process_tree/util/search_graph_pt_replay_semantics.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:40.108419 pm4pyminimal-2.7.9.3/pm4py/algo/conformance/alignments/process_tree/variants/
--rw-rw-rw-   0        0        0      833 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/conformance/alignments/process_tree/variants/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:40.119900 pm4pyminimal-2.7.9.3/pm4py/algo/conformance/alignments/process_tree/variants/approximated/
--rw-rw-rw-   0        0        0      871 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/conformance/alignments/process_tree/variants/approximated/__init__.py
--rw-rw-rw-   0        0        0     5361 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/conformance/alignments/process_tree/variants/approximated/calculate_a_sa_ea_sets.py
--rw-rw-rw-   0        0        0    49808 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/conformance/alignments/process_tree/variants/approximated/matrix_lp.py
--rw-rw-rw-   0        0        0    36425 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/conformance/alignments/process_tree/variants/approximated/original.py
--rw-rw-rw-   0        0        0     6660 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/conformance/alignments/process_tree/variants/approximated/utilities.py
--rw-rw-rw-   0        0        0    17939 2024-01-15 12:00:43.000000 pm4pyminimal-2.7.9.3/pm4py/algo/conformance/alignments/process_tree/variants/search_graph_pt.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:40.123890 pm4pyminimal-2.7.9.3/pm4py/algo/conformance/antialignments/
--rw-rw-rw-   0        0        0      805 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/conformance/antialignments/__init__.py
--rw-rw-rw-   0        0        0     3166 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/conformance/antialignments/algorithm.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:40.127880 pm4pyminimal-2.7.9.3/pm4py/algo/conformance/antialignments/variants/
--rw-rw-rw-   0        0        0      812 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/conformance/antialignments/variants/__init__.py
--rw-rw-rw-   0        0        0     7582 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/conformance/antialignments/variants/discounted_a_star.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:40.132991 pm4pyminimal-2.7.9.3/pm4py/algo/conformance/declare/
--rw-rw-rw-   0        0        0      800 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/conformance/declare/__init__.py
--rw-rw-rw-   0        0        0     2733 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/conformance/declare/algorithm.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:40.136983 pm4pyminimal-2.7.9.3/pm4py/algo/conformance/declare/variants/
--rw-rw-rw-   0        0        0      797 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/conformance/declare/variants/__init__.py
--rw-rw-rw-   0        0        0    18351 2024-01-02 13:29:21.000000 pm4pyminimal-2.7.9.3/pm4py/algo/conformance/declare/variants/classic.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:40.141243 pm4pyminimal-2.7.9.3/pm4py/algo/conformance/footprints/
--rw-rw-rw-   0        0        0      807 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/conformance/footprints/__init__.py
--rw-rw-rw-   0        0        0     2061 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/conformance/footprints/algorithm.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:40.147223 pm4pyminimal-2.7.9.3/pm4py/algo/conformance/footprints/util/
--rw-rw-rw-   0        0        0      817 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/conformance/footprints/util/__init__.py
--rw-rw-rw-   0        0        0     6154 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/conformance/footprints/util/evaluation.py
--rw-rw-rw-   0        0        0     3573 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/conformance/footprints/util/tree_visualization.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:40.155004 pm4pyminimal-2.7.9.3/pm4py/algo/conformance/footprints/variants/
--rw-rw-rw-   0        0        0      832 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/conformance/footprints/variants/__init__.py
--rw-rw-rw-   0        0        0     3708 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/conformance/footprints/variants/log_extensive.py
--rw-rw-rw-   0        0        0     5119 2024-01-02 13:29:21.000000 pm4pyminimal-2.7.9.3/pm4py/algo/conformance/footprints/variants/log_model.py
--rw-rw-rw-   0        0        0     7141 2024-01-02 13:29:21.000000 pm4pyminimal-2.7.9.3/pm4py/algo/conformance/footprints/variants/trace_extensive.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:40.157999 pm4pyminimal-2.7.9.3/pm4py/algo/conformance/log_skeleton/
--rw-rw-rw-   0        0        0      803 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/conformance/log_skeleton/__init__.py
--rw-rw-rw-   0        0        0     4040 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/conformance/log_skeleton/algorithm.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:40.163321 pm4pyminimal-2.7.9.3/pm4py/algo/conformance/log_skeleton/variants/
--rw-rw-rw-   0        0        0      800 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/conformance/log_skeleton/variants/__init__.py
--rw-rw-rw-   0        0        0    13160 2024-01-15 12:00:43.000000 pm4pyminimal-2.7.9.3/pm4py/algo/conformance/log_skeleton/variants/classic.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:40.167310 pm4pyminimal-2.7.9.3/pm4py/algo/conformance/multialignments/
--rw-rw-rw-   0        0        0      806 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/conformance/multialignments/__init__.py
--rw-rw-rw-   0        0        0     3143 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/conformance/multialignments/algorithm.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:40.170409 pm4pyminimal-2.7.9.3/pm4py/algo/conformance/multialignments/variants/
--rw-rw-rw-   0        0        0      813 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/conformance/multialignments/variants/__init__.py
--rw-rw-rw-   0        0        0     6557 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/conformance/multialignments/variants/discounted_a_star.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:40.174398 pm4pyminimal-2.7.9.3/pm4py/algo/conformance/temporal_profile/
--rw-rw-rw-   0        0        0      807 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/conformance/temporal_profile/__init__.py
--rw-rw-rw-   0        0        0     4738 2024-01-02 13:29:21.000000 pm4pyminimal-2.7.9.3/pm4py/algo/conformance/temporal_profile/algorithm.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:40.182649 pm4pyminimal-2.7.9.3/pm4py/algo/conformance/temporal_profile/variants/
--rw-rw-rw-   0        0        0      811 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/conformance/temporal_profile/variants/__init__.py
--rw-rw-rw-   0        0        0     5476 2024-01-02 13:29:21.000000 pm4pyminimal-2.7.9.3/pm4py/algo/conformance/temporal_profile/variants/dataframe.py
--rw-rw-rw-   0        0        0     5957 2024-01-02 13:29:21.000000 pm4pyminimal-2.7.9.3/pm4py/algo/conformance/temporal_profile/variants/log.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:40.186638 pm4pyminimal-2.7.9.3/pm4py/algo/conformance/tokenreplay/
--rw-rw-rw-   0        0        0      815 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/conformance/tokenreplay/__init__.py
--rw-rw-rw-   0        0        0     2965 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/conformance/tokenreplay/algorithm.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:40.194796 pm4pyminimal-2.7.9.3/pm4py/algo/conformance/tokenreplay/diagnostics/
--rw-rw-rw-   0        0        0      836 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/conformance/tokenreplay/diagnostics/__init__.py
--rw-rw-rw-   0        0        0     6720 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/conformance/tokenreplay/diagnostics/duration_diagnostics.py
--rw-rw-rw-   0        0        0    11104 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/conformance/tokenreplay/diagnostics/root_cause_analysis.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:40.200903 pm4pyminimal-2.7.9.3/pm4py/algo/conformance/tokenreplay/variants/
--rw-rw-rw-   0        0        0      804 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/conformance/tokenreplay/variants/__init__.py
--rw-rw-rw-   0        0        0    12130 2024-01-02 13:29:21.000000 pm4pyminimal-2.7.9.3/pm4py/algo/conformance/tokenreplay/variants/backwards.py
--rw-rw-rw-   0        0        0    59022 2024-01-15 12:00:43.000000 pm4pyminimal-2.7.9.3/pm4py/algo/conformance/tokenreplay/variants/token_replay.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:40.205890 pm4pyminimal-2.7.9.3/pm4py/algo/connectors/
--rw-rw-rw-   0        0        0      786 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/connectors/__init__.py
--rw-rw-rw-   0        0        0     2768 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/connectors/algorithm.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:40.212996 pm4pyminimal-2.7.9.3/pm4py/algo/connectors/util/
--rw-rw-rw-   0        0        0      781 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/connectors/util/__init__.py
--rw-rw-rw-   0        0        0     1628 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/connectors/util/mail.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:40.234598 pm4pyminimal-2.7.9.3/pm4py/algo/connectors/variants/
--rw-rw-rw-   0        0        0      736 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/connectors/variants/__init__.py
--rw-rw-rw-   0        0        0     2592 2024-01-02 13:29:21.000000 pm4pyminimal-2.7.9.3/pm4py/algo/connectors/variants/camunda_workflow.py
--rw-rw-rw-   0        0        0     3743 2024-01-02 13:29:21.000000 pm4pyminimal-2.7.9.3/pm4py/algo/connectors/variants/chrome_history.py
--rw-rw-rw-   0        0        0     3777 2024-01-02 13:29:21.000000 pm4pyminimal-2.7.9.3/pm4py/algo/connectors/variants/firefox_history.py
--rw-rw-rw-   0        0        0     5250 2024-01-02 13:29:21.000000 pm4pyminimal-2.7.9.3/pm4py/algo/connectors/variants/github_repo.py
--rw-rw-rw-   0        0        0     4432 2024-01-02 13:29:21.000000 pm4pyminimal-2.7.9.3/pm4py/algo/connectors/variants/outlook_calendar.py
--rw-rw-rw-   0        0        0     4568 2024-01-02 13:29:21.000000 pm4pyminimal-2.7.9.3/pm4py/algo/connectors/variants/outlook_mail_extractor.py
--rw-rw-rw-   0        0        0     3168 2024-01-02 13:29:21.000000 pm4pyminimal-2.7.9.3/pm4py/algo/connectors/variants/sap_accounting.py
--rw-rw-rw-   0        0        0     4012 2024-01-02 13:29:21.000000 pm4pyminimal-2.7.9.3/pm4py/algo/connectors/variants/sap_o2c.py
--rw-rw-rw-   0        0        0     4243 2024-01-02 13:29:21.000000 pm4pyminimal-2.7.9.3/pm4py/algo/connectors/variants/windows_events.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:40.239726 pm4pyminimal-2.7.9.3/pm4py/algo/decision_mining/
--rw-rw-rw-   0        0        0      964 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/decision_mining/__init__.py
--rw-rw-rw-   0        0        0    23509 2024-01-02 13:29:21.000000 pm4pyminimal-2.7.9.3/pm4py/algo/decision_mining/algorithm.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:40.241721 pm4pyminimal-2.7.9.3/pm4py/algo/discovery/
--rw-rw-rw-   0        0        0      945 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/discovery/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:40.246708 pm4pyminimal-2.7.9.3/pm4py/algo/discovery/alpha/
--rw-rw-rw-   0        0        0      818 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/discovery/alpha/__init__.py
--rw-rw-rw-   0        0        0     5066 2024-01-02 13:29:21.000000 pm4pyminimal-2.7.9.3/pm4py/algo/discovery/alpha/algorithm.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:40.250813 pm4pyminimal-2.7.9.3/pm4py/algo/discovery/alpha/data_structures/
--rw-rw-rw-   0        0        0      816 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/discovery/alpha/data_structures/__init__.py
--rw-rw-rw-   0        0        0     2420 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/discovery/alpha/data_structures/alpha_classic_abstraction.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:40.256797 pm4pyminimal-2.7.9.3/pm4py/algo/discovery/alpha/utils/
--rw-rw-rw-   0        0        0      790 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/discovery/alpha/utils/__init__.py
--rw-rw-rw-   0        0        0     1622 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/discovery/alpha/utils/endpoints.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:40.263907 pm4pyminimal-2.7.9.3/pm4py/algo/discovery/alpha/variants/
--rw-rw-rw-   0        0        0      797 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/discovery/alpha/variants/__init__.py
--rw-rw-rw-   0        0        0    10830 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/discovery/alpha/variants/classic.py
--rw-rw-rw-   0        0        0    22005 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/discovery/alpha/variants/plus.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:40.269029 pm4pyminimal-2.7.9.3/pm4py/algo/discovery/batches/
--rw-rw-rw-   0        0        0      803 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/discovery/batches/__init__.py
--rw-rw-rw-   0        0        0     3756 2024-01-02 13:29:21.000000 pm4pyminimal-2.7.9.3/pm4py/algo/discovery/batches/algorithm.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:40.273020 pm4pyminimal-2.7.9.3/pm4py/algo/discovery/batches/utils/
--rw-rw-rw-   0        0        0      792 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/discovery/batches/utils/__init__.py
--rw-rw-rw-   0        0        0     9636 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/discovery/batches/utils/detection.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:40.280108 pm4pyminimal-2.7.9.3/pm4py/algo/discovery/batches/variants/
--rw-rw-rw-   0        0        0      797 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/discovery/batches/variants/__init__.py
--rw-rw-rw-   0        0        0     5216 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/discovery/batches/variants/log.py
--rw-rw-rw-   0        0        0     6427 2024-01-15 12:00:43.000000 pm4pyminimal-2.7.9.3/pm4py/algo/discovery/batches/variants/pandas.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:40.285096 pm4pyminimal-2.7.9.3/pm4py/algo/discovery/causal/
--rw-rw-rw-   0        0        0      795 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/discovery/causal/__init__.py
--rw-rw-rw-   0        0        0     1646 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/discovery/causal/algorithm.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:40.291500 pm4pyminimal-2.7.9.3/pm4py/algo/discovery/causal/variants/
--rw-rw-rw-   0        0        0      801 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/discovery/causal/variants/__init__.py
--rw-rw-rw-   0        0        0     1787 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/discovery/causal/variants/alpha.py
--rw-rw-rw-   0        0        0     1589 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/discovery/causal/variants/heuristic.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:40.299583 pm4pyminimal-2.7.9.3/pm4py/algo/discovery/correlation_mining/
--rw-rw-rw-   0        0        0      813 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/discovery/correlation_mining/__init__.py
--rw-rw-rw-   0        0        0     2249 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/discovery/correlation_mining/algorithm.py
--rw-rw-rw-   0        0        0     7934 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/discovery/correlation_mining/util.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:40.307561 pm4pyminimal-2.7.9.3/pm4py/algo/discovery/correlation_mining/variants/
--rw-rw-rw-   0        0        0      832 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/discovery/correlation_mining/variants/__init__.py
--rw-rw-rw-   0        0        0     9663 2024-01-02 13:29:21.000000 pm4pyminimal-2.7.9.3/pm4py/algo/discovery/correlation_mining/variants/classic.py
--rw-rw-rw-   0        0        0     4405 2024-01-15 12:00:43.000000 pm4pyminimal-2.7.9.3/pm4py/algo/discovery/correlation_mining/variants/classic_split.py
--rw-rw-rw-   0        0        0    10288 2024-01-02 13:29:21.000000 pm4pyminimal-2.7.9.3/pm4py/algo/discovery/correlation_mining/variants/trace_based.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:40.315670 pm4pyminimal-2.7.9.3/pm4py/algo/discovery/declare/
--rw-rw-rw-   0        0        0      798 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/discovery/declare/__init__.py
--rw-rw-rw-   0        0        0     1725 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/discovery/declare/algorithm.py
--rw-rw-rw-   0        0        0     1290 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/discovery/declare/templates.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:40.319788 pm4pyminimal-2.7.9.3/pm4py/algo/discovery/declare/variants/
--rw-rw-rw-   0        0        0      795 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/discovery/declare/variants/__init__.py
--rw-rw-rw-   0        0        0    30263 2024-01-15 12:00:43.000000 pm4pyminimal-2.7.9.3/pm4py/algo/discovery/declare/variants/classic.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:40.328763 pm4pyminimal-2.7.9.3/pm4py/algo/discovery/dfg/
--rw-rw-rw-   0        0        0      822 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/discovery/dfg/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:40.330274 pm4pyminimal-2.7.9.3/pm4py/algo/discovery/dfg/adapters/
--rw-rw-rw-   0        0        0      788 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/discovery/dfg/adapters/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:40.336260 pm4pyminimal-2.7.9.3/pm4py/algo/discovery/dfg/adapters/pandas/
--rw-rw-rw-   0        0        0      816 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/discovery/dfg/adapters/pandas/__init__.py
--rw-rw-rw-   0        0        0    15047 2024-01-15 12:00:43.000000 pm4pyminimal-2.7.9.3/pm4py/algo/discovery/dfg/adapters/pandas/df_statistics.py
--rw-rw-rw-   0        0        0     2962 2024-01-02 13:29:21.000000 pm4pyminimal-2.7.9.3/pm4py/algo/discovery/dfg/adapters/pandas/freq_triples.py
--rw-rw-rw-   0        0        0     4898 2024-01-02 13:29:21.000000 pm4pyminimal-2.7.9.3/pm4py/algo/discovery/dfg/algorithm.py
--rw-rw-rw-   0        0        0     1260 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/discovery/dfg/replacement.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:40.340386 pm4pyminimal-2.7.9.3/pm4py/algo/discovery/dfg/utils/
--rw-rw-rw-   0        0        0      788 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/discovery/dfg/utils/__init__.py
--rw-rw-rw-   0        0        0      783 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/discovery/dfg/utils/dfg_utils.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:40.358551 pm4pyminimal-2.7.9.3/pm4py/algo/discovery/dfg/variants/
--rw-rw-rw-   0        0        0      968 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/discovery/dfg/variants/__init__.py
--rw-rw-rw-   0        0        0     4609 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/discovery/dfg/variants/case_attributes.py
--rw-rw-rw-   0        0        0     2852 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/discovery/dfg/variants/clean.py
--rw-rw-rw-   0        0        0     2795 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/discovery/dfg/variants/clean_polars.py
--rw-rw-rw-   0        0        0     3347 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/discovery/dfg/variants/clean_time.py
--rw-rw-rw-   0        0        0     2200 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/discovery/dfg/variants/freq_triples.py
--rw-rw-rw-   0        0        0     2574 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/discovery/dfg/variants/native.py
--rw-rw-rw-   0        0        0     5794 2024-01-02 13:29:21.000000 pm4pyminimal-2.7.9.3/pm4py/algo/discovery/dfg/variants/performance.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:40.365338 pm4pyminimal-2.7.9.3/pm4py/algo/discovery/footprints/
--rw-rw-rw-   0        0        0      812 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/discovery/footprints/__init__.py
--rw-rw-rw-   0        0        0     3131 2024-01-02 13:29:21.000000 pm4pyminimal-2.7.9.3/pm4py/algo/discovery/footprints/algorithm.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:40.367333 pm4pyminimal-2.7.9.3/pm4py/algo/discovery/footprints/dfg/
--rw-rw-rw-   0        0        0      792 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/discovery/footprints/dfg/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:40.371544 pm4pyminimal-2.7.9.3/pm4py/algo/discovery/footprints/dfg/variants/
--rw-rw-rw-   0        0        0      796 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/discovery/footprints/dfg/variants/__init__.py
--rw-rw-rw-   0        0        0     2258 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/discovery/footprints/dfg/variants/dfg.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:40.373538 pm4pyminimal-2.7.9.3/pm4py/algo/discovery/footprints/log/
--rw-rw-rw-   0        0        0      792 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/discovery/footprints/log/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:40.382781 pm4pyminimal-2.7.9.3/pm4py/algo/discovery/footprints/log/variants/
--rw-rw-rw-   0        0        0      843 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/discovery/footprints/log/variants/__init__.py
--rw-rw-rw-   0        0        0     4664 2024-01-02 13:29:21.000000 pm4pyminimal-2.7.9.3/pm4py/algo/discovery/footprints/log/variants/entire_dataframe.py
--rw-rw-rw-   0        0        0     3314 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/discovery/footprints/log/variants/entire_event_log.py
--rw-rw-rw-   0        0        0     3195 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/discovery/footprints/log/variants/trace_by_trace.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:40.385773 pm4pyminimal-2.7.9.3/pm4py/algo/discovery/footprints/petri/
--rw-rw-rw-   0        0        0      794 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/discovery/footprints/petri/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:40.388894 pm4pyminimal-2.7.9.3/pm4py/algo/discovery/footprints/petri/variants/
--rw-rw-rw-   0        0        0      806 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/discovery/footprints/petri/variants/__init__.py
--rw-rw-rw-   0        0        0     3629 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/discovery/footprints/petri/variants/reach_graph.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:40.392883 pm4pyminimal-2.7.9.3/pm4py/algo/discovery/footprints/tree/
--rw-rw-rw-   0        0        0      793 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/discovery/footprints/tree/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:40.397870 pm4pyminimal-2.7.9.3/pm4py/algo/discovery/footprints/tree/variants/
--rw-rw-rw-   0        0        0      802 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/discovery/footprints/tree/variants/__init__.py
--rw-rw-rw-   0        0        0    13403 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/discovery/footprints/tree/variants/bottomup.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:40.401981 pm4pyminimal-2.7.9.3/pm4py/algo/discovery/heuristics/
--rw-rw-rw-   0        0        0      799 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/discovery/heuristics/__init__.py
--rw-rw-rw-   0        0        0     7484 2024-01-02 13:29:21.000000 pm4pyminimal-2.7.9.3/pm4py/algo/discovery/heuristics/algorithm.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:40.410429 pm4pyminimal-2.7.9.3/pm4py/algo/discovery/heuristics/variants/
--rw-rw-rw-   0        0        0      806 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/discovery/heuristics/variants/__init__.py
--rw-rw-rw-   0        0        0    26145 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/discovery/heuristics/variants/classic.py
--rw-rw-rw-   0        0        0    24355 2024-01-02 13:29:21.000000 pm4pyminimal-2.7.9.3/pm4py/algo/discovery/heuristics/variants/plusplus.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:40.415415 pm4pyminimal-2.7.9.3/pm4py/algo/discovery/ilp/
--rw-rw-rw-   0        0        0      792 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/discovery/ilp/__init__.py
--rw-rw-rw-   0        0        0     1782 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/discovery/ilp/algorithm.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:40.420132 pm4pyminimal-2.7.9.3/pm4py/algo/discovery/ilp/variants/
--rw-rw-rw-   0        0        0      789 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/discovery/ilp/variants/__init__.py
--rw-rw-rw-   0        0        0    12873 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/discovery/ilp/variants/classic.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:40.424122 pm4pyminimal-2.7.9.3/pm4py/algo/discovery/inductive/
--rw-rw-rw-   0        0        0      800 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/discovery/inductive/__init__.py
--rw-rw-rw-   0        0        0     3602 2024-01-02 13:29:21.000000 pm4pyminimal-2.7.9.3/pm4py/algo/discovery/inductive/algorithm.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:40.436587 pm4pyminimal-2.7.9.3/pm4py/algo/discovery/inductive/base_case/
--rw-rw-rw-   0        0        0      829 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/discovery/inductive/base_case/__init__.py
--rw-rw-rw-   0        0        0     1533 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/discovery/inductive/base_case/abc.py
--rw-rw-rw-   0        0        0     1768 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/discovery/inductive/base_case/empty_log.py
--rw-rw-rw-   0        0        0     2268 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/discovery/inductive/base_case/factory.py
--rw-rw-rw-   0        0        0     2060 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/discovery/inductive/base_case/single_activity.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:40.454913 pm4pyminimal-2.7.9.3/pm4py/algo/discovery/inductive/cuts/
--rw-rw-rw-   0        0        0      816 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/discovery/inductive/cuts/__init__.py
--rw-rw-rw-   0        0        0     2100 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/discovery/inductive/cuts/abc.py
--rw-rw-rw-   0        0        0     4570 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/discovery/inductive/cuts/concurrency.py
--rw-rw-rw-   0        0        0     3143 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/discovery/inductive/cuts/factory.py
--rw-rw-rw-   0        0        0    10916 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/discovery/inductive/cuts/loop.py
--rw-rw-rw-   0        0        0    11571 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/discovery/inductive/cuts/sequence.py
--rw-rw-rw-   0        0        0     1519 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/discovery/inductive/cuts/utils.py
--rw-rw-rw-   0        0        0     4316 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/discovery/inductive/cuts/xor.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:40.462010 pm4pyminimal-2.7.9.3/pm4py/algo/discovery/inductive/dtypes/
--rw-rw-rw-   0        0        0      797 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/discovery/inductive/dtypes/__init__.py
--rw-rw-rw-   0        0        0     1050 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/discovery/inductive/dtypes/im_dfg.py
--rw-rw-rw-   0        0        0     2568 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/discovery/inductive/dtypes/im_ds.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:40.484524 pm4pyminimal-2.7.9.3/pm4py/algo/discovery/inductive/fall_through/
--rw-rw-rw-   0        0        0      897 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/discovery/inductive/fall_through/__init__.py
--rw-rw-rw-   0        0        0     1385 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/discovery/inductive/fall_through/abc.py
--rw-rw-rw-   0        0        0     4792 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/discovery/inductive/fall_through/activity_concurrent.py
--rw-rw-rw-   0        0        0     1643 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/discovery/inductive/fall_through/activity_once_per_trace.py
--rw-rw-rw-   0        0        0     2709 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/discovery/inductive/fall_through/empty_traces.py
--rw-rw-rw-   0        0        0     3254 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/discovery/inductive/fall_through/factory.py
--rw-rw-rw-   0        0        0     3059 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/discovery/inductive/fall_through/flower.py
--rw-rw-rw-   0        0        0     2441 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/discovery/inductive/fall_through/strict_tau_loop.py
--rw-rw-rw-   0        0        0     1520 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/discovery/inductive/fall_through/tau_loop.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:40.498901 pm4pyminimal-2.7.9.3/pm4py/algo/discovery/inductive/variants/
--rw-rw-rw-   0        0        0      807 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/discovery/inductive/variants/__init__.py
--rw-rw-rw-   0        0        0     4160 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/discovery/inductive/variants/abc.py
--rw-rw-rw-   0        0        0     1740 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/discovery/inductive/variants/im.py
--rw-rw-rw-   0        0        0     1098 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/discovery/inductive/variants/imd.py
--rw-rw-rw-   0        0        0     4381 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/discovery/inductive/variants/imf.py
--rw-rw-rw-   0        0        0      881 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/discovery/inductive/variants/instances.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:40.505883 pm4pyminimal-2.7.9.3/pm4py/algo/discovery/log_skeleton/
--rw-rw-rw-   0        0        0      815 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/discovery/log_skeleton/__init__.py
--rw-rw-rw-   0        0        0     2450 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/discovery/log_skeleton/algorithm.py
--rw-rw-rw-   0        0        0     3194 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/discovery/log_skeleton/trace_skel.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:40.511161 pm4pyminimal-2.7.9.3/pm4py/algo/discovery/log_skeleton/variants/
--rw-rw-rw-   0        0        0      798 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/discovery/log_skeleton/variants/__init__.py
--rw-rw-rw-   0        0        0    11111 2024-01-15 12:00:43.000000 pm4pyminimal-2.7.9.3/pm4py/algo/discovery/log_skeleton/variants/classic.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:40.518142 pm4pyminimal-2.7.9.3/pm4py/algo/discovery/minimum_self_distance/
--rw-rw-rw-   0        0        0      819 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/discovery/minimum_self_distance/__init__.py
--rw-rw-rw-   0        0        0     1567 2024-01-02 13:29:21.000000 pm4pyminimal-2.7.9.3/pm4py/algo/discovery/minimum_self_distance/algorithm.py
--rw-rw-rw-   0        0        0     3132 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/discovery/minimum_self_distance/utils.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:40.524247 pm4pyminimal-2.7.9.3/pm4py/algo/discovery/minimum_self_distance/variants/
--rw-rw-rw-   0        0        0      811 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/discovery/minimum_self_distance/variants/__init__.py
--rw-rw-rw-   0        0        0     2878 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/discovery/minimum_self_distance/variants/log.py
--rw-rw-rw-   0        0        0     2904 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/discovery/minimum_self_distance/variants/pandas.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:40.526240 pm4pyminimal-2.7.9.3/pm4py/algo/discovery/ocel/
--rw-rw-rw-   0        0        0      802 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/discovery/ocel/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:40.532597 pm4pyminimal-2.7.9.3/pm4py/algo/discovery/ocel/interleavings/
--rw-rw-rw-   0        0        0      814 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/discovery/ocel/interleavings/__init__.py
--rw-rw-rw-   0        0        0     2007 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/discovery/ocel/interleavings/algorithm.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:40.537584 pm4pyminimal-2.7.9.3/pm4py/algo/discovery/ocel/interleavings/utils/
--rw-rw-rw-   0        0        0      819 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/discovery/ocel/interleavings/utils/__init__.py
--rw-rw-rw-   0        0        0     4451 2024-01-02 13:29:21.000000 pm4pyminimal-2.7.9.3/pm4py/algo/discovery/ocel/interleavings/utils/merge_dataframe_rel_cases.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:40.541689 pm4pyminimal-2.7.9.3/pm4py/algo/discovery/ocel/interleavings/variants/
--rw-rw-rw-   0        0        0      820 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/discovery/ocel/interleavings/variants/__init__.py
--rw-rw-rw-   0        0        0     6643 2024-01-15 12:00:43.000000 pm4pyminimal-2.7.9.3/pm4py/algo/discovery/ocel/interleavings/variants/timestamp_interleavings.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:40.546676 pm4pyminimal-2.7.9.3/pm4py/algo/discovery/ocel/link_analysis/
--rw-rw-rw-   0        0        0      796 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/discovery/ocel/link_analysis/__init__.py
--rw-rw-rw-   0        0        0     1841 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/discovery/ocel/link_analysis/algorithm.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:40.551258 pm4pyminimal-2.7.9.3/pm4py/algo/discovery/ocel/link_analysis/variants/
--rw-rw-rw-   0        0        0      804 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/discovery/ocel/link_analysis/variants/__init__.py
--rw-rw-rw-   0        0        0     6519 2024-01-02 13:29:21.000000 pm4pyminimal-2.7.9.3/pm4py/algo/discovery/ocel/link_analysis/variants/classic.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:40.556247 pm4pyminimal-2.7.9.3/pm4py/algo/discovery/ocel/ocdfg/
--rw-rw-rw-   0        0        0      799 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/discovery/ocel/ocdfg/__init__.py
--rw-rw-rw-   0        0        0     1775 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/discovery/ocel/ocdfg/algorithm.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:40.560374 pm4pyminimal-2.7.9.3/pm4py/algo/discovery/ocel/ocdfg/variants/
--rw-rw-rw-   0        0        0      796 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/discovery/ocel/ocdfg/variants/__init__.py
--rw-rw-rw-   0        0        0     8817 2024-01-02 13:29:21.000000 pm4pyminimal-2.7.9.3/pm4py/algo/discovery/ocel/ocdfg/variants/classic.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:40.566357 pm4pyminimal-2.7.9.3/pm4py/algo/discovery/ocel/ocpn/
--rw-rw-rw-   0        0        0      798 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/discovery/ocel/ocpn/__init__.py
--rw-rw-rw-   0        0        0     1785 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/discovery/ocel/ocpn/algorithm.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:40.572453 pm4pyminimal-2.7.9.3/pm4py/algo/discovery/ocel/ocpn/variants/
--rw-rw-rw-   0        0        0      797 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/discovery/ocel/ocpn/variants/__init__.py
--rw-rw-rw-   0        0        0    10290 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/discovery/ocel/ocpn/variants/classic.py
--rw-rw-rw-   0        0        0      812 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/discovery/ocel/ocpn/variants/wo_annotation.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:40.577441 pm4pyminimal-2.7.9.3/pm4py/algo/discovery/ocel/saw_nets/
--rw-rw-rw-   0        0        0      804 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/discovery/ocel/saw_nets/__init__.py
--rw-rw-rw-   0        0        0     1800 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/discovery/ocel/saw_nets/algorithm.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:40.582123 pm4pyminimal-2.7.9.3/pm4py/algo/discovery/ocel/saw_nets/variants/
--rw-rw-rw-   0        0        0      801 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/discovery/ocel/saw_nets/variants/__init__.py
--rw-rw-rw-   0        0        0     7569 2024-01-02 13:29:21.000000 pm4pyminimal-2.7.9.3/pm4py/algo/discovery/ocel/saw_nets/variants/classic.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:40.586111 pm4pyminimal-2.7.9.3/pm4py/algo/discovery/performance_spectrum/
--rw-rw-rw-   0        0        0      809 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/discovery/performance_spectrum/__init__.py
--rw-rw-rw-   0        0        0     3495 2024-01-02 13:29:21.000000 pm4pyminimal-2.7.9.3/pm4py/algo/discovery/performance_spectrum/algorithm.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:40.600363 pm4pyminimal-2.7.9.3/pm4py/algo/discovery/performance_spectrum/variants/
--rw-rw-rw-   0        0        0      855 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/discovery/performance_spectrum/variants/__init__.py
--rw-rw-rw-   0        0        0     4317 2024-01-02 13:29:21.000000 pm4pyminimal-2.7.9.3/pm4py/algo/discovery/performance_spectrum/variants/dataframe.py
--rw-rw-rw-   0        0        0     4970 2024-01-02 13:29:21.000000 pm4pyminimal-2.7.9.3/pm4py/algo/discovery/performance_spectrum/variants/dataframe_disconnected.py
--rw-rw-rw-   0        0        0     3382 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/discovery/performance_spectrum/variants/log.py
--rw-rw-rw-   0        0        0     4366 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/discovery/performance_spectrum/variants/log_disconnected.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:40.604353 pm4pyminimal-2.7.9.3/pm4py/algo/discovery/powl/
--rw-rw-rw-   0        0        0      779 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/discovery/powl/__init__.py
--rw-rw-rw-   0        0        0     3201 2024-01-02 13:29:21.000000 pm4pyminimal-2.7.9.3/pm4py/algo/discovery/powl/algorithm.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:40.606347 pm4pyminimal-2.7.9.3/pm4py/algo/discovery/powl/inductive/
--rw-rw-rw-   0        0        0      787 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/discovery/powl/inductive/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:40.618535 pm4pyminimal-2.7.9.3/pm4py/algo/discovery/powl/inductive/base_case/
--rw-rw-rw-   0        0        0      797 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/discovery/powl/inductive/base_case/__init__.py
--rw-rw-rw-   0        0        0     1506 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/discovery/powl/inductive/base_case/abc.py
--rw-rw-rw-   0        0        0     1457 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/discovery/powl/inductive/base_case/empty_log.py
--rw-rw-rw-   0        0        0     1867 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/discovery/powl/inductive/base_case/factory.py
--rw-rw-rw-   0        0        0     1547 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/discovery/powl/inductive/base_case/single_activity.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:40.633856 pm4pyminimal-2.7.9.3/pm4py/algo/discovery/powl/inductive/cuts/
--rw-rw-rw-   0        0        0      792 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/discovery/powl/inductive/cuts/__init__.py
--rw-rw-rw-   0        0        0     1361 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/discovery/powl/inductive/cuts/concurrency.py
--rw-rw-rw-   0        0        0     1974 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/discovery/powl/inductive/cuts/factory.py
--rw-rw-rw-   0        0        0     1353 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/discovery/powl/inductive/cuts/loop.py
--rw-rw-rw-   0        0        0     1975 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/discovery/powl/inductive/cuts/sequence.py
--rw-rw-rw-   0        0        0     1433 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/discovery/powl/inductive/cuts/xor.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:40.653355 pm4pyminimal-2.7.9.3/pm4py/algo/discovery/powl/inductive/fall_through/
--rw-rw-rw-   0        0        0      798 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/discovery/powl/inductive/fall_through/__init__.py
--rw-rw-rw-   0        0        0     1905 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/discovery/powl/inductive/fall_through/activity_concurrent.py
--rw-rw-rw-   0        0        0     1056 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/discovery/powl/inductive/fall_through/activity_once_per_trace.py
--rw-rw-rw-   0        0        0     1795 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/discovery/powl/inductive/fall_through/empty_traces.py
--rw-rw-rw-   0        0        0     2498 2024-01-02 13:29:21.000000 pm4pyminimal-2.7.9.3/pm4py/algo/discovery/powl/inductive/fall_through/factory.py
--rw-rw-rw-   0        0        0     1814 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/discovery/powl/inductive/fall_through/flower.py
--rw-rw-rw-   0        0        0     1651 2024-01-02 13:29:21.000000 pm4pyminimal-2.7.9.3/pm4py/algo/discovery/powl/inductive/fall_through/strict_tau_loop.py
--rw-rw-rw-   0        0        0     1630 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/discovery/powl/inductive/fall_through/tau_loop.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:40.658341 pm4pyminimal-2.7.9.3/pm4py/algo/discovery/powl/inductive/utils/
--rw-rw-rw-   0        0        0      734 2024-01-02 13:29:21.000000 pm4pyminimal-2.7.9.3/pm4py/algo/discovery/powl/inductive/utils/__init__.py
--rw-rw-rw-   0        0        0     2008 2024-01-02 13:29:21.000000 pm4pyminimal-2.7.9.3/pm4py/algo/discovery/powl/inductive/utils/filtering.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:40.675657 pm4pyminimal-2.7.9.3/pm4py/algo/discovery/powl/inductive/variants/
--rw-rw-rw-   0        0        0      798 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/discovery/powl/inductive/variants/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:40.682875 pm4pyminimal-2.7.9.3/pm4py/algo/discovery/powl/inductive/variants/brute_force/
--rw-rw-rw-   0        0        0      806 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/discovery/powl/inductive/variants/brute_force/__init__.py
--rw-rw-rw-   0        0        0     7020 2024-01-02 13:29:21.000000 pm4pyminimal-2.7.9.3/pm4py/algo/discovery/powl/inductive/variants/brute_force/bf_partial_order_cut.py
--rw-rw-rw-   0        0        0     2195 2024-01-02 13:29:21.000000 pm4pyminimal-2.7.9.3/pm4py/algo/discovery/powl/inductive/variants/brute_force/factory.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:40.690020 pm4pyminimal-2.7.9.3/pm4py/algo/discovery/powl/inductive/variants/dynamic_clustering/
--rw-rw-rw-   0        0        0      813 2024-01-02 13:29:21.000000 pm4pyminimal-2.7.9.3/pm4py/algo/discovery/powl/inductive/variants/dynamic_clustering/__init__.py
--rw-rw-rw-   0        0        0     7347 2024-01-02 13:29:21.000000 pm4pyminimal-2.7.9.3/pm4py/algo/discovery/powl/inductive/variants/dynamic_clustering/dynamic_clustering_partial_order_cut.py
--rw-rw-rw-   0        0        0     2043 2024-01-02 13:29:21.000000 pm4pyminimal-2.7.9.3/pm4py/algo/discovery/powl/inductive/variants/dynamic_clustering/factory.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:40.697999 pm4pyminimal-2.7.9.3/pm4py/algo/discovery/powl/inductive/variants/dynamic_clustering_frequency/
--rw-rw-rw-   0        0        0      823 2024-01-02 13:29:21.000000 pm4pyminimal-2.7.9.3/pm4py/algo/discovery/powl/inductive/variants/dynamic_clustering_frequency/__init__.py
--rw-rw-rw-   0        0        0     8397 2024-01-02 13:29:21.000000 pm4pyminimal-2.7.9.3/pm4py/algo/discovery/powl/inductive/variants/dynamic_clustering_frequency/dynamic_clustering_frequency_partial_order_cut.py
--rw-rw-rw-   0        0        0     2099 2024-01-02 13:29:21.000000 pm4pyminimal-2.7.9.3/pm4py/algo/discovery/powl/inductive/variants/dynamic_clustering_frequency/factory.py
--rw-rw-rw-   0        0        0     1482 2024-01-02 13:29:21.000000 pm4pyminimal-2.7.9.3/pm4py/algo/discovery/powl/inductive/variants/im_brute_force.py
--rw-rw-rw-   0        0        0     1643 2024-01-02 13:29:21.000000 pm4pyminimal-2.7.9.3/pm4py/algo/discovery/powl/inductive/variants/im_dynamic_clustering.py
--rw-rw-rw-   0        0        0     1687 2024-01-02 13:29:21.000000 pm4pyminimal-2.7.9.3/pm4py/algo/discovery/powl/inductive/variants/im_dynamic_clustering_frequencies.py
--rw-rw-rw-   0        0        0     1468 2024-01-02 13:29:21.000000 pm4pyminimal-2.7.9.3/pm4py/algo/discovery/powl/inductive/variants/im_maximal.py
--rw-rw-rw-   0        0        0     5456 2024-01-02 13:29:21.000000 pm4pyminimal-2.7.9.3/pm4py/algo/discovery/powl/inductive/variants/im_tree.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:40.706079 pm4pyminimal-2.7.9.3/pm4py/algo/discovery/powl/inductive/variants/maximal/
--rw-rw-rw-   0        0        0      800 2024-01-02 13:29:21.000000 pm4pyminimal-2.7.9.3/pm4py/algo/discovery/powl/inductive/variants/maximal/__init__.py
--rw-rw-rw-   0        0        0     2373 2024-01-02 13:29:21.000000 pm4pyminimal-2.7.9.3/pm4py/algo/discovery/powl/inductive/variants/maximal/factory.py
--rw-rw-rw-   0        0        0     7192 2024-01-02 13:29:21.000000 pm4pyminimal-2.7.9.3/pm4py/algo/discovery/powl/inductive/variants/maximal/maximal_partial_order_cut.py
--rw-rw-rw-   0        0        0      936 2024-01-02 13:29:21.000000 pm4pyminimal-2.7.9.3/pm4py/algo/discovery/powl/inductive/variants/powl_discovery_varaints.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:40.710291 pm4pyminimal-2.7.9.3/pm4py/algo/discovery/temporal_profile/
--rw-rw-rw-   0        0        0      805 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/discovery/temporal_profile/__init__.py
--rw-rw-rw-   0        0        0     2006 2024-01-02 13:29:21.000000 pm4pyminimal-2.7.9.3/pm4py/algo/discovery/temporal_profile/algorithm.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:40.719265 pm4pyminimal-2.7.9.3/pm4py/algo/discovery/temporal_profile/variants/
--rw-rw-rw-   0        0        0      809 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/discovery/temporal_profile/variants/__init__.py
--rw-rw-rw-   0        0        0     4044 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/discovery/temporal_profile/variants/dataframe.py
--rw-rw-rw-   0        0        0     5236 2024-01-02 13:29:21.000000 pm4pyminimal-2.7.9.3/pm4py/algo/discovery/temporal_profile/variants/log.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:40.725960 pm4pyminimal-2.7.9.3/pm4py/algo/discovery/transition_system/
--rw-rw-rw-   0        0        0      806 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/discovery/transition_system/__init__.py
--rw-rw-rw-   0        0        0     1984 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/discovery/transition_system/algorithm.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:40.730169 pm4pyminimal-2.7.9.3/pm4py/algo/discovery/transition_system/variants/
--rw-rw-rw-   0        0        0      806 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/discovery/transition_system/variants/__init__.py
--rw-rw-rw-   0        0        0     5956 2024-01-15 12:00:43.000000 pm4pyminimal-2.7.9.3/pm4py/algo/discovery/transition_system/variants/view_based.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:40.734158 pm4pyminimal-2.7.9.3/pm4py/algo/evaluation/
--rw-rw-rw-   0        0        0      836 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/evaluation/__init__.py
--rw-rw-rw-   0        0        0     4819 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/evaluation/algorithm.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:40.739145 pm4pyminimal-2.7.9.3/pm4py/algo/evaluation/earth_mover_distance/
--rw-rw-rw-   0        0        0      995 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/evaluation/earth_mover_distance/__init__.py
--rw-rw-rw-   0        0        0     1678 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/evaluation/earth_mover_distance/algorithm.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:40.742556 pm4pyminimal-2.7.9.3/pm4py/algo/evaluation/earth_mover_distance/variants/
--rw-rw-rw-   0        0        0      805 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/evaluation/earth_mover_distance/variants/__init__.py
--rw-rw-rw-   0        0        0     4864 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/evaluation/earth_mover_distance/variants/pyemd.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:40.750571 pm4pyminimal-2.7.9.3/pm4py/algo/evaluation/generalization/
--rw-rw-rw-   0        0        0      804 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/evaluation/generalization/__init__.py
--rw-rw-rw-   0        0        0     1703 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/evaluation/generalization/algorithm.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:40.753563 pm4pyminimal-2.7.9.3/pm4py/algo/evaluation/generalization/variants/
--rw-rw-rw-   0        0        0      805 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/evaluation/generalization/variants/__init__.py
--rw-rw-rw-   0        0        0     2285 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/evaluation/generalization/variants/token_based.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:40.764652 pm4pyminimal-2.7.9.3/pm4py/algo/evaluation/precision/
--rw-rw-rw-   0        0        0      811 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/evaluation/precision/__init__.py
--rw-rw-rw-   0        0        0     2994 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/evaluation/precision/algorithm.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:40.770233 pm4pyminimal-2.7.9.3/pm4py/algo/evaluation/precision/dfg/
--rw-rw-rw-   0        0        0      793 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/evaluation/precision/dfg/__init__.py
--rw-rw-rw-   0        0        0     3992 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/evaluation/precision/dfg/algorithm.py
--rw-rw-rw-   0        0        0     5525 2024-01-15 12:00:43.000000 pm4pyminimal-2.7.9.3/pm4py/algo/evaluation/precision/utils.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:40.782220 pm4pyminimal-2.7.9.3/pm4py/algo/evaluation/precision/variants/
--rw-rw-rw-   0        0        0      829 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/evaluation/precision/variants/__init__.py
--rw-rw-rw-   0        0        0    13806 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/evaluation/precision/variants/align_etconformance.py
--rw-rw-rw-   0        0        0     6199 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/evaluation/precision/variants/etconformance_token.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:40.789202 pm4pyminimal-2.7.9.3/pm4py/algo/evaluation/replay_fitness/
--rw-rw-rw-   0        0        0      804 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/evaluation/replay_fitness/__init__.py
--rw-rw-rw-   0        0        0     4486 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/evaluation/replay_fitness/algorithm.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:40.797183 pm4pyminimal-2.7.9.3/pm4py/algo/evaluation/replay_fitness/variants/
--rw-rw-rw-   0        0        0      823 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/evaluation/replay_fitness/variants/__init__.py
--rw-rw-rw-   0        0        0     6788 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/evaluation/replay_fitness/variants/alignment_based.py
--rw-rw-rw-   0        0        0     5159 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/evaluation/replay_fitness/variants/token_replay.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:40.803303 pm4pyminimal-2.7.9.3/pm4py/algo/evaluation/simplicity/
--rw-rw-rw-   0        0        0      802 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/evaluation/simplicity/__init__.py
--rw-rw-rw-   0        0        0     1585 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/evaluation/simplicity/algorithm.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:40.816629 pm4pyminimal-2.7.9.3/pm4py/algo/evaluation/simplicity/variants/
--rw-rw-rw-   0        0        0      841 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/evaluation/simplicity/variants/__init__.py
--rw-rw-rw-   0        0        0     2696 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/evaluation/simplicity/variants/arc_degree.py
--rw-rw-rw-   0        0        0     1602 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/evaluation/simplicity/variants/extended_cardoso.py
--rw-rw-rw-   0        0        0     2120 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/evaluation/simplicity/variants/extended_cyclomatic.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:40.819621 pm4pyminimal-2.7.9.3/pm4py/algo/filtering/
--rw-rw-rw-   0        0        0      734 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/filtering/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:40.825756 pm4pyminimal-2.7.9.3/pm4py/algo/filtering/common/
--rw-rw-rw-   0        0        0      852 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/filtering/common/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:40.832479 pm4pyminimal-2.7.9.3/pm4py/algo/filtering/common/attributes/
--rw-rw-rw-   0        0        0      734 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/filtering/common/attributes/__init__.py
--rw-rw-rw-   0        0        0      951 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/filtering/common/attributes/attributes_common.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:40.839461 pm4pyminimal-2.7.9.3/pm4py/algo/filtering/common/end_activities/
--rw-rw-rw-   0        0        0      812 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/filtering/common/end_activities/__init__.py
--rw-rw-rw-   0        0        0      851 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/filtering/common/end_activities/end_activities_common.py
--rw-rw-rw-   0        0        0      845 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/filtering/common/filtering_constants.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:40.839757 pm4pyminimal-2.7.9.3/pm4py/algo/filtering/common/start_activities/
--rw-rw-rw-   0        0        0      816 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/filtering/common/start_activities/__init__.py
--rw-rw-rw-   0        0        0      857 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/filtering/common/start_activities/start_activities_common.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:40.854303 pm4pyminimal-2.7.9.3/pm4py/algo/filtering/common/timestamp/
--rw-rw-rw-   0        0        0      734 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/filtering/common/timestamp/__init__.py
--rw-rw-rw-   0        0        0     1250 2024-01-02 13:29:21.000000 pm4pyminimal-2.7.9.3/pm4py/algo/filtering/common/timestamp/timestamp_common.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:40.863483 pm4pyminimal-2.7.9.3/pm4py/algo/filtering/common/traces/
--rw-rw-rw-   0        0        0      734 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/filtering/common/traces/__init__.py
--rw-rw-rw-   0        0        0     1246 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/filtering/common/traces/infix_to_regex.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:40.869465 pm4pyminimal-2.7.9.3/pm4py/algo/filtering/dfg/
--rw-rw-rw-   0        0        0      734 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/filtering/dfg/__init__.py
--rw-rw-rw-   0        0        0    25920 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/filtering/dfg/dfg_filtering.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:40.875137 pm4pyminimal-2.7.9.3/pm4py/algo/filtering/log/
--rw-rw-rw-   0        0        0      866 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/filtering/log/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:40.883836 pm4pyminimal-2.7.9.3/pm4py/algo/filtering/log/attr_value_repetition/
--rw-rw-rw-   0        0        0      994 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/filtering/log/attr_value_repetition/__init__.py
--rw-rw-rw-   0        0        0     2754 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/filtering/log/attr_value_repetition/filter.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:40.894812 pm4pyminimal-2.7.9.3/pm4py/algo/filtering/log/attributes/
--rw-rw-rw-   0        0        0      801 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/filtering/log/attributes/__init__.py
--rw-rw-rw-   0        0        0    18308 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/filtering/log/attributes/attributes_filter.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:40.902367 pm4pyminimal-2.7.9.3/pm4py/algo/filtering/log/between/
--rw-rw-rw-   0        0        0      795 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/filtering/log/between/__init__.py
--rw-rw-rw-   0        0        0     2944 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/filtering/log/between/between_filter.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:40.902367 pm4pyminimal-2.7.9.3/pm4py/algo/filtering/log/cases/
--rw-rw-rw-   0        0        0      790 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/filtering/log/cases/__init__.py
--rw-rw-rw-   0        0        0     4597 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/filtering/log/cases/case_filter.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:40.917988 pm4pyminimal-2.7.9.3/pm4py/algo/filtering/log/end_activities/
--rw-rw-rw-   0        0        0      809 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/filtering/log/end_activities/__init__.py
--rw-rw-rw-   0        0        0     3719 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/filtering/log/end_activities/end_activities_filter.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:40.938249 pm4pyminimal-2.7.9.3/pm4py/algo/filtering/log/ltl/
--rw-rw-rw-   0        0        0      788 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/filtering/log/ltl/__init__.py
--rw-rw-rw-   0        0        0    11094 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/filtering/log/ltl/ltl_checker.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:40.943235 pm4pyminimal-2.7.9.3/pm4py/algo/filtering/log/paths/
--rw-rw-rw-   0        0        0      791 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/filtering/log/paths/__init__.py
--rw-rw-rw-   0        0        0     9660 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/filtering/log/paths/paths_filter.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:40.950364 pm4pyminimal-2.7.9.3/pm4py/algo/filtering/log/prefixes/
--rw-rw-rw-   0        0        0      797 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/filtering/log/prefixes/__init__.py
--rw-rw-rw-   0        0        0     3218 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/filtering/log/prefixes/prefix_filter.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:40.956133 pm4pyminimal-2.7.9.3/pm4py/algo/filtering/log/rework/
--rw-rw-rw-   0        0        0      793 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/filtering/log/rework/__init__.py
--rw-rw-rw-   0        0        0     3412 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/filtering/log/rework/rework_filter.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:40.962245 pm4pyminimal-2.7.9.3/pm4py/algo/filtering/log/start_activities/
--rw-rw-rw-   0        0        0      813 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/filtering/log/start_activities/__init__.py
--rw-rw-rw-   0        0        0     3950 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/filtering/log/start_activities/start_activities_filter.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:40.967231 pm4pyminimal-2.7.9.3/pm4py/algo/filtering/log/suffixes/
--rw-rw-rw-   0        0        0      797 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/filtering/log/suffixes/__init__.py
--rw-rw-rw-   0        0        0     3223 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/filtering/log/suffixes/suffix_filter.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:40.972740 pm4pyminimal-2.7.9.3/pm4py/algo/filtering/log/timestamp/
--rw-rw-rw-   0        0        0      799 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/filtering/log/timestamp/__init__.py
--rw-rw-rw-   0        0        0    11509 2024-01-02 13:29:21.000000 pm4pyminimal-2.7.9.3/pm4py/algo/filtering/log/timestamp/timestamp_filter.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:40.979935 pm4pyminimal-2.7.9.3/pm4py/algo/filtering/log/traces/
--rw-rw-rw-   0        0        0      734 2024-01-02 13:29:21.000000 pm4pyminimal-2.7.9.3/pm4py/algo/filtering/log/traces/__init__.py
--rw-rw-rw-   0        0        0     3785 2024-01-02 13:29:21.000000 pm4pyminimal-2.7.9.3/pm4py/algo/filtering/log/traces/trace_filter.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:40.979935 pm4pyminimal-2.7.9.3/pm4py/algo/filtering/log/variants/
--rw-rw-rw-   0        0        0      797 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/filtering/log/variants/__init__.py
--rw-rw-rw-   0        0        0     9002 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/filtering/log/variants/variants_filter.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:41.006146 pm4pyminimal-2.7.9.3/pm4py/algo/filtering/ocel/
--rw-rw-rw-   0        0        0      865 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/filtering/ocel/__init__.py
--rw-rw-rw-   0        0        0     3392 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/filtering/ocel/activity_type_matching.py
--rw-rw-rw-   0        0        0     3843 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/filtering/ocel/event_attributes.py
--rw-rw-rw-   0        0        0     2319 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/filtering/ocel/object_attributes.py
--rw-rw-rw-   0        0        0     3436 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/filtering/ocel/objects_ot_count.py
--rw-rw-rw-   0        0        0     4195 2024-01-02 13:29:21.000000 pm4pyminimal-2.7.9.3/pm4py/algo/filtering/ocel/ot_endpoints.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:41.016986 pm4pyminimal-2.7.9.3/pm4py/algo/filtering/pandas/
--rw-rw-rw-   0        0        0      891 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/filtering/pandas/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:41.024700 pm4pyminimal-2.7.9.3/pm4py/algo/filtering/pandas/attr_value_repetition/
--rw-rw-rw-   0        0        0      997 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/filtering/pandas/attr_value_repetition/__init__.py
--rw-rw-rw-   0        0        0     2786 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/filtering/pandas/attr_value_repetition/filter.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:41.032901 pm4pyminimal-2.7.9.3/pm4py/algo/filtering/pandas/attributes/
--rw-rw-rw-   0        0        0      734 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/filtering/pandas/attributes/__init__.py
--rw-rw-rw-   0        0        0    13156 2024-01-15 12:00:43.000000 pm4pyminimal-2.7.9.3/pm4py/algo/filtering/pandas/attributes/attributes_filter.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:41.039593 pm4pyminimal-2.7.9.3/pm4py/algo/filtering/pandas/between/
--rw-rw-rw-   0        0        0      798 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/filtering/pandas/between/__init__.py
--rw-rw-rw-   0        0        0     3266 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/filtering/pandas/between/between_filter.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:41.046574 pm4pyminimal-2.7.9.3/pm4py/algo/filtering/pandas/cases/
--rw-rw-rw-   0        0        0      793 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/filtering/pandas/cases/__init__.py
--rw-rw-rw-   0        0        0     6322 2024-01-15 12:00:43.000000 pm4pyminimal-2.7.9.3/pm4py/algo/filtering/pandas/cases/case_filter.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:41.049856 pm4pyminimal-2.7.9.3/pm4py/algo/filtering/pandas/consecutive_act_case_grouping/
--rw-rw-rw-   0        0        0      842 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/filtering/pandas/consecutive_act_case_grouping/__init__.py
--rw-rw-rw-   0        0        0     3077 2024-01-02 13:29:21.000000 pm4pyminimal-2.7.9.3/pm4py/algo/filtering/pandas/consecutive_act_case_grouping/consecutive_act_case_grouping_filter.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:41.059542 pm4pyminimal-2.7.9.3/pm4py/algo/filtering/pandas/end_activities/
--rw-rw-rw-   0        0        0      812 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/filtering/pandas/end_activities/__init__.py
--rw-rw-rw-   0        0        0     6142 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/filtering/pandas/end_activities/end_activities_filter.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:41.066098 pm4pyminimal-2.7.9.3/pm4py/algo/filtering/pandas/ends_with/
--rw-rw-rw-   0        0        0      734 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/filtering/pandas/ends_with/__init__.py
--rw-rw-rw-   0        0        0     3508 2023-12-11 09:33:51.000000 pm4pyminimal-2.7.9.3/pm4py/algo/filtering/pandas/ends_with/ends_with_filter.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:41.071889 pm4pyminimal-2.7.9.3/pm4py/algo/filtering/pandas/ltl/
--rw-rw-rw-   0        0        0      791 2023-12-11 09:33:52.000000 pm4pyminimal-2.7.9.3/pm4py/algo/filtering/pandas/ltl/__init__.py
--rw-rw-rw-   0        0        0    11763 2024-01-15 12:00:43.000000 pm4pyminimal-2.7.9.3/pm4py/algo/filtering/pandas/ltl/ltl_checker.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:41.078918 pm4pyminimal-2.7.9.3/pm4py/algo/filtering/pandas/paths/
--rw-rw-rw-   0        0        0      794 2023-12-11 09:33:52.000000 pm4pyminimal-2.7.9.3/pm4py/algo/filtering/pandas/paths/__init__.py
--rw-rw-rw-   0        0        0     6919 2024-01-15 12:00:43.000000 pm4pyminimal-2.7.9.3/pm4py/algo/filtering/pandas/paths/paths_filter.py
--rw-rw-rw-   0        0        0      832 2023-12-11 09:33:52.000000 pm4pyminimal-2.7.9.3/pm4py/algo/filtering/pandas/pd_filtering_constants.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:41.084247 pm4pyminimal-2.7.9.3/pm4py/algo/filtering/pandas/prefixes/
--rw-rw-rw-   0        0        0      800 2023-12-11 09:33:52.000000 pm4pyminimal-2.7.9.3/pm4py/algo/filtering/pandas/prefixes/__init__.py
--rw-rw-rw-   0        0        0     3950 2023-12-11 09:33:52.000000 pm4pyminimal-2.7.9.3/pm4py/algo/filtering/pandas/prefixes/prefix_filter.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:41.089886 pm4pyminimal-2.7.9.3/pm4py/algo/filtering/pandas/rework/
--rw-rw-rw-   0        0        0      796 2023-12-11 09:33:52.000000 pm4pyminimal-2.7.9.3/pm4py/algo/filtering/pandas/rework/__init__.py
--rw-rw-rw-   0        0        0     3425 2024-01-02 13:29:21.000000 pm4pyminimal-2.7.9.3/pm4py/algo/filtering/pandas/rework/rework_filter.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:41.095870 pm4pyminimal-2.7.9.3/pm4py/algo/filtering/pandas/start_activities/
--rw-rw-rw-   0        0        0      816 2023-12-11 09:33:52.000000 pm4pyminimal-2.7.9.3/pm4py/algo/filtering/pandas/start_activities/__init__.py
--rw-rw-rw-   0        0        0     5585 2023-12-11 09:33:52.000000 pm4pyminimal-2.7.9.3/pm4py/algo/filtering/pandas/start_activities/start_activities_filter.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:41.102517 pm4pyminimal-2.7.9.3/pm4py/algo/filtering/pandas/starts_with/
--rw-rw-rw-   0        0        0      734 2023-12-11 09:33:52.000000 pm4pyminimal-2.7.9.3/pm4py/algo/filtering/pandas/starts_with/__init__.py
--rw-rw-rw-   0        0        0     3510 2023-12-11 09:33:52.000000 pm4pyminimal-2.7.9.3/pm4py/algo/filtering/pandas/starts_with/starts_with_filter.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:41.111493 pm4pyminimal-2.7.9.3/pm4py/algo/filtering/pandas/suffixes/
--rw-rw-rw-   0        0        0      736 2023-12-11 09:33:52.000000 pm4pyminimal-2.7.9.3/pm4py/algo/filtering/pandas/suffixes/__init__.py
--rw-rw-rw-   0        0        0     3950 2023-12-11 09:33:52.000000 pm4pyminimal-2.7.9.3/pm4py/algo/filtering/pandas/suffixes/suffix_filter.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:41.115932 pm4pyminimal-2.7.9.3/pm4py/algo/filtering/pandas/timestamp/
--rw-rw-rw-   0        0        0      802 2023-12-11 09:33:52.000000 pm4pyminimal-2.7.9.3/pm4py/algo/filtering/pandas/timestamp/__init__.py
--rw-rw-rw-   0        0        0     8208 2024-01-02 13:29:21.000000 pm4pyminimal-2.7.9.3/pm4py/algo/filtering/pandas/timestamp/timestamp_filter.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:41.115932 pm4pyminimal-2.7.9.3/pm4py/algo/filtering/pandas/timestamp_case_grouping/
--rw-rw-rw-   0        0        0      830 2023-12-11 09:33:52.000000 pm4pyminimal-2.7.9.3/pm4py/algo/filtering/pandas/timestamp_case_grouping/__init__.py
--rw-rw-rw-   0        0        0     3499 2024-01-02 13:29:21.000000 pm4pyminimal-2.7.9.3/pm4py/algo/filtering/pandas/timestamp_case_grouping/timestamp_case_grouping_filter.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:41.135343 pm4pyminimal-2.7.9.3/pm4py/algo/filtering/pandas/traces/
--rw-rw-rw-   0        0        0      736 2023-12-11 09:33:52.000000 pm4pyminimal-2.7.9.3/pm4py/algo/filtering/pandas/traces/__init__.py
--rw-rw-rw-   0        0        0     3604 2023-12-11 09:33:52.000000 pm4pyminimal-2.7.9.3/pm4py/algo/filtering/pandas/traces/trace_filter.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:41.142641 pm4pyminimal-2.7.9.3/pm4py/algo/filtering/pandas/variants/
--rw-rw-rw-   0        0        0      734 2023-12-11 09:33:52.000000 pm4pyminimal-2.7.9.3/pm4py/algo/filtering/pandas/variants/__init__.py
--rw-rw-rw-   0        0        0     6083 2023-12-11 09:33:52.000000 pm4pyminimal-2.7.9.3/pm4py/algo/filtering/pandas/variants/variants_filter.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:41.153732 pm4pyminimal-2.7.9.3/pm4py/algo/label_splitting/
--rw-rw-rw-   0        0        0      794 2024-01-02 13:29:21.000000 pm4pyminimal-2.7.9.3/pm4py/algo/label_splitting/__init__.py
--rw-rw-rw-   0        0        0     1921 2024-01-02 13:29:21.000000 pm4pyminimal-2.7.9.3/pm4py/algo/label_splitting/algorithm.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:41.161712 pm4pyminimal-2.7.9.3/pm4py/algo/label_splitting/variants/
--rw-rw-rw-   0        0        0      794 2024-01-02 13:29:21.000000 pm4pyminimal-2.7.9.3/pm4py/algo/label_splitting/variants/__init__.py
--rw-rw-rw-   0        0        0     9446 2024-01-02 13:29:21.000000 pm4pyminimal-2.7.9.3/pm4py/algo/label_splitting/variants/contextual.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:41.165080 pm4pyminimal-2.7.9.3/pm4py/algo/merging/
--rw-rw-rw-   0        0        0      781 2023-12-11 09:33:52.000000 pm4pyminimal-2.7.9.3/pm4py/algo/merging/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:41.175055 pm4pyminimal-2.7.9.3/pm4py/algo/merging/case_relations/
--rw-rw-rw-   0        0        0      801 2023-12-11 09:33:52.000000 pm4pyminimal-2.7.9.3/pm4py/algo/merging/case_relations/__init__.py
--rw-rw-rw-   0        0        0     2326 2023-12-11 09:33:52.000000 pm4pyminimal-2.7.9.3/pm4py/algo/merging/case_relations/algorithm.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:41.191012 pm4pyminimal-2.7.9.3/pm4py/algo/merging/case_relations/variants/
--rw-rw-rw-   0        0        0      797 2023-12-11 09:33:52.000000 pm4pyminimal-2.7.9.3/pm4py/algo/merging/case_relations/variants/__init__.py
--rw-rw-rw-   0        0        0     3498 2024-01-02 13:29:21.000000 pm4pyminimal-2.7.9.3/pm4py/algo/merging/case_relations/variants/pandas.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:41.205971 pm4pyminimal-2.7.9.3/pm4py/algo/organizational_mining/
--rw-rw-rw-   0        0        0      855 2023-12-11 09:33:52.000000 pm4pyminimal-2.7.9.3/pm4py/algo/organizational_mining/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:41.220443 pm4pyminimal-2.7.9.3/pm4py/algo/organizational_mining/local_diagnostics/
--rw-rw-rw-   0        0        0      808 2023-12-11 09:33:52.000000 pm4pyminimal-2.7.9.3/pm4py/algo/organizational_mining/local_diagnostics/__init__.py
--rw-rw-rw-   0        0        0    12440 2023-12-11 09:33:52.000000 pm4pyminimal-2.7.9.3/pm4py/algo/organizational_mining/local_diagnostics/algorithm.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:41.226849 pm4pyminimal-2.7.9.3/pm4py/algo/organizational_mining/network_analysis/
--rw-rw-rw-   0        0        0      817 2023-12-11 09:33:52.000000 pm4pyminimal-2.7.9.3/pm4py/algo/organizational_mining/network_analysis/__init__.py
--rw-rw-rw-   0        0        0     1840 2023-12-11 09:33:52.000000 pm4pyminimal-2.7.9.3/pm4py/algo/organizational_mining/network_analysis/algorithm.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:41.231551 pm4pyminimal-2.7.9.3/pm4py/algo/organizational_mining/network_analysis/variants/
--rw-rw-rw-   0        0        0      816 2023-12-11 09:33:52.000000 pm4pyminimal-2.7.9.3/pm4py/algo/organizational_mining/network_analysis/variants/__init__.py
--rw-rw-rw-   0        0        0    10562 2024-01-15 12:00:43.000000 pm4pyminimal-2.7.9.3/pm4py/algo/organizational_mining/network_analysis/variants/dataframe.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:41.241079 pm4pyminimal-2.7.9.3/pm4py/algo/organizational_mining/resource_profiles/
--rw-rw-rw-   0        0        0      818 2023-12-11 09:33:52.000000 pm4pyminimal-2.7.9.3/pm4py/algo/organizational_mining/resource_profiles/__init__.py
--rw-rw-rw-   0        0        0    12251 2024-01-02 13:29:21.000000 pm4pyminimal-2.7.9.3/pm4py/algo/organizational_mining/resource_profiles/algorithm.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:41.250267 pm4pyminimal-2.7.9.3/pm4py/algo/organizational_mining/resource_profiles/variants/
--rw-rw-rw-   0        0        0      819 2023-12-11 09:33:52.000000 pm4pyminimal-2.7.9.3/pm4py/algo/organizational_mining/resource_profiles/variants/__init__.py
--rw-rw-rw-   0        0        0    23271 2024-01-02 13:29:21.000000 pm4pyminimal-2.7.9.3/pm4py/algo/organizational_mining/resource_profiles/variants/log.py
--rw-rw-rw-   0        0        0    23967 2024-01-15 12:00:43.000000 pm4pyminimal-2.7.9.3/pm4py/algo/organizational_mining/resource_profiles/variants/pandas.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:41.256469 pm4pyminimal-2.7.9.3/pm4py/algo/organizational_mining/roles/
--rw-rw-rw-   0        0        0      814 2023-12-11 09:33:52.000000 pm4pyminimal-2.7.9.3/pm4py/algo/organizational_mining/roles/__init__.py
--rw-rw-rw-   0        0        0     2427 2024-01-02 13:29:21.000000 pm4pyminimal-2.7.9.3/pm4py/algo/organizational_mining/roles/algorithm.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:41.260872 pm4pyminimal-2.7.9.3/pm4py/algo/organizational_mining/roles/common/
--rw-rw-rw-   0        0        0      803 2023-12-11 09:33:52.000000 pm4pyminimal-2.7.9.3/pm4py/algo/organizational_mining/roles/common/__init__.py
--rw-rw-rw-   0        0        0     8411 2023-12-11 09:33:52.000000 pm4pyminimal-2.7.9.3/pm4py/algo/organizational_mining/roles/common/algorithm.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:41.260872 pm4pyminimal-2.7.9.3/pm4py/algo/organizational_mining/roles/variants/
--rw-rw-rw-   0        0        0      807 2023-12-11 09:33:52.000000 pm4pyminimal-2.7.9.3/pm4py/algo/organizational_mining/roles/variants/__init__.py
--rw-rw-rw-   0        0        0     2448 2023-12-11 09:33:52.000000 pm4pyminimal-2.7.9.3/pm4py/algo/organizational_mining/roles/variants/log.py
--rw-rw-rw-   0        0        0     2213 2024-01-15 12:00:43.000000 pm4pyminimal-2.7.9.3/pm4py/algo/organizational_mining/roles/variants/pandas.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:41.280188 pm4pyminimal-2.7.9.3/pm4py/algo/organizational_mining/sna/
--rw-rw-rw-   0        0        0      810 2023-12-11 09:33:52.000000 pm4pyminimal-2.7.9.3/pm4py/algo/organizational_mining/sna/__init__.py
--rw-rw-rw-   0        0        0     3689 2023-12-11 09:33:52.000000 pm4pyminimal-2.7.9.3/pm4py/algo/organizational_mining/sna/algorithm.py
--rw-rw-rw-   0        0        0     3199 2023-12-11 09:33:52.000000 pm4pyminimal-2.7.9.3/pm4py/algo/organizational_mining/sna/util.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:41.283180 pm4pyminimal-2.7.9.3/pm4py/algo/organizational_mining/sna/variants/
--rw-rw-rw-   0        0        0      805 2023-12-11 09:33:52.000000 pm4pyminimal-2.7.9.3/pm4py/algo/organizational_mining/sna/variants/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:41.305812 pm4pyminimal-2.7.9.3/pm4py/algo/organizational_mining/sna/variants/log/
--rw-rw-rw-   0        0        0      857 2023-12-11 09:33:52.000000 pm4pyminimal-2.7.9.3/pm4py/algo/organizational_mining/sna/variants/log/__init__.py
--rw-rw-rw-   0        0        0     3735 2023-12-11 09:33:52.000000 pm4pyminimal-2.7.9.3/pm4py/algo/organizational_mining/sna/variants/log/handover.py
--rw-rw-rw-   0        0        0     3286 2023-12-11 09:33:52.000000 pm4pyminimal-2.7.9.3/pm4py/algo/organizational_mining/sna/variants/log/jointactivities.py
--rw-rw-rw-   0        0        0     3525 2023-12-11 09:33:52.000000 pm4pyminimal-2.7.9.3/pm4py/algo/organizational_mining/sna/variants/log/subcontracting.py
--rw-rw-rw-   0        0        0     3155 2023-12-11 09:33:52.000000 pm4pyminimal-2.7.9.3/pm4py/algo/organizational_mining/sna/variants/log/working_together.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:41.317012 pm4pyminimal-2.7.9.3/pm4py/algo/organizational_mining/sna/variants/pandas/
--rw-rw-rw-   0        0        0      860 2023-12-11 09:33:52.000000 pm4pyminimal-2.7.9.3/pm4py/algo/organizational_mining/sna/variants/pandas/__init__.py
--rw-rw-rw-   0        0        0     4235 2023-12-11 09:33:52.000000 pm4pyminimal-2.7.9.3/pm4py/algo/organizational_mining/sna/variants/pandas/handover.py
--rw-rw-rw-   0        0        0     2998 2024-01-15 12:00:43.000000 pm4pyminimal-2.7.9.3/pm4py/algo/organizational_mining/sna/variants/pandas/jointactivities.py
--rw-rw-rw-   0        0        0     3804 2023-12-11 09:33:52.000000 pm4pyminimal-2.7.9.3/pm4py/algo/organizational_mining/sna/variants/pandas/subcontracting.py
--rw-rw-rw-   0        0        0     3432 2023-12-11 09:33:52.000000 pm4pyminimal-2.7.9.3/pm4py/algo/organizational_mining/sna/variants/pandas/working_together.py
--rw-rw-rw-   0        0        0     7667 2024-01-02 13:29:21.000000 pm4pyminimal-2.7.9.3/pm4py/algo/organizational_mining/util.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:41.319118 pm4pyminimal-2.7.9.3/pm4py/algo/querying/
--rw-rw-rw-   0        0        0      736 2023-12-11 09:33:52.000000 pm4pyminimal-2.7.9.3/pm4py/algo/querying/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:41.321112 pm4pyminimal-2.7.9.3/pm4py/algo/querying/llm/
--rw-rw-rw-   0        0        0      798 2023-12-11 09:33:52.000000 pm4pyminimal-2.7.9.3/pm4py/algo/querying/llm/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:41.353524 pm4pyminimal-2.7.9.3/pm4py/algo/querying/llm/abstractions/
--rw-rw-rw-   0        0        0      960 2023-12-11 09:33:52.000000 pm4pyminimal-2.7.9.3/pm4py/algo/querying/llm/abstractions/__init__.py
--rw-rw-rw-   0        0        0     4006 2023-12-11 09:33:52.000000 pm4pyminimal-2.7.9.3/pm4py/algo/querying/llm/abstractions/case_to_descr.py
--rw-rw-rw-   0        0        0     4382 2024-01-12 06:34:29.000000 pm4pyminimal-2.7.9.3/pm4py/algo/querying/llm/abstractions/declare_to_descr.py
--rw-rw-rw-   0        0        0     3100 2023-12-11 09:33:52.000000 pm4pyminimal-2.7.9.3/pm4py/algo/querying/llm/abstractions/log_to_cols_descr.py
--rw-rw-rw-   0        0        0     9696 2023-12-11 09:33:52.000000 pm4pyminimal-2.7.9.3/pm4py/algo/querying/llm/abstractions/log_to_dfg_descr.py
--rw-rw-rw-   0        0        0     7886 2024-01-02 13:29:21.000000 pm4pyminimal-2.7.9.3/pm4py/algo/querying/llm/abstractions/log_to_fea_descr.py
--rw-rw-rw-   0        0        0    10693 2024-01-02 13:29:21.000000 pm4pyminimal-2.7.9.3/pm4py/algo/querying/llm/abstractions/log_to_variants_descr.py
--rw-rw-rw-   0        0        0     3241 2024-01-12 06:34:29.000000 pm4pyminimal-2.7.9.3/pm4py/algo/querying/llm/abstractions/logske_to_descr.py
--rw-rw-rw-   0        0        0     1931 2023-12-11 09:33:52.000000 pm4pyminimal-2.7.9.3/pm4py/algo/querying/llm/abstractions/net_to_descr.py
--rw-rw-rw-   0        0        0     6145 2023-12-11 09:33:52.000000 pm4pyminimal-2.7.9.3/pm4py/algo/querying/llm/abstractions/ocel_fea_descr.py
--rw-rw-rw-   0        0        0     3680 2023-12-11 09:33:52.000000 pm4pyminimal-2.7.9.3/pm4py/algo/querying/llm/abstractions/ocel_ocdfg_descr.py
--rw-rw-rw-   0        0        0     3004 2023-12-11 09:33:52.000000 pm4pyminimal-2.7.9.3/pm4py/algo/querying/llm/abstractions/stream_to_descr.py
--rw-rw-rw-   0        0        0     2481 2024-01-12 06:34:29.000000 pm4pyminimal-2.7.9.3/pm4py/algo/querying/llm/abstractions/tempprofile_to_descr.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:41.357513 pm4pyminimal-2.7.9.3/pm4py/algo/querying/llm/connectors/
--rw-rw-rw-   0        0        0      791 2023-12-11 09:33:52.000000 pm4pyminimal-2.7.9.3/pm4py/algo/querying/llm/connectors/__init__.py
--rw-rw-rw-   0        0        0     2596 2024-01-02 13:29:21.000000 pm4pyminimal-2.7.9.3/pm4py/algo/querying/llm/connectors/openai.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:41.365875 pm4pyminimal-2.7.9.3/pm4py/algo/querying/llm/utils/
--rw-rw-rw-   0        0        0      787 2024-01-02 13:29:21.000000 pm4pyminimal-2.7.9.3/pm4py/algo/querying/llm/utils/__init__.py
--rw-rw-rw-   0        0        0     1634 2024-01-02 13:29:21.000000 pm4pyminimal-2.7.9.3/pm4py/algo/querying/llm/utils/sql_utils.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:41.367870 pm4pyminimal-2.7.9.3/pm4py/algo/reduction/
--rw-rw-rw-   0        0        0      955 2023-12-11 09:33:52.000000 pm4pyminimal-2.7.9.3/pm4py/algo/reduction/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:41.372984 pm4pyminimal-2.7.9.3/pm4py/algo/reduction/process_tree/
--rw-rw-rw-   0        0        0      799 2023-12-11 09:33:52.000000 pm4pyminimal-2.7.9.3/pm4py/algo/reduction/process_tree/__init__.py
--rw-rw-rw-   0        0        0     1601 2023-12-11 09:33:52.000000 pm4pyminimal-2.7.9.3/pm4py/algo/reduction/process_tree/reducer.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:41.377971 pm4pyminimal-2.7.9.3/pm4py/algo/reduction/process_tree/variants/
--rw-rw-rw-   0        0        0      804 2023-12-11 09:33:52.000000 pm4pyminimal-2.7.9.3/pm4py/algo/reduction/process_tree/variants/__init__.py
--rw-rw-rw-   0        0        0     3743 2023-12-11 09:33:52.000000 pm4pyminimal-2.7.9.3/pm4py/algo/reduction/process_tree/variants/tree_tr_based.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:41.381107 pm4pyminimal-2.7.9.3/pm4py/algo/simulation/
--rw-rw-rw-   0        0        0      904 2023-12-11 09:33:52.000000 pm4pyminimal-2.7.9.3/pm4py/algo/simulation/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:41.385095 pm4pyminimal-2.7.9.3/pm4py/algo/simulation/montecarlo/
--rw-rw-rw-   0        0        0      995 2023-12-11 09:33:52.000000 pm4pyminimal-2.7.9.3/pm4py/algo/simulation/montecarlo/__init__.py
--rw-rw-rw-   0        0        0     4562 2023-12-11 09:33:52.000000 pm4pyminimal-2.7.9.3/pm4py/algo/simulation/montecarlo/algorithm.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:41.389864 pm4pyminimal-2.7.9.3/pm4py/algo/simulation/montecarlo/utils/
--rw-rw-rw-   0        0        0      793 2023-12-11 09:33:52.000000 pm4pyminimal-2.7.9.3/pm4py/algo/simulation/montecarlo/utils/__init__.py
--rw-rw-rw-   0        0        0     5316 2023-12-11 09:33:52.000000 pm4pyminimal-2.7.9.3/pm4py/algo/simulation/montecarlo/utils/replay.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:41.395489 pm4pyminimal-2.7.9.3/pm4py/algo/simulation/montecarlo/variants/
--rw-rw-rw-   0        0        0      807 2023-12-11 09:33:52.000000 pm4pyminimal-2.7.9.3/pm4py/algo/simulation/montecarlo/variants/__init__.py
--rw-rw-rw-   0        0        0    19853 2024-01-02 13:29:21.000000 pm4pyminimal-2.7.9.3/pm4py/algo/simulation/montecarlo/variants/petri_semaph_fifo.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:41.398480 pm4pyminimal-2.7.9.3/pm4py/algo/simulation/playout/
--rw-rw-rw-   0        0        0      806 2023-12-11 09:33:52.000000 pm4pyminimal-2.7.9.3/pm4py/algo/simulation/playout/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:41.402598 pm4pyminimal-2.7.9.3/pm4py/algo/simulation/playout/dfg/
--rw-rw-rw-   0        0        0      801 2023-12-11 09:33:52.000000 pm4pyminimal-2.7.9.3/pm4py/algo/simulation/playout/dfg/__init__.py
--rw-rw-rw-   0        0        0     1940 2023-12-11 09:33:52.000000 pm4pyminimal-2.7.9.3/pm4py/algo/simulation/playout/dfg/algorithm.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:41.410256 pm4pyminimal-2.7.9.3/pm4py/algo/simulation/playout/dfg/variants/
--rw-rw-rw-   0        0        0      811 2023-12-11 09:33:52.000000 pm4pyminimal-2.7.9.3/pm4py/algo/simulation/playout/dfg/variants/__init__.py
--rw-rw-rw-   0        0        0    14627 2024-01-02 13:29:21.000000 pm4pyminimal-2.7.9.3/pm4py/algo/simulation/playout/dfg/variants/classic.py
--rw-rw-rw-   0        0        0     6099 2024-01-02 13:29:21.000000 pm4pyminimal-2.7.9.3/pm4py/algo/simulation/playout/dfg/variants/performance.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:41.415233 pm4pyminimal-2.7.9.3/pm4py/algo/simulation/playout/petri_net/
--rw-rw-rw-   0        0        0      807 2023-12-11 09:33:52.000000 pm4pyminimal-2.7.9.3/pm4py/algo/simulation/playout/petri_net/__init__.py
--rw-rw-rw-   0        0        0     2552 2023-12-11 09:33:52.000000 pm4pyminimal-2.7.9.3/pm4py/algo/simulation/playout/petri_net/algorithm.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:41.424330 pm4pyminimal-2.7.9.3/pm4py/algo/simulation/playout/petri_net/variants/
--rw-rw-rw-   0        0        0      821 2023-12-11 09:33:52.000000 pm4pyminimal-2.7.9.3/pm4py/algo/simulation/playout/petri_net/variants/__init__.py
--rw-rw-rw-   0        0        0     9126 2024-01-02 13:29:21.000000 pm4pyminimal-2.7.9.3/pm4py/algo/simulation/playout/petri_net/variants/basic_playout.py
--rw-rw-rw-   0        0        0     5306 2024-01-02 13:29:21.000000 pm4pyminimal-2.7.9.3/pm4py/algo/simulation/playout/petri_net/variants/extensive.py
--rw-rw-rw-   0        0        0     8008 2024-01-02 13:29:21.000000 pm4pyminimal-2.7.9.3/pm4py/algo/simulation/playout/petri_net/variants/stochastic_playout.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:41.430442 pm4pyminimal-2.7.9.3/pm4py/algo/simulation/playout/process_tree/
--rw-rw-rw-   0        0        0      810 2023-12-11 09:33:52.000000 pm4pyminimal-2.7.9.3/pm4py/algo/simulation/playout/process_tree/__init__.py
--rw-rw-rw-   0        0        0     1862 2023-12-11 09:33:52.000000 pm4pyminimal-2.7.9.3/pm4py/algo/simulation/playout/process_tree/algorithm.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:41.439452 pm4pyminimal-2.7.9.3/pm4py/algo/simulation/playout/process_tree/variants/
--rw-rw-rw-   0        0        0      835 2023-12-11 09:33:52.000000 pm4pyminimal-2.7.9.3/pm4py/algo/simulation/playout/process_tree/variants/__init__.py
--rw-rw-rw-   0        0        0     1679 2023-12-11 09:33:52.000000 pm4pyminimal-2.7.9.3/pm4py/algo/simulation/playout/process_tree/variants/basic_playout.py
--rw-rw-rw-   0        0        0    13571 2023-12-11 09:33:52.000000 pm4pyminimal-2.7.9.3/pm4py/algo/simulation/playout/process_tree/variants/extensive.py
--rw-rw-rw-   0        0        0     4861 2023-12-11 09:33:52.000000 pm4pyminimal-2.7.9.3/pm4py/algo/simulation/playout/process_tree/variants/topbottom.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:41.444045 pm4pyminimal-2.7.9.3/pm4py/algo/simulation/tree_generator/
--rw-rw-rw-   0        0        0      806 2023-12-11 09:33:52.000000 pm4pyminimal-2.7.9.3/pm4py/algo/simulation/tree_generator/__init__.py
--rw-rw-rw-   0        0        0     1765 2023-12-11 09:33:52.000000 pm4pyminimal-2.7.9.3/pm4py/algo/simulation/tree_generator/algorithm.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:41.451260 pm4pyminimal-2.7.9.3/pm4py/algo/simulation/tree_generator/variants/
--rw-rw-rw-   0        0        0      818 2023-12-11 09:33:52.000000 pm4pyminimal-2.7.9.3/pm4py/algo/simulation/tree_generator/variants/__init__.py
--rw-rw-rw-   0        0        0     5357 2023-12-11 09:33:52.000000 pm4pyminimal-2.7.9.3/pm4py/algo/simulation/tree_generator/variants/basic.py
--rw-rw-rw-   0        0        0    12955 2023-12-11 09:33:52.000000 pm4pyminimal-2.7.9.3/pm4py/algo/simulation/tree_generator/variants/ptandloggenerator.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:41.453255 pm4pyminimal-2.7.9.3/pm4py/algo/transformation/
--rw-rw-rw-   0        0        0      808 2023-12-11 09:33:52.000000 pm4pyminimal-2.7.9.3/pm4py/algo/transformation/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:41.458241 pm4pyminimal-2.7.9.3/pm4py/algo/transformation/log_to_features/
--rw-rw-rw-   0        0        0      809 2023-12-11 09:33:52.000000 pm4pyminimal-2.7.9.3/pm4py/algo/transformation/log_to_features/__init__.py
--rw-rw-rw-   0        0        0     2205 2023-12-11 09:33:52.000000 pm4pyminimal-2.7.9.3/pm4py/algo/transformation/log_to_features/algorithm.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:41.463275 pm4pyminimal-2.7.9.3/pm4py/algo/transformation/log_to_features/util/
--rw-rw-rw-   0        0        0      819 2023-12-11 09:33:52.000000 pm4pyminimal-2.7.9.3/pm4py/algo/transformation/log_to_features/util/__init__.py
--rw-rw-rw-   0        0        0     3933 2024-01-02 13:29:21.000000 pm4pyminimal-2.7.9.3/pm4py/algo/transformation/log_to_features/util/locally_linear_embedding.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:41.472351 pm4pyminimal-2.7.9.3/pm4py/algo/transformation/log_to_features/variants/
--rw-rw-rw-   0        0        0      823 2023-12-11 09:33:52.000000 pm4pyminimal-2.7.9.3/pm4py/algo/transformation/log_to_features/variants/__init__.py
--rw-rw-rw-   0        0        0     6689 2023-12-11 09:33:52.000000 pm4pyminimal-2.7.9.3/pm4py/algo/transformation/log_to_features/variants/event_based.py
--rw-rw-rw-   0        0        0     6644 2024-01-15 12:00:43.000000 pm4pyminimal-2.7.9.3/pm4py/algo/transformation/log_to_features/variants/temporal.py
--rw-rw-rw-   0        0        0    50368 2024-01-02 13:29:21.000000 pm4pyminimal-2.7.9.3/pm4py/algo/transformation/log_to_features/variants/trace_based.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:41.478337 pm4pyminimal-2.7.9.3/pm4py/algo/transformation/log_to_interval_tree/
--rw-rw-rw-   0        0        0      999 2023-12-11 09:33:52.000000 pm4pyminimal-2.7.9.3/pm4py/algo/transformation/log_to_interval_tree/__init__.py
--rw-rw-rw-   0        0        0     2171 2023-12-11 09:33:52.000000 pm4pyminimal-2.7.9.3/pm4py/algo/transformation/log_to_interval_tree/algorithm.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:41.484992 pm4pyminimal-2.7.9.3/pm4py/algo/transformation/log_to_interval_tree/variants/
--rw-rw-rw-   0        0        0      814 2023-12-11 09:33:52.000000 pm4pyminimal-2.7.9.3/pm4py/algo/transformation/log_to_interval_tree/variants/__init__.py
--rw-rw-rw-   0        0        0     6365 2023-12-11 09:33:52.000000 pm4pyminimal-2.7.9.3/pm4py/algo/transformation/log_to_interval_tree/variants/open_paths.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:41.489085 pm4pyminimal-2.7.9.3/pm4py/algo/transformation/log_to_target/
--rw-rw-rw-   0        0        0      807 2023-12-11 09:33:52.000000 pm4pyminimal-2.7.9.3/pm4py/algo/transformation/log_to_target/__init__.py
--rw-rw-rw-   0        0        0     2161 2023-12-11 09:33:52.000000 pm4pyminimal-2.7.9.3/pm4py/algo/transformation/log_to_target/algorithm.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:41.504272 pm4pyminimal-2.7.9.3/pm4py/algo/transformation/log_to_target/variants/
--rw-rw-rw-   0        0        0      837 2023-12-11 09:33:52.000000 pm4pyminimal-2.7.9.3/pm4py/algo/transformation/log_to_target/variants/__init__.py
--rw-rw-rw-   0        0        0     2922 2023-12-11 09:33:52.000000 pm4pyminimal-2.7.9.3/pm4py/algo/transformation/log_to_target/variants/next_activity.py
--rw-rw-rw-   0        0        0     2526 2023-12-11 09:33:52.000000 pm4pyminimal-2.7.9.3/pm4py/algo/transformation/log_to_target/variants/next_time.py
--rw-rw-rw-   0        0        0     2385 2023-12-11 09:33:52.000000 pm4pyminimal-2.7.9.3/pm4py/algo/transformation/log_to_target/variants/remaining_time.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:41.508262 pm4pyminimal-2.7.9.3/pm4py/algo/transformation/log_to_trie/
--rw-rw-rw-   0        0        0      795 2023-12-11 09:33:52.000000 pm4pyminimal-2.7.9.3/pm4py/algo/transformation/log_to_trie/__init__.py
--rw-rw-rw-   0        0        0     2261 2024-01-02 13:29:21.000000 pm4pyminimal-2.7.9.3/pm4py/algo/transformation/log_to_trie/algorithm.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:41.511319 pm4pyminimal-2.7.9.3/pm4py/algo/transformation/ocel/
--rw-rw-rw-   0        0        0      807 2023-12-11 09:33:52.000000 pm4pyminimal-2.7.9.3/pm4py/algo/transformation/ocel/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:41.516305 pm4pyminimal-2.7.9.3/pm4py/algo/transformation/ocel/description/
--rw-rw-rw-   0        0        0      736 2023-12-11 09:33:52.000000 pm4pyminimal-2.7.9.3/pm4py/algo/transformation/ocel/description/__init__.py
--rw-rw-rw-   0        0        0     1684 2023-12-11 09:33:52.000000 pm4pyminimal-2.7.9.3/pm4py/algo/transformation/ocel/description/algorithm.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:41.521432 pm4pyminimal-2.7.9.3/pm4py/algo/transformation/ocel/description/variants/
--rw-rw-rw-   0        0        0      736 2023-12-11 09:33:52.000000 pm4pyminimal-2.7.9.3/pm4py/algo/transformation/ocel/description/variants/__init__.py
--rw-rw-rw-   0        0        0     3318 2023-12-11 09:33:52.000000 pm4pyminimal-2.7.9.3/pm4py/algo/transformation/ocel/description/variants/variant1.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:41.523424 pm4pyminimal-2.7.9.3/pm4py/algo/transformation/ocel/features/
--rw-rw-rw-   0        0        0      821 2023-12-11 09:33:52.000000 pm4pyminimal-2.7.9.3/pm4py/algo/transformation/ocel/features/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:41.555179 pm4pyminimal-2.7.9.3/pm4py/algo/transformation/ocel/features/events/
--rw-rw-rw-   0        0        0     1002 2023-12-11 09:33:52.000000 pm4pyminimal-2.7.9.3/pm4py/algo/transformation/ocel/features/events/__init__.py
--rw-rw-rw-   0        0        0     9094 2024-01-02 13:29:21.000000 pm4pyminimal-2.7.9.3/pm4py/algo/transformation/ocel/features/events/algorithm.py
--rw-rw-rw-   0        0        0     2022 2024-01-02 13:29:21.000000 pm4pyminimal-2.7.9.3/pm4py/algo/transformation/ocel/features/events/event_activity.py
--rw-rw-rw-   0        0        0     2250 2024-01-02 13:29:21.000000 pm4pyminimal-2.7.9.3/pm4py/algo/transformation/ocel/features/events/event_end_ot.py
--rw-rw-rw-   0        0        0     2542 2024-01-02 13:29:21.000000 pm4pyminimal-2.7.9.3/pm4py/algo/transformation/ocel/features/events/event_num_attributes.py
--rw-rw-rw-   0        0        0     1691 2024-01-02 13:29:21.000000 pm4pyminimal-2.7.9.3/pm4py/algo/transformation/ocel/features/events/event_num_rel_objs.py
--rw-rw-rw-   0        0        0     2354 2024-01-02 13:29:21.000000 pm4pyminimal-2.7.9.3/pm4py/algo/transformation/ocel/features/events/event_num_rel_objs_type.py
--rw-rw-rw-   0        0        0     2236 2024-01-02 13:29:21.000000 pm4pyminimal-2.7.9.3/pm4py/algo/transformation/ocel/features/events/event_start_ot.py
--rw-rw-rw-   0        0        0     3041 2024-01-02 13:29:21.000000 pm4pyminimal-2.7.9.3/pm4py/algo/transformation/ocel/features/events/event_str_attributes.py
--rw-rw-rw-   0        0        0     2031 2024-01-02 13:29:21.000000 pm4pyminimal-2.7.9.3/pm4py/algo/transformation/ocel/features/events/event_timestamp.py
--rw-rw-rw-   0        0        0     1990 2024-01-02 13:29:21.000000 pm4pyminimal-2.7.9.3/pm4py/algo/transformation/ocel/features/events/new_interactions.py
--rw-rw-rw-   0        0        0     2805 2024-01-02 13:29:21.000000 pm4pyminimal-2.7.9.3/pm4py/algo/transformation/ocel/features/events/related_objects_features.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:41.563049 pm4pyminimal-2.7.9.3/pm4py/algo/transformation/ocel/features/events_objects/
--rw-rw-rw-   0        0        0      831 2023-12-11 09:33:52.000000 pm4pyminimal-2.7.9.3/pm4py/algo/transformation/ocel/features/events_objects/__init__.py
--rw-rw-rw-   0        0        0     3899 2024-01-02 13:29:21.000000 pm4pyminimal-2.7.9.3/pm4py/algo/transformation/ocel/features/events_objects/algorithm.py
--rw-rw-rw-   0        0        0     4959 2024-01-02 13:29:21.000000 pm4pyminimal-2.7.9.3/pm4py/algo/transformation/ocel/features/events_objects/prefix_features.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:41.613602 pm4pyminimal-2.7.9.3/pm4py/algo/transformation/ocel/features/objects/
--rw-rw-rw-   0        0        0     1268 2023-12-11 09:33:52.000000 pm4pyminimal-2.7.9.3/pm4py/algo/transformation/ocel/features/objects/__init__.py
--rw-rw-rw-   0        0        0    20532 2024-01-02 13:29:21.000000 pm4pyminimal-2.7.9.3/pm4py/algo/transformation/ocel/features/objects/algorithm.py
--rw-rw-rw-   0        0        0     3400 2024-01-02 13:29:21.000000 pm4pyminimal-2.7.9.3/pm4py/algo/transformation/ocel/features/objects/obj_con_in_graph_features.py
--rw-rw-rw-   0        0        0     1912 2024-01-02 13:29:21.000000 pm4pyminimal-2.7.9.3/pm4py/algo/transformation/ocel/features/objects/object_cobirth_graph.py
--rw-rw-rw-   0        0        0     1912 2024-01-02 13:29:21.000000 pm4pyminimal-2.7.9.3/pm4py/algo/transformation/ocel/features/objects/object_codeath_graph.py
--rw-rw-rw-   0        0        0     1988 2024-01-02 13:29:21.000000 pm4pyminimal-2.7.9.3/pm4py/algo/transformation/ocel/features/objects/object_degree_centrality.py
--rw-rw-rw-   0        0        0     2100 2024-01-02 13:29:21.000000 pm4pyminimal-2.7.9.3/pm4py/algo/transformation/ocel/features/objects/object_general_descendants_graph.py
--rw-rw-rw-   0        0        0     2152 2024-01-02 13:29:21.000000 pm4pyminimal-2.7.9.3/pm4py/algo/transformation/ocel/features/objects/object_general_inheritance_graph.py
--rw-rw-rw-   0        0        0     1942 2024-01-02 13:29:21.000000 pm4pyminimal-2.7.9.3/pm4py/algo/transformation/ocel/features/objects/object_general_interaction_graph.py
--rw-rw-rw-   0        0        0     2080 2024-01-02 13:29:21.000000 pm4pyminimal-2.7.9.3/pm4py/algo/transformation/ocel/features/objects/object_lifecycle_activities.py
--rw-rw-rw-   0        0        0     2197 2024-01-02 13:29:21.000000 pm4pyminimal-2.7.9.3/pm4py/algo/transformation/ocel/features/objects/object_lifecycle_duration.py
--rw-rw-rw-   0        0        0     1794 2024-01-02 13:29:21.000000 pm4pyminimal-2.7.9.3/pm4py/algo/transformation/ocel/features/objects/object_lifecycle_length.py
--rw-rw-rw-   0        0        0     2205 2024-01-02 13:29:21.000000 pm4pyminimal-2.7.9.3/pm4py/algo/transformation/ocel/features/objects/object_lifecycle_paths.py
--rw-rw-rw-   0        0        0     1920 2024-01-02 13:29:21.000000 pm4pyminimal-2.7.9.3/pm4py/algo/transformation/ocel/features/objects/object_lifecycle_unq_act.py
--rw-rw-rw-   0        0        0     2586 2024-01-02 13:29:21.000000 pm4pyminimal-2.7.9.3/pm4py/algo/transformation/ocel/features/objects/object_num_attributes.py
--rw-rw-rw-   0        0        0     3062 2024-01-02 13:29:21.000000 pm4pyminimal-2.7.9.3/pm4py/algo/transformation/ocel/features/objects/object_str_attributes.py
--rw-rw-rw-   0        0        0     2455 2024-01-02 13:29:21.000000 pm4pyminimal-2.7.9.3/pm4py/algo/transformation/ocel/features/objects/object_work_in_progress.py
--rw-rw-rw-   0        0        0     2486 2024-01-02 13:29:21.000000 pm4pyminimal-2.7.9.3/pm4py/algo/transformation/ocel/features/objects/objects_interaction_graph_ot.py
--rw-rw-rw-   0        0        0     3063 2024-01-02 13:29:21.000000 pm4pyminimal-2.7.9.3/pm4py/algo/transformation/ocel/features/objects/related_activities_features.py
--rw-rw-rw-   0        0        0     2788 2024-01-02 13:29:21.000000 pm4pyminimal-2.7.9.3/pm4py/algo/transformation/ocel/features/objects/related_events_features.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:41.632000 pm4pyminimal-2.7.9.3/pm4py/algo/transformation/ocel/graphs/
--rw-rw-rw-   0        0        0      906 2023-12-11 09:33:52.000000 pm4pyminimal-2.7.9.3/pm4py/algo/transformation/ocel/graphs/__init__.py
--rw-rw-rw-   0        0        0     2305 2024-01-02 13:29:21.000000 pm4pyminimal-2.7.9.3/pm4py/algo/transformation/ocel/graphs/object_cobirth_graph.py
--rw-rw-rw-   0        0        0     2103 2024-01-02 13:29:21.000000 pm4pyminimal-2.7.9.3/pm4py/algo/transformation/ocel/graphs/object_codeath_graph.py
--rw-rw-rw-   0        0        0     2327 2024-01-02 13:29:21.000000 pm4pyminimal-2.7.9.3/pm4py/algo/transformation/ocel/graphs/object_descendants_graph.py
--rw-rw-rw-   0        0        0     2852 2024-01-02 13:29:21.000000 pm4pyminimal-2.7.9.3/pm4py/algo/transformation/ocel/graphs/object_inheritance_graph.py
--rw-rw-rw-   0        0        0     1736 2024-01-02 13:29:21.000000 pm4pyminimal-2.7.9.3/pm4py/algo/transformation/ocel/graphs/object_interaction_graph.py
--rw-rw-rw-   0        0        0     3641 2024-01-02 13:29:21.000000 pm4pyminimal-2.7.9.3/pm4py/algo/transformation/ocel/graphs/ocel20_computation.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:41.637984 pm4pyminimal-2.7.9.3/pm4py/algo/transformation/ocel/split_ocel/
--rw-rw-rw-   0        0        0      809 2023-12-11 09:33:52.000000 pm4pyminimal-2.7.9.3/pm4py/algo/transformation/ocel/split_ocel/__init__.py
--rw-rw-rw-   0        0        0     1730 2023-12-11 09:33:52.000000 pm4pyminimal-2.7.9.3/pm4py/algo/transformation/ocel/split_ocel/algorithm.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:41.645069 pm4pyminimal-2.7.9.3/pm4py/algo/transformation/ocel/split_ocel/variants/
--rw-rw-rw-   0        0        0      819 2023-12-11 09:33:52.000000 pm4pyminimal-2.7.9.3/pm4py/algo/transformation/ocel/split_ocel/variants/__init__.py
--rw-rw-rw-   0        0        0     3429 2024-01-02 13:29:21.000000 pm4pyminimal-2.7.9.3/pm4py/algo/transformation/ocel/split_ocel/variants/ancestors_descendants.py
--rw-rw-rw-   0        0        0     3467 2024-01-02 13:29:21.000000 pm4pyminimal-2.7.9.3/pm4py/algo/transformation/ocel/split_ocel/variants/connected_components.py
--rw-rw-rw-   0        0        0    20646 2023-12-11 09:33:52.000000 pm4pyminimal-2.7.9.3/pm4py/analysis.py
--rw-rw-rw-   0        0        0    13471 2024-01-02 13:29:21.000000 pm4pyminimal-2.7.9.3/pm4py/cli.py
--rw-rw-rw-   0        0        0    48213 2024-01-02 13:29:21.000000 pm4pyminimal-2.7.9.3/pm4py/conformance.py
--rw-rw-rw-   0        0        0    19636 2023-12-11 09:33:52.000000 pm4pyminimal-2.7.9.3/pm4py/connectors.py
--rw-rw-rw-   0        0        0    20826 2023-12-11 09:33:52.000000 pm4pyminimal-2.7.9.3/pm4py/convert.py
--rw-rw-rw-   0        0        0    47943 2024-01-02 13:29:21.000000 pm4pyminimal-2.7.9.3/pm4py/discovery.py
--rw-rw-rw-   0        0        0    63155 2024-01-15 12:00:43.000000 pm4pyminimal-2.7.9.3/pm4py/filtering.py
--rw-rw-rw-   0        0        0     5192 2023-12-11 09:33:52.000000 pm4pyminimal-2.7.9.3/pm4py/hof.py
--rw-rw-rw-   0        0        0    18976 2024-01-04 13:34:19.000000 pm4pyminimal-2.7.9.3/pm4py/llm.py
--rw-rw-rw-   0        0        0     1098 2024-01-16 10:11:31.000000 pm4pyminimal-2.7.9.3/pm4py/meta.py
--rw-rw-rw-   0        0        0    16160 2024-01-02 13:29:21.000000 pm4pyminimal-2.7.9.3/pm4py/ml.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:41.647061 pm4pyminimal-2.7.9.3/pm4py/objects/
--rw-rw-rw-   0        0        0      947 2023-12-11 09:33:52.000000 pm4pyminimal-2.7.9.3/pm4py/objects/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:41.653533 pm4pyminimal-2.7.9.3/pm4py/objects/bpmn/
--rw-rw-rw-   0        0        0      913 2023-12-11 09:33:52.000000 pm4pyminimal-2.7.9.3/pm4py/objects/bpmn/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:41.658519 pm4pyminimal-2.7.9.3/pm4py/objects/bpmn/exporter/
--rw-rw-rw-   0        0        0      794 2023-12-11 09:33:52.000000 pm4pyminimal-2.7.9.3/pm4py/objects/bpmn/exporter/__init__.py
--rw-rw-rw-   0        0        0     2130 2023-12-11 09:33:52.000000 pm4pyminimal-2.7.9.3/pm4py/objects/bpmn/exporter/exporter.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:41.663009 pm4pyminimal-2.7.9.3/pm4py/objects/bpmn/exporter/variants/
--rw-rw-rw-   0        0        0      790 2023-12-11 09:33:52.000000 pm4pyminimal-2.7.9.3/pm4py/objects/bpmn/exporter/variants/__init__.py
--rw-rw-rw-   0        0        0     7688 2024-01-02 13:29:21.000000 pm4pyminimal-2.7.9.3/pm4py/objects/bpmn/exporter/variants/etree.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:41.666998 pm4pyminimal-2.7.9.3/pm4py/objects/bpmn/importer/
--rw-rw-rw-   0        0        0      794 2023-12-11 09:33:52.000000 pm4pyminimal-2.7.9.3/pm4py/objects/bpmn/importer/__init__.py
--rw-rw-rw-   0        0        0     2085 2023-12-11 09:33:52.000000 pm4pyminimal-2.7.9.3/pm4py/objects/bpmn/importer/importer.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:41.671297 pm4pyminimal-2.7.9.3/pm4py/objects/bpmn/importer/variants/
--rw-rw-rw-   0        0        0      789 2023-12-11 09:33:52.000000 pm4pyminimal-2.7.9.3/pm4py/objects/bpmn/importer/variants/__init__.py
--rw-rw-rw-   0        0        0    17373 2023-12-11 09:33:52.000000 pm4pyminimal-2.7.9.3/pm4py/objects/bpmn/importer/variants/lxml.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:41.676285 pm4pyminimal-2.7.9.3/pm4py/objects/bpmn/layout/
--rw-rw-rw-   0        0        0      792 2023-12-11 09:33:52.000000 pm4pyminimal-2.7.9.3/pm4py/objects/bpmn/layout/__init__.py
--rw-rw-rw-   0        0        0     1534 2023-12-11 09:33:52.000000 pm4pyminimal-2.7.9.3/pm4py/objects/bpmn/layout/layouter.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:41.681416 pm4pyminimal-2.7.9.3/pm4py/objects/bpmn/layout/variants/
--rw-rw-rw-   0        0        0      793 2023-12-11 09:33:52.000000 pm4pyminimal-2.7.9.3/pm4py/objects/bpmn/layout/variants/__init__.py
--rw-rw-rw-   0        0        0    18042 2023-12-11 09:33:52.000000 pm4pyminimal-2.7.9.3/pm4py/objects/bpmn/layout/variants/graphviz.py
--rw-rw-rw-   0        0        0    19676 2023-12-11 09:33:52.000000 pm4pyminimal-2.7.9.3/pm4py/objects/bpmn/obj.py
--rw-rw-rw-   0        0        0     9205 2023-12-11 09:33:52.000000 pm4pyminimal-2.7.9.3/pm4py/objects/bpmn/semantics.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:41.689519 pm4pyminimal-2.7.9.3/pm4py/objects/bpmn/util/
--rw-rw-rw-   0        0        0      802 2023-12-11 09:33:52.000000 pm4pyminimal-2.7.9.3/pm4py/objects/bpmn/util/__init__.py
--rw-rw-rw-   0        0        0     6246 2023-12-11 09:33:52.000000 pm4pyminimal-2.7.9.3/pm4py/objects/bpmn/util/bpmn_utils.py
--rw-rw-rw-   0        0        0     3352 2023-12-11 09:33:52.000000 pm4pyminimal-2.7.9.3/pm4py/objects/bpmn/util/reduction.py
--rw-rw-rw-   0        0        0     3729 2023-12-11 09:33:52.000000 pm4pyminimal-2.7.9.3/pm4py/objects/bpmn/util/sorting.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:41.692511 pm4pyminimal-2.7.9.3/pm4py/objects/conversion/
--rw-rw-rw-   0        0        0      825 2023-12-11 09:33:52.000000 pm4pyminimal-2.7.9.3/pm4py/objects/conversion/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:41.703585 pm4pyminimal-2.7.9.3/pm4py/objects/conversion/bpmn/
--rw-rw-rw-   0        0        0      797 2023-12-11 09:33:52.000000 pm4pyminimal-2.7.9.3/pm4py/objects/conversion/bpmn/__init__.py
--rw-rw-rw-   0        0        0     1160 2023-12-11 09:33:52.000000 pm4pyminimal-2.7.9.3/pm4py/objects/conversion/bpmn/converter.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:41.710672 pm4pyminimal-2.7.9.3/pm4py/objects/conversion/bpmn/variants/
--rw-rw-rw-   0        0        0      799 2023-12-11 09:33:52.000000 pm4pyminimal-2.7.9.3/pm4py/objects/conversion/bpmn/variants/__init__.py
--rw-rw-rw-   0        0        0    10026 2023-12-11 09:33:52.000000 pm4pyminimal-2.7.9.3/pm4py/objects/conversion/bpmn/variants/to_petri_net.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:41.711615 pm4pyminimal-2.7.9.3/pm4py/objects/conversion/dfg/
--rw-rw-rw-   0        0        0      796 2023-12-11 09:33:52.000000 pm4pyminimal-2.7.9.3/pm4py/objects/conversion/dfg/__init__.py
--rw-rw-rw-   0        0        0     1340 2023-12-11 09:33:52.000000 pm4pyminimal-2.7.9.3/pm4py/objects/conversion/dfg/converter.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:41.711615 pm4pyminimal-2.7.9.3/pm4py/objects/conversion/dfg/variants/
--rw-rw-rw-   0        0        0      860 2023-12-11 09:33:52.000000 pm4pyminimal-2.7.9.3/pm4py/objects/conversion/dfg/variants/__init__.py
--rw-rw-rw-   0        0        0     3494 2023-12-11 09:33:52.000000 pm4pyminimal-2.7.9.3/pm4py/objects/conversion/dfg/variants/to_petri_net_activity_defines_place.py
--rw-rw-rw-   0        0        0     4229 2023-12-11 09:33:52.000000 pm4pyminimal-2.7.9.3/pm4py/objects/conversion/dfg/variants/to_petri_net_invisibles_no_duplicates.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:41.727236 pm4pyminimal-2.7.9.3/pm4py/objects/conversion/heuristics_net/
--rw-rw-rw-   0        0        0      807 2023-12-11 09:33:52.000000 pm4pyminimal-2.7.9.3/pm4py/objects/conversion/heuristics_net/__init__.py
--rw-rw-rw-   0        0        0     1384 2023-12-11 09:33:52.000000 pm4pyminimal-2.7.9.3/pm4py/objects/conversion/heuristics_net/converter.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:41.727236 pm4pyminimal-2.7.9.3/pm4py/objects/conversion/heuristics_net/variants/
--rw-rw-rw-   0        0        0      809 2023-12-11 09:33:52.000000 pm4pyminimal-2.7.9.3/pm4py/objects/conversion/heuristics_net/variants/__init__.py
--rw-rw-rw-   0        0        0    11773 2023-12-11 09:33:52.000000 pm4pyminimal-2.7.9.3/pm4py/objects/conversion/heuristics_net/variants/to_petri_net.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:41.746794 pm4pyminimal-2.7.9.3/pm4py/objects/conversion/log/
--rw-rw-rw-   0        0        0      807 2023-12-11 09:33:52.000000 pm4pyminimal-2.7.9.3/pm4py/objects/conversion/log/__init__.py
--rw-rw-rw-   0        0        0     1061 2023-12-11 09:33:52.000000 pm4pyminimal-2.7.9.3/pm4py/objects/conversion/log/constants.py
--rw-rw-rw-   0        0        0     1319 2023-12-11 09:33:52.000000 pm4pyminimal-2.7.9.3/pm4py/objects/conversion/log/converter.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:41.767232 pm4pyminimal-2.7.9.3/pm4py/objects/conversion/log/variants/
--rw-rw-rw-   0        0        0      870 2023-12-11 09:33:52.000000 pm4pyminimal-2.7.9.3/pm4py/objects/conversion/log/variants/__init__.py
--rw-rw-rw-   0        0        0     1923 2023-12-11 09:33:52.000000 pm4pyminimal-2.7.9.3/pm4py/objects/conversion/log/variants/df_to_event_log_1v.py
--rw-rw-rw-   0        0        0     2535 2023-12-11 09:33:52.000000 pm4pyminimal-2.7.9.3/pm4py/objects/conversion/log/variants/df_to_event_log_nv.py
--rw-rw-rw-   0        0        0     2585 2024-01-02 13:29:21.000000 pm4pyminimal-2.7.9.3/pm4py/objects/conversion/log/variants/to_data_frame.py
--rw-rw-rw-   0        0        0     4332 2024-01-02 13:29:21.000000 pm4pyminimal-2.7.9.3/pm4py/objects/conversion/log/variants/to_event_log.py
--rw-rw-rw-   0        0        0    10224 2024-01-02 13:29:21.000000 pm4pyminimal-2.7.9.3/pm4py/objects/conversion/log/variants/to_event_stream.py
--rw-rw-rw-   0        0        0     5236 2023-12-11 09:33:52.000000 pm4pyminimal-2.7.9.3/pm4py/objects/conversion/log/variants/to_nx.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:41.772336 pm4pyminimal-2.7.9.3/pm4py/objects/conversion/ocel/
--rw-rw-rw-   0        0        0      799 2023-12-11 09:33:52.000000 pm4pyminimal-2.7.9.3/pm4py/objects/conversion/ocel/__init__.py
--rw-rw-rw-   0        0        0     1814 2023-12-11 09:33:52.000000 pm4pyminimal-2.7.9.3/pm4py/objects/conversion/ocel/converter.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:41.780974 pm4pyminimal-2.7.9.3/pm4py/objects/conversion/ocel/variants/
--rw-rw-rw-   0        0        0      820 2023-12-11 09:33:52.000000 pm4pyminimal-2.7.9.3/pm4py/objects/conversion/ocel/variants/__init__.py
--rw-rw-rw-   0        0        0     4056 2023-12-11 09:33:52.000000 pm4pyminimal-2.7.9.3/pm4py/objects/conversion/ocel/variants/ocel_features_to_nx.py
--rw-rw-rw-   0        0        0     4164 2023-12-11 09:33:52.000000 pm4pyminimal-2.7.9.3/pm4py/objects/conversion/ocel/variants/ocel_to_nx.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:41.787952 pm4pyminimal-2.7.9.3/pm4py/objects/conversion/powl/
--rw-rw-rw-   0        0        0      781 2023-12-11 09:33:52.000000 pm4pyminimal-2.7.9.3/pm4py/objects/conversion/powl/__init__.py
--rw-rw-rw-   0        0        0     1494 2024-01-02 13:29:21.000000 pm4pyminimal-2.7.9.3/pm4py/objects/conversion/powl/converter.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:41.794052 pm4pyminimal-2.7.9.3/pm4py/objects/conversion/powl/variants/
--rw-rw-rw-   0        0        0      790 2023-12-11 09:33:52.000000 pm4pyminimal-2.7.9.3/pm4py/objects/conversion/powl/variants/__init__.py
--rw-rw-rw-   0        0        0    11169 2024-01-02 13:29:21.000000 pm4pyminimal-2.7.9.3/pm4py/objects/conversion/powl/variants/to_petri_net.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:41.799657 pm4pyminimal-2.7.9.3/pm4py/objects/conversion/process_tree/
--rw-rw-rw-   0        0        0      805 2023-12-11 09:33:52.000000 pm4pyminimal-2.7.9.3/pm4py/objects/conversion/process_tree/__init__.py
--rw-rw-rw-   0        0        0     1824 2023-12-11 09:33:52.000000 pm4pyminimal-2.7.9.3/pm4py/objects/conversion/process_tree/converter.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:41.808954 pm4pyminimal-2.7.9.3/pm4py/objects/conversion/process_tree/variants/
--rw-rw-rw-   0        0        0      850 2023-12-11 09:33:52.000000 pm4pyminimal-2.7.9.3/pm4py/objects/conversion/process_tree/variants/__init__.py
--rw-rw-rw-   0        0        0    10139 2023-12-11 09:33:52.000000 pm4pyminimal-2.7.9.3/pm4py/objects/conversion/process_tree/variants/to_bpmn.py
--rw-rw-rw-   0        0        0    21550 2023-12-11 09:33:52.000000 pm4pyminimal-2.7.9.3/pm4py/objects/conversion/process_tree/variants/to_petri_net.py
--rw-rw-rw-   0        0        0     4772 2023-12-11 09:33:52.000000 pm4pyminimal-2.7.9.3/pm4py/objects/conversion/process_tree/variants/to_petri_net_transition_bordered.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:41.814938 pm4pyminimal-2.7.9.3/pm4py/objects/conversion/wf_net/
--rw-rw-rw-   0        0        0      799 2023-12-11 09:33:52.000000 pm4pyminimal-2.7.9.3/pm4py/objects/conversion/wf_net/__init__.py
--rw-rw-rw-   0        0        0     1167 2023-12-11 09:33:52.000000 pm4pyminimal-2.7.9.3/pm4py/objects/conversion/wf_net/converter.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:41.821627 pm4pyminimal-2.7.9.3/pm4py/objects/conversion/wf_net/variants/
--rw-rw-rw-   0        0        0      813 2023-12-11 09:33:52.000000 pm4pyminimal-2.7.9.3/pm4py/objects/conversion/wf_net/variants/__init__.py
--rw-rw-rw-   0        0        0     3774 2023-12-11 09:33:52.000000 pm4pyminimal-2.7.9.3/pm4py/objects/conversion/wf_net/variants/to_bpmn.py
--rw-rw-rw-   0        0        0    10849 2023-12-11 09:33:52.000000 pm4pyminimal-2.7.9.3/pm4py/objects/conversion/wf_net/variants/to_process_tree.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:41.829606 pm4pyminimal-2.7.9.3/pm4py/objects/dfg/
--rw-rw-rw-   0        0        0      796 2023-12-11 09:33:52.000000 pm4pyminimal-2.7.9.3/pm4py/objects/dfg/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:41.833315 pm4pyminimal-2.7.9.3/pm4py/objects/dfg/exporter/
--rw-rw-rw-   0        0        0      793 2023-12-11 09:33:52.000000 pm4pyminimal-2.7.9.3/pm4py/objects/dfg/exporter/__init__.py
--rw-rw-rw-   0        0        0     2041 2023-12-11 09:33:52.000000 pm4pyminimal-2.7.9.3/pm4py/objects/dfg/exporter/exporter.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:41.838301 pm4pyminimal-2.7.9.3/pm4py/objects/dfg/exporter/variants/
--rw-rw-rw-   0        0        0      791 2023-12-11 09:33:52.000000 pm4pyminimal-2.7.9.3/pm4py/objects/dfg/exporter/variants/__init__.py
--rw-rw-rw-   0        0        0     4571 2023-12-11 09:33:52.000000 pm4pyminimal-2.7.9.3/pm4py/objects/dfg/exporter/variants/classic.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:41.842396 pm4pyminimal-2.7.9.3/pm4py/objects/dfg/filtering/
--rw-rw-rw-   0        0        0      734 2023-12-11 09:33:52.000000 pm4pyminimal-2.7.9.3/pm4py/objects/dfg/filtering/__init__.py
--rw-rw-rw-   0        0        0      788 2023-12-11 09:33:52.000000 pm4pyminimal-2.7.9.3/pm4py/objects/dfg/filtering/dfg_filtering.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:41.849377 pm4pyminimal-2.7.9.3/pm4py/objects/dfg/importer/
--rw-rw-rw-   0        0        0      793 2023-12-11 09:33:52.000000 pm4pyminimal-2.7.9.3/pm4py/objects/dfg/importer/__init__.py
--rw-rw-rw-   0        0        0     2278 2023-12-11 09:33:52.000000 pm4pyminimal-2.7.9.3/pm4py/objects/dfg/importer/importer.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:41.856329 pm4pyminimal-2.7.9.3/pm4py/objects/dfg/importer/variants/
--rw-rw-rw-   0        0        0      791 2023-12-11 09:33:52.000000 pm4pyminimal-2.7.9.3/pm4py/objects/dfg/importer/variants/__init__.py
--rw-rw-rw-   0        0        0     4037 2023-12-11 09:33:52.000000 pm4pyminimal-2.7.9.3/pm4py/objects/dfg/importer/variants/classic.py
--rw-rw-rw-   0        0        0     1881 2023-12-11 09:33:52.000000 pm4pyminimal-2.7.9.3/pm4py/objects/dfg/obj.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:41.864626 pm4pyminimal-2.7.9.3/pm4py/objects/dfg/retrieval/
--rw-rw-rw-   0        0        0      734 2023-12-11 09:33:52.000000 pm4pyminimal-2.7.9.3/pm4py/objects/dfg/retrieval/__init__.py
--rw-rw-rw-   0        0        0      913 2023-12-11 09:33:52.000000 pm4pyminimal-2.7.9.3/pm4py/objects/dfg/retrieval/log.py
--rw-rw-rw-   0        0        0      873 2023-12-11 09:33:52.000000 pm4pyminimal-2.7.9.3/pm4py/objects/dfg/retrieval/pandas.py
--rw-rw-rw-   0        0        0     5092 2023-12-11 09:33:52.000000 pm4pyminimal-2.7.9.3/pm4py/objects/dfg/util.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:41.869638 pm4pyminimal-2.7.9.3/pm4py/objects/dfg/utils/
--rw-rw-rw-   0        0        0      781 2023-12-11 09:33:52.000000 pm4pyminimal-2.7.9.3/pm4py/objects/dfg/utils/__init__.py
--rw-rw-rw-   0        0        0    26490 2023-12-11 09:33:52.000000 pm4pyminimal-2.7.9.3/pm4py/objects/dfg/utils/dfg_utils.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:41.880335 pm4pyminimal-2.7.9.3/pm4py/objects/heuristics_net/
--rw-rw-rw-   0        0        0      802 2023-12-11 09:33:52.000000 pm4pyminimal-2.7.9.3/pm4py/objects/heuristics_net/__init__.py
--rw-rw-rw-   0        0        0     1226 2023-12-11 09:33:52.000000 pm4pyminimal-2.7.9.3/pm4py/objects/heuristics_net/defaults.py
--rw-rw-rw-   0        0        0     2689 2023-12-11 09:33:52.000000 pm4pyminimal-2.7.9.3/pm4py/objects/heuristics_net/edge.py
--rw-rw-rw-   0        0        0     9877 2023-12-11 09:33:52.000000 pm4pyminimal-2.7.9.3/pm4py/objects/heuristics_net/node.py
--rw-rw-rw-   0        0        0     5684 2023-12-11 09:33:52.000000 pm4pyminimal-2.7.9.3/pm4py/objects/heuristics_net/obj.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:41.884323 pm4pyminimal-2.7.9.3/pm4py/objects/log/
--rw-rw-rw-   0        0        0      795 2023-12-11 09:33:52.000000 pm4pyminimal-2.7.9.3/pm4py/objects/log/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:41.887314 pm4pyminimal-2.7.9.3/pm4py/objects/log/exporter/
--rw-rw-rw-   0        0        0      778 2023-12-11 09:33:52.000000 pm4pyminimal-2.7.9.3/pm4py/objects/log/exporter/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:41.890486 pm4pyminimal-2.7.9.3/pm4py/objects/log/exporter/xes/
--rw-rw-rw-   0        0        0      803 2023-12-11 09:33:52.000000 pm4pyminimal-2.7.9.3/pm4py/objects/log/exporter/xes/__init__.py
--rw-rw-rw-   0        0        0     2578 2023-12-11 09:33:52.000000 pm4pyminimal-2.7.9.3/pm4py/objects/log/exporter/xes/exporter.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:41.896471 pm4pyminimal-2.7.9.3/pm4py/objects/log/exporter/xes/util/
--rw-rw-rw-   0        0        0      795 2023-12-11 09:33:52.000000 pm4pyminimal-2.7.9.3/pm4py/objects/log/exporter/xes/util/__init__.py
--rw-rw-rw-   0        0        0     1423 2023-12-11 09:33:52.000000 pm4pyminimal-2.7.9.3/pm4py/objects/log/exporter/xes/util/compression.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:41.902612 pm4pyminimal-2.7.9.3/pm4py/objects/log/exporter/xes/variants/
--rw-rw-rw-   0        0        0      815 2023-12-11 09:33:52.000000 pm4pyminimal-2.7.9.3/pm4py/objects/log/exporter/xes/variants/__init__.py
--rw-rw-rw-   0        0        0    12326 2023-12-11 09:33:52.000000 pm4pyminimal-2.7.9.3/pm4py/objects/log/exporter/xes/variants/etree_xes_exp.py
--rw-rw-rw-   0        0        0    10430 2023-12-11 09:33:52.000000 pm4pyminimal-2.7.9.3/pm4py/objects/log/exporter/xes/variants/line_by_line.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:41.904606 pm4pyminimal-2.7.9.3/pm4py/objects/log/importer/
--rw-rw-rw-   0        0        0      778 2023-12-11 09:33:52.000000 pm4pyminimal-2.7.9.3/pm4py/objects/log/importer/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:41.909594 pm4pyminimal-2.7.9.3/pm4py/objects/log/importer/xes/
--rw-rw-rw-   0        0        0      797 2023-12-11 09:33:52.000000 pm4pyminimal-2.7.9.3/pm4py/objects/log/importer/xes/__init__.py
--rw-rw-rw-   0        0        0     4379 2023-12-11 09:33:52.000000 pm4pyminimal-2.7.9.3/pm4py/objects/log/importer/xes/importer.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:41.929254 pm4pyminimal-2.7.9.3/pm4py/objects/log/importer/xes/variants/
--rw-rw-rw-   0        0        0      850 2023-12-11 09:33:52.000000 pm4pyminimal-2.7.9.3/pm4py/objects/log/importer/xes/variants/__init__.py
--rw-rw-rw-   0        0        0     9534 2023-12-11 09:33:52.000000 pm4pyminimal-2.7.9.3/pm4py/objects/log/importer/xes/variants/chunk_regex.py
--rw-rw-rw-   0        0        0    17582 2023-12-11 09:33:52.000000 pm4pyminimal-2.7.9.3/pm4py/objects/log/importer/xes/variants/iterparse.py
--rw-rw-rw-   0        0        0    17851 2023-12-11 09:33:52.000000 pm4pyminimal-2.7.9.3/pm4py/objects/log/importer/xes/variants/iterparse_20.py
--rw-rw-rw-   0        0        0    18150 2023-12-11 09:33:52.000000 pm4pyminimal-2.7.9.3/pm4py/objects/log/importer/xes/variants/iterparse_mem_compressed.py
--rw-rw-rw-   0        0        0    11435 2023-12-11 09:33:52.000000 pm4pyminimal-2.7.9.3/pm4py/objects/log/importer/xes/variants/line_by_line.py
--rw-rw-rw-   0        0        0     2094 2024-01-02 13:29:21.000000 pm4pyminimal-2.7.9.3/pm4py/objects/log/importer/xes/variants/rustxes.py
--rw-rw-rw-   0        0        0    12284 2023-12-11 09:33:52.000000 pm4pyminimal-2.7.9.3/pm4py/objects/log/obj.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:41.974396 pm4pyminimal-2.7.9.3/pm4py/objects/log/util/
--rw-rw-rw-   0        0        0     1010 2023-12-11 09:33:52.000000 pm4pyminimal-2.7.9.3/pm4py/objects/log/util/__init__.py
--rw-rw-rw-   0        0        0     3127 2023-12-11 09:33:52.000000 pm4pyminimal-2.7.9.3/pm4py/objects/log/util/activities_to_alphabet.py
--rw-rw-rw-   0        0        0     3114 2023-12-11 09:33:52.000000 pm4pyminimal-2.7.9.3/pm4py/objects/log/util/artificial.py
--rw-rw-rw-   0        0        0     3974 2023-12-11 09:33:52.000000 pm4pyminimal-2.7.9.3/pm4py/objects/log/util/basic_filter.py
--rw-rw-rw-   0        0        0    18992 2024-01-15 12:00:43.000000 pm4pyminimal-2.7.9.3/pm4py/objects/log/util/dataframe_utils.py
--rw-rw-rw-   0        0        0     2283 2023-12-11 09:33:52.000000 pm4pyminimal-2.7.9.3/pm4py/objects/log/util/filtering_utils.py
--rw-rw-rw-   0        0        0     4856 2024-01-02 13:29:21.000000 pm4pyminimal-2.7.9.3/pm4py/objects/log/util/get_class_representation.py
--rw-rw-rw-   0        0        0     3195 2023-12-11 09:33:52.000000 pm4pyminimal-2.7.9.3/pm4py/objects/log/util/get_log_encoded.py
--rw-rw-rw-   0        0        0     8099 2023-12-11 09:33:52.000000 pm4pyminimal-2.7.9.3/pm4py/objects/log/util/get_prefixes.py
--rw-rw-rw-   0        0        0     1752 2023-12-11 09:33:52.000000 pm4pyminimal-2.7.9.3/pm4py/objects/log/util/index_attribute.py
--rw-rw-rw-   0        0        0     4067 2023-12-11 09:33:52.000000 pm4pyminimal-2.7.9.3/pm4py/objects/log/util/insert_classifier.py
--rw-rw-rw-   0        0        0    12476 2024-01-02 13:29:21.000000 pm4pyminimal-2.7.9.3/pm4py/objects/log/util/interval_lifecycle.py
--rw-rw-rw-   0        0        0     5167 2023-12-11 09:33:52.000000 pm4pyminimal-2.7.9.3/pm4py/objects/log/util/log.py
--rw-rw-rw-   0        0        0     4389 2023-12-11 09:33:52.000000 pm4pyminimal-2.7.9.3/pm4py/objects/log/util/log_regex.py
--rw-rw-rw-   0        0        0     2867 2023-12-11 09:33:52.000000 pm4pyminimal-2.7.9.3/pm4py/objects/log/util/move_attrs_to_trace.py
--rw-rw-rw-   0        0        0     4527 2023-12-11 09:33:52.000000 pm4pyminimal-2.7.9.3/pm4py/objects/log/util/pandas_log_wrapper.py
--rw-rw-rw-   0        0        0     4094 2024-01-15 12:00:43.000000 pm4pyminimal-2.7.9.3/pm4py/objects/log/util/pandas_numpy_variants.py
--rw-rw-rw-   0        0        0     2465 2023-12-11 09:33:52.000000 pm4pyminimal-2.7.9.3/pm4py/objects/log/util/sampling.py
--rw-rw-rw-   0        0        0     6049 2023-12-11 09:33:52.000000 pm4pyminimal-2.7.9.3/pm4py/objects/log/util/sorting.py
--rw-rw-rw-   0        0        0     2078 2023-12-11 09:33:52.000000 pm4pyminimal-2.7.9.3/pm4py/objects/log/util/split_train_test.py
--rw-rw-rw-   0        0        0     1695 2023-12-11 09:33:52.000000 pm4pyminimal-2.7.9.3/pm4py/objects/log/util/xes.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:41.981639 pm4pyminimal-2.7.9.3/pm4py/objects/ocel/
--rw-rw-rw-   0        0        0      819 2023-12-11 09:33:52.000000 pm4pyminimal-2.7.9.3/pm4py/objects/ocel/__init__.py
--rw-rw-rw-   0        0        0     2372 2023-12-11 09:33:52.000000 pm4pyminimal-2.7.9.3/pm4py/objects/ocel/constants.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:41.982636 pm4pyminimal-2.7.9.3/pm4py/objects/ocel/exporter/
--rw-rw-rw-   0        0        0      911 2023-12-11 09:33:52.000000 pm4pyminimal-2.7.9.3/pm4py/objects/ocel/exporter/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:41.986626 pm4pyminimal-2.7.9.3/pm4py/objects/ocel/exporter/csv/
--rw-rw-rw-   0        0        0      798 2023-12-11 09:33:52.000000 pm4pyminimal-2.7.9.3/pm4py/objects/ocel/exporter/csv/__init__.py
--rw-rw-rw-   0        0        0     1695 2023-12-11 09:33:52.000000 pm4pyminimal-2.7.9.3/pm4py/objects/ocel/exporter/csv/exporter.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:41.990713 pm4pyminimal-2.7.9.3/pm4py/objects/ocel/exporter/csv/variants/
--rw-rw-rw-   0        0        0      795 2023-12-11 09:33:52.000000 pm4pyminimal-2.7.9.3/pm4py/objects/ocel/exporter/csv/variants/__init__.py
--rw-rw-rw-   0        0        0     1927 2023-12-11 09:33:52.000000 pm4pyminimal-2.7.9.3/pm4py/objects/ocel/exporter/csv/variants/pandas.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:41.996698 pm4pyminimal-2.7.9.3/pm4py/objects/ocel/exporter/jsonocel/
--rw-rw-rw-   0        0        0      803 2023-12-11 09:33:52.000000 pm4pyminimal-2.7.9.3/pm4py/objects/ocel/exporter/jsonocel/__init__.py
--rw-rw-rw-   0        0        0     1635 2023-12-11 09:33:52.000000 pm4pyminimal-2.7.9.3/pm4py/objects/ocel/exporter/jsonocel/exporter.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:42.005429 pm4pyminimal-2.7.9.3/pm4py/objects/ocel/exporter/jsonocel/variants/
--rw-rw-rw-   0        0        0      826 2023-12-11 09:33:52.000000 pm4pyminimal-2.7.9.3/pm4py/objects/ocel/exporter/jsonocel/variants/__init__.py
--rw-rw-rw-   0        0        0     5448 2024-01-02 13:29:21.000000 pm4pyminimal-2.7.9.3/pm4py/objects/ocel/exporter/jsonocel/variants/classic.py
--rw-rw-rw-   0        0        0     5591 2023-12-11 09:33:52.000000 pm4pyminimal-2.7.9.3/pm4py/objects/ocel/exporter/jsonocel/variants/ocel20.py
--rw-rw-rw-   0        0        0     4247 2023-12-11 09:33:52.000000 pm4pyminimal-2.7.9.3/pm4py/objects/ocel/exporter/jsonocel/variants/ocel20_standard.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:42.010807 pm4pyminimal-2.7.9.3/pm4py/objects/ocel/exporter/sqlite/
--rw-rw-rw-   0        0        0      803 2023-12-11 09:33:52.000000 pm4pyminimal-2.7.9.3/pm4py/objects/ocel/exporter/sqlite/__init__.py
--rw-rw-rw-   0        0        0     1673 2023-12-11 09:33:52.000000 pm4pyminimal-2.7.9.3/pm4py/objects/ocel/exporter/sqlite/exporter.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:42.017788 pm4pyminimal-2.7.9.3/pm4py/objects/ocel/exporter/sqlite/variants/
--rw-rw-rw-   0        0        0      809 2023-12-11 09:33:52.000000 pm4pyminimal-2.7.9.3/pm4py/objects/ocel/exporter/sqlite/variants/__init__.py
--rw-rw-rw-   0        0        0     4931 2024-01-02 13:29:21.000000 pm4pyminimal-2.7.9.3/pm4py/objects/ocel/exporter/sqlite/variants/ocel20.py
--rw-rw-rw-   0        0        0     1679 2023-12-11 09:33:52.000000 pm4pyminimal-2.7.9.3/pm4py/objects/ocel/exporter/sqlite/variants/pandas_exporter.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:42.022922 pm4pyminimal-2.7.9.3/pm4py/objects/ocel/exporter/util/
--rw-rw-rw-   0        0        0      797 2023-12-11 09:33:52.000000 pm4pyminimal-2.7.9.3/pm4py/objects/ocel/exporter/util/__init__.py
--rw-rw-rw-   0        0        0     1658 2024-01-02 13:29:21.000000 pm4pyminimal-2.7.9.3/pm4py/objects/ocel/exporter/util/clean_dataframes.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:42.027911 pm4pyminimal-2.7.9.3/pm4py/objects/ocel/exporter/xmlocel/
--rw-rw-rw-   0        0        0      802 2023-12-11 09:33:52.000000 pm4pyminimal-2.7.9.3/pm4py/objects/ocel/exporter/xmlocel/__init__.py
--rw-rw-rw-   0        0        0     1578 2023-12-11 09:33:52.000000 pm4pyminimal-2.7.9.3/pm4py/objects/ocel/exporter/xmlocel/exporter.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:42.036008 pm4pyminimal-2.7.9.3/pm4py/objects/ocel/exporter/xmlocel/variants/
--rw-rw-rw-   0        0        0      734 2023-12-11 09:33:52.000000 pm4pyminimal-2.7.9.3/pm4py/objects/ocel/exporter/xmlocel/variants/__init__.py
--rw-rw-rw-   0        0        0     8129 2024-01-02 13:29:21.000000 pm4pyminimal-2.7.9.3/pm4py/objects/ocel/exporter/xmlocel/variants/classic.py
--rw-rw-rw-   0        0        0     8746 2023-12-11 09:33:52.000000 pm4pyminimal-2.7.9.3/pm4py/objects/ocel/exporter/xmlocel/variants/ocel20.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:42.039891 pm4pyminimal-2.7.9.3/pm4py/objects/ocel/importer/
--rw-rw-rw-   0        0        0      905 2023-12-11 09:33:52.000000 pm4pyminimal-2.7.9.3/pm4py/objects/ocel/importer/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:42.047982 pm4pyminimal-2.7.9.3/pm4py/objects/ocel/importer/csv/
--rw-rw-rw-   0        0        0      798 2023-12-11 09:33:52.000000 pm4pyminimal-2.7.9.3/pm4py/objects/ocel/importer/csv/__init__.py
--rw-rw-rw-   0        0        0     1731 2023-12-11 09:33:52.000000 pm4pyminimal-2.7.9.3/pm4py/objects/ocel/importer/csv/importer.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:42.055219 pm4pyminimal-2.7.9.3/pm4py/objects/ocel/importer/csv/variants/
--rw-rw-rw-   0        0        0      795 2023-12-11 09:33:52.000000 pm4pyminimal-2.7.9.3/pm4py/objects/ocel/importer/csv/variants/__init__.py
--rw-rw-rw-   0        0        0     2211 2024-01-02 13:29:21.000000 pm4pyminimal-2.7.9.3/pm4py/objects/ocel/importer/csv/variants/pandas.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:42.062663 pm4pyminimal-2.7.9.3/pm4py/objects/ocel/importer/jsonocel/
--rw-rw-rw-   0        0        0      803 2023-12-11 09:33:52.000000 pm4pyminimal-2.7.9.3/pm4py/objects/ocel/importer/jsonocel/__init__.py
--rw-rw-rw-   0        0        0     1641 2023-12-11 09:33:52.000000 pm4pyminimal-2.7.9.3/pm4py/objects/ocel/importer/jsonocel/importer.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:42.069860 pm4pyminimal-2.7.9.3/pm4py/objects/ocel/importer/jsonocel/variants/
--rw-rw-rw-   0        0        0      818 2023-12-11 09:33:52.000000 pm4pyminimal-2.7.9.3/pm4py/objects/ocel/importer/jsonocel/variants/__init__.py
--rw-rw-rw-   0        0        0     7338 2024-01-16 10:09:19.000000 pm4pyminimal-2.7.9.3/pm4py/objects/ocel/importer/jsonocel/variants/classic.py
--rw-rw-rw-   0        0        0     3863 2023-12-11 09:33:52.000000 pm4pyminimal-2.7.9.3/pm4py/objects/ocel/importer/jsonocel/variants/ocel20_standard.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:42.074848 pm4pyminimal-2.7.9.3/pm4py/objects/ocel/importer/sqlite/
--rw-rw-rw-   0        0        0      803 2023-12-11 09:33:52.000000 pm4pyminimal-2.7.9.3/pm4py/objects/ocel/importer/sqlite/__init__.py
--rw-rw-rw-   0        0        0     1704 2023-12-11 09:33:52.000000 pm4pyminimal-2.7.9.3/pm4py/objects/ocel/importer/sqlite/importer.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:42.088267 pm4pyminimal-2.7.9.3/pm4py/objects/ocel/importer/sqlite/variants/
--rw-rw-rw-   0        0        0      809 2023-12-11 09:33:52.000000 pm4pyminimal-2.7.9.3/pm4py/objects/ocel/importer/sqlite/variants/__init__.py
--rw-rw-rw-   0        0        0     8462 2024-01-16 10:09:19.000000 pm4pyminimal-2.7.9.3/pm4py/objects/ocel/importer/sqlite/variants/ocel20.py
--rw-rw-rw-   0        0        0     2620 2024-01-02 13:29:21.000000 pm4pyminimal-2.7.9.3/pm4py/objects/ocel/importer/sqlite/variants/pandas_importer.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:42.095934 pm4pyminimal-2.7.9.3/pm4py/objects/ocel/importer/xmlocel/
--rw-rw-rw-   0        0        0      802 2023-12-11 09:33:52.000000 pm4pyminimal-2.7.9.3/pm4py/objects/ocel/importer/xmlocel/__init__.py
--rw-rw-rw-   0        0        0     1611 2023-12-11 09:33:52.000000 pm4pyminimal-2.7.9.3/pm4py/objects/ocel/importer/xmlocel/importer.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:42.103045 pm4pyminimal-2.7.9.3/pm4py/objects/ocel/importer/xmlocel/variants/
--rw-rw-rw-   0        0        0      800 2023-12-11 09:33:52.000000 pm4pyminimal-2.7.9.3/pm4py/objects/ocel/importer/xmlocel/variants/__init__.py
--rw-rw-rw-   0        0        0     8919 2024-01-02 13:29:21.000000 pm4pyminimal-2.7.9.3/pm4py/objects/ocel/importer/xmlocel/variants/classic.py
--rw-rw-rw-   0        0        0    10021 2024-01-16 10:09:19.000000 pm4pyminimal-2.7.9.3/pm4py/objects/ocel/importer/xmlocel/variants/ocel20.py
--rw-rw-rw-   0        0        0     7221 2024-01-02 13:29:21.000000 pm4pyminimal-2.7.9.3/pm4py/objects/ocel/obj.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:42.191516 pm4pyminimal-2.7.9.3/pm4py/objects/ocel/util/
--rw-rw-rw-   0        0        0     1067 2023-12-11 09:33:52.000000 pm4pyminimal-2.7.9.3/pm4py/objects/ocel/util/__init__.py
--rw-rw-rw-   0        0        0     1690 2023-12-11 09:33:52.000000 pm4pyminimal-2.7.9.3/pm4py/objects/ocel/util/attributes_names.py
--rw-rw-rw-   0        0        0     2156 2023-12-11 09:33:52.000000 pm4pyminimal-2.7.9.3/pm4py/objects/ocel/util/attributes_per_type.py
--rw-rw-rw-   0        0        0     2424 2023-12-11 09:33:52.000000 pm4pyminimal-2.7.9.3/pm4py/objects/ocel/util/convergence_divergence_diagnostics.py
--rw-rw-rw-   0        0        0     2690 2023-12-11 09:33:52.000000 pm4pyminimal-2.7.9.3/pm4py/objects/ocel/util/e2o_qualification.py
--rw-rw-rw-   0        0        0     3809 2024-01-02 13:29:21.000000 pm4pyminimal-2.7.9.3/pm4py/objects/ocel/util/ev_att_to_obj_type.py
--rw-rw-rw-   0        0        0     4453 2024-01-02 13:29:21.000000 pm4pyminimal-2.7.9.3/pm4py/objects/ocel/util/event_prefix_suffix_per_obj.py
--rw-rw-rw-   0        0        0     2215 2024-01-02 13:29:21.000000 pm4pyminimal-2.7.9.3/pm4py/objects/ocel/util/events_per_object_type.py
--rw-rw-rw-   0        0        0     3274 2024-01-02 13:29:21.000000 pm4pyminimal-2.7.9.3/pm4py/objects/ocel/util/events_per_type_per_activity.py
--rw-rw-rw-   0        0        0     1654 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/objects/ocel/util/explode.py
--rw-rw-rw-   0        0        0     5068 2024-01-02 13:29:21.000000 pm4pyminimal-2.7.9.3/pm4py/objects/ocel/util/extended_table.py
--rw-rw-rw-   0        0        0     6565 2024-01-02 13:29:21.000000 pm4pyminimal-2.7.9.3/pm4py/objects/ocel/util/filtering_utils.py
--rw-rw-rw-   0        0        0     3069 2024-01-02 13:29:21.000000 pm4pyminimal-2.7.9.3/pm4py/objects/ocel/util/flattening.py
--rw-rw-rw-   0        0        0    17070 2024-01-02 13:29:21.000000 pm4pyminimal-2.7.9.3/pm4py/objects/ocel/util/log_ocel.py
--rw-rw-rw-   0        0        0      942 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/objects/ocel/util/names_stripping.py
--rw-rw-rw-   0        0        0     3274 2024-01-02 13:29:21.000000 pm4pyminimal-2.7.9.3/pm4py/objects/ocel/util/objects_per_type_per_activity.py
--rw-rw-rw-   0        0        0     1974 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/objects/ocel/util/ocel_consistency.py
--rw-rw-rw-   0        0        0     1976 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/objects/ocel/util/ocel_iterator.py
--rw-rw-rw-   0        0        0     5167 2024-01-02 13:29:21.000000 pm4pyminimal-2.7.9.3/pm4py/objects/ocel/util/ocel_to_dict_types_rel.py
--rw-rw-rw-   0        0        0     3510 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/objects/ocel/util/ocel_type_renaming.py
--rw-rw-rw-   0        0        0     2478 2024-01-02 13:29:21.000000 pm4pyminimal-2.7.9.3/pm4py/objects/ocel/util/parent_children_ref.py
--rw-rw-rw-   0        0        0     1362 2024-01-02 13:29:21.000000 pm4pyminimal-2.7.9.3/pm4py/objects/ocel/util/related_events.py
--rw-rw-rw-   0        0        0     1830 2024-01-02 13:29:21.000000 pm4pyminimal-2.7.9.3/pm4py/objects/ocel/util/related_objects.py
--rw-rw-rw-   0        0        0     2610 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/objects/ocel/util/rename_objs_ot_tim_lex.py
--rw-rw-rw-   0        0        0     3783 2024-01-02 13:29:21.000000 pm4pyminimal-2.7.9.3/pm4py/objects/ocel/util/sampling.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:42.204188 pm4pyminimal-2.7.9.3/pm4py/objects/ocel/validation/
--rw-rw-rw-   0        0        0      795 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/objects/ocel/validation/__init__.py
--rw-rw-rw-   0        0        0     1389 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/objects/ocel/validation/jsonocel.py
--rw-rw-rw-   0        0        0    14786 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/objects/ocel/validation/ocel20_rel_validation.py
--rw-rw-rw-   0        0        0     1212 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/objects/ocel/validation/xmlocel.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:42.206183 pm4pyminimal-2.7.9.3/pm4py/objects/org/
--rw-rw-rw-   0        0        0      776 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/objects/org/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:42.212286 pm4pyminimal-2.7.9.3/pm4py/objects/org/roles/
--rw-rw-rw-   0        0        0      775 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/objects/org/roles/__init__.py
--rw-rw-rw-   0        0        0     1339 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/objects/org/roles/obj.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:42.217303 pm4pyminimal-2.7.9.3/pm4py/objects/org/sna/
--rw-rw-rw-   0        0        0      773 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/objects/org/sna/__init__.py
--rw-rw-rw-   0        0        0     1029 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/objects/org/sna/obj.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:42.232118 pm4pyminimal-2.7.9.3/pm4py/objects/petri_net/
--rw-rw-rw-   0        0        0      828 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/objects/petri_net/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:42.240096 pm4pyminimal-2.7.9.3/pm4py/objects/petri_net/data_petri_nets/
--rw-rw-rw-   0        0        0      734 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/objects/petri_net/data_petri_nets/__init__.py
--rw-rw-rw-   0        0        0     1287 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/objects/petri_net/data_petri_nets/data_marking.py
--rw-rw-rw-   0        0        0     6212 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/objects/petri_net/data_petri_nets/semantics.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:42.249073 pm4pyminimal-2.7.9.3/pm4py/objects/petri_net/exporter/
--rw-rw-rw-   0        0        0      799 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/objects/petri_net/exporter/__init__.py
--rw-rw-rw-   0        0        0     2366 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/objects/petri_net/exporter/exporter.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:42.257346 pm4pyminimal-2.7.9.3/pm4py/objects/petri_net/exporter/variants/
--rw-rw-rw-   0        0        0      794 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/objects/petri_net/exporter/variants/__init__.py
--rw-rw-rw-   0        0        0    13002 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/objects/petri_net/exporter/variants/pnml.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:42.263580 pm4pyminimal-2.7.9.3/pm4py/objects/petri_net/importer/
--rw-rw-rw-   0        0        0      799 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/objects/petri_net/importer/__init__.py
--rw-rw-rw-   0        0        0     1910 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/objects/petri_net/importer/importer.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:42.267569 pm4pyminimal-2.7.9.3/pm4py/objects/petri_net/importer/variants/
--rw-rw-rw-   0        0        0      794 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/objects/petri_net/importer/variants/__init__.py
--rw-rw-rw-   0        0        0    15369 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/objects/petri_net/importer/variants/pnml.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:42.272888 pm4pyminimal-2.7.9.3/pm4py/objects/petri_net/inhibitor_reset/
--rw-rw-rw-   0        0        0      734 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/objects/petri_net/inhibitor_reset/__init__.py
--rw-rw-rw-   0        0        0     4617 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/objects/petri_net/inhibitor_reset/semantics.py
--rw-rw-rw-   0        0        0    13270 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/objects/petri_net/obj.py
--rw-rw-rw-   0        0        0     1225 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/objects/petri_net/properties.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:42.282229 pm4pyminimal-2.7.9.3/pm4py/objects/petri_net/saw_net/
--rw-rw-rw-   0        0        0      805 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/objects/petri_net/saw_net/__init__.py
--rw-rw-rw-   0        0        0     4799 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/objects/petri_net/saw_net/convert.py
--rw-rw-rw-   0        0        0     1546 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/objects/petri_net/saw_net/obj.py
--rw-rw-rw-   0        0        0    10711 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/objects/petri_net/saw_net/semantics.py
--rw-rw-rw-   0        0        0     1503 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/objects/petri_net/sem_interface.py
--rw-rw-rw-   0        0        0     5339 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/objects/petri_net/semantics.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:42.287214 pm4pyminimal-2.7.9.3/pm4py/objects/petri_net/stochastic/
--rw-rw-rw-   0        0        0      799 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/objects/petri_net/stochastic/__init__.py
--rw-rw-rw-   0        0        0     1448 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/objects/petri_net/stochastic/obj.py
--rw-rw-rw-   0        0        0     2607 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/objects/petri_net/stochastic/semantics.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:42.327132 pm4pyminimal-2.7.9.3/pm4py/objects/petri_net/utils/
--rw-rw-rw-   0        0        0     1035 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/objects/petri_net/utils/__init__.py
--rw-rw-rw-   0        0        0    19297 2024-01-04 10:14:42.000000 pm4pyminimal-2.7.9.3/pm4py/objects/petri_net/utils/align_utils.py
--rw-rw-rw-   0        0        0     5923 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/objects/petri_net/utils/check_soundness.py
--rw-rw-rw-   0        0        0     4014 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/objects/petri_net/utils/consumption_matrix.py
--rw-rw-rw-   0        0        0     6609 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/objects/petri_net/utils/decomposition.py
--rw-rw-rw-   0        0        0     1672 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/objects/petri_net/utils/embed_stochastic_map.py
--rw-rw-rw-   0        0        0     5751 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/objects/petri_net/utils/explore_path.py
--rw-rw-rw-   0        0        0     1195 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/objects/petri_net/utils/final_marking.py
--rw-rw-rw-   0        0        0     2272 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/objects/petri_net/utils/incidence_matrix.py
--rw-rw-rw-   0        0        0     1227 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/objects/petri_net/utils/initial_marking.py
--rw-rw-rw-   0        0        0     4243 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/objects/petri_net/utils/murata.py
--rw-rw-rw-   0        0        0     4281 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/objects/petri_net/utils/networkx_graph.py
--rw-rw-rw-   0        0        0     4071 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/objects/petri_net/utils/obj_marking.py
--rw-rw-rw-   0        0        0    22973 2024-01-02 13:29:21.000000 pm4pyminimal-2.7.9.3/pm4py/objects/petri_net/utils/performance_map.py
--rw-rw-rw-   0        0        0    20395 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/objects/petri_net/utils/petri_utils.py
--rw-rw-rw-   0        0        0     4602 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/objects/petri_net/utils/projection.py
--rw-rw-rw-   0        0        0     5570 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/objects/petri_net/utils/reachability_graph.py
--rw-rw-rw-   0        0        0    14266 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/objects/petri_net/utils/reduction.py
--rw-rw-rw-   0        0        0     7288 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/objects/petri_net/utils/synchronous_product.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:42.339318 pm4pyminimal-2.7.9.3/pm4py/objects/powl/
--rw-rw-rw-   0        0        0     6732 2024-01-02 13:29:21.000000 pm4pyminimal-2.7.9.3/pm4py/objects/powl/BinaryRelation.py
--rw-rw-rw-   0        0        0      772 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/objects/powl/__init__.py
--rw-rw-rw-   0        0        0      804 2024-01-02 13:29:21.000000 pm4pyminimal-2.7.9.3/pm4py/objects/powl/constants.py
--rw-rw-rw-   0        0        0    15122 2024-01-02 13:29:21.000000 pm4pyminimal-2.7.9.3/pm4py/objects/powl/obj.py
--rw-rw-rw-   0        0        0     5268 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/objects/powl/parser.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:42.349291 pm4pyminimal-2.7.9.3/pm4py/objects/process_tree/
--rw-rw-rw-   0        0        0      929 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/objects/process_tree/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:42.352926 pm4pyminimal-2.7.9.3/pm4py/objects/process_tree/exporter/
--rw-rw-rw-   0        0        0      802 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/objects/process_tree/exporter/__init__.py
--rw-rw-rw-   0        0        0     1888 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/objects/process_tree/exporter/exporter.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:42.358946 pm4pyminimal-2.7.9.3/pm4py/objects/process_tree/exporter/variants/
--rw-rw-rw-   0        0        0      797 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/objects/process_tree/exporter/variants/__init__.py
--rw-rw-rw-   0        0        0     5832 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/objects/process_tree/exporter/variants/ptml.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:42.364019 pm4pyminimal-2.7.9.3/pm4py/objects/process_tree/importer/
--rw-rw-rw-   0        0        0      802 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/objects/process_tree/importer/__init__.py
--rw-rw-rw-   0        0        0     2048 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/objects/process_tree/importer/importer.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:42.368009 pm4pyminimal-2.7.9.3/pm4py/objects/process_tree/importer/variants/
--rw-rw-rw-   0        0        0      797 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/objects/process_tree/importer/variants/__init__.py
--rw-rw-rw-   0        0        0     5476 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/objects/process_tree/importer/variants/ptml.py
--rw-rw-rw-   0        0        0     8283 2024-01-02 13:29:21.000000 pm4pyminimal-2.7.9.3/pm4py/objects/process_tree/obj.py
--rw-rw-rw-   0        0        0     8883 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/objects/process_tree/semantics.py
--rw-rw-rw-   0        0        0      887 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/objects/process_tree/state.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:42.377581 pm4pyminimal-2.7.9.3/pm4py/objects/process_tree/utils/
--rw-rw-rw-   0        0        0      734 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/objects/process_tree/utils/__init__.py
--rw-rw-rw-   0        0        0     7128 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/objects/process_tree/utils/bottomup.py
--rw-rw-rw-   0        0        0    15834 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/objects/process_tree/utils/generic.py
--rw-rw-rw-   0        0        0     3438 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/objects/process_tree/utils/regex.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:42.383787 pm4pyminimal-2.7.9.3/pm4py/objects/random_variables/
--rw-rw-rw-   0        0        0     1034 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/objects/random_variables/__init__.py
--rw-rw-rw-   0        0        0     3878 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/objects/random_variables/basic_structure.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:42.388855 pm4pyminimal-2.7.9.3/pm4py/objects/random_variables/constant0/
--rw-rw-rw-   0        0        0      804 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/objects/random_variables/constant0/__init__.py
--rw-rw-rw-   0        0        0     3586 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/objects/random_variables/constant0/random_variable.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:42.392927 pm4pyminimal-2.7.9.3/pm4py/objects/random_variables/exponential/
--rw-rw-rw-   0        0        0      818 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/objects/random_variables/exponential/__init__.py
--rw-rw-rw-   0        0        0     3684 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/objects/random_variables/exponential/random_variable.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:42.397913 pm4pyminimal-2.7.9.3/pm4py/objects/random_variables/gamma/
--rw-rw-rw-   0        0        0      800 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/objects/random_variables/gamma/__init__.py
--rw-rw-rw-   0        0        0     3841 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/objects/random_variables/gamma/random_variable.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:42.402900 pm4pyminimal-2.7.9.3/pm4py/objects/random_variables/lognormal/
--rw-rw-rw-   0        0        0      804 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/objects/random_variables/lognormal/__init__.py
--rw-rw-rw-   0        0        0     3568 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/objects/random_variables/lognormal/random_variable.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:42.405892 pm4pyminimal-2.7.9.3/pm4py/objects/random_variables/normal/
--rw-rw-rw-   0        0        0      801 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/objects/random_variables/normal/__init__.py
--rw-rw-rw-   0        0        0     3594 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/objects/random_variables/normal/random_variable.py
--rw-rw-rw-   0        0        0     9224 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/objects/random_variables/random_variable.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:42.409556 pm4pyminimal-2.7.9.3/pm4py/objects/random_variables/uniform/
--rw-rw-rw-   0        0        0      802 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/objects/random_variables/uniform/__init__.py
--rw-rw-rw-   0        0        0     3588 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/objects/random_variables/uniform/random_variable.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:42.418535 pm4pyminimal-2.7.9.3/pm4py/objects/stochastic_petri/
--rw-rw-rw-   0        0        0      988 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/objects/stochastic_petri/__init__.py
--rw-rw-rw-   0        0        0    12887 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/objects/stochastic_petri/ctmc.py
--rw-rw-rw-   0        0        0     4714 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/objects/stochastic_petri/tangible_reachability.py
--rw-rw-rw-   0        0        0     1616 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/objects/stochastic_petri/utils.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:42.425622 pm4pyminimal-2.7.9.3/pm4py/objects/transition_system/
--rw-rw-rw-   0        0        0      803 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/objects/transition_system/__init__.py
--rw-rw-rw-   0        0        0      825 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/objects/transition_system/constants.py
--rw-rw-rw-   0        0        0     3958 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/objects/transition_system/obj.py
--rw-rw-rw-   0        0        0     3625 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/objects/transition_system/utils.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:42.429713 pm4pyminimal-2.7.9.3/pm4py/objects/trie/
--rw-rw-rw-   0        0        0      770 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/objects/trie/__init__.py
--rw-rw-rw-   0        0        0     1911 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/objects/trie/obj.py
--rw-rw-rw-   0        0        0    23143 2024-01-15 12:00:43.000000 pm4pyminimal-2.7.9.3/pm4py/ocel.py
--rw-rw-rw-   0        0        0    14594 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/org.py
--rw-rw-rw-   0        0        0     3805 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/privacy.py
--rw-rw-rw-   0        0        0    15303 2024-01-16 10:09:19.000000 pm4pyminimal-2.7.9.3/pm4py/read.py
--rw-rw-rw-   0        0        0     4578 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/sim.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:42.430710 pm4pyminimal-2.7.9.3/pm4py/statistics/
--rw-rw-rw-   0        0        0      899 2024-01-02 13:29:21.000000 pm4pyminimal-2.7.9.3/pm4py/statistics/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:42.433701 pm4pyminimal-2.7.9.3/pm4py/statistics/attributes/
--rw-rw-rw-   0        0        0      795 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/statistics/attributes/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:42.437690 pm4pyminimal-2.7.9.3/pm4py/statistics/attributes/common/
--rw-rw-rw-   0        0        0      786 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/statistics/attributes/common/__init__.py
--rw-rw-rw-   0        0        0     6611 2024-01-02 13:29:21.000000 pm4pyminimal-2.7.9.3/pm4py/statistics/attributes/common/get.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:42.444823 pm4pyminimal-2.7.9.3/pm4py/statistics/attributes/log/
--rw-rw-rw-   0        0        0      791 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/statistics/attributes/log/__init__.py
--rw-rw-rw-   0        0        0    13311 2024-01-02 13:29:21.000000 pm4pyminimal-2.7.9.3/pm4py/statistics/attributes/log/get.py
--rw-rw-rw-   0        0        0     6905 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/statistics/attributes/log/select.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:42.449212 pm4pyminimal-2.7.9.3/pm4py/statistics/attributes/pandas/
--rw-rw-rw-   0        0        0      786 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/statistics/attributes/pandas/__init__.py
--rw-rw-rw-   0        0        0     9777 2024-01-15 12:00:43.000000 pm4pyminimal-2.7.9.3/pm4py/statistics/attributes/pandas/get.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:42.451207 pm4pyminimal-2.7.9.3/pm4py/statistics/concurrent_activities/
--rw-rw-rw-   0        0        0      798 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/statistics/concurrent_activities/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:42.455196 pm4pyminimal-2.7.9.3/pm4py/statistics/concurrent_activities/log/
--rw-rw-rw-   0        0        0      794 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/statistics/concurrent_activities/log/__init__.py
--rw-rw-rw-   0        0        0     4081 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/statistics/concurrent_activities/log/get.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:42.460275 pm4pyminimal-2.7.9.3/pm4py/statistics/concurrent_activities/pandas/
--rw-rw-rw-   0        0        0      797 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/statistics/concurrent_activities/pandas/__init__.py
--rw-rw-rw-   0        0        0     3686 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/statistics/concurrent_activities/pandas/get.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:42.462273 pm4pyminimal-2.7.9.3/pm4py/statistics/end_activities/
--rw-rw-rw-   0        0        0      799 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/statistics/end_activities/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:42.467255 pm4pyminimal-2.7.9.3/pm4py/statistics/end_activities/common/
--rw-rw-rw-   0        0        0      790 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/statistics/end_activities/common/__init__.py
--rw-rw-rw-   0        0        0     1791 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/statistics/end_activities/common/get.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:42.470553 pm4pyminimal-2.7.9.3/pm4py/statistics/end_activities/log/
--rw-rw-rw-   0        0        0      787 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/statistics/end_activities/log/__init__.py
--rw-rw-rw-   0        0        0     2746 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/statistics/end_activities/log/get.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:42.474542 pm4pyminimal-2.7.9.3/pm4py/statistics/end_activities/pandas/
--rw-rw-rw-   0        0        0      790 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/statistics/end_activities/pandas/__init__.py
--rw-rw-rw-   0        0        0     2665 2024-01-15 12:00:43.000000 pm4pyminimal-2.7.9.3/pm4py/statistics/end_activities/pandas/get.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:42.477537 pm4pyminimal-2.7.9.3/pm4py/statistics/eventually_follows/
--rw-rw-rw-   0        0        0      801 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/statistics/eventually_follows/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:42.483519 pm4pyminimal-2.7.9.3/pm4py/statistics/eventually_follows/log/
--rw-rw-rw-   0        0        0      791 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/statistics/eventually_follows/log/__init__.py
--rw-rw-rw-   0        0        0     3015 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/statistics/eventually_follows/log/get.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:42.487508 pm4pyminimal-2.7.9.3/pm4py/statistics/eventually_follows/pandas/
--rw-rw-rw-   0        0        0      794 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/statistics/eventually_follows/pandas/__init__.py
--rw-rw-rw-   0        0        0     2879 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/statistics/eventually_follows/pandas/get.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:42.491817 pm4pyminimal-2.7.9.3/pm4py/statistics/eventually_follows/uvcl/
--rw-rw-rw-   0        0        0      792 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/statistics/eventually_follows/uvcl/__init__.py
--rw-rw-rw-   0        0        0     1936 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/statistics/eventually_follows/uvcl/get.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:42.509512 pm4pyminimal-2.7.9.3/pm4py/statistics/ocel/
--rw-rw-rw-   0        0        0      734 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/statistics/ocel/__init__.py
--rw-rw-rw-   0        0        0     3670 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/statistics/ocel/act_ot_dependent.py
--rw-rw-rw-   0        0        0     5684 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/statistics/ocel/act_utils.py
--rw-rw-rw-   0        0        0     9710 2024-01-02 13:29:21.000000 pm4pyminimal-2.7.9.3/pm4py/statistics/ocel/edge_metrics.py
--rw-rw-rw-   0        0        0     2361 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/statistics/ocel/objects_ot_count.py
--rw-rw-rw-   0        0        0     2395 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/statistics/ocel/ot_activities.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:42.511497 pm4pyminimal-2.7.9.3/pm4py/statistics/overlap/
--rw-rw-rw-   0        0        0      957 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/statistics/overlap/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:42.513491 pm4pyminimal-2.7.9.3/pm4py/statistics/overlap/cases/
--rw-rw-rw-   0        0        0      790 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/statistics/overlap/cases/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:42.516484 pm4pyminimal-2.7.9.3/pm4py/statistics/overlap/cases/log/
--rw-rw-rw-   0        0        0      786 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/statistics/overlap/cases/log/__init__.py
--rw-rw-rw-   0        0        0     2713 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/statistics/overlap/cases/log/get.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:42.520572 pm4pyminimal-2.7.9.3/pm4py/statistics/overlap/cases/pandas/
--rw-rw-rw-   0        0        0      789 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/statistics/overlap/cases/pandas/__init__.py
--rw-rw-rw-   0        0        0     3028 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/statistics/overlap/cases/pandas/get.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:42.521570 pm4pyminimal-2.7.9.3/pm4py/statistics/overlap/interval_events/
--rw-rw-rw-   0        0        0      800 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/statistics/overlap/interval_events/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:42.525558 pm4pyminimal-2.7.9.3/pm4py/statistics/overlap/interval_events/log/
--rw-rw-rw-   0        0        0      796 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/statistics/overlap/interval_events/log/__init__.py
--rw-rw-rw-   0        0        0     2767 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/statistics/overlap/interval_events/log/get.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:42.530662 pm4pyminimal-2.7.9.3/pm4py/statistics/overlap/interval_events/pandas/
--rw-rw-rw-   0        0        0      799 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/statistics/overlap/interval_events/pandas/__init__.py
--rw-rw-rw-   0        0        0     2570 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/statistics/overlap/interval_events/pandas/get.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:42.533654 pm4pyminimal-2.7.9.3/pm4py/statistics/overlap/utils/
--rw-rw-rw-   0        0        0      786 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/statistics/overlap/utils/__init__.py
--rw-rw-rw-   0        0        0     1986 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/statistics/overlap/utils/compute.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:42.535649 pm4pyminimal-2.7.9.3/pm4py/statistics/passed_time/
--rw-rw-rw-   0        0        0      790 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/statistics/passed_time/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:42.538745 pm4pyminimal-2.7.9.3/pm4py/statistics/passed_time/log/
--rw-rw-rw-   0        0        0      800 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/statistics/passed_time/log/__init__.py
--rw-rw-rw-   0        0        0     1781 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/statistics/passed_time/log/algorithm.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:42.547721 pm4pyminimal-2.7.9.3/pm4py/statistics/passed_time/log/variants/
--rw-rw-rw-   0        0        0      808 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/statistics/passed_time/log/variants/__init__.py
--rw-rw-rw-   0        0        0     2387 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/statistics/passed_time/log/variants/post.py
--rw-rw-rw-   0        0        0     2369 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/statistics/passed_time/log/variants/pre.py
--rw-rw-rw-   0        0        0     3050 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/statistics/passed_time/log/variants/prepost.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:42.552079 pm4pyminimal-2.7.9.3/pm4py/statistics/passed_time/pandas/
--rw-rw-rw-   0        0        0      803 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/statistics/passed_time/pandas/__init__.py
--rw-rw-rw-   0        0        0     1768 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/statistics/passed_time/pandas/algorithm.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:42.562053 pm4pyminimal-2.7.9.3/pm4py/statistics/passed_time/pandas/variants/
--rw-rw-rw-   0        0        0      811 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/statistics/passed_time/pandas/variants/__init__.py
--rw-rw-rw-   0        0        0     4131 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/statistics/passed_time/pandas/variants/post.py
--rw-rw-rw-   0        0        0     4235 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/statistics/passed_time/pandas/variants/pre.py
--rw-rw-rw-   0        0        0     4916 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/statistics/passed_time/pandas/variants/prepost.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:42.564118 pm4pyminimal-2.7.9.3/pm4py/statistics/rework/
--rw-rw-rw-   0        0        0      783 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/statistics/rework/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:42.567113 pm4pyminimal-2.7.9.3/pm4py/statistics/rework/cases/
--rw-rw-rw-   0        0        0      789 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/statistics/rework/cases/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:42.571228 pm4pyminimal-2.7.9.3/pm4py/statistics/rework/cases/log/
--rw-rw-rw-   0        0        0      785 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/statistics/rework/cases/log/__init__.py
--rw-rw-rw-   0        0        0     2597 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/statistics/rework/cases/log/get.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:42.576229 pm4pyminimal-2.7.9.3/pm4py/statistics/rework/cases/pandas/
--rw-rw-rw-   0        0        0      788 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/statistics/rework/cases/pandas/__init__.py
--rw-rw-rw-   0        0        0     2542 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/statistics/rework/cases/pandas/get.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:42.580334 pm4pyminimal-2.7.9.3/pm4py/statistics/rework/log/
--rw-rw-rw-   0        0        0      779 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/statistics/rework/log/__init__.py
--rw-rw-rw-   0        0        0     2265 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/statistics/rework/log/get.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:42.584951 pm4pyminimal-2.7.9.3/pm4py/statistics/rework/pandas/
--rw-rw-rw-   0        0        0      782 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/statistics/rework/pandas/__init__.py
--rw-rw-rw-   0        0        0     2378 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/statistics/rework/pandas/get.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:42.585948 pm4pyminimal-2.7.9.3/pm4py/statistics/service_time/
--rw-rw-rw-   0        0        0      789 2024-01-02 13:29:21.000000 pm4pyminimal-2.7.9.3/pm4py/statistics/service_time/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:42.590077 pm4pyminimal-2.7.9.3/pm4py/statistics/service_time/log/
--rw-rw-rw-   0        0        0      785 2024-01-02 13:29:21.000000 pm4pyminimal-2.7.9.3/pm4py/statistics/service_time/log/__init__.py
--rw-rw-rw-   0        0        0     5453 2024-01-02 13:29:21.000000 pm4pyminimal-2.7.9.3/pm4py/statistics/service_time/log/get.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:42.595063 pm4pyminimal-2.7.9.3/pm4py/statistics/service_time/pandas/
--rw-rw-rw-   0        0        0      788 2024-01-02 13:29:21.000000 pm4pyminimal-2.7.9.3/pm4py/statistics/service_time/pandas/__init__.py
--rw-rw-rw-   0        0        0     4930 2024-01-15 12:00:43.000000 pm4pyminimal-2.7.9.3/pm4py/statistics/service_time/pandas/get.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:42.598055 pm4pyminimal-2.7.9.3/pm4py/statistics/sojourn_time/
--rw-rw-rw-   0        0        0      779 2024-01-02 13:29:21.000000 pm4pyminimal-2.7.9.3/pm4py/statistics/sojourn_time/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:42.600050 pm4pyminimal-2.7.9.3/pm4py/statistics/start_activities/
--rw-rw-rw-   0        0        0      801 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/statistics/start_activities/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:42.604039 pm4pyminimal-2.7.9.3/pm4py/statistics/start_activities/common/
--rw-rw-rw-   0        0        0      792 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/statistics/start_activities/common/__init__.py
--rw-rw-rw-   0        0        0     1813 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/statistics/start_activities/common/get.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:42.608031 pm4pyminimal-2.7.9.3/pm4py/statistics/start_activities/log/
--rw-rw-rw-   0        0        0      789 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/statistics/start_activities/log/__init__.py
--rw-rw-rw-   0        0        0     2769 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/statistics/start_activities/log/get.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:42.614573 pm4pyminimal-2.7.9.3/pm4py/statistics/start_activities/pandas/
--rw-rw-rw-   0        0        0      792 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/statistics/start_activities/pandas/__init__.py
--rw-rw-rw-   0        0        0     2623 2024-01-15 12:00:43.000000 pm4pyminimal-2.7.9.3/pm4py/statistics/start_activities/pandas/get.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:42.616566 pm4pyminimal-2.7.9.3/pm4py/statistics/traces/
--rw-rw-rw-   0        0        0      791 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/statistics/traces/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:42.618673 pm4pyminimal-2.7.9.3/pm4py/statistics/traces/cycle_time/
--rw-rw-rw-   0        0        0      800 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/statistics/traces/cycle_time/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:42.622661 pm4pyminimal-2.7.9.3/pm4py/statistics/traces/cycle_time/log/
--rw-rw-rw-   0        0        0      790 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/statistics/traces/cycle_time/log/__init__.py
--rw-rw-rw-   0        0        0     3191 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/statistics/traces/cycle_time/log/get.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:42.626654 pm4pyminimal-2.7.9.3/pm4py/statistics/traces/cycle_time/pandas/
--rw-rw-rw-   0        0        0      793 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/statistics/traces/cycle_time/pandas/__init__.py
--rw-rw-rw-   0        0        0     3255 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/statistics/traces/cycle_time/pandas/get.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:42.630743 pm4pyminimal-2.7.9.3/pm4py/statistics/traces/cycle_time/util/
--rw-rw-rw-   0        0        0      795 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/statistics/traces/cycle_time/util/__init__.py
--rw-rw-rw-   0        0        0     2385 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/statistics/traces/cycle_time/util/compute.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:42.632737 pm4pyminimal-2.7.9.3/pm4py/statistics/traces/generic/
--rw-rw-rw-   0        0        0      799 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/statistics/traces/generic/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:42.635729 pm4pyminimal-2.7.9.3/pm4py/statistics/traces/generic/common/
--rw-rw-rw-   0        0        0      800 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/statistics/traces/generic/common/__init__.py
--rw-rw-rw-   0        0        0     2969 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/statistics/traces/generic/common/case_duration.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:42.640834 pm4pyminimal-2.7.9.3/pm4py/statistics/traces/generic/log/
--rw-rw-rw-   0        0        0      799 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/statistics/traces/generic/log/__init__.py
--rw-rw-rw-   0        0        0     5237 2024-01-02 13:29:21.000000 pm4pyminimal-2.7.9.3/pm4py/statistics/traces/generic/log/case_arrival.py
--rw-rw-rw-   0        0        0    13221 2024-01-02 13:29:21.000000 pm4pyminimal-2.7.9.3/pm4py/statistics/traces/generic/log/case_statistics.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:42.646818 pm4pyminimal-2.7.9.3/pm4py/statistics/traces/generic/pandas/
--rw-rw-rw-   0        0        0      799 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/statistics/traces/generic/pandas/__init__.py
--rw-rw-rw-   0        0        0     4223 2024-01-15 12:00:43.000000 pm4pyminimal-2.7.9.3/pm4py/statistics/traces/generic/pandas/case_arrival.py
--rw-rw-rw-   0        0        0    16954 2024-01-15 12:00:43.000000 pm4pyminimal-2.7.9.3/pm4py/statistics/traces/generic/pandas/case_statistics.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:42.650918 pm4pyminimal-2.7.9.3/pm4py/statistics/util/
--rw-rw-rw-   0        0        0      974 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/statistics/util/__init__.py
--rw-rw-rw-   0        0        0     2382 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/statistics/util/times_bipartite_matching.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:42.651914 pm4pyminimal-2.7.9.3/pm4py/statistics/variants/
--rw-rw-rw-   0        0        0      785 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/statistics/variants/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:42.655904 pm4pyminimal-2.7.9.3/pm4py/statistics/variants/log/
--rw-rw-rw-   0        0        0      781 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/statistics/variants/log/__init__.py
--rw-rw-rw-   0        0        0     7359 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/statistics/variants/log/get.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:42.658898 pm4pyminimal-2.7.9.3/pm4py/statistics/variants/pandas/
--rw-rw-rw-   0        0        0      784 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/statistics/variants/pandas/__init__.py
--rw-rw-rw-   0        0        0     2254 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/statistics/variants/pandas/get.py
--rw-rw-rw-   0        0        0    39292 2024-01-15 12:00:43.000000 pm4pyminimal-2.7.9.3/pm4py/stats.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:42.662270 pm4pyminimal-2.7.9.3/pm4py/streaming/
--rw-rw-rw-   0        0        0      804 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/streaming/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:42.668253 pm4pyminimal-2.7.9.3/pm4py/streaming/algo/
--rw-rw-rw-   0        0        0      800 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/streaming/algo/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:42.670347 pm4pyminimal-2.7.9.3/pm4py/streaming/algo/conformance/
--rw-rw-rw-   0        0        0      806 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/streaming/algo/conformance/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:42.676332 pm4pyminimal-2.7.9.3/pm4py/streaming/algo/conformance/footprints/
--rw-rw-rw-   0        0        0      811 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/streaming/algo/conformance/footprints/__init__.py
--rw-rw-rw-   0        0        0     1515 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/streaming/algo/conformance/footprints/algorithm.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:42.681571 pm4pyminimal-2.7.9.3/pm4py/streaming/algo/conformance/footprints/variants/
--rw-rw-rw-   0        0        0      808 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/streaming/algo/conformance/footprints/variants/__init__.py
--rw-rw-rw-   0        0        0    11003 2024-01-02 13:29:21.000000 pm4pyminimal-2.7.9.3/pm4py/streaming/algo/conformance/footprints/variants/classic.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:42.685560 pm4pyminimal-2.7.9.3/pm4py/streaming/algo/conformance/tbr/
--rw-rw-rw-   0        0        0      804 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/streaming/algo/conformance/tbr/__init__.py
--rw-rw-rw-   0        0        0     1523 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/streaming/algo/conformance/tbr/algorithm.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:42.689550 pm4pyminimal-2.7.9.3/pm4py/streaming/algo/conformance/tbr/variants/
--rw-rw-rw-   0        0        0      801 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/streaming/algo/conformance/tbr/variants/__init__.py
--rw-rw-rw-   0        0        0    17271 2024-01-02 13:29:21.000000 pm4pyminimal-2.7.9.3/pm4py/streaming/algo/conformance/tbr/variants/classic.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:42.695925 pm4pyminimal-2.7.9.3/pm4py/streaming/algo/conformance/temporal/
--rw-rw-rw-   0        0        0      809 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/streaming/algo/conformance/temporal/__init__.py
--rw-rw-rw-   0        0        0     2135 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/streaming/algo/conformance/temporal/algorithm.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:42.699913 pm4pyminimal-2.7.9.3/pm4py/streaming/algo/conformance/temporal/variants/
--rw-rw-rw-   0        0        0      806 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/streaming/algo/conformance/temporal/variants/__init__.py
--rw-rw-rw-   0        0        0     9602 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/streaming/algo/conformance/temporal/variants/classic.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:42.701907 pm4pyminimal-2.7.9.3/pm4py/streaming/algo/discovery/
--rw-rw-rw-   0        0        0      782 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/streaming/algo/discovery/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:42.706895 pm4pyminimal-2.7.9.3/pm4py/streaming/algo/discovery/dfg/
--rw-rw-rw-   0        0        0      802 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/streaming/algo/discovery/dfg/__init__.py
--rw-rw-rw-   0        0        0     1411 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/streaming/algo/discovery/dfg/algorithm.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:42.712527 pm4pyminimal-2.7.9.3/pm4py/streaming/algo/discovery/dfg/variants/
--rw-rw-rw-   0        0        0      801 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/streaming/algo/discovery/dfg/variants/__init__.py
--rw-rw-rw-   0        0        0     7371 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/streaming/algo/discovery/dfg/variants/frequency.py
--rw-rw-rw-   0        0        0     1476 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/streaming/algo/interface.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:42.719508 pm4pyminimal-2.7.9.3/pm4py/streaming/conversion/
--rw-rw-rw-   0        0        0     1468 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/streaming/conversion/__init__.py
--rw-rw-rw-   0        0        0     4925 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/streaming/conversion/from_pandas.py
--rw-rw-rw-   0        0        0     5211 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/streaming/conversion/ocel_flatts_distributor.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:42.721180 pm4pyminimal-2.7.9.3/pm4py/streaming/importer/
--rw-rw-rw-   0        0        0      885 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/streaming/importer/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:42.726167 pm4pyminimal-2.7.9.3/pm4py/streaming/importer/csv/
--rw-rw-rw-   0        0        0      795 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/streaming/importer/csv/__init__.py
--rw-rw-rw-   0        0        0     1488 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/streaming/importer/csv/importer.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:42.731464 pm4pyminimal-2.7.9.3/pm4py/streaming/importer/csv/variants/
--rw-rw-rw-   0        0        0      802 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/streaming/importer/csv/variants/__init__.py
--rw-rw-rw-   0        0        0     3406 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/streaming/importer/csv/variants/csv_event_stream.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:42.734456 pm4pyminimal-2.7.9.3/pm4py/streaming/importer/xes/
--rw-rw-rw-   0        0        0      795 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/streaming/importer/xes/__init__.py
--rw-rw-rw-   0        0        0     1523 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/streaming/importer/xes/importer.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:42.739544 pm4pyminimal-2.7.9.3/pm4py/streaming/importer/xes/variants/
--rw-rw-rw-   0        0        0      820 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/streaming/importer/xes/variants/__init__.py
--rw-rw-rw-   0        0        0     9461 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/streaming/importer/xes/variants/xes_event_stream.py
--rw-rw-rw-   0        0        0     9317 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/streaming/importer/xes/variants/xes_trace_stream.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:42.746526 pm4pyminimal-2.7.9.3/pm4py/streaming/stream/
--rw-rw-rw-   0        0        0      807 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/streaming/stream/__init__.py
--rw-rw-rw-   0        0        0     3109 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/streaming/stream/live_event_stream.py
--rw-rw-rw-   0        0        0     3109 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/streaming/stream/live_trace_stream.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:42.756738 pm4pyminimal-2.7.9.3/pm4py/streaming/util/
--rw-rw-rw-   0        0        0      819 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/streaming/util/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:42.760173 pm4pyminimal-2.7.9.3/pm4py/streaming/util/dictio/
--rw-rw-rw-   0        0        0      795 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/streaming/util/dictio/__init__.py
--rw-rw-rw-   0        0        0     1461 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/streaming/util/dictio/generator.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:42.767153 pm4pyminimal-2.7.9.3/pm4py/streaming/util/dictio/versions/
--rw-rw-rw-   0        0        0      805 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/streaming/util/dictio/versions/__init__.py
--rw-rw-rw-   0        0        0      941 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/streaming/util/dictio/versions/classic.py
--rw-rw-rw-   0        0        0     3540 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/streaming/util/dictio/versions/redis.py
--rw-rw-rw-   0        0        0     1949 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/streaming/util/dictio/versions/thread_safe.py
--rw-rw-rw-   0        0        0     1039 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/streaming/util/event_stream_printer.py
--rw-rw-rw-   0        0        0     1180 2024-01-04 10:14:42.000000 pm4pyminimal-2.7.9.3/pm4py/streaming/util/live_to_static_stream.py
--rw-rw-rw-   0        0        0     1039 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/streaming/util/trace_stream_printer.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:42.797528 pm4pyminimal-2.7.9.3/pm4py/util/
--rw-rw-rw-   0        0        0      918 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/util/__init__.py
--rw-rw-rw-   0        0        0     5056 2024-01-02 13:29:21.000000 pm4pyminimal-2.7.9.3/pm4py/util/business_hours.py
--rw-rw-rw-   0        0        0     2225 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/util/colors.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:42.804510 pm4pyminimal-2.7.9.3/pm4py/util/compression/
--rw-rw-rw-   0        0        0      781 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/util/compression/__init__.py
--rw-rw-rw-   0        0        0     1314 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/util/compression/dtypes.py
--rw-rw-rw-   0        0        0    11522 2024-01-02 13:29:21.000000 pm4pyminimal-2.7.9.3/pm4py/util/compression/util.py
--rw-rw-rw-   0        0        0     7079 2024-01-02 13:29:21.000000 pm4pyminimal-2.7.9.3/pm4py/util/constants.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:42.809497 pm4pyminimal-2.7.9.3/pm4py/util/dt_parsing/
--rw-rw-rw-   0        0        0      786 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/util/dt_parsing/__init__.py
--rw-rw-rw-   0        0        0     2682 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/util/dt_parsing/parser.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:42.823349 pm4pyminimal-2.7.9.3/pm4py/util/dt_parsing/variants/
--rw-rw-rw-   0        0        0      734 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/util/dt_parsing/variants/__init__.py
--rw-rw-rw-   0        0        0     1029 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/util/dt_parsing/variants/cs8601.py
--rw-rw-rw-   0        0        0     1470 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/util/dt_parsing/variants/dummy.py
--rw-rw-rw-   0        0        0     1916 2024-01-02 13:29:21.000000 pm4pyminimal-2.7.9.3/pm4py/util/dt_parsing/variants/strpfromiso.py
--rw-rw-rw-   0        0        0     1564 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/util/exec_utils.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:42.829613 pm4pyminimal-2.7.9.3/pm4py/util/lp/
--rw-rw-rw-   0        0        0      784 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/util/lp/__init__.py
--rw-rw-rw-   0        0        0     5457 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/util/lp/solver.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:42.831609 pm4pyminimal-2.7.9.3/pm4py/util/lp/util/
--rw-rw-rw-   0        0        0      734 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/util/lp/util/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:42.849583 pm4pyminimal-2.7.9.3/pm4py/util/lp/variants/
--rw-rw-rw-   0        0        0      943 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/util/lp/variants/__init__.py
--rw-rw-rw-   0        0        0     3639 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/util/lp/variants/cvxopt_solver.py
--rw-rw-rw-   0        0        0     3420 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/util/lp/variants/cvxopt_solver_custom_align.py
--rw-rw-rw-   0        0        0     3059 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/util/lp/variants/cvxopt_solver_custom_align_arm.py
--rw-rw-rw-   0        0        0     3937 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/util/lp/variants/cvxopt_solver_custom_align_ilp.py
--rw-rw-rw-   0        0        0     5153 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/util/lp/variants/ortools_solver.py
--rw-rw-rw-   0        0        0     6293 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/util/lp/variants/pulp_solver.py
--rw-rw-rw-   0        0        0     1853 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/util/lp/variants/scipy_solver.py
--rw-rw-rw-   0        0        0     9895 2024-01-02 13:29:21.000000 pm4pyminimal-2.7.9.3/pm4py/util/nx_utils.py
--rw-rw-rw-   0        0        0    13899 2024-01-15 12:00:43.000000 pm4pyminimal-2.7.9.3/pm4py/util/pandas_utils.py
--rw-rw-rw-   0        0        0     1494 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/util/points_subset.py
--rw-rw-rw-   0        0        0     1602 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/util/regex.py
--rw-rw-rw-   0        0        0     3663 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/util/string_distance.py
--rw-rw-rw-   0        0        0     1095 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/util/typing.py
--rw-rw-rw-   0        0        0     2261 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/util/variants_util.py
--rw-rw-rw-   0        0        0     6027 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/util/vis_utils.py
--rw-rw-rw-   0        0        0     1614 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/util/xes_constants.py
--rw-rw-rw-   0        0        0    25437 2024-01-15 12:00:43.000000 pm4pyminimal-2.7.9.3/pm4py/utils.py
--rw-rw-rw-   0        0        0    69901 2024-01-02 13:29:21.000000 pm4pyminimal-2.7.9.3/pm4py/vis.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:42.851579 pm4pyminimal-2.7.9.3/pm4py/visualization/
--rw-rw-rw-   0        0        0     1869 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/visualization/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:42.855569 pm4pyminimal-2.7.9.3/pm4py/visualization/align_table/
--rw-rw-rw-   0        0        0      790 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/visualization/align_table/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:42.859758 pm4pyminimal-2.7.9.3/pm4py/visualization/align_table/variants/
--rw-rw-rw-   0        0        0      796 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/visualization/align_table/variants/__init__.py
--rw-rw-rw-   0        0        0     3863 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/visualization/align_table/variants/classic.py
--rw-rw-rw-   0        0        0     2968 2024-01-02 13:29:21.000000 pm4pyminimal-2.7.9.3/pm4py/visualization/align_table/visualizer.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:42.863745 pm4pyminimal-2.7.9.3/pm4py/visualization/bpmn/
--rw-rw-rw-   0        0        0      793 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/visualization/bpmn/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:42.866737 pm4pyminimal-2.7.9.3/pm4py/visualization/bpmn/variants/
--rw-rw-rw-   0        0        0      789 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/visualization/bpmn/variants/__init__.py
--rw-rw-rw-   0        0        0     3654 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/visualization/bpmn/variants/classic.py
--rw-rw-rw-   0        0        0     2583 2024-01-02 13:29:21.000000 pm4pyminimal-2.7.9.3/pm4py/visualization/bpmn/visualizer.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:42.886948 pm4pyminimal-2.7.9.3/pm4py/visualization/common/
--rw-rw-rw-   0        0        0      817 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/visualization/common/__init__.py
--rw-rw-rw-   0        0        0     1160 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/visualization/common/dot_util.py
--rw-rw-rw-   0        0        0     3058 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/visualization/common/gview.py
--rw-rw-rw-   0        0        0     3394 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/visualization/common/html.py
--rw-rw-rw-   0        0        0     1531 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/visualization/common/save.py
--rw-rw-rw-   0        0        0     2526 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/visualization/common/svg_pos_parser.py
--rw-rw-rw-   0        0        0      879 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/visualization/common/utils.py
--rw-rw-rw-   0        0        0     1540 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/visualization/common/visualizer.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:42.892059 pm4pyminimal-2.7.9.3/pm4py/visualization/decisiontree/
--rw-rw-rw-   0        0        0     1008 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/visualization/decisiontree/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:42.897045 pm4pyminimal-2.7.9.3/pm4py/visualization/decisiontree/util/
--rw-rw-rw-   0        0        0      734 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/visualization/decisiontree/util/__init__.py
--rw-rw-rw-   0        0        0     2621 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/visualization/decisiontree/util/dt_to_string.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:42.901148 pm4pyminimal-2.7.9.3/pm4py/visualization/decisiontree/variants/
--rw-rw-rw-   0        0        0      797 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/visualization/decisiontree/variants/__init__.py
--rw-rw-rw-   0        0        0     2231 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/visualization/decisiontree/variants/classic.py
--rw-rw-rw-   0        0        0     2840 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/visualization/decisiontree/visualizer.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:42.906135 pm4pyminimal-2.7.9.3/pm4py/visualization/dfg/
--rw-rw-rw-   0        0        0      800 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/visualization/dfg/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:42.911466 pm4pyminimal-2.7.9.3/pm4py/visualization/dfg/util/
--rw-rw-rw-   0        0        0      787 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/visualization/dfg/util/__init__.py
--rw-rw-rw-   0        0        0     8994 2024-01-02 13:29:21.000000 pm4pyminimal-2.7.9.3/pm4py/visualization/dfg/util/dfg_gviz.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:42.923636 pm4pyminimal-2.7.9.3/pm4py/visualization/dfg/variants/
--rw-rw-rw-   0        0        0      803 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/visualization/dfg/variants/__init__.py
--rw-rw-rw-   0        0        0     5409 2024-01-02 13:29:21.000000 pm4pyminimal-2.7.9.3/pm4py/visualization/dfg/variants/cost.py
--rw-rw-rw-   0        0        0     5157 2024-01-02 13:29:21.000000 pm4pyminimal-2.7.9.3/pm4py/visualization/dfg/variants/frequency.py
--rw-rw-rw-   0        0        0     5580 2024-01-02 13:29:21.000000 pm4pyminimal-2.7.9.3/pm4py/visualization/dfg/variants/performance.py
--rw-rw-rw-   0        0        0    12854 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/visualization/dfg/variants/timeline.py
--rw-rw-rw-   0        0        0     3196 2024-01-02 13:29:21.000000 pm4pyminimal-2.7.9.3/pm4py/visualization/dfg/visualizer.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:42.928888 pm4pyminimal-2.7.9.3/pm4py/visualization/dotted_chart/
--rw-rw-rw-   0        0        0      801 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/visualization/dotted_chart/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:42.933874 pm4pyminimal-2.7.9.3/pm4py/visualization/dotted_chart/variants/
--rw-rw-rw-   0        0        0      797 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/visualization/dotted_chart/variants/__init__.py
--rw-rw-rw-   0        0        0     9236 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/visualization/dotted_chart/variants/classic.py
--rw-rw-rw-   0        0        0     3819 2024-01-02 13:29:21.000000 pm4pyminimal-2.7.9.3/pm4py/visualization/dotted_chart/visualizer.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:42.937863 pm4pyminimal-2.7.9.3/pm4py/visualization/footprints/
--rw-rw-rw-   0        0        0      799 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/visualization/footprints/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:42.946092 pm4pyminimal-2.7.9.3/pm4py/visualization/footprints/variants/
--rw-rw-rw-   0        0        0      828 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/visualization/footprints/variants/__init__.py
--rw-rw-rw-   0        0        0     3842 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/visualization/footprints/variants/comparison.py
--rw-rw-rw-   0        0        0     4374 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/visualization/footprints/variants/comparison_symmetric.py
--rw-rw-rw-   0        0        0     3280 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/visualization/footprints/variants/single.py
--rw-rw-rw-   0        0        0     3120 2024-01-02 13:29:21.000000 pm4pyminimal-2.7.9.3/pm4py/visualization/footprints/visualizer.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:42.950230 pm4pyminimal-2.7.9.3/pm4py/visualization/graphs/
--rw-rw-rw-   0        0        0      801 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/visualization/graphs/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:42.954222 pm4pyminimal-2.7.9.3/pm4py/visualization/graphs/util/
--rw-rw-rw-   0        0        0      786 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/visualization/graphs/util/__init__.py
--rw-rw-rw-   0        0        0     2849 2024-01-02 13:29:21.000000 pm4pyminimal-2.7.9.3/pm4py/visualization/graphs/util/common.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:42.964337 pm4pyminimal-2.7.9.3/pm4py/visualization/graphs/variants/
--rw-rw-rw-   0        0        0      817 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/visualization/graphs/variants/__init__.py
--rw-rw-rw-   0        0        0     4541 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/visualization/graphs/variants/attributes.py
--rw-rw-rw-   0        0        0     2763 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/visualization/graphs/variants/barplot.py
--rw-rw-rw-   0        0        0     4542 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/visualization/graphs/variants/cases.py
--rw-rw-rw-   0        0        0     4587 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/visualization/graphs/variants/dates.py
--rw-rw-rw-   0        0        0     3859 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/visualization/graphs/visualizer.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:42.967330 pm4pyminimal-2.7.9.3/pm4py/visualization/heuristics_net/
--rw-rw-rw-   0        0        0      803 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/visualization/heuristics_net/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:42.971433 pm4pyminimal-2.7.9.3/pm4py/visualization/heuristics_net/variants/
--rw-rw-rw-   0        0        0      805 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/visualization/heuristics_net/variants/__init__.py
--rw-rw-rw-   0        0        0    13357 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/visualization/heuristics_net/variants/pydotplus_vis.py
--rw-rw-rw-   0        0        0     4471 2024-01-02 13:29:21.000000 pm4pyminimal-2.7.9.3/pm4py/visualization/heuristics_net/visualizer.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:42.975427 pm4pyminimal-2.7.9.3/pm4py/visualization/network_analysis/
--rw-rw-rw-   0        0        0      805 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/visualization/network_analysis/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:42.982739 pm4pyminimal-2.7.9.3/pm4py/visualization/network_analysis/variants/
--rw-rw-rw-   0        0        0      816 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/visualization/network_analysis/variants/__init__.py
--rw-rw-rw-   0        0        0     4975 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/visualization/network_analysis/variants/frequency.py
--rw-rw-rw-   0        0        0     6154 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/visualization/network_analysis/variants/performance.py
--rw-rw-rw-   0        0        0     2496 2024-01-02 13:29:21.000000 pm4pyminimal-2.7.9.3/pm4py/visualization/network_analysis/visualizer.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:42.986729 pm4pyminimal-2.7.9.3/pm4py/visualization/networkx/
--rw-rw-rw-   0        0        0      734 2024-01-02 13:29:21.000000 pm4pyminimal-2.7.9.3/pm4py/visualization/networkx/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:42.990813 pm4pyminimal-2.7.9.3/pm4py/visualization/networkx/variants/
--rw-rw-rw-   0        0        0      734 2024-01-02 13:29:21.000000 pm4pyminimal-2.7.9.3/pm4py/visualization/networkx/variants/__init__.py
--rw-rw-rw-   0        0        0     3990 2024-01-02 13:29:21.000000 pm4pyminimal-2.7.9.3/pm4py/visualization/networkx/variants/digraph.py
--rw-rw-rw-   0        0        0     2362 2024-01-02 13:29:21.000000 pm4pyminimal-2.7.9.3/pm4py/visualization/networkx/visualizer.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:42.993806 pm4pyminimal-2.7.9.3/pm4py/visualization/ocel/
--rw-rw-rw-   0        0        0      813 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/visualization/ocel/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:42.999573 pm4pyminimal-2.7.9.3/pm4py/visualization/ocel/eve_to_obj_types/
--rw-rw-rw-   0        0        0      734 2024-01-02 13:29:21.000000 pm4pyminimal-2.7.9.3/pm4py/visualization/ocel/eve_to_obj_types/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:43.003562 pm4pyminimal-2.7.9.3/pm4py/visualization/ocel/eve_to_obj_types/variants/
--rw-rw-rw-   0        0        0      734 2024-01-02 13:29:21.000000 pm4pyminimal-2.7.9.3/pm4py/visualization/ocel/eve_to_obj_types/variants/__init__.py
--rw-rw-rw-   0        0        0     3613 2024-01-02 13:29:21.000000 pm4pyminimal-2.7.9.3/pm4py/visualization/ocel/eve_to_obj_types/variants/graphviz.py
--rw-rw-rw-   0        0        0     2724 2024-01-02 13:29:21.000000 pm4pyminimal-2.7.9.3/pm4py/visualization/ocel/eve_to_obj_types/visualizer.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:43.007551 pm4pyminimal-2.7.9.3/pm4py/visualization/ocel/interleavings/
--rw-rw-rw-   0        0        0      807 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/visualization/ocel/interleavings/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:43.013652 pm4pyminimal-2.7.9.3/pm4py/visualization/ocel/interleavings/variants/
--rw-rw-rw-   0        0        0      804 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/visualization/ocel/interleavings/variants/__init__.py
--rw-rw-rw-   0        0        0    15031 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/visualization/ocel/interleavings/variants/graphviz.py
--rw-rw-rw-   0        0        0     2989 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/visualization/ocel/interleavings/visualizer.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:43.017642 pm4pyminimal-2.7.9.3/pm4py/visualization/ocel/object_graph/
--rw-rw-rw-   0        0        0      734 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/visualization/ocel/object_graph/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:43.021790 pm4pyminimal-2.7.9.3/pm4py/visualization/ocel/object_graph/variants/
--rw-rw-rw-   0        0        0      734 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/visualization/ocel/object_graph/variants/__init__.py
--rw-rw-rw-   0        0        0     3447 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/visualization/ocel/object_graph/variants/graphviz.py
--rw-rw-rw-   0        0        0     2556 2024-01-02 13:29:21.000000 pm4pyminimal-2.7.9.3/pm4py/visualization/ocel/object_graph/visualizer.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:43.027775 pm4pyminimal-2.7.9.3/pm4py/visualization/ocel/ocdfg/
--rw-rw-rw-   0        0        0      799 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/visualization/ocel/ocdfg/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:43.031919 pm4pyminimal-2.7.9.3/pm4py/visualization/ocel/ocdfg/variants/
--rw-rw-rw-   0        0        0      795 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/visualization/ocel/ocdfg/variants/__init__.py
--rw-rw-rw-   0        0        0    12507 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/visualization/ocel/ocdfg/variants/classic.py
--rw-rw-rw-   0        0        0     2454 2024-01-02 13:29:21.000000 pm4pyminimal-2.7.9.3/pm4py/visualization/ocel/ocdfg/visualizer.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:43.035909 pm4pyminimal-2.7.9.3/pm4py/visualization/ocel/ocpn/
--rw-rw-rw-   0        0        0      798 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/visualization/ocel/ocpn/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:43.039138 pm4pyminimal-2.7.9.3/pm4py/visualization/ocel/ocpn/variants/
--rw-rw-rw-   0        0        0      800 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/visualization/ocel/ocpn/variants/__init__.py
--rw-rw-rw-   0        0        0     5941 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/visualization/ocel/ocpn/variants/wo_decoration.py
--rw-rw-rw-   0        0        0     2601 2024-01-02 13:29:21.000000 pm4pyminimal-2.7.9.3/pm4py/visualization/ocel/ocpn/visualizer.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:43.044125 pm4pyminimal-2.7.9.3/pm4py/visualization/performance_spectrum/
--rw-rw-rw-   0        0        0      809 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/visualization/performance_spectrum/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:43.047118 pm4pyminimal-2.7.9.3/pm4py/visualization/performance_spectrum/variants/
--rw-rw-rw-   0        0        0      803 2023-12-11 09:33:53.000000 pm4pyminimal-2.7.9.3/pm4py/visualization/performance_spectrum/variants/__init__.py
--rw-rw-rw-   0        0        0     7116 2024-01-02 13:29:21.000000 pm4pyminimal-2.7.9.3/pm4py/visualization/performance_spectrum/variants/neato.py
--rw-rw-rw-   0        0        0     3244 2024-01-02 13:29:21.000000 pm4pyminimal-2.7.9.3/pm4py/visualization/performance_spectrum/visualizer.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:43.054434 pm4pyminimal-2.7.9.3/pm4py/visualization/petri_net/
--rw-rw-rw-   0        0        0      812 2023-12-11 09:33:54.000000 pm4pyminimal-2.7.9.3/pm4py/visualization/petri_net/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:43.058431 pm4pyminimal-2.7.9.3/pm4py/visualization/petri_net/common/
--rw-rw-rw-   0        0        0      794 2023-12-11 09:33:54.000000 pm4pyminimal-2.7.9.3/pm4py/visualization/petri_net/common/__init__.py
--rw-rw-rw-   0        0        0     9446 2023-12-11 09:33:54.000000 pm4pyminimal-2.7.9.3/pm4py/visualization/petri_net/common/visualize.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:43.064888 pm4pyminimal-2.7.9.3/pm4py/visualization/petri_net/util/
--rw-rw-rw-   0        0        0      847 2023-12-11 09:33:54.000000 pm4pyminimal-2.7.9.3/pm4py/visualization/petri_net/util/__init__.py
--rw-rw-rw-   0        0        0     2935 2023-12-11 09:33:54.000000 pm4pyminimal-2.7.9.3/pm4py/visualization/petri_net/util/alignments_decoration.py
--rw-rw-rw-   0        0        0     1121 2023-12-11 09:33:54.000000 pm4pyminimal-2.7.9.3/pm4py/visualization/petri_net/util/performance_map.py
--rw-rw-rw-   0        0        0    11279 2023-12-11 09:33:54.000000 pm4pyminimal-2.7.9.3/pm4py/visualization/petri_net/util/vis_trans_shortest_paths.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:43.079412 pm4pyminimal-2.7.9.3/pm4py/visualization/petri_net/variants/
--rw-rw-rw-   0        0        0      937 2023-12-11 09:33:54.000000 pm4pyminimal-2.7.9.3/pm4py/visualization/petri_net/variants/__init__.py
--rw-rw-rw-   0        0        0     2044 2023-12-11 09:33:54.000000 pm4pyminimal-2.7.9.3/pm4py/visualization/petri_net/variants/alignments.py
--rw-rw-rw-   0        0        0     4730 2023-12-11 09:33:54.000000 pm4pyminimal-2.7.9.3/pm4py/visualization/petri_net/variants/greedy_decoration_frequency.py
--rw-rw-rw-   0        0        0     4837 2023-12-11 09:33:54.000000 pm4pyminimal-2.7.9.3/pm4py/visualization/petri_net/variants/greedy_decoration_performance.py
--rw-rw-rw-   0        0        0     5670 2023-12-11 09:33:54.000000 pm4pyminimal-2.7.9.3/pm4py/visualization/petri_net/variants/token_decoration_frequency.py
--rw-rw-rw-   0        0        0     5880 2023-12-11 09:33:54.000000 pm4pyminimal-2.7.9.3/pm4py/visualization/petri_net/variants/token_decoration_performance.py
--rw-rw-rw-   0        0        0     2237 2023-12-11 09:33:54.000000 pm4pyminimal-2.7.9.3/pm4py/visualization/petri_net/variants/wo_decoration.py
--rw-rw-rw-   0        0        0     3651 2024-01-02 13:29:21.000000 pm4pyminimal-2.7.9.3/pm4py/visualization/petri_net/visualizer.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:43.082404 pm4pyminimal-2.7.9.3/pm4py/visualization/powl/
--rw-rw-rw-   0        0        0      795 2023-12-11 09:33:54.000000 pm4pyminimal-2.7.9.3/pm4py/visualization/powl/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:43.098503 pm4pyminimal-2.7.9.3/pm4py/visualization/powl/variants/
--rw-rw-rw-   0        0        0      785 2023-12-11 09:33:54.000000 pm4pyminimal-2.7.9.3/pm4py/visualization/powl/variants/__init__.py
--rw-rw-rw-   0        0        0     7745 2024-01-02 13:29:21.000000 pm4pyminimal-2.7.9.3/pm4py/visualization/powl/variants/basic.py
--rw-rw-rw-   0        0        0      755 2024-01-02 13:29:21.000000 pm4pyminimal-2.7.9.3/pm4py/visualization/powl/variants/end.png
--rw-rw-rw-   0        0        0    25337 2024-01-02 13:29:21.000000 pm4pyminimal-2.7.9.3/pm4py/visualization/powl/variants/loop.png
--rw-rw-rw-   0        0        0    11069 2024-01-02 13:29:21.000000 pm4pyminimal-2.7.9.3/pm4py/visualization/powl/variants/net.py
--rw-rw-rw-   0        0        0      922 2024-01-02 13:29:21.000000 pm4pyminimal-2.7.9.3/pm4py/visualization/powl/variants/play.png
--rw-rw-rw-   0        0        0    78865 2024-01-02 13:29:21.000000 pm4pyminimal-2.7.9.3/pm4py/visualization/powl/variants/xor.png
--rw-rw-rw-   0        0        0     2853 2024-01-02 13:29:21.000000 pm4pyminimal-2.7.9.3/pm4py/visualization/powl/visualizer.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:43.103606 pm4pyminimal-2.7.9.3/pm4py/visualization/process_tree/
--rw-rw-rw-   0        0        0      801 2023-12-11 09:33:54.000000 pm4pyminimal-2.7.9.3/pm4py/visualization/process_tree/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:43.112269 pm4pyminimal-2.7.9.3/pm4py/visualization/process_tree/variants/
--rw-rw-rw-   0        0        0      813 2023-12-11 09:33:54.000000 pm4pyminimal-2.7.9.3/pm4py/visualization/process_tree/variants/__init__.py
--rw-rw-rw-   0        0        0     4873 2023-12-11 09:33:54.000000 pm4pyminimal-2.7.9.3/pm4py/visualization/process_tree/variants/frequency_annotation.py
--rw-rw-rw-   0        0        0     4104 2023-12-11 09:33:54.000000 pm4pyminimal-2.7.9.3/pm4py/visualization/process_tree/variants/symbolic.py
--rw-rw-rw-   0        0        0     4256 2023-12-11 09:33:54.000000 pm4pyminimal-2.7.9.3/pm4py/visualization/process_tree/variants/wo_decoration.py
--rw-rw-rw-   0        0        0     3017 2024-01-02 13:29:21.000000 pm4pyminimal-2.7.9.3/pm4py/visualization/process_tree/visualizer.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:43.116254 pm4pyminimal-2.7.9.3/pm4py/visualization/sna/
--rw-rw-rw-   0        0        0      792 2023-12-11 09:33:54.000000 pm4pyminimal-2.7.9.3/pm4py/visualization/sna/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:43.123901 pm4pyminimal-2.7.9.3/pm4py/visualization/sna/variants/
--rw-rw-rw-   0        0        0      796 2023-12-11 09:33:54.000000 pm4pyminimal-2.7.9.3/pm4py/visualization/sna/variants/__init__.py
--rw-rw-rw-   0        0        0     4180 2023-12-11 09:33:54.000000 pm4pyminimal-2.7.9.3/pm4py/visualization/sna/variants/networkx.py
--rw-rw-rw-   0        0        0     5472 2023-12-11 09:33:54.000000 pm4pyminimal-2.7.9.3/pm4py/visualization/sna/variants/pyvis.py
--rw-rw-rw-   0        0        0     2561 2023-12-11 09:33:54.000000 pm4pyminimal-2.7.9.3/pm4py/visualization/sna/visualizer.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:43.128887 pm4pyminimal-2.7.9.3/pm4py/visualization/transition_system/
--rw-rw-rw-   0        0        0      812 2023-12-11 09:33:54.000000 pm4pyminimal-2.7.9.3/pm4py/visualization/transition_system/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:43.134497 pm4pyminimal-2.7.9.3/pm4py/visualization/transition_system/util/
--rw-rw-rw-   0        0        0      809 2023-12-11 09:33:54.000000 pm4pyminimal-2.7.9.3/pm4py/visualization/transition_system/util/__init__.py
--rw-rw-rw-   0        0        0     3315 2023-12-11 09:33:54.000000 pm4pyminimal-2.7.9.3/pm4py/visualization/transition_system/util/visualize_graphviz.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:43.140579 pm4pyminimal-2.7.9.3/pm4py/visualization/transition_system/variants/
--rw-rw-rw-   0        0        0      822 2023-12-11 09:33:54.000000 pm4pyminimal-2.7.9.3/pm4py/visualization/transition_system/variants/__init__.py
--rw-rw-rw-   0        0        0     3138 2023-12-11 09:33:54.000000 pm4pyminimal-2.7.9.3/pm4py/visualization/transition_system/variants/trans_frequency.py
--rw-rw-rw-   0        0        0     1652 2023-12-11 09:33:54.000000 pm4pyminimal-2.7.9.3/pm4py/visualization/transition_system/variants/view_based.py
--rw-rw-rw-   0        0        0     2703 2024-01-02 13:29:21.000000 pm4pyminimal-2.7.9.3/pm4py/visualization/transition_system/visualizer.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:43.145564 pm4pyminimal-2.7.9.3/pm4py/visualization/trie/
--rw-rw-rw-   0        0        0      793 2023-12-11 09:33:54.000000 pm4pyminimal-2.7.9.3/pm4py/visualization/trie/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:43.149553 pm4pyminimal-2.7.9.3/pm4py/visualization/trie/variants/
--rw-rw-rw-   0        0        0      789 2023-12-11 09:33:54.000000 pm4pyminimal-2.7.9.3/pm4py/visualization/trie/variants/__init__.py
--rw-rw-rw-   0        0        0     2765 2023-12-11 09:33:54.000000 pm4pyminimal-2.7.9.3/pm4py/visualization/trie/variants/classic.py
--rw-rw-rw-   0        0        0     2512 2024-01-02 13:29:21.000000 pm4pyminimal-2.7.9.3/pm4py/visualization/trie/visualizer.py
--rw-rw-rw-   0        0        0    15531 2023-12-11 09:33:54.000000 pm4pyminimal-2.7.9.3/pm4py/write.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:43.185245 pm4pyminimal-2.7.9.3/pm4pyminimal.egg-info/
--rw-rw-rw-   0        0        0     3369 2024-01-16 10:11:37.000000 pm4pyminimal-2.7.9.3/pm4pyminimal.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0    66584 2024-01-16 10:11:39.000000 pm4pyminimal-2.7.9.3/pm4pyminimal.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-01-16 10:11:37.000000 pm4pyminimal-2.7.9.3/pm4pyminimal.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       34 2024-01-16 10:11:37.000000 pm4pyminimal-2.7.9.3/pm4pyminimal.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2024-01-16 10:11:37.000000 pm4pyminimal-2.7.9.3/pm4pyminimal.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-01-16 10:11:43.189389 pm4pyminimal-2.7.9.3/setup.cfg
--rw-rw-rw-   0        0        0     1246 2023-12-11 09:33:54.000000 pm4pyminimal-2.7.9.3/setup.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:11:43.183251 pm4pyminimal-2.7.9.3/tests/
--rw-rw-rw-   0        0        0     4971 2023-11-09 06:59:42.000000 pm4pyminimal-2.7.9.3/tests/test_cli.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:34.652912 pm4pyminimal-2.7.9.4/
+-rw-rw-rw-   0        0        0    34817 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/LICENSE
+-rw-rw-rw-   0        0        0       29 2024-01-04 13:34:19.000000 pm4pyminimal-2.7.9.4/MANIFEST.in
+-rw-rw-rw-   0        0        0     3371 2024-01-29 06:15:34.637290 pm4pyminimal-2.7.9.4/PKG-INFO
+-rw-rw-rw-   0        0        0     2792 2024-01-29 06:13:52.000000 pm4pyminimal-2.7.9.4/README.md
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:31.754105 pm4pyminimal-2.7.9.4/pm4py/
+-rw-rw-rw-   0        0        0     7677 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/__init__.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:31.754105 pm4pyminimal-2.7.9.4/pm4py/algo/
+-rw-rw-rw-   0        0        0      854 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/__init__.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:31.754105 pm4pyminimal-2.7.9.4/pm4py/algo/analysis/
+-rw-rw-rw-   0        0        0      833 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/analysis/__init__.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:31.754105 pm4pyminimal-2.7.9.4/pm4py/algo/analysis/extended_marking_equation/
+-rw-rw-rw-   0        0        0      802 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/analysis/extended_marking_equation/__init__.py
+-rw-rw-rw-   0        0        0     3588 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/analysis/extended_marking_equation/algorithm.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:31.754105 pm4pyminimal-2.7.9.4/pm4py/algo/analysis/extended_marking_equation/variants/
+-rw-rw-rw-   0        0        0      810 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/analysis/extended_marking_equation/variants/__init__.py
+-rw-rw-rw-   0        0        0    21448 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/analysis/extended_marking_equation/variants/classic.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:31.754105 pm4pyminimal-2.7.9.4/pm4py/algo/analysis/marking_equation/
+-rw-rw-rw-   0        0        0      794 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/analysis/marking_equation/__init__.py
+-rw-rw-rw-   0        0        0     2689 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/analysis/marking_equation/algorithm.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:31.769733 pm4pyminimal-2.7.9.4/pm4py/algo/analysis/marking_equation/variants/
+-rw-rw-rw-   0        0        0      801 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/analysis/marking_equation/variants/__init__.py
+-rw-rw-rw-   0        0        0    11636 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/analysis/marking_equation/variants/classic.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:31.769733 pm4pyminimal-2.7.9.4/pm4py/algo/analysis/woflan/
+-rw-rw-rw-   0        0        0      836 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/analysis/woflan/__init__.py
+-rw-rw-rw-   0        0        0    32308 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/analysis/woflan/algorithm.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:31.785355 pm4pyminimal-2.7.9.4/pm4py/algo/analysis/woflan/graphs/
+-rw-rw-rw-   0        0        0      868 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/analysis/woflan/graphs/__init__.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:31.785355 pm4pyminimal-2.7.9.4/pm4py/algo/analysis/woflan/graphs/minimal_coverability_graph/
+-rw-rw-rw-   0        0        0      835 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/analysis/woflan/graphs/minimal_coverability_graph/__init__.py
+-rw-rw-rw-   0        0        0     7988 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/analysis/woflan/graphs/minimal_coverability_graph/minimal_coverability_graph.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:31.785355 pm4pyminimal-2.7.9.4/pm4py/algo/analysis/woflan/graphs/reachability_graph/
+-rw-rw-rw-   0        0        0      819 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/analysis/woflan/graphs/reachability_graph/__init__.py
+-rw-rw-rw-   0        0        0     2451 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/analysis/woflan/graphs/reachability_graph/reachability_graph.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:31.800976 pm4pyminimal-2.7.9.4/pm4py/algo/analysis/woflan/graphs/restricted_coverability_graph/
+-rw-rw-rw-   0        0        0      841 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/analysis/woflan/graphs/restricted_coverability_graph/__init__.py
+-rw-rw-rw-   0        0        0     4061 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/analysis/woflan/graphs/restricted_coverability_graph/restricted_coverability_graph.py
+-rw-rw-rw-   0        0        0     5745 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/analysis/woflan/graphs/utility.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:31.800976 pm4pyminimal-2.7.9.4/pm4py/algo/analysis/woflan/not_well_handled_pairs/
+-rw-rw-rw-   0        0        0      820 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/analysis/woflan/not_well_handled_pairs/__init__.py
+-rw-rw-rw-   0        0        0     2632 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/analysis/woflan/not_well_handled_pairs/not_well_handled_pairs.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:31.800976 pm4pyminimal-2.7.9.4/pm4py/algo/analysis/woflan/place_invariants/
+-rw-rw-rw-   0        0        0      849 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/analysis/woflan/place_invariants/__init__.py
+-rw-rw-rw-   0        0        0     4300 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/analysis/woflan/place_invariants/place_invariants.py
+-rw-rw-rw-   0        0        0     3668 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/analysis/woflan/place_invariants/s_component.py
+-rw-rw-rw-   0        0        0     1098 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/analysis/woflan/place_invariants/uniform_invariant.py
+-rw-rw-rw-   0        0        0     8333 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/analysis/woflan/place_invariants/utility.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:31.816595 pm4pyminimal-2.7.9.4/pm4py/algo/analysis/workflow_net/
+-rw-rw-rw-   0        0        0      800 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/analysis/workflow_net/__init__.py
+-rw-rw-rw-   0        0        0     1542 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/analysis/workflow_net/algorithm.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:31.816595 pm4pyminimal-2.7.9.4/pm4py/algo/analysis/workflow_net/variants/
+-rw-rw-rw-   0        0        0      799 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/analysis/workflow_net/variants/__init__.py
+-rw-rw-rw-   0        0        0     3243 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/analysis/workflow_net/variants/petri_net.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:31.816595 pm4pyminimal-2.7.9.4/pm4py/algo/anonymization/
+-rw-rw-rw-   0        0        0      979 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/anonymization/__init__.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:31.816595 pm4pyminimal-2.7.9.4/pm4py/algo/anonymization/pripel/
+-rw-rw-rw-   0        0        0      807 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/anonymization/pripel/__init__.py
+-rw-rw-rw-   0        0        0     3170 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/anonymization/pripel/algorithm.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:31.832219 pm4pyminimal-2.7.9.4/pm4py/algo/anonymization/pripel/util/
+-rw-rw-rw-   0        0        0    13889 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/anonymization/pripel/util/AttributeAnonymizer.py
+-rw-rw-rw-   0        0        0    14468 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/anonymization/pripel/util/TraceMatcher.py
+-rw-rw-rw-   0        0        0      837 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/anonymization/pripel/util/__init__.py
+-rw-rw-rw-   0        0        0     1754 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/anonymization/pripel/util/trace_levenshtein.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:31.832219 pm4pyminimal-2.7.9.4/pm4py/algo/anonymization/pripel/variants/
+-rw-rw-rw-   0        0        0      797 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/anonymization/pripel/variants/__init__.py
+-rw-rw-rw-   0        0        0     5291 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/anonymization/pripel/variants/pripel.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:31.832219 pm4pyminimal-2.7.9.4/pm4py/algo/anonymization/trace_variant_query/
+-rw-rw-rw-   0        0        0      820 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/anonymization/trace_variant_query/__init__.py
+-rw-rw-rw-   0        0        0     3980 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/anonymization/trace_variant_query/algorithm.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:31.847838 pm4pyminimal-2.7.9.4/pm4py/algo/anonymization/trace_variant_query/util/
+-rw-rw-rw-   0        0        0      839 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/anonymization/trace_variant_query/util/__init__.py
+-rw-rw-rw-   0        0        0     6862 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/anonymization/trace_variant_query/util/behavioralAppropriateness.py
+-rw-rw-rw-   0        0        0     1323 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/anonymization/trace_variant_query/util/exp_mech.py
+-rw-rw-rw-   0        0        0     1687 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/anonymization/trace_variant_query/util/util.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:31.854344 pm4pyminimal-2.7.9.4/pm4py/algo/anonymization/trace_variant_query/variants/
+-rw-rw-rw-   0        0        0      817 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/anonymization/trace_variant_query/variants/__init__.py
+-rw-rw-rw-   0        0        0     7691 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/anonymization/trace_variant_query/variants/laplace.py
+-rw-rw-rw-   0        0        0    11329 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/anonymization/trace_variant_query/variants/sacofa.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:31.854344 pm4pyminimal-2.7.9.4/pm4py/algo/clustering/
+-rw-rw-rw-   0        0        0      734 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/clustering/__init__.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:31.854344 pm4pyminimal-2.7.9.4/pm4py/algo/clustering/profiles/
+-rw-rw-rw-   0        0        0      798 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/clustering/profiles/__init__.py
+-rw-rw-rw-   0        0        0     2118 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/clustering/profiles/algorithm.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:31.854344 pm4pyminimal-2.7.9.4/pm4py/algo/clustering/profiles/variants/
+-rw-rw-rw-   0        0        0      804 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/clustering/profiles/variants/__init__.py
+-rw-rw-rw-   0        0        0     3544 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/clustering/profiles/variants/sklearn_profiles.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:31.854344 pm4pyminimal-2.7.9.4/pm4py/algo/clustering/trace_attribute_driven/
+-rw-rw-rw-   0        0        0     1060 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/clustering/trace_attribute_driven/__init__.py
+-rw-rw-rw-   0        0        0     4705 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/clustering/trace_attribute_driven/algorithm.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:31.869972 pm4pyminimal-2.7.9.4/pm4py/algo/clustering/trace_attribute_driven/dfg/
+-rw-rw-rw-   0        0        0      805 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/clustering/trace_attribute_driven/dfg/__init__.py
+-rw-rw-rw-   0        0        0     3989 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/clustering/trace_attribute_driven/dfg/dfg_dist.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:31.869972 pm4pyminimal-2.7.9.4/pm4py/algo/clustering/trace_attribute_driven/leven_dist/
+-rw-rw-rw-   0        0        0      819 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/clustering/trace_attribute_driven/leven_dist/__init__.py
+-rw-rw-rw-   0        0        0     5473 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/clustering/trace_attribute_driven/leven_dist/leven_dist_calc.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:31.869972 pm4pyminimal-2.7.9.4/pm4py/algo/clustering/trace_attribute_driven/linkage_method/
+-rw-rw-rw-   0        0        0      819 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/clustering/trace_attribute_driven/linkage_method/__init__.py
+-rw-rw-rw-   0        0        0    13583 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/clustering/trace_attribute_driven/linkage_method/linkage_avg.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:31.869972 pm4pyminimal-2.7.9.4/pm4py/algo/clustering/trace_attribute_driven/merge_log/
+-rw-rw-rw-   0        0        0      812 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/clustering/trace_attribute_driven/merge_log/__init__.py
+-rw-rw-rw-   0        0        0     4290 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/clustering/trace_attribute_driven/merge_log/merge_log.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:31.885593 pm4pyminimal-2.7.9.4/pm4py/algo/clustering/trace_attribute_driven/util/
+-rw-rw-rw-   0        0        0      824 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/clustering/trace_attribute_driven/util/__init__.py
+-rw-rw-rw-   0        0        0     3396 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/clustering/trace_attribute_driven/util/evaluation.py
+-rw-rw-rw-   0        0        0    15776 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/clustering/trace_attribute_driven/util/filter_subsets.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:31.901222 pm4pyminimal-2.7.9.4/pm4py/algo/clustering/trace_attribute_driven/variants/
+-rw-rw-rw-   0        0        0      855 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/clustering/trace_attribute_driven/variants/__init__.py
+-rw-rw-rw-   0        0        0    18463 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/clustering/trace_attribute_driven/variants/act_dist_calc.py
+-rw-rw-rw-   0        0        0     6806 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/clustering/trace_attribute_driven/variants/logslice_dist.py
+-rw-rw-rw-   0        0        0     6329 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/clustering/trace_attribute_driven/variants/sim_calc.py
+-rw-rw-rw-   0        0        0    15790 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/clustering/trace_attribute_driven/variants/suc_dist_calc.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:31.901222 pm4pyminimal-2.7.9.4/pm4py/algo/comparison/
+-rw-rw-rw-   0        0        0      851 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/comparison/__init__.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:31.901222 pm4pyminimal-2.7.9.4/pm4py/algo/comparison/petrinet/
+-rw-rw-rw-   0        0        0      803 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/comparison/petrinet/__init__.py
+-rw-rw-rw-   0        0        0     6719 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/comparison/petrinet/element_usage_comparison.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:31.901222 pm4pyminimal-2.7.9.4/pm4py/algo/conformance/
+-rw-rw-rw-   0        0        0      946 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/conformance/__init__.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:31.901222 pm4pyminimal-2.7.9.4/pm4py/algo/conformance/alignments/
+-rw-rw-rw-   0        0        0      822 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/conformance/alignments/__init__.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:31.901222 pm4pyminimal-2.7.9.4/pm4py/algo/conformance/alignments/decomposed/
+-rw-rw-rw-   0        0        0      812 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/conformance/alignments/decomposed/__init__.py
+-rw-rw-rw-   0        0        0     2018 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/conformance/alignments/decomposed/algorithm.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:31.916836 pm4pyminimal-2.7.9.4/pm4py/algo/conformance/alignments/decomposed/variants/
+-rw-rw-rw-   0        0        0      818 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/conformance/alignments/decomposed/variants/__init__.py
+-rw-rw-rw-   0        0        0    19051 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/conformance/alignments/decomposed/variants/recompos_maximal.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:31.916836 pm4pyminimal-2.7.9.4/pm4py/algo/conformance/alignments/dfg/
+-rw-rw-rw-   0        0        0      805 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/conformance/alignments/dfg/__init__.py
+-rw-rw-rw-   0        0        0     1956 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/conformance/alignments/dfg/algorithm.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:31.916836 pm4pyminimal-2.7.9.4/pm4py/algo/conformance/alignments/dfg/variants/
+-rw-rw-rw-   0        0        0      802 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/conformance/alignments/dfg/variants/__init__.py
+-rw-rw-rw-   0        0        0    24120 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/conformance/alignments/dfg/variants/classic.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:31.916836 pm4pyminimal-2.7.9.4/pm4py/algo/conformance/alignments/edit_distance/
+-rw-rw-rw-   0        0        0      815 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/conformance/alignments/edit_distance/__init__.py
+-rw-rw-rw-   0        0        0     1876 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/conformance/alignments/edit_distance/algorithm.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:31.916836 pm4pyminimal-2.7.9.4/pm4py/algo/conformance/alignments/edit_distance/variants/
+-rw-rw-rw-   0        0        0      818 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/conformance/alignments/edit_distance/variants/__init__.py
+-rw-rw-rw-   0        0        0    11234 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/conformance/alignments/edit_distance/variants/edit_distance.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:31.932457 pm4pyminimal-2.7.9.4/pm4py/algo/conformance/alignments/petri_net/
+-rw-rw-rw-   0        0        0      818 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/conformance/alignments/petri_net/__init__.py
+-rw-rw-rw-   0        0        0    16964 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/conformance/alignments/petri_net/algorithm.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:31.932457 pm4pyminimal-2.7.9.4/pm4py/algo/conformance/alignments/petri_net/utils/
+-rw-rw-rw-   0        0        0      812 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/conformance/alignments/petri_net/utils/__init__.py
+-rw-rw-rw-   0        0        0     2896 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/conformance/alignments/petri_net/utils/log_enrichment.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:31.954581 pm4pyminimal-2.7.9.4/pm4py/algo/conformance/alignments/petri_net/variants/
+-rw-rw-rw-   0        0        0      925 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/conformance/alignments/petri_net/variants/__init__.py
+-rw-rw-rw-   0        0        0    27553 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/conformance/alignments/petri_net/variants/dijkstra_less_memory.py
+-rw-rw-rw-   0        0        0    17167 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/conformance/alignments/petri_net/variants/dijkstra_no_heuristics.py
+-rw-rw-rw-   0        0        0    23651 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/conformance/alignments/petri_net/variants/discounted_a_star.py
+-rw-rw-rw-   0        0        0    23429 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/conformance/alignments/petri_net/variants/generator_dijkstra_less_memory.py
+-rw-rw-rw-   0        0        0    17357 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/conformance/alignments/petri_net/variants/generator_dijkstra_no_heuristics.py
+-rw-rw-rw-   0        0        0    23978 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/conformance/alignments/petri_net/variants/state_equation_a_star.py
+-rw-rw-rw-   0        0        0    27872 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/conformance/alignments/petri_net/variants/tweaked_state_equation_a_star.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:31.954581 pm4pyminimal-2.7.9.4/pm4py/algo/conformance/alignments/process_tree/
+-rw-rw-rw-   0        0        0      820 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/conformance/alignments/process_tree/__init__.py
+-rw-rw-rw-   0        0        0     2203 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/conformance/alignments/process_tree/algorithm.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:31.954581 pm4pyminimal-2.7.9.4/pm4py/algo/conformance/alignments/process_tree/util/
+-rw-rw-rw-   0        0        0      870 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/conformance/alignments/process_tree/util/__init__.py
+-rw-rw-rw-   0        0        0     3355 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/conformance/alignments/process_tree/util/search_graph_pt_frequency_annotation.py
+-rw-rw-rw-   0        0        0    15712 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/conformance/alignments/process_tree/util/search_graph_pt_replay_semantics.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:31.954581 pm4pyminimal-2.7.9.4/pm4py/algo/conformance/alignments/process_tree/variants/
+-rw-rw-rw-   0        0        0      833 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/conformance/alignments/process_tree/variants/__init__.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:31.978044 pm4pyminimal-2.7.9.4/pm4py/algo/conformance/alignments/process_tree/variants/approximated/
+-rw-rw-rw-   0        0        0      871 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/conformance/alignments/process_tree/variants/approximated/__init__.py
+-rw-rw-rw-   0        0        0     5361 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/conformance/alignments/process_tree/variants/approximated/calculate_a_sa_ea_sets.py
+-rw-rw-rw-   0        0        0    49808 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/conformance/alignments/process_tree/variants/approximated/matrix_lp.py
+-rw-rw-rw-   0        0        0    36425 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/conformance/alignments/process_tree/variants/approximated/original.py
+-rw-rw-rw-   0        0        0     6660 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/conformance/alignments/process_tree/variants/approximated/utilities.py
+-rw-rw-rw-   0        0        0    17939 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/conformance/alignments/process_tree/variants/search_graph_pt.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:31.978044 pm4pyminimal-2.7.9.4/pm4py/algo/conformance/antialignments/
+-rw-rw-rw-   0        0        0      805 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/conformance/antialignments/__init__.py
+-rw-rw-rw-   0        0        0     3166 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/conformance/antialignments/algorithm.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:31.978044 pm4pyminimal-2.7.9.4/pm4py/algo/conformance/antialignments/variants/
+-rw-rw-rw-   0        0        0      812 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/conformance/antialignments/variants/__init__.py
+-rw-rw-rw-   0        0        0     7582 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/conformance/antialignments/variants/discounted_a_star.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:31.978044 pm4pyminimal-2.7.9.4/pm4py/algo/conformance/declare/
+-rw-rw-rw-   0        0        0      800 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/conformance/declare/__init__.py
+-rw-rw-rw-   0        0        0     2733 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/conformance/declare/algorithm.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:31.978044 pm4pyminimal-2.7.9.4/pm4py/algo/conformance/declare/variants/
+-rw-rw-rw-   0        0        0      797 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/conformance/declare/variants/__init__.py
+-rw-rw-rw-   0        0        0    18351 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/conformance/declare/variants/classic.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:31.993682 pm4pyminimal-2.7.9.4/pm4py/algo/conformance/footprints/
+-rw-rw-rw-   0        0        0      807 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/conformance/footprints/__init__.py
+-rw-rw-rw-   0        0        0     2061 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/conformance/footprints/algorithm.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:31.993682 pm4pyminimal-2.7.9.4/pm4py/algo/conformance/footprints/util/
+-rw-rw-rw-   0        0        0      817 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/conformance/footprints/util/__init__.py
+-rw-rw-rw-   0        0        0     6154 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/conformance/footprints/util/evaluation.py
+-rw-rw-rw-   0        0        0     3573 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/conformance/footprints/util/tree_visualization.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:31.993682 pm4pyminimal-2.7.9.4/pm4py/algo/conformance/footprints/variants/
+-rw-rw-rw-   0        0        0      832 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/conformance/footprints/variants/__init__.py
+-rw-rw-rw-   0        0        0     3708 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/conformance/footprints/variants/log_extensive.py
+-rw-rw-rw-   0        0        0     5119 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/conformance/footprints/variants/log_model.py
+-rw-rw-rw-   0        0        0     7141 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/conformance/footprints/variants/trace_extensive.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:32.011525 pm4pyminimal-2.7.9.4/pm4py/algo/conformance/log_skeleton/
+-rw-rw-rw-   0        0        0      803 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/conformance/log_skeleton/__init__.py
+-rw-rw-rw-   0        0        0     4040 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/conformance/log_skeleton/algorithm.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:32.011525 pm4pyminimal-2.7.9.4/pm4py/algo/conformance/log_skeleton/variants/
+-rw-rw-rw-   0        0        0      800 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/conformance/log_skeleton/variants/__init__.py
+-rw-rw-rw-   0        0        0    13160 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/conformance/log_skeleton/variants/classic.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:32.011525 pm4pyminimal-2.7.9.4/pm4py/algo/conformance/multialignments/
+-rw-rw-rw-   0        0        0      806 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/conformance/multialignments/__init__.py
+-rw-rw-rw-   0        0        0     3143 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/conformance/multialignments/algorithm.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:32.011525 pm4pyminimal-2.7.9.4/pm4py/algo/conformance/multialignments/variants/
+-rw-rw-rw-   0        0        0      813 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/conformance/multialignments/variants/__init__.py
+-rw-rw-rw-   0        0        0     6557 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/conformance/multialignments/variants/discounted_a_star.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:32.011525 pm4pyminimal-2.7.9.4/pm4py/algo/conformance/temporal_profile/
+-rw-rw-rw-   0        0        0      807 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/conformance/temporal_profile/__init__.py
+-rw-rw-rw-   0        0        0     4738 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/conformance/temporal_profile/algorithm.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:32.027149 pm4pyminimal-2.7.9.4/pm4py/algo/conformance/temporal_profile/variants/
+-rw-rw-rw-   0        0        0      811 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/conformance/temporal_profile/variants/__init__.py
+-rw-rw-rw-   0        0        0     5476 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/conformance/temporal_profile/variants/dataframe.py
+-rw-rw-rw-   0        0        0     5957 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/conformance/temporal_profile/variants/log.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:32.027149 pm4pyminimal-2.7.9.4/pm4py/algo/conformance/tokenreplay/
+-rw-rw-rw-   0        0        0      815 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/conformance/tokenreplay/__init__.py
+-rw-rw-rw-   0        0        0     2965 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/conformance/tokenreplay/algorithm.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:32.027149 pm4pyminimal-2.7.9.4/pm4py/algo/conformance/tokenreplay/diagnostics/
+-rw-rw-rw-   0        0        0      836 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/conformance/tokenreplay/diagnostics/__init__.py
+-rw-rw-rw-   0        0        0     6720 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/conformance/tokenreplay/diagnostics/duration_diagnostics.py
+-rw-rw-rw-   0        0        0    11104 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/conformance/tokenreplay/diagnostics/root_cause_analysis.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:32.042778 pm4pyminimal-2.7.9.4/pm4py/algo/conformance/tokenreplay/variants/
+-rw-rw-rw-   0        0        0      804 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/conformance/tokenreplay/variants/__init__.py
+-rw-rw-rw-   0        0        0    12130 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/conformance/tokenreplay/variants/backwards.py
+-rw-rw-rw-   0        0        0    61056 2024-01-22 11:53:06.000000 pm4pyminimal-2.7.9.4/pm4py/algo/conformance/tokenreplay/variants/token_replay.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:32.042778 pm4pyminimal-2.7.9.4/pm4py/algo/connectors/
+-rw-rw-rw-   0        0        0      786 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/connectors/__init__.py
+-rw-rw-rw-   0        0        0     2768 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/connectors/algorithm.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:32.042778 pm4pyminimal-2.7.9.4/pm4py/algo/connectors/util/
+-rw-rw-rw-   0        0        0      781 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/connectors/util/__init__.py
+-rw-rw-rw-   0        0        0     1628 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/connectors/util/mail.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:32.054784 pm4pyminimal-2.7.9.4/pm4py/algo/connectors/variants/
+-rw-rw-rw-   0        0        0      736 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/connectors/variants/__init__.py
+-rw-rw-rw-   0        0        0     2592 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/connectors/variants/camunda_workflow.py
+-rw-rw-rw-   0        0        0     3743 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/connectors/variants/chrome_history.py
+-rw-rw-rw-   0        0        0     3777 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/connectors/variants/firefox_history.py
+-rw-rw-rw-   0        0        0     5250 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/connectors/variants/github_repo.py
+-rw-rw-rw-   0        0        0     4432 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/connectors/variants/outlook_calendar.py
+-rw-rw-rw-   0        0        0     4568 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/connectors/variants/outlook_mail_extractor.py
+-rw-rw-rw-   0        0        0     3168 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/connectors/variants/sap_accounting.py
+-rw-rw-rw-   0        0        0     4012 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/connectors/variants/sap_o2c.py
+-rw-rw-rw-   0        0        0     4243 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/connectors/variants/windows_events.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:32.070411 pm4pyminimal-2.7.9.4/pm4py/algo/decision_mining/
+-rw-rw-rw-   0        0        0      964 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/decision_mining/__init__.py
+-rw-rw-rw-   0        0        0    23509 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/decision_mining/algorithm.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:32.070411 pm4pyminimal-2.7.9.4/pm4py/algo/discovery/
+-rw-rw-rw-   0        0        0      945 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/discovery/__init__.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:32.070411 pm4pyminimal-2.7.9.4/pm4py/algo/discovery/alpha/
+-rw-rw-rw-   0        0        0      818 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/discovery/alpha/__init__.py
+-rw-rw-rw-   0        0        0     5066 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/discovery/alpha/algorithm.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:32.070411 pm4pyminimal-2.7.9.4/pm4py/algo/discovery/alpha/data_structures/
+-rw-rw-rw-   0        0        0      816 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/discovery/alpha/data_structures/__init__.py
+-rw-rw-rw-   0        0        0     2420 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/discovery/alpha/data_structures/alpha_classic_abstraction.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:32.086033 pm4pyminimal-2.7.9.4/pm4py/algo/discovery/alpha/utils/
+-rw-rw-rw-   0        0        0      790 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/discovery/alpha/utils/__init__.py
+-rw-rw-rw-   0        0        0     1622 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/discovery/alpha/utils/endpoints.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:32.086033 pm4pyminimal-2.7.9.4/pm4py/algo/discovery/alpha/variants/
+-rw-rw-rw-   0        0        0      797 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/discovery/alpha/variants/__init__.py
+-rw-rw-rw-   0        0        0    10830 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/discovery/alpha/variants/classic.py
+-rw-rw-rw-   0        0        0    22005 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/discovery/alpha/variants/plus.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:32.086033 pm4pyminimal-2.7.9.4/pm4py/algo/discovery/batches/
+-rw-rw-rw-   0        0        0      803 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/discovery/batches/__init__.py
+-rw-rw-rw-   0        0        0     3756 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/discovery/batches/algorithm.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:32.086033 pm4pyminimal-2.7.9.4/pm4py/algo/discovery/batches/utils/
+-rw-rw-rw-   0        0        0      792 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/discovery/batches/utils/__init__.py
+-rw-rw-rw-   0        0        0     9636 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/discovery/batches/utils/detection.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:32.101656 pm4pyminimal-2.7.9.4/pm4py/algo/discovery/batches/variants/
+-rw-rw-rw-   0        0        0      797 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/discovery/batches/variants/__init__.py
+-rw-rw-rw-   0        0        0     5216 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/discovery/batches/variants/log.py
+-rw-rw-rw-   0        0        0     6427 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/discovery/batches/variants/pandas.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:32.101656 pm4pyminimal-2.7.9.4/pm4py/algo/discovery/causal/
+-rw-rw-rw-   0        0        0      795 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/discovery/causal/__init__.py
+-rw-rw-rw-   0        0        0     1646 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/discovery/causal/algorithm.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:32.113190 pm4pyminimal-2.7.9.4/pm4py/algo/discovery/causal/variants/
+-rw-rw-rw-   0        0        0      801 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/discovery/causal/variants/__init__.py
+-rw-rw-rw-   0        0        0     1787 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/discovery/causal/variants/alpha.py
+-rw-rw-rw-   0        0        0     1589 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/discovery/causal/variants/heuristic.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:32.113190 pm4pyminimal-2.7.9.4/pm4py/algo/discovery/correlation_mining/
+-rw-rw-rw-   0        0        0      813 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/discovery/correlation_mining/__init__.py
+-rw-rw-rw-   0        0        0     2249 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/discovery/correlation_mining/algorithm.py
+-rw-rw-rw-   0        0        0     7934 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/discovery/correlation_mining/util.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:32.113190 pm4pyminimal-2.7.9.4/pm4py/algo/discovery/correlation_mining/variants/
+-rw-rw-rw-   0        0        0      832 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/discovery/correlation_mining/variants/__init__.py
+-rw-rw-rw-   0        0        0     9663 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/discovery/correlation_mining/variants/classic.py
+-rw-rw-rw-   0        0        0     4405 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/discovery/correlation_mining/variants/classic_split.py
+-rw-rw-rw-   0        0        0    10288 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/discovery/correlation_mining/variants/trace_based.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:32.128817 pm4pyminimal-2.7.9.4/pm4py/algo/discovery/declare/
+-rw-rw-rw-   0        0        0      798 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/discovery/declare/__init__.py
+-rw-rw-rw-   0        0        0     1725 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/discovery/declare/algorithm.py
+-rw-rw-rw-   0        0        0     1290 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/discovery/declare/templates.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:32.128817 pm4pyminimal-2.7.9.4/pm4py/algo/discovery/declare/variants/
+-rw-rw-rw-   0        0        0      795 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/discovery/declare/variants/__init__.py
+-rw-rw-rw-   0        0        0    30263 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/discovery/declare/variants/classic.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:32.128817 pm4pyminimal-2.7.9.4/pm4py/algo/discovery/dfg/
+-rw-rw-rw-   0        0        0      822 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/discovery/dfg/__init__.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:32.128817 pm4pyminimal-2.7.9.4/pm4py/algo/discovery/dfg/adapters/
+-rw-rw-rw-   0        0        0      788 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/discovery/dfg/adapters/__init__.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:32.145569 pm4pyminimal-2.7.9.4/pm4py/algo/discovery/dfg/adapters/pandas/
+-rw-rw-rw-   0        0        0      816 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/discovery/dfg/adapters/pandas/__init__.py
+-rw-rw-rw-   0        0        0    15047 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/discovery/dfg/adapters/pandas/df_statistics.py
+-rw-rw-rw-   0        0        0     2962 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/discovery/dfg/adapters/pandas/freq_triples.py
+-rw-rw-rw-   0        0        0     4898 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/discovery/dfg/algorithm.py
+-rw-rw-rw-   0        0        0     1260 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/discovery/dfg/replacement.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:32.145569 pm4pyminimal-2.7.9.4/pm4py/algo/discovery/dfg/utils/
+-rw-rw-rw-   0        0        0      788 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/discovery/dfg/utils/__init__.py
+-rw-rw-rw-   0        0        0      783 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/discovery/dfg/utils/dfg_utils.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:32.155078 pm4pyminimal-2.7.9.4/pm4py/algo/discovery/dfg/variants/
+-rw-rw-rw-   0        0        0      968 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/discovery/dfg/variants/__init__.py
+-rw-rw-rw-   0        0        0     4609 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/discovery/dfg/variants/case_attributes.py
+-rw-rw-rw-   0        0        0     2852 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/discovery/dfg/variants/clean.py
+-rw-rw-rw-   0        0        0     2795 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/discovery/dfg/variants/clean_polars.py
+-rw-rw-rw-   0        0        0     3347 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/discovery/dfg/variants/clean_time.py
+-rw-rw-rw-   0        0        0     2200 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/discovery/dfg/variants/freq_triples.py
+-rw-rw-rw-   0        0        0     2574 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/discovery/dfg/variants/native.py
+-rw-rw-rw-   0        0        0     5794 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/discovery/dfg/variants/performance.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:32.170703 pm4pyminimal-2.7.9.4/pm4py/algo/discovery/footprints/
+-rw-rw-rw-   0        0        0      812 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/discovery/footprints/__init__.py
+-rw-rw-rw-   0        0        0     3131 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/discovery/footprints/algorithm.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:32.170703 pm4pyminimal-2.7.9.4/pm4py/algo/discovery/footprints/dfg/
+-rw-rw-rw-   0        0        0      792 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/discovery/footprints/dfg/__init__.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:32.170703 pm4pyminimal-2.7.9.4/pm4py/algo/discovery/footprints/dfg/variants/
+-rw-rw-rw-   0        0        0      796 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/discovery/footprints/dfg/variants/__init__.py
+-rw-rw-rw-   0        0        0     2258 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/discovery/footprints/dfg/variants/dfg.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:32.186325 pm4pyminimal-2.7.9.4/pm4py/algo/discovery/footprints/log/
+-rw-rw-rw-   0        0        0      792 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/discovery/footprints/log/__init__.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:32.186325 pm4pyminimal-2.7.9.4/pm4py/algo/discovery/footprints/log/variants/
+-rw-rw-rw-   0        0        0      843 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/discovery/footprints/log/variants/__init__.py
+-rw-rw-rw-   0        0        0     4664 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/discovery/footprints/log/variants/entire_dataframe.py
+-rw-rw-rw-   0        0        0     3314 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/discovery/footprints/log/variants/entire_event_log.py
+-rw-rw-rw-   0        0        0     3195 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/discovery/footprints/log/variants/trace_by_trace.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:32.186325 pm4pyminimal-2.7.9.4/pm4py/algo/discovery/footprints/petri/
+-rw-rw-rw-   0        0        0      794 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/discovery/footprints/petri/__init__.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:32.201946 pm4pyminimal-2.7.9.4/pm4py/algo/discovery/footprints/petri/variants/
+-rw-rw-rw-   0        0        0      806 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/discovery/footprints/petri/variants/__init__.py
+-rw-rw-rw-   0        0        0     3629 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/discovery/footprints/petri/variants/reach_graph.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:32.201946 pm4pyminimal-2.7.9.4/pm4py/algo/discovery/footprints/tree/
+-rw-rw-rw-   0        0        0      793 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/discovery/footprints/tree/__init__.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:32.201946 pm4pyminimal-2.7.9.4/pm4py/algo/discovery/footprints/tree/variants/
+-rw-rw-rw-   0        0        0      802 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/discovery/footprints/tree/variants/__init__.py
+-rw-rw-rw-   0        0        0    13403 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/discovery/footprints/tree/variants/bottomup.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:32.217568 pm4pyminimal-2.7.9.4/pm4py/algo/discovery/heuristics/
+-rw-rw-rw-   0        0        0      799 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/discovery/heuristics/__init__.py
+-rw-rw-rw-   0        0        0     7484 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/discovery/heuristics/algorithm.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:32.217568 pm4pyminimal-2.7.9.4/pm4py/algo/discovery/heuristics/variants/
+-rw-rw-rw-   0        0        0      806 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/discovery/heuristics/variants/__init__.py
+-rw-rw-rw-   0        0        0    26145 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/discovery/heuristics/variants/classic.py
+-rw-rw-rw-   0        0        0    24355 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/discovery/heuristics/variants/plusplus.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:32.217568 pm4pyminimal-2.7.9.4/pm4py/algo/discovery/ilp/
+-rw-rw-rw-   0        0        0      792 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/discovery/ilp/__init__.py
+-rw-rw-rw-   0        0        0     1782 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/discovery/ilp/algorithm.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:32.233190 pm4pyminimal-2.7.9.4/pm4py/algo/discovery/ilp/variants/
+-rw-rw-rw-   0        0        0      789 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/discovery/ilp/variants/__init__.py
+-rw-rw-rw-   0        0        0    12873 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/discovery/ilp/variants/classic.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:32.233190 pm4pyminimal-2.7.9.4/pm4py/algo/discovery/inductive/
+-rw-rw-rw-   0        0        0      800 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/discovery/inductive/__init__.py
+-rw-rw-rw-   0        0        0     3602 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/discovery/inductive/algorithm.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:32.255317 pm4pyminimal-2.7.9.4/pm4py/algo/discovery/inductive/base_case/
+-rw-rw-rw-   0        0        0      829 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/discovery/inductive/base_case/__init__.py
+-rw-rw-rw-   0        0        0     1533 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/discovery/inductive/base_case/abc.py
+-rw-rw-rw-   0        0        0     1768 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/discovery/inductive/base_case/empty_log.py
+-rw-rw-rw-   0        0        0     2268 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/discovery/inductive/base_case/factory.py
+-rw-rw-rw-   0        0        0     2060 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/discovery/inductive/base_case/single_activity.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:32.273260 pm4pyminimal-2.7.9.4/pm4py/algo/discovery/inductive/cuts/
+-rw-rw-rw-   0        0        0      816 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/discovery/inductive/cuts/__init__.py
+-rw-rw-rw-   0        0        0     2100 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/discovery/inductive/cuts/abc.py
+-rw-rw-rw-   0        0        0     4570 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/discovery/inductive/cuts/concurrency.py
+-rw-rw-rw-   0        0        0     3143 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/discovery/inductive/cuts/factory.py
+-rw-rw-rw-   0        0        0    10916 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/discovery/inductive/cuts/loop.py
+-rw-rw-rw-   0        0        0    11571 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/discovery/inductive/cuts/sequence.py
+-rw-rw-rw-   0        0        0     1519 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/discovery/inductive/cuts/utils.py
+-rw-rw-rw-   0        0        0     4316 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/discovery/inductive/cuts/xor.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:32.273260 pm4pyminimal-2.7.9.4/pm4py/algo/discovery/inductive/dtypes/
+-rw-rw-rw-   0        0        0      797 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/discovery/inductive/dtypes/__init__.py
+-rw-rw-rw-   0        0        0     1050 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/discovery/inductive/dtypes/im_dfg.py
+-rw-rw-rw-   0        0        0     2568 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/discovery/inductive/dtypes/im_ds.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:32.304503 pm4pyminimal-2.7.9.4/pm4py/algo/discovery/inductive/fall_through/
+-rw-rw-rw-   0        0        0      897 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/discovery/inductive/fall_through/__init__.py
+-rw-rw-rw-   0        0        0     1385 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/discovery/inductive/fall_through/abc.py
+-rw-rw-rw-   0        0        0     4792 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/discovery/inductive/fall_through/activity_concurrent.py
+-rw-rw-rw-   0        0        0     1643 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/discovery/inductive/fall_through/activity_once_per_trace.py
+-rw-rw-rw-   0        0        0     2709 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/discovery/inductive/fall_through/empty_traces.py
+-rw-rw-rw-   0        0        0     3254 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/discovery/inductive/fall_through/factory.py
+-rw-rw-rw-   0        0        0     3059 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/discovery/inductive/fall_through/flower.py
+-rw-rw-rw-   0        0        0     2441 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/discovery/inductive/fall_through/strict_tau_loop.py
+-rw-rw-rw-   0        0        0     1520 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/discovery/inductive/fall_through/tau_loop.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:32.320125 pm4pyminimal-2.7.9.4/pm4py/algo/discovery/inductive/variants/
+-rw-rw-rw-   0        0        0      807 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/discovery/inductive/variants/__init__.py
+-rw-rw-rw-   0        0        0     4160 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/discovery/inductive/variants/abc.py
+-rw-rw-rw-   0        0        0     1740 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/discovery/inductive/variants/im.py
+-rw-rw-rw-   0        0        0     1098 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/discovery/inductive/variants/imd.py
+-rw-rw-rw-   0        0        0     4381 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/discovery/inductive/variants/imf.py
+-rw-rw-rw-   0        0        0      881 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/discovery/inductive/variants/instances.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:32.320125 pm4pyminimal-2.7.9.4/pm4py/algo/discovery/log_skeleton/
+-rw-rw-rw-   0        0        0      815 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/discovery/log_skeleton/__init__.py
+-rw-rw-rw-   0        0        0     2450 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/discovery/log_skeleton/algorithm.py
+-rw-rw-rw-   0        0        0     3194 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/discovery/log_skeleton/trace_skel.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:32.320125 pm4pyminimal-2.7.9.4/pm4py/algo/discovery/log_skeleton/variants/
+-rw-rw-rw-   0        0        0      798 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/discovery/log_skeleton/variants/__init__.py
+-rw-rw-rw-   0        0        0    11111 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/discovery/log_skeleton/variants/classic.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:32.335747 pm4pyminimal-2.7.9.4/pm4py/algo/discovery/minimum_self_distance/
+-rw-rw-rw-   0        0        0      819 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/discovery/minimum_self_distance/__init__.py
+-rw-rw-rw-   0        0        0     1567 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/discovery/minimum_self_distance/algorithm.py
+-rw-rw-rw-   0        0        0     3132 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/discovery/minimum_self_distance/utils.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:32.355397 pm4pyminimal-2.7.9.4/pm4py/algo/discovery/minimum_self_distance/variants/
+-rw-rw-rw-   0        0        0      811 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/discovery/minimum_self_distance/variants/__init__.py
+-rw-rw-rw-   0        0        0     2878 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/discovery/minimum_self_distance/variants/log.py
+-rw-rw-rw-   0        0        0     2904 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/discovery/minimum_self_distance/variants/pandas.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:32.355397 pm4pyminimal-2.7.9.4/pm4py/algo/discovery/ocel/
+-rw-rw-rw-   0        0        0      802 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/discovery/ocel/__init__.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:32.355397 pm4pyminimal-2.7.9.4/pm4py/algo/discovery/ocel/interleavings/
+-rw-rw-rw-   0        0        0      814 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/discovery/ocel/interleavings/__init__.py
+-rw-rw-rw-   0        0        0     2007 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/discovery/ocel/interleavings/algorithm.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:32.355397 pm4pyminimal-2.7.9.4/pm4py/algo/discovery/ocel/interleavings/utils/
+-rw-rw-rw-   0        0        0      819 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/discovery/ocel/interleavings/utils/__init__.py
+-rw-rw-rw-   0        0        0     4451 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/discovery/ocel/interleavings/utils/merge_dataframe_rel_cases.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:32.371023 pm4pyminimal-2.7.9.4/pm4py/algo/discovery/ocel/interleavings/variants/
+-rw-rw-rw-   0        0        0      820 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/discovery/ocel/interleavings/variants/__init__.py
+-rw-rw-rw-   0        0        0     6643 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/discovery/ocel/interleavings/variants/timestamp_interleavings.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:32.371023 pm4pyminimal-2.7.9.4/pm4py/algo/discovery/ocel/link_analysis/
+-rw-rw-rw-   0        0        0      796 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/discovery/ocel/link_analysis/__init__.py
+-rw-rw-rw-   0        0        0     1841 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/discovery/ocel/link_analysis/algorithm.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:32.371023 pm4pyminimal-2.7.9.4/pm4py/algo/discovery/ocel/link_analysis/variants/
+-rw-rw-rw-   0        0        0      804 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/discovery/ocel/link_analysis/variants/__init__.py
+-rw-rw-rw-   0        0        0     6519 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/discovery/ocel/link_analysis/variants/classic.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:32.386645 pm4pyminimal-2.7.9.4/pm4py/algo/discovery/ocel/ocdfg/
+-rw-rw-rw-   0        0        0      799 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/discovery/ocel/ocdfg/__init__.py
+-rw-rw-rw-   0        0        0     1775 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/discovery/ocel/ocdfg/algorithm.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:32.386645 pm4pyminimal-2.7.9.4/pm4py/algo/discovery/ocel/ocdfg/variants/
+-rw-rw-rw-   0        0        0      796 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/discovery/ocel/ocdfg/variants/__init__.py
+-rw-rw-rw-   0        0        0     8817 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/discovery/ocel/ocdfg/variants/classic.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:32.386645 pm4pyminimal-2.7.9.4/pm4py/algo/discovery/ocel/ocpn/
+-rw-rw-rw-   0        0        0      798 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/discovery/ocel/ocpn/__init__.py
+-rw-rw-rw-   0        0        0     1785 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/discovery/ocel/ocpn/algorithm.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:32.403406 pm4pyminimal-2.7.9.4/pm4py/algo/discovery/ocel/ocpn/variants/
+-rw-rw-rw-   0        0        0      797 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/discovery/ocel/ocpn/variants/__init__.py
+-rw-rw-rw-   0        0        0    10290 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/discovery/ocel/ocpn/variants/classic.py
+-rw-rw-rw-   0        0        0      812 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/discovery/ocel/ocpn/variants/wo_annotation.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:32.403406 pm4pyminimal-2.7.9.4/pm4py/algo/discovery/ocel/saw_nets/
+-rw-rw-rw-   0        0        0      804 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/discovery/ocel/saw_nets/__init__.py
+-rw-rw-rw-   0        0        0     1800 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/discovery/ocel/saw_nets/algorithm.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:32.403406 pm4pyminimal-2.7.9.4/pm4py/algo/discovery/ocel/saw_nets/variants/
+-rw-rw-rw-   0        0        0      801 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/discovery/ocel/saw_nets/variants/__init__.py
+-rw-rw-rw-   0        0        0     7569 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/discovery/ocel/saw_nets/variants/classic.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:32.403406 pm4pyminimal-2.7.9.4/pm4py/algo/discovery/performance_spectrum/
+-rw-rw-rw-   0        0        0      809 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/discovery/performance_spectrum/__init__.py
+-rw-rw-rw-   0        0        0     3495 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/discovery/performance_spectrum/algorithm.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:32.419028 pm4pyminimal-2.7.9.4/pm4py/algo/discovery/performance_spectrum/variants/
+-rw-rw-rw-   0        0        0      855 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/discovery/performance_spectrum/variants/__init__.py
+-rw-rw-rw-   0        0        0     4317 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/discovery/performance_spectrum/variants/dataframe.py
+-rw-rw-rw-   0        0        0     4970 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/discovery/performance_spectrum/variants/dataframe_disconnected.py
+-rw-rw-rw-   0        0        0     3382 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/discovery/performance_spectrum/variants/log.py
+-rw-rw-rw-   0        0        0     4366 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/discovery/performance_spectrum/variants/log_disconnected.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:32.419028 pm4pyminimal-2.7.9.4/pm4py/algo/discovery/powl/
+-rw-rw-rw-   0        0        0      779 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/discovery/powl/__init__.py
+-rw-rw-rw-   0        0        0     3201 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/discovery/powl/algorithm.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:32.434651 pm4pyminimal-2.7.9.4/pm4py/algo/discovery/powl/inductive/
+-rw-rw-rw-   0        0        0      787 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/discovery/powl/inductive/__init__.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:32.434651 pm4pyminimal-2.7.9.4/pm4py/algo/discovery/powl/inductive/base_case/
+-rw-rw-rw-   0        0        0      797 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/discovery/powl/inductive/base_case/__init__.py
+-rw-rw-rw-   0        0        0     1506 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/discovery/powl/inductive/base_case/abc.py
+-rw-rw-rw-   0        0        0     1457 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/discovery/powl/inductive/base_case/empty_log.py
+-rw-rw-rw-   0        0        0     1867 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/discovery/powl/inductive/base_case/factory.py
+-rw-rw-rw-   0        0        0     1547 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/discovery/powl/inductive/base_case/single_activity.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:32.455280 pm4pyminimal-2.7.9.4/pm4py/algo/discovery/powl/inductive/cuts/
+-rw-rw-rw-   0        0        0      792 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/discovery/powl/inductive/cuts/__init__.py
+-rw-rw-rw-   0        0        0     1361 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/discovery/powl/inductive/cuts/concurrency.py
+-rw-rw-rw-   0        0        0     1974 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/discovery/powl/inductive/cuts/factory.py
+-rw-rw-rw-   0        0        0     1353 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/discovery/powl/inductive/cuts/loop.py
+-rw-rw-rw-   0        0        0     1975 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/discovery/powl/inductive/cuts/sequence.py
+-rw-rw-rw-   0        0        0     1433 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/discovery/powl/inductive/cuts/xor.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:32.470909 pm4pyminimal-2.7.9.4/pm4py/algo/discovery/powl/inductive/fall_through/
+-rw-rw-rw-   0        0        0      798 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/discovery/powl/inductive/fall_through/__init__.py
+-rw-rw-rw-   0        0        0     1905 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/discovery/powl/inductive/fall_through/activity_concurrent.py
+-rw-rw-rw-   0        0        0     1056 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/discovery/powl/inductive/fall_through/activity_once_per_trace.py
+-rw-rw-rw-   0        0        0     1795 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/discovery/powl/inductive/fall_through/empty_traces.py
+-rw-rw-rw-   0        0        0     2498 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/discovery/powl/inductive/fall_through/factory.py
+-rw-rw-rw-   0        0        0     1814 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/discovery/powl/inductive/fall_through/flower.py
+-rw-rw-rw-   0        0        0     1651 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/discovery/powl/inductive/fall_through/strict_tau_loop.py
+-rw-rw-rw-   0        0        0     1630 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/discovery/powl/inductive/fall_through/tau_loop.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:32.470909 pm4pyminimal-2.7.9.4/pm4py/algo/discovery/powl/inductive/utils/
+-rw-rw-rw-   0        0        0      734 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/discovery/powl/inductive/utils/__init__.py
+-rw-rw-rw-   0        0        0     2008 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/discovery/powl/inductive/utils/filtering.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:32.486529 pm4pyminimal-2.7.9.4/pm4py/algo/discovery/powl/inductive/variants/
+-rw-rw-rw-   0        0        0      798 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/discovery/powl/inductive/variants/__init__.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:32.502159 pm4pyminimal-2.7.9.4/pm4py/algo/discovery/powl/inductive/variants/brute_force/
+-rw-rw-rw-   0        0        0      806 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/discovery/powl/inductive/variants/brute_force/__init__.py
+-rw-rw-rw-   0        0        0     7020 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/discovery/powl/inductive/variants/brute_force/bf_partial_order_cut.py
+-rw-rw-rw-   0        0        0     2195 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/discovery/powl/inductive/variants/brute_force/factory.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:32.512763 pm4pyminimal-2.7.9.4/pm4py/algo/discovery/powl/inductive/variants/dynamic_clustering/
+-rw-rw-rw-   0        0        0      813 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/discovery/powl/inductive/variants/dynamic_clustering/__init__.py
+-rw-rw-rw-   0        0        0     7347 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/discovery/powl/inductive/variants/dynamic_clustering/dynamic_clustering_partial_order_cut.py
+-rw-rw-rw-   0        0        0     2043 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/discovery/powl/inductive/variants/dynamic_clustering/factory.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:32.512763 pm4pyminimal-2.7.9.4/pm4py/algo/discovery/powl/inductive/variants/dynamic_clustering_frequency/
+-rw-rw-rw-   0        0        0      823 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/discovery/powl/inductive/variants/dynamic_clustering_frequency/__init__.py
+-rw-rw-rw-   0        0        0     8397 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/discovery/powl/inductive/variants/dynamic_clustering_frequency/dynamic_clustering_frequency_partial_order_cut.py
+-rw-rw-rw-   0        0        0     2099 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/discovery/powl/inductive/variants/dynamic_clustering_frequency/factory.py
+-rw-rw-rw-   0        0        0     1482 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/discovery/powl/inductive/variants/im_brute_force.py
+-rw-rw-rw-   0        0        0     1643 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/discovery/powl/inductive/variants/im_dynamic_clustering.py
+-rw-rw-rw-   0        0        0     1687 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/discovery/powl/inductive/variants/im_dynamic_clustering_frequencies.py
+-rw-rw-rw-   0        0        0     1468 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/discovery/powl/inductive/variants/im_maximal.py
+-rw-rw-rw-   0        0        0     5456 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/discovery/powl/inductive/variants/im_tree.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:32.512763 pm4pyminimal-2.7.9.4/pm4py/algo/discovery/powl/inductive/variants/maximal/
+-rw-rw-rw-   0        0        0      800 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/discovery/powl/inductive/variants/maximal/__init__.py
+-rw-rw-rw-   0        0        0     2373 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/discovery/powl/inductive/variants/maximal/factory.py
+-rw-rw-rw-   0        0        0     7192 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/discovery/powl/inductive/variants/maximal/maximal_partial_order_cut.py
+-rw-rw-rw-   0        0        0      936 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/discovery/powl/inductive/variants/powl_discovery_varaints.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:32.528390 pm4pyminimal-2.7.9.4/pm4py/algo/discovery/temporal_profile/
+-rw-rw-rw-   0        0        0      805 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/discovery/temporal_profile/__init__.py
+-rw-rw-rw-   0        0        0     2006 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/discovery/temporal_profile/algorithm.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:32.528390 pm4pyminimal-2.7.9.4/pm4py/algo/discovery/temporal_profile/variants/
+-rw-rw-rw-   0        0        0      809 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/discovery/temporal_profile/variants/__init__.py
+-rw-rw-rw-   0        0        0     4044 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/discovery/temporal_profile/variants/dataframe.py
+-rw-rw-rw-   0        0        0     5236 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/discovery/temporal_profile/variants/log.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:32.544010 pm4pyminimal-2.7.9.4/pm4py/algo/discovery/transition_system/
+-rw-rw-rw-   0        0        0      806 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/discovery/transition_system/__init__.py
+-rw-rw-rw-   0        0        0     1984 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/discovery/transition_system/algorithm.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:32.544010 pm4pyminimal-2.7.9.4/pm4py/algo/discovery/transition_system/variants/
+-rw-rw-rw-   0        0        0      806 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/discovery/transition_system/variants/__init__.py
+-rw-rw-rw-   0        0        0     5956 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/discovery/transition_system/variants/view_based.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:32.555519 pm4pyminimal-2.7.9.4/pm4py/algo/evaluation/
+-rw-rw-rw-   0        0        0      836 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/evaluation/__init__.py
+-rw-rw-rw-   0        0        0     4819 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/evaluation/algorithm.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:32.555519 pm4pyminimal-2.7.9.4/pm4py/algo/evaluation/earth_mover_distance/
+-rw-rw-rw-   0        0        0      995 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/evaluation/earth_mover_distance/__init__.py
+-rw-rw-rw-   0        0        0     1678 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/evaluation/earth_mover_distance/algorithm.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:32.555519 pm4pyminimal-2.7.9.4/pm4py/algo/evaluation/earth_mover_distance/variants/
+-rw-rw-rw-   0        0        0      805 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/evaluation/earth_mover_distance/variants/__init__.py
+-rw-rw-rw-   0        0        0     4864 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/evaluation/earth_mover_distance/variants/pyemd.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:32.571147 pm4pyminimal-2.7.9.4/pm4py/algo/evaluation/generalization/
+-rw-rw-rw-   0        0        0      804 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/evaluation/generalization/__init__.py
+-rw-rw-rw-   0        0        0     1703 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/evaluation/generalization/algorithm.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:32.571147 pm4pyminimal-2.7.9.4/pm4py/algo/evaluation/generalization/variants/
+-rw-rw-rw-   0        0        0      805 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/evaluation/generalization/variants/__init__.py
+-rw-rw-rw-   0        0        0     2285 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/evaluation/generalization/variants/token_based.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:32.571147 pm4pyminimal-2.7.9.4/pm4py/algo/evaluation/precision/
+-rw-rw-rw-   0        0        0      811 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/evaluation/precision/__init__.py
+-rw-rw-rw-   0        0        0     2994 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/evaluation/precision/algorithm.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:32.586769 pm4pyminimal-2.7.9.4/pm4py/algo/evaluation/precision/dfg/
+-rw-rw-rw-   0        0        0      793 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/evaluation/precision/dfg/__init__.py
+-rw-rw-rw-   0        0        0     3992 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/evaluation/precision/dfg/algorithm.py
+-rw-rw-rw-   0        0        0     5525 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/evaluation/precision/utils.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:32.586769 pm4pyminimal-2.7.9.4/pm4py/algo/evaluation/precision/variants/
+-rw-rw-rw-   0        0        0      829 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/evaluation/precision/variants/__init__.py
+-rw-rw-rw-   0        0        0    13806 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/evaluation/precision/variants/align_etconformance.py
+-rw-rw-rw-   0        0        0     6199 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/evaluation/precision/variants/etconformance_token.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:32.586769 pm4pyminimal-2.7.9.4/pm4py/algo/evaluation/replay_fitness/
+-rw-rw-rw-   0        0        0      804 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/evaluation/replay_fitness/__init__.py
+-rw-rw-rw-   0        0        0     4486 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/evaluation/replay_fitness/algorithm.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:32.602388 pm4pyminimal-2.7.9.4/pm4py/algo/evaluation/replay_fitness/variants/
+-rw-rw-rw-   0        0        0      823 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/evaluation/replay_fitness/variants/__init__.py
+-rw-rw-rw-   0        0        0     6788 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/evaluation/replay_fitness/variants/alignment_based.py
+-rw-rw-rw-   0        0        0     5159 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/evaluation/replay_fitness/variants/token_replay.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:32.602388 pm4pyminimal-2.7.9.4/pm4py/algo/evaluation/simplicity/
+-rw-rw-rw-   0        0        0      802 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/evaluation/simplicity/__init__.py
+-rw-rw-rw-   0        0        0     1585 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/evaluation/simplicity/algorithm.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:32.618010 pm4pyminimal-2.7.9.4/pm4py/algo/evaluation/simplicity/variants/
+-rw-rw-rw-   0        0        0      841 2024-01-17 08:27:47.000000 pm4pyminimal-2.7.9.4/pm4py/algo/evaluation/simplicity/variants/__init__.py
+-rw-rw-rw-   0        0        0     2696 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/algo/evaluation/simplicity/variants/arc_degree.py
+-rw-rw-rw-   0        0        0     1602 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/algo/evaluation/simplicity/variants/extended_cardoso.py
+-rw-rw-rw-   0        0        0     2120 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/algo/evaluation/simplicity/variants/extended_cyclomatic.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:32.618010 pm4pyminimal-2.7.9.4/pm4py/algo/filtering/
+-rw-rw-rw-   0        0        0      734 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/algo/filtering/__init__.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:32.618010 pm4pyminimal-2.7.9.4/pm4py/algo/filtering/common/
+-rw-rw-rw-   0        0        0      852 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/algo/filtering/common/__init__.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:32.618010 pm4pyminimal-2.7.9.4/pm4py/algo/filtering/common/attributes/
+-rw-rw-rw-   0        0        0      734 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/algo/filtering/common/attributes/__init__.py
+-rw-rw-rw-   0        0        0      951 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/algo/filtering/common/attributes/attributes_common.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:32.633631 pm4pyminimal-2.7.9.4/pm4py/algo/filtering/common/end_activities/
+-rw-rw-rw-   0        0        0      812 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/algo/filtering/common/end_activities/__init__.py
+-rw-rw-rw-   0        0        0      851 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/algo/filtering/common/end_activities/end_activities_common.py
+-rw-rw-rw-   0        0        0      845 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/algo/filtering/common/filtering_constants.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:32.633631 pm4pyminimal-2.7.9.4/pm4py/algo/filtering/common/start_activities/
+-rw-rw-rw-   0        0        0      816 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/algo/filtering/common/start_activities/__init__.py
+-rw-rw-rw-   0        0        0      857 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/algo/filtering/common/start_activities/start_activities_common.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:32.633631 pm4pyminimal-2.7.9.4/pm4py/algo/filtering/common/timestamp/
+-rw-rw-rw-   0        0        0      734 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/algo/filtering/common/timestamp/__init__.py
+-rw-rw-rw-   0        0        0     1250 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/algo/filtering/common/timestamp/timestamp_common.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:32.633631 pm4pyminimal-2.7.9.4/pm4py/algo/filtering/common/traces/
+-rw-rw-rw-   0        0        0      734 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/algo/filtering/common/traces/__init__.py
+-rw-rw-rw-   0        0        0     1246 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/algo/filtering/common/traces/infix_to_regex.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:32.649252 pm4pyminimal-2.7.9.4/pm4py/algo/filtering/dfg/
+-rw-rw-rw-   0        0        0      734 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/algo/filtering/dfg/__init__.py
+-rw-rw-rw-   0        0        0    25920 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/algo/filtering/dfg/dfg_filtering.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:32.649252 pm4pyminimal-2.7.9.4/pm4py/algo/filtering/log/
+-rw-rw-rw-   0        0        0      866 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/algo/filtering/log/__init__.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:32.655758 pm4pyminimal-2.7.9.4/pm4py/algo/filtering/log/attr_value_repetition/
+-rw-rw-rw-   0        0        0      994 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/algo/filtering/log/attr_value_repetition/__init__.py
+-rw-rw-rw-   0        0        0     2754 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/algo/filtering/log/attr_value_repetition/filter.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:32.655758 pm4pyminimal-2.7.9.4/pm4py/algo/filtering/log/attributes/
+-rw-rw-rw-   0        0        0      801 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/algo/filtering/log/attributes/__init__.py
+-rw-rw-rw-   0        0        0    18308 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/algo/filtering/log/attributes/attributes_filter.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:32.655758 pm4pyminimal-2.7.9.4/pm4py/algo/filtering/log/between/
+-rw-rw-rw-   0        0        0      795 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/algo/filtering/log/between/__init__.py
+-rw-rw-rw-   0        0        0     2944 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/algo/filtering/log/between/between_filter.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:32.655758 pm4pyminimal-2.7.9.4/pm4py/algo/filtering/log/cases/
+-rw-rw-rw-   0        0        0      790 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/algo/filtering/log/cases/__init__.py
+-rw-rw-rw-   0        0        0     4597 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/algo/filtering/log/cases/case_filter.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:32.673383 pm4pyminimal-2.7.9.4/pm4py/algo/filtering/log/end_activities/
+-rw-rw-rw-   0        0        0      809 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/algo/filtering/log/end_activities/__init__.py
+-rw-rw-rw-   0        0        0     3719 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/algo/filtering/log/end_activities/end_activities_filter.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:32.678247 pm4pyminimal-2.7.9.4/pm4py/algo/filtering/log/ltl/
+-rw-rw-rw-   0        0        0      788 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/algo/filtering/log/ltl/__init__.py
+-rw-rw-rw-   0        0        0    11094 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/algo/filtering/log/ltl/ltl_checker.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:32.678247 pm4pyminimal-2.7.9.4/pm4py/algo/filtering/log/paths/
+-rw-rw-rw-   0        0        0      791 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/algo/filtering/log/paths/__init__.py
+-rw-rw-rw-   0        0        0     9660 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/algo/filtering/log/paths/paths_filter.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:32.678247 pm4pyminimal-2.7.9.4/pm4py/algo/filtering/log/prefixes/
+-rw-rw-rw-   0        0        0      797 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/algo/filtering/log/prefixes/__init__.py
+-rw-rw-rw-   0        0        0     3218 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/algo/filtering/log/prefixes/prefix_filter.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:32.678247 pm4pyminimal-2.7.9.4/pm4py/algo/filtering/log/rework/
+-rw-rw-rw-   0        0        0      793 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/algo/filtering/log/rework/__init__.py
+-rw-rw-rw-   0        0        0     3412 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/algo/filtering/log/rework/rework_filter.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:32.693875 pm4pyminimal-2.7.9.4/pm4py/algo/filtering/log/start_activities/
+-rw-rw-rw-   0        0        0      813 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/algo/filtering/log/start_activities/__init__.py
+-rw-rw-rw-   0        0        0     3950 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/algo/filtering/log/start_activities/start_activities_filter.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:32.693875 pm4pyminimal-2.7.9.4/pm4py/algo/filtering/log/suffixes/
+-rw-rw-rw-   0        0        0      797 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/algo/filtering/log/suffixes/__init__.py
+-rw-rw-rw-   0        0        0     3223 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/algo/filtering/log/suffixes/suffix_filter.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:32.693875 pm4pyminimal-2.7.9.4/pm4py/algo/filtering/log/timestamp/
+-rw-rw-rw-   0        0        0      799 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/algo/filtering/log/timestamp/__init__.py
+-rw-rw-rw-   0        0        0    11509 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/algo/filtering/log/timestamp/timestamp_filter.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:32.693875 pm4pyminimal-2.7.9.4/pm4py/algo/filtering/log/traces/
+-rw-rw-rw-   0        0        0      734 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/algo/filtering/log/traces/__init__.py
+-rw-rw-rw-   0        0        0     3785 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/algo/filtering/log/traces/trace_filter.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:32.709497 pm4pyminimal-2.7.9.4/pm4py/algo/filtering/log/variants/
+-rw-rw-rw-   0        0        0      797 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/algo/filtering/log/variants/__init__.py
+-rw-rw-rw-   0        0        0     9002 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/algo/filtering/log/variants/variants_filter.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:32.709497 pm4pyminimal-2.7.9.4/pm4py/algo/filtering/ocel/
+-rw-rw-rw-   0        0        0      865 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/algo/filtering/ocel/__init__.py
+-rw-rw-rw-   0        0        0     3392 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/algo/filtering/ocel/activity_type_matching.py
+-rw-rw-rw-   0        0        0     3843 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/algo/filtering/ocel/event_attributes.py
+-rw-rw-rw-   0        0        0     2319 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/algo/filtering/ocel/object_attributes.py
+-rw-rw-rw-   0        0        0     3436 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/algo/filtering/ocel/objects_ot_count.py
+-rw-rw-rw-   0        0        0     4195 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/algo/filtering/ocel/ot_endpoints.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:32.725118 pm4pyminimal-2.7.9.4/pm4py/algo/filtering/pandas/
+-rw-rw-rw-   0        0        0      891 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/algo/filtering/pandas/__init__.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:32.725118 pm4pyminimal-2.7.9.4/pm4py/algo/filtering/pandas/attr_value_repetition/
+-rw-rw-rw-   0        0        0      997 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/algo/filtering/pandas/attr_value_repetition/__init__.py
+-rw-rw-rw-   0        0        0     2786 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/algo/filtering/pandas/attr_value_repetition/filter.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:32.725118 pm4pyminimal-2.7.9.4/pm4py/algo/filtering/pandas/attributes/
+-rw-rw-rw-   0        0        0      734 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/algo/filtering/pandas/attributes/__init__.py
+-rw-rw-rw-   0        0        0    13156 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/algo/filtering/pandas/attributes/attributes_filter.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:32.740739 pm4pyminimal-2.7.9.4/pm4py/algo/filtering/pandas/between/
+-rw-rw-rw-   0        0        0      798 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/algo/filtering/pandas/between/__init__.py
+-rw-rw-rw-   0        0        0     3266 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/algo/filtering/pandas/between/between_filter.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:32.740739 pm4pyminimal-2.7.9.4/pm4py/algo/filtering/pandas/cases/
+-rw-rw-rw-   0        0        0      793 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/algo/filtering/pandas/cases/__init__.py
+-rw-rw-rw-   0        0        0     6322 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/algo/filtering/pandas/cases/case_filter.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:32.740739 pm4pyminimal-2.7.9.4/pm4py/algo/filtering/pandas/consecutive_act_case_grouping/
+-rw-rw-rw-   0        0        0      842 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/algo/filtering/pandas/consecutive_act_case_grouping/__init__.py
+-rw-rw-rw-   0        0        0     3077 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/algo/filtering/pandas/consecutive_act_case_grouping/consecutive_act_case_grouping_filter.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:32.740739 pm4pyminimal-2.7.9.4/pm4py/algo/filtering/pandas/end_activities/
+-rw-rw-rw-   0        0        0      812 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/algo/filtering/pandas/end_activities/__init__.py
+-rw-rw-rw-   0        0        0     6142 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/algo/filtering/pandas/end_activities/end_activities_filter.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:32.755748 pm4pyminimal-2.7.9.4/pm4py/algo/filtering/pandas/ends_with/
+-rw-rw-rw-   0        0        0      734 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/algo/filtering/pandas/ends_with/__init__.py
+-rw-rw-rw-   0        0        0     3508 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/algo/filtering/pandas/ends_with/ends_with_filter.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:32.755748 pm4pyminimal-2.7.9.4/pm4py/algo/filtering/pandas/ltl/
+-rw-rw-rw-   0        0        0      791 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/algo/filtering/pandas/ltl/__init__.py
+-rw-rw-rw-   0        0        0    11763 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/algo/filtering/pandas/ltl/ltl_checker.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:32.755748 pm4pyminimal-2.7.9.4/pm4py/algo/filtering/pandas/paths/
+-rw-rw-rw-   0        0        0      794 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/algo/filtering/pandas/paths/__init__.py
+-rw-rw-rw-   0        0        0     6919 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/algo/filtering/pandas/paths/paths_filter.py
+-rw-rw-rw-   0        0        0      832 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/algo/filtering/pandas/pd_filtering_constants.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:32.755748 pm4pyminimal-2.7.9.4/pm4py/algo/filtering/pandas/prefixes/
+-rw-rw-rw-   0        0        0      800 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/algo/filtering/pandas/prefixes/__init__.py
+-rw-rw-rw-   0        0        0     3950 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/algo/filtering/pandas/prefixes/prefix_filter.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:32.776663 pm4pyminimal-2.7.9.4/pm4py/algo/filtering/pandas/rework/
+-rw-rw-rw-   0        0        0      796 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/algo/filtering/pandas/rework/__init__.py
+-rw-rw-rw-   0        0        0     3425 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/algo/filtering/pandas/rework/rework_filter.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:32.777671 pm4pyminimal-2.7.9.4/pm4py/algo/filtering/pandas/start_activities/
+-rw-rw-rw-   0        0        0      816 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/algo/filtering/pandas/start_activities/__init__.py
+-rw-rw-rw-   0        0        0     5585 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/algo/filtering/pandas/start_activities/start_activities_filter.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:32.777671 pm4pyminimal-2.7.9.4/pm4py/algo/filtering/pandas/starts_with/
+-rw-rw-rw-   0        0        0      734 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/algo/filtering/pandas/starts_with/__init__.py
+-rw-rw-rw-   0        0        0     3510 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/algo/filtering/pandas/starts_with/starts_with_filter.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:32.777671 pm4pyminimal-2.7.9.4/pm4py/algo/filtering/pandas/suffixes/
+-rw-rw-rw-   0        0        0      736 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/algo/filtering/pandas/suffixes/__init__.py
+-rw-rw-rw-   0        0        0     3950 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/algo/filtering/pandas/suffixes/suffix_filter.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:32.777671 pm4pyminimal-2.7.9.4/pm4py/algo/filtering/pandas/timestamp/
+-rw-rw-rw-   0        0        0      802 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/algo/filtering/pandas/timestamp/__init__.py
+-rw-rw-rw-   0        0        0     8208 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/algo/filtering/pandas/timestamp/timestamp_filter.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:32.793297 pm4pyminimal-2.7.9.4/pm4py/algo/filtering/pandas/timestamp_case_grouping/
+-rw-rw-rw-   0        0        0      830 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/algo/filtering/pandas/timestamp_case_grouping/__init__.py
+-rw-rw-rw-   0        0        0     3499 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/algo/filtering/pandas/timestamp_case_grouping/timestamp_case_grouping_filter.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:32.793297 pm4pyminimal-2.7.9.4/pm4py/algo/filtering/pandas/traces/
+-rw-rw-rw-   0        0        0      736 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/algo/filtering/pandas/traces/__init__.py
+-rw-rw-rw-   0        0        0     3604 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/algo/filtering/pandas/traces/trace_filter.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:32.793297 pm4pyminimal-2.7.9.4/pm4py/algo/filtering/pandas/variants/
+-rw-rw-rw-   0        0        0      734 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/algo/filtering/pandas/variants/__init__.py
+-rw-rw-rw-   0        0        0     6083 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/algo/filtering/pandas/variants/variants_filter.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:32.793297 pm4pyminimal-2.7.9.4/pm4py/algo/label_splitting/
+-rw-rw-rw-   0        0        0      794 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/algo/label_splitting/__init__.py
+-rw-rw-rw-   0        0        0     1921 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/algo/label_splitting/algorithm.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:32.811105 pm4pyminimal-2.7.9.4/pm4py/algo/label_splitting/variants/
+-rw-rw-rw-   0        0        0      794 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/algo/label_splitting/variants/__init__.py
+-rw-rw-rw-   0        0        0     9446 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/algo/label_splitting/variants/contextual.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:32.811105 pm4pyminimal-2.7.9.4/pm4py/algo/merging/
+-rw-rw-rw-   0        0        0      781 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/algo/merging/__init__.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:32.811105 pm4pyminimal-2.7.9.4/pm4py/algo/merging/case_relations/
+-rw-rw-rw-   0        0        0      801 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/algo/merging/case_relations/__init__.py
+-rw-rw-rw-   0        0        0     2326 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/algo/merging/case_relations/algorithm.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:32.811105 pm4pyminimal-2.7.9.4/pm4py/algo/merging/case_relations/variants/
+-rw-rw-rw-   0        0        0      797 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/algo/merging/case_relations/variants/__init__.py
+-rw-rw-rw-   0        0        0     3498 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/algo/merging/case_relations/variants/pandas.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:32.826727 pm4pyminimal-2.7.9.4/pm4py/algo/organizational_mining/
+-rw-rw-rw-   0        0        0      855 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/algo/organizational_mining/__init__.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:32.826727 pm4pyminimal-2.7.9.4/pm4py/algo/organizational_mining/local_diagnostics/
+-rw-rw-rw-   0        0        0      808 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/algo/organizational_mining/local_diagnostics/__init__.py
+-rw-rw-rw-   0        0        0    12440 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/algo/organizational_mining/local_diagnostics/algorithm.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:32.826727 pm4pyminimal-2.7.9.4/pm4py/algo/organizational_mining/network_analysis/
+-rw-rw-rw-   0        0        0      817 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/algo/organizational_mining/network_analysis/__init__.py
+-rw-rw-rw-   0        0        0     1840 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/algo/organizational_mining/network_analysis/algorithm.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:32.826727 pm4pyminimal-2.7.9.4/pm4py/algo/organizational_mining/network_analysis/variants/
+-rw-rw-rw-   0        0        0      816 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/algo/organizational_mining/network_analysis/variants/__init__.py
+-rw-rw-rw-   0        0        0    10562 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/algo/organizational_mining/network_analysis/variants/dataframe.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:32.842348 pm4pyminimal-2.7.9.4/pm4py/algo/organizational_mining/resource_profiles/
+-rw-rw-rw-   0        0        0      818 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/algo/organizational_mining/resource_profiles/__init__.py
+-rw-rw-rw-   0        0        0    12251 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/algo/organizational_mining/resource_profiles/algorithm.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:32.842348 pm4pyminimal-2.7.9.4/pm4py/algo/organizational_mining/resource_profiles/variants/
+-rw-rw-rw-   0        0        0      819 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/algo/organizational_mining/resource_profiles/variants/__init__.py
+-rw-rw-rw-   0        0        0    23271 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/algo/organizational_mining/resource_profiles/variants/log.py
+-rw-rw-rw-   0        0        0    23967 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/algo/organizational_mining/resource_profiles/variants/pandas.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:32.842348 pm4pyminimal-2.7.9.4/pm4py/algo/organizational_mining/roles/
+-rw-rw-rw-   0        0        0      814 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/algo/organizational_mining/roles/__init__.py
+-rw-rw-rw-   0        0        0     2427 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/algo/organizational_mining/roles/algorithm.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:32.855859 pm4pyminimal-2.7.9.4/pm4py/algo/organizational_mining/roles/common/
+-rw-rw-rw-   0        0        0      803 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/algo/organizational_mining/roles/common/__init__.py
+-rw-rw-rw-   0        0        0     8411 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/algo/organizational_mining/roles/common/algorithm.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:32.855859 pm4pyminimal-2.7.9.4/pm4py/algo/organizational_mining/roles/variants/
+-rw-rw-rw-   0        0        0      807 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/algo/organizational_mining/roles/variants/__init__.py
+-rw-rw-rw-   0        0        0     2448 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/algo/organizational_mining/roles/variants/log.py
+-rw-rw-rw-   0        0        0     2213 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/algo/organizational_mining/roles/variants/pandas.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:32.855859 pm4pyminimal-2.7.9.4/pm4py/algo/organizational_mining/sna/
+-rw-rw-rw-   0        0        0      810 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/algo/organizational_mining/sna/__init__.py
+-rw-rw-rw-   0        0        0     3689 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/algo/organizational_mining/sna/algorithm.py
+-rw-rw-rw-   0        0        0     3199 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/algo/organizational_mining/sna/util.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:32.872741 pm4pyminimal-2.7.9.4/pm4py/algo/organizational_mining/sna/variants/
+-rw-rw-rw-   0        0        0      805 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/algo/organizational_mining/sna/variants/__init__.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:32.888363 pm4pyminimal-2.7.9.4/pm4py/algo/organizational_mining/sna/variants/log/
+-rw-rw-rw-   0        0        0      857 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/algo/organizational_mining/sna/variants/log/__init__.py
+-rw-rw-rw-   0        0        0     3735 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/algo/organizational_mining/sna/variants/log/handover.py
+-rw-rw-rw-   0        0        0     3286 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/algo/organizational_mining/sna/variants/log/jointactivities.py
+-rw-rw-rw-   0        0        0     3525 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/algo/organizational_mining/sna/variants/log/subcontracting.py
+-rw-rw-rw-   0        0        0     3155 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/algo/organizational_mining/sna/variants/log/working_together.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:32.888363 pm4pyminimal-2.7.9.4/pm4py/algo/organizational_mining/sna/variants/pandas/
+-rw-rw-rw-   0        0        0      860 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/algo/organizational_mining/sna/variants/pandas/__init__.py
+-rw-rw-rw-   0        0        0     4235 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/algo/organizational_mining/sna/variants/pandas/handover.py
+-rw-rw-rw-   0        0        0     2998 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/algo/organizational_mining/sna/variants/pandas/jointactivities.py
+-rw-rw-rw-   0        0        0     3804 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/algo/organizational_mining/sna/variants/pandas/subcontracting.py
+-rw-rw-rw-   0        0        0     3432 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/algo/organizational_mining/sna/variants/pandas/working_together.py
+-rw-rw-rw-   0        0        0     7667 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/algo/organizational_mining/util.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:32.888363 pm4pyminimal-2.7.9.4/pm4py/algo/querying/
+-rw-rw-rw-   0        0        0      736 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/algo/querying/__init__.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:32.903984 pm4pyminimal-2.7.9.4/pm4py/algo/querying/llm/
+-rw-rw-rw-   0        0        0      798 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/algo/querying/llm/__init__.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:32.935228 pm4pyminimal-2.7.9.4/pm4py/algo/querying/llm/abstractions/
+-rw-rw-rw-   0        0        0      960 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/algo/querying/llm/abstractions/__init__.py
+-rw-rw-rw-   0        0        0     4006 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/algo/querying/llm/abstractions/case_to_descr.py
+-rw-rw-rw-   0        0        0     4382 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/algo/querying/llm/abstractions/declare_to_descr.py
+-rw-rw-rw-   0        0        0     3100 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/algo/querying/llm/abstractions/log_to_cols_descr.py
+-rw-rw-rw-   0        0        0     9696 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/algo/querying/llm/abstractions/log_to_dfg_descr.py
+-rw-rw-rw-   0        0        0     7886 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/algo/querying/llm/abstractions/log_to_fea_descr.py
+-rw-rw-rw-   0        0        0    10693 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/algo/querying/llm/abstractions/log_to_variants_descr.py
+-rw-rw-rw-   0        0        0     3241 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/algo/querying/llm/abstractions/logske_to_descr.py
+-rw-rw-rw-   0        0        0     1931 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/algo/querying/llm/abstractions/net_to_descr.py
+-rw-rw-rw-   0        0        0     6145 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/algo/querying/llm/abstractions/ocel_fea_descr.py
+-rw-rw-rw-   0        0        0     3680 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/algo/querying/llm/abstractions/ocel_ocdfg_descr.py
+-rw-rw-rw-   0        0        0     3004 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/algo/querying/llm/abstractions/stream_to_descr.py
+-rw-rw-rw-   0        0        0     2481 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/algo/querying/llm/abstractions/tempprofile_to_descr.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:32.935228 pm4pyminimal-2.7.9.4/pm4py/algo/querying/llm/connectors/
+-rw-rw-rw-   0        0        0      791 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/algo/querying/llm/connectors/__init__.py
+-rw-rw-rw-   0        0        0     2596 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/algo/querying/llm/connectors/openai.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:32.950849 pm4pyminimal-2.7.9.4/pm4py/algo/querying/llm/utils/
+-rw-rw-rw-   0        0        0      787 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/algo/querying/llm/utils/__init__.py
+-rw-rw-rw-   0        0        0     1634 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/algo/querying/llm/utils/sql_utils.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:32.955859 pm4pyminimal-2.7.9.4/pm4py/algo/reduction/
+-rw-rw-rw-   0        0        0      955 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/algo/reduction/__init__.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:32.960870 pm4pyminimal-2.7.9.4/pm4py/algo/reduction/process_tree/
+-rw-rw-rw-   0        0        0      799 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/algo/reduction/process_tree/__init__.py
+-rw-rw-rw-   0        0        0     1601 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/algo/reduction/process_tree/reducer.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:32.960870 pm4pyminimal-2.7.9.4/pm4py/algo/reduction/process_tree/variants/
+-rw-rw-rw-   0        0        0      804 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/algo/reduction/process_tree/variants/__init__.py
+-rw-rw-rw-   0        0        0     3743 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/algo/reduction/process_tree/variants/tree_tr_based.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:32.960870 pm4pyminimal-2.7.9.4/pm4py/algo/simulation/
+-rw-rw-rw-   0        0        0      904 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/algo/simulation/__init__.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:32.976484 pm4pyminimal-2.7.9.4/pm4py/algo/simulation/montecarlo/
+-rw-rw-rw-   0        0        0      995 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/algo/simulation/montecarlo/__init__.py
+-rw-rw-rw-   0        0        0     4562 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/algo/simulation/montecarlo/algorithm.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:32.976484 pm4pyminimal-2.7.9.4/pm4py/algo/simulation/montecarlo/utils/
+-rw-rw-rw-   0        0        0      793 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/algo/simulation/montecarlo/utils/__init__.py
+-rw-rw-rw-   0        0        0     5316 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/algo/simulation/montecarlo/utils/replay.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:32.976484 pm4pyminimal-2.7.9.4/pm4py/algo/simulation/montecarlo/variants/
+-rw-rw-rw-   0        0        0      807 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/algo/simulation/montecarlo/variants/__init__.py
+-rw-rw-rw-   0        0        0    19853 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/algo/simulation/montecarlo/variants/petri_semaph_fifo.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:32.976484 pm4pyminimal-2.7.9.4/pm4py/algo/simulation/playout/
+-rw-rw-rw-   0        0        0      806 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/algo/simulation/playout/__init__.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:32.992106 pm4pyminimal-2.7.9.4/pm4py/algo/simulation/playout/dfg/
+-rw-rw-rw-   0        0        0      801 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/algo/simulation/playout/dfg/__init__.py
+-rw-rw-rw-   0        0        0     1940 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/algo/simulation/playout/dfg/algorithm.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:32.992106 pm4pyminimal-2.7.9.4/pm4py/algo/simulation/playout/dfg/variants/
+-rw-rw-rw-   0        0        0      811 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/algo/simulation/playout/dfg/variants/__init__.py
+-rw-rw-rw-   0        0        0    14627 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/algo/simulation/playout/dfg/variants/classic.py
+-rw-rw-rw-   0        0        0     6099 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/algo/simulation/playout/dfg/variants/performance.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:33.007726 pm4pyminimal-2.7.9.4/pm4py/algo/simulation/playout/petri_net/
+-rw-rw-rw-   0        0        0      807 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/algo/simulation/playout/petri_net/__init__.py
+-rw-rw-rw-   0        0        0     2552 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/algo/simulation/playout/petri_net/algorithm.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:33.007726 pm4pyminimal-2.7.9.4/pm4py/algo/simulation/playout/petri_net/variants/
+-rw-rw-rw-   0        0        0      821 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/algo/simulation/playout/petri_net/variants/__init__.py
+-rw-rw-rw-   0        0        0     9126 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/algo/simulation/playout/petri_net/variants/basic_playout.py
+-rw-rw-rw-   0        0        0     5306 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/algo/simulation/playout/petri_net/variants/extensive.py
+-rw-rw-rw-   0        0        0     8008 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/algo/simulation/playout/petri_net/variants/stochastic_playout.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:33.023347 pm4pyminimal-2.7.9.4/pm4py/algo/simulation/playout/process_tree/
+-rw-rw-rw-   0        0        0      810 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/algo/simulation/playout/process_tree/__init__.py
+-rw-rw-rw-   0        0        0     1862 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/algo/simulation/playout/process_tree/algorithm.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:33.038968 pm4pyminimal-2.7.9.4/pm4py/algo/simulation/playout/process_tree/variants/
+-rw-rw-rw-   0        0        0      835 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/algo/simulation/playout/process_tree/variants/__init__.py
+-rw-rw-rw-   0        0        0     1679 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/algo/simulation/playout/process_tree/variants/basic_playout.py
+-rw-rw-rw-   0        0        0    13571 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/algo/simulation/playout/process_tree/variants/extensive.py
+-rw-rw-rw-   0        0        0     4861 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/algo/simulation/playout/process_tree/variants/topbottom.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:33.038968 pm4pyminimal-2.7.9.4/pm4py/algo/simulation/tree_generator/
+-rw-rw-rw-   0        0        0      806 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/algo/simulation/tree_generator/__init__.py
+-rw-rw-rw-   0        0        0     1765 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/algo/simulation/tree_generator/algorithm.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:33.038968 pm4pyminimal-2.7.9.4/pm4py/algo/simulation/tree_generator/variants/
+-rw-rw-rw-   0        0        0      818 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/algo/simulation/tree_generator/variants/__init__.py
+-rw-rw-rw-   0        0        0     5357 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/algo/simulation/tree_generator/variants/basic.py
+-rw-rw-rw-   0        0        0    12955 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/algo/simulation/tree_generator/variants/ptandloggenerator.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:33.038968 pm4pyminimal-2.7.9.4/pm4py/algo/transformation/
+-rw-rw-rw-   0        0        0      808 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/algo/transformation/__init__.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:33.056100 pm4pyminimal-2.7.9.4/pm4py/algo/transformation/log_to_features/
+-rw-rw-rw-   0        0        0      809 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/algo/transformation/log_to_features/__init__.py
+-rw-rw-rw-   0        0        0     2205 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/algo/transformation/log_to_features/algorithm.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:33.056100 pm4pyminimal-2.7.9.4/pm4py/algo/transformation/log_to_features/util/
+-rw-rw-rw-   0        0        0      819 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/algo/transformation/log_to_features/util/__init__.py
+-rw-rw-rw-   0        0        0     3933 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/algo/transformation/log_to_features/util/locally_linear_embedding.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:33.072003 pm4pyminimal-2.7.9.4/pm4py/algo/transformation/log_to_features/variants/
+-rw-rw-rw-   0        0        0      823 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/algo/transformation/log_to_features/variants/__init__.py
+-rw-rw-rw-   0        0        0     6689 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/algo/transformation/log_to_features/variants/event_based.py
+-rw-rw-rw-   0        0        0     6644 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/algo/transformation/log_to_features/variants/temporal.py
+-rw-rw-rw-   0        0        0    50368 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/algo/transformation/log_to_features/variants/trace_based.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:33.077298 pm4pyminimal-2.7.9.4/pm4py/algo/transformation/log_to_interval_tree/
+-rw-rw-rw-   0        0        0      999 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/algo/transformation/log_to_interval_tree/__init__.py
+-rw-rw-rw-   0        0        0     2171 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/algo/transformation/log_to_interval_tree/algorithm.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:33.077298 pm4pyminimal-2.7.9.4/pm4py/algo/transformation/log_to_interval_tree/variants/
+-rw-rw-rw-   0        0        0      814 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/algo/transformation/log_to_interval_tree/variants/__init__.py
+-rw-rw-rw-   0        0        0     6365 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/algo/transformation/log_to_interval_tree/variants/open_paths.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:33.077298 pm4pyminimal-2.7.9.4/pm4py/algo/transformation/log_to_target/
+-rw-rw-rw-   0        0        0      807 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/algo/transformation/log_to_target/__init__.py
+-rw-rw-rw-   0        0        0     2161 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/algo/transformation/log_to_target/algorithm.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:33.095292 pm4pyminimal-2.7.9.4/pm4py/algo/transformation/log_to_target/variants/
+-rw-rw-rw-   0        0        0      837 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/algo/transformation/log_to_target/variants/__init__.py
+-rw-rw-rw-   0        0        0     2922 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/algo/transformation/log_to_target/variants/next_activity.py
+-rw-rw-rw-   0        0        0     2526 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/algo/transformation/log_to_target/variants/next_time.py
+-rw-rw-rw-   0        0        0     2385 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/algo/transformation/log_to_target/variants/remaining_time.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:33.095292 pm4pyminimal-2.7.9.4/pm4py/algo/transformation/log_to_trie/
+-rw-rw-rw-   0        0        0      795 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/algo/transformation/log_to_trie/__init__.py
+-rw-rw-rw-   0        0        0     2261 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/algo/transformation/log_to_trie/algorithm.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:33.095292 pm4pyminimal-2.7.9.4/pm4py/algo/transformation/ocel/
+-rw-rw-rw-   0        0        0      807 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/algo/transformation/ocel/__init__.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:33.095292 pm4pyminimal-2.7.9.4/pm4py/algo/transformation/ocel/description/
+-rw-rw-rw-   0        0        0      736 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/algo/transformation/ocel/description/__init__.py
+-rw-rw-rw-   0        0        0     1684 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/algo/transformation/ocel/description/algorithm.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:33.110914 pm4pyminimal-2.7.9.4/pm4py/algo/transformation/ocel/description/variants/
+-rw-rw-rw-   0        0        0      736 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/algo/transformation/ocel/description/variants/__init__.py
+-rw-rw-rw-   0        0        0     3318 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/algo/transformation/ocel/description/variants/variant1.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:33.110914 pm4pyminimal-2.7.9.4/pm4py/algo/transformation/ocel/features/
+-rw-rw-rw-   0        0        0      821 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/algo/transformation/ocel/features/__init__.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:33.126534 pm4pyminimal-2.7.9.4/pm4py/algo/transformation/ocel/features/events/
+-rw-rw-rw-   0        0        0     1002 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/algo/transformation/ocel/features/events/__init__.py
+-rw-rw-rw-   0        0        0     9094 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/algo/transformation/ocel/features/events/algorithm.py
+-rw-rw-rw-   0        0        0     2022 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/algo/transformation/ocel/features/events/event_activity.py
+-rw-rw-rw-   0        0        0     2250 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/algo/transformation/ocel/features/events/event_end_ot.py
+-rw-rw-rw-   0        0        0     2542 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/algo/transformation/ocel/features/events/event_num_attributes.py
+-rw-rw-rw-   0        0        0     1691 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/algo/transformation/ocel/features/events/event_num_rel_objs.py
+-rw-rw-rw-   0        0        0     2354 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/algo/transformation/ocel/features/events/event_num_rel_objs_type.py
+-rw-rw-rw-   0        0        0     2236 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/algo/transformation/ocel/features/events/event_start_ot.py
+-rw-rw-rw-   0        0        0     3041 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/algo/transformation/ocel/features/events/event_str_attributes.py
+-rw-rw-rw-   0        0        0     2031 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/algo/transformation/ocel/features/events/event_timestamp.py
+-rw-rw-rw-   0        0        0     1990 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/algo/transformation/ocel/features/events/new_interactions.py
+-rw-rw-rw-   0        0        0     2805 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/algo/transformation/ocel/features/events/related_objects_features.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:33.142156 pm4pyminimal-2.7.9.4/pm4py/algo/transformation/ocel/features/events_objects/
+-rw-rw-rw-   0        0        0      831 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/algo/transformation/ocel/features/events_objects/__init__.py
+-rw-rw-rw-   0        0        0     3899 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/algo/transformation/ocel/features/events_objects/algorithm.py
+-rw-rw-rw-   0        0        0     4959 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/algo/transformation/ocel/features/events_objects/prefix_features.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:33.187409 pm4pyminimal-2.7.9.4/pm4py/algo/transformation/ocel/features/objects/
+-rw-rw-rw-   0        0        0     1268 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/algo/transformation/ocel/features/objects/__init__.py
+-rw-rw-rw-   0        0        0    20532 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/algo/transformation/ocel/features/objects/algorithm.py
+-rw-rw-rw-   0        0        0     3400 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/algo/transformation/ocel/features/objects/obj_con_in_graph_features.py
+-rw-rw-rw-   0        0        0     1912 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/algo/transformation/ocel/features/objects/object_cobirth_graph.py
+-rw-rw-rw-   0        0        0     1912 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/algo/transformation/ocel/features/objects/object_codeath_graph.py
+-rw-rw-rw-   0        0        0     1988 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/algo/transformation/ocel/features/objects/object_degree_centrality.py
+-rw-rw-rw-   0        0        0     2100 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/algo/transformation/ocel/features/objects/object_general_descendants_graph.py
+-rw-rw-rw-   0        0        0     2152 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/algo/transformation/ocel/features/objects/object_general_inheritance_graph.py
+-rw-rw-rw-   0        0        0     1942 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/algo/transformation/ocel/features/objects/object_general_interaction_graph.py
+-rw-rw-rw-   0        0        0     2080 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/algo/transformation/ocel/features/objects/object_lifecycle_activities.py
+-rw-rw-rw-   0        0        0     2197 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/algo/transformation/ocel/features/objects/object_lifecycle_duration.py
+-rw-rw-rw-   0        0        0     1794 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/algo/transformation/ocel/features/objects/object_lifecycle_length.py
+-rw-rw-rw-   0        0        0     2205 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/algo/transformation/ocel/features/objects/object_lifecycle_paths.py
+-rw-rw-rw-   0        0        0     1920 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/algo/transformation/ocel/features/objects/object_lifecycle_unq_act.py
+-rw-rw-rw-   0        0        0     2586 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/algo/transformation/ocel/features/objects/object_num_attributes.py
+-rw-rw-rw-   0        0        0     3062 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/algo/transformation/ocel/features/objects/object_str_attributes.py
+-rw-rw-rw-   0        0        0     2455 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/algo/transformation/ocel/features/objects/object_work_in_progress.py
+-rw-rw-rw-   0        0        0     2486 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/algo/transformation/ocel/features/objects/objects_interaction_graph_ot.py
+-rw-rw-rw-   0        0        0     3063 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/algo/transformation/ocel/features/objects/related_activities_features.py
+-rw-rw-rw-   0        0        0     2788 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/algo/transformation/ocel/features/objects/related_events_features.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:33.203031 pm4pyminimal-2.7.9.4/pm4py/algo/transformation/ocel/graphs/
+-rw-rw-rw-   0        0        0      906 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/algo/transformation/ocel/graphs/__init__.py
+-rw-rw-rw-   0        0        0     2305 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/algo/transformation/ocel/graphs/object_cobirth_graph.py
+-rw-rw-rw-   0        0        0     2103 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/algo/transformation/ocel/graphs/object_codeath_graph.py
+-rw-rw-rw-   0        0        0     2327 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/algo/transformation/ocel/graphs/object_descendants_graph.py
+-rw-rw-rw-   0        0        0     2852 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/algo/transformation/ocel/graphs/object_inheritance_graph.py
+-rw-rw-rw-   0        0        0     1736 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/algo/transformation/ocel/graphs/object_interaction_graph.py
+-rw-rw-rw-   0        0        0     3641 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/algo/transformation/ocel/graphs/ocel20_computation.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:33.203031 pm4pyminimal-2.7.9.4/pm4py/algo/transformation/ocel/split_ocel/
+-rw-rw-rw-   0        0        0      809 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/algo/transformation/ocel/split_ocel/__init__.py
+-rw-rw-rw-   0        0        0     1730 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/algo/transformation/ocel/split_ocel/algorithm.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:33.203031 pm4pyminimal-2.7.9.4/pm4py/algo/transformation/ocel/split_ocel/variants/
+-rw-rw-rw-   0        0        0      819 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/algo/transformation/ocel/split_ocel/variants/__init__.py
+-rw-rw-rw-   0        0        0     3429 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/algo/transformation/ocel/split_ocel/variants/ancestors_descendants.py
+-rw-rw-rw-   0        0        0     3467 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/algo/transformation/ocel/split_ocel/variants/connected_components.py
+-rw-rw-rw-   0        0        0    20646 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/analysis.py
+-rw-rw-rw-   0        0        0    13471 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/cli.py
+-rw-rw-rw-   0        0        0    48213 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/conformance.py
+-rw-rw-rw-   0        0        0    19636 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/connectors.py
+-rw-rw-rw-   0        0        0    20826 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/convert.py
+-rw-rw-rw-   0        0        0    47943 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/discovery.py
+-rw-rw-rw-   0        0        0    63155 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/filtering.py
+-rw-rw-rw-   0        0        0     5192 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/hof.py
+-rw-rw-rw-   0        0        0    18976 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/llm.py
+-rw-rw-rw-   0        0        0     1098 2024-01-29 06:15:14.000000 pm4pyminimal-2.7.9.4/pm4py/meta.py
+-rw-rw-rw-   0        0        0    16160 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/ml.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:33.218652 pm4pyminimal-2.7.9.4/pm4py/objects/
+-rw-rw-rw-   0        0        0      947 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/objects/__init__.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:33.218652 pm4pyminimal-2.7.9.4/pm4py/objects/bpmn/
+-rw-rw-rw-   0        0        0      913 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/objects/bpmn/__init__.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:33.218652 pm4pyminimal-2.7.9.4/pm4py/objects/bpmn/exporter/
+-rw-rw-rw-   0        0        0      794 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/objects/bpmn/exporter/__init__.py
+-rw-rw-rw-   0        0        0     2130 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/objects/bpmn/exporter/exporter.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:33.236303 pm4pyminimal-2.7.9.4/pm4py/objects/bpmn/exporter/variants/
+-rw-rw-rw-   0        0        0      790 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/objects/bpmn/exporter/variants/__init__.py
+-rw-rw-rw-   0        0        0     7688 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/objects/bpmn/exporter/variants/etree.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:33.236303 pm4pyminimal-2.7.9.4/pm4py/objects/bpmn/importer/
+-rw-rw-rw-   0        0        0      794 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/objects/bpmn/importer/__init__.py
+-rw-rw-rw-   0        0        0     2085 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/objects/bpmn/importer/importer.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:33.236303 pm4pyminimal-2.7.9.4/pm4py/objects/bpmn/importer/variants/
+-rw-rw-rw-   0        0        0      789 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/objects/bpmn/importer/variants/__init__.py
+-rw-rw-rw-   0        0        0    17373 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/objects/bpmn/importer/variants/lxml.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:33.236303 pm4pyminimal-2.7.9.4/pm4py/objects/bpmn/layout/
+-rw-rw-rw-   0        0        0      792 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/objects/bpmn/layout/__init__.py
+-rw-rw-rw-   0        0        0     1534 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/objects/bpmn/layout/layouter.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:33.251925 pm4pyminimal-2.7.9.4/pm4py/objects/bpmn/layout/variants/
+-rw-rw-rw-   0        0        0      793 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/objects/bpmn/layout/variants/__init__.py
+-rw-rw-rw-   0        0        0    18042 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/objects/bpmn/layout/variants/graphviz.py
+-rw-rw-rw-   0        0        0    19676 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/objects/bpmn/obj.py
+-rw-rw-rw-   0        0        0     9205 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/objects/bpmn/semantics.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:33.256434 pm4pyminimal-2.7.9.4/pm4py/objects/bpmn/util/
+-rw-rw-rw-   0        0        0      802 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/objects/bpmn/util/__init__.py
+-rw-rw-rw-   0        0        0     6246 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/objects/bpmn/util/bpmn_utils.py
+-rw-rw-rw-   0        0        0     3352 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/objects/bpmn/util/reduction.py
+-rw-rw-rw-   0        0        0     3729 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/objects/bpmn/util/sorting.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:33.256434 pm4pyminimal-2.7.9.4/pm4py/objects/conversion/
+-rw-rw-rw-   0        0        0      825 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/objects/conversion/__init__.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:33.256434 pm4pyminimal-2.7.9.4/pm4py/objects/conversion/bpmn/
+-rw-rw-rw-   0        0        0      797 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/objects/conversion/bpmn/__init__.py
+-rw-rw-rw-   0        0        0     1160 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/objects/conversion/bpmn/converter.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:33.272060 pm4pyminimal-2.7.9.4/pm4py/objects/conversion/bpmn/variants/
+-rw-rw-rw-   0        0        0      799 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/objects/conversion/bpmn/variants/__init__.py
+-rw-rw-rw-   0        0        0    10026 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/objects/conversion/bpmn/variants/to_petri_net.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:33.272060 pm4pyminimal-2.7.9.4/pm4py/objects/conversion/dfg/
+-rw-rw-rw-   0        0        0      796 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/objects/conversion/dfg/__init__.py
+-rw-rw-rw-   0        0        0     1340 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/objects/conversion/dfg/converter.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:33.272060 pm4pyminimal-2.7.9.4/pm4py/objects/conversion/dfg/variants/
+-rw-rw-rw-   0        0        0      860 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/objects/conversion/dfg/variants/__init__.py
+-rw-rw-rw-   0        0        0     3494 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/objects/conversion/dfg/variants/to_petri_net_activity_defines_place.py
+-rw-rw-rw-   0        0        0     4229 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/objects/conversion/dfg/variants/to_petri_net_invisibles_no_duplicates.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:33.287682 pm4pyminimal-2.7.9.4/pm4py/objects/conversion/heuristics_net/
+-rw-rw-rw-   0        0        0      807 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/objects/conversion/heuristics_net/__init__.py
+-rw-rw-rw-   0        0        0     1384 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/objects/conversion/heuristics_net/converter.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:33.287682 pm4pyminimal-2.7.9.4/pm4py/objects/conversion/heuristics_net/variants/
+-rw-rw-rw-   0        0        0      809 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/objects/conversion/heuristics_net/variants/__init__.py
+-rw-rw-rw-   0        0        0    11773 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/objects/conversion/heuristics_net/variants/to_petri_net.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:33.287682 pm4pyminimal-2.7.9.4/pm4py/objects/conversion/log/
+-rw-rw-rw-   0        0        0      807 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/objects/conversion/log/__init__.py
+-rw-rw-rw-   0        0        0     1061 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/objects/conversion/log/constants.py
+-rw-rw-rw-   0        0        0     1319 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/objects/conversion/log/converter.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:33.303304 pm4pyminimal-2.7.9.4/pm4py/objects/conversion/log/variants/
+-rw-rw-rw-   0        0        0      870 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/objects/conversion/log/variants/__init__.py
+-rw-rw-rw-   0        0        0     1923 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/objects/conversion/log/variants/df_to_event_log_1v.py
+-rw-rw-rw-   0        0        0     2535 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/objects/conversion/log/variants/df_to_event_log_nv.py
+-rw-rw-rw-   0        0        0     2585 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/objects/conversion/log/variants/to_data_frame.py
+-rw-rw-rw-   0        0        0     4332 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/objects/conversion/log/variants/to_event_log.py
+-rw-rw-rw-   0        0        0    10224 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/objects/conversion/log/variants/to_event_stream.py
+-rw-rw-rw-   0        0        0     5236 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/objects/conversion/log/variants/to_nx.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:33.318924 pm4pyminimal-2.7.9.4/pm4py/objects/conversion/ocel/
+-rw-rw-rw-   0        0        0      799 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/objects/conversion/ocel/__init__.py
+-rw-rw-rw-   0        0        0     1814 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/objects/conversion/ocel/converter.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:33.318924 pm4pyminimal-2.7.9.4/pm4py/objects/conversion/ocel/variants/
+-rw-rw-rw-   0        0        0      820 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/objects/conversion/ocel/variants/__init__.py
+-rw-rw-rw-   0        0        0     4056 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/objects/conversion/ocel/variants/ocel_features_to_nx.py
+-rw-rw-rw-   0        0        0     4164 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/objects/conversion/ocel/variants/ocel_to_nx.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:33.318924 pm4pyminimal-2.7.9.4/pm4py/objects/conversion/powl/
+-rw-rw-rw-   0        0        0      781 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/objects/conversion/powl/__init__.py
+-rw-rw-rw-   0        0        0     1494 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/objects/conversion/powl/converter.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:33.334545 pm4pyminimal-2.7.9.4/pm4py/objects/conversion/powl/variants/
+-rw-rw-rw-   0        0        0      790 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/objects/conversion/powl/variants/__init__.py
+-rw-rw-rw-   0        0        0    11169 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/objects/conversion/powl/variants/to_petri_net.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:33.334545 pm4pyminimal-2.7.9.4/pm4py/objects/conversion/process_tree/
+-rw-rw-rw-   0        0        0      805 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/objects/conversion/process_tree/__init__.py
+-rw-rw-rw-   0        0        0     1824 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/objects/conversion/process_tree/converter.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:33.334545 pm4pyminimal-2.7.9.4/pm4py/objects/conversion/process_tree/variants/
+-rw-rw-rw-   0        0        0      850 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/objects/conversion/process_tree/variants/__init__.py
+-rw-rw-rw-   0        0        0    10139 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/objects/conversion/process_tree/variants/to_bpmn.py
+-rw-rw-rw-   0        0        0    21550 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/objects/conversion/process_tree/variants/to_petri_net.py
+-rw-rw-rw-   0        0        0     4772 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/objects/conversion/process_tree/variants/to_petri_net_transition_bordered.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:33.350166 pm4pyminimal-2.7.9.4/pm4py/objects/conversion/wf_net/
+-rw-rw-rw-   0        0        0      799 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/objects/conversion/wf_net/__init__.py
+-rw-rw-rw-   0        0        0     1167 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/objects/conversion/wf_net/converter.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:33.356674 pm4pyminimal-2.7.9.4/pm4py/objects/conversion/wf_net/variants/
+-rw-rw-rw-   0        0        0      813 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/objects/conversion/wf_net/variants/__init__.py
+-rw-rw-rw-   0        0        0     3774 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/objects/conversion/wf_net/variants/to_bpmn.py
+-rw-rw-rw-   0        0        0    10849 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/objects/conversion/wf_net/variants/to_process_tree.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:33.356674 pm4pyminimal-2.7.9.4/pm4py/objects/dfg/
+-rw-rw-rw-   0        0        0      796 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/objects/dfg/__init__.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:33.356674 pm4pyminimal-2.7.9.4/pm4py/objects/dfg/exporter/
+-rw-rw-rw-   0        0        0      793 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/objects/dfg/exporter/__init__.py
+-rw-rw-rw-   0        0        0     2041 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/objects/dfg/exporter/exporter.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:33.372301 pm4pyminimal-2.7.9.4/pm4py/objects/dfg/exporter/variants/
+-rw-rw-rw-   0        0        0      791 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/objects/dfg/exporter/variants/__init__.py
+-rw-rw-rw-   0        0        0     4571 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/objects/dfg/exporter/variants/classic.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:33.372301 pm4pyminimal-2.7.9.4/pm4py/objects/dfg/filtering/
+-rw-rw-rw-   0        0        0      734 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/objects/dfg/filtering/__init__.py
+-rw-rw-rw-   0        0        0      788 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/objects/dfg/filtering/dfg_filtering.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:33.372301 pm4pyminimal-2.7.9.4/pm4py/objects/dfg/importer/
+-rw-rw-rw-   0        0        0      793 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/objects/dfg/importer/__init__.py
+-rw-rw-rw-   0        0        0     2278 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/objects/dfg/importer/importer.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:33.387924 pm4pyminimal-2.7.9.4/pm4py/objects/dfg/importer/variants/
+-rw-rw-rw-   0        0        0      791 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/objects/dfg/importer/variants/__init__.py
+-rw-rw-rw-   0        0        0     4037 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/objects/dfg/importer/variants/classic.py
+-rw-rw-rw-   0        0        0     1881 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/objects/dfg/obj.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:33.387924 pm4pyminimal-2.7.9.4/pm4py/objects/dfg/retrieval/
+-rw-rw-rw-   0        0        0      734 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/objects/dfg/retrieval/__init__.py
+-rw-rw-rw-   0        0        0      913 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/objects/dfg/retrieval/log.py
+-rw-rw-rw-   0        0        0      873 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/objects/dfg/retrieval/pandas.py
+-rw-rw-rw-   0        0        0     5092 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/objects/dfg/util.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:33.387924 pm4pyminimal-2.7.9.4/pm4py/objects/dfg/utils/
+-rw-rw-rw-   0        0        0      781 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/objects/dfg/utils/__init__.py
+-rw-rw-rw-   0        0        0    26490 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/objects/dfg/utils/dfg_utils.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:33.403544 pm4pyminimal-2.7.9.4/pm4py/objects/heuristics_net/
+-rw-rw-rw-   0        0        0      802 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/objects/heuristics_net/__init__.py
+-rw-rw-rw-   0        0        0     1226 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/objects/heuristics_net/defaults.py
+-rw-rw-rw-   0        0        0     2689 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/objects/heuristics_net/edge.py
+-rw-rw-rw-   0        0        0     9877 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/objects/heuristics_net/node.py
+-rw-rw-rw-   0        0        0     5684 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/objects/heuristics_net/obj.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:33.403544 pm4pyminimal-2.7.9.4/pm4py/objects/log/
+-rw-rw-rw-   0        0        0      795 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/objects/log/__init__.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:33.403544 pm4pyminimal-2.7.9.4/pm4py/objects/log/exporter/
+-rw-rw-rw-   0        0        0      778 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/objects/log/exporter/__init__.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:33.419165 pm4pyminimal-2.7.9.4/pm4py/objects/log/exporter/xes/
+-rw-rw-rw-   0        0        0      803 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/objects/log/exporter/xes/__init__.py
+-rw-rw-rw-   0        0        0     2578 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/objects/log/exporter/xes/exporter.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:33.419165 pm4pyminimal-2.7.9.4/pm4py/objects/log/exporter/xes/util/
+-rw-rw-rw-   0        0        0      795 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/objects/log/exporter/xes/util/__init__.py
+-rw-rw-rw-   0        0        0     1423 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/objects/log/exporter/xes/util/compression.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:33.419165 pm4pyminimal-2.7.9.4/pm4py/objects/log/exporter/xes/variants/
+-rw-rw-rw-   0        0        0      815 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/objects/log/exporter/xes/variants/__init__.py
+-rw-rw-rw-   0        0        0    12326 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/objects/log/exporter/xes/variants/etree_xes_exp.py
+-rw-rw-rw-   0        0        0    10430 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/objects/log/exporter/xes/variants/line_by_line.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:33.419165 pm4pyminimal-2.7.9.4/pm4py/objects/log/importer/
+-rw-rw-rw-   0        0        0      778 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/objects/log/importer/__init__.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:33.434788 pm4pyminimal-2.7.9.4/pm4py/objects/log/importer/xes/
+-rw-rw-rw-   0        0        0      797 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/objects/log/importer/xes/__init__.py
+-rw-rw-rw-   0        0        0     4379 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/objects/log/importer/xes/importer.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:33.452762 pm4pyminimal-2.7.9.4/pm4py/objects/log/importer/xes/variants/
+-rw-rw-rw-   0        0        0      850 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/objects/log/importer/xes/variants/__init__.py
+-rw-rw-rw-   0        0        0     9534 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/objects/log/importer/xes/variants/chunk_regex.py
+-rw-rw-rw-   0        0        0    17582 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/objects/log/importer/xes/variants/iterparse.py
+-rw-rw-rw-   0        0        0    17851 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/objects/log/importer/xes/variants/iterparse_20.py
+-rw-rw-rw-   0        0        0    18150 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/objects/log/importer/xes/variants/iterparse_mem_compressed.py
+-rw-rw-rw-   0        0        0    11435 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/objects/log/importer/xes/variants/line_by_line.py
+-rw-rw-rw-   0        0        0     2094 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/objects/log/importer/xes/variants/rustxes.py
+-rw-rw-rw-   0        0        0    12284 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/objects/log/obj.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:33.494644 pm4pyminimal-2.7.9.4/pm4py/objects/log/util/
+-rw-rw-rw-   0        0        0     1010 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/objects/log/util/__init__.py
+-rw-rw-rw-   0        0        0     3127 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/objects/log/util/activities_to_alphabet.py
+-rw-rw-rw-   0        0        0     3114 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/objects/log/util/artificial.py
+-rw-rw-rw-   0        0        0     3974 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/objects/log/util/basic_filter.py
+-rw-rw-rw-   0        0        0    18992 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/objects/log/util/dataframe_utils.py
+-rw-rw-rw-   0        0        0     2283 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/objects/log/util/filtering_utils.py
+-rw-rw-rw-   0        0        0     4856 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/objects/log/util/get_class_representation.py
+-rw-rw-rw-   0        0        0     3195 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/objects/log/util/get_log_encoded.py
+-rw-rw-rw-   0        0        0     8099 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/objects/log/util/get_prefixes.py
+-rw-rw-rw-   0        0        0     1752 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/objects/log/util/index_attribute.py
+-rw-rw-rw-   0        0        0     4067 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/objects/log/util/insert_classifier.py
+-rw-rw-rw-   0        0        0    12476 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/objects/log/util/interval_lifecycle.py
+-rw-rw-rw-   0        0        0     5167 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/objects/log/util/log.py
+-rw-rw-rw-   0        0        0     4389 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/objects/log/util/log_regex.py
+-rw-rw-rw-   0        0        0     2867 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/objects/log/util/move_attrs_to_trace.py
+-rw-rw-rw-   0        0        0     4527 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/objects/log/util/pandas_log_wrapper.py
+-rw-rw-rw-   0        0        0     4094 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/objects/log/util/pandas_numpy_variants.py
+-rw-rw-rw-   0        0        0     2465 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/objects/log/util/sampling.py
+-rw-rw-rw-   0        0        0     6049 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/objects/log/util/sorting.py
+-rw-rw-rw-   0        0        0     2078 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/objects/log/util/split_train_test.py
+-rw-rw-rw-   0        0        0     1695 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/objects/log/util/xes.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:33.494644 pm4pyminimal-2.7.9.4/pm4py/objects/ocel/
+-rw-rw-rw-   0        0        0      819 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/objects/ocel/__init__.py
+-rw-rw-rw-   0        0        0     2372 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/objects/ocel/constants.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:33.494644 pm4pyminimal-2.7.9.4/pm4py/objects/ocel/exporter/
+-rw-rw-rw-   0        0        0      911 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/objects/ocel/exporter/__init__.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:33.494644 pm4pyminimal-2.7.9.4/pm4py/objects/ocel/exporter/csv/
+-rw-rw-rw-   0        0        0      798 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/objects/ocel/exporter/csv/__init__.py
+-rw-rw-rw-   0        0        0     1695 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/objects/ocel/exporter/csv/exporter.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:33.512023 pm4pyminimal-2.7.9.4/pm4py/objects/ocel/exporter/csv/variants/
+-rw-rw-rw-   0        0        0      795 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/objects/ocel/exporter/csv/variants/__init__.py
+-rw-rw-rw-   0        0        0     1927 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/objects/ocel/exporter/csv/variants/pandas.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:33.512023 pm4pyminimal-2.7.9.4/pm4py/objects/ocel/exporter/jsonocel/
+-rw-rw-rw-   0        0        0      803 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/objects/ocel/exporter/jsonocel/__init__.py
+-rw-rw-rw-   0        0        0     1635 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/objects/ocel/exporter/jsonocel/exporter.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:33.512023 pm4pyminimal-2.7.9.4/pm4py/objects/ocel/exporter/jsonocel/variants/
+-rw-rw-rw-   0        0        0      826 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/objects/ocel/exporter/jsonocel/variants/__init__.py
+-rw-rw-rw-   0        0        0     5448 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/objects/ocel/exporter/jsonocel/variants/classic.py
+-rw-rw-rw-   0        0        0     5591 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/objects/ocel/exporter/jsonocel/variants/ocel20.py
+-rw-rw-rw-   0        0        0     4247 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/objects/ocel/exporter/jsonocel/variants/ocel20_standard.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:33.527645 pm4pyminimal-2.7.9.4/pm4py/objects/ocel/exporter/sqlite/
+-rw-rw-rw-   0        0        0      803 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/objects/ocel/exporter/sqlite/__init__.py
+-rw-rw-rw-   0        0        0     1673 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/objects/ocel/exporter/sqlite/exporter.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:33.527645 pm4pyminimal-2.7.9.4/pm4py/objects/ocel/exporter/sqlite/variants/
+-rw-rw-rw-   0        0        0      809 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/objects/ocel/exporter/sqlite/variants/__init__.py
+-rw-rw-rw-   0        0        0     4931 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/objects/ocel/exporter/sqlite/variants/ocel20.py
+-rw-rw-rw-   0        0        0     1679 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/objects/ocel/exporter/sqlite/variants/pandas_exporter.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:33.527645 pm4pyminimal-2.7.9.4/pm4py/objects/ocel/exporter/util/
+-rw-rw-rw-   0        0        0      797 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/objects/ocel/exporter/util/__init__.py
+-rw-rw-rw-   0        0        0     1658 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/objects/ocel/exporter/util/clean_dataframes.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:33.543270 pm4pyminimal-2.7.9.4/pm4py/objects/ocel/exporter/xmlocel/
+-rw-rw-rw-   0        0        0      802 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/objects/ocel/exporter/xmlocel/__init__.py
+-rw-rw-rw-   0        0        0     1578 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/objects/ocel/exporter/xmlocel/exporter.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:33.543270 pm4pyminimal-2.7.9.4/pm4py/objects/ocel/exporter/xmlocel/variants/
+-rw-rw-rw-   0        0        0      734 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/objects/ocel/exporter/xmlocel/variants/__init__.py
+-rw-rw-rw-   0        0        0     8129 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/objects/ocel/exporter/xmlocel/variants/classic.py
+-rw-rw-rw-   0        0        0     8746 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/objects/ocel/exporter/xmlocel/variants/ocel20.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:33.543270 pm4pyminimal-2.7.9.4/pm4py/objects/ocel/importer/
+-rw-rw-rw-   0        0        0      905 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/objects/ocel/importer/__init__.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:33.556784 pm4pyminimal-2.7.9.4/pm4py/objects/ocel/importer/csv/
+-rw-rw-rw-   0        0        0      798 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/objects/ocel/importer/csv/__init__.py
+-rw-rw-rw-   0        0        0     1731 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/objects/ocel/importer/csv/importer.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:33.556784 pm4pyminimal-2.7.9.4/pm4py/objects/ocel/importer/csv/variants/
+-rw-rw-rw-   0        0        0      795 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/objects/ocel/importer/csv/variants/__init__.py
+-rw-rw-rw-   0        0        0     2211 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/objects/ocel/importer/csv/variants/pandas.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:33.556784 pm4pyminimal-2.7.9.4/pm4py/objects/ocel/importer/jsonocel/
+-rw-rw-rw-   0        0        0      803 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/objects/ocel/importer/jsonocel/__init__.py
+-rw-rw-rw-   0        0        0     1641 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/objects/ocel/importer/jsonocel/importer.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:33.556784 pm4pyminimal-2.7.9.4/pm4py/objects/ocel/importer/jsonocel/variants/
+-rw-rw-rw-   0        0        0      818 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/objects/ocel/importer/jsonocel/variants/__init__.py
+-rw-rw-rw-   0        0        0     7338 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/objects/ocel/importer/jsonocel/variants/classic.py
+-rw-rw-rw-   0        0        0     3863 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/objects/ocel/importer/jsonocel/variants/ocel20_standard.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:33.572411 pm4pyminimal-2.7.9.4/pm4py/objects/ocel/importer/sqlite/
+-rw-rw-rw-   0        0        0      803 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/objects/ocel/importer/sqlite/__init__.py
+-rw-rw-rw-   0        0        0     1704 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/objects/ocel/importer/sqlite/importer.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:33.572411 pm4pyminimal-2.7.9.4/pm4py/objects/ocel/importer/sqlite/variants/
+-rw-rw-rw-   0        0        0      809 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/objects/ocel/importer/sqlite/variants/__init__.py
+-rw-rw-rw-   0        0        0     8462 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/objects/ocel/importer/sqlite/variants/ocel20.py
+-rw-rw-rw-   0        0        0     2620 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/objects/ocel/importer/sqlite/variants/pandas_importer.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:33.572411 pm4pyminimal-2.7.9.4/pm4py/objects/ocel/importer/xmlocel/
+-rw-rw-rw-   0        0        0      802 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/objects/ocel/importer/xmlocel/__init__.py
+-rw-rw-rw-   0        0        0     1611 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/objects/ocel/importer/xmlocel/importer.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:33.588033 pm4pyminimal-2.7.9.4/pm4py/objects/ocel/importer/xmlocel/variants/
+-rw-rw-rw-   0        0        0      800 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/objects/ocel/importer/xmlocel/variants/__init__.py
+-rw-rw-rw-   0        0        0     8919 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/objects/ocel/importer/xmlocel/variants/classic.py
+-rw-rw-rw-   0        0        0    10021 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/objects/ocel/importer/xmlocel/variants/ocel20.py
+-rw-rw-rw-   0        0        0     7221 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/objects/ocel/obj.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:33.656944 pm4pyminimal-2.7.9.4/pm4py/objects/ocel/util/
+-rw-rw-rw-   0        0        0     1067 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/objects/ocel/util/__init__.py
+-rw-rw-rw-   0        0        0     1690 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/objects/ocel/util/attributes_names.py
+-rw-rw-rw-   0        0        0     2156 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/objects/ocel/util/attributes_per_type.py
+-rw-rw-rw-   0        0        0     2424 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/objects/ocel/util/convergence_divergence_diagnostics.py
+-rw-rw-rw-   0        0        0     2690 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/objects/ocel/util/e2o_qualification.py
+-rw-rw-rw-   0        0        0     3809 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/objects/ocel/util/ev_att_to_obj_type.py
+-rw-rw-rw-   0        0        0     4453 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/objects/ocel/util/event_prefix_suffix_per_obj.py
+-rw-rw-rw-   0        0        0     2215 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/objects/ocel/util/events_per_object_type.py
+-rw-rw-rw-   0        0        0     3274 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/objects/ocel/util/events_per_type_per_activity.py
+-rw-rw-rw-   0        0        0     1654 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/objects/ocel/util/explode.py
+-rw-rw-rw-   0        0        0     5068 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/objects/ocel/util/extended_table.py
+-rw-rw-rw-   0        0        0     6565 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/objects/ocel/util/filtering_utils.py
+-rw-rw-rw-   0        0        0     3069 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/objects/ocel/util/flattening.py
+-rw-rw-rw-   0        0        0    17070 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/objects/ocel/util/log_ocel.py
+-rw-rw-rw-   0        0        0      942 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/objects/ocel/util/names_stripping.py
+-rw-rw-rw-   0        0        0     3274 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/objects/ocel/util/objects_per_type_per_activity.py
+-rw-rw-rw-   0        0        0     1974 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/objects/ocel/util/ocel_consistency.py
+-rw-rw-rw-   0        0        0     1976 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/objects/ocel/util/ocel_iterator.py
+-rw-rw-rw-   0        0        0     5167 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/objects/ocel/util/ocel_to_dict_types_rel.py
+-rw-rw-rw-   0        0        0     3510 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/objects/ocel/util/ocel_type_renaming.py
+-rw-rw-rw-   0        0        0     2478 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/objects/ocel/util/parent_children_ref.py
+-rw-rw-rw-   0        0        0     1362 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/objects/ocel/util/related_events.py
+-rw-rw-rw-   0        0        0     1830 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/objects/ocel/util/related_objects.py
+-rw-rw-rw-   0        0        0     2610 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/objects/ocel/util/rename_objs_ot_tim_lex.py
+-rw-rw-rw-   0        0        0     3783 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/objects/ocel/util/sampling.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:33.656944 pm4pyminimal-2.7.9.4/pm4py/objects/ocel/validation/
+-rw-rw-rw-   0        0        0      795 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/objects/ocel/validation/__init__.py
+-rw-rw-rw-   0        0        0     1389 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/objects/ocel/validation/jsonocel.py
+-rw-rw-rw-   0        0        0    14786 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/objects/ocel/validation/ocel20_rel_validation.py
+-rw-rw-rw-   0        0        0     1212 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/objects/ocel/validation/xmlocel.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:33.656944 pm4pyminimal-2.7.9.4/pm4py/objects/org/
+-rw-rw-rw-   0        0        0      776 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/objects/org/__init__.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:33.672566 pm4pyminimal-2.7.9.4/pm4py/objects/org/roles/
+-rw-rw-rw-   0        0        0      775 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/objects/org/roles/__init__.py
+-rw-rw-rw-   0        0        0     1339 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/objects/org/roles/obj.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:33.672566 pm4pyminimal-2.7.9.4/pm4py/objects/org/sna/
+-rw-rw-rw-   0        0        0      773 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/objects/org/sna/__init__.py
+-rw-rw-rw-   0        0        0     1029 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/objects/org/sna/obj.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:33.688189 pm4pyminimal-2.7.9.4/pm4py/objects/petri_net/
+-rw-rw-rw-   0        0        0      828 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/objects/petri_net/__init__.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:33.688189 pm4pyminimal-2.7.9.4/pm4py/objects/petri_net/data_petri_nets/
+-rw-rw-rw-   0        0        0      734 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/objects/petri_net/data_petri_nets/__init__.py
+-rw-rw-rw-   0        0        0     1287 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/objects/petri_net/data_petri_nets/data_marking.py
+-rw-rw-rw-   0        0        0     6212 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/objects/petri_net/data_petri_nets/semantics.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:33.703809 pm4pyminimal-2.7.9.4/pm4py/objects/petri_net/exporter/
+-rw-rw-rw-   0        0        0      799 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/objects/petri_net/exporter/__init__.py
+-rw-rw-rw-   0        0        0     2366 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/objects/petri_net/exporter/exporter.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:33.712312 pm4pyminimal-2.7.9.4/pm4py/objects/petri_net/exporter/variants/
+-rw-rw-rw-   0        0        0      794 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/objects/petri_net/exporter/variants/__init__.py
+-rw-rw-rw-   0        0        0    13002 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/objects/petri_net/exporter/variants/pnml.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:33.712312 pm4pyminimal-2.7.9.4/pm4py/objects/petri_net/importer/
+-rw-rw-rw-   0        0        0      799 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/objects/petri_net/importer/__init__.py
+-rw-rw-rw-   0        0        0     1910 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/objects/petri_net/importer/importer.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:33.712312 pm4pyminimal-2.7.9.4/pm4py/objects/petri_net/importer/variants/
+-rw-rw-rw-   0        0        0      794 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/objects/petri_net/importer/variants/__init__.py
+-rw-rw-rw-   0        0        0    15369 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/objects/petri_net/importer/variants/pnml.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:33.727938 pm4pyminimal-2.7.9.4/pm4py/objects/petri_net/inhibitor_reset/
+-rw-rw-rw-   0        0        0      734 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/objects/petri_net/inhibitor_reset/__init__.py
+-rw-rw-rw-   0        0        0     4617 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/objects/petri_net/inhibitor_reset/semantics.py
+-rw-rw-rw-   0        0        0    13270 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/objects/petri_net/obj.py
+-rw-rw-rw-   0        0        0     1225 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/objects/petri_net/properties.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:33.727938 pm4pyminimal-2.7.9.4/pm4py/objects/petri_net/saw_net/
+-rw-rw-rw-   0        0        0      805 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/objects/petri_net/saw_net/__init__.py
+-rw-rw-rw-   0        0        0     4799 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/objects/petri_net/saw_net/convert.py
+-rw-rw-rw-   0        0        0     1546 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/objects/petri_net/saw_net/obj.py
+-rw-rw-rw-   0        0        0    10711 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/objects/petri_net/saw_net/semantics.py
+-rw-rw-rw-   0        0        0     1503 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/objects/petri_net/sem_interface.py
+-rw-rw-rw-   0        0        0     5339 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/objects/petri_net/semantics.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:33.743560 pm4pyminimal-2.7.9.4/pm4py/objects/petri_net/stochastic/
+-rw-rw-rw-   0        0        0      799 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/objects/petri_net/stochastic/__init__.py
+-rw-rw-rw-   0        0        0     1448 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/objects/petri_net/stochastic/obj.py
+-rw-rw-rw-   0        0        0     2607 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/objects/petri_net/stochastic/semantics.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:33.788328 pm4pyminimal-2.7.9.4/pm4py/objects/petri_net/utils/
+-rw-rw-rw-   0        0        0     1035 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/objects/petri_net/utils/__init__.py
+-rw-rw-rw-   0        0        0    19297 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/objects/petri_net/utils/align_utils.py
+-rw-rw-rw-   0        0        0     5923 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/objects/petri_net/utils/check_soundness.py
+-rw-rw-rw-   0        0        0     4014 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/objects/petri_net/utils/consumption_matrix.py
+-rw-rw-rw-   0        0        0     6609 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/objects/petri_net/utils/decomposition.py
+-rw-rw-rw-   0        0        0     1672 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/objects/petri_net/utils/embed_stochastic_map.py
+-rw-rw-rw-   0        0        0     5751 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/objects/petri_net/utils/explore_path.py
+-rw-rw-rw-   0        0        0     1195 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/objects/petri_net/utils/final_marking.py
+-rw-rw-rw-   0        0        0     2272 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/objects/petri_net/utils/incidence_matrix.py
+-rw-rw-rw-   0        0        0     1227 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/objects/petri_net/utils/initial_marking.py
+-rw-rw-rw-   0        0        0     4243 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/objects/petri_net/utils/murata.py
+-rw-rw-rw-   0        0        0     4281 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/objects/petri_net/utils/networkx_graph.py
+-rw-rw-rw-   0        0        0     4071 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/objects/petri_net/utils/obj_marking.py
+-rw-rw-rw-   0        0        0    22973 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/objects/petri_net/utils/performance_map.py
+-rw-rw-rw-   0        0        0    20395 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/objects/petri_net/utils/petri_utils.py
+-rw-rw-rw-   0        0        0     4602 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/objects/petri_net/utils/projection.py
+-rw-rw-rw-   0        0        0     5570 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/objects/petri_net/utils/reachability_graph.py
+-rw-rw-rw-   0        0        0    14266 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/objects/petri_net/utils/reduction.py
+-rw-rw-rw-   0        0        0     7288 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/objects/petri_net/utils/synchronous_product.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:33.803949 pm4pyminimal-2.7.9.4/pm4py/objects/powl/
+-rw-rw-rw-   0        0        0     6732 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/objects/powl/BinaryRelation.py
+-rw-rw-rw-   0        0        0      772 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/objects/powl/__init__.py
+-rw-rw-rw-   0        0        0      804 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/objects/powl/constants.py
+-rw-rw-rw-   0        0        0    15122 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/objects/powl/obj.py
+-rw-rw-rw-   0        0        0     5268 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/objects/powl/parser.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:33.803949 pm4pyminimal-2.7.9.4/pm4py/objects/process_tree/
+-rw-rw-rw-   0        0        0      929 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/objects/process_tree/__init__.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:33.803949 pm4pyminimal-2.7.9.4/pm4py/objects/process_tree/exporter/
+-rw-rw-rw-   0        0        0      802 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/objects/process_tree/exporter/__init__.py
+-rw-rw-rw-   0        0        0     1888 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/objects/process_tree/exporter/exporter.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:33.819572 pm4pyminimal-2.7.9.4/pm4py/objects/process_tree/exporter/variants/
+-rw-rw-rw-   0        0        0      797 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/objects/process_tree/exporter/variants/__init__.py
+-rw-rw-rw-   0        0        0     5832 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/objects/process_tree/exporter/variants/ptml.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:33.819572 pm4pyminimal-2.7.9.4/pm4py/objects/process_tree/importer/
+-rw-rw-rw-   0        0        0      802 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/objects/process_tree/importer/__init__.py
+-rw-rw-rw-   0        0        0     2048 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/objects/process_tree/importer/importer.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:33.819572 pm4pyminimal-2.7.9.4/pm4py/objects/process_tree/importer/variants/
+-rw-rw-rw-   0        0        0      797 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/objects/process_tree/importer/variants/__init__.py
+-rw-rw-rw-   0        0        0     5476 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/objects/process_tree/importer/variants/ptml.py
+-rw-rw-rw-   0        0        0     8283 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/objects/process_tree/obj.py
+-rw-rw-rw-   0        0        0     8883 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/objects/process_tree/semantics.py
+-rw-rw-rw-   0        0        0      887 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/objects/process_tree/state.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:33.835194 pm4pyminimal-2.7.9.4/pm4py/objects/process_tree/utils/
+-rw-rw-rw-   0        0        0      734 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/objects/process_tree/utils/__init__.py
+-rw-rw-rw-   0        0        0     7128 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/objects/process_tree/utils/bottomup.py
+-rw-rw-rw-   0        0        0    15834 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/objects/process_tree/utils/generic.py
+-rw-rw-rw-   0        0        0     3438 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/objects/process_tree/utils/regex.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:33.835194 pm4pyminimal-2.7.9.4/pm4py/objects/random_variables/
+-rw-rw-rw-   0        0        0     1034 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/objects/random_variables/__init__.py
+-rw-rw-rw-   0        0        0     3878 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/objects/random_variables/basic_structure.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:33.835194 pm4pyminimal-2.7.9.4/pm4py/objects/random_variables/constant0/
+-rw-rw-rw-   0        0        0      804 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/objects/random_variables/constant0/__init__.py
+-rw-rw-rw-   0        0        0     3586 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/objects/random_variables/constant0/random_variable.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:33.850814 pm4pyminimal-2.7.9.4/pm4py/objects/random_variables/exponential/
+-rw-rw-rw-   0        0        0      818 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/objects/random_variables/exponential/__init__.py
+-rw-rw-rw-   0        0        0     3684 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/objects/random_variables/exponential/random_variable.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:33.850814 pm4pyminimal-2.7.9.4/pm4py/objects/random_variables/gamma/
+-rw-rw-rw-   0        0        0      800 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/objects/random_variables/gamma/__init__.py
+-rw-rw-rw-   0        0        0     3841 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/objects/random_variables/gamma/random_variable.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:33.857320 pm4pyminimal-2.7.9.4/pm4py/objects/random_variables/lognormal/
+-rw-rw-rw-   0        0        0      804 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/objects/random_variables/lognormal/__init__.py
+-rw-rw-rw-   0        0        0     3568 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/objects/random_variables/lognormal/random_variable.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:33.857320 pm4pyminimal-2.7.9.4/pm4py/objects/random_variables/normal/
+-rw-rw-rw-   0        0        0      801 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/objects/random_variables/normal/__init__.py
+-rw-rw-rw-   0        0        0     3594 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/objects/random_variables/normal/random_variable.py
+-rw-rw-rw-   0        0        0     9224 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/objects/random_variables/random_variable.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:33.857320 pm4pyminimal-2.7.9.4/pm4py/objects/random_variables/uniform/
+-rw-rw-rw-   0        0        0      802 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/objects/random_variables/uniform/__init__.py
+-rw-rw-rw-   0        0        0     3588 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/objects/random_variables/uniform/random_variable.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:33.876952 pm4pyminimal-2.7.9.4/pm4py/objects/stochastic_petri/
+-rw-rw-rw-   0        0        0      988 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/objects/stochastic_petri/__init__.py
+-rw-rw-rw-   0        0        0    12887 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/objects/stochastic_petri/ctmc.py
+-rw-rw-rw-   0        0        0     4714 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/objects/stochastic_petri/tangible_reachability.py
+-rw-rw-rw-   0        0        0     1616 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/objects/stochastic_petri/utils.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:33.876952 pm4pyminimal-2.7.9.4/pm4py/objects/transition_system/
+-rw-rw-rw-   0        0        0      803 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/objects/transition_system/__init__.py
+-rw-rw-rw-   0        0        0      825 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/objects/transition_system/constants.py
+-rw-rw-rw-   0        0        0     3958 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/objects/transition_system/obj.py
+-rw-rw-rw-   0        0        0     3625 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/objects/transition_system/utils.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:33.876952 pm4pyminimal-2.7.9.4/pm4py/objects/trie/
+-rw-rw-rw-   0        0        0      770 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/objects/trie/__init__.py
+-rw-rw-rw-   0        0        0     1911 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/objects/trie/obj.py
+-rw-rw-rw-   0        0        0    23143 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/ocel.py
+-rw-rw-rw-   0        0        0    14594 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/org.py
+-rw-rw-rw-   0        0        0     3805 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/privacy.py
+-rw-rw-rw-   0        0        0    15303 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/read.py
+-rw-rw-rw-   0        0        0     4578 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/sim.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:33.892577 pm4pyminimal-2.7.9.4/pm4py/statistics/
+-rw-rw-rw-   0        0        0      899 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/statistics/__init__.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:33.892577 pm4pyminimal-2.7.9.4/pm4py/statistics/attributes/
+-rw-rw-rw-   0        0        0      795 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/statistics/attributes/__init__.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:33.892577 pm4pyminimal-2.7.9.4/pm4py/statistics/attributes/common/
+-rw-rw-rw-   0        0        0      786 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/statistics/attributes/common/__init__.py
+-rw-rw-rw-   0        0        0     6611 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/statistics/attributes/common/get.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:33.892577 pm4pyminimal-2.7.9.4/pm4py/statistics/attributes/log/
+-rw-rw-rw-   0        0        0      791 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/statistics/attributes/log/__init__.py
+-rw-rw-rw-   0        0        0    13311 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/statistics/attributes/log/get.py
+-rw-rw-rw-   0        0        0     6905 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/statistics/attributes/log/select.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:33.911291 pm4pyminimal-2.7.9.4/pm4py/statistics/attributes/pandas/
+-rw-rw-rw-   0        0        0      786 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/statistics/attributes/pandas/__init__.py
+-rw-rw-rw-   0        0        0     9777 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/statistics/attributes/pandas/get.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:33.911291 pm4pyminimal-2.7.9.4/pm4py/statistics/concurrent_activities/
+-rw-rw-rw-   0        0        0      798 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/statistics/concurrent_activities/__init__.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:33.926917 pm4pyminimal-2.7.9.4/pm4py/statistics/concurrent_activities/log/
+-rw-rw-rw-   0        0        0      794 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/statistics/concurrent_activities/log/__init__.py
+-rw-rw-rw-   0        0        0     4081 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/statistics/concurrent_activities/log/get.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:33.926917 pm4pyminimal-2.7.9.4/pm4py/statistics/concurrent_activities/pandas/
+-rw-rw-rw-   0        0        0      797 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/statistics/concurrent_activities/pandas/__init__.py
+-rw-rw-rw-   0        0        0     3686 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/statistics/concurrent_activities/pandas/get.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:33.926917 pm4pyminimal-2.7.9.4/pm4py/statistics/end_activities/
+-rw-rw-rw-   0        0        0      799 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/statistics/end_activities/__init__.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:33.926917 pm4pyminimal-2.7.9.4/pm4py/statistics/end_activities/common/
+-rw-rw-rw-   0        0        0      790 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/statistics/end_activities/common/__init__.py
+-rw-rw-rw-   0        0        0     1791 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/statistics/end_activities/common/get.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:33.942541 pm4pyminimal-2.7.9.4/pm4py/statistics/end_activities/log/
+-rw-rw-rw-   0        0        0      787 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/statistics/end_activities/log/__init__.py
+-rw-rw-rw-   0        0        0     2746 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/statistics/end_activities/log/get.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:33.942541 pm4pyminimal-2.7.9.4/pm4py/statistics/end_activities/pandas/
+-rw-rw-rw-   0        0        0      790 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/statistics/end_activities/pandas/__init__.py
+-rw-rw-rw-   0        0        0     2665 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/statistics/end_activities/pandas/get.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:33.942541 pm4pyminimal-2.7.9.4/pm4py/statistics/eventually_follows/
+-rw-rw-rw-   0        0        0      801 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/statistics/eventually_follows/__init__.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:33.957550 pm4pyminimal-2.7.9.4/pm4py/statistics/eventually_follows/log/
+-rw-rw-rw-   0        0        0      791 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/statistics/eventually_follows/log/__init__.py
+-rw-rw-rw-   0        0        0     3015 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/statistics/eventually_follows/log/get.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:33.957550 pm4pyminimal-2.7.9.4/pm4py/statistics/eventually_follows/pandas/
+-rw-rw-rw-   0        0        0      794 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/statistics/eventually_follows/pandas/__init__.py
+-rw-rw-rw-   0        0        0     2879 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/statistics/eventually_follows/pandas/get.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:33.957550 pm4pyminimal-2.7.9.4/pm4py/statistics/eventually_follows/uvcl/
+-rw-rw-rw-   0        0        0      792 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/statistics/eventually_follows/uvcl/__init__.py
+-rw-rw-rw-   0        0        0     1936 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/statistics/eventually_follows/uvcl/get.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:33.977013 pm4pyminimal-2.7.9.4/pm4py/statistics/ocel/
+-rw-rw-rw-   0        0        0      734 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/statistics/ocel/__init__.py
+-rw-rw-rw-   0        0        0     3670 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/statistics/ocel/act_ot_dependent.py
+-rw-rw-rw-   0        0        0     5684 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/statistics/ocel/act_utils.py
+-rw-rw-rw-   0        0        0     9710 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/statistics/ocel/edge_metrics.py
+-rw-rw-rw-   0        0        0     2361 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/statistics/ocel/objects_ot_count.py
+-rw-rw-rw-   0        0        0     2395 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/statistics/ocel/ot_activities.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:33.992640 pm4pyminimal-2.7.9.4/pm4py/statistics/overlap/
+-rw-rw-rw-   0        0        0      957 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/statistics/overlap/__init__.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:33.992640 pm4pyminimal-2.7.9.4/pm4py/statistics/overlap/cases/
+-rw-rw-rw-   0        0        0      790 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/statistics/overlap/cases/__init__.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:33.992640 pm4pyminimal-2.7.9.4/pm4py/statistics/overlap/cases/log/
+-rw-rw-rw-   0        0        0      786 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/statistics/overlap/cases/log/__init__.py
+-rw-rw-rw-   0        0        0     2713 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/statistics/overlap/cases/log/get.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:34.010229 pm4pyminimal-2.7.9.4/pm4py/statistics/overlap/cases/pandas/
+-rw-rw-rw-   0        0        0      789 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/statistics/overlap/cases/pandas/__init__.py
+-rw-rw-rw-   0        0        0     3028 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/statistics/overlap/cases/pandas/get.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:34.011238 pm4pyminimal-2.7.9.4/pm4py/statistics/overlap/interval_events/
+-rw-rw-rw-   0        0        0      800 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/statistics/overlap/interval_events/__init__.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:34.011238 pm4pyminimal-2.7.9.4/pm4py/statistics/overlap/interval_events/log/
+-rw-rw-rw-   0        0        0      796 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/statistics/overlap/interval_events/log/__init__.py
+-rw-rw-rw-   0        0        0     2767 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/statistics/overlap/interval_events/log/get.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:34.011238 pm4pyminimal-2.7.9.4/pm4py/statistics/overlap/interval_events/pandas/
+-rw-rw-rw-   0        0        0      799 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/statistics/overlap/interval_events/pandas/__init__.py
+-rw-rw-rw-   0        0        0     2570 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/statistics/overlap/interval_events/pandas/get.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:34.026868 pm4pyminimal-2.7.9.4/pm4py/statistics/overlap/utils/
+-rw-rw-rw-   0        0        0      786 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/statistics/overlap/utils/__init__.py
+-rw-rw-rw-   0        0        0     1986 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/statistics/overlap/utils/compute.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:34.026868 pm4pyminimal-2.7.9.4/pm4py/statistics/passed_time/
+-rw-rw-rw-   0        0        0      790 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/statistics/passed_time/__init__.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:34.026868 pm4pyminimal-2.7.9.4/pm4py/statistics/passed_time/log/
+-rw-rw-rw-   0        0        0      800 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/statistics/passed_time/log/__init__.py
+-rw-rw-rw-   0        0        0     1781 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/statistics/passed_time/log/algorithm.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:34.042489 pm4pyminimal-2.7.9.4/pm4py/statistics/passed_time/log/variants/
+-rw-rw-rw-   0        0        0      808 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/statistics/passed_time/log/variants/__init__.py
+-rw-rw-rw-   0        0        0     2387 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/statistics/passed_time/log/variants/post.py
+-rw-rw-rw-   0        0        0     2369 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/statistics/passed_time/log/variants/pre.py
+-rw-rw-rw-   0        0        0     3050 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/statistics/passed_time/log/variants/prepost.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:34.042489 pm4pyminimal-2.7.9.4/pm4py/statistics/passed_time/pandas/
+-rw-rw-rw-   0        0        0      803 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/statistics/passed_time/pandas/__init__.py
+-rw-rw-rw-   0        0        0     1768 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/statistics/passed_time/pandas/algorithm.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:34.042489 pm4pyminimal-2.7.9.4/pm4py/statistics/passed_time/pandas/variants/
+-rw-rw-rw-   0        0        0      811 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/statistics/passed_time/pandas/variants/__init__.py
+-rw-rw-rw-   0        0        0     4131 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/statistics/passed_time/pandas/variants/post.py
+-rw-rw-rw-   0        0        0     4235 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/statistics/passed_time/pandas/variants/pre.py
+-rw-rw-rw-   0        0        0     4916 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/statistics/passed_time/pandas/variants/prepost.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:34.042489 pm4pyminimal-2.7.9.4/pm4py/statistics/rework/
+-rw-rw-rw-   0        0        0      783 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/statistics/rework/__init__.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:34.057500 pm4pyminimal-2.7.9.4/pm4py/statistics/rework/cases/
+-rw-rw-rw-   0        0        0      789 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/statistics/rework/cases/__init__.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:34.057500 pm4pyminimal-2.7.9.4/pm4py/statistics/rework/cases/log/
+-rw-rw-rw-   0        0        0      785 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/statistics/rework/cases/log/__init__.py
+-rw-rw-rw-   0        0        0     2597 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/statistics/rework/cases/log/get.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:34.057500 pm4pyminimal-2.7.9.4/pm4py/statistics/rework/cases/pandas/
+-rw-rw-rw-   0        0        0      788 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/statistics/rework/cases/pandas/__init__.py
+-rw-rw-rw-   0        0        0     2542 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/statistics/rework/cases/pandas/get.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:34.057500 pm4pyminimal-2.7.9.4/pm4py/statistics/rework/log/
+-rw-rw-rw-   0        0        0      779 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/statistics/rework/log/__init__.py
+-rw-rw-rw-   0        0        0     2265 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/statistics/rework/log/get.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:34.057500 pm4pyminimal-2.7.9.4/pm4py/statistics/rework/pandas/
+-rw-rw-rw-   0        0        0      782 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/statistics/rework/pandas/__init__.py
+-rw-rw-rw-   0        0        0     2378 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/statistics/rework/pandas/get.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:34.057500 pm4pyminimal-2.7.9.4/pm4py/statistics/service_time/
+-rw-rw-rw-   0        0        0      789 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/statistics/service_time/__init__.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:34.076118 pm4pyminimal-2.7.9.4/pm4py/statistics/service_time/log/
+-rw-rw-rw-   0        0        0      785 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/statistics/service_time/log/__init__.py
+-rw-rw-rw-   0        0        0     5453 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/statistics/service_time/log/get.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:34.076118 pm4pyminimal-2.7.9.4/pm4py/statistics/service_time/pandas/
+-rw-rw-rw-   0        0        0      788 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/statistics/service_time/pandas/__init__.py
+-rw-rw-rw-   0        0        0     4930 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/statistics/service_time/pandas/get.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:34.076118 pm4pyminimal-2.7.9.4/pm4py/statistics/sojourn_time/
+-rw-rw-rw-   0        0        0      779 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/statistics/sojourn_time/__init__.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:34.076118 pm4pyminimal-2.7.9.4/pm4py/statistics/start_activities/
+-rw-rw-rw-   0        0        0      801 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/statistics/start_activities/__init__.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:34.076118 pm4pyminimal-2.7.9.4/pm4py/statistics/start_activities/common/
+-rw-rw-rw-   0        0        0      792 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/statistics/start_activities/common/__init__.py
+-rw-rw-rw-   0        0        0     1813 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/statistics/start_activities/common/get.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:34.091740 pm4pyminimal-2.7.9.4/pm4py/statistics/start_activities/log/
+-rw-rw-rw-   0        0        0      789 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/statistics/start_activities/log/__init__.py
+-rw-rw-rw-   0        0        0     2769 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/statistics/start_activities/log/get.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:34.091740 pm4pyminimal-2.7.9.4/pm4py/statistics/start_activities/pandas/
+-rw-rw-rw-   0        0        0      792 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/statistics/start_activities/pandas/__init__.py
+-rw-rw-rw-   0        0        0     2623 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/statistics/start_activities/pandas/get.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:34.091740 pm4pyminimal-2.7.9.4/pm4py/statistics/traces/
+-rw-rw-rw-   0        0        0      791 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/statistics/traces/__init__.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:34.091740 pm4pyminimal-2.7.9.4/pm4py/statistics/traces/cycle_time/
+-rw-rw-rw-   0        0        0      800 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/statistics/traces/cycle_time/__init__.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:34.091740 pm4pyminimal-2.7.9.4/pm4py/statistics/traces/cycle_time/log/
+-rw-rw-rw-   0        0        0      790 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/statistics/traces/cycle_time/log/__init__.py
+-rw-rw-rw-   0        0        0     3191 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/statistics/traces/cycle_time/log/get.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:34.110166 pm4pyminimal-2.7.9.4/pm4py/statistics/traces/cycle_time/pandas/
+-rw-rw-rw-   0        0        0      793 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/statistics/traces/cycle_time/pandas/__init__.py
+-rw-rw-rw-   0        0        0     3255 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/statistics/traces/cycle_time/pandas/get.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:34.111176 pm4pyminimal-2.7.9.4/pm4py/statistics/traces/cycle_time/util/
+-rw-rw-rw-   0        0        0      795 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/statistics/traces/cycle_time/util/__init__.py
+-rw-rw-rw-   0        0        0     2385 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/statistics/traces/cycle_time/util/compute.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:34.111176 pm4pyminimal-2.7.9.4/pm4py/statistics/traces/generic/
+-rw-rw-rw-   0        0        0      799 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/statistics/traces/generic/__init__.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:34.111176 pm4pyminimal-2.7.9.4/pm4py/statistics/traces/generic/common/
+-rw-rw-rw-   0        0        0      800 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/statistics/traces/generic/common/__init__.py
+-rw-rw-rw-   0        0        0     2969 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/statistics/traces/generic/common/case_duration.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:34.111176 pm4pyminimal-2.7.9.4/pm4py/statistics/traces/generic/log/
+-rw-rw-rw-   0        0        0      799 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/statistics/traces/generic/log/__init__.py
+-rw-rw-rw-   0        0        0     5237 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/statistics/traces/generic/log/case_arrival.py
+-rw-rw-rw-   0        0        0    13221 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/statistics/traces/generic/log/case_statistics.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:34.126802 pm4pyminimal-2.7.9.4/pm4py/statistics/traces/generic/pandas/
+-rw-rw-rw-   0        0        0      799 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/statistics/traces/generic/pandas/__init__.py
+-rw-rw-rw-   0        0        0     4223 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/statistics/traces/generic/pandas/case_arrival.py
+-rw-rw-rw-   0        0        0    16954 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/statistics/traces/generic/pandas/case_statistics.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:34.126802 pm4pyminimal-2.7.9.4/pm4py/statistics/util/
+-rw-rw-rw-   0        0        0      974 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/statistics/util/__init__.py
+-rw-rw-rw-   0        0        0     2382 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/statistics/util/times_bipartite_matching.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:34.126802 pm4pyminimal-2.7.9.4/pm4py/statistics/variants/
+-rw-rw-rw-   0        0        0      785 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/statistics/variants/__init__.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:34.126802 pm4pyminimal-2.7.9.4/pm4py/statistics/variants/log/
+-rw-rw-rw-   0        0        0      781 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/statistics/variants/log/__init__.py
+-rw-rw-rw-   0        0        0     7359 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/statistics/variants/log/get.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:34.142424 pm4pyminimal-2.7.9.4/pm4py/statistics/variants/pandas/
+-rw-rw-rw-   0        0        0      784 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/statistics/variants/pandas/__init__.py
+-rw-rw-rw-   0        0        0     2254 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/statistics/variants/pandas/get.py
+-rw-rw-rw-   0        0        0    39292 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/stats.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:34.142424 pm4pyminimal-2.7.9.4/pm4py/streaming/
+-rw-rw-rw-   0        0        0      804 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/streaming/__init__.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:34.142424 pm4pyminimal-2.7.9.4/pm4py/streaming/algo/
+-rw-rw-rw-   0        0        0      800 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/streaming/algo/__init__.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:34.142424 pm4pyminimal-2.7.9.4/pm4py/streaming/algo/conformance/
+-rw-rw-rw-   0        0        0      806 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/streaming/algo/conformance/__init__.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:34.142424 pm4pyminimal-2.7.9.4/pm4py/streaming/algo/conformance/footprints/
+-rw-rw-rw-   0        0        0      811 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/streaming/algo/conformance/footprints/__init__.py
+-rw-rw-rw-   0        0        0     1515 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/streaming/algo/conformance/footprints/algorithm.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:34.142424 pm4pyminimal-2.7.9.4/pm4py/streaming/algo/conformance/footprints/variants/
+-rw-rw-rw-   0        0        0      808 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/streaming/algo/conformance/footprints/variants/__init__.py
+-rw-rw-rw-   0        0        0    11003 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/streaming/algo/conformance/footprints/variants/classic.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:34.157431 pm4pyminimal-2.7.9.4/pm4py/streaming/algo/conformance/tbr/
+-rw-rw-rw-   0        0        0      804 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/streaming/algo/conformance/tbr/__init__.py
+-rw-rw-rw-   0        0        0     1523 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/streaming/algo/conformance/tbr/algorithm.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:34.157431 pm4pyminimal-2.7.9.4/pm4py/streaming/algo/conformance/tbr/variants/
+-rw-rw-rw-   0        0        0      801 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/streaming/algo/conformance/tbr/variants/__init__.py
+-rw-rw-rw-   0        0        0    17271 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/streaming/algo/conformance/tbr/variants/classic.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:34.157431 pm4pyminimal-2.7.9.4/pm4py/streaming/algo/conformance/temporal/
+-rw-rw-rw-   0        0        0      809 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/streaming/algo/conformance/temporal/__init__.py
+-rw-rw-rw-   0        0        0     2135 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/streaming/algo/conformance/temporal/algorithm.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:34.157431 pm4pyminimal-2.7.9.4/pm4py/streaming/algo/conformance/temporal/variants/
+-rw-rw-rw-   0        0        0      806 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/streaming/algo/conformance/temporal/variants/__init__.py
+-rw-rw-rw-   0        0        0     9602 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/streaming/algo/conformance/temporal/variants/classic.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:34.157431 pm4pyminimal-2.7.9.4/pm4py/streaming/algo/discovery/
+-rw-rw-rw-   0        0        0      782 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/streaming/algo/discovery/__init__.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:34.173058 pm4pyminimal-2.7.9.4/pm4py/streaming/algo/discovery/dfg/
+-rw-rw-rw-   0        0        0      802 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/streaming/algo/discovery/dfg/__init__.py
+-rw-rw-rw-   0        0        0     1411 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/streaming/algo/discovery/dfg/algorithm.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:34.173058 pm4pyminimal-2.7.9.4/pm4py/streaming/algo/discovery/dfg/variants/
+-rw-rw-rw-   0        0        0      801 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/streaming/algo/discovery/dfg/variants/__init__.py
+-rw-rw-rw-   0        0        0     7371 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/streaming/algo/discovery/dfg/variants/frequency.py
+-rw-rw-rw-   0        0        0     1476 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/streaming/algo/interface.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:34.173058 pm4pyminimal-2.7.9.4/pm4py/streaming/conversion/
+-rw-rw-rw-   0        0        0     1468 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/streaming/conversion/__init__.py
+-rw-rw-rw-   0        0        0     4925 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/streaming/conversion/from_pandas.py
+-rw-rw-rw-   0        0        0     5211 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/streaming/conversion/ocel_flatts_distributor.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:34.173058 pm4pyminimal-2.7.9.4/pm4py/streaming/importer/
+-rw-rw-rw-   0        0        0      885 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/streaming/importer/__init__.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:34.188679 pm4pyminimal-2.7.9.4/pm4py/streaming/importer/csv/
+-rw-rw-rw-   0        0        0      795 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/streaming/importer/csv/__init__.py
+-rw-rw-rw-   0        0        0     1488 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/streaming/importer/csv/importer.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:34.188679 pm4pyminimal-2.7.9.4/pm4py/streaming/importer/csv/variants/
+-rw-rw-rw-   0        0        0      802 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/streaming/importer/csv/variants/__init__.py
+-rw-rw-rw-   0        0        0     3406 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/streaming/importer/csv/variants/csv_event_stream.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:34.188679 pm4pyminimal-2.7.9.4/pm4py/streaming/importer/xes/
+-rw-rw-rw-   0        0        0      795 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/streaming/importer/xes/__init__.py
+-rw-rw-rw-   0        0        0     1523 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/streaming/importer/xes/importer.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:34.204805 pm4pyminimal-2.7.9.4/pm4py/streaming/importer/xes/variants/
+-rw-rw-rw-   0        0        0      820 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/streaming/importer/xes/variants/__init__.py
+-rw-rw-rw-   0        0        0     9461 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/streaming/importer/xes/variants/xes_event_stream.py
+-rw-rw-rw-   0        0        0     9317 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/streaming/importer/xes/variants/xes_trace_stream.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:34.204805 pm4pyminimal-2.7.9.4/pm4py/streaming/stream/
+-rw-rw-rw-   0        0        0      807 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/streaming/stream/__init__.py
+-rw-rw-rw-   0        0        0     3109 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/streaming/stream/live_event_stream.py
+-rw-rw-rw-   0        0        0     3109 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/streaming/stream/live_trace_stream.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:34.220426 pm4pyminimal-2.7.9.4/pm4py/streaming/util/
+-rw-rw-rw-   0        0        0      819 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/streaming/util/__init__.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:34.220426 pm4pyminimal-2.7.9.4/pm4py/streaming/util/dictio/
+-rw-rw-rw-   0        0        0      795 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/streaming/util/dictio/__init__.py
+-rw-rw-rw-   0        0        0     1461 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/streaming/util/dictio/generator.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:34.220426 pm4pyminimal-2.7.9.4/pm4py/streaming/util/dictio/versions/
+-rw-rw-rw-   0        0        0      805 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/streaming/util/dictio/versions/__init__.py
+-rw-rw-rw-   0        0        0      941 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/streaming/util/dictio/versions/classic.py
+-rw-rw-rw-   0        0        0     3540 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/streaming/util/dictio/versions/redis.py
+-rw-rw-rw-   0        0        0     1949 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/streaming/util/dictio/versions/thread_safe.py
+-rw-rw-rw-   0        0        0     1039 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/streaming/util/event_stream_printer.py
+-rw-rw-rw-   0        0        0     1180 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/streaming/util/live_to_static_stream.py
+-rw-rw-rw-   0        0        0     1039 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/streaming/util/trace_stream_printer.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:34.257676 pm4pyminimal-2.7.9.4/pm4py/util/
+-rw-rw-rw-   0        0        0      928 2024-01-17 08:28:40.000000 pm4pyminimal-2.7.9.4/pm4py/util/__init__.py
+-rw-rw-rw-   0        0        0     5056 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/util/business_hours.py
+-rw-rw-rw-   0        0        0     2225 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/util/colors.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:34.273302 pm4pyminimal-2.7.9.4/pm4py/util/compression/
+-rw-rw-rw-   0        0        0      781 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/util/compression/__init__.py
+-rw-rw-rw-   0        0        0     1314 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/util/compression/dtypes.py
+-rw-rw-rw-   0        0        0    11522 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/util/compression/util.py
+-rw-rw-rw-   0        0        0     7079 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/util/constants.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:34.273302 pm4pyminimal-2.7.9.4/pm4py/util/dt_parsing/
+-rw-rw-rw-   0        0        0      786 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/util/dt_parsing/__init__.py
+-rw-rw-rw-   0        0        0     2682 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/util/dt_parsing/parser.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:34.288924 pm4pyminimal-2.7.9.4/pm4py/util/dt_parsing/variants/
+-rw-rw-rw-   0        0        0      734 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/util/dt_parsing/variants/__init__.py
+-rw-rw-rw-   0        0        0     1029 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/util/dt_parsing/variants/cs8601.py
+-rw-rw-rw-   0        0        0     1470 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/util/dt_parsing/variants/dummy.py
+-rw-rw-rw-   0        0        0     1916 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/util/dt_parsing/variants/strpfromiso.py
+-rw-rw-rw-   0        0        0     1564 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/util/exec_utils.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:34.288924 pm4pyminimal-2.7.9.4/pm4py/util/lp/
+-rw-rw-rw-   0        0        0      784 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/util/lp/__init__.py
+-rw-rw-rw-   0        0        0     5457 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/util/lp/solver.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:34.288924 pm4pyminimal-2.7.9.4/pm4py/util/lp/util/
+-rw-rw-rw-   0        0        0      734 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/util/lp/util/__init__.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:34.320167 pm4pyminimal-2.7.9.4/pm4py/util/lp/variants/
+-rw-rw-rw-   0        0        0      943 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/util/lp/variants/__init__.py
+-rw-rw-rw-   0        0        0     3639 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/util/lp/variants/cvxopt_solver.py
+-rw-rw-rw-   0        0        0     3420 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/util/lp/variants/cvxopt_solver_custom_align.py
+-rw-rw-rw-   0        0        0     3059 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/util/lp/variants/cvxopt_solver_custom_align_arm.py
+-rw-rw-rw-   0        0        0     3937 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/util/lp/variants/cvxopt_solver_custom_align_ilp.py
+-rw-rw-rw-   0        0        0     5153 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/util/lp/variants/ortools_solver.py
+-rw-rw-rw-   0        0        0     6293 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/util/lp/variants/pulp_solver.py
+-rw-rw-rw-   0        0        0     1853 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/util/lp/variants/scipy_solver.py
+-rw-rw-rw-   0        0        0    10037 2024-01-18 11:43:23.000000 pm4pyminimal-2.7.9.4/pm4py/util/nx_utils.py
+-rw-rw-rw-   0        0        0    13899 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/util/pandas_utils.py
+-rw-rw-rw-   0        0        0     1494 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/util/points_subset.py
+-rw-rw-rw-   0        0        0     1602 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/util/regex.py
+-rw-rw-rw-   0        0        0     3663 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/util/string_distance.py
+-rw-rw-rw-   0        0        0     1095 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/util/typing.py
+-rw-rw-rw-   0        0        0     2261 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/util/variants_util.py
+-rw-rw-rw-   0        0        0     6027 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/util/vis_utils.py
+-rw-rw-rw-   0        0        0     1614 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/util/xes_constants.py
+-rw-rw-rw-   0        0        0    25437 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/utils.py
+-rw-rw-rw-   0        0        0    69901 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/vis.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:34.320167 pm4pyminimal-2.7.9.4/pm4py/visualization/
+-rw-rw-rw-   0        0        0     1869 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/visualization/__init__.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:34.320167 pm4pyminimal-2.7.9.4/pm4py/visualization/align_table/
+-rw-rw-rw-   0        0        0      790 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/visualization/align_table/__init__.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:34.335789 pm4pyminimal-2.7.9.4/pm4py/visualization/align_table/variants/
+-rw-rw-rw-   0        0        0      796 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/visualization/align_table/variants/__init__.py
+-rw-rw-rw-   0        0        0     3863 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/visualization/align_table/variants/classic.py
+-rw-rw-rw-   0        0        0     2968 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/visualization/align_table/visualizer.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:34.335789 pm4pyminimal-2.7.9.4/pm4py/visualization/bpmn/
+-rw-rw-rw-   0        0        0      793 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/visualization/bpmn/__init__.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:34.345960 pm4pyminimal-2.7.9.4/pm4py/visualization/bpmn/variants/
+-rw-rw-rw-   0        0        0      789 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/visualization/bpmn/variants/__init__.py
+-rw-rw-rw-   0        0        0     3654 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/visualization/bpmn/variants/classic.py
+-rw-rw-rw-   0        0        0     2583 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/visualization/bpmn/visualizer.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:34.357965 pm4pyminimal-2.7.9.4/pm4py/visualization/common/
+-rw-rw-rw-   0        0        0      817 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/visualization/common/__init__.py
+-rw-rw-rw-   0        0        0     1160 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/visualization/common/dot_util.py
+-rw-rw-rw-   0        0        0     3058 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/visualization/common/gview.py
+-rw-rw-rw-   0        0        0     3394 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/visualization/common/html.py
+-rw-rw-rw-   0        0        0     1531 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/visualization/common/save.py
+-rw-rw-rw-   0        0        0     2526 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/visualization/common/svg_pos_parser.py
+-rw-rw-rw-   0        0        0      879 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/visualization/common/utils.py
+-rw-rw-rw-   0        0        0     1540 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/visualization/common/visualizer.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:34.373593 pm4pyminimal-2.7.9.4/pm4py/visualization/decisiontree/
+-rw-rw-rw-   0        0        0     1008 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/visualization/decisiontree/__init__.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:34.373593 pm4pyminimal-2.7.9.4/pm4py/visualization/decisiontree/util/
+-rw-rw-rw-   0        0        0      734 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/visualization/decisiontree/util/__init__.py
+-rw-rw-rw-   0        0        0     2621 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/visualization/decisiontree/util/dt_to_string.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:34.373593 pm4pyminimal-2.7.9.4/pm4py/visualization/decisiontree/variants/
+-rw-rw-rw-   0        0        0      797 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/visualization/decisiontree/variants/__init__.py
+-rw-rw-rw-   0        0        0     2231 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/visualization/decisiontree/variants/classic.py
+-rw-rw-rw-   0        0        0     2840 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/visualization/decisiontree/visualizer.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:34.389216 pm4pyminimal-2.7.9.4/pm4py/visualization/dfg/
+-rw-rw-rw-   0        0        0      800 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/visualization/dfg/__init__.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:34.393537 pm4pyminimal-2.7.9.4/pm4py/visualization/dfg/util/
+-rw-rw-rw-   0        0        0      787 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/visualization/dfg/util/__init__.py
+-rw-rw-rw-   0        0        0     8994 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/visualization/dfg/util/dfg_gviz.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:34.393537 pm4pyminimal-2.7.9.4/pm4py/visualization/dfg/variants/
+-rw-rw-rw-   0        0        0      803 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/visualization/dfg/variants/__init__.py
+-rw-rw-rw-   0        0        0     5409 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/visualization/dfg/variants/cost.py
+-rw-rw-rw-   0        0        0     5157 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/visualization/dfg/variants/frequency.py
+-rw-rw-rw-   0        0        0     5580 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/visualization/dfg/variants/performance.py
+-rw-rw-rw-   0        0        0    12854 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/visualization/dfg/variants/timeline.py
+-rw-rw-rw-   0        0        0     3196 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/visualization/dfg/visualizer.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:34.393537 pm4pyminimal-2.7.9.4/pm4py/visualization/dotted_chart/
+-rw-rw-rw-   0        0        0      801 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/visualization/dotted_chart/__init__.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:34.409159 pm4pyminimal-2.7.9.4/pm4py/visualization/dotted_chart/variants/
+-rw-rw-rw-   0        0        0      797 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/visualization/dotted_chart/variants/__init__.py
+-rw-rw-rw-   0        0        0     9236 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/visualization/dotted_chart/variants/classic.py
+-rw-rw-rw-   0        0        0     3819 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/visualization/dotted_chart/visualizer.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:34.409159 pm4pyminimal-2.7.9.4/pm4py/visualization/footprints/
+-rw-rw-rw-   0        0        0      799 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/visualization/footprints/__init__.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:34.409159 pm4pyminimal-2.7.9.4/pm4py/visualization/footprints/variants/
+-rw-rw-rw-   0        0        0      828 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/visualization/footprints/variants/__init__.py
+-rw-rw-rw-   0        0        0     3842 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/visualization/footprints/variants/comparison.py
+-rw-rw-rw-   0        0        0     4374 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/visualization/footprints/variants/comparison_symmetric.py
+-rw-rw-rw-   0        0        0     3280 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/visualization/footprints/variants/single.py
+-rw-rw-rw-   0        0        0     3120 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/visualization/footprints/visualizer.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:34.409159 pm4pyminimal-2.7.9.4/pm4py/visualization/graphs/
+-rw-rw-rw-   0        0        0      801 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/visualization/graphs/__init__.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:34.424781 pm4pyminimal-2.7.9.4/pm4py/visualization/graphs/util/
+-rw-rw-rw-   0        0        0      786 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/visualization/graphs/util/__init__.py
+-rw-rw-rw-   0        0        0     2849 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/visualization/graphs/util/common.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:34.424781 pm4pyminimal-2.7.9.4/pm4py/visualization/graphs/variants/
+-rw-rw-rw-   0        0        0      817 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/visualization/graphs/variants/__init__.py
+-rw-rw-rw-   0        0        0     4541 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/visualization/graphs/variants/attributes.py
+-rw-rw-rw-   0        0        0     2763 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/visualization/graphs/variants/barplot.py
+-rw-rw-rw-   0        0        0     4542 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/visualization/graphs/variants/cases.py
+-rw-rw-rw-   0        0        0     4587 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/visualization/graphs/variants/dates.py
+-rw-rw-rw-   0        0        0     3859 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/visualization/graphs/visualizer.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:34.443969 pm4pyminimal-2.7.9.4/pm4py/visualization/heuristics_net/
+-rw-rw-rw-   0        0        0      803 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/visualization/heuristics_net/__init__.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:34.446004 pm4pyminimal-2.7.9.4/pm4py/visualization/heuristics_net/variants/
+-rw-rw-rw-   0        0        0      805 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/visualization/heuristics_net/variants/__init__.py
+-rw-rw-rw-   0        0        0    13357 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/visualization/heuristics_net/variants/pydotplus_vis.py
+-rw-rw-rw-   0        0        0     4471 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/visualization/heuristics_net/visualizer.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:34.446004 pm4pyminimal-2.7.9.4/pm4py/visualization/network_analysis/
+-rw-rw-rw-   0        0        0      805 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/visualization/network_analysis/__init__.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:34.458007 pm4pyminimal-2.7.9.4/pm4py/visualization/network_analysis/variants/
+-rw-rw-rw-   0        0        0      816 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/visualization/network_analysis/variants/__init__.py
+-rw-rw-rw-   0        0        0     4975 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/visualization/network_analysis/variants/frequency.py
+-rw-rw-rw-   0        0        0     6154 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/visualization/network_analysis/variants/performance.py
+-rw-rw-rw-   0        0        0     2496 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/visualization/network_analysis/visualizer.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:34.458007 pm4pyminimal-2.7.9.4/pm4py/visualization/networkx/
+-rw-rw-rw-   0        0        0      734 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/visualization/networkx/__init__.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:34.458007 pm4pyminimal-2.7.9.4/pm4py/visualization/networkx/variants/
+-rw-rw-rw-   0        0        0      734 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/visualization/networkx/variants/__init__.py
+-rw-rw-rw-   0        0        0     3990 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/visualization/networkx/variants/digraph.py
+-rw-rw-rw-   0        0        0     2362 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/visualization/networkx/visualizer.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:34.458007 pm4pyminimal-2.7.9.4/pm4py/visualization/ocel/
+-rw-rw-rw-   0        0        0      813 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/visualization/ocel/__init__.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:34.458007 pm4pyminimal-2.7.9.4/pm4py/visualization/ocel/eve_to_obj_types/
+-rw-rw-rw-   0        0        0      734 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/visualization/ocel/eve_to_obj_types/__init__.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:34.478263 pm4pyminimal-2.7.9.4/pm4py/visualization/ocel/eve_to_obj_types/variants/
+-rw-rw-rw-   0        0        0      734 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/visualization/ocel/eve_to_obj_types/variants/__init__.py
+-rw-rw-rw-   0        0        0     3613 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/visualization/ocel/eve_to_obj_types/variants/graphviz.py
+-rw-rw-rw-   0        0        0     2724 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/visualization/ocel/eve_to_obj_types/visualizer.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:34.479269 pm4pyminimal-2.7.9.4/pm4py/visualization/ocel/interleavings/
+-rw-rw-rw-   0        0        0      807 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/visualization/ocel/interleavings/__init__.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:34.479269 pm4pyminimal-2.7.9.4/pm4py/visualization/ocel/interleavings/variants/
+-rw-rw-rw-   0        0        0      804 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/visualization/ocel/interleavings/variants/__init__.py
+-rw-rw-rw-   0        0        0    15031 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/visualization/ocel/interleavings/variants/graphviz.py
+-rw-rw-rw-   0        0        0     2989 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/visualization/ocel/interleavings/visualizer.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:34.479269 pm4pyminimal-2.7.9.4/pm4py/visualization/ocel/object_graph/
+-rw-rw-rw-   0        0        0      734 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/visualization/ocel/object_graph/__init__.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:34.479269 pm4pyminimal-2.7.9.4/pm4py/visualization/ocel/object_graph/variants/
+-rw-rw-rw-   0        0        0      734 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/visualization/ocel/object_graph/variants/__init__.py
+-rw-rw-rw-   0        0        0     3447 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/visualization/ocel/object_graph/variants/graphviz.py
+-rw-rw-rw-   0        0        0     2556 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/visualization/ocel/object_graph/visualizer.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:34.494896 pm4pyminimal-2.7.9.4/pm4py/visualization/ocel/ocdfg/
+-rw-rw-rw-   0        0        0      799 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/visualization/ocel/ocdfg/__init__.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:34.494896 pm4pyminimal-2.7.9.4/pm4py/visualization/ocel/ocdfg/variants/
+-rw-rw-rw-   0        0        0      795 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/visualization/ocel/ocdfg/variants/__init__.py
+-rw-rw-rw-   0        0        0    12507 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/visualization/ocel/ocdfg/variants/classic.py
+-rw-rw-rw-   0        0        0     2454 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/visualization/ocel/ocdfg/visualizer.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:34.494896 pm4pyminimal-2.7.9.4/pm4py/visualization/ocel/ocpn/
+-rw-rw-rw-   0        0        0      798 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/visualization/ocel/ocpn/__init__.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:34.494896 pm4pyminimal-2.7.9.4/pm4py/visualization/ocel/ocpn/variants/
+-rw-rw-rw-   0        0        0      800 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/visualization/ocel/ocpn/variants/__init__.py
+-rw-rw-rw-   0        0        0     5941 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/visualization/ocel/ocpn/variants/wo_decoration.py
+-rw-rw-rw-   0        0        0     2601 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/visualization/ocel/ocpn/visualizer.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:34.510517 pm4pyminimal-2.7.9.4/pm4py/visualization/performance_spectrum/
+-rw-rw-rw-   0        0        0      809 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/visualization/performance_spectrum/__init__.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:34.510517 pm4pyminimal-2.7.9.4/pm4py/visualization/performance_spectrum/variants/
+-rw-rw-rw-   0        0        0      803 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/visualization/performance_spectrum/variants/__init__.py
+-rw-rw-rw-   0        0        0     7116 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/visualization/performance_spectrum/variants/neato.py
+-rw-rw-rw-   0        0        0     3244 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/visualization/performance_spectrum/visualizer.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:34.510517 pm4pyminimal-2.7.9.4/pm4py/visualization/petri_net/
+-rw-rw-rw-   0        0        0      812 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/visualization/petri_net/__init__.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:34.510517 pm4pyminimal-2.7.9.4/pm4py/visualization/petri_net/common/
+-rw-rw-rw-   0        0        0      794 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/visualization/petri_net/common/__init__.py
+-rw-rw-rw-   0        0        0     9446 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/visualization/petri_net/common/visualize.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:34.526139 pm4pyminimal-2.7.9.4/pm4py/visualization/petri_net/util/
+-rw-rw-rw-   0        0        0      847 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/visualization/petri_net/util/__init__.py
+-rw-rw-rw-   0        0        0     2935 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/visualization/petri_net/util/alignments_decoration.py
+-rw-rw-rw-   0        0        0     1121 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/visualization/petri_net/util/performance_map.py
+-rw-rw-rw-   0        0        0    11279 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/visualization/petri_net/util/vis_trans_shortest_paths.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:34.526139 pm4pyminimal-2.7.9.4/pm4py/visualization/petri_net/variants/
+-rw-rw-rw-   0        0        0      937 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/visualization/petri_net/variants/__init__.py
+-rw-rw-rw-   0        0        0     2044 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/visualization/petri_net/variants/alignments.py
+-rw-rw-rw-   0        0        0     4730 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/visualization/petri_net/variants/greedy_decoration_frequency.py
+-rw-rw-rw-   0        0        0     4837 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/visualization/petri_net/variants/greedy_decoration_performance.py
+-rw-rw-rw-   0        0        0     5670 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/visualization/petri_net/variants/token_decoration_frequency.py
+-rw-rw-rw-   0        0        0     5880 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/visualization/petri_net/variants/token_decoration_performance.py
+-rw-rw-rw-   0        0        0     2237 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/visualization/petri_net/variants/wo_decoration.py
+-rw-rw-rw-   0        0        0     3651 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/visualization/petri_net/visualizer.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:34.541762 pm4pyminimal-2.7.9.4/pm4py/visualization/powl/
+-rw-rw-rw-   0        0        0      795 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/visualization/powl/__init__.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:34.557892 pm4pyminimal-2.7.9.4/pm4py/visualization/powl/variants/
+-rw-rw-rw-   0        0        0      785 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/visualization/powl/variants/__init__.py
+-rw-rw-rw-   0        0        0     7745 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/visualization/powl/variants/basic.py
+-rw-rw-rw-   0        0        0      755 2024-01-02 13:29:21.000000 pm4pyminimal-2.7.9.4/pm4py/visualization/powl/variants/end.png
+-rw-rw-rw-   0        0        0    25337 2024-01-02 13:29:21.000000 pm4pyminimal-2.7.9.4/pm4py/visualization/powl/variants/loop.png
+-rw-rw-rw-   0        0        0    11069 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/visualization/powl/variants/net.py
+-rw-rw-rw-   0        0        0      922 2024-01-02 13:29:21.000000 pm4pyminimal-2.7.9.4/pm4py/visualization/powl/variants/play.png
+-rw-rw-rw-   0        0        0    78865 2024-01-02 13:29:21.000000 pm4pyminimal-2.7.9.4/pm4py/visualization/powl/variants/xor.png
+-rw-rw-rw-   0        0        0     2853 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/visualization/powl/visualizer.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:34.557892 pm4pyminimal-2.7.9.4/pm4py/visualization/process_tree/
+-rw-rw-rw-   0        0        0      801 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/visualization/process_tree/__init__.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:34.573522 pm4pyminimal-2.7.9.4/pm4py/visualization/process_tree/variants/
+-rw-rw-rw-   0        0        0      813 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/visualization/process_tree/variants/__init__.py
+-rw-rw-rw-   0        0        0     4873 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/visualization/process_tree/variants/frequency_annotation.py
+-rw-rw-rw-   0        0        0     4104 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/visualization/process_tree/variants/symbolic.py
+-rw-rw-rw-   0        0        0     4256 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/visualization/process_tree/variants/wo_decoration.py
+-rw-rw-rw-   0        0        0     3017 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/visualization/process_tree/visualizer.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:34.573522 pm4pyminimal-2.7.9.4/pm4py/visualization/sna/
+-rw-rw-rw-   0        0        0      792 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/visualization/sna/__init__.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:34.573522 pm4pyminimal-2.7.9.4/pm4py/visualization/sna/variants/
+-rw-rw-rw-   0        0        0      796 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/visualization/sna/variants/__init__.py
+-rw-rw-rw-   0        0        0     4180 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/visualization/sna/variants/networkx.py
+-rw-rw-rw-   0        0        0     5472 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/visualization/sna/variants/pyvis.py
+-rw-rw-rw-   0        0        0     2561 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/visualization/sna/visualizer.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:34.589144 pm4pyminimal-2.7.9.4/pm4py/visualization/transition_system/
+-rw-rw-rw-   0        0        0      812 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/visualization/transition_system/__init__.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:34.589144 pm4pyminimal-2.7.9.4/pm4py/visualization/transition_system/util/
+-rw-rw-rw-   0        0        0      809 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/visualization/transition_system/util/__init__.py
+-rw-rw-rw-   0        0        0     3315 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/visualization/transition_system/util/visualize_graphviz.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:34.589144 pm4pyminimal-2.7.9.4/pm4py/visualization/transition_system/variants/
+-rw-rw-rw-   0        0        0      822 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/visualization/transition_system/variants/__init__.py
+-rw-rw-rw-   0        0        0     3138 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/visualization/transition_system/variants/trans_frequency.py
+-rw-rw-rw-   0        0        0     1652 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/visualization/transition_system/variants/view_based.py
+-rw-rw-rw-   0        0        0     2703 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/visualization/transition_system/visualizer.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:34.606047 pm4pyminimal-2.7.9.4/pm4py/visualization/trie/
+-rw-rw-rw-   0        0        0      793 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/visualization/trie/__init__.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:34.606047 pm4pyminimal-2.7.9.4/pm4py/visualization/trie/variants/
+-rw-rw-rw-   0        0        0      789 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/visualization/trie/variants/__init__.py
+-rw-rw-rw-   0        0        0     2765 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/visualization/trie/variants/classic.py
+-rw-rw-rw-   0        0        0     2512 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/visualization/trie/visualizer.py
+-rw-rw-rw-   0        0        0    15531 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/pm4py/write.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:34.637290 pm4pyminimal-2.7.9.4/pm4pyminimal.egg-info/
+-rw-rw-rw-   0        0        0     3371 2024-01-29 06:15:29.000000 pm4pyminimal-2.7.9.4/pm4pyminimal.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0    66584 2024-01-29 06:15:31.000000 pm4pyminimal-2.7.9.4/pm4pyminimal.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-01-29 06:15:29.000000 pm4pyminimal-2.7.9.4/pm4pyminimal.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       34 2024-01-29 06:15:29.000000 pm4pyminimal-2.7.9.4/pm4pyminimal.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-01-29 06:15:29.000000 pm4pyminimal-2.7.9.4/pm4pyminimal.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-01-29 06:15:34.652912 pm4pyminimal-2.7.9.4/setup.cfg
+-rw-rw-rw-   0        0        0     1246 2024-01-17 08:27:48.000000 pm4pyminimal-2.7.9.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:15:34.637290 pm4pyminimal-2.7.9.4/tests/
+-rw-rw-rw-   0        0        0     4971 2023-11-09 06:59:42.000000 pm4pyminimal-2.7.9.4/tests/test_cli.py
```

### Comparing `pm4pyminimal-2.7.9.3/LICENSE` & `pm4pyminimal-2.7.9.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/PKG-INFO` & `pm4pyminimal-2.7.9.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pm4pyminimal
-Version: 2.7.9.3
+Version: 2.7.9.4
 Summary: Process mining for Python
 Home-page: https://pm4py.fit.fraunhofer.de
 Author: Fraunhofer Institute for Applied Information Technology FIT
 Author-email: pm4py@fit.fraunhofer.de
 License: GPL 3.0
 Project-URL: Documentation, https://pm4py.fit.fraunhofer.de
 Project-URL: Source, https://github.com/pm4py/pm4py-source
@@ -68,7 +68,8 @@
 pages = {100556},  
 year = {2023},  
 issn = {2665-9638},  
 doi = {https://doi.org/10.1016/j.simpa.2023.100556},  
 url = {https://www.sciencedirect.com/science/article/pii/S2665963823000933},  
 author = {Alessandro Berti and Sebastiaan van Zelst and Daniel Schuster},  
 }
+
```

### Comparing `pm4pyminimal-2.7.9.3/README.md` & `pm4pyminimal-2.7.9.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -51,7 +51,8 @@
 pages = {100556},  
 year = {2023},  
 issn = {2665-9638},  
 doi = {https://doi.org/10.1016/j.simpa.2023.100556},  
 url = {https://www.sciencedirect.com/science/article/pii/S2665963823000933},  
 author = {Alessandro Berti and Sebastiaan van Zelst and Daniel Schuster},  
 }
+
```

### Comparing `pm4pyminimal-2.7.9.3/pm4py/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/analysis/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/analysis/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/analysis/extended_marking_equation/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/analysis/extended_marking_equation/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/analysis/extended_marking_equation/algorithm.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/analysis/extended_marking_equation/algorithm.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/analysis/extended_marking_equation/variants/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/analysis/extended_marking_equation/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/analysis/extended_marking_equation/variants/classic.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/analysis/extended_marking_equation/variants/classic.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/analysis/marking_equation/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/analysis/marking_equation/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/analysis/marking_equation/algorithm.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/analysis/marking_equation/algorithm.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/analysis/marking_equation/variants/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/analysis/marking_equation/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/analysis/marking_equation/variants/classic.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/analysis/marking_equation/variants/classic.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/analysis/woflan/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/analysis/woflan/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/analysis/woflan/algorithm.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/analysis/woflan/algorithm.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/analysis/woflan/graphs/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/analysis/woflan/graphs/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/analysis/woflan/graphs/minimal_coverability_graph/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/analysis/woflan/graphs/minimal_coverability_graph/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/analysis/woflan/graphs/minimal_coverability_graph/minimal_coverability_graph.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/analysis/woflan/graphs/minimal_coverability_graph/minimal_coverability_graph.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/analysis/woflan/graphs/reachability_graph/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/analysis/woflan/graphs/reachability_graph/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/analysis/woflan/graphs/reachability_graph/reachability_graph.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/analysis/woflan/graphs/reachability_graph/reachability_graph.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/analysis/woflan/graphs/restricted_coverability_graph/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/analysis/woflan/graphs/restricted_coverability_graph/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/analysis/woflan/graphs/restricted_coverability_graph/restricted_coverability_graph.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/analysis/woflan/graphs/restricted_coverability_graph/restricted_coverability_graph.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/analysis/woflan/graphs/utility.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/analysis/woflan/graphs/utility.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/analysis/woflan/not_well_handled_pairs/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/analysis/woflan/not_well_handled_pairs/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/analysis/woflan/not_well_handled_pairs/not_well_handled_pairs.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/analysis/woflan/not_well_handled_pairs/not_well_handled_pairs.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/analysis/woflan/place_invariants/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/analysis/woflan/place_invariants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/analysis/woflan/place_invariants/place_invariants.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/analysis/woflan/place_invariants/place_invariants.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/analysis/woflan/place_invariants/s_component.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/analysis/woflan/place_invariants/s_component.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/analysis/woflan/place_invariants/uniform_invariant.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/analysis/woflan/place_invariants/uniform_invariant.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/analysis/woflan/place_invariants/utility.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/analysis/woflan/place_invariants/utility.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/analysis/workflow_net/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/analysis/workflow_net/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/analysis/workflow_net/algorithm.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/analysis/workflow_net/algorithm.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/analysis/workflow_net/variants/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/analysis/workflow_net/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/analysis/workflow_net/variants/petri_net.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/analysis/workflow_net/variants/petri_net.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/anonymization/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/anonymization/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/anonymization/pripel/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/anonymization/pripel/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/anonymization/pripel/algorithm.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/anonymization/pripel/algorithm.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/anonymization/pripel/util/AttributeAnonymizer.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/anonymization/pripel/util/AttributeAnonymizer.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/anonymization/pripel/util/TraceMatcher.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/anonymization/pripel/util/TraceMatcher.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/anonymization/pripel/util/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/anonymization/pripel/util/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/anonymization/pripel/util/trace_levenshtein.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/anonymization/pripel/util/trace_levenshtein.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/anonymization/pripel/variants/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/anonymization/pripel/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/anonymization/pripel/variants/pripel.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/anonymization/pripel/variants/pripel.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/anonymization/trace_variant_query/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/anonymization/trace_variant_query/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/anonymization/trace_variant_query/algorithm.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/anonymization/trace_variant_query/algorithm.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/anonymization/trace_variant_query/util/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/anonymization/trace_variant_query/util/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/anonymization/trace_variant_query/util/behavioralAppropriateness.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/anonymization/trace_variant_query/util/behavioralAppropriateness.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/anonymization/trace_variant_query/util/exp_mech.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/anonymization/trace_variant_query/util/exp_mech.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/anonymization/trace_variant_query/util/util.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/anonymization/trace_variant_query/util/util.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/anonymization/trace_variant_query/variants/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/anonymization/trace_variant_query/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/anonymization/trace_variant_query/variants/laplace.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/anonymization/trace_variant_query/variants/laplace.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/anonymization/trace_variant_query/variants/sacofa.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/anonymization/trace_variant_query/variants/sacofa.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/clustering/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/clustering/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/clustering/profiles/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/clustering/profiles/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/clustering/profiles/algorithm.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/clustering/profiles/algorithm.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/clustering/profiles/variants/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/clustering/profiles/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/clustering/profiles/variants/sklearn_profiles.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/clustering/profiles/variants/sklearn_profiles.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/clustering/trace_attribute_driven/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/clustering/trace_attribute_driven/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/clustering/trace_attribute_driven/algorithm.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/clustering/trace_attribute_driven/algorithm.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/clustering/trace_attribute_driven/dfg/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/clustering/trace_attribute_driven/dfg/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/clustering/trace_attribute_driven/dfg/dfg_dist.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/clustering/trace_attribute_driven/dfg/dfg_dist.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/clustering/trace_attribute_driven/leven_dist/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/clustering/trace_attribute_driven/leven_dist/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/clustering/trace_attribute_driven/leven_dist/leven_dist_calc.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/clustering/trace_attribute_driven/leven_dist/leven_dist_calc.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/clustering/trace_attribute_driven/linkage_method/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/clustering/trace_attribute_driven/linkage_method/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/clustering/trace_attribute_driven/linkage_method/linkage_avg.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/clustering/trace_attribute_driven/linkage_method/linkage_avg.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/clustering/trace_attribute_driven/merge_log/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/clustering/trace_attribute_driven/merge_log/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/clustering/trace_attribute_driven/merge_log/merge_log.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/clustering/trace_attribute_driven/merge_log/merge_log.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/clustering/trace_attribute_driven/util/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/clustering/trace_attribute_driven/util/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/clustering/trace_attribute_driven/util/evaluation.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/clustering/trace_attribute_driven/util/evaluation.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/clustering/trace_attribute_driven/util/filter_subsets.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/clustering/trace_attribute_driven/util/filter_subsets.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/clustering/trace_attribute_driven/variants/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/clustering/trace_attribute_driven/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/clustering/trace_attribute_driven/variants/act_dist_calc.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/clustering/trace_attribute_driven/variants/act_dist_calc.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/clustering/trace_attribute_driven/variants/logslice_dist.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/clustering/trace_attribute_driven/variants/logslice_dist.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/clustering/trace_attribute_driven/variants/sim_calc.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/clustering/trace_attribute_driven/variants/sim_calc.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/clustering/trace_attribute_driven/variants/suc_dist_calc.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/clustering/trace_attribute_driven/variants/suc_dist_calc.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/comparison/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/comparison/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/comparison/petrinet/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/comparison/petrinet/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/comparison/petrinet/element_usage_comparison.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/comparison/petrinet/element_usage_comparison.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/conformance/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/conformance/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/conformance/alignments/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/conformance/alignments/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/conformance/alignments/decomposed/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/conformance/alignments/decomposed/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/conformance/alignments/decomposed/algorithm.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/conformance/alignments/decomposed/algorithm.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/conformance/alignments/decomposed/variants/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/conformance/alignments/decomposed/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/conformance/alignments/decomposed/variants/recompos_maximal.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/conformance/alignments/decomposed/variants/recompos_maximal.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/conformance/alignments/dfg/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/conformance/alignments/dfg/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/conformance/alignments/dfg/algorithm.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/conformance/alignments/dfg/algorithm.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/conformance/alignments/dfg/variants/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/conformance/alignments/dfg/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/conformance/alignments/dfg/variants/classic.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/conformance/alignments/dfg/variants/classic.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/conformance/alignments/edit_distance/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/conformance/alignments/edit_distance/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/conformance/alignments/edit_distance/algorithm.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/conformance/alignments/edit_distance/algorithm.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/conformance/alignments/edit_distance/variants/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/conformance/alignments/edit_distance/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/conformance/alignments/edit_distance/variants/edit_distance.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/conformance/alignments/edit_distance/variants/edit_distance.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/conformance/alignments/petri_net/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/conformance/alignments/petri_net/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/conformance/alignments/petri_net/algorithm.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/conformance/alignments/petri_net/algorithm.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/conformance/alignments/petri_net/utils/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/conformance/alignments/petri_net/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/conformance/alignments/petri_net/utils/log_enrichment.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/conformance/alignments/petri_net/utils/log_enrichment.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/conformance/alignments/petri_net/variants/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/conformance/alignments/petri_net/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/conformance/alignments/petri_net/variants/dijkstra_less_memory.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/conformance/alignments/petri_net/variants/dijkstra_less_memory.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/conformance/alignments/petri_net/variants/dijkstra_no_heuristics.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/conformance/alignments/petri_net/variants/dijkstra_no_heuristics.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/conformance/alignments/petri_net/variants/discounted_a_star.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/conformance/alignments/petri_net/variants/discounted_a_star.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/conformance/alignments/petri_net/variants/generator_dijkstra_less_memory.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/conformance/alignments/petri_net/variants/generator_dijkstra_less_memory.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/conformance/alignments/petri_net/variants/generator_dijkstra_no_heuristics.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/conformance/alignments/petri_net/variants/generator_dijkstra_no_heuristics.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/conformance/alignments/petri_net/variants/state_equation_a_star.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/conformance/alignments/petri_net/variants/state_equation_a_star.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/conformance/alignments/petri_net/variants/tweaked_state_equation_a_star.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/conformance/alignments/petri_net/variants/tweaked_state_equation_a_star.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/conformance/alignments/process_tree/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/conformance/alignments/process_tree/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/conformance/alignments/process_tree/algorithm.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/conformance/alignments/process_tree/algorithm.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/conformance/alignments/process_tree/util/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/conformance/alignments/process_tree/util/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/conformance/alignments/process_tree/util/search_graph_pt_frequency_annotation.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/conformance/alignments/process_tree/util/search_graph_pt_frequency_annotation.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/conformance/alignments/process_tree/util/search_graph_pt_replay_semantics.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/conformance/alignments/process_tree/util/search_graph_pt_replay_semantics.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/conformance/alignments/process_tree/variants/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/conformance/alignments/process_tree/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/conformance/alignments/process_tree/variants/approximated/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/conformance/alignments/process_tree/variants/approximated/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/conformance/alignments/process_tree/variants/approximated/calculate_a_sa_ea_sets.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/conformance/alignments/process_tree/variants/approximated/calculate_a_sa_ea_sets.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/conformance/alignments/process_tree/variants/approximated/matrix_lp.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/conformance/alignments/process_tree/variants/approximated/matrix_lp.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/conformance/alignments/process_tree/variants/approximated/original.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/conformance/alignments/process_tree/variants/approximated/original.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/conformance/alignments/process_tree/variants/approximated/utilities.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/conformance/alignments/process_tree/variants/approximated/utilities.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/conformance/alignments/process_tree/variants/search_graph_pt.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/conformance/alignments/process_tree/variants/search_graph_pt.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/conformance/antialignments/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/conformance/antialignments/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/conformance/antialignments/algorithm.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/conformance/antialignments/algorithm.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/conformance/antialignments/variants/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/conformance/antialignments/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/conformance/antialignments/variants/discounted_a_star.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/conformance/antialignments/variants/discounted_a_star.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/conformance/declare/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/conformance/declare/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/conformance/declare/algorithm.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/conformance/declare/algorithm.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/conformance/declare/variants/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/conformance/declare/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/conformance/declare/variants/classic.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/conformance/declare/variants/classic.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/conformance/footprints/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/conformance/footprints/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/conformance/footprints/algorithm.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/conformance/footprints/algorithm.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/conformance/footprints/util/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/conformance/footprints/util/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/conformance/footprints/util/evaluation.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/conformance/footprints/util/evaluation.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/conformance/footprints/util/tree_visualization.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/conformance/footprints/util/tree_visualization.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/conformance/footprints/variants/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/conformance/footprints/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/conformance/footprints/variants/log_extensive.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/conformance/footprints/variants/log_extensive.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/conformance/footprints/variants/log_model.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/conformance/footprints/variants/log_model.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/conformance/footprints/variants/trace_extensive.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/conformance/footprints/variants/trace_extensive.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/conformance/log_skeleton/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/conformance/log_skeleton/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/conformance/log_skeleton/algorithm.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/conformance/log_skeleton/algorithm.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/conformance/log_skeleton/variants/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/conformance/log_skeleton/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/conformance/log_skeleton/variants/classic.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/conformance/log_skeleton/variants/classic.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/conformance/multialignments/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/conformance/multialignments/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/conformance/multialignments/algorithm.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/conformance/multialignments/algorithm.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/conformance/multialignments/variants/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/conformance/multialignments/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/conformance/multialignments/variants/discounted_a_star.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/conformance/multialignments/variants/discounted_a_star.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/conformance/temporal_profile/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/conformance/temporal_profile/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/conformance/temporal_profile/algorithm.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/conformance/temporal_profile/algorithm.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/conformance/temporal_profile/variants/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/conformance/temporal_profile/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/conformance/temporal_profile/variants/dataframe.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/conformance/temporal_profile/variants/dataframe.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/conformance/temporal_profile/variants/log.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/conformance/temporal_profile/variants/log.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/conformance/tokenreplay/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/conformance/tokenreplay/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/conformance/tokenreplay/algorithm.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/conformance/tokenreplay/algorithm.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/conformance/tokenreplay/diagnostics/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/conformance/tokenreplay/diagnostics/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/conformance/tokenreplay/diagnostics/duration_diagnostics.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/conformance/tokenreplay/diagnostics/duration_diagnostics.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/conformance/tokenreplay/diagnostics/root_cause_analysis.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/conformance/tokenreplay/diagnostics/root_cause_analysis.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/conformance/tokenreplay/variants/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/conformance/tokenreplay/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/conformance/tokenreplay/variants/backwards.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/conformance/tokenreplay/variants/backwards.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/conformance/tokenreplay/variants/token_replay.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/conformance/tokenreplay/variants/token_replay.py`

 * *Files 6% similar despite different names*

```diff
@@ -908,14 +908,50 @@
     if disable_variants:
         return str(hash(trace))
     parameters = {}
     parameters[variants_util.Parameters.ACTIVITY_KEY] = activity_key
     return variants_util.get_variant_from_trace(trace, parameters=parameters)
 
 
+def transcribe_result(t, return_object_names=True):
+    corr_value = {"trace_is_fit": copy(t.t_fit),
+                  "trace_fitness": float(copy(t.t_value)),
+                  "activated_transitions": copy(t.act_trans),
+                  "reached_marking": copy(t.reached_marking),
+                  "enabled_transitions_in_marking": copy(
+                      t.enabled_trans_in_mark),
+                  "transitions_with_problems": copy(
+                      t.trans_probl),
+                  "missing_tokens": int(t.missing),
+                  "consumed_tokens": int(t.consumed),
+                  "remaining_tokens": int(t.remaining),
+                  "produced_tokens": int(t.produced)}
+
+    if return_object_names:
+        corr_value["activated_transitions_labels"] = [x.label for x in
+                                                      corr_value[
+                                                          "activated_transitions"]]
+        corr_value["activated_transitions"] = [x.name for x in corr_value[
+            "activated_transitions"]]
+        corr_value["enabled_transitions_in_marking_labels"] = [x.label for x in
+                                                               corr_value[
+                                                                   "enabled_transitions_in_marking"]]
+        corr_value["enabled_transitions_in_marking"] = [x.name for x in
+                                                        corr_value[
+                                                            "enabled_transitions_in_marking"]]
+        corr_value["transitions_with_problems"] = [x.name for x in
+                                                   corr_value[
+                                                       "transitions_with_problems"]]
+        corr_value["reached_marking"] = {x.name: y for x, y in
+                                         corr_value[
+                                             "reached_marking"].items()}
+
+    return corr_value
+
+
 def apply_log(log, net, initial_marking, final_marking, enable_pltr_fitness=False, consider_remaining_in_fitness=False,
               activity_key="concept:name", reach_mark_through_hidden=True, stop_immediately_unfit=False,
               walk_through_hidden_trans=True, places_shortest_path_by_hidden=None,
               is_reduction=False, thread_maximum_ex_time=TechnicalParameters.MAX_DEF_THR_EX_TIME.value,
               cleaning_token_flood=False, disable_variants=False, return_object_names=False, show_progress_bar=True,
               consider_activities_not_in_model_in_fitness=False, case_id_key=constants.CASE_CONCEPT_NAME):
     """
@@ -983,94 +1019,102 @@
     notexisting_activities_in_model = {}
 
     trans_map = {}
     for t in net.transitions:
         trans_map[t.label] = t
 
     if pandas_utils.check_is_pandas_dataframe(log):
-        traces = [tuple(x) for x in log.groupby(case_id_key)[activity_key].agg(list).to_dict().values()]
+        traces = [(tuple(x), y) for y, x in log.groupby(case_id_key)[activity_key].agg(list).to_dict().items()]
+        traces = [(traces[i][0], i) for i in range(len(traces))]
     else:
-        traces = [tuple(x[activity_key] for x in trace) for trace in log]
+        traces = [(tuple(x[activity_key] for x in log[i]), i) for i in range(len(log))]
 
-    variants = Counter(traces)
+    variants = dict()
+    for t in traces:
+        if t[0] not in variants:
+            variants[t[0]] = list()
+        variants[t[0]].append(t[1])
+
+    traces = [t[0] for t in traces]
 
     vc = [(k, v) for k, v in variants.items()]
-    vc = list(sorted(vc, key=lambda x: (x[1], x[0]), reverse=True))
+    vc = list(sorted(vc, key=lambda x: (len(x[1]), x[0]), reverse=True))
+
+    threads_results = {}
 
     progress = None
+
     if importlib.util.find_spec("tqdm") and show_progress_bar and len(variants) > 1:
         from tqdm.auto import tqdm
-        progress = tqdm(total=len(variants), desc="replaying log with TBR, completed variants :: ")
 
-    threads = {}
-    threads_results = {}
+        if disable_variants and not pandas_utils.check_is_pandas_dataframe(log):
+            progress = tqdm(total=len(traces), desc="replaying log with TBR, completed traces :: ")
+        else:
+            progress = tqdm(total=len(variants), desc="replaying log with TBR, completed traces :: ")
 
     for i in range(len(vc)):
         variant = vc[i][0]
-        considered_case = variants_util.variant_to_trace(variant, parameters={constants.PARAMETER_CONSTANT_ACTIVITY_KEY: activity_key})
+        all_cases = vc[i][1]
+
+        if disable_variants and not pandas_utils.check_is_pandas_dataframe(log):
+            for j in range(len(all_cases)):
+                case_position = all_cases[j]
+                considered_case = log[case_position]
+                t = ApplyTraceTokenReplay(considered_case, net, initial_marking, final_marking,
+                                          trans_map, enable_pltr_fitness, place_fitness_per_trace,
+                                          transition_fitness_per_trace,
+                                          notexisting_activities_in_model,
+                                          places_shortest_path_by_hidden,
+                                          consider_remaining_in_fitness,
+                                          activity_key=activity_key,
+                                          reach_mark_through_hidden=reach_mark_through_hidden,
+                                          stop_immediately_when_unfit=stop_immediately_unfit,
+                                          walk_through_hidden_trans=walk_through_hidden_trans,
+                                          post_fix_caching=post_fix_cache,
+                                          marking_to_activity_caching=marking_to_activity_cache,
+                                          is_reduction=is_reduction,
+                                          thread_maximum_ex_time=thread_maximum_ex_time,
+                                          cleaning_token_flood=cleaning_token_flood,
+                                          s_components=s_components, trace_occurrences=1,
+                                          consider_activities_not_in_model_in_fitness=consider_activities_not_in_model_in_fitness)
+                t.run()
+                threads_results[case_position] = transcribe_result(t, return_object_names=return_object_names)
+                if progress is not None:
+                    progress.update()
+        else:
+            considered_case = variants_util.variant_to_trace(variant, parameters={constants.PARAMETER_CONSTANT_ACTIVITY_KEY: activity_key})
+            t = ApplyTraceTokenReplay(considered_case, net, initial_marking, final_marking,
+                                                     trans_map, enable_pltr_fitness, place_fitness_per_trace,
+                                                     transition_fitness_per_trace,
+                                                     notexisting_activities_in_model,
+                                                     places_shortest_path_by_hidden,
+                                                     consider_remaining_in_fitness,
+                                                     activity_key=activity_key,
+                                                     reach_mark_through_hidden=reach_mark_through_hidden,
+                                                     stop_immediately_when_unfit=stop_immediately_unfit,
+                                                     walk_through_hidden_trans=walk_through_hidden_trans,
+                                                     post_fix_caching=post_fix_cache,
+                                                     marking_to_activity_caching=marking_to_activity_cache,
+                                                     is_reduction=is_reduction,
+                                                     thread_maximum_ex_time=thread_maximum_ex_time,
+                                                     cleaning_token_flood=cleaning_token_flood,
+                                                     s_components=s_components, trace_occurrences=len(vc[i][1]),
+                                                     consider_activities_not_in_model_in_fitness=consider_activities_not_in_model_in_fitness)
+            t.run()
+
+            for j in range(len(all_cases)):
+                case_position = all_cases[j]
+
+                threads_results[case_position] = transcribe_result(t, return_object_names=return_object_names)
+
+            if progress is not None:
+                progress.update()
 
-        threads[variant] = ApplyTraceTokenReplay(considered_case, net, initial_marking, final_marking,
-                                                 trans_map, enable_pltr_fitness, place_fitness_per_trace,
-                                                 transition_fitness_per_trace,
-                                                 notexisting_activities_in_model,
-                                                 places_shortest_path_by_hidden,
-                                                 consider_remaining_in_fitness,
-                                                 activity_key=activity_key,
-                                                 reach_mark_through_hidden=reach_mark_through_hidden,
-                                                 stop_immediately_when_unfit=stop_immediately_unfit,
-                                                 walk_through_hidden_trans=walk_through_hidden_trans,
-                                                 post_fix_caching=post_fix_cache,
-                                                 marking_to_activity_caching=marking_to_activity_cache,
-                                                 is_reduction=is_reduction,
-                                                 thread_maximum_ex_time=thread_maximum_ex_time,
-                                                 cleaning_token_flood=cleaning_token_flood,
-                                                 s_components=s_components, trace_occurrences=vc[i][1],
-                                                 consider_activities_not_in_model_in_fitness=consider_activities_not_in_model_in_fitness)
-        threads[variant].run()
-        if progress is not None:
-            progress.update()
-
-        t = threads[variant]
-        threads_results[variant] = {"trace_is_fit": copy(t.t_fit),
-                                    "trace_fitness": float(copy(t.t_value)),
-                                    "activated_transitions": copy(t.act_trans),
-                                    "reached_marking": copy(t.reached_marking),
-                                    "enabled_transitions_in_marking": copy(
-                                        t.enabled_trans_in_mark),
-                                    "transitions_with_problems": copy(
-                                        t.trans_probl),
-                                    "missing_tokens": int(t.missing),
-                                    "consumed_tokens": int(t.consumed),
-                                    "remaining_tokens": int(t.remaining),
-                                    "produced_tokens": int(t.produced)}
-
-        if return_object_names:
-            threads_results[variant]["activated_transitions_labels"] = [x.label for x in
-                                                                        threads_results[variant][
-                                                                            "activated_transitions"]]
-            threads_results[variant]["activated_transitions"] = [x.name for x in threads_results[variant][
-                "activated_transitions"]]
-            threads_results[variant]["enabled_transitions_in_marking_labels"] = [x.label for x in
-                                                                                 threads_results[variant][
-                                                                                     "enabled_transitions_in_marking"]]
-            threads_results[variant]["enabled_transitions_in_marking"] = [x.name for x in
-                                                                          threads_results[variant][
-                                                                              "enabled_transitions_in_marking"]]
-            threads_results[variant]["transitions_with_problems"] = [x.name for x in
-                                                                     threads_results[variant][
-                                                                         "transitions_with_problems"]]
-            threads_results[variant]["reached_marking"] = {x.name: y for x, y in
-                                                           threads_results[variant][
-                                                               "reached_marking"].items()}
-        del threads[variant]
-
-    for trace_variant in traces:
-        if trace_variant in threads_results:
-            t = threads_results[trace_variant]
-            aligned_traces.append(t)
+    for i in range(len(traces)):
+        aligned_traces.append(threads_results[i])
 
     # gracefully close progress bar
     if progress is not None:
         progress.close()
     del progress
 
     if enable_pltr_fitness:
```

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/connectors/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/connectors/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/connectors/algorithm.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/connectors/algorithm.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/connectors/util/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/connectors/util/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/connectors/util/mail.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/connectors/util/mail.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/connectors/variants/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/connectors/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/connectors/variants/camunda_workflow.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/connectors/variants/camunda_workflow.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/connectors/variants/chrome_history.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/connectors/variants/chrome_history.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/connectors/variants/firefox_history.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/connectors/variants/firefox_history.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/connectors/variants/github_repo.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/connectors/variants/github_repo.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/connectors/variants/outlook_calendar.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/connectors/variants/outlook_calendar.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/connectors/variants/outlook_mail_extractor.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/connectors/variants/outlook_mail_extractor.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/connectors/variants/sap_accounting.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/connectors/variants/sap_accounting.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/connectors/variants/sap_o2c.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/connectors/variants/sap_o2c.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/connectors/variants/windows_events.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/connectors/variants/windows_events.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/decision_mining/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/decision_mining/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/decision_mining/algorithm.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/decision_mining/algorithm.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/discovery/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/discovery/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/discovery/alpha/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/discovery/alpha/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/discovery/alpha/algorithm.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/discovery/alpha/algorithm.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/discovery/alpha/data_structures/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/discovery/alpha/data_structures/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/discovery/alpha/data_structures/alpha_classic_abstraction.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/discovery/alpha/data_structures/alpha_classic_abstraction.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/discovery/alpha/utils/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/discovery/alpha/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/discovery/alpha/utils/endpoints.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/discovery/alpha/utils/endpoints.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/discovery/alpha/variants/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/discovery/alpha/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/discovery/alpha/variants/classic.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/discovery/alpha/variants/classic.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/discovery/alpha/variants/plus.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/discovery/alpha/variants/plus.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/discovery/batches/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/discovery/batches/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/discovery/batches/algorithm.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/discovery/batches/algorithm.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/discovery/batches/utils/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/discovery/batches/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/discovery/batches/utils/detection.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/discovery/batches/utils/detection.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/discovery/batches/variants/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/discovery/batches/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/discovery/batches/variants/log.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/discovery/batches/variants/log.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/discovery/batches/variants/pandas.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/discovery/batches/variants/pandas.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/discovery/causal/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/discovery/causal/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/discovery/causal/algorithm.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/discovery/causal/algorithm.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/discovery/causal/variants/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/discovery/causal/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/discovery/causal/variants/alpha.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/discovery/causal/variants/alpha.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/discovery/causal/variants/heuristic.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/discovery/causal/variants/heuristic.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/discovery/correlation_mining/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/discovery/correlation_mining/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/discovery/correlation_mining/algorithm.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/discovery/correlation_mining/algorithm.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/discovery/correlation_mining/util.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/discovery/correlation_mining/util.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/discovery/correlation_mining/variants/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/discovery/correlation_mining/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/discovery/correlation_mining/variants/classic.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/discovery/correlation_mining/variants/classic.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/discovery/correlation_mining/variants/classic_split.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/discovery/correlation_mining/variants/classic_split.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/discovery/correlation_mining/variants/trace_based.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/discovery/correlation_mining/variants/trace_based.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/discovery/declare/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/discovery/declare/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/discovery/declare/algorithm.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/discovery/declare/algorithm.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/discovery/declare/templates.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/discovery/declare/templates.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/discovery/declare/variants/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/discovery/declare/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/discovery/declare/variants/classic.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/discovery/declare/variants/classic.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/discovery/dfg/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/discovery/dfg/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/discovery/dfg/adapters/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/discovery/dfg/adapters/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/discovery/dfg/adapters/pandas/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/discovery/dfg/adapters/pandas/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/discovery/dfg/adapters/pandas/df_statistics.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/discovery/dfg/adapters/pandas/df_statistics.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/discovery/dfg/adapters/pandas/freq_triples.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/discovery/dfg/adapters/pandas/freq_triples.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/discovery/dfg/algorithm.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/discovery/dfg/algorithm.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/discovery/dfg/replacement.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/discovery/dfg/replacement.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/discovery/dfg/utils/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/discovery/dfg/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/discovery/dfg/utils/dfg_utils.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/discovery/dfg/utils/dfg_utils.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/discovery/dfg/variants/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/discovery/dfg/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/discovery/dfg/variants/case_attributes.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/discovery/dfg/variants/case_attributes.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/discovery/dfg/variants/clean.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/discovery/dfg/variants/clean.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/discovery/dfg/variants/clean_polars.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/discovery/dfg/variants/clean_polars.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/discovery/dfg/variants/clean_time.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/discovery/dfg/variants/clean_time.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/discovery/dfg/variants/freq_triples.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/discovery/dfg/variants/freq_triples.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/discovery/dfg/variants/native.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/discovery/dfg/variants/native.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/discovery/dfg/variants/performance.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/discovery/dfg/variants/performance.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/discovery/footprints/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/discovery/footprints/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/discovery/footprints/algorithm.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/discovery/footprints/algorithm.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/discovery/footprints/dfg/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/discovery/footprints/dfg/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/discovery/footprints/dfg/variants/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/discovery/footprints/dfg/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/discovery/footprints/dfg/variants/dfg.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/discovery/footprints/dfg/variants/dfg.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/discovery/footprints/log/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/discovery/footprints/log/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/discovery/footprints/log/variants/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/discovery/footprints/log/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/discovery/footprints/log/variants/entire_dataframe.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/discovery/footprints/log/variants/entire_dataframe.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/discovery/footprints/log/variants/entire_event_log.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/discovery/footprints/log/variants/entire_event_log.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/discovery/footprints/log/variants/trace_by_trace.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/discovery/footprints/log/variants/trace_by_trace.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/discovery/footprints/petri/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/discovery/footprints/petri/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/discovery/footprints/petri/variants/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/discovery/footprints/petri/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/discovery/footprints/petri/variants/reach_graph.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/discovery/footprints/petri/variants/reach_graph.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/discovery/footprints/tree/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/discovery/footprints/tree/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/discovery/footprints/tree/variants/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/discovery/footprints/tree/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/discovery/footprints/tree/variants/bottomup.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/discovery/footprints/tree/variants/bottomup.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/discovery/heuristics/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/discovery/heuristics/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/discovery/heuristics/algorithm.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/discovery/heuristics/algorithm.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/discovery/heuristics/variants/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/discovery/heuristics/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/discovery/heuristics/variants/classic.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/discovery/heuristics/variants/classic.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/discovery/heuristics/variants/plusplus.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/discovery/heuristics/variants/plusplus.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/discovery/ilp/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/discovery/ilp/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/discovery/ilp/algorithm.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/discovery/ilp/algorithm.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/discovery/ilp/variants/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/discovery/ilp/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/discovery/ilp/variants/classic.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/discovery/ilp/variants/classic.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/discovery/inductive/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/discovery/inductive/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/discovery/inductive/algorithm.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/discovery/inductive/algorithm.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/discovery/inductive/base_case/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/discovery/inductive/base_case/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/discovery/inductive/base_case/abc.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/discovery/inductive/base_case/abc.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/discovery/inductive/base_case/empty_log.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/discovery/inductive/base_case/empty_log.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/discovery/inductive/base_case/factory.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/discovery/inductive/base_case/factory.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/discovery/inductive/base_case/single_activity.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/discovery/inductive/base_case/single_activity.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/discovery/inductive/cuts/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/discovery/inductive/cuts/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/discovery/inductive/cuts/abc.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/discovery/inductive/cuts/abc.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/discovery/inductive/cuts/concurrency.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/discovery/inductive/cuts/concurrency.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/discovery/inductive/cuts/factory.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/discovery/inductive/cuts/factory.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/discovery/inductive/cuts/loop.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/discovery/inductive/cuts/loop.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/discovery/inductive/cuts/sequence.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/discovery/inductive/cuts/sequence.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/discovery/inductive/cuts/utils.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/discovery/inductive/cuts/utils.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/discovery/inductive/cuts/xor.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/discovery/inductive/cuts/xor.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/discovery/inductive/dtypes/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/discovery/inductive/dtypes/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/discovery/inductive/dtypes/im_dfg.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/discovery/inductive/dtypes/im_dfg.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/discovery/inductive/dtypes/im_ds.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/discovery/inductive/dtypes/im_ds.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/discovery/inductive/fall_through/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/discovery/inductive/fall_through/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/discovery/inductive/fall_through/abc.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/discovery/inductive/fall_through/abc.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/discovery/inductive/fall_through/activity_concurrent.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/discovery/inductive/fall_through/activity_concurrent.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/discovery/inductive/fall_through/activity_once_per_trace.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/discovery/inductive/fall_through/activity_once_per_trace.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/discovery/inductive/fall_through/empty_traces.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/discovery/inductive/fall_through/empty_traces.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/discovery/inductive/fall_through/factory.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/discovery/inductive/fall_through/factory.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/discovery/inductive/fall_through/flower.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/discovery/inductive/fall_through/flower.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/discovery/inductive/fall_through/strict_tau_loop.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/discovery/inductive/fall_through/strict_tau_loop.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/discovery/inductive/fall_through/tau_loop.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/discovery/inductive/fall_through/tau_loop.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/discovery/inductive/variants/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/discovery/inductive/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/discovery/inductive/variants/abc.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/discovery/inductive/variants/abc.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/discovery/inductive/variants/im.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/discovery/inductive/variants/im.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/discovery/inductive/variants/imd.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/discovery/inductive/variants/imd.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/discovery/inductive/variants/imf.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/discovery/inductive/variants/imf.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/discovery/inductive/variants/instances.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/discovery/inductive/variants/instances.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/discovery/log_skeleton/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/discovery/log_skeleton/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/discovery/log_skeleton/algorithm.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/discovery/log_skeleton/algorithm.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/discovery/log_skeleton/trace_skel.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/discovery/log_skeleton/trace_skel.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/discovery/log_skeleton/variants/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/discovery/log_skeleton/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/discovery/log_skeleton/variants/classic.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/discovery/log_skeleton/variants/classic.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/discovery/minimum_self_distance/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/discovery/minimum_self_distance/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/discovery/minimum_self_distance/algorithm.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/discovery/minimum_self_distance/algorithm.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/discovery/minimum_self_distance/utils.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/discovery/minimum_self_distance/utils.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/discovery/minimum_self_distance/variants/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/discovery/minimum_self_distance/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/discovery/minimum_self_distance/variants/log.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/discovery/minimum_self_distance/variants/log.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/discovery/minimum_self_distance/variants/pandas.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/discovery/minimum_self_distance/variants/pandas.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/discovery/ocel/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/discovery/ocel/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/discovery/ocel/interleavings/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/discovery/ocel/interleavings/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/discovery/ocel/interleavings/algorithm.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/discovery/ocel/interleavings/algorithm.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/discovery/ocel/interleavings/utils/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/discovery/ocel/interleavings/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/discovery/ocel/interleavings/utils/merge_dataframe_rel_cases.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/discovery/ocel/interleavings/utils/merge_dataframe_rel_cases.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/discovery/ocel/interleavings/variants/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/discovery/ocel/interleavings/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/discovery/ocel/interleavings/variants/timestamp_interleavings.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/discovery/ocel/interleavings/variants/timestamp_interleavings.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/discovery/ocel/link_analysis/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/discovery/ocel/link_analysis/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/discovery/ocel/link_analysis/algorithm.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/discovery/ocel/link_analysis/algorithm.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/discovery/ocel/link_analysis/variants/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/discovery/ocel/link_analysis/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/discovery/ocel/link_analysis/variants/classic.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/discovery/ocel/link_analysis/variants/classic.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/discovery/ocel/ocdfg/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/discovery/ocel/ocdfg/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/discovery/ocel/ocdfg/algorithm.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/discovery/ocel/ocdfg/algorithm.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/discovery/ocel/ocdfg/variants/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/discovery/ocel/ocdfg/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/discovery/ocel/ocdfg/variants/classic.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/discovery/ocel/ocdfg/variants/classic.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/discovery/ocel/ocpn/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/discovery/ocel/ocpn/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/discovery/ocel/ocpn/algorithm.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/discovery/ocel/ocpn/algorithm.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/discovery/ocel/ocpn/variants/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/discovery/ocel/ocpn/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/discovery/ocel/ocpn/variants/classic.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/discovery/ocel/ocpn/variants/classic.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/discovery/ocel/ocpn/variants/wo_annotation.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/discovery/ocel/ocpn/variants/wo_annotation.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/discovery/ocel/saw_nets/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/discovery/ocel/saw_nets/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/discovery/ocel/saw_nets/algorithm.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/discovery/ocel/saw_nets/algorithm.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/discovery/ocel/saw_nets/variants/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/discovery/ocel/saw_nets/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/discovery/ocel/saw_nets/variants/classic.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/discovery/ocel/saw_nets/variants/classic.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/discovery/performance_spectrum/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/discovery/performance_spectrum/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/discovery/performance_spectrum/algorithm.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/discovery/performance_spectrum/algorithm.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/discovery/performance_spectrum/variants/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/discovery/performance_spectrum/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/discovery/performance_spectrum/variants/dataframe.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/discovery/performance_spectrum/variants/dataframe.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/discovery/performance_spectrum/variants/dataframe_disconnected.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/discovery/performance_spectrum/variants/dataframe_disconnected.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/discovery/performance_spectrum/variants/log.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/discovery/performance_spectrum/variants/log.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/discovery/performance_spectrum/variants/log_disconnected.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/discovery/performance_spectrum/variants/log_disconnected.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/discovery/powl/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/discovery/powl/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/discovery/powl/algorithm.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/discovery/powl/algorithm.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/discovery/powl/inductive/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/discovery/powl/inductive/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/discovery/powl/inductive/base_case/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/discovery/powl/inductive/base_case/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/discovery/powl/inductive/base_case/abc.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/discovery/powl/inductive/base_case/abc.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/discovery/powl/inductive/base_case/empty_log.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/discovery/powl/inductive/base_case/empty_log.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/discovery/powl/inductive/base_case/factory.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/discovery/powl/inductive/base_case/factory.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/discovery/powl/inductive/base_case/single_activity.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/discovery/powl/inductive/base_case/single_activity.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/discovery/powl/inductive/cuts/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/discovery/powl/inductive/cuts/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/discovery/powl/inductive/cuts/concurrency.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/discovery/powl/inductive/cuts/concurrency.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/discovery/powl/inductive/cuts/factory.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/discovery/powl/inductive/cuts/factory.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/discovery/powl/inductive/cuts/loop.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/discovery/powl/inductive/cuts/loop.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/discovery/powl/inductive/cuts/sequence.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/discovery/powl/inductive/cuts/sequence.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/discovery/powl/inductive/cuts/xor.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/discovery/powl/inductive/cuts/xor.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/discovery/powl/inductive/fall_through/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/discovery/powl/inductive/fall_through/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/discovery/powl/inductive/fall_through/activity_concurrent.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/discovery/powl/inductive/fall_through/activity_concurrent.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/discovery/powl/inductive/fall_through/activity_once_per_trace.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/discovery/powl/inductive/fall_through/activity_once_per_trace.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/discovery/powl/inductive/fall_through/empty_traces.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/discovery/powl/inductive/fall_through/empty_traces.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/discovery/powl/inductive/fall_through/factory.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/discovery/powl/inductive/fall_through/factory.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/discovery/powl/inductive/fall_through/flower.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/discovery/powl/inductive/fall_through/flower.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/discovery/powl/inductive/fall_through/strict_tau_loop.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/discovery/powl/inductive/fall_through/strict_tau_loop.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/discovery/powl/inductive/fall_through/tau_loop.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/discovery/powl/inductive/fall_through/tau_loop.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/discovery/powl/inductive/utils/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/discovery/powl/inductive/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/discovery/powl/inductive/utils/filtering.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/discovery/powl/inductive/utils/filtering.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/discovery/powl/inductive/variants/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/discovery/powl/inductive/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/discovery/powl/inductive/variants/brute_force/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/discovery/powl/inductive/variants/brute_force/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/discovery/powl/inductive/variants/brute_force/bf_partial_order_cut.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/discovery/powl/inductive/variants/brute_force/bf_partial_order_cut.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/discovery/powl/inductive/variants/brute_force/factory.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/discovery/powl/inductive/variants/brute_force/factory.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/discovery/powl/inductive/variants/dynamic_clustering/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/discovery/powl/inductive/variants/dynamic_clustering/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/discovery/powl/inductive/variants/dynamic_clustering/dynamic_clustering_partial_order_cut.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/discovery/powl/inductive/variants/dynamic_clustering/dynamic_clustering_partial_order_cut.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/discovery/powl/inductive/variants/dynamic_clustering/factory.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/discovery/powl/inductive/variants/dynamic_clustering/factory.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/discovery/powl/inductive/variants/dynamic_clustering_frequency/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/discovery/powl/inductive/variants/dynamic_clustering_frequency/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/discovery/powl/inductive/variants/dynamic_clustering_frequency/dynamic_clustering_frequency_partial_order_cut.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/discovery/powl/inductive/variants/dynamic_clustering_frequency/dynamic_clustering_frequency_partial_order_cut.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/discovery/powl/inductive/variants/dynamic_clustering_frequency/factory.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/discovery/powl/inductive/variants/dynamic_clustering_frequency/factory.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/discovery/powl/inductive/variants/im_brute_force.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/discovery/powl/inductive/variants/im_brute_force.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/discovery/powl/inductive/variants/im_dynamic_clustering.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/discovery/powl/inductive/variants/im_dynamic_clustering.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/discovery/powl/inductive/variants/im_dynamic_clustering_frequencies.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/discovery/powl/inductive/variants/im_dynamic_clustering_frequencies.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/discovery/powl/inductive/variants/im_maximal.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/discovery/powl/inductive/variants/im_maximal.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/discovery/powl/inductive/variants/im_tree.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/discovery/powl/inductive/variants/im_tree.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/discovery/powl/inductive/variants/maximal/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/discovery/powl/inductive/variants/maximal/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/discovery/powl/inductive/variants/maximal/factory.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/discovery/powl/inductive/variants/maximal/factory.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/discovery/powl/inductive/variants/maximal/maximal_partial_order_cut.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/discovery/powl/inductive/variants/maximal/maximal_partial_order_cut.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/discovery/powl/inductive/variants/powl_discovery_varaints.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/discovery/powl/inductive/variants/powl_discovery_varaints.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/discovery/temporal_profile/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/discovery/temporal_profile/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/discovery/temporal_profile/algorithm.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/discovery/temporal_profile/algorithm.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/discovery/temporal_profile/variants/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/discovery/temporal_profile/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/discovery/temporal_profile/variants/dataframe.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/discovery/temporal_profile/variants/dataframe.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/discovery/temporal_profile/variants/log.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/discovery/temporal_profile/variants/log.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/discovery/transition_system/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/discovery/transition_system/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/discovery/transition_system/algorithm.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/discovery/transition_system/algorithm.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/discovery/transition_system/variants/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/discovery/transition_system/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/discovery/transition_system/variants/view_based.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/discovery/transition_system/variants/view_based.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/evaluation/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/evaluation/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/evaluation/algorithm.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/evaluation/algorithm.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/evaluation/earth_mover_distance/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/evaluation/earth_mover_distance/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/evaluation/earth_mover_distance/algorithm.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/evaluation/earth_mover_distance/algorithm.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/evaluation/earth_mover_distance/variants/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/evaluation/earth_mover_distance/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/evaluation/earth_mover_distance/variants/pyemd.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/evaluation/earth_mover_distance/variants/pyemd.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/evaluation/generalization/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/evaluation/generalization/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/evaluation/generalization/algorithm.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/evaluation/generalization/algorithm.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/evaluation/generalization/variants/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/evaluation/generalization/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/evaluation/generalization/variants/token_based.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/evaluation/generalization/variants/token_based.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/evaluation/precision/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/evaluation/precision/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/evaluation/precision/algorithm.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/evaluation/precision/algorithm.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/evaluation/precision/dfg/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/evaluation/precision/dfg/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/evaluation/precision/dfg/algorithm.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/evaluation/precision/dfg/algorithm.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/evaluation/precision/utils.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/evaluation/precision/utils.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/evaluation/precision/variants/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/evaluation/precision/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/evaluation/precision/variants/align_etconformance.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/evaluation/precision/variants/align_etconformance.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/evaluation/precision/variants/etconformance_token.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/evaluation/precision/variants/etconformance_token.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/evaluation/replay_fitness/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/evaluation/replay_fitness/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/evaluation/replay_fitness/algorithm.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/evaluation/replay_fitness/algorithm.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/evaluation/replay_fitness/variants/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/evaluation/replay_fitness/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/evaluation/replay_fitness/variants/alignment_based.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/evaluation/replay_fitness/variants/alignment_based.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/evaluation/replay_fitness/variants/token_replay.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/evaluation/replay_fitness/variants/token_replay.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/evaluation/simplicity/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/evaluation/simplicity/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/evaluation/simplicity/algorithm.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/evaluation/simplicity/algorithm.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/evaluation/simplicity/variants/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/evaluation/simplicity/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/evaluation/simplicity/variants/arc_degree.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/evaluation/simplicity/variants/arc_degree.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/evaluation/simplicity/variants/extended_cardoso.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/evaluation/simplicity/variants/extended_cardoso.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/evaluation/simplicity/variants/extended_cyclomatic.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/evaluation/simplicity/variants/extended_cyclomatic.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/filtering/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/filtering/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/filtering/common/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/filtering/common/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/filtering/common/attributes/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/filtering/common/attributes/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/filtering/common/attributes/attributes_common.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/filtering/common/attributes/attributes_common.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/filtering/common/end_activities/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/filtering/common/end_activities/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/filtering/common/end_activities/end_activities_common.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/filtering/common/end_activities/end_activities_common.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/filtering/common/filtering_constants.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/filtering/common/filtering_constants.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/filtering/common/start_activities/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/filtering/common/start_activities/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/filtering/common/start_activities/start_activities_common.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/filtering/common/start_activities/start_activities_common.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/filtering/common/timestamp/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/filtering/common/timestamp/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/filtering/common/timestamp/timestamp_common.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/filtering/common/timestamp/timestamp_common.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/filtering/common/traces/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/filtering/common/traces/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/filtering/common/traces/infix_to_regex.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/filtering/common/traces/infix_to_regex.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/filtering/dfg/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/filtering/dfg/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/filtering/dfg/dfg_filtering.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/filtering/dfg/dfg_filtering.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/filtering/log/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/filtering/log/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/filtering/log/attr_value_repetition/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/filtering/log/attr_value_repetition/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/filtering/log/attr_value_repetition/filter.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/filtering/log/attr_value_repetition/filter.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/filtering/log/attributes/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/filtering/log/attributes/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/filtering/log/attributes/attributes_filter.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/filtering/log/attributes/attributes_filter.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/filtering/log/between/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/filtering/log/between/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/filtering/log/between/between_filter.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/filtering/log/between/between_filter.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/filtering/log/cases/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/filtering/log/cases/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/filtering/log/cases/case_filter.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/filtering/log/cases/case_filter.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/filtering/log/end_activities/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/filtering/log/end_activities/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/filtering/log/end_activities/end_activities_filter.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/filtering/log/end_activities/end_activities_filter.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/filtering/log/ltl/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/filtering/log/ltl/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/filtering/log/ltl/ltl_checker.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/filtering/log/ltl/ltl_checker.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/filtering/log/paths/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/filtering/log/paths/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/filtering/log/paths/paths_filter.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/filtering/log/paths/paths_filter.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/filtering/log/prefixes/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/filtering/log/prefixes/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/filtering/log/prefixes/prefix_filter.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/filtering/log/prefixes/prefix_filter.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/filtering/log/rework/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/filtering/log/rework/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/filtering/log/rework/rework_filter.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/filtering/log/rework/rework_filter.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/filtering/log/start_activities/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/filtering/log/start_activities/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/filtering/log/start_activities/start_activities_filter.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/filtering/log/start_activities/start_activities_filter.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/filtering/log/suffixes/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/filtering/log/suffixes/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/filtering/log/suffixes/suffix_filter.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/filtering/log/suffixes/suffix_filter.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/filtering/log/timestamp/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/filtering/log/timestamp/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/filtering/log/timestamp/timestamp_filter.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/filtering/log/timestamp/timestamp_filter.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/filtering/log/traces/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/filtering/log/traces/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/filtering/log/traces/trace_filter.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/filtering/log/traces/trace_filter.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/filtering/log/variants/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/filtering/log/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/filtering/log/variants/variants_filter.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/filtering/log/variants/variants_filter.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/filtering/ocel/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/filtering/ocel/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/filtering/ocel/activity_type_matching.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/filtering/ocel/activity_type_matching.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/filtering/ocel/event_attributes.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/filtering/ocel/event_attributes.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/filtering/ocel/object_attributes.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/filtering/ocel/object_attributes.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/filtering/ocel/objects_ot_count.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/filtering/ocel/objects_ot_count.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/filtering/ocel/ot_endpoints.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/filtering/ocel/ot_endpoints.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/filtering/pandas/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/filtering/pandas/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/filtering/pandas/attr_value_repetition/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/filtering/pandas/attr_value_repetition/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/filtering/pandas/attr_value_repetition/filter.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/filtering/pandas/attr_value_repetition/filter.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/filtering/pandas/attributes/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/filtering/pandas/attributes/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/filtering/pandas/attributes/attributes_filter.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/filtering/pandas/attributes/attributes_filter.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/filtering/pandas/between/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/filtering/pandas/between/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/filtering/pandas/between/between_filter.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/filtering/pandas/between/between_filter.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/filtering/pandas/cases/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/filtering/pandas/cases/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/filtering/pandas/cases/case_filter.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/filtering/pandas/cases/case_filter.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/filtering/pandas/consecutive_act_case_grouping/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/filtering/pandas/consecutive_act_case_grouping/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/filtering/pandas/consecutive_act_case_grouping/consecutive_act_case_grouping_filter.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/filtering/pandas/consecutive_act_case_grouping/consecutive_act_case_grouping_filter.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/filtering/pandas/end_activities/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/filtering/pandas/end_activities/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/filtering/pandas/end_activities/end_activities_filter.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/filtering/pandas/end_activities/end_activities_filter.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/filtering/pandas/ends_with/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/filtering/pandas/ends_with/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/filtering/pandas/ends_with/ends_with_filter.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/filtering/pandas/ends_with/ends_with_filter.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/filtering/pandas/ltl/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/filtering/pandas/ltl/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/filtering/pandas/ltl/ltl_checker.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/filtering/pandas/ltl/ltl_checker.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/filtering/pandas/paths/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/filtering/pandas/paths/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/filtering/pandas/paths/paths_filter.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/filtering/pandas/paths/paths_filter.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/filtering/pandas/pd_filtering_constants.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/filtering/pandas/pd_filtering_constants.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/filtering/pandas/prefixes/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/filtering/pandas/prefixes/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/filtering/pandas/prefixes/prefix_filter.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/filtering/pandas/prefixes/prefix_filter.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/filtering/pandas/rework/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/filtering/pandas/rework/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/filtering/pandas/rework/rework_filter.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/filtering/pandas/rework/rework_filter.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/filtering/pandas/start_activities/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/filtering/pandas/start_activities/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/filtering/pandas/start_activities/start_activities_filter.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/filtering/pandas/start_activities/start_activities_filter.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/filtering/pandas/starts_with/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/filtering/pandas/starts_with/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/filtering/pandas/starts_with/starts_with_filter.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/filtering/pandas/starts_with/starts_with_filter.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/filtering/pandas/suffixes/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/filtering/pandas/suffixes/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/filtering/pandas/suffixes/suffix_filter.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/filtering/pandas/suffixes/suffix_filter.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/filtering/pandas/timestamp/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/filtering/pandas/timestamp/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/filtering/pandas/timestamp/timestamp_filter.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/filtering/pandas/timestamp/timestamp_filter.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/filtering/pandas/timestamp_case_grouping/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/filtering/pandas/timestamp_case_grouping/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/filtering/pandas/timestamp_case_grouping/timestamp_case_grouping_filter.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/filtering/pandas/timestamp_case_grouping/timestamp_case_grouping_filter.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/filtering/pandas/traces/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/filtering/pandas/traces/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/filtering/pandas/traces/trace_filter.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/filtering/pandas/traces/trace_filter.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/filtering/pandas/variants/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/filtering/pandas/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/filtering/pandas/variants/variants_filter.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/filtering/pandas/variants/variants_filter.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/label_splitting/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/label_splitting/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/label_splitting/algorithm.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/label_splitting/algorithm.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/label_splitting/variants/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/label_splitting/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/label_splitting/variants/contextual.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/label_splitting/variants/contextual.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/merging/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/merging/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/merging/case_relations/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/merging/case_relations/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/merging/case_relations/algorithm.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/merging/case_relations/algorithm.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/merging/case_relations/variants/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/merging/case_relations/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/merging/case_relations/variants/pandas.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/merging/case_relations/variants/pandas.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/organizational_mining/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/organizational_mining/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/organizational_mining/local_diagnostics/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/organizational_mining/local_diagnostics/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/organizational_mining/local_diagnostics/algorithm.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/organizational_mining/local_diagnostics/algorithm.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/organizational_mining/network_analysis/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/organizational_mining/network_analysis/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/organizational_mining/network_analysis/algorithm.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/organizational_mining/network_analysis/algorithm.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/organizational_mining/network_analysis/variants/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/organizational_mining/network_analysis/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/organizational_mining/network_analysis/variants/dataframe.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/organizational_mining/network_analysis/variants/dataframe.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/organizational_mining/resource_profiles/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/organizational_mining/resource_profiles/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/organizational_mining/resource_profiles/algorithm.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/organizational_mining/resource_profiles/algorithm.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/organizational_mining/resource_profiles/variants/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/organizational_mining/resource_profiles/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/organizational_mining/resource_profiles/variants/log.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/organizational_mining/resource_profiles/variants/log.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/organizational_mining/resource_profiles/variants/pandas.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/organizational_mining/resource_profiles/variants/pandas.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/organizational_mining/roles/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/organizational_mining/roles/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/organizational_mining/roles/algorithm.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/organizational_mining/roles/algorithm.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/organizational_mining/roles/common/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/organizational_mining/roles/common/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/organizational_mining/roles/common/algorithm.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/organizational_mining/roles/common/algorithm.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/organizational_mining/roles/variants/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/organizational_mining/roles/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/organizational_mining/roles/variants/log.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/organizational_mining/roles/variants/log.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/organizational_mining/roles/variants/pandas.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/organizational_mining/roles/variants/pandas.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/organizational_mining/sna/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/organizational_mining/sna/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/organizational_mining/sna/algorithm.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/organizational_mining/sna/algorithm.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/organizational_mining/sna/util.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/organizational_mining/sna/util.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/organizational_mining/sna/variants/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/organizational_mining/sna/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/organizational_mining/sna/variants/log/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/organizational_mining/sna/variants/log/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/organizational_mining/sna/variants/log/handover.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/organizational_mining/sna/variants/log/handover.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/organizational_mining/sna/variants/log/jointactivities.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/organizational_mining/sna/variants/log/jointactivities.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/organizational_mining/sna/variants/log/subcontracting.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/organizational_mining/sna/variants/log/subcontracting.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/organizational_mining/sna/variants/log/working_together.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/organizational_mining/sna/variants/log/working_together.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/organizational_mining/sna/variants/pandas/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/organizational_mining/sna/variants/pandas/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/organizational_mining/sna/variants/pandas/handover.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/organizational_mining/sna/variants/pandas/handover.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/organizational_mining/sna/variants/pandas/jointactivities.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/organizational_mining/sna/variants/pandas/jointactivities.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/organizational_mining/sna/variants/pandas/subcontracting.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/organizational_mining/sna/variants/pandas/subcontracting.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/organizational_mining/sna/variants/pandas/working_together.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/organizational_mining/sna/variants/pandas/working_together.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/organizational_mining/util.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/organizational_mining/util.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/querying/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/querying/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/querying/llm/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/querying/llm/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/querying/llm/abstractions/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/querying/llm/abstractions/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/querying/llm/abstractions/case_to_descr.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/querying/llm/abstractions/case_to_descr.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/querying/llm/abstractions/declare_to_descr.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/querying/llm/abstractions/declare_to_descr.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/querying/llm/abstractions/log_to_cols_descr.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/querying/llm/abstractions/log_to_cols_descr.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/querying/llm/abstractions/log_to_dfg_descr.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/querying/llm/abstractions/log_to_dfg_descr.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/querying/llm/abstractions/log_to_fea_descr.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/querying/llm/abstractions/log_to_fea_descr.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/querying/llm/abstractions/log_to_variants_descr.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/querying/llm/abstractions/log_to_variants_descr.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/querying/llm/abstractions/logske_to_descr.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/querying/llm/abstractions/logske_to_descr.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/querying/llm/abstractions/net_to_descr.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/querying/llm/abstractions/net_to_descr.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/querying/llm/abstractions/ocel_fea_descr.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/querying/llm/abstractions/ocel_fea_descr.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/querying/llm/abstractions/ocel_ocdfg_descr.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/querying/llm/abstractions/ocel_ocdfg_descr.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/querying/llm/abstractions/stream_to_descr.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/querying/llm/abstractions/stream_to_descr.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/querying/llm/abstractions/tempprofile_to_descr.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/querying/llm/abstractions/tempprofile_to_descr.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/querying/llm/connectors/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/querying/llm/connectors/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/querying/llm/connectors/openai.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/querying/llm/connectors/openai.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/querying/llm/utils/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/querying/llm/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/querying/llm/utils/sql_utils.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/querying/llm/utils/sql_utils.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/reduction/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/reduction/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/reduction/process_tree/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/reduction/process_tree/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/reduction/process_tree/reducer.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/reduction/process_tree/reducer.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/reduction/process_tree/variants/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/reduction/process_tree/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/reduction/process_tree/variants/tree_tr_based.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/reduction/process_tree/variants/tree_tr_based.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/simulation/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/simulation/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/simulation/montecarlo/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/simulation/montecarlo/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/simulation/montecarlo/algorithm.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/simulation/montecarlo/algorithm.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/simulation/montecarlo/utils/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/simulation/montecarlo/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/simulation/montecarlo/utils/replay.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/simulation/montecarlo/utils/replay.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/simulation/montecarlo/variants/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/simulation/montecarlo/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/simulation/montecarlo/variants/petri_semaph_fifo.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/simulation/montecarlo/variants/petri_semaph_fifo.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/simulation/playout/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/simulation/playout/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/simulation/playout/dfg/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/simulation/playout/dfg/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/simulation/playout/dfg/algorithm.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/simulation/playout/dfg/algorithm.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/simulation/playout/dfg/variants/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/simulation/playout/dfg/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/simulation/playout/dfg/variants/classic.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/simulation/playout/dfg/variants/classic.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/simulation/playout/dfg/variants/performance.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/simulation/playout/dfg/variants/performance.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/simulation/playout/petri_net/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/simulation/playout/petri_net/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/simulation/playout/petri_net/algorithm.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/simulation/playout/petri_net/algorithm.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/simulation/playout/petri_net/variants/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/simulation/playout/petri_net/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/simulation/playout/petri_net/variants/basic_playout.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/simulation/playout/petri_net/variants/basic_playout.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/simulation/playout/petri_net/variants/extensive.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/simulation/playout/petri_net/variants/extensive.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/simulation/playout/petri_net/variants/stochastic_playout.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/simulation/playout/petri_net/variants/stochastic_playout.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/simulation/playout/process_tree/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/simulation/playout/process_tree/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/simulation/playout/process_tree/algorithm.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/simulation/playout/process_tree/algorithm.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/simulation/playout/process_tree/variants/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/simulation/playout/process_tree/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/simulation/playout/process_tree/variants/basic_playout.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/simulation/playout/process_tree/variants/basic_playout.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/simulation/playout/process_tree/variants/extensive.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/simulation/playout/process_tree/variants/extensive.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/simulation/playout/process_tree/variants/topbottom.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/simulation/playout/process_tree/variants/topbottom.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/simulation/tree_generator/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/simulation/tree_generator/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/simulation/tree_generator/algorithm.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/simulation/tree_generator/algorithm.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/simulation/tree_generator/variants/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/simulation/tree_generator/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/simulation/tree_generator/variants/basic.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/simulation/tree_generator/variants/basic.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/simulation/tree_generator/variants/ptandloggenerator.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/simulation/tree_generator/variants/ptandloggenerator.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/transformation/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/transformation/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/transformation/log_to_features/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/transformation/log_to_features/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/transformation/log_to_features/algorithm.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/transformation/log_to_features/algorithm.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/transformation/log_to_features/util/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/transformation/log_to_features/util/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/transformation/log_to_features/util/locally_linear_embedding.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/transformation/log_to_features/util/locally_linear_embedding.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/transformation/log_to_features/variants/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/transformation/log_to_features/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/transformation/log_to_features/variants/event_based.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/transformation/log_to_features/variants/event_based.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/transformation/log_to_features/variants/temporal.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/transformation/log_to_features/variants/temporal.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/transformation/log_to_features/variants/trace_based.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/transformation/log_to_features/variants/trace_based.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/transformation/log_to_interval_tree/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/transformation/log_to_interval_tree/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/transformation/log_to_interval_tree/algorithm.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/transformation/log_to_interval_tree/algorithm.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/transformation/log_to_interval_tree/variants/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/transformation/log_to_interval_tree/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/transformation/log_to_interval_tree/variants/open_paths.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/transformation/log_to_interval_tree/variants/open_paths.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/transformation/log_to_target/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/transformation/log_to_target/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/transformation/log_to_target/algorithm.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/transformation/log_to_target/algorithm.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/transformation/log_to_target/variants/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/transformation/log_to_target/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/transformation/log_to_target/variants/next_activity.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/transformation/log_to_target/variants/next_activity.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/transformation/log_to_target/variants/next_time.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/transformation/log_to_target/variants/next_time.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/transformation/log_to_target/variants/remaining_time.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/transformation/log_to_target/variants/remaining_time.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/transformation/log_to_trie/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/transformation/log_to_trie/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/transformation/log_to_trie/algorithm.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/transformation/log_to_trie/algorithm.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/transformation/ocel/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/transformation/ocel/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/transformation/ocel/description/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/transformation/ocel/description/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/transformation/ocel/description/algorithm.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/transformation/ocel/description/algorithm.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/transformation/ocel/description/variants/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/transformation/ocel/description/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/transformation/ocel/description/variants/variant1.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/transformation/ocel/description/variants/variant1.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/transformation/ocel/features/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/transformation/ocel/features/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/transformation/ocel/features/events/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/transformation/ocel/features/events/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/transformation/ocel/features/events/algorithm.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/transformation/ocel/features/events/algorithm.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/transformation/ocel/features/events/event_activity.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/transformation/ocel/features/events/event_activity.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/transformation/ocel/features/events/event_end_ot.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/transformation/ocel/features/events/event_end_ot.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/transformation/ocel/features/events/event_num_attributes.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/transformation/ocel/features/events/event_num_attributes.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/transformation/ocel/features/events/event_num_rel_objs.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/transformation/ocel/features/events/event_num_rel_objs.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/transformation/ocel/features/events/event_num_rel_objs_type.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/transformation/ocel/features/events/event_num_rel_objs_type.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/transformation/ocel/features/events/event_start_ot.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/transformation/ocel/features/events/event_start_ot.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/transformation/ocel/features/events/event_str_attributes.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/transformation/ocel/features/events/event_str_attributes.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/transformation/ocel/features/events/event_timestamp.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/transformation/ocel/features/events/event_timestamp.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/transformation/ocel/features/events/new_interactions.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/transformation/ocel/features/events/new_interactions.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/transformation/ocel/features/events/related_objects_features.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/transformation/ocel/features/events/related_objects_features.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/transformation/ocel/features/events_objects/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/transformation/ocel/features/events_objects/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/transformation/ocel/features/events_objects/algorithm.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/transformation/ocel/features/events_objects/algorithm.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/transformation/ocel/features/events_objects/prefix_features.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/transformation/ocel/features/events_objects/prefix_features.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/transformation/ocel/features/objects/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/transformation/ocel/features/objects/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/transformation/ocel/features/objects/algorithm.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/transformation/ocel/features/objects/algorithm.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/transformation/ocel/features/objects/obj_con_in_graph_features.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/transformation/ocel/features/objects/obj_con_in_graph_features.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/transformation/ocel/features/objects/object_cobirth_graph.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/transformation/ocel/features/objects/object_cobirth_graph.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/transformation/ocel/features/objects/object_codeath_graph.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/transformation/ocel/features/objects/object_codeath_graph.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/transformation/ocel/features/objects/object_degree_centrality.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/transformation/ocel/features/objects/object_degree_centrality.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/transformation/ocel/features/objects/object_general_descendants_graph.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/transformation/ocel/features/objects/object_general_descendants_graph.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/transformation/ocel/features/objects/object_general_inheritance_graph.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/transformation/ocel/features/objects/object_general_inheritance_graph.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/transformation/ocel/features/objects/object_general_interaction_graph.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/transformation/ocel/features/objects/object_general_interaction_graph.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/transformation/ocel/features/objects/object_lifecycle_activities.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/transformation/ocel/features/objects/object_lifecycle_activities.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/transformation/ocel/features/objects/object_lifecycle_duration.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/transformation/ocel/features/objects/object_lifecycle_duration.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/transformation/ocel/features/objects/object_lifecycle_length.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/transformation/ocel/features/objects/object_lifecycle_length.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/transformation/ocel/features/objects/object_lifecycle_paths.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/transformation/ocel/features/objects/object_lifecycle_paths.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/transformation/ocel/features/objects/object_lifecycle_unq_act.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/transformation/ocel/features/objects/object_lifecycle_unq_act.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/transformation/ocel/features/objects/object_num_attributes.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/transformation/ocel/features/objects/object_num_attributes.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/transformation/ocel/features/objects/object_str_attributes.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/transformation/ocel/features/objects/object_str_attributes.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/transformation/ocel/features/objects/object_work_in_progress.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/transformation/ocel/features/objects/object_work_in_progress.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/transformation/ocel/features/objects/objects_interaction_graph_ot.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/transformation/ocel/features/objects/objects_interaction_graph_ot.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/transformation/ocel/features/objects/related_activities_features.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/transformation/ocel/features/objects/related_activities_features.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/transformation/ocel/features/objects/related_events_features.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/transformation/ocel/features/objects/related_events_features.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/transformation/ocel/graphs/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/transformation/ocel/graphs/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/transformation/ocel/graphs/object_cobirth_graph.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/transformation/ocel/graphs/object_cobirth_graph.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/transformation/ocel/graphs/object_codeath_graph.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/transformation/ocel/graphs/object_codeath_graph.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/transformation/ocel/graphs/object_descendants_graph.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/transformation/ocel/graphs/object_descendants_graph.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/transformation/ocel/graphs/object_inheritance_graph.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/transformation/ocel/graphs/object_inheritance_graph.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/transformation/ocel/graphs/object_interaction_graph.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/transformation/ocel/graphs/object_interaction_graph.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/transformation/ocel/graphs/ocel20_computation.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/transformation/ocel/graphs/ocel20_computation.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/transformation/ocel/split_ocel/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/transformation/ocel/split_ocel/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/transformation/ocel/split_ocel/algorithm.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/transformation/ocel/split_ocel/algorithm.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/transformation/ocel/split_ocel/variants/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/transformation/ocel/split_ocel/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/transformation/ocel/split_ocel/variants/ancestors_descendants.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/transformation/ocel/split_ocel/variants/ancestors_descendants.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/algo/transformation/ocel/split_ocel/variants/connected_components.py` & `pm4pyminimal-2.7.9.4/pm4py/algo/transformation/ocel/split_ocel/variants/connected_components.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/analysis.py` & `pm4pyminimal-2.7.9.4/pm4py/analysis.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/cli.py` & `pm4pyminimal-2.7.9.4/pm4py/cli.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/conformance.py` & `pm4pyminimal-2.7.9.4/pm4py/conformance.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/connectors.py` & `pm4pyminimal-2.7.9.4/pm4py/connectors.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/convert.py` & `pm4pyminimal-2.7.9.4/pm4py/convert.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/discovery.py` & `pm4pyminimal-2.7.9.4/pm4py/discovery.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/filtering.py` & `pm4pyminimal-2.7.9.4/pm4py/filtering.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/hof.py` & `pm4pyminimal-2.7.9.4/pm4py/hof.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/llm.py` & `pm4pyminimal-2.7.9.4/pm4py/llm.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/meta.py` & `pm4pyminimal-2.7.9.4/pm4py/meta.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,14 +12,14 @@
     GNU General Public License for more details.
 
     You should have received a copy of the GNU General Public License
     along with PM4Py.  If not, see <https://www.gnu.org/licenses/>.
 '''
 
 __name__ = 'pm4pyminimal'
-VERSION = '2.7.9.3'
+VERSION = '2.7.9.4'
 __version__ = VERSION
 __doc__ = 'Process mining for Python'
 __author__ = 'Fraunhofer Institute for Applied Information Technology FIT'
 __author_email__ = 'pm4py@fit.fraunhofer.de'
 __maintainer__ = 'Fraunhofer Institute for Applied Information Technology FIT'
 __maintainer_email__ = "pm4py@fit.fraunhofer.de"
```

### Comparing `pm4pyminimal-2.7.9.3/pm4py/ml.py` & `pm4pyminimal-2.7.9.4/pm4py/ml.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/objects/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/objects/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/objects/bpmn/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/objects/bpmn/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/objects/bpmn/exporter/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/objects/bpmn/exporter/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/objects/bpmn/exporter/exporter.py` & `pm4pyminimal-2.7.9.4/pm4py/objects/bpmn/exporter/exporter.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/objects/bpmn/exporter/variants/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/objects/bpmn/exporter/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/objects/bpmn/exporter/variants/etree.py` & `pm4pyminimal-2.7.9.4/pm4py/objects/bpmn/exporter/variants/etree.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/objects/bpmn/importer/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/objects/bpmn/importer/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/objects/bpmn/importer/importer.py` & `pm4pyminimal-2.7.9.4/pm4py/objects/bpmn/importer/importer.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/objects/bpmn/importer/variants/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/objects/bpmn/importer/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/objects/bpmn/importer/variants/lxml.py` & `pm4pyminimal-2.7.9.4/pm4py/objects/bpmn/importer/variants/lxml.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/objects/bpmn/layout/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/objects/bpmn/layout/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/objects/bpmn/layout/layouter.py` & `pm4pyminimal-2.7.9.4/pm4py/objects/bpmn/layout/layouter.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/objects/bpmn/layout/variants/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/objects/bpmn/layout/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/objects/bpmn/layout/variants/graphviz.py` & `pm4pyminimal-2.7.9.4/pm4py/objects/bpmn/layout/variants/graphviz.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/objects/bpmn/obj.py` & `pm4pyminimal-2.7.9.4/pm4py/objects/bpmn/obj.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/objects/bpmn/semantics.py` & `pm4pyminimal-2.7.9.4/pm4py/objects/bpmn/semantics.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/objects/bpmn/util/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/objects/bpmn/util/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/objects/bpmn/util/bpmn_utils.py` & `pm4pyminimal-2.7.9.4/pm4py/objects/bpmn/util/bpmn_utils.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/objects/bpmn/util/reduction.py` & `pm4pyminimal-2.7.9.4/pm4py/objects/bpmn/util/reduction.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/objects/bpmn/util/sorting.py` & `pm4pyminimal-2.7.9.4/pm4py/objects/bpmn/util/sorting.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/objects/conversion/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/objects/conversion/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/objects/conversion/bpmn/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/objects/conversion/bpmn/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/objects/conversion/bpmn/converter.py` & `pm4pyminimal-2.7.9.4/pm4py/objects/conversion/bpmn/converter.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/objects/conversion/bpmn/variants/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/objects/conversion/bpmn/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/objects/conversion/bpmn/variants/to_petri_net.py` & `pm4pyminimal-2.7.9.4/pm4py/objects/conversion/bpmn/variants/to_petri_net.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/objects/conversion/dfg/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/objects/conversion/dfg/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/objects/conversion/dfg/converter.py` & `pm4pyminimal-2.7.9.4/pm4py/objects/conversion/dfg/converter.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/objects/conversion/dfg/variants/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/objects/conversion/dfg/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/objects/conversion/dfg/variants/to_petri_net_activity_defines_place.py` & `pm4pyminimal-2.7.9.4/pm4py/objects/conversion/dfg/variants/to_petri_net_activity_defines_place.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/objects/conversion/dfg/variants/to_petri_net_invisibles_no_duplicates.py` & `pm4pyminimal-2.7.9.4/pm4py/objects/conversion/dfg/variants/to_petri_net_invisibles_no_duplicates.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/objects/conversion/heuristics_net/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/objects/conversion/heuristics_net/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/objects/conversion/heuristics_net/converter.py` & `pm4pyminimal-2.7.9.4/pm4py/objects/conversion/heuristics_net/converter.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/objects/conversion/heuristics_net/variants/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/objects/conversion/heuristics_net/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/objects/conversion/heuristics_net/variants/to_petri_net.py` & `pm4pyminimal-2.7.9.4/pm4py/objects/conversion/heuristics_net/variants/to_petri_net.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/objects/conversion/log/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/objects/conversion/log/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/objects/conversion/log/constants.py` & `pm4pyminimal-2.7.9.4/pm4py/objects/conversion/log/constants.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/objects/conversion/log/converter.py` & `pm4pyminimal-2.7.9.4/pm4py/objects/conversion/log/converter.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/objects/conversion/log/variants/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/objects/conversion/log/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/objects/conversion/log/variants/df_to_event_log_1v.py` & `pm4pyminimal-2.7.9.4/pm4py/objects/conversion/log/variants/df_to_event_log_1v.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/objects/conversion/log/variants/df_to_event_log_nv.py` & `pm4pyminimal-2.7.9.4/pm4py/objects/conversion/log/variants/df_to_event_log_nv.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/objects/conversion/log/variants/to_data_frame.py` & `pm4pyminimal-2.7.9.4/pm4py/objects/conversion/log/variants/to_data_frame.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/objects/conversion/log/variants/to_event_log.py` & `pm4pyminimal-2.7.9.4/pm4py/objects/conversion/log/variants/to_event_log.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/objects/conversion/log/variants/to_event_stream.py` & `pm4pyminimal-2.7.9.4/pm4py/objects/conversion/log/variants/to_event_stream.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/objects/conversion/log/variants/to_nx.py` & `pm4pyminimal-2.7.9.4/pm4py/objects/conversion/log/variants/to_nx.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/objects/conversion/ocel/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/objects/conversion/ocel/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/objects/conversion/ocel/converter.py` & `pm4pyminimal-2.7.9.4/pm4py/objects/conversion/ocel/converter.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/objects/conversion/ocel/variants/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/objects/conversion/ocel/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/objects/conversion/ocel/variants/ocel_features_to_nx.py` & `pm4pyminimal-2.7.9.4/pm4py/objects/conversion/ocel/variants/ocel_features_to_nx.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/objects/conversion/ocel/variants/ocel_to_nx.py` & `pm4pyminimal-2.7.9.4/pm4py/objects/conversion/ocel/variants/ocel_to_nx.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/objects/conversion/powl/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/objects/conversion/powl/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/objects/conversion/powl/converter.py` & `pm4pyminimal-2.7.9.4/pm4py/objects/conversion/powl/converter.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/objects/conversion/powl/variants/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/objects/conversion/powl/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/objects/conversion/powl/variants/to_petri_net.py` & `pm4pyminimal-2.7.9.4/pm4py/objects/conversion/powl/variants/to_petri_net.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/objects/conversion/process_tree/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/objects/conversion/process_tree/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/objects/conversion/process_tree/converter.py` & `pm4pyminimal-2.7.9.4/pm4py/objects/conversion/process_tree/converter.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/objects/conversion/process_tree/variants/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/objects/conversion/process_tree/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/objects/conversion/process_tree/variants/to_bpmn.py` & `pm4pyminimal-2.7.9.4/pm4py/objects/conversion/process_tree/variants/to_bpmn.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/objects/conversion/process_tree/variants/to_petri_net.py` & `pm4pyminimal-2.7.9.4/pm4py/objects/conversion/process_tree/variants/to_petri_net.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/objects/conversion/process_tree/variants/to_petri_net_transition_bordered.py` & `pm4pyminimal-2.7.9.4/pm4py/objects/conversion/process_tree/variants/to_petri_net_transition_bordered.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/objects/conversion/wf_net/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/objects/conversion/wf_net/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/objects/conversion/wf_net/converter.py` & `pm4pyminimal-2.7.9.4/pm4py/objects/conversion/wf_net/converter.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/objects/conversion/wf_net/variants/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/objects/conversion/wf_net/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/objects/conversion/wf_net/variants/to_bpmn.py` & `pm4pyminimal-2.7.9.4/pm4py/objects/conversion/wf_net/variants/to_bpmn.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/objects/conversion/wf_net/variants/to_process_tree.py` & `pm4pyminimal-2.7.9.4/pm4py/objects/conversion/wf_net/variants/to_process_tree.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/objects/dfg/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/objects/dfg/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/objects/dfg/exporter/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/objects/dfg/exporter/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/objects/dfg/exporter/exporter.py` & `pm4pyminimal-2.7.9.4/pm4py/objects/dfg/exporter/exporter.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/objects/dfg/exporter/variants/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/objects/dfg/exporter/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/objects/dfg/exporter/variants/classic.py` & `pm4pyminimal-2.7.9.4/pm4py/objects/dfg/exporter/variants/classic.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/objects/dfg/filtering/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/objects/dfg/filtering/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/objects/dfg/filtering/dfg_filtering.py` & `pm4pyminimal-2.7.9.4/pm4py/objects/dfg/filtering/dfg_filtering.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/objects/dfg/importer/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/objects/dfg/importer/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/objects/dfg/importer/importer.py` & `pm4pyminimal-2.7.9.4/pm4py/objects/dfg/importer/importer.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/objects/dfg/importer/variants/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/objects/dfg/importer/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/objects/dfg/importer/variants/classic.py` & `pm4pyminimal-2.7.9.4/pm4py/objects/dfg/importer/variants/classic.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/objects/dfg/obj.py` & `pm4pyminimal-2.7.9.4/pm4py/objects/dfg/obj.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/objects/dfg/retrieval/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/objects/dfg/retrieval/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/objects/dfg/retrieval/log.py` & `pm4pyminimal-2.7.9.4/pm4py/objects/dfg/retrieval/log.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/objects/dfg/retrieval/pandas.py` & `pm4pyminimal-2.7.9.4/pm4py/objects/dfg/retrieval/pandas.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/objects/dfg/util.py` & `pm4pyminimal-2.7.9.4/pm4py/objects/dfg/util.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/objects/dfg/utils/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/objects/dfg/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/objects/dfg/utils/dfg_utils.py` & `pm4pyminimal-2.7.9.4/pm4py/objects/dfg/utils/dfg_utils.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/objects/heuristics_net/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/objects/heuristics_net/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/objects/heuristics_net/defaults.py` & `pm4pyminimal-2.7.9.4/pm4py/objects/heuristics_net/defaults.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/objects/heuristics_net/edge.py` & `pm4pyminimal-2.7.9.4/pm4py/objects/heuristics_net/edge.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/objects/heuristics_net/node.py` & `pm4pyminimal-2.7.9.4/pm4py/objects/heuristics_net/node.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/objects/heuristics_net/obj.py` & `pm4pyminimal-2.7.9.4/pm4py/objects/heuristics_net/obj.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/objects/log/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/objects/log/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/objects/log/exporter/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/objects/log/exporter/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/objects/log/exporter/xes/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/objects/log/exporter/xes/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/objects/log/exporter/xes/exporter.py` & `pm4pyminimal-2.7.9.4/pm4py/objects/log/exporter/xes/exporter.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/objects/log/exporter/xes/util/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/objects/log/exporter/xes/util/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/objects/log/exporter/xes/util/compression.py` & `pm4pyminimal-2.7.9.4/pm4py/objects/log/exporter/xes/util/compression.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/objects/log/exporter/xes/variants/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/objects/log/exporter/xes/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/objects/log/exporter/xes/variants/etree_xes_exp.py` & `pm4pyminimal-2.7.9.4/pm4py/objects/log/exporter/xes/variants/etree_xes_exp.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/objects/log/exporter/xes/variants/line_by_line.py` & `pm4pyminimal-2.7.9.4/pm4py/objects/log/exporter/xes/variants/line_by_line.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/objects/log/importer/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/objects/log/importer/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/objects/log/importer/xes/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/objects/log/importer/xes/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/objects/log/importer/xes/importer.py` & `pm4pyminimal-2.7.9.4/pm4py/objects/log/importer/xes/importer.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/objects/log/importer/xes/variants/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/objects/log/importer/xes/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/objects/log/importer/xes/variants/chunk_regex.py` & `pm4pyminimal-2.7.9.4/pm4py/objects/log/importer/xes/variants/chunk_regex.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/objects/log/importer/xes/variants/iterparse.py` & `pm4pyminimal-2.7.9.4/pm4py/objects/log/importer/xes/variants/iterparse.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/objects/log/importer/xes/variants/iterparse_20.py` & `pm4pyminimal-2.7.9.4/pm4py/objects/log/importer/xes/variants/iterparse_20.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/objects/log/importer/xes/variants/iterparse_mem_compressed.py` & `pm4pyminimal-2.7.9.4/pm4py/objects/log/importer/xes/variants/iterparse_mem_compressed.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/objects/log/importer/xes/variants/line_by_line.py` & `pm4pyminimal-2.7.9.4/pm4py/objects/log/importer/xes/variants/line_by_line.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/objects/log/importer/xes/variants/rustxes.py` & `pm4pyminimal-2.7.9.4/pm4py/objects/log/importer/xes/variants/rustxes.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/objects/log/obj.py` & `pm4pyminimal-2.7.9.4/pm4py/objects/log/obj.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/objects/log/util/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/objects/log/util/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/objects/log/util/activities_to_alphabet.py` & `pm4pyminimal-2.7.9.4/pm4py/objects/log/util/activities_to_alphabet.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/objects/log/util/artificial.py` & `pm4pyminimal-2.7.9.4/pm4py/objects/log/util/artificial.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/objects/log/util/basic_filter.py` & `pm4pyminimal-2.7.9.4/pm4py/objects/log/util/basic_filter.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/objects/log/util/dataframe_utils.py` & `pm4pyminimal-2.7.9.4/pm4py/objects/log/util/dataframe_utils.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/objects/log/util/filtering_utils.py` & `pm4pyminimal-2.7.9.4/pm4py/objects/log/util/filtering_utils.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/objects/log/util/get_class_representation.py` & `pm4pyminimal-2.7.9.4/pm4py/objects/log/util/get_class_representation.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/objects/log/util/get_log_encoded.py` & `pm4pyminimal-2.7.9.4/pm4py/objects/log/util/get_log_encoded.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/objects/log/util/get_prefixes.py` & `pm4pyminimal-2.7.9.4/pm4py/objects/log/util/get_prefixes.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/objects/log/util/index_attribute.py` & `pm4pyminimal-2.7.9.4/pm4py/objects/log/util/index_attribute.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/objects/log/util/insert_classifier.py` & `pm4pyminimal-2.7.9.4/pm4py/objects/log/util/insert_classifier.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/objects/log/util/interval_lifecycle.py` & `pm4pyminimal-2.7.9.4/pm4py/objects/log/util/interval_lifecycle.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/objects/log/util/log.py` & `pm4pyminimal-2.7.9.4/pm4py/objects/log/util/log.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/objects/log/util/log_regex.py` & `pm4pyminimal-2.7.9.4/pm4py/objects/log/util/log_regex.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/objects/log/util/move_attrs_to_trace.py` & `pm4pyminimal-2.7.9.4/pm4py/objects/log/util/move_attrs_to_trace.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/objects/log/util/pandas_log_wrapper.py` & `pm4pyminimal-2.7.9.4/pm4py/objects/log/util/pandas_log_wrapper.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/objects/log/util/pandas_numpy_variants.py` & `pm4pyminimal-2.7.9.4/pm4py/objects/log/util/pandas_numpy_variants.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/objects/log/util/sampling.py` & `pm4pyminimal-2.7.9.4/pm4py/objects/log/util/sampling.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/objects/log/util/sorting.py` & `pm4pyminimal-2.7.9.4/pm4py/objects/log/util/sorting.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/objects/log/util/split_train_test.py` & `pm4pyminimal-2.7.9.4/pm4py/objects/log/util/split_train_test.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/objects/log/util/xes.py` & `pm4pyminimal-2.7.9.4/pm4py/objects/log/util/xes.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/objects/ocel/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/objects/ocel/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/objects/ocel/constants.py` & `pm4pyminimal-2.7.9.4/pm4py/objects/ocel/constants.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/objects/ocel/exporter/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/objects/ocel/exporter/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/objects/ocel/exporter/csv/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/objects/ocel/exporter/csv/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/objects/ocel/exporter/csv/exporter.py` & `pm4pyminimal-2.7.9.4/pm4py/objects/ocel/exporter/csv/exporter.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/objects/ocel/exporter/csv/variants/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/objects/ocel/exporter/csv/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/objects/ocel/exporter/csv/variants/pandas.py` & `pm4pyminimal-2.7.9.4/pm4py/objects/ocel/exporter/csv/variants/pandas.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/objects/ocel/exporter/jsonocel/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/objects/ocel/exporter/jsonocel/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/objects/ocel/exporter/jsonocel/exporter.py` & `pm4pyminimal-2.7.9.4/pm4py/objects/ocel/exporter/jsonocel/exporter.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/objects/ocel/exporter/jsonocel/variants/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/objects/ocel/exporter/jsonocel/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/objects/ocel/exporter/jsonocel/variants/classic.py` & `pm4pyminimal-2.7.9.4/pm4py/objects/ocel/exporter/jsonocel/variants/classic.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/objects/ocel/exporter/jsonocel/variants/ocel20.py` & `pm4pyminimal-2.7.9.4/pm4py/objects/ocel/exporter/jsonocel/variants/ocel20.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/objects/ocel/exporter/jsonocel/variants/ocel20_standard.py` & `pm4pyminimal-2.7.9.4/pm4py/objects/ocel/exporter/jsonocel/variants/ocel20_standard.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/objects/ocel/exporter/sqlite/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/objects/ocel/exporter/sqlite/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/objects/ocel/exporter/sqlite/exporter.py` & `pm4pyminimal-2.7.9.4/pm4py/objects/ocel/exporter/sqlite/exporter.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/objects/ocel/exporter/sqlite/variants/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/objects/ocel/exporter/sqlite/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/objects/ocel/exporter/sqlite/variants/ocel20.py` & `pm4pyminimal-2.7.9.4/pm4py/objects/ocel/exporter/sqlite/variants/ocel20.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/objects/ocel/exporter/sqlite/variants/pandas_exporter.py` & `pm4pyminimal-2.7.9.4/pm4py/objects/ocel/exporter/sqlite/variants/pandas_exporter.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/objects/ocel/exporter/util/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/objects/ocel/exporter/util/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/objects/ocel/exporter/util/clean_dataframes.py` & `pm4pyminimal-2.7.9.4/pm4py/objects/ocel/exporter/util/clean_dataframes.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/objects/ocel/exporter/xmlocel/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/objects/ocel/exporter/xmlocel/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/objects/ocel/exporter/xmlocel/exporter.py` & `pm4pyminimal-2.7.9.4/pm4py/objects/ocel/exporter/xmlocel/exporter.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/objects/ocel/exporter/xmlocel/variants/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/objects/ocel/exporter/xmlocel/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/objects/ocel/exporter/xmlocel/variants/classic.py` & `pm4pyminimal-2.7.9.4/pm4py/objects/ocel/exporter/xmlocel/variants/classic.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/objects/ocel/exporter/xmlocel/variants/ocel20.py` & `pm4pyminimal-2.7.9.4/pm4py/objects/ocel/exporter/xmlocel/variants/ocel20.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/objects/ocel/importer/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/objects/ocel/importer/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/objects/ocel/importer/csv/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/objects/ocel/importer/csv/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/objects/ocel/importer/csv/importer.py` & `pm4pyminimal-2.7.9.4/pm4py/objects/ocel/importer/csv/importer.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/objects/ocel/importer/csv/variants/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/objects/ocel/importer/csv/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/objects/ocel/importer/csv/variants/pandas.py` & `pm4pyminimal-2.7.9.4/pm4py/objects/ocel/importer/csv/variants/pandas.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/objects/ocel/importer/jsonocel/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/objects/ocel/importer/jsonocel/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/objects/ocel/importer/jsonocel/importer.py` & `pm4pyminimal-2.7.9.4/pm4py/objects/ocel/importer/jsonocel/importer.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/objects/ocel/importer/jsonocel/variants/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/objects/ocel/importer/jsonocel/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/objects/ocel/importer/jsonocel/variants/classic.py` & `pm4pyminimal-2.7.9.4/pm4py/objects/ocel/importer/jsonocel/variants/classic.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/objects/ocel/importer/jsonocel/variants/ocel20_standard.py` & `pm4pyminimal-2.7.9.4/pm4py/objects/ocel/importer/jsonocel/variants/ocel20_standard.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/objects/ocel/importer/sqlite/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/objects/ocel/importer/sqlite/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/objects/ocel/importer/sqlite/importer.py` & `pm4pyminimal-2.7.9.4/pm4py/objects/ocel/importer/sqlite/importer.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/objects/ocel/importer/sqlite/variants/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/objects/ocel/importer/sqlite/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/objects/ocel/importer/sqlite/variants/ocel20.py` & `pm4pyminimal-2.7.9.4/pm4py/objects/ocel/importer/sqlite/variants/ocel20.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/objects/ocel/importer/sqlite/variants/pandas_importer.py` & `pm4pyminimal-2.7.9.4/pm4py/objects/ocel/importer/sqlite/variants/pandas_importer.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/objects/ocel/importer/xmlocel/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/objects/ocel/importer/xmlocel/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/objects/ocel/importer/xmlocel/importer.py` & `pm4pyminimal-2.7.9.4/pm4py/objects/ocel/importer/xmlocel/importer.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/objects/ocel/importer/xmlocel/variants/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/objects/ocel/importer/xmlocel/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/objects/ocel/importer/xmlocel/variants/classic.py` & `pm4pyminimal-2.7.9.4/pm4py/objects/ocel/importer/xmlocel/variants/classic.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/objects/ocel/importer/xmlocel/variants/ocel20.py` & `pm4pyminimal-2.7.9.4/pm4py/objects/ocel/importer/xmlocel/variants/ocel20.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/objects/ocel/obj.py` & `pm4pyminimal-2.7.9.4/pm4py/objects/ocel/obj.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/objects/ocel/util/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/objects/ocel/util/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/objects/ocel/util/attributes_names.py` & `pm4pyminimal-2.7.9.4/pm4py/objects/ocel/util/attributes_names.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/objects/ocel/util/attributes_per_type.py` & `pm4pyminimal-2.7.9.4/pm4py/objects/ocel/util/attributes_per_type.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/objects/ocel/util/convergence_divergence_diagnostics.py` & `pm4pyminimal-2.7.9.4/pm4py/objects/ocel/util/convergence_divergence_diagnostics.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/objects/ocel/util/e2o_qualification.py` & `pm4pyminimal-2.7.9.4/pm4py/objects/ocel/util/e2o_qualification.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/objects/ocel/util/ev_att_to_obj_type.py` & `pm4pyminimal-2.7.9.4/pm4py/objects/ocel/util/ev_att_to_obj_type.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/objects/ocel/util/event_prefix_suffix_per_obj.py` & `pm4pyminimal-2.7.9.4/pm4py/objects/ocel/util/event_prefix_suffix_per_obj.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/objects/ocel/util/events_per_object_type.py` & `pm4pyminimal-2.7.9.4/pm4py/objects/ocel/util/events_per_object_type.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/objects/ocel/util/events_per_type_per_activity.py` & `pm4pyminimal-2.7.9.4/pm4py/objects/ocel/util/events_per_type_per_activity.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/objects/ocel/util/explode.py` & `pm4pyminimal-2.7.9.4/pm4py/objects/ocel/util/explode.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/objects/ocel/util/extended_table.py` & `pm4pyminimal-2.7.9.4/pm4py/objects/ocel/util/extended_table.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/objects/ocel/util/filtering_utils.py` & `pm4pyminimal-2.7.9.4/pm4py/objects/ocel/util/filtering_utils.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/objects/ocel/util/flattening.py` & `pm4pyminimal-2.7.9.4/pm4py/objects/ocel/util/flattening.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/objects/ocel/util/log_ocel.py` & `pm4pyminimal-2.7.9.4/pm4py/objects/ocel/util/log_ocel.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/objects/ocel/util/names_stripping.py` & `pm4pyminimal-2.7.9.4/pm4py/objects/ocel/util/names_stripping.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/objects/ocel/util/objects_per_type_per_activity.py` & `pm4pyminimal-2.7.9.4/pm4py/objects/ocel/util/objects_per_type_per_activity.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/objects/ocel/util/ocel_consistency.py` & `pm4pyminimal-2.7.9.4/pm4py/objects/ocel/util/ocel_consistency.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/objects/ocel/util/ocel_iterator.py` & `pm4pyminimal-2.7.9.4/pm4py/objects/ocel/util/ocel_iterator.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/objects/ocel/util/ocel_to_dict_types_rel.py` & `pm4pyminimal-2.7.9.4/pm4py/objects/ocel/util/ocel_to_dict_types_rel.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/objects/ocel/util/ocel_type_renaming.py` & `pm4pyminimal-2.7.9.4/pm4py/objects/ocel/util/ocel_type_renaming.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/objects/ocel/util/parent_children_ref.py` & `pm4pyminimal-2.7.9.4/pm4py/objects/ocel/util/parent_children_ref.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/objects/ocel/util/related_events.py` & `pm4pyminimal-2.7.9.4/pm4py/objects/ocel/util/related_events.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/objects/ocel/util/related_objects.py` & `pm4pyminimal-2.7.9.4/pm4py/objects/ocel/util/related_objects.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/objects/ocel/util/rename_objs_ot_tim_lex.py` & `pm4pyminimal-2.7.9.4/pm4py/objects/ocel/util/rename_objs_ot_tim_lex.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/objects/ocel/util/sampling.py` & `pm4pyminimal-2.7.9.4/pm4py/objects/ocel/util/sampling.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/objects/ocel/validation/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/objects/ocel/validation/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/objects/ocel/validation/jsonocel.py` & `pm4pyminimal-2.7.9.4/pm4py/objects/ocel/validation/jsonocel.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/objects/ocel/validation/ocel20_rel_validation.py` & `pm4pyminimal-2.7.9.4/pm4py/objects/ocel/validation/ocel20_rel_validation.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/objects/ocel/validation/xmlocel.py` & `pm4pyminimal-2.7.9.4/pm4py/objects/ocel/validation/xmlocel.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/objects/org/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/objects/org/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/objects/org/roles/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/objects/org/roles/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/objects/org/roles/obj.py` & `pm4pyminimal-2.7.9.4/pm4py/objects/org/roles/obj.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/objects/org/sna/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/objects/org/sna/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/objects/org/sna/obj.py` & `pm4pyminimal-2.7.9.4/pm4py/objects/org/sna/obj.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/objects/petri_net/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/objects/petri_net/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/objects/petri_net/data_petri_nets/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/objects/petri_net/data_petri_nets/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/objects/petri_net/data_petri_nets/data_marking.py` & `pm4pyminimal-2.7.9.4/pm4py/objects/petri_net/data_petri_nets/data_marking.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/objects/petri_net/data_petri_nets/semantics.py` & `pm4pyminimal-2.7.9.4/pm4py/objects/petri_net/data_petri_nets/semantics.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/objects/petri_net/exporter/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/objects/petri_net/exporter/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/objects/petri_net/exporter/exporter.py` & `pm4pyminimal-2.7.9.4/pm4py/objects/petri_net/exporter/exporter.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/objects/petri_net/exporter/variants/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/objects/petri_net/exporter/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/objects/petri_net/exporter/variants/pnml.py` & `pm4pyminimal-2.7.9.4/pm4py/objects/petri_net/exporter/variants/pnml.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/objects/petri_net/importer/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/objects/petri_net/importer/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/objects/petri_net/importer/importer.py` & `pm4pyminimal-2.7.9.4/pm4py/objects/petri_net/importer/importer.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/objects/petri_net/importer/variants/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/objects/petri_net/importer/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/objects/petri_net/importer/variants/pnml.py` & `pm4pyminimal-2.7.9.4/pm4py/objects/petri_net/importer/variants/pnml.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/objects/petri_net/inhibitor_reset/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/objects/petri_net/inhibitor_reset/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/objects/petri_net/inhibitor_reset/semantics.py` & `pm4pyminimal-2.7.9.4/pm4py/objects/petri_net/inhibitor_reset/semantics.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/objects/petri_net/obj.py` & `pm4pyminimal-2.7.9.4/pm4py/objects/petri_net/obj.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/objects/petri_net/properties.py` & `pm4pyminimal-2.7.9.4/pm4py/objects/petri_net/properties.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/objects/petri_net/saw_net/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/objects/petri_net/saw_net/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/objects/petri_net/saw_net/convert.py` & `pm4pyminimal-2.7.9.4/pm4py/objects/petri_net/saw_net/convert.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/objects/petri_net/saw_net/obj.py` & `pm4pyminimal-2.7.9.4/pm4py/objects/petri_net/saw_net/obj.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/objects/petri_net/saw_net/semantics.py` & `pm4pyminimal-2.7.9.4/pm4py/objects/petri_net/saw_net/semantics.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/objects/petri_net/sem_interface.py` & `pm4pyminimal-2.7.9.4/pm4py/objects/petri_net/sem_interface.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/objects/petri_net/semantics.py` & `pm4pyminimal-2.7.9.4/pm4py/objects/petri_net/semantics.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/objects/petri_net/stochastic/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/objects/petri_net/stochastic/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/objects/petri_net/stochastic/obj.py` & `pm4pyminimal-2.7.9.4/pm4py/objects/petri_net/stochastic/obj.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/objects/petri_net/stochastic/semantics.py` & `pm4pyminimal-2.7.9.4/pm4py/objects/petri_net/stochastic/semantics.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/objects/petri_net/utils/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/objects/petri_net/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/objects/petri_net/utils/align_utils.py` & `pm4pyminimal-2.7.9.4/pm4py/objects/petri_net/utils/align_utils.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/objects/petri_net/utils/check_soundness.py` & `pm4pyminimal-2.7.9.4/pm4py/objects/petri_net/utils/check_soundness.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/objects/petri_net/utils/consumption_matrix.py` & `pm4pyminimal-2.7.9.4/pm4py/objects/petri_net/utils/consumption_matrix.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/objects/petri_net/utils/decomposition.py` & `pm4pyminimal-2.7.9.4/pm4py/objects/petri_net/utils/decomposition.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/objects/petri_net/utils/embed_stochastic_map.py` & `pm4pyminimal-2.7.9.4/pm4py/objects/petri_net/utils/embed_stochastic_map.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/objects/petri_net/utils/explore_path.py` & `pm4pyminimal-2.7.9.4/pm4py/objects/petri_net/utils/explore_path.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/objects/petri_net/utils/final_marking.py` & `pm4pyminimal-2.7.9.4/pm4py/objects/petri_net/utils/final_marking.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/objects/petri_net/utils/incidence_matrix.py` & `pm4pyminimal-2.7.9.4/pm4py/objects/petri_net/utils/incidence_matrix.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/objects/petri_net/utils/initial_marking.py` & `pm4pyminimal-2.7.9.4/pm4py/objects/petri_net/utils/initial_marking.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/objects/petri_net/utils/murata.py` & `pm4pyminimal-2.7.9.4/pm4py/objects/petri_net/utils/murata.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/objects/petri_net/utils/networkx_graph.py` & `pm4pyminimal-2.7.9.4/pm4py/objects/petri_net/utils/networkx_graph.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/objects/petri_net/utils/obj_marking.py` & `pm4pyminimal-2.7.9.4/pm4py/objects/petri_net/utils/obj_marking.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/objects/petri_net/utils/performance_map.py` & `pm4pyminimal-2.7.9.4/pm4py/objects/petri_net/utils/performance_map.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/objects/petri_net/utils/petri_utils.py` & `pm4pyminimal-2.7.9.4/pm4py/objects/petri_net/utils/petri_utils.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/objects/petri_net/utils/projection.py` & `pm4pyminimal-2.7.9.4/pm4py/objects/petri_net/utils/projection.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/objects/petri_net/utils/reachability_graph.py` & `pm4pyminimal-2.7.9.4/pm4py/objects/petri_net/utils/reachability_graph.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/objects/petri_net/utils/reduction.py` & `pm4pyminimal-2.7.9.4/pm4py/objects/petri_net/utils/reduction.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/objects/petri_net/utils/synchronous_product.py` & `pm4pyminimal-2.7.9.4/pm4py/objects/petri_net/utils/synchronous_product.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/objects/powl/BinaryRelation.py` & `pm4pyminimal-2.7.9.4/pm4py/objects/powl/BinaryRelation.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/objects/powl/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/objects/powl/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/objects/powl/constants.py` & `pm4pyminimal-2.7.9.4/pm4py/objects/powl/constants.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/objects/powl/obj.py` & `pm4pyminimal-2.7.9.4/pm4py/objects/powl/obj.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/objects/powl/parser.py` & `pm4pyminimal-2.7.9.4/pm4py/objects/powl/parser.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/objects/process_tree/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/objects/process_tree/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/objects/process_tree/exporter/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/objects/process_tree/exporter/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/objects/process_tree/exporter/exporter.py` & `pm4pyminimal-2.7.9.4/pm4py/objects/process_tree/exporter/exporter.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/objects/process_tree/exporter/variants/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/objects/process_tree/exporter/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/objects/process_tree/exporter/variants/ptml.py` & `pm4pyminimal-2.7.9.4/pm4py/objects/process_tree/exporter/variants/ptml.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/objects/process_tree/importer/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/objects/process_tree/importer/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/objects/process_tree/importer/importer.py` & `pm4pyminimal-2.7.9.4/pm4py/objects/process_tree/importer/importer.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/objects/process_tree/importer/variants/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/objects/process_tree/importer/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/objects/process_tree/importer/variants/ptml.py` & `pm4pyminimal-2.7.9.4/pm4py/objects/process_tree/importer/variants/ptml.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/objects/process_tree/obj.py` & `pm4pyminimal-2.7.9.4/pm4py/objects/process_tree/obj.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/objects/process_tree/semantics.py` & `pm4pyminimal-2.7.9.4/pm4py/objects/process_tree/semantics.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/objects/process_tree/state.py` & `pm4pyminimal-2.7.9.4/pm4py/objects/process_tree/state.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/objects/process_tree/utils/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/objects/process_tree/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/objects/process_tree/utils/bottomup.py` & `pm4pyminimal-2.7.9.4/pm4py/objects/process_tree/utils/bottomup.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/objects/process_tree/utils/generic.py` & `pm4pyminimal-2.7.9.4/pm4py/objects/process_tree/utils/generic.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/objects/process_tree/utils/regex.py` & `pm4pyminimal-2.7.9.4/pm4py/objects/process_tree/utils/regex.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/objects/random_variables/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/objects/random_variables/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/objects/random_variables/basic_structure.py` & `pm4pyminimal-2.7.9.4/pm4py/objects/random_variables/basic_structure.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/objects/random_variables/constant0/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/objects/random_variables/constant0/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/objects/random_variables/constant0/random_variable.py` & `pm4pyminimal-2.7.9.4/pm4py/objects/random_variables/constant0/random_variable.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/objects/random_variables/exponential/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/objects/random_variables/exponential/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/objects/random_variables/exponential/random_variable.py` & `pm4pyminimal-2.7.9.4/pm4py/objects/random_variables/exponential/random_variable.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/objects/random_variables/gamma/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/objects/random_variables/gamma/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/objects/random_variables/gamma/random_variable.py` & `pm4pyminimal-2.7.9.4/pm4py/objects/random_variables/gamma/random_variable.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/objects/random_variables/lognormal/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/objects/random_variables/lognormal/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/objects/random_variables/lognormal/random_variable.py` & `pm4pyminimal-2.7.9.4/pm4py/objects/random_variables/lognormal/random_variable.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/objects/random_variables/normal/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/objects/random_variables/normal/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/objects/random_variables/normal/random_variable.py` & `pm4pyminimal-2.7.9.4/pm4py/objects/random_variables/normal/random_variable.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/objects/random_variables/random_variable.py` & `pm4pyminimal-2.7.9.4/pm4py/objects/random_variables/random_variable.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/objects/random_variables/uniform/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/objects/random_variables/uniform/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/objects/random_variables/uniform/random_variable.py` & `pm4pyminimal-2.7.9.4/pm4py/objects/random_variables/uniform/random_variable.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/objects/stochastic_petri/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/objects/stochastic_petri/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/objects/stochastic_petri/ctmc.py` & `pm4pyminimal-2.7.9.4/pm4py/objects/stochastic_petri/ctmc.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/objects/stochastic_petri/tangible_reachability.py` & `pm4pyminimal-2.7.9.4/pm4py/objects/stochastic_petri/tangible_reachability.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/objects/stochastic_petri/utils.py` & `pm4pyminimal-2.7.9.4/pm4py/objects/stochastic_petri/utils.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/objects/transition_system/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/objects/transition_system/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/objects/transition_system/constants.py` & `pm4pyminimal-2.7.9.4/pm4py/objects/transition_system/constants.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/objects/transition_system/obj.py` & `pm4pyminimal-2.7.9.4/pm4py/objects/transition_system/obj.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/objects/transition_system/utils.py` & `pm4pyminimal-2.7.9.4/pm4py/objects/transition_system/utils.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/objects/trie/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/objects/trie/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/objects/trie/obj.py` & `pm4pyminimal-2.7.9.4/pm4py/objects/trie/obj.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/ocel.py` & `pm4pyminimal-2.7.9.4/pm4py/ocel.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/org.py` & `pm4pyminimal-2.7.9.4/pm4py/org.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/privacy.py` & `pm4pyminimal-2.7.9.4/pm4py/privacy.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/read.py` & `pm4pyminimal-2.7.9.4/pm4py/read.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/sim.py` & `pm4pyminimal-2.7.9.4/pm4py/sim.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/statistics/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/statistics/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/statistics/attributes/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/statistics/attributes/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/statistics/attributes/common/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/statistics/attributes/common/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/statistics/attributes/common/get.py` & `pm4pyminimal-2.7.9.4/pm4py/statistics/attributes/common/get.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/statistics/attributes/log/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/statistics/attributes/log/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/statistics/attributes/log/get.py` & `pm4pyminimal-2.7.9.4/pm4py/statistics/attributes/log/get.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/statistics/attributes/log/select.py` & `pm4pyminimal-2.7.9.4/pm4py/statistics/attributes/log/select.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/statistics/attributes/pandas/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/statistics/attributes/pandas/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/statistics/attributes/pandas/get.py` & `pm4pyminimal-2.7.9.4/pm4py/statistics/attributes/pandas/get.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/statistics/concurrent_activities/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/statistics/concurrent_activities/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/statistics/concurrent_activities/log/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/statistics/concurrent_activities/log/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/statistics/concurrent_activities/log/get.py` & `pm4pyminimal-2.7.9.4/pm4py/statistics/concurrent_activities/log/get.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/statistics/concurrent_activities/pandas/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/statistics/concurrent_activities/pandas/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/statistics/concurrent_activities/pandas/get.py` & `pm4pyminimal-2.7.9.4/pm4py/statistics/concurrent_activities/pandas/get.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/statistics/end_activities/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/statistics/end_activities/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/statistics/end_activities/common/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/statistics/end_activities/common/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/statistics/end_activities/common/get.py` & `pm4pyminimal-2.7.9.4/pm4py/statistics/end_activities/common/get.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/statistics/end_activities/log/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/statistics/end_activities/log/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/statistics/end_activities/log/get.py` & `pm4pyminimal-2.7.9.4/pm4py/statistics/end_activities/log/get.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/statistics/end_activities/pandas/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/statistics/end_activities/pandas/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/statistics/end_activities/pandas/get.py` & `pm4pyminimal-2.7.9.4/pm4py/statistics/end_activities/pandas/get.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/statistics/eventually_follows/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/statistics/eventually_follows/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/statistics/eventually_follows/log/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/statistics/eventually_follows/log/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/statistics/eventually_follows/log/get.py` & `pm4pyminimal-2.7.9.4/pm4py/statistics/eventually_follows/log/get.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/statistics/eventually_follows/pandas/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/statistics/eventually_follows/pandas/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/statistics/eventually_follows/pandas/get.py` & `pm4pyminimal-2.7.9.4/pm4py/statistics/eventually_follows/pandas/get.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/statistics/eventually_follows/uvcl/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/statistics/eventually_follows/uvcl/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/statistics/eventually_follows/uvcl/get.py` & `pm4pyminimal-2.7.9.4/pm4py/statistics/eventually_follows/uvcl/get.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/statistics/ocel/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/statistics/ocel/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/statistics/ocel/act_ot_dependent.py` & `pm4pyminimal-2.7.9.4/pm4py/statistics/ocel/act_ot_dependent.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/statistics/ocel/act_utils.py` & `pm4pyminimal-2.7.9.4/pm4py/statistics/ocel/act_utils.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/statistics/ocel/edge_metrics.py` & `pm4pyminimal-2.7.9.4/pm4py/statistics/ocel/edge_metrics.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/statistics/ocel/objects_ot_count.py` & `pm4pyminimal-2.7.9.4/pm4py/statistics/ocel/objects_ot_count.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/statistics/ocel/ot_activities.py` & `pm4pyminimal-2.7.9.4/pm4py/statistics/ocel/ot_activities.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/statistics/overlap/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/statistics/overlap/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/statistics/overlap/cases/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/statistics/overlap/cases/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/statistics/overlap/cases/log/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/statistics/overlap/cases/log/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/statistics/overlap/cases/log/get.py` & `pm4pyminimal-2.7.9.4/pm4py/statistics/overlap/cases/log/get.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/statistics/overlap/cases/pandas/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/statistics/overlap/cases/pandas/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/statistics/overlap/cases/pandas/get.py` & `pm4pyminimal-2.7.9.4/pm4py/statistics/overlap/cases/pandas/get.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/statistics/overlap/interval_events/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/statistics/overlap/interval_events/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/statistics/overlap/interval_events/log/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/statistics/overlap/interval_events/log/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/statistics/overlap/interval_events/log/get.py` & `pm4pyminimal-2.7.9.4/pm4py/statistics/overlap/interval_events/log/get.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/statistics/overlap/interval_events/pandas/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/statistics/overlap/interval_events/pandas/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/statistics/overlap/interval_events/pandas/get.py` & `pm4pyminimal-2.7.9.4/pm4py/statistics/overlap/interval_events/pandas/get.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/statistics/overlap/utils/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/statistics/overlap/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/statistics/overlap/utils/compute.py` & `pm4pyminimal-2.7.9.4/pm4py/statistics/overlap/utils/compute.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/statistics/passed_time/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/statistics/passed_time/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/statistics/passed_time/log/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/statistics/passed_time/log/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/statistics/passed_time/log/algorithm.py` & `pm4pyminimal-2.7.9.4/pm4py/statistics/passed_time/log/algorithm.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/statistics/passed_time/log/variants/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/statistics/passed_time/log/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/statistics/passed_time/log/variants/post.py` & `pm4pyminimal-2.7.9.4/pm4py/statistics/passed_time/log/variants/post.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/statistics/passed_time/log/variants/pre.py` & `pm4pyminimal-2.7.9.4/pm4py/statistics/passed_time/log/variants/pre.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/statistics/passed_time/log/variants/prepost.py` & `pm4pyminimal-2.7.9.4/pm4py/statistics/passed_time/log/variants/prepost.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/statistics/passed_time/pandas/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/statistics/passed_time/pandas/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/statistics/passed_time/pandas/algorithm.py` & `pm4pyminimal-2.7.9.4/pm4py/statistics/passed_time/pandas/algorithm.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/statistics/passed_time/pandas/variants/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/statistics/passed_time/pandas/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/statistics/passed_time/pandas/variants/post.py` & `pm4pyminimal-2.7.9.4/pm4py/statistics/passed_time/pandas/variants/post.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/statistics/passed_time/pandas/variants/pre.py` & `pm4pyminimal-2.7.9.4/pm4py/statistics/passed_time/pandas/variants/pre.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/statistics/passed_time/pandas/variants/prepost.py` & `pm4pyminimal-2.7.9.4/pm4py/statistics/passed_time/pandas/variants/prepost.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/statistics/rework/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/statistics/rework/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/statistics/rework/cases/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/statistics/rework/cases/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/statistics/rework/cases/log/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/statistics/rework/cases/log/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/statistics/rework/cases/log/get.py` & `pm4pyminimal-2.7.9.4/pm4py/statistics/rework/cases/log/get.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/statistics/rework/cases/pandas/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/statistics/rework/cases/pandas/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/statistics/rework/cases/pandas/get.py` & `pm4pyminimal-2.7.9.4/pm4py/statistics/rework/cases/pandas/get.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/statistics/rework/log/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/statistics/rework/log/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/statistics/rework/log/get.py` & `pm4pyminimal-2.7.9.4/pm4py/statistics/rework/log/get.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/statistics/rework/pandas/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/statistics/rework/pandas/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/statistics/rework/pandas/get.py` & `pm4pyminimal-2.7.9.4/pm4py/statistics/rework/pandas/get.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/statistics/service_time/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/statistics/service_time/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/statistics/service_time/log/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/statistics/service_time/log/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/statistics/service_time/log/get.py` & `pm4pyminimal-2.7.9.4/pm4py/statistics/service_time/log/get.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/statistics/service_time/pandas/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/statistics/service_time/pandas/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/statistics/service_time/pandas/get.py` & `pm4pyminimal-2.7.9.4/pm4py/statistics/service_time/pandas/get.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/statistics/sojourn_time/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/statistics/sojourn_time/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/statistics/start_activities/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/statistics/start_activities/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/statistics/start_activities/common/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/statistics/start_activities/common/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/statistics/start_activities/common/get.py` & `pm4pyminimal-2.7.9.4/pm4py/statistics/start_activities/common/get.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/statistics/start_activities/log/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/statistics/start_activities/log/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/statistics/start_activities/log/get.py` & `pm4pyminimal-2.7.9.4/pm4py/statistics/start_activities/log/get.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/statistics/start_activities/pandas/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/statistics/start_activities/pandas/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/statistics/start_activities/pandas/get.py` & `pm4pyminimal-2.7.9.4/pm4py/statistics/start_activities/pandas/get.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/statistics/traces/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/statistics/traces/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/statistics/traces/cycle_time/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/statistics/traces/cycle_time/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/statistics/traces/cycle_time/log/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/statistics/traces/cycle_time/log/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/statistics/traces/cycle_time/log/get.py` & `pm4pyminimal-2.7.9.4/pm4py/statistics/traces/cycle_time/log/get.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/statistics/traces/cycle_time/pandas/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/statistics/traces/cycle_time/pandas/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/statistics/traces/cycle_time/pandas/get.py` & `pm4pyminimal-2.7.9.4/pm4py/statistics/traces/cycle_time/pandas/get.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/statistics/traces/cycle_time/util/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/statistics/traces/cycle_time/util/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/statistics/traces/cycle_time/util/compute.py` & `pm4pyminimal-2.7.9.4/pm4py/statistics/traces/cycle_time/util/compute.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/statistics/traces/generic/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/statistics/traces/generic/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/statistics/traces/generic/common/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/statistics/traces/generic/common/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/statistics/traces/generic/common/case_duration.py` & `pm4pyminimal-2.7.9.4/pm4py/statistics/traces/generic/common/case_duration.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/statistics/traces/generic/log/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/statistics/traces/generic/log/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/statistics/traces/generic/log/case_arrival.py` & `pm4pyminimal-2.7.9.4/pm4py/statistics/traces/generic/log/case_arrival.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/statistics/traces/generic/log/case_statistics.py` & `pm4pyminimal-2.7.9.4/pm4py/statistics/traces/generic/log/case_statistics.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/statistics/traces/generic/pandas/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/statistics/traces/generic/pandas/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/statistics/traces/generic/pandas/case_arrival.py` & `pm4pyminimal-2.7.9.4/pm4py/statistics/traces/generic/pandas/case_arrival.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/statistics/traces/generic/pandas/case_statistics.py` & `pm4pyminimal-2.7.9.4/pm4py/statistics/traces/generic/pandas/case_statistics.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/statistics/util/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/statistics/util/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/statistics/util/times_bipartite_matching.py` & `pm4pyminimal-2.7.9.4/pm4py/statistics/util/times_bipartite_matching.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/statistics/variants/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/statistics/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/statistics/variants/log/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/statistics/variants/log/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/statistics/variants/log/get.py` & `pm4pyminimal-2.7.9.4/pm4py/statistics/variants/log/get.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/statistics/variants/pandas/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/statistics/variants/pandas/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/statistics/variants/pandas/get.py` & `pm4pyminimal-2.7.9.4/pm4py/statistics/variants/pandas/get.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/stats.py` & `pm4pyminimal-2.7.9.4/pm4py/stats.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/streaming/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/streaming/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/streaming/algo/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/streaming/algo/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/streaming/algo/conformance/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/streaming/algo/conformance/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/streaming/algo/conformance/footprints/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/streaming/algo/conformance/footprints/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/streaming/algo/conformance/footprints/algorithm.py` & `pm4pyminimal-2.7.9.4/pm4py/streaming/algo/conformance/footprints/algorithm.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/streaming/algo/conformance/footprints/variants/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/streaming/algo/conformance/footprints/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/streaming/algo/conformance/footprints/variants/classic.py` & `pm4pyminimal-2.7.9.4/pm4py/streaming/algo/conformance/footprints/variants/classic.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/streaming/algo/conformance/tbr/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/streaming/algo/conformance/tbr/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/streaming/algo/conformance/tbr/algorithm.py` & `pm4pyminimal-2.7.9.4/pm4py/streaming/algo/conformance/tbr/algorithm.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/streaming/algo/conformance/tbr/variants/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/streaming/algo/conformance/tbr/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/streaming/algo/conformance/tbr/variants/classic.py` & `pm4pyminimal-2.7.9.4/pm4py/streaming/algo/conformance/tbr/variants/classic.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/streaming/algo/conformance/temporal/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/streaming/algo/conformance/temporal/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/streaming/algo/conformance/temporal/algorithm.py` & `pm4pyminimal-2.7.9.4/pm4py/streaming/algo/conformance/temporal/algorithm.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/streaming/algo/conformance/temporal/variants/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/streaming/algo/conformance/temporal/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/streaming/algo/conformance/temporal/variants/classic.py` & `pm4pyminimal-2.7.9.4/pm4py/streaming/algo/conformance/temporal/variants/classic.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/streaming/algo/discovery/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/streaming/algo/discovery/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/streaming/algo/discovery/dfg/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/streaming/algo/discovery/dfg/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/streaming/algo/discovery/dfg/algorithm.py` & `pm4pyminimal-2.7.9.4/pm4py/streaming/algo/discovery/dfg/algorithm.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/streaming/algo/discovery/dfg/variants/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/streaming/algo/discovery/dfg/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/streaming/algo/discovery/dfg/variants/frequency.py` & `pm4pyminimal-2.7.9.4/pm4py/streaming/algo/discovery/dfg/variants/frequency.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/streaming/algo/interface.py` & `pm4pyminimal-2.7.9.4/pm4py/streaming/algo/interface.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/streaming/conversion/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/streaming/conversion/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/streaming/conversion/from_pandas.py` & `pm4pyminimal-2.7.9.4/pm4py/streaming/conversion/from_pandas.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/streaming/conversion/ocel_flatts_distributor.py` & `pm4pyminimal-2.7.9.4/pm4py/streaming/conversion/ocel_flatts_distributor.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/streaming/importer/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/streaming/importer/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/streaming/importer/csv/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/streaming/importer/csv/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/streaming/importer/csv/importer.py` & `pm4pyminimal-2.7.9.4/pm4py/streaming/importer/csv/importer.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/streaming/importer/csv/variants/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/streaming/importer/csv/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/streaming/importer/csv/variants/csv_event_stream.py` & `pm4pyminimal-2.7.9.4/pm4py/streaming/importer/csv/variants/csv_event_stream.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/streaming/importer/xes/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/streaming/importer/xes/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/streaming/importer/xes/importer.py` & `pm4pyminimal-2.7.9.4/pm4py/streaming/importer/xes/importer.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/streaming/importer/xes/variants/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/streaming/importer/xes/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/streaming/importer/xes/variants/xes_event_stream.py` & `pm4pyminimal-2.7.9.4/pm4py/streaming/importer/xes/variants/xes_event_stream.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/streaming/importer/xes/variants/xes_trace_stream.py` & `pm4pyminimal-2.7.9.4/pm4py/streaming/importer/xes/variants/xes_trace_stream.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/streaming/stream/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/streaming/stream/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/streaming/stream/live_event_stream.py` & `pm4pyminimal-2.7.9.4/pm4py/streaming/stream/live_event_stream.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/streaming/stream/live_trace_stream.py` & `pm4pyminimal-2.7.9.4/pm4py/streaming/stream/live_trace_stream.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/streaming/util/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/streaming/util/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/streaming/util/dictio/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/streaming/util/dictio/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/streaming/util/dictio/generator.py` & `pm4pyminimal-2.7.9.4/pm4py/streaming/util/dictio/generator.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/streaming/util/dictio/versions/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/streaming/util/dictio/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/streaming/util/dictio/versions/classic.py` & `pm4pyminimal-2.7.9.4/pm4py/streaming/util/dictio/versions/classic.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/streaming/util/dictio/versions/redis.py` & `pm4pyminimal-2.7.9.4/pm4py/streaming/util/dictio/versions/redis.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/streaming/util/dictio/versions/thread_safe.py` & `pm4pyminimal-2.7.9.4/pm4py/streaming/util/dictio/versions/thread_safe.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/streaming/util/event_stream_printer.py` & `pm4pyminimal-2.7.9.4/pm4py/streaming/util/event_stream_printer.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/streaming/util/live_to_static_stream.py` & `pm4pyminimal-2.7.9.4/pm4py/streaming/util/live_to_static_stream.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/streaming/util/trace_stream_printer.py` & `pm4pyminimal-2.7.9.4/pm4py/streaming/util/trace_stream_printer.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/util/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/util/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,9 +10,9 @@
     but WITHOUT ANY WARRANTY; without even the implied warranty of
     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
     GNU General Public License for more details.
 
     You should have received a copy of the GNU General Public License
     along with PM4Py.  If not, see <https://www.gnu.org/licenses/>.
 '''
-from pm4py.util import variants_util, lp, constants, points_subset, business_hours, xes_constants, vis_utils, \
-    dt_parsing, colors, exec_utils, pandas_utils, typing, compression
+from pm4py.util import exec_utils, constants, xes_constants, pandas_utils, nx_utils, lp, variants_util, points_subset, business_hours, vis_utils, \
+    dt_parsing, colors, typing, compression
```

### Comparing `pm4pyminimal-2.7.9.3/pm4py/util/business_hours.py` & `pm4pyminimal-2.7.9.4/pm4py/util/business_hours.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/util/colors.py` & `pm4pyminimal-2.7.9.4/pm4py/util/colors.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/util/compression/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/util/compression/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/util/compression/dtypes.py` & `pm4pyminimal-2.7.9.4/pm4py/util/compression/dtypes.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/util/compression/util.py` & `pm4pyminimal-2.7.9.4/pm4py/util/compression/util.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/util/constants.py` & `pm4pyminimal-2.7.9.4/pm4py/util/constants.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/util/dt_parsing/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/util/dt_parsing/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/util/dt_parsing/parser.py` & `pm4pyminimal-2.7.9.4/pm4py/util/dt_parsing/parser.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/util/dt_parsing/variants/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/util/dt_parsing/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/util/dt_parsing/variants/cs8601.py` & `pm4pyminimal-2.7.9.4/pm4py/util/dt_parsing/variants/cs8601.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/util/dt_parsing/variants/dummy.py` & `pm4pyminimal-2.7.9.4/pm4py/util/dt_parsing/variants/dummy.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/util/dt_parsing/variants/strpfromiso.py` & `pm4pyminimal-2.7.9.4/pm4py/util/dt_parsing/variants/strpfromiso.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/util/exec_utils.py` & `pm4pyminimal-2.7.9.4/pm4py/util/exec_utils.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/util/lp/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/util/lp/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/util/lp/solver.py` & `pm4pyminimal-2.7.9.4/pm4py/util/lp/solver.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/util/lp/util/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/util/lp/util/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/util/lp/variants/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/util/lp/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/util/lp/variants/cvxopt_solver.py` & `pm4pyminimal-2.7.9.4/pm4py/util/lp/variants/cvxopt_solver.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/util/lp/variants/cvxopt_solver_custom_align.py` & `pm4pyminimal-2.7.9.4/pm4py/util/lp/variants/cvxopt_solver_custom_align.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/util/lp/variants/cvxopt_solver_custom_align_arm.py` & `pm4pyminimal-2.7.9.4/pm4py/util/lp/variants/cvxopt_solver_custom_align_arm.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/util/lp/variants/cvxopt_solver_custom_align_ilp.py` & `pm4pyminimal-2.7.9.4/pm4py/util/lp/variants/cvxopt_solver_custom_align_ilp.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/util/lp/variants/ortools_solver.py` & `pm4pyminimal-2.7.9.4/pm4py/util/lp/variants/ortools_solver.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/util/lp/variants/pulp_solver.py` & `pm4pyminimal-2.7.9.4/pm4py/util/lp/variants/pulp_solver.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/util/lp/variants/scipy_solver.py` & `pm4pyminimal-2.7.9.4/pm4py/util/lp/variants/scipy_solver.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/util/nx_utils.py` & `pm4pyminimal-2.7.9.4/pm4py/util/nx_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,28 +12,31 @@
     GNU General Public License for more details.
 
     You should have received a copy of the GNU General Public License
     along with PM4Py.  If not, see <https://www.gnu.org/licenses/>.
 '''
 import networkx as nx
 from enum import Enum
-from pm4py.util import exec_utils, constants, dt_parsing, pandas_utils
 from typing import Optional, Dict, Any
-from pm4py.objects.ocel.obj import OCEL
-from pm4py.objects.log.obj import EventLog, Trace, Event
-from pm4py.objects.log.util import sorting
-import pandas as pd
+from pm4py.util import exec_utils, constants
 import importlib.util
 from copy import copy
 
 
 class Parameters(Enum):
     SHOW_PROGRESS_BAR = "show_progress_bar"
 
 
+def get_default_nx_enviroment():
+    return nx
+
+
+DEFAULT_NX_ENVIRONMENT = get_default_nx_enviroment()
+
+
 def __format_attrs(attributes0: Dict[str, Any]) -> Dict[str, Any]:
     """
     Internal method to format properties.
     """
     attributes = {}
 
     keys = list(attributes0.keys())
@@ -138,14 +141,15 @@
     --------------
     nx_graph
         NetworkX DiGraph
     """
     if parameters is None:
         parameters = {}
 
+    from pm4py.util import dt_parsing
     date_parser = dt_parsing.parser.get()
 
     nodes = session.run("MATCH (n) RETURN n")
     nodes = [dict(node["n"]) for node in nodes]
 
     edges = session.run("MATCH (n)-[r]->(m) RETURN n, r, m")
     edges = [(edge["n"]["id"], edge["m"]["id"], dict(edge["r"])) for edge in edges]
@@ -165,15 +169,15 @@
 
     for e in edges:
         nx_graph.add_edge(e[0], e[1], attr=e[2])
 
     return nx_graph
 
 
-def nx_to_ocel(nx_graph: nx.DiGraph, parameters: Optional[Dict[Any, Any]] = None) -> OCEL:
+def nx_to_ocel(nx_graph: nx.DiGraph, parameters: Optional[Dict[Any, Any]] = None):
     """
     Transforms a NetworkX DiGraph representing an OCEL to a proper OCEL.
 
     Parameters
     ----------------
     nx_graph
         NetworkX DiGraph
@@ -184,14 +188,16 @@
     ----------------
     ocel
         Object-centric event log
     """
     if parameters is None:
         parameters = {}
 
+    from pm4py.util import pandas_utils
+
     events = []
     objects = []
     relations = []
     o2o = []
     object_changes = []
 
     events_activity = {}
@@ -250,18 +256,20 @@
 
     del events["type"]
     del objects["type"]
 
     if object_changes is not None:
         del object_changes["type"]
 
+    from pm4py.objects.ocel.obj import OCEL
+
     return OCEL(events, objects, relations, o2o=o2o, object_changes=object_changes)
 
 
-def nx_to_event_log(nx_graph: nx.DiGraph, parameters: Optional[Dict[Any, Any]] = None) -> EventLog:
+def nx_to_event_log(nx_graph: nx.DiGraph, parameters: Optional[Dict[Any, Any]] = None):
     """
     Transforms a NetworkX DiGraph representing a traditional event log to a proper event log.
 
     Parameters
     ----------------
     nx_graph
         NetworkX DiGraph
@@ -272,14 +280,17 @@
     ----------------
     event_log
         Traditional event log.
     """
     if parameters is None:
         parameters = {}
 
+    from pm4py.objects.log.obj import EventLog, Trace, Event
+    from pm4py.objects.log.util import sorting
+
     log = EventLog()
 
     case_nodes = [(k, v["attr"]) for k, v in nx_graph.nodes.items() if v["attr"]["type"] == "CASE"]
     event_nodes = [(k, v["attr"]) for k, v in nx_graph.nodes.items() if v["attr"]["type"] == "EVENT"]
 
     cases = {}
     for i in range(len(case_nodes)):
```

### Comparing `pm4pyminimal-2.7.9.3/pm4py/util/pandas_utils.py` & `pm4pyminimal-2.7.9.4/pm4py/util/pandas_utils.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/util/points_subset.py` & `pm4pyminimal-2.7.9.4/pm4py/util/points_subset.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/util/regex.py` & `pm4pyminimal-2.7.9.4/pm4py/util/regex.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/util/string_distance.py` & `pm4pyminimal-2.7.9.4/pm4py/util/string_distance.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/util/typing.py` & `pm4pyminimal-2.7.9.4/pm4py/util/typing.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/util/variants_util.py` & `pm4pyminimal-2.7.9.4/pm4py/util/variants_util.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/util/vis_utils.py` & `pm4pyminimal-2.7.9.4/pm4py/util/vis_utils.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/util/xes_constants.py` & `pm4pyminimal-2.7.9.4/pm4py/util/xes_constants.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/utils.py` & `pm4pyminimal-2.7.9.4/pm4py/utils.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/vis.py` & `pm4pyminimal-2.7.9.4/pm4py/vis.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/visualization/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/visualization/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/visualization/align_table/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/visualization/align_table/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/visualization/align_table/variants/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/visualization/align_table/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/visualization/align_table/variants/classic.py` & `pm4pyminimal-2.7.9.4/pm4py/visualization/align_table/variants/classic.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/visualization/align_table/visualizer.py` & `pm4pyminimal-2.7.9.4/pm4py/visualization/align_table/visualizer.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/visualization/bpmn/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/visualization/bpmn/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/visualization/bpmn/variants/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/visualization/bpmn/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/visualization/bpmn/variants/classic.py` & `pm4pyminimal-2.7.9.4/pm4py/visualization/bpmn/variants/classic.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/visualization/bpmn/visualizer.py` & `pm4pyminimal-2.7.9.4/pm4py/visualization/bpmn/visualizer.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/visualization/common/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/visualization/common/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/visualization/common/dot_util.py` & `pm4pyminimal-2.7.9.4/pm4py/visualization/common/dot_util.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/visualization/common/gview.py` & `pm4pyminimal-2.7.9.4/pm4py/visualization/common/gview.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/visualization/common/html.py` & `pm4pyminimal-2.7.9.4/pm4py/visualization/common/html.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/visualization/common/save.py` & `pm4pyminimal-2.7.9.4/pm4py/visualization/common/save.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/visualization/common/svg_pos_parser.py` & `pm4pyminimal-2.7.9.4/pm4py/visualization/common/svg_pos_parser.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/visualization/common/utils.py` & `pm4pyminimal-2.7.9.4/pm4py/visualization/common/utils.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/visualization/common/visualizer.py` & `pm4pyminimal-2.7.9.4/pm4py/visualization/common/visualizer.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/visualization/decisiontree/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/visualization/decisiontree/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/visualization/decisiontree/util/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/visualization/decisiontree/util/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/visualization/decisiontree/util/dt_to_string.py` & `pm4pyminimal-2.7.9.4/pm4py/visualization/decisiontree/util/dt_to_string.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/visualization/decisiontree/variants/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/visualization/decisiontree/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/visualization/decisiontree/variants/classic.py` & `pm4pyminimal-2.7.9.4/pm4py/visualization/decisiontree/variants/classic.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/visualization/decisiontree/visualizer.py` & `pm4pyminimal-2.7.9.4/pm4py/visualization/decisiontree/visualizer.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/visualization/dfg/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/visualization/dfg/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/visualization/dfg/util/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/visualization/dfg/util/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/visualization/dfg/util/dfg_gviz.py` & `pm4pyminimal-2.7.9.4/pm4py/visualization/dfg/util/dfg_gviz.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/visualization/dfg/variants/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/visualization/dfg/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/visualization/dfg/variants/cost.py` & `pm4pyminimal-2.7.9.4/pm4py/visualization/dfg/variants/cost.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/visualization/dfg/variants/frequency.py` & `pm4pyminimal-2.7.9.4/pm4py/visualization/dfg/variants/frequency.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/visualization/dfg/variants/performance.py` & `pm4pyminimal-2.7.9.4/pm4py/visualization/dfg/variants/performance.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/visualization/dfg/variants/timeline.py` & `pm4pyminimal-2.7.9.4/pm4py/visualization/dfg/variants/timeline.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/visualization/dfg/visualizer.py` & `pm4pyminimal-2.7.9.4/pm4py/visualization/dfg/visualizer.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/visualization/dotted_chart/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/visualization/dotted_chart/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/visualization/dotted_chart/variants/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/visualization/dotted_chart/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/visualization/dotted_chart/variants/classic.py` & `pm4pyminimal-2.7.9.4/pm4py/visualization/dotted_chart/variants/classic.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/visualization/dotted_chart/visualizer.py` & `pm4pyminimal-2.7.9.4/pm4py/visualization/dotted_chart/visualizer.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/visualization/footprints/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/visualization/footprints/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/visualization/footprints/variants/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/visualization/footprints/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/visualization/footprints/variants/comparison.py` & `pm4pyminimal-2.7.9.4/pm4py/visualization/footprints/variants/comparison.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/visualization/footprints/variants/comparison_symmetric.py` & `pm4pyminimal-2.7.9.4/pm4py/visualization/footprints/variants/comparison_symmetric.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/visualization/footprints/variants/single.py` & `pm4pyminimal-2.7.9.4/pm4py/visualization/footprints/variants/single.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/visualization/footprints/visualizer.py` & `pm4pyminimal-2.7.9.4/pm4py/visualization/footprints/visualizer.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/visualization/graphs/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/visualization/graphs/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/visualization/graphs/util/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/visualization/graphs/util/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/visualization/graphs/util/common.py` & `pm4pyminimal-2.7.9.4/pm4py/visualization/graphs/util/common.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/visualization/graphs/variants/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/visualization/graphs/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/visualization/graphs/variants/attributes.py` & `pm4pyminimal-2.7.9.4/pm4py/visualization/graphs/variants/attributes.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/visualization/graphs/variants/barplot.py` & `pm4pyminimal-2.7.9.4/pm4py/visualization/graphs/variants/barplot.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/visualization/graphs/variants/cases.py` & `pm4pyminimal-2.7.9.4/pm4py/visualization/graphs/variants/cases.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/visualization/graphs/variants/dates.py` & `pm4pyminimal-2.7.9.4/pm4py/visualization/graphs/variants/dates.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/visualization/graphs/visualizer.py` & `pm4pyminimal-2.7.9.4/pm4py/visualization/graphs/visualizer.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/visualization/heuristics_net/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/visualization/heuristics_net/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/visualization/heuristics_net/variants/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/visualization/heuristics_net/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/visualization/heuristics_net/variants/pydotplus_vis.py` & `pm4pyminimal-2.7.9.4/pm4py/visualization/heuristics_net/variants/pydotplus_vis.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/visualization/heuristics_net/visualizer.py` & `pm4pyminimal-2.7.9.4/pm4py/visualization/heuristics_net/visualizer.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/visualization/network_analysis/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/visualization/network_analysis/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/visualization/network_analysis/variants/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/visualization/network_analysis/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/visualization/network_analysis/variants/frequency.py` & `pm4pyminimal-2.7.9.4/pm4py/visualization/network_analysis/variants/frequency.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/visualization/network_analysis/variants/performance.py` & `pm4pyminimal-2.7.9.4/pm4py/visualization/network_analysis/variants/performance.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/visualization/network_analysis/visualizer.py` & `pm4pyminimal-2.7.9.4/pm4py/visualization/network_analysis/visualizer.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/visualization/networkx/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/visualization/networkx/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/visualization/networkx/variants/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/visualization/networkx/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/visualization/networkx/variants/digraph.py` & `pm4pyminimal-2.7.9.4/pm4py/visualization/networkx/variants/digraph.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/visualization/networkx/visualizer.py` & `pm4pyminimal-2.7.9.4/pm4py/visualization/networkx/visualizer.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/visualization/ocel/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/visualization/ocel/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/visualization/ocel/eve_to_obj_types/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/visualization/ocel/eve_to_obj_types/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/visualization/ocel/eve_to_obj_types/variants/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/visualization/ocel/eve_to_obj_types/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/visualization/ocel/eve_to_obj_types/variants/graphviz.py` & `pm4pyminimal-2.7.9.4/pm4py/visualization/ocel/eve_to_obj_types/variants/graphviz.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/visualization/ocel/eve_to_obj_types/visualizer.py` & `pm4pyminimal-2.7.9.4/pm4py/visualization/ocel/eve_to_obj_types/visualizer.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/visualization/ocel/interleavings/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/visualization/ocel/interleavings/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/visualization/ocel/interleavings/variants/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/visualization/ocel/interleavings/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/visualization/ocel/interleavings/variants/graphviz.py` & `pm4pyminimal-2.7.9.4/pm4py/visualization/ocel/interleavings/variants/graphviz.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/visualization/ocel/interleavings/visualizer.py` & `pm4pyminimal-2.7.9.4/pm4py/visualization/ocel/interleavings/visualizer.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/visualization/ocel/object_graph/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/visualization/ocel/object_graph/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/visualization/ocel/object_graph/variants/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/visualization/ocel/object_graph/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/visualization/ocel/object_graph/variants/graphviz.py` & `pm4pyminimal-2.7.9.4/pm4py/visualization/ocel/object_graph/variants/graphviz.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/visualization/ocel/object_graph/visualizer.py` & `pm4pyminimal-2.7.9.4/pm4py/visualization/ocel/object_graph/visualizer.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/visualization/ocel/ocdfg/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/visualization/ocel/ocdfg/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/visualization/ocel/ocdfg/variants/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/visualization/ocel/ocdfg/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/visualization/ocel/ocdfg/variants/classic.py` & `pm4pyminimal-2.7.9.4/pm4py/visualization/ocel/ocdfg/variants/classic.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/visualization/ocel/ocdfg/visualizer.py` & `pm4pyminimal-2.7.9.4/pm4py/visualization/ocel/ocdfg/visualizer.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/visualization/ocel/ocpn/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/visualization/ocel/ocpn/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/visualization/ocel/ocpn/variants/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/visualization/ocel/ocpn/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/visualization/ocel/ocpn/variants/wo_decoration.py` & `pm4pyminimal-2.7.9.4/pm4py/visualization/ocel/ocpn/variants/wo_decoration.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/visualization/ocel/ocpn/visualizer.py` & `pm4pyminimal-2.7.9.4/pm4py/visualization/ocel/ocpn/visualizer.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/visualization/performance_spectrum/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/visualization/performance_spectrum/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/visualization/performance_spectrum/variants/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/visualization/performance_spectrum/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/visualization/performance_spectrum/variants/neato.py` & `pm4pyminimal-2.7.9.4/pm4py/visualization/performance_spectrum/variants/neato.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/visualization/performance_spectrum/visualizer.py` & `pm4pyminimal-2.7.9.4/pm4py/visualization/performance_spectrum/visualizer.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/visualization/petri_net/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/visualization/petri_net/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/visualization/petri_net/common/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/visualization/petri_net/common/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/visualization/petri_net/common/visualize.py` & `pm4pyminimal-2.7.9.4/pm4py/visualization/petri_net/common/visualize.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/visualization/petri_net/util/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/visualization/petri_net/util/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/visualization/petri_net/util/alignments_decoration.py` & `pm4pyminimal-2.7.9.4/pm4py/visualization/petri_net/util/alignments_decoration.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/visualization/petri_net/util/performance_map.py` & `pm4pyminimal-2.7.9.4/pm4py/visualization/petri_net/util/performance_map.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/visualization/petri_net/util/vis_trans_shortest_paths.py` & `pm4pyminimal-2.7.9.4/pm4py/visualization/petri_net/util/vis_trans_shortest_paths.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/visualization/petri_net/variants/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/visualization/petri_net/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/visualization/petri_net/variants/alignments.py` & `pm4pyminimal-2.7.9.4/pm4py/visualization/petri_net/variants/alignments.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/visualization/petri_net/variants/greedy_decoration_frequency.py` & `pm4pyminimal-2.7.9.4/pm4py/visualization/petri_net/variants/greedy_decoration_frequency.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/visualization/petri_net/variants/greedy_decoration_performance.py` & `pm4pyminimal-2.7.9.4/pm4py/visualization/petri_net/variants/greedy_decoration_performance.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/visualization/petri_net/variants/token_decoration_frequency.py` & `pm4pyminimal-2.7.9.4/pm4py/visualization/petri_net/variants/token_decoration_frequency.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/visualization/petri_net/variants/token_decoration_performance.py` & `pm4pyminimal-2.7.9.4/pm4py/visualization/petri_net/variants/token_decoration_performance.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/visualization/petri_net/variants/wo_decoration.py` & `pm4pyminimal-2.7.9.4/pm4py/visualization/petri_net/variants/wo_decoration.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/visualization/petri_net/visualizer.py` & `pm4pyminimal-2.7.9.4/pm4py/visualization/petri_net/visualizer.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/visualization/powl/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/visualization/powl/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/visualization/powl/variants/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/visualization/powl/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/visualization/powl/variants/basic.py` & `pm4pyminimal-2.7.9.4/pm4py/visualization/powl/variants/basic.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/visualization/powl/variants/end.png` & `pm4pyminimal-2.7.9.4/pm4py/visualization/powl/variants/end.png`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/visualization/powl/variants/loop.png` & `pm4pyminimal-2.7.9.4/pm4py/visualization/powl/variants/loop.png`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/visualization/powl/variants/net.py` & `pm4pyminimal-2.7.9.4/pm4py/visualization/powl/variants/net.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/visualization/powl/variants/play.png` & `pm4pyminimal-2.7.9.4/pm4py/visualization/powl/variants/play.png`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/visualization/powl/variants/xor.png` & `pm4pyminimal-2.7.9.4/pm4py/visualization/powl/variants/xor.png`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/visualization/powl/visualizer.py` & `pm4pyminimal-2.7.9.4/pm4py/visualization/powl/visualizer.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/visualization/process_tree/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/visualization/process_tree/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/visualization/process_tree/variants/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/visualization/process_tree/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/visualization/process_tree/variants/frequency_annotation.py` & `pm4pyminimal-2.7.9.4/pm4py/visualization/process_tree/variants/frequency_annotation.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/visualization/process_tree/variants/symbolic.py` & `pm4pyminimal-2.7.9.4/pm4py/visualization/process_tree/variants/symbolic.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/visualization/process_tree/variants/wo_decoration.py` & `pm4pyminimal-2.7.9.4/pm4py/visualization/process_tree/variants/wo_decoration.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/visualization/process_tree/visualizer.py` & `pm4pyminimal-2.7.9.4/pm4py/visualization/process_tree/visualizer.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/visualization/sna/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/visualization/sna/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/visualization/sna/variants/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/visualization/sna/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/visualization/sna/variants/networkx.py` & `pm4pyminimal-2.7.9.4/pm4py/visualization/sna/variants/networkx.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/visualization/sna/variants/pyvis.py` & `pm4pyminimal-2.7.9.4/pm4py/visualization/sna/variants/pyvis.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/visualization/sna/visualizer.py` & `pm4pyminimal-2.7.9.4/pm4py/visualization/sna/visualizer.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/visualization/transition_system/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/visualization/transition_system/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/visualization/transition_system/util/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/visualization/transition_system/util/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/visualization/transition_system/util/visualize_graphviz.py` & `pm4pyminimal-2.7.9.4/pm4py/visualization/transition_system/util/visualize_graphviz.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/visualization/transition_system/variants/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/visualization/transition_system/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/visualization/transition_system/variants/trans_frequency.py` & `pm4pyminimal-2.7.9.4/pm4py/visualization/transition_system/variants/trans_frequency.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/visualization/transition_system/variants/view_based.py` & `pm4pyminimal-2.7.9.4/pm4py/visualization/transition_system/variants/view_based.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/visualization/transition_system/visualizer.py` & `pm4pyminimal-2.7.9.4/pm4py/visualization/transition_system/visualizer.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/visualization/trie/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/visualization/trie/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/visualization/trie/variants/__init__.py` & `pm4pyminimal-2.7.9.4/pm4py/visualization/trie/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/visualization/trie/variants/classic.py` & `pm4pyminimal-2.7.9.4/pm4py/visualization/trie/variants/classic.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/visualization/trie/visualizer.py` & `pm4pyminimal-2.7.9.4/pm4py/visualization/trie/visualizer.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4py/write.py` & `pm4pyminimal-2.7.9.4/pm4py/write.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/pm4pyminimal.egg-info/PKG-INFO` & `pm4pyminimal-2.7.9.4/pm4pyminimal.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pm4pyminimal
-Version: 2.7.9.3
+Version: 2.7.9.4
 Summary: Process mining for Python
 Home-page: https://pm4py.fit.fraunhofer.de
 Author: Fraunhofer Institute for Applied Information Technology FIT
 Author-email: pm4py@fit.fraunhofer.de
 License: GPL 3.0
 Project-URL: Documentation, https://pm4py.fit.fraunhofer.de
 Project-URL: Source, https://github.com/pm4py/pm4py-source
@@ -68,7 +68,8 @@
 pages = {100556},  
 year = {2023},  
 issn = {2665-9638},  
 doi = {https://doi.org/10.1016/j.simpa.2023.100556},  
 url = {https://www.sciencedirect.com/science/article/pii/S2665963823000933},  
 author = {Alessandro Berti and Sebastiaan van Zelst and Daniel Schuster},  
 }
+
```

### Comparing `pm4pyminimal-2.7.9.3/pm4pyminimal.egg-info/SOURCES.txt` & `pm4pyminimal-2.7.9.4/pm4pyminimal.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/setup.py` & `pm4pyminimal-2.7.9.4/setup.py`

 * *Files identical despite different names*

### Comparing `pm4pyminimal-2.7.9.3/tests/test_cli.py` & `pm4pyminimal-2.7.9.4/tests/test_cli.py`

 * *Files identical despite different names*

