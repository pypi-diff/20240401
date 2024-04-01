# Comparing `tmp/polars-0.9.8.tar.gz` & `tmp/polars-0.9.9.tar.gz`

## Comparing `polars-0.9.8.tar` & `polars-0.9.9.tar`

### file list

```diff
@@ -1,313 +1,313 @@
--rw-r--r--   0        0        0      759 1970-01-01 00:00:00.000000 polars-0.9.8/local_dependencies/polars-arrow/Cargo.toml
--rw-r--r--   0     1001      121      985 2021-09-18 12:23:02.000000 polars-0.9.8/local_dependencies/polars-arrow/src/array/default_arrays.rs
--rw-r--r--   0     1001      121     5443 2021-09-18 12:23:02.000000 polars-0.9.8/local_dependencies/polars-arrow/src/array/mod.rs
--rw-r--r--   0     1001      121     2294 2021-09-18 12:23:02.000000 polars-0.9.8/local_dependencies/polars-arrow/src/bit_util.rs
--rw-r--r--   0     1001      121      395 2021-09-18 12:23:02.000000 polars-0.9.8/local_dependencies/polars-arrow/src/error.rs
--rw-r--r--   0     1001      121      862 2021-09-18 12:23:02.000000 polars-0.9.8/local_dependencies/polars-arrow/src/is_valid.rs
--rw-r--r--   0     1001      121     9506 2021-09-18 12:23:02.000000 polars-0.9.8/local_dependencies/polars-arrow/src/kernels/mod.rs
--rw-r--r--   0     1001      121     4800 2021-09-18 12:23:02.000000 polars-0.9.8/local_dependencies/polars-arrow/src/kernels/set.rs
--rw-r--r--   0     1001      121      151 2021-09-18 12:23:02.000000 polars-0.9.8/local_dependencies/polars-arrow/src/lib.rs
--rw-r--r--   0     1001      121       66 2021-09-18 12:23:02.000000 polars-0.9.8/local_dependencies/polars-arrow/src/prelude.rs
--rw-r--r--   0     1001      121      997 2021-09-18 12:23:02.000000 polars-0.9.8/local_dependencies/polars-arrow/src/trusted_len/boolean.rs
--rw-r--r--   0     1001      121     4897 2021-09-18 12:23:02.000000 polars-0.9.8/local_dependencies/polars-arrow/src/trusted_len/mod.rs
--rw-r--r--   0     1001      121     2594 2021-09-18 12:23:02.000000 polars-0.9.8/local_dependencies/polars-arrow/src/utils.rs
--rw-r--r--   0        0        0     4793 1970-01-01 00:00:00.000000 polars-0.9.8/local_dependencies/polars/Cargo.toml
--rw-r--r--   0     1001      121      941 2021-09-18 12:23:02.000000 polars-0.9.8/local_dependencies/polars/Makefile
--rw-r--r--   0     1001      121     1966 2021-09-18 12:23:02.000000 polars-0.9.8/local_dependencies/polars/benches/bench.rs
--rw-r--r--   0     1001      121     2743 2021-09-18 12:23:02.000000 polars-0.9.8/local_dependencies/polars/benches/collect.rs
--rw-r--r--   0     1001      121      667 2021-09-18 12:23:02.000000 polars-0.9.8/local_dependencies/polars/benches/csv.rs
--rw-r--r--   0     1001      121     5105 2021-09-18 12:23:02.000000 polars-0.9.8/local_dependencies/polars/benches/groupby.rs
--rw-r--r--   0     1001      121     2252 2021-09-18 12:23:02.000000 polars-0.9.8/local_dependencies/polars/benches/take.rs
--rw-r--r--   0     1001      121    19759 2021-09-18 12:23:02.000000 polars-0.9.8/local_dependencies/polars/src/docs/eager.rs
--rw-r--r--   0     1001      121     9038 2021-09-18 12:23:02.000000 polars-0.9.8/local_dependencies/polars/src/docs/lazy.rs
--rw-r--r--   0     1001      121       50 2021-09-18 12:23:02.000000 polars-0.9.8/local_dependencies/polars/src/docs/mod.rs
--rw-r--r--   0     1001      121     3772 2021-09-18 12:23:02.000000 polars-0.9.8/local_dependencies/polars/src/docs/performance.rs
--rw-r--r--   0     1001      121    11633 2021-09-18 12:23:02.000000 polars-0.9.8/local_dependencies/polars/src/lib.rs
--rw-r--r--   0     1001      121      170 2021-09-18 12:23:02.000000 polars-0.9.8/local_dependencies/polars/src/prelude.rs
--rw-r--r--   0        0        0     1659 1970-01-01 00:00:00.000000 polars-0.9.8/local_dependencies/polars-io/Cargo.toml
--rw-r--r--   0     1001      121    34545 2021-09-18 12:23:02.000000 polars-0.9.8/local_dependencies/polars-io/src/csv.rs
--rw-r--r--   0     1001      121    15713 2021-09-18 12:23:02.000000 polars-0.9.8/local_dependencies/polars-io/src/csv_core/buffer.rs
--rw-r--r--   0     1001      121    22465 2021-09-18 12:23:02.000000 polars-0.9.8/local_dependencies/polars-io/src/csv_core/csv.rs
--rw-r--r--   0     1001      121      158 2021-09-18 12:23:02.000000 polars-0.9.8/local_dependencies/polars-io/src/csv_core/mod.rs
--rw-r--r--   0     1001      121    16002 2021-09-18 12:23:02.000000 polars-0.9.8/local_dependencies/polars-io/src/csv_core/parser.rs
--rw-r--r--   0     1001      121    10564 2021-09-18 12:23:02.000000 polars-0.9.8/local_dependencies/polars-io/src/csv_core/utils.rs
--rw-r--r--   0     1001      121     4211 2021-09-18 12:23:02.000000 polars-0.9.8/local_dependencies/polars-io/src/ipc.rs
--rw-r--r--   0     1001      121     5733 2021-09-18 12:23:02.000000 polars-0.9.8/local_dependencies/polars-io/src/json.rs
--rw-r--r--   0     1001      121     5770 2021-09-18 12:23:02.000000 polars-0.9.8/local_dependencies/polars-io/src/lib.rs
--rw-r--r--   0     1001      121     1226 2021-09-18 12:23:02.000000 polars-0.9.8/local_dependencies/polars-io/src/mmap.rs
--rw-r--r--   0     1001      121     7935 2021-09-18 12:23:02.000000 polars-0.9.8/local_dependencies/polars-io/src/parquet.rs
--rw-r--r--   0     1001      121      567 2021-09-18 12:23:02.000000 polars-0.9.8/local_dependencies/polars-io/src/prelude.rs
--rw-r--r--   0     1001      121      436 2021-09-18 12:23:02.000000 polars-0.9.8/local_dependencies/polars-io/src/tests.rs
--rw-r--r--   0     1001      121     2093 2021-09-18 12:23:02.000000 polars-0.9.8/local_dependencies/polars-io/src/utils.rs
--rw-r--r--   0        0        0     1935 1970-01-01 00:00:00.000000 polars-0.9.8/local_dependencies/polars-lazy/Cargo.toml
--rw-r--r--   0     1001      121    13389 2021-09-18 12:23:02.000000 polars-0.9.8/local_dependencies/polars-lazy/src/datafusion/conversion.rs
--rw-r--r--   0     1001      121     2393 2021-09-18 12:23:02.000000 polars-0.9.8/local_dependencies/polars-lazy/src/datafusion/mod.rs
--rw-r--r--   0     1001      121    59894 2021-09-18 12:23:02.000000 polars-0.9.8/local_dependencies/polars-lazy/src/dsl.rs
--rw-r--r--   0     1001      121      524 2021-09-18 12:23:02.000000 polars-0.9.8/local_dependencies/polars-lazy/src/dummies.rs
--rw-r--r--   0     1001      121    36544 2021-09-18 12:23:02.000000 polars-0.9.8/local_dependencies/polars-lazy/src/frame.rs
--rw-r--r--   0     1001      121     6863 2021-09-18 12:23:02.000000 polars-0.9.8/local_dependencies/polars-lazy/src/functions.rs
--rw-r--r--   0     1001      121     7405 2021-09-18 12:23:02.000000 polars-0.9.8/local_dependencies/polars-lazy/src/lib.rs
--rw-r--r--   0     1001      121    14547 2021-09-18 12:23:02.000000 polars-0.9.8/local_dependencies/polars-lazy/src/logical_plan/aexpr.rs
--rw-r--r--   0     1001      121    22886 2021-09-18 12:23:02.000000 polars-0.9.8/local_dependencies/polars-lazy/src/logical_plan/alp.rs
--rw-r--r--   0     1001      121    25945 2021-09-18 12:23:02.000000 polars-0.9.8/local_dependencies/polars-lazy/src/logical_plan/conversion.rs
--rw-r--r--   0     1001      121     9320 2021-09-18 12:23:02.000000 polars-0.9.8/local_dependencies/polars-lazy/src/logical_plan/iterator.rs
--rw-r--r--   0     1001      121    47979 2021-09-18 12:23:02.000000 polars-0.9.8/local_dependencies/polars-lazy/src/logical_plan/mod.rs
--rw-r--r--   0     1001      121     6336 2021-09-18 12:23:02.000000 polars-0.9.8/local_dependencies/polars-lazy/src/logical_plan/optimizer/aggregate_pushdown.rs
--rw-r--r--   0     1001      121     6277 2021-09-18 12:23:02.000000 polars-0.9.8/local_dependencies/polars-lazy/src/logical_plan/optimizer/aggregate_scan_projections.rs
--rw-r--r--   0     1001      121     1960 2021-09-18 12:23:02.000000 polars-0.9.8/local_dependencies/polars-lazy/src/logical_plan/optimizer/drop_nulls.rs
--rw-r--r--   0     1001      121     2359 2021-09-18 12:23:02.000000 polars-0.9.8/local_dependencies/polars-lazy/src/logical_plan/optimizer/fast_projection.rs
--rw-r--r--   0     1001      121     7011 2021-09-18 12:23:02.000000 polars-0.9.8/local_dependencies/polars-lazy/src/logical_plan/optimizer/join_pruning.rs
--rw-r--r--   0     1001      121      762 2021-09-18 12:23:02.000000 polars-0.9.8/local_dependencies/polars-lazy/src/logical_plan/optimizer/mod.rs
--rw-r--r--   0     1001      121    19264 2021-09-18 12:23:02.000000 polars-0.9.8/local_dependencies/polars-lazy/src/logical_plan/optimizer/predicate_pushdown/mod.rs
--rw-r--r--   0     1001      121     9945 2021-09-18 12:23:02.000000 polars-0.9.8/local_dependencies/polars-lazy/src/logical_plan/optimizer/predicate_pushdown/utils.rs
--rw-r--r--   0     1001      121    30562 2021-09-18 12:23:02.000000 polars-0.9.8/local_dependencies/polars-lazy/src/logical_plan/optimizer/projection_pushdown.rs
--rw-r--r--   0     1001      121    15318 2021-09-18 12:23:02.000000 polars-0.9.8/local_dependencies/polars-lazy/src/logical_plan/optimizer/simplify_expr.rs
--rw-r--r--   0     1001      121     3083 2021-09-18 12:23:02.000000 polars-0.9.8/local_dependencies/polars-lazy/src/logical_plan/optimizer/stack_opt.rs
--rw-r--r--   0     1001      121    10231 2021-09-18 12:23:02.000000 polars-0.9.8/local_dependencies/polars-lazy/src/logical_plan/optimizer/type_coercion.rs
--rw-r--r--   0     1001      121      703 2021-09-18 12:23:02.000000 polars-0.9.8/local_dependencies/polars-lazy/src/physical_plan/executors/cache.rs
--rw-r--r--   0     1001      121      556 2021-09-18 12:23:02.000000 polars-0.9.8/local_dependencies/polars-lazy/src/physical_plan/executors/drop_duplicates.rs
--rw-r--r--   0     1001      121      407 2021-09-18 12:23:02.000000 polars-0.9.8/local_dependencies/polars-lazy/src/physical_plan/executors/explode.rs
--rw-r--r--   0     1001      121      787 2021-09-18 12:23:02.000000 polars-0.9.8/local_dependencies/polars-lazy/src/physical_plan/executors/filter.rs
--rw-r--r--   0     1001      121    11695 2021-09-18 12:23:02.000000 polars-0.9.8/local_dependencies/polars-lazy/src/physical_plan/executors/groupby.rs
--rw-r--r--   0     1001      121     2527 2021-09-18 12:23:02.000000 polars-0.9.8/local_dependencies/polars-lazy/src/physical_plan/executors/join.rs
--rw-r--r--   0     1001      121      460 2021-09-18 12:23:02.000000 polars-0.9.8/local_dependencies/polars-lazy/src/physical_plan/executors/melt.rs
--rw-r--r--   0     1001      121     2486 2021-09-18 12:23:02.000000 polars-0.9.8/local_dependencies/polars-lazy/src/physical_plan/executors/mod.rs
--rw-r--r--   0     1001      121      823 2021-09-18 12:23:02.000000 polars-0.9.8/local_dependencies/polars-lazy/src/physical_plan/executors/projection.rs
--rw-r--r--   0     1001      121     6636 2021-09-18 12:23:02.000000 polars-0.9.8/local_dependencies/polars-lazy/src/physical_plan/executors/scan.rs
--rw-r--r--   0     1001      121      403 2021-09-18 12:23:02.000000 polars-0.9.8/local_dependencies/polars-lazy/src/physical_plan/executors/slice.rs
--rw-r--r--   0     1001      121     1301 2021-09-18 12:23:02.000000 polars-0.9.8/local_dependencies/polars-lazy/src/physical_plan/executors/sort.rs
--rw-r--r--   0     1001      121     1305 2021-09-18 12:23:02.000000 polars-0.9.8/local_dependencies/polars-lazy/src/physical_plan/executors/stack.rs
--rw-r--r--   0     1001      121      411 2021-09-18 12:23:02.000000 polars-0.9.8/local_dependencies/polars-lazy/src/physical_plan/executors/udf.rs
--rw-r--r--   0     1001      121    11023 2021-09-18 12:23:02.000000 polars-0.9.8/local_dependencies/polars-lazy/src/physical_plan/expressions/aggregation.rs
--rw-r--r--   0     1001      121     2074 2021-09-18 12:23:02.000000 polars-0.9.8/local_dependencies/polars-lazy/src/physical_plan/expressions/alias.rs
--rw-r--r--   0     1001      121     5798 2021-09-18 12:23:02.000000 polars-0.9.8/local_dependencies/polars-lazy/src/physical_plan/expressions/apply.rs
--rw-r--r--   0     1001      121     4758 2021-09-18 12:23:02.000000 polars-0.9.8/local_dependencies/polars-lazy/src/physical_plan/expressions/binary.rs
--rw-r--r--   0     1001      121     5598 2021-09-18 12:23:02.000000 polars-0.9.8/local_dependencies/polars-lazy/src/physical_plan/expressions/binary_function.rs
--rw-r--r--   0     1001      121     2033 2021-09-18 12:23:02.000000 polars-0.9.8/local_dependencies/polars-lazy/src/physical_plan/expressions/cast.rs
--rw-r--r--   0     1001      121     1297 2021-09-18 12:23:02.000000 polars-0.9.8/local_dependencies/polars-lazy/src/physical_plan/expressions/column.rs
--rw-r--r--   0     1001      121     2019 2021-09-18 12:23:02.000000 polars-0.9.8/local_dependencies/polars-lazy/src/physical_plan/expressions/filter.rs
--rw-r--r--   0     1001      121     1273 2021-09-18 12:23:02.000000 polars-0.9.8/local_dependencies/polars-lazy/src/physical_plan/expressions/is_not_null.rs
--rw-r--r--   0     1001      121     1253 2021-09-18 12:23:02.000000 polars-0.9.8/local_dependencies/polars-lazy/src/physical_plan/expressions/is_null.rs
--rw-r--r--   0     1001      121     5822 2021-09-18 12:23:02.000000 polars-0.9.8/local_dependencies/polars-lazy/src/physical_plan/expressions/literal.rs
--rw-r--r--   0     1001      121    12535 2021-09-18 12:23:02.000000 polars-0.9.8/local_dependencies/polars-lazy/src/physical_plan/expressions/mod.rs
--rw-r--r--   0     1001      121     1428 2021-09-18 12:23:02.000000 polars-0.9.8/local_dependencies/polars-lazy/src/physical_plan/expressions/not.rs
--rw-r--r--   0     1001      121     2198 2021-09-18 12:23:02.000000 polars-0.9.8/local_dependencies/polars-lazy/src/physical_plan/expressions/shift.rs
--rw-r--r--   0     1001      121     2000 2021-09-18 12:23:02.000000 polars-0.9.8/local_dependencies/polars-lazy/src/physical_plan/expressions/slice.rs
--rw-r--r--   0     1001      121     2756 2021-09-18 12:23:02.000000 polars-0.9.8/local_dependencies/polars-lazy/src/physical_plan/expressions/sort.rs
--rw-r--r--   0     1001      121     3986 2021-09-18 12:23:02.000000 polars-0.9.8/local_dependencies/polars-lazy/src/physical_plan/expressions/sortby.rs
--rw-r--r--   0     1001      121     1599 2021-09-18 12:23:02.000000 polars-0.9.8/local_dependencies/polars-lazy/src/physical_plan/expressions/take.rs
--rw-r--r--   0     1001      121     1797 2021-09-18 12:23:02.000000 polars-0.9.8/local_dependencies/polars-lazy/src/physical_plan/expressions/ternary.rs
--rw-r--r--   0     1001      121      779 2021-09-18 12:23:02.000000 polars-0.9.8/local_dependencies/polars-lazy/src/physical_plan/expressions/utils.rs
--rw-r--r--   0     1001      121     5219 2021-09-18 12:23:02.000000 polars-0.9.8/local_dependencies/polars-lazy/src/physical_plan/expressions/window.rs
--rw-r--r--   0     1001      121     1131 2021-09-18 12:23:02.000000 polars-0.9.8/local_dependencies/polars-lazy/src/physical_plan/mod.rs
--rw-r--r--   0     1001      121    42925 2021-09-18 12:23:02.000000 polars-0.9.8/local_dependencies/polars-lazy/src/physical_plan/planner.rs
--rw-r--r--   0     1001      121     1969 2021-09-18 12:23:02.000000 polars-0.9.8/local_dependencies/polars-lazy/src/physical_plan/state.rs
--rw-r--r--   0     1001      121     1730 2021-09-18 12:23:02.000000 polars-0.9.8/local_dependencies/polars-lazy/src/prelude.rs
--rw-r--r--   0     1001      121    46889 2021-09-18 12:23:02.000000 polars-0.9.8/local_dependencies/polars-lazy/src/test.rs
--rw-r--r--   0     1001      121    10120 2021-09-18 12:23:02.000000 polars-0.9.8/local_dependencies/polars-lazy/src/utils.rs
--rw-r--r--   0        0        0     2836 1970-01-01 00:00:00.000000 polars-0.9.8/local_dependencies/polars-core/Cargo.toml
--rw-r--r--   0     1001      121    15272 2021-09-18 12:23:02.000000 polars-0.9.8/local_dependencies/polars-core/src/chunked_array/arithmetic.rs
--rw-r--r--   0     1001      121      323 2021-09-18 12:23:02.000000 polars-0.9.8/local_dependencies/polars-core/src/chunked_array/boolean.rs
--rw-r--r--   0     1001      121     7160 2021-09-18 12:23:02.000000 polars-0.9.8/local_dependencies/polars-core/src/chunked_array/builder/categorical.rs
--rw-r--r--   0     1001      121    20347 2021-09-18 12:23:02.000000 polars-0.9.8/local_dependencies/polars-core/src/chunked_array/builder/mod.rs
--rw-r--r--   0     1001      121    11474 2021-09-18 12:23:02.000000 polars-0.9.8/local_dependencies/polars-core/src/chunked_array/cast.rs
--rw-r--r--   0     1001      121     1712 2021-09-18 12:23:02.000000 polars-0.9.8/local_dependencies/polars-core/src/chunked_array/categorical/mod.rs
--rw-r--r--   0     1001      121    32451 2021-09-18 12:23:02.000000 polars-0.9.8/local_dependencies/polars-core/src/chunked_array/comparison.rs
--rw-r--r--   0     1001      121      611 2021-09-18 12:23:02.000000 polars-0.9.8/local_dependencies/polars-core/src/chunked_array/float.rs
--rw-r--r--   0     1001      121    34608 2021-09-18 12:23:02.000000 polars-0.9.8/local_dependencies/polars-core/src/chunked_array/iterator/mod.rs
--rw-r--r--   0     1001      121    16814 2021-09-18 12:23:02.000000 polars-0.9.8/local_dependencies/polars-core/src/chunked_array/iterator/par/boolean.rs
--rw-r--r--   0     1001      121     1585 2021-09-18 12:23:02.000000 polars-0.9.8/local_dependencies/polars-core/src/chunked_array/iterator/par/list.rs
--rw-r--r--   0     1001      121    32979 2021-09-18 12:23:02.000000 polars-0.9.8/local_dependencies/polars-core/src/chunked_array/iterator/par/macros.rs
--rw-r--r--   0     1001      121     1935 2021-09-18 12:23:02.000000 polars-0.9.8/local_dependencies/polars-core/src/chunked_array/iterator/par/mod.rs
--rw-r--r--   0     1001      121    40847 2021-09-18 12:23:02.000000 polars-0.9.8/local_dependencies/polars-core/src/chunked_array/iterator/par/numeric.rs
--rw-r--r--   0     1001      121    16173 2021-09-18 12:23:02.000000 polars-0.9.8/local_dependencies/polars-core/src/chunked_array/iterator/par/utf8.rs
--rw-r--r--   0     1001      121     2224 2021-09-18 12:23:02.000000 polars-0.9.8/local_dependencies/polars-core/src/chunked_array/kernels/mod.rs
--rw-r--r--   0     1001      121      460 2021-09-18 12:23:02.000000 polars-0.9.8/local_dependencies/polars-core/src/chunked_array/kernels/strings.rs
--rw-r--r--   0     1001      121    19790 2021-09-18 12:23:02.000000 polars-0.9.8/local_dependencies/polars-core/src/chunked_array/kernels/take.rs
--rw-r--r--   0     1001      121     2409 2021-09-18 12:23:02.000000 polars-0.9.8/local_dependencies/polars-core/src/chunked_array/kernels/take_agg.rs
--rw-r--r--   0     1001      121     2965 2021-09-18 12:23:02.000000 polars-0.9.8/local_dependencies/polars-core/src/chunked_array/kernels/temporal.rs
--rw-r--r--   0     1001      121     5647 2021-09-18 12:23:02.000000 polars-0.9.8/local_dependencies/polars-core/src/chunked_array/list/iterator.rs
--rw-r--r--   0     1001      121      327 2021-09-18 12:23:02.000000 polars-0.9.8/local_dependencies/polars-core/src/chunked_array/list/mod.rs
--rw-r--r--   0     1001      121     3303 2021-09-18 12:23:02.000000 polars-0.9.8/local_dependencies/polars-core/src/chunked_array/list/namespace.rs
--rw-r--r--   0     1001      121    35705 2021-09-18 12:23:02.000000 polars-0.9.8/local_dependencies/polars-core/src/chunked_array/mod.rs
--rw-r--r--   0     1001      121     4026 2021-09-18 12:23:02.000000 polars-0.9.8/local_dependencies/polars-core/src/chunked_array/ndarray.rs
--rw-r--r--   0     1001      121     3902 2021-09-18 12:23:02.000000 polars-0.9.8/local_dependencies/polars-core/src/chunked_array/object/builder.rs
--rw-r--r--   0     1001      121      136 2021-09-18 12:23:02.000000 polars-0.9.8/local_dependencies/polars-core/src/chunked_array/object/is_valid.rs
--rw-r--r--   0     1001      121     2683 2021-09-18 12:23:02.000000 polars-0.9.8/local_dependencies/polars-core/src/chunked_array/object/iterator.rs
--rw-r--r--   0     1001      121     3848 2021-09-18 12:23:02.000000 polars-0.9.8/local_dependencies/polars-core/src/chunked_array/object/mod.rs
--rw-r--r--   0     1001      121    18611 2021-09-18 12:23:02.000000 polars-0.9.8/local_dependencies/polars-core/src/chunked_array/ops/aggregate.rs
--rw-r--r--   0     1001      121     2690 2021-09-18 12:23:02.000000 polars-0.9.8/local_dependencies/polars-core/src/chunked_array/ops/any_value.rs
--rw-r--r--   0     1001      121    19701 2021-09-18 12:23:02.000000 polars-0.9.8/local_dependencies/polars-core/src/chunked_array/ops/apply.rs
--rw-r--r--   0     1001      121     3328 2021-09-18 12:23:02.000000 polars-0.9.8/local_dependencies/polars-core/src/chunked_array/ops/bit_repr.rs
--rw-r--r--   0     1001      121     4048 2021-09-18 12:23:02.000000 polars-0.9.8/local_dependencies/polars-core/src/chunked_array/ops/chunkops.rs
--rw-r--r--   0     1001      121    10474 2021-09-18 12:23:02.000000 polars-0.9.8/local_dependencies/polars-core/src/chunked_array/ops/compare_inner.rs
--rw-r--r--   0     1001      121     4349 2021-09-18 12:23:02.000000 polars-0.9.8/local_dependencies/polars-core/src/chunked_array/ops/cum_agg.rs
--rw-r--r--   0     1001      121     4802 2021-09-18 12:23:02.000000 polars-0.9.8/local_dependencies/polars-core/src/chunked_array/ops/downcast.rs
--rw-r--r--   0     1001      121    15096 2021-09-18 12:23:02.000000 polars-0.9.8/local_dependencies/polars-core/src/chunked_array/ops/explode.rs
--rw-r--r--   0     1001      121    10183 2021-09-18 12:23:02.000000 polars-0.9.8/local_dependencies/polars-core/src/chunked_array/ops/fill_null.rs
--rw-r--r--   0     1001      121     5535 2021-09-18 12:23:02.000000 polars-0.9.8/local_dependencies/polars-core/src/chunked_array/ops/filter.rs
--rw-r--r--   0     1001      121     5977 2021-09-18 12:23:02.000000 polars-0.9.8/local_dependencies/polars-core/src/chunked_array/ops/interpolate.rs
--rw-r--r--   0     1001      121     7556 2021-09-18 12:23:02.000000 polars-0.9.8/local_dependencies/polars-core/src/chunked_array/ops/is_in.rs
--rw-r--r--   0     1001      121    33738 2021-09-18 12:23:02.000000 polars-0.9.8/local_dependencies/polars-core/src/chunked_array/ops/mod.rs
--rw-r--r--   0     1001      121      995 2021-09-18 12:23:02.000000 polars-0.9.8/local_dependencies/polars-core/src/chunked_array/ops/peaks.rs
--rw-r--r--   0     1001      121     2287 2021-09-18 12:23:02.000000 polars-0.9.8/local_dependencies/polars-core/src/chunked_array/ops/repeat_by.rs
--rw-r--r--   0     1001      121    16644 2021-09-18 12:23:02.000000 polars-0.9.8/local_dependencies/polars-core/src/chunked_array/ops/rolling_window.rs
--rw-r--r--   0     1001      121    12149 2021-09-18 12:23:02.000000 polars-0.9.8/local_dependencies/polars-core/src/chunked_array/ops/set.rs
--rw-r--r--   0     1001      121     5802 2021-09-18 12:23:02.000000 polars-0.9.8/local_dependencies/polars-core/src/chunked_array/ops/shift.rs
--rw-r--r--   0     1001      121    16679 2021-09-18 12:23:02.000000 polars-0.9.8/local_dependencies/polars-core/src/chunked_array/ops/sort.rs
--rw-r--r--   0     1001      121    19985 2021-09-18 12:23:02.000000 polars-0.9.8/local_dependencies/polars-core/src/chunked_array/ops/take/mod.rs
--rw-r--r--   0     1001      121     1931 2021-09-18 12:23:02.000000 polars-0.9.8/local_dependencies/polars-core/src/chunked_array/ops/take/take_every.rs
--rw-r--r--   0     1001      121    13541 2021-09-18 12:23:02.000000 polars-0.9.8/local_dependencies/polars-core/src/chunked_array/ops/take/take_random.rs
--rw-r--r--   0     1001      121     5081 2021-09-18 12:23:02.000000 polars-0.9.8/local_dependencies/polars-core/src/chunked_array/ops/take/take_single.rs
--rw-r--r--   0     1001      121     4751 2021-09-18 12:23:02.000000 polars-0.9.8/local_dependencies/polars-core/src/chunked_array/ops/take/traits.rs
--rw-r--r--   0     1001      121    19214 2021-09-18 12:23:02.000000 polars-0.9.8/local_dependencies/polars-core/src/chunked_array/ops/unique/mod.rs
--rw-r--r--   0     1001      121     5200 2021-09-18 12:23:02.000000 polars-0.9.8/local_dependencies/polars-core/src/chunked_array/ops/unique/rank.rs
--rw-r--r--   0     1001      121     7040 2021-09-18 12:23:02.000000 polars-0.9.8/local_dependencies/polars-core/src/chunked_array/ops/zip.rs
--rw-r--r--   0     1001      121     6324 2021-09-18 12:23:02.000000 polars-0.9.8/local_dependencies/polars-core/src/chunked_array/random.rs
--rw-r--r--   0     1001      121     1170 2021-09-18 12:23:02.000000 polars-0.9.8/local_dependencies/polars-core/src/chunked_array/strings/json_path.rs
--rw-r--r--   0     1001      121     2333 2021-09-18 12:23:02.000000 polars-0.9.8/local_dependencies/polars-core/src/chunked_array/strings/mod.rs
--rw-r--r--   0     1001      121    15928 2021-09-18 12:23:02.000000 polars-0.9.8/local_dependencies/polars-core/src/chunked_array/temporal/conversion.rs
--rw-r--r--   0     1001      121     1852 2021-09-18 12:23:02.000000 polars-0.9.8/local_dependencies/polars-core/src/chunked_array/temporal/conversions_utils.rs
--rw-r--r--   0     1001      121     1901 2021-09-18 12:23:02.000000 polars-0.9.8/local_dependencies/polars-core/src/chunked_array/temporal/mod.rs
--rw-r--r--   0     1001      121     3469 2021-09-18 12:23:02.000000 polars-0.9.8/local_dependencies/polars-core/src/chunked_array/trusted_len.rs
--rw-r--r--   0     1001      121    13354 2021-09-18 12:23:02.000000 polars-0.9.8/local_dependencies/polars-core/src/chunked_array/upstream_traits.rs
--rw-r--r--   0     1001      121    21954 2021-09-18 12:23:02.000000 polars-0.9.8/local_dependencies/polars-core/src/datatypes.rs
--rw-r--r--   0     1001      121      118 2021-09-18 12:23:02.000000 polars-0.9.8/local_dependencies/polars-core/src/doc/changelog/mod.rs
--rw-r--r--   0     1001      121      898 2021-09-18 12:23:02.000000 polars-0.9.8/local_dependencies/polars-core/src/doc/changelog/v0_10_0_11.rs
--rw-r--r--   0     1001      121      481 2021-09-18 12:23:02.000000 polars-0.9.8/local_dependencies/polars-core/src/doc/changelog/v0_3.rs
--rw-r--r--   0     1001      121      293 2021-09-18 12:23:02.000000 polars-0.9.8/local_dependencies/polars-core/src/doc/changelog/v0_4.rs
--rw-r--r--   0     1001      121      499 2021-09-18 12:23:02.000000 polars-0.9.8/local_dependencies/polars-core/src/doc/changelog/v0_5.rs
--rw-r--r--   0     1001      121      288 2021-09-18 12:23:02.000000 polars-0.9.8/local_dependencies/polars-core/src/doc/changelog/v0_6.rs
--rw-r--r--   0     1001      121     1072 2021-09-18 12:23:02.000000 polars-0.9.8/local_dependencies/polars-core/src/doc/changelog/v0_7.rs
--rw-r--r--   0     1001      121      817 2021-09-18 12:23:02.000000 polars-0.9.8/local_dependencies/polars-core/src/doc/changelog/v0_8.rs
--rw-r--r--   0     1001      121      596 2021-09-18 12:23:02.000000 polars-0.9.8/local_dependencies/polars-core/src/doc/changelog/v0_9.rs
--rw-r--r--   0     1001      121       86 2021-09-18 12:23:02.000000 polars-0.9.8/local_dependencies/polars-core/src/doc/mod.rs
--rw-r--r--   0     1001      121     3007 2021-09-18 12:23:02.000000 polars-0.9.8/local_dependencies/polars-core/src/doc/time.rs
--rw-r--r--   0     1001      121     1654 2021-09-18 12:23:02.000000 polars-0.9.8/local_dependencies/polars-core/src/error.rs
--rw-r--r--   0     1001      121       15 2021-09-18 12:23:02.000000 polars-0.9.8/local_dependencies/polars-core/src/export.rs
--rw-r--r--   0     1001      121    23250 2021-09-18 12:23:02.000000 polars-0.9.8/local_dependencies/polars-core/src/fmt.rs
--rw-r--r--   0     1001      121     2488 2021-09-18 12:23:02.000000 polars-0.9.8/local_dependencies/polars-core/src/frame/arithmetic.rs
--rw-r--r--   0     1001      121     6719 2021-09-18 12:23:02.000000 polars-0.9.8/local_dependencies/polars-core/src/frame/asof_join.rs
--rw-r--r--   0     1001      121     1890 2021-09-18 12:23:02.000000 polars-0.9.8/local_dependencies/polars-core/src/frame/cross_join.rs
--rw-r--r--   0     1001      121     9799 2021-09-18 12:23:02.000000 polars-0.9.8/local_dependencies/polars-core/src/frame/explode.rs
--rw-r--r--   0     1001      121    22890 2021-09-18 12:23:02.000000 polars-0.9.8/local_dependencies/polars-core/src/frame/groupby/aggregations.rs
--rw-r--r--   0     1001      121    10541 2021-09-18 12:23:02.000000 polars-0.9.8/local_dependencies/polars-core/src/frame/groupby/hashing.rs
--rw-r--r--   0     1001      121    52773 2021-09-18 12:23:02.000000 polars-0.9.8/local_dependencies/polars-core/src/frame/groupby/mod.rs
--rw-r--r--   0     1001      121    21385 2021-09-18 12:23:02.000000 polars-0.9.8/local_dependencies/polars-core/src/frame/groupby/pivot.rs
--rw-r--r--   0     1001      121    19949 2021-09-18 12:23:02.000000 polars-0.9.8/local_dependencies/polars-core/src/frame/groupby/resample.rs
--rw-r--r--   0     1001      121    57841 2021-09-18 12:23:02.000000 polars-0.9.8/local_dependencies/polars-core/src/frame/hash_join/mod.rs
--rw-r--r--   0     1001      121    13377 2021-09-18 12:23:02.000000 polars-0.9.8/local_dependencies/polars-core/src/frame/hash_join/multiple_keys.rs
--rw-r--r--   0     1001      121    70052 2021-09-18 12:23:02.000000 polars-0.9.8/local_dependencies/polars-core/src/frame/mod.rs
--rw-r--r--   0     1001      121    12482 2021-09-18 12:23:02.000000 polars-0.9.8/local_dependencies/polars-core/src/frame/row.rs
--rw-r--r--   0     1001      121     2392 2021-09-18 12:23:02.000000 polars-0.9.8/local_dependencies/polars-core/src/frame/select.rs
--rw-r--r--   0     1001      121     1381 2021-09-18 12:23:02.000000 polars-0.9.8/local_dependencies/polars-core/src/frame/upstream_traits.rs
--rw-r--r--   0     1001      121     5096 2021-09-18 12:23:02.000000 polars-0.9.8/local_dependencies/polars-core/src/functions.rs
--rw-r--r--   0     1001      121     3516 2021-09-18 12:23:02.000000 polars-0.9.8/local_dependencies/polars-core/src/lib.rs
--rw-r--r--   0     1001      121     1729 2021-09-18 12:23:02.000000 polars-0.9.8/local_dependencies/polars-core/src/prelude.rs
--rw-r--r--   0     1001      121     2574 2021-09-18 12:23:02.000000 polars-0.9.8/local_dependencies/polars-core/src/serde/chunked_array.rs
--rw-r--r--   0     1001      121     3109 2021-09-18 12:23:02.000000 polars-0.9.8/local_dependencies/polars-core/src/serde/mod.rs
--rw-r--r--   0     1001      121     7553 2021-09-18 12:23:02.000000 polars-0.9.8/local_dependencies/polars-core/src/serde/series.rs
--rw-r--r--   0     1001      121    22184 2021-09-18 12:23:02.000000 polars-0.9.8/local_dependencies/polars-core/src/series/arithmetic.rs
--rw-r--r--   0     1001      121     8321 2021-09-18 12:23:02.000000 polars-0.9.8/local_dependencies/polars-core/src/series/comparison.rs
--rw-r--r--   0     1001      121    28200 2021-09-18 12:23:02.000000 polars-0.9.8/local_dependencies/polars-core/src/series/implementations/dates.rs
--rw-r--r--   0     1001      121    33418 2021-09-18 12:23:02.000000 polars-0.9.8/local_dependencies/polars-core/src/series/implementations/mod.rs
--rw-r--r--   0     1001      121     9311 2021-09-18 12:23:02.000000 polars-0.9.8/local_dependencies/polars-core/src/series/implementations/object.rs
--rw-r--r--   0     1001      121     2198 2021-09-18 12:23:02.000000 polars-0.9.8/local_dependencies/polars-core/src/series/iterator.rs
--rw-r--r--   0     1001      121    68176 2021-09-18 12:23:02.000000 polars-0.9.8/local_dependencies/polars-core/src/series/mod.rs
--rw-r--r--   0     1001      121      473 2021-09-18 12:23:02.000000 polars-0.9.8/local_dependencies/polars-core/src/series/ops/diff.rs
--rw-r--r--   0     1001      121      207 2021-09-18 12:23:02.000000 polars-0.9.8/local_dependencies/polars-core/src/series/ops/mod.rs
--rw-r--r--   0     1001      121     5049 2021-09-18 12:23:02.000000 polars-0.9.8/local_dependencies/polars-core/src/series/ops/moment.rs
--rw-r--r--   0     1001      121     1208 2021-09-18 12:23:02.000000 polars-0.9.8/local_dependencies/polars-core/src/series/ops/to_list.rs
--rw-r--r--   0     1001      121     3561 2021-09-18 12:23:02.000000 polars-0.9.8/local_dependencies/polars-core/src/testing.rs
--rw-r--r--   0     1001      121    27597 2021-09-18 12:23:02.000000 polars-0.9.8/local_dependencies/polars-core/src/utils.rs
--rw-r--r--   0     1001      121    16835 2021-09-18 12:23:02.000000 polars-0.9.8/local_dependencies/polars-core/src/vector_hasher.rs
--rw-r--r--   0        0        0     1628 1970-01-01 00:00:00.000000 polars-0.9.8/Cargo.toml
--rw-r--r--   0     1001      121      169 2021-09-18 12:23:02.000000 polars-0.9.8/.flake8
--rw-r--r--   0     1001      121       28 2021-09-18 12:23:02.000000 polars-0.9.8/.gitignore
--rw-r--r--   0     1001      121    11235 2021-09-18 12:23:02.000000 polars-0.9.8/CHANGELOG.md
--rw-r--r--   0     1001      121       71 2021-09-18 12:23:02.000000 polars-0.9.8/Makefile
--rw-r--r--   0        0        0     7807 2021-09-18 12:23:03.000000 polars-0.9.8/README.md
--rw-r--r--   0     1001      121      397 2021-09-18 12:23:02.000000 polars-0.9.8/build.requirements.txt
--rw-r--r--   0     1001      121       36 2021-09-18 12:23:02.000000 polars-0.9.8/docs/.gitignore
--rw-r--r--   0     1001      121      638 2021-09-18 12:23:02.000000 polars-0.9.8/docs/Makefile
--rw-r--r--   0     1001      121      318 2021-09-18 12:23:02.000000 polars-0.9.8/docs/_templates/api_redirect.html
--rw-r--r--   0     1001      121      151 2021-09-18 12:23:02.000000 polars-0.9.8/docs/_templates/autosummary/accessor.rst
--rw-r--r--   0     1001      121      160 2021-09-18 12:23:02.000000 polars-0.9.8/docs/_templates/autosummary/accessor_attribute.rst
--rw-r--r--   0     1001      121      168 2021-09-18 12:23:02.000000 polars-0.9.8/docs/_templates/autosummary/accessor_callable.rst
--rw-r--r--   0     1001      121      157 2021-09-18 12:23:02.000000 polars-0.9.8/docs/_templates/autosummary/accessor_method.rst
--rw-r--r--   0     1001      121      836 2021-09-18 12:23:02.000000 polars-0.9.8/docs/_templates/autosummary/class.rst
--rw-r--r--   0     1001      121       94 2021-09-18 12:23:02.000000 polars-0.9.8/docs/_templates/autosummary/class_without_autosummary.rst
--rw-r--r--   0     1001      121      406 2021-09-18 12:23:02.000000 polars-0.9.8/docs/_templates/sidebar-nav-bs.html
--rw-r--r--   0     1001      121     3239 2021-09-18 12:23:02.000000 polars-0.9.8/docs/img/polars_logo.png
--rw-r--r--   0     1001      121     2690 2021-09-18 12:23:02.000000 polars-0.9.8/docs/source/conf.py
--rw-r--r--   0     1001      121       51 2021-09-18 12:23:02.000000 polars-0.9.8/docs/source/index.rst
--rw-r--r--   0     1001      121      343 2021-09-18 12:23:02.000000 polars-0.9.8/docs/source/reference/config.rst
--rw-r--r--   0     1001      121     3083 2021-09-18 12:23:02.000000 polars-0.9.8/docs/source/reference/dataframe.rst
--rw-r--r--   0     1001      121     4262 2021-09-18 12:23:02.000000 polars-0.9.8/docs/source/reference/expression.rst
--rw-r--r--   0     1001      121      417 2021-09-18 12:23:02.000000 polars-0.9.8/docs/source/reference/functions.rst
--rw-r--r--   0     1001      121      307 2021-09-18 12:23:02.000000 polars-0.9.8/docs/source/reference/index.rst
--rw-r--r--   0     1001      121      517 2021-09-18 12:23:02.000000 polars-0.9.8/docs/source/reference/io.rst
--rw-r--r--   0     1001      121     1584 2021-09-18 12:23:02.000000 polars-0.9.8/docs/source/reference/lazyframe.rst
--rw-r--r--   0     1001      121     4111 2021-09-18 12:23:02.000000 polars-0.9.8/docs/source/reference/series.rst
--rw-r--r--   0     1001      121      205 2021-09-18 12:23:02.000000 polars-0.9.8/legacy/README.md
--rwxr-xr-x   0     1001      121       86 2021-09-18 12:23:02.000000 polars-0.9.8/legacy/deploy.sh
--rw-r--r--   0     1001      121      202 2021-09-18 12:23:02.000000 polars-0.9.8/legacy/pypolars/__init__.py
--rw-r--r--   0     1001      121       31 2021-09-18 12:23:02.000000 polars-0.9.8/legacy/pypolars/datatypes.py
--rw-r--r--   0     1001      121       27 2021-09-18 12:23:02.000000 polars-0.9.8/legacy/pypolars/frame.py
--rw-r--r--   0     1001      121       31 2021-09-18 12:23:02.000000 polars-0.9.8/legacy/pypolars/functions.py
--rw-r--r--   0     1001      121       26 2021-09-18 12:23:02.000000 polars-0.9.8/legacy/pypolars/lazy.py
--rw-r--r--   0     1001      121       28 2021-09-18 12:23:02.000000 polars-0.9.8/legacy/pypolars/series.py
--rw-r--r--   0     1001      121      554 2021-09-18 12:23:02.000000 polars-0.9.8/legacy/setup.py
--rw-r--r--   0     1001      121     1011 2021-09-18 12:23:02.000000 polars-0.9.8/polars/__init__.py
--rw-r--r--   0     1001      121     5440 2021-09-18 12:23:02.000000 polars-0.9.8/polars/_html.py
--rw-r--r--   0     1001      121     1867 2021-09-18 12:23:02.000000 polars-0.9.8/polars/cfg.py
--rw-r--r--   0     1001      121     9413 2021-09-18 12:23:02.000000 polars-0.9.8/polars/convert.py
--rw-r--r--   0     1001      121     6475 2021-09-18 12:23:02.000000 polars-0.9.8/polars/datatypes.py
--rw-r--r--   0     1001      121      128 2021-09-18 12:23:02.000000 polars-0.9.8/polars/eager/__init__.py
--rw-r--r--   0     1001      121   119083 2021-09-18 12:23:02.000000 polars-0.9.8/polars/eager/frame.py
--rw-r--r--   0     1001      121    87511 2021-09-18 12:23:02.000000 polars-0.9.8/polars/eager/series.py
--rw-r--r--   0     1001      121     1810 2021-09-18 12:23:02.000000 polars-0.9.8/polars/functions.py
--rw-r--r--   0     1001      121        0 2021-09-18 12:23:02.000000 polars-0.9.8/polars/internals/__init__.py
--rw-r--r--   0     1001      121    11018 2021-09-18 12:23:02.000000 polars-0.9.8/polars/internals/construction.py
--rw-r--r--   0     1001      121    19661 2021-09-18 12:23:02.000000 polars-0.9.8/polars/io.py
--rw-r--r--   0     1001      121      231 2021-09-18 12:23:02.000000 polars-0.9.8/polars/lazy/__init__.py
--rw-r--r--   0     1001      121    68958 2021-09-18 12:23:02.000000 polars-0.9.8/polars/lazy/expr.py
--rw-r--r--   0     1001      121    32330 2021-09-18 12:23:02.000000 polars-0.9.8/polars/lazy/frame.py
--rw-r--r--   0     1001      121    17383 2021-09-18 12:23:02.000000 polars-0.9.8/polars/lazy/functions.py
--rw-r--r--   0     1001      121     3029 2021-09-18 12:23:02.000000 polars-0.9.8/polars/lazy/whenthen.py
--rw-r--r--   0     1001      121        0 2021-09-18 12:23:02.000000 polars-0.9.8/polars/py.typed
--rw-r--r--   0     1001      121     1094 2021-09-18 12:23:02.000000 polars-0.9.8/polars/string_cache.py
--rw-r--r--   0     1001      121     2874 2021-09-18 12:23:02.000000 polars-0.9.8/polars/utils.py
--rw-r--r--   0     1001      121      423 2021-09-18 12:23:02.000000 polars-0.9.8/pyproject.toml
--rw-r--r--   0     1001      121        8 2021-09-18 12:23:02.000000 polars-0.9.8/rust-toolchain
--rw-r--r--   0     1001      121     6385 2021-09-18 12:23:02.000000 polars-0.9.8/src/apply/dataframe.rs
--rw-r--r--   0     1001      121     4250 2021-09-18 12:23:02.000000 polars-0.9.8/src/apply/mod.rs
--rw-r--r--   0     1001      121    59591 2021-09-18 12:23:02.000000 polars-0.9.8/src/apply/series.rs
--rw-r--r--   0     1001      121       32 2021-09-18 12:23:02.000000 polars-0.9.8/src/arrow_interop/mod.rs
--rw-r--r--   0     1001      121     1625 2021-09-18 12:23:02.000000 polars-0.9.8/src/arrow_interop/to_py.rs
--rw-r--r--   0     1001      121     2115 2021-09-18 12:23:02.000000 polars-0.9.8/src/arrow_interop/to_rust.rs
--rw-r--r--   0     1001      121    13200 2021-09-18 12:23:02.000000 polars-0.9.8/src/conversion.rs
--rw-r--r--   0     1001      121    30850 2021-09-18 12:23:02.000000 polars-0.9.8/src/dataframe.rs
--rw-r--r--   0     1001      121     1919 2021-09-18 12:23:02.000000 polars-0.9.8/src/datatypes.rs
--rw-r--r--   0     1001      121      501 2021-09-18 12:23:02.000000 polars-0.9.8/src/error.rs
--rw-r--r--   0     1001      121     8541 2021-09-18 12:23:02.000000 polars-0.9.8/src/file.rs
--rw-r--r--   0     1001      121    13767 2021-09-18 12:23:02.000000 polars-0.9.8/src/lazy/dataframe.rs
--rw-r--r--   0     1001      121    36077 2021-09-18 12:23:02.000000 polars-0.9.8/src/lazy/dsl.rs
--rw-r--r--   0     1001      121       47 2021-09-18 12:23:02.000000 polars-0.9.8/src/lazy/mod.rs
--rw-r--r--   0     1001      121      211 2021-09-18 12:23:02.000000 polars-0.9.8/src/lazy/utils.rs
--rw-r--r--   0     1001      121     5164 2021-09-18 12:23:02.000000 polars-0.9.8/src/lib.rs
--rw-r--r--   0     1001      121     1547 2021-09-18 12:23:02.000000 polars-0.9.8/src/npy.rs
--rw-r--r--   0     1001      121       87 2021-09-18 12:23:02.000000 polars-0.9.8/src/prelude.rs
--rw-r--r--   0     1001      121    53916 2021-09-18 12:23:02.000000 polars-0.9.8/src/series.rs
--rw-r--r--   0     1001      121     2542 2021-09-18 12:23:02.000000 polars-0.9.8/src/utils.rs
--rwxr-xr-x   0     1001      121      869 2021-09-18 12:23:02.000000 polars-0.9.8/tasks.sh
--rw-r--r--   0     1001      121      786 2021-09-18 12:23:02.000000 polars-0.9.8/tests/conftest.py
--rw-r--r--   0     1001      121     2189 2021-09-18 12:23:02.000000 polars-0.9.8/tests/db-benchmark/groupby-datagen.R
--rw-r--r--   0     1001      121     6860 2021-09-18 12:23:02.000000 polars-0.9.8/tests/db-benchmark/main.py
--rw-r--r--   0     1001      121       49 2021-09-18 12:23:02.000000 polars-0.9.8/tests/files/gzipped.csv
--rw-r--r--   0     1001      121    31940 2021-09-18 12:23:02.000000 polars-0.9.8/tests/test_df.py
--rw-r--r--   0     1001      121     1488 2021-09-18 12:23:02.000000 polars-0.9.8/tests/test_interop.py
--rw-r--r--   0     1001      121     5614 2021-09-18 12:23:02.000000 polars-0.9.8/tests/test_io.py
--rw-r--r--   0     1001      121    15674 2021-09-18 12:23:02.000000 polars-0.9.8/tests/test_lazy.py
--rw-r--r--   0     1001      121    16372 2021-09-18 12:23:02.000000 polars-0.9.8/tests/test_series.py
--rw-r--r--   0        0        0     8182 1970-01-01 00:00:00.000000 polars-0.9.8/PKG-INFO
+-rw-r--r--   0        0        0     4793 1970-01-01 00:00:00.000000 polars-0.9.9/local_dependencies/polars/Cargo.toml
+-rw-r--r--   0     1001      121      941 2021-09-19 07:10:07.000000 polars-0.9.9/local_dependencies/polars/Makefile
+-rw-r--r--   0     1001      121     1966 2021-09-19 07:10:07.000000 polars-0.9.9/local_dependencies/polars/benches/bench.rs
+-rw-r--r--   0     1001      121     2743 2021-09-19 07:10:07.000000 polars-0.9.9/local_dependencies/polars/benches/collect.rs
+-rw-r--r--   0     1001      121      667 2021-09-19 07:10:07.000000 polars-0.9.9/local_dependencies/polars/benches/csv.rs
+-rw-r--r--   0     1001      121     5105 2021-09-19 07:10:07.000000 polars-0.9.9/local_dependencies/polars/benches/groupby.rs
+-rw-r--r--   0     1001      121     2252 2021-09-19 07:10:07.000000 polars-0.9.9/local_dependencies/polars/benches/take.rs
+-rw-r--r--   0     1001      121    19759 2021-09-19 07:10:07.000000 polars-0.9.9/local_dependencies/polars/src/docs/eager.rs
+-rw-r--r--   0     1001      121     9038 2021-09-19 07:10:07.000000 polars-0.9.9/local_dependencies/polars/src/docs/lazy.rs
+-rw-r--r--   0     1001      121       50 2021-09-19 07:10:07.000000 polars-0.9.9/local_dependencies/polars/src/docs/mod.rs
+-rw-r--r--   0     1001      121     3772 2021-09-19 07:10:07.000000 polars-0.9.9/local_dependencies/polars/src/docs/performance.rs
+-rw-r--r--   0     1001      121    11633 2021-09-19 07:10:07.000000 polars-0.9.9/local_dependencies/polars/src/lib.rs
+-rw-r--r--   0     1001      121      170 2021-09-19 07:10:07.000000 polars-0.9.9/local_dependencies/polars/src/prelude.rs
+-rw-r--r--   0        0        0     1659 1970-01-01 00:00:00.000000 polars-0.9.9/local_dependencies/polars-io/Cargo.toml
+-rw-r--r--   0     1001      121    34545 2021-09-19 07:10:07.000000 polars-0.9.9/local_dependencies/polars-io/src/csv.rs
+-rw-r--r--   0     1001      121    15713 2021-09-19 07:10:07.000000 polars-0.9.9/local_dependencies/polars-io/src/csv_core/buffer.rs
+-rw-r--r--   0     1001      121    22465 2021-09-19 07:10:07.000000 polars-0.9.9/local_dependencies/polars-io/src/csv_core/csv.rs
+-rw-r--r--   0     1001      121      158 2021-09-19 07:10:07.000000 polars-0.9.9/local_dependencies/polars-io/src/csv_core/mod.rs
+-rw-r--r--   0     1001      121    16002 2021-09-19 07:10:07.000000 polars-0.9.9/local_dependencies/polars-io/src/csv_core/parser.rs
+-rw-r--r--   0     1001      121    10564 2021-09-19 07:10:07.000000 polars-0.9.9/local_dependencies/polars-io/src/csv_core/utils.rs
+-rw-r--r--   0     1001      121     4211 2021-09-19 07:10:07.000000 polars-0.9.9/local_dependencies/polars-io/src/ipc.rs
+-rw-r--r--   0     1001      121     5733 2021-09-19 07:10:07.000000 polars-0.9.9/local_dependencies/polars-io/src/json.rs
+-rw-r--r--   0     1001      121     5770 2021-09-19 07:10:07.000000 polars-0.9.9/local_dependencies/polars-io/src/lib.rs
+-rw-r--r--   0     1001      121     1226 2021-09-19 07:10:07.000000 polars-0.9.9/local_dependencies/polars-io/src/mmap.rs
+-rw-r--r--   0     1001      121     7935 2021-09-19 07:10:07.000000 polars-0.9.9/local_dependencies/polars-io/src/parquet.rs
+-rw-r--r--   0     1001      121      567 2021-09-19 07:10:07.000000 polars-0.9.9/local_dependencies/polars-io/src/prelude.rs
+-rw-r--r--   0     1001      121      436 2021-09-19 07:10:07.000000 polars-0.9.9/local_dependencies/polars-io/src/tests.rs
+-rw-r--r--   0     1001      121     2093 2021-09-19 07:10:07.000000 polars-0.9.9/local_dependencies/polars-io/src/utils.rs
+-rw-r--r--   0        0        0     1935 1970-01-01 00:00:00.000000 polars-0.9.9/local_dependencies/polars-lazy/Cargo.toml
+-rw-r--r--   0     1001      121    13389 2021-09-19 07:10:07.000000 polars-0.9.9/local_dependencies/polars-lazy/src/datafusion/conversion.rs
+-rw-r--r--   0     1001      121     2393 2021-09-19 07:10:07.000000 polars-0.9.9/local_dependencies/polars-lazy/src/datafusion/mod.rs
+-rw-r--r--   0     1001      121    61867 2021-09-19 07:10:07.000000 polars-0.9.9/local_dependencies/polars-lazy/src/dsl.rs
+-rw-r--r--   0     1001      121      524 2021-09-19 07:10:07.000000 polars-0.9.9/local_dependencies/polars-lazy/src/dummies.rs
+-rw-r--r--   0     1001      121    36544 2021-09-19 07:10:07.000000 polars-0.9.9/local_dependencies/polars-lazy/src/frame.rs
+-rw-r--r--   0     1001      121     6863 2021-09-19 07:10:07.000000 polars-0.9.9/local_dependencies/polars-lazy/src/functions.rs
+-rw-r--r--   0     1001      121     7405 2021-09-19 07:10:07.000000 polars-0.9.9/local_dependencies/polars-lazy/src/lib.rs
+-rw-r--r--   0     1001      121    14547 2021-09-19 07:10:07.000000 polars-0.9.9/local_dependencies/polars-lazy/src/logical_plan/aexpr.rs
+-rw-r--r--   0     1001      121    22886 2021-09-19 07:10:07.000000 polars-0.9.9/local_dependencies/polars-lazy/src/logical_plan/alp.rs
+-rw-r--r--   0     1001      121    25945 2021-09-19 07:10:07.000000 polars-0.9.9/local_dependencies/polars-lazy/src/logical_plan/conversion.rs
+-rw-r--r--   0     1001      121     9320 2021-09-19 07:10:07.000000 polars-0.9.9/local_dependencies/polars-lazy/src/logical_plan/iterator.rs
+-rw-r--r--   0     1001      121    47979 2021-09-19 07:10:07.000000 polars-0.9.9/local_dependencies/polars-lazy/src/logical_plan/mod.rs
+-rw-r--r--   0     1001      121     6336 2021-09-19 07:10:07.000000 polars-0.9.9/local_dependencies/polars-lazy/src/logical_plan/optimizer/aggregate_pushdown.rs
+-rw-r--r--   0     1001      121     6277 2021-09-19 07:10:07.000000 polars-0.9.9/local_dependencies/polars-lazy/src/logical_plan/optimizer/aggregate_scan_projections.rs
+-rw-r--r--   0     1001      121     1960 2021-09-19 07:10:07.000000 polars-0.9.9/local_dependencies/polars-lazy/src/logical_plan/optimizer/drop_nulls.rs
+-rw-r--r--   0     1001      121     2359 2021-09-19 07:10:07.000000 polars-0.9.9/local_dependencies/polars-lazy/src/logical_plan/optimizer/fast_projection.rs
+-rw-r--r--   0     1001      121     7011 2021-09-19 07:10:07.000000 polars-0.9.9/local_dependencies/polars-lazy/src/logical_plan/optimizer/join_pruning.rs
+-rw-r--r--   0     1001      121      762 2021-09-19 07:10:07.000000 polars-0.9.9/local_dependencies/polars-lazy/src/logical_plan/optimizer/mod.rs
+-rw-r--r--   0     1001      121    19264 2021-09-19 07:10:07.000000 polars-0.9.9/local_dependencies/polars-lazy/src/logical_plan/optimizer/predicate_pushdown/mod.rs
+-rw-r--r--   0     1001      121     9945 2021-09-19 07:10:07.000000 polars-0.9.9/local_dependencies/polars-lazy/src/logical_plan/optimizer/predicate_pushdown/utils.rs
+-rw-r--r--   0     1001      121    30562 2021-09-19 07:10:07.000000 polars-0.9.9/local_dependencies/polars-lazy/src/logical_plan/optimizer/projection_pushdown.rs
+-rw-r--r--   0     1001      121    15318 2021-09-19 07:10:07.000000 polars-0.9.9/local_dependencies/polars-lazy/src/logical_plan/optimizer/simplify_expr.rs
+-rw-r--r--   0     1001      121     3083 2021-09-19 07:10:07.000000 polars-0.9.9/local_dependencies/polars-lazy/src/logical_plan/optimizer/stack_opt.rs
+-rw-r--r--   0     1001      121    10231 2021-09-19 07:10:07.000000 polars-0.9.9/local_dependencies/polars-lazy/src/logical_plan/optimizer/type_coercion.rs
+-rw-r--r--   0     1001      121      703 2021-09-19 07:10:07.000000 polars-0.9.9/local_dependencies/polars-lazy/src/physical_plan/executors/cache.rs
+-rw-r--r--   0     1001      121      556 2021-09-19 07:10:07.000000 polars-0.9.9/local_dependencies/polars-lazy/src/physical_plan/executors/drop_duplicates.rs
+-rw-r--r--   0     1001      121      407 2021-09-19 07:10:07.000000 polars-0.9.9/local_dependencies/polars-lazy/src/physical_plan/executors/explode.rs
+-rw-r--r--   0     1001      121      787 2021-09-19 07:10:07.000000 polars-0.9.9/local_dependencies/polars-lazy/src/physical_plan/executors/filter.rs
+-rw-r--r--   0     1001      121    11695 2021-09-19 07:10:07.000000 polars-0.9.9/local_dependencies/polars-lazy/src/physical_plan/executors/groupby.rs
+-rw-r--r--   0     1001      121     2527 2021-09-19 07:10:07.000000 polars-0.9.9/local_dependencies/polars-lazy/src/physical_plan/executors/join.rs
+-rw-r--r--   0     1001      121      460 2021-09-19 07:10:07.000000 polars-0.9.9/local_dependencies/polars-lazy/src/physical_plan/executors/melt.rs
+-rw-r--r--   0     1001      121     2486 2021-09-19 07:10:07.000000 polars-0.9.9/local_dependencies/polars-lazy/src/physical_plan/executors/mod.rs
+-rw-r--r--   0     1001      121      823 2021-09-19 07:10:07.000000 polars-0.9.9/local_dependencies/polars-lazy/src/physical_plan/executors/projection.rs
+-rw-r--r--   0     1001      121     6636 2021-09-19 07:10:07.000000 polars-0.9.9/local_dependencies/polars-lazy/src/physical_plan/executors/scan.rs
+-rw-r--r--   0     1001      121      403 2021-09-19 07:10:07.000000 polars-0.9.9/local_dependencies/polars-lazy/src/physical_plan/executors/slice.rs
+-rw-r--r--   0     1001      121     1301 2021-09-19 07:10:07.000000 polars-0.9.9/local_dependencies/polars-lazy/src/physical_plan/executors/sort.rs
+-rw-r--r--   0     1001      121     1305 2021-09-19 07:10:07.000000 polars-0.9.9/local_dependencies/polars-lazy/src/physical_plan/executors/stack.rs
+-rw-r--r--   0     1001      121      411 2021-09-19 07:10:07.000000 polars-0.9.9/local_dependencies/polars-lazy/src/physical_plan/executors/udf.rs
+-rw-r--r--   0     1001      121    11023 2021-09-19 07:10:07.000000 polars-0.9.9/local_dependencies/polars-lazy/src/physical_plan/expressions/aggregation.rs
+-rw-r--r--   0     1001      121     2074 2021-09-19 07:10:07.000000 polars-0.9.9/local_dependencies/polars-lazy/src/physical_plan/expressions/alias.rs
+-rw-r--r--   0     1001      121     5798 2021-09-19 07:10:07.000000 polars-0.9.9/local_dependencies/polars-lazy/src/physical_plan/expressions/apply.rs
+-rw-r--r--   0     1001      121     4758 2021-09-19 07:10:07.000000 polars-0.9.9/local_dependencies/polars-lazy/src/physical_plan/expressions/binary.rs
+-rw-r--r--   0     1001      121     5598 2021-09-19 07:10:07.000000 polars-0.9.9/local_dependencies/polars-lazy/src/physical_plan/expressions/binary_function.rs
+-rw-r--r--   0     1001      121     2033 2021-09-19 07:10:07.000000 polars-0.9.9/local_dependencies/polars-lazy/src/physical_plan/expressions/cast.rs
+-rw-r--r--   0     1001      121     1297 2021-09-19 07:10:07.000000 polars-0.9.9/local_dependencies/polars-lazy/src/physical_plan/expressions/column.rs
+-rw-r--r--   0     1001      121     2019 2021-09-19 07:10:07.000000 polars-0.9.9/local_dependencies/polars-lazy/src/physical_plan/expressions/filter.rs
+-rw-r--r--   0     1001      121     1273 2021-09-19 07:10:07.000000 polars-0.9.9/local_dependencies/polars-lazy/src/physical_plan/expressions/is_not_null.rs
+-rw-r--r--   0     1001      121     1253 2021-09-19 07:10:07.000000 polars-0.9.9/local_dependencies/polars-lazy/src/physical_plan/expressions/is_null.rs
+-rw-r--r--   0     1001      121     5822 2021-09-19 07:10:07.000000 polars-0.9.9/local_dependencies/polars-lazy/src/physical_plan/expressions/literal.rs
+-rw-r--r--   0     1001      121    12535 2021-09-19 07:10:07.000000 polars-0.9.9/local_dependencies/polars-lazy/src/physical_plan/expressions/mod.rs
+-rw-r--r--   0     1001      121     1428 2021-09-19 07:10:07.000000 polars-0.9.9/local_dependencies/polars-lazy/src/physical_plan/expressions/not.rs
+-rw-r--r--   0     1001      121     2198 2021-09-19 07:10:07.000000 polars-0.9.9/local_dependencies/polars-lazy/src/physical_plan/expressions/shift.rs
+-rw-r--r--   0     1001      121     2000 2021-09-19 07:10:07.000000 polars-0.9.9/local_dependencies/polars-lazy/src/physical_plan/expressions/slice.rs
+-rw-r--r--   0     1001      121     2756 2021-09-19 07:10:07.000000 polars-0.9.9/local_dependencies/polars-lazy/src/physical_plan/expressions/sort.rs
+-rw-r--r--   0     1001      121     3986 2021-09-19 07:10:07.000000 polars-0.9.9/local_dependencies/polars-lazy/src/physical_plan/expressions/sortby.rs
+-rw-r--r--   0     1001      121     1599 2021-09-19 07:10:07.000000 polars-0.9.9/local_dependencies/polars-lazy/src/physical_plan/expressions/take.rs
+-rw-r--r--   0     1001      121     1797 2021-09-19 07:10:07.000000 polars-0.9.9/local_dependencies/polars-lazy/src/physical_plan/expressions/ternary.rs
+-rw-r--r--   0     1001      121      779 2021-09-19 07:10:07.000000 polars-0.9.9/local_dependencies/polars-lazy/src/physical_plan/expressions/utils.rs
+-rw-r--r--   0     1001      121     5219 2021-09-19 07:10:07.000000 polars-0.9.9/local_dependencies/polars-lazy/src/physical_plan/expressions/window.rs
+-rw-r--r--   0     1001      121     1131 2021-09-19 07:10:07.000000 polars-0.9.9/local_dependencies/polars-lazy/src/physical_plan/mod.rs
+-rw-r--r--   0     1001      121    42925 2021-09-19 07:10:07.000000 polars-0.9.9/local_dependencies/polars-lazy/src/physical_plan/planner.rs
+-rw-r--r--   0     1001      121     1969 2021-09-19 07:10:07.000000 polars-0.9.9/local_dependencies/polars-lazy/src/physical_plan/state.rs
+-rw-r--r--   0     1001      121     1730 2021-09-19 07:10:07.000000 polars-0.9.9/local_dependencies/polars-lazy/src/prelude.rs
+-rw-r--r--   0     1001      121    46889 2021-09-19 07:10:07.000000 polars-0.9.9/local_dependencies/polars-lazy/src/test.rs
+-rw-r--r--   0     1001      121    10120 2021-09-19 07:10:07.000000 polars-0.9.9/local_dependencies/polars-lazy/src/utils.rs
+-rw-r--r--   0        0        0      759 1970-01-01 00:00:00.000000 polars-0.9.9/local_dependencies/polars-arrow/Cargo.toml
+-rw-r--r--   0     1001      121      985 2021-09-19 07:10:07.000000 polars-0.9.9/local_dependencies/polars-arrow/src/array/default_arrays.rs
+-rw-r--r--   0     1001      121     5443 2021-09-19 07:10:07.000000 polars-0.9.9/local_dependencies/polars-arrow/src/array/mod.rs
+-rw-r--r--   0     1001      121     2294 2021-09-19 07:10:07.000000 polars-0.9.9/local_dependencies/polars-arrow/src/bit_util.rs
+-rw-r--r--   0     1001      121      395 2021-09-19 07:10:07.000000 polars-0.9.9/local_dependencies/polars-arrow/src/error.rs
+-rw-r--r--   0     1001      121      862 2021-09-19 07:10:07.000000 polars-0.9.9/local_dependencies/polars-arrow/src/is_valid.rs
+-rw-r--r--   0     1001      121     9506 2021-09-19 07:10:07.000000 polars-0.9.9/local_dependencies/polars-arrow/src/kernels/mod.rs
+-rw-r--r--   0     1001      121     4800 2021-09-19 07:10:07.000000 polars-0.9.9/local_dependencies/polars-arrow/src/kernels/set.rs
+-rw-r--r--   0     1001      121      151 2021-09-19 07:10:07.000000 polars-0.9.9/local_dependencies/polars-arrow/src/lib.rs
+-rw-r--r--   0     1001      121       66 2021-09-19 07:10:07.000000 polars-0.9.9/local_dependencies/polars-arrow/src/prelude.rs
+-rw-r--r--   0     1001      121      997 2021-09-19 07:10:07.000000 polars-0.9.9/local_dependencies/polars-arrow/src/trusted_len/boolean.rs
+-rw-r--r--   0     1001      121     4897 2021-09-19 07:10:07.000000 polars-0.9.9/local_dependencies/polars-arrow/src/trusted_len/mod.rs
+-rw-r--r--   0     1001      121     2594 2021-09-19 07:10:07.000000 polars-0.9.9/local_dependencies/polars-arrow/src/utils.rs
+-rw-r--r--   0        0        0     2836 1970-01-01 00:00:00.000000 polars-0.9.9/local_dependencies/polars-core/Cargo.toml
+-rw-r--r--   0     1001      121    15272 2021-09-19 07:10:07.000000 polars-0.9.9/local_dependencies/polars-core/src/chunked_array/arithmetic.rs
+-rw-r--r--   0     1001      121      323 2021-09-19 07:10:07.000000 polars-0.9.9/local_dependencies/polars-core/src/chunked_array/boolean.rs
+-rw-r--r--   0     1001      121     7160 2021-09-19 07:10:07.000000 polars-0.9.9/local_dependencies/polars-core/src/chunked_array/builder/categorical.rs
+-rw-r--r--   0     1001      121    20347 2021-09-19 07:10:07.000000 polars-0.9.9/local_dependencies/polars-core/src/chunked_array/builder/mod.rs
+-rw-r--r--   0     1001      121    11474 2021-09-19 07:10:07.000000 polars-0.9.9/local_dependencies/polars-core/src/chunked_array/cast.rs
+-rw-r--r--   0     1001      121     1712 2021-09-19 07:10:07.000000 polars-0.9.9/local_dependencies/polars-core/src/chunked_array/categorical/mod.rs
+-rw-r--r--   0     1001      121    32451 2021-09-19 07:10:07.000000 polars-0.9.9/local_dependencies/polars-core/src/chunked_array/comparison.rs
+-rw-r--r--   0     1001      121      611 2021-09-19 07:10:07.000000 polars-0.9.9/local_dependencies/polars-core/src/chunked_array/float.rs
+-rw-r--r--   0     1001      121    34608 2021-09-19 07:10:07.000000 polars-0.9.9/local_dependencies/polars-core/src/chunked_array/iterator/mod.rs
+-rw-r--r--   0     1001      121    16814 2021-09-19 07:10:07.000000 polars-0.9.9/local_dependencies/polars-core/src/chunked_array/iterator/par/boolean.rs
+-rw-r--r--   0     1001      121     1585 2021-09-19 07:10:07.000000 polars-0.9.9/local_dependencies/polars-core/src/chunked_array/iterator/par/list.rs
+-rw-r--r--   0     1001      121    32979 2021-09-19 07:10:07.000000 polars-0.9.9/local_dependencies/polars-core/src/chunked_array/iterator/par/macros.rs
+-rw-r--r--   0     1001      121     1935 2021-09-19 07:10:07.000000 polars-0.9.9/local_dependencies/polars-core/src/chunked_array/iterator/par/mod.rs
+-rw-r--r--   0     1001      121    40847 2021-09-19 07:10:07.000000 polars-0.9.9/local_dependencies/polars-core/src/chunked_array/iterator/par/numeric.rs
+-rw-r--r--   0     1001      121    16173 2021-09-19 07:10:07.000000 polars-0.9.9/local_dependencies/polars-core/src/chunked_array/iterator/par/utf8.rs
+-rw-r--r--   0     1001      121     2224 2021-09-19 07:10:07.000000 polars-0.9.9/local_dependencies/polars-core/src/chunked_array/kernels/mod.rs
+-rw-r--r--   0     1001      121      460 2021-09-19 07:10:07.000000 polars-0.9.9/local_dependencies/polars-core/src/chunked_array/kernels/strings.rs
+-rw-r--r--   0     1001      121    19790 2021-09-19 07:10:07.000000 polars-0.9.9/local_dependencies/polars-core/src/chunked_array/kernels/take.rs
+-rw-r--r--   0     1001      121     2409 2021-09-19 07:10:07.000000 polars-0.9.9/local_dependencies/polars-core/src/chunked_array/kernels/take_agg.rs
+-rw-r--r--   0     1001      121     2965 2021-09-19 07:10:07.000000 polars-0.9.9/local_dependencies/polars-core/src/chunked_array/kernels/temporal.rs
+-rw-r--r--   0     1001      121     5647 2021-09-19 07:10:07.000000 polars-0.9.9/local_dependencies/polars-core/src/chunked_array/list/iterator.rs
+-rw-r--r--   0     1001      121      327 2021-09-19 07:10:07.000000 polars-0.9.9/local_dependencies/polars-core/src/chunked_array/list/mod.rs
+-rw-r--r--   0     1001      121     3303 2021-09-19 07:10:07.000000 polars-0.9.9/local_dependencies/polars-core/src/chunked_array/list/namespace.rs
+-rw-r--r--   0     1001      121    35705 2021-09-19 07:10:07.000000 polars-0.9.9/local_dependencies/polars-core/src/chunked_array/mod.rs
+-rw-r--r--   0     1001      121     4026 2021-09-19 07:10:07.000000 polars-0.9.9/local_dependencies/polars-core/src/chunked_array/ndarray.rs
+-rw-r--r--   0     1001      121     3902 2021-09-19 07:10:07.000000 polars-0.9.9/local_dependencies/polars-core/src/chunked_array/object/builder.rs
+-rw-r--r--   0     1001      121      136 2021-09-19 07:10:07.000000 polars-0.9.9/local_dependencies/polars-core/src/chunked_array/object/is_valid.rs
+-rw-r--r--   0     1001      121     2683 2021-09-19 07:10:07.000000 polars-0.9.9/local_dependencies/polars-core/src/chunked_array/object/iterator.rs
+-rw-r--r--   0     1001      121     3848 2021-09-19 07:10:07.000000 polars-0.9.9/local_dependencies/polars-core/src/chunked_array/object/mod.rs
+-rw-r--r--   0     1001      121    18611 2021-09-19 07:10:07.000000 polars-0.9.9/local_dependencies/polars-core/src/chunked_array/ops/aggregate.rs
+-rw-r--r--   0     1001      121     2690 2021-09-19 07:10:07.000000 polars-0.9.9/local_dependencies/polars-core/src/chunked_array/ops/any_value.rs
+-rw-r--r--   0     1001      121    19701 2021-09-19 07:10:07.000000 polars-0.9.9/local_dependencies/polars-core/src/chunked_array/ops/apply.rs
+-rw-r--r--   0     1001      121     3328 2021-09-19 07:10:07.000000 polars-0.9.9/local_dependencies/polars-core/src/chunked_array/ops/bit_repr.rs
+-rw-r--r--   0     1001      121     4048 2021-09-19 07:10:07.000000 polars-0.9.9/local_dependencies/polars-core/src/chunked_array/ops/chunkops.rs
+-rw-r--r--   0     1001      121    10474 2021-09-19 07:10:07.000000 polars-0.9.9/local_dependencies/polars-core/src/chunked_array/ops/compare_inner.rs
+-rw-r--r--   0     1001      121     4349 2021-09-19 07:10:07.000000 polars-0.9.9/local_dependencies/polars-core/src/chunked_array/ops/cum_agg.rs
+-rw-r--r--   0     1001      121     4802 2021-09-19 07:10:07.000000 polars-0.9.9/local_dependencies/polars-core/src/chunked_array/ops/downcast.rs
+-rw-r--r--   0     1001      121    15154 2021-09-19 07:10:07.000000 polars-0.9.9/local_dependencies/polars-core/src/chunked_array/ops/explode.rs
+-rw-r--r--   0     1001      121    10183 2021-09-19 07:10:07.000000 polars-0.9.9/local_dependencies/polars-core/src/chunked_array/ops/fill_null.rs
+-rw-r--r--   0     1001      121     5535 2021-09-19 07:10:07.000000 polars-0.9.9/local_dependencies/polars-core/src/chunked_array/ops/filter.rs
+-rw-r--r--   0     1001      121     5977 2021-09-19 07:10:07.000000 polars-0.9.9/local_dependencies/polars-core/src/chunked_array/ops/interpolate.rs
+-rw-r--r--   0     1001      121     7556 2021-09-19 07:10:07.000000 polars-0.9.9/local_dependencies/polars-core/src/chunked_array/ops/is_in.rs
+-rw-r--r--   0     1001      121    33738 2021-09-19 07:10:07.000000 polars-0.9.9/local_dependencies/polars-core/src/chunked_array/ops/mod.rs
+-rw-r--r--   0     1001      121      995 2021-09-19 07:10:07.000000 polars-0.9.9/local_dependencies/polars-core/src/chunked_array/ops/peaks.rs
+-rw-r--r--   0     1001      121     2287 2021-09-19 07:10:07.000000 polars-0.9.9/local_dependencies/polars-core/src/chunked_array/ops/repeat_by.rs
+-rw-r--r--   0     1001      121    21542 2021-09-19 07:10:07.000000 polars-0.9.9/local_dependencies/polars-core/src/chunked_array/ops/rolling_window.rs
+-rw-r--r--   0     1001      121    12149 2021-09-19 07:10:07.000000 polars-0.9.9/local_dependencies/polars-core/src/chunked_array/ops/set.rs
+-rw-r--r--   0     1001      121     5802 2021-09-19 07:10:07.000000 polars-0.9.9/local_dependencies/polars-core/src/chunked_array/ops/shift.rs
+-rw-r--r--   0     1001      121    16679 2021-09-19 07:10:07.000000 polars-0.9.9/local_dependencies/polars-core/src/chunked_array/ops/sort.rs
+-rw-r--r--   0     1001      121    19985 2021-09-19 07:10:07.000000 polars-0.9.9/local_dependencies/polars-core/src/chunked_array/ops/take/mod.rs
+-rw-r--r--   0     1001      121     1931 2021-09-19 07:10:07.000000 polars-0.9.9/local_dependencies/polars-core/src/chunked_array/ops/take/take_every.rs
+-rw-r--r--   0     1001      121    13541 2021-09-19 07:10:07.000000 polars-0.9.9/local_dependencies/polars-core/src/chunked_array/ops/take/take_random.rs
+-rw-r--r--   0     1001      121     5081 2021-09-19 07:10:07.000000 polars-0.9.9/local_dependencies/polars-core/src/chunked_array/ops/take/take_single.rs
+-rw-r--r--   0     1001      121     4751 2021-09-19 07:10:07.000000 polars-0.9.9/local_dependencies/polars-core/src/chunked_array/ops/take/traits.rs
+-rw-r--r--   0     1001      121    19214 2021-09-19 07:10:07.000000 polars-0.9.9/local_dependencies/polars-core/src/chunked_array/ops/unique/mod.rs
+-rw-r--r--   0     1001      121     5200 2021-09-19 07:10:07.000000 polars-0.9.9/local_dependencies/polars-core/src/chunked_array/ops/unique/rank.rs
+-rw-r--r--   0     1001      121     7040 2021-09-19 07:10:07.000000 polars-0.9.9/local_dependencies/polars-core/src/chunked_array/ops/zip.rs
+-rw-r--r--   0     1001      121     6324 2021-09-19 07:10:07.000000 polars-0.9.9/local_dependencies/polars-core/src/chunked_array/random.rs
+-rw-r--r--   0     1001      121     1170 2021-09-19 07:10:07.000000 polars-0.9.9/local_dependencies/polars-core/src/chunked_array/strings/json_path.rs
+-rw-r--r--   0     1001      121     2333 2021-09-19 07:10:07.000000 polars-0.9.9/local_dependencies/polars-core/src/chunked_array/strings/mod.rs
+-rw-r--r--   0     1001      121    15928 2021-09-19 07:10:07.000000 polars-0.9.9/local_dependencies/polars-core/src/chunked_array/temporal/conversion.rs
+-rw-r--r--   0     1001      121     1852 2021-09-19 07:10:07.000000 polars-0.9.9/local_dependencies/polars-core/src/chunked_array/temporal/conversions_utils.rs
+-rw-r--r--   0     1001      121     1901 2021-09-19 07:10:07.000000 polars-0.9.9/local_dependencies/polars-core/src/chunked_array/temporal/mod.rs
+-rw-r--r--   0     1001      121     3469 2021-09-19 07:10:07.000000 polars-0.9.9/local_dependencies/polars-core/src/chunked_array/trusted_len.rs
+-rw-r--r--   0     1001      121    13354 2021-09-19 07:10:07.000000 polars-0.9.9/local_dependencies/polars-core/src/chunked_array/upstream_traits.rs
+-rw-r--r--   0     1001      121    21954 2021-09-19 07:10:07.000000 polars-0.9.9/local_dependencies/polars-core/src/datatypes.rs
+-rw-r--r--   0     1001      121      118 2021-09-19 07:10:07.000000 polars-0.9.9/local_dependencies/polars-core/src/doc/changelog/mod.rs
+-rw-r--r--   0     1001      121      898 2021-09-19 07:10:07.000000 polars-0.9.9/local_dependencies/polars-core/src/doc/changelog/v0_10_0_11.rs
+-rw-r--r--   0     1001      121      481 2021-09-19 07:10:07.000000 polars-0.9.9/local_dependencies/polars-core/src/doc/changelog/v0_3.rs
+-rw-r--r--   0     1001      121      293 2021-09-19 07:10:07.000000 polars-0.9.9/local_dependencies/polars-core/src/doc/changelog/v0_4.rs
+-rw-r--r--   0     1001      121      499 2021-09-19 07:10:07.000000 polars-0.9.9/local_dependencies/polars-core/src/doc/changelog/v0_5.rs
+-rw-r--r--   0     1001      121      288 2021-09-19 07:10:07.000000 polars-0.9.9/local_dependencies/polars-core/src/doc/changelog/v0_6.rs
+-rw-r--r--   0     1001      121     1072 2021-09-19 07:10:07.000000 polars-0.9.9/local_dependencies/polars-core/src/doc/changelog/v0_7.rs
+-rw-r--r--   0     1001      121      817 2021-09-19 07:10:07.000000 polars-0.9.9/local_dependencies/polars-core/src/doc/changelog/v0_8.rs
+-rw-r--r--   0     1001      121      596 2021-09-19 07:10:07.000000 polars-0.9.9/local_dependencies/polars-core/src/doc/changelog/v0_9.rs
+-rw-r--r--   0     1001      121       86 2021-09-19 07:10:07.000000 polars-0.9.9/local_dependencies/polars-core/src/doc/mod.rs
+-rw-r--r--   0     1001      121     3007 2021-09-19 07:10:07.000000 polars-0.9.9/local_dependencies/polars-core/src/doc/time.rs
+-rw-r--r--   0     1001      121     1654 2021-09-19 07:10:07.000000 polars-0.9.9/local_dependencies/polars-core/src/error.rs
+-rw-r--r--   0     1001      121       15 2021-09-19 07:10:07.000000 polars-0.9.9/local_dependencies/polars-core/src/export.rs
+-rw-r--r--   0     1001      121    23250 2021-09-19 07:10:07.000000 polars-0.9.9/local_dependencies/polars-core/src/fmt.rs
+-rw-r--r--   0     1001      121     2488 2021-09-19 07:10:07.000000 polars-0.9.9/local_dependencies/polars-core/src/frame/arithmetic.rs
+-rw-r--r--   0     1001      121     6719 2021-09-19 07:10:07.000000 polars-0.9.9/local_dependencies/polars-core/src/frame/asof_join.rs
+-rw-r--r--   0     1001      121     1890 2021-09-19 07:10:07.000000 polars-0.9.9/local_dependencies/polars-core/src/frame/cross_join.rs
+-rw-r--r--   0     1001      121     9800 2021-09-19 07:10:07.000000 polars-0.9.9/local_dependencies/polars-core/src/frame/explode.rs
+-rw-r--r--   0     1001      121    22890 2021-09-19 07:10:07.000000 polars-0.9.9/local_dependencies/polars-core/src/frame/groupby/aggregations.rs
+-rw-r--r--   0     1001      121    10541 2021-09-19 07:10:07.000000 polars-0.9.9/local_dependencies/polars-core/src/frame/groupby/hashing.rs
+-rw-r--r--   0     1001      121    52773 2021-09-19 07:10:07.000000 polars-0.9.9/local_dependencies/polars-core/src/frame/groupby/mod.rs
+-rw-r--r--   0     1001      121    21385 2021-09-19 07:10:07.000000 polars-0.9.9/local_dependencies/polars-core/src/frame/groupby/pivot.rs
+-rw-r--r--   0     1001      121    19949 2021-09-19 07:10:07.000000 polars-0.9.9/local_dependencies/polars-core/src/frame/groupby/resample.rs
+-rw-r--r--   0     1001      121    57841 2021-09-19 07:10:07.000000 polars-0.9.9/local_dependencies/polars-core/src/frame/hash_join/mod.rs
+-rw-r--r--   0     1001      121    13377 2021-09-19 07:10:07.000000 polars-0.9.9/local_dependencies/polars-core/src/frame/hash_join/multiple_keys.rs
+-rw-r--r--   0     1001      121    70052 2021-09-19 07:10:07.000000 polars-0.9.9/local_dependencies/polars-core/src/frame/mod.rs
+-rw-r--r--   0     1001      121    12482 2021-09-19 07:10:07.000000 polars-0.9.9/local_dependencies/polars-core/src/frame/row.rs
+-rw-r--r--   0     1001      121     2392 2021-09-19 07:10:07.000000 polars-0.9.9/local_dependencies/polars-core/src/frame/select.rs
+-rw-r--r--   0     1001      121     1381 2021-09-19 07:10:07.000000 polars-0.9.9/local_dependencies/polars-core/src/frame/upstream_traits.rs
+-rw-r--r--   0     1001      121     5096 2021-09-19 07:10:07.000000 polars-0.9.9/local_dependencies/polars-core/src/functions.rs
+-rw-r--r--   0     1001      121     3516 2021-09-19 07:10:07.000000 polars-0.9.9/local_dependencies/polars-core/src/lib.rs
+-rw-r--r--   0     1001      121     1729 2021-09-19 07:10:07.000000 polars-0.9.9/local_dependencies/polars-core/src/prelude.rs
+-rw-r--r--   0     1001      121     2574 2021-09-19 07:10:07.000000 polars-0.9.9/local_dependencies/polars-core/src/serde/chunked_array.rs
+-rw-r--r--   0     1001      121     3109 2021-09-19 07:10:07.000000 polars-0.9.9/local_dependencies/polars-core/src/serde/mod.rs
+-rw-r--r--   0     1001      121     7553 2021-09-19 07:10:07.000000 polars-0.9.9/local_dependencies/polars-core/src/serde/series.rs
+-rw-r--r--   0     1001      121    22184 2021-09-19 07:10:07.000000 polars-0.9.9/local_dependencies/polars-core/src/series/arithmetic.rs
+-rw-r--r--   0     1001      121     8321 2021-09-19 07:10:07.000000 polars-0.9.9/local_dependencies/polars-core/src/series/comparison.rs
+-rw-r--r--   0     1001      121    28200 2021-09-19 07:10:07.000000 polars-0.9.9/local_dependencies/polars-core/src/series/implementations/dates.rs
+-rw-r--r--   0     1001      121    33418 2021-09-19 07:10:07.000000 polars-0.9.9/local_dependencies/polars-core/src/series/implementations/mod.rs
+-rw-r--r--   0     1001      121     9311 2021-09-19 07:10:07.000000 polars-0.9.9/local_dependencies/polars-core/src/series/implementations/object.rs
+-rw-r--r--   0     1001      121     2198 2021-09-19 07:10:07.000000 polars-0.9.9/local_dependencies/polars-core/src/series/iterator.rs
+-rw-r--r--   0     1001      121    68176 2021-09-19 07:10:07.000000 polars-0.9.9/local_dependencies/polars-core/src/series/mod.rs
+-rw-r--r--   0     1001      121      473 2021-09-19 07:10:07.000000 polars-0.9.9/local_dependencies/polars-core/src/series/ops/diff.rs
+-rw-r--r--   0     1001      121      207 2021-09-19 07:10:07.000000 polars-0.9.9/local_dependencies/polars-core/src/series/ops/mod.rs
+-rw-r--r--   0     1001      121     5049 2021-09-19 07:10:07.000000 polars-0.9.9/local_dependencies/polars-core/src/series/ops/moment.rs
+-rw-r--r--   0     1001      121     1208 2021-09-19 07:10:07.000000 polars-0.9.9/local_dependencies/polars-core/src/series/ops/to_list.rs
+-rw-r--r--   0     1001      121     3561 2021-09-19 07:10:07.000000 polars-0.9.9/local_dependencies/polars-core/src/testing.rs
+-rw-r--r--   0     1001      121    27597 2021-09-19 07:10:07.000000 polars-0.9.9/local_dependencies/polars-core/src/utils.rs
+-rw-r--r--   0     1001      121    16835 2021-09-19 07:10:07.000000 polars-0.9.9/local_dependencies/polars-core/src/vector_hasher.rs
+-rw-r--r--   0        0        0     1628 1970-01-01 00:00:00.000000 polars-0.9.9/Cargo.toml
+-rw-r--r--   0     1001      121      169 2021-09-19 07:10:07.000000 polars-0.9.9/.flake8
+-rw-r--r--   0     1001      121       28 2021-09-19 07:10:07.000000 polars-0.9.9/.gitignore
+-rw-r--r--   0     1001      121    11235 2021-09-19 07:10:07.000000 polars-0.9.9/CHANGELOG.md
+-rw-r--r--   0     1001      121       71 2021-09-19 07:10:07.000000 polars-0.9.9/Makefile
+-rw-r--r--   0        0        0     7807 2021-09-19 07:10:08.000000 polars-0.9.9/README.md
+-rw-r--r--   0     1001      121      397 2021-09-19 07:10:07.000000 polars-0.9.9/build.requirements.txt
+-rw-r--r--   0     1001      121       36 2021-09-19 07:10:07.000000 polars-0.9.9/docs/.gitignore
+-rw-r--r--   0     1001      121      638 2021-09-19 07:10:07.000000 polars-0.9.9/docs/Makefile
+-rw-r--r--   0     1001      121      318 2021-09-19 07:10:07.000000 polars-0.9.9/docs/_templates/api_redirect.html
+-rw-r--r--   0     1001      121      151 2021-09-19 07:10:07.000000 polars-0.9.9/docs/_templates/autosummary/accessor.rst
+-rw-r--r--   0     1001      121      160 2021-09-19 07:10:07.000000 polars-0.9.9/docs/_templates/autosummary/accessor_attribute.rst
+-rw-r--r--   0     1001      121      168 2021-09-19 07:10:07.000000 polars-0.9.9/docs/_templates/autosummary/accessor_callable.rst
+-rw-r--r--   0     1001      121      157 2021-09-19 07:10:07.000000 polars-0.9.9/docs/_templates/autosummary/accessor_method.rst
+-rw-r--r--   0     1001      121      836 2021-09-19 07:10:07.000000 polars-0.9.9/docs/_templates/autosummary/class.rst
+-rw-r--r--   0     1001      121       94 2021-09-19 07:10:07.000000 polars-0.9.9/docs/_templates/autosummary/class_without_autosummary.rst
+-rw-r--r--   0     1001      121      406 2021-09-19 07:10:07.000000 polars-0.9.9/docs/_templates/sidebar-nav-bs.html
+-rw-r--r--   0     1001      121     3239 2021-09-19 07:10:07.000000 polars-0.9.9/docs/img/polars_logo.png
+-rw-r--r--   0     1001      121     2690 2021-09-19 07:10:07.000000 polars-0.9.9/docs/source/conf.py
+-rw-r--r--   0     1001      121       51 2021-09-19 07:10:07.000000 polars-0.9.9/docs/source/index.rst
+-rw-r--r--   0     1001      121      343 2021-09-19 07:10:07.000000 polars-0.9.9/docs/source/reference/config.rst
+-rw-r--r--   0     1001      121     3083 2021-09-19 07:10:07.000000 polars-0.9.9/docs/source/reference/dataframe.rst
+-rw-r--r--   0     1001      121     4262 2021-09-19 07:10:07.000000 polars-0.9.9/docs/source/reference/expression.rst
+-rw-r--r--   0     1001      121      417 2021-09-19 07:10:07.000000 polars-0.9.9/docs/source/reference/functions.rst
+-rw-r--r--   0     1001      121      307 2021-09-19 07:10:07.000000 polars-0.9.9/docs/source/reference/index.rst
+-rw-r--r--   0     1001      121      517 2021-09-19 07:10:07.000000 polars-0.9.9/docs/source/reference/io.rst
+-rw-r--r--   0     1001      121     1584 2021-09-19 07:10:07.000000 polars-0.9.9/docs/source/reference/lazyframe.rst
+-rw-r--r--   0     1001      121     4111 2021-09-19 07:10:07.000000 polars-0.9.9/docs/source/reference/series.rst
+-rw-r--r--   0     1001      121      205 2021-09-19 07:10:07.000000 polars-0.9.9/legacy/README.md
+-rwxr-xr-x   0     1001      121       86 2021-09-19 07:10:07.000000 polars-0.9.9/legacy/deploy.sh
+-rw-r--r--   0     1001      121      202 2021-09-19 07:10:07.000000 polars-0.9.9/legacy/pypolars/__init__.py
+-rw-r--r--   0     1001      121       31 2021-09-19 07:10:07.000000 polars-0.9.9/legacy/pypolars/datatypes.py
+-rw-r--r--   0     1001      121       27 2021-09-19 07:10:07.000000 polars-0.9.9/legacy/pypolars/frame.py
+-rw-r--r--   0     1001      121       31 2021-09-19 07:10:07.000000 polars-0.9.9/legacy/pypolars/functions.py
+-rw-r--r--   0     1001      121       26 2021-09-19 07:10:07.000000 polars-0.9.9/legacy/pypolars/lazy.py
+-rw-r--r--   0     1001      121       28 2021-09-19 07:10:07.000000 polars-0.9.9/legacy/pypolars/series.py
+-rw-r--r--   0     1001      121      554 2021-09-19 07:10:07.000000 polars-0.9.9/legacy/setup.py
+-rw-r--r--   0     1001      121     1011 2021-09-19 07:10:07.000000 polars-0.9.9/polars/__init__.py
+-rw-r--r--   0     1001      121     5440 2021-09-19 07:10:07.000000 polars-0.9.9/polars/_html.py
+-rw-r--r--   0     1001      121     1867 2021-09-19 07:10:07.000000 polars-0.9.9/polars/cfg.py
+-rw-r--r--   0     1001      121     9413 2021-09-19 07:10:07.000000 polars-0.9.9/polars/convert.py
+-rw-r--r--   0     1001      121     6475 2021-09-19 07:10:07.000000 polars-0.9.9/polars/datatypes.py
+-rw-r--r--   0     1001      121      128 2021-09-19 07:10:07.000000 polars-0.9.9/polars/eager/__init__.py
+-rw-r--r--   0     1001      121   119083 2021-09-19 07:10:07.000000 polars-0.9.9/polars/eager/frame.py
+-rw-r--r--   0     1001      121    87511 2021-09-19 07:10:07.000000 polars-0.9.9/polars/eager/series.py
+-rw-r--r--   0     1001      121     1810 2021-09-19 07:10:07.000000 polars-0.9.9/polars/functions.py
+-rw-r--r--   0     1001      121        0 2021-09-19 07:10:07.000000 polars-0.9.9/polars/internals/__init__.py
+-rw-r--r--   0     1001      121    11018 2021-09-19 07:10:07.000000 polars-0.9.9/polars/internals/construction.py
+-rw-r--r--   0     1001      121    19661 2021-09-19 07:10:07.000000 polars-0.9.9/polars/io.py
+-rw-r--r--   0     1001      121      231 2021-09-19 07:10:07.000000 polars-0.9.9/polars/lazy/__init__.py
+-rw-r--r--   0     1001      121    68958 2021-09-19 07:10:07.000000 polars-0.9.9/polars/lazy/expr.py
+-rw-r--r--   0     1001      121    32330 2021-09-19 07:10:07.000000 polars-0.9.9/polars/lazy/frame.py
+-rw-r--r--   0     1001      121    17383 2021-09-19 07:10:07.000000 polars-0.9.9/polars/lazy/functions.py
+-rw-r--r--   0     1001      121     3029 2021-09-19 07:10:07.000000 polars-0.9.9/polars/lazy/whenthen.py
+-rw-r--r--   0     1001      121        0 2021-09-19 07:10:07.000000 polars-0.9.9/polars/py.typed
+-rw-r--r--   0     1001      121     1094 2021-09-19 07:10:07.000000 polars-0.9.9/polars/string_cache.py
+-rw-r--r--   0     1001      121     2874 2021-09-19 07:10:07.000000 polars-0.9.9/polars/utils.py
+-rw-r--r--   0     1001      121      423 2021-09-19 07:10:07.000000 polars-0.9.9/pyproject.toml
+-rw-r--r--   0     1001      121        8 2021-09-19 07:10:07.000000 polars-0.9.9/rust-toolchain
+-rw-r--r--   0     1001      121     6385 2021-09-19 07:10:07.000000 polars-0.9.9/src/apply/dataframe.rs
+-rw-r--r--   0     1001      121     4250 2021-09-19 07:10:07.000000 polars-0.9.9/src/apply/mod.rs
+-rw-r--r--   0     1001      121    59591 2021-09-19 07:10:07.000000 polars-0.9.9/src/apply/series.rs
+-rw-r--r--   0     1001      121       32 2021-09-19 07:10:07.000000 polars-0.9.9/src/arrow_interop/mod.rs
+-rw-r--r--   0     1001      121     1625 2021-09-19 07:10:07.000000 polars-0.9.9/src/arrow_interop/to_py.rs
+-rw-r--r--   0     1001      121     2115 2021-09-19 07:10:07.000000 polars-0.9.9/src/arrow_interop/to_rust.rs
+-rw-r--r--   0     1001      121    13190 2021-09-19 07:10:07.000000 polars-0.9.9/src/conversion.rs
+-rw-r--r--   0     1001      121    30851 2021-09-19 07:10:07.000000 polars-0.9.9/src/dataframe.rs
+-rw-r--r--   0     1001      121     1919 2021-09-19 07:10:07.000000 polars-0.9.9/src/datatypes.rs
+-rw-r--r--   0     1001      121      501 2021-09-19 07:10:07.000000 polars-0.9.9/src/error.rs
+-rw-r--r--   0     1001      121     8541 2021-09-19 07:10:07.000000 polars-0.9.9/src/file.rs
+-rw-r--r--   0     1001      121    13767 2021-09-19 07:10:07.000000 polars-0.9.9/src/lazy/dataframe.rs
+-rw-r--r--   0     1001      121    35822 2021-09-19 07:10:07.000000 polars-0.9.9/src/lazy/dsl.rs
+-rw-r--r--   0     1001      121       47 2021-09-19 07:10:07.000000 polars-0.9.9/src/lazy/mod.rs
+-rw-r--r--   0     1001      121      211 2021-09-19 07:10:07.000000 polars-0.9.9/src/lazy/utils.rs
+-rw-r--r--   0     1001      121     5139 2021-09-19 07:10:07.000000 polars-0.9.9/src/lib.rs
+-rw-r--r--   0     1001      121     1547 2021-09-19 07:10:07.000000 polars-0.9.9/src/npy.rs
+-rw-r--r--   0     1001      121       87 2021-09-19 07:10:07.000000 polars-0.9.9/src/prelude.rs
+-rw-r--r--   0     1001      121    53916 2021-09-19 07:10:07.000000 polars-0.9.9/src/series.rs
+-rw-r--r--   0     1001      121     2542 2021-09-19 07:10:07.000000 polars-0.9.9/src/utils.rs
+-rwxr-xr-x   0     1001      121      869 2021-09-19 07:10:07.000000 polars-0.9.9/tasks.sh
+-rw-r--r--   0     1001      121      786 2021-09-19 07:10:07.000000 polars-0.9.9/tests/conftest.py
+-rw-r--r--   0     1001      121     2189 2021-09-19 07:10:07.000000 polars-0.9.9/tests/db-benchmark/groupby-datagen.R
+-rw-r--r--   0     1001      121     6860 2021-09-19 07:10:07.000000 polars-0.9.9/tests/db-benchmark/main.py
+-rw-r--r--   0     1001      121       49 2021-09-19 07:10:07.000000 polars-0.9.9/tests/files/gzipped.csv
+-rw-r--r--   0     1001      121    32156 2021-09-19 07:10:07.000000 polars-0.9.9/tests/test_df.py
+-rw-r--r--   0     1001      121     1488 2021-09-19 07:10:07.000000 polars-0.9.9/tests/test_interop.py
+-rw-r--r--   0     1001      121     5614 2021-09-19 07:10:07.000000 polars-0.9.9/tests/test_io.py
+-rw-r--r--   0     1001      121    15674 2021-09-19 07:10:07.000000 polars-0.9.9/tests/test_lazy.py
+-rw-r--r--   0     1001      121    16372 2021-09-19 07:10:07.000000 polars-0.9.9/tests/test_series.py
+-rw-r--r--   0        0        0     8182 1970-01-01 00:00:00.000000 polars-0.9.9/PKG-INFO
```

