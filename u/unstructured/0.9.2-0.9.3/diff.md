# Comparing `tmp/unstructured-0.9.2.tar.gz` & `tmp/unstructured-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unstructured-0.9.2.tar", last modified: Fri Aug 11 02:32:46 2023, max compression
+gzip compressed data, was "unstructured-0.9.3.tar", last modified: Tue Aug 15 05:20:36 2023, max compression
```

## Comparing `unstructured-0.9.2.tar` & `unstructured-0.9.3.tar`

### file list

```diff
@@ -1,202 +1,273 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-11 02:32:46.293376 unstructured-0.9.2/
--rw-r--r--   0 runner    (1001) docker     (123)    11360 2023-08-11 02:32:35.000000 unstructured-0.9.2/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)      639 2023-08-11 02:32:35.000000 unstructured-0.9.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    20849 2023-08-11 02:32:46.293376 unstructured-0.9.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    16707 2023-08-11 02:32:35.000000 unstructured-0.9.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-11 02:32:46.217376 unstructured-0.9.2/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-08-11 02:32:35.000000 unstructured-0.9.2/requirements/base.in
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-08-11 02:32:35.000000 unstructured-0.9.2/requirements/huggingface.in
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-08-11 02:32:35.000000 unstructured-0.9.2/requirements/ingest-azure.in
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-08-11 02:32:35.000000 unstructured-0.9.2/requirements/ingest-box.in
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-08-11 02:32:35.000000 unstructured-0.9.2/requirements/ingest-discord.in
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-08-11 02:32:35.000000 unstructured-0.9.2/requirements/ingest-dropbox.in
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-08-11 02:32:35.000000 unstructured-0.9.2/requirements/ingest-gcs.in
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-08-11 02:32:35.000000 unstructured-0.9.2/requirements/ingest-github.in
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-08-11 02:32:35.000000 unstructured-0.9.2/requirements/ingest-gitlab.in
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-08-11 02:32:35.000000 unstructured-0.9.2/requirements/ingest-google-drive.in
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-08-11 02:32:35.000000 unstructured-0.9.2/requirements/ingest-onedrive.in
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-08-11 02:32:35.000000 unstructured-0.9.2/requirements/ingest-outlook.in
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-08-11 02:32:35.000000 unstructured-0.9.2/requirements/ingest-reddit.in
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-08-11 02:32:35.000000 unstructured-0.9.2/requirements/ingest-s3.in
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-08-11 02:32:35.000000 unstructured-0.9.2/requirements/ingest-slack.in
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-08-11 02:32:35.000000 unstructured-0.9.2/requirements/ingest-wikipedia.in
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-08-11 02:32:46.293376 unstructured-0.9.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     5810 2023-08-11 02:32:35.000000 unstructured-0.9.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-11 02:32:46.217376 unstructured-0.9.2/test_unstructured/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-11 02:32:35.000000 unstructured-0.9.2/test_unstructured/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-11 02:32:46.221376 unstructured-0.9.2/test_unstructured/nlp/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-11 02:32:35.000000 unstructured-0.9.2/test_unstructured/nlp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      566 2023-08-11 02:32:35.000000 unstructured-0.9.2/test_unstructured/nlp/mock_nltk.py
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-08-11 02:32:35.000000 unstructured-0.9.2/test_unstructured/nlp/test_partition.py
--rw-r--r--   0 runner    (1001) docker     (123)     2731 2023-08-11 02:32:35.000000 unstructured-0.9.2/test_unstructured/nlp/test_tokenize.py
--rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-08-11 02:32:35.000000 unstructured-0.9.2/test_unstructured/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-11 02:32:46.221376 unstructured-0.9.2/unstructured/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-11 02:32:35.000000 unstructured-0.9.2/unstructured/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-08-11 02:32:35.000000 unstructured-0.9.2/unstructured/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-11 02:32:46.225376 unstructured-0.9.2/unstructured/cleaners/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-11 02:32:35.000000 unstructured-0.9.2/unstructured/cleaners/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11050 2023-08-11 02:32:35.000000 unstructured-0.9.2/unstructured/cleaners/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     4209 2023-08-11 02:32:35.000000 unstructured-0.9.2/unstructured/cleaners/extract.py
--rw-r--r--   0 runner    (1001) docker     (123)     3250 2023-08-11 02:32:35.000000 unstructured-0.9.2/unstructured/cleaners/translate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-11 02:32:46.229375 unstructured-0.9.2/unstructured/documents/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-11 02:32:35.000000 unstructured-0.9.2/unstructured/documents/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3331 2023-08-11 02:32:35.000000 unstructured-0.9.2/unstructured/documents/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3331 2023-08-11 02:32:35.000000 unstructured-0.9.2/unstructured/documents/coordinates.py
--rw-r--r--   0 runner    (1001) docker     (123)    16096 2023-08-11 02:32:35.000000 unstructured-0.9.2/unstructured/documents/elements.py
--rw-r--r--   0 runner    (1001) docker     (123)     3454 2023-08-11 02:32:35.000000 unstructured-0.9.2/unstructured/documents/email_elements.py
--rw-r--r--   0 runner    (1001) docker     (123)    18363 2023-08-11 02:32:35.000000 unstructured-0.9.2/unstructured/documents/html.py
--rw-r--r--   0 runner    (1001) docker     (123)     5301 2023-08-11 02:32:35.000000 unstructured-0.9.2/unstructured/documents/xml.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-11 02:32:46.233376 unstructured-0.9.2/unstructured/file_utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-11 02:32:35.000000 unstructured-0.9.2/unstructured/file_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4413 2023-08-11 02:32:35.000000 unstructured-0.9.2/unstructured/file_utils/encoding.py
--rw-r--r--   0 runner    (1001) docker     (123)     2398 2023-08-11 02:32:35.000000 unstructured-0.9.2/unstructured/file_utils/exploration.py
--rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-08-11 02:32:35.000000 unstructured-0.9.2/unstructured/file_utils/file_conversion.py
--rw-r--r--   0 runner    (1001) docker     (123)    20754 2023-08-11 02:32:35.000000 unstructured-0.9.2/unstructured/file_utils/filetype.py
--rw-r--r--   0 runner    (1001) docker     (123)      468 2023-08-11 02:32:35.000000 unstructured-0.9.2/unstructured/file_utils/google_filetype.py
--rw-r--r--   0 runner    (1001) docker     (123)     5420 2023-08-11 02:32:35.000000 unstructured-0.9.2/unstructured/file_utils/metadata.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-11 02:32:46.233376 unstructured-0.9.2/unstructured/ingest/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-11 02:32:35.000000 unstructured-0.9.2/unstructured/ingest/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-11 02:32:46.237376 unstructured-0.9.2/unstructured/ingest/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-11 02:32:35.000000 unstructured-0.9.2/unstructured/ingest/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      903 2023-08-11 02:32:35.000000 unstructured-0.9.2/unstructured/ingest/cli/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-11 02:32:46.245376 unstructured-0.9.2/unstructured/ingest/cli/cmds/
--rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-08-11 02:32:35.000000 unstructured-0.9.2/unstructured/ingest/cli/cmds/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-08-11 02:32:35.000000 unstructured-0.9.2/unstructured/ingest/cli/cmds/azure.py
--rw-r--r--   0 runner    (1001) docker     (123)     1742 2023-08-11 02:32:35.000000 unstructured-0.9.2/unstructured/ingest/cli/cmds/biomed.py
--rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-08-11 02:32:35.000000 unstructured-0.9.2/unstructured/ingest/cli/cmds/box.py
--rw-r--r--   0 runner    (1001) docker     (123)     2533 2023-08-11 02:32:35.000000 unstructured-0.9.2/unstructured/ingest/cli/cmds/confluence.py
--rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-08-11 02:32:35.000000 unstructured-0.9.2/unstructured/ingest/cli/cmds/discord.py
--rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-08-11 02:32:35.000000 unstructured-0.9.2/unstructured/ingest/cli/cmds/dropbox.py
--rw-r--r--   0 runner    (1001) docker     (123)     1656 2023-08-11 02:32:35.000000 unstructured-0.9.2/unstructured/ingest/cli/cmds/elasticsearch.py
--rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-08-11 02:32:35.000000 unstructured-0.9.2/unstructured/ingest/cli/cmds/fsspec.py
--rw-r--r--   0 runner    (1001) docker     (123)     1319 2023-08-11 02:32:35.000000 unstructured-0.9.2/unstructured/ingest/cli/cmds/gcs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1796 2023-08-11 02:32:35.000000 unstructured-0.9.2/unstructured/ingest/cli/cmds/github.py
--rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-08-11 02:32:35.000000 unstructured-0.9.2/unstructured/ingest/cli/cmds/gitlab.py
--rw-r--r--   0 runner    (1001) docker     (123)     1410 2023-08-11 02:32:35.000000 unstructured-0.9.2/unstructured/ingest/cli/cmds/google_drive.py
--rw-r--r--   0 runner    (1001) docker     (123)     1354 2023-08-11 02:32:35.000000 unstructured-0.9.2/unstructured/ingest/cli/cmds/local.py
--rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-08-11 02:32:35.000000 unstructured-0.9.2/unstructured/ingest/cli/cmds/notion.py
--rw-r--r--   0 runner    (1001) docker     (123)     1784 2023-08-11 02:32:35.000000 unstructured-0.9.2/unstructured/ingest/cli/cmds/onedrive.py
--rw-r--r--   0 runner    (1001) docker     (123)     1878 2023-08-11 02:32:35.000000 unstructured-0.9.2/unstructured/ingest/cli/cmds/outlook.py
--rw-r--r--   0 runner    (1001) docker     (123)     2046 2023-08-11 02:32:35.000000 unstructured-0.9.2/unstructured/ingest/cli/cmds/reddit.py
--rw-r--r--   0 runner    (1001) docker     (123)     1209 2023-08-11 02:32:35.000000 unstructured-0.9.2/unstructured/ingest/cli/cmds/s3.py
--rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-08-11 02:32:35.000000 unstructured-0.9.2/unstructured/ingest/cli/cmds/sharepoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1667 2023-08-11 02:32:35.000000 unstructured-0.9.2/unstructured/ingest/cli/cmds/slack.py
--rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-08-11 02:32:35.000000 unstructured-0.9.2/unstructured/ingest/cli/cmds/wikipedia.py
--rw-r--r--   0 runner    (1001) docker     (123)     9951 2023-08-11 02:32:35.000000 unstructured-0.9.2/unstructured/ingest/cli/common.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-11 02:32:46.257376 unstructured-0.9.2/unstructured/ingest/connector/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-11 02:32:35.000000 unstructured-0.9.2/unstructured/ingest/connector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      952 2023-08-11 02:32:35.000000 unstructured-0.9.2/unstructured/ingest/connector/azure.py
--rw-r--r--   0 runner    (1001) docker     (123)     9521 2023-08-11 02:32:35.000000 unstructured-0.9.2/unstructured/ingest/connector/biomed.py
--rw-r--r--   0 runner    (1001) docker     (123)     2618 2023-08-11 02:32:35.000000 unstructured-0.9.2/unstructured/ingest/connector/box.py
--rw-r--r--   0 runner    (1001) docker     (123)     6877 2023-08-11 02:32:35.000000 unstructured-0.9.2/unstructured/ingest/connector/confluence.py
--rw-r--r--   0 runner    (1001) docker     (123)     4534 2023-08-11 02:32:35.000000 unstructured-0.9.2/unstructured/ingest/connector/discord.py
--rw-r--r--   0 runner    (1001) docker     (123)     4564 2023-08-11 02:32:35.000000 unstructured-0.9.2/unstructured/ingest/connector/dropbox.py
--rw-r--r--   0 runner    (1001) docker     (123)     5958 2023-08-11 02:32:35.000000 unstructured-0.9.2/unstructured/ingest/connector/elasticsearch.py
--rw-r--r--   0 runner    (1001) docker     (123)     5706 2023-08-11 02:32:35.000000 unstructured-0.9.2/unstructured/ingest/connector/fsspec.py
--rw-r--r--   0 runner    (1001) docker     (123)      847 2023-08-11 02:32:35.000000 unstructured-0.9.2/unstructured/ingest/connector/gcs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2741 2023-08-11 02:32:35.000000 unstructured-0.9.2/unstructured/ingest/connector/git.py
--rw-r--r--   0 runner    (1001) docker     (123)     3123 2023-08-11 02:32:35.000000 unstructured-0.9.2/unstructured/ingest/connector/github.py
--rw-r--r--   0 runner    (1001) docker     (123)     2296 2023-08-11 02:32:35.000000 unstructured-0.9.2/unstructured/ingest/connector/gitlab.py
--rw-r--r--   0 runner    (1001) docker     (123)     9598 2023-08-11 02:32:35.000000 unstructured-0.9.2/unstructured/ingest/connector/google_drive.py
--rw-r--r--   0 runner    (1001) docker     (123)     3379 2023-08-11 02:32:35.000000 unstructured-0.9.2/unstructured/ingest/connector/local.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-11 02:32:46.257376 unstructured-0.9.2/unstructured/ingest/connector/notion/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-11 02:32:35.000000 unstructured-0.9.2/unstructured/ingest/connector/notion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3840 2023-08-11 02:32:35.000000 unstructured-0.9.2/unstructured/ingest/connector/notion/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    15023 2023-08-11 02:32:35.000000 unstructured-0.9.2/unstructured/ingest/connector/notion/connector.py
--rw-r--r--   0 runner    (1001) docker     (123)    18419 2023-08-11 02:32:35.000000 unstructured-0.9.2/unstructured/ingest/connector/notion/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)      563 2023-08-11 02:32:35.000000 unstructured-0.9.2/unstructured/ingest/connector/notion/interfaces.py
--rw-r--r--   0 runner    (1001) docker     (123)     5987 2023-08-11 02:32:35.000000 unstructured-0.9.2/unstructured/ingest/connector/onedrive.py
--rw-r--r--   0 runner    (1001) docker     (123)     8165 2023-08-11 02:32:35.000000 unstructured-0.9.2/unstructured/ingest/connector/outlook.py
--rw-r--r--   0 runner    (1001) docker     (123)     2743 2023-08-11 02:32:35.000000 unstructured-0.9.2/unstructured/ingest/connector/reddit.py
--rw-r--r--   0 runner    (1001) docker     (123)      837 2023-08-11 02:32:35.000000 unstructured-0.9.2/unstructured/ingest/connector/s3.py
--rw-r--r--   0 runner    (1001) docker     (123)    12948 2023-08-11 02:32:35.000000 unstructured-0.9.2/unstructured/ingest/connector/sharepoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     5411 2023-08-11 02:32:35.000000 unstructured-0.9.2/unstructured/ingest/connector/slack.py
--rw-r--r--   0 runner    (1001) docker     (123)     3631 2023-08-11 02:32:35.000000 unstructured-0.9.2/unstructured/ingest/connector/wikipedia.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-11 02:32:46.257376 unstructured-0.9.2/unstructured/ingest/doc_processor/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-11 02:32:35.000000 unstructured-0.9.2/unstructured/ingest/doc_processor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-08-11 02:32:35.000000 unstructured-0.9.2/unstructured/ingest/doc_processor/generalized.py
--rw-r--r--   0 runner    (1001) docker     (123)    12548 2023-08-11 02:32:35.000000 unstructured-0.9.2/unstructured/ingest/interfaces.py
--rw-r--r--   0 runner    (1001) docker     (123)      903 2023-08-11 02:32:35.000000 unstructured-0.9.2/unstructured/ingest/logger.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      169 2023-08-11 02:32:35.000000 unstructured-0.9.2/unstructured/ingest/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     3802 2023-08-11 02:32:35.000000 unstructured-0.9.2/unstructured/ingest/processor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-11 02:32:46.269376 unstructured-0.9.2/unstructured/ingest/runner/
--rw-r--r--   0 runner    (1001) docker     (123)      912 2023-08-11 02:32:35.000000 unstructured-0.9.2/unstructured/ingest/runner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1778 2023-08-11 02:32:35.000000 unstructured-0.9.2/unstructured/ingest/runner/azure.py
--rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-08-11 02:32:35.000000 unstructured-0.9.2/unstructured/ingest/runner/biomed.py
--rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-08-11 02:32:35.000000 unstructured-0.9.2/unstructured/ingest/runner/box.py
--rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-08-11 02:32:35.000000 unstructured-0.9.2/unstructured/ingest/runner/confluence.py
--rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-08-11 02:32:35.000000 unstructured-0.9.2/unstructured/ingest/runner/discord.py
--rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-08-11 02:32:35.000000 unstructured-0.9.2/unstructured/ingest/runner/dropbox.py
--rw-r--r--   0 runner    (1001) docker     (123)     1391 2023-08-11 02:32:35.000000 unstructured-0.9.2/unstructured/ingest/runner/elasticsearch.py
--rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-08-11 02:32:35.000000 unstructured-0.9.2/unstructured/ingest/runner/fsspec.py
--rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-08-11 02:32:35.000000 unstructured-0.9.2/unstructured/ingest/runner/gcs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1436 2023-08-11 02:32:35.000000 unstructured-0.9.2/unstructured/ingest/runner/github.py
--rw-r--r--   0 runner    (1001) docker     (123)     1436 2023-08-11 02:32:35.000000 unstructured-0.9.2/unstructured/ingest/runner/gitlab.py
--rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-08-11 02:32:35.000000 unstructured-0.9.2/unstructured/ingest/runner/google_drive.py
--rw-r--r--   0 runner    (1001) docker     (123)      982 2023-08-11 02:32:35.000000 unstructured-0.9.2/unstructured/ingest/runner/local.py
--rw-r--r--   0 runner    (1001) docker     (123)     2073 2023-08-11 02:32:35.000000 unstructured-0.9.2/unstructured/ingest/runner/notion.py
--rw-r--r--   0 runner    (1001) docker     (123)     1585 2023-08-11 02:32:35.000000 unstructured-0.9.2/unstructured/ingest/runner/onedrive.py
--rw-r--r--   0 runner    (1001) docker     (123)     1702 2023-08-11 02:32:35.000000 unstructured-0.9.2/unstructured/ingest/runner/outlook.py
--rw-r--r--   0 runner    (1001) docker     (123)     1555 2023-08-11 02:32:35.000000 unstructured-0.9.2/unstructured/ingest/runner/reddit.py
--rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-08-11 02:32:35.000000 unstructured-0.9.2/unstructured/ingest/runner/s3.py
--rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-08-11 02:32:35.000000 unstructured-0.9.2/unstructured/ingest/runner/sharepoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-08-11 02:32:35.000000 unstructured-0.9.2/unstructured/ingest/runner/slack.py
--rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-08-11 02:32:35.000000 unstructured-0.9.2/unstructured/ingest/runner/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-08-11 02:32:35.000000 unstructured-0.9.2/unstructured/ingest/runner/wikipedia.py
--rw-r--r--   0 runner    (1001) docker     (123)      480 2023-08-11 02:32:35.000000 unstructured-0.9.2/unstructured/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-11 02:32:46.269376 unstructured-0.9.2/unstructured/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-11 02:32:35.000000 unstructured-0.9.2/unstructured/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-11 02:32:46.277376 unstructured-0.9.2/unstructured/nlp/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-11 02:32:35.000000 unstructured-0.9.2/unstructured/nlp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)  4472047 2023-08-11 02:32:35.000000 unstructured-0.9.2/unstructured/nlp/english-words.txt
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-08-11 02:32:35.000000 unstructured-0.9.2/unstructured/nlp/english_words.py
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-08-11 02:32:35.000000 unstructured-0.9.2/unstructured/nlp/partition.py
--rw-r--r--   0 runner    (1001) docker     (123)     5550 2023-08-11 02:32:35.000000 unstructured-0.9.2/unstructured/nlp/patterns.py
--rw-r--r--   0 runner    (1001) docker     (123)     2090 2023-08-11 02:32:35.000000 unstructured-0.9.2/unstructured/nlp/tokenize.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-11 02:32:46.289376 unstructured-0.9.2/unstructured/partition/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-11 02:32:35.000000 unstructured-0.9.2/unstructured/partition/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6619 2023-08-11 02:32:35.000000 unstructured-0.9.2/unstructured/partition/api.py
--rw-r--r--   0 runner    (1001) docker     (123)    12467 2023-08-11 02:32:35.000000 unstructured-0.9.2/unstructured/partition/auto.py
--rw-r--r--   0 runner    (1001) docker     (123)    10854 2023-08-11 02:32:35.000000 unstructured-0.9.2/unstructured/partition/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     2229 2023-08-11 02:32:35.000000 unstructured-0.9.2/unstructured/partition/csv.py
--rw-r--r--   0 runner    (1001) docker     (123)     3046 2023-08-11 02:32:35.000000 unstructured-0.9.2/unstructured/partition/doc.py
--rw-r--r--   0 runner    (1001) docker     (123)    13938 2023-08-11 02:32:35.000000 unstructured-0.9.2/unstructured/partition/docx.py
--rw-r--r--   0 runner    (1001) docker     (123)    14888 2023-08-11 02:32:35.000000 unstructured-0.9.2/unstructured/partition/email.py
--rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-08-11 02:32:35.000000 unstructured-0.9.2/unstructured/partition/epub.py
--rw-r--r--   0 runner    (1001) docker     (123)     6542 2023-08-11 02:32:35.000000 unstructured-0.9.2/unstructured/partition/html.py
--rw-r--r--   0 runner    (1001) docker     (123)     2370 2023-08-11 02:32:35.000000 unstructured-0.9.2/unstructured/partition/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     2527 2023-08-11 02:32:35.000000 unstructured-0.9.2/unstructured/partition/json.py
--rw-r--r--   0 runner    (1001) docker     (123)     3174 2023-08-11 02:32:35.000000 unstructured-0.9.2/unstructured/partition/md.py
--rw-r--r--   0 runner    (1001) docker     (123)     5813 2023-08-11 02:32:35.000000 unstructured-0.9.2/unstructured/partition/msg.py
--rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-08-11 02:32:35.000000 unstructured-0.9.2/unstructured/partition/odt.py
--rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-08-11 02:32:35.000000 unstructured-0.9.2/unstructured/partition/org.py
--rw-r--r--   0 runner    (1001) docker     (123)    17794 2023-08-11 02:32:35.000000 unstructured-0.9.2/unstructured/partition/pdf.py
--rw-r--r--   0 runner    (1001) docker     (123)     2795 2023-08-11 02:32:35.000000 unstructured-0.9.2/unstructured/partition/ppt.py
--rw-r--r--   0 runner    (1001) docker     (123)     5907 2023-08-11 02:32:35.000000 unstructured-0.9.2/unstructured/partition/pptx.py
--rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-08-11 02:32:35.000000 unstructured-0.9.2/unstructured/partition/rst.py
--rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-08-11 02:32:35.000000 unstructured-0.9.2/unstructured/partition/rtf.py
--rw-r--r--   0 runner    (1001) docker     (123)     4781 2023-08-11 02:32:35.000000 unstructured-0.9.2/unstructured/partition/strategies.py
--rw-r--r--   0 runner    (1001) docker     (123)     9318 2023-08-11 02:32:35.000000 unstructured-0.9.2/unstructured/partition/text.py
--rw-r--r--   0 runner    (1001) docker     (123)    11494 2023-08-11 02:32:35.000000 unstructured-0.9.2/unstructured/partition/text_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     2170 2023-08-11 02:32:35.000000 unstructured-0.9.2/unstructured/partition/tsv.py
--rw-r--r--   0 runner    (1001) docker     (123)     2721 2023-08-11 02:32:35.000000 unstructured-0.9.2/unstructured/partition/xlsx.py
--rw-r--r--   0 runner    (1001) docker     (123)     4163 2023-08-11 02:32:35.000000 unstructured-0.9.2/unstructured/partition/xml.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-11 02:32:46.289376 unstructured-0.9.2/unstructured/staging/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-11 02:32:35.000000 unstructured-0.9.2/unstructured/staging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2288 2023-08-11 02:32:35.000000 unstructured-0.9.2/unstructured/staging/argilla.py
--rw-r--r--   0 runner    (1001) docker     (123)     6958 2023-08-11 02:32:35.000000 unstructured-0.9.2/unstructured/staging/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1755 2023-08-11 02:32:35.000000 unstructured-0.9.2/unstructured/staging/baseplate.py
--rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-08-11 02:32:35.000000 unstructured-0.9.2/unstructured/staging/datasaur.py
--rw-r--r--   0 runner    (1001) docker     (123)     3838 2023-08-11 02:32:35.000000 unstructured-0.9.2/unstructured/staging/huggingface.py
--rw-r--r--   0 runner    (1001) docker     (123)     3916 2023-08-11 02:32:35.000000 unstructured-0.9.2/unstructured/staging/label_box.py
--rw-r--r--   0 runner    (1001) docker     (123)     4904 2023-08-11 02:32:35.000000 unstructured-0.9.2/unstructured/staging/label_studio.py
--rw-r--r--   0 runner    (1001) docker     (123)     3188 2023-08-11 02:32:35.000000 unstructured-0.9.2/unstructured/staging/prodigy.py
--rw-r--r--   0 runner    (1001) docker     (123)     2534 2023-08-11 02:32:35.000000 unstructured-0.9.2/unstructured/staging/weaviate.py
--rw-r--r--   0 runner    (1001) docker     (123)     2311 2023-08-11 02:32:35.000000 unstructured-0.9.2/unstructured/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-11 02:32:46.225376 unstructured-0.9.2/unstructured.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    20849 2023-08-11 02:32:46.000000 unstructured-0.9.2/unstructured.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6320 2023-08-11 02:32:46.000000 unstructured-0.9.2/unstructured.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-11 02:32:46.000000 unstructured-0.9.2/unstructured.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-08-11 02:32:46.000000 unstructured-0.9.2/unstructured.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-08-11 02:32:46.000000 unstructured-0.9.2/unstructured.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-08-11 02:32:46.000000 unstructured-0.9.2/unstructured.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-15 05:20:36.606748 unstructured-0.9.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    11360 2023-08-15 05:20:24.000000 unstructured-0.9.3/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      806 2023-08-15 05:20:24.000000 unstructured-0.9.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    20208 2023-08-15 05:20:36.606748 unstructured-0.9.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    16366 2023-08-15 05:20:24.000000 unstructured-0.9.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-15 05:20:36.566748 unstructured-0.9.3/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-08-15 05:20:24.000000 unstructured-0.9.3/requirements/base.in
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-08-15 05:20:24.000000 unstructured-0.9.3/requirements/huggingface.in
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-08-15 05:20:24.000000 unstructured-0.9.3/requirements/ingest-airtable.in
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-08-15 05:20:24.000000 unstructured-0.9.3/requirements/ingest-azure.in
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-08-15 05:20:24.000000 unstructured-0.9.3/requirements/ingest-box.in
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-08-15 05:20:24.000000 unstructured-0.9.3/requirements/ingest-confluence.in
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-08-15 05:20:24.000000 unstructured-0.9.3/requirements/ingest-discord.in
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-08-15 05:20:24.000000 unstructured-0.9.3/requirements/ingest-dropbox.in
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-08-15 05:20:24.000000 unstructured-0.9.3/requirements/ingest-elasticsearch.in
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-08-15 05:20:24.000000 unstructured-0.9.3/requirements/ingest-gcs.in
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-08-15 05:20:24.000000 unstructured-0.9.3/requirements/ingest-github.in
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-08-15 05:20:24.000000 unstructured-0.9.3/requirements/ingest-gitlab.in
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-08-15 05:20:24.000000 unstructured-0.9.3/requirements/ingest-google-drive.in
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-08-15 05:20:24.000000 unstructured-0.9.3/requirements/ingest-notion.in
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-08-15 05:20:24.000000 unstructured-0.9.3/requirements/ingest-onedrive.in
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-08-15 05:20:24.000000 unstructured-0.9.3/requirements/ingest-outlook.in
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-08-15 05:20:24.000000 unstructured-0.9.3/requirements/ingest-reddit.in
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-08-15 05:20:24.000000 unstructured-0.9.3/requirements/ingest-s3.in
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-08-15 05:20:24.000000 unstructured-0.9.3/requirements/ingest-sharepoint.in
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-08-15 05:20:24.000000 unstructured-0.9.3/requirements/ingest-slack.in
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-08-15 05:20:24.000000 unstructured-0.9.3/requirements/ingest-wikipedia.in
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-08-15 05:20:36.606748 unstructured-0.9.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     5960 2023-08-15 05:20:24.000000 unstructured-0.9.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-15 05:20:36.566748 unstructured-0.9.3/test_unstructured/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-15 05:20:24.000000 unstructured-0.9.3/test_unstructured/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-15 05:20:36.566748 unstructured-0.9.3/test_unstructured/nlp/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-15 05:20:24.000000 unstructured-0.9.3/test_unstructured/nlp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-08-15 05:20:24.000000 unstructured-0.9.3/test_unstructured/nlp/mock_nltk.py
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-08-15 05:20:24.000000 unstructured-0.9.3/test_unstructured/nlp/test_partition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2731 2023-08-15 05:20:24.000000 unstructured-0.9.3/test_unstructured/nlp/test_tokenize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-08-15 05:20:24.000000 unstructured-0.9.3/test_unstructured/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-15 05:20:36.566748 unstructured-0.9.3/unstructured/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-15 05:20:24.000000 unstructured-0.9.3/unstructured/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-08-15 05:20:24.000000 unstructured-0.9.3/unstructured/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-15 05:20:36.570748 unstructured-0.9.3/unstructured/cleaners/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-15 05:20:24.000000 unstructured-0.9.3/unstructured/cleaners/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11050 2023-08-15 05:20:24.000000 unstructured-0.9.3/unstructured/cleaners/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4209 2023-08-15 05:20:24.000000 unstructured-0.9.3/unstructured/cleaners/extract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3250 2023-08-15 05:20:24.000000 unstructured-0.9.3/unstructured/cleaners/translate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-15 05:20:36.570748 unstructured-0.9.3/unstructured/documents/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-15 05:20:24.000000 unstructured-0.9.3/unstructured/documents/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3331 2023-08-15 05:20:24.000000 unstructured-0.9.3/unstructured/documents/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3331 2023-08-15 05:20:24.000000 unstructured-0.9.3/unstructured/documents/coordinates.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16466 2023-08-15 05:20:24.000000 unstructured-0.9.3/unstructured/documents/elements.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3454 2023-08-15 05:20:24.000000 unstructured-0.9.3/unstructured/documents/email_elements.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18363 2023-08-15 05:20:24.000000 unstructured-0.9.3/unstructured/documents/html.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5301 2023-08-15 05:20:24.000000 unstructured-0.9.3/unstructured/documents/xml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-15 05:20:36.570748 unstructured-0.9.3/unstructured/file_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-15 05:20:24.000000 unstructured-0.9.3/unstructured/file_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4413 2023-08-15 05:20:24.000000 unstructured-0.9.3/unstructured/file_utils/encoding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2398 2023-08-15 05:20:24.000000 unstructured-0.9.3/unstructured/file_utils/exploration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-08-15 05:20:24.000000 unstructured-0.9.3/unstructured/file_utils/file_conversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20794 2023-08-15 05:20:24.000000 unstructured-0.9.3/unstructured/file_utils/filetype.py
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-08-15 05:20:24.000000 unstructured-0.9.3/unstructured/file_utils/google_filetype.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5420 2023-08-15 05:20:24.000000 unstructured-0.9.3/unstructured/file_utils/metadata.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-15 05:20:36.570748 unstructured-0.9.3/unstructured/ingest/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-15 05:20:24.000000 unstructured-0.9.3/unstructured/ingest/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-15 05:20:36.570748 unstructured-0.9.3/unstructured/ingest/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-15 05:20:24.000000 unstructured-0.9.3/unstructured/ingest/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      926 2023-08-15 05:20:24.000000 unstructured-0.9.3/unstructured/ingest/cli/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-15 05:20:36.574748 unstructured-0.9.3/unstructured/ingest/cli/cmds/
+-rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-08-15 05:20:24.000000 unstructured-0.9.3/unstructured/ingest/cli/cmds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2802 2023-08-15 05:20:24.000000 unstructured-0.9.3/unstructured/ingest/cli/cmds/airtable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-08-15 05:20:24.000000 unstructured-0.9.3/unstructured/ingest/cli/cmds/azure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1742 2023-08-15 05:20:24.000000 unstructured-0.9.3/unstructured/ingest/cli/cmds/biomed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-08-15 05:20:24.000000 unstructured-0.9.3/unstructured/ingest/cli/cmds/box.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2533 2023-08-15 05:20:24.000000 unstructured-0.9.3/unstructured/ingest/cli/cmds/confluence.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-08-15 05:20:24.000000 unstructured-0.9.3/unstructured/ingest/cli/cmds/discord.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-08-15 05:20:24.000000 unstructured-0.9.3/unstructured/ingest/cli/cmds/dropbox.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1656 2023-08-15 05:20:24.000000 unstructured-0.9.3/unstructured/ingest/cli/cmds/elasticsearch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-08-15 05:20:24.000000 unstructured-0.9.3/unstructured/ingest/cli/cmds/fsspec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1319 2023-08-15 05:20:24.000000 unstructured-0.9.3/unstructured/ingest/cli/cmds/gcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1796 2023-08-15 05:20:24.000000 unstructured-0.9.3/unstructured/ingest/cli/cmds/github.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-08-15 05:20:24.000000 unstructured-0.9.3/unstructured/ingest/cli/cmds/gitlab.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1410 2023-08-15 05:20:24.000000 unstructured-0.9.3/unstructured/ingest/cli/cmds/google_drive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1354 2023-08-15 05:20:24.000000 unstructured-0.9.3/unstructured/ingest/cli/cmds/local.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-08-15 05:20:24.000000 unstructured-0.9.3/unstructured/ingest/cli/cmds/notion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1784 2023-08-15 05:20:24.000000 unstructured-0.9.3/unstructured/ingest/cli/cmds/onedrive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1878 2023-08-15 05:20:24.000000 unstructured-0.9.3/unstructured/ingest/cli/cmds/outlook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2046 2023-08-15 05:20:24.000000 unstructured-0.9.3/unstructured/ingest/cli/cmds/reddit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1209 2023-08-15 05:20:24.000000 unstructured-0.9.3/unstructured/ingest/cli/cmds/s3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-08-15 05:20:24.000000 unstructured-0.9.3/unstructured/ingest/cli/cmds/sharepoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1667 2023-08-15 05:20:24.000000 unstructured-0.9.3/unstructured/ingest/cli/cmds/slack.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-08-15 05:20:24.000000 unstructured-0.9.3/unstructured/ingest/cli/cmds/wikipedia.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9951 2023-08-15 05:20:24.000000 unstructured-0.9.3/unstructured/ingest/cli/common.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-15 05:20:36.582748 unstructured-0.9.3/unstructured/ingest/connector/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-15 05:20:24.000000 unstructured-0.9.3/unstructured/ingest/connector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7477 2023-08-15 05:20:24.000000 unstructured-0.9.3/unstructured/ingest/connector/airtable.py
+-rw-r--r--   0 runner    (1001) docker     (123)      952 2023-08-15 05:20:24.000000 unstructured-0.9.3/unstructured/ingest/connector/azure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9521 2023-08-15 05:20:24.000000 unstructured-0.9.3/unstructured/ingest/connector/biomed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2618 2023-08-15 05:20:24.000000 unstructured-0.9.3/unstructured/ingest/connector/box.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6877 2023-08-15 05:20:24.000000 unstructured-0.9.3/unstructured/ingest/connector/confluence.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4534 2023-08-15 05:20:24.000000 unstructured-0.9.3/unstructured/ingest/connector/discord.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4564 2023-08-15 05:20:24.000000 unstructured-0.9.3/unstructured/ingest/connector/dropbox.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5958 2023-08-15 05:20:24.000000 unstructured-0.9.3/unstructured/ingest/connector/elasticsearch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5706 2023-08-15 05:20:24.000000 unstructured-0.9.3/unstructured/ingest/connector/fsspec.py
+-rw-r--r--   0 runner    (1001) docker     (123)      847 2023-08-15 05:20:24.000000 unstructured-0.9.3/unstructured/ingest/connector/gcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2741 2023-08-15 05:20:24.000000 unstructured-0.9.3/unstructured/ingest/connector/git.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3123 2023-08-15 05:20:24.000000 unstructured-0.9.3/unstructured/ingest/connector/github.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2296 2023-08-15 05:20:24.000000 unstructured-0.9.3/unstructured/ingest/connector/gitlab.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9598 2023-08-15 05:20:24.000000 unstructured-0.9.3/unstructured/ingest/connector/google_drive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3379 2023-08-15 05:20:24.000000 unstructured-0.9.3/unstructured/ingest/connector/local.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-15 05:20:36.582748 unstructured-0.9.3/unstructured/ingest/connector/notion/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-15 05:20:24.000000 unstructured-0.9.3/unstructured/ingest/connector/notion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3840 2023-08-15 05:20:24.000000 unstructured-0.9.3/unstructured/ingest/connector/notion/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15023 2023-08-15 05:20:24.000000 unstructured-0.9.3/unstructured/ingest/connector/notion/connector.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18419 2023-08-15 05:20:24.000000 unstructured-0.9.3/unstructured/ingest/connector/notion/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2023-08-15 05:20:24.000000 unstructured-0.9.3/unstructured/ingest/connector/notion/interfaces.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-15 05:20:36.582748 unstructured-0.9.3/unstructured/ingest/connector/notion/types/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-15 05:20:24.000000 unstructured-0.9.3/unstructured/ingest/connector/notion/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2933 2023-08-15 05:20:24.000000 unstructured-0.9.3/unstructured/ingest/connector/notion/types/block.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-15 05:20:36.586748 unstructured-0.9.3/unstructured/ingest/connector/notion/types/blocks/
+-rw-r--r--   0 runner    (1001) docker     (123)     1450 2023-08-15 05:20:24.000000 unstructured-0.9.3/unstructured/ingest/connector/notion/types/blocks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-08-15 05:20:24.000000 unstructured-0.9.3/unstructured/ingest/connector/notion/types/blocks/bookmark.py
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-08-15 05:20:24.000000 unstructured-0.9.3/unstructured/ingest/connector/notion/types/blocks/breadcrumb.py
+-rw-r--r--   0 runner    (1001) docker     (123)      971 2023-08-15 05:20:24.000000 unstructured-0.9.3/unstructured/ingest/connector/notion/types/blocks/bulleted_list_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2597 2023-08-15 05:20:24.000000 unstructured-0.9.3/unstructured/ingest/connector/notion/types/blocks/callout.py
+-rw-r--r--   0 runner    (1001) docker     (123)      533 2023-08-15 05:20:24.000000 unstructured-0.9.3/unstructured/ingest/connector/notion/types/blocks/child_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2023-08-15 05:20:24.000000 unstructured-0.9.3/unstructured/ingest/connector/notion/types/blocks/child_page.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-08-15 05:20:24.000000 unstructured-0.9.3/unstructured/ingest/connector/notion/types/blocks/code.py
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-08-15 05:20:24.000000 unstructured-0.9.3/unstructured/ingest/connector/notion/types/blocks/column_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)      565 2023-08-15 05:20:24.000000 unstructured-0.9.3/unstructured/ingest/connector/notion/types/blocks/divider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-08-15 05:20:24.000000 unstructured-0.9.3/unstructured/ingest/connector/notion/types/blocks/embed.py
+-rw-r--r--   0 runner    (1001) docker     (123)      537 2023-08-15 05:20:24.000000 unstructured-0.9.3/unstructured/ingest/connector/notion/types/blocks/equation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-08-15 05:20:24.000000 unstructured-0.9.3/unstructured/ingest/connector/notion/types/blocks/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-08-15 05:20:24.000000 unstructured-0.9.3/unstructured/ingest/connector/notion/types/blocks/heading.py
+-rw-r--r--   0 runner    (1001) docker     (123)      636 2023-08-15 05:20:24.000000 unstructured-0.9.3/unstructured/ingest/connector/notion/types/blocks/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)      580 2023-08-15 05:20:24.000000 unstructured-0.9.3/unstructured/ingest/connector/notion/types/blocks/link_preview.py
+-rw-r--r--   0 runner    (1001) docker     (123)      937 2023-08-15 05:20:24.000000 unstructured-0.9.3/unstructured/ingest/connector/notion/types/blocks/numbered_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)      970 2023-08-15 05:20:24.000000 unstructured-0.9.3/unstructured/ingest/connector/notion/types/blocks/paragraph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-08-15 05:20:24.000000 unstructured-0.9.3/unstructured/ingest/connector/notion/types/blocks/pdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-08-15 05:20:24.000000 unstructured-0.9.3/unstructured/ingest/connector/notion/types/blocks/quote.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-08-15 05:20:24.000000 unstructured-0.9.3/unstructured/ingest/connector/notion/types/blocks/synced_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-08-15 05:20:24.000000 unstructured-0.9.3/unstructured/ingest/connector/notion/types/blocks/table.py
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-08-15 05:20:24.000000 unstructured-0.9.3/unstructured/ingest/connector/notion/types/blocks/table_of_contents.py
+-rw-r--r--   0 runner    (1001) docker     (123)      946 2023-08-15 05:20:24.000000 unstructured-0.9.3/unstructured/ingest/connector/notion/types/blocks/template.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-08-15 05:20:24.000000 unstructured-0.9.3/unstructured/ingest/connector/notion/types/blocks/todo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-08-15 05:20:24.000000 unstructured-0.9.3/unstructured/ingest/connector/notion/types/blocks/toggle.py
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-08-15 05:20:24.000000 unstructured-0.9.3/unstructured/ingest/connector/notion/types/blocks/unsupported.py
+-rw-r--r--   0 runner    (1001) docker     (123)      757 2023-08-15 05:20:24.000000 unstructured-0.9.3/unstructured/ingest/connector/notion/types/blocks/video.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2514 2023-08-15 05:20:24.000000 unstructured-0.9.3/unstructured/ingest/connector/notion/types/database.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-15 05:20:36.590748 unstructured-0.9.3/unstructured/ingest/connector/notion/types/database_properties/
+-rw-r--r--   0 runner    (1001) docker     (123)     3214 2023-08-15 05:20:24.000000 unstructured-0.9.3/unstructured/ingest/connector/notion/types/database_properties/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      999 2023-08-15 05:20:24.000000 unstructured-0.9.3/unstructured/ingest/connector/notion/types/database_properties/checkbox.py
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-08-15 05:20:24.000000 unstructured-0.9.3/unstructured/ingest/connector/notion/types/database_properties/created_by.py
+-rw-r--r--   0 runner    (1001) docker     (123)      823 2023-08-15 05:20:24.000000 unstructured-0.9.3/unstructured/ingest/connector/notion/types/database_properties/created_time.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-08-15 05:20:24.000000 unstructured-0.9.3/unstructured/ingest/connector/notion/types/database_properties/date.py
+-rw-r--r--   0 runner    (1001) docker     (123)      820 2023-08-15 05:20:24.000000 unstructured-0.9.3/unstructured/ingest/connector/notion/types/database_properties/email.py
+-rw-r--r--   0 runner    (1001) docker     (123)      998 2023-08-15 05:20:24.000000 unstructured-0.9.3/unstructured/ingest/connector/notion/types/database_properties/files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-08-15 05:20:24.000000 unstructured-0.9.3/unstructured/ingest/connector/notion/types/database_properties/formula.py
+-rw-r--r--   0 runner    (1001) docker     (123)      904 2023-08-15 05:20:24.000000 unstructured-0.9.3/unstructured/ingest/connector/notion/types/database_properties/last_edited_by.py
+-rw-r--r--   0 runner    (1001) docker     (123)      853 2023-08-15 05:20:24.000000 unstructured-0.9.3/unstructured/ingest/connector/notion/types/database_properties/last_edited_time.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-08-15 05:20:24.000000 unstructured-0.9.3/unstructured/ingest/connector/notion/types/database_properties/multiselect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-08-15 05:20:24.000000 unstructured-0.9.3/unstructured/ingest/connector/notion/types/database_properties/number.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-08-15 05:20:24.000000 unstructured-0.9.3/unstructured/ingest/connector/notion/types/database_properties/people.py
+-rw-r--r--   0 runner    (1001) docker     (123)      898 2023-08-15 05:20:24.000000 unstructured-0.9.3/unstructured/ingest/connector/notion/types/database_properties/phone_number.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-08-15 05:20:24.000000 unstructured-0.9.3/unstructured/ingest/connector/notion/types/database_properties/relation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-08-15 05:20:24.000000 unstructured-0.9.3/unstructured/ingest/connector/notion/types/database_properties/rich_text.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1266 2023-08-15 05:20:24.000000 unstructured-0.9.3/unstructured/ingest/connector/notion/types/database_properties/rollup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1707 2023-08-15 05:20:24.000000 unstructured-0.9.3/unstructured/ingest/connector/notion/types/database_properties/select.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1995 2023-08-15 05:20:24.000000 unstructured-0.9.3/unstructured/ingest/connector/notion/types/database_properties/status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-08-15 05:20:24.000000 unstructured-0.9.3/unstructured/ingest/connector/notion/types/database_properties/title.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-08-15 05:20:24.000000 unstructured-0.9.3/unstructured/ingest/connector/notion/types/database_properties/unique_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)      862 2023-08-15 05:20:24.000000 unstructured-0.9.3/unstructured/ingest/connector/notion/types/database_properties/url.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2334 2023-08-15 05:20:24.000000 unstructured-0.9.3/unstructured/ingest/connector/notion/types/database_properties/verification.py
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-08-15 05:20:24.000000 unstructured-0.9.3/unstructured/ingest/connector/notion/types/date.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-08-15 05:20:24.000000 unstructured-0.9.3/unstructured/ingest/connector/notion/types/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-08-15 05:20:24.000000 unstructured-0.9.3/unstructured/ingest/connector/notion/types/page.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1695 2023-08-15 05:20:24.000000 unstructured-0.9.3/unstructured/ingest/connector/notion/types/parent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5450 2023-08-15 05:20:24.000000 unstructured-0.9.3/unstructured/ingest/connector/notion/types/rich_text.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-08-15 05:20:24.000000 unstructured-0.9.3/unstructured/ingest/connector/notion/types/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5987 2023-08-15 05:20:24.000000 unstructured-0.9.3/unstructured/ingest/connector/onedrive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8165 2023-08-15 05:20:24.000000 unstructured-0.9.3/unstructured/ingest/connector/outlook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2743 2023-08-15 05:20:24.000000 unstructured-0.9.3/unstructured/ingest/connector/reddit.py
+-rw-r--r--   0 runner    (1001) docker     (123)      837 2023-08-15 05:20:24.000000 unstructured-0.9.3/unstructured/ingest/connector/s3.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12948 2023-08-15 05:20:24.000000 unstructured-0.9.3/unstructured/ingest/connector/sharepoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5411 2023-08-15 05:20:24.000000 unstructured-0.9.3/unstructured/ingest/connector/slack.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3631 2023-08-15 05:20:24.000000 unstructured-0.9.3/unstructured/ingest/connector/wikipedia.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-15 05:20:36.590748 unstructured-0.9.3/unstructured/ingest/doc_processor/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-15 05:20:24.000000 unstructured-0.9.3/unstructured/ingest/doc_processor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-08-15 05:20:24.000000 unstructured-0.9.3/unstructured/ingest/doc_processor/generalized.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12548 2023-08-15 05:20:24.000000 unstructured-0.9.3/unstructured/ingest/interfaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)      903 2023-08-15 05:20:24.000000 unstructured-0.9.3/unstructured/ingest/logger.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      169 2023-08-15 05:20:24.000000 unstructured-0.9.3/unstructured/ingest/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3802 2023-08-15 05:20:24.000000 unstructured-0.9.3/unstructured/ingest/processor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-15 05:20:36.594748 unstructured-0.9.3/unstructured/ingest/runner/
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-08-15 05:20:24.000000 unstructured-0.9.3/unstructured/ingest/runner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-08-15 05:20:24.000000 unstructured-0.9.3/unstructured/ingest/runner/airtable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1778 2023-08-15 05:20:24.000000 unstructured-0.9.3/unstructured/ingest/runner/azure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-08-15 05:20:24.000000 unstructured-0.9.3/unstructured/ingest/runner/biomed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-08-15 05:20:24.000000 unstructured-0.9.3/unstructured/ingest/runner/box.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-08-15 05:20:24.000000 unstructured-0.9.3/unstructured/ingest/runner/confluence.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-08-15 05:20:24.000000 unstructured-0.9.3/unstructured/ingest/runner/discord.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-08-15 05:20:24.000000 unstructured-0.9.3/unstructured/ingest/runner/dropbox.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1391 2023-08-15 05:20:24.000000 unstructured-0.9.3/unstructured/ingest/runner/elasticsearch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-08-15 05:20:24.000000 unstructured-0.9.3/unstructured/ingest/runner/fsspec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-08-15 05:20:24.000000 unstructured-0.9.3/unstructured/ingest/runner/gcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1436 2023-08-15 05:20:24.000000 unstructured-0.9.3/unstructured/ingest/runner/github.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1436 2023-08-15 05:20:24.000000 unstructured-0.9.3/unstructured/ingest/runner/gitlab.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-08-15 05:20:24.000000 unstructured-0.9.3/unstructured/ingest/runner/google_drive.py
+-rw-r--r--   0 runner    (1001) docker     (123)      982 2023-08-15 05:20:24.000000 unstructured-0.9.3/unstructured/ingest/runner/local.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2073 2023-08-15 05:20:24.000000 unstructured-0.9.3/unstructured/ingest/runner/notion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1585 2023-08-15 05:20:24.000000 unstructured-0.9.3/unstructured/ingest/runner/onedrive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1702 2023-08-15 05:20:24.000000 unstructured-0.9.3/unstructured/ingest/runner/outlook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1555 2023-08-15 05:20:24.000000 unstructured-0.9.3/unstructured/ingest/runner/reddit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-08-15 05:20:24.000000 unstructured-0.9.3/unstructured/ingest/runner/s3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-08-15 05:20:24.000000 unstructured-0.9.3/unstructured/ingest/runner/sharepoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-08-15 05:20:24.000000 unstructured-0.9.3/unstructured/ingest/runner/slack.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-08-15 05:20:24.000000 unstructured-0.9.3/unstructured/ingest/runner/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-08-15 05:20:24.000000 unstructured-0.9.3/unstructured/ingest/runner/wikipedia.py
+-rw-r--r--   0 runner    (1001) docker     (123)      480 2023-08-15 05:20:24.000000 unstructured-0.9.3/unstructured/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-15 05:20:36.594748 unstructured-0.9.3/unstructured/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-15 05:20:24.000000 unstructured-0.9.3/unstructured/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-15 05:20:36.602748 unstructured-0.9.3/unstructured/nlp/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-15 05:20:24.000000 unstructured-0.9.3/unstructured/nlp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)  4472047 2023-08-15 05:20:24.000000 unstructured-0.9.3/unstructured/nlp/english-words.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-08-15 05:20:24.000000 unstructured-0.9.3/unstructured/nlp/english_words.py
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-08-15 05:20:24.000000 unstructured-0.9.3/unstructured/nlp/partition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5550 2023-08-15 05:20:24.000000 unstructured-0.9.3/unstructured/nlp/patterns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2090 2023-08-15 05:20:24.000000 unstructured-0.9.3/unstructured/nlp/tokenize.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-15 05:20:36.606748 unstructured-0.9.3/unstructured/partition/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-15 05:20:24.000000 unstructured-0.9.3/unstructured/partition/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6619 2023-08-15 05:20:24.000000 unstructured-0.9.3/unstructured/partition/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12503 2023-08-15 05:20:24.000000 unstructured-0.9.3/unstructured/partition/auto.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11236 2023-08-15 05:20:24.000000 unstructured-0.9.3/unstructured/partition/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2273 2023-08-15 05:20:24.000000 unstructured-0.9.3/unstructured/partition/csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3046 2023-08-15 05:20:24.000000 unstructured-0.9.3/unstructured/partition/doc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13938 2023-08-15 05:20:24.000000 unstructured-0.9.3/unstructured/partition/docx.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15400 2023-08-15 05:20:24.000000 unstructured-0.9.3/unstructured/partition/email.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3331 2023-08-15 05:20:24.000000 unstructured-0.9.3/unstructured/partition/epub.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6562 2023-08-15 05:20:24.000000 unstructured-0.9.3/unstructured/partition/html.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2370 2023-08-15 05:20:24.000000 unstructured-0.9.3/unstructured/partition/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2527 2023-08-15 05:20:24.000000 unstructured-0.9.3/unstructured/partition/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3174 2023-08-15 05:20:24.000000 unstructured-0.9.3/unstructured/partition/md.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5813 2023-08-15 05:20:24.000000 unstructured-0.9.3/unstructured/partition/msg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-08-15 05:20:24.000000 unstructured-0.9.3/unstructured/partition/odt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-08-15 05:20:24.000000 unstructured-0.9.3/unstructured/partition/org.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17794 2023-08-15 05:20:24.000000 unstructured-0.9.3/unstructured/partition/pdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2795 2023-08-15 05:20:24.000000 unstructured-0.9.3/unstructured/partition/ppt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5907 2023-08-15 05:20:24.000000 unstructured-0.9.3/unstructured/partition/pptx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-08-15 05:20:24.000000 unstructured-0.9.3/unstructured/partition/rst.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-08-15 05:20:24.000000 unstructured-0.9.3/unstructured/partition/rtf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4781 2023-08-15 05:20:24.000000 unstructured-0.9.3/unstructured/partition/strategies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9318 2023-08-15 05:20:24.000000 unstructured-0.9.3/unstructured/partition/text.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11494 2023-08-15 05:20:24.000000 unstructured-0.9.3/unstructured/partition/text_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2214 2023-08-15 05:20:24.000000 unstructured-0.9.3/unstructured/partition/tsv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2570 2023-08-15 05:20:24.000000 unstructured-0.9.3/unstructured/partition/xlsx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4163 2023-08-15 05:20:24.000000 unstructured-0.9.3/unstructured/partition/xml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-15 05:20:36.606748 unstructured-0.9.3/unstructured/staging/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-15 05:20:24.000000 unstructured-0.9.3/unstructured/staging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2288 2023-08-15 05:20:24.000000 unstructured-0.9.3/unstructured/staging/argilla.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6958 2023-08-15 05:20:24.000000 unstructured-0.9.3/unstructured/staging/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1755 2023-08-15 05:20:24.000000 unstructured-0.9.3/unstructured/staging/baseplate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-08-15 05:20:24.000000 unstructured-0.9.3/unstructured/staging/datasaur.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3838 2023-08-15 05:20:24.000000 unstructured-0.9.3/unstructured/staging/huggingface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3916 2023-08-15 05:20:24.000000 unstructured-0.9.3/unstructured/staging/label_box.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4904 2023-08-15 05:20:24.000000 unstructured-0.9.3/unstructured/staging/label_studio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3188 2023-08-15 05:20:24.000000 unstructured-0.9.3/unstructured/staging/prodigy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2534 2023-08-15 05:20:24.000000 unstructured-0.9.3/unstructured/staging/weaviate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2311 2023-08-15 05:20:24.000000 unstructured-0.9.3/unstructured/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-15 05:20:36.570748 unstructured-0.9.3/unstructured.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    20208 2023-08-15 05:20:36.000000 unstructured-0.9.3/unstructured.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10561 2023-08-15 05:20:36.000000 unstructured-0.9.3/unstructured.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-15 05:20:36.000000 unstructured-0.9.3/unstructured.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-08-15 05:20:36.000000 unstructured-0.9.3/unstructured.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-08-15 05:20:36.000000 unstructured-0.9.3/unstructured.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-08-15 05:20:36.000000 unstructured-0.9.3/unstructured.egg-info/top_level.txt
```

### Comparing `unstructured-0.9.2/LICENSE.md` & `unstructured-0.9.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `unstructured-0.9.2/MANIFEST.in` & `unstructured-0.9.3/MANIFEST.in`

 * *Files 11% similar despite different names*

