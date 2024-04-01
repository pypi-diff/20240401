# Comparing `tmp/bytewax-0.8.0_beta.2.tar.gz` & `tmp/bytewax-0.9.0.tar.gz`

## Comparing `bytewax-0.8.0_beta.2.tar` & `bytewax-0.9.0.tar`

### file list

```diff
@@ -1,62 +1,103 @@
--rw-r--r--   0        0        0      846 1970-01-01 00:00:00.000000 bytewax-0.8.0_beta.2/Cargo.toml
--rw-r--r--   0     1001      121      990 2022-02-25 12:22:50.000000 bytewax-0.8.0_beta.2/.dockerignore
--rw-r--r--   0     1001      121     1376 2022-02-25 12:22:50.000000 bytewax-0.8.0_beta.2/.github/ISSUE_TEMPLATE/bug_report.yml
--rw-r--r--   0     1001      121      599 2022-02-25 12:22:50.000000 bytewax-0.8.0_beta.2/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0     1001      121     4753 2022-02-25 12:22:50.000000 bytewax-0.8.0_beta.2/.github/workflows/CI.yml
--rw-r--r--   0     1001      121      686 2022-02-25 12:22:50.000000 bytewax-0.8.0_beta.2/.gitignore
--rw-r--r--   0     1001      121     1306 2022-02-25 12:22:50.000000 bytewax-0.8.0_beta.2/CHANGELOG.md
--rw-r--r--   0     1001      121     5481 2022-02-25 12:22:50.000000 bytewax-0.8.0_beta.2/CODE_OF_CONDUCT.md
--rw-r--r--   0     1001      121      549 2022-02-25 12:22:50.000000 bytewax-0.8.0_beta.2/COPYRIGHT
--rw-r--r--   0     1001      121      985 2022-02-25 12:22:50.000000 bytewax-0.8.0_beta.2/Dockerfile
--rw-r--r--   0     1001      121      443 2022-02-25 12:22:50.000000 bytewax-0.8.0_beta.2/Dockerfile.release
--rw-r--r--   0     1001      121    10142 2022-02-25 12:22:50.000000 bytewax-0.8.0_beta.2/LICENSE.md
--rw-r--r--   0     1001      121     2069 2022-02-25 12:22:50.000000 bytewax-0.8.0_beta.2/README.md
--rw-r--r--   0     1001      121  1446261 2022-02-25 12:22:50.000000 bytewax-0.8.0_beta.2/benches/benchmarks/collected-works.txt
--rw-r--r--   0     1001      121      413 2022-02-25 12:22:50.000000 bytewax-0.8.0_beta.2/benches/benchmarks/wordcount_bytewax.py
--rw-r--r--   0     1001      121      325 2022-02-25 12:22:50.000000 bytewax-0.8.0_beta.2/benches/benchmarks/wordcount_python.py
--rw-r--r--   0     1001      121     1129 2022-02-25 12:22:50.000000 bytewax-0.8.0_beta.2/benches/benchmarks.rs
--rwxr-xr-x   0     1001      121      221 2022-02-25 12:22:50.000000 bytewax-0.8.0_beta.2/entrypoint.sh
--rw-r--r--   0     1001      121     1817 2022-02-25 12:22:50.000000 bytewax-0.8.0_beta.2/examples/anomaly_detector.py
--rw-r--r--   0     1001      121      505 2022-02-25 12:22:50.000000 bytewax-0.8.0_beta.2/examples/basic.py
--rw-r--r--   0     1001      121     2420 2022-02-25 12:22:50.000000 bytewax-0.8.0_beta.2/examples/events_to_parquet.py
--rw-r--r--   0     1001      121     2270 2022-02-25 12:22:50.000000 bytewax-0.8.0_beta.2/examples/manual_cluster.py
--rw-r--r--   0     1001      121     2156 2022-02-25 12:22:50.000000 bytewax-0.8.0_beta.2/examples/pagerank.py
--rw-r--r--   0     1001      121       30 2022-02-25 12:22:50.000000 bytewax-0.8.0_beta.2/examples/sample_data/cluster/partition-1.txt
--rw-r--r--   0     1001      121       30 2022-02-25 12:22:50.000000 bytewax-0.8.0_beta.2/examples/sample_data/cluster/partition-2.txt
--rw-r--r--   0     1001      121       42 2022-02-25 12:22:50.000000 bytewax-0.8.0_beta.2/examples/sample_data/cluster/partition-3.txt
--rw-r--r--   0     1001      121       36 2022-02-25 12:22:50.000000 bytewax-0.8.0_beta.2/examples/sample_data/cluster/partition-4.txt
--rw-r--r--   0     1001      121       36 2022-02-25 12:22:50.000000 bytewax-0.8.0_beta.2/examples/sample_data/cluster/partition-5.txt
--rw-r--r--   0     1001      121       10 2022-02-25 12:22:50.000000 bytewax-0.8.0_beta.2/examples/sample_data/easy_count.txt
--rw-r--r--   0     1001      121       72 2022-02-25 12:22:50.000000 bytewax-0.8.0_beta.2/examples/sample_data/graph.txt
--rw-r--r--   0     1001      121      217 2022-02-25 12:22:50.000000 bytewax-0.8.0_beta.2/examples/sample_data/lyrics.txt
--rw-r--r--   0     1001      121      198 2022-02-25 12:22:50.000000 bytewax-0.8.0_beta.2/examples/sample_data/wordcount.txt
--rw-r--r--   0     1001      121     2594 2022-02-25 12:22:50.000000 bytewax-0.8.0_beta.2/examples/search_session.py
--rw-r--r--   0     1001      121      200 2022-02-25 12:22:50.000000 bytewax-0.8.0_beta.2/examples/simple.py
--rw-r--r--   0     1001      121      763 2022-02-25 12:22:50.000000 bytewax-0.8.0_beta.2/examples/sleepyworkers.py
--rw-r--r--   0     1001      121     1213 2022-02-25 12:22:50.000000 bytewax-0.8.0_beta.2/examples/subflow.py
--rw-r--r--   0     1001      121      592 2022-02-25 12:22:50.000000 bytewax-0.8.0_beta.2/examples/translator.py
--rw-r--r--   0     1001      121      876 2022-02-25 12:22:50.000000 bytewax-0.8.0_beta.2/examples/twitter_stream.py
--rw-r--r--   0     1001      121        0 2022-02-25 12:22:50.000000 bytewax-0.8.0_beta.2/examples/utils/__init__.py
--rw-r--r--   0     1001      121      362 2022-02-25 12:22:50.000000 bytewax-0.8.0_beta.2/examples/utils/fake_events.py
--rw-r--r--   0     1001      121     2902 2022-02-25 12:22:50.000000 bytewax-0.8.0_beta.2/examples/utils/twitter.py
--rw-r--r--   0     1001      121     1105 2022-02-25 12:22:50.000000 bytewax-0.8.0_beta.2/examples/wikistream.py
--rw-r--r--   0     1001      121      754 2022-02-25 12:22:50.000000 bytewax-0.8.0_beta.2/examples/wordcount.py
--rw-r--r--   0     1001      121     1068 2022-02-25 12:22:50.000000 bytewax-0.8.0_beta.2/pyproject.toml
--rw-r--r--   0     1001      121       48 2022-02-25 12:22:50.000000 bytewax-0.8.0_beta.2/pysrc/bytewax/__init__.py
--rw-r--r--   0     1001      121        0 2022-02-25 12:22:50.000000 bytewax-0.8.0_beta.2/pysrc/bytewax/bytewax.pyi
--rw-r--r--   0     1001      121     5508 2022-02-25 12:22:50.000000 bytewax-0.8.0_beta.2/pysrc/bytewax/execution.py
--rw-r--r--   0     1001      121     1847 2022-02-25 12:22:50.000000 bytewax-0.8.0_beta.2/pysrc/bytewax/exhash.py
--rw-r--r--   0     1001      121     2132 2022-02-25 12:22:50.000000 bytewax-0.8.0_beta.2/pysrc/bytewax/inp.py
--rw-r--r--   0     1001      121     4629 2022-02-25 12:22:50.000000 bytewax-0.8.0_beta.2/pysrc/bytewax/parse.py
--rw-r--r--   0     1001      121        0 2022-02-25 12:22:50.000000 bytewax-0.8.0_beta.2/pysrc/bytewax/py.typed
--rw-r--r--   0     1001      121     1267 2022-02-25 12:22:50.000000 bytewax-0.8.0_beta.2/pytests/test_exhash.py
--rw-r--r--   0     1001      121      740 2022-02-25 12:22:50.000000 bytewax-0.8.0_beta.2/pytests/test_inputs.py
--rw-r--r--   0     1001      121     5840 2022-02-25 12:22:50.000000 bytewax-0.8.0_beta.2/pytests/test_operators.py
--rw-r--r--   0     1001      121     1112 2022-02-25 12:22:50.000000 bytewax-0.8.0_beta.2/pytests/test_parse.py
--rw-r--r--   0     1001      121     1496 2022-02-25 12:22:50.000000 bytewax-0.8.0_beta.2/pytests/test_run.py
--rwxr-xr-x   0     1001      121      716 2022-02-25 12:23:16.000000 bytewax-0.8.0_beta.2/run-maturin-action.sh
--rw-r--r--   0     1001      121       31 2022-02-25 12:22:50.000000 bytewax-0.8.0_beta.2/rust-toolchain.toml
--rw-r--r--   0     1001      121    40466 2022-02-25 12:22:50.000000 bytewax-0.8.0_beta.2/src/lib.rs
--rw-r--r--   0     1001      121      373 2022-02-25 12:22:50.000000 bytewax-0.8.0_beta.2/src/macros.rs
--rw-r--r--   0     1001      121     1307 2022-02-25 12:22:50.000000 bytewax-0.8.0_beta.2/src/webserver/mod.rs
--rw-r--r--   0        0        0     3123 1970-01-01 00:00:00.000000 bytewax-0.8.0_beta.2/PKG-INFO
+-rw-r--r--   0        0        0      693 1970-01-01 00:00:00.000000 bytewax-0.9.0/Cargo.toml
+-rw-r--r--   0     1001      121      990 2022-04-22 17:56:01.000000 bytewax-0.9.0/.dockerignore
+-rw-r--r--   0     1001      121     1376 2022-04-22 17:56:01.000000 bytewax-0.9.0/.github/ISSUE_TEMPLATE/bug_report.yml
+-rw-r--r--   0     1001      121      599 2022-04-22 17:56:01.000000 bytewax-0.9.0/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0     1001      121     6646 2022-04-22 17:56:01.000000 bytewax-0.9.0/.github/workflows/CI.yml
+-rw-r--r--   0     1001      121      686 2022-04-22 17:56:01.000000 bytewax-0.9.0/.gitignore
+-rw-r--r--   0     1001      121     1902 2022-04-22 17:56:01.000000 bytewax-0.9.0/CHANGELOG.md
+-rw-r--r--   0     1001      121     5481 2022-04-22 17:56:01.000000 bytewax-0.9.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0     1001      121      549 2022-04-22 17:56:01.000000 bytewax-0.9.0/COPYRIGHT
+-rw-r--r--   0     1001      121     1063 2022-04-22 17:56:01.000000 bytewax-0.9.0/Dockerfile
+-rw-r--r--   0     1001      121      573 2022-04-22 17:56:01.000000 bytewax-0.9.0/Dockerfile.release
+-rw-r--r--   0     1001      121    11343 2022-04-22 17:56:01.000000 bytewax-0.9.0/LICENSE
+-rw-r--r--   0     1001      121     3711 2022-04-22 17:56:01.000000 bytewax-0.9.0/README.md
+-rw-r--r--   0     1001      121     2571 2022-04-22 17:56:01.000000 bytewax-0.9.0/RELEASE.md
+-rwxr-xr-x   0     1001      121       93 2022-04-22 17:56:01.000000 bytewax-0.9.0/apidocs/build.sh
+-rw-r--r--   0     1001      121     5572 2022-04-22 17:56:01.000000 bytewax-0.9.0/apidocs/html/bytewax/exhash.html
+-rw-r--r--   0     1001      121    33429 2022-04-22 17:56:01.000000 bytewax-0.9.0/apidocs/html/bytewax/index.html
+-rw-r--r--   0     1001      121    31334 2022-04-22 17:56:01.000000 bytewax-0.9.0/apidocs/html/bytewax/inputs.html
+-rw-r--r--   0     1001      121    19084 2022-04-22 17:56:01.000000 bytewax-0.9.0/apidocs/html/bytewax/parse.html
+-rw-r--r--   0     1001      121     9196 2022-04-22 17:56:01.000000 bytewax-0.9.0/apidocs/html/bytewax/testing.html
+-rw-r--r--   0     1001      121       14 2022-04-22 17:56:01.000000 bytewax-0.9.0/apidocs/requirements.txt
+-rw-r--r--   0     1001      121        0 2022-04-22 17:56:01.000000 bytewax-0.9.0/apidocs/templates/.gitkeep
+-rw-r--r--   0     1001      121      987 2022-04-22 17:56:01.000000 bytewax-0.9.0/apidocs/templates/config.mako
+-rw-r--r--   0     1001      121    12482 2022-04-22 17:56:01.000000 bytewax-0.9.0/apidocs/templates/html.mako
+-rw-r--r--   0     1001      121       36 2022-04-22 17:56:01.000000 bytewax-0.9.0/build.requirements.txt
+-rw-r--r--   0     1001      121     4039 2022-04-22 17:56:01.000000 bytewax-0.9.0/docs/articles/getting-started/design-patterns.md
+-rw-r--r--   0     1001      121     7132 2022-04-22 17:56:01.000000 bytewax-0.9.0/docs/articles/getting-started/epochs.md
+-rw-r--r--   0     1001      121     9073 2022-04-22 17:56:01.000000 bytewax-0.9.0/docs/articles/getting-started/execution.md
+-rw-r--r--   0     1001      121      392 2022-04-22 17:56:01.000000 bytewax-0.9.0/docs/articles/getting-started/installation.md
+-rw-r--r--   0     1001      121     2191 2022-04-22 17:56:01.000000 bytewax-0.9.0/docs/articles/getting-started/operators.md
+-rw-r--r--   0     1001      121      889 2022-04-22 17:56:01.000000 bytewax-0.9.0/docs/articles/getting-started/overview.md
+-rw-r--r--   0     1001      121     7509 2022-04-22 17:56:01.000000 bytewax-0.9.0/docs/articles/getting-started/simple-example.md
+-rw-r--r--   0     1001      121      198 2022-04-22 17:56:01.000000 bytewax-0.9.0/docs/articles/getting-started/wordcount.txt
+-rw-r--r--   0     1001      121      700 2022-04-22 17:56:01.000000 bytewax-0.9.0/docs/articles/metadata.json
+-rw-r--r--   0     1001      121    13208 2022-04-22 17:56:01.000000 bytewax-0.9.0/docs/conftest.py
+-rw-r--r--   0     1001      121      260 2022-04-22 17:56:01.000000 bytewax-0.9.0/docs/examples/metadata.json
+-rw-r--r--   0     1001      121     8916 2022-04-22 17:56:01.000000 bytewax-0.9.0/docs/examples/search-session.md
+-rwxr-xr-x   0     1001      121      221 2022-04-22 17:56:01.000000 bytewax-0.9.0/entrypoint.sh
+-rw-r--r--   0     1001      121     1827 2022-04-22 17:56:01.000000 bytewax-0.9.0/examples/anomaly_detector.py
+-rw-r--r--   0     1001      121     2094 2022-04-22 17:56:01.000000 bytewax-0.9.0/examples/apriori.py
+-rw-r--r--   0     1001      121      505 2022-04-22 17:56:01.000000 bytewax-0.9.0/examples/basic.py
+-rw-r--r--   0     1001      121     2447 2022-04-22 17:56:01.000000 bytewax-0.9.0/examples/events_to_parquet.py
+-rw-r--r--   0     1001      121       15 2022-04-22 17:56:01.000000 bytewax-0.9.0/examples/feast/.feastignore
+-rw-r--r--   0     1001      121      922 2022-04-22 17:56:01.000000 bytewax-0.9.0/examples/feast/README.md
+-rw-r--r--   0     1001      121    34728 2022-04-22 17:56:01.000000 bytewax-0.9.0/examples/feast/data/driver_stats.parquet
+-rw-r--r--   0     1001      121      930 2022-04-22 17:56:01.000000 bytewax-0.9.0/examples/feast/docker-compose.yml
+-rw-r--r--   0     1001      121     3424 2022-04-22 17:56:01.000000 bytewax-0.9.0/examples/feast/feast_dataflow.py
+-rw-r--r--   0     1001      121      219 2022-04-22 17:56:01.000000 bytewax-0.9.0/examples/feast/feature_store.yaml
+-rw-r--r--   0     1001      121     1344 2022-04-22 17:56:01.000000 bytewax-0.9.0/examples/feast/feature_view.py
+-rw-r--r--   0     1001      121       41 2022-04-22 17:56:01.000000 bytewax-0.9.0/examples/feast/requirements.txt
+-rw-r--r--   0     1001      121     1089 2022-04-22 17:56:01.000000 bytewax-0.9.0/examples/feast/utils/stream_data.py
+-rw-r--r--   0     1001      121     2727 2022-04-22 17:56:01.000000 bytewax-0.9.0/examples/k8s_cluster.py
+-rw-r--r--   0     1001      121     2269 2022-04-22 17:56:01.000000 bytewax-0.9.0/examples/manual_cluster.py
+-rw-r--r--   0     1001      121     2156 2022-04-22 17:56:01.000000 bytewax-0.9.0/examples/pagerank.py
+-rw-r--r--   0     1001      121  7547152 2022-04-22 17:56:01.000000 bytewax-0.9.0/examples/rpk-events-stream.ipynb
+-rw-r--r--   0     1001      121      247 2022-04-22 17:56:01.000000 bytewax-0.9.0/examples/sample_data/apriori.txt
+-rw-r--r--   0     1001      121       30 2022-04-22 17:56:01.000000 bytewax-0.9.0/examples/sample_data/cluster/partition-1.txt
+-rw-r--r--   0     1001      121       30 2022-04-22 17:56:01.000000 bytewax-0.9.0/examples/sample_data/cluster/partition-2.txt
+-rw-r--r--   0     1001      121       42 2022-04-22 17:56:01.000000 bytewax-0.9.0/examples/sample_data/cluster/partition-3.txt
+-rw-r--r--   0     1001      121       36 2022-04-22 17:56:01.000000 bytewax-0.9.0/examples/sample_data/cluster/partition-4.txt
+-rw-r--r--   0     1001      121       36 2022-04-22 17:56:01.000000 bytewax-0.9.0/examples/sample_data/cluster/partition-5.txt
+-rw-r--r--   0     1001      121  1446261 2022-04-22 17:56:01.000000 bytewax-0.9.0/examples/sample_data/collected-works.txt
+-rw-r--r--   0     1001      121       10 2022-04-22 17:56:01.000000 bytewax-0.9.0/examples/sample_data/easy_count.txt
+-rw-r--r--   0     1001      121  1242820 2022-04-22 17:56:01.000000 bytewax-0.9.0/examples/sample_data/ec2_metrics.csv
+-rw-r--r--   0     1001      121       72 2022-04-22 17:56:01.000000 bytewax-0.9.0/examples/sample_data/graph.txt
+-rw-r--r--   0     1001      121      217 2022-04-22 17:56:01.000000 bytewax-0.9.0/examples/sample_data/lyrics.txt
+-rw-r--r--   0     1001      121      198 2022-04-22 17:56:01.000000 bytewax-0.9.0/examples/sample_data/wordcount.txt
+-rw-r--r--   0     1001      121     2594 2022-04-22 17:56:01.000000 bytewax-0.9.0/examples/search_session.py
+-rw-r--r--   0     1001      121      200 2022-04-22 17:56:01.000000 bytewax-0.9.0/examples/simple.py
+-rw-r--r--   0     1001      121      763 2022-04-22 17:56:01.000000 bytewax-0.9.0/examples/sleepyworkers.py
+-rw-r--r--   0     1001      121     1219 2022-04-22 17:56:01.000000 bytewax-0.9.0/examples/subflow.py
+-rw-r--r--   0     1001      121      598 2022-04-22 17:56:01.000000 bytewax-0.9.0/examples/translator.py
+-rw-r--r--   0     1001      121      934 2022-04-22 17:56:01.000000 bytewax-0.9.0/examples/twitter_stream.py
+-rw-r--r--   0     1001      121        0 2022-04-22 17:56:01.000000 bytewax-0.9.0/examples/utils/__init__.py
+-rw-r--r--   0     1001      121      362 2022-04-22 17:56:01.000000 bytewax-0.9.0/examples/utils/fake_events.py
+-rw-r--r--   0     1001      121     1516 2022-04-22 17:56:01.000000 bytewax-0.9.0/examples/utils/topics_helper.py
+-rw-r--r--   0     1001      121     2902 2022-04-22 17:56:01.000000 bytewax-0.9.0/examples/utils/twitter.py
+-rw-r--r--   0     1001      121     1564 2022-04-22 17:56:01.000000 bytewax-0.9.0/examples/wikistream.py
+-rw-r--r--   0     1001      121      749 2022-04-22 17:56:01.000000 bytewax-0.9.0/examples/wordcount.py
+-rw-r--r--   0     1001      121     1297 2022-04-22 17:56:01.000000 bytewax-0.9.0/pyproject.toml
+-rw-r--r--   0     1001      121      711 2022-04-22 17:56:01.000000 bytewax-0.9.0/pysrc/bytewax/__init__.py
+-rw-r--r--   0     1001      121     7053 2022-04-22 17:56:01.000000 bytewax-0.9.0/pysrc/bytewax/execution.py
+-rw-r--r--   0     1001      121     1964 2022-04-22 17:56:01.000000 bytewax-0.9.0/pysrc/bytewax/exhash.py
+-rw-r--r--   0     1001      121     8985 2022-04-22 17:56:01.000000 bytewax-0.9.0/pysrc/bytewax/inputs.py
+-rw-r--r--   0     1001      121     5308 2022-04-22 17:56:01.000000 bytewax-0.9.0/pysrc/bytewax/parse.py
+-rw-r--r--   0     1001      121        0 2022-04-22 17:56:01.000000 bytewax-0.9.0/pysrc/bytewax/py.typed
+-rw-r--r--   0     1001      121     1445 2022-04-22 17:56:01.000000 bytewax-0.9.0/pysrc/bytewax/testing.py
+-rw-r--r--   0     1001      121      121 2022-04-22 17:56:01.000000 bytewax-0.9.0/pytests/conftest.py
+-rw-r--r--   0     1001      121     5224 2022-04-22 17:56:01.000000 bytewax-0.9.0/pytests/test_execution.py
+-rw-r--r--   0     1001      121     1267 2022-04-22 17:56:01.000000 bytewax-0.9.0/pytests/test_exhash.py
+-rw-r--r--   0     1001      121     3335 2022-04-22 17:56:01.000000 bytewax-0.9.0/pytests/test_inputs.py
+-rw-r--r--   0     1001      121     6162 2022-04-22 17:56:01.000000 bytewax-0.9.0/pytests/test_operators.py
+-rw-r--r--   0     1001      121     1112 2022-04-22 17:56:01.000000 bytewax-0.9.0/pytests/test_parse.py
+-rwxr-xr-x   0     1001      121      716 2022-04-22 17:56:23.000000 bytewax-0.9.0/run-maturin-action.sh
+-rw-r--r--   0     1001      121       31 2022-04-22 17:56:01.000000 bytewax-0.9.0/rust-toolchain.toml
+-rw-r--r--   0     1001      121    24814 2022-04-22 17:56:01.000000 bytewax-0.9.0/src/dataflow/mod.rs
+-rw-r--r--   0     1001      121    13951 2022-04-22 17:56:01.000000 bytewax-0.9.0/src/execution/mod.rs
+-rw-r--r--   0     1001      121      946 2022-04-22 17:56:01.000000 bytewax-0.9.0/src/lib.rs
+-rw-r--r--   0     1001      121      639 2022-04-22 17:56:01.000000 bytewax-0.9.0/src/macros.rs
+-rw-r--r--   0     1001      121     6312 2022-04-22 17:56:01.000000 bytewax-0.9.0/src/operators/mod.rs
+-rw-r--r--   0     1001      121     9804 2022-04-22 17:56:01.000000 bytewax-0.9.0/src/pyo3_extensions/mod.rs
+-rw-r--r--   0     1001      121     1307 2022-04-22 17:56:01.000000 bytewax-0.9.0/src/webserver/mod.rs
+-rw-r--r--   0        0        0     4780 1970-01-01 00:00:00.000000 bytewax-0.9.0/PKG-INFO
```