### Comparing `polars-0.9.8/local_dependencies/polars-arrow/Cargo.toml` & `polars-0.9.9/local_dependencies/polars-arrow/Cargo.toml`

 * *Files identical despite different names*

### Comparing `polars-0.9.8/local_dependencies/polars-arrow/src/array/default_arrays.rs` & `polars-0.9.9/local_dependencies/polars-arrow/src/array/default_arrays.rs`

 * *Files identical despite different names*

### Comparing `polars-0.9.8/local_dependencies/polars-arrow/src/array/mod.rs` & `polars-0.9.9/local_dependencies/polars-arrow/src/array/mod.rs`

 * *Files identical despite different names*

### Comparing `polars-0.9.8/local_dependencies/polars-arrow/src/bit_util.rs` & `polars-0.9.9/local_dependencies/polars-arrow/src/bit_util.rs`

 * *Files identical despite different names*

### Comparing `polars-0.9.8/local_dependencies/polars-arrow/src/is_valid.rs` & `polars-0.9.9/local_dependencies/polars-arrow/src/is_valid.rs`

 * *Files identical despite different names*

### Comparing `polars-0.9.8/local_dependencies/polars-arrow/src/kernels/mod.rs` & `polars-0.9.9/local_dependencies/polars-arrow/src/kernels/mod.rs`

 * *Files identical despite different names*

