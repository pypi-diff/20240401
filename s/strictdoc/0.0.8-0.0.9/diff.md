# Comparing `tmp/strictdoc-0.0.8.tar.gz` & `tmp/strictdoc-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "strictdoc-0.0.8.tar", last modified: Sun Jan 24 21:48:28 2021, max compression
+gzip compressed data, was "strictdoc-0.0.9.tar", last modified: Mon Feb  1 09:58:36 2021, max compression
```

## Comparing `strictdoc-0.0.8.tar` & `strictdoc-0.0.9.tar`

### file list

```diff
@@ -1,75 +1,75 @@
--rw-r--r--   0        0        0    11357 2021-01-24 21:48:19.660401 strictdoc-0.0.8/LICENSE
--rw-r--r--   0        0        0      451 2021-01-24 21:48:19.660401 strictdoc-0.0.8/README.md
--rw-r--r--   0        0        0     1256 2021-01-24 21:48:19.664401 strictdoc-0.0.8/pyproject.toml
--rw-r--r--   0        0        0        0 2021-01-24 21:48:19.664401 strictdoc-0.0.8/strictdoc/__init__.py
--rw-r--r--   0        0        0        0 2021-01-24 21:48:19.664401 strictdoc-0.0.8/strictdoc/backend/__init__.py
--rw-r--r--   0        0        0      211 2021-01-24 21:48:19.664401 strictdoc-0.0.8/strictdoc/backend/dsl/document_reference.py
--rw-r--r--   0        0        0     5112 2021-01-24 21:48:19.664401 strictdoc-0.0.8/strictdoc/backend/dsl/error_handling.py
--rw-r--r--   0        0        0     2731 2021-01-24 21:48:19.664401 strictdoc-0.0.8/strictdoc/backend/dsl/grammar.py
--rw-r--r--   0        0        0        0 2021-01-24 21:48:19.664401 strictdoc-0.0.8/strictdoc/backend/dsl/models/__init__.py
--rw-r--r--   0        0        0      589 2021-01-24 21:48:19.664401 strictdoc-0.0.8/strictdoc/backend/dsl/models/config_special_field.py
--rw-r--r--   0        0        0      860 2021-01-24 21:48:19.664401 strictdoc-0.0.8/strictdoc/backend/dsl/models/document.py
--rw-r--r--   0        0        0      741 2021-01-24 21:48:19.664401 strictdoc-0.0.8/strictdoc/backend/dsl/models/document_config.py
--rw-r--r--   0        0        0      357 2021-01-24 21:48:19.664401 strictdoc-0.0.8/strictdoc/backend/dsl/models/reference.py
--rw-r--r--   0        0        0     5341 2021-01-24 21:48:19.664401 strictdoc-0.0.8/strictdoc/backend/dsl/models/requirement.py
--rw-r--r--   0        0        0     1050 2021-01-24 21:48:19.664401 strictdoc-0.0.8/strictdoc/backend/dsl/models/section.py
--rw-r--r--   0        0        0      378 2021-01-24 21:48:19.664401 strictdoc-0.0.8/strictdoc/backend/dsl/models/special_field.py
--rw-r--r--   0        0        0        0 2021-01-24 21:48:19.664401 strictdoc-0.0.8/strictdoc/backend/dsl/models.py
--rw-r--r--   0        0        0    10013 2021-01-24 21:48:19.664401 strictdoc-0.0.8/strictdoc/backend/dsl/reader.py
--rw-r--r--   0        0        0     6450 2021-01-24 21:48:19.664401 strictdoc-0.0.8/strictdoc/backend/dsl/writer.py
--rw-r--r--   0        0        0        0 2021-01-24 21:48:19.664401 strictdoc-0.0.8/strictdoc/cli/__init__.py
--rw-r--r--   0        0        0     2750 2021-01-24 21:48:19.664401 strictdoc-0.0.8/strictdoc/cli/cli_arg_parser.py
--rw-r--r--   0        0        0     1813 2021-01-24 21:48:19.664401 strictdoc-0.0.8/strictdoc/cli/main.py
--rw-r--r--   0        0        0        0 2021-01-24 21:48:19.664401 strictdoc-0.0.8/strictdoc/core/__init__.py
--rw-r--r--   0        0        0     2947 2021-01-24 21:48:19.664401 strictdoc-0.0.8/strictdoc/core/actions/export_action.py
--rw-r--r--   0        0        0      650 2021-01-24 21:48:19.664401 strictdoc-0.0.8/strictdoc/core/actions/passthrough_action.py
--rw-r--r--   0        0        0     7059 2021-01-24 21:48:19.664401 strictdoc-0.0.8/strictdoc/core/document_finder.py
--rw-r--r--   0        0        0     1932 2021-01-24 21:48:19.664401 strictdoc-0.0.8/strictdoc/core/document_iterator.py
--rw-r--r--   0        0        0     2895 2021-01-24 21:48:19.664401 strictdoc-0.0.8/strictdoc/core/document_meta.py
--rw-r--r--   0        0        0     2684 2021-01-24 21:48:19.664401 strictdoc-0.0.8/strictdoc/core/document_tree.py
--rw-r--r--   0        0        0      898 2021-01-24 21:48:19.664401 strictdoc-0.0.8/strictdoc/core/document_tree_iterator.py
--rw-r--r--   0        0        0      550 2021-01-24 21:48:19.664401 strictdoc-0.0.8/strictdoc/core/level_counter.py
--rw-r--r--   0        0        0      950 2021-01-24 21:48:19.664401 strictdoc-0.0.8/strictdoc/core/logger.py
--rw-r--r--   0        0        0    11501 2021-01-24 21:48:19.664401 strictdoc-0.0.8/strictdoc/core/traceability_index.py
--rw-r--r--   0        0        0     6923 2021-01-24 21:48:19.664401 strictdoc-0.0.8/strictdoc/export/excel/excel_generator.py
--rw-r--r--   0        0        0     1871 2021-01-24 21:48:19.664401 strictdoc-0.0.8/strictdoc/export/html/_static/_base.css
--rw-r--r--   0        0        0     1928 2021-01-24 21:48:19.664401 strictdoc-0.0.8/strictdoc/export/html/_static/_content.css
--rw-r--r--   0        0        0     8387 2021-01-24 21:48:19.664401 strictdoc-0.0.8/strictdoc/export/html/_static/_element.css
--rw-r--r--   0        0        0     3714 2021-01-24 21:48:19.664401 strictdoc-0.0.8/strictdoc/export/html/_static/_layout.css
--rw-r--r--   0        0        0     3962 2021-01-24 21:48:19.664401 strictdoc-0.0.8/strictdoc/export/html/_static/_tree.css
--rw-r--r--   0        0        0     5637 2021-01-24 21:48:19.664401 strictdoc-0.0.8/strictdoc/export/html/_static/document_tree.css
--rw-r--r--   0        0        0    92629 2021-01-24 21:48:19.664401 strictdoc-0.0.8/strictdoc/export/html/_static/jquery.min.js
--rw-r--r--   0        0        0     2223 2021-01-24 21:48:19.664401 strictdoc-0.0.8/strictdoc/export/html/_static/pan-with-space.js
--rw-r--r--   0        0        0      906 2021-01-24 21:48:19.664401 strictdoc-0.0.8/strictdoc/export/html/_static/toc.js
--rw-r--r--   0        0        0      583 2021-01-24 21:48:19.664401 strictdoc-0.0.8/strictdoc/export/html/document_type.py
--rw-r--r--   0        0        0      922 2021-01-24 21:48:19.664401 strictdoc-0.0.8/strictdoc/export/html/generators/document.py
--rw-r--r--   0        0        0      912 2021-01-24 21:48:19.664401 strictdoc-0.0.8/strictdoc/export/html/generators/document_deep_trace.py
--rw-r--r--   0        0        0      812 2021-01-24 21:48:19.664401 strictdoc-0.0.8/strictdoc/export/html/generators/document_table.py
--rw-r--r--   0        0        0      876 2021-01-24 21:48:19.664401 strictdoc-0.0.8/strictdoc/export/html/generators/document_trace.py
--rw-r--r--   0        0        0      710 2021-01-24 21:48:19.664401 strictdoc-0.0.8/strictdoc/export/html/generators/document_tree.py
--rw-r--r--   0        0        0     7912 2021-01-24 21:48:19.664401 strictdoc-0.0.8/strictdoc/export/html/html_generator.py
--rw-r--r--   0        0        0     2277 2021-01-24 21:48:19.664401 strictdoc-0.0.8/strictdoc/export/html/renderers/link_renderer.py
--rw-r--r--   0        0        0     1727 2021-01-24 21:48:19.664401 strictdoc-0.0.8/strictdoc/export/html/renderers/markup_renderer.py
--rw-r--r--   0        0        0      771 2021-01-24 21:48:19.664401 strictdoc-0.0.8/strictdoc/export/html/templates/_shared/docsection.jinja.html
--rw-r--r--   0        0        0     3385 2021-01-24 21:48:19.668401 strictdoc-0.0.8/strictdoc/export/html/templates/_shared/requirement.jinja.html
--rw-r--r--   0        0        0      248 2021-01-24 21:48:19.668401 strictdoc-0.0.8/strictdoc/export/html/templates/_shared/tags.jinja.html
--rw-r--r--   0        0        0     1720 2021-01-24 21:48:19.668401 strictdoc-0.0.8/strictdoc/export/html/templates/_shared/toc.jinja.html
--rw-r--r--   0        0        0     2799 2021-01-24 21:48:19.668401 strictdoc-0.0.8/strictdoc/export/html/templates/base.jinja.html
--rw-r--r--   0        0        0     3984 2021-01-24 21:48:19.668401 strictdoc-0.0.8/strictdoc/export/html/templates/document_tree/document_tree.jinja.html
--rw-r--r--   0        0        0     1219 2021-01-24 21:48:19.668401 strictdoc-0.0.8/strictdoc/export/html/templates/single_document/document.jinja.html
--rw-r--r--   0        0        0     1573 2021-01-24 21:48:19.668401 strictdoc-0.0.8/strictdoc/export/html/templates/single_document_table/document.jinja.html
--rw-r--r--   0        0        0     2066 2021-01-24 21:48:19.668401 strictdoc-0.0.8/strictdoc/export/html/templates/single_document_traceability/document.jinja.html
--rw-r--r--   0        0        0     2517 2021-01-24 21:48:19.668401 strictdoc-0.0.8/strictdoc/export/html/templates/single_document_traceability_deep/document.jinja.html
--rw-r--r--   0        0        0      573 2021-01-24 21:48:19.668401 strictdoc-0.0.8/strictdoc/export/html/templates/single_document_traceability_deep/recursive_cell_children.jinja.html
--rw-r--r--   0        0        0      567 2021-01-24 21:48:19.668401 strictdoc-0.0.8/strictdoc/export/html/templates/single_document_traceability_deep/recursive_cell_parent.jinja.html
--rw-r--r--   0        0        0     2893 2021-01-24 21:48:19.668401 strictdoc-0.0.8/strictdoc/export/html/tools/html_embedded.py
--rw-r--r--   0        0        0     1150 2021-01-24 21:48:19.668401 strictdoc-0.0.8/strictdoc/export/rst/document_rst_generator.py
--rw-r--r--   0        0        0      343 2021-01-24 21:48:19.668401 strictdoc-0.0.8/strictdoc/export/rst/rst_to_html_fragment_writer.py
--rw-r--r--   0        0        0     4939 2021-01-24 21:48:19.668401 strictdoc-0.0.8/strictdoc/export/rst/writer.py
--rw-r--r--   0        0        0      175 2021-01-24 21:48:19.668401 strictdoc-0.0.8/strictdoc/helpers/file_modification_time.py
--rw-r--r--   0        0        0      289 2021-01-24 21:48:19.668401 strictdoc-0.0.8/strictdoc/helpers/file_system.py
--rw-r--r--   0        0        0      748 2021-01-24 21:48:19.668401 strictdoc-0.0.8/strictdoc/helpers/parallelizer.py
--rw-r--r--   0        0        0      343 2021-01-24 21:48:19.668401 strictdoc-0.0.8/strictdoc/helpers/sorting.py
--rw-r--r--   0        0        0      691 2021-01-24 21:48:19.668401 strictdoc-0.0.8/strictdoc/helpers/timing.py
--rw-r--r--   0        0        0     2208 2021-01-24 21:48:29.002228 strictdoc-0.0.8/setup.py
--rw-r--r--   0        0        0     1484 2021-01-24 21:48:29.002708 strictdoc-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0    11357 2021-02-01 09:58:23.112496 strictdoc-0.0.9/LICENSE
+-rw-r--r--   0        0        0     1966 2021-02-01 09:58:23.112496 strictdoc-0.0.9/README.md
+-rw-r--r--   0        0        0     1262 2021-02-01 09:58:23.116497 strictdoc-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0        0 2021-02-01 09:58:23.116497 strictdoc-0.0.9/strictdoc/__init__.py
+-rw-r--r--   0        0        0        0 2021-02-01 09:58:23.116497 strictdoc-0.0.9/strictdoc/backend/__init__.py
+-rw-r--r--   0        0        0      211 2021-02-01 09:58:23.116497 strictdoc-0.0.9/strictdoc/backend/dsl/document_reference.py
+-rw-r--r--   0        0        0     5112 2021-02-01 09:58:23.116497 strictdoc-0.0.9/strictdoc/backend/dsl/error_handling.py
+-rw-r--r--   0        0        0     2731 2021-02-01 09:58:23.116497 strictdoc-0.0.9/strictdoc/backend/dsl/grammar.py
+-rw-r--r--   0        0        0        0 2021-02-01 09:58:23.116497 strictdoc-0.0.9/strictdoc/backend/dsl/models/__init__.py
+-rw-r--r--   0        0        0      589 2021-02-01 09:58:23.116497 strictdoc-0.0.9/strictdoc/backend/dsl/models/config_special_field.py
+-rw-r--r--   0        0        0      860 2021-02-01 09:58:23.116497 strictdoc-0.0.9/strictdoc/backend/dsl/models/document.py
+-rw-r--r--   0        0        0      741 2021-02-01 09:58:23.116497 strictdoc-0.0.9/strictdoc/backend/dsl/models/document_config.py
+-rw-r--r--   0        0        0      357 2021-02-01 09:58:23.116497 strictdoc-0.0.9/strictdoc/backend/dsl/models/reference.py
+-rw-r--r--   0        0        0     5341 2021-02-01 09:58:23.116497 strictdoc-0.0.9/strictdoc/backend/dsl/models/requirement.py
+-rw-r--r--   0        0        0     1050 2021-02-01 09:58:23.116497 strictdoc-0.0.9/strictdoc/backend/dsl/models/section.py
+-rw-r--r--   0        0        0      378 2021-02-01 09:58:23.116497 strictdoc-0.0.9/strictdoc/backend/dsl/models/special_field.py
+-rw-r--r--   0        0        0        0 2021-02-01 09:58:23.116497 strictdoc-0.0.9/strictdoc/backend/dsl/models.py
+-rw-r--r--   0        0        0    10013 2021-02-01 09:58:23.116497 strictdoc-0.0.9/strictdoc/backend/dsl/reader.py
+-rw-r--r--   0        0        0     6450 2021-02-01 09:58:23.116497 strictdoc-0.0.9/strictdoc/backend/dsl/writer.py
+-rw-r--r--   0        0        0        0 2021-02-01 09:58:23.116497 strictdoc-0.0.9/strictdoc/cli/__init__.py
+-rw-r--r--   0        0        0     2750 2021-02-01 09:58:23.116497 strictdoc-0.0.9/strictdoc/cli/cli_arg_parser.py
+-rw-r--r--   0        0        0     1813 2021-02-01 09:58:23.116497 strictdoc-0.0.9/strictdoc/cli/main.py
+-rw-r--r--   0        0        0        0 2021-02-01 09:58:23.116497 strictdoc-0.0.9/strictdoc/core/__init__.py
+-rw-r--r--   0        0        0     2947 2021-02-01 09:58:23.116497 strictdoc-0.0.9/strictdoc/core/actions/export_action.py
+-rw-r--r--   0        0        0      650 2021-02-01 09:58:23.116497 strictdoc-0.0.9/strictdoc/core/actions/passthrough_action.py
+-rw-r--r--   0        0        0     7059 2021-02-01 09:58:23.116497 strictdoc-0.0.9/strictdoc/core/document_finder.py
+-rw-r--r--   0        0        0     1932 2021-02-01 09:58:23.116497 strictdoc-0.0.9/strictdoc/core/document_iterator.py
+-rw-r--r--   0        0        0     2895 2021-02-01 09:58:23.116497 strictdoc-0.0.9/strictdoc/core/document_meta.py
+-rw-r--r--   0        0        0     2684 2021-02-01 09:58:23.116497 strictdoc-0.0.9/strictdoc/core/document_tree.py
+-rw-r--r--   0        0        0      898 2021-02-01 09:58:23.116497 strictdoc-0.0.9/strictdoc/core/document_tree_iterator.py
+-rw-r--r--   0        0        0      550 2021-02-01 09:58:23.116497 strictdoc-0.0.9/strictdoc/core/level_counter.py
+-rw-r--r--   0        0        0      950 2021-02-01 09:58:23.116497 strictdoc-0.0.9/strictdoc/core/logger.py
+-rw-r--r--   0        0        0    11501 2021-02-01 09:58:23.116497 strictdoc-0.0.9/strictdoc/core/traceability_index.py
+-rw-r--r--   0        0        0     6923 2021-02-01 09:58:23.116497 strictdoc-0.0.9/strictdoc/export/excel/excel_generator.py
+-rw-r--r--   0        0        0     1871 2021-02-01 09:58:23.116497 strictdoc-0.0.9/strictdoc/export/html/_static/_base.css
+-rw-r--r--   0        0        0     1928 2021-02-01 09:58:23.116497 strictdoc-0.0.9/strictdoc/export/html/_static/_content.css
+-rw-r--r--   0        0        0     8475 2021-02-01 09:58:23.116497 strictdoc-0.0.9/strictdoc/export/html/_static/_element.css
+-rw-r--r--   0        0        0     3714 2021-02-01 09:58:23.116497 strictdoc-0.0.9/strictdoc/export/html/_static/_layout.css
+-rw-r--r--   0        0        0     3962 2021-02-01 09:58:23.116497 strictdoc-0.0.9/strictdoc/export/html/_static/_tree.css
+-rw-r--r--   0        0        0     5637 2021-02-01 09:58:23.116497 strictdoc-0.0.9/strictdoc/export/html/_static/document_tree.css
+-rw-r--r--   0        0        0    92629 2021-02-01 09:58:23.116497 strictdoc-0.0.9/strictdoc/export/html/_static/jquery.min.js
+-rw-r--r--   0        0        0     2223 2021-02-01 09:58:23.116497 strictdoc-0.0.9/strictdoc/export/html/_static/pan-with-space.js
+-rw-r--r--   0        0        0      906 2021-02-01 09:58:23.116497 strictdoc-0.0.9/strictdoc/export/html/_static/toc.js
+-rw-r--r--   0        0        0      583 2021-02-01 09:58:23.116497 strictdoc-0.0.9/strictdoc/export/html/document_type.py
+-rw-r--r--   0        0        0      922 2021-02-01 09:58:23.116497 strictdoc-0.0.9/strictdoc/export/html/generators/document.py
+-rw-r--r--   0        0        0      912 2021-02-01 09:58:23.116497 strictdoc-0.0.9/strictdoc/export/html/generators/document_deep_trace.py
+-rw-r--r--   0        0        0      812 2021-02-01 09:58:23.116497 strictdoc-0.0.9/strictdoc/export/html/generators/document_table.py
+-rw-r--r--   0        0        0      876 2021-02-01 09:58:23.116497 strictdoc-0.0.9/strictdoc/export/html/generators/document_trace.py
+-rw-r--r--   0        0        0      710 2021-02-01 09:58:23.116497 strictdoc-0.0.9/strictdoc/export/html/generators/document_tree.py
+-rw-r--r--   0        0        0     7912 2021-02-01 09:58:23.116497 strictdoc-0.0.9/strictdoc/export/html/html_generator.py
+-rw-r--r--   0        0        0     2277 2021-02-01 09:58:23.116497 strictdoc-0.0.9/strictdoc/export/html/renderers/link_renderer.py
+-rw-r--r--   0        0        0     1727 2021-02-01 09:58:23.116497 strictdoc-0.0.9/strictdoc/export/html/renderers/markup_renderer.py
+-rw-r--r--   0        0        0      771 2021-02-01 09:58:23.116497 strictdoc-0.0.9/strictdoc/export/html/templates/_shared/docsection.jinja.html
+-rw-r--r--   0        0        0     3385 2021-02-01 09:58:23.116497 strictdoc-0.0.9/strictdoc/export/html/templates/_shared/requirement.jinja.html
+-rw-r--r--   0        0        0      248 2021-02-01 09:58:23.116497 strictdoc-0.0.9/strictdoc/export/html/templates/_shared/tags.jinja.html
+-rw-r--r--   0        0        0     1720 2021-02-01 09:58:23.116497 strictdoc-0.0.9/strictdoc/export/html/templates/_shared/toc.jinja.html
+-rw-r--r--   0        0        0     2799 2021-02-01 09:58:23.116497 strictdoc-0.0.9/strictdoc/export/html/templates/base.jinja.html
+-rw-r--r--   0        0        0     3984 2021-02-01 09:58:23.116497 strictdoc-0.0.9/strictdoc/export/html/templates/document_tree/document_tree.jinja.html
+-rw-r--r--   0        0        0     1219 2021-02-01 09:58:23.116497 strictdoc-0.0.9/strictdoc/export/html/templates/single_document/document.jinja.html
+-rw-r--r--   0        0        0     1573 2021-02-01 09:58:23.116497 strictdoc-0.0.9/strictdoc/export/html/templates/single_document_table/document.jinja.html
+-rw-r--r--   0        0        0     2066 2021-02-01 09:58:23.120497 strictdoc-0.0.9/strictdoc/export/html/templates/single_document_traceability/document.jinja.html
+-rw-r--r--   0        0        0     2517 2021-02-01 09:58:23.120497 strictdoc-0.0.9/strictdoc/export/html/templates/single_document_traceability_deep/document.jinja.html
+-rw-r--r--   0        0        0      573 2021-02-01 09:58:23.120497 strictdoc-0.0.9/strictdoc/export/html/templates/single_document_traceability_deep/recursive_cell_children.jinja.html
+-rw-r--r--   0        0        0      567 2021-02-01 09:58:23.120497 strictdoc-0.0.9/strictdoc/export/html/templates/single_document_traceability_deep/recursive_cell_parent.jinja.html
+-rw-r--r--   0        0        0     2893 2021-02-01 09:58:23.120497 strictdoc-0.0.9/strictdoc/export/html/tools/html_embedded.py
+-rw-r--r--   0        0        0     1150 2021-02-01 09:58:23.120497 strictdoc-0.0.9/strictdoc/export/rst/document_rst_generator.py
+-rw-r--r--   0        0        0      343 2021-02-01 09:58:23.120497 strictdoc-0.0.9/strictdoc/export/rst/rst_to_html_fragment_writer.py
+-rw-r--r--   0        0        0     4939 2021-02-01 09:58:23.120497 strictdoc-0.0.9/strictdoc/export/rst/writer.py
+-rw-r--r--   0        0        0      175 2021-02-01 09:58:23.120497 strictdoc-0.0.9/strictdoc/helpers/file_modification_time.py
+-rw-r--r--   0        0        0      289 2021-02-01 09:58:23.120497 strictdoc-0.0.9/strictdoc/helpers/file_system.py
+-rw-r--r--   0        0        0      748 2021-02-01 09:58:23.120497 strictdoc-0.0.9/strictdoc/helpers/parallelizer.py
+-rw-r--r--   0        0        0      343 2021-02-01 09:58:23.120497 strictdoc-0.0.9/strictdoc/helpers/sorting.py
+-rw-r--r--   0        0        0      691 2021-02-01 09:58:23.120497 strictdoc-0.0.9/strictdoc/helpers/timing.py
+-rw-r--r--   0        0        0     3782 2021-02-01 09:58:36.678387 strictdoc-0.0.9/setup.py
+-rw-r--r--   0        0        0     3046 2021-02-01 09:58:36.678839 strictdoc-0.0.9/PKG-INFO
```

### Comparing `strictdoc-0.0.8/LICENSE` & `strictdoc-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `strictdoc-0.0.8/pyproject.toml` & `strictdoc-0.0.9/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "strictdoc"
-version = "0.0.8"
+version = "0.0.9"
 description = " Software for writing technical requirements and specifications."
 authors = ["Stanislav Pankevich <s.pankevich@gmail.com>"]
 maintainers = ["Stanislav Pankevich <s.pankevich@gmail.com>"]
 license = "Apache 2"
 readme = "README.md"
 homepage = ""
 repository = "https://github.com/stanislaw/strictdoc"
@@ -17,26 +17,26 @@
 [tool.poetry.dependencies]
 python = "^3.6.2"
 textx = "2.3.0"
 jinja2 = "2.11.2"
 docutils = "0.16"
 XlsxWriter = "^1.3.7"
 python-datauri = "^0.2.9"
+beautifulsoup4 = '^4.9.3'
 
 [tool.poetry.dev-dependencies]
 invoke = "1.4.1"
-pytest = "*"
+pytest = "^6.2.2"
 lit = '0.11.0.post1'
 filecheck = "*"
 black = "20.8b1"
 pylint = "2.6.0"
 sphinx = '3.2.1'
 html5lib = '1.1'
 pytidylib = '0.3.2'
-beautifulsoup4 = '4.9.3'
 lxml = '4.6.2'
 openpyxl = '^3.0.5'
 
 # https://python-poetry.org/blog/announcing-poetry-1-1-0.html#standalone-build-backend
 # https://github.com/python-poetry/poetry/issues/3153#issuecomment-727196619
 [build-system]
 requires = ["setuptools", "poetry-core>=1.0.0"]
```