### Comparing `bytewax-0.8.0_beta.2/.dockerignore` & `bytewax-0.9.0/.dockerignore`

 * *Files identical despite different names*

### Comparing `bytewax-0.8.0_beta.2/.github/ISSUE_TEMPLATE/bug_report.yml` & `bytewax-0.9.0/.github/ISSUE_TEMPLATE/bug_report.yml`

 * *Files identical despite different names*

### Comparing `bytewax-0.8.0_beta.2/.github/ISSUE_TEMPLATE/feature_request.md` & `bytewax-0.9.0/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `bytewax-0.8.0_beta.2/.gitignore` & `bytewax-0.9.0/.gitignore`

 * *Files identical despite different names*

### Comparing `bytewax-0.8.0_beta.2/CODE_OF_CONDUCT.md` & `bytewax-0.9.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `bytewax-0.8.0_beta.2/COPYRIGHT` & `bytewax-0.9.0/COPYRIGHT`

 * *Files identical despite different names*

### Comparing `bytewax-0.8.0_beta.2/Dockerfile` & `bytewax-0.9.0/Dockerfile`

 * *Files 26% similar despite different names*

```diff
@@ -22,7 +22,11 @@
 COPY --from=maturin-builder /bytewax/target/wheels/bytewax-$BYTEWAX_VERSION-cp39-cp39-manylinux_2_12_x86_64.manylinux2010_x86_64.whl /bytewax/target/wheels/bytewax-$BYTEWAX_VERSION-cp39-cp39-manylinux_2_12_x86_64.manylinux2010_x86_64.whl
 RUN /venv/bin/pip3 install /bytewax/target/wheels/bytewax-$BYTEWAX_VERSION-cp39-cp39-manylinux_2_12_x86_64.manylinux2010_x86_64.whl
 
 FROM gcr.io/distroless/python3-debian11:debug
 COPY --from=build /venv /venv
 WORKDIR /bytewax
 COPY ./entrypoint.sh .
+
+ENV BYTEWAX_WORKDIR=/bytewax
+
+ENTRYPOINT ["/bin/sh", "-c", "./entrypoint.sh"]
```