### Comparing `polars-0.9.8/local_dependencies/polars-arrow/src/kernels/set.rs` & `polars-0.9.9/local_dependencies/polars-arrow/src/kernels/set.rs`

 * *Files identical despite different names*

### Comparing `polars-0.9.8/local_dependencies/polars-arrow/src/trusted_len/boolean.rs` & `polars-0.9.9/local_dependencies/polars-arrow/src/trusted_len/boolean.rs`

 * *Files identical despite different names*

### Comparing `polars-0.9.8/local_dependencies/polars-arrow/src/trusted_len/mod.rs` & `polars-0.9.9/local_dependencies/polars-arrow/src/trusted_len/mod.rs`

 * *Files identical despite different names*

### Comparing `polars-0.9.8/local_dependencies/polars-arrow/src/utils.rs` & `polars-0.9.9/local_dependencies/polars-arrow/src/utils.rs`

 * *Files identical despite different names*

### Comparing `polars-0.9.8/local_dependencies/polars/Cargo.toml` & `polars-0.9.9/local_dependencies/polars/Cargo.toml`

 * *Files identical despite different names*

### Comparing `polars-0.9.8/local_dependencies/polars/Makefile` & `polars-0.9.9/local_dependencies/polars/Makefile`

 * *Files identical despite different names*