### Comparing `strictdoc-0.0.8/strictdoc/backend/dsl/error_handling.py` & `strictdoc-0.0.9/strictdoc/backend/dsl/error_handling.py`

 * *Files identical despite different names*

### Comparing `strictdoc-0.0.8/strictdoc/backend/dsl/grammar.py` & `strictdoc-0.0.9/strictdoc/backend/dsl/grammar.py`

 * *Files identical despite different names*

### Comparing `strictdoc-0.0.8/strictdoc/backend/dsl/models/config_special_field.py` & `strictdoc-0.0.9/strictdoc/backend/dsl/models/config_special_field.py`

 * *Files identical despite different names*

### Comparing `strictdoc-0.0.8/strictdoc/backend/dsl/models/document.py` & `strictdoc-0.0.9/strictdoc/backend/dsl/models/document.py`

 * *Files identical despite different names*

### Comparing `strictdoc-0.0.8/strictdoc/backend/dsl/models/document_config.py` & `strictdoc-0.0.9/strictdoc/backend/dsl/models/document_config.py`

 * *Files identical despite different names*

### Comparing `strictdoc-0.0.8/strictdoc/backend/dsl/models/requirement.py` & `strictdoc-0.0.9/strictdoc/backend/dsl/models/requirement.py`

 * *Files identical despite different names*

