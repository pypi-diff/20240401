# Comparing `tmp/pm4py-2.7.9.3.tar.gz` & `tmp/pm4py-2.7.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pm4py-2.7.9.3.tar", last modified: Tue Jan 16 10:10:43 2024, max compression
+gzip compressed data, was "pm4py-2.7.9.4.tar", last modified: Mon Jan 29 06:14:26 2024, max compression
```

## Comparing `pm4py-2.7.9.3.tar` & `pm4py-2.7.9.4.tar`

### file list

```diff
@@ -1,1804 +1,1804 @@
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:43.360753 pm4py-2.7.9.3/
--rw-rw-rw-   0        0        0    34817 2023-12-11 09:33:50.000000 pm4py-2.7.9.3/LICENSE
--rw-rw-rw-   0        0        0       29 2024-01-04 13:34:19.000000 pm4py-2.7.9.3/MANIFEST.in
--rw-rw-rw-   0        0        0     3629 2024-01-16 10:10:43.358513 pm4py-2.7.9.3/PKG-INFO
--rw-rw-rw-   0        0        0     2790 2024-01-16 10:10:16.000000 pm4py-2.7.9.3/README.md
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:28.646172 pm4py-2.7.9.3/pm4py/
--rw-rw-rw-   0        0        0     7677 2024-01-16 10:09:19.000000 pm4py-2.7.9.3/pm4py/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:28.709890 pm4py-2.7.9.3/pm4py/algo/
--rw-rw-rw-   0        0        0      854 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:28.726949 pm4py-2.7.9.3/pm4py/algo/analysis/
--rw-rw-rw-   0        0        0      833 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/analysis/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:28.759843 pm4py-2.7.9.3/pm4py/algo/analysis/extended_marking_equation/
--rw-rw-rw-   0        0        0      802 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/analysis/extended_marking_equation/__init__.py
--rw-rw-rw-   0        0        0     3588 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/analysis/extended_marking_equation/algorithm.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:28.793864 pm4py-2.7.9.3/pm4py/algo/analysis/extended_marking_equation/variants/
--rw-rw-rw-   0        0        0      810 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/analysis/extended_marking_equation/variants/__init__.py
--rw-rw-rw-   0        0        0    21448 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/analysis/extended_marking_equation/variants/classic.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:28.822154 pm4py-2.7.9.3/pm4py/algo/analysis/marking_equation/
--rw-rw-rw-   0        0        0      794 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/analysis/marking_equation/__init__.py
--rw-rw-rw-   0        0        0     2689 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/analysis/marking_equation/algorithm.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:28.850923 pm4py-2.7.9.3/pm4py/algo/analysis/marking_equation/variants/
--rw-rw-rw-   0        0        0      801 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/analysis/marking_equation/variants/__init__.py
--rw-rw-rw-   0        0        0    11636 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/analysis/marking_equation/variants/classic.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:28.880196 pm4py-2.7.9.3/pm4py/algo/analysis/woflan/
--rw-rw-rw-   0        0        0      836 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/analysis/woflan/__init__.py
--rw-rw-rw-   0        0        0    32308 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/analysis/woflan/algorithm.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:28.913312 pm4py-2.7.9.3/pm4py/algo/analysis/woflan/graphs/
--rw-rw-rw-   0        0        0      868 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/analysis/woflan/graphs/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:28.943560 pm4py-2.7.9.3/pm4py/algo/analysis/woflan/graphs/minimal_coverability_graph/
--rw-rw-rw-   0        0        0      835 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/analysis/woflan/graphs/minimal_coverability_graph/__init__.py
--rw-rw-rw-   0        0        0     7988 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/analysis/woflan/graphs/minimal_coverability_graph/minimal_coverability_graph.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:28.972805 pm4py-2.7.9.3/pm4py/algo/analysis/woflan/graphs/reachability_graph/
--rw-rw-rw-   0        0        0      819 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/analysis/woflan/graphs/reachability_graph/__init__.py
--rw-rw-rw-   0        0        0     2451 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/analysis/woflan/graphs/reachability_graph/reachability_graph.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:29.002817 pm4py-2.7.9.3/pm4py/algo/analysis/woflan/graphs/restricted_coverability_graph/
--rw-rw-rw-   0        0        0      841 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/analysis/woflan/graphs/restricted_coverability_graph/__init__.py
--rw-rw-rw-   0        0        0     4061 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/analysis/woflan/graphs/restricted_coverability_graph/restricted_coverability_graph.py
--rw-rw-rw-   0        0        0     5745 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/analysis/woflan/graphs/utility.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:29.030272 pm4py-2.7.9.3/pm4py/algo/analysis/woflan/not_well_handled_pairs/
--rw-rw-rw-   0        0        0      820 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/analysis/woflan/not_well_handled_pairs/__init__.py
--rw-rw-rw-   0        0        0     2632 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/analysis/woflan/not_well_handled_pairs/not_well_handled_pairs.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:29.085675 pm4py-2.7.9.3/pm4py/algo/analysis/woflan/place_invariants/
--rw-rw-rw-   0        0        0      849 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/analysis/woflan/place_invariants/__init__.py
--rw-rw-rw-   0        0        0     4300 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/analysis/woflan/place_invariants/place_invariants.py
--rw-rw-rw-   0        0        0     3668 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/analysis/woflan/place_invariants/s_component.py
--rw-rw-rw-   0        0        0     1098 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/analysis/woflan/place_invariants/uniform_invariant.py
--rw-rw-rw-   0        0        0     8333 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/analysis/woflan/place_invariants/utility.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:29.108707 pm4py-2.7.9.3/pm4py/algo/analysis/workflow_net/
--rw-rw-rw-   0        0        0      800 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/analysis/workflow_net/__init__.py
--rw-rw-rw-   0        0        0     1542 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/analysis/workflow_net/algorithm.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:29.129307 pm4py-2.7.9.3/pm4py/algo/analysis/workflow_net/variants/
--rw-rw-rw-   0        0        0      799 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/analysis/workflow_net/variants/__init__.py
--rw-rw-rw-   0        0        0     3243 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/analysis/workflow_net/variants/petri_net.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:29.142790 pm4py-2.7.9.3/pm4py/algo/anonymization/
--rw-rw-rw-   0        0        0      979 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/anonymization/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:29.164920 pm4py-2.7.9.3/pm4py/algo/anonymization/pripel/
--rw-rw-rw-   0        0        0      807 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/anonymization/pripel/__init__.py
--rw-rw-rw-   0        0        0     3170 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/anonymization/pripel/algorithm.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:29.211542 pm4py-2.7.9.3/pm4py/algo/anonymization/pripel/util/
--rw-rw-rw-   0        0        0    13889 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/anonymization/pripel/util/AttributeAnonymizer.py
--rw-rw-rw-   0        0        0    14468 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/anonymization/pripel/util/TraceMatcher.py
--rw-rw-rw-   0        0        0      837 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/anonymization/pripel/util/__init__.py
--rw-rw-rw-   0        0        0     1754 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/anonymization/pripel/util/trace_levenshtein.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:29.236153 pm4py-2.7.9.3/pm4py/algo/anonymization/pripel/variants/
--rw-rw-rw-   0        0        0      797 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/anonymization/pripel/variants/__init__.py
--rw-rw-rw-   0        0        0     5291 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/anonymization/pripel/variants/pripel.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:29.263864 pm4py-2.7.9.3/pm4py/algo/anonymization/trace_variant_query/
--rw-rw-rw-   0        0        0      820 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/anonymization/trace_variant_query/__init__.py
--rw-rw-rw-   0        0        0     3980 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/anonymization/trace_variant_query/algorithm.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:29.335520 pm4py-2.7.9.3/pm4py/algo/anonymization/trace_variant_query/util/
--rw-rw-rw-   0        0        0      839 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/anonymization/trace_variant_query/util/__init__.py
--rw-rw-rw-   0        0        0     6862 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/anonymization/trace_variant_query/util/behavioralAppropriateness.py
--rw-rw-rw-   0        0        0     1323 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/anonymization/trace_variant_query/util/exp_mech.py
--rw-rw-rw-   0        0        0     1687 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/anonymization/trace_variant_query/util/util.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:29.398931 pm4py-2.7.9.3/pm4py/algo/anonymization/trace_variant_query/variants/
--rw-rw-rw-   0        0        0      817 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/anonymization/trace_variant_query/variants/__init__.py
--rw-rw-rw-   0        0        0     7691 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/anonymization/trace_variant_query/variants/laplace.py
--rw-rw-rw-   0        0        0    11329 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/anonymization/trace_variant_query/variants/sacofa.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:29.414009 pm4py-2.7.9.3/pm4py/algo/clustering/
--rw-rw-rw-   0        0        0      734 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/clustering/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:29.444237 pm4py-2.7.9.3/pm4py/algo/clustering/profiles/
--rw-rw-rw-   0        0        0      798 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/clustering/profiles/__init__.py
--rw-rw-rw-   0        0        0     2118 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/clustering/profiles/algorithm.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:29.467681 pm4py-2.7.9.3/pm4py/algo/clustering/profiles/variants/
--rw-rw-rw-   0        0        0      804 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/clustering/profiles/variants/__init__.py
--rw-rw-rw-   0        0        0     3544 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/clustering/profiles/variants/sklearn_profiles.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:29.492260 pm4py-2.7.9.3/pm4py/algo/clustering/trace_attribute_driven/
--rw-rw-rw-   0        0        0     1060 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/clustering/trace_attribute_driven/__init__.py
--rw-rw-rw-   0        0        0     4705 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/clustering/trace_attribute_driven/algorithm.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:29.516749 pm4py-2.7.9.3/pm4py/algo/clustering/trace_attribute_driven/dfg/
--rw-rw-rw-   0        0        0      805 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/clustering/trace_attribute_driven/dfg/__init__.py
--rw-rw-rw-   0        0        0     3989 2024-01-02 13:29:21.000000 pm4py-2.7.9.3/pm4py/algo/clustering/trace_attribute_driven/dfg/dfg_dist.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:29.543165 pm4py-2.7.9.3/pm4py/algo/clustering/trace_attribute_driven/leven_dist/
--rw-rw-rw-   0        0        0      819 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/clustering/trace_attribute_driven/leven_dist/__init__.py
--rw-rw-rw-   0        0        0     5473 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/clustering/trace_attribute_driven/leven_dist/leven_dist_calc.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:29.566985 pm4py-2.7.9.3/pm4py/algo/clustering/trace_attribute_driven/linkage_method/
--rw-rw-rw-   0        0        0      819 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/clustering/trace_attribute_driven/linkage_method/__init__.py
--rw-rw-rw-   0        0        0    13583 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/clustering/trace_attribute_driven/linkage_method/linkage_avg.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:29.589400 pm4py-2.7.9.3/pm4py/algo/clustering/trace_attribute_driven/merge_log/
--rw-rw-rw-   0        0        0      812 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/clustering/trace_attribute_driven/merge_log/__init__.py
--rw-rw-rw-   0        0        0     4290 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/clustering/trace_attribute_driven/merge_log/merge_log.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:29.624440 pm4py-2.7.9.3/pm4py/algo/clustering/trace_attribute_driven/util/
--rw-rw-rw-   0        0        0      824 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/clustering/trace_attribute_driven/util/__init__.py
--rw-rw-rw-   0        0        0     3396 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/clustering/trace_attribute_driven/util/evaluation.py
--rw-rw-rw-   0        0        0    15776 2024-01-02 13:29:21.000000 pm4py-2.7.9.3/pm4py/algo/clustering/trace_attribute_driven/util/filter_subsets.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:29.679914 pm4py-2.7.9.3/pm4py/algo/clustering/trace_attribute_driven/variants/
--rw-rw-rw-   0        0        0      855 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/clustering/trace_attribute_driven/variants/__init__.py
--rw-rw-rw-   0        0        0    18463 2024-01-02 13:29:21.000000 pm4py-2.7.9.3/pm4py/algo/clustering/trace_attribute_driven/variants/act_dist_calc.py
--rw-rw-rw-   0        0        0     6806 2024-01-02 13:29:21.000000 pm4py-2.7.9.3/pm4py/algo/clustering/trace_attribute_driven/variants/logslice_dist.py
--rw-rw-rw-   0        0        0     6329 2024-01-02 13:29:21.000000 pm4py-2.7.9.3/pm4py/algo/clustering/trace_attribute_driven/variants/sim_calc.py
--rw-rw-rw-   0        0        0    15790 2024-01-02 13:29:21.000000 pm4py-2.7.9.3/pm4py/algo/clustering/trace_attribute_driven/variants/suc_dist_calc.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:29.692079 pm4py-2.7.9.3/pm4py/algo/comparison/
--rw-rw-rw-   0        0        0      851 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/comparison/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:29.717462 pm4py-2.7.9.3/pm4py/algo/comparison/petrinet/
--rw-rw-rw-   0        0        0      803 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/comparison/petrinet/__init__.py
--rw-rw-rw-   0        0        0     6719 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/comparison/petrinet/element_usage_comparison.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:29.730237 pm4py-2.7.9.3/pm4py/algo/conformance/
--rw-rw-rw-   0        0        0      946 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/conformance/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:29.742072 pm4py-2.7.9.3/pm4py/algo/conformance/alignments/
--rw-rw-rw-   0        0        0      822 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/conformance/alignments/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:29.764543 pm4py-2.7.9.3/pm4py/algo/conformance/alignments/decomposed/
--rw-rw-rw-   0        0        0      812 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/conformance/alignments/decomposed/__init__.py
--rw-rw-rw-   0        0        0     2018 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/conformance/alignments/decomposed/algorithm.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:29.788253 pm4py-2.7.9.3/pm4py/algo/conformance/alignments/decomposed/variants/
--rw-rw-rw-   0        0        0      818 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/conformance/alignments/decomposed/variants/__init__.py
--rw-rw-rw-   0        0        0    19051 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/conformance/alignments/decomposed/variants/recompos_maximal.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:29.813183 pm4py-2.7.9.3/pm4py/algo/conformance/alignments/dfg/
--rw-rw-rw-   0        0        0      805 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/conformance/alignments/dfg/__init__.py
--rw-rw-rw-   0        0        0     1956 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/conformance/alignments/dfg/algorithm.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:29.836937 pm4py-2.7.9.3/pm4py/algo/conformance/alignments/dfg/variants/
--rw-rw-rw-   0        0        0      802 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/conformance/alignments/dfg/variants/__init__.py
--rw-rw-rw-   0        0        0    24120 2024-01-15 12:00:43.000000 pm4py-2.7.9.3/pm4py/algo/conformance/alignments/dfg/variants/classic.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:29.859941 pm4py-2.7.9.3/pm4py/algo/conformance/alignments/edit_distance/
--rw-rw-rw-   0        0        0      815 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/conformance/alignments/edit_distance/__init__.py
--rw-rw-rw-   0        0        0     1876 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/conformance/alignments/edit_distance/algorithm.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:29.882525 pm4py-2.7.9.3/pm4py/algo/conformance/alignments/edit_distance/variants/
--rw-rw-rw-   0        0        0      818 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/conformance/alignments/edit_distance/variants/__init__.py
--rw-rw-rw-   0        0        0    11234 2024-01-02 13:29:21.000000 pm4py-2.7.9.3/pm4py/algo/conformance/alignments/edit_distance/variants/edit_distance.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:29.907299 pm4py-2.7.9.3/pm4py/algo/conformance/alignments/petri_net/
--rw-rw-rw-   0        0        0      818 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/conformance/alignments/petri_net/__init__.py
--rw-rw-rw-   0        0        0    16964 2024-01-15 12:00:43.000000 pm4py-2.7.9.3/pm4py/algo/conformance/alignments/petri_net/algorithm.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:29.932606 pm4py-2.7.9.3/pm4py/algo/conformance/alignments/petri_net/utils/
--rw-rw-rw-   0        0        0      812 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/conformance/alignments/petri_net/utils/__init__.py
--rw-rw-rw-   0        0        0     2896 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/conformance/alignments/petri_net/utils/log_enrichment.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:30.037181 pm4py-2.7.9.3/pm4py/algo/conformance/alignments/petri_net/variants/
--rw-rw-rw-   0        0        0      925 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/conformance/alignments/petri_net/variants/__init__.py
--rw-rw-rw-   0        0        0    27553 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/conformance/alignments/petri_net/variants/dijkstra_less_memory.py
--rw-rw-rw-   0        0        0    17167 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/conformance/alignments/petri_net/variants/dijkstra_no_heuristics.py
--rw-rw-rw-   0        0        0    23651 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/conformance/alignments/petri_net/variants/discounted_a_star.py
--rw-rw-rw-   0        0        0    23429 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/conformance/alignments/petri_net/variants/generator_dijkstra_less_memory.py
--rw-rw-rw-   0        0        0    17357 2024-01-02 13:29:21.000000 pm4py-2.7.9.3/pm4py/algo/conformance/alignments/petri_net/variants/generator_dijkstra_no_heuristics.py
--rw-rw-rw-   0        0        0    23978 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/conformance/alignments/petri_net/variants/state_equation_a_star.py
--rw-rw-rw-   0        0        0    27872 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/conformance/alignments/petri_net/variants/tweaked_state_equation_a_star.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:30.060173 pm4py-2.7.9.3/pm4py/algo/conformance/alignments/process_tree/
--rw-rw-rw-   0        0        0      820 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/conformance/alignments/process_tree/__init__.py
--rw-rw-rw-   0        0        0     2203 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/conformance/alignments/process_tree/algorithm.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:30.094684 pm4py-2.7.9.3/pm4py/algo/conformance/alignments/process_tree/util/
--rw-rw-rw-   0        0        0      870 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/conformance/alignments/process_tree/util/__init__.py
--rw-rw-rw-   0        0        0     3355 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/conformance/alignments/process_tree/util/search_graph_pt_frequency_annotation.py
--rw-rw-rw-   0        0        0    15712 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/conformance/alignments/process_tree/util/search_graph_pt_replay_semantics.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:30.116902 pm4py-2.7.9.3/pm4py/algo/conformance/alignments/process_tree/variants/
--rw-rw-rw-   0        0        0      833 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/conformance/alignments/process_tree/variants/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:30.176948 pm4py-2.7.9.3/pm4py/algo/conformance/alignments/process_tree/variants/approximated/
--rw-rw-rw-   0        0        0      871 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/conformance/alignments/process_tree/variants/approximated/__init__.py
--rw-rw-rw-   0        0        0     5361 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/conformance/alignments/process_tree/variants/approximated/calculate_a_sa_ea_sets.py
--rw-rw-rw-   0        0        0    49808 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/conformance/alignments/process_tree/variants/approximated/matrix_lp.py
--rw-rw-rw-   0        0        0    36425 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/conformance/alignments/process_tree/variants/approximated/original.py
--rw-rw-rw-   0        0        0     6660 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/conformance/alignments/process_tree/variants/approximated/utilities.py
--rw-rw-rw-   0        0        0    17939 2024-01-15 12:00:43.000000 pm4py-2.7.9.3/pm4py/algo/conformance/alignments/process_tree/variants/search_graph_pt.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:30.200338 pm4py-2.7.9.3/pm4py/algo/conformance/antialignments/
--rw-rw-rw-   0        0        0      805 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/conformance/antialignments/__init__.py
--rw-rw-rw-   0        0        0     3166 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/conformance/antialignments/algorithm.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:30.225130 pm4py-2.7.9.3/pm4py/algo/conformance/antialignments/variants/
--rw-rw-rw-   0        0        0      812 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/conformance/antialignments/variants/__init__.py
--rw-rw-rw-   0        0        0     7582 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/conformance/antialignments/variants/discounted_a_star.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:30.246925 pm4py-2.7.9.3/pm4py/algo/conformance/declare/
--rw-rw-rw-   0        0        0      800 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/conformance/declare/__init__.py
--rw-rw-rw-   0        0        0     2733 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/conformance/declare/algorithm.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:30.270578 pm4py-2.7.9.3/pm4py/algo/conformance/declare/variants/
--rw-rw-rw-   0        0        0      797 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/conformance/declare/variants/__init__.py
--rw-rw-rw-   0        0        0    18351 2024-01-02 13:29:21.000000 pm4py-2.7.9.3/pm4py/algo/conformance/declare/variants/classic.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:30.292805 pm4py-2.7.9.3/pm4py/algo/conformance/footprints/
--rw-rw-rw-   0        0        0      807 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/conformance/footprints/__init__.py
--rw-rw-rw-   0        0        0     2061 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/conformance/footprints/algorithm.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:30.326989 pm4py-2.7.9.3/pm4py/algo/conformance/footprints/util/
--rw-rw-rw-   0        0        0      817 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/conformance/footprints/util/__init__.py
--rw-rw-rw-   0        0        0     6154 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/conformance/footprints/util/evaluation.py
--rw-rw-rw-   0        0        0     3573 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/conformance/footprints/util/tree_visualization.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:30.370037 pm4py-2.7.9.3/pm4py/algo/conformance/footprints/variants/
--rw-rw-rw-   0        0        0      832 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/conformance/footprints/variants/__init__.py
--rw-rw-rw-   0        0        0     3708 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/conformance/footprints/variants/log_extensive.py
--rw-rw-rw-   0        0        0     5119 2024-01-02 13:29:21.000000 pm4py-2.7.9.3/pm4py/algo/conformance/footprints/variants/log_model.py
--rw-rw-rw-   0        0        0     7141 2024-01-02 13:29:21.000000 pm4py-2.7.9.3/pm4py/algo/conformance/footprints/variants/trace_extensive.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:30.393988 pm4py-2.7.9.3/pm4py/algo/conformance/log_skeleton/
--rw-rw-rw-   0        0        0      803 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/conformance/log_skeleton/__init__.py
--rw-rw-rw-   0        0        0     4040 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/conformance/log_skeleton/algorithm.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:30.415413 pm4py-2.7.9.3/pm4py/algo/conformance/log_skeleton/variants/
--rw-rw-rw-   0        0        0      800 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/conformance/log_skeleton/variants/__init__.py
--rw-rw-rw-   0        0        0    13160 2024-01-15 12:00:43.000000 pm4py-2.7.9.3/pm4py/algo/conformance/log_skeleton/variants/classic.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:30.438867 pm4py-2.7.9.3/pm4py/algo/conformance/multialignments/
--rw-rw-rw-   0        0        0      806 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/conformance/multialignments/__init__.py
--rw-rw-rw-   0        0        0     3143 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/conformance/multialignments/algorithm.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:30.462680 pm4py-2.7.9.3/pm4py/algo/conformance/multialignments/variants/
--rw-rw-rw-   0        0        0      813 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/conformance/multialignments/variants/__init__.py
--rw-rw-rw-   0        0        0     6557 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/conformance/multialignments/variants/discounted_a_star.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:30.484951 pm4py-2.7.9.3/pm4py/algo/conformance/temporal_profile/
--rw-rw-rw-   0        0        0      807 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/conformance/temporal_profile/__init__.py
--rw-rw-rw-   0        0        0     4738 2024-01-02 13:29:21.000000 pm4py-2.7.9.3/pm4py/algo/conformance/temporal_profile/algorithm.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:30.518243 pm4py-2.7.9.3/pm4py/algo/conformance/temporal_profile/variants/
--rw-rw-rw-   0        0        0      811 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/conformance/temporal_profile/variants/__init__.py
--rw-rw-rw-   0        0        0     5476 2024-01-02 13:29:21.000000 pm4py-2.7.9.3/pm4py/algo/conformance/temporal_profile/variants/dataframe.py
--rw-rw-rw-   0        0        0     5957 2024-01-02 13:29:21.000000 pm4py-2.7.9.3/pm4py/algo/conformance/temporal_profile/variants/log.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:30.542048 pm4py-2.7.9.3/pm4py/algo/conformance/tokenreplay/
--rw-rw-rw-   0        0        0      815 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/conformance/tokenreplay/__init__.py
--rw-rw-rw-   0        0        0     2965 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/conformance/tokenreplay/algorithm.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:30.576802 pm4py-2.7.9.3/pm4py/algo/conformance/tokenreplay/diagnostics/
--rw-rw-rw-   0        0        0      836 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/conformance/tokenreplay/diagnostics/__init__.py
--rw-rw-rw-   0        0        0     6720 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/conformance/tokenreplay/diagnostics/duration_diagnostics.py
--rw-rw-rw-   0        0        0    11104 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/conformance/tokenreplay/diagnostics/root_cause_analysis.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:30.612897 pm4py-2.7.9.3/pm4py/algo/conformance/tokenreplay/variants/
--rw-rw-rw-   0        0        0      804 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/conformance/tokenreplay/variants/__init__.py
--rw-rw-rw-   0        0        0    12130 2024-01-02 13:29:21.000000 pm4py-2.7.9.3/pm4py/algo/conformance/tokenreplay/variants/backwards.py
--rw-rw-rw-   0        0        0    59022 2024-01-15 12:00:43.000000 pm4py-2.7.9.3/pm4py/algo/conformance/tokenreplay/variants/token_replay.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:30.637406 pm4py-2.7.9.3/pm4py/algo/connectors/
--rw-rw-rw-   0        0        0      786 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/connectors/__init__.py
--rw-rw-rw-   0        0        0     2768 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/connectors/algorithm.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:30.661662 pm4py-2.7.9.3/pm4py/algo/connectors/util/
--rw-rw-rw-   0        0        0      781 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/connectors/util/__init__.py
--rw-rw-rw-   0        0        0     1628 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/connectors/util/mail.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:30.793271 pm4py-2.7.9.3/pm4py/algo/connectors/variants/
--rw-rw-rw-   0        0        0      736 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/connectors/variants/__init__.py
--rw-rw-rw-   0        0        0     2592 2024-01-02 13:29:21.000000 pm4py-2.7.9.3/pm4py/algo/connectors/variants/camunda_workflow.py
--rw-rw-rw-   0        0        0     3743 2024-01-02 13:29:21.000000 pm4py-2.7.9.3/pm4py/algo/connectors/variants/chrome_history.py
--rw-rw-rw-   0        0        0     3777 2024-01-02 13:29:21.000000 pm4py-2.7.9.3/pm4py/algo/connectors/variants/firefox_history.py
--rw-rw-rw-   0        0        0     5250 2024-01-02 13:29:21.000000 pm4py-2.7.9.3/pm4py/algo/connectors/variants/github_repo.py
--rw-rw-rw-   0        0        0     4432 2024-01-02 13:29:21.000000 pm4py-2.7.9.3/pm4py/algo/connectors/variants/outlook_calendar.py
--rw-rw-rw-   0        0        0     4568 2024-01-02 13:29:21.000000 pm4py-2.7.9.3/pm4py/algo/connectors/variants/outlook_mail_extractor.py
--rw-rw-rw-   0        0        0     3168 2024-01-02 13:29:21.000000 pm4py-2.7.9.3/pm4py/algo/connectors/variants/sap_accounting.py
--rw-rw-rw-   0        0        0     4012 2024-01-02 13:29:21.000000 pm4py-2.7.9.3/pm4py/algo/connectors/variants/sap_o2c.py
--rw-rw-rw-   0        0        0     4243 2024-01-02 13:29:21.000000 pm4py-2.7.9.3/pm4py/algo/connectors/variants/windows_events.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:30.817882 pm4py-2.7.9.3/pm4py/algo/decision_mining/
--rw-rw-rw-   0        0        0      964 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/decision_mining/__init__.py
--rw-rw-rw-   0        0        0    23509 2024-01-02 13:29:21.000000 pm4py-2.7.9.3/pm4py/algo/decision_mining/algorithm.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:30.833099 pm4py-2.7.9.3/pm4py/algo/discovery/
--rw-rw-rw-   0        0        0      945 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/discovery/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:30.859635 pm4py-2.7.9.3/pm4py/algo/discovery/alpha/
--rw-rw-rw-   0        0        0      818 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/discovery/alpha/__init__.py
--rw-rw-rw-   0        0        0     5066 2024-01-02 13:29:21.000000 pm4py-2.7.9.3/pm4py/algo/discovery/alpha/algorithm.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:30.883163 pm4py-2.7.9.3/pm4py/algo/discovery/alpha/data_structures/
--rw-rw-rw-   0        0        0      816 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/discovery/alpha/data_structures/__init__.py
--rw-rw-rw-   0        0        0     2420 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/discovery/alpha/data_structures/alpha_classic_abstraction.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:30.907176 pm4py-2.7.9.3/pm4py/algo/discovery/alpha/utils/
--rw-rw-rw-   0        0        0      790 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/discovery/alpha/utils/__init__.py
--rw-rw-rw-   0        0        0     1622 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/discovery/alpha/utils/endpoints.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:30.940896 pm4py-2.7.9.3/pm4py/algo/discovery/alpha/variants/
--rw-rw-rw-   0        0        0      797 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/discovery/alpha/variants/__init__.py
--rw-rw-rw-   0        0        0    10830 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/discovery/alpha/variants/classic.py
--rw-rw-rw-   0        0        0    22005 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/discovery/alpha/variants/plus.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:30.964723 pm4py-2.7.9.3/pm4py/algo/discovery/batches/
--rw-rw-rw-   0        0        0      803 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/discovery/batches/__init__.py
--rw-rw-rw-   0        0        0     3756 2024-01-02 13:29:21.000000 pm4py-2.7.9.3/pm4py/algo/discovery/batches/algorithm.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:30.989383 pm4py-2.7.9.3/pm4py/algo/discovery/batches/utils/
--rw-rw-rw-   0        0        0      792 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/discovery/batches/utils/__init__.py
--rw-rw-rw-   0        0        0     9636 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/discovery/batches/utils/detection.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:31.024162 pm4py-2.7.9.3/pm4py/algo/discovery/batches/variants/
--rw-rw-rw-   0        0        0      797 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/discovery/batches/variants/__init__.py
--rw-rw-rw-   0        0        0     5216 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/discovery/batches/variants/log.py
--rw-rw-rw-   0        0        0     6427 2024-01-15 12:00:43.000000 pm4py-2.7.9.3/pm4py/algo/discovery/batches/variants/pandas.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:31.046644 pm4py-2.7.9.3/pm4py/algo/discovery/causal/
--rw-rw-rw-   0        0        0      795 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/discovery/causal/__init__.py
--rw-rw-rw-   0        0        0     1646 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/discovery/causal/algorithm.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:31.084014 pm4py-2.7.9.3/pm4py/algo/discovery/causal/variants/
--rw-rw-rw-   0        0        0      801 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/discovery/causal/variants/__init__.py
--rw-rw-rw-   0        0        0     1787 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/discovery/causal/variants/alpha.py
--rw-rw-rw-   0        0        0     1589 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/discovery/causal/variants/heuristic.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:31.116511 pm4py-2.7.9.3/pm4py/algo/discovery/correlation_mining/
--rw-rw-rw-   0        0        0      813 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/discovery/correlation_mining/__init__.py
--rw-rw-rw-   0        0        0     2249 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/discovery/correlation_mining/algorithm.py
--rw-rw-rw-   0        0        0     7934 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/discovery/correlation_mining/util.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:31.163357 pm4py-2.7.9.3/pm4py/algo/discovery/correlation_mining/variants/
--rw-rw-rw-   0        0        0      832 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/discovery/correlation_mining/variants/__init__.py
--rw-rw-rw-   0        0        0     9663 2024-01-02 13:29:21.000000 pm4py-2.7.9.3/pm4py/algo/discovery/correlation_mining/variants/classic.py
--rw-rw-rw-   0        0        0     4405 2024-01-15 12:00:43.000000 pm4py-2.7.9.3/pm4py/algo/discovery/correlation_mining/variants/classic_split.py
--rw-rw-rw-   0        0        0    10288 2024-01-02 13:29:21.000000 pm4py-2.7.9.3/pm4py/algo/discovery/correlation_mining/variants/trace_based.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:31.199550 pm4py-2.7.9.3/pm4py/algo/discovery/declare/
--rw-rw-rw-   0        0        0      798 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/discovery/declare/__init__.py
--rw-rw-rw-   0        0        0     1725 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/discovery/declare/algorithm.py
--rw-rw-rw-   0        0        0     1290 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/discovery/declare/templates.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:31.221957 pm4py-2.7.9.3/pm4py/algo/discovery/declare/variants/
--rw-rw-rw-   0        0        0      795 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/discovery/declare/variants/__init__.py
--rw-rw-rw-   0        0        0    30263 2024-01-15 12:00:43.000000 pm4py-2.7.9.3/pm4py/algo/discovery/declare/variants/classic.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:31.255951 pm4py-2.7.9.3/pm4py/algo/discovery/dfg/
--rw-rw-rw-   0        0        0      822 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/discovery/dfg/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:31.266963 pm4py-2.7.9.3/pm4py/algo/discovery/dfg/adapters/
--rw-rw-rw-   0        0        0      788 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/discovery/dfg/adapters/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:31.302575 pm4py-2.7.9.3/pm4py/algo/discovery/dfg/adapters/pandas/
--rw-rw-rw-   0        0        0      816 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/discovery/dfg/adapters/pandas/__init__.py
--rw-rw-rw-   0        0        0    15047 2024-01-15 12:00:43.000000 pm4py-2.7.9.3/pm4py/algo/discovery/dfg/adapters/pandas/df_statistics.py
--rw-rw-rw-   0        0        0     2962 2024-01-02 13:29:21.000000 pm4py-2.7.9.3/pm4py/algo/discovery/dfg/adapters/pandas/freq_triples.py
--rw-rw-rw-   0        0        0     4898 2024-01-02 13:29:21.000000 pm4py-2.7.9.3/pm4py/algo/discovery/dfg/algorithm.py
--rw-rw-rw-   0        0        0     1260 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/discovery/dfg/replacement.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:31.327594 pm4py-2.7.9.3/pm4py/algo/discovery/dfg/utils/
--rw-rw-rw-   0        0        0      788 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/discovery/dfg/utils/__init__.py
--rw-rw-rw-   0        0        0      783 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/discovery/dfg/utils/dfg_utils.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:31.411946 pm4py-2.7.9.3/pm4py/algo/discovery/dfg/variants/
--rw-rw-rw-   0        0        0      968 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/discovery/dfg/variants/__init__.py
--rw-rw-rw-   0        0        0     4609 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/discovery/dfg/variants/case_attributes.py
--rw-rw-rw-   0        0        0     2852 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/discovery/dfg/variants/clean.py
--rw-rw-rw-   0        0        0     2795 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/discovery/dfg/variants/clean_polars.py
--rw-rw-rw-   0        0        0     3347 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/discovery/dfg/variants/clean_time.py
--rw-rw-rw-   0        0        0     2200 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/discovery/dfg/variants/freq_triples.py
--rw-rw-rw-   0        0        0     2574 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/discovery/dfg/variants/native.py
--rw-rw-rw-   0        0        0     5794 2024-01-02 13:29:21.000000 pm4py-2.7.9.3/pm4py/algo/discovery/dfg/variants/performance.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:31.434375 pm4py-2.7.9.3/pm4py/algo/discovery/footprints/
--rw-rw-rw-   0        0        0      812 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/discovery/footprints/__init__.py
--rw-rw-rw-   0        0        0     3131 2024-01-02 13:29:21.000000 pm4py-2.7.9.3/pm4py/algo/discovery/footprints/algorithm.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:31.446323 pm4py-2.7.9.3/pm4py/algo/discovery/footprints/dfg/
--rw-rw-rw-   0        0        0      792 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/discovery/footprints/dfg/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:31.467482 pm4py-2.7.9.3/pm4py/algo/discovery/footprints/dfg/variants/
--rw-rw-rw-   0        0        0      796 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/discovery/footprints/dfg/variants/__init__.py
--rw-rw-rw-   0        0        0     2258 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/discovery/footprints/dfg/variants/dfg.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:31.479351 pm4py-2.7.9.3/pm4py/algo/discovery/footprints/log/
--rw-rw-rw-   0        0        0      792 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/discovery/footprints/log/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:31.523252 pm4py-2.7.9.3/pm4py/algo/discovery/footprints/log/variants/
--rw-rw-rw-   0        0        0      843 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/discovery/footprints/log/variants/__init__.py
--rw-rw-rw-   0        0        0     4664 2024-01-02 13:29:21.000000 pm4py-2.7.9.3/pm4py/algo/discovery/footprints/log/variants/entire_dataframe.py
--rw-rw-rw-   0        0        0     3314 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/discovery/footprints/log/variants/entire_event_log.py
--rw-rw-rw-   0        0        0     3195 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/discovery/footprints/log/variants/trace_by_trace.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:31.535424 pm4py-2.7.9.3/pm4py/algo/discovery/footprints/petri/
--rw-rw-rw-   0        0        0      794 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/discovery/footprints/petri/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:31.557998 pm4py-2.7.9.3/pm4py/algo/discovery/footprints/petri/variants/
--rw-rw-rw-   0        0        0      806 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/discovery/footprints/petri/variants/__init__.py
--rw-rw-rw-   0        0        0     3629 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/discovery/footprints/petri/variants/reach_graph.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:31.569067 pm4py-2.7.9.3/pm4py/algo/discovery/footprints/tree/
--rw-rw-rw-   0        0        0      793 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/discovery/footprints/tree/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:31.592995 pm4py-2.7.9.3/pm4py/algo/discovery/footprints/tree/variants/
--rw-rw-rw-   0        0        0      802 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/discovery/footprints/tree/variants/__init__.py
--rw-rw-rw-   0        0        0    13403 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/discovery/footprints/tree/variants/bottomup.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:31.615441 pm4py-2.7.9.3/pm4py/algo/discovery/heuristics/
--rw-rw-rw-   0        0        0      799 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/discovery/heuristics/__init__.py
--rw-rw-rw-   0        0        0     7484 2024-01-02 13:29:21.000000 pm4py-2.7.9.3/pm4py/algo/discovery/heuristics/algorithm.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:31.650689 pm4py-2.7.9.3/pm4py/algo/discovery/heuristics/variants/
--rw-rw-rw-   0        0        0      806 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/discovery/heuristics/variants/__init__.py
--rw-rw-rw-   0        0        0    26145 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/discovery/heuristics/variants/classic.py
--rw-rw-rw-   0        0        0    24355 2024-01-02 13:29:21.000000 pm4py-2.7.9.3/pm4py/algo/discovery/heuristics/variants/plusplus.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:31.673407 pm4py-2.7.9.3/pm4py/algo/discovery/ilp/
--rw-rw-rw-   0        0        0      792 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/discovery/ilp/__init__.py
--rw-rw-rw-   0        0        0     1782 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/discovery/ilp/algorithm.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:31.696622 pm4py-2.7.9.3/pm4py/algo/discovery/ilp/variants/
--rw-rw-rw-   0        0        0      789 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/discovery/ilp/variants/__init__.py
--rw-rw-rw-   0        0        0    12873 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/discovery/ilp/variants/classic.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:31.717561 pm4py-2.7.9.3/pm4py/algo/discovery/inductive/
--rw-rw-rw-   0        0        0      800 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/discovery/inductive/__init__.py
--rw-rw-rw-   0        0        0     3602 2024-01-02 13:29:21.000000 pm4py-2.7.9.3/pm4py/algo/discovery/inductive/algorithm.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:31.778571 pm4py-2.7.9.3/pm4py/algo/discovery/inductive/base_case/
--rw-rw-rw-   0        0        0      829 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/discovery/inductive/base_case/__init__.py
--rw-rw-rw-   0        0        0     1533 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/discovery/inductive/base_case/abc.py
--rw-rw-rw-   0        0        0     1768 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/discovery/inductive/base_case/empty_log.py
--rw-rw-rw-   0        0        0     2268 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/discovery/inductive/base_case/factory.py
--rw-rw-rw-   0        0        0     2060 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/discovery/inductive/base_case/single_activity.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:31.876389 pm4py-2.7.9.3/pm4py/algo/discovery/inductive/cuts/
--rw-rw-rw-   0        0        0      816 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/discovery/inductive/cuts/__init__.py
--rw-rw-rw-   0        0        0     2100 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/discovery/inductive/cuts/abc.py
--rw-rw-rw-   0        0        0     4570 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/discovery/inductive/cuts/concurrency.py
--rw-rw-rw-   0        0        0     3143 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/discovery/inductive/cuts/factory.py
--rw-rw-rw-   0        0        0    10916 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/discovery/inductive/cuts/loop.py
--rw-rw-rw-   0        0        0    11571 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/discovery/inductive/cuts/sequence.py
--rw-rw-rw-   0        0        0     1519 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/discovery/inductive/cuts/utils.py
--rw-rw-rw-   0        0        0     4316 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/discovery/inductive/cuts/xor.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:31.914480 pm4py-2.7.9.3/pm4py/algo/discovery/inductive/dtypes/
--rw-rw-rw-   0        0        0      797 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/discovery/inductive/dtypes/__init__.py
--rw-rw-rw-   0        0        0     1050 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/discovery/inductive/dtypes/im_dfg.py
--rw-rw-rw-   0        0        0     2568 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/discovery/inductive/dtypes/im_ds.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:32.020254 pm4py-2.7.9.3/pm4py/algo/discovery/inductive/fall_through/
--rw-rw-rw-   0        0        0      897 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/discovery/inductive/fall_through/__init__.py
--rw-rw-rw-   0        0        0     1385 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/discovery/inductive/fall_through/abc.py
--rw-rw-rw-   0        0        0     4792 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/discovery/inductive/fall_through/activity_concurrent.py
--rw-rw-rw-   0        0        0     1643 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/discovery/inductive/fall_through/activity_once_per_trace.py
--rw-rw-rw-   0        0        0     2709 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/discovery/inductive/fall_through/empty_traces.py
--rw-rw-rw-   0        0        0     3254 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/discovery/inductive/fall_through/factory.py
--rw-rw-rw-   0        0        0     3059 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/discovery/inductive/fall_through/flower.py
--rw-rw-rw-   0        0        0     2441 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/discovery/inductive/fall_through/strict_tau_loop.py
--rw-rw-rw-   0        0        0     1520 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/discovery/inductive/fall_through/tau_loop.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:32.088968 pm4py-2.7.9.3/pm4py/algo/discovery/inductive/variants/
--rw-rw-rw-   0        0        0      807 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/discovery/inductive/variants/__init__.py
--rw-rw-rw-   0        0        0     4160 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/discovery/inductive/variants/abc.py
--rw-rw-rw-   0        0        0     1740 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/discovery/inductive/variants/im.py
--rw-rw-rw-   0        0        0     1098 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/discovery/inductive/variants/imd.py
--rw-rw-rw-   0        0        0     4381 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/discovery/inductive/variants/imf.py
--rw-rw-rw-   0        0        0      881 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/discovery/inductive/variants/instances.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:32.121548 pm4py-2.7.9.3/pm4py/algo/discovery/log_skeleton/
--rw-rw-rw-   0        0        0      815 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/discovery/log_skeleton/__init__.py
--rw-rw-rw-   0        0        0     2450 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/discovery/log_skeleton/algorithm.py
--rw-rw-rw-   0        0        0     3194 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/discovery/log_skeleton/trace_skel.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:32.144890 pm4py-2.7.9.3/pm4py/algo/discovery/log_skeleton/variants/
--rw-rw-rw-   0        0        0      798 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/discovery/log_skeleton/variants/__init__.py
--rw-rw-rw-   0        0        0    11111 2024-01-15 12:00:43.000000 pm4py-2.7.9.3/pm4py/algo/discovery/log_skeleton/variants/classic.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:32.178584 pm4py-2.7.9.3/pm4py/algo/discovery/minimum_self_distance/
--rw-rw-rw-   0        0        0      819 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/discovery/minimum_self_distance/__init__.py
--rw-rw-rw-   0        0        0     1567 2024-01-02 13:29:21.000000 pm4py-2.7.9.3/pm4py/algo/discovery/minimum_self_distance/algorithm.py
--rw-rw-rw-   0        0        0     3132 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/discovery/minimum_self_distance/utils.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:32.211148 pm4py-2.7.9.3/pm4py/algo/discovery/minimum_self_distance/variants/
--rw-rw-rw-   0        0        0      811 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/discovery/minimum_self_distance/variants/__init__.py
--rw-rw-rw-   0        0        0     2878 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/discovery/minimum_self_distance/variants/log.py
--rw-rw-rw-   0        0        0     2904 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/discovery/minimum_self_distance/variants/pandas.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:32.223326 pm4py-2.7.9.3/pm4py/algo/discovery/ocel/
--rw-rw-rw-   0        0        0      802 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/discovery/ocel/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:32.245557 pm4py-2.7.9.3/pm4py/algo/discovery/ocel/interleavings/
--rw-rw-rw-   0        0        0      814 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/discovery/ocel/interleavings/__init__.py
--rw-rw-rw-   0        0        0     2007 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/discovery/ocel/interleavings/algorithm.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:32.267484 pm4py-2.7.9.3/pm4py/algo/discovery/ocel/interleavings/utils/
--rw-rw-rw-   0        0        0      819 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/discovery/ocel/interleavings/utils/__init__.py
--rw-rw-rw-   0        0        0     4451 2024-01-02 13:29:21.000000 pm4py-2.7.9.3/pm4py/algo/discovery/ocel/interleavings/utils/merge_dataframe_rel_cases.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:32.291964 pm4py-2.7.9.3/pm4py/algo/discovery/ocel/interleavings/variants/
--rw-rw-rw-   0        0        0      820 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/discovery/ocel/interleavings/variants/__init__.py
--rw-rw-rw-   0        0        0     6643 2024-01-15 12:00:43.000000 pm4py-2.7.9.3/pm4py/algo/discovery/ocel/interleavings/variants/timestamp_interleavings.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:32.314312 pm4py-2.7.9.3/pm4py/algo/discovery/ocel/link_analysis/
--rw-rw-rw-   0        0        0      796 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/discovery/ocel/link_analysis/__init__.py
--rw-rw-rw-   0        0        0     1841 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/discovery/ocel/link_analysis/algorithm.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:32.337252 pm4py-2.7.9.3/pm4py/algo/discovery/ocel/link_analysis/variants/
--rw-rw-rw-   0        0        0      804 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/discovery/ocel/link_analysis/variants/__init__.py
--rw-rw-rw-   0        0        0     6519 2024-01-02 13:29:21.000000 pm4py-2.7.9.3/pm4py/algo/discovery/ocel/link_analysis/variants/classic.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:32.359150 pm4py-2.7.9.3/pm4py/algo/discovery/ocel/ocdfg/
--rw-rw-rw-   0        0        0      799 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/discovery/ocel/ocdfg/__init__.py
--rw-rw-rw-   0        0        0     1775 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/discovery/ocel/ocdfg/algorithm.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:32.381694 pm4py-2.7.9.3/pm4py/algo/discovery/ocel/ocdfg/variants/
--rw-rw-rw-   0        0        0      796 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/discovery/ocel/ocdfg/variants/__init__.py
--rw-rw-rw-   0        0        0     8817 2024-01-02 13:29:21.000000 pm4py-2.7.9.3/pm4py/algo/discovery/ocel/ocdfg/variants/classic.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:32.404083 pm4py-2.7.9.3/pm4py/algo/discovery/ocel/ocpn/
--rw-rw-rw-   0        0        0      798 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/discovery/ocel/ocpn/__init__.py
--rw-rw-rw-   0        0        0     1785 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/discovery/ocel/ocpn/algorithm.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:32.439357 pm4py-2.7.9.3/pm4py/algo/discovery/ocel/ocpn/variants/
--rw-rw-rw-   0        0        0      797 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/discovery/ocel/ocpn/variants/__init__.py
--rw-rw-rw-   0        0        0    10290 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/discovery/ocel/ocpn/variants/classic.py
--rw-rw-rw-   0        0        0      812 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/discovery/ocel/ocpn/variants/wo_annotation.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:32.462164 pm4py-2.7.9.3/pm4py/algo/discovery/ocel/saw_nets/
--rw-rw-rw-   0        0        0      804 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/discovery/ocel/saw_nets/__init__.py
--rw-rw-rw-   0        0        0     1800 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/discovery/ocel/saw_nets/algorithm.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:32.484109 pm4py-2.7.9.3/pm4py/algo/discovery/ocel/saw_nets/variants/
--rw-rw-rw-   0        0        0      801 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/discovery/ocel/saw_nets/variants/__init__.py
--rw-rw-rw-   0        0        0     7569 2024-01-02 13:29:21.000000 pm4py-2.7.9.3/pm4py/algo/discovery/ocel/saw_nets/variants/classic.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:32.506832 pm4py-2.7.9.3/pm4py/algo/discovery/performance_spectrum/
--rw-rw-rw-   0        0        0      809 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/discovery/performance_spectrum/__init__.py
--rw-rw-rw-   0        0        0     3495 2024-01-02 13:29:21.000000 pm4py-2.7.9.3/pm4py/algo/discovery/performance_spectrum/algorithm.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:32.565771 pm4py-2.7.9.3/pm4py/algo/discovery/performance_spectrum/variants/
--rw-rw-rw-   0        0        0      855 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/discovery/performance_spectrum/variants/__init__.py
--rw-rw-rw-   0        0        0     4317 2024-01-02 13:29:21.000000 pm4py-2.7.9.3/pm4py/algo/discovery/performance_spectrum/variants/dataframe.py
--rw-rw-rw-   0        0        0     4970 2024-01-02 13:29:21.000000 pm4py-2.7.9.3/pm4py/algo/discovery/performance_spectrum/variants/dataframe_disconnected.py
--rw-rw-rw-   0        0        0     3382 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/discovery/performance_spectrum/variants/log.py
--rw-rw-rw-   0        0        0     4366 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/discovery/performance_spectrum/variants/log_disconnected.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:32.588751 pm4py-2.7.9.3/pm4py/algo/discovery/powl/
--rw-rw-rw-   0        0        0      779 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/discovery/powl/__init__.py
--rw-rw-rw-   0        0        0     3201 2024-01-02 13:29:21.000000 pm4py-2.7.9.3/pm4py/algo/discovery/powl/algorithm.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:32.600159 pm4py-2.7.9.3/pm4py/algo/discovery/powl/inductive/
--rw-rw-rw-   0        0        0      787 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/discovery/powl/inductive/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:32.668453 pm4py-2.7.9.3/pm4py/algo/discovery/powl/inductive/base_case/
--rw-rw-rw-   0        0        0      797 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/discovery/powl/inductive/base_case/__init__.py
--rw-rw-rw-   0        0        0     1506 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/discovery/powl/inductive/base_case/abc.py
--rw-rw-rw-   0        0        0     1457 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/discovery/powl/inductive/base_case/empty_log.py
--rw-rw-rw-   0        0        0     1867 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/discovery/powl/inductive/base_case/factory.py
--rw-rw-rw-   0        0        0     1547 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/discovery/powl/inductive/base_case/single_activity.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:32.746856 pm4py-2.7.9.3/pm4py/algo/discovery/powl/inductive/cuts/
--rw-rw-rw-   0        0        0      792 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/discovery/powl/inductive/cuts/__init__.py
--rw-rw-rw-   0        0        0     1361 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/discovery/powl/inductive/cuts/concurrency.py
--rw-rw-rw-   0        0        0     1974 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/discovery/powl/inductive/cuts/factory.py
--rw-rw-rw-   0        0        0     1353 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/discovery/powl/inductive/cuts/loop.py
--rw-rw-rw-   0        0        0     1975 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/discovery/powl/inductive/cuts/sequence.py
--rw-rw-rw-   0        0        0     1433 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/discovery/powl/inductive/cuts/xor.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:32.834614 pm4py-2.7.9.3/pm4py/algo/discovery/powl/inductive/fall_through/
--rw-rw-rw-   0        0        0      798 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/discovery/powl/inductive/fall_through/__init__.py
--rw-rw-rw-   0        0        0     1905 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/discovery/powl/inductive/fall_through/activity_concurrent.py
--rw-rw-rw-   0        0        0     1056 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/discovery/powl/inductive/fall_through/activity_once_per_trace.py
--rw-rw-rw-   0        0        0     1795 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/discovery/powl/inductive/fall_through/empty_traces.py
--rw-rw-rw-   0        0        0     2498 2024-01-02 13:29:21.000000 pm4py-2.7.9.3/pm4py/algo/discovery/powl/inductive/fall_through/factory.py
--rw-rw-rw-   0        0        0     1814 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/discovery/powl/inductive/fall_through/flower.py
--rw-rw-rw-   0        0        0     1651 2024-01-02 13:29:21.000000 pm4py-2.7.9.3/pm4py/algo/discovery/powl/inductive/fall_through/strict_tau_loop.py
--rw-rw-rw-   0        0        0     1630 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/discovery/powl/inductive/fall_through/tau_loop.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:32.849693 pm4py-2.7.9.3/pm4py/algo/discovery/powl/inductive/utils/
--rw-rw-rw-   0        0        0      734 2024-01-02 13:29:21.000000 pm4py-2.7.9.3/pm4py/algo/discovery/powl/inductive/utils/__init__.py
--rw-rw-rw-   0        0        0     2008 2024-01-02 13:29:21.000000 pm4py-2.7.9.3/pm4py/algo/discovery/powl/inductive/utils/filtering.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:32.924779 pm4py-2.7.9.3/pm4py/algo/discovery/powl/inductive/variants/
--rw-rw-rw-   0        0        0      798 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/discovery/powl/inductive/variants/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:32.959076 pm4py-2.7.9.3/pm4py/algo/discovery/powl/inductive/variants/brute_force/
--rw-rw-rw-   0        0        0      806 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/discovery/powl/inductive/variants/brute_force/__init__.py
--rw-rw-rw-   0        0        0     7020 2024-01-02 13:29:21.000000 pm4py-2.7.9.3/pm4py/algo/discovery/powl/inductive/variants/brute_force/bf_partial_order_cut.py
--rw-rw-rw-   0        0        0     2195 2024-01-02 13:29:21.000000 pm4py-2.7.9.3/pm4py/algo/discovery/powl/inductive/variants/brute_force/factory.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:32.993023 pm4py-2.7.9.3/pm4py/algo/discovery/powl/inductive/variants/dynamic_clustering/
--rw-rw-rw-   0        0        0      813 2024-01-02 13:29:21.000000 pm4py-2.7.9.3/pm4py/algo/discovery/powl/inductive/variants/dynamic_clustering/__init__.py
--rw-rw-rw-   0        0        0     7347 2024-01-02 13:29:21.000000 pm4py-2.7.9.3/pm4py/algo/discovery/powl/inductive/variants/dynamic_clustering/dynamic_clustering_partial_order_cut.py
--rw-rw-rw-   0        0        0     2043 2024-01-02 13:29:21.000000 pm4py-2.7.9.3/pm4py/algo/discovery/powl/inductive/variants/dynamic_clustering/factory.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:33.026357 pm4py-2.7.9.3/pm4py/algo/discovery/powl/inductive/variants/dynamic_clustering_frequency/
--rw-rw-rw-   0        0        0      823 2024-01-02 13:29:21.000000 pm4py-2.7.9.3/pm4py/algo/discovery/powl/inductive/variants/dynamic_clustering_frequency/__init__.py
--rw-rw-rw-   0        0        0     8397 2024-01-02 13:29:21.000000 pm4py-2.7.9.3/pm4py/algo/discovery/powl/inductive/variants/dynamic_clustering_frequency/dynamic_clustering_frequency_partial_order_cut.py
--rw-rw-rw-   0        0        0     2099 2024-01-02 13:29:21.000000 pm4py-2.7.9.3/pm4py/algo/discovery/powl/inductive/variants/dynamic_clustering_frequency/factory.py
--rw-rw-rw-   0        0        0     1482 2024-01-02 13:29:21.000000 pm4py-2.7.9.3/pm4py/algo/discovery/powl/inductive/variants/im_brute_force.py
--rw-rw-rw-   0        0        0     1643 2024-01-02 13:29:21.000000 pm4py-2.7.9.3/pm4py/algo/discovery/powl/inductive/variants/im_dynamic_clustering.py
--rw-rw-rw-   0        0        0     1687 2024-01-02 13:29:21.000000 pm4py-2.7.9.3/pm4py/algo/discovery/powl/inductive/variants/im_dynamic_clustering_frequencies.py
--rw-rw-rw-   0        0        0     1468 2024-01-02 13:29:21.000000 pm4py-2.7.9.3/pm4py/algo/discovery/powl/inductive/variants/im_maximal.py
--rw-rw-rw-   0        0        0     5456 2024-01-02 13:29:21.000000 pm4py-2.7.9.3/pm4py/algo/discovery/powl/inductive/variants/im_tree.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:33.060607 pm4py-2.7.9.3/pm4py/algo/discovery/powl/inductive/variants/maximal/
--rw-rw-rw-   0        0        0      800 2024-01-02 13:29:21.000000 pm4py-2.7.9.3/pm4py/algo/discovery/powl/inductive/variants/maximal/__init__.py
--rw-rw-rw-   0        0        0     2373 2024-01-02 13:29:21.000000 pm4py-2.7.9.3/pm4py/algo/discovery/powl/inductive/variants/maximal/factory.py
--rw-rw-rw-   0        0        0     7192 2024-01-02 13:29:21.000000 pm4py-2.7.9.3/pm4py/algo/discovery/powl/inductive/variants/maximal/maximal_partial_order_cut.py
--rw-rw-rw-   0        0        0      936 2024-01-02 13:29:21.000000 pm4py-2.7.9.3/pm4py/algo/discovery/powl/inductive/variants/powl_discovery_varaints.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:33.084694 pm4py-2.7.9.3/pm4py/algo/discovery/temporal_profile/
--rw-rw-rw-   0        0        0      805 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/discovery/temporal_profile/__init__.py
--rw-rw-rw-   0        0        0     2006 2024-01-02 13:29:21.000000 pm4py-2.7.9.3/pm4py/algo/discovery/temporal_profile/algorithm.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:33.118693 pm4py-2.7.9.3/pm4py/algo/discovery/temporal_profile/variants/
--rw-rw-rw-   0        0        0      809 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/discovery/temporal_profile/variants/__init__.py
--rw-rw-rw-   0        0        0     4044 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/discovery/temporal_profile/variants/dataframe.py
--rw-rw-rw-   0        0        0     5236 2024-01-02 13:29:21.000000 pm4py-2.7.9.3/pm4py/algo/discovery/temporal_profile/variants/log.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:33.140535 pm4py-2.7.9.3/pm4py/algo/discovery/transition_system/
--rw-rw-rw-   0        0        0      806 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/discovery/transition_system/__init__.py
--rw-rw-rw-   0        0        0     1984 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/discovery/transition_system/algorithm.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:33.163644 pm4py-2.7.9.3/pm4py/algo/discovery/transition_system/variants/
--rw-rw-rw-   0        0        0      806 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/discovery/transition_system/variants/__init__.py
--rw-rw-rw-   0        0        0     5956 2024-01-15 12:00:43.000000 pm4py-2.7.9.3/pm4py/algo/discovery/transition_system/variants/view_based.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:33.186429 pm4py-2.7.9.3/pm4py/algo/evaluation/
--rw-rw-rw-   0        0        0      836 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/evaluation/__init__.py
--rw-rw-rw-   0        0        0     4819 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/evaluation/algorithm.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:33.209283 pm4py-2.7.9.3/pm4py/algo/evaluation/earth_mover_distance/
--rw-rw-rw-   0        0        0      995 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/evaluation/earth_mover_distance/__init__.py
--rw-rw-rw-   0        0        0     1678 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/evaluation/earth_mover_distance/algorithm.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:33.232843 pm4py-2.7.9.3/pm4py/algo/evaluation/earth_mover_distance/variants/
--rw-rw-rw-   0        0        0      805 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/evaluation/earth_mover_distance/variants/__init__.py
--rw-rw-rw-   0        0        0     4864 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/evaluation/earth_mover_distance/variants/pyemd.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:33.254473 pm4py-2.7.9.3/pm4py/algo/evaluation/generalization/
--rw-rw-rw-   0        0        0      804 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/evaluation/generalization/__init__.py
--rw-rw-rw-   0        0        0     1703 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/evaluation/generalization/algorithm.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:33.277980 pm4py-2.7.9.3/pm4py/algo/evaluation/generalization/variants/
--rw-rw-rw-   0        0        0      805 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/evaluation/generalization/variants/__init__.py
--rw-rw-rw-   0        0        0     2285 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/evaluation/generalization/variants/token_based.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:33.312518 pm4py-2.7.9.3/pm4py/algo/evaluation/precision/
--rw-rw-rw-   0        0        0      811 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/evaluation/precision/__init__.py
--rw-rw-rw-   0        0        0     2994 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/evaluation/precision/algorithm.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:33.333955 pm4py-2.7.9.3/pm4py/algo/evaluation/precision/dfg/
--rw-rw-rw-   0        0        0      793 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/evaluation/precision/dfg/__init__.py
--rw-rw-rw-   0        0        0     3992 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/evaluation/precision/dfg/algorithm.py
--rw-rw-rw-   0        0        0     5525 2024-01-15 12:00:43.000000 pm4py-2.7.9.3/pm4py/algo/evaluation/precision/utils.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:33.372517 pm4py-2.7.9.3/pm4py/algo/evaluation/precision/variants/
--rw-rw-rw-   0        0        0      829 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/evaluation/precision/variants/__init__.py
--rw-rw-rw-   0        0        0    13806 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/evaluation/precision/variants/align_etconformance.py
--rw-rw-rw-   0        0        0     6199 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/evaluation/precision/variants/etconformance_token.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:33.396778 pm4py-2.7.9.3/pm4py/algo/evaluation/replay_fitness/
--rw-rw-rw-   0        0        0      804 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/evaluation/replay_fitness/__init__.py
--rw-rw-rw-   0        0        0     4486 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/evaluation/replay_fitness/algorithm.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:33.430904 pm4py-2.7.9.3/pm4py/algo/evaluation/replay_fitness/variants/
--rw-rw-rw-   0        0        0      823 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/evaluation/replay_fitness/variants/__init__.py
--rw-rw-rw-   0        0        0     6788 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/evaluation/replay_fitness/variants/alignment_based.py
--rw-rw-rw-   0        0        0     5159 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/evaluation/replay_fitness/variants/token_replay.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:33.453091 pm4py-2.7.9.3/pm4py/algo/evaluation/simplicity/
--rw-rw-rw-   0        0        0      802 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/evaluation/simplicity/__init__.py
--rw-rw-rw-   0        0        0     1585 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/evaluation/simplicity/algorithm.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:33.496994 pm4py-2.7.9.3/pm4py/algo/evaluation/simplicity/variants/
--rw-rw-rw-   0        0        0      841 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/evaluation/simplicity/variants/__init__.py
--rw-rw-rw-   0        0        0     2696 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/evaluation/simplicity/variants/arc_degree.py
--rw-rw-rw-   0        0        0     1602 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/evaluation/simplicity/variants/extended_cardoso.py
--rw-rw-rw-   0        0        0     2120 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/evaluation/simplicity/variants/extended_cyclomatic.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:33.500884 pm4py-2.7.9.3/pm4py/algo/filtering/
--rw-rw-rw-   0        0        0      734 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/filtering/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:33.524756 pm4py-2.7.9.3/pm4py/algo/filtering/common/
--rw-rw-rw-   0        0        0      852 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/filtering/common/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:33.540028 pm4py-2.7.9.3/pm4py/algo/filtering/common/attributes/
--rw-rw-rw-   0        0        0      734 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/filtering/common/attributes/__init__.py
--rw-rw-rw-   0        0        0      951 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/filtering/common/attributes/attributes_common.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:33.564149 pm4py-2.7.9.3/pm4py/algo/filtering/common/end_activities/
--rw-rw-rw-   0        0        0      812 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/filtering/common/end_activities/__init__.py
--rw-rw-rw-   0        0        0      851 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/filtering/common/end_activities/end_activities_common.py
--rw-rw-rw-   0        0        0      845 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/filtering/common/filtering_constants.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:33.589012 pm4py-2.7.9.3/pm4py/algo/filtering/common/start_activities/
--rw-rw-rw-   0        0        0      816 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/filtering/common/start_activities/__init__.py
--rw-rw-rw-   0        0        0      857 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/filtering/common/start_activities/start_activities_common.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:33.604245 pm4py-2.7.9.3/pm4py/algo/filtering/common/timestamp/
--rw-rw-rw-   0        0        0      734 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/filtering/common/timestamp/__init__.py
--rw-rw-rw-   0        0        0     1250 2024-01-02 13:29:21.000000 pm4py-2.7.9.3/pm4py/algo/filtering/common/timestamp/timestamp_common.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:33.620893 pm4py-2.7.9.3/pm4py/algo/filtering/common/traces/
--rw-rw-rw-   0        0        0      734 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/filtering/common/traces/__init__.py
--rw-rw-rw-   0        0        0     1246 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/filtering/common/traces/infix_to_regex.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:33.636931 pm4py-2.7.9.3/pm4py/algo/filtering/dfg/
--rw-rw-rw-   0        0        0      734 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/filtering/dfg/__init__.py
--rw-rw-rw-   0        0        0    25920 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/filtering/dfg/dfg_filtering.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:33.652675 pm4py-2.7.9.3/pm4py/algo/filtering/log/
--rw-rw-rw-   0        0        0      866 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/filtering/log/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:33.678066 pm4py-2.7.9.3/pm4py/algo/filtering/log/attr_value_repetition/
--rw-rw-rw-   0        0        0      994 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/filtering/log/attr_value_repetition/__init__.py
--rw-rw-rw-   0        0        0     2754 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/filtering/log/attr_value_repetition/filter.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:33.701130 pm4py-2.7.9.3/pm4py/algo/filtering/log/attributes/
--rw-rw-rw-   0        0        0      801 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/filtering/log/attributes/__init__.py
--rw-rw-rw-   0        0        0    18308 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/filtering/log/attributes/attributes_filter.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:33.723851 pm4py-2.7.9.3/pm4py/algo/filtering/log/between/
--rw-rw-rw-   0        0        0      795 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/filtering/log/between/__init__.py
--rw-rw-rw-   0        0        0     2944 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/filtering/log/between/between_filter.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:33.750366 pm4py-2.7.9.3/pm4py/algo/filtering/log/cases/
--rw-rw-rw-   0        0        0      790 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/filtering/log/cases/__init__.py
--rw-rw-rw-   0        0        0     4597 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/filtering/log/cases/case_filter.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:33.774229 pm4py-2.7.9.3/pm4py/algo/filtering/log/end_activities/
--rw-rw-rw-   0        0        0      809 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/filtering/log/end_activities/__init__.py
--rw-rw-rw-   0        0        0     3719 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/filtering/log/end_activities/end_activities_filter.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:33.797006 pm4py-2.7.9.3/pm4py/algo/filtering/log/ltl/
--rw-rw-rw-   0        0        0      788 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/filtering/log/ltl/__init__.py
--rw-rw-rw-   0        0        0    11094 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/filtering/log/ltl/ltl_checker.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:33.820544 pm4py-2.7.9.3/pm4py/algo/filtering/log/paths/
--rw-rw-rw-   0        0        0      791 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/filtering/log/paths/__init__.py
--rw-rw-rw-   0        0        0     9660 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/filtering/log/paths/paths_filter.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:33.843009 pm4py-2.7.9.3/pm4py/algo/filtering/log/prefixes/
--rw-rw-rw-   0        0        0      797 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/filtering/log/prefixes/__init__.py
--rw-rw-rw-   0        0        0     3218 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/filtering/log/prefixes/prefix_filter.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:33.865129 pm4py-2.7.9.3/pm4py/algo/filtering/log/rework/
--rw-rw-rw-   0        0        0      793 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/filtering/log/rework/__init__.py
--rw-rw-rw-   0        0        0     3412 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/filtering/log/rework/rework_filter.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:33.886761 pm4py-2.7.9.3/pm4py/algo/filtering/log/start_activities/
--rw-rw-rw-   0        0        0      813 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/filtering/log/start_activities/__init__.py
--rw-rw-rw-   0        0        0     3950 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/filtering/log/start_activities/start_activities_filter.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:33.911175 pm4py-2.7.9.3/pm4py/algo/filtering/log/suffixes/
--rw-rw-rw-   0        0        0      797 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/filtering/log/suffixes/__init__.py
--rw-rw-rw-   0        0        0     3223 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/filtering/log/suffixes/suffix_filter.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:33.934735 pm4py-2.7.9.3/pm4py/algo/filtering/log/timestamp/
--rw-rw-rw-   0        0        0      799 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/filtering/log/timestamp/__init__.py
--rw-rw-rw-   0        0        0    11509 2024-01-02 13:29:21.000000 pm4py-2.7.9.3/pm4py/algo/filtering/log/timestamp/timestamp_filter.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:33.948967 pm4py-2.7.9.3/pm4py/algo/filtering/log/traces/
--rw-rw-rw-   0        0        0      734 2024-01-02 13:29:21.000000 pm4py-2.7.9.3/pm4py/algo/filtering/log/traces/__init__.py
--rw-rw-rw-   0        0        0     3785 2024-01-02 13:29:21.000000 pm4py-2.7.9.3/pm4py/algo/filtering/log/traces/trace_filter.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:33.971495 pm4py-2.7.9.3/pm4py/algo/filtering/log/variants/
--rw-rw-rw-   0        0        0      797 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/filtering/log/variants/__init__.py
--rw-rw-rw-   0        0        0     9002 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/filtering/log/variants/variants_filter.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:34.038396 pm4py-2.7.9.3/pm4py/algo/filtering/ocel/
--rw-rw-rw-   0        0        0      865 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/filtering/ocel/__init__.py
--rw-rw-rw-   0        0        0     3392 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/filtering/ocel/activity_type_matching.py
--rw-rw-rw-   0        0        0     3843 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/filtering/ocel/event_attributes.py
--rw-rw-rw-   0        0        0     2319 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/filtering/ocel/object_attributes.py
--rw-rw-rw-   0        0        0     3436 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/filtering/ocel/objects_ot_count.py
--rw-rw-rw-   0        0        0     4195 2024-01-02 13:29:21.000000 pm4py-2.7.9.3/pm4py/algo/filtering/ocel/ot_endpoints.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:34.061961 pm4py-2.7.9.3/pm4py/algo/filtering/pandas/
--rw-rw-rw-   0        0        0      891 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/filtering/pandas/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:34.085000 pm4py-2.7.9.3/pm4py/algo/filtering/pandas/attr_value_repetition/
--rw-rw-rw-   0        0        0      997 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/filtering/pandas/attr_value_repetition/__init__.py
--rw-rw-rw-   0        0        0     2786 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/filtering/pandas/attr_value_repetition/filter.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:34.100190 pm4py-2.7.9.3/pm4py/algo/filtering/pandas/attributes/
--rw-rw-rw-   0        0        0      734 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/filtering/pandas/attributes/__init__.py
--rw-rw-rw-   0        0        0    13156 2024-01-15 12:00:43.000000 pm4py-2.7.9.3/pm4py/algo/filtering/pandas/attributes/attributes_filter.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:34.122621 pm4py-2.7.9.3/pm4py/algo/filtering/pandas/between/
--rw-rw-rw-   0        0        0      798 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/filtering/pandas/between/__init__.py
--rw-rw-rw-   0        0        0     3266 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/filtering/pandas/between/between_filter.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:34.144096 pm4py-2.7.9.3/pm4py/algo/filtering/pandas/cases/
--rw-rw-rw-   0        0        0      793 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/filtering/pandas/cases/__init__.py
--rw-rw-rw-   0        0        0     6322 2024-01-15 12:00:43.000000 pm4py-2.7.9.3/pm4py/algo/filtering/pandas/cases/case_filter.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:34.166868 pm4py-2.7.9.3/pm4py/algo/filtering/pandas/consecutive_act_case_grouping/
--rw-rw-rw-   0        0        0      842 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/filtering/pandas/consecutive_act_case_grouping/__init__.py
--rw-rw-rw-   0        0        0     3077 2024-01-02 13:29:21.000000 pm4py-2.7.9.3/pm4py/algo/filtering/pandas/consecutive_act_case_grouping/consecutive_act_case_grouping_filter.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:34.189178 pm4py-2.7.9.3/pm4py/algo/filtering/pandas/end_activities/
--rw-rw-rw-   0        0        0      812 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/filtering/pandas/end_activities/__init__.py
--rw-rw-rw-   0        0        0     6142 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/filtering/pandas/end_activities/end_activities_filter.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:34.202064 pm4py-2.7.9.3/pm4py/algo/filtering/pandas/ends_with/
--rw-rw-rw-   0        0        0      734 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/filtering/pandas/ends_with/__init__.py
--rw-rw-rw-   0        0        0     3508 2023-12-11 09:33:51.000000 pm4py-2.7.9.3/pm4py/algo/filtering/pandas/ends_with/ends_with_filter.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:34.226179 pm4py-2.7.9.3/pm4py/algo/filtering/pandas/ltl/
--rw-rw-rw-   0        0        0      791 2023-12-11 09:33:52.000000 pm4py-2.7.9.3/pm4py/algo/filtering/pandas/ltl/__init__.py
--rw-rw-rw-   0        0        0    11763 2024-01-15 12:00:43.000000 pm4py-2.7.9.3/pm4py/algo/filtering/pandas/ltl/ltl_checker.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:34.254186 pm4py-2.7.9.3/pm4py/algo/filtering/pandas/paths/
--rw-rw-rw-   0        0        0      794 2023-12-11 09:33:52.000000 pm4py-2.7.9.3/pm4py/algo/filtering/pandas/paths/__init__.py
--rw-rw-rw-   0        0        0     6919 2024-01-15 12:00:43.000000 pm4py-2.7.9.3/pm4py/algo/filtering/pandas/paths/paths_filter.py
--rw-rw-rw-   0        0        0      832 2023-12-11 09:33:52.000000 pm4py-2.7.9.3/pm4py/algo/filtering/pandas/pd_filtering_constants.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:34.279822 pm4py-2.7.9.3/pm4py/algo/filtering/pandas/prefixes/
--rw-rw-rw-   0        0        0      800 2023-12-11 09:33:52.000000 pm4py-2.7.9.3/pm4py/algo/filtering/pandas/prefixes/__init__.py
--rw-rw-rw-   0        0        0     3950 2023-12-11 09:33:52.000000 pm4py-2.7.9.3/pm4py/algo/filtering/pandas/prefixes/prefix_filter.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:34.303043 pm4py-2.7.9.3/pm4py/algo/filtering/pandas/rework/
--rw-rw-rw-   0        0        0      796 2023-12-11 09:33:52.000000 pm4py-2.7.9.3/pm4py/algo/filtering/pandas/rework/__init__.py
--rw-rw-rw-   0        0        0     3425 2024-01-02 13:29:21.000000 pm4py-2.7.9.3/pm4py/algo/filtering/pandas/rework/rework_filter.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:34.327228 pm4py-2.7.9.3/pm4py/algo/filtering/pandas/start_activities/
--rw-rw-rw-   0        0        0      816 2023-12-11 09:33:52.000000 pm4py-2.7.9.3/pm4py/algo/filtering/pandas/start_activities/__init__.py
--rw-rw-rw-   0        0        0     5585 2023-12-11 09:33:52.000000 pm4py-2.7.9.3/pm4py/algo/filtering/pandas/start_activities/start_activities_filter.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:34.340748 pm4py-2.7.9.3/pm4py/algo/filtering/pandas/starts_with/
--rw-rw-rw-   0        0        0      734 2023-12-11 09:33:52.000000 pm4py-2.7.9.3/pm4py/algo/filtering/pandas/starts_with/__init__.py
--rw-rw-rw-   0        0        0     3510 2023-12-11 09:33:52.000000 pm4py-2.7.9.3/pm4py/algo/filtering/pandas/starts_with/starts_with_filter.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:34.362434 pm4py-2.7.9.3/pm4py/algo/filtering/pandas/suffixes/
--rw-rw-rw-   0        0        0      736 2023-12-11 09:33:52.000000 pm4py-2.7.9.3/pm4py/algo/filtering/pandas/suffixes/__init__.py
--rw-rw-rw-   0        0        0     3950 2023-12-11 09:33:52.000000 pm4py-2.7.9.3/pm4py/algo/filtering/pandas/suffixes/suffix_filter.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:34.383731 pm4py-2.7.9.3/pm4py/algo/filtering/pandas/timestamp/
--rw-rw-rw-   0        0        0      802 2023-12-11 09:33:52.000000 pm4py-2.7.9.3/pm4py/algo/filtering/pandas/timestamp/__init__.py
--rw-rw-rw-   0        0        0     8208 2024-01-02 13:29:21.000000 pm4py-2.7.9.3/pm4py/algo/filtering/pandas/timestamp/timestamp_filter.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:34.407123 pm4py-2.7.9.3/pm4py/algo/filtering/pandas/timestamp_case_grouping/
--rw-rw-rw-   0        0        0      830 2023-12-11 09:33:52.000000 pm4py-2.7.9.3/pm4py/algo/filtering/pandas/timestamp_case_grouping/__init__.py
--rw-rw-rw-   0        0        0     3499 2024-01-02 13:29:21.000000 pm4py-2.7.9.3/pm4py/algo/filtering/pandas/timestamp_case_grouping/timestamp_case_grouping_filter.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:34.420945 pm4py-2.7.9.3/pm4py/algo/filtering/pandas/traces/
--rw-rw-rw-   0        0        0      736 2023-12-11 09:33:52.000000 pm4py-2.7.9.3/pm4py/algo/filtering/pandas/traces/__init__.py
--rw-rw-rw-   0        0        0     3604 2023-12-11 09:33:52.000000 pm4py-2.7.9.3/pm4py/algo/filtering/pandas/traces/trace_filter.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:34.433665 pm4py-2.7.9.3/pm4py/algo/filtering/pandas/variants/
--rw-rw-rw-   0        0        0      734 2023-12-11 09:33:52.000000 pm4py-2.7.9.3/pm4py/algo/filtering/pandas/variants/__init__.py
--rw-rw-rw-   0        0        0     6083 2023-12-11 09:33:52.000000 pm4py-2.7.9.3/pm4py/algo/filtering/pandas/variants/variants_filter.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:34.458464 pm4py-2.7.9.3/pm4py/algo/label_splitting/
--rw-rw-rw-   0        0        0      794 2024-01-02 13:29:21.000000 pm4py-2.7.9.3/pm4py/algo/label_splitting/__init__.py
--rw-rw-rw-   0        0        0     1921 2024-01-02 13:29:21.000000 pm4py-2.7.9.3/pm4py/algo/label_splitting/algorithm.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:34.482827 pm4py-2.7.9.3/pm4py/algo/label_splitting/variants/
--rw-rw-rw-   0        0        0      794 2024-01-02 13:29:21.000000 pm4py-2.7.9.3/pm4py/algo/label_splitting/variants/__init__.py
--rw-rw-rw-   0        0        0     9446 2024-01-02 13:29:21.000000 pm4py-2.7.9.3/pm4py/algo/label_splitting/variants/contextual.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:34.494980 pm4py-2.7.9.3/pm4py/algo/merging/
--rw-rw-rw-   0        0        0      781 2023-12-11 09:33:52.000000 pm4py-2.7.9.3/pm4py/algo/merging/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:34.516464 pm4py-2.7.9.3/pm4py/algo/merging/case_relations/
--rw-rw-rw-   0        0        0      801 2023-12-11 09:33:52.000000 pm4py-2.7.9.3/pm4py/algo/merging/case_relations/__init__.py
--rw-rw-rw-   0        0        0     2326 2023-12-11 09:33:52.000000 pm4py-2.7.9.3/pm4py/algo/merging/case_relations/algorithm.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:34.538553 pm4py-2.7.9.3/pm4py/algo/merging/case_relations/variants/
--rw-rw-rw-   0        0        0      797 2023-12-11 09:33:52.000000 pm4py-2.7.9.3/pm4py/algo/merging/case_relations/variants/__init__.py
--rw-rw-rw-   0        0        0     3498 2024-01-02 13:29:21.000000 pm4py-2.7.9.3/pm4py/algo/merging/case_relations/variants/pandas.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:34.560325 pm4py-2.7.9.3/pm4py/algo/organizational_mining/
--rw-rw-rw-   0        0        0      855 2023-12-11 09:33:52.000000 pm4py-2.7.9.3/pm4py/algo/organizational_mining/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:34.582056 pm4py-2.7.9.3/pm4py/algo/organizational_mining/local_diagnostics/
--rw-rw-rw-   0        0        0      808 2023-12-11 09:33:52.000000 pm4py-2.7.9.3/pm4py/algo/organizational_mining/local_diagnostics/__init__.py
--rw-rw-rw-   0        0        0    12440 2023-12-11 09:33:52.000000 pm4py-2.7.9.3/pm4py/algo/organizational_mining/local_diagnostics/algorithm.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:34.604849 pm4py-2.7.9.3/pm4py/algo/organizational_mining/network_analysis/
--rw-rw-rw-   0        0        0      817 2023-12-11 09:33:52.000000 pm4py-2.7.9.3/pm4py/algo/organizational_mining/network_analysis/__init__.py
--rw-rw-rw-   0        0        0     1840 2023-12-11 09:33:52.000000 pm4py-2.7.9.3/pm4py/algo/organizational_mining/network_analysis/algorithm.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:34.627098 pm4py-2.7.9.3/pm4py/algo/organizational_mining/network_analysis/variants/
--rw-rw-rw-   0        0        0      816 2023-12-11 09:33:52.000000 pm4py-2.7.9.3/pm4py/algo/organizational_mining/network_analysis/variants/__init__.py
--rw-rw-rw-   0        0        0    10562 2024-01-15 12:00:43.000000 pm4py-2.7.9.3/pm4py/algo/organizational_mining/network_analysis/variants/dataframe.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:34.654693 pm4py-2.7.9.3/pm4py/algo/organizational_mining/resource_profiles/
--rw-rw-rw-   0        0        0      818 2023-12-11 09:33:52.000000 pm4py-2.7.9.3/pm4py/algo/organizational_mining/resource_profiles/__init__.py
--rw-rw-rw-   0        0        0    12251 2024-01-02 13:29:21.000000 pm4py-2.7.9.3/pm4py/algo/organizational_mining/resource_profiles/algorithm.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:34.689287 pm4py-2.7.9.3/pm4py/algo/organizational_mining/resource_profiles/variants/
--rw-rw-rw-   0        0        0      819 2023-12-11 09:33:52.000000 pm4py-2.7.9.3/pm4py/algo/organizational_mining/resource_profiles/variants/__init__.py
--rw-rw-rw-   0        0        0    23271 2024-01-02 13:29:21.000000 pm4py-2.7.9.3/pm4py/algo/organizational_mining/resource_profiles/variants/log.py
--rw-rw-rw-   0        0        0    23967 2024-01-15 12:00:43.000000 pm4py-2.7.9.3/pm4py/algo/organizational_mining/resource_profiles/variants/pandas.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:34.711365 pm4py-2.7.9.3/pm4py/algo/organizational_mining/roles/
--rw-rw-rw-   0        0        0      814 2023-12-11 09:33:52.000000 pm4py-2.7.9.3/pm4py/algo/organizational_mining/roles/__init__.py
--rw-rw-rw-   0        0        0     2427 2024-01-02 13:29:21.000000 pm4py-2.7.9.3/pm4py/algo/organizational_mining/roles/algorithm.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:34.735020 pm4py-2.7.9.3/pm4py/algo/organizational_mining/roles/common/
--rw-rw-rw-   0        0        0      803 2023-12-11 09:33:52.000000 pm4py-2.7.9.3/pm4py/algo/organizational_mining/roles/common/__init__.py
--rw-rw-rw-   0        0        0     8411 2023-12-11 09:33:52.000000 pm4py-2.7.9.3/pm4py/algo/organizational_mining/roles/common/algorithm.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:34.766462 pm4py-2.7.9.3/pm4py/algo/organizational_mining/roles/variants/
--rw-rw-rw-   0        0        0      807 2023-12-11 09:33:52.000000 pm4py-2.7.9.3/pm4py/algo/organizational_mining/roles/variants/__init__.py
--rw-rw-rw-   0        0        0     2448 2023-12-11 09:33:52.000000 pm4py-2.7.9.3/pm4py/algo/organizational_mining/roles/variants/log.py
--rw-rw-rw-   0        0        0     2213 2024-01-15 12:00:43.000000 pm4py-2.7.9.3/pm4py/algo/organizational_mining/roles/variants/pandas.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:34.800025 pm4py-2.7.9.3/pm4py/algo/organizational_mining/sna/
--rw-rw-rw-   0        0        0      810 2023-12-11 09:33:52.000000 pm4py-2.7.9.3/pm4py/algo/organizational_mining/sna/__init__.py
--rw-rw-rw-   0        0        0     3689 2023-12-11 09:33:52.000000 pm4py-2.7.9.3/pm4py/algo/organizational_mining/sna/algorithm.py
--rw-rw-rw-   0        0        0     3199 2023-12-11 09:33:52.000000 pm4py-2.7.9.3/pm4py/algo/organizational_mining/sna/util.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:34.812493 pm4py-2.7.9.3/pm4py/algo/organizational_mining/sna/variants/
--rw-rw-rw-   0        0        0      805 2023-12-11 09:33:52.000000 pm4py-2.7.9.3/pm4py/algo/organizational_mining/sna/variants/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:34.865280 pm4py-2.7.9.3/pm4py/algo/organizational_mining/sna/variants/log/
--rw-rw-rw-   0        0        0      857 2023-12-11 09:33:52.000000 pm4py-2.7.9.3/pm4py/algo/organizational_mining/sna/variants/log/__init__.py
--rw-rw-rw-   0        0        0     3735 2023-12-11 09:33:52.000000 pm4py-2.7.9.3/pm4py/algo/organizational_mining/sna/variants/log/handover.py
--rw-rw-rw-   0        0        0     3286 2023-12-11 09:33:52.000000 pm4py-2.7.9.3/pm4py/algo/organizational_mining/sna/variants/log/jointactivities.py
--rw-rw-rw-   0        0        0     3525 2023-12-11 09:33:52.000000 pm4py-2.7.9.3/pm4py/algo/organizational_mining/sna/variants/log/subcontracting.py
--rw-rw-rw-   0        0        0     3155 2023-12-11 09:33:52.000000 pm4py-2.7.9.3/pm4py/algo/organizational_mining/sna/variants/log/working_together.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:34.921614 pm4py-2.7.9.3/pm4py/algo/organizational_mining/sna/variants/pandas/
--rw-rw-rw-   0        0        0      860 2023-12-11 09:33:52.000000 pm4py-2.7.9.3/pm4py/algo/organizational_mining/sna/variants/pandas/__init__.py
--rw-rw-rw-   0        0        0     4235 2023-12-11 09:33:52.000000 pm4py-2.7.9.3/pm4py/algo/organizational_mining/sna/variants/pandas/handover.py
--rw-rw-rw-   0        0        0     2998 2024-01-15 12:00:43.000000 pm4py-2.7.9.3/pm4py/algo/organizational_mining/sna/variants/pandas/jointactivities.py
--rw-rw-rw-   0        0        0     3804 2023-12-11 09:33:52.000000 pm4py-2.7.9.3/pm4py/algo/organizational_mining/sna/variants/pandas/subcontracting.py
--rw-rw-rw-   0        0        0     3432 2023-12-11 09:33:52.000000 pm4py-2.7.9.3/pm4py/algo/organizational_mining/sna/variants/pandas/working_together.py
--rw-rw-rw-   0        0        0     7667 2024-01-02 13:29:21.000000 pm4py-2.7.9.3/pm4py/algo/organizational_mining/util.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:34.923728 pm4py-2.7.9.3/pm4py/algo/querying/
--rw-rw-rw-   0        0        0      736 2023-12-11 09:33:52.000000 pm4py-2.7.9.3/pm4py/algo/querying/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:34.935515 pm4py-2.7.9.3/pm4py/algo/querying/llm/
--rw-rw-rw-   0        0        0      798 2023-12-11 09:33:52.000000 pm4py-2.7.9.3/pm4py/algo/querying/llm/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:35.079361 pm4py-2.7.9.3/pm4py/algo/querying/llm/abstractions/
--rw-rw-rw-   0        0        0      960 2023-12-11 09:33:52.000000 pm4py-2.7.9.3/pm4py/algo/querying/llm/abstractions/__init__.py
--rw-rw-rw-   0        0        0     4006 2023-12-11 09:33:52.000000 pm4py-2.7.9.3/pm4py/algo/querying/llm/abstractions/case_to_descr.py
--rw-rw-rw-   0        0        0     4382 2024-01-12 06:34:29.000000 pm4py-2.7.9.3/pm4py/algo/querying/llm/abstractions/declare_to_descr.py
--rw-rw-rw-   0        0        0     3100 2023-12-11 09:33:52.000000 pm4py-2.7.9.3/pm4py/algo/querying/llm/abstractions/log_to_cols_descr.py
--rw-rw-rw-   0        0        0     9696 2023-12-11 09:33:52.000000 pm4py-2.7.9.3/pm4py/algo/querying/llm/abstractions/log_to_dfg_descr.py
--rw-rw-rw-   0        0        0     7886 2024-01-02 13:29:21.000000 pm4py-2.7.9.3/pm4py/algo/querying/llm/abstractions/log_to_fea_descr.py
--rw-rw-rw-   0        0        0    10693 2024-01-02 13:29:21.000000 pm4py-2.7.9.3/pm4py/algo/querying/llm/abstractions/log_to_variants_descr.py
--rw-rw-rw-   0        0        0     3241 2024-01-12 06:34:29.000000 pm4py-2.7.9.3/pm4py/algo/querying/llm/abstractions/logske_to_descr.py
--rw-rw-rw-   0        0        0     1931 2023-12-11 09:33:52.000000 pm4py-2.7.9.3/pm4py/algo/querying/llm/abstractions/net_to_descr.py
--rw-rw-rw-   0        0        0     6145 2023-12-11 09:33:52.000000 pm4py-2.7.9.3/pm4py/algo/querying/llm/abstractions/ocel_fea_descr.py
--rw-rw-rw-   0        0        0     3680 2023-12-11 09:33:52.000000 pm4py-2.7.9.3/pm4py/algo/querying/llm/abstractions/ocel_ocdfg_descr.py
--rw-rw-rw-   0        0        0     3004 2023-12-11 09:33:52.000000 pm4py-2.7.9.3/pm4py/algo/querying/llm/abstractions/stream_to_descr.py
--rw-rw-rw-   0        0        0     2481 2024-01-12 06:34:29.000000 pm4py-2.7.9.3/pm4py/algo/querying/llm/abstractions/tempprofile_to_descr.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:35.101123 pm4py-2.7.9.3/pm4py/algo/querying/llm/connectors/
--rw-rw-rw-   0        0        0      791 2023-12-11 09:33:52.000000 pm4py-2.7.9.3/pm4py/algo/querying/llm/connectors/__init__.py
--rw-rw-rw-   0        0        0     2596 2024-01-02 13:29:21.000000 pm4py-2.7.9.3/pm4py/algo/querying/llm/connectors/openai.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:35.127363 pm4py-2.7.9.3/pm4py/algo/querying/llm/utils/
--rw-rw-rw-   0        0        0      787 2024-01-02 13:29:21.000000 pm4py-2.7.9.3/pm4py/algo/querying/llm/utils/__init__.py
--rw-rw-rw-   0        0        0     1634 2024-01-02 13:29:21.000000 pm4py-2.7.9.3/pm4py/algo/querying/llm/utils/sql_utils.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:35.142972 pm4py-2.7.9.3/pm4py/algo/reduction/
--rw-rw-rw-   0        0        0      955 2023-12-11 09:33:52.000000 pm4py-2.7.9.3/pm4py/algo/reduction/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:35.164533 pm4py-2.7.9.3/pm4py/algo/reduction/process_tree/
--rw-rw-rw-   0        0        0      799 2023-12-11 09:33:52.000000 pm4py-2.7.9.3/pm4py/algo/reduction/process_tree/__init__.py
--rw-rw-rw-   0        0        0     1601 2023-12-11 09:33:52.000000 pm4py-2.7.9.3/pm4py/algo/reduction/process_tree/reducer.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:35.188318 pm4py-2.7.9.3/pm4py/algo/reduction/process_tree/variants/
--rw-rw-rw-   0        0        0      804 2023-12-11 09:33:52.000000 pm4py-2.7.9.3/pm4py/algo/reduction/process_tree/variants/__init__.py
--rw-rw-rw-   0        0        0     3743 2023-12-11 09:33:52.000000 pm4py-2.7.9.3/pm4py/algo/reduction/process_tree/variants/tree_tr_based.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:35.200966 pm4py-2.7.9.3/pm4py/algo/simulation/
--rw-rw-rw-   0        0        0      904 2023-12-11 09:33:52.000000 pm4py-2.7.9.3/pm4py/algo/simulation/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:35.225511 pm4py-2.7.9.3/pm4py/algo/simulation/montecarlo/
--rw-rw-rw-   0        0        0      995 2023-12-11 09:33:52.000000 pm4py-2.7.9.3/pm4py/algo/simulation/montecarlo/__init__.py
--rw-rw-rw-   0        0        0     4562 2023-12-11 09:33:52.000000 pm4py-2.7.9.3/pm4py/algo/simulation/montecarlo/algorithm.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:35.248719 pm4py-2.7.9.3/pm4py/algo/simulation/montecarlo/utils/
--rw-rw-rw-   0        0        0      793 2023-12-11 09:33:52.000000 pm4py-2.7.9.3/pm4py/algo/simulation/montecarlo/utils/__init__.py
--rw-rw-rw-   0        0        0     5316 2023-12-11 09:33:52.000000 pm4py-2.7.9.3/pm4py/algo/simulation/montecarlo/utils/replay.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:35.274134 pm4py-2.7.9.3/pm4py/algo/simulation/montecarlo/variants/
--rw-rw-rw-   0        0        0      807 2023-12-11 09:33:52.000000 pm4py-2.7.9.3/pm4py/algo/simulation/montecarlo/variants/__init__.py
--rw-rw-rw-   0        0        0    19853 2024-01-02 13:29:21.000000 pm4py-2.7.9.3/pm4py/algo/simulation/montecarlo/variants/petri_semaph_fifo.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:35.285381 pm4py-2.7.9.3/pm4py/algo/simulation/playout/
--rw-rw-rw-   0        0        0      806 2023-12-11 09:33:52.000000 pm4py-2.7.9.3/pm4py/algo/simulation/playout/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:35.310315 pm4py-2.7.9.3/pm4py/algo/simulation/playout/dfg/
--rw-rw-rw-   0        0        0      801 2023-12-11 09:33:52.000000 pm4py-2.7.9.3/pm4py/algo/simulation/playout/dfg/__init__.py
--rw-rw-rw-   0        0        0     1940 2023-12-11 09:33:52.000000 pm4py-2.7.9.3/pm4py/algo/simulation/playout/dfg/algorithm.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:35.345447 pm4py-2.7.9.3/pm4py/algo/simulation/playout/dfg/variants/
--rw-rw-rw-   0        0        0      811 2023-12-11 09:33:52.000000 pm4py-2.7.9.3/pm4py/algo/simulation/playout/dfg/variants/__init__.py
--rw-rw-rw-   0        0        0    14627 2024-01-02 13:29:21.000000 pm4py-2.7.9.3/pm4py/algo/simulation/playout/dfg/variants/classic.py
--rw-rw-rw-   0        0        0     6099 2024-01-02 13:29:21.000000 pm4py-2.7.9.3/pm4py/algo/simulation/playout/dfg/variants/performance.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:35.367580 pm4py-2.7.9.3/pm4py/algo/simulation/playout/petri_net/
--rw-rw-rw-   0        0        0      807 2023-12-11 09:33:52.000000 pm4py-2.7.9.3/pm4py/algo/simulation/playout/petri_net/__init__.py
--rw-rw-rw-   0        0        0     2552 2023-12-11 09:33:52.000000 pm4py-2.7.9.3/pm4py/algo/simulation/playout/petri_net/algorithm.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:35.415441 pm4py-2.7.9.3/pm4py/algo/simulation/playout/petri_net/variants/
--rw-rw-rw-   0        0        0      821 2023-12-11 09:33:52.000000 pm4py-2.7.9.3/pm4py/algo/simulation/playout/petri_net/variants/__init__.py
--rw-rw-rw-   0        0        0     9126 2024-01-02 13:29:21.000000 pm4py-2.7.9.3/pm4py/algo/simulation/playout/petri_net/variants/basic_playout.py
--rw-rw-rw-   0        0        0     5306 2024-01-02 13:29:21.000000 pm4py-2.7.9.3/pm4py/algo/simulation/playout/petri_net/variants/extensive.py
--rw-rw-rw-   0        0        0     8008 2024-01-02 13:29:21.000000 pm4py-2.7.9.3/pm4py/algo/simulation/playout/petri_net/variants/stochastic_playout.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:35.438980 pm4py-2.7.9.3/pm4py/algo/simulation/playout/process_tree/
--rw-rw-rw-   0        0        0      810 2023-12-11 09:33:52.000000 pm4py-2.7.9.3/pm4py/algo/simulation/playout/process_tree/__init__.py
--rw-rw-rw-   0        0        0     1862 2023-12-11 09:33:52.000000 pm4py-2.7.9.3/pm4py/algo/simulation/playout/process_tree/algorithm.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:35.487432 pm4py-2.7.9.3/pm4py/algo/simulation/playout/process_tree/variants/
--rw-rw-rw-   0        0        0      835 2023-12-11 09:33:52.000000 pm4py-2.7.9.3/pm4py/algo/simulation/playout/process_tree/variants/__init__.py
--rw-rw-rw-   0        0        0     1679 2023-12-11 09:33:52.000000 pm4py-2.7.9.3/pm4py/algo/simulation/playout/process_tree/variants/basic_playout.py
--rw-rw-rw-   0        0        0    13571 2023-12-11 09:33:52.000000 pm4py-2.7.9.3/pm4py/algo/simulation/playout/process_tree/variants/extensive.py
--rw-rw-rw-   0        0        0     4861 2023-12-11 09:33:52.000000 pm4py-2.7.9.3/pm4py/algo/simulation/playout/process_tree/variants/topbottom.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:35.509831 pm4py-2.7.9.3/pm4py/algo/simulation/tree_generator/
--rw-rw-rw-   0        0        0      806 2023-12-11 09:33:52.000000 pm4py-2.7.9.3/pm4py/algo/simulation/tree_generator/__init__.py
--rw-rw-rw-   0        0        0     1765 2023-12-11 09:33:52.000000 pm4py-2.7.9.3/pm4py/algo/simulation/tree_generator/algorithm.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:35.547536 pm4py-2.7.9.3/pm4py/algo/simulation/tree_generator/variants/
--rw-rw-rw-   0        0        0      818 2023-12-11 09:33:52.000000 pm4py-2.7.9.3/pm4py/algo/simulation/tree_generator/variants/__init__.py
--rw-rw-rw-   0        0        0     5357 2023-12-11 09:33:52.000000 pm4py-2.7.9.3/pm4py/algo/simulation/tree_generator/variants/basic.py
--rw-rw-rw-   0        0        0    12955 2023-12-11 09:33:52.000000 pm4py-2.7.9.3/pm4py/algo/simulation/tree_generator/variants/ptandloggenerator.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:35.560694 pm4py-2.7.9.3/pm4py/algo/transformation/
--rw-rw-rw-   0        0        0      808 2023-12-11 09:33:52.000000 pm4py-2.7.9.3/pm4py/algo/transformation/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:35.582469 pm4py-2.7.9.3/pm4py/algo/transformation/log_to_features/
--rw-rw-rw-   0        0        0      809 2023-12-11 09:33:52.000000 pm4py-2.7.9.3/pm4py/algo/transformation/log_to_features/__init__.py
--rw-rw-rw-   0        0        0     2205 2023-12-11 09:33:52.000000 pm4py-2.7.9.3/pm4py/algo/transformation/log_to_features/algorithm.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:35.606177 pm4py-2.7.9.3/pm4py/algo/transformation/log_to_features/util/
--rw-rw-rw-   0        0        0      819 2023-12-11 09:33:52.000000 pm4py-2.7.9.3/pm4py/algo/transformation/log_to_features/util/__init__.py
--rw-rw-rw-   0        0        0     3933 2024-01-02 13:29:21.000000 pm4py-2.7.9.3/pm4py/algo/transformation/log_to_features/util/locally_linear_embedding.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:35.653197 pm4py-2.7.9.3/pm4py/algo/transformation/log_to_features/variants/
--rw-rw-rw-   0        0        0      823 2023-12-11 09:33:52.000000 pm4py-2.7.9.3/pm4py/algo/transformation/log_to_features/variants/__init__.py
--rw-rw-rw-   0        0        0     6689 2023-12-11 09:33:52.000000 pm4py-2.7.9.3/pm4py/algo/transformation/log_to_features/variants/event_based.py
--rw-rw-rw-   0        0        0     6644 2024-01-15 12:00:43.000000 pm4py-2.7.9.3/pm4py/algo/transformation/log_to_features/variants/temporal.py
--rw-rw-rw-   0        0        0    50368 2024-01-02 13:29:21.000000 pm4py-2.7.9.3/pm4py/algo/transformation/log_to_features/variants/trace_based.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:35.675841 pm4py-2.7.9.3/pm4py/algo/transformation/log_to_interval_tree/
--rw-rw-rw-   0        0        0      999 2023-12-11 09:33:52.000000 pm4py-2.7.9.3/pm4py/algo/transformation/log_to_interval_tree/__init__.py
--rw-rw-rw-   0        0        0     2171 2023-12-11 09:33:52.000000 pm4py-2.7.9.3/pm4py/algo/transformation/log_to_interval_tree/algorithm.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:35.698613 pm4py-2.7.9.3/pm4py/algo/transformation/log_to_interval_tree/variants/
--rw-rw-rw-   0        0        0      814 2023-12-11 09:33:52.000000 pm4py-2.7.9.3/pm4py/algo/transformation/log_to_interval_tree/variants/__init__.py
--rw-rw-rw-   0        0        0     6365 2023-12-11 09:33:52.000000 pm4py-2.7.9.3/pm4py/algo/transformation/log_to_interval_tree/variants/open_paths.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:35.721449 pm4py-2.7.9.3/pm4py/algo/transformation/log_to_target/
--rw-rw-rw-   0        0        0      807 2023-12-11 09:33:52.000000 pm4py-2.7.9.3/pm4py/algo/transformation/log_to_target/__init__.py
--rw-rw-rw-   0        0        0     2161 2023-12-11 09:33:52.000000 pm4py-2.7.9.3/pm4py/algo/transformation/log_to_target/algorithm.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:35.765130 pm4py-2.7.9.3/pm4py/algo/transformation/log_to_target/variants/
--rw-rw-rw-   0        0        0      837 2023-12-11 09:33:52.000000 pm4py-2.7.9.3/pm4py/algo/transformation/log_to_target/variants/__init__.py
--rw-rw-rw-   0        0        0     2922 2023-12-11 09:33:52.000000 pm4py-2.7.9.3/pm4py/algo/transformation/log_to_target/variants/next_activity.py
--rw-rw-rw-   0        0        0     2526 2023-12-11 09:33:52.000000 pm4py-2.7.9.3/pm4py/algo/transformation/log_to_target/variants/next_time.py
--rw-rw-rw-   0        0        0     2385 2023-12-11 09:33:52.000000 pm4py-2.7.9.3/pm4py/algo/transformation/log_to_target/variants/remaining_time.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:35.787729 pm4py-2.7.9.3/pm4py/algo/transformation/log_to_trie/
--rw-rw-rw-   0        0        0      795 2023-12-11 09:33:52.000000 pm4py-2.7.9.3/pm4py/algo/transformation/log_to_trie/__init__.py
--rw-rw-rw-   0        0        0     2261 2024-01-02 13:29:21.000000 pm4py-2.7.9.3/pm4py/algo/transformation/log_to_trie/algorithm.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:35.799547 pm4py-2.7.9.3/pm4py/algo/transformation/ocel/
--rw-rw-rw-   0        0        0      807 2023-12-11 09:33:52.000000 pm4py-2.7.9.3/pm4py/algo/transformation/ocel/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:35.813350 pm4py-2.7.9.3/pm4py/algo/transformation/ocel/description/
--rw-rw-rw-   0        0        0      736 2023-12-11 09:33:52.000000 pm4py-2.7.9.3/pm4py/algo/transformation/ocel/description/__init__.py
--rw-rw-rw-   0        0        0     1684 2023-12-11 09:33:52.000000 pm4py-2.7.9.3/pm4py/algo/transformation/ocel/description/algorithm.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:35.827397 pm4py-2.7.9.3/pm4py/algo/transformation/ocel/description/variants/
--rw-rw-rw-   0        0        0      736 2023-12-11 09:33:52.000000 pm4py-2.7.9.3/pm4py/algo/transformation/ocel/description/variants/__init__.py
--rw-rw-rw-   0        0        0     3318 2023-12-11 09:33:52.000000 pm4py-2.7.9.3/pm4py/algo/transformation/ocel/description/variants/variant1.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:35.839731 pm4py-2.7.9.3/pm4py/algo/transformation/ocel/features/
--rw-rw-rw-   0        0        0      821 2023-12-11 09:33:52.000000 pm4py-2.7.9.3/pm4py/algo/transformation/ocel/features/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:35.966997 pm4py-2.7.9.3/pm4py/algo/transformation/ocel/features/events/
--rw-rw-rw-   0        0        0     1002 2023-12-11 09:33:52.000000 pm4py-2.7.9.3/pm4py/algo/transformation/ocel/features/events/__init__.py
--rw-rw-rw-   0        0        0     9094 2024-01-02 13:29:21.000000 pm4py-2.7.9.3/pm4py/algo/transformation/ocel/features/events/algorithm.py
--rw-rw-rw-   0        0        0     2022 2024-01-02 13:29:21.000000 pm4py-2.7.9.3/pm4py/algo/transformation/ocel/features/events/event_activity.py
--rw-rw-rw-   0        0        0     2250 2024-01-02 13:29:21.000000 pm4py-2.7.9.3/pm4py/algo/transformation/ocel/features/events/event_end_ot.py
--rw-rw-rw-   0        0        0     2542 2024-01-02 13:29:21.000000 pm4py-2.7.9.3/pm4py/algo/transformation/ocel/features/events/event_num_attributes.py
--rw-rw-rw-   0        0        0     1691 2024-01-02 13:29:21.000000 pm4py-2.7.9.3/pm4py/algo/transformation/ocel/features/events/event_num_rel_objs.py
--rw-rw-rw-   0        0        0     2354 2024-01-02 13:29:21.000000 pm4py-2.7.9.3/pm4py/algo/transformation/ocel/features/events/event_num_rel_objs_type.py
--rw-rw-rw-   0        0        0     2236 2024-01-02 13:29:21.000000 pm4py-2.7.9.3/pm4py/algo/transformation/ocel/features/events/event_start_ot.py
--rw-rw-rw-   0        0        0     3041 2024-01-02 13:29:21.000000 pm4py-2.7.9.3/pm4py/algo/transformation/ocel/features/events/event_str_attributes.py
--rw-rw-rw-   0        0        0     2031 2024-01-02 13:29:21.000000 pm4py-2.7.9.3/pm4py/algo/transformation/ocel/features/events/event_timestamp.py
--rw-rw-rw-   0        0        0     1990 2024-01-02 13:29:21.000000 pm4py-2.7.9.3/pm4py/algo/transformation/ocel/features/events/new_interactions.py
--rw-rw-rw-   0        0        0     2805 2024-01-02 13:29:21.000000 pm4py-2.7.9.3/pm4py/algo/transformation/ocel/features/events/related_objects_features.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:36.000387 pm4py-2.7.9.3/pm4py/algo/transformation/ocel/features/events_objects/
--rw-rw-rw-   0        0        0      831 2023-12-11 09:33:52.000000 pm4py-2.7.9.3/pm4py/algo/transformation/ocel/features/events_objects/__init__.py
--rw-rw-rw-   0        0        0     3899 2024-01-02 13:29:21.000000 pm4py-2.7.9.3/pm4py/algo/transformation/ocel/features/events_objects/algorithm.py
--rw-rw-rw-   0        0        0     4959 2024-01-02 13:29:21.000000 pm4py-2.7.9.3/pm4py/algo/transformation/ocel/features/events_objects/prefix_features.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:36.231386 pm4py-2.7.9.3/pm4py/algo/transformation/ocel/features/objects/
--rw-rw-rw-   0        0        0     1268 2023-12-11 09:33:52.000000 pm4py-2.7.9.3/pm4py/algo/transformation/ocel/features/objects/__init__.py
--rw-rw-rw-   0        0        0    20532 2024-01-02 13:29:21.000000 pm4py-2.7.9.3/pm4py/algo/transformation/ocel/features/objects/algorithm.py
--rw-rw-rw-   0        0        0     3400 2024-01-02 13:29:21.000000 pm4py-2.7.9.3/pm4py/algo/transformation/ocel/features/objects/obj_con_in_graph_features.py
--rw-rw-rw-   0        0        0     1912 2024-01-02 13:29:21.000000 pm4py-2.7.9.3/pm4py/algo/transformation/ocel/features/objects/object_cobirth_graph.py
--rw-rw-rw-   0        0        0     1912 2024-01-02 13:29:21.000000 pm4py-2.7.9.3/pm4py/algo/transformation/ocel/features/objects/object_codeath_graph.py
--rw-rw-rw-   0        0        0     1988 2024-01-02 13:29:21.000000 pm4py-2.7.9.3/pm4py/algo/transformation/ocel/features/objects/object_degree_centrality.py
--rw-rw-rw-   0        0        0     2100 2024-01-02 13:29:21.000000 pm4py-2.7.9.3/pm4py/algo/transformation/ocel/features/objects/object_general_descendants_graph.py
--rw-rw-rw-   0        0        0     2152 2024-01-02 13:29:21.000000 pm4py-2.7.9.3/pm4py/algo/transformation/ocel/features/objects/object_general_inheritance_graph.py
--rw-rw-rw-   0        0        0     1942 2024-01-02 13:29:21.000000 pm4py-2.7.9.3/pm4py/algo/transformation/ocel/features/objects/object_general_interaction_graph.py
--rw-rw-rw-   0        0        0     2080 2024-01-02 13:29:21.000000 pm4py-2.7.9.3/pm4py/algo/transformation/ocel/features/objects/object_lifecycle_activities.py
--rw-rw-rw-   0        0        0     2197 2024-01-02 13:29:21.000000 pm4py-2.7.9.3/pm4py/algo/transformation/ocel/features/objects/object_lifecycle_duration.py
--rw-rw-rw-   0        0        0     1794 2024-01-02 13:29:21.000000 pm4py-2.7.9.3/pm4py/algo/transformation/ocel/features/objects/object_lifecycle_length.py
--rw-rw-rw-   0        0        0     2205 2024-01-02 13:29:21.000000 pm4py-2.7.9.3/pm4py/algo/transformation/ocel/features/objects/object_lifecycle_paths.py
--rw-rw-rw-   0        0        0     1920 2024-01-02 13:29:21.000000 pm4py-2.7.9.3/pm4py/algo/transformation/ocel/features/objects/object_lifecycle_unq_act.py
--rw-rw-rw-   0        0        0     2586 2024-01-02 13:29:21.000000 pm4py-2.7.9.3/pm4py/algo/transformation/ocel/features/objects/object_num_attributes.py
--rw-rw-rw-   0        0        0     3062 2024-01-02 13:29:21.000000 pm4py-2.7.9.3/pm4py/algo/transformation/ocel/features/objects/object_str_attributes.py
--rw-rw-rw-   0        0        0     2455 2024-01-02 13:29:21.000000 pm4py-2.7.9.3/pm4py/algo/transformation/ocel/features/objects/object_work_in_progress.py
--rw-rw-rw-   0        0        0     2486 2024-01-02 13:29:21.000000 pm4py-2.7.9.3/pm4py/algo/transformation/ocel/features/objects/objects_interaction_graph_ot.py
--rw-rw-rw-   0        0        0     3063 2024-01-02 13:29:21.000000 pm4py-2.7.9.3/pm4py/algo/transformation/ocel/features/objects/related_activities_features.py
--rw-rw-rw-   0        0        0     2788 2024-01-02 13:29:21.000000 pm4py-2.7.9.3/pm4py/algo/transformation/ocel/features/objects/related_events_features.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:36.305474 pm4py-2.7.9.3/pm4py/algo/transformation/ocel/graphs/
--rw-rw-rw-   0        0        0      906 2023-12-11 09:33:52.000000 pm4py-2.7.9.3/pm4py/algo/transformation/ocel/graphs/__init__.py
--rw-rw-rw-   0        0        0     2305 2024-01-02 13:29:21.000000 pm4py-2.7.9.3/pm4py/algo/transformation/ocel/graphs/object_cobirth_graph.py
--rw-rw-rw-   0        0        0     2103 2024-01-02 13:29:21.000000 pm4py-2.7.9.3/pm4py/algo/transformation/ocel/graphs/object_codeath_graph.py
--rw-rw-rw-   0        0        0     2327 2024-01-02 13:29:21.000000 pm4py-2.7.9.3/pm4py/algo/transformation/ocel/graphs/object_descendants_graph.py
--rw-rw-rw-   0        0        0     2852 2024-01-02 13:29:21.000000 pm4py-2.7.9.3/pm4py/algo/transformation/ocel/graphs/object_inheritance_graph.py
--rw-rw-rw-   0        0        0     1736 2024-01-02 13:29:21.000000 pm4py-2.7.9.3/pm4py/algo/transformation/ocel/graphs/object_interaction_graph.py
--rw-rw-rw-   0        0        0     3641 2024-01-02 13:29:21.000000 pm4py-2.7.9.3/pm4py/algo/transformation/ocel/graphs/ocel20_computation.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:36.327616 pm4py-2.7.9.3/pm4py/algo/transformation/ocel/split_ocel/
--rw-rw-rw-   0        0        0      809 2023-12-11 09:33:52.000000 pm4py-2.7.9.3/pm4py/algo/transformation/ocel/split_ocel/__init__.py
--rw-rw-rw-   0        0        0     1730 2023-12-11 09:33:52.000000 pm4py-2.7.9.3/pm4py/algo/transformation/ocel/split_ocel/algorithm.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:36.361196 pm4py-2.7.9.3/pm4py/algo/transformation/ocel/split_ocel/variants/
--rw-rw-rw-   0        0        0      819 2023-12-11 09:33:52.000000 pm4py-2.7.9.3/pm4py/algo/transformation/ocel/split_ocel/variants/__init__.py
--rw-rw-rw-   0        0        0     3429 2024-01-02 13:29:21.000000 pm4py-2.7.9.3/pm4py/algo/transformation/ocel/split_ocel/variants/ancestors_descendants.py
--rw-rw-rw-   0        0        0     3467 2024-01-02 13:29:21.000000 pm4py-2.7.9.3/pm4py/algo/transformation/ocel/split_ocel/variants/connected_components.py
--rw-rw-rw-   0        0        0    20646 2023-12-11 09:33:52.000000 pm4py-2.7.9.3/pm4py/analysis.py
--rw-rw-rw-   0        0        0    13471 2024-01-02 13:29:21.000000 pm4py-2.7.9.3/pm4py/cli.py
--rw-rw-rw-   0        0        0    48213 2024-01-02 13:29:21.000000 pm4py-2.7.9.3/pm4py/conformance.py
--rw-rw-rw-   0        0        0    19636 2023-12-11 09:33:52.000000 pm4py-2.7.9.3/pm4py/connectors.py
--rw-rw-rw-   0        0        0    20826 2023-12-11 09:33:52.000000 pm4py-2.7.9.3/pm4py/convert.py
--rw-rw-rw-   0        0        0    47943 2024-01-02 13:29:21.000000 pm4py-2.7.9.3/pm4py/discovery.py
--rw-rw-rw-   0        0        0    63155 2024-01-15 12:00:43.000000 pm4py-2.7.9.3/pm4py/filtering.py
--rw-rw-rw-   0        0        0     5192 2023-12-11 09:33:52.000000 pm4py-2.7.9.3/pm4py/hof.py
--rw-rw-rw-   0        0        0    18976 2024-01-04 13:34:19.000000 pm4py-2.7.9.3/pm4py/llm.py
--rw-rw-rw-   0        0        0     1091 2024-01-16 10:09:19.000000 pm4py-2.7.9.3/pm4py/meta.py
--rw-rw-rw-   0        0        0    16160 2024-01-02 13:29:21.000000 pm4py-2.7.9.3/pm4py/ml.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:36.373765 pm4py-2.7.9.3/pm4py/objects/
--rw-rw-rw-   0        0        0      947 2023-12-11 09:33:52.000000 pm4py-2.7.9.3/pm4py/objects/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:36.407907 pm4py-2.7.9.3/pm4py/objects/bpmn/
--rw-rw-rw-   0        0        0      913 2023-12-11 09:33:52.000000 pm4py-2.7.9.3/pm4py/objects/bpmn/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:36.429853 pm4py-2.7.9.3/pm4py/objects/bpmn/exporter/
--rw-rw-rw-   0        0        0      794 2023-12-11 09:33:52.000000 pm4py-2.7.9.3/pm4py/objects/bpmn/exporter/__init__.py
--rw-rw-rw-   0        0        0     2130 2023-12-11 09:33:52.000000 pm4py-2.7.9.3/pm4py/objects/bpmn/exporter/exporter.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:36.454072 pm4py-2.7.9.3/pm4py/objects/bpmn/exporter/variants/
--rw-rw-rw-   0        0        0      790 2023-12-11 09:33:52.000000 pm4py-2.7.9.3/pm4py/objects/bpmn/exporter/variants/__init__.py
--rw-rw-rw-   0        0        0     7688 2024-01-02 13:29:21.000000 pm4py-2.7.9.3/pm4py/objects/bpmn/exporter/variants/etree.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:36.475586 pm4py-2.7.9.3/pm4py/objects/bpmn/importer/
--rw-rw-rw-   0        0        0      794 2023-12-11 09:33:52.000000 pm4py-2.7.9.3/pm4py/objects/bpmn/importer/__init__.py
--rw-rw-rw-   0        0        0     2085 2023-12-11 09:33:52.000000 pm4py-2.7.9.3/pm4py/objects/bpmn/importer/importer.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:36.498944 pm4py-2.7.9.3/pm4py/objects/bpmn/importer/variants/
--rw-rw-rw-   0        0        0      789 2023-12-11 09:33:52.000000 pm4py-2.7.9.3/pm4py/objects/bpmn/importer/variants/__init__.py
--rw-rw-rw-   0        0        0    17373 2023-12-11 09:33:52.000000 pm4py-2.7.9.3/pm4py/objects/bpmn/importer/variants/lxml.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:36.522281 pm4py-2.7.9.3/pm4py/objects/bpmn/layout/
--rw-rw-rw-   0        0        0      792 2023-12-11 09:33:52.000000 pm4py-2.7.9.3/pm4py/objects/bpmn/layout/__init__.py
--rw-rw-rw-   0        0        0     1534 2023-12-11 09:33:52.000000 pm4py-2.7.9.3/pm4py/objects/bpmn/layout/layouter.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:36.545267 pm4py-2.7.9.3/pm4py/objects/bpmn/layout/variants/
--rw-rw-rw-   0        0        0      793 2023-12-11 09:33:52.000000 pm4py-2.7.9.3/pm4py/objects/bpmn/layout/variants/__init__.py
--rw-rw-rw-   0        0        0    18042 2023-12-11 09:33:52.000000 pm4py-2.7.9.3/pm4py/objects/bpmn/layout/variants/graphviz.py
--rw-rw-rw-   0        0        0    19676 2023-12-11 09:33:52.000000 pm4py-2.7.9.3/pm4py/objects/bpmn/obj.py
--rw-rw-rw-   0        0        0     9205 2023-12-11 09:33:52.000000 pm4py-2.7.9.3/pm4py/objects/bpmn/semantics.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:36.590433 pm4py-2.7.9.3/pm4py/objects/bpmn/util/
--rw-rw-rw-   0        0        0      802 2023-12-11 09:33:52.000000 pm4py-2.7.9.3/pm4py/objects/bpmn/util/__init__.py
--rw-rw-rw-   0        0        0     6246 2023-12-11 09:33:52.000000 pm4py-2.7.9.3/pm4py/objects/bpmn/util/bpmn_utils.py
--rw-rw-rw-   0        0        0     3352 2023-12-11 09:33:52.000000 pm4py-2.7.9.3/pm4py/objects/bpmn/util/reduction.py
--rw-rw-rw-   0        0        0     3729 2023-12-11 09:33:52.000000 pm4py-2.7.9.3/pm4py/objects/bpmn/util/sorting.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:36.601856 pm4py-2.7.9.3/pm4py/objects/conversion/
--rw-rw-rw-   0        0        0      825 2023-12-11 09:33:52.000000 pm4py-2.7.9.3/pm4py/objects/conversion/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:36.624597 pm4py-2.7.9.3/pm4py/objects/conversion/bpmn/
--rw-rw-rw-   0        0        0      797 2023-12-11 09:33:52.000000 pm4py-2.7.9.3/pm4py/objects/conversion/bpmn/__init__.py
--rw-rw-rw-   0        0        0     1160 2023-12-11 09:33:52.000000 pm4py-2.7.9.3/pm4py/objects/conversion/bpmn/converter.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:36.648892 pm4py-2.7.9.3/pm4py/objects/conversion/bpmn/variants/
--rw-rw-rw-   0        0        0      799 2023-12-11 09:33:52.000000 pm4py-2.7.9.3/pm4py/objects/conversion/bpmn/variants/__init__.py
--rw-rw-rw-   0        0        0    10026 2023-12-11 09:33:52.000000 pm4py-2.7.9.3/pm4py/objects/conversion/bpmn/variants/to_petri_net.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:36.671074 pm4py-2.7.9.3/pm4py/objects/conversion/dfg/
--rw-rw-rw-   0        0        0      796 2023-12-11 09:33:52.000000 pm4py-2.7.9.3/pm4py/objects/conversion/dfg/__init__.py
--rw-rw-rw-   0        0        0     1340 2023-12-11 09:33:52.000000 pm4py-2.7.9.3/pm4py/objects/conversion/dfg/converter.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:36.704631 pm4py-2.7.9.3/pm4py/objects/conversion/dfg/variants/
--rw-rw-rw-   0        0        0      860 2023-12-11 09:33:52.000000 pm4py-2.7.9.3/pm4py/objects/conversion/dfg/variants/__init__.py
--rw-rw-rw-   0        0        0     3494 2023-12-11 09:33:52.000000 pm4py-2.7.9.3/pm4py/objects/conversion/dfg/variants/to_petri_net_activity_defines_place.py
--rw-rw-rw-   0        0        0     4229 2023-12-11 09:33:52.000000 pm4py-2.7.9.3/pm4py/objects/conversion/dfg/variants/to_petri_net_invisibles_no_duplicates.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:36.728391 pm4py-2.7.9.3/pm4py/objects/conversion/heuristics_net/
--rw-rw-rw-   0        0        0      807 2023-12-11 09:33:52.000000 pm4py-2.7.9.3/pm4py/objects/conversion/heuristics_net/__init__.py
--rw-rw-rw-   0        0        0     1384 2023-12-11 09:33:52.000000 pm4py-2.7.9.3/pm4py/objects/conversion/heuristics_net/converter.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:36.753924 pm4py-2.7.9.3/pm4py/objects/conversion/heuristics_net/variants/
--rw-rw-rw-   0        0        0      809 2023-12-11 09:33:52.000000 pm4py-2.7.9.3/pm4py/objects/conversion/heuristics_net/variants/__init__.py
--rw-rw-rw-   0        0        0    11773 2023-12-11 09:33:52.000000 pm4py-2.7.9.3/pm4py/objects/conversion/heuristics_net/variants/to_petri_net.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:36.790033 pm4py-2.7.9.3/pm4py/objects/conversion/log/
--rw-rw-rw-   0        0        0      807 2023-12-11 09:33:52.000000 pm4py-2.7.9.3/pm4py/objects/conversion/log/__init__.py
--rw-rw-rw-   0        0        0     1061 2023-12-11 09:33:52.000000 pm4py-2.7.9.3/pm4py/objects/conversion/log/constants.py
--rw-rw-rw-   0        0        0     1319 2023-12-11 09:33:52.000000 pm4py-2.7.9.3/pm4py/objects/conversion/log/converter.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:36.864775 pm4py-2.7.9.3/pm4py/objects/conversion/log/variants/
--rw-rw-rw-   0        0        0      870 2023-12-11 09:33:52.000000 pm4py-2.7.9.3/pm4py/objects/conversion/log/variants/__init__.py
--rw-rw-rw-   0        0        0     1923 2023-12-11 09:33:52.000000 pm4py-2.7.9.3/pm4py/objects/conversion/log/variants/df_to_event_log_1v.py
--rw-rw-rw-   0        0        0     2535 2023-12-11 09:33:52.000000 pm4py-2.7.9.3/pm4py/objects/conversion/log/variants/df_to_event_log_nv.py
--rw-rw-rw-   0        0        0     2585 2024-01-02 13:29:21.000000 pm4py-2.7.9.3/pm4py/objects/conversion/log/variants/to_data_frame.py
--rw-rw-rw-   0        0        0     4332 2024-01-02 13:29:21.000000 pm4py-2.7.9.3/pm4py/objects/conversion/log/variants/to_event_log.py
--rw-rw-rw-   0        0        0    10224 2024-01-02 13:29:21.000000 pm4py-2.7.9.3/pm4py/objects/conversion/log/variants/to_event_stream.py
--rw-rw-rw-   0        0        0     5236 2023-12-11 09:33:52.000000 pm4py-2.7.9.3/pm4py/objects/conversion/log/variants/to_nx.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:36.887621 pm4py-2.7.9.3/pm4py/objects/conversion/ocel/
--rw-rw-rw-   0        0        0      799 2023-12-11 09:33:52.000000 pm4py-2.7.9.3/pm4py/objects/conversion/ocel/__init__.py
--rw-rw-rw-   0        0        0     1814 2023-12-11 09:33:52.000000 pm4py-2.7.9.3/pm4py/objects/conversion/ocel/converter.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:36.921723 pm4py-2.7.9.3/pm4py/objects/conversion/ocel/variants/
--rw-rw-rw-   0        0        0      820 2023-12-11 09:33:52.000000 pm4py-2.7.9.3/pm4py/objects/conversion/ocel/variants/__init__.py
--rw-rw-rw-   0        0        0     4056 2023-12-11 09:33:52.000000 pm4py-2.7.9.3/pm4py/objects/conversion/ocel/variants/ocel_features_to_nx.py
--rw-rw-rw-   0        0        0     4164 2023-12-11 09:33:52.000000 pm4py-2.7.9.3/pm4py/objects/conversion/ocel/variants/ocel_to_nx.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:36.943328 pm4py-2.7.9.3/pm4py/objects/conversion/powl/
--rw-rw-rw-   0        0        0      781 2023-12-11 09:33:52.000000 pm4py-2.7.9.3/pm4py/objects/conversion/powl/__init__.py
--rw-rw-rw-   0        0        0     1494 2024-01-02 13:29:21.000000 pm4py-2.7.9.3/pm4py/objects/conversion/powl/converter.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:36.970398 pm4py-2.7.9.3/pm4py/objects/conversion/powl/variants/
--rw-rw-rw-   0        0        0      790 2023-12-11 09:33:52.000000 pm4py-2.7.9.3/pm4py/objects/conversion/powl/variants/__init__.py
--rw-rw-rw-   0        0        0    11169 2024-01-02 13:29:21.000000 pm4py-2.7.9.3/pm4py/objects/conversion/powl/variants/to_petri_net.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:36.992470 pm4py-2.7.9.3/pm4py/objects/conversion/process_tree/
--rw-rw-rw-   0        0        0      805 2023-12-11 09:33:52.000000 pm4py-2.7.9.3/pm4py/objects/conversion/process_tree/__init__.py
--rw-rw-rw-   0        0        0     1824 2023-12-11 09:33:52.000000 pm4py-2.7.9.3/pm4py/objects/conversion/process_tree/converter.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:37.037013 pm4py-2.7.9.3/pm4py/objects/conversion/process_tree/variants/
--rw-rw-rw-   0        0        0      850 2023-12-11 09:33:52.000000 pm4py-2.7.9.3/pm4py/objects/conversion/process_tree/variants/__init__.py
--rw-rw-rw-   0        0        0    10139 2023-12-11 09:33:52.000000 pm4py-2.7.9.3/pm4py/objects/conversion/process_tree/variants/to_bpmn.py
--rw-rw-rw-   0        0        0    21550 2023-12-11 09:33:52.000000 pm4py-2.7.9.3/pm4py/objects/conversion/process_tree/variants/to_petri_net.py
--rw-rw-rw-   0        0        0     4772 2023-12-11 09:33:52.000000 pm4py-2.7.9.3/pm4py/objects/conversion/process_tree/variants/to_petri_net_transition_bordered.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:37.060809 pm4py-2.7.9.3/pm4py/objects/conversion/wf_net/
--rw-rw-rw-   0        0        0      799 2023-12-11 09:33:52.000000 pm4py-2.7.9.3/pm4py/objects/conversion/wf_net/__init__.py
--rw-rw-rw-   0        0        0     1167 2023-12-11 09:33:52.000000 pm4py-2.7.9.3/pm4py/objects/conversion/wf_net/converter.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:37.094866 pm4py-2.7.9.3/pm4py/objects/conversion/wf_net/variants/
--rw-rw-rw-   0        0        0      813 2023-12-11 09:33:52.000000 pm4py-2.7.9.3/pm4py/objects/conversion/wf_net/variants/__init__.py
--rw-rw-rw-   0        0        0     3774 2023-12-11 09:33:52.000000 pm4py-2.7.9.3/pm4py/objects/conversion/wf_net/variants/to_bpmn.py
--rw-rw-rw-   0        0        0    10849 2023-12-11 09:33:52.000000 pm4py-2.7.9.3/pm4py/objects/conversion/wf_net/variants/to_process_tree.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:37.128119 pm4py-2.7.9.3/pm4py/objects/dfg/
--rw-rw-rw-   0        0        0      796 2023-12-11 09:33:52.000000 pm4py-2.7.9.3/pm4py/objects/dfg/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:37.150066 pm4py-2.7.9.3/pm4py/objects/dfg/exporter/
--rw-rw-rw-   0        0        0      793 2023-12-11 09:33:52.000000 pm4py-2.7.9.3/pm4py/objects/dfg/exporter/__init__.py
--rw-rw-rw-   0        0        0     2041 2023-12-11 09:33:52.000000 pm4py-2.7.9.3/pm4py/objects/dfg/exporter/exporter.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:37.174377 pm4py-2.7.9.3/pm4py/objects/dfg/exporter/variants/
--rw-rw-rw-   0        0        0      791 2023-12-11 09:33:52.000000 pm4py-2.7.9.3/pm4py/objects/dfg/exporter/variants/__init__.py
--rw-rw-rw-   0        0        0     4571 2023-12-11 09:33:52.000000 pm4py-2.7.9.3/pm4py/objects/dfg/exporter/variants/classic.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:37.190033 pm4py-2.7.9.3/pm4py/objects/dfg/filtering/
--rw-rw-rw-   0        0        0      734 2023-12-11 09:33:52.000000 pm4py-2.7.9.3/pm4py/objects/dfg/filtering/__init__.py
--rw-rw-rw-   0        0        0      788 2023-12-11 09:33:52.000000 pm4py-2.7.9.3/pm4py/objects/dfg/filtering/dfg_filtering.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:37.212651 pm4py-2.7.9.3/pm4py/objects/dfg/importer/
--rw-rw-rw-   0        0        0      793 2023-12-11 09:33:52.000000 pm4py-2.7.9.3/pm4py/objects/dfg/importer/__init__.py
--rw-rw-rw-   0        0        0     2278 2023-12-11 09:33:52.000000 pm4py-2.7.9.3/pm4py/objects/dfg/importer/importer.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:37.236087 pm4py-2.7.9.3/pm4py/objects/dfg/importer/variants/
--rw-rw-rw-   0        0        0      791 2023-12-11 09:33:52.000000 pm4py-2.7.9.3/pm4py/objects/dfg/importer/variants/__init__.py
--rw-rw-rw-   0        0        0     4037 2023-12-11 09:33:52.000000 pm4py-2.7.9.3/pm4py/objects/dfg/importer/variants/classic.py
--rw-rw-rw-   0        0        0     1881 2023-12-11 09:33:52.000000 pm4py-2.7.9.3/pm4py/objects/dfg/obj.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:37.262470 pm4py-2.7.9.3/pm4py/objects/dfg/retrieval/
--rw-rw-rw-   0        0        0      734 2023-12-11 09:33:52.000000 pm4py-2.7.9.3/pm4py/objects/dfg/retrieval/__init__.py
--rw-rw-rw-   0        0        0      913 2023-12-11 09:33:52.000000 pm4py-2.7.9.3/pm4py/objects/dfg/retrieval/log.py
--rw-rw-rw-   0        0        0      873 2023-12-11 09:33:52.000000 pm4py-2.7.9.3/pm4py/objects/dfg/retrieval/pandas.py
--rw-rw-rw-   0        0        0     5092 2023-12-11 09:33:52.000000 pm4py-2.7.9.3/pm4py/objects/dfg/util.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:37.286581 pm4py-2.7.9.3/pm4py/objects/dfg/utils/
--rw-rw-rw-   0        0        0      781 2023-12-11 09:33:52.000000 pm4py-2.7.9.3/pm4py/objects/dfg/utils/__init__.py
--rw-rw-rw-   0        0        0    26490 2023-12-11 09:33:52.000000 pm4py-2.7.9.3/pm4py/objects/dfg/utils/dfg_utils.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:37.343030 pm4py-2.7.9.3/pm4py/objects/heuristics_net/
--rw-rw-rw-   0        0        0      802 2023-12-11 09:33:52.000000 pm4py-2.7.9.3/pm4py/objects/heuristics_net/__init__.py
--rw-rw-rw-   0        0        0     1226 2023-12-11 09:33:52.000000 pm4py-2.7.9.3/pm4py/objects/heuristics_net/defaults.py
--rw-rw-rw-   0        0        0     2689 2023-12-11 09:33:52.000000 pm4py-2.7.9.3/pm4py/objects/heuristics_net/edge.py
--rw-rw-rw-   0        0        0     9877 2023-12-11 09:33:52.000000 pm4py-2.7.9.3/pm4py/objects/heuristics_net/node.py
--rw-rw-rw-   0        0        0     5684 2023-12-11 09:33:52.000000 pm4py-2.7.9.3/pm4py/objects/heuristics_net/obj.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:37.366131 pm4py-2.7.9.3/pm4py/objects/log/
--rw-rw-rw-   0        0        0      795 2023-12-11 09:33:52.000000 pm4py-2.7.9.3/pm4py/objects/log/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:37.377403 pm4py-2.7.9.3/pm4py/objects/log/exporter/
--rw-rw-rw-   0        0        0      778 2023-12-11 09:33:52.000000 pm4py-2.7.9.3/pm4py/objects/log/exporter/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:37.399660 pm4py-2.7.9.3/pm4py/objects/log/exporter/xes/
--rw-rw-rw-   0        0        0      803 2023-12-11 09:33:52.000000 pm4py-2.7.9.3/pm4py/objects/log/exporter/xes/__init__.py
--rw-rw-rw-   0        0        0     2578 2023-12-11 09:33:52.000000 pm4py-2.7.9.3/pm4py/objects/log/exporter/xes/exporter.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:37.428015 pm4py-2.7.9.3/pm4py/objects/log/exporter/xes/util/
--rw-rw-rw-   0        0        0      795 2023-12-11 09:33:52.000000 pm4py-2.7.9.3/pm4py/objects/log/exporter/xes/util/__init__.py
--rw-rw-rw-   0        0        0     1423 2023-12-11 09:33:52.000000 pm4py-2.7.9.3/pm4py/objects/log/exporter/xes/util/compression.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:37.463407 pm4py-2.7.9.3/pm4py/objects/log/exporter/xes/variants/
--rw-rw-rw-   0        0        0      815 2023-12-11 09:33:52.000000 pm4py-2.7.9.3/pm4py/objects/log/exporter/xes/variants/__init__.py
--rw-rw-rw-   0        0        0    12326 2023-12-11 09:33:52.000000 pm4py-2.7.9.3/pm4py/objects/log/exporter/xes/variants/etree_xes_exp.py
--rw-rw-rw-   0        0        0    10430 2023-12-11 09:33:52.000000 pm4py-2.7.9.3/pm4py/objects/log/exporter/xes/variants/line_by_line.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:37.475165 pm4py-2.7.9.3/pm4py/objects/log/importer/
--rw-rw-rw-   0        0        0      778 2023-12-11 09:33:52.000000 pm4py-2.7.9.3/pm4py/objects/log/importer/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:37.497495 pm4py-2.7.9.3/pm4py/objects/log/importer/xes/
--rw-rw-rw-   0        0        0      797 2023-12-11 09:33:52.000000 pm4py-2.7.9.3/pm4py/objects/log/importer/xes/__init__.py
--rw-rw-rw-   0        0        0     4379 2023-12-11 09:33:52.000000 pm4py-2.7.9.3/pm4py/objects/log/importer/xes/importer.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:37.577392 pm4py-2.7.9.3/pm4py/objects/log/importer/xes/variants/
--rw-rw-rw-   0        0        0      850 2023-12-11 09:33:52.000000 pm4py-2.7.9.3/pm4py/objects/log/importer/xes/variants/__init__.py
--rw-rw-rw-   0        0        0     9534 2023-12-11 09:33:52.000000 pm4py-2.7.9.3/pm4py/objects/log/importer/xes/variants/chunk_regex.py
--rw-rw-rw-   0        0        0    17582 2023-12-11 09:33:52.000000 pm4py-2.7.9.3/pm4py/objects/log/importer/xes/variants/iterparse.py
--rw-rw-rw-   0        0        0    17851 2023-12-11 09:33:52.000000 pm4py-2.7.9.3/pm4py/objects/log/importer/xes/variants/iterparse_20.py
--rw-rw-rw-   0        0        0    18150 2023-12-11 09:33:52.000000 pm4py-2.7.9.3/pm4py/objects/log/importer/xes/variants/iterparse_mem_compressed.py
--rw-rw-rw-   0        0        0    11435 2023-12-11 09:33:52.000000 pm4py-2.7.9.3/pm4py/objects/log/importer/xes/variants/line_by_line.py
--rw-rw-rw-   0        0        0     2094 2024-01-02 13:29:21.000000 pm4py-2.7.9.3/pm4py/objects/log/importer/xes/variants/rustxes.py
--rw-rw-rw-   0        0        0    12284 2023-12-11 09:33:52.000000 pm4py-2.7.9.3/pm4py/objects/log/obj.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:37.814040 pm4py-2.7.9.3/pm4py/objects/log/util/
--rw-rw-rw-   0        0        0     1010 2023-12-11 09:33:52.000000 pm4py-2.7.9.3/pm4py/objects/log/util/__init__.py
--rw-rw-rw-   0        0        0     3127 2023-12-11 09:33:52.000000 pm4py-2.7.9.3/pm4py/objects/log/util/activities_to_alphabet.py
--rw-rw-rw-   0        0        0     3114 2023-12-11 09:33:52.000000 pm4py-2.7.9.3/pm4py/objects/log/util/artificial.py
--rw-rw-rw-   0        0        0     3974 2023-12-11 09:33:52.000000 pm4py-2.7.9.3/pm4py/objects/log/util/basic_filter.py
--rw-rw-rw-   0        0        0    18992 2024-01-15 12:00:43.000000 pm4py-2.7.9.3/pm4py/objects/log/util/dataframe_utils.py
--rw-rw-rw-   0        0        0     2283 2023-12-11 09:33:52.000000 pm4py-2.7.9.3/pm4py/objects/log/util/filtering_utils.py
--rw-rw-rw-   0        0        0     4856 2024-01-02 13:29:21.000000 pm4py-2.7.9.3/pm4py/objects/log/util/get_class_representation.py
--rw-rw-rw-   0        0        0     3195 2023-12-11 09:33:52.000000 pm4py-2.7.9.3/pm4py/objects/log/util/get_log_encoded.py
--rw-rw-rw-   0        0        0     8099 2023-12-11 09:33:52.000000 pm4py-2.7.9.3/pm4py/objects/log/util/get_prefixes.py
--rw-rw-rw-   0        0        0     1752 2023-12-11 09:33:52.000000 pm4py-2.7.9.3/pm4py/objects/log/util/index_attribute.py
--rw-rw-rw-   0        0        0     4067 2023-12-11 09:33:52.000000 pm4py-2.7.9.3/pm4py/objects/log/util/insert_classifier.py
--rw-rw-rw-   0        0        0    12476 2024-01-02 13:29:21.000000 pm4py-2.7.9.3/pm4py/objects/log/util/interval_lifecycle.py
--rw-rw-rw-   0        0        0     5167 2023-12-11 09:33:52.000000 pm4py-2.7.9.3/pm4py/objects/log/util/log.py
--rw-rw-rw-   0        0        0     4389 2023-12-11 09:33:52.000000 pm4py-2.7.9.3/pm4py/objects/log/util/log_regex.py
--rw-rw-rw-   0        0        0     2867 2023-12-11 09:33:52.000000 pm4py-2.7.9.3/pm4py/objects/log/util/move_attrs_to_trace.py
--rw-rw-rw-   0        0        0     4527 2023-12-11 09:33:52.000000 pm4py-2.7.9.3/pm4py/objects/log/util/pandas_log_wrapper.py
--rw-rw-rw-   0        0        0     4094 2024-01-15 12:00:43.000000 pm4py-2.7.9.3/pm4py/objects/log/util/pandas_numpy_variants.py
--rw-rw-rw-   0        0        0     2465 2023-12-11 09:33:52.000000 pm4py-2.7.9.3/pm4py/objects/log/util/sampling.py
--rw-rw-rw-   0        0        0     6049 2023-12-11 09:33:52.000000 pm4py-2.7.9.3/pm4py/objects/log/util/sorting.py
--rw-rw-rw-   0        0        0     2078 2023-12-11 09:33:52.000000 pm4py-2.7.9.3/pm4py/objects/log/util/split_train_test.py
--rw-rw-rw-   0        0        0     1695 2023-12-11 09:33:52.000000 pm4py-2.7.9.3/pm4py/objects/log/util/xes.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:37.848055 pm4py-2.7.9.3/pm4py/objects/ocel/
--rw-rw-rw-   0        0        0      819 2023-12-11 09:33:52.000000 pm4py-2.7.9.3/pm4py/objects/ocel/__init__.py
--rw-rw-rw-   0        0        0     2372 2023-12-11 09:33:52.000000 pm4py-2.7.9.3/pm4py/objects/ocel/constants.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:37.860963 pm4py-2.7.9.3/pm4py/objects/ocel/exporter/
--rw-rw-rw-   0        0        0      911 2023-12-11 09:33:52.000000 pm4py-2.7.9.3/pm4py/objects/ocel/exporter/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:37.884043 pm4py-2.7.9.3/pm4py/objects/ocel/exporter/csv/
--rw-rw-rw-   0        0        0      798 2023-12-11 09:33:52.000000 pm4py-2.7.9.3/pm4py/objects/ocel/exporter/csv/__init__.py
--rw-rw-rw-   0        0        0     1695 2023-12-11 09:33:52.000000 pm4py-2.7.9.3/pm4py/objects/ocel/exporter/csv/exporter.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:37.905946 pm4py-2.7.9.3/pm4py/objects/ocel/exporter/csv/variants/
--rw-rw-rw-   0        0        0      795 2023-12-11 09:33:52.000000 pm4py-2.7.9.3/pm4py/objects/ocel/exporter/csv/variants/__init__.py
--rw-rw-rw-   0        0        0     1927 2023-12-11 09:33:52.000000 pm4py-2.7.9.3/pm4py/objects/ocel/exporter/csv/variants/pandas.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:37.927167 pm4py-2.7.9.3/pm4py/objects/ocel/exporter/jsonocel/
--rw-rw-rw-   0        0        0      803 2023-12-11 09:33:52.000000 pm4py-2.7.9.3/pm4py/objects/ocel/exporter/jsonocel/__init__.py
--rw-rw-rw-   0        0        0     1635 2023-12-11 09:33:52.000000 pm4py-2.7.9.3/pm4py/objects/ocel/exporter/jsonocel/exporter.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:37.972510 pm4py-2.7.9.3/pm4py/objects/ocel/exporter/jsonocel/variants/
--rw-rw-rw-   0        0        0      826 2023-12-11 09:33:52.000000 pm4py-2.7.9.3/pm4py/objects/ocel/exporter/jsonocel/variants/__init__.py
--rw-rw-rw-   0        0        0     5448 2024-01-02 13:29:21.000000 pm4py-2.7.9.3/pm4py/objects/ocel/exporter/jsonocel/variants/classic.py
--rw-rw-rw-   0        0        0     5591 2023-12-11 09:33:52.000000 pm4py-2.7.9.3/pm4py/objects/ocel/exporter/jsonocel/variants/ocel20.py
--rw-rw-rw-   0        0        0     4247 2023-12-11 09:33:52.000000 pm4py-2.7.9.3/pm4py/objects/ocel/exporter/jsonocel/variants/ocel20_standard.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:37.997249 pm4py-2.7.9.3/pm4py/objects/ocel/exporter/sqlite/
--rw-rw-rw-   0        0        0      803 2023-12-11 09:33:52.000000 pm4py-2.7.9.3/pm4py/objects/ocel/exporter/sqlite/__init__.py
--rw-rw-rw-   0        0        0     1673 2023-12-11 09:33:52.000000 pm4py-2.7.9.3/pm4py/objects/ocel/exporter/sqlite/exporter.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:38.034446 pm4py-2.7.9.3/pm4py/objects/ocel/exporter/sqlite/variants/
--rw-rw-rw-   0        0        0      809 2023-12-11 09:33:52.000000 pm4py-2.7.9.3/pm4py/objects/ocel/exporter/sqlite/variants/__init__.py
--rw-rw-rw-   0        0        0     4931 2024-01-02 13:29:21.000000 pm4py-2.7.9.3/pm4py/objects/ocel/exporter/sqlite/variants/ocel20.py
--rw-rw-rw-   0        0        0     1679 2023-12-11 09:33:52.000000 pm4py-2.7.9.3/pm4py/objects/ocel/exporter/sqlite/variants/pandas_exporter.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:38.056535 pm4py-2.7.9.3/pm4py/objects/ocel/exporter/util/
--rw-rw-rw-   0        0        0      797 2023-12-11 09:33:52.000000 pm4py-2.7.9.3/pm4py/objects/ocel/exporter/util/__init__.py
--rw-rw-rw-   0        0        0     1658 2024-01-02 13:29:21.000000 pm4py-2.7.9.3/pm4py/objects/ocel/exporter/util/clean_dataframes.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:38.077198 pm4py-2.7.9.3/pm4py/objects/ocel/exporter/xmlocel/
--rw-rw-rw-   0        0        0      802 2023-12-11 09:33:52.000000 pm4py-2.7.9.3/pm4py/objects/ocel/exporter/xmlocel/__init__.py
--rw-rw-rw-   0        0        0     1578 2023-12-11 09:33:52.000000 pm4py-2.7.9.3/pm4py/objects/ocel/exporter/xmlocel/exporter.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:38.111929 pm4py-2.7.9.3/pm4py/objects/ocel/exporter/xmlocel/variants/
--rw-rw-rw-   0        0        0      734 2023-12-11 09:33:52.000000 pm4py-2.7.9.3/pm4py/objects/ocel/exporter/xmlocel/variants/__init__.py
--rw-rw-rw-   0        0        0     8129 2024-01-02 13:29:21.000000 pm4py-2.7.9.3/pm4py/objects/ocel/exporter/xmlocel/variants/classic.py
--rw-rw-rw-   0        0        0     8746 2023-12-11 09:33:52.000000 pm4py-2.7.9.3/pm4py/objects/ocel/exporter/xmlocel/variants/ocel20.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:38.124404 pm4py-2.7.9.3/pm4py/objects/ocel/importer/
--rw-rw-rw-   0        0        0      905 2023-12-11 09:33:52.000000 pm4py-2.7.9.3/pm4py/objects/ocel/importer/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:38.145421 pm4py-2.7.9.3/pm4py/objects/ocel/importer/csv/
--rw-rw-rw-   0        0        0      798 2023-12-11 09:33:52.000000 pm4py-2.7.9.3/pm4py/objects/ocel/importer/csv/__init__.py
--rw-rw-rw-   0        0        0     1731 2023-12-11 09:33:52.000000 pm4py-2.7.9.3/pm4py/objects/ocel/importer/csv/importer.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:38.165981 pm4py-2.7.9.3/pm4py/objects/ocel/importer/csv/variants/
--rw-rw-rw-   0        0        0      795 2023-12-11 09:33:52.000000 pm4py-2.7.9.3/pm4py/objects/ocel/importer/csv/variants/__init__.py
--rw-rw-rw-   0        0        0     2211 2024-01-02 13:29:21.000000 pm4py-2.7.9.3/pm4py/objects/ocel/importer/csv/variants/pandas.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:38.188631 pm4py-2.7.9.3/pm4py/objects/ocel/importer/jsonocel/
--rw-rw-rw-   0        0        0      803 2023-12-11 09:33:52.000000 pm4py-2.7.9.3/pm4py/objects/ocel/importer/jsonocel/__init__.py
--rw-rw-rw-   0        0        0     1641 2023-12-11 09:33:52.000000 pm4py-2.7.9.3/pm4py/objects/ocel/importer/jsonocel/importer.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:38.221192 pm4py-2.7.9.3/pm4py/objects/ocel/importer/jsonocel/variants/
--rw-rw-rw-   0        0        0      818 2023-12-11 09:33:52.000000 pm4py-2.7.9.3/pm4py/objects/ocel/importer/jsonocel/variants/__init__.py
--rw-rw-rw-   0        0        0     7338 2024-01-16 10:09:19.000000 pm4py-2.7.9.3/pm4py/objects/ocel/importer/jsonocel/variants/classic.py
--rw-rw-rw-   0        0        0     3863 2023-12-11 09:33:52.000000 pm4py-2.7.9.3/pm4py/objects/ocel/importer/jsonocel/variants/ocel20_standard.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:38.235710 pm4py-2.7.9.3/pm4py/objects/ocel/importer/sqlite/
--rw-rw-rw-   0        0        0      803 2023-12-11 09:33:52.000000 pm4py-2.7.9.3/pm4py/objects/ocel/importer/sqlite/__init__.py
--rw-rw-rw-   0        0        0     1704 2023-12-11 09:33:52.000000 pm4py-2.7.9.3/pm4py/objects/ocel/importer/sqlite/importer.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:38.271759 pm4py-2.7.9.3/pm4py/objects/ocel/importer/sqlite/variants/
--rw-rw-rw-   0        0        0      809 2023-12-11 09:33:52.000000 pm4py-2.7.9.3/pm4py/objects/ocel/importer/sqlite/variants/__init__.py
--rw-rw-rw-   0        0        0     8462 2024-01-16 10:09:19.000000 pm4py-2.7.9.3/pm4py/objects/ocel/importer/sqlite/variants/ocel20.py
--rw-rw-rw-   0        0        0     2620 2024-01-02 13:29:21.000000 pm4py-2.7.9.3/pm4py/objects/ocel/importer/sqlite/variants/pandas_importer.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:38.292976 pm4py-2.7.9.3/pm4py/objects/ocel/importer/xmlocel/
--rw-rw-rw-   0        0        0      802 2023-12-11 09:33:52.000000 pm4py-2.7.9.3/pm4py/objects/ocel/importer/xmlocel/__init__.py
--rw-rw-rw-   0        0        0     1611 2023-12-11 09:33:52.000000 pm4py-2.7.9.3/pm4py/objects/ocel/importer/xmlocel/importer.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:38.325933 pm4py-2.7.9.3/pm4py/objects/ocel/importer/xmlocel/variants/
--rw-rw-rw-   0        0        0      800 2023-12-11 09:33:52.000000 pm4py-2.7.9.3/pm4py/objects/ocel/importer/xmlocel/variants/__init__.py
--rw-rw-rw-   0        0        0     8919 2024-01-02 13:29:21.000000 pm4py-2.7.9.3/pm4py/objects/ocel/importer/xmlocel/variants/classic.py
--rw-rw-rw-   0        0        0    10021 2024-01-16 10:09:19.000000 pm4py-2.7.9.3/pm4py/objects/ocel/importer/xmlocel/variants/ocel20.py
--rw-rw-rw-   0        0        0     7221 2024-01-02 13:29:21.000000 pm4py-2.7.9.3/pm4py/objects/ocel/obj.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:38.603985 pm4py-2.7.9.3/pm4py/objects/ocel/util/
--rw-rw-rw-   0        0        0     1067 2023-12-11 09:33:52.000000 pm4py-2.7.9.3/pm4py/objects/ocel/util/__init__.py
--rw-rw-rw-   0        0        0     1690 2023-12-11 09:33:52.000000 pm4py-2.7.9.3/pm4py/objects/ocel/util/attributes_names.py
--rw-rw-rw-   0        0        0     2156 2023-12-11 09:33:52.000000 pm4py-2.7.9.3/pm4py/objects/ocel/util/attributes_per_type.py
--rw-rw-rw-   0        0        0     2424 2023-12-11 09:33:52.000000 pm4py-2.7.9.3/pm4py/objects/ocel/util/convergence_divergence_diagnostics.py
--rw-rw-rw-   0        0        0     2690 2023-12-11 09:33:52.000000 pm4py-2.7.9.3/pm4py/objects/ocel/util/e2o_qualification.py
--rw-rw-rw-   0        0        0     3809 2024-01-02 13:29:21.000000 pm4py-2.7.9.3/pm4py/objects/ocel/util/ev_att_to_obj_type.py
--rw-rw-rw-   0        0        0     4453 2024-01-02 13:29:21.000000 pm4py-2.7.9.3/pm4py/objects/ocel/util/event_prefix_suffix_per_obj.py
--rw-rw-rw-   0        0        0     2215 2024-01-02 13:29:21.000000 pm4py-2.7.9.3/pm4py/objects/ocel/util/events_per_object_type.py
--rw-rw-rw-   0        0        0     3274 2024-01-02 13:29:21.000000 pm4py-2.7.9.3/pm4py/objects/ocel/util/events_per_type_per_activity.py
--rw-rw-rw-   0        0        0     1654 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/objects/ocel/util/explode.py
--rw-rw-rw-   0        0        0     5068 2024-01-02 13:29:21.000000 pm4py-2.7.9.3/pm4py/objects/ocel/util/extended_table.py
--rw-rw-rw-   0        0        0     6565 2024-01-02 13:29:21.000000 pm4py-2.7.9.3/pm4py/objects/ocel/util/filtering_utils.py
--rw-rw-rw-   0        0        0     3069 2024-01-02 13:29:21.000000 pm4py-2.7.9.3/pm4py/objects/ocel/util/flattening.py
--rw-rw-rw-   0        0        0    17070 2024-01-02 13:29:21.000000 pm4py-2.7.9.3/pm4py/objects/ocel/util/log_ocel.py
--rw-rw-rw-   0        0        0      942 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/objects/ocel/util/names_stripping.py
--rw-rw-rw-   0        0        0     3274 2024-01-02 13:29:21.000000 pm4py-2.7.9.3/pm4py/objects/ocel/util/objects_per_type_per_activity.py
--rw-rw-rw-   0        0        0     1974 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/objects/ocel/util/ocel_consistency.py
--rw-rw-rw-   0        0        0     1976 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/objects/ocel/util/ocel_iterator.py
--rw-rw-rw-   0        0        0     5167 2024-01-02 13:29:21.000000 pm4py-2.7.9.3/pm4py/objects/ocel/util/ocel_to_dict_types_rel.py
--rw-rw-rw-   0        0        0     3510 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/objects/ocel/util/ocel_type_renaming.py
--rw-rw-rw-   0        0        0     2478 2024-01-02 13:29:21.000000 pm4py-2.7.9.3/pm4py/objects/ocel/util/parent_children_ref.py
--rw-rw-rw-   0        0        0     1362 2024-01-02 13:29:21.000000 pm4py-2.7.9.3/pm4py/objects/ocel/util/related_events.py
--rw-rw-rw-   0        0        0     1830 2024-01-02 13:29:21.000000 pm4py-2.7.9.3/pm4py/objects/ocel/util/related_objects.py
--rw-rw-rw-   0        0        0     2610 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/objects/ocel/util/rename_objs_ot_tim_lex.py
--rw-rw-rw-   0        0        0     3783 2024-01-02 13:29:21.000000 pm4py-2.7.9.3/pm4py/objects/ocel/util/sampling.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:38.652969 pm4py-2.7.9.3/pm4py/objects/ocel/validation/
--rw-rw-rw-   0        0        0      795 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/objects/ocel/validation/__init__.py
--rw-rw-rw-   0        0        0     1389 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/objects/ocel/validation/jsonocel.py
--rw-rw-rw-   0        0        0    14786 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/objects/ocel/validation/ocel20_rel_validation.py
--rw-rw-rw-   0        0        0     1212 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/objects/ocel/validation/xmlocel.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:38.665049 pm4py-2.7.9.3/pm4py/objects/org/
--rw-rw-rw-   0        0        0      776 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/objects/org/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:38.686266 pm4py-2.7.9.3/pm4py/objects/org/roles/
--rw-rw-rw-   0        0        0      775 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/objects/org/roles/__init__.py
--rw-rw-rw-   0        0        0     1339 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/objects/org/roles/obj.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:38.707112 pm4py-2.7.9.3/pm4py/objects/org/sna/
--rw-rw-rw-   0        0        0      773 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/objects/org/sna/__init__.py
--rw-rw-rw-   0        0        0     1029 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/objects/org/sna/obj.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:38.763802 pm4py-2.7.9.3/pm4py/objects/petri_net/
--rw-rw-rw-   0        0        0      828 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/objects/petri_net/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:38.789870 pm4py-2.7.9.3/pm4py/objects/petri_net/data_petri_nets/
--rw-rw-rw-   0        0        0      734 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/objects/petri_net/data_petri_nets/__init__.py
--rw-rw-rw-   0        0        0     1287 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/objects/petri_net/data_petri_nets/data_marking.py
--rw-rw-rw-   0        0        0     6212 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/objects/petri_net/data_petri_nets/semantics.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:38.811418 pm4py-2.7.9.3/pm4py/objects/petri_net/exporter/
--rw-rw-rw-   0        0        0      799 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/objects/petri_net/exporter/__init__.py
--rw-rw-rw-   0        0        0     2366 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/objects/petri_net/exporter/exporter.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:38.833721 pm4py-2.7.9.3/pm4py/objects/petri_net/exporter/variants/
--rw-rw-rw-   0        0        0      794 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/objects/petri_net/exporter/variants/__init__.py
--rw-rw-rw-   0        0        0    13002 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/objects/petri_net/exporter/variants/pnml.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:38.855612 pm4py-2.7.9.3/pm4py/objects/petri_net/importer/
--rw-rw-rw-   0        0        0      799 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/objects/petri_net/importer/__init__.py
--rw-rw-rw-   0        0        0     1910 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/objects/petri_net/importer/importer.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:38.879517 pm4py-2.7.9.3/pm4py/objects/petri_net/importer/variants/
--rw-rw-rw-   0        0        0      794 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/objects/petri_net/importer/variants/__init__.py
--rw-rw-rw-   0        0        0    15369 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/objects/petri_net/importer/variants/pnml.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:38.894581 pm4py-2.7.9.3/pm4py/objects/petri_net/inhibitor_reset/
--rw-rw-rw-   0        0        0      734 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/objects/petri_net/inhibitor_reset/__init__.py
--rw-rw-rw-   0        0        0     4617 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/objects/petri_net/inhibitor_reset/semantics.py
--rw-rw-rw-   0        0        0    13270 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/objects/petri_net/obj.py
--rw-rw-rw-   0        0        0     1225 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/objects/petri_net/properties.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:38.938377 pm4py-2.7.9.3/pm4py/objects/petri_net/saw_net/
--rw-rw-rw-   0        0        0      805 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/objects/petri_net/saw_net/__init__.py
--rw-rw-rw-   0        0        0     4799 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/objects/petri_net/saw_net/convert.py
--rw-rw-rw-   0        0        0     1546 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/objects/petri_net/saw_net/obj.py
--rw-rw-rw-   0        0        0    10711 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/objects/petri_net/saw_net/semantics.py
--rw-rw-rw-   0        0        0     1503 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/objects/petri_net/sem_interface.py
--rw-rw-rw-   0        0        0     5339 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/objects/petri_net/semantics.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:38.973418 pm4py-2.7.9.3/pm4py/objects/petri_net/stochastic/
--rw-rw-rw-   0        0        0      799 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/objects/petri_net/stochastic/__init__.py
--rw-rw-rw-   0        0        0     1448 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/objects/petri_net/stochastic/obj.py
--rw-rw-rw-   0        0        0     2607 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/objects/petri_net/stochastic/semantics.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:39.177823 pm4py-2.7.9.3/pm4py/objects/petri_net/utils/
--rw-rw-rw-   0        0        0     1035 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/objects/petri_net/utils/__init__.py
--rw-rw-rw-   0        0        0    19297 2024-01-04 10:14:42.000000 pm4py-2.7.9.3/pm4py/objects/petri_net/utils/align_utils.py
--rw-rw-rw-   0        0        0     5923 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/objects/petri_net/utils/check_soundness.py
--rw-rw-rw-   0        0        0     4014 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/objects/petri_net/utils/consumption_matrix.py
--rw-rw-rw-   0        0        0     6609 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/objects/petri_net/utils/decomposition.py
--rw-rw-rw-   0        0        0     1672 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/objects/petri_net/utils/embed_stochastic_map.py
--rw-rw-rw-   0        0        0     5751 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/objects/petri_net/utils/explore_path.py
--rw-rw-rw-   0        0        0     1195 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/objects/petri_net/utils/final_marking.py
--rw-rw-rw-   0        0        0     2272 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/objects/petri_net/utils/incidence_matrix.py
--rw-rw-rw-   0        0        0     1227 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/objects/petri_net/utils/initial_marking.py
--rw-rw-rw-   0        0        0     4243 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/objects/petri_net/utils/murata.py
--rw-rw-rw-   0        0        0     4281 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/objects/petri_net/utils/networkx_graph.py
--rw-rw-rw-   0        0        0     4071 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/objects/petri_net/utils/obj_marking.py
--rw-rw-rw-   0        0        0    22973 2024-01-02 13:29:21.000000 pm4py-2.7.9.3/pm4py/objects/petri_net/utils/performance_map.py
--rw-rw-rw-   0        0        0    20395 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/objects/petri_net/utils/petri_utils.py
--rw-rw-rw-   0        0        0     4602 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/objects/petri_net/utils/projection.py
--rw-rw-rw-   0        0        0     5570 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/objects/petri_net/utils/reachability_graph.py
--rw-rw-rw-   0        0        0    14266 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/objects/petri_net/utils/reduction.py
--rw-rw-rw-   0        0        0     7288 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/objects/petri_net/utils/synchronous_product.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:39.233056 pm4py-2.7.9.3/pm4py/objects/powl/
--rw-rw-rw-   0        0        0     6732 2024-01-02 13:29:21.000000 pm4py-2.7.9.3/pm4py/objects/powl/BinaryRelation.py
--rw-rw-rw-   0        0        0      772 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/objects/powl/__init__.py
--rw-rw-rw-   0        0        0      804 2024-01-02 13:29:21.000000 pm4py-2.7.9.3/pm4py/objects/powl/constants.py
--rw-rw-rw-   0        0        0    15122 2024-01-02 13:29:21.000000 pm4py-2.7.9.3/pm4py/objects/powl/obj.py
--rw-rw-rw-   0        0        0     5268 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/objects/powl/parser.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:39.277605 pm4py-2.7.9.3/pm4py/objects/process_tree/
--rw-rw-rw-   0        0        0      929 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/objects/process_tree/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:39.301511 pm4py-2.7.9.3/pm4py/objects/process_tree/exporter/
--rw-rw-rw-   0        0        0      802 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/objects/process_tree/exporter/__init__.py
--rw-rw-rw-   0        0        0     1888 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/objects/process_tree/exporter/exporter.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:39.327716 pm4py-2.7.9.3/pm4py/objects/process_tree/exporter/variants/
--rw-rw-rw-   0        0        0      797 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/objects/process_tree/exporter/variants/__init__.py
--rw-rw-rw-   0        0        0     5832 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/objects/process_tree/exporter/variants/ptml.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:39.353684 pm4py-2.7.9.3/pm4py/objects/process_tree/importer/
--rw-rw-rw-   0        0        0      802 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/objects/process_tree/importer/__init__.py
--rw-rw-rw-   0        0        0     2048 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/objects/process_tree/importer/importer.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:39.376297 pm4py-2.7.9.3/pm4py/objects/process_tree/importer/variants/
--rw-rw-rw-   0        0        0      797 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/objects/process_tree/importer/variants/__init__.py
--rw-rw-rw-   0        0        0     5476 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/objects/process_tree/importer/variants/ptml.py
--rw-rw-rw-   0        0        0     8283 2024-01-02 13:29:21.000000 pm4py-2.7.9.3/pm4py/objects/process_tree/obj.py
--rw-rw-rw-   0        0        0     8883 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/objects/process_tree/semantics.py
--rw-rw-rw-   0        0        0      887 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/objects/process_tree/state.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:39.414341 pm4py-2.7.9.3/pm4py/objects/process_tree/utils/
--rw-rw-rw-   0        0        0      734 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/objects/process_tree/utils/__init__.py
--rw-rw-rw-   0        0        0     7128 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/objects/process_tree/utils/bottomup.py
--rw-rw-rw-   0        0        0    15834 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/objects/process_tree/utils/generic.py
--rw-rw-rw-   0        0        0     3438 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/objects/process_tree/utils/regex.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:39.451139 pm4py-2.7.9.3/pm4py/objects/random_variables/
--rw-rw-rw-   0        0        0     1034 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/objects/random_variables/__init__.py
--rw-rw-rw-   0        0        0     3878 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/objects/random_variables/basic_structure.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:39.474891 pm4py-2.7.9.3/pm4py/objects/random_variables/constant0/
--rw-rw-rw-   0        0        0      804 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/objects/random_variables/constant0/__init__.py
--rw-rw-rw-   0        0        0     3586 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/objects/random_variables/constant0/random_variable.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:39.496572 pm4py-2.7.9.3/pm4py/objects/random_variables/exponential/
--rw-rw-rw-   0        0        0      818 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/objects/random_variables/exponential/__init__.py
--rw-rw-rw-   0        0        0     3684 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/objects/random_variables/exponential/random_variable.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:39.518962 pm4py-2.7.9.3/pm4py/objects/random_variables/gamma/
--rw-rw-rw-   0        0        0      800 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/objects/random_variables/gamma/__init__.py
--rw-rw-rw-   0        0        0     3841 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/objects/random_variables/gamma/random_variable.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:39.541053 pm4py-2.7.9.3/pm4py/objects/random_variables/lognormal/
--rw-rw-rw-   0        0        0      804 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/objects/random_variables/lognormal/__init__.py
--rw-rw-rw-   0        0        0     3568 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/objects/random_variables/lognormal/random_variable.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:39.564429 pm4py-2.7.9.3/pm4py/objects/random_variables/normal/
--rw-rw-rw-   0        0        0      801 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/objects/random_variables/normal/__init__.py
--rw-rw-rw-   0        0        0     3594 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/objects/random_variables/normal/random_variable.py
--rw-rw-rw-   0        0        0     9224 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/objects/random_variables/random_variable.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:39.587715 pm4py-2.7.9.3/pm4py/objects/random_variables/uniform/
--rw-rw-rw-   0        0        0      802 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/objects/random_variables/uniform/__init__.py
--rw-rw-rw-   0        0        0     3588 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/objects/random_variables/uniform/random_variable.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:39.630600 pm4py-2.7.9.3/pm4py/objects/stochastic_petri/
--rw-rw-rw-   0        0        0      988 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/objects/stochastic_petri/__init__.py
--rw-rw-rw-   0        0        0    12887 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/objects/stochastic_petri/ctmc.py
--rw-rw-rw-   0        0        0     4714 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/objects/stochastic_petri/tangible_reachability.py
--rw-rw-rw-   0        0        0     1616 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/objects/stochastic_petri/utils.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:39.675432 pm4py-2.7.9.3/pm4py/objects/transition_system/
--rw-rw-rw-   0        0        0      803 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/objects/transition_system/__init__.py
--rw-rw-rw-   0        0        0      825 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/objects/transition_system/constants.py
--rw-rw-rw-   0        0        0     3958 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/objects/transition_system/obj.py
--rw-rw-rw-   0        0        0     3625 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/objects/transition_system/utils.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:39.697373 pm4py-2.7.9.3/pm4py/objects/trie/
--rw-rw-rw-   0        0        0      770 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/objects/trie/__init__.py
--rw-rw-rw-   0        0        0     1911 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/objects/trie/obj.py
--rw-rw-rw-   0        0        0    23143 2024-01-15 12:00:43.000000 pm4py-2.7.9.3/pm4py/ocel.py
--rw-rw-rw-   0        0        0    14594 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/org.py
--rw-rw-rw-   0        0        0     3805 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/privacy.py
--rw-rw-rw-   0        0        0    15303 2024-01-16 10:09:19.000000 pm4py-2.7.9.3/pm4py/read.py
--rw-rw-rw-   0        0        0     4578 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/sim.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:39.709879 pm4py-2.7.9.3/pm4py/statistics/
--rw-rw-rw-   0        0        0      899 2024-01-02 13:29:21.000000 pm4py-2.7.9.3/pm4py/statistics/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:39.721293 pm4py-2.7.9.3/pm4py/statistics/attributes/
--rw-rw-rw-   0        0        0      795 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/statistics/attributes/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:39.744066 pm4py-2.7.9.3/pm4py/statistics/attributes/common/
--rw-rw-rw-   0        0        0      786 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/statistics/attributes/common/__init__.py
--rw-rw-rw-   0        0        0     6611 2024-01-02 13:29:21.000000 pm4py-2.7.9.3/pm4py/statistics/attributes/common/get.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:39.776965 pm4py-2.7.9.3/pm4py/statistics/attributes/log/
--rw-rw-rw-   0        0        0      791 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/statistics/attributes/log/__init__.py
--rw-rw-rw-   0        0        0    13311 2024-01-02 13:29:21.000000 pm4py-2.7.9.3/pm4py/statistics/attributes/log/get.py
--rw-rw-rw-   0        0        0     6905 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/statistics/attributes/log/select.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:39.802476 pm4py-2.7.9.3/pm4py/statistics/attributes/pandas/
--rw-rw-rw-   0        0        0      786 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/statistics/attributes/pandas/__init__.py
--rw-rw-rw-   0        0        0     9777 2024-01-15 12:00:43.000000 pm4py-2.7.9.3/pm4py/statistics/attributes/pandas/get.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:39.813766 pm4py-2.7.9.3/pm4py/statistics/concurrent_activities/
--rw-rw-rw-   0        0        0      798 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/statistics/concurrent_activities/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:39.837126 pm4py-2.7.9.3/pm4py/statistics/concurrent_activities/log/
--rw-rw-rw-   0        0        0      794 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/statistics/concurrent_activities/log/__init__.py
--rw-rw-rw-   0        0        0     4081 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/statistics/concurrent_activities/log/get.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:39.858666 pm4py-2.7.9.3/pm4py/statistics/concurrent_activities/pandas/
--rw-rw-rw-   0        0        0      797 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/statistics/concurrent_activities/pandas/__init__.py
--rw-rw-rw-   0        0        0     3686 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/statistics/concurrent_activities/pandas/get.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:39.871788 pm4py-2.7.9.3/pm4py/statistics/end_activities/
--rw-rw-rw-   0        0        0      799 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/statistics/end_activities/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:39.893720 pm4py-2.7.9.3/pm4py/statistics/end_activities/common/
--rw-rw-rw-   0        0        0      790 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/statistics/end_activities/common/__init__.py
--rw-rw-rw-   0        0        0     1791 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/statistics/end_activities/common/get.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:39.915284 pm4py-2.7.9.3/pm4py/statistics/end_activities/log/
--rw-rw-rw-   0        0        0      787 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/statistics/end_activities/log/__init__.py
--rw-rw-rw-   0        0        0     2746 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/statistics/end_activities/log/get.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:39.937687 pm4py-2.7.9.3/pm4py/statistics/end_activities/pandas/
--rw-rw-rw-   0        0        0      790 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/statistics/end_activities/pandas/__init__.py
--rw-rw-rw-   0        0        0     2665 2024-01-15 12:00:43.000000 pm4py-2.7.9.3/pm4py/statistics/end_activities/pandas/get.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:39.949134 pm4py-2.7.9.3/pm4py/statistics/eventually_follows/
--rw-rw-rw-   0        0        0      801 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/statistics/eventually_follows/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:39.971241 pm4py-2.7.9.3/pm4py/statistics/eventually_follows/log/
--rw-rw-rw-   0        0        0      791 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/statistics/eventually_follows/log/__init__.py
--rw-rw-rw-   0        0        0     3015 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/statistics/eventually_follows/log/get.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:39.993746 pm4py-2.7.9.3/pm4py/statistics/eventually_follows/pandas/
--rw-rw-rw-   0        0        0      794 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/statistics/eventually_follows/pandas/__init__.py
--rw-rw-rw-   0        0        0     2879 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/statistics/eventually_follows/pandas/get.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:40.018552 pm4py-2.7.9.3/pm4py/statistics/eventually_follows/uvcl/
--rw-rw-rw-   0        0        0      792 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/statistics/eventually_follows/uvcl/__init__.py
--rw-rw-rw-   0        0        0     1936 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/statistics/eventually_follows/uvcl/get.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:40.074065 pm4py-2.7.9.3/pm4py/statistics/ocel/
--rw-rw-rw-   0        0        0      734 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/statistics/ocel/__init__.py
--rw-rw-rw-   0        0        0     3670 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/statistics/ocel/act_ot_dependent.py
--rw-rw-rw-   0        0        0     5684 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/statistics/ocel/act_utils.py
--rw-rw-rw-   0        0        0     9710 2024-01-02 13:29:21.000000 pm4py-2.7.9.3/pm4py/statistics/ocel/edge_metrics.py
--rw-rw-rw-   0        0        0     2361 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/statistics/ocel/objects_ot_count.py
--rw-rw-rw-   0        0        0     2395 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/statistics/ocel/ot_activities.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:40.086492 pm4py-2.7.9.3/pm4py/statistics/overlap/
--rw-rw-rw-   0        0        0      957 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/statistics/overlap/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:40.097627 pm4py-2.7.9.3/pm4py/statistics/overlap/cases/
--rw-rw-rw-   0        0        0      790 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/statistics/overlap/cases/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:40.120021 pm4py-2.7.9.3/pm4py/statistics/overlap/cases/log/
--rw-rw-rw-   0        0        0      786 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/statistics/overlap/cases/log/__init__.py
--rw-rw-rw-   0        0        0     2713 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/statistics/overlap/cases/log/get.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:40.142596 pm4py-2.7.9.3/pm4py/statistics/overlap/cases/pandas/
--rw-rw-rw-   0        0        0      789 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/statistics/overlap/cases/pandas/__init__.py
--rw-rw-rw-   0        0        0     3028 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/statistics/overlap/cases/pandas/get.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:40.153964 pm4py-2.7.9.3/pm4py/statistics/overlap/interval_events/
--rw-rw-rw-   0        0        0      800 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/statistics/overlap/interval_events/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:40.176927 pm4py-2.7.9.3/pm4py/statistics/overlap/interval_events/log/
--rw-rw-rw-   0        0        0      796 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/statistics/overlap/interval_events/log/__init__.py
--rw-rw-rw-   0        0        0     2767 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/statistics/overlap/interval_events/log/get.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:40.198862 pm4py-2.7.9.3/pm4py/statistics/overlap/interval_events/pandas/
--rw-rw-rw-   0        0        0      799 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/statistics/overlap/interval_events/pandas/__init__.py
--rw-rw-rw-   0        0        0     2570 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/statistics/overlap/interval_events/pandas/get.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:40.222463 pm4py-2.7.9.3/pm4py/statistics/overlap/utils/
--rw-rw-rw-   0        0        0      786 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/statistics/overlap/utils/__init__.py
--rw-rw-rw-   0        0        0     1986 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/statistics/overlap/utils/compute.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:40.235673 pm4py-2.7.9.3/pm4py/statistics/passed_time/
--rw-rw-rw-   0        0        0      790 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/statistics/passed_time/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:40.259339 pm4py-2.7.9.3/pm4py/statistics/passed_time/log/
--rw-rw-rw-   0        0        0      800 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/statistics/passed_time/log/__init__.py
--rw-rw-rw-   0        0        0     1781 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/statistics/passed_time/log/algorithm.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:40.318356 pm4py-2.7.9.3/pm4py/statistics/passed_time/log/variants/
--rw-rw-rw-   0        0        0      808 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/statistics/passed_time/log/variants/__init__.py
--rw-rw-rw-   0        0        0     2387 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/statistics/passed_time/log/variants/post.py
--rw-rw-rw-   0        0        0     2369 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/statistics/passed_time/log/variants/pre.py
--rw-rw-rw-   0        0        0     3050 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/statistics/passed_time/log/variants/prepost.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:40.340643 pm4py-2.7.9.3/pm4py/statistics/passed_time/pandas/
--rw-rw-rw-   0        0        0      803 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/statistics/passed_time/pandas/__init__.py
--rw-rw-rw-   0        0        0     1768 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/statistics/passed_time/pandas/algorithm.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:40.389463 pm4py-2.7.9.3/pm4py/statistics/passed_time/pandas/variants/
--rw-rw-rw-   0        0        0      811 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/statistics/passed_time/pandas/variants/__init__.py
--rw-rw-rw-   0        0        0     4131 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/statistics/passed_time/pandas/variants/post.py
--rw-rw-rw-   0        0        0     4235 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/statistics/passed_time/pandas/variants/pre.py
--rw-rw-rw-   0        0        0     4916 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/statistics/passed_time/pandas/variants/prepost.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:40.401402 pm4py-2.7.9.3/pm4py/statistics/rework/
--rw-rw-rw-   0        0        0      783 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/statistics/rework/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:40.412379 pm4py-2.7.9.3/pm4py/statistics/rework/cases/
--rw-rw-rw-   0        0        0      789 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/statistics/rework/cases/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:40.434728 pm4py-2.7.9.3/pm4py/statistics/rework/cases/log/
--rw-rw-rw-   0        0        0      785 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/statistics/rework/cases/log/__init__.py
--rw-rw-rw-   0        0        0     2597 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/statistics/rework/cases/log/get.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:40.456820 pm4py-2.7.9.3/pm4py/statistics/rework/cases/pandas/
--rw-rw-rw-   0        0        0      788 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/statistics/rework/cases/pandas/__init__.py
--rw-rw-rw-   0        0        0     2542 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/statistics/rework/cases/pandas/get.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:40.477567 pm4py-2.7.9.3/pm4py/statistics/rework/log/
--rw-rw-rw-   0        0        0      779 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/statistics/rework/log/__init__.py
--rw-rw-rw-   0        0        0     2265 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/statistics/rework/log/get.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:40.500669 pm4py-2.7.9.3/pm4py/statistics/rework/pandas/
--rw-rw-rw-   0        0        0      782 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/statistics/rework/pandas/__init__.py
--rw-rw-rw-   0        0        0     2378 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/statistics/rework/pandas/get.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:40.511920 pm4py-2.7.9.3/pm4py/statistics/service_time/
--rw-rw-rw-   0        0        0      789 2024-01-02 13:29:21.000000 pm4py-2.7.9.3/pm4py/statistics/service_time/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:40.535559 pm4py-2.7.9.3/pm4py/statistics/service_time/log/
--rw-rw-rw-   0        0        0      785 2024-01-02 13:29:21.000000 pm4py-2.7.9.3/pm4py/statistics/service_time/log/__init__.py
--rw-rw-rw-   0        0        0     5453 2024-01-02 13:29:21.000000 pm4py-2.7.9.3/pm4py/statistics/service_time/log/get.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:40.557625 pm4py-2.7.9.3/pm4py/statistics/service_time/pandas/
--rw-rw-rw-   0        0        0      788 2024-01-02 13:29:21.000000 pm4py-2.7.9.3/pm4py/statistics/service_time/pandas/__init__.py
--rw-rw-rw-   0        0        0     4930 2024-01-15 12:00:43.000000 pm4py-2.7.9.3/pm4py/statistics/service_time/pandas/get.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:40.568832 pm4py-2.7.9.3/pm4py/statistics/sojourn_time/
--rw-rw-rw-   0        0        0      779 2024-01-02 13:29:21.000000 pm4py-2.7.9.3/pm4py/statistics/sojourn_time/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:40.580669 pm4py-2.7.9.3/pm4py/statistics/start_activities/
--rw-rw-rw-   0        0        0      801 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/statistics/start_activities/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:40.604128 pm4py-2.7.9.3/pm4py/statistics/start_activities/common/
--rw-rw-rw-   0        0        0      792 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/statistics/start_activities/common/__init__.py
--rw-rw-rw-   0        0        0     1813 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/statistics/start_activities/common/get.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:40.626701 pm4py-2.7.9.3/pm4py/statistics/start_activities/log/
--rw-rw-rw-   0        0        0      789 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/statistics/start_activities/log/__init__.py
--rw-rw-rw-   0        0        0     2769 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/statistics/start_activities/log/get.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:40.648884 pm4py-2.7.9.3/pm4py/statistics/start_activities/pandas/
--rw-rw-rw-   0        0        0      792 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/statistics/start_activities/pandas/__init__.py
--rw-rw-rw-   0        0        0     2623 2024-01-15 12:00:43.000000 pm4py-2.7.9.3/pm4py/statistics/start_activities/pandas/get.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:40.660469 pm4py-2.7.9.3/pm4py/statistics/traces/
--rw-rw-rw-   0        0        0      791 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/statistics/traces/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:40.673158 pm4py-2.7.9.3/pm4py/statistics/traces/cycle_time/
--rw-rw-rw-   0        0        0      800 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/statistics/traces/cycle_time/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:40.695009 pm4py-2.7.9.3/pm4py/statistics/traces/cycle_time/log/
--rw-rw-rw-   0        0        0      790 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/statistics/traces/cycle_time/log/__init__.py
--rw-rw-rw-   0        0        0     3191 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/statistics/traces/cycle_time/log/get.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:40.720148 pm4py-2.7.9.3/pm4py/statistics/traces/cycle_time/pandas/
--rw-rw-rw-   0        0        0      793 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/statistics/traces/cycle_time/pandas/__init__.py
--rw-rw-rw-   0        0        0     3255 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/statistics/traces/cycle_time/pandas/get.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:40.743858 pm4py-2.7.9.3/pm4py/statistics/traces/cycle_time/util/
--rw-rw-rw-   0        0        0      795 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/statistics/traces/cycle_time/util/__init__.py
--rw-rw-rw-   0        0        0     2385 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/statistics/traces/cycle_time/util/compute.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:40.757187 pm4py-2.7.9.3/pm4py/statistics/traces/generic/
--rw-rw-rw-   0        0        0      799 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/statistics/traces/generic/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:40.780431 pm4py-2.7.9.3/pm4py/statistics/traces/generic/common/
--rw-rw-rw-   0        0        0      800 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/statistics/traces/generic/common/__init__.py
--rw-rw-rw-   0        0        0     2969 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/statistics/traces/generic/common/case_duration.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:40.814146 pm4py-2.7.9.3/pm4py/statistics/traces/generic/log/
--rw-rw-rw-   0        0        0      799 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/statistics/traces/generic/log/__init__.py
--rw-rw-rw-   0        0        0     5237 2024-01-02 13:29:21.000000 pm4py-2.7.9.3/pm4py/statistics/traces/generic/log/case_arrival.py
--rw-rw-rw-   0        0        0    13221 2024-01-02 13:29:21.000000 pm4py-2.7.9.3/pm4py/statistics/traces/generic/log/case_statistics.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:40.848810 pm4py-2.7.9.3/pm4py/statistics/traces/generic/pandas/
--rw-rw-rw-   0        0        0      799 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/statistics/traces/generic/pandas/__init__.py
--rw-rw-rw-   0        0        0     4223 2024-01-15 12:00:43.000000 pm4py-2.7.9.3/pm4py/statistics/traces/generic/pandas/case_arrival.py
--rw-rw-rw-   0        0        0    16954 2024-01-15 12:00:43.000000 pm4py-2.7.9.3/pm4py/statistics/traces/generic/pandas/case_statistics.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:40.872951 pm4py-2.7.9.3/pm4py/statistics/util/
--rw-rw-rw-   0        0        0      974 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/statistics/util/__init__.py
--rw-rw-rw-   0        0        0     2382 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/statistics/util/times_bipartite_matching.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:40.885106 pm4py-2.7.9.3/pm4py/statistics/variants/
--rw-rw-rw-   0        0        0      785 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/statistics/variants/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:40.906359 pm4py-2.7.9.3/pm4py/statistics/variants/log/
--rw-rw-rw-   0        0        0      781 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/statistics/variants/log/__init__.py
--rw-rw-rw-   0        0        0     7359 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/statistics/variants/log/get.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:40.930682 pm4py-2.7.9.3/pm4py/statistics/variants/pandas/
--rw-rw-rw-   0        0        0      784 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/statistics/variants/pandas/__init__.py
--rw-rw-rw-   0        0        0     2254 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/statistics/variants/pandas/get.py
--rw-rw-rw-   0        0        0    39292 2024-01-15 12:00:43.000000 pm4py-2.7.9.3/pm4py/stats.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:40.943177 pm4py-2.7.9.3/pm4py/streaming/
--rw-rw-rw-   0        0        0      804 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/streaming/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:40.964395 pm4py-2.7.9.3/pm4py/streaming/algo/
--rw-rw-rw-   0        0        0      800 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/streaming/algo/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:40.976519 pm4py-2.7.9.3/pm4py/streaming/algo/conformance/
--rw-rw-rw-   0        0        0      806 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/streaming/algo/conformance/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:40.998171 pm4py-2.7.9.3/pm4py/streaming/algo/conformance/footprints/
--rw-rw-rw-   0        0        0      811 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/streaming/algo/conformance/footprints/__init__.py
--rw-rw-rw-   0        0        0     1515 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/streaming/algo/conformance/footprints/algorithm.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:41.021992 pm4py-2.7.9.3/pm4py/streaming/algo/conformance/footprints/variants/
--rw-rw-rw-   0        0        0      808 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/streaming/algo/conformance/footprints/variants/__init__.py
--rw-rw-rw-   0        0        0    11003 2024-01-02 13:29:21.000000 pm4py-2.7.9.3/pm4py/streaming/algo/conformance/footprints/variants/classic.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:41.044119 pm4py-2.7.9.3/pm4py/streaming/algo/conformance/tbr/
--rw-rw-rw-   0        0        0      804 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/streaming/algo/conformance/tbr/__init__.py
--rw-rw-rw-   0        0        0     1523 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/streaming/algo/conformance/tbr/algorithm.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:41.069597 pm4py-2.7.9.3/pm4py/streaming/algo/conformance/tbr/variants/
--rw-rw-rw-   0        0        0      801 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/streaming/algo/conformance/tbr/variants/__init__.py
--rw-rw-rw-   0        0        0    17271 2024-01-02 13:29:21.000000 pm4py-2.7.9.3/pm4py/streaming/algo/conformance/tbr/variants/classic.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:41.095029 pm4py-2.7.9.3/pm4py/streaming/algo/conformance/temporal/
--rw-rw-rw-   0        0        0      809 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/streaming/algo/conformance/temporal/__init__.py
--rw-rw-rw-   0        0        0     2135 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/streaming/algo/conformance/temporal/algorithm.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:41.124314 pm4py-2.7.9.3/pm4py/streaming/algo/conformance/temporal/variants/
--rw-rw-rw-   0        0        0      806 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/streaming/algo/conformance/temporal/variants/__init__.py
--rw-rw-rw-   0        0        0     9602 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/streaming/algo/conformance/temporal/variants/classic.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:41.139667 pm4py-2.7.9.3/pm4py/streaming/algo/discovery/
--rw-rw-rw-   0        0        0      782 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/streaming/algo/discovery/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:41.161072 pm4py-2.7.9.3/pm4py/streaming/algo/discovery/dfg/
--rw-rw-rw-   0        0        0      802 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/streaming/algo/discovery/dfg/__init__.py
--rw-rw-rw-   0        0        0     1411 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/streaming/algo/discovery/dfg/algorithm.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:41.186910 pm4py-2.7.9.3/pm4py/streaming/algo/discovery/dfg/variants/
--rw-rw-rw-   0        0        0      801 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/streaming/algo/discovery/dfg/variants/__init__.py
--rw-rw-rw-   0        0        0     7371 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/streaming/algo/discovery/dfg/variants/frequency.py
--rw-rw-rw-   0        0        0     1476 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/streaming/algo/interface.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:41.222625 pm4py-2.7.9.3/pm4py/streaming/conversion/
--rw-rw-rw-   0        0        0     1468 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/streaming/conversion/__init__.py
--rw-rw-rw-   0        0        0     4925 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/streaming/conversion/from_pandas.py
--rw-rw-rw-   0        0        0     5211 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/streaming/conversion/ocel_flatts_distributor.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:41.234678 pm4py-2.7.9.3/pm4py/streaming/importer/
--rw-rw-rw-   0        0        0      885 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/streaming/importer/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:41.256114 pm4py-2.7.9.3/pm4py/streaming/importer/csv/
--rw-rw-rw-   0        0        0      795 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/streaming/importer/csv/__init__.py
--rw-rw-rw-   0        0        0     1488 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/streaming/importer/csv/importer.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:41.278369 pm4py-2.7.9.3/pm4py/streaming/importer/csv/variants/
--rw-rw-rw-   0        0        0      802 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/streaming/importer/csv/variants/__init__.py
--rw-rw-rw-   0        0        0     3406 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/streaming/importer/csv/variants/csv_event_stream.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:41.301660 pm4py-2.7.9.3/pm4py/streaming/importer/xes/
--rw-rw-rw-   0        0        0      795 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/streaming/importer/xes/__init__.py
--rw-rw-rw-   0        0        0     1523 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/streaming/importer/xes/importer.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:41.335706 pm4py-2.7.9.3/pm4py/streaming/importer/xes/variants/
--rw-rw-rw-   0        0        0      820 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/streaming/importer/xes/variants/__init__.py
--rw-rw-rw-   0        0        0     9461 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/streaming/importer/xes/variants/xes_event_stream.py
--rw-rw-rw-   0        0        0     9317 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/streaming/importer/xes/variants/xes_trace_stream.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:41.367032 pm4py-2.7.9.3/pm4py/streaming/stream/
--rw-rw-rw-   0        0        0      807 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/streaming/stream/__init__.py
--rw-rw-rw-   0        0        0     3109 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/streaming/stream/live_event_stream.py
--rw-rw-rw-   0        0        0     3109 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/streaming/stream/live_trace_stream.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:41.409681 pm4py-2.7.9.3/pm4py/streaming/util/
--rw-rw-rw-   0        0        0      819 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/streaming/util/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:41.434360 pm4py-2.7.9.3/pm4py/streaming/util/dictio/
--rw-rw-rw-   0        0        0      795 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/streaming/util/dictio/__init__.py
--rw-rw-rw-   0        0        0     1461 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/streaming/util/dictio/generator.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:41.479320 pm4py-2.7.9.3/pm4py/streaming/util/dictio/versions/
--rw-rw-rw-   0        0        0      805 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/streaming/util/dictio/versions/__init__.py
--rw-rw-rw-   0        0        0      941 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/streaming/util/dictio/versions/classic.py
--rw-rw-rw-   0        0        0     3540 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/streaming/util/dictio/versions/redis.py
--rw-rw-rw-   0        0        0     1949 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/streaming/util/dictio/versions/thread_safe.py
--rw-rw-rw-   0        0        0     1039 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/streaming/util/event_stream_printer.py
--rw-rw-rw-   0        0        0     1180 2024-01-04 10:14:42.000000 pm4py-2.7.9.3/pm4py/streaming/util/live_to_static_stream.py
--rw-rw-rw-   0        0        0     1039 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/streaming/util/trace_stream_printer.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:41.638096 pm4py-2.7.9.3/pm4py/util/
--rw-rw-rw-   0        0        0      918 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/util/__init__.py
--rw-rw-rw-   0        0        0     5056 2024-01-02 13:29:21.000000 pm4py-2.7.9.3/pm4py/util/business_hours.py
--rw-rw-rw-   0        0        0     2225 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/util/colors.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:41.674054 pm4py-2.7.9.3/pm4py/util/compression/
--rw-rw-rw-   0        0        0      781 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/util/compression/__init__.py
--rw-rw-rw-   0        0        0     1314 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/util/compression/dtypes.py
--rw-rw-rw-   0        0        0    11522 2024-01-02 13:29:21.000000 pm4py-2.7.9.3/pm4py/util/compression/util.py
--rw-rw-rw-   0        0        0     7079 2024-01-02 13:29:21.000000 pm4py-2.7.9.3/pm4py/util/constants.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:41.698408 pm4py-2.7.9.3/pm4py/util/dt_parsing/
--rw-rw-rw-   0        0        0      786 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/util/dt_parsing/__init__.py
--rw-rw-rw-   0        0        0     2682 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/util/dt_parsing/parser.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:41.747894 pm4py-2.7.9.3/pm4py/util/dt_parsing/variants/
--rw-rw-rw-   0        0        0      734 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/util/dt_parsing/variants/__init__.py
--rw-rw-rw-   0        0        0     1029 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/util/dt_parsing/variants/cs8601.py
--rw-rw-rw-   0        0        0     1470 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/util/dt_parsing/variants/dummy.py
--rw-rw-rw-   0        0        0     1916 2024-01-02 13:29:21.000000 pm4py-2.7.9.3/pm4py/util/dt_parsing/variants/strpfromiso.py
--rw-rw-rw-   0        0        0     1564 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/util/exec_utils.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:41.770000 pm4py-2.7.9.3/pm4py/util/lp/
--rw-rw-rw-   0        0        0      784 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/util/lp/__init__.py
--rw-rw-rw-   0        0        0     5457 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/util/lp/solver.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:41.772614 pm4py-2.7.9.3/pm4py/util/lp/util/
--rw-rw-rw-   0        0        0      734 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/util/lp/util/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:41.875128 pm4py-2.7.9.3/pm4py/util/lp/variants/
--rw-rw-rw-   0        0        0      943 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/util/lp/variants/__init__.py
--rw-rw-rw-   0        0        0     3639 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/util/lp/variants/cvxopt_solver.py
--rw-rw-rw-   0        0        0     3420 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/util/lp/variants/cvxopt_solver_custom_align.py
--rw-rw-rw-   0        0        0     3059 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/util/lp/variants/cvxopt_solver_custom_align_arm.py
--rw-rw-rw-   0        0        0     3937 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/util/lp/variants/cvxopt_solver_custom_align_ilp.py
--rw-rw-rw-   0        0        0     5153 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/util/lp/variants/ortools_solver.py
--rw-rw-rw-   0        0        0     6293 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/util/lp/variants/pulp_solver.py
--rw-rw-rw-   0        0        0     1853 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/util/lp/variants/scipy_solver.py
--rw-rw-rw-   0        0        0     9895 2024-01-02 13:29:21.000000 pm4py-2.7.9.3/pm4py/util/nx_utils.py
--rw-rw-rw-   0        0        0    13899 2024-01-15 12:00:43.000000 pm4py-2.7.9.3/pm4py/util/pandas_utils.py
--rw-rw-rw-   0        0        0     1494 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/util/points_subset.py
--rw-rw-rw-   0        0        0     1602 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/util/regex.py
--rw-rw-rw-   0        0        0     3663 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/util/string_distance.py
--rw-rw-rw-   0        0        0     1095 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/util/typing.py
--rw-rw-rw-   0        0        0     2261 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/util/variants_util.py
--rw-rw-rw-   0        0        0     6027 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/util/vis_utils.py
--rw-rw-rw-   0        0        0     1614 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/util/xes_constants.py
--rw-rw-rw-   0        0        0    25437 2024-01-15 12:00:43.000000 pm4py-2.7.9.3/pm4py/utils.py
--rw-rw-rw-   0        0        0    69901 2024-01-02 13:29:21.000000 pm4py-2.7.9.3/pm4py/vis.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:41.887572 pm4py-2.7.9.3/pm4py/visualization/
--rw-rw-rw-   0        0        0     1869 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/visualization/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:41.909433 pm4py-2.7.9.3/pm4py/visualization/align_table/
--rw-rw-rw-   0        0        0      790 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/visualization/align_table/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:41.932866 pm4py-2.7.9.3/pm4py/visualization/align_table/variants/
--rw-rw-rw-   0        0        0      796 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/visualization/align_table/variants/__init__.py
--rw-rw-rw-   0        0        0     3863 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/visualization/align_table/variants/classic.py
--rw-rw-rw-   0        0        0     2968 2024-01-02 13:29:21.000000 pm4py-2.7.9.3/pm4py/visualization/align_table/visualizer.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:41.955059 pm4py-2.7.9.3/pm4py/visualization/bpmn/
--rw-rw-rw-   0        0        0      793 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/visualization/bpmn/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:41.976715 pm4py-2.7.9.3/pm4py/visualization/bpmn/variants/
--rw-rw-rw-   0        0        0      789 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/visualization/bpmn/variants/__init__.py
--rw-rw-rw-   0        0        0     3654 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/visualization/bpmn/variants/classic.py
--rw-rw-rw-   0        0        0     2583 2024-01-02 13:29:21.000000 pm4py-2.7.9.3/pm4py/visualization/bpmn/visualizer.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:42.075568 pm4py-2.7.9.3/pm4py/visualization/common/
--rw-rw-rw-   0        0        0      817 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/visualization/common/__init__.py
--rw-rw-rw-   0        0        0     1160 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/visualization/common/dot_util.py
--rw-rw-rw-   0        0        0     3058 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/visualization/common/gview.py
--rw-rw-rw-   0        0        0     3394 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/visualization/common/html.py
--rw-rw-rw-   0        0        0     1531 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/visualization/common/save.py
--rw-rw-rw-   0        0        0     2526 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/visualization/common/svg_pos_parser.py
--rw-rw-rw-   0        0        0      879 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/visualization/common/utils.py
--rw-rw-rw-   0        0        0     1540 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/visualization/common/visualizer.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:42.109102 pm4py-2.7.9.3/pm4py/visualization/decisiontree/
--rw-rw-rw-   0        0        0     1008 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/visualization/decisiontree/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:42.124212 pm4py-2.7.9.3/pm4py/visualization/decisiontree/util/
--rw-rw-rw-   0        0        0      734 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/visualization/decisiontree/util/__init__.py
--rw-rw-rw-   0        0        0     2621 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/visualization/decisiontree/util/dt_to_string.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:42.146548 pm4py-2.7.9.3/pm4py/visualization/decisiontree/variants/
--rw-rw-rw-   0        0        0      797 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/visualization/decisiontree/variants/__init__.py
--rw-rw-rw-   0        0        0     2231 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/visualization/decisiontree/variants/classic.py
--rw-rw-rw-   0        0        0     2840 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/visualization/decisiontree/visualizer.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:42.169663 pm4py-2.7.9.3/pm4py/visualization/dfg/
--rw-rw-rw-   0        0        0      800 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/visualization/dfg/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:42.196722 pm4py-2.7.9.3/pm4py/visualization/dfg/util/
--rw-rw-rw-   0        0        0      787 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/visualization/dfg/util/__init__.py
--rw-rw-rw-   0        0        0     8994 2024-01-02 13:29:21.000000 pm4py-2.7.9.3/pm4py/visualization/dfg/util/dfg_gviz.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:42.256202 pm4py-2.7.9.3/pm4py/visualization/dfg/variants/
--rw-rw-rw-   0        0        0      803 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/visualization/dfg/variants/__init__.py
--rw-rw-rw-   0        0        0     5409 2024-01-02 13:29:21.000000 pm4py-2.7.9.3/pm4py/visualization/dfg/variants/cost.py
--rw-rw-rw-   0        0        0     5157 2024-01-02 13:29:21.000000 pm4py-2.7.9.3/pm4py/visualization/dfg/variants/frequency.py
--rw-rw-rw-   0        0        0     5580 2024-01-02 13:29:21.000000 pm4py-2.7.9.3/pm4py/visualization/dfg/variants/performance.py
--rw-rw-rw-   0        0        0    12854 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/visualization/dfg/variants/timeline.py
--rw-rw-rw-   0        0        0     3196 2024-01-02 13:29:21.000000 pm4py-2.7.9.3/pm4py/visualization/dfg/visualizer.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:42.281348 pm4py-2.7.9.3/pm4py/visualization/dotted_chart/
--rw-rw-rw-   0        0        0      801 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/visualization/dotted_chart/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:42.305000 pm4py-2.7.9.3/pm4py/visualization/dotted_chart/variants/
--rw-rw-rw-   0        0        0      797 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/visualization/dotted_chart/variants/__init__.py
--rw-rw-rw-   0        0        0     9236 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/visualization/dotted_chart/variants/classic.py
--rw-rw-rw-   0        0        0     3819 2024-01-02 13:29:21.000000 pm4py-2.7.9.3/pm4py/visualization/dotted_chart/visualizer.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:42.327644 pm4py-2.7.9.3/pm4py/visualization/footprints/
--rw-rw-rw-   0        0        0      799 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/visualization/footprints/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:42.372482 pm4py-2.7.9.3/pm4py/visualization/footprints/variants/
--rw-rw-rw-   0        0        0      828 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/visualization/footprints/variants/__init__.py
--rw-rw-rw-   0        0        0     3842 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/visualization/footprints/variants/comparison.py
--rw-rw-rw-   0        0        0     4374 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/visualization/footprints/variants/comparison_symmetric.py
--rw-rw-rw-   0        0        0     3280 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/visualization/footprints/variants/single.py
--rw-rw-rw-   0        0        0     3120 2024-01-02 13:29:21.000000 pm4py-2.7.9.3/pm4py/visualization/footprints/visualizer.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:42.394739 pm4py-2.7.9.3/pm4py/visualization/graphs/
--rw-rw-rw-   0        0        0      801 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/visualization/graphs/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:42.420068 pm4py-2.7.9.3/pm4py/visualization/graphs/util/
--rw-rw-rw-   0        0        0      786 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/visualization/graphs/util/__init__.py
--rw-rw-rw-   0        0        0     2849 2024-01-02 13:29:21.000000 pm4py-2.7.9.3/pm4py/visualization/graphs/util/common.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:42.473102 pm4py-2.7.9.3/pm4py/visualization/graphs/variants/
--rw-rw-rw-   0        0        0      817 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/visualization/graphs/variants/__init__.py
--rw-rw-rw-   0        0        0     4541 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/visualization/graphs/variants/attributes.py
--rw-rw-rw-   0        0        0     2763 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/visualization/graphs/variants/barplot.py
--rw-rw-rw-   0        0        0     4542 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/visualization/graphs/variants/cases.py
--rw-rw-rw-   0        0        0     4587 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/visualization/graphs/variants/dates.py
--rw-rw-rw-   0        0        0     3859 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/visualization/graphs/visualizer.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:42.495440 pm4py-2.7.9.3/pm4py/visualization/heuristics_net/
--rw-rw-rw-   0        0        0      803 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/visualization/heuristics_net/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:42.517888 pm4py-2.7.9.3/pm4py/visualization/heuristics_net/variants/
--rw-rw-rw-   0        0        0      805 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/visualization/heuristics_net/variants/__init__.py
--rw-rw-rw-   0        0        0    13357 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/visualization/heuristics_net/variants/pydotplus_vis.py
--rw-rw-rw-   0        0        0     4471 2024-01-02 13:29:21.000000 pm4py-2.7.9.3/pm4py/visualization/heuristics_net/visualizer.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:42.539193 pm4py-2.7.9.3/pm4py/visualization/network_analysis/
--rw-rw-rw-   0        0        0      805 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/visualization/network_analysis/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:42.572823 pm4py-2.7.9.3/pm4py/visualization/network_analysis/variants/
--rw-rw-rw-   0        0        0      816 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/visualization/network_analysis/variants/__init__.py
--rw-rw-rw-   0        0        0     4975 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/visualization/network_analysis/variants/frequency.py
--rw-rw-rw-   0        0        0     6154 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/visualization/network_analysis/variants/performance.py
--rw-rw-rw-   0        0        0     2496 2024-01-02 13:29:21.000000 pm4py-2.7.9.3/pm4py/visualization/network_analysis/visualizer.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:42.585779 pm4py-2.7.9.3/pm4py/visualization/networkx/
--rw-rw-rw-   0        0        0      734 2024-01-02 13:29:21.000000 pm4py-2.7.9.3/pm4py/visualization/networkx/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:42.599018 pm4py-2.7.9.3/pm4py/visualization/networkx/variants/
--rw-rw-rw-   0        0        0      734 2024-01-02 13:29:21.000000 pm4py-2.7.9.3/pm4py/visualization/networkx/variants/__init__.py
--rw-rw-rw-   0        0        0     3990 2024-01-02 13:29:21.000000 pm4py-2.7.9.3/pm4py/visualization/networkx/variants/digraph.py
--rw-rw-rw-   0        0        0     2362 2024-01-02 13:29:21.000000 pm4py-2.7.9.3/pm4py/visualization/networkx/visualizer.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:42.610090 pm4py-2.7.9.3/pm4py/visualization/ocel/
--rw-rw-rw-   0        0        0      813 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/visualization/ocel/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:42.624939 pm4py-2.7.9.3/pm4py/visualization/ocel/eve_to_obj_types/
--rw-rw-rw-   0        0        0      734 2024-01-02 13:29:21.000000 pm4py-2.7.9.3/pm4py/visualization/ocel/eve_to_obj_types/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:42.639026 pm4py-2.7.9.3/pm4py/visualization/ocel/eve_to_obj_types/variants/
--rw-rw-rw-   0        0        0      734 2024-01-02 13:29:21.000000 pm4py-2.7.9.3/pm4py/visualization/ocel/eve_to_obj_types/variants/__init__.py
--rw-rw-rw-   0        0        0     3613 2024-01-02 13:29:21.000000 pm4py-2.7.9.3/pm4py/visualization/ocel/eve_to_obj_types/variants/graphviz.py
--rw-rw-rw-   0        0        0     2724 2024-01-02 13:29:21.000000 pm4py-2.7.9.3/pm4py/visualization/ocel/eve_to_obj_types/visualizer.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:42.660499 pm4py-2.7.9.3/pm4py/visualization/ocel/interleavings/
--rw-rw-rw-   0        0        0      807 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/visualization/ocel/interleavings/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:42.684625 pm4py-2.7.9.3/pm4py/visualization/ocel/interleavings/variants/
--rw-rw-rw-   0        0        0      804 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/visualization/ocel/interleavings/variants/__init__.py
--rw-rw-rw-   0        0        0    15031 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/visualization/ocel/interleavings/variants/graphviz.py
--rw-rw-rw-   0        0        0     2989 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/visualization/ocel/interleavings/visualizer.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:42.697149 pm4py-2.7.9.3/pm4py/visualization/ocel/object_graph/
--rw-rw-rw-   0        0        0      734 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/visualization/ocel/object_graph/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:42.711346 pm4py-2.7.9.3/pm4py/visualization/ocel/object_graph/variants/
--rw-rw-rw-   0        0        0      734 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/visualization/ocel/object_graph/variants/__init__.py
--rw-rw-rw-   0        0        0     3447 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/visualization/ocel/object_graph/variants/graphviz.py
--rw-rw-rw-   0        0        0     2556 2024-01-02 13:29:21.000000 pm4py-2.7.9.3/pm4py/visualization/ocel/object_graph/visualizer.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:42.733925 pm4py-2.7.9.3/pm4py/visualization/ocel/ocdfg/
--rw-rw-rw-   0        0        0      799 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/visualization/ocel/ocdfg/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:42.756282 pm4py-2.7.9.3/pm4py/visualization/ocel/ocdfg/variants/
--rw-rw-rw-   0        0        0      795 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/visualization/ocel/ocdfg/variants/__init__.py
--rw-rw-rw-   0        0        0    12507 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/visualization/ocel/ocdfg/variants/classic.py
--rw-rw-rw-   0        0        0     2454 2024-01-02 13:29:21.000000 pm4py-2.7.9.3/pm4py/visualization/ocel/ocdfg/visualizer.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:42.779545 pm4py-2.7.9.3/pm4py/visualization/ocel/ocpn/
--rw-rw-rw-   0        0        0      798 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/visualization/ocel/ocpn/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:42.807830 pm4py-2.7.9.3/pm4py/visualization/ocel/ocpn/variants/
--rw-rw-rw-   0        0        0      800 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/visualization/ocel/ocpn/variants/__init__.py
--rw-rw-rw-   0        0        0     5941 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/visualization/ocel/ocpn/variants/wo_decoration.py
--rw-rw-rw-   0        0        0     2601 2024-01-02 13:29:21.000000 pm4py-2.7.9.3/pm4py/visualization/ocel/ocpn/visualizer.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:42.831330 pm4py-2.7.9.3/pm4py/visualization/performance_spectrum/
--rw-rw-rw-   0        0        0      809 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/visualization/performance_spectrum/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:42.854085 pm4py-2.7.9.3/pm4py/visualization/performance_spectrum/variants/
--rw-rw-rw-   0        0        0      803 2023-12-11 09:33:53.000000 pm4py-2.7.9.3/pm4py/visualization/performance_spectrum/variants/__init__.py
--rw-rw-rw-   0        0        0     7116 2024-01-02 13:29:21.000000 pm4py-2.7.9.3/pm4py/visualization/performance_spectrum/variants/neato.py
--rw-rw-rw-   0        0        0     3244 2024-01-02 13:29:21.000000 pm4py-2.7.9.3/pm4py/visualization/performance_spectrum/visualizer.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:42.876571 pm4py-2.7.9.3/pm4py/visualization/petri_net/
--rw-rw-rw-   0        0        0      812 2023-12-11 09:33:54.000000 pm4py-2.7.9.3/pm4py/visualization/petri_net/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:42.901642 pm4py-2.7.9.3/pm4py/visualization/petri_net/common/
--rw-rw-rw-   0        0        0      794 2023-12-11 09:33:54.000000 pm4py-2.7.9.3/pm4py/visualization/petri_net/common/__init__.py
--rw-rw-rw-   0        0        0     9446 2023-12-11 09:33:54.000000 pm4py-2.7.9.3/pm4py/visualization/petri_net/common/visualize.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:42.948604 pm4py-2.7.9.3/pm4py/visualization/petri_net/util/
--rw-rw-rw-   0        0        0      847 2023-12-11 09:33:54.000000 pm4py-2.7.9.3/pm4py/visualization/petri_net/util/__init__.py
--rw-rw-rw-   0        0        0     2935 2023-12-11 09:33:54.000000 pm4py-2.7.9.3/pm4py/visualization/petri_net/util/alignments_decoration.py
--rw-rw-rw-   0        0        0     1121 2023-12-11 09:33:54.000000 pm4py-2.7.9.3/pm4py/visualization/petri_net/util/performance_map.py
--rw-rw-rw-   0        0        0    11279 2023-12-11 09:33:54.000000 pm4py-2.7.9.3/pm4py/visualization/petri_net/util/vis_trans_shortest_paths.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:43.028524 pm4py-2.7.9.3/pm4py/visualization/petri_net/variants/
--rw-rw-rw-   0        0        0      937 2023-12-11 09:33:54.000000 pm4py-2.7.9.3/pm4py/visualization/petri_net/variants/__init__.py
--rw-rw-rw-   0        0        0     2044 2023-12-11 09:33:54.000000 pm4py-2.7.9.3/pm4py/visualization/petri_net/variants/alignments.py
--rw-rw-rw-   0        0        0     4730 2023-12-11 09:33:54.000000 pm4py-2.7.9.3/pm4py/visualization/petri_net/variants/greedy_decoration_frequency.py
--rw-rw-rw-   0        0        0     4837 2023-12-11 09:33:54.000000 pm4py-2.7.9.3/pm4py/visualization/petri_net/variants/greedy_decoration_performance.py
--rw-rw-rw-   0        0        0     5670 2023-12-11 09:33:54.000000 pm4py-2.7.9.3/pm4py/visualization/petri_net/variants/token_decoration_frequency.py
--rw-rw-rw-   0        0        0     5880 2023-12-11 09:33:54.000000 pm4py-2.7.9.3/pm4py/visualization/petri_net/variants/token_decoration_performance.py
--rw-rw-rw-   0        0        0     2237 2023-12-11 09:33:54.000000 pm4py-2.7.9.3/pm4py/visualization/petri_net/variants/wo_decoration.py
--rw-rw-rw-   0        0        0     3651 2024-01-02 13:29:21.000000 pm4py-2.7.9.3/pm4py/visualization/petri_net/visualizer.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:43.050804 pm4py-2.7.9.3/pm4py/visualization/powl/
--rw-rw-rw-   0        0        0      795 2023-12-11 09:33:54.000000 pm4py-2.7.9.3/pm4py/visualization/powl/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:43.095971 pm4py-2.7.9.3/pm4py/visualization/powl/variants/
--rw-rw-rw-   0        0        0      785 2023-12-11 09:33:54.000000 pm4py-2.7.9.3/pm4py/visualization/powl/variants/__init__.py
--rw-rw-rw-   0        0        0     7745 2024-01-02 13:29:21.000000 pm4py-2.7.9.3/pm4py/visualization/powl/variants/basic.py
--rw-rw-rw-   0        0        0      755 2024-01-02 13:29:21.000000 pm4py-2.7.9.3/pm4py/visualization/powl/variants/end.png
--rw-rw-rw-   0        0        0    25337 2024-01-02 13:29:21.000000 pm4py-2.7.9.3/pm4py/visualization/powl/variants/loop.png
--rw-rw-rw-   0        0        0    11069 2024-01-02 13:29:21.000000 pm4py-2.7.9.3/pm4py/visualization/powl/variants/net.py
--rw-rw-rw-   0        0        0      922 2024-01-02 13:29:21.000000 pm4py-2.7.9.3/pm4py/visualization/powl/variants/play.png
--rw-rw-rw-   0        0        0    78865 2024-01-02 13:29:21.000000 pm4py-2.7.9.3/pm4py/visualization/powl/variants/xor.png
--rw-rw-rw-   0        0        0     2853 2024-01-02 13:29:21.000000 pm4py-2.7.9.3/pm4py/visualization/powl/visualizer.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:43.120077 pm4py-2.7.9.3/pm4py/visualization/process_tree/
--rw-rw-rw-   0        0        0      801 2023-12-11 09:33:54.000000 pm4py-2.7.9.3/pm4py/visualization/process_tree/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:43.166721 pm4py-2.7.9.3/pm4py/visualization/process_tree/variants/
--rw-rw-rw-   0        0        0      813 2023-12-11 09:33:54.000000 pm4py-2.7.9.3/pm4py/visualization/process_tree/variants/__init__.py
--rw-rw-rw-   0        0        0     4873 2023-12-11 09:33:54.000000 pm4py-2.7.9.3/pm4py/visualization/process_tree/variants/frequency_annotation.py
--rw-rw-rw-   0        0        0     4104 2023-12-11 09:33:54.000000 pm4py-2.7.9.3/pm4py/visualization/process_tree/variants/symbolic.py
--rw-rw-rw-   0        0        0     4256 2023-12-11 09:33:54.000000 pm4py-2.7.9.3/pm4py/visualization/process_tree/variants/wo_decoration.py
--rw-rw-rw-   0        0        0     3017 2024-01-02 13:29:21.000000 pm4py-2.7.9.3/pm4py/visualization/process_tree/visualizer.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:43.188665 pm4py-2.7.9.3/pm4py/visualization/sna/
--rw-rw-rw-   0        0        0      792 2023-12-11 09:33:54.000000 pm4py-2.7.9.3/pm4py/visualization/sna/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:43.221429 pm4py-2.7.9.3/pm4py/visualization/sna/variants/
--rw-rw-rw-   0        0        0      796 2023-12-11 09:33:54.000000 pm4py-2.7.9.3/pm4py/visualization/sna/variants/__init__.py
--rw-rw-rw-   0        0        0     4180 2023-12-11 09:33:54.000000 pm4py-2.7.9.3/pm4py/visualization/sna/variants/networkx.py
--rw-rw-rw-   0        0        0     5472 2023-12-11 09:33:54.000000 pm4py-2.7.9.3/pm4py/visualization/sna/variants/pyvis.py
--rw-rw-rw-   0        0        0     2561 2023-12-11 09:33:54.000000 pm4py-2.7.9.3/pm4py/visualization/sna/visualizer.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:43.244837 pm4py-2.7.9.3/pm4py/visualization/transition_system/
--rw-rw-rw-   0        0        0      812 2023-12-11 09:33:54.000000 pm4py-2.7.9.3/pm4py/visualization/transition_system/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:43.267707 pm4py-2.7.9.3/pm4py/visualization/transition_system/util/
--rw-rw-rw-   0        0        0      809 2023-12-11 09:33:54.000000 pm4py-2.7.9.3/pm4py/visualization/transition_system/util/__init__.py
--rw-rw-rw-   0        0        0     3315 2023-12-11 09:33:54.000000 pm4py-2.7.9.3/pm4py/visualization/transition_system/util/visualize_graphviz.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:43.300758 pm4py-2.7.9.3/pm4py/visualization/transition_system/variants/
--rw-rw-rw-   0        0        0      822 2023-12-11 09:33:54.000000 pm4py-2.7.9.3/pm4py/visualization/transition_system/variants/__init__.py
--rw-rw-rw-   0        0        0     3138 2023-12-11 09:33:54.000000 pm4py-2.7.9.3/pm4py/visualization/transition_system/variants/trans_frequency.py
--rw-rw-rw-   0        0        0     1652 2023-12-11 09:33:54.000000 pm4py-2.7.9.3/pm4py/visualization/transition_system/variants/view_based.py
--rw-rw-rw-   0        0        0     2703 2024-01-02 13:29:21.000000 pm4py-2.7.9.3/pm4py/visualization/transition_system/visualizer.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:43.322969 pm4py-2.7.9.3/pm4py/visualization/trie/
--rw-rw-rw-   0        0        0      793 2023-12-11 09:33:54.000000 pm4py-2.7.9.3/pm4py/visualization/trie/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:43.344402 pm4py-2.7.9.3/pm4py/visualization/trie/variants/
--rw-rw-rw-   0        0        0      789 2023-12-11 09:33:54.000000 pm4py-2.7.9.3/pm4py/visualization/trie/variants/__init__.py
--rw-rw-rw-   0        0        0     2765 2023-12-11 09:33:54.000000 pm4py-2.7.9.3/pm4py/visualization/trie/variants/classic.py
--rw-rw-rw-   0        0        0     2512 2024-01-02 13:29:21.000000 pm4py-2.7.9.3/pm4py/visualization/trie/visualizer.py
--rw-rw-rw-   0        0        0    15531 2023-12-11 09:33:54.000000 pm4py-2.7.9.3/pm4py/write.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:43.356516 pm4py-2.7.9.3/pm4py.egg-info/
--rw-rw-rw-   0        0        0     3629 2024-01-16 10:10:26.000000 pm4py-2.7.9.3/pm4py.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0    66549 2024-01-16 10:10:27.000000 pm4py-2.7.9.3/pm4py.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-01-16 10:10:26.000000 pm4py-2.7.9.3/pm4py.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      144 2024-01-16 10:10:26.000000 pm4py-2.7.9.3/pm4py.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2024-01-16 10:10:26.000000 pm4py-2.7.9.3/pm4py.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-01-16 10:10:43.360753 pm4py-2.7.9.3/setup.cfg
--rw-rw-rw-   0        0        0     1246 2023-12-11 09:33:54.000000 pm4py-2.7.9.3/setup.py
-drwxrwxrwx   0        0        0        0 2024-01-16 10:10:43.354522 pm4py-2.7.9.3/tests/
--rw-rw-rw-   0        0        0     4971 2023-11-09 06:59:42.000000 pm4py-2.7.9.3/tests/test_cli.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:26.520942 pm4py-2.7.9.4/
+-rw-rw-rw-   0        0        0    34817 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/LICENSE
+-rw-rw-rw-   0        0        0       29 2024-01-04 13:34:19.000000 pm4py-2.7.9.4/MANIFEST.in
+-rw-rw-rw-   0        0        0     3631 2024-01-29 06:14:26.520942 pm4py-2.7.9.4/PKG-INFO
+-rw-rw-rw-   0        0        0     2792 2024-01-29 06:13:52.000000 pm4py-2.7.9.4/README.md
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:23.495785 pm4py-2.7.9.4/pm4py/
+-rw-rw-rw-   0        0        0     7677 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/__init__.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:23.540558 pm4py-2.7.9.4/pm4py/algo/
+-rw-rw-rw-   0        0        0      854 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/__init__.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:23.540558 pm4py-2.7.9.4/pm4py/algo/analysis/
+-rw-rw-rw-   0        0        0      833 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/analysis/__init__.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:23.540558 pm4py-2.7.9.4/pm4py/algo/analysis/extended_marking_equation/
+-rw-rw-rw-   0        0        0      802 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/analysis/extended_marking_equation/__init__.py
+-rw-rw-rw-   0        0        0     3588 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/analysis/extended_marking_equation/algorithm.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:23.556183 pm4py-2.7.9.4/pm4py/algo/analysis/extended_marking_equation/variants/
+-rw-rw-rw-   0        0        0      810 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/analysis/extended_marking_equation/variants/__init__.py
+-rw-rw-rw-   0        0        0    21448 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/analysis/extended_marking_equation/variants/classic.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:23.556183 pm4py-2.7.9.4/pm4py/algo/analysis/marking_equation/
+-rw-rw-rw-   0        0        0      794 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/analysis/marking_equation/__init__.py
+-rw-rw-rw-   0        0        0     2689 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/analysis/marking_equation/algorithm.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:23.556183 pm4py-2.7.9.4/pm4py/algo/analysis/marking_equation/variants/
+-rw-rw-rw-   0        0        0      801 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/analysis/marking_equation/variants/__init__.py
+-rw-rw-rw-   0        0        0    11636 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/analysis/marking_equation/variants/classic.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:23.571806 pm4py-2.7.9.4/pm4py/algo/analysis/woflan/
+-rw-rw-rw-   0        0        0      836 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/analysis/woflan/__init__.py
+-rw-rw-rw-   0        0        0    32308 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/analysis/woflan/algorithm.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:23.571806 pm4py-2.7.9.4/pm4py/algo/analysis/woflan/graphs/
+-rw-rw-rw-   0        0        0      868 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/analysis/woflan/graphs/__init__.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:23.580313 pm4py-2.7.9.4/pm4py/algo/analysis/woflan/graphs/minimal_coverability_graph/
+-rw-rw-rw-   0        0        0      835 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/analysis/woflan/graphs/minimal_coverability_graph/__init__.py
+-rw-rw-rw-   0        0        0     7988 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/analysis/woflan/graphs/minimal_coverability_graph/minimal_coverability_graph.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:23.580313 pm4py-2.7.9.4/pm4py/algo/analysis/woflan/graphs/reachability_graph/
+-rw-rw-rw-   0        0        0      819 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/analysis/woflan/graphs/reachability_graph/__init__.py
+-rw-rw-rw-   0        0        0     2451 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/analysis/woflan/graphs/reachability_graph/reachability_graph.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:23.580313 pm4py-2.7.9.4/pm4py/algo/analysis/woflan/graphs/restricted_coverability_graph/
+-rw-rw-rw-   0        0        0      841 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/analysis/woflan/graphs/restricted_coverability_graph/__init__.py
+-rw-rw-rw-   0        0        0     4061 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/analysis/woflan/graphs/restricted_coverability_graph/restricted_coverability_graph.py
+-rw-rw-rw-   0        0        0     5745 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/analysis/woflan/graphs/utility.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:23.580313 pm4py-2.7.9.4/pm4py/algo/analysis/woflan/not_well_handled_pairs/
+-rw-rw-rw-   0        0        0      820 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/analysis/woflan/not_well_handled_pairs/__init__.py
+-rw-rw-rw-   0        0        0     2632 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/analysis/woflan/not_well_handled_pairs/not_well_handled_pairs.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:23.595945 pm4py-2.7.9.4/pm4py/algo/analysis/woflan/place_invariants/
+-rw-rw-rw-   0        0        0      849 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/analysis/woflan/place_invariants/__init__.py
+-rw-rw-rw-   0        0        0     4300 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/analysis/woflan/place_invariants/place_invariants.py
+-rw-rw-rw-   0        0        0     3668 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/analysis/woflan/place_invariants/s_component.py
+-rw-rw-rw-   0        0        0     1098 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/analysis/woflan/place_invariants/uniform_invariant.py
+-rw-rw-rw-   0        0        0     8333 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/analysis/woflan/place_invariants/utility.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:23.611564 pm4py-2.7.9.4/pm4py/algo/analysis/workflow_net/
+-rw-rw-rw-   0        0        0      800 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/analysis/workflow_net/__init__.py
+-rw-rw-rw-   0        0        0     1542 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/analysis/workflow_net/algorithm.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:23.611564 pm4py-2.7.9.4/pm4py/algo/analysis/workflow_net/variants/
+-rw-rw-rw-   0        0        0      799 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/analysis/workflow_net/variants/__init__.py
+-rw-rw-rw-   0        0        0     3243 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/analysis/workflow_net/variants/petri_net.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:23.611564 pm4py-2.7.9.4/pm4py/algo/anonymization/
+-rw-rw-rw-   0        0        0      979 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/anonymization/__init__.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:23.611564 pm4py-2.7.9.4/pm4py/algo/anonymization/pripel/
+-rw-rw-rw-   0        0        0      807 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/anonymization/pripel/__init__.py
+-rw-rw-rw-   0        0        0     3170 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/anonymization/pripel/algorithm.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:23.627185 pm4py-2.7.9.4/pm4py/algo/anonymization/pripel/util/
+-rw-rw-rw-   0        0        0    13889 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/anonymization/pripel/util/AttributeAnonymizer.py
+-rw-rw-rw-   0        0        0    14468 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/anonymization/pripel/util/TraceMatcher.py
+-rw-rw-rw-   0        0        0      837 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/anonymization/pripel/util/__init__.py
+-rw-rw-rw-   0        0        0     1754 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/anonymization/pripel/util/trace_levenshtein.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:23.627185 pm4py-2.7.9.4/pm4py/algo/anonymization/pripel/variants/
+-rw-rw-rw-   0        0        0      797 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/anonymization/pripel/variants/__init__.py
+-rw-rw-rw-   0        0        0     5291 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/anonymization/pripel/variants/pripel.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:23.627185 pm4py-2.7.9.4/pm4py/algo/anonymization/trace_variant_query/
+-rw-rw-rw-   0        0        0      820 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/anonymization/trace_variant_query/__init__.py
+-rw-rw-rw-   0        0        0     3980 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/anonymization/trace_variant_query/algorithm.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:23.642807 pm4py-2.7.9.4/pm4py/algo/anonymization/trace_variant_query/util/
+-rw-rw-rw-   0        0        0      839 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/anonymization/trace_variant_query/util/__init__.py
+-rw-rw-rw-   0        0        0     6862 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/anonymization/trace_variant_query/util/behavioralAppropriateness.py
+-rw-rw-rw-   0        0        0     1323 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/anonymization/trace_variant_query/util/exp_mech.py
+-rw-rw-rw-   0        0        0     1687 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/anonymization/trace_variant_query/util/util.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:23.658429 pm4py-2.7.9.4/pm4py/algo/anonymization/trace_variant_query/variants/
+-rw-rw-rw-   0        0        0      817 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/anonymization/trace_variant_query/variants/__init__.py
+-rw-rw-rw-   0        0        0     7691 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/anonymization/trace_variant_query/variants/laplace.py
+-rw-rw-rw-   0        0        0    11329 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/anonymization/trace_variant_query/variants/sacofa.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:23.661087 pm4py-2.7.9.4/pm4py/algo/clustering/
+-rw-rw-rw-   0        0        0      734 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/clustering/__init__.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:23.661087 pm4py-2.7.9.4/pm4py/algo/clustering/profiles/
+-rw-rw-rw-   0        0        0      798 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/clustering/profiles/__init__.py
+-rw-rw-rw-   0        0        0     2118 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/clustering/profiles/algorithm.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:23.661087 pm4py-2.7.9.4/pm4py/algo/clustering/profiles/variants/
+-rw-rw-rw-   0        0        0      804 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/clustering/profiles/variants/__init__.py
+-rw-rw-rw-   0        0        0     3544 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/clustering/profiles/variants/sklearn_profiles.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:23.661087 pm4py-2.7.9.4/pm4py/algo/clustering/trace_attribute_driven/
+-rw-rw-rw-   0        0        0     1060 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/clustering/trace_attribute_driven/__init__.py
+-rw-rw-rw-   0        0        0     4705 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/clustering/trace_attribute_driven/algorithm.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:23.676709 pm4py-2.7.9.4/pm4py/algo/clustering/trace_attribute_driven/dfg/
+-rw-rw-rw-   0        0        0      805 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/clustering/trace_attribute_driven/dfg/__init__.py
+-rw-rw-rw-   0        0        0     3989 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/clustering/trace_attribute_driven/dfg/dfg_dist.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:23.680219 pm4py-2.7.9.4/pm4py/algo/clustering/trace_attribute_driven/leven_dist/
+-rw-rw-rw-   0        0        0      819 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/clustering/trace_attribute_driven/leven_dist/__init__.py
+-rw-rw-rw-   0        0        0     5473 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/clustering/trace_attribute_driven/leven_dist/leven_dist_calc.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:23.680219 pm4py-2.7.9.4/pm4py/algo/clustering/trace_attribute_driven/linkage_method/
+-rw-rw-rw-   0        0        0      819 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/clustering/trace_attribute_driven/linkage_method/__init__.py
+-rw-rw-rw-   0        0        0    13583 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/clustering/trace_attribute_driven/linkage_method/linkage_avg.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:23.680219 pm4py-2.7.9.4/pm4py/algo/clustering/trace_attribute_driven/merge_log/
+-rw-rw-rw-   0        0        0      812 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/clustering/trace_attribute_driven/merge_log/__init__.py
+-rw-rw-rw-   0        0        0     4290 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/clustering/trace_attribute_driven/merge_log/merge_log.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:23.695846 pm4py-2.7.9.4/pm4py/algo/clustering/trace_attribute_driven/util/
+-rw-rw-rw-   0        0        0      824 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/clustering/trace_attribute_driven/util/__init__.py
+-rw-rw-rw-   0        0        0     3396 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/clustering/trace_attribute_driven/util/evaluation.py
+-rw-rw-rw-   0        0        0    15776 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/clustering/trace_attribute_driven/util/filter_subsets.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:23.705023 pm4py-2.7.9.4/pm4py/algo/clustering/trace_attribute_driven/variants/
+-rw-rw-rw-   0        0        0      855 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/clustering/trace_attribute_driven/variants/__init__.py
+-rw-rw-rw-   0        0        0    18463 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/clustering/trace_attribute_driven/variants/act_dist_calc.py
+-rw-rw-rw-   0        0        0     6806 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/clustering/trace_attribute_driven/variants/logslice_dist.py
+-rw-rw-rw-   0        0        0     6329 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/clustering/trace_attribute_driven/variants/sim_calc.py
+-rw-rw-rw-   0        0        0    15790 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/clustering/trace_attribute_driven/variants/suc_dist_calc.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:23.705023 pm4py-2.7.9.4/pm4py/algo/comparison/
+-rw-rw-rw-   0        0        0      851 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/comparison/__init__.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:23.705023 pm4py-2.7.9.4/pm4py/algo/comparison/petrinet/
+-rw-rw-rw-   0        0        0      803 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/comparison/petrinet/__init__.py
+-rw-rw-rw-   0        0        0     6719 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/comparison/petrinet/element_usage_comparison.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:23.720649 pm4py-2.7.9.4/pm4py/algo/conformance/
+-rw-rw-rw-   0        0        0      946 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/conformance/__init__.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:23.720649 pm4py-2.7.9.4/pm4py/algo/conformance/alignments/
+-rw-rw-rw-   0        0        0      822 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/conformance/alignments/__init__.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:23.720649 pm4py-2.7.9.4/pm4py/algo/conformance/alignments/decomposed/
+-rw-rw-rw-   0        0        0      812 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/conformance/alignments/decomposed/__init__.py
+-rw-rw-rw-   0        0        0     2018 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/conformance/alignments/decomposed/algorithm.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:23.720649 pm4py-2.7.9.4/pm4py/algo/conformance/alignments/decomposed/variants/
+-rw-rw-rw-   0        0        0      818 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/conformance/alignments/decomposed/variants/__init__.py
+-rw-rw-rw-   0        0        0    19051 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/conformance/alignments/decomposed/variants/recompos_maximal.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:23.736271 pm4py-2.7.9.4/pm4py/algo/conformance/alignments/dfg/
+-rw-rw-rw-   0        0        0      805 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/conformance/alignments/dfg/__init__.py
+-rw-rw-rw-   0        0        0     1956 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/conformance/alignments/dfg/algorithm.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:23.736271 pm4py-2.7.9.4/pm4py/algo/conformance/alignments/dfg/variants/
+-rw-rw-rw-   0        0        0      802 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/conformance/alignments/dfg/variants/__init__.py
+-rw-rw-rw-   0        0        0    24120 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/conformance/alignments/dfg/variants/classic.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:23.736271 pm4py-2.7.9.4/pm4py/algo/conformance/alignments/edit_distance/
+-rw-rw-rw-   0        0        0      815 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/conformance/alignments/edit_distance/__init__.py
+-rw-rw-rw-   0        0        0     1876 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/conformance/alignments/edit_distance/algorithm.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:23.736271 pm4py-2.7.9.4/pm4py/algo/conformance/alignments/edit_distance/variants/
+-rw-rw-rw-   0        0        0      818 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/conformance/alignments/edit_distance/variants/__init__.py
+-rw-rw-rw-   0        0        0    11234 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/conformance/alignments/edit_distance/variants/edit_distance.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:23.751891 pm4py-2.7.9.4/pm4py/algo/conformance/alignments/petri_net/
+-rw-rw-rw-   0        0        0      818 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/conformance/alignments/petri_net/__init__.py
+-rw-rw-rw-   0        0        0    16964 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/conformance/alignments/petri_net/algorithm.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:23.751891 pm4py-2.7.9.4/pm4py/algo/conformance/alignments/petri_net/utils/
+-rw-rw-rw-   0        0        0      812 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/conformance/alignments/petri_net/utils/__init__.py
+-rw-rw-rw-   0        0        0     2896 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/conformance/alignments/petri_net/utils/log_enrichment.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:23.780521 pm4py-2.7.9.4/pm4py/algo/conformance/alignments/petri_net/variants/
+-rw-rw-rw-   0        0        0      925 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/conformance/alignments/petri_net/variants/__init__.py
+-rw-rw-rw-   0        0        0    27553 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/conformance/alignments/petri_net/variants/dijkstra_less_memory.py
+-rw-rw-rw-   0        0        0    17167 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/conformance/alignments/petri_net/variants/dijkstra_no_heuristics.py
+-rw-rw-rw-   0        0        0    23651 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/conformance/alignments/petri_net/variants/discounted_a_star.py
+-rw-rw-rw-   0        0        0    23429 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/conformance/alignments/petri_net/variants/generator_dijkstra_less_memory.py
+-rw-rw-rw-   0        0        0    17357 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/conformance/alignments/petri_net/variants/generator_dijkstra_no_heuristics.py
+-rw-rw-rw-   0        0        0    23978 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/conformance/alignments/petri_net/variants/state_equation_a_star.py
+-rw-rw-rw-   0        0        0    27872 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/conformance/alignments/petri_net/variants/tweaked_state_equation_a_star.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:23.780521 pm4py-2.7.9.4/pm4py/algo/conformance/alignments/process_tree/
+-rw-rw-rw-   0        0        0      820 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/conformance/alignments/process_tree/__init__.py
+-rw-rw-rw-   0        0        0     2203 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/conformance/alignments/process_tree/algorithm.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:23.780521 pm4py-2.7.9.4/pm4py/algo/conformance/alignments/process_tree/util/
+-rw-rw-rw-   0        0        0      870 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/conformance/alignments/process_tree/util/__init__.py
+-rw-rw-rw-   0        0        0     3355 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/conformance/alignments/process_tree/util/search_graph_pt_frequency_annotation.py
+-rw-rw-rw-   0        0        0    15712 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/conformance/alignments/process_tree/util/search_graph_pt_replay_semantics.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:23.796149 pm4py-2.7.9.4/pm4py/algo/conformance/alignments/process_tree/variants/
+-rw-rw-rw-   0        0        0      833 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/conformance/alignments/process_tree/variants/__init__.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:23.798398 pm4py-2.7.9.4/pm4py/algo/conformance/alignments/process_tree/variants/approximated/
+-rw-rw-rw-   0        0        0      871 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/conformance/alignments/process_tree/variants/approximated/__init__.py
+-rw-rw-rw-   0        0        0     5361 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/conformance/alignments/process_tree/variants/approximated/calculate_a_sa_ea_sets.py
+-rw-rw-rw-   0        0        0    49808 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/conformance/alignments/process_tree/variants/approximated/matrix_lp.py
+-rw-rw-rw-   0        0        0    36425 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/conformance/alignments/process_tree/variants/approximated/original.py
+-rw-rw-rw-   0        0        0     6660 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/conformance/alignments/process_tree/variants/approximated/utilities.py
+-rw-rw-rw-   0        0        0    17939 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/conformance/alignments/process_tree/variants/search_graph_pt.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:23.814020 pm4py-2.7.9.4/pm4py/algo/conformance/antialignments/
+-rw-rw-rw-   0        0        0      805 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/conformance/antialignments/__init__.py
+-rw-rw-rw-   0        0        0     3166 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/conformance/antialignments/algorithm.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:23.814020 pm4py-2.7.9.4/pm4py/algo/conformance/antialignments/variants/
+-rw-rw-rw-   0        0        0      812 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/conformance/antialignments/variants/__init__.py
+-rw-rw-rw-   0        0        0     7582 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/conformance/antialignments/variants/discounted_a_star.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:23.814020 pm4py-2.7.9.4/pm4py/algo/conformance/declare/
+-rw-rw-rw-   0        0        0      800 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/conformance/declare/__init__.py
+-rw-rw-rw-   0        0        0     2733 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/conformance/declare/algorithm.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:23.814020 pm4py-2.7.9.4/pm4py/algo/conformance/declare/variants/
+-rw-rw-rw-   0        0        0      797 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/conformance/declare/variants/__init__.py
+-rw-rw-rw-   0        0        0    18351 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/conformance/declare/variants/classic.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:23.829641 pm4py-2.7.9.4/pm4py/algo/conformance/footprints/
+-rw-rw-rw-   0        0        0      807 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/conformance/footprints/__init__.py
+-rw-rw-rw-   0        0        0     2061 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/conformance/footprints/algorithm.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:23.829641 pm4py-2.7.9.4/pm4py/algo/conformance/footprints/util/
+-rw-rw-rw-   0        0        0      817 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/conformance/footprints/util/__init__.py
+-rw-rw-rw-   0        0        0     6154 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/conformance/footprints/util/evaluation.py
+-rw-rw-rw-   0        0        0     3573 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/conformance/footprints/util/tree_visualization.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:23.845267 pm4py-2.7.9.4/pm4py/algo/conformance/footprints/variants/
+-rw-rw-rw-   0        0        0      832 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/conformance/footprints/variants/__init__.py
+-rw-rw-rw-   0        0        0     3708 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/conformance/footprints/variants/log_extensive.py
+-rw-rw-rw-   0        0        0     5119 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/conformance/footprints/variants/log_model.py
+-rw-rw-rw-   0        0        0     7141 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/conformance/footprints/variants/trace_extensive.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:23.845267 pm4py-2.7.9.4/pm4py/algo/conformance/log_skeleton/
+-rw-rw-rw-   0        0        0      803 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/conformance/log_skeleton/__init__.py
+-rw-rw-rw-   0        0        0     4040 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/conformance/log_skeleton/algorithm.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:23.845267 pm4py-2.7.9.4/pm4py/algo/conformance/log_skeleton/variants/
+-rw-rw-rw-   0        0        0      800 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/conformance/log_skeleton/variants/__init__.py
+-rw-rw-rw-   0        0        0    13160 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/conformance/log_skeleton/variants/classic.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:23.860883 pm4py-2.7.9.4/pm4py/algo/conformance/multialignments/
+-rw-rw-rw-   0        0        0      806 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/conformance/multialignments/__init__.py
+-rw-rw-rw-   0        0        0     3143 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/conformance/multialignments/algorithm.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:23.860883 pm4py-2.7.9.4/pm4py/algo/conformance/multialignments/variants/
+-rw-rw-rw-   0        0        0      813 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/conformance/multialignments/variants/__init__.py
+-rw-rw-rw-   0        0        0     6557 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/conformance/multialignments/variants/discounted_a_star.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:23.860883 pm4py-2.7.9.4/pm4py/algo/conformance/temporal_profile/
+-rw-rw-rw-   0        0        0      807 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/conformance/temporal_profile/__init__.py
+-rw-rw-rw-   0        0        0     4738 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/conformance/temporal_profile/algorithm.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:23.880510 pm4py-2.7.9.4/pm4py/algo/conformance/temporal_profile/variants/
+-rw-rw-rw-   0        0        0      811 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/conformance/temporal_profile/variants/__init__.py
+-rw-rw-rw-   0        0        0     5476 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/conformance/temporal_profile/variants/dataframe.py
+-rw-rw-rw-   0        0        0     5957 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/conformance/temporal_profile/variants/log.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:23.880510 pm4py-2.7.9.4/pm4py/algo/conformance/tokenreplay/
+-rw-rw-rw-   0        0        0      815 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/conformance/tokenreplay/__init__.py
+-rw-rw-rw-   0        0        0     2965 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/conformance/tokenreplay/algorithm.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:23.880510 pm4py-2.7.9.4/pm4py/algo/conformance/tokenreplay/diagnostics/
+-rw-rw-rw-   0        0        0      836 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/conformance/tokenreplay/diagnostics/__init__.py
+-rw-rw-rw-   0        0        0     6720 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/conformance/tokenreplay/diagnostics/duration_diagnostics.py
+-rw-rw-rw-   0        0        0    11104 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/conformance/tokenreplay/diagnostics/root_cause_analysis.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:23.896137 pm4py-2.7.9.4/pm4py/algo/conformance/tokenreplay/variants/
+-rw-rw-rw-   0        0        0      804 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/conformance/tokenreplay/variants/__init__.py
+-rw-rw-rw-   0        0        0    12130 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/conformance/tokenreplay/variants/backwards.py
+-rw-rw-rw-   0        0        0    61056 2024-01-22 11:53:06.000000 pm4py-2.7.9.4/pm4py/algo/conformance/tokenreplay/variants/token_replay.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:23.896137 pm4py-2.7.9.4/pm4py/algo/connectors/
+-rw-rw-rw-   0        0        0      786 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/connectors/__init__.py
+-rw-rw-rw-   0        0        0     2768 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/connectors/algorithm.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:23.896137 pm4py-2.7.9.4/pm4py/algo/connectors/util/
+-rw-rw-rw-   0        0        0      781 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/connectors/util/__init__.py
+-rw-rw-rw-   0        0        0     1628 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/connectors/util/mail.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:23.928789 pm4py-2.7.9.4/pm4py/algo/connectors/variants/
+-rw-rw-rw-   0        0        0      736 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/connectors/variants/__init__.py
+-rw-rw-rw-   0        0        0     2592 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/connectors/variants/camunda_workflow.py
+-rw-rw-rw-   0        0        0     3743 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/connectors/variants/chrome_history.py
+-rw-rw-rw-   0        0        0     3777 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/connectors/variants/firefox_history.py
+-rw-rw-rw-   0        0        0     5250 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/connectors/variants/github_repo.py
+-rw-rw-rw-   0        0        0     4432 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/connectors/variants/outlook_calendar.py
+-rw-rw-rw-   0        0        0     4568 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/connectors/variants/outlook_mail_extractor.py
+-rw-rw-rw-   0        0        0     3168 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/connectors/variants/sap_accounting.py
+-rw-rw-rw-   0        0        0     4012 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/connectors/variants/sap_o2c.py
+-rw-rw-rw-   0        0        0     4243 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/connectors/variants/windows_events.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:23.938013 pm4py-2.7.9.4/pm4py/algo/decision_mining/
+-rw-rw-rw-   0        0        0      964 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/decision_mining/__init__.py
+-rw-rw-rw-   0        0        0    23509 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/decision_mining/algorithm.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:23.940046 pm4py-2.7.9.4/pm4py/algo/discovery/
+-rw-rw-rw-   0        0        0      945 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/discovery/__init__.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:23.940046 pm4py-2.7.9.4/pm4py/algo/discovery/alpha/
+-rw-rw-rw-   0        0        0      818 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/discovery/alpha/__init__.py
+-rw-rw-rw-   0        0        0     5066 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/discovery/alpha/algorithm.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:23.940046 pm4py-2.7.9.4/pm4py/algo/discovery/alpha/data_structures/
+-rw-rw-rw-   0        0        0      816 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/discovery/alpha/data_structures/__init__.py
+-rw-rw-rw-   0        0        0     2420 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/discovery/alpha/data_structures/alpha_classic_abstraction.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:23.940046 pm4py-2.7.9.4/pm4py/algo/discovery/alpha/utils/
+-rw-rw-rw-   0        0        0      790 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/discovery/alpha/utils/__init__.py
+-rw-rw-rw-   0        0        0     1622 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/discovery/alpha/utils/endpoints.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:23.955675 pm4py-2.7.9.4/pm4py/algo/discovery/alpha/variants/
+-rw-rw-rw-   0        0        0      797 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/discovery/alpha/variants/__init__.py
+-rw-rw-rw-   0        0        0    10830 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/discovery/alpha/variants/classic.py
+-rw-rw-rw-   0        0        0    22005 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/discovery/alpha/variants/plus.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:23.955675 pm4py-2.7.9.4/pm4py/algo/discovery/batches/
+-rw-rw-rw-   0        0        0      803 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/discovery/batches/__init__.py
+-rw-rw-rw-   0        0        0     3756 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/discovery/batches/algorithm.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:23.955675 pm4py-2.7.9.4/pm4py/algo/discovery/batches/utils/
+-rw-rw-rw-   0        0        0      792 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/discovery/batches/utils/__init__.py
+-rw-rw-rw-   0        0        0     9636 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/discovery/batches/utils/detection.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:23.971764 pm4py-2.7.9.4/pm4py/algo/discovery/batches/variants/
+-rw-rw-rw-   0        0        0      797 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/discovery/batches/variants/__init__.py
+-rw-rw-rw-   0        0        0     5216 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/discovery/batches/variants/log.py
+-rw-rw-rw-   0        0        0     6427 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/discovery/batches/variants/pandas.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:23.971764 pm4py-2.7.9.4/pm4py/algo/discovery/causal/
+-rw-rw-rw-   0        0        0      795 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/discovery/causal/__init__.py
+-rw-rw-rw-   0        0        0     1646 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/discovery/causal/algorithm.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:23.980770 pm4py-2.7.9.4/pm4py/algo/discovery/causal/variants/
+-rw-rw-rw-   0        0        0      801 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/discovery/causal/variants/__init__.py
+-rw-rw-rw-   0        0        0     1787 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/discovery/causal/variants/alpha.py
+-rw-rw-rw-   0        0        0     1589 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/discovery/causal/variants/heuristic.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:23.980770 pm4py-2.7.9.4/pm4py/algo/discovery/correlation_mining/
+-rw-rw-rw-   0        0        0      813 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/discovery/correlation_mining/__init__.py
+-rw-rw-rw-   0        0        0     2249 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/discovery/correlation_mining/algorithm.py
+-rw-rw-rw-   0        0        0     7934 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/discovery/correlation_mining/util.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:23.996395 pm4py-2.7.9.4/pm4py/algo/discovery/correlation_mining/variants/
+-rw-rw-rw-   0        0        0      832 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/discovery/correlation_mining/variants/__init__.py
+-rw-rw-rw-   0        0        0     9663 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/discovery/correlation_mining/variants/classic.py
+-rw-rw-rw-   0        0        0     4405 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/discovery/correlation_mining/variants/classic_split.py
+-rw-rw-rw-   0        0        0    10288 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/discovery/correlation_mining/variants/trace_based.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:23.996395 pm4py-2.7.9.4/pm4py/algo/discovery/declare/
+-rw-rw-rw-   0        0        0      798 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/discovery/declare/__init__.py
+-rw-rw-rw-   0        0        0     1725 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/discovery/declare/algorithm.py
+-rw-rw-rw-   0        0        0     1290 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/discovery/declare/templates.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:24.012017 pm4py-2.7.9.4/pm4py/algo/discovery/declare/variants/
+-rw-rw-rw-   0        0        0      795 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/discovery/declare/variants/__init__.py
+-rw-rw-rw-   0        0        0    30263 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/discovery/declare/variants/classic.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:24.012017 pm4py-2.7.9.4/pm4py/algo/discovery/dfg/
+-rw-rw-rw-   0        0        0      822 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/discovery/dfg/__init__.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:24.012017 pm4py-2.7.9.4/pm4py/algo/discovery/dfg/adapters/
+-rw-rw-rw-   0        0        0      788 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/discovery/dfg/adapters/__init__.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:24.027639 pm4py-2.7.9.4/pm4py/algo/discovery/dfg/adapters/pandas/
+-rw-rw-rw-   0        0        0      816 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/discovery/dfg/adapters/pandas/__init__.py
+-rw-rw-rw-   0        0        0    15047 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/discovery/dfg/adapters/pandas/df_statistics.py
+-rw-rw-rw-   0        0        0     2962 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/discovery/dfg/adapters/pandas/freq_triples.py
+-rw-rw-rw-   0        0        0     4898 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/discovery/dfg/algorithm.py
+-rw-rw-rw-   0        0        0     1260 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/discovery/dfg/replacement.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:24.027639 pm4py-2.7.9.4/pm4py/algo/discovery/dfg/utils/
+-rw-rw-rw-   0        0        0      788 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/discovery/dfg/utils/__init__.py
+-rw-rw-rw-   0        0        0      783 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/discovery/dfg/utils/dfg_utils.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:24.043259 pm4py-2.7.9.4/pm4py/algo/discovery/dfg/variants/
+-rw-rw-rw-   0        0        0      968 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/discovery/dfg/variants/__init__.py
+-rw-rw-rw-   0        0        0     4609 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/discovery/dfg/variants/case_attributes.py
+-rw-rw-rw-   0        0        0     2852 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/discovery/dfg/variants/clean.py
+-rw-rw-rw-   0        0        0     2795 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/discovery/dfg/variants/clean_polars.py
+-rw-rw-rw-   0        0        0     3347 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/discovery/dfg/variants/clean_time.py
+-rw-rw-rw-   0        0        0     2200 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/discovery/dfg/variants/freq_triples.py
+-rw-rw-rw-   0        0        0     2574 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/discovery/dfg/variants/native.py
+-rw-rw-rw-   0        0        0     5794 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/discovery/dfg/variants/performance.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:24.043259 pm4py-2.7.9.4/pm4py/algo/discovery/footprints/
+-rw-rw-rw-   0        0        0      812 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/discovery/footprints/__init__.py
+-rw-rw-rw-   0        0        0     3131 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/discovery/footprints/algorithm.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:24.058881 pm4py-2.7.9.4/pm4py/algo/discovery/footprints/dfg/
+-rw-rw-rw-   0        0        0      792 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/discovery/footprints/dfg/__init__.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:24.058881 pm4py-2.7.9.4/pm4py/algo/discovery/footprints/dfg/variants/
+-rw-rw-rw-   0        0        0      796 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/discovery/footprints/dfg/variants/__init__.py
+-rw-rw-rw-   0        0        0     2258 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/discovery/footprints/dfg/variants/dfg.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:24.058881 pm4py-2.7.9.4/pm4py/algo/discovery/footprints/log/
+-rw-rw-rw-   0        0        0      792 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/discovery/footprints/log/__init__.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:24.074503 pm4py-2.7.9.4/pm4py/algo/discovery/footprints/log/variants/
+-rw-rw-rw-   0        0        0      843 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/discovery/footprints/log/variants/__init__.py
+-rw-rw-rw-   0        0        0     4664 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/discovery/footprints/log/variants/entire_dataframe.py
+-rw-rw-rw-   0        0        0     3314 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/discovery/footprints/log/variants/entire_event_log.py
+-rw-rw-rw-   0        0        0     3195 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/discovery/footprints/log/variants/trace_by_trace.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:24.074503 pm4py-2.7.9.4/pm4py/algo/discovery/footprints/petri/
+-rw-rw-rw-   0        0        0      794 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/discovery/footprints/petri/__init__.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:24.081009 pm4py-2.7.9.4/pm4py/algo/discovery/footprints/petri/variants/
+-rw-rw-rw-   0        0        0      806 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/discovery/footprints/petri/variants/__init__.py
+-rw-rw-rw-   0        0        0     3629 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/discovery/footprints/petri/variants/reach_graph.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:24.081009 pm4py-2.7.9.4/pm4py/algo/discovery/footprints/tree/
+-rw-rw-rw-   0        0        0      793 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/discovery/footprints/tree/__init__.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:24.081009 pm4py-2.7.9.4/pm4py/algo/discovery/footprints/tree/variants/
+-rw-rw-rw-   0        0        0      802 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/discovery/footprints/tree/variants/__init__.py
+-rw-rw-rw-   0        0        0    13403 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/discovery/footprints/tree/variants/bottomup.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:24.081009 pm4py-2.7.9.4/pm4py/algo/discovery/heuristics/
+-rw-rw-rw-   0        0        0      799 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/discovery/heuristics/__init__.py
+-rw-rw-rw-   0        0        0     7484 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/discovery/heuristics/algorithm.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:24.096637 pm4py-2.7.9.4/pm4py/algo/discovery/heuristics/variants/
+-rw-rw-rw-   0        0        0      806 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/discovery/heuristics/variants/__init__.py
+-rw-rw-rw-   0        0        0    26145 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/discovery/heuristics/variants/classic.py
+-rw-rw-rw-   0        0        0    24355 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/discovery/heuristics/variants/plusplus.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:24.096637 pm4py-2.7.9.4/pm4py/algo/discovery/ilp/
+-rw-rw-rw-   0        0        0      792 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/discovery/ilp/__init__.py
+-rw-rw-rw-   0        0        0     1782 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/discovery/ilp/algorithm.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:24.112258 pm4py-2.7.9.4/pm4py/algo/discovery/ilp/variants/
+-rw-rw-rw-   0        0        0      789 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/discovery/ilp/variants/__init__.py
+-rw-rw-rw-   0        0        0    12873 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/discovery/ilp/variants/classic.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:24.112258 pm4py-2.7.9.4/pm4py/algo/discovery/inductive/
+-rw-rw-rw-   0        0        0      800 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/discovery/inductive/__init__.py
+-rw-rw-rw-   0        0        0     3602 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/discovery/inductive/algorithm.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:24.127879 pm4py-2.7.9.4/pm4py/algo/discovery/inductive/base_case/
+-rw-rw-rw-   0        0        0      829 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/discovery/inductive/base_case/__init__.py
+-rw-rw-rw-   0        0        0     1533 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/discovery/inductive/base_case/abc.py
+-rw-rw-rw-   0        0        0     1768 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/discovery/inductive/base_case/empty_log.py
+-rw-rw-rw-   0        0        0     2268 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/discovery/inductive/base_case/factory.py
+-rw-rw-rw-   0        0        0     2060 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/discovery/inductive/base_case/single_activity.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:24.143501 pm4py-2.7.9.4/pm4py/algo/discovery/inductive/cuts/
+-rw-rw-rw-   0        0        0      816 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/discovery/inductive/cuts/__init__.py
+-rw-rw-rw-   0        0        0     2100 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/discovery/inductive/cuts/abc.py
+-rw-rw-rw-   0        0        0     4570 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/discovery/inductive/cuts/concurrency.py
+-rw-rw-rw-   0        0        0     3143 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/discovery/inductive/cuts/factory.py
+-rw-rw-rw-   0        0        0    10916 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/discovery/inductive/cuts/loop.py
+-rw-rw-rw-   0        0        0    11571 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/discovery/inductive/cuts/sequence.py
+-rw-rw-rw-   0        0        0     1519 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/discovery/inductive/cuts/utils.py
+-rw-rw-rw-   0        0        0     4316 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/discovery/inductive/cuts/xor.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:24.159121 pm4py-2.7.9.4/pm4py/algo/discovery/inductive/dtypes/
+-rw-rw-rw-   0        0        0      797 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/discovery/inductive/dtypes/__init__.py
+-rw-rw-rw-   0        0        0     1050 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/discovery/inductive/dtypes/im_dfg.py
+-rw-rw-rw-   0        0        0     2568 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/discovery/inductive/dtypes/im_ds.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:24.181257 pm4py-2.7.9.4/pm4py/algo/discovery/inductive/fall_through/
+-rw-rw-rw-   0        0        0      897 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/discovery/inductive/fall_through/__init__.py
+-rw-rw-rw-   0        0        0     1385 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/discovery/inductive/fall_through/abc.py
+-rw-rw-rw-   0        0        0     4792 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/discovery/inductive/fall_through/activity_concurrent.py
+-rw-rw-rw-   0        0        0     1643 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/discovery/inductive/fall_through/activity_once_per_trace.py
+-rw-rw-rw-   0        0        0     2709 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/discovery/inductive/fall_through/empty_traces.py
+-rw-rw-rw-   0        0        0     3254 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/discovery/inductive/fall_through/factory.py
+-rw-rw-rw-   0        0        0     3059 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/discovery/inductive/fall_through/flower.py
+-rw-rw-rw-   0        0        0     2441 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/discovery/inductive/fall_through/strict_tau_loop.py
+-rw-rw-rw-   0        0        0     1520 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/discovery/inductive/fall_through/tau_loop.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:24.208812 pm4py-2.7.9.4/pm4py/algo/discovery/inductive/variants/
+-rw-rw-rw-   0        0        0      807 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/discovery/inductive/variants/__init__.py
+-rw-rw-rw-   0        0        0     4160 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/discovery/inductive/variants/abc.py
+-rw-rw-rw-   0        0        0     1740 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/discovery/inductive/variants/im.py
+-rw-rw-rw-   0        0        0     1098 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/discovery/inductive/variants/imd.py
+-rw-rw-rw-   0        0        0     4381 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/discovery/inductive/variants/imf.py
+-rw-rw-rw-   0        0        0      881 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/discovery/inductive/variants/instances.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:24.208812 pm4py-2.7.9.4/pm4py/algo/discovery/log_skeleton/
+-rw-rw-rw-   0        0        0      815 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/discovery/log_skeleton/__init__.py
+-rw-rw-rw-   0        0        0     2450 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/discovery/log_skeleton/algorithm.py
+-rw-rw-rw-   0        0        0     3194 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/discovery/log_skeleton/trace_skel.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:24.208812 pm4py-2.7.9.4/pm4py/algo/discovery/log_skeleton/variants/
+-rw-rw-rw-   0        0        0      798 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/discovery/log_skeleton/variants/__init__.py
+-rw-rw-rw-   0        0        0    11111 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/discovery/log_skeleton/variants/classic.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:24.224432 pm4py-2.7.9.4/pm4py/algo/discovery/minimum_self_distance/
+-rw-rw-rw-   0        0        0      819 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/discovery/minimum_self_distance/__init__.py
+-rw-rw-rw-   0        0        0     1567 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/discovery/minimum_self_distance/algorithm.py
+-rw-rw-rw-   0        0        0     3132 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/discovery/minimum_self_distance/utils.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:24.240054 pm4py-2.7.9.4/pm4py/algo/discovery/minimum_self_distance/variants/
+-rw-rw-rw-   0        0        0      811 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/discovery/minimum_self_distance/variants/__init__.py
+-rw-rw-rw-   0        0        0     2878 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/discovery/minimum_self_distance/variants/log.py
+-rw-rw-rw-   0        0        0     2904 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/discovery/minimum_self_distance/variants/pandas.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:24.240054 pm4py-2.7.9.4/pm4py/algo/discovery/ocel/
+-rw-rw-rw-   0        0        0      802 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/discovery/ocel/__init__.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:24.240054 pm4py-2.7.9.4/pm4py/algo/discovery/ocel/interleavings/
+-rw-rw-rw-   0        0        0      814 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/discovery/ocel/interleavings/__init__.py
+-rw-rw-rw-   0        0        0     2007 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/discovery/ocel/interleavings/algorithm.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:24.240054 pm4py-2.7.9.4/pm4py/algo/discovery/ocel/interleavings/utils/
+-rw-rw-rw-   0        0        0      819 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/discovery/ocel/interleavings/utils/__init__.py
+-rw-rw-rw-   0        0        0     4451 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/discovery/ocel/interleavings/utils/merge_dataframe_rel_cases.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:24.255675 pm4py-2.7.9.4/pm4py/algo/discovery/ocel/interleavings/variants/
+-rw-rw-rw-   0        0        0      820 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/discovery/ocel/interleavings/variants/__init__.py
+-rw-rw-rw-   0        0        0     6643 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/discovery/ocel/interleavings/variants/timestamp_interleavings.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:24.271297 pm4py-2.7.9.4/pm4py/algo/discovery/ocel/link_analysis/
+-rw-rw-rw-   0        0        0      796 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/discovery/ocel/link_analysis/__init__.py
+-rw-rw-rw-   0        0        0     1841 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/discovery/ocel/link_analysis/algorithm.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:24.271297 pm4py-2.7.9.4/pm4py/algo/discovery/ocel/link_analysis/variants/
+-rw-rw-rw-   0        0        0      804 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/discovery/ocel/link_analysis/variants/__init__.py
+-rw-rw-rw-   0        0        0     6519 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/discovery/ocel/link_analysis/variants/classic.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:24.281303 pm4py-2.7.9.4/pm4py/algo/discovery/ocel/ocdfg/
+-rw-rw-rw-   0        0        0      799 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/discovery/ocel/ocdfg/__init__.py
+-rw-rw-rw-   0        0        0     1775 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/discovery/ocel/ocdfg/algorithm.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:24.281303 pm4py-2.7.9.4/pm4py/algo/discovery/ocel/ocdfg/variants/
+-rw-rw-rw-   0        0        0      796 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/discovery/ocel/ocdfg/variants/__init__.py
+-rw-rw-rw-   0        0        0     8817 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/discovery/ocel/ocdfg/variants/classic.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:24.281303 pm4py-2.7.9.4/pm4py/algo/discovery/ocel/ocpn/
+-rw-rw-rw-   0        0        0      798 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/discovery/ocel/ocpn/__init__.py
+-rw-rw-rw-   0        0        0     1785 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/discovery/ocel/ocpn/algorithm.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:24.296930 pm4py-2.7.9.4/pm4py/algo/discovery/ocel/ocpn/variants/
+-rw-rw-rw-   0        0        0      797 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/discovery/ocel/ocpn/variants/__init__.py
+-rw-rw-rw-   0        0        0    10290 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/discovery/ocel/ocpn/variants/classic.py
+-rw-rw-rw-   0        0        0      812 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/discovery/ocel/ocpn/variants/wo_annotation.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:24.304238 pm4py-2.7.9.4/pm4py/algo/discovery/ocel/saw_nets/
+-rw-rw-rw-   0        0        0      804 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/discovery/ocel/saw_nets/__init__.py
+-rw-rw-rw-   0        0        0     1800 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/discovery/ocel/saw_nets/algorithm.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:24.306265 pm4py-2.7.9.4/pm4py/algo/discovery/ocel/saw_nets/variants/
+-rw-rw-rw-   0        0        0      801 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/discovery/ocel/saw_nets/variants/__init__.py
+-rw-rw-rw-   0        0        0     7569 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/discovery/ocel/saw_nets/variants/classic.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:24.306265 pm4py-2.7.9.4/pm4py/algo/discovery/performance_spectrum/
+-rw-rw-rw-   0        0        0      809 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/discovery/performance_spectrum/__init__.py
+-rw-rw-rw-   0        0        0     3495 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/discovery/performance_spectrum/algorithm.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:24.321892 pm4py-2.7.9.4/pm4py/algo/discovery/performance_spectrum/variants/
+-rw-rw-rw-   0        0        0      855 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/discovery/performance_spectrum/variants/__init__.py
+-rw-rw-rw-   0        0        0     4317 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/discovery/performance_spectrum/variants/dataframe.py
+-rw-rw-rw-   0        0        0     4970 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/discovery/performance_spectrum/variants/dataframe_disconnected.py
+-rw-rw-rw-   0        0        0     3382 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/discovery/performance_spectrum/variants/log.py
+-rw-rw-rw-   0        0        0     4366 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/discovery/performance_spectrum/variants/log_disconnected.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:24.321892 pm4py-2.7.9.4/pm4py/algo/discovery/powl/
+-rw-rw-rw-   0        0        0      779 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/discovery/powl/__init__.py
+-rw-rw-rw-   0        0        0     3201 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/discovery/powl/algorithm.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:24.321892 pm4py-2.7.9.4/pm4py/algo/discovery/powl/inductive/
+-rw-rw-rw-   0        0        0      787 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/discovery/powl/inductive/__init__.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:24.337513 pm4py-2.7.9.4/pm4py/algo/discovery/powl/inductive/base_case/
+-rw-rw-rw-   0        0        0      797 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/discovery/powl/inductive/base_case/__init__.py
+-rw-rw-rw-   0        0        0     1506 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/discovery/powl/inductive/base_case/abc.py
+-rw-rw-rw-   0        0        0     1457 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/discovery/powl/inductive/base_case/empty_log.py
+-rw-rw-rw-   0        0        0     1867 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/discovery/powl/inductive/base_case/factory.py
+-rw-rw-rw-   0        0        0     1547 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/discovery/powl/inductive/base_case/single_activity.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:24.353134 pm4py-2.7.9.4/pm4py/algo/discovery/powl/inductive/cuts/
+-rw-rw-rw-   0        0        0      792 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/discovery/powl/inductive/cuts/__init__.py
+-rw-rw-rw-   0        0        0     1361 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/discovery/powl/inductive/cuts/concurrency.py
+-rw-rw-rw-   0        0        0     1974 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/discovery/powl/inductive/cuts/factory.py
+-rw-rw-rw-   0        0        0     1353 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/discovery/powl/inductive/cuts/loop.py
+-rw-rw-rw-   0        0        0     1975 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/discovery/powl/inductive/cuts/sequence.py
+-rw-rw-rw-   0        0        0     1433 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/discovery/powl/inductive/cuts/xor.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:24.368755 pm4py-2.7.9.4/pm4py/algo/discovery/powl/inductive/fall_through/
+-rw-rw-rw-   0        0        0      798 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/discovery/powl/inductive/fall_through/__init__.py
+-rw-rw-rw-   0        0        0     1905 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/discovery/powl/inductive/fall_through/activity_concurrent.py
+-rw-rw-rw-   0        0        0     1056 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/discovery/powl/inductive/fall_through/activity_once_per_trace.py
+-rw-rw-rw-   0        0        0     1795 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/discovery/powl/inductive/fall_through/empty_traces.py
+-rw-rw-rw-   0        0        0     2498 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/discovery/powl/inductive/fall_through/factory.py
+-rw-rw-rw-   0        0        0     1814 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/discovery/powl/inductive/fall_through/flower.py
+-rw-rw-rw-   0        0        0     1651 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/discovery/powl/inductive/fall_through/strict_tau_loop.py
+-rw-rw-rw-   0        0        0     1630 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/discovery/powl/inductive/fall_through/tau_loop.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:24.381261 pm4py-2.7.9.4/pm4py/algo/discovery/powl/inductive/utils/
+-rw-rw-rw-   0        0        0      734 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/discovery/powl/inductive/utils/__init__.py
+-rw-rw-rw-   0        0        0     2008 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/discovery/powl/inductive/utils/filtering.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:24.396889 pm4py-2.7.9.4/pm4py/algo/discovery/powl/inductive/variants/
+-rw-rw-rw-   0        0        0      798 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/discovery/powl/inductive/variants/__init__.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:24.412510 pm4py-2.7.9.4/pm4py/algo/discovery/powl/inductive/variants/brute_force/
+-rw-rw-rw-   0        0        0      806 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/discovery/powl/inductive/variants/brute_force/__init__.py
+-rw-rw-rw-   0        0        0     7020 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/discovery/powl/inductive/variants/brute_force/bf_partial_order_cut.py
+-rw-rw-rw-   0        0        0     2195 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/discovery/powl/inductive/variants/brute_force/factory.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:24.412510 pm4py-2.7.9.4/pm4py/algo/discovery/powl/inductive/variants/dynamic_clustering/
+-rw-rw-rw-   0        0        0      813 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/discovery/powl/inductive/variants/dynamic_clustering/__init__.py
+-rw-rw-rw-   0        0        0     7347 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/discovery/powl/inductive/variants/dynamic_clustering/dynamic_clustering_partial_order_cut.py
+-rw-rw-rw-   0        0        0     2043 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/discovery/powl/inductive/variants/dynamic_clustering/factory.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:24.428131 pm4py-2.7.9.4/pm4py/algo/discovery/powl/inductive/variants/dynamic_clustering_frequency/
+-rw-rw-rw-   0        0        0      823 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/discovery/powl/inductive/variants/dynamic_clustering_frequency/__init__.py
+-rw-rw-rw-   0        0        0     8397 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/discovery/powl/inductive/variants/dynamic_clustering_frequency/dynamic_clustering_frequency_partial_order_cut.py
+-rw-rw-rw-   0        0        0     2099 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/discovery/powl/inductive/variants/dynamic_clustering_frequency/factory.py
+-rw-rw-rw-   0        0        0     1482 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/discovery/powl/inductive/variants/im_brute_force.py
+-rw-rw-rw-   0        0        0     1643 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/discovery/powl/inductive/variants/im_dynamic_clustering.py
+-rw-rw-rw-   0        0        0     1687 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/discovery/powl/inductive/variants/im_dynamic_clustering_frequencies.py
+-rw-rw-rw-   0        0        0     1468 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/discovery/powl/inductive/variants/im_maximal.py
+-rw-rw-rw-   0        0        0     5456 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/discovery/powl/inductive/variants/im_tree.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:24.439826 pm4py-2.7.9.4/pm4py/algo/discovery/powl/inductive/variants/maximal/
+-rw-rw-rw-   0        0        0      800 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/discovery/powl/inductive/variants/maximal/__init__.py
+-rw-rw-rw-   0        0        0     2373 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/discovery/powl/inductive/variants/maximal/factory.py
+-rw-rw-rw-   0        0        0     7192 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/discovery/powl/inductive/variants/maximal/maximal_partial_order_cut.py
+-rw-rw-rw-   0        0        0      936 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/discovery/powl/inductive/variants/powl_discovery_varaints.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:24.439826 pm4py-2.7.9.4/pm4py/algo/discovery/temporal_profile/
+-rw-rw-rw-   0        0        0      805 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/discovery/temporal_profile/__init__.py
+-rw-rw-rw-   0        0        0     2006 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/discovery/temporal_profile/algorithm.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:24.439826 pm4py-2.7.9.4/pm4py/algo/discovery/temporal_profile/variants/
+-rw-rw-rw-   0        0        0      809 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/discovery/temporal_profile/variants/__init__.py
+-rw-rw-rw-   0        0        0     4044 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/discovery/temporal_profile/variants/dataframe.py
+-rw-rw-rw-   0        0        0     5236 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/discovery/temporal_profile/variants/log.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:24.455453 pm4py-2.7.9.4/pm4py/algo/discovery/transition_system/
+-rw-rw-rw-   0        0        0      806 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/discovery/transition_system/__init__.py
+-rw-rw-rw-   0        0        0     1984 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/discovery/transition_system/algorithm.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:24.455453 pm4py-2.7.9.4/pm4py/algo/discovery/transition_system/variants/
+-rw-rw-rw-   0        0        0      806 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/discovery/transition_system/variants/__init__.py
+-rw-rw-rw-   0        0        0     5956 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/discovery/transition_system/variants/view_based.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:24.473020 pm4py-2.7.9.4/pm4py/algo/evaluation/
+-rw-rw-rw-   0        0        0      836 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/evaluation/__init__.py
+-rw-rw-rw-   0        0        0     4819 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/evaluation/algorithm.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:24.473020 pm4py-2.7.9.4/pm4py/algo/evaluation/earth_mover_distance/
+-rw-rw-rw-   0        0        0      995 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/evaluation/earth_mover_distance/__init__.py
+-rw-rw-rw-   0        0        0     1678 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/evaluation/earth_mover_distance/algorithm.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:24.481547 pm4py-2.7.9.4/pm4py/algo/evaluation/earth_mover_distance/variants/
+-rw-rw-rw-   0        0        0      805 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/evaluation/earth_mover_distance/variants/__init__.py
+-rw-rw-rw-   0        0        0     4864 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/evaluation/earth_mover_distance/variants/pyemd.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:24.483575 pm4py-2.7.9.4/pm4py/algo/evaluation/generalization/
+-rw-rw-rw-   0        0        0      804 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/evaluation/generalization/__init__.py
+-rw-rw-rw-   0        0        0     1703 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/evaluation/generalization/algorithm.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:24.493638 pm4py-2.7.9.4/pm4py/algo/evaluation/generalization/variants/
+-rw-rw-rw-   0        0        0      805 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/evaluation/generalization/variants/__init__.py
+-rw-rw-rw-   0        0        0     2285 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/evaluation/generalization/variants/token_based.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:24.501661 pm4py-2.7.9.4/pm4py/algo/evaluation/precision/
+-rw-rw-rw-   0        0        0      811 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/evaluation/precision/__init__.py
+-rw-rw-rw-   0        0        0     2994 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/evaluation/precision/algorithm.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:24.501661 pm4py-2.7.9.4/pm4py/algo/evaluation/precision/dfg/
+-rw-rw-rw-   0        0        0      793 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/evaluation/precision/dfg/__init__.py
+-rw-rw-rw-   0        0        0     3992 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/evaluation/precision/dfg/algorithm.py
+-rw-rw-rw-   0        0        0     5525 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/evaluation/precision/utils.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:24.513731 pm4py-2.7.9.4/pm4py/algo/evaluation/precision/variants/
+-rw-rw-rw-   0        0        0      829 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/evaluation/precision/variants/__init__.py
+-rw-rw-rw-   0        0        0    13806 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/evaluation/precision/variants/align_etconformance.py
+-rw-rw-rw-   0        0        0     6199 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/evaluation/precision/variants/etconformance_token.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:24.521759 pm4py-2.7.9.4/pm4py/algo/evaluation/replay_fitness/
+-rw-rw-rw-   0        0        0      804 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/evaluation/replay_fitness/__init__.py
+-rw-rw-rw-   0        0        0     4486 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/evaluation/replay_fitness/algorithm.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:24.523777 pm4py-2.7.9.4/pm4py/algo/evaluation/replay_fitness/variants/
+-rw-rw-rw-   0        0        0      823 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/evaluation/replay_fitness/variants/__init__.py
+-rw-rw-rw-   0        0        0     6788 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/evaluation/replay_fitness/variants/alignment_based.py
+-rw-rw-rw-   0        0        0     5159 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/evaluation/replay_fitness/variants/token_replay.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:24.533844 pm4py-2.7.9.4/pm4py/algo/evaluation/simplicity/
+-rw-rw-rw-   0        0        0      802 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/evaluation/simplicity/__init__.py
+-rw-rw-rw-   0        0        0     1585 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/evaluation/simplicity/algorithm.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:24.541860 pm4py-2.7.9.4/pm4py/algo/evaluation/simplicity/variants/
+-rw-rw-rw-   0        0        0      841 2024-01-17 08:27:47.000000 pm4py-2.7.9.4/pm4py/algo/evaluation/simplicity/variants/__init__.py
+-rw-rw-rw-   0        0        0     2696 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/algo/evaluation/simplicity/variants/arc_degree.py
+-rw-rw-rw-   0        0        0     1602 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/algo/evaluation/simplicity/variants/extended_cardoso.py
+-rw-rw-rw-   0        0        0     2120 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/algo/evaluation/simplicity/variants/extended_cyclomatic.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:24.541860 pm4py-2.7.9.4/pm4py/algo/filtering/
+-rw-rw-rw-   0        0        0      734 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/algo/filtering/__init__.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:24.541860 pm4py-2.7.9.4/pm4py/algo/filtering/common/
+-rw-rw-rw-   0        0        0      852 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/algo/filtering/common/__init__.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:24.551865 pm4py-2.7.9.4/pm4py/algo/filtering/common/attributes/
+-rw-rw-rw-   0        0        0      734 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/algo/filtering/common/attributes/__init__.py
+-rw-rw-rw-   0        0        0      951 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/algo/filtering/common/attributes/attributes_common.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:24.551865 pm4py-2.7.9.4/pm4py/algo/filtering/common/end_activities/
+-rw-rw-rw-   0        0        0      812 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/algo/filtering/common/end_activities/__init__.py
+-rw-rw-rw-   0        0        0      851 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/algo/filtering/common/end_activities/end_activities_common.py
+-rw-rw-rw-   0        0        0      845 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/algo/filtering/common/filtering_constants.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:24.551865 pm4py-2.7.9.4/pm4py/algo/filtering/common/start_activities/
+-rw-rw-rw-   0        0        0      816 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/algo/filtering/common/start_activities/__init__.py
+-rw-rw-rw-   0        0        0      857 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/algo/filtering/common/start_activities/start_activities_common.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:24.567490 pm4py-2.7.9.4/pm4py/algo/filtering/common/timestamp/
+-rw-rw-rw-   0        0        0      734 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/algo/filtering/common/timestamp/__init__.py
+-rw-rw-rw-   0        0        0     1250 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/algo/filtering/common/timestamp/timestamp_common.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:24.567490 pm4py-2.7.9.4/pm4py/algo/filtering/common/traces/
+-rw-rw-rw-   0        0        0      734 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/algo/filtering/common/traces/__init__.py
+-rw-rw-rw-   0        0        0     1246 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/algo/filtering/common/traces/infix_to_regex.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:24.567490 pm4py-2.7.9.4/pm4py/algo/filtering/dfg/
+-rw-rw-rw-   0        0        0      734 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/algo/filtering/dfg/__init__.py
+-rw-rw-rw-   0        0        0    25920 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/algo/filtering/dfg/dfg_filtering.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:24.567490 pm4py-2.7.9.4/pm4py/algo/filtering/log/
+-rw-rw-rw-   0        0        0      866 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/algo/filtering/log/__init__.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:24.567490 pm4py-2.7.9.4/pm4py/algo/filtering/log/attr_value_repetition/
+-rw-rw-rw-   0        0        0      994 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/algo/filtering/log/attr_value_repetition/__init__.py
+-rw-rw-rw-   0        0        0     2754 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/algo/filtering/log/attr_value_repetition/filter.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:24.583112 pm4py-2.7.9.4/pm4py/algo/filtering/log/attributes/
+-rw-rw-rw-   0        0        0      801 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/algo/filtering/log/attributes/__init__.py
+-rw-rw-rw-   0        0        0    18308 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/algo/filtering/log/attributes/attributes_filter.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:24.583112 pm4py-2.7.9.4/pm4py/algo/filtering/log/between/
+-rw-rw-rw-   0        0        0      795 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/algo/filtering/log/between/__init__.py
+-rw-rw-rw-   0        0        0     2944 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/algo/filtering/log/between/between_filter.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:24.583112 pm4py-2.7.9.4/pm4py/algo/filtering/log/cases/
+-rw-rw-rw-   0        0        0      790 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/algo/filtering/log/cases/__init__.py
+-rw-rw-rw-   0        0        0     4597 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/algo/filtering/log/cases/case_filter.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:24.583112 pm4py-2.7.9.4/pm4py/algo/filtering/log/end_activities/
+-rw-rw-rw-   0        0        0      809 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/algo/filtering/log/end_activities/__init__.py
+-rw-rw-rw-   0        0        0     3719 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/algo/filtering/log/end_activities/end_activities_filter.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:24.598733 pm4py-2.7.9.4/pm4py/algo/filtering/log/ltl/
+-rw-rw-rw-   0        0        0      788 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/algo/filtering/log/ltl/__init__.py
+-rw-rw-rw-   0        0        0    11094 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/algo/filtering/log/ltl/ltl_checker.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:24.598733 pm4py-2.7.9.4/pm4py/algo/filtering/log/paths/
+-rw-rw-rw-   0        0        0      791 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/algo/filtering/log/paths/__init__.py
+-rw-rw-rw-   0        0        0     9660 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/algo/filtering/log/paths/paths_filter.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:24.598733 pm4py-2.7.9.4/pm4py/algo/filtering/log/prefixes/
+-rw-rw-rw-   0        0        0      797 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/algo/filtering/log/prefixes/__init__.py
+-rw-rw-rw-   0        0        0     3218 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/algo/filtering/log/prefixes/prefix_filter.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:24.598733 pm4py-2.7.9.4/pm4py/algo/filtering/log/rework/
+-rw-rw-rw-   0        0        0      793 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/algo/filtering/log/rework/__init__.py
+-rw-rw-rw-   0        0        0     3412 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/algo/filtering/log/rework/rework_filter.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:24.614355 pm4py-2.7.9.4/pm4py/algo/filtering/log/start_activities/
+-rw-rw-rw-   0        0        0      813 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/algo/filtering/log/start_activities/__init__.py
+-rw-rw-rw-   0        0        0     3950 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/algo/filtering/log/start_activities/start_activities_filter.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:24.614355 pm4py-2.7.9.4/pm4py/algo/filtering/log/suffixes/
+-rw-rw-rw-   0        0        0      797 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/algo/filtering/log/suffixes/__init__.py
+-rw-rw-rw-   0        0        0     3223 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/algo/filtering/log/suffixes/suffix_filter.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:24.614355 pm4py-2.7.9.4/pm4py/algo/filtering/log/timestamp/
+-rw-rw-rw-   0        0        0      799 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/algo/filtering/log/timestamp/__init__.py
+-rw-rw-rw-   0        0        0    11509 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/algo/filtering/log/timestamp/timestamp_filter.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:24.614355 pm4py-2.7.9.4/pm4py/algo/filtering/log/traces/
+-rw-rw-rw-   0        0        0      734 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/algo/filtering/log/traces/__init__.py
+-rw-rw-rw-   0        0        0     3785 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/algo/filtering/log/traces/trace_filter.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:24.629976 pm4py-2.7.9.4/pm4py/algo/filtering/log/variants/
+-rw-rw-rw-   0        0        0      797 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/algo/filtering/log/variants/__init__.py
+-rw-rw-rw-   0        0        0     9002 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/algo/filtering/log/variants/variants_filter.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:24.629976 pm4py-2.7.9.4/pm4py/algo/filtering/ocel/
+-rw-rw-rw-   0        0        0      865 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/algo/filtering/ocel/__init__.py
+-rw-rw-rw-   0        0        0     3392 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/algo/filtering/ocel/activity_type_matching.py
+-rw-rw-rw-   0        0        0     3843 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/algo/filtering/ocel/event_attributes.py
+-rw-rw-rw-   0        0        0     2319 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/algo/filtering/ocel/object_attributes.py
+-rw-rw-rw-   0        0        0     3436 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/algo/filtering/ocel/objects_ot_count.py
+-rw-rw-rw-   0        0        0     4195 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/algo/filtering/ocel/ot_endpoints.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:24.645599 pm4py-2.7.9.4/pm4py/algo/filtering/pandas/
+-rw-rw-rw-   0        0        0      891 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/algo/filtering/pandas/__init__.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:24.652104 pm4py-2.7.9.4/pm4py/algo/filtering/pandas/attr_value_repetition/
+-rw-rw-rw-   0        0        0      997 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/algo/filtering/pandas/attr_value_repetition/__init__.py
+-rw-rw-rw-   0        0        0     2786 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/algo/filtering/pandas/attr_value_repetition/filter.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:24.652104 pm4py-2.7.9.4/pm4py/algo/filtering/pandas/attributes/
+-rw-rw-rw-   0        0        0      734 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/algo/filtering/pandas/attributes/__init__.py
+-rw-rw-rw-   0        0        0    13156 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/algo/filtering/pandas/attributes/attributes_filter.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:24.652104 pm4py-2.7.9.4/pm4py/algo/filtering/pandas/between/
+-rw-rw-rw-   0        0        0      798 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/algo/filtering/pandas/between/__init__.py
+-rw-rw-rw-   0        0        0     3266 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/algo/filtering/pandas/between/between_filter.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:24.652104 pm4py-2.7.9.4/pm4py/algo/filtering/pandas/cases/
+-rw-rw-rw-   0        0        0      793 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/algo/filtering/pandas/cases/__init__.py
+-rw-rw-rw-   0        0        0     6322 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/algo/filtering/pandas/cases/case_filter.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:24.667730 pm4py-2.7.9.4/pm4py/algo/filtering/pandas/consecutive_act_case_grouping/
+-rw-rw-rw-   0        0        0      842 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/algo/filtering/pandas/consecutive_act_case_grouping/__init__.py
+-rw-rw-rw-   0        0        0     3077 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/algo/filtering/pandas/consecutive_act_case_grouping/consecutive_act_case_grouping_filter.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:24.667730 pm4py-2.7.9.4/pm4py/algo/filtering/pandas/end_activities/
+-rw-rw-rw-   0        0        0      812 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/algo/filtering/pandas/end_activities/__init__.py
+-rw-rw-rw-   0        0        0     6142 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/algo/filtering/pandas/end_activities/end_activities_filter.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:24.667730 pm4py-2.7.9.4/pm4py/algo/filtering/pandas/ends_with/
+-rw-rw-rw-   0        0        0      734 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/algo/filtering/pandas/ends_with/__init__.py
+-rw-rw-rw-   0        0        0     3508 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/algo/filtering/pandas/ends_with/ends_with_filter.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:24.683353 pm4py-2.7.9.4/pm4py/algo/filtering/pandas/ltl/
+-rw-rw-rw-   0        0        0      791 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/algo/filtering/pandas/ltl/__init__.py
+-rw-rw-rw-   0        0        0    11763 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/algo/filtering/pandas/ltl/ltl_checker.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:24.683353 pm4py-2.7.9.4/pm4py/algo/filtering/pandas/paths/
+-rw-rw-rw-   0        0        0      794 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/algo/filtering/pandas/paths/__init__.py
+-rw-rw-rw-   0        0        0     6919 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/algo/filtering/pandas/paths/paths_filter.py
+-rw-rw-rw-   0        0        0      832 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/algo/filtering/pandas/pd_filtering_constants.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:24.683353 pm4py-2.7.9.4/pm4py/algo/filtering/pandas/prefixes/
+-rw-rw-rw-   0        0        0      800 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/algo/filtering/pandas/prefixes/__init__.py
+-rw-rw-rw-   0        0        0     3950 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/algo/filtering/pandas/prefixes/prefix_filter.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:24.698973 pm4py-2.7.9.4/pm4py/algo/filtering/pandas/rework/
+-rw-rw-rw-   0        0        0      796 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/algo/filtering/pandas/rework/__init__.py
+-rw-rw-rw-   0        0        0     3425 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/algo/filtering/pandas/rework/rework_filter.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:24.698973 pm4py-2.7.9.4/pm4py/algo/filtering/pandas/start_activities/
+-rw-rw-rw-   0        0        0      816 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/algo/filtering/pandas/start_activities/__init__.py
+-rw-rw-rw-   0        0        0     5585 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/algo/filtering/pandas/start_activities/start_activities_filter.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:24.698973 pm4py-2.7.9.4/pm4py/algo/filtering/pandas/starts_with/
+-rw-rw-rw-   0        0        0      734 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/algo/filtering/pandas/starts_with/__init__.py
+-rw-rw-rw-   0        0        0     3510 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/algo/filtering/pandas/starts_with/starts_with_filter.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:24.714600 pm4py-2.7.9.4/pm4py/algo/filtering/pandas/suffixes/
+-rw-rw-rw-   0        0        0      736 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/algo/filtering/pandas/suffixes/__init__.py
+-rw-rw-rw-   0        0        0     3950 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/algo/filtering/pandas/suffixes/suffix_filter.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:24.714600 pm4py-2.7.9.4/pm4py/algo/filtering/pandas/timestamp/
+-rw-rw-rw-   0        0        0      802 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/algo/filtering/pandas/timestamp/__init__.py
+-rw-rw-rw-   0        0        0     8208 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/algo/filtering/pandas/timestamp/timestamp_filter.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:24.714600 pm4py-2.7.9.4/pm4py/algo/filtering/pandas/timestamp_case_grouping/
+-rw-rw-rw-   0        0        0      830 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/algo/filtering/pandas/timestamp_case_grouping/__init__.py
+-rw-rw-rw-   0        0        0     3499 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/algo/filtering/pandas/timestamp_case_grouping/timestamp_case_grouping_filter.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:24.732339 pm4py-2.7.9.4/pm4py/algo/filtering/pandas/traces/
+-rw-rw-rw-   0        0        0      736 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/algo/filtering/pandas/traces/__init__.py
+-rw-rw-rw-   0        0        0     3604 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/algo/filtering/pandas/traces/trace_filter.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:24.732339 pm4py-2.7.9.4/pm4py/algo/filtering/pandas/variants/
+-rw-rw-rw-   0        0        0      734 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/algo/filtering/pandas/variants/__init__.py
+-rw-rw-rw-   0        0        0     6083 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/algo/filtering/pandas/variants/variants_filter.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:24.732339 pm4py-2.7.9.4/pm4py/algo/label_splitting/
+-rw-rw-rw-   0        0        0      794 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/algo/label_splitting/__init__.py
+-rw-rw-rw-   0        0        0     1921 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/algo/label_splitting/algorithm.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:24.747963 pm4py-2.7.9.4/pm4py/algo/label_splitting/variants/
+-rw-rw-rw-   0        0        0      794 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/algo/label_splitting/variants/__init__.py
+-rw-rw-rw-   0        0        0     9446 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/algo/label_splitting/variants/contextual.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:24.747963 pm4py-2.7.9.4/pm4py/algo/merging/
+-rw-rw-rw-   0        0        0      781 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/algo/merging/__init__.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:24.751969 pm4py-2.7.9.4/pm4py/algo/merging/case_relations/
+-rw-rw-rw-   0        0        0      801 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/algo/merging/case_relations/__init__.py
+-rw-rw-rw-   0        0        0     2326 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/algo/merging/case_relations/algorithm.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:24.751969 pm4py-2.7.9.4/pm4py/algo/merging/case_relations/variants/
+-rw-rw-rw-   0        0        0      797 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/algo/merging/case_relations/variants/__init__.py
+-rw-rw-rw-   0        0        0     3498 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/algo/merging/case_relations/variants/pandas.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:24.751969 pm4py-2.7.9.4/pm4py/algo/organizational_mining/
+-rw-rw-rw-   0        0        0      855 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/algo/organizational_mining/__init__.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:24.767596 pm4py-2.7.9.4/pm4py/algo/organizational_mining/local_diagnostics/
+-rw-rw-rw-   0        0        0      808 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/algo/organizational_mining/local_diagnostics/__init__.py
+-rw-rw-rw-   0        0        0    12440 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/algo/organizational_mining/local_diagnostics/algorithm.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:24.767596 pm4py-2.7.9.4/pm4py/algo/organizational_mining/network_analysis/
+-rw-rw-rw-   0        0        0      817 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/algo/organizational_mining/network_analysis/__init__.py
+-rw-rw-rw-   0        0        0     1840 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/algo/organizational_mining/network_analysis/algorithm.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:24.783218 pm4py-2.7.9.4/pm4py/algo/organizational_mining/network_analysis/variants/
+-rw-rw-rw-   0        0        0      816 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/algo/organizational_mining/network_analysis/variants/__init__.py
+-rw-rw-rw-   0        0        0    10562 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/algo/organizational_mining/network_analysis/variants/dataframe.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:24.783218 pm4py-2.7.9.4/pm4py/algo/organizational_mining/resource_profiles/
+-rw-rw-rw-   0        0        0      818 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/algo/organizational_mining/resource_profiles/__init__.py
+-rw-rw-rw-   0        0        0    12251 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/algo/organizational_mining/resource_profiles/algorithm.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:24.783218 pm4py-2.7.9.4/pm4py/algo/organizational_mining/resource_profiles/variants/
+-rw-rw-rw-   0        0        0      819 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/algo/organizational_mining/resource_profiles/variants/__init__.py
+-rw-rw-rw-   0        0        0    23271 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/algo/organizational_mining/resource_profiles/variants/log.py
+-rw-rw-rw-   0        0        0    23967 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/algo/organizational_mining/resource_profiles/variants/pandas.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:24.798839 pm4py-2.7.9.4/pm4py/algo/organizational_mining/roles/
+-rw-rw-rw-   0        0        0      814 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/algo/organizational_mining/roles/__init__.py
+-rw-rw-rw-   0        0        0     2427 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/algo/organizational_mining/roles/algorithm.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:24.798839 pm4py-2.7.9.4/pm4py/algo/organizational_mining/roles/common/
+-rw-rw-rw-   0        0        0      803 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/algo/organizational_mining/roles/common/__init__.py
+-rw-rw-rw-   0        0        0     8411 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/algo/organizational_mining/roles/common/algorithm.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:24.814460 pm4py-2.7.9.4/pm4py/algo/organizational_mining/roles/variants/
+-rw-rw-rw-   0        0        0      807 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/algo/organizational_mining/roles/variants/__init__.py
+-rw-rw-rw-   0        0        0     2448 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/algo/organizational_mining/roles/variants/log.py
+-rw-rw-rw-   0        0        0     2213 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/algo/organizational_mining/roles/variants/pandas.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:24.814460 pm4py-2.7.9.4/pm4py/algo/organizational_mining/sna/
+-rw-rw-rw-   0        0        0      810 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/algo/organizational_mining/sna/__init__.py
+-rw-rw-rw-   0        0        0     3689 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/algo/organizational_mining/sna/algorithm.py
+-rw-rw-rw-   0        0        0     3199 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/algo/organizational_mining/sna/util.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:24.814460 pm4py-2.7.9.4/pm4py/algo/organizational_mining/sna/variants/
+-rw-rw-rw-   0        0        0      805 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/algo/organizational_mining/sna/variants/__init__.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:24.830083 pm4py-2.7.9.4/pm4py/algo/organizational_mining/sna/variants/log/
+-rw-rw-rw-   0        0        0      857 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/algo/organizational_mining/sna/variants/log/__init__.py
+-rw-rw-rw-   0        0        0     3735 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/algo/organizational_mining/sna/variants/log/handover.py
+-rw-rw-rw-   0        0        0     3286 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/algo/organizational_mining/sna/variants/log/jointactivities.py
+-rw-rw-rw-   0        0        0     3525 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/algo/organizational_mining/sna/variants/log/subcontracting.py
+-rw-rw-rw-   0        0        0     3155 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/algo/organizational_mining/sna/variants/log/working_together.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:24.852211 pm4py-2.7.9.4/pm4py/algo/organizational_mining/sna/variants/pandas/
+-rw-rw-rw-   0        0        0      860 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/algo/organizational_mining/sna/variants/pandas/__init__.py
+-rw-rw-rw-   0        0        0     4235 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/algo/organizational_mining/sna/variants/pandas/handover.py
+-rw-rw-rw-   0        0        0     2998 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/algo/organizational_mining/sna/variants/pandas/jointactivities.py
+-rw-rw-rw-   0        0        0     3804 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/algo/organizational_mining/sna/variants/pandas/subcontracting.py
+-rw-rw-rw-   0        0        0     3432 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/algo/organizational_mining/sna/variants/pandas/working_together.py
+-rw-rw-rw-   0        0        0     7667 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/algo/organizational_mining/util.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:24.852211 pm4py-2.7.9.4/pm4py/algo/querying/
+-rw-rw-rw-   0        0        0      736 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/algo/querying/__init__.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:24.852211 pm4py-2.7.9.4/pm4py/algo/querying/llm/
+-rw-rw-rw-   0        0        0      798 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/algo/querying/llm/__init__.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:24.886548 pm4py-2.7.9.4/pm4py/algo/querying/llm/abstractions/
+-rw-rw-rw-   0        0        0      960 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/algo/querying/llm/abstractions/__init__.py
+-rw-rw-rw-   0        0        0     4006 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/algo/querying/llm/abstractions/case_to_descr.py
+-rw-rw-rw-   0        0        0     4382 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/algo/querying/llm/abstractions/declare_to_descr.py
+-rw-rw-rw-   0        0        0     3100 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/algo/querying/llm/abstractions/log_to_cols_descr.py
+-rw-rw-rw-   0        0        0     9696 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/algo/querying/llm/abstractions/log_to_dfg_descr.py
+-rw-rw-rw-   0        0        0     7886 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/algo/querying/llm/abstractions/log_to_fea_descr.py
+-rw-rw-rw-   0        0        0    10693 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/algo/querying/llm/abstractions/log_to_variants_descr.py
+-rw-rw-rw-   0        0        0     3241 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/algo/querying/llm/abstractions/logske_to_descr.py
+-rw-rw-rw-   0        0        0     1931 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/algo/querying/llm/abstractions/net_to_descr.py
+-rw-rw-rw-   0        0        0     6145 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/algo/querying/llm/abstractions/ocel_fea_descr.py
+-rw-rw-rw-   0        0        0     3680 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/algo/querying/llm/abstractions/ocel_ocdfg_descr.py
+-rw-rw-rw-   0        0        0     3004 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/algo/querying/llm/abstractions/stream_to_descr.py
+-rw-rw-rw-   0        0        0     2481 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/algo/querying/llm/abstractions/tempprofile_to_descr.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:24.886548 pm4py-2.7.9.4/pm4py/algo/querying/llm/connectors/
+-rw-rw-rw-   0        0        0      791 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/algo/querying/llm/connectors/__init__.py
+-rw-rw-rw-   0        0        0     2596 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/algo/querying/llm/connectors/openai.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:24.886548 pm4py-2.7.9.4/pm4py/algo/querying/llm/utils/
+-rw-rw-rw-   0        0        0      787 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/algo/querying/llm/utils/__init__.py
+-rw-rw-rw-   0        0        0     1634 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/algo/querying/llm/utils/sql_utils.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:24.886548 pm4py-2.7.9.4/pm4py/algo/reduction/
+-rw-rw-rw-   0        0        0      955 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/algo/reduction/__init__.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:24.905141 pm4py-2.7.9.4/pm4py/algo/reduction/process_tree/
+-rw-rw-rw-   0        0        0      799 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/algo/reduction/process_tree/__init__.py
+-rw-rw-rw-   0        0        0     1601 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/algo/reduction/process_tree/reducer.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:24.905141 pm4py-2.7.9.4/pm4py/algo/reduction/process_tree/variants/
+-rw-rw-rw-   0        0        0      804 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/algo/reduction/process_tree/variants/__init__.py
+-rw-rw-rw-   0        0        0     3743 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/algo/reduction/process_tree/variants/tree_tr_based.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:24.905141 pm4py-2.7.9.4/pm4py/algo/simulation/
+-rw-rw-rw-   0        0        0      904 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/algo/simulation/__init__.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:24.905141 pm4py-2.7.9.4/pm4py/algo/simulation/montecarlo/
+-rw-rw-rw-   0        0        0      995 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/algo/simulation/montecarlo/__init__.py
+-rw-rw-rw-   0        0        0     4562 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/algo/simulation/montecarlo/algorithm.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:24.905141 pm4py-2.7.9.4/pm4py/algo/simulation/montecarlo/utils/
+-rw-rw-rw-   0        0        0      793 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/algo/simulation/montecarlo/utils/__init__.py
+-rw-rw-rw-   0        0        0     5316 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/algo/simulation/montecarlo/utils/replay.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:24.920769 pm4py-2.7.9.4/pm4py/algo/simulation/montecarlo/variants/
+-rw-rw-rw-   0        0        0      807 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/algo/simulation/montecarlo/variants/__init__.py
+-rw-rw-rw-   0        0        0    19853 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/algo/simulation/montecarlo/variants/petri_semaph_fifo.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:24.920769 pm4py-2.7.9.4/pm4py/algo/simulation/playout/
+-rw-rw-rw-   0        0        0      806 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/algo/simulation/playout/__init__.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:24.920769 pm4py-2.7.9.4/pm4py/algo/simulation/playout/dfg/
+-rw-rw-rw-   0        0        0      801 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/algo/simulation/playout/dfg/__init__.py
+-rw-rw-rw-   0        0        0     1940 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/algo/simulation/playout/dfg/algorithm.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:24.920769 pm4py-2.7.9.4/pm4py/algo/simulation/playout/dfg/variants/
+-rw-rw-rw-   0        0        0      811 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/algo/simulation/playout/dfg/variants/__init__.py
+-rw-rw-rw-   0        0        0    14627 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/algo/simulation/playout/dfg/variants/classic.py
+-rw-rw-rw-   0        0        0     6099 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/algo/simulation/playout/dfg/variants/performance.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:24.936391 pm4py-2.7.9.4/pm4py/algo/simulation/playout/petri_net/
+-rw-rw-rw-   0        0        0      807 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/algo/simulation/playout/petri_net/__init__.py
+-rw-rw-rw-   0        0        0     2552 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/algo/simulation/playout/petri_net/algorithm.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:24.936391 pm4py-2.7.9.4/pm4py/algo/simulation/playout/petri_net/variants/
+-rw-rw-rw-   0        0        0      821 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/algo/simulation/playout/petri_net/variants/__init__.py
+-rw-rw-rw-   0        0        0     9126 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/algo/simulation/playout/petri_net/variants/basic_playout.py
+-rw-rw-rw-   0        0        0     5306 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/algo/simulation/playout/petri_net/variants/extensive.py
+-rw-rw-rw-   0        0        0     8008 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/algo/simulation/playout/petri_net/variants/stochastic_playout.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:24.936391 pm4py-2.7.9.4/pm4py/algo/simulation/playout/process_tree/
+-rw-rw-rw-   0        0        0      810 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/algo/simulation/playout/process_tree/__init__.py
+-rw-rw-rw-   0        0        0     1862 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/algo/simulation/playout/process_tree/algorithm.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:24.952518 pm4py-2.7.9.4/pm4py/algo/simulation/playout/process_tree/variants/
+-rw-rw-rw-   0        0        0      835 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/algo/simulation/playout/process_tree/variants/__init__.py
+-rw-rw-rw-   0        0        0     1679 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/algo/simulation/playout/process_tree/variants/basic_playout.py
+-rw-rw-rw-   0        0        0    13571 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/algo/simulation/playout/process_tree/variants/extensive.py
+-rw-rw-rw-   0        0        0     4861 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/algo/simulation/playout/process_tree/variants/topbottom.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:24.952518 pm4py-2.7.9.4/pm4py/algo/simulation/tree_generator/
+-rw-rw-rw-   0        0        0      806 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/algo/simulation/tree_generator/__init__.py
+-rw-rw-rw-   0        0        0     1765 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/algo/simulation/tree_generator/algorithm.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:24.952518 pm4py-2.7.9.4/pm4py/algo/simulation/tree_generator/variants/
+-rw-rw-rw-   0        0        0      818 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/algo/simulation/tree_generator/variants/__init__.py
+-rw-rw-rw-   0        0        0     5357 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/algo/simulation/tree_generator/variants/basic.py
+-rw-rw-rw-   0        0        0    12955 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/algo/simulation/tree_generator/variants/ptandloggenerator.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:24.952518 pm4py-2.7.9.4/pm4py/algo/transformation/
+-rw-rw-rw-   0        0        0      808 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/algo/transformation/__init__.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:24.972119 pm4py-2.7.9.4/pm4py/algo/transformation/log_to_features/
+-rw-rw-rw-   0        0        0      809 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/algo/transformation/log_to_features/__init__.py
+-rw-rw-rw-   0        0        0     2205 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/algo/transformation/log_to_features/algorithm.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:24.972119 pm4py-2.7.9.4/pm4py/algo/transformation/log_to_features/util/
+-rw-rw-rw-   0        0        0      819 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/algo/transformation/log_to_features/util/__init__.py
+-rw-rw-rw-   0        0        0     3933 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/algo/transformation/log_to_features/util/locally_linear_embedding.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:24.972119 pm4py-2.7.9.4/pm4py/algo/transformation/log_to_features/variants/
+-rw-rw-rw-   0        0        0      823 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/algo/transformation/log_to_features/variants/__init__.py
+-rw-rw-rw-   0        0        0     6689 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/algo/transformation/log_to_features/variants/event_based.py
+-rw-rw-rw-   0        0        0     6644 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/algo/transformation/log_to_features/variants/temporal.py
+-rw-rw-rw-   0        0        0    50368 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/algo/transformation/log_to_features/variants/trace_based.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:24.989241 pm4py-2.7.9.4/pm4py/algo/transformation/log_to_interval_tree/
+-rw-rw-rw-   0        0        0      999 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/algo/transformation/log_to_interval_tree/__init__.py
+-rw-rw-rw-   0        0        0     2171 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/algo/transformation/log_to_interval_tree/algorithm.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:24.989241 pm4py-2.7.9.4/pm4py/algo/transformation/log_to_interval_tree/variants/
+-rw-rw-rw-   0        0        0      814 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/algo/transformation/log_to_interval_tree/variants/__init__.py
+-rw-rw-rw-   0        0        0     6365 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/algo/transformation/log_to_interval_tree/variants/open_paths.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:24.989241 pm4py-2.7.9.4/pm4py/algo/transformation/log_to_target/
+-rw-rw-rw-   0        0        0      807 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/algo/transformation/log_to_target/__init__.py
+-rw-rw-rw-   0        0        0     2161 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/algo/transformation/log_to_target/algorithm.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:25.004256 pm4py-2.7.9.4/pm4py/algo/transformation/log_to_target/variants/
+-rw-rw-rw-   0        0        0      837 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/algo/transformation/log_to_target/variants/__init__.py
+-rw-rw-rw-   0        0        0     2922 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/algo/transformation/log_to_target/variants/next_activity.py
+-rw-rw-rw-   0        0        0     2526 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/algo/transformation/log_to_target/variants/next_time.py
+-rw-rw-rw-   0        0        0     2385 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/algo/transformation/log_to_target/variants/remaining_time.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:25.004256 pm4py-2.7.9.4/pm4py/algo/transformation/log_to_trie/
+-rw-rw-rw-   0        0        0      795 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/algo/transformation/log_to_trie/__init__.py
+-rw-rw-rw-   0        0        0     2261 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/algo/transformation/log_to_trie/algorithm.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:25.004256 pm4py-2.7.9.4/pm4py/algo/transformation/ocel/
+-rw-rw-rw-   0        0        0      807 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/algo/transformation/ocel/__init__.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:25.019882 pm4py-2.7.9.4/pm4py/algo/transformation/ocel/description/
+-rw-rw-rw-   0        0        0      736 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/algo/transformation/ocel/description/__init__.py
+-rw-rw-rw-   0        0        0     1684 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/algo/transformation/ocel/description/algorithm.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:25.022544 pm4py-2.7.9.4/pm4py/algo/transformation/ocel/description/variants/
+-rw-rw-rw-   0        0        0      736 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/algo/transformation/ocel/description/variants/__init__.py
+-rw-rw-rw-   0        0        0     3318 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/algo/transformation/ocel/description/variants/variant1.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:25.022544 pm4py-2.7.9.4/pm4py/algo/transformation/ocel/features/
+-rw-rw-rw-   0        0        0      821 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/algo/transformation/ocel/features/__init__.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:25.038165 pm4py-2.7.9.4/pm4py/algo/transformation/ocel/features/events/
+-rw-rw-rw-   0        0        0     1002 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/algo/transformation/ocel/features/events/__init__.py
+-rw-rw-rw-   0        0        0     9094 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/algo/transformation/ocel/features/events/algorithm.py
+-rw-rw-rw-   0        0        0     2022 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/algo/transformation/ocel/features/events/event_activity.py
+-rw-rw-rw-   0        0        0     2250 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/algo/transformation/ocel/features/events/event_end_ot.py
+-rw-rw-rw-   0        0        0     2542 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/algo/transformation/ocel/features/events/event_num_attributes.py
+-rw-rw-rw-   0        0        0     1691 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/algo/transformation/ocel/features/events/event_num_rel_objs.py
+-rw-rw-rw-   0        0        0     2354 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/algo/transformation/ocel/features/events/event_num_rel_objs_type.py
+-rw-rw-rw-   0        0        0     2236 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/algo/transformation/ocel/features/events/event_start_ot.py
+-rw-rw-rw-   0        0        0     3041 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/algo/transformation/ocel/features/events/event_str_attributes.py
+-rw-rw-rw-   0        0        0     2031 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/algo/transformation/ocel/features/events/event_timestamp.py
+-rw-rw-rw-   0        0        0     1990 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/algo/transformation/ocel/features/events/new_interactions.py
+-rw-rw-rw-   0        0        0     2805 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/algo/transformation/ocel/features/events/related_objects_features.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:25.052670 pm4py-2.7.9.4/pm4py/algo/transformation/ocel/features/events_objects/
+-rw-rw-rw-   0        0        0      831 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/algo/transformation/ocel/features/events_objects/__init__.py
+-rw-rw-rw-   0        0        0     3899 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/algo/transformation/ocel/features/events_objects/algorithm.py
+-rw-rw-rw-   0        0        0     4959 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/algo/transformation/ocel/features/events_objects/prefix_features.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:25.086638 pm4py-2.7.9.4/pm4py/algo/transformation/ocel/features/objects/
+-rw-rw-rw-   0        0        0     1268 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/algo/transformation/ocel/features/objects/__init__.py
+-rw-rw-rw-   0        0        0    20532 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/algo/transformation/ocel/features/objects/algorithm.py
+-rw-rw-rw-   0        0        0     3400 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/algo/transformation/ocel/features/objects/obj_con_in_graph_features.py
+-rw-rw-rw-   0        0        0     1912 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/algo/transformation/ocel/features/objects/object_cobirth_graph.py
+-rw-rw-rw-   0        0        0     1912 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/algo/transformation/ocel/features/objects/object_codeath_graph.py
+-rw-rw-rw-   0        0        0     1988 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/algo/transformation/ocel/features/objects/object_degree_centrality.py
+-rw-rw-rw-   0        0        0     2100 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/algo/transformation/ocel/features/objects/object_general_descendants_graph.py
+-rw-rw-rw-   0        0        0     2152 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/algo/transformation/ocel/features/objects/object_general_inheritance_graph.py
+-rw-rw-rw-   0        0        0     1942 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/algo/transformation/ocel/features/objects/object_general_interaction_graph.py
+-rw-rw-rw-   0        0        0     2080 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/algo/transformation/ocel/features/objects/object_lifecycle_activities.py
+-rw-rw-rw-   0        0        0     2197 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/algo/transformation/ocel/features/objects/object_lifecycle_duration.py
+-rw-rw-rw-   0        0        0     1794 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/algo/transformation/ocel/features/objects/object_lifecycle_length.py
+-rw-rw-rw-   0        0        0     2205 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/algo/transformation/ocel/features/objects/object_lifecycle_paths.py
+-rw-rw-rw-   0        0        0     1920 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/algo/transformation/ocel/features/objects/object_lifecycle_unq_act.py
+-rw-rw-rw-   0        0        0     2586 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/algo/transformation/ocel/features/objects/object_num_attributes.py
+-rw-rw-rw-   0        0        0     3062 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/algo/transformation/ocel/features/objects/object_str_attributes.py
+-rw-rw-rw-   0        0        0     2455 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/algo/transformation/ocel/features/objects/object_work_in_progress.py
+-rw-rw-rw-   0        0        0     2486 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/algo/transformation/ocel/features/objects/objects_interaction_graph_ot.py
+-rw-rw-rw-   0        0        0     3063 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/algo/transformation/ocel/features/objects/related_activities_features.py
+-rw-rw-rw-   0        0        0     2788 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/algo/transformation/ocel/features/objects/related_events_features.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:25.102261 pm4py-2.7.9.4/pm4py/algo/transformation/ocel/graphs/
+-rw-rw-rw-   0        0        0      906 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/algo/transformation/ocel/graphs/__init__.py
+-rw-rw-rw-   0        0        0     2305 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/algo/transformation/ocel/graphs/object_cobirth_graph.py
+-rw-rw-rw-   0        0        0     2103 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/algo/transformation/ocel/graphs/object_codeath_graph.py
+-rw-rw-rw-   0        0        0     2327 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/algo/transformation/ocel/graphs/object_descendants_graph.py
+-rw-rw-rw-   0        0        0     2852 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/algo/transformation/ocel/graphs/object_inheritance_graph.py
+-rw-rw-rw-   0        0        0     1736 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/algo/transformation/ocel/graphs/object_interaction_graph.py
+-rw-rw-rw-   0        0        0     3641 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/algo/transformation/ocel/graphs/ocel20_computation.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:25.117881 pm4py-2.7.9.4/pm4py/algo/transformation/ocel/split_ocel/
+-rw-rw-rw-   0        0        0      809 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/algo/transformation/ocel/split_ocel/__init__.py
+-rw-rw-rw-   0        0        0     1730 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/algo/transformation/ocel/split_ocel/algorithm.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:25.117881 pm4py-2.7.9.4/pm4py/algo/transformation/ocel/split_ocel/variants/
+-rw-rw-rw-   0        0        0      819 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/algo/transformation/ocel/split_ocel/variants/__init__.py
+-rw-rw-rw-   0        0        0     3429 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/algo/transformation/ocel/split_ocel/variants/ancestors_descendants.py
+-rw-rw-rw-   0        0        0     3467 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/algo/transformation/ocel/split_ocel/variants/connected_components.py
+-rw-rw-rw-   0        0        0    20646 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/analysis.py
+-rw-rw-rw-   0        0        0    13471 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/cli.py
+-rw-rw-rw-   0        0        0    48213 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/conformance.py
+-rw-rw-rw-   0        0        0    19636 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/connectors.py
+-rw-rw-rw-   0        0        0    20826 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/convert.py
+-rw-rw-rw-   0        0        0    47943 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/discovery.py
+-rw-rw-rw-   0        0        0    63155 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/filtering.py
+-rw-rw-rw-   0        0        0     5192 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/hof.py
+-rw-rw-rw-   0        0        0    18976 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/llm.py
+-rw-rw-rw-   0        0        0     1091 2024-01-29 06:14:09.000000 pm4py-2.7.9.4/pm4py/meta.py
+-rw-rw-rw-   0        0        0    16160 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/ml.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:25.117881 pm4py-2.7.9.4/pm4py/objects/
+-rw-rw-rw-   0        0        0      947 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/objects/__init__.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:25.133502 pm4py-2.7.9.4/pm4py/objects/bpmn/
+-rw-rw-rw-   0        0        0      913 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/objects/bpmn/__init__.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:25.133502 pm4py-2.7.9.4/pm4py/objects/bpmn/exporter/
+-rw-rw-rw-   0        0        0      794 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/objects/bpmn/exporter/__init__.py
+-rw-rw-rw-   0        0        0     2130 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/objects/bpmn/exporter/exporter.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:25.150934 pm4py-2.7.9.4/pm4py/objects/bpmn/exporter/variants/
+-rw-rw-rw-   0        0        0      790 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/objects/bpmn/exporter/variants/__init__.py
+-rw-rw-rw-   0        0        0     7688 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/objects/bpmn/exporter/variants/etree.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:25.152942 pm4py-2.7.9.4/pm4py/objects/bpmn/importer/
+-rw-rw-rw-   0        0        0      794 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/objects/bpmn/importer/__init__.py
+-rw-rw-rw-   0        0        0     2085 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/objects/bpmn/importer/importer.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:25.152942 pm4py-2.7.9.4/pm4py/objects/bpmn/importer/variants/
+-rw-rw-rw-   0        0        0      789 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/objects/bpmn/importer/variants/__init__.py
+-rw-rw-rw-   0        0        0    17373 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/objects/bpmn/importer/variants/lxml.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:25.152942 pm4py-2.7.9.4/pm4py/objects/bpmn/layout/
+-rw-rw-rw-   0        0        0      792 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/objects/bpmn/layout/__init__.py
+-rw-rw-rw-   0        0        0     1534 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/objects/bpmn/layout/layouter.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:25.168572 pm4py-2.7.9.4/pm4py/objects/bpmn/layout/variants/
+-rw-rw-rw-   0        0        0      793 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/objects/bpmn/layout/variants/__init__.py
+-rw-rw-rw-   0        0        0    18042 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/objects/bpmn/layout/variants/graphviz.py
+-rw-rw-rw-   0        0        0    19676 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/objects/bpmn/obj.py
+-rw-rw-rw-   0        0        0     9205 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/objects/bpmn/semantics.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:25.168572 pm4py-2.7.9.4/pm4py/objects/bpmn/util/
+-rw-rw-rw-   0        0        0      802 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/objects/bpmn/util/__init__.py
+-rw-rw-rw-   0        0        0     6246 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/objects/bpmn/util/bpmn_utils.py
+-rw-rw-rw-   0        0        0     3352 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/objects/bpmn/util/reduction.py
+-rw-rw-rw-   0        0        0     3729 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/objects/bpmn/util/sorting.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:25.184194 pm4py-2.7.9.4/pm4py/objects/conversion/
+-rw-rw-rw-   0        0        0      825 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/objects/conversion/__init__.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:25.184194 pm4py-2.7.9.4/pm4py/objects/conversion/bpmn/
+-rw-rw-rw-   0        0        0      797 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/objects/conversion/bpmn/__init__.py
+-rw-rw-rw-   0        0        0     1160 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/objects/conversion/bpmn/converter.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:25.184194 pm4py-2.7.9.4/pm4py/objects/conversion/bpmn/variants/
+-rw-rw-rw-   0        0        0      799 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/objects/conversion/bpmn/variants/__init__.py
+-rw-rw-rw-   0        0        0    10026 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/objects/conversion/bpmn/variants/to_petri_net.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:25.199815 pm4py-2.7.9.4/pm4py/objects/conversion/dfg/
+-rw-rw-rw-   0        0        0      796 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/objects/conversion/dfg/__init__.py
+-rw-rw-rw-   0        0        0     1340 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/objects/conversion/dfg/converter.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:25.199815 pm4py-2.7.9.4/pm4py/objects/conversion/dfg/variants/
+-rw-rw-rw-   0        0        0      860 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/objects/conversion/dfg/variants/__init__.py
+-rw-rw-rw-   0        0        0     3494 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/objects/conversion/dfg/variants/to_petri_net_activity_defines_place.py
+-rw-rw-rw-   0        0        0     4229 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/objects/conversion/dfg/variants/to_petri_net_invisibles_no_duplicates.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:25.215436 pm4py-2.7.9.4/pm4py/objects/conversion/heuristics_net/
+-rw-rw-rw-   0        0        0      807 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/objects/conversion/heuristics_net/__init__.py
+-rw-rw-rw-   0        0        0     1384 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/objects/conversion/heuristics_net/converter.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:25.215436 pm4py-2.7.9.4/pm4py/objects/conversion/heuristics_net/variants/
+-rw-rw-rw-   0        0        0      809 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/objects/conversion/heuristics_net/variants/__init__.py
+-rw-rw-rw-   0        0        0    11773 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/objects/conversion/heuristics_net/variants/to_petri_net.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:25.215436 pm4py-2.7.9.4/pm4py/objects/conversion/log/
+-rw-rw-rw-   0        0        0      807 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/objects/conversion/log/__init__.py
+-rw-rw-rw-   0        0        0     1061 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/objects/conversion/log/constants.py
+-rw-rw-rw-   0        0        0     1319 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/objects/conversion/log/converter.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:25.246679 pm4py-2.7.9.4/pm4py/objects/conversion/log/variants/
+-rw-rw-rw-   0        0        0      870 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/objects/conversion/log/variants/__init__.py
+-rw-rw-rw-   0        0        0     1923 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/objects/conversion/log/variants/df_to_event_log_1v.py
+-rw-rw-rw-   0        0        0     2535 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/objects/conversion/log/variants/df_to_event_log_nv.py
+-rw-rw-rw-   0        0        0     2585 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/objects/conversion/log/variants/to_data_frame.py
+-rw-rw-rw-   0        0        0     4332 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/objects/conversion/log/variants/to_event_log.py
+-rw-rw-rw-   0        0        0    10224 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/objects/conversion/log/variants/to_event_stream.py
+-rw-rw-rw-   0        0        0     5236 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/objects/conversion/log/variants/to_nx.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:25.253187 pm4py-2.7.9.4/pm4py/objects/conversion/ocel/
+-rw-rw-rw-   0        0        0      799 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/objects/conversion/ocel/__init__.py
+-rw-rw-rw-   0        0        0     1814 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/objects/conversion/ocel/converter.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:25.253187 pm4py-2.7.9.4/pm4py/objects/conversion/ocel/variants/
+-rw-rw-rw-   0        0        0      820 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/objects/conversion/ocel/variants/__init__.py
+-rw-rw-rw-   0        0        0     4056 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/objects/conversion/ocel/variants/ocel_features_to_nx.py
+-rw-rw-rw-   0        0        0     4164 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/objects/conversion/ocel/variants/ocel_to_nx.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:25.268816 pm4py-2.7.9.4/pm4py/objects/conversion/powl/
+-rw-rw-rw-   0        0        0      781 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/objects/conversion/powl/__init__.py
+-rw-rw-rw-   0        0        0     1494 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/objects/conversion/powl/converter.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:25.268816 pm4py-2.7.9.4/pm4py/objects/conversion/powl/variants/
+-rw-rw-rw-   0        0        0      790 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/objects/conversion/powl/variants/__init__.py
+-rw-rw-rw-   0        0        0    11169 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/objects/conversion/powl/variants/to_petri_net.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:25.268816 pm4py-2.7.9.4/pm4py/objects/conversion/process_tree/
+-rw-rw-rw-   0        0        0      805 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/objects/conversion/process_tree/__init__.py
+-rw-rw-rw-   0        0        0     1824 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/objects/conversion/process_tree/converter.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:25.284437 pm4py-2.7.9.4/pm4py/objects/conversion/process_tree/variants/
+-rw-rw-rw-   0        0        0      850 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/objects/conversion/process_tree/variants/__init__.py
+-rw-rw-rw-   0        0        0    10139 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/objects/conversion/process_tree/variants/to_bpmn.py
+-rw-rw-rw-   0        0        0    21550 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/objects/conversion/process_tree/variants/to_petri_net.py
+-rw-rw-rw-   0        0        0     4772 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/objects/conversion/process_tree/variants/to_petri_net_transition_bordered.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:25.284437 pm4py-2.7.9.4/pm4py/objects/conversion/wf_net/
+-rw-rw-rw-   0        0        0      799 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/objects/conversion/wf_net/__init__.py
+-rw-rw-rw-   0        0        0     1167 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/objects/conversion/wf_net/converter.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:25.284437 pm4py-2.7.9.4/pm4py/objects/conversion/wf_net/variants/
+-rw-rw-rw-   0        0        0      813 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/objects/conversion/wf_net/variants/__init__.py
+-rw-rw-rw-   0        0        0     3774 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/objects/conversion/wf_net/variants/to_bpmn.py
+-rw-rw-rw-   0        0        0    10849 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/objects/conversion/wf_net/variants/to_process_tree.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:25.300058 pm4py-2.7.9.4/pm4py/objects/dfg/
+-rw-rw-rw-   0        0        0      796 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/objects/dfg/__init__.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:25.300058 pm4py-2.7.9.4/pm4py/objects/dfg/exporter/
+-rw-rw-rw-   0        0        0      793 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/objects/dfg/exporter/__init__.py
+-rw-rw-rw-   0        0        0     2041 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/objects/dfg/exporter/exporter.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:25.315681 pm4py-2.7.9.4/pm4py/objects/dfg/exporter/variants/
+-rw-rw-rw-   0        0        0      791 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/objects/dfg/exporter/variants/__init__.py
+-rw-rw-rw-   0        0        0     4571 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/objects/dfg/exporter/variants/classic.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:25.315681 pm4py-2.7.9.4/pm4py/objects/dfg/filtering/
+-rw-rw-rw-   0        0        0      734 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/objects/dfg/filtering/__init__.py
+-rw-rw-rw-   0        0        0      788 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/objects/dfg/filtering/dfg_filtering.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:25.315681 pm4py-2.7.9.4/pm4py/objects/dfg/importer/
+-rw-rw-rw-   0        0        0      793 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/objects/dfg/importer/__init__.py
+-rw-rw-rw-   0        0        0     2278 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/objects/dfg/importer/importer.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:25.315681 pm4py-2.7.9.4/pm4py/objects/dfg/importer/variants/
+-rw-rw-rw-   0        0        0      791 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/objects/dfg/importer/variants/__init__.py
+-rw-rw-rw-   0        0        0     4037 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/objects/dfg/importer/variants/classic.py
+-rw-rw-rw-   0        0        0     1881 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/objects/dfg/obj.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:25.331301 pm4py-2.7.9.4/pm4py/objects/dfg/retrieval/
+-rw-rw-rw-   0        0        0      734 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/objects/dfg/retrieval/__init__.py
+-rw-rw-rw-   0        0        0      913 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/objects/dfg/retrieval/log.py
+-rw-rw-rw-   0        0        0      873 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/objects/dfg/retrieval/pandas.py
+-rw-rw-rw-   0        0        0     5092 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/objects/dfg/util.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:25.331301 pm4py-2.7.9.4/pm4py/objects/dfg/utils/
+-rw-rw-rw-   0        0        0      781 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/objects/dfg/utils/__init__.py
+-rw-rw-rw-   0        0        0    26490 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/objects/dfg/utils/dfg_utils.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:25.346922 pm4py-2.7.9.4/pm4py/objects/heuristics_net/
+-rw-rw-rw-   0        0        0      802 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/objects/heuristics_net/__init__.py
+-rw-rw-rw-   0        0        0     1226 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/objects/heuristics_net/defaults.py
+-rw-rw-rw-   0        0        0     2689 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/objects/heuristics_net/edge.py
+-rw-rw-rw-   0        0        0     9877 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/objects/heuristics_net/node.py
+-rw-rw-rw-   0        0        0     5684 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/objects/heuristics_net/obj.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:25.353429 pm4py-2.7.9.4/pm4py/objects/log/
+-rw-rw-rw-   0        0        0      795 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/objects/log/__init__.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:25.353429 pm4py-2.7.9.4/pm4py/objects/log/exporter/
+-rw-rw-rw-   0        0        0      778 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/objects/log/exporter/__init__.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:25.353429 pm4py-2.7.9.4/pm4py/objects/log/exporter/xes/
+-rw-rw-rw-   0        0        0      803 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/objects/log/exporter/xes/__init__.py
+-rw-rw-rw-   0        0        0     2578 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/objects/log/exporter/xes/exporter.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:25.353429 pm4py-2.7.9.4/pm4py/objects/log/exporter/xes/util/
+-rw-rw-rw-   0        0        0      795 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/objects/log/exporter/xes/util/__init__.py
+-rw-rw-rw-   0        0        0     1423 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/objects/log/exporter/xes/util/compression.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:25.371503 pm4py-2.7.9.4/pm4py/objects/log/exporter/xes/variants/
+-rw-rw-rw-   0        0        0      815 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/objects/log/exporter/xes/variants/__init__.py
+-rw-rw-rw-   0        0        0    12326 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/objects/log/exporter/xes/variants/etree_xes_exp.py
+-rw-rw-rw-   0        0        0    10430 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/objects/log/exporter/xes/variants/line_by_line.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:25.371503 pm4py-2.7.9.4/pm4py/objects/log/importer/
+-rw-rw-rw-   0        0        0      778 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/objects/log/importer/__init__.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:25.371503 pm4py-2.7.9.4/pm4py/objects/log/importer/xes/
+-rw-rw-rw-   0        0        0      797 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/objects/log/importer/xes/__init__.py
+-rw-rw-rw-   0        0        0     4379 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/objects/log/importer/xes/importer.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:25.387130 pm4py-2.7.9.4/pm4py/objects/log/importer/xes/variants/
+-rw-rw-rw-   0        0        0      850 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/objects/log/importer/xes/variants/__init__.py
+-rw-rw-rw-   0        0        0     9534 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/objects/log/importer/xes/variants/chunk_regex.py
+-rw-rw-rw-   0        0        0    17582 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/objects/log/importer/xes/variants/iterparse.py
+-rw-rw-rw-   0        0        0    17851 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/objects/log/importer/xes/variants/iterparse_20.py
+-rw-rw-rw-   0        0        0    18150 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/objects/log/importer/xes/variants/iterparse_mem_compressed.py
+-rw-rw-rw-   0        0        0    11435 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/objects/log/importer/xes/variants/line_by_line.py
+-rw-rw-rw-   0        0        0     2094 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/objects/log/importer/xes/variants/rustxes.py
+-rw-rw-rw-   0        0        0    12284 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/objects/log/obj.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:25.419454 pm4py-2.7.9.4/pm4py/objects/log/util/
+-rw-rw-rw-   0        0        0     1010 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/objects/log/util/__init__.py
+-rw-rw-rw-   0        0        0     3127 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/objects/log/util/activities_to_alphabet.py
+-rw-rw-rw-   0        0        0     3114 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/objects/log/util/artificial.py
+-rw-rw-rw-   0        0        0     3974 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/objects/log/util/basic_filter.py
+-rw-rw-rw-   0        0        0    18992 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/objects/log/util/dataframe_utils.py
+-rw-rw-rw-   0        0        0     2283 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/objects/log/util/filtering_utils.py
+-rw-rw-rw-   0        0        0     4856 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/objects/log/util/get_class_representation.py
+-rw-rw-rw-   0        0        0     3195 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/objects/log/util/get_log_encoded.py
+-rw-rw-rw-   0        0        0     8099 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/objects/log/util/get_prefixes.py
+-rw-rw-rw-   0        0        0     1752 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/objects/log/util/index_attribute.py
+-rw-rw-rw-   0        0        0     4067 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/objects/log/util/insert_classifier.py
+-rw-rw-rw-   0        0        0    12476 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/objects/log/util/interval_lifecycle.py
+-rw-rw-rw-   0        0        0     5167 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/objects/log/util/log.py
+-rw-rw-rw-   0        0        0     4389 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/objects/log/util/log_regex.py
+-rw-rw-rw-   0        0        0     2867 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/objects/log/util/move_attrs_to_trace.py
+-rw-rw-rw-   0        0        0     4527 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/objects/log/util/pandas_log_wrapper.py
+-rw-rw-rw-   0        0        0     4094 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/objects/log/util/pandas_numpy_variants.py
+-rw-rw-rw-   0        0        0     2465 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/objects/log/util/sampling.py
+-rw-rw-rw-   0        0        0     6049 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/objects/log/util/sorting.py
+-rw-rw-rw-   0        0        0     2078 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/objects/log/util/split_train_test.py
+-rw-rw-rw-   0        0        0     1695 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/objects/log/util/xes.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:25.435076 pm4py-2.7.9.4/pm4py/objects/ocel/
+-rw-rw-rw-   0        0        0      819 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/objects/ocel/__init__.py
+-rw-rw-rw-   0        0        0     2372 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/objects/ocel/constants.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:25.435076 pm4py-2.7.9.4/pm4py/objects/ocel/exporter/
+-rw-rw-rw-   0        0        0      911 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/objects/ocel/exporter/__init__.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:25.435076 pm4py-2.7.9.4/pm4py/objects/ocel/exporter/csv/
+-rw-rw-rw-   0        0        0      798 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/objects/ocel/exporter/csv/__init__.py
+-rw-rw-rw-   0        0        0     1695 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/objects/ocel/exporter/csv/exporter.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:25.452275 pm4py-2.7.9.4/pm4py/objects/ocel/exporter/csv/variants/
+-rw-rw-rw-   0        0        0      795 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/objects/ocel/exporter/csv/variants/__init__.py
+-rw-rw-rw-   0        0        0     1927 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/objects/ocel/exporter/csv/variants/pandas.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:25.456403 pm4py-2.7.9.4/pm4py/objects/ocel/exporter/jsonocel/
+-rw-rw-rw-   0        0        0      803 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/objects/ocel/exporter/jsonocel/__init__.py
+-rw-rw-rw-   0        0        0     1635 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/objects/ocel/exporter/jsonocel/exporter.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:25.456403 pm4py-2.7.9.4/pm4py/objects/ocel/exporter/jsonocel/variants/
+-rw-rw-rw-   0        0        0      826 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/objects/ocel/exporter/jsonocel/variants/__init__.py
+-rw-rw-rw-   0        0        0     5448 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/objects/ocel/exporter/jsonocel/variants/classic.py
+-rw-rw-rw-   0        0        0     5591 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/objects/ocel/exporter/jsonocel/variants/ocel20.py
+-rw-rw-rw-   0        0        0     4247 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/objects/ocel/exporter/jsonocel/variants/ocel20_standard.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:25.456403 pm4py-2.7.9.4/pm4py/objects/ocel/exporter/sqlite/
+-rw-rw-rw-   0        0        0      803 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/objects/ocel/exporter/sqlite/__init__.py
+-rw-rw-rw-   0        0        0     1673 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/objects/ocel/exporter/sqlite/exporter.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:25.472025 pm4py-2.7.9.4/pm4py/objects/ocel/exporter/sqlite/variants/
+-rw-rw-rw-   0        0        0      809 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/objects/ocel/exporter/sqlite/variants/__init__.py
+-rw-rw-rw-   0        0        0     4931 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/objects/ocel/exporter/sqlite/variants/ocel20.py
+-rw-rw-rw-   0        0        0     1679 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/objects/ocel/exporter/sqlite/variants/pandas_exporter.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:25.472025 pm4py-2.7.9.4/pm4py/objects/ocel/exporter/util/
+-rw-rw-rw-   0        0        0      797 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/objects/ocel/exporter/util/__init__.py
+-rw-rw-rw-   0        0        0     1658 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/objects/ocel/exporter/util/clean_dataframes.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:25.472025 pm4py-2.7.9.4/pm4py/objects/ocel/exporter/xmlocel/
+-rw-rw-rw-   0        0        0      802 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/objects/ocel/exporter/xmlocel/__init__.py
+-rw-rw-rw-   0        0        0     1578 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/objects/ocel/exporter/xmlocel/exporter.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:25.487646 pm4py-2.7.9.4/pm4py/objects/ocel/exporter/xmlocel/variants/
+-rw-rw-rw-   0        0        0      734 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/objects/ocel/exporter/xmlocel/variants/__init__.py
+-rw-rw-rw-   0        0        0     8129 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/objects/ocel/exporter/xmlocel/variants/classic.py
+-rw-rw-rw-   0        0        0     8746 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/objects/ocel/exporter/xmlocel/variants/ocel20.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:25.487646 pm4py-2.7.9.4/pm4py/objects/ocel/importer/
+-rw-rw-rw-   0        0        0      905 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/objects/ocel/importer/__init__.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:25.487646 pm4py-2.7.9.4/pm4py/objects/ocel/importer/csv/
+-rw-rw-rw-   0        0        0      798 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/objects/ocel/importer/csv/__init__.py
+-rw-rw-rw-   0        0        0     1731 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/objects/ocel/importer/csv/importer.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:25.503268 pm4py-2.7.9.4/pm4py/objects/ocel/importer/csv/variants/
+-rw-rw-rw-   0        0        0      795 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/objects/ocel/importer/csv/variants/__init__.py
+-rw-rw-rw-   0        0        0     2211 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/objects/ocel/importer/csv/variants/pandas.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:25.503268 pm4py-2.7.9.4/pm4py/objects/ocel/importer/jsonocel/
+-rw-rw-rw-   0        0        0      803 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/objects/ocel/importer/jsonocel/__init__.py
+-rw-rw-rw-   0        0        0     1641 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/objects/ocel/importer/jsonocel/importer.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:25.503268 pm4py-2.7.9.4/pm4py/objects/ocel/importer/jsonocel/variants/
+-rw-rw-rw-   0        0        0      818 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/objects/ocel/importer/jsonocel/variants/__init__.py
+-rw-rw-rw-   0        0        0     7338 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/objects/ocel/importer/jsonocel/variants/classic.py
+-rw-rw-rw-   0        0        0     3863 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/objects/ocel/importer/jsonocel/variants/ocel20_standard.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:25.503268 pm4py-2.7.9.4/pm4py/objects/ocel/importer/sqlite/
+-rw-rw-rw-   0        0        0      803 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/objects/ocel/importer/sqlite/__init__.py
+-rw-rw-rw-   0        0        0     1704 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/objects/ocel/importer/sqlite/importer.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:25.518889 pm4py-2.7.9.4/pm4py/objects/ocel/importer/sqlite/variants/
+-rw-rw-rw-   0        0        0      809 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/objects/ocel/importer/sqlite/variants/__init__.py
+-rw-rw-rw-   0        0        0     8462 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/objects/ocel/importer/sqlite/variants/ocel20.py
+-rw-rw-rw-   0        0        0     2620 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/objects/ocel/importer/sqlite/variants/pandas_importer.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:25.518889 pm4py-2.7.9.4/pm4py/objects/ocel/importer/xmlocel/
+-rw-rw-rw-   0        0        0      802 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/objects/ocel/importer/xmlocel/__init__.py
+-rw-rw-rw-   0        0        0     1611 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/objects/ocel/importer/xmlocel/importer.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:25.518889 pm4py-2.7.9.4/pm4py/objects/ocel/importer/xmlocel/variants/
+-rw-rw-rw-   0        0        0      800 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/objects/ocel/importer/xmlocel/variants/__init__.py
+-rw-rw-rw-   0        0        0     8919 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/objects/ocel/importer/xmlocel/variants/classic.py
+-rw-rw-rw-   0        0        0    10021 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/objects/ocel/importer/xmlocel/variants/ocel20.py
+-rw-rw-rw-   0        0        0     7221 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/objects/ocel/obj.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:25.583321 pm4py-2.7.9.4/pm4py/objects/ocel/util/
+-rw-rw-rw-   0        0        0     1067 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/objects/ocel/util/__init__.py
+-rw-rw-rw-   0        0        0     1690 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/objects/ocel/util/attributes_names.py
+-rw-rw-rw-   0        0        0     2156 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/objects/ocel/util/attributes_per_type.py
+-rw-rw-rw-   0        0        0     2424 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/objects/ocel/util/convergence_divergence_diagnostics.py
+-rw-rw-rw-   0        0        0     2690 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/objects/ocel/util/e2o_qualification.py
+-rw-rw-rw-   0        0        0     3809 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/objects/ocel/util/ev_att_to_obj_type.py
+-rw-rw-rw-   0        0        0     4453 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/objects/ocel/util/event_prefix_suffix_per_obj.py
+-rw-rw-rw-   0        0        0     2215 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/objects/ocel/util/events_per_object_type.py
+-rw-rw-rw-   0        0        0     3274 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/objects/ocel/util/events_per_type_per_activity.py
+-rw-rw-rw-   0        0        0     1654 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/objects/ocel/util/explode.py
+-rw-rw-rw-   0        0        0     5068 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/objects/ocel/util/extended_table.py
+-rw-rw-rw-   0        0        0     6565 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/objects/ocel/util/filtering_utils.py
+-rw-rw-rw-   0        0        0     3069 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/objects/ocel/util/flattening.py
+-rw-rw-rw-   0        0        0    17070 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/objects/ocel/util/log_ocel.py
+-rw-rw-rw-   0        0        0      942 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/objects/ocel/util/names_stripping.py
+-rw-rw-rw-   0        0        0     3274 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/objects/ocel/util/objects_per_type_per_activity.py
+-rw-rw-rw-   0        0        0     1974 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/objects/ocel/util/ocel_consistency.py
+-rw-rw-rw-   0        0        0     1976 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/objects/ocel/util/ocel_iterator.py
+-rw-rw-rw-   0        0        0     5167 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/objects/ocel/util/ocel_to_dict_types_rel.py
+-rw-rw-rw-   0        0        0     3510 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/objects/ocel/util/ocel_type_renaming.py
+-rw-rw-rw-   0        0        0     2478 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/objects/ocel/util/parent_children_ref.py
+-rw-rw-rw-   0        0        0     1362 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/objects/ocel/util/related_events.py
+-rw-rw-rw-   0        0        0     1830 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/objects/ocel/util/related_objects.py
+-rw-rw-rw-   0        0        0     2610 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/objects/ocel/util/rename_objs_ot_tim_lex.py
+-rw-rw-rw-   0        0        0     3783 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/objects/ocel/util/sampling.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:25.598941 pm4py-2.7.9.4/pm4py/objects/ocel/validation/
+-rw-rw-rw-   0        0        0      795 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/objects/ocel/validation/__init__.py
+-rw-rw-rw-   0        0        0     1389 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/objects/ocel/validation/jsonocel.py
+-rw-rw-rw-   0        0        0    14786 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/objects/ocel/validation/ocel20_rel_validation.py
+-rw-rw-rw-   0        0        0     1212 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/objects/ocel/validation/xmlocel.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:25.598941 pm4py-2.7.9.4/pm4py/objects/org/
+-rw-rw-rw-   0        0        0      776 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/objects/org/__init__.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:25.598941 pm4py-2.7.9.4/pm4py/objects/org/roles/
+-rw-rw-rw-   0        0        0      775 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/objects/org/roles/__init__.py
+-rw-rw-rw-   0        0        0     1339 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/objects/org/roles/obj.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:25.614563 pm4py-2.7.9.4/pm4py/objects/org/sna/
+-rw-rw-rw-   0        0        0      773 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/objects/org/sna/__init__.py
+-rw-rw-rw-   0        0        0     1029 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/objects/org/sna/obj.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:25.630184 pm4py-2.7.9.4/pm4py/objects/petri_net/
+-rw-rw-rw-   0        0        0      828 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/objects/petri_net/__init__.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:25.630184 pm4py-2.7.9.4/pm4py/objects/petri_net/data_petri_nets/
+-rw-rw-rw-   0        0        0      734 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/objects/petri_net/data_petri_nets/__init__.py
+-rw-rw-rw-   0        0        0     1287 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/objects/petri_net/data_petri_nets/data_marking.py
+-rw-rw-rw-   0        0        0     6212 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/objects/petri_net/data_petri_nets/semantics.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:25.630184 pm4py-2.7.9.4/pm4py/objects/petri_net/exporter/
+-rw-rw-rw-   0        0        0      799 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/objects/petri_net/exporter/__init__.py
+-rw-rw-rw-   0        0        0     2366 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/objects/petri_net/exporter/exporter.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:25.645806 pm4py-2.7.9.4/pm4py/objects/petri_net/exporter/variants/
+-rw-rw-rw-   0        0        0      794 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/objects/petri_net/exporter/variants/__init__.py
+-rw-rw-rw-   0        0        0    13002 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/objects/petri_net/exporter/variants/pnml.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:25.653315 pm4py-2.7.9.4/pm4py/objects/petri_net/importer/
+-rw-rw-rw-   0        0        0      799 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/objects/petri_net/importer/__init__.py
+-rw-rw-rw-   0        0        0     1910 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/objects/petri_net/importer/importer.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:25.653315 pm4py-2.7.9.4/pm4py/objects/petri_net/importer/variants/
+-rw-rw-rw-   0        0        0      794 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/objects/petri_net/importer/variants/__init__.py
+-rw-rw-rw-   0        0        0    15369 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/objects/petri_net/importer/variants/pnml.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:25.653315 pm4py-2.7.9.4/pm4py/objects/petri_net/inhibitor_reset/
+-rw-rw-rw-   0        0        0      734 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/objects/petri_net/inhibitor_reset/__init__.py
+-rw-rw-rw-   0        0        0     4617 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/objects/petri_net/inhibitor_reset/semantics.py
+-rw-rw-rw-   0        0        0    13270 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/objects/petri_net/obj.py
+-rw-rw-rw-   0        0        0     1225 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/objects/petri_net/properties.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:25.668942 pm4py-2.7.9.4/pm4py/objects/petri_net/saw_net/
+-rw-rw-rw-   0        0        0      805 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/objects/petri_net/saw_net/__init__.py
+-rw-rw-rw-   0        0        0     4799 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/objects/petri_net/saw_net/convert.py
+-rw-rw-rw-   0        0        0     1546 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/objects/petri_net/saw_net/obj.py
+-rw-rw-rw-   0        0        0    10711 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/objects/petri_net/saw_net/semantics.py
+-rw-rw-rw-   0        0        0     1503 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/objects/petri_net/sem_interface.py
+-rw-rw-rw-   0        0        0     5339 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/objects/petri_net/semantics.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:25.668942 pm4py-2.7.9.4/pm4py/objects/petri_net/stochastic/
+-rw-rw-rw-   0        0        0      799 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/objects/petri_net/stochastic/__init__.py
+-rw-rw-rw-   0        0        0     1448 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/objects/petri_net/stochastic/obj.py
+-rw-rw-rw-   0        0        0     2607 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/objects/petri_net/stochastic/semantics.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:25.717271 pm4py-2.7.9.4/pm4py/objects/petri_net/utils/
+-rw-rw-rw-   0        0        0     1035 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/objects/petri_net/utils/__init__.py
+-rw-rw-rw-   0        0        0    19297 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/objects/petri_net/utils/align_utils.py
+-rw-rw-rw-   0        0        0     5923 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/objects/petri_net/utils/check_soundness.py
+-rw-rw-rw-   0        0        0     4014 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/objects/petri_net/utils/consumption_matrix.py
+-rw-rw-rw-   0        0        0     6609 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/objects/petri_net/utils/decomposition.py
+-rw-rw-rw-   0        0        0     1672 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/objects/petri_net/utils/embed_stochastic_map.py
+-rw-rw-rw-   0        0        0     5751 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/objects/petri_net/utils/explore_path.py
+-rw-rw-rw-   0        0        0     1195 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/objects/petri_net/utils/final_marking.py
+-rw-rw-rw-   0        0        0     2272 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/objects/petri_net/utils/incidence_matrix.py
+-rw-rw-rw-   0        0        0     1227 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/objects/petri_net/utils/initial_marking.py
+-rw-rw-rw-   0        0        0     4243 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/objects/petri_net/utils/murata.py
+-rw-rw-rw-   0        0        0     4281 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/objects/petri_net/utils/networkx_graph.py
+-rw-rw-rw-   0        0        0     4071 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/objects/petri_net/utils/obj_marking.py
+-rw-rw-rw-   0        0        0    22973 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/objects/petri_net/utils/performance_map.py
+-rw-rw-rw-   0        0        0    20395 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/objects/petri_net/utils/petri_utils.py
+-rw-rw-rw-   0        0        0     4602 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/objects/petri_net/utils/projection.py
+-rw-rw-rw-   0        0        0     5570 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/objects/petri_net/utils/reachability_graph.py
+-rw-rw-rw-   0        0        0    14266 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/objects/petri_net/utils/reduction.py
+-rw-rw-rw-   0        0        0     7288 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/objects/petri_net/utils/synchronous_product.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:25.732893 pm4py-2.7.9.4/pm4py/objects/powl/
+-rw-rw-rw-   0        0        0     6732 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/objects/powl/BinaryRelation.py
+-rw-rw-rw-   0        0        0      772 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/objects/powl/__init__.py
+-rw-rw-rw-   0        0        0      804 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/objects/powl/constants.py
+-rw-rw-rw-   0        0        0    15122 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/objects/powl/obj.py
+-rw-rw-rw-   0        0        0     5268 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/objects/powl/parser.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:25.732893 pm4py-2.7.9.4/pm4py/objects/process_tree/
+-rw-rw-rw-   0        0        0      929 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/objects/process_tree/__init__.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:25.732893 pm4py-2.7.9.4/pm4py/objects/process_tree/exporter/
+-rw-rw-rw-   0        0        0      802 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/objects/process_tree/exporter/__init__.py
+-rw-rw-rw-   0        0        0     1888 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/objects/process_tree/exporter/exporter.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:25.748514 pm4py-2.7.9.4/pm4py/objects/process_tree/exporter/variants/
+-rw-rw-rw-   0        0        0      797 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/objects/process_tree/exporter/variants/__init__.py
+-rw-rw-rw-   0        0        0     5832 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/objects/process_tree/exporter/variants/ptml.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:25.753522 pm4py-2.7.9.4/pm4py/objects/process_tree/importer/
+-rw-rw-rw-   0        0        0      802 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/objects/process_tree/importer/__init__.py
+-rw-rw-rw-   0        0        0     2048 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/objects/process_tree/importer/importer.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:25.753522 pm4py-2.7.9.4/pm4py/objects/process_tree/importer/variants/
+-rw-rw-rw-   0        0        0      797 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/objects/process_tree/importer/variants/__init__.py
+-rw-rw-rw-   0        0        0     5476 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/objects/process_tree/importer/variants/ptml.py
+-rw-rw-rw-   0        0        0     8283 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/objects/process_tree/obj.py
+-rw-rw-rw-   0        0        0     8883 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/objects/process_tree/semantics.py
+-rw-rw-rw-   0        0        0      887 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/objects/process_tree/state.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:25.753522 pm4py-2.7.9.4/pm4py/objects/process_tree/utils/
+-rw-rw-rw-   0        0        0      734 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/objects/process_tree/utils/__init__.py
+-rw-rw-rw-   0        0        0     7128 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/objects/process_tree/utils/bottomup.py
+-rw-rw-rw-   0        0        0    15834 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/objects/process_tree/utils/generic.py
+-rw-rw-rw-   0        0        0     3438 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/objects/process_tree/utils/regex.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:25.769153 pm4py-2.7.9.4/pm4py/objects/random_variables/
+-rw-rw-rw-   0        0        0     1034 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/objects/random_variables/__init__.py
+-rw-rw-rw-   0        0        0     3878 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/objects/random_variables/basic_structure.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:25.769153 pm4py-2.7.9.4/pm4py/objects/random_variables/constant0/
+-rw-rw-rw-   0        0        0      804 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/objects/random_variables/constant0/__init__.py
+-rw-rw-rw-   0        0        0     3586 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/objects/random_variables/constant0/random_variable.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:25.769153 pm4py-2.7.9.4/pm4py/objects/random_variables/exponential/
+-rw-rw-rw-   0        0        0      818 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/objects/random_variables/exponential/__init__.py
+-rw-rw-rw-   0        0        0     3684 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/objects/random_variables/exponential/random_variable.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:25.769153 pm4py-2.7.9.4/pm4py/objects/random_variables/gamma/
+-rw-rw-rw-   0        0        0      800 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/objects/random_variables/gamma/__init__.py
+-rw-rw-rw-   0        0        0     3841 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/objects/random_variables/gamma/random_variable.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:25.784771 pm4py-2.7.9.4/pm4py/objects/random_variables/lognormal/
+-rw-rw-rw-   0        0        0      804 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/objects/random_variables/lognormal/__init__.py
+-rw-rw-rw-   0        0        0     3568 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/objects/random_variables/lognormal/random_variable.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:25.784771 pm4py-2.7.9.4/pm4py/objects/random_variables/normal/
+-rw-rw-rw-   0        0        0      801 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/objects/random_variables/normal/__init__.py
+-rw-rw-rw-   0        0        0     3594 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/objects/random_variables/normal/random_variable.py
+-rw-rw-rw-   0        0        0     9224 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/objects/random_variables/random_variable.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:25.784771 pm4py-2.7.9.4/pm4py/objects/random_variables/uniform/
+-rw-rw-rw-   0        0        0      802 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/objects/random_variables/uniform/__init__.py
+-rw-rw-rw-   0        0        0     3588 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/objects/random_variables/uniform/random_variable.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:25.800393 pm4py-2.7.9.4/pm4py/objects/stochastic_petri/
+-rw-rw-rw-   0        0        0      988 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/objects/stochastic_petri/__init__.py
+-rw-rw-rw-   0        0        0    12887 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/objects/stochastic_petri/ctmc.py
+-rw-rw-rw-   0        0        0     4714 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/objects/stochastic_petri/tangible_reachability.py
+-rw-rw-rw-   0        0        0     1616 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/objects/stochastic_petri/utils.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:25.800393 pm4py-2.7.9.4/pm4py/objects/transition_system/
+-rw-rw-rw-   0        0        0      803 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/objects/transition_system/__init__.py
+-rw-rw-rw-   0        0        0      825 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/objects/transition_system/constants.py
+-rw-rw-rw-   0        0        0     3958 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/objects/transition_system/obj.py
+-rw-rw-rw-   0        0        0     3625 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/objects/transition_system/utils.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:25.800393 pm4py-2.7.9.4/pm4py/objects/trie/
+-rw-rw-rw-   0        0        0      770 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/objects/trie/__init__.py
+-rw-rw-rw-   0        0        0     1911 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/objects/trie/obj.py
+-rw-rw-rw-   0        0        0    23143 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/ocel.py
+-rw-rw-rw-   0        0        0    14594 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/org.py
+-rw-rw-rw-   0        0        0     3805 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/privacy.py
+-rw-rw-rw-   0        0        0    15303 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/read.py
+-rw-rw-rw-   0        0        0     4578 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/sim.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:25.816012 pm4py-2.7.9.4/pm4py/statistics/
+-rw-rw-rw-   0        0        0      899 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/statistics/__init__.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:25.816012 pm4py-2.7.9.4/pm4py/statistics/attributes/
+-rw-rw-rw-   0        0        0      795 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/statistics/attributes/__init__.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:25.816012 pm4py-2.7.9.4/pm4py/statistics/attributes/common/
+-rw-rw-rw-   0        0        0      786 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/statistics/attributes/common/__init__.py
+-rw-rw-rw-   0        0        0     6611 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/statistics/attributes/common/get.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:25.816012 pm4py-2.7.9.4/pm4py/statistics/attributes/log/
+-rw-rw-rw-   0        0        0      791 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/statistics/attributes/log/__init__.py
+-rw-rw-rw-   0        0        0    13311 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/statistics/attributes/log/get.py
+-rw-rw-rw-   0        0        0     6905 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/statistics/attributes/log/select.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:25.831634 pm4py-2.7.9.4/pm4py/statistics/attributes/pandas/
+-rw-rw-rw-   0        0        0      786 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/statistics/attributes/pandas/__init__.py
+-rw-rw-rw-   0        0        0     9777 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/statistics/attributes/pandas/get.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:25.831634 pm4py-2.7.9.4/pm4py/statistics/concurrent_activities/
+-rw-rw-rw-   0        0        0      798 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/statistics/concurrent_activities/__init__.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:25.831634 pm4py-2.7.9.4/pm4py/statistics/concurrent_activities/log/
+-rw-rw-rw-   0        0        0      794 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/statistics/concurrent_activities/log/__init__.py
+-rw-rw-rw-   0        0        0     4081 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/statistics/concurrent_activities/log/get.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:25.831634 pm4py-2.7.9.4/pm4py/statistics/concurrent_activities/pandas/
+-rw-rw-rw-   0        0        0      797 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/statistics/concurrent_activities/pandas/__init__.py
+-rw-rw-rw-   0        0        0     3686 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/statistics/concurrent_activities/pandas/get.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:25.848308 pm4py-2.7.9.4/pm4py/statistics/end_activities/
+-rw-rw-rw-   0        0        0      799 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/statistics/end_activities/__init__.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:25.853816 pm4py-2.7.9.4/pm4py/statistics/end_activities/common/
+-rw-rw-rw-   0        0        0      790 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/statistics/end_activities/common/__init__.py
+-rw-rw-rw-   0        0        0     1791 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/statistics/end_activities/common/get.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:25.853816 pm4py-2.7.9.4/pm4py/statistics/end_activities/log/
+-rw-rw-rw-   0        0        0      787 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/statistics/end_activities/log/__init__.py
+-rw-rw-rw-   0        0        0     2746 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/statistics/end_activities/log/get.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:25.853816 pm4py-2.7.9.4/pm4py/statistics/end_activities/pandas/
+-rw-rw-rw-   0        0        0      790 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/statistics/end_activities/pandas/__init__.py
+-rw-rw-rw-   0        0        0     2665 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/statistics/end_activities/pandas/get.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:25.853816 pm4py-2.7.9.4/pm4py/statistics/eventually_follows/
+-rw-rw-rw-   0        0        0      801 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/statistics/eventually_follows/__init__.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:25.853816 pm4py-2.7.9.4/pm4py/statistics/eventually_follows/log/
+-rw-rw-rw-   0        0        0      791 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/statistics/eventually_follows/log/__init__.py
+-rw-rw-rw-   0        0        0     3015 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/statistics/eventually_follows/log/get.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:25.853816 pm4py-2.7.9.4/pm4py/statistics/eventually_follows/pandas/
+-rw-rw-rw-   0        0        0      794 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/statistics/eventually_follows/pandas/__init__.py
+-rw-rw-rw-   0        0        0     2879 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/statistics/eventually_follows/pandas/get.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:25.869446 pm4py-2.7.9.4/pm4py/statistics/eventually_follows/uvcl/
+-rw-rw-rw-   0        0        0      792 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/statistics/eventually_follows/uvcl/__init__.py
+-rw-rw-rw-   0        0        0     1936 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/statistics/eventually_follows/uvcl/get.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:25.869446 pm4py-2.7.9.4/pm4py/statistics/ocel/
+-rw-rw-rw-   0        0        0      734 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/statistics/ocel/__init__.py
+-rw-rw-rw-   0        0        0     3670 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/statistics/ocel/act_ot_dependent.py
+-rw-rw-rw-   0        0        0     5684 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/statistics/ocel/act_utils.py
+-rw-rw-rw-   0        0        0     9710 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/statistics/ocel/edge_metrics.py
+-rw-rw-rw-   0        0        0     2361 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/statistics/ocel/objects_ot_count.py
+-rw-rw-rw-   0        0        0     2395 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/statistics/ocel/ot_activities.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:25.885064 pm4py-2.7.9.4/pm4py/statistics/overlap/
+-rw-rw-rw-   0        0        0      957 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/statistics/overlap/__init__.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:25.885064 pm4py-2.7.9.4/pm4py/statistics/overlap/cases/
+-rw-rw-rw-   0        0        0      790 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/statistics/overlap/cases/__init__.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:25.885064 pm4py-2.7.9.4/pm4py/statistics/overlap/cases/log/
+-rw-rw-rw-   0        0        0      786 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/statistics/overlap/cases/log/__init__.py
+-rw-rw-rw-   0        0        0     2713 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/statistics/overlap/cases/log/get.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:25.885064 pm4py-2.7.9.4/pm4py/statistics/overlap/cases/pandas/
+-rw-rw-rw-   0        0        0      789 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/statistics/overlap/cases/pandas/__init__.py
+-rw-rw-rw-   0        0        0     3028 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/statistics/overlap/cases/pandas/get.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:25.885064 pm4py-2.7.9.4/pm4py/statistics/overlap/interval_events/
+-rw-rw-rw-   0        0        0      800 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/statistics/overlap/interval_events/__init__.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:25.885064 pm4py-2.7.9.4/pm4py/statistics/overlap/interval_events/log/
+-rw-rw-rw-   0        0        0      796 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/statistics/overlap/interval_events/log/__init__.py
+-rw-rw-rw-   0        0        0     2767 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/statistics/overlap/interval_events/log/get.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:25.900685 pm4py-2.7.9.4/pm4py/statistics/overlap/interval_events/pandas/
+-rw-rw-rw-   0        0        0      799 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/statistics/overlap/interval_events/pandas/__init__.py
+-rw-rw-rw-   0        0        0     2570 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/statistics/overlap/interval_events/pandas/get.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:25.900685 pm4py-2.7.9.4/pm4py/statistics/overlap/utils/
+-rw-rw-rw-   0        0        0      786 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/statistics/overlap/utils/__init__.py
+-rw-rw-rw-   0        0        0     1986 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/statistics/overlap/utils/compute.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:25.900685 pm4py-2.7.9.4/pm4py/statistics/passed_time/
+-rw-rw-rw-   0        0        0      790 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/statistics/passed_time/__init__.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:25.916306 pm4py-2.7.9.4/pm4py/statistics/passed_time/log/
+-rw-rw-rw-   0        0        0      800 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/statistics/passed_time/log/__init__.py
+-rw-rw-rw-   0        0        0     1781 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/statistics/passed_time/log/algorithm.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:25.916306 pm4py-2.7.9.4/pm4py/statistics/passed_time/log/variants/
+-rw-rw-rw-   0        0        0      808 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/statistics/passed_time/log/variants/__init__.py
+-rw-rw-rw-   0        0        0     2387 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/statistics/passed_time/log/variants/post.py
+-rw-rw-rw-   0        0        0     2369 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/statistics/passed_time/log/variants/pre.py
+-rw-rw-rw-   0        0        0     3050 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/statistics/passed_time/log/variants/prepost.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:25.916306 pm4py-2.7.9.4/pm4py/statistics/passed_time/pandas/
+-rw-rw-rw-   0        0        0      803 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/statistics/passed_time/pandas/__init__.py
+-rw-rw-rw-   0        0        0     1768 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/statistics/passed_time/pandas/algorithm.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:25.931927 pm4py-2.7.9.4/pm4py/statistics/passed_time/pandas/variants/
+-rw-rw-rw-   0        0        0      811 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/statistics/passed_time/pandas/variants/__init__.py
+-rw-rw-rw-   0        0        0     4131 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/statistics/passed_time/pandas/variants/post.py
+-rw-rw-rw-   0        0        0     4235 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/statistics/passed_time/pandas/variants/pre.py
+-rw-rw-rw-   0        0        0     4916 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/statistics/passed_time/pandas/variants/prepost.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:25.931927 pm4py-2.7.9.4/pm4py/statistics/rework/
+-rw-rw-rw-   0        0        0      783 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/statistics/rework/__init__.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:25.931927 pm4py-2.7.9.4/pm4py/statistics/rework/cases/
+-rw-rw-rw-   0        0        0      789 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/statistics/rework/cases/__init__.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:25.949578 pm4py-2.7.9.4/pm4py/statistics/rework/cases/log/
+-rw-rw-rw-   0        0        0      785 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/statistics/rework/cases/log/__init__.py
+-rw-rw-rw-   0        0        0     2597 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/statistics/rework/cases/log/get.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:25.954083 pm4py-2.7.9.4/pm4py/statistics/rework/cases/pandas/
+-rw-rw-rw-   0        0        0      788 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/statistics/rework/cases/pandas/__init__.py
+-rw-rw-rw-   0        0        0     2542 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/statistics/rework/cases/pandas/get.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:25.954083 pm4py-2.7.9.4/pm4py/statistics/rework/log/
+-rw-rw-rw-   0        0        0      779 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/statistics/rework/log/__init__.py
+-rw-rw-rw-   0        0        0     2265 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/statistics/rework/log/get.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:25.954083 pm4py-2.7.9.4/pm4py/statistics/rework/pandas/
+-rw-rw-rw-   0        0        0      782 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/statistics/rework/pandas/__init__.py
+-rw-rw-rw-   0        0        0     2378 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/statistics/rework/pandas/get.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:25.954083 pm4py-2.7.9.4/pm4py/statistics/service_time/
+-rw-rw-rw-   0        0        0      789 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/statistics/service_time/__init__.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:25.954083 pm4py-2.7.9.4/pm4py/statistics/service_time/log/
+-rw-rw-rw-   0        0        0      785 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/statistics/service_time/log/__init__.py
+-rw-rw-rw-   0        0        0     5453 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/statistics/service_time/log/get.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:25.969711 pm4py-2.7.9.4/pm4py/statistics/service_time/pandas/
+-rw-rw-rw-   0        0        0      788 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/statistics/service_time/pandas/__init__.py
+-rw-rw-rw-   0        0        0     4930 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/statistics/service_time/pandas/get.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:25.969711 pm4py-2.7.9.4/pm4py/statistics/sojourn_time/
+-rw-rw-rw-   0        0        0      779 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/statistics/sojourn_time/__init__.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:25.969711 pm4py-2.7.9.4/pm4py/statistics/start_activities/
+-rw-rw-rw-   0        0        0      801 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/statistics/start_activities/__init__.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:25.969711 pm4py-2.7.9.4/pm4py/statistics/start_activities/common/
+-rw-rw-rw-   0        0        0      792 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/statistics/start_activities/common/__init__.py
+-rw-rw-rw-   0        0        0     1813 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/statistics/start_activities/common/get.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:25.969711 pm4py-2.7.9.4/pm4py/statistics/start_activities/log/
+-rw-rw-rw-   0        0        0      789 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/statistics/start_activities/log/__init__.py
+-rw-rw-rw-   0        0        0     2769 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/statistics/start_activities/log/get.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:25.985822 pm4py-2.7.9.4/pm4py/statistics/start_activities/pandas/
+-rw-rw-rw-   0        0        0      792 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/statistics/start_activities/pandas/__init__.py
+-rw-rw-rw-   0        0        0     2623 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/statistics/start_activities/pandas/get.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:25.985822 pm4py-2.7.9.4/pm4py/statistics/traces/
+-rw-rw-rw-   0        0        0      791 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/statistics/traces/__init__.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:25.985822 pm4py-2.7.9.4/pm4py/statistics/traces/cycle_time/
+-rw-rw-rw-   0        0        0      800 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/statistics/traces/cycle_time/__init__.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:25.985822 pm4py-2.7.9.4/pm4py/statistics/traces/cycle_time/log/
+-rw-rw-rw-   0        0        0      790 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/statistics/traces/cycle_time/log/__init__.py
+-rw-rw-rw-   0        0        0     3191 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/statistics/traces/cycle_time/log/get.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:25.985822 pm4py-2.7.9.4/pm4py/statistics/traces/cycle_time/pandas/
+-rw-rw-rw-   0        0        0      793 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/statistics/traces/cycle_time/pandas/__init__.py
+-rw-rw-rw-   0        0        0     3255 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/statistics/traces/cycle_time/pandas/get.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:26.001432 pm4py-2.7.9.4/pm4py/statistics/traces/cycle_time/util/
+-rw-rw-rw-   0        0        0      795 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/statistics/traces/cycle_time/util/__init__.py
+-rw-rw-rw-   0        0        0     2385 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/statistics/traces/cycle_time/util/compute.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:26.001432 pm4py-2.7.9.4/pm4py/statistics/traces/generic/
+-rw-rw-rw-   0        0        0      799 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/statistics/traces/generic/__init__.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:26.001432 pm4py-2.7.9.4/pm4py/statistics/traces/generic/common/
+-rw-rw-rw-   0        0        0      800 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/statistics/traces/generic/common/__init__.py
+-rw-rw-rw-   0        0        0     2969 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/statistics/traces/generic/common/case_duration.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:26.001432 pm4py-2.7.9.4/pm4py/statistics/traces/generic/log/
+-rw-rw-rw-   0        0        0      799 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/statistics/traces/generic/log/__init__.py
+-rw-rw-rw-   0        0        0     5237 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/statistics/traces/generic/log/case_arrival.py
+-rw-rw-rw-   0        0        0    13221 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/statistics/traces/generic/log/case_statistics.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:26.017053 pm4py-2.7.9.4/pm4py/statistics/traces/generic/pandas/
+-rw-rw-rw-   0        0        0      799 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/statistics/traces/generic/pandas/__init__.py
+-rw-rw-rw-   0        0        0     4223 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/statistics/traces/generic/pandas/case_arrival.py
+-rw-rw-rw-   0        0        0    16954 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/statistics/traces/generic/pandas/case_statistics.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:26.017053 pm4py-2.7.9.4/pm4py/statistics/util/
+-rw-rw-rw-   0        0        0      974 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/statistics/util/__init__.py
+-rw-rw-rw-   0        0        0     2382 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/statistics/util/times_bipartite_matching.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:26.017053 pm4py-2.7.9.4/pm4py/statistics/variants/
+-rw-rw-rw-   0        0        0      785 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/statistics/variants/__init__.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:26.017053 pm4py-2.7.9.4/pm4py/statistics/variants/log/
+-rw-rw-rw-   0        0        0      781 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/statistics/variants/log/__init__.py
+-rw-rw-rw-   0        0        0     7359 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/statistics/variants/log/get.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:26.032674 pm4py-2.7.9.4/pm4py/statistics/variants/pandas/
+-rw-rw-rw-   0        0        0      784 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/statistics/variants/pandas/__init__.py
+-rw-rw-rw-   0        0        0     2254 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/statistics/variants/pandas/get.py
+-rw-rw-rw-   0        0        0    39292 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/stats.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:26.032674 pm4py-2.7.9.4/pm4py/streaming/
+-rw-rw-rw-   0        0        0      804 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/streaming/__init__.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:26.032674 pm4py-2.7.9.4/pm4py/streaming/algo/
+-rw-rw-rw-   0        0        0      800 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/streaming/algo/__init__.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:26.032674 pm4py-2.7.9.4/pm4py/streaming/algo/conformance/
+-rw-rw-rw-   0        0        0      806 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/streaming/algo/conformance/__init__.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:26.048297 pm4py-2.7.9.4/pm4py/streaming/algo/conformance/footprints/
+-rw-rw-rw-   0        0        0      811 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/streaming/algo/conformance/footprints/__init__.py
+-rw-rw-rw-   0        0        0     1515 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/streaming/algo/conformance/footprints/algorithm.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:26.048297 pm4py-2.7.9.4/pm4py/streaming/algo/conformance/footprints/variants/
+-rw-rw-rw-   0        0        0      808 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/streaming/algo/conformance/footprints/variants/__init__.py
+-rw-rw-rw-   0        0        0    11003 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/streaming/algo/conformance/footprints/variants/classic.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:26.054303 pm4py-2.7.9.4/pm4py/streaming/algo/conformance/tbr/
+-rw-rw-rw-   0        0        0      804 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/streaming/algo/conformance/tbr/__init__.py
+-rw-rw-rw-   0        0        0     1523 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/streaming/algo/conformance/tbr/algorithm.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:26.054303 pm4py-2.7.9.4/pm4py/streaming/algo/conformance/tbr/variants/
+-rw-rw-rw-   0        0        0      801 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/streaming/algo/conformance/tbr/variants/__init__.py
+-rw-rw-rw-   0        0        0    17271 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/streaming/algo/conformance/tbr/variants/classic.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:26.054303 pm4py-2.7.9.4/pm4py/streaming/algo/conformance/temporal/
+-rw-rw-rw-   0        0        0      809 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/streaming/algo/conformance/temporal/__init__.py
+-rw-rw-rw-   0        0        0     2135 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/streaming/algo/conformance/temporal/algorithm.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:26.069930 pm4py-2.7.9.4/pm4py/streaming/algo/conformance/temporal/variants/
+-rw-rw-rw-   0        0        0      806 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/streaming/algo/conformance/temporal/variants/__init__.py
+-rw-rw-rw-   0        0        0     9602 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/streaming/algo/conformance/temporal/variants/classic.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:26.069930 pm4py-2.7.9.4/pm4py/streaming/algo/discovery/
+-rw-rw-rw-   0        0        0      782 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/streaming/algo/discovery/__init__.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:26.069930 pm4py-2.7.9.4/pm4py/streaming/algo/discovery/dfg/
+-rw-rw-rw-   0        0        0      802 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/streaming/algo/discovery/dfg/__init__.py
+-rw-rw-rw-   0        0        0     1411 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/streaming/algo/discovery/dfg/algorithm.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:26.085556 pm4py-2.7.9.4/pm4py/streaming/algo/discovery/dfg/variants/
+-rw-rw-rw-   0        0        0      801 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/streaming/algo/discovery/dfg/variants/__init__.py
+-rw-rw-rw-   0        0        0     7371 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/streaming/algo/discovery/dfg/variants/frequency.py
+-rw-rw-rw-   0        0        0     1476 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/streaming/algo/interface.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:26.085556 pm4py-2.7.9.4/pm4py/streaming/conversion/
+-rw-rw-rw-   0        0        0     1468 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/streaming/conversion/__init__.py
+-rw-rw-rw-   0        0        0     4925 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/streaming/conversion/from_pandas.py
+-rw-rw-rw-   0        0        0     5211 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/streaming/conversion/ocel_flatts_distributor.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:26.085556 pm4py-2.7.9.4/pm4py/streaming/importer/
+-rw-rw-rw-   0        0        0      885 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/streaming/importer/__init__.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:26.101173 pm4py-2.7.9.4/pm4py/streaming/importer/csv/
+-rw-rw-rw-   0        0        0      795 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/streaming/importer/csv/__init__.py
+-rw-rw-rw-   0        0        0     1488 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/streaming/importer/csv/importer.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:26.101173 pm4py-2.7.9.4/pm4py/streaming/importer/csv/variants/
+-rw-rw-rw-   0        0        0      802 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/streaming/importer/csv/variants/__init__.py
+-rw-rw-rw-   0        0        0     3406 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/streaming/importer/csv/variants/csv_event_stream.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:26.101173 pm4py-2.7.9.4/pm4py/streaming/importer/xes/
+-rw-rw-rw-   0        0        0      795 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/streaming/importer/xes/__init__.py
+-rw-rw-rw-   0        0        0     1523 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/streaming/importer/xes/importer.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:26.116794 pm4py-2.7.9.4/pm4py/streaming/importer/xes/variants/
+-rw-rw-rw-   0        0        0      820 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/streaming/importer/xes/variants/__init__.py
+-rw-rw-rw-   0        0        0     9461 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/streaming/importer/xes/variants/xes_event_stream.py
+-rw-rw-rw-   0        0        0     9317 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/streaming/importer/xes/variants/xes_trace_stream.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:26.116794 pm4py-2.7.9.4/pm4py/streaming/stream/
+-rw-rw-rw-   0        0        0      807 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/streaming/stream/__init__.py
+-rw-rw-rw-   0        0        0     3109 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/streaming/stream/live_event_stream.py
+-rw-rw-rw-   0        0        0     3109 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/streaming/stream/live_trace_stream.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:26.132415 pm4py-2.7.9.4/pm4py/streaming/util/
+-rw-rw-rw-   0        0        0      819 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/streaming/util/__init__.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:26.132415 pm4py-2.7.9.4/pm4py/streaming/util/dictio/
+-rw-rw-rw-   0        0        0      795 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/streaming/util/dictio/__init__.py
+-rw-rw-rw-   0        0        0     1461 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/streaming/util/dictio/generator.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:26.154543 pm4py-2.7.9.4/pm4py/streaming/util/dictio/versions/
+-rw-rw-rw-   0        0        0      805 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/streaming/util/dictio/versions/__init__.py
+-rw-rw-rw-   0        0        0      941 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/streaming/util/dictio/versions/classic.py
+-rw-rw-rw-   0        0        0     3540 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/streaming/util/dictio/versions/redis.py
+-rw-rw-rw-   0        0        0     1949 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/streaming/util/dictio/versions/thread_safe.py
+-rw-rw-rw-   0        0        0     1039 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/streaming/util/event_stream_printer.py
+-rw-rw-rw-   0        0        0     1180 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/streaming/util/live_to_static_stream.py
+-rw-rw-rw-   0        0        0     1039 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/streaming/util/trace_stream_printer.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:26.185794 pm4py-2.7.9.4/pm4py/util/
+-rw-rw-rw-   0        0        0      928 2024-01-17 08:28:40.000000 pm4py-2.7.9.4/pm4py/util/__init__.py
+-rw-rw-rw-   0        0        0     5056 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/util/business_hours.py
+-rw-rw-rw-   0        0        0     2225 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/util/colors.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:26.201413 pm4py-2.7.9.4/pm4py/util/compression/
+-rw-rw-rw-   0        0        0      781 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/util/compression/__init__.py
+-rw-rw-rw-   0        0        0     1314 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/util/compression/dtypes.py
+-rw-rw-rw-   0        0        0    11522 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/util/compression/util.py
+-rw-rw-rw-   0        0        0     7079 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/util/constants.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:26.201413 pm4py-2.7.9.4/pm4py/util/dt_parsing/
+-rw-rw-rw-   0        0        0      786 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/util/dt_parsing/__init__.py
+-rw-rw-rw-   0        0        0     2682 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/util/dt_parsing/parser.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:26.201413 pm4py-2.7.9.4/pm4py/util/dt_parsing/variants/
+-rw-rw-rw-   0        0        0      734 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/util/dt_parsing/variants/__init__.py
+-rw-rw-rw-   0        0        0     1029 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/util/dt_parsing/variants/cs8601.py
+-rw-rw-rw-   0        0        0     1470 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/util/dt_parsing/variants/dummy.py
+-rw-rw-rw-   0        0        0     1916 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/util/dt_parsing/variants/strpfromiso.py
+-rw-rw-rw-   0        0        0     1564 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/util/exec_utils.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:26.217036 pm4py-2.7.9.4/pm4py/util/lp/
+-rw-rw-rw-   0        0        0      784 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/util/lp/__init__.py
+-rw-rw-rw-   0        0        0     5457 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/util/lp/solver.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:26.217036 pm4py-2.7.9.4/pm4py/util/lp/util/
+-rw-rw-rw-   0        0        0      734 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/util/lp/util/__init__.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:26.232657 pm4py-2.7.9.4/pm4py/util/lp/variants/
+-rw-rw-rw-   0        0        0      943 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/util/lp/variants/__init__.py
+-rw-rw-rw-   0        0        0     3639 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/util/lp/variants/cvxopt_solver.py
+-rw-rw-rw-   0        0        0     3420 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/util/lp/variants/cvxopt_solver_custom_align.py
+-rw-rw-rw-   0        0        0     3059 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/util/lp/variants/cvxopt_solver_custom_align_arm.py
+-rw-rw-rw-   0        0        0     3937 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/util/lp/variants/cvxopt_solver_custom_align_ilp.py
+-rw-rw-rw-   0        0        0     5153 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/util/lp/variants/ortools_solver.py
+-rw-rw-rw-   0        0        0     6293 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/util/lp/variants/pulp_solver.py
+-rw-rw-rw-   0        0        0     1853 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/util/lp/variants/scipy_solver.py
+-rw-rw-rw-   0        0        0    10037 2024-01-18 11:43:23.000000 pm4py-2.7.9.4/pm4py/util/nx_utils.py
+-rw-rw-rw-   0        0        0    13899 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/util/pandas_utils.py
+-rw-rw-rw-   0        0        0     1494 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/util/points_subset.py
+-rw-rw-rw-   0        0        0     1602 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/util/regex.py
+-rw-rw-rw-   0        0        0     3663 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/util/string_distance.py
+-rw-rw-rw-   0        0        0     1095 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/util/typing.py
+-rw-rw-rw-   0        0        0     2261 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/util/variants_util.py
+-rw-rw-rw-   0        0        0     6027 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/util/vis_utils.py
+-rw-rw-rw-   0        0        0     1614 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/util/xes_constants.py
+-rw-rw-rw-   0        0        0    25437 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/utils.py
+-rw-rw-rw-   0        0        0    69901 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/vis.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:26.232657 pm4py-2.7.9.4/pm4py/visualization/
+-rw-rw-rw-   0        0        0     1869 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/visualization/__init__.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:26.232657 pm4py-2.7.9.4/pm4py/visualization/align_table/
+-rw-rw-rw-   0        0        0      790 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/visualization/align_table/__init__.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:26.249019 pm4py-2.7.9.4/pm4py/visualization/align_table/variants/
+-rw-rw-rw-   0        0        0      796 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/visualization/align_table/variants/__init__.py
+-rw-rw-rw-   0        0        0     3863 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/visualization/align_table/variants/classic.py
+-rw-rw-rw-   0        0        0     2968 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/visualization/align_table/visualizer.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:26.254527 pm4py-2.7.9.4/pm4py/visualization/bpmn/
+-rw-rw-rw-   0        0        0      793 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/visualization/bpmn/__init__.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:26.254527 pm4py-2.7.9.4/pm4py/visualization/bpmn/variants/
+-rw-rw-rw-   0        0        0      789 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/visualization/bpmn/variants/__init__.py
+-rw-rw-rw-   0        0        0     3654 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/visualization/bpmn/variants/classic.py
+-rw-rw-rw-   0        0        0     2583 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/visualization/bpmn/visualizer.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:26.270153 pm4py-2.7.9.4/pm4py/visualization/common/
+-rw-rw-rw-   0        0        0      817 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/visualization/common/__init__.py
+-rw-rw-rw-   0        0        0     1160 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/visualization/common/dot_util.py
+-rw-rw-rw-   0        0        0     3058 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/visualization/common/gview.py
+-rw-rw-rw-   0        0        0     3394 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/visualization/common/html.py
+-rw-rw-rw-   0        0        0     1531 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/visualization/common/save.py
+-rw-rw-rw-   0        0        0     2526 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/visualization/common/svg_pos_parser.py
+-rw-rw-rw-   0        0        0      879 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/visualization/common/utils.py
+-rw-rw-rw-   0        0        0     1540 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/visualization/common/visualizer.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:26.270153 pm4py-2.7.9.4/pm4py/visualization/decisiontree/
+-rw-rw-rw-   0        0        0     1008 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/visualization/decisiontree/__init__.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:26.270153 pm4py-2.7.9.4/pm4py/visualization/decisiontree/util/
+-rw-rw-rw-   0        0        0      734 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/visualization/decisiontree/util/__init__.py
+-rw-rw-rw-   0        0        0     2621 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/visualization/decisiontree/util/dt_to_string.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:26.285778 pm4py-2.7.9.4/pm4py/visualization/decisiontree/variants/
+-rw-rw-rw-   0        0        0      797 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/visualization/decisiontree/variants/__init__.py
+-rw-rw-rw-   0        0        0     2231 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/visualization/decisiontree/variants/classic.py
+-rw-rw-rw-   0        0        0     2840 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/visualization/decisiontree/visualizer.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:26.285778 pm4py-2.7.9.4/pm4py/visualization/dfg/
+-rw-rw-rw-   0        0        0      800 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/visualization/dfg/__init__.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:26.285778 pm4py-2.7.9.4/pm4py/visualization/dfg/util/
+-rw-rw-rw-   0        0        0      787 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/visualization/dfg/util/__init__.py
+-rw-rw-rw-   0        0        0     8994 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/visualization/dfg/util/dfg_gviz.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:26.301397 pm4py-2.7.9.4/pm4py/visualization/dfg/variants/
+-rw-rw-rw-   0        0        0      803 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/visualization/dfg/variants/__init__.py
+-rw-rw-rw-   0        0        0     5409 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/visualization/dfg/variants/cost.py
+-rw-rw-rw-   0        0        0     5157 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/visualization/dfg/variants/frequency.py
+-rw-rw-rw-   0        0        0     5580 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/visualization/dfg/variants/performance.py
+-rw-rw-rw-   0        0        0    12854 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/visualization/dfg/variants/timeline.py
+-rw-rw-rw-   0        0        0     3196 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/visualization/dfg/visualizer.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:26.301397 pm4py-2.7.9.4/pm4py/visualization/dotted_chart/
+-rw-rw-rw-   0        0        0      801 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/visualization/dotted_chart/__init__.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:26.301397 pm4py-2.7.9.4/pm4py/visualization/dotted_chart/variants/
+-rw-rw-rw-   0        0        0      797 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/visualization/dotted_chart/variants/__init__.py
+-rw-rw-rw-   0        0        0     9236 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/visualization/dotted_chart/variants/classic.py
+-rw-rw-rw-   0        0        0     3819 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/visualization/dotted_chart/visualizer.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:26.317019 pm4py-2.7.9.4/pm4py/visualization/footprints/
+-rw-rw-rw-   0        0        0      799 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/visualization/footprints/__init__.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:26.317019 pm4py-2.7.9.4/pm4py/visualization/footprints/variants/
+-rw-rw-rw-   0        0        0      828 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/visualization/footprints/variants/__init__.py
+-rw-rw-rw-   0        0        0     3842 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/visualization/footprints/variants/comparison.py
+-rw-rw-rw-   0        0        0     4374 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/visualization/footprints/variants/comparison_symmetric.py
+-rw-rw-rw-   0        0        0     3280 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/visualization/footprints/variants/single.py
+-rw-rw-rw-   0        0        0     3120 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/visualization/footprints/visualizer.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:26.317019 pm4py-2.7.9.4/pm4py/visualization/graphs/
+-rw-rw-rw-   0        0        0      801 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/visualization/graphs/__init__.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:26.332638 pm4py-2.7.9.4/pm4py/visualization/graphs/util/
+-rw-rw-rw-   0        0        0      786 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/visualization/graphs/util/__init__.py
+-rw-rw-rw-   0        0        0     2849 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/visualization/graphs/util/common.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:26.332638 pm4py-2.7.9.4/pm4py/visualization/graphs/variants/
+-rw-rw-rw-   0        0        0      817 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/visualization/graphs/variants/__init__.py
+-rw-rw-rw-   0        0        0     4541 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/visualization/graphs/variants/attributes.py
+-rw-rw-rw-   0        0        0     2763 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/visualization/graphs/variants/barplot.py
+-rw-rw-rw-   0        0        0     4542 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/visualization/graphs/variants/cases.py
+-rw-rw-rw-   0        0        0     4587 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/visualization/graphs/variants/dates.py
+-rw-rw-rw-   0        0        0     3859 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/visualization/graphs/visualizer.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:26.332638 pm4py-2.7.9.4/pm4py/visualization/heuristics_net/
+-rw-rw-rw-   0        0        0      803 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/visualization/heuristics_net/__init__.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:26.348260 pm4py-2.7.9.4/pm4py/visualization/heuristics_net/variants/
+-rw-rw-rw-   0        0        0      805 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/visualization/heuristics_net/variants/__init__.py
+-rw-rw-rw-   0        0        0    13357 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/visualization/heuristics_net/variants/pydotplus_vis.py
+-rw-rw-rw-   0        0        0     4471 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/visualization/heuristics_net/visualizer.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:26.354766 pm4py-2.7.9.4/pm4py/visualization/network_analysis/
+-rw-rw-rw-   0        0        0      805 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/visualization/network_analysis/__init__.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:26.354766 pm4py-2.7.9.4/pm4py/visualization/network_analysis/variants/
+-rw-rw-rw-   0        0        0      816 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/visualization/network_analysis/variants/__init__.py
+-rw-rw-rw-   0        0        0     4975 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/visualization/network_analysis/variants/frequency.py
+-rw-rw-rw-   0        0        0     6154 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/visualization/network_analysis/variants/performance.py
+-rw-rw-rw-   0        0        0     2496 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/visualization/network_analysis/visualizer.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:26.354766 pm4py-2.7.9.4/pm4py/visualization/networkx/
+-rw-rw-rw-   0        0        0      734 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/visualization/networkx/__init__.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:26.354766 pm4py-2.7.9.4/pm4py/visualization/networkx/variants/
+-rw-rw-rw-   0        0        0      734 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/visualization/networkx/variants/__init__.py
+-rw-rw-rw-   0        0        0     3990 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/visualization/networkx/variants/digraph.py
+-rw-rw-rw-   0        0        0     2362 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/visualization/networkx/visualizer.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:26.354766 pm4py-2.7.9.4/pm4py/visualization/ocel/
+-rw-rw-rw-   0        0        0      813 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/visualization/ocel/__init__.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:26.370399 pm4py-2.7.9.4/pm4py/visualization/ocel/eve_to_obj_types/
+-rw-rw-rw-   0        0        0      734 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/visualization/ocel/eve_to_obj_types/__init__.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:26.370399 pm4py-2.7.9.4/pm4py/visualization/ocel/eve_to_obj_types/variants/
+-rw-rw-rw-   0        0        0      734 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/visualization/ocel/eve_to_obj_types/variants/__init__.py
+-rw-rw-rw-   0        0        0     3613 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/visualization/ocel/eve_to_obj_types/variants/graphviz.py
+-rw-rw-rw-   0        0        0     2724 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/visualization/ocel/eve_to_obj_types/visualizer.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:26.370399 pm4py-2.7.9.4/pm4py/visualization/ocel/interleavings/
+-rw-rw-rw-   0        0        0      807 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/visualization/ocel/interleavings/__init__.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:26.386925 pm4py-2.7.9.4/pm4py/visualization/ocel/interleavings/variants/
+-rw-rw-rw-   0        0        0      804 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/visualization/ocel/interleavings/variants/__init__.py
+-rw-rw-rw-   0        0        0    15031 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/visualization/ocel/interleavings/variants/graphviz.py
+-rw-rw-rw-   0        0        0     2989 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/visualization/ocel/interleavings/visualizer.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:26.386925 pm4py-2.7.9.4/pm4py/visualization/ocel/object_graph/
+-rw-rw-rw-   0        0        0      734 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/visualization/ocel/object_graph/__init__.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:26.386925 pm4py-2.7.9.4/pm4py/visualization/ocel/object_graph/variants/
+-rw-rw-rw-   0        0        0      734 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/visualization/ocel/object_graph/variants/__init__.py
+-rw-rw-rw-   0        0        0     3447 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/visualization/ocel/object_graph/variants/graphviz.py
+-rw-rw-rw-   0        0        0     2556 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/visualization/ocel/object_graph/visualizer.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:26.386925 pm4py-2.7.9.4/pm4py/visualization/ocel/ocdfg/
+-rw-rw-rw-   0        0        0      799 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/visualization/ocel/ocdfg/__init__.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:26.402547 pm4py-2.7.9.4/pm4py/visualization/ocel/ocdfg/variants/
+-rw-rw-rw-   0        0        0      795 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/visualization/ocel/ocdfg/variants/__init__.py
+-rw-rw-rw-   0        0        0    12507 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/visualization/ocel/ocdfg/variants/classic.py
+-rw-rw-rw-   0        0        0     2454 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/visualization/ocel/ocdfg/visualizer.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:26.402547 pm4py-2.7.9.4/pm4py/visualization/ocel/ocpn/
+-rw-rw-rw-   0        0        0      798 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/visualization/ocel/ocpn/__init__.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:26.402547 pm4py-2.7.9.4/pm4py/visualization/ocel/ocpn/variants/
+-rw-rw-rw-   0        0        0      800 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/visualization/ocel/ocpn/variants/__init__.py
+-rw-rw-rw-   0        0        0     5941 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/visualization/ocel/ocpn/variants/wo_decoration.py
+-rw-rw-rw-   0        0        0     2601 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/visualization/ocel/ocpn/visualizer.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:26.402547 pm4py-2.7.9.4/pm4py/visualization/performance_spectrum/
+-rw-rw-rw-   0        0        0      809 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/visualization/performance_spectrum/__init__.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:26.418175 pm4py-2.7.9.4/pm4py/visualization/performance_spectrum/variants/
+-rw-rw-rw-   0        0        0      803 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/visualization/performance_spectrum/variants/__init__.py
+-rw-rw-rw-   0        0        0     7116 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/visualization/performance_spectrum/variants/neato.py
+-rw-rw-rw-   0        0        0     3244 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/visualization/performance_spectrum/visualizer.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:26.418175 pm4py-2.7.9.4/pm4py/visualization/petri_net/
+-rw-rw-rw-   0        0        0      812 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/visualization/petri_net/__init__.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:26.418175 pm4py-2.7.9.4/pm4py/visualization/petri_net/common/
+-rw-rw-rw-   0        0        0      794 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/visualization/petri_net/common/__init__.py
+-rw-rw-rw-   0        0        0     9446 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/visualization/petri_net/common/visualize.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:26.433803 pm4py-2.7.9.4/pm4py/visualization/petri_net/util/
+-rw-rw-rw-   0        0        0      847 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/visualization/petri_net/util/__init__.py
+-rw-rw-rw-   0        0        0     2935 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/visualization/petri_net/util/alignments_decoration.py
+-rw-rw-rw-   0        0        0     1121 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/visualization/petri_net/util/performance_map.py
+-rw-rw-rw-   0        0        0    11279 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/visualization/petri_net/util/vis_trans_shortest_paths.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:26.454918 pm4py-2.7.9.4/pm4py/visualization/petri_net/variants/
+-rw-rw-rw-   0        0        0      937 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/visualization/petri_net/variants/__init__.py
+-rw-rw-rw-   0        0        0     2044 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/visualization/petri_net/variants/alignments.py
+-rw-rw-rw-   0        0        0     4730 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/visualization/petri_net/variants/greedy_decoration_frequency.py
+-rw-rw-rw-   0        0        0     4837 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/visualization/petri_net/variants/greedy_decoration_performance.py
+-rw-rw-rw-   0        0        0     5670 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/visualization/petri_net/variants/token_decoration_frequency.py
+-rw-rw-rw-   0        0        0     5880 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/visualization/petri_net/variants/token_decoration_performance.py
+-rw-rw-rw-   0        0        0     2237 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/visualization/petri_net/variants/wo_decoration.py
+-rw-rw-rw-   0        0        0     3651 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/visualization/petri_net/visualizer.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:26.454918 pm4py-2.7.9.4/pm4py/visualization/powl/
+-rw-rw-rw-   0        0        0      795 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/visualization/powl/__init__.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:26.470545 pm4py-2.7.9.4/pm4py/visualization/powl/variants/
+-rw-rw-rw-   0        0        0      785 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/visualization/powl/variants/__init__.py
+-rw-rw-rw-   0        0        0     7745 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/visualization/powl/variants/basic.py
+-rw-rw-rw-   0        0        0      755 2024-01-02 13:29:21.000000 pm4py-2.7.9.4/pm4py/visualization/powl/variants/end.png
+-rw-rw-rw-   0        0        0    25337 2024-01-02 13:29:21.000000 pm4py-2.7.9.4/pm4py/visualization/powl/variants/loop.png
+-rw-rw-rw-   0        0        0    11069 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/visualization/powl/variants/net.py
+-rw-rw-rw-   0        0        0      922 2024-01-02 13:29:21.000000 pm4py-2.7.9.4/pm4py/visualization/powl/variants/play.png
+-rw-rw-rw-   0        0        0    78865 2024-01-02 13:29:21.000000 pm4py-2.7.9.4/pm4py/visualization/powl/variants/xor.png
+-rw-rw-rw-   0        0        0     2853 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/visualization/powl/visualizer.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:26.470545 pm4py-2.7.9.4/pm4py/visualization/process_tree/
+-rw-rw-rw-   0        0        0      801 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/visualization/process_tree/__init__.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:26.470545 pm4py-2.7.9.4/pm4py/visualization/process_tree/variants/
+-rw-rw-rw-   0        0        0      813 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/visualization/process_tree/variants/__init__.py
+-rw-rw-rw-   0        0        0     4873 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/visualization/process_tree/variants/frequency_annotation.py
+-rw-rw-rw-   0        0        0     4104 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/visualization/process_tree/variants/symbolic.py
+-rw-rw-rw-   0        0        0     4256 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/visualization/process_tree/variants/wo_decoration.py
+-rw-rw-rw-   0        0        0     3017 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/visualization/process_tree/visualizer.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:26.486166 pm4py-2.7.9.4/pm4py/visualization/sna/
+-rw-rw-rw-   0        0        0      792 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/visualization/sna/__init__.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:26.486166 pm4py-2.7.9.4/pm4py/visualization/sna/variants/
+-rw-rw-rw-   0        0        0      796 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/visualization/sna/variants/__init__.py
+-rw-rw-rw-   0        0        0     4180 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/visualization/sna/variants/networkx.py
+-rw-rw-rw-   0        0        0     5472 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/visualization/sna/variants/pyvis.py
+-rw-rw-rw-   0        0        0     2561 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/visualization/sna/visualizer.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:26.486166 pm4py-2.7.9.4/pm4py/visualization/transition_system/
+-rw-rw-rw-   0        0        0      812 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/visualization/transition_system/__init__.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:26.503298 pm4py-2.7.9.4/pm4py/visualization/transition_system/util/
+-rw-rw-rw-   0        0        0      809 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/visualization/transition_system/util/__init__.py
+-rw-rw-rw-   0        0        0     3315 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/visualization/transition_system/util/visualize_graphviz.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:26.504306 pm4py-2.7.9.4/pm4py/visualization/transition_system/variants/
+-rw-rw-rw-   0        0        0      822 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/visualization/transition_system/variants/__init__.py
+-rw-rw-rw-   0        0        0     3138 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/visualization/transition_system/variants/trans_frequency.py
+-rw-rw-rw-   0        0        0     1652 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/visualization/transition_system/variants/view_based.py
+-rw-rw-rw-   0        0        0     2703 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/visualization/transition_system/visualizer.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:26.504306 pm4py-2.7.9.4/pm4py/visualization/trie/
+-rw-rw-rw-   0        0        0      793 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/visualization/trie/__init__.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:26.504306 pm4py-2.7.9.4/pm4py/visualization/trie/variants/
+-rw-rw-rw-   0        0        0      789 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/visualization/trie/variants/__init__.py
+-rw-rw-rw-   0        0        0     2765 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/visualization/trie/variants/classic.py
+-rw-rw-rw-   0        0        0     2512 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/visualization/trie/visualizer.py
+-rw-rw-rw-   0        0        0    15531 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/pm4py/write.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:26.520942 pm4py-2.7.9.4/pm4py.egg-info/
+-rw-rw-rw-   0        0        0     3631 2024-01-29 06:14:21.000000 pm4py-2.7.9.4/pm4py.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0    66549 2024-01-29 06:14:22.000000 pm4py-2.7.9.4/pm4py.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-01-29 06:14:21.000000 pm4py-2.7.9.4/pm4py.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      144 2024-01-29 06:14:21.000000 pm4py-2.7.9.4/pm4py.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-01-29 06:14:21.000000 pm4py-2.7.9.4/pm4py.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-01-29 06:14:26.520942 pm4py-2.7.9.4/setup.cfg
+-rw-rw-rw-   0        0        0     1246 2024-01-17 08:27:48.000000 pm4py-2.7.9.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-01-29 06:14:26.520942 pm4py-2.7.9.4/tests/
+-rw-rw-rw-   0        0        0     4971 2023-11-09 06:59:42.000000 pm4py-2.7.9.4/tests/test_cli.py
```

### Comparing `pm4py-2.7.9.3/LICENSE` & `pm4py-2.7.9.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/PKG-INFO` & `pm4py-2.7.9.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: pm4py
-Version: 2.7.9.3
+Version: 2.7.9.4
 Summary: Process mining for Python
 Home-page: https://pm4py.fit.fraunhofer.de
 Author: Fraunhofer Institute for Applied Information Technology FIT
 Author-email: pm4py@fit.fraunhofer.de
 License: GPL 3.0
 Project-URL: Documentation, https://pm4py.fit.fraunhofer.de
 Project-URL: Source, https://github.com/pm4py/pm4py-source
 Project-URL: Tracker, https://github.com/pm4py/pm4py-source/issues
 License-File: LICENSE
-Requires-Dist: cvxopt; python_version < "3.12"
+Requires-Dist: cvxopt; python_version < "3.13"
 Requires-Dist: deprecation
 Requires-Dist: graphviz
 Requires-Dist: intervaltree
 Requires-Dist: lxml
 Requires-Dist: matplotlib
 Requires-Dist: networkx
 Requires-Dist: numpy
@@ -78,7 +78,8 @@
 pages = {100556},  
 year = {2023},  
 issn = {2665-9638},  
 doi = {https://doi.org/10.1016/j.simpa.2023.100556},  
 url = {https://www.sciencedirect.com/science/article/pii/S2665963823000933},  
 author = {Alessandro Berti and Sebastiaan van Zelst and Daniel Schuster},  
 }
+
```

### Comparing `pm4py-2.7.9.3/README.md` & `pm4py-2.7.9.4/README.md`

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

### Comparing `pm4py-2.7.9.3/pm4py/__init__.py` & `pm4py-2.7.9.4/pm4py/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/__init__.py` & `pm4py-2.7.9.4/pm4py/algo/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/analysis/__init__.py` & `pm4py-2.7.9.4/pm4py/algo/analysis/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/analysis/extended_marking_equation/__init__.py` & `pm4py-2.7.9.4/pm4py/algo/analysis/extended_marking_equation/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/analysis/extended_marking_equation/algorithm.py` & `pm4py-2.7.9.4/pm4py/algo/analysis/extended_marking_equation/algorithm.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/analysis/extended_marking_equation/variants/__init__.py` & `pm4py-2.7.9.4/pm4py/algo/analysis/extended_marking_equation/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/analysis/extended_marking_equation/variants/classic.py` & `pm4py-2.7.9.4/pm4py/algo/analysis/extended_marking_equation/variants/classic.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/analysis/marking_equation/__init__.py` & `pm4py-2.7.9.4/pm4py/algo/analysis/marking_equation/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/analysis/marking_equation/algorithm.py` & `pm4py-2.7.9.4/pm4py/algo/analysis/marking_equation/algorithm.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/analysis/marking_equation/variants/__init__.py` & `pm4py-2.7.9.4/pm4py/algo/analysis/marking_equation/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/analysis/marking_equation/variants/classic.py` & `pm4py-2.7.9.4/pm4py/algo/analysis/marking_equation/variants/classic.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/analysis/woflan/__init__.py` & `pm4py-2.7.9.4/pm4py/algo/analysis/woflan/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/analysis/woflan/algorithm.py` & `pm4py-2.7.9.4/pm4py/algo/analysis/woflan/algorithm.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/analysis/woflan/graphs/__init__.py` & `pm4py-2.7.9.4/pm4py/algo/analysis/woflan/graphs/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/analysis/woflan/graphs/minimal_coverability_graph/__init__.py` & `pm4py-2.7.9.4/pm4py/algo/analysis/woflan/graphs/minimal_coverability_graph/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/analysis/woflan/graphs/minimal_coverability_graph/minimal_coverability_graph.py` & `pm4py-2.7.9.4/pm4py/algo/analysis/woflan/graphs/minimal_coverability_graph/minimal_coverability_graph.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/analysis/woflan/graphs/reachability_graph/__init__.py` & `pm4py-2.7.9.4/pm4py/algo/analysis/woflan/graphs/reachability_graph/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/analysis/woflan/graphs/reachability_graph/reachability_graph.py` & `pm4py-2.7.9.4/pm4py/algo/analysis/woflan/graphs/reachability_graph/reachability_graph.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/analysis/woflan/graphs/restricted_coverability_graph/__init__.py` & `pm4py-2.7.9.4/pm4py/algo/analysis/woflan/graphs/restricted_coverability_graph/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/analysis/woflan/graphs/restricted_coverability_graph/restricted_coverability_graph.py` & `pm4py-2.7.9.4/pm4py/algo/analysis/woflan/graphs/restricted_coverability_graph/restricted_coverability_graph.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/analysis/woflan/graphs/utility.py` & `pm4py-2.7.9.4/pm4py/algo/analysis/woflan/graphs/utility.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/analysis/woflan/not_well_handled_pairs/__init__.py` & `pm4py-2.7.9.4/pm4py/algo/analysis/woflan/not_well_handled_pairs/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/analysis/woflan/not_well_handled_pairs/not_well_handled_pairs.py` & `pm4py-2.7.9.4/pm4py/algo/analysis/woflan/not_well_handled_pairs/not_well_handled_pairs.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/analysis/woflan/place_invariants/__init__.py` & `pm4py-2.7.9.4/pm4py/algo/analysis/woflan/place_invariants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/analysis/woflan/place_invariants/place_invariants.py` & `pm4py-2.7.9.4/pm4py/algo/analysis/woflan/place_invariants/place_invariants.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/analysis/woflan/place_invariants/s_component.py` & `pm4py-2.7.9.4/pm4py/algo/analysis/woflan/place_invariants/s_component.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/analysis/woflan/place_invariants/uniform_invariant.py` & `pm4py-2.7.9.4/pm4py/algo/analysis/woflan/place_invariants/uniform_invariant.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/analysis/woflan/place_invariants/utility.py` & `pm4py-2.7.9.4/pm4py/algo/analysis/woflan/place_invariants/utility.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/analysis/workflow_net/__init__.py` & `pm4py-2.7.9.4/pm4py/algo/analysis/workflow_net/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/analysis/workflow_net/algorithm.py` & `pm4py-2.7.9.4/pm4py/algo/analysis/workflow_net/algorithm.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/analysis/workflow_net/variants/__init__.py` & `pm4py-2.7.9.4/pm4py/algo/analysis/workflow_net/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/analysis/workflow_net/variants/petri_net.py` & `pm4py-2.7.9.4/pm4py/algo/analysis/workflow_net/variants/petri_net.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/anonymization/__init__.py` & `pm4py-2.7.9.4/pm4py/algo/anonymization/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/anonymization/pripel/__init__.py` & `pm4py-2.7.9.4/pm4py/algo/anonymization/pripel/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/anonymization/pripel/algorithm.py` & `pm4py-2.7.9.4/pm4py/algo/anonymization/pripel/algorithm.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/anonymization/pripel/util/AttributeAnonymizer.py` & `pm4py-2.7.9.4/pm4py/algo/anonymization/pripel/util/AttributeAnonymizer.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/anonymization/pripel/util/TraceMatcher.py` & `pm4py-2.7.9.4/pm4py/algo/anonymization/pripel/util/TraceMatcher.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/anonymization/pripel/util/__init__.py` & `pm4py-2.7.9.4/pm4py/algo/anonymization/pripel/util/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/anonymization/pripel/util/trace_levenshtein.py` & `pm4py-2.7.9.4/pm4py/algo/anonymization/pripel/util/trace_levenshtein.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/anonymization/pripel/variants/__init__.py` & `pm4py-2.7.9.4/pm4py/algo/anonymization/pripel/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/anonymization/pripel/variants/pripel.py` & `pm4py-2.7.9.4/pm4py/algo/anonymization/pripel/variants/pripel.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/anonymization/trace_variant_query/__init__.py` & `pm4py-2.7.9.4/pm4py/algo/anonymization/trace_variant_query/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/anonymization/trace_variant_query/algorithm.py` & `pm4py-2.7.9.4/pm4py/algo/anonymization/trace_variant_query/algorithm.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/anonymization/trace_variant_query/util/__init__.py` & `pm4py-2.7.9.4/pm4py/algo/anonymization/trace_variant_query/util/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/anonymization/trace_variant_query/util/behavioralAppropriateness.py` & `pm4py-2.7.9.4/pm4py/algo/anonymization/trace_variant_query/util/behavioralAppropriateness.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/anonymization/trace_variant_query/util/exp_mech.py` & `pm4py-2.7.9.4/pm4py/algo/anonymization/trace_variant_query/util/exp_mech.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/anonymization/trace_variant_query/util/util.py` & `pm4py-2.7.9.4/pm4py/algo/anonymization/trace_variant_query/util/util.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/anonymization/trace_variant_query/variants/__init__.py` & `pm4py-2.7.9.4/pm4py/algo/anonymization/trace_variant_query/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/anonymization/trace_variant_query/variants/laplace.py` & `pm4py-2.7.9.4/pm4py/algo/anonymization/trace_variant_query/variants/laplace.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/anonymization/trace_variant_query/variants/sacofa.py` & `pm4py-2.7.9.4/pm4py/algo/anonymization/trace_variant_query/variants/sacofa.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/clustering/__init__.py` & `pm4py-2.7.9.4/pm4py/algo/clustering/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/clustering/profiles/__init__.py` & `pm4py-2.7.9.4/pm4py/algo/clustering/profiles/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/clustering/profiles/algorithm.py` & `pm4py-2.7.9.4/pm4py/algo/clustering/profiles/algorithm.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/clustering/profiles/variants/__init__.py` & `pm4py-2.7.9.4/pm4py/algo/clustering/profiles/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/clustering/profiles/variants/sklearn_profiles.py` & `pm4py-2.7.9.4/pm4py/algo/clustering/profiles/variants/sklearn_profiles.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/clustering/trace_attribute_driven/__init__.py` & `pm4py-2.7.9.4/pm4py/algo/clustering/trace_attribute_driven/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/clustering/trace_attribute_driven/algorithm.py` & `pm4py-2.7.9.4/pm4py/algo/clustering/trace_attribute_driven/algorithm.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/clustering/trace_attribute_driven/dfg/__init__.py` & `pm4py-2.7.9.4/pm4py/algo/clustering/trace_attribute_driven/dfg/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/clustering/trace_attribute_driven/dfg/dfg_dist.py` & `pm4py-2.7.9.4/pm4py/algo/clustering/trace_attribute_driven/dfg/dfg_dist.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/clustering/trace_attribute_driven/leven_dist/__init__.py` & `pm4py-2.7.9.4/pm4py/algo/clustering/trace_attribute_driven/leven_dist/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/clustering/trace_attribute_driven/leven_dist/leven_dist_calc.py` & `pm4py-2.7.9.4/pm4py/algo/clustering/trace_attribute_driven/leven_dist/leven_dist_calc.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/clustering/trace_attribute_driven/linkage_method/__init__.py` & `pm4py-2.7.9.4/pm4py/algo/clustering/trace_attribute_driven/linkage_method/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/clustering/trace_attribute_driven/linkage_method/linkage_avg.py` & `pm4py-2.7.9.4/pm4py/algo/clustering/trace_attribute_driven/linkage_method/linkage_avg.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/clustering/trace_attribute_driven/merge_log/__init__.py` & `pm4py-2.7.9.4/pm4py/algo/clustering/trace_attribute_driven/merge_log/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/clustering/trace_attribute_driven/merge_log/merge_log.py` & `pm4py-2.7.9.4/pm4py/algo/clustering/trace_attribute_driven/merge_log/merge_log.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/clustering/trace_attribute_driven/util/__init__.py` & `pm4py-2.7.9.4/pm4py/algo/clustering/trace_attribute_driven/util/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/clustering/trace_attribute_driven/util/evaluation.py` & `pm4py-2.7.9.4/pm4py/algo/clustering/trace_attribute_driven/util/evaluation.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/clustering/trace_attribute_driven/util/filter_subsets.py` & `pm4py-2.7.9.4/pm4py/algo/clustering/trace_attribute_driven/util/filter_subsets.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/clustering/trace_attribute_driven/variants/__init__.py` & `pm4py-2.7.9.4/pm4py/algo/clustering/trace_attribute_driven/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/clustering/trace_attribute_driven/variants/act_dist_calc.py` & `pm4py-2.7.9.4/pm4py/algo/clustering/trace_attribute_driven/variants/act_dist_calc.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/clustering/trace_attribute_driven/variants/logslice_dist.py` & `pm4py-2.7.9.4/pm4py/algo/clustering/trace_attribute_driven/variants/logslice_dist.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/clustering/trace_attribute_driven/variants/sim_calc.py` & `pm4py-2.7.9.4/pm4py/algo/clustering/trace_attribute_driven/variants/sim_calc.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/clustering/trace_attribute_driven/variants/suc_dist_calc.py` & `pm4py-2.7.9.4/pm4py/algo/clustering/trace_attribute_driven/variants/suc_dist_calc.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/comparison/__init__.py` & `pm4py-2.7.9.4/pm4py/algo/comparison/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/comparison/petrinet/__init__.py` & `pm4py-2.7.9.4/pm4py/algo/comparison/petrinet/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/comparison/petrinet/element_usage_comparison.py` & `pm4py-2.7.9.4/pm4py/algo/comparison/petrinet/element_usage_comparison.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/conformance/__init__.py` & `pm4py-2.7.9.4/pm4py/algo/conformance/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/conformance/alignments/__init__.py` & `pm4py-2.7.9.4/pm4py/algo/conformance/alignments/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/conformance/alignments/decomposed/__init__.py` & `pm4py-2.7.9.4/pm4py/algo/conformance/alignments/decomposed/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/conformance/alignments/decomposed/algorithm.py` & `pm4py-2.7.9.4/pm4py/algo/conformance/alignments/decomposed/algorithm.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/conformance/alignments/decomposed/variants/__init__.py` & `pm4py-2.7.9.4/pm4py/algo/conformance/alignments/decomposed/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/conformance/alignments/decomposed/variants/recompos_maximal.py` & `pm4py-2.7.9.4/pm4py/algo/conformance/alignments/decomposed/variants/recompos_maximal.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/conformance/alignments/dfg/__init__.py` & `pm4py-2.7.9.4/pm4py/algo/conformance/alignments/dfg/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/conformance/alignments/dfg/algorithm.py` & `pm4py-2.7.9.4/pm4py/algo/conformance/alignments/dfg/algorithm.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/conformance/alignments/dfg/variants/__init__.py` & `pm4py-2.7.9.4/pm4py/algo/conformance/alignments/dfg/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/conformance/alignments/dfg/variants/classic.py` & `pm4py-2.7.9.4/pm4py/algo/conformance/alignments/dfg/variants/classic.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/conformance/alignments/edit_distance/__init__.py` & `pm4py-2.7.9.4/pm4py/algo/conformance/alignments/edit_distance/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/conformance/alignments/edit_distance/algorithm.py` & `pm4py-2.7.9.4/pm4py/algo/conformance/alignments/edit_distance/algorithm.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/conformance/alignments/edit_distance/variants/__init__.py` & `pm4py-2.7.9.4/pm4py/algo/conformance/alignments/edit_distance/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/conformance/alignments/edit_distance/variants/edit_distance.py` & `pm4py-2.7.9.4/pm4py/algo/conformance/alignments/edit_distance/variants/edit_distance.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/conformance/alignments/petri_net/__init__.py` & `pm4py-2.7.9.4/pm4py/algo/conformance/alignments/petri_net/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/conformance/alignments/petri_net/algorithm.py` & `pm4py-2.7.9.4/pm4py/algo/conformance/alignments/petri_net/algorithm.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/conformance/alignments/petri_net/utils/__init__.py` & `pm4py-2.7.9.4/pm4py/algo/conformance/alignments/petri_net/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/conformance/alignments/petri_net/utils/log_enrichment.py` & `pm4py-2.7.9.4/pm4py/algo/conformance/alignments/petri_net/utils/log_enrichment.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/conformance/alignments/petri_net/variants/__init__.py` & `pm4py-2.7.9.4/pm4py/algo/conformance/alignments/petri_net/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/conformance/alignments/petri_net/variants/dijkstra_less_memory.py` & `pm4py-2.7.9.4/pm4py/algo/conformance/alignments/petri_net/variants/dijkstra_less_memory.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/conformance/alignments/petri_net/variants/dijkstra_no_heuristics.py` & `pm4py-2.7.9.4/pm4py/algo/conformance/alignments/petri_net/variants/dijkstra_no_heuristics.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/conformance/alignments/petri_net/variants/discounted_a_star.py` & `pm4py-2.7.9.4/pm4py/algo/conformance/alignments/petri_net/variants/discounted_a_star.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/conformance/alignments/petri_net/variants/generator_dijkstra_less_memory.py` & `pm4py-2.7.9.4/pm4py/algo/conformance/alignments/petri_net/variants/generator_dijkstra_less_memory.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/conformance/alignments/petri_net/variants/generator_dijkstra_no_heuristics.py` & `pm4py-2.7.9.4/pm4py/algo/conformance/alignments/petri_net/variants/generator_dijkstra_no_heuristics.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/conformance/alignments/petri_net/variants/state_equation_a_star.py` & `pm4py-2.7.9.4/pm4py/algo/conformance/alignments/petri_net/variants/state_equation_a_star.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/conformance/alignments/petri_net/variants/tweaked_state_equation_a_star.py` & `pm4py-2.7.9.4/pm4py/algo/conformance/alignments/petri_net/variants/tweaked_state_equation_a_star.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/conformance/alignments/process_tree/__init__.py` & `pm4py-2.7.9.4/pm4py/algo/conformance/alignments/process_tree/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/conformance/alignments/process_tree/algorithm.py` & `pm4py-2.7.9.4/pm4py/algo/conformance/alignments/process_tree/algorithm.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/conformance/alignments/process_tree/util/__init__.py` & `pm4py-2.7.9.4/pm4py/algo/conformance/alignments/process_tree/util/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/conformance/alignments/process_tree/util/search_graph_pt_frequency_annotation.py` & `pm4py-2.7.9.4/pm4py/algo/conformance/alignments/process_tree/util/search_graph_pt_frequency_annotation.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/conformance/alignments/process_tree/util/search_graph_pt_replay_semantics.py` & `pm4py-2.7.9.4/pm4py/algo/conformance/alignments/process_tree/util/search_graph_pt_replay_semantics.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/conformance/alignments/process_tree/variants/__init__.py` & `pm4py-2.7.9.4/pm4py/algo/conformance/alignments/process_tree/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/conformance/alignments/process_tree/variants/approximated/__init__.py` & `pm4py-2.7.9.4/pm4py/algo/conformance/alignments/process_tree/variants/approximated/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/conformance/alignments/process_tree/variants/approximated/calculate_a_sa_ea_sets.py` & `pm4py-2.7.9.4/pm4py/algo/conformance/alignments/process_tree/variants/approximated/calculate_a_sa_ea_sets.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/conformance/alignments/process_tree/variants/approximated/matrix_lp.py` & `pm4py-2.7.9.4/pm4py/algo/conformance/alignments/process_tree/variants/approximated/matrix_lp.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/conformance/alignments/process_tree/variants/approximated/original.py` & `pm4py-2.7.9.4/pm4py/algo/conformance/alignments/process_tree/variants/approximated/original.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/conformance/alignments/process_tree/variants/approximated/utilities.py` & `pm4py-2.7.9.4/pm4py/algo/conformance/alignments/process_tree/variants/approximated/utilities.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/conformance/alignments/process_tree/variants/search_graph_pt.py` & `pm4py-2.7.9.4/pm4py/algo/conformance/alignments/process_tree/variants/search_graph_pt.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/conformance/antialignments/__init__.py` & `pm4py-2.7.9.4/pm4py/algo/conformance/antialignments/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/conformance/antialignments/algorithm.py` & `pm4py-2.7.9.4/pm4py/algo/conformance/antialignments/algorithm.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/conformance/antialignments/variants/__init__.py` & `pm4py-2.7.9.4/pm4py/algo/conformance/antialignments/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/conformance/antialignments/variants/discounted_a_star.py` & `pm4py-2.7.9.4/pm4py/algo/conformance/antialignments/variants/discounted_a_star.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/conformance/declare/__init__.py` & `pm4py-2.7.9.4/pm4py/algo/conformance/declare/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/conformance/declare/algorithm.py` & `pm4py-2.7.9.4/pm4py/algo/conformance/declare/algorithm.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/conformance/declare/variants/__init__.py` & `pm4py-2.7.9.4/pm4py/algo/conformance/declare/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/conformance/declare/variants/classic.py` & `pm4py-2.7.9.4/pm4py/algo/conformance/declare/variants/classic.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/conformance/footprints/__init__.py` & `pm4py-2.7.9.4/pm4py/algo/conformance/footprints/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/conformance/footprints/algorithm.py` & `pm4py-2.7.9.4/pm4py/algo/conformance/footprints/algorithm.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/conformance/footprints/util/__init__.py` & `pm4py-2.7.9.4/pm4py/algo/conformance/footprints/util/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/conformance/footprints/util/evaluation.py` & `pm4py-2.7.9.4/pm4py/algo/conformance/footprints/util/evaluation.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/conformance/footprints/util/tree_visualization.py` & `pm4py-2.7.9.4/pm4py/algo/conformance/footprints/util/tree_visualization.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/conformance/footprints/variants/__init__.py` & `pm4py-2.7.9.4/pm4py/algo/conformance/footprints/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/conformance/footprints/variants/log_extensive.py` & `pm4py-2.7.9.4/pm4py/algo/conformance/footprints/variants/log_extensive.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/conformance/footprints/variants/log_model.py` & `pm4py-2.7.9.4/pm4py/algo/conformance/footprints/variants/log_model.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/conformance/footprints/variants/trace_extensive.py` & `pm4py-2.7.9.4/pm4py/algo/conformance/footprints/variants/trace_extensive.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/conformance/log_skeleton/__init__.py` & `pm4py-2.7.9.4/pm4py/algo/conformance/log_skeleton/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/conformance/log_skeleton/algorithm.py` & `pm4py-2.7.9.4/pm4py/algo/conformance/log_skeleton/algorithm.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/conformance/log_skeleton/variants/__init__.py` & `pm4py-2.7.9.4/pm4py/algo/conformance/log_skeleton/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/conformance/log_skeleton/variants/classic.py` & `pm4py-2.7.9.4/pm4py/algo/conformance/log_skeleton/variants/classic.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/conformance/multialignments/__init__.py` & `pm4py-2.7.9.4/pm4py/algo/conformance/multialignments/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/conformance/multialignments/algorithm.py` & `pm4py-2.7.9.4/pm4py/algo/conformance/multialignments/algorithm.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/conformance/multialignments/variants/__init__.py` & `pm4py-2.7.9.4/pm4py/algo/conformance/multialignments/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/conformance/multialignments/variants/discounted_a_star.py` & `pm4py-2.7.9.4/pm4py/algo/conformance/multialignments/variants/discounted_a_star.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/conformance/temporal_profile/__init__.py` & `pm4py-2.7.9.4/pm4py/algo/conformance/temporal_profile/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/conformance/temporal_profile/algorithm.py` & `pm4py-2.7.9.4/pm4py/algo/conformance/temporal_profile/algorithm.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/conformance/temporal_profile/variants/__init__.py` & `pm4py-2.7.9.4/pm4py/algo/conformance/temporal_profile/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/conformance/temporal_profile/variants/dataframe.py` & `pm4py-2.7.9.4/pm4py/algo/conformance/temporal_profile/variants/dataframe.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/conformance/temporal_profile/variants/log.py` & `pm4py-2.7.9.4/pm4py/algo/conformance/temporal_profile/variants/log.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/conformance/tokenreplay/__init__.py` & `pm4py-2.7.9.4/pm4py/algo/conformance/tokenreplay/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/conformance/tokenreplay/algorithm.py` & `pm4py-2.7.9.4/pm4py/algo/conformance/tokenreplay/algorithm.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/conformance/tokenreplay/diagnostics/__init__.py` & `pm4py-2.7.9.4/pm4py/algo/conformance/tokenreplay/diagnostics/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/conformance/tokenreplay/diagnostics/duration_diagnostics.py` & `pm4py-2.7.9.4/pm4py/algo/conformance/tokenreplay/diagnostics/duration_diagnostics.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/conformance/tokenreplay/diagnostics/root_cause_analysis.py` & `pm4py-2.7.9.4/pm4py/algo/conformance/tokenreplay/diagnostics/root_cause_analysis.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/conformance/tokenreplay/variants/__init__.py` & `pm4py-2.7.9.4/pm4py/algo/conformance/tokenreplay/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/conformance/tokenreplay/variants/backwards.py` & `pm4py-2.7.9.4/pm4py/algo/conformance/tokenreplay/variants/backwards.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/conformance/tokenreplay/variants/token_replay.py` & `pm4py-2.7.9.4/pm4py/algo/conformance/tokenreplay/variants/token_replay.py`

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

### Comparing `pm4py-2.7.9.3/pm4py/algo/connectors/__init__.py` & `pm4py-2.7.9.4/pm4py/algo/connectors/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/connectors/algorithm.py` & `pm4py-2.7.9.4/pm4py/algo/connectors/algorithm.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/connectors/util/__init__.py` & `pm4py-2.7.9.4/pm4py/algo/connectors/util/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/connectors/util/mail.py` & `pm4py-2.7.9.4/pm4py/algo/connectors/util/mail.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/connectors/variants/__init__.py` & `pm4py-2.7.9.4/pm4py/algo/connectors/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/connectors/variants/camunda_workflow.py` & `pm4py-2.7.9.4/pm4py/algo/connectors/variants/camunda_workflow.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/connectors/variants/chrome_history.py` & `pm4py-2.7.9.4/pm4py/algo/connectors/variants/chrome_history.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/connectors/variants/firefox_history.py` & `pm4py-2.7.9.4/pm4py/algo/connectors/variants/firefox_history.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/connectors/variants/github_repo.py` & `pm4py-2.7.9.4/pm4py/algo/connectors/variants/github_repo.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/connectors/variants/outlook_calendar.py` & `pm4py-2.7.9.4/pm4py/algo/connectors/variants/outlook_calendar.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/connectors/variants/outlook_mail_extractor.py` & `pm4py-2.7.9.4/pm4py/algo/connectors/variants/outlook_mail_extractor.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/connectors/variants/sap_accounting.py` & `pm4py-2.7.9.4/pm4py/algo/connectors/variants/sap_accounting.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/connectors/variants/sap_o2c.py` & `pm4py-2.7.9.4/pm4py/algo/connectors/variants/sap_o2c.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/connectors/variants/windows_events.py` & `pm4py-2.7.9.4/pm4py/algo/connectors/variants/windows_events.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/decision_mining/__init__.py` & `pm4py-2.7.9.4/pm4py/algo/decision_mining/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/decision_mining/algorithm.py` & `pm4py-2.7.9.4/pm4py/algo/decision_mining/algorithm.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/discovery/__init__.py` & `pm4py-2.7.9.4/pm4py/algo/discovery/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/discovery/alpha/__init__.py` & `pm4py-2.7.9.4/pm4py/algo/discovery/alpha/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/discovery/alpha/algorithm.py` & `pm4py-2.7.9.4/pm4py/algo/discovery/alpha/algorithm.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/discovery/alpha/data_structures/__init__.py` & `pm4py-2.7.9.4/pm4py/algo/discovery/alpha/data_structures/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/discovery/alpha/data_structures/alpha_classic_abstraction.py` & `pm4py-2.7.9.4/pm4py/algo/discovery/alpha/data_structures/alpha_classic_abstraction.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/discovery/alpha/utils/__init__.py` & `pm4py-2.7.9.4/pm4py/algo/discovery/alpha/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/discovery/alpha/utils/endpoints.py` & `pm4py-2.7.9.4/pm4py/algo/discovery/alpha/utils/endpoints.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/discovery/alpha/variants/__init__.py` & `pm4py-2.7.9.4/pm4py/algo/discovery/alpha/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/discovery/alpha/variants/classic.py` & `pm4py-2.7.9.4/pm4py/algo/discovery/alpha/variants/classic.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/discovery/alpha/variants/plus.py` & `pm4py-2.7.9.4/pm4py/algo/discovery/alpha/variants/plus.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/discovery/batches/__init__.py` & `pm4py-2.7.9.4/pm4py/algo/discovery/batches/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/discovery/batches/algorithm.py` & `pm4py-2.7.9.4/pm4py/algo/discovery/batches/algorithm.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/discovery/batches/utils/__init__.py` & `pm4py-2.7.9.4/pm4py/algo/discovery/batches/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/discovery/batches/utils/detection.py` & `pm4py-2.7.9.4/pm4py/algo/discovery/batches/utils/detection.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/discovery/batches/variants/__init__.py` & `pm4py-2.7.9.4/pm4py/algo/discovery/batches/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/discovery/batches/variants/log.py` & `pm4py-2.7.9.4/pm4py/algo/discovery/batches/variants/log.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/discovery/batches/variants/pandas.py` & `pm4py-2.7.9.4/pm4py/algo/discovery/batches/variants/pandas.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/discovery/causal/__init__.py` & `pm4py-2.7.9.4/pm4py/algo/discovery/causal/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/discovery/causal/algorithm.py` & `pm4py-2.7.9.4/pm4py/algo/discovery/causal/algorithm.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/discovery/causal/variants/__init__.py` & `pm4py-2.7.9.4/pm4py/algo/discovery/causal/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/discovery/causal/variants/alpha.py` & `pm4py-2.7.9.4/pm4py/algo/discovery/causal/variants/alpha.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/discovery/causal/variants/heuristic.py` & `pm4py-2.7.9.4/pm4py/algo/discovery/causal/variants/heuristic.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/discovery/correlation_mining/__init__.py` & `pm4py-2.7.9.4/pm4py/algo/discovery/correlation_mining/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/discovery/correlation_mining/algorithm.py` & `pm4py-2.7.9.4/pm4py/algo/discovery/correlation_mining/algorithm.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/discovery/correlation_mining/util.py` & `pm4py-2.7.9.4/pm4py/algo/discovery/correlation_mining/util.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/discovery/correlation_mining/variants/__init__.py` & `pm4py-2.7.9.4/pm4py/algo/discovery/correlation_mining/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/discovery/correlation_mining/variants/classic.py` & `pm4py-2.7.9.4/pm4py/algo/discovery/correlation_mining/variants/classic.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/discovery/correlation_mining/variants/classic_split.py` & `pm4py-2.7.9.4/pm4py/algo/discovery/correlation_mining/variants/classic_split.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/discovery/correlation_mining/variants/trace_based.py` & `pm4py-2.7.9.4/pm4py/algo/discovery/correlation_mining/variants/trace_based.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/discovery/declare/__init__.py` & `pm4py-2.7.9.4/pm4py/algo/discovery/declare/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/discovery/declare/algorithm.py` & `pm4py-2.7.9.4/pm4py/algo/discovery/declare/algorithm.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/discovery/declare/templates.py` & `pm4py-2.7.9.4/pm4py/algo/discovery/declare/templates.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/discovery/declare/variants/__init__.py` & `pm4py-2.7.9.4/pm4py/algo/discovery/declare/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/discovery/declare/variants/classic.py` & `pm4py-2.7.9.4/pm4py/algo/discovery/declare/variants/classic.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/discovery/dfg/__init__.py` & `pm4py-2.7.9.4/pm4py/algo/discovery/dfg/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/discovery/dfg/adapters/__init__.py` & `pm4py-2.7.9.4/pm4py/algo/discovery/dfg/adapters/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/discovery/dfg/adapters/pandas/__init__.py` & `pm4py-2.7.9.4/pm4py/algo/discovery/dfg/adapters/pandas/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/discovery/dfg/adapters/pandas/df_statistics.py` & `pm4py-2.7.9.4/pm4py/algo/discovery/dfg/adapters/pandas/df_statistics.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/discovery/dfg/adapters/pandas/freq_triples.py` & `pm4py-2.7.9.4/pm4py/algo/discovery/dfg/adapters/pandas/freq_triples.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/discovery/dfg/algorithm.py` & `pm4py-2.7.9.4/pm4py/algo/discovery/dfg/algorithm.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/discovery/dfg/replacement.py` & `pm4py-2.7.9.4/pm4py/algo/discovery/dfg/replacement.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/discovery/dfg/utils/__init__.py` & `pm4py-2.7.9.4/pm4py/algo/discovery/dfg/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/discovery/dfg/utils/dfg_utils.py` & `pm4py-2.7.9.4/pm4py/algo/discovery/dfg/utils/dfg_utils.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/discovery/dfg/variants/__init__.py` & `pm4py-2.7.9.4/pm4py/algo/discovery/dfg/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/discovery/dfg/variants/case_attributes.py` & `pm4py-2.7.9.4/pm4py/algo/discovery/dfg/variants/case_attributes.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/discovery/dfg/variants/clean.py` & `pm4py-2.7.9.4/pm4py/algo/discovery/dfg/variants/clean.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/discovery/dfg/variants/clean_polars.py` & `pm4py-2.7.9.4/pm4py/algo/discovery/dfg/variants/clean_polars.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/discovery/dfg/variants/clean_time.py` & `pm4py-2.7.9.4/pm4py/algo/discovery/dfg/variants/clean_time.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/discovery/dfg/variants/freq_triples.py` & `pm4py-2.7.9.4/pm4py/algo/discovery/dfg/variants/freq_triples.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/discovery/dfg/variants/native.py` & `pm4py-2.7.9.4/pm4py/algo/discovery/dfg/variants/native.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/discovery/dfg/variants/performance.py` & `pm4py-2.7.9.4/pm4py/algo/discovery/dfg/variants/performance.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/discovery/footprints/__init__.py` & `pm4py-2.7.9.4/pm4py/algo/discovery/footprints/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/discovery/footprints/algorithm.py` & `pm4py-2.7.9.4/pm4py/algo/discovery/footprints/algorithm.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/discovery/footprints/dfg/__init__.py` & `pm4py-2.7.9.4/pm4py/algo/discovery/footprints/dfg/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/discovery/footprints/dfg/variants/__init__.py` & `pm4py-2.7.9.4/pm4py/algo/discovery/footprints/dfg/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/discovery/footprints/dfg/variants/dfg.py` & `pm4py-2.7.9.4/pm4py/algo/discovery/footprints/dfg/variants/dfg.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/discovery/footprints/log/__init__.py` & `pm4py-2.7.9.4/pm4py/algo/discovery/footprints/log/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/discovery/footprints/log/variants/__init__.py` & `pm4py-2.7.9.4/pm4py/algo/discovery/footprints/log/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/discovery/footprints/log/variants/entire_dataframe.py` & `pm4py-2.7.9.4/pm4py/algo/discovery/footprints/log/variants/entire_dataframe.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/discovery/footprints/log/variants/entire_event_log.py` & `pm4py-2.7.9.4/pm4py/algo/discovery/footprints/log/variants/entire_event_log.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/discovery/footprints/log/variants/trace_by_trace.py` & `pm4py-2.7.9.4/pm4py/algo/discovery/footprints/log/variants/trace_by_trace.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/discovery/footprints/petri/__init__.py` & `pm4py-2.7.9.4/pm4py/algo/discovery/footprints/petri/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/discovery/footprints/petri/variants/__init__.py` & `pm4py-2.7.9.4/pm4py/algo/discovery/footprints/petri/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/discovery/footprints/petri/variants/reach_graph.py` & `pm4py-2.7.9.4/pm4py/algo/discovery/footprints/petri/variants/reach_graph.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/discovery/footprints/tree/__init__.py` & `pm4py-2.7.9.4/pm4py/algo/discovery/footprints/tree/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/discovery/footprints/tree/variants/__init__.py` & `pm4py-2.7.9.4/pm4py/algo/discovery/footprints/tree/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/discovery/footprints/tree/variants/bottomup.py` & `pm4py-2.7.9.4/pm4py/algo/discovery/footprints/tree/variants/bottomup.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/discovery/heuristics/__init__.py` & `pm4py-2.7.9.4/pm4py/algo/discovery/heuristics/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/discovery/heuristics/algorithm.py` & `pm4py-2.7.9.4/pm4py/algo/discovery/heuristics/algorithm.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/discovery/heuristics/variants/__init__.py` & `pm4py-2.7.9.4/pm4py/algo/discovery/heuristics/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/discovery/heuristics/variants/classic.py` & `pm4py-2.7.9.4/pm4py/algo/discovery/heuristics/variants/classic.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/discovery/heuristics/variants/plusplus.py` & `pm4py-2.7.9.4/pm4py/algo/discovery/heuristics/variants/plusplus.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/discovery/ilp/__init__.py` & `pm4py-2.7.9.4/pm4py/algo/discovery/ilp/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/discovery/ilp/algorithm.py` & `pm4py-2.7.9.4/pm4py/algo/discovery/ilp/algorithm.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/discovery/ilp/variants/__init__.py` & `pm4py-2.7.9.4/pm4py/algo/discovery/ilp/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/discovery/ilp/variants/classic.py` & `pm4py-2.7.9.4/pm4py/algo/discovery/ilp/variants/classic.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/discovery/inductive/__init__.py` & `pm4py-2.7.9.4/pm4py/algo/discovery/inductive/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/discovery/inductive/algorithm.py` & `pm4py-2.7.9.4/pm4py/algo/discovery/inductive/algorithm.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/discovery/inductive/base_case/__init__.py` & `pm4py-2.7.9.4/pm4py/algo/discovery/inductive/base_case/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/discovery/inductive/base_case/abc.py` & `pm4py-2.7.9.4/pm4py/algo/discovery/inductive/base_case/abc.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/discovery/inductive/base_case/empty_log.py` & `pm4py-2.7.9.4/pm4py/algo/discovery/inductive/base_case/empty_log.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/discovery/inductive/base_case/factory.py` & `pm4py-2.7.9.4/pm4py/algo/discovery/inductive/base_case/factory.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/discovery/inductive/base_case/single_activity.py` & `pm4py-2.7.9.4/pm4py/algo/discovery/inductive/base_case/single_activity.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/discovery/inductive/cuts/__init__.py` & `pm4py-2.7.9.4/pm4py/algo/discovery/inductive/cuts/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/discovery/inductive/cuts/abc.py` & `pm4py-2.7.9.4/pm4py/algo/discovery/inductive/cuts/abc.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/discovery/inductive/cuts/concurrency.py` & `pm4py-2.7.9.4/pm4py/algo/discovery/inductive/cuts/concurrency.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/discovery/inductive/cuts/factory.py` & `pm4py-2.7.9.4/pm4py/algo/discovery/inductive/cuts/factory.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/discovery/inductive/cuts/loop.py` & `pm4py-2.7.9.4/pm4py/algo/discovery/inductive/cuts/loop.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/discovery/inductive/cuts/sequence.py` & `pm4py-2.7.9.4/pm4py/algo/discovery/inductive/cuts/sequence.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/discovery/inductive/cuts/utils.py` & `pm4py-2.7.9.4/pm4py/algo/discovery/inductive/cuts/utils.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/discovery/inductive/cuts/xor.py` & `pm4py-2.7.9.4/pm4py/algo/discovery/inductive/cuts/xor.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/discovery/inductive/dtypes/__init__.py` & `pm4py-2.7.9.4/pm4py/algo/discovery/inductive/dtypes/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/discovery/inductive/dtypes/im_dfg.py` & `pm4py-2.7.9.4/pm4py/algo/discovery/inductive/dtypes/im_dfg.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/discovery/inductive/dtypes/im_ds.py` & `pm4py-2.7.9.4/pm4py/algo/discovery/inductive/dtypes/im_ds.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/discovery/inductive/fall_through/__init__.py` & `pm4py-2.7.9.4/pm4py/algo/discovery/inductive/fall_through/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/discovery/inductive/fall_through/abc.py` & `pm4py-2.7.9.4/pm4py/algo/discovery/inductive/fall_through/abc.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/discovery/inductive/fall_through/activity_concurrent.py` & `pm4py-2.7.9.4/pm4py/algo/discovery/inductive/fall_through/activity_concurrent.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/discovery/inductive/fall_through/activity_once_per_trace.py` & `pm4py-2.7.9.4/pm4py/algo/discovery/inductive/fall_through/activity_once_per_trace.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/discovery/inductive/fall_through/empty_traces.py` & `pm4py-2.7.9.4/pm4py/algo/discovery/inductive/fall_through/empty_traces.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/discovery/inductive/fall_through/factory.py` & `pm4py-2.7.9.4/pm4py/algo/discovery/inductive/fall_through/factory.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/discovery/inductive/fall_through/flower.py` & `pm4py-2.7.9.4/pm4py/algo/discovery/inductive/fall_through/flower.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/discovery/inductive/fall_through/strict_tau_loop.py` & `pm4py-2.7.9.4/pm4py/algo/discovery/inductive/fall_through/strict_tau_loop.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/discovery/inductive/fall_through/tau_loop.py` & `pm4py-2.7.9.4/pm4py/algo/discovery/inductive/fall_through/tau_loop.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/discovery/inductive/variants/__init__.py` & `pm4py-2.7.9.4/pm4py/algo/discovery/inductive/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/discovery/inductive/variants/abc.py` & `pm4py-2.7.9.4/pm4py/algo/discovery/inductive/variants/abc.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/discovery/inductive/variants/im.py` & `pm4py-2.7.9.4/pm4py/algo/discovery/inductive/variants/im.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/discovery/inductive/variants/imd.py` & `pm4py-2.7.9.4/pm4py/algo/discovery/inductive/variants/imd.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/discovery/inductive/variants/imf.py` & `pm4py-2.7.9.4/pm4py/algo/discovery/inductive/variants/imf.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/discovery/inductive/variants/instances.py` & `pm4py-2.7.9.4/pm4py/algo/discovery/inductive/variants/instances.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/discovery/log_skeleton/__init__.py` & `pm4py-2.7.9.4/pm4py/algo/discovery/log_skeleton/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/discovery/log_skeleton/algorithm.py` & `pm4py-2.7.9.4/pm4py/algo/discovery/log_skeleton/algorithm.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/discovery/log_skeleton/trace_skel.py` & `pm4py-2.7.9.4/pm4py/algo/discovery/log_skeleton/trace_skel.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/discovery/log_skeleton/variants/__init__.py` & `pm4py-2.7.9.4/pm4py/algo/discovery/log_skeleton/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/discovery/log_skeleton/variants/classic.py` & `pm4py-2.7.9.4/pm4py/algo/discovery/log_skeleton/variants/classic.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/discovery/minimum_self_distance/__init__.py` & `pm4py-2.7.9.4/pm4py/algo/discovery/minimum_self_distance/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/discovery/minimum_self_distance/algorithm.py` & `pm4py-2.7.9.4/pm4py/algo/discovery/minimum_self_distance/algorithm.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/discovery/minimum_self_distance/utils.py` & `pm4py-2.7.9.4/pm4py/algo/discovery/minimum_self_distance/utils.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/discovery/minimum_self_distance/variants/__init__.py` & `pm4py-2.7.9.4/pm4py/algo/discovery/minimum_self_distance/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/discovery/minimum_self_distance/variants/log.py` & `pm4py-2.7.9.4/pm4py/algo/discovery/minimum_self_distance/variants/log.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/discovery/minimum_self_distance/variants/pandas.py` & `pm4py-2.7.9.4/pm4py/algo/discovery/minimum_self_distance/variants/pandas.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/discovery/ocel/__init__.py` & `pm4py-2.7.9.4/pm4py/algo/discovery/ocel/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/discovery/ocel/interleavings/__init__.py` & `pm4py-2.7.9.4/pm4py/algo/discovery/ocel/interleavings/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/discovery/ocel/interleavings/algorithm.py` & `pm4py-2.7.9.4/pm4py/algo/discovery/ocel/interleavings/algorithm.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/discovery/ocel/interleavings/utils/__init__.py` & `pm4py-2.7.9.4/pm4py/algo/discovery/ocel/interleavings/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/discovery/ocel/interleavings/utils/merge_dataframe_rel_cases.py` & `pm4py-2.7.9.4/pm4py/algo/discovery/ocel/interleavings/utils/merge_dataframe_rel_cases.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/discovery/ocel/interleavings/variants/__init__.py` & `pm4py-2.7.9.4/pm4py/algo/discovery/ocel/interleavings/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/discovery/ocel/interleavings/variants/timestamp_interleavings.py` & `pm4py-2.7.9.4/pm4py/algo/discovery/ocel/interleavings/variants/timestamp_interleavings.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/discovery/ocel/link_analysis/__init__.py` & `pm4py-2.7.9.4/pm4py/algo/discovery/ocel/link_analysis/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/discovery/ocel/link_analysis/algorithm.py` & `pm4py-2.7.9.4/pm4py/algo/discovery/ocel/link_analysis/algorithm.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/discovery/ocel/link_analysis/variants/__init__.py` & `pm4py-2.7.9.4/pm4py/algo/discovery/ocel/link_analysis/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/discovery/ocel/link_analysis/variants/classic.py` & `pm4py-2.7.9.4/pm4py/algo/discovery/ocel/link_analysis/variants/classic.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/discovery/ocel/ocdfg/__init__.py` & `pm4py-2.7.9.4/pm4py/algo/discovery/ocel/ocdfg/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/discovery/ocel/ocdfg/algorithm.py` & `pm4py-2.7.9.4/pm4py/algo/discovery/ocel/ocdfg/algorithm.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/discovery/ocel/ocdfg/variants/__init__.py` & `pm4py-2.7.9.4/pm4py/algo/discovery/ocel/ocdfg/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/discovery/ocel/ocdfg/variants/classic.py` & `pm4py-2.7.9.4/pm4py/algo/discovery/ocel/ocdfg/variants/classic.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/discovery/ocel/ocpn/__init__.py` & `pm4py-2.7.9.4/pm4py/algo/discovery/ocel/ocpn/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/discovery/ocel/ocpn/algorithm.py` & `pm4py-2.7.9.4/pm4py/algo/discovery/ocel/ocpn/algorithm.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/discovery/ocel/ocpn/variants/__init__.py` & `pm4py-2.7.9.4/pm4py/algo/discovery/ocel/ocpn/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/discovery/ocel/ocpn/variants/classic.py` & `pm4py-2.7.9.4/pm4py/algo/discovery/ocel/ocpn/variants/classic.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/discovery/ocel/ocpn/variants/wo_annotation.py` & `pm4py-2.7.9.4/pm4py/algo/discovery/ocel/ocpn/variants/wo_annotation.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/discovery/ocel/saw_nets/__init__.py` & `pm4py-2.7.9.4/pm4py/algo/discovery/ocel/saw_nets/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/discovery/ocel/saw_nets/algorithm.py` & `pm4py-2.7.9.4/pm4py/algo/discovery/ocel/saw_nets/algorithm.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/discovery/ocel/saw_nets/variants/__init__.py` & `pm4py-2.7.9.4/pm4py/algo/discovery/ocel/saw_nets/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/discovery/ocel/saw_nets/variants/classic.py` & `pm4py-2.7.9.4/pm4py/algo/discovery/ocel/saw_nets/variants/classic.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/discovery/performance_spectrum/__init__.py` & `pm4py-2.7.9.4/pm4py/algo/discovery/performance_spectrum/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/discovery/performance_spectrum/algorithm.py` & `pm4py-2.7.9.4/pm4py/algo/discovery/performance_spectrum/algorithm.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/discovery/performance_spectrum/variants/__init__.py` & `pm4py-2.7.9.4/pm4py/algo/discovery/performance_spectrum/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/discovery/performance_spectrum/variants/dataframe.py` & `pm4py-2.7.9.4/pm4py/algo/discovery/performance_spectrum/variants/dataframe.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/discovery/performance_spectrum/variants/dataframe_disconnected.py` & `pm4py-2.7.9.4/pm4py/algo/discovery/performance_spectrum/variants/dataframe_disconnected.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/discovery/performance_spectrum/variants/log.py` & `pm4py-2.7.9.4/pm4py/algo/discovery/performance_spectrum/variants/log.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/discovery/performance_spectrum/variants/log_disconnected.py` & `pm4py-2.7.9.4/pm4py/algo/discovery/performance_spectrum/variants/log_disconnected.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/discovery/powl/__init__.py` & `pm4py-2.7.9.4/pm4py/algo/discovery/powl/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/discovery/powl/algorithm.py` & `pm4py-2.7.9.4/pm4py/algo/discovery/powl/algorithm.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/discovery/powl/inductive/__init__.py` & `pm4py-2.7.9.4/pm4py/algo/discovery/powl/inductive/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/discovery/powl/inductive/base_case/__init__.py` & `pm4py-2.7.9.4/pm4py/algo/discovery/powl/inductive/base_case/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/discovery/powl/inductive/base_case/abc.py` & `pm4py-2.7.9.4/pm4py/algo/discovery/powl/inductive/base_case/abc.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/discovery/powl/inductive/base_case/empty_log.py` & `pm4py-2.7.9.4/pm4py/algo/discovery/powl/inductive/base_case/empty_log.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/discovery/powl/inductive/base_case/factory.py` & `pm4py-2.7.9.4/pm4py/algo/discovery/powl/inductive/base_case/factory.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/discovery/powl/inductive/base_case/single_activity.py` & `pm4py-2.7.9.4/pm4py/algo/discovery/powl/inductive/base_case/single_activity.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/discovery/powl/inductive/cuts/__init__.py` & `pm4py-2.7.9.4/pm4py/algo/discovery/powl/inductive/cuts/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/discovery/powl/inductive/cuts/concurrency.py` & `pm4py-2.7.9.4/pm4py/algo/discovery/powl/inductive/cuts/concurrency.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/discovery/powl/inductive/cuts/factory.py` & `pm4py-2.7.9.4/pm4py/algo/discovery/powl/inductive/cuts/factory.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/discovery/powl/inductive/cuts/loop.py` & `pm4py-2.7.9.4/pm4py/algo/discovery/powl/inductive/cuts/loop.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/discovery/powl/inductive/cuts/sequence.py` & `pm4py-2.7.9.4/pm4py/algo/discovery/powl/inductive/cuts/sequence.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/discovery/powl/inductive/cuts/xor.py` & `pm4py-2.7.9.4/pm4py/algo/discovery/powl/inductive/cuts/xor.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/discovery/powl/inductive/fall_through/__init__.py` & `pm4py-2.7.9.4/pm4py/algo/discovery/powl/inductive/fall_through/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/discovery/powl/inductive/fall_through/activity_concurrent.py` & `pm4py-2.7.9.4/pm4py/algo/discovery/powl/inductive/fall_through/activity_concurrent.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/discovery/powl/inductive/fall_through/activity_once_per_trace.py` & `pm4py-2.7.9.4/pm4py/algo/discovery/powl/inductive/fall_through/activity_once_per_trace.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/discovery/powl/inductive/fall_through/empty_traces.py` & `pm4py-2.7.9.4/pm4py/algo/discovery/powl/inductive/fall_through/empty_traces.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/discovery/powl/inductive/fall_through/factory.py` & `pm4py-2.7.9.4/pm4py/algo/discovery/powl/inductive/fall_through/factory.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/discovery/powl/inductive/fall_through/flower.py` & `pm4py-2.7.9.4/pm4py/algo/discovery/powl/inductive/fall_through/flower.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/discovery/powl/inductive/fall_through/strict_tau_loop.py` & `pm4py-2.7.9.4/pm4py/algo/discovery/powl/inductive/fall_through/strict_tau_loop.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/discovery/powl/inductive/fall_through/tau_loop.py` & `pm4py-2.7.9.4/pm4py/algo/discovery/powl/inductive/fall_through/tau_loop.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/discovery/powl/inductive/utils/__init__.py` & `pm4py-2.7.9.4/pm4py/algo/discovery/powl/inductive/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/discovery/powl/inductive/utils/filtering.py` & `pm4py-2.7.9.4/pm4py/algo/discovery/powl/inductive/utils/filtering.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/discovery/powl/inductive/variants/__init__.py` & `pm4py-2.7.9.4/pm4py/algo/discovery/powl/inductive/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/discovery/powl/inductive/variants/brute_force/__init__.py` & `pm4py-2.7.9.4/pm4py/algo/discovery/powl/inductive/variants/brute_force/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/discovery/powl/inductive/variants/brute_force/bf_partial_order_cut.py` & `pm4py-2.7.9.4/pm4py/algo/discovery/powl/inductive/variants/brute_force/bf_partial_order_cut.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/discovery/powl/inductive/variants/brute_force/factory.py` & `pm4py-2.7.9.4/pm4py/algo/discovery/powl/inductive/variants/brute_force/factory.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/discovery/powl/inductive/variants/dynamic_clustering/__init__.py` & `pm4py-2.7.9.4/pm4py/algo/discovery/powl/inductive/variants/dynamic_clustering/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/discovery/powl/inductive/variants/dynamic_clustering/dynamic_clustering_partial_order_cut.py` & `pm4py-2.7.9.4/pm4py/algo/discovery/powl/inductive/variants/dynamic_clustering/dynamic_clustering_partial_order_cut.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/discovery/powl/inductive/variants/dynamic_clustering/factory.py` & `pm4py-2.7.9.4/pm4py/algo/discovery/powl/inductive/variants/dynamic_clustering/factory.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/discovery/powl/inductive/variants/dynamic_clustering_frequency/__init__.py` & `pm4py-2.7.9.4/pm4py/algo/discovery/powl/inductive/variants/dynamic_clustering_frequency/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/discovery/powl/inductive/variants/dynamic_clustering_frequency/dynamic_clustering_frequency_partial_order_cut.py` & `pm4py-2.7.9.4/pm4py/algo/discovery/powl/inductive/variants/dynamic_clustering_frequency/dynamic_clustering_frequency_partial_order_cut.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/discovery/powl/inductive/variants/dynamic_clustering_frequency/factory.py` & `pm4py-2.7.9.4/pm4py/algo/discovery/powl/inductive/variants/dynamic_clustering_frequency/factory.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/discovery/powl/inductive/variants/im_brute_force.py` & `pm4py-2.7.9.4/pm4py/algo/discovery/powl/inductive/variants/im_brute_force.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/discovery/powl/inductive/variants/im_dynamic_clustering.py` & `pm4py-2.7.9.4/pm4py/algo/discovery/powl/inductive/variants/im_dynamic_clustering.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/discovery/powl/inductive/variants/im_dynamic_clustering_frequencies.py` & `pm4py-2.7.9.4/pm4py/algo/discovery/powl/inductive/variants/im_dynamic_clustering_frequencies.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/discovery/powl/inductive/variants/im_maximal.py` & `pm4py-2.7.9.4/pm4py/algo/discovery/powl/inductive/variants/im_maximal.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/discovery/powl/inductive/variants/im_tree.py` & `pm4py-2.7.9.4/pm4py/algo/discovery/powl/inductive/variants/im_tree.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/discovery/powl/inductive/variants/maximal/__init__.py` & `pm4py-2.7.9.4/pm4py/algo/discovery/powl/inductive/variants/maximal/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/discovery/powl/inductive/variants/maximal/factory.py` & `pm4py-2.7.9.4/pm4py/algo/discovery/powl/inductive/variants/maximal/factory.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/discovery/powl/inductive/variants/maximal/maximal_partial_order_cut.py` & `pm4py-2.7.9.4/pm4py/algo/discovery/powl/inductive/variants/maximal/maximal_partial_order_cut.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/discovery/powl/inductive/variants/powl_discovery_varaints.py` & `pm4py-2.7.9.4/pm4py/algo/discovery/powl/inductive/variants/powl_discovery_varaints.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/discovery/temporal_profile/__init__.py` & `pm4py-2.7.9.4/pm4py/algo/discovery/temporal_profile/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/discovery/temporal_profile/algorithm.py` & `pm4py-2.7.9.4/pm4py/algo/discovery/temporal_profile/algorithm.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/discovery/temporal_profile/variants/__init__.py` & `pm4py-2.7.9.4/pm4py/algo/discovery/temporal_profile/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/discovery/temporal_profile/variants/dataframe.py` & `pm4py-2.7.9.4/pm4py/algo/discovery/temporal_profile/variants/dataframe.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/discovery/temporal_profile/variants/log.py` & `pm4py-2.7.9.4/pm4py/algo/discovery/temporal_profile/variants/log.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/discovery/transition_system/__init__.py` & `pm4py-2.7.9.4/pm4py/algo/discovery/transition_system/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/discovery/transition_system/algorithm.py` & `pm4py-2.7.9.4/pm4py/algo/discovery/transition_system/algorithm.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/discovery/transition_system/variants/__init__.py` & `pm4py-2.7.9.4/pm4py/algo/discovery/transition_system/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/discovery/transition_system/variants/view_based.py` & `pm4py-2.7.9.4/pm4py/algo/discovery/transition_system/variants/view_based.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/evaluation/__init__.py` & `pm4py-2.7.9.4/pm4py/algo/evaluation/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/evaluation/algorithm.py` & `pm4py-2.7.9.4/pm4py/algo/evaluation/algorithm.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/evaluation/earth_mover_distance/__init__.py` & `pm4py-2.7.9.4/pm4py/algo/evaluation/earth_mover_distance/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/evaluation/earth_mover_distance/algorithm.py` & `pm4py-2.7.9.4/pm4py/algo/evaluation/earth_mover_distance/algorithm.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/evaluation/earth_mover_distance/variants/__init__.py` & `pm4py-2.7.9.4/pm4py/algo/evaluation/earth_mover_distance/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/evaluation/earth_mover_distance/variants/pyemd.py` & `pm4py-2.7.9.4/pm4py/algo/evaluation/earth_mover_distance/variants/pyemd.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/evaluation/generalization/__init__.py` & `pm4py-2.7.9.4/pm4py/algo/evaluation/generalization/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/evaluation/generalization/algorithm.py` & `pm4py-2.7.9.4/pm4py/algo/evaluation/generalization/algorithm.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/evaluation/generalization/variants/__init__.py` & `pm4py-2.7.9.4/pm4py/algo/evaluation/generalization/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/evaluation/generalization/variants/token_based.py` & `pm4py-2.7.9.4/pm4py/algo/evaluation/generalization/variants/token_based.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/evaluation/precision/__init__.py` & `pm4py-2.7.9.4/pm4py/algo/evaluation/precision/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/evaluation/precision/algorithm.py` & `pm4py-2.7.9.4/pm4py/algo/evaluation/precision/algorithm.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/evaluation/precision/dfg/__init__.py` & `pm4py-2.7.9.4/pm4py/algo/evaluation/precision/dfg/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/evaluation/precision/dfg/algorithm.py` & `pm4py-2.7.9.4/pm4py/algo/evaluation/precision/dfg/algorithm.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/evaluation/precision/utils.py` & `pm4py-2.7.9.4/pm4py/algo/evaluation/precision/utils.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/evaluation/precision/variants/__init__.py` & `pm4py-2.7.9.4/pm4py/algo/evaluation/precision/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/evaluation/precision/variants/align_etconformance.py` & `pm4py-2.7.9.4/pm4py/algo/evaluation/precision/variants/align_etconformance.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/evaluation/precision/variants/etconformance_token.py` & `pm4py-2.7.9.4/pm4py/algo/evaluation/precision/variants/etconformance_token.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/evaluation/replay_fitness/__init__.py` & `pm4py-2.7.9.4/pm4py/algo/evaluation/replay_fitness/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/evaluation/replay_fitness/algorithm.py` & `pm4py-2.7.9.4/pm4py/algo/evaluation/replay_fitness/algorithm.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/evaluation/replay_fitness/variants/__init__.py` & `pm4py-2.7.9.4/pm4py/algo/evaluation/replay_fitness/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/evaluation/replay_fitness/variants/alignment_based.py` & `pm4py-2.7.9.4/pm4py/algo/evaluation/replay_fitness/variants/alignment_based.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/evaluation/replay_fitness/variants/token_replay.py` & `pm4py-2.7.9.4/pm4py/algo/evaluation/replay_fitness/variants/token_replay.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/evaluation/simplicity/__init__.py` & `pm4py-2.7.9.4/pm4py/algo/evaluation/simplicity/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/evaluation/simplicity/algorithm.py` & `pm4py-2.7.9.4/pm4py/algo/evaluation/simplicity/algorithm.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/evaluation/simplicity/variants/__init__.py` & `pm4py-2.7.9.4/pm4py/algo/evaluation/simplicity/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/evaluation/simplicity/variants/arc_degree.py` & `pm4py-2.7.9.4/pm4py/algo/evaluation/simplicity/variants/arc_degree.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/evaluation/simplicity/variants/extended_cardoso.py` & `pm4py-2.7.9.4/pm4py/algo/evaluation/simplicity/variants/extended_cardoso.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/evaluation/simplicity/variants/extended_cyclomatic.py` & `pm4py-2.7.9.4/pm4py/algo/evaluation/simplicity/variants/extended_cyclomatic.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/filtering/__init__.py` & `pm4py-2.7.9.4/pm4py/algo/filtering/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/filtering/common/__init__.py` & `pm4py-2.7.9.4/pm4py/algo/filtering/common/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/filtering/common/attributes/__init__.py` & `pm4py-2.7.9.4/pm4py/algo/filtering/common/attributes/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/filtering/common/attributes/attributes_common.py` & `pm4py-2.7.9.4/pm4py/algo/filtering/common/attributes/attributes_common.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/filtering/common/end_activities/__init__.py` & `pm4py-2.7.9.4/pm4py/algo/filtering/common/end_activities/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/filtering/common/end_activities/end_activities_common.py` & `pm4py-2.7.9.4/pm4py/algo/filtering/common/end_activities/end_activities_common.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/filtering/common/filtering_constants.py` & `pm4py-2.7.9.4/pm4py/algo/filtering/common/filtering_constants.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/filtering/common/start_activities/__init__.py` & `pm4py-2.7.9.4/pm4py/algo/filtering/common/start_activities/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/filtering/common/start_activities/start_activities_common.py` & `pm4py-2.7.9.4/pm4py/algo/filtering/common/start_activities/start_activities_common.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/filtering/common/timestamp/__init__.py` & `pm4py-2.7.9.4/pm4py/algo/filtering/common/timestamp/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/filtering/common/timestamp/timestamp_common.py` & `pm4py-2.7.9.4/pm4py/algo/filtering/common/timestamp/timestamp_common.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/filtering/common/traces/__init__.py` & `pm4py-2.7.9.4/pm4py/algo/filtering/common/traces/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/filtering/common/traces/infix_to_regex.py` & `pm4py-2.7.9.4/pm4py/algo/filtering/common/traces/infix_to_regex.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/filtering/dfg/__init__.py` & `pm4py-2.7.9.4/pm4py/algo/filtering/dfg/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/filtering/dfg/dfg_filtering.py` & `pm4py-2.7.9.4/pm4py/algo/filtering/dfg/dfg_filtering.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/filtering/log/__init__.py` & `pm4py-2.7.9.4/pm4py/algo/filtering/log/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/filtering/log/attr_value_repetition/__init__.py` & `pm4py-2.7.9.4/pm4py/algo/filtering/log/attr_value_repetition/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/filtering/log/attr_value_repetition/filter.py` & `pm4py-2.7.9.4/pm4py/algo/filtering/log/attr_value_repetition/filter.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/filtering/log/attributes/__init__.py` & `pm4py-2.7.9.4/pm4py/algo/filtering/log/attributes/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/filtering/log/attributes/attributes_filter.py` & `pm4py-2.7.9.4/pm4py/algo/filtering/log/attributes/attributes_filter.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/filtering/log/between/__init__.py` & `pm4py-2.7.9.4/pm4py/algo/filtering/log/between/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/filtering/log/between/between_filter.py` & `pm4py-2.7.9.4/pm4py/algo/filtering/log/between/between_filter.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/filtering/log/cases/__init__.py` & `pm4py-2.7.9.4/pm4py/algo/filtering/log/cases/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/filtering/log/cases/case_filter.py` & `pm4py-2.7.9.4/pm4py/algo/filtering/log/cases/case_filter.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/filtering/log/end_activities/__init__.py` & `pm4py-2.7.9.4/pm4py/algo/filtering/log/end_activities/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/filtering/log/end_activities/end_activities_filter.py` & `pm4py-2.7.9.4/pm4py/algo/filtering/log/end_activities/end_activities_filter.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/filtering/log/ltl/__init__.py` & `pm4py-2.7.9.4/pm4py/algo/filtering/log/ltl/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/filtering/log/ltl/ltl_checker.py` & `pm4py-2.7.9.4/pm4py/algo/filtering/log/ltl/ltl_checker.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/filtering/log/paths/__init__.py` & `pm4py-2.7.9.4/pm4py/algo/filtering/log/paths/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/filtering/log/paths/paths_filter.py` & `pm4py-2.7.9.4/pm4py/algo/filtering/log/paths/paths_filter.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/filtering/log/prefixes/__init__.py` & `pm4py-2.7.9.4/pm4py/algo/filtering/log/prefixes/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/filtering/log/prefixes/prefix_filter.py` & `pm4py-2.7.9.4/pm4py/algo/filtering/log/prefixes/prefix_filter.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/filtering/log/rework/__init__.py` & `pm4py-2.7.9.4/pm4py/algo/filtering/log/rework/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/filtering/log/rework/rework_filter.py` & `pm4py-2.7.9.4/pm4py/algo/filtering/log/rework/rework_filter.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/filtering/log/start_activities/__init__.py` & `pm4py-2.7.9.4/pm4py/algo/filtering/log/start_activities/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/filtering/log/start_activities/start_activities_filter.py` & `pm4py-2.7.9.4/pm4py/algo/filtering/log/start_activities/start_activities_filter.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/filtering/log/suffixes/__init__.py` & `pm4py-2.7.9.4/pm4py/algo/filtering/log/suffixes/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/filtering/log/suffixes/suffix_filter.py` & `pm4py-2.7.9.4/pm4py/algo/filtering/log/suffixes/suffix_filter.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/filtering/log/timestamp/__init__.py` & `pm4py-2.7.9.4/pm4py/algo/filtering/log/timestamp/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/filtering/log/timestamp/timestamp_filter.py` & `pm4py-2.7.9.4/pm4py/algo/filtering/log/timestamp/timestamp_filter.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/filtering/log/traces/__init__.py` & `pm4py-2.7.9.4/pm4py/algo/filtering/log/traces/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/filtering/log/traces/trace_filter.py` & `pm4py-2.7.9.4/pm4py/algo/filtering/log/traces/trace_filter.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/filtering/log/variants/__init__.py` & `pm4py-2.7.9.4/pm4py/algo/filtering/log/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/filtering/log/variants/variants_filter.py` & `pm4py-2.7.9.4/pm4py/algo/filtering/log/variants/variants_filter.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/filtering/ocel/__init__.py` & `pm4py-2.7.9.4/pm4py/algo/filtering/ocel/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/filtering/ocel/activity_type_matching.py` & `pm4py-2.7.9.4/pm4py/algo/filtering/ocel/activity_type_matching.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/filtering/ocel/event_attributes.py` & `pm4py-2.7.9.4/pm4py/algo/filtering/ocel/event_attributes.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/filtering/ocel/object_attributes.py` & `pm4py-2.7.9.4/pm4py/algo/filtering/ocel/object_attributes.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/filtering/ocel/objects_ot_count.py` & `pm4py-2.7.9.4/pm4py/algo/filtering/ocel/objects_ot_count.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/filtering/ocel/ot_endpoints.py` & `pm4py-2.7.9.4/pm4py/algo/filtering/ocel/ot_endpoints.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/filtering/pandas/__init__.py` & `pm4py-2.7.9.4/pm4py/algo/filtering/pandas/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/filtering/pandas/attr_value_repetition/__init__.py` & `pm4py-2.7.9.4/pm4py/algo/filtering/pandas/attr_value_repetition/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/filtering/pandas/attr_value_repetition/filter.py` & `pm4py-2.7.9.4/pm4py/algo/filtering/pandas/attr_value_repetition/filter.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/filtering/pandas/attributes/__init__.py` & `pm4py-2.7.9.4/pm4py/algo/filtering/pandas/attributes/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/filtering/pandas/attributes/attributes_filter.py` & `pm4py-2.7.9.4/pm4py/algo/filtering/pandas/attributes/attributes_filter.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/filtering/pandas/between/__init__.py` & `pm4py-2.7.9.4/pm4py/algo/filtering/pandas/between/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/filtering/pandas/between/between_filter.py` & `pm4py-2.7.9.4/pm4py/algo/filtering/pandas/between/between_filter.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/filtering/pandas/cases/__init__.py` & `pm4py-2.7.9.4/pm4py/algo/filtering/pandas/cases/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/filtering/pandas/cases/case_filter.py` & `pm4py-2.7.9.4/pm4py/algo/filtering/pandas/cases/case_filter.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/filtering/pandas/consecutive_act_case_grouping/__init__.py` & `pm4py-2.7.9.4/pm4py/algo/filtering/pandas/consecutive_act_case_grouping/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/filtering/pandas/consecutive_act_case_grouping/consecutive_act_case_grouping_filter.py` & `pm4py-2.7.9.4/pm4py/algo/filtering/pandas/consecutive_act_case_grouping/consecutive_act_case_grouping_filter.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/filtering/pandas/end_activities/__init__.py` & `pm4py-2.7.9.4/pm4py/algo/filtering/pandas/end_activities/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/filtering/pandas/end_activities/end_activities_filter.py` & `pm4py-2.7.9.4/pm4py/algo/filtering/pandas/end_activities/end_activities_filter.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/filtering/pandas/ends_with/__init__.py` & `pm4py-2.7.9.4/pm4py/algo/filtering/pandas/ends_with/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/filtering/pandas/ends_with/ends_with_filter.py` & `pm4py-2.7.9.4/pm4py/algo/filtering/pandas/ends_with/ends_with_filter.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/filtering/pandas/ltl/__init__.py` & `pm4py-2.7.9.4/pm4py/algo/filtering/pandas/ltl/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/filtering/pandas/ltl/ltl_checker.py` & `pm4py-2.7.9.4/pm4py/algo/filtering/pandas/ltl/ltl_checker.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/filtering/pandas/paths/__init__.py` & `pm4py-2.7.9.4/pm4py/algo/filtering/pandas/paths/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/filtering/pandas/paths/paths_filter.py` & `pm4py-2.7.9.4/pm4py/algo/filtering/pandas/paths/paths_filter.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/filtering/pandas/pd_filtering_constants.py` & `pm4py-2.7.9.4/pm4py/algo/filtering/pandas/pd_filtering_constants.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/filtering/pandas/prefixes/__init__.py` & `pm4py-2.7.9.4/pm4py/algo/filtering/pandas/prefixes/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/filtering/pandas/prefixes/prefix_filter.py` & `pm4py-2.7.9.4/pm4py/algo/filtering/pandas/prefixes/prefix_filter.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/filtering/pandas/rework/__init__.py` & `pm4py-2.7.9.4/pm4py/algo/filtering/pandas/rework/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/filtering/pandas/rework/rework_filter.py` & `pm4py-2.7.9.4/pm4py/algo/filtering/pandas/rework/rework_filter.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/filtering/pandas/start_activities/__init__.py` & `pm4py-2.7.9.4/pm4py/algo/filtering/pandas/start_activities/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/filtering/pandas/start_activities/start_activities_filter.py` & `pm4py-2.7.9.4/pm4py/algo/filtering/pandas/start_activities/start_activities_filter.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/filtering/pandas/starts_with/__init__.py` & `pm4py-2.7.9.4/pm4py/algo/filtering/pandas/starts_with/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/filtering/pandas/starts_with/starts_with_filter.py` & `pm4py-2.7.9.4/pm4py/algo/filtering/pandas/starts_with/starts_with_filter.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/filtering/pandas/suffixes/__init__.py` & `pm4py-2.7.9.4/pm4py/algo/filtering/pandas/suffixes/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/filtering/pandas/suffixes/suffix_filter.py` & `pm4py-2.7.9.4/pm4py/algo/filtering/pandas/suffixes/suffix_filter.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/filtering/pandas/timestamp/__init__.py` & `pm4py-2.7.9.4/pm4py/algo/filtering/pandas/timestamp/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/filtering/pandas/timestamp/timestamp_filter.py` & `pm4py-2.7.9.4/pm4py/algo/filtering/pandas/timestamp/timestamp_filter.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/filtering/pandas/timestamp_case_grouping/__init__.py` & `pm4py-2.7.9.4/pm4py/algo/filtering/pandas/timestamp_case_grouping/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/filtering/pandas/timestamp_case_grouping/timestamp_case_grouping_filter.py` & `pm4py-2.7.9.4/pm4py/algo/filtering/pandas/timestamp_case_grouping/timestamp_case_grouping_filter.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/filtering/pandas/traces/__init__.py` & `pm4py-2.7.9.4/pm4py/algo/filtering/pandas/traces/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/filtering/pandas/traces/trace_filter.py` & `pm4py-2.7.9.4/pm4py/algo/filtering/pandas/traces/trace_filter.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/filtering/pandas/variants/__init__.py` & `pm4py-2.7.9.4/pm4py/algo/filtering/pandas/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/filtering/pandas/variants/variants_filter.py` & `pm4py-2.7.9.4/pm4py/algo/filtering/pandas/variants/variants_filter.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/label_splitting/__init__.py` & `pm4py-2.7.9.4/pm4py/algo/label_splitting/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/label_splitting/algorithm.py` & `pm4py-2.7.9.4/pm4py/algo/label_splitting/algorithm.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/label_splitting/variants/__init__.py` & `pm4py-2.7.9.4/pm4py/algo/label_splitting/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/label_splitting/variants/contextual.py` & `pm4py-2.7.9.4/pm4py/algo/label_splitting/variants/contextual.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/merging/__init__.py` & `pm4py-2.7.9.4/pm4py/algo/merging/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/merging/case_relations/__init__.py` & `pm4py-2.7.9.4/pm4py/algo/merging/case_relations/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/merging/case_relations/algorithm.py` & `pm4py-2.7.9.4/pm4py/algo/merging/case_relations/algorithm.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/merging/case_relations/variants/__init__.py` & `pm4py-2.7.9.4/pm4py/algo/merging/case_relations/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/merging/case_relations/variants/pandas.py` & `pm4py-2.7.9.4/pm4py/algo/merging/case_relations/variants/pandas.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/organizational_mining/__init__.py` & `pm4py-2.7.9.4/pm4py/algo/organizational_mining/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/organizational_mining/local_diagnostics/__init__.py` & `pm4py-2.7.9.4/pm4py/algo/organizational_mining/local_diagnostics/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/organizational_mining/local_diagnostics/algorithm.py` & `pm4py-2.7.9.4/pm4py/algo/organizational_mining/local_diagnostics/algorithm.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/organizational_mining/network_analysis/__init__.py` & `pm4py-2.7.9.4/pm4py/algo/organizational_mining/network_analysis/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/organizational_mining/network_analysis/algorithm.py` & `pm4py-2.7.9.4/pm4py/algo/organizational_mining/network_analysis/algorithm.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/organizational_mining/network_analysis/variants/__init__.py` & `pm4py-2.7.9.4/pm4py/algo/organizational_mining/network_analysis/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/organizational_mining/network_analysis/variants/dataframe.py` & `pm4py-2.7.9.4/pm4py/algo/organizational_mining/network_analysis/variants/dataframe.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/organizational_mining/resource_profiles/__init__.py` & `pm4py-2.7.9.4/pm4py/algo/organizational_mining/resource_profiles/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/organizational_mining/resource_profiles/algorithm.py` & `pm4py-2.7.9.4/pm4py/algo/organizational_mining/resource_profiles/algorithm.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/organizational_mining/resource_profiles/variants/__init__.py` & `pm4py-2.7.9.4/pm4py/algo/organizational_mining/resource_profiles/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/organizational_mining/resource_profiles/variants/log.py` & `pm4py-2.7.9.4/pm4py/algo/organizational_mining/resource_profiles/variants/log.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/organizational_mining/resource_profiles/variants/pandas.py` & `pm4py-2.7.9.4/pm4py/algo/organizational_mining/resource_profiles/variants/pandas.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/organizational_mining/roles/__init__.py` & `pm4py-2.7.9.4/pm4py/algo/organizational_mining/roles/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/organizational_mining/roles/algorithm.py` & `pm4py-2.7.9.4/pm4py/algo/organizational_mining/roles/algorithm.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/organizational_mining/roles/common/__init__.py` & `pm4py-2.7.9.4/pm4py/algo/organizational_mining/roles/common/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/organizational_mining/roles/common/algorithm.py` & `pm4py-2.7.9.4/pm4py/algo/organizational_mining/roles/common/algorithm.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/organizational_mining/roles/variants/__init__.py` & `pm4py-2.7.9.4/pm4py/algo/organizational_mining/roles/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/organizational_mining/roles/variants/log.py` & `pm4py-2.7.9.4/pm4py/algo/organizational_mining/roles/variants/log.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/organizational_mining/roles/variants/pandas.py` & `pm4py-2.7.9.4/pm4py/algo/organizational_mining/roles/variants/pandas.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/organizational_mining/sna/__init__.py` & `pm4py-2.7.9.4/pm4py/algo/organizational_mining/sna/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/organizational_mining/sna/algorithm.py` & `pm4py-2.7.9.4/pm4py/algo/organizational_mining/sna/algorithm.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/organizational_mining/sna/util.py` & `pm4py-2.7.9.4/pm4py/algo/organizational_mining/sna/util.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/organizational_mining/sna/variants/__init__.py` & `pm4py-2.7.9.4/pm4py/algo/organizational_mining/sna/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/organizational_mining/sna/variants/log/__init__.py` & `pm4py-2.7.9.4/pm4py/algo/organizational_mining/sna/variants/log/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/organizational_mining/sna/variants/log/handover.py` & `pm4py-2.7.9.4/pm4py/algo/organizational_mining/sna/variants/log/handover.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/organizational_mining/sna/variants/log/jointactivities.py` & `pm4py-2.7.9.4/pm4py/algo/organizational_mining/sna/variants/log/jointactivities.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/organizational_mining/sna/variants/log/subcontracting.py` & `pm4py-2.7.9.4/pm4py/algo/organizational_mining/sna/variants/log/subcontracting.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/organizational_mining/sna/variants/log/working_together.py` & `pm4py-2.7.9.4/pm4py/algo/organizational_mining/sna/variants/log/working_together.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/organizational_mining/sna/variants/pandas/__init__.py` & `pm4py-2.7.9.4/pm4py/algo/organizational_mining/sna/variants/pandas/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/organizational_mining/sna/variants/pandas/handover.py` & `pm4py-2.7.9.4/pm4py/algo/organizational_mining/sna/variants/pandas/handover.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/organizational_mining/sna/variants/pandas/jointactivities.py` & `pm4py-2.7.9.4/pm4py/algo/organizational_mining/sna/variants/pandas/jointactivities.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/organizational_mining/sna/variants/pandas/subcontracting.py` & `pm4py-2.7.9.4/pm4py/algo/organizational_mining/sna/variants/pandas/subcontracting.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/organizational_mining/sna/variants/pandas/working_together.py` & `pm4py-2.7.9.4/pm4py/algo/organizational_mining/sna/variants/pandas/working_together.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/organizational_mining/util.py` & `pm4py-2.7.9.4/pm4py/algo/organizational_mining/util.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/querying/__init__.py` & `pm4py-2.7.9.4/pm4py/algo/querying/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/querying/llm/__init__.py` & `pm4py-2.7.9.4/pm4py/algo/querying/llm/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/querying/llm/abstractions/__init__.py` & `pm4py-2.7.9.4/pm4py/algo/querying/llm/abstractions/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/querying/llm/abstractions/case_to_descr.py` & `pm4py-2.7.9.4/pm4py/algo/querying/llm/abstractions/case_to_descr.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/querying/llm/abstractions/declare_to_descr.py` & `pm4py-2.7.9.4/pm4py/algo/querying/llm/abstractions/declare_to_descr.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/querying/llm/abstractions/log_to_cols_descr.py` & `pm4py-2.7.9.4/pm4py/algo/querying/llm/abstractions/log_to_cols_descr.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/querying/llm/abstractions/log_to_dfg_descr.py` & `pm4py-2.7.9.4/pm4py/algo/querying/llm/abstractions/log_to_dfg_descr.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/querying/llm/abstractions/log_to_fea_descr.py` & `pm4py-2.7.9.4/pm4py/algo/querying/llm/abstractions/log_to_fea_descr.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/querying/llm/abstractions/log_to_variants_descr.py` & `pm4py-2.7.9.4/pm4py/algo/querying/llm/abstractions/log_to_variants_descr.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/querying/llm/abstractions/logske_to_descr.py` & `pm4py-2.7.9.4/pm4py/algo/querying/llm/abstractions/logske_to_descr.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/querying/llm/abstractions/net_to_descr.py` & `pm4py-2.7.9.4/pm4py/algo/querying/llm/abstractions/net_to_descr.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/querying/llm/abstractions/ocel_fea_descr.py` & `pm4py-2.7.9.4/pm4py/algo/querying/llm/abstractions/ocel_fea_descr.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/querying/llm/abstractions/ocel_ocdfg_descr.py` & `pm4py-2.7.9.4/pm4py/algo/querying/llm/abstractions/ocel_ocdfg_descr.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/querying/llm/abstractions/stream_to_descr.py` & `pm4py-2.7.9.4/pm4py/algo/querying/llm/abstractions/stream_to_descr.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/querying/llm/abstractions/tempprofile_to_descr.py` & `pm4py-2.7.9.4/pm4py/algo/querying/llm/abstractions/tempprofile_to_descr.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/querying/llm/connectors/__init__.py` & `pm4py-2.7.9.4/pm4py/algo/querying/llm/connectors/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/querying/llm/connectors/openai.py` & `pm4py-2.7.9.4/pm4py/algo/querying/llm/connectors/openai.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/querying/llm/utils/__init__.py` & `pm4py-2.7.9.4/pm4py/algo/querying/llm/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/querying/llm/utils/sql_utils.py` & `pm4py-2.7.9.4/pm4py/algo/querying/llm/utils/sql_utils.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/reduction/__init__.py` & `pm4py-2.7.9.4/pm4py/algo/reduction/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/reduction/process_tree/__init__.py` & `pm4py-2.7.9.4/pm4py/algo/reduction/process_tree/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/reduction/process_tree/reducer.py` & `pm4py-2.7.9.4/pm4py/algo/reduction/process_tree/reducer.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/reduction/process_tree/variants/__init__.py` & `pm4py-2.7.9.4/pm4py/algo/reduction/process_tree/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/reduction/process_tree/variants/tree_tr_based.py` & `pm4py-2.7.9.4/pm4py/algo/reduction/process_tree/variants/tree_tr_based.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/simulation/__init__.py` & `pm4py-2.7.9.4/pm4py/algo/simulation/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/simulation/montecarlo/__init__.py` & `pm4py-2.7.9.4/pm4py/algo/simulation/montecarlo/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/simulation/montecarlo/algorithm.py` & `pm4py-2.7.9.4/pm4py/algo/simulation/montecarlo/algorithm.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/simulation/montecarlo/utils/__init__.py` & `pm4py-2.7.9.4/pm4py/algo/simulation/montecarlo/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/simulation/montecarlo/utils/replay.py` & `pm4py-2.7.9.4/pm4py/algo/simulation/montecarlo/utils/replay.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/simulation/montecarlo/variants/__init__.py` & `pm4py-2.7.9.4/pm4py/algo/simulation/montecarlo/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/simulation/montecarlo/variants/petri_semaph_fifo.py` & `pm4py-2.7.9.4/pm4py/algo/simulation/montecarlo/variants/petri_semaph_fifo.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/simulation/playout/__init__.py` & `pm4py-2.7.9.4/pm4py/algo/simulation/playout/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/simulation/playout/dfg/__init__.py` & `pm4py-2.7.9.4/pm4py/algo/simulation/playout/dfg/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/simulation/playout/dfg/algorithm.py` & `pm4py-2.7.9.4/pm4py/algo/simulation/playout/dfg/algorithm.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/simulation/playout/dfg/variants/__init__.py` & `pm4py-2.7.9.4/pm4py/algo/simulation/playout/dfg/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/simulation/playout/dfg/variants/classic.py` & `pm4py-2.7.9.4/pm4py/algo/simulation/playout/dfg/variants/classic.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/simulation/playout/dfg/variants/performance.py` & `pm4py-2.7.9.4/pm4py/algo/simulation/playout/dfg/variants/performance.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/simulation/playout/petri_net/__init__.py` & `pm4py-2.7.9.4/pm4py/algo/simulation/playout/petri_net/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/simulation/playout/petri_net/algorithm.py` & `pm4py-2.7.9.4/pm4py/algo/simulation/playout/petri_net/algorithm.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/simulation/playout/petri_net/variants/__init__.py` & `pm4py-2.7.9.4/pm4py/algo/simulation/playout/petri_net/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/simulation/playout/petri_net/variants/basic_playout.py` & `pm4py-2.7.9.4/pm4py/algo/simulation/playout/petri_net/variants/basic_playout.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/simulation/playout/petri_net/variants/extensive.py` & `pm4py-2.7.9.4/pm4py/algo/simulation/playout/petri_net/variants/extensive.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/simulation/playout/petri_net/variants/stochastic_playout.py` & `pm4py-2.7.9.4/pm4py/algo/simulation/playout/petri_net/variants/stochastic_playout.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/simulation/playout/process_tree/__init__.py` & `pm4py-2.7.9.4/pm4py/algo/simulation/playout/process_tree/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/simulation/playout/process_tree/algorithm.py` & `pm4py-2.7.9.4/pm4py/algo/simulation/playout/process_tree/algorithm.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/simulation/playout/process_tree/variants/__init__.py` & `pm4py-2.7.9.4/pm4py/algo/simulation/playout/process_tree/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/simulation/playout/process_tree/variants/basic_playout.py` & `pm4py-2.7.9.4/pm4py/algo/simulation/playout/process_tree/variants/basic_playout.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/simulation/playout/process_tree/variants/extensive.py` & `pm4py-2.7.9.4/pm4py/algo/simulation/playout/process_tree/variants/extensive.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/simulation/playout/process_tree/variants/topbottom.py` & `pm4py-2.7.9.4/pm4py/algo/simulation/playout/process_tree/variants/topbottom.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/simulation/tree_generator/__init__.py` & `pm4py-2.7.9.4/pm4py/algo/simulation/tree_generator/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/simulation/tree_generator/algorithm.py` & `pm4py-2.7.9.4/pm4py/algo/simulation/tree_generator/algorithm.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/simulation/tree_generator/variants/__init__.py` & `pm4py-2.7.9.4/pm4py/algo/simulation/tree_generator/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/simulation/tree_generator/variants/basic.py` & `pm4py-2.7.9.4/pm4py/algo/simulation/tree_generator/variants/basic.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/simulation/tree_generator/variants/ptandloggenerator.py` & `pm4py-2.7.9.4/pm4py/algo/simulation/tree_generator/variants/ptandloggenerator.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/transformation/__init__.py` & `pm4py-2.7.9.4/pm4py/algo/transformation/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/transformation/log_to_features/__init__.py` & `pm4py-2.7.9.4/pm4py/algo/transformation/log_to_features/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/transformation/log_to_features/algorithm.py` & `pm4py-2.7.9.4/pm4py/algo/transformation/log_to_features/algorithm.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/transformation/log_to_features/util/__init__.py` & `pm4py-2.7.9.4/pm4py/algo/transformation/log_to_features/util/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/transformation/log_to_features/util/locally_linear_embedding.py` & `pm4py-2.7.9.4/pm4py/algo/transformation/log_to_features/util/locally_linear_embedding.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/transformation/log_to_features/variants/__init__.py` & `pm4py-2.7.9.4/pm4py/algo/transformation/log_to_features/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/transformation/log_to_features/variants/event_based.py` & `pm4py-2.7.9.4/pm4py/algo/transformation/log_to_features/variants/event_based.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/transformation/log_to_features/variants/temporal.py` & `pm4py-2.7.9.4/pm4py/algo/transformation/log_to_features/variants/temporal.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/transformation/log_to_features/variants/trace_based.py` & `pm4py-2.7.9.4/pm4py/algo/transformation/log_to_features/variants/trace_based.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/transformation/log_to_interval_tree/__init__.py` & `pm4py-2.7.9.4/pm4py/algo/transformation/log_to_interval_tree/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/transformation/log_to_interval_tree/algorithm.py` & `pm4py-2.7.9.4/pm4py/algo/transformation/log_to_interval_tree/algorithm.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/transformation/log_to_interval_tree/variants/__init__.py` & `pm4py-2.7.9.4/pm4py/algo/transformation/log_to_interval_tree/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/transformation/log_to_interval_tree/variants/open_paths.py` & `pm4py-2.7.9.4/pm4py/algo/transformation/log_to_interval_tree/variants/open_paths.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/transformation/log_to_target/__init__.py` & `pm4py-2.7.9.4/pm4py/algo/transformation/log_to_target/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/transformation/log_to_target/algorithm.py` & `pm4py-2.7.9.4/pm4py/algo/transformation/log_to_target/algorithm.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/transformation/log_to_target/variants/__init__.py` & `pm4py-2.7.9.4/pm4py/algo/transformation/log_to_target/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/transformation/log_to_target/variants/next_activity.py` & `pm4py-2.7.9.4/pm4py/algo/transformation/log_to_target/variants/next_activity.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/transformation/log_to_target/variants/next_time.py` & `pm4py-2.7.9.4/pm4py/algo/transformation/log_to_target/variants/next_time.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/transformation/log_to_target/variants/remaining_time.py` & `pm4py-2.7.9.4/pm4py/algo/transformation/log_to_target/variants/remaining_time.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/transformation/log_to_trie/__init__.py` & `pm4py-2.7.9.4/pm4py/algo/transformation/log_to_trie/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/transformation/log_to_trie/algorithm.py` & `pm4py-2.7.9.4/pm4py/algo/transformation/log_to_trie/algorithm.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/transformation/ocel/__init__.py` & `pm4py-2.7.9.4/pm4py/algo/transformation/ocel/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/transformation/ocel/description/__init__.py` & `pm4py-2.7.9.4/pm4py/algo/transformation/ocel/description/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/transformation/ocel/description/algorithm.py` & `pm4py-2.7.9.4/pm4py/algo/transformation/ocel/description/algorithm.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/transformation/ocel/description/variants/__init__.py` & `pm4py-2.7.9.4/pm4py/algo/transformation/ocel/description/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/transformation/ocel/description/variants/variant1.py` & `pm4py-2.7.9.4/pm4py/algo/transformation/ocel/description/variants/variant1.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/transformation/ocel/features/__init__.py` & `pm4py-2.7.9.4/pm4py/algo/transformation/ocel/features/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/transformation/ocel/features/events/__init__.py` & `pm4py-2.7.9.4/pm4py/algo/transformation/ocel/features/events/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/transformation/ocel/features/events/algorithm.py` & `pm4py-2.7.9.4/pm4py/algo/transformation/ocel/features/events/algorithm.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/transformation/ocel/features/events/event_activity.py` & `pm4py-2.7.9.4/pm4py/algo/transformation/ocel/features/events/event_activity.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/transformation/ocel/features/events/event_end_ot.py` & `pm4py-2.7.9.4/pm4py/algo/transformation/ocel/features/events/event_end_ot.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/transformation/ocel/features/events/event_num_attributes.py` & `pm4py-2.7.9.4/pm4py/algo/transformation/ocel/features/events/event_num_attributes.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/transformation/ocel/features/events/event_num_rel_objs.py` & `pm4py-2.7.9.4/pm4py/algo/transformation/ocel/features/events/event_num_rel_objs.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/transformation/ocel/features/events/event_num_rel_objs_type.py` & `pm4py-2.7.9.4/pm4py/algo/transformation/ocel/features/events/event_num_rel_objs_type.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/transformation/ocel/features/events/event_start_ot.py` & `pm4py-2.7.9.4/pm4py/algo/transformation/ocel/features/events/event_start_ot.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/transformation/ocel/features/events/event_str_attributes.py` & `pm4py-2.7.9.4/pm4py/algo/transformation/ocel/features/events/event_str_attributes.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/transformation/ocel/features/events/event_timestamp.py` & `pm4py-2.7.9.4/pm4py/algo/transformation/ocel/features/events/event_timestamp.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/transformation/ocel/features/events/new_interactions.py` & `pm4py-2.7.9.4/pm4py/algo/transformation/ocel/features/events/new_interactions.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/transformation/ocel/features/events/related_objects_features.py` & `pm4py-2.7.9.4/pm4py/algo/transformation/ocel/features/events/related_objects_features.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/transformation/ocel/features/events_objects/__init__.py` & `pm4py-2.7.9.4/pm4py/algo/transformation/ocel/features/events_objects/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/transformation/ocel/features/events_objects/algorithm.py` & `pm4py-2.7.9.4/pm4py/algo/transformation/ocel/features/events_objects/algorithm.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/transformation/ocel/features/events_objects/prefix_features.py` & `pm4py-2.7.9.4/pm4py/algo/transformation/ocel/features/events_objects/prefix_features.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/transformation/ocel/features/objects/__init__.py` & `pm4py-2.7.9.4/pm4py/algo/transformation/ocel/features/objects/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/transformation/ocel/features/objects/algorithm.py` & `pm4py-2.7.9.4/pm4py/algo/transformation/ocel/features/objects/algorithm.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/transformation/ocel/features/objects/obj_con_in_graph_features.py` & `pm4py-2.7.9.4/pm4py/algo/transformation/ocel/features/objects/obj_con_in_graph_features.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/transformation/ocel/features/objects/object_cobirth_graph.py` & `pm4py-2.7.9.4/pm4py/algo/transformation/ocel/features/objects/object_cobirth_graph.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/transformation/ocel/features/objects/object_codeath_graph.py` & `pm4py-2.7.9.4/pm4py/algo/transformation/ocel/features/objects/object_codeath_graph.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/transformation/ocel/features/objects/object_degree_centrality.py` & `pm4py-2.7.9.4/pm4py/algo/transformation/ocel/features/objects/object_degree_centrality.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/transformation/ocel/features/objects/object_general_descendants_graph.py` & `pm4py-2.7.9.4/pm4py/algo/transformation/ocel/features/objects/object_general_descendants_graph.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/transformation/ocel/features/objects/object_general_inheritance_graph.py` & `pm4py-2.7.9.4/pm4py/algo/transformation/ocel/features/objects/object_general_inheritance_graph.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/transformation/ocel/features/objects/object_general_interaction_graph.py` & `pm4py-2.7.9.4/pm4py/algo/transformation/ocel/features/objects/object_general_interaction_graph.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/transformation/ocel/features/objects/object_lifecycle_activities.py` & `pm4py-2.7.9.4/pm4py/algo/transformation/ocel/features/objects/object_lifecycle_activities.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/transformation/ocel/features/objects/object_lifecycle_duration.py` & `pm4py-2.7.9.4/pm4py/algo/transformation/ocel/features/objects/object_lifecycle_duration.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/transformation/ocel/features/objects/object_lifecycle_length.py` & `pm4py-2.7.9.4/pm4py/algo/transformation/ocel/features/objects/object_lifecycle_length.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/transformation/ocel/features/objects/object_lifecycle_paths.py` & `pm4py-2.7.9.4/pm4py/algo/transformation/ocel/features/objects/object_lifecycle_paths.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/transformation/ocel/features/objects/object_lifecycle_unq_act.py` & `pm4py-2.7.9.4/pm4py/algo/transformation/ocel/features/objects/object_lifecycle_unq_act.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/transformation/ocel/features/objects/object_num_attributes.py` & `pm4py-2.7.9.4/pm4py/algo/transformation/ocel/features/objects/object_num_attributes.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/transformation/ocel/features/objects/object_str_attributes.py` & `pm4py-2.7.9.4/pm4py/algo/transformation/ocel/features/objects/object_str_attributes.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/transformation/ocel/features/objects/object_work_in_progress.py` & `pm4py-2.7.9.4/pm4py/algo/transformation/ocel/features/objects/object_work_in_progress.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/transformation/ocel/features/objects/objects_interaction_graph_ot.py` & `pm4py-2.7.9.4/pm4py/algo/transformation/ocel/features/objects/objects_interaction_graph_ot.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/transformation/ocel/features/objects/related_activities_features.py` & `pm4py-2.7.9.4/pm4py/algo/transformation/ocel/features/objects/related_activities_features.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/transformation/ocel/features/objects/related_events_features.py` & `pm4py-2.7.9.4/pm4py/algo/transformation/ocel/features/objects/related_events_features.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/transformation/ocel/graphs/__init__.py` & `pm4py-2.7.9.4/pm4py/algo/transformation/ocel/graphs/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/transformation/ocel/graphs/object_cobirth_graph.py` & `pm4py-2.7.9.4/pm4py/algo/transformation/ocel/graphs/object_cobirth_graph.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/transformation/ocel/graphs/object_codeath_graph.py` & `pm4py-2.7.9.4/pm4py/algo/transformation/ocel/graphs/object_codeath_graph.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/transformation/ocel/graphs/object_descendants_graph.py` & `pm4py-2.7.9.4/pm4py/algo/transformation/ocel/graphs/object_descendants_graph.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/transformation/ocel/graphs/object_inheritance_graph.py` & `pm4py-2.7.9.4/pm4py/algo/transformation/ocel/graphs/object_inheritance_graph.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/transformation/ocel/graphs/object_interaction_graph.py` & `pm4py-2.7.9.4/pm4py/algo/transformation/ocel/graphs/object_interaction_graph.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/transformation/ocel/graphs/ocel20_computation.py` & `pm4py-2.7.9.4/pm4py/algo/transformation/ocel/graphs/ocel20_computation.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/transformation/ocel/split_ocel/__init__.py` & `pm4py-2.7.9.4/pm4py/algo/transformation/ocel/split_ocel/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/transformation/ocel/split_ocel/algorithm.py` & `pm4py-2.7.9.4/pm4py/algo/transformation/ocel/split_ocel/algorithm.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/transformation/ocel/split_ocel/variants/__init__.py` & `pm4py-2.7.9.4/pm4py/algo/transformation/ocel/split_ocel/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/transformation/ocel/split_ocel/variants/ancestors_descendants.py` & `pm4py-2.7.9.4/pm4py/algo/transformation/ocel/split_ocel/variants/ancestors_descendants.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/algo/transformation/ocel/split_ocel/variants/connected_components.py` & `pm4py-2.7.9.4/pm4py/algo/transformation/ocel/split_ocel/variants/connected_components.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/analysis.py` & `pm4py-2.7.9.4/pm4py/analysis.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/cli.py` & `pm4py-2.7.9.4/pm4py/cli.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/conformance.py` & `pm4py-2.7.9.4/pm4py/conformance.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/connectors.py` & `pm4py-2.7.9.4/pm4py/connectors.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/convert.py` & `pm4py-2.7.9.4/pm4py/convert.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/discovery.py` & `pm4py-2.7.9.4/pm4py/discovery.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/filtering.py` & `pm4py-2.7.9.4/pm4py/filtering.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/hof.py` & `pm4py-2.7.9.4/pm4py/hof.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/llm.py` & `pm4py-2.7.9.4/pm4py/llm.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/meta.py` & `pm4py-2.7.9.4/pm4py/meta.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,14 +12,14 @@
     GNU General Public License for more details.
 
     You should have received a copy of the GNU General Public License
     along with PM4Py.  If not, see <https://www.gnu.org/licenses/>.
 '''
 
 __name__ = 'pm4py'
-VERSION = '2.7.9.3'
+VERSION = '2.7.9.4'
 __version__ = VERSION
 __doc__ = 'Process mining for Python'
 __author__ = 'Fraunhofer Institute for Applied Information Technology FIT'
 __author_email__ = 'pm4py@fit.fraunhofer.de'
 __maintainer__ = 'Fraunhofer Institute for Applied Information Technology FIT'
 __maintainer_email__ = "pm4py@fit.fraunhofer.de"
```

### Comparing `pm4py-2.7.9.3/pm4py/ml.py` & `pm4py-2.7.9.4/pm4py/ml.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/objects/__init__.py` & `pm4py-2.7.9.4/pm4py/objects/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/objects/bpmn/__init__.py` & `pm4py-2.7.9.4/pm4py/objects/bpmn/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/objects/bpmn/exporter/__init__.py` & `pm4py-2.7.9.4/pm4py/objects/bpmn/exporter/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/objects/bpmn/exporter/exporter.py` & `pm4py-2.7.9.4/pm4py/objects/bpmn/exporter/exporter.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/objects/bpmn/exporter/variants/__init__.py` & `pm4py-2.7.9.4/pm4py/objects/bpmn/exporter/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/objects/bpmn/exporter/variants/etree.py` & `pm4py-2.7.9.4/pm4py/objects/bpmn/exporter/variants/etree.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/objects/bpmn/importer/__init__.py` & `pm4py-2.7.9.4/pm4py/objects/bpmn/importer/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/objects/bpmn/importer/importer.py` & `pm4py-2.7.9.4/pm4py/objects/bpmn/importer/importer.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/objects/bpmn/importer/variants/__init__.py` & `pm4py-2.7.9.4/pm4py/objects/bpmn/importer/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/objects/bpmn/importer/variants/lxml.py` & `pm4py-2.7.9.4/pm4py/objects/bpmn/importer/variants/lxml.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/objects/bpmn/layout/__init__.py` & `pm4py-2.7.9.4/pm4py/objects/bpmn/layout/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/objects/bpmn/layout/layouter.py` & `pm4py-2.7.9.4/pm4py/objects/bpmn/layout/layouter.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/objects/bpmn/layout/variants/__init__.py` & `pm4py-2.7.9.4/pm4py/objects/bpmn/layout/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/objects/bpmn/layout/variants/graphviz.py` & `pm4py-2.7.9.4/pm4py/objects/bpmn/layout/variants/graphviz.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/objects/bpmn/obj.py` & `pm4py-2.7.9.4/pm4py/objects/bpmn/obj.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/objects/bpmn/semantics.py` & `pm4py-2.7.9.4/pm4py/objects/bpmn/semantics.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/objects/bpmn/util/__init__.py` & `pm4py-2.7.9.4/pm4py/objects/bpmn/util/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/objects/bpmn/util/bpmn_utils.py` & `pm4py-2.7.9.4/pm4py/objects/bpmn/util/bpmn_utils.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/objects/bpmn/util/reduction.py` & `pm4py-2.7.9.4/pm4py/objects/bpmn/util/reduction.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/objects/bpmn/util/sorting.py` & `pm4py-2.7.9.4/pm4py/objects/bpmn/util/sorting.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/objects/conversion/__init__.py` & `pm4py-2.7.9.4/pm4py/objects/conversion/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/objects/conversion/bpmn/__init__.py` & `pm4py-2.7.9.4/pm4py/objects/conversion/bpmn/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/objects/conversion/bpmn/converter.py` & `pm4py-2.7.9.4/pm4py/objects/conversion/bpmn/converter.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/objects/conversion/bpmn/variants/__init__.py` & `pm4py-2.7.9.4/pm4py/objects/conversion/bpmn/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/objects/conversion/bpmn/variants/to_petri_net.py` & `pm4py-2.7.9.4/pm4py/objects/conversion/bpmn/variants/to_petri_net.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/objects/conversion/dfg/__init__.py` & `pm4py-2.7.9.4/pm4py/objects/conversion/dfg/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/objects/conversion/dfg/converter.py` & `pm4py-2.7.9.4/pm4py/objects/conversion/dfg/converter.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/objects/conversion/dfg/variants/__init__.py` & `pm4py-2.7.9.4/pm4py/objects/conversion/dfg/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/objects/conversion/dfg/variants/to_petri_net_activity_defines_place.py` & `pm4py-2.7.9.4/pm4py/objects/conversion/dfg/variants/to_petri_net_activity_defines_place.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/objects/conversion/dfg/variants/to_petri_net_invisibles_no_duplicates.py` & `pm4py-2.7.9.4/pm4py/objects/conversion/dfg/variants/to_petri_net_invisibles_no_duplicates.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/objects/conversion/heuristics_net/__init__.py` & `pm4py-2.7.9.4/pm4py/objects/conversion/heuristics_net/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/objects/conversion/heuristics_net/converter.py` & `pm4py-2.7.9.4/pm4py/objects/conversion/heuristics_net/converter.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/objects/conversion/heuristics_net/variants/__init__.py` & `pm4py-2.7.9.4/pm4py/objects/conversion/heuristics_net/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/objects/conversion/heuristics_net/variants/to_petri_net.py` & `pm4py-2.7.9.4/pm4py/objects/conversion/heuristics_net/variants/to_petri_net.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/objects/conversion/log/__init__.py` & `pm4py-2.7.9.4/pm4py/objects/conversion/log/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/objects/conversion/log/constants.py` & `pm4py-2.7.9.4/pm4py/objects/conversion/log/constants.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/objects/conversion/log/converter.py` & `pm4py-2.7.9.4/pm4py/objects/conversion/log/converter.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/objects/conversion/log/variants/__init__.py` & `pm4py-2.7.9.4/pm4py/objects/conversion/log/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/objects/conversion/log/variants/df_to_event_log_1v.py` & `pm4py-2.7.9.4/pm4py/objects/conversion/log/variants/df_to_event_log_1v.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/objects/conversion/log/variants/df_to_event_log_nv.py` & `pm4py-2.7.9.4/pm4py/objects/conversion/log/variants/df_to_event_log_nv.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/objects/conversion/log/variants/to_data_frame.py` & `pm4py-2.7.9.4/pm4py/objects/conversion/log/variants/to_data_frame.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/objects/conversion/log/variants/to_event_log.py` & `pm4py-2.7.9.4/pm4py/objects/conversion/log/variants/to_event_log.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/objects/conversion/log/variants/to_event_stream.py` & `pm4py-2.7.9.4/pm4py/objects/conversion/log/variants/to_event_stream.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/objects/conversion/log/variants/to_nx.py` & `pm4py-2.7.9.4/pm4py/objects/conversion/log/variants/to_nx.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/objects/conversion/ocel/__init__.py` & `pm4py-2.7.9.4/pm4py/objects/conversion/ocel/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/objects/conversion/ocel/converter.py` & `pm4py-2.7.9.4/pm4py/objects/conversion/ocel/converter.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/objects/conversion/ocel/variants/__init__.py` & `pm4py-2.7.9.4/pm4py/objects/conversion/ocel/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/objects/conversion/ocel/variants/ocel_features_to_nx.py` & `pm4py-2.7.9.4/pm4py/objects/conversion/ocel/variants/ocel_features_to_nx.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/objects/conversion/ocel/variants/ocel_to_nx.py` & `pm4py-2.7.9.4/pm4py/objects/conversion/ocel/variants/ocel_to_nx.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/objects/conversion/powl/__init__.py` & `pm4py-2.7.9.4/pm4py/objects/conversion/powl/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/objects/conversion/powl/converter.py` & `pm4py-2.7.9.4/pm4py/objects/conversion/powl/converter.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/objects/conversion/powl/variants/__init__.py` & `pm4py-2.7.9.4/pm4py/objects/conversion/powl/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/objects/conversion/powl/variants/to_petri_net.py` & `pm4py-2.7.9.4/pm4py/objects/conversion/powl/variants/to_petri_net.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/objects/conversion/process_tree/__init__.py` & `pm4py-2.7.9.4/pm4py/objects/conversion/process_tree/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/objects/conversion/process_tree/converter.py` & `pm4py-2.7.9.4/pm4py/objects/conversion/process_tree/converter.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/objects/conversion/process_tree/variants/__init__.py` & `pm4py-2.7.9.4/pm4py/objects/conversion/process_tree/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/objects/conversion/process_tree/variants/to_bpmn.py` & `pm4py-2.7.9.4/pm4py/objects/conversion/process_tree/variants/to_bpmn.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/objects/conversion/process_tree/variants/to_petri_net.py` & `pm4py-2.7.9.4/pm4py/objects/conversion/process_tree/variants/to_petri_net.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/objects/conversion/process_tree/variants/to_petri_net_transition_bordered.py` & `pm4py-2.7.9.4/pm4py/objects/conversion/process_tree/variants/to_petri_net_transition_bordered.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/objects/conversion/wf_net/__init__.py` & `pm4py-2.7.9.4/pm4py/objects/conversion/wf_net/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/objects/conversion/wf_net/converter.py` & `pm4py-2.7.9.4/pm4py/objects/conversion/wf_net/converter.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/objects/conversion/wf_net/variants/__init__.py` & `pm4py-2.7.9.4/pm4py/objects/conversion/wf_net/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/objects/conversion/wf_net/variants/to_bpmn.py` & `pm4py-2.7.9.4/pm4py/objects/conversion/wf_net/variants/to_bpmn.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/objects/conversion/wf_net/variants/to_process_tree.py` & `pm4py-2.7.9.4/pm4py/objects/conversion/wf_net/variants/to_process_tree.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/objects/dfg/__init__.py` & `pm4py-2.7.9.4/pm4py/objects/dfg/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/objects/dfg/exporter/__init__.py` & `pm4py-2.7.9.4/pm4py/objects/dfg/exporter/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/objects/dfg/exporter/exporter.py` & `pm4py-2.7.9.4/pm4py/objects/dfg/exporter/exporter.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/objects/dfg/exporter/variants/__init__.py` & `pm4py-2.7.9.4/pm4py/objects/dfg/exporter/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/objects/dfg/exporter/variants/classic.py` & `pm4py-2.7.9.4/pm4py/objects/dfg/exporter/variants/classic.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/objects/dfg/filtering/__init__.py` & `pm4py-2.7.9.4/pm4py/objects/dfg/filtering/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/objects/dfg/filtering/dfg_filtering.py` & `pm4py-2.7.9.4/pm4py/objects/dfg/filtering/dfg_filtering.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/objects/dfg/importer/__init__.py` & `pm4py-2.7.9.4/pm4py/objects/dfg/importer/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/objects/dfg/importer/importer.py` & `pm4py-2.7.9.4/pm4py/objects/dfg/importer/importer.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/objects/dfg/importer/variants/__init__.py` & `pm4py-2.7.9.4/pm4py/objects/dfg/importer/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/objects/dfg/importer/variants/classic.py` & `pm4py-2.7.9.4/pm4py/objects/dfg/importer/variants/classic.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/objects/dfg/obj.py` & `pm4py-2.7.9.4/pm4py/objects/dfg/obj.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/objects/dfg/retrieval/__init__.py` & `pm4py-2.7.9.4/pm4py/objects/dfg/retrieval/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/objects/dfg/retrieval/log.py` & `pm4py-2.7.9.4/pm4py/objects/dfg/retrieval/log.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/objects/dfg/retrieval/pandas.py` & `pm4py-2.7.9.4/pm4py/objects/dfg/retrieval/pandas.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/objects/dfg/util.py` & `pm4py-2.7.9.4/pm4py/objects/dfg/util.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/objects/dfg/utils/__init__.py` & `pm4py-2.7.9.4/pm4py/objects/dfg/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/objects/dfg/utils/dfg_utils.py` & `pm4py-2.7.9.4/pm4py/objects/dfg/utils/dfg_utils.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/objects/heuristics_net/__init__.py` & `pm4py-2.7.9.4/pm4py/objects/heuristics_net/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/objects/heuristics_net/defaults.py` & `pm4py-2.7.9.4/pm4py/objects/heuristics_net/defaults.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/objects/heuristics_net/edge.py` & `pm4py-2.7.9.4/pm4py/objects/heuristics_net/edge.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/objects/heuristics_net/node.py` & `pm4py-2.7.9.4/pm4py/objects/heuristics_net/node.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/objects/heuristics_net/obj.py` & `pm4py-2.7.9.4/pm4py/objects/heuristics_net/obj.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/objects/log/__init__.py` & `pm4py-2.7.9.4/pm4py/objects/log/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/objects/log/exporter/__init__.py` & `pm4py-2.7.9.4/pm4py/objects/log/exporter/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/objects/log/exporter/xes/__init__.py` & `pm4py-2.7.9.4/pm4py/objects/log/exporter/xes/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/objects/log/exporter/xes/exporter.py` & `pm4py-2.7.9.4/pm4py/objects/log/exporter/xes/exporter.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/objects/log/exporter/xes/util/__init__.py` & `pm4py-2.7.9.4/pm4py/objects/log/exporter/xes/util/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/objects/log/exporter/xes/util/compression.py` & `pm4py-2.7.9.4/pm4py/objects/log/exporter/xes/util/compression.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/objects/log/exporter/xes/variants/__init__.py` & `pm4py-2.7.9.4/pm4py/objects/log/exporter/xes/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/objects/log/exporter/xes/variants/etree_xes_exp.py` & `pm4py-2.7.9.4/pm4py/objects/log/exporter/xes/variants/etree_xes_exp.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/objects/log/exporter/xes/variants/line_by_line.py` & `pm4py-2.7.9.4/pm4py/objects/log/exporter/xes/variants/line_by_line.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/objects/log/importer/__init__.py` & `pm4py-2.7.9.4/pm4py/objects/log/importer/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/objects/log/importer/xes/__init__.py` & `pm4py-2.7.9.4/pm4py/objects/log/importer/xes/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/objects/log/importer/xes/importer.py` & `pm4py-2.7.9.4/pm4py/objects/log/importer/xes/importer.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/objects/log/importer/xes/variants/__init__.py` & `pm4py-2.7.9.4/pm4py/objects/log/importer/xes/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/objects/log/importer/xes/variants/chunk_regex.py` & `pm4py-2.7.9.4/pm4py/objects/log/importer/xes/variants/chunk_regex.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/objects/log/importer/xes/variants/iterparse.py` & `pm4py-2.7.9.4/pm4py/objects/log/importer/xes/variants/iterparse.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/objects/log/importer/xes/variants/iterparse_20.py` & `pm4py-2.7.9.4/pm4py/objects/log/importer/xes/variants/iterparse_20.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/objects/log/importer/xes/variants/iterparse_mem_compressed.py` & `pm4py-2.7.9.4/pm4py/objects/log/importer/xes/variants/iterparse_mem_compressed.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/objects/log/importer/xes/variants/line_by_line.py` & `pm4py-2.7.9.4/pm4py/objects/log/importer/xes/variants/line_by_line.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/objects/log/importer/xes/variants/rustxes.py` & `pm4py-2.7.9.4/pm4py/objects/log/importer/xes/variants/rustxes.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/objects/log/obj.py` & `pm4py-2.7.9.4/pm4py/objects/log/obj.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/objects/log/util/__init__.py` & `pm4py-2.7.9.4/pm4py/objects/log/util/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/objects/log/util/activities_to_alphabet.py` & `pm4py-2.7.9.4/pm4py/objects/log/util/activities_to_alphabet.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/objects/log/util/artificial.py` & `pm4py-2.7.9.4/pm4py/objects/log/util/artificial.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/objects/log/util/basic_filter.py` & `pm4py-2.7.9.4/pm4py/objects/log/util/basic_filter.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/objects/log/util/dataframe_utils.py` & `pm4py-2.7.9.4/pm4py/objects/log/util/dataframe_utils.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/objects/log/util/filtering_utils.py` & `pm4py-2.7.9.4/pm4py/objects/log/util/filtering_utils.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/objects/log/util/get_class_representation.py` & `pm4py-2.7.9.4/pm4py/objects/log/util/get_class_representation.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/objects/log/util/get_log_encoded.py` & `pm4py-2.7.9.4/pm4py/objects/log/util/get_log_encoded.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/objects/log/util/get_prefixes.py` & `pm4py-2.7.9.4/pm4py/objects/log/util/get_prefixes.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/objects/log/util/index_attribute.py` & `pm4py-2.7.9.4/pm4py/objects/log/util/index_attribute.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/objects/log/util/insert_classifier.py` & `pm4py-2.7.9.4/pm4py/objects/log/util/insert_classifier.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/objects/log/util/interval_lifecycle.py` & `pm4py-2.7.9.4/pm4py/objects/log/util/interval_lifecycle.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/objects/log/util/log.py` & `pm4py-2.7.9.4/pm4py/objects/log/util/log.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/objects/log/util/log_regex.py` & `pm4py-2.7.9.4/pm4py/objects/log/util/log_regex.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/objects/log/util/move_attrs_to_trace.py` & `pm4py-2.7.9.4/pm4py/objects/log/util/move_attrs_to_trace.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/objects/log/util/pandas_log_wrapper.py` & `pm4py-2.7.9.4/pm4py/objects/log/util/pandas_log_wrapper.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/objects/log/util/pandas_numpy_variants.py` & `pm4py-2.7.9.4/pm4py/objects/log/util/pandas_numpy_variants.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/objects/log/util/sampling.py` & `pm4py-2.7.9.4/pm4py/objects/log/util/sampling.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/objects/log/util/sorting.py` & `pm4py-2.7.9.4/pm4py/objects/log/util/sorting.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/objects/log/util/split_train_test.py` & `pm4py-2.7.9.4/pm4py/objects/log/util/split_train_test.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/objects/log/util/xes.py` & `pm4py-2.7.9.4/pm4py/objects/log/util/xes.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/objects/ocel/__init__.py` & `pm4py-2.7.9.4/pm4py/objects/ocel/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/objects/ocel/constants.py` & `pm4py-2.7.9.4/pm4py/objects/ocel/constants.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/objects/ocel/exporter/__init__.py` & `pm4py-2.7.9.4/pm4py/objects/ocel/exporter/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/objects/ocel/exporter/csv/__init__.py` & `pm4py-2.7.9.4/pm4py/objects/ocel/exporter/csv/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/objects/ocel/exporter/csv/exporter.py` & `pm4py-2.7.9.4/pm4py/objects/ocel/exporter/csv/exporter.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/objects/ocel/exporter/csv/variants/__init__.py` & `pm4py-2.7.9.4/pm4py/objects/ocel/exporter/csv/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/objects/ocel/exporter/csv/variants/pandas.py` & `pm4py-2.7.9.4/pm4py/objects/ocel/exporter/csv/variants/pandas.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/objects/ocel/exporter/jsonocel/__init__.py` & `pm4py-2.7.9.4/pm4py/objects/ocel/exporter/jsonocel/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/objects/ocel/exporter/jsonocel/exporter.py` & `pm4py-2.7.9.4/pm4py/objects/ocel/exporter/jsonocel/exporter.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/objects/ocel/exporter/jsonocel/variants/__init__.py` & `pm4py-2.7.9.4/pm4py/objects/ocel/exporter/jsonocel/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/objects/ocel/exporter/jsonocel/variants/classic.py` & `pm4py-2.7.9.4/pm4py/objects/ocel/exporter/jsonocel/variants/classic.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/objects/ocel/exporter/jsonocel/variants/ocel20.py` & `pm4py-2.7.9.4/pm4py/objects/ocel/exporter/jsonocel/variants/ocel20.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/objects/ocel/exporter/jsonocel/variants/ocel20_standard.py` & `pm4py-2.7.9.4/pm4py/objects/ocel/exporter/jsonocel/variants/ocel20_standard.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/objects/ocel/exporter/sqlite/__init__.py` & `pm4py-2.7.9.4/pm4py/objects/ocel/exporter/sqlite/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/objects/ocel/exporter/sqlite/exporter.py` & `pm4py-2.7.9.4/pm4py/objects/ocel/exporter/sqlite/exporter.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/objects/ocel/exporter/sqlite/variants/__init__.py` & `pm4py-2.7.9.4/pm4py/objects/ocel/exporter/sqlite/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/objects/ocel/exporter/sqlite/variants/ocel20.py` & `pm4py-2.7.9.4/pm4py/objects/ocel/exporter/sqlite/variants/ocel20.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/objects/ocel/exporter/sqlite/variants/pandas_exporter.py` & `pm4py-2.7.9.4/pm4py/objects/ocel/exporter/sqlite/variants/pandas_exporter.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/objects/ocel/exporter/util/__init__.py` & `pm4py-2.7.9.4/pm4py/objects/ocel/exporter/util/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/objects/ocel/exporter/util/clean_dataframes.py` & `pm4py-2.7.9.4/pm4py/objects/ocel/exporter/util/clean_dataframes.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/objects/ocel/exporter/xmlocel/__init__.py` & `pm4py-2.7.9.4/pm4py/objects/ocel/exporter/xmlocel/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/objects/ocel/exporter/xmlocel/exporter.py` & `pm4py-2.7.9.4/pm4py/objects/ocel/exporter/xmlocel/exporter.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/objects/ocel/exporter/xmlocel/variants/__init__.py` & `pm4py-2.7.9.4/pm4py/objects/ocel/exporter/xmlocel/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/objects/ocel/exporter/xmlocel/variants/classic.py` & `pm4py-2.7.9.4/pm4py/objects/ocel/exporter/xmlocel/variants/classic.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/objects/ocel/exporter/xmlocel/variants/ocel20.py` & `pm4py-2.7.9.4/pm4py/objects/ocel/exporter/xmlocel/variants/ocel20.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/objects/ocel/importer/__init__.py` & `pm4py-2.7.9.4/pm4py/objects/ocel/importer/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/objects/ocel/importer/csv/__init__.py` & `pm4py-2.7.9.4/pm4py/objects/ocel/importer/csv/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/objects/ocel/importer/csv/importer.py` & `pm4py-2.7.9.4/pm4py/objects/ocel/importer/csv/importer.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/objects/ocel/importer/csv/variants/__init__.py` & `pm4py-2.7.9.4/pm4py/objects/ocel/importer/csv/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/objects/ocel/importer/csv/variants/pandas.py` & `pm4py-2.7.9.4/pm4py/objects/ocel/importer/csv/variants/pandas.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/objects/ocel/importer/jsonocel/__init__.py` & `pm4py-2.7.9.4/pm4py/objects/ocel/importer/jsonocel/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/objects/ocel/importer/jsonocel/importer.py` & `pm4py-2.7.9.4/pm4py/objects/ocel/importer/jsonocel/importer.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/objects/ocel/importer/jsonocel/variants/__init__.py` & `pm4py-2.7.9.4/pm4py/objects/ocel/importer/jsonocel/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/objects/ocel/importer/jsonocel/variants/classic.py` & `pm4py-2.7.9.4/pm4py/objects/ocel/importer/jsonocel/variants/classic.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/objects/ocel/importer/jsonocel/variants/ocel20_standard.py` & `pm4py-2.7.9.4/pm4py/objects/ocel/importer/jsonocel/variants/ocel20_standard.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/objects/ocel/importer/sqlite/__init__.py` & `pm4py-2.7.9.4/pm4py/objects/ocel/importer/sqlite/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/objects/ocel/importer/sqlite/importer.py` & `pm4py-2.7.9.4/pm4py/objects/ocel/importer/sqlite/importer.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/objects/ocel/importer/sqlite/variants/__init__.py` & `pm4py-2.7.9.4/pm4py/objects/ocel/importer/sqlite/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/objects/ocel/importer/sqlite/variants/ocel20.py` & `pm4py-2.7.9.4/pm4py/objects/ocel/importer/sqlite/variants/ocel20.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/objects/ocel/importer/sqlite/variants/pandas_importer.py` & `pm4py-2.7.9.4/pm4py/objects/ocel/importer/sqlite/variants/pandas_importer.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/objects/ocel/importer/xmlocel/__init__.py` & `pm4py-2.7.9.4/pm4py/objects/ocel/importer/xmlocel/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/objects/ocel/importer/xmlocel/importer.py` & `pm4py-2.7.9.4/pm4py/objects/ocel/importer/xmlocel/importer.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/objects/ocel/importer/xmlocel/variants/__init__.py` & `pm4py-2.7.9.4/pm4py/objects/ocel/importer/xmlocel/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/objects/ocel/importer/xmlocel/variants/classic.py` & `pm4py-2.7.9.4/pm4py/objects/ocel/importer/xmlocel/variants/classic.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/objects/ocel/importer/xmlocel/variants/ocel20.py` & `pm4py-2.7.9.4/pm4py/objects/ocel/importer/xmlocel/variants/ocel20.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/objects/ocel/obj.py` & `pm4py-2.7.9.4/pm4py/objects/ocel/obj.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/objects/ocel/util/__init__.py` & `pm4py-2.7.9.4/pm4py/objects/ocel/util/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/objects/ocel/util/attributes_names.py` & `pm4py-2.7.9.4/pm4py/objects/ocel/util/attributes_names.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/objects/ocel/util/attributes_per_type.py` & `pm4py-2.7.9.4/pm4py/objects/ocel/util/attributes_per_type.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/objects/ocel/util/convergence_divergence_diagnostics.py` & `pm4py-2.7.9.4/pm4py/objects/ocel/util/convergence_divergence_diagnostics.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/objects/ocel/util/e2o_qualification.py` & `pm4py-2.7.9.4/pm4py/objects/ocel/util/e2o_qualification.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/objects/ocel/util/ev_att_to_obj_type.py` & `pm4py-2.7.9.4/pm4py/objects/ocel/util/ev_att_to_obj_type.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/objects/ocel/util/event_prefix_suffix_per_obj.py` & `pm4py-2.7.9.4/pm4py/objects/ocel/util/event_prefix_suffix_per_obj.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/objects/ocel/util/events_per_object_type.py` & `pm4py-2.7.9.4/pm4py/objects/ocel/util/events_per_object_type.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/objects/ocel/util/events_per_type_per_activity.py` & `pm4py-2.7.9.4/pm4py/objects/ocel/util/events_per_type_per_activity.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/objects/ocel/util/explode.py` & `pm4py-2.7.9.4/pm4py/objects/ocel/util/explode.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/objects/ocel/util/extended_table.py` & `pm4py-2.7.9.4/pm4py/objects/ocel/util/extended_table.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/objects/ocel/util/filtering_utils.py` & `pm4py-2.7.9.4/pm4py/objects/ocel/util/filtering_utils.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/objects/ocel/util/flattening.py` & `pm4py-2.7.9.4/pm4py/objects/ocel/util/flattening.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/objects/ocel/util/log_ocel.py` & `pm4py-2.7.9.4/pm4py/objects/ocel/util/log_ocel.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/objects/ocel/util/names_stripping.py` & `pm4py-2.7.9.4/pm4py/objects/ocel/util/names_stripping.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/objects/ocel/util/objects_per_type_per_activity.py` & `pm4py-2.7.9.4/pm4py/objects/ocel/util/objects_per_type_per_activity.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/objects/ocel/util/ocel_consistency.py` & `pm4py-2.7.9.4/pm4py/objects/ocel/util/ocel_consistency.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/objects/ocel/util/ocel_iterator.py` & `pm4py-2.7.9.4/pm4py/objects/ocel/util/ocel_iterator.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/objects/ocel/util/ocel_to_dict_types_rel.py` & `pm4py-2.7.9.4/pm4py/objects/ocel/util/ocel_to_dict_types_rel.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/objects/ocel/util/ocel_type_renaming.py` & `pm4py-2.7.9.4/pm4py/objects/ocel/util/ocel_type_renaming.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/objects/ocel/util/parent_children_ref.py` & `pm4py-2.7.9.4/pm4py/objects/ocel/util/parent_children_ref.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/objects/ocel/util/related_events.py` & `pm4py-2.7.9.4/pm4py/objects/ocel/util/related_events.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/objects/ocel/util/related_objects.py` & `pm4py-2.7.9.4/pm4py/objects/ocel/util/related_objects.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/objects/ocel/util/rename_objs_ot_tim_lex.py` & `pm4py-2.7.9.4/pm4py/objects/ocel/util/rename_objs_ot_tim_lex.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/objects/ocel/util/sampling.py` & `pm4py-2.7.9.4/pm4py/objects/ocel/util/sampling.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/objects/ocel/validation/__init__.py` & `pm4py-2.7.9.4/pm4py/objects/ocel/validation/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/objects/ocel/validation/jsonocel.py` & `pm4py-2.7.9.4/pm4py/objects/ocel/validation/jsonocel.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/objects/ocel/validation/ocel20_rel_validation.py` & `pm4py-2.7.9.4/pm4py/objects/ocel/validation/ocel20_rel_validation.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/objects/ocel/validation/xmlocel.py` & `pm4py-2.7.9.4/pm4py/objects/ocel/validation/xmlocel.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/objects/org/__init__.py` & `pm4py-2.7.9.4/pm4py/objects/org/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/objects/org/roles/__init__.py` & `pm4py-2.7.9.4/pm4py/objects/org/roles/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/objects/org/roles/obj.py` & `pm4py-2.7.9.4/pm4py/objects/org/roles/obj.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/objects/org/sna/__init__.py` & `pm4py-2.7.9.4/pm4py/objects/org/sna/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/objects/org/sna/obj.py` & `pm4py-2.7.9.4/pm4py/objects/org/sna/obj.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/objects/petri_net/__init__.py` & `pm4py-2.7.9.4/pm4py/objects/petri_net/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/objects/petri_net/data_petri_nets/__init__.py` & `pm4py-2.7.9.4/pm4py/objects/petri_net/data_petri_nets/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/objects/petri_net/data_petri_nets/data_marking.py` & `pm4py-2.7.9.4/pm4py/objects/petri_net/data_petri_nets/data_marking.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/objects/petri_net/data_petri_nets/semantics.py` & `pm4py-2.7.9.4/pm4py/objects/petri_net/data_petri_nets/semantics.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/objects/petri_net/exporter/__init__.py` & `pm4py-2.7.9.4/pm4py/objects/petri_net/exporter/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/objects/petri_net/exporter/exporter.py` & `pm4py-2.7.9.4/pm4py/objects/petri_net/exporter/exporter.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/objects/petri_net/exporter/variants/__init__.py` & `pm4py-2.7.9.4/pm4py/objects/petri_net/exporter/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/objects/petri_net/exporter/variants/pnml.py` & `pm4py-2.7.9.4/pm4py/objects/petri_net/exporter/variants/pnml.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/objects/petri_net/importer/__init__.py` & `pm4py-2.7.9.4/pm4py/objects/petri_net/importer/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/objects/petri_net/importer/importer.py` & `pm4py-2.7.9.4/pm4py/objects/petri_net/importer/importer.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/objects/petri_net/importer/variants/__init__.py` & `pm4py-2.7.9.4/pm4py/objects/petri_net/importer/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/objects/petri_net/importer/variants/pnml.py` & `pm4py-2.7.9.4/pm4py/objects/petri_net/importer/variants/pnml.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/objects/petri_net/inhibitor_reset/__init__.py` & `pm4py-2.7.9.4/pm4py/objects/petri_net/inhibitor_reset/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/objects/petri_net/inhibitor_reset/semantics.py` & `pm4py-2.7.9.4/pm4py/objects/petri_net/inhibitor_reset/semantics.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/objects/petri_net/obj.py` & `pm4py-2.7.9.4/pm4py/objects/petri_net/obj.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/objects/petri_net/properties.py` & `pm4py-2.7.9.4/pm4py/objects/petri_net/properties.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/objects/petri_net/saw_net/__init__.py` & `pm4py-2.7.9.4/pm4py/objects/petri_net/saw_net/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/objects/petri_net/saw_net/convert.py` & `pm4py-2.7.9.4/pm4py/objects/petri_net/saw_net/convert.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/objects/petri_net/saw_net/obj.py` & `pm4py-2.7.9.4/pm4py/objects/petri_net/saw_net/obj.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/objects/petri_net/saw_net/semantics.py` & `pm4py-2.7.9.4/pm4py/objects/petri_net/saw_net/semantics.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/objects/petri_net/sem_interface.py` & `pm4py-2.7.9.4/pm4py/objects/petri_net/sem_interface.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/objects/petri_net/semantics.py` & `pm4py-2.7.9.4/pm4py/objects/petri_net/semantics.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/objects/petri_net/stochastic/__init__.py` & `pm4py-2.7.9.4/pm4py/objects/petri_net/stochastic/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/objects/petri_net/stochastic/obj.py` & `pm4py-2.7.9.4/pm4py/objects/petri_net/stochastic/obj.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/objects/petri_net/stochastic/semantics.py` & `pm4py-2.7.9.4/pm4py/objects/petri_net/stochastic/semantics.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/objects/petri_net/utils/__init__.py` & `pm4py-2.7.9.4/pm4py/objects/petri_net/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/objects/petri_net/utils/align_utils.py` & `pm4py-2.7.9.4/pm4py/objects/petri_net/utils/align_utils.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/objects/petri_net/utils/check_soundness.py` & `pm4py-2.7.9.4/pm4py/objects/petri_net/utils/check_soundness.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/objects/petri_net/utils/consumption_matrix.py` & `pm4py-2.7.9.4/pm4py/objects/petri_net/utils/consumption_matrix.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/objects/petri_net/utils/decomposition.py` & `pm4py-2.7.9.4/pm4py/objects/petri_net/utils/decomposition.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/objects/petri_net/utils/embed_stochastic_map.py` & `pm4py-2.7.9.4/pm4py/objects/petri_net/utils/embed_stochastic_map.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/objects/petri_net/utils/explore_path.py` & `pm4py-2.7.9.4/pm4py/objects/petri_net/utils/explore_path.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/objects/petri_net/utils/final_marking.py` & `pm4py-2.7.9.4/pm4py/objects/petri_net/utils/final_marking.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/objects/petri_net/utils/incidence_matrix.py` & `pm4py-2.7.9.4/pm4py/objects/petri_net/utils/incidence_matrix.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/objects/petri_net/utils/initial_marking.py` & `pm4py-2.7.9.4/pm4py/objects/petri_net/utils/initial_marking.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/objects/petri_net/utils/murata.py` & `pm4py-2.7.9.4/pm4py/objects/petri_net/utils/murata.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/objects/petri_net/utils/networkx_graph.py` & `pm4py-2.7.9.4/pm4py/objects/petri_net/utils/networkx_graph.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/objects/petri_net/utils/obj_marking.py` & `pm4py-2.7.9.4/pm4py/objects/petri_net/utils/obj_marking.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/objects/petri_net/utils/performance_map.py` & `pm4py-2.7.9.4/pm4py/objects/petri_net/utils/performance_map.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/objects/petri_net/utils/petri_utils.py` & `pm4py-2.7.9.4/pm4py/objects/petri_net/utils/petri_utils.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/objects/petri_net/utils/projection.py` & `pm4py-2.7.9.4/pm4py/objects/petri_net/utils/projection.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/objects/petri_net/utils/reachability_graph.py` & `pm4py-2.7.9.4/pm4py/objects/petri_net/utils/reachability_graph.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/objects/petri_net/utils/reduction.py` & `pm4py-2.7.9.4/pm4py/objects/petri_net/utils/reduction.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/objects/petri_net/utils/synchronous_product.py` & `pm4py-2.7.9.4/pm4py/objects/petri_net/utils/synchronous_product.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/objects/powl/BinaryRelation.py` & `pm4py-2.7.9.4/pm4py/objects/powl/BinaryRelation.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/objects/powl/__init__.py` & `pm4py-2.7.9.4/pm4py/objects/powl/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/objects/powl/constants.py` & `pm4py-2.7.9.4/pm4py/objects/powl/constants.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/objects/powl/obj.py` & `pm4py-2.7.9.4/pm4py/objects/powl/obj.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/objects/powl/parser.py` & `pm4py-2.7.9.4/pm4py/objects/powl/parser.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/objects/process_tree/__init__.py` & `pm4py-2.7.9.4/pm4py/objects/process_tree/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/objects/process_tree/exporter/__init__.py` & `pm4py-2.7.9.4/pm4py/objects/process_tree/exporter/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/objects/process_tree/exporter/exporter.py` & `pm4py-2.7.9.4/pm4py/objects/process_tree/exporter/exporter.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/objects/process_tree/exporter/variants/__init__.py` & `pm4py-2.7.9.4/pm4py/objects/process_tree/exporter/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/objects/process_tree/exporter/variants/ptml.py` & `pm4py-2.7.9.4/pm4py/objects/process_tree/exporter/variants/ptml.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/objects/process_tree/importer/__init__.py` & `pm4py-2.7.9.4/pm4py/objects/process_tree/importer/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/objects/process_tree/importer/importer.py` & `pm4py-2.7.9.4/pm4py/objects/process_tree/importer/importer.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/objects/process_tree/importer/variants/__init__.py` & `pm4py-2.7.9.4/pm4py/objects/process_tree/importer/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/objects/process_tree/importer/variants/ptml.py` & `pm4py-2.7.9.4/pm4py/objects/process_tree/importer/variants/ptml.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/objects/process_tree/obj.py` & `pm4py-2.7.9.4/pm4py/objects/process_tree/obj.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/objects/process_tree/semantics.py` & `pm4py-2.7.9.4/pm4py/objects/process_tree/semantics.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/objects/process_tree/state.py` & `pm4py-2.7.9.4/pm4py/objects/process_tree/state.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/objects/process_tree/utils/__init__.py` & `pm4py-2.7.9.4/pm4py/objects/process_tree/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/objects/process_tree/utils/bottomup.py` & `pm4py-2.7.9.4/pm4py/objects/process_tree/utils/bottomup.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/objects/process_tree/utils/generic.py` & `pm4py-2.7.9.4/pm4py/objects/process_tree/utils/generic.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/objects/process_tree/utils/regex.py` & `pm4py-2.7.9.4/pm4py/objects/process_tree/utils/regex.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/objects/random_variables/__init__.py` & `pm4py-2.7.9.4/pm4py/objects/random_variables/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/objects/random_variables/basic_structure.py` & `pm4py-2.7.9.4/pm4py/objects/random_variables/basic_structure.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/objects/random_variables/constant0/__init__.py` & `pm4py-2.7.9.4/pm4py/objects/random_variables/constant0/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/objects/random_variables/constant0/random_variable.py` & `pm4py-2.7.9.4/pm4py/objects/random_variables/constant0/random_variable.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/objects/random_variables/exponential/__init__.py` & `pm4py-2.7.9.4/pm4py/objects/random_variables/exponential/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/objects/random_variables/exponential/random_variable.py` & `pm4py-2.7.9.4/pm4py/objects/random_variables/exponential/random_variable.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/objects/random_variables/gamma/__init__.py` & `pm4py-2.7.9.4/pm4py/objects/random_variables/gamma/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/objects/random_variables/gamma/random_variable.py` & `pm4py-2.7.9.4/pm4py/objects/random_variables/gamma/random_variable.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/objects/random_variables/lognormal/__init__.py` & `pm4py-2.7.9.4/pm4py/objects/random_variables/lognormal/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/objects/random_variables/lognormal/random_variable.py` & `pm4py-2.7.9.4/pm4py/objects/random_variables/lognormal/random_variable.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/objects/random_variables/normal/__init__.py` & `pm4py-2.7.9.4/pm4py/objects/random_variables/normal/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/objects/random_variables/normal/random_variable.py` & `pm4py-2.7.9.4/pm4py/objects/random_variables/normal/random_variable.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/objects/random_variables/random_variable.py` & `pm4py-2.7.9.4/pm4py/objects/random_variables/random_variable.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/objects/random_variables/uniform/__init__.py` & `pm4py-2.7.9.4/pm4py/objects/random_variables/uniform/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/objects/random_variables/uniform/random_variable.py` & `pm4py-2.7.9.4/pm4py/objects/random_variables/uniform/random_variable.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/objects/stochastic_petri/__init__.py` & `pm4py-2.7.9.4/pm4py/objects/stochastic_petri/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/objects/stochastic_petri/ctmc.py` & `pm4py-2.7.9.4/pm4py/objects/stochastic_petri/ctmc.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/objects/stochastic_petri/tangible_reachability.py` & `pm4py-2.7.9.4/pm4py/objects/stochastic_petri/tangible_reachability.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/objects/stochastic_petri/utils.py` & `pm4py-2.7.9.4/pm4py/objects/stochastic_petri/utils.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/objects/transition_system/__init__.py` & `pm4py-2.7.9.4/pm4py/objects/transition_system/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/objects/transition_system/constants.py` & `pm4py-2.7.9.4/pm4py/objects/transition_system/constants.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/objects/transition_system/obj.py` & `pm4py-2.7.9.4/pm4py/objects/transition_system/obj.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/objects/transition_system/utils.py` & `pm4py-2.7.9.4/pm4py/objects/transition_system/utils.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/objects/trie/__init__.py` & `pm4py-2.7.9.4/pm4py/objects/trie/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/objects/trie/obj.py` & `pm4py-2.7.9.4/pm4py/objects/trie/obj.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/ocel.py` & `pm4py-2.7.9.4/pm4py/ocel.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/org.py` & `pm4py-2.7.9.4/pm4py/org.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/privacy.py` & `pm4py-2.7.9.4/pm4py/privacy.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/read.py` & `pm4py-2.7.9.4/pm4py/read.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/sim.py` & `pm4py-2.7.9.4/pm4py/sim.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/statistics/__init__.py` & `pm4py-2.7.9.4/pm4py/statistics/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/statistics/attributes/__init__.py` & `pm4py-2.7.9.4/pm4py/statistics/attributes/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/statistics/attributes/common/__init__.py` & `pm4py-2.7.9.4/pm4py/statistics/attributes/common/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/statistics/attributes/common/get.py` & `pm4py-2.7.9.4/pm4py/statistics/attributes/common/get.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/statistics/attributes/log/__init__.py` & `pm4py-2.7.9.4/pm4py/statistics/attributes/log/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/statistics/attributes/log/get.py` & `pm4py-2.7.9.4/pm4py/statistics/attributes/log/get.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/statistics/attributes/log/select.py` & `pm4py-2.7.9.4/pm4py/statistics/attributes/log/select.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/statistics/attributes/pandas/__init__.py` & `pm4py-2.7.9.4/pm4py/statistics/attributes/pandas/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/statistics/attributes/pandas/get.py` & `pm4py-2.7.9.4/pm4py/statistics/attributes/pandas/get.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/statistics/concurrent_activities/__init__.py` & `pm4py-2.7.9.4/pm4py/statistics/concurrent_activities/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/statistics/concurrent_activities/log/__init__.py` & `pm4py-2.7.9.4/pm4py/statistics/concurrent_activities/log/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/statistics/concurrent_activities/log/get.py` & `pm4py-2.7.9.4/pm4py/statistics/concurrent_activities/log/get.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/statistics/concurrent_activities/pandas/__init__.py` & `pm4py-2.7.9.4/pm4py/statistics/concurrent_activities/pandas/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/statistics/concurrent_activities/pandas/get.py` & `pm4py-2.7.9.4/pm4py/statistics/concurrent_activities/pandas/get.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/statistics/end_activities/__init__.py` & `pm4py-2.7.9.4/pm4py/statistics/end_activities/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/statistics/end_activities/common/__init__.py` & `pm4py-2.7.9.4/pm4py/statistics/end_activities/common/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/statistics/end_activities/common/get.py` & `pm4py-2.7.9.4/pm4py/statistics/end_activities/common/get.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/statistics/end_activities/log/__init__.py` & `pm4py-2.7.9.4/pm4py/statistics/end_activities/log/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/statistics/end_activities/log/get.py` & `pm4py-2.7.9.4/pm4py/statistics/end_activities/log/get.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/statistics/end_activities/pandas/__init__.py` & `pm4py-2.7.9.4/pm4py/statistics/end_activities/pandas/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/statistics/end_activities/pandas/get.py` & `pm4py-2.7.9.4/pm4py/statistics/end_activities/pandas/get.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/statistics/eventually_follows/__init__.py` & `pm4py-2.7.9.4/pm4py/statistics/eventually_follows/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/statistics/eventually_follows/log/__init__.py` & `pm4py-2.7.9.4/pm4py/statistics/eventually_follows/log/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/statistics/eventually_follows/log/get.py` & `pm4py-2.7.9.4/pm4py/statistics/eventually_follows/log/get.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/statistics/eventually_follows/pandas/__init__.py` & `pm4py-2.7.9.4/pm4py/statistics/eventually_follows/pandas/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/statistics/eventually_follows/pandas/get.py` & `pm4py-2.7.9.4/pm4py/statistics/eventually_follows/pandas/get.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/statistics/eventually_follows/uvcl/__init__.py` & `pm4py-2.7.9.4/pm4py/statistics/eventually_follows/uvcl/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/statistics/eventually_follows/uvcl/get.py` & `pm4py-2.7.9.4/pm4py/statistics/eventually_follows/uvcl/get.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/statistics/ocel/__init__.py` & `pm4py-2.7.9.4/pm4py/statistics/ocel/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/statistics/ocel/act_ot_dependent.py` & `pm4py-2.7.9.4/pm4py/statistics/ocel/act_ot_dependent.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/statistics/ocel/act_utils.py` & `pm4py-2.7.9.4/pm4py/statistics/ocel/act_utils.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/statistics/ocel/edge_metrics.py` & `pm4py-2.7.9.4/pm4py/statistics/ocel/edge_metrics.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/statistics/ocel/objects_ot_count.py` & `pm4py-2.7.9.4/pm4py/statistics/ocel/objects_ot_count.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/statistics/ocel/ot_activities.py` & `pm4py-2.7.9.4/pm4py/statistics/ocel/ot_activities.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/statistics/overlap/__init__.py` & `pm4py-2.7.9.4/pm4py/statistics/overlap/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/statistics/overlap/cases/__init__.py` & `pm4py-2.7.9.4/pm4py/statistics/overlap/cases/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/statistics/overlap/cases/log/__init__.py` & `pm4py-2.7.9.4/pm4py/statistics/overlap/cases/log/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/statistics/overlap/cases/log/get.py` & `pm4py-2.7.9.4/pm4py/statistics/overlap/cases/log/get.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/statistics/overlap/cases/pandas/__init__.py` & `pm4py-2.7.9.4/pm4py/statistics/overlap/cases/pandas/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/statistics/overlap/cases/pandas/get.py` & `pm4py-2.7.9.4/pm4py/statistics/overlap/cases/pandas/get.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/statistics/overlap/interval_events/__init__.py` & `pm4py-2.7.9.4/pm4py/statistics/overlap/interval_events/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/statistics/overlap/interval_events/log/__init__.py` & `pm4py-2.7.9.4/pm4py/statistics/overlap/interval_events/log/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/statistics/overlap/interval_events/log/get.py` & `pm4py-2.7.9.4/pm4py/statistics/overlap/interval_events/log/get.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/statistics/overlap/interval_events/pandas/__init__.py` & `pm4py-2.7.9.4/pm4py/statistics/overlap/interval_events/pandas/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/statistics/overlap/interval_events/pandas/get.py` & `pm4py-2.7.9.4/pm4py/statistics/overlap/interval_events/pandas/get.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/statistics/overlap/utils/__init__.py` & `pm4py-2.7.9.4/pm4py/statistics/overlap/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/statistics/overlap/utils/compute.py` & `pm4py-2.7.9.4/pm4py/statistics/overlap/utils/compute.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/statistics/passed_time/__init__.py` & `pm4py-2.7.9.4/pm4py/statistics/passed_time/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/statistics/passed_time/log/__init__.py` & `pm4py-2.7.9.4/pm4py/statistics/passed_time/log/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/statistics/passed_time/log/algorithm.py` & `pm4py-2.7.9.4/pm4py/statistics/passed_time/log/algorithm.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/statistics/passed_time/log/variants/__init__.py` & `pm4py-2.7.9.4/pm4py/statistics/passed_time/log/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/statistics/passed_time/log/variants/post.py` & `pm4py-2.7.9.4/pm4py/statistics/passed_time/log/variants/post.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/statistics/passed_time/log/variants/pre.py` & `pm4py-2.7.9.4/pm4py/statistics/passed_time/log/variants/pre.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/statistics/passed_time/log/variants/prepost.py` & `pm4py-2.7.9.4/pm4py/statistics/passed_time/log/variants/prepost.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/statistics/passed_time/pandas/__init__.py` & `pm4py-2.7.9.4/pm4py/statistics/passed_time/pandas/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/statistics/passed_time/pandas/algorithm.py` & `pm4py-2.7.9.4/pm4py/statistics/passed_time/pandas/algorithm.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/statistics/passed_time/pandas/variants/__init__.py` & `pm4py-2.7.9.4/pm4py/statistics/passed_time/pandas/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/statistics/passed_time/pandas/variants/post.py` & `pm4py-2.7.9.4/pm4py/statistics/passed_time/pandas/variants/post.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/statistics/passed_time/pandas/variants/pre.py` & `pm4py-2.7.9.4/pm4py/statistics/passed_time/pandas/variants/pre.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/statistics/passed_time/pandas/variants/prepost.py` & `pm4py-2.7.9.4/pm4py/statistics/passed_time/pandas/variants/prepost.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/statistics/rework/__init__.py` & `pm4py-2.7.9.4/pm4py/statistics/rework/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/statistics/rework/cases/__init__.py` & `pm4py-2.7.9.4/pm4py/statistics/rework/cases/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/statistics/rework/cases/log/__init__.py` & `pm4py-2.7.9.4/pm4py/statistics/rework/cases/log/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/statistics/rework/cases/log/get.py` & `pm4py-2.7.9.4/pm4py/statistics/rework/cases/log/get.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/statistics/rework/cases/pandas/__init__.py` & `pm4py-2.7.9.4/pm4py/statistics/rework/cases/pandas/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/statistics/rework/cases/pandas/get.py` & `pm4py-2.7.9.4/pm4py/statistics/rework/cases/pandas/get.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/statistics/rework/log/__init__.py` & `pm4py-2.7.9.4/pm4py/statistics/rework/log/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/statistics/rework/log/get.py` & `pm4py-2.7.9.4/pm4py/statistics/rework/log/get.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/statistics/rework/pandas/__init__.py` & `pm4py-2.7.9.4/pm4py/statistics/rework/pandas/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/statistics/rework/pandas/get.py` & `pm4py-2.7.9.4/pm4py/statistics/rework/pandas/get.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/statistics/service_time/__init__.py` & `pm4py-2.7.9.4/pm4py/statistics/service_time/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/statistics/service_time/log/__init__.py` & `pm4py-2.7.9.4/pm4py/statistics/service_time/log/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/statistics/service_time/log/get.py` & `pm4py-2.7.9.4/pm4py/statistics/service_time/log/get.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/statistics/service_time/pandas/__init__.py` & `pm4py-2.7.9.4/pm4py/statistics/service_time/pandas/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/statistics/service_time/pandas/get.py` & `pm4py-2.7.9.4/pm4py/statistics/service_time/pandas/get.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/statistics/sojourn_time/__init__.py` & `pm4py-2.7.9.4/pm4py/statistics/sojourn_time/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/statistics/start_activities/__init__.py` & `pm4py-2.7.9.4/pm4py/statistics/start_activities/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/statistics/start_activities/common/__init__.py` & `pm4py-2.7.9.4/pm4py/statistics/start_activities/common/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/statistics/start_activities/common/get.py` & `pm4py-2.7.9.4/pm4py/statistics/start_activities/common/get.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/statistics/start_activities/log/__init__.py` & `pm4py-2.7.9.4/pm4py/statistics/start_activities/log/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/statistics/start_activities/log/get.py` & `pm4py-2.7.9.4/pm4py/statistics/start_activities/log/get.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/statistics/start_activities/pandas/__init__.py` & `pm4py-2.7.9.4/pm4py/statistics/start_activities/pandas/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/statistics/start_activities/pandas/get.py` & `pm4py-2.7.9.4/pm4py/statistics/start_activities/pandas/get.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/statistics/traces/__init__.py` & `pm4py-2.7.9.4/pm4py/statistics/traces/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/statistics/traces/cycle_time/__init__.py` & `pm4py-2.7.9.4/pm4py/statistics/traces/cycle_time/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/statistics/traces/cycle_time/log/__init__.py` & `pm4py-2.7.9.4/pm4py/statistics/traces/cycle_time/log/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/statistics/traces/cycle_time/log/get.py` & `pm4py-2.7.9.4/pm4py/statistics/traces/cycle_time/log/get.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/statistics/traces/cycle_time/pandas/__init__.py` & `pm4py-2.7.9.4/pm4py/statistics/traces/cycle_time/pandas/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/statistics/traces/cycle_time/pandas/get.py` & `pm4py-2.7.9.4/pm4py/statistics/traces/cycle_time/pandas/get.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/statistics/traces/cycle_time/util/__init__.py` & `pm4py-2.7.9.4/pm4py/statistics/traces/cycle_time/util/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/statistics/traces/cycle_time/util/compute.py` & `pm4py-2.7.9.4/pm4py/statistics/traces/cycle_time/util/compute.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/statistics/traces/generic/__init__.py` & `pm4py-2.7.9.4/pm4py/statistics/traces/generic/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/statistics/traces/generic/common/__init__.py` & `pm4py-2.7.9.4/pm4py/statistics/traces/generic/common/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/statistics/traces/generic/common/case_duration.py` & `pm4py-2.7.9.4/pm4py/statistics/traces/generic/common/case_duration.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/statistics/traces/generic/log/__init__.py` & `pm4py-2.7.9.4/pm4py/statistics/traces/generic/log/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/statistics/traces/generic/log/case_arrival.py` & `pm4py-2.7.9.4/pm4py/statistics/traces/generic/log/case_arrival.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/statistics/traces/generic/log/case_statistics.py` & `pm4py-2.7.9.4/pm4py/statistics/traces/generic/log/case_statistics.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/statistics/traces/generic/pandas/__init__.py` & `pm4py-2.7.9.4/pm4py/statistics/traces/generic/pandas/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/statistics/traces/generic/pandas/case_arrival.py` & `pm4py-2.7.9.4/pm4py/statistics/traces/generic/pandas/case_arrival.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/statistics/traces/generic/pandas/case_statistics.py` & `pm4py-2.7.9.4/pm4py/statistics/traces/generic/pandas/case_statistics.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/statistics/util/__init__.py` & `pm4py-2.7.9.4/pm4py/statistics/util/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/statistics/util/times_bipartite_matching.py` & `pm4py-2.7.9.4/pm4py/statistics/util/times_bipartite_matching.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/statistics/variants/__init__.py` & `pm4py-2.7.9.4/pm4py/statistics/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/statistics/variants/log/__init__.py` & `pm4py-2.7.9.4/pm4py/statistics/variants/log/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/statistics/variants/log/get.py` & `pm4py-2.7.9.4/pm4py/statistics/variants/log/get.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/statistics/variants/pandas/__init__.py` & `pm4py-2.7.9.4/pm4py/statistics/variants/pandas/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/statistics/variants/pandas/get.py` & `pm4py-2.7.9.4/pm4py/statistics/variants/pandas/get.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/stats.py` & `pm4py-2.7.9.4/pm4py/stats.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/streaming/__init__.py` & `pm4py-2.7.9.4/pm4py/streaming/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/streaming/algo/__init__.py` & `pm4py-2.7.9.4/pm4py/streaming/algo/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/streaming/algo/conformance/__init__.py` & `pm4py-2.7.9.4/pm4py/streaming/algo/conformance/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/streaming/algo/conformance/footprints/__init__.py` & `pm4py-2.7.9.4/pm4py/streaming/algo/conformance/footprints/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/streaming/algo/conformance/footprints/algorithm.py` & `pm4py-2.7.9.4/pm4py/streaming/algo/conformance/footprints/algorithm.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/streaming/algo/conformance/footprints/variants/__init__.py` & `pm4py-2.7.9.4/pm4py/streaming/algo/conformance/footprints/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/streaming/algo/conformance/footprints/variants/classic.py` & `pm4py-2.7.9.4/pm4py/streaming/algo/conformance/footprints/variants/classic.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/streaming/algo/conformance/tbr/__init__.py` & `pm4py-2.7.9.4/pm4py/streaming/algo/conformance/tbr/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/streaming/algo/conformance/tbr/algorithm.py` & `pm4py-2.7.9.4/pm4py/streaming/algo/conformance/tbr/algorithm.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/streaming/algo/conformance/tbr/variants/__init__.py` & `pm4py-2.7.9.4/pm4py/streaming/algo/conformance/tbr/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/streaming/algo/conformance/tbr/variants/classic.py` & `pm4py-2.7.9.4/pm4py/streaming/algo/conformance/tbr/variants/classic.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/streaming/algo/conformance/temporal/__init__.py` & `pm4py-2.7.9.4/pm4py/streaming/algo/conformance/temporal/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/streaming/algo/conformance/temporal/algorithm.py` & `pm4py-2.7.9.4/pm4py/streaming/algo/conformance/temporal/algorithm.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/streaming/algo/conformance/temporal/variants/__init__.py` & `pm4py-2.7.9.4/pm4py/streaming/algo/conformance/temporal/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/streaming/algo/conformance/temporal/variants/classic.py` & `pm4py-2.7.9.4/pm4py/streaming/algo/conformance/temporal/variants/classic.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/streaming/algo/discovery/__init__.py` & `pm4py-2.7.9.4/pm4py/streaming/algo/discovery/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/streaming/algo/discovery/dfg/__init__.py` & `pm4py-2.7.9.4/pm4py/streaming/algo/discovery/dfg/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/streaming/algo/discovery/dfg/algorithm.py` & `pm4py-2.7.9.4/pm4py/streaming/algo/discovery/dfg/algorithm.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/streaming/algo/discovery/dfg/variants/__init__.py` & `pm4py-2.7.9.4/pm4py/streaming/algo/discovery/dfg/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/streaming/algo/discovery/dfg/variants/frequency.py` & `pm4py-2.7.9.4/pm4py/streaming/algo/discovery/dfg/variants/frequency.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/streaming/algo/interface.py` & `pm4py-2.7.9.4/pm4py/streaming/algo/interface.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/streaming/conversion/__init__.py` & `pm4py-2.7.9.4/pm4py/streaming/conversion/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/streaming/conversion/from_pandas.py` & `pm4py-2.7.9.4/pm4py/streaming/conversion/from_pandas.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/streaming/conversion/ocel_flatts_distributor.py` & `pm4py-2.7.9.4/pm4py/streaming/conversion/ocel_flatts_distributor.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/streaming/importer/__init__.py` & `pm4py-2.7.9.4/pm4py/streaming/importer/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/streaming/importer/csv/__init__.py` & `pm4py-2.7.9.4/pm4py/streaming/importer/csv/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/streaming/importer/csv/importer.py` & `pm4py-2.7.9.4/pm4py/streaming/importer/csv/importer.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/streaming/importer/csv/variants/__init__.py` & `pm4py-2.7.9.4/pm4py/streaming/importer/csv/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/streaming/importer/csv/variants/csv_event_stream.py` & `pm4py-2.7.9.4/pm4py/streaming/importer/csv/variants/csv_event_stream.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/streaming/importer/xes/__init__.py` & `pm4py-2.7.9.4/pm4py/streaming/importer/xes/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/streaming/importer/xes/importer.py` & `pm4py-2.7.9.4/pm4py/streaming/importer/xes/importer.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/streaming/importer/xes/variants/__init__.py` & `pm4py-2.7.9.4/pm4py/streaming/importer/xes/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/streaming/importer/xes/variants/xes_event_stream.py` & `pm4py-2.7.9.4/pm4py/streaming/importer/xes/variants/xes_event_stream.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/streaming/importer/xes/variants/xes_trace_stream.py` & `pm4py-2.7.9.4/pm4py/streaming/importer/xes/variants/xes_trace_stream.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/streaming/stream/__init__.py` & `pm4py-2.7.9.4/pm4py/streaming/stream/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/streaming/stream/live_event_stream.py` & `pm4py-2.7.9.4/pm4py/streaming/stream/live_event_stream.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/streaming/stream/live_trace_stream.py` & `pm4py-2.7.9.4/pm4py/streaming/stream/live_trace_stream.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/streaming/util/__init__.py` & `pm4py-2.7.9.4/pm4py/streaming/util/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/streaming/util/dictio/__init__.py` & `pm4py-2.7.9.4/pm4py/streaming/util/dictio/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/streaming/util/dictio/generator.py` & `pm4py-2.7.9.4/pm4py/streaming/util/dictio/generator.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/streaming/util/dictio/versions/__init__.py` & `pm4py-2.7.9.4/pm4py/streaming/util/dictio/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/streaming/util/dictio/versions/classic.py` & `pm4py-2.7.9.4/pm4py/streaming/util/dictio/versions/classic.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/streaming/util/dictio/versions/redis.py` & `pm4py-2.7.9.4/pm4py/streaming/util/dictio/versions/redis.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/streaming/util/dictio/versions/thread_safe.py` & `pm4py-2.7.9.4/pm4py/streaming/util/dictio/versions/thread_safe.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/streaming/util/event_stream_printer.py` & `pm4py-2.7.9.4/pm4py/streaming/util/event_stream_printer.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/streaming/util/live_to_static_stream.py` & `pm4py-2.7.9.4/pm4py/streaming/util/live_to_static_stream.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/streaming/util/trace_stream_printer.py` & `pm4py-2.7.9.4/pm4py/streaming/util/trace_stream_printer.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/util/__init__.py` & `pm4py-2.7.9.4/pm4py/util/__init__.py`

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

### Comparing `pm4py-2.7.9.3/pm4py/util/business_hours.py` & `pm4py-2.7.9.4/pm4py/util/business_hours.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/util/colors.py` & `pm4py-2.7.9.4/pm4py/util/colors.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/util/compression/__init__.py` & `pm4py-2.7.9.4/pm4py/util/compression/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/util/compression/dtypes.py` & `pm4py-2.7.9.4/pm4py/util/compression/dtypes.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/util/compression/util.py` & `pm4py-2.7.9.4/pm4py/util/compression/util.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/util/constants.py` & `pm4py-2.7.9.4/pm4py/util/constants.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/util/dt_parsing/__init__.py` & `pm4py-2.7.9.4/pm4py/util/dt_parsing/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/util/dt_parsing/parser.py` & `pm4py-2.7.9.4/pm4py/util/dt_parsing/parser.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/util/dt_parsing/variants/__init__.py` & `pm4py-2.7.9.4/pm4py/util/dt_parsing/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/util/dt_parsing/variants/cs8601.py` & `pm4py-2.7.9.4/pm4py/util/dt_parsing/variants/cs8601.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/util/dt_parsing/variants/dummy.py` & `pm4py-2.7.9.4/pm4py/util/dt_parsing/variants/dummy.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/util/dt_parsing/variants/strpfromiso.py` & `pm4py-2.7.9.4/pm4py/util/dt_parsing/variants/strpfromiso.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/util/exec_utils.py` & `pm4py-2.7.9.4/pm4py/util/exec_utils.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/util/lp/__init__.py` & `pm4py-2.7.9.4/pm4py/util/lp/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/util/lp/solver.py` & `pm4py-2.7.9.4/pm4py/util/lp/solver.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/util/lp/util/__init__.py` & `pm4py-2.7.9.4/pm4py/util/lp/util/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/util/lp/variants/__init__.py` & `pm4py-2.7.9.4/pm4py/util/lp/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/util/lp/variants/cvxopt_solver.py` & `pm4py-2.7.9.4/pm4py/util/lp/variants/cvxopt_solver.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/util/lp/variants/cvxopt_solver_custom_align.py` & `pm4py-2.7.9.4/pm4py/util/lp/variants/cvxopt_solver_custom_align.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/util/lp/variants/cvxopt_solver_custom_align_arm.py` & `pm4py-2.7.9.4/pm4py/util/lp/variants/cvxopt_solver_custom_align_arm.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/util/lp/variants/cvxopt_solver_custom_align_ilp.py` & `pm4py-2.7.9.4/pm4py/util/lp/variants/cvxopt_solver_custom_align_ilp.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/util/lp/variants/ortools_solver.py` & `pm4py-2.7.9.4/pm4py/util/lp/variants/ortools_solver.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/util/lp/variants/pulp_solver.py` & `pm4py-2.7.9.4/pm4py/util/lp/variants/pulp_solver.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/util/lp/variants/scipy_solver.py` & `pm4py-2.7.9.4/pm4py/util/lp/variants/scipy_solver.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/util/nx_utils.py` & `pm4py-2.7.9.4/pm4py/util/nx_utils.py`

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

### Comparing `pm4py-2.7.9.3/pm4py/util/pandas_utils.py` & `pm4py-2.7.9.4/pm4py/util/pandas_utils.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/util/points_subset.py` & `pm4py-2.7.9.4/pm4py/util/points_subset.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/util/regex.py` & `pm4py-2.7.9.4/pm4py/util/regex.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/util/string_distance.py` & `pm4py-2.7.9.4/pm4py/util/string_distance.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/util/typing.py` & `pm4py-2.7.9.4/pm4py/util/typing.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/util/variants_util.py` & `pm4py-2.7.9.4/pm4py/util/variants_util.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/util/vis_utils.py` & `pm4py-2.7.9.4/pm4py/util/vis_utils.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/util/xes_constants.py` & `pm4py-2.7.9.4/pm4py/util/xes_constants.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/utils.py` & `pm4py-2.7.9.4/pm4py/utils.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/vis.py` & `pm4py-2.7.9.4/pm4py/vis.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/visualization/__init__.py` & `pm4py-2.7.9.4/pm4py/visualization/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/visualization/align_table/__init__.py` & `pm4py-2.7.9.4/pm4py/visualization/align_table/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/visualization/align_table/variants/__init__.py` & `pm4py-2.7.9.4/pm4py/visualization/align_table/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/visualization/align_table/variants/classic.py` & `pm4py-2.7.9.4/pm4py/visualization/align_table/variants/classic.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/visualization/align_table/visualizer.py` & `pm4py-2.7.9.4/pm4py/visualization/align_table/visualizer.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/visualization/bpmn/__init__.py` & `pm4py-2.7.9.4/pm4py/visualization/bpmn/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/visualization/bpmn/variants/__init__.py` & `pm4py-2.7.9.4/pm4py/visualization/bpmn/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/visualization/bpmn/variants/classic.py` & `pm4py-2.7.9.4/pm4py/visualization/bpmn/variants/classic.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/visualization/bpmn/visualizer.py` & `pm4py-2.7.9.4/pm4py/visualization/bpmn/visualizer.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/visualization/common/__init__.py` & `pm4py-2.7.9.4/pm4py/visualization/common/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/visualization/common/dot_util.py` & `pm4py-2.7.9.4/pm4py/visualization/common/dot_util.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/visualization/common/gview.py` & `pm4py-2.7.9.4/pm4py/visualization/common/gview.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/visualization/common/html.py` & `pm4py-2.7.9.4/pm4py/visualization/common/html.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/visualization/common/save.py` & `pm4py-2.7.9.4/pm4py/visualization/common/save.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/visualization/common/svg_pos_parser.py` & `pm4py-2.7.9.4/pm4py/visualization/common/svg_pos_parser.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/visualization/common/utils.py` & `pm4py-2.7.9.4/pm4py/visualization/common/utils.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/visualization/common/visualizer.py` & `pm4py-2.7.9.4/pm4py/visualization/common/visualizer.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/visualization/decisiontree/__init__.py` & `pm4py-2.7.9.4/pm4py/visualization/decisiontree/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/visualization/decisiontree/util/__init__.py` & `pm4py-2.7.9.4/pm4py/visualization/decisiontree/util/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/visualization/decisiontree/util/dt_to_string.py` & `pm4py-2.7.9.4/pm4py/visualization/decisiontree/util/dt_to_string.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/visualization/decisiontree/variants/__init__.py` & `pm4py-2.7.9.4/pm4py/visualization/decisiontree/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/visualization/decisiontree/variants/classic.py` & `pm4py-2.7.9.4/pm4py/visualization/decisiontree/variants/classic.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/visualization/decisiontree/visualizer.py` & `pm4py-2.7.9.4/pm4py/visualization/decisiontree/visualizer.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/visualization/dfg/__init__.py` & `pm4py-2.7.9.4/pm4py/visualization/dfg/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/visualization/dfg/util/__init__.py` & `pm4py-2.7.9.4/pm4py/visualization/dfg/util/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/visualization/dfg/util/dfg_gviz.py` & `pm4py-2.7.9.4/pm4py/visualization/dfg/util/dfg_gviz.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/visualization/dfg/variants/__init__.py` & `pm4py-2.7.9.4/pm4py/visualization/dfg/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/visualization/dfg/variants/cost.py` & `pm4py-2.7.9.4/pm4py/visualization/dfg/variants/cost.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/visualization/dfg/variants/frequency.py` & `pm4py-2.7.9.4/pm4py/visualization/dfg/variants/frequency.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/visualization/dfg/variants/performance.py` & `pm4py-2.7.9.4/pm4py/visualization/dfg/variants/performance.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/visualization/dfg/variants/timeline.py` & `pm4py-2.7.9.4/pm4py/visualization/dfg/variants/timeline.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/visualization/dfg/visualizer.py` & `pm4py-2.7.9.4/pm4py/visualization/dfg/visualizer.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/visualization/dotted_chart/__init__.py` & `pm4py-2.7.9.4/pm4py/visualization/dotted_chart/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/visualization/dotted_chart/variants/__init__.py` & `pm4py-2.7.9.4/pm4py/visualization/dotted_chart/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/visualization/dotted_chart/variants/classic.py` & `pm4py-2.7.9.4/pm4py/visualization/dotted_chart/variants/classic.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/visualization/dotted_chart/visualizer.py` & `pm4py-2.7.9.4/pm4py/visualization/dotted_chart/visualizer.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/visualization/footprints/__init__.py` & `pm4py-2.7.9.4/pm4py/visualization/footprints/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/visualization/footprints/variants/__init__.py` & `pm4py-2.7.9.4/pm4py/visualization/footprints/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/visualization/footprints/variants/comparison.py` & `pm4py-2.7.9.4/pm4py/visualization/footprints/variants/comparison.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/visualization/footprints/variants/comparison_symmetric.py` & `pm4py-2.7.9.4/pm4py/visualization/footprints/variants/comparison_symmetric.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/visualization/footprints/variants/single.py` & `pm4py-2.7.9.4/pm4py/visualization/footprints/variants/single.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/visualization/footprints/visualizer.py` & `pm4py-2.7.9.4/pm4py/visualization/footprints/visualizer.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/visualization/graphs/__init__.py` & `pm4py-2.7.9.4/pm4py/visualization/graphs/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/visualization/graphs/util/__init__.py` & `pm4py-2.7.9.4/pm4py/visualization/graphs/util/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/visualization/graphs/util/common.py` & `pm4py-2.7.9.4/pm4py/visualization/graphs/util/common.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/visualization/graphs/variants/__init__.py` & `pm4py-2.7.9.4/pm4py/visualization/graphs/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/visualization/graphs/variants/attributes.py` & `pm4py-2.7.9.4/pm4py/visualization/graphs/variants/attributes.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/visualization/graphs/variants/barplot.py` & `pm4py-2.7.9.4/pm4py/visualization/graphs/variants/barplot.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/visualization/graphs/variants/cases.py` & `pm4py-2.7.9.4/pm4py/visualization/graphs/variants/cases.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/visualization/graphs/variants/dates.py` & `pm4py-2.7.9.4/pm4py/visualization/graphs/variants/dates.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/visualization/graphs/visualizer.py` & `pm4py-2.7.9.4/pm4py/visualization/graphs/visualizer.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/visualization/heuristics_net/__init__.py` & `pm4py-2.7.9.4/pm4py/visualization/heuristics_net/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/visualization/heuristics_net/variants/__init__.py` & `pm4py-2.7.9.4/pm4py/visualization/heuristics_net/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/visualization/heuristics_net/variants/pydotplus_vis.py` & `pm4py-2.7.9.4/pm4py/visualization/heuristics_net/variants/pydotplus_vis.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/visualization/heuristics_net/visualizer.py` & `pm4py-2.7.9.4/pm4py/visualization/heuristics_net/visualizer.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/visualization/network_analysis/__init__.py` & `pm4py-2.7.9.4/pm4py/visualization/network_analysis/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/visualization/network_analysis/variants/__init__.py` & `pm4py-2.7.9.4/pm4py/visualization/network_analysis/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/visualization/network_analysis/variants/frequency.py` & `pm4py-2.7.9.4/pm4py/visualization/network_analysis/variants/frequency.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/visualization/network_analysis/variants/performance.py` & `pm4py-2.7.9.4/pm4py/visualization/network_analysis/variants/performance.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/visualization/network_analysis/visualizer.py` & `pm4py-2.7.9.4/pm4py/visualization/network_analysis/visualizer.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/visualization/networkx/__init__.py` & `pm4py-2.7.9.4/pm4py/visualization/networkx/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/visualization/networkx/variants/__init__.py` & `pm4py-2.7.9.4/pm4py/visualization/networkx/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/visualization/networkx/variants/digraph.py` & `pm4py-2.7.9.4/pm4py/visualization/networkx/variants/digraph.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/visualization/networkx/visualizer.py` & `pm4py-2.7.9.4/pm4py/visualization/networkx/visualizer.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/visualization/ocel/__init__.py` & `pm4py-2.7.9.4/pm4py/visualization/ocel/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/visualization/ocel/eve_to_obj_types/__init__.py` & `pm4py-2.7.9.4/pm4py/visualization/ocel/eve_to_obj_types/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/visualization/ocel/eve_to_obj_types/variants/__init__.py` & `pm4py-2.7.9.4/pm4py/visualization/ocel/eve_to_obj_types/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/visualization/ocel/eve_to_obj_types/variants/graphviz.py` & `pm4py-2.7.9.4/pm4py/visualization/ocel/eve_to_obj_types/variants/graphviz.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/visualization/ocel/eve_to_obj_types/visualizer.py` & `pm4py-2.7.9.4/pm4py/visualization/ocel/eve_to_obj_types/visualizer.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/visualization/ocel/interleavings/__init__.py` & `pm4py-2.7.9.4/pm4py/visualization/ocel/interleavings/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/visualization/ocel/interleavings/variants/__init__.py` & `pm4py-2.7.9.4/pm4py/visualization/ocel/interleavings/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/visualization/ocel/interleavings/variants/graphviz.py` & `pm4py-2.7.9.4/pm4py/visualization/ocel/interleavings/variants/graphviz.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/visualization/ocel/interleavings/visualizer.py` & `pm4py-2.7.9.4/pm4py/visualization/ocel/interleavings/visualizer.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/visualization/ocel/object_graph/__init__.py` & `pm4py-2.7.9.4/pm4py/visualization/ocel/object_graph/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/visualization/ocel/object_graph/variants/__init__.py` & `pm4py-2.7.9.4/pm4py/visualization/ocel/object_graph/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/visualization/ocel/object_graph/variants/graphviz.py` & `pm4py-2.7.9.4/pm4py/visualization/ocel/object_graph/variants/graphviz.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/visualization/ocel/object_graph/visualizer.py` & `pm4py-2.7.9.4/pm4py/visualization/ocel/object_graph/visualizer.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/visualization/ocel/ocdfg/__init__.py` & `pm4py-2.7.9.4/pm4py/visualization/ocel/ocdfg/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/visualization/ocel/ocdfg/variants/__init__.py` & `pm4py-2.7.9.4/pm4py/visualization/ocel/ocdfg/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/visualization/ocel/ocdfg/variants/classic.py` & `pm4py-2.7.9.4/pm4py/visualization/ocel/ocdfg/variants/classic.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/visualization/ocel/ocdfg/visualizer.py` & `pm4py-2.7.9.4/pm4py/visualization/ocel/ocdfg/visualizer.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/visualization/ocel/ocpn/__init__.py` & `pm4py-2.7.9.4/pm4py/visualization/ocel/ocpn/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/visualization/ocel/ocpn/variants/__init__.py` & `pm4py-2.7.9.4/pm4py/visualization/ocel/ocpn/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/visualization/ocel/ocpn/variants/wo_decoration.py` & `pm4py-2.7.9.4/pm4py/visualization/ocel/ocpn/variants/wo_decoration.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/visualization/ocel/ocpn/visualizer.py` & `pm4py-2.7.9.4/pm4py/visualization/ocel/ocpn/visualizer.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/visualization/performance_spectrum/__init__.py` & `pm4py-2.7.9.4/pm4py/visualization/performance_spectrum/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/visualization/performance_spectrum/variants/__init__.py` & `pm4py-2.7.9.4/pm4py/visualization/performance_spectrum/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/visualization/performance_spectrum/variants/neato.py` & `pm4py-2.7.9.4/pm4py/visualization/performance_spectrum/variants/neato.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/visualization/performance_spectrum/visualizer.py` & `pm4py-2.7.9.4/pm4py/visualization/performance_spectrum/visualizer.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/visualization/petri_net/__init__.py` & `pm4py-2.7.9.4/pm4py/visualization/petri_net/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/visualization/petri_net/common/__init__.py` & `pm4py-2.7.9.4/pm4py/visualization/petri_net/common/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/visualization/petri_net/common/visualize.py` & `pm4py-2.7.9.4/pm4py/visualization/petri_net/common/visualize.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/visualization/petri_net/util/__init__.py` & `pm4py-2.7.9.4/pm4py/visualization/petri_net/util/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/visualization/petri_net/util/alignments_decoration.py` & `pm4py-2.7.9.4/pm4py/visualization/petri_net/util/alignments_decoration.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/visualization/petri_net/util/performance_map.py` & `pm4py-2.7.9.4/pm4py/visualization/petri_net/util/performance_map.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/visualization/petri_net/util/vis_trans_shortest_paths.py` & `pm4py-2.7.9.4/pm4py/visualization/petri_net/util/vis_trans_shortest_paths.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/visualization/petri_net/variants/__init__.py` & `pm4py-2.7.9.4/pm4py/visualization/petri_net/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/visualization/petri_net/variants/alignments.py` & `pm4py-2.7.9.4/pm4py/visualization/petri_net/variants/alignments.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/visualization/petri_net/variants/greedy_decoration_frequency.py` & `pm4py-2.7.9.4/pm4py/visualization/petri_net/variants/greedy_decoration_frequency.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/visualization/petri_net/variants/greedy_decoration_performance.py` & `pm4py-2.7.9.4/pm4py/visualization/petri_net/variants/greedy_decoration_performance.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/visualization/petri_net/variants/token_decoration_frequency.py` & `pm4py-2.7.9.4/pm4py/visualization/petri_net/variants/token_decoration_frequency.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/visualization/petri_net/variants/token_decoration_performance.py` & `pm4py-2.7.9.4/pm4py/visualization/petri_net/variants/token_decoration_performance.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/visualization/petri_net/variants/wo_decoration.py` & `pm4py-2.7.9.4/pm4py/visualization/petri_net/variants/wo_decoration.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/visualization/petri_net/visualizer.py` & `pm4py-2.7.9.4/pm4py/visualization/petri_net/visualizer.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/visualization/powl/__init__.py` & `pm4py-2.7.9.4/pm4py/visualization/powl/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/visualization/powl/variants/__init__.py` & `pm4py-2.7.9.4/pm4py/visualization/powl/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/visualization/powl/variants/basic.py` & `pm4py-2.7.9.4/pm4py/visualization/powl/variants/basic.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/visualization/powl/variants/end.png` & `pm4py-2.7.9.4/pm4py/visualization/powl/variants/end.png`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/visualization/powl/variants/loop.png` & `pm4py-2.7.9.4/pm4py/visualization/powl/variants/loop.png`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/visualization/powl/variants/net.py` & `pm4py-2.7.9.4/pm4py/visualization/powl/variants/net.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/visualization/powl/variants/play.png` & `pm4py-2.7.9.4/pm4py/visualization/powl/variants/play.png`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/visualization/powl/variants/xor.png` & `pm4py-2.7.9.4/pm4py/visualization/powl/variants/xor.png`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/visualization/powl/visualizer.py` & `pm4py-2.7.9.4/pm4py/visualization/powl/visualizer.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/visualization/process_tree/__init__.py` & `pm4py-2.7.9.4/pm4py/visualization/process_tree/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/visualization/process_tree/variants/__init__.py` & `pm4py-2.7.9.4/pm4py/visualization/process_tree/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/visualization/process_tree/variants/frequency_annotation.py` & `pm4py-2.7.9.4/pm4py/visualization/process_tree/variants/frequency_annotation.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/visualization/process_tree/variants/symbolic.py` & `pm4py-2.7.9.4/pm4py/visualization/process_tree/variants/symbolic.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/visualization/process_tree/variants/wo_decoration.py` & `pm4py-2.7.9.4/pm4py/visualization/process_tree/variants/wo_decoration.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/visualization/process_tree/visualizer.py` & `pm4py-2.7.9.4/pm4py/visualization/process_tree/visualizer.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/visualization/sna/__init__.py` & `pm4py-2.7.9.4/pm4py/visualization/sna/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/visualization/sna/variants/__init__.py` & `pm4py-2.7.9.4/pm4py/visualization/sna/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/visualization/sna/variants/networkx.py` & `pm4py-2.7.9.4/pm4py/visualization/sna/variants/networkx.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/visualization/sna/variants/pyvis.py` & `pm4py-2.7.9.4/pm4py/visualization/sna/variants/pyvis.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/visualization/sna/visualizer.py` & `pm4py-2.7.9.4/pm4py/visualization/sna/visualizer.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/visualization/transition_system/__init__.py` & `pm4py-2.7.9.4/pm4py/visualization/transition_system/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/visualization/transition_system/util/__init__.py` & `pm4py-2.7.9.4/pm4py/visualization/transition_system/util/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/visualization/transition_system/util/visualize_graphviz.py` & `pm4py-2.7.9.4/pm4py/visualization/transition_system/util/visualize_graphviz.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/visualization/transition_system/variants/__init__.py` & `pm4py-2.7.9.4/pm4py/visualization/transition_system/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/visualization/transition_system/variants/trans_frequency.py` & `pm4py-2.7.9.4/pm4py/visualization/transition_system/variants/trans_frequency.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/visualization/transition_system/variants/view_based.py` & `pm4py-2.7.9.4/pm4py/visualization/transition_system/variants/view_based.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/visualization/transition_system/visualizer.py` & `pm4py-2.7.9.4/pm4py/visualization/transition_system/visualizer.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/visualization/trie/__init__.py` & `pm4py-2.7.9.4/pm4py/visualization/trie/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/visualization/trie/variants/__init__.py` & `pm4py-2.7.9.4/pm4py/visualization/trie/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/visualization/trie/variants/classic.py` & `pm4py-2.7.9.4/pm4py/visualization/trie/variants/classic.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/visualization/trie/visualizer.py` & `pm4py-2.7.9.4/pm4py/visualization/trie/visualizer.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py/write.py` & `pm4py-2.7.9.4/pm4py/write.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/pm4py.egg-info/PKG-INFO` & `pm4py-2.7.9.4/pm4py.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: pm4py
-Version: 2.7.9.3
+Version: 2.7.9.4
 Summary: Process mining for Python
 Home-page: https://pm4py.fit.fraunhofer.de
 Author: Fraunhofer Institute for Applied Information Technology FIT
 Author-email: pm4py@fit.fraunhofer.de
 License: GPL 3.0
 Project-URL: Documentation, https://pm4py.fit.fraunhofer.de
 Project-URL: Source, https://github.com/pm4py/pm4py-source
 Project-URL: Tracker, https://github.com/pm4py/pm4py-source/issues
 License-File: LICENSE
-Requires-Dist: cvxopt; python_version < "3.12"
+Requires-Dist: cvxopt; python_version < "3.13"
 Requires-Dist: deprecation
 Requires-Dist: graphviz
 Requires-Dist: intervaltree
 Requires-Dist: lxml
 Requires-Dist: matplotlib
 Requires-Dist: networkx
 Requires-Dist: numpy
@@ -78,7 +78,8 @@
 pages = {100556},  
 year = {2023},  
 issn = {2665-9638},  
 doi = {https://doi.org/10.1016/j.simpa.2023.100556},  
 url = {https://www.sciencedirect.com/science/article/pii/S2665963823000933},  
 author = {Alessandro Berti and Sebastiaan van Zelst and Daniel Schuster},  
 }
+
```

### Comparing `pm4py-2.7.9.3/pm4py.egg-info/SOURCES.txt` & `pm4py-2.7.9.4/pm4py.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/setup.py` & `pm4py-2.7.9.4/setup.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.9.3/tests/test_cli.py` & `pm4py-2.7.9.4/tests/test_cli.py`

 * *Files identical despite different names*