### Comparing `bytewax-0.8.0_beta.2/LICENSE.md` & `bytewax-0.9.0/LICENSE`

 * *Files 4% similar despite different names*

```diff
@@ -169,7 +169,33 @@
       License. However, in accepting such obligations, You may act only
       on Your own behalf and on Your sole responsibility, not on behalf
       of any other Contributor, and only if You agree to indemnify,
       defend, and hold each Contributor harmless for any liability
       incurred by, or claims asserted against, such Contributor by reason
       of your accepting any such warranty or additional liability.
 
+   END OF TERMS AND CONDITIONS
+
+   APPENDIX: How to apply the Apache License to your work.
+
+      To apply the Apache License to your work, attach the following
+      boilerplate notice, with the fields enclosed by brackets "[]"
+      replaced with your own identifying information. (Don't include
+      the brackets!)  The text should be enclosed in the appropriate
+      comment syntax for the file format. We also recommend that a
+      file or class name and description of purpose be included on the
+      same "printed page" as the copyright notice for easier
+      identification within third-party archives.
+
+   Copyright 2022 Bytewax, Inc.
+
+   Licensed under the Apache License, Version 2.0 (the "License");
+   you may not use this file except in compliance with the License.
+   You may obtain a copy of the License at
+
+       http://www.apache.org/licenses/LICENSE-2.0
+
+   Unless required by applicable law or agreed to in writing, software
+   distributed under the License is distributed on an "AS IS" BASIS,
+   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+   See the License for the specific language governing permissions and
+   limitations under the License.
```