```diff
@@ -1,17 +1,21 @@
 include requirements/base.in
 include requirements/huggingface.in
-include requirements/local-inference.in
 include requirements/ingest-s3.in
-include requirements/ingest-gcs.in
-include requirements/ingest-dropbox.in
 include requirements/ingest-azure.in
 include requirements/ingest-discord.in
 include requirements/ingest-github.in
 include requirements/ingest-gitlab.in
 include requirements/ingest-reddit.in
+include requirements/ingest-notion.in
 include requirements/ingest-slack.in
 include requirements/ingest-wikipedia.in
 include requirements/ingest-google-drive.in
-include requirements/ingest-outlook.in
-include requirements/ingest-onedrive.in
+include requirements/ingest-gcs.in
+include requirements/ingest-elasticsearch.in
+include requirements/ingest-dropbox.in
 include requirements/ingest-box.in
+include requirements/ingest-onedrive.in
+include requirements/ingest-outlook.in
+include requirements/ingest-confluence.in
+include requirements/ingest-airtable.in
+include requirements/ingest-sharepoint.in
```

### Comparing `unstructured-0.9.2/PKG-INFO` & `unstructured-0.9.3/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unstructured
-Version: 0.9.2
+Version: 0.9.3
 Summary: A library that prepares raw documents for downstream ML tasks.
 Home-page: https://github.com/Unstructured-IO/unstructured
 Author: Unstructured Technologies
 Author-email: devops@unstructuredai.io
 License: Apache-2.0
 Description: <h3 align="center">
           <img