### Comparing `strictdoc-0.0.8/strictdoc/backend/dsl/models/section.py` & `strictdoc-0.0.9/strictdoc/backend/dsl/models/section.py`

 * *Files identical despite different names*

### Comparing `strictdoc-0.0.8/strictdoc/backend/dsl/reader.py` & `strictdoc-0.0.9/strictdoc/backend/dsl/reader.py`

 * *Files identical despite different names*

### Comparing `strictdoc-0.0.8/strictdoc/backend/dsl/writer.py` & `strictdoc-0.0.9/strictdoc/backend/dsl/writer.py`

 * *Files identical despite different names*

### Comparing `strictdoc-0.0.8/strictdoc/cli/cli_arg_parser.py` & `strictdoc-0.0.9/strictdoc/cli/cli_arg_parser.py`

 * *Files identical despite different names*

### Comparing `strictdoc-0.0.8/strictdoc/cli/main.py` & `strictdoc-0.0.9/strictdoc/cli/main.py`

 * *Files identical despite different names*

### Comparing `strictdoc-0.0.8/strictdoc/core/actions/export_action.py` & `strictdoc-0.0.9/strictdoc/core/actions/export_action.py`

 * *Files identical despite different names*

### Comparing `strictdoc-0.0.8/strictdoc/core/actions/passthrough_action.py` & `strictdoc-0.0.9/strictdoc/core/actions/passthrough_action.py`

 * *Files identical despite different names*