### Comparing `polars-0.9.8/local_dependencies/polars/benches/bench.rs` & `polars-0.9.9/local_dependencies/polars/benches/bench.rs`

 * *Files identical despite different names*

### Comparing `polars-0.9.8/local_dependencies/polars/benches/collect.rs` & `polars-0.9.9/local_dependencies/polars/benches/collect.rs`

 * *Files identical despite different names*

### Comparing `polars-0.9.8/local_dependencies/polars/benches/csv.rs` & `polars-0.9.9/local_dependencies/polars/benches/csv.rs`

 * *Files identical despite different names*

### Comparing `polars-0.9.8/local_dependencies/polars/benches/groupby.rs` & `polars-0.9.9/local_dependencies/polars/benches/groupby.rs`

 * *Files identical despite different names*

### Comparing `polars-0.9.8/local_dependencies/polars/benches/take.rs` & `polars-0.9.9/local_dependencies/polars/benches/take.rs`

 * *Files identical despite different names*

### Comparing `polars-0.9.8/local_dependencies/polars/src/docs/eager.rs` & `polars-0.9.9/local_dependencies/polars/src/docs/eager.rs`

 * *Files identical despite different names*

### Comparing `polars-0.9.8/local_dependencies/polars/src/docs/lazy.rs` & `polars-0.9.9/local_dependencies/polars/src/docs/lazy.rs`

 * *Files identical despite different names*