@@ -33,57 +33,44 @@
             <img src="https://img.shields.io/badge/JOIN US ON SLACK-4A154B?style=for-the-badge&logo=slack&logoColor=white" />
           </a>
           <a href="https://www.linkedin.com/company/unstructuredio/">
             <img src="https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white" />
           </a>
         </div>
         
+        <h2 align="center">
+          <p>Open-Source Pre-Processing Tools for Unstructured Data</p>
+        </h2>
+        
+        The `unstructured` library provides open-source components for ingesting and pre-processing images and text documents, such as PDFs, HTML, Word docs, and [many more](https://unstructured-io.github.io/unstructured/bricks.html#partitioning). The use cases of `unstructured` revolve around streamlining and optimizing the data processing workflow for LLMs. `unstructured` modular bricks and connectors form a cohesive system that simplifies data ingestion and pre-processing, making it adaptable to different platforms and is efficient in transforming unstructured data into structured outputs.
+        
         <h3 align="center">
           <p>API Announcement!</p>
         </h3>
         
-        We are thrilled to announce our newly launched [Unstructured API](https://unstructured-io.github.io/unstructured/api.html). While access to the hosted Unstructured API will remain free, API Keys are required to make requests. To prevent disruption, get yours [here](https://unstructured.io/#get-api-key) now and start using it today! Check out the [readme](https://github.com/Unstructured-IO/unstructured-api#--) here to get started making API calls.</p>
+        We are thrilled to announce our newly launched [Unstructured API](https://unstructured-io.github.io/unstructured/api.html), providing the Unstructured capabilities from `unstructured` as an API. Check out the [`unstructured-api` GitHub repository](https://github.com/Unstructured-IO/unstructured-api) to start making API calls. You’ll also find instructions about how to host your own API version.
+        
+        While access to the hosted Unstructured API will remain free, API Keys are required to make requests. To prevent disruption, get yours [here](https://unstructured.io/#get-api-key) and start using it today! Check out the [`unstructured-api` README](https://github.com/Unstructured-IO/unstructured-api#--) to start making API calls.</p>
         
         #### :rocket: Beta Feature: Chipper Model
         
-        We are releasing the beta version of our Chipper model to deliver superior performance when processing high-resolution, complex documents. To start using the Chipper model in your API request, you can utilize the `hi_res` strategy. Please refer to the documentation [here](https://unstructured-io.github.io/unstructured/api.html#strategies).
+        We are releasing the beta version of our Chipper model to deliver superior performance when processing high-resolution, complex documents. To start using the Chipper model in your API request, you can utilize the `hi_res_model_name=chipper` parameter. Please refer to the documentation [here](https://unstructured-io.github.io/unstructured/api.html#beta-version-hi-res-strategy-with-chipper-model).
         
         As the Chipper model is in beta version, we welcome feedback and suggestions. For those interested in testing the Chipper model, we encourage you to connect with us on [Slack community](https://join.slack.com/t/unstructuredw-kbe4326/shared_invite/zt-1x7cgo0pg-PTptXWylzPQF9xZolzCnwQ).
         
-        <h3 align="center">
-          <p>Open-Source Pre-Processing Tools for Unstructured Data</p>
-        </h3>
-        
-        The `unstructured` library provides open-source components for pre-processing text documents
-        such as **PDFs**, **HTML** and **Word** Documents. These components are packaged as *bricks* 🧱, which provide
-        users the building blocks they need to build pipelines targeted at the documents they care
-        about. Bricks in the library fall into three categories:
-        
-        - :jigsaw: ***Partitioning bricks*** that break raw documents down into standard, structured
-          elements.
-        - :broom: ***Cleaning bricks*** that remove unwanted text from documents, such as boilerplate and
-          sentence
-          fragments.
-        - :performing_arts: ***Staging bricks*** that format data for downstream tasks, such as ML inference
-          and data labeling.
-        
-        Unstructured also provides the capabilities from `unstructured` as an API.
-        Checkout the [`unstructured-api` repo](https://github.com/Unstructured-IO/unstructured-api)
-        to get started making API calls.
-        You’ll also find instructions there about how to host your own version of the API.
-        
-        ## :bookmark: Documentation
-        This README gives an overview of how to install, use and develop the library.
-        For more comprehensive documentation, visit https://unstructured-io.github.io/unstructured/ .
-        
         ## :eight_pointed_black_star: Quick Start
         
-        There are two ways to use the library: 1) run a container or 2) install it
+        There are several ways to use the `unstructured` library:
+        * [Run the library in a container](https://github.com/Unstructured-IO/unstructured#using-the-library-in-a-container) or
+        * Install the library
+            1. [Install from PyPI](https://github.com/Unstructured-IO/unstructured#installing-the-library)
+            2. [Install for local development](https://github.com/Unstructured-IO/unstructured#coffee-installation-instructions-for-local-development)
+        * For installation with `conda` on Windows system, please refer to the [documentation](https://unstructured-io.github.io/unstructured/installing.html#installation-with-conda-on-windows)
         
-        ### Using the library in a container
+        ### Run the library in a container
         
         The following instructions are intended to help you get up and running using Docker to interact with `unstructured`.
         See [here](https://docs.docker.com/get-docker/) if you don't already have docker installed on your machine.
         
         NOTE: we build multi-platform images to support both x86_64 and Apple silicon hardware. `docker pull` should download the corresponding image for your architecture, but you can specify with `--platform` (e.g. `--platform linux/amd64`) if needed.
         
         We build Docker images for all pushes to `main`. We tag each image with the corresponding short commit hash (e.g. `fbc7a69`) and the application version (e.g. `0.5.5-dev1`). We also tag the most recent image with `latest`. To leverage this, `docker pull` from our image repository.
@@ -111,15 +98,15 @@
         ```bash
         make docker-build
         
         # this will drop you into a bash shell where the Docker image is running
         make docker-start-bash
         ```
         
-        Once in the running container, you can try things out directly in Python interpreter's interactive mode.
+        Once in the running container, you can try things directly in Python interpreter's interactive mode.
         ```bash
         # this will drop you into a python console so you can run the below partition functions
         python3
         
         >>> from unstructured.partition.pdf import partition_pdf
         >>> elements = partition_pdf(filename="example-docs/layout-parser-paper-fast.pdf")
         
@@ -127,69 +114,38 @@
         >>> elements = partition_text(filename="example-docs/fake-text.txt")
         ```
         
         ### Installing the library
         Use the following instructions to get up and running with `unstructured` and test your
         installation.
         
-        - Install the Python SDK with `pip install "unstructured[local-inference]"`
-        		- If you do not need to process PDFs or images, you can run `pip install unstructured`
+        - Install the Python SDK to support all document types with `pip install "unstructured[all-docs]"`
+          - For plain text files, HTML, XML, JSON and Emails that do not require any extra dependencies, you can run `pip install unstructured`
+          - To process other doc types, you can install the extras required for those documents, such as `pip install "unstructured[docx,pptx]"`
         - Install the following system dependencies if they are not already available on your system.
           Depending on what document types you're parsing, you may not need all of these.
             - `libmagic-dev` (filetype detection)
             - `poppler-utils` (images and PDFs)
             - `tesseract-ocr` (images and PDFs)
             - `libreoffice` (MS Office docs)
             - `pandoc` (EPUBs, RTFs and Open Office docs)
         
-        - For suggestions on how to install on Windows and to learn about dependencies for other features, see the
+        - For suggestions on how to install on the Windows and to learn about dependencies for other features, see the
           installation documentation [here](https://unstructured-io.github.io/unstructured/installing.html).
         
         At this point, you should be able to run the following code:
         
         ```python
         from unstructured.partition.auto import partition
         
         elements = partition(filename="example-docs/eml/fake-email.eml")
         print("\n\n".join([str(el) for el in elements]))
         ```
         
-        The following table shows the document types the `unstructured` library currently supports.
-        `partition` will recognize each of these document types and route the document to the
-        appropriate partitioning function. If you already know your document type, you can use
-        the partitioning function listed in the table directly.
-        See our [documentation page](https://unstructured-io.github.io/unstructured/) for more details
-        about the library.
-        
-        | Document Type | Partition Function | Strategies | Table Support | Options |
-        | --- | --- | --- | --- | --- |
-        | CSV Files (`.csv`) | `partition_csv` | N/A | Yes | None |
-        | E-mails (`.eml`) | `partition_eml` | N/A | No | Encoding; Max Partition; Process Attachments |
-        | E-mails (`.msg`) | `partition_msg` | N/A | No | Encoding; Max Partition; Process Attachments |
-        | EPubs (`.epub`) | `partition_epub` | N/A | Yes | Include Page Breaks |
-        | Excel Documents (`.xlsx`/`.xls`) | `partition_xlsx` | N/A | Yes | None |
-        | HTML Pages (`.html`) | `partition_html` | N/A | No | Encoding; Include Page Breaks |
-        | Images (`.png`/`.jpg`) | `partition_image` | `"auto"`, `"hi_res"`, `"ocr_only"` | Yes | Encoding; Include Page Breaks; Infer Table Structure; OCR Languages, Strategy |
-        | Markdown (`.md`) | `partitin_md` | N/A | Yes | Include Page Breaks |
-        | Org Mode (`.org`) | `partition_org` | N/A | Yes | Include Page Breaks |
-        | Open Office Documents (`.odt`) | `partition_odt` | N/A | Yes | None |
-        | PDFs (`.pdf`) | `partition_pdf` | `"auto"`, `"fast"`, `"hi_res"`, `"ocr_only"` | Yes | Encoding; Include Page Breaks; Infer Table Structure; Max Partition; OCR Languages, Strategy |
-        | Plain Text (`.txt`) | `partition_text` | N/A | No | Encoding; Max Partition; Paragraph Grouper |
-        | Power Points (`.ppt`) | `partition_ppt` | N/A | Yes | Include Page Breaks |
-        | Power Points (`.pptx`) | `partition_pptx` | N/A | Yes | Include Page Breaks |
-        | ReStructured Text (`.rst`) | `partition_rst` | N/A | Yes | Include Page Breaks |
-        | Rich Text Files (`.rtf`) | `partition_rtf` | N/A | Yes | Include Page Breaks |
-        | TSV Files (`.tsv`) | `partition_tsv` | N/A | Yes | None |
-        | Word Documents (`.doc`) | `partition_doc` | N/A | Yes | Include Page Breaks |
-        | Word Documents (`.docx`) | `partition_docx` | N/A | Yes | Include Page Breaks |
-        | XML Documents (`.xml`) | `partition_xml` | N/A | No | Encoding; Max Partition; XML Keep Tags |
-        
-        
-        
-        ## :coffee: Installation Instructions for Local Development
+        ### Installation Instructions for Local Development
         
         The following instructions are intended to help you get up and running with `unstructured`
         locally if you are planning to contribute to the project.
         
         * Using `pyenv` to manage virtualenv's is recommended but not necessary
         	* Mac install instructions. See [here](https://github.com/Unstructured-IO/community#mac--homebrew) for more detailed instructions.
         		* `brew install pyenv-virtualenv`
@@ -206,41 +162,41 @@
         * Optional:
           * To install models and dependencies for processing images and PDFs locally, run `make install-local-inference`.
           * For processing image files, `tesseract` is required. See [here](https://tesseract-ocr.github.io/tessdoc/Installation.html) for installation instructions.
           * For processing PDF files, `tesseract` and `poppler` are required. The [pdf2image docs](https://pdf2image.readthedocs.io/en/latest/installation.html) have instructions on installing `poppler` across various platforms.
         
         Additionally, if you're planning to contribute to `unstructured`, we provide you an optional `pre-commit` configuration
         file to ensure your code matches the formatting and linting standards used in `unstructured`.
-        If you'd prefer not having code changes auto-tidied before every commit, you can use  `make check` to see
+        If you'd prefer not to have code changes auto-tidied before every commit, you can use  `make check` to see
         whether any linting or formatting changes should be applied, and `make tidy` to apply them.
         
         If using the optional `pre-commit`, you'll just need to install the hooks with `pre-commit install` since the
         `pre-commit` package is installed as part of `make install` mentioned above. Finally, if you decided to use `pre-commit`
         you can also uninstall the hooks with `pre-commit uninstall`.
         
         ## :clap: Quick Tour
         
-        You can run this [Colab notebook](https://colab.research.google.com/drive/1U8VCjY2-x8c6y5TYMbSFtQGlQVFHCVIW) to run the examples below.
+        ### Documentation
+        This README overviews how to install, use and develop the library. For more comprehensive documentation, visit https://unstructured-io.github.io/unstructured/ .
+        
+        ### Concepts Guide
+        
+        **Bricks** 🧱 in `unstructured` are the foundational elements that drive the data processing workflow within the system. These components provide users with the building blocks to build pipelines targeted at the documents they care about. The bricks fall into three categories:
+        - :jigsaw: *Partitioning* bricks break raw documents into standard, structured elements.
+        - :broom: *Cleaning* bricks remove unwanted text from documents, such as boilerplate and sentence fragments.
+        - :performing_arts: *Staging* bricks format data for downstream tasks, such as ML inference and data labeling. 
+        
+        These bricks create a cohesive, streamlined process that enables effective data handling and analysis. Check out the available bricks and how to use them from the [Bricks documentation](https://unstructured-io.github.io/unstructured/bricks.html).
+        
+        The **Connectors** 🔗 in `unstructured` serve as vital links between the pre-processing pipeline and various data storage platforms. They allow for the batch processing of documents across various sources, including cloud services, repositories, and local directories. Each connector is tailored to a specific platform, such as Azure, Google Drive, or Github, and comes with unique commands and dependencies. To see the list of Connectors available in `unstructured` library, please check out the [Connectors GitHub folder](https://github.com/Unstructured-IO/unstructured/tree/main/unstructured/ingest/connector) and [documentation](https://unstructured-io.github.io/unstructured/connectors.html)
+        
+        ### PDF Document Parsing Example
+        The following examples show how to get started with the `unstructured` library. You can parse over a dozen document types with one line of code! Use this [Colab notebook](https://colab.research.google.com/drive/1U8VCjY2-x8c6y5TYMbSFtQGlQVFHCVIW) to run the example below.
         
-        The following examples show how to get started with the `unstructured` library.
-        You can parse over a dozen document types with one line of code!
-        <br></br>
-        See our [documentation page](https://unstructured-io.github.io/unstructured) for a full description
-        of the features in the library.
-        
-        ### Document Parsing
-        
-        The easiest way to parse a document in unstructured is to use the `partition` brick. If you
-        use `partition` brick, `unstructured` will detect the file type and route it to the appropriate
-        file-specific partitioning brick.
-        If you are using the `partition` brick, you may need to install additional parameters via `pip install unstructured[local-inference]`. Ensure you first install `libmagic` using the
-        instructions outlined [here](https://unstructured-io.github.io/unstructured/installing.html#filetype-detection)
-        `partition` will always apply the default arguments. If you need
-        advanced features, use a document-specific brick.
-        See the table above for a full list of document types supported in the library.
+        The easiest way to parse a document in unstructured is to use the `partition` brick. If you use `partition` brick, `unstructured` will detect the file type and route it to the appropriate file-specific partitioning brick. If you are using the `partition` brick, you may need to install additional parameters via `pip install unstructured[local-inference]`. Ensure you first install `libmagic` using the instructions outlined [here](https://unstructured-io.github.io/unstructured/installing.html#filetype-detection) `partition` will always apply the default arguments. If you need advanced features, use a document-specific brick.
         
         ```python
         from unstructured.partition.auto import partition
         
         elements = partition("example-docs/layout-parser-paper.pdf")
         ```
         
@@ -342,9 +298,11 @@
 Provides-Extra: gcs
 Provides-Extra: elasticsearch
 Provides-Extra: dropbox
 Provides-Extra: box
 Provides-Extra: onedrive
 Provides-Extra: outlook
 Provides-Extra: confluence
+Provides-Extra: airtable
+Provides-Extra: sharepoint
 Provides-Extra: huggingface
 Provides-Extra: local-inference
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: unstructured Version: 0.9.2 Summary: A library that
+Metadata-Version: 2.1 Name: unstructured Version: 0.9.3 Summary: A library that
 prepares raw documents for downstream ML tasks. Home-page: https://github.com/
 Unstructured-IO/unstructured Author: Unstructured Technologies Author-email:
 devops@unstructuredai.io License: Apache-2.0 Description:
 ******** [[hhttttppss::////rraaww..ggiitthhuubbuusseerrccoonntteenntt..ccoomm//UUnnssttrruuccttuurreedd--IIOO//uunnssttrruuccttuurreedd//mmaaiinn//iimmgg//
                           uunnssttrruuccttuurreedd__llooggoo..ppnngg]] ********
  _!_[_h_t_t_p_s_:_/_/_p_y_p_i_._p_y_t_h_o_n_._o_r_g_/_p_y_p_i_/_u_n_s_t_r_u_c_t_u_r_e_d_/_]_(_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_p_y_p_i_/_l_/
    _u_n_s_t_r_u_c_t_u_r_e_d_._s_v_g_) _!_[_h_t_t_p_s_:_/_/_p_y_p_i_._p_y_t_h_o_n_._o_r_g_/_p_y_p_i_/_u_n_s_t_r_u_c_t_u_r_e_d_/_]_(_h_t_t_p_s_:_/_/
@@ -15,192 +15,188 @@
 _b_a_d_g_e_s_/_]_(_h_t_t_p_s_:_/_/_b_a_d_g_e_n_._n_e_t_/_b_a_d_g_e_/_O_p_e_n_%_2_0_S_o_u_r_c_e_%_2_0_%_3_F_/_Y_e_s_%_2_1_/_b_l_u_e_?_i_c_o_n_=_g_i_t_h_u_b_)
 [![Downloads](https://static.pepy.tech/badge/unstructured)](https://pepy.tech/
       project/unstructured) [![Downloads](https://static.pepy.tech/badge/
          unstructured/month)](https://pepy.tech/project/unstructured)
      _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_J_O_I_N_ _U_S_ _O_N_ _S_L_A_C_K_-_4_A_1_5_4_B_?_s_t_y_l_e_=_f_o_r_-_t_h_e_-
    _b_a_d_g_e_&_l_o_g_o_=_s_l_a_c_k_&_l_o_g_o_C_o_l_o_r_=_w_h_i_t_e_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_L_i_n_k_e_d_I_n_-
            _0_0_7_7_B_5_?_s_t_y_l_e_=_f_o_r_-_t_h_e_-_b_a_d_g_e_&_l_o_g_o_=_l_i_n_k_e_d_i_n_&_l_o_g_o_C_o_l_o_r_=_w_h_i_t_e_]
+      ********** OOppeenn--SSoouurrccee PPrree--PPrroocceessssiinngg TToooollss ffoorr UUnnssttrruuccttuurreedd DDaattaa **********
+The `unstructured` library provides open-source components for ingesting and
+pre-processing images and text documents, such as PDFs, HTML, Word docs, and
+[many more](https://unstructured-io.github.io/unstructured/
+bricks.html#partitioning). The use cases of `unstructured` revolve around
+streamlining and optimizing the data processing workflow for LLMs.
+`unstructured` modular bricks and connectors form a cohesive system that
+simplifies data ingestion and pre-processing, making it adaptable to different
+platforms and is efficient in transforming unstructured data into structured
+outputs.
                           ******** AAPPII AAnnnnoouunncceemmeenntt!! ********
 We are thrilled to announce our newly launched [Unstructured API](https://
-unstructured-io.github.io/unstructured/api.html). While access to the hosted
-Unstructured API will remain free, API Keys are required to make requests. To
-prevent disruption, get yours [here](https://unstructured.io/#get-api-key) now
-and start using it today! Check out the [readme](https://github.com/
-Unstructured-IO/unstructured-api#--) here to get started making API calls.
+unstructured-io.github.io/unstructured/api.html), providing the Unstructured
+capabilities from `unstructured` as an API. Check out the [`unstructured-api`
+GitHub repository](https://github.com/Unstructured-IO/unstructured-api) to
+start making API calls. Youâll also find instructions about how to host your
+own API version. While access to the hosted Unstructured API will remain free,
+API Keys are required to make requests. To prevent disruption, get yours [here]
+(https://unstructured.io/#get-api-key) and start using it today! Check out the
+[`unstructured-api` README](https://github.com/Unstructured-IO/unstructured-
+api#--) to start making API calls.
 #### :rocket: Beta Feature: Chipper Model We are releasing the beta version of
 our Chipper model to deliver superior performance when processing high-
 resolution, complex documents. To start using the Chipper model in your API
-request, you can utilize the `hi_res` strategy. Please refer to the
-documentation [here](https://unstructured-io.github.io/unstructured/
-api.html#strategies). As the Chipper model is in beta version, we welcome
-feedback and suggestions. For those interested in testing the Chipper model, we
-encourage you to connect with us on [Slack community](https://join.slack.com/t/
-unstructuredw-kbe4326/shared_invite/zt-1x7cgo0pg-PTptXWylzPQF9xZolzCnwQ).
-       ******** OOppeenn--SSoouurrccee PPrree--PPrroocceessssiinngg TToooollss ffoorr UUnnssttrruuccttuurreedd DDaattaa ********
-The `unstructured` library provides open-source components for pre-processing
-text documents such as **PDFs**, **HTML** and **Word** Documents. These
-components are packaged as *bricks* ð§±, which provide users the building
-blocks they need to build pipelines targeted at the documents they care about.
-Bricks in the library fall into three categories: - :jigsaw: ***Partitioning
-bricks*** that break raw documents down into standard, structured elements. - :
-broom: ***Cleaning bricks*** that remove unwanted text from documents, such as
-boilerplate and sentence fragments. - :performing_arts: ***Staging bricks***
-that format data for downstream tasks, such as ML inference and data labeling.
-Unstructured also provides the capabilities from `unstructured` as an API.
-Checkout the [`unstructured-api` repo](https://github.com/Unstructured-IO/
-unstructured-api) to get started making API calls. Youâll also find
-instructions there about how to host your own version of the API. ## :bookmark:
-Documentation This README gives an overview of how to install, use and develop
-the library. For more comprehensive documentation, visit https://unstructured-
-io.github.io/unstructured/ . ## :eight_pointed_black_star: Quick Start There
-are two ways to use the library: 1) run a container or 2) install it ### Using
-the library in a container The following instructions are intended to help you
-get up and running using Docker to interact with `unstructured`. See [here]
-(https://docs.docker.com/get-docker/) if you don't already have docker
-installed on your machine. NOTE: we build multi-platform images to support both
-x86_64 and Apple silicon hardware. `docker pull` should download the
-corresponding image for your architecture, but you can specify with `--
-platform` (e.g. `--platform linux/amd64`) if needed. We build Docker images for
-all pushes to `main`. We tag each image with the corresponding short commit
-hash (e.g. `fbc7a69`) and the application version (e.g. `0.5.5-dev1`). We also
-tag the most recent image with `latest`. To leverage this, `docker pull` from
-our image repository. ```bash docker pull quay.io/unstructured-io/unstructured:
-latest ``` Once pulled, you can create a container from this image and shell to
-it. ```bash # create the container docker run -dt --name unstructured quay.io/
-unstructured-io/unstructured:latest # this will drop you into a bash shell
-where the Docker image is running docker exec -it unstructured bash ``` You can
-also build your own Docker image. If you only plan on parsing one type of data
-you can speed up building the image by commenting out some of the packages/
-requirements necessary for other data types. See Dockerfile to know which lines
-are necessary for your use case. ```bash make docker-build # this will drop you
+request, you can utilize the `hi_res_model_name=chipper` parameter. Please
+refer to the documentation [here](https://unstructured-io.github.io/
+unstructured/api.html#beta-version-hi-res-strategy-with-chipper-model). As the
+Chipper model is in beta version, we welcome feedback and suggestions. For
+those interested in testing the Chipper model, we encourage you to connect with
+us on [Slack community](https://join.slack.com/t/unstructuredw-kbe4326/
+shared_invite/zt-1x7cgo0pg-PTptXWylzPQF9xZolzCnwQ). ## :
+eight_pointed_black_star: Quick Start There are several ways to use the
+`unstructured` library: * [Run the library in a container](https://github.com/
+Unstructured-IO/unstructured#using-the-library-in-a-container) or * Install the
+library 1. [Install from PyPI](https://github.com/Unstructured-IO/
+unstructured#installing-the-library) 2. [Install for local development](https:/
+/github.com/Unstructured-IO/unstructured#coffee-installation-instructions-for-
+local-development) * For installation with `conda` on Windows system, please
+refer to the [documentation](https://unstructured-io.github.io/unstructured/
+installing.html#installation-with-conda-on-windows) ### Run the library in a
+container The following instructions are intended to help you get up and
+running using Docker to interact with `unstructured`. See [here](https://
+docs.docker.com/get-docker/) if you don't already have docker installed on your
+machine. NOTE: we build multi-platform images to support both x86_64 and Apple
+silicon hardware. `docker pull` should download the corresponding image for
+your architecture, but you can specify with `--platform` (e.g. `--platform
+linux/amd64`) if needed. We build Docker images for all pushes to `main`. We
+tag each image with the corresponding short commit hash (e.g. `fbc7a69`) and
+the application version (e.g. `0.5.5-dev1`). We also tag the most recent image
+with `latest`. To leverage this, `docker pull` from our image repository.
+```bash docker pull quay.io/unstructured-io/unstructured:latest ``` Once
+pulled, you can create a container from this image and shell to it. ```bash #
+create the container docker run -dt --name unstructured quay.io/unstructured-
+io/unstructured:latest # this will drop you into a bash shell where the Docker
+image is running docker exec -it unstructured bash ``` You can also build your
+own Docker image. If you only plan on parsing one type of data you can speed up
+building the image by commenting out some of the packages/requirements
+necessary for other data types. See Dockerfile to know which lines are
+necessary for your use case. ```bash make docker-build # this will drop you
 into a bash shell where the Docker image is running make docker-start-bash ```
-Once in the running container, you can try things out directly in Python
+Once in the running container, you can try things directly in Python
 interpreter's interactive mode. ```bash # this will drop you into a python
 console so you can run the below partition functions python3 >>> from
 unstructured.partition.pdf import partition_pdf >>> elements = partition_pdf
 (filename="example-docs/layout-parser-paper-fast.pdf") >>> from
 unstructured.partition.text import partition_text >>> elements = partition_text
 (filename="example-docs/fake-text.txt") ``` ### Installing the library Use the
 following instructions to get up and running with `unstructured` and test your
-installation. - Install the Python SDK with `pip install "unstructured[local-
-inference]"` - If you do not need to process PDFs or images, you can run `pip
-install unstructured` - Install the following system dependencies if they are
-not already available on your system. Depending on what document types you're
-parsing, you may not need all of these. - `libmagic-dev` (filetype detection) -
-`poppler-utils` (images and PDFs) - `tesseract-ocr` (images and PDFs) -
-`libreoffice` (MS Office docs) - `pandoc` (EPUBs, RTFs and Open Office docs) -
-For suggestions on how to install on Windows and to learn about dependencies
-for other features, see the installation documentation [here](https://
-unstructured-io.github.io/unstructured/installing.html). At this point, you
-should be able to run the following code: ```python from
-unstructured.partition.auto import partition elements = partition
-(filename="example-docs/eml/fake-email.eml") print("\n\n".join([str(el) for el
-in elements])) ``` The following table shows the document types the
-`unstructured` library currently supports. `partition` will recognize each of
-these document types and route the document to the appropriate partitioning
-function. If you already know your document type, you can use the partitioning
-function listed in the table directly. See our [documentation page](https://
-unstructured-io.github.io/unstructured/) for more details about the library. |
-Document Type | Partition Function | Strategies | Table Support | Options | | -
--- | --- | --- | --- | --- | | CSV Files (`.csv`) | `partition_csv` | N/A | Yes
-| None | | E-mails (`.eml`) | `partition_eml` | N/A | No | Encoding; Max
-Partition; Process Attachments | | E-mails (`.msg`) | `partition_msg` | N/A |
-No | Encoding; Max Partition; Process Attachments | | EPubs (`.epub`) |
-`partition_epub` | N/A | Yes | Include Page Breaks | | Excel Documents
-(`.xlsx`/`.xls`) | `partition_xlsx` | N/A | Yes | None | | HTML Pages (`.html`)
-| `partition_html` | N/A | No | Encoding; Include Page Breaks | | Images
-(`.png`/`.jpg`) | `partition_image` | `"auto"`, `"hi_res"`, `"ocr_only"` | Yes
-| Encoding; Include Page Breaks; Infer Table Structure; OCR Languages, Strategy
-| | Markdown (`.md`) | `partitin_md` | N/A | Yes | Include Page Breaks | | Org
-Mode (`.org`) | `partition_org` | N/A | Yes | Include Page Breaks | | Open
-Office Documents (`.odt`) | `partition_odt` | N/A | Yes | None | | PDFs
-(`.pdf`) | `partition_pdf` | `"auto"`, `"fast"`, `"hi_res"`, `"ocr_only"` | Yes
-| Encoding; Include Page Breaks; Infer Table Structure; Max Partition; OCR
-Languages, Strategy | | Plain Text (`.txt`) | `partition_text` | N/A | No |
-Encoding; Max Partition; Paragraph Grouper | | Power Points (`.ppt`) |
-`partition_ppt` | N/A | Yes | Include Page Breaks | | Power Points (`.pptx`) |
-`partition_pptx` | N/A | Yes | Include Page Breaks | | ReStructured Text
-(`.rst`) | `partition_rst` | N/A | Yes | Include Page Breaks | | Rich Text
-Files (`.rtf`) | `partition_rtf` | N/A | Yes | Include Page Breaks | | TSV
-Files (`.tsv`) | `partition_tsv` | N/A | Yes | None | | Word Documents (`.doc`)
-| `partition_doc` | N/A | Yes | Include Page Breaks | | Word Documents
-(`.docx`) | `partition_docx` | N/A | Yes | Include Page Breaks | | XML
-Documents (`.xml`) | `partition_xml` | N/A | No | Encoding; Max Partition; XML
-Keep Tags | ## :coffee: Installation Instructions for Local Development The
-following instructions are intended to help you get up and running with
-`unstructured` locally if you are planning to contribute to the project. *
-Using `pyenv` to manage virtualenv's is recommended but not necessary * Mac
-install instructions. See [here](https://github.com/Unstructured-IO/
-community#mac--homebrew) for more detailed instructions. * `brew install pyenv-
-virtualenv` * `pyenv install 3.8.17` * Linux instructions are available [here]
-(https://github.com/Unstructured-IO/community#linux). * Create a virtualenv to
-work in and activate it, e.g. for one named `unstructured`: `pyenv virtualenv
-3.8.17 unstructured`
+installation. - Install the Python SDK to support all document types with `pip
+install "unstructured[all-docs]"` - For plain text files, HTML, XML, JSON and
+Emails that do not require any extra dependencies, you can run `pip install
+unstructured` - To process other doc types, you can install the extras required
+for those documents, such as `pip install "unstructured[docx,pptx]"` - Install
+the following system dependencies if they are not already available on your
+system. Depending on what document types you're parsing, you may not need all
+of these. - `libmagic-dev` (filetype detection) - `poppler-utils` (images and
+PDFs) - `tesseract-ocr` (images and PDFs) - `libreoffice` (MS Office docs) -
+`pandoc` (EPUBs, RTFs and Open Office docs) - For suggestions on how to install
+on the Windows and to learn about dependencies for other features, see the
+installation documentation [here](https://unstructured-io.github.io/
+unstructured/installing.html). At this point, you should be able to run the
+following code: ```python from unstructured.partition.auto import partition
+elements = partition(filename="example-docs/eml/fake-email.eml") print
+("\n\n".join([str(el) for el in elements])) ``` ### Installation Instructions
+for Local Development The following instructions are intended to help you get
+up and running with `unstructured` locally if you are planning to contribute to
+the project. * Using `pyenv` to manage virtualenv's is recommended but not
+necessary * Mac install instructions. See [here](https://github.com/
+Unstructured-IO/community#mac--homebrew) for more detailed instructions. *
+`brew install pyenv-virtualenv` * `pyenv install 3.8.17` * Linux instructions
+are available [here](https://github.com/Unstructured-IO/community#linux). *
+Create a virtualenv to work in and activate it, e.g. for one named
+`unstructured`: `pyenv virtualenv 3.8.17 unstructured`
 `pyenv activate unstructured` * Run `make install` * Optional: * To install
 models and dependencies for processing images and PDFs locally, run `make
 install-local-inference`. * For processing image files, `tesseract` is
 required. See [here](https://tesseract-ocr.github.io/tessdoc/Installation.html)
 for installation instructions. * For processing PDF files, `tesseract` and
 `poppler` are required. The [pdf2image docs](https://pdf2image.readthedocs.io/
 en/latest/installation.html) have instructions on installing `poppler` across
 various platforms. Additionally, if you're planning to contribute to
 `unstructured`, we provide you an optional `pre-commit` configuration file to
 ensure your code matches the formatting and linting standards used in
-`unstructured`. If you'd prefer not having code changes auto-tidied before
+`unstructured`. If you'd prefer not to have code changes auto-tidied before
 every commit, you can use `make check` to see whether any linting or formatting
 changes should be applied, and `make tidy` to apply them. If using the optional
 `pre-commit`, you'll just need to install the hooks with `pre-commit install`
 since the `pre-commit` package is installed as part of `make install` mentioned
 above. Finally, if you decided to use `pre-commit` you can also uninstall the
-hooks with `pre-commit uninstall`. ## :clap: Quick Tour You can run this [Colab
-notebook](https://colab.research.google.com/drive/1U8VCjY2-
-x8c6y5TYMbSFtQGlQVFHCVIW) to run the examples below. The following examples
-show how to get started with the `unstructured` library. You can parse over a
-dozen document types with one line of code!
-See our [documentation page](https://unstructured-io.github.io/unstructured)
-for a full description of the features in the library. ### Document Parsing The
-easiest way to parse a document in unstructured is to use the `partition`
-brick. If you use `partition` brick, `unstructured` will detect the file type
-and route it to the appropriate file-specific partitioning brick. If you are
-using the `partition` brick, you may need to install additional parameters via
-`pip install unstructured[local-inference]`. Ensure you first install
-`libmagic` using the instructions outlined [here](https://unstructured-
-io.github.io/unstructured/installing.html#filetype-detection) `partition` will
-always apply the default arguments. If you need advanced features, use a
-document-specific brick. See the table above for a full list of document types
-supported in the library. ```python from unstructured.partition.auto import
-partition elements = partition("example-docs/layout-parser-paper.pdf") ``` Run
-`print("\n\n".join([str(el) for el in elements]))` to get a string
-representation of the output, which looks like: ``` LayoutParser : A Uniï¬ed
-Toolkit for Deep Learning Based Document Image Analysis Zejiang Shen 1 ( (cid:
-0) ), Ruochen Zhang 2 , Melissa Dell 3 , Benjamin Charles Germain Lee 4 , Jacob
-Carlson 3 , and Weining Li 5 Abstract. Recent advances in document image
-analysis (DIA) have been primarily driven by the application of neural
-networks. Ideally, research outcomes could be easily deployed in production and
-extended for further investigation. However, various factors like loosely
-organized codebases and sophisticated model conï¬gurations complicate the easy
-reuse of im- portant innovations by a wide audience. Though there have been on-
-going eï¬orts to improve reusability and simplify deep learning (DL) model
-development in disciplines like natural language processing and computer
-vision, none of them are optimized for challenges in the domain of DIA. This
-represents a major gap in the existing toolkit, as DIA is central to academic
-research across a wide range of disciplines in the social sciences and
-humanities. This paper introduces LayoutParser , an open-source library for
-streamlining the usage of DL in DIA research and applica- tions. The core
-LayoutParser library comes with a set of simple and intuitive interfaces for
-applying and customizing DL models for layout de- tection, character
-recognition, and many other document processing tasks. To promote
-extensibility, LayoutParser also incorporates a community platform for sharing
-both pre-trained models and full document digiti- zation pipelines. We
-demonstrate that LayoutParser is helpful for both lightweight and large-scale
-digitization pipelines in real-word use cases. The library is publicly
-available at https://layout-parser.github.io Keywords: Document Image Analysis
-Â· Deep Learning Â· Layout Analysis Â· Character Recognition Â· Open Source
-library Â· Toolkit. Introduction Deep Learning(DL)-based approaches are the
-state-of-the-art for a wide range of document image analysis (DIA) tasks
+hooks with `pre-commit uninstall`. ## :clap: Quick Tour ### Documentation This
+README overviews how to install, use and develop the library. For more
+comprehensive documentation, visit https://unstructured-io.github.io/
+unstructured/ . ### Concepts Guide **Bricks** ð§± in `unstructured` are the
+foundational elements that drive the data processing workflow within the
+system. These components provide users with the building blocks to build
+pipelines targeted at the documents they care about. The bricks fall into three
+categories: - :jigsaw: *Partitioning* bricks break raw documents into standard,
+structured elements. - :broom: *Cleaning* bricks remove unwanted text from
+documents, such as boilerplate and sentence fragments. - :performing_arts:
+*Staging* bricks format data for downstream tasks, such as ML inference and
+data labeling. These bricks create a cohesive, streamlined process that enables
+effective data handling and analysis. Check out the available bricks and how to
+use them from the [Bricks documentation](https://unstructured-io.github.io/
+unstructured/bricks.html). The **Connectors** ð in `unstructured` serve as
+vital links between the pre-processing pipeline and various data storage
+platforms. They allow for the batch processing of documents across various
+sources, including cloud services, repositories, and local directories. Each
+connector is tailored to a specific platform, such as Azure, Google Drive, or
+Github, and comes with unique commands and dependencies. To see the list of
+Connectors available in `unstructured` library, please check out the
+[Connectors GitHub folder](https://github.com/Unstructured-IO/unstructured/
+tree/main/unstructured/ingest/connector) and [documentation](https://
+unstructured-io.github.io/unstructured/connectors.html) ### PDF Document
+Parsing Example The following examples show how to get started with the
+`unstructured` library. You can parse over a dozen document types with one line
+of code! Use this [Colab notebook](https://colab.research.google.com/drive/
+1U8VCjY2-x8c6y5TYMbSFtQGlQVFHCVIW) to run the example below. The easiest way to
+parse a document in unstructured is to use the `partition` brick. If you use
+`partition` brick, `unstructured` will detect the file type and route it to the
+appropriate file-specific partitioning brick. If you are using the `partition`
+brick, you may need to install additional parameters via `pip install
+unstructured[local-inference]`. Ensure you first install `libmagic` using the
+instructions outlined [here](https://unstructured-io.github.io/unstructured/
+installing.html#filetype-detection) `partition` will always apply the default
+arguments. If you need advanced features, use a document-specific brick.
+```python from unstructured.partition.auto import partition elements =
+partition("example-docs/layout-parser-paper.pdf") ``` Run `print("\n\n".join(
+[str(el) for el in elements]))` to get a string representation of the output,
+which looks like: ``` LayoutParser : A Uniï¬ed Toolkit for Deep Learning Based
+Document Image Analysis Zejiang Shen 1 ( (cid:0) ), Ruochen Zhang 2 , Melissa
+Dell 3 , Benjamin Charles Germain Lee 4 , Jacob Carlson 3 , and Weining Li 5
+Abstract. Recent advances in document image analysis (DIA) have been primarily
+driven by the application of neural networks. Ideally, research outcomes could
+be easily deployed in production and extended for further investigation.
+However, various factors like loosely organized codebases and sophisticated
+model conï¬gurations complicate the easy reuse of im- portant innovations by a
+wide audience. Though there have been on-going eï¬orts to improve reusability
+and simplify deep learning (DL) model development in disciplines like natural
+language processing and computer vision, none of them are optimized for
+challenges in the domain of DIA. This represents a major gap in the existing
+toolkit, as DIA is central to academic research across a wide range of
+disciplines in the social sciences and humanities. This paper introduces
+LayoutParser , an open-source library for streamlining the usage of DL in DIA
+research and applica- tions. The core LayoutParser library comes with a set of
+simple and intuitive interfaces for applying and customizing DL models for
+layout de- tection, character recognition, and many other document processing
+tasks. To promote extensibility, LayoutParser also incorporates a community
+platform for sharing both pre-trained models and full document digiti- zation
+pipelines. We demonstrate that LayoutParser is helpful for both lightweight and
+large-scale digitization pipelines in real-word use cases. The library is
+publicly available at https://layout-parser.github.io Keywords: Document Image
+Analysis Â· Deep Learning Â· Layout Analysis Â· Character Recognition Â· Open
+Source library Â· Toolkit. Introduction Deep Learning(DL)-based approaches are
+the state-of-the-art for a wide range of document image analysis (DIA) tasks
 including document image classiï¬cation [11, ``` See the [partitioning](https:
 //unstructured-io.github.io/unstructured/bricks.html#partitioning) section in
 our documentation for a full list of options and instructions on how to use
 file-specific partitioning functions. ## :guardsman: Security Policy See our
 [security policy](https://github.com/Unstructured-IO/unstructured/security/
 policy) for information on how to report security vulnerabilities. ## :bug:
 Reporting Bugs Encountered a bug? Please create a new [GitHub issue](https://
@@ -228,9 +224,9 @@
 Provides-Extra: odt Provides-Extra: org Provides-Extra: pdf Provides-Extra:
 pptx Provides-Extra: rtf Provides-Extra: rst Provides-Extra: tsv Provides-
 Extra: xlsx Provides-Extra: s3 Provides-Extra: azure Provides-Extra: discord
 Provides-Extra: github Provides-Extra: gitlab Provides-Extra: reddit Provides-
 Extra: notion Provides-Extra: slack Provides-Extra: wikipedia Provides-Extra:
 google-drive Provides-Extra: gcs Provides-Extra: elasticsearch Provides-Extra:
 dropbox Provides-Extra: box Provides-Extra: onedrive Provides-Extra: outlook
-Provides-Extra: confluence Provides-Extra: huggingface Provides-Extra: local-
-inference
+Provides-Extra: confluence Provides-Extra: airtable Provides-Extra: sharepoint
+Provides-Extra: huggingface Provides-Extra: local-inference
```

### Comparing `unstructured-0.9.2/README.md` & `unstructured-0.9.3/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -25,57 +25,44 @@
     <img src="https://img.shields.io/badge/JOIN US ON SLACK-4A154B?style=for-the-badge&logo=slack&logoColor=white" />
   </a>
   <a href="https://www.linkedin.com/company/unstructuredio/">
     <img src="https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white" />
   </a>
 </div>
 
+<h2 align="center">
+  <p>Open-Source Pre-Processing Tools for Unstructured Data</p>
+</h2>
+
+The `unstructured` library provides open-source components for ingesting and pre-processing images and text documents, such as PDFs, HTML, Word docs, and [many more](https://unstructured-io.github.io/unstructured/bricks.html#partitioning). The use cases of `unstructured` revolve around streamlining and optimizing the data processing workflow for LLMs. `unstructured` modular bricks and connectors form a cohesive system that simplifies data ingestion and pre-processing, making it adaptable to different platforms and is efficient in transforming unstructured data into structured outputs.
+
 <h3 align="center">
   <p>API Announcement!</p>
 </h3>
 
-We are thrilled to announce our newly launched [Unstructured API](https://unstructured-io.github.io/unstructured/api.html). While access to the hosted Unstructured API will remain free, API Keys are required to make requests. To prevent disruption, get yours [here](https://unstructured.io/#get-api-key) now and start using it today! Check out the [readme](https://github.com/Unstructured-IO/unstructured-api#--) here to get started making API calls.</p>
+We are thrilled to announce our newly launched [Unstructured API](https://unstructured-io.github.io/unstructured/api.html), providing the Unstructured capabilities from `unstructured` as an API. Check out the [`unstructured-api` GitHub repository](https://github.com/Unstructured-IO/unstructured-api) to start making API calls. You’ll also find instructions about how to host your own API version.
+
+While access to the hosted Unstructured API will remain free, API Keys are required to make requests. To prevent disruption, get yours [here](https://unstructured.io/#get-api-key) and start using it today! Check out the [`unstructured-api` README](https://github.com/Unstructured-IO/unstructured-api#--) to start making API calls.</p>
 
 #### :rocket: Beta Feature: Chipper Model
 
-We are releasing the beta version of our Chipper model to deliver superior performance when processing high-resolution, complex documents. To start using the Chipper model in your API request, you can utilize the `hi_res` strategy. Please refer to the documentation [here](https://unstructured-io.github.io/unstructured/api.html#strategies).
+We are releasing the beta version of our Chipper model to deliver superior performance when processing high-resolution, complex documents. To start using the Chipper model in your API request, you can utilize the `hi_res_model_name=chipper` parameter. Please refer to the documentation [here](https://unstructured-io.github.io/unstructured/api.html#beta-version-hi-res-strategy-with-chipper-model).
 
 As the Chipper model is in beta version, we welcome feedback and suggestions. For those interested in testing the Chipper model, we encourage you to connect with us on [Slack community](https://join.slack.com/t/unstructuredw-kbe4326/shared_invite/zt-1x7cgo0pg-PTptXWylzPQF9xZolzCnwQ).
 
-<h3 align="center">
-  <p>Open-Source Pre-Processing Tools for Unstructured Data</p>
-</h3>
-
-The `unstructured` library provides open-source components for pre-processing text documents
-such as **PDFs**, **HTML** and **Word** Documents. These components are packaged as *bricks* 🧱, which provide
-users the building blocks they need to build pipelines targeted at the documents they care
-about. Bricks in the library fall into three categories:
-
-- :jigsaw: ***Partitioning bricks*** that break raw documents down into standard, structured
-  elements.
-- :broom: ***Cleaning bricks*** that remove unwanted text from documents, such as boilerplate and
-  sentence
-  fragments.
-- :performing_arts: ***Staging bricks*** that format data for downstream tasks, such as ML inference
-  and data labeling.
-
-Unstructured also provides the capabilities from `unstructured` as an API.
-Checkout the [`unstructured-api` repo](https://github.com/Unstructured-IO/unstructured-api)
-to get started making API calls.
-You’ll also find instructions there about how to host your own version of the API.
-
-## :bookmark: Documentation
-This README gives an overview of how to install, use and develop the library.
-For more comprehensive documentation, visit https://unstructured-io.github.io/unstructured/ .
-
 ## :eight_pointed_black_star: Quick Start
 
-There are two ways to use the library: 1) run a container or 2) install it
+There are several ways to use the `unstructured` library:
+* [Run the library in a container](https://github.com/Unstructured-IO/unstructured#using-the-library-in-a-container) or
+* Install the library
+    1. [Install from PyPI](https://github.com/Unstructured-IO/unstructured#installing-the-library)
+    2. [Install for local development](https://github.com/Unstructured-IO/unstructured#coffee-installation-instructions-for-local-development)
+* For installation with `conda` on Windows system, please refer to the [documentation](https://unstructured-io.github.io/unstructured/installing.html#installation-with-conda-on-windows)
 
-### Using the library in a container
+### Run the library in a container
 
 The following instructions are intended to help you get up and running using Docker to interact with `unstructured`.
 See [here](https://docs.docker.com/get-docker/) if you don't already have docker installed on your machine.
 
 NOTE: we build multi-platform images to support both x86_64 and Apple silicon hardware. `docker pull` should download the corresponding image for your architecture, but you can specify with `--platform` (e.g. `--platform linux/amd64`) if needed.
 
 We build Docker images for all pushes to `main`. We tag each image with the corresponding short commit hash (e.g. `fbc7a69`) and the application version (e.g. `0.5.5-dev1`). We also tag the most recent image with `latest`. To leverage this, `docker pull` from our image repository.
@@ -103,15 +90,15 @@
 ```bash
 make docker-build
 
 # this will drop you into a bash shell where the Docker image is running
 make docker-start-bash
 ```
 
-Once in the running container, you can try things out directly in Python interpreter's interactive mode.
+Once in the running container, you can try things directly in Python interpreter's interactive mode.
 ```bash
 # this will drop you into a python console so you can run the below partition functions
 python3
 
 >>> from unstructured.partition.pdf import partition_pdf
 >>> elements = partition_pdf(filename="example-docs/layout-parser-paper-fast.pdf")
 
@@ -119,69 +106,38 @@
 >>> elements = partition_text(filename="example-docs/fake-text.txt")
 ```
 
 ### Installing the library
 Use the following instructions to get up and running with `unstructured` and test your
 installation.
 
-- Install the Python SDK with `pip install "unstructured[local-inference]"`
-		- If you do not need to process PDFs or images, you can run `pip install unstructured`
+- Install the Python SDK to support all document types with `pip install "unstructured[all-docs]"`
+  - For plain text files, HTML, XML, JSON and Emails that do not require any extra dependencies, you can run `pip install unstructured`
+  - To process other doc types, you can install the extras required for those documents, such as `pip install "unstructured[docx,pptx]"`
 - Install the following system dependencies if they are not already available on your system.
   Depending on what document types you're parsing, you may not need all of these.
     - `libmagic-dev` (filetype detection)
     - `poppler-utils` (images and PDFs)
     - `tesseract-ocr` (images and PDFs)
     - `libreoffice` (MS Office docs)
     - `pandoc` (EPUBs, RTFs and Open Office docs)
 
-- For suggestions on how to install on Windows and to learn about dependencies for other features, see the
+- For suggestions on how to install on the Windows and to learn about dependencies for other features, see the
   installation documentation [here](https://unstructured-io.github.io/unstructured/installing.html).
 
 At this point, you should be able to run the following code:
 
 ```python
 from unstructured.partition.auto import partition
 
 elements = partition(filename="example-docs/eml/fake-email.eml")
 print("\n\n".join([str(el) for el in elements]))
 ```
 
-The following table shows the document types the `unstructured` library currently supports.
-`partition` will recognize each of these document types and route the document to the
-appropriate partitioning function. If you already know your document type, you can use
-the partitioning function listed in the table directly.
-See our [documentation page](https://unstructured-io.github.io/unstructured/) for more details
-about the library.
-
-| Document Type | Partition Function | Strategies | Table Support | Options |
-| --- | --- | --- | --- | --- |
-| CSV Files (`.csv`) | `partition_csv` | N/A | Yes | None |
-| E-mails (`.eml`) | `partition_eml` | N/A | No | Encoding; Max Partition; Process Attachments |
-| E-mails (`.msg`) | `partition_msg` | N/A | No | Encoding; Max Partition; Process Attachments |
-| EPubs (`.epub`) | `partition_epub` | N/A | Yes | Include Page Breaks |
-| Excel Documents (`.xlsx`/`.xls`) | `partition_xlsx` | N/A | Yes | None |
-| HTML Pages (`.html`) | `partition_html` | N/A | No | Encoding; Include Page Breaks |
-| Images (`.png`/`.jpg`) | `partition_image` | `"auto"`, `"hi_res"`, `"ocr_only"` | Yes | Encoding; Include Page Breaks; Infer Table Structure; OCR Languages, Strategy |
-| Markdown (`.md`) | `partitin_md` | N/A | Yes | Include Page Breaks |
-| Org Mode (`.org`) | `partition_org` | N/A | Yes | Include Page Breaks |
-| Open Office Documents (`.odt`) | `partition_odt` | N/A | Yes | None |
-| PDFs (`.pdf`) | `partition_pdf` | `"auto"`, `"fast"`, `"hi_res"`, `"ocr_only"` | Yes | Encoding; Include Page Breaks; Infer Table Structure; Max Partition; OCR Languages, Strategy |
-| Plain Text (`.txt`) | `partition_text` | N/A | No | Encoding; Max Partition; Paragraph Grouper |
-| Power Points (`.ppt`) | `partition_ppt` | N/A | Yes | Include Page Breaks |
-| Power Points (`.pptx`) | `partition_pptx` | N/A | Yes | Include Page Breaks |
-| ReStructured Text (`.rst`) | `partition_rst` | N/A | Yes | Include Page Breaks |
-| Rich Text Files (`.rtf`) | `partition_rtf` | N/A | Yes | Include Page Breaks |
-| TSV Files (`.tsv`) | `partition_tsv` | N/A | Yes | None |
-| Word Documents (`.doc`) | `partition_doc` | N/A | Yes | Include Page Breaks |
-| Word Documents (`.docx`) | `partition_docx` | N/A | Yes | Include Page Breaks |
-| XML Documents (`.xml`) | `partition_xml` | N/A | No | Encoding; Max Partition; XML Keep Tags |
-
-
-
-## :coffee: Installation Instructions for Local Development
+### Installation Instructions for Local Development
 
 The following instructions are intended to help you get up and running with `unstructured`
 locally if you are planning to contribute to the project.
 
 * Using `pyenv` to manage virtualenv's is recommended but not necessary
 	* Mac install instructions. See [here](https://github.com/Unstructured-IO/community#mac--homebrew) for more detailed instructions.
 		* `brew install pyenv-virtualenv`
@@ -198,41 +154,41 @@
 * Optional:
   * To install models and dependencies for processing images and PDFs locally, run `make install-local-inference`.
   * For processing image files, `tesseract` is required. See [here](https://tesseract-ocr.github.io/tessdoc/Installation.html) for installation instructions.
   * For processing PDF files, `tesseract` and `poppler` are required. The [pdf2image docs](https://pdf2image.readthedocs.io/en/latest/installation.html) have instructions on installing `poppler` across various platforms.
 
 Additionally, if you're planning to contribute to `unstructured`, we provide you an optional `pre-commit` configuration
 file to ensure your code matches the formatting and linting standards used in `unstructured`.
-If you'd prefer not having code changes auto-tidied before every commit, you can use  `make check` to see
+If you'd prefer not to have code changes auto-tidied before every commit, you can use  `make check` to see
 whether any linting or formatting changes should be applied, and `make tidy` to apply them.
 
 If using the optional `pre-commit`, you'll just need to install the hooks with `pre-commit install` since the
 `pre-commit` package is installed as part of `make install` mentioned above. Finally, if you decided to use `pre-commit`
 you can also uninstall the hooks with `pre-commit uninstall`.
 
 ## :clap: Quick Tour
 
-You can run this [Colab notebook](https://colab.research.google.com/drive/1U8VCjY2-x8c6y5TYMbSFtQGlQVFHCVIW) to run the examples below.
+### Documentation
+This README overviews how to install, use and develop the library. For more comprehensive documentation, visit https://unstructured-io.github.io/unstructured/ .
+
+### Concepts Guide
+
+**Bricks** 🧱 in `unstructured` are the foundational elements that drive the data processing workflow within the system. These components provide users with the building blocks to build pipelines targeted at the documents they care about. The bricks fall into three categories:
+- :jigsaw: *Partitioning* bricks break raw documents into standard, structured elements.
+- :broom: *Cleaning* bricks remove unwanted text from documents, such as boilerplate and sentence fragments.
+- :performing_arts: *Staging* bricks format data for downstream tasks, such as ML inference and data labeling. 
+
+These bricks create a cohesive, streamlined process that enables effective data handling and analysis. Check out the available bricks and how to use them from the [Bricks documentation](https://unstructured-io.github.io/unstructured/bricks.html).
+
+The **Connectors** 🔗 in `unstructured` serve as vital links between the pre-processing pipeline and various data storage platforms. They allow for the batch processing of documents across various sources, including cloud services, repositories, and local directories. Each connector is tailored to a specific platform, such as Azure, Google Drive, or Github, and comes with unique commands and dependencies. To see the list of Connectors available in `unstructured` library, please check out the [Connectors GitHub folder](https://github.com/Unstructured-IO/unstructured/tree/main/unstructured/ingest/connector) and [documentation](https://unstructured-io.github.io/unstructured/connectors.html)
+
+### PDF Document Parsing Example
+The following examples show how to get started with the `unstructured` library. You can parse over a dozen document types with one line of code! Use this [Colab notebook](https://colab.research.google.com/drive/1U8VCjY2-x8c6y5TYMbSFtQGlQVFHCVIW) to run the example below.
 
-The following examples show how to get started with the `unstructured` library.
-You can parse over a dozen document types with one line of code!
-<br></br>
-See our [documentation page](https://unstructured-io.github.io/unstructured) for a full description
-of the features in the library.
-
-### Document Parsing
-
-The easiest way to parse a document in unstructured is to use the `partition` brick. If you
-use `partition` brick, `unstructured` will detect the file type and route it to the appropriate
-file-specific partitioning brick.
-If you are using the `partition` brick, you may need to install additional parameters via `pip install unstructured[local-inference]`. Ensure you first install `libmagic` using the
-instructions outlined [here](https://unstructured-io.github.io/unstructured/installing.html#filetype-detection)
-`partition` will always apply the default arguments. If you need
-advanced features, use a document-specific brick.
-See the table above for a full list of document types supported in the library.
+The easiest way to parse a document in unstructured is to use the `partition` brick. If you use `partition` brick, `unstructured` will detect the file type and route it to the appropriate file-specific partitioning brick. If you are using the `partition` brick, you may need to install additional parameters via `pip install unstructured[local-inference]`. Ensure you first install `libmagic` using the instructions outlined [here](https://unstructured-io.github.io/unstructured/installing.html#filetype-detection) `partition` will always apply the default arguments. If you need advanced features, use a document-specific brick.
 
 ```python
 from unstructured.partition.auto import partition
 
 elements = partition("example-docs/layout-parser-paper.pdf")
 ```
```

#### html2text {}

```diff
@@ -11,192 +11,188 @@
 _b_a_d_g_e_s_/_]_(_h_t_t_p_s_:_/_/_b_a_d_g_e_n_._n_e_t_/_b_a_d_g_e_/_O_p_e_n_%_2_0_S_o_u_r_c_e_%_2_0_%_3_F_/_Y_e_s_%_2_1_/_b_l_u_e_?_i_c_o_n_=_g_i_t_h_u_b_)
 [![Downloads](https://static.pepy.tech/badge/unstructured)](https://pepy.tech/
       project/unstructured) [![Downloads](https://static.pepy.tech/badge/
          unstructured/month)](https://pepy.tech/project/unstructured)
      _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_J_O_I_N_ _U_S_ _O_N_ _S_L_A_C_K_-_4_A_1_5_4_B_?_s_t_y_l_e_=_f_o_r_-_t_h_e_-
    _b_a_d_g_e_&_l_o_g_o_=_s_l_a_c_k_&_l_o_g_o_C_o_l_o_r_=_w_h_i_t_e_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_L_i_n_k_e_d_I_n_-
            _0_0_7_7_B_5_?_s_t_y_l_e_=_f_o_r_-_t_h_e_-_b_a_d_g_e_&_l_o_g_o_=_l_i_n_k_e_d_i_n_&_l_o_g_o_C_o_l_o_r_=_w_h_i_t_e_]
+      ********** OOppeenn--SSoouurrccee PPrree--PPrroocceessssiinngg TToooollss ffoorr UUnnssttrruuccttuurreedd DDaattaa **********
+The `unstructured` library provides open-source components for ingesting and
+pre-processing images and text documents, such as PDFs, HTML, Word docs, and
+[many more](https://unstructured-io.github.io/unstructured/
+bricks.html#partitioning). The use cases of `unstructured` revolve around
+streamlining and optimizing the data processing workflow for LLMs.
+`unstructured` modular bricks and connectors form a cohesive system that
+simplifies data ingestion and pre-processing, making it adaptable to different
+platforms and is efficient in transforming unstructured data into structured
+outputs.
                           ******** AAPPII AAnnnnoouunncceemmeenntt!! ********
 We are thrilled to announce our newly launched [Unstructured API](https://
-unstructured-io.github.io/unstructured/api.html). While access to the hosted
-Unstructured API will remain free, API Keys are required to make requests. To
-prevent disruption, get yours [here](https://unstructured.io/#get-api-key) now
-and start using it today! Check out the [readme](https://github.com/
-Unstructured-IO/unstructured-api#--) here to get started making API calls.
+unstructured-io.github.io/unstructured/api.html), providing the Unstructured
+capabilities from `unstructured` as an API. Check out the [`unstructured-api`
+GitHub repository](https://github.com/Unstructured-IO/unstructured-api) to
+start making API calls. Youâll also find instructions about how to host your
+own API version. While access to the hosted Unstructured API will remain free,
+API Keys are required to make requests. To prevent disruption, get yours [here]
+(https://unstructured.io/#get-api-key) and start using it today! Check out the
+[`unstructured-api` README](https://github.com/Unstructured-IO/unstructured-
+api#--) to start making API calls.
 #### :rocket: Beta Feature: Chipper Model We are releasing the beta version of
 our Chipper model to deliver superior performance when processing high-
 resolution, complex documents. To start using the Chipper model in your API
-request, you can utilize the `hi_res` strategy. Please refer to the
-documentation [here](https://unstructured-io.github.io/unstructured/
-api.html#strategies). As the Chipper model is in beta version, we welcome
-feedback and suggestions. For those interested in testing the Chipper model, we
-encourage you to connect with us on [Slack community](https://join.slack.com/t/
-unstructuredw-kbe4326/shared_invite/zt-1x7cgo0pg-PTptXWylzPQF9xZolzCnwQ).
-       ******** OOppeenn--SSoouurrccee PPrree--PPrroocceessssiinngg TToooollss ffoorr UUnnssttrruuccttuurreedd DDaattaa ********
-The `unstructured` library provides open-source components for pre-processing
-text documents such as **PDFs**, **HTML** and **Word** Documents. These
-components are packaged as *bricks* ð§±, which provide users the building
-blocks they need to build pipelines targeted at the documents they care about.
-Bricks in the library fall into three categories: - :jigsaw: ***Partitioning
-bricks*** that break raw documents down into standard, structured elements. - :
-broom: ***Cleaning bricks*** that remove unwanted text from documents, such as
-boilerplate and sentence fragments. - :performing_arts: ***Staging bricks***
-that format data for downstream tasks, such as ML inference and data labeling.
-Unstructured also provides the capabilities from `unstructured` as an API.
-Checkout the [`unstructured-api` repo](https://github.com/Unstructured-IO/
-unstructured-api) to get started making API calls. Youâll also find
-instructions there about how to host your own version of the API. ## :bookmark:
-Documentation This README gives an overview of how to install, use and develop
-the library. For more comprehensive documentation, visit https://unstructured-
-io.github.io/unstructured/ . ## :eight_pointed_black_star: Quick Start There
-are two ways to use the library: 1) run a container or 2) install it ### Using
-the library in a container The following instructions are intended to help you
-get up and running using Docker to interact with `unstructured`. See [here]
-(https://docs.docker.com/get-docker/) if you don't already have docker
-installed on your machine. NOTE: we build multi-platform images to support both
-x86_64 and Apple silicon hardware. `docker pull` should download the
-corresponding image for your architecture, but you can specify with `--
-platform` (e.g. `--platform linux/amd64`) if needed. We build Docker images for
-all pushes to `main`. We tag each image with the corresponding short commit
-hash (e.g. `fbc7a69`) and the application version (e.g. `0.5.5-dev1`). We also
-tag the most recent image with `latest`. To leverage this, `docker pull` from
-our image repository. ```bash docker pull quay.io/unstructured-io/unstructured:
-latest ``` Once pulled, you can create a container from this image and shell to
-it. ```bash # create the container docker run -dt --name unstructured quay.io/
-unstructured-io/unstructured:latest # this will drop you into a bash shell
-where the Docker image is running docker exec -it unstructured bash ``` You can
-also build your own Docker image. If you only plan on parsing one type of data
-you can speed up building the image by commenting out some of the packages/
-requirements necessary for other data types. See Dockerfile to know which lines
-are necessary for your use case. ```bash make docker-build # this will drop you
+request, you can utilize the `hi_res_model_name=chipper` parameter. Please
+refer to the documentation [here](https://unstructured-io.github.io/
+unstructured/api.html#beta-version-hi-res-strategy-with-chipper-model). As the
+Chipper model is in beta version, we welcome feedback and suggestions. For
+those interested in testing the Chipper model, we encourage you to connect with
+us on [Slack community](https://join.slack.com/t/unstructuredw-kbe4326/
+shared_invite/zt-1x7cgo0pg-PTptXWylzPQF9xZolzCnwQ). ## :
+eight_pointed_black_star: Quick Start There are several ways to use the
+`unstructured` library: * [Run the library in a container](https://github.com/
+Unstructured-IO/unstructured#using-the-library-in-a-container) or * Install the
+library 1. [Install from PyPI](https://github.com/Unstructured-IO/
+unstructured#installing-the-library) 2. [Install for local development](https:/
+/github.com/Unstructured-IO/unstructured#coffee-installation-instructions-for-
+local-development) * For installation with `conda` on Windows system, please
+refer to the [documentation](https://unstructured-io.github.io/unstructured/
+installing.html#installation-with-conda-on-windows) ### Run the library in a
+container The following instructions are intended to help you get up and
+running using Docker to interact with `unstructured`. See [here](https://
+docs.docker.com/get-docker/) if you don't already have docker installed on your
+machine. NOTE: we build multi-platform images to support both x86_64 and Apple
+silicon hardware. `docker pull` should download the corresponding image for
+your architecture, but you can specify with `--platform` (e.g. `--platform
+linux/amd64`) if needed. We build Docker images for all pushes to `main`. We
+tag each image with the corresponding short commit hash (e.g. `fbc7a69`) and
+the application version (e.g. `0.5.5-dev1`). We also tag the most recent image
+with `latest`. To leverage this, `docker pull` from our image repository.
+```bash docker pull quay.io/unstructured-io/unstructured:latest ``` Once
+pulled, you can create a container from this image and shell to it. ```bash #
+create the container docker run -dt --name unstructured quay.io/unstructured-
+io/unstructured:latest # this will drop you into a bash shell where the Docker
+image is running docker exec -it unstructured bash ``` You can also build your
+own Docker image. If you only plan on parsing one type of data you can speed up
+building the image by commenting out some of the packages/requirements
+necessary for other data types. See Dockerfile to know which lines are
+necessary for your use case. ```bash make docker-build # this will drop you
 into a bash shell where the Docker image is running make docker-start-bash ```
-Once in the running container, you can try things out directly in Python
+Once in the running container, you can try things directly in Python
 interpreter's interactive mode. ```bash # this will drop you into a python
 console so you can run the below partition functions python3 >>> from
 unstructured.partition.pdf import partition_pdf >>> elements = partition_pdf
 (filename="example-docs/layout-parser-paper-fast.pdf") >>> from
 unstructured.partition.text import partition_text >>> elements = partition_text
 (filename="example-docs/fake-text.txt") ``` ### Installing the library Use the
 following instructions to get up and running with `unstructured` and test your
-installation. - Install the Python SDK with `pip install "unstructured[local-
-inference]"` - If you do not need to process PDFs or images, you can run `pip
-install unstructured` - Install the following system dependencies if they are
-not already available on your system. Depending on what document types you're
-parsing, you may not need all of these. - `libmagic-dev` (filetype detection) -
-`poppler-utils` (images and PDFs) - `tesseract-ocr` (images and PDFs) -
-`libreoffice` (MS Office docs) - `pandoc` (EPUBs, RTFs and Open Office docs) -
-For suggestions on how to install on Windows and to learn about dependencies
-for other features, see the installation documentation [here](https://
-unstructured-io.github.io/unstructured/installing.html). At this point, you
-should be able to run the following code: ```python from
-unstructured.partition.auto import partition elements = partition
-(filename="example-docs/eml/fake-email.eml") print("\n\n".join([str(el) for el
-in elements])) ``` The following table shows the document types the
-`unstructured` library currently supports. `partition` will recognize each of
-these document types and route the document to the appropriate partitioning
-function. If you already know your document type, you can use the partitioning
-function listed in the table directly. See our [documentation page](https://
-unstructured-io.github.io/unstructured/) for more details about the library. |
-Document Type | Partition Function | Strategies | Table Support | Options | | -
--- | --- | --- | --- | --- | | CSV Files (`.csv`) | `partition_csv` | N/A | Yes
-| None | | E-mails (`.eml`) | `partition_eml` | N/A | No | Encoding; Max
-Partition; Process Attachments | | E-mails (`.msg`) | `partition_msg` | N/A |
-No | Encoding; Max Partition; Process Attachments | | EPubs (`.epub`) |
-`partition_epub` | N/A | Yes | Include Page Breaks | | Excel Documents
-(`.xlsx`/`.xls`) | `partition_xlsx` | N/A | Yes | None | | HTML Pages (`.html`)
-| `partition_html` | N/A | No | Encoding; Include Page Breaks | | Images
-(`.png`/`.jpg`) | `partition_image` | `"auto"`, `"hi_res"`, `"ocr_only"` | Yes
-| Encoding; Include Page Breaks; Infer Table Structure; OCR Languages, Strategy
-| | Markdown (`.md`) | `partitin_md` | N/A | Yes | Include Page Breaks | | Org
-Mode (`.org`) | `partition_org` | N/A | Yes | Include Page Breaks | | Open
-Office Documents (`.odt`) | `partition_odt` | N/A | Yes | None | | PDFs
-(`.pdf`) | `partition_pdf` | `"auto"`, `"fast"`, `"hi_res"`, `"ocr_only"` | Yes
-| Encoding; Include Page Breaks; Infer Table Structure; Max Partition; OCR
-Languages, Strategy | | Plain Text (`.txt`) | `partition_text` | N/A | No |
-Encoding; Max Partition; Paragraph Grouper | | Power Points (`.ppt`) |
-`partition_ppt` | N/A | Yes | Include Page Breaks | | Power Points (`.pptx`) |
-`partition_pptx` | N/A | Yes | Include Page Breaks | | ReStructured Text
-(`.rst`) | `partition_rst` | N/A | Yes | Include Page Breaks | | Rich Text
-Files (`.rtf`) | `partition_rtf` | N/A | Yes | Include Page Breaks | | TSV
-Files (`.tsv`) | `partition_tsv` | N/A | Yes | None | | Word Documents (`.doc`)
-| `partition_doc` | N/A | Yes | Include Page Breaks | | Word Documents
-(`.docx`) | `partition_docx` | N/A | Yes | Include Page Breaks | | XML
-Documents (`.xml`) | `partition_xml` | N/A | No | Encoding; Max Partition; XML
-Keep Tags | ## :coffee: Installation Instructions for Local Development The
-following instructions are intended to help you get up and running with
-`unstructured` locally if you are planning to contribute to the project. *
-Using `pyenv` to manage virtualenv's is recommended but not necessary * Mac
-install instructions. See [here](https://github.com/Unstructured-IO/
-community#mac--homebrew) for more detailed instructions. * `brew install pyenv-
-virtualenv` * `pyenv install 3.8.17` * Linux instructions are available [here]
-(https://github.com/Unstructured-IO/community#linux). * Create a virtualenv to
-work in and activate it, e.g. for one named `unstructured`: `pyenv virtualenv
-3.8.17 unstructured`
+installation. - Install the Python SDK to support all document types with `pip
+install "unstructured[all-docs]"` - For plain text files, HTML, XML, JSON and
+Emails that do not require any extra dependencies, you can run `pip install
+unstructured` - To process other doc types, you can install the extras required
+for those documents, such as `pip install "unstructured[docx,pptx]"` - Install
+the following system dependencies if they are not already available on your
+system. Depending on what document types you're parsing, you may not need all
+of these. - `libmagic-dev` (filetype detection) - `poppler-utils` (images and
+PDFs) - `tesseract-ocr` (images and PDFs) - `libreoffice` (MS Office docs) -
+`pandoc` (EPUBs, RTFs and Open Office docs) - For suggestions on how to install
+on the Windows and to learn about dependencies for other features, see the
+installation documentation [here](https://unstructured-io.github.io/
+unstructured/installing.html). At this point, you should be able to run the
+following code: ```python from unstructured.partition.auto import partition
+elements = partition(filename="example-docs/eml/fake-email.eml") print
+("\n\n".join([str(el) for el in elements])) ``` ### Installation Instructions
+for Local Development The following instructions are intended to help you get
+up and running with `unstructured` locally if you are planning to contribute to
+the project. * Using `pyenv` to manage virtualenv's is recommended but not
+necessary * Mac install instructions. See [here](https://github.com/
+Unstructured-IO/community#mac--homebrew) for more detailed instructions. *
+`brew install pyenv-virtualenv` * `pyenv install 3.8.17` * Linux instructions
+are available [here](https://github.com/Unstructured-IO/community#linux). *
+Create a virtualenv to work in and activate it, e.g. for one named
+`unstructured`: `pyenv virtualenv 3.8.17 unstructured`
 `pyenv activate unstructured` * Run `make install` * Optional: * To install
 models and dependencies for processing images and PDFs locally, run `make
 install-local-inference`. * For processing image files, `tesseract` is
 required. See [here](https://tesseract-ocr.github.io/tessdoc/Installation.html)
 for installation instructions. * For processing PDF files, `tesseract` and
 `poppler` are required. The [pdf2image docs](https://pdf2image.readthedocs.io/
 en/latest/installation.html) have instructions on installing `poppler` across
 various platforms. Additionally, if you're planning to contribute to
 `unstructured`, we provide you an optional `pre-commit` configuration file to
 ensure your code matches the formatting and linting standards used in
-`unstructured`. If you'd prefer not having code changes auto-tidied before
+`unstructured`. If you'd prefer not to have code changes auto-tidied before
 every commit, you can use `make check` to see whether any linting or formatting
 changes should be applied, and `make tidy` to apply them. If using the optional
 `pre-commit`, you'll just need to install the hooks with `pre-commit install`
 since the `pre-commit` package is installed as part of `make install` mentioned
 above. Finally, if you decided to use `pre-commit` you can also uninstall the
-hooks with `pre-commit uninstall`. ## :clap: Quick Tour You can run this [Colab
-notebook](https://colab.research.google.com/drive/1U8VCjY2-
-x8c6y5TYMbSFtQGlQVFHCVIW) to run the examples below. The following examples
-show how to get started with the `unstructured` library. You can parse over a
-dozen document types with one line of code!
-See our [documentation page](https://unstructured-io.github.io/unstructured)
-for a full description of the features in the library. ### Document Parsing The
-easiest way to parse a document in unstructured is to use the `partition`
-brick. If you use `partition` brick, `unstructured` will detect the file type
-and route it to the appropriate file-specific partitioning brick. If you are
-using the `partition` brick, you may need to install additional parameters via
-`pip install unstructured[local-inference]`. Ensure you first install
-`libmagic` using the instructions outlined [here](https://unstructured-
-io.github.io/unstructured/installing.html#filetype-detection) `partition` will
-always apply the default arguments. If you need advanced features, use a
-document-specific brick. See the table above for a full list of document types
-supported in the library. ```python from unstructured.partition.auto import
-partition elements = partition("example-docs/layout-parser-paper.pdf") ``` Run
-`print("\n\n".join([str(el) for el in elements]))` to get a string
-representation of the output, which looks like: ``` LayoutParser : A Uniï¬ed
-Toolkit for Deep Learning Based Document Image Analysis Zejiang Shen 1 ( (cid:
-0) ), Ruochen Zhang 2 , Melissa Dell 3 , Benjamin Charles Germain Lee 4 , Jacob
-Carlson 3 , and Weining Li 5 Abstract. Recent advances in document image
-analysis (DIA) have been primarily driven by the application of neural
-networks. Ideally, research outcomes could be easily deployed in production and
-extended for further investigation. However, various factors like loosely
-organized codebases and sophisticated model conï¬gurations complicate the easy
-reuse of im- portant innovations by a wide audience. Though there have been on-
-going eï¬orts to improve reusability and simplify deep learning (DL) model
-development in disciplines like natural language processing and computer
-vision, none of them are optimized for challenges in the domain of DIA. This
-represents a major gap in the existing toolkit, as DIA is central to academic
-research across a wide range of disciplines in the social sciences and
-humanities. This paper introduces LayoutParser , an open-source library for
-streamlining the usage of DL in DIA research and applica- tions. The core
-LayoutParser library comes with a set of simple and intuitive interfaces for
-applying and customizing DL models for layout de- tection, character
-recognition, and many other document processing tasks. To promote
-extensibility, LayoutParser also incorporates a community platform for sharing
-both pre-trained models and full document digiti- zation pipelines. We
-demonstrate that LayoutParser is helpful for both lightweight and large-scale
-digitization pipelines in real-word use cases. The library is publicly
-available at https://layout-parser.github.io Keywords: Document Image Analysis
-Â· Deep Learning Â· Layout Analysis Â· Character Recognition Â· Open Source
-library Â· Toolkit. Introduction Deep Learning(DL)-based approaches are the
-state-of-the-art for a wide range of document image analysis (DIA) tasks
+hooks with `pre-commit uninstall`. ## :clap: Quick Tour ### Documentation This
+README overviews how to install, use and develop the library. For more
+comprehensive documentation, visit https://unstructured-io.github.io/
+unstructured/ . ### Concepts Guide **Bricks** ð§± in `unstructured` are the
+foundational elements that drive the data processing workflow within the
+system. These components provide users with the building blocks to build
+pipelines targeted at the documents they care about. The bricks fall into three
+categories: - :jigsaw: *Partitioning* bricks break raw documents into standard,
+structured elements. - :broom: *Cleaning* bricks remove unwanted text from
+documents, such as boilerplate and sentence fragments. - :performing_arts:
+*Staging* bricks format data for downstream tasks, such as ML inference and
+data labeling. These bricks create a cohesive, streamlined process that enables
+effective data handling and analysis. Check out the available bricks and how to
+use them from the [Bricks documentation](https://unstructured-io.github.io/
+unstructured/bricks.html). The **Connectors** ð in `unstructured` serve as
+vital links between the pre-processing pipeline and various data storage
+platforms. They allow for the batch processing of documents across various
+sources, including cloud services, repositories, and local directories. Each
+connector is tailored to a specific platform, such as Azure, Google Drive, or
+Github, and comes with unique commands and dependencies. To see the list of
+Connectors available in `unstructured` library, please check out the
+[Connectors GitHub folder](https://github.com/Unstructured-IO/unstructured/
+tree/main/unstructured/ingest/connector) and [documentation](https://
+unstructured-io.github.io/unstructured/connectors.html) ### PDF Document
+Parsing Example The following examples show how to get started with the
+`unstructured` library. You can parse over a dozen document types with one line
+of code! Use this [Colab notebook](https://colab.research.google.com/drive/
+1U8VCjY2-x8c6y5TYMbSFtQGlQVFHCVIW) to run the example below. The easiest way to
+parse a document in unstructured is to use the `partition` brick. If you use
+`partition` brick, `unstructured` will detect the file type and route it to the
+appropriate file-specific partitioning brick. If you are using the `partition`
+brick, you may need to install additional parameters via `pip install
+unstructured[local-inference]`. Ensure you first install `libmagic` using the
+instructions outlined [here](https://unstructured-io.github.io/unstructured/
+installing.html#filetype-detection) `partition` will always apply the default
+arguments. If you need advanced features, use a document-specific brick.
+```python from unstructured.partition.auto import partition elements =
+partition("example-docs/layout-parser-paper.pdf") ``` Run `print("\n\n".join(
+[str(el) for el in elements]))` to get a string representation of the output,
+which looks like: ``` LayoutParser : A Uniï¬ed Toolkit for Deep Learning Based
+Document Image Analysis Zejiang Shen 1 ( (cid:0) ), Ruochen Zhang 2 , Melissa
+Dell 3 , Benjamin Charles Germain Lee 4 , Jacob Carlson 3 , and Weining Li 5
+Abstract. Recent advances in document image analysis (DIA) have been primarily
+driven by the application of neural networks. Ideally, research outcomes could
+be easily deployed in production and extended for further investigation.
+However, various factors like loosely organized codebases and sophisticated
+model conï¬gurations complicate the easy reuse of im- portant innovations by a
+wide audience. Though there have been on-going eï¬orts to improve reusability
+and simplify deep learning (DL) model development in disciplines like natural
+language processing and computer vision, none of them are optimized for
+challenges in the domain of DIA. This represents a major gap in the existing
+toolkit, as DIA is central to academic research across a wide range of
+disciplines in the social sciences and humanities. This paper introduces
+LayoutParser , an open-source library for streamlining the usage of DL in DIA
+research and applica- tions. The core LayoutParser library comes with a set of
+simple and intuitive interfaces for applying and customizing DL models for
+layout de- tection, character recognition, and many other document processing
+tasks. To promote extensibility, LayoutParser also incorporates a community
+platform for sharing both pre-trained models and full document digiti- zation
+pipelines. We demonstrate that LayoutParser is helpful for both lightweight and
+large-scale digitization pipelines in real-word use cases. The library is
+publicly available at https://layout-parser.github.io Keywords: Document Image
+Analysis Â· Deep Learning Â· Layout Analysis Â· Character Recognition Â· Open
+Source library Â· Toolkit. Introduction Deep Learning(DL)-based approaches are
+the state-of-the-art for a wide range of document image analysis (DIA) tasks
 including document image classiï¬cation [11, ``` See the [partitioning](https:
 //unstructured-io.github.io/unstructured/bricks.html#partitioning) section in
 our documentation for a full list of options and instructions on how to use
 file-specific partitioning functions. ## :guardsman: Security Policy See our
 [security policy](https://github.com/Unstructured-IO/unstructured/security/
 policy) for information on how to report security vulnerabilities. ## :bug:
 Reporting Bugs Encountered a bug? Please create a new [GitHub issue](https://
```

### Comparing `unstructured-0.9.2/setup.py` & `unstructured-0.9.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,15 +37,15 @@
         req for req in requirements if not req.startswith("#") and not req.startswith("-")
     ]
     return requirements
 
 
 csv_reqs = load_requirements("requirements/extra-csv.in")
 docx_reqs = load_requirements("requirements/extra-docx.in")
-epub_reqs = load_requirements("requirements/extra-pandoc.in")
+epub_reqs = load_requirements("requirements/extra-epub.in")
 image_reqs = load_requirements("requirements/extra-pdf-image.in")
 markdown_reqs = load_requirements("requirements/extra-markdown.in")
 msg_reqs = load_requirements("requirements/extra-msg.in")
 odt_reqs = load_requirements("requirements/extra-odt.in")
 org_reqs = load_requirements("requirements/extra-pandoc.in")
 pdf_reqs = load_requirements("requirements/extra-pdf-image.in")
 pptx_reqs = load_requirements("requirements/extra-pptx.in")
@@ -136,14 +136,16 @@
         "gcs": load_requirements("requirements/ingest-gcs.in"),
         "elasticsearch": load_requirements("requirements/ingest-elasticsearch.in"),
         "dropbox": load_requirements("requirements/ingest-dropbox.in"),
         "box": load_requirements("requirements/ingest-box.in"),
         "onedrive": load_requirements("requirements/ingest-onedrive.in"),
         "outlook": load_requirements("requirements/ingest-outlook.in"),
         "confluence": load_requirements("requirements/ingest-confluence.in"),
+        "airtable": load_requirements("requirements/ingest-airtable.in"),
+        "sharepoint": load_requirements("requirements/ingest-sharepoint.in"),
         # Legacy extra requirements
         "huggingface": load_requirements("requirements/huggingface.in"),
         "local-inference": all_doc_reqs,
     },
     package_dir={"unstructured": "unstructured"},
     package_data={"unstructured": ["nlp/*.txt"]},
 )
```

### Comparing `unstructured-0.9.2/test_unstructured/nlp/mock_nltk.py` & `unstructured-0.9.3/test_unstructured/nlp/mock_nltk.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.9.2/test_unstructured/nlp/test_tokenize.py` & `unstructured-0.9.3/test_unstructured/nlp/test_tokenize.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.9.2/test_unstructured/test_utils.py` & `unstructured-0.9.3/test_unstructured/test_utils.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.9.2/unstructured/cleaners/core.py` & `unstructured-0.9.3/unstructured/cleaners/core.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.9.2/unstructured/cleaners/extract.py` & `unstructured-0.9.3/unstructured/cleaners/extract.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.9.2/unstructured/cleaners/translate.py` & `unstructured-0.9.3/unstructured/cleaners/translate.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.9.2/unstructured/documents/base.py` & `unstructured-0.9.3/unstructured/documents/base.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.9.2/unstructured/documents/coordinates.py` & `unstructured-0.9.3/unstructured/documents/coordinates.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.9.2/unstructured/documents/elements.py` & `unstructured-0.9.3/unstructured/documents/elements.py`

 * *Files 1% similar despite different names*

```diff
@@ -146,14 +146,17 @@
     links: Optional[List[Link]] = None
 
     # E-mail specific metadata fields
     sent_from: Optional[List[str]] = None
     sent_to: Optional[List[str]] = None
     subject: Optional[str] = None
 
+    # Document section fields
+    section: Optional[str] = None
+
     # MSFT Word specific metadata fields
     header_footer_type: Optional[str] = None
 
     # Formatting metadata fields
     emphasized_texts: Optional[List[dict]] = None
 
     # Text format metadata fields
@@ -235,21 +238,30 @@
             for param in sig.parameters.values():
                 if param.name not in params and param.default is not param.empty:
                     params[param.name] = param.default
 
             regex_metadata: Dict["str", "str"] = params.get("regex_metadata", {})
             elements = _add_regex_metadata(elements, regex_metadata)
 
+            unique_element_ids: bool = params.get("unique_element_ids", False)
+            if unique_element_ids:
+                for element in elements:
+                    element.id_to_uuid()
+
             return elements
 
         return wrapper
 
     return decorator
 
 
+def _elements_ids_to_uuid():
+    pass
+
+
 def _add_regex_metadata(
     elements: List[Element],
     regex_metadata: Dict[str, str] = {},
 ) -> List[Element]:
     """Adds metadata based on a user provided regular expression.
     The additional metadata will be added to the regex_metadata
     attrbuted in the element metadata."""
@@ -296,14 +308,17 @@
                     points=coordinates,
                     system=coordinate_system,
                 )
             )
         )
         self.metadata = metadata.merge(ElementMetadata(coordinates=coordinates_metadata))
 
+    def id_to_uuid(self):
+        self.id = str(uuid.uuid4())
+
     def to_dict(self) -> dict:
         return {
             "type": None,
             "element_id": self.id,
             "metadata": self.metadata.to_dict(),
         }
 
@@ -381,15 +396,15 @@
         self.text: str = text
 
         if isinstance(element_id, NoID):
             # NOTE(robinson) - Cut the SHA256 hex in half to get the first 128 bits
             element_id = hashlib.sha256(text.encode()).hexdigest()[:32]
 
         elif isinstance(element_id, UUID):
-            element_id = uuid.uuid4()
+            element_id = str(uuid.uuid4())
 
         super().__init__(
             element_id=element_id,
             metadata=metadata,
             coordinates=coordinates,
             coordinate_system=coordinate_system,
         )
```

### Comparing `unstructured-0.9.2/unstructured/documents/email_elements.py` & `unstructured-0.9.3/unstructured/documents/email_elements.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.9.2/unstructured/documents/html.py` & `unstructured-0.9.3/unstructured/documents/html.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.9.2/unstructured/documents/xml.py` & `unstructured-0.9.3/unstructured/documents/xml.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.9.2/unstructured/file_utils/encoding.py` & `unstructured-0.9.3/unstructured/file_utils/encoding.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.9.2/unstructured/file_utils/exploration.py` & `unstructured-0.9.3/unstructured/file_utils/exploration.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.9.2/unstructured/file_utils/file_conversion.py` & `unstructured-0.9.3/unstructured/file_utils/file_conversion.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.9.2/unstructured/file_utils/filetype.py` & `unstructured-0.9.3/unstructured/file_utils/filetype.py`

 * *Files 0% similar despite different names*

```diff
@@ -499,14 +499,15 @@
 
 
 def document_to_element_list(
     document: "DocumentLayout",
     include_page_breaks: bool = False,
     sort: bool = False,
     last_modification_date: Optional[str] = None,
+    **kwargs,
 ) -> List[Element]:
     """Converts a DocumentLayout object to a list of unstructured elements."""
     elements: List[Element] = []
     num_pages = len(document.pages)
     for i, page in enumerate(document.pages):
         page_elements: List[Element] = []
 
@@ -542,14 +543,15 @@
             )
             _add_element_metadata(
                 element,
                 page_number=i + 1,
                 filetype=image_format,
                 coordinates=coordinates,
                 coordinate_system=coordinate_system,
+                **kwargs,
             )
         if sort:
             page_elements = sorted(
                 page_elements,
                 key=lambda el: (
                     el.metadata.coordinates.points[0][1]
                     if el.metadata.coordinates
```

### Comparing `unstructured-0.9.2/unstructured/file_utils/metadata.py` & `unstructured-0.9.3/unstructured/file_utils/metadata.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.9.2/unstructured/ingest/cli/cli.py` & `unstructured-0.9.3/unstructured/ingest/cli/cli.py`

 * *Files 5% similar despite different names*

```diff
@@ -27,14 +27,15 @@
     cli_cmds.notion,
     cli_cmds.onedrive,
     cli_cmds.outlook,
     cli_cmds.local,
     cli_cmds.elasticsearch,
     cli_cmds.confluence,
     cli_cmds.sharepoint,
+    cli_cmds.airtable,
 ]
 
 for subcommand in subcommands:
     ingest.add_command(subcommand())
 
 
 def get_cmd() -> click.Command:
```

### Comparing `unstructured-0.9.2/unstructured/ingest/cli/cmds/__init__.py` & `unstructured-0.9.3/unstructured/ingest/cli/cmds/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from .airtable import get_cmd as airtable
 from .azure import get_cmd as azure
 from .biomed import get_cmd as biomed
 from .box import get_cmd as box
 from .confluence import get_cmd as confluence
 from .discord import get_cmd as discord
 from .dropbox import get_cmd as dropbox
 from .elasticsearch import get_cmd as elasticsearch
@@ -17,14 +18,15 @@
 from .reddit import get_cmd as reddit
 from .s3 import get_cmd as s3
 from .sharepoint import get_cmd as sharepoint
 from .slack import get_cmd as slack
 from .wikipedia import get_cmd as wikipedia
 
 __all__ = [
+    "airtable",
     "azure",
     "biomed",
     "box",
     "confluence",
     "discord",
     "dropbox",
     "elasticsearch",
```

### Comparing `unstructured-0.9.2/unstructured/ingest/cli/cmds/azure.py` & `unstructured-0.9.3/unstructured/ingest/cli/cmds/azure.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.9.2/unstructured/ingest/cli/cmds/biomed.py` & `unstructured-0.9.3/unstructured/ingest/cli/cmds/biomed.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.9.2/unstructured/ingest/cli/cmds/box.py` & `unstructured-0.9.3/unstructured/ingest/cli/cmds/box.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.9.2/unstructured/ingest/cli/cmds/confluence.py` & `unstructured-0.9.3/unstructured/ingest/cli/cmds/confluence.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.9.2/unstructured/ingest/cli/cmds/discord.py` & `unstructured-0.9.3/unstructured/ingest/cli/cmds/discord.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.9.2/unstructured/ingest/cli/cmds/dropbox.py` & `unstructured-0.9.3/unstructured/ingest/cli/cmds/dropbox.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.9.2/unstructured/ingest/cli/cmds/elasticsearch.py` & `unstructured-0.9.3/unstructured/ingest/cli/cmds/elasticsearch.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.9.2/unstructured/ingest/cli/cmds/fsspec.py` & `unstructured-0.9.3/unstructured/ingest/cli/cmds/fsspec.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.9.2/unstructured/ingest/cli/cmds/gcs.py` & `unstructured-0.9.3/unstructured/ingest/cli/cmds/gcs.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.9.2/unstructured/ingest/cli/cmds/github.py` & `unstructured-0.9.3/unstructured/ingest/cli/cmds/github.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.9.2/unstructured/ingest/cli/cmds/gitlab.py` & `unstructured-0.9.3/unstructured/ingest/cli/cmds/gitlab.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.9.2/unstructured/ingest/cli/cmds/google_drive.py` & `unstructured-0.9.3/unstructured/ingest/cli/cmds/google_drive.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.9.2/unstructured/ingest/cli/cmds/local.py` & `unstructured-0.9.3/unstructured/ingest/cli/cmds/local.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.9.2/unstructured/ingest/cli/cmds/notion.py` & `unstructured-0.9.3/unstructured/ingest/cli/cmds/notion.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.9.2/unstructured/ingest/cli/cmds/onedrive.py` & `unstructured-0.9.3/unstructured/ingest/cli/cmds/onedrive.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.9.2/unstructured/ingest/cli/cmds/outlook.py` & `unstructured-0.9.3/unstructured/ingest/cli/cmds/outlook.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.9.2/unstructured/ingest/cli/cmds/reddit.py` & `unstructured-0.9.3/unstructured/ingest/cli/cmds/reddit.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.9.2/unstructured/ingest/cli/cmds/s3.py` & `unstructured-0.9.3/unstructured/ingest/cli/cmds/s3.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.9.2/unstructured/ingest/cli/cmds/sharepoint.py` & `unstructured-0.9.3/unstructured/ingest/cli/cmds/sharepoint.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.9.2/unstructured/ingest/cli/cmds/slack.py` & `unstructured-0.9.3/unstructured/ingest/cli/cmds/slack.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.9.2/unstructured/ingest/cli/cmds/wikipedia.py` & `unstructured-0.9.3/unstructured/ingest/cli/cmds/wikipedia.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.9.2/unstructured/ingest/cli/common.py` & `unstructured-0.9.3/unstructured/ingest/cli/common.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.9.2/unstructured/ingest/connector/azure.py` & `unstructured-0.9.3/unstructured/ingest/connector/azure.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.9.2/unstructured/ingest/connector/biomed.py` & `unstructured-0.9.3/unstructured/ingest/connector/biomed.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.9.2/unstructured/ingest/connector/box.py` & `unstructured-0.9.3/unstructured/ingest/connector/box.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.9.2/unstructured/ingest/connector/confluence.py` & `unstructured-0.9.3/unstructured/ingest/connector/confluence.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.9.2/unstructured/ingest/connector/discord.py` & `unstructured-0.9.3/unstructured/ingest/connector/discord.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.9.2/unstructured/ingest/connector/dropbox.py` & `unstructured-0.9.3/unstructured/ingest/connector/dropbox.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.9.2/unstructured/ingest/connector/elasticsearch.py` & `unstructured-0.9.3/unstructured/ingest/connector/elasticsearch.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.9.2/unstructured/ingest/connector/fsspec.py` & `unstructured-0.9.3/unstructured/ingest/connector/fsspec.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.9.2/unstructured/ingest/connector/gcs.py` & `unstructured-0.9.3/unstructured/ingest/connector/gcs.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.9.2/unstructured/ingest/connector/git.py` & `unstructured-0.9.3/unstructured/ingest/connector/git.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.9.2/unstructured/ingest/connector/github.py` & `unstructured-0.9.3/unstructured/ingest/connector/github.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.9.2/unstructured/ingest/connector/gitlab.py` & `unstructured-0.9.3/unstructured/ingest/connector/gitlab.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.9.2/unstructured/ingest/connector/google_drive.py` & `unstructured-0.9.3/unstructured/ingest/connector/google_drive.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.9.2/unstructured/ingest/connector/local.py` & `unstructured-0.9.3/unstructured/ingest/connector/local.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.9.2/unstructured/ingest/connector/notion/client.py` & `unstructured-0.9.3/unstructured/ingest/connector/notion/client.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.9.2/unstructured/ingest/connector/notion/connector.py` & `unstructured-0.9.3/unstructured/ingest/connector/notion/connector.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.9.2/unstructured/ingest/connector/notion/helpers.py` & `unstructured-0.9.3/unstructured/ingest/connector/notion/helpers.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.9.2/unstructured/ingest/connector/notion/interfaces.py` & `unstructured-0.9.3/unstructured/ingest/connector/notion/interfaces.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.9.2/unstructured/ingest/connector/onedrive.py` & `unstructured-0.9.3/unstructured/ingest/connector/onedrive.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.9.2/unstructured/ingest/connector/outlook.py` & `unstructured-0.9.3/unstructured/ingest/connector/outlook.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.9.2/unstructured/ingest/connector/reddit.py` & `unstructured-0.9.3/unstructured/ingest/connector/reddit.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.9.2/unstructured/ingest/connector/s3.py` & `unstructured-0.9.3/unstructured/ingest/connector/s3.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.9.2/unstructured/ingest/connector/sharepoint.py` & `unstructured-0.9.3/unstructured/ingest/connector/sharepoint.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.9.2/unstructured/ingest/connector/slack.py` & `unstructured-0.9.3/unstructured/ingest/connector/slack.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.9.2/unstructured/ingest/connector/wikipedia.py` & `unstructured-0.9.3/unstructured/ingest/connector/wikipedia.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.9.2/unstructured/ingest/doc_processor/generalized.py` & `unstructured-0.9.3/unstructured/ingest/doc_processor/generalized.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.9.2/unstructured/ingest/interfaces.py` & `unstructured-0.9.3/unstructured/ingest/interfaces.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.9.2/unstructured/ingest/logger.py` & `unstructured-0.9.3/unstructured/ingest/logger.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.9.2/unstructured/ingest/processor.py` & `unstructured-0.9.3/unstructured/ingest/processor.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.9.2/unstructured/ingest/runner/__init__.py` & `unstructured-0.9.3/unstructured/ingest/runner/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from .airtable import airtable
 from .azure import azure
 from .biomed import biomed
 from .box import box
 from .confluence import confluence
 from .discord import discord
 from .dropbox import dropbox
 from .elasticsearch import elasticsearch
@@ -17,14 +18,15 @@
 from .reddit import reddit
 from .s3 import s3
 from .sharepoint import sharepoint
 from .slack import slack
 from .wikipedia import wikipedia
 
 __all__ = [
+    "airtable",
     "azure",
     "biomed",
     "box",
     "confluence",
     "discord",
     "dropbox",
     "elasticsearch",
```

### Comparing `unstructured-0.9.2/unstructured/ingest/runner/azure.py` & `unstructured-0.9.3/unstructured/ingest/runner/azure.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.9.2/unstructured/ingest/runner/biomed.py` & `unstructured-0.9.3/unstructured/ingest/runner/biomed.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.9.2/unstructured/ingest/runner/box.py` & `unstructured-0.9.3/unstructured/ingest/runner/box.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.9.2/unstructured/ingest/runner/confluence.py` & `unstructured-0.9.3/unstructured/ingest/runner/confluence.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.9.2/unstructured/ingest/runner/discord.py` & `unstructured-0.9.3/unstructured/ingest/runner/discord.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.9.2/unstructured/ingest/runner/dropbox.py` & `unstructured-0.9.3/unstructured/ingest/runner/dropbox.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.9.2/unstructured/ingest/runner/elasticsearch.py` & `unstructured-0.9.3/unstructured/ingest/runner/elasticsearch.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.9.2/unstructured/ingest/runner/fsspec.py` & `unstructured-0.9.3/unstructured/ingest/runner/fsspec.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.9.2/unstructured/ingest/runner/gcs.py` & `unstructured-0.9.3/unstructured/ingest/runner/gcs.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.9.2/unstructured/ingest/runner/github.py` & `unstructured-0.9.3/unstructured/ingest/runner/github.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.9.2/unstructured/ingest/runner/gitlab.py` & `unstructured-0.9.3/unstructured/ingest/runner/gitlab.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.9.2/unstructured/ingest/runner/google_drive.py` & `unstructured-0.9.3/unstructured/ingest/runner/google_drive.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.9.2/unstructured/ingest/runner/local.py` & `unstructured-0.9.3/unstructured/ingest/runner/local.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.9.2/unstructured/ingest/runner/notion.py` & `unstructured-0.9.3/unstructured/ingest/runner/notion.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.9.2/unstructured/ingest/runner/onedrive.py` & `unstructured-0.9.3/unstructured/ingest/runner/onedrive.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.9.2/unstructured/ingest/runner/outlook.py` & `unstructured-0.9.3/unstructured/ingest/runner/outlook.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.9.2/unstructured/ingest/runner/reddit.py` & `unstructured-0.9.3/unstructured/ingest/runner/reddit.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.9.2/unstructured/ingest/runner/s3.py` & `unstructured-0.9.3/unstructured/ingest/runner/s3.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.9.2/unstructured/ingest/runner/sharepoint.py` & `unstructured-0.9.3/unstructured/ingest/runner/sharepoint.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.9.2/unstructured/ingest/runner/slack.py` & `unstructured-0.9.3/unstructured/ingest/runner/slack.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.9.2/unstructured/ingest/runner/utils.py` & `unstructured-0.9.3/unstructured/ingest/runner/utils.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.9.2/unstructured/ingest/runner/wikipedia.py` & `unstructured-0.9.3/unstructured/ingest/runner/wikipedia.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.9.2/unstructured/nlp/english-words.txt` & `unstructured-0.9.3/unstructured/nlp/english-words.txt`

 * *Files identical despite different names*

### Comparing `unstructured-0.9.2/unstructured/nlp/english_words.py` & `unstructured-0.9.3/unstructured/nlp/english_words.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.9.2/unstructured/nlp/patterns.py` & `unstructured-0.9.3/unstructured/nlp/patterns.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.9.2/unstructured/nlp/tokenize.py` & `unstructured-0.9.3/unstructured/nlp/tokenize.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.9.2/unstructured/partition/api.py` & `unstructured-0.9.3/unstructured/partition/api.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.9.2/unstructured/partition/auto.py` & `unstructured-0.9.3/unstructured/partition/auto.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,16 +30,19 @@
     from unstructured.partition.docx import partition_docx
 
 
 if dependency_exists("docx") and dependency_exists("pypandoc"):
     from unstructured.partition.odt import partition_odt
 
 
-if dependency_exists("pypandoc"):
+if dependency_exists("ebooklib"):
     from unstructured.partition.epub import partition_epub
+
+
+if dependency_exists("pypandoc"):
     from unstructured.partition.org import partition_org
     from unstructured.partition.rst import partition_rst
     from unstructured.partition.rtf import partition_rtf
 
 
 if dependency_exists("markdown"):
     from unstructured.partition.md import partition_md
```

### Comparing `unstructured-0.9.2/unstructured/partition/common.py` & `unstructured-0.9.3/unstructured/partition/common.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import os
 import subprocess
 from datetime import datetime
 from io import BufferedReader, BytesIO, TextIOWrapper
 from tempfile import SpooledTemporaryFile
 from typing import IO, TYPE_CHECKING, Any, BinaryIO, Dict, List, Optional, Tuple, Union
 
+import emoji
 from tabulate import tabulate
 
 from unstructured.documents.coordinates import CoordinateSystem
 from unstructured.documents.elements import (
     TYPE_TO_TEXT_ELEMENT_MAP,
     CheckBox,
     CoordinatesMetadata,
@@ -146,14 +147,16 @@
     filename: Optional[str] = None,
     filetype: Optional[str] = None,
     page_number: Optional[int] = None,
     url: Optional[str] = None,
     text_as_html: Optional[str] = None,
     coordinates: Optional[Tuple[Tuple[float, float], ...]] = None,
     coordinate_system: Optional[CoordinateSystem] = None,
+    section: Optional[str] = None,
+    **kwargs,
 ) -> Element:
     """Adds document metadata to the document element. Document metadata includes information
     like the filename, source url, and page number."""
     coordinates_metadata = (
         CoordinatesMetadata(
             points=coordinates,
             system=coordinate_system,
@@ -172,14 +175,15 @@
         filename=filename,
         filetype=filetype,
         page_number=page_number,
         url=url,
         text_as_html=text_as_html,
         links=links,
         emphasized_texts=emphasized_texts,
+        section=section,
     )
     element.metadata = metadata.merge(element.metadata)
     return element
 
 
 def _remove_element_metadata(
     layout_elements,
@@ -329,7 +333,21 @@
     if len(rows) > 0:
         headers = [cell.text for cell in rows[0].cells]
         data = [[cell.text for cell in row.cells] for row in rows[1:]]
         table_text = tabulate(data, headers=headers, tablefmt=fmt)
     else:
         table_text = ""
     return table_text
+
+
+def contains_emoji(s: str) -> bool:
+    """
+    Check if the input string contains any emoji characters.
+
+    Parameters:
+    - s (str): The input string to check.
+
+    Returns:
+    - bool: True if the string contains any emoji, False otherwise.
+    """
+
+    return bool(emoji.emoji_count(s))
```

### Comparing `unstructured-0.9.2/unstructured/partition/csv.py` & `unstructured-0.9.3/unstructured/partition/csv.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from tempfile import SpooledTemporaryFile
 from typing import IO, BinaryIO, List, Optional, Union, cast
 
-import lxml.html
 import pandas as pd
+from lxml.html.soupparser import fromstring as soupparser_fromstring
 
 from unstructured.documents.elements import (
     Element,
     ElementMetadata,
     Table,
     process_metadata,
 )
@@ -54,15 +54,15 @@
         last_modification_date = get_last_modified_date_from_file(file)
         f = spooled_to_bytes_io_if_needed(
             cast(Union[BinaryIO, SpooledTemporaryFile], file),
         )
         table = pd.read_csv(f)
 
     html_text = table.to_html(index=False, header=False, na_rep="")
-    text = lxml.html.document_fromstring(html_text).text_content()
+    text = soupparser_fromstring(html_text).text_content()
 
     if include_metadata:
         metadata = ElementMetadata(
             text_as_html=html_text,
             filename=metadata_filename or filename,
             last_modified=metadata_last_modified or last_modification_date,
         )
```

### Comparing `unstructured-0.9.2/unstructured/partition/doc.py` & `unstructured-0.9.3/unstructured/partition/doc.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.9.2/unstructured/partition/docx.py` & `unstructured-0.9.3/unstructured/partition/docx.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.9.2/unstructured/partition/email.py` & `unstructured-0.9.3/unstructured/partition/email.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import datetime
 import email
 import os
 import re
 import sys
 from email.message import Message
 from functools import partial
-from tempfile import SpooledTemporaryFile, TemporaryDirectory
+from tempfile import NamedTemporaryFile, SpooledTemporaryFile, TemporaryDirectory
 from typing import IO, Callable, Dict, List, Optional, Tuple, Union
 
 from unstructured.file_utils.encoding import (
     COMMON_ENCODINGS,
     format_encoding_str,
     read_txt_file,
     validate_encoding,
@@ -159,35 +159,44 @@
     list_attachments = []
 
     for part in message.walk():
         if "content-disposition" in part:
             cdisp = part["content-disposition"].split(";")
             cdisp = [clean_extra_whitespace(item) for item in cdisp]
 
+            attachment_info = {}
             for item in cdisp:
-                attachment_info = {}
-
-                if item.lower() == "attachment":
+                if item.lower() in ("attachment", "inline"):
                     continue
-                key, value = item.split("=")
+                key, value = item.split("=", 1)
                 key = clean_extra_whitespace(key.replace('"', ""))
                 value = clean_extra_whitespace(value.replace('"', ""))
                 attachment_info[clean_extra_whitespace(key)] = clean_extra_whitespace(
                     value,
                 )
             attachment_info["payload"] = part.get_payload(decode=True)
             list_attachments.append(attachment_info)
 
-            for attachment in list_attachments:
+            for idx, attachment in enumerate(list_attachments):
                 if output_dir:
-                    filename = output_dir + "/" + attachment["filename"]
-                    with open(filename, "wb") as f:
-                        # Note(harrell) mypy wants to just us `w` when opening the file but this
-                        # causes an error since the payloads are bytes not str
-                        f.write(attachment["payload"])  # type: ignore
+                    if "filename" in attachment:
+                        filename = output_dir + "/" + attachment["filename"]
+                        with open(filename, "wb") as f:
+                            # Note(harrell) mypy wants to just us `w` when opening the file but this
+                            # causes an error since the payloads are bytes not str
+                            f.write(attachment["payload"])  # type: ignore
+                    else:
+                        with NamedTemporaryFile(
+                            mode="wb",
+                            dir=output_dir,
+                            delete=False,
+                        ) as f:
+                            list_attachments[idx]["filename"] = os.path.basename(f.name)
+                            f.write(attachment["payload"])  # type: ignore
+
     return list_attachments
 
 
 def has_embedded_image(element):
     PATTERN = re.compile("\[image: .+\]")  # noqa: W605 NOTE(harrell)
     return PATTERN.search(element.text)
```

### Comparing `unstructured-0.9.2/unstructured/partition/epub.py` & `unstructured-0.9.3/unstructured/partition/rst.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,40 +2,39 @@
 
 from unstructured.documents.elements import Element, process_metadata
 from unstructured.file_utils.filetype import FileType, add_metadata_with_filetype
 from unstructured.partition.html import convert_and_partition_html
 
 
 @process_metadata()
-@add_metadata_with_filetype(FileType.EPUB)
-def partition_epub(
+@add_metadata_with_filetype(FileType.RST)
+def partition_rst(
     filename: Optional[str] = None,
     file: Optional[IO[bytes]] = None,
     include_page_breaks: bool = False,
     include_metadata: bool = True,
     metadata_filename: Optional[str] = None,
     metadata_last_modified: Optional[str] = None,
     **kwargs,
 ) -> List[Element]:
-    """Partitions an EPUB document. The document is first converted to HTML and then
-    partitoned using partiton_html.
+    """Partitions an RST document. The document is first converted to HTML and then
+    partitioned using partition_html.
 
     Parameters
     ----------
     filename
         A string defining the target filename path.
     file
         A file-like object using "rb" mode --> open(filename, "rb").
     include_page_breaks
-        If True, the output will include page breaks if the filetype supports it
+        If True, the output will include page breaks if the filetype supports it.
     metadata_last_modified
         The last modified date for the document.
-
     """
     return convert_and_partition_html(
-        source_format="epub",
+        source_format="rst",
         filename=filename,
         file=file,
         include_page_breaks=include_page_breaks,
         metadata_filename=metadata_filename,
         metadata_last_modified=metadata_last_modified,
     )
```

### Comparing `unstructured-0.9.2/unstructured/partition/html.py` & `unstructured-0.9.3/unstructured/partition/html.py`

 * *Files 1% similar despite different names*

```diff
@@ -119,14 +119,15 @@
     if skip_headers_and_footers:
         document = filter_footer_and_header(document)
 
     return document_to_element_list(
         document,
         include_page_breaks=include_page_breaks,
         last_modification_date=metadata_last_modified or last_modification_date,
+        **kwargs,
     )
 
 
 def convert_and_partition_html(
     source_format: str,
     filename: Optional[str] = None,
     file: Optional[IO[bytes]] = None,
@@ -145,15 +146,15 @@
         A string defining the target filename path.
     file
         A file-like object using "rb" mode --> open(filename, "rb").
     include_page_breaks
         If True, the output will include page breaks if the filetype supports it.
     metadata_filename
         The filename to use in element metadata.
-    last_modication_date
+    metadata_last_modified
         The last modified date for the document.
     """
 
     last_modification_date = None
     if filename:
         last_modification_date = get_last_modified_date(filename)
     elif file:
```

### Comparing `unstructured-0.9.2/unstructured/partition/image.py` & `unstructured-0.9.3/unstructured/partition/image.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.9.2/unstructured/partition/json.py` & `unstructured-0.9.3/unstructured/partition/json.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.9.2/unstructured/partition/md.py` & `unstructured-0.9.3/unstructured/partition/md.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.9.2/unstructured/partition/msg.py` & `unstructured-0.9.3/unstructured/partition/msg.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.9.2/unstructured/partition/odt.py` & `unstructured-0.9.3/unstructured/partition/odt.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.9.2/unstructured/partition/org.py` & `unstructured-0.9.3/unstructured/partition/org.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.9.2/unstructured/partition/pdf.py` & `unstructured-0.9.3/unstructured/partition/pdf.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.9.2/unstructured/partition/ppt.py` & `unstructured-0.9.3/unstructured/partition/ppt.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.9.2/unstructured/partition/pptx.py` & `unstructured-0.9.3/unstructured/partition/pptx.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.9.2/unstructured/partition/rst.py` & `unstructured-0.9.3/unstructured/partition/rtf.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,39 +2,39 @@
 
 from unstructured.documents.elements import Element, process_metadata
 from unstructured.file_utils.filetype import FileType, add_metadata_with_filetype
 from unstructured.partition.html import convert_and_partition_html
 
 
 @process_metadata()
-@add_metadata_with_filetype(FileType.RST)
-def partition_rst(
+@add_metadata_with_filetype(FileType.RTF)
+def partition_rtf(
     filename: Optional[str] = None,
     file: Optional[IO[bytes]] = None,
     include_page_breaks: bool = False,
     include_metadata: bool = True,
     metadata_filename: Optional[str] = None,
     metadata_last_modified: Optional[str] = None,
     **kwargs,
 ) -> List[Element]:
-    """Partitions an RST document. The document is first converted to HTML and then
+    """Partitions an RTF document. The document is first converted to HTML and then
     partitioned using partition_html.
 
     Parameters
     ----------
     filename
         A string defining the target filename path.
     file
         A file-like object using "rb" mode --> open(filename, "rb").
     include_page_breaks
-        If True, the output will include page breaks if the filetype supports it.
+        If True, the output will include page breaks if the filetype supports it
     metadata_last_modified
         The last modified date for the document.
     """
     return convert_and_partition_html(
-        source_format="rst",
+        source_format="rtf",
         filename=filename,
         file=file,
         include_page_breaks=include_page_breaks,
         metadata_filename=metadata_filename,
         metadata_last_modified=metadata_last_modified,
     )
```

### Comparing `unstructured-0.9.2/unstructured/partition/rtf.py` & `unstructured-0.9.3/unstructured/partition/tsv.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,40 +1,69 @@
-from typing import IO, List, Optional
+from tempfile import SpooledTemporaryFile
+from typing import IO, BinaryIO, List, Optional, Union, cast
 
-from unstructured.documents.elements import Element, process_metadata
+import pandas as pd
+from lxml.html.soupparser import fromstring as soupparser_fromstring
+
+from unstructured.documents.elements import (
+    Element,
+    ElementMetadata,
+    Table,
+    process_metadata,
+)
 from unstructured.file_utils.filetype import FileType, add_metadata_with_filetype
-from unstructured.partition.html import convert_and_partition_html
+from unstructured.partition.common import (
+    exactly_one,
+    get_last_modified_date,
+    get_last_modified_date_from_file,
+    spooled_to_bytes_io_if_needed,
+)
 
 
 @process_metadata()
-@add_metadata_with_filetype(FileType.RTF)
-def partition_rtf(
+@add_metadata_with_filetype(FileType.TSV)
+def partition_tsv(
     filename: Optional[str] = None,
-    file: Optional[IO[bytes]] = None,
-    include_page_breaks: bool = False,
-    include_metadata: bool = True,
+    file: Optional[Union[IO[bytes], SpooledTemporaryFile]] = None,
     metadata_filename: Optional[str] = None,
     metadata_last_modified: Optional[str] = None,
+    include_metadata: bool = True,
     **kwargs,
 ) -> List[Element]:
-    """Partitions an RTF document. The document is first converted to HTML and then
-    partitioned using partiton_html.
+    """Partitions TSV files into document elements.
 
     Parameters
     ----------
     filename
         A string defining the target filename path.
     file
         A file-like object using "rb" mode --> open(filename, "rb").
-    include_page_breaks
-        If True, the output will include page breaks if the filetype supports it
+    include_metadata
+        Determines whether or not metadata is included in the output.
     metadata_last_modified
-        The last modified date for the document.
+        The day of the last modification
     """
-    return convert_and_partition_html(
-        source_format="rtf",
-        filename=filename,
-        file=file,
-        include_page_breaks=include_page_breaks,
-        metadata_filename=metadata_filename,
-        metadata_last_modified=metadata_last_modified,
-    )
+    exactly_one(filename=filename, file=file)
+    last_modification_date = None
+    if filename:
+        table = pd.read_csv(filename, sep="\t")
+        last_modification_date = get_last_modified_date(filename)
+    elif file:
+        f = spooled_to_bytes_io_if_needed(
+            cast(Union[BinaryIO, SpooledTemporaryFile], file),
+        )
+        table = pd.read_csv(f, sep="\t")
+        last_modification_date = get_last_modified_date_from_file(file)
+
+    html_text = table.to_html(index=False, header=False, na_rep="")
+    text = soupparser_fromstring(html_text).text_content()
+
+    if include_metadata:
+        metadata = ElementMetadata(
+            text_as_html=html_text,
+            filename=metadata_filename or filename,
+            last_modified=metadata_last_modified or last_modification_date,
+        )
+    else:
+        metadata = ElementMetadata()
+
+    return [Table(text=text, metadata=metadata)]
```

### Comparing `unstructured-0.9.2/unstructured/partition/strategies.py` & `unstructured-0.9.3/unstructured/partition/strategies.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.9.2/unstructured/partition/text.py` & `unstructured-0.9.3/unstructured/partition/text.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.9.2/unstructured/partition/text_type.py` & `unstructured-0.9.3/unstructured/partition/text_type.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.9.2/unstructured/partition/xlsx.py` & `unstructured-0.9.3/unstructured/partition/xlsx.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,31 +1,26 @@
 from tempfile import SpooledTemporaryFile
 from typing import IO, BinaryIO, List, Optional, Union, cast
 
 import pandas as pd
+from lxml.html.soupparser import fromstring as soupparser_fromstring
 
 from unstructured.documents.elements import (
     Element,
     ElementMetadata,
     Table,
     process_metadata,
 )
 from unstructured.file_utils.filetype import FileType, add_metadata_with_filetype
 from unstructured.partition.common import (
     exactly_one,
     get_last_modified_date,
     get_last_modified_date_from_file,
     spooled_to_bytes_io_if_needed,
 )
-from unstructured.utils import dependency_exists
-
-if dependency_exists("bs4"):
-    from lxml.html.soupparser import fromstring as html_string_parser
-else:
-    from lxml.html import document_fromstring as html_string_parser
 
 
 @process_metadata()
 @add_metadata_with_filetype(FileType.XLSX)
 def partition_xlsx(
     filename: Optional[str] = None,
     file: Optional[Union[IO[bytes], SpooledTemporaryFile]] = None,
@@ -61,15 +56,15 @@
         last_modification_date = get_last_modified_date_from_file(file)
 
     elements: List[Element] = []
     page_number = 0
     for sheet_name, table in sheets.items():
         page_number += 1
         html_text = table.to_html(index=False, header=False, na_rep="")
-        text = html_string_parser(html_text).text_content()
+        text = soupparser_fromstring(html_text).text_content()
 
         if include_metadata:
             metadata = ElementMetadata(
                 text_as_html=html_text,
                 page_name=sheet_name,
                 page_number=page_number,
                 filename=metadata_filename or filename,
```

### Comparing `unstructured-0.9.2/unstructured/partition/xml.py` & `unstructured-0.9.3/unstructured/partition/xml.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.9.2/unstructured/staging/argilla.py` & `unstructured-0.9.3/unstructured/staging/argilla.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.9.2/unstructured/staging/base.py` & `unstructured-0.9.3/unstructured/staging/base.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.9.2/unstructured/staging/baseplate.py` & `unstructured-0.9.3/unstructured/staging/baseplate.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.9.2/unstructured/staging/datasaur.py` & `unstructured-0.9.3/unstructured/staging/datasaur.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.9.2/unstructured/staging/huggingface.py` & `unstructured-0.9.3/unstructured/staging/huggingface.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.9.2/unstructured/staging/label_box.py` & `unstructured-0.9.3/unstructured/staging/label_box.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.9.2/unstructured/staging/label_studio.py` & `unstructured-0.9.3/unstructured/staging/label_studio.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.9.2/unstructured/staging/prodigy.py` & `unstructured-0.9.3/unstructured/staging/prodigy.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.9.2/unstructured/staging/weaviate.py` & `unstructured-0.9.3/unstructured/staging/weaviate.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.9.2/unstructured/utils.py` & `unstructured-0.9.3/unstructured/utils.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.9.2/unstructured.egg-info/PKG-INFO` & `unstructured-0.9.3/unstructured.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unstructured
-Version: 0.9.2
+Version: 0.9.3
 Summary: A library that prepares raw documents for downstream ML tasks.
 Home-page: https://github.com/Unstructured-IO/unstructured
 Author: Unstructured Technologies
 Author-email: devops@unstructuredai.io
 License: Apache-2.0
 Description: <h3 align="center">
           <img
@@ -33,57 +33,44 @@
             <img src="https://img.shields.io/badge/JOIN US ON SLACK-4A154B?style=for-the-badge&logo=slack&logoColor=white" />
           </a>
           <a href="https://www.linkedin.com/company/unstructuredio/">
             <img src="https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white" />
           </a>
         </div>
         
+        <h2 align="center">
+          <p>Open-Source Pre-Processing Tools for Unstructured Data</p>
+        </h2>
+        
+        The `unstructured` library provides open-source components for ingesting and pre-processing images and text documents, such as PDFs, HTML, Word docs, and [many more](https://unstructured-io.github.io/unstructured/bricks.html#partitioning). The use cases of `unstructured` revolve around streamlining and optimizing the data processing workflow for LLMs. `unstructured` modular bricks and connectors form a cohesive system that simplifies data ingestion and pre-processing, making it adaptable to different platforms and is efficient in transforming unstructured data into structured outputs.
+        
         <h3 align="center">
           <p>API Announcement!</p>
         </h3>
         
-        We are thrilled to announce our newly launched [Unstructured API](https://unstructured-io.github.io/unstructured/api.html). While access to the hosted Unstructured API will remain free, API Keys are required to make requests. To prevent disruption, get yours [here](https://unstructured.io/#get-api-key) now and start using it today! Check out the [readme](https://github.com/Unstructured-IO/unstructured-api#--) here to get started making API calls.</p>
+        We are thrilled to announce our newly launched [Unstructured API](https://unstructured-io.github.io/unstructured/api.html), providing the Unstructured capabilities from `unstructured` as an API. Check out the [`unstructured-api` GitHub repository](https://github.com/Unstructured-IO/unstructured-api) to start making API calls. You’ll also find instructions about how to host your own API version.
+        
+        While access to the hosted Unstructured API will remain free, API Keys are required to make requests. To prevent disruption, get yours [here](https://unstructured.io/#get-api-key) and start using it today! Check out the [`unstructured-api` README](https://github.com/Unstructured-IO/unstructured-api#--) to start making API calls.</p>
         
         #### :rocket: Beta Feature: Chipper Model
         
-        We are releasing the beta version of our Chipper model to deliver superior performance when processing high-resolution, complex documents. To start using the Chipper model in your API request, you can utilize the `hi_res` strategy. Please refer to the documentation [here](https://unstructured-io.github.io/unstructured/api.html#strategies).
+        We are releasing the beta version of our Chipper model to deliver superior performance when processing high-resolution, complex documents. To start using the Chipper model in your API request, you can utilize the `hi_res_model_name=chipper` parameter. Please refer to the documentation [here](https://unstructured-io.github.io/unstructured/api.html#beta-version-hi-res-strategy-with-chipper-model).
         
         As the Chipper model is in beta version, we welcome feedback and suggestions. For those interested in testing the Chipper model, we encourage you to connect with us on [Slack community](https://join.slack.com/t/unstructuredw-kbe4326/shared_invite/zt-1x7cgo0pg-PTptXWylzPQF9xZolzCnwQ).
         
-        <h3 align="center">
-          <p>Open-Source Pre-Processing Tools for Unstructured Data</p>
-        </h3>
-        
-        The `unstructured` library provides open-source components for pre-processing text documents
-        such as **PDFs**, **HTML** and **Word** Documents. These components are packaged as *bricks* 🧱, which provide
-        users the building blocks they need to build pipelines targeted at the documents they care
-        about. Bricks in the library fall into three categories:
-        
-        - :jigsaw: ***Partitioning bricks*** that break raw documents down into standard, structured
-          elements.
-        - :broom: ***Cleaning bricks*** that remove unwanted text from documents, such as boilerplate and
-          sentence
-          fragments.
-        - :performing_arts: ***Staging bricks*** that format data for downstream tasks, such as ML inference
-          and data labeling.
-        
-        Unstructured also provides the capabilities from `unstructured` as an API.
-        Checkout the [`unstructured-api` repo](https://github.com/Unstructured-IO/unstructured-api)
-        to get started making API calls.
-        You’ll also find instructions there about how to host your own version of the API.
-        
-        ## :bookmark: Documentation
-        This README gives an overview of how to install, use and develop the library.
-        For more comprehensive documentation, visit https://unstructured-io.github.io/unstructured/ .
-        
         ## :eight_pointed_black_star: Quick Start
         
-        There are two ways to use the library: 1) run a container or 2) install it
+        There are several ways to use the `unstructured` library:
+        * [Run the library in a container](https://github.com/Unstructured-IO/unstructured#using-the-library-in-a-container) or
+        * Install the library
+            1. [Install from PyPI](https://github.com/Unstructured-IO/unstructured#installing-the-library)
+            2. [Install for local development](https://github.com/Unstructured-IO/unstructured#coffee-installation-instructions-for-local-development)
+        * For installation with `conda` on Windows system, please refer to the [documentation](https://unstructured-io.github.io/unstructured/installing.html#installation-with-conda-on-windows)
         
-        ### Using the library in a container
+        ### Run the library in a container
         
         The following instructions are intended to help you get up and running using Docker to interact with `unstructured`.
         See [here](https://docs.docker.com/get-docker/) if you don't already have docker installed on your machine.
         
         NOTE: we build multi-platform images to support both x86_64 and Apple silicon hardware. `docker pull` should download the corresponding image for your architecture, but you can specify with `--platform` (e.g. `--platform linux/amd64`) if needed.
         
         We build Docker images for all pushes to `main`. We tag each image with the corresponding short commit hash (e.g. `fbc7a69`) and the application version (e.g. `0.5.5-dev1`). We also tag the most recent image with `latest`. To leverage this, `docker pull` from our image repository.
@@ -111,15 +98,15 @@
         ```bash
         make docker-build
         
         # this will drop you into a bash shell where the Docker image is running
         make docker-start-bash
         ```
         
-        Once in the running container, you can try things out directly in Python interpreter's interactive mode.
+        Once in the running container, you can try things directly in Python interpreter's interactive mode.
         ```bash
         # this will drop you into a python console so you can run the below partition functions
         python3
         
         >>> from unstructured.partition.pdf import partition_pdf
         >>> elements = partition_pdf(filename="example-docs/layout-parser-paper-fast.pdf")
         
@@ -127,69 +114,38 @@
         >>> elements = partition_text(filename="example-docs/fake-text.txt")
         ```
         
         ### Installing the library
         Use the following instructions to get up and running with `unstructured` and test your
         installation.
         
-        - Install the Python SDK with `pip install "unstructured[local-inference]"`
-        		- If you do not need to process PDFs or images, you can run `pip install unstructured`
+        - Install the Python SDK to support all document types with `pip install "unstructured[all-docs]"`
+          - For plain text files, HTML, XML, JSON and Emails that do not require any extra dependencies, you can run `pip install unstructured`
+          - To process other doc types, you can install the extras required for those documents, such as `pip install "unstructured[docx,pptx]"`
         - Install the following system dependencies if they are not already available on your system.
           Depending on what document types you're parsing, you may not need all of these.
             - `libmagic-dev` (filetype detection)
             - `poppler-utils` (images and PDFs)
             - `tesseract-ocr` (images and PDFs)
             - `libreoffice` (MS Office docs)
             - `pandoc` (EPUBs, RTFs and Open Office docs)
         
-        - For suggestions on how to install on Windows and to learn about dependencies for other features, see the
+        - For suggestions on how to install on the Windows and to learn about dependencies for other features, see the
           installation documentation [here](https://unstructured-io.github.io/unstructured/installing.html).
         
         At this point, you should be able to run the following code:
         
         ```python
         from unstructured.partition.auto import partition
         
         elements = partition(filename="example-docs/eml/fake-email.eml")
         print("\n\n".join([str(el) for el in elements]))
         ```
         
-        The following table shows the document types the `unstructured` library currently supports.
-        `partition` will recognize each of these document types and route the document to the
-        appropriate partitioning function. If you already know your document type, you can use
-        the partitioning function listed in the table directly.
-        See our [documentation page](https://unstructured-io.github.io/unstructured/) for more details
-        about the library.
-        
-        | Document Type | Partition Function | Strategies | Table Support | Options |
-        | --- | --- | --- | --- | --- |
-        | CSV Files (`.csv`) | `partition_csv` | N/A | Yes | None |
-        | E-mails (`.eml`) | `partition_eml` | N/A | No | Encoding; Max Partition; Process Attachments |
-        | E-mails (`.msg`) | `partition_msg` | N/A | No | Encoding; Max Partition; Process Attachments |
-        | EPubs (`.epub`) | `partition_epub` | N/A | Yes | Include Page Breaks |
-        | Excel Documents (`.xlsx`/`.xls`) | `partition_xlsx` | N/A | Yes | None |
-        | HTML Pages (`.html`) | `partition_html` | N/A | No | Encoding; Include Page Breaks |
-        | Images (`.png`/`.jpg`) | `partition_image` | `"auto"`, `"hi_res"`, `"ocr_only"` | Yes | Encoding; Include Page Breaks; Infer Table Structure; OCR Languages, Strategy |
-        | Markdown (`.md`) | `partitin_md` | N/A | Yes | Include Page Breaks |
-        | Org Mode (`.org`) | `partition_org` | N/A | Yes | Include Page Breaks |
-        | Open Office Documents (`.odt`) | `partition_odt` | N/A | Yes | None |
-        | PDFs (`.pdf`) | `partition_pdf` | `"auto"`, `"fast"`, `"hi_res"`, `"ocr_only"` | Yes | Encoding; Include Page Breaks; Infer Table Structure; Max Partition; OCR Languages, Strategy |
-        | Plain Text (`.txt`) | `partition_text` | N/A | No | Encoding; Max Partition; Paragraph Grouper |
-        | Power Points (`.ppt`) | `partition_ppt` | N/A | Yes | Include Page Breaks |
-        | Power Points (`.pptx`) | `partition_pptx` | N/A | Yes | Include Page Breaks |
-        | ReStructured Text (`.rst`) | `partition_rst` | N/A | Yes | Include Page Breaks |
-        | Rich Text Files (`.rtf`) | `partition_rtf` | N/A | Yes | Include Page Breaks |
-        | TSV Files (`.tsv`) | `partition_tsv` | N/A | Yes | None |
-        | Word Documents (`.doc`) | `partition_doc` | N/A | Yes | Include Page Breaks |
-        | Word Documents (`.docx`) | `partition_docx` | N/A | Yes | Include Page Breaks |
-        | XML Documents (`.xml`) | `partition_xml` | N/A | No | Encoding; Max Partition; XML Keep Tags |
-        
-        
-        
-        ## :coffee: Installation Instructions for Local Development
+        ### Installation Instructions for Local Development
         
         The following instructions are intended to help you get up and running with `unstructured`
         locally if you are planning to contribute to the project.
         
         * Using `pyenv` to manage virtualenv's is recommended but not necessary
         	* Mac install instructions. See [here](https://github.com/Unstructured-IO/community#mac--homebrew) for more detailed instructions.
         		* `brew install pyenv-virtualenv`
@@ -206,41 +162,41 @@
         * Optional:
           * To install models and dependencies for processing images and PDFs locally, run `make install-local-inference`.
           * For processing image files, `tesseract` is required. See [here](https://tesseract-ocr.github.io/tessdoc/Installation.html) for installation instructions.
           * For processing PDF files, `tesseract` and `poppler` are required. The [pdf2image docs](https://pdf2image.readthedocs.io/en/latest/installation.html) have instructions on installing `poppler` across various platforms.
         
         Additionally, if you're planning to contribute to `unstructured`, we provide you an optional `pre-commit` configuration
         file to ensure your code matches the formatting and linting standards used in `unstructured`.
-        If you'd prefer not having code changes auto-tidied before every commit, you can use  `make check` to see
+        If you'd prefer not to have code changes auto-tidied before every commit, you can use  `make check` to see
         whether any linting or formatting changes should be applied, and `make tidy` to apply them.
         
         If using the optional `pre-commit`, you'll just need to install the hooks with `pre-commit install` since the
         `pre-commit` package is installed as part of `make install` mentioned above. Finally, if you decided to use `pre-commit`
         you can also uninstall the hooks with `pre-commit uninstall`.
         
         ## :clap: Quick Tour
         
-        You can run this [Colab notebook](https://colab.research.google.com/drive/1U8VCjY2-x8c6y5TYMbSFtQGlQVFHCVIW) to run the examples below.
+        ### Documentation
+        This README overviews how to install, use and develop the library. For more comprehensive documentation, visit https://unstructured-io.github.io/unstructured/ .
+        
+        ### Concepts Guide
+        
+        **Bricks** 🧱 in `unstructured` are the foundational elements that drive the data processing workflow within the system. These components provide users with the building blocks to build pipelines targeted at the documents they care about. The bricks fall into three categories:
+        - :jigsaw: *Partitioning* bricks break raw documents into standard, structured elements.
+        - :broom: *Cleaning* bricks remove unwanted text from documents, such as boilerplate and sentence fragments.
+        - :performing_arts: *Staging* bricks format data for downstream tasks, such as ML inference and data labeling. 
+        
+        These bricks create a cohesive, streamlined process that enables effective data handling and analysis. Check out the available bricks and how to use them from the [Bricks documentation](https://unstructured-io.github.io/unstructured/bricks.html).
+        
+        The **Connectors** 🔗 in `unstructured` serve as vital links between the pre-processing pipeline and various data storage platforms. They allow for the batch processing of documents across various sources, including cloud services, repositories, and local directories. Each connector is tailored to a specific platform, such as Azure, Google Drive, or Github, and comes with unique commands and dependencies. To see the list of Connectors available in `unstructured` library, please check out the [Connectors GitHub folder](https://github.com/Unstructured-IO/unstructured/tree/main/unstructured/ingest/connector) and [documentation](https://unstructured-io.github.io/unstructured/connectors.html)
+        
+        ### PDF Document Parsing Example
+        The following examples show how to get started with the `unstructured` library. You can parse over a dozen document types with one line of code! Use this [Colab notebook](https://colab.research.google.com/drive/1U8VCjY2-x8c6y5TYMbSFtQGlQVFHCVIW) to run the example below.
         
-        The following examples show how to get started with the `unstructured` library.
-        You can parse over a dozen document types with one line of code!
-        <br></br>
-        See our [documentation page](https://unstructured-io.github.io/unstructured) for a full description
-        of the features in the library.
-        
-        ### Document Parsing
-        
-        The easiest way to parse a document in unstructured is to use the `partition` brick. If you
-        use `partition` brick, `unstructured` will detect the file type and route it to the appropriate
-        file-specific partitioning brick.
-        If you are using the `partition` brick, you may need to install additional parameters via `pip install unstructured[local-inference]`. Ensure you first install `libmagic` using the
-        instructions outlined [here](https://unstructured-io.github.io/unstructured/installing.html#filetype-detection)
-        `partition` will always apply the default arguments. If you need
-        advanced features, use a document-specific brick.
-        See the table above for a full list of document types supported in the library.
+        The easiest way to parse a document in unstructured is to use the `partition` brick. If you use `partition` brick, `unstructured` will detect the file type and route it to the appropriate file-specific partitioning brick. If you are using the `partition` brick, you may need to install additional parameters via `pip install unstructured[local-inference]`. Ensure you first install `libmagic` using the instructions outlined [here](https://unstructured-io.github.io/unstructured/installing.html#filetype-detection) `partition` will always apply the default arguments. If you need advanced features, use a document-specific brick.
         
         ```python
         from unstructured.partition.auto import partition
         
         elements = partition("example-docs/layout-parser-paper.pdf")
         ```
         
@@ -342,9 +298,11 @@
 Provides-Extra: gcs
 Provides-Extra: elasticsearch
 Provides-Extra: dropbox
 Provides-Extra: box
 Provides-Extra: onedrive
 Provides-Extra: outlook
 Provides-Extra: confluence
+Provides-Extra: airtable
+Provides-Extra: sharepoint
 Provides-Extra: huggingface
 Provides-Extra: local-inference
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: unstructured Version: 0.9.2 Summary: A library that
+Metadata-Version: 2.1 Name: unstructured Version: 0.9.3 Summary: A library that
 prepares raw documents for downstream ML tasks. Home-page: https://github.com/
 Unstructured-IO/unstructured Author: Unstructured Technologies Author-email:
 devops@unstructuredai.io License: Apache-2.0 Description:
 ******** [[hhttttppss::////rraaww..ggiitthhuubbuusseerrccoonntteenntt..ccoomm//UUnnssttrruuccttuurreedd--IIOO//uunnssttrruuccttuurreedd//mmaaiinn//iimmgg//
                           uunnssttrruuccttuurreedd__llooggoo..ppnngg]] ********
  _!_[_h_t_t_p_s_:_/_/_p_y_p_i_._p_y_t_h_o_n_._o_r_g_/_p_y_p_i_/_u_n_s_t_r_u_c_t_u_r_e_d_/_]_(_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_p_y_p_i_/_l_/
    _u_n_s_t_r_u_c_t_u_r_e_d_._s_v_g_) _!_[_h_t_t_p_s_:_/_/_p_y_p_i_._p_y_t_h_o_n_._o_r_g_/_p_y_p_i_/_u_n_s_t_r_u_c_t_u_r_e_d_/_]_(_h_t_t_p_s_:_/_/
@@ -15,192 +15,188 @@
 _b_a_d_g_e_s_/_]_(_h_t_t_p_s_:_/_/_b_a_d_g_e_n_._n_e_t_/_b_a_d_g_e_/_O_p_e_n_%_2_0_S_o_u_r_c_e_%_2_0_%_3_F_/_Y_e_s_%_2_1_/_b_l_u_e_?_i_c_o_n_=_g_i_t_h_u_b_)
 [![Downloads](https://static.pepy.tech/badge/unstructured)](https://pepy.tech/
       project/unstructured) [![Downloads](https://static.pepy.tech/badge/
          unstructured/month)](https://pepy.tech/project/unstructured)
      _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_J_O_I_N_ _U_S_ _O_N_ _S_L_A_C_K_-_4_A_1_5_4_B_?_s_t_y_l_e_=_f_o_r_-_t_h_e_-
    _b_a_d_g_e_&_l_o_g_o_=_s_l_a_c_k_&_l_o_g_o_C_o_l_o_r_=_w_h_i_t_e_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_L_i_n_k_e_d_I_n_-
            _0_0_7_7_B_5_?_s_t_y_l_e_=_f_o_r_-_t_h_e_-_b_a_d_g_e_&_l_o_g_o_=_l_i_n_k_e_d_i_n_&_l_o_g_o_C_o_l_o_r_=_w_h_i_t_e_]
+      ********** OOppeenn--SSoouurrccee PPrree--PPrroocceessssiinngg TToooollss ffoorr UUnnssttrruuccttuurreedd DDaattaa **********
+The `unstructured` library provides open-source components for ingesting and
+pre-processing images and text documents, such as PDFs, HTML, Word docs, and
+[many more](https://unstructured-io.github.io/unstructured/
+bricks.html#partitioning). The use cases of `unstructured` revolve around
+streamlining and optimizing the data processing workflow for LLMs.
+`unstructured` modular bricks and connectors form a cohesive system that
+simplifies data ingestion and pre-processing, making it adaptable to different
+platforms and is efficient in transforming unstructured data into structured
+outputs.
                           ******** AAPPII AAnnnnoouunncceemmeenntt!! ********
 We are thrilled to announce our newly launched [Unstructured API](https://
-unstructured-io.github.io/unstructured/api.html). While access to the hosted
-Unstructured API will remain free, API Keys are required to make requests. To
-prevent disruption, get yours [here](https://unstructured.io/#get-api-key) now
-and start using it today! Check out the [readme](https://github.com/
-Unstructured-IO/unstructured-api#--) here to get started making API calls.
+unstructured-io.github.io/unstructured/api.html), providing the Unstructured
+capabilities from `unstructured` as an API. Check out the [`unstructured-api`
+GitHub repository](https://github.com/Unstructured-IO/unstructured-api) to
+start making API calls. Youâll also find instructions about how to host your
+own API version. While access to the hosted Unstructured API will remain free,
+API Keys are required to make requests. To prevent disruption, get yours [here]
+(https://unstructured.io/#get-api-key) and start using it today! Check out the
+[`unstructured-api` README](https://github.com/Unstructured-IO/unstructured-
+api#--) to start making API calls.
 #### :rocket: Beta Feature: Chipper Model We are releasing the beta version of
 our Chipper model to deliver superior performance when processing high-
 resolution, complex documents. To start using the Chipper model in your API
-request, you can utilize the `hi_res` strategy. Please refer to the
-documentation [here](https://unstructured-io.github.io/unstructured/
-api.html#strategies). As the Chipper model is in beta version, we welcome
-feedback and suggestions. For those interested in testing the Chipper model, we
-encourage you to connect with us on [Slack community](https://join.slack.com/t/
-unstructuredw-kbe4326/shared_invite/zt-1x7cgo0pg-PTptXWylzPQF9xZolzCnwQ).
-       ******** OOppeenn--SSoouurrccee PPrree--PPrroocceessssiinngg TToooollss ffoorr UUnnssttrruuccttuurreedd DDaattaa ********
-The `unstructured` library provides open-source components for pre-processing
-text documents such as **PDFs**, **HTML** and **Word** Documents. These
-components are packaged as *bricks* ð§±, which provide users the building
-blocks they need to build pipelines targeted at the documents they care about.
-Bricks in the library fall into three categories: - :jigsaw: ***Partitioning
-bricks*** that break raw documents down into standard, structured elements. - :
-broom: ***Cleaning bricks*** that remove unwanted text from documents, such as
-boilerplate and sentence fragments. - :performing_arts: ***Staging bricks***
-that format data for downstream tasks, such as ML inference and data labeling.
-Unstructured also provides the capabilities from `unstructured` as an API.
-Checkout the [`unstructured-api` repo](https://github.com/Unstructured-IO/
-unstructured-api) to get started making API calls. Youâll also find
-instructions there about how to host your own version of the API. ## :bookmark:
-Documentation This README gives an overview of how to install, use and develop
-the library. For more comprehensive documentation, visit https://unstructured-
-io.github.io/unstructured/ . ## :eight_pointed_black_star: Quick Start There
-are two ways to use the library: 1) run a container or 2) install it ### Using
-the library in a container The following instructions are intended to help you
-get up and running using Docker to interact with `unstructured`. See [here]
-(https://docs.docker.com/get-docker/) if you don't already have docker
-installed on your machine. NOTE: we build multi-platform images to support both
-x86_64 and Apple silicon hardware. `docker pull` should download the
-corresponding image for your architecture, but you can specify with `--
-platform` (e.g. `--platform linux/amd64`) if needed. We build Docker images for
-all pushes to `main`. We tag each image with the corresponding short commit
-hash (e.g. `fbc7a69`) and the application version (e.g. `0.5.5-dev1`). We also
-tag the most recent image with `latest`. To leverage this, `docker pull` from
-our image repository. ```bash docker pull quay.io/unstructured-io/unstructured:
-latest ``` Once pulled, you can create a container from this image and shell to
-it. ```bash # create the container docker run -dt --name unstructured quay.io/
-unstructured-io/unstructured:latest # this will drop you into a bash shell
-where the Docker image is running docker exec -it unstructured bash ``` You can
-also build your own Docker image. If you only plan on parsing one type of data
-you can speed up building the image by commenting out some of the packages/
-requirements necessary for other data types. See Dockerfile to know which lines
-are necessary for your use case. ```bash make docker-build # this will drop you
+request, you can utilize the `hi_res_model_name=chipper` parameter. Please
+refer to the documentation [here](https://unstructured-io.github.io/
+unstructured/api.html#beta-version-hi-res-strategy-with-chipper-model). As the
+Chipper model is in beta version, we welcome feedback and suggestions. For
+those interested in testing the Chipper model, we encourage you to connect with
+us on [Slack community](https://join.slack.com/t/unstructuredw-kbe4326/
+shared_invite/zt-1x7cgo0pg-PTptXWylzPQF9xZolzCnwQ). ## :
+eight_pointed_black_star: Quick Start There are several ways to use the
+`unstructured` library: * [Run the library in a container](https://github.com/
+Unstructured-IO/unstructured#using-the-library-in-a-container) or * Install the
+library 1. [Install from PyPI](https://github.com/Unstructured-IO/
+unstructured#installing-the-library) 2. [Install for local development](https:/
+/github.com/Unstructured-IO/unstructured#coffee-installation-instructions-for-
+local-development) * For installation with `conda` on Windows system, please
+refer to the [documentation](https://unstructured-io.github.io/unstructured/
+installing.html#installation-with-conda-on-windows) ### Run the library in a
+container The following instructions are intended to help you get up and
+running using Docker to interact with `unstructured`. See [here](https://
+docs.docker.com/get-docker/) if you don't already have docker installed on your
+machine. NOTE: we build multi-platform images to support both x86_64 and Apple
+silicon hardware. `docker pull` should download the corresponding image for
+your architecture, but you can specify with `--platform` (e.g. `--platform
+linux/amd64`) if needed. We build Docker images for all pushes to `main`. We
+tag each image with the corresponding short commit hash (e.g. `fbc7a69`) and
+the application version (e.g. `0.5.5-dev1`). We also tag the most recent image
+with `latest`. To leverage this, `docker pull` from our image repository.
+```bash docker pull quay.io/unstructured-io/unstructured:latest ``` Once
+pulled, you can create a container from this image and shell to it. ```bash #
+create the container docker run -dt --name unstructured quay.io/unstructured-
+io/unstructured:latest # this will drop you into a bash shell where the Docker
+image is running docker exec -it unstructured bash ``` You can also build your
+own Docker image. If you only plan on parsing one type of data you can speed up
+building the image by commenting out some of the packages/requirements
+necessary for other data types. See Dockerfile to know which lines are
+necessary for your use case. ```bash make docker-build # this will drop you
 into a bash shell where the Docker image is running make docker-start-bash ```
-Once in the running container, you can try things out directly in Python
+Once in the running container, you can try things directly in Python
 interpreter's interactive mode. ```bash # this will drop you into a python
 console so you can run the below partition functions python3 >>> from
 unstructured.partition.pdf import partition_pdf >>> elements = partition_pdf
 (filename="example-docs/layout-parser-paper-fast.pdf") >>> from
 unstructured.partition.text import partition_text >>> elements = partition_text
 (filename="example-docs/fake-text.txt") ``` ### Installing the library Use the
 following instructions to get up and running with `unstructured` and test your
-installation. - Install the Python SDK with `pip install "unstructured[local-
-inference]"` - If you do not need to process PDFs or images, you can run `pip
-install unstructured` - Install the following system dependencies if they are
-not already available on your system. Depending on what document types you're
-parsing, you may not need all of these. - `libmagic-dev` (filetype detection) -
-`poppler-utils` (images and PDFs) - `tesseract-ocr` (images and PDFs) -
-`libreoffice` (MS Office docs) - `pandoc` (EPUBs, RTFs and Open Office docs) -
-For suggestions on how to install on Windows and to learn about dependencies
-for other features, see the installation documentation [here](https://
-unstructured-io.github.io/unstructured/installing.html). At this point, you
-should be able to run the following code: ```python from
-unstructured.partition.auto import partition elements = partition
-(filename="example-docs/eml/fake-email.eml") print("\n\n".join([str(el) for el
-in elements])) ``` The following table shows the document types the
-`unstructured` library currently supports. `partition` will recognize each of
-these document types and route the document to the appropriate partitioning
-function. If you already know your document type, you can use the partitioning
-function listed in the table directly. See our [documentation page](https://
-unstructured-io.github.io/unstructured/) for more details about the library. |
-Document Type | Partition Function | Strategies | Table Support | Options | | -
--- | --- | --- | --- | --- | | CSV Files (`.csv`) | `partition_csv` | N/A | Yes
-| None | | E-mails (`.eml`) | `partition_eml` | N/A | No | Encoding; Max
-Partition; Process Attachments | | E-mails (`.msg`) | `partition_msg` | N/A |
-No | Encoding; Max Partition; Process Attachments | | EPubs (`.epub`) |
-`partition_epub` | N/A | Yes | Include Page Breaks | | Excel Documents
-(`.xlsx`/`.xls`) | `partition_xlsx` | N/A | Yes | None | | HTML Pages (`.html`)
-| `partition_html` | N/A | No | Encoding; Include Page Breaks | | Images
-(`.png`/`.jpg`) | `partition_image` | `"auto"`, `"hi_res"`, `"ocr_only"` | Yes
-| Encoding; Include Page Breaks; Infer Table Structure; OCR Languages, Strategy
-| | Markdown (`.md`) | `partitin_md` | N/A | Yes | Include Page Breaks | | Org
-Mode (`.org`) | `partition_org` | N/A | Yes | Include Page Breaks | | Open
-Office Documents (`.odt`) | `partition_odt` | N/A | Yes | None | | PDFs
-(`.pdf`) | `partition_pdf` | `"auto"`, `"fast"`, `"hi_res"`, `"ocr_only"` | Yes
-| Encoding; Include Page Breaks; Infer Table Structure; Max Partition; OCR
-Languages, Strategy | | Plain Text (`.txt`) | `partition_text` | N/A | No |
-Encoding; Max Partition; Paragraph Grouper | | Power Points (`.ppt`) |
-`partition_ppt` | N/A | Yes | Include Page Breaks | | Power Points (`.pptx`) |
-`partition_pptx` | N/A | Yes | Include Page Breaks | | ReStructured Text
-(`.rst`) | `partition_rst` | N/A | Yes | Include Page Breaks | | Rich Text
-Files (`.rtf`) | `partition_rtf` | N/A | Yes | Include Page Breaks | | TSV
-Files (`.tsv`) | `partition_tsv` | N/A | Yes | None | | Word Documents (`.doc`)
-| `partition_doc` | N/A | Yes | Include Page Breaks | | Word Documents
-(`.docx`) | `partition_docx` | N/A | Yes | Include Page Breaks | | XML
-Documents (`.xml`) | `partition_xml` | N/A | No | Encoding; Max Partition; XML
-Keep Tags | ## :coffee: Installation Instructions for Local Development The
-following instructions are intended to help you get up and running with
-`unstructured` locally if you are planning to contribute to the project. *
-Using `pyenv` to manage virtualenv's is recommended but not necessary * Mac
-install instructions. See [here](https://github.com/Unstructured-IO/
-community#mac--homebrew) for more detailed instructions. * `brew install pyenv-
-virtualenv` * `pyenv install 3.8.17` * Linux instructions are available [here]
-(https://github.com/Unstructured-IO/community#linux). * Create a virtualenv to
-work in and activate it, e.g. for one named `unstructured`: `pyenv virtualenv
-3.8.17 unstructured`
+installation. - Install the Python SDK to support all document types with `pip
+install "unstructured[all-docs]"` - For plain text files, HTML, XML, JSON and
+Emails that do not require any extra dependencies, you can run `pip install
+unstructured` - To process other doc types, you can install the extras required
+for those documents, such as `pip install "unstructured[docx,pptx]"` - Install
+the following system dependencies if they are not already available on your
+system. Depending on what document types you're parsing, you may not need all
+of these. - `libmagic-dev` (filetype detection) - `poppler-utils` (images and
+PDFs) - `tesseract-ocr` (images and PDFs) - `libreoffice` (MS Office docs) -
+`pandoc` (EPUBs, RTFs and Open Office docs) - For suggestions on how to install
+on the Windows and to learn about dependencies for other features, see the
+installation documentation [here](https://unstructured-io.github.io/
+unstructured/installing.html). At this point, you should be able to run the
+following code: ```python from unstructured.partition.auto import partition
+elements = partition(filename="example-docs/eml/fake-email.eml") print
+("\n\n".join([str(el) for el in elements])) ``` ### Installation Instructions
+for Local Development The following instructions are intended to help you get
+up and running with `unstructured` locally if you are planning to contribute to
+the project. * Using `pyenv` to manage virtualenv's is recommended but not
+necessary * Mac install instructions. See [here](https://github.com/
+Unstructured-IO/community#mac--homebrew) for more detailed instructions. *
+`brew install pyenv-virtualenv` * `pyenv install 3.8.17` * Linux instructions
+are available [here](https://github.com/Unstructured-IO/community#linux). *
+Create a virtualenv to work in and activate it, e.g. for one named
+`unstructured`: `pyenv virtualenv 3.8.17 unstructured`
 `pyenv activate unstructured` * Run `make install` * Optional: * To install
 models and dependencies for processing images and PDFs locally, run `make
 install-local-inference`. * For processing image files, `tesseract` is
 required. See [here](https://tesseract-ocr.github.io/tessdoc/Installation.html)
 for installation instructions. * For processing PDF files, `tesseract` and
 `poppler` are required. The [pdf2image docs](https://pdf2image.readthedocs.io/
 en/latest/installation.html) have instructions on installing `poppler` across
 various platforms. Additionally, if you're planning to contribute to
 `unstructured`, we provide you an optional `pre-commit` configuration file to
 ensure your code matches the formatting and linting standards used in
-`unstructured`. If you'd prefer not having code changes auto-tidied before
+`unstructured`. If you'd prefer not to have code changes auto-tidied before
 every commit, you can use `make check` to see whether any linting or formatting
 changes should be applied, and `make tidy` to apply them. If using the optional
 `pre-commit`, you'll just need to install the hooks with `pre-commit install`
 since the `pre-commit` package is installed as part of `make install` mentioned
 above. Finally, if you decided to use `pre-commit` you can also uninstall the
-hooks with `pre-commit uninstall`. ## :clap: Quick Tour You can run this [Colab
-notebook](https://colab.research.google.com/drive/1U8VCjY2-
-x8c6y5TYMbSFtQGlQVFHCVIW) to run the examples below. The following examples
-show how to get started with the `unstructured` library. You can parse over a
-dozen document types with one line of code!
-See our [documentation page](https://unstructured-io.github.io/unstructured)
-for a full description of the features in the library. ### Document Parsing The
-easiest way to parse a document in unstructured is to use the `partition`
-brick. If you use `partition` brick, `unstructured` will detect the file type
-and route it to the appropriate file-specific partitioning brick. If you are
-using the `partition` brick, you may need to install additional parameters via
-`pip install unstructured[local-inference]`. Ensure you first install
-`libmagic` using the instructions outlined [here](https://unstructured-
-io.github.io/unstructured/installing.html#filetype-detection) `partition` will
-always apply the default arguments. If you need advanced features, use a
-document-specific brick. See the table above for a full list of document types
-supported in the library. ```python from unstructured.partition.auto import
-partition elements = partition("example-docs/layout-parser-paper.pdf") ``` Run
-`print("\n\n".join([str(el) for el in elements]))` to get a string
-representation of the output, which looks like: ``` LayoutParser : A Uniï¬ed
-Toolkit for Deep Learning Based Document Image Analysis Zejiang Shen 1 ( (cid:
-0) ), Ruochen Zhang 2 , Melissa Dell 3 , Benjamin Charles Germain Lee 4 , Jacob
-Carlson 3 , and Weining Li 5 Abstract. Recent advances in document image
-analysis (DIA) have been primarily driven by the application of neural
-networks. Ideally, research outcomes could be easily deployed in production and
-extended for further investigation. However, various factors like loosely
-organized codebases and sophisticated model conï¬gurations complicate the easy
-reuse of im- portant innovations by a wide audience. Though there have been on-
-going eï¬orts to improve reusability and simplify deep learning (DL) model
-development in disciplines like natural language processing and computer
-vision, none of them are optimized for challenges in the domain of DIA. This
-represents a major gap in the existing toolkit, as DIA is central to academic
-research across a wide range of disciplines in the social sciences and
-humanities. This paper introduces LayoutParser , an open-source library for
-streamlining the usage of DL in DIA research and applica- tions. The core
-LayoutParser library comes with a set of simple and intuitive interfaces for
-applying and customizing DL models for layout de- tection, character
-recognition, and many other document processing tasks. To promote
-extensibility, LayoutParser also incorporates a community platform for sharing
-both pre-trained models and full document digiti- zation pipelines. We
-demonstrate that LayoutParser is helpful for both lightweight and large-scale
-digitization pipelines in real-word use cases. The library is publicly
-available at https://layout-parser.github.io Keywords: Document Image Analysis
-Â· Deep Learning Â· Layout Analysis Â· Character Recognition Â· Open Source
-library Â· Toolkit. Introduction Deep Learning(DL)-based approaches are the
-state-of-the-art for a wide range of document image analysis (DIA) tasks
+hooks with `pre-commit uninstall`. ## :clap: Quick Tour ### Documentation This
+README overviews how to install, use and develop the library. For more
+comprehensive documentation, visit https://unstructured-io.github.io/
+unstructured/ . ### Concepts Guide **Bricks** ð§± in `unstructured` are the
+foundational elements that drive the data processing workflow within the
+system. These components provide users with the building blocks to build
+pipelines targeted at the documents they care about. The bricks fall into three
+categories: - :jigsaw: *Partitioning* bricks break raw documents into standard,
+structured elements. - :broom: *Cleaning* bricks remove unwanted text from
+documents, such as boilerplate and sentence fragments. - :performing_arts:
+*Staging* bricks format data for downstream tasks, such as ML inference and
+data labeling. These bricks create a cohesive, streamlined process that enables
+effective data handling and analysis. Check out the available bricks and how to
+use them from the [Bricks documentation](https://unstructured-io.github.io/
+unstructured/bricks.html). The **Connectors** ð in `unstructured` serve as
+vital links between the pre-processing pipeline and various data storage
+platforms. They allow for the batch processing of documents across various
+sources, including cloud services, repositories, and local directories. Each
+connector is tailored to a specific platform, such as Azure, Google Drive, or
+Github, and comes with unique commands and dependencies. To see the list of
+Connectors available in `unstructured` library, please check out the
+[Connectors GitHub folder](https://github.com/Unstructured-IO/unstructured/
+tree/main/unstructured/ingest/connector) and [documentation](https://
+unstructured-io.github.io/unstructured/connectors.html) ### PDF Document
+Parsing Example The following examples show how to get started with the
+`unstructured` library. You can parse over a dozen document types with one line
+of code! Use this [Colab notebook](https://colab.research.google.com/drive/
+1U8VCjY2-x8c6y5TYMbSFtQGlQVFHCVIW) to run the example below. The easiest way to
+parse a document in unstructured is to use the `partition` brick. If you use
+`partition` brick, `unstructured` will detect the file type and route it to the
+appropriate file-specific partitioning brick. If you are using the `partition`
+brick, you may need to install additional parameters via `pip install
+unstructured[local-inference]`. Ensure you first install `libmagic` using the
+instructions outlined [here](https://unstructured-io.github.io/unstructured/
+installing.html#filetype-detection) `partition` will always apply the default
+arguments. If you need advanced features, use a document-specific brick.
+```python from unstructured.partition.auto import partition elements =
+partition("example-docs/layout-parser-paper.pdf") ``` Run `print("\n\n".join(
+[str(el) for el in elements]))` to get a string representation of the output,
+which looks like: ``` LayoutParser : A Uniï¬ed Toolkit for Deep Learning Based
+Document Image Analysis Zejiang Shen 1 ( (cid:0) ), Ruochen Zhang 2 , Melissa
+Dell 3 , Benjamin Charles Germain Lee 4 , Jacob Carlson 3 , and Weining Li 5
+Abstract. Recent advances in document image analysis (DIA) have been primarily
+driven by the application of neural networks. Ideally, research outcomes could
+be easily deployed in production and extended for further investigation.
+However, various factors like loosely organized codebases and sophisticated
+model conï¬gurations complicate the easy reuse of im- portant innovations by a
+wide audience. Though there have been on-going eï¬orts to improve reusability
+and simplify deep learning (DL) model development in disciplines like natural
+language processing and computer vision, none of them are optimized for
+challenges in the domain of DIA. This represents a major gap in the existing
+toolkit, as DIA is central to academic research across a wide range of
+disciplines in the social sciences and humanities. This paper introduces
+LayoutParser , an open-source library for streamlining the usage of DL in DIA
+research and applica- tions. The core LayoutParser library comes with a set of
+simple and intuitive interfaces for applying and customizing DL models for
+layout de- tection, character recognition, and many other document processing
+tasks. To promote extensibility, LayoutParser also incorporates a community
+platform for sharing both pre-trained models and full document digiti- zation
+pipelines. We demonstrate that LayoutParser is helpful for both lightweight and
+large-scale digitization pipelines in real-word use cases. The library is
+publicly available at https://layout-parser.github.io Keywords: Document Image
+Analysis Â· Deep Learning Â· Layout Analysis Â· Character Recognition Â· Open
+Source library Â· Toolkit. Introduction Deep Learning(DL)-based approaches are
+the state-of-the-art for a wide range of document image analysis (DIA) tasks
 including document image classiï¬cation [11, ``` See the [partitioning](https:
 //unstructured-io.github.io/unstructured/bricks.html#partitioning) section in
 our documentation for a full list of options and instructions on how to use
 file-specific partitioning functions. ## :guardsman: Security Policy See our
 [security policy](https://github.com/Unstructured-IO/unstructured/security/
 policy) for information on how to report security vulnerabilities. ## :bug:
 Reporting Bugs Encountered a bug? Please create a new [GitHub issue](https://
@@ -228,9 +224,9 @@
 Provides-Extra: odt Provides-Extra: org Provides-Extra: pdf Provides-Extra:
 pptx Provides-Extra: rtf Provides-Extra: rst Provides-Extra: tsv Provides-
 Extra: xlsx Provides-Extra: s3 Provides-Extra: azure Provides-Extra: discord
 Provides-Extra: github Provides-Extra: gitlab Provides-Extra: reddit Provides-
 Extra: notion Provides-Extra: slack Provides-Extra: wikipedia Provides-Extra:
 google-drive Provides-Extra: gcs Provides-Extra: elasticsearch Provides-Extra:
 dropbox Provides-Extra: box Provides-Extra: onedrive Provides-Extra: outlook
-Provides-Extra: confluence Provides-Extra: huggingface Provides-Extra: local-
-inference
+Provides-Extra: confluence Provides-Extra: airtable Provides-Extra: sharepoint
+Provides-Extra: huggingface Provides-Extra: local-inference
```