### Comparing `strictdoc-0.0.8/strictdoc/core/document_finder.py` & `strictdoc-0.0.9/strictdoc/core/document_finder.py`

 * *Files identical despite different names*

### Comparing `strictdoc-0.0.8/strictdoc/core/document_iterator.py` & `strictdoc-0.0.9/strictdoc/core/document_iterator.py`

 * *Files identical despite different names*

### Comparing `strictdoc-0.0.8/strictdoc/core/document_meta.py` & `strictdoc-0.0.9/strictdoc/core/document_meta.py`

 * *Files identical despite different names*

### Comparing `strictdoc-0.0.8/strictdoc/core/document_tree.py` & `strictdoc-0.0.9/strictdoc/core/document_tree.py`

 * *Files identical despite different names*

### Comparing `strictdoc-0.0.8/strictdoc/core/document_tree_iterator.py` & `strictdoc-0.0.9/strictdoc/core/document_tree_iterator.py`

 * *Files identical despite different names*

### Comparing `strictdoc-0.0.8/strictdoc/core/level_counter.py` & `strictdoc-0.0.9/strictdoc/core/level_counter.py`

 * *Files identical despite different names*

### Comparing `strictdoc-0.0.8/strictdoc/core/logger.py` & `strictdoc-0.0.9/strictdoc/core/logger.py`

 * *Files identical despite different names*