### Comparing `bytewax-0.8.0_beta.2/benches/benchmarks/collected-works.txt` & `bytewax-0.9.0/examples/sample_data/collected-works.txt`

 * *Files identical despite different names*

### Comparing `bytewax-0.8.0_beta.2/examples/anomaly_detector.py` & `bytewax-0.9.0/examples/anomaly_detector.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import random
 
-from bytewax import Dataflow, inp, parse, run_cluster
+from bytewax import Dataflow, inputs, parse, run_cluster
 
 
 def random_datapoints():
     for _ in range(20):
         yield "QPS", random.randrange(0, 10)
 
 
@@ -51,17 +51,17 @@
     print(
         f"{metric} @ {epoch}: value = {value}, mu = {mu:.2f}, sigma = {sigma:.2f}, {is_anomalous}"
     )
 
 
 flow = Dataflow()
 # ("metric", value)
-flow.stateful_map(lambda: ZTestDetector(2.0), ZTestDetector.push)
+flow.stateful_map(lambda key: ZTestDetector(2.0), ZTestDetector.push)
 # ("metric", (value, mu, sigma, is_anomalous))
 flow.capture()
 
 
 if __name__ == "__main__":
     for epoch, item in run_cluster(
-        flow, inp.fully_ordered(random_datapoints()), **parse.cluster_args()
+        flow, inputs.fully_ordered(random_datapoints()), **parse.cluster_args()
     ):
         inspector(epoch, item)