### Comparing `polars-0.9.8/local_dependencies/polars/src/docs/performance.rs` & `polars-0.9.9/local_dependencies/polars/src/docs/performance.rs`

 * *Files identical despite different names*

### Comparing `polars-0.9.8/local_dependencies/polars/src/lib.rs` & `polars-0.9.9/local_dependencies/polars/src/lib.rs`

 * *Files identical despite different names*

### Comparing `polars-0.9.8/local_dependencies/polars-io/Cargo.toml` & `polars-0.9.9/local_dependencies/polars-io/Cargo.toml`

 * *Files identical despite different names*

### Comparing `polars-0.9.8/local_dependencies/polars-io/src/csv.rs` & `polars-0.9.9/local_dependencies/polars-io/src/csv.rs`

 * *Files identical despite different names*

### Comparing `polars-0.9.8/local_dependencies/polars-io/src/csv_core/buffer.rs` & `polars-0.9.9/local_dependencies/polars-io/src/csv_core/buffer.rs`

 * *Files identical despite different names*

### Comparing `polars-0.9.8/local_dependencies/polars-io/src/csv_core/csv.rs` & `polars-0.9.9/local_dependencies/polars-io/src/csv_core/csv.rs`

 * *Files identical despite different names*

### Comparing `polars-0.9.8/local_dependencies/polars-io/src/csv_core/parser.rs` & `polars-0.9.9/local_dependencies/polars-io/src/csv_core/parser.rs`

 * *Files identical despite different names*

### Comparing `polars-0.9.8/local_dependencies/polars-io/src/csv_core/utils.rs` & `polars-0.9.9/local_dependencies/polars-io/src/csv_core/utils.rs`

 * *Files identical despite different names*

### Comparing `polars-0.9.8/local_dependencies/polars-io/src/ipc.rs` & `polars-0.9.9/local_dependencies/polars-io/src/ipc.rs`

 * *Files identical despite different names*

### Comparing `polars-0.9.8/local_dependencies/polars-io/src/json.rs` & `polars-0.9.9/local_dependencies/polars-io/src/json.rs`

 * *Files identical despite different names*

### Comparing `polars-0.9.8/local_dependencies/polars-io/src/lib.rs` & `polars-0.9.9/local_dependencies/polars-io/src/lib.rs`

 * *Files identical despite different names*

### Comparing `polars-0.9.8/local_dependencies/polars-io/src/mmap.rs` & `polars-0.9.9/local_dependencies/polars-io/src/mmap.rs`

 * *Files identical despite different names*

### Comparing `polars-0.9.8/local_dependencies/polars-io/src/parquet.rs` & `polars-0.9.9/local_dependencies/polars-io/src/parquet.rs`

 * *Files identical despite different names*

### Comparing `polars-0.9.8/local_dependencies/polars-io/src/prelude.rs` & `polars-0.9.9/local_dependencies/polars-io/src/prelude.rs`

 * *Files identical despite different names*

### Comparing `polars-0.9.8/local_dependencies/polars-io/src/utils.rs` & `polars-0.9.9/local_dependencies/polars-io/src/utils.rs`

 * *Files identical despite different names*

### Comparing `polars-0.9.8/local_dependencies/polars-lazy/Cargo.toml` & `polars-0.9.9/local_dependencies/polars-lazy/Cargo.toml`

 * *Files identical despite different names*

### Comparing `polars-0.9.8/local_dependencies/polars-lazy/src/datafusion/conversion.rs` & `polars-0.9.9/local_dependencies/polars-lazy/src/datafusion/conversion.rs`

 * *Files identical despite different names*

### Comparing `polars-0.9.8/local_dependencies/polars-lazy/src/datafusion/mod.rs` & `polars-0.9.9/local_dependencies/polars-lazy/src/datafusion/mod.rs`

 * *Files identical despite different names*

### Comparing `polars-0.9.8/local_dependencies/polars-lazy/src/dsl.rs` & `polars-0.9.9/local_dependencies/polars-lazy/src/dsl.rs`

 * *Files 3% similar despite different names*