### Comparing `strictdoc-0.0.8/strictdoc/core/traceability_index.py` & `strictdoc-0.0.9/strictdoc/core/traceability_index.py`

 * *Files identical despite different names*

### Comparing `strictdoc-0.0.8/strictdoc/export/excel/excel_generator.py` & `strictdoc-0.0.9/strictdoc/export/excel/excel_generator.py`

 * *Files identical despite different names*

### Comparing `strictdoc-0.0.8/strictdoc/export/html/_static/_base.css` & `strictdoc-0.0.9/strictdoc/export/html/_static/_base.css`

 * *Files identical despite different names*

### Comparing `strictdoc-0.0.8/strictdoc/export/html/_static/_content.css` & `strictdoc-0.0.9/strictdoc/export/html/_static/_content.css`

 * *Files identical despite different names*

### Comparing `strictdoc-0.0.8/strictdoc/export/html/_static/_element.css` & `strictdoc-0.0.9/strictdoc/export/html/_static/_element.css`

 * *Files 2% similar despite different names*

```diff
@@ -190,15 +190,16 @@
             calc(var(--code-font-size)*2);
 
   overflow: auto;
   background-color: var(--color-bg-main);
   border: 1px solid var(--color-border);
 }
 
-cite {
+/* ``some text`` is generated into: <tt class="docutils literal"> by docutils. */
+tt.literal {
   position: relative;
   padding: 2px 6px;
   font-style: normal;
   font-family: var(--code-font-family);
   font-size: var(--code-font-size);
   background-color: var(--color-bg-main);
   border: 1px solid var(--color-border);
```