```

### Comparing `bytewax-0.8.0_beta.2/examples/events_to_parquet.py` & `bytewax-0.9.0/examples/events_to_parquet.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 import json
 import time
-from datetime import datetime
+import datetime
 
 import pandas
 
 import pyarrow.parquet as parquet
-from bytewax import Dataflow, inp, parse, spawn_cluster
+from bytewax import Dataflow, inputs, parse, spawn_cluster
 from pandas import DataFrame
 from pyarrow import Table
 
 from utils import fake_events
 
 # Collect 5 second tumbling windows of data and write them out as
 # Parquet datasets. `fake_events` will generate events for multiple
 # days around today. Each worker will generate independent fake
 # events.
 def input_builder(worker_index, worker_count):
-    return inp.tumbling_epoch(5.0, fake_events.generate_web_events())
+    return inputs.tumbling_epoch(fake_events.generate_web_events(), datetime.timedelta(seconds=5))
 
 
 # Arrow assigns a UUID to each worker / window's file so they won't
 # clobber each other. They are further automatically placed in the
 # correct directory structure based on date and path.
 def write_parquet(epoch__events_df):
     """Write events as partitioned Parquet in `$PWD/parquet_demo_out/`"""
@@ -36,15 +36,15 @@
 # Each worker writes using the same code because we don't need to
 # further partition because of the UUID described above.
 def output_builder(worker_index, worker_count):
     return write_parquet
 
 
 def add_date_columns(event):