```diff
@@ -1479,14 +1479,60 @@
         let weight = weight.map(|v| v.to_vec());
         self.apply(
             move |s| s.rolling_sum(window_size, weight.as_deref(), ignore_null, min_periods),
             GetOutput::same_type(),
         )
     }
 
+    /// Apply a rolling variance
+    #[cfg_attr(docsrs, doc(cfg(feature = "rolling_window")))]
+    #[cfg(feature = "rolling_window")]
+    pub fn rolling_var(self, window_size: usize) -> Expr {
+        self.apply(
+            move |s| match s.dtype() {
+                DataType::Float32 => Ok(s.f32().unwrap().rolling_var(window_size).into_series()),
+                DataType::Float64 => Ok(s.f64().unwrap().rolling_var(window_size).into_series()),
+                _ => Ok(s
+                    .cast_with_dtype(&DataType::Float64)?
+                    .f64()
+                    .unwrap()
+                    .rolling_var(window_size)
+                    .into_series()),
+            },
+            GetOutput::map_field(|field| match field.data_type() {
+                DataType::Float64 => field.clone(),
+                DataType::Float32 => Field::new(field.name(), DataType::Float32),
+                _ => Field::new(field.name(), DataType::Float64),
+            }),
+        )
+    }
+
+    /// Apply a rolling std-dev
+    #[cfg_attr(docsrs, doc(cfg(feature = "rolling_window")))]
+    #[cfg(feature = "rolling_window")]
+    pub fn rolling_std(self, window_size: usize) -> Expr {
+        self.apply(
+            move |s| match s.dtype() {
+                DataType::Float32 => Ok(s.f32().unwrap().rolling_std(window_size).into_series()),
+                DataType::Float64 => Ok(s.f64().unwrap().rolling_std(window_size).into_series()),
+                _ => Ok(s
+                    .cast_with_dtype(&DataType::Float64)?
+                    .f64()
+                    .unwrap()
+                    .rolling_std(window_size)
+                    .into_series()),
+            },
+            GetOutput::map_field(|field| match field.data_type() {
+                DataType::Float64 => field.clone(),
+                DataType::Float32 => Field::new(field.name(), DataType::Float32),
+                _ => Field::new(field.name(), DataType::Float64),
+            }),
+        )
+    }
+
     #[cfg_attr(docsrs, doc(cfg(feature = "rolling_window")))]
     #[cfg(feature = "rolling_window")]
     /// Apply a custom function over a rolling/ moving window of the array.
     /// This has quite some dynamic dispatch, so prefer rolling_min, max, mean, sum over this.
     pub fn rolling_apply(
         self,
         window_size: usize,
```

### Comparing `polars-0.9.8/local_dependencies/polars-lazy/src/dummies.rs` & `polars-0.9.9/local_dependencies/polars-lazy/src/dummies.rs`

 * *Files identical despite different names*

### Comparing `polars-0.9.8/local_dependencies/polars-lazy/src/frame.rs` & `polars-0.9.9/local_dependencies/polars-lazy/src/frame.rs`

 * *Files identical despite different names*

### Comparing `polars-0.9.8/local_dependencies/polars-lazy/src/functions.rs` & `polars-0.9.9/local_dependencies/polars-lazy/src/functions.rs`

 * *Files identical despite different names*

### Comparing `polars-0.9.8/local_dependencies/polars-lazy/src/lib.rs` & `polars-0.9.9/local_dependencies/polars-lazy/src/lib.rs`

 * *Files identical despite different names*

### Comparing `polars-0.9.8/local_dependencies/polars-lazy/src/logical_plan/aexpr.rs` & `polars-0.9.9/local_dependencies/polars-lazy/src/logical_plan/aexpr.rs`

 * *Files identical despite different names*

### Comparing `polars-0.9.8/local_dependencies/polars-lazy/src/logical_plan/alp.rs` & `polars-0.9.9/local_dependencies/polars-lazy/src/logical_plan/alp.rs`

 * *Files identical despite different names*

### Comparing `polars-0.9.8/local_dependencies/polars-lazy/src/logical_plan/conversion.rs` & `polars-0.9.9/local_dependencies/polars-lazy/src/logical_plan/conversion.rs`

 * *Files identical despite different names*

### Comparing `polars-0.9.8/local_dependencies/polars-lazy/src/logical_plan/iterator.rs` & `polars-0.9.9/local_dependencies/polars-lazy/src/logical_plan/iterator.rs`

 * *Files identical despite different names*

### Comparing `polars-0.9.8/local_dependencies/polars-lazy/src/logical_plan/mod.rs` & `polars-0.9.9/local_dependencies/polars-lazy/src/logical_plan/mod.rs`

 * *Files identical despite different names*

### Comparing `polars-0.9.8/local_dependencies/polars-lazy/src/logical_plan/optimizer/aggregate_pushdown.rs` & `polars-0.9.9/local_dependencies/polars-lazy/src/logical_plan/optimizer/aggregate_pushdown.rs`

 * *Files identical despite different names*

### Comparing `polars-0.9.8/local_dependencies/polars-lazy/src/logical_plan/optimizer/aggregate_scan_projections.rs` & `polars-0.9.9/local_dependencies/polars-lazy/src/logical_plan/optimizer/aggregate_scan_projections.rs`

 * *Files identical despite different names*

### Comparing `polars-0.9.8/local_dependencies/polars-lazy/src/logical_plan/optimizer/drop_nulls.rs` & `polars-0.9.9/local_dependencies/polars-lazy/src/logical_plan/optimizer/drop_nulls.rs`

 * *Files identical despite different names*

### Comparing `polars-0.9.8/local_dependencies/polars-lazy/src/logical_plan/optimizer/fast_projection.rs` & `polars-0.9.9/local_dependencies/polars-lazy/src/logical_plan/optimizer/fast_projection.rs`

 * *Files identical despite different names*

### Comparing `polars-0.9.8/local_dependencies/polars-lazy/src/logical_plan/optimizer/join_pruning.rs` & `polars-0.9.9/local_dependencies/polars-lazy/src/logical_plan/optimizer/join_pruning.rs`

 * *Files identical despite different names*

### Comparing `polars-0.9.8/local_dependencies/polars-lazy/src/logical_plan/optimizer/mod.rs` & `polars-0.9.9/local_dependencies/polars-lazy/src/logical_plan/optimizer/mod.rs`

 * *Files identical despite different names*

### Comparing `polars-0.9.8/local_dependencies/polars-lazy/src/logical_plan/optimizer/predicate_pushdown/mod.rs` & `polars-0.9.9/local_dependencies/polars-lazy/src/logical_plan/optimizer/predicate_pushdown/mod.rs`

 * *Files identical despite different names*

### Comparing `polars-0.9.8/local_dependencies/polars-lazy/src/logical_plan/optimizer/predicate_pushdown/utils.rs` & `polars-0.9.9/local_dependencies/polars-lazy/src/logical_plan/optimizer/predicate_pushdown/utils.rs`

 * *Files identical despite different names*

### Comparing `polars-0.9.8/local_dependencies/polars-lazy/src/logical_plan/optimizer/projection_pushdown.rs` & `polars-0.9.9/local_dependencies/polars-lazy/src/logical_plan/optimizer/projection_pushdown.rs`

 * *Files identical despite different names*

### Comparing `polars-0.9.8/local_dependencies/polars-lazy/src/logical_plan/optimizer/simplify_expr.rs` & `polars-0.9.9/local_dependencies/polars-lazy/src/logical_plan/optimizer/simplify_expr.rs`

 * *Files identical despite different names*

### Comparing `polars-0.9.8/local_dependencies/polars-lazy/src/logical_plan/optimizer/stack_opt.rs` & `polars-0.9.9/local_dependencies/polars-lazy/src/logical_plan/optimizer/stack_opt.rs`

 * *Files identical despite different names*

### Comparing `polars-0.9.8/local_dependencies/polars-lazy/src/logical_plan/optimizer/type_coercion.rs` & `polars-0.9.9/local_dependencies/polars-lazy/src/logical_plan/optimizer/type_coercion.rs`

 * *Files identical despite different names*

### Comparing `polars-0.9.8/local_dependencies/polars-lazy/src/physical_plan/executors/cache.rs` & `polars-0.9.9/local_dependencies/polars-lazy/src/physical_plan/executors/cache.rs`

 * *Files identical despite different names*

### Comparing `polars-0.9.8/local_dependencies/polars-lazy/src/physical_plan/executors/drop_duplicates.rs` & `polars-0.9.9/local_dependencies/polars-lazy/src/physical_plan/executors/drop_duplicates.rs`

 * *Files identical despite different names*

### Comparing `polars-0.9.8/local_dependencies/polars-lazy/src/physical_plan/executors/filter.rs` & `polars-0.9.9/local_dependencies/polars-lazy/src/physical_plan/executors/filter.rs`

 * *Files identical despite different names*

### Comparing `polars-0.9.8/local_dependencies/polars-lazy/src/physical_plan/executors/groupby.rs` & `polars-0.9.9/local_dependencies/polars-lazy/src/physical_plan/executors/groupby.rs`

 * *Files identical despite different names*

### Comparing `polars-0.9.8/local_dependencies/polars-lazy/src/physical_plan/executors/join.rs` & `polars-0.9.9/local_dependencies/polars-lazy/src/physical_plan/executors/join.rs`

 * *Files identical despite different names*

### Comparing `polars-0.9.8/local_dependencies/polars-lazy/src/physical_plan/executors/mod.rs` & `polars-0.9.9/local_dependencies/polars-lazy/src/physical_plan/executors/mod.rs`

 * *Files identical despite different names*

### Comparing `polars-0.9.8/local_dependencies/polars-lazy/src/physical_plan/executors/projection.rs` & `polars-0.9.9/local_dependencies/polars-lazy/src/physical_plan/executors/projection.rs`

 * *Files identical despite different names*

### Comparing `polars-0.9.8/local_dependencies/polars-lazy/src/physical_plan/executors/scan.rs` & `polars-0.9.9/local_dependencies/polars-lazy/src/physical_plan/executors/scan.rs`

 * *Files identical despite different names*

### Comparing `polars-0.9.8/local_dependencies/polars-lazy/src/physical_plan/executors/sort.rs` & `polars-0.9.9/local_dependencies/polars-lazy/src/physical_plan/executors/sort.rs`

 * *Files identical despite different names*

### Comparing `polars-0.9.8/local_dependencies/polars-lazy/src/physical_plan/executors/stack.rs` & `polars-0.9.9/local_dependencies/polars-lazy/src/physical_plan/executors/stack.rs`

 * *Files identical despite different names*

### Comparing `polars-0.9.8/local_dependencies/polars-lazy/src/physical_plan/expressions/aggregation.rs` & `polars-0.9.9/local_dependencies/polars-lazy/src/physical_plan/expressions/aggregation.rs`

 * *Files identical despite different names*

### Comparing `polars-0.9.8/local_dependencies/polars-lazy/src/physical_plan/expressions/alias.rs` & `polars-0.9.9/local_dependencies/polars-lazy/src/physical_plan/expressions/alias.rs`

 * *Files identical despite different names*

### Comparing `polars-0.9.8/local_dependencies/polars-lazy/src/physical_plan/expressions/apply.rs` & `polars-0.9.9/local_dependencies/polars-lazy/src/physical_plan/expressions/apply.rs`

 * *Files identical despite different names*

### Comparing `polars-0.9.8/local_dependencies/polars-lazy/src/physical_plan/expressions/binary.rs` & `polars-0.9.9/local_dependencies/polars-lazy/src/physical_plan/expressions/binary.rs`

 * *Files identical despite different names*

### Comparing `polars-0.9.8/local_dependencies/polars-lazy/src/physical_plan/expressions/binary_function.rs` & `polars-0.9.9/local_dependencies/polars-lazy/src/physical_plan/expressions/binary_function.rs`

 * *Files identical despite different names*

### Comparing `polars-0.9.8/local_dependencies/polars-lazy/src/physical_plan/expressions/cast.rs` & `polars-0.9.9/local_dependencies/polars-lazy/src/physical_plan/expressions/cast.rs`

 * *Files identical despite different names*

### Comparing `polars-0.9.8/local_dependencies/polars-lazy/src/physical_plan/expressions/column.rs` & `polars-0.9.9/local_dependencies/polars-lazy/src/physical_plan/expressions/column.rs`

 * *Files identical despite different names*

### Comparing `polars-0.9.8/local_dependencies/polars-lazy/src/physical_plan/expressions/filter.rs` & `polars-0.9.9/local_dependencies/polars-lazy/src/physical_plan/expressions/filter.rs`

 * *Files identical despite different names*

### Comparing `polars-0.9.8/local_dependencies/polars-lazy/src/physical_plan/expressions/is_not_null.rs` & `polars-0.9.9/local_dependencies/polars-lazy/src/physical_plan/expressions/is_not_null.rs`

 * *Files identical despite different names*

### Comparing `polars-0.9.8/local_dependencies/polars-lazy/src/physical_plan/expressions/is_null.rs` & `polars-0.9.9/local_dependencies/polars-lazy/src/physical_plan/expressions/is_null.rs`

 * *Files identical despite different names*

### Comparing `polars-0.9.8/local_dependencies/polars-lazy/src/physical_plan/expressions/literal.rs` & `polars-0.9.9/local_dependencies/polars-lazy/src/physical_plan/expressions/literal.rs`

 * *Files identical despite different names*

### Comparing `polars-0.9.8/local_dependencies/polars-lazy/src/physical_plan/expressions/mod.rs` & `polars-0.9.9/local_dependencies/polars-lazy/src/physical_plan/expressions/mod.rs`

 * *Files identical despite different names*

### Comparing `polars-0.9.8/local_dependencies/polars-lazy/src/physical_plan/expressions/not.rs` & `polars-0.9.9/local_dependencies/polars-lazy/src/physical_plan/expressions/not.rs`

 * *Files identical despite different names*

### Comparing `polars-0.9.8/local_dependencies/polars-lazy/src/physical_plan/expressions/shift.rs` & `polars-0.9.9/local_dependencies/polars-lazy/src/physical_plan/expressions/shift.rs`

 * *Files identical despite different names*

### Comparing `polars-0.9.8/local_dependencies/polars-lazy/src/physical_plan/expressions/slice.rs` & `polars-0.9.9/local_dependencies/polars-lazy/src/physical_plan/expressions/slice.rs`

 * *Files identical despite different names*

### Comparing `polars-0.9.8/local_dependencies/polars-lazy/src/physical_plan/expressions/sort.rs` & `polars-0.9.9/local_dependencies/polars-lazy/src/physical_plan/expressions/sort.rs`

 * *Files identical despite different names*

### Comparing `polars-0.9.8/local_dependencies/polars-lazy/src/physical_plan/expressions/sortby.rs` & `polars-0.9.9/local_dependencies/polars-lazy/src/physical_plan/expressions/sortby.rs`

 * *Files identical despite different names*

### Comparing `polars-0.9.8/local_dependencies/polars-lazy/src/physical_plan/expressions/take.rs` & `polars-0.9.9/local_dependencies/polars-lazy/src/physical_plan/expressions/take.rs`

 * *Files identical despite different names*

### Comparing `polars-0.9.8/local_dependencies/polars-lazy/src/physical_plan/expressions/ternary.rs` & `polars-0.9.9/local_dependencies/polars-lazy/src/physical_plan/expressions/ternary.rs`

 * *Files identical despite different names*

### Comparing `polars-0.9.8/local_dependencies/polars-lazy/src/physical_plan/expressions/utils.rs` & `polars-0.9.9/local_dependencies/polars-lazy/src/physical_plan/expressions/utils.rs`

 * *Files identical despite different names*

### Comparing `polars-0.9.8/local_dependencies/polars-lazy/src/physical_plan/expressions/window.rs` & `polars-0.9.9/local_dependencies/polars-lazy/src/physical_plan/expressions/window.rs`

 * *Files identical despite different names*

### Comparing `polars-0.9.8/local_dependencies/polars-lazy/src/physical_plan/mod.rs` & `polars-0.9.9/local_dependencies/polars-lazy/src/physical_plan/mod.rs`

 * *Files identical despite different names*

### Comparing `polars-0.9.8/local_dependencies/polars-lazy/src/physical_plan/planner.rs` & `polars-0.9.9/local_dependencies/polars-lazy/src/physical_plan/planner.rs`

 * *Files identical despite different names*

### Comparing `polars-0.9.8/local_dependencies/polars-lazy/src/physical_plan/state.rs` & `polars-0.9.9/local_dependencies/polars-lazy/src/physical_plan/state.rs`

 * *Files identical despite different names*

### Comparing `polars-0.9.8/local_dependencies/polars-lazy/src/prelude.rs` & `polars-0.9.9/local_dependencies/polars-lazy/src/prelude.rs`

 * *Files identical despite different names*

### Comparing `polars-0.9.8/local_dependencies/polars-lazy/src/test.rs` & `polars-0.9.9/local_dependencies/polars-lazy/src/test.rs`

 * *Files identical despite different names*

### Comparing `polars-0.9.8/local_dependencies/polars-lazy/src/utils.rs` & `polars-0.9.9/local_dependencies/polars-lazy/src/utils.rs`

 * *Files identical despite different names*

### Comparing `polars-0.9.8/local_dependencies/polars-core/Cargo.toml` & `polars-0.9.9/local_dependencies/polars-core/Cargo.toml`

 * *Files identical despite different names*

### Comparing `polars-0.9.8/local_dependencies/polars-core/src/chunked_array/arithmetic.rs` & `polars-0.9.9/local_dependencies/polars-core/src/chunked_array/arithmetic.rs`

 * *Files identical despite different names*

### Comparing `polars-0.9.8/local_dependencies/polars-core/src/chunked_array/builder/categorical.rs` & `polars-0.9.9/local_dependencies/polars-core/src/chunked_array/builder/categorical.rs`

 * *Files identical despite different names*

### Comparing `polars-0.9.8/local_dependencies/polars-core/src/chunked_array/builder/mod.rs` & `polars-0.9.9/local_dependencies/polars-core/src/chunked_array/builder/mod.rs`

 * *Files identical despite different names*

### Comparing `polars-0.9.8/local_dependencies/polars-core/src/chunked_array/cast.rs` & `polars-0.9.9/local_dependencies/polars-core/src/chunked_array/cast.rs`

 * *Files identical despite different names*

### Comparing `polars-0.9.8/local_dependencies/polars-core/src/chunked_array/categorical/mod.rs` & `polars-0.9.9/local_dependencies/polars-core/src/chunked_array/categorical/mod.rs`

 * *Files identical despite different names*

### Comparing `polars-0.9.8/local_dependencies/polars-core/src/chunked_array/comparison.rs` & `polars-0.9.9/local_dependencies/polars-core/src/chunked_array/comparison.rs`

 * *Files identical despite different names*

### Comparing `polars-0.9.8/local_dependencies/polars-core/src/chunked_array/float.rs` & `polars-0.9.9/local_dependencies/polars-core/src/chunked_array/float.rs`

 * *Files identical despite different names*

### Comparing `polars-0.9.8/local_dependencies/polars-core/src/chunked_array/iterator/mod.rs` & `polars-0.9.9/local_dependencies/polars-core/src/chunked_array/iterator/mod.rs`

 * *Files identical despite different names*

### Comparing `polars-0.9.8/local_dependencies/polars-core/src/chunked_array/iterator/par/boolean.rs` & `polars-0.9.9/local_dependencies/polars-core/src/chunked_array/iterator/par/boolean.rs`

 * *Files identical despite different names*

### Comparing `polars-0.9.8/local_dependencies/polars-core/src/chunked_array/iterator/par/list.rs` & `polars-0.9.9/local_dependencies/polars-core/src/chunked_array/iterator/par/list.rs`

 * *Files identical despite different names*

### Comparing `polars-0.9.8/local_dependencies/polars-core/src/chunked_array/iterator/par/macros.rs` & `polars-0.9.9/local_dependencies/polars-core/src/chunked_array/iterator/par/macros.rs`

 * *Files identical despite different names*

### Comparing `polars-0.9.8/local_dependencies/polars-core/src/chunked_array/iterator/par/mod.rs` & `polars-0.9.9/local_dependencies/polars-core/src/chunked_array/iterator/par/mod.rs`

 * *Files identical despite different names*

### Comparing `polars-0.9.8/local_dependencies/polars-core/src/chunked_array/iterator/par/numeric.rs` & `polars-0.9.9/local_dependencies/polars-core/src/chunked_array/iterator/par/numeric.rs`

 * *Files identical despite different names*

### Comparing `polars-0.9.8/local_dependencies/polars-core/src/chunked_array/iterator/par/utf8.rs` & `polars-0.9.9/local_dependencies/polars-core/src/chunked_array/iterator/par/utf8.rs`

 * *Files identical despite different names*

### Comparing `polars-0.9.8/local_dependencies/polars-core/src/chunked_array/kernels/mod.rs` & `polars-0.9.9/local_dependencies/polars-core/src/chunked_array/kernels/mod.rs`

 * *Files identical despite different names*

### Comparing `polars-0.9.8/local_dependencies/polars-core/src/chunked_array/kernels/take.rs` & `polars-0.9.9/local_dependencies/polars-core/src/chunked_array/kernels/take.rs`

 * *Files identical despite different names*

### Comparing `polars-0.9.8/local_dependencies/polars-core/src/chunked_array/kernels/take_agg.rs` & `polars-0.9.9/local_dependencies/polars-core/src/chunked_array/kernels/take_agg.rs`

 * *Files identical despite different names*

### Comparing `polars-0.9.8/local_dependencies/polars-core/src/chunked_array/kernels/temporal.rs` & `polars-0.9.9/local_dependencies/polars-core/src/chunked_array/kernels/temporal.rs`

 * *Files identical despite different names*

### Comparing `polars-0.9.8/local_dependencies/polars-core/src/chunked_array/list/iterator.rs` & `polars-0.9.9/local_dependencies/polars-core/src/chunked_array/list/iterator.rs`

 * *Files identical despite different names*

### Comparing `polars-0.9.8/local_dependencies/polars-core/src/chunked_array/list/namespace.rs` & `polars-0.9.9/local_dependencies/polars-core/src/chunked_array/list/namespace.rs`

 * *Files identical despite different names*

### Comparing `polars-0.9.8/local_dependencies/polars-core/src/chunked_array/mod.rs` & `polars-0.9.9/local_dependencies/polars-core/src/chunked_array/mod.rs`

 * *Files identical despite different names*

### Comparing `polars-0.9.8/local_dependencies/polars-core/src/chunked_array/ndarray.rs` & `polars-0.9.9/local_dependencies/polars-core/src/chunked_array/ndarray.rs`

 * *Files identical despite different names*

### Comparing `polars-0.9.8/local_dependencies/polars-core/src/chunked_array/object/builder.rs` & `polars-0.9.9/local_dependencies/polars-core/src/chunked_array/object/builder.rs`

 * *Files identical despite different names*

### Comparing `polars-0.9.8/local_dependencies/polars-core/src/chunked_array/object/iterator.rs` & `polars-0.9.9/local_dependencies/polars-core/src/chunked_array/object/iterator.rs`

 * *Files identical despite different names*