### Comparing `strictdoc-0.0.8/strictdoc/export/html/_static/_layout.css` & `strictdoc-0.0.9/strictdoc/export/html/_static/_layout.css`

 * *Files identical despite different names*

### Comparing `strictdoc-0.0.8/strictdoc/export/html/_static/_tree.css` & `strictdoc-0.0.9/strictdoc/export/html/_static/_tree.css`

 * *Files identical despite different names*

### Comparing `strictdoc-0.0.8/strictdoc/export/html/_static/document_tree.css` & `strictdoc-0.0.9/strictdoc/export/html/_static/document_tree.css`

 * *Files identical despite different names*

### Comparing `strictdoc-0.0.8/strictdoc/export/html/_static/jquery.min.js` & `strictdoc-0.0.9/strictdoc/export/html/_static/jquery.min.js`

 * *Files identical despite different names*

### Comparing `strictdoc-0.0.8/strictdoc/export/html/_static/pan-with-space.js` & `strictdoc-0.0.9/strictdoc/export/html/_static/pan-with-space.js`

 * *Files identical despite different names*

### Comparing `strictdoc-0.0.8/strictdoc/export/html/_static/toc.js` & `strictdoc-0.0.9/strictdoc/export/html/_static/toc.js`

 * *Files identical despite different names*