-    timestamp = datetime.fromisoformat(event["event_timestamp"])
+    timestamp = datetime.datetime.fromisoformat(event["event_timestamp"])
     event["year"] = timestamp.year
     event["month"] = timestamp.month
     event["day"] = timestamp.day
     return event
 
 
 def group_by_page(event):
```

### Comparing `bytewax-0.8.0_beta.2/examples/manual_cluster.py` & `bytewax-0.9.0/examples/manual_cluster.py`

 * *Files 0% similar despite different names*

```diff
@@ -54,14 +54,14 @@
     # ./examples/sample_data/cluster/*.txt which have lines like
     # `one1`.
 
     # They will then both finish and you'll see ./cluster_out/0.out
     # and ./cluster_out/1.out with the data that each process in the
     # cluster wrote with the lines uppercased.
 
-    # You could imagine reading from / writing to separate Kafaka
+    # You could imagine reading from / writing to separate Kafka
     # partitions, S3 blobs, etc.
 
     # When using `cluster_main()` you have to coordinate ensuring each
     # process knows the address of all other processes in the cluster
     # and their unique process ID.
     cluster_main(flow, input_builder, output_builder, **parse.proc_args())
```

### Comparing `bytewax-0.8.0_beta.2/examples/pagerank.py` & `bytewax-0.9.0/examples/pagerank.py`

 * *Files identical despite different names*

### Comparing `bytewax-0.8.0_beta.2/examples/search_session.py` & `bytewax-0.9.0/examples/search_session.py`

 * *Files identical despite different names*

### Comparing `bytewax-0.8.0_beta.2/examples/sleepyworkers.py` & `bytewax-0.9.0/examples/sleepyworkers.py`

 * *Files identical despite different names*

### Comparing `bytewax-0.8.0_beta.2/examples/subflow.py` & `bytewax-0.9.0/examples/subflow.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import collections
 import operator
 
-from bytewax import Dataflow, inp, parse, run_cluster
+from bytewax import Dataflow, inputs, parse, run_cluster
 
 
 # You can define your own functions which add groupings of steps to a
 # dataflow. This allows you to repeat a pattern of steps easily.
 def calc_counts(flow):
     """Add steps to this flow which counts the frequencies of input
     items and emits (item, count) tuples downstream."""
@@ -37,11 +37,11 @@
 # (that_same_count, num_words_with_the_same_count)
 flow.capture()
 
 
 if __name__ == "__main__":
     for epoch, item in run_cluster(
         flow,
-        inp.single_batch(open("examples/sample_data/wordcount.txt")),
+        inputs.single_batch(open("examples/sample_data/wordcount.txt")),
         **parse.cluster_args(),
     ):
         inspector(item)
```

### Comparing `bytewax-0.8.0_beta.2/examples/translator.py` & `bytewax-0.9.0/examples/translator.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import bytewax
-from bytewax import Dataflow, inp, parse, run_cluster
+from bytewax import Dataflow, inputs, parse, run_cluster
 from transformers import pipeline
 
 
 def predict(en):
     de = translator(en)[0]["translation_text"]
     return (en, de)
 
@@ -20,11 +20,11 @@
 
 
 if __name__ == "__main__":
     translator = pipeline("translation_en_to_de")
 
     for epoch, item in run_cluster(
         flow,
-        inp.single_batch(open("examples/sample_data/lyrics.txt")),
+        inputs.single_batch(open("examples/sample_data/lyrics.txt")),
         **parse.cluster_args(),
     ):
         inspector(item)
```

### Comparing `bytewax-0.8.0_beta.2/examples/twitter_stream.py` & `bytewax-0.9.0/examples/twitter_stream.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import json
 import operator
-import time
+from datetime import timedelta
 from collections import defaultdict
 
-from bytewax import Dataflow, inp, parse, run_cluster
+from bytewax import Dataflow, inputs, parse, run_cluster
 
 from utils import twitter
 
 
 def decode(x):
     try:
         return [json.loads(x)]
