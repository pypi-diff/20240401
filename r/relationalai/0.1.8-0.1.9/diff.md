# Comparing `tmp/relationalai-0.1.8.tar.gz` & `tmp/relationalai-0.1.9.tar.gz`

## Comparing `relationalai-0.1.8.tar` & `relationalai-0.1.9.tar`

### file list

```diff
@@ -1,121 +1,121 @@
--rw-r--r--   0        0        0     1947 2020-02-02 00:00:00.000000 relationalai-0.1.8/CONTRIBUTING.md
--rw-r--r--   0        0        0     2744 2020-02-02 00:00:00.000000 relationalai-0.1.8/README.md
--rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 relationalai-0.1.8/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 relationalai-0.1.8/.github/workflows/ruff.yml
--rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 relationalai-0.1.8/docs/README.md
--rw-r--r--   0        0        0    16617 2020-02-02 00:00:00.000000 relationalai-0.1.8/docs/getting_started.md
--rw-r--r--   0        0        0     9875 2020-02-02 00:00:00.000000 relationalai-0.1.8/docs/_old/OLD_pyrel_quickstart.md
--rw-r--r--   0        0        0     3956 2020-02-02 00:00:00.000000 relationalai-0.1.8/docs/_old/metamodel.md
--rw-r--r--   0        0        0     5935 2020-02-02 00:00:00.000000 relationalai-0.1.8/docs/_old/python_dsl.md
--rw-r--r--   0        0        0     9371 2020-02-02 00:00:00.000000 relationalai-0.1.8/docs/_old/quickstart.md
--rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 relationalai-0.1.8/docs/api_reference/README.md
--rw-r--r--   0        0        0     8436 2020-02-02 00:00:00.000000 relationalai-0.1.8/docs/api_reference/cli/README.md
--rw-r--r--   0        0        0    16584 2020-02-02 00:00:00.000000 relationalai-0.1.8/docs/api_reference/python/Aggregates.md
--rw-r--r--   0        0        0     9333 2020-02-02 00:00:00.000000 relationalai-0.1.8/docs/api_reference/python/Context.md
--rw-r--r--   0        0        0     9650 2020-02-02 00:00:00.000000 relationalai-0.1.8/docs/api_reference/python/ContextSelect.md
--rw-r--r--   0        0        0     1858 2020-02-02 00:00:00.000000 relationalai-0.1.8/docs/api_reference/python/Expression.md
--rw-r--r--   0        0        0     5046 2020-02-02 00:00:00.000000 relationalai-0.1.8/docs/api_reference/python/Instance.md
--rw-r--r--   0        0        0     1549 2020-02-02 00:00:00.000000 relationalai-0.1.8/docs/api_reference/python/InstanceProperty.md
--rw-r--r--   0        0        0    24150 2020-02-02 00:00:00.000000 relationalai-0.1.8/docs/api_reference/python/Model.md
--rw-r--r--   0        0        0    23126 2020-02-02 00:00:00.000000 relationalai-0.1.8/docs/api_reference/python/Producer.md
--rw-r--r--   0        0        0     3186 2020-02-02 00:00:00.000000 relationalai-0.1.8/docs/api_reference/python/README.md
--rw-r--r--   0        0        0     6621 2020-02-02 00:00:00.000000 relationalai-0.1.8/docs/api_reference/python/Type.md
--rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 relationalai-0.1.8/docs/api_reference/sql/README.md
--rw-r--r--   0        0        0     1203 2020-02-02 00:00:00.000000 relationalai-0.1.8/examples/README.md
--rw-r--r--   0        0        0     5614 2020-02-02 00:00:00.000000 relationalai-0.1.8/examples/SF_pagerank.ipynb
--rw-r--r--   0        0        0      914 2020-02-02 00:00:00.000000 relationalai-0.1.8/examples/cdc.py
--rw-r--r--   0        0        0      935 2020-02-02 00:00:00.000000 relationalai-0.1.8/examples/emit_playground.py
--rw-r--r--   0        0        0      589 2020-02-02 00:00:00.000000 relationalai-0.1.8/examples/found.py
--rw-r--r--   0        0        0     6699 2020-02-02 00:00:00.000000 relationalai-0.1.8/examples/fraud.ipynb
--rw-r--r--   0        0        0     3028 2020-02-02 00:00:00.000000 relationalai-0.1.8/examples/fraud.py
--rw-r--r--   0        0        0   698999 2020-02-02 00:00:00.000000 relationalai-0.1.8/examples/graph.ipynb
--rw-r--r--   0        0        0     1254 2020-02-02 00:00:00.000000 relationalai-0.1.8/examples/graph.py
--rw-r--r--   0        0        0     3470 2020-02-02 00:00:00.000000 relationalai-0.1.8/examples/graphlib.py
--rw-r--r--   0        0        0      312 2020-02-02 00:00:00.000000 relationalai-0.1.8/examples/load_raw.py
--rw-r--r--   0        0        0      627 2020-02-02 00:00:00.000000 relationalai-0.1.8/examples/or_types.py
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 relationalai-0.1.8/examples/requirements.txt
--rw-r--r--   0        0        0      480 2020-02-02 00:00:00.000000 relationalai-0.1.8/examples/simple.py
--rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 relationalai-0.1.8/examples/simple_recursion.py
--rw-r--r--   0        0        0      722 2020-02-02 00:00:00.000000 relationalai-0.1.8/examples/simple_streamlit.py
--rw-r--r--   0        0        0     2430 2020-02-02 00:00:00.000000 relationalai-0.1.8/examples/snowflake_pagerank.py
--rw-r--r--   0        0        0     2403 2020-02-02 00:00:00.000000 relationalai-0.1.8/examples/solver.py
--rw-r--r--   0        0        0     4740 2020-02-02 00:00:00.000000 relationalai-0.1.8/examples/data/people.csv
--rw-r--r--   0        0        0    10518 2020-02-02 00:00:00.000000 relationalai-0.1.8/examples/data/transactions.csv
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 relationalai-0.1.8/examples/rel/bar.rel
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 relationalai-0.1.8/examples/rel/foo.rel
--rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 relationalai-0.1.8/examples/rel/solver.rel
--rw-r--r--   0        0        0     3709 2020-02-02 00:00:00.000000 relationalai-0.1.8/src/gentest/README.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 relationalai-0.1.8/src/gentest/__init__.py
--rw-r--r--   0        0        0    12342 2020-02-02 00:00:00.000000 relationalai-0.1.8/src/gentest/emit.py
--rw-r--r--   0        0        0     1301 2020-02-02 00:00:00.000000 relationalai-0.1.8/src/gentest/exec.py
--rw-r--r--   0        0        0      792 2020-02-02 00:00:00.000000 relationalai-0.1.8/src/gentest/fixtures.py
--rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 relationalai-0.1.8/src/gentest/patch.py
--rw-r--r--   0        0        0     7629 2020-02-02 00:00:00.000000 relationalai-0.1.8/src/gentest/util.py
--rwxr-xr-x   0        0        0     3521 2020-02-02 00:00:00.000000 relationalai-0.1.8/src/gentest/cli/__main__.py
--rw-r--r--   0        0        0     1299 2020-02-02 00:00:00.000000 relationalai-0.1.8/src/gentest/cli/collect_failures.py
--rw-r--r--   0        0        0     1331 2020-02-02 00:00:00.000000 relationalai-0.1.8/src/gentest/cli/collect_tests.py
--rw-r--r--   0        0        0     5707 2020-02-02 00:00:00.000000 relationalai-0.1.8/src/gentest/cli/repro.py
--rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 relationalai-0.1.8/src/gentest/cli/run_tests.py
--rw-r--r--   0        0        0    15710 2020-02-02 00:00:00.000000 relationalai-0.1.8/src/gentest/cli/watch.py
--rw-r--r--   0        0        0     3232 2020-02-02 00:00:00.000000 relationalai-0.1.8/src/gentest/gen/action.py
--rw-r--r--   0        0        0     5461 2020-02-02 00:00:00.000000 relationalai-0.1.8/src/gentest/gen/context.py
--rw-r--r--   0        0        0     1610 2020-02-02 00:00:00.000000 relationalai-0.1.8/src/gentest/gen/document.py
--rw-r--r--   0        0        0      442 2020-02-02 00:00:00.000000 relationalai-0.1.8/src/gentest/gen/error.py
--rw-r--r--   0        0        0     6095 2020-02-02 00:00:00.000000 relationalai-0.1.8/src/gentest/gen/group_limited.py
--rw-r--r--   0        0        0     4662 2020-02-02 00:00:00.000000 relationalai-0.1.8/src/gentest/gen/ir.py
--rw-r--r--   0        0        0    17029 2020-02-02 00:00:00.000000 relationalai-0.1.8/src/gentest/gen/scope.py
--rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 relationalai-0.1.8/src/gentest/gen/staged.py
--rw-r--r--   0        0        0     2888 2020-02-02 00:00:00.000000 relationalai-0.1.8/src/gentest/gen/task.py
--rw-r--r--   0        0        0     2204 2020-02-02 00:00:00.000000 relationalai-0.1.8/src/gentest/gen/test.py
--rw-r--r--   0        0        0     2863 2020-02-02 00:00:00.000000 relationalai-0.1.8/src/gentest/harness/database.py
--rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 relationalai-0.1.8/src/gentest/harness/vendor_types.py
--rw-r--r--   0        0        0     1709 2020-02-02 00:00:00.000000 relationalai-0.1.8/src/gentest/validate/diff.py
--rw-r--r--   0        0        0     5588 2020-02-02 00:00:00.000000 relationalai-0.1.8/src/gentest/validate/errors.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 relationalai-0.1.8/src/gentest/validate/mapping.py
--rw-r--r--   0        0        0     5374 2020-02-02 00:00:00.000000 relationalai-0.1.8/src/gentest/validate/roundtrip.py
--rw-r--r--   0        0        0     1284 2020-02-02 00:00:00.000000 relationalai-0.1.8/src/relationalai/__init__.py
--rw-r--r--   0        0        0     5906 2020-02-02 00:00:00.000000 relationalai-0.1.8/src/relationalai/compiler.py
--rw-r--r--   0        0        0     7274 2020-02-02 00:00:00.000000 relationalai-0.1.8/src/relationalai/debugging.py
--rw-r--r--   0        0        0    34043 2020-02-02 00:00:00.000000 relationalai-0.1.8/src/relationalai/dsl.py
--rw-r--r--   0        0        0     8992 2020-02-02 00:00:00.000000 relationalai-0.1.8/src/relationalai/errors.py
--rw-r--r--   0        0        0    26388 2020-02-02 00:00:00.000000 relationalai-0.1.8/src/relationalai/metagen.py
--rw-r--r--   0        0        0    22355 2020-02-02 00:00:00.000000 relationalai-0.1.8/src/relationalai/metamodel.py
--rw-r--r--   0        0        0    26353 2020-02-02 00:00:00.000000 relationalai-0.1.8/src/relationalai/rel.py
--rw-r--r--   0        0        0      914 2020-02-02 00:00:00.000000 relationalai-0.1.8/src/relationalai/analysis/whynot.py
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 relationalai-0.1.8/src/relationalai/clients/__init__.py
--rw-r--r--   0        0        0     6468 2020-02-02 00:00:00.000000 relationalai-0.1.8/src/relationalai/clients/azure.py
--rw-r--r--   0        0        0     8153 2020-02-02 00:00:00.000000 relationalai-0.1.8/src/relationalai/clients/client.py
--rw-r--r--   0        0        0     4275 2020-02-02 00:00:00.000000 relationalai-0.1.8/src/relationalai/clients/config.py
--rw-r--r--   0        0        0    26236 2020-02-02 00:00:00.000000 relationalai-0.1.8/src/relationalai/clients/snowflake.py
--rw-r--r--   0        0        0    10405 2020-02-02 00:00:00.000000 relationalai-0.1.8/src/relationalai/clients/sqlite.py
--rw-r--r--   0        0        0     4474 2020-02-02 00:00:00.000000 relationalai-0.1.8/src/relationalai/clients/test.py
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 relationalai-0.1.8/src/relationalai/graphs/__init__.py
--rw-r--r--   0        0        0     8238 2020-02-02 00:00:00.000000 relationalai-0.1.8/src/relationalai/graphs/lib.py
--rw-r--r--   0        0        0     2876 2020-02-02 00:00:00.000000 relationalai-0.1.8/src/relationalai/loaders/csv.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 relationalai-0.1.8/src/relationalai/tools/__init__.py
--rw-r--r--   0        0        0    21470 2020-02-02 00:00:00.000000 relationalai-0.1.8/src/relationalai/tools/cli.py
--rw-r--r--   0        0        0     5506 2020-02-02 00:00:00.000000 relationalai-0.1.8/src/relationalai/tools/cli_controls.py
--rw-r--r--   0        0        0     6145 2020-02-02 00:00:00.000000 relationalai-0.1.8/src/relationalai/tools/debugger.py
--rw-r--r--   0        0        0     8678 2020-02-02 00:00:00.000000 relationalai-0.1.8/src/relationalai/tools/dev.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 relationalai-0.1.8/tests/__init__.py
--rw-r--r--   0        0        0     1386 2020-02-02 00:00:00.000000 relationalai-0.1.8/tests/conftest.py
--rw-r--r--   0        0        0      414 2020-02-02 00:00:00.000000 relationalai-0.1.8/tests/execution/test_core.py
--rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 relationalai-0.1.8/tests/execution/test_examples.py
--rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 relationalai-0.1.8/tests/execution/basic/smoketest.py
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 relationalai-0.1.8/tests/execution/snapshots/test_core/test_basic/smoketest/query0.txt
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 relationalai-0.1.8/tests/execution/snapshots/test_examples/test_example/emit_playground/query0.txt
--rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 relationalai-0.1.8/tests/execution/snapshots/test_examples/test_example/found/query0.txt
--rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 relationalai-0.1.8/tests/execution/snapshots/test_examples/test_example/graph/query0.txt
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 relationalai-0.1.8/tests/execution/snapshots/test_examples/test_example/graph/query1.txt
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 relationalai-0.1.8/tests/execution/snapshots/test_examples/test_example/load_raw/query0.txt
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 relationalai-0.1.8/tests/execution/snapshots/test_examples/test_example/or_types/query0.txt
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 relationalai-0.1.8/tests/execution/snapshots/test_examples/test_example/simple/query0.txt
--rw-r--r--   0        0        0      327 2020-02-02 00:00:00.000000 relationalai-0.1.8/tests/execution/snapshots/test_examples/test_example/simple_recursion/query0.txt
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 relationalai-0.1.8/tests/execution/snapshots/test_examples/test_example/simple_streamlit/query0.txt
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 relationalai-0.1.8/tests/execution/snapshots/test_examples/test_example/test/query0.txt
--rw-r--r--   0        0        0     3097 2020-02-02 00:00:00.000000 relationalai-0.1.8/tests/roundtrip/test_document.py
--rw-r--r--   0        0        0     2956 2020-02-02 00:00:00.000000 relationalai-0.1.8/tests/roundtrip/test_task.py
--rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 relationalai-0.1.8/.gitignore
--rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 relationalai-0.1.8/PYPI_README.md
--rw-r--r--   0        0        0     1043 2020-02-02 00:00:00.000000 relationalai-0.1.8/pyproject.toml
--rw-r--r--   0        0        0     1188 2020-02-02 00:00:00.000000 relationalai-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0     1947 2020-02-02 00:00:00.000000 relationalai-0.1.9/CONTRIBUTING.md
+-rw-r--r--   0        0        0     2744 2020-02-02 00:00:00.000000 relationalai-0.1.9/README.md
+-rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 relationalai-0.1.9/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 relationalai-0.1.9/.github/workflows/ruff.yml
+-rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 relationalai-0.1.9/docs/README.md
+-rw-r--r--   0        0        0    16610 2020-02-02 00:00:00.000000 relationalai-0.1.9/docs/getting_started.md
+-rw-r--r--   0        0        0     9875 2020-02-02 00:00:00.000000 relationalai-0.1.9/docs/_old/OLD_pyrel_quickstart.md
+-rw-r--r--   0        0        0     3956 2020-02-02 00:00:00.000000 relationalai-0.1.9/docs/_old/metamodel.md
+-rw-r--r--   0        0        0     5935 2020-02-02 00:00:00.000000 relationalai-0.1.9/docs/_old/python_dsl.md
+-rw-r--r--   0        0        0     9371 2020-02-02 00:00:00.000000 relationalai-0.1.9/docs/_old/quickstart.md
+-rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 relationalai-0.1.9/docs/api_reference/README.md
+-rw-r--r--   0        0        0     8436 2020-02-02 00:00:00.000000 relationalai-0.1.9/docs/api_reference/cli/README.md
+-rw-r--r--   0        0        0    16584 2020-02-02 00:00:00.000000 relationalai-0.1.9/docs/api_reference/python/Aggregates.md
+-rw-r--r--   0        0        0     9333 2020-02-02 00:00:00.000000 relationalai-0.1.9/docs/api_reference/python/Context.md
+-rw-r--r--   0        0        0     9650 2020-02-02 00:00:00.000000 relationalai-0.1.9/docs/api_reference/python/ContextSelect.md
+-rw-r--r--   0        0        0     1858 2020-02-02 00:00:00.000000 relationalai-0.1.9/docs/api_reference/python/Expression.md
+-rw-r--r--   0        0        0     5046 2020-02-02 00:00:00.000000 relationalai-0.1.9/docs/api_reference/python/Instance.md
+-rw-r--r--   0        0        0     1549 2020-02-02 00:00:00.000000 relationalai-0.1.9/docs/api_reference/python/InstanceProperty.md
+-rw-r--r--   0        0        0    25616 2020-02-02 00:00:00.000000 relationalai-0.1.9/docs/api_reference/python/Model.md
+-rw-r--r--   0        0        0    23126 2020-02-02 00:00:00.000000 relationalai-0.1.9/docs/api_reference/python/Producer.md
+-rw-r--r--   0        0        0     3186 2020-02-02 00:00:00.000000 relationalai-0.1.9/docs/api_reference/python/README.md
+-rw-r--r--   0        0        0     6621 2020-02-02 00:00:00.000000 relationalai-0.1.9/docs/api_reference/python/Type.md
+-rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 relationalai-0.1.9/docs/api_reference/sql/README.md
+-rw-r--r--   0        0        0     1203 2020-02-02 00:00:00.000000 relationalai-0.1.9/examples/README.md
+-rw-r--r--   0        0        0     6135 2020-02-02 00:00:00.000000 relationalai-0.1.9/examples/SF_pagerank.ipynb
+-rw-r--r--   0        0        0      914 2020-02-02 00:00:00.000000 relationalai-0.1.9/examples/cdc.py
+-rw-r--r--   0        0        0      935 2020-02-02 00:00:00.000000 relationalai-0.1.9/examples/emit_playground.py
+-rw-r--r--   0        0        0      589 2020-02-02 00:00:00.000000 relationalai-0.1.9/examples/found.py
+-rw-r--r--   0        0        0     6699 2020-02-02 00:00:00.000000 relationalai-0.1.9/examples/fraud.ipynb
+-rw-r--r--   0        0        0     3028 2020-02-02 00:00:00.000000 relationalai-0.1.9/examples/fraud.py
+-rw-r--r--   0        0        0   698999 2020-02-02 00:00:00.000000 relationalai-0.1.9/examples/graph.ipynb
+-rw-r--r--   0        0        0     1254 2020-02-02 00:00:00.000000 relationalai-0.1.9/examples/graph.py
+-rw-r--r--   0        0        0     3654 2020-02-02 00:00:00.000000 relationalai-0.1.9/examples/graphlib.py
+-rw-r--r--   0        0        0      312 2020-02-02 00:00:00.000000 relationalai-0.1.9/examples/load_raw.py
+-rw-r--r--   0        0        0      627 2020-02-02 00:00:00.000000 relationalai-0.1.9/examples/or_types.py
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 relationalai-0.1.9/examples/requirements.txt
+-rw-r--r--   0        0        0      480 2020-02-02 00:00:00.000000 relationalai-0.1.9/examples/simple.py
+-rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 relationalai-0.1.9/examples/simple_recursion.py
+-rw-r--r--   0        0        0      722 2020-02-02 00:00:00.000000 relationalai-0.1.9/examples/simple_streamlit.py
+-rw-r--r--   0        0        0     2802 2020-02-02 00:00:00.000000 relationalai-0.1.9/examples/snowflake_pagerank.py
+-rw-r--r--   0        0        0     2403 2020-02-02 00:00:00.000000 relationalai-0.1.9/examples/solver.py
+-rw-r--r--   0        0        0     4740 2020-02-02 00:00:00.000000 relationalai-0.1.9/examples/data/people.csv
+-rw-r--r--   0        0        0    10518 2020-02-02 00:00:00.000000 relationalai-0.1.9/examples/data/transactions.csv
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 relationalai-0.1.9/examples/rel/bar.rel
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 relationalai-0.1.9/examples/rel/foo.rel
+-rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 relationalai-0.1.9/examples/rel/solver.rel
+-rw-r--r--   0        0        0     3709 2020-02-02 00:00:00.000000 relationalai-0.1.9/src/gentest/README.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 relationalai-0.1.9/src/gentest/__init__.py
+-rw-r--r--   0        0        0    12342 2020-02-02 00:00:00.000000 relationalai-0.1.9/src/gentest/emit.py
+-rw-r--r--   0        0        0     1301 2020-02-02 00:00:00.000000 relationalai-0.1.9/src/gentest/exec.py
+-rw-r--r--   0        0        0      792 2020-02-02 00:00:00.000000 relationalai-0.1.9/src/gentest/fixtures.py
+-rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 relationalai-0.1.9/src/gentest/patch.py
+-rw-r--r--   0        0        0     7629 2020-02-02 00:00:00.000000 relationalai-0.1.9/src/gentest/util.py
+-rwxr-xr-x   0        0        0     3521 2020-02-02 00:00:00.000000 relationalai-0.1.9/src/gentest/cli/__main__.py
+-rw-r--r--   0        0        0     1299 2020-02-02 00:00:00.000000 relationalai-0.1.9/src/gentest/cli/collect_failures.py
+-rw-r--r--   0        0        0     1331 2020-02-02 00:00:00.000000 relationalai-0.1.9/src/gentest/cli/collect_tests.py
+-rw-r--r--   0        0        0     5707 2020-02-02 00:00:00.000000 relationalai-0.1.9/src/gentest/cli/repro.py
+-rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 relationalai-0.1.9/src/gentest/cli/run_tests.py
+-rw-r--r--   0        0        0    15710 2020-02-02 00:00:00.000000 relationalai-0.1.9/src/gentest/cli/watch.py
+-rw-r--r--   0        0        0     3232 2020-02-02 00:00:00.000000 relationalai-0.1.9/src/gentest/gen/action.py
+-rw-r--r--   0        0        0     5461 2020-02-02 00:00:00.000000 relationalai-0.1.9/src/gentest/gen/context.py
+-rw-r--r--   0        0        0     1610 2020-02-02 00:00:00.000000 relationalai-0.1.9/src/gentest/gen/document.py
+-rw-r--r--   0        0        0      442 2020-02-02 00:00:00.000000 relationalai-0.1.9/src/gentest/gen/error.py
+-rw-r--r--   0        0        0     6095 2020-02-02 00:00:00.000000 relationalai-0.1.9/src/gentest/gen/group_limited.py
+-rw-r--r--   0        0        0     4662 2020-02-02 00:00:00.000000 relationalai-0.1.9/src/gentest/gen/ir.py
+-rw-r--r--   0        0        0    17029 2020-02-02 00:00:00.000000 relationalai-0.1.9/src/gentest/gen/scope.py
+-rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 relationalai-0.1.9/src/gentest/gen/staged.py
+-rw-r--r--   0        0        0     2888 2020-02-02 00:00:00.000000 relationalai-0.1.9/src/gentest/gen/task.py
+-rw-r--r--   0        0        0     2204 2020-02-02 00:00:00.000000 relationalai-0.1.9/src/gentest/gen/test.py
+-rw-r--r--   0        0        0     2863 2020-02-02 00:00:00.000000 relationalai-0.1.9/src/gentest/harness/database.py
+-rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 relationalai-0.1.9/src/gentest/harness/vendor_types.py
+-rw-r--r--   0        0        0     1709 2020-02-02 00:00:00.000000 relationalai-0.1.9/src/gentest/validate/diff.py
+-rw-r--r--   0        0        0     5588 2020-02-02 00:00:00.000000 relationalai-0.1.9/src/gentest/validate/errors.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 relationalai-0.1.9/src/gentest/validate/mapping.py
+-rw-r--r--   0        0        0     5374 2020-02-02 00:00:00.000000 relationalai-0.1.9/src/gentest/validate/roundtrip.py
+-rw-r--r--   0        0        0     1284 2020-02-02 00:00:00.000000 relationalai-0.1.9/src/relationalai/__init__.py
+-rw-r--r--   0        0        0     5906 2020-02-02 00:00:00.000000 relationalai-0.1.9/src/relationalai/compiler.py
+-rw-r--r--   0        0        0     7274 2020-02-02 00:00:00.000000 relationalai-0.1.9/src/relationalai/debugging.py
+-rw-r--r--   0        0        0    35221 2020-02-02 00:00:00.000000 relationalai-0.1.9/src/relationalai/dsl.py
+-rw-r--r--   0        0        0     8992 2020-02-02 00:00:00.000000 relationalai-0.1.9/src/relationalai/errors.py
+-rw-r--r--   0        0        0    26388 2020-02-02 00:00:00.000000 relationalai-0.1.9/src/relationalai/metagen.py
+-rw-r--r--   0        0        0    23175 2020-02-02 00:00:00.000000 relationalai-0.1.9/src/relationalai/metamodel.py
+-rw-r--r--   0        0        0    27114 2020-02-02 00:00:00.000000 relationalai-0.1.9/src/relationalai/rel.py
+-rw-r--r--   0        0        0      914 2020-02-02 00:00:00.000000 relationalai-0.1.9/src/relationalai/analysis/whynot.py
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 relationalai-0.1.9/src/relationalai/clients/__init__.py
+-rw-r--r--   0        0        0     6468 2020-02-02 00:00:00.000000 relationalai-0.1.9/src/relationalai/clients/azure.py
+-rw-r--r--   0        0        0     8153 2020-02-02 00:00:00.000000 relationalai-0.1.9/src/relationalai/clients/client.py
+-rw-r--r--   0        0        0     4275 2020-02-02 00:00:00.000000 relationalai-0.1.9/src/relationalai/clients/config.py
+-rw-r--r--   0        0        0    26254 2020-02-02 00:00:00.000000 relationalai-0.1.9/src/relationalai/clients/snowflake.py
+-rw-r--r--   0        0        0    10405 2020-02-02 00:00:00.000000 relationalai-0.1.9/src/relationalai/clients/sqlite.py
+-rw-r--r--   0        0        0     4474 2020-02-02 00:00:00.000000 relationalai-0.1.9/src/relationalai/clients/test.py
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 relationalai-0.1.9/src/relationalai/graphs/__init__.py
+-rw-r--r--   0        0        0    10435 2020-02-02 00:00:00.000000 relationalai-0.1.9/src/relationalai/graphs/lib.py
+-rw-r--r--   0        0        0     2876 2020-02-02 00:00:00.000000 relationalai-0.1.9/src/relationalai/loaders/csv.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 relationalai-0.1.9/src/relationalai/tools/__init__.py
+-rw-r--r--   0        0        0    21470 2020-02-02 00:00:00.000000 relationalai-0.1.9/src/relationalai/tools/cli.py
+-rw-r--r--   0        0        0     5506 2020-02-02 00:00:00.000000 relationalai-0.1.9/src/relationalai/tools/cli_controls.py
+-rw-r--r--   0        0        0     6145 2020-02-02 00:00:00.000000 relationalai-0.1.9/src/relationalai/tools/debugger.py
+-rw-r--r--   0        0        0     8737 2020-02-02 00:00:00.000000 relationalai-0.1.9/src/relationalai/tools/dev.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 relationalai-0.1.9/tests/__init__.py
+-rw-r--r--   0        0        0     1386 2020-02-02 00:00:00.000000 relationalai-0.1.9/tests/conftest.py
+-rw-r--r--   0        0        0      414 2020-02-02 00:00:00.000000 relationalai-0.1.9/tests/execution/test_core.py
+-rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 relationalai-0.1.9/tests/execution/test_examples.py
+-rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 relationalai-0.1.9/tests/execution/basic/smoketest.py
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 relationalai-0.1.9/tests/execution/snapshots/test_core/test_basic/smoketest/query0.txt
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 relationalai-0.1.9/tests/execution/snapshots/test_examples/test_example/emit_playground/query0.txt
+-rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 relationalai-0.1.9/tests/execution/snapshots/test_examples/test_example/found/query0.txt
+-rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 relationalai-0.1.9/tests/execution/snapshots/test_examples/test_example/graph/query0.txt
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 relationalai-0.1.9/tests/execution/snapshots/test_examples/test_example/graph/query1.txt
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 relationalai-0.1.9/tests/execution/snapshots/test_examples/test_example/load_raw/query0.txt
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 relationalai-0.1.9/tests/execution/snapshots/test_examples/test_example/or_types/query0.txt
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 relationalai-0.1.9/tests/execution/snapshots/test_examples/test_example/simple/query0.txt
+-rw-r--r--   0        0        0      327 2020-02-02 00:00:00.000000 relationalai-0.1.9/tests/execution/snapshots/test_examples/test_example/simple_recursion/query0.txt
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 relationalai-0.1.9/tests/execution/snapshots/test_examples/test_example/simple_streamlit/query0.txt
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 relationalai-0.1.9/tests/execution/snapshots/test_examples/test_example/test/query0.txt
+-rw-r--r--   0        0        0     3097 2020-02-02 00:00:00.000000 relationalai-0.1.9/tests/roundtrip/test_document.py
+-rw-r--r--   0        0        0     2956 2020-02-02 00:00:00.000000 relationalai-0.1.9/tests/roundtrip/test_task.py
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 relationalai-0.1.9/.gitignore
+-rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 relationalai-0.1.9/PYPI_README.md
+-rw-r--r--   0        0        0     1043 2020-02-02 00:00:00.000000 relationalai-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0     1188 2020-02-02 00:00:00.000000 relationalai-0.1.9/PKG-INFO
```