### Comparing `polars-0.9.8/local_dependencies/polars-core/src/chunked_array/object/mod.rs` & `polars-0.9.9/local_dependencies/polars-core/src/chunked_array/object/mod.rs`

 * *Files identical despite different names*

### Comparing `polars-0.9.8/local_dependencies/polars-core/src/chunked_array/ops/aggregate.rs` & `polars-0.9.9/local_dependencies/polars-core/src/chunked_array/ops/aggregate.rs`

 * *Files identical despite different names*

### Comparing `polars-0.9.8/local_dependencies/polars-core/src/chunked_array/ops/any_value.rs` & `polars-0.9.9/local_dependencies/polars-core/src/chunked_array/ops/any_value.rs`

 * *Files identical despite different names*

### Comparing `polars-0.9.8/local_dependencies/polars-core/src/chunked_array/ops/apply.rs` & `polars-0.9.9/local_dependencies/polars-core/src/chunked_array/ops/apply.rs`

 * *Files identical despite different names*

### Comparing `polars-0.9.8/local_dependencies/polars-core/src/chunked_array/ops/bit_repr.rs` & `polars-0.9.9/local_dependencies/polars-core/src/chunked_array/ops/bit_repr.rs`

 * *Files identical despite different names*

### Comparing `polars-0.9.8/local_dependencies/polars-core/src/chunked_array/ops/chunkops.rs` & `polars-0.9.9/local_dependencies/polars-core/src/chunked_array/ops/chunkops.rs`

 * *Files identical despite different names*

### Comparing `polars-0.9.8/local_dependencies/polars-core/src/chunked_array/ops/compare_inner.rs` & `polars-0.9.9/local_dependencies/polars-core/src/chunked_array/ops/compare_inner.rs`

 * *Files identical despite different names*

### Comparing `polars-0.9.8/local_dependencies/polars-core/src/chunked_array/ops/cum_agg.rs` & `polars-0.9.9/local_dependencies/polars-core/src/chunked_array/ops/cum_agg.rs`

 * *Files identical despite different names*

### Comparing `polars-0.9.8/local_dependencies/polars-core/src/chunked_array/ops/downcast.rs` & `polars-0.9.9/local_dependencies/polars-core/src/chunked_array/ops/downcast.rs`

 * *Files identical despite different names*

### Comparing `polars-0.9.8/local_dependencies/polars-core/src/chunked_array/ops/explode.rs` & `polars-0.9.9/local_dependencies/polars-core/src/chunked_array/ops/explode.rs`

 * *Files 1% similar despite different names*

```diff
@@ -236,17 +236,18 @@
                     last = o;
                 }
                 if !has_empty {
                     panic!()
                 }
             }
 
-            let values = Series::try_from(("", values)).unwrap();
+            let values = Series::try_from((self.name(), values)).unwrap();
             values.explode_by_offsets(offsets)
         };
+        debug_assert_eq!(s.name(), self.name());
         Ok((s, offsets_buf))
     }
 }
 
 impl ChunkExplode for Utf8Chunked {
     fn explode_and_offsets(&self) -> Result<(Series, Buffer<i64>)> {
         // A list array's memory layout is actually already 'exploded', so we can just take the values array
```

### Comparing `polars-0.9.8/local_dependencies/polars-core/src/chunked_array/ops/fill_null.rs` & `polars-0.9.9/local_dependencies/polars-core/src/chunked_array/ops/fill_null.rs`

 * *Files identical despite different names*

### Comparing `polars-0.9.8/local_dependencies/polars-core/src/chunked_array/ops/filter.rs` & `polars-0.9.9/local_dependencies/polars-core/src/chunked_array/ops/filter.rs`

 * *Files identical despite different names*

### Comparing `polars-0.9.8/local_dependencies/polars-core/src/chunked_array/ops/interpolate.rs` & `polars-0.9.9/local_dependencies/polars-core/src/chunked_array/ops/interpolate.rs`

 * *Files identical despite different names*

### Comparing `polars-0.9.8/local_dependencies/polars-core/src/chunked_array/ops/is_in.rs` & `polars-0.9.9/local_dependencies/polars-core/src/chunked_array/ops/is_in.rs`

 * *Files identical despite different names*

### Comparing `polars-0.9.8/local_dependencies/polars-core/src/chunked_array/ops/mod.rs` & `polars-0.9.9/local_dependencies/polars-core/src/chunked_array/ops/mod.rs`

 * *Files identical despite different names*

### Comparing `polars-0.9.8/local_dependencies/polars-core/src/chunked_array/ops/peaks.rs` & `polars-0.9.9/local_dependencies/polars-core/src/chunked_array/ops/peaks.rs`

 * *Files identical despite different names*

### Comparing `polars-0.9.8/local_dependencies/polars-core/src/chunked_array/ops/repeat_by.rs` & `polars-0.9.9/local_dependencies/polars-core/src/chunked_array/ops/repeat_by.rs`

 * *Files identical despite different names*

### Comparing `polars-0.9.8/local_dependencies/polars-core/src/chunked_array/ops/rolling_window.rs` & `polars-0.9.9/local_dependencies/polars-core/src/chunked_array/ops/rolling_window.rs`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,14 @@
 use crate::prelude::*;
 use arrow::array::{Array, PrimitiveArray};
-use num::{Bounded, NumCast, One, Zero};
+use arrow::bitmap::utils::count_zeros;
+use arrow::bitmap::MutableBitmap;
+use num::{Bounded, Float, NumCast, One, Zero};
+use polars_arrow::bit_util::unset_bit_raw;
+use polars_arrow::trusted_len::PushUnchecked;
 use polars_arrow::utils::CustomIterTools;
 use std::ops::{Add, Div, Mul, Rem, Sub};
 
 /// a fold function to compute the sum. Returns a Null if there is a single null in the window
 fn sum_fold<T>(acc: Option<T>, opt_v: Option<T>) -> Option<T>
 where
     T: Add<Output = T> + Copy,
@@ -440,51 +444,152 @@
             builder.append_option(out.get(0));
         }
 
         Ok(builder.finish())
     }
 }
 
+fn variance<T>(vals: &[T]) -> T
+where
+    T: Float + std::iter::Sum,
+{
+    let len = T::from(vals.len()).unwrap();
+    let mean = vals.iter().copied().sum::<T>() / len;
+
+    let mut sum = T::zero();
+    for &val in vals {
+        let v = val - mean;
+        sum = sum + v * v
+    }
+    sum / (len - T::one())
+}
+
 impl<T> ChunkedArray<T>
 where
+    ChunkedArray<T>: IntoSeries,
     T: PolarsFloatType,
+    T::Native: Default + std::iter::Sum + Float,
 {
     pub fn rolling_apply_float<F>(&self, window_size: usize, f: F) -> Result<Self>
     where
         F: Fn(&ChunkedArray<T>) -> Option<T::Native>,
         T::Native: Zero,
     {
         let ca = self.rechunk();
         let arr = ca.downcast_iter().next().unwrap();
 
         let arr_container = ChunkedArray::<T>::new_from_slice("", &[T::Native::zero()]);
         let array_ptr = &arr_container.chunks()[0];
         let ptr = Arc::as_ptr(array_ptr) as *mut dyn Array as *mut PrimitiveArray<T::Native>;
 
-        let mut builder = PrimitiveChunkedBuilder::<T>::new(self.name(), self.len());
-        for _ in 0..window_size - 1 {
-            builder.append_null();
-        }
+        let mut validity = MutableBitmap::with_capacity(ca.len());
+        validity.extend_constant(window_size - 1, false);
+        validity.extend_constant(ca.len() - (window_size - 1), true);
+        let validity_ptr = validity.as_slice().as_ptr() as *mut u8;
+
+        let mut values = AlignedVec::with_capacity(ca.len());
+        values.extend_constant(window_size - 1, Default::default());
 
         for offset in 0..self.len() + 1 - window_size {
             let arr_window = arr.slice(offset, window_size);
 
             // Safety.
             // ptr is not dropped as we are in scope
             // We are also the only owner of the contents of the Arc
             // we do this to reduce heap allocs.
             unsafe {
                 *ptr = arr_window;
             }
 
             let out = f(&arr_container);
-            builder.append_option(out);
+            match out {
+                Some(v) => unsafe { values.push_unchecked(v) },
+                None => unsafe { unset_bit_raw(validity_ptr, offset + window_size - 1) },
+            }
+        }
+        let arr = PrimitiveArray::from_data(
+            T::get_dtype().to_arrow(),
+            values.into(),
+            Some(validity.into()),
+        );
+        Ok(Self::new_from_chunks(self.name(), vec![Arc::new(arr)]))
+    }
+
+    pub fn rolling_var(&self, window_size: usize) -> Self {
+        let ca = self.rechunk();
+        let arr = ca.downcast_iter().next().unwrap();
+        let values = arr.values().as_slice();
+
+        let mut validity = MutableBitmap::with_capacity(ca.len());
+        validity.extend_constant(window_size - 1, false);
+        validity.extend_constant(ca.len() - (window_size - 1), true);
+        let validity_ptr = validity.as_slice().as_ptr() as *mut u8;
+
+        let mut rolling_values = AlignedVec::with_capacity(ca.len());
+        rolling_values.extend_constant(window_size - 1, Default::default());
+
+        if ca.null_count() == 0 {
+            for offset in 0..self.len() + 1 - window_size {
+                let window = &values[offset..offset + window_size];
+                let val = variance(window);
+
+                unsafe {
+                    // Safety:
+                    // We pre-allocated enough capacity
+                    rolling_values.push_unchecked(val);
+                };
+            }
+        } else {
+            let old_validity = arr.validity().as_ref().unwrap().clone();
+            let (bytes, bytes_offset, _) = old_validity.as_slice();
+            for offset in 0..self.len() + 1 - window_size {
+                if count_zeros(bytes, bytes_offset + offset, window_size) > 0 {
+                    unsafe {
+                        // Safety:
+                        // We pre-allocated enough capacity
+                        rolling_values.push_unchecked(Default::default());
+                        // Safety:
+                        // We are in bounds
+                        unset_bit_raw(validity_ptr, offset + window_size - 1)
+                    };
+                } else {
+                    let window = &values[offset..offset + window_size];
+                    let val = variance(window);
+                    // Safety:
+                    // We pre-allocated enough capacity
+                    unsafe { rolling_values.push_unchecked(val) };
+                }
+            }
         }
 
-        Ok(builder.finish())
+        let arr = PrimitiveArray::from_data(
+            T::get_dtype().to_arrow(),
+            rolling_values.into(),
+            Some(validity.into()),
+        );
+        Self::new_from_chunks(self.name(), vec![Arc::new(arr)])
+    }
+
+    pub fn rolling_std(&self, window_size: usize) -> Self {
+        let s = self.rolling_var(window_size).into_series();
+        // Safety:
+        // We are still guarded by the type system.
+        match self.dtype() {
+            DataType::Float32 => unsafe {
+                std::mem::transmute::<Float32Chunked, ChunkedArray<T>>(
+                    s.f32().unwrap().pow_f32(0.5),
+                )
+            },
+            DataType::Float64 => unsafe {
+                std::mem::transmute::<Float64Chunked, ChunkedArray<T>>(
+                    s.f64().unwrap().pow_f64(0.5),
+                )
+            },
+            _ => unreachable!(),
+        }
     }
 }
 
 impl ChunkRollApply for ListChunked {}
 impl ChunkRollApply for Utf8Chunked {}
 impl ChunkRollApply for BooleanChunked {}
 #[cfg(feature = "dtype-categorical")]
@@ -596,8 +701,38 @@
                 Some(3.0),
                 Some(2.0),
                 Some(5.0),
                 Some(11.0)
             ]
         );
     }
+
+    #[test]
+    fn test_rolling_var() {
+        let ca = Float64Chunked::new_from_opt_slice(
+            "foo",
+            &[
+                Some(0.0),
+                Some(1.0),
+                Some(2.0),
+                None,
+                None,
+                Some(5.0),
+                Some(6.0),
+            ],
+        );
+        let out = ca.rolling_var(3).cast::<Int32Type>().unwrap();
+        assert_eq!(
+            Vec::from(&out),
+            &[None, None, Some(1), None, None, None, None,]
+        );
+
+        let ca = Float64Chunked::new_from_slice("", &[0.0, 2.0, 8.0, 3.0, 12.0, 1.0]);
+        let out = ca.rolling_var(3).cast::<Int32Type>().unwrap();
+
+        assert_eq!(
+            Vec::from(&out),
+            &[None, None, Some(17), Some(10), Some(20), Some(34),]
+        );
+        dbg!(out);
+    }
 }