@@ -35,10 +35,12 @@
 flow.reduce_epoch(operator.add)
 # ("coin", count)
 flow.capture()
 
 
 if __name__ == "__main__":
     for epoch, item in run_cluster(
-        flow, inp.tumbling_epoch(2.0, twitter.get_stream()), **parse.cluster_args()
+        flow,
+        inputs.tumbling_epoch(twitter.get_stream(), timedelta(seconds=2)),
+        **parse.cluster_args()
     ):
         print(epoch, item)
```

### Comparing `bytewax-0.8.0_beta.2/examples/utils/twitter.py` & `bytewax-0.9.0/examples/utils/twitter.py`

 * *Files identical despite different names*

### Comparing `bytewax-0.8.0_beta.2/examples/wordcount.py` & `bytewax-0.9.0/examples/wordcount.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import re
 
-from bytewax import Dataflow, inp, parse, run_cluster
+from bytewax import Dataflow, parse, run_cluster
 
 
 def file_input():
     for line in open("examples/sample_data/wordcount.txt"):
         yield 1, line
```

### Comparing `bytewax-0.8.0_beta.2/pyproject.toml` & `bytewax-0.9.0/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -13,20 +13,29 @@
     "Programming Language :: Python :: Implementation :: CPython",
     "Programming Language :: Python :: Implementation :: PyPy",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Topic :: System :: Networking",
-    "Topic :: System :: Distributed Computing"
+    "Topic :: System :: Distributed Computing",
 ]
 dependencies = ["multiprocess>=0.70"]
 
 [project.urls]
 "Source Code" = "https://github.com/bytewax/bytewax"
 Issues = "https://github.com/bytewax/bytewax/issues"
 Documentation = "https://docs.bytewax.io/"
 Changelog = "https://github.com/bytewax/bytewax/blob/main/CHANGELOG.md"
 
 [metadata]
-long_description= "file: README.md"
+long_description = "file: README.md"
 long_description_content_type = "text/markdown"
+
+[tool.pytest.ini_options]
+addopts = "-v"
+doctest_optionflags = "NORMALIZE_WHITESPACE"
+testpaths = [
+    "pytests",
+    # TODO: Add back in doctests when we can figure out how to run them without import problems.
+    "docs",
+]
```

### Comparing `bytewax-0.8.0_beta.2/pysrc/bytewax/exhash.py` & `bytewax-0.9.0/pysrc/bytewax/exhash.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""`exhash` is a consistent hash that Bytewax calls internally to
+"""Exhash is a consistent hash that Bytewax calls internally to
 route data to workers.
 
 We do not use Python's `hash` because it is not consistent between
 processes by default and do not want to force modifying hash behavior
 in unrelated code via
 [`PYTHONHASHSEED`](https://docs.python.org/3/using/cmdline.html#envvar-PYTHONHASHSEED).
 
@@ -18,14 +18,19 @@
 @singledispatch
 def exhash(key, h=None):
     """A consistent hash of a value."""
     raise NotImplementedError(f"{type(key)} isn't exhash-able")
 
 
 def new_hasher():
+    """Build a new `hashlib` hasher object.
+
+    Override this if you want to use a different hashing method.
+
+    """
     return blake2b(digest_size=8)
 
 
 @exhash.register
 def _(key: list, h=None):
     raise NotImplementedError("can't exhash mutable list")
```

### Comparing `bytewax-0.8.0_beta.2/pysrc/bytewax/parse.py` & `bytewax-0.9.0/pysrc/bytewax/parse.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,30 +1,45 @@
+"""Helpers to read execution arguments from the environment or command
+line.
+
+"""
 import os
 from argparse import ArgumentParser
 from typing import Any, Dict, Iterable, List, Optional, Tuple
 
 
 def cluster_args(args: Iterable[str] = None) -> Dict[str, Any]:
     """Parse command line arguments to generate arguments for
-    `run_cluster()`
+    `bytewax.run_cluster()`.
 
-    See documentation for `run_cluster()` for semantics of these
-    variables.
+    See documentation for `bytewax.run_cluster()` for semantics of
+    these variables.
 
     >>> from bytewax import Dataflow, run_cluster
+    >>> from bytewax.testing import doctest_ctx
     >>> flow = Dataflow()
     >>> flow.capture()
     >>> args = "-w2 -n2".split()
-    >>> out = run_cluster(flow, enumerate(range(3)), **cluster_args(args))
+    >>> out = run_cluster(
+    ...     flow,
+    ...     enumerate(range(3)),
+    ...     mp_ctx=doctest_ctx,
+    ...     **cluster_args(args),
+    ... )
     >>> sorted(out)
     [(0, 0), (1, 1), (2, 2)]
 
     Args:
+
         args: List of arguments to parse. Defaults to `sys.argv`.