### Comparing `relationalai-0.1.8/CONTRIBUTING.md` & `relationalai-0.1.9/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.1.8/README.md` & `relationalai-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.1.8/.github/workflows/publish-to-pypi.yml` & `relationalai-0.1.9/.github/workflows/publish-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `relationalai-0.1.8/.github/workflows/ruff.yml` & `relationalai-0.1.9/.github/workflows/ruff.yml`

 * *Files identical despite different names*

### Comparing `relationalai-0.1.8/docs/getting_started.md` & `relationalai-0.1.9/docs/getting_started.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Getting Started With RelationalAI
 
 Ready to dive into RelationalAI?
 This document will quickly get you up and running.
 
 ## Install The `relationalai` Python Package
 
-First, install the `relationalai-python` package with `pip`:
+First, install the `relationalai` package with `pip`:
 
 > [!IMPORTANT]
 > RelationalAI is compatible with Python version 3.11 (recommended) and 3.10.
 > Python 3.12 is currently not supported.
 > Visit [https://www.python.org/downloads/](https://www.python.org/downloads/)
 > to download a compatible version of Python.
```

### Comparing `relationalai-0.1.8/docs/_old/OLD_pyrel_quickstart.md` & `relationalai-0.1.9/docs/_old/OLD_pyrel_quickstart.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.1.8/docs/_old/metamodel.md` & `relationalai-0.1.9/docs/_old/metamodel.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.1.8/docs/_old/python_dsl.md` & `relationalai-0.1.9/docs/_old/python_dsl.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.1.8/docs/_old/quickstart.md` & `relationalai-0.1.9/docs/_old/quickstart.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.1.8/docs/api_reference/cli/README.md` & `relationalai-0.1.9/docs/api_reference/cli/README.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.1.8/docs/api_reference/python/Aggregates.md` & `relationalai-0.1.9/docs/api_reference/python/Aggregates.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.1.8/docs/api_reference/python/Context.md` & `relationalai-0.1.9/docs/api_reference/python/Context.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.1.8/docs/api_reference/python/ContextSelect.md` & `relationalai-0.1.9/docs/api_reference/python/ContextSelect.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.1.8/docs/api_reference/python/Expression.md` & `relationalai-0.1.9/docs/api_reference/python/Expression.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.1.8/docs/api_reference/python/Instance.md` & `relationalai-0.1.9/docs/api_reference/python/Instance.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.1.8/docs/api_reference/python/InstanceProperty.md` & `relationalai-0.1.9/docs/api_reference/python/InstanceProperty.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.1.8/docs/api_reference/python/Model.md` & `relationalai-0.1.9/docs/api_reference/python/Model.md`

 * *Files 8% similar despite different names*

```diff
@@ -259,15 +259,15 @@
 ### `model.not_found()`
 
 ```python
 Model.not_found(dynamic: bool = False) -> Context
 ```
 
 Creates a [`Context`](./Context.md) that restricts [producers](./Producer.md) in a [rule](#modelrule) or [query](#modelquery)
-to only those values for which none of the conditions in the `.not_found()` context hold.
+to only those values for which any of the conditions in the `.not_found()` context fail.
 
 #### Parameters
 
 | Name | Type | Description |
 | :--- | :--- | :------ |
 | `dynamic` | `bool` | Whether or not the context is dynamic. Dynamic queries support Python control flow as macros. See [`Context`](./Context.md) for more information. |
 
@@ -799,43 +799,77 @@
 `Model.union()` is a [context manager](https://docs.python.org/3/glossary.html#term-context-manager)
 and should be called in a `with` statement.
 It must be called from within a [rule](#modelrule) or [query](#modelquery) context:
 
 ```python
 import relationalai as rai
 
-model = rai.Model("students")
-Student = model.Type("Student")
+model = rai.Model("people")
+Person = model.Type("Person")
 
 with model.rule():
-    Student.add(name="Fred", grade=87)
-    Student.add(name="Johnny", grade=65)
-    Student.add(name="Mary", grade=98)
+    Person.add(name="Alice", age=10)
+    Person.add(name="Bob", age=30)
+    Person.add(name="Carol", age=60)
 
 # `model.union()` is always called in a nested `with` block
 # inside of a `model.rule()` or `model.query()` context.
 with model.query() as select:
-    # Get students with a grade greater than 90 or less than 70.
-    student = Student()
-    with model.union() as students:
-        # Only `with` statements are allowed inside of a `Model.union()` context.
-        with student.grade > 90:
+    person = Person()
+    with model.union() as seniors_and_kids:
+        # Only `with` statements are allowed directly inside of a `Model.union()` context.
+        with person.age >= 60:
             # A `with` block may contain any valid query builder code.
-            students.add(student, note="Outstanding student")
-        with student.grade < 70:
-            students.add(student, note="Failing student")
-    response = select(students.name, students.grade, students.note)
+            seniors_and_kids.add(person)
+        with person.age < 13:
+            seniors_and_kids.add(person)
+    response = select(seniors_and_kids.name)
+
+print(response.results)
+# Output:
+#     name
+# 0  Alice
+# 1  Carol
+```
+
+Here, `seniors_and_kids` is a [`ContextSelect`](./ContextSelect.md) object returned by
+the `model.union()` context's `.__enter__()` method when the `with` statement is executed.
+It behaves similar to a [`Type`](./Type.md) in the sense that
+`seniors_and_kids` is a collection of objects and has an `.add()` method used to add objects to the collection.
+Unlike a `Type`, however, `seniors_and_kids` may only have existing objects added to it.
+Moreover, the fact that an object is in `seniors_and_kids` is only retained for the lifetime of the query.
+
+You can use `seniors_and_kids` outside of the `model.union()` block that created it.
+Accessing a property from `seniors_and_kids` returns an [`InstanceProperty`](./InstanceProperty.md) object that
+produces the property values of the objects in the `seniors_and_kids` collection.
+
+You may also add collection-specific properties to objects when they are added to `seniors_and_kids`.
+For instance, the following modified query adds a note to each object in the `seniors_and_kids` collection:
+
+```python
+with model.query() as select:
+    person = Person()
+    with model.union() as seniors_and_kids:
+        with person.age >= 60:
+            seniors_and_kids.add(person, note="senior")
+        with person.age < 13:
+            seniors_and_kids.add(person, note="kid")
+    response = select(seniors_and_kids.name, seniors_and_kids.note)
 
 print(response.results)
 # Output:
-#      name  grade                    v
-# 0  Johnny     65      Failing student
-# 1    Mary     98  Outstanding student
+#     name       v
+# 0  Alice     kid
+# 1  Carol  senior
 ```
 
+The `note` property is only accessible from the `seniors_and_kids` object.
+Trying to access `person.note` property on `person` will fail,
+unless there is already a `note` property for `person` objects.
+
 ### `Model.Vars()`
 
 ```python
 Model.Vars(count: int) -> List[Instance]
 ```
 
 Creates `count` number of [`Instance`](./Instance.md) objects that represent unknown values
```

### Comparing `relationalai-0.1.8/docs/api_reference/python/Producer.md` & `relationalai-0.1.9/docs/api_reference/python/Producer.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.1.8/docs/api_reference/python/README.md` & `relationalai-0.1.9/docs/api_reference/python/README.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.1.8/docs/api_reference/python/Type.md` & `relationalai-0.1.9/docs/api_reference/python/Type.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.1.8/examples/README.md` & `relationalai-0.1.9/examples/README.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.1.8/examples/SF_pagerank.ipynb` & `relationalai-0.1.9/examples/SF_pagerank.ipynb`

 * *Files 10% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9990483164369979%*

 * *Differences: {"'cells'": "{8: {'source': {insert: [(4, 'nodes.extend(Account, name=Account.name)\\n'), (5, "*

 * *            '\'nodes.extend(Person, kind="person")\\n\'), (6, \'nodes.extend(Merchant, '*

 * *            'kind="merchant", label=Merchant.name)\\n\'), (8, \'# add edges for '*

 * *            "transactions\\n'), (11, '    edges.add(t.from_, t.to, amount=t.amount)')], delete: "*

 * *            "[11, 8, 6, 5, 4]}}, 10: {'source': {insert: [(3, '    nodes.add(m, rank=rank)\\n')], "*

 * *            "delete: [3]}}, 12: {'source': {ins […]*

```diff
@@ -109,22 +109,22 @@
             "metadata": {},
             "outputs": [],
             "source": [
                 "graph = Graph(model)\n",
                 "nodes, edges = graph.nodes, graph.edges\n",
                 "\n",
                 "# add some nodes\n",
-                "nodes.extend(Account, hover=Account.name)\n",
-                "nodes.extend(Person, color=\"#bbb\")\n",
-                "nodes.extend(Merchant, color=\"green\", label=Merchant.name)\n",
+                "nodes.extend(Account, name=Account.name)\n",
+                "nodes.extend(Person, kind=\"person\")\n",
+                "nodes.extend(Merchant, kind=\"merchant\", label=Merchant.name)\n",
                 "\n",
-                "# add transaction edges\n",
+                "# add edges for transactions\n",
                 "with model.rule():\n",
                 "    t = Transaction()\n",
-                "    edges.add(t.from_, t.to, size=t.amount / 50, color=\"#ccc\", opacity=0.3)"
+                "    edges.add(t.from_, t.to, amount=t.amount)"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "a4694972-4208-45f1-b7ab-999632c98509",
             "metadata": {},
             "source": [
@@ -137,15 +137,15 @@
             "id": "6394e745-e1ee-4557-a95d-29112989ff83",
             "metadata": {},
             "outputs": [],
             "source": [
                 "with model.rule():\n",
                 "    m = Merchant()\n",
                 "    rank = graph.compute.pagerank(m)\n",
-                "    nodes.add(m, size=((rank * 100) ** 2.2) + 10, rank=rank)\n",
+                "    nodes.add(m, rank=rank)\n",
                 "    m.set(rank=rank)"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "73859cc7-da3d-4593-b7be-fd93bed890e9",
             "metadata": {},
@@ -164,14 +164,26 @@
             "source": [
                 "graph.visualize(\n",
                 "    three=True,\n",
                 "    node_label_size_factor=1.2,\n",
                 "    use_links_force=True,\n",
                 "    links_force_distance=140,\n",
                 "    node_hover_neighborhood=True,\n",
+                "    style={\n",
+                "        \"node\": {\n",
+                "            \"size\": lambda n: (n.get(\"rank\", 0.01) * 100) ** 2.2 + 10,\n",
+                "            \"color\": lambda n: \"green\" if n[\"kind\"] == \"merchant\" else \"#bbb\",\n",
+                "            \"hover\": lambda n: f'{n[\"name\"]} ({n.get(\"rank\", 0):,.3f})' if n.get(\"rank\") else n[\"name\"]\n",
+                "        },\n",
+                "        \"edge\": {\n",
+                "            \"opacity\": 0.3,\n",
+                "            \"color\": \"#ccc\",\n",
+                "            \"size\": lambda t: t[\"amount\"] / 50\n",
+                "        }\n",
+                "    }\n",
                 ")"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "36ae137f-49d7-4c62-b759-cb969c51d36e",
             "metadata": {},
```

### Comparing `relationalai-0.1.8/examples/cdc.py` & `relationalai-0.1.9/examples/cdc.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.1.8/examples/emit_playground.py` & `relationalai-0.1.9/examples/emit_playground.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.1.8/examples/found.py` & `relationalai-0.1.9/examples/found.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.1.8/examples/fraud.ipynb` & `relationalai-0.1.9/examples/fraud.ipynb`

 * *Files identical despite different names*

### Comparing `relationalai-0.1.8/examples/fraud.py` & `relationalai-0.1.9/examples/fraud.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.1.8/examples/graph.ipynb` & `relationalai-0.1.9/examples/graph.ipynb`

 * *Files identical despite different names*

### Comparing `relationalai-0.1.8/examples/graph.py` & `relationalai-0.1.9/examples/graph.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.1.8/examples/graphlib.py` & `relationalai-0.1.9/examples/graphlib.py`

 * *Files 10% similar despite different names*

```diff
@@ -38,26 +38,26 @@
 #--------------------------------------------------
 
 graph = Graph(model)
 nodes, edges = graph.nodes, graph.edges
 sum = model.aggregates.sum
 
 nodes.extend(Person, label=Person.name)
-nodes.extend(Criminal, color="red")
+nodes.extend(Criminal, criminal=True)
 edges.extend(Person.knows, label="knows")
 
 with model.rule():
     t = Transaction()
     weight = sum(t, t.amount, per=[t.from_, t.to])
-    edges.add(t.from_, t.to, label="Transfer", size=weight / 120, color="red")
+    edges.add(t.from_, t.to, label="Transfer", weight=weight)
 
 with model.rule():
     p = Person()
-    degree = graph.compute.degree(p)
-    nodes.add(p, size=degree * 5)
+    rank = graph.compute.pagerank(p)
+    nodes.add(p, rank=rank * 5)
 
 #--------------------------------------------------
 # Paths
 #--------------------------------------------------
 
 # Transfer = Edge(Transaction, Transaction.from_, Transaction.to)
 # Teller = Edge(Transaction, Transaction.from_, Transaction.teller)
@@ -113,8 +113,16 @@
 
 #--------------------------------------------------
 # Go
 #--------------------------------------------------
 
 data = graph.fetch()
 rich.print(data)
-# graph.visualize().display()
+graph.visualize(three=True, style={
+    "node": {
+        "color": lambda x: "red" if x.get("criminal") else "blue",
+        "size": lambda x: (x["rank"] * 2) ** 2
+    },
+    "edge": {
+        "color": "yellow",
+    }
+}).display()
```

### Comparing `relationalai-0.1.8/examples/or_types.py` & `relationalai-0.1.9/examples/or_types.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.1.8/examples/simple_recursion.py` & `relationalai-0.1.9/examples/simple_recursion.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.1.8/examples/simple_streamlit.py` & `relationalai-0.1.9/examples/simple_streamlit.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.1.8/examples/snowflake_pagerank.py` & `relationalai-0.1.9/examples/snowflake_pagerank.py`

 * *Files 23% similar despite different names*

```diff
@@ -41,38 +41,50 @@
 #--------------------------------------------------
 # Create a graph
 #--------------------------------------------------
 
 graph = Graph(model)
 nodes, edges = graph.nodes, graph.edges
 
-nodes.extend(Account, hover=Account.name)
-nodes.extend(Person, color="#bbb")
-nodes.extend(Merchant, color="green", label=Merchant.name)
+nodes.extend(Account, name=Account.name)
+nodes.extend(Person, kind="person")
+nodes.extend(Merchant, kind="merchant", label=Merchant.name)
 
 with model.rule():
     t = Transaction()
-    edges.add(t.from_, t.to, size=t.amount / 50, color="#ccc", opacity=0.3)
+    edges.add(t.from_, t.to, amount=t.amount)
 
 with model.rule():
     m = Merchant()
     rank = graph.compute.pagerank(m)
-    nodes.add(m, size=((rank * 100) ** 2.2) + 10, rank=rank)
+    nodes.add(m, rank=rank)
     m.set(rank=rank)
 
 #--------------------------------------------------
 # Visualize the graph
 #--------------------------------------------------
 
 graph.visualize(
     three=True,
     node_label_size_factor=1.2,
     use_links_force=True,
     links_force_distance=140,
     node_hover_neighborhood=True,
+    style={
+        "node": {
+            "size": lambda n: (n.get("rank", 0.01) * 100) ** 2.2 + 10,
+            "color": lambda n: "green" if n["kind"] == "merchant" else "#bbb",
+            "hover": lambda n: f'{n["name"]} ({n.get("rank", 0):,.3f})' if n.get("rank") else n["name"]
+        },
+        "edge": {
+            "opacity": 0.3,
+            "color": "#ccc",
+            "size": lambda t: t["amount"] / 50
+        }
+    }
 ).display()
 
 #--------------------------------------------------
 # Export the analysis
 #--------------------------------------------------
 
 @model.export("sandbox.public")
```

### Comparing `relationalai-0.1.8/examples/solver.py` & `relationalai-0.1.9/examples/solver.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.1.8/examples/data/people.csv` & `relationalai-0.1.9/examples/data/people.csv`

 * *Files identical despite different names*

### Comparing `relationalai-0.1.8/examples/data/transactions.csv` & `relationalai-0.1.9/examples/data/transactions.csv`

 * *Files identical despite different names*

### Comparing `relationalai-0.1.8/examples/rel/solver.rel` & `relationalai-0.1.9/examples/rel/solver.rel`

 * *Files identical despite different names*

### Comparing `relationalai-0.1.8/src/gentest/README.md` & `relationalai-0.1.9/src/gentest/README.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.1.8/src/gentest/emit.py` & `relationalai-0.1.9/src/gentest/emit.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.1.8/src/gentest/exec.py` & `relationalai-0.1.9/src/gentest/exec.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.1.8/src/gentest/fixtures.py` & `relationalai-0.1.9/src/gentest/fixtures.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.1.8/src/gentest/patch.py` & `relationalai-0.1.9/src/gentest/patch.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.1.8/src/gentest/util.py` & `relationalai-0.1.9/src/gentest/util.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.1.8/src/gentest/cli/__main__.py` & `relationalai-0.1.9/src/gentest/cli/__main__.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.1.8/src/gentest/cli/collect_failures.py` & `relationalai-0.1.9/src/gentest/cli/collect_failures.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.1.8/src/gentest/cli/collect_tests.py` & `relationalai-0.1.9/src/gentest/cli/collect_tests.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.1.8/src/gentest/cli/repro.py` & `relationalai-0.1.9/src/gentest/cli/repro.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.1.8/src/gentest/cli/watch.py` & `relationalai-0.1.9/src/gentest/cli/watch.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.1.8/src/gentest/gen/action.py` & `relationalai-0.1.9/src/gentest/gen/action.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.1.8/src/gentest/gen/context.py` & `relationalai-0.1.9/src/gentest/gen/context.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.1.8/src/gentest/gen/document.py` & `relationalai-0.1.9/src/gentest/gen/document.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.1.8/src/gentest/gen/group_limited.py` & `relationalai-0.1.9/src/gentest/gen/group_limited.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.1.8/src/gentest/gen/ir.py` & `relationalai-0.1.9/src/gentest/gen/ir.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.1.8/src/gentest/gen/scope.py` & `relationalai-0.1.9/src/gentest/gen/scope.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.1.8/src/gentest/gen/task.py` & `relationalai-0.1.9/src/gentest/gen/task.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.1.8/src/gentest/gen/test.py` & `relationalai-0.1.9/src/gentest/gen/test.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.1.8/src/gentest/harness/database.py` & `relationalai-0.1.9/src/gentest/harness/database.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.1.8/src/gentest/validate/diff.py` & `relationalai-0.1.9/src/gentest/validate/diff.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.1.8/src/gentest/validate/errors.py` & `relationalai-0.1.9/src/gentest/validate/errors.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.1.8/src/gentest/validate/mapping.py` & `relationalai-0.1.9/src/gentest/validate/mapping.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.1.8/src/gentest/validate/roundtrip.py` & `relationalai-0.1.9/src/gentest/validate/roundtrip.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.1.8/src/relationalai/__init__.py` & `relationalai-0.1.9/src/relationalai/__init__.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.1.8/src/relationalai/compiler.py` & `relationalai-0.1.9/src/relationalai/compiler.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.1.8/src/relationalai/debugging.py` & `relationalai-0.1.9/src/relationalai/debugging.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.1.8/src/relationalai/dsl.py` & `relationalai-0.1.9/src/relationalai/dsl.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from enum import Enum
 import inspect
 from itertools import zip_longest
 import typing
-from typing import Any, Dict, List, Optional, get_type_hints
+from typing import Any, Dict, List, Optional, Tuple, get_type_hints
 import numbers
 import os
 import datetime
 import hashlib
 
 from pandas import DataFrame
 
@@ -19,14 +19,16 @@
 #--------------------------------------------------
 # Helpers
 #--------------------------------------------------
 
 def to_var(x:Any):
     if isinstance(x, Var):
         return x
+    if getattr(x, "_to_var", None):
+        return to_var(x._to_var())
     if isinstance(x, ContextSelect):
         return x._vars[0]
     if isinstance(x, mProperty):
         return Var(value=x)
     if isinstance(x, mType):
         return Var(value=x)
     if isinstance(x, Producer):
@@ -36,16 +38,14 @@
         return Var(Builtins.Any, value=[to_var(i) for i in x])
     if isinstance(x, str):
         return Var(Builtins.String, None, x)
     if isinstance(x, numbers.Number):
         return Var(Builtins.Number, None, x)
     if isinstance(x, datetime.datetime) or isinstance(x, datetime.date):
         return Var(value=x)
-    if getattr(x, "_to_var", None):
-        return to_var(x._to_var())
     raise Exception(f"Unknown type: {type(x)}\n{x}")
 
 build = Builder(to_var)
 
 def to_list(x:Any):
     if isinstance(x, list):
         return x
@@ -563,14 +563,19 @@
         return RelationNS(self._graph, ns, name)
 
     def add(self, *args):
         name = ":".join([*self._ns, self._name])
         op = build.relation(name, len(args))
         self._graph._action(build.relation_action(ActionType.Bind, op, list(args)))
 
+    def _to_var(self):
+        name = ":".join([*self._ns, self._name])
+        rel = build.relation(name, 0)
+        return Var(Builtins.Relation, value=rel)
+
 #--------------------------------------------------
 # RawRelation
 #--------------------------------------------------
 
 class RawRelation(Producer):
     def __init__(self, graph:'Graph', name:str, arity:int):
         super().__init__(graph, ["add"])
@@ -583,14 +588,49 @@
 
     def add(self, *args):
         self._graph._action(build.relation_action(ActionType.Bind, self._type, list(args)))
 
     def _make_sub(self, name: str, existing=None):
         return existing
 
+    def _to_var(self):
+        return Var(Builtins.Relation, value=self._type)
+
+#--------------------------------------------------
+# InlineRelation
+#--------------------------------------------------
+
+class InlineRelation():
+    def __init__(self, graph:'Graph', data:List[Tuple]):
+        self._var = Var()
+        self._graph = graph
+        cols = [[] for _ in range(len(data[0]))]
+        for row in data:
+            for i, val in enumerate(row):
+                cols[i].append(to_var(val))
+
+        params = [Var(value=col) for col in cols]
+        params.append(self._var)
+        q = build.relation_action(ActionType.Get, Builtins.InlineRawData, params)
+        self._graph._action(q)
+
+    def _to_var(self):
+        return self._var
+
+#--------------------------------------------------
+# Symbol
+#--------------------------------------------------
+
+class Symbol():
+    def __init__(self, name:str):
+        self._var = Var(Builtins.Symbol, value=name)
+
+    def _to_var(self):
+        return self._var
+
 #--------------------------------------------------
 # RelationRef
 #--------------------------------------------------
 
 class RelationRef(Producer):
     def __init__(self, graph:'Graph', rel:Task|mType, args:List[Var]):
         super().__init__(graph, [])
```

### Comparing `relationalai-0.1.8/src/relationalai/errors.py` & `relationalai-0.1.9/src/relationalai/errors.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.1.8/src/relationalai/metagen.py` & `relationalai-0.1.9/src/relationalai/metagen.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.1.8/src/relationalai/metamodel.py` & `relationalai-0.1.9/src/relationalai/metamodel.py`

 * *Files 4% similar despite different names*

```diff
@@ -214,21 +214,27 @@
         if not seen:
             seen = set()
         if self in seen:
             return requires, provides
 
         seen.add(self)
         if isinstance(self.entity.value, Task) and len(self.entity.value.items):
+            sub_requires = set()
+            sub_provides = set()
             for i in self.entity.value.items:
                 r, p = i.requires_provides(seen)
-                requires.update(r)
-                provides.update(p)
+                sub_requires.update(r)
+                sub_provides.update(p)
+            requires.update(sub_requires - sub_provides)
 
         if self.action == ActionType.Get and self.entity.value is None:
-            provides.add(self.entity)
+            if len(self.types):
+                provides.add(self.entity)
+            else:
+                requires.add(self.entity)
         elif self.action != ActionType.Call and self.entity.value is None:
             requires.add(self.entity)
 
         for k,var in self.bindings.items():
             into = provides
             if self.action == ActionType.Bind:
                 into = requires
@@ -278,21 +284,23 @@
         self.Any = Type("Any")
         self.String = Type("String", parents=[self.Primitive])
         self.Number = Type("Number", parents=[self.Primitive])
         self.Int = Type("Int", parents=[self.Number])
         self.Decimal = Type("Decimal", parents=[self.Number])
         self.Bool = Type("Bool", parents=[self.Primitive])
         self.Type = Type("Type", parents=[self.Primitive])
+        self.Symbol = Type("Type", parents=[self.Primitive])
         self.Relation = Type("Relation", parents=[self.Primitive], properties=[Property(f"v{id}", self.Any) for i in range(1000)])
         self.Anonymous = Type("Anonymous") # A thing we assume to exist in the host DB for which we don't have information.
         self.Task = Type("Task", parents=[self.Type, self.Relation])
         Task._task_builtin = self.Task
         self.Return = Type("Return", parents=[self.Relation], properties=[Property(f"v{id}", self.Any) for i in range(20)])
         self.RawCode = Type("RawCode", properties=[Property("code", self.String)])
         self.RawData = Type("RawData", parents=[self.Relation])
+        self.InlineRawData = Type("RawData", parents=[self.RawData])
         self.Aggregate = Type("Aggregate", parents=[self.Task])
         self.Extender = Type("Extender", parents=[self.Aggregate])
         self.Quantifier = Type("Quantifier", parents=[self.Task])
         self.Not = Task("Not", parents=[self.Quantifier], properties=[Property("group", self.Any, True), Property("task", self.Task, True)])
         self.Exists = Task("Exists", parents=[self.Quantifier], properties=[Property("group", self.Any, True), Property("task", self.Task, True)])
         self.Every = Task("Every", parents=[self.Quantifier], properties=[Property("group", self.Any, True), Property("task", self.Task, True)])
 
@@ -553,37 +561,49 @@
         return final
 
 
 #--------------------------------------------------
 # Utils
 #--------------------------------------------------
 
+def _graph_debug(actions, in_degree):
+    rich.print("\n[yellow bold]STRATIFY CHECK")
+    for item in actions:
+        print("-------------------------------------------")
+        print(in_degree.get(item, 0), item)
+        (requires, provides) = item.requires_provides()
+        rich.print("    in:", ", ".join([str(r.id) for r in requires]))
+        rich.print("    out:", ", ".join([str(p.id) for p in provides]))
+
 class Utils:
 
     @staticmethod
     def action_graph(actions:List[Action]):
         graph:Dict[Action, List[Action]] = defaultdict(list)
         in_degree:Dict[Action, int] = defaultdict(int)
         vars_provided_by:Dict[Var, List[Action]] = defaultdict(list)
         vars_required_by:Dict[Var, List[Action]] = defaultdict(list)
 
+
         for item in actions:
             (requires, provides) = item.requires_provides()
             for var in provides:
                 vars_provided_by[var].append(item)
             for var in requires:
                 vars_required_by[var].append(item)
 
         for var, requirers in vars_required_by.items():
             providers = vars_provided_by.get(var, [])
             for r in requirers:
                 for provider in providers:
                     graph[provider].append(r)
                     in_degree[r] += 1
 
+        # _graph_debug(actions, in_degree)
+
         return graph, in_degree
 
     #--------------------------------------------------
     # Stratify
     #--------------------------------------------------
 
     @staticmethod
```

### Comparing `relationalai-0.1.8/src/relationalai/rel.py` & `relationalai-0.1.9/src/relationalai/rel.py`

 * *Files 1% similar despite different names*

```diff
@@ -449,20 +449,22 @@
 
 class Emitter(c.Emitter):
 
     def __init__(self):
         super().__init__()
         self.namer = Namer()
         self.stack:List[Set[Var]] = []
+        self.mapped = {}
 
     #--------------------------------------------------
     # Emit
     #--------------------------------------------------
 
     def emit(self, task: Task|Var):
+        self.mapped.clear()
         code = ""
         try:
             if isinstance(task, Task):
                 code = getattr(self, task.behavior.value)(task)
             elif isinstance(task, Var):
                 code = self.emit_var(task)
         except Exception as e:
@@ -511,14 +513,18 @@
             t = value
             return t.isoformat()
         return json.dumps(value)
 
     def emit_var(self, var: Var|Value):
         if not isinstance(var, Var):
             return self.emit_val(var)
+        if var in self.mapped:
+            return self.mapped[var]
+        if var.type.isa(Builtins.Symbol):
+            return f":{self.sanitize(var.value)}"
         if var.value is not None:
             return self.emit_val(var.value)
         if var.name == "_":
             return "_"
         name = self.namer.get(var)
         return f"_{self.sanitize(name).lower()}"
 
@@ -593,14 +599,22 @@
         vars_str = ", ".join([self.emit_var(i) for i in vals[mid_point:]])
         rows = []
         for ix in range(len(vals[0].value)):
             rows.append(",".join([self.emit_var(col.value[ix]) for col in vals[:mid_point]]))
         row_str = "; ".join(rows)
         return f"{{{row_str}}}({vars_str})"
 
+    def to_inline_set(self, action: Action, vars: set):
+        vals:Any = [v for v in action.bindings.values()]
+        rows = []
+        for ix in range(len(vals[0].value)):
+            rows.append(",".join([self.emit_var(col.value[ix]) for col in vals[:-1]]))
+        row_str = "; ".join(rows)
+        return (vals[-1], f"{{{row_str}}}")
+
     def to_inline_relation(self, task:Task, existing_vars=set()):
         return f"( {self.query(task, True)} )"
 
     #--------------------------------------------------
     # Query
     #--------------------------------------------------
 
@@ -614,14 +628,18 @@
         task_vars = gather_vars(task.items)
         self.stack.append(task_vars)
 
         for i in task.items:
             if i.action in [ActionType.Get, ActionType.Call]:
                 if i.entity.value == Builtins.RawData:
                     body.append(self.to_set(i, body_vars))
+                elif i.entity.value == Builtins.InlineRawData:
+                    (v, data) = self.to_inline_set(i, body_vars)
+                    self.mapped[v] = data
+                    head_vars.add(v)
                 else:
                     body.append(self.to_relation(i, body_vars, body))
             elif i.action == ActionType.Bind and i.entity.value == Builtins.Return:
                 head_rel = self.to_return(i, head_vars, body)
                 head = f"def {head_rel} =\n    "
             elif i.action in [ActionType.Bind, ActionType.Persist, ActionType.Unpersist]:
                 if not inline:
```

### Comparing `relationalai-0.1.8/src/relationalai/analysis/whynot.py` & `relationalai-0.1.9/src/relationalai/analysis/whynot.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.1.8/src/relationalai/clients/azure.py` & `relationalai-0.1.9/src/relationalai/clients/azure.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.1.8/src/relationalai/clients/client.py` & `relationalai-0.1.9/src/relationalai/clients/client.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.1.8/src/relationalai/clients/config.py` & `relationalai-0.1.9/src/relationalai/clients/config.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.1.8/src/relationalai/clients/snowflake.py` & `relationalai-0.1.9/src/relationalai/clients/snowflake.py`

 * *Files 0% similar despite different names*

```diff
@@ -471,16 +471,16 @@
 
     def schema_info(self, database:str, schema:str, tables:Iterable[str]):
         pks = self._exec(f"SHOW PRIMARY KEYS IN SCHEMA {database}.{schema};")
         fks = self._exec(f"SHOW IMPORTED KEYS IN SCHEMA {database}.{schema};")
         tables = ", ".join([f"'{x.upper()}'" for x in tables])
         columns = self._exec(f"""
             SELECT TABLE_NAME, COLUMN_NAME, DATA_TYPE
-            FROM {database}.INFORMATION_SCHEMA.COLUMNS
-            WHERE TABLE_SCHEMA = 'PUBLIC'
+            FROM {database.upper()}.INFORMATION_SCHEMA.COLUMNS
+            WHERE TABLE_SCHEMA = '{schema.upper()}'
             AND TABLE_NAME in ({tables})
             AND TABLE_CATALOG = '{database.upper()}';
         """)
         results = defaultdict(lambda: {"pks": [], "fks": {}, "columns": {}})
         if pks:
             for row in pks:
                 results[row[3].lower()]["pks"].append(row[4].lower()) # type: ignore
```

### Comparing `relationalai-0.1.8/src/relationalai/clients/sqlite.py` & `relationalai-0.1.9/src/relationalai/clients/sqlite.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.1.8/src/relationalai/clients/test.py` & `relationalai-0.1.9/src/relationalai/clients/test.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.1.8/src/relationalai/graphs/lib.py` & `relationalai-0.1.9/src/relationalai/graphs/lib.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,40 +1,85 @@
 from collections import defaultdict
+from copy import deepcopy
 from typing import Any
-from .. import dsl
+from .. import dsl, errors
 import gravis as gv
 
 #--------------------------------------------------
+# Errors
+#--------------------------------------------------
+
+def invalid_param(param:str, message:str):
+    source = errors.Errors.call_source(4)
+    marked = errors.mark_source(source, source.line, source.line) if source else ""
+    content = f"""
+    The [yellow]{param}[/yellow] parameter {message}
+
+    {marked}
+    """
+    errors.print_source_error(source, "Invalid algorithm parameter", content)
+    exit(1)
+
+#--------------------------------------------------
+# Validation
+#--------------------------------------------------
+
+def between(param:str, value, min, max):
+    if value < min or value > max:
+        invalid_param(param, f"must be between {min} and {max}")
+
+def positive(param:str, value):
+    if value <= 0:
+        invalid_param(param, "must be positive")
+
+#--------------------------------------------------
 # Graph
 #--------------------------------------------------
 
 class Compute:
     def __init__(self, graph:'Graph'):
         self._graph = graph
-        self._lib = getattr(self._graph.model.rel, self._graph._lib_ref())
+        self._lib = self._graph.model.rel.rel.graph
+        self._old_lib = getattr(self._graph.model.rel, self._graph._lib_ref())
 
+    def _config(self, **kwargs):
+        return dsl.InlineRelation(self._graph.model, [
+            *[(dsl.Symbol(k), v) for k, v in kwargs.items()],
+        ])
+
+    def pagerank(self, node, damping_factor=0.85, tolerance=1e-6, max_iter=20):
+        between("damping_factor", damping_factor, 0, 1)
+        positive("tolerance", tolerance)
+        positive("max_iter", max_iter)
+
+        config = self._config(
+            graph=self._graph,
+            damping_factor=damping_factor,
+            tolerance=tolerance,
+            max_iter=max_iter,
+        )
+        return self._lib.centrality.pagerank(config, node)
+
+    #TODO: these are still in the old style graph lib
     def degree(self, node, weight=None):
         if not weight:
-            return self._lib.degree(node)
-        return self._lib.weighted_degree(node)
-
-    def pagerank(self, node):
-        return self._lib.pagerank(node)
+            return self._old_lib.degree(node)
+        return self._old_lib.weighted_degree(node)
 
     def betweenness_centrality(self, node):
-        return self._lib.betweenness_centrality(node)
+        return self._old_lib.betweenness_centrality(node)
 
     def degree_centrality(self, node):
-        return self._lib.degree_centrality(node)
+        return self._old_lib.degree_centrality(node)
 
     def label_propagation(self, node):
-        return self._lib.label_propagation(node)
+        return self._old_lib.label_propagation(node)
 
     def weakly_connected_component(self, node):
-        return self._lib.weakly_connected_component(node)
+        return self._old_lib.weakly_connected_component(node)
 
 class Nodes:
     def __init__(self, graph:'Graph'):
         self._graph = graph
         self._type = dsl.RawRelation(self._graph.model, f"graph{self._graph.id}_nodes", 1)
         self._props = {}
 
@@ -107,75 +152,20 @@
 
     def _graph_ref(self):
         return f"graph{self.id}"
 
     def _lib_ref(self):
         return f"graphlib{self.id}"
 
-    def visualize(self, three=False, **kwargs):
-        data = self._last_fetch
-        if not data:
-            data = self.fetch()
-        def prepare_metadata(info):
-            metadata = {}
-            allowed_gjgf_node_keys = [
-                "color",
-                "opacity",
-                "size",
-                "shape",
-                "border_color",
-                "border_size",
-                "label_color",
-                "label_size",
-                "hover",
-                "click",
-                "image",
-                "x",
-                "y",
-                "z",
-            ]
-            hover_text = "\n".join([f"{k}: {v}" for (k,v) in info.items()
-                                    if k not in allowed_gjgf_node_keys + ["label"]])
-            for k in allowed_gjgf_node_keys:
-                if k in info:
-                    metadata[k] = info[k]
-            if hover_text:
-                metadata["hover"] = "\n".join([metadata["hover"] or "", hover_text])
-            return metadata
-        graph1 = {
-            "graph": {
-                "directed": not self.undirected,
-                "metadata": {
-                    "arrow_size": 4,
-                    "edge_size": 1,
-                    "edge_label_size": 10,
-                    "edge_label_color": "#E1856C",
-                    "edge_color": "#E1856C",
-                    "node_size": 10,
-                    "node_color": "#474B77",
-                    "node_label_color": "#474B77",
-                    "node_label_size": 10,
-                },
-                "nodes": {
-                    node_id: {
-                        **({"label": info["label"]} if "label" in info else {}),
-                        "metadata": prepare_metadata(info),
-                    }
-                    for (node_id, info) in data["nodes"].items()
-                },
-                "edges": [
-                    {"source": source, "target": target, "metadata": info}
-                    for ((source, target), info) in data["edges"].items()
-                ],
-            }
-        }
+    def _to_var(self):
+        return getattr(self.model.rel, self._graph_ref())._to_var()
 
-        vis = gv.vis if not three else gv.three
-        fig = vis(graph1, edge_label_data_source='label', node_label_data_source='label', edge_curvature=0.4, **kwargs)
-        return fig
+    #--------------------------------------------------
+    # Fetch
+    #--------------------------------------------------
 
     def fetch(self):
         code = []
         code.append(f"def output:nodes(n) = {self.nodes._type._name}(n)")
         for name, prop in self.nodes._props.items():
             code.append(f"def output:nodes:{name}(n, v) = {prop._name}(n, v)")
         code.append(f"def output:edges(a,b) = {self.edges._type._name}(a,b)")
@@ -204,14 +194,97 @@
                     for (a,b,v) in set["table"].itertuples(index=False):
                         cur[(a,b)][path[1]] = v
             else:
                 raise Exception(f"Unexpected path: {path}")
         self._last_fetch = output
         return output
 
+    #--------------------------------------------------
+    # Visualize
+    #--------------------------------------------------
+
+    default_visual_props = {
+        "node": {
+            "color": "black",
+            "opacity": 1,
+            "size": 10,
+            "shape": "circle",
+            "border_color": "black",
+            "border_size": 1,
+            "label_color": "black",
+            "label_size": 10,
+        },
+        "edge": {
+            "color": "#999",
+            "opacity": 1,
+            "size": 2,
+            "shape": "circle",
+            "border_color": "#999",
+            "border_size": 1,
+            "label_color": "black",
+            "label_size": 10,
+            "arrow_size": 4,
+            "arrow_color": "#999",
+        }
+    }
+
+    _style_map = {
+        "arrow_size": "arrow_size",
+        "arrow_color": "arrow_color",
+    }
+
+
+    def _visual_props(self, prop_def, metadata):
+        for k, v in prop_def.items():
+            if callable(v):
+                metadata[k] = v(metadata)
+        return metadata
+
+    def visualize(self, three=False, style={"node": {}, "edge": {}}, **kwargs):
+        data = self._last_fetch
+        if not data:
+            data = self.fetch()
+
+        style = deepcopy(style)
+        if "node" not in style:
+            style["node"] = {}
+        if "edge" not in style:
+            style["edge"] = {}
+        merged_style = deepcopy(self.default_visual_props)
+        for category in ["node", "edge"]:
+            for k, v in style.get(category, {}).items():
+                if not callable(v):
+                    merged_style[category][k] = v
+        flat_style = {self._style_map.get(k, f"{type}_{k}"): v
+                        for type, category in merged_style.items()
+                        for k, v in category.items()}
+
+        graph1 = {
+            "graph": {
+                "directed": not self.undirected,
+                "metadata": flat_style,
+                "nodes": {
+                    node_id: {
+                        **({"label": info["label"]} if "label" in info else {}),
+                        "metadata": self._visual_props(style["node"], info),
+                    }
+                    for (node_id, info) in data["nodes"].items()
+                },
+                "edges": [
+                    {"source": source, "target": target, "metadata": self._visual_props(style["edge"], info)}
+                    for ((source, target), info) in data["edges"].items()
+                ],
+            }
+        }
+
+        vis = gv.vis if not three else gv.three
+        fig = vis(graph1, edge_label_data_source='label', node_label_data_source='label', edge_curvature=0.4, **kwargs)
+        return fig
+
+
 #--------------------------------------------------
 # Edge
 #--------------------------------------------------
 
 class Edge:
     def __init__(self, type:Any, from_:Any, to:Any):
         # raise NotImplementedError()
```

### Comparing `relationalai-0.1.8/src/relationalai/loaders/csv.py` & `relationalai-0.1.9/src/relationalai/loaders/csv.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.1.8/src/relationalai/tools/cli.py` & `relationalai-0.1.9/src/relationalai/tools/cli.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.1.8/src/relationalai/tools/cli_controls.py` & `relationalai-0.1.9/src/relationalai/tools/cli_controls.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.1.8/src/relationalai/tools/debugger.py` & `relationalai-0.1.9/src/relationalai/tools/debugger.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.1.8/src/relationalai/tools/dev.py` & `relationalai-0.1.9/src/relationalai/tools/dev.py`

 * *Files 2% similar despite different names*

```diff
@@ -124,18 +124,19 @@
 @cli.command()
 def stats():
     core = cloc(["compiler.py", "dsl.py", "metamodel.py", "rel.py"])
     dsl = cloc(["dsl.py"])
     compiler = cloc(["compiler.py"])
     metamodel = cloc(["metamodel.py"])
     rel = cloc(["rel.py"])
-    gentest = cloc(["../gentest"])
+    metagen = cloc(["metagen.py"])
+    gentest = cloc(["../gentest", "metagen.py"])
     tools = cloc(["tools/"])
     clients = cloc(["clients/"])
-    non_test_total = cloc(["."])
+    non_test_total = cloc(["."]) - metagen
     total = non_test_total + gentest
 
     max_width = len(f"{total:,}")
 
     # Print statements with numbers right-aligned
     divider()
     rich.print(f"[yellow]RelationalAI  {non_test_total:>{max_width},} loc")
```

### Comparing `relationalai-0.1.8/tests/conftest.py` & `relationalai-0.1.9/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.1.8/tests/roundtrip/test_document.py` & `relationalai-0.1.9/tests/roundtrip/test_document.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.1.8/tests/roundtrip/test_task.py` & `relationalai-0.1.9/tests/roundtrip/test_task.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.1.8/pyproject.toml` & `relationalai-0.1.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = 'relationalai'
-version = '0.1.8'
+version = '0.1.9'
 description = 'RelationalAI Library and CLI'
 readme="PYPI_README.md"
 authors = [
     { name="RelationalAI", email="support@relational.ai" },
 ]
 requires-python = ">= 3.10"
 dependencies = [
```

### Comparing `relationalai-0.1.8/PKG-INFO` & `relationalai-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: relationalai
-Version: 0.1.8
+Version: 0.1.9
 Summary: RelationalAI Library and CLI
 Author-email: RelationalAI <support@relational.ai>
 Requires-Python: >=3.10
 Requires-Dist: bytecode
 Requires-Dist: click
 Requires-Dist: colorama
 Requires-Dist: docutils
```