```

### Comparing `polars-0.9.8/local_dependencies/polars-core/src/chunked_array/ops/set.rs` & `polars-0.9.9/local_dependencies/polars-core/src/chunked_array/ops/set.rs`

 * *Files identical despite different names*

### Comparing `polars-0.9.8/local_dependencies/polars-core/src/chunked_array/ops/shift.rs` & `polars-0.9.9/local_dependencies/polars-core/src/chunked_array/ops/shift.rs`

 * *Files identical despite different names*

### Comparing `polars-0.9.8/local_dependencies/polars-core/src/chunked_array/ops/sort.rs` & `polars-0.9.9/local_dependencies/polars-core/src/chunked_array/ops/sort.rs`

 * *Files identical despite different names*

### Comparing `polars-0.9.8/local_dependencies/polars-core/src/chunked_array/ops/take/mod.rs` & `polars-0.9.9/local_dependencies/polars-core/src/chunked_array/ops/take/mod.rs`

 * *Files identical despite different names*

### Comparing `polars-0.9.8/local_dependencies/polars-core/src/chunked_array/ops/take/take_every.rs` & `polars-0.9.9/local_dependencies/polars-core/src/chunked_array/ops/take/take_every.rs`

 * *Files identical despite different names*

### Comparing `polars-0.9.8/local_dependencies/polars-core/src/chunked_array/ops/take/take_random.rs` & `polars-0.9.9/local_dependencies/polars-core/src/chunked_array/ops/take/take_random.rs`

 * *Files identical despite different names*

### Comparing `polars-0.9.8/local_dependencies/polars-core/src/chunked_array/ops/take/take_single.rs` & `polars-0.9.9/local_dependencies/polars-core/src/chunked_array/ops/take/take_single.rs`

 * *Files identical despite different names*

### Comparing `polars-0.9.8/local_dependencies/polars-core/src/chunked_array/ops/take/traits.rs` & `polars-0.9.9/local_dependencies/polars-core/src/chunked_array/ops/take/traits.rs`

 * *Files identical despite different names*

### Comparing `polars-0.9.8/local_dependencies/polars-core/src/chunked_array/ops/unique/mod.rs` & `polars-0.9.9/local_dependencies/polars-core/src/chunked_array/ops/unique/mod.rs`

 * *Files identical despite different names*

### Comparing `polars-0.9.8/local_dependencies/polars-core/src/chunked_array/ops/unique/rank.rs` & `polars-0.9.9/local_dependencies/polars-core/src/chunked_array/ops/unique/rank.rs`

 * *Files identical despite different names*

### Comparing `polars-0.9.8/local_dependencies/polars-core/src/chunked_array/ops/zip.rs` & `polars-0.9.9/local_dependencies/polars-core/src/chunked_array/ops/zip.rs`

 * *Files identical despite different names*

### Comparing `polars-0.9.8/local_dependencies/polars-core/src/chunked_array/random.rs` & `polars-0.9.9/local_dependencies/polars-core/src/chunked_array/random.rs`

 * *Files identical despite different names*

### Comparing `polars-0.9.8/local_dependencies/polars-core/src/chunked_array/strings/json_path.rs` & `polars-0.9.9/local_dependencies/polars-core/src/chunked_array/strings/json_path.rs`

 * *Files identical despite different names*

### Comparing `polars-0.9.8/local_dependencies/polars-core/src/chunked_array/strings/mod.rs` & `polars-0.9.9/local_dependencies/polars-core/src/chunked_array/strings/mod.rs`

 * *Files identical despite different names*

### Comparing `polars-0.9.8/local_dependencies/polars-core/src/chunked_array/temporal/conversion.rs` & `polars-0.9.9/local_dependencies/polars-core/src/chunked_array/temporal/conversion.rs`

 * *Files identical despite different names*

### Comparing `polars-0.9.8/local_dependencies/polars-core/src/chunked_array/temporal/conversions_utils.rs` & `polars-0.9.9/local_dependencies/polars-core/src/chunked_array/temporal/conversions_utils.rs`

 * *Files identical despite different names*

### Comparing `polars-0.9.8/local_dependencies/polars-core/src/chunked_array/temporal/mod.rs` & `polars-0.9.9/local_dependencies/polars-core/src/chunked_array/temporal/mod.rs`

 * *Files identical despite different names*

### Comparing `polars-0.9.8/local_dependencies/polars-core/src/chunked_array/trusted_len.rs` & `polars-0.9.9/local_dependencies/polars-core/src/chunked_array/trusted_len.rs`

 * *Files identical despite different names*

### Comparing `polars-0.9.8/local_dependencies/polars-core/src/chunked_array/upstream_traits.rs` & `polars-0.9.9/local_dependencies/polars-core/src/chunked_array/upstream_traits.rs`

 * *Files identical despite different names*

### Comparing `polars-0.9.8/local_dependencies/polars-core/src/datatypes.rs` & `polars-0.9.9/local_dependencies/polars-core/src/datatypes.rs`

 * *Files identical despite different names*

### Comparing `polars-0.9.8/local_dependencies/polars-core/src/doc/changelog/v0_10_0_11.rs` & `polars-0.9.9/local_dependencies/polars-core/src/doc/changelog/v0_10_0_11.rs`

 * *Files identical despite different names*

### Comparing `polars-0.9.8/local_dependencies/polars-core/src/doc/changelog/v0_7.rs` & `polars-0.9.9/local_dependencies/polars-core/src/doc/changelog/v0_7.rs`

 * *Files identical despite different names*

### Comparing `polars-0.9.8/local_dependencies/polars-core/src/doc/changelog/v0_8.rs` & `polars-0.9.9/local_dependencies/polars-core/src/doc/changelog/v0_8.rs`

 * *Files identical despite different names*

### Comparing `polars-0.9.8/local_dependencies/polars-core/src/doc/changelog/v0_9.rs` & `polars-0.9.9/local_dependencies/polars-core/src/doc/changelog/v0_9.rs`

 * *Files identical despite different names*

### Comparing `polars-0.9.8/local_dependencies/polars-core/src/doc/time.rs` & `polars-0.9.9/local_dependencies/polars-core/src/doc/time.rs`

 * *Files identical despite different names*

### Comparing `polars-0.9.8/local_dependencies/polars-core/src/error.rs` & `polars-0.9.9/local_dependencies/polars-core/src/error.rs`

 * *Files identical despite different names*

### Comparing `polars-0.9.8/local_dependencies/polars-core/src/fmt.rs` & `polars-0.9.9/local_dependencies/polars-core/src/fmt.rs`

 * *Files identical despite different names*

### Comparing `polars-0.9.8/local_dependencies/polars-core/src/frame/arithmetic.rs` & `polars-0.9.9/local_dependencies/polars-core/src/frame/arithmetic.rs`

 * *Files identical despite different names*

### Comparing `polars-0.9.8/local_dependencies/polars-core/src/frame/asof_join.rs` & `polars-0.9.9/local_dependencies/polars-core/src/frame/asof_join.rs`

 * *Files identical despite different names*

### Comparing `polars-0.9.8/local_dependencies/polars-core/src/frame/cross_join.rs` & `polars-0.9.9/local_dependencies/polars-core/src/frame/cross_join.rs`

 * *Files identical despite different names*

### Comparing `polars-0.9.8/local_dependencies/polars-core/src/frame/explode.rs` & `polars-0.9.9/local_dependencies/polars-core/src/frame/explode.rs`

 * *Files 0% similar despite different names*

```diff
@@ -68,15 +68,15 @@
     ///  +-----+-----+-----+
     ///  | 2   | 3   | 1   |
     ///  +-----+-----+-----+
     ///  | 2   | 3   | 1   |
     ///  +-----+-----+-----+
     /// ```
     pub fn explode<'a, J, S: Selection<'a, J>>(&self, columns: S) -> Result<DataFrame> {
-        // We need to sort the column by order of original occurence. Otherwise the insert by index
+        // We need to sort the column by order of original occurrence. Otherwise the insert by index
         // below will panic
         let mut columns = self.select_series(columns)?;
         columns.sort_by(|sa, sb| {
             self.name_to_idx(sa.name())
                 .expect("checked above")
                 .partial_cmp(&self.name_to_idx(sb.name()).expect("checked above"))
                 .expect("cmp usize -> Ordering")
```

### Comparing `polars-0.9.8/local_dependencies/polars-core/src/frame/groupby/aggregations.rs` & `polars-0.9.9/local_dependencies/polars-core/src/frame/groupby/aggregations.rs`

 * *Files identical despite different names*

### Comparing `polars-0.9.8/local_dependencies/polars-core/src/frame/groupby/hashing.rs` & `polars-0.9.9/local_dependencies/polars-core/src/frame/groupby/hashing.rs`

 * *Files identical despite different names*

### Comparing `polars-0.9.8/local_dependencies/polars-core/src/frame/groupby/mod.rs` & `polars-0.9.9/local_dependencies/polars-core/src/frame/groupby/mod.rs`

 * *Files identical despite different names*

### Comparing `polars-0.9.8/local_dependencies/polars-core/src/frame/groupby/pivot.rs` & `polars-0.9.9/local_dependencies/polars-core/src/frame/groupby/pivot.rs`

 * *Files identical despite different names*

### Comparing `polars-0.9.8/local_dependencies/polars-core/src/frame/groupby/resample.rs` & `polars-0.9.9/local_dependencies/polars-core/src/frame/groupby/resample.rs`

 * *Files identical despite different names*

### Comparing `polars-0.9.8/local_dependencies/polars-core/src/frame/hash_join/mod.rs` & `polars-0.9.9/local_dependencies/polars-core/src/frame/hash_join/mod.rs`

 * *Files identical despite different names*

### Comparing `polars-0.9.8/local_dependencies/polars-core/src/frame/hash_join/multiple_keys.rs` & `polars-0.9.9/local_dependencies/polars-core/src/frame/hash_join/multiple_keys.rs`

 * *Files identical despite different names*

### Comparing `polars-0.9.8/local_dependencies/polars-core/src/frame/mod.rs` & `polars-0.9.9/local_dependencies/polars-core/src/frame/mod.rs`

 * *Files identical despite different names*

### Comparing `polars-0.9.8/local_dependencies/polars-core/src/frame/row.rs` & `polars-0.9.9/local_dependencies/polars-core/src/frame/row.rs`

 * *Files identical despite different names*

### Comparing `polars-0.9.8/local_dependencies/polars-core/src/frame/select.rs` & `polars-0.9.9/local_dependencies/polars-core/src/frame/select.rs`

 * *Files identical despite different names*

### Comparing `polars-0.9.8/local_dependencies/polars-core/src/frame/upstream_traits.rs` & `polars-0.9.9/local_dependencies/polars-core/src/frame/upstream_traits.rs`

 * *Files identical despite different names*

### Comparing `polars-0.9.8/local_dependencies/polars-core/src/functions.rs` & `polars-0.9.9/local_dependencies/polars-core/src/functions.rs`

 * *Files identical despite different names*

### Comparing `polars-0.9.8/local_dependencies/polars-core/src/lib.rs` & `polars-0.9.9/local_dependencies/polars-core/src/lib.rs`

 * *Files identical despite different names*

### Comparing `polars-0.9.8/local_dependencies/polars-core/src/prelude.rs` & `polars-0.9.9/local_dependencies/polars-core/src/prelude.rs`

 * *Files identical despite different names*

### Comparing `polars-0.9.8/local_dependencies/polars-core/src/serde/chunked_array.rs` & `polars-0.9.9/local_dependencies/polars-core/src/serde/chunked_array.rs`

 * *Files identical despite different names*

### Comparing `polars-0.9.8/local_dependencies/polars-core/src/serde/mod.rs` & `polars-0.9.9/local_dependencies/polars-core/src/serde/mod.rs`

 * *Files identical despite different names*

### Comparing `polars-0.9.8/local_dependencies/polars-core/src/serde/series.rs` & `polars-0.9.9/local_dependencies/polars-core/src/serde/series.rs`

 * *Files identical despite different names*

### Comparing `polars-0.9.8/local_dependencies/polars-core/src/series/arithmetic.rs` & `polars-0.9.9/local_dependencies/polars-core/src/series/arithmetic.rs`

 * *Files identical despite different names*

### Comparing `polars-0.9.8/local_dependencies/polars-core/src/series/comparison.rs` & `polars-0.9.9/local_dependencies/polars-core/src/series/comparison.rs`

 * *Files identical despite different names*

### Comparing `polars-0.9.8/local_dependencies/polars-core/src/series/implementations/dates.rs` & `polars-0.9.9/local_dependencies/polars-core/src/series/implementations/dates.rs`

 * *Files identical despite different names*

### Comparing `polars-0.9.8/local_dependencies/polars-core/src/series/implementations/mod.rs` & `polars-0.9.9/local_dependencies/polars-core/src/series/implementations/mod.rs`

 * *Files identical despite different names*

### Comparing `polars-0.9.8/local_dependencies/polars-core/src/series/implementations/object.rs` & `polars-0.9.9/local_dependencies/polars-core/src/series/implementations/object.rs`

 * *Files identical despite different names*

### Comparing `polars-0.9.8/local_dependencies/polars-core/src/series/iterator.rs` & `polars-0.9.9/local_dependencies/polars-core/src/series/iterator.rs`

 * *Files identical despite different names*

### Comparing `polars-0.9.8/local_dependencies/polars-core/src/series/mod.rs` & `polars-0.9.9/local_dependencies/polars-core/src/series/mod.rs`

 * *Files identical despite different names*

### Comparing `polars-0.9.8/local_dependencies/polars-core/src/series/ops/moment.rs` & `polars-0.9.9/local_dependencies/polars-core/src/series/ops/moment.rs`

 * *Files identical despite different names*

### Comparing `polars-0.9.8/local_dependencies/polars-core/src/series/ops/to_list.rs` & `polars-0.9.9/local_dependencies/polars-core/src/series/ops/to_list.rs`

 * *Files identical despite different names*

### Comparing `polars-0.9.8/local_dependencies/polars-core/src/testing.rs` & `polars-0.9.9/local_dependencies/polars-core/src/testing.rs`

 * *Files identical despite different names*

### Comparing `polars-0.9.8/local_dependencies/polars-core/src/utils.rs` & `polars-0.9.9/local_dependencies/polars-core/src/utils.rs`

 * *Files identical despite different names*

### Comparing `polars-0.9.8/local_dependencies/polars-core/src/vector_hasher.rs` & `polars-0.9.9/local_dependencies/polars-core/src/vector_hasher.rs`

 * *Files identical despite different names*

### Comparing `polars-0.9.8/Cargo.toml` & `polars-0.9.9/Cargo.toml`

 * *Files 0% similar despite different names*

```diff
@@ -44,13 +44,13 @@
 documentation = "https://pola-rs.github.io/polars-book/"
 edition = "2018"
 homepage = "https://github.com/pola-rs/polars"
 license = "MIT"
 name = "py-polars"
 readme = "README.md"
 repository = "https://github.com/pola-rs/polars"
-version = "0.9.8"
+version = "0.9.9"
 [profile.release]
 codegen-units = 1
 lto = "fat"
 
 [workspace]
```

### Comparing `polars-0.9.8/CHANGELOG.md` & `polars-0.9.9/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `polars-0.9.8/README.md` & `polars-0.9.9/README.md`

 * *Files identical despite different names*

### Comparing `polars-0.9.8/docs/Makefile` & `polars-0.9.9/docs/Makefile`

 * *Files identical despite different names*

### Comparing `polars-0.9.8/docs/_templates/autosummary/class.rst` & `polars-0.9.9/docs/_templates/autosummary/class.rst`

 * *Files identical despite different names*

### Comparing `polars-0.9.8/docs/img/polars_logo.png` & `polars-0.9.9/docs/img/polars_logo.png`

 * *Files identical despite different names*

### Comparing `polars-0.9.8/docs/source/conf.py` & `polars-0.9.9/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `polars-0.9.8/docs/source/reference/dataframe.rst` & `polars-0.9.9/docs/source/reference/dataframe.rst`

 * *Files identical despite different names*

### Comparing `polars-0.9.8/docs/source/reference/expression.rst` & `polars-0.9.9/docs/source/reference/expression.rst`

 * *Files identical despite different names*

### Comparing `polars-0.9.8/docs/source/reference/io.rst` & `polars-0.9.9/docs/source/reference/io.rst`

 * *Files identical despite different names*

### Comparing `polars-0.9.8/docs/source/reference/lazyframe.rst` & `polars-0.9.9/docs/source/reference/lazyframe.rst`

 * *Files identical despite different names*

### Comparing `polars-0.9.8/docs/source/reference/series.rst` & `polars-0.9.9/docs/source/reference/series.rst`

 * *Files identical despite different names*

### Comparing `polars-0.9.8/legacy/setup.py` & `polars-0.9.9/legacy/setup.py`

 * *Files identical despite different names*

### Comparing `polars-0.9.8/polars/__init__.py` & `polars-0.9.9/polars/__init__.py`

 * *Files identical despite different names*

### Comparing `polars-0.9.8/polars/_html.py` & `polars-0.9.9/polars/_html.py`

 * *Files identical despite different names*

### Comparing `polars-0.9.8/polars/cfg.py` & `polars-0.9.9/polars/cfg.py`

 * *Files identical despite different names*

### Comparing `polars-0.9.8/polars/convert.py` & `polars-0.9.9/polars/convert.py`

 * *Files identical despite different names*

### Comparing `polars-0.9.8/polars/datatypes.py` & `polars-0.9.9/polars/datatypes.py`

 * *Files identical despite different names*

### Comparing `polars-0.9.8/polars/eager/frame.py` & `polars-0.9.9/polars/eager/frame.py`

 * *Files identical despite different names*

### Comparing `polars-0.9.8/polars/eager/series.py` & `polars-0.9.9/polars/eager/series.py`

 * *Files identical despite different names*

### Comparing `polars-0.9.8/polars/functions.py` & `polars-0.9.9/polars/functions.py`

 * *Files identical despite different names*

### Comparing `polars-0.9.8/polars/internals/construction.py` & `polars-0.9.9/polars/internals/construction.py`

 * *Files identical despite different names*

### Comparing `polars-0.9.8/polars/io.py` & `polars-0.9.9/polars/io.py`

 * *Files identical despite different names*

### Comparing `polars-0.9.8/polars/lazy/expr.py` & `polars-0.9.9/polars/lazy/expr.py`

 * *Files identical despite different names*

### Comparing `polars-0.9.8/polars/lazy/frame.py` & `polars-0.9.9/polars/lazy/frame.py`

 * *Files identical despite different names*

### Comparing `polars-0.9.8/polars/lazy/functions.py` & `polars-0.9.9/polars/lazy/functions.py`

 * *Files identical despite different names*

### Comparing `polars-0.9.8/polars/lazy/whenthen.py` & `polars-0.9.9/polars/lazy/whenthen.py`

 * *Files identical despite different names*

### Comparing `polars-0.9.8/polars/string_cache.py` & `polars-0.9.9/polars/string_cache.py`

 * *Files identical despite different names*

### Comparing `polars-0.9.8/polars/utils.py` & `polars-0.9.9/polars/utils.py`

 * *Files identical despite different names*

### Comparing `polars-0.9.8/src/apply/dataframe.rs` & `polars-0.9.9/src/apply/dataframe.rs`

 * *Files identical despite different names*

### Comparing `polars-0.9.8/src/apply/mod.rs` & `polars-0.9.9/src/apply/mod.rs`

 * *Files identical despite different names*

### Comparing `polars-0.9.8/src/apply/series.rs` & `polars-0.9.9/src/apply/series.rs`

 * *Files identical despite different names*

### Comparing `polars-0.9.8/src/arrow_interop/to_py.rs` & `polars-0.9.9/src/arrow_interop/to_py.rs`

 * *Files identical despite different names*

### Comparing `polars-0.9.8/src/arrow_interop/to_rust.rs` & `polars-0.9.9/src/arrow_interop/to_rust.rs`

 * *Files identical despite different names*

### Comparing `polars-0.9.8/src/conversion.rs` & `polars-0.9.9/src/conversion.rs`

 * *Files 0% similar despite different names*

```diff
@@ -166,17 +166,16 @@
             DataType::UInt32 => pl.getattr("UInt32").unwrap().into(),
             DataType::UInt64 => pl.getattr("UInt64").unwrap().into(),
             DataType::Float32 => pl.getattr("Float32").unwrap().into(),
             DataType::Float64 => pl.getattr("Float64").unwrap().into(),
             DataType::Boolean => pl.getattr("Boolean").unwrap().into(),
             DataType::Utf8 => pl.getattr("Utf8").unwrap().into(),
             DataType::List(_) => pl.getattr("List").unwrap().into(),
-            dt => panic!("{} not supported", dt)
+            dt => panic!("{} not supported", dt),
         }
-
     }
 }
 
 impl ToPyObject for Wrap<AnyValue<'_>> {
     fn to_object(&self, py: Python) -> PyObject {
         self.clone().into_py(py)
     }
@@ -188,31 +187,30 @@
             Ok(AnyValue::Int64(v).into())
         } else if let Ok(v) = ob.extract::<f64>() {
             Ok(AnyValue::Float64(v).into())
         } else if let Ok(v) = ob.extract::<&'s str>() {
             Ok(AnyValue::Utf8(v).into())
         } else if let Ok(v) = ob.extract::<bool>() {
             Ok(AnyValue::Boolean(v).into())
-        }
-        else if ob.get_type().name()?.contains("datetime") {
+        } else if ob.get_type().name()?.contains("datetime") {
             let gil = Python::acquire_gil();
             let py = gil.python();
 
             // windows
             #[cfg(target_arch = "windows")]
             {
                 let kwargs = PyDict::new(py);
                 kwargs.set_item("tzinfo", py.None())?;
                 let dt = ob.call_method("replace", (), Some(kwargs))?;
 
                 let pytz = PyModule::import(py, "pytz")?;
-                let tz = pytz.call_method("timezone", ("UTC", ), None)?;
+                let tz = pytz.call_method("timezone", ("UTC",), None)?;
                 let kwargs = PyDict::new(py);
                 kwargs.set_item("is_dst", py.None())?;
-                let loc_tz = tz.call_method("localize", (dt, ), Some(kwargs))?;
+                let loc_tz = tz.call_method("localize", (dt,), Some(kwargs))?;
                 loc_tz.call_method0("timestamp")?;
                 // s to ms
                 let v = ts.extract::<f64>()? as i64;
                 Ok(AnyValue::Date64(v * 1000).into())
             }
             // unix
             #[cfg(not(target_arch = "windows"))]
```

### Comparing `polars-0.9.8/src/dataframe.rs` & `polars-0.9.9/src/dataframe.rs`

 * *Files 0% similar despite different names*

```diff
@@ -94,15 +94,15 @@
         n_threads: Option<usize>,
         path: Option<String>,
         overwrite_dtype: Option<Vec<(&str, &PyAny)>>,
         overwrite_dtype_slice: Option<Vec<&PyAny>>,
         low_memory: bool,
         comment_char: Option<&str>,
         null_values: Option<Wrap<NullValues>>,
-        parse_dates: bool
+        parse_dates: bool,
     ) -> PyResult<Self> {
         let null_values = null_values.map(|w| w.0);
         let comment_char = comment_char.map(|s| s.as_bytes()[0]);
         let encoding = match encoding {
             "utf8" => CsvEncoding::Utf8,
             "utf8-lossy" => CsvEncoding::LossyUtf8,
             e => {
```

### Comparing `polars-0.9.8/src/datatypes.rs` & `polars-0.9.9/src/datatypes.rs`

 * *Files identical despite different names*

### Comparing `polars-0.9.8/src/file.rs` & `polars-0.9.9/src/file.rs`

 * *Files identical despite different names*

### Comparing `polars-0.9.8/src/lazy/dataframe.rs` & `polars-0.9.9/src/lazy/dataframe.rs`

 * *Files identical despite different names*

### Comparing `polars-0.9.8/src/lazy/dsl.rs` & `polars-0.9.9/src/lazy/dsl.rs`

 * *Files 4% similar despite different names*

```diff
@@ -760,72 +760,47 @@
     ) -> Self {
         self.inner
             .clone()
             .rolling_mean(window_size, weight.as_deref(), ignore_null, min_periods)
             .into()
     }
 
-    pub fn rolling_std(
-        &self,
-        window_size: usize,
-    ) -> Self {
-        self.inner
-            .clone()
-            .rolling_apply_float(window_size, |ca| ca.std()
-            )
-            .into()
+    pub fn rolling_std(&self, window_size: usize) -> Self {
+        self.inner.clone().rolling_std(window_size).into()
     }
 
-    pub fn rolling_var(
-        &self,
-        window_size: usize,
-    ) -> Self {
-        self.inner
-            .clone()
-            .rolling_apply_float(window_size, |ca| ca.var()
-            )
-            .into()
+    pub fn rolling_var(&self, window_size: usize) -> Self {
+        self.inner.clone().rolling_var(window_size).into()
     }
 
-    pub fn rolling_median(
-        &self,
-        window_size: usize,
-    ) -> Self {
+    pub fn rolling_median(&self, window_size: usize) -> Self {
         self.inner
             .clone()
-            .rolling_apply_float(window_size, |ca| ChunkAgg::median(ca)
-            )
+            .rolling_apply_float(window_size, |ca| ChunkAgg::median(ca))
             .into()
     }
 
-    pub fn rolling_quantile(
-        &self,
-        window_size: usize,
-        quantile: f64
-    ) -> Self {
+    pub fn rolling_quantile(&self, window_size: usize, quantile: f64) -> Self {
         self.inner
             .clone()
-            .rolling_apply_float(window_size, move |ca| ChunkAgg::quantile(ca, quantile).unwrap()
-            )
+            .rolling_apply_float(window_size, move |ca| {
+                ChunkAgg::quantile(ca, quantile).unwrap()
+            })
             .into()
     }
 
-    pub fn rolling_skew(
-        &self,
-        window_size: usize,
-        bias: bool
-    ) -> Self {
+    pub fn rolling_skew(&self, window_size: usize, bias: bool) -> Self {
         self.inner
             .clone()
-            .rolling_apply_float(window_size, move |ca| ca.clone().into_series().skew(bias).unwrap()
-            )
+            .rolling_apply_float(window_size, move |ca| {
+                ca.clone().into_series().skew(bias).unwrap()
+            })
             .into()
     }
 
-
     fn lst_max(&self) -> Self {
         self.inner
             .clone()
             .map(
                 |s| Ok(s.list()?.lst_max()),
                 GetOutput::map_field(|f| {
                     if let DataType::List(adt) = f.data_type() {
```

### Comparing `polars-0.9.8/src/lib.rs` & `polars-0.9.9/src/lib.rs`

 * *Files 2% similar despite different names*

```diff
@@ -4,20 +4,20 @@
 
 use pyo3::prelude::*;
 use pyo3::wrap_pyfunction;
 
 use crate::lazy::dsl::PyExpr;
 use crate::{
     dataframe::PyDataFrame,
+    file::EitherRustPythonFile,
     lazy::{
         dataframe::{PyLazyFrame, PyLazyGroupBy},
         dsl,
     },
     series::PySeries,
-    file::EitherRustPythonFile
 };
 
 pub mod apply;
 pub mod arrow_interop;
 pub mod conversion;
 pub mod dataframe;
 pub mod datatypes;
@@ -26,20 +26,20 @@
 pub mod lazy;
 pub mod npy;
 pub mod prelude;
 pub mod series;
 pub mod utils;
 
 use crate::conversion::{get_df, get_pyseq, Wrap};
-use polars_core::export::arrow::io::ipc::read::read_file_metadata;
 use crate::error::PyPolarsEr;
+use crate::file::get_either_file;
+use crate::prelude::DataType;
 use mimalloc::MiMalloc;
+use polars_core::export::arrow::io::ipc::read::read_file_metadata;
 use pyo3::types::PyDict;
-use crate::prelude::DataType;
-use crate::file::get_either_file;
 
 #[global_allocator]
 static GLOBAL: MiMalloc = MiMalloc;
 
 #[pyfunction]
 fn col(name: &str) -> dsl::PyExpr {
     dsl::col(name)
@@ -136,26 +136,21 @@
         let item = res?;
         let other = get_df(item)?;
         df.vstack_mut(&other).map_err(PyPolarsEr::from)?;
     }
     Ok(df.into())
 }
 
-
-
-
 #[pyfunction]
-fn ipc_schema(py: Python, py_f: PyObject) -> PyResult<PyObject>{
+fn ipc_schema(py: Python, py_f: PyObject) -> PyResult<PyObject> {
     let metadata = match get_either_file(py_f, false)? {
         EitherRustPythonFile::Rust(mut r) => {
             read_file_metadata(&mut r).map_err(PyPolarsEr::from)?
-        },
-        EitherRustPythonFile::Py(mut r) => {
-            read_file_metadata(&mut r).map_err(PyPolarsEr::from)?
         }
+        EitherRustPythonFile::Py(mut r) => read_file_metadata(&mut r).map_err(PyPolarsEr::from)?,
     };
 
     let dict = PyDict::new(py);
     for field in metadata.schema().fields() {
         let dt: Wrap<DataType> = Wrap((&field.data_type).into());
         dict.set_item(field.name(), dt.to_object(py))?;
     }
```

### Comparing `polars-0.9.8/src/npy.rs` & `polars-0.9.9/src/npy.rs`

 * *Files identical despite different names*

### Comparing `polars-0.9.8/src/series.rs` & `polars-0.9.9/src/series.rs`

 * *Files identical despite different names*

### Comparing `polars-0.9.8/src/utils.rs` & `polars-0.9.9/src/utils.rs`

 * *Files identical despite different names*

### Comparing `polars-0.9.8/tasks.sh` & `polars-0.9.9/tasks.sh`

 * *Files identical despite different names*

### Comparing `polars-0.9.8/tests/conftest.py` & `polars-0.9.9/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `polars-0.9.8/tests/db-benchmark/groupby-datagen.R` & `polars-0.9.9/tests/db-benchmark/groupby-datagen.R`

 * *Files identical despite different names*

### Comparing `polars-0.9.8/tests/db-benchmark/main.py` & `polars-0.9.9/tests/db-benchmark/main.py`

 * *Files identical despite different names*

### Comparing `polars-0.9.8/tests/test_df.py` & `polars-0.9.9/tests/test_df.py`

 * *Files 0% similar despite different names*

```diff
@@ -368,14 +368,21 @@
 
     assert not df.head(5).frame_equal(df.tail(5))
     # check if it doesn't fail when out of bounds
     assert df.head(100).height == 10
     assert df.tail(100).height == 10
 
 
+def test_explode():
+    df = pl.DataFrame({"letters": ["c", "a"], "nrs": [[1, 2], [1, 3]]})
+    out = df.explode("nrs")
+    out["letters"].to_list() == ["c", "c", "a", "a"]
+    out["nrs"].to_list() == [1, 2, 1, 3]
+
+
 def test_groupby():
     df = pl.DataFrame(
         {
             "a": ["a", "b", "a", "b", "b", "c"],
             "b": [1, 2, 3, 4, 5, 6],
             "c": [6, 5, 4, 3, 2, 1],
         }
```

### Comparing `polars-0.9.8/tests/test_interop.py` & `polars-0.9.9/tests/test_interop.py`

 * *Files identical despite different names*

### Comparing `polars-0.9.8/tests/test_io.py` & `polars-0.9.9/tests/test_io.py`

 * *Files identical despite different names*

### Comparing `polars-0.9.8/tests/test_lazy.py` & `polars-0.9.9/tests/test_lazy.py`

 * *Files identical despite different names*

### Comparing `polars-0.9.8/tests/test_series.py` & `polars-0.9.9/tests/test_series.py`

 * *Files identical despite different names*

### Comparing `polars-0.9.8/PKG-INFO` & `polars-0.9.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: polars
-Version: 0.9.8
+Version: 0.9.9
 Requires-Dist: numpy
 Requires-Dist: pyarrow>=4.0.*
 Home-Page: https://github.com/pola-rs/polars
 Author: ritchie46 <ritchie46@gmail.com>
 Author-email: ritchie46 <ritchie46@gmail.com>
 License: MIT
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
```