-    Returns: kwargs to pass to `run_cluster()`.
+
+    Returns:
+
+        kwargs to pass to `bytewax.run_cluster()`.
+
     """
     p = ArgumentParser()
     p.add_argument(
         "-w",
         dest="worker_count_per_proc",
         type=int,
         help="Number of worker threads per process",
@@ -43,21 +58,22 @@
         "proc_count": out.proc_count,
         "worker_count_per_proc": out.worker_count_per_proc,
     }
     return kwargs
 
 
 def proc_env(env: Dict[str, str] = os.environ) -> Dict[str, Any]:
-    """Parse environment variables to generate arguments for `main_proc()`
-    when you are manually launching a cluster.
+    """Parse environment variables to generate arguments for
+    `bytewax.cluster_main()` when you are manually launching a
+    cluster.
 
     This is probably what you want to use in Kubernetes.
 
-    See documentation for `main_proc()` for semantics of these
-    variables.
+    See documentation for `bytewax.cluster_main()` for semantics of
+    these variables.
 
     The environment variables you need set are:
 
     * `BYTEWAX_WORKERS_PER_PROCESS`
 
     Then either:
 
@@ -71,28 +87,37 @@
 
     * `BYTEWAX_PROCESS_ID`
 
     * `BYTEWAX_POD_NAME` and `BYTEWAX_STATEFULSET_NAME` -
       E.g. `cluster_name-0` and `cluster_name` and we will calculate
       the process ID from that.
 
-    >>> from bytewax import Dataflow, main_proc
+    >>> from bytewax import Dataflow, cluster_main, AdvanceTo, Emit
     >>> flow = Dataflow()
-    >>> ih = lambda i, n: enumerate(range(3))
-    >>> oh = lambda i, n: print
+    >>> flow.capture()
+    >>> def ib(i, n):
+    ...   for epoch, item in enumerate(range(3)):
+    ...     yield AdvanceTo(epoch)
+    ...     yield Emit(item)
+    >>> ob = lambda i, n: print
     >>> env = {
     ...     "BYTEWAX_ADDRESSES": "localhost:2101",
     ...     "BYTEWAX_PROCESS_ID": "0",
     ...     "BYTEWAX_WORKERS_PER_PROCESS": "2",
     ... }
-    >>> main_proc(flow, ih, oh, **proc_env(env))
+    >>> cluster_main(flow, ib, ob, **proc_env(env))  # doctest: +ELLIPSIS
+    (...)
 
     Args:
+
         env: Environment variables. Defaults to `os.environ`.
-    Returns: kwargs to pass to `main_proc()`.
+
+    Returns:
+
+        kwargs to pass to `bytewax.cluster_main()`.
 
     """
     if "BYTEWAX_ADDRESSES" in env:
         addresses = env["BYTEWAX_ADDRESSES"].split(";")
     else:
         with open(env["BYTEWAX_HOSTFILE_PATH"]) as hostfile:
             addresses = [
@@ -112,29 +137,40 @@
         "proc_id": proc_id,
     }
     return kwargs
 
 
 def proc_args(args: Iterable[str] = None) -> Dict[str, Any]:
     """Parse command line arguments to generate arguments for
-    `main_proc()` when you are manually launching a cluster.
+    `bytewax.cluster_main()` when you are manually launching a
+    cluster.
 
-    See documentation for `main_proc()` for semantics of these
-    variables.
+    See documentation for `bytewax.cluster_main()` for semantics of
+    these variables.
 
-    >>> from bytewax import Dataflow, main_proc
+    >>> from bytewax import Dataflow, cluster_main, AdvanceTo, Emit
     >>> flow = Dataflow()
-    >>> ih = lambda i, n: enumerate(range(3))
-    >>> oh = lambda i, n: print
+    >>> flow.capture()
+    >>> def ib(i, n):
+    ...   for epoch, item in enumerate(range(3)):
+    ...     yield AdvanceTo(epoch)
+    ...     yield Emit(item)
+    >>> ob = lambda i, n: print
     >>> args = "-w2 -p0 -a localhost:2101".split()
-    >>> main_proc(flow, ih, oh, **proc_args(args))
+    >>> cluster_main(flow, ib, ob, **proc_args(args))  # doctest: +ELLIPSIS
+    (...)
 
     Args:
+
         args: List of arguments to parse. Defaults to `sys.argv`.
-    Returns: kwargs to pass to `main_proc()`.
+
+    Returns:
+
+        kwargs to pass to `bytewax.cluster_main()`.
+
     """
     p = ArgumentParser()
     p.add_argument(
         "-w",
         dest="worker_count_per_proc",
         type=int,
         help="Number of worker threads per process",
```

### Comparing `bytewax-0.8.0_beta.2/pytests/test_exhash.py` & `bytewax-0.9.0/pytests/test_exhash.py`

 * *Files identical despite different names*

### Comparing `bytewax-0.8.0_beta.2/pytests/test_operators.py` & `bytewax-0.9.0/pytests/test_operators.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,13 @@
+import os
+
 from collections import defaultdict
 
 from bytewax import Dataflow, run, run_cluster
+from pytest import mark
 
 
 def test_map():
     def add_one(item):
         return item + 1
 
     inp = [
@@ -75,31 +78,43 @@
     ]
     seen = []
 
     flow = Dataflow()
     flow.inspect(seen.append)
     flow.capture()
 
-    run(flow, inp)
+    out = run(flow, inp)
 
+    assert sorted(out) == sorted(
+        [
+            (1, "a"),
+        ]
+    )
+    # Check side-effects after execution is complete.
     assert seen == ["a"]
 
 
 def test_inspect_epoch():
     inp = [
         (1, "a"),
     ]
     seen = []
 
     flow = Dataflow()
     flow.inspect_epoch(lambda epoch, item: seen.append((epoch, item)))
     flow.capture()
 
-    run(flow, inp)
+    out = run(flow, inp)
 
+    assert sorted(out) == sorted(
+        [
+            (1, "a"),
+        ]
+    )
+    # Check side-effects after execution is complete.
     assert seen == [(1, "a")]
 
 
 def test_reduce():
     def user_as_key(event):
         return (event["user"], [event])
 
@@ -213,15 +228,15 @@
         user, count = user_count
         epoch_user_to_count[(epoch, user)] += 1
 
     assert workers in set(epoch_user_to_count.values())
 
 
 def test_stateful_map():
-    def build_seen():
+    def build_seen(key):
         return set()
 
     def add_key(item):
         return item, item
 
     def check(seen, value):
         if value in seen:
```

### Comparing `bytewax-0.8.0_beta.2/pytests/test_parse.py` & `bytewax-0.9.0/pytests/test_parse.py`

 * *Files identical despite different names*

### Comparing `bytewax-0.8.0_beta.2/run-maturin-action.sh` & `bytewax-0.9.0/run-maturin-action.sh`

 * *Files identical despite different names*

### Comparing `bytewax-0.8.0_beta.2/src/webserver/mod.rs` & `bytewax-0.9.0/src/webserver/mod.rs`

 * *Files identical despite different names*