### Comparing `strictdoc-0.0.8/strictdoc/export/html/document_type.py` & `strictdoc-0.0.9/strictdoc/export/html/document_type.py`

 * *Files identical despite different names*

### Comparing `strictdoc-0.0.8/strictdoc/export/html/generators/document.py` & `strictdoc-0.0.9/strictdoc/export/html/generators/document.py`

 * *Files identical despite different names*

### Comparing `strictdoc-0.0.8/strictdoc/export/html/generators/document_deep_trace.py` & `strictdoc-0.0.9/strictdoc/export/html/generators/document_deep_trace.py`

 * *Files identical despite different names*

### Comparing `strictdoc-0.0.8/strictdoc/export/html/generators/document_table.py` & `strictdoc-0.0.9/strictdoc/export/html/generators/document_table.py`

 * *Files identical despite different names*

### Comparing `strictdoc-0.0.8/strictdoc/export/html/generators/document_trace.py` & `strictdoc-0.0.9/strictdoc/export/html/generators/document_trace.py`

 * *Files identical despite different names*

### Comparing `strictdoc-0.0.8/strictdoc/export/html/generators/document_tree.py` & `strictdoc-0.0.9/strictdoc/export/html/generators/document_tree.py`

 * *Files identical despite different names*

### Comparing `strictdoc-0.0.8/strictdoc/export/html/html_generator.py` & `strictdoc-0.0.9/strictdoc/export/html/html_generator.py`

 * *Files identical despite different names*

