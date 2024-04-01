# Comparing `tmp/morph_kgc-2.6.4.tar.gz` & `tmp/morph_kgc-2.7.0.tar.gz`

## Comparing `morph_kgc-2.6.4.tar` & `morph_kgc-2.7.0.tar`

### file list

```diff
@@ -1,1376 +1,1358 @@
--rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/.zenodo.json
--rw-r--r--   0        0        0      845 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/CITATION.cff
--rw-r--r--   0        0        0      882 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0      710 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/CONTRIBUTING.md
--rw-r--r--   0        0        0     1740 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/mkdocs.yml
--rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/readthedocs.yml
--rw-r--r--   0        0        0      454 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/.github/ISSUE_TEMPLATE/bug-report.md
--rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/.github/ISSUE_TEMPLATE/documentation-improvement.md
--rw-r--r--   0        0        0      577 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/.github/ISSUE_TEMPLATE/feature-request.md
--rw-r--r--   0        0        0      630 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/.github/ISSUE_TEMPLATE/installation-issue.md
--rw-r--r--   0        0        0      328 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/.github/ISSUE_TEMPLATE/submit-quesion.md
--rw-r--r--   0        0        0      640 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/.github/workflows/ci.yml
--rw-r--r--   0        0        0      863 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/.github/workflows/pypi-publish.yml
--rw-r--r--   0        0        0    27529 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/docs/documentation.md
--rw-r--r--   0        0        0     2599 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/docs/faq.md
--rw-r--r--   0        0        0     3944 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/docs/index.md
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/docs/requirements.txt
--rw-r--r--   0        0        0     2784 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/docs/research.md
--rw-r--r--   0        0        0     3609 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/docs/why-morph-kgc.md
--rw-r--r--   0        0        0    58421 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/docs/assets/BASF.png
--rw-r--r--   0        0        0   172672 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/docs/assets/BASF.tif
--rw-r--r--   0        0        0    44456 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/docs/assets/datos40.png
--rw-r--r--   0        0        0    40106 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/docs/assets/entente.png
--rw-r--r--   0        0        0    33187 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/docs/assets/knowledgespaces.png
--rw-r--r--   0        0        0   299520 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/docs/assets/logo-oeg.png
--rw-r--r--   0        0        0   133582 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/docs/assets/logo-upm.png
--rw-r--r--   0        0        0    50123 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/docs/assets/logo.png
--rw-r--r--   0        0        0    60779 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/docs/assets/sigtrans.png
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/docs/stylesheets/extra.css
--rw-r--r--   0        0        0     3706 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/examples/README.md
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/examples/configuration-file/basic_config.ini
--rw-r--r--   0        0        0      560 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/examples/configuration-file/default_config.ini
--rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/examples/configuration-file/oracle_config.ini
--rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/examples/csv/config.ini
--rw-r--r--   0        0        0    33628 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/examples/csv/mapping.csv.ttl
--rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/examples/csv/data/AGENCY.csv
--rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/examples/csv/data/CALENDAR.csv
--rw-r--r--   0        0        0      507 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/examples/csv/data/CALENDAR_DATES.csv
--rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/examples/csv/data/FEED_INFO.csv
--rw-r--r--   0        0        0     3503 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/examples/csv/data/FREQUENCIES.csv
--rw-r--r--   0        0        0     2924 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/examples/csv/data/ROUTES.csv
--rw-r--r--   0        0        0     3171 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/examples/csv/data/SHAPES.csv
--rw-r--r--   0        0        0     4379 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/examples/csv/data/STOPS.csv
--rw-r--r--   0        0        0     4700 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/examples/csv/data/STOP_TIMES.csv
--rw-r--r--   0        0        0     6000 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/examples/csv/data/TRIPS.csv
--rw-r--r--   0        0        0      926 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/examples/dataframe/kg_generation.py
--rw-r--r--   0        0        0     2319 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/examples/dataframe/mapping_rml.ttl
--rw-r--r--   0        0        0     1578 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/examples/dict/kg_generation.py
--rw-r--r--   0        0        0     2330 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/examples/dict/mapping_rml.ttl
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/examples/json/config.ini
--rw-r--r--   0        0        0     3464 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/examples/json/data.json
--rw-r--r--   0        0        0     9731 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/examples/json/mapping.json.ttl
--rw-r--r--   0        0        0     1791 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/examples/json/mapping.json.yaml
--rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/examples/rdb/config.ini
--rw-r--r--   0        0        0    29169 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/examples/rdb/gtfs-rdb.r2rml.ttl
--rw-r--r--   0        0        0    13238 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/examples/tutorial/Morph-KGC.ipynb
--rw-r--r--   0        0        0      327 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/examples/tutorial/README.md
--rw-r--r--   0        0        0    34542 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/examples/tutorial/mapping.gtfs.ttl
--rw-r--r--   0        0        0    26514 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/examples/tutorial/mapping.somef.ttl
--rw-r--r--   0        0        0    35086 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/examples/tutorial/oeg-upm_morph-kgc.json
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/examples/xml/config.ini
--rw-r--r--   0        0        0     3656 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/examples/xml/data.xml
--rw-r--r--   0        0        0     1756 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/examples/xml/mapping.xml.yaml
--rw-r--r--   0        0        0     9696 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/examples/xml/mappingOA.xml.ttl
--rw-r--r--   0        0        0     3056 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/src/morph_kgc/__init__.py
--rw-r--r--   0        0        0     1841 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/src/morph_kgc/__main__.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/src/morph_kgc/_version.py
--rw-r--r--   0        0        0     2205 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/src/morph_kgc/args_parser.py
--rw-r--r--   0        0        0    14497 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/src/morph_kgc/config.py
--rw-r--r--   0        0        0    11310 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/src/morph_kgc/constants.py
--rw-r--r--   0        0        0    25583 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/src/morph_kgc/materializer.py
--rw-r--r--   0        0        0     9756 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/src/morph_kgc/utils.py
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/src/morph_kgc/data_source/__init__.py
--rw-r--r--   0        0        0     8849 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/src/morph_kgc/data_source/data_file.py
--rw-r--r--   0        0        0     2563 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/src/morph_kgc/data_source/python_data.py
--rw-r--r--   0        0        0     7602 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/src/morph_kgc/data_source/relational_database.py
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/src/morph_kgc/fnml/__init__.py
--rw-r--r--   0        0        0     8530 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/src/morph_kgc/fnml/built_in_functions.py
--rw-r--r--   0        0        0     4678 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/src/morph_kgc/fnml/fnml_executer.py
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/src/morph_kgc/mapping/__init__.py
--rw-r--r--   0        0        0     6465 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/src/morph_kgc/mapping/mapping_constants.py
--rw-r--r--   0        0        0    40596 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/src/morph_kgc/mapping/mapping_parser.py
--rw-r--r--   0        0        0    20082 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/src/morph_kgc/mapping/mapping_partitioner.py
--rw-r--r--   0        0        0    31838 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/src/morph_kgc/mapping/yarrrml.py
--rw-r--r--   0        0        0     1540 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/issues/issue_118/mapping.ttl
--rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/issues/issue_118/output.nq
--rw-r--r--   0        0        0     1500 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/issues/issue_118/premis.xml
--rw-r--r--   0        0        0      689 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/issues/issue_118/test_issue_118.py
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/issues/issue_124/data.csv
--rw-r--r--   0        0        0     1724 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/issues/issue_124/mapping.ttl
--rw-r--r--   0        0        0     1136 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/issues/issue_124/output.nq
--rw-r--r--   0        0        0      758 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/issues/issue_124/test_issue_124.py
--rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/issues/issue_145/data.csv
--rw-r--r--   0        0        0     1630 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/issues/issue_145/mapping.ttl
--rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/issues/issue_145/output.nq
--rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/issues/issue_145/test_issue_145.py
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/issues/issue_174/data-1.csv
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/issues/issue_174/data-2.csv
--rw-r--r--   0        0        0     1554 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/issues/issue_174/mapping-a.ttl
--rw-r--r--   0        0        0     1431 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/issues/issue_174/mapping-b.ttl
--rw-r--r--   0        0        0     1407 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/issues/issue_174/mapping-c.ttl
--rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/issues/issue_174/output-a.nq
--rw-r--r--   0        0        0      772 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/issues/issue_174/output-b.nq
--rw-r--r--   0        0        0      684 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/issues/issue_174/output-c.nq
--rw-r--r--   0        0        0     1557 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/issues/issue_174/test_issue_174.py
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/issues/issue_62/data1.csv
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/issues/issue_62/data2.csv
--rw-r--r--   0        0        0     1043 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/issues/issue_62/mapping.ttl
--rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/issues/issue_62/output.nq
--rw-r--r--   0        0        0      709 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/issues/issue_62/test_issue_62.py
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/issues/issue_67/data.csv
--rw-r--r--   0        0        0      978 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/issues/issue_67/mapping.ttl
--rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/issues/issue_67/output.nq
--rw-r--r--   0        0        0      686 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/issues/issue_67/test_issue_67.py
--rw-r--r--   0        0        0      635 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/issues/issue_80/mapping.rml
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/issues/issue_80/output.nq
--rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/issues/issue_80/student.csv
--rw-r--r--   0        0        0      686 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/issues/issue_80/test_issue_80.py
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/issues/issue_81/country_info.csv
--rw-r--r--   0        0        0      682 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/issues/issue_81/mapping.ttl
--rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/issues/issue_81/output.nq
--rw-r--r--   0        0        0      686 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/issues/issue_81/test_issue_81.py
--rw-r--r--   0        0        0      480 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/r2rml/R2RMLTC0000/mapping.ttl
--rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/r2rml/R2RMLTC0000/output.nq
--rw-r--r--   0        0        0     8192 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/r2rml/R2RMLTC0000/resource.db
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/r2rml/R2RMLTC0000/resource.sql
--rw-r--r--   0        0        0      829 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/r2rml/R2RMLTC0000/test_R2RMLTC0000_SQLITE.py
--rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/r2rml/R2RMLTC0001a/mapping.ttl
--rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/r2rml/R2RMLTC0001a/output.nq
--rw-r--r--   0        0        0     8192 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/r2rml/R2RMLTC0001a/resource.db
--rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/r2rml/R2RMLTC0001a/resource.sql
--rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/r2rml/R2RMLTC0001a/test_R2RMLTC0001a_SQLITE.py
--rw-r--r--   0        0        0      489 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/r2rml/R2RMLTC0001b/mapping.ttl
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/r2rml/R2RMLTC0001b/output.nq
--rw-r--r--   0        0        0     8192 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/r2rml/R2RMLTC0001b/resource.db
--rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/r2rml/R2RMLTC0001b/resource.sql
--rw-r--r--   0        0        0      794 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/r2rml/R2RMLTC0001b/test_R2RMLTC0001b_SQLITE.py
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/r2rml/R2RMLTC0002a/mapping.ttl
--rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/r2rml/R2RMLTC0002a/output.nq
--rw-r--r--   0        0        0     8192 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/r2rml/R2RMLTC0002a/resource.db
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/r2rml/R2RMLTC0002a/resource.sql
--rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/r2rml/R2RMLTC0002a/test_R2RMLTC0002a_SQLITE.py
--rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/r2rml/R2RMLTC0002b/mapping.ttl
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/r2rml/R2RMLTC0002b/output.nq
--rw-r--r--   0        0        0     8192 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/r2rml/R2RMLTC0002b/resource.db
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/r2rml/R2RMLTC0002b/resource.sql
--rw-r--r--   0        0        0      764 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/r2rml/R2RMLTC0002b/test_R2RMLTC0002b_SQLITE.py
--rw-r--r--   0        0        0      481 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/r2rml/R2RMLTC0002c/mapping.ttl
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/r2rml/R2RMLTC0002c/output.nq
--rw-r--r--   0        0        0     8192 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/r2rml/R2RMLTC0002c/resource.db
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/r2rml/R2RMLTC0002c/resource.sql
--rw-r--r--   0        0        0      764 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/r2rml/R2RMLTC0002c/test_R2RMLTC0002c_SQLITE.py
--rw-r--r--   0        0        0      728 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/r2rml/R2RMLTC0002d/mapping.ttl
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/r2rml/R2RMLTC0002d/output.nq
--rw-r--r--   0        0        0     8192 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/r2rml/R2RMLTC0002d/resource.db
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/r2rml/R2RMLTC0002d/resource.sql
--rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/r2rml/R2RMLTC0002d/test_R2RMLTC0002d_SQLITE.py
--rw-r--r--   0        0        0      483 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/r2rml/R2RMLTC0002e/mapping.ttl
--rw-r--r--   0        0        0     8192 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/r2rml/R2RMLTC0002e/resource.db
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/r2rml/R2RMLTC0002e/resource.sql
--rw-r--r--   0        0        0      764 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/r2rml/R2RMLTC0002e/test_R2RMLTC0002e_SQLITE.py
--rw-r--r--   0        0        0      632 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/r2rml/R2RMLTC0002f/mapping.ttl
--rw-r--r--   0        0        0     8192 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/r2rml/R2RMLTC0002f/resource.db
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/r2rml/R2RMLTC0002f/resource.sql
--rw-r--r--   0        0        0      764 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/r2rml/R2RMLTC0002f/test_R2RMLTC0002f_SQLITE.py
--rw-r--r--   0        0        0      575 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/r2rml/R2RMLTC0002g/mapping.ttl
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/r2rml/R2RMLTC0002g/output.nq
--rw-r--r--   0        0        0     8192 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/r2rml/R2RMLTC0002g/resource.db
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/r2rml/R2RMLTC0002g/resource.sql
--rw-r--r--   0        0        0      764 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/r2rml/R2RMLTC0002g/test_R2RMLTC0002g_SQLITE.py
--rw-r--r--   0        0        0      712 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/r2rml/R2RMLTC0002h/mapping.ttl
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/r2rml/R2RMLTC0002h/output.nq
--rw-r--r--   0        0        0     8192 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/r2rml/R2RMLTC0002h/resource.db
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/r2rml/R2RMLTC0002h/resource.sql
--rw-r--r--   0        0        0      764 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/r2rml/R2RMLTC0002h/test_R2RMLTC0002h_SQLITE.py
--rw-r--r--   0        0        0      694 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/r2rml/R2RMLTC0002i/mapping.ttl
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/r2rml/R2RMLTC0002i/output.nq
--rw-r--r--   0        0        0     8192 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/r2rml/R2RMLTC0002i/resource.db
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/r2rml/R2RMLTC0002i/resource.sql
--rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/r2rml/R2RMLTC0002i/test_R2RMLTC0002i_SQLITE.py
--rw-r--r--   0        0        0      646 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/r2rml/R2RMLTC0002j/mapping.ttl
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/r2rml/R2RMLTC0002j/output.nq
--rw-r--r--   0        0        0     8192 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/r2rml/R2RMLTC0002j/resource.db
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/r2rml/R2RMLTC0002j/resource.sql
--rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/r2rml/R2RMLTC0002j/test_R2RMLTC0002j_SQLITE.py
--rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/r2rml/R2RMLTC0003a/R2RMLTC0003a_SQLITE.py
--rw-r--r--   0        0        0      711 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/r2rml/R2RMLTC0003a/mapping.ttl
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/r2rml/R2RMLTC0003a/output.nq
--rw-r--r--   0        0        0     8192 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/r2rml/R2RMLTC0003a/resource.db
--rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/r2rml/R2RMLTC0003a/resource.sql
--rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/r2rml/R2RMLTC0003b/mapping.ttl
--rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/r2rml/R2RMLTC0003b/output.nq
--rw-r--r--   0        0        0     8192 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/r2rml/R2RMLTC0003b/resource.db
--rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/r2rml/R2RMLTC0003b/resource.sql
--rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/r2rml/R2RMLTC0003b/test_R2RMLTC0003b_SQLITE.py
--rw-r--r--   0        0        0      533 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/r2rml/R2RMLTC0003c/mapping.ttl
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/r2rml/R2RMLTC0003c/output.nq
--rw-r--r--   0        0        0     8192 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/r2rml/R2RMLTC0003c/resource.db
--rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/r2rml/R2RMLTC0003c/resource.sql
--rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/r2rml/R2RMLTC0003c/test_R2RMLTC0003c_SQLITE.py
--rw-r--r--   0        0        0      839 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/r2rml/R2RMLTC0004a/mapping.ttl
--rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/r2rml/R2RMLTC0004a/output.nq
--rw-r--r--   0        0        0     8192 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/r2rml/R2RMLTC0004a/resource.db
--rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/r2rml/R2RMLTC0004a/resource.sql
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/r2rml/R2RMLTC0004a/student_sport.csv
--rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/r2rml/R2RMLTC0004a/test_R2RMLTC0004a_SQLITE.py
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/r2rml/R2RMLTC0004b/mapping.ttl
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/r2rml/R2RMLTC0004b/output.nq
--rw-r--r--   0        0        0     8192 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/r2rml/R2RMLTC0004b/resource.db
--rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/r2rml/R2RMLTC0004b/resource.sql
--rw-r--r--   0        0        0      764 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/r2rml/R2RMLTC0004b/test_R2RMLTC0004b_SQLITE.py
--rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/r2rml/R2RMLTC0005a/mapping.ttl
--rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/r2rml/R2RMLTC0005a/output.nq
--rw-r--r--   0        0        0     8192 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/r2rml/R2RMLTC0005a/resource.db
--rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/r2rml/R2RMLTC0005a/resource.sql
--rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/r2rml/R2RMLTC0005a/test_R2RMLTC0005a_SQLITE.py
--rw-r--r--   0        0        0      817 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/r2rml/R2RMLTC0005b/mapping.ttl
--rw-r--r--   0        0        0      542 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/r2rml/R2RMLTC0005b/output.nq
--rw-r--r--   0        0        0     8192 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/r2rml/R2RMLTC0005b/resource.db
--rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/r2rml/R2RMLTC0005b/resource.sql
--rw-r--r--   0        0        0      794 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/r2rml/R2RMLTC0005b/test_R2RMLTC0005b_SQLITE.py
--rw-r--r--   0        0        0      571 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/r2rml/R2RMLTC0006a/mapping.ttl
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/r2rml/R2RMLTC0006a/output.nq
--rw-r--r--   0        0        0     8192 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/r2rml/R2RMLTC0006a/resource.db
--rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/r2rml/R2RMLTC0006a/resource.sql
--rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/r2rml/R2RMLTC0006a/test_R2RMLTC0006a_SQLITE.py
--rw-r--r--   0        0        0      528 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/r2rml/R2RMLTC0007a/mapping.ttl
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/r2rml/R2RMLTC0007a/output.nq
--rw-r--r--   0        0        0     8192 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/r2rml/R2RMLTC0007a/resource.db
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/r2rml/R2RMLTC0007a/resource.sql
--rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/r2rml/R2RMLTC0007a/test_R2RMLTC0007a_SQLITE.py
--rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/r2rml/R2RMLTC0007b/mapping.ttl
--rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/r2rml/R2RMLTC0007b/output.nq
--rw-r--r--   0        0        0     8192 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/r2rml/R2RMLTC0007b/resource.db
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/r2rml/R2RMLTC0007b/resource.sql
--rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/r2rml/R2RMLTC0007b/test_R2RMLTC0007b_SQLITE.py
--rw-r--r--   0        0        0      690 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/r2rml/R2RMLTC0007c/mapping.ttl
--rw-r--r--   0        0        0      395 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/r2rml/R2RMLTC0007c/output.nq
--rw-r--r--   0        0        0     8192 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/r2rml/R2RMLTC0007c/resource.db
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/r2rml/R2RMLTC0007c/resource.sql
--rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/r2rml/R2RMLTC0007c/test_R2RMLTC0007c_SQLITE.py
--rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/r2rml/R2RMLTC0007d/mapping.ttl
--rw-r--r--   0        0        0      395 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/r2rml/R2RMLTC0007d/output.nq
--rw-r--r--   0        0        0     8192 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/r2rml/R2RMLTC0007d/resource.db
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/r2rml/R2RMLTC0007d/resource.sql
--rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/r2rml/R2RMLTC0007d/test_R2RMLTC0007d_SQLITE.py
--rw-r--r--   0        0        0      709 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/r2rml/R2RMLTC0007e/mapping.ttl
--rw-r--r--   0        0        0      419 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/r2rml/R2RMLTC0007e/output.nq
--rw-r--r--   0        0        0     8192 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/r2rml/R2RMLTC0007e/resource.db
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/r2rml/R2RMLTC0007e/resource.sql
--rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/r2rml/R2RMLTC0007e/test_R2RMLTC0007e_SQLITE.py
--rw-r--r--   0        0        0      763 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/r2rml/R2RMLTC0007f/mapping.ttl
--rw-r--r--   0        0        0      419 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/r2rml/R2RMLTC0007f/output.nq
--rw-r--r--   0        0        0     8192 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/r2rml/R2RMLTC0007f/resource.db
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/r2rml/R2RMLTC0007f/resource.sql
--rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/r2rml/R2RMLTC0007f/test_R2RMLTC0007f_SQLITE.py
--rw-r--r--   0        0        0      676 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/r2rml/R2RMLTC0007g/mapping.ttl
--rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/r2rml/R2RMLTC0007g/output.nq
--rw-r--r--   0        0        0     8192 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/r2rml/R2RMLTC0007g/resource.db
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/r2rml/R2RMLTC0007g/resource.sql
--rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/r2rml/R2RMLTC0007g/test_R2RMLTC0007g_SQLITE.py
--rw-r--r--   0        0        0      708 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/r2rml/R2RMLTC0007h/mapping.ttl
--rw-r--r--   0        0        0     8192 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/r2rml/R2RMLTC0007h/resource.db
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/r2rml/R2RMLTC0007h/resource.sql
--rw-r--r--   0        0        0      737 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/r2rml/R2RMLTC0007h/test_R2RMLTC0007h_SQLITE.py
--rw-r--r--   0        0        0      938 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/r2rml/R2RMLTC0008a/mapping.ttl
--rw-r--r--   0        0        0      672 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/r2rml/R2RMLTC0008a/output.nq
--rw-r--r--   0        0        0     8192 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/r2rml/R2RMLTC0008a/resource.db
--rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/r2rml/R2RMLTC0008a/resource.sql
--rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/r2rml/R2RMLTC0008a/test_R2RMLTC0008a_SQLITE.py
--rw-r--r--   0        0        0     1235 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/r2rml/R2RMLTC0008b/mapping.ttl
--rw-r--r--   0        0        0      541 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/r2rml/R2RMLTC0008b/output.nq
--rw-r--r--   0        0        0     8192 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/r2rml/R2RMLTC0008b/resource.db
--rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/r2rml/R2RMLTC0008b/resource.sql
--rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/r2rml/R2RMLTC0008b/test_R2RMLTC0008b_SQLITE.py
--rw-r--r--   0        0        0      568 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/r2rml/R2RMLTC0008c/mapping.ttl
--rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/r2rml/R2RMLTC0008c/output.nq
--rw-r--r--   0        0        0     8192 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/r2rml/R2RMLTC0008c/resource.db
--rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/r2rml/R2RMLTC0008c/resource.sql
--rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/r2rml/R2RMLTC0008c/test_R2RMLTC0008c_SQLITE.py
--rw-r--r--   0        0        0     1129 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/r2rml/R2RMLTC0009a/mapping.ttl
--rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/r2rml/R2RMLTC0009a/output.nq
--rw-r--r--   0        0        0    12288 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/r2rml/R2RMLTC0009a/resource.db
--rw-r--r--   0        0        0      444 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/r2rml/R2RMLTC0009a/resource.sql
--rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/r2rml/R2RMLTC0009a/test_R2RMLTC0009a_SQLITE.py
--rw-r--r--   0        0        0     1495 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/r2rml/R2RMLTC0009b/mapping.ttl
--rw-r--r--   0        0        0     1198 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/r2rml/R2RMLTC0009b/output.nq
--rw-r--r--   0        0        0    12288 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/r2rml/R2RMLTC0009b/resource.db
--rw-r--r--   0        0        0      444 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/r2rml/R2RMLTC0009b/resource.sql
--rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/r2rml/R2RMLTC0009b/test_R2RMLTC0009b_SQLITE.py
--rw-r--r--   0        0        0      647 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/r2rml/R2RMLTC0009c/mapping.ttl
--rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/r2rml/R2RMLTC0009c/output.nq
--rw-r--r--   0        0        0    12288 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/r2rml/R2RMLTC0009c/resource.db
--rw-r--r--   0        0        0      444 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/r2rml/R2RMLTC0009c/resource.sql
--rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/r2rml/R2RMLTC0009c/test_R2RMLTC0009c_SQLITE.py
--rw-r--r--   0        0        0      773 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/r2rml/R2RMLTC0009d/mapping.ttl
--rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/r2rml/R2RMLTC0009d/output.nq
--rw-r--r--   0        0        0    12288 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/r2rml/R2RMLTC0009d/resource.db
--rw-r--r--   0        0        0      444 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/r2rml/R2RMLTC0009d/resource.sql
--rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/r2rml/R2RMLTC0009d/test_R2RMLTC0009d_SQLITE.py
--rw-r--r--   0        0        0      468 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/r2rml/R2RMLTC0010a/mapping.ttl
--rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/r2rml/R2RMLTC0010a/output.nq
--rw-r--r--   0        0        0     8192 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/r2rml/R2RMLTC0010a/resource.db
--rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/r2rml/R2RMLTC0010a/resource.sql
--rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/r2rml/R2RMLTC0010a/test_R2RMLTC0010a_SQLITE.py
--rw-r--r--   0        0        0      480 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/r2rml/R2RMLTC0010b/mapping.ttl
--rw-r--r--   0        0        0      312 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/r2rml/R2RMLTC0010b/output.nq
--rw-r--r--   0        0        0     8192 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/r2rml/R2RMLTC0010b/resource.db
--rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/r2rml/R2RMLTC0010b/resource.sql
--rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/r2rml/R2RMLTC0010b/test_R2RMLTC0010b_SQLITE.py
--rw-r--r--   0        0        0      530 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/r2rml/R2RMLTC0010c/mapping.ttl
--rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/r2rml/R2RMLTC0010c/output.nq
--rw-r--r--   0        0        0     8192 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/r2rml/R2RMLTC0010c/resource.db
--rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/r2rml/R2RMLTC0010c/resource.sql
--rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/r2rml/R2RMLTC0010c/test_R2RMLTC0010c_SQLITE.py
--rw-r--r--   0        0        0     1660 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/r2rml/R2RMLTC0011a/mapping.ttl
--rw-r--r--   0        0        0     1525 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/r2rml/R2RMLTC0011a/output.nq
--rw-r--r--   0        0        0    20480 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/r2rml/R2RMLTC0011a/resource.db
--rw-r--r--   0        0        0     1143 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/r2rml/R2RMLTC0011a/resource.sql
--rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/r2rml/R2RMLTC0011a/test_R2RMLTC0011a_SQLITE.py
--rw-r--r--   0        0        0     1248 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/r2rml/R2RMLTC0011b/mapping.ttl
--rw-r--r--   0        0        0     1228 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/r2rml/R2RMLTC0011b/output.nq
--rw-r--r--   0        0        0    20480 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/r2rml/R2RMLTC0011b/resource.db
--rw-r--r--   0        0        0     1143 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/r2rml/R2RMLTC0011b/resource.sql
--rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/r2rml/R2RMLTC0011b/test_R2RMLTC0011b_SQLITE.py
--rw-r--r--   0        0        0      700 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/r2rml/R2RMLTC0012a/mapping.ttl
--rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/r2rml/R2RMLTC0012a/output.nq
--rw-r--r--   0        0        0    12288 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/r2rml/R2RMLTC0012a/resource.db
--rw-r--r--   0        0        0      680 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/r2rml/R2RMLTC0012a/resource.sql
--rw-r--r--   0        0        0      794 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/r2rml/R2RMLTC0012a/test_R2RMLTC0012a_SQLITE.py
--rw-r--r--   0        0        0      898 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/r2rml/R2RMLTC0012b/mapping.ttl
--rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/r2rml/R2RMLTC0012b/output.nq
--rw-r--r--   0        0        0    12288 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/r2rml/R2RMLTC0012b/resource.db
--rw-r--r--   0        0        0      680 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/r2rml/R2RMLTC0012b/resource.sql
--rw-r--r--   0        0        0      794 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/r2rml/R2RMLTC0012b/test_R2RMLTC0012b_SQLITE.py
--rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/r2rml/R2RMLTC0012c/mapping.ttl
--rw-r--r--   0        0        0    12288 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/r2rml/R2RMLTC0012c/resource.db
--rw-r--r--   0        0        0      680 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/r2rml/R2RMLTC0012c/resource.sql
--rw-r--r--   0        0        0      764 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/r2rml/R2RMLTC0012c/test_R2RMLTC0012c_SQLITE.py
--rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/r2rml/R2RMLTC0012d/mapping.ttl
--rw-r--r--   0        0        0    12288 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/r2rml/R2RMLTC0012d/resource.db
--rw-r--r--   0        0        0      680 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/r2rml/R2RMLTC0012d/resource.sql
--rw-r--r--   0        0        0      764 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/r2rml/R2RMLTC0012d/test_R2RMLTC0012d_SQLITE.py
--rw-r--r--   0        0        0     1500 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/r2rml/R2RMLTC0012e/mapping.ttl
--rw-r--r--   0        0        0     1252 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/r2rml/R2RMLTC0012e/output.nq
--rw-r--r--   0        0        0    12288 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/r2rml/R2RMLTC0012e/resource.db
--rw-r--r--   0        0        0      680 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/r2rml/R2RMLTC0012e/resource.sql
--rw-r--r--   0        0        0      794 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/r2rml/R2RMLTC0012e/test_R2RMLTC0012e_SQLITE.py
--rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/r2rml/R2RMLTC0013a/mapping.ttl
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/r2rml/R2RMLTC0013a/output.nq
--rw-r--r--   0        0        0     8192 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/r2rml/R2RMLTC0013a/resource.db
--rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/r2rml/R2RMLTC0013a/resource.sql
--rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/r2rml/R2RMLTC0013a/test_R2RMLTC0013a_SQLITE.py
--rw-r--r--   0        0        0      843 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/r2rml/R2RMLTC0014d/mapping.ttl
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/r2rml/R2RMLTC0014d/output.nq
--rw-r--r--   0        0        0    20480 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/r2rml/R2RMLTC0014d/resource.db
--rw-r--r--   0        0        0      775 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/r2rml/R2RMLTC0014d/resource.sql
--rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/r2rml/R2RMLTC0014d/test_R2RMLTC0014d_SQLITE.py
--rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/r2rml/R2RMLTC0015a/mapping.ttl
--rw-r--r--   0        0        0      386 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/r2rml/R2RMLTC0015a/output.nq
--rw-r--r--   0        0        0    12288 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/r2rml/R2RMLTC0015a/resource.db
--rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/r2rml/R2RMLTC0015a/resource.sql
--rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/r2rml/R2RMLTC0015a/test_R2RMLTC0015a_SQLITE.py
--rw-r--r--   0        0        0     1122 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/r2rml/R2RMLTC0015b/mapping.ttl
--rw-r--r--   0        0        0    12288 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/r2rml/R2RMLTC0015b/resource.db
--rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/r2rml/R2RMLTC0015b/resource.sql
--rw-r--r--   0        0        0      764 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/r2rml/R2RMLTC0015b/test_R2RMLTC0015b_SQLITE.py
--rw-r--r--   0        0        0      974 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/r2rml/R2RMLTC0016a/mapping.ttl
--rw-r--r--   0        0        0     1197 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/r2rml/R2RMLTC0016a/output.nq
--rw-r--r--   0        0        0     8192 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/r2rml/R2RMLTC0016a/resource.db
--rw-r--r--   0        0        0     1435 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/r2rml/R2RMLTC0016a/resource.sql
--rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/r2rml/R2RMLTC0016a/test_R2RMLTC0016a_SQLITE.py
--rw-r--r--   0        0        0      910 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/r2rml/R2RMLTC0016b/R2RMLTC0016b_SQLITE.py
--rw-r--r--   0        0        0      751 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/r2rml/R2RMLTC0016b/mapping.ttl
--rw-r--r--   0        0        0      776 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/r2rml/R2RMLTC0016b/output.nq
--rw-r--r--   0        0        0     8192 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/r2rml/R2RMLTC0016b/resource.db
--rw-r--r--   0        0        0     1435 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/r2rml/R2RMLTC0016b/resource.sql
--rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/r2rml/R2RMLTC0016c/R2RMLTC0016c_SQLITE.py
--rw-r--r--   0        0        0      769 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/r2rml/R2RMLTC0016c/mapping.ttl
--rw-r--r--   0        0        0     1110 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/r2rml/R2RMLTC0016c/output.nq
--rw-r--r--   0        0        0     8192 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/r2rml/R2RMLTC0016c/resource.db
--rw-r--r--   0        0        0     1435 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/r2rml/R2RMLTC0016c/resource.sql
--rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/r2rml/R2RMLTC0016d/R2RMLTC0016d_SQLITE.py
--rw-r--r--   0        0        0      641 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/r2rml/R2RMLTC0016d/mapping.ttl
--rw-r--r--   0        0        0      685 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/r2rml/R2RMLTC0016d/output.nq
--rw-r--r--   0        0        0     8192 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/r2rml/R2RMLTC0016d/resource.db
--rw-r--r--   0        0        0     1435 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/r2rml/R2RMLTC0016d/resource.sql
--rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/r2rml/R2RMLTC0016e/R2RMLTC0016e_SQLITE.py
--rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/r2rml/R2RMLTC0016e/mapping.ttl
--rw-r--r--   0        0        0     1110 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/r2rml/R2RMLTC0016e/output.nq
--rw-r--r--   0        0        0     8192 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/r2rml/R2RMLTC0016e/resource.db
--rw-r--r--   0        0        0     1435 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/r2rml/R2RMLTC0016e/resource.sql
--rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/r2rml/R2RMLTC0018a/mapping.ttl
--rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/r2rml/R2RMLTC0018a/output.nq
--rw-r--r--   0        0        0     8192 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/r2rml/R2RMLTC0018a/resource.db
--rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/r2rml/R2RMLTC0018a/resource.sql
--rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/r2rml/R2RMLTC0018a/test_R2RMLTC0018a_SQLITE.py
--rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/r2rml/R2RMLTC0019a/R2RMLTC0019a_SQLITE.py
--rw-r--r--   0        0        0      654 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/r2rml/R2RMLTC0019a/mapping.ttl
--rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/r2rml/R2RMLTC0019a/output.nq
--rw-r--r--   0        0        0     8192 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/r2rml/R2RMLTC0019a/resource.db
--rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/r2rml/R2RMLTC0019a/resource.sql
--rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/r2rml/R2RMLTC0019b/R2RMLTC0019b_SQLITE.py
--rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/r2rml/R2RMLTC0019b/mapping.ttl
--rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/r2rml/R2RMLTC0019b/output.nq
--rw-r--r--   0        0        0     8192 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/r2rml/R2RMLTC0019b/resource.db
--rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/r2rml/R2RMLTC0019b/resource.sql
--rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/r2rml/R2RMLTC0020a/R2RMLTC0020a_SQLITE.py
--rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/r2rml/R2RMLTC0020a/mapping.ttl
--rw-r--r--   0        0        0      658 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/r2rml/R2RMLTC0020a/output.nq
--rw-r--r--   0        0        0     8192 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/r2rml/R2RMLTC0020a/resource.db
--rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/r2rml/R2RMLTC0020a/resource.sql
--rw-r--r--   0        0        0      764 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/r2rml/R2RMLTC0020b/R2RMLTC0020b_SQLITE.py
--rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/r2rml/R2RMLTC0020b/mapping.ttl
--rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/r2rml/R2RMLTC0020b/output.nq
--rw-r--r--   0        0        0     8192 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/r2rml/R2RMLTC0020b/resource.db
--rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/r2rml/R2RMLTC0020b/resource.sql
--rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/csv/RMLTC0000/mapping.ttl
--rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/csv/RMLTC0000/output.nq
--rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/csv/RMLTC0000/student.csv
--rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/csv/RMLTC0000/test_RMLTC0000_CSV.py
--rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/csv/RMLTC0001a/mapping.ttl
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/csv/RMLTC0001a/output.nq
--rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/csv/RMLTC0001a/student.csv
--rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/csv/RMLTC0001a/test_RMLTC0001a_CSV.py
--rw-r--r--   0        0        0      648 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/csv/RMLTC0001b/mapping.ttl
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/csv/RMLTC0001b/output.nq
--rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/csv/RMLTC0001b/student.csv
--rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/csv/RMLTC0001b/test_RMLTC0001b_CSV.py
--rw-r--r--   0        0        0      754 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/csv/RMLTC0002a/mapping.ttl
--rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/csv/RMLTC0002a/output.nq
--rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/csv/RMLTC0002a/student.csv
--rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/csv/RMLTC0002a/test_RMLTC0002a_CSV.py
--rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/csv/RMLTC0002b/mapping.ttl
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/csv/RMLTC0002b/output.nq
--rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/csv/RMLTC0002b/student.csv
--rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/csv/RMLTC0002b/test_RMLTC0002b_CSV.py
--rw-r--r--   0        0        0      627 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/csv/RMLTC0002c/mapping.ttl
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/csv/RMLTC0002c/output.nq
--rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/csv/RMLTC0002c/student.csv
--rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/csv/RMLTC0002c/test_RMLTC0002c_CSV.py
--rw-r--r--   0        0        0      627 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/csv/RMLTC0002e/mapping.ttl
--rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/csv/RMLTC0002e/student.csv
--rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/csv/RMLTC0002e/test_RMLTC0002e_CSV.py
--rw-r--r--   0        0        0      689 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/csv/RMLTC0003c/mapping.ttl
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/csv/RMLTC0003c/output.nq
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/csv/RMLTC0003c/student.csv
--rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/csv/RMLTC0003c/test_RMLTC0003c_CSV.py
--rw-r--r--   0        0        0     1035 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/csv/RMLTC0004a/mapping.ttl
--rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/csv/RMLTC0004a/output.nq
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/csv/RMLTC0004a/student_sport.csv
--rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/csv/RMLTC0004a/test_RMLTC0004a_CSV.py
--rw-r--r--   0        0        0      666 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/csv/RMLTC0004b/mapping.ttl
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/csv/RMLTC0004b/output.nq
--rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/csv/RMLTC0004b/student.csv
--rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/csv/RMLTC0004b/test_RMLTC0004b_CSV.py
--rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/csv/RMLTC0005a/ious.csv
--rw-r--r--   0        0        0      659 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/csv/RMLTC0005a/mapping.ttl
--rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/csv/RMLTC0005a/output.nq
--rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/csv/RMLTC0005a/test_RMLTC0005a_CSV.py
--rw-r--r--   0        0        0      710 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/csv/RMLTC0006a/mapping.ttl
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/csv/RMLTC0006a/output.nq
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/csv/RMLTC0006a/student.csv
--rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/csv/RMLTC0006a/test_RMLTC0006a_CSV.py
--rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/csv/RMLTC0007a/mapping.ttl
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/csv/RMLTC0007a/output.nq
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/csv/RMLTC0007a/student.csv
--rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/csv/RMLTC0007a/test_RMLTC0007a_CSV.py
--rw-r--r--   0        0        0      824 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/csv/RMLTC0007b/mapping.ttl
--rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/csv/RMLTC0007b/output.nq
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/csv/RMLTC0007b/student.csv
--rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/csv/RMLTC0007b/test_RMLTC0007b_CSV.py
--rw-r--r--   0        0        0      785 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/csv/RMLTC0007c/mapping.ttl
--rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/csv/RMLTC0007c/output.nq
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/csv/RMLTC0007c/student.csv
--rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/csv/RMLTC0007c/test_RMLTC0007c_CSV.py
--rw-r--r--   0        0        0      976 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/csv/RMLTC0007d/mapping.ttl
--rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/csv/RMLTC0007d/output.nq
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/csv/RMLTC0007d/student.csv
--rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/csv/RMLTC0007d/test_RMLTC0007d_CSV.py
--rw-r--r--   0        0        0      805 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/csv/RMLTC0007e/mapping.ttl
--rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/csv/RMLTC0007e/output.nq
--rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/csv/RMLTC0007e/student.csv
--rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/csv/RMLTC0007e/test_RMLTC0007e_CSV.py
--rw-r--r--   0        0        0      923 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/csv/RMLTC0007f/mapping.ttl
--rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/csv/RMLTC0007f/output.nq
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/csv/RMLTC0007f/student.csv
--rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/csv/RMLTC0007f/test_RMLTC0007f_CSV.py
--rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/csv/RMLTC0007g/mapping.ttl
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/csv/RMLTC0007g/output.nq
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/csv/RMLTC0007g/student.csv
--rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/csv/RMLTC0007g/test_RMLTC0007g_CSV.py
--rw-r--r--   0        0        0      730 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/csv/RMLTC0007h/mapping.ttl
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/csv/RMLTC0007h/student.csv
--rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/csv/RMLTC0007h/test_RMLTC0007h_CSV.py
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/csv/RMLTC0008a/mapping.ttl
--rw-r--r--   0        0        0      627 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/csv/RMLTC0008a/output.nq
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/csv/RMLTC0008a/student.csv
--rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/csv/RMLTC0008a/test_RMLTC0008a_CSV.py
--rw-r--r--   0        0        0     1410 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/csv/RMLTC0008b/mapping.ttl
--rw-r--r--   0        0        0      544 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/csv/RMLTC0008b/output.nq
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/csv/RMLTC0008b/student.csv
--rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/csv/RMLTC0008b/test_RMLTC0008b_CSV.py
--rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/csv/RMLTC0008c/mapping.ttl
--rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/csv/RMLTC0008c/output.nq
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/csv/RMLTC0008c/student.csv
--rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/csv/RMLTC0008c/test_RMLTC0008c_CSV.py
--rw-r--r--   0        0        0     1344 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/csv/RMLTC0009a/mapping.ttl
--rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/csv/RMLTC0009a/output.nq
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/csv/RMLTC0009a/sport.csv
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/csv/RMLTC0009a/student.csv
--rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/csv/RMLTC0009a/test_RMLTC0009a_CSV.py
--rw-r--r--   0        0        0     1665 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/csv/RMLTC0009b/mapping.ttl
--rw-r--r--   0        0        0     1198 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/csv/RMLTC0009b/output.nq
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/csv/RMLTC0009b/sport.csv
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/csv/RMLTC0009b/student.csv
--rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/csv/RMLTC0009b/test_RMLTC0009b_CSV.py
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/csv/RMLTC0010a/country_info.csv
--rw-r--r--   0        0        0      685 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/csv/RMLTC0010a/mapping.ttl
--rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/csv/RMLTC0010a/output.nq
--rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/csv/RMLTC0010a/test_RMLTC0010a_CSV.py
--rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/csv/RMLTC0010b/country_info.csv
--rw-r--r--   0        0        0      692 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/csv/RMLTC0010b/mapping.ttl
--rw-r--r--   0        0        0      312 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/csv/RMLTC0010b/output.nq
--rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/csv/RMLTC0010b/test_RMLTC0010b_CSV.py
--rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/csv/RMLTC0010c/country_info.csv
--rw-r--r--   0        0        0      739 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/csv/RMLTC0010c/mapping.ttl
--rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/csv/RMLTC0010c/output.nq
--rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/csv/RMLTC0010c/test_RMLTC0010c_CSV.py
--rw-r--r--   0        0        0     1605 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/csv/RMLTC0011b/mapping.ttl
--rw-r--r--   0        0        0     1229 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/csv/RMLTC0011b/output.nq
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/csv/RMLTC0011b/sport.csv
--rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/csv/RMLTC0011b/student.csv
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/csv/RMLTC0011b/student_sport.csv
--rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/csv/RMLTC0011b/test_RMLTC0011b_CSV.py
--rw-r--r--   0        0        0      817 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/csv/RMLTC0012a/mapping.ttl
--rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/csv/RMLTC0012a/output.nq
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/csv/RMLTC0012a/persons.csv
--rw-r--r--   0        0        0      652 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/csv/RMLTC0012a/test_RMLTC0012a_CSV.py
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/csv/RMLTC0012b/lives.csv
--rw-r--r--   0        0        0     1058 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/csv/RMLTC0012b/mapping.ttl
--rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/csv/RMLTC0012b/output.nq
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/csv/RMLTC0012b/persons.csv
--rw-r--r--   0        0        0      652 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/csv/RMLTC0012b/test_RMLTC0012b_CSV.py
--rw-r--r--   0        0        0      731 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/csv/RMLTC0012c/mapping.ttl
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/csv/RMLTC0012c/persons.csv
--rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/csv/RMLTC0012c/test_RMLTC0012c_CSV.py
--rw-r--r--   0        0        0      907 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/csv/RMLTC0012d/mapping.ttl
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/csv/RMLTC0012d/persons.csv
--rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/csv/RMLTC0012d/test_RMLTC0012d_CSV.py
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/csv/RMLTC0015a/country_en.csv
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/csv/RMLTC0015a/country_es.csv
--rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/csv/RMLTC0015a/mapping.ttl
--rw-r--r--   0        0        0      386 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/csv/RMLTC0015a/output.nq
--rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/csv/RMLTC0015a/test_RMLTC0015a_CSV.py
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/csv/RMLTC0015b/country_en.csv
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/csv/RMLTC0015b/country_es.csv
--rw-r--r--   0        0        0     1081 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/csv/RMLTC0015b/mapping.ttl
--rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/csv/RMLTC0015b/test_RMLTC0015b_CSV.py
--rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/csv/RMLTC0019a/RMLTC0019a_CSV.py
--rw-r--r--   0        0        0      680 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/csv/RMLTC0019a/mapping.ttl
--rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/csv/RMLTC0019a/output.nq
--rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/csv/RMLTC0019a/persons.csv
--rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/csv/RMLTC0019b/RMLTC0019b_CSV.py
--rw-r--r--   0        0        0      680 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/csv/RMLTC0019b/mapping.ttl
--rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/csv/RMLTC0019b/output.nq
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/csv/RMLTC0019b/persons.csv
--rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/csv/RMLTC0020a/RMLTC0020a_CSV.py
--rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/csv/RMLTC0020a/mapping.ttl
--rw-r--r--   0        0        0      658 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/csv/RMLTC0020a/output.nq
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/csv/RMLTC0020a/student.csv
--rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/csv/RMLTC0020b/RMLTC0020b_CSV.py
--rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/csv/RMLTC0020b/mapping.ttl
--rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/csv/RMLTC0020b/output.nq
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/csv/RMLTC0020b/student.csv
--rw-r--r--   0        0        0      755 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/csv/null_filter/mapping.ttl
--rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/csv/null_filter/output.nq
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/csv/null_filter/student.csv
--rw-r--r--   0        0        0      689 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/csv/null_filter/test_null_filter_CSV.py
--rw-r--r--   0        0        0     1161 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/csv/triples_map_without_pom/mapping.ttl
--rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/csv/triples_map_without_pom/output.nq
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/csv/triples_map_without_pom/sport.csv
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/csv/triples_map_without_pom/student.csv
--rw-r--r--   0        0        0      701 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/csv/triples_map_without_pom/test_triples_map_without_pom_CSV.py
--rw-r--r--   0        0        0      680 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/json/RMLTC0000/mapping.ttl
--rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/json/RMLTC0000/output.nq
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/json/RMLTC0000/student.json
--rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/json/RMLTC0000/test_RMLTC0000_JSON.py
--rw-r--r--   0        0        0      709 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/json/RMLTC0001a/mapping.ttl
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/json/RMLTC0001a/output.nq
--rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/json/RMLTC0001a/student.json
--rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/json/RMLTC0001a/test_RMLTC0001a_JSON.py
--rw-r--r--   0        0        0      689 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/json/RMLTC0001b/mapping.ttl
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/json/RMLTC0001b/output.nq
--rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/json/RMLTC0001b/student.json
--rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/json/RMLTC0001b/test_RMLTC0001b_JSON.py
--rw-r--r--   0        0        0      795 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/json/RMLTC0002a/mapping.ttl
--rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/json/RMLTC0002a/output.nq
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/json/RMLTC0002a/student.json
--rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/json/RMLTC0002a/test_RMLTC0002a_JSON.py
--rw-r--r--   0        0        0      683 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/json/RMLTC0002b/mapping.ttl
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/json/RMLTC0002b/output.nq
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/json/RMLTC0002b/student.json
--rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/json/RMLTC0002b/test_RMLTC0002b_JSON.py
--rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/json/RMLTC0002c/mapping.ttl
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/json/RMLTC0002c/output.nq
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/json/RMLTC0002c/student.json
--rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/json/RMLTC0002c/test_RMLTC0002c_JSON.py
--rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/json/RMLTC0002e/mapping.ttl
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/json/RMLTC0002e/student.json
--rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/json/RMLTC0002e/test_RMLTC0002e_JSON.py
--rw-r--r--   0        0        0      730 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/json/RMLTC0003c/mapping.ttl
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/json/RMLTC0003c/output.nq
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/json/RMLTC0003c/student.json
--rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/json/RMLTC0003c/test_RMLTC0003c_JSON.py
--rw-r--r--   0        0        0     1117 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/json/RMLTC0004a/mapping.ttl
--rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/json/RMLTC0004a/output.nq
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/json/RMLTC0004a/student_sport.json
--rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/json/RMLTC0004a/test_RMLTC0004a_JSON.py
--rw-r--r--   0        0        0      707 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/json/RMLTC0004b/mapping.ttl
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/json/RMLTC0004b/output.nq
--rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/json/RMLTC0004b/student.json
--rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/json/RMLTC0004b/test_RMLTC0004b_JSON.py
--rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/json/RMLTC0005a/ious.json
--rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/json/RMLTC0005a/mapping.ttl
--rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/json/RMLTC0005a/output.nq
--rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/json/RMLTC0005a/test_RMLTC0005a_JSON.py
--rw-r--r--   0        0        0      751 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/json/RMLTC0006a/mapping.ttl
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/json/RMLTC0006a/output.nq
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/json/RMLTC0006a/student.json
--rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/json/RMLTC0006a/test_RMLTC0006a_JSON.py
--rw-r--r--   0        0        0      729 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/json/RMLTC0007a/mapping.ttl
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/json/RMLTC0007a/output.nq
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/json/RMLTC0007a/student.json
--rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/json/RMLTC0007a/test_RMLTC0007a_JSON.py
--rw-r--r--   0        0        0      865 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/json/RMLTC0007b/mapping.ttl
--rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/json/RMLTC0007b/output.nq
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/json/RMLTC0007b/student.json
--rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/json/RMLTC0007b/test_RMLTC0007b_JSON.py
--rw-r--r--   0        0        0      826 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/json/RMLTC0007c/mapping.ttl
--rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/json/RMLTC0007c/output.nq
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/json/RMLTC0007c/student.json
--rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/json/RMLTC0007c/test_RMLTC0007c_JSON.py
--rw-r--r--   0        0        0     1015 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/json/RMLTC0007d/mapping.ttl
--rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/json/RMLTC0007d/output.nq
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/json/RMLTC0007d/student.json
--rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/json/RMLTC0007d/test_RMLTC0007d_JSON.py
--rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/json/RMLTC0007e/mapping.ttl
--rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/json/RMLTC0007e/output.nq
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/json/RMLTC0007e/student.json
--rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/json/RMLTC0007e/test_RMLTC0007e_JSON.py
--rw-r--r--   0        0        0      964 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/json/RMLTC0007f/mapping.ttl
--rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/json/RMLTC0007f/output.nq
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/json/RMLTC0007f/student.json
--rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/json/RMLTC0007f/test_RMLTC0007f_JSON.py
--rw-r--r--   0        0        0      729 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/json/RMLTC0007g/mapping.ttl
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/json/RMLTC0007g/output.nq
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/json/RMLTC0007g/student.json
--rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/json/RMLTC0007g/test_RMLTC0007g_JSON.py
--rw-r--r--   0        0        0      771 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/json/RMLTC0007h/mapping.ttl
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/json/RMLTC0007h/student.json
--rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/json/RMLTC0007h/test_RMLTC0007h_JSON.py
--rw-r--r--   0        0        0     1111 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/json/RMLTC0008a/mapping.ttl
--rw-r--r--   0        0        0      627 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/json/RMLTC0008a/output.nq
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/json/RMLTC0008a/student.json
--rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/json/RMLTC0008a/test_RMLTC0008a_JSON.py
--rw-r--r--   0        0        0     1492 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/json/RMLTC0008b/mapping.ttl
--rw-r--r--   0        0        0      544 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/json/RMLTC0008b/output.nq
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/json/RMLTC0008b/student.json
--rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/json/RMLTC0008b/test_RMLTC0008b_JSON.py
--rw-r--r--   0        0        0      755 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/json/RMLTC0008c/mapping.ttl
--rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/json/RMLTC0008c/output.nq
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/json/RMLTC0008c/student.json
--rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/json/RMLTC0008c/test_RMLTC0008c_JSON.py
--rw-r--r--   0        0        0     1424 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/json/RMLTC0009a/mapping.ttl
--rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/json/RMLTC0009a/output.nq
--rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/json/RMLTC0009a/sport.json
--rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/json/RMLTC0009a/student.json
--rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/json/RMLTC0009a/test_RMLTC0009a_JSON.py
--rw-r--r--   0        0        0     1735 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/json/RMLTC0009b/mapping.ttl
--rw-r--r--   0        0        0     1198 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/json/RMLTC0009b/output.nq
--rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/json/RMLTC0009b/sport.json
--rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/json/RMLTC0009b/student.json
--rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/json/RMLTC0009b/test_RMLTC0009b_JSON.py
--rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/json/RMLTC0010a/country_info.json
--rw-r--r--   0        0        0      727 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/json/RMLTC0010a/mapping.ttl
--rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/json/RMLTC0010a/output.nq
--rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/json/RMLTC0010a/test_RMLTC0010a_JSON.py
--rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/json/RMLTC0010b/country_info.json
--rw-r--r--   0        0        0      734 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/json/RMLTC0010b/mapping.ttl
--rw-r--r--   0        0        0      312 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/json/RMLTC0010b/output.nq
--rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/json/RMLTC0010b/test_RMLTC0010b_JSON.py
--rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/json/RMLTC0010c/country_info.json
--rw-r--r--   0        0        0      781 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/json/RMLTC0010c/mapping.ttl
--rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/json/RMLTC0010c/output.nq
--rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/json/RMLTC0010c/test_RMLTC0010c_JSON.py
--rw-r--r--   0        0        0     1723 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/json/RMLTC0011b/mapping.ttl
--rw-r--r--   0        0        0     1229 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/json/RMLTC0011b/output.nq
--rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/json/RMLTC0011b/sport.json
--rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/json/RMLTC0011b/student.json
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/json/RMLTC0011b/student_sport.json
--rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/json/RMLTC0011b/test_RMLTC0011b_JSON.py
--rw-r--r--   0        0        0      857 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/json/RMLTC0012a/mapping.ttl
--rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/json/RMLTC0012a/output.nq
--rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/json/RMLTC0012a/persons.json
--rw-r--r--   0        0        0      652 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/json/RMLTC0012a/test_RMLTC0012a_JSON.py
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/json/RMLTC0012b/lives.json
--rw-r--r--   0        0        0     1136 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/json/RMLTC0012b/mapping.ttl
--rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/json/RMLTC0012b/output.nq
--rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/json/RMLTC0012b/persons.json
--rw-r--r--   0        0        0      652 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/json/RMLTC0012b/test_RMLTC0012b_JSON.py
--rw-r--r--   0        0        0      771 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/json/RMLTC0012c/mapping.ttl
--rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/json/RMLTC0012c/persons.json
--rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/json/RMLTC0012c/test_RMLTC0012c_JSON.py
--rw-r--r--   0        0        0      947 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/json/RMLTC0012d/mapping.ttl
--rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/json/RMLTC0012d/persons.json
--rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/json/RMLTC0012d/test_RMLTC0012d_JSON.py
--rw-r--r--   0        0        0      709 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/json/RMLTC0013a/mapping.ttl
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/json/RMLTC0013a/output.nq
--rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/json/RMLTC0013a/persons.json
--rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/json/RMLTC0013a/test_RMLTC0013a_JSON.py
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/json/RMLTC0015a/country_en.json
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/json/RMLTC0015a/country_es.json
--rw-r--r--   0        0        0     1167 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/json/RMLTC0015a/mapping.ttl
--rw-r--r--   0        0        0      386 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/json/RMLTC0015a/output.nq
--rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/json/RMLTC0015a/test_RMLTC0015a_JSON.py
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/json/RMLTC0015b/country_en.json
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/json/RMLTC0015b/country_es.json
--rw-r--r--   0        0        0     1165 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/json/RMLTC0015b/mapping.ttl
--rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/json/RMLTC0015b/test_RMLTC0015b_JSON.py
--rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/json/RMLTC0019a/RMLTC0019a_JSON.py
--rw-r--r--   0        0        0      720 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/json/RMLTC0019a/mapping.ttl
--rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/json/RMLTC0019a/output.nq
--rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/json/RMLTC0019a/persons.json
--rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/json/RMLTC0019b/RMLTC0019b_JSON.py
--rw-r--r--   0        0        0      720 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/json/RMLTC0019b/mapping.ttl
--rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/json/RMLTC0019b/output.nq
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/json/RMLTC0019b/persons.json
--rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/json/RMLTC0020a/RMLTC0020a_JSON.py
--rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/json/RMLTC0020a/mapping.ttl
--rw-r--r--   0        0        0      658 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/json/RMLTC0020a/output.nq
--rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/json/RMLTC0020a/student.json
--rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/json/RMLTC0020b/RMLTC0020b_JSON.py
--rw-r--r--   0        0        0      728 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/json/RMLTC0020b/mapping.ttl
--rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/json/RMLTC0020b/output.nq
--rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/json/RMLTC0020b/student.json
--rw-r--r--   0        0        0     3464 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/json/complex/data.json
--rw-r--r--   0        0        0     9797 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/json/complex/mapping.ttl
--rw-r--r--   0        0        0     1791 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/json/complex/mapping.yaml
--rw-r--r--   0        0        0     3729 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/json/complex/output.nq
--rw-r--r--   0        0        0     2021 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/json/complex/test_complex_JSON.py
--rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/tabular/RMLTC0002a_EXCEL/mapping.ttl
--rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/tabular/RMLTC0002a_EXCEL/output.nq
--rw-r--r--   0        0        0     4925 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/tabular/RMLTC0002a_EXCEL/student.xlsx
--rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/tabular/RMLTC0002a_EXCEL/test_RMLTC0002a_EXCEL.py
--rw-r--r--   0        0        0      770 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/tabular/RMLTC0002a_FEATHER/mapping.ttl
--rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/tabular/RMLTC0002a_FEATHER/output.nq
--rw-r--r--   0        0        0     1538 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/tabular/RMLTC0002a_FEATHER/student.feather
--rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/tabular/RMLTC0002a_FEATHER/test_RMLTC0002a_FEATHER.py
--rw-r--r--   0        0        0      762 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/tabular/RMLTC0002a_ODS/mapping.ttl
--rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/tabular/RMLTC0002a_ODS/output.nq
--rw-r--r--   0        0        0     5269 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/tabular/RMLTC0002a_ODS/student.ods
--rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/tabular/RMLTC0002a_ODS/test_RMLTC0002a_ODS.py
--rw-r--r--   0        0        0      770 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/tabular/RMLTC0002a_PARQUET/mapping.ttl
--rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/tabular/RMLTC0002a_PARQUET/output.nq
--rw-r--r--   0        0        0     1746 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/tabular/RMLTC0002a_PARQUET/student.parquet
--rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/tabular/RMLTC0002a_PARQUET/test_RMLTC0002a_PARQUET.py
--rw-r--r--   0        0        0      764 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/tabular/RMLTC0002a_STATA/mapping.ttl
--rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/tabular/RMLTC0002a_STATA/output.nq
--rw-r--r--   0        0        0     1844 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/tabular/RMLTC0002a_STATA/student.dta
--rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/tabular/RMLTC0002a_STATA/test_RMLTC0002a_STATA.py
--rw-r--r--   0        0        0      762 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/tabular/RMLTC0002a_TSV/mapping.ttl
--rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/tabular/RMLTC0002a_TSV/output.nq
--rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/tabular/RMLTC0002a_TSV/student.tsv
--rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/tabular/RMLTC0002a_TSV/test_RMLTC0002a_TSV.py
--rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/xml/RMLTC0000/mapping.ttl
--rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/xml/RMLTC0000/output.nq
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/xml/RMLTC0000/student.xml
--rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/xml/RMLTC0000/test_RMLTC0000_XML.py
--rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/xml/RMLTC0001a/mapping.ttl
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/xml/RMLTC0001a/output.nq
--rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/xml/RMLTC0001a/student.xml
--rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/xml/RMLTC0001a/test_RMLTC0001a_XML.py
--rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/xml/RMLTC0001b/mapping.ttl
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/xml/RMLTC0001b/output.nq
--rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/xml/RMLTC0001b/student.xml
--rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/xml/RMLTC0001b/test_RMLTC0001b_XML.py
--rw-r--r--   0        0        0      794 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/xml/RMLTC0002a/mapping.ttl
--rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/xml/RMLTC0002a/output.nq
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/xml/RMLTC0002a/student.xml
--rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/xml/RMLTC0002a/test_RMLTC0002a_XML.py
--rw-r--r--   0        0        0      682 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/xml/RMLTC0002b/mapping.ttl
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/xml/RMLTC0002b/output.nq
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/xml/RMLTC0002b/student.xml
--rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/xml/RMLTC0002b/test_RMLTC0002b_XML.py
--rw-r--r--   0        0        0      667 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/xml/RMLTC0002c/mapping.ttl
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/xml/RMLTC0002c/output.nq
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/xml/RMLTC0002c/student.xml
--rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/xml/RMLTC0002c/test_RMLTC0002c_XML.py
--rw-r--r--   0        0        0      667 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/xml/RMLTC0002e/mapping.ttl
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/xml/RMLTC0002e/student.xml
--rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/xml/RMLTC0002e/test_RMLTC0002e_XML.py
--rw-r--r--   0        0        0      728 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/xml/RMLTC0003c/mapping.ttl
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/xml/RMLTC0003c/output.nq
--rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/xml/RMLTC0003c/student.xml
--rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/xml/RMLTC0003c/test_RMLTC0003c_XML.py
--rw-r--r--   0        0        0     1115 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/xml/RMLTC0004a/mapping.ttl
--rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/xml/RMLTC0004a/output.nq
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/xml/RMLTC0004a/student_sport.xml
--rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/xml/RMLTC0004a/test_RMLTC0004a_XML.py
--rw-r--r--   0        0        0      706 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/xml/RMLTC0004b/mapping.ttl
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/xml/RMLTC0004b/output.nq
--rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/xml/RMLTC0004b/student.xml
--rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/xml/RMLTC0004b/test_RMLTC0004b_XML.py
--rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/xml/RMLTC0005a/ious.xml
--rw-r--r--   0        0        0      697 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/xml/RMLTC0005a/mapping.ttl
--rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/xml/RMLTC0005a/output.nq
--rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/xml/RMLTC0005a/test_RMLTC0005a_XML.py
--rw-r--r--   0        0        0      750 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/xml/RMLTC0006a/mapping.ttl
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/xml/RMLTC0006a/output.nq
--rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/xml/RMLTC0006a/student.xml
--rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/xml/RMLTC0006a/test_RMLTC0006a_XML.py
--rw-r--r--   0        0        0      728 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/xml/RMLTC0007a/mapping.ttl
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/xml/RMLTC0007a/output.nq
--rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/xml/RMLTC0007a/student.xml
--rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/xml/RMLTC0007a/test_RMLTC0007a_XML.py
--rw-r--r--   0        0        0      864 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/xml/RMLTC0007b/mapping.ttl
--rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/xml/RMLTC0007b/output.nq
--rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/xml/RMLTC0007b/student.xml
--rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/xml/RMLTC0007b/test_RMLTC0007b_XML.py
--rw-r--r--   0        0        0      825 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/xml/RMLTC0007c/mapping.ttl
--rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/xml/RMLTC0007c/output.nq
--rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/xml/RMLTC0007c/student.xml
--rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/xml/RMLTC0007c/test_RMLTC0007c_XML.py
--rw-r--r--   0        0        0     1014 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/xml/RMLTC0007d/mapping.ttl
--rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/xml/RMLTC0007d/output.nq
--rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/xml/RMLTC0007d/student.xml
--rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/xml/RMLTC0007d/test_RMLTC0007d_XML.py
--rw-r--r--   0        0        0      845 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/xml/RMLTC0007e/mapping.ttl
--rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/xml/RMLTC0007e/output.nq
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/xml/RMLTC0007e/student.xml
--rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/xml/RMLTC0007e/test_RMLTC0007e_XML.py
--rw-r--r--   0        0        0      963 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/xml/RMLTC0007f/mapping.ttl
--rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/xml/RMLTC0007f/output.nq
--rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/xml/RMLTC0007f/student.xml
--rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/xml/RMLTC0007f/test_RMLTC0007f_XML.py
--rw-r--r--   0        0        0      728 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/xml/RMLTC0007g/mapping.ttl
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/xml/RMLTC0007g/output.nq
--rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/xml/RMLTC0007g/student.xml
--rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/xml/RMLTC0007g/test_RMLTC0007g_XML.py
--rw-r--r--   0        0        0      770 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/xml/RMLTC0007h/mapping.ttl
--rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/xml/RMLTC0007h/student.xml
--rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/xml/RMLTC0007h/test_RMLTC0007h_XML.py
--rw-r--r--   0        0        0     1110 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/xml/RMLTC0008a/mapping.ttl
--rw-r--r--   0        0        0      627 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/xml/RMLTC0008a/output.nq
--rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/xml/RMLTC0008a/student.xml
--rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/xml/RMLTC0008a/test_RMLTC0008a_XML.py
--rw-r--r--   0        0        0     1490 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/xml/RMLTC0008b/mapping.ttl
--rw-r--r--   0        0        0      544 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/xml/RMLTC0008b/output.nq
--rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/xml/RMLTC0008b/student.xml
--rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/xml/RMLTC0008b/test_RMLTC0008b_XML.py
--rw-r--r--   0        0        0      754 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/xml/RMLTC0008c/mapping.ttl
--rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/xml/RMLTC0008c/output.nq
--rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/xml/RMLTC0008c/student.xml
--rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/xml/RMLTC0008c/test_RMLTC0008c_XML.py
--rw-r--r--   0        0        0     1420 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/xml/RMLTC0009a/mapping.ttl
--rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/xml/RMLTC0009a/output.nq
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/xml/RMLTC0009a/sport.xml
--rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/xml/RMLTC0009a/student.xml
--rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/xml/RMLTC0009a/test_RMLTC0009a_XML.py
--rw-r--r--   0        0        0     1740 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/xml/RMLTC0009b/mapping.ttl
--rw-r--r--   0        0        0     1198 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/xml/RMLTC0009b/output.nq
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/xml/RMLTC0009b/sport.xml
--rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/xml/RMLTC0009b/student.xml
--rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/xml/RMLTC0009b/test_RMLTC0009b_XML.py
--rw-r--r--   0        0        0      419 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/xml/RMLTC0010b/country_info.xml
--rw-r--r--   0        0        0      732 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/xml/RMLTC0010b/mapping.ttl
--rw-r--r--   0        0        0      312 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/xml/RMLTC0010b/output.nq
--rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/xml/RMLTC0010b/test_RMLTC0010b_XML.py
--rw-r--r--   0        0        0      419 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/xml/RMLTC0010c/country_info.xml
--rw-r--r--   0        0        0      778 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/xml/RMLTC0010c/mapping.ttl
--rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/xml/RMLTC0010c/output.nq
--rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/xml/RMLTC0010c/test_RMLTC0010c_XML.py
--rw-r--r--   0        0        0     1715 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/xml/RMLTC0011b/mapping.ttl
--rw-r--r--   0        0        0     1229 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/xml/RMLTC0011b/output.nq
--rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/xml/RMLTC0011b/sport.xml
--rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/xml/RMLTC0011b/student.xml
--rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/xml/RMLTC0011b/student_sport.xml
--rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/xml/RMLTC0011b/test_RMLTC0011b_XML.py
--rw-r--r--   0        0        0      855 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/xml/RMLTC0012a/mapping.ttl
--rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/xml/RMLTC0012a/output.nq
--rw-r--r--   0        0        0      329 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/xml/RMLTC0012a/persons.xml
--rw-r--r--   0        0        0      652 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/xml/RMLTC0012a/test_RMLTC0012a_XML.py
--rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/xml/RMLTC0012b/lives.xml
--rw-r--r--   0        0        0     1132 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/xml/RMLTC0012b/mapping.ttl
--rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/xml/RMLTC0012b/output.nq
--rw-r--r--   0        0        0      329 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/xml/RMLTC0012b/persons.xml
--rw-r--r--   0        0        0      652 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/xml/RMLTC0012b/test_RMLTC0012b_XML.py
--rw-r--r--   0        0        0      769 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/xml/RMLTC0012c/mapping.ttl
--rw-r--r--   0        0        0      332 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/xml/RMLTC0012c/persons.xml
--rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/xml/RMLTC0012c/test_RMLTC0012c_XML.py
--rw-r--r--   0        0        0      945 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/xml/RMLTC0012d/mapping.ttl
--rw-r--r--   0        0        0      332 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/xml/RMLTC0012d/persons.xml
--rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/xml/RMLTC0012d/test_RMLTC0012d_XML.py
--rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/xml/RMLTC0015a/country_en.xml
--rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/xml/RMLTC0015a/country_es.xml
--rw-r--r--   0        0        0     1165 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/xml/RMLTC0015a/mapping.ttl
--rw-r--r--   0        0        0      386 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/xml/RMLTC0015a/output.nq
--rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/xml/RMLTC0015a/test_RMLTC0015a_XML.py
--rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/xml/RMLTC0015b/country_en.xml
--rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/xml/RMLTC0015b/country_es.xml
--rw-r--r--   0        0        0     1163 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/xml/RMLTC0015b/mapping.ttl
--rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/xml/RMLTC0015b/test_RMLTC0015b_XML.py
--rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/xml/RMLTC0019a/RMLTC0019a_XML.py
--rw-r--r--   0        0        0      718 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/xml/RMLTC0019a/mapping.ttl
--rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/xml/RMLTC0019a/output.nq
--rw-r--r--   0        0        0      306 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/xml/RMLTC0019a/persons.xml
--rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/xml/RMLTC0019b/RMLTC0019b_XML.py
--rw-r--r--   0        0        0      718 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/xml/RMLTC0019b/mapping.ttl
--rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/xml/RMLTC0019b/output.nq
--rw-r--r--   0        0        0      432 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/xml/RMLTC0019b/persons.xml
--rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/xml/RMLTC0020a/RMLTC0020a_XML.py
--rw-r--r--   0        0        0      754 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/xml/RMLTC0020a/mapping.ttl
--rw-r--r--   0        0        0      658 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/xml/RMLTC0020a/output.nq
--rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/xml/RMLTC0020a/student.xml
--rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/xml/RMLTC0020b/RMLTC0020b_XML.py
--rw-r--r--   0        0        0      727 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/xml/RMLTC0020b/mapping.ttl
--rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/xml/RMLTC0020b/output.nq
--rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/xml/RMLTC0020b/student.xml
--rw-r--r--   0        0        0      859 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/xml/attributes/data.xml
--rw-r--r--   0        0        0     1516 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/xml/attributes/mapping.ttl
--rw-r--r--   0        0        0     1532 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/xml/attributes/output.nq
--rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/xml/attributes/test_attributes_XML.py
--rw-r--r--   0        0        0     3656 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/xml/complex/data.xml
--rw-r--r--   0        0        0     9759 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/xml/complex/mapping.ttl
--rw-r--r--   0        0        0     1756 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/xml/complex/mapping.yaml
--rw-r--r--   0        0        0     4539 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/xml/complex/output.nq
--rw-r--r--   0        0        0     2020 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/xml/complex/test_complex_XML.py
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/xml/rml_spec_example_section_3/Transport.xml
--rw-r--r--   0        0        0      980 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/xml/rml_spec_example_section_3/mapping.ttl
--rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/xml/rml_spec_example_section_3/output.nq
--rw-r--r--   0        0        0      704 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/xml/rml_spec_example_section_3/test_rml_spec_example_section_3_XML.py
--rw-r--r--   0        0        0      435 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/xml/rml_spec_example_section_5/Transport.xml
--rw-r--r--   0        0        0      776 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/xml/rml_spec_example_section_5/mapping.ttl
--rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/xml/rml_spec_example_section_5/output.nq
--rw-r--r--   0        0        0      704 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml/xml/rml_spec_example_section_5/test_rml_spec_example_section_5_XML.py
--rw-r--r--   0        0        0      900 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-fnml/RMLFNOTC0000-CSV/mapping.ttl
--rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-fnml/RMLFNOTC0000-CSV/output.nq
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-fnml/RMLFNOTC0000-CSV/student.csv
--rw-r--r--   0        0        0      841 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-fnml/RMLFNOTC0000-CSV/test_RMLFNOTC0000-CSV.py
--rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-fnml/RMLFNOTC0001-CSV/mapping.ttl
--rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-fnml/RMLFNOTC0001-CSV/output.nq
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-fnml/RMLFNOTC0001-CSV/student.csv
--rw-r--r--   0        0        0      694 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-fnml/RMLFNOTC0001-CSV/test_RMLFNOTC0001-CSV.py
--rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-fnml/RMLFNOTC0002-CSV/mapping.ttl
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-fnml/RMLFNOTC0002-CSV/output.nq
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-fnml/RMLFNOTC0002-CSV/student.csv
--rw-r--r--   0        0        0      694 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-fnml/RMLFNOTC0002-CSV/test_RMLFNOTC0002-CSV.py
--rw-r--r--   0        0        0     1162 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-fnml/RMLFNOTC0003-CSV/mapping.ttl
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-fnml/RMLFNOTC0003-CSV/output.nq
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-fnml/RMLFNOTC0003-CSV/student.csv
--rw-r--r--   0        0        0      717 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-fnml/RMLFNOTC0003-CSV/test_RMLFNOTC0003-CSV.py
--rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-fnml/RMLFNOTC0004-CSV/mapping.ttl
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-fnml/RMLFNOTC0004-CSV/output.nq
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-fnml/RMLFNOTC0004-CSV/student.csv
--rw-r--r--   0        0        0      694 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-fnml/RMLFNOTC0004-CSV/test_RMLFNOTC0004-CSV.py
--rw-r--r--   0        0        0     1028 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-fnml/RMLFNOTC0005-CSV/mapping.ttl
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-fnml/RMLFNOTC0005-CSV/output.nq
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-fnml/RMLFNOTC0005-CSV/student.csv
--rw-r--r--   0        0        0      717 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-fnml/RMLFNOTC0005-CSV/test_RMLFNOTC0005-CSV.py
--rw-r--r--   0        0        0     1104 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-fnml/RMLFNOTC0006-CSV/mapping.ttl
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-fnml/RMLFNOTC0006-CSV/output.nq
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-fnml/RMLFNOTC0006-CSV/student.csv
--rw-r--r--   0        0        0      717 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-fnml/RMLFNOTC0006-CSV/test_RMLFNOTC0006-CSV.py
--rw-r--r--   0        0        0     1053 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-fnml/RMLFNOTC0008-CSV/mapping.ttl
--rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-fnml/RMLFNOTC0008-CSV/output.nq
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-fnml/RMLFNOTC0008-CSV/student.csv
--rw-r--r--   0        0        0      694 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-fnml/RMLFNOTC0008-CSV/test_RMLFNOTC0008-CSV.py
--rw-r--r--   0        0        0     1702 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-fnml/RMLFNOTC0009-CSV/mapping.ttl
--rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-fnml/RMLFNOTC0009-CSV/output.nq
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-fnml/RMLFNOTC0009-CSV/student.csv
--rw-r--r--   0        0        0      794 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-fnml/RMLFNOTC0009-CSV/test_RMLFNOTC0009-CSV.py
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-fnml/array_get_slice/article.tsv
--rw-r--r--   0        0        0     1652 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-fnml/array_get_slice/mapping.ttl
--rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-fnml/array_get_slice/output.nq
--rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-fnml/array_get_slice/test_array_get_slice.py
--rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-fnml/controls_if/calendar.csv
--rw-r--r--   0        0        0     1917 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-fnml/controls_if/mapping.ttl
--rw-r--r--   0        0        0      518 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-fnml/controls_if/output.nq
--rw-r--r--   0        0        0      649 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-fnml/controls_if/test_controls_if.py
--rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-fnml/controls_if_cast/calendar.csv
--rw-r--r--   0        0        0     1921 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-fnml/controls_if_cast/mapping.ttl
--rw-r--r--   0        0        0      518 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-fnml/controls_if_cast/output.nq
--rw-r--r--   0        0        0      654 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-fnml/controls_if_cast/test_controls_if_cast.py
--rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-fnml/date_to_date/calendar.csv
--rw-r--r--   0        0        0     1315 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-fnml/date_to_date/mapping.ttl
--rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-fnml/date_to_date/output.nq
--rw-r--r--   0        0        0      650 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-fnml/date_to_date/test_date_to_date.py
--rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-fnml/math_round/distances.tsv
--rw-r--r--   0        0        0     1116 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-fnml/math_round/mapping.ttl
--rw-r--r--   0        0        0      342 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-fnml/math_round/output.nq
--rw-r--r--   0        0        0      648 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-fnml/math_round/test_math_round.py
--rw-r--r--   0        0        0     1184 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-fnml/split_explode/mapping.ttl
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-fnml/split_explode/mixed_content_list.csv
--rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-fnml/split_explode/output.nq
--rw-r--r--   0        0        0      651 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-fnml/split_explode/test_split_explode.py
--rw-r--r--   0        0        0     1189 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-fnml/split_explode_null/mapping.ttl
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-fnml/split_explode_null/mixed_content_list.csv
--rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-fnml/split_explode_null/output.nq
--rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-fnml/split_explode_null/test_split_explode_null.py
--rw-r--r--   0        0        0     1052 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-fnml/udf/mapping.ttl
--rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-fnml/udf/output.nq
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-fnml/udf/student.csv
--rw-r--r--   0        0        0      781 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-fnml/udf/test_udf.py
--rw-r--r--   0        0        0      376 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-fnml/udf/udf.py
--rw-r--r--   0        0        0      970 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-in-memory/json_dictionary/RMLIMTC0000/mapping.ttl
--rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-in-memory/json_dictionary/RMLIMTC0000/output.nq
--rw-r--r--   0        0        0      900 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-in-memory/json_dictionary/RMLIMTC0000/test_RMLTC0000_DICT.py
--rw-r--r--   0        0        0      998 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-in-memory/json_dictionary/RMLIMTC0001a/mapping.ttl
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-in-memory/json_dictionary/RMLIMTC0001a/output.nq
--rw-r--r--   0        0        0      803 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-in-memory/json_dictionary/RMLIMTC0001a/test_RMLTC0001a_DICT.py
--rw-r--r--   0        0        0      979 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-in-memory/json_dictionary/RMLIMTC0001b/mapping.ttl
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-in-memory/json_dictionary/RMLIMTC0001b/output.nq
--rw-r--r--   0        0        0      803 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-in-memory/json_dictionary/RMLIMTC0001b/test_RMLTC0001b_DICT.py
--rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-in-memory/json_dictionary/RMLIMTC0002a/mapping.ttl
--rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-in-memory/json_dictionary/RMLIMTC0002a/output.nq
--rw-r--r--   0        0        0      821 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-in-memory/json_dictionary/RMLIMTC0002a/test_RMLTC0002a_DICT.py
--rw-r--r--   0        0        0      973 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-in-memory/json_dictionary/RMLIMTC0002b/mapping.ttl
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-in-memory/json_dictionary/RMLIMTC0002b/output.nq
--rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-in-memory/json_dictionary/RMLIMTC0002b/test_RMLTC0002b_DICT.py
--rw-r--r--   0        0        0      958 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-in-memory/json_dictionary/RMLIMTC0002c/mapping.ttl
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-in-memory/json_dictionary/RMLIMTC0002c/output.nq
--rw-r--r--   0        0        0      751 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-in-memory/json_dictionary/RMLIMTC0002c/test_RMLTC0002c_DICT.py
--rw-r--r--   0        0        0      957 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-in-memory/json_dictionary/RMLIMTC0002e/mapping.ttl
--rw-r--r--   0        0        0      751 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-in-memory/json_dictionary/RMLIMTC0002e/test_RMLTC0002e_DICT.py
--rw-r--r--   0        0        0     1021 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-in-memory/json_dictionary/RMLIMTC0003c/mapping.ttl
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-in-memory/json_dictionary/RMLIMTC0003c/output.nq
--rw-r--r--   0        0        0      857 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-in-memory/json_dictionary/RMLIMTC0003c/test_RMLTC0003c_DICT.py
--rw-r--r--   0        0        0     1523 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-in-memory/json_dictionary/RMLIMTC0004a/mapping.ttl
--rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-in-memory/json_dictionary/RMLIMTC0004a/output.nq
--rw-r--r--   0        0        0      833 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-in-memory/json_dictionary/RMLIMTC0004a/test_RMLTC0004a_DICT.py
--rw-r--r--   0        0        0      996 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-in-memory/json_dictionary/RMLIMTC0004b/mapping.ttl
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-in-memory/json_dictionary/RMLIMTC0004b/output.nq
--rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-in-memory/json_dictionary/RMLIMTC0004b/test_RMLTC0004b_DICT.py
--rw-r--r--   0        0        0      992 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-in-memory/json_dictionary/RMLIMTC0005a/mapping.ttl
--rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-in-memory/json_dictionary/RMLIMTC0005a/output.nq
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-in-memory/json_dictionary/RMLIMTC0005a/test_RMLTC0005a_DICT.py
--rw-r--r--   0        0        0     1040 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-in-memory/json_dictionary/RMLIMTC0006a/mapping.ttl
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-in-memory/json_dictionary/RMLIMTC0006a/output.nq
--rw-r--r--   0        0        0      857 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-in-memory/json_dictionary/RMLIMTC0006a/test_RMLTC0006a_DICT.py
--rw-r--r--   0        0        0     1019 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-in-memory/json_dictionary/RMLIMTC0007a/mapping.ttl
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-in-memory/json_dictionary/RMLIMTC0007a/output.nq
--rw-r--r--   0        0        0      857 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-in-memory/json_dictionary/RMLIMTC0007a/test_RMLTC0007a_DICT.py
--rw-r--r--   0        0        0     1155 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-in-memory/json_dictionary/RMLIMTC0007b/mapping.ttl
--rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-in-memory/json_dictionary/RMLIMTC0007b/output.nq
--rw-r--r--   0        0        0      857 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-in-memory/json_dictionary/RMLIMTC0007b/test_RMLTC0007b_DICT.py
--rw-r--r--   0        0        0     1116 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-in-memory/json_dictionary/RMLIMTC0007c/mapping.ttl
--rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-in-memory/json_dictionary/RMLIMTC0007c/output.nq
--rw-r--r--   0        0        0      857 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-in-memory/json_dictionary/RMLIMTC0007c/test_RMLTC0007c_DICT.py
--rw-r--r--   0        0        0     1305 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-in-memory/json_dictionary/RMLIMTC0007d/mapping.ttl
--rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-in-memory/json_dictionary/RMLIMTC0007d/output.nq
--rw-r--r--   0        0        0      857 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-in-memory/json_dictionary/RMLIMTC0007d/test_RMLTC0007d_DICT.py
--rw-r--r--   0        0        0     1123 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-in-memory/json_dictionary/RMLIMTC0007e/mapping.ttl
--rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-in-memory/json_dictionary/RMLIMTC0007e/output.nq
--rw-r--r--   0        0        0      821 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-in-memory/json_dictionary/RMLIMTC0007e/test_RMLTC0007e_DICT.py
--rw-r--r--   0        0        0     1254 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-in-memory/json_dictionary/RMLIMTC0007f/mapping.ttl
--rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-in-memory/json_dictionary/RMLIMTC0007f/output.nq
--rw-r--r--   0        0        0      858 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-in-memory/json_dictionary/RMLIMTC0007f/test_RMLTC0007f_DICT.py
--rw-r--r--   0        0        0     1019 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-in-memory/json_dictionary/RMLIMTC0007g/mapping.ttl
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-in-memory/json_dictionary/RMLIMTC0007g/output.nq
--rw-r--r--   0        0        0      858 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-in-memory/json_dictionary/RMLIMTC0007g/test_RMLTC0007g_DICT.py
--rw-r--r--   0        0        0     1060 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-in-memory/json_dictionary/RMLIMTC0007h/mapping.ttl
--rw-r--r--   0        0        0      760 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-in-memory/json_dictionary/RMLIMTC0007h/test_RMLTC0007h_DICT.py
--rw-r--r--   0        0        0     1401 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-in-memory/json_dictionary/RMLIMTC0008a/mapping.ttl
--rw-r--r--   0        0        0      627 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-in-memory/json_dictionary/RMLIMTC0008a/output.nq
--rw-r--r--   0        0        0      858 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-in-memory/json_dictionary/RMLIMTC0008a/test_RMLTC0008a_DICT.py
--rw-r--r--   0        0        0     1909 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-in-memory/json_dictionary/RMLIMTC0008b/mapping.ttl
--rw-r--r--   0        0        0      544 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-in-memory/json_dictionary/RMLIMTC0008b/output.nq
--rw-r--r--   0        0        0      858 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-in-memory/json_dictionary/RMLIMTC0008b/test_RMLTC0008b_DICT.py
--rw-r--r--   0        0        0     1045 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-in-memory/json_dictionary/RMLIMTC0008c/mapping.ttl
--rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-in-memory/json_dictionary/RMLIMTC0008c/output.nq
--rw-r--r--   0        0        0      857 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-in-memory/json_dictionary/RMLIMTC0008c/test_RMLTC0008c_DICT.py
--rw-r--r--   0        0        0     1843 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-in-memory/json_dictionary/RMLIMTC0009a/mapping.ttl
--rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-in-memory/json_dictionary/RMLIMTC0009a/output.nq
--rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-in-memory/json_dictionary/RMLIMTC0009a/test_RMLTC0009a_DICT.py
--rw-r--r--   0        0        0     2153 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-in-memory/json_dictionary/RMLIMTC0009b/mapping.ttl
--rw-r--r--   0        0        0     1198 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-in-memory/json_dictionary/RMLIMTC0009b/output.nq
--rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-in-memory/json_dictionary/RMLIMTC0009b/test_RMLTC0009b_DICT.py
--rw-r--r--   0        0        0     1011 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-in-memory/json_dictionary/RMLIMTC0010a/mapping.ttl
--rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-in-memory/json_dictionary/RMLIMTC0010a/output.nq
--rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-in-memory/json_dictionary/RMLIMTC0010a/test_RMLTC0010a_DICT.py
--rw-r--r--   0        0        0     1018 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-in-memory/json_dictionary/RMLIMTC0010b/mapping.ttl
--rw-r--r--   0        0        0      312 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-in-memory/json_dictionary/RMLIMTC0010b/output.nq
--rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-in-memory/json_dictionary/RMLIMTC0010b/test_RMLTC0010b_DICT.py
--rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-in-memory/json_dictionary/RMLIMTC0010c/mapping.ttl
--rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-in-memory/json_dictionary/RMLIMTC0010c/output.nq
--rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-in-memory/json_dictionary/RMLIMTC0010c/test_RMLTC0010c_DICT.py
--rw-r--r--   0        0        0     2261 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-in-memory/json_dictionary/RMLIMTC0011b/mapping.ttl
--rw-r--r--   0        0        0     1229 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-in-memory/json_dictionary/RMLIMTC0011b/output.nq
--rw-r--r--   0        0        0     1391 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-in-memory/json_dictionary/RMLIMTC0011b/test_RMLTC0011b_DICT.py
--rw-r--r--   0        0        0     1146 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-in-memory/json_dictionary/RMLIMTC0012a/mapping.ttl
--rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-in-memory/json_dictionary/RMLIMTC0012a/output.nq
--rw-r--r--   0        0        0      899 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-in-memory/json_dictionary/RMLIMTC0012a/test_RMLTC0012a_DICT.py
--rw-r--r--   0        0        0     1553 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-in-memory/json_dictionary/RMLIMTC0012b/mapping.ttl
--rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-in-memory/json_dictionary/RMLIMTC0012b/output.nq
--rw-r--r--   0        0        0     1129 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-in-memory/json_dictionary/RMLIMTC0012b/test_RMLTC0012b_DICT.py
--rw-r--r--   0        0        0     1060 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-in-memory/json_dictionary/RMLIMTC0012c/mapping.ttl
--rw-r--r--   0        0        0      865 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-in-memory/json_dictionary/RMLIMTC0012c/test_RMLTC0012c_DICT.py
--rw-r--r--   0        0        0     1235 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-in-memory/json_dictionary/RMLIMTC0012d/mapping.ttl
--rw-r--r--   0        0        0      865 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-in-memory/json_dictionary/RMLIMTC0012d/test_RMLTC0012d_DICT.py
--rw-r--r--   0        0        0      997 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-in-memory/json_dictionary/RMLIMTC0013a/mapping.ttl
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-in-memory/json_dictionary/RMLIMTC0013a/output.nq
--rw-r--r--   0        0        0      899 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-in-memory/json_dictionary/RMLIMTC0013a/test_RMLTC0013a_DICT.py
--rw-r--r--   0        0        0     1577 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-in-memory/json_dictionary/RMLIMTC0015a/mapping.ttl
--rw-r--r--   0        0        0      386 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-in-memory/json_dictionary/RMLIMTC0015a/output.nq
--rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-in-memory/json_dictionary/RMLIMTC0015a/test_RMLTC0015a_DICT.py
--rw-r--r--   0        0        0     1574 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-in-memory/json_dictionary/RMLIMTC0015b/mapping.ttl
--rw-r--r--   0        0        0      991 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-in-memory/json_dictionary/RMLIMTC0015b/test_RMLTC0015b_DICT.py
--rw-r--r--   0        0        0      984 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-in-memory/pandas_dataframe/RMLIMTC0000/mapping.ttl
--rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-in-memory/pandas_dataframe/RMLIMTC0000/output.nq
--rw-r--r--   0        0        0      790 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-in-memory/pandas_dataframe/RMLIMTC0000/test_RMLIMTC0000_DF.py
--rw-r--r--   0        0        0      983 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-in-memory/pandas_dataframe/RMLIMTC0001a/mapping.ttl
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-in-memory/pandas_dataframe/RMLIMTC0001a/output.nq
--rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-in-memory/pandas_dataframe/RMLIMTC0001a/student.csv
--rw-r--r--   0        0        0      795 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-in-memory/pandas_dataframe/RMLIMTC0001a/test_RMLTC0001a_DF.py
--rw-r--r--   0        0        0      994 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-in-memory/pandas_dataframe/RMLIMTC0001b/mapping.ttl
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-in-memory/pandas_dataframe/RMLIMTC0001b/output.nq
--rw-r--r--   0        0        0      795 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-in-memory/pandas_dataframe/RMLIMTC0001b/test_RMLIMTC0001b_DF.py
--rw-r--r--   0        0        0     1100 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-in-memory/pandas_dataframe/RMLIMTC0002a/mapping.ttl
--rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-in-memory/pandas_dataframe/RMLIMTC0002a/output.nq
--rw-r--r--   0        0        0      806 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-in-memory/pandas_dataframe/RMLIMTC0002a/test_RMLIMTC0002a_DF.py
--rw-r--r--   0        0        0      988 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-in-memory/pandas_dataframe/RMLIMTC0002b/mapping.ttl
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-in-memory/pandas_dataframe/RMLIMTC0002b/output.nq
--rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-in-memory/pandas_dataframe/RMLIMTC0002b/test_RMLIMTC0002b_DF.py
--rw-r--r--   0        0        0      973 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-in-memory/pandas_dataframe/RMLIMTC0002c/mapping.ttl
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-in-memory/pandas_dataframe/RMLIMTC0002c/output.nq
--rw-r--r--   0        0        0      736 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-in-memory/pandas_dataframe/RMLIMTC0002c/test_RMLIMTC0002c_DF.py
--rw-r--r--   0        0        0      972 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-in-memory/pandas_dataframe/RMLIMTC0002e/mapping.ttl
--rw-r--r--   0        0        0      736 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-in-memory/pandas_dataframe/RMLIMTC0002e/test_RMLIMTC0002e_DF.py
--rw-r--r--   0        0        0     1034 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-in-memory/pandas_dataframe/RMLIMTC0003c/mapping.ttl
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-in-memory/pandas_dataframe/RMLIMTC0003c/output.nq
--rw-r--r--   0        0        0      836 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-in-memory/pandas_dataframe/RMLIMTC0003c/test_RMLIMTC0003c_DF.py
--rw-r--r--   0        0        0     1552 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-in-memory/pandas_dataframe/RMLIMTC0004a/mapping.ttl
--rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-in-memory/pandas_dataframe/RMLIMTC0004a/output.nq
--rw-r--r--   0        0        0      818 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-in-memory/pandas_dataframe/RMLIMTC0004a/test_RMLIMTC0004a_DF.py
--rw-r--r--   0        0        0     1005 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-in-memory/pandas_dataframe/RMLIMTC0004b/mapping.ttl
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-in-memory/pandas_dataframe/RMLIMTC0004b/output.nq
--rw-r--r--   0        0        0      725 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-in-memory/pandas_dataframe/RMLIMTC0004b/test_RMLIMTC0004b_DF.py
--rw-r--r--   0        0        0     1001 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-in-memory/pandas_dataframe/RMLIMTC0005a/mapping.ttl
--rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-in-memory/pandas_dataframe/RMLIMTC0005a/output.nq
--rw-r--r--   0        0        0      907 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-in-memory/pandas_dataframe/RMLIMTC0005a/test_RMLIMTC0005a_DF.py
--rw-r--r--   0        0        0     1056 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-in-memory/pandas_dataframe/RMLIMTC0006a/mapping.ttl
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-in-memory/pandas_dataframe/RMLIMTC0006a/output.nq
--rw-r--r--   0        0        0      836 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-in-memory/pandas_dataframe/RMLIMTC0006a/test_RMLIMTC0006a_DF.py
--rw-r--r--   0        0        0     1034 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-in-memory/pandas_dataframe/RMLIMTC0007a/mapping.ttl
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-in-memory/pandas_dataframe/RMLIMTC0007a/output.nq
--rw-r--r--   0        0        0      836 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-in-memory/pandas_dataframe/RMLIMTC0007a/test_RMLIMTC0007a_DF.py
--rw-r--r--   0        0        0     1163 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-in-memory/pandas_dataframe/RMLIMTC0007b/mapping.ttl
--rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-in-memory/pandas_dataframe/RMLIMTC0007b/output.nq
--rw-r--r--   0        0        0      836 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-in-memory/pandas_dataframe/RMLIMTC0007b/test_RMLIMTC0007b_DF.py
--rw-r--r--   0        0        0     1131 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-in-memory/pandas_dataframe/RMLIMTC0007c/mapping.ttl
--rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-in-memory/pandas_dataframe/RMLIMTC0007c/output.nq
--rw-r--r--   0        0        0      836 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-in-memory/pandas_dataframe/RMLIMTC0007c/test_RMLIMTC0007c_DF.py
--rw-r--r--   0        0        0     1322 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-in-memory/pandas_dataframe/RMLIMTC0007d/mapping.ttl
--rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-in-memory/pandas_dataframe/RMLIMTC0007d/output.nq
--rw-r--r--   0        0        0      835 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-in-memory/pandas_dataframe/RMLIMTC0007d/test_RMLTC0007d_DF.py
--rw-r--r--   0        0        0     1151 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-in-memory/pandas_dataframe/RMLIMTC0007e/mapping.ttl
--rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-in-memory/pandas_dataframe/RMLIMTC0007e/output.nq
--rw-r--r--   0        0        0      806 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-in-memory/pandas_dataframe/RMLIMTC0007e/test_RMLIMTC0007e_DF.py
--rw-r--r--   0        0        0     1269 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-in-memory/pandas_dataframe/RMLIMTC0007f/mapping.ttl
--rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-in-memory/pandas_dataframe/RMLIMTC0007f/output.nq
--rw-r--r--   0        0        0      836 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-in-memory/pandas_dataframe/RMLIMTC0007f/test_RMLIMTC0007f_DF.py
--rw-r--r--   0        0        0     1034 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-in-memory/pandas_dataframe/RMLIMTC0007g/mapping.ttl
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-in-memory/pandas_dataframe/RMLIMTC0007g/output.nq
--rw-r--r--   0        0        0      836 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-in-memory/pandas_dataframe/RMLIMTC0007g/test_RMLIMTC0007g_DF.py
--rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-in-memory/pandas_dataframe/RMLIMTC0007h/mapping.ttl
--rw-r--r--   0        0        0      739 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-in-memory/pandas_dataframe/RMLIMTC0007h/test_RMLIMTC0007h_DF.py
--rw-r--r--   0        0        0     1416 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-in-memory/pandas_dataframe/RMLIMTC0008a/mapping.ttl
--rw-r--r--   0        0        0      627 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-in-memory/pandas_dataframe/RMLIMTC0008a/output.nq
--rw-r--r--   0        0        0      835 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-in-memory/pandas_dataframe/RMLIMTC0008a/test_RMLIMTC0008a_DF.py
--rw-r--r--   0        0        0     1933 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-in-memory/pandas_dataframe/RMLIMTC0008b/mapping.ttl
--rw-r--r--   0        0        0      544 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-in-memory/pandas_dataframe/RMLIMTC0008b/output.nq
--rw-r--r--   0        0        0      835 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-in-memory/pandas_dataframe/RMLIMTC0008b/test_RMLIMTC0008b_DF.py
--rw-r--r--   0        0        0     1060 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-in-memory/pandas_dataframe/RMLIMTC0008c/mapping.ttl
--rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-in-memory/pandas_dataframe/RMLIMTC0008c/output.nq
--rw-r--r--   0        0        0      835 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-in-memory/pandas_dataframe/RMLIMTC0008c/test_RMLIMTC0008c_DF.py
--rw-r--r--   0        0        0     1875 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-in-memory/pandas_dataframe/RMLIMTC0009a/mapping.ttl
--rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-in-memory/pandas_dataframe/RMLIMTC0009a/output.nq
--rw-r--r--   0        0        0      925 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-in-memory/pandas_dataframe/RMLIMTC0009a/test_RMLIMTC0009a_DF.py
--rw-r--r--   0        0        0     2190 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-in-memory/pandas_dataframe/RMLIMTC0009b/mapping.ttl
--rw-r--r--   0        0        0     1198 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-in-memory/pandas_dataframe/RMLIMTC0009b/output.nq
--rw-r--r--   0        0        0      925 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-in-memory/pandas_dataframe/RMLIMTC0009b/test_RMLIMTC0009b_DF.py
--rw-r--r--   0        0        0     1026 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-in-memory/pandas_dataframe/RMLIMTC0010a/mapping.ttl
--rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-in-memory/pandas_dataframe/RMLIMTC0010a/output.nq
--rw-r--r--   0        0        0      938 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-in-memory/pandas_dataframe/RMLIMTC0010a/test_RMLIMTC0010a_DF.py
--rw-r--r--   0        0        0     1033 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-in-memory/pandas_dataframe/RMLIMTC0010b/mapping.ttl
--rw-r--r--   0        0        0      312 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-in-memory/pandas_dataframe/RMLIMTC0010b/output.nq
--rw-r--r--   0        0        0      930 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-in-memory/pandas_dataframe/RMLIMTC0010b/test_RMLIMTC0010b_DF.py
--rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-in-memory/pandas_dataframe/RMLIMTC0010c/mapping.ttl
--rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-in-memory/pandas_dataframe/RMLIMTC0010c/output.nq
--rw-r--r--   0        0        0      930 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-in-memory/pandas_dataframe/RMLIMTC0010c/test_RMLIMTC0010c_DF.py
--rw-r--r--   0        0        0     2315 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-in-memory/pandas_dataframe/RMLIMTC0011b/mapping.ttl
--rw-r--r--   0        0        0     1229 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-in-memory/pandas_dataframe/RMLIMTC0011b/output.nq
--rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-in-memory/pandas_dataframe/RMLIMTC0011b/test_RMLIMTC0011b_DF.py
--rw-r--r--   0        0        0     1162 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-in-memory/pandas_dataframe/RMLIMTC0012a/mapping.ttl
--rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-in-memory/pandas_dataframe/RMLIMTC0012a/output.nq
--rw-r--r--   0        0        0      831 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-in-memory/pandas_dataframe/RMLIMTC0012a/test_RMLIMTC0012a_DF.py
--rw-r--r--   0        0        0     1589 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-in-memory/pandas_dataframe/RMLIMTC0012b/mapping.ttl
--rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-in-memory/pandas_dataframe/RMLIMTC0012b/output.nq
--rw-r--r--   0        0        0      987 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-in-memory/pandas_dataframe/RMLIMTC0012b/test_RMLIMTC0012b_DF.py
--rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-in-memory/pandas_dataframe/RMLIMTC0012c/mapping.ttl
--rw-r--r--   0        0        0      796 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-in-memory/pandas_dataframe/RMLIMTC0012c/test_RMLIMTC0012c_DF.py
--rw-r--r--   0        0        0     1252 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-in-memory/pandas_dataframe/RMLIMTC0012d/mapping.ttl
--rw-r--r--   0        0        0      797 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-in-memory/pandas_dataframe/RMLIMTC0012d/test_RMLIMTC0012d_DF.py
--rw-r--r--   0        0        0     1607 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-in-memory/pandas_dataframe/RMLIMTC0015a/mapping.ttl
--rw-r--r--   0        0        0      386 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-in-memory/pandas_dataframe/RMLIMTC0015a/output.nq
--rw-r--r--   0        0        0      992 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-in-memory/pandas_dataframe/RMLIMTC0015a/test_RMLIMTC0015a_DF.py
--rw-r--r--   0        0        0     1604 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-in-memory/pandas_dataframe/RMLIMTC0015b/mapping.ttl
--rw-r--r--   0        0        0      922 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-in-memory/pandas_dataframe/RMLIMTC0015b/test_RMLIMTC0015b_DF.py
--rw-r--r--   0        0        0     1031 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-in-memory/pandas_dataframe/RMLIMTC0016a/mapping.ttl
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-in-memory/pandas_dataframe/RMLIMTC0016a/test.csv
--rw-r--r--   0        0        0      768 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-in-memory/pandas_dataframe/RMLIMTC0016a/test_RMLIMTC0016a_DF.py
--rw-r--r--   0        0        0     1662 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-in-memory/pandas_dataframe/triples_map_without_pom/mapping.ttl
--rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-in-memory/pandas_dataframe/triples_map_without_pom/output.nq
--rw-r--r--   0        0        0      937 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-in-memory/pandas_dataframe/triples_map_without_pom/test_triples_map_without_pom_DF.py
--rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-star/RMLSTARTC001a/data.csv
--rw-r--r--   0        0        0      968 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-star/RMLSTARTC001a/mapping.ttl
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-star/RMLSTARTC001a/output.nq
--rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-star/RMLSTARTC001a/test_RMLSTARTC001a_CSV.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-star/RMLSTARTC001b/data1.csv
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-star/RMLSTARTC001b/data2.csv
--rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-star/RMLSTARTC001b/mapping.ttl
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-star/RMLSTARTC001b/output.nq
--rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-star/RMLSTARTC001b/test_RMLSTARTC001b_CSV.py
--rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-star/RMLSTARTC002a/data.csv
--rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-star/RMLSTARTC002a/mapping.ttl
--rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-star/RMLSTARTC002a/output.nq
--rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-star/RMLSTARTC002a/test_RMLSTARTC002a_CSV.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-star/RMLSTARTC002b/data1.csv
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-star/RMLSTARTC002b/data2.csv
--rw-r--r--   0        0        0     1169 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-star/RMLSTARTC002b/mapping.ttl
--rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-star/RMLSTARTC002b/output.nq
--rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-star/RMLSTARTC002b/test_RMLSTARTC002b_CSV.py
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-star/RMLSTARTC003a/data.csv
--rw-r--r--   0        0        0     1419 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-star/RMLSTARTC003a/mapping.ttl
--rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-star/RMLSTARTC003a/output.nq
--rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-star/RMLSTARTC003a/test_RMLSTARTC003a_CSV.py
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-star/RMLSTARTC003b/data1.csv
--rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-star/RMLSTARTC003b/data2.csv
--rw-r--r--   0        0        0     1529 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-star/RMLSTARTC003b/mapping.ttl
--rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-star/RMLSTARTC003b/output.nq
--rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-star/RMLSTARTC003b/test_RMLSTARTC003b_CSV.py
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-star/RMLSTARTC004a/data.csv
--rw-r--r--   0        0        0     1396 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-star/RMLSTARTC004a/mapping.ttl
--rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-star/RMLSTARTC004a/output.nq
--rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-star/RMLSTARTC004a/test_RMLSTARTC004a_CSV.py
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-star/RMLSTARTC004b/data1.csv
--rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-star/RMLSTARTC004b/data2.csv
--rw-r--r--   0        0        0     1506 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-star/RMLSTARTC004b/mapping.ttl
--rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-star/RMLSTARTC004b/output.nq
--rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-star/RMLSTARTC004b/test_RMLSTARTC004b_CSV.py
--rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-star/RMLSTARTC005a/data.csv
--rw-r--r--   0        0        0     1021 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-star/RMLSTARTC005a/mapping.ttl
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-star/RMLSTARTC005a/output.nq
--rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-star/RMLSTARTC005a/test_RMLSTARTC005a_CSV.py
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-star/RMLSTARTC005b/data1.csv
--rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-star/RMLSTARTC005b/data2.csv
--rw-r--r--   0        0        0     1145 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-star/RMLSTARTC005b/mapping.ttl
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-star/RMLSTARTC005b/output.nq
--rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-star/RMLSTARTC005b/test_RMLSTARTC005b_CSV.py
--rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-star/RMLSTARTC006a/data.csv
--rw-r--r--   0        0        0     1121 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-star/RMLSTARTC006a/mapping.ttl
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-star/RMLSTARTC006a/output.nq
--rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-star/RMLSTARTC006a/test_RMLSTARTC006a_CSV.py
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-star/RMLSTARTC006b/data1.csv
--rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-star/RMLSTARTC006b/data2.csv
--rw-r--r--   0        0        0     1244 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-star/RMLSTARTC006b/mapping.ttl
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-star/RMLSTARTC006b/output.nq
--rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-star/RMLSTARTC006b/test_RMLSTARTC006b_CSV.py
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-star/RMLSTARTC007a/data.csv
--rw-r--r--   0        0        0     1408 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-star/RMLSTARTC007a/mapping.ttl
--rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-star/RMLSTARTC007a/output.nq
--rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-star/RMLSTARTC007a/test_RMLSTARTC007a_CSV.py
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-star/RMLSTARTC007b/data1.csv
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-star/RMLSTARTC007b/data2.csv
--rw-r--r--   0        0        0     1535 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-star/RMLSTARTC007b/mapping.ttl
--rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-star/RMLSTARTC007b/output.nq
--rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-star/RMLSTARTC007b/test_RMLSTARTC007b_CSV.py
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-star/RMLSTARTC008a/data.csv
--rw-r--r--   0        0        0     3028 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-star/RMLSTARTC008a/mapping.ttl
--rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-star/RMLSTARTC008a/output.nq
--rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-star/RMLSTARTC008a/test_RMLSTARTC008a_CSV.py
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-star/RMLSTARTC008b/data1.csv
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-star/RMLSTARTC008b/data2.csv
--rw-r--r--   0        0        0     3167 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-star/RMLSTARTC008b/mapping.ttl
--rw-r--r--   0        0        0      311 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-star/RMLSTARTC008b/output.nq
--rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rml-star/RMLSTARTC008b/test_RMLSTARTC008b_CSV.py
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rmltv/RMLTVTC0002d/mapping.ttl
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rmltv/RMLTVTC0002d/output.nq
--rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rmltv/RMLTVTC0002d/student.csv
--rw-r--r--   0        0        0      654 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rmltv/RMLTVTC0002d/test_RMLTVTC0002d_CSV.py
--rw-r--r--   0        0        0      572 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rmltv/RMLTVTC0002g/mapping.ttl
--rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rmltv/RMLTVTC0002g/student.csv
--rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rmltv/RMLTVTC0002g/test_RMLTVTC0002g_CSV.py
--rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rmltv/RMLTVTC0002h/mapping.ttl
--rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rmltv/RMLTVTC0002h/student.csv
--rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rmltv/RMLTVTC0002h/test_RMLTVTC0002h_CSV.py
--rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rmltv/RMLTVTC0002i/mapping.ttl
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rmltv/RMLTVTC0002i/output.nq
--rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rmltv/RMLTVTC0002i/student.csv
--rw-r--r--   0        0        0      654 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rmltv/RMLTVTC0002i/test_RMLTVTC0002i_CSV.py
--rw-r--r--   0        0        0      612 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rmltv/RMLTVTC0002j/mapping.ttl
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rmltv/RMLTVTC0002j/output.nq
--rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rmltv/RMLTVTC0002j/student.csv
--rw-r--r--   0        0        0      654 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rmltv/RMLTVTC0002j/test_RMLTVTC0002j_CSV.py
--rw-r--r--   0        0        0      648 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rmltv/RMLTVTC0003b/mapping.ttl
--rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rmltv/RMLTVTC0003b/output.nq
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rmltv/RMLTVTC0003b/student.csv
--rw-r--r--   0        0        0      654 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rmltv/RMLTVTC0003b/test_RMLTVTC0003b_CSV.py
--rw-r--r--   0        0        0      541 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rmltv/RMLTVTC0009c/mapping.ttl
--rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rmltv/RMLTVTC0009c/output.nq
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rmltv/RMLTVTC0009c/sport.csv
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rmltv/RMLTVTC0009c/student.csv
--rw-r--r--   0        0        0      654 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rmltv/RMLTVTC0009c/test_RMLTVTC0009c_CSV.py
--rw-r--r--   0        0        0      707 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rmltv/RMLTVTC0009d/mapping.ttl
--rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rmltv/RMLTVTC0009d/output.nq
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rmltv/RMLTVTC0009d/sport.csv
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rmltv/RMLTVTC0009d/student.csv
--rw-r--r--   0        0        0      654 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rmltv/RMLTVTC0009d/test_RMLTVTC0009d_CSV.py
--rw-r--r--   0        0        0     1753 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rmltv/RMLTVTC0011a/mapping.ttl
--rw-r--r--   0        0        0     1525 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rmltv/RMLTVTC0011a/output.nq
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rmltv/RMLTVTC0011a/sport.csv
--rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rmltv/RMLTVTC0011a/student.csv
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rmltv/RMLTVTC0011a/student_sport.csv
--rw-r--r--   0        0        0      650 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rmltv/RMLTVTC0011a/test_RMLTVTC0011a_CSV.py
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rmltv/RMLTVTC0014d/dept.csv
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rmltv/RMLTVTC0014d/emp.csv
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rmltv/RMLTVTC0014d/likes.csv
--rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rmltv/RMLTVTC0014d/mapping.ttl
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rmltv/RMLTVTC0014d/output.nq
--rw-r--r--   0        0        0      650 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rmltv/RMLTVTC0014d/test_RMLTVTC0014d_CSV.py
--rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rmltv/RMLTVTC0015a/country.csv
--rw-r--r--   0        0        0     1012 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rmltv/RMLTVTC0015a/mapping.ttl
--rw-r--r--   0        0        0      386 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rmltv/RMLTVTC0015a/output.nq
--rw-r--r--   0        0        0      650 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rmltv/RMLTVTC0015a/test_RMLTVTC0015a_CSV.py
--rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rmltv/RMLTVTC0015b/country.csv
--rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rmltv/RMLTVTC0015b/mapping.ttl
--rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rmltv/RMLTVTC0015b/test_RMLTVTC0015b_CSV.py
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rmltv/RMLTVTC0019a/employee.csv
--rw-r--r--   0        0        0      616 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rmltv/RMLTVTC0019a/mapping.ttl
--rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rmltv/RMLTVTC0019a/output.nq
--rw-r--r--   0        0        0      650 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rmltv/RMLTVTC0019a/test_RMLTVTC0019a_CSV.py
--rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rmltv/RMLTVTC0026a/mapping.ttl
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rmltv/RMLTVTC0026a/mixed_content_list.csv
--rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rmltv/RMLTVTC0026a/output.nq
--rw-r--r--   0        0        0      650 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rmltv/RMLTVTC0026a/test_RMLTVTC0026a_CSV.py
--rw-r--r--   0        0        0      795 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rmltv/RMLTVTC0027a/mapping.ttl
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rmltv/RMLTVTC0027a/mixed_content_json.csv
--rw-r--r--   0        0        0      342 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rmltv/RMLTVTC0027a/output.nq
--rw-r--r--   0        0        0      650 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rmltv/RMLTVTC0027a/test_RMLTVTC0027a_CSV.py
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rmltv/RMLTVTC0028a/aka_title.csv
--rw-r--r--   0        0        0      821 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rmltv/RMLTVTC0028a/mapping.ttl
--rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rmltv/RMLTVTC0028a/output.nq
--rw-r--r--   0        0        0      650 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rmltv/RMLTVTC0028a/test_RMLTVTC0028a_CSV.py
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rmltv/RMLTVTC0028a/title.csv
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rmltv/RMLTVTC0029a/department.csv
--rw-r--r--   0        0        0      299 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rmltv/RMLTVTC0029a/faculty.csv
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rmltv/RMLTVTC0029a/graduatecourse.csv
--rw-r--r--   0        0        0      965 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rmltv/RMLTVTC0029a/mapping.ttl
--rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rmltv/RMLTVTC0029a/output.nq
--rw-r--r--   0        0        0      650 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/test/rmltv/RMLTVTC0029a/test_RMLTVTC0029a_CSV.py
--rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/LICENSE
--rw-r--r--   0        0        0     6956 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/README.md
--rw-r--r--   0        0        0     2580 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/pyproject.toml
--rw-r--r--   0        0        0    10225 2020-02-02 00:00:00.000000 morph_kgc-2.6.4/PKG-INFO
+-rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/.zenodo.json
+-rw-r--r--   0        0        0      869 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/CITATION.cff
+-rw-r--r--   0        0        0      881 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0      700 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/CONTRIBUTING.md
+-rw-r--r--   0        0        0     1546 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/Dockerfile
+-rw-r--r--   0        0        0      454 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/.github/ISSUE_TEMPLATE/bug-report.md
+-rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/.github/ISSUE_TEMPLATE/documentation-improvement.md
+-rw-r--r--   0        0        0      577 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/.github/ISSUE_TEMPLATE/feature-request.md
+-rw-r--r--   0        0        0      630 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/.github/ISSUE_TEMPLATE/installation-issue.md
+-rw-r--r--   0        0        0      328 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/.github/ISSUE_TEMPLATE/submit-quesion.md
+-rw-r--r--   0        0        0      640 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/.github/workflows/ci.yml
+-rw-r--r--   0        0        0      863 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/.github/workflows/pypi-publish.yml
+-rw-r--r--   0        0        0     3580 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/examples/README.md
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/examples/configuration-file/basic_config.ini
+-rw-r--r--   0        0        0      560 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/examples/configuration-file/default_config.ini
+-rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/examples/configuration-file/oracle_config.ini
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/examples/csv/config.ini
+-rw-r--r--   0        0        0     7907 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/examples/csv/mapping.csv.yml
+-rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/examples/csv/data/AGENCY.csv
+-rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/examples/csv/data/CALENDAR.csv
+-rw-r--r--   0        0        0      507 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/examples/csv/data/CALENDAR_DATES.csv
+-rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/examples/csv/data/FEED_INFO.csv
+-rw-r--r--   0        0        0     3503 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/examples/csv/data/FREQUENCIES.csv
+-rw-r--r--   0        0        0     2924 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/examples/csv/data/ROUTES.csv
+-rw-r--r--   0        0        0     3171 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/examples/csv/data/SHAPES.csv
+-rw-r--r--   0        0        0     4379 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/examples/csv/data/STOPS.csv
+-rw-r--r--   0        0        0     4700 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/examples/csv/data/STOP_TIMES.csv
+-rw-r--r--   0        0        0     6000 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/examples/csv/data/TRIPS.csv
+-rw-r--r--   0        0        0      926 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/examples/dataframe/kg_generation.py
+-rw-r--r--   0        0        0     2102 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/examples/dataframe/mapping.rml.ttl
+-rw-r--r--   0        0        0     1578 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/examples/dict/kg_generation.py
+-rw-r--r--   0        0        0     2116 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/examples/dict/mapping.rml.ttl
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/examples/json/config.ini
+-rw-r--r--   0        0        0     3464 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/examples/json/data.json
+-rw-r--r--   0        0        0     1773 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/examples/json/mapping.json.yaml
+-rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/examples/rdb/config.ini
+-rw-r--r--   0        0        0     8193 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/examples/rdb/mapping.rdb.yml
+-rw-r--r--   0        0        0    13238 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/examples/tutorial/Morph-KGC.ipynb
+-rw-r--r--   0        0        0      327 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/examples/tutorial/README.md
+-rw-r--r--   0        0        0    34542 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/examples/tutorial/mapping.gtfs.ttl
+-rw-r--r--   0        0        0    26514 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/examples/tutorial/mapping.somef.ttl
+-rw-r--r--   0        0        0    35086 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/examples/tutorial/oeg-upm_morph-kgc.json
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/examples/xml/config.ini
+-rw-r--r--   0        0        0     3656 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/examples/xml/data.xml
+-rw-r--r--   0        0        0     1738 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/examples/xml/mapping.xml.yaml
+-rw-r--r--   0        0        0    50123 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/logo/logo.png
+-rw-r--r--   0        0        0     3952 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/src/morph_kgc/__init__.py
+-rw-r--r--   0        0        0     2350 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/src/morph_kgc/__main__.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/src/morph_kgc/_version.py
+-rw-r--r--   0        0        0     2195 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/src/morph_kgc/args_parser.py
+-rw-r--r--   0        0        0    15236 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/src/morph_kgc/config.py
+-rw-r--r--   0        0        0    11310 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/src/morph_kgc/constants.py
+-rw-r--r--   0        0        0    26179 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/src/morph_kgc/materializer.py
+-rw-r--r--   0        0        0    10751 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/src/morph_kgc/utils.py
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/src/morph_kgc/data_source/__init__.py
+-rw-r--r--   0        0        0     8878 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/src/morph_kgc/data_source/data_file.py
+-rw-r--r--   0        0        0     2563 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/src/morph_kgc/data_source/python_data.py
+-rw-r--r--   0        0        0     7610 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/src/morph_kgc/data_source/relational_database.py
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/src/morph_kgc/fnml/__init__.py
+-rw-r--r--   0        0        0     8730 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/src/morph_kgc/fnml/built_in_functions.py
+-rw-r--r--   0        0        0     4678 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/src/morph_kgc/fnml/fnml_executer.py
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/src/morph_kgc/mapping/__init__.py
+-rw-r--r--   0        0        0     6465 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/src/morph_kgc/mapping/mapping_constants.py
+-rw-r--r--   0        0        0    40611 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/src/morph_kgc/mapping/mapping_parser.py
+-rw-r--r--   0        0        0    20050 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/src/morph_kgc/mapping/mapping_partitioner.py
+-rw-r--r--   0        0        0    31995 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/src/morph_kgc/mapping/yarrrml.py
+-rw-r--r--   0        0        0     1455 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/issues/issue_118/mapping.ttl
+-rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/issues/issue_118/output.nq
+-rw-r--r--   0        0        0     1500 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/issues/issue_118/premis.xml
+-rw-r--r--   0        0        0      689 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/issues/issue_118/test_issue_118.py
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/issues/issue_124/data.csv
+-rw-r--r--   0        0        0     1645 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/issues/issue_124/mapping.ttl
+-rw-r--r--   0        0        0     1136 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/issues/issue_124/output.nq
+-rw-r--r--   0        0        0      758 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/issues/issue_124/test_issue_124.py
+-rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/issues/issue_145/data.csv
+-rw-r--r--   0        0        0     1537 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/issues/issue_145/mapping.ttl
+-rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/issues/issue_145/output.nq
+-rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/issues/issue_145/test_issue_145.py
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/issues/issue_174/data-1.csv
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/issues/issue_174/data-2.csv
+-rw-r--r--   0        0        0     1554 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/issues/issue_174/mapping-a.ttl
+-rw-r--r--   0        0        0     1431 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/issues/issue_174/mapping-b.ttl
+-rw-r--r--   0        0        0     1407 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/issues/issue_174/mapping-c.ttl
+-rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/issues/issue_174/output-a.nq
+-rw-r--r--   0        0        0      772 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/issues/issue_174/output-b.nq
+-rw-r--r--   0        0        0      684 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/issues/issue_174/output-c.nq
+-rw-r--r--   0        0        0     1557 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/issues/issue_174/test_issue_174.py
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/issues/issue_62/data1.csv
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/issues/issue_62/data2.csv
+-rw-r--r--   0        0        0      962 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/issues/issue_62/mapping.ttl
+-rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/issues/issue_62/output.nq
+-rw-r--r--   0        0        0      709 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/issues/issue_62/test_issue_62.py
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/issues/issue_67/data.csv
+-rw-r--r--   0        0        0      906 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/issues/issue_67/mapping.ttl
+-rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/issues/issue_67/output.nq
+-rw-r--r--   0        0        0      686 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/issues/issue_67/test_issue_67.py
+-rw-r--r--   0        0        0      635 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/issues/issue_80/mapping.rml
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/issues/issue_80/output.nq
+-rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/issues/issue_80/student.csv
+-rw-r--r--   0        0        0      686 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/issues/issue_80/test_issue_80.py
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/issues/issue_81/country_info.csv
+-rw-r--r--   0        0        0      589 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/issues/issue_81/mapping.ttl
+-rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/issues/issue_81/output.nq
+-rw-r--r--   0        0        0      686 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/issues/issue_81/test_issue_81.py
+-rw-r--r--   0        0        0      480 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/r2rml/R2RMLTC0000/mapping.ttl
+-rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/r2rml/R2RMLTC0000/output.nq
+-rw-r--r--   0        0        0     8192 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/r2rml/R2RMLTC0000/resource.db
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/r2rml/R2RMLTC0000/resource.sql
+-rw-r--r--   0        0        0      829 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/r2rml/R2RMLTC0000/test_R2RMLTC0000_SQLITE.py
+-rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/r2rml/R2RMLTC0001a/mapping.ttl
+-rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/r2rml/R2RMLTC0001a/output.nq
+-rw-r--r--   0        0        0     8192 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/r2rml/R2RMLTC0001a/resource.db
+-rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/r2rml/R2RMLTC0001a/resource.sql
+-rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/r2rml/R2RMLTC0001a/test_R2RMLTC0001a_SQLITE.py
+-rw-r--r--   0        0        0      489 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/r2rml/R2RMLTC0001b/mapping.ttl
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/r2rml/R2RMLTC0001b/output.nq
+-rw-r--r--   0        0        0     8192 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/r2rml/R2RMLTC0001b/resource.db
+-rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/r2rml/R2RMLTC0001b/resource.sql
+-rw-r--r--   0        0        0      794 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/r2rml/R2RMLTC0001b/test_R2RMLTC0001b_SQLITE.py
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/r2rml/R2RMLTC0002a/mapping.ttl
+-rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/r2rml/R2RMLTC0002a/output.nq
+-rw-r--r--   0        0        0     8192 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/r2rml/R2RMLTC0002a/resource.db
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/r2rml/R2RMLTC0002a/resource.sql
+-rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/r2rml/R2RMLTC0002a/test_R2RMLTC0002a_SQLITE.py
+-rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/r2rml/R2RMLTC0002b/mapping.ttl
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/r2rml/R2RMLTC0002b/output.nq
+-rw-r--r--   0        0        0     8192 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/r2rml/R2RMLTC0002b/resource.db
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/r2rml/R2RMLTC0002b/resource.sql
+-rw-r--r--   0        0        0      764 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/r2rml/R2RMLTC0002b/test_R2RMLTC0002b_SQLITE.py
+-rw-r--r--   0        0        0      481 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/r2rml/R2RMLTC0002c/mapping.ttl
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/r2rml/R2RMLTC0002c/output.nq
+-rw-r--r--   0        0        0     8192 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/r2rml/R2RMLTC0002c/resource.db
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/r2rml/R2RMLTC0002c/resource.sql
+-rw-r--r--   0        0        0      764 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/r2rml/R2RMLTC0002c/test_R2RMLTC0002c_SQLITE.py
+-rw-r--r--   0        0        0      728 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/r2rml/R2RMLTC0002d/mapping.ttl
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/r2rml/R2RMLTC0002d/output.nq
+-rw-r--r--   0        0        0     8192 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/r2rml/R2RMLTC0002d/resource.db
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/r2rml/R2RMLTC0002d/resource.sql
+-rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/r2rml/R2RMLTC0002d/test_R2RMLTC0002d_SQLITE.py
+-rw-r--r--   0        0        0      483 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/r2rml/R2RMLTC0002e/mapping.ttl
+-rw-r--r--   0        0        0     8192 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/r2rml/R2RMLTC0002e/resource.db
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/r2rml/R2RMLTC0002e/resource.sql
+-rw-r--r--   0        0        0      764 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/r2rml/R2RMLTC0002e/test_R2RMLTC0002e_SQLITE.py
+-rw-r--r--   0        0        0      632 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/r2rml/R2RMLTC0002f/mapping.ttl
+-rw-r--r--   0        0        0     8192 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/r2rml/R2RMLTC0002f/resource.db
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/r2rml/R2RMLTC0002f/resource.sql
+-rw-r--r--   0        0        0      764 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/r2rml/R2RMLTC0002f/test_R2RMLTC0002f_SQLITE.py
+-rw-r--r--   0        0        0      575 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/r2rml/R2RMLTC0002g/mapping.ttl
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/r2rml/R2RMLTC0002g/output.nq
+-rw-r--r--   0        0        0     8192 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/r2rml/R2RMLTC0002g/resource.db
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/r2rml/R2RMLTC0002g/resource.sql
+-rw-r--r--   0        0        0      764 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/r2rml/R2RMLTC0002g/test_R2RMLTC0002g_SQLITE.py
+-rw-r--r--   0        0        0      712 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/r2rml/R2RMLTC0002h/mapping.ttl
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/r2rml/R2RMLTC0002h/output.nq
+-rw-r--r--   0        0        0     8192 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/r2rml/R2RMLTC0002h/resource.db
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/r2rml/R2RMLTC0002h/resource.sql
+-rw-r--r--   0        0        0      764 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/r2rml/R2RMLTC0002h/test_R2RMLTC0002h_SQLITE.py
+-rw-r--r--   0        0        0      694 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/r2rml/R2RMLTC0002i/mapping.ttl
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/r2rml/R2RMLTC0002i/output.nq
+-rw-r--r--   0        0        0     8192 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/r2rml/R2RMLTC0002i/resource.db
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/r2rml/R2RMLTC0002i/resource.sql
+-rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/r2rml/R2RMLTC0002i/test_R2RMLTC0002i_SQLITE.py
+-rw-r--r--   0        0        0      646 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/r2rml/R2RMLTC0002j/mapping.ttl
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/r2rml/R2RMLTC0002j/output.nq
+-rw-r--r--   0        0        0     8192 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/r2rml/R2RMLTC0002j/resource.db
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/r2rml/R2RMLTC0002j/resource.sql
+-rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/r2rml/R2RMLTC0002j/test_R2RMLTC0002j_SQLITE.py
+-rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/r2rml/R2RMLTC0003a/R2RMLTC0003a_SQLITE.py
+-rw-r--r--   0        0        0      711 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/r2rml/R2RMLTC0003a/mapping.ttl
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/r2rml/R2RMLTC0003a/output.nq
+-rw-r--r--   0        0        0     8192 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/r2rml/R2RMLTC0003a/resource.db
+-rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/r2rml/R2RMLTC0003a/resource.sql
+-rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/r2rml/R2RMLTC0003b/mapping.ttl
+-rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/r2rml/R2RMLTC0003b/output.nq
+-rw-r--r--   0        0        0     8192 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/r2rml/R2RMLTC0003b/resource.db
+-rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/r2rml/R2RMLTC0003b/resource.sql
+-rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/r2rml/R2RMLTC0003b/test_R2RMLTC0003b_SQLITE.py
+-rw-r--r--   0        0        0      533 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/r2rml/R2RMLTC0003c/mapping.ttl
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/r2rml/R2RMLTC0003c/output.nq
+-rw-r--r--   0        0        0     8192 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/r2rml/R2RMLTC0003c/resource.db
+-rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/r2rml/R2RMLTC0003c/resource.sql
+-rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/r2rml/R2RMLTC0003c/test_R2RMLTC0003c_SQLITE.py
+-rw-r--r--   0        0        0      839 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/r2rml/R2RMLTC0004a/mapping.ttl
+-rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/r2rml/R2RMLTC0004a/output.nq
+-rw-r--r--   0        0        0     8192 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/r2rml/R2RMLTC0004a/resource.db
+-rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/r2rml/R2RMLTC0004a/resource.sql
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/r2rml/R2RMLTC0004a/student_sport.csv
+-rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/r2rml/R2RMLTC0004a/test_R2RMLTC0004a_SQLITE.py
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/r2rml/R2RMLTC0004b/mapping.ttl
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/r2rml/R2RMLTC0004b/output.nq
+-rw-r--r--   0        0        0     8192 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/r2rml/R2RMLTC0004b/resource.db
+-rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/r2rml/R2RMLTC0004b/resource.sql
+-rw-r--r--   0        0        0      764 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/r2rml/R2RMLTC0004b/test_R2RMLTC0004b_SQLITE.py
+-rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/r2rml/R2RMLTC0005a/mapping.ttl
+-rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/r2rml/R2RMLTC0005a/output.nq
+-rw-r--r--   0        0        0     8192 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/r2rml/R2RMLTC0005a/resource.db
+-rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/r2rml/R2RMLTC0005a/resource.sql
+-rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/r2rml/R2RMLTC0005a/test_R2RMLTC0005a_SQLITE.py
+-rw-r--r--   0        0        0      817 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/r2rml/R2RMLTC0005b/mapping.ttl
+-rw-r--r--   0        0        0      542 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/r2rml/R2RMLTC0005b/output.nq
+-rw-r--r--   0        0        0     8192 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/r2rml/R2RMLTC0005b/resource.db
+-rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/r2rml/R2RMLTC0005b/resource.sql
+-rw-r--r--   0        0        0      794 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/r2rml/R2RMLTC0005b/test_R2RMLTC0005b_SQLITE.py
+-rw-r--r--   0        0        0      571 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/r2rml/R2RMLTC0006a/mapping.ttl
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/r2rml/R2RMLTC0006a/output.nq
+-rw-r--r--   0        0        0     8192 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/r2rml/R2RMLTC0006a/resource.db
+-rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/r2rml/R2RMLTC0006a/resource.sql
+-rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/r2rml/R2RMLTC0006a/test_R2RMLTC0006a_SQLITE.py
+-rw-r--r--   0        0        0      528 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/r2rml/R2RMLTC0007a/mapping.ttl
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/r2rml/R2RMLTC0007a/output.nq
+-rw-r--r--   0        0        0     8192 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/r2rml/R2RMLTC0007a/resource.db
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/r2rml/R2RMLTC0007a/resource.sql
+-rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/r2rml/R2RMLTC0007a/test_R2RMLTC0007a_SQLITE.py
+-rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/r2rml/R2RMLTC0007b/mapping.ttl
+-rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/r2rml/R2RMLTC0007b/output.nq
+-rw-r--r--   0        0        0     8192 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/r2rml/R2RMLTC0007b/resource.db
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/r2rml/R2RMLTC0007b/resource.sql
+-rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/r2rml/R2RMLTC0007b/test_R2RMLTC0007b_SQLITE.py
+-rw-r--r--   0        0        0      690 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/r2rml/R2RMLTC0007c/mapping.ttl
+-rw-r--r--   0        0        0      395 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/r2rml/R2RMLTC0007c/output.nq
+-rw-r--r--   0        0        0     8192 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/r2rml/R2RMLTC0007c/resource.db
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/r2rml/R2RMLTC0007c/resource.sql
+-rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/r2rml/R2RMLTC0007c/test_R2RMLTC0007c_SQLITE.py
+-rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/r2rml/R2RMLTC0007d/mapping.ttl
+-rw-r--r--   0        0        0      395 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/r2rml/R2RMLTC0007d/output.nq
+-rw-r--r--   0        0        0     8192 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/r2rml/R2RMLTC0007d/resource.db
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/r2rml/R2RMLTC0007d/resource.sql
+-rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/r2rml/R2RMLTC0007d/test_R2RMLTC0007d_SQLITE.py
+-rw-r--r--   0        0        0      709 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/r2rml/R2RMLTC0007e/mapping.ttl
+-rw-r--r--   0        0        0      419 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/r2rml/R2RMLTC0007e/output.nq
+-rw-r--r--   0        0        0     8192 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/r2rml/R2RMLTC0007e/resource.db
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/r2rml/R2RMLTC0007e/resource.sql
+-rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/r2rml/R2RMLTC0007e/test_R2RMLTC0007e_SQLITE.py
+-rw-r--r--   0        0        0      763 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/r2rml/R2RMLTC0007f/mapping.ttl
+-rw-r--r--   0        0        0      419 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/r2rml/R2RMLTC0007f/output.nq
+-rw-r--r--   0        0        0     8192 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/r2rml/R2RMLTC0007f/resource.db
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/r2rml/R2RMLTC0007f/resource.sql
+-rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/r2rml/R2RMLTC0007f/test_R2RMLTC0007f_SQLITE.py
+-rw-r--r--   0        0        0      676 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/r2rml/R2RMLTC0007g/mapping.ttl
+-rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/r2rml/R2RMLTC0007g/output.nq
+-rw-r--r--   0        0        0     8192 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/r2rml/R2RMLTC0007g/resource.db
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/r2rml/R2RMLTC0007g/resource.sql
+-rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/r2rml/R2RMLTC0007g/test_R2RMLTC0007g_SQLITE.py
+-rw-r--r--   0        0        0      708 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/r2rml/R2RMLTC0007h/mapping.ttl
+-rw-r--r--   0        0        0     8192 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/r2rml/R2RMLTC0007h/resource.db
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/r2rml/R2RMLTC0007h/resource.sql
+-rw-r--r--   0        0        0      737 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/r2rml/R2RMLTC0007h/test_R2RMLTC0007h_SQLITE.py
+-rw-r--r--   0        0        0      938 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/r2rml/R2RMLTC0008a/mapping.ttl
+-rw-r--r--   0        0        0      672 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/r2rml/R2RMLTC0008a/output.nq
+-rw-r--r--   0        0        0     8192 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/r2rml/R2RMLTC0008a/resource.db
+-rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/r2rml/R2RMLTC0008a/resource.sql
+-rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/r2rml/R2RMLTC0008a/test_R2RMLTC0008a_SQLITE.py
+-rw-r--r--   0        0        0     1235 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/r2rml/R2RMLTC0008b/mapping.ttl
+-rw-r--r--   0        0        0      541 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/r2rml/R2RMLTC0008b/output.nq
+-rw-r--r--   0        0        0     8192 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/r2rml/R2RMLTC0008b/resource.db
+-rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/r2rml/R2RMLTC0008b/resource.sql
+-rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/r2rml/R2RMLTC0008b/test_R2RMLTC0008b_SQLITE.py
+-rw-r--r--   0        0        0      568 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/r2rml/R2RMLTC0008c/mapping.ttl
+-rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/r2rml/R2RMLTC0008c/output.nq
+-rw-r--r--   0        0        0     8192 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/r2rml/R2RMLTC0008c/resource.db
+-rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/r2rml/R2RMLTC0008c/resource.sql
+-rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/r2rml/R2RMLTC0008c/test_R2RMLTC0008c_SQLITE.py
+-rw-r--r--   0        0        0     1129 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/r2rml/R2RMLTC0009a/mapping.ttl
+-rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/r2rml/R2RMLTC0009a/output.nq
+-rw-r--r--   0        0        0    12288 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/r2rml/R2RMLTC0009a/resource.db
+-rw-r--r--   0        0        0      444 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/r2rml/R2RMLTC0009a/resource.sql
+-rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/r2rml/R2RMLTC0009a/test_R2RMLTC0009a_SQLITE.py
+-rw-r--r--   0        0        0     1495 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/r2rml/R2RMLTC0009b/mapping.ttl
+-rw-r--r--   0        0        0     1198 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/r2rml/R2RMLTC0009b/output.nq
+-rw-r--r--   0        0        0    12288 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/r2rml/R2RMLTC0009b/resource.db
+-rw-r--r--   0        0        0      444 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/r2rml/R2RMLTC0009b/resource.sql
+-rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/r2rml/R2RMLTC0009b/test_R2RMLTC0009b_SQLITE.py
+-rw-r--r--   0        0        0      647 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/r2rml/R2RMLTC0009c/mapping.ttl
+-rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/r2rml/R2RMLTC0009c/output.nq
+-rw-r--r--   0        0        0    12288 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/r2rml/R2RMLTC0009c/resource.db
+-rw-r--r--   0        0        0      444 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/r2rml/R2RMLTC0009c/resource.sql
+-rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/r2rml/R2RMLTC0009c/test_R2RMLTC0009c_SQLITE.py
+-rw-r--r--   0        0        0      773 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/r2rml/R2RMLTC0009d/mapping.ttl
+-rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/r2rml/R2RMLTC0009d/output.nq
+-rw-r--r--   0        0        0    12288 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/r2rml/R2RMLTC0009d/resource.db
+-rw-r--r--   0        0        0      444 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/r2rml/R2RMLTC0009d/resource.sql
+-rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/r2rml/R2RMLTC0009d/test_R2RMLTC0009d_SQLITE.py
+-rw-r--r--   0        0        0      468 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/r2rml/R2RMLTC0010a/mapping.ttl
+-rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/r2rml/R2RMLTC0010a/output.nq
+-rw-r--r--   0        0        0     8192 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/r2rml/R2RMLTC0010a/resource.db
+-rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/r2rml/R2RMLTC0010a/resource.sql
+-rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/r2rml/R2RMLTC0010a/test_R2RMLTC0010a_SQLITE.py
+-rw-r--r--   0        0        0      480 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/r2rml/R2RMLTC0010b/mapping.ttl
+-rw-r--r--   0        0        0      312 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/r2rml/R2RMLTC0010b/output.nq
+-rw-r--r--   0        0        0     8192 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/r2rml/R2RMLTC0010b/resource.db
+-rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/r2rml/R2RMLTC0010b/resource.sql
+-rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/r2rml/R2RMLTC0010b/test_R2RMLTC0010b_SQLITE.py
+-rw-r--r--   0        0        0      530 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/r2rml/R2RMLTC0010c/mapping.ttl
+-rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/r2rml/R2RMLTC0010c/output.nq
+-rw-r--r--   0        0        0     8192 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/r2rml/R2RMLTC0010c/resource.db
+-rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/r2rml/R2RMLTC0010c/resource.sql
+-rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/r2rml/R2RMLTC0010c/test_R2RMLTC0010c_SQLITE.py
+-rw-r--r--   0        0        0     1660 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/r2rml/R2RMLTC0011a/mapping.ttl
+-rw-r--r--   0        0        0     1525 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/r2rml/R2RMLTC0011a/output.nq
+-rw-r--r--   0        0        0    20480 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/r2rml/R2RMLTC0011a/resource.db
+-rw-r--r--   0        0        0     1143 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/r2rml/R2RMLTC0011a/resource.sql
+-rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/r2rml/R2RMLTC0011a/test_R2RMLTC0011a_SQLITE.py
+-rw-r--r--   0        0        0     1248 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/r2rml/R2RMLTC0011b/mapping.ttl
+-rw-r--r--   0        0        0     1228 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/r2rml/R2RMLTC0011b/output.nq
+-rw-r--r--   0        0        0    20480 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/r2rml/R2RMLTC0011b/resource.db
+-rw-r--r--   0        0        0     1143 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/r2rml/R2RMLTC0011b/resource.sql
+-rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/r2rml/R2RMLTC0011b/test_R2RMLTC0011b_SQLITE.py
+-rw-r--r--   0        0        0      700 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/r2rml/R2RMLTC0012a/mapping.ttl
+-rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/r2rml/R2RMLTC0012a/output.nq
+-rw-r--r--   0        0        0    12288 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/r2rml/R2RMLTC0012a/resource.db
+-rw-r--r--   0        0        0      680 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/r2rml/R2RMLTC0012a/resource.sql
+-rw-r--r--   0        0        0      794 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/r2rml/R2RMLTC0012a/test_R2RMLTC0012a_SQLITE.py
+-rw-r--r--   0        0        0      898 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/r2rml/R2RMLTC0012b/mapping.ttl
+-rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/r2rml/R2RMLTC0012b/output.nq
+-rw-r--r--   0        0        0    12288 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/r2rml/R2RMLTC0012b/resource.db
+-rw-r--r--   0        0        0      680 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/r2rml/R2RMLTC0012b/resource.sql
+-rw-r--r--   0        0        0      794 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/r2rml/R2RMLTC0012b/test_R2RMLTC0012b_SQLITE.py
+-rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/r2rml/R2RMLTC0012c/mapping.ttl
+-rw-r--r--   0        0        0    12288 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/r2rml/R2RMLTC0012c/resource.db
+-rw-r--r--   0        0        0      680 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/r2rml/R2RMLTC0012c/resource.sql
+-rw-r--r--   0        0        0      764 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/r2rml/R2RMLTC0012c/test_R2RMLTC0012c_SQLITE.py
+-rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/r2rml/R2RMLTC0012d/mapping.ttl
+-rw-r--r--   0        0        0    12288 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/r2rml/R2RMLTC0012d/resource.db
+-rw-r--r--   0        0        0      680 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/r2rml/R2RMLTC0012d/resource.sql
+-rw-r--r--   0        0        0      764 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/r2rml/R2RMLTC0012d/test_R2RMLTC0012d_SQLITE.py
+-rw-r--r--   0        0        0     1500 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/r2rml/R2RMLTC0012e/mapping.ttl
+-rw-r--r--   0        0        0     1252 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/r2rml/R2RMLTC0012e/output.nq
+-rw-r--r--   0        0        0    12288 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/r2rml/R2RMLTC0012e/resource.db
+-rw-r--r--   0        0        0      680 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/r2rml/R2RMLTC0012e/resource.sql
+-rw-r--r--   0        0        0      794 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/r2rml/R2RMLTC0012e/test_R2RMLTC0012e_SQLITE.py
+-rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/r2rml/R2RMLTC0013a/mapping.ttl
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/r2rml/R2RMLTC0013a/output.nq
+-rw-r--r--   0        0        0     8192 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/r2rml/R2RMLTC0013a/resource.db
+-rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/r2rml/R2RMLTC0013a/resource.sql
+-rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/r2rml/R2RMLTC0013a/test_R2RMLTC0013a_SQLITE.py
+-rw-r--r--   0        0        0      843 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/r2rml/R2RMLTC0014d/mapping.ttl
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/r2rml/R2RMLTC0014d/output.nq
+-rw-r--r--   0        0        0    20480 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/r2rml/R2RMLTC0014d/resource.db
+-rw-r--r--   0        0        0      775 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/r2rml/R2RMLTC0014d/resource.sql
+-rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/r2rml/R2RMLTC0014d/test_R2RMLTC0014d_SQLITE.py
+-rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/r2rml/R2RMLTC0015a/mapping.ttl
+-rw-r--r--   0        0        0      386 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/r2rml/R2RMLTC0015a/output.nq
+-rw-r--r--   0        0        0    12288 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/r2rml/R2RMLTC0015a/resource.db
+-rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/r2rml/R2RMLTC0015a/resource.sql
+-rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/r2rml/R2RMLTC0015a/test_R2RMLTC0015a_SQLITE.py
+-rw-r--r--   0        0        0     1122 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/r2rml/R2RMLTC0015b/mapping.ttl
+-rw-r--r--   0        0        0    12288 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/r2rml/R2RMLTC0015b/resource.db
+-rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/r2rml/R2RMLTC0015b/resource.sql
+-rw-r--r--   0        0        0      764 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/r2rml/R2RMLTC0015b/test_R2RMLTC0015b_SQLITE.py
+-rw-r--r--   0        0        0      974 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/r2rml/R2RMLTC0016a/mapping.ttl
+-rw-r--r--   0        0        0     1197 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/r2rml/R2RMLTC0016a/output.nq
+-rw-r--r--   0        0        0     8192 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/r2rml/R2RMLTC0016a/resource.db
+-rw-r--r--   0        0        0     1435 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/r2rml/R2RMLTC0016a/resource.sql
+-rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/r2rml/R2RMLTC0016a/test_R2RMLTC0016a_SQLITE.py
+-rw-r--r--   0        0        0      910 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/r2rml/R2RMLTC0016b/R2RMLTC0016b_SQLITE.py
+-rw-r--r--   0        0        0      751 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/r2rml/R2RMLTC0016b/mapping.ttl
+-rw-r--r--   0        0        0      776 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/r2rml/R2RMLTC0016b/output.nq
+-rw-r--r--   0        0        0     8192 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/r2rml/R2RMLTC0016b/resource.db
+-rw-r--r--   0        0        0     1435 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/r2rml/R2RMLTC0016b/resource.sql
+-rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/r2rml/R2RMLTC0016c/R2RMLTC0016c_SQLITE.py
+-rw-r--r--   0        0        0      769 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/r2rml/R2RMLTC0016c/mapping.ttl
+-rw-r--r--   0        0        0     1110 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/r2rml/R2RMLTC0016c/output.nq
+-rw-r--r--   0        0        0     8192 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/r2rml/R2RMLTC0016c/resource.db
+-rw-r--r--   0        0        0     1435 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/r2rml/R2RMLTC0016c/resource.sql
+-rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/r2rml/R2RMLTC0016d/R2RMLTC0016d_SQLITE.py
+-rw-r--r--   0        0        0      641 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/r2rml/R2RMLTC0016d/mapping.ttl
+-rw-r--r--   0        0        0      685 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/r2rml/R2RMLTC0016d/output.nq
+-rw-r--r--   0        0        0     8192 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/r2rml/R2RMLTC0016d/resource.db
+-rw-r--r--   0        0        0     1435 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/r2rml/R2RMLTC0016d/resource.sql
+-rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/r2rml/R2RMLTC0016e/R2RMLTC0016e_SQLITE.py
+-rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/r2rml/R2RMLTC0016e/mapping.ttl
+-rw-r--r--   0        0        0     1110 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/r2rml/R2RMLTC0016e/output.nq
+-rw-r--r--   0        0        0     8192 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/r2rml/R2RMLTC0016e/resource.db
+-rw-r--r--   0        0        0     1435 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/r2rml/R2RMLTC0016e/resource.sql
+-rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/r2rml/R2RMLTC0018a/mapping.ttl
+-rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/r2rml/R2RMLTC0018a/output.nq
+-rw-r--r--   0        0        0     8192 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/r2rml/R2RMLTC0018a/resource.db
+-rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/r2rml/R2RMLTC0018a/resource.sql
+-rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/r2rml/R2RMLTC0018a/test_R2RMLTC0018a_SQLITE.py
+-rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/r2rml/R2RMLTC0019a/R2RMLTC0019a_SQLITE.py
+-rw-r--r--   0        0        0      654 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/r2rml/R2RMLTC0019a/mapping.ttl
+-rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/r2rml/R2RMLTC0019a/output.nq
+-rw-r--r--   0        0        0     8192 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/r2rml/R2RMLTC0019a/resource.db
+-rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/r2rml/R2RMLTC0019a/resource.sql
+-rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/r2rml/R2RMLTC0019b/R2RMLTC0019b_SQLITE.py
+-rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/r2rml/R2RMLTC0019b/mapping.ttl
+-rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/r2rml/R2RMLTC0019b/output.nq
+-rw-r--r--   0        0        0     8192 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/r2rml/R2RMLTC0019b/resource.db
+-rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/r2rml/R2RMLTC0019b/resource.sql
+-rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/r2rml/R2RMLTC0020a/R2RMLTC0020a_SQLITE.py
+-rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/r2rml/R2RMLTC0020a/mapping.ttl
+-rw-r--r--   0        0        0      658 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/r2rml/R2RMLTC0020a/output.nq
+-rw-r--r--   0        0        0     8192 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/r2rml/R2RMLTC0020a/resource.db
+-rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/r2rml/R2RMLTC0020a/resource.sql
+-rw-r--r--   0        0        0      764 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/r2rml/R2RMLTC0020b/R2RMLTC0020b_SQLITE.py
+-rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/r2rml/R2RMLTC0020b/mapping.ttl
+-rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/r2rml/R2RMLTC0020b/output.nq
+-rw-r--r--   0        0        0     8192 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/r2rml/R2RMLTC0020b/resource.db
+-rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/r2rml/R2RMLTC0020b/resource.sql
+-rw-r--r--   0        0        0      551 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/csv/RMLTC0000/mapping.ttl
+-rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/csv/RMLTC0000/output.nq
+-rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/csv/RMLTC0000/student.csv
+-rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/csv/RMLTC0000/test_RMLTC0000_CSV.py
+-rw-r--r--   0        0        0      551 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/csv/RMLTC0001a/mapping.ttl
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/csv/RMLTC0001a/output.nq
+-rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/csv/RMLTC0001a/student.csv
+-rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/csv/RMLTC0001a/test_RMLTC0001a_CSV.py
+-rw-r--r--   0        0        0      562 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/csv/RMLTC0001b/mapping.ttl
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/csv/RMLTC0001b/output.nq
+-rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/csv/RMLTC0001b/student.csv
+-rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/csv/RMLTC0001b/test_RMLTC0001b_CSV.py
+-rw-r--r--   0        0        0      670 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/csv/RMLTC0002a/mapping.ttl
+-rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/csv/RMLTC0002a/output.nq
+-rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/csv/RMLTC0002a/student.csv
+-rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/csv/RMLTC0002a/test_RMLTC0002a_CSV.py
+-rw-r--r--   0        0        0      556 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/csv/RMLTC0002b/mapping.ttl
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/csv/RMLTC0002b/output.nq
+-rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/csv/RMLTC0002b/student.csv
+-rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/csv/RMLTC0002b/test_RMLTC0002b_CSV.py
+-rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/csv/RMLTC0002c/mapping.ttl
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/csv/RMLTC0002c/output.nq
+-rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/csv/RMLTC0002c/student.csv
+-rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/csv/RMLTC0002c/test_RMLTC0002c_CSV.py
+-rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/csv/RMLTC0002e/mapping.ttl
+-rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/csv/RMLTC0002e/student.csv
+-rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/csv/RMLTC0002e/test_RMLTC0002e_CSV.py
+-rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/csv/RMLTC0003c/mapping.ttl
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/csv/RMLTC0003c/output.nq
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/csv/RMLTC0003c/student.csv
+-rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/csv/RMLTC0003c/test_RMLTC0003c_CSV.py
+-rw-r--r--   0        0        0      961 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/csv/RMLTC0004a/mapping.ttl
+-rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/csv/RMLTC0004a/output.nq
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/csv/RMLTC0004a/student_sport.csv
+-rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/csv/RMLTC0004a/test_RMLTC0004a_CSV.py
+-rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/csv/RMLTC0004b/mapping.ttl
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/csv/RMLTC0004b/output.nq
+-rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/csv/RMLTC0004b/student.csv
+-rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/csv/RMLTC0004b/test_RMLTC0004b_CSV.py
+-rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/csv/RMLTC0005a/ious.csv
+-rw-r--r--   0        0        0      572 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/csv/RMLTC0005a/mapping.ttl
+-rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/csv/RMLTC0005a/output.nq
+-rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/csv/RMLTC0005a/test_RMLTC0005a_CSV.py
+-rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/csv/RMLTC0006a/mapping.ttl
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/csv/RMLTC0006a/output.nq
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/csv/RMLTC0006a/student.csv
+-rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/csv/RMLTC0006a/test_RMLTC0006a_CSV.py
+-rw-r--r--   0        0        0      600 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/csv/RMLTC0007a/mapping.ttl
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/csv/RMLTC0007a/output.nq
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/csv/RMLTC0007a/student.csv
+-rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/csv/RMLTC0007a/test_RMLTC0007a_CSV.py
+-rw-r--r--   0        0        0      740 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/csv/RMLTC0007b/mapping.ttl
+-rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/csv/RMLTC0007b/output.nq
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/csv/RMLTC0007b/student.csv
+-rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/csv/RMLTC0007b/test_RMLTC0007b_CSV.py
+-rw-r--r--   0        0        0      701 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/csv/RMLTC0007c/mapping.ttl
+-rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/csv/RMLTC0007c/output.nq
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/csv/RMLTC0007c/student.csv
+-rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/csv/RMLTC0007c/test_RMLTC0007c_CSV.py
+-rw-r--r--   0        0        0      897 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/csv/RMLTC0007d/mapping.ttl
+-rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/csv/RMLTC0007d/output.nq
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/csv/RMLTC0007d/student.csv
+-rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/csv/RMLTC0007d/test_RMLTC0007d_CSV.py
+-rw-r--r--   0        0        0      722 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/csv/RMLTC0007e/mapping.ttl
+-rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/csv/RMLTC0007e/output.nq
+-rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/csv/RMLTC0007e/student.csv
+-rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/csv/RMLTC0007e/test_RMLTC0007e_CSV.py
+-rw-r--r--   0        0        0      842 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/csv/RMLTC0007f/mapping.ttl
+-rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/csv/RMLTC0007f/output.nq
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/csv/RMLTC0007f/student.csv
+-rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/csv/RMLTC0007f/test_RMLTC0007f_CSV.py
+-rw-r--r--   0        0        0      602 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/csv/RMLTC0007g/mapping.ttl
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/csv/RMLTC0007g/output.nq
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/csv/RMLTC0007g/student.csv
+-rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/csv/RMLTC0007g/test_RMLTC0007g_CSV.py
+-rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/csv/RMLTC0007h/mapping.ttl
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/csv/RMLTC0007h/student.csv
+-rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/csv/RMLTC0007h/test_RMLTC0007h_CSV.py
+-rw-r--r--   0        0        0      993 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/csv/RMLTC0008a/mapping.ttl
+-rw-r--r--   0        0        0      627 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/csv/RMLTC0008a/output.nq
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/csv/RMLTC0008a/student.csv
+-rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/csv/RMLTC0008a/test_RMLTC0008a_CSV.py
+-rw-r--r--   0        0        0     1345 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/csv/RMLTC0008b/mapping.ttl
+-rw-r--r--   0        0        0      544 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/csv/RMLTC0008b/output.nq
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/csv/RMLTC0008b/student.csv
+-rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/csv/RMLTC0008b/test_RMLTC0008b_CSV.py
+-rw-r--r--   0        0        0      627 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/csv/RMLTC0008c/mapping.ttl
+-rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/csv/RMLTC0008c/output.nq
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/csv/RMLTC0008c/student.csv
+-rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/csv/RMLTC0008c/test_RMLTC0008c_CSV.py
+-rw-r--r--   0        0        0     1276 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/csv/RMLTC0009a/mapping.ttl
+-rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/csv/RMLTC0009a/output.nq
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/csv/RMLTC0009a/sport.csv
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/csv/RMLTC0009a/student.csv
+-rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/csv/RMLTC0009a/test_RMLTC0009a_CSV.py
+-rw-r--r--   0        0        0     1603 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/csv/RMLTC0009b/mapping.ttl
+-rw-r--r--   0        0        0     1198 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/csv/RMLTC0009b/output.nq
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/csv/RMLTC0009b/sport.csv
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/csv/RMLTC0009b/student.csv
+-rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/csv/RMLTC0009b/test_RMLTC0009b_CSV.py
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/csv/RMLTC0010a/country_info.csv
+-rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/csv/RMLTC0010a/mapping.ttl
+-rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/csv/RMLTC0010a/output.nq
+-rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/csv/RMLTC0010a/test_RMLTC0010a_CSV.py
+-rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/csv/RMLTC0010b/country_info.csv
+-rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/csv/RMLTC0010b/mapping.ttl
+-rw-r--r--   0        0        0      312 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/csv/RMLTC0010b/output.nq
+-rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/csv/RMLTC0010b/test_RMLTC0010b_CSV.py
+-rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/csv/RMLTC0010c/country_info.csv
+-rw-r--r--   0        0        0      654 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/csv/RMLTC0010c/mapping.ttl
+-rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/csv/RMLTC0010c/output.nq
+-rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/csv/RMLTC0010c/test_RMLTC0010c_CSV.py
+-rw-r--r--   0        0        0     1548 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/csv/RMLTC0011b/mapping.ttl
+-rw-r--r--   0        0        0     1229 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/csv/RMLTC0011b/output.nq
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/csv/RMLTC0011b/sport.csv
+-rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/csv/RMLTC0011b/student.csv
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/csv/RMLTC0011b/student_sport.csv
+-rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/csv/RMLTC0011b/test_RMLTC0011b_CSV.py
+-rw-r--r--   0        0        0      737 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/csv/RMLTC0012a/mapping.ttl
+-rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/csv/RMLTC0012a/output.nq
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/csv/RMLTC0012a/persons.csv
+-rw-r--r--   0        0        0      652 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/csv/RMLTC0012a/test_RMLTC0012a_CSV.py
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/csv/RMLTC0012b/lives.csv
+-rw-r--r--   0        0        0      989 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/csv/RMLTC0012b/mapping.ttl
+-rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/csv/RMLTC0012b/output.nq
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/csv/RMLTC0012b/persons.csv
+-rw-r--r--   0        0        0      652 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/csv/RMLTC0012b/test_RMLTC0012b_CSV.py
+-rw-r--r--   0        0        0      647 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/csv/RMLTC0012c/mapping.ttl
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/csv/RMLTC0012c/persons.csv
+-rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/csv/RMLTC0012c/test_RMLTC0012c_CSV.py
+-rw-r--r--   0        0        0      831 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/csv/RMLTC0012d/mapping.ttl
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/csv/RMLTC0012d/persons.csv
+-rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/csv/RMLTC0012d/test_RMLTC0012d_CSV.py
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/csv/RMLTC0015a/country_en.csv
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/csv/RMLTC0015a/country_es.csv
+-rw-r--r--   0        0        0     1009 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/csv/RMLTC0015a/mapping.ttl
+-rw-r--r--   0        0        0      386 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/csv/RMLTC0015a/output.nq
+-rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/csv/RMLTC0015a/test_RMLTC0015a_CSV.py
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/csv/RMLTC0015b/country_en.csv
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/csv/RMLTC0015b/country_es.csv
+-rw-r--r--   0        0        0     1007 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/csv/RMLTC0015b/mapping.ttl
+-rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/csv/RMLTC0015b/test_RMLTC0015b_CSV.py
+-rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/csv/RMLTC0019a/RMLTC0019a_CSV.py
+-rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/csv/RMLTC0019a/mapping.ttl
+-rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/csv/RMLTC0019a/output.nq
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/csv/RMLTC0019a/persons.csv
+-rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/csv/RMLTC0019b/RMLTC0019b_CSV.py
+-rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/csv/RMLTC0019b/mapping.ttl
+-rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/csv/RMLTC0019b/output.nq
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/csv/RMLTC0019b/persons.csv
+-rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/csv/RMLTC0020a/RMLTC0020a_CSV.py
+-rw-r--r--   0        0        0      647 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/csv/RMLTC0020a/mapping.ttl
+-rw-r--r--   0        0        0      658 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/csv/RMLTC0020a/output.nq
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/csv/RMLTC0020a/student.csv
+-rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/csv/RMLTC0020b/RMLTC0020b_CSV.py
+-rw-r--r--   0        0        0      646 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/csv/RMLTC0020b/mapping.ttl
+-rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/csv/RMLTC0020b/output.nq
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/csv/RMLTC0020b/student.csv
+-rw-r--r--   0        0        0      671 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/csv/null_filter/mapping.ttl
+-rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/csv/null_filter/output.nq
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/csv/null_filter/student.csv
+-rw-r--r--   0        0        0      689 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/csv/null_filter/test_null_filter_CSV.py
+-rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/csv/triples_map_without_pom/mapping.ttl
+-rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/csv/triples_map_without_pom/output.nq
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/csv/triples_map_without_pom/sport.csv
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/csv/triples_map_without_pom/student.csv
+-rw-r--r--   0        0        0      701 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/csv/triples_map_without_pom/test_triples_map_without_pom_CSV.py
+-rw-r--r--   0        0        0      592 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/json/RMLTC0000/mapping.ttl
+-rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/json/RMLTC0000/output.nq
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/json/RMLTC0000/student.json
+-rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/json/RMLTC0000/test_RMLTC0000_JSON.py
+-rw-r--r--   0        0        0      621 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/json/RMLTC0001a/mapping.ttl
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/json/RMLTC0001a/output.nq
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/json/RMLTC0001a/student.json
+-rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/json/RMLTC0001a/test_RMLTC0001a_JSON.py
+-rw-r--r--   0        0        0      603 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/json/RMLTC0001b/mapping.ttl
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/json/RMLTC0001b/output.nq
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/json/RMLTC0001b/student.json
+-rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/json/RMLTC0001b/test_RMLTC0001b_JSON.py
+-rw-r--r--   0        0        0      711 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/json/RMLTC0002a/mapping.ttl
+-rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/json/RMLTC0002a/output.nq
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/json/RMLTC0002a/student.json
+-rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/json/RMLTC0002a/test_RMLTC0002a_JSON.py
+-rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/json/RMLTC0002b/mapping.ttl
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/json/RMLTC0002b/output.nq
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/json/RMLTC0002b/student.json
+-rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/json/RMLTC0002b/test_RMLTC0002b_JSON.py
+-rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/json/RMLTC0002c/mapping.ttl
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/json/RMLTC0002c/output.nq
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/json/RMLTC0002c/student.json
+-rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/json/RMLTC0002c/test_RMLTC0002c_JSON.py
+-rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/json/RMLTC0002e/mapping.ttl
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/json/RMLTC0002e/student.json
+-rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/json/RMLTC0002e/test_RMLTC0002e_JSON.py
+-rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/json/RMLTC0003c/mapping.ttl
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/json/RMLTC0003c/output.nq
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/json/RMLTC0003c/student.json
+-rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/json/RMLTC0003c/test_RMLTC0003c_JSON.py
+-rw-r--r--   0        0        0     1043 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/json/RMLTC0004a/mapping.ttl
+-rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/json/RMLTC0004a/output.nq
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/json/RMLTC0004a/student_sport.json
+-rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/json/RMLTC0004a/test_RMLTC0004a_JSON.py
+-rw-r--r--   0        0        0      621 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/json/RMLTC0004b/mapping.ttl
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/json/RMLTC0004b/output.nq
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/json/RMLTC0004b/student.json
+-rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/json/RMLTC0004b/test_RMLTC0004b_JSON.py
+-rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/json/RMLTC0005a/ious.json
+-rw-r--r--   0        0        0      612 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/json/RMLTC0005a/mapping.ttl
+-rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/json/RMLTC0005a/output.nq
+-rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/json/RMLTC0005a/test_RMLTC0005a_JSON.py
+-rw-r--r--   0        0        0      667 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/json/RMLTC0006a/mapping.ttl
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/json/RMLTC0006a/output.nq
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/json/RMLTC0006a/student.json
+-rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/json/RMLTC0006a/test_RMLTC0006a_JSON.py
+-rw-r--r--   0        0        0      641 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/json/RMLTC0007a/mapping.ttl
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/json/RMLTC0007a/output.nq
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/json/RMLTC0007a/student.json
+-rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/json/RMLTC0007a/test_RMLTC0007a_JSON.py
+-rw-r--r--   0        0        0      781 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/json/RMLTC0007b/mapping.ttl
+-rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/json/RMLTC0007b/output.nq
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/json/RMLTC0007b/student.json
+-rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/json/RMLTC0007b/test_RMLTC0007b_JSON.py
+-rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/json/RMLTC0007c/mapping.ttl
+-rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/json/RMLTC0007c/output.nq
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/json/RMLTC0007c/student.json
+-rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/json/RMLTC0007c/test_RMLTC0007c_JSON.py
+-rw-r--r--   0        0        0      936 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/json/RMLTC0007d/mapping.ttl
+-rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/json/RMLTC0007d/output.nq
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/json/RMLTC0007d/student.json
+-rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/json/RMLTC0007d/test_RMLTC0007d_JSON.py
+-rw-r--r--   0        0        0      751 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/json/RMLTC0007e/mapping.ttl
+-rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/json/RMLTC0007e/output.nq
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/json/RMLTC0007e/student.json
+-rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/json/RMLTC0007e/test_RMLTC0007e_JSON.py
+-rw-r--r--   0        0        0      883 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/json/RMLTC0007f/mapping.ttl
+-rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/json/RMLTC0007f/output.nq
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/json/RMLTC0007f/student.json
+-rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/json/RMLTC0007f/test_RMLTC0007f_JSON.py
+-rw-r--r--   0        0        0      643 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/json/RMLTC0007g/mapping.ttl
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/json/RMLTC0007g/output.nq
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/json/RMLTC0007g/student.json
+-rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/json/RMLTC0007g/test_RMLTC0007g_JSON.py
+-rw-r--r--   0        0        0      686 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/json/RMLTC0007h/mapping.ttl
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/json/RMLTC0007h/student.json
+-rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/json/RMLTC0007h/test_RMLTC0007h_JSON.py
+-rw-r--r--   0        0        0     1034 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/json/RMLTC0008a/mapping.ttl
+-rw-r--r--   0        0        0      627 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/json/RMLTC0008a/output.nq
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/json/RMLTC0008a/student.json
+-rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/json/RMLTC0008a/test_RMLTC0008a_JSON.py
+-rw-r--r--   0        0        0     1427 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/json/RMLTC0008b/mapping.ttl
+-rw-r--r--   0        0        0      544 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/json/RMLTC0008b/output.nq
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/json/RMLTC0008b/student.json
+-rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/json/RMLTC0008b/test_RMLTC0008b_JSON.py
+-rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/json/RMLTC0008c/mapping.ttl
+-rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/json/RMLTC0008c/output.nq
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/json/RMLTC0008c/student.json
+-rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/json/RMLTC0008c/test_RMLTC0008c_JSON.py
+-rw-r--r--   0        0        0     1356 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/json/RMLTC0009a/mapping.ttl
+-rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/json/RMLTC0009a/output.nq
+-rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/json/RMLTC0009a/sport.json
+-rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/json/RMLTC0009a/student.json
+-rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/json/RMLTC0009a/test_RMLTC0009a_JSON.py
+-rw-r--r--   0        0        0     1673 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/json/RMLTC0009b/mapping.ttl
+-rw-r--r--   0        0        0     1198 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/json/RMLTC0009b/output.nq
+-rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/json/RMLTC0009b/sport.json
+-rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/json/RMLTC0009b/student.json
+-rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/json/RMLTC0009b/test_RMLTC0009b_JSON.py
+-rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/json/RMLTC0010a/country_info.json
+-rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/json/RMLTC0010a/mapping.ttl
+-rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/json/RMLTC0010a/output.nq
+-rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/json/RMLTC0010a/test_RMLTC0010a_JSON.py
+-rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/json/RMLTC0010b/country_info.json
+-rw-r--r--   0        0        0      646 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/json/RMLTC0010b/mapping.ttl
+-rw-r--r--   0        0        0      312 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/json/RMLTC0010b/output.nq
+-rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/json/RMLTC0010b/test_RMLTC0010b_JSON.py
+-rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/json/RMLTC0010c/country_info.json
+-rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/json/RMLTC0010c/mapping.ttl
+-rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/json/RMLTC0010c/output.nq
+-rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/json/RMLTC0010c/test_RMLTC0010c_JSON.py
+-rw-r--r--   0        0        0     1666 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/json/RMLTC0011b/mapping.ttl
+-rw-r--r--   0        0        0     1229 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/json/RMLTC0011b/output.nq
+-rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/json/RMLTC0011b/sport.json
+-rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/json/RMLTC0011b/student.json
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/json/RMLTC0011b/student_sport.json
+-rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/json/RMLTC0011b/test_RMLTC0011b_JSON.py
+-rw-r--r--   0        0        0      777 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/json/RMLTC0012a/mapping.ttl
+-rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/json/RMLTC0012a/output.nq
+-rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/json/RMLTC0012a/persons.json
+-rw-r--r--   0        0        0      652 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/json/RMLTC0012a/test_RMLTC0012a_JSON.py
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/json/RMLTC0012b/lives.json
+-rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/json/RMLTC0012b/mapping.ttl
+-rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/json/RMLTC0012b/output.nq
+-rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/json/RMLTC0012b/persons.json
+-rw-r--r--   0        0        0      652 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/json/RMLTC0012b/test_RMLTC0012b_JSON.py
+-rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/json/RMLTC0012c/mapping.ttl
+-rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/json/RMLTC0012c/persons.json
+-rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/json/RMLTC0012c/test_RMLTC0012c_JSON.py
+-rw-r--r--   0        0        0      871 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/json/RMLTC0012d/mapping.ttl
+-rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/json/RMLTC0012d/persons.json
+-rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/json/RMLTC0012d/test_RMLTC0012d_JSON.py
+-rw-r--r--   0        0        0      621 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/json/RMLTC0013a/mapping.ttl
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/json/RMLTC0013a/output.nq
+-rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/json/RMLTC0013a/persons.json
+-rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/json/RMLTC0013a/test_RMLTC0013a_JSON.py
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/json/RMLTC0015a/country_en.json
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/json/RMLTC0015a/country_es.json
+-rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/json/RMLTC0015a/mapping.ttl
+-rw-r--r--   0        0        0      386 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/json/RMLTC0015a/output.nq
+-rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/json/RMLTC0015a/test_RMLTC0015a_JSON.py
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/json/RMLTC0015b/country_en.json
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/json/RMLTC0015b/country_es.json
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/json/RMLTC0015b/mapping.ttl
+-rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/json/RMLTC0015b/test_RMLTC0015b_JSON.py
+-rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/json/RMLTC0019a/RMLTC0019a_JSON.py
+-rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/json/RMLTC0019a/mapping.ttl
+-rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/json/RMLTC0019a/output.nq
+-rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/json/RMLTC0019a/persons.json
+-rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/json/RMLTC0019b/RMLTC0019b_JSON.py
+-rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/json/RMLTC0019b/mapping.ttl
+-rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/json/RMLTC0019b/output.nq
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/json/RMLTC0019b/persons.json
+-rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/json/RMLTC0020a/RMLTC0020a_JSON.py
+-rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/json/RMLTC0020a/mapping.ttl
+-rw-r--r--   0        0        0      658 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/json/RMLTC0020a/output.nq
+-rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/json/RMLTC0020a/student.json
+-rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/json/RMLTC0020b/RMLTC0020b_JSON.py
+-rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/json/RMLTC0020b/mapping.ttl
+-rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/json/RMLTC0020b/output.nq
+-rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/json/RMLTC0020b/student.json
+-rw-r--r--   0        0        0     3464 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/json/complex/data.json
+-rw-r--r--   0        0        0     9778 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/json/complex/mapping.ttl
+-rw-r--r--   0        0        0     1791 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/json/complex/mapping.yaml
+-rw-r--r--   0        0        0     3729 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/json/complex/output.nq
+-rw-r--r--   0        0        0     2021 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/json/complex/test_complex_JSON.py
+-rw-r--r--   0        0        0      681 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/tabular/RMLTC0002a_EXCEL/mapping.ttl
+-rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/tabular/RMLTC0002a_EXCEL/output.nq
+-rw-r--r--   0        0        0     4925 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/tabular/RMLTC0002a_EXCEL/student.xlsx
+-rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/tabular/RMLTC0002a_EXCEL/test_RMLTC0002a_EXCEL.py
+-rw-r--r--   0        0        0      686 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/tabular/RMLTC0002a_FEATHER/mapping.ttl
+-rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/tabular/RMLTC0002a_FEATHER/output.nq
+-rw-r--r--   0        0        0     1538 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/tabular/RMLTC0002a_FEATHER/student.feather
+-rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/tabular/RMLTC0002a_FEATHER/test_RMLTC0002a_FEATHER.py
+-rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/tabular/RMLTC0002a_ODS/mapping.ttl
+-rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/tabular/RMLTC0002a_ODS/output.nq
+-rw-r--r--   0        0        0     5269 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/tabular/RMLTC0002a_ODS/student.ods
+-rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/tabular/RMLTC0002a_ODS/test_RMLTC0002a_ODS.py
+-rw-r--r--   0        0        0      686 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/tabular/RMLTC0002a_PARQUET/mapping.ttl
+-rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/tabular/RMLTC0002a_PARQUET/output.nq
+-rw-r--r--   0        0        0     1746 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/tabular/RMLTC0002a_PARQUET/student.parquet
+-rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/tabular/RMLTC0002a_PARQUET/test_RMLTC0002a_PARQUET.py
+-rw-r--r--   0        0        0      680 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/tabular/RMLTC0002a_STATA/mapping.ttl
+-rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/tabular/RMLTC0002a_STATA/output.nq
+-rw-r--r--   0        0        0     1844 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/tabular/RMLTC0002a_STATA/student.dta
+-rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/tabular/RMLTC0002a_STATA/test_RMLTC0002a_STATA.py
+-rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/tabular/RMLTC0002a_TSV/mapping.ttl
+-rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/tabular/RMLTC0002a_TSV/output.nq
+-rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/tabular/RMLTC0002a_TSV/student.tsv
+-rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/tabular/RMLTC0002a_TSV/test_RMLTC0002a_TSV.py
+-rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/xml/RMLTC0000/mapping.ttl
+-rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/xml/RMLTC0000/output.nq
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/xml/RMLTC0000/student.xml
+-rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/xml/RMLTC0000/test_RMLTC0000_XML.py
+-rw-r--r--   0        0        0      590 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/xml/RMLTC0001a/mapping.ttl
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/xml/RMLTC0001a/output.nq
+-rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/xml/RMLTC0001a/student.xml
+-rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/xml/RMLTC0001a/test_RMLTC0001a_XML.py
+-rw-r--r--   0        0        0      602 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/xml/RMLTC0001b/mapping.ttl
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/xml/RMLTC0001b/output.nq
+-rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/xml/RMLTC0001b/student.xml
+-rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/xml/RMLTC0001b/test_RMLTC0001b_XML.py
+-rw-r--r--   0        0        0      710 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/xml/RMLTC0002a/mapping.ttl
+-rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/xml/RMLTC0002a/output.nq
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/xml/RMLTC0002a/student.xml
+-rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/xml/RMLTC0002a/test_RMLTC0002a_XML.py
+-rw-r--r--   0        0        0      596 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/xml/RMLTC0002b/mapping.ttl
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/xml/RMLTC0002b/output.nq
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/xml/RMLTC0002b/student.xml
+-rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/xml/RMLTC0002b/test_RMLTC0002b_XML.py
+-rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/xml/RMLTC0002c/mapping.ttl
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/xml/RMLTC0002c/output.nq
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/xml/RMLTC0002c/student.xml
+-rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/xml/RMLTC0002c/test_RMLTC0002c_XML.py
+-rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/xml/RMLTC0002e/mapping.ttl
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/xml/RMLTC0002e/student.xml
+-rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/xml/RMLTC0002e/test_RMLTC0002e_XML.py
+-rw-r--r--   0        0        0      643 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/xml/RMLTC0003c/mapping.ttl
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/xml/RMLTC0003c/output.nq
+-rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/xml/RMLTC0003c/student.xml
+-rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/xml/RMLTC0003c/test_RMLTC0003c_XML.py
+-rw-r--r--   0        0        0     1041 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/xml/RMLTC0004a/mapping.ttl
+-rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/xml/RMLTC0004a/output.nq
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/xml/RMLTC0004a/student_sport.xml
+-rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/xml/RMLTC0004a/test_RMLTC0004a_XML.py
+-rw-r--r--   0        0        0      620 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/xml/RMLTC0004b/mapping.ttl
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/xml/RMLTC0004b/output.nq
+-rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/xml/RMLTC0004b/student.xml
+-rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/xml/RMLTC0004b/test_RMLTC0004b_XML.py
+-rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/xml/RMLTC0005a/ious.xml
+-rw-r--r--   0        0        0      610 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/xml/RMLTC0005a/mapping.ttl
+-rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/xml/RMLTC0005a/output.nq
+-rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/xml/RMLTC0005a/test_RMLTC0005a_XML.py
+-rw-r--r--   0        0        0      666 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/xml/RMLTC0006a/mapping.ttl
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/xml/RMLTC0006a/output.nq
+-rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/xml/RMLTC0006a/student.xml
+-rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/xml/RMLTC0006a/test_RMLTC0006a_XML.py
+-rw-r--r--   0        0        0      640 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/xml/RMLTC0007a/mapping.ttl
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/xml/RMLTC0007a/output.nq
+-rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/xml/RMLTC0007a/student.xml
+-rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/xml/RMLTC0007a/test_RMLTC0007a_XML.py
+-rw-r--r--   0        0        0      780 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/xml/RMLTC0007b/mapping.ttl
+-rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/xml/RMLTC0007b/output.nq
+-rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/xml/RMLTC0007b/student.xml
+-rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/xml/RMLTC0007b/test_RMLTC0007b_XML.py
+-rw-r--r--   0        0        0      741 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/xml/RMLTC0007c/mapping.ttl
+-rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/xml/RMLTC0007c/output.nq
+-rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/xml/RMLTC0007c/student.xml
+-rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/xml/RMLTC0007c/test_RMLTC0007c_XML.py
+-rw-r--r--   0        0        0      935 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/xml/RMLTC0007d/mapping.ttl
+-rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/xml/RMLTC0007d/output.nq
+-rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/xml/RMLTC0007d/student.xml
+-rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/xml/RMLTC0007d/test_RMLTC0007d_XML.py
+-rw-r--r--   0        0        0      762 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/xml/RMLTC0007e/mapping.ttl
+-rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/xml/RMLTC0007e/output.nq
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/xml/RMLTC0007e/student.xml
+-rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/xml/RMLTC0007e/test_RMLTC0007e_XML.py
+-rw-r--r--   0        0        0      882 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/xml/RMLTC0007f/mapping.ttl
+-rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/xml/RMLTC0007f/output.nq
+-rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/xml/RMLTC0007f/student.xml
+-rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/xml/RMLTC0007f/test_RMLTC0007f_XML.py
+-rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/xml/RMLTC0007g/mapping.ttl
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/xml/RMLTC0007g/output.nq
+-rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/xml/RMLTC0007g/student.xml
+-rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/xml/RMLTC0007g/test_RMLTC0007g_XML.py
+-rw-r--r--   0        0        0      685 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/xml/RMLTC0007h/mapping.ttl
+-rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/xml/RMLTC0007h/student.xml
+-rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/xml/RMLTC0007h/test_RMLTC0007h_XML.py
+-rw-r--r--   0        0        0     1033 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/xml/RMLTC0008a/mapping.ttl
+-rw-r--r--   0        0        0      627 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/xml/RMLTC0008a/output.nq
+-rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/xml/RMLTC0008a/student.xml
+-rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/xml/RMLTC0008a/test_RMLTC0008a_XML.py
+-rw-r--r--   0        0        0     1425 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/xml/RMLTC0008b/mapping.ttl
+-rw-r--r--   0        0        0      544 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/xml/RMLTC0008b/output.nq
+-rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/xml/RMLTC0008b/student.xml
+-rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/xml/RMLTC0008b/test_RMLTC0008b_XML.py
+-rw-r--r--   0        0        0      667 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/xml/RMLTC0008c/mapping.ttl
+-rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/xml/RMLTC0008c/output.nq
+-rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/xml/RMLTC0008c/student.xml
+-rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/xml/RMLTC0008c/test_RMLTC0008c_XML.py
+-rw-r--r--   0        0        0     1352 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/xml/RMLTC0009a/mapping.ttl
+-rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/xml/RMLTC0009a/output.nq
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/xml/RMLTC0009a/sport.xml
+-rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/xml/RMLTC0009a/student.xml
+-rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/xml/RMLTC0009a/test_RMLTC0009a_XML.py
+-rw-r--r--   0        0        0     1678 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/xml/RMLTC0009b/mapping.ttl
+-rw-r--r--   0        0        0     1198 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/xml/RMLTC0009b/output.nq
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/xml/RMLTC0009b/sport.xml
+-rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/xml/RMLTC0009b/student.xml
+-rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/xml/RMLTC0009b/test_RMLTC0009b_XML.py
+-rw-r--r--   0        0        0      419 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/xml/RMLTC0010b/country_info.xml
+-rw-r--r--   0        0        0      644 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/xml/RMLTC0010b/mapping.ttl
+-rw-r--r--   0        0        0      312 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/xml/RMLTC0010b/output.nq
+-rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/xml/RMLTC0010b/test_RMLTC0010b_XML.py
+-rw-r--r--   0        0        0      419 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/xml/RMLTC0010c/country_info.xml
+-rw-r--r--   0        0        0      693 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/xml/RMLTC0010c/mapping.ttl
+-rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/xml/RMLTC0010c/output.nq
+-rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/xml/RMLTC0010c/test_RMLTC0010c_XML.py
+-rw-r--r--   0        0        0     1658 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/xml/RMLTC0011b/mapping.ttl
+-rw-r--r--   0        0        0     1229 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/xml/RMLTC0011b/output.nq
+-rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/xml/RMLTC0011b/sport.xml
+-rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/xml/RMLTC0011b/student.xml
+-rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/xml/RMLTC0011b/student_sport.xml
+-rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/xml/RMLTC0011b/test_RMLTC0011b_XML.py
+-rw-r--r--   0        0        0      775 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/xml/RMLTC0012a/mapping.ttl
+-rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/xml/RMLTC0012a/output.nq
+-rw-r--r--   0        0        0      329 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/xml/RMLTC0012a/persons.xml
+-rw-r--r--   0        0        0      652 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/xml/RMLTC0012a/test_RMLTC0012a_XML.py
+-rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/xml/RMLTC0012b/lives.xml
+-rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/xml/RMLTC0012b/mapping.ttl
+-rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/xml/RMLTC0012b/output.nq
+-rw-r--r--   0        0        0      329 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/xml/RMLTC0012b/persons.xml
+-rw-r--r--   0        0        0      652 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/xml/RMLTC0012b/test_RMLTC0012b_XML.py
+-rw-r--r--   0        0        0      685 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/xml/RMLTC0012c/mapping.ttl
+-rw-r--r--   0        0        0      332 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/xml/RMLTC0012c/persons.xml
+-rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/xml/RMLTC0012c/test_RMLTC0012c_XML.py
+-rw-r--r--   0        0        0      869 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/xml/RMLTC0012d/mapping.ttl
+-rw-r--r--   0        0        0      332 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/xml/RMLTC0012d/persons.xml
+-rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/xml/RMLTC0012d/test_RMLTC0012d_XML.py
+-rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/xml/RMLTC0015a/country_en.xml
+-rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/xml/RMLTC0015a/country_es.xml
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/xml/RMLTC0015a/mapping.ttl
+-rw-r--r--   0        0        0      386 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/xml/RMLTC0015a/output.nq
+-rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/xml/RMLTC0015a/test_RMLTC0015a_XML.py
+-rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/xml/RMLTC0015b/country_en.xml
+-rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/xml/RMLTC0015b/country_es.xml
+-rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/xml/RMLTC0015b/mapping.ttl
+-rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/xml/RMLTC0015b/test_RMLTC0015b_XML.py
+-rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/xml/RMLTC0019a/RMLTC0019a_XML.py
+-rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/xml/RMLTC0019a/mapping.ttl
+-rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/xml/RMLTC0019a/output.nq
+-rw-r--r--   0        0        0      306 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/xml/RMLTC0019a/persons.xml
+-rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/xml/RMLTC0019b/RMLTC0019b_XML.py
+-rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/xml/RMLTC0019b/mapping.ttl
+-rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/xml/RMLTC0019b/output.nq
+-rw-r--r--   0        0        0      432 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/xml/RMLTC0019b/persons.xml
+-rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/xml/RMLTC0020a/RMLTC0020a_XML.py
+-rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/xml/RMLTC0020a/mapping.ttl
+-rw-r--r--   0        0        0      658 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/xml/RMLTC0020a/output.nq
+-rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/xml/RMLTC0020a/student.xml
+-rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/xml/RMLTC0020b/RMLTC0020b_XML.py
+-rw-r--r--   0        0        0      686 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/xml/RMLTC0020b/mapping.ttl
+-rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/xml/RMLTC0020b/output.nq
+-rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/xml/RMLTC0020b/student.xml
+-rw-r--r--   0        0        0      859 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/xml/attributes/data.xml
+-rw-r--r--   0        0        0     1490 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/xml/attributes/mapping.ttl
+-rw-r--r--   0        0        0     1532 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/xml/attributes/output.nq
+-rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/xml/attributes/test_attributes_XML.py
+-rw-r--r--   0        0        0     3656 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/xml/complex/data.xml
+-rw-r--r--   0        0        0     9740 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/xml/complex/mapping.ttl
+-rw-r--r--   0        0        0     1756 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/xml/complex/mapping.yaml
+-rw-r--r--   0        0        0     4539 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/xml/complex/output.nq
+-rw-r--r--   0        0        0     2020 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/xml/complex/test_complex_XML.py
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/xml/rml_spec_example_section_3/Transport.xml
+-rw-r--r--   0        0        0      952 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/xml/rml_spec_example_section_3/mapping.ttl
+-rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/xml/rml_spec_example_section_3/output.nq
+-rw-r--r--   0        0        0      704 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/xml/rml_spec_example_section_3/test_rml_spec_example_section_3_XML.py
+-rw-r--r--   0        0        0      435 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/xml/rml_spec_example_section_5/Transport.xml
+-rw-r--r--   0        0        0      752 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/xml/rml_spec_example_section_5/mapping.ttl
+-rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/xml/rml_spec_example_section_5/output.nq
+-rw-r--r--   0        0        0      704 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-core/xml/rml_spec_example_section_5/test_rml_spec_example_section_5_XML.py
+-rw-r--r--   0        0        0      900 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-fnml/RMLFNOTC0000-CSV/mapping.ttl
+-rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-fnml/RMLFNOTC0000-CSV/output.nq
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-fnml/RMLFNOTC0000-CSV/student.csv
+-rw-r--r--   0        0        0      841 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-fnml/RMLFNOTC0000-CSV/test_RMLFNOTC0000-CSV.py
+-rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-fnml/RMLFNOTC0001-CSV/mapping.ttl
+-rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-fnml/RMLFNOTC0001-CSV/output.nq
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-fnml/RMLFNOTC0001-CSV/student.csv
+-rw-r--r--   0        0        0      694 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-fnml/RMLFNOTC0001-CSV/test_RMLFNOTC0001-CSV.py
+-rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-fnml/RMLFNOTC0002-CSV/mapping.ttl
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-fnml/RMLFNOTC0002-CSV/output.nq
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-fnml/RMLFNOTC0002-CSV/student.csv
+-rw-r--r--   0        0        0      694 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-fnml/RMLFNOTC0002-CSV/test_RMLFNOTC0002-CSV.py
+-rw-r--r--   0        0        0     1162 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-fnml/RMLFNOTC0003-CSV/mapping.ttl
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-fnml/RMLFNOTC0003-CSV/output.nq
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-fnml/RMLFNOTC0003-CSV/student.csv
+-rw-r--r--   0        0        0      717 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-fnml/RMLFNOTC0003-CSV/test_RMLFNOTC0003-CSV.py
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-fnml/RMLFNOTC0004-CSV/mapping.ttl
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-fnml/RMLFNOTC0004-CSV/output.nq
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-fnml/RMLFNOTC0004-CSV/student.csv
+-rw-r--r--   0        0        0      694 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-fnml/RMLFNOTC0004-CSV/test_RMLFNOTC0004-CSV.py
+-rw-r--r--   0        0        0     1028 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-fnml/RMLFNOTC0005-CSV/mapping.ttl
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-fnml/RMLFNOTC0005-CSV/output.nq
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-fnml/RMLFNOTC0005-CSV/student.csv
+-rw-r--r--   0        0        0      717 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-fnml/RMLFNOTC0005-CSV/test_RMLFNOTC0005-CSV.py
+-rw-r--r--   0        0        0     1104 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-fnml/RMLFNOTC0006-CSV/mapping.ttl
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-fnml/RMLFNOTC0006-CSV/output.nq
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-fnml/RMLFNOTC0006-CSV/student.csv
+-rw-r--r--   0        0        0      717 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-fnml/RMLFNOTC0006-CSV/test_RMLFNOTC0006-CSV.py
+-rw-r--r--   0        0        0     1053 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-fnml/RMLFNOTC0008-CSV/mapping.ttl
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-fnml/RMLFNOTC0008-CSV/output.nq
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-fnml/RMLFNOTC0008-CSV/student.csv
+-rw-r--r--   0        0        0      694 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-fnml/RMLFNOTC0008-CSV/test_RMLFNOTC0008-CSV.py
+-rw-r--r--   0        0        0     1702 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-fnml/RMLFNOTC0009-CSV/mapping.ttl
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-fnml/RMLFNOTC0009-CSV/output.nq
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-fnml/RMLFNOTC0009-CSV/student.csv
+-rw-r--r--   0        0        0      794 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-fnml/RMLFNOTC0009-CSV/test_RMLFNOTC0009-CSV.py
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-fnml/array_get_slice/article.tsv
+-rw-r--r--   0        0        0     1652 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-fnml/array_get_slice/mapping.ttl
+-rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-fnml/array_get_slice/output.nq
+-rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-fnml/array_get_slice/test_array_get_slice.py
+-rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-fnml/controls_if/calendar.csv
+-rw-r--r--   0        0        0     1917 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-fnml/controls_if/mapping.ttl
+-rw-r--r--   0        0        0      518 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-fnml/controls_if/output.nq
+-rw-r--r--   0        0        0      649 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-fnml/controls_if/test_controls_if.py
+-rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-fnml/controls_if_cast/calendar.csv
+-rw-r--r--   0        0        0     1921 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-fnml/controls_if_cast/mapping.ttl
+-rw-r--r--   0        0        0      518 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-fnml/controls_if_cast/output.nq
+-rw-r--r--   0        0        0      654 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-fnml/controls_if_cast/test_controls_if_cast.py
+-rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-fnml/date_to_date/calendar.csv
+-rw-r--r--   0        0        0     1315 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-fnml/date_to_date/mapping.ttl
+-rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-fnml/date_to_date/output.nq
+-rw-r--r--   0        0        0      650 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-fnml/date_to_date/test_date_to_date.py
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-fnml/math_round/distances.tsv
+-rw-r--r--   0        0        0     1116 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-fnml/math_round/mapping.ttl
+-rw-r--r--   0        0        0      342 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-fnml/math_round/output.nq
+-rw-r--r--   0        0        0      648 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-fnml/math_round/test_math_round.py
+-rw-r--r--   0        0        0     1184 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-fnml/split_explode/mapping.ttl
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-fnml/split_explode/mixed_content_list.csv
+-rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-fnml/split_explode/output.nq
+-rw-r--r--   0        0        0      651 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-fnml/split_explode/test_split_explode.py
+-rw-r--r--   0        0        0     1189 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-fnml/split_explode_null/mapping.ttl
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-fnml/split_explode_null/mixed_content_list.csv
+-rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-fnml/split_explode_null/output.nq
+-rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-fnml/split_explode_null/test_split_explode_null.py
+-rw-r--r--   0        0        0     1052 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-fnml/udf/mapping.ttl
+-rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-fnml/udf/output.nq
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-fnml/udf/student.csv
+-rw-r--r--   0        0        0      781 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-fnml/udf/test_udf.py
+-rw-r--r--   0        0        0      376 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-fnml/udf/udf.py
+-rw-r--r--   0        0        0      878 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-in-memory/json_dictionary/RMLIMTC0000/mapping.ttl
+-rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-in-memory/json_dictionary/RMLIMTC0000/output.nq
+-rw-r--r--   0        0        0      900 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-in-memory/json_dictionary/RMLIMTC0000/test_RMLTC0000_DICT.py
+-rw-r--r--   0        0        0      906 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-in-memory/json_dictionary/RMLIMTC0001a/mapping.ttl
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-in-memory/json_dictionary/RMLIMTC0001a/output.nq
+-rw-r--r--   0        0        0      803 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-in-memory/json_dictionary/RMLIMTC0001a/test_RMLTC0001a_DICT.py
+-rw-r--r--   0        0        0      889 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-in-memory/json_dictionary/RMLIMTC0001b/mapping.ttl
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-in-memory/json_dictionary/RMLIMTC0001b/output.nq
+-rw-r--r--   0        0        0      803 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-in-memory/json_dictionary/RMLIMTC0001b/test_RMLTC0001b_DICT.py
+-rw-r--r--   0        0        0      997 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-in-memory/json_dictionary/RMLIMTC0002a/mapping.ttl
+-rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-in-memory/json_dictionary/RMLIMTC0002a/output.nq
+-rw-r--r--   0        0        0      821 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-in-memory/json_dictionary/RMLIMTC0002a/test_RMLTC0002a_DICT.py
+-rw-r--r--   0        0        0      883 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-in-memory/json_dictionary/RMLIMTC0002b/mapping.ttl
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-in-memory/json_dictionary/RMLIMTC0002b/output.nq
+-rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-in-memory/json_dictionary/RMLIMTC0002b/test_RMLTC0002b_DICT.py
+-rw-r--r--   0        0        0      866 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-in-memory/json_dictionary/RMLIMTC0002c/mapping.ttl
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-in-memory/json_dictionary/RMLIMTC0002c/output.nq
+-rw-r--r--   0        0        0      751 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-in-memory/json_dictionary/RMLIMTC0002c/test_RMLTC0002c_DICT.py
+-rw-r--r--   0        0        0      865 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-in-memory/json_dictionary/RMLIMTC0002e/mapping.ttl
+-rw-r--r--   0        0        0      751 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-in-memory/json_dictionary/RMLIMTC0002e/test_RMLTC0002e_DICT.py
+-rw-r--r--   0        0        0      932 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-in-memory/json_dictionary/RMLIMTC0003c/mapping.ttl
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-in-memory/json_dictionary/RMLIMTC0003c/output.nq
+-rw-r--r--   0        0        0      857 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-in-memory/json_dictionary/RMLIMTC0003c/test_RMLTC0003c_DICT.py
+-rw-r--r--   0        0        0     1440 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-in-memory/json_dictionary/RMLIMTC0004a/mapping.ttl
+-rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-in-memory/json_dictionary/RMLIMTC0004a/output.nq
+-rw-r--r--   0        0        0      833 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-in-memory/json_dictionary/RMLIMTC0004a/test_RMLTC0004a_DICT.py
+-rw-r--r--   0        0        0      906 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-in-memory/json_dictionary/RMLIMTC0004b/mapping.ttl
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-in-memory/json_dictionary/RMLIMTC0004b/output.nq
+-rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-in-memory/json_dictionary/RMLIMTC0004b/test_RMLTC0004b_DICT.py
+-rw-r--r--   0        0        0      901 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-in-memory/json_dictionary/RMLIMTC0005a/mapping.ttl
+-rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-in-memory/json_dictionary/RMLIMTC0005a/output.nq
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-in-memory/json_dictionary/RMLIMTC0005a/test_RMLTC0005a_DICT.py
+-rw-r--r--   0        0        0      952 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-in-memory/json_dictionary/RMLIMTC0006a/mapping.ttl
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-in-memory/json_dictionary/RMLIMTC0006a/output.nq
+-rw-r--r--   0        0        0      857 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-in-memory/json_dictionary/RMLIMTC0006a/test_RMLTC0006a_DICT.py
+-rw-r--r--   0        0        0      927 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-in-memory/json_dictionary/RMLIMTC0007a/mapping.ttl
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-in-memory/json_dictionary/RMLIMTC0007a/output.nq
+-rw-r--r--   0        0        0      857 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-in-memory/json_dictionary/RMLIMTC0007a/test_RMLTC0007a_DICT.py
+-rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-in-memory/json_dictionary/RMLIMTC0007b/mapping.ttl
+-rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-in-memory/json_dictionary/RMLIMTC0007b/output.nq
+-rw-r--r--   0        0        0      857 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-in-memory/json_dictionary/RMLIMTC0007b/test_RMLTC0007b_DICT.py
+-rw-r--r--   0        0        0     1028 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-in-memory/json_dictionary/RMLIMTC0007c/mapping.ttl
+-rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-in-memory/json_dictionary/RMLIMTC0007c/output.nq
+-rw-r--r--   0        0        0      857 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-in-memory/json_dictionary/RMLIMTC0007c/test_RMLTC0007c_DICT.py
+-rw-r--r--   0        0        0     1222 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-in-memory/json_dictionary/RMLIMTC0007d/mapping.ttl
+-rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-in-memory/json_dictionary/RMLIMTC0007d/output.nq
+-rw-r--r--   0        0        0      857 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-in-memory/json_dictionary/RMLIMTC0007d/test_RMLTC0007d_DICT.py
+-rw-r--r--   0        0        0     1036 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-in-memory/json_dictionary/RMLIMTC0007e/mapping.ttl
+-rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-in-memory/json_dictionary/RMLIMTC0007e/output.nq
+-rw-r--r--   0        0        0      821 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-in-memory/json_dictionary/RMLIMTC0007e/test_RMLTC0007e_DICT.py
+-rw-r--r--   0        0        0     1169 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-in-memory/json_dictionary/RMLIMTC0007f/mapping.ttl
+-rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-in-memory/json_dictionary/RMLIMTC0007f/output.nq
+-rw-r--r--   0        0        0      858 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-in-memory/json_dictionary/RMLIMTC0007f/test_RMLTC0007f_DICT.py
+-rw-r--r--   0        0        0      929 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-in-memory/json_dictionary/RMLIMTC0007g/mapping.ttl
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-in-memory/json_dictionary/RMLIMTC0007g/output.nq
+-rw-r--r--   0        0        0      858 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-in-memory/json_dictionary/RMLIMTC0007g/test_RMLTC0007g_DICT.py
+-rw-r--r--   0        0        0      971 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-in-memory/json_dictionary/RMLIMTC0007h/mapping.ttl
+-rw-r--r--   0        0        0      760 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-in-memory/json_dictionary/RMLIMTC0007h/test_RMLTC0007h_DICT.py
+-rw-r--r--   0        0        0     1320 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-in-memory/json_dictionary/RMLIMTC0008a/mapping.ttl
+-rw-r--r--   0        0        0      627 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-in-memory/json_dictionary/RMLIMTC0008a/output.nq
+-rw-r--r--   0        0        0      858 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-in-memory/json_dictionary/RMLIMTC0008a/test_RMLTC0008a_DICT.py
+-rw-r--r--   0        0        0     1835 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-in-memory/json_dictionary/RMLIMTC0008b/mapping.ttl
+-rw-r--r--   0        0        0      544 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-in-memory/json_dictionary/RMLIMTC0008b/output.nq
+-rw-r--r--   0        0        0      858 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-in-memory/json_dictionary/RMLIMTC0008b/test_RMLTC0008b_DICT.py
+-rw-r--r--   0        0        0      954 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-in-memory/json_dictionary/RMLIMTC0008c/mapping.ttl
+-rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-in-memory/json_dictionary/RMLIMTC0008c/output.nq
+-rw-r--r--   0        0        0      857 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-in-memory/json_dictionary/RMLIMTC0008c/test_RMLTC0008c_DICT.py
+-rw-r--r--   0        0        0     1766 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-in-memory/json_dictionary/RMLIMTC0009a/mapping.ttl
+-rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-in-memory/json_dictionary/RMLIMTC0009a/output.nq
+-rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-in-memory/json_dictionary/RMLIMTC0009a/test_RMLTC0009a_DICT.py
+-rw-r--r--   0        0        0     2082 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-in-memory/json_dictionary/RMLIMTC0009b/mapping.ttl
+-rw-r--r--   0        0        0     1198 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-in-memory/json_dictionary/RMLIMTC0009b/output.nq
+-rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-in-memory/json_dictionary/RMLIMTC0009b/test_RMLTC0009b_DICT.py
+-rw-r--r--   0        0        0      919 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-in-memory/json_dictionary/RMLIMTC0010a/mapping.ttl
+-rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-in-memory/json_dictionary/RMLIMTC0010a/output.nq
+-rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-in-memory/json_dictionary/RMLIMTC0010a/test_RMLTC0010a_DICT.py
+-rw-r--r--   0        0        0      926 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-in-memory/json_dictionary/RMLIMTC0010b/mapping.ttl
+-rw-r--r--   0        0        0      312 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-in-memory/json_dictionary/RMLIMTC0010b/output.nq
+-rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-in-memory/json_dictionary/RMLIMTC0010b/test_RMLTC0010b_DICT.py
+-rw-r--r--   0        0        0      976 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-in-memory/json_dictionary/RMLIMTC0010c/mapping.ttl
+-rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-in-memory/json_dictionary/RMLIMTC0010c/output.nq
+-rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-in-memory/json_dictionary/RMLIMTC0010c/test_RMLTC0010c_DICT.py
+-rw-r--r--   0        0        0     2190 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-in-memory/json_dictionary/RMLIMTC0011b/mapping.ttl
+-rw-r--r--   0        0        0     1229 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-in-memory/json_dictionary/RMLIMTC0011b/output.nq
+-rw-r--r--   0        0        0     1391 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-in-memory/json_dictionary/RMLIMTC0011b/test_RMLTC0011b_DICT.py
+-rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-in-memory/json_dictionary/RMLIMTC0012a/mapping.ttl
+-rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-in-memory/json_dictionary/RMLIMTC0012a/output.nq
+-rw-r--r--   0        0        0      899 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-in-memory/json_dictionary/RMLIMTC0012a/test_RMLTC0012a_DICT.py
+-rw-r--r--   0        0        0     1475 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-in-memory/json_dictionary/RMLIMTC0012b/mapping.ttl
+-rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-in-memory/json_dictionary/RMLIMTC0012b/output.nq
+-rw-r--r--   0        0        0     1129 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-in-memory/json_dictionary/RMLIMTC0012b/test_RMLTC0012b_DICT.py
+-rw-r--r--   0        0        0      972 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-in-memory/json_dictionary/RMLIMTC0012c/mapping.ttl
+-rw-r--r--   0        0        0      865 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-in-memory/json_dictionary/RMLIMTC0012c/test_RMLTC0012c_DICT.py
+-rw-r--r--   0        0        0     1155 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-in-memory/json_dictionary/RMLIMTC0012d/mapping.ttl
+-rw-r--r--   0        0        0      865 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-in-memory/json_dictionary/RMLIMTC0012d/test_RMLTC0012d_DICT.py
+-rw-r--r--   0        0        0      905 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-in-memory/json_dictionary/RMLIMTC0013a/mapping.ttl
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-in-memory/json_dictionary/RMLIMTC0013a/output.nq
+-rw-r--r--   0        0        0      899 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-in-memory/json_dictionary/RMLIMTC0013a/test_RMLTC0013a_DICT.py
+-rw-r--r--   0        0        0     1494 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-in-memory/json_dictionary/RMLIMTC0015a/mapping.ttl
+-rw-r--r--   0        0        0      386 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-in-memory/json_dictionary/RMLIMTC0015a/output.nq
+-rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-in-memory/json_dictionary/RMLIMTC0015a/test_RMLTC0015a_DICT.py
+-rw-r--r--   0        0        0     1491 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-in-memory/json_dictionary/RMLIMTC0015b/mapping.ttl
+-rw-r--r--   0        0        0      991 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-in-memory/json_dictionary/RMLIMTC0015b/test_RMLTC0015b_DICT.py
+-rw-r--r--   0        0        0      892 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0000/mapping.ttl
+-rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0000/output.nq
+-rw-r--r--   0        0        0      790 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0000/test_RMLIMTC0000_DF.py
+-rw-r--r--   0        0        0      891 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0001a/mapping.ttl
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0001a/output.nq
+-rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0001a/student.csv
+-rw-r--r--   0        0        0      795 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0001a/test_RMLTC0001a_DF.py
+-rw-r--r--   0        0        0      904 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0001b/mapping.ttl
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0001b/output.nq
+-rw-r--r--   0        0        0      795 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0001b/test_RMLIMTC0001b_DF.py
+-rw-r--r--   0        0        0     1012 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0002a/mapping.ttl
+-rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0002a/output.nq
+-rw-r--r--   0        0        0      806 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0002a/test_RMLIMTC0002a_DF.py
+-rw-r--r--   0        0        0      898 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0002b/mapping.ttl
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0002b/output.nq
+-rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0002b/test_RMLIMTC0002b_DF.py
+-rw-r--r--   0        0        0      881 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0002c/mapping.ttl
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0002c/output.nq
+-rw-r--r--   0        0        0      736 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0002c/test_RMLIMTC0002c_DF.py
+-rw-r--r--   0        0        0      880 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0002e/mapping.ttl
+-rw-r--r--   0        0        0      736 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0002e/test_RMLIMTC0002e_DF.py
+-rw-r--r--   0        0        0      945 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0003c/mapping.ttl
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0003c/output.nq
+-rw-r--r--   0        0        0      836 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0003c/test_RMLIMTC0003c_DF.py
+-rw-r--r--   0        0        0     1469 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0004a/mapping.ttl
+-rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0004a/output.nq
+-rw-r--r--   0        0        0      818 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0004a/test_RMLIMTC0004a_DF.py
+-rw-r--r--   0        0        0      915 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0004b/mapping.ttl
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0004b/output.nq
+-rw-r--r--   0        0        0      725 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0004b/test_RMLIMTC0004b_DF.py
+-rw-r--r--   0        0        0      910 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0005a/mapping.ttl
+-rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0005a/output.nq
+-rw-r--r--   0        0        0      907 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0005a/test_RMLIMTC0005a_DF.py
+-rw-r--r--   0        0        0      968 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0006a/mapping.ttl
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0006a/output.nq
+-rw-r--r--   0        0        0      836 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0006a/test_RMLIMTC0006a_DF.py
+-rw-r--r--   0        0        0      942 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0007a/mapping.ttl
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0007a/output.nq
+-rw-r--r--   0        0        0      836 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0007a/test_RMLIMTC0007a_DF.py
+-rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0007b/mapping.ttl
+-rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0007b/output.nq
+-rw-r--r--   0        0        0      836 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0007b/test_RMLIMTC0007b_DF.py
+-rw-r--r--   0        0        0     1043 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0007c/mapping.ttl
+-rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0007c/output.nq
+-rw-r--r--   0        0        0      836 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0007c/test_RMLIMTC0007c_DF.py
+-rw-r--r--   0        0        0     1239 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0007d/mapping.ttl
+-rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0007d/output.nq
+-rw-r--r--   0        0        0      835 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0007d/test_RMLTC0007d_DF.py
+-rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0007e/mapping.ttl
+-rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0007e/output.nq
+-rw-r--r--   0        0        0      806 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0007e/test_RMLIMTC0007e_DF.py
+-rw-r--r--   0        0        0     1184 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0007f/mapping.ttl
+-rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0007f/output.nq
+-rw-r--r--   0        0        0      836 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0007f/test_RMLIMTC0007f_DF.py
+-rw-r--r--   0        0        0      944 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0007g/mapping.ttl
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0007g/output.nq
+-rw-r--r--   0        0        0      836 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0007g/test_RMLIMTC0007g_DF.py
+-rw-r--r--   0        0        0      987 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0007h/mapping.ttl
+-rw-r--r--   0        0        0      739 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0007h/test_RMLIMTC0007h_DF.py
+-rw-r--r--   0        0        0     1335 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0008a/mapping.ttl
+-rw-r--r--   0        0        0      627 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0008a/output.nq
+-rw-r--r--   0        0        0      835 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0008a/test_RMLIMTC0008a_DF.py
+-rw-r--r--   0        0        0     1859 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0008b/mapping.ttl
+-rw-r--r--   0        0        0      544 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0008b/output.nq
+-rw-r--r--   0        0        0      835 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0008b/test_RMLIMTC0008b_DF.py
+-rw-r--r--   0        0        0      969 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0008c/mapping.ttl
+-rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0008c/output.nq
+-rw-r--r--   0        0        0      835 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0008c/test_RMLIMTC0008c_DF.py
+-rw-r--r--   0        0        0     1798 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0009a/mapping.ttl
+-rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0009a/output.nq
+-rw-r--r--   0        0        0      925 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0009a/test_RMLIMTC0009a_DF.py
+-rw-r--r--   0        0        0     2119 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0009b/mapping.ttl
+-rw-r--r--   0        0        0     1198 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0009b/output.nq
+-rw-r--r--   0        0        0      925 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0009b/test_RMLIMTC0009b_DF.py
+-rw-r--r--   0        0        0      934 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0010a/mapping.ttl
+-rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0010a/output.nq
+-rw-r--r--   0        0        0      938 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0010a/test_RMLIMTC0010a_DF.py
+-rw-r--r--   0        0        0      941 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0010b/mapping.ttl
+-rw-r--r--   0        0        0      312 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0010b/output.nq
+-rw-r--r--   0        0        0      930 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0010b/test_RMLIMTC0010b_DF.py
+-rw-r--r--   0        0        0      991 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0010c/mapping.ttl
+-rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0010c/output.nq
+-rw-r--r--   0        0        0      930 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0010c/test_RMLIMTC0010c_DF.py
+-rw-r--r--   0        0        0     2244 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0011b/mapping.ttl
+-rw-r--r--   0        0        0     1229 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0011b/output.nq
+-rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0011b/test_RMLIMTC0011b_DF.py
+-rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0012a/mapping.ttl
+-rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0012a/output.nq
+-rw-r--r--   0        0        0      831 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0012a/test_RMLIMTC0012a_DF.py
+-rw-r--r--   0        0        0     1511 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0012b/mapping.ttl
+-rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0012b/output.nq
+-rw-r--r--   0        0        0      987 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0012b/test_RMLIMTC0012b_DF.py
+-rw-r--r--   0        0        0      988 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0012c/mapping.ttl
+-rw-r--r--   0        0        0      796 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0012c/test_RMLIMTC0012c_DF.py
+-rw-r--r--   0        0        0     1172 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0012d/mapping.ttl
+-rw-r--r--   0        0        0      797 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0012d/test_RMLIMTC0012d_DF.py
+-rw-r--r--   0        0        0     1524 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0015a/mapping.ttl
+-rw-r--r--   0        0        0      386 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0015a/output.nq
+-rw-r--r--   0        0        0      992 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0015a/test_RMLIMTC0015a_DF.py
+-rw-r--r--   0        0        0     1521 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0015b/mapping.ttl
+-rw-r--r--   0        0        0      922 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0015b/test_RMLIMTC0015b_DF.py
+-rw-r--r--   0        0        0      939 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0016a/mapping.ttl
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0016a/test.csv
+-rw-r--r--   0        0        0      768 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0016a/test_RMLIMTC0016a_DF.py
+-rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-in-memory/pandas_dataframe/triples_map_without_pom/mapping.ttl
+-rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-in-memory/pandas_dataframe/triples_map_without_pom/output.nq
+-rw-r--r--   0        0        0      937 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-in-memory/pandas_dataframe/triples_map_without_pom/test_triples_map_without_pom_DF.py
+-rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-star/RMLSTARTC001a/data.csv
+-rw-r--r--   0        0        0      968 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-star/RMLSTARTC001a/mapping.ttl
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-star/RMLSTARTC001a/output.nq
+-rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-star/RMLSTARTC001a/test_RMLSTARTC001a_CSV.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-star/RMLSTARTC001b/data1.csv
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-star/RMLSTARTC001b/data2.csv
+-rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-star/RMLSTARTC001b/mapping.ttl
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-star/RMLSTARTC001b/output.nq
+-rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-star/RMLSTARTC001b/test_RMLSTARTC001b_CSV.py
+-rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-star/RMLSTARTC002a/data.csv
+-rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-star/RMLSTARTC002a/mapping.ttl
+-rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-star/RMLSTARTC002a/output.nq
+-rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-star/RMLSTARTC002a/test_RMLSTARTC002a_CSV.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-star/RMLSTARTC002b/data1.csv
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-star/RMLSTARTC002b/data2.csv
+-rw-r--r--   0        0        0     1169 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-star/RMLSTARTC002b/mapping.ttl
+-rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-star/RMLSTARTC002b/output.nq
+-rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-star/RMLSTARTC002b/test_RMLSTARTC002b_CSV.py
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-star/RMLSTARTC003a/data.csv
+-rw-r--r--   0        0        0     1419 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-star/RMLSTARTC003a/mapping.ttl
+-rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-star/RMLSTARTC003a/output.nq
+-rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-star/RMLSTARTC003a/test_RMLSTARTC003a_CSV.py
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-star/RMLSTARTC003b/data1.csv
+-rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-star/RMLSTARTC003b/data2.csv
+-rw-r--r--   0        0        0     1529 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-star/RMLSTARTC003b/mapping.ttl
+-rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-star/RMLSTARTC003b/output.nq
+-rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-star/RMLSTARTC003b/test_RMLSTARTC003b_CSV.py
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-star/RMLSTARTC004a/data.csv
+-rw-r--r--   0        0        0     1396 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-star/RMLSTARTC004a/mapping.ttl
+-rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-star/RMLSTARTC004a/output.nq
+-rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-star/RMLSTARTC004a/test_RMLSTARTC004a_CSV.py
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-star/RMLSTARTC004b/data1.csv
+-rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-star/RMLSTARTC004b/data2.csv
+-rw-r--r--   0        0        0     1506 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-star/RMLSTARTC004b/mapping.ttl
+-rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-star/RMLSTARTC004b/output.nq
+-rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-star/RMLSTARTC004b/test_RMLSTARTC004b_CSV.py
+-rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-star/RMLSTARTC005a/data.csv
+-rw-r--r--   0        0        0     1021 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-star/RMLSTARTC005a/mapping.ttl
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-star/RMLSTARTC005a/output.nq
+-rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-star/RMLSTARTC005a/test_RMLSTARTC005a_CSV.py
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-star/RMLSTARTC005b/data1.csv
+-rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-star/RMLSTARTC005b/data2.csv
+-rw-r--r--   0        0        0     1145 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-star/RMLSTARTC005b/mapping.ttl
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-star/RMLSTARTC005b/output.nq
+-rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-star/RMLSTARTC005b/test_RMLSTARTC005b_CSV.py
+-rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-star/RMLSTARTC006a/data.csv
+-rw-r--r--   0        0        0     1121 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-star/RMLSTARTC006a/mapping.ttl
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-star/RMLSTARTC006a/output.nq
+-rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-star/RMLSTARTC006a/test_RMLSTARTC006a_CSV.py
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-star/RMLSTARTC006b/data1.csv
+-rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-star/RMLSTARTC006b/data2.csv
+-rw-r--r--   0        0        0     1244 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-star/RMLSTARTC006b/mapping.ttl
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-star/RMLSTARTC006b/output.nq
+-rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-star/RMLSTARTC006b/test_RMLSTARTC006b_CSV.py
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-star/RMLSTARTC007a/data.csv
+-rw-r--r--   0        0        0     1408 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-star/RMLSTARTC007a/mapping.ttl
+-rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-star/RMLSTARTC007a/output.nq
+-rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-star/RMLSTARTC007a/test_RMLSTARTC007a_CSV.py
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-star/RMLSTARTC007b/data1.csv
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-star/RMLSTARTC007b/data2.csv
+-rw-r--r--   0        0        0     1535 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-star/RMLSTARTC007b/mapping.ttl
+-rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-star/RMLSTARTC007b/output.nq
+-rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-star/RMLSTARTC007b/test_RMLSTARTC007b_CSV.py
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-star/RMLSTARTC008a/data.csv
+-rw-r--r--   0        0        0     3028 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-star/RMLSTARTC008a/mapping.ttl
+-rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-star/RMLSTARTC008a/output.nq
+-rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-star/RMLSTARTC008a/test_RMLSTARTC008a_CSV.py
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-star/RMLSTARTC008b/data1.csv
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-star/RMLSTARTC008b/data2.csv
+-rw-r--r--   0        0        0     3167 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-star/RMLSTARTC008b/mapping.ttl
+-rw-r--r--   0        0        0      311 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-star/RMLSTARTC008b/output.nq
+-rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-star/RMLSTARTC008b/test_RMLSTARTC008b_CSV.py
+-rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-tv/RMLTVTC0002d/mapping.ttl
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-tv/RMLTVTC0002d/output.nq
+-rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-tv/RMLTVTC0002d/student.csv
+-rw-r--r--   0        0        0      654 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-tv/RMLTVTC0002d/test_RMLTVTC0002d_CSV.py
+-rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-tv/RMLTVTC0002g/mapping.ttl
+-rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-tv/RMLTVTC0002g/student.csv
+-rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-tv/RMLTVTC0002g/test_RMLTVTC0002g_CSV.py
+-rw-r--r--   0        0        0      474 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-tv/RMLTVTC0002h/mapping.ttl
+-rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-tv/RMLTVTC0002h/student.csv
+-rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-tv/RMLTVTC0002h/test_RMLTVTC0002h_CSV.py
+-rw-r--r--   0        0        0      415 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-tv/RMLTVTC0002i/mapping.ttl
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-tv/RMLTVTC0002i/output.nq
+-rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-tv/RMLTVTC0002i/student.csv
+-rw-r--r--   0        0        0      654 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-tv/RMLTVTC0002i/test_RMLTVTC0002i_CSV.py
+-rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-tv/RMLTVTC0002j/mapping.ttl
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-tv/RMLTVTC0002j/output.nq
+-rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-tv/RMLTVTC0002j/student.csv
+-rw-r--r--   0        0        0      654 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-tv/RMLTVTC0002j/test_RMLTVTC0002j_CSV.py
+-rw-r--r--   0        0        0      601 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-tv/RMLTVTC0003b/mapping.ttl
+-rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-tv/RMLTVTC0003b/output.nq
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-tv/RMLTVTC0003b/student.csv
+-rw-r--r--   0        0        0      654 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-tv/RMLTVTC0003b/test_RMLTVTC0003b_CSV.py
+-rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-tv/RMLTVTC0009c/mapping.ttl
+-rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-tv/RMLTVTC0009c/output.nq
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-tv/RMLTVTC0009c/sport.csv
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-tv/RMLTVTC0009c/student.csv
+-rw-r--r--   0        0        0      654 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-tv/RMLTVTC0009c/test_RMLTVTC0009c_CSV.py
+-rw-r--r--   0        0        0      663 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-tv/RMLTVTC0009d/mapping.ttl
+-rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-tv/RMLTVTC0009d/output.nq
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-tv/RMLTVTC0009d/sport.csv
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-tv/RMLTVTC0009d/student.csv
+-rw-r--r--   0        0        0      654 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-tv/RMLTVTC0009d/test_RMLTVTC0009d_CSV.py
+-rw-r--r--   0        0        0     1728 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-tv/RMLTVTC0011a/mapping.ttl
+-rw-r--r--   0        0        0     1525 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-tv/RMLTVTC0011a/output.nq
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-tv/RMLTVTC0011a/sport.csv
+-rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-tv/RMLTVTC0011a/student.csv
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-tv/RMLTVTC0011a/student_sport.csv
+-rw-r--r--   0        0        0      650 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-tv/RMLTVTC0011a/test_RMLTVTC0011a_CSV.py
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-tv/RMLTVTC0014d/dept.csv
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-tv/RMLTVTC0014d/emp.csv
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-tv/RMLTVTC0014d/likes.csv
+-rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-tv/RMLTVTC0014d/mapping.ttl
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-tv/RMLTVTC0014d/output.nq
+-rw-r--r--   0        0        0      650 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-tv/RMLTVTC0014d/test_RMLTVTC0014d_CSV.py
+-rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-tv/RMLTVTC0015a/country.csv
+-rw-r--r--   0        0        0      982 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-tv/RMLTVTC0015a/mapping.ttl
+-rw-r--r--   0        0        0      386 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-tv/RMLTVTC0015a/output.nq
+-rw-r--r--   0        0        0      650 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-tv/RMLTVTC0015a/test_RMLTVTC0015a_CSV.py
+-rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-tv/RMLTVTC0015b/country.csv
+-rw-r--r--   0        0        0     1029 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-tv/RMLTVTC0015b/mapping.ttl
+-rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-tv/RMLTVTC0015b/test_RMLTVTC0015b_CSV.py
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-tv/RMLTVTC0019a/employee.csv
+-rw-r--r--   0        0        0      568 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-tv/RMLTVTC0019a/mapping.ttl
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-tv/RMLTVTC0019a/output.nq
+-rw-r--r--   0        0        0      650 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-tv/RMLTVTC0019a/test_RMLTVTC0019a_CSV.py
+-rw-r--r--   0        0        0      538 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-tv/RMLTVTC0026a/mapping.ttl
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-tv/RMLTVTC0026a/mixed_content_list.csv
+-rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-tv/RMLTVTC0026a/output.nq
+-rw-r--r--   0        0        0      650 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-tv/RMLTVTC0026a/test_RMLTVTC0026a_CSV.py
+-rw-r--r--   0        0        0      751 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-tv/RMLTVTC0027a/mapping.ttl
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-tv/RMLTVTC0027a/mixed_content_json.csv
+-rw-r--r--   0        0        0      342 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-tv/RMLTVTC0027a/output.nq
+-rw-r--r--   0        0        0      650 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-tv/RMLTVTC0027a/test_RMLTVTC0027a_CSV.py
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-tv/RMLTVTC0028a/aka_title.csv
+-rw-r--r--   0        0        0      786 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-tv/RMLTVTC0028a/mapping.ttl
+-rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-tv/RMLTVTC0028a/output.nq
+-rw-r--r--   0        0        0      650 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-tv/RMLTVTC0028a/test_RMLTVTC0028a_CSV.py
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-tv/RMLTVTC0028a/title.csv
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-tv/RMLTVTC0029a/department.csv
+-rw-r--r--   0        0        0      299 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-tv/RMLTVTC0029a/faculty.csv
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-tv/RMLTVTC0029a/graduatecourse.csv
+-rw-r--r--   0        0        0      921 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-tv/RMLTVTC0029a/mapping.ttl
+-rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-tv/RMLTVTC0029a/output.nq
+-rw-r--r--   0        0        0      650 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/test/rml-tv/RMLTVTC0029a/test_RMLTVTC0029a_CSV.py
+-rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/LICENSE
+-rw-r--r--   0        0        0     6981 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/README.md
+-rw-r--r--   0        0        0     2870 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/pyproject.toml
+-rw-r--r--   0        0        0    10956 2020-02-02 00:00:00.000000 morph_kgc-2.7.0/PKG-INFO
```

### Comparing `morph_kgc-2.6.4/.zenodo.json` & `morph_kgc-2.7.0/.zenodo.json`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/CITATION.cff` & `morph_kgc-2.7.0/CITATION.cff`

 * *Files 9% similar despite different names*

```diff
@@ -17,12 +17,14 @@
       given-names: María S.
     - family-names: Corcho
       given-names: Oscar
   title: "Morph-KGC: Scalable knowledge graph materialization with mapping partitions"
   type: article
   journal: Semantic Web
   doi: 10.3233/SW-223135
-  year: 2022
+  year: 2024
+  volume: 15
+  issue: 1
 identifiers:
   - description: "Collection of archived snapshots for Morph-KGC"
     type: doi
     value: 10.5281/zenodo.6524684
```

### Comparing `morph_kgc-2.6.4/CODE_OF_CONDUCT.md` & `morph_kgc-2.7.0/CODE_OF_CONDUCT.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Contributor Code of Conduct
 
 **All creatures are welcome**: We aim to create a safe space for all community members, regardless of their age, race, gender, sexual orientation, physical appearance or disability, choice of text editor, or any other qualities by which living beings can be discriminated.
 
-**Be excellent to each other**: We do not tolerate verbal or physical harrassment, violence or intimidation.
+**Be excellent to each other**: We do not tolerate verbal or physical harassment, violence or intimidation.
 
 We do not tolerate life forms who refuse to share this openness and respect towards others: Creatures that are not excellent to others are not welcome.
 
 If you are made uncomfortable as a community member, please let us know: You can contact [julian.arenas.guerrero@upm.es](mailto:julian.arenas.guerrero@upm.es).
 
 #### Attribution
```

### Comparing `morph_kgc-2.6.4/CONTRIBUTING.md` & `morph_kgc-2.7.0/CONTRIBUTING.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Contributing
 
 We welcome contributions of new features or addressing any of the current [issues](https://github.com/morph-kgc/morph-kgc/issues). In order to push your contribution:
 
 - Push your pull request to the **main** branch.
 - If possible, create a [unit test](https://github.com/morph-kgc/morph-kgc/tree/main/test), to ensure that the issue does not occur again.
 - Please, provide a description with your pull request.
-- If applicable, update the [docs](https://github.com/morph-kgc/morph-kgc/tree/main/docs) accordingly.
+- If applicable, update the [docs](https://github.com/morph-kgc/morph-kgc-docs) accordingly.
 
 ## Testing
 
 We use [pytest](https://docs.pytest.org) for testing. In order to run the tests locally you need to install additional dependencies via:
 
 ```
 pip install .[test]
```

### Comparing `morph_kgc-2.6.4/.github/ISSUE_TEMPLATE/documentation-improvement.md` & `morph_kgc-2.7.0/.github/ISSUE_TEMPLATE/documentation-improvement.md`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/.github/ISSUE_TEMPLATE/feature-request.md` & `morph_kgc-2.7.0/.github/ISSUE_TEMPLATE/feature-request.md`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/.github/ISSUE_TEMPLATE/installation-issue.md` & `morph_kgc-2.7.0/.github/ISSUE_TEMPLATE/installation-issue.md`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/.github/workflows/ci.yml` & `morph_kgc-2.7.0/.github/workflows/ci.yml`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 jobs:
   build:
     runs-on: ${{ matrix.os }}
     strategy:
       matrix:
         os: [ubuntu-latest, macos-latest, windows-latest]
-        python-version: ['3.8', '3.11']
+        python-version: ['3.9', '3.11']
 
     steps:
     - uses: actions/checkout@v3
     - name: Set up Python ${{ matrix.python-version }}
       uses: actions/setup-python@v4
       with:
         python-version: ${{ matrix.python-version }}
```

### Comparing `morph_kgc-2.6.4/.github/workflows/pypi-publish.yml` & `morph_kgc-2.7.0/.github/workflows/pypi-publish.yml`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/docs/assets/logo.png` & `morph_kgc-2.7.0/logo/logo.png`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/examples/README.md` & `morph_kgc-2.7.0/examples/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -5,42 +5,40 @@
 [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1ByFx_NOEfTZeaJ1Wtw3UwTH3H3-Sye2O?usp=sharing)
 
 The tutorial in **[Google Colaboratory](https://colab.research.google.com/drive/1ByFx_NOEfTZeaJ1Wtw3UwTH3H3-Sye2O?usp=sharing)** is the easiest way to learn how to use Morph-KGC. Some relevant files for the tutorial can be found in the [`tutorial`](https://github.com/morph-kgc/morph-kgc/tree/main/examples/tutorial) directory.
 
 
 ### Relational Databases
 An example with _MySQL_ using [GTFS-Madrid-Bench](https://github.com/oeg-upm/gtfs-bench) data can be found in the [`rdb`](https://github.com/morph-kgc/morph-kgc/tree/main/examples/rdb) directory. The directory contains:
-- The `mapping` file.
+- The `mapping` file in [YARRRML](https://rml.io/yarrrml/spec/) format.
 - The `configuration` file that has to be provided to Morph-KGC.
 
 To start a docker container with the MySQL instance containing the data, run the following:
 ```bash
 docker run --name mysql-gtfs1 -p 3306:3306 -d -e MYSQL_ROOT_PASSWORD=gtfs oegdataintegration/mysql-gtfs1:1.0
 ```
 
-Note that the MySQL driver needs to be installed, as detailed in the **[documentation](https://morph-kgc.readthedocs.io/en/latest/documentation/#relational-databases_1)**. You just need to run the following:
+Note that the MySQL driver needs to be installed. You just need to install Morph-KGC in the following way:
 ```
-pip install pymysql
-pip install cryptography
+pip install morph-kgc[mysql]
 ```
 Also, **update the _paths_ parameters in the configuration file** accordingly.
 
 ### JSON and XML
 Examples for _JSON_ and _XML_ can be found in [`json`](https://github.com/morph-kgc/morph-kgc/tree/main/examples/json) and [`xml`](https://github.com/morph-kgc/morph-kgc/tree/main/examples/xml) directories. The directories contain:
-- The `data` file.
+- The `data` file in [YARRRML](https://rml.io/yarrrml/spec/) format.
 - The `mapping` file.
 - The `configuration` file that has to be provided to Morph-KGC.
-- The mapping file in [YARRRML](https://rml.io/yarrrml/spec/) format. This is **not** necessary, but allows to inspect the mapping in a human-readable format.
 
 Note that the **_paths_ parameters in the configuration file need to be updated** accordingly.
 
 ### CSV
 An example for _CSV_ can be found in the [`csv`](https://github.com/morph-kgc/morph-kgc/tree/main/examples/csv) directory. The directory contains:
 - The `data` directory with several CSV files.
-- The `mapping` file.
+- The `mapping` file in [YARRRML](https://rml.io/yarrrml/spec/) format.
 - The `configuration` file that has to be provided to Morph-KGC.
 
 Note that the **_paths_ parameters in the configuration file need to be updated** accordingly. Given that this example involves multiple CSV files, the paths to these files are provided in the mapping file with the `rml:source` property. The values of this property have to be updated with the correct _paths_ to the CSV files in your system.
 
 ### In-memory Data Structures
 Examples for [Python Dictionaries](https://docs.python.org/3/tutorial/datastructures.html#dictionaries) and [DataFrames](https://pandas.pydata.org/docs/reference/api/pandas.DataFrame.html) can be found in [`dict`](https://github.com/morph-kgc/morph-kgc/tree/main/examples/dict) and [`dataframe`](https://github.com/morph-kgc/morph-kgc/tree/main/examples/dataframe) directories.
```

### Comparing `morph_kgc-2.6.4/examples/configuration-file/default_config.ini` & `morph_kgc-2.7.0/examples/configuration-file/default_config.ini`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/examples/csv/mapping.csv.ttl` & `morph_kgc-2.7.0/examples/tutorial/mapping.gtfs.ttl`

 * *Files 8% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 @prefix schema: <http://schema.org/>.
 @prefix dct: <http://purl.org/dc/terms/>.
 
 :rules_000 a void:Dataset;
     void:exampleResource :map_stoptimes_000.
 :map_stoptimes_000 rml:logicalSource :source_000.
 :source_000 a rml:LogicalSource;
-    rml:source "data/STOP_TIMES.csv";
+    rml:source "https://raw.githubusercontent.com/oeg-upm/morph-kgc/main/examples/csv/data/STOP_TIMES.csv";
     rml:referenceFormulation ql:CSV.
 :map_stoptimes_000 a rr:TriplesMap;
     rdfs:label "stoptimes".
 :s_000 a rr:SubjectMap.
 :map_stoptimes_000 rr:subjectMap :s_000.
 :s_000 rr:template "http://transport.linkeddata.es/madrid/metro/stoptimes/{trip_id}-{stop_id}-{arrival_time}".
 :pom_000 a rr:PredicateObjectMap.
@@ -112,15 +112,15 @@
 :pm_009 a rr:PredicateMap.
 :pom_009 rr:predicateMap :pm_009.
 :pm_009 rr:constant gtfs:stop.
 :pom_009 rr:objectMap :om_009.
 :rules_000 void:exampleResource :map_trips_000.
 :map_trips_000 rml:logicalSource :source_001.
 :source_001 a rml:LogicalSource;
-    rml:source "data/TRIPS.csv";
+    rml:source "https://raw.githubusercontent.com/oeg-upm/morph-kgc/main/examples/csv/data/TRIPS.csv";
     rml:referenceFormulation ql:CSV.
 :map_trips_000 a rr:TriplesMap;
     rdfs:label "trips".
 :s_001 a rr:SubjectMap.
 :map_trips_000 rr:subjectMap :s_001.
 :s_001 rr:template "http://transport.linkeddata.es/madrid/metro/trips/{trip_id}".
 :pom_010 a rr:PredicateObjectMap.
@@ -194,15 +194,15 @@
 :pm_018 a rr:PredicateMap.
 :pom_018 rr:predicateMap :pm_018.
 :pm_018 rr:constant gtfs:shape.
 :pom_018 rr:objectMap :om_019.
 :rules_000 void:exampleResource :map_routes_000.
 :map_routes_000 rml:logicalSource :source_002.
 :source_002 a rml:LogicalSource;
-    rml:source "data/ROUTES.csv";
+    rml:source "https://raw.githubusercontent.com/oeg-upm/morph-kgc/main/examples/csv/data/ROUTES.csv";
     rml:referenceFormulation ql:CSV.
 :map_routes_000 a rr:TriplesMap;
     rdfs:label "routes".
 :s_002 a rr:SubjectMap.
 :map_routes_000 rr:subjectMap :s_002.
 :s_002 rr:template "http://transport.linkeddata.es/madrid/metro/routes/{route_id}".
 :pom_019 a rr:PredicateObjectMap.
@@ -282,15 +282,15 @@
 :pm_027 a rr:PredicateMap.
 :pom_027 rr:predicateMap :pm_027.
 :pm_027 rr:constant gtfs:agency.
 :pom_027 rr:objectMap :om_028.
 :rules_000 void:exampleResource :map_agency_000.
 :map_agency_000 rml:logicalSource :source_003.
 :source_003 a rml:LogicalSource;
-    rml:source "data/AGENCY.csv";
+    rml:source "https://raw.githubusercontent.com/oeg-upm/morph-kgc/main/examples/csv/data/AGENCY.csv";
     rml:referenceFormulation ql:CSV.
 :map_agency_000 a rr:TriplesMap;
     rdfs:label "agency".
 :s_003 a rr:SubjectMap.
 :map_agency_000 rr:subjectMap :s_003.
 :s_003 rr:template "http://transport.linkeddata.es/madrid/agency/{agency_id}".
 :pom_028 a rr:PredicateObjectMap.
@@ -355,15 +355,15 @@
 :pom_034 rr:objectMap :om_035.
 :om_035 a rr:ObjectMap;
     rml:reference "agency_fare_url";
     rr:termType rr:IRI.
 :rules_000 void:exampleResource :map_stops_000.
 :map_stops_000 rml:logicalSource :source_004.
 :source_004 a rml:LogicalSource;
-    rml:source "data/STOPS.csv";
+    rml:source "https://raw.githubusercontent.com/oeg-upm/morph-kgc/main/examples/csv/data/STOPS.csv";
     rml:referenceFormulation ql:CSV.
 :map_stops_000 a rr:TriplesMap;
     rdfs:label "stops".
 :s_004 a rr:SubjectMap.
 :map_stops_000 rr:subjectMap :s_004.
 :s_004 rr:template "http://transport.linkeddata.es/madrid/metro/stops/{stop_id}".
 :pom_035 a rr:PredicateObjectMap.
@@ -481,15 +481,15 @@
 :pm_047 a rr:PredicateMap.
 :pom_047 rr:predicateMap :pm_047.
 :pm_047 rr:constant gtfs:parentStation.
 :pom_047 rr:objectMap :om_048.
 :rules_000 void:exampleResource :map_services1_000.
 :map_services1_000 rml:logicalSource :source_005.
 :source_005 a rml:LogicalSource;
-    rml:source "data/CALENDAR.csv";
+    rml:source "https://raw.githubusercontent.com/oeg-upm/morph-kgc/main/examples/csv/data/CALENDAR.csv";
     rml:referenceFormulation ql:CSV.
 :map_services1_000 a rr:TriplesMap;
     rdfs:label "services1".
 :s_005 a rr:SubjectMap.
 :map_services1_000 rr:subjectMap :s_005.
 :s_005 rr:template "http://transport.linkeddata.es/madrid/metro/services/{service_id}".
 :pom_048 a rr:PredicateObjectMap.
@@ -506,15 +506,15 @@
 :pm_049 a rr:PredicateMap.
 :pom_049 rr:predicateMap :pm_049.
 :pm_049 rr:constant gtfs:serviceRule.
 :pom_049 rr:objectMap :om_050.
 :rules_000 void:exampleResource :map_services2_000.
 :map_services2_000 rml:logicalSource :source_006.
 :source_006 a rml:LogicalSource;
-    rml:source "data/CALENDAR_DATES.csv";
+    rml:source "https://raw.githubusercontent.com/oeg-upm/morph-kgc/main/examples/csv/data/CALENDAR_DATES.csv";
     rml:referenceFormulation ql:CSV.
 :map_services2_000 a rr:TriplesMap;
     rdfs:label "services2".
 :s_006 a rr:SubjectMap.
 :map_services2_000 rr:subjectMap :s_006.
 :s_006 rr:template "http://transport.linkeddata.es/madrid/metro/services/{service_id}".
 :pom_050 a rr:PredicateObjectMap.
@@ -531,15 +531,15 @@
 :pm_051 a rr:PredicateMap.
 :pom_051 rr:predicateMap :pm_051.
 :pm_051 rr:constant gtfs:serviceRule.
 :pom_051 rr:objectMap :om_052.
 :rules_000 void:exampleResource :map_calendar_date_rules_000.
 :map_calendar_date_rules_000 rml:logicalSource :source_007.
 :source_007 a rml:LogicalSource;
-    rml:source "data/CALENDAR_DATES.csv";
+    rml:source "https://raw.githubusercontent.com/oeg-upm/morph-kgc/main/examples/csv/data/CALENDAR_DATES.csv";
     rml:referenceFormulation ql:CSV.
 :map_calendar_date_rules_000 a rr:TriplesMap;
     rdfs:label "calendar_date_rules".
 :s_007 a rr:SubjectMap.
 :map_calendar_date_rules_000 rr:subjectMap :s_007.
 :s_007 rr:template "http://transport.linkeddata.es/madrid/metro/calendar_date_rule/{service_id}-{date}".
 :pom_052 a rr:PredicateObjectMap.
@@ -570,15 +570,15 @@
 :om_055 a rr:ObjectMap;
     rml:reference "exception_type";
     rr:termType rr:Literal;
     rr:datatype xsd:boolean.
 :rules_000 void:exampleResource :map_calendar_rules_000.
 :map_calendar_rules_000 rml:logicalSource :source_008.
 :source_008 a rml:LogicalSource;
-    rml:source "data/CALENDAR.csv";
+    rml:source "https://raw.githubusercontent.com/oeg-upm/morph-kgc/main/examples/csv/data/CALENDAR.csv";
     rml:referenceFormulation ql:CSV.
 :map_calendar_rules_000 a rr:TriplesMap;
     rdfs:label "calendar_rules".
 :s_008 a rr:SubjectMap.
 :map_calendar_rules_000 rr:subjectMap :s_008.
 :s_008 rr:template "http://transport.linkeddata.es/madrid/metro/calendar_rules/{service_id}".
 :pom_055 a rr:PredicateObjectMap.
@@ -679,15 +679,15 @@
 :om_065 a rr:ObjectMap;
     rml:reference "end_date";
     rr:termType rr:Literal;
     rr:datatype xsd:date.
 :rules_000 void:exampleResource :map_feed_000.
 :map_feed_000 rml:logicalSource :source_009.
 :source_009 a rml:LogicalSource;
-    rml:source "data/FEED_INFO.csv";
+    rml:source "https://raw.githubusercontent.com/oeg-upm/morph-kgc/main/examples/csv/data/FEED_INFO.csv";
     rml:referenceFormulation ql:CSV.
 :map_feed_000 a rr:TriplesMap;
     rdfs:label "feed".
 :s_009 a rr:SubjectMap.
 :map_feed_000 rr:subjectMap :s_009.
 :s_009 rr:template "http://transport.linkeddata.es/madrid/metro/feed/{feed_publisher_name}".
 :pom_065 a rr:PredicateObjectMap.
@@ -754,15 +754,15 @@
 :pom_071 rr:objectMap :om_072.
 :om_072 a rr:ObjectMap;
     rml:reference "feed_version";
     rr:termType rr:Literal.
 :rules_000 void:exampleResource :map_shapes_000.
 :map_shapes_000 rml:logicalSource :source_010.
 :source_010 a rml:LogicalSource;
-    rml:source "data/SHAPES.csv";
+    rml:source "https://raw.githubusercontent.com/oeg-upm/morph-kgc/main/examples/csv/data/SHAPES.csv";
     rml:referenceFormulation ql:CSV.
 :map_shapes_000 a rr:TriplesMap;
     rdfs:label "shapes".
 :s_010 a rr:SubjectMap.
 :map_shapes_000 rr:subjectMap :s_010.
 :s_010 rr:template "http://transport.linkeddata.es/madrid/metro/shape/{shape_id}".
 :pom_072 a rr:PredicateObjectMap.
@@ -778,19 +778,19 @@
 :map_shapes_000 rr:predicateObjectMap :pom_073.
 :pm_073 a rr:PredicateMap.
 :pom_073 rr:predicateMap :pm_073.
 :pm_073 rr:constant gtfs:shapePoint.
 :pom_073 rr:objectMap :om_074.
 :om_074 a rr:ObjectMap;
     rr:template "http://transport.linkeddata.es/madrid/metro/shape_point/{shape_id}-{shape_pt_sequence}";
-    rr:termType rr:IRI.
+    rr:termType rr:Literal.
 :rules_000 void:exampleResource :map_shapePoints_000.
 :map_shapePoints_000 rml:logicalSource :source_011.
 :source_011 a rml:LogicalSource;
-    rml:source "data/SHAPES.csv";
+    rml:source "https://raw.githubusercontent.com/oeg-upm/morph-kgc/main/examples/csv/data/SHAPES.csv";
     rml:referenceFormulation ql:CSV.
 :map_shapePoints_000 a rr:TriplesMap;
     rdfs:label "shapePoints".
 :s_011 a rr:SubjectMap.
 :map_shapePoints_000 rr:subjectMap :s_011.
 :s_011 rr:template "http://transport.linkeddata.es/madrid/metro/shape_point/{shape_id}-{shape_pt_sequence}".
 :pom_074 a rr:PredicateObjectMap.
@@ -839,15 +839,15 @@
 :pom_078 rr:objectMap :om_079.
 :om_079 a rr:ObjectMap;
     rml:reference "shape_dist_traveled";
     rr:termType rr:Literal.
 :rules_000 void:exampleResource :map_frequencies_000.
 :map_frequencies_000 rml:logicalSource :source_012.
 :source_012 a rml:LogicalSource;
-    rml:source "data/FREQUENCIES.csv";
+    rml:source "https://raw.githubusercontent.com/oeg-upm/morph-kgc/main/examples/csv/data/FREQUENCIES.csv";
     rml:referenceFormulation ql:CSV.
 :map_frequencies_000 a rr:TriplesMap;
     rdfs:label "frequencies".
 :s_012 a rr:SubjectMap.
 :map_frequencies_000 rr:subjectMap :s_012.
 :s_012 rr:template "http://transport.linkeddata.es/madrid/metro/frequency/{trip_id}-{start_time}".
 :pom_079 a rr:PredicateObjectMap.
```

### Comparing `morph_kgc-2.6.4/examples/csv/data/FREQUENCIES.csv` & `morph_kgc-2.7.0/examples/csv/data/FREQUENCIES.csv`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/examples/csv/data/ROUTES.csv` & `morph_kgc-2.7.0/examples/csv/data/ROUTES.csv`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/examples/csv/data/SHAPES.csv` & `morph_kgc-2.7.0/examples/csv/data/SHAPES.csv`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/examples/csv/data/STOPS.csv` & `morph_kgc-2.7.0/examples/csv/data/STOPS.csv`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/examples/csv/data/STOP_TIMES.csv` & `morph_kgc-2.7.0/examples/csv/data/STOP_TIMES.csv`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/examples/csv/data/TRIPS.csv` & `morph_kgc-2.7.0/examples/csv/data/TRIPS.csv`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/examples/dataframe/kg_generation.py` & `morph_kgc-2.7.0/examples/dataframe/kg_generation.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 data_dict = {"variable1": users_df,
             "variable2": followers_df}
 
 
 config = """
     [DataSource]
-    mappings=./mapping_rml.ttl
+    mappings=./mapping.rml.ttl
 """
 
 g_rdflib = morph_kgc.materialize('./config.ini', data_dict)
 
 print("Knowledge graphs triples:")
 for s,p,o in g_rdflib.triples((None, None, None)):
     print(s,p,o)
```

### Comparing `morph_kgc-2.6.4/examples/dict/kg_generation.py` & `morph_kgc-2.7.0/examples/dict/kg_generation.py`

 * *Files 1% similar despite different names*

```diff
@@ -61,15 +61,15 @@
     ]}
 
 data_dict = {"variable1": users_dict,
             "variable2": followers_dict}
 
 config = """
     [DataSource]
-    mappings=./mapping_rml.ttl
+    mappings=./mapping.rml.ttl
 """
 
 g_rdflib = morph_kgc.materialize('./config.ini', data_dict)
 
 print("Knowledge graphs triples:")
 for s,p,o in g_rdflib.triples((None, None, None)):
     print(s,p,o)
```

### Comparing `morph_kgc-2.6.4/examples/json/data.json` & `morph_kgc-2.7.0/examples/json/data.json`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/examples/json/mapping.json.ttl` & `morph_kgc-2.7.0/test/rml-core/json/complex/mapping.ttl`

 * *Files 26% similar despite different names*

```diff
@@ -1,264 +1,264 @@
-@prefix rr: <http://www.w3.org/ns/r2rml#>.
-@prefix rml: <http://semweb.mmlab.be/ns/rml#>.
-@prefix rdf: <http://www.w3.org/1999/02/22-rdf-syntax-ns#>.
-@prefix rdfs: <http://www.w3.org/2000/01/rdf-schema#>.
-@prefix ql: <http://semweb.mmlab.be/ns/ql#>.
-@prefix map: <http://mapping.example.com/>.
-
-map:jc_000 rr:child "id";
-    rr:parent "id".
-map:language_000 rml:reference "language.code".
-map:map_Author_000 rml:logicalSource map:source_001;
-    a rr:TriplesMap;
-    rdfs:label "Author";
-    rr:subjectMap map:s_000;
-    rr:predicateObjectMap map:pom_000, map:pom_001, map:pom_002, map:pom_003, map:pom_004.
-map:map_idTypeOpenAire_000 rml:logicalSource map:source_002;
-    a rr:TriplesMap;
-    rdfs:label "idTypeOpenAire";
-    rr:subjectMap map:s_002;
-    rr:predicateObjectMap map:pom_020, map:pom_021, map:pom_022.
-map:map_idTypePaperResource_000 rml:logicalSource map:source_002;
-    a rr:TriplesMap;
-    rdfs:label "idTypePaperResource";
-    rr:subjectMap map:s_003;
-    rr:predicateObjectMap map:pom_023, map:pom_024, map:pom_025.
-map:map_Paper_000 rml:logicalSource map:source_000;
-    a rr:TriplesMap;
-    rdfs:label "Paper";
-    rr:subjectMap map:s_001;
-    rr:predicateObjectMap map:pom_005, map:pom_006, map:pom_007, map:pom_008, map:pom_009, map:pom_010, map:pom_011, map:pom_012, map:pom_013, map:pom_014, map:pom_015, map:pom_016, map:pom_017, map:pom_018, map:pom_019.
-map:om_000 a rr:ObjectMap;
-    rr:constant "https://w3id.org/okn/os/o/Author";
-    rr:termType rr:IRI.
-map:om_001 a rr:ObjectMap;
-    rml:reference "fullname";
-    rr:termType rr:Literal.
-map:om_002 a rr:ObjectMap;
-    rml:reference "name";
-    rr:termType rr:Literal.
-map:om_003 a rr:ObjectMap;
-    rml:reference "surname";
-    rr:termType rr:Literal.
-map:om_004 a rr:ObjectMap;
-    rml:reference "pid.id.value";
-    rr:termType rr:Literal.
-map:om_005 a rr:ObjectMap;
-    rr:constant "https://w3id.org/okn/os/o/Paper";
-    rr:termType rr:IRI.
-map:om_006 a rr:ObjectMap;
-    rml:reference "maintitle";
-    rr:termType rr:Literal.
-map:om_007 a rr:ObjectMap;
-    rml:reference "subtitle";
-    rr:termType rr:Literal.
-map:om_008 a rr:ObjectMap;
-    rml:reference "description";
-    rr:termType rr:Literal;
-    rml:languageMap map:language_000.
-map:om_009 a rr:ObjectMap;
-    rml:reference "language.label";
-    rr:termType rr:Literal.
-map:om_010 a rr:ObjectMap;
-    rml:reference "format";
-    rr:termType rr:Literal.
-map:om_011 a rr:ObjectMap;
-    rml:reference "publicationdate";
-    rr:termType rr:Literal.
-map:om_012 a rr:ObjectMap;
-    rml:reference "type";
-    rr:termType rr:Literal.
-map:om_013 a rr:ObjectMap;
-    rml:reference "country.*.label";
-    rr:termType rr:Literal.
-map:om_014 a rr:ObjectMap;
-    rml:reference "instance.*.license";
-    rr:termType rr:Literal.
-map:om_015 a rr:ObjectMap;
-    rml:reference "publisher";
-    rr:termType rr:Literal.
-map:om_016 a rr:ObjectMap;
-    rml:reference "source";
-    rr:termType rr:Literal.
-map:om_017 a rr:ObjectMap;
-    rr:template "https://w3id.org/okn/os/i/idType/{pid.*.value}";
-    rr:termType rr:IRI.
-map:om_018 a rr:ObjectMap;
-    rr:template "https://w3id.org/okn/os/i/author/{author.*.fullname}";
-    rr:termType rr:IRI.
-map:om_019 a rr:ObjectMap;
-    rr:parentTriplesMap map:map_idTypeOpenAire_000;
-    rr:joinCondition map:jc_000.
-map:om_020 a rr:ObjectMap;
-    rr:constant "https://w3id.org/okn/os/o/idType";
-    rr:termType rr:IRI.
-map:om_021 a rr:ObjectMap;
-    rr:constant "OpenAire";
-    rr:termType rr:Literal.
-map:om_022 a rr:ObjectMap;
-    rml:reference "id";
-    rr:termType rr:Literal.
-map:om_023 a rr:ObjectMap;
-    rr:constant "https://w3id.org/okn/os/o/idType";
-    rr:termType rr:IRI.
-map:om_024 a rr:ObjectMap;
-    rml:reference "scheme";
-    rr:termType rr:Literal.
-map:om_025 a rr:ObjectMap;
-    rml:reference "value";
-    rr:termType rr:Literal.
-map:pm_000 a rr:PredicateMap;
-    rr:constant rdf:type.
-map:pm_001 a rr:PredicateMap;
-    rr:constant <https://w3id.org/okn/os/o/fullname>.
-map:pm_002 a rr:PredicateMap;
-    rr:constant <https://w3id.org/okn/os/o/name>.
-map:pm_003 a rr:PredicateMap;
-    rr:constant <https://w3id.org/okn/os/o/surname>.
-map:pm_004 a rr:PredicateMap;
-    rr:template "https://w3id.org/okn/os/o/{pid.id.scheme}ID".
-map:pm_005 a rr:PredicateMap;
-    rr:constant rdf:type.
-map:pm_006 a rr:PredicateMap;
-    rr:constant <https://w3id.org/okn/os/o/title>.
-map:pm_007 a rr:PredicateMap;
-    rr:constant <https://w3id.org/okn/os/o/subtitle>.
-map:pm_008 a rr:PredicateMap;
-    rr:constant <https://w3id.org/okn/os/o/description>.
-map:pm_009 a rr:PredicateMap;
-    rr:constant <https://w3id.org/okn/os/o/language>.
-map:pm_010 a rr:PredicateMap;
-    rr:constant <https://w3id.org/okn/os/o/format>.
-map:pm_011 a rr:PredicateMap;
-    rr:constant <https://w3id.org/okn/os/o/publicationDate>.
-map:pm_012 a rr:PredicateMap;
-    rr:constant <https://w3id.org/okn/os/o/type>.
-map:pm_013 a rr:PredicateMap;
-    rr:constant <https://w3id.org/okn/os/o/country>.
-map:pm_014 a rr:PredicateMap;
-    rr:constant <https://w3id.org/okn/os/o/license>.
-map:pm_015 a rr:PredicateMap;
-    rr:constant <https://w3id.org/okn/os/o/publisher>.
-map:pm_016 a rr:PredicateMap;
-    rr:constant <https://w3id.org/okn/os/o/source>.
-map:pm_017 a rr:PredicateMap;
-    rr:constant <https://w3id.org/okn/os/o/has_id>.
-map:pm_018 a rr:PredicateMap;
-    rr:constant <https://w3id.org/okn/os/o/has_id>.
-map:pm_019 a rr:PredicateMap;
-    rr:constant <https://w3id.org/okn/os/o/has_id>.
-map:pm_020 a rr:PredicateMap;
-    rr:constant rdf:type.
-map:pm_021 a rr:PredicateMap;
-    rr:constant <https://w3id.org/okn/os/o/source>.
-map:pm_022 a rr:PredicateMap;
-    rr:constant <https://w3id.org/okn/os/o/identifier>.
-map:pm_023 a rr:PredicateMap;
-    rr:constant rdf:type.
-map:pm_024 a rr:PredicateMap;
-    rr:constant <https://w3id.org/okn/os/o/source>.
-map:pm_025 a rr:PredicateMap;
-    rr:constant <https://w3id.org/okn/os/o/identifier>.
-map:pom_000 a rr:PredicateObjectMap;
-    rr:predicateMap map:pm_000;
-    rr:objectMap map:om_000.
-map:pom_001 a rr:PredicateObjectMap;
-    rr:predicateMap map:pm_001;
-    rr:objectMap map:om_001.
-map:pom_002 a rr:PredicateObjectMap;
-    rr:predicateMap map:pm_002;
-    rr:objectMap map:om_002.
-map:pom_003 a rr:PredicateObjectMap;
-    rr:predicateMap map:pm_003;
-    rr:objectMap map:om_003.
-map:pom_004 a rr:PredicateObjectMap;
-    rr:predicateMap map:pm_004;
-    rr:objectMap map:om_004.
-map:pom_005 a rr:PredicateObjectMap;
-    rr:predicateMap map:pm_005;
-    rr:objectMap map:om_005.
-map:pom_006 a rr:PredicateObjectMap;
-    rr:predicateMap map:pm_006;
-    rr:objectMap map:om_006.
-map:pom_007 a rr:PredicateObjectMap;
-    rr:predicateMap map:pm_007;
-    rr:objectMap map:om_007.
-map:pom_008 a rr:PredicateObjectMap;
-    rr:predicateMap map:pm_008;
-    rr:objectMap map:om_008.
-map:pom_009 a rr:PredicateObjectMap;
-    rr:predicateMap map:pm_009;
-    rr:objectMap map:om_009.
-map:pom_010 a rr:PredicateObjectMap;
-    rr:predicateMap map:pm_010;
-    rr:objectMap map:om_010.
-map:pom_011 a rr:PredicateObjectMap;
-    rr:predicateMap map:pm_011;
-    rr:objectMap map:om_011.
-map:pom_012 a rr:PredicateObjectMap;
-    rr:predicateMap map:pm_012;
-    rr:objectMap map:om_012.
-map:pom_013 a rr:PredicateObjectMap;
-    rr:predicateMap map:pm_013;
-    rr:objectMap map:om_013.
-map:pom_014 a rr:PredicateObjectMap;
-    rr:predicateMap map:pm_014;
-    rr:objectMap map:om_014.
-map:pom_015 a rr:PredicateObjectMap;
-    rr:predicateMap map:pm_015;
-    rr:objectMap map:om_015.
-map:pom_016 a rr:PredicateObjectMap;
-    rr:predicateMap map:pm_016;
-    rr:objectMap map:om_016.
-map:pom_017 a rr:PredicateObjectMap;
-    rr:predicateMap map:pm_017;
-    rr:objectMap map:om_017.
-map:pom_018 a rr:PredicateObjectMap;
-    rr:predicateMap map:pm_018;
-    rr:objectMap map:om_018.
-map:pom_019 a rr:PredicateObjectMap;
-    rr:predicateMap map:pm_019;
-    rr:objectMap map:om_019.
-map:pom_020 a rr:PredicateObjectMap;
-    rr:predicateMap map:pm_020;
-    rr:objectMap map:om_020.
-map:pom_021 a rr:PredicateObjectMap;
-    rr:predicateMap map:pm_021;
-    rr:objectMap map:om_021.
-map:pom_022 a rr:PredicateObjectMap;
-    rr:predicateMap map:pm_022;
-    rr:objectMap map:om_022.
-map:pom_023 a rr:PredicateObjectMap;
-    rr:predicateMap map:pm_023;
-    rr:objectMap map:om_023.
-map:pom_024 a rr:PredicateObjectMap;
-    rr:predicateMap map:pm_024;
-    rr:objectMap map:om_024.
-map:pom_025 a rr:PredicateObjectMap;
-    rr:predicateMap map:pm_025;
-    rr:objectMap map:om_025.
-map:rules_000 a <http://rdfs.org/ns/void#Dataset>;
-    <http://rdfs.org/ns/void#exampleResource> map:map_Author_000, map:map_Paper_000, map:map_idTypeOpenAire_000, map:map_idTypePaperResource_000.
-map:s_000 a rr:SubjectMap;
-    rr:template "https://w3id.org/okn/os/i/author/{fullname}".
-map:s_001 a rr:SubjectMap;
-    rr:template "https://w3id.org/okn/os/i/paper/{id}".
-map:s_002 a rr:SubjectMap;
-    rr:template "https://w3id.org/okn/os/i/idType/{id}".
-map:s_003 a rr:SubjectMap;
-    rr:template "https://w3id.org/okn/os/i/idType/{value}".
-map:source_000 a rml:LogicalSource;
-    rdfs:label "main-source";
-    rml:source "data.json";
-    rml:iterator "$.*";
-    rml:referenceFormulation ql:JSONPath.
-map:source_001 a rml:LogicalSource;
-    rdfs:label "author-source";
-    rml:source "data.json";
-    rml:iterator "$.*.author[*]";
-    rml:referenceFormulation ql:JSONPath.
-map:source_002 a rml:LogicalSource;
-    rdfs:label "pid-source";
-    rml:source "data.json";
-    rml:iterator "$.*.pid[*]";
-    rml:referenceFormulation ql:JSONPath.
+@prefix rr: <http://www.w3.org/ns/r2rml#>.
+@prefix rml: <http://w3id.org/rml/>.
+@prefix rdf: <http://www.w3.org/1999/02/22-rdf-syntax-ns#>.
+@prefix rdfs: <http://www.w3.org/2000/01/rdf-schema#>.
+@prefix ql: <http://semweb.mmlab.be/ns/ql#>.
+@prefix map: <http://mapping.example.com/>.
+
+map:jc_000 rml:child "id";
+    rml:parent "id".
+map:language_000 rml:reference "language.code".
+map:map_Author_000 rml:logicalSource map:source_001;
+    a rml:TriplesMap;
+    rdfs:label "Author";
+    rml:subjectMap map:s_000;
+    rml:predicateObjectMap map:pom_000, map:pom_001, map:pom_002, map:pom_003, map:pom_004.
+map:map_idTypeOpenAire_000 rml:logicalSource map:source_002;
+    a rml:TriplesMap;
+    rdfs:label "idTypeOpenAire";
+    rml:subjectMap map:s_002;
+    rml:predicateObjectMap map:pom_020, map:pom_021, map:pom_022.
+map:map_idTypePaperResource_000 rml:logicalSource map:source_002;
+    a rml:TriplesMap;
+    rdfs:label "idTypePaperResource";
+    rml:subjectMap map:s_003;
+    rml:predicateObjectMap map:pom_023, map:pom_024, map:pom_025.
+map:map_Paper_000 rml:logicalSource map:source_000;
+    a rml:TriplesMap;
+    rdfs:label "Paper";
+    rml:subjectMap map:s_001;
+    rml:predicateObjectMap map:pom_005, map:pom_006, map:pom_007, map:pom_008, map:pom_009, map:pom_010, map:pom_011, map:pom_012, map:pom_013, map:pom_014, map:pom_015, map:pom_016, map:pom_017, map:pom_018, map:pom_019.
+map:om_000 a rml:ObjectMap;
+    rml:constant "https://w3id.org/okn/os/o/Author";
+    rml:termType rml:IRI.
+map:om_001 a rml:ObjectMap;
+    rml:reference "fullname";
+    rml:termType rml:Literal.
+map:om_002 a rml:ObjectMap;
+    rml:reference "name";
+    rml:termType rml:Literal.
+map:om_003 a rml:ObjectMap;
+    rml:reference "surname";
+    rml:termType rml:Literal.
+map:om_004 a rml:ObjectMap;
+    rml:reference "pid.id.value";
+    rml:termType rml:Literal.
+map:om_005 a rml:ObjectMap;
+    rml:constant "https://w3id.org/okn/os/o/Paper";
+    rml:termType rml:IRI.
+map:om_006 a rml:ObjectMap;
+    rml:reference "maintitle";
+    rml:termType rml:Literal.
+map:om_007 a rml:ObjectMap;
+    rml:reference "subtitle";
+    rml:termType rml:Literal.
+map:om_008 a rml:ObjectMap;
+    rml:reference "description";
+    rml:termType rml:Literal;
+    rml:languageMap map:language_000.
+map:om_009 a rml:ObjectMap;
+    rml:reference "language.label";
+    rml:termType rml:Literal.
+map:om_010 a rml:ObjectMap;
+    rml:reference "format";
+    rml:termType rml:Literal.
+map:om_011 a rml:ObjectMap;
+    rml:reference "publicationdate";
+    rml:termType rml:Literal.
+map:om_012 a rml:ObjectMap;
+    rml:reference "type";
+    rml:termType rml:Literal.
+map:om_013 a rml:ObjectMap;
+    rml:reference "country.*.label";
+    rml:termType rml:Literal.
+map:om_014 a rml:ObjectMap;
+    rml:reference "instance.*.license";
+    rml:termType rml:Literal.
+map:om_015 a rml:ObjectMap;
+    rml:reference "publisher";
+    rml:termType rml:Literal.
+map:om_016 a rml:ObjectMap;
+    rml:reference "source";
+    rml:termType rml:Literal.
+map:om_017 a rml:ObjectMap;
+    rml:template "https://w3id.org/okn/os/i/idType/{pid.*.value}";
+    rml:termType rml:IRI.
+map:om_018 a rml:ObjectMap;
+    rml:template "https://w3id.org/okn/os/i/author/{author.*.fullname}";
+    rml:termType rml:IRI.
+map:om_019 a rml:ObjectMap;
+    rml:parentTriplesMap map:map_idTypeOpenAire_000;
+    rml:joinCondition map:jc_000.
+map:om_020 a rml:ObjectMap;
+    rml:constant "https://w3id.org/okn/os/o/idType";
+    rml:termType rml:IRI.
+map:om_021 a rml:ObjectMap;
+    rml:constant "OpenAire";
+    rml:termType rml:Literal.
+map:om_022 a rml:ObjectMap;
+    rml:reference "id";
+    rml:termType rml:Literal.
+map:om_023 a rml:ObjectMap;
+    rml:constant "https://w3id.org/okn/os/o/idType";
+    rml:termType rml:IRI.
+map:om_024 a rml:ObjectMap;
+    rml:reference "scheme";
+    rml:termType rml:Literal.
+map:om_025 a rml:ObjectMap;
+    rml:reference "value";
+    rml:termType rml:Literal.
+map:pm_000 a rml:PredicateMap;
+    rml:constant rdf:type.
+map:pm_001 a rml:PredicateMap;
+    rml:constant <https://w3id.org/okn/os/o/fullname>.
+map:pm_002 a rml:PredicateMap;
+    rml:constant <https://w3id.org/okn/os/o/name>.
+map:pm_003 a rml:PredicateMap;
+    rml:constant <https://w3id.org/okn/os/o/surname>.
+map:pm_004 a rml:PredicateMap;
+    rml:template "https://w3id.org/okn/os/o/{pid.id.scheme}ID".
+map:pm_005 a rml:PredicateMap;
+    rml:constant rdf:type.
+map:pm_006 a rml:PredicateMap;
+    rml:constant <https://w3id.org/okn/os/o/title>.
+map:pm_007 a rml:PredicateMap;
+    rml:constant <https://w3id.org/okn/os/o/subtitle>.
+map:pm_008 a rml:PredicateMap;
+    rml:constant <https://w3id.org/okn/os/o/description>.
+map:pm_009 a rml:PredicateMap;
+    rml:constant <https://w3id.org/okn/os/o/language>.
+map:pm_010 a rml:PredicateMap;
+    rml:constant <https://w3id.org/okn/os/o/format>.
+map:pm_011 a rml:PredicateMap;
+    rml:constant <https://w3id.org/okn/os/o/publicationDate>.
+map:pm_012 a rml:PredicateMap;
+    rml:constant <https://w3id.org/okn/os/o/type>.
+map:pm_013 a rml:PredicateMap;
+    rml:constant <https://w3id.org/okn/os/o/country>.
+map:pm_014 a rml:PredicateMap;
+    rml:constant <https://w3id.org/okn/os/o/license>.
+map:pm_015 a rml:PredicateMap;
+    rml:constant <https://w3id.org/okn/os/o/publisher>.
+map:pm_016 a rml:PredicateMap;
+    rml:constant <https://w3id.org/okn/os/o/source>.
+map:pm_017 a rml:PredicateMap;
+    rml:constant <https://w3id.org/okn/os/o/has_id>.
+map:pm_018 a rml:PredicateMap;
+    rml:constant <https://w3id.org/okn/os/o/has_id>.
+map:pm_019 a rml:PredicateMap;
+    rml:constant <https://w3id.org/okn/os/o/has_id>.
+map:pm_020 a rml:PredicateMap;
+    rml:constant rdf:type.
+map:pm_021 a rml:PredicateMap;
+    rml:constant <https://w3id.org/okn/os/o/source>.
+map:pm_022 a rml:PredicateMap;
+    rml:constant <https://w3id.org/okn/os/o/identifier>.
+map:pm_023 a rml:PredicateMap;
+    rml:constant rdf:type.
+map:pm_024 a rml:PredicateMap;
+    rml:constant <https://w3id.org/okn/os/o/source>.
+map:pm_025 a rml:PredicateMap;
+    rml:constant <https://w3id.org/okn/os/o/identifier>.
+map:pom_000 a rml:PredicateObjectMap;
+    rml:predicateMap map:pm_000;
+    rml:objectMap map:om_000.
+map:pom_001 a rml:PredicateObjectMap;
+    rml:predicateMap map:pm_001;
+    rml:objectMap map:om_001.
+map:pom_002 a rml:PredicateObjectMap;
+    rml:predicateMap map:pm_002;
+    rml:objectMap map:om_002.
+map:pom_003 a rml:PredicateObjectMap;
+    rml:predicateMap map:pm_003;
+    rml:objectMap map:om_003.
+map:pom_004 a rml:PredicateObjectMap;
+    rml:predicateMap map:pm_004;
+    rml:objectMap map:om_004.
+map:pom_005 a rml:PredicateObjectMap;
+    rml:predicateMap map:pm_005;
+    rml:objectMap map:om_005.
+map:pom_006 a rml:PredicateObjectMap;
+    rml:predicateMap map:pm_006;
+    rml:objectMap map:om_006.
+map:pom_007 a rml:PredicateObjectMap;
+    rml:predicateMap map:pm_007;
+    rml:objectMap map:om_007.
+map:pom_008 a rml:PredicateObjectMap;
+    rml:predicateMap map:pm_008;
+    rml:objectMap map:om_008.
+map:pom_009 a rml:PredicateObjectMap;
+    rml:predicateMap map:pm_009;
+    rml:objectMap map:om_009.
+map:pom_010 a rml:PredicateObjectMap;
+    rml:predicateMap map:pm_010;
+    rml:objectMap map:om_010.
+map:pom_011 a rml:PredicateObjectMap;
+    rml:predicateMap map:pm_011;
+    rml:objectMap map:om_011.
+map:pom_012 a rml:PredicateObjectMap;
+    rml:predicateMap map:pm_012;
+    rml:objectMap map:om_012.
+map:pom_013 a rml:PredicateObjectMap;
+    rml:predicateMap map:pm_013;
+    rml:objectMap map:om_013.
+map:pom_014 a rml:PredicateObjectMap;
+    rml:predicateMap map:pm_014;
+    rml:objectMap map:om_014.
+map:pom_015 a rml:PredicateObjectMap;
+    rml:predicateMap map:pm_015;
+    rml:objectMap map:om_015.
+map:pom_016 a rml:PredicateObjectMap;
+    rml:predicateMap map:pm_016;
+    rml:objectMap map:om_016.
+map:pom_017 a rml:PredicateObjectMap;
+    rml:predicateMap map:pm_017;
+    rml:objectMap map:om_017.
+map:pom_018 a rml:PredicateObjectMap;
+    rml:predicateMap map:pm_018;
+    rml:objectMap map:om_018.
+map:pom_019 a rml:PredicateObjectMap;
+    rml:predicateMap map:pm_019;
+    rml:objectMap map:om_019.
+map:pom_020 a rml:PredicateObjectMap;
+    rml:predicateMap map:pm_020;
+    rml:objectMap map:om_020.
+map:pom_021 a rml:PredicateObjectMap;
+    rml:predicateMap map:pm_021;
+    rml:objectMap map:om_021.
+map:pom_022 a rml:PredicateObjectMap;
+    rml:predicateMap map:pm_022;
+    rml:objectMap map:om_022.
+map:pom_023 a rml:PredicateObjectMap;
+    rml:predicateMap map:pm_023;
+    rml:objectMap map:om_023.
+map:pom_024 a rml:PredicateObjectMap;
+    rml:predicateMap map:pm_024;
+    rml:objectMap map:om_024.
+map:pom_025 a rml:PredicateObjectMap;
+    rml:predicateMap map:pm_025;
+    rml:objectMap map:om_025.
+map:rules_000 a <http://rdfs.org/ns/void#Dataset>;
+    <http://rdfs.org/ns/void#exampleResource> map:map_Author_000, map:map_Paper_000, map:map_idTypeOpenAire_000, map:map_idTypePaperResource_000.
+map:s_000 a rml:SubjectMap;
+    rml:template "https://w3id.org/okn/os/i/author/{fullname}".
+map:s_001 a rml:SubjectMap;
+    rml:template "https://w3id.org/okn/os/i/paper/{id}".
+map:s_002 a rml:SubjectMap;
+    rml:template "https://w3id.org/okn/os/i/idType/{id}".
+map:s_003 a rml:SubjectMap;
+    rml:template "https://w3id.org/okn/os/i/idType/{value}".
+map:source_000 a rml:LogicalSource;
+    rdfs:label "main-source";
+    rml:source "test/rml-core/json/complex/data.json";
+    rml:iterator "$.*";
+    rml:referenceFormulation rml:JSONPath.
+map:source_001 a rml:LogicalSource;
+    rdfs:label "author-source";
+    rml:source "test/rml-core/json/complex/data.json";
+    rml:iterator "$.*.author[*]";
+    rml:referenceFormulation rml:JSONPath.
+map:source_002 a rml:LogicalSource;
+    rdfs:label "pid-source";
+    rml:source "test/rml-core/json/complex/data.json";
+    rml:iterator "$.*.pid[*]";
+    rml:referenceFormulation rml:JSONPath.
```

### Comparing `morph_kgc-2.6.4/examples/json/mapping.json.yaml` & `morph_kgc-2.7.0/test/rml-core/json/complex/mapping.yaml`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/examples/tutorial/Morph-KGC.ipynb` & `morph_kgc-2.7.0/examples/tutorial/Morph-KGC.ipynb`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/examples/tutorial/mapping.somef.ttl` & `morph_kgc-2.7.0/examples/tutorial/mapping.somef.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/examples/tutorial/oeg-upm_morph-kgc.json` & `morph_kgc-2.7.0/examples/tutorial/oeg-upm_morph-kgc.json`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/examples/xml/data.xml` & `morph_kgc-2.7.0/examples/xml/data.xml`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/examples/xml/mapping.xml.yaml` & `morph_kgc-2.7.0/test/rml-core/xml/complex/mapping.yaml`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/examples/xml/mappingOA.xml.ttl` & `morph_kgc-2.7.0/test/rml-core/xml/complex/mapping.ttl`

 * *Files 26% similar despite different names*

```diff
@@ -1,264 +1,264 @@
-@prefix rr: <http://www.w3.org/ns/r2rml#>.
-@prefix rml: <http://semweb.mmlab.be/ns/rml#>.
-@prefix rdf: <http://www.w3.org/1999/02/22-rdf-syntax-ns#>.
-@prefix rdfs: <http://www.w3.org/2000/01/rdf-schema#>.
-@prefix ql: <http://semweb.mmlab.be/ns/ql#>.
-@prefix map: <http://mapping.example.com/>.
-
-map:jc_000 rr:child "id";
-    rr:parent "id".
-map:language_000 rml:reference "language.code".
-map:map_Author_000 rml:logicalSource map:source_001;
-    a rr:TriplesMap;
-    rdfs:label "Author";
-    rr:subjectMap map:s_000;
-    rr:predicateObjectMap map:pom_000, map:pom_001, map:pom_002, map:pom_003, map:pom_004.
-map:map_idTypeOpenAire_000 rml:logicalSource map:source_002;
-    a rr:TriplesMap;
-    rdfs:label "idTypeOpenAire";
-    rr:subjectMap map:s_002;
-    rr:predicateObjectMap map:pom_020, map:pom_021, map:pom_022.
-map:map_idTypePaperResource_000 rml:logicalSource map:source_002;
-    a rr:TriplesMap;
-    rdfs:label "idTypePaperResource";
-    rr:subjectMap map:s_003;
-    rr:predicateObjectMap map:pom_023, map:pom_024, map:pom_025.
-map:map_Paper_000 rml:logicalSource map:source_000;
-    a rr:TriplesMap;
-    rdfs:label "Paper";
-    rr:subjectMap map:s_001;
-    rr:predicateObjectMap map:pom_005, map:pom_006, map:pom_007, map:pom_008, map:pom_009, map:pom_010, map:pom_011, map:pom_012, map:pom_013, map:pom_014, map:pom_015, map:pom_016, map:pom_017, map:pom_018, map:pom_019.
-map:om_000 a rr:ObjectMap;
-    rr:constant "https://w3id.org/okn/os/o/Author";
-    rr:termType rr:IRI.
-map:om_001 a rr:ObjectMap;
-    rml:reference "fullname";
-    rr:termType rr:Literal.
-map:om_002 a rr:ObjectMap;
-    rml:reference "name";
-    rr:termType rr:Literal.
-map:om_003 a rr:ObjectMap;
-    rml:reference "surname";
-    rr:termType rr:Literal.
-map:om_004 a rr:ObjectMap;
-    rml:reference "pid.id.value";
-    rr:termType rr:Literal.
-map:om_005 a rr:ObjectMap;
-    rr:constant "https://w3id.org/okn/os/o/Paper";
-    rr:termType rr:IRI.
-map:om_006 a rr:ObjectMap;
-    rml:reference "maintitle";
-    rr:termType rr:Literal.
-map:om_007 a rr:ObjectMap;
-    rml:reference "subtitle";
-    rr:termType rr:Literal.
-map:om_008 a rr:ObjectMap;
-    rml:reference "description";
-    rr:termType rr:Literal;
-    rml:languageMap map:language_000.
-map:om_009 a rr:ObjectMap;
-    rml:reference "language.label";
-    rr:termType rr:Literal.
-map:om_010 a rr:ObjectMap;
-    rml:reference "format";
-    rr:termType rr:Literal.
-map:om_011 a rr:ObjectMap;
-    rml:reference "publicationdate";
-    rr:termType rr:Literal.
-map:om_012 a rr:ObjectMap;
-    rml:reference "type";
-    rr:termType rr:Literal.
-map:om_013 a rr:ObjectMap;
-    rml:reference "country/label";
-    rr:termType rr:Literal.
-map:om_014 a rr:ObjectMap;
-    rml:reference "instance/license";
-    rr:termType rr:Literal.
-map:om_015 a rr:ObjectMap;
-    rml:reference "publisher";
-    rr:termType rr:Literal.
-map:om_016 a rr:ObjectMap;
-    rml:reference "source";
-    rr:termType rr:Literal.
-map:om_017 a rr:ObjectMap;
-    rr:template "https://w3id.org/okn/os/i/idType/{pid/value}";
-    rr:termType rr:IRI.
-map:om_018 a rr:ObjectMap;
-    rr:template "https://w3id.org/okn/os/i/author/{author/fullname}";
-    rr:termType rr:IRI.
-map:om_019 a rr:ObjectMap;
-    rr:parentTriplesMap map:map_idTypeOpenAire_000;
-    rr:joinCondition map:jc_000.
-map:om_020 a rr:ObjectMap;
-    rr:constant "https://w3id.org/okn/os/o/idType";
-    rr:termType rr:IRI.
-map:om_021 a rr:ObjectMap;
-    rr:constant "OpenAire";
-    rr:termType rr:Literal.
-map:om_022 a rr:ObjectMap;
-    rml:reference "id";
-    rr:termType rr:Literal.
-map:om_023 a rr:ObjectMap;
-    rr:constant "https://w3id.org/okn/os/o/idType";
-    rr:termType rr:IRI.
-map:om_024 a rr:ObjectMap;
-    rml:reference "scheme";
-    rr:termType rr:Literal.
-map:om_025 a rr:ObjectMap;
-    rml:reference "value";
-    rr:termType rr:Literal.
-map:pm_000 a rr:PredicateMap;
-    rr:constant rdf:type.
-map:pm_001 a rr:PredicateMap;
-    rr:constant <https://w3id.org/okn/os/o/fullname>.
-map:pm_002 a rr:PredicateMap;
-    rr:constant <https://w3id.org/okn/os/o/name>.
-map:pm_003 a rr:PredicateMap;
-    rr:constant <https://w3id.org/okn/os/o/surname>.
-map:pm_004 a rr:PredicateMap;
-    rr:template "https://w3id.org/okn/os/o/{pid.id.scheme}ID".
-map:pm_005 a rr:PredicateMap;
-    rr:constant rdf:type.
-map:pm_006 a rr:PredicateMap;
-    rr:constant <https://w3id.org/okn/os/o/title>.
-map:pm_007 a rr:PredicateMap;
-    rr:constant <https://w3id.org/okn/os/o/subtitle>.
-map:pm_008 a rr:PredicateMap;
-    rr:constant <https://w3id.org/okn/os/o/description>.
-map:pm_009 a rr:PredicateMap;
-    rr:constant <https://w3id.org/okn/os/o/language>.
-map:pm_010 a rr:PredicateMap;
-    rr:constant <https://w3id.org/okn/os/o/format>.
-map:pm_011 a rr:PredicateMap;
-    rr:constant <https://w3id.org/okn/os/o/publicationDate>.
-map:pm_012 a rr:PredicateMap;
-    rr:constant <https://w3id.org/okn/os/o/type>.
-map:pm_013 a rr:PredicateMap;
-    rr:constant <https://w3id.org/okn/os/o/country>.
-map:pm_014 a rr:PredicateMap;
-    rr:constant <https://w3id.org/okn/os/o/license>.
-map:pm_015 a rr:PredicateMap;
-    rr:constant <https://w3id.org/okn/os/o/publisher>.
-map:pm_016 a rr:PredicateMap;
-    rr:constant <https://w3id.org/okn/os/o/source>.
-map:pm_017 a rr:PredicateMap;
-    rr:constant <https://w3id.org/okn/os/o/has_id>.
-map:pm_018 a rr:PredicateMap;
-    rr:constant <https://w3id.org/okn/os/o/has_id>.
-map:pm_019 a rr:PredicateMap;
-    rr:constant <https://w3id.org/okn/os/o/has_id>.
-map:pm_020 a rr:PredicateMap;
-    rr:constant rdf:type.
-map:pm_021 a rr:PredicateMap;
-    rr:constant <https://w3id.org/okn/os/o/source>.
-map:pm_022 a rr:PredicateMap;
-    rr:constant <https://w3id.org/okn/os/o/identifier>.
-map:pm_023 a rr:PredicateMap;
-    rr:constant rdf:type.
-map:pm_024 a rr:PredicateMap;
-    rr:constant <https://w3id.org/okn/os/o/source>.
-map:pm_025 a rr:PredicateMap;
-    rr:constant <https://w3id.org/okn/os/o/identifier>.
-map:pom_000 a rr:PredicateObjectMap;
-    rr:predicateMap map:pm_000;
-    rr:objectMap map:om_000.
-map:pom_001 a rr:PredicateObjectMap;
-    rr:predicateMap map:pm_001;
-    rr:objectMap map:om_001.
-map:pom_002 a rr:PredicateObjectMap;
-    rr:predicateMap map:pm_002;
-    rr:objectMap map:om_002.
-map:pom_003 a rr:PredicateObjectMap;
-    rr:predicateMap map:pm_003;
-    rr:objectMap map:om_003.
-map:pom_004 a rr:PredicateObjectMap;
-    rr:predicateMap map:pm_004;
-    rr:objectMap map:om_004.
-map:pom_005 a rr:PredicateObjectMap;
-    rr:predicateMap map:pm_005;
-    rr:objectMap map:om_005.
-map:pom_006 a rr:PredicateObjectMap;
-    rr:predicateMap map:pm_006;
-    rr:objectMap map:om_006.
-map:pom_007 a rr:PredicateObjectMap;
-    rr:predicateMap map:pm_007;
-    rr:objectMap map:om_007.
-map:pom_008 a rr:PredicateObjectMap;
-    rr:predicateMap map:pm_008;
-    rr:objectMap map:om_008.
-map:pom_009 a rr:PredicateObjectMap;
-    rr:predicateMap map:pm_009;
-    rr:objectMap map:om_009.
-map:pom_010 a rr:PredicateObjectMap;
-    rr:predicateMap map:pm_010;
-    rr:objectMap map:om_010.
-map:pom_011 a rr:PredicateObjectMap;
-    rr:predicateMap map:pm_011;
-    rr:objectMap map:om_011.
-map:pom_012 a rr:PredicateObjectMap;
-    rr:predicateMap map:pm_012;
-    rr:objectMap map:om_012.
-map:pom_013 a rr:PredicateObjectMap;
-    rr:predicateMap map:pm_013;
-    rr:objectMap map:om_013.
-map:pom_014 a rr:PredicateObjectMap;
-    rr:predicateMap map:pm_014;
-    rr:objectMap map:om_014.
-map:pom_015 a rr:PredicateObjectMap;
-    rr:predicateMap map:pm_015;
-    rr:objectMap map:om_015.
-map:pom_016 a rr:PredicateObjectMap;
-    rr:predicateMap map:pm_016;
-    rr:objectMap map:om_016.
-map:pom_017 a rr:PredicateObjectMap;
-    rr:predicateMap map:pm_017;
-    rr:objectMap map:om_017.
-map:pom_018 a rr:PredicateObjectMap;
-    rr:predicateMap map:pm_018;
-    rr:objectMap map:om_018.
-map:pom_019 a rr:PredicateObjectMap;
-    rr:predicateMap map:pm_019;
-    rr:objectMap map:om_019.
-map:pom_020 a rr:PredicateObjectMap;
-    rr:predicateMap map:pm_020;
-    rr:objectMap map:om_020.
-map:pom_021 a rr:PredicateObjectMap;
-    rr:predicateMap map:pm_021;
-    rr:objectMap map:om_021.
-map:pom_022 a rr:PredicateObjectMap;
-    rr:predicateMap map:pm_022;
-    rr:objectMap map:om_022.
-map:pom_023 a rr:PredicateObjectMap;
-    rr:predicateMap map:pm_023;
-    rr:objectMap map:om_023.
-map:pom_024 a rr:PredicateObjectMap;
-    rr:predicateMap map:pm_024;
-    rr:objectMap map:om_024.
-map:pom_025 a rr:PredicateObjectMap;
-    rr:predicateMap map:pm_025;
-    rr:objectMap map:om_025.
-map:rules_000 a <http://rdfs.org/ns/void#Dataset>;
-    <http://rdfs.org/ns/void#exampleResource> map:map_Author_000, map:map_Paper_000, map:map_idTypeOpenAire_000, map:map_idTypePaperResource_000.
-map:s_000 a rr:SubjectMap;
-    rr:template "https://w3id.org/okn/os/i/author/{fullname}".
-map:s_001 a rr:SubjectMap;
-    rr:template "https://w3id.org/okn/os/i/paper/{id}".
-map:s_002 a rr:SubjectMap;
-    rr:template "https://w3id.org/okn/os/i/idType/{id}".
-map:s_003 a rr:SubjectMap;
-    rr:template "https://w3id.org/okn/os/i/idType/{value}".
-map:source_000 a rml:LogicalSource;
-    rdfs:label "main-source";
-    rml:source "data.xml";
-    rml:iterator "/*";
-    rml:referenceFormulation ql:XPath.
-map:source_001 a rml:LogicalSource;
-    rdfs:label "author-source";
-    rml:source "data.xml";
-    rml:iterator "author";
-    rml:referenceFormulation ql:XPath.
-map:source_002 a rml:LogicalSource;
-    rdfs:label "pid-source";
-    rml:source "data.xml";
-    rml:iterator "pid";
-    rml:referenceFormulation ql:XPath.
+@prefix rr: <http://www.w3.org/ns/r2rml#>.
+@prefix rml: <http://w3id.org/rml/>.
+@prefix rdf: <http://www.w3.org/1999/02/22-rdf-syntax-ns#>.
+@prefix rdfs: <http://www.w3.org/2000/01/rdf-schema#>.
+@prefix ql: <http://semweb.mmlab.be/ns/ql#>.
+@prefix map: <http://mapping.example.com/>.
+
+map:jc_000 rml:child "id";
+    rml:parent "id".
+map:language_000 rml:reference "language.code".
+map:map_Author_000 rml:logicalSource map:source_001;
+    a rml:TriplesMap;
+    rdfs:label "Author";
+    rml:subjectMap map:s_000;
+    rml:predicateObjectMap map:pom_000, map:pom_001, map:pom_002, map:pom_003, map:pom_004.
+map:map_idTypeOpenAire_000 rml:logicalSource map:source_002;
+    a rml:TriplesMap;
+    rdfs:label "idTypeOpenAire";
+    rml:subjectMap map:s_002;
+    rml:predicateObjectMap map:pom_020, map:pom_021, map:pom_022.
+map:map_idTypePaperResource_000 rml:logicalSource map:source_002;
+    a rml:TriplesMap;
+    rdfs:label "idTypePaperResource";
+    rml:subjectMap map:s_003;
+    rml:predicateObjectMap map:pom_023, map:pom_024, map:pom_025.
+map:map_Paper_000 rml:logicalSource map:source_000;
+    a rml:TriplesMap;
+    rdfs:label "Paper";
+    rml:subjectMap map:s_001;
+    rml:predicateObjectMap map:pom_005, map:pom_006, map:pom_007, map:pom_008, map:pom_009, map:pom_010, map:pom_011, map:pom_012, map:pom_013, map:pom_014, map:pom_015, map:pom_016, map:pom_017, map:pom_018, map:pom_019.
+map:om_000 a rml:ObjectMap;
+    rml:constant "https://w3id.org/okn/os/o/Author";
+    rml:termType rml:IRI.
+map:om_001 a rml:ObjectMap;
+    rml:reference "fullname";
+    rml:termType rml:Literal.
+map:om_002 a rml:ObjectMap;
+    rml:reference "name";
+    rml:termType rml:Literal.
+map:om_003 a rml:ObjectMap;
+    rml:reference "surname";
+    rml:termType rml:Literal.
+map:om_004 a rml:ObjectMap;
+    rml:reference "pid.id.value";
+    rml:termType rml:Literal.
+map:om_005 a rml:ObjectMap;
+    rml:constant "https://w3id.org/okn/os/o/Paper";
+    rml:termType rml:IRI.
+map:om_006 a rml:ObjectMap;
+    rml:reference "maintitle";
+    rml:termType rml:Literal.
+map:om_007 a rml:ObjectMap;
+    rml:reference "subtitle";
+    rml:termType rml:Literal.
+map:om_008 a rml:ObjectMap;
+    rml:reference "description";
+    rml:termType rml:Literal;
+    rml:languageMap map:language_000.
+map:om_009 a rml:ObjectMap;
+    rml:reference "language.label";
+    rml:termType rml:Literal.
+map:om_010 a rml:ObjectMap;
+    rml:reference "format";
+    rml:termType rml:Literal.
+map:om_011 a rml:ObjectMap;
+    rml:reference "publicationdate";
+    rml:termType rml:Literal.
+map:om_012 a rml:ObjectMap;
+    rml:reference "type";
+    rml:termType rml:Literal.
+map:om_013 a rml:ObjectMap;
+    rml:reference "country/label";
+    rml:termType rml:Literal.
+map:om_014 a rml:ObjectMap;
+    rml:reference "instance/license";
+    rml:termType rml:Literal.
+map:om_015 a rml:ObjectMap;
+    rml:reference "publisher";
+    rml:termType rml:Literal.
+map:om_016 a rml:ObjectMap;
+    rml:reference "source";
+    rml:termType rml:Literal.
+map:om_017 a rml:ObjectMap;
+    rml:template "https://w3id.org/okn/os/i/idType/{pid/value}";
+    rml:termType rml:IRI.
+map:om_018 a rml:ObjectMap;
+    rml:template "https://w3id.org/okn/os/i/author/{author/fullname}";
+    rml:termType rml:IRI.
+map:om_019 a rml:ObjectMap;
+    rml:parentTriplesMap map:map_idTypeOpenAire_000;
+    rml:joinCondition map:jc_000.
+map:om_020 a rml:ObjectMap;
+    rml:constant "https://w3id.org/okn/os/o/idType";
+    rml:termType rml:IRI.
+map:om_021 a rml:ObjectMap;
+    rml:constant "OpenAire";
+    rml:termType rml:Literal.
+map:om_022 a rml:ObjectMap;
+    rml:reference "id";
+    rml:termType rml:Literal.
+map:om_023 a rml:ObjectMap;
+    rml:constant "https://w3id.org/okn/os/o/idType";
+    rml:termType rml:IRI.
+map:om_024 a rml:ObjectMap;
+    rml:reference "scheme";
+    rml:termType rml:Literal.
+map:om_025 a rml:ObjectMap;
+    rml:reference "value";
+    rml:termType rml:Literal.
+map:pm_000 a rml:PredicateMap;
+    rml:constant rdf:type.
+map:pm_001 a rml:PredicateMap;
+    rml:constant <https://w3id.org/okn/os/o/fullname>.
+map:pm_002 a rml:PredicateMap;
+    rml:constant <https://w3id.org/okn/os/o/name>.
+map:pm_003 a rml:PredicateMap;
+    rml:constant <https://w3id.org/okn/os/o/surname>.
+map:pm_004 a rml:PredicateMap;
+    rml:template "https://w3id.org/okn/os/o/{pid.id.scheme}ID".
+map:pm_005 a rml:PredicateMap;
+    rml:constant rdf:type.
+map:pm_006 a rml:PredicateMap;
+    rml:constant <https://w3id.org/okn/os/o/title>.
+map:pm_007 a rml:PredicateMap;
+    rml:constant <https://w3id.org/okn/os/o/subtitle>.
+map:pm_008 a rml:PredicateMap;
+    rml:constant <https://w3id.org/okn/os/o/description>.
+map:pm_009 a rml:PredicateMap;
+    rml:constant <https://w3id.org/okn/os/o/language>.
+map:pm_010 a rml:PredicateMap;
+    rml:constant <https://w3id.org/okn/os/o/format>.
+map:pm_011 a rml:PredicateMap;
+    rml:constant <https://w3id.org/okn/os/o/publicationDate>.
+map:pm_012 a rml:PredicateMap;
+    rml:constant <https://w3id.org/okn/os/o/type>.
+map:pm_013 a rml:PredicateMap;
+    rml:constant <https://w3id.org/okn/os/o/country>.
+map:pm_014 a rml:PredicateMap;
+    rml:constant <https://w3id.org/okn/os/o/license>.
+map:pm_015 a rml:PredicateMap;
+    rml:constant <https://w3id.org/okn/os/o/publisher>.
+map:pm_016 a rml:PredicateMap;
+    rml:constant <https://w3id.org/okn/os/o/source>.
+map:pm_017 a rml:PredicateMap;
+    rml:constant <https://w3id.org/okn/os/o/has_id>.
+map:pm_018 a rml:PredicateMap;
+    rml:constant <https://w3id.org/okn/os/o/has_id>.
+map:pm_019 a rml:PredicateMap;
+    rml:constant <https://w3id.org/okn/os/o/has_id>.
+map:pm_020 a rml:PredicateMap;
+    rml:constant rdf:type.
+map:pm_021 a rml:PredicateMap;
+    rml:constant <https://w3id.org/okn/os/o/source>.
+map:pm_022 a rml:PredicateMap;
+    rml:constant <https://w3id.org/okn/os/o/identifier>.
+map:pm_023 a rml:PredicateMap;
+    rml:constant rdf:type.
+map:pm_024 a rml:PredicateMap;
+    rml:constant <https://w3id.org/okn/os/o/source>.
+map:pm_025 a rml:PredicateMap;
+    rml:constant <https://w3id.org/okn/os/o/identifier>.
+map:pom_000 a rml:PredicateObjectMap;
+    rml:predicateMap map:pm_000;
+    rml:objectMap map:om_000.
+map:pom_001 a rml:PredicateObjectMap;
+    rml:predicateMap map:pm_001;
+    rml:objectMap map:om_001.
+map:pom_002 a rml:PredicateObjectMap;
+    rml:predicateMap map:pm_002;
+    rml:objectMap map:om_002.
+map:pom_003 a rml:PredicateObjectMap;
+    rml:predicateMap map:pm_003;
+    rml:objectMap map:om_003.
+map:pom_004 a rml:PredicateObjectMap;
+    rml:predicateMap map:pm_004;
+    rml:objectMap map:om_004.
+map:pom_005 a rml:PredicateObjectMap;
+    rml:predicateMap map:pm_005;
+    rml:objectMap map:om_005.
+map:pom_006 a rml:PredicateObjectMap;
+    rml:predicateMap map:pm_006;
+    rml:objectMap map:om_006.
+map:pom_007 a rml:PredicateObjectMap;
+    rml:predicateMap map:pm_007;
+    rml:objectMap map:om_007.
+map:pom_008 a rml:PredicateObjectMap;
+    rml:predicateMap map:pm_008;
+    rml:objectMap map:om_008.
+map:pom_009 a rml:PredicateObjectMap;
+    rml:predicateMap map:pm_009;
+    rml:objectMap map:om_009.
+map:pom_010 a rml:PredicateObjectMap;
+    rml:predicateMap map:pm_010;
+    rml:objectMap map:om_010.
+map:pom_011 a rml:PredicateObjectMap;
+    rml:predicateMap map:pm_011;
+    rml:objectMap map:om_011.
+map:pom_012 a rml:PredicateObjectMap;
+    rml:predicateMap map:pm_012;
+    rml:objectMap map:om_012.
+map:pom_013 a rml:PredicateObjectMap;
+    rml:predicateMap map:pm_013;
+    rml:objectMap map:om_013.
+map:pom_014 a rml:PredicateObjectMap;
+    rml:predicateMap map:pm_014;
+    rml:objectMap map:om_014.
+map:pom_015 a rml:PredicateObjectMap;
+    rml:predicateMap map:pm_015;
+    rml:objectMap map:om_015.
+map:pom_016 a rml:PredicateObjectMap;
+    rml:predicateMap map:pm_016;
+    rml:objectMap map:om_016.
+map:pom_017 a rml:PredicateObjectMap;
+    rml:predicateMap map:pm_017;
+    rml:objectMap map:om_017.
+map:pom_018 a rml:PredicateObjectMap;
+    rml:predicateMap map:pm_018;
+    rml:objectMap map:om_018.
+map:pom_019 a rml:PredicateObjectMap;
+    rml:predicateMap map:pm_019;
+    rml:objectMap map:om_019.
+map:pom_020 a rml:PredicateObjectMap;
+    rml:predicateMap map:pm_020;
+    rml:objectMap map:om_020.
+map:pom_021 a rml:PredicateObjectMap;
+    rml:predicateMap map:pm_021;
+    rml:objectMap map:om_021.
+map:pom_022 a rml:PredicateObjectMap;
+    rml:predicateMap map:pm_022;
+    rml:objectMap map:om_022.
+map:pom_023 a rml:PredicateObjectMap;
+    rml:predicateMap map:pm_023;
+    rml:objectMap map:om_023.
+map:pom_024 a rml:PredicateObjectMap;
+    rml:predicateMap map:pm_024;
+    rml:objectMap map:om_024.
+map:pom_025 a rml:PredicateObjectMap;
+    rml:predicateMap map:pm_025;
+    rml:objectMap map:om_025.
+map:rules_000 a <http://rdfs.org/ns/void#Dataset>;
+    <http://rdfs.org/ns/void#exampleResource> map:map_Author_000, map:map_Paper_000, map:map_idTypeOpenAire_000, map:map_idTypePaperResource_000.
+map:s_000 a rml:SubjectMap;
+    rml:template "https://w3id.org/okn/os/i/author/{fullname}".
+map:s_001 a rml:SubjectMap;
+    rml:template "https://w3id.org/okn/os/i/paper/{id}".
+map:s_002 a rml:SubjectMap;
+    rml:template "https://w3id.org/okn/os/i/idType/{id}".
+map:s_003 a rml:SubjectMap;
+    rml:template "https://w3id.org/okn/os/i/idType/{value}".
+map:source_000 a rml:LogicalSource;
+    rdfs:label "main-source";
+    rml:source "test/rml-core/xml/complex/data.xml";
+    rml:iterator "/*";
+    rml:referenceFormulation rml:XPath.
+map:source_001 a rml:LogicalSource;
+    rdfs:label "author-source";
+    rml:source "test/rml-core/xml/complex/data.xml";
+    rml:iterator "author";
+    rml:referenceFormulation rml:XPath.
+map:source_002 a rml:LogicalSource;
+    rdfs:label "pid-source";
+    rml:source "test/rml-core/xml/complex/data.xml";
+    rml:iterator "pid";
+    rml:referenceFormulation rml:XPath.
```

### Comparing `morph_kgc-2.6.4/src/morph_kgc/__main__.py` & `morph_kgc-2.7.0/src/morph_kgc/__main__.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 
 import multiprocessing as mp
 
 from itertools import repeat
 
 from .args_parser import load_config_from_command_line
 from .materializer import _materialize_mapping_group_to_file
+from .materializer import _materialize_mapping_group_to_kafka
 from .data_source.relational_database import setup_oracle
 from .utils import get_delta_time
 from .mapping.mapping_parser import retrieve_mappings
 from .constants import RML_TRIPLES_MAP_CLASS
 from .utils import prepare_output_files
 
 
@@ -38,17 +39,24 @@
 
     start_time = time.time()
     num_triples = 0
     if config.is_multiprocessing_enabled():
         logging.debug(f'Parallelizing with {config.get_number_of_processes()} cores.')
 
         pool = mp.Pool(config.get_number_of_processes())
-        num_triples = sum(pool.starmap(_materialize_mapping_group_to_file,
-                                       zip(mapping_groups, repeat(rml_df), repeat(fnml_df), repeat(config))))
+        if not config.get_output_kafka_server():
+            num_triples = sum(pool.starmap(_materialize_mapping_group_to_file,
+                                           zip(mapping_groups, repeat(rml_df), repeat(fnml_df), repeat(config))))
+        else:
+            num_triples = sum(pool.starmap(_materialize_mapping_group_to_kafka,
+                                           zip(mapping_groups, repeat(rml_df), repeat(fnml_df), repeat(config))))
         pool.close()
         pool.join()
     else:
         for mapping_group in mapping_groups:
-            num_triples += _materialize_mapping_group_to_file(mapping_group, rml_df, fnml_df, config)
+            if not config.get_output_kafka_server():
+                num_triples += _materialize_mapping_group_to_file(mapping_group, rml_df, fnml_df, config)
+            else:
+                num_triples += _materialize_mapping_group_to_kafka(mapping_group, rml_df, fnml_df, config)
 
     logging.info(f'Number of triples generated in total: {num_triples}.')
     logging.info(f'Materialization finished in {get_delta_time(start_time)} seconds.')
```

### Comparing `morph_kgc-2.6.4/src/morph_kgc/args_parser.py` & `morph_kgc-2.7.0/src/morph_kgc/args_parser.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,23 +26,23 @@
 def _parse_arguments():
     """
     Parses command line arguments.
     """
 
     parser = argparse.ArgumentParser(
         description='Generate Knowledge Graphs from Heterogeneous Data Sources.',
-        epilog="Copyright © 2020-2023 Julián Arenas-Guerrero",
+        epilog="Copyright © 2020 Julián Arenas-Guerrero",
         allow_abbrev=False,
         prog='python3 -m morph_kgc',
         argument_default=argparse.SUPPRESS
     )
 
     parser.add_argument('config', type=_existing_file_path, help='path to the configuration file')
     parser.add_argument('-v', '--version', action='version',
-                        version=f'Morph-KGC {__version__} | Copyright © 2020-2023 Julián Arenas-Guerrero')
+                        version=f'Morph-KGC {__version__} | Copyright © 2020 Julián Arenas-Guerrero')
 
     return parser.parse_args()
 
 
 def _parse_config(config):
     """
     Parses the config file. Logger is configured.
```

### Comparing `morph_kgc-2.6.4/src/morph_kgc/config.py` & `morph_kgc-2.7.0/src/morph_kgc/config.py`

 * *Files 3% similar despite different names*

```diff
@@ -56,14 +56,19 @@
 ##############################################################################
 
 MAPPINGS = 'mappings'
 FILE_PATH = 'file_path'
 DATABASE_URL = 'db_url'
 CONNECT_ARGS = 'connect_args'
 
+##############################################################################
+##########################  KAFKA PARAMETERS  ################################
+##############################################################################
+OUTPUT_KAFKA_SERVER = 'output_kafka_server'
+OUTPUT_KAFKA_TOPIC = 'output_kafka_topic'
 
 ##############################################################################
 ########################   ARGUMENTS DEFAULT VALUES   ########################
 ##############################################################################
 
 DEFAULT_OUTPUT_FILE = 'knowledge-graph'
 DEFAULT_OUTPUT_DIR = ''
@@ -72,14 +77,16 @@
 DEFAULT_LOGGING_FILE = ''
 DEFAULT_LOGGING_LEVEL = 'INFO'
 DEFAULT_INFER_SQL_DATATYPES = 'no'
 DEFAULT_NUMBER_OF_PROCESSES = 2 * mp.cpu_count()
 DEFAULT_NA_VALUES = ',nan' # ',#N/A,N/A,#N/A N/A,n/a,NA,<NA>,#NA,NULL,null,NaN,nan,None'
 DEFAULT_ONLY_PRINTABLE_CHARS = 'no'
 DEFAULT_UDFS = ''
+DEFAULT_OUTPUT_KAFKA_SERVER = ''
+DEFAULT_OUTPUT_KAFKA_TOPIC = ''
 
 # ORACLE
 DEFAULT_ORACLE_CLIENT_LIB_DIR = ''
 DEFAULT_ORACLE_CLIENT_CONFIG_DIR = ''
 
 # DEVELOPMENT OPTIONS
 DEFAULT_READ_PARSED_MAPPINGS_PATH = ''
@@ -98,17 +105,19 @@
             READ_PARSED_MAPPINGS_PATH: DEFAULT_READ_PARSED_MAPPINGS_PATH,
             WRITE_PARSED_MAPPINGS_PATH: DEFAULT_WRITE_PARSED_MAPPINGS_PATH,
             MAPPING_PARTITIONING: PARTIAL_AGGREGATIONS_PARTITIONING,
             LOGGING_FILE: DEFAULT_LOGGING_FILE,
             ORACLE_CLIENT_LIB_DIR: DEFAULT_ORACLE_CLIENT_LIB_DIR,
             ORACLE_CLIENT_CONFIG_DIR: DEFAULT_ORACLE_CLIENT_LIB_DIR,
             UDFS: DEFAULT_UDFS,
+            OUTPUT_KAFKA_SERVER: DEFAULT_OUTPUT_KAFKA_SERVER,
+            OUTPUT_KAFKA_TOPIC: DEFAULT_OUTPUT_KAFKA_TOPIC,
         }
 
-# input parameters that are to be replaced with the default vale if they are empty
+# input parameters that are to be replaced with the default value if they are empty
 CONFIGURATION_OPTIONS_EMPTY_NON_VALID = {
             OUTPUT_DIR: DEFAULT_OUTPUT_DIR,
             OUTPUT_FORMAT: DEFAULT_OUTPUT_FORMAT,
             ONLY_PRINTABLE_CHARS: DEFAULT_ONLY_PRINTABLE_CHARS,
             INFER_SQL_DATATYPES: DEFAULT_INFER_SQL_DATATYPES,
             LOGGING_LEVEL: DEFAULT_LOGGING_LEVEL,
             NUMBER_OF_PROCESSES: DEFAULT_NUMBER_OF_PROCESSES
@@ -283,14 +292,20 @@
         else:
             # neither output_file was specified nor mapping partition are used. Use default output_file.
             file_name = OUTPUT_FILE
             file_path = Path(file_name).with_suffix(file_extension)
 
         return file_path.as_posix()
 
+    def get_output_kafka_server(self):
+        return self.get(self.configuration_section, OUTPUT_KAFKA_SERVER)
+
+    def get_output_kafka_topic(self):
+        return self.get(self.configuration_section, OUTPUT_KAFKA_TOPIC)
+    
     def set_mapping_partitioning(self, mapping_partitioning):
         self.set(self.configuration_section, MAPPING_PARTITIONING, mapping_partitioning.upper())
 
     def set_logging_level(self, logging_level):
         self.set(self.configuration_section, LOGGING_LEVEL, logging_level)
 
     def set_output_format(self, output_format):
```

### Comparing `morph_kgc-2.6.4/src/morph_kgc/constants.py` & `morph_kgc-2.7.0/src/morph_kgc/constants.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/src/morph_kgc/materializer.py` & `morph_kgc-2.7.0/src/morph_kgc/materializer.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 def _preprocess_data(data, rml_rule, references, config):
     # deal with ORACLE
     if rml_rule['source_type'] == RDB:
         if config.get_database_url(rml_rule['source_name']).lower().startswith(ORACLE.lower()):
             data = normalize_oracle_identifier_casing(data, references)
 
     # TODO: can this be removed?
-    data = data.applymap(str)
+    data = data.map(str)
 
     data = remove_null_values_from_dataframe(data, config, references)
     data = data.convert_dtypes(convert_boolean=False)
 
     # data to str
     data = data.astype(str)
 
@@ -408,31 +408,44 @@
         data['triple'] = data['triple'] + ' ' + data['graph']
 
     data = data.drop(columns=['subject', 'predicate', 'object'], errors='ignore')
 
     return data
 
 
-def _materialize_mapping_group_to_file(mapping_group_df, rml_df, fnml_df, config):
+def _materialize_mapping_group_to_set(mapping_group_df, rml_df, fnml_df, config, python_source=None):
+    triples = set()
+    for i, rml_rule in mapping_group_df.iterrows():
+        data = _materialize_rml_rule(rml_rule, rml_df, fnml_df, config, python_source=python_source)
+        triples.update(set(data['triple']))
+
+    return triples
+
 
+def _materialize_mapping_group_to_file(mapping_group_df, rml_df, fnml_df, config):
     triples = set()
     for i, rml_rule in mapping_group_df.iterrows():
         start_time = time.time()
         data = _materialize_rml_rule(rml_rule, rml_df, fnml_df, config)
         triples.update(set(data['triple']))
 
         logging.debug(f"{len(triples)} triples generated for mapping rule `{rml_rule['triples_map_id']}` "
                       f"in {get_delta_time(start_time)} seconds.")
 
     triples_to_file(triples, config, mapping_group_df.iloc[0]['mapping_partition'])
 
     return len(triples)
 
 
-def _materialize_mapping_group_to_set(mapping_group_df, rml_df, fnml_df, config, python_source=None):
-
+def _materialize_mapping_group_to_kafka(mapping_group_df, rml_df, fnml_df, config, python_source=None):
     triples = set()
     for i, rml_rule in mapping_group_df.iterrows():
+        start_time = time.time()
         data = _materialize_rml_rule(rml_rule, rml_df, fnml_df, config, python_source=python_source)
         triples.update(set(data['triple']))
 
-    return triples
+        logging.debug(f"{len(triples)} triples generated for mapping rule `{rml_rule['triples_map_id']}` "
+                      f"in {get_delta_time(start_time)} seconds.")
+        
+    triples_to_kafka(triples, config)
+
+    return len(triples)
```

### Comparing `morph_kgc-2.6.4/src/morph_kgc/utils.py` & `morph_kgc-2.7.0/src/morph_kgc/utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,17 +5,18 @@
 __maintainer__ = "Julián Arenas-Guerrero"
 __email__ = "arenas.guerrero.julian@outlook.com"
 
 
 import re
 import os
 import logging
+import sys
+
 import rdflib
 import time
-import numpy as np
 import pandas as pd
 import multiprocessing as mp
 
 from itertools import product
 from .constants import AUXILIAR_UNIQUE_REPLACING_STRING, RML_EXECUTION, RML_TEMPLATE, RML_REFERENCE
 
 
@@ -123,29 +124,14 @@
             references.extend([parameter['value_map_value']])
         elif parameter['value_map_type'] == RML_EXECUTION:
             references.extend(get_references_in_fnml_execution(fnml_df, parameter['value_map_value']))
 
     return references
 
 
-def triples_to_file(triples, config, mapping_group=None):
-    """
-    Writes triples to file.
-    """
-
-    lock = mp.Lock()    # necessary for issue #65
-    with lock:
-        f = open(config.get_output_file_path(mapping_group), 'a', encoding='utf-8')
-        for triple in triples:
-            f.write(f'{triple} .\n')
-        f.flush()
-        os.fsync(f.fileno())
-        f.close()
-
-
 def remove_non_printable_characters(string):
     """
     Eliminates from the input string all the characters that are not printable.
     """
 
     return ''.join(char for char in string if char.isprintable())
 
@@ -248,17 +234,17 @@
     return dataframe
 
 
 def remove_null_values_from_dataframe(data, config, references, column=None):
     if config.get_na_values():  # if there is some NULL values to replace
         if column:
             # only replace nulls in the given column
-            data[column] = data[column].replace(config.get_na_values(), np.NaN)
+            data[column] = data[column].replace(config.get_na_values(), None)
         else:
-            data = data.replace(config.get_na_values(), np.NaN)
+            data = data.replace(config.get_na_values(), None)
         data = data.dropna(axis=0, how='any', subset=references)
 
     return data
 
 
 def normalize_hierarchical_data(data):
     """
@@ -271,7 +257,55 @@
         for i in product(*values):
             yield (dict(zip(keys, i)))
     elif isinstance(data, list):
         for i in data:
             yield from normalize_hierarchical_data(i)
     else:
         yield data
+
+
+def triples_to_file(triples, config, mapping_group=None):
+    """
+    Writes triples to file.
+    """
+
+    lock = mp.Lock()    # necessary for issue #65
+    with lock:
+        f = open(config.get_output_file_path(mapping_group), 'a', encoding='utf-8')
+        for triple in triples:
+            f.write(f'{triple} .\n')
+        f.flush()
+        os.fsync(f.fileno())
+        f.close()
+
+
+def triples_to_kafka(triples, config):
+    """
+    Writes triples to Kafka.
+    """
+    from kafka import KafkaProducer
+
+    kafka_producer = None
+    output_kafka_server = config.get_output_kafka_server()
+    output_kafka_topic = config.get_output_kafka_topic()
+
+    if not output_kafka_server or not output_kafka_topic:
+        logging.error('Output Kafka server or topic is empty.')
+        sys.exit()
+    try:
+        kafka_producer = KafkaProducer(bootstrap_servers=output_kafka_server)
+
+        if triples:
+            rdf_ntriples = '.\n'.join(triples)
+            rdf_ntriples += '.'
+
+            # send the triples to Kafka
+            kafka_producer.send(output_kafka_topic, value=rdf_ntriples.encode('utf-8'))
+
+        return len(triples)
+    except Exception as e:
+            logging.error(f'Error during materialization or Kafka publishing: {e}')
+            return f'Error: {e}'
+    finally:
+        # close the Kafka producer
+        if kafka_producer:
+            kafka_producer.close()
```

### Comparing `morph_kgc-2.6.4/src/morph_kgc/data_source/data_file.py` & `morph_kgc-2.7.0/src/morph_kgc/data_source/data_file.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 __maintainer__ = "Julián Arenas-Guerrero"
 __email__ = "arenas.guerrero.julian@outlook.com"
 
 
 import json
 import duckdb
 import pandas as pd
-import numpy as np
 import elementpath
 import xml.etree.ElementTree as et
 import urllib.request
 
 from jsonpath import JSONPath
 from elementpath.xpath3 import XPath3Parser
 from io import BytesIO
@@ -152,15 +151,16 @@
 
     jsonpath_result = JSONPath(jsonpath_expression).parse(json_data)
     # normalize and remove nulls
     json_df = pd.json_normalize([json_object for json_object in normalize_hierarchical_data(jsonpath_result) if None not in json_object.values()])
 
     # add columns with null values for those references in the mapping rule that are not present in the data file
     missing_references_in_df = list(set(references).difference(set(json_df.columns)))
-    json_df[missing_references_in_df] = np.nan
+    json_df[missing_references_in_df] = None
+    json_df.dropna(axis=0, how='any', inplace=True)
 
     return json_df
 
 
 def _read_xml(rml_rule, references):
     if rml_rule['logical_source_value'].startswith('http'):
         with urllib.request.urlopen(rml_rule['logical_source_value']) as xml_url:
@@ -216,14 +216,14 @@
     # with XPath 3.1 the above could be achieved using just an XPath expression by including the references in it
     # for instance, the XPath expression: /root/[id,creator/name] obtaining for example ["2479", ["Julián", "Jhon"]]
 
     xml_df = pd.DataFrame.from_records(data_records, columns=references)
 
     # add columns with null values for those references in the mapping rule that are not present in the data file
     missing_references_in_df = list(set(references).difference(set(xml_df.columns)))
-    xml_df[missing_references_in_df] = np.nan
+    xml_df[missing_references_in_df] = None
     xml_df.dropna(axis=0, how='any', inplace=True)
 
     for reference in references:
         xml_df = xml_df.explode(reference)
 
     return xml_df
```

### Comparing `morph_kgc-2.6.4/src/morph_kgc/data_source/python_data.py` & `morph_kgc-2.7.0/src/morph_kgc/data_source/python_data.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/src/morph_kgc/data_source/relational_database.py` & `morph_kgc-2.7.0/src/morph_kgc/data_source/relational_database.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,17 +5,14 @@
 __maintainer__ = "Julián Arenas-Guerrero"
 __email__ = "arenas.guerrero.julian@outlook.com"
 
 
 import logging
 import pandas as pd
 
-from sqlalchemy import create_engine
-from sqlalchemy.pool import NullPool
-
 from ..constants import *
 
 
 # PostgresSQL data types: https://www.postgresql.org/docs/14/datatype.html
 # Oracle data types: https://docs.oracle.com/cd/A58617_01/server.804/a58241/ch5.htm
 # MySQL data types: https://dev.mysql.com/doc/refman/8.0/en/data-types.html
 SQL_RDF_DATATYPE = {
@@ -82,14 +79,17 @@
         # replace backticks with double quotes
         dialect_sql_query = sql_query.replace('`', '"')
 
     return dialect_sql_query
 
 
 def _relational_db_connection(config, source_name):
+    from sqlalchemy import create_engine
+    from sqlalchemy.pool import NullPool
+
     connect_args = eval(config.get_connect_args(source_name)) if config.has_connect_args(source_name) else {}
 
     db_connection = create_engine(config.get_database_url(source_name), connect_args=connect_args, poolclass=NullPool)
     db_dialect = db_connection.dialect.name.upper()
 
     return db_connection, db_dialect
```

### Comparing `morph_kgc-2.6.4/src/morph_kgc/fnml/built_in_functions.py` & `morph_kgc-2.7.0/src/morph_kgc/fnml/built_in_functions.py`

 * *Files 2% similar despite different names*

```diff
@@ -139,14 +139,21 @@
     fun_id='http://users.ugent.be/~bjdmeest/function/grel.ttl#toTitleCase',
     string='http://users.ugent.be/~bjdmeest/function/grel.ttl#valueParam')
 def to_title_case(string):
     return string.title()
 
 
 @bif(
+    fun_id='http://users.ugent.be/~bjdmeest/function/grel.ttl#reverse',
+    string='http://users.ugent.be/~bjdmeest/function/grel.ttl#valueParam')
+def reverse(string):
+    return string[::-1]
+
+
+@bif(
     fun_id='http://users.ugent.be/~bjdmeest/function/grel.ttl#string_trim',
     string='http://users.ugent.be/~bjdmeest/function/grel.ttl#valueParam')
 def string_trim(string):
     return string.strip()
 
 
 @bif(
```

### Comparing `morph_kgc-2.6.4/src/morph_kgc/fnml/fnml_executer.py` & `morph_kgc-2.7.0/src/morph_kgc/fnml/fnml_executer.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/src/morph_kgc/mapping/mapping_constants.py` & `morph_kgc-2.7.0/src/morph_kgc/mapping/mapping_constants.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/src/morph_kgc/mapping/mapping_parser.py` & `morph_kgc-2.7.0/src/morph_kgc/mapping/mapping_parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -383,15 +383,15 @@
 
     # subject_map and object_map columns were used to handle join conditions, no longer needed
     rml_df = rml_df.drop(columns=['subject_map', 'object_map'])
 
     # FNML in graph to DataFrame
     fnml_df = pd.DataFrame(fnml_query_results.bindings)
     fnml_df.columns = fnml_df.columns.map(str)
-    fnml_df = fnml_df.applymap(str)
+    fnml_df = fnml_df.map(str)
 
     return rml_df, fnml_df
 
 
 def _is_delimited_identifier(identifier):
     """
     Checks if an identifier is delimited or not.
@@ -478,15 +478,15 @@
 
         self._infer_datatypes()
         self.validate_mappings()
 
         logging.info(f'{len(self.rml_df)} mapping rules retrieved.')
 
         # replace empty strings with NaN
-        self.rml_df = self.rml_df.replace(r'^\s*$', np.nan, regex=True)
+        self.rml_df = self.rml_df.infer_objects(copy=False).replace(r'^\s*$', None, regex=True)
 
         # generate mapping partitions
         mapping_partitioner = MappingPartitioner(self.rml_df, self.config)
         self.rml_df = mapping_partitioner.partition_mappings()
 
         return self.rml_df, self.fnml_df
 
@@ -799,15 +799,15 @@
 
     # TODO: deprecate
     def _remove_self_joins_no_condition(self):
         for i, rml_rule in self.rml_df.iterrows():
             if rml_rule['object_map_type'] == RML_PARENT_TRIPLES_MAP:
                 parent_triples_map_rule = get_rml_rule(self.rml_df, rml_rule['object_map_value'])
                 if rml_rule['logical_source_value'] == parent_triples_map_rule['logical_source_value'] and str(
-                        # str() is to be able to compare np.nan
+                        # str() is to be able to compare None
                         rml_rule['iterator']) == str(parent_triples_map_rule['iterator']):
 
                     remove_join = True
                     # check that all conditions in the join condition have the same references
                     try:
                         join_conditions = eval(rml_rule['object_join_conditions'])
                         for key, join_condition in join_conditions.items():
@@ -817,9 +817,9 @@
                         # eval() has failed because there are no join conditions, the join can be removed
                         remove_join = True
 
                     if remove_join and pd.notna(rml_rule['object_join_conditions']):
                         self.rml_df.at[i, 'object_map_type'] = parent_triples_map_rule.at['subject_map_type']
                         self.rml_df.at[i, 'object_map_value'] = parent_triples_map_rule.at['subject_map_value']
                         self.rml_df.at[i, 'object_termtype'] = parent_triples_map_rule.at['subject_termtype']
-                        self.rml_df.at[i, 'object_join_conditions'] = np.nan
+                        self.rml_df.at[i, 'object_join_conditions'] = None
                         logging.debug(f"Removed self-join from mapping rule `{rml_rule['triples_map_id']}`.")
```

### Comparing `morph_kgc-2.6.4/src/morph_kgc/mapping/mapping_partitioner.py` & `morph_kgc-2.7.0/src/morph_kgc/mapping/mapping_partitioner.py`

 * *Files 0% similar despite different names*

```diff
@@ -175,28 +175,26 @@
             # assign empty partition
             self.rml_df['mapping_partition'] = '0-0-0-0'
         else:
             logging.error('Selected mapping partitioning algorithm is not valid.')
 
         logging.info(f"Mapping partition with {len(set(self.rml_df['mapping_partition']))} groups generated.")
         logging.info('Maximum number of rules within mapping group: '
-                     f"{self.rml_df['mapping_partition'].value_counts()[0]}.")
+                     f"{self.rml_df['mapping_partition'].value_counts().iloc[0]}.")
 
         return self.rml_df
 
     def _generate_maximal_partition(self):
         """
         Generates a mapping partition with the maximum number of mapping groups.
         """
 
         self.rml_df['literal_type'] = self.rml_df['object_language'] + self.rml_df['object_datatype']
         self.rml_df['mapping_partition'] = ''
 
-        rml_df = self.rml_df.copy()
-
         position_orderings = list(permutations(['S', 'P', 'O', 'G']))
 
         if self.config.is_multiprocessing_enabled():
             pool = mp.Pool(self.config.get_number_of_processes())
             mapping_partitions_dfs = pool.starmap(_generate_maximal_partition_for_a_position_ordering,
                                                   zip([self.rml_df.copy()] * len(position_orderings),
                                                       position_orderings))
```

### Comparing `morph_kgc-2.6.4/src/morph_kgc/mapping/yarrrml.py` & `morph_kgc-2.7.0/src/morph_kgc/mapping/yarrrml.py`

 * *Files 1% similar despite different names*

```diff
@@ -82,14 +82,16 @@
                 mappings['predicateobjects'] = mappings.pop(key)
             elif key in ['predicate', 'p']:
                 mappings['predicates'] = mappings.pop(key)
             elif key in ['inversepredicate', 'i']:
                 mappings['inversepredicates'] = mappings.pop(key)
             elif key in ['object', 'o']:
                 mappings['objects'] = mappings.pop(key)
+            elif key in ['graph', 'g']:
+                mappings['graphs'] = mappings.pop(key)
             elif key in ['fn', 'f']:
                 mappings['function'] = mappings.pop(key)
             elif key in ['pms']:
                 mappings['parameters'] = mappings.pop(key)
             elif key in ['pm']:
                 mappings['parameter'] = mappings.pop(key)
             elif key in ['v']:
@@ -250,25 +252,14 @@
     #############################################################################
     ############################ NORMALIZE TRIPLES MAPS #########################
     #############################################################################
 
     for property in ['sources', 'subjects', 'predicateobjects']:
         mappings = _normalize_property_in_mapping(mappings, property)
 
-    # move graphs in subjects to predicateobjects
-    for mapping_key, mapping_value in mappings['mappings'].items():
-        if 'graphs' in mapping_value and 'predicateobjects' in mapping_value:
-            if 'graphs' in mapping_value['predicateobjects']:
-                # there are graphs in the subjects and the predicateobjects
-                graphs_subject_list = mapping_value['graphs'] if type(mapping_value['graphs']) is list else [mapping_value['graphs']]
-                mapping_value['predicateobjects']['graphs'] = mapping_value['predicateobjects']['graphs'] if type(mapping_value['predicateobjects']['graphs']) is list else [mapping_value['predicateobjects']['graphs']]
-                mapping_value['predicateobjects']['graphs'].extend(graphs_subject_list)
-            else:
-                mapping_value['predicateobjects']['graphs'] = mapping_value['graphs']
-            mapping_value.pop('graphs')
     # predicateobject shortcuts [foaf: firstName, $(firstname)] to dict
     #- [foaf: firstName, $(firstname), xsd: string]
     #- [[foaf: knows, rdfs: label], $(colleague)~iri]
     #- [[foaf: name, rdfs: label], [$(firstname), $(lastname)]]
     #- [foaf: firstName, $(firstname), en~lang]
     for mapping_key, mapping_value in mappings['mappings'].items():
         if 'predicateobjects' in mapping_value:
@@ -282,14 +273,29 @@
                     predicateobject_dict = {'predicates': predicates, 'objects': {'value': objects}}
                     if lang_datatype.endswith('~lang'):
                         predicateobject_dict['objects']['language'] = lang_datatype[:-5]
                     else:
                         predicateobject_dict['objects']['datatype'] = lang_datatype
                 mapping_value['predicateobjects'] = predicateobject_dict
 
+    # move graphs in subjects to predicateobjects
+    for mapping_key, mapping_value in mappings['mappings'].items():
+        if 'graphs' in mapping_value and 'predicateobjects' in mapping_value:
+            if 'graphs' in mapping_value['predicateobjects']:
+                # there are graphs in the subjects and the predicateobjects
+                graphs_subject_list = mapping_value['graphs'] if type(mapping_value['graphs']) is list else [
+                    mapping_value['graphs']]
+                mapping_value['predicateobjects']['graphs'] = mapping_value['predicateobjects']['graphs'] if type(
+                    mapping_value['predicateobjects']['graphs']) is list else [
+                    mapping_value['predicateobjects']['graphs']]
+                mapping_value['predicateobjects']['graphs'].extend(graphs_subject_list)
+            else:
+                mapping_value['predicateobjects']['graphs'] = mapping_value['graphs']
+            mapping_value.pop('graphs')
+
     # expand objects: [[$(firstname), en~lang], [$(lastname), nl~lang]] (Example 83 in YARRRML spec)
     for mapping_key, mapping_value in mappings['mappings'].items():
         if 'predicateobjects' in mapping_value and 'objects' in mapping_value['predicateobjects'] and type(mapping_value['predicateobjects']['objects']) is list:
             if type(mapping_value['predicateobjects']['objects'][0]) is list:
                 for i, object in enumerate(mapping_value['predicateobjects']['objects']):
                     value, lang_datatype = object
                     if '~' in lang_datatype:
@@ -468,15 +474,15 @@
             mapping_graph.add((subject_bnode, rdflib.term.URIRef(RML_CONSTANT), rdflib.BNode()))
             mapping_graph.add((subject_bnode, rdflib.term.URIRef(RML_TERM_TYPE), rdflib.term.URIRef(RML_BLANK_NODE)))
 
         ####################### GRAPHS ####################
         if 'graphs' in mapping_value:
             graph_bnode = rdflib.BNode()
             mapping_graph.add((triples_map_iri, rdflib.term.URIRef(RML_GRAPH_MAP), graph_bnode))
-            mapping_graph = _add_template(mapping_graph, subject_bnode, mapping_value['graphs'])
+            mapping_graph = _add_template(mapping_graph, graph_bnode, mapping_value['graphs'])
 
         ####################### PREDICATE OBJECTS ############
         if 'predicateobjects' in mapping_value:
             predicateobject_bnode = rdflib.BNode()
             mapping_graph.add((triples_map_iri, rdflib.term.URIRef(RML_PREDICATE_OBJECT_MAP), predicateobject_bnode))
 
             for position, property in zip(['predicates', 'objects', 'graphs'], [RML_PREDICATE_MAP, RML_OBJECT_MAP, RML_GRAPH_MAP]):
```

### Comparing `morph_kgc-2.6.4/test/issues/issue_118/mapping.ttl` & `morph_kgc-2.7.0/test/issues/issue_118/mapping.ttl`

 * *Files 11% similar despite different names*

```diff
@@ -1,42 +1,40 @@
-@prefix rr: <http://www.w3.org/ns/r2rml#> .
 @prefix rdf: <http://www.w3.org/1999/02/22-rdf-syntax-ns#> .
 @prefix rdfs: <http://www.w3.org/2000/01/rdf-schema#> .
 @prefix fnml: <http://semweb.mmlab.be/ns/fnml#> .
 @prefix fno: <https://w3id.org/function/ontology#> .
 @prefix d2rq: <http://www.wiwiss.fu-berlin.de/suhl/bizer/D2RQ/0.1#> .
 @prefix void: <http://rdfs.org/ns/void#> .
 @prefix dc: <http://purl.org/dc/terms/> .
 @prefix foaf: <http://xmlns.com/foaf/0.1/> .
-@prefix rml: <http://semweb.mmlab.be/ns/rml#> .
-@prefix ql: <http://semweb.mmlab.be/ns/ql#> .
+@prefix rml: <http://w3id.org/rml/> .
 @prefix haObjId: <https://data.hetarchief.be/id/object/> .
 @prefix premis: <http://www.loc.gov/premis/rdf/v3/> .
 @prefix : <http://mapping.example.com/> .
 
 :map_premis_000 rml:logicalSource :source_000 ;
-	rdf:type rr:TriplesMap ;
+	rdf:type rml:TriplesMap ;
 	rdfs:label "premis" ;
-	rr:predicateObjectMap :pom_000 ;
-	rr:subjectMap :s_000 .
+	rml:predicateObjectMap :pom_000 ;
+	rml:subjectMap :s_000 .
 
-:om_000 rdf:type rr:ObjectMap ;
-	rr:constant "http://www.loc.gov/premis/rdf/v3/IntellectualEntity" ;
-	rr:termType rr:IRI .
-
-:pm_000 rdf:type rr:PredicateMap ;
-	rr:constant rdf:type .
-
-:pom_000 rdf:type rr:PredicateObjectMap ;
-	rr:objectMap :om_000 ;
-	rr:predicateMap :pm_000 .
+:om_000 rdf:type rml:ObjectMap ;
+	rml:constant "http://www.loc.gov/premis/rdf/v3/IntellectualEntity" ;
+	rml:termType rml:IRI .
+
+:pm_000 rdf:type rml:PredicateMap ;
+	rml:constant rdf:type .
+
+:pom_000 rdf:type rml:PredicateObjectMap ;
+	rml:objectMap :om_000 ;
+	rml:predicateMap :pm_000 .
 
 :rules_000 void:exampleResource :map_premis_000 ;
 	rdf:type void:Dataset .
 
-:s_000 rdf:type rr:SubjectMap ;
-	rr:template "https://data.hetarchief.be/id/object/{premis:object/premis:objectIdentifier/premis:objectIdentifierValue}" .
+:s_000 rdf:type rml:SubjectMap ;
+	rml:template "https://data.hetarchief.be/id/object/{premis:object/premis:objectIdentifier/premis:objectIdentifierValue}" .
 
 :source_000 rml:iterator "/premis:premis" ;
-	rml:referenceFormulation ql:XPath ;
+	rml:referenceFormulation rml:XPath ;
 	rml:source "test/issues/issue_118/premis.xml" ;
 	rdf:type rml:LogicalSource .
```

### Comparing `morph_kgc-2.6.4/test/issues/issue_118/premis.xml` & `morph_kgc-2.7.0/test/issues/issue_118/premis.xml`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/issues/issue_118/test_issue_118.py` & `morph_kgc-2.7.0/test/issues/issue_118/test_issue_118.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/issues/issue_124/mapping.ttl` & `morph_kgc-2.7.0/test/rml-star/RMLSTARTC006a/mapping.ttl`

 * *Files 12% similar despite different names*

```diff
@@ -1,65 +1,36 @@
-@prefix rr: <http://www.w3.org/ns/r2rml#> .
-@prefix rml: <http://semweb.mmlab.be/ns/rml#> .
 @prefix rdf: <http://www.w3.org/1999/02/22-rdf-syntax-ns#> .
-@prefix ql: <http://semweb.mmlab.be/ns/ql#> .
+@prefix rml: <http://w3id.org/rml/> .
 @prefix ex: <http://example/> .
 @prefix xsd: <http://www.w3.org/2001/XMLSchema#> .
 @prefix : <http://example.org/> .
 @base <http://example.org/> .
 
-:firstTM a rr:TriplesMap ;
+:firstTM a rml:NonAssertedTriplesMap ; # This refers to the y statement in the rdf-star
     rml:logicalSource [
-        rml:source "test/issues/issue_124/data.csv";
-        rml:referenceFormulation ql:CSV
+        rml:source "test/rml-star/RMLSTARTC006a/data.csv";
+        rml:referenceFormulation rml:CSV
     ];
     rml:subjectMap [
-        rr:template "http://example/{c1}"
+        rml:template "http://example/{c1}"
     ];
-    rr:predicateObjectMap [
-        rr:predicate ex:p1 ;
+    rml:predicateObjectMap [
+        rml:predicate ex:p ;
         rml:objectMap [
-            rr:template "http://example/{c2}"
-        ]
-    ];
-    rr:predicateObjectMap [
-        rr:predicate ex:p2 ;
-        rml:objectMap [
-            rr:template "http://example/{c2}"
+            rml:template "http://example/{c2}"
         ]
     ] .
 
-:secondTM a rr:TriplesMap ;
+:secondTM a rml:AssertedTriplesMap ;  # This refers to the x statement in the rdf-star
     rml:logicalSource [
-        rml:source "test/issues/issue_124/data.csv";
-        rml:referenceFormulation ql:CSV
+        rml:source "test/rml-star/RMLSTARTC006a/data.csv";
+        rml:referenceFormulation rml:CSV
     ];
     rml:subjectMap [
-        rr:template "http://example/{c3}"
-    ];
-    rr:predicateObjectMap [
-        rr:predicate ex:q1 ;
-        rml:objectMap [
-            rml:quotedTriplesMap :firstTM
-        ]
+            rml:template "http://example/{c3}"
     ];
-    rr:predicateObjectMap [
-        rr:predicate ex:q2 ;
+    rml:predicateObjectMap [
+        rml:predicate ex:p; ;
         rml:objectMap [
             rml:quotedTriplesMap :firstTM
         ]
     ] .
-
-:thirdTM a rr:TriplesMap ;
-    rml:logicalSource [
-        rml:source "test/issues/issue_124/data.csv";
-        rml:referenceFormulation ql:CSV
-    ];
-    rml:subjectMap [
-        rml:quotedTriplesMap :secondTM
-    ];
-    rr:predicateObjectMap [
-        rr:predicate ex:r ;
-        rml:objectMap [
-            rr:template "http://example/{c4}"
-        ]
-    ] .
```

### Comparing `morph_kgc-2.6.4/test/issues/issue_124/output.nq` & `morph_kgc-2.7.0/test/issues/issue_124/output.nq`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/issues/issue_124/test_issue_124.py` & `morph_kgc-2.7.0/test/issues/issue_124/test_issue_124.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/issues/issue_145/mapping.ttl` & `morph_kgc-2.7.0/test/issues/issue_145/mapping.ttl`

 * *Files 8% similar despite different names*

```diff
@@ -1,34 +1,32 @@
-@prefix rr: <http://www.w3.org/ns/r2rml#> .
 @prefix foaf: <http://xmlns.com/foaf/0.1/> .
 @prefix ex: <http://example.com/> .
 @prefix xsd: <http://www.w3.org/2001/XMLSchema#> .
-@prefix rml: <http://semweb.mmlab.be/ns/rml#> .
-@prefix ql: <http://semweb.mmlab.be/ns/ql#> .
+@prefix rml: <http://w3id.org/rml/> .
 @prefix fnml: <http://semweb.mmlab.be/ns/fnml#> .
 @prefix fno: <https://w3id.org/function/ontology#> .
 @prefix morph-kgc: <https://github.com/morph-kgc/morph-kgc/function/built-in.ttl#> .
 @prefix grel: <http://users.ugent.be/~bjdmeest/function/grel.ttl#> .
 @prefix idlab-fn: <http://example.com/idlab/function/> .
 @prefix gtfs: <http://vocab.gtfs.org/terms#> .
 @prefix dct: <http://purl.org/dc/terms/> .
 
 @base <http://example.com/base/> .
 
 <TriplesMap1>
     rml:logicalSource [
         rml:source "test/issues/issue_145/data.csv" ;
-        rml:referenceFormulation ql:CSV ;
+        rml:referenceFormulation rml:CSV ;
     ];
-    rr:subjectMap [
-        rr:template "http://transport.linkeddata.es/madrid/metro/calendar_rules/{service_id}"
+    rml:subjectMap [
+        rml:template "http://transport.linkeddata.es/madrid/metro/calendar_rules/{service_id}"
     ];
-    rr:predicateObjectMap [
-        rr:predicate dct:example;
-        rr:objectMap [
+    rml:predicateObjectMap [
+        rml:predicate dct:example;
+        rml:objectMap [
             fnml:execution <#Execution>
         ]
     ].
 
 <#Execution>
     fnml:function morph-kgc:concat ;
     fnml:input
@@ -44,10 +42,10 @@
                 rml:reference "monday"
             ]
         ],
         [
 
             fnml:parameter grel:param_string_sep ;
             fnml:valueMap [
-                rr:template "-"
+                rml:template "-"
             ]
         ] .
```

### Comparing `morph_kgc-2.6.4/test/issues/issue_145/test_issue_145.py` & `morph_kgc-2.7.0/test/issues/issue_145/test_issue_145.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/issues/issue_174/mapping-a.ttl` & `morph_kgc-2.7.0/test/issues/issue_174/mapping-a.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/issues/issue_174/mapping-b.ttl` & `morph_kgc-2.7.0/test/issues/issue_174/mapping-b.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/issues/issue_174/mapping-c.ttl` & `morph_kgc-2.7.0/test/issues/issue_174/mapping-c.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/issues/issue_174/output-a.nq` & `morph_kgc-2.7.0/test/issues/issue_174/output-a.nq`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/issues/issue_174/output-b.nq` & `morph_kgc-2.7.0/test/issues/issue_174/output-b.nq`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/issues/issue_174/output-c.nq` & `morph_kgc-2.7.0/test/issues/issue_174/output-c.nq`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/issues/issue_174/test_issue_174.py` & `morph_kgc-2.7.0/test/issues/issue_174/test_issue_174.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/issues/issue_62/mapping.ttl` & `morph_kgc-2.7.0/test/rml-star/RMLSTARTC001b/mapping.ttl`

 * *Files 20% similar despite different names*

```diff
@@ -1,39 +1,40 @@
-@prefix rr: <http://www.w3.org/ns/r2rml#> .
-@prefix rml: <http://semweb.mmlab.be/ns/rml#> .
-@prefix ql: <http://semweb.mmlab.be/ns/ql#> .
-@prefix ex: <http://www.example.com/> .
+@prefix rdf: <http://www.w3.org/1999/02/22-rdf-syntax-ns#> .
+@prefix rml: <http://w3id.org/rml/> .
+@prefix ex: <http://example/> .
+@prefix : <http://example.org/> .
+@base <http://example.org/> .
 
-<#TriplesMap1>
-    a rr:TriplesMap;
+:firstTM a rml:AssertedTriplesMap ;
     rml:logicalSource [
-        rml:source "test/issues/issue_62/data1.csv";
-        rml:referenceFormulation ql:CSV
+        rml:source "test/rml-star/RMLSTARTC001b/data1.csv";
+        rml:referenceFormulation rml:CSV
     ];
-    rr:subjectMap [
-        rr:template "http://example.com/{id}";
-        rr:class ex:Example
+    rml:subjectMap [
+        rml:reference "c1-1" ;
+        rml:termType rml:BlankNode
     ];
-    rr:predicateObjectMap [
-        rr:predicate ex:relation;
-        rr:objectMap [
-        rr:parentTriplesMap <#TriplesMap2>;
-        rr:joinCondition [
-            rr:child "column1";
-            rr:parent "column1";
-            ];
-        rr:joinCondition [
-            rr:child "column2";
-            rr:parent "column2";
-            ];
-        ];
-    ].
+    rml:predicateObjectMap [
+        rml:predicate ex:p ;
+        rml:objectMap [
+            rml:template "http://example/{c1-2}"
+        ]
+    ] .
 
-<#TriplesMap2>
-    a rr:TriplesMap;
+:secondTM a rml:AssertedTriplesMap ;
     rml:logicalSource [
-        rml:source "test/issues/issue_62/data2.csv";
-        rml:referenceFormulation ql:CSV
+        rml:source "test/rml-star/RMLSTARTC001b/data2.csv";
+        rml:referenceFormulation rml:CSV
+    ];
+    rml:subjectMap [
+        rml:quotedTriplesMap :firstTM ;
+        rml:joinCondition [
+          rml:child "c2-2" ;
+          rml:parent "c1-3" ;
+        ];
     ];
-    rr:subjectMap [
-        rr:template "http://second-example.com/{id}"
-    ].
+    rml:predicateObjectMap [
+        rml:predicate ex:q ;
+        rml:objectMap [
+            rml:reference "c2-1"
+        ]
+    ] .
```

### Comparing `morph_kgc-2.6.4/test/issues/issue_62/output.nq` & `morph_kgc-2.7.0/test/issues/issue_62/output.nq`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/issues/issue_62/test_issue_62.py` & `morph_kgc-2.7.0/test/issues/issue_62/test_issue_62.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/issues/issue_67/mapping.ttl` & `morph_kgc-2.7.0/test/r2rml/R2RMLTC0014d/mapping.ttl`

 * *Files 23% similar despite different names*

```diff
@@ -1,36 +1,26 @@
 @prefix rr: <http://www.w3.org/ns/r2rml#> .
-@prefix rml: <http://semweb.mmlab.be/ns/rml#> .
-@prefix ql: <http://semweb.mmlab.be/ns/ql#> .
+@prefix rdf: <http://www.w3.org/1999/02/22-rdf-syntax-ns#> .
+@prefix ex: <http://example.com/ns#> .
+@prefix emp: <http://example.com/emp#> .
+@prefix dept: <http://example.com/dept#> .
 @prefix xsd: <http://www.w3.org/2001/XMLSchema#> .
-@prefix ex: <http://www.example.com/> .
+@base <http://example.com/base/> .
 
-<#TriplesMap1>
-    a rr:TriplesMap;
-    rml:logicalSource [
-        rml:source "test/issues/issue_67/data.csv";
-        rml:referenceFormulation ql:CSV
-    ];
+<TriplesMap4>
+	a rr:TriplesMap;
+    rr:logicalTable [ rr:sqlQuery """
+
+        SELECT "EMP".*, (CASE "job"
+            WHEN 'CLERK' THEN 'general-office'
+            WHEN 'NIGHTGUARD' THEN 'security'
+            WHEN 'ENGINEER' THEN 'engineering'
+        END) AS ROLE FROM "EMP"
+
+        """ ];
     rr:subjectMap [
-        rr:template "http://example.com/{id}";
-    ];
-    rr:predicateObjectMap [
-        rr:predicate ex:boolean;
-        rr:objectMap [
-            rr:column "column1";
-            rr:datatype xsd:boolean
-        ];
-    ];
-    rr:predicateObjectMap [
-        rr:predicate ex:dateTime;
-        rr:objectMap [
-            rr:column "column2";
-            rr:datatype xsd:dateTime
-        ];
+        rr:template "http://data.example.com/employee/{empno}";
     ];
     rr:predicateObjectMap [
-        rr:predicate ex:integer;
-        rr:objectMap [
-            rr:column "column3";
-            rr:datatype xsd:integer
-        ];
+        rr:predicate ex:role;
+        rr:objectMap [ rr:template "http://data.example.com/roles/{ROLE}" ];
     ].
```

### Comparing `morph_kgc-2.6.4/test/issues/issue_67/test_issue_67.py` & `morph_kgc-2.7.0/test/issues/issue_67/test_issue_67.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/issues/issue_80/mapping.rml` & `morph_kgc-2.7.0/test/issues/issue_80/mapping.rml`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/issues/issue_80/test_issue_80.py` & `morph_kgc-2.7.0/test/issues/issue_80/test_issue_80.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/issues/issue_81/mapping.ttl` & `morph_kgc-2.7.0/test/rml-core/csv/RMLTC0000/mapping.ttl`

 * *Files 14% similar despite different names*

```diff
@@ -1,23 +1,25 @@
-@prefix rr: <http://www.w3.org/ns/r2rml#> .
 @prefix foaf: <http://xmlns.com/foaf/0.1/> .
 @prefix ex: <http://example.com/> .
 @prefix xsd: <http://www.w3.org/2001/XMLSchema#> .
-@prefix rml: <http://semweb.mmlab.be/ns/rml#> .
-@prefix ql: <http://semweb.mmlab.be/ns/ql#> .
-@prefix activity: <http://example.com/activity/> .
+@prefix rml: <http://w3id.org/rml/> .
+
 @base <http://example.com/base/> .
 
 <TriplesMap1>
-  a rr:TriplesMap;
+  a rml:TriplesMap;
 
   rml:logicalSource [
-    rml:source "test/issues/issue_81/country_info.csv";
-    rml:referenceFormulation ql:CSV
-  ];
+    rml:source "test/rml-core/csv/RMLTC0000/student.csv";
+    rml:referenceFormulation rml:CSV
+  ] ;
 
-  rr:subjectMap [ rr:template "http://example.com/{Country Code}" ];
+  rml:subjectMap [
+    rml:template "http://example.com/{Name}"
+  ];
 
-  rr:predicateObjectMap [
-    rr:predicate ex:name ;
-    rr:objectMap [ rml:reference "Name" ]
-  ] .
+  rml:predicateObjectMap [
+    rml:predicate foaf:name ;
+    rml:objectMap [
+      rml:reference "Name"
+    ]
+  ].
```

### Comparing `morph_kgc-2.6.4/test/issues/issue_81/test_issue_81.py` & `morph_kgc-2.7.0/test/issues/issue_81/test_issue_81.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/r2rml/R2RMLTC0000/resource.db` & `morph_kgc-2.7.0/test/r2rml/R2RMLTC0000/resource.db`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/r2rml/R2RMLTC0000/test_R2RMLTC0000_SQLITE.py` & `morph_kgc-2.7.0/test/r2rml/R2RMLTC0000/test_R2RMLTC0000_SQLITE.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/r2rml/R2RMLTC0001a/resource.db` & `morph_kgc-2.7.0/test/r2rml/R2RMLTC0001a/resource.db`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/r2rml/R2RMLTC0001a/test_R2RMLTC0001a_SQLITE.py` & `morph_kgc-2.7.0/test/r2rml/R2RMLTC0001a/test_R2RMLTC0001a_SQLITE.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/r2rml/R2RMLTC0001b/resource.db` & `morph_kgc-2.7.0/test/r2rml/R2RMLTC0001b/resource.db`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/r2rml/R2RMLTC0001b/test_R2RMLTC0001b_SQLITE.py` & `morph_kgc-2.7.0/test/r2rml/R2RMLTC0001b/test_R2RMLTC0001b_SQLITE.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/r2rml/R2RMLTC0002a/mapping.ttl` & `morph_kgc-2.7.0/test/r2rml/R2RMLTC0002a/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/r2rml/R2RMLTC0002a/resource.db` & `morph_kgc-2.7.0/test/r2rml/R2RMLTC0002a/resource.db`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/r2rml/R2RMLTC0002a/test_R2RMLTC0002a_SQLITE.py` & `morph_kgc-2.7.0/test/r2rml/R2RMLTC0002a/test_R2RMLTC0002a_SQLITE.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/r2rml/R2RMLTC0002b/resource.db` & `morph_kgc-2.7.0/test/r2rml/R2RMLTC0002b/resource.db`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/r2rml/R2RMLTC0002b/test_R2RMLTC0002b_SQLITE.py` & `morph_kgc-2.7.0/test/r2rml/R2RMLTC0002b/test_R2RMLTC0002b_SQLITE.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/r2rml/R2RMLTC0002c/resource.db` & `morph_kgc-2.7.0/test/r2rml/R2RMLTC0002c/resource.db`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/r2rml/R2RMLTC0002c/test_R2RMLTC0002c_SQLITE.py` & `morph_kgc-2.7.0/test/r2rml/R2RMLTC0002c/test_R2RMLTC0002c_SQLITE.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/r2rml/R2RMLTC0002d/mapping.ttl` & `morph_kgc-2.7.0/test/r2rml/R2RMLTC0002d/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/r2rml/R2RMLTC0002d/resource.db` & `morph_kgc-2.7.0/test/r2rml/R2RMLTC0002d/resource.db`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/r2rml/R2RMLTC0002d/test_R2RMLTC0002d_SQLITE.py` & `morph_kgc-2.7.0/test/r2rml/R2RMLTC0002d/test_R2RMLTC0002d_SQLITE.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/r2rml/R2RMLTC0002e/resource.db` & `morph_kgc-2.7.0/test/r2rml/R2RMLTC0002e/resource.db`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/r2rml/R2RMLTC0002e/test_R2RMLTC0002e_SQLITE.py` & `morph_kgc-2.7.0/test/r2rml/R2RMLTC0002e/test_R2RMLTC0002e_SQLITE.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/r2rml/R2RMLTC0002f/mapping.ttl` & `morph_kgc-2.7.0/test/r2rml/R2RMLTC0002f/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/r2rml/R2RMLTC0002f/resource.db` & `morph_kgc-2.7.0/test/r2rml/R2RMLTC0002f/resource.db`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/r2rml/R2RMLTC0002f/test_R2RMLTC0002f_SQLITE.py` & `morph_kgc-2.7.0/test/r2rml/R2RMLTC0002f/test_R2RMLTC0002f_SQLITE.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/r2rml/R2RMLTC0002g/mapping.ttl` & `morph_kgc-2.7.0/test/r2rml/R2RMLTC0002g/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/r2rml/R2RMLTC0002g/resource.db` & `morph_kgc-2.7.0/test/r2rml/R2RMLTC0002g/resource.db`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/r2rml/R2RMLTC0002g/test_R2RMLTC0002g_SQLITE.py` & `morph_kgc-2.7.0/test/r2rml/R2RMLTC0002g/test_R2RMLTC0002g_SQLITE.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/r2rml/R2RMLTC0002h/mapping.ttl` & `morph_kgc-2.7.0/test/r2rml/R2RMLTC0002h/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/r2rml/R2RMLTC0002h/resource.db` & `morph_kgc-2.7.0/test/r2rml/R2RMLTC0002h/resource.db`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/r2rml/R2RMLTC0002h/test_R2RMLTC0002h_SQLITE.py` & `morph_kgc-2.7.0/test/r2rml/R2RMLTC0002h/test_R2RMLTC0002h_SQLITE.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/r2rml/R2RMLTC0002i/mapping.ttl` & `morph_kgc-2.7.0/test/r2rml/R2RMLTC0002i/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/r2rml/R2RMLTC0002i/resource.db` & `morph_kgc-2.7.0/test/r2rml/R2RMLTC0002i/resource.db`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/r2rml/R2RMLTC0002i/test_R2RMLTC0002i_SQLITE.py` & `morph_kgc-2.7.0/test/r2rml/R2RMLTC0002i/test_R2RMLTC0002i_SQLITE.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/r2rml/R2RMLTC0002j/mapping.ttl` & `morph_kgc-2.7.0/test/r2rml/R2RMLTC0002j/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/r2rml/R2RMLTC0002j/resource.db` & `morph_kgc-2.7.0/test/r2rml/R2RMLTC0002j/resource.db`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/r2rml/R2RMLTC0002j/test_R2RMLTC0002j_SQLITE.py` & `morph_kgc-2.7.0/test/r2rml/R2RMLTC0002j/test_R2RMLTC0002j_SQLITE.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/r2rml/R2RMLTC0003a/R2RMLTC0003a_SQLITE.py` & `morph_kgc-2.7.0/test/r2rml/R2RMLTC0003a/R2RMLTC0003a_SQLITE.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/r2rml/R2RMLTC0003a/mapping.ttl` & `morph_kgc-2.7.0/test/r2rml/R2RMLTC0003a/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/r2rml/R2RMLTC0003a/resource.db` & `morph_kgc-2.7.0/test/r2rml/R2RMLTC0003a/resource.db`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/r2rml/R2RMLTC0003b/mapping.ttl` & `morph_kgc-2.7.0/test/r2rml/R2RMLTC0003b/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/r2rml/R2RMLTC0003b/resource.db` & `morph_kgc-2.7.0/test/r2rml/R2RMLTC0003b/resource.db`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/r2rml/R2RMLTC0003b/test_R2RMLTC0003b_SQLITE.py` & `morph_kgc-2.7.0/test/r2rml/R2RMLTC0003b/test_R2RMLTC0003b_SQLITE.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/r2rml/R2RMLTC0003c/mapping.ttl` & `morph_kgc-2.7.0/test/r2rml/R2RMLTC0003c/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/r2rml/R2RMLTC0003c/resource.db` & `morph_kgc-2.7.0/test/r2rml/R2RMLTC0003c/resource.db`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/r2rml/R2RMLTC0003c/test_R2RMLTC0003c_SQLITE.py` & `morph_kgc-2.7.0/test/r2rml/R2RMLTC0003c/test_R2RMLTC0003c_SQLITE.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/r2rml/R2RMLTC0004a/mapping.ttl` & `morph_kgc-2.7.0/test/r2rml/R2RMLTC0004a/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/r2rml/R2RMLTC0004a/resource.db` & `morph_kgc-2.7.0/test/r2rml/R2RMLTC0004a/resource.db`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/r2rml/R2RMLTC0004a/test_R2RMLTC0004a_SQLITE.py` & `morph_kgc-2.7.0/test/r2rml/R2RMLTC0004a/test_R2RMLTC0004a_SQLITE.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/r2rml/R2RMLTC0004b/mapping.ttl` & `morph_kgc-2.7.0/test/r2rml/R2RMLTC0004b/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/r2rml/R2RMLTC0004b/resource.db` & `morph_kgc-2.7.0/test/r2rml/R2RMLTC0004b/resource.db`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/r2rml/R2RMLTC0004b/test_R2RMLTC0004b_SQLITE.py` & `morph_kgc-2.7.0/test/r2rml/R2RMLTC0004b/test_R2RMLTC0004b_SQLITE.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/r2rml/R2RMLTC0005a/mapping.ttl` & `morph_kgc-2.7.0/test/r2rml/R2RMLTC0005a/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/r2rml/R2RMLTC0005a/resource.db` & `morph_kgc-2.7.0/test/r2rml/R2RMLTC0005a/resource.db`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/r2rml/R2RMLTC0005a/test_R2RMLTC0005a_SQLITE.py` & `morph_kgc-2.7.0/test/r2rml/R2RMLTC0005a/test_R2RMLTC0005a_SQLITE.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/r2rml/R2RMLTC0005b/mapping.ttl` & `morph_kgc-2.7.0/test/r2rml/R2RMLTC0005b/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/r2rml/R2RMLTC0005b/output.nq` & `morph_kgc-2.7.0/test/r2rml/R2RMLTC0005b/output.nq`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/r2rml/R2RMLTC0005b/resource.db` & `morph_kgc-2.7.0/test/r2rml/R2RMLTC0005b/resource.db`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/r2rml/R2RMLTC0005b/test_R2RMLTC0005b_SQLITE.py` & `morph_kgc-2.7.0/test/r2rml/R2RMLTC0005b/test_R2RMLTC0005b_SQLITE.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/r2rml/R2RMLTC0006a/mapping.ttl` & `morph_kgc-2.7.0/test/r2rml/R2RMLTC0006a/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/r2rml/R2RMLTC0006a/resource.db` & `morph_kgc-2.7.0/test/r2rml/R2RMLTC0006a/resource.db`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/r2rml/R2RMLTC0006a/test_R2RMLTC0006a_SQLITE.py` & `morph_kgc-2.7.0/test/r2rml/R2RMLTC0006a/test_R2RMLTC0006a_SQLITE.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/r2rml/R2RMLTC0007a/mapping.ttl` & `morph_kgc-2.7.0/test/r2rml/R2RMLTC0007a/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/r2rml/R2RMLTC0007a/resource.db` & `morph_kgc-2.7.0/test/r2rml/R2RMLTC0007a/resource.db`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/r2rml/R2RMLTC0007a/test_R2RMLTC0007a_SQLITE.py` & `morph_kgc-2.7.0/test/r2rml/R2RMLTC0007a/test_R2RMLTC0007a_SQLITE.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/r2rml/R2RMLTC0007b/mapping.ttl` & `morph_kgc-2.7.0/test/r2rml/R2RMLTC0007b/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/r2rml/R2RMLTC0007b/resource.db` & `morph_kgc-2.7.0/test/r2rml/R2RMLTC0007b/resource.db`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/r2rml/R2RMLTC0007b/test_R2RMLTC0007b_SQLITE.py` & `morph_kgc-2.7.0/test/r2rml/R2RMLTC0007b/test_R2RMLTC0007b_SQLITE.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/r2rml/R2RMLTC0007c/mapping.ttl` & `morph_kgc-2.7.0/test/r2rml/R2RMLTC0007c/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/r2rml/R2RMLTC0007c/resource.db` & `morph_kgc-2.7.0/test/r2rml/R2RMLTC0007c/resource.db`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/r2rml/R2RMLTC0007c/test_R2RMLTC0007c_SQLITE.py` & `morph_kgc-2.7.0/test/r2rml/R2RMLTC0007c/test_R2RMLTC0007c_SQLITE.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/r2rml/R2RMLTC0007d/mapping.ttl` & `morph_kgc-2.7.0/test/r2rml/R2RMLTC0007d/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/r2rml/R2RMLTC0007d/resource.db` & `morph_kgc-2.7.0/test/r2rml/R2RMLTC0007d/resource.db`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/r2rml/R2RMLTC0007d/test_R2RMLTC0007d_SQLITE.py` & `morph_kgc-2.7.0/test/r2rml/R2RMLTC0007d/test_R2RMLTC0007d_SQLITE.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/r2rml/R2RMLTC0007e/mapping.ttl` & `morph_kgc-2.7.0/test/r2rml/R2RMLTC0007e/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/r2rml/R2RMLTC0007e/resource.db` & `morph_kgc-2.7.0/test/r2rml/R2RMLTC0007e/resource.db`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/r2rml/R2RMLTC0007e/test_R2RMLTC0007e_SQLITE.py` & `morph_kgc-2.7.0/test/r2rml/R2RMLTC0007e/test_R2RMLTC0007e_SQLITE.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/r2rml/R2RMLTC0007f/mapping.ttl` & `morph_kgc-2.7.0/test/r2rml/R2RMLTC0007f/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/r2rml/R2RMLTC0007f/resource.db` & `morph_kgc-2.7.0/test/r2rml/R2RMLTC0007f/resource.db`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/r2rml/R2RMLTC0007f/test_R2RMLTC0007f_SQLITE.py` & `morph_kgc-2.7.0/test/r2rml/R2RMLTC0007f/test_R2RMLTC0007f_SQLITE.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/r2rml/R2RMLTC0007g/mapping.ttl` & `morph_kgc-2.7.0/test/r2rml/R2RMLTC0007g/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/r2rml/R2RMLTC0007g/resource.db` & `morph_kgc-2.7.0/test/r2rml/R2RMLTC0007g/resource.db`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/r2rml/R2RMLTC0007g/test_R2RMLTC0007g_SQLITE.py` & `morph_kgc-2.7.0/test/r2rml/R2RMLTC0007g/test_R2RMLTC0007g_SQLITE.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/r2rml/R2RMLTC0007h/mapping.ttl` & `morph_kgc-2.7.0/test/r2rml/R2RMLTC0007h/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/r2rml/R2RMLTC0007h/resource.db` & `morph_kgc-2.7.0/test/r2rml/R2RMLTC0007h/resource.db`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/r2rml/R2RMLTC0007h/test_R2RMLTC0007h_SQLITE.py` & `morph_kgc-2.7.0/test/r2rml/R2RMLTC0007h/test_R2RMLTC0007h_SQLITE.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/r2rml/R2RMLTC0008a/mapping.ttl` & `morph_kgc-2.7.0/test/r2rml/R2RMLTC0008a/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/r2rml/R2RMLTC0008a/output.nq` & `morph_kgc-2.7.0/test/r2rml/R2RMLTC0008a/output.nq`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/r2rml/R2RMLTC0008a/resource.db` & `morph_kgc-2.7.0/test/r2rml/R2RMLTC0008a/resource.db`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/r2rml/R2RMLTC0008a/test_R2RMLTC0008a_SQLITE.py` & `morph_kgc-2.7.0/test/r2rml/R2RMLTC0008a/test_R2RMLTC0008a_SQLITE.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/r2rml/R2RMLTC0008b/mapping.ttl` & `morph_kgc-2.7.0/test/r2rml/R2RMLTC0008b/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/r2rml/R2RMLTC0008b/output.nq` & `morph_kgc-2.7.0/test/r2rml/R2RMLTC0008b/output.nq`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/r2rml/R2RMLTC0008b/resource.db` & `morph_kgc-2.7.0/test/r2rml/R2RMLTC0008b/resource.db`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/r2rml/R2RMLTC0008b/test_R2RMLTC0008b_SQLITE.py` & `morph_kgc-2.7.0/test/r2rml/R2RMLTC0008b/test_R2RMLTC0008b_SQLITE.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/r2rml/R2RMLTC0008c/mapping.ttl` & `morph_kgc-2.7.0/test/r2rml/R2RMLTC0008c/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/r2rml/R2RMLTC0008c/resource.db` & `morph_kgc-2.7.0/test/r2rml/R2RMLTC0008c/resource.db`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/r2rml/R2RMLTC0008c/test_R2RMLTC0008c_SQLITE.py` & `morph_kgc-2.7.0/test/r2rml/R2RMLTC0008c/test_R2RMLTC0008c_SQLITE.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/r2rml/R2RMLTC0009a/mapping.ttl` & `morph_kgc-2.7.0/test/r2rml/R2RMLTC0009a/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/r2rml/R2RMLTC0009a/resource.db` & `morph_kgc-2.7.0/test/r2rml/R2RMLTC0009a/resource.db`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/r2rml/R2RMLTC0009a/test_R2RMLTC0009a_SQLITE.py` & `morph_kgc-2.7.0/test/r2rml/R2RMLTC0009a/test_R2RMLTC0009a_SQLITE.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/r2rml/R2RMLTC0009b/mapping.ttl` & `morph_kgc-2.7.0/test/r2rml/R2RMLTC0009b/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/r2rml/R2RMLTC0009b/output.nq` & `morph_kgc-2.7.0/test/r2rml/R2RMLTC0009b/output.nq`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/r2rml/R2RMLTC0009b/resource.db` & `morph_kgc-2.7.0/test/r2rml/R2RMLTC0009b/resource.db`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/r2rml/R2RMLTC0009b/test_R2RMLTC0009b_SQLITE.py` & `morph_kgc-2.7.0/test/r2rml/R2RMLTC0009b/test_R2RMLTC0009b_SQLITE.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/r2rml/R2RMLTC0009c/mapping.ttl` & `morph_kgc-2.7.0/test/r2rml/R2RMLTC0009c/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/r2rml/R2RMLTC0009c/resource.db` & `morph_kgc-2.7.0/test/r2rml/R2RMLTC0009c/resource.db`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/r2rml/R2RMLTC0009c/test_R2RMLTC0009c_SQLITE.py` & `morph_kgc-2.7.0/test/r2rml/R2RMLTC0009c/test_R2RMLTC0009c_SQLITE.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/r2rml/R2RMLTC0009d/mapping.ttl` & `morph_kgc-2.7.0/test/r2rml/R2RMLTC0009d/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/r2rml/R2RMLTC0009d/resource.db` & `morph_kgc-2.7.0/test/r2rml/R2RMLTC0009d/resource.db`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/r2rml/R2RMLTC0009d/test_R2RMLTC0009d_SQLITE.py` & `morph_kgc-2.7.0/test/r2rml/R2RMLTC0009d/test_R2RMLTC0009d_SQLITE.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/r2rml/R2RMLTC0010a/resource.db` & `morph_kgc-2.7.0/test/r2rml/R2RMLTC0010a/resource.db`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/r2rml/R2RMLTC0010a/test_R2RMLTC0010a_SQLITE.py` & `morph_kgc-2.7.0/test/r2rml/R2RMLTC0010a/test_R2RMLTC0010a_SQLITE.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/r2rml/R2RMLTC0010b/resource.db` & `morph_kgc-2.7.0/test/r2rml/R2RMLTC0010b/resource.db`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/r2rml/R2RMLTC0010b/test_R2RMLTC0010b_SQLITE.py` & `morph_kgc-2.7.0/test/r2rml/R2RMLTC0010b/test_R2RMLTC0010b_SQLITE.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/r2rml/R2RMLTC0010c/mapping.ttl` & `morph_kgc-2.7.0/test/r2rml/R2RMLTC0010c/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/r2rml/R2RMLTC0010c/resource.db` & `morph_kgc-2.7.0/test/r2rml/R2RMLTC0010c/resource.db`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/r2rml/R2RMLTC0010c/test_R2RMLTC0010c_SQLITE.py` & `morph_kgc-2.7.0/test/r2rml/R2RMLTC0010c/test_R2RMLTC0010c_SQLITE.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/r2rml/R2RMLTC0011a/mapping.ttl` & `morph_kgc-2.7.0/test/r2rml/R2RMLTC0011a/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/r2rml/R2RMLTC0011a/output.nq` & `morph_kgc-2.7.0/test/r2rml/R2RMLTC0011a/output.nq`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/r2rml/R2RMLTC0011a/resource.db` & `morph_kgc-2.7.0/test/r2rml/R2RMLTC0011a/resource.db`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/r2rml/R2RMLTC0011a/resource.sql` & `morph_kgc-2.7.0/test/r2rml/R2RMLTC0011a/resource.sql`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/r2rml/R2RMLTC0011a/test_R2RMLTC0011a_SQLITE.py` & `morph_kgc-2.7.0/test/r2rml/R2RMLTC0011a/test_R2RMLTC0011a_SQLITE.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/r2rml/R2RMLTC0011b/mapping.ttl` & `morph_kgc-2.7.0/test/r2rml/R2RMLTC0011b/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/r2rml/R2RMLTC0011b/output.nq` & `morph_kgc-2.7.0/test/r2rml/R2RMLTC0011b/output.nq`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/r2rml/R2RMLTC0011b/resource.db` & `morph_kgc-2.7.0/test/r2rml/R2RMLTC0011b/resource.db`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/r2rml/R2RMLTC0011b/resource.sql` & `morph_kgc-2.7.0/test/r2rml/R2RMLTC0011b/resource.sql`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/r2rml/R2RMLTC0011b/test_R2RMLTC0011b_SQLITE.py` & `morph_kgc-2.7.0/test/r2rml/R2RMLTC0011b/test_R2RMLTC0011b_SQLITE.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/r2rml/R2RMLTC0012a/mapping.ttl` & `morph_kgc-2.7.0/test/r2rml/R2RMLTC0012a/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/r2rml/R2RMLTC0012a/resource.db` & `morph_kgc-2.7.0/test/r2rml/R2RMLTC0012a/resource.db`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/r2rml/R2RMLTC0012a/resource.sql` & `morph_kgc-2.7.0/test/r2rml/R2RMLTC0012a/resource.sql`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/r2rml/R2RMLTC0012a/test_R2RMLTC0012a_SQLITE.py` & `morph_kgc-2.7.0/test/r2rml/R2RMLTC0012a/test_R2RMLTC0012a_SQLITE.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/r2rml/R2RMLTC0012b/mapping.ttl` & `morph_kgc-2.7.0/test/r2rml/R2RMLTC0012b/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/r2rml/R2RMLTC0012b/resource.db` & `morph_kgc-2.7.0/test/r2rml/R2RMLTC0012b/resource.db`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/r2rml/R2RMLTC0012b/resource.sql` & `morph_kgc-2.7.0/test/r2rml/R2RMLTC0012b/resource.sql`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/r2rml/R2RMLTC0012b/test_R2RMLTC0012b_SQLITE.py` & `morph_kgc-2.7.0/test/r2rml/R2RMLTC0012b/test_R2RMLTC0012b_SQLITE.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/r2rml/R2RMLTC0012c/mapping.ttl` & `morph_kgc-2.7.0/test/r2rml/R2RMLTC0012c/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/r2rml/R2RMLTC0012c/resource.db` & `morph_kgc-2.7.0/test/r2rml/R2RMLTC0012c/resource.db`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/r2rml/R2RMLTC0012c/resource.sql` & `morph_kgc-2.7.0/test/r2rml/R2RMLTC0012c/resource.sql`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/r2rml/R2RMLTC0012c/test_R2RMLTC0012c_SQLITE.py` & `morph_kgc-2.7.0/test/r2rml/R2RMLTC0012c/test_R2RMLTC0012c_SQLITE.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/r2rml/R2RMLTC0012d/mapping.ttl` & `morph_kgc-2.7.0/test/r2rml/R2RMLTC0012d/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/r2rml/R2RMLTC0012d/resource.db` & `morph_kgc-2.7.0/test/r2rml/R2RMLTC0012d/resource.db`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/r2rml/R2RMLTC0012d/resource.sql` & `morph_kgc-2.7.0/test/r2rml/R2RMLTC0012d/resource.sql`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/r2rml/R2RMLTC0012d/test_R2RMLTC0012d_SQLITE.py` & `morph_kgc-2.7.0/test/r2rml/R2RMLTC0012d/test_R2RMLTC0012d_SQLITE.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/r2rml/R2RMLTC0012e/mapping.ttl` & `morph_kgc-2.7.0/test/r2rml/R2RMLTC0012e/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/r2rml/R2RMLTC0012e/output.nq` & `morph_kgc-2.7.0/test/r2rml/R2RMLTC0012e/output.nq`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/r2rml/R2RMLTC0012e/resource.db` & `morph_kgc-2.7.0/test/r2rml/R2RMLTC0012e/resource.db`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/r2rml/R2RMLTC0012e/resource.sql` & `morph_kgc-2.7.0/test/r2rml/R2RMLTC0012e/resource.sql`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/r2rml/R2RMLTC0012e/test_R2RMLTC0012e_SQLITE.py` & `morph_kgc-2.7.0/test/r2rml/R2RMLTC0012e/test_R2RMLTC0012e_SQLITE.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/r2rml/R2RMLTC0013a/mapping.ttl` & `morph_kgc-2.7.0/test/r2rml/R2RMLTC0013a/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/r2rml/R2RMLTC0013a/resource.db` & `morph_kgc-2.7.0/test/r2rml/R2RMLTC0013a/resource.db`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/r2rml/R2RMLTC0013a/test_R2RMLTC0013a_SQLITE.py` & `morph_kgc-2.7.0/test/r2rml/R2RMLTC0013a/test_R2RMLTC0013a_SQLITE.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/r2rml/R2RMLTC0014d/mapping.ttl` & `morph_kgc-2.7.0/test/rml-in-memory/json_dictionary/RMLIMTC0007a/mapping.ttl`

 * *Files 27% similar despite different names*

```diff
@@ -1,26 +1,36 @@
-@prefix rr: <http://www.w3.org/ns/r2rml#> .
-@prefix rdf: <http://www.w3.org/1999/02/22-rdf-syntax-ns#> .
-@prefix ex: <http://example.com/ns#> .
-@prefix emp: <http://example.com/emp#> .
-@prefix dept: <http://example.com/dept#> .
+@prefix foaf: <http://xmlns.com/foaf/0.1/> .
+@prefix ex: <http://example.com/> .
 @prefix xsd: <http://www.w3.org/2001/XMLSchema#> .
+@prefix rml: <http://w3id.org/rml/> .
+@prefix rdf: <http://www.w3.org/1999/02/22-rdf-syntax-ns#> .
 @base <http://example.com/base/> .
+@prefix sd: <https://w3id.org/okn/o/sd#>.
+@prefix kg4di: <https://w3id.org/kg4di/definedBy>.
+
+<TriplesMap1> a rml:TriplesMap;
+
+  rml:logicalSource [
+    rml:source [
+			a sd:DatasetSpecification;
+			sd:name "variable1";
+			sd:hasDataTransformation [
+				sd:hasSourceCode [
+					sd:programmingLanguage "Python3.9";
+				];
+			];
+		];
+		rml:referenceFormulation rml:Dictionary;
+    rml:iterator "$.students[*]"
+  ];
 
-<TriplesMap4>
-	a rr:TriplesMap;
-    rr:logicalTable [ rr:sqlQuery """
+  rml:subjectMap [
+    rml:template "http://example.com/Student/{ID}/{FirstName}"
+  ];
 
-        SELECT "EMP".*, (CASE "job"
-            WHEN 'CLERK' THEN 'general-office'
-            WHEN 'NIGHTGUARD' THEN 'security'
-            WHEN 'ENGINEER' THEN 'engineering'
-        END) AS ROLE FROM "EMP"
+  rml:predicateObjectMap [
+    rml:predicate rdf:type;
+    rml:object foaf:Person;
+  ].
 
-        """ ];
-    rr:subjectMap [
-        rr:template "http://data.example.com/employee/{empno}";
-    ];
-    rr:predicateObjectMap [
-        rr:predicate ex:role;
-        rr:objectMap [ rr:template "http://data.example.com/roles/{ROLE}" ];
-    ].
+rml:Dictionary a rml:ReferenceFormulation;
+	kg4di:definedBy "Python".
```

### Comparing `morph_kgc-2.6.4/test/r2rml/R2RMLTC0014d/resource.db` & `morph_kgc-2.7.0/test/r2rml/R2RMLTC0014d/resource.db`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/r2rml/R2RMLTC0014d/resource.sql` & `morph_kgc-2.7.0/test/r2rml/R2RMLTC0014d/resource.sql`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/r2rml/R2RMLTC0014d/test_R2RMLTC0014d_SQLITE.py` & `morph_kgc-2.7.0/test/r2rml/R2RMLTC0014d/test_R2RMLTC0014d_SQLITE.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/r2rml/R2RMLTC0015a/mapping.ttl` & `morph_kgc-2.7.0/test/r2rml/R2RMLTC0015a/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/r2rml/R2RMLTC0015a/resource.db` & `morph_kgc-2.7.0/test/r2rml/R2RMLTC0015a/resource.db`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/r2rml/R2RMLTC0015a/test_R2RMLTC0015a_SQLITE.py` & `morph_kgc-2.7.0/test/r2rml/R2RMLTC0015a/test_R2RMLTC0015a_SQLITE.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/r2rml/R2RMLTC0015b/mapping.ttl` & `morph_kgc-2.7.0/test/r2rml/R2RMLTC0015b/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/r2rml/R2RMLTC0015b/resource.db` & `morph_kgc-2.7.0/test/r2rml/R2RMLTC0015b/resource.db`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/r2rml/R2RMLTC0015b/test_R2RMLTC0015b_SQLITE.py` & `morph_kgc-2.7.0/test/r2rml/R2RMLTC0015b/test_R2RMLTC0015b_SQLITE.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/r2rml/R2RMLTC0016a/mapping.ttl` & `morph_kgc-2.7.0/test/r2rml/R2RMLTC0016a/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/r2rml/R2RMLTC0016a/output.nq` & `morph_kgc-2.7.0/test/r2rml/R2RMLTC0016a/output.nq`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/r2rml/R2RMLTC0016a/resource.db` & `morph_kgc-2.7.0/test/r2rml/R2RMLTC0016a/resource.db`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/r2rml/R2RMLTC0016a/resource.sql` & `morph_kgc-2.7.0/test/r2rml/R2RMLTC0016a/resource.sql`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/r2rml/R2RMLTC0016a/test_R2RMLTC0016a_SQLITE.py` & `morph_kgc-2.7.0/test/r2rml/R2RMLTC0016a/test_R2RMLTC0016a_SQLITE.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/r2rml/R2RMLTC0016b/R2RMLTC0016b_SQLITE.py` & `morph_kgc-2.7.0/test/r2rml/R2RMLTC0016b/R2RMLTC0016b_SQLITE.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/r2rml/R2RMLTC0016b/mapping.ttl` & `morph_kgc-2.7.0/test/r2rml/R2RMLTC0016b/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/r2rml/R2RMLTC0016b/output.nq` & `morph_kgc-2.7.0/test/r2rml/R2RMLTC0016b/output.nq`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/r2rml/R2RMLTC0016b/resource.db` & `morph_kgc-2.7.0/test/r2rml/R2RMLTC0016b/resource.db`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/r2rml/R2RMLTC0016b/resource.sql` & `morph_kgc-2.7.0/test/r2rml/R2RMLTC0016b/resource.sql`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/r2rml/R2RMLTC0016c/R2RMLTC0016c_SQLITE.py` & `morph_kgc-2.7.0/test/r2rml/R2RMLTC0016c/R2RMLTC0016c_SQLITE.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/r2rml/R2RMLTC0016c/mapping.ttl` & `morph_kgc-2.7.0/test/r2rml/R2RMLTC0016c/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/r2rml/R2RMLTC0016c/output.nq` & `morph_kgc-2.7.0/test/r2rml/R2RMLTC0016c/output.nq`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/r2rml/R2RMLTC0016c/resource.db` & `morph_kgc-2.7.0/test/r2rml/R2RMLTC0016c/resource.db`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/r2rml/R2RMLTC0016c/resource.sql` & `morph_kgc-2.7.0/test/r2rml/R2RMLTC0016c/resource.sql`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/r2rml/R2RMLTC0016d/R2RMLTC0016d_SQLITE.py` & `morph_kgc-2.7.0/test/r2rml/R2RMLTC0016d/R2RMLTC0016d_SQLITE.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/r2rml/R2RMLTC0016d/mapping.ttl` & `morph_kgc-2.7.0/test/r2rml/R2RMLTC0016d/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/r2rml/R2RMLTC0016d/output.nq` & `morph_kgc-2.7.0/test/r2rml/R2RMLTC0016d/output.nq`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/r2rml/R2RMLTC0016d/resource.db` & `morph_kgc-2.7.0/test/r2rml/R2RMLTC0016d/resource.db`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/r2rml/R2RMLTC0016d/resource.sql` & `morph_kgc-2.7.0/test/r2rml/R2RMLTC0016d/resource.sql`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/r2rml/R2RMLTC0016e/R2RMLTC0016e_SQLITE.py` & `morph_kgc-2.7.0/test/r2rml/R2RMLTC0016e/R2RMLTC0016e_SQLITE.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/r2rml/R2RMLTC0016e/mapping.ttl` & `morph_kgc-2.7.0/test/r2rml/R2RMLTC0016e/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/r2rml/R2RMLTC0016e/output.nq` & `morph_kgc-2.7.0/test/r2rml/R2RMLTC0016e/output.nq`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/r2rml/R2RMLTC0016e/resource.db` & `morph_kgc-2.7.0/test/r2rml/R2RMLTC0016e/resource.db`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/r2rml/R2RMLTC0016e/resource.sql` & `morph_kgc-2.7.0/test/r2rml/R2RMLTC0016e/resource.sql`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/r2rml/R2RMLTC0018a/mapping.ttl` & `morph_kgc-2.7.0/test/r2rml/R2RMLTC0018a/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/r2rml/R2RMLTC0018a/output.nq` & `morph_kgc-2.7.0/test/r2rml/R2RMLTC0018a/output.nq`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/r2rml/R2RMLTC0018a/resource.db` & `morph_kgc-2.7.0/test/r2rml/R2RMLTC0018a/resource.db`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/r2rml/R2RMLTC0018a/test_R2RMLTC0018a_SQLITE.py` & `morph_kgc-2.7.0/test/r2rml/R2RMLTC0018a/test_R2RMLTC0018a_SQLITE.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/r2rml/R2RMLTC0019a/R2RMLTC0019a_SQLITE.py` & `morph_kgc-2.7.0/test/r2rml/R2RMLTC0019a/R2RMLTC0019a_SQLITE.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/r2rml/R2RMLTC0019a/mapping.ttl` & `morph_kgc-2.7.0/test/r2rml/R2RMLTC0019a/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/r2rml/R2RMLTC0019a/resource.db` & `morph_kgc-2.7.0/test/r2rml/R2RMLTC0019a/resource.db`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/r2rml/R2RMLTC0019b/R2RMLTC0019b_SQLITE.py` & `morph_kgc-2.7.0/test/r2rml/R2RMLTC0019b/R2RMLTC0019b_SQLITE.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/r2rml/R2RMLTC0019b/resource.db` & `morph_kgc-2.7.0/test/r2rml/R2RMLTC0019b/resource.db`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/r2rml/R2RMLTC0020a/R2RMLTC0020a_SQLITE.py` & `morph_kgc-2.7.0/test/r2rml/R2RMLTC0020a/R2RMLTC0020a_SQLITE.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/r2rml/R2RMLTC0020a/mapping.ttl` & `morph_kgc-2.7.0/test/r2rml/R2RMLTC0020a/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/r2rml/R2RMLTC0020a/output.nq` & `morph_kgc-2.7.0/test/r2rml/R2RMLTC0020a/output.nq`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/r2rml/R2RMLTC0020a/resource.db` & `morph_kgc-2.7.0/test/r2rml/R2RMLTC0020a/resource.db`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/r2rml/R2RMLTC0020b/R2RMLTC0020b_SQLITE.py` & `morph_kgc-2.7.0/test/r2rml/R2RMLTC0020b/R2RMLTC0020b_SQLITE.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/r2rml/R2RMLTC0020b/mapping.ttl` & `morph_kgc-2.7.0/test/r2rml/R2RMLTC0020b/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/r2rml/R2RMLTC0020b/resource.db` & `morph_kgc-2.7.0/test/r2rml/R2RMLTC0020b/resource.db`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/rml/csv/RMLTC0000/mapping.ttl` & `morph_kgc-2.7.0/test/rml-core/json/RMLTC0003c/mapping.ttl`

 * *Files 12% similar despite different names*

```diff
@@ -1,27 +1,25 @@
-@prefix rr: <http://www.w3.org/ns/r2rml#> .
 @prefix foaf: <http://xmlns.com/foaf/0.1/> .
 @prefix ex: <http://example.com/> .
 @prefix xsd: <http://www.w3.org/2001/XMLSchema#> .
-@prefix rml: <http://semweb.mmlab.be/ns/rml#> .
-@prefix ql: <http://semweb.mmlab.be/ns/ql#> .
-
+@prefix rml: <http://w3id.org/rml/> .
 @base <http://example.com/base/> .
 
-<TriplesMap1>
-  a rr:TriplesMap;
+<TriplesMap1> a rml:TriplesMap;
 
   rml:logicalSource [
-    rml:source "test/rml/csv/RMLTC0000/student.csv";
-    rml:referenceFormulation ql:CSV
-  ] ;
+    rml:source "test/rml-core/json/RMLTC0003c/student.json";
+    rml:referenceFormulation rml:JSONPath;
+    rml:iterator "$.students[*]"
+  ];
 
-  rr:subjectMap [
-    rr:template "http://example.com/{Name}"
+  rml:subjectMap [
+    rml:template "http://example.com/Student{ID}";
   ];
 
-  rr:predicateObjectMap [
-    rr:predicate foaf:name ;
-    rr:objectMap [
-      rml:reference "Name"
+  rml:predicateObjectMap [
+    rml:predicate foaf:name ;
+    rml:objectMap [
+      rml:template "{FirstName} {LastName}";
+      rml:termType rml:Literal;
     ]
   ].
```

### Comparing `morph_kgc-2.6.4/test/rml/csv/RMLTC0000/test_RMLTC0000_CSV.py` & `morph_kgc-2.7.0/test/rml-core/csv/RMLTC0000/test_RMLTC0000_CSV.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/rml/csv/RMLTC0001a/mapping.ttl` & `morph_kgc-2.7.0/test/rml-core/csv/RMLTC0004b/mapping.ttl`

 * *Files 15% similar despite different names*

```diff
@@ -1,28 +1,26 @@
-@prefix rr: <http://www.w3.org/ns/r2rml#> .
 @prefix foaf: <http://xmlns.com/foaf/0.1/> .
 @prefix ex: <http://example.com/> .
 @prefix xsd: <http://www.w3.org/2001/XMLSchema#> .
-@prefix rml: <http://semweb.mmlab.be/ns/rml#> .
-@prefix ql: <http://semweb.mmlab.be/ns/ql#> .
+@prefix rml: <http://w3id.org/rml/> .
 
 @base <http://example.com/base/> .
 
 <TriplesMap1>
-  a rr:TriplesMap;
+  a rml:TriplesMap;
 
   rml:logicalSource [
-    rml:source "test/rml/csv/RMLTC0001a/student.csv";
-    rml:referenceFormulation ql:CSV
+    rml:source "test/rml-core/csv/RMLTC0004b/student.csv";
+    rml:referenceFormulation rml:CSV
   ];
 
-  rr:subjectMap [
-    rr:template "http://example.com/{Name}"
+  rml:subjectMap [
+    rml:template "http://example.com/{Name}";
+    rml:termType rml:Literal
   ];
 
-  rr:predicateObjectMap [
-    rr:predicate foaf:name;
-    rr:objectMap [
+  rml:predicateObjectMap [
+    rml:predicate foaf:name;
+    rml:objectMap [
       rml:reference "Name"
     ]
   ].
-
```

### Comparing `morph_kgc-2.6.4/test/rml/csv/RMLTC0001a/test_RMLTC0001a_CSV.py` & `morph_kgc-2.7.0/test/rml-core/csv/RMLTC0001a/test_RMLTC0001a_CSV.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/rml/csv/RMLTC0001b/mapping.ttl` & `morph_kgc-2.7.0/test/rml-core/csv/RMLTC0020b/mapping.ttl`

 * *Files 14% similar despite different names*

```diff
@@ -1,27 +1,23 @@
-@prefix rr: <http://www.w3.org/ns/r2rml#> .
 @prefix foaf: <http://xmlns.com/foaf/0.1/> .
 @prefix ex: <http://example.com/> .
 @prefix xsd: <http://www.w3.org/2001/XMLSchema#> .
-@prefix rml: <http://semweb.mmlab.be/ns/rml#> .
-@prefix ql: <http://semweb.mmlab.be/ns/ql#> .
+@prefix rdf: <http://www.w3.org/1999/02/22-rdf-syntax-ns#> .
+@prefix rml:    <http://w3id.org/rml/> .
+@prefix ql:     <http://semweb.mmlab.be/ns/ql#> .
+
 @base <http://example.com/base/> .
 
 <TriplesMap1>
-  a rr:TriplesMap;
-
+  a rml:TriplesMap;
   rml:logicalSource [
-    rml:source "test/rml/csv/RMLTC0001b/student.csv";
-    rml:referenceFormulation ql:CSV
+    rml:source "test/rml-core/csv/RMLTC0020b/student.csv";
+    rml:referenceFormulation rml:CSV
   ];
 
-  rr:subjectMap [
-    rr:template "{Name}";
-    rr:termType rr:BlankNode
-  ];
+    rml:subjectMap [ rml:reference "Name"; rml:termType rml:IRI; ];
 
-  rr:predicateObjectMap [
-    rr:predicate foaf:name;
-    rr:objectMap [
-      rml:reference "Name"
-    ]
-  ].
+    rml:predicateObjectMap
+    [
+    	rml:predicate rdf:type;
+    	rml:object foaf:Person;
+    ].
```

### Comparing `morph_kgc-2.6.4/test/rml/csv/RMLTC0001b/test_RMLTC0001b_CSV.py` & `morph_kgc-2.7.0/test/rml-core/csv/RMLTC0001b/test_RMLTC0001b_CSV.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/rml/csv/RMLTC0002a/mapping.ttl` & `morph_kgc-2.7.0/test/rml-core/tabular/RMLTC0002a_STATA/mapping.ttl`

 * *Files 14% similar despite different names*

```diff
@@ -1,29 +1,27 @@
-@prefix rr: <http://www.w3.org/ns/r2rml#> .
 @prefix foaf: <http://xmlns.com/foaf/0.1/> .
 @prefix ex: <http://example.com/> .
 @prefix xsd: <http://www.w3.org/2001/XMLSchema#> .
-@prefix rml: <http://semweb.mmlab.be/ns/rml#> .
-@prefix ql: <http://semweb.mmlab.be/ns/ql#> .
+@prefix rml: <http://w3id.org/rml/> .
 @base <http://example.com/base/> .
 
-<TriplesMap1> a rr:TriplesMap;
+<TriplesMap1> a rml:TriplesMap;
 
   rml:logicalSource [
-    rml:source "test/rml/csv/RMLTC0002a/student.csv";
-    rml:referenceFormulation ql:CSV
+    rml:source "test/rml-core/tabular/RMLTC0002a_STATA/student.dta";
+    rml:referenceFormulation rml:CSV
   ];
 
-  rr:subjectMap [
-    rr:template "http://example.com/{ID}/{Name}";
-    rr:class foaf:Person
+  rml:subjectMap [
+    rml:template "http://example.com/{ID}/{Name}";
+    rml:class foaf:Person
   ];
 
-  rr:predicateObjectMap [
-    rr:predicate ex:id ;
-    rr:objectMap [ rml:reference "ID" ]
+  rml:predicateObjectMap [
+    rml:predicate ex:id ;
+    rml:objectMap [ rml:reference "ID" ]
   ];
 
-  rr:predicateObjectMap [
-    rr:predicate foaf:name ;
-    rr:objectMap [ rml:reference "Name" ]
+  rml:predicateObjectMap [
+    rml:predicate foaf:name ;
+    rml:objectMap [ rml:reference "Name" ]
   ].
```

### Comparing `morph_kgc-2.6.4/test/rml/csv/RMLTC0002a/test_RMLTC0002a_CSV.py` & `morph_kgc-2.7.0/test/rml-core/csv/RMLTC0002a/test_RMLTC0002a_CSV.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/rml/csv/RMLTC0002b/mapping.ttl` & `morph_kgc-2.7.0/test/rml-core/xml/RMLTC0007b/mapping.ttl`

 * *Files 15% similar despite different names*

```diff
@@ -1,24 +1,29 @@
-@prefix rr: <http://www.w3.org/ns/r2rml#> .
 @prefix foaf: <http://xmlns.com/foaf/0.1/> .
 @prefix ex: <http://example.com/> .
 @prefix xsd: <http://www.w3.org/2001/XMLSchema#> .
-@prefix rml: <http://semweb.mmlab.be/ns/rml#> .
-@prefix ql: <http://semweb.mmlab.be/ns/ql#> .
+@prefix rml: <http://w3id.org/rml/> .
+@prefix rdf: <http://www.w3.org/1999/02/22-rdf-syntax-ns#> .
 @base <http://example.com/base/> .
 
-<TriplesMap1> a rr:TriplesMap;
+<TriplesMap1> a rml:TriplesMap;
 
   rml:logicalSource [
-    rml:source "test/rml/csv/RMLTC0002b/student.csv";
-    rml:referenceFormulation ql:CSV
+    rml:source "test/rml-core/xml/RMLTC0007b/student.xml";
+    rml:referenceFormulation rml:XPath;
+    rml:iterator "/students/student"
   ];
 
-  rr:subjectMap [
-    rr:template "students{ID}";
-    rr:termType rr:BlankNode
+  rml:subjectMap [
+    rml:template "http://example.com/Student/{ID}/{FirstName}";
+    rml:graph ex:PersonGraph
   ];
 
-  rr:predicateObjectMap [
-    rr:predicate foaf:name;
-    rr:objectMap [ rml:reference "Name" ]
+  rml:predicateObjectMap [
+    rml:predicate rdf:type;
+    rml:object foaf:Person;
+  ];
+
+  rml:predicateObjectMap [
+    rml:predicate foaf:name;
+    rml:objectMap [ rml:reference "FirstName" ]
   ].
```

### Comparing `morph_kgc-2.6.4/test/rml/csv/RMLTC0002b/test_RMLTC0002b_CSV.py` & `morph_kgc-2.7.0/test/rml-core/csv/RMLTC0002b/test_RMLTC0002b_CSV.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/rml/csv/RMLTC0002c/mapping.ttl` & `morph_kgc-2.7.0/test/rml-core/csv/RMLTC0007h/mapping.ttl`

 * *Files 15% similar despite different names*

```diff
@@ -1,23 +1,24 @@
-@prefix rr: <http://www.w3.org/ns/r2rml#> .
 @prefix foaf: <http://xmlns.com/foaf/0.1/> .
 @prefix ex: <http://example.com/> .
 @prefix xsd: <http://www.w3.org/2001/XMLSchema#> .
-@prefix rml: <http://semweb.mmlab.be/ns/rml#> .
-@prefix ql: <http://semweb.mmlab.be/ns/ql#> .
+@prefix rml: <http://w3id.org/rml/> .
 @base <http://example.com/base/> .
 
-<TriplesMap1> a rr:TriplesMap;
+<TriplesMap1> a rml:TriplesMap;
 
   rml:logicalSource [
-    rml:source "test/rml/csv/RMLTC0002c/student.csv";
-    rml:referenceFormulation ql:CSV
+    rml:source "test/rml-core/csv/RMLTC0007h/student.csv";
+    rml:referenceFormulation rml:CSV
   ];
 
-  rr:subjectMap [
-    rr:template "http://example.com/{ID}/{Name}";
+  rml:subjectMap [
+    rml:template "http://example.com/Student/{ID}/{FirstName}";
+    rml:graphMap [ rml:reference "FirstName"; rml:termType rml:Literal; ]
   ];
 
-  rr:predicateObjectMap [
-    rr:predicate ex:id ;
-    rr:objectMap [ rml:reference "IDs" ]
+  rml:predicateObjectMap [
+    rml:predicate foaf:name;
+    rml:objectMap [
+      rml:reference "FirstName"
+    ]
   ].
```

### Comparing `morph_kgc-2.6.4/test/rml/csv/RMLTC0002c/test_RMLTC0002c_CSV.py` & `morph_kgc-2.7.0/test/rml-core/csv/RMLTC0002c/test_RMLTC0002c_CSV.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/rml/csv/RMLTC0002e/mapping.ttl` & `morph_kgc-2.7.0/test/rml-core/json/RMLTC0004b/mapping.ttl`

 * *Files 16% similar despite different names*

```diff
@@ -1,23 +1,27 @@
-@prefix rr: <http://www.w3.org/ns/r2rml#> .
 @prefix foaf: <http://xmlns.com/foaf/0.1/> .
 @prefix ex: <http://example.com/> .
 @prefix xsd: <http://www.w3.org/2001/XMLSchema#> .
-@prefix rml: <http://semweb.mmlab.be/ns/rml#> .
-@prefix ql: <http://semweb.mmlab.be/ns/ql#> .
+@prefix rml: <http://w3id.org/rml/> .
+
 @base <http://example.com/base/> .
 
-<TriplesMap1> a rr:TriplesMap;
+<TriplesMap1>
+  a rml:TriplesMap;
 
   rml:logicalSource [
-    rml:source "test/rml/csv/RMLTC0002e/student2.csv";
-    rml:referenceFormulation ql:CSV
+    rml:source "test/rml-core/json/RMLTC0004b/student.json";
+    rml:referenceFormulation rml:JSONPath;
+    rml:iterator "$.students[*]"
   ];
 
-  rr:subjectMap [
-    rr:template "http://example.com/{ID}/{Name}";
+  rml:subjectMap [
+    rml:template "http://example.com/{Name}";
+    rml:termType rml:Literal
   ];
 
-  rr:predicateObjectMap [
-    rr:predicate ex:id ;
-    rr:objectMap [ rml:reference "ID" ]
+  rml:predicateObjectMap [
+    rml:predicate foaf:name;
+    rml:objectMap [
+      rml:reference "Name"
+    ]
   ].
```

### Comparing `morph_kgc-2.6.4/test/rml/csv/RMLTC0002e/test_RMLTC0002e_CSV.py` & `morph_kgc-2.7.0/test/rml-core/csv/RMLTC0002e/test_RMLTC0002e_CSV.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/rml/csv/RMLTC0003c/mapping.ttl` & `morph_kgc-2.7.0/test/rml-core/csv/RMLTC0001a/mapping.ttl`

 * *Files 14% similar despite different names*

```diff
@@ -1,26 +1,26 @@
-@prefix rr: <http://www.w3.org/ns/r2rml#> .
 @prefix foaf: <http://xmlns.com/foaf/0.1/> .
 @prefix ex: <http://example.com/> .
 @prefix xsd: <http://www.w3.org/2001/XMLSchema#> .
-@prefix rml: <http://semweb.mmlab.be/ns/rml#> .
-@prefix ql: <http://semweb.mmlab.be/ns/ql#> .
+@prefix rml: <http://w3id.org/rml/> .
+
 @base <http://example.com/base/> .
 
-<TriplesMap1> a rr:TriplesMap;
+<TriplesMap1>
+  a rml:TriplesMap;
 
   rml:logicalSource [
-    rml:source "test/rml/csv/RMLTC0003c/student.csv";
-    rml:referenceFormulation ql:CSV
+    rml:source "test/rml-core/csv/RMLTC0001a/student.csv";
+    rml:referenceFormulation rml:CSV
   ];
 
-  rr:subjectMap [
-    rr:template "http://example.com/Student{ID}";
+  rml:subjectMap [
+    rml:template "http://example.com/{Name}"
   ];
 
-  rr:predicateObjectMap [
-    rr:predicate foaf:name ;
-    rr:objectMap [
-      rr:template "{FirstName} {LastName}";
-      rr:termType rr:Literal;
+  rml:predicateObjectMap [
+    rml:predicate foaf:name;
+    rml:objectMap [
+      rml:reference "Name"
     ]
   ].
+
```

### Comparing `morph_kgc-2.6.4/test/rml/csv/RMLTC0003c/test_RMLTC0003c_CSV.py` & `morph_kgc-2.7.0/test/rml-core/csv/RMLTC0003c/test_RMLTC0003c_CSV.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/rml/csv/RMLTC0004a/mapping.ttl` & `morph_kgc-2.7.0/test/rml-core/tabular/RMLTC0002a_PARQUET/mapping.ttl`

 * *Files 17% similar despite different names*

```diff
@@ -1,45 +1,27 @@
-@prefix rr: <http://www.w3.org/ns/r2rml#> .
 @prefix foaf: <http://xmlns.com/foaf/0.1/> .
 @prefix ex: <http://example.com/> .
 @prefix xsd: <http://www.w3.org/2001/XMLSchema#> .
-@prefix rml: <http://semweb.mmlab.be/ns/rml#> .
-@prefix ql: <http://semweb.mmlab.be/ns/ql#> .
+@prefix rml: <http://w3id.org/rml/> .
 @base <http://example.com/base/> .
 
-<TriplesMap1> a rr:TriplesMap;
+<TriplesMap1> a rml:TriplesMap;
 
   rml:logicalSource [
-    rml:source "test/rml/csv/RMLTC0004a/student_sport.csv";
-    rml:referenceFormulation ql:CSV
+    rml:source "test/rml-core/tabular/RMLTC0002a_PARQUET/student.parquet";
+    rml:referenceFormulation rml:CSV
   ];
 
-  rr:subjectMap [
-    rr:template "http://example.com/{Student}";
-    rr:class ex:Student
+  rml:subjectMap [
+    rml:template "http://example.com/{ID}/{Name}";
+    rml:class foaf:Person
   ];
 
-  rr:predicateObjectMap [
-    rr:predicate foaf:name ;
-    rr:objectMap [
-      rml:reference "Student"
-    ]
-  ].
-
-<TriplesMap2> a rr:TriplesMap;
-
-  rml:logicalSource [
-    rml:source "test/rml/csv/RMLTC0004a/student_sport.csv";
-    rml:referenceFormulation ql:CSV
-  ];
-
-  rr:subjectMap [
-    rr:template "http://example.com/{Sport}";
-    rr:class ex:Sport
+  rml:predicateObjectMap [
+    rml:predicate ex:id ;
+    rml:objectMap [ rml:reference "ID" ]
   ];
 
-  rr:predicateObjectMap [
-    rr:predicate foaf:name ;
-    rr:objectMap [
-      rml:reference "Sport"
-    ]
+  rml:predicateObjectMap [
+    rml:predicate foaf:name ;
+    rml:objectMap [ rml:reference "Name" ]
   ].
```

### Comparing `morph_kgc-2.6.4/test/rml/csv/RMLTC0004a/test_RMLTC0004a_CSV.py` & `morph_kgc-2.7.0/test/rml-core/csv/RMLTC0004a/test_RMLTC0004a_CSV.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/rml/csv/RMLTC0004b/mapping.ttl` & `morph_kgc-2.7.0/test/rml-core/csv/RMLTC0002b/mapping.ttl`

 * *Files 14% similar despite different names*

```diff
@@ -1,28 +1,22 @@
-@prefix rr: <http://www.w3.org/ns/r2rml#> .
 @prefix foaf: <http://xmlns.com/foaf/0.1/> .
 @prefix ex: <http://example.com/> .
 @prefix xsd: <http://www.w3.org/2001/XMLSchema#> .
-@prefix rml: <http://semweb.mmlab.be/ns/rml#> .
-@prefix ql: <http://semweb.mmlab.be/ns/ql#> .
-
+@prefix rml: <http://w3id.org/rml/> .
 @base <http://example.com/base/> .
 
-<TriplesMap1>
-  a rr:TriplesMap;
+<TriplesMap1> a rml:TriplesMap;
 
   rml:logicalSource [
-    rml:source "test/rml/csv/RMLTC0004b/student.csv";
-    rml:referenceFormulation ql:CSV
+    rml:source "test/rml-core/csv/RMLTC0002b/student.csv";
+    rml:referenceFormulation rml:CSV
   ];
 
-  rr:subjectMap [
-    rr:template "http://example.com/{Name}";
-    rr:termType rr:Literal
+  rml:subjectMap [
+    rml:template "students{ID}";
+    rml:termType rml:BlankNode
   ];
 
-  rr:predicateObjectMap [
-    rr:predicate foaf:name;
-    rr:objectMap [
-      rml:reference "Name"
-    ]
+  rml:predicateObjectMap [
+    rml:predicate foaf:name;
+    rml:objectMap [ rml:reference "Name" ]
   ].
```

### Comparing `morph_kgc-2.6.4/test/rml/csv/RMLTC0004b/test_RMLTC0004b_CSV.py` & `morph_kgc-2.7.0/test/rml-core/csv/RMLTC0004b/test_RMLTC0004b_CSV.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/rml/csv/RMLTC0005a/mapping.ttl` & `morph_kgc-2.7.0/test/rml-core/csv/RMLTC0005a/mapping.ttl`

 * *Files 16% similar despite different names*

```diff
@@ -1,24 +1,22 @@
-@prefix rr: <http://www.w3.org/ns/r2rml#> .
 @prefix foaf: <http://xmlns.com/foaf/0.1/> .
 @prefix ex: <http://example.com/> .
 @prefix xsd: <http://www.w3.org/2001/XMLSchema#> .
-@prefix rml: <http://semweb.mmlab.be/ns/rml#> .
-@prefix ql: <http://semweb.mmlab.be/ns/ql#> .
+@prefix rml: <http://w3id.org/rml/> .
 @base <http://example.com/base/> .
 
-<TriplesMap1> a rr:TriplesMap;
+<TriplesMap1> a rml:TriplesMap;
 
   rml:logicalSource [
-    rml:source "test/rml/csv/RMLTC0005a/ious.csv";
-    rml:referenceFormulation ql:CSV
+    rml:source "test/rml-core/csv/RMLTC0005a/ious.csv";
+    rml:referenceFormulation rml:CSV
   ];
 
-  rr:subjectMap [
-    rr:template "http://example.com/{fname};{lname}";
-    rr:class foaf:Person;
+  rml:subjectMap [
+    rml:template "http://example.com/{fname};{lname}";
+    rml:class foaf:Person;
   ];
 
-  rr:predicateObjectMap [
-    rr:predicate ex:owes;
-    rr:objectMap [ rml:reference "amount"; ]
+  rml:predicateObjectMap [
+    rml:predicate ex:owes;
+    rml:objectMap [ rml:reference "amount"; ]
   ].
```

### Comparing `morph_kgc-2.6.4/test/rml/csv/RMLTC0005a/test_RMLTC0005a_CSV.py` & `morph_kgc-2.7.0/test/rml-core/csv/RMLTC0005a/test_RMLTC0005a_CSV.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/rml/csv/RMLTC0006a/mapping.ttl` & `morph_kgc-2.7.0/test/rml-core/xml/rml_spec_example_section_5/mapping.ttl`

 * *Files 22% similar despite different names*

```diff
@@ -1,24 +1,27 @@
-@prefix rr: <http://www.w3.org/ns/r2rml#> .
-@prefix foaf: <http://xmlns.com/foaf/0.1/> .
-@prefix ex: <http://example.com/> .
-@prefix xsd: <http://www.w3.org/2001/XMLSchema#> .
-@prefix rml: <http://semweb.mmlab.be/ns/rml#> .
-@prefix ql: <http://semweb.mmlab.be/ns/ql#> .
-@base <http://example.com/base/> .
-
-<TriplesMap1> a rr:TriplesMap;
+@prefix rr: <http://www.w3.org/ns/r2rml#>.
+@prefix rml: <http://w3id.org/rml/>.
+@prefix ex: <http://example.com/ns#>.
+@prefix ql: <http://semweb.mmlab.be/ns/ql#>.
+@prefix xsd: <http://www.w3.org/2001/XMLSchema#>.
+@prefix rdfs: <http://www.w3.org/2000/01/rdf-schema#>.
+@base <http://example.com/ns#>.
 
+<#TransportMapping> a rml:TriplesMap;
   rml:logicalSource [
-    rml:source "test/rml/csv/RMLTC0006a/student.csv";
-    rml:referenceFormulation ql:CSV
+    rml:source "test/rml-core/xml/rml_spec_example_section_5/Transport.xml" ;
+    rml:iterator "/transport/bus/route/stop";
+    rml:referenceFormulation rml:XPath;
   ];
 
-  rr:subjectMap [
-    rr:constant ex:BadStudent;
-    rr:graphMap [ rr:constant <http://example.com/graph/student> ];
+  rml:subjectMap [
+    rml:template
+      "http://trans.example.com/stop/{@id}";
+    rml:class ex:Stop
   ];
 
-  rr:predicateObjectMap [
-    rr:predicateMap [ rr:constant ex:description ];
-    rr:objectMap [ rr:constant "Bad Student"; ]
+  rml:predicateObjectMap [
+    rml:predicate rdfs:label;
+    rml:objectMap [
+      rml:reference "."
+    ]
   ].
```

### Comparing `morph_kgc-2.6.4/test/rml/csv/RMLTC0006a/test_RMLTC0006a_CSV.py` & `morph_kgc-2.7.0/test/rml-core/csv/RMLTC0006a/test_RMLTC0006a_CSV.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/rml/csv/RMLTC0007a/mapping.ttl` & `morph_kgc-2.7.0/test/rml-core/json/RMLTC0019a/mapping.ttl`

 * *Files 22% similar despite different names*

```diff
@@ -1,24 +1,25 @@
-@prefix rr: <http://www.w3.org/ns/r2rml#> .
 @prefix foaf: <http://xmlns.com/foaf/0.1/> .
+@prefix rdfs: <http://www.w3.org/2000/01/rdf-schema#> .
 @prefix ex: <http://example.com/> .
 @prefix xsd: <http://www.w3.org/2001/XMLSchema#> .
-@prefix rml: <http://semweb.mmlab.be/ns/rml#> .
-@prefix ql: <http://semweb.mmlab.be/ns/ql#> .
-@prefix rdf: <http://www.w3.org/1999/02/22-rdf-syntax-ns#> .
+@prefix rml: <http://w3id.org/rml/> .
+
 @base <http://example.com/base/> .
 
-<TriplesMap1> a rr:TriplesMap;
+<TriplesMap1>
+  a rml:TriplesMap;
 
   rml:logicalSource [
-    rml:source "test/rml/csv/RMLTC0007a/student.csv";
-    rml:referenceFormulation ql:CSV
+    rml:source "test/rml-core/json/RMLTC0019a/persons.json";
+    rml:referenceFormulation rml:JSONPath;
+    rml:iterator "$.persons[*]"
   ];
 
-  rr:subjectMap [
-    rr:template "http://example.com/Student/{ID}/{FirstName}"
-  ];
+  rml:subjectMap [ rml:reference "FirstName" ];
 
-  rr:predicateObjectMap [
-    rr:predicate rdf:type;
-    rr:object foaf:Person;
-  ].
+  rml:predicateObjectMap [
+    rml:predicate foaf:name;
+    rml:objectMap [
+      rml:reference "FirstName"
+    ]
+  ] .
```

### Comparing `morph_kgc-2.6.4/test/rml/csv/RMLTC0007a/test_RMLTC0007a_CSV.py` & `morph_kgc-2.7.0/test/rml-core/csv/RMLTC0007a/test_RMLTC0007a_CSV.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/rml/csv/RMLTC0007b/mapping.ttl` & `morph_kgc-2.7.0/test/rml-core/csv/RMLTC0007b/mapping.ttl`

 * *Files 15% similar despite different names*

```diff
@@ -1,30 +1,28 @@
-@prefix rr: <http://www.w3.org/ns/r2rml#> .
 @prefix foaf: <http://xmlns.com/foaf/0.1/> .
 @prefix ex: <http://example.com/> .
 @prefix xsd: <http://www.w3.org/2001/XMLSchema#> .
-@prefix rml: <http://semweb.mmlab.be/ns/rml#> .
-@prefix ql: <http://semweb.mmlab.be/ns/ql#> .
+@prefix rml: <http://w3id.org/rml/> .
 @prefix rdf: <http://www.w3.org/1999/02/22-rdf-syntax-ns#> .
 @base <http://example.com/base/> .
 
-<TriplesMap1> a rr:TriplesMap;
+<TriplesMap1> a rml:TriplesMap;
 
   rml:logicalSource [
-    rml:source "test/rml/csv/RMLTC0007b/student.csv";
-    rml:referenceFormulation ql:CSV
+    rml:source "test/rml-core/csv/RMLTC0007b/student.csv";
+    rml:referenceFormulation rml:CSV
   ];
 
-  rr:subjectMap [
-    rr:template "http://example.com/Student/{ID}/{FirstName}";
-    rr:graph ex:PersonGraph
+  rml:subjectMap [
+    rml:template "http://example.com/Student/{ID}/{FirstName}";
+    rml:graph ex:PersonGraph
   ];
 
-  rr:predicateObjectMap [
-    rr:predicate rdf:type;
-    rr:object foaf:Person;
+  rml:predicateObjectMap [
+    rml:predicate rdf:type;
+    rml:object foaf:Person;
   ];
 
-  rr:predicateObjectMap [
-    rr:predicate foaf:name;
-    rr:objectMap [ rml:reference "FirstName" ]
+  rml:predicateObjectMap [
+    rml:predicate foaf:name;
+    rml:objectMap [ rml:reference "FirstName" ]
   ].
```

### Comparing `morph_kgc-2.6.4/test/rml/csv/RMLTC0007b/test_RMLTC0007b_CSV.py` & `morph_kgc-2.7.0/test/rml-core/csv/RMLTC0007b/test_RMLTC0007b_CSV.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/rml/csv/RMLTC0007c/mapping.ttl` & `morph_kgc-2.7.0/test/rml-core/json/RMLTC0019b/mapping.ttl`

 * *Files 17% similar despite different names*

```diff
@@ -1,29 +1,25 @@
-@prefix rr: <http://www.w3.org/ns/r2rml#> .
 @prefix foaf: <http://xmlns.com/foaf/0.1/> .
+@prefix rdfs: <http://www.w3.org/2000/01/rdf-schema#> .
 @prefix ex: <http://example.com/> .
 @prefix xsd: <http://www.w3.org/2001/XMLSchema#> .
-@prefix rml: <http://semweb.mmlab.be/ns/rml#> .
-@prefix ql: <http://semweb.mmlab.be/ns/ql#> .
+@prefix rml: <http://w3id.org/rml/> .
+
 @base <http://example.com/base/> .
 
-<TriplesMap1> a rr:TriplesMap;
+<TriplesMap1>
+  a rml:TriplesMap;
 
   rml:logicalSource [
-    rml:source "test/rml/csv/RMLTC0007c/student.csv";
-    rml:referenceFormulation ql:CSV
-  ];
-
-  rr:subjectMap [
-    rr:template "http://example.com/Student/{ID}/{FirstName}";
-    rr:class foaf:Person, ex:Student
+    rml:source "test/rml-core/json/RMLTC0019b/persons.json";
+    rml:referenceFormulation rml:JSONPath;
+    rml:iterator "$.persons[*]"
   ];
 
-  rr:predicateObjectMap [
-    rr:predicate ex:id ;
-    rr:objectMap [ rml:reference "ID";  ]
-  ];
+  rml:subjectMap [ rml:reference "FirstName" ];
 
-  rr:predicateObjectMap [
-    rr:predicate foaf:name;
-    rr:objectMap [ rml:reference "FirstName" ]
-  ].
+  rml:predicateObjectMap [
+    rml:predicate foaf:name;
+    rml:objectMap [
+      rml:reference "FirstName"
+    ]
+  ] .
```

### Comparing `morph_kgc-2.6.4/test/rml/csv/RMLTC0007c/test_RMLTC0007c_CSV.py` & `morph_kgc-2.7.0/test/rml-core/csv/RMLTC0007c/test_RMLTC0007c_CSV.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/rml/csv/RMLTC0007d/mapping.ttl` & `morph_kgc-2.7.0/test/rml-core/json/RMLTC0007b/mapping.ttl`

 * *Files 14% similar despite different names*

```diff
@@ -1,39 +1,29 @@
-@prefix rr: <http://www.w3.org/ns/r2rml#> .
 @prefix foaf: <http://xmlns.com/foaf/0.1/> .
 @prefix ex: <http://example.com/> .
 @prefix xsd: <http://www.w3.org/2001/XMLSchema#> .
-@prefix rml: <http://semweb.mmlab.be/ns/rml#> .
-@prefix ql: <http://semweb.mmlab.be/ns/ql#> .
+@prefix rml: <http://w3id.org/rml/> .
 @prefix rdf: <http://www.w3.org/1999/02/22-rdf-syntax-ns#> .
 @base <http://example.com/base/> .
 
-<TriplesMap1> a rr:TriplesMap;
+<TriplesMap1> a rml:TriplesMap;
 
   rml:logicalSource [
-    rml:source "test/rml/csv/RMLTC0007d/student.csv";
-    rml:referenceFormulation ql:CSV
+    rml:source "test/rml-core/json/RMLTC0007b/student.json";
+    rml:referenceFormulation rml:JSONPath;
+    rml:iterator "$.students[*]"
   ];
 
-  rr:subjectMap [
-    rr:template "http://example.com/Student/{ID}/{FirstName}"
+  rml:subjectMap [
+    rml:template "http://example.com/Student/{ID}/{FirstName}";
+    rml:graph ex:PersonGraph
   ];
 
-  rr:predicateObjectMap [
-    rr:predicate rdf:type;
-    rr:object foaf:Person;
+  rml:predicateObjectMap [
+    rml:predicate rdf:type;
+    rml:object foaf:Person;
   ];
 
-  rr:predicateObjectMap [
-    rr:predicate rdf:type;
-    rr:object ex:Student;
-  ];
-
-  rr:predicateObjectMap [
-    rr:predicate ex:id;
-    rr:objectMap [ rml:reference "ID" ]
-  ];
-
-  rr:predicateObjectMap [
-    rr:predicate foaf:name;
-    rr:objectMap [ rml:reference "FirstName" ]
+  rml:predicateObjectMap [
+    rml:predicate foaf:name;
+    rml:objectMap [ rml:reference "FirstName" ]
   ].
```

### Comparing `morph_kgc-2.6.4/test/rml/csv/RMLTC0007d/test_RMLTC0007d_CSV.py` & `morph_kgc-2.7.0/test/rml-core/csv/RMLTC0007d/test_RMLTC0007d_CSV.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/rml/csv/RMLTC0007e/mapping.ttl` & `morph_kgc-2.7.0/test/rml-core/xml/RMLTC0005a/mapping.ttl`

 * *Files 16% similar despite different names*

```diff
@@ -1,31 +1,23 @@
-@prefix rr: <http://www.w3.org/ns/r2rml#> .
 @prefix foaf: <http://xmlns.com/foaf/0.1/> .
 @prefix ex: <http://example.com/> .
 @prefix xsd: <http://www.w3.org/2001/XMLSchema#> .
-@prefix rml: <http://semweb.mmlab.be/ns/rml#> .
-@prefix ql: <http://semweb.mmlab.be/ns/ql#> .
+@prefix rml: <http://w3id.org/rml/> .
 @base <http://example.com/base/> .
 
-<TriplesMap1> a rr:TriplesMap;
+<TriplesMap1> a rml:TriplesMap;
 
   rml:logicalSource [
-    rml:source "test/rml/csv/RMLTC0007e/student.csv";
-    rml:referenceFormulation ql:CSV
+    rml:source "test/rml-core/xml/RMLTC0005a/ious.xml";
+    rml:referenceFormulation rml:XPath;
+    rml:iterator "/persons/person"
   ];
 
-  rr:subjectMap [
-    rr:template "http://example.com/Student/{ID}/{Name}";
-    rr:graph ex:PersonGraph ;
-    rr:class foaf:Person
+  rml:subjectMap [
+    rml:template "http://example.com/{fname};{lname}";
+    rml:class foaf:Person;
   ];
 
-  rr:predicateObjectMap [
-    rr:predicate ex:id ;
-    rr:objectMap [ rml:reference "ID"; ]
-  ];
-
-  rr:predicateObjectMap
-    [
-      rr:predicate		foaf:name ;
-      rr:objectMap		[ rml:reference "Name" ]
-    ].
+  rml:predicateObjectMap [
+    rml:predicate ex:owes;
+    rml:objectMap [ rml:reference "amount"; ]
+  ].
```

### Comparing `morph_kgc-2.6.4/test/rml/csv/RMLTC0007e/test_RMLTC0007e_CSV.py` & `morph_kgc-2.7.0/test/rml-core/csv/RMLTC0007e/test_RMLTC0007e_CSV.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/rml/csv/RMLTC0007f/mapping.ttl` & `morph_kgc-2.7.0/test/rml-core/xml/RMLTC0009a/mapping.ttl`

 * *Files 18% similar despite different names*

```diff
@@ -1,35 +1,51 @@
-@prefix rr: <http://www.w3.org/ns/r2rml#> .
 @prefix foaf: <http://xmlns.com/foaf/0.1/> .
 @prefix ex: <http://example.com/> .
 @prefix xsd: <http://www.w3.org/2001/XMLSchema#> .
-@prefix rml: <http://semweb.mmlab.be/ns/rml#> .
-@prefix ql: <http://semweb.mmlab.be/ns/ql#> .
-@prefix rdf: <http://www.w3.org/1999/02/22-rdf-syntax-ns#> .
+@prefix rml: <http://w3id.org/rml/> .
+@prefix activity: <http://example.com/activity/> .
+@prefix rdfs: <http://www.w3.org/2000/01/rdf-schema#> .
 @base <http://example.com/base/> .
 
-<TriplesMap1> a rr:TriplesMap;
+<TriplesMap1>
+  a rml:TriplesMap;
 
   rml:logicalSource [
-    rml:source "test/rml/csv/RMLTC0007f/student.csv";
-    rml:referenceFormulation ql:CSV
+    rml:source "test/rml-core/xml/RMLTC0009a/student.xml";
+    rml:referenceFormulation rml:XPath;
+    rml:iterator "/students/student"
   ];
 
-  rr:subjectMap [
-    rr:template "http://example.com/Student/{ID}/{FirstName}";
-    rr:graph ex:PersonGraph
-  ];
+  rml:subjectMap [ rml:template "http://example.com/resource/student_{ID}" ];
 
-  rr:predicateObjectMap [
-    rr:predicate rdf:type;
-    rr:object foaf:Person
-  ];
+  rml:predicateObjectMap [
+    rml:predicate foaf:name ;
+    rml:objectMap [ rml:reference "Name" ]
+  ] ;
+
+  rml:predicateObjectMap [
+    rml:predicate <http://example.com/ontology/practises> ;
+    rml:objectMap [
+      a rml:RefObjectMap ;
+      rml:parentTriplesMap <TriplesMap2>;
+      rml:joinCondition [
+        rml:child "Sport" ;
+        rml:parent "ID" ;
+      ]
+    ]
+  ] .
+
+<TriplesMap2>
+  a rml:TriplesMap;
 
-  rr:predicateObjectMap [
-    rr:predicate ex:id ;
-    rr:objectMap [ rml:reference "ID";  ]
+  rml:logicalSource [
+    rml:source "test/rml-core/xml/RMLTC0009a/sport.xml";
+    rml:referenceFormulation rml:XPath;
+    rml:iterator "/sports/sport"
   ];
 
-  rr:predicateObjectMap [
-    rr:predicate foaf:name ;
-    rr:objectMap [ rml:reference "FirstName" ]
+  rml:subjectMap [ rml:template "http://example.com/resource/sport_{ID}" ];
+
+  rml:predicateObjectMap [
+    rml:predicate rdfs:label ;
+    rml:objectMap [ rml:reference "Name" ];
   ].
```

### Comparing `morph_kgc-2.6.4/test/rml/csv/RMLTC0007f/test_RMLTC0007f_CSV.py` & `morph_kgc-2.7.0/test/rml-core/csv/RMLTC0007f/test_RMLTC0007f_CSV.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/rml/csv/RMLTC0007g/mapping.ttl` & `morph_kgc-2.7.0/test/rml-core/json/RMLTC0020b/mapping.ttl`

 * *Files 14% similar despite different names*

```diff
@@ -1,26 +1,24 @@
-@prefix rr: <http://www.w3.org/ns/r2rml#> .
 @prefix foaf: <http://xmlns.com/foaf/0.1/> .
 @prefix ex: <http://example.com/> .
 @prefix xsd: <http://www.w3.org/2001/XMLSchema#> .
-@prefix rml: <http://semweb.mmlab.be/ns/rml#> .
-@prefix ql: <http://semweb.mmlab.be/ns/ql#> .
-@base <http://example.com/base/> .
+@prefix rdf: <http://www.w3.org/1999/02/22-rdf-syntax-ns#> .
+@prefix rml:    <http://w3id.org/rml/> .
+@prefix ql:     <http://semweb.mmlab.be/ns/ql#> .
 
-<TriplesMap1> a rr:TriplesMap;
+@base <http://example.com/base/> .
 
+<TriplesMap1>
+  a rml:TriplesMap;
   rml:logicalSource [
-    rml:source "test/rml/csv/RMLTC0007g/student.csv";
-    rml:referenceFormulation ql:CSV
+    rml:source "test/rml-core/json/RMLTC0020b/student.json";
+    rml:referenceFormulation rml:JSONPath;
+    rml:iterator "$.students[*]"
   ];
 
-  rr:subjectMap [
-    rr:template "http://example.com/Student/{ID}/{FirstName}";
-    rr:graph rr:defaultGraph
-  ];
+    rml:subjectMap [ rml:reference "Name"; rml:termType rml:IRI; ];
 
-  rr:predicateObjectMap [
-    rr:predicate foaf:name;
-    rr:objectMap [
-      rml:reference "FirstName"
-    ]
-  ].
+    rml:predicateObjectMap
+    [
+    	rml:predicate rdf:type;
+    	rml:object foaf:Person;
+    ].
```

### Comparing `morph_kgc-2.6.4/test/rml/csv/RMLTC0007g/test_RMLTC0007g_CSV.py` & `morph_kgc-2.7.0/test/rml-core/csv/RMLTC0007g/test_RMLTC0007g_CSV.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/rml/csv/RMLTC0007h/mapping.ttl` & `morph_kgc-2.7.0/test/rml-core/csv/RMLTC0008c/mapping.ttl`

 * *Files 16% similar despite different names*

```diff
@@ -1,26 +1,22 @@
-@prefix rr: <http://www.w3.org/ns/r2rml#> .
 @prefix foaf: <http://xmlns.com/foaf/0.1/> .
 @prefix ex: <http://example.com/> .
 @prefix xsd: <http://www.w3.org/2001/XMLSchema#> .
-@prefix rml: <http://semweb.mmlab.be/ns/rml#> .
-@prefix ql: <http://semweb.mmlab.be/ns/ql#> .
+@prefix rml: <http://w3id.org/rml/> .
+@prefix activity: <http://example.com/activity/> .
 @base <http://example.com/base/> .
 
-<TriplesMap1> a rr:TriplesMap;
+<TriplesMap1>
+  a rml:TriplesMap;
 
   rml:logicalSource [
-    rml:source "test/rml/csv/RMLTC0007h/student.csv";
-    rml:referenceFormulation ql:CSV
+    rml:source "test/rml-core/csv/RMLTC0008c/student.csv";
+    rml:referenceFormulation rml:CSV
   ];
 
-  rr:subjectMap [
-    rr:template "http://example.com/Student/{ID}/{FirstName}";
-    rr:graphMap [ rml:reference "FirstName"; rr:termType rr:Literal; ]
-  ];
+  rml:subjectMap [ rml:template "http://example.com/Student/{ID}/{Name}" ];
 
-  rr:predicateObjectMap [
-    rr:predicate foaf:name;
-    rr:objectMap [
-      rml:reference "FirstName"
-    ]
-  ].
+  rml:predicateObjectMap [
+    rml:predicate foaf:name ;
+    rml:predicate ex:name ;
+    rml:objectMap [ rml:reference "Name" ]
+  ] .
```

### Comparing `morph_kgc-2.6.4/test/rml/csv/RMLTC0007h/test_RMLTC0007h_CSV.py` & `morph_kgc-2.7.0/test/rml-core/csv/RMLTC0007h/test_RMLTC0007h_CSV.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/rml/csv/RMLTC0008a/mapping.ttl` & `morph_kgc-2.7.0/test/rml-core/xml/RMLTC0012a/mapping.ttl`

 * *Files 16% similar despite different names*

```diff
@@ -1,41 +1,32 @@
-@prefix rr: <http://www.w3.org/ns/r2rml#> .
 @prefix foaf: <http://xmlns.com/foaf/0.1/> .
 @prefix ex: <http://example.com/> .
 @prefix xsd: <http://www.w3.org/2001/XMLSchema#> .
-@prefix rml: <http://semweb.mmlab.be/ns/rml#> .
-@prefix ql: <http://semweb.mmlab.be/ns/ql#> .
-@prefix rdf: <http://www.w3.org/1999/02/22-rdf-syntax-ns#> .
+@prefix rml: <http://w3id.org/rml/> .
+
 @base <http://example.com/base/> .
 
 <TriplesMap1>
-  a rr:TriplesMap;
+  a rml:TriplesMap;
 
   rml:logicalSource [
-    rml:source "test/rml/csv/RMLTC0008a/student.csv";
-    rml:referenceFormulation ql:CSV
-  ];
-
-  rr:subjectMap [
-    rr:template "http://example.com/Student/{ID}/{Name}";
-    rr:graphMap [ rr:template "http://example.com/graph/Student/{ID}/{Name}" ]
+    rml:source "test/rml-core/xml/RMLTC0012a/persons.xml";
+    rml:referenceFormulation rml:XPath;
+    rml:iterator "/Persons/Person"
   ];
 
-  rr:predicateObjectMap [
-    rr:predicate rdf:type ;
-    rr:object foaf:Person;
-  ];
-
-  rr:predicateObjectMap [
-    rr:predicate ex:id ;
-    rr:objectMap [ rml:reference "ID" ]
-  ];
+  rml:subjectMap [ rml:template "{fname}{lname}{amount}"; rml:termType rml:BlankNode; ];
 
-  rr:predicateObjectMap [
-    rr:predicate foaf:name ;
-    rr:objectMap [ rml:reference "Name" ]
+  rml:predicateObjectMap [
+    rml:predicate foaf:name ;
+    rml:objectMap [
+      rml:template "{fname} {lname}";
+      rml:termType rml:Literal ;
+    ]
   ];
 
-  rr:predicateObjectMap [
-    rr:predicate ex:Sport ;
-    rr:objectMap [ rml:reference "Sport" ]
-  ] .
+  rml:predicateObjectMap [
+    rml:predicate ex:amount ;
+    rml:objectMap    [
+      rml:reference "amount";
+    ]
+  ].
```

### Comparing `morph_kgc-2.6.4/test/rml/csv/RMLTC0008a/output.nq` & `morph_kgc-2.7.0/test/rml-core/csv/RMLTC0008a/output.nq`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/rml/csv/RMLTC0008a/test_RMLTC0008a_CSV.py` & `morph_kgc-2.7.0/test/rml-core/csv/RMLTC0008a/test_RMLTC0008a_CSV.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/rml/csv/RMLTC0008b/mapping.ttl` & `morph_kgc-2.7.0/test/rml-core/csv/RMLTC0008b/mapping.ttl`

 * *Files 12% similar despite different names*

```diff
@@ -1,58 +1,56 @@
-@prefix rr: <http://www.w3.org/ns/r2rml#> .
 @prefix foaf: <http://xmlns.com/foaf/0.1/> .
 @prefix ex: <http://example.com/> .
 @prefix xsd: <http://www.w3.org/2001/XMLSchema#> .
-@prefix rml: <http://semweb.mmlab.be/ns/rml#> .
-@prefix ql: <http://semweb.mmlab.be/ns/ql#> .
+@prefix rml: <http://w3id.org/rml/> .
 @prefix activity: <http://example.com/activity/> .
 @prefix rdf: <http://www.w3.org/1999/02/22-rdf-syntax-ns#> .
 @base <http://example.com/base/> .
 
 <TriplesMap2>
-  a rr:TriplesMap;
+  a rml:TriplesMap;
   rml:logicalSource [
-    rml:source "test/rml/csv/RMLTC0008b/student.csv";
-    rml:referenceFormulation ql:CSV
+    rml:source "test/rml-core/csv/RMLTC0008b/student.csv";
+    rml:referenceFormulation rml:CSV
   ];
 
-  rr:subjectMap [ rr:template "http://example.com/{Sport}" ];
+  rml:subjectMap [ rml:template "http://example.com/{Sport}" ];
 
-  rr:predicateObjectMap [
-    rr:predicate rdf:type ;
-    rr:object activity:Sport ;
+  rml:predicateObjectMap [
+    rml:predicate rdf:type ;
+    rml:object activity:Sport ;
   ] .
 
 <TriplesMap1>
-  a rr:TriplesMap;
+  a rml:TriplesMap;
 
   rml:logicalSource [
-    rml:source "test/rml/csv/RMLTC0008b/student.csv";
-    rml:referenceFormulation ql:CSV
+    rml:source "test/rml-core/csv/RMLTC0008b/student.csv";
+    rml:referenceFormulation rml:CSV
   ];
 
-  rr:subjectMap [ rr:template "http://example.com/Student/{ID}/{Name}" ];
+  rml:subjectMap [ rml:template "http://example.com/Student/{ID}/{Name}" ];
 
-  rr:predicateObjectMap [
-    rr:predicate rdf:type ;
-    rr:object foaf:Person ;
+  rml:predicateObjectMap [
+    rml:predicate rdf:type ;
+    rml:object foaf:Person ;
   ];
 
-  rr:predicateObjectMap [
-    rr:predicate ex:id ;
-    rr:objectMap [ rml:reference "ID"; ]
+  rml:predicateObjectMap [
+    rml:predicate ex:id ;
+    rml:objectMap [ rml:reference "ID"; ]
   ];
 
-  rr:predicateObjectMap [
-    rr:predicate foaf:name ;
-    rr:objectMap [ rml:reference "Name" ]
+  rml:predicateObjectMap [
+    rml:predicate foaf:name ;
+    rml:objectMap [ rml:reference "Name" ]
   ];
 
-  rr:predicateObjectMap [
-    rr:predicate ex:Sport ;
-    rr:objectMap <RefObjectMap1>
+  rml:predicateObjectMap [
+    rml:predicate ex:Sport ;
+    rml:objectMap <RefObjectMap1>
   ] .
 
 
 <RefObjectMap1>
-  a rr:RefObjectMap;
-  rr:parentTriplesMap <TriplesMap2> .
+  a rml:RefObjectMap;
+  rml:parentTriplesMap <TriplesMap2> .
```

### Comparing `morph_kgc-2.6.4/test/rml/csv/RMLTC0008b/output.nq` & `morph_kgc-2.7.0/test/rml-core/csv/RMLTC0008b/output.nq`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/rml/csv/RMLTC0008b/test_RMLTC0008b_CSV.py` & `morph_kgc-2.7.0/test/rml-core/csv/RMLTC0008b/test_RMLTC0008b_CSV.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/rml/csv/RMLTC0008c/mapping.ttl` & `morph_kgc-2.7.0/test/rml-core/json/RMLTC0000/mapping.ttl`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,26 @@
-@prefix rr: <http://www.w3.org/ns/r2rml#> .
 @prefix foaf: <http://xmlns.com/foaf/0.1/> .
 @prefix ex: <http://example.com/> .
 @prefix xsd: <http://www.w3.org/2001/XMLSchema#> .
-@prefix rml: <http://semweb.mmlab.be/ns/rml#> .
-@prefix ql: <http://semweb.mmlab.be/ns/ql#> .
-@prefix activity: <http://example.com/activity/> .
+@prefix rml: <http://w3id.org/rml/> .
+
 @base <http://example.com/base/> .
 
 <TriplesMap1>
-  a rr:TriplesMap;
+  a rml:TriplesMap;
 
   rml:logicalSource [
-    rml:source "test/rml/csv/RMLTC0008c/student.csv";
-    rml:referenceFormulation ql:CSV
-  ];
+    rml:source "test/rml-core/json/RMLTC0000/student.json";
+    rml:referenceFormulation rml:JSONPath;
+    rml:iterator "$.students[*]"
+  ] ;
 
-  rr:subjectMap [ rr:template "http://example.com/Student/{ID}/{Name}" ];
+  rml:subjectMap [
+    rml:template "http://example.com/{Name}"
+  ];
 
-  rr:predicateObjectMap [
-    rr:predicate foaf:name ;
-    rr:predicate ex:name ;
-    rr:objectMap [ rml:reference "Name" ]
-  ] .
+  rml:predicateObjectMap [
+    rml:predicate foaf:name ;
+    rml:objectMap [
+      rml:reference "Name"
+    ]
+  ].
```

### Comparing `morph_kgc-2.6.4/test/rml/csv/RMLTC0008c/test_RMLTC0008c_CSV.py` & `morph_kgc-2.7.0/test/rml-core/csv/RMLTC0008c/test_RMLTC0008c_CSV.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/rml/csv/RMLTC0009a/mapping.ttl` & `morph_kgc-2.7.0/test/rml-core/json/RMLTC0009b/mapping.ttl`

 * *Files 16% similar despite different names*

```diff
@@ -1,51 +1,59 @@
-@prefix rr: <http://www.w3.org/ns/r2rml#> .
 @prefix foaf: <http://xmlns.com/foaf/0.1/> .
 @prefix ex: <http://example.com/> .
 @prefix xsd: <http://www.w3.org/2001/XMLSchema#> .
-@prefix rml: <http://semweb.mmlab.be/ns/rml#> .
-@prefix ql: <http://semweb.mmlab.be/ns/ql#> .
+@prefix rml: <http://w3id.org/rml/> .
 @prefix activity: <http://example.com/activity/> .
 @prefix rdfs: <http://www.w3.org/2000/01/rdf-schema#> .
 @base <http://example.com/base/> .
 
 <TriplesMap1>
-  a rr:TriplesMap;
+  a rml:TriplesMap;
 
   rml:logicalSource [
-    rml:source "test/rml/csv/RMLTC0009a/student.csv";
-    rml:referenceFormulation ql:CSV
+    rml:source "test/rml-core/json/RMLTC0009b/student.json";
+    rml:referenceFormulation rml:JSONPath;
+    rml:iterator "$.students[*]"
   ];
 
-  rr:subjectMap [ rr:template "http://example.com/resource/student_{ID}" ];
-
-  rr:predicateObjectMap [
-    rr:predicate foaf:name ;
-    rr:objectMap [ rml:reference "Name" ]
+  rml:subjectMap [ rml:template "http://example.com/resource/student_{ID}";
+    rml:class <http://example.com/ontology/Student>;
+    rml:graph <http://example.com/graph/students> ;
+ ];
+
+  rml:predicateObjectMap [
+    rml:predicate foaf:name ;
+    rml:objectMap [ rml:reference "Name" ];
+    rml:graph <http://example.com/graph/students> ;
   ] ;
 
-  rr:predicateObjectMap [
-    rr:predicate <http://example.com/ontology/practises> ;
-    rr:objectMap [
-      a rr:RefObjectMap ;
-      rr:parentTriplesMap <TriplesMap2>;
-      rr:joinCondition [
-        rr:child "Sport" ;
-        rr:parent "ID" ;
+  rml:predicateObjectMap [
+    rml:predicate <http://example.com/ontology/practises> ;
+    rml:objectMap [
+      a rml:RefObjectMap ;
+      rml:parentTriplesMap <TriplesMap2>;
+      rml:joinCondition [
+        rml:child "Sport" ;
+        rml:parent "ID" ;
       ]
-    ]
+    ];
+    rml:graph <http://example.com/graph/practise> ;
   ] .
 
 <TriplesMap2>
-  a rr:TriplesMap;
+  a rml:TriplesMap;
 
   rml:logicalSource [
-    rml:source "test/rml/csv/RMLTC0009a/sport.csv";
-    rml:referenceFormulation ql:CSV
+    rml:source "test/rml-core/json/RMLTC0009b/sport.json";
+    rml:referenceFormulation rml:JSONPath;
+    rml:iterator "$.sports[*]"
   ];
 
-  rr:subjectMap [ rr:template "http://example.com/resource/sport_{ID}" ];
+  rml:subjectMap [ rml:template "http://example.com/resource/sport_{ID}";
+    rml:class <http://example.com/ontology/Sport>;
+    rml:graph <http://example.com/graph/sports> ;
+  ];
 
-  rr:predicateObjectMap [
-    rr:predicate rdfs:label ;
-    rr:objectMap [ rml:reference "Name" ];
+  rml:predicateObjectMap [
+    rml:predicate rdfs:label ;
+    rml:objectMap [ rml:reference "Name" ];
   ].
```

### Comparing `morph_kgc-2.6.4/test/rml/csv/RMLTC0009a/test_RMLTC0009a_CSV.py` & `morph_kgc-2.7.0/test/rml-core/csv/RMLTC0009a/test_RMLTC0009a_CSV.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/rml/csv/RMLTC0009b/mapping.ttl` & `morph_kgc-2.7.0/test/rml-fnml/split_explode/mapping.ttl`

 * *Files 20% similar despite different names*

```diff
@@ -1,61 +1,39 @@
-@prefix rr: <http://www.w3.org/ns/r2rml#> .
 @prefix foaf: <http://xmlns.com/foaf/0.1/> .
 @prefix ex: <http://example.com/> .
 @prefix xsd: <http://www.w3.org/2001/XMLSchema#> .
-@prefix rml: <http://semweb.mmlab.be/ns/rml#> .
-@prefix ql: <http://semweb.mmlab.be/ns/ql#> .
-@prefix activity: <http://example.com/activity/> .
-@prefix rdfs: <http://www.w3.org/2000/01/rdf-schema#> .
+@prefix rml: <http://w3id.org/rml/> .
+@prefix fno: <https://w3id.org/function/ontology#> .
+@prefix morph-kgc: <https://github.com/morph-kgc/morph-kgc/function/built-in.ttl#> .
+@prefix grel: <http://users.ugent.be/~bjdmeest/function/grel.ttl#> .
+@prefix idlab-fn: <http://example.com/idlab/function/> .
+
 @base <http://example.com/base/> .
 
 <TriplesMap1>
-  a rr:TriplesMap;
-
-  rml:logicalSource [
-    rml:source "test/rml/csv/RMLTC0009b/student.csv";
-    rml:referenceFormulation ql:CSV
-  ];
-
-  rr:subjectMap [
-    rr:template "http://example.com/resource/student_{ID}" ;
-    rr:class <http://example.com/ontology/Student>;
-    rr:graph <http://example.com/graph/students> ;
-  ];
-
-  rr:predicateObjectMap [
-    rr:predicate foaf:name ;
-    rr:objectMap [ rml:reference "Name" ];
-    rr:graph <http://example.com/graph/students> ;
-  ] ;
-
-  rr:predicateObjectMap [
-    rr:predicate <http://example.com/ontology/practises> ;
-    rr:objectMap [
-      a rr:RefObjectMap ;
-      rr:parentTriplesMap <TriplesMap2>;
-      rr:joinCondition [
-        rr:child "Sport" ;
-        rr:parent "ID" ;
-      ]
+    rml:logicalSource [
+        rml:source "test/rml-fnml/split_explode/mixed_content_list.csv";
+        rml:referenceFormulation rml:CSV
     ];
-    rr:graph <http://example.com/graph/practise> ;
-  ] .
-
-<TriplesMap2>
-  a rr:TriplesMap;
-
-  rml:logicalSource [
-    rml:source "test/rml/csv/RMLTC0009b/sport.csv";
-    rml:referenceFormulation ql:CSV
-  ];
-
-  rr:subjectMap [
-    rr:template "http://example.com/resource/sport_{ID}";
-    rr:class <http://example.com/ontology/Sport>;
-    rr:graph <http://example.com/graph/sports> ;
-  ];
-
-  rr:predicateObjectMap [
-    rr:predicate rdfs:label ;
-    rr:objectMap [ rml:reference "Name" ];
-  ].
+    rml:subjectMap [
+        rml:template "http://example.com/{ID}"
+    ];
+    rml:predicateObjectMap [
+        rml:predicate ex:col;
+        rml:objectMap [
+            rml:functionExecution <#Execution> ;
+        ]
+    ] .
+
+<#Execution>
+    rml:function morph-kgc:string_split_explode ;
+    rml:input
+        [
+            rml:parameter grel:valueParam ;
+            rml:inputValueMap [
+                rml:reference "COL"
+            ]
+        ] ,
+        [
+            rml:parameter grel:param_string_sep ;
+            rml:inputValue ";"
+        ] .
```

### Comparing `morph_kgc-2.6.4/test/rml/csv/RMLTC0009b/output.nq` & `morph_kgc-2.7.0/test/rml-core/csv/RMLTC0009b/output.nq`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/rml/csv/RMLTC0009b/test_RMLTC0009b_CSV.py` & `morph_kgc-2.7.0/test/rml-core/csv/RMLTC0009b/test_RMLTC0009b_CSV.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/rml/csv/RMLTC0010a/mapping.ttl` & `morph_kgc-2.7.0/test/rml-core/json/RMLTC0002c/mapping.ttl`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,22 @@
-@prefix rr: <http://www.w3.org/ns/r2rml#> .
 @prefix foaf: <http://xmlns.com/foaf/0.1/> .
 @prefix ex: <http://example.com/> .
 @prefix xsd: <http://www.w3.org/2001/XMLSchema#> .
-@prefix rml: <http://semweb.mmlab.be/ns/rml#> .
-@prefix ql: <http://semweb.mmlab.be/ns/ql#> .
-@prefix activity: <http://example.com/activity/> .
+@prefix rml: <http://w3id.org/rml/> .
 @base <http://example.com/base/> .
 
-<TriplesMap1>
-  a rr:TriplesMap;
+<TriplesMap1> a rml:TriplesMap;
 
   rml:logicalSource [
-    rml:source "test/rml/csv/RMLTC0010a/country_info.csv";
-    rml:referenceFormulation ql:CSV
+    rml:source "test/rml-core/json/RMLTC0002c/student.json";
+    rml:referenceFormulation rml:JSONPath;
+    rml:iterator "$.students[*]"
   ];
 
-  rr:subjectMap [ rr:template "http://example.com/{Country Code}" ];
+  rml:subjectMap [
+    rml:template "http://example.com/{ID}/{Name}";
+  ];
 
-  rr:predicateObjectMap [
-    rr:predicate ex:name ;
-    rr:objectMap [ rml:reference "Name" ]
-  ] .
+  rml:predicateObjectMap [
+    rml:predicate ex:id ;
+    rml:objectMap [ rml:reference "IDs" ]
+  ].
```

### Comparing `morph_kgc-2.6.4/test/rml/csv/RMLTC0010a/test_RMLTC0010a_CSV.py` & `morph_kgc-2.7.0/test/rml-core/csv/RMLTC0010a/test_RMLTC0010a_CSV.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/rml/csv/RMLTC0010b/mapping.ttl` & `morph_kgc-2.7.0/test/rml-core/json/RMLTC0002e/mapping.ttl`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,22 @@
-@prefix rr: <http://www.w3.org/ns/r2rml#> .
 @prefix foaf: <http://xmlns.com/foaf/0.1/> .
 @prefix ex: <http://example.com/> .
 @prefix xsd: <http://www.w3.org/2001/XMLSchema#> .
-@prefix rml: <http://semweb.mmlab.be/ns/rml#> .
-@prefix ql: <http://semweb.mmlab.be/ns/ql#> .
-@prefix activity: <http://example.com/activity/> .
+@prefix rml: <http://w3id.org/rml/> .
 @base <http://example.com/base/> .
 
-<TriplesMap1>
-  a rr:TriplesMap;
+<TriplesMap1> a rml:TriplesMap;
 
   rml:logicalSource [
-    rml:source "test/rml/csv/RMLTC0010b/country_info.csv";
-    rml:referenceFormulation ql:CSV
+    rml:source "test/rml-core/json/RMLTC0002e/student2.json";
+    rml:referenceFormulation rml:JSONPath;
+    rml:iterator "$.students[*]"
   ];
 
-  rr:subjectMap [ rr:template "http://example.com/{Country Code}/{Name}" ];
+  rml:subjectMap [
+    rml:template "http://example.com/{ID}/{Name}";
+  ];
 
-  rr:predicateObjectMap [
-    rr:predicate ex:name ;
-    rr:objectMap [ rml:reference "Name" ]
-  ] .
+  rml:predicateObjectMap [
+    rml:predicate ex:id ;
+    rml:objectMap [ rml:reference "ID" ]
+  ].
```

### Comparing `morph_kgc-2.6.4/test/rml/csv/RMLTC0010b/test_RMLTC0010b_CSV.py` & `morph_kgc-2.7.0/test/rml-core/csv/RMLTC0010b/test_RMLTC0010b_CSV.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/rml/csv/RMLTC0010c/mapping.ttl` & `morph_kgc-2.7.0/test/rml-core/xml/RMLTC0010c/mapping.ttl`

 * *Files 15% similar despite different names*

```diff
@@ -1,23 +1,22 @@
-@prefix rr: <http://www.w3.org/ns/r2rml#> .
 @prefix foaf: <http://xmlns.com/foaf/0.1/> .
 @prefix ex: <http://example.com/> .
 @prefix xsd: <http://www.w3.org/2001/XMLSchema#> .
-@prefix rml: <http://semweb.mmlab.be/ns/rml#> .
-@prefix ql: <http://semweb.mmlab.be/ns/ql#> .
+@prefix rml: <http://w3id.org/rml/> .
 @prefix activity: <http://example.com/activity/> .
 @base <http://example.com/base/> .
 
 <TriplesMap1>
-  a rr:TriplesMap;
+  a rml:TriplesMap;
 
   rml:logicalSource [
-    rml:source "test/rml/csv/RMLTC0010c/country_info.csv";
-    rml:referenceFormulation ql:CSV
+    rml:source "test/rml-core/xml/RMLTC0010c/country_info.xml";
+    rml:referenceFormulation rml:XPath;
+    rml:iterator "/countries/country"
   ];
 
-  rr:subjectMap [ rr:template "http://example.com/{Country Code}/{Name}" ];
+  rml:subjectMap [ rml:template "http://example.com/{CountryCode}/{Name}" ];
 
-  rr:predicateObjectMap [
-    rr:predicate ex:code ;
-    rr:objectMap [ rr:template "\\{\\{\\{ {ISO 3166} \\}\\}\\}"; rr:termType rr:Literal]
+  rml:predicateObjectMap [
+    rml:predicate ex:code ;
+    rml:objectMap [ rml:template "\\{\\{\\{ {ISO3166} \\}\\}\\}"; rml:termType rml:Literal]
   ] .
```

### Comparing `morph_kgc-2.6.4/test/rml/csv/RMLTC0010c/test_RMLTC0010c_CSV.py` & `morph_kgc-2.7.0/test/rml-core/csv/RMLTC0010c/test_RMLTC0010c_CSV.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/rml/csv/RMLTC0011b/mapping.ttl` & `morph_kgc-2.7.0/test/rml-core/json/RMLTC0011b/mapping.ttl`

 * *Files 12% similar despite different names*

```diff
@@ -1,79 +1,80 @@
-@prefix rr: <http://www.w3.org/ns/r2rml#> .
 @prefix foaf: <http://xmlns.com/foaf/0.1/> .
 @prefix ex: <http://example.com/> .
 @prefix xsd: <http://www.w3.org/2001/XMLSchema#> .
-@prefix rml: <http://semweb.mmlab.be/ns/rml#> .
-@prefix ql: <http://semweb.mmlab.be/ns/ql#> .
+@prefix rml: <http://w3id.org/rml/> .
 
 @base <http://example.com/base/> .
 
 <TriplesMap1>
-  a rr:TriplesMap;
+  a rml:TriplesMap;
 
   rml:logicalSource [
-    rml:source "test/rml/csv/RMLTC0011b/student.csv";
-    rml:referenceFormulation ql:CSV
+    rml:source "test/rml-core/json/RMLTC0011b/student.json";
+    rml:referenceFormulation rml:JSONPath;
+    rml:iterator "$.students[*]"
   ];
 
-  rr:subjectMap [
-    rr:template "http://example.com/student/{ID}";
+  rml:subjectMap [
+    rml:template "http://example.com/student/{ID}";
   ];
 
-  rr:predicateObjectMap [
-    rr:predicate ex:firstName;
-    rr:objectMap [
+  rml:predicateObjectMap [
+    rml:predicate ex:firstName;
+    rml:objectMap [
       rml:reference "FirstName"
     ]
   ];
 
-  rr:predicateObjectMap [
-    rr:predicate ex:lastName;
-    rr:objectMap [
+  rml:predicateObjectMap [
+    rml:predicate ex:lastName;
+    rml:objectMap [
       rml:reference "LastName"
     ]
   ].
 
 <TriplesMap2>
-  a rr:TriplesMap;
+  a rml:TriplesMap;
 
   rml:logicalSource [
-    rml:source "test/rml/csv/RMLTC0011b/sport.csv";
-    rml:referenceFormulation ql:CSV
+    rml:source "test/rml-core/json/RMLTC0011b/sport.json";
+    rml:referenceFormulation rml:JSONPath;
+    rml:iterator "$.sports[*]"
   ];
 
-  rr:subjectMap [
-    rr:template "http://example.com/sport/{ID}";
+  rml:subjectMap [
+    rml:template "http://example.com/sport/{ID}";
   ];
 
-  rr:predicateObjectMap [
-    rr:predicate ex:id;
-    rr:objectMap [
+  rml:predicateObjectMap [
+    rml:predicate ex:id;
+    rml:objectMap [
       rml:reference "ID"
     ]
   ];
 
-  rr:predicateObjectMap [
-    rr:predicate ex:description;
-    rr:objectMap [
+  rml:predicateObjectMap [
+    rml:predicate ex:description;
+    rml:objectMap [
       rml:reference "Description"
     ]
   ].
 
 <LinkMap_1_2>
-  a rr:TriplesMap;
+  a rml:TriplesMap;
 
   rml:logicalSource [
-    rml:source "test/rml/csv/RMLTC0011b/student_sport.csv";
-    rml:referenceFormulation ql:CSV
+    rml:source "test/rml-core/json/RMLTC0011b/student_sport.json";
+    rml:referenceFormulation rml:JSONPath;
+    rml:iterator "$.links[*]"
   ];
 
-  rr:subjectMap [
-    rr:template "http://example.com/student/{ID_Student}";
+  rml:subjectMap [
+    rml:template "http://example.com/student/{ID_Student}";
   ];
 
-  rr:predicateObjectMap [
-    rr:predicate ex:plays;
-    rr:objectMap [
-      rr:template "http://example.com/sport/{ID_Sport}"
+  rml:predicateObjectMap [
+    rml:predicate ex:plays;
+    rml:objectMap [
+      rml:template "http://example.com/sport/{ID_Sport}"
     ]
   ].
```

### Comparing `morph_kgc-2.6.4/test/rml/csv/RMLTC0011b/output.nq` & `morph_kgc-2.7.0/test/rml-core/csv/RMLTC0011b/output.nq`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/rml/csv/RMLTC0011b/test_RMLTC0011b_CSV.py` & `morph_kgc-2.7.0/test/rml-core/csv/RMLTC0011b/test_RMLTC0011b_CSV.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/rml/csv/RMLTC0012a/mapping.ttl` & `morph_kgc-2.7.0/test/rml-core/csv/RMLTC0012d/mapping.ttl`

 * *Files 16% similar despite different names*

```diff
@@ -1,33 +1,33 @@
-@prefix rr: <http://www.w3.org/ns/r2rml#> .
 @prefix foaf: <http://xmlns.com/foaf/0.1/> .
 @prefix ex: <http://example.com/> .
 @prefix xsd: <http://www.w3.org/2001/XMLSchema#> .
-@prefix rml: <http://semweb.mmlab.be/ns/rml#> .
-@prefix ql: <http://semweb.mmlab.be/ns/ql#> .
+@prefix rml: <http://w3id.org/rml/> .
 
 @base <http://example.com/base/> .
 
 <TriplesMap1>
-  a rr:TriplesMap;
+  a rml:TriplesMap;
 
   rml:logicalSource [
-    rml:source "test/rml/csv/RMLTC0012a/persons.csv";
-    rml:referenceFormulation ql:CSV
+    rml:source "test/rml-core/csv/RMLTC0012d/persons.csv";
+    rml:referenceFormulation rml:CSV
   ];
 
-  rr:subjectMap [ rr:template "{fname}{lname}{amount}"; rr:termType rr:BlankNode; ];
+  rml:subjectMap [ rml:template "{fname}_{lname}_{amount}"; rml:termType rml:BlankNode; ];
 
-  rr:predicateObjectMap [
-    rr:predicate foaf:name ;
-    rr:objectMap [
-      rr:template "{fname} {lname}";
-      rr:termType rr:Literal ;
+  rml:subjectMap [ rml:template "{amount}_{fname}_{lname}"; rml:termType rml:BlankNode; ];
+
+  rml:predicateObjectMap [
+    rml:predicate foaf:name ;
+    rml:objectMap [
+      rml:template "{fname} {lname}";
+      rml:termType rml:Literal ;
     ]
   ];
 
-  rr:predicateObjectMap [
-    rr:predicate ex:amount ;
-    rr:objectMap    [
+  rml:predicateObjectMap [
+    rml:predicate ex:amount ;
+    rml:objectMap    [
       rml:reference "amount";
     ]
   ].
```

### Comparing `morph_kgc-2.6.4/test/rml/csv/RMLTC0012a/test_RMLTC0012a_CSV.py` & `morph_kgc-2.7.0/test/rml-core/csv/RMLTC0012a/test_RMLTC0012a_CSV.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/rml/csv/RMLTC0012b/mapping.ttl` & `morph_kgc-2.7.0/test/rml-core/csv/RMLTC0012b/mapping.ttl`

 * *Files 14% similar despite different names*

```diff
@@ -1,52 +1,50 @@
-@prefix rr: <http://www.w3.org/ns/r2rml#> .
 @prefix foaf: <http://xmlns.com/foaf/0.1/> .
 @prefix ex: <http://example.com/> .
 @prefix xsd: <http://www.w3.org/2001/XMLSchema#> .
-@prefix rml: <http://semweb.mmlab.be/ns/rml#> .
-@prefix ql: <http://semweb.mmlab.be/ns/ql#> .
+@prefix rml: <http://w3id.org/rml/> .
 
 @base <http://example.com/base/> .
 
 <TriplesMap1>
-  a rr:TriplesMap;
+  a rml:TriplesMap;
 
   rml:logicalSource [
-    rml:source "test/rml/csv/RMLTC0012b/persons.csv";
-    rml:referenceFormulation ql:CSV
+    rml:source "test/rml-core/csv/RMLTC0012b/persons.csv";
+    rml:referenceFormulation rml:CSV
   ];
 
-  rr:subjectMap [
-    rr:template "{fname}{lname}";
-    rr:termType rr:BlankNode ;
+  rml:subjectMap [
+    rml:template "{fname}{lname}";
+    rml:termType rml:BlankNode ;
   ];
 
-  rr:predicateObjectMap [
-    rr:predicate foaf:name ;
-    rr:objectMap [
-      rr:template "{fname} {lname}";
-      rr:termType rr:Literal ;
+  rml:predicateObjectMap [
+    rml:predicate foaf:name ;
+    rml:objectMap [
+      rml:template "{fname} {lname}";
+      rml:termType rml:Literal ;
     ]
   ];
   .
 
 <TriplesMap2>
-  a rr:TriplesMap;
+  a rml:TriplesMap;
 
   rml:logicalSource [
-    rml:source "test/rml/csv/RMLTC0012b/lives.csv";
-    rml:referenceFormulation ql:CSV
+    rml:source "test/rml-core/csv/RMLTC0012b/lives.csv";
+    rml:referenceFormulation rml:CSV
 ];
 
-  rr:subjectMap [
-    rr:template "{fname}{lname}";
-    rr:termType rr:BlankNode;
+  rml:subjectMap [
+    rml:template "{fname}{lname}";
+    rml:termType rml:BlankNode;
   ];
 
-  rr:predicateObjectMap
+  rml:predicateObjectMap
   [
-    rr:predicate	ex:city ;
-    rr:objectMap    [
+    rml:predicate	ex:city ;
+    rml:objectMap    [
       rml:reference "city";
     ]
 ];
 .
```

### Comparing `morph_kgc-2.6.4/test/rml/csv/RMLTC0012b/test_RMLTC0012b_CSV.py` & `morph_kgc-2.7.0/test/rml-core/csv/RMLTC0012b/test_RMLTC0012b_CSV.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/rml/csv/RMLTC0012c/mapping.ttl` & `morph_kgc-2.7.0/test/rml-core/xml/RMLTC0020a/mapping.ttl`

 * *Files 16% similar despite different names*

```diff
@@ -1,31 +1,25 @@
-@prefix rr: <http://www.w3.org/ns/r2rml#> .
 @prefix foaf: <http://xmlns.com/foaf/0.1/> .
 @prefix ex: <http://example.com/> .
 @prefix xsd: <http://www.w3.org/2001/XMLSchema#> .
-@prefix rml: <http://semweb.mmlab.be/ns/rml#> .
-@prefix ql: <http://semweb.mmlab.be/ns/ql#> .
+@prefix rdf: <http://www.w3.org/1999/02/22-rdf-syntax-ns#> .
+@prefix rml:    <http://w3id.org/rml/> .
+@prefix ql:     <http://semweb.mmlab.be/ns/ql#> .
 
 @base <http://example.com/base/> .
 
 <TriplesMap1>
-  a rr:TriplesMap;
-
+  a rml:TriplesMap;
   rml:logicalSource [
-    rml:source "test/rml/csv/RMLTC0012c/persons.csv";
-    rml:referenceFormulation ql:CSV
+    rml:source "test/rml-core/xml/RMLTC0020a/student.xml";
+    rml:referenceFormulation rml:XPath;
+    rml:iterator "/students/student"
   ];
 
-  rr:predicateObjectMap [
-    rr:predicate foaf:name ;
-    rr:objectMap [
-      rr:template "{fname} {lname}";
-      rr:termType rr:Literal ;
-    ]
-  ];
+    rml:subjectMap [     rml:template "{Name}";
+                        rml:termType rml:IRI ];
 
-  rr:predicateObjectMap [
-    rr:predicate ex:amount ;
-    rr:objectMap    [
-      rml:reference "amount";
-    ]
-  ].
+    rml:predicateObjectMap
+    [
+    	rml:predicate rdf:type;
+    	rml:object foaf:Person;
+    ].
```

### Comparing `morph_kgc-2.6.4/test/rml/csv/RMLTC0012c/test_RMLTC0012c_CSV.py` & `morph_kgc-2.7.0/test/rml-core/csv/RMLTC0012c/test_RMLTC0012c_CSV.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/rml/csv/RMLTC0012d/mapping.ttl` & `morph_kgc-2.7.0/test/rml-core/csv/RMLTC0012a/mapping.ttl`

 * *Files 14% similar despite different names*

```diff
@@ -1,35 +1,31 @@
-@prefix rr: <http://www.w3.org/ns/r2rml#> .
 @prefix foaf: <http://xmlns.com/foaf/0.1/> .
 @prefix ex: <http://example.com/> .
 @prefix xsd: <http://www.w3.org/2001/XMLSchema#> .
-@prefix rml: <http://semweb.mmlab.be/ns/rml#> .
-@prefix ql: <http://semweb.mmlab.be/ns/ql#> .
+@prefix rml: <http://w3id.org/rml/> .
 
 @base <http://example.com/base/> .
 
 <TriplesMap1>
-  a rr:TriplesMap;
+  a rml:TriplesMap;
 
   rml:logicalSource [
-    rml:source "test/rml/csv/RMLTC0012d/persons.csv";
-    rml:referenceFormulation ql:CSV
+    rml:source "test/rml-core/csv/RMLTC0012a/persons.csv";
+    rml:referenceFormulation rml:CSV
   ];
 
-  rr:subjectMap [ rr:template "{fname}_{lname}_{amount}"; rr:termType rr:BlankNode; ];
+  rml:subjectMap [ rml:template "{fname}{lname}{amount}"; rml:termType rml:BlankNode; ];
 
-  rr:subjectMap [ rr:template "{amount}_{fname}_{lname}"; rr:termType rr:BlankNode; ];
-
-  rr:predicateObjectMap [
-    rr:predicate foaf:name ;
-    rr:objectMap [
-      rr:template "{fname} {lname}";
-      rr:termType rr:Literal ;
+  rml:predicateObjectMap [
+    rml:predicate foaf:name ;
+    rml:objectMap [
+      rml:template "{fname} {lname}";
+      rml:termType rml:Literal ;
     ]
   ];
 
-  rr:predicateObjectMap [
-    rr:predicate ex:amount ;
-    rr:objectMap    [
+  rml:predicateObjectMap [
+    rml:predicate ex:amount ;
+    rml:objectMap    [
       rml:reference "amount";
     ]
   ].
```

### Comparing `morph_kgc-2.6.4/test/rml/csv/RMLTC0012d/test_RMLTC0012d_CSV.py` & `morph_kgc-2.7.0/test/rml-core/csv/RMLTC0012d/test_RMLTC0012d_CSV.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/rml/csv/RMLTC0015a/mapping.ttl` & `morph_kgc-2.7.0/test/rml-core/json/RMLTC0015b/mapping.ttl`

 * *Files 14% similar despite different names*

```diff
@@ -1,48 +1,45 @@
-@prefix rr: <http://www.w3.org/ns/r2rml#> .
 @prefix foaf: <http://xmlns.com/foaf/0.1/> .
+@prefix rdfs: <http://www.w3.org/2000/01/rdf-schema#> .
 @prefix ex: <http://example.com/> .
 @prefix xsd: <http://www.w3.org/2001/XMLSchema#> .
-@prefix rml: <http://semweb.mmlab.be/ns/rml#> .
-@prefix ql: <http://semweb.mmlab.be/ns/ql#> .
-@prefix rdfs: <http://www.w3.org/2000/01/rdf-schema#> .
+@prefix rml: <http://w3id.org/rml/> .
+
 @base <http://example.com/base/> .
 
 <TriplesMap1>
-  a rr:TriplesMap;
+  a rml:TriplesMap;
 
   rml:logicalSource [
-    rml:source "test/rml/csv/RMLTC0015a/country_en.csv";
-    rml:referenceFormulation ql:CSV
+    rml:source "test/rml-core/json/RMLTC0015b/country_en.json";
+    rml:referenceFormulation rml:JSONPath;
+    rml:iterator "$.countries[*]"
   ];
 
-  rr:subjectMap [
-    rr:template "http://example.com/{Code}"
-  ];
+  rml:subjectMap [ rml:template "http://example.com/{Code}" ];
 
-  rr:predicateObjectMap [
-    rr:predicate rdfs:label ;
-    rr:objectMap [
+  rml:predicateObjectMap [
+    rml:predicate rdfs:label;
+    rml:objectMap [
       rml:reference "Name";
-      rr:language "en"
+      rml:language "english"
     ]
-  ].
+  ] .
 
 <TriplesMap2>
-  a rr:TriplesMap;
+  a rml:TriplesMap;
 
   rml:logicalSource [
-    rml:source "test/rml/csv/RMLTC0015a/country_es.csv";
-    rml:referenceFormulation ql:CSV
+    rml:source "test/rml-core/json/RMLTC0015b/country_en.json";
+    rml:referenceFormulation rml:JSONPath;
+    rml:iterator "$.countries[*]"
   ];
 
-  rr:subjectMap [
-    rr:template "http://example.com/{Code}"
-  ];
+  rml:subjectMap [ rml:template "http://example.com/{Code}" ];
 
-  rr:predicateObjectMap [
-    rr:predicate rdfs:label ;
-    rr:objectMap [
+  rml:predicateObjectMap [
+    rml:predicate rdfs:label;
+    rml:objectMap [
       rml:reference "Name";
-      rr:language "es"
+      rml:language "spanish"
     ]
   ].
```

### Comparing `morph_kgc-2.6.4/test/rml/csv/RMLTC0015a/test_RMLTC0015a_CSV.py` & `morph_kgc-2.7.0/test/rml-core/csv/RMLTC0015a/test_RMLTC0015a_CSV.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/rml/csv/RMLTC0015b/mapping.ttl` & `morph_kgc-2.7.0/test/rml-core/xml/RMLTC0015b/mapping.ttl`

 * *Files 12% similar despite different names*

```diff
@@ -1,45 +1,45 @@
-@prefix rr: <http://www.w3.org/ns/r2rml#> .
 @prefix foaf: <http://xmlns.com/foaf/0.1/> .
 @prefix rdfs: <http://www.w3.org/2000/01/rdf-schema#> .
 @prefix ex: <http://example.com/> .
 @prefix xsd: <http://www.w3.org/2001/XMLSchema#> .
-@prefix rml: <http://semweb.mmlab.be/ns/rml#> .
-@prefix ql: <http://semweb.mmlab.be/ns/ql#> .
+@prefix rml: <http://w3id.org/rml/> .
 
 @base <http://example.com/base/> .
 
 <TriplesMap1>
-  a rr:TriplesMap;
+  a rml:TriplesMap;
 
   rml:logicalSource [
-    rml:source "test/rml/csv/RMLTC0015b/country_en.csv";
-    rml:referenceFormulation ql:CSV
+    rml:source "test/rml-core/xml/RMLTC0015b/country_en.xml";
+    rml:referenceFormulation rml:XPath;
+    rml:iterator "/countries/country"
   ];
 
-  rr:subjectMap [ rr:template "http://example.com/{Code}" ];
+  rml:subjectMap [ rml:template "http://example.com/{Code}" ];
 
-  rr:predicateObjectMap [
-    rr:predicate rdfs:label;
-    rr:objectMap [
+  rml:predicateObjectMap [
+    rml:predicate rdfs:label;
+    rml:objectMap [
       rml:reference "Name";
-      rr:language "english"
+      rml:language "english"
     ]
   ] .
 
 <TriplesMap2>
-  a rr:TriplesMap;
+  a rml:TriplesMap;
 
   rml:logicalSource [
-    rml:source "test/rml/csv/RMLTC0015b/country_es.csv";
-    rml:referenceFormulation ql:CSV
+    rml:source "test/rml-core/xml/RMLTC0015b/country_es.xml";
+    rml:referenceFormulation rml:XPath;
+    rml:iterator "/countries/country"
   ];
 
-  rr:subjectMap [ rr:template "http://example.com/{Code}" ];
+  rml:subjectMap [ rml:template "http://example.com/{Code}" ];
 
-  rr:predicateObjectMap [
-    rr:predicate rdfs:label;
-    rr:objectMap [
+  rml:predicateObjectMap [
+    rml:predicate rdfs:label;
+    rml:objectMap [
       rml:reference "Name";
-      rr:language "spanish"
+      rml:language "spanish"
     ]
   ].
```

### Comparing `morph_kgc-2.6.4/test/rml/csv/RMLTC0015b/test_RMLTC0015b_CSV.py` & `morph_kgc-2.7.0/test/rml-core/csv/RMLTC0015b/test_RMLTC0015b_CSV.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/rml/csv/RMLTC0019a/RMLTC0019a_CSV.py` & `morph_kgc-2.7.0/test/rml-core/csv/RMLTC0019a/RMLTC0019a_CSV.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/rml/csv/RMLTC0019a/mapping.ttl` & `morph_kgc-2.7.0/test/rml-core/xml/RMLTC0020b/mapping.ttl`

 * *Files 14% similar despite different names*

```diff
@@ -1,26 +1,24 @@
-@prefix rr: <http://www.w3.org/ns/r2rml#> .
 @prefix foaf: <http://xmlns.com/foaf/0.1/> .
-@prefix rdfs: <http://www.w3.org/2000/01/rdf-schema#> .
 @prefix ex: <http://example.com/> .
 @prefix xsd: <http://www.w3.org/2001/XMLSchema#> .
-@prefix rml: <http://semweb.mmlab.be/ns/rml#> .
-@prefix ql: <http://semweb.mmlab.be/ns/ql#> .
+@prefix rdf: <http://www.w3.org/1999/02/22-rdf-syntax-ns#> .
+@prefix rml:    <http://w3id.org/rml/> .
+@prefix ql:     <http://semweb.mmlab.be/ns/ql#> .
 
 @base <http://example.com/base/> .
 
 <TriplesMap1>
-  a rr:TriplesMap;
-
+  a rml:TriplesMap;
   rml:logicalSource [
-    rml:source "test/rml/csv/RMLTC0019a/persons.csv";
-    rml:referenceFormulation ql:CSV
+    rml:source "test/rml-core/xml/RMLTC0020b/student.xml";
+    rml:referenceFormulation rml:XPath;
+    rml:iterator "/students/student"
   ];
 
-  rr:subjectMap [ rml:reference "FirstName" ];
+    rml:subjectMap [ rml:reference "Name"; rml:termType rml:IRI; ];
 
-  rr:predicateObjectMap [
-    rr:predicate foaf:name;
-    rr:objectMap [
-      rml:reference "FirstName"
-    ]
-  ] .
+    rml:predicateObjectMap
+    [
+    	rml:predicate rdf:type;
+    	rml:object foaf:Person;
+    ].
```

### Comparing `morph_kgc-2.6.4/test/rml/csv/RMLTC0019b/RMLTC0019b_CSV.py` & `morph_kgc-2.7.0/test/rml-core/csv/RMLTC0019b/RMLTC0019b_CSV.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/rml/csv/RMLTC0019b/mapping.ttl` & `morph_kgc-2.7.0/test/rml-core/xml/RMLTC0019a/mapping.ttl`

 * *Files 15% similar despite different names*

```diff
@@ -1,26 +1,25 @@
-@prefix rr: <http://www.w3.org/ns/r2rml#> .
 @prefix foaf: <http://xmlns.com/foaf/0.1/> .
 @prefix rdfs: <http://www.w3.org/2000/01/rdf-schema#> .
 @prefix ex: <http://example.com/> .
 @prefix xsd: <http://www.w3.org/2001/XMLSchema#> .
-@prefix rml: <http://semweb.mmlab.be/ns/rml#> .
-@prefix ql: <http://semweb.mmlab.be/ns/ql#> .
+@prefix rml: <http://w3id.org/rml/> .
 
 @base <http://example.com/base/> .
 
 <TriplesMap1>
-  a rr:TriplesMap;
+  a rml:TriplesMap;
 
   rml:logicalSource [
-    rml:source "test/rml/csv/RMLTC0019b/persons.csv";
-    rml:referenceFormulation ql:CSV
+    rml:source "test/rml-core/xml/RMLTC0019a/persons.xml";
+    rml:referenceFormulation rml:XPath;
+    rml:iterator "/persons/person"
   ];
 
-  rr:subjectMap [ rml:reference "FirstName" ];
+  rml:subjectMap [ rml:reference "FirstName" ];
 
-  rr:predicateObjectMap [
-    rr:predicate foaf:name;
-    rr:objectMap [
+  rml:predicateObjectMap [
+    rml:predicate foaf:name;
+    rml:objectMap [
       rml:reference "FirstName"
     ]
   ] .
```

### Comparing `morph_kgc-2.6.4/test/rml/csv/RMLTC0020a/RMLTC0020a_CSV.py` & `morph_kgc-2.7.0/test/rml-core/csv/RMLTC0020a/RMLTC0020a_CSV.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/rml/csv/RMLTC0020a/mapping.ttl` & `morph_kgc-2.7.0/test/rml-core/csv/RMLTC0020a/mapping.ttl`

 * *Files 18% similar despite different names*

```diff
@@ -1,28 +1,26 @@
-@prefix rr: <http://www.w3.org/ns/r2rml#> .
 @prefix foaf: <http://xmlns.com/foaf/0.1/> .
 @prefix rdfs: <http://www.w3.org/2000/01/rdf-schema#> .
 @prefix ex: <http://example.com/> .
 @prefix xsd: <http://www.w3.org/2001/XMLSchema#> .
-@prefix rml: <http://semweb.mmlab.be/ns/rml#> .
-@prefix ql: <http://semweb.mmlab.be/ns/ql#> .
+@prefix rml: <http://w3id.org/rml/> .
 @prefix rdf: <http://www.w3.org/1999/02/22-rdf-syntax-ns#> .
 
 @base <http://example.com/base/> .
 
 <TriplesMap1>
-  a rr:TriplesMap;
+  a rml:TriplesMap;
 
   rml:logicalSource [
-    rml:source "test/rml/csv/RMLTC0020a/student.csv";
-    rml:referenceFormulation ql:CSV
+    rml:source "test/rml-core/csv/RMLTC0020a/student.csv";
+    rml:referenceFormulation rml:CSV
   ];
 
-  rr:subjectMap [
-    rr:template "{Name}";
-    rr:termType rr:IRI
+  rml:subjectMap [
+    rml:template "{Name}";
+    rml:termType rml:IRI
   ];
 
-  rr:predicateObjectMap [
-    rr:predicate rdf:type;
-    rr:object foaf:Person
+  rml:predicateObjectMap [
+    rml:predicate rdf:type;
+    rml:object foaf:Person
   ].
```

### Comparing `morph_kgc-2.6.4/test/rml/csv/RMLTC0020a/output.nq` & `morph_kgc-2.7.0/test/rml-core/csv/RMLTC0020a/output.nq`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/rml/csv/RMLTC0020b/RMLTC0020b_CSV.py` & `morph_kgc-2.7.0/test/rml-core/csv/RMLTC0020b/RMLTC0020b_CSV.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/rml/csv/RMLTC0020b/mapping.ttl` & `morph_kgc-2.7.0/test/rml-core/json/RMLTC0020a/mapping.ttl`

 * *Files 14% similar despite different names*

```diff
@@ -1,24 +1,27 @@
-@prefix rr: <http://www.w3.org/ns/r2rml#> .
 @prefix foaf: <http://xmlns.com/foaf/0.1/> .
+@prefix rdfs: <http://www.w3.org/2000/01/rdf-schema#> .
 @prefix ex: <http://example.com/> .
 @prefix xsd: <http://www.w3.org/2001/XMLSchema#> .
+@prefix rml: <http://w3id.org/rml/> .
 @prefix rdf: <http://www.w3.org/1999/02/22-rdf-syntax-ns#> .
-@prefix rml:    <http://semweb.mmlab.be/ns/rml#> .
-@prefix ql:     <http://semweb.mmlab.be/ns/ql#> .
 
 @base <http://example.com/base/> .
 
 <TriplesMap1>
-  a rr:TriplesMap;
+  a rml:TriplesMap;
+
   rml:logicalSource [
-    rml:source "test/rml/csv/RMLTC0020b/student.csv";
-    rml:referenceFormulation ql:CSV
+    rml:source "test/rml-core/json/RMLTC0020a/student.json";
+    rml:referenceFormulation rml:JSONPath;
+    rml:iterator "$.students[*]"
   ];
 
-    rr:subjectMap [ rml:reference "Name"; rr:termType rr:IRI; ];
+  rml:subjectMap [
+    rml:template "{Name}";
+    rml:termType rml:IRI
+  ];
 
-    rr:predicateObjectMap
-    [
-    	rr:predicate rdf:type;
-    	rr:object foaf:Person;
-    ].
+  rml:predicateObjectMap [
+    rml:predicate rdf:type;
+    rml:object foaf:Person
+  ].
```

### Comparing `morph_kgc-2.6.4/test/rml/csv/null_filter/mapping.ttl` & `morph_kgc-2.7.0/test/rml-core/json/RMLTC0012a/mapping.ttl`

 * *Files 18% similar despite different names*

```diff
@@ -1,29 +1,32 @@
-@prefix rr: <http://www.w3.org/ns/r2rml#> .
 @prefix foaf: <http://xmlns.com/foaf/0.1/> .
 @prefix ex: <http://example.com/> .
 @prefix xsd: <http://www.w3.org/2001/XMLSchema#> .
-@prefix rml: <http://semweb.mmlab.be/ns/rml#> .
-@prefix ql: <http://semweb.mmlab.be/ns/ql#> .
+@prefix rml: <http://w3id.org/rml/> .
+
 @base <http://example.com/base/> .
 
-<TriplesMap1> a rr:TriplesMap;
+<TriplesMap1>
+  a rml:TriplesMap;
 
   rml:logicalSource [
-    rml:source "test/rml/csv/null_filter/student.csv";
-    rml:referenceFormulation ql:CSV
+    rml:source "test/rml-core/json/RMLTC0012a/persons.json";
+    rml:referenceFormulation rml:JSONPath;
+    rml:iterator "$.persons[*]"
   ];
 
-  rr:subjectMap [
-    rr:template "http://example.com/{ID}/{Name}";
-    rr:class foaf:Person
-  ];
+  rml:subjectMap [ rml:template "{fname}{lname}{amount}"; rml:termType rml:BlankNode; ];
 
-  rr:predicateObjectMap [
-    rr:predicate ex:id ;
-    rr:objectMap [ rml:reference "ID" ]
+  rml:predicateObjectMap [
+    rml:predicate foaf:name ;
+    rml:objectMap [
+      rml:template "{fname} {lname}";
+      rml:termType rml:Literal ;
+    ]
   ];
 
-  rr:predicateObjectMap [
-    rr:predicate foaf:name ;
-    rr:objectMap [ rml:reference "Name" ]
+  rml:predicateObjectMap [
+    rml:predicate ex:amount ;
+    rml:objectMap    [
+      rml:reference "amount";
+    ]
   ].
```

### Comparing `morph_kgc-2.6.4/test/rml/csv/null_filter/test_null_filter_CSV.py` & `morph_kgc-2.7.0/test/rml-core/csv/null_filter/test_null_filter_CSV.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/rml/csv/triples_map_without_pom/mapping.ttl` & `morph_kgc-2.7.0/test/rml-core/xml/RMLTC0008b/mapping.ttl`

 * *Files 18% similar despite different names*

```diff
@@ -1,41 +1,58 @@
-@prefix rr: <http://www.w3.org/ns/r2rml#> .
 @prefix foaf: <http://xmlns.com/foaf/0.1/> .
 @prefix ex: <http://example.com/> .
 @prefix xsd: <http://www.w3.org/2001/XMLSchema#> .
-@prefix rml: <http://semweb.mmlab.be/ns/rml#> .
-@prefix ql: <http://semweb.mmlab.be/ns/ql#> .
+@prefix rml: <http://w3id.org/rml/> .
 @prefix activity: <http://example.com/activity/> .
-@prefix rdfs: <http://www.w3.org/2000/01/rdf-schema#> .
+@prefix rdf: <http://www.w3.org/1999/02/22-rdf-syntax-ns#> .
 @base <http://example.com/base/> .
 
-<TriplesMap1>
-  a rr:TriplesMap;
-
+<TriplesMap2>
+  a rml:TriplesMap;
   rml:logicalSource [
-    rml:source "test/rml/csv/triples_map_without_pom/student.csv";
-    rml:referenceFormulation ql:CSV
+    rml:source "test/rml-core/xml/RMLTC0008b/student.xml";
+    rml:referenceFormulation rml:XPath;
+    rml:iterator "/students/student"
   ];
 
-  rr:subjectMap [ rr:template "http://example.com/resource/student_{ID}" ];
+  rml:subjectMap [ rml:template "http://example.com/{Sport}" ];
 
-  rr:predicateObjectMap [
-    rr:predicate <http://example.com/ontology/practises> ;
-    rr:objectMap [
-      a rr:RefObjectMap ;
-      rr:parentTriplesMap <TriplesMap2>;
-      rr:joinCondition [
-        rr:child "Sport" ;
-        rr:parent "ID" ;
-      ]
-    ]
+  rml:predicateObjectMap [
+    rml:predicate rdf:type ;
+    rml:object activity:Sport ;
   ] .
 
-<TriplesMap2>
-  a rr:TriplesMap;
+<TriplesMap1>
+  a rml:TriplesMap;
 
   rml:logicalSource [
-    rml:source "test/rml/csv/triples_map_without_pom/sport.csv";
-    rml:referenceFormulation ql:CSV
+    rml:source "test/rml-core/xml/RMLTC0008b/student.xml";
+    rml:referenceFormulation rml:XPath;
+    rml:iterator "/students/student"
+  ];
+
+  rml:subjectMap [ rml:template "http://example.com/Student/{ID}/{Name}" ];
+
+  rml:predicateObjectMap [
+    rml:predicate rdf:type ;
+    rml:object foaf:Person ;
   ];
 
-  rr:subjectMap [ rr:template "http://example.com/resource/sport_{ID}" ].
+  rml:predicateObjectMap [
+    rml:predicate ex:id ;
+    rml:objectMap [ rml:reference "ID"; ]
+  ];
+
+  rml:predicateObjectMap [
+    rml:predicate foaf:name ;
+    rml:objectMap [ rml:reference "Name" ]
+  ];
+
+  rml:predicateObjectMap [
+    rml:predicate ex:Sport ;
+    rml:objectMap <RefObjectMap1>
+  ] .
+
+
+<RefObjectMap1>
+  a rml:RefObjectMap;
+  rml:parentTriplesMap <TriplesMap2> .
```

### Comparing `morph_kgc-2.6.4/test/rml/csv/triples_map_without_pom/test_triples_map_without_pom_CSV.py` & `morph_kgc-2.7.0/test/rml-core/csv/triples_map_without_pom/test_triples_map_without_pom_CSV.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/rml/json/RMLTC0000/mapping.ttl` & `morph_kgc-2.7.0/test/rml-core/csv/RMLTC0001b/mapping.ttl`

 * *Files 14% similar despite different names*

```diff
@@ -1,28 +1,25 @@
-@prefix rr: <http://www.w3.org/ns/r2rml#> .
 @prefix foaf: <http://xmlns.com/foaf/0.1/> .
 @prefix ex: <http://example.com/> .
 @prefix xsd: <http://www.w3.org/2001/XMLSchema#> .
-@prefix rml: <http://semweb.mmlab.be/ns/rml#> .
-@prefix ql: <http://semweb.mmlab.be/ns/ql#> .
-
+@prefix rml: <http://w3id.org/rml/> .
 @base <http://example.com/base/> .
 
 <TriplesMap1>
-  a rr:TriplesMap;
+  a rml:TriplesMap;
 
   rml:logicalSource [
-    rml:source "test/rml/json/RMLTC0000/student.json";
-    rml:referenceFormulation ql:JSONPath;
-    rml:iterator "$.students[*]"
-  ] ;
+    rml:source "test/rml-core/csv/RMLTC0001b/student.csv";
+    rml:referenceFormulation rml:CSV
+  ];
 
-  rr:subjectMap [
-    rr:template "http://example.com/{Name}"
+  rml:subjectMap [
+    rml:template "{Name}";
+    rml:termType rml:BlankNode
   ];
 
-  rr:predicateObjectMap [
-    rr:predicate foaf:name ;
-    rr:objectMap [
+  rml:predicateObjectMap [
+    rml:predicate foaf:name;
+    rml:objectMap [
       rml:reference "Name"
     ]
   ].
```

### Comparing `morph_kgc-2.6.4/test/rml/json/RMLTC0000/test_RMLTC0000_JSON.py` & `morph_kgc-2.7.0/test/rml-core/json/RMLTC0000/test_RMLTC0000_JSON.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/rml/json/RMLTC0001a/mapping.ttl` & `morph_kgc-2.7.0/test/rml-core/json/RMLTC0005a/mapping.ttl`

 * *Files 14% similar despite different names*

```diff
@@ -1,28 +1,23 @@
-@prefix rr: <http://www.w3.org/ns/r2rml#> .
 @prefix foaf: <http://xmlns.com/foaf/0.1/> .
 @prefix ex: <http://example.com/> .
 @prefix xsd: <http://www.w3.org/2001/XMLSchema#> .
-@prefix rml: <http://semweb.mmlab.be/ns/rml#> .
-@prefix ql: <http://semweb.mmlab.be/ns/ql#> .
-
+@prefix rml: <http://w3id.org/rml/> .
 @base <http://example.com/base/> .
 
-<TriplesMap1>
-  a rr:TriplesMap;
+<TriplesMap1> a rml:TriplesMap;
 
   rml:logicalSource [
-    rml:source "test/rml/json/RMLTC0001a/student.json";
-    rml:referenceFormulation ql:JSONPath;
-    rml:iterator "$.students[*]"
+    rml:source "test/rml-core/json/RMLTC0005a/ious.json";
+    rml:referenceFormulation rml:JSONPath;
+    rml:iterator "$.persons[*]"
   ];
 
-  rr:subjectMap <#NameSubjectMap> ;
+  rml:subjectMap [
+    rml:template "http://example.com/{fname};{lname}";
+    rml:class foaf:Person;
+  ];
 
-  rr:predicateObjectMap [
-    rr:predicate foaf:name;
-    rr:objectMap [
-      rml:reference "Name"
-    ]
+  rml:predicateObjectMap [
+    rml:predicate ex:owes;
+    rml:objectMap [ rml:reference "amount"; ]
   ].
-
-<#NameSubjectMap> rr:template "http://example.com/{Name}" .
```

### Comparing `morph_kgc-2.6.4/test/rml/json/RMLTC0001a/test_RMLTC0001a_JSON.py` & `morph_kgc-2.7.0/test/rml-core/json/RMLTC0001a/test_RMLTC0001a_JSON.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/rml/json/RMLTC0001b/mapping.ttl` & `morph_kgc-2.7.0/test/rml-core/json/RMLTC0010c/mapping.ttl`

 * *Files 16% similar despite different names*

```diff
@@ -1,28 +1,22 @@
-@prefix rr: <http://www.w3.org/ns/r2rml#> .
 @prefix foaf: <http://xmlns.com/foaf/0.1/> .
 @prefix ex: <http://example.com/> .
 @prefix xsd: <http://www.w3.org/2001/XMLSchema#> .
-@prefix rml: <http://semweb.mmlab.be/ns/rml#> .
-@prefix ql: <http://semweb.mmlab.be/ns/ql#> .
+@prefix rml: <http://w3id.org/rml/> .
+@prefix activity: <http://example.com/activity/> .
 @base <http://example.com/base/> .
 
 <TriplesMap1>
-  a rr:TriplesMap;
+  a rml:TriplesMap;
 
   rml:logicalSource [
-    rml:source "test/rml/json/RMLTC0001b/student.json";
-    rml:referenceFormulation ql:JSONPath;
-    rml:iterator "$.students[*]"
+    rml:source "test/rml-core/json/RMLTC0010c/country_info.json";
+    rml:referenceFormulation rml:JSONPath;
+    rml:iterator "$.countries[*]"
   ];
 
-  rr:subjectMap [
-    rr:template "{Name}";
-    rr:termType rr:BlankNode
-  ];
+  rml:subjectMap [ rml:template "http://example.com/{Country Code}/{Name}" ];
 
-  rr:predicateObjectMap [
-    rr:predicate foaf:name;
-    rr:objectMap [
-      rml:reference "Name"
-    ]
-  ].
+  rml:predicateObjectMap [
+    rml:predicate ex:code ;
+    rml:objectMap [ rml:template "\\{\\{\\{ {ISO 3166} \\}\\}\\}"; rml:termType rml:Literal]
+  ] .
```

### Comparing `morph_kgc-2.6.4/test/rml/json/RMLTC0001b/test_RMLTC0001b_JSON.py` & `morph_kgc-2.7.0/test/rml-core/json/RMLTC0001b/test_RMLTC0001b_JSON.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/rml/json/RMLTC0002a/mapping.ttl` & `morph_kgc-2.7.0/test/rml-core/xml/RMLTC0012c/mapping.ttl`

 * *Files 17% similar despite different names*

```diff
@@ -1,30 +1,30 @@
-@prefix rr: <http://www.w3.org/ns/r2rml#> .
 @prefix foaf: <http://xmlns.com/foaf/0.1/> .
 @prefix ex: <http://example.com/> .
 @prefix xsd: <http://www.w3.org/2001/XMLSchema#> .
-@prefix rml: <http://semweb.mmlab.be/ns/rml#> .
-@prefix ql: <http://semweb.mmlab.be/ns/ql#> .
+@prefix rml: <http://w3id.org/rml/> .
+
 @base <http://example.com/base/> .
 
-<TriplesMap1> a rr:TriplesMap;
+<TriplesMap1>
+  a rml:TriplesMap;
 
   rml:logicalSource [
-    rml:source "test/rml/json/RMLTC0002a/student.json";
-    rml:referenceFormulation ql:JSONPath;
-    rml:iterator "$.students[*]"
-  ];
-
-  rr:subjectMap [
-    rr:template "http://example.com/{ID}/{Name}";
-    rr:class foaf:Person
+    rml:source "test/rml-core/xml/RMLTC0012c/persons.xml";
+    rml:referenceFormulation rml:XPath;
+    rml:iterator "/Persons/Person"
   ];
 
-  rr:predicateObjectMap [
-    rr:predicate ex:id ;
-    rr:objectMap [ rml:reference "ID" ]
+  rml:predicateObjectMap [
+    rml:predicate foaf:name ;
+    rml:objectMap [
+      rml:template "{fname} {lname}";
+      rml:termType rml:Literal ;
+    ]
   ];
 
-  rr:predicateObjectMap [
-    rr:predicate foaf:name ;
-    rr:objectMap [ rml:reference "Name" ]
+  rml:predicateObjectMap [
+    rml:predicate ex:amount ;
+    rml:objectMap    [
+      rml:reference "amount";
+    ]
   ].
```

### Comparing `morph_kgc-2.6.4/test/rml/json/RMLTC0002a/test_RMLTC0002a_JSON.py` & `morph_kgc-2.7.0/test/rml-core/json/RMLTC0002a/test_RMLTC0002a_JSON.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/rml/json/RMLTC0002b/mapping.ttl` & `morph_kgc-2.7.0/test/rml-core/xml/RMLTC0002a/mapping.ttl`

 * *Files 18% similar despite different names*

```diff
@@ -1,25 +1,28 @@
-@prefix rr: <http://www.w3.org/ns/r2rml#> .
 @prefix foaf: <http://xmlns.com/foaf/0.1/> .
 @prefix ex: <http://example.com/> .
 @prefix xsd: <http://www.w3.org/2001/XMLSchema#> .
-@prefix rml: <http://semweb.mmlab.be/ns/rml#> .
-@prefix ql: <http://semweb.mmlab.be/ns/ql#> .
+@prefix rml: <http://w3id.org/rml/> .
 @base <http://example.com/base/> .
 
-<TriplesMap1> a rr:TriplesMap;
+<TriplesMap1> a rml:TriplesMap;
 
   rml:logicalSource [
-    rml:source "test/rml/json/RMLTC0002b/student.json";
-    rml:referenceFormulation ql:JSONPath;
-    rml:iterator "$.students[*]"
+    rml:source "test/rml-core/xml/RMLTC0002a/student.xml";
+    rml:referenceFormulation rml:XPath;
+    rml:iterator "/students/student"
   ];
 
-  rr:subjectMap [
-    rr:template "students{ID}";
-    rr:termType rr:BlankNode
+  rml:subjectMap [
+    rml:template "http://example.com/{ID}/{Name}";
+    rml:class foaf:Person
   ];
 
-  rr:predicateObjectMap [
-    rr:predicate foaf:name;
-    rr:objectMap [ rml:reference "Name" ]
+  rml:predicateObjectMap [
+    rml:predicate ex:id ;
+    rml:objectMap [ rml:reference "ID" ]
+  ];
+
+  rml:predicateObjectMap [
+    rml:predicate foaf:name ;
+    rml:objectMap [ rml:reference "Name" ]
   ].
```

### Comparing `morph_kgc-2.6.4/test/rml/json/RMLTC0002b/test_RMLTC0002b_JSON.py` & `morph_kgc-2.7.0/test/rml-core/json/RMLTC0002b/test_RMLTC0002b_JSON.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/rml/json/RMLTC0002c/mapping.ttl` & `morph_kgc-2.7.0/test/rml-core/json/RMLTC0007a/mapping.ttl`

 * *Files 16% similar despite different names*

```diff
@@ -1,24 +1,23 @@
-@prefix rr: <http://www.w3.org/ns/r2rml#> .
 @prefix foaf: <http://xmlns.com/foaf/0.1/> .
 @prefix ex: <http://example.com/> .
 @prefix xsd: <http://www.w3.org/2001/XMLSchema#> .
-@prefix rml: <http://semweb.mmlab.be/ns/rml#> .
-@prefix ql: <http://semweb.mmlab.be/ns/ql#> .
+@prefix rml: <http://w3id.org/rml/> .
+@prefix rdf: <http://www.w3.org/1999/02/22-rdf-syntax-ns#> .
 @base <http://example.com/base/> .
 
-<TriplesMap1> a rr:TriplesMap;
+<TriplesMap1> a rml:TriplesMap;
 
   rml:logicalSource [
-    rml:source "test/rml/json/RMLTC0002c/student.json";
-    rml:referenceFormulation ql:JSONPath;
+    rml:source "test/rml-core/json/RMLTC0007a/student.json";
+    rml:referenceFormulation rml:JSONPath;
     rml:iterator "$.students[*]"
   ];
 
-  rr:subjectMap [
-    rr:template "http://example.com/{ID}/{Name}";
+  rml:subjectMap [
+    rml:template "http://example.com/Student/{ID}/{FirstName}"
   ];
 
-  rr:predicateObjectMap [
-    rr:predicate ex:id ;
-    rr:objectMap [ rml:reference "IDs" ]
+  rml:predicateObjectMap [
+    rml:predicate rdf:type;
+    rml:object foaf:Person;
   ].
```

### Comparing `morph_kgc-2.6.4/test/rml/json/RMLTC0002c/test_RMLTC0002c_JSON.py` & `morph_kgc-2.7.0/test/rml-core/json/RMLTC0002c/test_RMLTC0002c_JSON.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/rml/json/RMLTC0002e/mapping.ttl` & `morph_kgc-2.7.0/test/rml-core/json/RMLTC0015a/mapping.ttl`

 * *Files 17% similar despite different names*

```diff
@@ -1,24 +1,48 @@
-@prefix rr: <http://www.w3.org/ns/r2rml#> .
 @prefix foaf: <http://xmlns.com/foaf/0.1/> .
 @prefix ex: <http://example.com/> .
 @prefix xsd: <http://www.w3.org/2001/XMLSchema#> .
-@prefix rml: <http://semweb.mmlab.be/ns/rml#> .
-@prefix ql: <http://semweb.mmlab.be/ns/ql#> .
+@prefix rml: <http://w3id.org/rml/> .
+@prefix rdfs: <http://www.w3.org/2000/01/rdf-schema#> .
 @base <http://example.com/base/> .
 
-<TriplesMap1> a rr:TriplesMap;
+<TriplesMap1>
+  a rml:TriplesMap;
 
   rml:logicalSource [
-    rml:source "test/rml/json/RMLTC0002e/student2.json";
-    rml:referenceFormulation ql:JSONPath;
-    rml:iterator "$.students[*]"
+    rml:source "test/rml-core/json/RMLTC0015a/country_en.json";
+    rml:referenceFormulation rml:JSONPath;
+    rml:iterator "$.countries[*]"
   ];
 
-  rr:subjectMap [
-    rr:template "http://example.com/{ID}/{Name}";
+  rml:subjectMap [
+    rml:template "http://example.com/{Code}"
   ];
 
-  rr:predicateObjectMap [
-    rr:predicate ex:id ;
-    rr:objectMap [ rml:reference "ID" ]
+  rml:predicateObjectMap [
+    rml:predicate rdfs:label ;
+    rml:objectMap [
+      rml:reference "Name";
+      rml:language "en"
+    ]
+  ].
+
+<TriplesMap2>
+  a rml:TriplesMap;
+
+  rml:logicalSource [
+    rml:source "test/rml-core/json/RMLTC0015a/country_es.json";
+    rml:referenceFormulation rml:JSONPath;
+    rml:iterator "$.countries[*]"
+  ];
+
+  rml:subjectMap [
+    rml:template "http://example.com/{Code}"
+  ];
+
+  rml:predicateObjectMap [
+    rml:predicate rdfs:label ;
+    rml:objectMap [
+      rml:reference "Name";
+      rml:language "es"
+    ]
   ].
```

### Comparing `morph_kgc-2.6.4/test/rml/json/RMLTC0002e/test_RMLTC0002e_JSON.py` & `morph_kgc-2.7.0/test/rml-core/json/RMLTC0002e/test_RMLTC0002e_JSON.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/rml/json/RMLTC0003c/mapping.ttl` & `morph_kgc-2.7.0/test/rml-core/xml/RMLTC0004b/mapping.ttl`

 * *Files 15% similar despite different names*

```diff
@@ -1,27 +1,27 @@
-@prefix rr: <http://www.w3.org/ns/r2rml#> .
 @prefix foaf: <http://xmlns.com/foaf/0.1/> .
 @prefix ex: <http://example.com/> .
 @prefix xsd: <http://www.w3.org/2001/XMLSchema#> .
-@prefix rml: <http://semweb.mmlab.be/ns/rml#> .
-@prefix ql: <http://semweb.mmlab.be/ns/ql#> .
+@prefix rml: <http://w3id.org/rml/> .
+
 @base <http://example.com/base/> .
 
-<TriplesMap1> a rr:TriplesMap;
+<TriplesMap1>
+  a rml:TriplesMap;
 
   rml:logicalSource [
-    rml:source "test/rml/json/RMLTC0003c/student.json";
-    rml:referenceFormulation ql:JSONPath;
-    rml:iterator "$.students[*]"
+    rml:source "test/rml-core/xml/RMLTC0004b/student.xml";
+    rml:referenceFormulation rml:XPath;
+    rml:iterator "/students/student"
   ];
 
-  rr:subjectMap [
-    rr:template "http://example.com/Student{ID}";
+  rml:subjectMap [
+    rml:template "http://example.com/{Name}";
+    rml:termType rml:Literal
   ];
 
-  rr:predicateObjectMap [
-    rr:predicate foaf:name ;
-    rr:objectMap [
-      rr:template "{FirstName} {LastName}";
-      rr:termType rr:Literal;
+  rml:predicateObjectMap [
+    rml:predicate foaf:name;
+    rml:objectMap [
+      rml:reference "Name"
     ]
   ].
```

### Comparing `morph_kgc-2.6.4/test/rml/json/RMLTC0003c/test_RMLTC0003c_JSON.py` & `morph_kgc-2.7.0/test/rml-core/json/RMLTC0003c/test_RMLTC0003c_JSON.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/rml/json/RMLTC0004a/mapping.ttl` & `morph_kgc-2.7.0/test/rml-core/json/RMLTC0007f/mapping.ttl`

 * *Files 18% similar despite different names*

```diff
@@ -1,47 +1,34 @@
-@prefix rr: <http://www.w3.org/ns/r2rml#> .
 @prefix foaf: <http://xmlns.com/foaf/0.1/> .
 @prefix ex: <http://example.com/> .
 @prefix xsd: <http://www.w3.org/2001/XMLSchema#> .
-@prefix rml: <http://semweb.mmlab.be/ns/rml#> .
-@prefix ql: <http://semweb.mmlab.be/ns/ql#> .
+@prefix rml: <http://w3id.org/rml/> .
+@prefix rdf: <http://www.w3.org/1999/02/22-rdf-syntax-ns#> .
 @base <http://example.com/base/> .
 
-<TriplesMap1> a rr:TriplesMap;
+<TriplesMap1> a rml:TriplesMap;
 
   rml:logicalSource [
-    rml:source "test/rml/json/RMLTC0004a/student_sport.json";
-    rml:referenceFormulation ql:JSONPath;
+    rml:source "test/rml-core/json/RMLTC0007f/student.json";
+    rml:referenceFormulation rml:JSONPath;
     rml:iterator "$.students[*]"
   ];
 
-  rr:subjectMap [
-    rr:template "http://example.com/{Student}";
-    rr:class ex:Student
+  rml:subjectMap [
+    rml:template "http://example.com/Student/{ID}/{FirstName}";
+    rml:graph ex:PersonGraph
   ];
 
-  rr:predicateObjectMap [
-    rr:predicate foaf:name ;
-    rr:objectMap [
-      rml:reference "Student"
-    ]
-  ].
-
-<TriplesMap2> a rr:TriplesMap;
-
-  rml:logicalSource [
-    rml:source "test/rml/json/RMLTC0004a/student_sport.json";
-    rml:referenceFormulation ql:JSONPath;
-    rml:iterator "$.students[*]"
+  rml:predicateObjectMap [
+    rml:predicate rdf:type;
+    rml:object foaf:Person
   ];
 
-  rr:subjectMap [
-    rr:template "http://example.com/{Sport}";
-    rr:class ex:Sport
+  rml:predicateObjectMap [
+    rml:predicate ex:id ;
+    rml:objectMap [ rml:reference "ID";  ]
   ];
 
-  rr:predicateObjectMap [
-    rr:predicate foaf:name ;
-    rr:objectMap [
-      rml:reference "Sport"
-    ]
+  rml:predicateObjectMap [
+    rml:predicate foaf:name ;
+    rml:objectMap [ rml:reference "FirstName" ]
   ].
```

### Comparing `morph_kgc-2.6.4/test/rml/json/RMLTC0004a/test_RMLTC0004a_JSON.py` & `morph_kgc-2.7.0/test/rml-core/json/RMLTC0004a/test_RMLTC0004a_JSON.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/rml/json/RMLTC0004b/mapping.ttl` & `morph_kgc-2.7.0/test/rml-core/xml/RMLTC0002c/mapping.ttl`

 * *Files 15% similar despite different names*

```diff
@@ -1,29 +1,22 @@
-@prefix rr: <http://www.w3.org/ns/r2rml#> .
 @prefix foaf: <http://xmlns.com/foaf/0.1/> .
 @prefix ex: <http://example.com/> .
 @prefix xsd: <http://www.w3.org/2001/XMLSchema#> .
-@prefix rml: <http://semweb.mmlab.be/ns/rml#> .
-@prefix ql: <http://semweb.mmlab.be/ns/ql#> .
-
+@prefix rml: <http://w3id.org/rml/> .
 @base <http://example.com/base/> .
 
-<TriplesMap1>
-  a rr:TriplesMap;
+<TriplesMap1> a rml:TriplesMap;
 
   rml:logicalSource [
-    rml:source "test/rml/json/RMLTC0004b/student.json";
-    rml:referenceFormulation ql:JSONPath;
-    rml:iterator "$.students[*]"
+    rml:source "test/rml-core/xml/RMLTC0002c/student.xml";
+    rml:referenceFormulation rml:XPath;
+    rml:iterator "/students/student"
   ];
 
-  rr:subjectMap [
-    rr:template "http://example.com/{Name}";
-    rr:termType rr:Literal
+  rml:subjectMap [
+    rml:template "http://example.com/{ID}/{Name}";
   ];
 
-  rr:predicateObjectMap [
-    rr:predicate foaf:name;
-    rr:objectMap [
-      rml:reference "Name"
-    ]
+  rml:predicateObjectMap [
+    rml:predicate ex:id ;
+    rml:objectMap [ rml:reference "IDs" ]
   ].
```

### Comparing `morph_kgc-2.6.4/test/rml/json/RMLTC0004b/test_RMLTC0004b_JSON.py` & `morph_kgc-2.7.0/test/rml-core/json/RMLTC0004b/test_RMLTC0004b_JSON.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/rml/json/RMLTC0005a/mapping.ttl` & `morph_kgc-2.7.0/test/rml-core/xml/RMLTC0012b/mapping.ttl`

 * *Files 21% similar despite different names*

```diff
@@ -1,25 +1,52 @@
-@prefix rr: <http://www.w3.org/ns/r2rml#> .
 @prefix foaf: <http://xmlns.com/foaf/0.1/> .
 @prefix ex: <http://example.com/> .
 @prefix xsd: <http://www.w3.org/2001/XMLSchema#> .
-@prefix rml: <http://semweb.mmlab.be/ns/rml#> .
-@prefix ql: <http://semweb.mmlab.be/ns/ql#> .
+@prefix rml: <http://w3id.org/rml/> .
+
 @base <http://example.com/base/> .
 
-<TriplesMap1> a rr:TriplesMap;
+<TriplesMap1>
+  a rml:TriplesMap;
+
+  rml:logicalSource [
+    rml:source "test/rml-core/xml/RMLTC0012b/persons.xml";
+    rml:referenceFormulation rml:XPath;
+    rml:iterator "/Persons/Person"
+  ];
+
+  rml:subjectMap [
+    rml:template "{fname}{lname}";
+    rml:termType rml:BlankNode ;
+  ];
+
+  rml:predicateObjectMap [
+    rml:predicate foaf:name ;
+    rml:objectMap [
+      rml:template "{fname} {lname}";
+      rml:termType rml:Literal ;
+    ]
+  ];
+  .
+
+<TriplesMap2>
+  a rml:TriplesMap;
 
   rml:logicalSource [
-    rml:source "test/rml/json/RMLTC0005a/ious.json";
-    rml:referenceFormulation ql:JSONPath;
-    rml:iterator "$.persons[*]"
+    rml:source "test/rml-core/xml/RMLTC0012b/lives.xml";
+    rml:referenceFormulation rml:XPath;
+    rml:iterator "/Lives/Live"
   ];
 
-  rr:subjectMap [
-    rr:template "http://example.com/{fname};{lname}";
-    rr:class foaf:Person;
+  rml:subjectMap [
+    rml:template "{fname}{lname}";
+    rml:termType rml:BlankNode;
   ];
 
-  rr:predicateObjectMap [
-    rr:predicate ex:owes;
-    rr:objectMap [ rml:reference "amount"; ]
-  ].
+  rml:predicateObjectMap
+  [
+    rml:predicate	ex:city ;
+    rml:objectMap    [
+      rml:reference "city";
+    ]
+];
+.
```

### Comparing `morph_kgc-2.6.4/test/rml/json/RMLTC0005a/test_RMLTC0005a_JSON.py` & `morph_kgc-2.7.0/test/rml-core/json/RMLTC0005a/test_RMLTC0005a_JSON.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/rml/json/RMLTC0006a/mapping.ttl` & `morph_kgc-2.7.0/test/rml-core/json/RMLTC0006a/mapping.ttl`

 * *Files 20% similar despite different names*

```diff
@@ -1,25 +1,23 @@
-@prefix rr: <http://www.w3.org/ns/r2rml#> .
 @prefix foaf: <http://xmlns.com/foaf/0.1/> .
 @prefix ex: <http://example.com/> .
 @prefix xsd: <http://www.w3.org/2001/XMLSchema#> .
-@prefix rml: <http://semweb.mmlab.be/ns/rml#> .
-@prefix ql: <http://semweb.mmlab.be/ns/ql#> .
+@prefix rml: <http://w3id.org/rml/> .
 @base <http://example.com/base/> .
 
-<TriplesMap1> a rr:TriplesMap;
+<TriplesMap1> a rml:TriplesMap;
 
   rml:logicalSource [
-    rml:source "test/rml/json/RMLTC0006a/student.json";
-    rml:referenceFormulation ql:JSONPath;
+    rml:source "test/rml-core/json/RMLTC0006a/student.json";
+    rml:referenceFormulation rml:JSONPath;
     rml:iterator "$.students[*]"
   ];
 
-  rr:subjectMap [
-    rr:constant ex:BadStudent;
-    rr:graphMap [ rr:constant <http://example.com/graph/student> ];
+  rml:subjectMap [
+    rml:constant ex:BadStudent;
+    rml:graphMap [ rml:constant <http://example.com/graph/student> ];
   ];
 
-  rr:predicateObjectMap [
-    rr:predicateMap [ rr:constant ex:description ];
-    rr:objectMap [ rr:constant "Bad Student"; ]
+  rml:predicateObjectMap [
+    rml:predicateMap [ rml:constant ex:description ];
+    rml:objectMap [ rml:constant "Bad Student"; ]
   ].
```

### Comparing `morph_kgc-2.6.4/test/rml/json/RMLTC0006a/test_RMLTC0006a_JSON.py` & `morph_kgc-2.7.0/test/rml-core/json/RMLTC0006a/test_RMLTC0006a_JSON.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/rml/json/RMLTC0007a/mapping.ttl` & `morph_kgc-2.7.0/test/rml-core/tabular/RMLTC0002a_FEATHER/mapping.ttl`

 * *Files 19% similar despite different names*

```diff
@@ -1,25 +1,27 @@
-@prefix rr: <http://www.w3.org/ns/r2rml#> .
 @prefix foaf: <http://xmlns.com/foaf/0.1/> .
 @prefix ex: <http://example.com/> .
 @prefix xsd: <http://www.w3.org/2001/XMLSchema#> .
-@prefix rml: <http://semweb.mmlab.be/ns/rml#> .
-@prefix ql: <http://semweb.mmlab.be/ns/ql#> .
-@prefix rdf: <http://www.w3.org/1999/02/22-rdf-syntax-ns#> .
+@prefix rml: <http://w3id.org/rml/> .
 @base <http://example.com/base/> .
 
-<TriplesMap1> a rr:TriplesMap;
+<TriplesMap1> a rml:TriplesMap;
 
   rml:logicalSource [
-    rml:source "test/rml/json/RMLTC0007a/student.json";
-    rml:referenceFormulation ql:JSONPath;
-    rml:iterator "$.students[*]"
+    rml:source "test/rml-core/tabular/RMLTC0002a_FEATHER/student.feather";
+    rml:referenceFormulation rml:CSV
   ];
 
-  rr:subjectMap [
-    rr:template "http://example.com/Student/{ID}/{FirstName}"
+  rml:subjectMap [
+    rml:template "http://example.com/{ID}/{Name}";
+    rml:class foaf:Person
   ];
 
-  rr:predicateObjectMap [
-    rr:predicate rdf:type;
-    rr:object foaf:Person;
+  rml:predicateObjectMap [
+    rml:predicate ex:id ;
+    rml:objectMap [ rml:reference "ID" ]
+  ];
+
+  rml:predicateObjectMap [
+    rml:predicate foaf:name ;
+    rml:objectMap [ rml:reference "Name" ]
   ].
```

### Comparing `morph_kgc-2.6.4/test/rml/json/RMLTC0007a/test_RMLTC0007a_JSON.py` & `morph_kgc-2.7.0/test/rml-core/json/RMLTC0007a/test_RMLTC0007a_JSON.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/rml/json/RMLTC0007b/mapping.ttl` & `morph_kgc-2.7.0/test/rml-core/xml/RMLTC0012d/mapping.ttl`

 * *Files 20% similar despite different names*

```diff
@@ -1,31 +1,34 @@
-@prefix rr: <http://www.w3.org/ns/r2rml#> .
 @prefix foaf: <http://xmlns.com/foaf/0.1/> .
 @prefix ex: <http://example.com/> .
 @prefix xsd: <http://www.w3.org/2001/XMLSchema#> .
-@prefix rml: <http://semweb.mmlab.be/ns/rml#> .
-@prefix ql: <http://semweb.mmlab.be/ns/ql#> .
-@prefix rdf: <http://www.w3.org/1999/02/22-rdf-syntax-ns#> .
+@prefix rml: <http://w3id.org/rml/> .
+
 @base <http://example.com/base/> .
 
-<TriplesMap1> a rr:TriplesMap;
+<TriplesMap1>
+  a rml:TriplesMap;
 
   rml:logicalSource [
-    rml:source "test/rml/json/RMLTC0007b/student.json";
-    rml:referenceFormulation ql:JSONPath;
-    rml:iterator "$.students[*]"
+    rml:source "test/rml-core/xml/RMLTC0012d/persons.xml";
+    rml:referenceFormulation rml:XPath;
+    rml:iterator "/Persons/Person"
   ];
 
-  rr:subjectMap [
-    rr:template "http://example.com/Student/{ID}/{FirstName}";
-    rr:graph ex:PersonGraph
-  ];
+  rml:subjectMap [ rml:template "{fname}_{lname}_{amount}"; rml:termType rml:BlankNode; ];
+
+  rml:subjectMap [ rml:template "{amount}_{fname}_{lname}"; rml:termType rml:BlankNode; ];
 
-  rr:predicateObjectMap [
-    rr:predicate rdf:type;
-    rr:object foaf:Person;
+  rml:predicateObjectMap [
+    rml:predicate foaf:name ;
+    rml:objectMap [
+      rml:template "{fname} {lname}";
+      rml:termType rml:Literal ;
+    ]
   ];
 
-  rr:predicateObjectMap [
-    rr:predicate foaf:name;
-    rr:objectMap [ rml:reference "FirstName" ]
+  rml:predicateObjectMap [
+    rml:predicate ex:amount ;
+    rml:objectMap    [
+      rml:reference "amount";
+    ]
   ].
```

### Comparing `morph_kgc-2.6.4/test/rml/json/RMLTC0007b/test_RMLTC0007b_JSON.py` & `morph_kgc-2.7.0/test/rml-core/json/RMLTC0007b/test_RMLTC0007b_JSON.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/rml/json/RMLTC0007c/mapping.ttl` & `morph_kgc-2.7.0/test/rml-core/json/RMLTC0007g/mapping.ttl`

 * *Files 17% similar despite different names*

```diff
@@ -1,30 +1,25 @@
-@prefix rr: <http://www.w3.org/ns/r2rml#> .
 @prefix foaf: <http://xmlns.com/foaf/0.1/> .
 @prefix ex: <http://example.com/> .
 @prefix xsd: <http://www.w3.org/2001/XMLSchema#> .
-@prefix rml: <http://semweb.mmlab.be/ns/rml#> .
-@prefix ql: <http://semweb.mmlab.be/ns/ql#> .
+@prefix rml: <http://w3id.org/rml/> .
 @base <http://example.com/base/> .
 
-<TriplesMap1> a rr:TriplesMap;
+<TriplesMap1> a rml:TriplesMap;
 
   rml:logicalSource [
-    rml:source "test/rml/json/RMLTC0007c/student.json";
-    rml:referenceFormulation ql:JSONPath;
+    rml:source "test/rml-core/json/RMLTC0007g/student.json";
+    rml:referenceFormulation rml:JSONPath;
     rml:iterator "$.students[*]"
   ];
 
-  rr:subjectMap [
-    rr:template "http://example.com/Student/{ID}/{FirstName}";
-    rr:class foaf:Person, ex:Student
+  rml:subjectMap [
+    rml:template "http://example.com/Student/{ID}/{FirstName}";
+    rml:graph rml:defaultGraph
   ];
 
-  rr:predicateObjectMap [
-    rr:predicate ex:id ;
-    rr:objectMap [ rml:reference "ID";  ]
-  ];
-
-  rr:predicateObjectMap [
-    rr:predicate foaf:name;
-    rr:objectMap [ rml:reference "FirstName" ]
+  rml:predicateObjectMap [
+    rml:predicate foaf:name;
+    rml:objectMap [
+      rml:reference "FirstName"
+    ]
   ].
```

### Comparing `morph_kgc-2.6.4/test/rml/json/RMLTC0007c/test_RMLTC0007c_JSON.py` & `morph_kgc-2.7.0/test/rml-core/json/RMLTC0007c/test_RMLTC0007c_JSON.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/rml/json/RMLTC0007d/mapping.ttl` & `morph_kgc-2.7.0/test/rml-in-memory/json_dictionary/RMLIMTC0007f/mapping.ttl`

 * *Files 22% similar despite different names*

```diff
@@ -1,40 +1,47 @@
-@prefix rr: <http://www.w3.org/ns/r2rml#> .
 @prefix foaf: <http://xmlns.com/foaf/0.1/> .
 @prefix ex: <http://example.com/> .
 @prefix xsd: <http://www.w3.org/2001/XMLSchema#> .
-@prefix rml: <http://semweb.mmlab.be/ns/rml#> .
-@prefix ql: <http://semweb.mmlab.be/ns/ql#> .
+@prefix rml: <http://w3id.org/rml/> .
 @prefix rdf: <http://www.w3.org/1999/02/22-rdf-syntax-ns#> .
 @base <http://example.com/base/> .
+@prefix sd: <https://w3id.org/okn/o/sd#>.
+@prefix kg4di: <https://w3id.org/kg4di/definedBy>.
 
-<TriplesMap1> a rr:TriplesMap;
+<TriplesMap1> a rml:TriplesMap;
 
   rml:logicalSource [
-    rml:source "test/rml/json/RMLTC0007d/student.json";
-    rml:referenceFormulation ql:JSONPath;
+    rml:source [
+			a sd:DatasetSpecification;
+			sd:name "variable1";
+			sd:hasDataTransformation [
+				sd:hasSourceCode [
+					sd:programmingLanguage "Python3.9";
+				];
+			];
+		];
+		rml:referenceFormulation rml:Dictionary;
     rml:iterator "$.students[*]"
   ];
 
-  rr:subjectMap [
-    rr:template "http://example.com/Student/{ID}/{FirstName}"
+  rml:subjectMap [
+    rml:template "http://example.com/Student/{ID}/{FirstName}";
+    rml:graph ex:PersonGraph
   ];
 
-  rr:predicateObjectMap [
-    rr:predicate rdf:type;
-    rr:object foaf:Person;
+  rml:predicateObjectMap [
+    rml:predicate rdf:type;
+    rml:object foaf:Person
   ];
 
-  rr:predicateObjectMap [
-    rr:predicate rdf:type;
-    rr:object ex:Student;
+  rml:predicateObjectMap [
+    rml:predicate ex:id ;
+    rml:objectMap [ rml:reference "ID";  ]
   ];
 
-  rr:predicateObjectMap [
-    rr:predicate ex:id;
-    rr:objectMap [rml:reference "ID"]
-  ];
-
-  rr:predicateObjectMap [
-    rr:predicate foaf:name;
-    rr:objectMap [ rml:reference "FirstName" ]
+  rml:predicateObjectMap [
+    rml:predicate foaf:name ;
+    rml:objectMap [ rml:reference "FirstName" ]
   ].
+
+rml:Dictionary a rml:ReferenceFormulation;
+	kg4di:definedBy "Python".
```

### Comparing `morph_kgc-2.6.4/test/rml/json/RMLTC0007d/test_RMLTC0007d_JSON.py` & `morph_kgc-2.7.0/test/rml-core/json/RMLTC0007d/test_RMLTC0007d_JSON.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/rml/json/RMLTC0007e/mapping.ttl` & `morph_kgc-2.7.0/test/rml-core/xml/RMLTC0007h/mapping.ttl`

 * *Files 20% similar despite different names*

```diff
@@ -1,31 +1,25 @@
-@prefix rr: <http://www.w3.org/ns/r2rml#> .
 @prefix foaf: <http://xmlns.com/foaf/0.1/> .
 @prefix ex: <http://example.com/> .
 @prefix xsd: <http://www.w3.org/2001/XMLSchema#> .
-@prefix rml: <http://semweb.mmlab.be/ns/rml#> .
-@prefix ql: <http://semweb.mmlab.be/ns/ql#> .
+@prefix rml: <http://w3id.org/rml/> .
 @base <http://example.com/base/> .
 
-<TriplesMap1> a rr:TriplesMap;
+<TriplesMap1> a rml:TriplesMap;
 
   rml:logicalSource [
-    rml:source "test/rml/json/RMLTC0007e/student.json";
-    rml:referenceFormulation ql:JSONPath;
-    rml:iterator "$.students[*]"
+    rml:source "test/rml-core/xml/RMLTC0007h/student.xml";
+    rml:referenceFormulation rml:XPath;
+    rml:iterator "/students/student"
   ];
 
-  rr:subjectMap [
-    rr:template "http://example.com/Student/{ID}/{Name}";
-    rr:graph ex:PersonGraph ;
-    rr:class foaf:Person
+  rml:subjectMap [
+    rml:template "http://example.com/Student/{ID}/{FirstName}";
+    rml:graphMap [ rml:reference "FirstName"; rml:termType rml:Literal; ]
   ];
 
-  rr:predicateObjectMap [
-    rr:predicate ex:id ;
-    rr:objectMap [ rml:reference "ID"; ]
-  ];
-
-  rr:predicateObjectMap [
-    rr:predicate foaf:name ;
-    rr:objectMap [ rml:reference "Name" ]
+  rml:predicateObjectMap [
+    rml:predicate foaf:name;
+    rml:objectMap [
+      rml:reference "FirstName"
+    ]
   ].
```

### Comparing `morph_kgc-2.6.4/test/rml/json/RMLTC0007e/test_RMLTC0007e_JSON.py` & `morph_kgc-2.7.0/test/rml-core/json/RMLTC0007e/test_RMLTC0007e_JSON.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/rml/json/RMLTC0007f/mapping.ttl` & `morph_kgc-2.7.0/test/rml-core/json/RMLTC0012d/mapping.ttl`

 * *Files 22% similar despite different names*

```diff
@@ -1,36 +1,34 @@
-@prefix rr: <http://www.w3.org/ns/r2rml#> .
 @prefix foaf: <http://xmlns.com/foaf/0.1/> .
 @prefix ex: <http://example.com/> .
 @prefix xsd: <http://www.w3.org/2001/XMLSchema#> .
-@prefix rml: <http://semweb.mmlab.be/ns/rml#> .
-@prefix ql: <http://semweb.mmlab.be/ns/ql#> .
-@prefix rdf: <http://www.w3.org/1999/02/22-rdf-syntax-ns#> .
+@prefix rml: <http://w3id.org/rml/> .
+
 @base <http://example.com/base/> .
 
-<TriplesMap1> a rr:TriplesMap;
+<TriplesMap1>
+  a rml:TriplesMap;
 
   rml:logicalSource [
-    rml:source "test/rml/json/RMLTC0007f/student.json";
-    rml:referenceFormulation ql:JSONPath;
-    rml:iterator "$.students[*]"
+    rml:source "test/rml-core/json/RMLTC0012d/persons.json";
+    rml:referenceFormulation rml:JSONPath;
+    rml:iterator "$.persons[*]"
   ];
 
-  rr:subjectMap [
-    rr:template "http://example.com/Student/{ID}/{FirstName}";
-    rr:graph ex:PersonGraph
-  ];
+  rml:subjectMap [ rml:template "{fname}_{lname}_{amount}"; rml:termType rml:BlankNode; ];
 
-  rr:predicateObjectMap [
-    rr:predicate rdf:type;
-    rr:object foaf:Person
-  ];
+  rml:subjectMap [ rml:template "{amount}_{fname}_{lname}"; rml:termType rml:BlankNode; ];
 
-  rr:predicateObjectMap [
-    rr:predicate ex:id ;
-    rr:objectMap [ rml:reference "ID";  ]
+  rml:predicateObjectMap [
+    rml:predicate foaf:name ;
+    rml:objectMap [
+      rml:template "{fname} {lname}";
+      rml:termType rml:Literal ;
+    ]
   ];
 
-  rr:predicateObjectMap [
-    rr:predicate foaf:name ;
-    rr:objectMap [ rml:reference "FirstName" ]
+  rml:predicateObjectMap [
+    rml:predicate ex:amount ;
+    rml:objectMap    [
+      rml:reference "amount";
+    ]
   ].
```

### Comparing `morph_kgc-2.6.4/test/rml/json/RMLTC0007f/test_RMLTC0007f_JSON.py` & `morph_kgc-2.7.0/test/rml-core/json/RMLTC0007f/test_RMLTC0007f_JSON.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/rml/json/RMLTC0007g/mapping.ttl` & `morph_kgc-2.7.0/test/rml-core/csv/RMLTC0007g/mapping.ttl`

 * *Files 14% similar despite different names*

```diff
@@ -1,27 +1,24 @@
-@prefix rr: <http://www.w3.org/ns/r2rml#> .
 @prefix foaf: <http://xmlns.com/foaf/0.1/> .
 @prefix ex: <http://example.com/> .
 @prefix xsd: <http://www.w3.org/2001/XMLSchema#> .
-@prefix rml: <http://semweb.mmlab.be/ns/rml#> .
-@prefix ql: <http://semweb.mmlab.be/ns/ql#> .
+@prefix rml: <http://w3id.org/rml/> .
 @base <http://example.com/base/> .
 
-<TriplesMap1> a rr:TriplesMap;
+<TriplesMap1> a rml:TriplesMap;
 
   rml:logicalSource [
-    rml:source "test/rml/json/RMLTC0007g/student.json";
-    rml:referenceFormulation ql:JSONPath;
-    rml:iterator "$.students[*]"
+    rml:source "test/rml-core/csv/RMLTC0007g/student.csv";
+    rml:referenceFormulation rml:CSV
   ];
 
-  rr:subjectMap [
-    rr:template "http://example.com/Student/{ID}/{FirstName}";
-    rr:graph rr:defaultGraph
+  rml:subjectMap [
+    rml:template "http://example.com/Student/{ID}/{FirstName}";
+    rml:graph rml:defaultGraph
   ];
 
-  rr:predicateObjectMap [
-    rr:predicate foaf:name;
-    rr:objectMap [
+  rml:predicateObjectMap [
+    rml:predicate foaf:name;
+    rml:objectMap [
       rml:reference "FirstName"
     ]
   ].
```

### Comparing `morph_kgc-2.6.4/test/rml/json/RMLTC0007g/test_RMLTC0007g_JSON.py` & `morph_kgc-2.7.0/test/rml-core/json/RMLTC0007g/test_RMLTC0007g_JSON.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/rml/json/RMLTC0007h/mapping.ttl` & `morph_kgc-2.7.0/test/rml-core/json/RMLTC0010b/mapping.ttl`

 * *Files 17% similar despite different names*

```diff
@@ -1,27 +1,22 @@
-@prefix rr: <http://www.w3.org/ns/r2rml#> .
 @prefix foaf: <http://xmlns.com/foaf/0.1/> .
 @prefix ex: <http://example.com/> .
 @prefix xsd: <http://www.w3.org/2001/XMLSchema#> .
-@prefix rml: <http://semweb.mmlab.be/ns/rml#> .
-@prefix ql: <http://semweb.mmlab.be/ns/ql#> .
+@prefix rml: <http://w3id.org/rml/> .
+@prefix activity: <http://example.com/activity/> .
 @base <http://example.com/base/> .
 
-<TriplesMap1> a rr:TriplesMap;
+<TriplesMap1>
+  a rml:TriplesMap;
 
   rml:logicalSource [
-    rml:source "test/rml/json/RMLTC0007h/student.json";
-    rml:referenceFormulation ql:JSONPath;
-    rml:iterator "$.students[*]"
+    rml:source "test/rml-core/json/RMLTC0010b/country_info.json";
+    rml:referenceFormulation rml:JSONPath;
+    rml:iterator "$.countries[*]"
   ];
 
-  rr:subjectMap [
-    rr:template "http://example.com/Student/{ID}/{FirstName}";
-    rr:graphMap [ rml:reference "FirstName"; rr:termType rr:Literal; ]
-  ];
+  rml:subjectMap [ rml:template "http://example.com/{Country Code}/{Name}" ];
 
-  rr:predicateObjectMap [
-    rr:predicate foaf:name;
-    rr:objectMap [
-      rml:reference "FirstName"
-    ]
-  ].
+  rml:predicateObjectMap [
+    rml:predicate ex:name ;
+    rml:objectMap [ rml:reference "Name" ]
+  ] .
```

### Comparing `morph_kgc-2.6.4/test/rml/json/RMLTC0007h/test_RMLTC0007h_JSON.py` & `morph_kgc-2.7.0/test/rml-core/json/RMLTC0007h/test_RMLTC0007h_JSON.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/rml/json/RMLTC0008a/mapping.ttl` & `morph_kgc-2.7.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0003c/mapping.ttl`

 * *Files 24% similar despite different names*

```diff
@@ -1,42 +1,38 @@
-@prefix rr: <http://www.w3.org/ns/r2rml#> .
 @prefix foaf: <http://xmlns.com/foaf/0.1/> .
 @prefix ex: <http://example.com/> .
 @prefix xsd: <http://www.w3.org/2001/XMLSchema#> .
-@prefix rml: <http://semweb.mmlab.be/ns/rml#> .
-@prefix ql: <http://semweb.mmlab.be/ns/ql#> .
-@prefix rdf: <http://www.w3.org/1999/02/22-rdf-syntax-ns#> .
+@prefix rml: <http://w3id.org/rml/> .
 @base <http://example.com/base/> .
+@prefix sd: <https://w3id.org/okn/o/sd#>.
+@prefix kg4di: <https://w3id.org/kg4di/definedBy>.
 
-<TriplesMap1>
-  a rr:TriplesMap;
+<TriplesMap1> a rml:TriplesMap;
 
   rml:logicalSource [
-    rml:source "test/rml/json/RMLTC0008a/student.json";
-    rml:referenceFormulation ql:JSONPath;
-    rml:iterator "$.students[*]"
+    rml:source [
+			a sd:DatasetSpecification;
+			sd:name "variable1";
+			sd:hasDataTransformation [
+				sd:hasSoftwareRequirements "pandas>=1.1.0";
+				sd:hasSourceCode [
+					sd:programmingLanguage "Python3.9";
+				];
+			];
+		];
+    rml:referenceFormulation rml:DataFrame;
   ];
 
-  rr:subjectMap [
-    rr:template "http://example.com/Student/{ID}/{Name}";
-    rr:graphMap [ rr:template "http://example.com/graph/Student/{ID}/{Name}" ]
+  rml:subjectMap [
+    rml:template "http://example.com/Student{ID}";
   ];
 
-  rr:predicateObjectMap [
-    rr:predicate rdf:type ;
-    rr:object foaf:Person;
-  ];
-
-  rr:predicateObjectMap [
-    rr:predicate ex:id ;
-    rr:objectMap [ rml:reference "ID" ]
-  ];
-
-  rr:predicateObjectMap [
-    rr:predicate foaf:name ;
-    rr:objectMap [ rml:reference "Name" ]
-  ];
+  rml:predicateObjectMap [
+    rml:predicate foaf:name ;
+    rml:objectMap [
+      rml:template "{FirstName} {LastName}";
+      rml:termType rml:Literal;
+    ]
+  ].
 
-  rr:predicateObjectMap [
-    rr:predicate ex:Sport ;
-    rr:objectMap [ rml:reference "Sport" ]
-  ] .
+rml:DataFrame a rml:ReferenceFormulation;
+	kg4di:definedBy "Pandas".
```

### Comparing `morph_kgc-2.6.4/test/rml/json/RMLTC0008a/output.nq` & `morph_kgc-2.7.0/test/rml-core/json/RMLTC0008a/output.nq`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/rml/json/RMLTC0008a/test_RMLTC0008a_JSON.py` & `morph_kgc-2.7.0/test/rml-core/json/RMLTC0008a/test_RMLTC0008a_JSON.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/rml/json/RMLTC0008b/mapping.ttl` & `morph_kgc-2.7.0/test/rml-core/json/RMLTC0008b/mapping.ttl`

 * *Files 12% similar despite different names*

```diff
@@ -1,60 +1,58 @@
-@prefix rr: <http://www.w3.org/ns/r2rml#> .
 @prefix foaf: <http://xmlns.com/foaf/0.1/> .
 @prefix ex: <http://example.com/> .
 @prefix xsd: <http://www.w3.org/2001/XMLSchema#> .
-@prefix rml: <http://semweb.mmlab.be/ns/rml#> .
-@prefix ql: <http://semweb.mmlab.be/ns/ql#> .
+@prefix rml: <http://w3id.org/rml/> .
 @prefix activity: <http://example.com/activity/> .
 @prefix rdf: <http://www.w3.org/1999/02/22-rdf-syntax-ns#> .
 @base <http://example.com/base/> .
 
 <TriplesMap2>
-  a rr:TriplesMap;
+  a rml:TriplesMap;
   rml:logicalSource [
-    rml:source "test/rml/json/RMLTC0008b/student.json";
-    rml:referenceFormulation ql:JSONPath;
+    rml:source "test/rml-core/json/RMLTC0008b/student.json";
+    rml:referenceFormulation rml:JSONPath;
     rml:iterator "$.students[*]"
   ];
 
-  rr:subjectMap [ rr:template "http://example.com/{Sport}" ];
+  rml:subjectMap [ rml:template "http://example.com/{Sport}" ];
 
-  rr:predicateObjectMap [
-    rr:predicate rdf:type ;
-    rr:object activity:Sport ;
+  rml:predicateObjectMap [
+    rml:predicate rdf:type ;
+    rml:object activity:Sport ;
   ] .
 
 <TriplesMap1>
-  a rr:TriplesMap;
+  a rml:TriplesMap;
 
   rml:logicalSource [
-    rml:source "test/rml/json/RMLTC0008b/student.json";
-    rml:referenceFormulation ql:JSONPath;
+    rml:source "test/rml-core/json/RMLTC0008b/student.json";
+    rml:referenceFormulation rml:JSONPath;
     rml:iterator "$.students[*]"
   ];
 
-  rr:subjectMap [ rr:template "http://example.com/Student/{ID}/{Name}" ];
+  rml:subjectMap [ rml:template "http://example.com/Student/{ID}/{Name}" ];
 
-  rr:predicateObjectMap [
-    rr:predicate rdf:type ;
-    rr:object foaf:Person ;
+  rml:predicateObjectMap [
+    rml:predicate rdf:type ;
+    rml:object foaf:Person ;
   ];
 
-  rr:predicateObjectMap [
-    rr:predicate ex:id ;
-    rr:objectMap [ rml:reference "ID"; ]
+  rml:predicateObjectMap [
+    rml:predicate ex:id ;
+    rml:objectMap [ rml:reference "ID"; ]
   ];
 
-  rr:predicateObjectMap [
-    rr:predicate foaf:name ;
-    rr:objectMap [ rml:reference "Name" ]
+  rml:predicateObjectMap [
+    rml:predicate foaf:name ;
+    rml:objectMap [ rml:reference "Name" ]
   ];
 
-  rr:predicateObjectMap [
-    rr:predicate ex:Sport ;
-    rr:objectMap <RefObjectMap1>
+  rml:predicateObjectMap [
+    rml:predicate ex:Sport ;
+    rml:objectMap <RefObjectMap1>
   ] .
 
 
 <RefObjectMap1>
-  a rr:RefObjectMap;
-  rr:parentTriplesMap <TriplesMap2> .
+  a rml:RefObjectMap;
+  rml:parentTriplesMap <TriplesMap2> .
```

### Comparing `morph_kgc-2.6.4/test/rml/json/RMLTC0008b/output.nq` & `morph_kgc-2.7.0/test/rml-core/json/RMLTC0008b/output.nq`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/rml/json/RMLTC0008b/test_RMLTC0008b_JSON.py` & `morph_kgc-2.7.0/test/rml-core/json/RMLTC0008b/test_RMLTC0008b_JSON.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/rml/json/RMLTC0008c/mapping.ttl` & `morph_kgc-2.7.0/test/rml-core/xml/RMLTC0007g/mapping.ttl`

 * *Files 14% similar despite different names*

```diff
@@ -1,25 +1,25 @@
-@prefix rr: <http://www.w3.org/ns/r2rml#> .
 @prefix foaf: <http://xmlns.com/foaf/0.1/> .
 @prefix ex: <http://example.com/> .
 @prefix xsd: <http://www.w3.org/2001/XMLSchema#> .
-@prefix rml: <http://semweb.mmlab.be/ns/rml#> .
-@prefix ql: <http://semweb.mmlab.be/ns/ql#> .
-@prefix activity: <http://example.com/activity/> .
+@prefix rml: <http://w3id.org/rml/> .
 @base <http://example.com/base/> .
 
-<TriplesMap1>
-  a rr:TriplesMap;
+<TriplesMap1> a rml:TriplesMap;
 
   rml:logicalSource [
-    rml:source "test/rml/json/RMLTC0008c/student.json";
-    rml:referenceFormulation ql:JSONPath;
-    rml:iterator "$.students[*]"
+    rml:source "test/rml-core/xml/RMLTC0007g/student.xml";
+    rml:referenceFormulation rml:XPath;
+    rml:iterator "/students/student"
   ];
 
-  rr:subjectMap [ rr:template "http://example.com/Student/{ID}/{Name}" ];
+  rml:subjectMap [
+    rml:template "http://example.com/Student/{ID}/{FirstName}";
+    rml:graph rml:defaultGraph
+  ];
 
-  rr:predicateObjectMap [
-    rr:predicate foaf:name ;
-    rr:predicate ex:name ;
-    rr:objectMap [ rml:reference "Name" ]
-  ] .
+  rml:predicateObjectMap [
+    rml:predicate foaf:name;
+    rml:objectMap [
+      rml:reference "FirstName"
+    ]
+  ].
```

### Comparing `morph_kgc-2.6.4/test/rml/json/RMLTC0008c/test_RMLTC0008c_JSON.py` & `morph_kgc-2.7.0/test/rml-core/json/RMLTC0008c/test_RMLTC0008c_JSON.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/rml/json/RMLTC0009a/mapping.ttl` & `morph_kgc-2.7.0/test/rml-core/json/RMLTC0012b/mapping.ttl`

 * *Files 20% similar despite different names*

```diff
@@ -1,53 +1,52 @@
-@prefix rr: <http://www.w3.org/ns/r2rml#> .
 @prefix foaf: <http://xmlns.com/foaf/0.1/> .
 @prefix ex: <http://example.com/> .
 @prefix xsd: <http://www.w3.org/2001/XMLSchema#> .
-@prefix rml: <http://semweb.mmlab.be/ns/rml#> .
-@prefix ql: <http://semweb.mmlab.be/ns/ql#> .
-@prefix activity: <http://example.com/activity/> .
-@prefix rdfs: <http://www.w3.org/2000/01/rdf-schema#> .
+@prefix rml: <http://w3id.org/rml/> .
+
 @base <http://example.com/base/> .
 
 <TriplesMap1>
-  a rr:TriplesMap;
+  a rml:TriplesMap;
 
   rml:logicalSource [
-    rml:source "test/rml/json/RMLTC0009a/student.json";
-    rml:referenceFormulation ql:JSONPath;
-    rml:iterator "$.students[*]"
+    rml:source "test/rml-core/json/RMLTC0012b/persons.json";
+    rml:referenceFormulation rml:JSONPath;
+    rml:iterator "$.persons[*]"
   ];
 
-  rr:subjectMap [ rr:template "http://example.com/resource/student_{ID}" ];
+  rml:subjectMap [
+    rml:template "{fname}{lname}";
+    rml:termType rml:BlankNode ;
+  ];
 
-  rr:predicateObjectMap [
-    rr:predicate foaf:name ;
-    rr:objectMap [ rml:reference "Name" ]
-  ] ;
-
-  rr:predicateObjectMap [
-    rr:predicate <http://example.com/ontology/practises> ;
-    rr:objectMap [
-      a rr:RefObjectMap ;
-      rr:parentTriplesMap <TriplesMap2>;
-      rr:joinCondition [
-        rr:child "Sport" ;
-        rr:parent "ID" ;
-      ]
+  rml:predicateObjectMap [
+    rml:predicate foaf:name ;
+    rml:objectMap [
+      rml:template "{fname} {lname}";
+      rml:termType rml:Literal ;
     ]
-  ] .
+  ];
+  .
 
 <TriplesMap2>
-  a rr:TriplesMap;
+  a rml:TriplesMap;
 
   rml:logicalSource [
-    rml:source "test/rml/json/RMLTC0009a/sport.json";
-    rml:referenceFormulation ql:JSONPath;
-    rml:iterator "$.sports[*]"
+    rml:source "test/rml-core/json/RMLTC0012b/lives.json";
+    rml:referenceFormulation rml:JSONPath;
+    rml:iterator "$.lives[*]"
+];
+
+  rml:subjectMap [
+    rml:template "{fname}{lname}";
+    rml:termType rml:BlankNode;
   ];
 
-  rr:subjectMap [ rr:template "http://example.com/resource/sport_{ID}" ];
-
-  rr:predicateObjectMap [
-    rr:predicate rdfs:label ;
-    rr:objectMap [ rml:reference "Name" ];
-  ].
+  rml:predicateObjectMap
+  [
+    rml:predicate	ex:city ;
+    rml:objectMap    [
+      rml:reference "city";
+    ]
+];
+.
```

### Comparing `morph_kgc-2.6.4/test/rml/json/RMLTC0009a/test_RMLTC0009a_JSON.py` & `morph_kgc-2.7.0/test/rml-core/json/RMLTC0009a/test_RMLTC0009a_JSON.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/rml/json/RMLTC0009b/mapping.ttl` & `morph_kgc-2.7.0/test/rml-in-memory/json_dictionary/RMLIMTC0009b/mapping.ttl`

 * *Files 18% similar despite different names*

```diff
@@ -1,61 +1,80 @@
-@prefix rr: <http://www.w3.org/ns/r2rml#> .
 @prefix foaf: <http://xmlns.com/foaf/0.1/> .
 @prefix ex: <http://example.com/> .
 @prefix xsd: <http://www.w3.org/2001/XMLSchema#> .
-@prefix rml: <http://semweb.mmlab.be/ns/rml#> .
-@prefix ql: <http://semweb.mmlab.be/ns/ql#> .
+@prefix rml: <http://w3id.org/rml/> .
 @prefix activity: <http://example.com/activity/> .
 @prefix rdfs: <http://www.w3.org/2000/01/rdf-schema#> .
 @base <http://example.com/base/> .
+@prefix sd: <https://w3id.org/okn/o/sd#>.
+@prefix kg4di: <https://w3id.org/kg4di/definedBy>.
 
 <TriplesMap1>
-  a rr:TriplesMap;
+  a rml:TriplesMap;
 
   rml:logicalSource [
-    rml:source "test/rml/json/RMLTC0009b/student.json";
-    rml:referenceFormulation ql:JSONPath;
+    rml:source [
+			a sd:DatasetSpecification;
+			sd:name "variable2";
+			sd:hasDataTransformation [
+				sd:hasSourceCode [
+					sd:programmingLanguage "Python3.9";
+				];
+			];
+		];
+		rml:referenceFormulation rml:Dictionary;
     rml:iterator "$.students[*]"
   ];
 
-  rr:subjectMap [ rr:template "http://example.com/resource/student_{ID}";
-    rr:class <http://example.com/ontology/Student>;
-    rr:graph <http://example.com/graph/students> ;
+  rml:subjectMap [ rml:template "http://example.com/resource/student_{ID}";
+    rml:class <http://example.com/ontology/Student>;
+    rml:graph <http://example.com/graph/students> ;
  ];
 
-  rr:predicateObjectMap [
-    rr:predicate foaf:name ;
-    rr:objectMap [ rml:reference "Name" ];
-    rr:graph <http://example.com/graph/students> ;
+  rml:predicateObjectMap [
+    rml:predicate foaf:name ;
+    rml:objectMap [ rml:reference "Name" ];
+    rml:graph <http://example.com/graph/students> ;
   ] ;
 
-  rr:predicateObjectMap [
-    rr:predicate <http://example.com/ontology/practises> ;
-    rr:objectMap [
-      a rr:RefObjectMap ;
-      rr:parentTriplesMap <TriplesMap2>;
-      rr:joinCondition [
-        rr:child "Sport" ;
-        rr:parent "ID" ;
+  rml:predicateObjectMap [
+    rml:predicate <http://example.com/ontology/practises> ;
+    rml:objectMap [
+      a rml:RefObjectMap ;
+      rml:parentTriplesMap <TriplesMap2>;
+      rml:joinCondition [
+        rml:child "Sport" ;
+        rml:parent "ID" ;
       ]
     ];
-    rr:graph <http://example.com/graph/practise> ;
+    rml:graph <http://example.com/graph/practise> ;
   ] .
 
 <TriplesMap2>
-  a rr:TriplesMap;
+  a rml:TriplesMap;
 
   rml:logicalSource [
-    rml:source "test/rml/json/RMLTC0009b/sport.json";
-    rml:referenceFormulation ql:JSONPath;
+    rml:source [
+			a sd:DatasetSpecification;
+			sd:name "variable1";
+			sd:hasDataTransformation [
+				sd:hasSourceCode [
+					sd:programmingLanguage "Python3.9";
+				];
+			];
+		];
+		rml:referenceFormulation rml:Dictionary;
     rml:iterator "$.sports[*]"
   ];
 
-  rr:subjectMap [ rr:template "http://example.com/resource/sport_{ID}";
-    rr:class <http://example.com/ontology/Sport>;
-    rr:graph <http://example.com/graph/sports> ;
+  rml:subjectMap [ rml:template "http://example.com/resource/sport_{ID}";
+    rml:class <http://example.com/ontology/Sport>;
+    rml:graph <http://example.com/graph/sports> ;
   ];
 
-  rr:predicateObjectMap [
-    rr:predicate rdfs:label ;
-    rr:objectMap [ rml:reference "Name" ];
+  rml:predicateObjectMap [
+    rml:predicate rdfs:label ;
+    rml:objectMap [ rml:reference "Name" ];
   ].
+
+rml:Dictionary a rml:ReferenceFormulation;
+	kg4di:definedBy "Python".
```

### Comparing `morph_kgc-2.6.4/test/rml/json/RMLTC0009b/output.nq` & `morph_kgc-2.7.0/test/rml-core/json/RMLTC0009b/output.nq`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/rml/json/RMLTC0009b/test_RMLTC0009b_JSON.py` & `morph_kgc-2.7.0/test/rml-core/json/RMLTC0009b/test_RMLTC0009b_JSON.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/rml/json/RMLTC0010a/mapping.ttl` & `morph_kgc-2.7.0/test/rml-core/json/RMLTC0007h/mapping.ttl`

 * *Files 18% similar despite different names*

```diff
@@ -1,24 +1,25 @@
-@prefix rr: <http://www.w3.org/ns/r2rml#> .
 @prefix foaf: <http://xmlns.com/foaf/0.1/> .
 @prefix ex: <http://example.com/> .
 @prefix xsd: <http://www.w3.org/2001/XMLSchema#> .
-@prefix rml: <http://semweb.mmlab.be/ns/rml#> .
-@prefix ql: <http://semweb.mmlab.be/ns/ql#> .
-@prefix activity: <http://example.com/activity/> .
+@prefix rml: <http://w3id.org/rml/> .
 @base <http://example.com/base/> .
 
-<TriplesMap1>
-  a rr:TriplesMap;
+<TriplesMap1> a rml:TriplesMap;
 
   rml:logicalSource [
-    rml:source "test/rml/json/RMLTC0010a/country_info.json";
-    rml:referenceFormulation ql:JSONPath;
-    rml:iterator "$.countries[*]"
+    rml:source "test/rml-core/json/RMLTC0007h/student.json";
+    rml:referenceFormulation rml:JSONPath;
+    rml:iterator "$.students[*]"
   ];
 
-  rr:subjectMap [ rr:template "http://example.com/{Country Code}" ];
+  rml:subjectMap [
+    rml:template "http://example.com/Student/{ID}/{FirstName}";
+    rml:graphMap [ rml:reference "FirstName"; rml:termType rml:Literal; ]
+  ];
 
-  rr:predicateObjectMap [
-    rr:predicate ex:name ;
-    rr:objectMap [ rml:reference "Name" ]
-  ] .
+  rml:predicateObjectMap [
+    rml:predicate foaf:name;
+    rml:objectMap [
+      rml:reference "FirstName"
+    ]
+  ].
```

### Comparing `morph_kgc-2.6.4/test/rml/json/RMLTC0010a/test_RMLTC0010a_JSON.py` & `morph_kgc-2.7.0/test/rml-core/json/RMLTC0010a/test_RMLTC0010a_JSON.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/rml/json/RMLTC0010b/mapping.ttl` & `morph_kgc-2.7.0/test/rml-core/json/RMLTC0001a/mapping.ttl`

 * *Files 20% similar despite different names*

```diff
@@ -1,24 +1,26 @@
-@prefix rr: <http://www.w3.org/ns/r2rml#> .
 @prefix foaf: <http://xmlns.com/foaf/0.1/> .
 @prefix ex: <http://example.com/> .
 @prefix xsd: <http://www.w3.org/2001/XMLSchema#> .
-@prefix rml: <http://semweb.mmlab.be/ns/rml#> .
-@prefix ql: <http://semweb.mmlab.be/ns/ql#> .
-@prefix activity: <http://example.com/activity/> .
+@prefix rml: <http://w3id.org/rml/> .
+
 @base <http://example.com/base/> .
 
 <TriplesMap1>
-  a rr:TriplesMap;
+  a rml:TriplesMap;
 
   rml:logicalSource [
-    rml:source "test/rml/json/RMLTC0010b/country_info.json";
-    rml:referenceFormulation ql:JSONPath;
-    rml:iterator "$.countries[*]"
+    rml:source "test/rml-core/json/RMLTC0001a/student.json";
+    rml:referenceFormulation rml:JSONPath;
+    rml:iterator "$.students[*]"
   ];
 
-  rr:subjectMap [ rr:template "http://example.com/{Country Code}/{Name}" ];
+  rml:subjectMap <#NameSubjectMap> ;
+
+  rml:predicateObjectMap [
+    rml:predicate foaf:name;
+    rml:objectMap [
+      rml:reference "Name"
+    ]
+  ].
 
-  rr:predicateObjectMap [
-    rr:predicate ex:name ;
-    rr:objectMap [ rml:reference "Name" ]
-  ] .
+<#NameSubjectMap> rml:template "http://example.com/{Name}" .
```

### Comparing `morph_kgc-2.6.4/test/rml/json/RMLTC0010b/test_RMLTC0010b_JSON.py` & `morph_kgc-2.7.0/test/rml-core/json/RMLTC0010b/test_RMLTC0010b_JSON.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/rml/json/RMLTC0010c/mapping.ttl` & `morph_kgc-2.7.0/test/rml-core/json/RMLTC0007c/mapping.ttl`

 * *Files 22% similar despite different names*

```diff
@@ -1,24 +1,28 @@
-@prefix rr: <http://www.w3.org/ns/r2rml#> .
 @prefix foaf: <http://xmlns.com/foaf/0.1/> .
 @prefix ex: <http://example.com/> .
 @prefix xsd: <http://www.w3.org/2001/XMLSchema#> .
-@prefix rml: <http://semweb.mmlab.be/ns/rml#> .
-@prefix ql: <http://semweb.mmlab.be/ns/ql#> .
-@prefix activity: <http://example.com/activity/> .
+@prefix rml: <http://w3id.org/rml/> .
 @base <http://example.com/base/> .
 
-<TriplesMap1>
-  a rr:TriplesMap;
+<TriplesMap1> a rml:TriplesMap;
 
   rml:logicalSource [
-    rml:source "test/rml/json/RMLTC0010c/country_info.json";
-    rml:referenceFormulation ql:JSONPath;
-    rml:iterator "$.countries[*]"
+    rml:source "test/rml-core/json/RMLTC0007c/student.json";
+    rml:referenceFormulation rml:JSONPath;
+    rml:iterator "$.students[*]"
   ];
 
-  rr:subjectMap [ rr:template "http://example.com/{Country Code}/{Name}" ];
+  rml:subjectMap [
+    rml:template "http://example.com/Student/{ID}/{FirstName}";
+    rml:class foaf:Person, ex:Student
+  ];
+
+  rml:predicateObjectMap [
+    rml:predicate ex:id ;
+    rml:objectMap [ rml:reference "ID";  ]
+  ];
 
-  rr:predicateObjectMap [
-    rr:predicate ex:code ;
-    rr:objectMap [ rr:template "\\{\\{\\{ {ISO 3166} \\}\\}\\}"; rr:termType rr:Literal]
-  ] .
+  rml:predicateObjectMap [
+    rml:predicate foaf:name;
+    rml:objectMap [ rml:reference "FirstName" ]
+  ].
```

### Comparing `morph_kgc-2.6.4/test/rml/json/RMLTC0010c/test_RMLTC0010c_JSON.py` & `morph_kgc-2.7.0/test/rml-core/json/RMLTC0010c/test_RMLTC0010c_JSON.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/rml/json/RMLTC0011b/mapping.ttl` & `morph_kgc-2.7.0/test/rml-core/csv/RMLTC0011b/mapping.ttl`

 * *Files 24% similar despite different names*

```diff
@@ -1,82 +1,77 @@
-@prefix rr: <http://www.w3.org/ns/r2rml#> .
 @prefix foaf: <http://xmlns.com/foaf/0.1/> .
 @prefix ex: <http://example.com/> .
 @prefix xsd: <http://www.w3.org/2001/XMLSchema#> .
-@prefix rml: <http://semweb.mmlab.be/ns/rml#> .
-@prefix ql: <http://semweb.mmlab.be/ns/ql#> .
+@prefix rml: <http://w3id.org/rml/> .
 
 @base <http://example.com/base/> .
 
 <TriplesMap1>
-  a rr:TriplesMap;
+  a rml:TriplesMap;
 
   rml:logicalSource [
-    rml:source "test/rml/json/RMLTC0011b/student.json";
-    rml:referenceFormulation ql:JSONPath;
-    rml:iterator "$.students[*]"
+    rml:source "test/rml-core/csv/RMLTC0011b/student.csv";
+    rml:referenceFormulation rml:CSV
   ];
 
-  rr:subjectMap [
-    rr:template "http://example.com/student/{ID}";
+  rml:subjectMap [
+    rml:template "http://example.com/student/{ID}";
   ];
 
-  rr:predicateObjectMap [
-    rr:predicate ex:firstName;
-    rr:objectMap [
+  rml:predicateObjectMap [
+    rml:predicate ex:firstName;
+    rml:objectMap [
       rml:reference "FirstName"
     ]
   ];
 
-  rr:predicateObjectMap [
-    rr:predicate ex:lastName;
-    rr:objectMap [
+  rml:predicateObjectMap [
+    rml:predicate ex:lastName;
+    rml:objectMap [
       rml:reference "LastName"
     ]
   ].
 
 <TriplesMap2>
-  a rr:TriplesMap;
+  a rml:TriplesMap;
 
   rml:logicalSource [
-    rml:source "test/rml/json/RMLTC0011b/sport.json";
-    rml:referenceFormulation ql:JSONPath;
-    rml:iterator "$.sports[*]"
+    rml:source "test/rml-core/csv/RMLTC0011b/sport.csv";
+    rml:referenceFormulation rml:CSV
   ];
 
-  rr:subjectMap [
-    rr:template "http://example.com/sport/{ID}";
+  rml:subjectMap [
+    rml:template "http://example.com/sport/{ID}";
   ];
 
-  rr:predicateObjectMap [
-    rr:predicate ex:id;
-    rr:objectMap [
+  rml:predicateObjectMap [
+    rml:predicate ex:id;
+    rml:objectMap [
       rml:reference "ID"
     ]
   ];
 
-  rr:predicateObjectMap [
-    rr:predicate ex:description;
-    rr:objectMap [
+  rml:predicateObjectMap [
+    rml:predicate ex:description;
+    rml:objectMap [
       rml:reference "Description"
     ]
   ].
 
 <LinkMap_1_2>
-  a rr:TriplesMap;
+  a rml:TriplesMap;
 
   rml:logicalSource [
-    rml:source "test/rml/json/RMLTC0011b/student_sport.json";
-    rml:referenceFormulation ql:JSONPath;
-    rml:iterator "$.links[*]"
+    rml:source "test/rml-core/csv/RMLTC0011b/student_sport.csv";
+    rml:referenceFormulation rml:CSV
   ];
 
-  rr:subjectMap [
-    rr:template "http://example.com/student/{ID_Student}";
+  rml:subjectMap [
+    rml:template "http://example.com/student/{ID_Student}";
   ];
 
-  rr:predicateObjectMap [
-    rr:predicate ex:plays;
-    rr:objectMap [
-      rr:template "http://example.com/sport/{ID_Sport}"
+  rml:predicateObjectMap [
+    rml:predicate ex:plays;
+    rml:objectMap [
+      rml:template "http://example.com/sport/{ID_Sport}"
     ]
   ].
```

### Comparing `morph_kgc-2.6.4/test/rml/json/RMLTC0011b/output.nq` & `morph_kgc-2.7.0/test/rml-core/json/RMLTC0011b/output.nq`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/rml/json/RMLTC0011b/test_RMLTC0011b_JSON.py` & `morph_kgc-2.7.0/test/rml-core/json/RMLTC0011b/test_RMLTC0011b_JSON.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/rml/json/RMLTC0012a/test_RMLTC0012a_JSON.py` & `morph_kgc-2.7.0/test/rml-core/json/RMLTC0012a/test_RMLTC0012a_JSON.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/rml/json/RMLTC0012b/mapping.ttl` & `morph_kgc-2.7.0/test/rml-fnml/split_explode_null/mapping.ttl`

 * *Files 22% similar despite different names*

```diff
@@ -1,54 +1,39 @@
-@prefix rr: <http://www.w3.org/ns/r2rml#> .
 @prefix foaf: <http://xmlns.com/foaf/0.1/> .
 @prefix ex: <http://example.com/> .
 @prefix xsd: <http://www.w3.org/2001/XMLSchema#> .
-@prefix rml: <http://semweb.mmlab.be/ns/rml#> .
-@prefix ql: <http://semweb.mmlab.be/ns/ql#> .
+@prefix rml: <http://w3id.org/rml/> .
+@prefix fno: <https://w3id.org/function/ontology#> .
+@prefix morph-kgc: <https://github.com/morph-kgc/morph-kgc/function/built-in.ttl#> .
+@prefix grel: <http://users.ugent.be/~bjdmeest/function/grel.ttl#> .
+@prefix idlab-fn: <http://example.com/idlab/function/> .
 
 @base <http://example.com/base/> .
 
 <TriplesMap1>
-  a rr:TriplesMap;
-
-  rml:logicalSource [
-    rml:source "test/rml/json/RMLTC0012b/persons.json";
-    rml:referenceFormulation ql:JSONPath;
-    rml:iterator "$.persons[*]"
-  ];
-
-  rr:subjectMap [
-    rr:template "{fname}{lname}";
-    rr:termType rr:BlankNode ;
-  ];
-
-  rr:predicateObjectMap [
-    rr:predicate foaf:name ;
-    rr:objectMap [
-      rr:template "{fname} {lname}";
-      rr:termType rr:Literal ;
-    ]
-  ];
-  .
-
-<TriplesMap2>
-  a rr:TriplesMap;
-
-  rml:logicalSource [
-    rml:source "test/rml/json/RMLTC0012b/lives.json";
-    rml:referenceFormulation ql:JSONPath;
-    rml:iterator "$.lives[*]"
-];
-
-  rr:subjectMap [
-    rr:template "{fname}{lname}";
-    rr:termType rr:BlankNode;
-  ];
-
-  rr:predicateObjectMap
-  [
-    rr:predicate	ex:city ;
-    rr:objectMap    [
-      rml:reference "city";
-    ]
-];
-.
+    rml:logicalSource [
+        rml:source "test/rml-fnml/split_explode_null/mixed_content_list.csv";
+        rml:referenceFormulation rml:CSV
+    ];
+    rml:subjectMap [
+        rml:template "http://example.com/{ID}"
+    ];
+    rml:predicateObjectMap [
+        rml:predicate ex:col;
+        rml:objectMap [
+            rml:functionExecution <#Execution> ;
+        ]
+    ] .
+
+<#Execution>
+    rml:function morph-kgc:string_split_explode ;
+    rml:input
+        [
+            rml:parameter grel:valueParam ;
+            rml:inputValueMap [
+                rml:reference "COL"
+            ]
+        ] ,
+        [
+            rml:parameter grel:param_string_sep ;
+            rml:inputValue ";"
+        ] .
```

### Comparing `morph_kgc-2.6.4/test/rml/json/RMLTC0012b/test_RMLTC0012b_JSON.py` & `morph_kgc-2.7.0/test/rml-core/json/RMLTC0012b/test_RMLTC0012b_JSON.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/rml/json/RMLTC0012c/mapping.ttl` & `morph_kgc-2.7.0/test/rml-core/csv/RMLTC0003c/mapping.ttl`

 * *Files 21% similar despite different names*

```diff
@@ -1,32 +1,24 @@
-@prefix rr: <http://www.w3.org/ns/r2rml#> .
 @prefix foaf: <http://xmlns.com/foaf/0.1/> .
 @prefix ex: <http://example.com/> .
 @prefix xsd: <http://www.w3.org/2001/XMLSchema#> .
-@prefix rml: <http://semweb.mmlab.be/ns/rml#> .
-@prefix ql: <http://semweb.mmlab.be/ns/ql#> .
-
+@prefix rml: <http://w3id.org/rml/> .
 @base <http://example.com/base/> .
 
-<TriplesMap1>
-  a rr:TriplesMap;
+<TriplesMap1> a rml:TriplesMap;
 
   rml:logicalSource [
-    rml:source "test/rml/json/RMLTC0012c/persons.json";
-    rml:referenceFormulation ql:JSONPath;
-    rml:iterator "$.persons[*]"
+    rml:source "test/rml-core/csv/RMLTC0003c/student.csv";
+    rml:referenceFormulation rml:CSV
   ];
 
-  rr:predicateObjectMap [
-    rr:predicate foaf:name ;
-    rr:objectMap [
-      rr:template "{fname} {lname}";
-      rr:termType rr:Literal ;
-    ]
+  rml:subjectMap [
+    rml:template "http://example.com/Student{ID}";
   ];
 
-  rr:predicateObjectMap [
-    rr:predicate ex:amount ;
-    rr:objectMap    [
-      rml:reference "amount";
+  rml:predicateObjectMap [
+    rml:predicate foaf:name ;
+    rml:objectMap [
+      rml:template "{FirstName} {LastName}";
+      rml:termType rml:Literal;
     ]
   ].
```

### Comparing `morph_kgc-2.6.4/test/rml/json/RMLTC0012c/test_RMLTC0012c_JSON.py` & `morph_kgc-2.7.0/test/rml-core/json/RMLTC0012c/test_RMLTC0012c_JSON.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/rml/json/RMLTC0012d/mapping.ttl` & `morph_kgc-2.7.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0012a/mapping.ttl`

 * *Files 22% similar despite different names*

```diff
@@ -1,36 +1,44 @@
-@prefix rr: <http://www.w3.org/ns/r2rml#> .
 @prefix foaf: <http://xmlns.com/foaf/0.1/> .
 @prefix ex: <http://example.com/> .
 @prefix xsd: <http://www.w3.org/2001/XMLSchema#> .
-@prefix rml: <http://semweb.mmlab.be/ns/rml#> .
-@prefix ql: <http://semweb.mmlab.be/ns/ql#> .
-
+@prefix rml: <http://w3id.org/rml/> .
+@prefix sd: <https://w3id.org/okn/o/sd#>.
+@prefix kg4di: <https://w3id.org/kg4di/definedBy>.
 @base <http://example.com/base/> .
 
 <TriplesMap1>
-  a rr:TriplesMap;
+  a rml:TriplesMap;
 
   rml:logicalSource [
-    rml:source "test/rml/json/RMLTC0012d/persons.json";
-    rml:referenceFormulation ql:JSONPath;
-    rml:iterator "$.persons[*]"
+    rml:source [
+			a sd:DatasetSpecification;
+			sd:name "variable1";
+			sd:hasDataTransformation [
+				sd:hasSoftwareRequirements "pandas>=1.1.0";
+				sd:hasSourceCode [
+					sd:programmingLanguage "Python3.9";
+				];
+			];
+		];
+    rml:referenceFormulation rml:DataFrame;
   ];
 
-  rr:subjectMap [ rr:template "{fname}_{lname}_{amount}"; rr:termType rr:BlankNode; ];
-
-  rr:subjectMap [ rr:template "{amount}_{fname}_{lname}"; rr:termType rr:BlankNode; ];
+  rml:subjectMap [ rml:template "{fname}{lname}{amount}"; rml:termType rml:BlankNode; ];
 
-  rr:predicateObjectMap [
-    rr:predicate foaf:name ;
-    rr:objectMap [
-      rr:template "{fname} {lname}";
-      rr:termType rr:Literal ;
+  rml:predicateObjectMap [
+    rml:predicate foaf:name ;
+    rml:objectMap [
+      rml:template "{fname} {lname}";
+      rml:termType rml:Literal ;
     ]
   ];
 
-  rr:predicateObjectMap [
-    rr:predicate ex:amount ;
-    rr:objectMap    [
+  rml:predicateObjectMap [
+    rml:predicate ex:amount ;
+    rml:objectMap    [
       rml:reference "amount";
     ]
   ].
+
+rml:DataFrame a rml:ReferenceFormulation;
+	kg4di:definedBy "Pandas".
```

### Comparing `morph_kgc-2.6.4/test/rml/json/RMLTC0012d/test_RMLTC0012d_JSON.py` & `morph_kgc-2.7.0/test/rml-core/json/RMLTC0012d/test_RMLTC0012d_JSON.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/rml/json/RMLTC0013a/mapping.ttl` & `morph_kgc-2.7.0/test/rml-core/csv/RMLTC0007a/mapping.ttl`

 * *Files 16% similar despite different names*

```diff
@@ -1,25 +1,22 @@
-@prefix rr: <http://www.w3.org/ns/r2rml#> .
 @prefix foaf: <http://xmlns.com/foaf/0.1/> .
 @prefix ex: <http://example.com/> .
 @prefix xsd: <http://www.w3.org/2001/XMLSchema#> .
-@prefix rml: <http://semweb.mmlab.be/ns/rml#> .
-@prefix ql: <http://semweb.mmlab.be/ns/ql#> .
-
+@prefix rml: <http://w3id.org/rml/> .
+@prefix rdf: <http://www.w3.org/1999/02/22-rdf-syntax-ns#> .
 @base <http://example.com/base/> .
 
-<TriplesMap1>
-  a rr:TriplesMap;
+<TriplesMap1> a rml:TriplesMap;
 
   rml:logicalSource [
-    rml:source "test/rml/json/RMLTC0013a/persons.json";
-    rml:referenceFormulation ql:JSONPath;
-    rml:iterator "$.persons[*]"
+    rml:source "test/rml-core/csv/RMLTC0007a/student.csv";
+    rml:referenceFormulation rml:CSV
   ];
 
-  rr:subjectMap [ rr:template "http://example.com/Person/{ID}/{Name}/{DateOfBirth}"];
+  rml:subjectMap [
+    rml:template "http://example.com/Student/{ID}/{FirstName}"
+  ];
 
-  rr:predicateObjectMap
-    [
-      rr:predicate		ex:BirthDay ;
-      rr:objectMap		[ rml:reference "DateOfBirth" ]
-    ].
+  rml:predicateObjectMap [
+    rml:predicate rdf:type;
+    rml:object foaf:Person;
+  ].
```

### Comparing `morph_kgc-2.6.4/test/rml/json/RMLTC0013a/test_RMLTC0013a_JSON.py` & `morph_kgc-2.7.0/test/rml-core/json/RMLTC0013a/test_RMLTC0013a_JSON.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/rml/json/RMLTC0015a/test_RMLTC0015a_JSON.py` & `morph_kgc-2.7.0/test/rml-core/json/RMLTC0015a/test_RMLTC0015a_JSON.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/rml/json/RMLTC0015b/test_RMLTC0015b_JSON.py` & `morph_kgc-2.7.0/test/rml-core/json/RMLTC0015b/test_RMLTC0015b_JSON.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/rml/json/RMLTC0019a/RMLTC0019a_JSON.py` & `morph_kgc-2.7.0/test/rml-core/json/RMLTC0019a/RMLTC0019a_JSON.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/rml/json/RMLTC0019a/mapping.ttl` & `morph_kgc-2.7.0/test/rml-core/xml/RMLTC0019b/mapping.ttl`

 * *Files 23% similar despite different names*

```diff
@@ -1,27 +1,25 @@
-@prefix rr: <http://www.w3.org/ns/r2rml#> .
 @prefix foaf: <http://xmlns.com/foaf/0.1/> .
 @prefix rdfs: <http://www.w3.org/2000/01/rdf-schema#> .
 @prefix ex: <http://example.com/> .
 @prefix xsd: <http://www.w3.org/2001/XMLSchema#> .
-@prefix rml: <http://semweb.mmlab.be/ns/rml#> .
-@prefix ql: <http://semweb.mmlab.be/ns/ql#> .
+@prefix rml: <http://w3id.org/rml/> .
 
 @base <http://example.com/base/> .
 
 <TriplesMap1>
-  a rr:TriplesMap;
+  a rml:TriplesMap;
 
   rml:logicalSource [
-    rml:source "test/rml/json/RMLTC0019a/persons.json";
-    rml:referenceFormulation ql:JSONPath;
-    rml:iterator "$.persons[*]"
+    rml:source "test/rml-core/xml/RMLTC0019b/persons.xml";
+    rml:referenceFormulation rml:XPath;
+    rml:iterator "/persons/person"
   ];
 
-  rr:subjectMap [ rml:reference "FirstName" ];
+  rml:subjectMap [ rml:reference "FirstName" ];
 
-  rr:predicateObjectMap [
-    rr:predicate foaf:name;
-    rr:objectMap [
+  rml:predicateObjectMap [
+    rml:predicate foaf:name;
+    rml:objectMap [
       rml:reference "FirstName"
     ]
   ] .
```

### Comparing `morph_kgc-2.6.4/test/rml/json/RMLTC0019b/RMLTC0019b_JSON.py` & `morph_kgc-2.7.0/test/rml-core/json/RMLTC0019b/RMLTC0019b_JSON.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/rml/json/RMLTC0019b/mapping.ttl` & `morph_kgc-2.7.0/test/rml-core/csv/RMLTC0019a/mapping.ttl`

 * *Files 19% similar despite different names*

```diff
@@ -1,27 +1,24 @@
-@prefix rr: <http://www.w3.org/ns/r2rml#> .
 @prefix foaf: <http://xmlns.com/foaf/0.1/> .
 @prefix rdfs: <http://www.w3.org/2000/01/rdf-schema#> .
 @prefix ex: <http://example.com/> .
 @prefix xsd: <http://www.w3.org/2001/XMLSchema#> .
-@prefix rml: <http://semweb.mmlab.be/ns/rml#> .
-@prefix ql: <http://semweb.mmlab.be/ns/ql#> .
+@prefix rml: <http://w3id.org/rml/> .
 
 @base <http://example.com/base/> .
 
 <TriplesMap1>
-  a rr:TriplesMap;
+  a rml:TriplesMap;
 
   rml:logicalSource [
-    rml:source "test/rml/json/RMLTC0019b/persons.json";
-    rml:referenceFormulation ql:JSONPath;
-    rml:iterator "$.persons[*]"
+    rml:source "test/rml-core/csv/RMLTC0019a/persons.csv";
+    rml:referenceFormulation rml:CSV
   ];
 
-  rr:subjectMap [ rml:reference "FirstName" ];
+  rml:subjectMap [ rml:reference "FirstName" ];
 
-  rr:predicateObjectMap [
-    rr:predicate foaf:name;
-    rr:objectMap [
+  rml:predicateObjectMap [
+    rml:predicate foaf:name;
+    rml:objectMap [
       rml:reference "FirstName"
     ]
   ] .
```

### Comparing `morph_kgc-2.6.4/test/rml/json/RMLTC0020a/RMLTC0020a_JSON.py` & `morph_kgc-2.7.0/test/rml-core/json/RMLTC0020a/RMLTC0020a_JSON.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/rml/json/RMLTC0020a/mapping.ttl` & `morph_kgc-2.7.0/test/rml-core/json/RMLTC0008c/mapping.ttl`

 * *Files 24% similar despite different names*

```diff
@@ -1,29 +1,23 @@
-@prefix rr: <http://www.w3.org/ns/r2rml#> .
 @prefix foaf: <http://xmlns.com/foaf/0.1/> .
-@prefix rdfs: <http://www.w3.org/2000/01/rdf-schema#> .
 @prefix ex: <http://example.com/> .
 @prefix xsd: <http://www.w3.org/2001/XMLSchema#> .
-@prefix rml: <http://semweb.mmlab.be/ns/rml#> .
-@prefix ql: <http://semweb.mmlab.be/ns/ql#> .
-@prefix rdf: <http://www.w3.org/1999/02/22-rdf-syntax-ns#> .
-
+@prefix rml: <http://w3id.org/rml/> .
+@prefix activity: <http://example.com/activity/> .
 @base <http://example.com/base/> .
 
 <TriplesMap1>
-  a rr:TriplesMap;
+  a rml:TriplesMap;
 
   rml:logicalSource [
-    rml:source "test/rml/json/RMLTC0020a/student.json";
-    rml:referenceFormulation ql:JSONPath;
+    rml:source "test/rml-core/json/RMLTC0008c/student.json";
+    rml:referenceFormulation rml:JSONPath;
     rml:iterator "$.students[*]"
   ];
 
-  rr:subjectMap [
-    rr:template "{Name}";
-    rr:termType rr:IRI
-  ];
+  rml:subjectMap [ rml:template "http://example.com/Student/{ID}/{Name}" ];
 
-  rr:predicateObjectMap [
-    rr:predicate rdf:type;
-    rr:object foaf:Person
-  ].
+  rml:predicateObjectMap [
+    rml:predicate foaf:name ;
+    rml:predicate ex:name ;
+    rml:objectMap [ rml:reference "Name" ]
+  ] .
```

### Comparing `morph_kgc-2.6.4/test/rml/json/RMLTC0020a/output.nq` & `morph_kgc-2.7.0/test/rml-core/json/RMLTC0020a/output.nq`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/rml/json/RMLTC0020b/RMLTC0020b_JSON.py` & `morph_kgc-2.7.0/test/rml-core/json/RMLTC0020b/RMLTC0020b_JSON.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/rml/json/RMLTC0020b/mapping.ttl` & `morph_kgc-2.7.0/test/rml-in-memory/json_dictionary/RMLIMTC0000/mapping.ttl`

 * *Files 24% similar despite different names*

```diff
@@ -1,25 +1,38 @@
-@prefix rr: <http://www.w3.org/ns/r2rml#> .
 @prefix foaf: <http://xmlns.com/foaf/0.1/> .
 @prefix ex: <http://example.com/> .
 @prefix xsd: <http://www.w3.org/2001/XMLSchema#> .
-@prefix rdf: <http://www.w3.org/1999/02/22-rdf-syntax-ns#> .
-@prefix rml:    <http://semweb.mmlab.be/ns/rml#> .
-@prefix ql:     <http://semweb.mmlab.be/ns/ql#> .
-
+@prefix rml: <http://w3id.org/rml/> .
+@prefix sd: <https://w3id.org/okn/o/sd#>.
+@prefix kg4di: <https://w3id.org/kg4di/definedBy>.
 @base <http://example.com/base/> .
 
 <TriplesMap1>
-  a rr:TriplesMap;
+  a rml:TriplesMap;
+
   rml:logicalSource [
-    rml:source "test/rml/json/RMLTC0020b/student.json";
-    rml:referenceFormulation ql:JSONPath;
+    rml:source [
+			a sd:DatasetSpecification;
+			sd:name "variable1";
+			sd:hasDataTransformation [
+				sd:hasSourceCode [
+					sd:programmingLanguage "Python3.9";
+				];
+			];
+		];
+		rml:referenceFormulation rml:Dictionary;
     rml:iterator "$.students[*]"
+  ] ;
+
+  rml:subjectMap [
+    rml:template "http://example.com/{Name}"
   ];
 
-    rr:subjectMap [ rml:reference "Name"; rr:termType rr:IRI; ];
+  rml:predicateObjectMap [
+    rml:predicate foaf:name ;
+    rml:objectMap [
+      rml:reference "Name"
+    ]
+  ].
 
-    rr:predicateObjectMap
-    [
-    	rr:predicate rdf:type;
-    	rr:object foaf:Person;
-    ].
+rml:Dictionary a rml:ReferenceFormulation;
+	kg4di:definedBy "Python".
```

### Comparing `morph_kgc-2.6.4/test/rml/json/complex/data.json` & `morph_kgc-2.7.0/test/rml-core/json/complex/data.json`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/rml/json/complex/mapping.yaml` & `morph_kgc-2.7.0/examples/json/mapping.json.yaml`

 * *Files 12% similar despite different names*

```diff
@@ -1,34 +1,36 @@
 prefixes:
   ex: "https://w3id.org/okn/os/o/"
+
 sources:
   main-source: ['data.json~jsonpath', '$.*']
   author-source: ['data.json~jsonpath', '$.*.author[*]']
   pid-source: ['data.json~jsonpath', '$.*.pid[*]']
+
 mappings:
   Author:
     sources:
       - author-source
-
     s: https://w3id.org/okn/os/i/author/$(fullname)
     po:
       - [a, ex:Author]
       - [ex:fullname, $(fullname)]
       - [ex:name, $(name)]
       - [ex:surname, $(surname)]
       - [ex:$(pid.id.scheme)ID, $(pid.id.value)]
+
   Paper:
     sources:
       - main-source
     s: https://w3id.org/okn/os/i/paper/$(id)
     po:
       - [a, ex:Paper]
       - [ex:title, $(maintitle)]
       - [ex:subtitle, $(subtitle)]
-      - [ex:description, $(description),$(language.code)~lang]
+      - [ex:description, $(description)]
       - [ex:language, $(language.label)]
       - [ex:format, $(format)]
       - [ex:publicationDate, $(publicationdate)]
       - [ex:type, $(type)]
       - [ex:country, $(country.*.label)]
       - [ex:license, $(instance.*.license)]
       - [ex:publisher, $(publisher)]
@@ -39,22 +41,24 @@
         o:
             - mapping: idTypeOpenAire
               condition:
                function: equal
                parameters:
                  - [str1, $(id)]
                  - [str2, $(id)]
+
   idTypeOpenAire:
     sources:
       - pid-source
     s: https://w3id.org/okn/os/i/idType/$(id)
     po:
       - [a, ex:idType]
       - [ex:source,OpenAire]
       - [ex:identifier,$(id)]
+
   idTypePaperResource:
     sources:
       - pid-source
     s: https://w3id.org/okn/os/i/idType/$(value)
     po:
       - [a, ex:idType]
       - [ex:source,$(scheme)]
```

### Comparing `morph_kgc-2.6.4/test/rml/json/complex/output.nq` & `morph_kgc-2.7.0/test/rml-core/json/complex/output.nq`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/rml/json/complex/test_complex_JSON.py` & `morph_kgc-2.7.0/test/rml-core/json/complex/test_complex_JSON.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/rml/tabular/RMLTC0002a_EXCEL/mapping.ttl` & `morph_kgc-2.7.0/test/rml-core/csv/RMLTC0007c/mapping.ttl`

 * *Files 19% similar despite different names*

```diff
@@ -1,29 +1,27 @@
-@prefix rr: <http://www.w3.org/ns/r2rml#> .
 @prefix foaf: <http://xmlns.com/foaf/0.1/> .
 @prefix ex: <http://example.com/> .
 @prefix xsd: <http://www.w3.org/2001/XMLSchema#> .
-@prefix rml: <http://semweb.mmlab.be/ns/rml#> .
-@prefix ql: <http://semweb.mmlab.be/ns/ql#> .
+@prefix rml: <http://w3id.org/rml/> .
 @base <http://example.com/base/> .
 
-<TriplesMap1> a rr:TriplesMap;
+<TriplesMap1> a rml:TriplesMap;
 
   rml:logicalSource [
-    rml:source "test/rml/tabular/RMLTC0002a_EXCEL/student.xlsx";
-    rml:referenceFormulation ql:CSV
+    rml:source "test/rml-core/csv/RMLTC0007c/student.csv";
+    rml:referenceFormulation rml:CSV
   ];
 
-  rr:subjectMap [
-    rr:template "http://example.com/{ID}/{Name}";
-    rr:class foaf:Person
+  rml:subjectMap [
+    rml:template "http://example.com/Student/{ID}/{FirstName}";
+    rml:class foaf:Person, ex:Student
   ];
 
-  rr:predicateObjectMap [
-    rr:predicate ex:id ;
-    rr:objectMap [ rml:reference "ID" ]
+  rml:predicateObjectMap [
+    rml:predicate ex:id ;
+    rml:objectMap [ rml:reference "ID";  ]
   ];
 
-  rr:predicateObjectMap [
-    rr:predicate foaf:name ;
-    rr:objectMap [ rml:reference "Name" ]
+  rml:predicateObjectMap [
+    rml:predicate foaf:name;
+    rml:objectMap [ rml:reference "FirstName" ]
   ].
```

### Comparing `morph_kgc-2.6.4/test/rml/tabular/RMLTC0002a_EXCEL/student.xlsx` & `morph_kgc-2.7.0/test/rml-core/tabular/RMLTC0002a_EXCEL/student.xlsx`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/rml/tabular/RMLTC0002a_EXCEL/test_RMLTC0002a_EXCEL.py` & `morph_kgc-2.7.0/test/rml-core/tabular/RMLTC0002a_EXCEL/test_RMLTC0002a_EXCEL.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/rml/tabular/RMLTC0002a_FEATHER/mapping.ttl` & `morph_kgc-2.7.0/test/rml-core/json/RMLTC0002b/mapping.ttl`

 * *Files 20% similar despite different names*

```diff
@@ -1,29 +1,23 @@
-@prefix rr: <http://www.w3.org/ns/r2rml#> .
 @prefix foaf: <http://xmlns.com/foaf/0.1/> .
 @prefix ex: <http://example.com/> .
 @prefix xsd: <http://www.w3.org/2001/XMLSchema#> .
-@prefix rml: <http://semweb.mmlab.be/ns/rml#> .
-@prefix ql: <http://semweb.mmlab.be/ns/ql#> .
+@prefix rml: <http://w3id.org/rml/> .
 @base <http://example.com/base/> .
 
-<TriplesMap1> a rr:TriplesMap;
+<TriplesMap1> a rml:TriplesMap;
 
   rml:logicalSource [
-    rml:source "test/rml/tabular/RMLTC0002a_FEATHER/student.feather";
-    rml:referenceFormulation ql:CSV
+    rml:source "test/rml-core/json/RMLTC0002b/student.json";
+    rml:referenceFormulation rml:JSONPath;
+    rml:iterator "$.students[*]"
   ];
 
-  rr:subjectMap [
-    rr:template "http://example.com/{ID}/{Name}";
-    rr:class foaf:Person
+  rml:subjectMap [
+    rml:template "students{ID}";
+    rml:termType rml:BlankNode
   ];
 
-  rr:predicateObjectMap [
-    rr:predicate ex:id ;
-    rr:objectMap [ rml:reference "ID" ]
-  ];
-
-  rr:predicateObjectMap [
-    rr:predicate foaf:name ;
-    rr:objectMap [ rml:reference "Name" ]
+  rml:predicateObjectMap [
+    rml:predicate foaf:name;
+    rml:objectMap [ rml:reference "Name" ]
   ].
```

### Comparing `morph_kgc-2.6.4/test/rml/tabular/RMLTC0002a_FEATHER/student.feather` & `morph_kgc-2.7.0/test/rml-core/tabular/RMLTC0002a_FEATHER/student.feather`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/rml/tabular/RMLTC0002a_FEATHER/test_RMLTC0002a_FEATHER.py` & `morph_kgc-2.7.0/test/rml-core/tabular/RMLTC0002a_FEATHER/test_RMLTC0002a_FEATHER.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/rml/tabular/RMLTC0002a_ODS/mapping.ttl` & `morph_kgc-2.7.0/test/rml-core/json/RMLTC0001b/mapping.ttl`

 * *Files 20% similar despite different names*

```diff
@@ -1,29 +1,26 @@
-@prefix rr: <http://www.w3.org/ns/r2rml#> .
 @prefix foaf: <http://xmlns.com/foaf/0.1/> .
 @prefix ex: <http://example.com/> .
 @prefix xsd: <http://www.w3.org/2001/XMLSchema#> .
-@prefix rml: <http://semweb.mmlab.be/ns/rml#> .
-@prefix ql: <http://semweb.mmlab.be/ns/ql#> .
+@prefix rml: <http://w3id.org/rml/> .
 @base <http://example.com/base/> .
 
-<TriplesMap1> a rr:TriplesMap;
+<TriplesMap1>
+  a rml:TriplesMap;
 
   rml:logicalSource [
-    rml:source "test/rml/tabular/RMLTC0002a_ODS/student.ods";
-    rml:referenceFormulation ql:CSV
+    rml:source "test/rml-core/json/RMLTC0001b/student.json";
+    rml:referenceFormulation rml:JSONPath;
+    rml:iterator "$.students[*]"
   ];
 
-  rr:subjectMap [
-    rr:template "http://example.com/{ID}/{Name}";
-    rr:class foaf:Person
+  rml:subjectMap [
+    rml:template "{Name}";
+    rml:termType rml:BlankNode
   ];
 
-  rr:predicateObjectMap [
-    rr:predicate ex:id ;
-    rr:objectMap [ rml:reference "ID" ]
-  ];
-
-  rr:predicateObjectMap [
-    rr:predicate foaf:name ;
-    rr:objectMap [ rml:reference "Name" ]
+  rml:predicateObjectMap [
+    rml:predicate foaf:name;
+    rml:objectMap [
+      rml:reference "Name"
+    ]
   ].
```

### Comparing `morph_kgc-2.6.4/test/rml/tabular/RMLTC0002a_ODS/student.ods` & `morph_kgc-2.7.0/test/rml-core/tabular/RMLTC0002a_ODS/student.ods`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/rml/tabular/RMLTC0002a_ODS/test_RMLTC0002a_ODS.py` & `morph_kgc-2.7.0/test/rml-core/tabular/RMLTC0002a_ODS/test_RMLTC0002a_ODS.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/rml/tabular/RMLTC0002a_PARQUET/mapping.ttl` & `morph_kgc-2.7.0/test/rml-core/tabular/RMLTC0002a_TSV/mapping.ttl`

 * *Files 14% similar despite different names*

```diff
@@ -1,29 +1,27 @@
-@prefix rr: <http://www.w3.org/ns/r2rml#> .
 @prefix foaf: <http://xmlns.com/foaf/0.1/> .
 @prefix ex: <http://example.com/> .
 @prefix xsd: <http://www.w3.org/2001/XMLSchema#> .
-@prefix rml: <http://semweb.mmlab.be/ns/rml#> .
-@prefix ql: <http://semweb.mmlab.be/ns/ql#> .
+@prefix rml: <http://w3id.org/rml/> .
 @base <http://example.com/base/> .
 
-<TriplesMap1> a rr:TriplesMap;
+<TriplesMap1> a rml:TriplesMap;
 
   rml:logicalSource [
-    rml:source "test/rml/tabular/RMLTC0002a_PARQUET/student.parquet";
-    rml:referenceFormulation ql:CSV
+    rml:source "test/rml-core/tabular/RMLTC0002a_TSV/student.tsv";
+    rml:referenceFormulation rml:CSV
   ];
 
-  rr:subjectMap [
-    rr:template "http://example.com/{ID}/{Name}";
-    rr:class foaf:Person
+  rml:subjectMap [
+    rml:template "http://example.com/{ID}/{Name}";
+    rml:class foaf:Person
   ];
 
-  rr:predicateObjectMap [
-    rr:predicate ex:id ;
-    rr:objectMap [ rml:reference "ID" ]
+  rml:predicateObjectMap [
+    rml:predicate ex:id ;
+    rml:objectMap [ rml:reference "ID" ]
   ];
 
-  rr:predicateObjectMap [
-    rr:predicate foaf:name ;
-    rr:objectMap [ rml:reference "Name" ]
+  rml:predicateObjectMap [
+    rml:predicate foaf:name ;
+    rml:objectMap [ rml:reference "Name" ]
   ].
```

### Comparing `morph_kgc-2.6.4/test/rml/tabular/RMLTC0002a_PARQUET/student.parquet` & `morph_kgc-2.7.0/test/rml-core/tabular/RMLTC0002a_PARQUET/student.parquet`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/rml/tabular/RMLTC0002a_PARQUET/test_RMLTC0002a_PARQUET.py` & `morph_kgc-2.7.0/test/rml-core/tabular/RMLTC0002a_PARQUET/test_RMLTC0002a_PARQUET.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/rml/tabular/RMLTC0002a_STATA/mapping.ttl` & `morph_kgc-2.7.0/test/rml-core/csv/null_filter/mapping.ttl`

 * *Files 14% similar despite different names*

```diff
@@ -1,29 +1,27 @@
-@prefix rr: <http://www.w3.org/ns/r2rml#> .
 @prefix foaf: <http://xmlns.com/foaf/0.1/> .
 @prefix ex: <http://example.com/> .
 @prefix xsd: <http://www.w3.org/2001/XMLSchema#> .
-@prefix rml: <http://semweb.mmlab.be/ns/rml#> .
-@prefix ql: <http://semweb.mmlab.be/ns/ql#> .
+@prefix rml: <http://w3id.org/rml/> .
 @base <http://example.com/base/> .
 
-<TriplesMap1> a rr:TriplesMap;
+<TriplesMap1> a rml:TriplesMap;
 
   rml:logicalSource [
-    rml:source "test/rml/tabular/RMLTC0002a_STATA/student.dta";
-    rml:referenceFormulation ql:CSV
+    rml:source "test/rml-core/csv/null_filter/student.csv";
+    rml:referenceFormulation rml:CSV
   ];
 
-  rr:subjectMap [
-    rr:template "http://example.com/{ID}/{Name}";
-    rr:class foaf:Person
+  rml:subjectMap [
+    rml:template "http://example.com/{ID}/{Name}";
+    rml:class foaf:Person
   ];
 
-  rr:predicateObjectMap [
-    rr:predicate ex:id ;
-    rr:objectMap [ rml:reference "ID" ]
+  rml:predicateObjectMap [
+    rml:predicate ex:id ;
+    rml:objectMap [ rml:reference "ID" ]
   ];
 
-  rr:predicateObjectMap [
-    rr:predicate foaf:name ;
-    rr:objectMap [ rml:reference "Name" ]
+  rml:predicateObjectMap [
+    rml:predicate foaf:name ;
+    rml:objectMap [ rml:reference "Name" ]
   ].
```

### Comparing `morph_kgc-2.6.4/test/rml/tabular/RMLTC0002a_STATA/student.dta` & `morph_kgc-2.7.0/test/rml-core/tabular/RMLTC0002a_STATA/student.dta`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/rml/tabular/RMLTC0002a_STATA/test_RMLTC0002a_STATA.py` & `morph_kgc-2.7.0/test/rml-core/tabular/RMLTC0002a_STATA/test_RMLTC0002a_STATA.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/rml/tabular/RMLTC0002a_TSV/mapping.ttl` & `morph_kgc-2.7.0/test/rml-core/xml/RMLTC0001a/mapping.ttl`

 * *Files 21% similar despite different names*

```diff
@@ -1,29 +1,26 @@
-@prefix rr: <http://www.w3.org/ns/r2rml#> .
 @prefix foaf: <http://xmlns.com/foaf/0.1/> .
 @prefix ex: <http://example.com/> .
 @prefix xsd: <http://www.w3.org/2001/XMLSchema#> .
-@prefix rml: <http://semweb.mmlab.be/ns/rml#> .
-@prefix ql: <http://semweb.mmlab.be/ns/ql#> .
+@prefix rml: <http://w3id.org/rml/> .
+
 @base <http://example.com/base/> .
 
-<TriplesMap1> a rr:TriplesMap;
+<TriplesMap1>
+  a rml:TriplesMap;
 
   rml:logicalSource [
-    rml:source "test/rml/tabular/RMLTC0002a_TSV/student.tsv";
-    rml:referenceFormulation ql:CSV
-  ];
-
-  rr:subjectMap [
-    rr:template "http://example.com/{ID}/{Name}";
-    rr:class foaf:Person
+    rml:source "test/rml-core/xml/RMLTC0001a/student.xml";
+    rml:referenceFormulation rml:XPath;
+    rml:iterator "/students/student"
   ];
 
-  rr:predicateObjectMap [
-    rr:predicate ex:id ;
-    rr:objectMap [ rml:reference "ID" ]
+  rml:subjectMap [
+    rml:template "http://example.com/{Name}"
   ];
 
-  rr:predicateObjectMap [
-    rr:predicate foaf:name ;
-    rr:objectMap [ rml:reference "Name" ]
+  rml:predicateObjectMap [
+    rml:predicate foaf:name;
+    rml:objectMap [
+      rml:reference "Name"
+    ]
   ].
```

### Comparing `morph_kgc-2.6.4/test/rml/tabular/RMLTC0002a_TSV/test_RMLTC0002a_TSV.py` & `morph_kgc-2.7.0/test/rml-core/tabular/RMLTC0002a_TSV/test_RMLTC0002a_TSV.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/rml/xml/RMLTC0000/mapping.ttl` & `morph_kgc-2.7.0/test/rml-core/xml/RMLTC0002b/mapping.ttl`

 * *Files 18% similar despite different names*

```diff
@@ -1,28 +1,23 @@
-@prefix rr: <http://www.w3.org/ns/r2rml#> .
 @prefix foaf: <http://xmlns.com/foaf/0.1/> .
 @prefix ex: <http://example.com/> .
 @prefix xsd: <http://www.w3.org/2001/XMLSchema#> .
-@prefix rml: <http://semweb.mmlab.be/ns/rml#> .
-@prefix ql: <http://semweb.mmlab.be/ns/ql#> .
-
+@prefix rml: <http://w3id.org/rml/> .
 @base <http://example.com/base/> .
 
-<TriplesMap1>
-  a rr:TriplesMap;
+<TriplesMap1> a rml:TriplesMap;
 
   rml:logicalSource [
-    rml:source "test/rml/xml/RMLTC0000/student.xml";
-    rml:referenceFormulation ql:XPath;
+    rml:source "test/rml-core/xml/RMLTC0002b/student.xml";
+    rml:referenceFormulation rml:XPath;
     rml:iterator "/students/student"
-  ] ;
+  ];
 
-  rr:subjectMap [
-    rr:template "http://example.com/{Name}"
+  rml:subjectMap [
+    rml:template "students{ID}";
+    rml:termType rml:BlankNode
   ];
 
-  rr:predicateObjectMap [
-    rr:predicate foaf:name ;
-    rr:objectMap [
-      rml:reference "Name"
-    ]
+  rml:predicateObjectMap [
+    rml:predicate foaf:name;
+    rml:objectMap [ rml:reference "Name" ]
   ].
```

### Comparing `morph_kgc-2.6.4/test/rml/xml/RMLTC0000/test_RMLTC0000_XML.py` & `morph_kgc-2.7.0/test/rml-core/xml/RMLTC0000/test_RMLTC0000_XML.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/rml/xml/RMLTC0001a/mapping.ttl` & `morph_kgc-2.7.0/test/rml-core/xml/RMLTC0007a/mapping.ttl`

 * *Files 18% similar despite different names*

```diff
@@ -1,28 +1,23 @@
-@prefix rr: <http://www.w3.org/ns/r2rml#> .
 @prefix foaf: <http://xmlns.com/foaf/0.1/> .
 @prefix ex: <http://example.com/> .
 @prefix xsd: <http://www.w3.org/2001/XMLSchema#> .
-@prefix rml: <http://semweb.mmlab.be/ns/rml#> .
-@prefix ql: <http://semweb.mmlab.be/ns/ql#> .
-
+@prefix rml: <http://w3id.org/rml/> .
+@prefix rdf: <http://www.w3.org/1999/02/22-rdf-syntax-ns#> .
 @base <http://example.com/base/> .
 
-<TriplesMap1>
-  a rr:TriplesMap;
+<TriplesMap1> a rml:TriplesMap;
 
   rml:logicalSource [
-    rml:source "test/rml/xml/RMLTC0001a/student.xml";
-    rml:referenceFormulation ql:XPath;
+    rml:source "test/rml-core/xml/RMLTC0007a/student.xml";
+    rml:referenceFormulation rml:XPath;
     rml:iterator "/students/student"
   ];
 
-  rr:subjectMap [
-    rr:template "http://example.com/{Name}"
+  rml:subjectMap [
+    rml:template "http://example.com/Student/{ID}/{FirstName}"
   ];
 
-  rr:predicateObjectMap [
-    rr:predicate foaf:name;
-    rr:objectMap [
-      rml:reference "Name"
-    ]
+  rml:predicateObjectMap [
+    rml:predicate rdf:type;
+    rml:object foaf:Person;
   ].
```

### Comparing `morph_kgc-2.6.4/test/rml/xml/RMLTC0001a/test_RMLTC0001a_XML.py` & `morph_kgc-2.7.0/test/rml-core/xml/RMLTC0001a/test_RMLTC0001a_XML.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/rml/xml/RMLTC0001b/mapping.ttl` & `morph_kgc-2.7.0/test/rml-core/xml/RMLTC0007d/mapping.ttl`

 * *Files 19% similar despite different names*

```diff
@@ -1,28 +1,38 @@
-@prefix rr: <http://www.w3.org/ns/r2rml#> .
 @prefix foaf: <http://xmlns.com/foaf/0.1/> .
 @prefix ex: <http://example.com/> .
 @prefix xsd: <http://www.w3.org/2001/XMLSchema#> .
-@prefix rml: <http://semweb.mmlab.be/ns/rml#> .
-@prefix ql: <http://semweb.mmlab.be/ns/ql#> .
+@prefix rml: <http://w3id.org/rml/> .
+@prefix rdf: <http://www.w3.org/1999/02/22-rdf-syntax-ns#> .
 @base <http://example.com/base/> .
 
-<TriplesMap1>
-  a rr:TriplesMap;
+<TriplesMap1> a rml:TriplesMap;
 
   rml:logicalSource [
-    rml:source "test/rml/xml/RMLTC0001b/student.xml";
-    rml:referenceFormulation ql:XPath;
+    rml:source "test/rml-core/xml/RMLTC0007d/student.xml";
+    rml:referenceFormulation rml:XPath;
     rml:iterator "/students/student"
   ];
 
-  rr:subjectMap [
-    rr:template "{Name}";
-    rr:termType rr:BlankNode
+  rml:subjectMap [
+    rml:template "http://example.com/Student/{ID}/{FirstName}"
   ];
 
-  rr:predicateObjectMap [
-    rr:predicate foaf:name;
-    rr:objectMap [
-      rml:reference "Name"
-    ]
+  rml:predicateObjectMap [
+    rml:predicate rdf:type;
+    rml:object foaf:Person;
+  ];
+
+  rml:predicateObjectMap [
+    rml:predicate rdf:type;
+    rml:object ex:Student;
+  ];
+
+  rml:predicateObjectMap [
+    rml:predicate ex:id;
+    rml:objectMap [rml:reference "ID"]
+  ];
+
+  rml:predicateObjectMap [
+    rml:predicate foaf:name;
+    rml:objectMap [ rml:reference "FirstName" ]
   ].
```

### Comparing `morph_kgc-2.6.4/test/rml/xml/RMLTC0001b/test_RMLTC0001b_XML.py` & `morph_kgc-2.7.0/test/rml-core/xml/RMLTC0001b/test_RMLTC0001b_XML.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/rml/xml/RMLTC0002a/mapping.ttl` & `morph_kgc-2.7.0/test/rml-core/csv/RMLTC0002a/mapping.ttl`

 * *Files 13% similar despite different names*

```diff
@@ -1,30 +1,27 @@
-@prefix rr: <http://www.w3.org/ns/r2rml#> .
 @prefix foaf: <http://xmlns.com/foaf/0.1/> .
 @prefix ex: <http://example.com/> .
 @prefix xsd: <http://www.w3.org/2001/XMLSchema#> .
-@prefix rml: <http://semweb.mmlab.be/ns/rml#> .
-@prefix ql: <http://semweb.mmlab.be/ns/ql#> .
+@prefix rml: <http://w3id.org/rml/> .
 @base <http://example.com/base/> .
 
-<TriplesMap1> a rr:TriplesMap;
+<TriplesMap1> a rml:TriplesMap;
 
   rml:logicalSource [
-    rml:source "test/rml/xml/RMLTC0002a/student.xml";
-    rml:referenceFormulation ql:XPath;
-    rml:iterator "/students/student"
+    rml:source "test/rml-core/csv/RMLTC0002a/student.csv";
+    rml:referenceFormulation rml:CSV
   ];
 
-  rr:subjectMap [
-    rr:template "http://example.com/{ID}/{Name}";
-    rr:class foaf:Person
+  rml:subjectMap [
+    rml:template "http://example.com/{ID}/{Name}";
+    rml:class foaf:Person
   ];
 
-  rr:predicateObjectMap [
-    rr:predicate ex:id ;
-    rr:objectMap [ rml:reference "ID" ]
+  rml:predicateObjectMap [
+    rml:predicate ex:id ;
+    rml:objectMap [ rml:reference "ID" ]
   ];
 
-  rr:predicateObjectMap [
-    rr:predicate foaf:name ;
-    rr:objectMap [ rml:reference "Name" ]
+  rml:predicateObjectMap [
+    rml:predicate foaf:name ;
+    rml:objectMap [ rml:reference "Name" ]
   ].
```

### Comparing `morph_kgc-2.6.4/test/rml/xml/RMLTC0002a/test_RMLTC0002a_XML.py` & `morph_kgc-2.7.0/test/rml-core/xml/RMLTC0002a/test_RMLTC0002a_XML.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/rml/xml/RMLTC0002b/mapping.ttl` & `morph_kgc-2.7.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0007e/mapping.ttl`

 * *Files 24% similar despite different names*

```diff
@@ -1,25 +1,43 @@
-@prefix rr: <http://www.w3.org/ns/r2rml#> .
 @prefix foaf: <http://xmlns.com/foaf/0.1/> .
 @prefix ex: <http://example.com/> .
 @prefix xsd: <http://www.w3.org/2001/XMLSchema#> .
-@prefix rml: <http://semweb.mmlab.be/ns/rml#> .
-@prefix ql: <http://semweb.mmlab.be/ns/ql#> .
+@prefix rml: <http://w3id.org/rml/> .
 @base <http://example.com/base/> .
+@prefix sd: <https://w3id.org/okn/o/sd#>.
+@prefix kg4di: <https://w3id.org/kg4di/definedBy>.
 
-<TriplesMap1> a rr:TriplesMap;
+<TriplesMap1> a rml:TriplesMap;
 
   rml:logicalSource [
-    rml:source "test/rml/xml/RMLTC0002b/student.xml";
-    rml:referenceFormulation ql:XPath;
-    rml:iterator "/students/student"
+    rml:source [
+			a sd:DatasetSpecification;
+			sd:name "variable1";
+			sd:hasDataTransformation [
+				sd:hasSoftwareRequirements "pandas>=1.1.0";
+				sd:hasSourceCode [
+					sd:programmingLanguage "Python3.9";
+				];
+			];
+		];
+    rml:referenceFormulation rml:DataFrame;
   ];
 
-  rr:subjectMap [
-    rr:template "students{ID}";
-    rr:termType rr:BlankNode
+  rml:subjectMap [
+    rml:template "http://example.com/Student/{ID}/{Name}";
+    rml:graph ex:PersonGraph ;
+    rml:class foaf:Person
   ];
 
-  rr:predicateObjectMap [
-    rr:predicate foaf:name;
-    rr:objectMap [ rml:reference "Name" ]
-  ].
+  rml:predicateObjectMap [
+    rml:predicate ex:id ;
+    rml:objectMap [ rml:reference "ID"; ]
+  ];
+
+  rml:predicateObjectMap
+    [
+      rml:predicate		foaf:name ;
+      rml:objectMap		[ rml:reference "Name" ]
+    ].
+
+rml:DataFrame a rml:ReferenceFormulation;
+	kg4di:definedBy "Pandas".
```

### Comparing `morph_kgc-2.6.4/test/rml/xml/RMLTC0002b/test_RMLTC0002b_XML.py` & `morph_kgc-2.7.0/test/rml-core/xml/RMLTC0002b/test_RMLTC0002b_XML.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/rml/xml/RMLTC0002c/mapping.ttl` & `morph_kgc-2.7.0/test/rml-core/csv/RMLTC0012c/mapping.ttl`

 * *Files 20% similar despite different names*

```diff
@@ -1,24 +1,29 @@
-@prefix rr: <http://www.w3.org/ns/r2rml#> .
 @prefix foaf: <http://xmlns.com/foaf/0.1/> .
 @prefix ex: <http://example.com/> .
 @prefix xsd: <http://www.w3.org/2001/XMLSchema#> .
-@prefix rml: <http://semweb.mmlab.be/ns/rml#> .
-@prefix ql: <http://semweb.mmlab.be/ns/ql#> .
+@prefix rml: <http://w3id.org/rml/> .
+
 @base <http://example.com/base/> .
 
-<TriplesMap1> a rr:TriplesMap;
+<TriplesMap1>
+  a rml:TriplesMap;
 
   rml:logicalSource [
-    rml:source "test/rml/xml/RMLTC0002c/student.xml";
-    rml:referenceFormulation ql:XPath;
-    rml:iterator "/students/student"
+    rml:source "test/rml-core/csv/RMLTC0012c/persons.csv";
+    rml:referenceFormulation rml:CSV
   ];
 
-  rr:subjectMap [
-    rr:template "http://example.com/{ID}/{Name}";
+  rml:predicateObjectMap [
+    rml:predicate foaf:name ;
+    rml:objectMap [
+      rml:template "{fname} {lname}";
+      rml:termType rml:Literal ;
+    ]
   ];
 
-  rr:predicateObjectMap [
-    rr:predicate ex:id ;
-    rr:objectMap [ rml:reference "IDs" ]
+  rml:predicateObjectMap [
+    rml:predicate ex:amount ;
+    rml:objectMap    [
+      rml:reference "amount";
+    ]
   ].
```

### Comparing `morph_kgc-2.6.4/test/rml/xml/RMLTC0002c/test_RMLTC0002c_XML.py` & `morph_kgc-2.7.0/test/rml-core/xml/RMLTC0002c/test_RMLTC0002c_XML.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/rml/xml/RMLTC0002e/mapping.ttl` & `morph_kgc-2.7.0/test/rml-core/json/RMLTC0013a/mapping.ttl`

 * *Files 21% similar despite different names*

```diff
@@ -1,24 +1,23 @@
-@prefix rr: <http://www.w3.org/ns/r2rml#> .
 @prefix foaf: <http://xmlns.com/foaf/0.1/> .
 @prefix ex: <http://example.com/> .
 @prefix xsd: <http://www.w3.org/2001/XMLSchema#> .
-@prefix rml: <http://semweb.mmlab.be/ns/rml#> .
-@prefix ql: <http://semweb.mmlab.be/ns/ql#> .
+@prefix rml: <http://w3id.org/rml/> .
+
 @base <http://example.com/base/> .
 
-<TriplesMap1> a rr:TriplesMap;
+<TriplesMap1>
+  a rml:TriplesMap;
 
   rml:logicalSource [
-    rml:source "test/rml/xml/RMLTC0002e/student2.xml";
-    rml:referenceFormulation ql:XPath;
-    rml:iterator "/students/student"
+    rml:source "test/rml-core/json/RMLTC0013a/persons.json";
+    rml:referenceFormulation rml:JSONPath;
+    rml:iterator "$.persons[*]"
   ];
 
-  rr:subjectMap [
-    rr:template "http://example.com/{ID}/{Name}";
-  ];
+  rml:subjectMap [ rml:template "http://example.com/Person/{ID}/{Name}/{DateOfBirth}"];
 
-  rr:predicateObjectMap [
-    rr:predicate ex:id ;
-    rr:objectMap [ rml:reference "ID" ]
-  ].
+  rml:predicateObjectMap
+    [
+      rml:predicate		ex:BirthDay ;
+      rml:objectMap		[ rml:reference "DateOfBirth" ]
+    ].
```

### Comparing `morph_kgc-2.6.4/test/rml/xml/RMLTC0002e/test_RMLTC0002e_XML.py` & `morph_kgc-2.7.0/test/rml-core/xml/RMLTC0002e/test_RMLTC0002e_XML.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/rml/xml/RMLTC0003c/mapping.ttl` & `morph_kgc-2.7.0/test/rml-core/csv/RMLTC0004a/mapping.ttl`

 * *Files 25% similar despite different names*

```diff
@@ -1,27 +1,43 @@
-@prefix rr: <http://www.w3.org/ns/r2rml#> .
 @prefix foaf: <http://xmlns.com/foaf/0.1/> .
 @prefix ex: <http://example.com/> .
 @prefix xsd: <http://www.w3.org/2001/XMLSchema#> .
-@prefix rml: <http://semweb.mmlab.be/ns/rml#> .
-@prefix ql: <http://semweb.mmlab.be/ns/ql#> .
+@prefix rml: <http://w3id.org/rml/> .
 @base <http://example.com/base/> .
 
-<TriplesMap1> a rr:TriplesMap;
+<TriplesMap1> a rml:TriplesMap;
 
   rml:logicalSource [
-    rml:source "test/rml/xml/RMLTC0003c/student.xml";
-    rml:referenceFormulation ql:XPath;
-    rml:iterator "/students/student"
+    rml:source "test/rml-core/csv/RMLTC0004a/student_sport.csv";
+    rml:referenceFormulation rml:CSV
   ];
 
-  rr:subjectMap [
-    rr:template "http://example.com/Student{ID}";
+  rml:subjectMap [
+    rml:template "http://example.com/{Student}";
+    rml:class ex:Student
   ];
 
-  rr:predicateObjectMap [
-    rr:predicate foaf:name;
-    rr:objectMap [
-      rr:template "{FirstName} {LastName}";
-      rr:termType rr:Literal;
+  rml:predicateObjectMap [
+    rml:predicate foaf:name ;
+    rml:objectMap [
+      rml:reference "Student"
+    ]
+  ].
+
+<TriplesMap2> a rml:TriplesMap;
+
+  rml:logicalSource [
+    rml:source "test/rml-core/csv/RMLTC0004a/student_sport.csv";
+    rml:referenceFormulation rml:CSV
+  ];
+
+  rml:subjectMap [
+    rml:template "http://example.com/{Sport}";
+    rml:class ex:Sport
+  ];
+
+  rml:predicateObjectMap [
+    rml:predicate foaf:name ;
+    rml:objectMap [
+      rml:reference "Sport"
     ]
   ].
```

### Comparing `morph_kgc-2.6.4/test/rml/xml/RMLTC0003c/test_RMLTC0003c_XML.py` & `morph_kgc-2.7.0/test/rml-core/xml/RMLTC0003c/test_RMLTC0003c_XML.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/rml/xml/RMLTC0004a/mapping.ttl` & `morph_kgc-2.7.0/test/rml-core/xml/RMLTC0004a/mapping.ttl`

 * *Files 18% similar despite different names*

```diff
@@ -1,47 +1,45 @@
-@prefix rr: <http://www.w3.org/ns/r2rml#> .
 @prefix foaf: <http://xmlns.com/foaf/0.1/> .
 @prefix ex: <http://example.com/> .
 @prefix xsd: <http://www.w3.org/2001/XMLSchema#> .
-@prefix rml: <http://semweb.mmlab.be/ns/rml#> .
-@prefix ql: <http://semweb.mmlab.be/ns/ql#> .
+@prefix rml: <http://w3id.org/rml/> .
 @base <http://example.com/base/> .
 
-<TriplesMap1> a rr:TriplesMap;
+<TriplesMap1> a rml:TriplesMap;
 
   rml:logicalSource [
-    rml:source "test/rml/xml/RMLTC0004a/student_sport.xml";
-    rml:referenceFormulation ql:XPath;
+    rml:source "test/rml-core/xml/RMLTC0004a/student_sport.xml";
+    rml:referenceFormulation rml:XPath;
     rml:iterator "/students/student"
   ];
 
-  rr:subjectMap [
-    rr:template "http://example.com/{Student}";
-    rr:class ex:Student
+  rml:subjectMap [
+    rml:template "http://example.com/{Student}";
+    rml:class ex:Student
   ];
 
-  rr:predicateObjectMap [
-    rr:predicate foaf:name ;
-    rr:objectMap [
+  rml:predicateObjectMap [
+    rml:predicate foaf:name ;
+    rml:objectMap [
       rml:reference "Student"
     ]
   ].
 
-<TriplesMap2> a rr:TriplesMap;
+<TriplesMap2> a rml:TriplesMap;
 
   rml:logicalSource [
-    rml:source "test/rml/xml/RMLTC0004a/student_sport.xml";
-    rml:referenceFormulation ql:XPath;
+    rml:source "test/rml-core/xml/RMLTC0004a/student_sport.xml";
+    rml:referenceFormulation rml:XPath;
     rml:iterator "/students/student"
   ];
 
-  rr:subjectMap [
-    rr:template "http://example.com/{Sport}";
-    rr:class ex:Sport
+  rml:subjectMap [
+    rml:template "http://example.com/{Sport}";
+    rml:class ex:Sport
   ];
 
-  rr:predicateObjectMap [
-    rr:predicate foaf:name ;
-    rr:objectMap [
+  rml:predicateObjectMap [
+    rml:predicate foaf:name ;
+    rml:objectMap [
       rml:reference "Sport"
     ]
   ].
```

### Comparing `morph_kgc-2.6.4/test/rml/xml/RMLTC0004a/test_RMLTC0004a_XML.py` & `morph_kgc-2.7.0/test/rml-core/xml/RMLTC0004a/test_RMLTC0004a_XML.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/rml/xml/RMLTC0004b/mapping.ttl` & `morph_kgc-2.7.0/test/rml-core/csv/RMLTC0002c/mapping.ttl`

 * *Files 25% similar despite different names*

```diff
@@ -1,29 +1,21 @@
-@prefix rr: <http://www.w3.org/ns/r2rml#> .
 @prefix foaf: <http://xmlns.com/foaf/0.1/> .
 @prefix ex: <http://example.com/> .
 @prefix xsd: <http://www.w3.org/2001/XMLSchema#> .
-@prefix rml: <http://semweb.mmlab.be/ns/rml#> .
-@prefix ql: <http://semweb.mmlab.be/ns/ql#> .
-
+@prefix rml: <http://w3id.org/rml/> .
 @base <http://example.com/base/> .
 
-<TriplesMap1>
-  a rr:TriplesMap;
+<TriplesMap1> a rml:TriplesMap;
 
   rml:logicalSource [
-    rml:source "test/rml/xml/RMLTC0004b/student.xml";
-    rml:referenceFormulation ql:XPath;
-    rml:iterator "/students/student"
+    rml:source "test/rml-core/csv/RMLTC0002c/student.csv";
+    rml:referenceFormulation rml:CSV
   ];
 
-  rr:subjectMap [
-    rr:template "http://example.com/{Name}";
-    rr:termType rr:Literal
+  rml:subjectMap [
+    rml:template "http://example.com/{ID}/{Name}";
   ];
 
-  rr:predicateObjectMap [
-    rr:predicate foaf:name;
-    rr:objectMap [
-      rml:reference "Name"
-    ]
+  rml:predicateObjectMap [
+    rml:predicate ex:id ;
+    rml:objectMap [ rml:reference "IDs" ]
   ].
```

### Comparing `morph_kgc-2.6.4/test/rml/xml/RMLTC0004b/test_RMLTC0004b_XML.py` & `morph_kgc-2.7.0/test/rml-core/xml/RMLTC0004b/test_RMLTC0004b_XML.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/rml/xml/RMLTC0005a/mapping.ttl` & `morph_kgc-2.7.0/test/rml-fnml/RMLFNOTC0003-CSV/mapping.ttl`

 * *Files 25% similar despite different names*

```diff
@@ -1,25 +1,39 @@
-@prefix rr: <http://www.w3.org/ns/r2rml#> .
 @prefix foaf: <http://xmlns.com/foaf/0.1/> .
 @prefix ex: <http://example.com/> .
 @prefix xsd: <http://www.w3.org/2001/XMLSchema#> .
-@prefix rml: <http://semweb.mmlab.be/ns/rml#> .
-@prefix ql: <http://semweb.mmlab.be/ns/ql#> .
-@base <http://example.com/base/> .
-
-<TriplesMap1> a rr:TriplesMap;
+@prefix rml: <http://w3id.org/rml/> .
+@prefix fno: <https://w3id.org/function/ontology#> .
+@prefix morph-kgc: <https://github.com/morph-kgc/morph-kgc/function/built-in.ttl#> .
+@prefix grel: <http://users.ugent.be/~bjdmeest/function/grel.ttl#> .
+@prefix idlab-fn: <http://example.com/idlab/function/> .
 
-  rml:logicalSource [
-    rml:source "test/rml/xml/RMLTC0005a/ious.xml";
-    rml:referenceFormulation ql:XPath;
-    rml:iterator "/persons/person"
-  ];
+@base <http://example.com/base/> .
 
-  rr:subjectMap [
-    rr:template "http://example.com/{fname};{lname}";
-    rr:class foaf:Person;
-  ];
+<TriplesMap1>
+    rml:logicalSource [
+        rml:source "test/rml-fnml/RMLFNOTC0003-CSV/student.csv";
+        rml:referenceFormulation rml:CSV
+    ];
+    rml:subjectMap [
+        rml:template "http://example.com/{Name}"
+    ];
+    rml:predicateObjectMap [
+        rml:predicate foaf:name;
+        rml:objectMap [
+            rml:functionExecution <#Execution> ;
+        ]
+    ] .
 
-  rr:predicateObjectMap [
-    rr:predicate ex:owes;
-    rr:objectMap [ rml:reference "amount"; ]
-  ].
+<#Execution>
+    rml:function grel:escape ;
+    rml:input
+        [
+            rml:parameter grel:valueParam ;
+            rml:inputValueMap [
+                rml:reference "Comment"
+            ]
+        ] ,
+        [
+            rml:parameter grel:modeParam ;
+            rml:inputValue "html"
+        ] .
```

### Comparing `morph_kgc-2.6.4/test/rml/xml/RMLTC0005a/test_RMLTC0005a_XML.py` & `morph_kgc-2.7.0/test/rml-core/xml/RMLTC0005a/test_RMLTC0005a_XML.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/rml/xml/RMLTC0006a/mapping.ttl` & `morph_kgc-2.7.0/test/rml-core/xml/RMLTC0003c/mapping.ttl`

 * *Files 18% similar despite different names*

```diff
@@ -1,25 +1,25 @@
-@prefix rr: <http://www.w3.org/ns/r2rml#> .
 @prefix foaf: <http://xmlns.com/foaf/0.1/> .
 @prefix ex: <http://example.com/> .
 @prefix xsd: <http://www.w3.org/2001/XMLSchema#> .
-@prefix rml: <http://semweb.mmlab.be/ns/rml#> .
-@prefix ql: <http://semweb.mmlab.be/ns/ql#> .
+@prefix rml: <http://w3id.org/rml/> .
 @base <http://example.com/base/> .
 
-<TriplesMap1> a rr:TriplesMap;
+<TriplesMap1> a rml:TriplesMap;
 
   rml:logicalSource [
-    rml:source "test/rml/xml/RMLTC0006a/student.xml";
-    rml:referenceFormulation ql:XPath;
+    rml:source "test/rml-core/xml/RMLTC0003c/student.xml";
+    rml:referenceFormulation rml:XPath;
     rml:iterator "/students/student"
   ];
 
-  rr:subjectMap [
-    rr:constant ex:BadStudent;
-    rr:graphMap [ rr:constant <http://example.com/graph/student> ];
+  rml:subjectMap [
+    rml:template "http://example.com/Student{ID}";
   ];
 
-  rr:predicateObjectMap [
-    rr:predicateMap [ rr:constant ex:description ];
-    rr:objectMap [ rr:constant "Bad Student"; ]
+  rml:predicateObjectMap [
+    rml:predicate foaf:name;
+    rml:objectMap [
+      rml:template "{FirstName} {LastName}";
+      rml:termType rml:Literal;
+    ]
   ].
```

### Comparing `morph_kgc-2.6.4/test/rml/xml/RMLTC0006a/test_RMLTC0006a_XML.py` & `morph_kgc-2.7.0/test/rml-core/xml/RMLTC0006a/test_RMLTC0006a_XML.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/rml/xml/RMLTC0007a/mapping.ttl` & `morph_kgc-2.7.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0007c/mapping.ttl`

 * *Files 25% similar despite different names*

```diff
@@ -1,25 +1,41 @@
-@prefix rr: <http://www.w3.org/ns/r2rml#> .
 @prefix foaf: <http://xmlns.com/foaf/0.1/> .
 @prefix ex: <http://example.com/> .
 @prefix xsd: <http://www.w3.org/2001/XMLSchema#> .
-@prefix rml: <http://semweb.mmlab.be/ns/rml#> .
-@prefix ql: <http://semweb.mmlab.be/ns/ql#> .
-@prefix rdf: <http://www.w3.org/1999/02/22-rdf-syntax-ns#> .
+@prefix rml: <http://w3id.org/rml/> .
 @base <http://example.com/base/> .
+@prefix sd: <https://w3id.org/okn/o/sd#>.
+@prefix kg4di: <https://w3id.org/kg4di/definedBy>.
 
-<TriplesMap1> a rr:TriplesMap;
+<TriplesMap1> a rml:TriplesMap;
 
   rml:logicalSource [
-    rml:source "test/rml/xml/RMLTC0007a/student.xml";
-    rml:referenceFormulation ql:XPath;
-    rml:iterator "/students/student"
+    rml:source [
+			a sd:DatasetSpecification;
+			sd:name "variable1";
+			sd:hasDataTransformation [
+				sd:hasSoftwareRequirements "pandas>=1.1.0";
+				sd:hasSourceCode [
+					sd:programmingLanguage "Python3.9";
+				];
+			];
+		];
+    rml:referenceFormulation rml:DataFrame;
   ];
 
-  rr:subjectMap [
-    rr:template "http://example.com/Student/{ID}/{FirstName}"
+  rml:subjectMap [
+    rml:template "http://example.com/Student/{ID}/{FirstName}";
+    rml:class foaf:Person, ex:Student
   ];
 
-  rr:predicateObjectMap [
-    rr:predicate rdf:type;
-    rr:object foaf:Person;
+  rml:predicateObjectMap [
+    rml:predicate ex:id ;
+    rml:objectMap [ rml:reference "ID";  ]
+  ];
+
+  rml:predicateObjectMap [
+    rml:predicate foaf:name;
+    rml:objectMap [ rml:reference "FirstName" ]
   ].
+
+rml:DataFrame a rml:ReferenceFormulation;
+	kg4di:definedBy "Pandas".
```

### Comparing `morph_kgc-2.6.4/test/rml/xml/RMLTC0007a/test_RMLTC0007a_XML.py` & `morph_kgc-2.7.0/test/rml-core/xml/RMLTC0007a/test_RMLTC0007a_XML.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/rml/xml/RMLTC0007b/mapping.ttl` & `morph_kgc-2.7.0/test/rml-in-memory/json_dictionary/RMLIMTC0005a/mapping.ttl`

 * *Files 26% similar despite different names*

```diff
@@ -1,31 +1,36 @@
-@prefix rr: <http://www.w3.org/ns/r2rml#> .
 @prefix foaf: <http://xmlns.com/foaf/0.1/> .
 @prefix ex: <http://example.com/> .
 @prefix xsd: <http://www.w3.org/2001/XMLSchema#> .
-@prefix rml: <http://semweb.mmlab.be/ns/rml#> .
-@prefix ql: <http://semweb.mmlab.be/ns/ql#> .
-@prefix rdf: <http://www.w3.org/1999/02/22-rdf-syntax-ns#> .
+@prefix rml: <http://w3id.org/rml/> .
 @base <http://example.com/base/> .
+@prefix sd: <https://w3id.org/okn/o/sd#>.
+@prefix kg4di: <https://w3id.org/kg4di/definedBy>.
 
-<TriplesMap1> a rr:TriplesMap;
+<TriplesMap1> a rml:TriplesMap;
 
   rml:logicalSource [
-    rml:source "test/rml/xml/RMLTC0007b/student.xml";
-    rml:referenceFormulation ql:XPath;
-    rml:iterator "/students/student"
+    rml:source [
+			a sd:DatasetSpecification;
+			sd:name "variable1";
+			sd:hasDataTransformation [
+				sd:hasSourceCode [
+					sd:programmingLanguage "Python3.9";
+				];
+			];
+		];
+		rml:referenceFormulation rml:Dictionary;
+    rml:iterator "$.persons[*]"
   ];
 
-  rr:subjectMap [
-    rr:template "http://example.com/Student/{ID}/{FirstName}";
-    rr:graph ex:PersonGraph
+  rml:subjectMap [
+    rml:template "http://example.com/{fname};{lname}";
+    rml:class foaf:Person;
   ];
 
-  rr:predicateObjectMap [
-    rr:predicate rdf:type;
-    rr:object foaf:Person;
-  ];
-
-  rr:predicateObjectMap [
-    rr:predicate foaf:name;
-    rr:objectMap [ rml:reference "FirstName" ]
+  rml:predicateObjectMap [
+    rml:predicate ex:owes;
+    rml:objectMap [ rml:reference "amount"; ]
   ].
+
+rml:Dictionary a rml:ReferenceFormulation;
+	kg4di:definedBy "Python".
```

### Comparing `morph_kgc-2.6.4/test/rml/xml/RMLTC0007b/test_RMLTC0007b_XML.py` & `morph_kgc-2.7.0/test/rml-core/xml/RMLTC0007b/test_RMLTC0007b_XML.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/rml/xml/RMLTC0007c/mapping.ttl` & `morph_kgc-2.7.0/test/rml-core/xml/RMLTC0007c/mapping.ttl`

 * *Files 24% similar despite different names*

```diff
@@ -1,30 +1,28 @@
-@prefix rr: <http://www.w3.org/ns/r2rml#> .
 @prefix foaf: <http://xmlns.com/foaf/0.1/> .
 @prefix ex: <http://example.com/> .
 @prefix xsd: <http://www.w3.org/2001/XMLSchema#> .
-@prefix rml: <http://semweb.mmlab.be/ns/rml#> .
-@prefix ql: <http://semweb.mmlab.be/ns/ql#> .
+@prefix rml: <http://w3id.org/rml/> .
 @base <http://example.com/base/> .
 
-<TriplesMap1> a rr:TriplesMap;
+<TriplesMap1> a rml:TriplesMap;
 
   rml:logicalSource [
-    rml:source "test/rml/xml/RMLTC0007c/student.xml";
-    rml:referenceFormulation ql:XPath;
+    rml:source "test/rml-core/xml/RMLTC0007c/student.xml";
+    rml:referenceFormulation rml:XPath;
     rml:iterator "/students/student"
   ];
 
-  rr:subjectMap [
-    rr:template "http://example.com/Student/{ID}/{FirstName}";
-    rr:class foaf:Person, ex:Student
+  rml:subjectMap [
+    rml:template "http://example.com/Student/{ID}/{FirstName}";
+    rml:class foaf:Person, ex:Student
   ];
 
-  rr:predicateObjectMap [
-    rr:predicate ex:id ;
-    rr:objectMap [ rml:reference "ID";  ]
+  rml:predicateObjectMap [
+    rml:predicate ex:id ;
+    rml:objectMap [ rml:reference "ID";  ]
   ];
 
-  rr:predicateObjectMap [
-    rr:predicate foaf:name;
-    rr:objectMap [ rml:reference "FirstName" ]
+  rml:predicateObjectMap [
+    rml:predicate foaf:name;
+    rml:objectMap [ rml:reference "FirstName" ]
   ].
```

### Comparing `morph_kgc-2.6.4/test/rml/xml/RMLTC0007c/test_RMLTC0007c_XML.py` & `morph_kgc-2.7.0/test/rml-core/xml/RMLTC0007c/test_RMLTC0007c_XML.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/rml/xml/RMLTC0007d/mapping.ttl` & `morph_kgc-2.7.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0007d/mapping.ttl`

 * *Files 24% similar despite different names*

```diff
@@ -1,40 +1,51 @@
-@prefix rr: <http://www.w3.org/ns/r2rml#> .
 @prefix foaf: <http://xmlns.com/foaf/0.1/> .
 @prefix ex: <http://example.com/> .
 @prefix xsd: <http://www.w3.org/2001/XMLSchema#> .
-@prefix rml: <http://semweb.mmlab.be/ns/rml#> .
-@prefix ql: <http://semweb.mmlab.be/ns/ql#> .
+@prefix rml: <http://w3id.org/rml/> .
 @prefix rdf: <http://www.w3.org/1999/02/22-rdf-syntax-ns#> .
 @base <http://example.com/base/> .
+@prefix sd: <https://w3id.org/okn/o/sd#>.
+@prefix kg4di: <https://w3id.org/kg4di/definedBy>.
 
-<TriplesMap1> a rr:TriplesMap;
+<TriplesMap1> a rml:TriplesMap;
 
   rml:logicalSource [
-    rml:source "test/rml/xml/RMLTC0007d/student.xml";
-    rml:referenceFormulation ql:XPath;
-    rml:iterator "/students/student"
+    rml:source [
+			a sd:DatasetSpecification;
+			sd:name "variable1";
+			sd:hasDataTransformation [
+				sd:hasSoftwareRequirements "pandas>=1.1.0";
+				sd:hasSourceCode [
+					sd:programmingLanguage "Python3.9";
+				];
+			];
+		];
+    rml:referenceFormulation rml:DataFrame;
   ];
 
-  rr:subjectMap [
-    rr:template "http://example.com/Student/{ID}/{FirstName}"
+  rml:subjectMap [
+    rml:template "http://example.com/Student/{ID}/{FirstName}"
   ];
 
-  rr:predicateObjectMap [
-    rr:predicate rdf:type;
-    rr:object foaf:Person;
+  rml:predicateObjectMap [
+    rml:predicate rdf:type;
+    rml:object foaf:Person;
   ];
 
-  rr:predicateObjectMap [
-    rr:predicate rdf:type;
-    rr:object ex:Student;
+  rml:predicateObjectMap [
+    rml:predicate rdf:type;
+    rml:object ex:Student;
   ];
 
-  rr:predicateObjectMap [
-    rr:predicate ex:id;
-    rr:objectMap [rml:reference "ID"]
+  rml:predicateObjectMap [
+    rml:predicate ex:id;
+    rml:objectMap [ rml:reference "ID" ]
   ];
 
-  rr:predicateObjectMap [
-    rr:predicate foaf:name;
-    rr:objectMap [ rml:reference "FirstName" ]
+  rml:predicateObjectMap [
+    rml:predicate foaf:name;
+    rml:objectMap [ rml:reference "FirstName" ]
   ].
+
+rml:DataFrame a rml:ReferenceFormulation;
+	kg4di:definedBy "Pandas".
```

### Comparing `morph_kgc-2.6.4/test/rml/xml/RMLTC0007d/test_RMLTC0007d_XML.py` & `morph_kgc-2.7.0/test/rml-core/xml/RMLTC0007d/test_RMLTC0007d_XML.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/rml/xml/RMLTC0007e/mapping.ttl` & `morph_kgc-2.7.0/test/rml-tv/RMLTVTC0026a/mapping.ttl`

 * *Files 26% similar despite different names*

```diff
@@ -1,32 +1,19 @@
-@prefix rr: <http://www.w3.org/ns/r2rml#> .
-@prefix foaf: <http://xmlns.com/foaf/0.1/> .
 @prefix ex: <http://example.com/> .
-@prefix xsd: <http://www.w3.org/2001/XMLSchema#> .
-@prefix rml: <http://semweb.mmlab.be/ns/rml#> .
-@prefix ql: <http://semweb.mmlab.be/ns/ql#> .
-@base <http://example.com/base/> .
+@prefix rml: <http://w3id.org/rml/> .
 
-<TriplesMap1> a rr:TriplesMap;
+<TriplesMap1>
+    a rml:TriplesMap;
+ 	rml:logicalSource [
+                     rml:query """
+                       SELECT ID, UNNEST(COL::VARCHAR[]) AS COL
+                       FROM 'test/rml-tv/RMLTVTC0026a/mixed_content_list.csv'
+                       """
+                       ];
 
-  rml:logicalSource [
-    rml:source "test/rml/xml/RMLTC0007e/student.xml";
-    rml:referenceFormulation ql:XPath;
-    rml:iterator "/students/student"
-  ];
-
-  rr:subjectMap [
-    rr:template "http://example.com/Student/{ID}/{Name}";
-    rr:graph ex:PersonGraph ;
-    rr:class foaf:Person
-  ];
-
-  rr:predicateObjectMap [
-    rr:predicate ex:id ;
-    rr:objectMap [ rml:reference "ID"; ]
-  ];
-
-  rr:predicateObjectMap
+	rml:subjectMap [ rml:template "http://example.com/{ID}" ];
+	rml:predicateObjectMap
     [
-      rr:predicate		foaf:name ;
-      rr:objectMap		[ rml:reference "Name" ]
-    ].
+      rml:predicate		ex:col;
+      rml:objectMap		[ rml:reference "COL" ];
+    ];
+.
```

### Comparing `morph_kgc-2.6.4/test/rml/xml/RMLTC0007e/test_RMLTC0007e_XML.py` & `morph_kgc-2.7.0/test/rml-core/xml/RMLTC0007e/test_RMLTC0007e_XML.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/rml/xml/RMLTC0007f/mapping.ttl` & `morph_kgc-2.7.0/test/rml-in-memory/json_dictionary/RMLIMTC0012a/mapping.ttl`

 * *Files 22% similar despite different names*

```diff
@@ -1,36 +1,44 @@
-@prefix rr: <http://www.w3.org/ns/r2rml#> .
 @prefix foaf: <http://xmlns.com/foaf/0.1/> .
 @prefix ex: <http://example.com/> .
 @prefix xsd: <http://www.w3.org/2001/XMLSchema#> .
-@prefix rml: <http://semweb.mmlab.be/ns/rml#> .
-@prefix ql: <http://semweb.mmlab.be/ns/ql#> .
-@prefix rdf: <http://www.w3.org/1999/02/22-rdf-syntax-ns#> .
+@prefix rml: <http://w3id.org/rml/> .
+@prefix sd: <https://w3id.org/okn/o/sd#>.
+@prefix kg4di: <https://w3id.org/kg4di/definedBy>.
 @base <http://example.com/base/> .
 
-<TriplesMap1> a rr:TriplesMap;
+<TriplesMap1>
+  a rml:TriplesMap;
 
   rml:logicalSource [
-    rml:source "test/rml/xml/RMLTC0007f/student.xml";
-    rml:referenceFormulation ql:XPath;
-    rml:iterator "/students/student"
+    rml:source [
+			a sd:DatasetSpecification;
+			sd:name "variable1";
+			sd:hasDataTransformation [
+				sd:hasSourceCode [
+					sd:programmingLanguage "Python3.9";
+				];
+			];
+		];
+		rml:referenceFormulation rml:Dictionary;
+    rml:iterator "$.persons[*]"
   ];
 
-  rr:subjectMap [
-    rr:template "http://example.com/Student/{ID}/{FirstName}";
-    rr:graph ex:PersonGraph
-  ];
-
-  rr:predicateObjectMap [
-    rr:predicate rdf:type;
-    rr:object foaf:Person
-  ];
+  rml:subjectMap [ rml:template "{fname}{lname}{amount}"; rml:termType rml:BlankNode; ];
 
-  rr:predicateObjectMap [
-    rr:predicate ex:id ;
-    rr:objectMap [ rml:reference "ID";  ]
+  rml:predicateObjectMap [
+    rml:predicate foaf:name ;
+    rml:objectMap [
+      rml:template "{fname} {lname}";
+      rml:termType rml:Literal ;
+    ]
   ];
 
-  rr:predicateObjectMap [
-    rr:predicate foaf:name ;
-    rr:objectMap [ rml:reference "FirstName" ]
+  rml:predicateObjectMap [
+    rml:predicate ex:amount ;
+    rml:objectMap    [
+      rml:reference "amount";
+    ]
   ].
+
+rml:Dictionary a rml:ReferenceFormulation;
+	kg4di:definedBy "Python".
```

### Comparing `morph_kgc-2.6.4/test/rml/xml/RMLTC0007f/test_RMLTC0007f_XML.py` & `morph_kgc-2.7.0/test/rml-core/xml/RMLTC0007f/test_RMLTC0007f_XML.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/rml/xml/RMLTC0007g/mapping.ttl` & `morph_kgc-2.7.0/test/rml-fnml/udf/mapping.ttl`

 * *Files 21% similar despite different names*

```diff
@@ -1,27 +1,35 @@
-@prefix rr: <http://www.w3.org/ns/r2rml#> .
 @prefix foaf: <http://xmlns.com/foaf/0.1/> .
 @prefix ex: <http://example.com/> .
 @prefix xsd: <http://www.w3.org/2001/XMLSchema#> .
-@prefix rml: <http://semweb.mmlab.be/ns/rml#> .
-@prefix ql: <http://semweb.mmlab.be/ns/ql#> .
-@base <http://example.com/base/> .
-
-<TriplesMap1> a rr:TriplesMap;
+@prefix rml: <http://w3id.org/rml/> .
+@prefix fno: <https://w3id.org/function/ontology#> .
+@prefix morph-kgc: <https://github.com/morph-kgc/morph-kgc/function/built-in.ttl#> .
+@prefix grel: <http://users.ugent.be/~bjdmeest/function/grel.ttl#> .
+@prefix idlab-fn: <http://example.com/idlab/function/> .
 
-  rml:logicalSource [
-    rml:source "test/rml/xml/RMLTC0007g/student.xml";
-    rml:referenceFormulation ql:XPath;
-    rml:iterator "/students/student"
-  ];
+@base <http://example.com/base/> .
 
-  rr:subjectMap [
-    rr:template "http://example.com/Student/{ID}/{FirstName}";
-    rr:graph rr:defaultGraph
-  ];
+<TriplesMap1>
+    rml:logicalSource [
+        rml:source "test/rml-fnml/udf/student.csv";
+        rml:referenceFormulation rml:CSV
+    ];
+    rml:subjectMap [
+        rml:template "http://example.com/{Name}"
+    ];
+    rml:predicateObjectMap [
+        rml:predicate foaf:name;
+        rml:objectMap [
+            rml:functionExecution <#Execution> ;
+        ]
+    ] .
 
-  rr:predicateObjectMap [
-    rr:predicate foaf:name;
-    rr:objectMap [
-      rml:reference "FirstName"
-    ]
-  ].
+<#Execution>
+    rml:function ex:toUpperCase ;
+    rml:input
+        [
+            rml:parameter grel:valueParam ;
+            rml:inputValueMap [
+                rml:reference "Name" ;
+            ]
+        ] .
```

### Comparing `morph_kgc-2.6.4/test/rml/xml/RMLTC0007g/test_RMLTC0007g_XML.py` & `morph_kgc-2.7.0/test/rml-core/xml/RMLTC0007g/test_RMLTC0007g_XML.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/rml/xml/RMLTC0007h/mapping.ttl` & `morph_kgc-2.7.0/test/rml-core/json/RMLTC0010a/mapping.ttl`

 * *Files 15% similar despite different names*

```diff
@@ -1,27 +1,22 @@
-@prefix rr: <http://www.w3.org/ns/r2rml#> .
 @prefix foaf: <http://xmlns.com/foaf/0.1/> .
 @prefix ex: <http://example.com/> .
 @prefix xsd: <http://www.w3.org/2001/XMLSchema#> .
-@prefix rml: <http://semweb.mmlab.be/ns/rml#> .
-@prefix ql: <http://semweb.mmlab.be/ns/ql#> .
+@prefix rml: <http://w3id.org/rml/> .
+@prefix activity: <http://example.com/activity/> .
 @base <http://example.com/base/> .
 
-<TriplesMap1> a rr:TriplesMap;
+<TriplesMap1>
+  a rml:TriplesMap;
 
   rml:logicalSource [
-    rml:source "test/rml/xml/RMLTC0007h/student.xml";
-    rml:referenceFormulation ql:XPath;
-    rml:iterator "/students/student"
+    rml:source "test/rml-core/json/RMLTC0010a/country_info.json";
+    rml:referenceFormulation rml:JSONPath;
+    rml:iterator "$.countries[*]"
   ];
 
-  rr:subjectMap [
-    rr:template "http://example.com/Student/{ID}/{FirstName}";
-    rr:graphMap [ rml:reference "FirstName"; rr:termType rr:Literal; ]
-  ];
+  rml:subjectMap [ rml:template "http://example.com/{Country Code}" ];
 
-  rr:predicateObjectMap [
-    rr:predicate foaf:name;
-    rr:objectMap [
-      rml:reference "FirstName"
-    ]
-  ].
+  rml:predicateObjectMap [
+    rml:predicate ex:name ;
+    rml:objectMap [ rml:reference "Name" ]
+  ] .
```

### Comparing `morph_kgc-2.6.4/test/rml/xml/RMLTC0007h/test_RMLTC0007h_XML.py` & `morph_kgc-2.7.0/test/rml-core/xml/RMLTC0007h/test_RMLTC0007h_XML.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/rml/xml/RMLTC0008a/mapping.ttl` & `morph_kgc-2.7.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0012d/mapping.ttl`

 * *Files 22% similar despite different names*

```diff
@@ -1,42 +1,46 @@
-@prefix rr: <http://www.w3.org/ns/r2rml#> .
 @prefix foaf: <http://xmlns.com/foaf/0.1/> .
 @prefix ex: <http://example.com/> .
 @prefix xsd: <http://www.w3.org/2001/XMLSchema#> .
-@prefix rml: <http://semweb.mmlab.be/ns/rml#> .
-@prefix ql: <http://semweb.mmlab.be/ns/ql#> .
-@prefix rdf: <http://www.w3.org/1999/02/22-rdf-syntax-ns#> .
+@prefix rml: <http://w3id.org/rml/> .
+@prefix sd: <https://w3id.org/okn/o/sd#>.
+@prefix kg4di: <https://w3id.org/kg4di/definedBy>.
 @base <http://example.com/base/> .
 
 <TriplesMap1>
-  a rr:TriplesMap;
+  a rml:TriplesMap;
 
   rml:logicalSource [
-    rml:source "test/rml/xml/RMLTC0008a/student.xml";
-    rml:referenceFormulation ql:XPath;
-    rml:iterator "/students/student"
+    rml:source [
+			a sd:DatasetSpecification;
+			sd:name "variable1";
+			sd:hasDataTransformation [
+				sd:hasSoftwareRequirements "pandas>=1.1.0";
+				sd:hasSourceCode [
+					sd:programmingLanguage "Python3.9";
+				];
+			];
+		];
+    rml:referenceFormulation rml:DataFrame;
   ];
 
-  rr:subjectMap [
-    rr:template "http://example.com/Student/{ID}/{Name}";
-    rr:graphMap [ rr:template "http://example.com/graph/Student/{ID}/{Name}" ]
-  ];
+  rml:subjectMap [ rml:template "{fname}_{lname}_{amount}"; rml:termType rml:BlankNode; ];
 
-  rr:predicateObjectMap [
-    rr:predicate rdf:type ;
-    rr:object foaf:Person;
-  ];
+  rml:subjectMap [ rml:template "{amount}_{fname}_{lname}"; rml:termType rml:BlankNode; ];
 
-  rr:predicateObjectMap [
-    rr:predicate ex:id ;
-    rr:objectMap [ rml:reference "ID" ]
+  rml:predicateObjectMap [
+    rml:predicate foaf:name ;
+    rml:objectMap [
+      rml:template "{fname} {lname}";
+      rml:termType rml:Literal ;
+    ]
   ];
 
-  rr:predicateObjectMap [
-    rr:predicate foaf:name ;
-    rr:objectMap [ rml:reference "Name" ]
-  ];
+  rml:predicateObjectMap [
+    rml:predicate ex:amount ;
+    rml:objectMap    [
+      rml:reference "amount";
+    ]
+  ].
 
-  rr:predicateObjectMap [
-    rr:predicate ex:Sport ;
-    rr:objectMap [ rml:reference "Sport" ]
-  ] .
+rml:DataFrame a rml:ReferenceFormulation;
+	kg4di:definedBy "Pandas".
```

### Comparing `morph_kgc-2.6.4/test/rml/xml/RMLTC0008a/output.nq` & `morph_kgc-2.7.0/test/rml-core/xml/RMLTC0008a/output.nq`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/rml/xml/RMLTC0008a/test_RMLTC0008a_XML.py` & `morph_kgc-2.7.0/test/rml-core/xml/RMLTC0008a/test_RMLTC0008a_XML.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/rml/xml/RMLTC0008b/output.nq` & `morph_kgc-2.7.0/test/rml-core/xml/RMLTC0008b/output.nq`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/rml/xml/RMLTC0008b/test_RMLTC0008b_XML.py` & `morph_kgc-2.7.0/test/rml-core/xml/RMLTC0008b/test_RMLTC0008b_XML.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/rml/xml/RMLTC0008c/mapping.ttl` & `morph_kgc-2.7.0/test/rml-core/json/RMLTC0007e/mapping.ttl`

 * *Files 14% similar despite different names*

```diff
@@ -1,25 +1,29 @@
-@prefix rr: <http://www.w3.org/ns/r2rml#> .
 @prefix foaf: <http://xmlns.com/foaf/0.1/> .
 @prefix ex: <http://example.com/> .
 @prefix xsd: <http://www.w3.org/2001/XMLSchema#> .
-@prefix rml: <http://semweb.mmlab.be/ns/rml#> .
-@prefix ql: <http://semweb.mmlab.be/ns/ql#> .
-@prefix activity: <http://example.com/activity/> .
+@prefix rml: <http://w3id.org/rml/> .
 @base <http://example.com/base/> .
 
-<TriplesMap1>
-  a rr:TriplesMap;
+<TriplesMap1> a rml:TriplesMap;
 
   rml:logicalSource [
-    rml:source "test/rml/xml/RMLTC0008c/student.xml";
-    rml:referenceFormulation ql:XPath;
-    rml:iterator "/students/student"
+    rml:source "test/rml-core/json/RMLTC0007e/student.json";
+    rml:referenceFormulation rml:JSONPath;
+    rml:iterator "$.students[*]"
   ];
 
-  rr:subjectMap [ rr:template "http://example.com/Student/{ID}/{Name}" ];
+  rml:subjectMap [
+    rml:template "http://example.com/Student/{ID}/{Name}";
+    rml:graph ex:PersonGraph ;
+    rml:class foaf:Person
+  ];
+
+  rml:predicateObjectMap [
+    rml:predicate ex:id ;
+    rml:objectMap [ rml:reference "ID"; ]
+  ];
 
-  rr:predicateObjectMap [
-    rr:predicate foaf:name ;
-    rr:predicate ex:name ;
-    rr:objectMap [ rml:reference "Name" ]
-  ] .
+  rml:predicateObjectMap [
+    rml:predicate foaf:name ;
+    rml:objectMap [ rml:reference "Name" ]
+  ].
```

### Comparing `morph_kgc-2.6.4/test/rml/xml/RMLTC0008c/test_RMLTC0008c_XML.py` & `morph_kgc-2.7.0/test/rml-core/xml/RMLTC0008c/test_RMLTC0008c_XML.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/rml/xml/RMLTC0009a/mapping.ttl` & `morph_kgc-2.7.0/test/rml-fnml/RMLFNOTC0001-CSV/mapping.ttl`

 * *Files 20% similar despite different names*

```diff
@@ -1,53 +1,35 @@
-@prefix rr: <http://www.w3.org/ns/r2rml#> .
 @prefix foaf: <http://xmlns.com/foaf/0.1/> .
 @prefix ex: <http://example.com/> .
 @prefix xsd: <http://www.w3.org/2001/XMLSchema#> .
-@prefix rml: <http://semweb.mmlab.be/ns/rml#> .
-@prefix ql: <http://semweb.mmlab.be/ns/ql#> .
-@prefix activity: <http://example.com/activity/> .
-@prefix rdfs: <http://www.w3.org/2000/01/rdf-schema#> .
+@prefix rml: <http://w3id.org/rml/> .
+@prefix fno: <https://w3id.org/function/ontology#> .
+@prefix morph-kgc: <https://github.com/morph-kgc/morph-kgc/function/built-in.ttl#> .
+@prefix grel: <http://users.ugent.be/~bjdmeest/function/grel.ttl#> .
+@prefix idlab-fn: <http://example.com/idlab/function/> .
+
 @base <http://example.com/base/> .
 
 <TriplesMap1>
-  a rr:TriplesMap;
-
-  rml:logicalSource [
-    rml:source "test/rml/xml/RMLTC0009a/student.xml";
-    rml:referenceFormulation ql:XPath;
-    rml:iterator "/students/student"
-  ];
-
-  rr:subjectMap [ rr:template "http://example.com/resource/student_{ID}" ];
-
-  rr:predicateObjectMap [
-    rr:predicate foaf:name ;
-    rr:objectMap [ rml:reference "Name" ]
-  ] ;
-
-  rr:predicateObjectMap [
-    rr:predicate <http://example.com/ontology/practises> ;
-    rr:objectMap [
-      a rr:RefObjectMap ;
-      rr:parentTriplesMap <TriplesMap2>;
-      rr:joinCondition [
-        rr:child "Sport" ;
-        rr:parent "ID" ;
-      ]
-    ]
-  ] .
-
-<TriplesMap2>
-  a rr:TriplesMap;
-
-  rml:logicalSource [
-    rml:source "test/rml/xml/RMLTC0009a/sport.xml";
-    rml:referenceFormulation ql:XPath;
-    rml:iterator "/sports/sport"
-  ];
-
-  rr:subjectMap [ rr:template "http://example.com/resource/sport_{ID}" ];
-
-  rr:predicateObjectMap [
-    rr:predicate rdfs:label ;
-    rr:objectMap [ rml:reference "Name" ];
-  ].
+    rml:logicalSource [
+        rml:source "test/rml-fnml/RMLFNOTC0001-CSV/student.csv";
+        rml:referenceFormulation rml:CSV
+    ];
+    rml:subjectMap [
+        rml:template "http://example.com/{Name}"
+    ];
+    rml:predicateObjectMap [
+        rml:predicate foaf:name;
+        rml:objectMap [
+            rml:functionExecution <#Execution> ;
+        ]
+    ] .
+
+<#Execution>
+    rml:function grel:toUpperCase ;
+    rml:input
+        [
+            rml:parameter grel:valueParam ;
+            rml:inputValueMap [
+                rml:reference "Name" ;
+            ]
+        ] .
```

### Comparing `morph_kgc-2.6.4/test/rml/xml/RMLTC0009a/test_RMLTC0009a_XML.py` & `morph_kgc-2.7.0/test/rml-core/xml/RMLTC0009a/test_RMLTC0009a_XML.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/rml/xml/RMLTC0009b/output.nq` & `morph_kgc-2.7.0/test/rml-core/xml/RMLTC0009b/output.nq`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/rml/xml/RMLTC0009b/test_RMLTC0009b_XML.py` & `morph_kgc-2.7.0/test/rml-core/xml/RMLTC0009b/test_RMLTC0009b_XML.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/rml/xml/RMLTC0010b/mapping.ttl` & `morph_kgc-2.7.0/test/rml-core/xml/RMLTC0007f/mapping.ttl`

 * *Files 18% similar despite different names*

```diff
@@ -1,24 +1,34 @@
-@prefix rr: <http://www.w3.org/ns/r2rml#> .
 @prefix foaf: <http://xmlns.com/foaf/0.1/> .
 @prefix ex: <http://example.com/> .
 @prefix xsd: <http://www.w3.org/2001/XMLSchema#> .
-@prefix rml: <http://semweb.mmlab.be/ns/rml#> .
-@prefix ql: <http://semweb.mmlab.be/ns/ql#> .
-@prefix activity: <http://example.com/activity/> .
+@prefix rml: <http://w3id.org/rml/> .
+@prefix rdf: <http://www.w3.org/1999/02/22-rdf-syntax-ns#> .
 @base <http://example.com/base/> .
 
-<TriplesMap1>
-  a rr:TriplesMap;
+<TriplesMap1> a rml:TriplesMap;
 
   rml:logicalSource [
-    rml:source "test/rml/xml/RMLTC0010b/country_info.xml";
-    rml:referenceFormulation ql:XPath;
-    rml:iterator "/countries/country"
+    rml:source "test/rml-core/xml/RMLTC0007f/student.xml";
+    rml:referenceFormulation rml:XPath;
+    rml:iterator "/students/student"
   ];
 
-  rr:subjectMap [ rr:template "http://example.com/{CountryCode}/{Name}" ];
+  rml:subjectMap [
+    rml:template "http://example.com/Student/{ID}/{FirstName}";
+    rml:graph ex:PersonGraph
+  ];
+
+  rml:predicateObjectMap [
+    rml:predicate rdf:type;
+    rml:object foaf:Person
+  ];
+
+  rml:predicateObjectMap [
+    rml:predicate ex:id ;
+    rml:objectMap [ rml:reference "ID";  ]
+  ];
 
-  rr:predicateObjectMap [
-    rr:predicate ex:name ;
-    rr:objectMap [ rml:reference "Name" ]
-  ] .
+  rml:predicateObjectMap [
+    rml:predicate foaf:name ;
+    rml:objectMap [ rml:reference "FirstName" ]
+  ].
```

### Comparing `morph_kgc-2.6.4/test/rml/xml/RMLTC0010b/test_RMLTC0010b_XML.py` & `morph_kgc-2.7.0/test/rml-core/xml/RMLTC0010b/test_RMLTC0010b_XML.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/rml/xml/RMLTC0010c/mapping.ttl` & `morph_kgc-2.7.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0001b/mapping.ttl`

 * *Files 26% similar despite different names*

```diff
@@ -1,24 +1,39 @@
-@prefix rr: <http://www.w3.org/ns/r2rml#> .
 @prefix foaf: <http://xmlns.com/foaf/0.1/> .
 @prefix ex: <http://example.com/> .
 @prefix xsd: <http://www.w3.org/2001/XMLSchema#> .
-@prefix rml: <http://semweb.mmlab.be/ns/rml#> .
-@prefix ql: <http://semweb.mmlab.be/ns/ql#> .
-@prefix activity: <http://example.com/activity/> .
+@prefix rml: <http://w3id.org/rml/> .
 @base <http://example.com/base/> .
+@prefix sd: <https://w3id.org/okn/o/sd#>.
+@prefix kg4di: <https://w3id.org/kg4di/definedBy>.
 
 <TriplesMap1>
-  a rr:TriplesMap;
+  a rml:TriplesMap;
 
   rml:logicalSource [
-    rml:source "test/rml/xml/RMLTC0010c/country_info.xml";
-    rml:referenceFormulation ql:XPath;
-    rml:iterator "/countries/country"
+    rml:source [
+			a sd:DatasetSpecification;
+			sd:name "variable1";
+			sd:hasDataTransformation [
+				sd:hasSoftwareRequirements "pandas>=1.1.0";
+				sd:hasSourceCode [
+					sd:programmingLanguage "Python3.9";
+				];
+			];
+		];
+    rml:referenceFormulation rml:DataFrame;
   ];
 
-  rr:subjectMap [ rr:template "http://example.com/{CountryCode}/{Name}" ];
+  rml:subjectMap [
+    rml:template "{Name}";
+    rml:termType rml:BlankNode
+  ];
+
+  rml:predicateObjectMap [
+    rml:predicate foaf:name;
+    rml:objectMap [
+      rml:reference "Name"
+    ]
+  ].
 
-  rr:predicateObjectMap [
-    rr:predicate ex:code ;
-    rr:objectMap [ rr:template "\\{\\{\\{ {ISO3166} \\}\\}\\}"; rr:termType rr:Literal]
-  ] .
+rml:DataFrame a rml:ReferenceFormulation;
+	kg4di:definedBy "Pandas".
```

### Comparing `morph_kgc-2.6.4/test/rml/xml/RMLTC0010c/test_RMLTC0010c_XML.py` & `morph_kgc-2.7.0/test/rml-core/xml/RMLTC0010c/test_RMLTC0010c_XML.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/rml/xml/RMLTC0011b/mapping.ttl` & `morph_kgc-2.7.0/test/rml-fnml/array_get_slice/mapping.ttl`

 * *Files 22% similar despite different names*

```diff
@@ -1,82 +1,59 @@
-@prefix rr: <http://www.w3.org/ns/r2rml#> .
 @prefix foaf: <http://xmlns.com/foaf/0.1/> .
 @prefix ex: <http://example.com/> .
 @prefix xsd: <http://www.w3.org/2001/XMLSchema#> .
-@prefix rml: <http://semweb.mmlab.be/ns/rml#> .
-@prefix ql: <http://semweb.mmlab.be/ns/ql#> .
+@prefix rml: <http://w3id.org/rml/> .
+@prefix fno: <https://w3id.org/function/ontology#> .
+@prefix morph-kgc: <https://github.com/morph-kgc/morph-kgc/function/built-in.ttl#> .
+@prefix grel: <http://users.ugent.be/~bjdmeest/function/grel.ttl#> .
+@prefix idlab-fn: <http://example.com/idlab/function/> .
 
 @base <http://example.com/base/> .
 
 <TriplesMap1>
-  a rr:TriplesMap;
-
-  rml:logicalSource [
-    rml:source "test/rml/xml/RMLTC0011b/student.xml";
-    rml:referenceFormulation ql:XPath;
-    rml:iterator "/Students/Student"
-  ];
-
-  rr:subjectMap [
-    rr:template "http://example.com/student/{ID}";
-  ];
-
-  rr:predicateObjectMap [
-    rr:predicate ex:firstName;
-    rr:objectMap [
-      rml:reference "FirstName"
-    ]
-  ];
-
-  rr:predicateObjectMap [
-    rr:predicate ex:lastName;
-    rr:objectMap [
-      rml:reference "LastName"
-    ]
-  ].
-
-<TriplesMap2>
-  a rr:TriplesMap;
-
-  rml:logicalSource [
-    rml:source "test/rml/xml/RMLTC0011b/sport.xml";
-    rml:referenceFormulation ql:XPath;
-    rml:iterator "/Sports/Sport"
-  ];
-
-  rr:subjectMap [
-    rr:template "http://example.com/sport/{ID}";
-  ];
-
-  rr:predicateObjectMap [
-    rr:predicate ex:id;
-    rr:objectMap [
-      rml:reference "ID"
-    ]
-  ];
-
-  rr:predicateObjectMap [
-    rr:predicate ex:description;
-    rr:objectMap [
-      rml:reference "Description"
-    ]
-  ].
-
-<LinkMap_1_2>
-  a rr:TriplesMap;
-
-  rml:logicalSource [
-    rml:source "test/rml/xml/RMLTC0011b/student_sport.xml";
-    rml:referenceFormulation ql:XPath;
-    rml:iterator "/links/link"
-  ];
-
-  rr:subjectMap [
-    rr:template "http://example.com/student/{ID_Student}";
-  ];
-
-  rr:predicateObjectMap [
-    rr:predicate ex:plays;
-    rr:objectMap [
-      rr:template "http://example.com/sport/{ID_Sport}"
-    ]
-  ].
+    rml:logicalSource [
+        rml:source "test/rml-fnml/array_get_slice/article.tsv" ;
+        rml:referenceFormulation rml:CSV ;
+    ];
+    rml:subjectMap [
+        rml:template "http://example.com/articles/{title}"
+    ];
+    rml:predicateObjectMap [
+        rml:predicate ex:firstAuthor;
+        rml:objectMap [
+            rml:functionExecution <#Execution1> ;
+        ]
+    ];
+    rml:predicateObjectMap [
+        rml:predicate ex:otherAuthors;
+        rml:objectMap [
+            rml:functionExecution <#Execution2> ;
+        ]
+    ].
+
+<#Execution1>
+    rml:function grel:array_get ;
+    rml:input
+        [
+            rml:parameter grel:param_a ;
+            rml:inputValueMap [
+                rml:reference "authors"
+            ]
+        ] ,
+        [
+            rml:parameter grel:p_int_i_from ;
+            rml:inputValue "0"
+        ] .
+
+<#Execution2>
+    rml:function grel:array_slice ;
+    rml:input
+        [
+            rml:parameter grel:param_a ;
+            rml:inputValueMap [
+                rml:reference "authors"
+            ]
+        ] ,
+        [
+            rml:parameter grel:p_int_i_from ;
+            rml:inputValue "1"
+        ] .
```

### Comparing `morph_kgc-2.6.4/test/rml/xml/RMLTC0011b/output.nq` & `morph_kgc-2.7.0/test/rml-core/xml/RMLTC0011b/output.nq`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/rml/xml/RMLTC0011b/test_RMLTC0011b_XML.py` & `morph_kgc-2.7.0/test/rml-core/xml/RMLTC0011b/test_RMLTC0011b_XML.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/rml/xml/RMLTC0012a/mapping.ttl` & `morph_kgc-2.7.0/test/rml-in-memory/json_dictionary/RMLIMTC0012c/mapping.ttl`

 * *Files 20% similar despite different names*

```diff
@@ -1,34 +1,42 @@
-@prefix rr: <http://www.w3.org/ns/r2rml#> .
 @prefix foaf: <http://xmlns.com/foaf/0.1/> .
 @prefix ex: <http://example.com/> .
 @prefix xsd: <http://www.w3.org/2001/XMLSchema#> .
-@prefix rml: <http://semweb.mmlab.be/ns/rml#> .
-@prefix ql: <http://semweb.mmlab.be/ns/ql#> .
-
+@prefix rml: <http://w3id.org/rml/> .
+@prefix sd: <https://w3id.org/okn/o/sd#>.
+@prefix kg4di: <https://w3id.org/kg4di/definedBy>.
 @base <http://example.com/base/> .
 
 <TriplesMap1>
-  a rr:TriplesMap;
+  a rml:TriplesMap;
 
   rml:logicalSource [
-    rml:source "test/rml/xml/RMLTC0012a/persons.xml";
-    rml:referenceFormulation ql:XPath;
-    rml:iterator "/Persons/Person"
+    rml:source [
+			a sd:DatasetSpecification;
+			sd:name "variable1";
+			sd:hasDataTransformation [
+				sd:hasSourceCode [
+					sd:programmingLanguage "Python3.9";
+				];
+			];
+		];
+		rml:referenceFormulation rml:Dictionary;
+    rml:iterator "$.persons[*]"
   ];
 
-  rr:subjectMap [ rr:template "{fname}{lname}{amount}"; rr:termType rr:BlankNode; ];
-
-  rr:predicateObjectMap [
-    rr:predicate foaf:name ;
-    rr:objectMap [
-      rr:template "{fname} {lname}";
-      rr:termType rr:Literal ;
+  rml:predicateObjectMap [
+    rml:predicate foaf:name ;
+    rml:objectMap [
+      rml:template "{fname} {lname}";
+      rml:termType rml:Literal ;
     ]
   ];
 
-  rr:predicateObjectMap [
-    rr:predicate ex:amount ;
-    rr:objectMap    [
+  rml:predicateObjectMap [
+    rml:predicate ex:amount ;
+    rml:objectMap    [
       rml:reference "amount";
     ]
   ].
+
+rml:Dictionary a rml:ReferenceFormulation;
+	kg4di:definedBy "Python".
```

### Comparing `morph_kgc-2.6.4/test/rml/xml/RMLTC0012a/test_RMLTC0012a_XML.py` & `morph_kgc-2.7.0/test/rml-core/xml/RMLTC0012a/test_RMLTC0012a_XML.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/rml/xml/RMLTC0012b/test_RMLTC0012b_XML.py` & `morph_kgc-2.7.0/test/rml-core/xml/RMLTC0012b/test_RMLTC0012b_XML.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/rml/xml/RMLTC0012c/mapping.ttl` & `morph_kgc-2.7.0/test/rml-fnml/RMLFNOTC0000-CSV/mapping.ttl`

 * *Files 24% similar despite different names*

```diff
@@ -1,32 +1,28 @@
-@prefix rr: <http://www.w3.org/ns/r2rml#> .
 @prefix foaf: <http://xmlns.com/foaf/0.1/> .
 @prefix ex: <http://example.com/> .
 @prefix xsd: <http://www.w3.org/2001/XMLSchema#> .
-@prefix rml: <http://semweb.mmlab.be/ns/rml#> .
-@prefix ql: <http://semweb.mmlab.be/ns/ql#> .
+@prefix rml: <http://w3id.org/rml/> .
+@prefix fno: <https://w3id.org/function/ontology#> .
+@prefix morph-kgc: <https://github.com/morph-kgc/morph-kgc/function/built-in.ttl#> .
+@prefix grel: <http://users.ugent.be/~bjdmeest/function/grel.ttl#> .
+@prefix idlab-fn: <http://example.com/idlab/function/> .
 
 @base <http://example.com/base/> .
 
 <TriplesMap1>
-  a rr:TriplesMap;
+    rml:logicalSource [
+        rml:source "test/rml-fnml/RMLFNOTC0000-CSV/student.csv";
+        rml:referenceFormulation rml:CSV
+    ];
+    rml:subjectMap [
+        rml:template "http://example.com/{Name}"
+    ];
+    rml:predicateObjectMap [
+        rml:predicate foaf:name;
+        rml:objectMap [
+            rml:functionExecution <#Execution> ;
+        ]
+    ] .
 
-  rml:logicalSource [
-    rml:source "test/rml/xml/RMLTC0012c/persons.xml";
-    rml:referenceFormulation ql:XPath;
-    rml:iterator "/Persons/Person"
-  ];
-
-  rr:predicateObjectMap [
-    rr:predicate foaf:name ;
-    rr:objectMap [
-      rr:template "{fname} {lname}";
-      rr:termType rr:Literal ;
-    ]
-  ];
-
-  rr:predicateObjectMap [
-    rr:predicate ex:amount ;
-    rr:objectMap    [
-      rml:reference "amount";
-    ]
-  ].
+<#Execution>
+    rml:function morph-kgc:uuid .
```

### Comparing `morph_kgc-2.6.4/test/rml/xml/RMLTC0012c/test_RMLTC0012c_XML.py` & `morph_kgc-2.7.0/test/rml-core/xml/RMLTC0012c/test_RMLTC0012c_XML.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/rml/xml/RMLTC0012d/mapping.ttl` & `morph_kgc-2.7.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0012c/mapping.ttl`

 * *Files 23% similar despite different names*

```diff
@@ -1,36 +1,42 @@
-@prefix rr: <http://www.w3.org/ns/r2rml#> .
 @prefix foaf: <http://xmlns.com/foaf/0.1/> .
 @prefix ex: <http://example.com/> .
 @prefix xsd: <http://www.w3.org/2001/XMLSchema#> .
-@prefix rml: <http://semweb.mmlab.be/ns/rml#> .
-@prefix ql: <http://semweb.mmlab.be/ns/ql#> .
-
+@prefix rml: <http://w3id.org/rml/> .
+@prefix sd: <https://w3id.org/okn/o/sd#>.
+@prefix kg4di: <https://w3id.org/kg4di/definedBy>.
 @base <http://example.com/base/> .
 
 <TriplesMap1>
-  a rr:TriplesMap;
+  a rml:TriplesMap;
 
   rml:logicalSource [
-    rml:source "test/rml/xml/RMLTC0012d/persons.xml";
-    rml:referenceFormulation ql:XPath;
-    rml:iterator "/Persons/Person"
+    rml:source [
+			a sd:DatasetSpecification;
+			sd:name "variable1";
+			sd:hasDataTransformation [
+				sd:hasSoftwareRequirements "pandas>=1.1.0";
+				sd:hasSourceCode [
+					sd:programmingLanguage "Python3.9";
+				];
+			];
+		];
+    rml:referenceFormulation rml:DataFrame;
   ];
 
-  rr:subjectMap [ rr:template "{fname}_{lname}_{amount}"; rr:termType rr:BlankNode; ];
-
-  rr:subjectMap [ rr:template "{amount}_{fname}_{lname}"; rr:termType rr:BlankNode; ];
-
-  rr:predicateObjectMap [
-    rr:predicate foaf:name ;
-    rr:objectMap [
-      rr:template "{fname} {lname}";
-      rr:termType rr:Literal ;
+  rml:predicateObjectMap [
+    rml:predicate foaf:name ;
+    rml:objectMap [
+      rml:template "{fname} {lname}";
+      rml:termType rml:Literal ;
     ]
   ];
 
-  rr:predicateObjectMap [
-    rr:predicate ex:amount ;
-    rr:objectMap    [
+  rml:predicateObjectMap [
+    rml:predicate ex:amount ;
+    rml:objectMap    [
       rml:reference "amount";
     ]
   ].
+
+rml:DataFrame a rml:ReferenceFormulation;
+	kg4di:definedBy "Pandas".
```

### Comparing `morph_kgc-2.6.4/test/rml/xml/RMLTC0012d/test_RMLTC0012d_XML.py` & `morph_kgc-2.7.0/test/rml-core/xml/RMLTC0012d/test_RMLTC0012d_XML.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/rml/xml/RMLTC0015a/mapping.ttl` & `morph_kgc-2.7.0/test/rml-core/csv/RMLTC0007d/mapping.ttl`

 * *Files 22% similar despite different names*

```diff
@@ -1,50 +1,37 @@
-@prefix rr: <http://www.w3.org/ns/r2rml#> .
 @prefix foaf: <http://xmlns.com/foaf/0.1/> .
 @prefix ex: <http://example.com/> .
 @prefix xsd: <http://www.w3.org/2001/XMLSchema#> .
-@prefix rml: <http://semweb.mmlab.be/ns/rml#> .
-@prefix ql: <http://semweb.mmlab.be/ns/ql#> .
-@prefix rdfs: <http://www.w3.org/2000/01/rdf-schema#> .
+@prefix rml: <http://w3id.org/rml/> .
+@prefix rdf: <http://www.w3.org/1999/02/22-rdf-syntax-ns#> .
 @base <http://example.com/base/> .
 
-<TriplesMap1>
-  a rr:TriplesMap;
+<TriplesMap1> a rml:TriplesMap;
 
   rml:logicalSource [
-    rml:source "test/rml/xml/RMLTC0015a/country_en.xml";
-    rml:referenceFormulation ql:XPath;
-    rml:iterator "/countries/country"
+    rml:source "test/rml-core/csv/RMLTC0007d/student.csv";
+    rml:referenceFormulation rml:CSV
   ];
 
-  rr:subjectMap [
-    rr:template "http://example.com/{Code}"
+  rml:subjectMap [
+    rml:template "http://example.com/Student/{ID}/{FirstName}"
   ];
 
-  rr:predicateObjectMap [
-    rr:predicate rdfs:label ;
-    rr:objectMap [
-      rml:reference "Name";
-      rr:language "en"
-    ]
-  ].
-
-<TriplesMap2>
-  a rr:TriplesMap;
+  rml:predicateObjectMap [
+    rml:predicate rdf:type;
+    rml:object foaf:Person;
+  ];
 
-  rml:logicalSource [
-    rml:source "test/rml/xml/RMLTC0015a/country_es.xml";
-    rml:referenceFormulation ql:XPath;
-    rml:iterator "/countries/country"
+  rml:predicateObjectMap [
+    rml:predicate rdf:type;
+    rml:object ex:Student;
   ];
 
-  rr:subjectMap [
-    rr:template "http://example.com/{Code}"
+  rml:predicateObjectMap [
+    rml:predicate ex:id;
+    rml:objectMap [ rml:reference "ID" ]
   ];
 
-  rr:predicateObjectMap [
-    rr:predicate rdfs:label ;
-    rr:objectMap [
-      rml:reference "Name";
-      rr:language "es"
-    ]
+  rml:predicateObjectMap [
+    rml:predicate foaf:name;
+    rml:objectMap [ rml:reference "FirstName" ]
   ].
```

### Comparing `morph_kgc-2.6.4/test/rml/xml/RMLTC0015a/test_RMLTC0015a_XML.py` & `morph_kgc-2.7.0/test/rml-core/xml/RMLTC0015a/test_RMLTC0015a_XML.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/rml/xml/RMLTC0015b/mapping.ttl` & `morph_kgc-2.7.0/test/rml-core/xml/RMLTC0015a/mapping.ttl`

 * *Files 16% similar despite different names*

```diff
@@ -1,47 +1,48 @@
-@prefix rr: <http://www.w3.org/ns/r2rml#> .
 @prefix foaf: <http://xmlns.com/foaf/0.1/> .
-@prefix rdfs: <http://www.w3.org/2000/01/rdf-schema#> .
 @prefix ex: <http://example.com/> .
 @prefix xsd: <http://www.w3.org/2001/XMLSchema#> .
-@prefix rml: <http://semweb.mmlab.be/ns/rml#> .
-@prefix ql: <http://semweb.mmlab.be/ns/ql#> .
-
+@prefix rml: <http://w3id.org/rml/> .
+@prefix rdfs: <http://www.w3.org/2000/01/rdf-schema#> .
 @base <http://example.com/base/> .
 
 <TriplesMap1>
-  a rr:TriplesMap;
+  a rml:TriplesMap;
 
   rml:logicalSource [
-    rml:source "test/rml/xml/RMLTC0015b/country_en.xml";
-    rml:referenceFormulation ql:XPath;
+    rml:source "test/rml-core/xml/RMLTC0015a/country_en.xml";
+    rml:referenceFormulation rml:XPath;
     rml:iterator "/countries/country"
   ];
 
-  rr:subjectMap [ rr:template "http://example.com/{Code}" ];
+  rml:subjectMap [
+    rml:template "http://example.com/{Code}"
+  ];
 
-  rr:predicateObjectMap [
-    rr:predicate rdfs:label;
-    rr:objectMap [
+  rml:predicateObjectMap [
+    rml:predicate rdfs:label ;
+    rml:objectMap [
       rml:reference "Name";
-      rr:language "english"
+      rml:language "en"
     ]
-  ] .
+  ].
 
 <TriplesMap2>
-  a rr:TriplesMap;
+  a rml:TriplesMap;
 
   rml:logicalSource [
-    rml:source "test/rml/xml/RMLTC0015b/country_es.xml";
-    rml:referenceFormulation ql:XPath;
+    rml:source "test/rml-core/xml/RMLTC0015a/country_es.xml";
+    rml:referenceFormulation rml:XPath;
     rml:iterator "/countries/country"
   ];
 
-  rr:subjectMap [ rr:template "http://example.com/{Code}" ];
+  rml:subjectMap [
+    rml:template "http://example.com/{Code}"
+  ];
 
-  rr:predicateObjectMap [
-    rr:predicate rdfs:label;
-    rr:objectMap [
+  rml:predicateObjectMap [
+    rml:predicate rdfs:label ;
+    rml:objectMap [
       rml:reference "Name";
-      rr:language "spanish"
+      rml:language "es"
     ]
   ].
```

### Comparing `morph_kgc-2.6.4/test/rml/xml/RMLTC0015b/test_RMLTC0015b_XML.py` & `morph_kgc-2.7.0/test/rml-core/xml/RMLTC0015b/test_RMLTC0015b_XML.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/rml/xml/RMLTC0019a/RMLTC0019a_XML.py` & `morph_kgc-2.7.0/test/rml-core/xml/RMLTC0019a/RMLTC0019a_XML.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/rml/xml/RMLTC0019b/RMLTC0019b_XML.py` & `morph_kgc-2.7.0/test/rml-core/xml/RMLTC0019b/RMLTC0019b_XML.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/rml/xml/RMLTC0020a/RMLTC0020a_XML.py` & `morph_kgc-2.7.0/test/rml-core/xml/RMLTC0020a/RMLTC0020a_XML.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/rml/xml/RMLTC0020a/mapping.ttl` & `morph_kgc-2.7.0/test/rml-in-memory/json_dictionary/RMLIMTC0013a/mapping.ttl`

 * *Files 23% similar despite different names*

```diff
@@ -1,26 +1,35 @@
-@prefix rr: <http://www.w3.org/ns/r2rml#> .
 @prefix foaf: <http://xmlns.com/foaf/0.1/> .
 @prefix ex: <http://example.com/> .
 @prefix xsd: <http://www.w3.org/2001/XMLSchema#> .
-@prefix rdf: <http://www.w3.org/1999/02/22-rdf-syntax-ns#> .
-@prefix rml:    <http://semweb.mmlab.be/ns/rml#> .
-@prefix ql:     <http://semweb.mmlab.be/ns/ql#> .
-
+@prefix rml: <http://w3id.org/rml/> .
+@prefix sd: <https://w3id.org/okn/o/sd#>.
+@prefix kg4di: <https://w3id.org/kg4di/definedBy>.
 @base <http://example.com/base/> .
 
 <TriplesMap1>
-  a rr:TriplesMap;
+  a rml:TriplesMap;
+
   rml:logicalSource [
-    rml:source "test/rml/xml/RMLTC0020a/student.xml";
-    rml:referenceFormulation ql:XPath;
-    rml:iterator "/students/student"
+    rml:source [
+			a sd:DatasetSpecification;
+			sd:name "variable1";
+			sd:hasDataTransformation [
+				sd:hasSourceCode [
+					sd:programmingLanguage "Python3.9";
+				];
+			];
+		];
+		rml:referenceFormulation rml:Dictionary;
+    rml:iterator "$.persons[*]"
   ];
 
-    rr:subjectMap [     rr:template "{Name}";
-                        rr:termType rr:IRI ];
+  rml:subjectMap [ rml:template "http://example.com/Person/{ID}/{Name}/{DateOfBirth}"];
 
-    rr:predicateObjectMap
+  rml:predicateObjectMap
     [
-    	rr:predicate rdf:type;
-    	rr:object foaf:Person;
+      rml:predicate		ex:BirthDay ;
+      rml:objectMap		[ rml:reference "DateOfBirth" ]
     ].
+
+rml:Dictionary a rml:ReferenceFormulation;
+	kg4di:definedBy "Python".
```

### Comparing `morph_kgc-2.6.4/test/rml/xml/RMLTC0020a/output.nq` & `morph_kgc-2.7.0/test/rml-core/xml/RMLTC0020a/output.nq`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/rml/xml/RMLTC0020b/RMLTC0020b_XML.py` & `morph_kgc-2.7.0/test/rml-core/xml/RMLTC0020b/RMLTC0020b_XML.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/rml/xml/attributes/data.xml` & `morph_kgc-2.7.0/test/rml-core/xml/attributes/data.xml`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/rml/xml/attributes/mapping.ttl` & `morph_kgc-2.7.0/test/rml-core/xml/attributes/mapping.ttl`

 * *Files 18% similar despite different names*

```diff
@@ -1,54 +1,54 @@
-@prefix rr: <http://www.w3.org/ns/r2rml#>.
-@prefix rml: <http://semweb.mmlab.be/ns/rml#>.
-@prefix ql: <http://semweb.mmlab.be/ns/ql#>.
-@prefix ex: <http://example.com/ns#>.
-
-<#Mapping1> a rr:TriplesMap;
-    rml:logicalSource [
-        rml:source "test/rml/xml/attributes/data.xml" ;
-        rml:iterator "/*";
-        rml:referenceFormulation ql:XPath;
-    ];
-    rr:subjectMap [
-        rr:template "http://example.com/{country@name}";
-    ];
-    rr:predicateObjectMap [
-        rr:predicate ex:rank;
-        rr:objectMap [
-            rml:reference "country/rank";
-        ];
-    ].
-
-<#Mapping2> a rr:TriplesMap;
-    rml:logicalSource [
-        rml:source "test/rml/xml/attributes/data.xml" ;
-        rml:iterator "country";
-        rml:referenceFormulation ql:XPath;
-    ];
-    rr:subjectMap [
-        rr:template "http://example.com/{@name}";
-        rr:class ex:Country;
-    ];
-    rr:predicateObjectMap [
-        rr:predicate ex:gdppc;
-        rr:objectMap [
-            rml:reference "gdppc";
-        ];
-    ].
-
-<#Mapping3> a rr:TriplesMap;
-    rml:logicalSource [
-        rml:source "test/rml/xml/attributes/data.xml" ;
-        rml:iterator "country";
-        rml:referenceFormulation ql:XPath;
-    ];
-    rr:subjectMap [
-        rr:template "http://example.com/{@name}";
-        rr:class ex:Country;
-    ];
-    rr:predicateObjectMap [
-        rr:predicate ex:neighbor;
-        rr:objectMap [
-            rml:reference "neighbor@name";
-        ];
-    ].
+@prefix rr: <http://www.w3.org/ns/r2rml#>.
+@prefix rml: <http://w3id.org/rml/>.
+@prefix ql: <http://semweb.mmlab.be/ns/ql#>.
+@prefix ex: <http://example.com/ns#>.
+
+<#Mapping1> a rml:TriplesMap;
+    rml:logicalSource [
+        rml:source "test/rml-core/xml/attributes/data.xml" ;
+        rml:iterator "/*";
+        rml:referenceFormulation rml:XPath;
+    ];
+    rml:subjectMap [
+        rml:template "http://example.com/{country@name}";
+    ];
+    rml:predicateObjectMap [
+        rml:predicate ex:rank;
+        rml:objectMap [
+            rml:reference "country/rank";
+        ];
+    ].
+
+<#Mapping2> a rml:TriplesMap;
+    rml:logicalSource [
+        rml:source "test/rml-core/xml/attributes/data.xml" ;
+        rml:iterator "country";
+        rml:referenceFormulation rml:XPath;
+    ];
+    rml:subjectMap [
+        rml:template "http://example.com/{@name}";
+        rml:class ex:Country;
+    ];
+    rml:predicateObjectMap [
+        rml:predicate ex:gdppc;
+        rml:objectMap [
+            rml:reference "gdppc";
+        ];
+    ].
+
+<#Mapping3> a rml:TriplesMap;
+    rml:logicalSource [
+        rml:source "test/rml-core/xml/attributes/data.xml" ;
+        rml:iterator "country";
+        rml:referenceFormulation rml:XPath;
+    ];
+    rml:subjectMap [
+        rml:template "http://example.com/{@name}";
+        rml:class ex:Country;
+    ];
+    rml:predicateObjectMap [
+        rml:predicate ex:neighbor;
+        rml:objectMap [
+            rml:reference "neighbor@name";
+        ];
+    ].
```

### Comparing `morph_kgc-2.6.4/test/rml/xml/attributes/output.nq` & `morph_kgc-2.7.0/test/rml-core/xml/attributes/output.nq`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/rml/xml/attributes/test_attributes_XML.py` & `morph_kgc-2.7.0/test/rml-core/xml/attributes/test_attributes_XML.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/rml/xml/complex/data.xml` & `morph_kgc-2.7.0/test/rml-core/xml/complex/data.xml`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/rml/xml/complex/mapping.yaml` & `morph_kgc-2.7.0/examples/xml/mapping.xml.yaml`

 * *Files 3% similar despite different names*

```diff
@@ -1,34 +1,36 @@
 prefixes:
   ex: "https://w3id.org/okn/os/o/"
+
 sources:
   main-source: ['data.xml~xpath', '/*']
   author-source: ['data.xml~xpath', 'author']
   pid-source: ['data.xml~xpath', 'pid']
+
 mappings:
   Author:
     sources:
       - author-source
-
     s: https://w3id.org/okn/os/i/author/$(fullname)
     po:
       - [a, ex:Author]
       - [ex:fullname, $(fullname)]
       - [ex:name, $(name)]
       - [ex:surname, $(surname)]
       - [ex:$(pid.id.scheme)ID, $(pid.id.value)]
+
   Paper:
     sources:
       - main-source
     s: https://w3id.org/okn/os/i/paper/$(id)
     po:
       - [a, ex:Paper]
       - [ex:title, $(maintitle)]
       - [ex:subtitle, $(subtitle)]
-      - [ex:description, $(description),$(language.code)~lang]
+      - [ex:description, $(description)]
       - [ex:language, $(language.label)]
       - [ex:format, $(format)]
       - [ex:publicationDate, $(publicationdate)]
       - [ex:type, $(type)]
       - [ex:country, $(country/label)]
       - [ex:license, $(instance/license)]
       - [ex:publisher, $(publisher)]
@@ -39,22 +41,24 @@
         o:
             - mapping: idTypeOpenAire
               condition:
                function: equal
                parameters:
                  - [str1, $(id)]
                  - [str2, $(id)]
+
   idTypeOpenAire:
     sources:
       - pid-source
     s: https://w3id.org/okn/os/i/idType/$(id)
     po:
       - [a, ex:idType]
       - [ex:source,OpenAire]
       - [ex:identifier,$(id)]
+
   idTypePaperResource:
     sources:
       - pid-source
     s: https://w3id.org/okn/os/i/idType/$(value)
     po:
       - [a, ex:idType]
       - [ex:source,$(scheme)]
```

### Comparing `morph_kgc-2.6.4/test/rml/xml/complex/output.nq` & `morph_kgc-2.7.0/test/rml-core/xml/complex/output.nq`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/rml/xml/complex/test_complex_XML.py` & `morph_kgc-2.7.0/test/rml-core/xml/complex/test_complex_XML.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/rml/xml/rml_spec_example_section_3/mapping.ttl` & `morph_kgc-2.7.0/test/rml-core/csv/RMLTC0008a/mapping.ttl`

 * *Files 25% similar despite different names*

```diff
@@ -1,35 +1,39 @@
-@prefix rr: <http://www.w3.org/ns/r2rml#>.
-@prefix rml: <http://semweb.mmlab.be/ns/rml#>.
-@prefix ex: <http://example.com/ns#>.
-@prefix ql: <http://semweb.mmlab.be/ns/ql#>.
-@prefix transit: <http://vocab.org/transit/terms/>.
-@prefix xsd: <http://www.w3.org/2001/XMLSchema#>.
-@prefix rdfs: <http://www.w3.org/2000/01/rdf-schema#>.
-@base <http://example.com/ns#>.
-
-<#TransportMapping> a rr:TriplesMap;
-  rml:logicalSource [
-    rml:source "test/rml/xml/rml_spec_example_section_3/Transport.xml" ;
-    rml:iterator "/transport/bus";
-    rml:referenceFormulation ql:XPath;
-  ];
-
-  rr:subjectMap [
-    rr:template "http://trans.example.com/{@id}";
-    rr:class transit:Stop
-  ];
-
-  rr:predicateObjectMap [
-    rr:predicate transit:stop;
-    rr:objectMap [
-      rml:reference "route/stop/@id";
-      rr:datatype xsd:int
-    ]
-  ];
-
-  rr:predicateObjectMap [
-    rr:predicate rdfs:label;
-    rr:objectMap [
-      rml:reference "route/stop"
-    ]
-  ].
+@prefix foaf: <http://xmlns.com/foaf/0.1/> .
+@prefix ex: <http://example.com/> .
+@prefix xsd: <http://www.w3.org/2001/XMLSchema#> .
+@prefix rml: <http://w3id.org/rml/> .
+@prefix rdf: <http://www.w3.org/1999/02/22-rdf-syntax-ns#> .
+@base <http://example.com/base/> .
+
+<TriplesMap1>
+  a rml:TriplesMap;
+
+  rml:logicalSource [
+    rml:source "test/rml-core/csv/RMLTC0008a/student.csv";
+    rml:referenceFormulation rml:CSV
+  ];
+
+  rml:subjectMap [
+    rml:template "http://example.com/Student/{ID}/{Name}";
+    rml:graphMap [ rml:template "http://example.com/graph/Student/{ID}/{Name}" ]
+  ];
+
+  rml:predicateObjectMap [
+    rml:predicate rdf:type ;
+    rml:object foaf:Person;
+  ];
+
+  rml:predicateObjectMap [
+    rml:predicate ex:id ;
+    rml:objectMap [ rml:reference "ID" ]
+  ];
+
+  rml:predicateObjectMap [
+    rml:predicate foaf:name ;
+    rml:objectMap [ rml:reference "Name" ]
+  ];
+
+  rml:predicateObjectMap [
+    rml:predicate ex:Sport ;
+    rml:objectMap [ rml:reference "Sport" ]
+  ] .
```

### Comparing `morph_kgc-2.6.4/test/rml/xml/rml_spec_example_section_3/output.nq` & `morph_kgc-2.7.0/test/rml-core/xml/rml_spec_example_section_3/output.nq`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/rml/xml/rml_spec_example_section_3/test_rml_spec_example_section_3_XML.py` & `morph_kgc-2.7.0/test/rml-core/xml/rml_spec_example_section_3/test_rml_spec_example_section_3_XML.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/rml/xml/rml_spec_example_section_5/mapping.ttl` & `morph_kgc-2.7.0/test/rml-core/csv/RMLTC0007e/mapping.ttl`

 * *Files 22% similar despite different names*

```diff
@@ -1,27 +1,29 @@
-@prefix rr: <http://www.w3.org/ns/r2rml#>.
-@prefix rml: <http://semweb.mmlab.be/ns/rml#>.
-@prefix ex: <http://example.com/ns#>.
-@prefix ql: <http://semweb.mmlab.be/ns/ql#>.
-@prefix xsd: <http://www.w3.org/2001/XMLSchema#>.
-@prefix rdfs: <http://www.w3.org/2000/01/rdf-schema#>.
-@base <http://example.com/ns#>.
-
-<#TransportMapping> a rr:TriplesMap;
-  rml:logicalSource [
-    rml:source "test/rml/xml/rml_spec_example_section_5/Transport.xml" ;
-    rml:iterator "/transport/bus/route/stop";
-    rml:referenceFormulation ql:XPath;
-  ];
-
-  rr:subjectMap [
-    rr:template
-      "http://trans.example.com/stop/{@id}";
-    rr:class ex:Stop
-  ];
-
-  rr:predicateObjectMap [
-    rr:predicate rdfs:label;
-    rr:objectMap [
-      rml:reference "."
-    ]
-  ].
+@prefix foaf: <http://xmlns.com/foaf/0.1/> .
+@prefix ex: <http://example.com/> .
+@prefix xsd: <http://www.w3.org/2001/XMLSchema#> .
+@prefix rml: <http://w3id.org/rml/> .
+@base <http://example.com/base/> .
+
+<TriplesMap1> a rml:TriplesMap;
+
+  rml:logicalSource [
+    rml:source "test/rml-core/csv/RMLTC0007e/student.csv";
+    rml:referenceFormulation rml:CSV
+  ];
+
+  rml:subjectMap [
+    rml:template "http://example.com/Student/{ID}/{Name}";
+    rml:graph ex:PersonGraph ;
+    rml:class foaf:Person
+  ];
+
+  rml:predicateObjectMap [
+    rml:predicate ex:id ;
+    rml:objectMap [ rml:reference "ID"; ]
+  ];
+
+  rml:predicateObjectMap
+    [
+      rml:predicate		foaf:name ;
+      rml:objectMap		[ rml:reference "Name" ]
+    ].
```

### Comparing `morph_kgc-2.6.4/test/rml/xml/rml_spec_example_section_5/output.nq` & `morph_kgc-2.7.0/test/rml-core/xml/rml_spec_example_section_5/output.nq`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/rml/xml/rml_spec_example_section_5/test_rml_spec_example_section_5_XML.py` & `morph_kgc-2.7.0/test/rml-core/xml/rml_spec_example_section_5/test_rml_spec_example_section_5_XML.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/rml-fnml/RMLFNOTC0000-CSV/mapping.ttl` & `morph_kgc-2.7.0/test/rml-fnml/RMLFNOTC0002-CSV/mapping.ttl`

 * *Files 6% similar despite different names*

```diff
@@ -7,22 +7,29 @@
 @prefix grel: <http://users.ugent.be/~bjdmeest/function/grel.ttl#> .
 @prefix idlab-fn: <http://example.com/idlab/function/> .
 
 @base <http://example.com/base/> .
 
 <TriplesMap1>
     rml:logicalSource [
-        rml:source "test/rml-fnml/RMLFNOTC0000-CSV/student.csv";
+        rml:source "test/rml-fnml/RMLFNOTC0002-CSV/student.csv";
         rml:referenceFormulation rml:CSV
     ];
     rml:subjectMap [
         rml:template "http://example.com/{Name}"
     ];
     rml:predicateObjectMap [
         rml:predicate foaf:name;
         rml:objectMap [
             rml:functionExecution <#Execution> ;
         ]
     ] .
 
 <#Execution>
-    rml:function morph-kgc:uuid .
+    rml:function grel:toUpperCase ;
+    rml:input
+        [
+            rml:parameter grel:valueParam ;
+            rml:inputValueMap [
+                rml:constant "name" ;
+            ]
+        ] .
```

### Comparing `morph_kgc-2.6.4/test/rml-fnml/RMLFNOTC0000-CSV/test_RMLFNOTC0000-CSV.py` & `morph_kgc-2.7.0/test/rml-fnml/RMLFNOTC0000-CSV/test_RMLFNOTC0000-CSV.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/rml-fnml/RMLFNOTC0001-CSV/mapping.ttl` & `morph_kgc-2.7.0/test/rml-fnml/RMLFNOTC0008-CSV/mapping.ttl`

 * *Files 4% similar despite different names*

```diff
@@ -7,29 +7,27 @@
 @prefix grel: <http://users.ugent.be/~bjdmeest/function/grel.ttl#> .
 @prefix idlab-fn: <http://example.com/idlab/function/> .
 
 @base <http://example.com/base/> .
 
 <TriplesMap1>
     rml:logicalSource [
-        rml:source "test/rml-fnml/RMLFNOTC0001-CSV/student.csv";
+        rml:source "test/rml-fnml/RMLFNOTC0008-CSV/student.csv";
         rml:referenceFormulation rml:CSV
     ];
     rml:subjectMap [
         rml:template "http://example.com/{Name}"
     ];
     rml:predicateObjectMap [
         rml:predicate foaf:name;
-        rml:objectMap [
-            rml:functionExecution <#Execution> ;
-        ]
+        rml:objectMap [ rml:functionExecution <#Execution> ] ;
     ] .
 
 <#Execution>
     rml:function grel:toUpperCase ;
     rml:input
         [
             rml:parameter grel:valueParam ;
             rml:inputValueMap [
-                rml:reference "Name" ;
-            ]
+                rml:template "Name: {Name}"
+            ];
         ] .
```

### Comparing `morph_kgc-2.6.4/test/rml-fnml/RMLFNOTC0001-CSV/test_RMLFNOTC0001-CSV.py` & `morph_kgc-2.7.0/test/rml-fnml/RMLFNOTC0001-CSV/test_RMLFNOTC0001-CSV.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/rml-fnml/RMLFNOTC0002-CSV/mapping.ttl` & `morph_kgc-2.7.0/test/rml-fnml/math_round/mapping.ttl`

 * *Files 10% similar despite different names*

```diff
@@ -7,29 +7,30 @@
 @prefix grel: <http://users.ugent.be/~bjdmeest/function/grel.ttl#> .
 @prefix idlab-fn: <http://example.com/idlab/function/> .
 
 @base <http://example.com/base/> .
 
 <TriplesMap1>
     rml:logicalSource [
-        rml:source "test/rml-fnml/RMLFNOTC0002-CSV/student.csv";
-        rml:referenceFormulation rml:CSV
+        rml:source "test/rml-fnml/math_round/distances.tsv" ;
+        rml:referenceFormulation rml:CSV ;
     ];
     rml:subjectMap [
-        rml:template "http://example.com/{Name}"
+        rml:template "http://example.com/distance/{id}"
     ];
     rml:predicateObjectMap [
-        rml:predicate foaf:name;
+        rml:predicate ex:distance;
         rml:objectMap [
             rml:functionExecution <#Execution> ;
+            rml:datatype xsd:integer
         ]
-    ] .
+    ].
 
 <#Execution>
-    rml:function grel:toUpperCase ;
+    rml:function grel:math_round ;
     rml:input
         [
-            rml:parameter grel:valueParam ;
+            rml:parameter grel:param_dec_n ;
             rml:inputValueMap [
-                rml:constant "name" ;
+                rml:reference "distance_km"
             ]
         ] .
```

### Comparing `morph_kgc-2.6.4/test/rml-fnml/RMLFNOTC0002-CSV/test_RMLFNOTC0002-CSV.py` & `morph_kgc-2.7.0/test/rml-fnml/RMLFNOTC0002-CSV/test_RMLFNOTC0002-CSV.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/rml-fnml/RMLFNOTC0003-CSV/mapping.ttl` & `morph_kgc-2.7.0/test/rml-fnml/date_to_date/mapping.ttl`

 * *Files 18% similar despite different names*

```diff
@@ -2,38 +2,40 @@
 @prefix ex: <http://example.com/> .
 @prefix xsd: <http://www.w3.org/2001/XMLSchema#> .
 @prefix rml: <http://w3id.org/rml/> .
 @prefix fno: <https://w3id.org/function/ontology#> .
 @prefix morph-kgc: <https://github.com/morph-kgc/morph-kgc/function/built-in.ttl#> .
 @prefix grel: <http://users.ugent.be/~bjdmeest/function/grel.ttl#> .
 @prefix idlab-fn: <http://example.com/idlab/function/> .
+@prefix dct: <http://purl.org/dc/terms/> .
 
 @base <http://example.com/base/> .
 
 <TriplesMap1>
     rml:logicalSource [
-        rml:source "test/rml-fnml/RMLFNOTC0003-CSV/student.csv";
-        rml:referenceFormulation rml:CSV
+        rml:source "test/rml-fnml/date_to_date/calendar.csv" ;
+        rml:referenceFormulation rml:CSV ;
     ];
     rml:subjectMap [
-        rml:template "http://example.com/{Name}"
+        rml:template "http://transport.linkeddata.es/madrid/metro/calendar_rules/{service_id}"
     ];
     rml:predicateObjectMap [
-        rml:predicate foaf:name;
+        rml:predicate dct:date;
         rml:objectMap [
             rml:functionExecution <#Execution> ;
+            rml:datatype xsd:date
         ]
-    ] .
+    ].
 
 <#Execution>
-    rml:function grel:escape ;
+    rml:function grel:date_toDate ;
     rml:input
         [
             rml:parameter grel:valueParam ;
             rml:inputValueMap [
-                rml:reference "Comment"
+                rml:reference "start_date"
             ]
         ] ,
         [
-            rml:parameter grel:modeParam ;
-            rml:inputValue "html"
+            rml:parameter grel:param_string_pattern ;
+            rml:inputValue "%Y-%m-%d %H:%M:%S"
         ] .
```

### Comparing `morph_kgc-2.6.4/test/rml-fnml/RMLFNOTC0003-CSV/test_RMLFNOTC0003-CSV.py` & `morph_kgc-2.7.0/test/rml-fnml/RMLFNOTC0003-CSV/test_RMLFNOTC0003-CSV.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/rml-fnml/RMLFNOTC0004-CSV/mapping.ttl` & `morph_kgc-2.7.0/test/rml-fnml/RMLFNOTC0004-CSV/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/rml-fnml/RMLFNOTC0004-CSV/test_RMLFNOTC0004-CSV.py` & `morph_kgc-2.7.0/test/rml-fnml/RMLFNOTC0004-CSV/test_RMLFNOTC0004-CSV.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/rml-fnml/RMLFNOTC0005-CSV/mapping.ttl` & `morph_kgc-2.7.0/test/rml-fnml/RMLFNOTC0005-CSV/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/rml-fnml/RMLFNOTC0005-CSV/test_RMLFNOTC0005-CSV.py` & `morph_kgc-2.7.0/test/rml-fnml/RMLFNOTC0005-CSV/test_RMLFNOTC0005-CSV.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/rml-fnml/RMLFNOTC0006-CSV/mapping.ttl` & `morph_kgc-2.7.0/test/rml-fnml/RMLFNOTC0006-CSV/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/rml-fnml/RMLFNOTC0006-CSV/test_RMLFNOTC0006-CSV.py` & `morph_kgc-2.7.0/test/rml-fnml/RMLFNOTC0006-CSV/test_RMLFNOTC0006-CSV.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/rml-fnml/RMLFNOTC0008-CSV/mapping.ttl` & `morph_kgc-2.7.0/test/rml-fnml/RMLFNOTC0009-CSV/mapping.ttl`

 * *Files 18% similar despite different names*

```diff
@@ -5,29 +5,55 @@
 @prefix fno: <https://w3id.org/function/ontology#> .
 @prefix morph-kgc: <https://github.com/morph-kgc/morph-kgc/function/built-in.ttl#> .
 @prefix grel: <http://users.ugent.be/~bjdmeest/function/grel.ttl#> .
 @prefix idlab-fn: <http://example.com/idlab/function/> .
 
 @base <http://example.com/base/> .
 
-<TriplesMap1>
+<#Person_Mapping>
     rml:logicalSource [
-        rml:source "test/rml-fnml/RMLFNOTC0008-CSV/student.csv";
+        rml:source "test/rml-fnml/RMLFNOTC0009-CSV/student.csv";
         rml:referenceFormulation rml:CSV
     ];
     rml:subjectMap [
         rml:template "http://example.com/{Name}"
     ];
-    rml:predicateObjectMap [
-        rml:predicate foaf:name;
-        rml:objectMap [ rml:functionExecution <#Execution> ] ;
-    ] .
+    rml:predicateObjectMap <#NameMapping> .
 
-<#Execution>
+<#NameMapping>
+    rml:predicate foaf:name ;
+    rml:objectMap [
+        rml:functionExecution <#Execution> ;
+    ]; .
+
+<#Execution> a rml:FunctionExecution ;
     rml:function grel:toUpperCase ;
     rml:input
         [
+            a rml:Input ;
             rml:parameter grel:valueParam ;
             rml:inputValueMap [
-                rml:template "Name: {Name}"
-            ];
+                rml:functionExecution <#Execution2> ;
+                rml:return grel:stringOut
+            ]
+        ] .
+
+<#Execution2> a rml:Execution ;
+    rml:function grel:string_replace ;
+    rml:input
+        [
+            a rml:Input ;
+            rml:parameter grel:valueParam ;
+            rml:inputValueMap [
+                rml:reference "Name"
+            ]
+        ] ,
+        [
+            a rml:Input ;
+            rml:parameter grel:param_find ;
+            rml:inputValue " "
+        ] ,
+        [
+            a rml:Input ;
+            rml:parameter grel:param_replace  ;
+            rml:inputValue "-"
         ] .
```

### Comparing `morph_kgc-2.6.4/test/rml-fnml/RMLFNOTC0008-CSV/test_RMLFNOTC0008-CSV.py` & `morph_kgc-2.7.0/test/rml-fnml/RMLFNOTC0008-CSV/test_RMLFNOTC0008-CSV.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/rml-fnml/RMLFNOTC0009-CSV/mapping.ttl` & `morph_kgc-2.7.0/test/rml-fnml/controls_if/mapping.ttl`

 * *Files 19% similar despite different names*

```diff
@@ -2,58 +2,65 @@
 @prefix ex: <http://example.com/> .
 @prefix xsd: <http://www.w3.org/2001/XMLSchema#> .
 @prefix rml: <http://w3id.org/rml/> .
 @prefix fno: <https://w3id.org/function/ontology#> .
 @prefix morph-kgc: <https://github.com/morph-kgc/morph-kgc/function/built-in.ttl#> .
 @prefix grel: <http://users.ugent.be/~bjdmeest/function/grel.ttl#> .
 @prefix idlab-fn: <http://example.com/idlab/function/> .
+@prefix gtfs: <http://vocab.gtfs.org/terms#> .
 
 @base <http://example.com/base/> .
 
-<#Person_Mapping>
+<TriplesMap1>
     rml:logicalSource [
-        rml:source "test/rml-fnml/RMLFNOTC0009-CSV/student.csv";
-        rml:referenceFormulation rml:CSV
+        rml:source "test/rml-fnml/controls_if/calendar.csv" ;
+        rml:referenceFormulation rml:CSV ;
     ];
     rml:subjectMap [
-        rml:template "http://example.com/{Name}"
+        rml:template "http://transport.linkeddata.es/madrid/metro/calendar_rules/{service_id}"
     ];
-    rml:predicateObjectMap <#NameMapping> .
-
-<#NameMapping>
-    rml:predicate foaf:name ;
-    rml:objectMap [
-        rml:functionExecution <#Execution> ;
-    ]; .
+    rml:predicateObjectMap [
+        rml:predicate gtfs:monday;
+        rml:objectMap [
+            rml:functionExecution <#Execution1> ;
+            rml:datatype xsd:boolean
+        ]
+    ];
+    rml:predicateObjectMap [
+        rml:predicate gtfs:tuesday;
+        rml:objectMap [
+            rml:functionExecution <#Execution2> ;
+            rml:datatype xsd:boolean
+        ]
+    ].
 
-<#Execution> a rml:FunctionExecution ;
-    rml:function grel:toUpperCase ;
+<#Execution1>
+    rml:function grel:controls_if ;
     rml:input
         [
-            a rml:Input ;
-            rml:parameter grel:valueParam ;
+            rml:parameter grel:bool_b ;
             rml:inputValueMap [
-                rml:functionExecution <#Execution2> ;
-                rml:return grel:stringOut
+                rml:template "'1' == '{monday}'"
             ]
+        ] ,
+        [
+            rml:parameter grel:any_true ;
+            rml:inputValue "true"
+        ] ,
+        [
+            rml:parameter grel:any_false ;
+            rml:inputValue "false"
         ] .
 
-<#Execution2> a rml:Execution ;
-    rml:function grel:string_replace ;
+<#Execution2>
+    rml:function grel:controls_if ;
     rml:input
         [
-            a rml:Input ;
-            rml:parameter grel:valueParam ;
+            rml:parameter grel:bool_b ;
             rml:inputValueMap [
-                rml:reference "Name"
+                rml:template "'1' == '{tuesday}'"
             ]
         ] ,
         [
-            a rml:Input ;
-            rml:parameter grel:param_find ;
-            rml:inputValue " "
-        ] ,
-        [
-            a rml:Input ;
-            rml:parameter grel:param_replace  ;
-            rml:inputValue "-"
+            rml:parameter grel:any_true ;
+            rml:inputValue "true"
         ] .
```

### Comparing `morph_kgc-2.6.4/test/rml-fnml/RMLFNOTC0009-CSV/test_RMLFNOTC0009-CSV.py` & `morph_kgc-2.7.0/test/rml-fnml/RMLFNOTC0009-CSV/test_RMLFNOTC0009-CSV.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/rml-fnml/array_get_slice/mapping.ttl` & `morph_kgc-2.7.0/test/rml-fnml/controls_if_cast/mapping.ttl`

 * *Files 13% similar despite different names*

```diff
@@ -2,58 +2,64 @@
 @prefix ex: <http://example.com/> .
 @prefix xsd: <http://www.w3.org/2001/XMLSchema#> .
 @prefix rml: <http://w3id.org/rml/> .
 @prefix fno: <https://w3id.org/function/ontology#> .
 @prefix morph-kgc: <https://github.com/morph-kgc/morph-kgc/function/built-in.ttl#> .
 @prefix grel: <http://users.ugent.be/~bjdmeest/function/grel.ttl#> .
 @prefix idlab-fn: <http://example.com/idlab/function/> .
+@prefix gtfs: <http://vocab.gtfs.org/terms#> .
 
 @base <http://example.com/base/> .
-
 <TriplesMap1>
     rml:logicalSource [
-        rml:source "test/rml-fnml/array_get_slice/article.tsv" ;
+        rml:source "test/rml-fnml/controls_if_cast/calendar.csv" ;
         rml:referenceFormulation rml:CSV ;
     ];
     rml:subjectMap [
-        rml:template "http://example.com/articles/{title}"
+        rml:template "http://transport.linkeddata.es/madrid/metro/calendar_rules/{service_id}"
     ];
     rml:predicateObjectMap [
-        rml:predicate ex:firstAuthor;
+        rml:predicate gtfs:monday;
         rml:objectMap [
             rml:functionExecution <#Execution1> ;
+            rml:datatype xsd:boolean
         ]
     ];
     rml:predicateObjectMap [
-        rml:predicate ex:otherAuthors;
+        rml:predicate gtfs:tuesday;
         rml:objectMap [
             rml:functionExecution <#Execution2> ;
+            rml:datatype xsd:boolean
         ]
     ].
 
 <#Execution1>
-    rml:function grel:array_get ;
+    rml:function morph-kgc:controls_if_cast ;
     rml:input
         [
-            rml:parameter grel:param_a ;
+            rml:parameter grel:bool_b ;
             rml:inputValueMap [
-                rml:reference "authors"
+                rml:reference "monday"
             ]
         ] ,
         [
-            rml:parameter grel:p_int_i_from ;
-            rml:inputValue "0"
+            rml:parameter grel:any_true ;
+            rml:inputValue "true"
+        ] ,
+        [
+            rml:parameter grel:any_false ;
+            rml:inputValue "false"
         ] .
 
 <#Execution2>
-    rml:function grel:array_slice ;
+    rml:function morph-kgc:controls_if_cast ;
     rml:input
         [
-            rml:parameter grel:param_a ;
+            rml:parameter grel:bool_b ;
             rml:inputValueMap [
-                rml:reference "authors"
+                rml:reference "tuesday"
             ]
         ] ,
         [
-            rml:parameter grel:p_int_i_from ;
-            rml:inputValue "1"
+            rml:parameter grel:any_true ;
+            rml:inputValue "true"
         ] .
```

### Comparing `morph_kgc-2.6.4/test/rml-fnml/array_get_slice/test_array_get_slice.py` & `morph_kgc-2.7.0/test/rml-fnml/array_get_slice/test_array_get_slice.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/rml-fnml/controls_if/output.nq` & `morph_kgc-2.7.0/test/rml-fnml/controls_if/output.nq`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/rml-fnml/controls_if/test_controls_if.py` & `morph_kgc-2.7.0/test/rml-fnml/controls_if/test_controls_if.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/rml-fnml/controls_if_cast/output.nq` & `morph_kgc-2.7.0/test/rml-fnml/controls_if_cast/output.nq`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/rml-fnml/controls_if_cast/test_controls_if_cast.py` & `morph_kgc-2.7.0/test/rml-fnml/controls_if_cast/test_controls_if_cast.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/rml-fnml/date_to_date/mapping.ttl` & `morph_kgc-2.7.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0000/mapping.ttl`

 * *Files 26% similar despite different names*

```diff
@@ -1,41 +1,39 @@
 @prefix foaf: <http://xmlns.com/foaf/0.1/> .
 @prefix ex: <http://example.com/> .
 @prefix xsd: <http://www.w3.org/2001/XMLSchema#> .
 @prefix rml: <http://w3id.org/rml/> .
-@prefix fno: <https://w3id.org/function/ontology#> .
-@prefix morph-kgc: <https://github.com/morph-kgc/morph-kgc/function/built-in.ttl#> .
-@prefix grel: <http://users.ugent.be/~bjdmeest/function/grel.ttl#> .
-@prefix idlab-fn: <http://example.com/idlab/function/> .
-@prefix dct: <http://purl.org/dc/terms/> .
+@prefix sd: <https://w3id.org/okn/o/sd#>.
+@prefix kg4di: <https://w3id.org/kg4di/definedBy>.
 
 @base <http://example.com/base/> .
 
 <TriplesMap1>
-    rml:logicalSource [
-        rml:source "test/rml-fnml/date_to_date/calendar.csv" ;
-        rml:referenceFormulation rml:CSV ;
-    ];
-    rml:subjectMap [
-        rml:template "http://transport.linkeddata.es/madrid/metro/calendar_rules/{service_id}"
-    ];
-    rml:predicateObjectMap [
-        rml:predicate dct:date;
-        rml:objectMap [
-            rml:functionExecution <#Execution> ;
-            rml:datatype xsd:date
-        ]
-    ].
-
-<#Execution>
-    rml:function grel:date_toDate ;
-    rml:input
-        [
-            rml:parameter grel:valueParam ;
-            rml:inputValueMap [
-                rml:reference "start_date"
-            ]
-        ] ,
-        [
-            rml:parameter grel:param_string_pattern ;
-            rml:inputValue "%Y-%m-%d %H:%M:%S"
-        ] .
+  a rml:TriplesMap;
+
+  rml:logicalSource [
+    rml:source [
+			a sd:DatasetSpecification;
+			sd:name "variable1";
+			sd:hasDataTransformation [
+				sd:hasSoftwareRequirements "pandas>=1.1.0";
+				sd:hasSourceCode [
+					sd:programmingLanguage "Python3.9";
+				];
+			];
+		];
+		rml:referenceFormulation rml:DataFrame;
+  ] ;
+
+  rml:subjectMap [
+    rml:template "http://example.com/{Name}"
+  ];
+
+  rml:predicateObjectMap [
+    rml:predicate foaf:name ;
+    rml:objectMap [
+      rml:reference "Name"
+    ]
+  ].
+
+rml:DataFrame a rml:ReferenceFormulation;
+	kg4di:definedBy "Pandas".
```

### Comparing `morph_kgc-2.6.4/test/rml-fnml/date_to_date/test_date_to_date.py` & `morph_kgc-2.7.0/test/rml-fnml/date_to_date/test_date_to_date.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/rml-fnml/math_round/mapping.ttl` & `morph_kgc-2.7.0/test/rml-core/csv/triples_map_without_pom/mapping.ttl`

 * *Files 22% similar despite different names*

```diff
@@ -1,36 +1,39 @@
 @prefix foaf: <http://xmlns.com/foaf/0.1/> .
 @prefix ex: <http://example.com/> .
 @prefix xsd: <http://www.w3.org/2001/XMLSchema#> .
 @prefix rml: <http://w3id.org/rml/> .
-@prefix fno: <https://w3id.org/function/ontology#> .
-@prefix morph-kgc: <https://github.com/morph-kgc/morph-kgc/function/built-in.ttl#> .
-@prefix grel: <http://users.ugent.be/~bjdmeest/function/grel.ttl#> .
-@prefix idlab-fn: <http://example.com/idlab/function/> .
-
+@prefix activity: <http://example.com/activity/> .
+@prefix rdfs: <http://www.w3.org/2000/01/rdf-schema#> .
 @base <http://example.com/base/> .
 
 <TriplesMap1>
-    rml:logicalSource [
-        rml:source "test/rml-fnml/math_round/distances.tsv" ;
-        rml:referenceFormulation rml:CSV ;
-    ];
-    rml:subjectMap [
-        rml:template "http://example.com/distance/{id}"
-    ];
-    rml:predicateObjectMap [
-        rml:predicate ex:distance;
-        rml:objectMap [
-            rml:functionExecution <#Execution> ;
-            rml:datatype xsd:integer
-        ]
-    ].
-
-<#Execution>
-    rml:function grel:math_round ;
-    rml:input
-        [
-            rml:parameter grel:param_dec_n ;
-            rml:inputValueMap [
-                rml:reference "distance_km"
-            ]
-        ] .
+  a rml:TriplesMap;
+
+  rml:logicalSource [
+    rml:source "test/rml-core/csv/triples_map_without_pom/student.csv";
+    rml:referenceFormulation rml:CSV
+  ];
+
+  rml:subjectMap [ rml:template "http://example.com/resource/student_{ID}" ];
+
+  rml:predicateObjectMap [
+    rml:predicate <http://example.com/ontology/practises> ;
+    rml:objectMap [
+      a rml:RefObjectMap ;
+      rml:parentTriplesMap <TriplesMap2>;
+      rml:joinCondition [
+        rml:child "Sport" ;
+        rml:parent "ID" ;
+      ]
+    ]
+  ] .
+
+<TriplesMap2>
+  a rml:TriplesMap;
+
+  rml:logicalSource [
+    rml:source "test/rml-core/csv/triples_map_without_pom/sport.csv";
+    rml:referenceFormulation rml:CSV
+  ];
+
+  rml:subjectMap [ rml:template "http://example.com/resource/sport_{ID}" ].
```

### Comparing `morph_kgc-2.6.4/test/rml-fnml/math_round/test_math_round.py` & `morph_kgc-2.7.0/test/rml-fnml/math_round/test_math_round.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/rml-fnml/split_explode/test_split_explode.py` & `morph_kgc-2.7.0/test/rml-fnml/split_explode/test_split_explode.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/rml-fnml/split_explode_null/mapping.ttl` & `morph_kgc-2.7.0/test/rml-core/csv/RMLTC0009a/mapping.ttl`

 * *Files 22% similar despite different names*

```diff
@@ -1,39 +1,49 @@
 @prefix foaf: <http://xmlns.com/foaf/0.1/> .
 @prefix ex: <http://example.com/> .
 @prefix xsd: <http://www.w3.org/2001/XMLSchema#> .
 @prefix rml: <http://w3id.org/rml/> .
-@prefix fno: <https://w3id.org/function/ontology#> .
-@prefix morph-kgc: <https://github.com/morph-kgc/morph-kgc/function/built-in.ttl#> .
-@prefix grel: <http://users.ugent.be/~bjdmeest/function/grel.ttl#> .
-@prefix idlab-fn: <http://example.com/idlab/function/> .
-
+@prefix activity: <http://example.com/activity/> .
+@prefix rdfs: <http://www.w3.org/2000/01/rdf-schema#> .
 @base <http://example.com/base/> .
 
 <TriplesMap1>
-    rml:logicalSource [
-        rml:source "test/rml-fnml/split_explode_null/mixed_content_list.csv";
-        rml:referenceFormulation rml:CSV
-    ];
-    rml:subjectMap [
-        rml:template "http://example.com/{ID}"
-    ];
-    rml:predicateObjectMap [
-        rml:predicate ex:col;
-        rml:objectMap [
-            rml:functionExecution <#Execution> ;
-        ]
-    ] .
-
-<#Execution>
-    rml:function morph-kgc:string_split_explode ;
-    rml:input
-        [
-            rml:parameter grel:valueParam ;
-            rml:inputValueMap [
-                rml:reference "COL"
-            ]
-        ] ,
-        [
-            rml:parameter grel:param_string_sep ;
-            rml:inputValue ";"
-        ] .
+  a rml:TriplesMap;
+
+  rml:logicalSource [
+    rml:source "test/rml-core/csv/RMLTC0009a/student.csv";
+    rml:referenceFormulation rml:CSV
+  ];
+
+  rml:subjectMap [ rml:template "http://example.com/resource/student_{ID}" ];
+
+  rml:predicateObjectMap [
+    rml:predicate foaf:name ;
+    rml:objectMap [ rml:reference "Name" ]
+  ] ;
+
+  rml:predicateObjectMap [
+    rml:predicate <http://example.com/ontology/practises> ;
+    rml:objectMap [
+      a rml:RefObjectMap ;
+      rml:parentTriplesMap <TriplesMap2>;
+      rml:joinCondition [
+        rml:child "Sport" ;
+        rml:parent "ID" ;
+      ]
+    ]
+  ] .
+
+<TriplesMap2>
+  a rml:TriplesMap;
+
+  rml:logicalSource [
+    rml:source "test/rml-core/csv/RMLTC0009a/sport.csv";
+    rml:referenceFormulation rml:CSV
+  ];
+
+  rml:subjectMap [ rml:template "http://example.com/resource/sport_{ID}" ];
+
+  rml:predicateObjectMap [
+    rml:predicate rdfs:label ;
+    rml:objectMap [ rml:reference "Name" ];
+  ].
```

### Comparing `morph_kgc-2.6.4/test/rml-fnml/split_explode_null/test_split_explode_null.py` & `morph_kgc-2.7.0/test/rml-fnml/split_explode_null/test_split_explode_null.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/rml-fnml/udf/mapping.ttl` & `morph_kgc-2.7.0/test/rml-core/json/RMLTC0012c/mapping.ttl`

 * *Files 21% similar despite different names*

```diff
@@ -1,35 +1,30 @@
 @prefix foaf: <http://xmlns.com/foaf/0.1/> .
 @prefix ex: <http://example.com/> .
 @prefix xsd: <http://www.w3.org/2001/XMLSchema#> .
 @prefix rml: <http://w3id.org/rml/> .
-@prefix fno: <https://w3id.org/function/ontology#> .
-@prefix morph-kgc: <https://github.com/morph-kgc/morph-kgc/function/built-in.ttl#> .
-@prefix grel: <http://users.ugent.be/~bjdmeest/function/grel.ttl#> .
-@prefix idlab-fn: <http://example.com/idlab/function/> .
 
 @base <http://example.com/base/> .
 
 <TriplesMap1>
-    rml:logicalSource [
-        rml:source "test/rml-fnml/udf/student.csv";
-        rml:referenceFormulation rml:CSV
-    ];
-    rml:subjectMap [
-        rml:template "http://example.com/{Name}"
-    ];
-    rml:predicateObjectMap [
-        rml:predicate foaf:name;
-        rml:objectMap [
-            rml:functionExecution <#Execution> ;
-        ]
-    ] .
+  a rml:TriplesMap;
 
-<#Execution>
-    rml:function ex:toUpperCase ;
-    rml:input
-        [
-            rml:parameter grel:valueParam ;
-            rml:inputValueMap [
-                rml:reference "Name" ;
-            ]
-        ] .
+  rml:logicalSource [
+    rml:source "test/rml-core/json/RMLTC0012c/persons.json";
+    rml:referenceFormulation rml:JSONPath;
+    rml:iterator "$.persons[*]"
+  ];
+
+  rml:predicateObjectMap [
+    rml:predicate foaf:name ;
+    rml:objectMap [
+      rml:template "{fname} {lname}";
+      rml:termType rml:Literal ;
+    ]
+  ];
+
+  rml:predicateObjectMap [
+    rml:predicate ex:amount ;
+    rml:objectMap    [
+      rml:reference "amount";
+    ]
+  ].
```

### Comparing `morph_kgc-2.6.4/test/rml-fnml/udf/test_udf.py` & `morph_kgc-2.7.0/test/rml-fnml/udf/test_udf.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/rml-in-memory/json_dictionary/RMLIMTC0000/mapping.ttl` & `morph_kgc-2.7.0/test/rml-in-memory/json_dictionary/RMLIMTC0008c/mapping.ttl`

 * *Files 15% similar despite different names*

```diff
@@ -1,40 +1,36 @@
-@prefix rr: <http://www.w3.org/ns/r2rml#> .
 @prefix foaf: <http://xmlns.com/foaf/0.1/> .
 @prefix ex: <http://example.com/> .
 @prefix xsd: <http://www.w3.org/2001/XMLSchema#> .
-@prefix rml: <http://semweb.mmlab.be/ns/rml#> .
-@prefix ql: <http://semweb.mmlab.be/ns/ql#> .
+@prefix rml: <http://w3id.org/rml/> .
+@prefix activity: <http://example.com/activity/> .
+@base <http://example.com/base/> .
 @prefix sd: <https://w3id.org/okn/o/sd#>.
 @prefix kg4di: <https://w3id.org/kg4di/definedBy>.
-@base <http://example.com/base/> .
 
 <TriplesMap1>
-  a rr:TriplesMap;
+  a rml:TriplesMap;
 
   rml:logicalSource [
     rml:source [
 			a sd:DatasetSpecification;
 			sd:name "variable1";
 			sd:hasDataTransformation [
 				sd:hasSourceCode [
 					sd:programmingLanguage "Python3.9";
 				];
 			];
 		];
-		rml:referenceFormulation ql:Dictionary;
+		rml:referenceFormulation rml:Dictionary;
     rml:iterator "$.students[*]"
-  ] ;
-
-  rr:subjectMap [
-    rr:template "http://example.com/{Name}"
   ];
 
-  rr:predicateObjectMap [
-    rr:predicate foaf:name ;
-    rr:objectMap [
-      rml:reference "Name"
-    ]
-  ].
+  rml:subjectMap [ rml:template "http://example.com/Student/{ID}/{Name}" ];
+
+  rml:predicateObjectMap [
+    rml:predicate foaf:name ;
+    rml:predicate ex:name ;
+    rml:objectMap [ rml:reference "Name" ]
+  ] .
 
-ql:Dictionary a rml:ReferenceFormulation;
+rml:Dictionary a rml:ReferenceFormulation;
 	kg4di:definedBy "Python".
```

### Comparing `morph_kgc-2.6.4/test/rml-in-memory/json_dictionary/RMLIMTC0000/test_RMLTC0000_DICT.py` & `morph_kgc-2.7.0/test/rml-in-memory/json_dictionary/RMLIMTC0000/test_RMLTC0000_DICT.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/rml-in-memory/json_dictionary/RMLIMTC0001a/mapping.ttl` & `morph_kgc-2.7.0/test/rml-in-memory/json_dictionary/RMLIMTC0001a/mapping.ttl`

 * *Files 12% similar despite different names*

```diff
@@ -1,40 +1,38 @@
-@prefix rr: <http://www.w3.org/ns/r2rml#> .
 @prefix foaf: <http://xmlns.com/foaf/0.1/> .
 @prefix ex: <http://example.com/> .
 @prefix xsd: <http://www.w3.org/2001/XMLSchema#> .
-@prefix rml: <http://semweb.mmlab.be/ns/rml#> .
-@prefix ql: <http://semweb.mmlab.be/ns/ql#> .
+@prefix rml: <http://w3id.org/rml/> .
 @prefix sd: <https://w3id.org/okn/o/sd#>.
 @prefix kg4di: <https://w3id.org/kg4di/definedBy>.
 @base <http://example.com/base/> .
 
 <TriplesMap1>
-  a rr:TriplesMap;
+  a rml:TriplesMap;
 
   rml:logicalSource [
     rml:source [
 			a sd:DatasetSpecification;
 			sd:name "variable1";
 			sd:hasDataTransformation [
 				sd:hasSourceCode [
 					sd:programmingLanguage "Python3.9";
 				];
 			];
 		];
-		rml:referenceFormulation ql:Dictionary;
+		rml:referenceFormulation rml:Dictionary;
     rml:iterator "$.students[*]"
   ];
 
-  rr:subjectMap <#NameSubjectMap> ;
+  rml:subjectMap <#NameSubjectMap> ;
 
-  rr:predicateObjectMap [
-    rr:predicate foaf:name;
-    rr:objectMap [
+  rml:predicateObjectMap [
+    rml:predicate foaf:name;
+    rml:objectMap [
       rml:reference "Name"
     ]
   ].
 
-<#NameSubjectMap> rr:template "http://example.com/{Name}" .
+<#NameSubjectMap> rml:template "http://example.com/{Name}" .
 
-ql:Dictionary a rml:ReferenceFormulation;
+rml:Dictionary a rml:ReferenceFormulation;
 	kg4di:definedBy "Python".
```

### Comparing `morph_kgc-2.6.4/test/rml-in-memory/json_dictionary/RMLIMTC0001a/test_RMLTC0001a_DICT.py` & `morph_kgc-2.7.0/test/rml-in-memory/json_dictionary/RMLIMTC0001a/test_RMLTC0001a_DICT.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/rml-in-memory/json_dictionary/RMLIMTC0001b/mapping.ttl` & `morph_kgc-2.7.0/test/rml-in-memory/json_dictionary/RMLIMTC0007h/mapping.ttl`

 * *Files 15% similar despite different names*

```diff
@@ -1,41 +1,38 @@
-@prefix rr: <http://www.w3.org/ns/r2rml#> .
 @prefix foaf: <http://xmlns.com/foaf/0.1/> .
 @prefix ex: <http://example.com/> .
 @prefix xsd: <http://www.w3.org/2001/XMLSchema#> .
-@prefix rml: <http://semweb.mmlab.be/ns/rml#> .
-@prefix ql: <http://semweb.mmlab.be/ns/ql#> .
+@prefix rml: <http://w3id.org/rml/> .
 @base <http://example.com/base/> .
 @prefix sd: <https://w3id.org/okn/o/sd#>.
 @prefix kg4di: <https://w3id.org/kg4di/definedBy>.
 
-<TriplesMap1>
-  a rr:TriplesMap;
+<TriplesMap1> a rml:TriplesMap;
 
   rml:logicalSource [
     rml:source [
 			a sd:DatasetSpecification;
 			sd:name "variable1";
 			sd:hasDataTransformation [
 				sd:hasSourceCode [
 					sd:programmingLanguage "Python3.9";
 				];
 			];
 		];
-		rml:referenceFormulation ql:Dictionary;
+		rml:referenceFormulation rml:Dictionary;
     rml:iterator "$.students[*]"
   ];
 
-  rr:subjectMap [
-    rr:template "{Name}";
-    rr:termType rr:BlankNode
+  rml:subjectMap [
+    rml:template "http://example.com/Student/{ID}/{FirstName}";
+    rml:graphMap [ rml:reference "FirstName"; rml:termType rml:Literal; ]
   ];
 
-  rr:predicateObjectMap [
-    rr:predicate foaf:name;
-    rr:objectMap [
-      rml:reference "Name"
+  rml:predicateObjectMap [
+    rml:predicate foaf:name;
+    rml:objectMap [
+      rml:reference "FirstName"
     ]
   ].
 
-ql:Dictionary a rml:ReferenceFormulation;
-	kg4di:definedBy "Python".
+rml:Dictionary a rml:ReferenceFormulation;
+	kg4di:definedBy "Python".
```

### Comparing `morph_kgc-2.6.4/test/rml-in-memory/json_dictionary/RMLIMTC0001b/test_RMLTC0001b_DICT.py` & `morph_kgc-2.7.0/test/rml-in-memory/json_dictionary/RMLIMTC0001b/test_RMLTC0001b_DICT.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/rml-in-memory/json_dictionary/RMLIMTC0002a/mapping.ttl` & `morph_kgc-2.7.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0010c/mapping.ttl`

 * *Files 16% similar despite different names*

```diff
@@ -1,43 +1,35 @@
-@prefix rr: <http://www.w3.org/ns/r2rml#> .
 @prefix foaf: <http://xmlns.com/foaf/0.1/> .
 @prefix ex: <http://example.com/> .
 @prefix xsd: <http://www.w3.org/2001/XMLSchema#> .
-@prefix rml: <http://semweb.mmlab.be/ns/rml#> .
-@prefix ql: <http://semweb.mmlab.be/ns/ql#> .
+@prefix rml: <http://w3id.org/rml/> .
+@prefix activity: <http://example.com/activity/> .
 @base <http://example.com/base/> .
 @prefix sd: <https://w3id.org/okn/o/sd#>.
 @prefix kg4di: <https://w3id.org/kg4di/definedBy>.
 
-<TriplesMap1> a rr:TriplesMap;
+<TriplesMap1>
+  a rml:TriplesMap;
 
   rml:logicalSource [
     rml:source [
 			a sd:DatasetSpecification;
 			sd:name "variable1";
 			sd:hasDataTransformation [
+				sd:hasSoftwareRequirements "pandas>=1.1.0";
 				sd:hasSourceCode [
 					sd:programmingLanguage "Python3.9";
 				];
 			];
 		];
-		rml:referenceFormulation ql:Dictionary;
-    rml:iterator "$.students[*]"
+    rml:referenceFormulation rml:DataFrame;
   ];
 
-  rr:subjectMap [
-    rr:template "http://example.com/{ID}/{Name}";
-    rr:class foaf:Person
-  ];
-
-  rr:predicateObjectMap [
-    rr:predicate ex:id ;
-    rr:objectMap [ rml:reference "ID" ]
-  ];
+  rml:subjectMap [ rml:template "http://example.com/{Country Code}/{Name}" ];
 
-  rr:predicateObjectMap [
-    rr:predicate foaf:name ;
-    rr:objectMap [ rml:reference "Name" ]
-  ].
+  rml:predicateObjectMap [
+    rml:predicate ex:code ;
+    rml:objectMap [ rml:template "\\{\\{\\{ {ISO 3166} \\}\\}\\}"; rml:termType rml:Literal]
+  ] .
 
-ql:Dictionary a rml:ReferenceFormulation;
-	kg4di:definedBy "Python".
+rml:DataFrame a rml:ReferenceFormulation;
+	kg4di:definedBy "Pandas".
```

### Comparing `morph_kgc-2.6.4/test/rml-in-memory/json_dictionary/RMLIMTC0002a/test_RMLTC0002a_DICT.py` & `morph_kgc-2.7.0/test/rml-in-memory/json_dictionary/RMLIMTC0002a/test_RMLTC0002a_DICT.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/rml-in-memory/json_dictionary/RMLIMTC0002b/mapping.ttl` & `morph_kgc-2.7.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0010a/mapping.ttl`

 * *Files 16% similar despite different names*

```diff
@@ -1,38 +1,35 @@
-@prefix rr: <http://www.w3.org/ns/r2rml#> .
 @prefix foaf: <http://xmlns.com/foaf/0.1/> .
 @prefix ex: <http://example.com/> .
 @prefix xsd: <http://www.w3.org/2001/XMLSchema#> .
-@prefix rml: <http://semweb.mmlab.be/ns/rml#> .
-@prefix ql: <http://semweb.mmlab.be/ns/ql#> .
+@prefix rml: <http://w3id.org/rml/> .
+@prefix activity: <http://example.com/activity/> .
 @base <http://example.com/base/> .
 @prefix sd: <https://w3id.org/okn/o/sd#>.
 @prefix kg4di: <https://w3id.org/kg4di/definedBy>.
 
-<TriplesMap1> a rr:TriplesMap;
+<TriplesMap1>
+  a rml:TriplesMap;
 
   rml:logicalSource [
     rml:source [
 			a sd:DatasetSpecification;
 			sd:name "variable1";
 			sd:hasDataTransformation [
+				sd:hasSoftwareRequirements "pandas>=1.1.0";
 				sd:hasSourceCode [
 					sd:programmingLanguage "Python3.9";
 				];
 			];
 		];
-		rml:referenceFormulation ql:Dictionary;
-    rml:iterator "$.students[*]"
+    rml:referenceFormulation rml:DataFrame;
   ];
 
-  rr:subjectMap [
-    rr:template "students{ID}";
-    rr:termType rr:BlankNode
-  ];
+  rml:subjectMap [ rml:template "http://example.com/{Country Code}" ];
 
-  rr:predicateObjectMap [
-    rr:predicate foaf:name;
-    rr:objectMap [ rml:reference "Name" ]
-  ].
+  rml:predicateObjectMap [
+    rml:predicate ex:name ;
+    rml:objectMap [ rml:reference "Name" ]
+  ] .
 
-ql:Dictionary a rml:ReferenceFormulation;
-	kg4di:definedBy "Python".
+rml:DataFrame a rml:ReferenceFormulation;
+	kg4di:definedBy "Pandas".
```

### Comparing `morph_kgc-2.6.4/test/rml-in-memory/json_dictionary/RMLIMTC0002b/test_RMLTC0002b_DICT.py` & `morph_kgc-2.7.0/test/rml-in-memory/json_dictionary/RMLIMTC0002b/test_RMLTC0002b_DICT.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/rml-in-memory/json_dictionary/RMLIMTC0002c/mapping.ttl` & `morph_kgc-2.7.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0010b/mapping.ttl`

 * *Files 16% similar despite different names*

```diff
@@ -1,37 +1,35 @@
-@prefix rr: <http://www.w3.org/ns/r2rml#> .
 @prefix foaf: <http://xmlns.com/foaf/0.1/> .
 @prefix ex: <http://example.com/> .
 @prefix xsd: <http://www.w3.org/2001/XMLSchema#> .
-@prefix rml: <http://semweb.mmlab.be/ns/rml#> .
-@prefix ql: <http://semweb.mmlab.be/ns/ql#> .
+@prefix rml: <http://w3id.org/rml/> .
+@prefix activity: <http://example.com/activity/> .
 @base <http://example.com/base/> .
 @prefix sd: <https://w3id.org/okn/o/sd#>.
 @prefix kg4di: <https://w3id.org/kg4di/definedBy>.
 
-<TriplesMap1> a rr:TriplesMap;
+<TriplesMap1>
+  a rml:TriplesMap;
 
   rml:logicalSource [
     rml:source [
 			a sd:DatasetSpecification;
 			sd:name "variable1";
 			sd:hasDataTransformation [
+				sd:hasSoftwareRequirements "pandas>=1.1.0";
 				sd:hasSourceCode [
 					sd:programmingLanguage "Python3.9";
 				];
 			];
 		];
-		rml:referenceFormulation ql:Dictionary;
-    rml:iterator "$.students[*]"
+    rml:referenceFormulation rml:DataFrame;
   ];
 
-  rr:subjectMap [
-    rr:template "http://example.com/{ID}/{Name}";
-  ];
+  rml:subjectMap [ rml:template "http://example.com/{Country Code}/{Name}" ];
 
-  rr:predicateObjectMap [
-    rr:predicate ex:id ;
-    rr:objectMap [ rml:reference "IDs" ]
-  ].
+  rml:predicateObjectMap [
+    rml:predicate ex:name ;
+    rml:objectMap [ rml:reference "Name" ]
+  ] .
 
-ql:Dictionary a rml:ReferenceFormulation;
-	kg4di:definedBy "Python".
+rml:DataFrame a rml:ReferenceFormulation;
+	kg4di:definedBy "Pandas".
```

### Comparing `morph_kgc-2.6.4/test/rml-in-memory/json_dictionary/RMLIMTC0002c/test_RMLTC0002c_DICT.py` & `morph_kgc-2.7.0/test/rml-in-memory/json_dictionary/RMLIMTC0002c/test_RMLTC0002c_DICT.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/rml-in-memory/json_dictionary/RMLIMTC0002e/mapping.ttl` & `morph_kgc-2.7.0/test/rml-in-memory/json_dictionary/RMLIMTC0010c/mapping.ttl`

 * *Files 17% similar despite different names*

```diff
@@ -1,37 +1,35 @@
-@prefix rr: <http://www.w3.org/ns/r2rml#> .
 @prefix foaf: <http://xmlns.com/foaf/0.1/> .
 @prefix ex: <http://example.com/> .
 @prefix xsd: <http://www.w3.org/2001/XMLSchema#> .
-@prefix rml: <http://semweb.mmlab.be/ns/rml#> .
-@prefix ql: <http://semweb.mmlab.be/ns/ql#> .
+@prefix rml: <http://w3id.org/rml/> .
+@prefix activity: <http://example.com/activity/> .
 @base <http://example.com/base/> .
 @prefix sd: <https://w3id.org/okn/o/sd#>.
 @prefix kg4di: <https://w3id.org/kg4di/definedBy>.
 
-<TriplesMap1> a rr:TriplesMap;
+<TriplesMap1>
+  a rml:TriplesMap;
 
   rml:logicalSource [
     rml:source [
 			a sd:DatasetSpecification;
 			sd:name "variable1";
 			sd:hasDataTransformation [
 				sd:hasSourceCode [
 					sd:programmingLanguage "Python3.9";
 				];
 			];
 		];
-		rml:referenceFormulation ql:Dictionary;
-    rml:iterator "$.students[*]"
+		rml:referenceFormulation rml:Dictionary;
+    rml:iterator "$.countries[*]"
   ];
 
-  rr:subjectMap [
-    rr:template "http://example.com/{ID}/{Name}";
-  ];
+  rml:subjectMap [ rml:template "http://example.com/{Country Code}/{Name}" ];
 
-  rr:predicateObjectMap [
-    rr:predicate ex:id ;
-    rr:objectMap [ rml:reference "ID" ]
-  ].
+  rml:predicateObjectMap [
+    rml:predicate ex:code ;
+    rml:objectMap [ rml:template "\\{\\{\\{ {ISO 3166} \\}\\}\\}"; rml:termType rml:Literal]
+  ] .
 
-ql:Dictionary a rml:ReferenceFormulation;
-	kg4di:definedBy "Python".
+rml:Dictionary a rml:ReferenceFormulation;
+	kg4di:definedBy "Python".
```

### Comparing `morph_kgc-2.6.4/test/rml-in-memory/json_dictionary/RMLIMTC0002e/test_RMLTC0002e_DICT.py` & `morph_kgc-2.7.0/test/rml-in-memory/json_dictionary/RMLIMTC0002e/test_RMLTC0002e_DICT.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/rml-in-memory/json_dictionary/RMLIMTC0003c/mapping.ttl` & `morph_kgc-2.7.0/test/rml-in-memory/json_dictionary/RMLIMTC0007g/mapping.ttl`

 * *Files 14% similar despite different names*

```diff
@@ -1,40 +1,38 @@
-@prefix rr: <http://www.w3.org/ns/r2rml#> .
 @prefix foaf: <http://xmlns.com/foaf/0.1/> .
 @prefix ex: <http://example.com/> .
 @prefix xsd: <http://www.w3.org/2001/XMLSchema#> .
-@prefix rml: <http://semweb.mmlab.be/ns/rml#> .
-@prefix ql: <http://semweb.mmlab.be/ns/ql#> .
+@prefix rml: <http://w3id.org/rml/> .
+@base <http://example.com/base/> .
 @prefix sd: <https://w3id.org/okn/o/sd#>.
 @prefix kg4di: <https://w3id.org/kg4di/definedBy>.
-@base <http://example.com/base/> .
 
-<TriplesMap1> a rr:TriplesMap;
+<TriplesMap1> a rml:TriplesMap;
 
   rml:logicalSource [
     rml:source [
 			a sd:DatasetSpecification;
 			sd:name "variable1";
 			sd:hasDataTransformation [
 				sd:hasSourceCode [
 					sd:programmingLanguage "Python3.9";
 				];
 			];
 		];
-    rml:referenceFormulation ql:Dictionary;
+		rml:referenceFormulation rml:Dictionary;
     rml:iterator "$.students[*]"
   ];
 
-  rr:subjectMap [
-    rr:template "http://example.com/Student{ID}";
+  rml:subjectMap [
+    rml:template "http://example.com/Student/{ID}/{FirstName}";
+    rml:graph rml:defaultGraph
   ];
 
-  rr:predicateObjectMap [
-    rr:predicate foaf:name ;
-    rr:objectMap [
-      rr:template "{FirstName} {LastName}";
-      rr:termType rr:Literal;
+  rml:predicateObjectMap [
+    rml:predicate foaf:name;
+    rml:objectMap [
+      rml:reference "FirstName"
     ]
   ].
 
-ql:Dictionary a rml:ReferenceFormulation;
-	kg4di:definedBy "Python".
+rml:Dictionary a rml:ReferenceFormulation;
+	kg4di:definedBy "Python".
```

### Comparing `morph_kgc-2.6.4/test/rml-in-memory/json_dictionary/RMLIMTC0003c/test_RMLTC0003c_DICT.py` & `morph_kgc-2.7.0/test/rml-in-memory/json_dictionary/RMLIMTC0003c/test_RMLTC0003c_DICT.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/rml-in-memory/json_dictionary/RMLIMTC0004a/mapping.ttl` & `morph_kgc-2.7.0/test/rml-in-memory/json_dictionary/RMLIMTC0004a/mapping.ttl`

 * *Files 9% similar despite different names*

```diff
@@ -1,69 +1,67 @@
-@prefix rr: <http://www.w3.org/ns/r2rml#> .
 @prefix foaf: <http://xmlns.com/foaf/0.1/> .
 @prefix ex: <http://example.com/> .
 @prefix xsd: <http://www.w3.org/2001/XMLSchema#> .
-@prefix rml: <http://semweb.mmlab.be/ns/rml#> .
-@prefix ql: <http://semweb.mmlab.be/ns/ql#> .
+@prefix rml: <http://w3id.org/rml/> .
 @base <http://example.com/base/> .
 @prefix sd: <https://w3id.org/okn/o/sd#>.
 @prefix kg4di: <https://w3id.org/kg4di/definedBy>.
 
-<TriplesMap1> a rr:TriplesMap;
+<TriplesMap1> a rml:TriplesMap;
 
   rml:logicalSource [
     rml:source [
 			a sd:DatasetSpecification;
 			sd:name "variable1";
 			sd:hasDataTransformation [
 				sd:hasSourceCode [
 					sd:programmingLanguage "Python3.9";
 				];
 			];
 		];
-		rml:referenceFormulation ql:Dictionary;
+		rml:referenceFormulation rml:Dictionary;
     rml:iterator "$.students[*]"
   ];
 
-  rr:subjectMap [
-    rr:template "http://example.com/{Student}";
-    rr:class ex:Student
+  rml:subjectMap [
+    rml:template "http://example.com/{Student}";
+    rml:class ex:Student
   ];
 
-  rr:predicateObjectMap [
-    rr:predicate foaf:name ;
-    rr:objectMap [
+  rml:predicateObjectMap [
+    rml:predicate foaf:name ;
+    rml:objectMap [
       rml:reference "Student"
     ]
   ].
 
-<TriplesMap2> a rr:TriplesMap;
+<TriplesMap2> a rml:TriplesMap;
 
   rml:logicalSource [
     rml:source [
 			a sd:DatasetSpecification;
 			sd:name "variable1";
 			sd:hasDataTransformation [
 				sd:hasSourceCode [
 					sd:programmingLanguage "Python3.9";
 				];
 			];
 		];
-		rml:referenceFormulation ql:Dictionary;
+		rml:referenceFormulation rml:Dictionary;
     rml:iterator "$.students[*]"
   ];
 
-  rr:subjectMap [
-    rr:template "http://example.com/{Sport}";
-    rr:class ex:Sport
+  rml:subjectMap [
+    rml:template "http://example.com/{Sport}";
+    rml:class ex:Sport
   ];
 
-  rr:predicateObjectMap [
-    rr:predicate foaf:name ;
-    rr:objectMap [
+  rml:predicateObjectMap [
+    rml:predicate foaf:name ;
+    rml:objectMap [
       rml:reference "Sport"
     ]
   ].
 
 
-ql:Dictionary a rml:ReferenceFormulation;
+rml:Dictionary a rml:ReferenceFormulation;
 	kg4di:definedBy "Python".
```

### Comparing `morph_kgc-2.6.4/test/rml-in-memory/json_dictionary/RMLIMTC0004a/test_RMLTC0004a_DICT.py` & `morph_kgc-2.7.0/test/rml-in-memory/json_dictionary/RMLIMTC0004a/test_RMLTC0004a_DICT.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/rml-in-memory/json_dictionary/RMLIMTC0004b/mapping.ttl` & `morph_kgc-2.7.0/test/rml-in-memory/json_dictionary/RMLIMTC0004b/mapping.ttl`

 * *Files 14% similar despite different names*

```diff
@@ -1,41 +1,39 @@
-@prefix rr: <http://www.w3.org/ns/r2rml#> .
 @prefix foaf: <http://xmlns.com/foaf/0.1/> .
 @prefix ex: <http://example.com/> .
 @prefix xsd: <http://www.w3.org/2001/XMLSchema#> .
-@prefix rml: <http://semweb.mmlab.be/ns/rml#> .
-@prefix ql: <http://semweb.mmlab.be/ns/ql#> .
+@prefix rml: <http://w3id.org/rml/> .
 @prefix sd: <https://w3id.org/okn/o/sd#>.
 @prefix kg4di: <https://w3id.org/kg4di/definedBy>.
 @base <http://example.com/base/> .
 
 <TriplesMap1>
-  a rr:TriplesMap;
+  a rml:TriplesMap;
 
   rml:logicalSource [
     rml:source [
 			a sd:DatasetSpecification;
 			sd:name "variable1";
 			sd:hasDataTransformation [
 				sd:hasSourceCode [
 					sd:programmingLanguage "Python3.9";
 				];
 			];
 		];
-		rml:referenceFormulation ql:Dictionary;
+		rml:referenceFormulation rml:Dictionary;
     rml:iterator "$.students[*]"
   ];
 
-  rr:subjectMap [
-    rr:template "http://example.com/{Name}";
-    rr:termType rr:Literal
+  rml:subjectMap [
+    rml:template "http://example.com/{Name}";
+    rml:termType rml:Literal
   ];
 
-  rr:predicateObjectMap [
-    rr:predicate foaf:name;
-    rr:objectMap [
+  rml:predicateObjectMap [
+    rml:predicate foaf:name;
+    rml:objectMap [
       rml:reference "Name"
     ]
   ].
 
-ql:Dictionary a rml:ReferenceFormulation;
+rml:Dictionary a rml:ReferenceFormulation;
 	kg4di:definedBy "Python".
```

### Comparing `morph_kgc-2.6.4/test/rml-in-memory/json_dictionary/RMLIMTC0004b/test_RMLTC0004b_DICT.py` & `morph_kgc-2.7.0/test/rml-in-memory/json_dictionary/RMLIMTC0004b/test_RMLTC0004b_DICT.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/rml-in-memory/json_dictionary/RMLIMTC0005a/mapping.ttl` & `morph_kgc-2.7.0/test/rml-in-memory/json_dictionary/RMLIMTC0002b/mapping.ttl`

 * *Files 16% similar despite different names*

```diff
@@ -1,38 +1,36 @@
-@prefix rr: <http://www.w3.org/ns/r2rml#> .
 @prefix foaf: <http://xmlns.com/foaf/0.1/> .
 @prefix ex: <http://example.com/> .
 @prefix xsd: <http://www.w3.org/2001/XMLSchema#> .
-@prefix rml: <http://semweb.mmlab.be/ns/rml#> .
-@prefix ql: <http://semweb.mmlab.be/ns/ql#> .
+@prefix rml: <http://w3id.org/rml/> .
 @base <http://example.com/base/> .
 @prefix sd: <https://w3id.org/okn/o/sd#>.
 @prefix kg4di: <https://w3id.org/kg4di/definedBy>.
 
-<TriplesMap1> a rr:TriplesMap;
+<TriplesMap1> a rml:TriplesMap;
 
   rml:logicalSource [
     rml:source [
 			a sd:DatasetSpecification;
 			sd:name "variable1";
 			sd:hasDataTransformation [
 				sd:hasSourceCode [
 					sd:programmingLanguage "Python3.9";
 				];
 			];
 		];
-		rml:referenceFormulation ql:Dictionary;
-    rml:iterator "$.persons[*]"
+		rml:referenceFormulation rml:Dictionary;
+    rml:iterator "$.students[*]"
   ];
 
-  rr:subjectMap [
-    rr:template "http://example.com/{fname};{lname}";
-    rr:class foaf:Person;
+  rml:subjectMap [
+    rml:template "students{ID}";
+    rml:termType rml:BlankNode
   ];
 
-  rr:predicateObjectMap [
-    rr:predicate ex:owes;
-    rr:objectMap [ rml:reference "amount"; ]
+  rml:predicateObjectMap [
+    rml:predicate foaf:name;
+    rml:objectMap [ rml:reference "Name" ]
   ].
 
-ql:Dictionary a rml:ReferenceFormulation;
+rml:Dictionary a rml:ReferenceFormulation;
 	kg4di:definedBy "Python".
```

### Comparing `morph_kgc-2.6.4/test/rml-in-memory/json_dictionary/RMLIMTC0005a/test_RMLTC0005a_DICT.py` & `morph_kgc-2.7.0/test/rml-in-memory/json_dictionary/RMLIMTC0005a/test_RMLTC0005a_DICT.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/rml-in-memory/json_dictionary/RMLIMTC0006a/mapping.ttl` & `morph_kgc-2.7.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0002a/mapping.ttl`

 * *Files 20% similar despite different names*

```diff
@@ -1,38 +1,41 @@
-@prefix rr: <http://www.w3.org/ns/r2rml#> .
 @prefix foaf: <http://xmlns.com/foaf/0.1/> .
 @prefix ex: <http://example.com/> .
 @prefix xsd: <http://www.w3.org/2001/XMLSchema#> .
-@prefix rml: <http://semweb.mmlab.be/ns/rml#> .
-@prefix ql: <http://semweb.mmlab.be/ns/ql#> .
+@prefix rml: <http://w3id.org/rml/> .
 @base <http://example.com/base/> .
 @prefix sd: <https://w3id.org/okn/o/sd#>.
 @prefix kg4di: <https://w3id.org/kg4di/definedBy>.
 
-<TriplesMap1> a rr:TriplesMap;
+<TriplesMap1> a rml:TriplesMap;
 
   rml:logicalSource [
     rml:source [
 			a sd:DatasetSpecification;
 			sd:name "variable1";
 			sd:hasDataTransformation [
+				sd:hasSoftwareRequirements "pandas>=1.1.0";
 				sd:hasSourceCode [
 					sd:programmingLanguage "Python3.9";
 				];
 			];
 		];
-		rml:referenceFormulation ql:Dictionary;
-    rml:iterator "$.students[*]"
+    rml:referenceFormulation rml:DataFrame;
   ];
 
-  rr:subjectMap [
-    rr:constant ex:BadStudent;
-    rr:graphMap [ rr:constant <http://example.com/graph/student> ];
+  rml:subjectMap [
+    rml:template "http://example.com/{ID}/{Name}";
+    rml:class foaf:Person
   ];
 
-  rr:predicateObjectMap [
-    rr:predicateMap [ rr:constant ex:description ];
-    rr:objectMap [ rr:constant "Bad Student"; ]
+  rml:predicateObjectMap [
+    rml:predicate ex:id ;
+    rml:objectMap [ rml:reference "ID" ]
+  ];
+
+  rml:predicateObjectMap [
+    rml:predicate foaf:name ;
+    rml:objectMap [ rml:reference "Name" ]
   ].
 
-ql:Dictionary a rml:ReferenceFormulation;
-	kg4di:definedBy "Python".
+rml:DataFrame a rml:ReferenceFormulation;
+	kg4di:definedBy "Pandas".
```

### Comparing `morph_kgc-2.6.4/test/rml-in-memory/json_dictionary/RMLIMTC0006a/test_RMLTC0006a_DICT.py` & `morph_kgc-2.7.0/test/rml-in-memory/json_dictionary/RMLIMTC0006a/test_RMLTC0006a_DICT.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/rml-in-memory/json_dictionary/RMLIMTC0007a/mapping.ttl` & `morph_kgc-2.7.0/test/rml-in-memory/json_dictionary/RMLIMTC0001b/mapping.ttl`

 * *Files 17% similar despite different names*

```diff
@@ -1,38 +1,39 @@
-@prefix rr: <http://www.w3.org/ns/r2rml#> .
 @prefix foaf: <http://xmlns.com/foaf/0.1/> .
 @prefix ex: <http://example.com/> .
 @prefix xsd: <http://www.w3.org/2001/XMLSchema#> .
-@prefix rml: <http://semweb.mmlab.be/ns/rml#> .
-@prefix ql: <http://semweb.mmlab.be/ns/ql#> .
-@prefix rdf: <http://www.w3.org/1999/02/22-rdf-syntax-ns#> .
+@prefix rml: <http://w3id.org/rml/> .
 @base <http://example.com/base/> .
 @prefix sd: <https://w3id.org/okn/o/sd#>.
 @prefix kg4di: <https://w3id.org/kg4di/definedBy>.
 
-<TriplesMap1> a rr:TriplesMap;
+<TriplesMap1>
+  a rml:TriplesMap;
 
   rml:logicalSource [
     rml:source [
 			a sd:DatasetSpecification;
 			sd:name "variable1";
 			sd:hasDataTransformation [
 				sd:hasSourceCode [
 					sd:programmingLanguage "Python3.9";
 				];
 			];
 		];
-		rml:referenceFormulation ql:Dictionary;
+		rml:referenceFormulation rml:Dictionary;
     rml:iterator "$.students[*]"
   ];
 
-  rr:subjectMap [
-    rr:template "http://example.com/Student/{ID}/{FirstName}"
+  rml:subjectMap [
+    rml:template "{Name}";
+    rml:termType rml:BlankNode
   ];
 
-  rr:predicateObjectMap [
-    rr:predicate rdf:type;
-    rr:object foaf:Person;
+  rml:predicateObjectMap [
+    rml:predicate foaf:name;
+    rml:objectMap [
+      rml:reference "Name"
+    ]
   ].
 
-ql:Dictionary a rml:ReferenceFormulation;
+rml:Dictionary a rml:ReferenceFormulation;
 	kg4di:definedBy "Python".
```

### Comparing `morph_kgc-2.6.4/test/rml-in-memory/json_dictionary/RMLIMTC0007a/test_RMLTC0007a_DICT.py` & `morph_kgc-2.7.0/test/rml-in-memory/json_dictionary/RMLIMTC0007a/test_RMLTC0007a_DICT.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/rml-in-memory/json_dictionary/RMLIMTC0007b/mapping.ttl` & `morph_kgc-2.7.0/test/rml-in-memory/json_dictionary/RMLIMTC0002c/mapping.ttl`

 * *Files 16% similar despite different names*

```diff
@@ -1,44 +1,35 @@
-@prefix rr: <http://www.w3.org/ns/r2rml#> .
 @prefix foaf: <http://xmlns.com/foaf/0.1/> .
 @prefix ex: <http://example.com/> .
 @prefix xsd: <http://www.w3.org/2001/XMLSchema#> .
-@prefix rml: <http://semweb.mmlab.be/ns/rml#> .
-@prefix ql: <http://semweb.mmlab.be/ns/ql#> .
-@prefix rdf: <http://www.w3.org/1999/02/22-rdf-syntax-ns#> .
+@prefix rml: <http://w3id.org/rml/> .
 @base <http://example.com/base/> .
 @prefix sd: <https://w3id.org/okn/o/sd#>.
 @prefix kg4di: <https://w3id.org/kg4di/definedBy>.
 
-<TriplesMap1> a rr:TriplesMap;
+<TriplesMap1> a rml:TriplesMap;
 
   rml:logicalSource [
     rml:source [
 			a sd:DatasetSpecification;
 			sd:name "variable1";
 			sd:hasDataTransformation [
 				sd:hasSourceCode [
 					sd:programmingLanguage "Python3.9";
 				];
 			];
 		];
-		rml:referenceFormulation ql:Dictionary;
+		rml:referenceFormulation rml:Dictionary;
     rml:iterator "$.students[*]"
   ];
 
-  rr:subjectMap [
-    rr:template "http://example.com/Student/{ID}/{FirstName}";
-    rr:graph ex:PersonGraph
+  rml:subjectMap [
+    rml:template "http://example.com/{ID}/{Name}";
   ];
 
-  rr:predicateObjectMap [
-    rr:predicate rdf:type;
-    rr:object foaf:Person;
-  ];
-
-  rr:predicateObjectMap [
-    rr:predicate foaf:name;
-    rr:objectMap [ rml:reference "FirstName" ]
+  rml:predicateObjectMap [
+    rml:predicate ex:id ;
+    rml:objectMap [ rml:reference "IDs" ]
   ].
 
-ql:Dictionary a rml:ReferenceFormulation;
+rml:Dictionary a rml:ReferenceFormulation;
 	kg4di:definedBy "Python".
```

### Comparing `morph_kgc-2.6.4/test/rml-in-memory/json_dictionary/RMLIMTC0007b/test_RMLTC0007b_DICT.py` & `morph_kgc-2.7.0/test/rml-in-memory/json_dictionary/RMLIMTC0007b/test_RMLTC0007b_DICT.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/rml-in-memory/json_dictionary/RMLIMTC0007c/mapping.ttl` & `morph_kgc-2.7.0/test/rml-in-memory/json_dictionary/RMLIMTC0002e/mapping.ttl`

 * *Files 14% similar despite different names*

```diff
@@ -1,43 +1,35 @@
-@prefix rr: <http://www.w3.org/ns/r2rml#> .
 @prefix foaf: <http://xmlns.com/foaf/0.1/> .
 @prefix ex: <http://example.com/> .
 @prefix xsd: <http://www.w3.org/2001/XMLSchema#> .
-@prefix rml: <http://semweb.mmlab.be/ns/rml#> .
-@prefix ql: <http://semweb.mmlab.be/ns/ql#> .
+@prefix rml: <http://w3id.org/rml/> .
 @base <http://example.com/base/> .
 @prefix sd: <https://w3id.org/okn/o/sd#>.
 @prefix kg4di: <https://w3id.org/kg4di/definedBy>.
 
-<TriplesMap1> a rr:TriplesMap;
+<TriplesMap1> a rml:TriplesMap;
 
   rml:logicalSource [
     rml:source [
 			a sd:DatasetSpecification;
 			sd:name "variable1";
 			sd:hasDataTransformation [
 				sd:hasSourceCode [
 					sd:programmingLanguage "Python3.9";
 				];
 			];
 		];
-		rml:referenceFormulation ql:Dictionary;
+		rml:referenceFormulation rml:Dictionary;
     rml:iterator "$.students[*]"
   ];
 
-  rr:subjectMap [
-    rr:template "http://example.com/Student/{ID}/{FirstName}";
-    rr:class foaf:Person, ex:Student
+  rml:subjectMap [
+    rml:template "http://example.com/{ID}/{Name}";
   ];
 
-  rr:predicateObjectMap [
-    rr:predicate ex:id ;
-    rr:objectMap [ rml:reference "ID";  ]
-  ];
-
-  rr:predicateObjectMap [
-    rr:predicate foaf:name;
-    rr:objectMap [ rml:reference "FirstName" ]
+  rml:predicateObjectMap [
+    rml:predicate ex:id ;
+    rml:objectMap [ rml:reference "ID" ]
   ].
 
-ql:Dictionary a rml:ReferenceFormulation;
+rml:Dictionary a rml:ReferenceFormulation;
 	kg4di:definedBy "Python".
```

### Comparing `morph_kgc-2.6.4/test/rml-in-memory/json_dictionary/RMLIMTC0007c/test_RMLTC0007c_DICT.py` & `morph_kgc-2.7.0/test/rml-in-memory/json_dictionary/RMLIMTC0007c/test_RMLTC0007c_DICT.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/rml-in-memory/json_dictionary/RMLIMTC0007d/mapping.ttl` & `morph_kgc-2.7.0/test/rml-in-memory/json_dictionary/RMLIMTC0002a/mapping.ttl`

 * *Files 15% similar despite different names*

```diff
@@ -1,53 +1,41 @@
-@prefix rr: <http://www.w3.org/ns/r2rml#> .
 @prefix foaf: <http://xmlns.com/foaf/0.1/> .
 @prefix ex: <http://example.com/> .
 @prefix xsd: <http://www.w3.org/2001/XMLSchema#> .
-@prefix rml: <http://semweb.mmlab.be/ns/rml#> .
-@prefix ql: <http://semweb.mmlab.be/ns/ql#> .
-@prefix rdf: <http://www.w3.org/1999/02/22-rdf-syntax-ns#> .
+@prefix rml: <http://w3id.org/rml/> .
 @base <http://example.com/base/> .
 @prefix sd: <https://w3id.org/okn/o/sd#>.
 @prefix kg4di: <https://w3id.org/kg4di/definedBy>.
 
-<TriplesMap1> a rr:TriplesMap;
+<TriplesMap1> a rml:TriplesMap;
 
   rml:logicalSource [
     rml:source [
 			a sd:DatasetSpecification;
 			sd:name "variable1";
 			sd:hasDataTransformation [
 				sd:hasSourceCode [
 					sd:programmingLanguage "Python3.9";
 				];
 			];
 		];
-		rml:referenceFormulation ql:Dictionary;
+		rml:referenceFormulation rml:Dictionary;
     rml:iterator "$.students[*]"
   ];
 
-  rr:subjectMap [
-    rr:template "http://example.com/Student/{ID}/{FirstName}"
+  rml:subjectMap [
+    rml:template "http://example.com/{ID}/{Name}";
+    rml:class foaf:Person
   ];
 
-  rr:predicateObjectMap [
-    rr:predicate rdf:type;
-    rr:object foaf:Person;
+  rml:predicateObjectMap [
+    rml:predicate ex:id ;
+    rml:objectMap [ rml:reference "ID" ]
   ];
 
-  rr:predicateObjectMap [
-    rr:predicate rdf:type;
-    rr:object ex:Student;
-  ];
-
-  rr:predicateObjectMap [
-    rr:predicate ex:id;
-    rr:objectMap [rml:reference "ID"]
-  ];
-
-  rr:predicateObjectMap [
-    rr:predicate foaf:name;
-    rr:objectMap [ rml:reference "FirstName" ]
+  rml:predicateObjectMap [
+    rml:predicate foaf:name ;
+    rml:objectMap [ rml:reference "Name" ]
   ].
 
-ql:Dictionary a rml:ReferenceFormulation;
+rml:Dictionary a rml:ReferenceFormulation;
 	kg4di:definedBy "Python".
```

### Comparing `morph_kgc-2.6.4/test/rml-in-memory/json_dictionary/RMLIMTC0007d/test_RMLTC0007d_DICT.py` & `morph_kgc-2.7.0/test/rml-in-memory/json_dictionary/RMLIMTC0007d/test_RMLTC0007d_DICT.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/rml-in-memory/json_dictionary/RMLIMTC0007e/mapping.ttl` & `morph_kgc-2.7.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0001a/mapping.ttl`

 * *Files 16% similar despite different names*

```diff
@@ -1,44 +1,39 @@
-@prefix rr: <http://www.w3.org/ns/r2rml#> .
 @prefix foaf: <http://xmlns.com/foaf/0.1/> .
 @prefix ex: <http://example.com/> .
 @prefix xsd: <http://www.w3.org/2001/XMLSchema#> .
-@prefix rml: <http://semweb.mmlab.be/ns/rml#> .
-@prefix ql: <http://semweb.mmlab.be/ns/ql#> .
-@base <http://example.com/base/> .
+@prefix rml: <http://w3id.org/rml/> .
 @prefix sd: <https://w3id.org/okn/o/sd#>.
 @prefix kg4di: <https://w3id.org/kg4di/definedBy>.
 
-<TriplesMap1> a rr:TriplesMap;
+@base <http://example.com/base/> .
+
+<TriplesMap1>
+  a rml:TriplesMap;
 
   rml:logicalSource [
     rml:source [
 			a sd:DatasetSpecification;
 			sd:name "variable1";
 			sd:hasDataTransformation [
+				sd:hasSoftwareRequirements "pandas>=1.1.0";
 				sd:hasSourceCode [
 					sd:programmingLanguage "Python3.9";
 				];
 			];
 		];
-		rml:referenceFormulation ql:Dictionary;
-    rml:iterator "$.students[*]"
-  ];
-
-  rr:subjectMap [
-    rr:template "http://example.com/Student/{ID}/{Name}";
-    rr:graph ex:PersonGraph ;
-    rr:class foaf:Person
+    rml:referenceFormulation rml:DataFrame
   ];
 
-  rr:predicateObjectMap [
-    rr:predicate ex:id ;
-    rr:objectMap [ rml:reference "ID"; ]
+  rml:subjectMap [
+    rml:template "http://example.com/{Name}"
   ];
 
-  rr:predicateObjectMap [
-    rr:predicate foaf:name ;
-    rr:objectMap [ rml:reference "Name" ]
+  rml:predicateObjectMap [
+    rml:predicate foaf:name;
+    rml:objectMap [
+      rml:reference "Name"
+    ]
   ].
 
-ql:Dictionary a rml:ReferenceFormulation;
-	kg4di:definedBy "Python".
+rml:DataFrame a rml:ReferenceFormulation;
+	kg4di:definedBy "Pandas".
```

### Comparing `morph_kgc-2.6.4/test/rml-in-memory/json_dictionary/RMLIMTC0007e/test_RMLTC0007e_DICT.py` & `morph_kgc-2.7.0/test/rml-in-memory/json_dictionary/RMLIMTC0007e/test_RMLTC0007e_DICT.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/rml-in-memory/json_dictionary/RMLIMTC0007f/mapping.ttl` & `morph_kgc-2.7.0/test/rml-in-memory/json_dictionary/RMLIMTC0008b/mapping.ttl`

 * *Files 17% similar despite different names*

```diff
@@ -1,49 +1,79 @@
-@prefix rr: <http://www.w3.org/ns/r2rml#> .
 @prefix foaf: <http://xmlns.com/foaf/0.1/> .
 @prefix ex: <http://example.com/> .
 @prefix xsd: <http://www.w3.org/2001/XMLSchema#> .
-@prefix rml: <http://semweb.mmlab.be/ns/rml#> .
-@prefix ql: <http://semweb.mmlab.be/ns/ql#> .
+@prefix rml: <http://w3id.org/rml/> .
+@prefix activity: <http://example.com/activity/> .
 @prefix rdf: <http://www.w3.org/1999/02/22-rdf-syntax-ns#> .
 @base <http://example.com/base/> .
 @prefix sd: <https://w3id.org/okn/o/sd#>.
 @prefix kg4di: <https://w3id.org/kg4di/definedBy>.
 
-<TriplesMap1> a rr:TriplesMap;
+<TriplesMap2>
+  a rml:TriplesMap;
+  rml:logicalSource [
+    rml:source [
+			a sd:DatasetSpecification;
+			sd:name "variable1";
+			sd:hasDataTransformation [
+				sd:hasSourceCode [
+					sd:programmingLanguage "Python3.9";
+				];
+			];
+		];
+		rml:referenceFormulation rml:Dictionary;
+    rml:iterator "$.students[*]"
+  ];
+
+  rml:subjectMap [ rml:template "http://example.com/{Sport}" ];
+
+  rml:predicateObjectMap [
+    rml:predicate rdf:type ;
+    rml:object activity:Sport ;
+  ] .
+
+<TriplesMap1>
+  a rml:TriplesMap;
 
   rml:logicalSource [
     rml:source [
 			a sd:DatasetSpecification;
 			sd:name "variable1";
 			sd:hasDataTransformation [
 				sd:hasSourceCode [
 					sd:programmingLanguage "Python3.9";
 				];
 			];
 		];
-		rml:referenceFormulation ql:Dictionary;
+		rml:referenceFormulation rml:Dictionary;
     rml:iterator "$.students[*]"
   ];
 
-  rr:subjectMap [
-    rr:template "http://example.com/Student/{ID}/{FirstName}";
-    rr:graph ex:PersonGraph
+  rml:subjectMap [ rml:template "http://example.com/Student/{ID}/{Name}" ];
+
+  rml:predicateObjectMap [
+    rml:predicate rdf:type ;
+    rml:object foaf:Person ;
   ];
 
-  rr:predicateObjectMap [
-    rr:predicate rdf:type;
-    rr:object foaf:Person
+  rml:predicateObjectMap [
+    rml:predicate ex:id ;
+    rml:objectMap [ rml:reference "ID"; ]
   ];
 
-  rr:predicateObjectMap [
-    rr:predicate ex:id ;
-    rr:objectMap [ rml:reference "ID";  ]
+  rml:predicateObjectMap [
+    rml:predicate foaf:name ;
+    rml:objectMap [ rml:reference "Name" ]
   ];
 
-  rr:predicateObjectMap [
-    rr:predicate foaf:name ;
-    rr:objectMap [ rml:reference "FirstName" ]
-  ].
+  rml:predicateObjectMap [
+    rml:predicate ex:Sport ;
+    rml:objectMap <RefObjectMap1>
+  ] .
+
+
+<RefObjectMap1>
+  a rml:RefObjectMap;
+  rml:parentTriplesMap <TriplesMap2> .
 
-ql:Dictionary a rml:ReferenceFormulation;
+rml:Dictionary a rml:ReferenceFormulation;
 	kg4di:definedBy "Python".
```

### Comparing `morph_kgc-2.6.4/test/rml-in-memory/json_dictionary/RMLIMTC0007f/test_RMLTC0007f_DICT.py` & `morph_kgc-2.7.0/test/rml-in-memory/json_dictionary/RMLIMTC0007f/test_RMLTC0007f_DICT.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/rml-in-memory/json_dictionary/RMLIMTC0007g/mapping.ttl` & `morph_kgc-2.7.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0007a/mapping.ttl`

 * *Files 17% similar despite different names*

```diff
@@ -1,40 +1,36 @@
-@prefix rr: <http://www.w3.org/ns/r2rml#> .
 @prefix foaf: <http://xmlns.com/foaf/0.1/> .
 @prefix ex: <http://example.com/> .
 @prefix xsd: <http://www.w3.org/2001/XMLSchema#> .
-@prefix rml: <http://semweb.mmlab.be/ns/rml#> .
-@prefix ql: <http://semweb.mmlab.be/ns/ql#> .
+@prefix rml: <http://w3id.org/rml/> .
+@prefix rdf: <http://www.w3.org/1999/02/22-rdf-syntax-ns#> .
 @base <http://example.com/base/> .
 @prefix sd: <https://w3id.org/okn/o/sd#>.
 @prefix kg4di: <https://w3id.org/kg4di/definedBy>.
 
-<TriplesMap1> a rr:TriplesMap;
+<TriplesMap1> a rml:TriplesMap;
 
   rml:logicalSource [
     rml:source [
 			a sd:DatasetSpecification;
 			sd:name "variable1";
 			sd:hasDataTransformation [
+				sd:hasSoftwareRequirements "pandas>=1.1.0";
 				sd:hasSourceCode [
 					sd:programmingLanguage "Python3.9";
 				];
 			];
 		];
-		rml:referenceFormulation ql:Dictionary;
-    rml:iterator "$.students[*]"
+    rml:referenceFormulation rml:DataFrame;
   ];
 
-  rr:subjectMap [
-    rr:template "http://example.com/Student/{ID}/{FirstName}";
-    rr:graph rr:defaultGraph
+  rml:subjectMap [
+    rml:template "http://example.com/Student/{ID}/{FirstName}"
   ];
 
-  rr:predicateObjectMap [
-    rr:predicate foaf:name;
-    rr:objectMap [
-      rml:reference "FirstName"
-    ]
+  rml:predicateObjectMap [
+    rml:predicate rdf:type;
+    rml:object foaf:Person;
   ].
 
-ql:Dictionary a rml:ReferenceFormulation;
-	kg4di:definedBy "Python".
+rml:DataFrame a rml:ReferenceFormulation;
+	kg4di:definedBy "Pandas".
```

### Comparing `morph_kgc-2.6.4/test/rml-in-memory/json_dictionary/RMLIMTC0007g/test_RMLTC0007g_DICT.py` & `morph_kgc-2.7.0/test/rml-in-memory/json_dictionary/RMLIMTC0007g/test_RMLTC0007g_DICT.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/rml-in-memory/json_dictionary/RMLIMTC0007h/mapping.ttl` & `morph_kgc-2.7.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0007h/mapping.ttl`

 * *Files 14% similar despite different names*

```diff
@@ -1,40 +1,38 @@
-@prefix rr: <http://www.w3.org/ns/r2rml#> .
 @prefix foaf: <http://xmlns.com/foaf/0.1/> .
 @prefix ex: <http://example.com/> .
 @prefix xsd: <http://www.w3.org/2001/XMLSchema#> .
-@prefix rml: <http://semweb.mmlab.be/ns/rml#> .
-@prefix ql: <http://semweb.mmlab.be/ns/ql#> .
+@prefix rml: <http://w3id.org/rml/> .
 @base <http://example.com/base/> .
 @prefix sd: <https://w3id.org/okn/o/sd#>.
 @prefix kg4di: <https://w3id.org/kg4di/definedBy>.
 
-<TriplesMap1> a rr:TriplesMap;
+<TriplesMap1> a rml:TriplesMap;
 
   rml:logicalSource [
     rml:source [
 			a sd:DatasetSpecification;
 			sd:name "variable1";
 			sd:hasDataTransformation [
+				sd:hasSoftwareRequirements "pandas>=1.1.0";
 				sd:hasSourceCode [
 					sd:programmingLanguage "Python3.9";
 				];
 			];
 		];
-		rml:referenceFormulation ql:Dictionary;
-    rml:iterator "$.students[*]"
+    rml:referenceFormulation rml:DataFrame;
   ];
 
-  rr:subjectMap [
-    rr:template "http://example.com/Student/{ID}/{FirstName}";
-    rr:graphMap [ rml:reference "FirstName"; rr:termType rr:Literal; ]
+  rml:subjectMap [
+    rml:template "http://example.com/Student/{ID}/{FirstName}";
+    rml:graphMap [ rml:reference "FirstName"; rml:termType rml:Literal; ]
   ];
 
-  rr:predicateObjectMap [
-    rr:predicate foaf:name;
-    rr:objectMap [
+  rml:predicateObjectMap [
+    rml:predicate foaf:name;
+    rml:objectMap [
       rml:reference "FirstName"
     ]
   ].
 
-ql:Dictionary a rml:ReferenceFormulation;
-	kg4di:definedBy "Python".
+rml:DataFrame a rml:ReferenceFormulation;
+	kg4di:definedBy "Pandas".
```

### Comparing `morph_kgc-2.6.4/test/rml-in-memory/json_dictionary/RMLIMTC0007h/test_RMLTC0007h_DICT.py` & `morph_kgc-2.7.0/test/rml-in-memory/json_dictionary/RMLIMTC0007h/test_RMLTC0007h_DICT.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/rml-in-memory/json_dictionary/RMLIMTC0008a/mapping.ttl` & `morph_kgc-2.7.0/test/rml-in-memory/json_dictionary/RMLIMTC0007d/mapping.ttl`

 * *Files 14% similar despite different names*

```diff
@@ -1,55 +1,51 @@
-@prefix rr: <http://www.w3.org/ns/r2rml#> .
 @prefix foaf: <http://xmlns.com/foaf/0.1/> .
 @prefix ex: <http://example.com/> .
 @prefix xsd: <http://www.w3.org/2001/XMLSchema#> .
-@prefix rml: <http://semweb.mmlab.be/ns/rml#> .
-@prefix ql: <http://semweb.mmlab.be/ns/ql#> .
+@prefix rml: <http://w3id.org/rml/> .
 @prefix rdf: <http://www.w3.org/1999/02/22-rdf-syntax-ns#> .
 @base <http://example.com/base/> .
 @prefix sd: <https://w3id.org/okn/o/sd#>.
 @prefix kg4di: <https://w3id.org/kg4di/definedBy>.
 
-<TriplesMap1>
-  a rr:TriplesMap;
+<TriplesMap1> a rml:TriplesMap;
 
   rml:logicalSource [
     rml:source [
 			a sd:DatasetSpecification;
 			sd:name "variable1";
 			sd:hasDataTransformation [
 				sd:hasSourceCode [
 					sd:programmingLanguage "Python3.9";
 				];
 			];
 		];
-		rml:referenceFormulation ql:Dictionary;
+		rml:referenceFormulation rml:Dictionary;
     rml:iterator "$.students[*]"
   ];
 
-  rr:subjectMap [
-    rr:template "http://example.com/Student/{ID}/{Name}";
-    rr:graphMap [ rr:template "http://example.com/graph/Student/{ID}/{Name}" ]
+  rml:subjectMap [
+    rml:template "http://example.com/Student/{ID}/{FirstName}"
   ];
 
-  rr:predicateObjectMap [
-    rr:predicate rdf:type ;
-    rr:object foaf:Person;
+  rml:predicateObjectMap [
+    rml:predicate rdf:type;
+    rml:object foaf:Person;
   ];
 
-  rr:predicateObjectMap [
-    rr:predicate ex:id ;
-    rr:objectMap [ rml:reference "ID" ]
+  rml:predicateObjectMap [
+    rml:predicate rdf:type;
+    rml:object ex:Student;
   ];
 
-  rr:predicateObjectMap [
-    rr:predicate foaf:name ;
-    rr:objectMap [ rml:reference "Name" ]
+  rml:predicateObjectMap [
+    rml:predicate ex:id;
+    rml:objectMap [rml:reference "ID"]
   ];
 
-  rr:predicateObjectMap [
-    rr:predicate ex:Sport ;
-    rr:objectMap [ rml:reference "Sport" ]
-  ] .
+  rml:predicateObjectMap [
+    rml:predicate foaf:name;
+    rml:objectMap [ rml:reference "FirstName" ]
+  ].
 
-ql:Dictionary a rml:ReferenceFormulation;
+rml:Dictionary a rml:ReferenceFormulation;
 	kg4di:definedBy "Python".
```

### Comparing `morph_kgc-2.6.4/test/rml-in-memory/json_dictionary/RMLIMTC0008a/output.nq` & `morph_kgc-2.7.0/test/rml-in-memory/json_dictionary/RMLIMTC0008a/output.nq`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/rml-in-memory/json_dictionary/RMLIMTC0008a/test_RMLTC0008a_DICT.py` & `morph_kgc-2.7.0/test/rml-in-memory/json_dictionary/RMLIMTC0008a/test_RMLTC0008a_DICT.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/rml-in-memory/json_dictionary/RMLIMTC0008b/mapping.ttl` & `morph_kgc-2.7.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0015b/mapping.ttl`

 * *Files 15% similar despite different names*

```diff
@@ -1,81 +1,65 @@
-@prefix rr: <http://www.w3.org/ns/r2rml#> .
 @prefix foaf: <http://xmlns.com/foaf/0.1/> .
+@prefix rdfs: <http://www.w3.org/2000/01/rdf-schema#> .
 @prefix ex: <http://example.com/> .
 @prefix xsd: <http://www.w3.org/2001/XMLSchema#> .
-@prefix rml: <http://semweb.mmlab.be/ns/rml#> .
-@prefix ql: <http://semweb.mmlab.be/ns/ql#> .
-@prefix activity: <http://example.com/activity/> .
-@prefix rdf: <http://www.w3.org/1999/02/22-rdf-syntax-ns#> .
-@base <http://example.com/base/> .
+@prefix rml: <http://w3id.org/rml/> .
 @prefix sd: <https://w3id.org/okn/o/sd#>.
 @prefix kg4di: <https://w3id.org/kg4di/definedBy>.
+@base <http://example.com/base/> .
+
+<TriplesMap1>
+  a rml:TriplesMap;
 
-<TriplesMap2>
-  a rr:TriplesMap;
   rml:logicalSource [
     rml:source [
 			a sd:DatasetSpecification;
 			sd:name "variable1";
 			sd:hasDataTransformation [
+				sd:hasSoftwareRequirements "pandas>=1.1.0";
 				sd:hasSourceCode [
 					sd:programmingLanguage "Python3.9";
 				];
 			];
 		];
-		rml:referenceFormulation ql:Dictionary;
-    rml:iterator "$.students[*]"
+    rml:referenceFormulation rml:DataFrame;
   ];
 
-  rr:subjectMap [ rr:template "http://example.com/{Sport}" ];
+  rml:subjectMap [ rml:template "http://example.com/{Code}" ];
 
-  rr:predicateObjectMap [
-    rr:predicate rdf:type ;
-    rr:object activity:Sport ;
+  rml:predicateObjectMap [
+    rml:predicate rdfs:label;
+    rml:objectMap [
+      rml:reference "Name";
+      rml:language "english"
+    ]
   ] .
 
-<TriplesMap1>
-  a rr:TriplesMap;
+<TriplesMap2>
+  a rml:TriplesMap;
 
   rml:logicalSource [
     rml:source [
 			a sd:DatasetSpecification;
-			sd:name "variable1";
+			sd:name "variable2";
 			sd:hasDataTransformation [
+				sd:hasSoftwareRequirements "pandas>=1.1.0";
 				sd:hasSourceCode [
 					sd:programmingLanguage "Python3.9";
 				];
 			];
 		];
-		rml:referenceFormulation ql:Dictionary;
-    rml:iterator "$.students[*]"
+    rml:referenceFormulation rml:DataFrame;
   ];
 
-  rr:subjectMap [ rr:template "http://example.com/Student/{ID}/{Name}" ];
-
-  rr:predicateObjectMap [
-    rr:predicate rdf:type ;
-    rr:object foaf:Person ;
-  ];
-
-  rr:predicateObjectMap [
-    rr:predicate ex:id ;
-    rr:objectMap [ rml:reference "ID"; ]
-  ];
-
-  rr:predicateObjectMap [
-    rr:predicate foaf:name ;
-    rr:objectMap [ rml:reference "Name" ]
-  ];
-
-  rr:predicateObjectMap [
-    rr:predicate ex:Sport ;
-    rr:objectMap <RefObjectMap1>
-  ] .
-
+  rml:subjectMap [ rml:template "http://example.com/{Code}" ];
 
-<RefObjectMap1>
-  a rr:RefObjectMap;
-  rr:parentTriplesMap <TriplesMap2> .
+  rml:predicateObjectMap [
+    rml:predicate rdfs:label;
+    rml:objectMap [
+      rml:reference "Name";
+      rml:language "spanish"
+    ]
+  ].
 
-ql:Dictionary a rml:ReferenceFormulation;
-	kg4di:definedBy "Python".
+rml:DataFrame a rml:ReferenceFormulation;
+	kg4di:definedBy "Pandas".
```

### Comparing `morph_kgc-2.6.4/test/rml-in-memory/json_dictionary/RMLIMTC0008b/output.nq` & `morph_kgc-2.7.0/test/rml-in-memory/json_dictionary/RMLIMTC0008b/output.nq`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/rml-in-memory/json_dictionary/RMLIMTC0008b/test_RMLTC0008b_DICT.py` & `morph_kgc-2.7.0/test/rml-in-memory/json_dictionary/RMLIMTC0008b/test_RMLTC0008b_DICT.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/rml-in-memory/json_dictionary/RMLIMTC0008c/mapping.ttl` & `morph_kgc-2.7.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0007f/mapping.ttl`

 * *Files 19% similar despite different names*

```diff
@@ -1,38 +1,47 @@
-@prefix rr: <http://www.w3.org/ns/r2rml#> .
 @prefix foaf: <http://xmlns.com/foaf/0.1/> .
 @prefix ex: <http://example.com/> .
 @prefix xsd: <http://www.w3.org/2001/XMLSchema#> .
-@prefix rml: <http://semweb.mmlab.be/ns/rml#> .
-@prefix ql: <http://semweb.mmlab.be/ns/ql#> .
-@prefix activity: <http://example.com/activity/> .
+@prefix rml: <http://w3id.org/rml/> .
+@prefix rdf: <http://www.w3.org/1999/02/22-rdf-syntax-ns#> .
 @base <http://example.com/base/> .
 @prefix sd: <https://w3id.org/okn/o/sd#>.
 @prefix kg4di: <https://w3id.org/kg4di/definedBy>.
 
-<TriplesMap1>
-  a rr:TriplesMap;
+<TriplesMap1> a rml:TriplesMap;
 
   rml:logicalSource [
     rml:source [
 			a sd:DatasetSpecification;
 			sd:name "variable1";
 			sd:hasDataTransformation [
+				sd:hasSoftwareRequirements "pandas>=1.1.0";
 				sd:hasSourceCode [
 					sd:programmingLanguage "Python3.9";
 				];
 			];
 		];
-		rml:referenceFormulation ql:Dictionary;
-    rml:iterator "$.students[*]"
+    rml:referenceFormulation rml:DataFrame;
   ];
 
-  rr:subjectMap [ rr:template "http://example.com/Student/{ID}/{Name}" ];
+  rml:subjectMap [
+    rml:template "http://example.com/Student/{ID}/{FirstName}";
+    rml:graph ex:PersonGraph
+  ];
+
+  rml:predicateObjectMap [
+    rml:predicate rdf:type;
+    rml:object foaf:Person
+  ];
+
+  rml:predicateObjectMap [
+    rml:predicate ex:id ;
+    rml:objectMap [ rml:reference "ID";  ]
+  ];
 
-  rr:predicateObjectMap [
-    rr:predicate foaf:name ;
-    rr:predicate ex:name ;
-    rr:objectMap [ rml:reference "Name" ]
-  ] .
+  rml:predicateObjectMap [
+    rml:predicate foaf:name ;
+    rml:objectMap [ rml:reference "FirstName" ]
+  ].
 
-ql:Dictionary a rml:ReferenceFormulation;
-	kg4di:definedBy "Python".
+rml:DataFrame a rml:ReferenceFormulation;
+	kg4di:definedBy "Pandas".
```

### Comparing `morph_kgc-2.6.4/test/rml-in-memory/json_dictionary/RMLIMTC0008c/test_RMLTC0008c_DICT.py` & `morph_kgc-2.7.0/test/rml-in-memory/json_dictionary/RMLIMTC0008c/test_RMLTC0008c_DICT.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/rml-in-memory/json_dictionary/RMLIMTC0009a/mapping.ttl` & `morph_kgc-2.7.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0009b/mapping.ttl`

 * *Files 12% similar despite different names*

```diff
@@ -1,74 +1,82 @@
-@prefix rr: <http://www.w3.org/ns/r2rml#> .
 @prefix foaf: <http://xmlns.com/foaf/0.1/> .
 @prefix ex: <http://example.com/> .
 @prefix xsd: <http://www.w3.org/2001/XMLSchema#> .
-@prefix rml: <http://semweb.mmlab.be/ns/rml#> .
-@prefix ql: <http://semweb.mmlab.be/ns/ql#> .
+@prefix rml: <http://w3id.org/rml/> .
 @prefix activity: <http://example.com/activity/> .
 @prefix rdfs: <http://www.w3.org/2000/01/rdf-schema#> .
 @base <http://example.com/base/> .
 @prefix sd: <https://w3id.org/okn/o/sd#>.
 @prefix kg4di: <https://w3id.org/kg4di/definedBy>.
 
 <TriplesMap1>
-  a rr:TriplesMap;
+  a rml:TriplesMap;
 
   rml:logicalSource [
     rml:source [
 			a sd:DatasetSpecification;
-			sd:name "variable2";
+			sd:name "variable1";
 			sd:hasDataTransformation [
+				sd:hasSoftwareRequirements "pandas>=1.1.0";
 				sd:hasSourceCode [
 					sd:programmingLanguage "Python3.9";
 				];
 			];
 		];
-		rml:referenceFormulation ql:Dictionary;
-    rml:iterator "$.students[*]"
+    rml:referenceFormulation rml:DataFrame;
   ];
 
-  rr:subjectMap [ rr:template "http://example.com/resource/student_{ID}" ];
+  rml:subjectMap [
+    rml:template "http://example.com/resource/student_{ID}" ;
+    rml:class <http://example.com/ontology/Student>;
+    rml:graph <http://example.com/graph/students> ;
+  ];
 
-  rr:predicateObjectMap [
-    rr:predicate foaf:name ;
-    rr:objectMap [ rml:reference "Name" ]
+  rml:predicateObjectMap [
+    rml:predicate foaf:name ;
+    rml:objectMap [ rml:reference "Name" ];
+    rml:graph <http://example.com/graph/students> ;
   ] ;
 
-  rr:predicateObjectMap [
-    rr:predicate <http://example.com/ontology/practises> ;
-    rr:objectMap [
-      a rr:RefObjectMap ;
-      rr:parentTriplesMap <TriplesMap2>;
-      rr:joinCondition [
-        rr:child "Sport" ;
-        rr:parent "ID" ;
+  rml:predicateObjectMap [
+    rml:predicate <http://example.com/ontology/practises> ;
+    rml:objectMap [
+      a rml:RefObjectMap ;
+      rml:parentTriplesMap <TriplesMap2>;
+      rml:joinCondition [
+        rml:child "Sport" ;
+        rml:parent "ID" ;
       ]
-    ]
+    ];
+    rml:graph <http://example.com/graph/practise> ;
   ] .
 
 <TriplesMap2>
-  a rr:TriplesMap;
+  a rml:TriplesMap;
 
   rml:logicalSource [
     rml:source [
 			a sd:DatasetSpecification;
-			sd:name "variable1";
+			sd:name "variable2";
 			sd:hasDataTransformation [
+				sd:hasSoftwareRequirements "pandas>=1.1.0";
 				sd:hasSourceCode [
 					sd:programmingLanguage "Python3.9";
 				];
 			];
 		];
-		rml:referenceFormulation ql:Dictionary;
-    rml:iterator "$.sports[*]"
+    rml:referenceFormulation rml:CSV
   ];
 
-  rr:subjectMap [ rr:template "http://example.com/resource/sport_{ID}" ];
+  rml:subjectMap [
+    rml:template "http://example.com/resource/sport_{ID}";
+    rml:class <http://example.com/ontology/Sport>;
+    rml:graph <http://example.com/graph/sports> ;
+  ];
 
-  rr:predicateObjectMap [
-    rr:predicate rdfs:label ;
-    rr:objectMap [ rml:reference "Name" ];
+  rml:predicateObjectMap [
+    rml:predicate rdfs:label ;
+    rml:objectMap [ rml:reference "Name" ];
   ].
 
-ql:Dictionary a rml:ReferenceFormulation;
-	kg4di:definedBy "Python".
+rml:DataFrame a rml:ReferenceFormulation;
+	kg4di:definedBy "Pandas".
```

### Comparing `morph_kgc-2.6.4/test/rml-in-memory/json_dictionary/RMLIMTC0009a/test_RMLTC0009a_DICT.py` & `morph_kgc-2.7.0/test/rml-in-memory/json_dictionary/RMLIMTC0009a/test_RMLTC0009a_DICT.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/rml-in-memory/json_dictionary/RMLIMTC0009b/mapping.ttl` & `morph_kgc-2.7.0/test/rml-in-memory/json_dictionary/RMLIMTC0015b/mapping.ttl`

 * *Files 20% similar despite different names*

```diff
@@ -1,82 +1,65 @@
-@prefix rr: <http://www.w3.org/ns/r2rml#> .
 @prefix foaf: <http://xmlns.com/foaf/0.1/> .
+@prefix rdfs: <http://www.w3.org/2000/01/rdf-schema#> .
 @prefix ex: <http://example.com/> .
 @prefix xsd: <http://www.w3.org/2001/XMLSchema#> .
-@prefix rml: <http://semweb.mmlab.be/ns/rml#> .
-@prefix ql: <http://semweb.mmlab.be/ns/ql#> .
-@prefix activity: <http://example.com/activity/> .
-@prefix rdfs: <http://www.w3.org/2000/01/rdf-schema#> .
-@base <http://example.com/base/> .
+@prefix rml: <http://w3id.org/rml/> .
 @prefix sd: <https://w3id.org/okn/o/sd#>.
 @prefix kg4di: <https://w3id.org/kg4di/definedBy>.
+@base <http://example.com/base/> .
 
 <TriplesMap1>
-  a rr:TriplesMap;
+  a rml:TriplesMap;
 
   rml:logicalSource [
     rml:source [
 			a sd:DatasetSpecification;
-			sd:name "variable2";
+			sd:name "variable1";
 			sd:hasDataTransformation [
 				sd:hasSourceCode [
 					sd:programmingLanguage "Python3.9";
 				];
 			];
 		];
-		rml:referenceFormulation ql:Dictionary;
-    rml:iterator "$.students[*]"
+		rml:referenceFormulation rml:Dictionary;
+    rml:iterator "$.countries[*]"
   ];
 
-  rr:subjectMap [ rr:template "http://example.com/resource/student_{ID}";
-    rr:class <http://example.com/ontology/Student>;
-    rr:graph <http://example.com/graph/students> ;
- ];
-
-  rr:predicateObjectMap [
-    rr:predicate foaf:name ;
-    rr:objectMap [ rml:reference "Name" ];
-    rr:graph <http://example.com/graph/students> ;
-  ] ;
-
-  rr:predicateObjectMap [
-    rr:predicate <http://example.com/ontology/practises> ;
-    rr:objectMap [
-      a rr:RefObjectMap ;
-      rr:parentTriplesMap <TriplesMap2>;
-      rr:joinCondition [
-        rr:child "Sport" ;
-        rr:parent "ID" ;
-      ]
-    ];
-    rr:graph <http://example.com/graph/practise> ;
+  rml:subjectMap [ rml:template "http://example.com/{Code}" ];
+
+  rml:predicateObjectMap [
+    rml:predicate rdfs:label;
+    rml:objectMap [
+      rml:reference "Name";
+      rml:language "english"
+    ]
   ] .
 
 <TriplesMap2>
-  a rr:TriplesMap;
+  a rml:TriplesMap;
 
   rml:logicalSource [
     rml:source [
 			a sd:DatasetSpecification;
-			sd:name "variable1";
+			sd:name "variable2";
 			sd:hasDataTransformation [
 				sd:hasSourceCode [
 					sd:programmingLanguage "Python3.9";
 				];
 			];
 		];
-		rml:referenceFormulation ql:Dictionary;
-    rml:iterator "$.sports[*]"
+		rml:referenceFormulation rml:Dictionary;
+    rml:iterator "$.countries[*]"
   ];
 
-  rr:subjectMap [ rr:template "http://example.com/resource/sport_{ID}";
-    rr:class <http://example.com/ontology/Sport>;
-    rr:graph <http://example.com/graph/sports> ;
-  ];
+  rml:subjectMap [ rml:template "http://example.com/{Code}" ];
 
-  rr:predicateObjectMap [
-    rr:predicate rdfs:label ;
-    rr:objectMap [ rml:reference "Name" ];
+  rml:predicateObjectMap [
+    rml:predicate rdfs:label;
+    rml:objectMap [
+      rml:reference "Name";
+      rml:language "spanish"
+    ]
   ].
 
-ql:Dictionary a rml:ReferenceFormulation;
+rml:Dictionary a rml:ReferenceFormulation;
 	kg4di:definedBy "Python".
```

### Comparing `morph_kgc-2.6.4/test/rml-in-memory/json_dictionary/RMLIMTC0009b/output.nq` & `morph_kgc-2.7.0/test/rml-in-memory/json_dictionary/RMLIMTC0009b/output.nq`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/rml-in-memory/json_dictionary/RMLIMTC0009b/test_RMLTC0009b_DICT.py` & `morph_kgc-2.7.0/test/rml-in-memory/json_dictionary/RMLIMTC0009b/test_RMLTC0009b_DICT.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/rml-in-memory/json_dictionary/RMLIMTC0010a/mapping.ttl` & `morph_kgc-2.7.0/test/rml-in-memory/json_dictionary/RMLIMTC0010b/mapping.ttl`

 * *Files 9% similar despite different names*

```diff
@@ -1,37 +1,35 @@
-@prefix rr: <http://www.w3.org/ns/r2rml#> .
 @prefix foaf: <http://xmlns.com/foaf/0.1/> .
 @prefix ex: <http://example.com/> .
 @prefix xsd: <http://www.w3.org/2001/XMLSchema#> .
-@prefix rml: <http://semweb.mmlab.be/ns/rml#> .
-@prefix ql: <http://semweb.mmlab.be/ns/ql#> .
+@prefix rml: <http://w3id.org/rml/> .
 @prefix activity: <http://example.com/activity/> .
 @base <http://example.com/base/> .
 @prefix sd: <https://w3id.org/okn/o/sd#>.
 @prefix kg4di: <https://w3id.org/kg4di/definedBy>.
 
 <TriplesMap1>
-  a rr:TriplesMap;
+  a rml:TriplesMap;
 
   rml:logicalSource [
     rml:source [
 			a sd:DatasetSpecification;
 			sd:name "variable1";
 			sd:hasDataTransformation [
 				sd:hasSourceCode [
 					sd:programmingLanguage "Python3.9";
 				];
 			];
 		];
-		rml:referenceFormulation ql:Dictionary;
+		rml:referenceFormulation rml:Dictionary;
     rml:iterator "$.countries[*]"
   ];
 
-  rr:subjectMap [ rr:template "http://example.com/{Country Code}" ];
+  rml:subjectMap [ rml:template "http://example.com/{Country Code}/{Name}" ];
 
-  rr:predicateObjectMap [
-    rr:predicate ex:name ;
-    rr:objectMap [ rml:reference "Name" ]
+  rml:predicateObjectMap [
+    rml:predicate ex:name ;
+    rml:objectMap [ rml:reference "Name" ]
   ] .
 
-ql:Dictionary a rml:ReferenceFormulation;
+rml:Dictionary a rml:ReferenceFormulation;
 	kg4di:definedBy "Python".
```

### Comparing `morph_kgc-2.6.4/test/rml-in-memory/json_dictionary/RMLIMTC0010a/test_RMLTC0010a_DICT.py` & `morph_kgc-2.7.0/test/rml-in-memory/json_dictionary/RMLIMTC0010a/test_RMLTC0010a_DICT.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/rml-in-memory/json_dictionary/RMLIMTC0010b/mapping.ttl` & `morph_kgc-2.7.0/test/rml-in-memory/json_dictionary/RMLIMTC0010a/mapping.ttl`

 * *Files 9% similar despite different names*

```diff
@@ -1,37 +1,35 @@
-@prefix rr: <http://www.w3.org/ns/r2rml#> .
 @prefix foaf: <http://xmlns.com/foaf/0.1/> .
 @prefix ex: <http://example.com/> .
 @prefix xsd: <http://www.w3.org/2001/XMLSchema#> .
-@prefix rml: <http://semweb.mmlab.be/ns/rml#> .
-@prefix ql: <http://semweb.mmlab.be/ns/ql#> .
+@prefix rml: <http://w3id.org/rml/> .
 @prefix activity: <http://example.com/activity/> .
 @base <http://example.com/base/> .
 @prefix sd: <https://w3id.org/okn/o/sd#>.
 @prefix kg4di: <https://w3id.org/kg4di/definedBy>.
 
 <TriplesMap1>
-  a rr:TriplesMap;
+  a rml:TriplesMap;
 
   rml:logicalSource [
     rml:source [
 			a sd:DatasetSpecification;
 			sd:name "variable1";
 			sd:hasDataTransformation [
 				sd:hasSourceCode [
 					sd:programmingLanguage "Python3.9";
 				];
 			];
 		];
-		rml:referenceFormulation ql:Dictionary;
+		rml:referenceFormulation rml:Dictionary;
     rml:iterator "$.countries[*]"
   ];
 
-  rr:subjectMap [ rr:template "http://example.com/{Country Code}/{Name}" ];
+  rml:subjectMap [ rml:template "http://example.com/{Country Code}" ];
 
-  rr:predicateObjectMap [
-    rr:predicate ex:name ;
-    rr:objectMap [ rml:reference "Name" ]
+  rml:predicateObjectMap [
+    rml:predicate ex:name ;
+    rml:objectMap [ rml:reference "Name" ]
   ] .
 
-ql:Dictionary a rml:ReferenceFormulation;
+rml:Dictionary a rml:ReferenceFormulation;
 	kg4di:definedBy "Python".
```

### Comparing `morph_kgc-2.6.4/test/rml-in-memory/json_dictionary/RMLIMTC0010b/test_RMLTC0010b_DICT.py` & `morph_kgc-2.7.0/test/rml-in-memory/json_dictionary/RMLIMTC0010b/test_RMLTC0010b_DICT.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/rml-in-memory/json_dictionary/RMLIMTC0010c/mapping.ttl` & `morph_kgc-2.7.0/test/rml-in-memory/json_dictionary/RMLIMTC0012d/mapping.ttl`

 * *Files 23% similar despite different names*

```diff
@@ -1,37 +1,46 @@
-@prefix rr: <http://www.w3.org/ns/r2rml#> .
 @prefix foaf: <http://xmlns.com/foaf/0.1/> .
 @prefix ex: <http://example.com/> .
 @prefix xsd: <http://www.w3.org/2001/XMLSchema#> .
-@prefix rml: <http://semweb.mmlab.be/ns/rml#> .
-@prefix ql: <http://semweb.mmlab.be/ns/ql#> .
-@prefix activity: <http://example.com/activity/> .
-@base <http://example.com/base/> .
+@prefix rml: <http://w3id.org/rml/> .
 @prefix sd: <https://w3id.org/okn/o/sd#>.
 @prefix kg4di: <https://w3id.org/kg4di/definedBy>.
+@base <http://example.com/base/> .
 
 <TriplesMap1>
-  a rr:TriplesMap;
+  a rml:TriplesMap;
 
   rml:logicalSource [
     rml:source [
 			a sd:DatasetSpecification;
 			sd:name "variable1";
 			sd:hasDataTransformation [
 				sd:hasSourceCode [
 					sd:programmingLanguage "Python3.9";
 				];
 			];
 		];
-		rml:referenceFormulation ql:Dictionary;
-    rml:iterator "$.countries[*]"
+		rml:referenceFormulation rml:Dictionary;
+    rml:iterator "$.persons[*]"
   ];
 
-  rr:subjectMap [ rr:template "http://example.com/{Country Code}/{Name}" ];
+  rml:subjectMap [ rml:template "{fname}_{lname}_{amount}"; rml:termType rml:BlankNode; ];
+
+  rml:subjectMap [ rml:template "{amount}_{fname}_{lname}"; rml:termType rml:BlankNode; ];
+
+  rml:predicateObjectMap [
+    rml:predicate foaf:name ;
+    rml:objectMap [
+      rml:template "{fname} {lname}";
+      rml:termType rml:Literal ;
+    ]
+  ];
 
-  rr:predicateObjectMap [
-    rr:predicate ex:code ;
-    rr:objectMap [ rr:template "\\{\\{\\{ {ISO 3166} \\}\\}\\}"; rr:termType rr:Literal]
-  ] .
+  rml:predicateObjectMap [
+    rml:predicate ex:amount ;
+    rml:objectMap    [
+      rml:reference "amount";
+    ]
+  ].
 
-ql:Dictionary a rml:ReferenceFormulation;
+rml:Dictionary a rml:ReferenceFormulation;
 	kg4di:definedBy "Python".
```

### Comparing `morph_kgc-2.6.4/test/rml-in-memory/json_dictionary/RMLIMTC0010c/test_RMLTC0010c_DICT.py` & `morph_kgc-2.7.0/test/rml-in-memory/json_dictionary/RMLIMTC0010c/test_RMLTC0010c_DICT.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/rml-in-memory/json_dictionary/RMLIMTC0011b/mapping.ttl` & `morph_kgc-2.7.0/test/rml-in-memory/json_dictionary/RMLIMTC0011b/mapping.ttl`

 * *Files 8% similar despite different names*

```diff
@@ -1,110 +1,108 @@
-@prefix rr: <http://www.w3.org/ns/r2rml#> .
 @prefix foaf: <http://xmlns.com/foaf/0.1/> .
 @prefix ex: <http://example.com/> .
 @prefix xsd: <http://www.w3.org/2001/XMLSchema#> .
-@prefix rml: <http://semweb.mmlab.be/ns/rml#> .
-@prefix ql: <http://semweb.mmlab.be/ns/ql#> .
+@prefix rml: <http://w3id.org/rml/> .
 @prefix sd: <https://w3id.org/okn/o/sd#>.
 @prefix kg4di: <https://w3id.org/kg4di/definedBy>.
 @base <http://example.com/base/> .
 
 <TriplesMap1>
-  a rr:TriplesMap;
+  a rml:TriplesMap;
 
   rml:logicalSource [
     rml:source [
 			a sd:DatasetSpecification;
 			sd:name "variable3";
 			sd:hasDataTransformation [
 				sd:hasSourceCode [
 					sd:programmingLanguage "Python3.9";
 				];
 			];
 		];
-		rml:referenceFormulation ql:Dictionary;
+		rml:referenceFormulation rml:Dictionary;
     rml:iterator "$.students[*]"
   ];
 
-  rr:subjectMap [
-    rr:template "http://example.com/student/{ID}";
+  rml:subjectMap [
+    rml:template "http://example.com/student/{ID}";
   ];
 
-  rr:predicateObjectMap [
-    rr:predicate ex:firstName;
-    rr:objectMap [
+  rml:predicateObjectMap [
+    rml:predicate ex:firstName;
+    rml:objectMap [
       rml:reference "FirstName"
     ]
   ];
 
-  rr:predicateObjectMap [
-    rr:predicate ex:lastName;
-    rr:objectMap [
+  rml:predicateObjectMap [
+    rml:predicate ex:lastName;
+    rml:objectMap [
       rml:reference "LastName"
     ]
   ].
 
 <TriplesMap2>
-  a rr:TriplesMap;
+  a rml:TriplesMap;
 
   rml:logicalSource [
     rml:source [
 			a sd:DatasetSpecification;
 			sd:name "variable1";
 			sd:hasDataTransformation [
 				sd:hasSourceCode [
 					sd:programmingLanguage "Python3.9";
 				];
 			];
 		];
-		rml:referenceFormulation ql:Dictionary;
+		rml:referenceFormulation rml:Dictionary;
     rml:iterator "$.sports[*]"
   ];
 
-  rr:subjectMap [
-    rr:template "http://example.com/sport/{ID}";
+  rml:subjectMap [
+    rml:template "http://example.com/sport/{ID}";
   ];
 
-  rr:predicateObjectMap [
-    rr:predicate ex:id;
-    rr:objectMap [
+  rml:predicateObjectMap [
+    rml:predicate ex:id;
+    rml:objectMap [
       rml:reference "ID"
     ]
   ];
 
-  rr:predicateObjectMap [
-    rr:predicate ex:description;
-    rr:objectMap [
+  rml:predicateObjectMap [
+    rml:predicate ex:description;
+    rml:objectMap [
       rml:reference "Description"
     ]
   ].
 
 <LinkMap_1_2>
-  a rr:TriplesMap;
+  a rml:TriplesMap;
 
   rml:logicalSource [
     rml:source [
 			a sd:DatasetSpecification;
 			sd:name "variable2";
 			sd:hasDataTransformation [
 				sd:hasSourceCode [
 					sd:programmingLanguage "Python3.9";
 				];
 			];
 		];
-		rml:referenceFormulation ql:Dictionary;
+		rml:referenceFormulation rml:Dictionary;
     rml:iterator "$.links[*]"
   ];
 
-  rr:subjectMap [
-    rr:template "http://example.com/student/{ID_Student}";
+  rml:subjectMap [
+    rml:template "http://example.com/student/{ID_Student}";
   ];
 
-  rr:predicateObjectMap [
-    rr:predicate ex:plays;
-    rr:objectMap [
-      rr:template "http://example.com/sport/{ID_Sport}"
+  rml:predicateObjectMap [
+    rml:predicate ex:plays;
+    rml:objectMap [
+      rml:template "http://example.com/sport/{ID_Sport}"
     ]
   ].
 
-ql:Dictionary a rml:ReferenceFormulation;
+rml:Dictionary a rml:ReferenceFormulation;
 	kg4di:definedBy "Python".
```

### Comparing `morph_kgc-2.6.4/test/rml-in-memory/json_dictionary/RMLIMTC0011b/output.nq` & `morph_kgc-2.7.0/test/rml-in-memory/json_dictionary/RMLIMTC0011b/output.nq`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/rml-in-memory/json_dictionary/RMLIMTC0011b/test_RMLTC0011b_DICT.py` & `morph_kgc-2.7.0/test/rml-in-memory/json_dictionary/RMLIMTC0011b/test_RMLTC0011b_DICT.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/rml-in-memory/json_dictionary/RMLIMTC0012a/mapping.ttl` & `morph_kgc-2.7.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0015a/mapping.ttl`

 * *Files 21% similar despite different names*

```diff
@@ -1,46 +1,69 @@
-@prefix rr: <http://www.w3.org/ns/r2rml#> .
 @prefix foaf: <http://xmlns.com/foaf/0.1/> .
 @prefix ex: <http://example.com/> .
 @prefix xsd: <http://www.w3.org/2001/XMLSchema#> .
-@prefix rml: <http://semweb.mmlab.be/ns/rml#> .
-@prefix ql: <http://semweb.mmlab.be/ns/ql#> .
+@prefix rml: <http://w3id.org/rml/> .
+@prefix rdfs: <http://www.w3.org/2000/01/rdf-schema#> .
+@base <http://example.com/base/> .
 @prefix sd: <https://w3id.org/okn/o/sd#>.
 @prefix kg4di: <https://w3id.org/kg4di/definedBy>.
-@base <http://example.com/base/> .
 
 <TriplesMap1>
-  a rr:TriplesMap;
+  a rml:TriplesMap;
 
   rml:logicalSource [
     rml:source [
 			a sd:DatasetSpecification;
 			sd:name "variable1";
 			sd:hasDataTransformation [
+				sd:hasSoftwareRequirements "pandas>=1.1.0";
 				sd:hasSourceCode [
 					sd:programmingLanguage "Python3.9";
 				];
 			];
 		];
-		rml:referenceFormulation ql:Dictionary;
-    rml:iterator "$.persons[*]"
+    rml:referenceFormulation rml:DataFrame;
   ];
 
-  rr:subjectMap [ rr:template "{fname}{lname}{amount}"; rr:termType rr:BlankNode; ];
+  rml:subjectMap [
+    rml:template "http://example.com/{Code}"
+  ];
 
-  rr:predicateObjectMap [
-    rr:predicate foaf:name ;
-    rr:objectMap [
-      rr:template "{fname} {lname}";
-      rr:termType rr:Literal ;
+  rml:predicateObjectMap [
+    rml:predicate rdfs:label ;
+    rml:objectMap [
+      rml:reference "Name";
+      rml:language "en"
     ]
+  ].
+
+<TriplesMap2>
+  a rml:TriplesMap;
+
+  rml:logicalSource [
+    rml:source [
+			a sd:DatasetSpecification;
+			sd:name "variable2";
+			sd:hasDataTransformation [
+				sd:hasSoftwareRequirements "pandas>=1.1.0";
+				sd:hasSourceCode [
+					sd:programmingLanguage "Python3.9";
+				];
+			];
+		];
+    rml:referenceFormulation rml:DataFrame;
+  ];
+
+  rml:subjectMap [
+    rml:template "http://example.com/{Code}"
   ];
 
-  rr:predicateObjectMap [
-    rr:predicate ex:amount ;
-    rr:objectMap    [
-      rml:reference "amount";
+  rml:predicateObjectMap [
+    rml:predicate rdfs:label ;
+    rml:objectMap [
+      rml:reference "Name";
+      rml:language "es"
     ]
   ].
 
-ql:Dictionary a rml:ReferenceFormulation;
-	kg4di:definedBy "Python".
+rml:DataFrame a rml:ReferenceFormulation;
+	kg4di:definedBy "Pandas".
```

### Comparing `morph_kgc-2.6.4/test/rml-in-memory/json_dictionary/RMLIMTC0012a/test_RMLTC0012a_DICT.py` & `morph_kgc-2.7.0/test/rml-in-memory/json_dictionary/RMLIMTC0012a/test_RMLTC0012a_DICT.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/rml-in-memory/json_dictionary/RMLIMTC0012b/mapping.ttl` & `morph_kgc-2.7.0/test/rml-in-memory/json_dictionary/RMLIMTC0012b/mapping.ttl`

 * *Files 12% similar despite different names*

```diff
@@ -1,74 +1,72 @@
-@prefix rr: <http://www.w3.org/ns/r2rml#> .
 @prefix foaf: <http://xmlns.com/foaf/0.1/> .
 @prefix ex: <http://example.com/> .
 @prefix xsd: <http://www.w3.org/2001/XMLSchema#> .
-@prefix rml: <http://semweb.mmlab.be/ns/rml#> .
-@prefix ql: <http://semweb.mmlab.be/ns/ql#> .
+@prefix rml: <http://w3id.org/rml/> .
 @prefix sd: <https://w3id.org/okn/o/sd#>.
 @prefix kg4di: <https://w3id.org/kg4di/definedBy>.
 @base <http://example.com/base/> .
 
 <TriplesMap1>
-  a rr:TriplesMap;
+  a rml:TriplesMap;
 
   rml:logicalSource [
     rml:source [
 			a sd:DatasetSpecification;
 			sd:name "variable2";
 			sd:hasDataTransformation [
 				sd:hasSourceCode [
 					sd:programmingLanguage "Python3.9";
 				];
 			];
 		];
-		rml:referenceFormulation ql:Dictionary;
+		rml:referenceFormulation rml:Dictionary;
     rml:iterator "$.persons[*]"
   ];
 
-  rr:subjectMap [
-    rr:template "{fname}{lname}";
-    rr:termType rr:BlankNode ;
+  rml:subjectMap [
+    rml:template "{fname}{lname}";
+    rml:termType rml:BlankNode ;
   ];
 
-  rr:predicateObjectMap [
-    rr:predicate foaf:name ;
-    rr:objectMap [
-      rr:template "{fname} {lname}";
-      rr:termType rr:Literal ;
+  rml:predicateObjectMap [
+    rml:predicate foaf:name ;
+    rml:objectMap [
+      rml:template "{fname} {lname}";
+      rml:termType rml:Literal ;
     ]
   ];
   .
 
 <TriplesMap2>
-  a rr:TriplesMap;
+  a rml:TriplesMap;
 
   rml:logicalSource [
     rml:source [
 			a sd:DatasetSpecification;
 			sd:name "variable1";
 			sd:hasDataTransformation [
 				sd:hasSourceCode [
 					sd:programmingLanguage "Python3.9";
 				];
 			];
 		];
-		rml:referenceFormulation ql:Dictionary;
+		rml:referenceFormulation rml:Dictionary;
     rml:iterator "$.lives[*]"
 ];
 
-  rr:subjectMap [
-    rr:template "{fname}{lname}";
-    rr:termType rr:BlankNode;
+  rml:subjectMap [
+    rml:template "{fname}{lname}";
+    rml:termType rml:BlankNode;
   ];
 
-  rr:predicateObjectMap
+  rml:predicateObjectMap
   [
-    rr:predicate	ex:city ;
-    rr:objectMap    [
+    rml:predicate	ex:city ;
+    rml:objectMap    [
       rml:reference "city";
     ]
 ];
 .
 
-ql:Dictionary a rml:ReferenceFormulation;
+rml:Dictionary a rml:ReferenceFormulation;
 	kg4di:definedBy "Python".
```

### Comparing `morph_kgc-2.6.4/test/rml-in-memory/json_dictionary/RMLIMTC0012b/test_RMLTC0012b_DICT.py` & `morph_kgc-2.7.0/test/rml-in-memory/json_dictionary/RMLIMTC0012b/test_RMLTC0012b_DICT.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/rml-in-memory/json_dictionary/RMLIMTC0012c/mapping.ttl` & `morph_kgc-2.7.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0008c/mapping.ttl`

 * *Files 17% similar despite different names*

```diff
@@ -1,44 +1,36 @@
-@prefix rr: <http://www.w3.org/ns/r2rml#> .
 @prefix foaf: <http://xmlns.com/foaf/0.1/> .
 @prefix ex: <http://example.com/> .
 @prefix xsd: <http://www.w3.org/2001/XMLSchema#> .
-@prefix rml: <http://semweb.mmlab.be/ns/rml#> .
-@prefix ql: <http://semweb.mmlab.be/ns/ql#> .
+@prefix rml: <http://w3id.org/rml/> .
+@prefix activity: <http://example.com/activity/> .
+@base <http://example.com/base/> .
 @prefix sd: <https://w3id.org/okn/o/sd#>.
 @prefix kg4di: <https://w3id.org/kg4di/definedBy>.
-@base <http://example.com/base/> .
 
 <TriplesMap1>
-  a rr:TriplesMap;
+  a rml:TriplesMap;
 
   rml:logicalSource [
     rml:source [
 			a sd:DatasetSpecification;
 			sd:name "variable1";
 			sd:hasDataTransformation [
+				sd:hasSoftwareRequirements "pandas>=1.1.0";
 				sd:hasSourceCode [
 					sd:programmingLanguage "Python3.9";
 				];
 			];
 		];
-		rml:referenceFormulation ql:Dictionary;
-    rml:iterator "$.persons[*]"
+    rml:referenceFormulation rml:DataFrame;
   ];
 
-  rr:predicateObjectMap [
-    rr:predicate foaf:name ;
-    rr:objectMap [
-      rr:template "{fname} {lname}";
-      rr:termType rr:Literal ;
-    ]
-  ];
+  rml:subjectMap [ rml:template "http://example.com/Student/{ID}/{Name}" ];
 
-  rr:predicateObjectMap [
-    rr:predicate ex:amount ;
-    rr:objectMap    [
-      rml:reference "amount";
-    ]
-  ].
+  rml:predicateObjectMap [
+    rml:predicate foaf:name ;
+    rml:predicate ex:name ;
+    rml:objectMap [ rml:reference "Name" ]
+  ] .
 
-ql:Dictionary a rml:ReferenceFormulation;
-	kg4di:definedBy "Python".
+rml:DataFrame a rml:ReferenceFormulation;
+	kg4di:definedBy "Pandas".
```

### Comparing `morph_kgc-2.6.4/test/rml-in-memory/json_dictionary/RMLIMTC0012c/test_RMLTC0012c_DICT.py` & `morph_kgc-2.7.0/test/rml-in-memory/json_dictionary/RMLIMTC0012c/test_RMLTC0012c_DICT.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/rml-in-memory/json_dictionary/RMLIMTC0012d/test_RMLTC0012d_DICT.py` & `morph_kgc-2.7.0/test/rml-in-memory/json_dictionary/RMLIMTC0012d/test_RMLTC0012d_DICT.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/rml-in-memory/json_dictionary/RMLIMTC0013a/mapping.ttl` & `morph_kgc-2.7.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0005a/mapping.ttl`

 * *Files 18% similar despite different names*

```diff
@@ -1,37 +1,36 @@
-@prefix rr: <http://www.w3.org/ns/r2rml#> .
 @prefix foaf: <http://xmlns.com/foaf/0.1/> .
 @prefix ex: <http://example.com/> .
 @prefix xsd: <http://www.w3.org/2001/XMLSchema#> .
-@prefix rml: <http://semweb.mmlab.be/ns/rml#> .
-@prefix ql: <http://semweb.mmlab.be/ns/ql#> .
+@prefix rml: <http://w3id.org/rml/> .
+@base <http://example.com/base/> .
 @prefix sd: <https://w3id.org/okn/o/sd#>.
 @prefix kg4di: <https://w3id.org/kg4di/definedBy>.
-@base <http://example.com/base/> .
 
-<TriplesMap1>
-  a rr:TriplesMap;
+<TriplesMap1> a rml:TriplesMap;
 
   rml:logicalSource [
     rml:source [
 			a sd:DatasetSpecification;
 			sd:name "variable1";
 			sd:hasDataTransformation [
+				sd:hasSoftwareRequirements "pandas>=1.1.0";
 				sd:hasSourceCode [
 					sd:programmingLanguage "Python3.9";
 				];
 			];
 		];
-		rml:referenceFormulation ql:Dictionary;
-    rml:iterator "$.persons[*]"
+    rml:referenceFormulation rml:CSV
   ];
 
-  rr:subjectMap [ rr:template "http://example.com/Person/{ID}/{Name}/{DateOfBirth}"];
+  rml:subjectMap [
+    rml:template "http://example.com/{fname};{lname}";
+    rml:class foaf:Person;
+  ];
 
-  rr:predicateObjectMap
-    [
-      rr:predicate		ex:BirthDay ;
-      rr:objectMap		[ rml:reference "DateOfBirth" ]
-    ].
+  rml:predicateObjectMap [
+    rml:predicate ex:owes;
+    rml:objectMap [ rml:reference "amount"; ]
+  ].
 
-ql:Dictionary a rml:ReferenceFormulation;
-	kg4di:definedBy "Python".
+rml:DataFrame a rml:ReferenceFormulation;
+	kg4di:definedBy "Pandas".
```

### Comparing `morph_kgc-2.6.4/test/rml-in-memory/json_dictionary/RMLIMTC0013a/test_RMLTC0013a_DICT.py` & `morph_kgc-2.7.0/test/rml-in-memory/json_dictionary/RMLIMTC0013a/test_RMLTC0013a_DICT.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/rml-in-memory/json_dictionary/RMLIMTC0015a/mapping.ttl` & `morph_kgc-2.7.0/test/rml-in-memory/json_dictionary/RMLIMTC0015a/mapping.ttl`

 * *Files 12% similar despite different names*

```diff
@@ -1,71 +1,69 @@
-@prefix rr: <http://www.w3.org/ns/r2rml#> .
 @prefix foaf: <http://xmlns.com/foaf/0.1/> .
 @prefix ex: <http://example.com/> .
 @prefix xsd: <http://www.w3.org/2001/XMLSchema#> .
-@prefix rml: <http://semweb.mmlab.be/ns/rml#> .
-@prefix ql: <http://semweb.mmlab.be/ns/ql#> .
+@prefix rml: <http://w3id.org/rml/> .
 @prefix rdfs: <http://www.w3.org/2000/01/rdf-schema#> .
 @base <http://example.com/base/> .
 @prefix sd: <https://w3id.org/okn/o/sd#>.
 @prefix kg4di: <https://w3id.org/kg4di/definedBy>.
 
 <TriplesMap1>
-  a rr:TriplesMap;
+  a rml:TriplesMap;
 
   rml:logicalSource [
     rml:source [
 			a sd:DatasetSpecification;
 			sd:name "variable1";
 			sd:hasDataTransformation [
 				sd:hasSourceCode [
 					sd:programmingLanguage "Python3.9";
 				];
 			];
 		];
-		rml:referenceFormulation ql:Dictionary;
+		rml:referenceFormulation rml:Dictionary;
     rml:iterator "$.countries[*]"
   ];
 
-  rr:subjectMap [
-    rr:template "http://example.com/{Code}"
+  rml:subjectMap [
+    rml:template "http://example.com/{Code}"
   ];
 
-  rr:predicateObjectMap [
-    rr:predicate rdfs:label ;
-    rr:objectMap [
+  rml:predicateObjectMap [
+    rml:predicate rdfs:label ;
+    rml:objectMap [
       rml:reference "Name";
-      rr:language "en"
+      rml:language "en"
     ]
   ].
 
 <TriplesMap2>
-  a rr:TriplesMap;
+  a rml:TriplesMap;
 
   rml:logicalSource [
     rml:source [
 			a sd:DatasetSpecification;
 			sd:name "variable2";
 			sd:hasDataTransformation [
 				sd:hasSourceCode [
 					sd:programmingLanguage "Python3.9";
 				];
 			];
 		];
-		rml:referenceFormulation ql:Dictionary;
+		rml:referenceFormulation rml:Dictionary;
     rml:iterator "$.countries[*]"
   ];
 
-  rr:subjectMap [
-    rr:template "http://example.com/{Code}"
+  rml:subjectMap [
+    rml:template "http://example.com/{Code}"
   ];
 
-  rr:predicateObjectMap [
-    rr:predicate rdfs:label ;
-    rr:objectMap [
+  rml:predicateObjectMap [
+    rml:predicate rdfs:label ;
+    rml:objectMap [
       rml:reference "Name";
-      rr:language "es"
+      rml:language "es"
     ]
   ].
 
-ql:Dictionary a rml:ReferenceFormulation;
+rml:Dictionary a rml:ReferenceFormulation;
 	kg4di:definedBy "Python".
```

### Comparing `morph_kgc-2.6.4/test/rml-in-memory/json_dictionary/RMLIMTC0015a/test_RMLTC0015a_DICT.py` & `morph_kgc-2.7.0/test/rml-in-memory/json_dictionary/RMLIMTC0015a/test_RMLTC0015a_DICT.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/rml-in-memory/json_dictionary/RMLIMTC0015b/mapping.ttl` & `morph_kgc-2.7.0/test/rml-in-memory/pandas_dataframe/triples_map_without_pom/mapping.ttl`

 * *Files 16% similar despite different names*

```diff
@@ -1,67 +1,62 @@
-@prefix rr: <http://www.w3.org/ns/r2rml#> .
 @prefix foaf: <http://xmlns.com/foaf/0.1/> .
-@prefix rdfs: <http://www.w3.org/2000/01/rdf-schema#> .
 @prefix ex: <http://example.com/> .
 @prefix xsd: <http://www.w3.org/2001/XMLSchema#> .
-@prefix rml: <http://semweb.mmlab.be/ns/rml#> .
-@prefix ql: <http://semweb.mmlab.be/ns/ql#> .
+@prefix rml: <http://w3id.org/rml/> .
+@prefix activity: <http://example.com/activity/> .
+@prefix rdfs: <http://www.w3.org/2000/01/rdf-schema#> .
+@base <http://example.com/base/> .
 @prefix sd: <https://w3id.org/okn/o/sd#>.
 @prefix kg4di: <https://w3id.org/kg4di/definedBy>.
-@base <http://example.com/base/> .
 
 <TriplesMap1>
-  a rr:TriplesMap;
+  a rml:TriplesMap;
 
   rml:logicalSource [
     rml:source [
 			a sd:DatasetSpecification;
 			sd:name "variable1";
 			sd:hasDataTransformation [
+				sd:hasSoftwareRequirements "pandas>=1.1.0";
 				sd:hasSourceCode [
 					sd:programmingLanguage "Python3.9";
 				];
 			];
 		];
-		rml:referenceFormulation ql:Dictionary;
-    rml:iterator "$.countries[*]"
+		rml:referenceFormulation rml:DataFrame;
   ];
 
-  rr:subjectMap [ rr:template "http://example.com/{Code}" ];
+  rml:subjectMap [ rml:template "http://example.com/resource/student_{ID}" ];
 
-  rr:predicateObjectMap [
-    rr:predicate rdfs:label;
-    rr:objectMap [
-      rml:reference "Name";
-      rr:language "english"
+  rml:predicateObjectMap [
+    rml:predicate <http://example.com/ontology/practises> ;
+    rml:objectMap [
+      a rml:RefObjectMap ;
+      rml:parentTriplesMap <TriplesMap2>;
+      rml:joinCondition [
+        rml:child "Sport" ;
+        rml:parent "ID" ;
+      ]
     ]
   ] .
 
 <TriplesMap2>
-  a rr:TriplesMap;
+  a rml:TriplesMap;
 
   rml:logicalSource [
     rml:source [
 			a sd:DatasetSpecification;
 			sd:name "variable2";
 			sd:hasDataTransformation [
+				sd:hasSoftwareRequirements "pandas>=1.1.0";
 				sd:hasSourceCode [
 					sd:programmingLanguage "Python3.9";
 				];
 			];
 		];
-		rml:referenceFormulation ql:Dictionary;
-    rml:iterator "$.countries[*]"
+		rml:referenceFormulation rml:DataFrame;
   ];
 
-  rr:subjectMap [ rr:template "http://example.com/{Code}" ];
-
-  rr:predicateObjectMap [
-    rr:predicate rdfs:label;
-    rr:objectMap [
-      rml:reference "Name";
-      rr:language "spanish"
-    ]
-  ].
+  rml:subjectMap [ rml:template "http://example.com/resource/sport_{ID}" ].
 
-ql:Dictionary a rml:ReferenceFormulation;
-	kg4di:definedBy "Python".
+rml:DataFrame a rml:ReferenceFormulation;
+	kg4di:definedBy "Pandas".
```

### Comparing `morph_kgc-2.6.4/test/rml-in-memory/json_dictionary/RMLIMTC0015b/test_RMLTC0015b_DICT.py` & `morph_kgc-2.7.0/test/rml-in-memory/json_dictionary/RMLIMTC0015b/test_RMLTC0015b_DICT.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/rml-in-memory/pandas_dataframe/RMLIMTC0000/mapping.ttl` & `morph_kgc-2.7.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0016a/mapping.ttl`

 * *Files 14% similar despite different names*

```diff
@@ -1,41 +1,37 @@
-@prefix rr: <http://www.w3.org/ns/r2rml#> .
 @prefix foaf: <http://xmlns.com/foaf/0.1/> .
+@prefix rdfs: <http://www.w3.org/2000/01/rdf-schema#> .
 @prefix ex: <http://example.com/> .
 @prefix xsd: <http://www.w3.org/2001/XMLSchema#> .
-@prefix rml: <http://semweb.mmlab.be/ns/rml#> .
-@prefix ql: <http://semweb.mmlab.be/ns/ql#> .
+@prefix rml: <http://w3id.org/rml/> .
 @prefix sd: <https://w3id.org/okn/o/sd#>.
 @prefix kg4di: <https://w3id.org/kg4di/definedBy>.
-
 @base <http://example.com/base/> .
 
 <TriplesMap1>
-  a rr:TriplesMap;
+  a rml:TriplesMap;
 
   rml:logicalSource [
     rml:source [
 			a sd:DatasetSpecification;
 			sd:name "variable1";
 			sd:hasDataTransformation [
 				sd:hasSoftwareRequirements "pandas>=1.1.0";
 				sd:hasSourceCode [
 					sd:programmingLanguage "Python3.9";
 				];
 			];
 		];
-		rml:referenceFormulation ql:DataFrame;
-  ] ;
-
-  rr:subjectMap [
-    rr:template "http://example.com/{Name}"
+    rml:referenceFormulation rml:DataFrame;
   ];
 
-  rr:predicateObjectMap [
-    rr:predicate foaf:name ;
-    rr:objectMap [
-      rml:reference "Name"
+  rml:subjectMap [ rml:template "http://example.com/{c1}" ];
+
+  rml:predicateObjectMap [
+    rml:predicate rdfs:label;
+    rml:objectMap [
+      rml:reference "c2"
     ]
-  ].
+  ] .
 
-ql:DataFrame a rml:ReferenceFormulation;
+rml:DataFrame a rml:ReferenceFormulation;
 	kg4di:definedBy "Pandas".
```

### Comparing `morph_kgc-2.6.4/test/rml-in-memory/pandas_dataframe/RMLIMTC0000/test_RMLIMTC0000_DF.py` & `morph_kgc-2.7.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0000/test_RMLIMTC0000_DF.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/rml-in-memory/pandas_dataframe/RMLIMTC0001a/mapping.ttl` & `morph_kgc-2.7.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0007g/mapping.ttl`

 * *Files 14% similar despite different names*

```diff
@@ -1,41 +1,38 @@
-@prefix rr: <http://www.w3.org/ns/r2rml#> .
 @prefix foaf: <http://xmlns.com/foaf/0.1/> .
 @prefix ex: <http://example.com/> .
 @prefix xsd: <http://www.w3.org/2001/XMLSchema#> .
-@prefix rml: <http://semweb.mmlab.be/ns/rml#> .
-@prefix ql: <http://semweb.mmlab.be/ns/ql#> .
+@prefix rml: <http://w3id.org/rml/> .
+@base <http://example.com/base/> .
 @prefix sd: <https://w3id.org/okn/o/sd#>.
 @prefix kg4di: <https://w3id.org/kg4di/definedBy>.
 
-@base <http://example.com/base/> .
-
-<TriplesMap1>
-  a rr:TriplesMap;
+<TriplesMap1> a rml:TriplesMap;
 
   rml:logicalSource [
     rml:source [
 			a sd:DatasetSpecification;
 			sd:name "variable1";
 			sd:hasDataTransformation [
 				sd:hasSoftwareRequirements "pandas>=1.1.0";
 				sd:hasSourceCode [
 					sd:programmingLanguage "Python3.9";
 				];
 			];
 		];
-    rml:referenceFormulation ql:DataFrame
+    rml:referenceFormulation rml:DataFrame;
   ];
 
-  rr:subjectMap [
-    rr:template "http://example.com/{Name}"
+  rml:subjectMap [
+    rml:template "http://example.com/Student/{ID}/{FirstName}";
+    rml:graph rml:defaultGraph
   ];
 
-  rr:predicateObjectMap [
-    rr:predicate foaf:name;
-    rr:objectMap [
-      rml:reference "Name"
+  rml:predicateObjectMap [
+    rml:predicate foaf:name;
+    rml:objectMap [
+      rml:reference "FirstName"
     ]
   ].
 
-ql:DataFrame a rml:ReferenceFormulation;
+rml:DataFrame a rml:ReferenceFormulation;
 	kg4di:definedBy "Pandas".
```

### Comparing `morph_kgc-2.6.4/test/rml-in-memory/pandas_dataframe/RMLIMTC0001a/test_RMLTC0001a_DF.py` & `morph_kgc-2.7.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0001a/test_RMLTC0001a_DF.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/rml-in-memory/pandas_dataframe/RMLIMTC0001b/test_RMLIMTC0001b_DF.py` & `morph_kgc-2.7.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0001b/test_RMLIMTC0001b_DF.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/rml-in-memory/pandas_dataframe/RMLIMTC0002a/mapping.ttl` & `morph_kgc-2.7.0/test/rml-in-memory/json_dictionary/RMLIMTC0008a/mapping.ttl`

 * *Files 27% similar despite different names*

```diff
@@ -1,43 +1,53 @@
-@prefix rr: <http://www.w3.org/ns/r2rml#> .
 @prefix foaf: <http://xmlns.com/foaf/0.1/> .
 @prefix ex: <http://example.com/> .
 @prefix xsd: <http://www.w3.org/2001/XMLSchema#> .
-@prefix rml: <http://semweb.mmlab.be/ns/rml#> .
-@prefix ql: <http://semweb.mmlab.be/ns/ql#> .
+@prefix rml: <http://w3id.org/rml/> .
+@prefix rdf: <http://www.w3.org/1999/02/22-rdf-syntax-ns#> .
 @base <http://example.com/base/> .
 @prefix sd: <https://w3id.org/okn/o/sd#>.
 @prefix kg4di: <https://w3id.org/kg4di/definedBy>.
 
-<TriplesMap1> a rr:TriplesMap;
+<TriplesMap1>
+  a rml:TriplesMap;
 
   rml:logicalSource [
     rml:source [
 			a sd:DatasetSpecification;
 			sd:name "variable1";
 			sd:hasDataTransformation [
-				sd:hasSoftwareRequirements "pandas>=1.1.0";
 				sd:hasSourceCode [
 					sd:programmingLanguage "Python3.9";
 				];
 			];
 		];
-    rml:referenceFormulation ql:DataFrame;
+		rml:referenceFormulation rml:Dictionary;
+    rml:iterator "$.students[*]"
   ];
 
-  rr:subjectMap [
-    rr:template "http://example.com/{ID}/{Name}";
-    rr:class foaf:Person
+  rml:subjectMap [
+    rml:template "http://example.com/Student/{ID}/{Name}";
+    rml:graphMap [ rml:template "http://example.com/graph/Student/{ID}/{Name}" ]
   ];
 
-  rr:predicateObjectMap [
-    rr:predicate ex:id ;
-    rr:objectMap [ rml:reference "ID" ]
+  rml:predicateObjectMap [
+    rml:predicate rdf:type ;
+    rml:object foaf:Person;
   ];
 
-  rr:predicateObjectMap [
-    rr:predicate foaf:name ;
-    rr:objectMap [ rml:reference "Name" ]
-  ].
+  rml:predicateObjectMap [
+    rml:predicate ex:id ;
+    rml:objectMap [ rml:reference "ID" ]
+  ];
+
+  rml:predicateObjectMap [
+    rml:predicate foaf:name ;
+    rml:objectMap [ rml:reference "Name" ]
+  ];
+
+  rml:predicateObjectMap [
+    rml:predicate ex:Sport ;
+    rml:objectMap [ rml:reference "Sport" ]
+  ] .
 
-ql:DataFrame a rml:ReferenceFormulation;
-	kg4di:definedBy "Pandas".
+rml:Dictionary a rml:ReferenceFormulation;
+	kg4di:definedBy "Python".
```

### Comparing `morph_kgc-2.6.4/test/rml-in-memory/pandas_dataframe/RMLIMTC0002a/test_RMLIMTC0002a_DF.py` & `morph_kgc-2.7.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0002a/test_RMLIMTC0002a_DF.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/rml-in-memory/pandas_dataframe/RMLIMTC0002b/mapping.ttl` & `morph_kgc-2.7.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0002c/mapping.ttl`

 * *Files 14% similar despite different names*

```diff
@@ -1,38 +1,35 @@
-@prefix rr: <http://www.w3.org/ns/r2rml#> .
 @prefix foaf: <http://xmlns.com/foaf/0.1/> .
 @prefix ex: <http://example.com/> .
 @prefix xsd: <http://www.w3.org/2001/XMLSchema#> .
-@prefix rml: <http://semweb.mmlab.be/ns/rml#> .
-@prefix ql: <http://semweb.mmlab.be/ns/ql#> .
+@prefix rml: <http://w3id.org/rml/> .
 @base <http://example.com/base/> .
 @prefix sd: <https://w3id.org/okn/o/sd#>.
 @prefix kg4di: <https://w3id.org/kg4di/definedBy>.
 
-<TriplesMap1> a rr:TriplesMap;
+<TriplesMap1> a rml:TriplesMap;
 
   rml:logicalSource [
     rml:source [
 			a sd:DatasetSpecification;
 			sd:name "variable1";
 			sd:hasDataTransformation [
 				sd:hasSoftwareRequirements "pandas>=1.1.0";
 				sd:hasSourceCode [
 					sd:programmingLanguage "Python3.9";
 				];
 			];
 		];
-    rml:referenceFormulation ql:DataFrame;
+    rml:referenceFormulation rml:DataFrame;
   ];
 
-  rr:subjectMap [
-    rr:template "students{ID}";
-    rr:termType rr:BlankNode
+  rml:subjectMap [
+    rml:template "http://example.com/{ID}/{Name}";
   ];
 
-  rr:predicateObjectMap [
-    rr:predicate foaf:name;
-    rr:objectMap [ rml:reference "Name" ]
+  rml:predicateObjectMap [
+    rml:predicate ex:id ;
+    rml:objectMap [ rml:reference "IDs" ]
   ].
 
-ql:DataFrame a rml:ReferenceFormulation;
+rml:DataFrame a rml:ReferenceFormulation;
 	kg4di:definedBy "Pandas".
```

### Comparing `morph_kgc-2.6.4/test/rml-in-memory/pandas_dataframe/RMLIMTC0002b/test_RMLIMTC0002b_DF.py` & `morph_kgc-2.7.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0002b/test_RMLIMTC0002b_DF.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/rml-in-memory/pandas_dataframe/RMLIMTC0002c/mapping.ttl` & `morph_kgc-2.7.0/test/rml-in-memory/json_dictionary/RMLIMTC0003c/mapping.ttl`

 * *Files 26% similar despite different names*

```diff
@@ -1,37 +1,38 @@
-@prefix rr: <http://www.w3.org/ns/r2rml#> .
 @prefix foaf: <http://xmlns.com/foaf/0.1/> .
 @prefix ex: <http://example.com/> .
 @prefix xsd: <http://www.w3.org/2001/XMLSchema#> .
-@prefix rml: <http://semweb.mmlab.be/ns/rml#> .
-@prefix ql: <http://semweb.mmlab.be/ns/ql#> .
-@base <http://example.com/base/> .
+@prefix rml: <http://w3id.org/rml/> .
 @prefix sd: <https://w3id.org/okn/o/sd#>.
 @prefix kg4di: <https://w3id.org/kg4di/definedBy>.
+@base <http://example.com/base/> .
 
-<TriplesMap1> a rr:TriplesMap;
+<TriplesMap1> a rml:TriplesMap;
 
   rml:logicalSource [
     rml:source [
 			a sd:DatasetSpecification;
 			sd:name "variable1";
 			sd:hasDataTransformation [
-				sd:hasSoftwareRequirements "pandas>=1.1.0";
 				sd:hasSourceCode [
 					sd:programmingLanguage "Python3.9";
 				];
 			];
 		];
-    rml:referenceFormulation ql:DataFrame;
+    rml:referenceFormulation rml:Dictionary;
+    rml:iterator "$.students[*]"
   ];
 
-  rr:subjectMap [
-    rr:template "http://example.com/{ID}/{Name}";
+  rml:subjectMap [
+    rml:template "http://example.com/Student{ID}";
   ];
 
-  rr:predicateObjectMap [
-    rr:predicate ex:id ;
-    rr:objectMap [ rml:reference "IDs" ]
+  rml:predicateObjectMap [
+    rml:predicate foaf:name ;
+    rml:objectMap [
+      rml:template "{FirstName} {LastName}";
+      rml:termType rml:Literal;
+    ]
   ].
 
-ql:DataFrame a rml:ReferenceFormulation;
-	kg4di:definedBy "Pandas".
+rml:Dictionary a rml:ReferenceFormulation;
+	kg4di:definedBy "Python".
```

### Comparing `morph_kgc-2.6.4/test/rml-in-memory/pandas_dataframe/RMLIMTC0002c/test_RMLIMTC0002c_DF.py` & `morph_kgc-2.7.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0002c/test_RMLIMTC0002c_DF.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/rml-in-memory/pandas_dataframe/RMLIMTC0002e/test_RMLIMTC0002e_DF.py` & `morph_kgc-2.7.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0002e/test_RMLIMTC0002e_DF.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/rml-in-memory/pandas_dataframe/RMLIMTC0003c/test_RMLIMTC0003c_DF.py` & `morph_kgc-2.7.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0003c/test_RMLIMTC0003c_DF.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/rml-in-memory/pandas_dataframe/RMLIMTC0004a/mapping.ttl` & `morph_kgc-2.7.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0004a/mapping.ttl`

 * *Files 16% similar despite different names*

```diff
@@ -1,68 +1,66 @@
-@prefix rr: <http://www.w3.org/ns/r2rml#> .
 @prefix foaf: <http://xmlns.com/foaf/0.1/> .
 @prefix ex: <http://example.com/> .
 @prefix xsd: <http://www.w3.org/2001/XMLSchema#> .
-@prefix rml: <http://semweb.mmlab.be/ns/rml#> .
-@prefix ql: <http://semweb.mmlab.be/ns/ql#> .
+@prefix rml: <http://w3id.org/rml/> .
 @base <http://example.com/base/> .
 @prefix sd: <https://w3id.org/okn/o/sd#>.
 @prefix kg4di: <https://w3id.org/kg4di/definedBy>.
 
-<TriplesMap1> a rr:TriplesMap;
+<TriplesMap1> a rml:TriplesMap;
 
   rml:logicalSource [
     rml:source [
 			a sd:DatasetSpecification;
 			sd:name "variable1";
 			sd:hasDataTransformation [
 				sd:hasSoftwareRequirements "pandas>=1.1.0";
 				sd:hasSourceCode [
 					sd:programmingLanguage "Python3.9";
 				];
 			];
 		];
-    rml:referenceFormulation ql:DataFrame
+    rml:referenceFormulation rml:DataFrame
   ];
 
-  rr:subjectMap [
-    rr:template "http://example.com/{Student}";
-    rr:class ex:Student
+  rml:subjectMap [
+    rml:template "http://example.com/{Student}";
+    rml:class ex:Student
   ];
 
-  rr:predicateObjectMap [
-    rr:predicate foaf:name ;
-    rr:objectMap [
+  rml:predicateObjectMap [
+    rml:predicate foaf:name ;
+    rml:objectMap [
       rml:reference "Student"
     ]
   ].
 
-<TriplesMap2> a rr:TriplesMap;
+<TriplesMap2> a rml:TriplesMap;
 
   rml:logicalSource [
     rml:source [
 			a sd:DatasetSpecification;
 			sd:name "variable1";
 			sd:hasDataTransformation [
 				sd:hasSoftwareRequirements "pandas>=1.1.0";
 				sd:hasSourceCode [
 					sd:programmingLanguage "Python3.9";
 				];
 			];
 		];
-    rml:referenceFormulation ql:DataFrame;
+    rml:referenceFormulation rml:DataFrame;
   ];
 
-  rr:subjectMap [
-    rr:template "http://example.com/{Sport}";
-    rr:class ex:Sport
+  rml:subjectMap [
+    rml:template "http://example.com/{Sport}";
+    rml:class ex:Sport
   ];
 
-  rr:predicateObjectMap [
-    rr:predicate foaf:name ;
-    rr:objectMap [
+  rml:predicateObjectMap [
+    rml:predicate foaf:name ;
+    rml:objectMap [
       rml:reference "Sport"
     ]
   ].
 
-ql:DataFrame a rml:ReferenceFormulation;
+rml:DataFrame a rml:ReferenceFormulation;
 	kg4di:definedBy "Pandas".
```

### Comparing `morph_kgc-2.6.4/test/rml-in-memory/pandas_dataframe/RMLIMTC0004a/test_RMLIMTC0004a_DF.py` & `morph_kgc-2.7.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0004a/test_RMLIMTC0004a_DF.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/rml-in-memory/pandas_dataframe/RMLIMTC0004b/mapping.ttl` & `morph_kgc-2.7.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0007b/mapping.ttl`

 * *Files 16% similar despite different names*

```diff
@@ -1,42 +1,42 @@
-@prefix rr: <http://www.w3.org/ns/r2rml#> .
 @prefix foaf: <http://xmlns.com/foaf/0.1/> .
 @prefix ex: <http://example.com/> .
 @prefix xsd: <http://www.w3.org/2001/XMLSchema#> .
-@prefix rml: <http://semweb.mmlab.be/ns/rml#> .
-@prefix ql: <http://semweb.mmlab.be/ns/ql#> .
+@prefix rml: <http://w3id.org/rml/> .
+@prefix rdf: <http://www.w3.org/1999/02/22-rdf-syntax-ns#> .
+@base <http://example.com/base/> .
 @prefix sd: <https://w3id.org/okn/o/sd#>.
 @prefix kg4di: <https://w3id.org/kg4di/definedBy>.
 
-@base <http://example.com/base/> .
-
-<TriplesMap1>
-  a rr:TriplesMap;
+<TriplesMap1> a rml:TriplesMap;
 
   rml:logicalSource [
     rml:source [
 			a sd:DatasetSpecification;
 			sd:name "variable1";
 			sd:hasDataTransformation [
 				sd:hasSoftwareRequirements "pandas>=1.1.0";
 				sd:hasSourceCode [
 					sd:programmingLanguage "Python3.9";
 				];
 			];
 		];
-    rml:referenceFormulation ql:CSV
+    rml:referenceFormulation rml:CSV
+  ];
+
+  rml:subjectMap [
+    rml:template "http://example.com/Student/{ID}/{FirstName}";
+    rml:graph ex:PersonGraph
   ];
 
-  rr:subjectMap [
-    rr:template "http://example.com/{Name}";
-    rr:termType rr:Literal
+  rml:predicateObjectMap [
+    rml:predicate rdf:type;
+    rml:object foaf:Person;
   ];
 
-  rr:predicateObjectMap [
-    rr:predicate foaf:name;
-    rr:objectMap [
-      rml:reference "Name"
-    ]
+  rml:predicateObjectMap [
+    rml:predicate foaf:name;
+    rml:objectMap [ rml:reference "FirstName" ]
   ].
 
-ql:DataFrame a rml:ReferenceFormulation;
+rml:DataFrame a rml:ReferenceFormulation;
 	kg4di:definedBy "Pandas".
```

### Comparing `morph_kgc-2.6.4/test/rml-in-memory/pandas_dataframe/RMLIMTC0004b/test_RMLIMTC0004b_DF.py` & `morph_kgc-2.7.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0004b/test_RMLIMTC0004b_DF.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/rml-in-memory/pandas_dataframe/RMLIMTC0005a/test_RMLIMTC0005a_DF.py` & `morph_kgc-2.7.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0005a/test_RMLIMTC0005a_DF.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/rml-in-memory/pandas_dataframe/RMLIMTC0006a/mapping.ttl` & `morph_kgc-2.7.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0006a/mapping.ttl`

 * *Files 22% similar despite different names*

```diff
@@ -1,38 +1,36 @@
-@prefix rr: <http://www.w3.org/ns/r2rml#> .
 @prefix foaf: <http://xmlns.com/foaf/0.1/> .
 @prefix ex: <http://example.com/> .
 @prefix xsd: <http://www.w3.org/2001/XMLSchema#> .
-@prefix rml: <http://semweb.mmlab.be/ns/rml#> .
-@prefix ql: <http://semweb.mmlab.be/ns/ql#> .
+@prefix rml: <http://w3id.org/rml/> .
 @base <http://example.com/base/> .
 @prefix sd: <https://w3id.org/okn/o/sd#>.
 @prefix kg4di: <https://w3id.org/kg4di/definedBy>.
 
-<TriplesMap1> a rr:TriplesMap;
+<TriplesMap1> a rml:TriplesMap;
 
   rml:logicalSource [
     rml:source [
 			a sd:DatasetSpecification;
 			sd:name "variable1";
 			sd:hasDataTransformation [
 				sd:hasSoftwareRequirements "pandas>=1.1.0";
 				sd:hasSourceCode [
 					sd:programmingLanguage "Python3.9";
 				];
 			];
 		];
-    rml:referenceFormulation ql:DataFrame;
+    rml:referenceFormulation rml:DataFrame;
   ];
 
-  rr:subjectMap [
-    rr:constant ex:BadStudent;
-    rr:graphMap [ rr:constant <http://example.com/graph/student> ];
+  rml:subjectMap [
+    rml:constant ex:BadStudent;
+    rml:graphMap [ rml:constant <http://example.com/graph/student> ];
   ];
 
-  rr:predicateObjectMap [
-    rr:predicateMap [ rr:constant ex:description ];
-    rr:objectMap [ rr:constant "Bad Student"; ]
+  rml:predicateObjectMap [
+    rml:predicateMap [ rml:constant ex:description ];
+    rml:objectMap [ rml:constant "Bad Student"; ]
   ].
 
-ql:DataFrame a rml:ReferenceFormulation;
+rml:DataFrame a rml:ReferenceFormulation;
 	kg4di:definedBy "Pandas".
```

### Comparing `morph_kgc-2.6.4/test/rml-in-memory/pandas_dataframe/RMLIMTC0006a/test_RMLIMTC0006a_DF.py` & `morph_kgc-2.7.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0006a/test_RMLIMTC0006a_DF.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/rml-in-memory/pandas_dataframe/RMLIMTC0007a/mapping.ttl` & `morph_kgc-2.7.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0008a/mapping.ttl`

 * *Files 22% similar despite different names*

```diff
@@ -1,38 +1,53 @@
-@prefix rr: <http://www.w3.org/ns/r2rml#> .
 @prefix foaf: <http://xmlns.com/foaf/0.1/> .
 @prefix ex: <http://example.com/> .
 @prefix xsd: <http://www.w3.org/2001/XMLSchema#> .
-@prefix rml: <http://semweb.mmlab.be/ns/rml#> .
-@prefix ql: <http://semweb.mmlab.be/ns/ql#> .
+@prefix rml: <http://w3id.org/rml/> .
 @prefix rdf: <http://www.w3.org/1999/02/22-rdf-syntax-ns#> .
 @base <http://example.com/base/> .
 @prefix sd: <https://w3id.org/okn/o/sd#>.
 @prefix kg4di: <https://w3id.org/kg4di/definedBy>.
 
-<TriplesMap1> a rr:TriplesMap;
+<TriplesMap1>
+  a rml:TriplesMap;
 
   rml:logicalSource [
     rml:source [
 			a sd:DatasetSpecification;
 			sd:name "variable1";
 			sd:hasDataTransformation [
 				sd:hasSoftwareRequirements "pandas>=1.1.0";
 				sd:hasSourceCode [
 					sd:programmingLanguage "Python3.9";
 				];
 			];
 		];
-    rml:referenceFormulation ql:DataFrame;
+    rml:referenceFormulation rml:DataFrame;
   ];
 
-  rr:subjectMap [
-    rr:template "http://example.com/Student/{ID}/{FirstName}"
+  rml:subjectMap [
+    rml:template "http://example.com/Student/{ID}/{Name}";
+    rml:graphMap [ rml:template "http://example.com/graph/Student/{ID}/{Name}" ]
   ];
 
-  rr:predicateObjectMap [
-    rr:predicate rdf:type;
-    rr:object foaf:Person;
-  ].
+  rml:predicateObjectMap [
+    rml:predicate rdf:type ;
+    rml:object foaf:Person;
+  ];
+
+  rml:predicateObjectMap [
+    rml:predicate ex:id ;
+    rml:objectMap [ rml:reference "ID" ]
+  ];
+
+  rml:predicateObjectMap [
+    rml:predicate foaf:name ;
+    rml:objectMap [ rml:reference "Name" ]
+  ];
+
+  rml:predicateObjectMap [
+    rml:predicate ex:Sport ;
+    rml:objectMap [ rml:reference "Sport" ]
+  ] .
 
-ql:DataFrame a rml:ReferenceFormulation;
+rml:DataFrame a rml:ReferenceFormulation;
 	kg4di:definedBy "Pandas".
```

### Comparing `morph_kgc-2.6.4/test/rml-in-memory/pandas_dataframe/RMLIMTC0007a/test_RMLIMTC0007a_DF.py` & `morph_kgc-2.7.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0007a/test_RMLIMTC0007a_DF.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/rml-in-memory/pandas_dataframe/RMLIMTC0007b/mapping.ttl` & `morph_kgc-2.7.0/test/rml-in-memory/json_dictionary/RMLIMTC0007b/mapping.ttl`

 * *Files 15% similar despite different names*

```diff
@@ -1,44 +1,42 @@
-@prefix rr: <http://www.w3.org/ns/r2rml#> .
 @prefix foaf: <http://xmlns.com/foaf/0.1/> .
 @prefix ex: <http://example.com/> .
 @prefix xsd: <http://www.w3.org/2001/XMLSchema#> .
-@prefix rml: <http://semweb.mmlab.be/ns/rml#> .
-@prefix ql: <http://semweb.mmlab.be/ns/ql#> .
+@prefix rml: <http://w3id.org/rml/> .
 @prefix rdf: <http://www.w3.org/1999/02/22-rdf-syntax-ns#> .
 @base <http://example.com/base/> .
 @prefix sd: <https://w3id.org/okn/o/sd#>.
 @prefix kg4di: <https://w3id.org/kg4di/definedBy>.
 
-<TriplesMap1> a rr:TriplesMap;
+<TriplesMap1> a rml:TriplesMap;
 
   rml:logicalSource [
     rml:source [
 			a sd:DatasetSpecification;
 			sd:name "variable1";
 			sd:hasDataTransformation [
-				sd:hasSoftwareRequirements "pandas>=1.1.0";
 				sd:hasSourceCode [
 					sd:programmingLanguage "Python3.9";
 				];
 			];
 		];
-    rml:referenceFormulation ql:CSV
+		rml:referenceFormulation rml:Dictionary;
+    rml:iterator "$.students[*]"
   ];
 
-  rr:subjectMap [
-    rr:template "http://example.com/Student/{ID}/{FirstName}";
-    rr:graph ex:PersonGraph
+  rml:subjectMap [
+    rml:template "http://example.com/Student/{ID}/{FirstName}";
+    rml:graph ex:PersonGraph
   ];
 
-  rr:predicateObjectMap [
-    rr:predicate rdf:type;
-    rr:object foaf:Person;
+  rml:predicateObjectMap [
+    rml:predicate rdf:type;
+    rml:object foaf:Person;
   ];
 
-  rr:predicateObjectMap [
-    rr:predicate foaf:name;
-    rr:objectMap [ rml:reference "FirstName" ]
+  rml:predicateObjectMap [
+    rml:predicate foaf:name;
+    rml:objectMap [ rml:reference "FirstName" ]
   ].
 
-ql:DataFrame a rml:ReferenceFormulation;
-	kg4di:definedBy "Pandas".
+rml:Dictionary a rml:ReferenceFormulation;
+	kg4di:definedBy "Python".
```

### Comparing `morph_kgc-2.6.4/test/rml-in-memory/pandas_dataframe/RMLIMTC0007b/test_RMLIMTC0007b_DF.py` & `morph_kgc-2.7.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0007b/test_RMLIMTC0007b_DF.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/rml-in-memory/pandas_dataframe/RMLIMTC0007c/test_RMLIMTC0007c_DF.py` & `morph_kgc-2.7.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0007c/test_RMLIMTC0007c_DF.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/rml-in-memory/pandas_dataframe/RMLIMTC0007d/mapping.ttl` & `morph_kgc-2.7.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0009a/mapping.ttl`

 * *Files 18% similar despite different names*

```diff
@@ -1,53 +1,72 @@
-@prefix rr: <http://www.w3.org/ns/r2rml#> .
 @prefix foaf: <http://xmlns.com/foaf/0.1/> .
 @prefix ex: <http://example.com/> .
 @prefix xsd: <http://www.w3.org/2001/XMLSchema#> .
-@prefix rml: <http://semweb.mmlab.be/ns/rml#> .
-@prefix ql: <http://semweb.mmlab.be/ns/ql#> .
-@prefix rdf: <http://www.w3.org/1999/02/22-rdf-syntax-ns#> .
+@prefix rml: <http://w3id.org/rml/> .
+@prefix activity: <http://example.com/activity/> .
+@prefix rdfs: <http://www.w3.org/2000/01/rdf-schema#> .
 @base <http://example.com/base/> .
 @prefix sd: <https://w3id.org/okn/o/sd#>.
 @prefix kg4di: <https://w3id.org/kg4di/definedBy>.
 
-<TriplesMap1> a rr:TriplesMap;
+<TriplesMap1>
+  a rml:TriplesMap;
 
   rml:logicalSource [
     rml:source [
 			a sd:DatasetSpecification;
 			sd:name "variable1";
 			sd:hasDataTransformation [
 				sd:hasSoftwareRequirements "pandas>=1.1.0";
 				sd:hasSourceCode [
 					sd:programmingLanguage "Python3.9";
 				];
 			];
 		];
-    rml:referenceFormulation ql:DataFrame;
+    rml:referenceFormulation rml:DataFrame;
   ];
 
-  rr:subjectMap [
-    rr:template "http://example.com/Student/{ID}/{FirstName}"
-  ];
+  rml:subjectMap [ rml:template "http://example.com/resource/student_{ID}" ];
 
-  rr:predicateObjectMap [
-    rr:predicate rdf:type;
-    rr:object foaf:Person;
-  ];
+  rml:predicateObjectMap [
+    rml:predicate foaf:name ;
+    rml:objectMap [ rml:reference "Name" ]
+  ] ;
+
+  rml:predicateObjectMap [
+    rml:predicate <http://example.com/ontology/practises> ;
+    rml:objectMap [
+      a rml:RefObjectMap ;
+      rml:parentTriplesMap <TriplesMap2>;
+      rml:joinCondition [
+        rml:child "Sport" ;
+        rml:parent "ID" ;
+      ]
+    ]
+  ] .
 
-  rr:predicateObjectMap [
-    rr:predicate rdf:type;
-    rr:object ex:Student;
-  ];
+<TriplesMap2>
+  a rml:TriplesMap;
 
-  rr:predicateObjectMap [
-    rr:predicate ex:id;
-    rr:objectMap [ rml:reference "ID" ]
+  rml:logicalSource [
+    rml:source [
+			a sd:DatasetSpecification;
+			sd:name "variable2";
+			sd:hasDataTransformation [
+				sd:hasSoftwareRequirements "pandas>=1.1.0";
+				sd:hasSourceCode [
+					sd:programmingLanguage "Python3.9";
+				];
+			];
+		];
+    rml:referenceFormulation rml:DataFrame;
   ];
 
-  rr:predicateObjectMap [
-    rr:predicate foaf:name;
-    rr:objectMap [ rml:reference "FirstName" ]
+  rml:subjectMap [ rml:template "http://example.com/resource/sport_{ID}" ];
+
+  rml:predicateObjectMap [
+    rml:predicate rdfs:label ;
+    rml:objectMap [ rml:reference "Name" ];
   ].
 
-ql:DataFrame a rml:ReferenceFormulation;
-	kg4di:definedBy "Pandas".
+rml:DataFrame a rml:ReferenceFormulation;
+	kg4di:definedBy "Pandas".
```

### Comparing `morph_kgc-2.6.4/test/rml-in-memory/pandas_dataframe/RMLIMTC0007d/test_RMLTC0007d_DF.py` & `morph_kgc-2.7.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0007d/test_RMLTC0007d_DF.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/rml-in-memory/pandas_dataframe/RMLIMTC0007e/mapping.ttl` & `morph_kgc-2.7.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0011b/mapping.ttl`

 * *Files 25% similar despite different names*

```diff
@@ -1,45 +1,109 @@
-@prefix rr: <http://www.w3.org/ns/r2rml#> .
 @prefix foaf: <http://xmlns.com/foaf/0.1/> .
 @prefix ex: <http://example.com/> .
 @prefix xsd: <http://www.w3.org/2001/XMLSchema#> .
-@prefix rml: <http://semweb.mmlab.be/ns/rml#> .
-@prefix ql: <http://semweb.mmlab.be/ns/ql#> .
-@base <http://example.com/base/> .
+@prefix rml: <http://w3id.org/rml/> .
 @prefix sd: <https://w3id.org/okn/o/sd#>.
 @prefix kg4di: <https://w3id.org/kg4di/definedBy>.
 
-<TriplesMap1> a rr:TriplesMap;
+@base <http://example.com/base/> .
+
+<TriplesMap1>
+  a rml:TriplesMap;
 
   rml:logicalSource [
     rml:source [
 			a sd:DatasetSpecification;
 			sd:name "variable1";
 			sd:hasDataTransformation [
 				sd:hasSoftwareRequirements "pandas>=1.1.0";
 				sd:hasSourceCode [
 					sd:programmingLanguage "Python3.9";
 				];
 			];
 		];
-    rml:referenceFormulation ql:DataFrame;
+    rml:referenceFormulation rml:DataFrame;
+  ];
+
+  rml:subjectMap [
+    rml:template "http://example.com/student/{ID}";
   ];
 
-  rr:subjectMap [
-    rr:template "http://example.com/Student/{ID}/{Name}";
-    rr:graph ex:PersonGraph ;
-    rr:class foaf:Person
+  rml:predicateObjectMap [
+    rml:predicate ex:firstName;
+    rml:objectMap [
+      rml:reference "FirstName"
+    ]
+  ];
+
+  rml:predicateObjectMap [
+    rml:predicate ex:lastName;
+    rml:objectMap [
+      rml:reference "LastName"
+    ]
+  ].
+
+<TriplesMap2>
+  a rml:TriplesMap;
+
+  rml:logicalSource [
+    rml:source [
+			a sd:DatasetSpecification;
+			sd:name "variable2";
+			sd:hasDataTransformation [
+				sd:hasSoftwareRequirements "pandas>=1.1.0";
+				sd:hasSourceCode [
+					sd:programmingLanguage "Python3.9";
+				];
+			];
+		];
+    rml:referenceFormulation rml:DataFrame;
+  ];
+
+  rml:subjectMap [
+    rml:template "http://example.com/sport/{ID}";
+  ];
+
+  rml:predicateObjectMap [
+    rml:predicate ex:id;
+    rml:objectMap [
+      rml:reference "ID"
+    ]
+  ];
+
+  rml:predicateObjectMap [
+    rml:predicate ex:description;
+    rml:objectMap [
+      rml:reference "Description"
+    ]
+  ].
+
+<LinkMap_1_2>
+  a rml:TriplesMap;
+
+  rml:logicalSource [
+    rml:source [
+			a sd:DatasetSpecification;
+			sd:name "variable3";
+			sd:hasDataTransformation [
+				sd:hasSoftwareRequirements "pandas>=1.1.0";
+				sd:hasSourceCode [
+					sd:programmingLanguage "Python3.9";
+				];
+			];
+		];
+    rml:referenceFormulation rml:DataFrame;
   ];
 
-  rr:predicateObjectMap [
-    rr:predicate ex:id ;
-    rr:objectMap [ rml:reference "ID"; ]
+  rml:subjectMap [
+    rml:template "http://example.com/student/{ID_Student}";
   ];
 
-  rr:predicateObjectMap
-    [
-      rr:predicate		foaf:name ;
-      rr:objectMap		[ rml:reference "Name" ]
-    ].
+  rml:predicateObjectMap [
+    rml:predicate ex:plays;
+    rml:objectMap [
+      rml:template "http://example.com/sport/{ID_Sport}"
+    ]
+  ].
 
-ql:DataFrame a rml:ReferenceFormulation;
+rml:DataFrame a rml:ReferenceFormulation;
 	kg4di:definedBy "Pandas".
```

### Comparing `morph_kgc-2.6.4/test/rml-in-memory/pandas_dataframe/RMLIMTC0007e/test_RMLIMTC0007e_DF.py` & `morph_kgc-2.7.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0007e/test_RMLIMTC0007e_DF.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/rml-in-memory/pandas_dataframe/RMLIMTC0007f/mapping.ttl` & `morph_kgc-2.7.0/test/rml-in-memory/json_dictionary/RMLIMTC0006a/mapping.ttl`

 * *Files 24% similar despite different names*

```diff
@@ -1,49 +1,36 @@
-@prefix rr: <http://www.w3.org/ns/r2rml#> .
 @prefix foaf: <http://xmlns.com/foaf/0.1/> .
 @prefix ex: <http://example.com/> .
 @prefix xsd: <http://www.w3.org/2001/XMLSchema#> .
-@prefix rml: <http://semweb.mmlab.be/ns/rml#> .
-@prefix ql: <http://semweb.mmlab.be/ns/ql#> .
-@prefix rdf: <http://www.w3.org/1999/02/22-rdf-syntax-ns#> .
+@prefix rml: <http://w3id.org/rml/> .
 @base <http://example.com/base/> .
 @prefix sd: <https://w3id.org/okn/o/sd#>.
 @prefix kg4di: <https://w3id.org/kg4di/definedBy>.
 
-<TriplesMap1> a rr:TriplesMap;
+<TriplesMap1> a rml:TriplesMap;
 
   rml:logicalSource [
     rml:source [
 			a sd:DatasetSpecification;
 			sd:name "variable1";
 			sd:hasDataTransformation [
-				sd:hasSoftwareRequirements "pandas>=1.1.0";
 				sd:hasSourceCode [
 					sd:programmingLanguage "Python3.9";
 				];
 			];
 		];
-    rml:referenceFormulation ql:DataFrame;
+		rml:referenceFormulation rml:Dictionary;
+    rml:iterator "$.students[*]"
   ];
 
-  rr:subjectMap [
-    rr:template "http://example.com/Student/{ID}/{FirstName}";
-    rr:graph ex:PersonGraph
+  rml:subjectMap [
+    rml:constant ex:BadStudent;
+    rml:graphMap [ rml:constant <http://example.com/graph/student> ];
   ];
 
-  rr:predicateObjectMap [
-    rr:predicate rdf:type;
-    rr:object foaf:Person
-  ];
-
-  rr:predicateObjectMap [
-    rr:predicate ex:id ;
-    rr:objectMap [ rml:reference "ID";  ]
-  ];
-
-  rr:predicateObjectMap [
-    rr:predicate foaf:name ;
-    rr:objectMap [ rml:reference "FirstName" ]
+  rml:predicateObjectMap [
+    rml:predicateMap [ rml:constant ex:description ];
+    rml:objectMap [ rml:constant "Bad Student"; ]
   ].
 
-ql:DataFrame a rml:ReferenceFormulation;
-	kg4di:definedBy "Pandas".
+rml:Dictionary a rml:ReferenceFormulation;
+	kg4di:definedBy "Python".
```

### Comparing `morph_kgc-2.6.4/test/rml-in-memory/pandas_dataframe/RMLIMTC0007f/test_RMLIMTC0007f_DF.py` & `morph_kgc-2.7.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0007f/test_RMLIMTC0007f_DF.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/rml-in-memory/pandas_dataframe/RMLIMTC0007g/test_RMLIMTC0007g_DF.py` & `morph_kgc-2.7.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0007g/test_RMLIMTC0007g_DF.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/rml-in-memory/pandas_dataframe/RMLIMTC0007h/test_RMLIMTC0007h_DF.py` & `morph_kgc-2.7.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0007h/test_RMLIMTC0007h_DF.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/rml-in-memory/pandas_dataframe/RMLIMTC0008a/output.nq` & `morph_kgc-2.7.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0008a/output.nq`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/rml-in-memory/pandas_dataframe/RMLIMTC0008a/test_RMLIMTC0008a_DF.py` & `morph_kgc-2.7.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0008a/test_RMLIMTC0008a_DF.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/rml-in-memory/pandas_dataframe/RMLIMTC0008b/mapping.ttl` & `morph_kgc-2.7.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0008b/mapping.ttl`

 * *Files 26% similar despite different names*

```diff
@@ -1,81 +1,79 @@
-@prefix rr: <http://www.w3.org/ns/r2rml#> .
 @prefix foaf: <http://xmlns.com/foaf/0.1/> .
 @prefix ex: <http://example.com/> .
 @prefix xsd: <http://www.w3.org/2001/XMLSchema#> .
-@prefix rml: <http://semweb.mmlab.be/ns/rml#> .
-@prefix ql: <http://semweb.mmlab.be/ns/ql#> .
+@prefix rml: <http://w3id.org/rml/> .
 @prefix activity: <http://example.com/activity/> .
 @prefix rdf: <http://www.w3.org/1999/02/22-rdf-syntax-ns#> .
 @base <http://example.com/base/> .
 @prefix sd: <https://w3id.org/okn/o/sd#>.
 @prefix kg4di: <https://w3id.org/kg4di/definedBy>.
 
 <TriplesMap2>
-  a rr:TriplesMap;
+  a rml:TriplesMap;
   rml:logicalSource [
     rml:source [
 			a sd:DatasetSpecification;
 			sd:name "variable1";
 			sd:hasDataTransformation [
 				sd:hasSoftwareRequirements "pandas>=1.1.0";
 				sd:hasSourceCode [
 					sd:programmingLanguage "Python3.9";
 				];
 			];
 		];
-    rml:referenceFormulation ql:CSV
+    rml:referenceFormulation rml:CSV
   ];
 
-  rr:subjectMap [ rr:template "http://example.com/{Sport}" ];
+  rml:subjectMap [ rml:template "http://example.com/{Sport}" ];
 
-  rr:predicateObjectMap [
-    rr:predicate rdf:type ;
-    rr:object activity:Sport ;
+  rml:predicateObjectMap [
+    rml:predicate rdf:type ;
+    rml:object activity:Sport ;
   ] .
 
 <TriplesMap1>
-  a rr:TriplesMap;
+  a rml:TriplesMap;
 
   rml:logicalSource [
     rml:source [
 			a sd:DatasetSpecification;
 			sd:name "variable1";
 			sd:hasDataTransformation [
 				sd:hasSoftwareRequirements "pandas>=1.1.0";
 				sd:hasSourceCode [
 					sd:programmingLanguage "Python3.9";
 				];
 			];
 		];
-    rml:referenceFormulation ql:DataFrame;
+    rml:referenceFormulation rml:DataFrame;
   ];
 
-  rr:subjectMap [ rr:template "http://example.com/Student/{ID}/{Name}" ];
+  rml:subjectMap [ rml:template "http://example.com/Student/{ID}/{Name}" ];
 
-  rr:predicateObjectMap [
-    rr:predicate rdf:type ;
-    rr:object foaf:Person ;
+  rml:predicateObjectMap [
+    rml:predicate rdf:type ;
+    rml:object foaf:Person ;
   ];
 
-  rr:predicateObjectMap [
-    rr:predicate ex:id ;
-    rr:objectMap [ rml:reference "ID"; ]
+  rml:predicateObjectMap [
+    rml:predicate ex:id ;
+    rml:objectMap [ rml:reference "ID"; ]
   ];
 
-  rr:predicateObjectMap [
-    rr:predicate foaf:name ;
-    rr:objectMap [ rml:reference "Name" ]
+  rml:predicateObjectMap [
+    rml:predicate foaf:name ;
+    rml:objectMap [ rml:reference "Name" ]
   ];
 
-  rr:predicateObjectMap [
-    rr:predicate ex:Sport ;
-    rr:objectMap <RefObjectMap1>
+  rml:predicateObjectMap [
+    rml:predicate ex:Sport ;
+    rml:objectMap <RefObjectMap1>
   ] .
 
 
 <RefObjectMap1>
-  a rr:RefObjectMap;
-  rr:parentTriplesMap <TriplesMap2> .
+  a rml:RefObjectMap;
+  rml:parentTriplesMap <TriplesMap2> .
 
-ql:DataFrame a rml:ReferenceFormulation;
+rml:DataFrame a rml:ReferenceFormulation;
 	kg4di:definedBy "Pandas".
```

### Comparing `morph_kgc-2.6.4/test/rml-in-memory/pandas_dataframe/RMLIMTC0008b/output.nq` & `morph_kgc-2.7.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0008b/output.nq`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/rml-in-memory/pandas_dataframe/RMLIMTC0008b/test_RMLIMTC0008b_DF.py` & `morph_kgc-2.7.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0008b/test_RMLIMTC0008b_DF.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/rml-in-memory/pandas_dataframe/RMLIMTC0008c/test_RMLIMTC0008c_DF.py` & `morph_kgc-2.7.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0008c/test_RMLIMTC0008c_DF.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/rml-in-memory/pandas_dataframe/RMLIMTC0009a/mapping.ttl` & `morph_kgc-2.7.0/test/rml-in-memory/json_dictionary/RMLIMTC0009a/mapping.ttl`

 * *Files 21% similar despite different names*

```diff
@@ -1,74 +1,72 @@
-@prefix rr: <http://www.w3.org/ns/r2rml#> .
 @prefix foaf: <http://xmlns.com/foaf/0.1/> .
 @prefix ex: <http://example.com/> .
 @prefix xsd: <http://www.w3.org/2001/XMLSchema#> .
-@prefix rml: <http://semweb.mmlab.be/ns/rml#> .
-@prefix ql: <http://semweb.mmlab.be/ns/ql#> .
+@prefix rml: <http://w3id.org/rml/> .
 @prefix activity: <http://example.com/activity/> .
 @prefix rdfs: <http://www.w3.org/2000/01/rdf-schema#> .
 @base <http://example.com/base/> .
 @prefix sd: <https://w3id.org/okn/o/sd#>.
 @prefix kg4di: <https://w3id.org/kg4di/definedBy>.
 
 <TriplesMap1>
-  a rr:TriplesMap;
+  a rml:TriplesMap;
 
   rml:logicalSource [
     rml:source [
 			a sd:DatasetSpecification;
-			sd:name "variable1";
+			sd:name "variable2";
 			sd:hasDataTransformation [
-				sd:hasSoftwareRequirements "pandas>=1.1.0";
 				sd:hasSourceCode [
 					sd:programmingLanguage "Python3.9";
 				];
 			];
 		];
-    rml:referenceFormulation ql:DataFrame;
+		rml:referenceFormulation rml:Dictionary;
+    rml:iterator "$.students[*]"
   ];
 
-  rr:subjectMap [ rr:template "http://example.com/resource/student_{ID}" ];
+  rml:subjectMap [ rml:template "http://example.com/resource/student_{ID}" ];
 
-  rr:predicateObjectMap [
-    rr:predicate foaf:name ;
-    rr:objectMap [ rml:reference "Name" ]
+  rml:predicateObjectMap [
+    rml:predicate foaf:name ;
+    rml:objectMap [ rml:reference "Name" ]
   ] ;
 
-  rr:predicateObjectMap [
-    rr:predicate <http://example.com/ontology/practises> ;
-    rr:objectMap [
-      a rr:RefObjectMap ;
-      rr:parentTriplesMap <TriplesMap2>;
-      rr:joinCondition [
-        rr:child "Sport" ;
-        rr:parent "ID" ;
+  rml:predicateObjectMap [
+    rml:predicate <http://example.com/ontology/practises> ;
+    rml:objectMap [
+      a rml:RefObjectMap ;
+      rml:parentTriplesMap <TriplesMap2>;
+      rml:joinCondition [
+        rml:child "Sport" ;
+        rml:parent "ID" ;
       ]
     ]
   ] .
 
 <TriplesMap2>
-  a rr:TriplesMap;
+  a rml:TriplesMap;
 
   rml:logicalSource [
     rml:source [
 			a sd:DatasetSpecification;
-			sd:name "variable2";
+			sd:name "variable1";
 			sd:hasDataTransformation [
-				sd:hasSoftwareRequirements "pandas>=1.1.0";
 				sd:hasSourceCode [
 					sd:programmingLanguage "Python3.9";
 				];
 			];
 		];
-    rml:referenceFormulation ql:DataFrame;
+		rml:referenceFormulation rml:Dictionary;
+    rml:iterator "$.sports[*]"
   ];
 
-  rr:subjectMap [ rr:template "http://example.com/resource/sport_{ID}" ];
+  rml:subjectMap [ rml:template "http://example.com/resource/sport_{ID}" ];
 
-  rr:predicateObjectMap [
-    rr:predicate rdfs:label ;
-    rr:objectMap [ rml:reference "Name" ];
+  rml:predicateObjectMap [
+    rml:predicate rdfs:label ;
+    rml:objectMap [ rml:reference "Name" ];
   ].
 
-ql:DataFrame a rml:ReferenceFormulation;
-	kg4di:definedBy "Pandas".
+rml:Dictionary a rml:ReferenceFormulation;
+	kg4di:definedBy "Python".
```

### Comparing `morph_kgc-2.6.4/test/rml-in-memory/pandas_dataframe/RMLIMTC0009a/test_RMLIMTC0009a_DF.py` & `morph_kgc-2.7.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0009a/test_RMLIMTC0009a_DF.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/rml-in-memory/pandas_dataframe/RMLIMTC0009b/mapping.ttl` & `morph_kgc-2.7.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0012b/mapping.ttl`

 * *Files 18% similar despite different names*

```diff
@@ -1,84 +1,72 @@
-@prefix rr: <http://www.w3.org/ns/r2rml#> .
 @prefix foaf: <http://xmlns.com/foaf/0.1/> .
 @prefix ex: <http://example.com/> .
 @prefix xsd: <http://www.w3.org/2001/XMLSchema#> .
-@prefix rml: <http://semweb.mmlab.be/ns/rml#> .
-@prefix ql: <http://semweb.mmlab.be/ns/ql#> .
-@prefix activity: <http://example.com/activity/> .
-@prefix rdfs: <http://www.w3.org/2000/01/rdf-schema#> .
-@base <http://example.com/base/> .
+@prefix rml: <http://w3id.org/rml/> .
 @prefix sd: <https://w3id.org/okn/o/sd#>.
 @prefix kg4di: <https://w3id.org/kg4di/definedBy>.
+@base <http://example.com/base/> .
 
 <TriplesMap1>
-  a rr:TriplesMap;
+  a rml:TriplesMap;
 
   rml:logicalSource [
     rml:source [
 			a sd:DatasetSpecification;
 			sd:name "variable1";
 			sd:hasDataTransformation [
 				sd:hasSoftwareRequirements "pandas>=1.1.0";
 				sd:hasSourceCode [
 					sd:programmingLanguage "Python3.9";
 				];
 			];
 		];
-    rml:referenceFormulation ql:DataFrame;
+    rml:referenceFormulation rml:DataFrame;
   ];
 
-  rr:subjectMap [
-    rr:template "http://example.com/resource/student_{ID}" ;
-    rr:class <http://example.com/ontology/Student>;
-    rr:graph <http://example.com/graph/students> ;
+  rml:subjectMap [
+    rml:template "{fname}{lname}";
+    rml:termType rml:BlankNode ;
   ];
 
-  rr:predicateObjectMap [
-    rr:predicate foaf:name ;
-    rr:objectMap [ rml:reference "Name" ];
-    rr:graph <http://example.com/graph/students> ;
-  ] ;
-
-  rr:predicateObjectMap [
-    rr:predicate <http://example.com/ontology/practises> ;
-    rr:objectMap [
-      a rr:RefObjectMap ;
-      rr:parentTriplesMap <TriplesMap2>;
-      rr:joinCondition [
-        rr:child "Sport" ;
-        rr:parent "ID" ;
-      ]
-    ];
-    rr:graph <http://example.com/graph/practise> ;
-  ] .
+  rml:predicateObjectMap [
+    rml:predicate foaf:name ;
+    rml:objectMap [
+      rml:template "{fname} {lname}";
+      rml:termType rml:Literal ;
+    ]
+  ];
+  .
 
 <TriplesMap2>
-  a rr:TriplesMap;
+  a rml:TriplesMap;
 
   rml:logicalSource [
     rml:source [
 			a sd:DatasetSpecification;
 			sd:name "variable2";
 			sd:hasDataTransformation [
 				sd:hasSoftwareRequirements "pandas>=1.1.0";
 				sd:hasSourceCode [
 					sd:programmingLanguage "Python3.9";
 				];
 			];
 		];
-    rml:referenceFormulation ql:CSV
-  ];
+    rml:referenceFormulation rml:DataFrame;
+];
 
-  rr:subjectMap [
-    rr:template "http://example.com/resource/sport_{ID}";
-    rr:class <http://example.com/ontology/Sport>;
-    rr:graph <http://example.com/graph/sports> ;
+  rml:subjectMap [
+    rml:template "{fname}{lname}";
+    rml:termType rml:BlankNode;
   ];
 
-  rr:predicateObjectMap [
-    rr:predicate rdfs:label ;
-    rr:objectMap [ rml:reference "Name" ];
-  ].
+  rml:predicateObjectMap
+  [
+    rml:predicate	ex:city ;
+    rml:objectMap    [
+      rml:reference "city";
+    ]
+];
+.
 
-ql:DataFrame a rml:ReferenceFormulation;
+rml:DataFrame a rml:ReferenceFormulation;
 	kg4di:definedBy "Pandas".
```

### Comparing `morph_kgc-2.6.4/test/rml-in-memory/pandas_dataframe/RMLIMTC0009b/output.nq` & `morph_kgc-2.7.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0009b/output.nq`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/rml-in-memory/pandas_dataframe/RMLIMTC0009b/test_RMLIMTC0009b_DF.py` & `morph_kgc-2.7.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0009b/test_RMLIMTC0009b_DF.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/rml-in-memory/pandas_dataframe/RMLIMTC0010a/test_RMLIMTC0010a_DF.py` & `morph_kgc-2.7.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0010a/test_RMLIMTC0010a_DF.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/rml-in-memory/pandas_dataframe/RMLIMTC0010b/mapping.ttl` & `morph_kgc-2.7.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0002e/mapping.ttl`

 * *Files 19% similar despite different names*

```diff
@@ -1,37 +1,35 @@
-@prefix rr: <http://www.w3.org/ns/r2rml#> .
 @prefix foaf: <http://xmlns.com/foaf/0.1/> .
 @prefix ex: <http://example.com/> .
 @prefix xsd: <http://www.w3.org/2001/XMLSchema#> .
-@prefix rml: <http://semweb.mmlab.be/ns/rml#> .
-@prefix ql: <http://semweb.mmlab.be/ns/ql#> .
-@prefix activity: <http://example.com/activity/> .
+@prefix rml: <http://w3id.org/rml/> .
 @base <http://example.com/base/> .
 @prefix sd: <https://w3id.org/okn/o/sd#>.
 @prefix kg4di: <https://w3id.org/kg4di/definedBy>.
 
-<TriplesMap1>
-  a rr:TriplesMap;
+<TriplesMap1> a rml:TriplesMap;
 
   rml:logicalSource [
     rml:source [
 			a sd:DatasetSpecification;
 			sd:name "variable1";
 			sd:hasDataTransformation [
 				sd:hasSoftwareRequirements "pandas>=1.1.0";
 				sd:hasSourceCode [
 					sd:programmingLanguage "Python3.9";
 				];
 			];
 		];
-    rml:referenceFormulation ql:DataFrame;
+    rml:referenceFormulation rml:DataFrame;
   ];
 
-  rr:subjectMap [ rr:template "http://example.com/{Country Code}/{Name}" ];
+  rml:subjectMap [
+    rml:template "http://example.com/{ID}/{Name}";
+  ];
 
-  rr:predicateObjectMap [
-    rr:predicate ex:name ;
-    rr:objectMap [ rml:reference "Name" ]
-  ] .
+  rml:predicateObjectMap [
+    rml:predicate ex:id ;
+    rml:objectMap [ rml:reference "ID" ]
+  ].
 
-ql:DataFrame a rml:ReferenceFormulation;
+rml:DataFrame a rml:ReferenceFormulation;
 	kg4di:definedBy "Pandas".
```

### Comparing `morph_kgc-2.6.4/test/rml-in-memory/pandas_dataframe/RMLIMTC0010b/test_RMLIMTC0010b_DF.py` & `morph_kgc-2.7.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0010b/test_RMLIMTC0010b_DF.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/rml-in-memory/pandas_dataframe/RMLIMTC0010c/test_RMLIMTC0010c_DF.py` & `morph_kgc-2.7.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0010c/test_RMLIMTC0010c_DF.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/rml-in-memory/pandas_dataframe/RMLIMTC0011b/output.nq` & `morph_kgc-2.7.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0011b/output.nq`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/rml-in-memory/pandas_dataframe/RMLIMTC0011b/test_RMLIMTC0011b_DF.py` & `morph_kgc-2.7.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0011b/test_RMLIMTC0011b_DF.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/rml-in-memory/pandas_dataframe/RMLIMTC0012a/test_RMLIMTC0012a_DF.py` & `morph_kgc-2.7.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0012a/test_RMLIMTC0012a_DF.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/rml-in-memory/pandas_dataframe/RMLIMTC0012b/mapping.ttl` & `morph_kgc-2.7.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0002b/mapping.ttl`

 * *Files 24% similar despite different names*

```diff
@@ -1,74 +1,36 @@
-@prefix rr: <http://www.w3.org/ns/r2rml#> .
 @prefix foaf: <http://xmlns.com/foaf/0.1/> .
 @prefix ex: <http://example.com/> .
 @prefix xsd: <http://www.w3.org/2001/XMLSchema#> .
-@prefix rml: <http://semweb.mmlab.be/ns/rml#> .
-@prefix ql: <http://semweb.mmlab.be/ns/ql#> .
+@prefix rml: <http://w3id.org/rml/> .
+@base <http://example.com/base/> .
 @prefix sd: <https://w3id.org/okn/o/sd#>.
 @prefix kg4di: <https://w3id.org/kg4di/definedBy>.
-@base <http://example.com/base/> .
 
-<TriplesMap1>
-  a rr:TriplesMap;
+<TriplesMap1> a rml:TriplesMap;
 
   rml:logicalSource [
     rml:source [
 			a sd:DatasetSpecification;
 			sd:name "variable1";
 			sd:hasDataTransformation [
 				sd:hasSoftwareRequirements "pandas>=1.1.0";
 				sd:hasSourceCode [
 					sd:programmingLanguage "Python3.9";
 				];
 			];
 		];
-    rml:referenceFormulation ql:DataFrame;
+    rml:referenceFormulation rml:DataFrame;
   ];
 
-  rr:subjectMap [
-    rr:template "{fname}{lname}";
-    rr:termType rr:BlankNode ;
-  ];
-
-  rr:predicateObjectMap [
-    rr:predicate foaf:name ;
-    rr:objectMap [
-      rr:template "{fname} {lname}";
-      rr:termType rr:Literal ;
-    ]
-  ];
-  .
-
-<TriplesMap2>
-  a rr:TriplesMap;
-
-  rml:logicalSource [
-    rml:source [
-			a sd:DatasetSpecification;
-			sd:name "variable2";
-			sd:hasDataTransformation [
-				sd:hasSoftwareRequirements "pandas>=1.1.0";
-				sd:hasSourceCode [
-					sd:programmingLanguage "Python3.9";
-				];
-			];
-		];
-    rml:referenceFormulation ql:DataFrame;
-];
-
-  rr:subjectMap [
-    rr:template "{fname}{lname}";
-    rr:termType rr:BlankNode;
+  rml:subjectMap [
+    rml:template "students{ID}";
+    rml:termType rml:BlankNode
   ];
 
-  rr:predicateObjectMap
-  [
-    rr:predicate	ex:city ;
-    rr:objectMap    [
-      rml:reference "city";
-    ]
-];
-.
+  rml:predicateObjectMap [
+    rml:predicate foaf:name;
+    rml:objectMap [ rml:reference "Name" ]
+  ].
 
-ql:DataFrame a rml:ReferenceFormulation;
+rml:DataFrame a rml:ReferenceFormulation;
 	kg4di:definedBy "Pandas".
```

### Comparing `morph_kgc-2.6.4/test/rml-in-memory/pandas_dataframe/RMLIMTC0012b/test_RMLIMTC0012b_DF.py` & `morph_kgc-2.7.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0012b/test_RMLIMTC0012b_DF.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/rml-in-memory/pandas_dataframe/RMLIMTC0012c/test_RMLIMTC0012c_DF.py` & `morph_kgc-2.7.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0012c/test_RMLIMTC0012c_DF.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/rml-in-memory/pandas_dataframe/RMLIMTC0012d/test_RMLIMTC0012d_DF.py` & `morph_kgc-2.7.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0012d/test_RMLIMTC0012d_DF.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/rml-in-memory/pandas_dataframe/RMLIMTC0015a/test_RMLIMTC0015a_DF.py` & `morph_kgc-2.7.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0015a/test_RMLIMTC0015a_DF.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/rml-in-memory/pandas_dataframe/RMLIMTC0015b/test_RMLIMTC0015b_DF.py` & `morph_kgc-2.7.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0015b/test_RMLIMTC0015b_DF.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/rml-in-memory/pandas_dataframe/RMLIMTC0016a/mapping.ttl` & `morph_kgc-2.7.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0004b/mapping.ttl`

 * *Files 21% similar despite different names*

```diff
@@ -1,39 +1,40 @@
-@prefix rr: <http://www.w3.org/ns/r2rml#> .
 @prefix foaf: <http://xmlns.com/foaf/0.1/> .
-@prefix rdfs: <http://www.w3.org/2000/01/rdf-schema#> .
 @prefix ex: <http://example.com/> .
 @prefix xsd: <http://www.w3.org/2001/XMLSchema#> .
-@prefix rml: <http://semweb.mmlab.be/ns/rml#> .
-@prefix ql: <http://semweb.mmlab.be/ns/ql#> .
+@prefix rml: <http://w3id.org/rml/> .
 @prefix sd: <https://w3id.org/okn/o/sd#>.
 @prefix kg4di: <https://w3id.org/kg4di/definedBy>.
+
 @base <http://example.com/base/> .
 
 <TriplesMap1>
-  a rr:TriplesMap;
+  a rml:TriplesMap;
 
   rml:logicalSource [
     rml:source [
 			a sd:DatasetSpecification;
 			sd:name "variable1";
 			sd:hasDataTransformation [
 				sd:hasSoftwareRequirements "pandas>=1.1.0";
 				sd:hasSourceCode [
 					sd:programmingLanguage "Python3.9";
 				];
 			];
 		];
-    rml:referenceFormulation ql:DataFrame;
+    rml:referenceFormulation rml:CSV
   ];
 
-  rr:subjectMap [ rr:template "http://example.com/{c1}" ];
+  rml:subjectMap [
+    rml:template "http://example.com/{Name}";
+    rml:termType rml:Literal
+  ];
 
-  rr:predicateObjectMap [
-    rr:predicate rdfs:label;
-    rr:objectMap [
-      rml:reference "c2"
+  rml:predicateObjectMap [
+    rml:predicate foaf:name;
+    rml:objectMap [
+      rml:reference "Name"
     ]
-  ] .
+  ].
 
-ql:DataFrame a rml:ReferenceFormulation;
+rml:DataFrame a rml:ReferenceFormulation;
 	kg4di:definedBy "Pandas".
```

### Comparing `morph_kgc-2.6.4/test/rml-in-memory/pandas_dataframe/RMLIMTC0016a/test_RMLIMTC0016a_DF.py` & `morph_kgc-2.7.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0016a/test_RMLIMTC0016a_DF.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/rml-in-memory/pandas_dataframe/triples_map_without_pom/test_triples_map_without_pom_DF.py` & `morph_kgc-2.7.0/test/rml-in-memory/pandas_dataframe/triples_map_without_pom/test_triples_map_without_pom_DF.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/rml-star/RMLSTARTC001a/mapping.ttl` & `morph_kgc-2.7.0/test/rml-star/RMLSTARTC001a/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/rml-star/RMLSTARTC001a/test_RMLSTARTC001a_CSV.py` & `morph_kgc-2.7.0/test/rml-star/RMLSTARTC001a/test_RMLSTARTC001a_CSV.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/rml-star/RMLSTARTC001b/mapping.ttl` & `morph_kgc-2.7.0/test/rml-star/RMLSTARTC002a/mapping.ttl`

 * *Files 12% similar despite different names*

```diff
@@ -1,40 +1,38 @@
 @prefix rdf: <http://www.w3.org/1999/02/22-rdf-syntax-ns#> .
 @prefix rml: <http://w3id.org/rml/> .
+@prefix xsd: <http://www.w3.org/2001/XMLSchema#> .
 @prefix ex: <http://example/> .
 @prefix : <http://example.org/> .
 @base <http://example.org/> .
 
 :firstTM a rml:AssertedTriplesMap ;
     rml:logicalSource [
-        rml:source "test/rml-star/RMLSTARTC001b/data1.csv";
+        rml:source "test/rml-star/RMLSTARTC002a/data.csv";
         rml:referenceFormulation rml:CSV
     ];
     rml:subjectMap [
-        rml:reference "c1-1" ;
-        rml:termType rml:BlankNode
+        rml:template "http://example/{c1}"
     ];
     rml:predicateObjectMap [
         rml:predicate ex:p ;
         rml:objectMap [
-            rml:template "http://example/{c1-2}"
+            rml:reference "c2" ;
+            rml:termType rml:BlankNode
         ]
     ] .
 
 :secondTM a rml:AssertedTriplesMap ;
     rml:logicalSource [
-        rml:source "test/rml-star/RMLSTARTC001b/data2.csv";
+        rml:source "test/rml-star/RMLSTARTC002a/data.csv";
         rml:referenceFormulation rml:CSV
     ];
     rml:subjectMap [
-        rml:quotedTriplesMap :firstTM ;
-        rml:joinCondition [
-          rml:child "c2-2" ;
-          rml:parent "c1-3" ;
-        ];
+        rml:quotedTriplesMap :firstTM
     ];
     rml:predicateObjectMap [
         rml:predicate ex:q ;
         rml:objectMap [
-            rml:reference "c2-1"
+            rml:reference "c3";
+            rml:datatype xsd:integer
         ]
     ] .
```

### Comparing `morph_kgc-2.6.4/test/rml-star/RMLSTARTC001b/test_RMLSTARTC001b_CSV.py` & `morph_kgc-2.7.0/test/rml-star/RMLSTARTC001b/test_RMLSTARTC001b_CSV.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/rml-star/RMLSTARTC002a/mapping.ttl` & `morph_kgc-2.7.0/test/rml-star/RMLSTARTC005b/mapping.ttl`

 * *Files 10% similar despite different names*

```diff
@@ -1,38 +1,40 @@
 @prefix rdf: <http://www.w3.org/1999/02/22-rdf-syntax-ns#> .
 @prefix rml: <http://w3id.org/rml/> .
-@prefix xsd: <http://www.w3.org/2001/XMLSchema#> .
 @prefix ex: <http://example/> .
+@prefix xsd: <http://www.w3.org/2001/XMLSchema#> .
 @prefix : <http://example.org/> .
 @base <http://example.org/> .
 
-:firstTM a rml:AssertedTriplesMap ;
+:firstTM a rml:NonAssertedTriplesMap ;
     rml:logicalSource [
-        rml:source "test/rml-star/RMLSTARTC002a/data.csv";
+        rml:source "test/rml-star/RMLSTARTC005b/data1.csv";
         rml:referenceFormulation rml:CSV
     ];
     rml:subjectMap [
-        rml:template "http://example/{c1}"
+        rml:template "http://example/{c1-1}"
     ];
     rml:predicateObjectMap [
         rml:predicate ex:p ;
         rml:objectMap [
-            rml:reference "c2" ;
-            rml:termType rml:BlankNode
+            rml:template "http://example/{c1-2}"
         ]
     ] .
 
 :secondTM a rml:AssertedTriplesMap ;
     rml:logicalSource [
-        rml:source "test/rml-star/RMLSTARTC002a/data.csv";
+        rml:source "test/rml-star/RMLSTARTC005b/data2.csv";
         rml:referenceFormulation rml:CSV
     ];
     rml:subjectMap [
-        rml:quotedTriplesMap :firstTM
+            rml:quotedTriplesMap :firstTM ;
+            rml:joinCondition [
+              rml:child "c2-2" ;
+              rml:parent "c1-3" ;
+            ];
     ];
     rml:predicateObjectMap [
         rml:predicate ex:q ;
         rml:objectMap [
-            rml:reference "c3";
-            rml:datatype xsd:integer
+            rml:template "http://example/{c2-1}"
         ]
     ] .
```

### Comparing `morph_kgc-2.6.4/test/rml-star/RMLSTARTC002a/test_RMLSTARTC002a_CSV.py` & `morph_kgc-2.7.0/test/rml-star/RMLSTARTC002a/test_RMLSTARTC002a_CSV.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/rml-star/RMLSTARTC002b/mapping.ttl` & `morph_kgc-2.7.0/test/rml-star/RMLSTARTC002b/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/rml-star/RMLSTARTC002b/test_RMLSTARTC002b_CSV.py` & `morph_kgc-2.7.0/test/rml-star/RMLSTARTC002b/test_RMLSTARTC002b_CSV.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/rml-star/RMLSTARTC003a/mapping.ttl` & `morph_kgc-2.7.0/test/rml-star/RMLSTARTC003a/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/rml-star/RMLSTARTC003a/test_RMLSTARTC003a_CSV.py` & `morph_kgc-2.7.0/test/rml-star/RMLSTARTC003a/test_RMLSTARTC003a_CSV.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/rml-star/RMLSTARTC003b/mapping.ttl` & `morph_kgc-2.7.0/test/rml-star/RMLSTARTC003b/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/rml-star/RMLSTARTC003b/test_RMLSTARTC003b_CSV.py` & `morph_kgc-2.7.0/test/rml-star/RMLSTARTC003b/test_RMLSTARTC003b_CSV.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/rml-star/RMLSTARTC004a/mapping.ttl` & `morph_kgc-2.7.0/test/rml-star/RMLSTARTC004a/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/rml-star/RMLSTARTC004a/test_RMLSTARTC004a_CSV.py` & `morph_kgc-2.7.0/test/rml-star/RMLSTARTC004a/test_RMLSTARTC004a_CSV.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/rml-star/RMLSTARTC004b/mapping.ttl` & `morph_kgc-2.7.0/test/rml-star/RMLSTARTC004b/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/rml-star/RMLSTARTC004b/test_RMLSTARTC004b_CSV.py` & `morph_kgc-2.7.0/test/rml-star/RMLSTARTC004b/test_RMLSTARTC004b_CSV.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/rml-star/RMLSTARTC005a/mapping.ttl` & `morph_kgc-2.7.0/test/rml-star/RMLSTARTC005a/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/rml-star/RMLSTARTC005a/test_RMLSTARTC005a_CSV.py` & `morph_kgc-2.7.0/test/rml-star/RMLSTARTC005a/test_RMLSTARTC005a_CSV.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/rml-star/RMLSTARTC005b/mapping.ttl` & `morph_kgc-2.7.0/test/rml-star/RMLSTARTC007a/mapping.ttl`

 * *Files 6% similar despite different names*

```diff
@@ -3,38 +3,49 @@
 @prefix ex: <http://example/> .
 @prefix xsd: <http://www.w3.org/2001/XMLSchema#> .
 @prefix : <http://example.org/> .
 @base <http://example.org/> .
 
 :firstTM a rml:NonAssertedTriplesMap ;
     rml:logicalSource [
-        rml:source "test/rml-star/RMLSTARTC005b/data1.csv";
+        rml:source "test/rml-star/RMLSTARTC007a/data.csv";
         rml:referenceFormulation rml:CSV
     ];
     rml:subjectMap [
-        rml:template "http://example/{c1-1}"
+        rml:template "http://example/{c1}"
     ];
     rml:predicateObjectMap [
-        rml:predicate ex:p ;
+        rml:predicate ex:p1 ;
         rml:objectMap [
-            rml:template "http://example/{c1-2}"
+            rml:template "http://example/{c2}"
         ]
     ] .
 
 :secondTM a rml:AssertedTriplesMap ;
     rml:logicalSource [
-        rml:source "test/rml-star/RMLSTARTC005b/data2.csv";
+        rml:source "test/rml-star/RMLSTARTC007a/data.csv";
         rml:referenceFormulation rml:CSV
     ];
     rml:subjectMap [
-            rml:quotedTriplesMap :firstTM ;
-            rml:joinCondition [
-              rml:child "c2-2" ;
-              rml:parent "c1-3" ;
-            ];
+            rml:quotedTriplesMap :firstTM
     ];
     rml:predicateObjectMap [
-        rml:predicate ex:q ;
+        rml:predicate ex:q; ;
         rml:objectMap [
-            rml:template "http://example/{c2-1}"
+            rml:quotedTriplesMap :thirdTM
+        ]
+    ] .
+
+:thirdTM a rml:NonAssertedTriplesMap ;
+    rml:logicalSource [
+        rml:source "test/rml-star/RMLSTARTC007a/data.csv";
+        rml:referenceFormulation rml:CSV
+    ];
+    rml:subjectMap [
+        rml:template "http://example/{c3}"
+    ];
+    rml:predicateObjectMap [
+        rml:predicate ex:p2 ;
+        rml:objectMap [
+            rml:template "http://example/{c4}"
         ]
     ] .
```

### Comparing `morph_kgc-2.6.4/test/rml-star/RMLSTARTC005b/test_RMLSTARTC005b_CSV.py` & `morph_kgc-2.7.0/test/rml-star/RMLSTARTC005b/test_RMLSTARTC005b_CSV.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/rml-star/RMLSTARTC006a/mapping.ttl` & `morph_kgc-2.7.0/test/rml-star/RMLSTARTC006b/mapping.ttl`

 * *Files 10% similar despite different names*

```diff
@@ -3,34 +3,38 @@
 @prefix ex: <http://example/> .
 @prefix xsd: <http://www.w3.org/2001/XMLSchema#> .
 @prefix : <http://example.org/> .
 @base <http://example.org/> .
 
 :firstTM a rml:NonAssertedTriplesMap ; # This refers to the y statement in the rdf-star
     rml:logicalSource [
-        rml:source "test/rml-star/RMLSTARTC006a/data.csv";
+        rml:source "test/rml-star/RMLSTARTC006b/data1.csv";
         rml:referenceFormulation rml:CSV
     ];
     rml:subjectMap [
-        rml:template "http://example/{c1}"
+        rml:template "http://example/{c1-1}"
     ];
     rml:predicateObjectMap [
         rml:predicate ex:p ;
         rml:objectMap [
-            rml:template "http://example/{c2}"
+            rml:template "http://example/{c1-2}"
         ]
     ] .
 
-:secondTM a rml:AssertedTriplesMap ;  # This refers to the x statement in the rdf-star
+:secondTM a rml:AssertedTriplesMap ; # This refers to the x statement in the rdf-star
     rml:logicalSource [
-        rml:source "test/rml-star/RMLSTARTC006a/data.csv";
+        rml:source "test/rml-star/RMLSTARTC006b/data2.csv";
         rml:referenceFormulation rml:CSV
     ];
     rml:subjectMap [
-            rml:template "http://example/{c3}"
+            rml:template "http://example/{c2-1}"
     ];
     rml:predicateObjectMap [
         rml:predicate ex:p; ;
         rml:objectMap [
-            rml:quotedTriplesMap :firstTM
+            rml:quotedTriplesMap :firstTM ;
+            rml:joinCondition [
+              rml:child "c2-2" ;
+              rml:parent "c1-3" ;
+            ];
         ]
     ] .
```

### Comparing `morph_kgc-2.6.4/test/rml-star/RMLSTARTC006a/test_RMLSTARTC006a_CSV.py` & `morph_kgc-2.7.0/test/rml-star/RMLSTARTC006a/test_RMLSTARTC006a_CSV.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/rml-star/RMLSTARTC006b/mapping.ttl` & `morph_kgc-2.7.0/test/rml-star/RMLSTARTC007b/mapping.ttl`

 * *Files 8% similar despite different names*

```diff
@@ -1,40 +1,55 @@
 @prefix rdf: <http://www.w3.org/1999/02/22-rdf-syntax-ns#> .
 @prefix rml: <http://w3id.org/rml/> .
 @prefix ex: <http://example/> .
 @prefix xsd: <http://www.w3.org/2001/XMLSchema#> .
 @prefix : <http://example.org/> .
 @base <http://example.org/> .
 
-:firstTM a rml:NonAssertedTriplesMap ; # This refers to the y statement in the rdf-star
+:firstTM a rml:NonAssertedTriplesMap ;
     rml:logicalSource [
-        rml:source "test/rml-star/RMLSTARTC006b/data1.csv";
+        rml:source "test/rml-star/RMLSTARTC007b/data1.csv";
         rml:referenceFormulation rml:CSV
     ];
     rml:subjectMap [
         rml:template "http://example/{c1-1}"
     ];
     rml:predicateObjectMap [
-        rml:predicate ex:p ;
+        rml:predicate ex:p1 ;
         rml:objectMap [
             rml:template "http://example/{c1-2}"
         ]
     ] .
 
-:secondTM a rml:AssertedTriplesMap ; # This refers to the x statement in the rdf-star
+:secondTM a rml:AssertedTriplesMap ;
     rml:logicalSource [
-        rml:source "test/rml-star/RMLSTARTC006b/data2.csv";
+        rml:source "test/rml-star/RMLSTARTC007b/data2.csv";
         rml:referenceFormulation rml:CSV
     ];
     rml:subjectMap [
-            rml:template "http://example/{c2-1}"
-    ];
-    rml:predicateObjectMap [
-        rml:predicate ex:p; ;
-        rml:objectMap [
             rml:quotedTriplesMap :firstTM ;
             rml:joinCondition [
-              rml:child "c2-2" ;
+              rml:child "c2-3" ;
               rml:parent "c1-3" ;
             ];
+    ];
+    rml:predicateObjectMap [
+        rml:predicate ex:q; ;
+        rml:objectMap [
+            rml:quotedTriplesMap :thirdTM
+        ]
+    ] .
+
+:thirdTM a rml:NonAssertedTriplesMap ;
+    rml:logicalSource [
+        rml:source "test/rml-star/RMLSTARTC007b/data2.csv";
+        rml:referenceFormulation rml:CSV
+    ];
+    rml:subjectMap [
+        rml:template "http://example/{c2-1}"
+    ];
+    rml:predicateObjectMap [
+        rml:predicate ex:p2 ;
+        rml:objectMap [
+            rml:template "http://example/{c2-2}"
         ]
     ] .
```

### Comparing `morph_kgc-2.6.4/test/rml-star/RMLSTARTC006b/test_RMLSTARTC006b_CSV.py` & `morph_kgc-2.7.0/test/rml-star/RMLSTARTC006b/test_RMLSTARTC006b_CSV.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/rml-star/RMLSTARTC007a/mapping.ttl` & `morph_kgc-2.7.0/test/rml-core/csv/RMLTC0015a/mapping.ttl`

 * *Files 16% similar despite different names*

```diff
@@ -1,51 +1,46 @@
-@prefix rdf: <http://www.w3.org/1999/02/22-rdf-syntax-ns#> .
-@prefix rml: <http://w3id.org/rml/> .
-@prefix ex: <http://example/> .
+@prefix foaf: <http://xmlns.com/foaf/0.1/> .
+@prefix ex: <http://example.com/> .
 @prefix xsd: <http://www.w3.org/2001/XMLSchema#> .
-@prefix : <http://example.org/> .
-@base <http://example.org/> .
+@prefix rml: <http://w3id.org/rml/> .
+@prefix rdfs: <http://www.w3.org/2000/01/rdf-schema#> .
+@base <http://example.com/base/> .
+
+<TriplesMap1>
+  a rml:TriplesMap;
+
+  rml:logicalSource [
+    rml:source "test/rml-core/csv/RMLTC0015a/country_en.csv";
+    rml:referenceFormulation rml:CSV
+  ];
+
+  rml:subjectMap [
+    rml:template "http://example.com/{Code}"
+  ];
+
+  rml:predicateObjectMap [
+    rml:predicate rdfs:label ;
+    rml:objectMap [
+      rml:reference "Name";
+      rml:language "en"
+    ]
+  ].
+
+<TriplesMap2>
+  a rml:TriplesMap;
+
+  rml:logicalSource [
+    rml:source "test/rml-core/csv/RMLTC0015a/country_es.csv";
+    rml:referenceFormulation rml:CSV
+  ];
+
+  rml:subjectMap [
+    rml:template "http://example.com/{Code}"
+  ];
 
-:firstTM a rml:NonAssertedTriplesMap ;
-    rml:logicalSource [
-        rml:source "test/rml-star/RMLSTARTC007a/data.csv";
-        rml:referenceFormulation rml:CSV
-    ];
-    rml:subjectMap [
-        rml:template "http://example/{c1}"
-    ];
-    rml:predicateObjectMap [
-        rml:predicate ex:p1 ;
-        rml:objectMap [
-            rml:template "http://example/{c2}"
-        ]
-    ] .
-
-:secondTM a rml:AssertedTriplesMap ;
-    rml:logicalSource [
-        rml:source "test/rml-star/RMLSTARTC007a/data.csv";
-        rml:referenceFormulation rml:CSV
-    ];
-    rml:subjectMap [
-            rml:quotedTriplesMap :firstTM
-    ];
-    rml:predicateObjectMap [
-        rml:predicate ex:q; ;
-        rml:objectMap [
-            rml:quotedTriplesMap :thirdTM
-        ]
-    ] .
-
-:thirdTM a rml:NonAssertedTriplesMap ;
-    rml:logicalSource [
-        rml:source "test/rml-star/RMLSTARTC007a/data.csv";
-        rml:referenceFormulation rml:CSV
-    ];
-    rml:subjectMap [
-        rml:template "http://example/{c3}"
-    ];
-    rml:predicateObjectMap [
-        rml:predicate ex:p2 ;
-        rml:objectMap [
-            rml:template "http://example/{c4}"
-        ]
-    ] .
+  rml:predicateObjectMap [
+    rml:predicate rdfs:label ;
+    rml:objectMap [
+      rml:reference "Name";
+      rml:language "es"
+    ]
+  ].
```

### Comparing `morph_kgc-2.6.4/test/rml-star/RMLSTARTC007a/test_RMLSTARTC007a_CSV.py` & `morph_kgc-2.7.0/test/rml-star/RMLSTARTC007a/test_RMLSTARTC007a_CSV.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/rml-star/RMLSTARTC007b/mapping.ttl` & `morph_kgc-2.7.0/test/rml-core/json/RMLTC0009a/mapping.ttl`

 * *Files 18% similar despite different names*

```diff
@@ -1,55 +1,51 @@
-@prefix rdf: <http://www.w3.org/1999/02/22-rdf-syntax-ns#> .
-@prefix rml: <http://w3id.org/rml/> .
-@prefix ex: <http://example/> .
+@prefix foaf: <http://xmlns.com/foaf/0.1/> .
+@prefix ex: <http://example.com/> .
 @prefix xsd: <http://www.w3.org/2001/XMLSchema#> .
-@prefix : <http://example.org/> .
-@base <http://example.org/> .
+@prefix rml: <http://w3id.org/rml/> .
+@prefix activity: <http://example.com/activity/> .
+@prefix rdfs: <http://www.w3.org/2000/01/rdf-schema#> .
+@base <http://example.com/base/> .
+
+<TriplesMap1>
+  a rml:TriplesMap;
+
+  rml:logicalSource [
+    rml:source "test/rml-core/json/RMLTC0009a/student.json";
+    rml:referenceFormulation rml:JSONPath;
+    rml:iterator "$.students[*]"
+  ];
+
+  rml:subjectMap [ rml:template "http://example.com/resource/student_{ID}" ];
+
+  rml:predicateObjectMap [
+    rml:predicate foaf:name ;
+    rml:objectMap [ rml:reference "Name" ]
+  ] ;
+
+  rml:predicateObjectMap [
+    rml:predicate <http://example.com/ontology/practises> ;
+    rml:objectMap [
+      a rml:RefObjectMap ;
+      rml:parentTriplesMap <TriplesMap2>;
+      rml:joinCondition [
+        rml:child "Sport" ;
+        rml:parent "ID" ;
+      ]
+    ]
+  ] .
+
+<TriplesMap2>
+  a rml:TriplesMap;
+
+  rml:logicalSource [
+    rml:source "test/rml-core/json/RMLTC0009a/sport.json";
+    rml:referenceFormulation rml:JSONPath;
+    rml:iterator "$.sports[*]"
+  ];
+
+  rml:subjectMap [ rml:template "http://example.com/resource/sport_{ID}" ];
 
-:firstTM a rml:NonAssertedTriplesMap ;
-    rml:logicalSource [
-        rml:source "test/rml-star/RMLSTARTC007b/data1.csv";
-        rml:referenceFormulation rml:CSV
-    ];
-    rml:subjectMap [
-        rml:template "http://example/{c1-1}"
-    ];
-    rml:predicateObjectMap [
-        rml:predicate ex:p1 ;
-        rml:objectMap [
-            rml:template "http://example/{c1-2}"
-        ]
-    ] .
-
-:secondTM a rml:AssertedTriplesMap ;
-    rml:logicalSource [
-        rml:source "test/rml-star/RMLSTARTC007b/data2.csv";
-        rml:referenceFormulation rml:CSV
-    ];
-    rml:subjectMap [
-            rml:quotedTriplesMap :firstTM ;
-            rml:joinCondition [
-              rml:child "c2-3" ;
-              rml:parent "c1-3" ;
-            ];
-    ];
-    rml:predicateObjectMap [
-        rml:predicate ex:q; ;
-        rml:objectMap [
-            rml:quotedTriplesMap :thirdTM
-        ]
-    ] .
-
-:thirdTM a rml:NonAssertedTriplesMap ;
-    rml:logicalSource [
-        rml:source "test/rml-star/RMLSTARTC007b/data2.csv";
-        rml:referenceFormulation rml:CSV
-    ];
-    rml:subjectMap [
-        rml:template "http://example/{c2-1}"
-    ];
-    rml:predicateObjectMap [
-        rml:predicate ex:p2 ;
-        rml:objectMap [
-            rml:template "http://example/{c2-2}"
-        ]
-    ] .
+  rml:predicateObjectMap [
+    rml:predicate rdfs:label ;
+    rml:objectMap [ rml:reference "Name" ];
+  ].
```

### Comparing `morph_kgc-2.6.4/test/rml-star/RMLSTARTC007b/test_RMLSTARTC007b_CSV.py` & `morph_kgc-2.7.0/test/rml-star/RMLSTARTC007b/test_RMLSTARTC007b_CSV.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/rml-star/RMLSTARTC008a/mapping.ttl` & `morph_kgc-2.7.0/test/rml-star/RMLSTARTC008a/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/rml-star/RMLSTARTC008a/test_RMLSTARTC008a_CSV.py` & `morph_kgc-2.7.0/test/rml-star/RMLSTARTC008a/test_RMLSTARTC008a_CSV.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/rml-star/RMLSTARTC008b/mapping.ttl` & `morph_kgc-2.7.0/test/rml-star/RMLSTARTC008b/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/rml-star/RMLSTARTC008b/test_RMLSTARTC008b_CSV.py` & `morph_kgc-2.7.0/test/rml-star/RMLSTARTC008b/test_RMLSTARTC008b_CSV.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/rmltv/RMLTVTC0002d/mapping.ttl` & `morph_kgc-2.7.0/test/rml-core/xml/RMLTC0007e/mapping.ttl`

 * *Files 25% similar despite different names*

```diff
@@ -1,23 +1,30 @@
-@prefix rr: <http://www.w3.org/ns/r2rml#> .
 @prefix foaf: <http://xmlns.com/foaf/0.1/> .
-@prefix rml: <http://semweb.mmlab.be/ns/rml#> .
-@prefix ql: <http://semweb.mmlab.be/ns/ql#> .
+@prefix ex: <http://example.com/> .
+@prefix xsd: <http://www.w3.org/2001/XMLSchema#> .
+@prefix rml: <http://w3id.org/rml/> .
+@base <http://example.com/base/> .
 
-<TriplesMap1> a rr:TriplesMap;
+<TriplesMap1> a rml:TriplesMap;
 
   rml:logicalSource [
-    rr:sqlVersion rr:SQL2008;
-    rml:query """
-        SELECT CONCAT('Student', ID) AS StudentId, ID, Name FROM 'test/rmltv/RMLTVTC0002d/student.csv'
-    """;
-    rml:referenceFormulation ql:CSV
+    rml:source "test/rml-core/xml/RMLTC0007e/student.xml";
+    rml:referenceFormulation rml:XPath;
+    rml:iterator "/students/student"
   ];
 
-  rr:subjectMap [
-      rml:reference "StudentId"; rr:termType rr:BlankNode
-    ];
+  rml:subjectMap [
+    rml:template "http://example.com/Student/{ID}/{Name}";
+    rml:graph ex:PersonGraph ;
+    rml:class foaf:Person
+  ];
+
+  rml:predicateObjectMap [
+    rml:predicate ex:id ;
+    rml:objectMap [ rml:reference "ID"; ]
+  ];
 
-    rr:predicateObjectMap [
-      rr:predicate foaf:name ;
-      rr:objectMap [ rml:reference "Name" ]
+  rml:predicateObjectMap
+    [
+      rml:predicate		foaf:name ;
+      rml:objectMap		[ rml:reference "Name" ]
     ].
```

### Comparing `morph_kgc-2.6.4/test/rmltv/RMLTVTC0002d/test_RMLTVTC0002d_CSV.py` & `morph_kgc-2.7.0/test/rml-tv/RMLTVTC0002d/test_RMLTVTC0002d_CSV.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/rmltv/RMLTVTC0002g/mapping.ttl` & `morph_kgc-2.7.0/test/rml-tv/RMLTVTC0003b/mapping.ttl`

 * *Files 24% similar despite different names*

```diff
@@ -1,21 +1,22 @@
-@prefix rr: <http://www.w3.org/ns/r2rml#> .
-@prefix ex: <http://example.com/> .
-@prefix rml: <http://semweb.mmlab.be/ns/rml#> .
-@prefix ql: <http://semweb.mmlab.be/ns/ql#> .
+@prefix foaf: <http://xmlns.com/foaf/0.1/> .
+@prefix rml: <http://w3id.org/rml/> .
 
-<TriplesMap1> a rr:TriplesMap;
+<TriplesMap1>
+     a rml:TriplesMap;
 
-  rml:logicalSource [
-    rr:sqlVersion rr:SQL2008;
-    rml:query "SELECT kjnqsdjfbqsdjfmsdnfm FROM 'test/rmltv/RMLTVTC0002g/student.csv'";
-    rml:referenceFormulation ql:CSV
-  ];
+     rml:logicalSource [
+                     rml:query """
+                     SELECT "ID",
+                            ("FirstName" || ' ' || "LastName") AS "Name"
+                     FROM 'test/rml-tv/RMLTVTC0003b/student.csv'
+                     """
+                     ];
 
-  rr:subjectMap [
-      rr:template "http://example.com/{ID}/{Name}";
-    ];
+    rml:subjectMap [ rml:template "http://example.com/Student/{ID}"; ];
 
-    rr:predicateObjectMap [
-      rr:predicate ex:id ;
-      rr:objectMap [ rml:reference "IDs" ]
-    ].
+    rml:predicateObjectMap
+    [
+      rml:predicate		foaf:name ;
+      rml:objectMap		[ rml:reference "Name" ]
+    ]
+    .
```

### Comparing `morph_kgc-2.6.4/test/rmltv/RMLTVTC0002g/test_RMLTVTC0002g_CSV.py` & `morph_kgc-2.7.0/test/rml-tv/RMLTVTC0002g/test_RMLTVTC0002g_CSV.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/rmltv/RMLTVTC0002h/test_RMLTVTC0002h_CSV.py` & `morph_kgc-2.7.0/test/rml-tv/RMLTVTC0002h/test_RMLTVTC0002h_CSV.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/rmltv/RMLTVTC0002i/test_RMLTVTC0002i_CSV.py` & `morph_kgc-2.7.0/test/rml-tv/RMLTVTC0002i/test_RMLTVTC0002i_CSV.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/rmltv/RMLTVTC0002j/test_RMLTVTC0002j_CSV.py` & `morph_kgc-2.7.0/test/rml-tv/RMLTVTC0002j/test_RMLTVTC0002j_CSV.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/rmltv/RMLTVTC0003b/test_RMLTVTC0003b_CSV.py` & `morph_kgc-2.7.0/test/rml-tv/RMLTVTC0003b/test_RMLTVTC0003b_CSV.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/rmltv/RMLTVTC0009c/mapping.ttl` & `morph_kgc-2.7.0/test/rml-tv/RMLTVTC0002j/mapping.ttl`

 * *Files 22% similar despite different names*

```diff
@@ -1,21 +1,19 @@
-@prefix rr: <http://www.w3.org/ns/r2rml#> .
 @prefix foaf: <http://xmlns.com/foaf/0.1/> .
-@prefix rml: <http://semweb.mmlab.be/ns/rml#> .
+@prefix rml: <http://w3id.org/rml/> .
 
-<TriplesMap1>
-   a rr:TriplesMap;
+<TriplesMap1> a rml:TriplesMap;
+    rml:logicalSource [
+                     rml:query """
+                       SELECT "Student"."ID", "Student"."Name"
+                       FROM 'test/rml-tv/RMLTVTC0002j/student.csv' AS "Student"
+                       """
+                       ];
 
-   rml:logicalSource [ rml:query """
-        SELECT "Name", COUNT("Sport")
-        FROM 'test/rmltv/RMLTVTC0009c/student.csv'
-        GROUP BY "Name"
-        """ ];
+    rml:subjectMap [ rml:template "http://example.com/{ID}/{Name}"; ];
 
-    rr:subjectMap [ rr:template "http://example.com/resource/student_{Name}"; ];
-
-    rr:predicateObjectMap
+    rml:predicateObjectMap
     [
-      rr:predicate	foaf:name ;
-      rr:objectMap	[ rml:reference "Name"; ];
-    ];
-  .
+      rml:predicate		foaf:name ;
+      rml:objectMap		[ rml:reference "Name" ]
+	]
+    .
```

### Comparing `morph_kgc-2.6.4/test/rmltv/RMLTVTC0009c/test_RMLTVTC0009c_CSV.py` & `morph_kgc-2.7.0/test/rml-tv/RMLTVTC0009c/test_RMLTVTC0009c_CSV.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/rmltv/RMLTVTC0009d/mapping.ttl` & `morph_kgc-2.7.0/test/rml-core/xml/RMLTC0008a/mapping.ttl`

 * *Files 18% similar despite different names*

```diff
@@ -1,28 +1,40 @@
-@prefix rr: <http://www.w3.org/ns/r2rml#> .
 @prefix foaf: <http://xmlns.com/foaf/0.1/> .
 @prefix ex: <http://example.com/> .
-@prefix rml: <http://semweb.mmlab.be/ns/rml#> .
+@prefix xsd: <http://www.w3.org/2001/XMLSchema#> .
+@prefix rml: <http://w3id.org/rml/> .
+@prefix rdf: <http://www.w3.org/1999/02/22-rdf-syntax-ns#> .
+@base <http://example.com/base/> .
 
 <TriplesMap1>
-   a rr:TriplesMap;
+  a rml:TriplesMap;
 
-   rml:logicalSource [ rml:query """
-        SELECT "Name", COUNT("Sport") as SPORTCOUNT
-        FROM 'test/rmltv/RMLTVTC0009d/student.csv'
-        GROUP BY "Name"
-        """ ];
-
-    rr:subjectMap [ rr:template "http://example.com/resource/student_{Name}"; ];
-
-    rr:predicateObjectMap
-    [
-      rr:predicate	foaf:name ;
-      rr:objectMap	[ rml:reference "Name"; ];
-    ];
-
-   rr:predicateObjectMap
-    [
-		rr:predicate	ex:numSport ;
-		rr:objectMap	[ rml:reference "SPORTCOUNT"; ];
-    ];
-  .
+  rml:logicalSource [
+    rml:source "test/rml-core/xml/RMLTC0008a/student.xml";
+    rml:referenceFormulation rml:XPath;
+    rml:iterator "/students/student"
+  ];
+
+  rml:subjectMap [
+    rml:template "http://example.com/Student/{ID}/{Name}";
+    rml:graphMap [ rml:template "http://example.com/graph/Student/{ID}/{Name}" ]
+  ];
+
+  rml:predicateObjectMap [
+    rml:predicate rdf:type ;
+    rml:object foaf:Person;
+  ];
+
+  rml:predicateObjectMap [
+    rml:predicate ex:id ;
+    rml:objectMap [ rml:reference "ID" ]
+  ];
+
+  rml:predicateObjectMap [
+    rml:predicate foaf:name ;
+    rml:objectMap [ rml:reference "Name" ]
+  ];
+
+  rml:predicateObjectMap [
+    rml:predicate ex:Sport ;
+    rml:objectMap [ rml:reference "Sport" ]
+  ] .
```

### Comparing `morph_kgc-2.6.4/test/rmltv/RMLTVTC0009d/test_RMLTVTC0009d_CSV.py` & `morph_kgc-2.7.0/test/rml-tv/RMLTVTC0009d/test_RMLTVTC0009d_CSV.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/rmltv/RMLTVTC0011a/output.nq` & `morph_kgc-2.7.0/test/rml-tv/RMLTVTC0011a/output.nq`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/rmltv/RMLTVTC0011a/test_RMLTVTC0011a_CSV.py` & `morph_kgc-2.7.0/test/rml-tv/RMLTVTC0011a/test_RMLTVTC0011a_CSV.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/rmltv/RMLTVTC0014d/mapping.ttl` & `morph_kgc-2.7.0/test/rml-tv/RMLTVTC0014d/mapping.ttl`

 * *Files 18% similar despite different names*

```diff
@@ -1,22 +1,21 @@
-@prefix rr: <http://www.w3.org/ns/r2rml#> .
 @prefix ex: <http://example.com/ns#> .
-@prefix rml: <http://semweb.mmlab.be/ns/rml#> .
+@prefix rml: <http://w3id.org/rml/> .
 
 <TriplesMap4>
-	a rr:TriplesMap;
+	a rml:TriplesMap;
     rml:logicalSource [ rml:query """
 
         SELECT "EMP".*, (CASE "job"
             WHEN 'CLERK' THEN 'general-office'
             WHEN 'NIGHTGUARD' THEN 'security'
             WHEN 'ENGINEER' THEN 'engineering'
-        END) AS "ROLE" FROM 'test/rmltv/RMLTVTC0014d/emp.csv' AS "EMP"
+        END) AS "ROLE" FROM 'test/rml-tv/RMLTVTC0014d/emp.csv' AS "EMP"
 
         """ ];
-    rr:subjectMap [
-        rr:template "http://data.example.com/employee/{empno}";
+    rml:subjectMap [
+        rml:template "http://data.example.com/employee/{empno}";
     ];
-    rr:predicateObjectMap [
-        rr:predicate ex:role;
-        rr:objectMap [ rr:template "http://data.example.com/roles/{ROLE}" ];
+    rml:predicateObjectMap [
+        rml:predicate ex:role;
+        rml:objectMap [ rml:template "http://data.example.com/roles/{ROLE}" ];
     ].
```

### Comparing `morph_kgc-2.6.4/test/rmltv/RMLTVTC0014d/test_RMLTVTC0014d_CSV.py` & `morph_kgc-2.7.0/test/rml-tv/RMLTVTC0014d/test_RMLTVTC0014d_CSV.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/rmltv/RMLTVTC0015a/mapping.ttl` & `morph_kgc-2.7.0/test/rml-tv/RMLTVTC0015b/mapping.ttl`

 * *Files 17% similar despite different names*

```diff
@@ -1,40 +1,39 @@
-@prefix rr: <http://www.w3.org/ns/r2rml#> .
 @prefix rdfs: <http://www.w3.org/2000/01/rdf-schema#> .
-@prefix rml: <http://semweb.mmlab.be/ns/rml#> .
+@prefix rml: <http://w3id.org/rml/> .
 
 
 <TriplesMap1>
-    a rr:TriplesMap;
+    a rml:TriplesMap;
 
 	rml:logicalSource [  rml:query """
-						SELECT "Code", "Name", "Lan"
-						FROM 'test/rmltv/RMLTVTC0015a/country.csv'
-						WHERE "Lan" = 'EN';
+                       SELECT "Code", "Name", "Lan"
+                       FROM 'test/rml-tv/RMLTVTC0015b/country.csv'
+					   WHERE "Lan" = 'EN';
                        """ ] ;
 
-    rr:subjectMap [ rr:template "http://example.com/{Code}" ];
+    rml:subjectMap [ rml:template "http://example.com/{Code}" ];
 
-    rr:predicateObjectMap
+    rml:predicateObjectMap
     [
-      rr:predicate	rdfs:label;
-      rr:objectMap	[ rr:column "Name"; rr:language "en" ]
+      rml:predicate		rdfs:label;
+      rml:objectMap		[ rml:reference "Name"; rml:language "english" ]
     ]
     .
 
 <TriplesMap2>
-    a rr:TriplesMap;
+    a rml:TriplesMap;
 
 	rml:logicalSource [  rml:query """
                        SELECT "Code", "Name", "Lan"
-                       FROM 'test/rmltv/RMLTVTC0015a/country.csv'
+                       FROM 'test/rml-tv/RMLTVTC0015b/country.csv'
 					   WHERE "Lan" = 'ES';
                        """ ] ;
 
-    rr:subjectMap [ rr:template "http://example.com/{Code}" ];
+    rml:subjectMap [ rml:template "http://example.com/{Code}" ];
 
-    rr:predicateObjectMap
+    rml:predicateObjectMap
     [
-      rr:predicate rdfs:label;
-      rr:objectMap    [ rr:column "Name"; rr:language "es" ]
+      rml:predicate		rdfs:label;
+      rml:objectMap		[ rml:reference "Name"; rml:language "spanish" ]
     ]
     .
```

### Comparing `morph_kgc-2.6.4/test/rmltv/RMLTVTC0015a/test_RMLTVTC0015a_CSV.py` & `morph_kgc-2.7.0/test/rml-tv/RMLTVTC0015a/test_RMLTVTC0015a_CSV.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/rmltv/RMLTVTC0015b/mapping.ttl` & `morph_kgc-2.7.0/test/rml-tv/RMLTVTC0027a/mapping.ttl`

 * *Files 27% similar despite different names*

```diff
@@ -1,40 +1,23 @@
-@prefix rr: <http://www.w3.org/ns/r2rml#> .
-@prefix rdfs: <http://www.w3.org/2000/01/rdf-schema#> .
-@prefix rml: <http://semweb.mmlab.be/ns/rml#> .
-
+@prefix ex: <http://example.com/> .
+@prefix rml: <http://w3id.org/rml/> .
 
 <TriplesMap1>
-    a rr:TriplesMap;
-
-	rml:logicalSource [  rml:query """
-                       SELECT "Code", "Name", "Lan"
-                       FROM 'test/rmltv/RMLTVTC0015b/country.csv'
-					   WHERE "Lan" = 'EN';
-                       """ ] ;
-
-    rr:subjectMap [ rr:template "http://example.com/{Code}" ];
-
-    rr:predicateObjectMap
-    [
-      rr:predicate		rdfs:label;
-      rr:objectMap		[ rml:reference "Name"; rr:language "english" ]
-    ]
-    .
-
-<TriplesMap2>
-    a rr:TriplesMap;
-
-	rml:logicalSource [  rml:query """
-                       SELECT "Code", "Name", "Lan"
-                       FROM 'test/rmltv/RMLTVTC0015b/country.csv'
-					   WHERE "Lan" = 'ES';
-                       """ ] ;
-
-    rr:subjectMap [ rr:template "http://example.com/{Code}" ];
+    a rml:TriplesMap;
+ 	rml:logicalSource [
+                     rml:query """
+                       SELECT ID, json_extract_string(COL, '$.field1') AS FIELD1, UNNEST(json_extract_string(COL, '$.field2')::VARCHAR[])[2:-2] AS FIELD2
+                       FROM 'test/rml-tv/RMLTVTC0027a/mixed_content_json.csv'
+                       """
+                       ];
 
-    rr:predicateObjectMap
+	rml:subjectMap [ rml:template "http://example.com/{ID}" ];
+	rml:predicateObjectMap
     [
-      rr:predicate		rdfs:label;
-      rr:objectMap		[ rml:reference "Name"; rr:language "spanish" ]
-    ]
-    .
+      rml:predicate		ex:field1;
+      rml:objectMap		[ rml:reference "FIELD1" ];
+    ];
+    rml:predicateObjectMap [
+      rml:predicate		ex:field2;
+      rml:objectMap		[ rml:reference "FIELD2" ];
+    ];
+.
```

### Comparing `morph_kgc-2.6.4/test/rmltv/RMLTVTC0015b/test_RMLTVTC0015b_CSV.py` & `morph_kgc-2.7.0/test/rml-tv/RMLTVTC0015b/test_RMLTVTC0015b_CSV.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/rmltv/RMLTVTC0019a/mapping.ttl` & `morph_kgc-2.7.0/test/rml-tv/RMLTVTC0019a/mapping.ttl`

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,20 @@
-@prefix rr: <http://www.w3.org/ns/r2rml#> .
 @prefix foaf: <http://xmlns.com/foaf/0.1/> .
-@prefix rml: <http://semweb.mmlab.be/ns/rml#> .
+@prefix rml: <http://w3id.org/rml/> .
 
 <TriplesMap1>
-    a rr:TriplesMap;
+    a rml:TriplesMap;
  	rml:logicalSource [
                      rml:query """
                        SELECT "ID", "FirstName", "LastName"
-                       FROM 'test/rmltv/RMLTVTC0019a/employee.csv'
+                       FROM 'test/rml-tv/RMLTVTC0019a/employee.csv'
                        WHERE "ID" < 20
                        """
                        ];
 
-	rr:subjectMap [ rml:reference "FirstName" ];
-	rr:predicateObjectMap
+	rml:subjectMap [ rml:reference "FirstName" ];
+	rml:predicateObjectMap
     [
-      rr:predicate		foaf:name;
-      rr:objectMap		[ rml:reference "FirstName" ];
+      rml:predicate		foaf:name;
+      rml:objectMap		[ rml:reference "FirstName" ];
     ];
 .
```

### Comparing `morph_kgc-2.6.4/test/rmltv/RMLTVTC0019a/test_RMLTVTC0019a_CSV.py` & `morph_kgc-2.7.0/test/rml-tv/RMLTVTC0019a/test_RMLTVTC0019a_CSV.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/rmltv/RMLTVTC0026a/mapping.ttl` & `morph_kgc-2.7.0/test/rml-core/csv/RMLTC0007f/mapping.ttl`

 * *Files 23% similar despite different names*

```diff
@@ -1,20 +1,33 @@
-@prefix rr: <http://www.w3.org/ns/r2rml#> .
+@prefix foaf: <http://xmlns.com/foaf/0.1/> .
 @prefix ex: <http://example.com/> .
-@prefix rml: <http://semweb.mmlab.be/ns/rml#> .
+@prefix xsd: <http://www.w3.org/2001/XMLSchema#> .
+@prefix rml: <http://w3id.org/rml/> .
+@prefix rdf: <http://www.w3.org/1999/02/22-rdf-syntax-ns#> .
+@base <http://example.com/base/> .
 
-<TriplesMap1>
-    a rr:TriplesMap;
- 	rml:logicalSource [
-                     rml:query """
-                       SELECT ID, UNNEST(COL::VARCHAR[]) AS COL
-                       FROM 'test/rmltv/RMLTVTC0026a/mixed_content_list.csv'
-                       """
-                       ];
-
-	rr:subjectMap [ rr:template "http://example.com/{ID}" ];
-	rr:predicateObjectMap
-    [
-      rr:predicate		ex:col;
-      rr:objectMap		[ rml:reference "COL" ];
-    ];
-.
+<TriplesMap1> a rml:TriplesMap;
+
+  rml:logicalSource [
+    rml:source "test/rml-core/csv/RMLTC0007f/student.csv";
+    rml:referenceFormulation rml:CSV
+  ];
+
+  rml:subjectMap [
+    rml:template "http://example.com/Student/{ID}/{FirstName}";
+    rml:graph ex:PersonGraph
+  ];
+
+  rml:predicateObjectMap [
+    rml:predicate rdf:type;
+    rml:object foaf:Person
+  ];
+
+  rml:predicateObjectMap [
+    rml:predicate ex:id ;
+    rml:objectMap [ rml:reference "ID";  ]
+  ];
+
+  rml:predicateObjectMap [
+    rml:predicate foaf:name ;
+    rml:objectMap [ rml:reference "FirstName" ]
+  ].
```

### Comparing `morph_kgc-2.6.4/test/rmltv/RMLTVTC0026a/test_RMLTVTC0026a_CSV.py` & `morph_kgc-2.7.0/test/rml-tv/RMLTVTC0026a/test_RMLTVTC0026a_CSV.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/rmltv/RMLTVTC0027a/test_RMLTVTC0027a_CSV.py` & `morph_kgc-2.7.0/test/rml-tv/RMLTVTC0027a/test_RMLTVTC0027a_CSV.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/rmltv/RMLTVTC0028a/test_RMLTVTC0028a_CSV.py` & `morph_kgc-2.7.0/test/rml-tv/RMLTVTC0028a/test_RMLTVTC0028a_CSV.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/test/rmltv/RMLTVTC0029a/test_RMLTVTC0029a_CSV.py` & `morph_kgc-2.7.0/test/rml-tv/RMLTVTC0029a/test_RMLTVTC0029a_CSV.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/LICENSE` & `morph_kgc-2.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.6.4/README.md` & `morph_kgc-2.7.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 <p align="center">
-<img src="https://github.com/morph-kgc/morph-kgc/blob/main/docs/assets/logo.png" height="100" alt="morph">
+<img src="https://github.com/morph-kgc/morph-kgc/blob/main/logo/logo.png" height="100" alt="morph">
 </p>
 
 [![License](https://img.shields.io/pypi/l/morph-kgc.svg)](https://github.com/morph-kgc/morph-kgc/blob/main/LICENSE)
 [![DOI](https://zenodo.org/badge/311956260.svg?style=flat)](https://zenodo.org/badge/latestdoi/311956260)
 [![Latest PyPI version](https://img.shields.io/pypi/v/morph-kgc?style=flat)](https://pypi.python.org/pypi/morph-kgc)
 [![Python Version](https://img.shields.io/pypi/pyversions/morph-kgc.svg)](https://pypi.python.org/pypi/morph-kgc)
 [![PyPI status](https://img.shields.io:/pypi/status/morph-kgc?)](https://pypi.python.org/pypi/morph-kgc)
@@ -15,16 +15,16 @@
 
 ## Features :sparkles:
 
 - Supports the **[R2RML](https://www.w3.org/TR/r2rml/)** and **[RML](https://w3id.org/rml/core/spec)** mapping languages.
 - User-friendly mappings with **[YARRRML](https://rml.io/yarrrml/spec/)**.
 - Transformation functions with **[RML-FNML](https://w3id.org/rml/fnml/spec)**, including **Python user-defined functions**.
 - [RDF-star](https://w3c.github.io/rdf-star/cg-spec/2021-12-17.html) generation with **[RML-star](https://w3id.org/rml/star/spec)**.
-- **[RML views](https://oa.upm.es/73463/1/_2023___ESWC__RML_Tabular_Views.pdf)** over tabular data sources and **[JSON](https://www.json.org)** files.
-- Integration with **[RDFLib](https://rdflib.readthedocs.io)** and **[Oxigraph](https://pyoxigraph.readthedocs.io/en/latest/)**.
+- **[RML views](https://oa.upm.es/73463/1/_2023___ESWC__RML_Tabular_Views.pdf)** over tabular data sources and [JSON](https://www.json.org) files.
+- Integration with **[RDFLib](https://rdflib.readthedocs.io)**, **[Oxigraph](https://pyoxigraph.readthedocs.io/en/latest/)** and **[Kafka](https://kafka-python.readthedocs.io)**.
 - **Optimized** to materialize large knowledge graphs.
 - **Remote** data and mapping files.
 - Input data formats:
     - **Relational databases**: **[MySQL](https://www.mysql.com/)**, **[PostgreSQL](https://www.postgresql.org/)**, **[Oracle](https://www.oracle.com/database/)**, **[Microsoft SQL Server](https://www.microsoft.com/sql-server)**, **[MariaDB](https://mariadb.org/)**, **[SQLite](https://www.sqlite.org)**.
     - **Tabular files**: **[CSV](https://en.wikipedia.org/wiki/Comma-separated_values)**, **[TSV](https://en.wikipedia.org/wiki/Tab-separated_values)**, **[Excel](https://www.microsoft.com/en-us/microsoft-365/excel)**, **[Parquet](https://parquet.apache.org/documentation/latest/)**, **[Feather](https://arrow.apache.org/docs/python/feather.html)**, **[ORC](https://orc.apache.org/)**, **[Stata](https://www.stata.com/)**, **[SAS](https://www.sas.com)**, **[SPSS](https://www.ibm.com/analytics/spss-statistics-software)**, **[ODS](https://en.wikipedia.org/wiki/OpenDocument)**.
     - **Hierarchical files**: **[JSON](https://www.json.org)**, **[XML](https://www.w3.org/TR/xml/)**.
     - **In-memory data structures**: **[Python Dictionaries](https://docs.python.org/3/tutorial/datastructures.html#dictionaries)**, **[DataFrames](https://pandas.pydata.org/docs/reference/api/pandas.DataFrame.html)**.
@@ -50,15 +50,15 @@
 To run the engine via **command line** you just need to execute the following:
 ```bash
 python3 -m morph_kgc config.ini
 ```
 
 Check the **[documentation](https://morph-kgc.readthedocs.io/en/latest/documentation/#configuration)** to see how to generate the configuration **INI file**. **[Here](https://github.com/morph-kgc/morph-kgc/blob/main/examples/configuration-file/default_config.ini)** you can also see an example INI file.
 
-It is also possible to run Morph-KGC as a **library** with **[RDFLib](https://rdflib.readthedocs.io)** and **[Oxigraph](https://pyoxigraph.readthedocs.io/en/latest/)**:
+It is also possible to run Morph-KGC as a **library** with **[RDFLib](https://rdflib.readthedocs.io)**, **[Oxigraph](https://pyoxigraph.readthedocs.io/en/latest/)** and **[Kafka](https://kafka-python.readthedocs.io)**:
 ```python
 import morph_kgc
 
 # generate the triples and load them to an RDFLib graph
 g_rdflib = morph_kgc.materialize('/path/to/config.ini')
 # work with the RDFLib graph
 q_res = g_rdflib.query('SELECT DISTINCT ?classes WHERE { ?s a ?classes }')
@@ -85,28 +85,29 @@
 
 - **[Julián Arenas-Guerrero](https://github.com/arenas-guerrero-julian/) - [julian.arenas.guerrero@upm.es](mailto:julian.arenas.guerrero@upm.es)**
 
 *[Ontology Engineering Group](https://oeg.fi.upm.es)*, *[Universidad Politécnica de Madrid](https://www.upm.es/internacional)*.
 
 ## Citing :speech_balloon:
 
-If you used Morph-KGC in your work, please cite the **[SWJ paper](https://content.iospress.com/download/semantic-web/sw223135?id=semantic-web%2Fsw223135)**:
+If you used Morph-KGC in your work, please cite the **[SWJ paper](https://www.doi.org/10.3233/SW-223135)**:
 
 ```bib
-@article{arenas2022morph,
-  title   = {{Morph-KGC: Scalable knowledge graph materialization with mapping partitions}},
-  author  = {Arenas-Guerrero, Julián and Chaves-Fraga, David and Toledo, Jhon and Pérez, María S. and Corcho, Oscar},
-  journal = {Semantic Web},
-  year    = {2022},
-  doi     = {10.3233/SW-223135}
+@article{arenas2024morph,
+  title     = {{Morph-KGC: Scalable knowledge graph materialization with mapping partitions}},
+  author    = {Arenas-Guerrero, Julián and Chaves-Fraga, David and Toledo, Jhon and Pérez, María S. and Corcho, Oscar},
+  journal   = {Semantic Web},
+  publisher = {IOS Press},
+  issn      = {2210-4968},
+  year      = {2024},
+  doi       = {10.3233/SW-223135},
+  volume    = {15},
+  number    = {1},
+  pages     = {1-20}
 }
 ```
 
-## Contributors :woman_technologist:
-
-See the full list of contributors **[here](https://github.com/morph-kgc/morph-kgc/graphs/contributors)**.
-
 ## Sponsor :shield:
 
 <p align="center">
-<img src="https://github.com/morph-kgc/morph-kgc/blob/main/docs/assets/BASF.png" height="100" alt="BASF">
+<img src="https://github.com/morph-kgc/morph-kgc-docs/blob/main/docs/assets/BASF.png" height="100" alt="BASF">
 </p>
```

### Comparing `morph_kgc-2.6.4/pyproject.toml` & `morph_kgc-2.7.0/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,74 +1,74 @@
 [build-system]
 requires = ['hatchling>=1.11.0']
 build-backend = 'hatchling.build'
 
 [project.urls]
-Documentation = 'https://morph-kgc.readthedocs.io/en/latest/documentation/'
+Documentation = 'https://morph-kgc.readthedocs.io'
 Source = 'https://github.com/morph-kgc/morph-kgc'
 Tracker = 'https://github.com/morph-kgc/morph-kgc/issues'
 CI = 'https://github.com/morph-kgc/morph-kgc/actions'
-Homepage = 'https://morph-kgc.readthedocs.io/en/latest/'
+Homepage = 'https://morph-kgc.readthedocs.io'
 History = 'https://github.com/morph-kgc/morph-kgc/releases'
 #Sponsor = ''
 
 [project]
 name = 'morph_kgc'
 description = 'Powerful [R2]RML engine to create RDF knowledge graphs from heterogeneous data sources.'
 readme = 'README.md'
 keywords = ['Morph-KGC', 'RDF', 'R2RML', 'RML', 'RML-star', 'Knowledge Graph', 'Data Integration']
 authors = [
   {name = 'Julián Arenas-Guerrero', email = 'julian.arenas.guerrero@upm.es'}
 ]
 license = 'Apache-2.0'
 classifiers = [
   'Programming Language :: Python :: 3',
-  'Programming Language :: Python :: 3.8',
   'Programming Language :: Python :: 3.9',
   'Programming Language :: Python :: 3.10',
   'Programming Language :: Python :: 3.11',
   'License :: OSI Approved :: Apache Software License',
   'Operating System :: OS Independent',
   'Development Status :: 5 - Production/Stable',
   'Environment :: Console',
   'Intended Audience :: Information Technology',
   'Intended Audience :: Science/Research',
   'Topic :: Software Development :: Pre-processors',
   'Topic :: Database',
   'Topic :: Utilities',
   'Topic :: Scientific/Engineering :: Interface Engine/Protocol Translator',
 ]
-requires-python = '>=3.8'
+requires-python = '>=3.9'
 dynamic = ['version']
 dependencies = [
   'pandas>=2.0.0, <3.0.0',
   'rdflib>=6.1.1, <8.0.0',
   'pyoxigraph>=0.3.0, <0.4.0',
   'ruamel.yaml==0.18.0, <0.19.0',
-  'sql-metadata>=2.6.0, <3.0.0',
-  'SQLAlchemy>=2.0.0, <3.0.0',
   'jsonpath-python>=1.0.6, <2.0.0',
   'elementpath>=4.0.0, <5.0.0',
-  'duckdb>=0.7.0, <0.8.0',
+  'duckdb>=0.10.0, <2.0.0',
   'falcon>=3.0.0, <4.0.0'
 ]
 
 [tool.hatch.version]
 path = 'src/morph_kgc/_version.py'
 
 [project.optional-dependencies]
-test = ['pytest>=7.0.0, <8.0.0', 'openpyxl>=3.0.0, <4.0.0', 'odfpy>=1.4.1, <2.0.0', 'pyarrow>=11.0.0, <14.0.0']
-mysql = ['pymysql>=1.0.2, <2.0.0', 'cryptography>=39.0.0, <42.0.0']
-postgresql = ['psycopg[binary]>=3.0.0, <4.0.0']
-oracle = ['cx-Oracle>=8.3.0, <9.0.0']
-mssql = ['pymssql>=2.2.7, <3.0.0']
+test = ['pytest>=8.0.0, <9.0.0', 'SQLAlchemy>=2.0.0, <3.0.0', 'sql-metadata>=2.6.0, <3.0.0', 'openpyxl>=3.0.0, <4.0.0', 'odfpy>=1.4.1, <2.0.0', 'pyarrow>=14.0.0, <16.0.0']
+kafka = ['kafka-python>=2.0.2, <3.0.0']
+sqlite = ['SQLAlchemy>=2.0.0, <3.0.0', 'sql-metadata>=2.6.0, <3.0.0']
+mysql = ['pymysql>=1.1.0, <2.0.0', 'cryptography>=42.0.0, <43.0.0', 'SQLAlchemy>=2.0.0, <3.0.0', 'sql-metadata>=2.6.0, <3.0.0']
+postgresql = ['psycopg[binary]>=3.0.0, <4.0.0', 'SQLAlchemy>=2.0.0, <3.0.0', 'sql-metadata>=2.6.0, <3.0.0']
+oracle = ['cx-Oracle>=8.3.0, <9.0.0', 'SQLAlchemy>=2.0.0, <3.0.0', 'sql-metadata>=2.6.0, <3.0.0']
+mssql = ['pymssql>=2.2.7, <3.0.0', 'SQLAlchemy>=2.0.0, <3.0.0', 'sql-metadata>=2.6.0, <3.0.0']
 excel = ['openpyxl>=3.0.0, <4.0.0', 'odfpy>=1.4.1, <2.0.0']
-tabular = ['pyarrow>=11.0.0, <14.0.0']
+tabular = ['pyarrow>=14.0.0, <16.0.0']
 spss = ['pyreadstat>=1.2.0, <2.0.0']
 all = [
+  'morph_kgc[kafka]',
   'morph_kgc[mysql]',
   'morph_kgc[postgresql]',
   'morph_kgc[oracle]',
   'morph_kgc[mssql]',
   'morph_kgc[excel]',
   'morph_kgc[tabular]',
   'morph_kgc[spss]',
```

### Comparing `morph_kgc-2.6.4/PKG-INFO` & `morph_kgc-2.7.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,80 +1,93 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: morph_kgc
-Version: 2.6.4
+Version: 2.7.0
 Summary: Powerful [R2]RML engine to create RDF knowledge graphs from heterogeneous data sources.
-Project-URL: Documentation, https://morph-kgc.readthedocs.io/en/latest/documentation/
+Project-URL: Documentation, https://morph-kgc.readthedocs.io
 Project-URL: Source, https://github.com/morph-kgc/morph-kgc
 Project-URL: Tracker, https://github.com/morph-kgc/morph-kgc/issues
 Project-URL: CI, https://github.com/morph-kgc/morph-kgc/actions
-Project-URL: Homepage, https://morph-kgc.readthedocs.io/en/latest/
+Project-URL: Homepage, https://morph-kgc.readthedocs.io
 Project-URL: History, https://github.com/morph-kgc/morph-kgc/releases
 Author-email: Julián Arenas-Guerrero <julian.arenas.guerrero@upm.es>
 License-Expression: Apache-2.0
 License-File: LICENSE
 Keywords: Data Integration,Knowledge Graph,Morph-KGC,R2RML,RDF,RML,RML-star
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Database
 Classifier: Topic :: Scientific/Engineering :: Interface Engine/Protocol Translator
 Classifier: Topic :: Software Development :: Pre-processors
 Classifier: Topic :: Utilities
-Requires-Python: >=3.8
-Requires-Dist: duckdb<0.8.0,>=0.7.0
+Requires-Python: >=3.9
+Requires-Dist: duckdb<2.0.0,>=0.10.0
 Requires-Dist: elementpath<5.0.0,>=4.0.0
 Requires-Dist: falcon<4.0.0,>=3.0.0
 Requires-Dist: jsonpath-python<2.0.0,>=1.0.6
 Requires-Dist: pandas<3.0.0,>=2.0.0
 Requires-Dist: pyoxigraph<0.4.0,>=0.3.0
 Requires-Dist: rdflib<8.0.0,>=6.1.1
 Requires-Dist: ruamel-yaml<0.19.0,==0.18.0
-Requires-Dist: sql-metadata<3.0.0,>=2.6.0
-Requires-Dist: sqlalchemy<3.0.0,>=2.0.0
 Provides-Extra: all
 Requires-Dist: morph-kgc[excel]; extra == 'all'
+Requires-Dist: morph-kgc[kafka]; extra == 'all'
 Requires-Dist: morph-kgc[mssql]; extra == 'all'
 Requires-Dist: morph-kgc[mysql]; extra == 'all'
 Requires-Dist: morph-kgc[oracle]; extra == 'all'
 Requires-Dist: morph-kgc[postgresql]; extra == 'all'
 Requires-Dist: morph-kgc[spss]; extra == 'all'
 Requires-Dist: morph-kgc[tabular]; extra == 'all'
 Provides-Extra: excel
 Requires-Dist: odfpy<2.0.0,>=1.4.1; extra == 'excel'
 Requires-Dist: openpyxl<4.0.0,>=3.0.0; extra == 'excel'
+Provides-Extra: kafka
+Requires-Dist: kafka-python<3.0.0,>=2.0.2; extra == 'kafka'
 Provides-Extra: mssql
 Requires-Dist: pymssql<3.0.0,>=2.2.7; extra == 'mssql'
+Requires-Dist: sql-metadata<3.0.0,>=2.6.0; extra == 'mssql'
+Requires-Dist: sqlalchemy<3.0.0,>=2.0.0; extra == 'mssql'
 Provides-Extra: mysql
-Requires-Dist: cryptography<42.0.0,>=39.0.0; extra == 'mysql'
-Requires-Dist: pymysql<2.0.0,>=1.0.2; extra == 'mysql'
+Requires-Dist: cryptography<43.0.0,>=42.0.0; extra == 'mysql'
+Requires-Dist: pymysql<2.0.0,>=1.1.0; extra == 'mysql'
+Requires-Dist: sql-metadata<3.0.0,>=2.6.0; extra == 'mysql'
+Requires-Dist: sqlalchemy<3.0.0,>=2.0.0; extra == 'mysql'
 Provides-Extra: oracle
 Requires-Dist: cx-oracle<9.0.0,>=8.3.0; extra == 'oracle'
+Requires-Dist: sql-metadata<3.0.0,>=2.6.0; extra == 'oracle'
+Requires-Dist: sqlalchemy<3.0.0,>=2.0.0; extra == 'oracle'
 Provides-Extra: postgresql
 Requires-Dist: psycopg[binary]<4.0.0,>=3.0.0; extra == 'postgresql'
+Requires-Dist: sql-metadata<3.0.0,>=2.6.0; extra == 'postgresql'
+Requires-Dist: sqlalchemy<3.0.0,>=2.0.0; extra == 'postgresql'
 Provides-Extra: spss
 Requires-Dist: pyreadstat<2.0.0,>=1.2.0; extra == 'spss'
+Provides-Extra: sqlite
+Requires-Dist: sql-metadata<3.0.0,>=2.6.0; extra == 'sqlite'
+Requires-Dist: sqlalchemy<3.0.0,>=2.0.0; extra == 'sqlite'
 Provides-Extra: tabular
-Requires-Dist: pyarrow<14.0.0,>=11.0.0; extra == 'tabular'
+Requires-Dist: pyarrow<16.0.0,>=14.0.0; extra == 'tabular'
 Provides-Extra: test
 Requires-Dist: odfpy<2.0.0,>=1.4.1; extra == 'test'
 Requires-Dist: openpyxl<4.0.0,>=3.0.0; extra == 'test'
-Requires-Dist: pyarrow<14.0.0,>=11.0.0; extra == 'test'
-Requires-Dist: pytest<8.0.0,>=7.0.0; extra == 'test'
+Requires-Dist: pyarrow<16.0.0,>=14.0.0; extra == 'test'
+Requires-Dist: pytest<9.0.0,>=8.0.0; extra == 'test'
+Requires-Dist: sql-metadata<3.0.0,>=2.6.0; extra == 'test'
+Requires-Dist: sqlalchemy<3.0.0,>=2.0.0; extra == 'test'
 Description-Content-Type: text/markdown
 
 <p align="center">
-<img src="https://github.com/morph-kgc/morph-kgc/blob/main/docs/assets/logo.png" height="100" alt="morph">
+<img src="https://github.com/morph-kgc/morph-kgc/blob/main/logo/logo.png" height="100" alt="morph">
 </p>
 
 [![License](https://img.shields.io/pypi/l/morph-kgc.svg)](https://github.com/morph-kgc/morph-kgc/blob/main/LICENSE)
 [![DOI](https://zenodo.org/badge/311956260.svg?style=flat)](https://zenodo.org/badge/latestdoi/311956260)
 [![Latest PyPI version](https://img.shields.io/pypi/v/morph-kgc?style=flat)](https://pypi.python.org/pypi/morph-kgc)
 [![Python Version](https://img.shields.io/pypi/pyversions/morph-kgc.svg)](https://pypi.python.org/pypi/morph-kgc)
 [![PyPI status](https://img.shields.io:/pypi/status/morph-kgc?)](https://pypi.python.org/pypi/morph-kgc)
@@ -86,16 +99,16 @@
 
 ## Features :sparkles:
 
 - Supports the **[R2RML](https://www.w3.org/TR/r2rml/)** and **[RML](https://w3id.org/rml/core/spec)** mapping languages.
 - User-friendly mappings with **[YARRRML](https://rml.io/yarrrml/spec/)**.
 - Transformation functions with **[RML-FNML](https://w3id.org/rml/fnml/spec)**, including **Python user-defined functions**.
 - [RDF-star](https://w3c.github.io/rdf-star/cg-spec/2021-12-17.html) generation with **[RML-star](https://w3id.org/rml/star/spec)**.
-- **[RML views](https://oa.upm.es/73463/1/_2023___ESWC__RML_Tabular_Views.pdf)** over tabular data sources and **[JSON](https://www.json.org)** files.
-- Integration with **[RDFLib](https://rdflib.readthedocs.io)** and **[Oxigraph](https://pyoxigraph.readthedocs.io/en/latest/)**.
+- **[RML views](https://oa.upm.es/73463/1/_2023___ESWC__RML_Tabular_Views.pdf)** over tabular data sources and [JSON](https://www.json.org) files.
+- Integration with **[RDFLib](https://rdflib.readthedocs.io)**, **[Oxigraph](https://pyoxigraph.readthedocs.io/en/latest/)** and **[Kafka](https://kafka-python.readthedocs.io)**.
 - **Optimized** to materialize large knowledge graphs.
 - **Remote** data and mapping files.
 - Input data formats:
     - **Relational databases**: **[MySQL](https://www.mysql.com/)**, **[PostgreSQL](https://www.postgresql.org/)**, **[Oracle](https://www.oracle.com/database/)**, **[Microsoft SQL Server](https://www.microsoft.com/sql-server)**, **[MariaDB](https://mariadb.org/)**, **[SQLite](https://www.sqlite.org)**.
     - **Tabular files**: **[CSV](https://en.wikipedia.org/wiki/Comma-separated_values)**, **[TSV](https://en.wikipedia.org/wiki/Tab-separated_values)**, **[Excel](https://www.microsoft.com/en-us/microsoft-365/excel)**, **[Parquet](https://parquet.apache.org/documentation/latest/)**, **[Feather](https://arrow.apache.org/docs/python/feather.html)**, **[ORC](https://orc.apache.org/)**, **[Stata](https://www.stata.com/)**, **[SAS](https://www.sas.com)**, **[SPSS](https://www.ibm.com/analytics/spss-statistics-software)**, **[ODS](https://en.wikipedia.org/wiki/OpenDocument)**.
     - **Hierarchical files**: **[JSON](https://www.json.org)**, **[XML](https://www.w3.org/TR/xml/)**.
     - **In-memory data structures**: **[Python Dictionaries](https://docs.python.org/3/tutorial/datastructures.html#dictionaries)**, **[DataFrames](https://pandas.pydata.org/docs/reference/api/pandas.DataFrame.html)**.
@@ -121,15 +134,15 @@
 To run the engine via **command line** you just need to execute the following:
 ```bash
 python3 -m morph_kgc config.ini
 ```
 
 Check the **[documentation](https://morph-kgc.readthedocs.io/en/latest/documentation/#configuration)** to see how to generate the configuration **INI file**. **[Here](https://github.com/morph-kgc/morph-kgc/blob/main/examples/configuration-file/default_config.ini)** you can also see an example INI file.
 
-It is also possible to run Morph-KGC as a **library** with **[RDFLib](https://rdflib.readthedocs.io)** and **[Oxigraph](https://pyoxigraph.readthedocs.io/en/latest/)**:
+It is also possible to run Morph-KGC as a **library** with **[RDFLib](https://rdflib.readthedocs.io)**, **[Oxigraph](https://pyoxigraph.readthedocs.io/en/latest/)** and **[Kafka](https://kafka-python.readthedocs.io)**:
 ```python
 import morph_kgc
 
 # generate the triples and load them to an RDFLib graph
 g_rdflib = morph_kgc.materialize('/path/to/config.ini')
 # work with the RDFLib graph
 q_res = g_rdflib.query('SELECT DISTINCT ?classes WHERE { ?s a ?classes }')
@@ -156,28 +169,29 @@
 
 - **[Julián Arenas-Guerrero](https://github.com/arenas-guerrero-julian/) - [julian.arenas.guerrero@upm.es](mailto:julian.arenas.guerrero@upm.es)**
 
 *[Ontology Engineering Group](https://oeg.fi.upm.es)*, *[Universidad Politécnica de Madrid](https://www.upm.es/internacional)*.
 
 ## Citing :speech_balloon:
 
-If you used Morph-KGC in your work, please cite the **[SWJ paper](https://content.iospress.com/download/semantic-web/sw223135?id=semantic-web%2Fsw223135)**:
+If you used Morph-KGC in your work, please cite the **[SWJ paper](https://www.doi.org/10.3233/SW-223135)**:
 
 ```bib
-@article{arenas2022morph,
-  title   = {{Morph-KGC: Scalable knowledge graph materialization with mapping partitions}},
-  author  = {Arenas-Guerrero, Julián and Chaves-Fraga, David and Toledo, Jhon and Pérez, María S. and Corcho, Oscar},
-  journal = {Semantic Web},
-  year    = {2022},
-  doi     = {10.3233/SW-223135}
+@article{arenas2024morph,
+  title     = {{Morph-KGC: Scalable knowledge graph materialization with mapping partitions}},
+  author    = {Arenas-Guerrero, Julián and Chaves-Fraga, David and Toledo, Jhon and Pérez, María S. and Corcho, Oscar},
+  journal   = {Semantic Web},
+  publisher = {IOS Press},
+  issn      = {2210-4968},
+  year      = {2024},
+  doi       = {10.3233/SW-223135},
+  volume    = {15},
+  number    = {1},
+  pages     = {1-20}
 }
 ```
 
-## Contributors :woman_technologist:
-
-See the full list of contributors **[here](https://github.com/morph-kgc/morph-kgc/graphs/contributors)**.
-
 ## Sponsor :shield:
 
 <p align="center">
-<img src="https://github.com/morph-kgc/morph-kgc/blob/main/docs/assets/BASF.png" height="100" alt="BASF">
+<img src="https://github.com/morph-kgc/morph-kgc-docs/blob/main/docs/assets/BASF.png" height="100" alt="BASF">
 </p>
```