### Comparing `strictdoc-0.0.8/strictdoc/export/html/renderers/link_renderer.py` & `strictdoc-0.0.9/strictdoc/export/html/renderers/link_renderer.py`

 * *Files identical despite different names*

### Comparing `strictdoc-0.0.8/strictdoc/export/html/renderers/markup_renderer.py` & `strictdoc-0.0.9/strictdoc/export/html/renderers/markup_renderer.py`

 * *Files identical despite different names*

### Comparing `strictdoc-0.0.8/strictdoc/export/html/templates/_shared/docsection.jinja.html` & `strictdoc-0.0.9/strictdoc/export/html/templates/_shared/docsection.jinja.html`

 * *Files identical despite different names*

### Comparing `strictdoc-0.0.8/strictdoc/export/html/templates/_shared/requirement.jinja.html` & `strictdoc-0.0.9/strictdoc/export/html/templates/_shared/requirement.jinja.html`

 * *Files identical despite different names*

### Comparing `strictdoc-0.0.8/strictdoc/export/html/templates/_shared/toc.jinja.html` & `strictdoc-0.0.9/strictdoc/export/html/templates/_shared/toc.jinja.html`

 * *Files identical despite different names*

### Comparing `strictdoc-0.0.8/strictdoc/export/html/templates/base.jinja.html` & `strictdoc-0.0.9/strictdoc/export/html/templates/base.jinja.html`

 * *Files identical despite different names*

### Comparing `strictdoc-0.0.8/strictdoc/export/html/templates/document_tree/document_tree.jinja.html` & `strictdoc-0.0.9/strictdoc/export/html/templates/document_tree/document_tree.jinja.html`

 * *Files identical despite different names*

### Comparing `strictdoc-0.0.8/strictdoc/export/html/templates/single_document/document.jinja.html` & `strictdoc-0.0.9/strictdoc/export/html/templates/single_document/document.jinja.html`

 * *Files identical despite different names*

### Comparing `strictdoc-0.0.8/strictdoc/export/html/templates/single_document_table/document.jinja.html` & `strictdoc-0.0.9/strictdoc/export/html/templates/single_document_table/document.jinja.html`

 * *Files identical despite different names*

### Comparing `strictdoc-0.0.8/strictdoc/export/html/templates/single_document_traceability/document.jinja.html` & `strictdoc-0.0.9/strictdoc/export/html/templates/single_document_traceability/document.jinja.html`

 * *Files identical despite different names*

### Comparing `strictdoc-0.0.8/strictdoc/export/html/templates/single_document_traceability_deep/document.jinja.html` & `strictdoc-0.0.9/strictdoc/export/html/templates/single_document_traceability_deep/document.jinja.html`

 * *Files identical despite different names*

### Comparing `strictdoc-0.0.8/strictdoc/export/html/templates/single_document_traceability_deep/recursive_cell_children.jinja.html` & `strictdoc-0.0.9/strictdoc/export/html/templates/single_document_traceability_deep/recursive_cell_children.jinja.html`

 * *Files identical despite different names*

### Comparing `strictdoc-0.0.8/strictdoc/export/html/templates/single_document_traceability_deep/recursive_cell_parent.jinja.html` & `strictdoc-0.0.9/strictdoc/export/html/templates/single_document_traceability_deep/recursive_cell_parent.jinja.html`

 * *Files identical despite different names*

### Comparing `strictdoc-0.0.8/strictdoc/export/html/tools/html_embedded.py` & `strictdoc-0.0.9/strictdoc/export/html/tools/html_embedded.py`

 * *Files identical despite different names*

### Comparing `strictdoc-0.0.8/strictdoc/export/rst/document_rst_generator.py` & `strictdoc-0.0.9/strictdoc/export/rst/document_rst_generator.py`

 * *Files identical despite different names*

### Comparing `strictdoc-0.0.8/strictdoc/export/rst/writer.py` & `strictdoc-0.0.9/strictdoc/export/rst/writer.py`

 * *Files identical despite different names*

### Comparing `strictdoc-0.0.8/strictdoc/helpers/parallelizer.py` & `strictdoc-0.0.9/strictdoc/helpers/parallelizer.py`

 * *Files identical despite different names*

### Comparing `strictdoc-0.0.8/strictdoc/helpers/timing.py` & `strictdoc-0.0.9/strictdoc/helpers/timing.py`

 * *Files identical despite different names*

