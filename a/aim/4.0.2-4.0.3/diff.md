# Comparing `tmp/aim-4.0.2.tar.gz` & `tmp/aim-4.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aim-4.0.2.tar", last modified: Tue Oct  3 17:16:35 2023, max compression
+gzip compressed data, was "aim-4.0.3.tar", last modified: Wed Oct  4 15:23:30 2023, max compression
```

## Comparing `aim-4.0.2.tar` & `aim-4.0.3.tar`

### file list

```diff
@@ -1,537 +1,553 @@
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-10-03 17:16:35.111830 aim-4.0.2/
--rw-r--r--   0 github     (503) staff       (20)    11347 2022-08-06 00:13:01.000000 aim-4.0.2/LICENSE
--rw-r--r--   0 github     (503) staff       (20)      214 2023-07-12 18:55:32.000000 aim-4.0.2/MANIFEST.in
--rw-r--r--   0 github     (503) staff       (20)    39615 2023-10-03 17:16:35.111575 aim-4.0.2/PKG-INFO
--rw-r--r--   0 github     (503) staff       (20)    38192 2023-10-03 16:38:51.000000 aim-4.0.2/README.md
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-10-03 17:16:35.021679 aim-4.0.2/aim.egg-info/
--rw-r--r--   0 github     (503) staff       (20)    39615 2023-10-03 17:16:34.000000 aim-4.0.2/aim.egg-info/PKG-INFO
--rw-r--r--   0 github     (503) staff       (20)    17304 2023-10-03 17:16:35.000000 aim-4.0.2/aim.egg-info/SOURCES.txt
--rw-r--r--   0 github     (503) staff       (20)        1 2023-10-03 17:16:34.000000 aim-4.0.2/aim.egg-info/dependency_links.txt
--rw-r--r--   0 github     (503) staff       (20)      110 2023-10-03 17:16:34.000000 aim-4.0.2/aim.egg-info/entry_points.txt
--rw-r--r--   0 github     (503) staff       (20)      381 2023-10-03 17:16:34.000000 aim-4.0.2/aim.egg-info/requires.txt
--rw-r--r--   0 github     (503) staff       (20)       21 2023-10-03 17:16:34.000000 aim-4.0.2/aim.egg-info/top_level.txt
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-10-03 17:16:35.012519 aim-4.0.2/pkgs/
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-10-03 17:16:35.021789 aim-4.0.2/pkgs/aimstack/
--rw-r--r--   0 github     (503) staff       (20)       24 2023-07-12 18:55:32.000000 aim-4.0.2/pkgs/aimstack/__init__.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-10-03 17:16:35.022064 aim-4.0.2/pkgs/aimstack/acme_tracker/
--rw-r--r--   0 github     (503) staff       (20)      131 2023-09-27 15:10:23.000000 aim-4.0.2/pkgs/aimstack/acme_tracker/__init__.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-10-03 17:16:35.022604 aim-4.0.2/pkgs/aimstack/acme_tracker/boards/
--rw-r--r--   0 github     (503) staff       (20)      122 2023-09-26 20:09:35.000000 aim-4.0.2/pkgs/aimstack/acme_tracker/boards/run.py
--rw-r--r--   0 github     (503) staff       (20)       87 2023-09-26 20:09:35.000000 aim-4.0.2/pkgs/aimstack/acme_tracker/boards/runs.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-10-03 17:16:35.023812 aim-4.0.2/pkgs/aimstack/acme_tracker/callbacks/
--rw-r--r--   0 github     (503) staff       (20)       83 2023-09-26 20:09:35.000000 aim-4.0.2/pkgs/aimstack/acme_tracker/callbacks/__init__.py
--rw-r--r--   0 github     (503) staff       (20)     2857 2023-09-27 17:12:13.000000 aim-4.0.2/pkgs/aimstack/acme_tracker/callbacks/base_callback.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-10-03 17:16:35.024525 aim-4.0.2/pkgs/aimstack/base/
--rw-r--r--   0 github     (503) staff       (20)      949 2023-09-27 15:10:23.000000 aim-4.0.2/pkgs/aimstack/base/__init__.py
--rw-r--r--   0 github     (503) staff       (20)     1740 2023-09-27 15:10:23.000000 aim-4.0.2/pkgs/aimstack/base/actions.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-10-03 17:16:35.026144 aim-4.0.2/pkgs/aimstack/base/boards/
--rw-r--r--   0 github     (503) staff       (20)     2900 2023-09-27 15:10:23.000000 aim-4.0.2/pkgs/aimstack/base/boards/audios.py
--rw-r--r--   0 github     (503) staff       (20)     2926 2023-09-27 15:10:23.000000 aim-4.0.2/pkgs/aimstack/base/boards/figures.py
--rw-r--r--   0 github     (503) staff       (20)     2900 2023-09-27 15:10:23.000000 aim-4.0.2/pkgs/aimstack/base/boards/images.py
--rw-r--r--   0 github     (503) staff       (20)     3350 2023-09-27 15:10:23.000000 aim-4.0.2/pkgs/aimstack/base/boards/logs_overview.py
--rw-r--r--   0 github     (503) staff       (20)     3719 2023-09-27 15:10:23.000000 aim-4.0.2/pkgs/aimstack/base/boards/metrics.py
--rw-r--r--   0 github     (503) staff       (20)     1776 2023-09-27 15:10:23.000000 aim-4.0.2/pkgs/aimstack/base/boards/run.py
--rw-r--r--   0 github     (503) staff       (20)     1956 2023-09-27 15:10:23.000000 aim-4.0.2/pkgs/aimstack/base/boards/runs.py
--rw-r--r--   0 github     (503) staff       (20)     2873 2023-09-27 15:10:23.000000 aim-4.0.2/pkgs/aimstack/base/boards/texts.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-10-03 17:16:35.027698 aim-4.0.2/pkgs/aimstack/base/types/
--rw-r--r--   0 github     (503) staff       (20)        0 2023-09-27 15:10:23.000000 aim-4.0.2/pkgs/aimstack/base/types/__init__.py
--rw-r--r--   0 github     (503) staff       (20)     3315 2023-09-27 15:10:23.000000 aim-4.0.2/pkgs/aimstack/base/types/audio.py
--rw-r--r--   0 github     (503) staff       (20)     4264 2023-09-27 15:10:23.000000 aim-4.0.2/pkgs/aimstack/base/types/distribution.py
--rw-r--r--   0 github     (503) staff       (20)     5244 2023-09-27 15:10:23.000000 aim-4.0.2/pkgs/aimstack/base/types/figures.py
--rw-r--r--   0 github     (503) staff       (20)    10080 2023-09-27 15:10:23.000000 aim-4.0.2/pkgs/aimstack/base/types/image.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-10-03 17:16:35.027950 aim-4.0.2/pkgs/aimstack/base/types/io/
--rw-r--r--   0 github     (503) staff       (20)        0 2023-09-27 15:10:23.000000 aim-4.0.2/pkgs/aimstack/base/types/io/__init__.py
--rw-r--r--   0 github     (503) staff       (20)    21094 2023-09-27 15:10:23.000000 aim-4.0.2/pkgs/aimstack/base/types/io/wavfile.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-10-03 17:16:35.028202 aim-4.0.2/pkgs/aimstack/base/types/logging/
--rw-r--r--   0 github     (503) staff       (20)     1663 2023-09-27 15:10:23.000000 aim-4.0.2/pkgs/aimstack/base/types/logging/__init__.py
--rw-r--r--   0 github     (503) staff       (20)     2567 2023-09-27 15:10:23.000000 aim-4.0.2/pkgs/aimstack/base/types/metric.py
--rw-r--r--   0 github     (503) staff       (20)     8919 2023-10-03 17:16:26.000000 aim-4.0.2/pkgs/aimstack/base/types/run.py
--rw-r--r--   0 github     (503) staff       (20)      718 2023-09-27 15:10:23.000000 aim-4.0.2/pkgs/aimstack/base/types/text.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-10-03 17:16:35.028364 aim-4.0.2/pkgs/aimstack/catboost_tracker/
--rw-r--r--   0 github     (503) staff       (20)      135 2023-09-27 15:10:23.000000 aim-4.0.2/pkgs/aimstack/catboost_tracker/__init__.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-10-03 17:16:35.028727 aim-4.0.2/pkgs/aimstack/catboost_tracker/boards/
--rw-r--r--   0 github     (503) staff       (20)      122 2023-09-26 20:09:35.000000 aim-4.0.2/pkgs/aimstack/catboost_tracker/boards/run.py
--rw-r--r--   0 github     (503) staff       (20)       91 2023-09-26 20:09:35.000000 aim-4.0.2/pkgs/aimstack/catboost_tracker/boards/runs.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-10-03 17:16:35.029054 aim-4.0.2/pkgs/aimstack/catboost_tracker/loggers/
--rw-r--r--   0 github     (503) staff       (20)       69 2023-09-26 20:09:35.000000 aim-4.0.2/pkgs/aimstack/catboost_tracker/loggers/__init__.py
--rw-r--r--   0 github     (503) staff       (20)     3876 2023-09-26 20:09:35.000000 aim-4.0.2/pkgs/aimstack/catboost_tracker/loggers/base_logger.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-10-03 17:16:35.029225 aim-4.0.2/pkgs/aimstack/docs/
--rw-r--r--   0 github     (503) staff       (20)      117 2023-09-27 15:10:23.000000 aim-4.0.2/pkgs/aimstack/docs/__init__.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-10-03 17:16:35.013486 aim-4.0.2/pkgs/aimstack/docs/boards/
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-10-03 17:16:35.030202 aim-4.0.2/pkgs/aimstack/docs/boards/sdk/
--rw-r--r--   0 github     (503) staff       (20)     4528 2023-07-12 18:55:32.000000 aim-4.0.2/pkgs/aimstack/docs/boards/sdk/aim_types.py
--rw-r--r--   0 github     (503) staff       (20)     4444 2023-07-12 18:55:32.000000 aim-4.0.2/pkgs/aimstack/docs/boards/sdk/container.py
--rw-r--r--   0 github     (503) staff       (20)     5074 2023-09-27 15:10:23.000000 aim-4.0.2/pkgs/aimstack/docs/boards/sdk/overview.py
--rw-r--r--   0 github     (503) staff       (20)     6979 2023-07-12 18:55:32.000000 aim-4.0.2/pkgs/aimstack/docs/boards/sdk/sequence.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-10-03 17:16:35.014007 aim-4.0.2/pkgs/aimstack/docs/boards/ui/
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-10-03 17:16:35.030640 aim-4.0.2/pkgs/aimstack/docs/boards/ui/board/
--rw-r--r--   0 github     (503) staff       (20)      527 2023-07-12 18:55:32.000000 aim-4.0.2/pkgs/aimstack/docs/boards/ui/board/board.py
--rw-r--r--   0 github     (503) staff       (20)      833 2023-07-12 18:55:32.000000 aim-4.0.2/pkgs/aimstack/docs/boards/ui/board/board_link.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-10-03 17:16:35.031006 aim-4.0.2/pkgs/aimstack/docs/boards/ui/charts/
--rw-r--r--   0 github     (503) staff       (20)     1547 2023-07-12 18:55:32.000000 aim-4.0.2/pkgs/aimstack/docs/boards/ui/charts/line_chart.py
--rw-r--r--   0 github     (503) staff       (20)     1001 2023-07-12 18:55:32.000000 aim-4.0.2/pkgs/aimstack/docs/boards/ui/charts/plotly.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-10-03 17:16:35.031600 aim-4.0.2/pkgs/aimstack/docs/boards/ui/data_viz/
--rw-r--r--   0 github     (503) staff       (20)      764 2023-07-12 18:55:32.000000 aim-4.0.2/pkgs/aimstack/docs/boards/ui/data_viz/dataframe.py
--rw-r--r--   0 github     (503) staff       (20)      713 2023-07-12 18:55:32.000000 aim-4.0.2/pkgs/aimstack/docs/boards/ui/data_viz/json.py
--rw-r--r--   0 github     (503) staff       (20)      702 2023-07-12 18:55:32.000000 aim-4.0.2/pkgs/aimstack/docs/boards/ui/data_viz/table.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-10-03 17:16:35.032224 aim-4.0.2/pkgs/aimstack/docs/boards/ui/examples/
--rw-r--r--   0 github     (503) staff       (20)     1967 2023-09-27 15:10:23.000000 aim-4.0.2/pkgs/aimstack/docs/boards/ui/examples/charts.py
--rw-r--r--   0 github     (503) staff       (20)      900 2023-09-27 15:10:23.000000 aim-4.0.2/pkgs/aimstack/docs/boards/ui/examples/data_display_elements.py
--rw-r--r--   0 github     (503) staff       (20)     3820 2023-09-27 15:10:23.000000 aim-4.0.2/pkgs/aimstack/docs/boards/ui/examples/input_components.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-10-03 17:16:35.034346 aim-4.0.2/pkgs/aimstack/docs/boards/ui/input/
--rw-r--r--   0 github     (503) staff       (20)      728 2023-07-12 18:55:32.000000 aim-4.0.2/pkgs/aimstack/docs/boards/ui/input/checkbox.py
--rw-r--r--   0 github     (503) staff       (20)     1207 2023-07-12 18:55:32.000000 aim-4.0.2/pkgs/aimstack/docs/boards/ui/input/multi_select.py
--rw-r--r--   0 github     (503) staff       (20)     1153 2023-07-12 18:55:32.000000 aim-4.0.2/pkgs/aimstack/docs/boards/ui/input/number_input.py
--rw-r--r--   0 github     (503) staff       (20)     1400 2023-07-12 18:55:32.000000 aim-4.0.2/pkgs/aimstack/docs/boards/ui/input/radio.py
--rw-r--r--   0 github     (503) staff       (20)     1173 2023-07-12 18:55:32.000000 aim-4.0.2/pkgs/aimstack/docs/boards/ui/input/range_slider.py
--rw-r--r--   0 github     (503) staff       (20)     1007 2023-07-12 18:55:32.000000 aim-4.0.2/pkgs/aimstack/docs/boards/ui/input/select.py
--rw-r--r--   0 github     (503) staff       (20)     1067 2023-07-12 18:55:32.000000 aim-4.0.2/pkgs/aimstack/docs/boards/ui/input/slider.py
--rw-r--r--   0 github     (503) staff       (20)      937 2023-07-12 18:55:32.000000 aim-4.0.2/pkgs/aimstack/docs/boards/ui/input/switch.py
--rw-r--r--   0 github     (503) staff       (20)     1000 2023-07-12 18:55:32.000000 aim-4.0.2/pkgs/aimstack/docs/boards/ui/input/text_area.py
--rw-r--r--   0 github     (503) staff       (20)      751 2023-07-12 18:55:32.000000 aim-4.0.2/pkgs/aimstack/docs/boards/ui/input/text_input.py
--rw-r--r--   0 github     (503) staff       (20)     1182 2023-07-12 18:55:32.000000 aim-4.0.2/pkgs/aimstack/docs/boards/ui/input/toggle_button.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-10-03 17:16:35.035112 aim-4.0.2/pkgs/aimstack/docs/boards/ui/layout_containers/
--rw-r--r--   0 github     (503) staff       (20)     1141 2023-07-12 18:55:32.000000 aim-4.0.2/pkgs/aimstack/docs/boards/ui/layout_containers/columns.py
--rw-r--r--   0 github     (503) staff       (20)     1125 2023-07-12 18:55:32.000000 aim-4.0.2/pkgs/aimstack/docs/boards/ui/layout_containers/form.py
--rw-r--r--   0 github     (503) staff       (20)     1023 2023-07-12 18:55:32.000000 aim-4.0.2/pkgs/aimstack/docs/boards/ui/layout_containers/rows.py
--rw-r--r--   0 github     (503) staff       (20)     1452 2023-07-12 18:55:32.000000 aim-4.0.2/pkgs/aimstack/docs/boards/ui/layout_containers/tabs.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-10-03 17:16:35.035914 aim-4.0.2/pkgs/aimstack/docs/boards/ui/sequence_viz/
--rw-r--r--   0 github     (503) staff       (20)      415 2023-09-27 15:10:23.000000 aim-4.0.2/pkgs/aimstack/docs/boards/ui/sequence_viz/audios.py
--rw-r--r--   0 github     (503) staff       (20)      423 2023-09-27 15:10:23.000000 aim-4.0.2/pkgs/aimstack/docs/boards/ui/sequence_viz/figures.py
--rw-r--r--   0 github     (503) staff       (20)      415 2023-09-27 15:10:23.000000 aim-4.0.2/pkgs/aimstack/docs/boards/ui/sequence_viz/images.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-10-03 17:16:35.037310 aim-4.0.2/pkgs/aimstack/docs/boards/ui/text/
--rw-r--r--   0 github     (503) staff       (20)      524 2023-07-12 18:55:32.000000 aim-4.0.2/pkgs/aimstack/docs/boards/ui/text/code.py
--rw-r--r--   0 github     (503) staff       (20)      428 2023-07-12 18:55:32.000000 aim-4.0.2/pkgs/aimstack/docs/boards/ui/text/header.py
--rw-r--r--   0 github     (503) staff       (20)      477 2023-07-12 18:55:32.000000 aim-4.0.2/pkgs/aimstack/docs/boards/ui/text/html.py
--rw-r--r--   0 github     (503) staff       (20)      606 2023-07-12 18:55:32.000000 aim-4.0.2/pkgs/aimstack/docs/boards/ui/text/link.py
--rw-r--r--   0 github     (503) staff       (20)      461 2023-07-12 18:55:32.000000 aim-4.0.2/pkgs/aimstack/docs/boards/ui/text/markdown.py
--rw-r--r--   0 github     (503) staff       (20)      452 2023-07-12 18:55:32.000000 aim-4.0.2/pkgs/aimstack/docs/boards/ui/text/subheader.py
--rw-r--r--   0 github     (503) staff       (20)      434 2023-07-12 18:55:32.000000 aim-4.0.2/pkgs/aimstack/docs/boards/ui/text/text.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-10-03 17:16:35.037684 aim-4.0.2/pkgs/aimstack/experiment_tracker/
--rw-r--r--   0 github     (503) staff       (20)      239 2023-09-27 15:10:23.000000 aim-4.0.2/pkgs/aimstack/experiment_tracker/__init__.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-10-03 17:16:35.038163 aim-4.0.2/pkgs/aimstack/experiment_tracker/boards/
--rw-r--r--   0 github     (503) staff       (20)     1831 2023-09-27 15:10:23.000000 aim-4.0.2/pkgs/aimstack/experiment_tracker/boards/run.py
--rw-r--r--   0 github     (503) staff       (20)     2068 2023-09-26 20:09:35.000000 aim-4.0.2/pkgs/aimstack/experiment_tracker/boards/runs.py
--rw-r--r--   0 github     (503) staff       (20)     2129 2023-09-27 15:10:23.000000 aim-4.0.2/pkgs/aimstack/experiment_tracker/training_flow.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-10-03 17:16:35.039335 aim-4.0.2/pkgs/aimstack/experiment_tracker/types/
--rw-r--r--   0 github     (503) staff       (20)        0 2023-09-26 20:09:35.000000 aim-4.0.2/pkgs/aimstack/experiment_tracker/types/__init__.py
--rw-r--r--   0 github     (503) staff       (20)     6055 2023-09-27 15:10:23.000000 aim-4.0.2/pkgs/aimstack/experiment_tracker/types/deeplake_dataset.py
--rw-r--r--   0 github     (503) staff       (20)     1921 2023-09-27 15:10:23.000000 aim-4.0.2/pkgs/aimstack/experiment_tracker/types/dvc_metadata.py
--rw-r--r--   0 github     (503) staff       (20)     3578 2023-09-27 15:10:23.000000 aim-4.0.2/pkgs/aimstack/experiment_tracker/types/hf_datasets_metadata.py
--rw-r--r--   0 github     (503) staff       (20)      141 2023-09-27 15:10:23.000000 aim-4.0.2/pkgs/aimstack/experiment_tracker/types/training_run.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-10-03 17:16:35.039669 aim-4.0.2/pkgs/aimstack/experiment_tracker/utils/
--rw-r--r--   0 github     (503) staff       (20)        0 2023-09-26 20:09:35.000000 aim-4.0.2/pkgs/aimstack/experiment_tracker/utils/__init__.py
--rw-r--r--   0 github     (503) staff       (20)     2524 2023-09-27 15:10:23.000000 aim-4.0.2/pkgs/aimstack/experiment_tracker/utils/pytorch.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-10-03 17:16:35.039860 aim-4.0.2/pkgs/aimstack/fastai_tracker/
--rw-r--r--   0 github     (503) staff       (20)      134 2023-09-27 15:10:23.000000 aim-4.0.2/pkgs/aimstack/fastai_tracker/__init__.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-10-03 17:16:35.040253 aim-4.0.2/pkgs/aimstack/fastai_tracker/boards/
--rw-r--r--   0 github     (503) staff       (20)      122 2023-09-26 20:09:35.000000 aim-4.0.2/pkgs/aimstack/fastai_tracker/boards/run.py
--rw-r--r--   0 github     (503) staff       (20)       89 2023-09-26 20:09:35.000000 aim-4.0.2/pkgs/aimstack/fastai_tracker/boards/runs.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-10-03 17:16:35.040656 aim-4.0.2/pkgs/aimstack/fastai_tracker/callbacks/
--rw-r--r--   0 github     (503) staff       (20)       73 2023-09-26 20:09:35.000000 aim-4.0.2/pkgs/aimstack/fastai_tracker/callbacks/__init__.py
--rw-r--r--   0 github     (503) staff       (20)     5696 2023-09-27 17:12:13.000000 aim-4.0.2/pkgs/aimstack/fastai_tracker/callbacks/base_callback.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-10-03 17:16:35.040950 aim-4.0.2/pkgs/aimstack/hugging_face_tracker/
--rw-r--r--   0 github     (503) staff       (20)      138 2023-09-27 15:10:23.000000 aim-4.0.2/pkgs/aimstack/hugging_face_tracker/__init__.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-10-03 17:16:35.041339 aim-4.0.2/pkgs/aimstack/hugging_face_tracker/boards/
--rw-r--r--   0 github     (503) staff       (20)      122 2023-09-26 20:09:35.000000 aim-4.0.2/pkgs/aimstack/hugging_face_tracker/boards/run.py
--rw-r--r--   0 github     (503) staff       (20)       95 2023-09-26 20:09:35.000000 aim-4.0.2/pkgs/aimstack/hugging_face_tracker/boards/runs.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-10-03 17:16:35.041875 aim-4.0.2/pkgs/aimstack/hugging_face_tracker/callbacks/
--rw-r--r--   0 github     (503) staff       (20)       79 2023-09-26 20:09:35.000000 aim-4.0.2/pkgs/aimstack/hugging_face_tracker/callbacks/__init__.py
--rw-r--r--   0 github     (503) staff       (20)     5795 2023-09-26 20:09:35.000000 aim-4.0.2/pkgs/aimstack/hugging_face_tracker/callbacks/base_callback.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-10-03 17:16:35.042278 aim-4.0.2/pkgs/aimstack/keras_tracker/
--rw-r--r--   0 github     (503) staff       (20)      132 2023-09-27 15:10:23.000000 aim-4.0.2/pkgs/aimstack/keras_tracker/__init__.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-10-03 17:16:35.042655 aim-4.0.2/pkgs/aimstack/keras_tracker/boards/
--rw-r--r--   0 github     (503) staff       (20)      122 2023-09-26 20:09:35.000000 aim-4.0.2/pkgs/aimstack/keras_tracker/boards/run.py
--rw-r--r--   0 github     (503) staff       (20)       88 2023-09-26 20:09:35.000000 aim-4.0.2/pkgs/aimstack/keras_tracker/boards/runs.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-10-03 17:16:35.043055 aim-4.0.2/pkgs/aimstack/keras_tracker/callbacks/
--rw-r--r--   0 github     (503) staff       (20)       72 2023-09-26 20:09:35.000000 aim-4.0.2/pkgs/aimstack/keras_tracker/callbacks/__init__.py
--rw-r--r--   0 github     (503) staff       (20)     2346 2023-09-27 17:12:13.000000 aim-4.0.2/pkgs/aimstack/keras_tracker/callbacks/base_callback.py
--rw-r--r--   0 github     (503) staff       (20)     1145 2023-09-26 20:09:35.000000 aim-4.0.2/pkgs/aimstack/keras_tracker/mixins.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-10-03 17:16:35.043331 aim-4.0.2/pkgs/aimstack/keras_tuner_tracker/
--rw-r--r--   0 github     (503) staff       (20)      137 2023-09-27 15:10:23.000000 aim-4.0.2/pkgs/aimstack/keras_tuner_tracker/__init__.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-10-03 17:16:35.043704 aim-4.0.2/pkgs/aimstack/keras_tuner_tracker/boards/
--rw-r--r--   0 github     (503) staff       (20)      122 2023-09-26 20:09:35.000000 aim-4.0.2/pkgs/aimstack/keras_tuner_tracker/boards/run.py
--rw-r--r--   0 github     (503) staff       (20)       94 2023-09-26 20:09:35.000000 aim-4.0.2/pkgs/aimstack/keras_tuner_tracker/boards/runs.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-10-03 17:16:35.044046 aim-4.0.2/pkgs/aimstack/keras_tuner_tracker/callbacks/
--rw-r--r--   0 github     (503) staff       (20)       78 2023-09-26 20:09:35.000000 aim-4.0.2/pkgs/aimstack/keras_tuner_tracker/callbacks/__init__.py
--rw-r--r--   0 github     (503) staff       (20)     2664 2023-09-26 20:09:35.000000 aim-4.0.2/pkgs/aimstack/keras_tuner_tracker/callbacks/base_callback.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-10-03 17:16:35.044216 aim-4.0.2/pkgs/aimstack/langchain_debugger/
--rw-r--r--   0 github     (503) staff       (20)      425 2023-09-27 15:10:23.000000 aim-4.0.2/pkgs/aimstack/langchain_debugger/__init__.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-10-03 17:16:35.045175 aim-4.0.2/pkgs/aimstack/langchain_debugger/boards/
--rw-r--r--   0 github     (503) staff       (20)     3366 2023-09-27 15:10:23.000000 aim-4.0.2/pkgs/aimstack/langchain_debugger/boards/cost.py
--rw-r--r--   0 github     (503) staff       (20)     5148 2023-09-27 15:10:23.000000 aim-4.0.2/pkgs/aimstack/langchain_debugger/boards/steps.py
--rw-r--r--   0 github     (503) staff       (20)     2490 2023-09-27 15:10:23.000000 aim-4.0.2/pkgs/aimstack/langchain_debugger/boards/trace.py
--rw-r--r--   0 github     (503) staff       (20)     2224 2023-09-27 15:10:23.000000 aim-4.0.2/pkgs/aimstack/langchain_debugger/boards/traces.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-10-03 17:16:35.045536 aim-4.0.2/pkgs/aimstack/langchain_debugger/callback_handlers/
--rw-r--r--   0 github     (503) staff       (20)      106 2023-09-27 15:10:23.000000 aim-4.0.2/pkgs/aimstack/langchain_debugger/callback_handlers/__init__.py
--rw-r--r--   0 github     (503) staff       (20)    11520 2023-09-27 15:10:23.000000 aim-4.0.2/pkgs/aimstack/langchain_debugger/callback_handlers/generic_callback_handler.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-10-03 17:16:35.046504 aim-4.0.2/pkgs/aimstack/langchain_debugger/types/
--rw-r--r--   0 github     (503) staff       (20)      128 2023-09-27 15:10:23.000000 aim-4.0.2/pkgs/aimstack/langchain_debugger/types/__init__.py
--rw-r--r--   0 github     (503) staff       (20)     4445 2023-09-27 15:10:23.000000 aim-4.0.2/pkgs/aimstack/langchain_debugger/types/action.py
--rw-r--r--   0 github     (503) staff       (20)     1800 2023-09-27 15:10:23.000000 aim-4.0.2/pkgs/aimstack/langchain_debugger/types/step.py
--rw-r--r--   0 github     (503) staff       (20)      660 2023-09-27 15:10:23.000000 aim-4.0.2/pkgs/aimstack/langchain_debugger/types/trace.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-10-03 17:16:35.046692 aim-4.0.2/pkgs/aimstack/lightgbm_tracker/
--rw-r--r--   0 github     (503) staff       (20)      135 2023-09-27 15:10:23.000000 aim-4.0.2/pkgs/aimstack/lightgbm_tracker/__init__.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-10-03 17:16:35.047124 aim-4.0.2/pkgs/aimstack/lightgbm_tracker/boards/
--rw-r--r--   0 github     (503) staff       (20)      122 2023-09-26 20:09:35.000000 aim-4.0.2/pkgs/aimstack/lightgbm_tracker/boards/run.py
--rw-r--r--   0 github     (503) staff       (20)       91 2023-09-26 20:09:35.000000 aim-4.0.2/pkgs/aimstack/lightgbm_tracker/boards/runs.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-10-03 17:16:35.047525 aim-4.0.2/pkgs/aimstack/lightgbm_tracker/callbacks/
--rw-r--r--   0 github     (503) staff       (20)       75 2023-09-26 20:09:35.000000 aim-4.0.2/pkgs/aimstack/lightgbm_tracker/callbacks/__init__.py
--rw-r--r--   0 github     (503) staff       (20)     3520 2023-09-27 17:12:13.000000 aim-4.0.2/pkgs/aimstack/lightgbm_tracker/callbacks/base_callback.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-10-03 17:16:35.047790 aim-4.0.2/pkgs/aimstack/llamaindex_observer/
--rw-r--r--   0 github     (503) staff       (20)      453 2023-09-27 15:10:23.000000 aim-4.0.2/pkgs/aimstack/llamaindex_observer/__init__.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-10-03 17:16:35.048571 aim-4.0.2/pkgs/aimstack/llamaindex_observer/boards/
--rw-r--r--   0 github     (503) staff       (20)     3365 2023-09-27 15:10:23.000000 aim-4.0.2/pkgs/aimstack/llamaindex_observer/boards/cost.py
--rw-r--r--   0 github     (503) staff       (20)     5922 2023-09-27 15:10:23.000000 aim-4.0.2/pkgs/aimstack/llamaindex_observer/boards/steps.py
--rw-r--r--   0 github     (503) staff       (20)     2555 2023-09-27 15:10:23.000000 aim-4.0.2/pkgs/aimstack/llamaindex_observer/boards/trace.py
--rw-r--r--   0 github     (503) staff       (20)     2007 2023-09-27 15:10:23.000000 aim-4.0.2/pkgs/aimstack/llamaindex_observer/boards/traces.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-10-03 17:16:35.049035 aim-4.0.2/pkgs/aimstack/llamaindex_observer/callback_handlers/
--rw-r--r--   0 github     (503) staff       (20)      107 2023-09-27 15:10:23.000000 aim-4.0.2/pkgs/aimstack/llamaindex_observer/callback_handlers/__init__.py
--rw-r--r--   0 github     (503) staff       (20)    11232 2023-09-27 15:10:23.000000 aim-4.0.2/pkgs/aimstack/llamaindex_observer/callback_handlers/generic_callback_handler.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-10-03 17:16:35.049942 aim-4.0.2/pkgs/aimstack/llamaindex_observer/types/
--rw-r--r--   0 github     (503) staff       (20)      130 2023-09-27 15:10:23.000000 aim-4.0.2/pkgs/aimstack/llamaindex_observer/types/__init__.py
--rw-r--r--   0 github     (503) staff       (20)     4080 2023-09-27 15:10:23.000000 aim-4.0.2/pkgs/aimstack/llamaindex_observer/types/action.py
--rw-r--r--   0 github     (503) staff       (20)     1544 2023-09-27 15:10:23.000000 aim-4.0.2/pkgs/aimstack/llamaindex_observer/types/step.py
--rw-r--r--   0 github     (503) staff       (20)      640 2023-09-27 15:10:23.000000 aim-4.0.2/pkgs/aimstack/llamaindex_observer/types/trace.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-10-03 17:16:35.050111 aim-4.0.2/pkgs/aimstack/mxnet_tracker/
--rw-r--r--   0 github     (503) staff       (20)      132 2023-09-27 15:10:23.000000 aim-4.0.2/pkgs/aimstack/mxnet_tracker/__init__.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-10-03 17:16:35.050449 aim-4.0.2/pkgs/aimstack/mxnet_tracker/boards/
--rw-r--r--   0 github     (503) staff       (20)      122 2023-09-26 20:09:35.000000 aim-4.0.2/pkgs/aimstack/mxnet_tracker/boards/run.py
--rw-r--r--   0 github     (503) staff       (20)       88 2023-09-26 20:09:35.000000 aim-4.0.2/pkgs/aimstack/mxnet_tracker/boards/runs.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-10-03 17:16:35.050776 aim-4.0.2/pkgs/aimstack/mxnet_tracker/loggers/
--rw-r--r--   0 github     (503) staff       (20)       70 2023-09-26 20:09:35.000000 aim-4.0.2/pkgs/aimstack/mxnet_tracker/loggers/__init__.py
--rw-r--r--   0 github     (503) staff       (20)     8250 2023-09-27 17:12:13.000000 aim-4.0.2/pkgs/aimstack/mxnet_tracker/loggers/base_logger.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-10-03 17:16:35.051029 aim-4.0.2/pkgs/aimstack/optuna_tracker/
--rw-r--r--   0 github     (503) staff       (20)      133 2023-09-27 15:10:23.000000 aim-4.0.2/pkgs/aimstack/optuna_tracker/__init__.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-10-03 17:16:35.051389 aim-4.0.2/pkgs/aimstack/optuna_tracker/boards/
--rw-r--r--   0 github     (503) staff       (20)      122 2023-09-26 20:09:35.000000 aim-4.0.2/pkgs/aimstack/optuna_tracker/boards/run.py
--rw-r--r--   0 github     (503) staff       (20)       89 2023-09-26 20:09:35.000000 aim-4.0.2/pkgs/aimstack/optuna_tracker/boards/runs.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-10-03 17:16:35.051755 aim-4.0.2/pkgs/aimstack/optuna_tracker/callbacks/
--rw-r--r--   0 github     (503) staff       (20)       74 2023-09-26 20:09:35.000000 aim-4.0.2/pkgs/aimstack/optuna_tracker/callbacks/__init__.py
--rw-r--r--   0 github     (503) staff       (20)     6530 2023-09-27 17:12:13.000000 aim-4.0.2/pkgs/aimstack/optuna_tracker/callbacks/base_callback.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-10-03 17:16:35.052131 aim-4.0.2/pkgs/aimstack/paddle_tracker/
--rw-r--r--   0 github     (503) staff       (20)      139 2023-09-27 15:10:23.000000 aim-4.0.2/pkgs/aimstack/paddle_tracker/__init__.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-10-03 17:16:35.052590 aim-4.0.2/pkgs/aimstack/paddle_tracker/boards/
--rw-r--r--   0 github     (503) staff       (20)      122 2023-09-26 20:09:35.000000 aim-4.0.2/pkgs/aimstack/paddle_tracker/boards/run.py
--rw-r--r--   0 github     (503) staff       (20)       89 2023-09-26 20:09:35.000000 aim-4.0.2/pkgs/aimstack/paddle_tracker/boards/runs.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-10-03 17:16:35.052974 aim-4.0.2/pkgs/aimstack/paddle_tracker/callbacks/
--rw-r--r--   0 github     (503) staff       (20)       73 2023-09-26 20:09:35.000000 aim-4.0.2/pkgs/aimstack/paddle_tracker/callbacks/__init__.py
--rw-r--r--   0 github     (503) staff       (20)     2744 2023-09-27 17:12:13.000000 aim-4.0.2/pkgs/aimstack/paddle_tracker/callbacks/base_callback.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-10-03 17:16:35.053151 aim-4.0.2/pkgs/aimstack/prophet_tracker/
--rw-r--r--   0 github     (503) staff       (20)      137 2023-09-27 15:10:23.000000 aim-4.0.2/pkgs/aimstack/prophet_tracker/__init__.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-10-03 17:16:35.053590 aim-4.0.2/pkgs/aimstack/prophet_tracker/boards/
--rw-r--r--   0 github     (503) staff       (20)      122 2023-09-26 20:09:35.000000 aim-4.0.2/pkgs/aimstack/prophet_tracker/boards/run.py
--rw-r--r--   0 github     (503) staff       (20)       90 2023-09-26 20:09:35.000000 aim-4.0.2/pkgs/aimstack/prophet_tracker/boards/runs.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-10-03 17:16:35.053964 aim-4.0.2/pkgs/aimstack/prophet_tracker/loggers/
--rw-r--r--   0 github     (503) staff       (20)       68 2023-09-26 20:09:35.000000 aim-4.0.2/pkgs/aimstack/prophet_tracker/loggers/__init__.py
--rw-r--r--   0 github     (503) staff       (20)     3003 2023-09-27 17:12:13.000000 aim-4.0.2/pkgs/aimstack/prophet_tracker/loggers/base_logger.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-10-03 17:16:35.054150 aim-4.0.2/pkgs/aimstack/pytorch_ignite_tracker/
--rw-r--r--   0 github     (503) staff       (20)      141 2023-09-27 15:10:23.000000 aim-4.0.2/pkgs/aimstack/pytorch_ignite_tracker/__init__.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-10-03 17:16:35.060210 aim-4.0.2/pkgs/aimstack/pytorch_ignite_tracker/boards/
--rw-r--r--   0 github     (503) staff       (20)      122 2023-09-26 20:09:35.000000 aim-4.0.2/pkgs/aimstack/pytorch_ignite_tracker/boards/run.py
--rw-r--r--   0 github     (503) staff       (20)       97 2023-09-26 20:09:35.000000 aim-4.0.2/pkgs/aimstack/pytorch_ignite_tracker/boards/runs.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-10-03 17:16:35.060538 aim-4.0.2/pkgs/aimstack/pytorch_ignite_tracker/loggers/
--rw-r--r--   0 github     (503) staff       (20)      110 2023-09-26 20:09:35.000000 aim-4.0.2/pkgs/aimstack/pytorch_ignite_tracker/loggers/__init__.py
--rw-r--r--   0 github     (503) staff       (20)     8692 2023-09-27 17:12:13.000000 aim-4.0.2/pkgs/aimstack/pytorch_ignite_tracker/loggers/base_logger.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-10-03 17:16:35.060709 aim-4.0.2/pkgs/aimstack/pytorch_lightning_tracker/
--rw-r--r--   0 github     (503) staff       (20)      144 2023-09-27 15:10:23.000000 aim-4.0.2/pkgs/aimstack/pytorch_lightning_tracker/__init__.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-10-03 17:16:35.061030 aim-4.0.2/pkgs/aimstack/pytorch_lightning_tracker/boards/
--rw-r--r--   0 github     (503) staff       (20)      122 2023-09-26 20:09:35.000000 aim-4.0.2/pkgs/aimstack/pytorch_lightning_tracker/boards/run.py
--rw-r--r--   0 github     (503) staff       (20)      100 2023-09-26 20:09:35.000000 aim-4.0.2/pkgs/aimstack/pytorch_lightning_tracker/boards/runs.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-10-03 17:16:35.061348 aim-4.0.2/pkgs/aimstack/pytorch_lightning_tracker/loggers/
--rw-r--r--   0 github     (503) staff       (20)       78 2023-09-26 20:09:35.000000 aim-4.0.2/pkgs/aimstack/pytorch_lightning_tracker/loggers/__init__.py
--rw-r--r--   0 github     (503) staff       (20)     6217 2023-09-27 17:12:13.000000 aim-4.0.2/pkgs/aimstack/pytorch_lightning_tracker/loggers/base_logger.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-10-03 17:16:35.061510 aim-4.0.2/pkgs/aimstack/sb3_tracker/
--rw-r--r--   0 github     (503) staff       (20)      144 2023-09-27 15:10:23.000000 aim-4.0.2/pkgs/aimstack/sb3_tracker/__init__.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-10-03 17:16:35.061820 aim-4.0.2/pkgs/aimstack/sb3_tracker/boards/
--rw-r--r--   0 github     (503) staff       (20)      122 2023-09-26 20:09:35.000000 aim-4.0.2/pkgs/aimstack/sb3_tracker/boards/run.py
--rw-r--r--   0 github     (503) staff       (20)       86 2023-09-26 20:09:35.000000 aim-4.0.2/pkgs/aimstack/sb3_tracker/boards/runs.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-10-03 17:16:35.062141 aim-4.0.2/pkgs/aimstack/sb3_tracker/callbacks/
--rw-r--r--   0 github     (503) staff       (20)       70 2023-09-26 20:09:35.000000 aim-4.0.2/pkgs/aimstack/sb3_tracker/callbacks/__init__.py
--rw-r--r--   0 github     (503) staff       (20)     3897 2023-09-27 17:12:13.000000 aim-4.0.2/pkgs/aimstack/sb3_tracker/callbacks/base_callback.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-10-03 17:16:35.062836 aim-4.0.2/pkgs/aimstack/tensorboard_sync/
--rw-r--r--   0 github     (503) staff       (20)       23 2023-09-27 15:10:23.000000 aim-4.0.2/pkgs/aimstack/tensorboard_sync/__init__.py
--rw-r--r--   0 github     (503) staff       (20)     1273 2023-07-12 18:55:32.000000 aim-4.0.2/pkgs/aimstack/tensorboard_sync/run.py
--rw-r--r--   0 github     (503) staff       (20)     9323 2023-07-12 18:55:32.000000 aim-4.0.2/pkgs/aimstack/tensorboard_sync/tracker.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-10-03 17:16:35.063105 aim-4.0.2/pkgs/aimstack/tensorflow_tracker/
--rw-r--r--   0 github     (503) staff       (20)      137 2023-09-27 15:10:23.000000 aim-4.0.2/pkgs/aimstack/tensorflow_tracker/__init__.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-10-03 17:16:35.063533 aim-4.0.2/pkgs/aimstack/tensorflow_tracker/boards/
--rw-r--r--   0 github     (503) staff       (20)      122 2023-09-26 20:09:35.000000 aim-4.0.2/pkgs/aimstack/tensorflow_tracker/boards/run.py
--rw-r--r--   0 github     (503) staff       (20)       93 2023-09-26 20:09:35.000000 aim-4.0.2/pkgs/aimstack/tensorflow_tracker/boards/runs.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-10-03 17:16:35.063911 aim-4.0.2/pkgs/aimstack/tensorflow_tracker/callbacks/
--rw-r--r--   0 github     (503) staff       (20)       77 2023-09-26 20:09:35.000000 aim-4.0.2/pkgs/aimstack/tensorflow_tracker/callbacks/__init__.py
--rw-r--r--   0 github     (503) staff       (20)     2593 2023-09-27 17:12:13.000000 aim-4.0.2/pkgs/aimstack/tensorflow_tracker/callbacks/base_callback.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-10-03 17:16:35.064218 aim-4.0.2/pkgs/aimstack/xgboost_tracker/
--rw-r--r--   0 github     (503) staff       (20)      134 2023-09-27 15:10:23.000000 aim-4.0.2/pkgs/aimstack/xgboost_tracker/__init__.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-10-03 17:16:35.064749 aim-4.0.2/pkgs/aimstack/xgboost_tracker/boards/
--rw-r--r--   0 github     (503) staff       (20)      122 2023-09-26 20:09:35.000000 aim-4.0.2/pkgs/aimstack/xgboost_tracker/boards/run.py
--rw-r--r--   0 github     (503) staff       (20)       90 2023-09-26 20:09:35.000000 aim-4.0.2/pkgs/aimstack/xgboost_tracker/boards/runs.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-10-03 17:16:35.065153 aim-4.0.2/pkgs/aimstack/xgboost_tracker/callbacks/
--rw-r--r--   0 github     (503) staff       (20)       74 2023-09-26 20:09:35.000000 aim-4.0.2/pkgs/aimstack/xgboost_tracker/callbacks/__init__.py
--rw-r--r--   0 github     (503) staff       (20)     3063 2023-09-27 17:12:13.000000 aim-4.0.2/pkgs/aimstack/xgboost_tracker/callbacks/base_callback.py
--rw-r--r--   0 github     (503) staff       (20)      898 2023-07-12 18:55:32.000000 aim-4.0.2/pyproject.toml
--rw-r--r--   0 github     (503) staff       (20)       38 2023-10-03 17:16:35.111871 aim-4.0.2/setup.cfg
--rw-r--r--   0 github     (503) staff       (20)     7017 2023-10-03 16:38:51.000000 aim-4.0.2/setup.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-10-03 17:16:35.019144 aim-4.0.2/src/
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-10-03 17:16:35.065454 aim-4.0.2/src/aimcore/
--rw-r--r--   0 github     (503) staff       (20)        0 2023-07-12 18:55:32.000000 aim-4.0.2/src/aimcore/__init__.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-10-03 17:16:35.066436 aim-4.0.2/src/aimcore/callbacks/
--rw-r--r--   0 github     (503) staff       (20)      130 2023-07-12 18:55:32.000000 aim-4.0.2/src/aimcore/callbacks/__init__.py
--rw-r--r--   0 github     (503) staff       (20)     1599 2023-07-12 18:55:32.000000 aim-4.0.2/src/aimcore/callbacks/caller.py
--rw-r--r--   0 github     (503) staff       (20)      478 2023-07-12 18:55:32.000000 aim-4.0.2/src/aimcore/callbacks/events.py
--rw-r--r--   0 github     (503) staff       (20)     1416 2023-07-12 18:55:32.000000 aim-4.0.2/src/aimcore/callbacks/helpers.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-10-03 17:16:35.066658 aim-4.0.2/src/aimcore/cleanup/
--rw-r--r--   0 github     (503) staff       (20)     3579 2023-07-12 18:55:32.000000 aim-4.0.2/src/aimcore/cleanup/__init__.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-10-03 17:16:35.067556 aim-4.0.2/src/aimcore/cli/
--rw-r--r--   0 github     (503) staff       (20)        0 2023-07-12 18:55:32.000000 aim-4.0.2/src/aimcore/cli/__init__.py
--rw-r--r--   0 github     (503) staff       (20)     1144 2023-09-26 20:09:35.000000 aim-4.0.2/src/aimcore/cli/cli.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-10-03 17:16:35.068070 aim-4.0.2/src/aimcore/cli/conatiners/
--rw-r--r--   0 github     (503) staff       (20)        0 2023-07-19 20:10:38.000000 aim-4.0.2/src/aimcore/cli/conatiners/__init__.py
--rw-r--r--   0 github     (503) staff       (20)     5434 2023-09-26 20:09:35.000000 aim-4.0.2/src/aimcore/cli/conatiners/commands.py
--rw-r--r--   0 github     (503) staff       (20)      791 2023-09-08 20:15:11.000000 aim-4.0.2/src/aimcore/cli/conatiners/utils.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-10-03 17:16:35.068530 aim-4.0.2/src/aimcore/cli/convert/
--rw-r--r--   0 github     (503) staff       (20)        0 2023-07-12 18:55:32.000000 aim-4.0.2/src/aimcore/cli/convert/__init__.py
--rw-r--r--   0 github     (503) staff       (20)     3004 2023-07-12 18:55:32.000000 aim-4.0.2/src/aimcore/cli/convert/commands.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-10-03 17:16:35.069331 aim-4.0.2/src/aimcore/cli/convert/processors/
--rw-r--r--   0 github     (503) staff       (20)      113 2023-07-12 18:55:32.000000 aim-4.0.2/src/aimcore/cli/convert/processors/__init__.py
--rw-r--r--   0 github     (503) staff       (20)     5916 2023-07-12 18:55:32.000000 aim-4.0.2/src/aimcore/cli/convert/processors/mlflow.py
--rw-r--r--   0 github     (503) staff       (20)    10374 2023-07-12 18:55:32.000000 aim-4.0.2/src/aimcore/cli/convert/processors/tensorboard.py
--rw-r--r--   0 github     (503) staff       (20)     6820 2023-07-12 18:55:32.000000 aim-4.0.2/src/aimcore/cli/convert/processors/wandb.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-10-03 17:16:35.069578 aim-4.0.2/src/aimcore/cli/init/
--rw-r--r--   0 github     (503) staff       (20)        0 2023-07-12 18:55:32.000000 aim-4.0.2/src/aimcore/cli/init/__init__.py
--rw-r--r--   0 github     (503) staff       (20)     1465 2023-07-12 18:55:32.000000 aim-4.0.2/src/aimcore/cli/init/commands.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-10-03 17:16:35.070092 aim-4.0.2/src/aimcore/cli/migrate/
--rw-r--r--   0 github     (503) staff       (20)        0 2023-07-25 12:19:13.000000 aim-4.0.2/src/aimcore/cli/migrate/__init__.py
--rw-r--r--   0 github     (503) staff       (20)     2055 2023-07-25 12:19:13.000000 aim-4.0.2/src/aimcore/cli/migrate/commands.py
--rw-r--r--   0 github     (503) staff       (20)     8167 2023-10-03 16:38:51.000000 aim-4.0.2/src/aimcore/cli/migrate/utils.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-10-03 17:16:35.070734 aim-4.0.2/src/aimcore/cli/package/
--rw-r--r--   0 github     (503) staff       (20)        0 2023-07-12 18:55:32.000000 aim-4.0.2/src/aimcore/cli/package/__init__.py
--rw-r--r--   0 github     (503) staff       (20)     6728 2023-09-26 20:09:35.000000 aim-4.0.2/src/aimcore/cli/package/commands.py
--rw-r--r--   0 github     (503) staff       (20)     1416 2023-09-26 20:09:35.000000 aim-4.0.2/src/aimcore/cli/package/utils.py
--rw-r--r--   0 github     (503) staff       (20)     4166 2023-08-04 20:11:55.000000 aim-4.0.2/src/aimcore/cli/package/watcher.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-10-03 17:16:35.071222 aim-4.0.2/src/aimcore/cli/server/
--rw-r--r--   0 github     (503) staff       (20)        0 2023-07-12 18:55:32.000000 aim-4.0.2/src/aimcore/cli/server/__init__.py
--rw-r--r--   0 github     (503) staff       (20)     4173 2023-09-19 20:11:49.000000 aim-4.0.2/src/aimcore/cli/server/commands.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-10-03 17:16:35.071570 aim-4.0.2/src/aimcore/cli/storage/
--rw-r--r--   0 github     (503) staff       (20)        0 2023-07-12 18:55:32.000000 aim-4.0.2/src/aimcore/cli/storage/__init__.py
--rw-r--r--   0 github     (503) staff       (20)     4082 2023-07-12 18:55:32.000000 aim-4.0.2/src/aimcore/cli/storage/commands.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-10-03 17:16:35.071822 aim-4.0.2/src/aimcore/cli/telemetry/
--rw-r--r--   0 github     (503) staff       (20)        0 2023-07-12 18:55:32.000000 aim-4.0.2/src/aimcore/cli/telemetry/__init__.py
--rw-r--r--   0 github     (503) staff       (20)      304 2023-07-12 18:55:32.000000 aim-4.0.2/src/aimcore/cli/telemetry/commands.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-10-03 17:16:35.072325 aim-4.0.2/src/aimcore/cli/ui/
--rw-r--r--   0 github     (503) staff       (20)        0 2023-07-25 12:19:13.000000 aim-4.0.2/src/aimcore/cli/ui/__init__.py
--rw-r--r--   0 github     (503) staff       (20)     5891 2023-09-19 20:11:49.000000 aim-4.0.2/src/aimcore/cli/ui/commands.py
--rw-r--r--   0 github     (503) staff       (20)      505 2023-09-19 20:11:49.000000 aim-4.0.2/src/aimcore/cli/ui/utils.py
--rw-r--r--   0 github     (503) staff       (20)      669 2023-09-19 20:11:49.000000 aim-4.0.2/src/aimcore/cli/utils.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-10-03 17:16:35.072580 aim-4.0.2/src/aimcore/cli/version/
--rw-r--r--   0 github     (503) staff       (20)        0 2023-07-12 18:55:32.000000 aim-4.0.2/src/aimcore/cli/version/__init__.py
--rw-r--r--   0 github     (503) staff       (20)      158 2023-07-12 18:55:32.000000 aim-4.0.2/src/aimcore/cli/version/commands.py
--rw-r--r--   0 github     (503) staff       (20)     9963 2023-07-12 18:55:32.000000 aim-4.0.2/src/aimcore/cli/watcher_cli.py
--rw-r--r--   0 github     (503) staff       (20)     1254 2023-09-04 20:14:49.000000 aim-4.0.2/src/aimcore/error_handling.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-10-03 17:16:35.072789 aim-4.0.2/src/aimcore/reporter/
--rw-r--r--   0 github     (503) staff       (20)    31358 2023-09-19 20:11:49.000000 aim-4.0.2/src/aimcore/reporter/__init__.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-10-03 17:16:35.076033 aim-4.0.2/src/aimcore/transport/
--rw-r--r--   0 github     (503) staff       (20)       27 2023-07-12 18:55:32.000000 aim-4.0.2/src/aimcore/transport/__init__.py
--rw-r--r--   0 github     (503) staff       (20)    10489 2023-09-04 20:14:49.000000 aim-4.0.2/src/aimcore/transport/client.py
--rw-r--r--   0 github     (503) staff       (20)      273 2023-07-12 18:55:32.000000 aim-4.0.2/src/aimcore/transport/config.py
--rw-r--r--   0 github     (503) staff       (20)     2239 2023-08-04 20:11:55.000000 aim-4.0.2/src/aimcore/transport/handlers.py
--rw-r--r--   0 github     (503) staff       (20)     5403 2023-07-13 20:09:35.000000 aim-4.0.2/src/aimcore/transport/heartbeat.py
--rw-r--r--   0 github     (503) staff       (20)     3095 2023-07-12 18:55:32.000000 aim-4.0.2/src/aimcore/transport/message_utils.py
--rw-r--r--   0 github     (503) staff       (20)      445 2023-07-12 18:55:32.000000 aim-4.0.2/src/aimcore/transport/remote_resource.py
--rw-r--r--   0 github     (503) staff       (20)     1825 2023-07-13 20:09:35.000000 aim-4.0.2/src/aimcore/transport/router.py
--rw-r--r--   0 github     (503) staff       (20)     3692 2023-07-12 18:55:32.000000 aim-4.0.2/src/aimcore/transport/rpc_queue.py
--rw-r--r--   0 github     (503) staff       (20)     4846 2023-08-04 20:11:55.000000 aim-4.0.2/src/aimcore/transport/server.py
--rw-r--r--   0 github     (503) staff       (20)     6358 2023-08-04 20:11:55.000000 aim-4.0.2/src/aimcore/transport/tracking.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-10-03 17:16:35.077046 aim-4.0.2/src/aimcore/web/
--rw-r--r--   0 github     (503) staff       (20)        0 2023-07-12 18:55:32.000000 aim-4.0.2/src/aimcore/web/__init__.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-10-03 17:16:35.078014 aim-4.0.2/src/aimcore/web/api/
--rw-r--r--   0 github     (503) staff       (20)     3317 2023-08-04 20:11:55.000000 aim-4.0.2/src/aimcore/web/api/__init__.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-10-03 17:16:35.078709 aim-4.0.2/src/aimcore/web/api/boards/
--rw-r--r--   0 github     (503) staff       (20)        0 2023-07-12 18:55:32.000000 aim-4.0.2/src/aimcore/web/api/boards/__init__.py
--rw-r--r--   0 github     (503) staff       (20)     1817 2023-07-12 18:55:32.000000 aim-4.0.2/src/aimcore/web/api/boards/models.py
--rw-r--r--   0 github     (503) staff       (20)      139 2023-07-12 18:55:32.000000 aim-4.0.2/src/aimcore/web/api/boards/pydantic_models.py
--rw-r--r--   0 github     (503) staff       (20)     1905 2023-09-19 20:11:49.000000 aim-4.0.2/src/aimcore/web/api/boards/views.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-10-03 17:16:35.079470 aim-4.0.2/src/aimcore/web/api/dashboard_apps/
--rw-r--r--   0 github     (503) staff       (20)        0 2023-07-12 18:55:32.000000 aim-4.0.2/src/aimcore/web/api/dashboard_apps/__init__.py
--rw-r--r--   0 github     (503) staff       (20)      920 2023-07-12 18:55:32.000000 aim-4.0.2/src/aimcore/web/api/dashboard_apps/models.py
--rw-r--r--   0 github     (503) staff       (20)      542 2023-07-12 18:55:32.000000 aim-4.0.2/src/aimcore/web/api/dashboard_apps/pydantic_models.py
--rw-r--r--   0 github     (503) staff       (20)      449 2023-07-12 18:55:32.000000 aim-4.0.2/src/aimcore/web/api/dashboard_apps/serializers.py
--rw-r--r--   0 github     (503) staff       (20)     2994 2023-07-12 18:55:32.000000 aim-4.0.2/src/aimcore/web/api/dashboard_apps/views.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-10-03 17:16:35.080232 aim-4.0.2/src/aimcore/web/api/dashboards/
--rw-r--r--   0 github     (503) staff       (20)        0 2023-07-12 18:55:32.000000 aim-4.0.2/src/aimcore/web/api/dashboards/__init__.py
--rw-r--r--   0 github     (503) staff       (20)      648 2023-07-12 18:55:32.000000 aim-4.0.2/src/aimcore/web/api/dashboards/models.py
--rw-r--r--   0 github     (503) staff       (20)      652 2023-07-12 18:55:32.000000 aim-4.0.2/src/aimcore/web/api/dashboards/pydantic_models.py
--rw-r--r--   0 github     (503) staff       (20)      783 2023-07-12 18:55:32.000000 aim-4.0.2/src/aimcore/web/api/dashboards/serializers.py
--rw-r--r--   0 github     (503) staff       (20)     3365 2023-07-12 18:55:32.000000 aim-4.0.2/src/aimcore/web/api/dashboards/views.py
--rw-r--r--   0 github     (503) staff       (20)      807 2023-07-12 18:55:32.000000 aim-4.0.2/src/aimcore/web/api/db.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-10-03 17:16:35.080968 aim-4.0.2/src/aimcore/web/api/projects/
--rw-r--r--   0 github     (503) staff       (20)        0 2023-07-12 18:55:32.000000 aim-4.0.2/src/aimcore/web/api/projects/__init__.py
--rw-r--r--   0 github     (503) staff       (20)      628 2023-07-12 18:55:32.000000 aim-4.0.2/src/aimcore/web/api/projects/project.py
--rw-r--r--   0 github     (503) staff       (20)     1247 2023-09-27 15:10:23.000000 aim-4.0.2/src/aimcore/web/api/projects/pydantic_models.py
--rw-r--r--   0 github     (503) staff       (20)     3489 2023-09-27 15:10:23.000000 aim-4.0.2/src/aimcore/web/api/projects/views.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-10-03 17:16:35.081306 aim-4.0.2/src/aimcore/web/api/queries/
--rw-r--r--   0 github     (503) staff       (20)        0 2023-07-12 18:55:32.000000 aim-4.0.2/src/aimcore/web/api/queries/__init__.py
--rw-r--r--   0 github     (503) staff       (20)     8582 2023-09-27 15:10:23.000000 aim-4.0.2/src/aimcore/web/api/queries/views.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-10-03 17:16:35.082069 aim-4.0.2/src/aimcore/web/api/reports/
--rw-r--r--   0 github     (503) staff       (20)        0 2023-07-12 18:55:32.000000 aim-4.0.2/src/aimcore/web/api/reports/__init__.py
--rw-r--r--   0 github     (503) staff       (20)      615 2023-07-12 18:55:32.000000 aim-4.0.2/src/aimcore/web/api/reports/models.py
--rw-r--r--   0 github     (503) staff       (20)      683 2023-07-12 18:55:32.000000 aim-4.0.2/src/aimcore/web/api/reports/pydantic_models.py
--rw-r--r--   0 github     (503) staff       (20)      461 2023-07-12 18:55:32.000000 aim-4.0.2/src/aimcore/web/api/reports/serializers.py
--rw-r--r--   0 github     (503) staff       (20)     2449 2023-09-08 20:15:11.000000 aim-4.0.2/src/aimcore/web/api/reports/views.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-10-03 17:16:35.082879 aim-4.0.2/src/aimcore/web/api/runs/
--rw-r--r--   0 github     (503) staff       (20)        0 2023-07-12 18:55:32.000000 aim-4.0.2/src/aimcore/web/api/runs/__init__.py
--rw-r--r--   0 github     (503) staff       (20)     4488 2023-07-12 18:55:32.000000 aim-4.0.2/src/aimcore/web/api/runs/pydantic_models.py
--rw-r--r--   0 github     (503) staff       (20)    14447 2023-09-08 20:15:11.000000 aim-4.0.2/src/aimcore/web/api/runs/utils.py
--rw-r--r--   0 github     (503) staff       (20)    13193 2023-07-12 18:55:32.000000 aim-4.0.2/src/aimcore/web/api/runs/views.py
--rw-r--r--   0 github     (503) staff       (20)     2906 2023-09-19 20:11:49.000000 aim-4.0.2/src/aimcore/web/api/utils.py
--rw-r--r--   0 github     (503) staff       (20)     1597 2023-07-12 18:55:32.000000 aim-4.0.2/src/aimcore/web/api/views.py
--rw-r--r--   0 github     (503) staff       (20)      384 2023-08-04 20:11:55.000000 aim-4.0.2/src/aimcore/web/configs.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-10-03 17:16:35.083140 aim-4.0.2/src/aimcore/web/middlewares/
--rw-r--r--   0 github     (503) staff       (20)        0 2023-07-12 18:55:32.000000 aim-4.0.2/src/aimcore/web/middlewares/__init__.py
--rw-r--r--   0 github     (503) staff       (20)     3654 2023-07-12 18:55:32.000000 aim-4.0.2/src/aimcore/web/middlewares/profiler.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-10-03 17:16:35.083988 aim-4.0.2/src/aimcore/web/migrations/
--rw-r--r--   0 github     (503) staff       (20)       38 2023-07-12 18:55:32.000000 aim-4.0.2/src/aimcore/web/migrations/README
--rw-r--r--   0 github     (503) staff       (20)      800 2023-07-12 18:55:32.000000 aim-4.0.2/src/aimcore/web/migrations/alembic.ini
--rw-r--r--   0 github     (503) staff       (20)      797 2023-07-12 18:55:32.000000 aim-4.0.2/src/aimcore/web/migrations/alembic_dev.ini
--rw-r--r--   0 github     (503) staff       (20)     2717 2023-07-12 18:55:32.000000 aim-4.0.2/src/aimcore/web/migrations/env.py
--rw-r--r--   0 github     (503) staff       (20)      494 2023-07-12 18:55:32.000000 aim-4.0.2/src/aimcore/web/migrations/script.py.mako
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-10-03 17:16:35.085185 aim-4.0.2/src/aimcore/web/migrations/versions/
--rw-r--r--   0 github     (503) staff       (20)     2183 2023-07-12 18:55:32.000000 aim-4.0.2/src/aimcore/web/migrations/versions/11672b13f92c_.py
--rw-r--r--   0 github     (503) staff       (20)     1545 2023-07-12 18:55:32.000000 aim-4.0.2/src/aimcore/web/migrations/versions/517a45b2e62c_.py
--rw-r--r--   0 github     (503) staff       (20)     5592 2023-07-12 18:55:32.000000 aim-4.0.2/src/aimcore/web/migrations/versions/5ae8371b7481_.py
--rw-r--r--   0 github     (503) staff       (20)     7262 2023-07-12 18:55:32.000000 aim-4.0.2/src/aimcore/web/migrations/versions/73a3d004c227_.py
--rw-r--r--   0 github     (503) staff       (20)     1788 2023-07-12 18:55:32.000000 aim-4.0.2/src/aimcore/web/migrations/versions/da08eab59790_board_and_board_templates.py
--rw-r--r--   0 github     (503) staff       (20)      959 2023-07-12 18:55:32.000000 aim-4.0.2/src/aimcore/web/migrations/versions/df1fff471cab_.py
--rw-r--r--   0 github     (503) staff       (20)       59 2023-07-12 18:55:32.000000 aim-4.0.2/src/aimcore/web/run.py
--rw-r--r--   0 github     (503) staff       (20)     3674 2023-09-19 20:11:49.000000 aim-4.0.2/src/aimcore/web/utils.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-10-03 17:16:35.019185 aim-4.0.2/src/python/
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-10-03 17:16:35.087214 aim-4.0.2/src/python/aim/
--rw-r--r--   0 github     (503) staff       (20)        6 2023-10-03 17:16:26.000000 aim-4.0.2/src/python/aim/VERSION
--rw-r--r--   0 github     (503) staff       (20)      825 2023-07-12 18:55:32.000000 aim-4.0.2/src/python/aim/__about__.py
--rw-r--r--   0 github     (503) staff       (20)      631 2023-09-05 20:15:25.000000 aim-4.0.2/src/python/aim/__init__.py
--rw-r--r--   0 github     (503) staff       (20)      183 2023-07-12 18:55:32.000000 aim-4.0.2/src/python/aim/__version__.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-10-03 17:16:35.087386 aim-4.0.2/src/python/aim/_core/
--rw-r--r--   0 github     (503) staff       (20)        0 2023-07-12 18:55:32.000000 aim-4.0.2/src/python/aim/_core/__init__.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-10-03 17:16:35.098045 aim-4.0.2/src/python/aim/_core/storage/
--rw-r--r--   0 github     (503) staff       (20)        0 2023-07-12 18:55:32.000000 aim-4.0.2/src/python/aim/_core/storage/__init__.py
--rw-r--r--   0 github     (503) staff       (20)   459259 2023-10-03 17:16:31.000000 aim-4.0.2/src/python/aim/_core/storage/arrayview.cpp
--rw-r--r--   0 github     (503) staff       (20)      278 2023-07-12 18:55:32.000000 aim-4.0.2/src/python/aim/_core/storage/arrayview.pxd
--rw-r--r--   0 github     (503) staff       (20)     3051 2023-07-12 18:55:32.000000 aim-4.0.2/src/python/aim/_core/storage/arrayview.py
--rw-r--r--   0 github     (503) staff       (20)   935063 2023-10-03 17:16:31.000000 aim-4.0.2/src/python/aim/_core/storage/container.cpp
--rw-r--r--   0 github     (503) staff       (20)      977 2023-07-12 18:55:32.000000 aim-4.0.2/src/python/aim/_core/storage/container.pxd
--rw-r--r--   0 github     (503) staff       (20)    12336 2023-07-12 18:55:32.000000 aim-4.0.2/src/python/aim/_core/storage/container.py
--rw-r--r--   0 github     (503) staff       (20)   968088 2023-10-03 17:16:32.000000 aim-4.0.2/src/python/aim/_core/storage/containertreeview.cpp
--rw-r--r--   0 github     (503) staff       (20)      337 2023-07-12 18:55:32.000000 aim-4.0.2/src/python/aim/_core/storage/containertreeview.pxd
--rw-r--r--   0 github     (503) staff       (20)     7258 2023-07-12 18:55:32.000000 aim-4.0.2/src/python/aim/_core/storage/containertreeview.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-10-03 17:16:35.099425 aim-4.0.2/src/python/aim/_core/storage/encoding/
--rw-r--r--   0 github     (503) staff       (20)   149167 2023-10-03 17:16:32.000000 aim-4.0.2/src/python/aim/_core/storage/encoding/__init__.cpp
--rw-r--r--   0 github     (503) staff       (20)      167 2023-07-12 18:55:32.000000 aim-4.0.2/src/python/aim/_core/storage/encoding/__init__.pxd
--rw-r--r--   0 github     (503) staff       (20)      107 2023-07-12 18:55:32.000000 aim-4.0.2/src/python/aim/_core/storage/encoding/__init__.py
--rw-r--r--   0 github     (503) staff       (20)   380498 2023-10-03 17:16:32.000000 aim-4.0.2/src/python/aim/_core/storage/encoding/encoding.cpp
--rw-r--r--   0 github     (503) staff       (20)      507 2023-07-12 18:55:32.000000 aim-4.0.2/src/python/aim/_core/storage/encoding/encoding.pxd
--rw-r--r--   0 github     (503) staff       (20)     7427 2023-07-12 18:55:32.000000 aim-4.0.2/src/python/aim/_core/storage/encoding/encoding.pyx
--rw-r--r--   0 github     (503) staff       (20)   356452 2023-10-03 17:16:32.000000 aim-4.0.2/src/python/aim/_core/storage/encoding/encoding_native.cpp
--rw-r--r--   0 github     (503) staff       (20)      930 2023-07-12 18:55:32.000000 aim-4.0.2/src/python/aim/_core/storage/encoding/encoding_native.pxd
--rw-r--r--   0 github     (503) staff       (20)     5980 2023-07-12 18:55:32.000000 aim-4.0.2/src/python/aim/_core/storage/encoding/encoding_native.pyx
--rw-r--r--   0 github     (503) staff       (20)      337 2023-07-12 18:55:32.000000 aim-4.0.2/src/python/aim/_core/storage/env.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-10-03 17:16:35.100755 aim-4.0.2/src/python/aim/_core/storage/hashing/
--rw-r--r--   0 github     (503) staff       (20)   142042 2023-10-03 17:16:32.000000 aim-4.0.2/src/python/aim/_core/storage/hashing/__init__.cpp
--rw-r--r--   0 github     (503) staff       (20)       97 2023-07-12 18:55:32.000000 aim-4.0.2/src/python/aim/_core/storage/hashing/__init__.pxd
--rw-r--r--   0 github     (503) staff       (20)       56 2023-07-12 18:55:32.000000 aim-4.0.2/src/python/aim/_core/storage/hashing/__init__.py
--rw-r--r--   0 github     (503) staff       (20)   206140 2023-10-03 17:16:32.000000 aim-4.0.2/src/python/aim/_core/storage/hashing/c_hash.cpp
--rw-r--r--   0 github     (503) staff       (20)      151 2023-07-12 18:55:32.000000 aim-4.0.2/src/python/aim/_core/storage/hashing/c_hash.pxd
--rw-r--r--   0 github     (503) staff       (20)     1083 2023-07-12 18:55:32.000000 aim-4.0.2/src/python/aim/_core/storage/hashing/c_hash.pyx
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-10-03 17:16:35.100858 aim-4.0.2/src/python/aim/_core/storage/hashing/hash/
--rw-r--r--   0 github     (503) staff       (20)     1412 2023-07-12 18:55:32.000000 aim-4.0.2/src/python/aim/_core/storage/hashing/hash/hash.h
--rw-r--r--   0 github     (503) staff       (20)   394398 2023-10-03 17:16:32.000000 aim-4.0.2/src/python/aim/_core/storage/hashing/hashing.cpp
--rw-r--r--   0 github     (503) staff       (20)     1021 2023-07-12 18:55:32.000000 aim-4.0.2/src/python/aim/_core/storage/hashing/hashing.pxd
--rw-r--r--   0 github     (503) staff       (20)     5580 2023-07-12 18:55:32.000000 aim-4.0.2/src/python/aim/_core/storage/hashing/hashing.py
--rw-r--r--   0 github     (503) staff       (20)   679035 2023-10-03 17:16:32.000000 aim-4.0.2/src/python/aim/_core/storage/inmemorytreeview.cpp
--rw-r--r--   0 github     (503) staff       (20)      202 2023-07-12 18:55:32.000000 aim-4.0.2/src/python/aim/_core/storage/inmemorytreeview.pxd
--rw-r--r--   0 github     (503) staff       (20)     4365 2023-07-12 18:55:32.000000 aim-4.0.2/src/python/aim/_core/storage/inmemorytreeview.py
--rw-r--r--   0 github     (503) staff       (20)     7858 2023-07-12 18:55:32.000000 aim-4.0.2/src/python/aim/_core/storage/locking.py
--rw-r--r--   0 github     (503) staff       (20)     2125 2023-09-14 20:15:29.000000 aim-4.0.2/src/python/aim/_core/storage/object.py
--rw-r--r--   0 github     (503) staff       (20)   979988 2023-10-03 17:16:33.000000 aim-4.0.2/src/python/aim/_core/storage/prefixview.cpp
--rw-r--r--   0 github     (503) staff       (20)      808 2023-07-12 18:55:32.000000 aim-4.0.2/src/python/aim/_core/storage/prefixview.pxd
--rw-r--r--   0 github     (503) staff       (20)    12274 2023-07-12 18:55:32.000000 aim-4.0.2/src/python/aim/_core/storage/prefixview.py
--rw-r--r--   0 github     (503) staff       (20)    11648 2023-07-12 18:55:32.000000 aim-4.0.2/src/python/aim/_core/storage/proxy.py
--rw-r--r--   0 github     (503) staff       (20)   996914 2023-10-03 17:16:33.000000 aim-4.0.2/src/python/aim/_core/storage/rockscontainer.cpp
--rw-r--r--   0 github     (503) staff       (20)    18696 2023-09-04 20:14:49.000000 aim-4.0.2/src/python/aim/_core/storage/rockscontainer.pyx
--rw-r--r--   0 github     (503) staff       (20)   706262 2023-10-03 17:16:33.000000 aim-4.0.2/src/python/aim/_core/storage/treearrayview.cpp
--rw-r--r--   0 github     (503) staff       (20)      263 2023-07-12 18:55:32.000000 aim-4.0.2/src/python/aim/_core/storage/treearrayview.pxd
--rw-r--r--   0 github     (503) staff       (20)     3044 2023-07-12 18:55:32.000000 aim-4.0.2/src/python/aim/_core/storage/treearrayview.py
--rw-r--r--   0 github     (503) staff       (20)   728377 2023-10-03 17:16:33.000000 aim-4.0.2/src/python/aim/_core/storage/treeutils.cpp
--rw-r--r--   0 github     (503) staff       (20)     8419 2023-07-12 18:55:32.000000 aim-4.0.2/src/python/aim/_core/storage/treeutils.pyx
--rw-r--r--   0 github     (503) staff       (20)      713 2023-07-12 18:55:32.000000 aim-4.0.2/src/python/aim/_core/storage/treeutils_non_native.py
--rw-r--r--   0 github     (503) staff       (20)   538818 2023-10-03 17:16:33.000000 aim-4.0.2/src/python/aim/_core/storage/treeview.cpp
--rw-r--r--   0 github     (503) staff       (20)      311 2023-07-12 18:55:32.000000 aim-4.0.2/src/python/aim/_core/storage/treeview.pxd
--rw-r--r--   0 github     (503) staff       (20)     3065 2023-07-12 18:55:32.000000 aim-4.0.2/src/python/aim/_core/storage/treeview.py
--rw-r--r--   0 github     (503) staff       (20)     1363 2023-07-12 18:55:32.000000 aim-4.0.2/src/python/aim/_core/storage/types.py
--rw-r--r--   0 github     (503) staff       (20)   813912 2023-10-03 17:16:33.000000 aim-4.0.2/src/python/aim/_core/storage/union.cpp
--rw-r--r--   0 github     (503) staff       (20)     7865 2023-09-04 20:14:49.000000 aim-4.0.2/src/python/aim/_core/storage/union.pyx
--rw-r--r--   0 github     (503) staff       (20)   817782 2023-10-03 17:16:34.000000 aim-4.0.2/src/python/aim/_core/storage/utils.cpp
--rw-r--r--   0 github     (503) staff       (20)      469 2023-07-12 18:55:32.000000 aim-4.0.2/src/python/aim/_core/storage/utils.pxd
--rw-r--r--   0 github     (503) staff       (20)     2102 2023-07-12 18:55:32.000000 aim-4.0.2/src/python/aim/_core/storage/utils.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-10-03 17:16:35.101307 aim-4.0.2/src/python/aim/_core/utils/
--rw-r--r--   0 github     (503) staff       (20)        0 2023-09-04 20:14:49.000000 aim-4.0.2/src/python/aim/_core/utils/__init__.py
--rw-r--r--   0 github     (503) staff       (20)      722 2023-07-12 18:55:32.000000 aim-4.0.2/src/python/aim/_core/utils/deprecation.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-10-03 17:16:35.101472 aim-4.0.2/src/python/aim/_ext/
--rw-r--r--   0 github     (503) staff       (20)        0 2023-07-12 18:55:32.000000 aim-4.0.2/src/python/aim/_ext/__init__.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-10-03 17:16:35.101880 aim-4.0.2/src/python/aim/_ext/notebook/
--rw-r--r--   0 github     (503) staff       (20)        0 2023-07-12 18:55:32.000000 aim-4.0.2/src/python/aim/_ext/notebook/__init__.py
--rw-r--r--   0 github     (503) staff       (20)     2615 2023-07-25 12:19:13.000000 aim-4.0.2/src/python/aim/_ext/notebook/manager.py
--rw-r--r--   0 github     (503) staff       (20)     7169 2023-07-25 12:19:13.000000 aim-4.0.2/src/python/aim/_ext/notebook/notebook.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-10-03 17:16:35.103578 aim-4.0.2/src/python/aim/_ext/notifier/
--rw-r--r--   0 github     (503) staff       (20)      593 2023-07-12 18:55:32.000000 aim-4.0.2/src/python/aim/_ext/notifier/__init__.py
--rw-r--r--   0 github     (503) staff       (20)      305 2023-07-12 18:55:32.000000 aim-4.0.2/src/python/aim/_ext/notifier/base_notifier.py
--rw-r--r--   0 github     (503) staff       (20)     1859 2023-07-12 18:55:32.000000 aim-4.0.2/src/python/aim/_ext/notifier/config.py
--rw-r--r--   0 github     (503) staff       (20)      523 2023-07-12 18:55:32.000000 aim-4.0.2/src/python/aim/_ext/notifier/logging_notifier.py
--rw-r--r--   0 github     (503) staff       (20)     1429 2023-07-12 18:55:32.000000 aim-4.0.2/src/python/aim/_ext/notifier/notifier.py
--rw-r--r--   0 github     (503) staff       (20)     1162 2023-07-12 18:55:32.000000 aim-4.0.2/src/python/aim/_ext/notifier/notifier_builder.py
--rw-r--r--   0 github     (503) staff       (20)      525 2023-07-12 18:55:32.000000 aim-4.0.2/src/python/aim/_ext/notifier/slack_notifier.py
--rw-r--r--   0 github     (503) staff       (20)     1035 2023-07-12 18:55:32.000000 aim-4.0.2/src/python/aim/_ext/notifier/utils.py
--rw-r--r--   0 github     (503) staff       (20)      863 2023-07-12 18:55:32.000000 aim-4.0.2/src/python/aim/_ext/notifier/workplace_notifier.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-10-03 17:16:35.105265 aim-4.0.2/src/python/aim/_ext/system_info/
--rw-r--r--   0 github     (503) staff       (20)      152 2023-07-12 18:55:32.000000 aim-4.0.2/src/python/aim/_ext/system_info/__init__.py
--rw-r--r--   0 github     (503) staff       (20)      100 2023-07-12 18:55:32.000000 aim-4.0.2/src/python/aim/_ext/system_info/configs.py
--rw-r--r--   0 github     (503) staff       (20)   148706 2023-07-12 18:55:32.000000 aim-4.0.2/src/python/aim/_ext/system_info/pynvml.py
--rw-r--r--   0 github     (503) staff       (20)     7798 2023-07-12 18:55:32.000000 aim-4.0.2/src/python/aim/_ext/system_info/resource_tracker.py
--rw-r--r--   0 github     (503) staff       (20)     6670 2023-09-19 20:11:49.000000 aim-4.0.2/src/python/aim/_ext/system_info/stat.py
--rw-r--r--   0 github     (503) staff       (20)     2246 2023-07-25 12:19:13.000000 aim-4.0.2/src/python/aim/_ext/system_info/utils.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-10-03 17:16:35.105423 aim-4.0.2/src/python/aim/_ext/tracking/
--rw-r--r--   0 github     (503) staff       (20)     4755 2023-07-12 18:55:32.000000 aim-4.0.2/src/python/aim/_ext/tracking/__init__.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-10-03 17:16:35.110650 aim-4.0.2/src/python/aim/_sdk/
--rw-r--r--   0 github     (503) staff       (20)        0 2023-07-12 18:55:32.000000 aim-4.0.2/src/python/aim/_sdk/__init__.py
--rw-r--r--   0 github     (503) staff       (20)      856 2023-09-14 20:15:29.000000 aim-4.0.2/src/python/aim/_sdk/action.py
--rw-r--r--   0 github     (503) staff       (20)       48 2023-07-12 18:55:32.000000 aim-4.0.2/src/python/aim/_sdk/blob.py
--rw-r--r--   0 github     (503) staff       (20)    10993 2023-08-04 20:11:55.000000 aim-4.0.2/src/python/aim/_sdk/collections.py
--rw-r--r--   0 github     (503) staff       (20)      363 2023-07-25 12:19:13.000000 aim-4.0.2/src/python/aim/_sdk/configs.py
--rw-r--r--   0 github     (503) staff       (20)      519 2023-07-12 18:55:32.000000 aim-4.0.2/src/python/aim/_sdk/constants.py
--rw-r--r--   0 github     (503) staff       (20)    15277 2023-09-27 17:12:13.000000 aim-4.0.2/src/python/aim/_sdk/container.py
--rw-r--r--   0 github     (503) staff       (20)     1837 2023-07-12 18:55:32.000000 aim-4.0.2/src/python/aim/_sdk/context.py
--rw-r--r--   0 github     (503) staff       (20)     1233 2023-08-04 20:11:55.000000 aim-4.0.2/src/python/aim/_sdk/dev_package.py
--rw-r--r--   0 github     (503) staff       (20)      561 2023-07-12 18:55:32.000000 aim-4.0.2/src/python/aim/_sdk/exceptions.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-10-03 17:16:35.111119 aim-4.0.2/src/python/aim/_sdk/interfaces/
--rw-r--r--   0 github     (503) staff       (20)        0 2023-07-12 18:55:32.000000 aim-4.0.2/src/python/aim/_sdk/interfaces/__init__.py
--rw-r--r--   0 github     (503) staff       (20)     1563 2023-09-19 20:11:49.000000 aim-4.0.2/src/python/aim/_sdk/interfaces/container.py
--rw-r--r--   0 github     (503) staff       (20)     2300 2023-07-25 12:19:13.000000 aim-4.0.2/src/python/aim/_sdk/interfaces/sequence.py
--rw-r--r--   0 github     (503) staff       (20)     3160 2023-07-19 20:10:38.000000 aim-4.0.2/src/python/aim/_sdk/local_storage.py
--rw-r--r--   0 github     (503) staff       (20)     5506 2023-10-03 16:38:51.000000 aim-4.0.2/src/python/aim/_sdk/lock_manager.py
--rw-r--r--   0 github     (503) staff       (20)     3397 2023-07-12 18:55:32.000000 aim-4.0.2/src/python/aim/_sdk/num_utils.py
--rw-r--r--   0 github     (503) staff       (20)     4349 2023-09-27 15:10:23.000000 aim-4.0.2/src/python/aim/_sdk/package_utils.py
--rw-r--r--   0 github     (503) staff       (20)     4221 2023-07-12 18:55:32.000000 aim-4.0.2/src/python/aim/_sdk/query.py
--rw-r--r--   0 github     (503) staff       (20)     3046 2023-07-12 18:55:32.000000 aim-4.0.2/src/python/aim/_sdk/query_utils.py
--rw-r--r--   0 github     (503) staff       (20)     2048 2023-09-19 20:11:49.000000 aim-4.0.2/src/python/aim/_sdk/record.py
--rw-r--r--   0 github     (503) staff       (20)    18237 2023-09-19 20:11:49.000000 aim-4.0.2/src/python/aim/_sdk/remote_storage.py
--rw-r--r--   0 github     (503) staff       (20)    20776 2023-09-27 17:12:13.000000 aim-4.0.2/src/python/aim/_sdk/repo.py
--rw-r--r--   0 github     (503) staff       (20)    14246 2023-09-26 20:09:35.000000 aim-4.0.2/src/python/aim/_sdk/sequence.py
--rw-r--r--   0 github     (503) staff       (20)      921 2023-07-12 18:55:32.000000 aim-4.0.2/src/python/aim/_sdk/storage_engine.py
--rw-r--r--   0 github     (503) staff       (20)     4112 2023-09-19 20:11:49.000000 aim-4.0.2/src/python/aim/_sdk/type_utils.py
--rw-r--r--   0 github     (503) staff       (20)      165 2023-07-12 18:55:32.000000 aim-4.0.2/src/python/aim/_sdk/types.py
--rw-r--r--   0 github     (503) staff       (20)     1479 2023-07-12 18:55:32.000000 aim-4.0.2/src/python/aim/_sdk/uri_service.py
--rw-r--r--   0 github     (503) staff       (20)     3723 2023-10-03 16:38:51.000000 aim-4.0.2/src/python/aim/_sdk/utils.py
--rw-r--r--   0 github     (503) staff       (20)       64 2023-09-05 20:15:25.000000 aim-4.0.2/src/python/aim/container.py
--rw-r--r--   0 github     (503) staff       (20)       48 2023-07-25 12:19:13.000000 aim-4.0.2/src/python/aim/record.py
--rw-r--r--   0 github     (503) staff       (20)       44 2023-07-12 18:55:32.000000 aim-4.0.2/src/python/aim/repo.py
--rw-r--r--   0 github     (503) staff       (20)       52 2023-07-12 18:55:32.000000 aim-4.0.2/src/python/aim/sequence.py
--rw-r--r--   0 github     (503) staff       (20)     5066 2023-09-08 20:15:11.000000 aim-4.0.2/src/python/aim/utils.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-10-04 15:23:30.813817 aim-4.0.3/
+-rw-r--r--   0 github     (503) staff       (20)    11347 2022-08-06 00:13:01.000000 aim-4.0.3/LICENSE
+-rw-r--r--   0 github     (503) staff       (20)      214 2023-07-12 18:55:32.000000 aim-4.0.3/MANIFEST.in
+-rw-r--r--   0 github     (503) staff       (20)    17821 2023-10-04 15:23:30.813570 aim-4.0.3/PKG-INFO
+-rw-r--r--   0 github     (503) staff       (20)    16398 2023-10-04 15:23:21.000000 aim-4.0.3/README.md
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-10-04 15:23:30.722315 aim-4.0.3/aim.egg-info/
+-rw-r--r--   0 github     (503) staff       (20)    17821 2023-10-04 15:23:30.000000 aim-4.0.3/aim.egg-info/PKG-INFO
+-rw-r--r--   0 github     (503) staff       (20)    18025 2023-10-04 15:23:30.000000 aim-4.0.3/aim.egg-info/SOURCES.txt
+-rw-r--r--   0 github     (503) staff       (20)        1 2023-10-04 15:23:30.000000 aim-4.0.3/aim.egg-info/dependency_links.txt
+-rw-r--r--   0 github     (503) staff       (20)      110 2023-10-04 15:23:30.000000 aim-4.0.3/aim.egg-info/entry_points.txt
+-rw-r--r--   0 github     (503) staff       (20)      381 2023-10-04 15:23:30.000000 aim-4.0.3/aim.egg-info/requires.txt
+-rw-r--r--   0 github     (503) staff       (20)       21 2023-10-04 15:23:30.000000 aim-4.0.3/aim.egg-info/top_level.txt
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-10-04 15:23:30.713033 aim-4.0.3/pkgs/
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-10-04 15:23:30.722425 aim-4.0.3/pkgs/aimstack/
+-rw-r--r--   0 github     (503) staff       (20)       24 2023-07-12 18:55:32.000000 aim-4.0.3/pkgs/aimstack/__init__.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-10-04 15:23:30.722708 aim-4.0.3/pkgs/aimstack/acme_tracker/
+-rw-r--r--   0 github     (503) staff       (20)      206 2023-10-04 15:23:21.000000 aim-4.0.3/pkgs/aimstack/acme_tracker/__init__.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-10-04 15:23:30.723076 aim-4.0.3/pkgs/aimstack/acme_tracker/boards/
+-rw-r--r--   0 github     (503) staff       (20)      122 2023-09-26 20:09:35.000000 aim-4.0.3/pkgs/aimstack/acme_tracker/boards/run.py
+-rw-r--r--   0 github     (503) staff       (20)       87 2023-09-26 20:09:35.000000 aim-4.0.3/pkgs/aimstack/acme_tracker/boards/runs.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-10-04 15:23:30.723496 aim-4.0.3/pkgs/aimstack/acme_tracker/callbacks/
+-rw-r--r--   0 github     (503) staff       (20)       83 2023-09-26 20:09:35.000000 aim-4.0.3/pkgs/aimstack/acme_tracker/callbacks/__init__.py
+-rw-r--r--   0 github     (503) staff       (20)     2857 2023-09-27 17:12:13.000000 aim-4.0.3/pkgs/aimstack/acme_tracker/callbacks/base_callback.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-10-04 15:23:30.724145 aim-4.0.3/pkgs/aimstack/base/
+-rw-r--r--   0 github     (503) staff       (20)      949 2023-09-27 15:10:23.000000 aim-4.0.3/pkgs/aimstack/base/__init__.py
+-rw-r--r--   0 github     (503) staff       (20)     1740 2023-09-27 15:10:23.000000 aim-4.0.3/pkgs/aimstack/base/actions.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-10-04 15:23:30.725808 aim-4.0.3/pkgs/aimstack/base/boards/
+-rw-r--r--   0 github     (503) staff       (20)     2900 2023-09-27 15:10:23.000000 aim-4.0.3/pkgs/aimstack/base/boards/audios.py
+-rw-r--r--   0 github     (503) staff       (20)     2926 2023-09-27 15:10:23.000000 aim-4.0.3/pkgs/aimstack/base/boards/figures.py
+-rw-r--r--   0 github     (503) staff       (20)     2900 2023-09-27 15:10:23.000000 aim-4.0.3/pkgs/aimstack/base/boards/images.py
+-rw-r--r--   0 github     (503) staff       (20)     3350 2023-09-27 15:10:23.000000 aim-4.0.3/pkgs/aimstack/base/boards/logs_overview.py
+-rw-r--r--   0 github     (503) staff       (20)     3719 2023-09-27 15:10:23.000000 aim-4.0.3/pkgs/aimstack/base/boards/metrics.py
+-rw-r--r--   0 github     (503) staff       (20)     1776 2023-09-27 15:10:23.000000 aim-4.0.3/pkgs/aimstack/base/boards/run.py
+-rw-r--r--   0 github     (503) staff       (20)     1956 2023-09-27 15:10:23.000000 aim-4.0.3/pkgs/aimstack/base/boards/runs.py
+-rw-r--r--   0 github     (503) staff       (20)     2873 2023-09-27 15:10:23.000000 aim-4.0.3/pkgs/aimstack/base/boards/texts.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-10-04 15:23:30.727650 aim-4.0.3/pkgs/aimstack/base/types/
+-rw-r--r--   0 github     (503) staff       (20)        0 2023-09-27 15:10:23.000000 aim-4.0.3/pkgs/aimstack/base/types/__init__.py
+-rw-r--r--   0 github     (503) staff       (20)     3315 2023-09-27 15:10:23.000000 aim-4.0.3/pkgs/aimstack/base/types/audio.py
+-rw-r--r--   0 github     (503) staff       (20)     4264 2023-09-27 15:10:23.000000 aim-4.0.3/pkgs/aimstack/base/types/distribution.py
+-rw-r--r--   0 github     (503) staff       (20)     5244 2023-09-27 15:10:23.000000 aim-4.0.3/pkgs/aimstack/base/types/figures.py
+-rw-r--r--   0 github     (503) staff       (20)    10080 2023-09-27 15:10:23.000000 aim-4.0.3/pkgs/aimstack/base/types/image.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-10-04 15:23:30.727898 aim-4.0.3/pkgs/aimstack/base/types/io/
+-rw-r--r--   0 github     (503) staff       (20)        0 2023-09-27 15:10:23.000000 aim-4.0.3/pkgs/aimstack/base/types/io/__init__.py
+-rw-r--r--   0 github     (503) staff       (20)    21094 2023-09-27 15:10:23.000000 aim-4.0.3/pkgs/aimstack/base/types/io/wavfile.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-10-04 15:23:30.728168 aim-4.0.3/pkgs/aimstack/base/types/logging/
+-rw-r--r--   0 github     (503) staff       (20)     1663 2023-09-27 15:10:23.000000 aim-4.0.3/pkgs/aimstack/base/types/logging/__init__.py
+-rw-r--r--   0 github     (503) staff       (20)     2567 2023-09-27 15:10:23.000000 aim-4.0.3/pkgs/aimstack/base/types/metric.py
+-rw-r--r--   0 github     (503) staff       (20)     8919 2023-10-03 17:16:26.000000 aim-4.0.3/pkgs/aimstack/base/types/run.py
+-rw-r--r--   0 github     (503) staff       (20)      718 2023-09-27 15:10:23.000000 aim-4.0.3/pkgs/aimstack/base/types/text.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-10-04 15:23:30.728338 aim-4.0.3/pkgs/aimstack/catboost_tracker/
+-rw-r--r--   0 github     (503) staff       (20)      210 2023-10-04 15:23:21.000000 aim-4.0.3/pkgs/aimstack/catboost_tracker/__init__.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-10-04 15:23:30.728609 aim-4.0.3/pkgs/aimstack/catboost_tracker/boards/
+-rw-r--r--   0 github     (503) staff       (20)      122 2023-09-26 20:09:35.000000 aim-4.0.3/pkgs/aimstack/catboost_tracker/boards/run.py
+-rw-r--r--   0 github     (503) staff       (20)       91 2023-09-26 20:09:35.000000 aim-4.0.3/pkgs/aimstack/catboost_tracker/boards/runs.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-10-04 15:23:30.728971 aim-4.0.3/pkgs/aimstack/catboost_tracker/loggers/
+-rw-r--r--   0 github     (503) staff       (20)       69 2023-09-26 20:09:35.000000 aim-4.0.3/pkgs/aimstack/catboost_tracker/loggers/__init__.py
+-rw-r--r--   0 github     (503) staff       (20)     3876 2023-09-26 20:09:35.000000 aim-4.0.3/pkgs/aimstack/catboost_tracker/loggers/base_logger.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-10-04 15:23:30.729140 aim-4.0.3/pkgs/aimstack/docs/
+-rw-r--r--   0 github     (503) staff       (20)      117 2023-09-27 15:10:23.000000 aim-4.0.3/pkgs/aimstack/docs/__init__.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-10-04 15:23:30.714038 aim-4.0.3/pkgs/aimstack/docs/boards/
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-10-04 15:23:30.730135 aim-4.0.3/pkgs/aimstack/docs/boards/sdk/
+-rw-r--r--   0 github     (503) staff       (20)     4528 2023-07-12 18:55:32.000000 aim-4.0.3/pkgs/aimstack/docs/boards/sdk/aim_types.py
+-rw-r--r--   0 github     (503) staff       (20)     4444 2023-07-12 18:55:32.000000 aim-4.0.3/pkgs/aimstack/docs/boards/sdk/container.py
+-rw-r--r--   0 github     (503) staff       (20)     5074 2023-09-27 15:10:23.000000 aim-4.0.3/pkgs/aimstack/docs/boards/sdk/overview.py
+-rw-r--r--   0 github     (503) staff       (20)     6979 2023-07-12 18:55:32.000000 aim-4.0.3/pkgs/aimstack/docs/boards/sdk/sequence.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-10-04 15:23:30.714566 aim-4.0.3/pkgs/aimstack/docs/boards/ui/
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-10-04 15:23:30.730525 aim-4.0.3/pkgs/aimstack/docs/boards/ui/board/
+-rw-r--r--   0 github     (503) staff       (20)      527 2023-07-12 18:55:32.000000 aim-4.0.3/pkgs/aimstack/docs/boards/ui/board/board.py
+-rw-r--r--   0 github     (503) staff       (20)      833 2023-07-12 18:55:32.000000 aim-4.0.3/pkgs/aimstack/docs/boards/ui/board/board_link.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-10-04 15:23:30.730883 aim-4.0.3/pkgs/aimstack/docs/boards/ui/charts/
+-rw-r--r--   0 github     (503) staff       (20)     1547 2023-07-12 18:55:32.000000 aim-4.0.3/pkgs/aimstack/docs/boards/ui/charts/line_chart.py
+-rw-r--r--   0 github     (503) staff       (20)     1001 2023-07-12 18:55:32.000000 aim-4.0.3/pkgs/aimstack/docs/boards/ui/charts/plotly.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-10-04 15:23:30.731392 aim-4.0.3/pkgs/aimstack/docs/boards/ui/data_viz/
+-rw-r--r--   0 github     (503) staff       (20)      764 2023-07-12 18:55:32.000000 aim-4.0.3/pkgs/aimstack/docs/boards/ui/data_viz/dataframe.py
+-rw-r--r--   0 github     (503) staff       (20)      713 2023-07-12 18:55:32.000000 aim-4.0.3/pkgs/aimstack/docs/boards/ui/data_viz/json.py
+-rw-r--r--   0 github     (503) staff       (20)      702 2023-07-12 18:55:32.000000 aim-4.0.3/pkgs/aimstack/docs/boards/ui/data_viz/table.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-10-04 15:23:30.732025 aim-4.0.3/pkgs/aimstack/docs/boards/ui/examples/
+-rw-r--r--   0 github     (503) staff       (20)     1967 2023-09-27 15:10:23.000000 aim-4.0.3/pkgs/aimstack/docs/boards/ui/examples/charts.py
+-rw-r--r--   0 github     (503) staff       (20)      900 2023-09-27 15:10:23.000000 aim-4.0.3/pkgs/aimstack/docs/boards/ui/examples/data_display_elements.py
+-rw-r--r--   0 github     (503) staff       (20)     3820 2023-09-27 15:10:23.000000 aim-4.0.3/pkgs/aimstack/docs/boards/ui/examples/input_components.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-10-04 15:23:30.734117 aim-4.0.3/pkgs/aimstack/docs/boards/ui/input/
+-rw-r--r--   0 github     (503) staff       (20)      728 2023-07-12 18:55:32.000000 aim-4.0.3/pkgs/aimstack/docs/boards/ui/input/checkbox.py
+-rw-r--r--   0 github     (503) staff       (20)     1207 2023-07-12 18:55:32.000000 aim-4.0.3/pkgs/aimstack/docs/boards/ui/input/multi_select.py
+-rw-r--r--   0 github     (503) staff       (20)     1153 2023-07-12 18:55:32.000000 aim-4.0.3/pkgs/aimstack/docs/boards/ui/input/number_input.py
+-rw-r--r--   0 github     (503) staff       (20)     1400 2023-07-12 18:55:32.000000 aim-4.0.3/pkgs/aimstack/docs/boards/ui/input/radio.py
+-rw-r--r--   0 github     (503) staff       (20)     1173 2023-07-12 18:55:32.000000 aim-4.0.3/pkgs/aimstack/docs/boards/ui/input/range_slider.py
+-rw-r--r--   0 github     (503) staff       (20)     1007 2023-07-12 18:55:32.000000 aim-4.0.3/pkgs/aimstack/docs/boards/ui/input/select.py
+-rw-r--r--   0 github     (503) staff       (20)     1067 2023-07-12 18:55:32.000000 aim-4.0.3/pkgs/aimstack/docs/boards/ui/input/slider.py
+-rw-r--r--   0 github     (503) staff       (20)      937 2023-07-12 18:55:32.000000 aim-4.0.3/pkgs/aimstack/docs/boards/ui/input/switch.py
+-rw-r--r--   0 github     (503) staff       (20)     1000 2023-07-12 18:55:32.000000 aim-4.0.3/pkgs/aimstack/docs/boards/ui/input/text_area.py
+-rw-r--r--   0 github     (503) staff       (20)      751 2023-07-12 18:55:32.000000 aim-4.0.3/pkgs/aimstack/docs/boards/ui/input/text_input.py
+-rw-r--r--   0 github     (503) staff       (20)     1182 2023-07-12 18:55:32.000000 aim-4.0.3/pkgs/aimstack/docs/boards/ui/input/toggle_button.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-10-04 15:23:30.734950 aim-4.0.3/pkgs/aimstack/docs/boards/ui/layout_containers/
+-rw-r--r--   0 github     (503) staff       (20)     1141 2023-07-12 18:55:32.000000 aim-4.0.3/pkgs/aimstack/docs/boards/ui/layout_containers/columns.py
+-rw-r--r--   0 github     (503) staff       (20)     1125 2023-07-12 18:55:32.000000 aim-4.0.3/pkgs/aimstack/docs/boards/ui/layout_containers/form.py
+-rw-r--r--   0 github     (503) staff       (20)     1023 2023-07-12 18:55:32.000000 aim-4.0.3/pkgs/aimstack/docs/boards/ui/layout_containers/rows.py
+-rw-r--r--   0 github     (503) staff       (20)     1452 2023-07-12 18:55:32.000000 aim-4.0.3/pkgs/aimstack/docs/boards/ui/layout_containers/tabs.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-10-04 15:23:30.735638 aim-4.0.3/pkgs/aimstack/docs/boards/ui/sequence_viz/
+-rw-r--r--   0 github     (503) staff       (20)      415 2023-09-27 15:10:23.000000 aim-4.0.3/pkgs/aimstack/docs/boards/ui/sequence_viz/audios.py
+-rw-r--r--   0 github     (503) staff       (20)      423 2023-09-27 15:10:23.000000 aim-4.0.3/pkgs/aimstack/docs/boards/ui/sequence_viz/figures.py
+-rw-r--r--   0 github     (503) staff       (20)      415 2023-09-27 15:10:23.000000 aim-4.0.3/pkgs/aimstack/docs/boards/ui/sequence_viz/images.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-10-04 15:23:30.736912 aim-4.0.3/pkgs/aimstack/docs/boards/ui/text/
+-rw-r--r--   0 github     (503) staff       (20)      524 2023-07-12 18:55:32.000000 aim-4.0.3/pkgs/aimstack/docs/boards/ui/text/code.py
+-rw-r--r--   0 github     (503) staff       (20)      428 2023-07-12 18:55:32.000000 aim-4.0.3/pkgs/aimstack/docs/boards/ui/text/header.py
+-rw-r--r--   0 github     (503) staff       (20)      477 2023-07-12 18:55:32.000000 aim-4.0.3/pkgs/aimstack/docs/boards/ui/text/html.py
+-rw-r--r--   0 github     (503) staff       (20)      606 2023-07-12 18:55:32.000000 aim-4.0.3/pkgs/aimstack/docs/boards/ui/text/link.py
+-rw-r--r--   0 github     (503) staff       (20)      461 2023-07-12 18:55:32.000000 aim-4.0.3/pkgs/aimstack/docs/boards/ui/text/markdown.py
+-rw-r--r--   0 github     (503) staff       (20)      452 2023-07-12 18:55:32.000000 aim-4.0.3/pkgs/aimstack/docs/boards/ui/text/subheader.py
+-rw-r--r--   0 github     (503) staff       (20)      434 2023-07-12 18:55:32.000000 aim-4.0.3/pkgs/aimstack/docs/boards/ui/text/text.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-10-04 15:23:30.739404 aim-4.0.3/pkgs/aimstack/experiment_tracker/
+-rw-r--r--   0 github     (503) staff       (20)      239 2023-09-27 15:10:23.000000 aim-4.0.3/pkgs/aimstack/experiment_tracker/__init__.py
+-rw-r--r--   0 github     (503) staff       (20)      113 2023-10-04 15:23:21.000000 aim-4.0.3/pkgs/aimstack/experiment_tracker/acme.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-10-04 15:23:30.739723 aim-4.0.3/pkgs/aimstack/experiment_tracker/boards/
+-rw-r--r--   0 github     (503) staff       (20)     1831 2023-09-27 15:10:23.000000 aim-4.0.3/pkgs/aimstack/experiment_tracker/boards/run.py
+-rw-r--r--   0 github     (503) staff       (20)     2068 2023-09-26 20:09:35.000000 aim-4.0.3/pkgs/aimstack/experiment_tracker/boards/runs.py
+-rw-r--r--   0 github     (503) staff       (20)       87 2023-10-04 15:23:21.000000 aim-4.0.3/pkgs/aimstack/experiment_tracker/catboost.py
+-rw-r--r--   0 github     (503) staff       (20)       93 2023-10-04 15:23:21.000000 aim-4.0.3/pkgs/aimstack/experiment_tracker/fastai.py
+-rw-r--r--   0 github     (503) staff       (20)       99 2023-10-04 15:23:21.000000 aim-4.0.3/pkgs/aimstack/experiment_tracker/hugging_face.py
+-rw-r--r--   0 github     (503) staff       (20)       92 2023-10-04 15:23:21.000000 aim-4.0.3/pkgs/aimstack/experiment_tracker/keras.py
+-rw-r--r--   0 github     (503) staff       (20)       98 2023-10-04 15:23:21.000000 aim-4.0.3/pkgs/aimstack/experiment_tracker/keras_tuner.py
+-rw-r--r--   0 github     (503) staff       (20)       94 2023-10-04 15:23:21.000000 aim-4.0.3/pkgs/aimstack/experiment_tracker/lightgbm.py
+-rw-r--r--   0 github     (503) staff       (20)       77 2023-10-04 15:23:21.000000 aim-4.0.3/pkgs/aimstack/experiment_tracker/mxnet.py
+-rw-r--r--   0 github     (503) staff       (20)       92 2023-10-04 15:23:21.000000 aim-4.0.3/pkgs/aimstack/experiment_tracker/optuna.py
+-rw-r--r--   0 github     (503) staff       (20)       93 2023-10-04 15:23:21.000000 aim-4.0.3/pkgs/aimstack/experiment_tracker/paddle.py
+-rw-r--r--   0 github     (503) staff       (20)       86 2023-10-04 15:23:21.000000 aim-4.0.3/pkgs/aimstack/experiment_tracker/prophet.py
+-rw-r--r--   0 github     (503) staff       (20)      117 2023-10-04 15:23:21.000000 aim-4.0.3/pkgs/aimstack/experiment_tracker/pytorch_ignite.py
+-rw-r--r--   0 github     (503) staff       (20)       95 2023-10-04 15:23:21.000000 aim-4.0.3/pkgs/aimstack/experiment_tracker/pytorch_lightning.py
+-rw-r--r--   0 github     (503) staff       (20)       89 2023-10-04 15:23:21.000000 aim-4.0.3/pkgs/aimstack/experiment_tracker/sb3.py
+-rw-r--r--   0 github     (503) staff       (20)       96 2023-10-04 15:23:21.000000 aim-4.0.3/pkgs/aimstack/experiment_tracker/tensorflow.py
+-rw-r--r--   0 github     (503) staff       (20)     2129 2023-09-27 15:10:23.000000 aim-4.0.3/pkgs/aimstack/experiment_tracker/training_flow.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-10-04 15:23:30.740801 aim-4.0.3/pkgs/aimstack/experiment_tracker/types/
+-rw-r--r--   0 github     (503) staff       (20)        0 2023-09-26 20:09:35.000000 aim-4.0.3/pkgs/aimstack/experiment_tracker/types/__init__.py
+-rw-r--r--   0 github     (503) staff       (20)     6055 2023-09-27 15:10:23.000000 aim-4.0.3/pkgs/aimstack/experiment_tracker/types/deeplake_dataset.py
+-rw-r--r--   0 github     (503) staff       (20)     1921 2023-09-27 15:10:23.000000 aim-4.0.3/pkgs/aimstack/experiment_tracker/types/dvc_metadata.py
+-rw-r--r--   0 github     (503) staff       (20)     3578 2023-09-27 15:10:23.000000 aim-4.0.3/pkgs/aimstack/experiment_tracker/types/hf_datasets_metadata.py
+-rw-r--r--   0 github     (503) staff       (20)      141 2023-09-27 15:10:23.000000 aim-4.0.3/pkgs/aimstack/experiment_tracker/types/training_run.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-10-04 15:23:30.741168 aim-4.0.3/pkgs/aimstack/experiment_tracker/utils/
+-rw-r--r--   0 github     (503) staff       (20)        0 2023-09-26 20:09:35.000000 aim-4.0.3/pkgs/aimstack/experiment_tracker/utils/__init__.py
+-rw-r--r--   0 github     (503) staff       (20)     2524 2023-09-27 15:10:23.000000 aim-4.0.3/pkgs/aimstack/experiment_tracker/utils/pytorch.py
+-rw-r--r--   0 github     (503) staff       (20)       94 2023-10-04 15:23:21.000000 aim-4.0.3/pkgs/aimstack/experiment_tracker/xgboost.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-10-04 15:23:30.741377 aim-4.0.3/pkgs/aimstack/fastai_tracker/
+-rw-r--r--   0 github     (503) staff       (20)      209 2023-10-04 15:23:21.000000 aim-4.0.3/pkgs/aimstack/fastai_tracker/__init__.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-10-04 15:23:30.741715 aim-4.0.3/pkgs/aimstack/fastai_tracker/boards/
+-rw-r--r--   0 github     (503) staff       (20)      122 2023-09-26 20:09:35.000000 aim-4.0.3/pkgs/aimstack/fastai_tracker/boards/run.py
+-rw-r--r--   0 github     (503) staff       (20)       89 2023-09-26 20:09:35.000000 aim-4.0.3/pkgs/aimstack/fastai_tracker/boards/runs.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-10-04 15:23:30.742108 aim-4.0.3/pkgs/aimstack/fastai_tracker/callbacks/
+-rw-r--r--   0 github     (503) staff       (20)       73 2023-09-26 20:09:35.000000 aim-4.0.3/pkgs/aimstack/fastai_tracker/callbacks/__init__.py
+-rw-r--r--   0 github     (503) staff       (20)     5696 2023-09-27 17:12:13.000000 aim-4.0.3/pkgs/aimstack/fastai_tracker/callbacks/base_callback.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-10-04 15:23:30.742576 aim-4.0.3/pkgs/aimstack/hugging_face_tracker/
+-rw-r--r--   0 github     (503) staff       (20)      213 2023-10-04 15:23:21.000000 aim-4.0.3/pkgs/aimstack/hugging_face_tracker/__init__.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-10-04 15:23:30.742908 aim-4.0.3/pkgs/aimstack/hugging_face_tracker/boards/
+-rw-r--r--   0 github     (503) staff       (20)      122 2023-09-26 20:09:35.000000 aim-4.0.3/pkgs/aimstack/hugging_face_tracker/boards/run.py
+-rw-r--r--   0 github     (503) staff       (20)       95 2023-09-26 20:09:35.000000 aim-4.0.3/pkgs/aimstack/hugging_face_tracker/boards/runs.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-10-04 15:23:30.743564 aim-4.0.3/pkgs/aimstack/hugging_face_tracker/callbacks/
+-rw-r--r--   0 github     (503) staff       (20)       79 2023-09-26 20:09:35.000000 aim-4.0.3/pkgs/aimstack/hugging_face_tracker/callbacks/__init__.py
+-rw-r--r--   0 github     (503) staff       (20)     5795 2023-09-26 20:09:35.000000 aim-4.0.3/pkgs/aimstack/hugging_face_tracker/callbacks/base_callback.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-10-04 15:23:30.743873 aim-4.0.3/pkgs/aimstack/keras_tracker/
+-rw-r--r--   0 github     (503) staff       (20)      207 2023-10-04 15:23:21.000000 aim-4.0.3/pkgs/aimstack/keras_tracker/__init__.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-10-04 15:23:30.744413 aim-4.0.3/pkgs/aimstack/keras_tracker/boards/
+-rw-r--r--   0 github     (503) staff       (20)      122 2023-09-26 20:09:35.000000 aim-4.0.3/pkgs/aimstack/keras_tracker/boards/run.py
+-rw-r--r--   0 github     (503) staff       (20)       88 2023-09-26 20:09:35.000000 aim-4.0.3/pkgs/aimstack/keras_tracker/boards/runs.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-10-04 15:23:30.744759 aim-4.0.3/pkgs/aimstack/keras_tracker/callbacks/
+-rw-r--r--   0 github     (503) staff       (20)       72 2023-09-26 20:09:35.000000 aim-4.0.3/pkgs/aimstack/keras_tracker/callbacks/__init__.py
+-rw-r--r--   0 github     (503) staff       (20)     2346 2023-09-27 17:12:13.000000 aim-4.0.3/pkgs/aimstack/keras_tracker/callbacks/base_callback.py
+-rw-r--r--   0 github     (503) staff       (20)     1145 2023-09-26 20:09:35.000000 aim-4.0.3/pkgs/aimstack/keras_tracker/mixins.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-10-04 15:23:30.745019 aim-4.0.3/pkgs/aimstack/keras_tuner_tracker/
+-rw-r--r--   0 github     (503) staff       (20)      212 2023-10-04 15:23:21.000000 aim-4.0.3/pkgs/aimstack/keras_tuner_tracker/__init__.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-10-04 15:23:30.745311 aim-4.0.3/pkgs/aimstack/keras_tuner_tracker/boards/
+-rw-r--r--   0 github     (503) staff       (20)      122 2023-09-26 20:09:35.000000 aim-4.0.3/pkgs/aimstack/keras_tuner_tracker/boards/run.py
+-rw-r--r--   0 github     (503) staff       (20)       94 2023-09-26 20:09:35.000000 aim-4.0.3/pkgs/aimstack/keras_tuner_tracker/boards/runs.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-10-04 15:23:30.745643 aim-4.0.3/pkgs/aimstack/keras_tuner_tracker/callbacks/
+-rw-r--r--   0 github     (503) staff       (20)       78 2023-09-26 20:09:35.000000 aim-4.0.3/pkgs/aimstack/keras_tuner_tracker/callbacks/__init__.py
+-rw-r--r--   0 github     (503) staff       (20)     2664 2023-09-26 20:09:35.000000 aim-4.0.3/pkgs/aimstack/keras_tuner_tracker/callbacks/base_callback.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-10-04 15:23:30.745823 aim-4.0.3/pkgs/aimstack/langchain_debugger/
+-rw-r--r--   0 github     (503) staff       (20)      425 2023-09-27 15:10:23.000000 aim-4.0.3/pkgs/aimstack/langchain_debugger/__init__.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-10-04 15:23:30.748058 aim-4.0.3/pkgs/aimstack/langchain_debugger/boards/
+-rw-r--r--   0 github     (503) staff       (20)     3366 2023-09-27 15:10:23.000000 aim-4.0.3/pkgs/aimstack/langchain_debugger/boards/cost.py
+-rw-r--r--   0 github     (503) staff       (20)     5148 2023-09-27 15:10:23.000000 aim-4.0.3/pkgs/aimstack/langchain_debugger/boards/steps.py
+-rw-r--r--   0 github     (503) staff       (20)     2490 2023-09-27 15:10:23.000000 aim-4.0.3/pkgs/aimstack/langchain_debugger/boards/trace.py
+-rw-r--r--   0 github     (503) staff       (20)     2224 2023-09-27 15:10:23.000000 aim-4.0.3/pkgs/aimstack/langchain_debugger/boards/traces.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-10-04 15:23:30.748437 aim-4.0.3/pkgs/aimstack/langchain_debugger/callback_handlers/
+-rw-r--r--   0 github     (503) staff       (20)      106 2023-09-27 15:10:23.000000 aim-4.0.3/pkgs/aimstack/langchain_debugger/callback_handlers/__init__.py
+-rw-r--r--   0 github     (503) staff       (20)    11520 2023-09-27 15:10:23.000000 aim-4.0.3/pkgs/aimstack/langchain_debugger/callback_handlers/generic_callback_handler.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-10-04 15:23:30.749217 aim-4.0.3/pkgs/aimstack/langchain_debugger/types/
+-rw-r--r--   0 github     (503) staff       (20)      128 2023-09-27 15:10:23.000000 aim-4.0.3/pkgs/aimstack/langchain_debugger/types/__init__.py
+-rw-r--r--   0 github     (503) staff       (20)     4445 2023-09-27 15:10:23.000000 aim-4.0.3/pkgs/aimstack/langchain_debugger/types/action.py
+-rw-r--r--   0 github     (503) staff       (20)     1800 2023-09-27 15:10:23.000000 aim-4.0.3/pkgs/aimstack/langchain_debugger/types/step.py
+-rw-r--r--   0 github     (503) staff       (20)      660 2023-09-27 15:10:23.000000 aim-4.0.3/pkgs/aimstack/langchain_debugger/types/trace.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-10-04 15:23:30.749395 aim-4.0.3/pkgs/aimstack/lightgbm_tracker/
+-rw-r--r--   0 github     (503) staff       (20)      210 2023-10-04 15:23:21.000000 aim-4.0.3/pkgs/aimstack/lightgbm_tracker/__init__.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-10-04 15:23:30.749720 aim-4.0.3/pkgs/aimstack/lightgbm_tracker/boards/
+-rw-r--r--   0 github     (503) staff       (20)      122 2023-09-26 20:09:35.000000 aim-4.0.3/pkgs/aimstack/lightgbm_tracker/boards/run.py
+-rw-r--r--   0 github     (503) staff       (20)       91 2023-09-26 20:09:35.000000 aim-4.0.3/pkgs/aimstack/lightgbm_tracker/boards/runs.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-10-04 15:23:30.750159 aim-4.0.3/pkgs/aimstack/lightgbm_tracker/callbacks/
+-rw-r--r--   0 github     (503) staff       (20)       75 2023-09-26 20:09:35.000000 aim-4.0.3/pkgs/aimstack/lightgbm_tracker/callbacks/__init__.py
+-rw-r--r--   0 github     (503) staff       (20)     3520 2023-09-27 17:12:13.000000 aim-4.0.3/pkgs/aimstack/lightgbm_tracker/callbacks/base_callback.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-10-04 15:23:30.750427 aim-4.0.3/pkgs/aimstack/llamaindex_observer/
+-rw-r--r--   0 github     (503) staff       (20)      453 2023-09-27 15:10:23.000000 aim-4.0.3/pkgs/aimstack/llamaindex_observer/__init__.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-10-04 15:23:30.751144 aim-4.0.3/pkgs/aimstack/llamaindex_observer/boards/
+-rw-r--r--   0 github     (503) staff       (20)     3365 2023-09-27 15:10:23.000000 aim-4.0.3/pkgs/aimstack/llamaindex_observer/boards/cost.py
+-rw-r--r--   0 github     (503) staff       (20)     5922 2023-09-27 15:10:23.000000 aim-4.0.3/pkgs/aimstack/llamaindex_observer/boards/steps.py
+-rw-r--r--   0 github     (503) staff       (20)     2555 2023-09-27 15:10:23.000000 aim-4.0.3/pkgs/aimstack/llamaindex_observer/boards/trace.py
+-rw-r--r--   0 github     (503) staff       (20)     2007 2023-09-27 15:10:23.000000 aim-4.0.3/pkgs/aimstack/llamaindex_observer/boards/traces.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-10-04 15:23:30.751524 aim-4.0.3/pkgs/aimstack/llamaindex_observer/callback_handlers/
+-rw-r--r--   0 github     (503) staff       (20)      107 2023-09-27 15:10:23.000000 aim-4.0.3/pkgs/aimstack/llamaindex_observer/callback_handlers/__init__.py
+-rw-r--r--   0 github     (503) staff       (20)    11232 2023-09-27 15:10:23.000000 aim-4.0.3/pkgs/aimstack/llamaindex_observer/callback_handlers/generic_callback_handler.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-10-04 15:23:30.752433 aim-4.0.3/pkgs/aimstack/llamaindex_observer/types/
+-rw-r--r--   0 github     (503) staff       (20)      130 2023-09-27 15:10:23.000000 aim-4.0.3/pkgs/aimstack/llamaindex_observer/types/__init__.py
+-rw-r--r--   0 github     (503) staff       (20)     4080 2023-09-27 15:10:23.000000 aim-4.0.3/pkgs/aimstack/llamaindex_observer/types/action.py
+-rw-r--r--   0 github     (503) staff       (20)     1544 2023-09-27 15:10:23.000000 aim-4.0.3/pkgs/aimstack/llamaindex_observer/types/step.py
+-rw-r--r--   0 github     (503) staff       (20)      640 2023-09-27 15:10:23.000000 aim-4.0.3/pkgs/aimstack/llamaindex_observer/types/trace.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-10-04 15:23:30.752617 aim-4.0.3/pkgs/aimstack/mxnet_tracker/
+-rw-r--r--   0 github     (503) staff       (20)      207 2023-10-04 15:23:21.000000 aim-4.0.3/pkgs/aimstack/mxnet_tracker/__init__.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-10-04 15:23:30.752910 aim-4.0.3/pkgs/aimstack/mxnet_tracker/boards/
+-rw-r--r--   0 github     (503) staff       (20)      122 2023-09-26 20:09:35.000000 aim-4.0.3/pkgs/aimstack/mxnet_tracker/boards/run.py
+-rw-r--r--   0 github     (503) staff       (20)       88 2023-09-26 20:09:35.000000 aim-4.0.3/pkgs/aimstack/mxnet_tracker/boards/runs.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-10-04 15:23:30.753284 aim-4.0.3/pkgs/aimstack/mxnet_tracker/loggers/
+-rw-r--r--   0 github     (503) staff       (20)       70 2023-09-26 20:09:35.000000 aim-4.0.3/pkgs/aimstack/mxnet_tracker/loggers/__init__.py
+-rw-r--r--   0 github     (503) staff       (20)     8250 2023-09-27 17:12:13.000000 aim-4.0.3/pkgs/aimstack/mxnet_tracker/loggers/base_logger.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-10-04 15:23:30.753565 aim-4.0.3/pkgs/aimstack/optuna_tracker/
+-rw-r--r--   0 github     (503) staff       (20)      208 2023-10-04 15:23:21.000000 aim-4.0.3/pkgs/aimstack/optuna_tracker/__init__.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-10-04 15:23:30.753883 aim-4.0.3/pkgs/aimstack/optuna_tracker/boards/
+-rw-r--r--   0 github     (503) staff       (20)      122 2023-09-26 20:09:35.000000 aim-4.0.3/pkgs/aimstack/optuna_tracker/boards/run.py
+-rw-r--r--   0 github     (503) staff       (20)       89 2023-09-26 20:09:35.000000 aim-4.0.3/pkgs/aimstack/optuna_tracker/boards/runs.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-10-04 15:23:30.754245 aim-4.0.3/pkgs/aimstack/optuna_tracker/callbacks/
+-rw-r--r--   0 github     (503) staff       (20)       74 2023-09-26 20:09:35.000000 aim-4.0.3/pkgs/aimstack/optuna_tracker/callbacks/__init__.py
+-rw-r--r--   0 github     (503) staff       (20)     6530 2023-09-27 17:12:13.000000 aim-4.0.3/pkgs/aimstack/optuna_tracker/callbacks/base_callback.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-10-04 15:23:30.754634 aim-4.0.3/pkgs/aimstack/paddle_tracker/
+-rw-r--r--   0 github     (503) staff       (20)      214 2023-10-04 15:23:21.000000 aim-4.0.3/pkgs/aimstack/paddle_tracker/__init__.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-10-04 15:23:30.754983 aim-4.0.3/pkgs/aimstack/paddle_tracker/boards/
+-rw-r--r--   0 github     (503) staff       (20)      122 2023-09-26 20:09:35.000000 aim-4.0.3/pkgs/aimstack/paddle_tracker/boards/run.py
+-rw-r--r--   0 github     (503) staff       (20)       89 2023-09-26 20:09:35.000000 aim-4.0.3/pkgs/aimstack/paddle_tracker/boards/runs.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-10-04 15:23:30.755379 aim-4.0.3/pkgs/aimstack/paddle_tracker/callbacks/
+-rw-r--r--   0 github     (503) staff       (20)       73 2023-09-26 20:09:35.000000 aim-4.0.3/pkgs/aimstack/paddle_tracker/callbacks/__init__.py
+-rw-r--r--   0 github     (503) staff       (20)     2744 2023-09-27 17:12:13.000000 aim-4.0.3/pkgs/aimstack/paddle_tracker/callbacks/base_callback.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-10-04 15:23:30.755560 aim-4.0.3/pkgs/aimstack/prophet_tracker/
+-rw-r--r--   0 github     (503) staff       (20)      212 2023-10-04 15:23:21.000000 aim-4.0.3/pkgs/aimstack/prophet_tracker/__init__.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-10-04 15:23:30.755842 aim-4.0.3/pkgs/aimstack/prophet_tracker/boards/
+-rw-r--r--   0 github     (503) staff       (20)      122 2023-09-26 20:09:35.000000 aim-4.0.3/pkgs/aimstack/prophet_tracker/boards/run.py
+-rw-r--r--   0 github     (503) staff       (20)       90 2023-09-26 20:09:35.000000 aim-4.0.3/pkgs/aimstack/prophet_tracker/boards/runs.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-10-04 15:23:30.756190 aim-4.0.3/pkgs/aimstack/prophet_tracker/loggers/
+-rw-r--r--   0 github     (503) staff       (20)       68 2023-09-26 20:09:35.000000 aim-4.0.3/pkgs/aimstack/prophet_tracker/loggers/__init__.py
+-rw-r--r--   0 github     (503) staff       (20)     3003 2023-09-27 17:12:13.000000 aim-4.0.3/pkgs/aimstack/prophet_tracker/loggers/base_logger.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-10-04 15:23:30.756349 aim-4.0.3/pkgs/aimstack/pytorch_ignite_tracker/
+-rw-r--r--   0 github     (503) staff       (20)      216 2023-10-04 15:23:21.000000 aim-4.0.3/pkgs/aimstack/pytorch_ignite_tracker/__init__.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-10-04 15:23:30.756656 aim-4.0.3/pkgs/aimstack/pytorch_ignite_tracker/boards/
+-rw-r--r--   0 github     (503) staff       (20)      122 2023-09-26 20:09:35.000000 aim-4.0.3/pkgs/aimstack/pytorch_ignite_tracker/boards/run.py
+-rw-r--r--   0 github     (503) staff       (20)       97 2023-09-26 20:09:35.000000 aim-4.0.3/pkgs/aimstack/pytorch_ignite_tracker/boards/runs.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-10-04 15:23:30.756985 aim-4.0.3/pkgs/aimstack/pytorch_ignite_tracker/loggers/
+-rw-r--r--   0 github     (503) staff       (20)      110 2023-09-26 20:09:35.000000 aim-4.0.3/pkgs/aimstack/pytorch_ignite_tracker/loggers/__init__.py
+-rw-r--r--   0 github     (503) staff       (20)     8692 2023-09-27 17:12:13.000000 aim-4.0.3/pkgs/aimstack/pytorch_ignite_tracker/loggers/base_logger.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-10-04 15:23:30.757168 aim-4.0.3/pkgs/aimstack/pytorch_lightning_tracker/
+-rw-r--r--   0 github     (503) staff       (20)      219 2023-10-04 15:23:21.000000 aim-4.0.3/pkgs/aimstack/pytorch_lightning_tracker/__init__.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-10-04 15:23:30.757421 aim-4.0.3/pkgs/aimstack/pytorch_lightning_tracker/boards/
+-rw-r--r--   0 github     (503) staff       (20)      122 2023-09-26 20:09:35.000000 aim-4.0.3/pkgs/aimstack/pytorch_lightning_tracker/boards/run.py
+-rw-r--r--   0 github     (503) staff       (20)      100 2023-09-26 20:09:35.000000 aim-4.0.3/pkgs/aimstack/pytorch_lightning_tracker/boards/runs.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-10-04 15:23:30.757785 aim-4.0.3/pkgs/aimstack/pytorch_lightning_tracker/loggers/
+-rw-r--r--   0 github     (503) staff       (20)       78 2023-09-26 20:09:35.000000 aim-4.0.3/pkgs/aimstack/pytorch_lightning_tracker/loggers/__init__.py
+-rw-r--r--   0 github     (503) staff       (20)     6217 2023-09-27 17:12:13.000000 aim-4.0.3/pkgs/aimstack/pytorch_lightning_tracker/loggers/base_logger.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-10-04 15:23:30.757966 aim-4.0.3/pkgs/aimstack/sb3_tracker/
+-rw-r--r--   0 github     (503) staff       (20)      219 2023-10-04 15:23:21.000000 aim-4.0.3/pkgs/aimstack/sb3_tracker/__init__.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-10-04 15:23:30.758305 aim-4.0.3/pkgs/aimstack/sb3_tracker/boards/
+-rw-r--r--   0 github     (503) staff       (20)      122 2023-09-26 20:09:35.000000 aim-4.0.3/pkgs/aimstack/sb3_tracker/boards/run.py
+-rw-r--r--   0 github     (503) staff       (20)       86 2023-09-26 20:09:35.000000 aim-4.0.3/pkgs/aimstack/sb3_tracker/boards/runs.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-10-04 15:23:30.758631 aim-4.0.3/pkgs/aimstack/sb3_tracker/callbacks/
+-rw-r--r--   0 github     (503) staff       (20)       70 2023-09-26 20:09:35.000000 aim-4.0.3/pkgs/aimstack/sb3_tracker/callbacks/__init__.py
+-rw-r--r--   0 github     (503) staff       (20)     3897 2023-09-27 17:12:13.000000 aim-4.0.3/pkgs/aimstack/sb3_tracker/callbacks/base_callback.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-10-04 15:23:30.759291 aim-4.0.3/pkgs/aimstack/tensorboard_sync/
+-rw-r--r--   0 github     (503) staff       (20)       23 2023-09-27 15:10:23.000000 aim-4.0.3/pkgs/aimstack/tensorboard_sync/__init__.py
+-rw-r--r--   0 github     (503) staff       (20)     1273 2023-07-12 18:55:32.000000 aim-4.0.3/pkgs/aimstack/tensorboard_sync/run.py
+-rw-r--r--   0 github     (503) staff       (20)     9323 2023-07-12 18:55:32.000000 aim-4.0.3/pkgs/aimstack/tensorboard_sync/tracker.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-10-04 15:23:30.765378 aim-4.0.3/pkgs/aimstack/tensorflow_tracker/
+-rw-r--r--   0 github     (503) staff       (20)      212 2023-10-04 15:23:21.000000 aim-4.0.3/pkgs/aimstack/tensorflow_tracker/__init__.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-10-04 15:23:30.765678 aim-4.0.3/pkgs/aimstack/tensorflow_tracker/boards/
+-rw-r--r--   0 github     (503) staff       (20)      122 2023-09-26 20:09:35.000000 aim-4.0.3/pkgs/aimstack/tensorflow_tracker/boards/run.py
+-rw-r--r--   0 github     (503) staff       (20)       93 2023-09-26 20:09:35.000000 aim-4.0.3/pkgs/aimstack/tensorflow_tracker/boards/runs.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-10-04 15:23:30.766129 aim-4.0.3/pkgs/aimstack/tensorflow_tracker/callbacks/
+-rw-r--r--   0 github     (503) staff       (20)       77 2023-09-26 20:09:35.000000 aim-4.0.3/pkgs/aimstack/tensorflow_tracker/callbacks/__init__.py
+-rw-r--r--   0 github     (503) staff       (20)     2593 2023-09-27 17:12:13.000000 aim-4.0.3/pkgs/aimstack/tensorflow_tracker/callbacks/base_callback.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-10-04 15:23:30.766455 aim-4.0.3/pkgs/aimstack/xgboost_tracker/
+-rw-r--r--   0 github     (503) staff       (20)      209 2023-10-04 15:23:21.000000 aim-4.0.3/pkgs/aimstack/xgboost_tracker/__init__.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-10-04 15:23:30.766819 aim-4.0.3/pkgs/aimstack/xgboost_tracker/boards/
+-rw-r--r--   0 github     (503) staff       (20)      122 2023-09-26 20:09:35.000000 aim-4.0.3/pkgs/aimstack/xgboost_tracker/boards/run.py
+-rw-r--r--   0 github     (503) staff       (20)       90 2023-09-26 20:09:35.000000 aim-4.0.3/pkgs/aimstack/xgboost_tracker/boards/runs.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-10-04 15:23:30.767237 aim-4.0.3/pkgs/aimstack/xgboost_tracker/callbacks/
+-rw-r--r--   0 github     (503) staff       (20)       74 2023-09-26 20:09:35.000000 aim-4.0.3/pkgs/aimstack/xgboost_tracker/callbacks/__init__.py
+-rw-r--r--   0 github     (503) staff       (20)     3063 2023-09-27 17:12:13.000000 aim-4.0.3/pkgs/aimstack/xgboost_tracker/callbacks/base_callback.py
+-rw-r--r--   0 github     (503) staff       (20)      898 2023-07-12 18:55:32.000000 aim-4.0.3/pyproject.toml
+-rw-r--r--   0 github     (503) staff       (20)       38 2023-10-04 15:23:30.813854 aim-4.0.3/setup.cfg
+-rw-r--r--   0 github     (503) staff       (20)     7017 2023-10-03 16:38:51.000000 aim-4.0.3/setup.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-10-04 15:23:30.719697 aim-4.0.3/src/
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-10-04 15:23:30.767497 aim-4.0.3/src/aimcore/
+-rw-r--r--   0 github     (503) staff       (20)        0 2023-07-12 18:55:32.000000 aim-4.0.3/src/aimcore/__init__.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-10-04 15:23:30.768418 aim-4.0.3/src/aimcore/callbacks/
+-rw-r--r--   0 github     (503) staff       (20)      130 2023-07-12 18:55:32.000000 aim-4.0.3/src/aimcore/callbacks/__init__.py
+-rw-r--r--   0 github     (503) staff       (20)     1599 2023-07-12 18:55:32.000000 aim-4.0.3/src/aimcore/callbacks/caller.py
+-rw-r--r--   0 github     (503) staff       (20)      478 2023-07-12 18:55:32.000000 aim-4.0.3/src/aimcore/callbacks/events.py
+-rw-r--r--   0 github     (503) staff       (20)     1416 2023-07-12 18:55:32.000000 aim-4.0.3/src/aimcore/callbacks/helpers.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-10-04 15:23:30.768634 aim-4.0.3/src/aimcore/cleanup/
+-rw-r--r--   0 github     (503) staff       (20)     3579 2023-07-12 18:55:32.000000 aim-4.0.3/src/aimcore/cleanup/__init__.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-10-04 15:23:30.769508 aim-4.0.3/src/aimcore/cli/
+-rw-r--r--   0 github     (503) staff       (20)        0 2023-07-12 18:55:32.000000 aim-4.0.3/src/aimcore/cli/__init__.py
+-rw-r--r--   0 github     (503) staff       (20)     2041 2023-10-03 20:10:16.000000 aim-4.0.3/src/aimcore/cli/cli.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-10-04 15:23:30.770105 aim-4.0.3/src/aimcore/cli/conatiners/
+-rw-r--r--   0 github     (503) staff       (20)        0 2023-07-19 20:10:38.000000 aim-4.0.3/src/aimcore/cli/conatiners/__init__.py
+-rw-r--r--   0 github     (503) staff       (20)     6934 2023-10-03 20:10:16.000000 aim-4.0.3/src/aimcore/cli/conatiners/commands.py
+-rw-r--r--   0 github     (503) staff       (20)      791 2023-09-08 20:15:11.000000 aim-4.0.3/src/aimcore/cli/conatiners/utils.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-10-04 15:23:30.770588 aim-4.0.3/src/aimcore/cli/convert/
+-rw-r--r--   0 github     (503) staff       (20)        0 2023-07-12 18:55:32.000000 aim-4.0.3/src/aimcore/cli/convert/__init__.py
+-rw-r--r--   0 github     (503) staff       (20)     3004 2023-07-12 18:55:32.000000 aim-4.0.3/src/aimcore/cli/convert/commands.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-10-04 15:23:30.771492 aim-4.0.3/src/aimcore/cli/convert/processors/
+-rw-r--r--   0 github     (503) staff       (20)      113 2023-07-12 18:55:32.000000 aim-4.0.3/src/aimcore/cli/convert/processors/__init__.py
+-rw-r--r--   0 github     (503) staff       (20)     5916 2023-07-12 18:55:32.000000 aim-4.0.3/src/aimcore/cli/convert/processors/mlflow.py
+-rw-r--r--   0 github     (503) staff       (20)    10374 2023-07-12 18:55:32.000000 aim-4.0.3/src/aimcore/cli/convert/processors/tensorboard.py
+-rw-r--r--   0 github     (503) staff       (20)     6820 2023-07-12 18:55:32.000000 aim-4.0.3/src/aimcore/cli/convert/processors/wandb.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-10-04 15:23:30.771743 aim-4.0.3/src/aimcore/cli/init/
+-rw-r--r--   0 github     (503) staff       (20)        0 2023-07-12 18:55:32.000000 aim-4.0.3/src/aimcore/cli/init/__init__.py
+-rw-r--r--   0 github     (503) staff       (20)     1741 2023-10-03 20:10:16.000000 aim-4.0.3/src/aimcore/cli/init/commands.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-10-04 15:23:30.772359 aim-4.0.3/src/aimcore/cli/migrate/
+-rw-r--r--   0 github     (503) staff       (20)        0 2023-07-25 12:19:13.000000 aim-4.0.3/src/aimcore/cli/migrate/__init__.py
+-rw-r--r--   0 github     (503) staff       (20)     2657 2023-10-03 20:10:16.000000 aim-4.0.3/src/aimcore/cli/migrate/commands.py
+-rw-r--r--   0 github     (503) staff       (20)     8167 2023-10-03 16:38:51.000000 aim-4.0.3/src/aimcore/cli/migrate/utils.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-10-04 15:23:30.773063 aim-4.0.3/src/aimcore/cli/package/
+-rw-r--r--   0 github     (503) staff       (20)        0 2023-07-12 18:55:32.000000 aim-4.0.3/src/aimcore/cli/package/__init__.py
+-rw-r--r--   0 github     (503) staff       (20)     7374 2023-10-03 20:10:16.000000 aim-4.0.3/src/aimcore/cli/package/commands.py
+-rw-r--r--   0 github     (503) staff       (20)     1416 2023-09-26 20:09:35.000000 aim-4.0.3/src/aimcore/cli/package/utils.py
+-rw-r--r--   0 github     (503) staff       (20)     4166 2023-08-04 20:11:55.000000 aim-4.0.3/src/aimcore/cli/package/watcher.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-10-04 15:23:30.773543 aim-4.0.3/src/aimcore/cli/server/
+-rw-r--r--   0 github     (503) staff       (20)        0 2023-07-12 18:55:32.000000 aim-4.0.3/src/aimcore/cli/server/__init__.py
+-rw-r--r--   0 github     (503) staff       (20)     4549 2023-10-03 20:10:16.000000 aim-4.0.3/src/aimcore/cli/server/commands.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-10-04 15:23:30.773814 aim-4.0.3/src/aimcore/cli/storage/
+-rw-r--r--   0 github     (503) staff       (20)        0 2023-07-12 18:55:32.000000 aim-4.0.3/src/aimcore/cli/storage/__init__.py
+-rw-r--r--   0 github     (503) staff       (20)     4082 2023-07-12 18:55:32.000000 aim-4.0.3/src/aimcore/cli/storage/commands.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-10-04 15:23:30.774059 aim-4.0.3/src/aimcore/cli/telemetry/
+-rw-r--r--   0 github     (503) staff       (20)        0 2023-07-12 18:55:32.000000 aim-4.0.3/src/aimcore/cli/telemetry/__init__.py
+-rw-r--r--   0 github     (503) staff       (20)      304 2023-07-12 18:55:32.000000 aim-4.0.3/src/aimcore/cli/telemetry/commands.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-10-04 15:23:30.774479 aim-4.0.3/src/aimcore/cli/ui/
+-rw-r--r--   0 github     (503) staff       (20)        0 2023-07-25 12:19:13.000000 aim-4.0.3/src/aimcore/cli/ui/__init__.py
+-rw-r--r--   0 github     (503) staff       (20)     6293 2023-10-03 20:10:16.000000 aim-4.0.3/src/aimcore/cli/ui/commands.py
+-rw-r--r--   0 github     (503) staff       (20)      505 2023-09-19 20:11:49.000000 aim-4.0.3/src/aimcore/cli/ui/utils.py
+-rw-r--r--   0 github     (503) staff       (20)      669 2023-09-19 20:11:49.000000 aim-4.0.3/src/aimcore/cli/utils.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-10-04 15:23:30.774814 aim-4.0.3/src/aimcore/cli/version/
+-rw-r--r--   0 github     (503) staff       (20)        0 2023-07-12 18:55:32.000000 aim-4.0.3/src/aimcore/cli/version/__init__.py
+-rw-r--r--   0 github     (503) staff       (20)      223 2023-10-03 20:10:16.000000 aim-4.0.3/src/aimcore/cli/version/commands.py
+-rw-r--r--   0 github     (503) staff       (20)     9963 2023-07-12 18:55:32.000000 aim-4.0.3/src/aimcore/cli/watcher_cli.py
+-rw-r--r--   0 github     (503) staff       (20)     1254 2023-09-04 20:14:49.000000 aim-4.0.3/src/aimcore/error_handling.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-10-04 15:23:30.774963 aim-4.0.3/src/aimcore/reporter/
+-rw-r--r--   0 github     (503) staff       (20)    31358 2023-09-19 20:11:49.000000 aim-4.0.3/src/aimcore/reporter/__init__.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-10-04 15:23:30.777742 aim-4.0.3/src/aimcore/transport/
+-rw-r--r--   0 github     (503) staff       (20)       27 2023-07-12 18:55:32.000000 aim-4.0.3/src/aimcore/transport/__init__.py
+-rw-r--r--   0 github     (503) staff       (20)    10489 2023-09-04 20:14:49.000000 aim-4.0.3/src/aimcore/transport/client.py
+-rw-r--r--   0 github     (503) staff       (20)      273 2023-07-12 18:55:32.000000 aim-4.0.3/src/aimcore/transport/config.py
+-rw-r--r--   0 github     (503) staff       (20)     2239 2023-08-04 20:11:55.000000 aim-4.0.3/src/aimcore/transport/handlers.py
+-rw-r--r--   0 github     (503) staff       (20)     5403 2023-07-13 20:09:35.000000 aim-4.0.3/src/aimcore/transport/heartbeat.py
+-rw-r--r--   0 github     (503) staff       (20)     3095 2023-07-12 18:55:32.000000 aim-4.0.3/src/aimcore/transport/message_utils.py
+-rw-r--r--   0 github     (503) staff       (20)      445 2023-07-12 18:55:32.000000 aim-4.0.3/src/aimcore/transport/remote_resource.py
+-rw-r--r--   0 github     (503) staff       (20)     1825 2023-07-13 20:09:35.000000 aim-4.0.3/src/aimcore/transport/router.py
+-rw-r--r--   0 github     (503) staff       (20)     3692 2023-07-12 18:55:32.000000 aim-4.0.3/src/aimcore/transport/rpc_queue.py
+-rw-r--r--   0 github     (503) staff       (20)     4846 2023-08-04 20:11:55.000000 aim-4.0.3/src/aimcore/transport/server.py
+-rw-r--r--   0 github     (503) staff       (20)     6358 2023-08-04 20:11:55.000000 aim-4.0.3/src/aimcore/transport/tracking.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-10-04 15:23:30.778570 aim-4.0.3/src/aimcore/web/
+-rw-r--r--   0 github     (503) staff       (20)        0 2023-07-12 18:55:32.000000 aim-4.0.3/src/aimcore/web/__init__.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-10-04 15:23:30.779427 aim-4.0.3/src/aimcore/web/api/
+-rw-r--r--   0 github     (503) staff       (20)     3317 2023-08-04 20:11:55.000000 aim-4.0.3/src/aimcore/web/api/__init__.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-10-04 15:23:30.780074 aim-4.0.3/src/aimcore/web/api/boards/
+-rw-r--r--   0 github     (503) staff       (20)        0 2023-07-12 18:55:32.000000 aim-4.0.3/src/aimcore/web/api/boards/__init__.py
+-rw-r--r--   0 github     (503) staff       (20)     1817 2023-07-12 18:55:32.000000 aim-4.0.3/src/aimcore/web/api/boards/models.py
+-rw-r--r--   0 github     (503) staff       (20)      139 2023-07-12 18:55:32.000000 aim-4.0.3/src/aimcore/web/api/boards/pydantic_models.py
+-rw-r--r--   0 github     (503) staff       (20)     1905 2023-09-19 20:11:49.000000 aim-4.0.3/src/aimcore/web/api/boards/views.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-10-04 15:23:30.780800 aim-4.0.3/src/aimcore/web/api/dashboard_apps/
+-rw-r--r--   0 github     (503) staff       (20)        0 2023-07-12 18:55:32.000000 aim-4.0.3/src/aimcore/web/api/dashboard_apps/__init__.py
+-rw-r--r--   0 github     (503) staff       (20)      920 2023-07-12 18:55:32.000000 aim-4.0.3/src/aimcore/web/api/dashboard_apps/models.py
+-rw-r--r--   0 github     (503) staff       (20)      542 2023-07-12 18:55:32.000000 aim-4.0.3/src/aimcore/web/api/dashboard_apps/pydantic_models.py
+-rw-r--r--   0 github     (503) staff       (20)      449 2023-07-12 18:55:32.000000 aim-4.0.3/src/aimcore/web/api/dashboard_apps/serializers.py
+-rw-r--r--   0 github     (503) staff       (20)     2994 2023-07-12 18:55:32.000000 aim-4.0.3/src/aimcore/web/api/dashboard_apps/views.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-10-04 15:23:30.781519 aim-4.0.3/src/aimcore/web/api/dashboards/
+-rw-r--r--   0 github     (503) staff       (20)        0 2023-07-12 18:55:32.000000 aim-4.0.3/src/aimcore/web/api/dashboards/__init__.py
+-rw-r--r--   0 github     (503) staff       (20)      648 2023-07-12 18:55:32.000000 aim-4.0.3/src/aimcore/web/api/dashboards/models.py
+-rw-r--r--   0 github     (503) staff       (20)      652 2023-07-12 18:55:32.000000 aim-4.0.3/src/aimcore/web/api/dashboards/pydantic_models.py
+-rw-r--r--   0 github     (503) staff       (20)      783 2023-07-12 18:55:32.000000 aim-4.0.3/src/aimcore/web/api/dashboards/serializers.py
+-rw-r--r--   0 github     (503) staff       (20)     3365 2023-07-12 18:55:32.000000 aim-4.0.3/src/aimcore/web/api/dashboards/views.py
+-rw-r--r--   0 github     (503) staff       (20)      807 2023-07-12 18:55:32.000000 aim-4.0.3/src/aimcore/web/api/db.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-10-04 15:23:30.782211 aim-4.0.3/src/aimcore/web/api/projects/
+-rw-r--r--   0 github     (503) staff       (20)        0 2023-07-12 18:55:32.000000 aim-4.0.3/src/aimcore/web/api/projects/__init__.py
+-rw-r--r--   0 github     (503) staff       (20)      628 2023-07-12 18:55:32.000000 aim-4.0.3/src/aimcore/web/api/projects/project.py
+-rw-r--r--   0 github     (503) staff       (20)     1247 2023-09-27 15:10:23.000000 aim-4.0.3/src/aimcore/web/api/projects/pydantic_models.py
+-rw-r--r--   0 github     (503) staff       (20)     3489 2023-09-27 15:10:23.000000 aim-4.0.3/src/aimcore/web/api/projects/views.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-10-04 15:23:30.782525 aim-4.0.3/src/aimcore/web/api/queries/
+-rw-r--r--   0 github     (503) staff       (20)        0 2023-07-12 18:55:32.000000 aim-4.0.3/src/aimcore/web/api/queries/__init__.py
+-rw-r--r--   0 github     (503) staff       (20)     8582 2023-09-27 15:10:23.000000 aim-4.0.3/src/aimcore/web/api/queries/views.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-10-04 15:23:30.783268 aim-4.0.3/src/aimcore/web/api/reports/
+-rw-r--r--   0 github     (503) staff       (20)        0 2023-07-12 18:55:32.000000 aim-4.0.3/src/aimcore/web/api/reports/__init__.py
+-rw-r--r--   0 github     (503) staff       (20)      615 2023-07-12 18:55:32.000000 aim-4.0.3/src/aimcore/web/api/reports/models.py
+-rw-r--r--   0 github     (503) staff       (20)      683 2023-07-12 18:55:32.000000 aim-4.0.3/src/aimcore/web/api/reports/pydantic_models.py
+-rw-r--r--   0 github     (503) staff       (20)      461 2023-07-12 18:55:32.000000 aim-4.0.3/src/aimcore/web/api/reports/serializers.py
+-rw-r--r--   0 github     (503) staff       (20)     2449 2023-09-08 20:15:11.000000 aim-4.0.3/src/aimcore/web/api/reports/views.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-10-04 15:23:30.784091 aim-4.0.3/src/aimcore/web/api/runs/
+-rw-r--r--   0 github     (503) staff       (20)        0 2023-07-12 18:55:32.000000 aim-4.0.3/src/aimcore/web/api/runs/__init__.py
+-rw-r--r--   0 github     (503) staff       (20)     4488 2023-07-12 18:55:32.000000 aim-4.0.3/src/aimcore/web/api/runs/pydantic_models.py
+-rw-r--r--   0 github     (503) staff       (20)    14447 2023-09-08 20:15:11.000000 aim-4.0.3/src/aimcore/web/api/runs/utils.py
+-rw-r--r--   0 github     (503) staff       (20)    13193 2023-07-12 18:55:32.000000 aim-4.0.3/src/aimcore/web/api/runs/views.py
+-rw-r--r--   0 github     (503) staff       (20)     2906 2023-09-19 20:11:49.000000 aim-4.0.3/src/aimcore/web/api/utils.py
+-rw-r--r--   0 github     (503) staff       (20)     1597 2023-07-12 18:55:32.000000 aim-4.0.3/src/aimcore/web/api/views.py
+-rw-r--r--   0 github     (503) staff       (20)      384 2023-08-04 20:11:55.000000 aim-4.0.3/src/aimcore/web/configs.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-10-04 15:23:30.784359 aim-4.0.3/src/aimcore/web/middlewares/
+-rw-r--r--   0 github     (503) staff       (20)        0 2023-07-12 18:55:32.000000 aim-4.0.3/src/aimcore/web/middlewares/__init__.py
+-rw-r--r--   0 github     (503) staff       (20)     3654 2023-07-12 18:55:32.000000 aim-4.0.3/src/aimcore/web/middlewares/profiler.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-10-04 15:23:30.785235 aim-4.0.3/src/aimcore/web/migrations/
+-rw-r--r--   0 github     (503) staff       (20)       38 2023-07-12 18:55:32.000000 aim-4.0.3/src/aimcore/web/migrations/README
+-rw-r--r--   0 github     (503) staff       (20)      800 2023-07-12 18:55:32.000000 aim-4.0.3/src/aimcore/web/migrations/alembic.ini
+-rw-r--r--   0 github     (503) staff       (20)      797 2023-07-12 18:55:32.000000 aim-4.0.3/src/aimcore/web/migrations/alembic_dev.ini
+-rw-r--r--   0 github     (503) staff       (20)     2717 2023-07-12 18:55:32.000000 aim-4.0.3/src/aimcore/web/migrations/env.py
+-rw-r--r--   0 github     (503) staff       (20)      494 2023-07-12 18:55:32.000000 aim-4.0.3/src/aimcore/web/migrations/script.py.mako
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-10-04 15:23:30.786528 aim-4.0.3/src/aimcore/web/migrations/versions/
+-rw-r--r--   0 github     (503) staff       (20)     2183 2023-07-12 18:55:32.000000 aim-4.0.3/src/aimcore/web/migrations/versions/11672b13f92c_.py
+-rw-r--r--   0 github     (503) staff       (20)     1545 2023-07-12 18:55:32.000000 aim-4.0.3/src/aimcore/web/migrations/versions/517a45b2e62c_.py
+-rw-r--r--   0 github     (503) staff       (20)     5592 2023-07-12 18:55:32.000000 aim-4.0.3/src/aimcore/web/migrations/versions/5ae8371b7481_.py
+-rw-r--r--   0 github     (503) staff       (20)     7262 2023-07-12 18:55:32.000000 aim-4.0.3/src/aimcore/web/migrations/versions/73a3d004c227_.py
+-rw-r--r--   0 github     (503) staff       (20)     1788 2023-07-12 18:55:32.000000 aim-4.0.3/src/aimcore/web/migrations/versions/da08eab59790_board_and_board_templates.py
+-rw-r--r--   0 github     (503) staff       (20)      959 2023-07-12 18:55:32.000000 aim-4.0.3/src/aimcore/web/migrations/versions/df1fff471cab_.py
+-rw-r--r--   0 github     (503) staff       (20)       59 2023-07-12 18:55:32.000000 aim-4.0.3/src/aimcore/web/run.py
+-rw-r--r--   0 github     (503) staff       (20)     3674 2023-09-19 20:11:49.000000 aim-4.0.3/src/aimcore/web/utils.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-10-04 15:23:30.719737 aim-4.0.3/src/python/
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-10-04 15:23:30.788572 aim-4.0.3/src/python/aim/
+-rw-r--r--   0 github     (503) staff       (20)        6 2023-10-04 15:23:21.000000 aim-4.0.3/src/python/aim/VERSION
+-rw-r--r--   0 github     (503) staff       (20)      825 2023-07-12 18:55:32.000000 aim-4.0.3/src/python/aim/__about__.py
+-rw-r--r--   0 github     (503) staff       (20)      631 2023-09-05 20:15:25.000000 aim-4.0.3/src/python/aim/__init__.py
+-rw-r--r--   0 github     (503) staff       (20)      183 2023-07-12 18:55:32.000000 aim-4.0.3/src/python/aim/__version__.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-10-04 15:23:30.788751 aim-4.0.3/src/python/aim/_core/
+-rw-r--r--   0 github     (503) staff       (20)        0 2023-07-12 18:55:32.000000 aim-4.0.3/src/python/aim/_core/__init__.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-10-04 15:23:30.799610 aim-4.0.3/src/python/aim/_core/storage/
+-rw-r--r--   0 github     (503) staff       (20)        0 2023-07-12 18:55:32.000000 aim-4.0.3/src/python/aim/_core/storage/__init__.py
+-rw-r--r--   0 github     (503) staff       (20)   459259 2023-10-04 15:23:27.000000 aim-4.0.3/src/python/aim/_core/storage/arrayview.cpp
+-rw-r--r--   0 github     (503) staff       (20)      278 2023-07-12 18:55:32.000000 aim-4.0.3/src/python/aim/_core/storage/arrayview.pxd
+-rw-r--r--   0 github     (503) staff       (20)     3051 2023-07-12 18:55:32.000000 aim-4.0.3/src/python/aim/_core/storage/arrayview.py
+-rw-r--r--   0 github     (503) staff       (20)   935063 2023-10-04 15:23:27.000000 aim-4.0.3/src/python/aim/_core/storage/container.cpp
+-rw-r--r--   0 github     (503) staff       (20)      977 2023-07-12 18:55:32.000000 aim-4.0.3/src/python/aim/_core/storage/container.pxd
+-rw-r--r--   0 github     (503) staff       (20)    12336 2023-07-12 18:55:32.000000 aim-4.0.3/src/python/aim/_core/storage/container.py
+-rw-r--r--   0 github     (503) staff       (20)   968088 2023-10-04 15:23:28.000000 aim-4.0.3/src/python/aim/_core/storage/containertreeview.cpp
+-rw-r--r--   0 github     (503) staff       (20)      337 2023-07-12 18:55:32.000000 aim-4.0.3/src/python/aim/_core/storage/containertreeview.pxd
+-rw-r--r--   0 github     (503) staff       (20)     7258 2023-07-12 18:55:32.000000 aim-4.0.3/src/python/aim/_core/storage/containertreeview.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-10-04 15:23:30.801319 aim-4.0.3/src/python/aim/_core/storage/encoding/
+-rw-r--r--   0 github     (503) staff       (20)   149167 2023-10-04 15:23:28.000000 aim-4.0.3/src/python/aim/_core/storage/encoding/__init__.cpp
+-rw-r--r--   0 github     (503) staff       (20)      167 2023-07-12 18:55:32.000000 aim-4.0.3/src/python/aim/_core/storage/encoding/__init__.pxd
+-rw-r--r--   0 github     (503) staff       (20)      107 2023-07-12 18:55:32.000000 aim-4.0.3/src/python/aim/_core/storage/encoding/__init__.py
+-rw-r--r--   0 github     (503) staff       (20)   380498 2023-10-04 15:23:28.000000 aim-4.0.3/src/python/aim/_core/storage/encoding/encoding.cpp
+-rw-r--r--   0 github     (503) staff       (20)      507 2023-07-12 18:55:32.000000 aim-4.0.3/src/python/aim/_core/storage/encoding/encoding.pxd
+-rw-r--r--   0 github     (503) staff       (20)     7427 2023-07-12 18:55:32.000000 aim-4.0.3/src/python/aim/_core/storage/encoding/encoding.pyx
+-rw-r--r--   0 github     (503) staff       (20)   356452 2023-10-04 15:23:28.000000 aim-4.0.3/src/python/aim/_core/storage/encoding/encoding_native.cpp
+-rw-r--r--   0 github     (503) staff       (20)      930 2023-07-12 18:55:32.000000 aim-4.0.3/src/python/aim/_core/storage/encoding/encoding_native.pxd
+-rw-r--r--   0 github     (503) staff       (20)     5980 2023-07-12 18:55:32.000000 aim-4.0.3/src/python/aim/_core/storage/encoding/encoding_native.pyx
+-rw-r--r--   0 github     (503) staff       (20)      337 2023-07-12 18:55:32.000000 aim-4.0.3/src/python/aim/_core/storage/env.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-10-04 15:23:30.802647 aim-4.0.3/src/python/aim/_core/storage/hashing/
+-rw-r--r--   0 github     (503) staff       (20)   142042 2023-10-04 15:23:28.000000 aim-4.0.3/src/python/aim/_core/storage/hashing/__init__.cpp
+-rw-r--r--   0 github     (503) staff       (20)       97 2023-07-12 18:55:32.000000 aim-4.0.3/src/python/aim/_core/storage/hashing/__init__.pxd
+-rw-r--r--   0 github     (503) staff       (20)       56 2023-07-12 18:55:32.000000 aim-4.0.3/src/python/aim/_core/storage/hashing/__init__.py
+-rw-r--r--   0 github     (503) staff       (20)   206140 2023-10-04 15:23:28.000000 aim-4.0.3/src/python/aim/_core/storage/hashing/c_hash.cpp
+-rw-r--r--   0 github     (503) staff       (20)      151 2023-07-12 18:55:32.000000 aim-4.0.3/src/python/aim/_core/storage/hashing/c_hash.pxd
+-rw-r--r--   0 github     (503) staff       (20)     1083 2023-07-12 18:55:32.000000 aim-4.0.3/src/python/aim/_core/storage/hashing/c_hash.pyx
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-10-04 15:23:30.802754 aim-4.0.3/src/python/aim/_core/storage/hashing/hash/
+-rw-r--r--   0 github     (503) staff       (20)     1412 2023-07-12 18:55:32.000000 aim-4.0.3/src/python/aim/_core/storage/hashing/hash/hash.h
+-rw-r--r--   0 github     (503) staff       (20)   394398 2023-10-04 15:23:28.000000 aim-4.0.3/src/python/aim/_core/storage/hashing/hashing.cpp
+-rw-r--r--   0 github     (503) staff       (20)     1021 2023-07-12 18:55:32.000000 aim-4.0.3/src/python/aim/_core/storage/hashing/hashing.pxd
+-rw-r--r--   0 github     (503) staff       (20)     5580 2023-07-12 18:55:32.000000 aim-4.0.3/src/python/aim/_core/storage/hashing/hashing.py
+-rw-r--r--   0 github     (503) staff       (20)   679035 2023-10-04 15:23:28.000000 aim-4.0.3/src/python/aim/_core/storage/inmemorytreeview.cpp
+-rw-r--r--   0 github     (503) staff       (20)      202 2023-07-12 18:55:32.000000 aim-4.0.3/src/python/aim/_core/storage/inmemorytreeview.pxd
+-rw-r--r--   0 github     (503) staff       (20)     4365 2023-07-12 18:55:32.000000 aim-4.0.3/src/python/aim/_core/storage/inmemorytreeview.py
+-rw-r--r--   0 github     (503) staff       (20)     7858 2023-07-12 18:55:32.000000 aim-4.0.3/src/python/aim/_core/storage/locking.py
+-rw-r--r--   0 github     (503) staff       (20)     2125 2023-09-14 20:15:29.000000 aim-4.0.3/src/python/aim/_core/storage/object.py
+-rw-r--r--   0 github     (503) staff       (20)   979988 2023-10-04 15:23:29.000000 aim-4.0.3/src/python/aim/_core/storage/prefixview.cpp
+-rw-r--r--   0 github     (503) staff       (20)      808 2023-07-12 18:55:32.000000 aim-4.0.3/src/python/aim/_core/storage/prefixview.pxd
+-rw-r--r--   0 github     (503) staff       (20)    12274 2023-07-12 18:55:32.000000 aim-4.0.3/src/python/aim/_core/storage/prefixview.py
+-rw-r--r--   0 github     (503) staff       (20)    11648 2023-07-12 18:55:32.000000 aim-4.0.3/src/python/aim/_core/storage/proxy.py
+-rw-r--r--   0 github     (503) staff       (20)   996914 2023-10-04 15:23:29.000000 aim-4.0.3/src/python/aim/_core/storage/rockscontainer.cpp
+-rw-r--r--   0 github     (503) staff       (20)    18696 2023-09-04 20:14:49.000000 aim-4.0.3/src/python/aim/_core/storage/rockscontainer.pyx
+-rw-r--r--   0 github     (503) staff       (20)   706262 2023-10-04 15:23:29.000000 aim-4.0.3/src/python/aim/_core/storage/treearrayview.cpp
+-rw-r--r--   0 github     (503) staff       (20)      263 2023-07-12 18:55:32.000000 aim-4.0.3/src/python/aim/_core/storage/treearrayview.pxd
+-rw-r--r--   0 github     (503) staff       (20)     3044 2023-07-12 18:55:32.000000 aim-4.0.3/src/python/aim/_core/storage/treearrayview.py
+-rw-r--r--   0 github     (503) staff       (20)   728377 2023-10-04 15:23:29.000000 aim-4.0.3/src/python/aim/_core/storage/treeutils.cpp
+-rw-r--r--   0 github     (503) staff       (20)     8419 2023-07-12 18:55:32.000000 aim-4.0.3/src/python/aim/_core/storage/treeutils.pyx
+-rw-r--r--   0 github     (503) staff       (20)      713 2023-07-12 18:55:32.000000 aim-4.0.3/src/python/aim/_core/storage/treeutils_non_native.py
+-rw-r--r--   0 github     (503) staff       (20)   538818 2023-10-04 15:23:29.000000 aim-4.0.3/src/python/aim/_core/storage/treeview.cpp
+-rw-r--r--   0 github     (503) staff       (20)      311 2023-07-12 18:55:32.000000 aim-4.0.3/src/python/aim/_core/storage/treeview.pxd
+-rw-r--r--   0 github     (503) staff       (20)     3065 2023-07-12 18:55:32.000000 aim-4.0.3/src/python/aim/_core/storage/treeview.py
+-rw-r--r--   0 github     (503) staff       (20)     1363 2023-07-12 18:55:32.000000 aim-4.0.3/src/python/aim/_core/storage/types.py
+-rw-r--r--   0 github     (503) staff       (20)   813912 2023-10-04 15:23:29.000000 aim-4.0.3/src/python/aim/_core/storage/union.cpp
+-rw-r--r--   0 github     (503) staff       (20)     7865 2023-09-04 20:14:49.000000 aim-4.0.3/src/python/aim/_core/storage/union.pyx
+-rw-r--r--   0 github     (503) staff       (20)   817782 2023-10-04 15:23:30.000000 aim-4.0.3/src/python/aim/_core/storage/utils.cpp
+-rw-r--r--   0 github     (503) staff       (20)      469 2023-07-12 18:55:32.000000 aim-4.0.3/src/python/aim/_core/storage/utils.pxd
+-rw-r--r--   0 github     (503) staff       (20)     2102 2023-07-12 18:55:32.000000 aim-4.0.3/src/python/aim/_core/storage/utils.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-10-04 15:23:30.803014 aim-4.0.3/src/python/aim/_core/utils/
+-rw-r--r--   0 github     (503) staff       (20)        0 2023-09-04 20:14:49.000000 aim-4.0.3/src/python/aim/_core/utils/__init__.py
+-rw-r--r--   0 github     (503) staff       (20)      722 2023-07-12 18:55:32.000000 aim-4.0.3/src/python/aim/_core/utils/deprecation.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-10-04 15:23:30.803190 aim-4.0.3/src/python/aim/_ext/
+-rw-r--r--   0 github     (503) staff       (20)        0 2023-07-12 18:55:32.000000 aim-4.0.3/src/python/aim/_ext/__init__.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-10-04 15:23:30.803607 aim-4.0.3/src/python/aim/_ext/notebook/
+-rw-r--r--   0 github     (503) staff       (20)        0 2023-07-12 18:55:32.000000 aim-4.0.3/src/python/aim/_ext/notebook/__init__.py
+-rw-r--r--   0 github     (503) staff       (20)     2615 2023-07-25 12:19:13.000000 aim-4.0.3/src/python/aim/_ext/notebook/manager.py
+-rw-r--r--   0 github     (503) staff       (20)     7169 2023-07-25 12:19:13.000000 aim-4.0.3/src/python/aim/_ext/notebook/notebook.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-10-04 15:23:30.805291 aim-4.0.3/src/python/aim/_ext/notifier/
+-rw-r--r--   0 github     (503) staff       (20)      593 2023-07-12 18:55:32.000000 aim-4.0.3/src/python/aim/_ext/notifier/__init__.py
+-rw-r--r--   0 github     (503) staff       (20)      305 2023-07-12 18:55:32.000000 aim-4.0.3/src/python/aim/_ext/notifier/base_notifier.py
+-rw-r--r--   0 github     (503) staff       (20)     1859 2023-07-12 18:55:32.000000 aim-4.0.3/src/python/aim/_ext/notifier/config.py
+-rw-r--r--   0 github     (503) staff       (20)      523 2023-07-12 18:55:32.000000 aim-4.0.3/src/python/aim/_ext/notifier/logging_notifier.py
+-rw-r--r--   0 github     (503) staff       (20)     1429 2023-07-12 18:55:32.000000 aim-4.0.3/src/python/aim/_ext/notifier/notifier.py
+-rw-r--r--   0 github     (503) staff       (20)     1162 2023-07-12 18:55:32.000000 aim-4.0.3/src/python/aim/_ext/notifier/notifier_builder.py
+-rw-r--r--   0 github     (503) staff       (20)      525 2023-07-12 18:55:32.000000 aim-4.0.3/src/python/aim/_ext/notifier/slack_notifier.py
+-rw-r--r--   0 github     (503) staff       (20)     1035 2023-07-12 18:55:32.000000 aim-4.0.3/src/python/aim/_ext/notifier/utils.py
+-rw-r--r--   0 github     (503) staff       (20)      863 2023-07-12 18:55:32.000000 aim-4.0.3/src/python/aim/_ext/notifier/workplace_notifier.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-10-04 15:23:30.807006 aim-4.0.3/src/python/aim/_ext/system_info/
+-rw-r--r--   0 github     (503) staff       (20)      152 2023-07-12 18:55:32.000000 aim-4.0.3/src/python/aim/_ext/system_info/__init__.py
+-rw-r--r--   0 github     (503) staff       (20)      100 2023-07-12 18:55:32.000000 aim-4.0.3/src/python/aim/_ext/system_info/configs.py
+-rw-r--r--   0 github     (503) staff       (20)   148706 2023-07-12 18:55:32.000000 aim-4.0.3/src/python/aim/_ext/system_info/pynvml.py
+-rw-r--r--   0 github     (503) staff       (20)     7798 2023-07-12 18:55:32.000000 aim-4.0.3/src/python/aim/_ext/system_info/resource_tracker.py
+-rw-r--r--   0 github     (503) staff       (20)     6670 2023-09-19 20:11:49.000000 aim-4.0.3/src/python/aim/_ext/system_info/stat.py
+-rw-r--r--   0 github     (503) staff       (20)     2246 2023-07-25 12:19:13.000000 aim-4.0.3/src/python/aim/_ext/system_info/utils.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-10-04 15:23:30.807190 aim-4.0.3/src/python/aim/_ext/tracking/
+-rw-r--r--   0 github     (503) staff       (20)     4755 2023-07-12 18:55:32.000000 aim-4.0.3/src/python/aim/_ext/tracking/__init__.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-10-04 15:23:30.812644 aim-4.0.3/src/python/aim/_sdk/
+-rw-r--r--   0 github     (503) staff       (20)        0 2023-07-12 18:55:32.000000 aim-4.0.3/src/python/aim/_sdk/__init__.py
+-rw-r--r--   0 github     (503) staff       (20)      856 2023-09-14 20:15:29.000000 aim-4.0.3/src/python/aim/_sdk/action.py
+-rw-r--r--   0 github     (503) staff       (20)       48 2023-07-12 18:55:32.000000 aim-4.0.3/src/python/aim/_sdk/blob.py
+-rw-r--r--   0 github     (503) staff       (20)    10993 2023-08-04 20:11:55.000000 aim-4.0.3/src/python/aim/_sdk/collections.py
+-rw-r--r--   0 github     (503) staff       (20)      363 2023-07-25 12:19:13.000000 aim-4.0.3/src/python/aim/_sdk/configs.py
+-rw-r--r--   0 github     (503) staff       (20)      519 2023-07-12 18:55:32.000000 aim-4.0.3/src/python/aim/_sdk/constants.py
+-rw-r--r--   0 github     (503) staff       (20)    20712 2023-10-03 20:10:16.000000 aim-4.0.3/src/python/aim/_sdk/container.py
+-rw-r--r--   0 github     (503) staff       (20)     1837 2023-07-12 18:55:32.000000 aim-4.0.3/src/python/aim/_sdk/context.py
+-rw-r--r--   0 github     (503) staff       (20)     1233 2023-08-04 20:11:55.000000 aim-4.0.3/src/python/aim/_sdk/dev_package.py
+-rw-r--r--   0 github     (503) staff       (20)      561 2023-07-12 18:55:32.000000 aim-4.0.3/src/python/aim/_sdk/exceptions.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-10-04 15:23:30.813166 aim-4.0.3/src/python/aim/_sdk/interfaces/
+-rw-r--r--   0 github     (503) staff       (20)        0 2023-07-12 18:55:32.000000 aim-4.0.3/src/python/aim/_sdk/interfaces/__init__.py
+-rw-r--r--   0 github     (503) staff       (20)     1563 2023-09-19 20:11:49.000000 aim-4.0.3/src/python/aim/_sdk/interfaces/container.py
+-rw-r--r--   0 github     (503) staff       (20)     2300 2023-07-25 12:19:13.000000 aim-4.0.3/src/python/aim/_sdk/interfaces/sequence.py
+-rw-r--r--   0 github     (503) staff       (20)     3160 2023-07-19 20:10:38.000000 aim-4.0.3/src/python/aim/_sdk/local_storage.py
+-rw-r--r--   0 github     (503) staff       (20)     5506 2023-10-03 16:38:51.000000 aim-4.0.3/src/python/aim/_sdk/lock_manager.py
+-rw-r--r--   0 github     (503) staff       (20)     3397 2023-07-12 18:55:32.000000 aim-4.0.3/src/python/aim/_sdk/num_utils.py
+-rw-r--r--   0 github     (503) staff       (20)     4349 2023-09-27 15:10:23.000000 aim-4.0.3/src/python/aim/_sdk/package_utils.py
+-rw-r--r--   0 github     (503) staff       (20)     4221 2023-07-12 18:55:32.000000 aim-4.0.3/src/python/aim/_sdk/query.py
+-rw-r--r--   0 github     (503) staff       (20)     3046 2023-07-12 18:55:32.000000 aim-4.0.3/src/python/aim/_sdk/query_utils.py
+-rw-r--r--   0 github     (503) staff       (20)     2048 2023-09-19 20:11:49.000000 aim-4.0.3/src/python/aim/_sdk/record.py
+-rw-r--r--   0 github     (503) staff       (20)    18237 2023-09-19 20:11:49.000000 aim-4.0.3/src/python/aim/_sdk/remote_storage.py
+-rw-r--r--   0 github     (503) staff       (20)    26503 2023-10-03 20:10:16.000000 aim-4.0.3/src/python/aim/_sdk/repo.py
+-rw-r--r--   0 github     (503) staff       (20)    18368 2023-10-03 20:10:16.000000 aim-4.0.3/src/python/aim/_sdk/sequence.py
+-rw-r--r--   0 github     (503) staff       (20)      921 2023-07-12 18:55:32.000000 aim-4.0.3/src/python/aim/_sdk/storage_engine.py
+-rw-r--r--   0 github     (503) staff       (20)     4112 2023-09-19 20:11:49.000000 aim-4.0.3/src/python/aim/_sdk/type_utils.py
+-rw-r--r--   0 github     (503) staff       (20)      165 2023-07-12 18:55:32.000000 aim-4.0.3/src/python/aim/_sdk/types.py
+-rw-r--r--   0 github     (503) staff       (20)     1479 2023-07-12 18:55:32.000000 aim-4.0.3/src/python/aim/_sdk/uri_service.py
+-rw-r--r--   0 github     (503) staff       (20)     3723 2023-10-03 16:38:51.000000 aim-4.0.3/src/python/aim/_sdk/utils.py
+-rw-r--r--   0 github     (503) staff       (20)       64 2023-09-05 20:15:25.000000 aim-4.0.3/src/python/aim/container.py
+-rw-r--r--   0 github     (503) staff       (20)       48 2023-07-25 12:19:13.000000 aim-4.0.3/src/python/aim/record.py
+-rw-r--r--   0 github     (503) staff       (20)       44 2023-07-12 18:55:32.000000 aim-4.0.3/src/python/aim/repo.py
+-rw-r--r--   0 github     (503) staff       (20)       52 2023-07-12 18:55:32.000000 aim-4.0.3/src/python/aim/sequence.py
+-rw-r--r--   0 github     (503) staff       (20)     5066 2023-09-08 20:15:11.000000 aim-4.0.3/src/python/aim/utils.py
```

### Comparing `aim-4.0.2/LICENSE` & `aim-4.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `aim-4.0.2/aim.egg-info/SOURCES.txt` & `aim-4.0.3/aim.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -78,15 +78,31 @@
 pkgs/aimstack/docs/boards/ui/text/header.py
 pkgs/aimstack/docs/boards/ui/text/html.py
 pkgs/aimstack/docs/boards/ui/text/link.py
 pkgs/aimstack/docs/boards/ui/text/markdown.py
 pkgs/aimstack/docs/boards/ui/text/subheader.py
 pkgs/aimstack/docs/boards/ui/text/text.py
 pkgs/aimstack/experiment_tracker/__init__.py
+pkgs/aimstack/experiment_tracker/acme.py
+pkgs/aimstack/experiment_tracker/catboost.py
+pkgs/aimstack/experiment_tracker/fastai.py
+pkgs/aimstack/experiment_tracker/hugging_face.py
+pkgs/aimstack/experiment_tracker/keras.py
+pkgs/aimstack/experiment_tracker/keras_tuner.py
+pkgs/aimstack/experiment_tracker/lightgbm.py
+pkgs/aimstack/experiment_tracker/mxnet.py
+pkgs/aimstack/experiment_tracker/optuna.py
+pkgs/aimstack/experiment_tracker/paddle.py
+pkgs/aimstack/experiment_tracker/prophet.py
+pkgs/aimstack/experiment_tracker/pytorch_ignite.py
+pkgs/aimstack/experiment_tracker/pytorch_lightning.py
+pkgs/aimstack/experiment_tracker/sb3.py
+pkgs/aimstack/experiment_tracker/tensorflow.py
 pkgs/aimstack/experiment_tracker/training_flow.py
+pkgs/aimstack/experiment_tracker/xgboost.py
 pkgs/aimstack/experiment_tracker/boards/run.py
 pkgs/aimstack/experiment_tracker/boards/runs.py
 pkgs/aimstack/experiment_tracker/types/__init__.py
 pkgs/aimstack/experiment_tracker/types/deeplake_dataset.py
 pkgs/aimstack/experiment_tracker/types/dvc_metadata.py
 pkgs/aimstack/experiment_tracker/types/hf_datasets_metadata.py
 pkgs/aimstack/experiment_tracker/types/training_run.py
```

### Comparing `aim-4.0.2/pkgs/aimstack/acme_tracker/callbacks/base_callback.py` & `aim-4.0.3/pkgs/aimstack/acme_tracker/callbacks/base_callback.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.2/pkgs/aimstack/base/__init__.py` & `aim-4.0.3/pkgs/aimstack/base/__init__.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.2/pkgs/aimstack/base/actions.py` & `aim-4.0.3/pkgs/aimstack/base/actions.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.2/pkgs/aimstack/base/boards/audios.py` & `aim-4.0.3/pkgs/aimstack/base/boards/audios.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.2/pkgs/aimstack/base/boards/figures.py` & `aim-4.0.3/pkgs/aimstack/base/boards/figures.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.2/pkgs/aimstack/base/boards/images.py` & `aim-4.0.3/pkgs/aimstack/base/boards/images.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.2/pkgs/aimstack/base/boards/logs_overview.py` & `aim-4.0.3/pkgs/aimstack/base/boards/logs_overview.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.2/pkgs/aimstack/base/boards/metrics.py` & `aim-4.0.3/pkgs/aimstack/base/boards/metrics.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.2/pkgs/aimstack/base/boards/run.py` & `aim-4.0.3/pkgs/aimstack/base/boards/run.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.2/pkgs/aimstack/base/boards/runs.py` & `aim-4.0.3/pkgs/aimstack/base/boards/runs.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.2/pkgs/aimstack/base/boards/texts.py` & `aim-4.0.3/pkgs/aimstack/base/boards/texts.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.2/pkgs/aimstack/base/types/audio.py` & `aim-4.0.3/pkgs/aimstack/base/types/audio.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.2/pkgs/aimstack/base/types/distribution.py` & `aim-4.0.3/pkgs/aimstack/base/types/distribution.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.2/pkgs/aimstack/base/types/figures.py` & `aim-4.0.3/pkgs/aimstack/base/types/figures.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.2/pkgs/aimstack/base/types/image.py` & `aim-4.0.3/pkgs/aimstack/base/types/image.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.2/pkgs/aimstack/base/types/io/wavfile.py` & `aim-4.0.3/pkgs/aimstack/base/types/io/wavfile.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.2/pkgs/aimstack/base/types/logging/__init__.py` & `aim-4.0.3/pkgs/aimstack/base/types/logging/__init__.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.2/pkgs/aimstack/base/types/metric.py` & `aim-4.0.3/pkgs/aimstack/base/types/metric.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.2/pkgs/aimstack/base/types/run.py` & `aim-4.0.3/pkgs/aimstack/base/types/run.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.2/pkgs/aimstack/base/types/text.py` & `aim-4.0.3/pkgs/aimstack/base/types/text.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.2/pkgs/aimstack/catboost_tracker/loggers/base_logger.py` & `aim-4.0.3/pkgs/aimstack/catboost_tracker/loggers/base_logger.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.2/pkgs/aimstack/docs/boards/sdk/aim_types.py` & `aim-4.0.3/pkgs/aimstack/docs/boards/sdk/aim_types.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.2/pkgs/aimstack/docs/boards/sdk/container.py` & `aim-4.0.3/pkgs/aimstack/docs/boards/sdk/container.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.2/pkgs/aimstack/docs/boards/sdk/overview.py` & `aim-4.0.3/pkgs/aimstack/docs/boards/sdk/overview.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.2/pkgs/aimstack/docs/boards/sdk/sequence.py` & `aim-4.0.3/pkgs/aimstack/docs/boards/sdk/sequence.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.2/pkgs/aimstack/docs/boards/ui/board/board.py` & `aim-4.0.3/pkgs/aimstack/docs/boards/ui/board/board.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.2/pkgs/aimstack/docs/boards/ui/board/board_link.py` & `aim-4.0.3/pkgs/aimstack/docs/boards/ui/board/board_link.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.2/pkgs/aimstack/docs/boards/ui/charts/line_chart.py` & `aim-4.0.3/pkgs/aimstack/docs/boards/ui/charts/line_chart.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.2/pkgs/aimstack/docs/boards/ui/charts/plotly.py` & `aim-4.0.3/pkgs/aimstack/docs/boards/ui/charts/plotly.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.2/pkgs/aimstack/docs/boards/ui/data_viz/dataframe.py` & `aim-4.0.3/pkgs/aimstack/docs/boards/ui/data_viz/dataframe.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.2/pkgs/aimstack/docs/boards/ui/data_viz/json.py` & `aim-4.0.3/pkgs/aimstack/docs/boards/ui/data_viz/json.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.2/pkgs/aimstack/docs/boards/ui/data_viz/table.py` & `aim-4.0.3/pkgs/aimstack/docs/boards/ui/data_viz/table.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.2/pkgs/aimstack/docs/boards/ui/examples/charts.py` & `aim-4.0.3/pkgs/aimstack/docs/boards/ui/examples/charts.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.2/pkgs/aimstack/docs/boards/ui/examples/data_display_elements.py` & `aim-4.0.3/pkgs/aimstack/docs/boards/ui/examples/data_display_elements.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.2/pkgs/aimstack/docs/boards/ui/examples/input_components.py` & `aim-4.0.3/pkgs/aimstack/docs/boards/ui/examples/input_components.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.2/pkgs/aimstack/docs/boards/ui/input/checkbox.py` & `aim-4.0.3/pkgs/aimstack/docs/boards/ui/input/checkbox.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.2/pkgs/aimstack/docs/boards/ui/input/multi_select.py` & `aim-4.0.3/pkgs/aimstack/docs/boards/ui/input/multi_select.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.2/pkgs/aimstack/docs/boards/ui/input/number_input.py` & `aim-4.0.3/pkgs/aimstack/docs/boards/ui/input/number_input.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.2/pkgs/aimstack/docs/boards/ui/input/radio.py` & `aim-4.0.3/pkgs/aimstack/docs/boards/ui/input/radio.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.2/pkgs/aimstack/docs/boards/ui/input/range_slider.py` & `aim-4.0.3/pkgs/aimstack/docs/boards/ui/input/range_slider.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.2/pkgs/aimstack/docs/boards/ui/input/select.py` & `aim-4.0.3/pkgs/aimstack/docs/boards/ui/input/select.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.2/pkgs/aimstack/docs/boards/ui/input/slider.py` & `aim-4.0.3/pkgs/aimstack/docs/boards/ui/input/slider.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.2/pkgs/aimstack/docs/boards/ui/input/switch.py` & `aim-4.0.3/pkgs/aimstack/docs/boards/ui/input/switch.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.2/pkgs/aimstack/docs/boards/ui/input/text_area.py` & `aim-4.0.3/pkgs/aimstack/docs/boards/ui/input/text_area.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.2/pkgs/aimstack/docs/boards/ui/input/text_input.py` & `aim-4.0.3/pkgs/aimstack/docs/boards/ui/input/text_input.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.2/pkgs/aimstack/docs/boards/ui/input/toggle_button.py` & `aim-4.0.3/pkgs/aimstack/docs/boards/ui/input/toggle_button.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.2/pkgs/aimstack/docs/boards/ui/layout_containers/columns.py` & `aim-4.0.3/pkgs/aimstack/docs/boards/ui/layout_containers/columns.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.2/pkgs/aimstack/docs/boards/ui/layout_containers/form.py` & `aim-4.0.3/pkgs/aimstack/docs/boards/ui/layout_containers/form.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.2/pkgs/aimstack/docs/boards/ui/layout_containers/rows.py` & `aim-4.0.3/pkgs/aimstack/docs/boards/ui/layout_containers/rows.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.2/pkgs/aimstack/docs/boards/ui/layout_containers/tabs.py` & `aim-4.0.3/pkgs/aimstack/docs/boards/ui/layout_containers/tabs.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.2/pkgs/aimstack/docs/boards/ui/text/code.py` & `aim-4.0.3/pkgs/aimstack/docs/boards/ui/text/code.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.2/pkgs/aimstack/docs/boards/ui/text/link.py` & `aim-4.0.3/pkgs/aimstack/docs/boards/ui/text/link.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.2/pkgs/aimstack/experiment_tracker/boards/run.py` & `aim-4.0.3/pkgs/aimstack/experiment_tracker/boards/run.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.2/pkgs/aimstack/experiment_tracker/boards/runs.py` & `aim-4.0.3/pkgs/aimstack/experiment_tracker/boards/runs.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.2/pkgs/aimstack/experiment_tracker/training_flow.py` & `aim-4.0.3/pkgs/aimstack/experiment_tracker/training_flow.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.2/pkgs/aimstack/experiment_tracker/types/deeplake_dataset.py` & `aim-4.0.3/pkgs/aimstack/experiment_tracker/types/deeplake_dataset.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.2/pkgs/aimstack/experiment_tracker/types/dvc_metadata.py` & `aim-4.0.3/pkgs/aimstack/experiment_tracker/types/dvc_metadata.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.2/pkgs/aimstack/experiment_tracker/types/hf_datasets_metadata.py` & `aim-4.0.3/pkgs/aimstack/experiment_tracker/types/hf_datasets_metadata.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.2/pkgs/aimstack/experiment_tracker/utils/pytorch.py` & `aim-4.0.3/pkgs/aimstack/experiment_tracker/utils/pytorch.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.2/pkgs/aimstack/fastai_tracker/callbacks/base_callback.py` & `aim-4.0.3/pkgs/aimstack/fastai_tracker/callbacks/base_callback.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.2/pkgs/aimstack/hugging_face_tracker/callbacks/base_callback.py` & `aim-4.0.3/pkgs/aimstack/hugging_face_tracker/callbacks/base_callback.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.2/pkgs/aimstack/keras_tracker/callbacks/base_callback.py` & `aim-4.0.3/pkgs/aimstack/keras_tracker/callbacks/base_callback.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.2/pkgs/aimstack/keras_tracker/mixins.py` & `aim-4.0.3/pkgs/aimstack/keras_tracker/mixins.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.2/pkgs/aimstack/keras_tuner_tracker/callbacks/base_callback.py` & `aim-4.0.3/pkgs/aimstack/keras_tuner_tracker/callbacks/base_callback.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.2/pkgs/aimstack/langchain_debugger/boards/cost.py` & `aim-4.0.3/pkgs/aimstack/langchain_debugger/boards/cost.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.2/pkgs/aimstack/langchain_debugger/boards/steps.py` & `aim-4.0.3/pkgs/aimstack/langchain_debugger/boards/steps.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.2/pkgs/aimstack/langchain_debugger/boards/trace.py` & `aim-4.0.3/pkgs/aimstack/langchain_debugger/boards/trace.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.2/pkgs/aimstack/langchain_debugger/boards/traces.py` & `aim-4.0.3/pkgs/aimstack/langchain_debugger/boards/traces.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.2/pkgs/aimstack/langchain_debugger/callback_handlers/generic_callback_handler.py` & `aim-4.0.3/pkgs/aimstack/langchain_debugger/callback_handlers/generic_callback_handler.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.2/pkgs/aimstack/langchain_debugger/types/action.py` & `aim-4.0.3/pkgs/aimstack/langchain_debugger/types/action.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.2/pkgs/aimstack/langchain_debugger/types/step.py` & `aim-4.0.3/pkgs/aimstack/langchain_debugger/types/step.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.2/pkgs/aimstack/langchain_debugger/types/trace.py` & `aim-4.0.3/pkgs/aimstack/langchain_debugger/types/trace.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.2/pkgs/aimstack/lightgbm_tracker/callbacks/base_callback.py` & `aim-4.0.3/pkgs/aimstack/lightgbm_tracker/callbacks/base_callback.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.2/pkgs/aimstack/llamaindex_observer/boards/cost.py` & `aim-4.0.3/pkgs/aimstack/llamaindex_observer/boards/cost.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.2/pkgs/aimstack/llamaindex_observer/boards/steps.py` & `aim-4.0.3/pkgs/aimstack/llamaindex_observer/boards/steps.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.2/pkgs/aimstack/llamaindex_observer/boards/trace.py` & `aim-4.0.3/pkgs/aimstack/llamaindex_observer/boards/trace.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.2/pkgs/aimstack/llamaindex_observer/boards/traces.py` & `aim-4.0.3/pkgs/aimstack/llamaindex_observer/boards/traces.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.2/pkgs/aimstack/llamaindex_observer/callback_handlers/generic_callback_handler.py` & `aim-4.0.3/pkgs/aimstack/llamaindex_observer/callback_handlers/generic_callback_handler.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.2/pkgs/aimstack/llamaindex_observer/types/action.py` & `aim-4.0.3/pkgs/aimstack/llamaindex_observer/types/action.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.2/pkgs/aimstack/llamaindex_observer/types/step.py` & `aim-4.0.3/pkgs/aimstack/llamaindex_observer/types/step.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.2/pkgs/aimstack/llamaindex_observer/types/trace.py` & `aim-4.0.3/pkgs/aimstack/llamaindex_observer/types/trace.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.2/pkgs/aimstack/mxnet_tracker/loggers/base_logger.py` & `aim-4.0.3/pkgs/aimstack/mxnet_tracker/loggers/base_logger.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.2/pkgs/aimstack/optuna_tracker/callbacks/base_callback.py` & `aim-4.0.3/pkgs/aimstack/optuna_tracker/callbacks/base_callback.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.2/pkgs/aimstack/paddle_tracker/callbacks/base_callback.py` & `aim-4.0.3/pkgs/aimstack/paddle_tracker/callbacks/base_callback.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.2/pkgs/aimstack/prophet_tracker/loggers/base_logger.py` & `aim-4.0.3/pkgs/aimstack/prophet_tracker/loggers/base_logger.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.2/pkgs/aimstack/pytorch_ignite_tracker/loggers/base_logger.py` & `aim-4.0.3/pkgs/aimstack/pytorch_ignite_tracker/loggers/base_logger.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.2/pkgs/aimstack/pytorch_lightning_tracker/loggers/base_logger.py` & `aim-4.0.3/pkgs/aimstack/pytorch_lightning_tracker/loggers/base_logger.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.2/pkgs/aimstack/sb3_tracker/callbacks/base_callback.py` & `aim-4.0.3/pkgs/aimstack/sb3_tracker/callbacks/base_callback.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.2/pkgs/aimstack/tensorboard_sync/run.py` & `aim-4.0.3/pkgs/aimstack/tensorboard_sync/run.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.2/pkgs/aimstack/tensorboard_sync/tracker.py` & `aim-4.0.3/pkgs/aimstack/tensorboard_sync/tracker.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.2/pkgs/aimstack/tensorflow_tracker/callbacks/base_callback.py` & `aim-4.0.3/pkgs/aimstack/tensorflow_tracker/callbacks/base_callback.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.2/pkgs/aimstack/xgboost_tracker/callbacks/base_callback.py` & `aim-4.0.3/pkgs/aimstack/xgboost_tracker/callbacks/base_callback.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.2/pyproject.toml` & `aim-4.0.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `aim-4.0.2/setup.py` & `aim-4.0.3/setup.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.2/src/aimcore/callbacks/caller.py` & `aim-4.0.3/src/aimcore/callbacks/caller.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.2/src/aimcore/callbacks/helpers.py` & `aim-4.0.3/src/aimcore/callbacks/helpers.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.2/src/aimcore/cleanup/__init__.py` & `aim-4.0.3/src/aimcore/cleanup/__init__.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.2/src/aimcore/cli/cli.py` & `aim-4.0.3/src/aimcore/cli/cli.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,30 +1,52 @@
 import click
-from click import core
+from click import core, Group
 
 from aimcore.cli.init import commands as init_commands
 from aimcore.cli.version import commands as version_commands
 from aimcore.cli.ui import commands as ui_commands
 from aimcore.cli.server import commands as server_commands
 from aimcore.cli.telemetry import commands as telemetry_commands
 from aimcore.cli.package import commands as package_commands
 from aimcore.cli.conatiners import commands as container_commands
 from aimcore.cli.migrate import commands as migrate_commands
 
+from typing import TYPE_CHECKING
+if TYPE_CHECKING:
+    from click import Context
+
 core._verify_python3_env = lambda: None
 
 
-@click.group()
+class CommandOrderedGroup(Group):
+    def get_help(self, ctx: 'Context') -> str:
+        ctx.terminal_width = 120
+        return super().get_help(ctx)
+
+    def list_commands(self, ctx: 'Context'):
+        # Return commands in the order of their definition
+        return self.commands
+
+
+@click.group(cls=CommandOrderedGroup)
 def cli_entry_point():
-    pass
+    """
+    The main entry point for Aim CLI: a toolset for tracking and managing machine learning experiments.
+
+    The Aim CLI provides a suite of commands to facilitate the tracking, visualization,
+    and management of machine learning experiments. The toolset is designed to seamlessly
+    integrate with various stages of the ML workflow, from initializing repositories and
+    tracking experiments in real-time, to visualizing results through the UI and managing
+    custom packages or apps.
+    """
 
 
 cli_entry_point.add_command(init_commands.init)
-cli_entry_point.add_command(version_commands.version)
+cli_entry_point.add_command(server_commands.server)
 cli_entry_point.add_command(ui_commands.ui)
 cli_entry_point.add_command(ui_commands.up)
-cli_entry_point.add_command(server_commands.server)
-cli_entry_point.add_command(telemetry_commands.telemetry)
 cli_entry_point.add_command(package_commands.packages)
 cli_entry_point.add_command(package_commands.packages, name='apps')
 cli_entry_point.add_command(container_commands.containers)
 cli_entry_point.add_command(migrate_commands.migrate)
+cli_entry_point.add_command(version_commands.version)
+cli_entry_point.add_command(telemetry_commands.telemetry)
```

### Comparing `aim-4.0.2/src/aimcore/cli/conatiners/commands.py` & `aim-4.0.3/src/aimcore/cli/conatiners/commands.py`

 * *Files 26% similar despite different names*

```diff
@@ -7,24 +7,39 @@
 
 @click.group()
 @click.option('--repo', required=False,
               default='aim://0.0.0.0:53800',
               type=str)
 @click.pass_context
 def containers(ctx, repo):
-    """Manage containers in aim repository."""
+    """
+    Command group for managing containers within an Aim repository.
+
+    This command group provides functionalities to list, delete, copy, move, and
+    close containers in an Aim repository. Each sub-command pertains to a specific
+    operation on the containers.
+
+    By default, the command group targets the Aim repository at 'aim://0.0.0.0:53800'.
+    A different repository can be specified using the '--repo' option.
+    """
     ctx.ensure_object(dict)
     ctx.obj['repo'] = repo
 
 
 @containers.command(name='ls')
 @click.pass_context
 def list_containers(ctx):
-    """List Containers available in Repo."""
-    # TODO [MV]: add more useful information
+    """
+    List all available containers within an Aim repository.
+
+    This command retrieves and displays containers from a specified Aim repository
+    in a tabulated format. For each container, various properties, as determined by
+    the Aim system, are shown. The default display format is 'psql',
+    which structures the output in a PostgreSQL-like table style.
+    """
     repo_path = ctx.obj['repo']
     if not Repo.is_remote_path(repo_path):
         if not Repo.exists(repo_path):
             click.echo(f'\'{repo_path}\' is not a valid aim repo.')
             exit(1)
 
     repo = Repo.from_path(repo_path)
@@ -48,15 +63,21 @@
 
 
 @containers.command(name='rm')
 @click.argument('hashes', nargs=-1, type=str)
 @click.pass_context
 @click.option('-y', '--yes', is_flag=True, help='Automatically confirm prompt')
 def remove_containers(ctx, hashes, yes):
-    """Remove Container data for given container hashes."""
+    """
+    Delete specified containers from an Aim repository.
+
+    This command deletes one or more containers identified by their hashes
+    from the Aim repository. You will be prompted for confirmation
+    before the containers are deleted unless the `--yes` option is used.
+    """
     if len(hashes) == 0:
         click.echo('Please specify at least one Container to delete.')
         exit(1)
     repo_path = ctx.obj['repo']
     repo = Repo.from_path(repo_path)
 
     matched_hashes = match_runs(repo, hashes)
@@ -77,15 +98,20 @@
 
 
 @containers.command(name='cp')
 @click.option('--destination', required=True, type=str)
 @click.argument('hashes', nargs=-1, type=str)
 @click.pass_context
 def copy_containers(ctx, destination, hashes):
-    """Copy Container data for given container hashes to destination Repo."""
+    """
+    Copy specified containers to another Aim repository.
+
+    This command copies one or more containers identified by their hashes
+    from the current Aim repository to a destination repository.
+    """
     if len(hashes) == 0:
         click.echo('Please specify at least one Container to copy.')
         exit(1)
     source = ctx.obj['repo']
     source_repo = Repo.from_path(source)
     destination_repo = Repo.from_path(destination)
 
@@ -100,15 +126,21 @@
 
 @containers.command(name='mv')
 @click.option('--destination', required=True,
               type=str)
 @click.argument('hashes', nargs=-1, type=str)
 @click.pass_context
 def move_containers(ctx, destination, hashes):
-    """Move Container data for given container hashes to destination Repo."""
+    """
+    Move specified containers to another Aim repository.
+
+    This command moves one or more containers identified by their hashes
+    from the current Aim repository to a destination repository. After the move,
+    the containers will no longer exist in the source repository.
+    """
     if len(hashes) == 0:
         click.echo('Please specify at least one Container to move.')
         exit(1)
     source = ctx.obj['repo']
     source_repo = Repo.from_path(source)
     destination_repo = Repo.from_path(destination)
 
@@ -123,15 +155,21 @@
 
 
 @containers.command(name='close')
 @click.argument('hashes', nargs=-1, type=str)
 @click.pass_context
 @click.option('-y', '--yes', is_flag=True, help='Automatically confirm prompt')
 def close_containers(ctx, hashes, yes):
-    """Close failed/stalled containers."""
+    """
+    Forcefully close specified failed or stalled containers.
+
+    This command attempts to close one or more containers that might have
+    failed or stalled. This is a forceful operation, and you'll be warned
+    to ensure the containers are not actively running.
+    """
     repo_path = ctx.obj['repo']
     repo = Repo.from_path(repo_path)
 
     if len(hashes) == 0:
         click.echo('Please specify at least one Container to close.')
         exit(1)
```

### Comparing `aim-4.0.2/src/aimcore/cli/conatiners/utils.py` & `aim-4.0.3/src/aimcore/cli/conatiners/utils.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.2/src/aimcore/cli/convert/commands.py` & `aim-4.0.3/src/aimcore/cli/convert/commands.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.2/src/aimcore/cli/convert/processors/mlflow.py` & `aim-4.0.3/src/aimcore/cli/convert/processors/mlflow.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.2/src/aimcore/cli/convert/processors/tensorboard.py` & `aim-4.0.3/src/aimcore/cli/convert/processors/tensorboard.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.2/src/aimcore/cli/convert/processors/wandb.py` & `aim-4.0.3/src/aimcore/cli/convert/processors/wandb.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.2/src/aimcore/cli/migrate/utils.py` & `aim-4.0.3/src/aimcore/cli/migrate/utils.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.2/src/aimcore/cli/package/commands.py` & `aim-4.0.3/src/aimcore/cli/package/commands.py`

 * *Files 9% similar despite different names*

```diff
@@ -7,30 +7,36 @@
 
 from .utils import init_template, pyproject_toml_template, get_pkg_distribution_sources
 from .watcher import PackageSourceWatcher
 
 
 @click.group('packages')
 def packages():
-    """Manage Aim packages/apps."""
+    """
+    Command group for managing Aim packages and apps.
+
+    Provides functionalities to create, synchronize, add, remove, and list Aim
+    packages. Each sub-command pertains to a specific operation related to
+    package management. The system ensures smooth interaction between Aim
+    repositories and the packages, allowing for seamless integration and utilization.
+    """
 
 
 @packages.command('create')
 @click.option('--name', '-n', required=True, type=str)
 @click.option('--install', '-i', is_flag=True, default=False)
 @click.option('--verbose', '-v', is_flag=True, default=False)
 def create_package(name, install, verbose):
     """
-    Create a new package with a specified name.
+    Initializes a new Aim package in the current working directory.
 
-    :param name: Name of the new package to be created.
-    :param install: Whether to install the created package using pip.
-    :param verbose: Provide verbose output when installing the package.
+    This command sets up the directory structure and necessary files for a new Aim
+    package. If the `--install` option is provided, the package will also be
+    installed in the current Python environment using pip.
     """
-
     pkg_dir = pathlib.Path(name)
     if pkg_dir.exists():
         click.echo(f'Cannot create package. Directory \'{name}\' already exists.')
         exit(1)
     try:
         package_categories = list({pkg.category for pkg in Package.pool.values()})
         package_categories.append('Other')
@@ -105,20 +111,20 @@
 
 
 @packages.command('sync')
 @click.option('--name', '-n', required=True, type=str)
 @click.option('--repo', default='', type=str)
 def sync_package(name, repo):
     """
-    Synchronize a package with a specified Aim repository.
+    Continuously sync package source code with an Aim repository.
 
-    :param name: Name of the package to be synchronized.
-    :param repo: The Aim repository to sync with. If not provided, uses default.
+    This command monitors the source directory of a specified package for changes,
+    and updates the corresponding Aim repository in real-time. It ensures the repository
+    reflects the latest version of the package code.
     """
-
     try:
         src_path = get_pkg_distribution_sources(name)
         click.echo(f'Found sources for package \'{name}\'. Location: \'{src_path}\'.')
     except Exception as e:
         click.echo(f'Failed to find sources directory for package \'{name}\'.')
         click.secho(f'Reason: {e}', fg='yellow')
         exit(1)
@@ -134,54 +140,52 @@
 
 
 @packages.command('add')
 @click.option('--name', '-n', required=True, type=str)
 @click.option('--repo', default='', type=str)
 def add_package(name, repo):
     """
-    Add a package to a specified Aim repository.
+    Register a package with an Aim repository.
 
-    :param name: Name of the package to be added.
-    :param repo: The Aim repository to add to. If not provided, uses default.
+    This command associates a specified package with an Aim repository. This means
+    that the repository will recognize the package and be able to utilize its functionalities.
     """
-
     repo_inst = Repo.from_path(repo) if repo else Repo.default()
     if not repo_inst.add_package(pkg_name=name):
         click.secho(f'Package \'{name}\' is already listed in Repo \'{repo_inst.path}\'', err=True)
         exit(1)
     click.echo(f'Added package \'{name}\' to Repo \'{repo_inst.path}\'')
 
 
 @packages.command('rm')
 @click.option('--name', '-n', required=True, type=str)
 @click.option('--repo', default='', type=str)
 def remove_package(name, repo):
     """
-    Remove a package from a specified Aim repository.
+    Deregister a package from an Aim repository.
 
-    :param name: Name of the package to be removed.
-    :param repo: The Aim repository to remove from. If not provided, uses default.
+    This command removes the association between a specified package and an Aim repository.
+    Post this operation, the repository will no longer recognize or be able to use the package.
     """
-
     repo_inst = Repo.from_path(repo) if repo else Repo.default()
     if not repo_inst.remove_package(pkg_name=name):
         click.secho(f'Package \'{name}\' is not listed in Repo \'{repo_inst.path}\'', err=True)
         exit(1)
     click.echo(f'Removed package \'{name}\' from Repo \'{repo_inst.path}\'')
 
 
 @packages.command('ls')
 @click.option('--repo', default='', type=str)
 def list_packages(repo):
     """
-    List all packages from a specified Aim repository.
+    Display all registered packages in an Aim repository.
 
-    :param repo: Path to the repository. If not specified, the default repository is used.
+    This command lists all packages that are currently associated with a specified
+    Aim repository. It provides a tabulated view of the package attributes.
     """
-
     repo_inst = Repo.from_path(repo) if repo else Repo.default()
     repo_inst.load_active_packages()
     pkg_infos = {attr_name: [] for attr_name in Package.attributes}
     for pkg in Package.pool.values():
         for attr_name in Package.attributes:
             pkg_infos[attr_name].append(getattr(pkg, attr_name))
     click.echo(tabulate.tabulate(pkg_infos, pkg_infos.keys(), tablefmt='psql'))
```

### Comparing `aim-4.0.2/src/aimcore/cli/package/utils.py` & `aim-4.0.3/src/aimcore/cli/package/utils.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.2/src/aimcore/cli/package/watcher.py` & `aim-4.0.3/src/aimcore/cli/package/watcher.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.2/src/aimcore/cli/server/commands.py` & `aim-4.0.3/src/aimcore/cli/server/commands.py`

 * *Files 10% similar despite different names*

```diff
@@ -31,14 +31,23 @@
 @click.option('--base-path', required=False, default='', type=str)
 @click.option('--log-level', required=False, default='', type=str)
 @click.option('--dev', is_flag=True, default=False)
 @click.option('-y', '--yes', is_flag=True, help='Automatically confirm prompt')
 def server(host, port,
            repo, ssl_keyfile, ssl_certfile,
            base_path, log_level, dev, yes):
+    """
+    Starts the Aim remote tracking server for real-time logging.
+
+    The Aim tracking server facilitates real-time logging of experiments
+    from remote locations. This command launches the server with specified
+    configurations, including host, port, and associated repository.
+
+    Like the UI, the server can also run in production or development mode.
+    """
     # TODO [MV, AT] remove code duplication with aim up cmd implementation
     if not log_level:
         log_level = 'debug' if dev else 'warning'
     set_log_level(log_level)
 
     if base_path:
         if base_path.endswith('/'):
```

### Comparing `aim-4.0.2/src/aimcore/cli/storage/commands.py` & `aim-4.0.3/src/aimcore/cli/storage/commands.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.2/src/aimcore/cli/ui/commands.py` & `aim-4.0.3/src/aimcore/cli/ui/commands.py`

 * *Files 6% similar despite different names*

```diff
@@ -43,22 +43,29 @@
                                                                 file_okay=True,
                                                                 dir_okay=False,
                                                                 readable=True))
 @click.option('--base-path', required=False, default='', type=str)
 @click.option('--profiler', is_flag=True, default=False)
 @click.option('--log-level', required=False, default='', type=str)
 @click.option('-y', '--yes', is_flag=True, help='Automatically confirm prompt')
-def ui(dev, host, port, workers, uds,
-       repo,
-       package,
+def ui(host, port, repo, package,
+       workers, uds,
        ssl_keyfile, ssl_certfile,
        base_path,
-       profiler, log_level, yes):
+       profiler, log_level, dev, yes):
     """
-    Start Aim UI with the --repo repository.
+    Launches the Aim web-based UI for interactive data exploration.
+
+    This command starts the Aim UI, allowing users to visually explore, compare,
+    and understand their machine learning experiments. The UI is customizable
+    with various options to determine the host, port, associated repository,
+    and more.
+
+    The UI can operate in either production or development mode, with the latter
+    offering features beneficial for Aim developers.
     """
     if not log_level:
         log_level = 'debug' if dev else 'warning'
     set_log_level(log_level)
 
     os.environ[AIM_ENV_MODE_KEY] = 'dev' if dev else 'prod'
```

### Comparing `aim-4.0.2/src/aimcore/cli/utils.py` & `aim-4.0.3/src/aimcore/cli/utils.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.2/src/aimcore/cli/watcher_cli.py` & `aim-4.0.3/src/aimcore/cli/watcher_cli.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.2/src/aimcore/error_handling.py` & `aim-4.0.3/src/aimcore/error_handling.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.2/src/aimcore/reporter/__init__.py` & `aim-4.0.3/src/aimcore/reporter/__init__.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.2/src/aimcore/transport/client.py` & `aim-4.0.3/src/aimcore/transport/client.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.2/src/aimcore/transport/handlers.py` & `aim-4.0.3/src/aimcore/transport/handlers.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.2/src/aimcore/transport/heartbeat.py` & `aim-4.0.3/src/aimcore/transport/heartbeat.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.2/src/aimcore/transport/message_utils.py` & `aim-4.0.3/src/aimcore/transport/message_utils.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.2/src/aimcore/transport/router.py` & `aim-4.0.3/src/aimcore/transport/router.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.2/src/aimcore/transport/rpc_queue.py` & `aim-4.0.3/src/aimcore/transport/rpc_queue.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.2/src/aimcore/transport/server.py` & `aim-4.0.3/src/aimcore/transport/server.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.2/src/aimcore/transport/tracking.py` & `aim-4.0.3/src/aimcore/transport/tracking.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.2/src/aimcore/web/api/__init__.py` & `aim-4.0.3/src/aimcore/web/api/__init__.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.2/src/aimcore/web/api/boards/models.py` & `aim-4.0.3/src/aimcore/web/api/boards/models.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.2/src/aimcore/web/api/boards/views.py` & `aim-4.0.3/src/aimcore/web/api/boards/views.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.2/src/aimcore/web/api/dashboard_apps/models.py` & `aim-4.0.3/src/aimcore/web/api/dashboard_apps/models.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.2/src/aimcore/web/api/dashboard_apps/pydantic_models.py` & `aim-4.0.3/src/aimcore/web/api/dashboard_apps/pydantic_models.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.2/src/aimcore/web/api/dashboard_apps/views.py` & `aim-4.0.3/src/aimcore/web/api/dashboard_apps/views.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.2/src/aimcore/web/api/dashboards/models.py` & `aim-4.0.3/src/aimcore/web/api/dashboards/models.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.2/src/aimcore/web/api/dashboards/pydantic_models.py` & `aim-4.0.3/src/aimcore/web/api/dashboards/pydantic_models.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.2/src/aimcore/web/api/dashboards/serializers.py` & `aim-4.0.3/src/aimcore/web/api/dashboards/serializers.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.2/src/aimcore/web/api/dashboards/views.py` & `aim-4.0.3/src/aimcore/web/api/dashboards/views.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.2/src/aimcore/web/api/db.py` & `aim-4.0.3/src/aimcore/web/api/db.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.2/src/aimcore/web/api/projects/project.py` & `aim-4.0.3/src/aimcore/web/api/projects/project.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.2/src/aimcore/web/api/projects/pydantic_models.py` & `aim-4.0.3/src/aimcore/web/api/projects/pydantic_models.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.2/src/aimcore/web/api/projects/views.py` & `aim-4.0.3/src/aimcore/web/api/projects/views.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.2/src/aimcore/web/api/queries/views.py` & `aim-4.0.3/src/aimcore/web/api/queries/views.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.2/src/aimcore/web/api/reports/models.py` & `aim-4.0.3/src/aimcore/web/api/reports/models.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.2/src/aimcore/web/api/reports/pydantic_models.py` & `aim-4.0.3/src/aimcore/web/api/reports/pydantic_models.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.2/src/aimcore/web/api/reports/views.py` & `aim-4.0.3/src/aimcore/web/api/reports/views.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.2/src/aimcore/web/api/runs/pydantic_models.py` & `aim-4.0.3/src/aimcore/web/api/runs/pydantic_models.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.2/src/aimcore/web/api/runs/utils.py` & `aim-4.0.3/src/aimcore/web/api/runs/utils.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.2/src/aimcore/web/api/runs/views.py` & `aim-4.0.3/src/aimcore/web/api/runs/views.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.2/src/aimcore/web/api/utils.py` & `aim-4.0.3/src/aimcore/web/api/utils.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.2/src/aimcore/web/api/views.py` & `aim-4.0.3/src/aimcore/web/api/views.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.2/src/aimcore/web/middlewares/profiler.py` & `aim-4.0.3/src/aimcore/web/middlewares/profiler.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.2/src/aimcore/web/migrations/alembic.ini` & `aim-4.0.3/src/aimcore/web/migrations/alembic.ini`

 * *Files identical despite different names*

### Comparing `aim-4.0.2/src/aimcore/web/migrations/alembic_dev.ini` & `aim-4.0.3/src/aimcore/web/migrations/alembic_dev.ini`

 * *Files identical despite different names*

### Comparing `aim-4.0.2/src/aimcore/web/migrations/env.py` & `aim-4.0.3/src/aimcore/web/migrations/env.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.2/src/aimcore/web/migrations/versions/11672b13f92c_.py` & `aim-4.0.3/src/aimcore/web/migrations/versions/11672b13f92c_.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.2/src/aimcore/web/migrations/versions/517a45b2e62c_.py` & `aim-4.0.3/src/aimcore/web/migrations/versions/517a45b2e62c_.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.2/src/aimcore/web/migrations/versions/5ae8371b7481_.py` & `aim-4.0.3/src/aimcore/web/migrations/versions/5ae8371b7481_.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.2/src/aimcore/web/migrations/versions/73a3d004c227_.py` & `aim-4.0.3/src/aimcore/web/migrations/versions/73a3d004c227_.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.2/src/aimcore/web/migrations/versions/da08eab59790_board_and_board_templates.py` & `aim-4.0.3/src/aimcore/web/migrations/versions/da08eab59790_board_and_board_templates.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.2/src/aimcore/web/migrations/versions/df1fff471cab_.py` & `aim-4.0.3/src/aimcore/web/migrations/versions/df1fff471cab_.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.2/src/aimcore/web/utils.py` & `aim-4.0.3/src/aimcore/web/utils.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.2/src/python/aim/__about__.py` & `aim-4.0.3/src/python/aim/__about__.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.2/src/python/aim/__init__.py` & `aim-4.0.3/src/python/aim/__init__.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.2/src/python/aim/_core/storage/arrayview.cpp` & `aim-4.0.3/src/python/aim/_core/storage/arrayview.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -10,22 +10,22 @@
             "-Wextra",
             "-Wconversion",
             "-fno-strict-aliasing",
             "-fno-rtti",
             "-fPIC"
         ],
         "include_dirs": [
-            "/tmp/build-env-wi9mgpyx/lib/python3.10/site-packages/aimrocks/include"
+            "/tmp/build-env-ncqe1md6/lib/python3.10/site-packages/aimrocks/include"
         ],
         "language": "c++",
         "libraries": [
             "rocksdb"
         ],
         "library_dirs": [
-            "/tmp/build-env-wi9mgpyx/lib/python3.10/site-packages/aimrocks"
+            "/tmp/build-env-ncqe1md6/lib/python3.10/site-packages/aimrocks"
         ],
         "name": "aim._core.storage.arrayview",
         "sources": [
             "src/python/aim/_core/storage/arrayview.py"
         ]
     },
     "module_name": "aim._core.storage.arrayview"
```

### Comparing `aim-4.0.2/src/python/aim/_core/storage/arrayview.py` & `aim-4.0.3/src/python/aim/_core/storage/arrayview.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.2/src/python/aim/_core/storage/container.cpp` & `aim-4.0.3/src/python/aim/_core/storage/container.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -1,56 +1,56 @@
 /* Generated by Cython 3.0.0a11 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [
-            "/tmp/build-env-wi9mgpyx/lib/python3.10/site-packages/aimrocks/include/rdb_include/comparator_wrapper.hpp",
-            "/tmp/build-env-wi9mgpyx/lib/python3.10/site-packages/aimrocks/include/rdb_include/filter_policy_wrapper.hpp",
-            "/tmp/build-env-wi9mgpyx/lib/python3.10/site-packages/aimrocks/include/rdb_include/memtable_factories.hpp",
-            "/tmp/build-env-wi9mgpyx/lib/python3.10/site-packages/aimrocks/include/rdb_include/merge_operator_wrapper.hpp",
-            "/tmp/build-env-wi9mgpyx/lib/python3.10/site-packages/aimrocks/include/rdb_include/slice_transform_wrapper.hpp",
-            "/tmp/build-env-wi9mgpyx/lib/python3.10/site-packages/aimrocks/include/rdb_include/utils.hpp",
-            "/tmp/build-env-wi9mgpyx/lib/python3.10/site-packages/aimrocks/include/rdb_include/write_batch_iter_helper.hpp",
-            "/tmp/build-env-wi9mgpyx/lib/python3.10/site-packages/aimrocks/include/rocksdb/cache.h",
-            "/tmp/build-env-wi9mgpyx/lib/python3.10/site-packages/aimrocks/include/rocksdb/comparator.h",
-            "/tmp/build-env-wi9mgpyx/lib/python3.10/site-packages/aimrocks/include/rocksdb/db.h",
-            "/tmp/build-env-wi9mgpyx/lib/python3.10/site-packages/aimrocks/include/rocksdb/env.h",
-            "/tmp/build-env-wi9mgpyx/lib/python3.10/site-packages/aimrocks/include/rocksdb/filter_policy.h",
-            "/tmp/build-env-wi9mgpyx/lib/python3.10/site-packages/aimrocks/include/rocksdb/iterator.h",
-            "/tmp/build-env-wi9mgpyx/lib/python3.10/site-packages/aimrocks/include/rocksdb/memtablerep.h",
-            "/tmp/build-env-wi9mgpyx/lib/python3.10/site-packages/aimrocks/include/rocksdb/merge_operator.h",
-            "/tmp/build-env-wi9mgpyx/lib/python3.10/site-packages/aimrocks/include/rocksdb/options.h",
-            "/tmp/build-env-wi9mgpyx/lib/python3.10/site-packages/aimrocks/include/rocksdb/slice.h",
-            "/tmp/build-env-wi9mgpyx/lib/python3.10/site-packages/aimrocks/include/rocksdb/slice_transform.h",
-            "/tmp/build-env-wi9mgpyx/lib/python3.10/site-packages/aimrocks/include/rocksdb/status.h",
-            "/tmp/build-env-wi9mgpyx/lib/python3.10/site-packages/aimrocks/include/rocksdb/table.h",
-            "/tmp/build-env-wi9mgpyx/lib/python3.10/site-packages/aimrocks/include/rocksdb/universal_compaction.h",
-            "/tmp/build-env-wi9mgpyx/lib/python3.10/site-packages/aimrocks/include/rocksdb/utilities/backup_engine.h",
-            "/tmp/build-env-wi9mgpyx/lib/python3.10/site-packages/aimrocks/include/rocksdb/write_batch.h"
+            "/tmp/build-env-ncqe1md6/lib/python3.10/site-packages/aimrocks/include/rdb_include/comparator_wrapper.hpp",
+            "/tmp/build-env-ncqe1md6/lib/python3.10/site-packages/aimrocks/include/rdb_include/filter_policy_wrapper.hpp",
+            "/tmp/build-env-ncqe1md6/lib/python3.10/site-packages/aimrocks/include/rdb_include/memtable_factories.hpp",
+            "/tmp/build-env-ncqe1md6/lib/python3.10/site-packages/aimrocks/include/rdb_include/merge_operator_wrapper.hpp",
+            "/tmp/build-env-ncqe1md6/lib/python3.10/site-packages/aimrocks/include/rdb_include/slice_transform_wrapper.hpp",
+            "/tmp/build-env-ncqe1md6/lib/python3.10/site-packages/aimrocks/include/rdb_include/utils.hpp",
+            "/tmp/build-env-ncqe1md6/lib/python3.10/site-packages/aimrocks/include/rdb_include/write_batch_iter_helper.hpp",
+            "/tmp/build-env-ncqe1md6/lib/python3.10/site-packages/aimrocks/include/rocksdb/cache.h",
+            "/tmp/build-env-ncqe1md6/lib/python3.10/site-packages/aimrocks/include/rocksdb/comparator.h",
+            "/tmp/build-env-ncqe1md6/lib/python3.10/site-packages/aimrocks/include/rocksdb/db.h",
+            "/tmp/build-env-ncqe1md6/lib/python3.10/site-packages/aimrocks/include/rocksdb/env.h",
+            "/tmp/build-env-ncqe1md6/lib/python3.10/site-packages/aimrocks/include/rocksdb/filter_policy.h",
+            "/tmp/build-env-ncqe1md6/lib/python3.10/site-packages/aimrocks/include/rocksdb/iterator.h",
+            "/tmp/build-env-ncqe1md6/lib/python3.10/site-packages/aimrocks/include/rocksdb/memtablerep.h",
+            "/tmp/build-env-ncqe1md6/lib/python3.10/site-packages/aimrocks/include/rocksdb/merge_operator.h",
+            "/tmp/build-env-ncqe1md6/lib/python3.10/site-packages/aimrocks/include/rocksdb/options.h",
+            "/tmp/build-env-ncqe1md6/lib/python3.10/site-packages/aimrocks/include/rocksdb/slice.h",
+            "/tmp/build-env-ncqe1md6/lib/python3.10/site-packages/aimrocks/include/rocksdb/slice_transform.h",
+            "/tmp/build-env-ncqe1md6/lib/python3.10/site-packages/aimrocks/include/rocksdb/status.h",
+            "/tmp/build-env-ncqe1md6/lib/python3.10/site-packages/aimrocks/include/rocksdb/table.h",
+            "/tmp/build-env-ncqe1md6/lib/python3.10/site-packages/aimrocks/include/rocksdb/universal_compaction.h",
+            "/tmp/build-env-ncqe1md6/lib/python3.10/site-packages/aimrocks/include/rocksdb/utilities/backup_engine.h",
+            "/tmp/build-env-ncqe1md6/lib/python3.10/site-packages/aimrocks/include/rocksdb/write_batch.h"
         ],
         "extra_compile_args": [
             "-std=c++11",
             "-O3",
             "-Wall",
             "-Wextra",
             "-Wconversion",
             "-fno-strict-aliasing",
             "-fno-rtti",
             "-fPIC"
         ],
         "include_dirs": [
-            "/tmp/build-env-wi9mgpyx/lib/python3.10/site-packages/aimrocks/include"
+            "/tmp/build-env-ncqe1md6/lib/python3.10/site-packages/aimrocks/include"
         ],
         "language": "c++",
         "libraries": [
             "rocksdb"
         ],
         "library_dirs": [
-            "/tmp/build-env-wi9mgpyx/lib/python3.10/site-packages/aimrocks"
+            "/tmp/build-env-ncqe1md6/lib/python3.10/site-packages/aimrocks"
         ],
         "name": "aim._core.storage.container",
         "sources": [
             "src/python/aim/_core/storage/container.py"
         ]
     },
     "module_name": "aim._core.storage.container"
```

### Comparing `aim-4.0.2/src/python/aim/_core/storage/container.pxd` & `aim-4.0.3/src/python/aim/_core/storage/container.pxd`

 * *Files identical despite different names*

### Comparing `aim-4.0.2/src/python/aim/_core/storage/container.py` & `aim-4.0.3/src/python/aim/_core/storage/container.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.2/src/python/aim/_core/storage/containertreeview.cpp` & `aim-4.0.3/src/python/aim/_core/storage/containertreeview.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -1,56 +1,56 @@
 /* Generated by Cython 3.0.0a11 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [
-            "/tmp/build-env-wi9mgpyx/lib/python3.10/site-packages/aimrocks/include/rdb_include/comparator_wrapper.hpp",
-            "/tmp/build-env-wi9mgpyx/lib/python3.10/site-packages/aimrocks/include/rdb_include/filter_policy_wrapper.hpp",
-            "/tmp/build-env-wi9mgpyx/lib/python3.10/site-packages/aimrocks/include/rdb_include/memtable_factories.hpp",
-            "/tmp/build-env-wi9mgpyx/lib/python3.10/site-packages/aimrocks/include/rdb_include/merge_operator_wrapper.hpp",
-            "/tmp/build-env-wi9mgpyx/lib/python3.10/site-packages/aimrocks/include/rdb_include/slice_transform_wrapper.hpp",
-            "/tmp/build-env-wi9mgpyx/lib/python3.10/site-packages/aimrocks/include/rdb_include/utils.hpp",
-            "/tmp/build-env-wi9mgpyx/lib/python3.10/site-packages/aimrocks/include/rdb_include/write_batch_iter_helper.hpp",
-            "/tmp/build-env-wi9mgpyx/lib/python3.10/site-packages/aimrocks/include/rocksdb/cache.h",
-            "/tmp/build-env-wi9mgpyx/lib/python3.10/site-packages/aimrocks/include/rocksdb/comparator.h",
-            "/tmp/build-env-wi9mgpyx/lib/python3.10/site-packages/aimrocks/include/rocksdb/db.h",
-            "/tmp/build-env-wi9mgpyx/lib/python3.10/site-packages/aimrocks/include/rocksdb/env.h",
-            "/tmp/build-env-wi9mgpyx/lib/python3.10/site-packages/aimrocks/include/rocksdb/filter_policy.h",
-            "/tmp/build-env-wi9mgpyx/lib/python3.10/site-packages/aimrocks/include/rocksdb/iterator.h",
-            "/tmp/build-env-wi9mgpyx/lib/python3.10/site-packages/aimrocks/include/rocksdb/memtablerep.h",
-            "/tmp/build-env-wi9mgpyx/lib/python3.10/site-packages/aimrocks/include/rocksdb/merge_operator.h",
-            "/tmp/build-env-wi9mgpyx/lib/python3.10/site-packages/aimrocks/include/rocksdb/options.h",
-            "/tmp/build-env-wi9mgpyx/lib/python3.10/site-packages/aimrocks/include/rocksdb/slice.h",
-            "/tmp/build-env-wi9mgpyx/lib/python3.10/site-packages/aimrocks/include/rocksdb/slice_transform.h",
-            "/tmp/build-env-wi9mgpyx/lib/python3.10/site-packages/aimrocks/include/rocksdb/status.h",
-            "/tmp/build-env-wi9mgpyx/lib/python3.10/site-packages/aimrocks/include/rocksdb/table.h",
-            "/tmp/build-env-wi9mgpyx/lib/python3.10/site-packages/aimrocks/include/rocksdb/universal_compaction.h",
-            "/tmp/build-env-wi9mgpyx/lib/python3.10/site-packages/aimrocks/include/rocksdb/utilities/backup_engine.h",
-            "/tmp/build-env-wi9mgpyx/lib/python3.10/site-packages/aimrocks/include/rocksdb/write_batch.h"
+            "/tmp/build-env-ncqe1md6/lib/python3.10/site-packages/aimrocks/include/rdb_include/comparator_wrapper.hpp",
+            "/tmp/build-env-ncqe1md6/lib/python3.10/site-packages/aimrocks/include/rdb_include/filter_policy_wrapper.hpp",
+            "/tmp/build-env-ncqe1md6/lib/python3.10/site-packages/aimrocks/include/rdb_include/memtable_factories.hpp",
+            "/tmp/build-env-ncqe1md6/lib/python3.10/site-packages/aimrocks/include/rdb_include/merge_operator_wrapper.hpp",
+            "/tmp/build-env-ncqe1md6/lib/python3.10/site-packages/aimrocks/include/rdb_include/slice_transform_wrapper.hpp",
+            "/tmp/build-env-ncqe1md6/lib/python3.10/site-packages/aimrocks/include/rdb_include/utils.hpp",
+            "/tmp/build-env-ncqe1md6/lib/python3.10/site-packages/aimrocks/include/rdb_include/write_batch_iter_helper.hpp",
+            "/tmp/build-env-ncqe1md6/lib/python3.10/site-packages/aimrocks/include/rocksdb/cache.h",
+            "/tmp/build-env-ncqe1md6/lib/python3.10/site-packages/aimrocks/include/rocksdb/comparator.h",
+            "/tmp/build-env-ncqe1md6/lib/python3.10/site-packages/aimrocks/include/rocksdb/db.h",
+            "/tmp/build-env-ncqe1md6/lib/python3.10/site-packages/aimrocks/include/rocksdb/env.h",
+            "/tmp/build-env-ncqe1md6/lib/python3.10/site-packages/aimrocks/include/rocksdb/filter_policy.h",
+            "/tmp/build-env-ncqe1md6/lib/python3.10/site-packages/aimrocks/include/rocksdb/iterator.h",
+            "/tmp/build-env-ncqe1md6/lib/python3.10/site-packages/aimrocks/include/rocksdb/memtablerep.h",
+            "/tmp/build-env-ncqe1md6/lib/python3.10/site-packages/aimrocks/include/rocksdb/merge_operator.h",
+            "/tmp/build-env-ncqe1md6/lib/python3.10/site-packages/aimrocks/include/rocksdb/options.h",
+            "/tmp/build-env-ncqe1md6/lib/python3.10/site-packages/aimrocks/include/rocksdb/slice.h",
+            "/tmp/build-env-ncqe1md6/lib/python3.10/site-packages/aimrocks/include/rocksdb/slice_transform.h",
+            "/tmp/build-env-ncqe1md6/lib/python3.10/site-packages/aimrocks/include/rocksdb/status.h",
+            "/tmp/build-env-ncqe1md6/lib/python3.10/site-packages/aimrocks/include/rocksdb/table.h",
+            "/tmp/build-env-ncqe1md6/lib/python3.10/site-packages/aimrocks/include/rocksdb/universal_compaction.h",
+            "/tmp/build-env-ncqe1md6/lib/python3.10/site-packages/aimrocks/include/rocksdb/utilities/backup_engine.h",
+            "/tmp/build-env-ncqe1md6/lib/python3.10/site-packages/aimrocks/include/rocksdb/write_batch.h"
         ],
         "extra_compile_args": [
             "-std=c++11",
             "-O3",
             "-Wall",
             "-Wextra",
             "-Wconversion",
             "-fno-strict-aliasing",
             "-fno-rtti",
             "-fPIC"
         ],
         "include_dirs": [
-            "/tmp/build-env-wi9mgpyx/lib/python3.10/site-packages/aimrocks/include"
+            "/tmp/build-env-ncqe1md6/lib/python3.10/site-packages/aimrocks/include"
         ],
         "language": "c++",
         "libraries": [
             "rocksdb"
         ],
         "library_dirs": [
-            "/tmp/build-env-wi9mgpyx/lib/python3.10/site-packages/aimrocks"
+            "/tmp/build-env-ncqe1md6/lib/python3.10/site-packages/aimrocks"
         ],
         "name": "aim._core.storage.containertreeview",
         "sources": [
             "src/python/aim/_core/storage/containertreeview.py"
         ]
     },
     "module_name": "aim._core.storage.containertreeview"
```

### Comparing `aim-4.0.2/src/python/aim/_core/storage/containertreeview.py` & `aim-4.0.3/src/python/aim/_core/storage/containertreeview.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.2/src/python/aim/_core/storage/encoding/__init__.cpp` & `aim-4.0.3/src/python/aim/_core/storage/encoding/__init__.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -11,22 +11,22 @@
             "-Wextra",
             "-Wconversion",
             "-fno-strict-aliasing",
             "-fno-rtti",
             "-fPIC"
         ],
         "include_dirs": [
-            "/tmp/build-env-wi9mgpyx/lib/python3.10/site-packages/aimrocks/include"
+            "/tmp/build-env-ncqe1md6/lib/python3.10/site-packages/aimrocks/include"
         ],
         "language": "c++",
         "libraries": [
             "rocksdb"
         ],
         "library_dirs": [
-            "/tmp/build-env-wi9mgpyx/lib/python3.10/site-packages/aimrocks"
+            "/tmp/build-env-ncqe1md6/lib/python3.10/site-packages/aimrocks"
         ],
         "name": "aim._core.storage.encoding",
         "sources": [
             "src/python/aim/_core/storage/encoding/__init__.py"
         ]
     },
     "module_name": "aim._core.storage.encoding"
```

### Comparing `aim-4.0.2/src/python/aim/_core/storage/encoding/encoding.cpp` & `aim-4.0.3/src/python/aim/_core/storage/encoding/encoding.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -11,22 +11,22 @@
             "-Wextra",
             "-Wconversion",
             "-fno-strict-aliasing",
             "-fno-rtti",
             "-fPIC"
         ],
         "include_dirs": [
-            "/tmp/build-env-wi9mgpyx/lib/python3.10/site-packages/aimrocks/include"
+            "/tmp/build-env-ncqe1md6/lib/python3.10/site-packages/aimrocks/include"
         ],
         "language": "c++",
         "libraries": [
             "rocksdb"
         ],
         "library_dirs": [
-            "/tmp/build-env-wi9mgpyx/lib/python3.10/site-packages/aimrocks"
+            "/tmp/build-env-ncqe1md6/lib/python3.10/site-packages/aimrocks"
         ],
         "name": "aim._core.storage.encoding.encoding",
         "sources": [
             "src/python/aim/_core/storage/encoding/encoding.pyx"
         ]
     },
     "module_name": "aim._core.storage.encoding.encoding"
```

### Comparing `aim-4.0.2/src/python/aim/_core/storage/encoding/encoding.pyx` & `aim-4.0.3/src/python/aim/_core/storage/encoding/encoding.pyx`

 * *Files identical despite different names*

### Comparing `aim-4.0.2/src/python/aim/_core/storage/encoding/encoding_native.cpp` & `aim-4.0.3/src/python/aim/_core/storage/encoding/encoding_native.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -11,22 +11,22 @@
             "-Wextra",
             "-Wconversion",
             "-fno-strict-aliasing",
             "-fno-rtti",
             "-fPIC"
         ],
         "include_dirs": [
-            "/tmp/build-env-wi9mgpyx/lib/python3.10/site-packages/aimrocks/include"
+            "/tmp/build-env-ncqe1md6/lib/python3.10/site-packages/aimrocks/include"
         ],
         "language": "c++",
         "libraries": [
             "rocksdb"
         ],
         "library_dirs": [
-            "/tmp/build-env-wi9mgpyx/lib/python3.10/site-packages/aimrocks"
+            "/tmp/build-env-ncqe1md6/lib/python3.10/site-packages/aimrocks"
         ],
         "name": "aim._core.storage.encoding.encoding_native",
         "sources": [
             "src/python/aim/_core/storage/encoding/encoding_native.pyx"
         ]
     },
     "module_name": "aim._core.storage.encoding.encoding_native"
```

### Comparing `aim-4.0.2/src/python/aim/_core/storage/encoding/encoding_native.pxd` & `aim-4.0.3/src/python/aim/_core/storage/encoding/encoding_native.pxd`

 * *Files identical despite different names*

### Comparing `aim-4.0.2/src/python/aim/_core/storage/encoding/encoding_native.pyx` & `aim-4.0.3/src/python/aim/_core/storage/encoding/encoding_native.pyx`

 * *Files identical despite different names*

### Comparing `aim-4.0.2/src/python/aim/_core/storage/hashing/__init__.cpp` & `aim-4.0.3/src/python/aim/_core/storage/hashing/__init__.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -14,22 +14,22 @@
             "-Wconversion",
             "-fno-strict-aliasing",
             "-fno-rtti",
             "-fPIC"
         ],
         "include_dirs": [
             "src/python/aim/_core/storage/hashing",
-            "/tmp/build-env-wi9mgpyx/lib/python3.10/site-packages/aimrocks/include"
+            "/tmp/build-env-ncqe1md6/lib/python3.10/site-packages/aimrocks/include"
         ],
         "language": "c++",
         "libraries": [
             "rocksdb"
         ],
         "library_dirs": [
-            "/tmp/build-env-wi9mgpyx/lib/python3.10/site-packages/aimrocks"
+            "/tmp/build-env-ncqe1md6/lib/python3.10/site-packages/aimrocks"
         ],
         "name": "aim._core.storage.hashing",
         "sources": [
             "src/python/aim/_core/storage/hashing/__init__.py"
         ]
     },
     "module_name": "aim._core.storage.hashing"
```

### Comparing `aim-4.0.2/src/python/aim/_core/storage/hashing/c_hash.cpp` & `aim-4.0.3/src/python/aim/_core/storage/hashing/c_hash.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -14,23 +14,23 @@
             "-Wconversion",
             "-fno-strict-aliasing",
             "-fno-rtti",
             "-fPIC"
         ],
         "include_dirs": [
             "src/python/aim/_core/storage/hashing",
-            "/tmp/build-env-wi9mgpyx/lib/python3.10/site-packages/aimrocks/include"
+            "/tmp/build-env-ncqe1md6/lib/python3.10/site-packages/aimrocks/include"
         ],
         "language": "c++",
         "language_level": "3",
         "libraries": [
             "rocksdb"
         ],
         "library_dirs": [
-            "/tmp/build-env-wi9mgpyx/lib/python3.10/site-packages/aimrocks"
+            "/tmp/build-env-ncqe1md6/lib/python3.10/site-packages/aimrocks"
         ],
         "name": "aim._core.storage.hashing.c_hash",
         "sources": [
             "src/python/aim/_core/storage/hashing/c_hash.pyx"
         ]
     },
     "module_name": "aim._core.storage.hashing.c_hash"
```

### Comparing `aim-4.0.2/src/python/aim/_core/storage/hashing/c_hash.pyx` & `aim-4.0.3/src/python/aim/_core/storage/hashing/c_hash.pyx`

 * *Files identical despite different names*

### Comparing `aim-4.0.2/src/python/aim/_core/storage/hashing/hash/hash.h` & `aim-4.0.3/src/python/aim/_core/storage/hashing/hash/hash.h`

 * *Files identical despite different names*

### Comparing `aim-4.0.2/src/python/aim/_core/storage/hashing/hashing.cpp` & `aim-4.0.3/src/python/aim/_core/storage/hashing/hashing.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -14,22 +14,22 @@
             "-Wconversion",
             "-fno-strict-aliasing",
             "-fno-rtti",
             "-fPIC"
         ],
         "include_dirs": [
             "src/python/aim/_core/storage/hashing",
-            "/tmp/build-env-wi9mgpyx/lib/python3.10/site-packages/aimrocks/include"
+            "/tmp/build-env-ncqe1md6/lib/python3.10/site-packages/aimrocks/include"
         ],
         "language": "c++",
         "libraries": [
             "rocksdb"
         ],
         "library_dirs": [
-            "/tmp/build-env-wi9mgpyx/lib/python3.10/site-packages/aimrocks"
+            "/tmp/build-env-ncqe1md6/lib/python3.10/site-packages/aimrocks"
         ],
         "name": "aim._core.storage.hashing.hashing",
         "sources": [
             "src/python/aim/_core/storage/hashing/hashing.py"
         ]
     },
     "module_name": "aim._core.storage.hashing.hashing"
```

### Comparing `aim-4.0.2/src/python/aim/_core/storage/hashing/hashing.pxd` & `aim-4.0.3/src/python/aim/_core/storage/hashing/hashing.pxd`

 * *Files identical despite different names*

### Comparing `aim-4.0.2/src/python/aim/_core/storage/hashing/hashing.py` & `aim-4.0.3/src/python/aim/_core/storage/hashing/hashing.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.2/src/python/aim/_core/storage/inmemorytreeview.cpp` & `aim-4.0.3/src/python/aim/_core/storage/inmemorytreeview.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -10,22 +10,22 @@
             "-Wextra",
             "-Wconversion",
             "-fno-strict-aliasing",
             "-fno-rtti",
             "-fPIC"
         ],
         "include_dirs": [
-            "/tmp/build-env-wi9mgpyx/lib/python3.10/site-packages/aimrocks/include"
+            "/tmp/build-env-ncqe1md6/lib/python3.10/site-packages/aimrocks/include"
         ],
         "language": "c++",
         "libraries": [
             "rocksdb"
         ],
         "library_dirs": [
-            "/tmp/build-env-wi9mgpyx/lib/python3.10/site-packages/aimrocks"
+            "/tmp/build-env-ncqe1md6/lib/python3.10/site-packages/aimrocks"
         ],
         "name": "aim._core.storage.inmemorytreeview",
         "sources": [
             "src/python/aim/_core/storage/inmemorytreeview.py"
         ]
     },
     "module_name": "aim._core.storage.inmemorytreeview"
```

### Comparing `aim-4.0.2/src/python/aim/_core/storage/inmemorytreeview.py` & `aim-4.0.3/src/python/aim/_core/storage/inmemorytreeview.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.2/src/python/aim/_core/storage/locking.py` & `aim-4.0.3/src/python/aim/_core/storage/locking.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.2/src/python/aim/_core/storage/object.py` & `aim-4.0.3/src/python/aim/_core/storage/object.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.2/src/python/aim/_core/storage/prefixview.cpp` & `aim-4.0.3/src/python/aim/_core/storage/prefixview.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -1,56 +1,56 @@
 /* Generated by Cython 3.0.0a11 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [
-            "/tmp/build-env-wi9mgpyx/lib/python3.10/site-packages/aimrocks/include/rdb_include/comparator_wrapper.hpp",
-            "/tmp/build-env-wi9mgpyx/lib/python3.10/site-packages/aimrocks/include/rdb_include/filter_policy_wrapper.hpp",
-            "/tmp/build-env-wi9mgpyx/lib/python3.10/site-packages/aimrocks/include/rdb_include/memtable_factories.hpp",
-            "/tmp/build-env-wi9mgpyx/lib/python3.10/site-packages/aimrocks/include/rdb_include/merge_operator_wrapper.hpp",
-            "/tmp/build-env-wi9mgpyx/lib/python3.10/site-packages/aimrocks/include/rdb_include/slice_transform_wrapper.hpp",
-            "/tmp/build-env-wi9mgpyx/lib/python3.10/site-packages/aimrocks/include/rdb_include/utils.hpp",
-            "/tmp/build-env-wi9mgpyx/lib/python3.10/site-packages/aimrocks/include/rdb_include/write_batch_iter_helper.hpp",
-            "/tmp/build-env-wi9mgpyx/lib/python3.10/site-packages/aimrocks/include/rocksdb/cache.h",
-            "/tmp/build-env-wi9mgpyx/lib/python3.10/site-packages/aimrocks/include/rocksdb/comparator.h",
-            "/tmp/build-env-wi9mgpyx/lib/python3.10/site-packages/aimrocks/include/rocksdb/db.h",
-            "/tmp/build-env-wi9mgpyx/lib/python3.10/site-packages/aimrocks/include/rocksdb/env.h",
-            "/tmp/build-env-wi9mgpyx/lib/python3.10/site-packages/aimrocks/include/rocksdb/filter_policy.h",
-            "/tmp/build-env-wi9mgpyx/lib/python3.10/site-packages/aimrocks/include/rocksdb/iterator.h",
-            "/tmp/build-env-wi9mgpyx/lib/python3.10/site-packages/aimrocks/include/rocksdb/memtablerep.h",
-            "/tmp/build-env-wi9mgpyx/lib/python3.10/site-packages/aimrocks/include/rocksdb/merge_operator.h",
-            "/tmp/build-env-wi9mgpyx/lib/python3.10/site-packages/aimrocks/include/rocksdb/options.h",
-            "/tmp/build-env-wi9mgpyx/lib/python3.10/site-packages/aimrocks/include/rocksdb/slice.h",
-            "/tmp/build-env-wi9mgpyx/lib/python3.10/site-packages/aimrocks/include/rocksdb/slice_transform.h",
-            "/tmp/build-env-wi9mgpyx/lib/python3.10/site-packages/aimrocks/include/rocksdb/status.h",
-            "/tmp/build-env-wi9mgpyx/lib/python3.10/site-packages/aimrocks/include/rocksdb/table.h",
-            "/tmp/build-env-wi9mgpyx/lib/python3.10/site-packages/aimrocks/include/rocksdb/universal_compaction.h",
-            "/tmp/build-env-wi9mgpyx/lib/python3.10/site-packages/aimrocks/include/rocksdb/utilities/backup_engine.h",
-            "/tmp/build-env-wi9mgpyx/lib/python3.10/site-packages/aimrocks/include/rocksdb/write_batch.h"
+            "/tmp/build-env-ncqe1md6/lib/python3.10/site-packages/aimrocks/include/rdb_include/comparator_wrapper.hpp",
+            "/tmp/build-env-ncqe1md6/lib/python3.10/site-packages/aimrocks/include/rdb_include/filter_policy_wrapper.hpp",
+            "/tmp/build-env-ncqe1md6/lib/python3.10/site-packages/aimrocks/include/rdb_include/memtable_factories.hpp",
+            "/tmp/build-env-ncqe1md6/lib/python3.10/site-packages/aimrocks/include/rdb_include/merge_operator_wrapper.hpp",
+            "/tmp/build-env-ncqe1md6/lib/python3.10/site-packages/aimrocks/include/rdb_include/slice_transform_wrapper.hpp",
+            "/tmp/build-env-ncqe1md6/lib/python3.10/site-packages/aimrocks/include/rdb_include/utils.hpp",
+            "/tmp/build-env-ncqe1md6/lib/python3.10/site-packages/aimrocks/include/rdb_include/write_batch_iter_helper.hpp",
+            "/tmp/build-env-ncqe1md6/lib/python3.10/site-packages/aimrocks/include/rocksdb/cache.h",
+            "/tmp/build-env-ncqe1md6/lib/python3.10/site-packages/aimrocks/include/rocksdb/comparator.h",
+            "/tmp/build-env-ncqe1md6/lib/python3.10/site-packages/aimrocks/include/rocksdb/db.h",
+            "/tmp/build-env-ncqe1md6/lib/python3.10/site-packages/aimrocks/include/rocksdb/env.h",
+            "/tmp/build-env-ncqe1md6/lib/python3.10/site-packages/aimrocks/include/rocksdb/filter_policy.h",
+            "/tmp/build-env-ncqe1md6/lib/python3.10/site-packages/aimrocks/include/rocksdb/iterator.h",
+            "/tmp/build-env-ncqe1md6/lib/python3.10/site-packages/aimrocks/include/rocksdb/memtablerep.h",
+            "/tmp/build-env-ncqe1md6/lib/python3.10/site-packages/aimrocks/include/rocksdb/merge_operator.h",
+            "/tmp/build-env-ncqe1md6/lib/python3.10/site-packages/aimrocks/include/rocksdb/options.h",
+            "/tmp/build-env-ncqe1md6/lib/python3.10/site-packages/aimrocks/include/rocksdb/slice.h",
+            "/tmp/build-env-ncqe1md6/lib/python3.10/site-packages/aimrocks/include/rocksdb/slice_transform.h",
+            "/tmp/build-env-ncqe1md6/lib/python3.10/site-packages/aimrocks/include/rocksdb/status.h",
+            "/tmp/build-env-ncqe1md6/lib/python3.10/site-packages/aimrocks/include/rocksdb/table.h",
+            "/tmp/build-env-ncqe1md6/lib/python3.10/site-packages/aimrocks/include/rocksdb/universal_compaction.h",
+            "/tmp/build-env-ncqe1md6/lib/python3.10/site-packages/aimrocks/include/rocksdb/utilities/backup_engine.h",
+            "/tmp/build-env-ncqe1md6/lib/python3.10/site-packages/aimrocks/include/rocksdb/write_batch.h"
         ],
         "extra_compile_args": [
             "-std=c++11",
             "-O3",
             "-Wall",
             "-Wextra",
             "-Wconversion",
             "-fno-strict-aliasing",
             "-fno-rtti",
             "-fPIC"
         ],
         "include_dirs": [
-            "/tmp/build-env-wi9mgpyx/lib/python3.10/site-packages/aimrocks/include"
+            "/tmp/build-env-ncqe1md6/lib/python3.10/site-packages/aimrocks/include"
         ],
         "language": "c++",
         "libraries": [
             "rocksdb"
         ],
         "library_dirs": [
-            "/tmp/build-env-wi9mgpyx/lib/python3.10/site-packages/aimrocks"
+            "/tmp/build-env-ncqe1md6/lib/python3.10/site-packages/aimrocks"
         ],
         "name": "aim._core.storage.prefixview",
         "sources": [
             "src/python/aim/_core/storage/prefixview.py"
         ]
     },
     "module_name": "aim._core.storage.prefixview"
```

### Comparing `aim-4.0.2/src/python/aim/_core/storage/prefixview.pxd` & `aim-4.0.3/src/python/aim/_core/storage/prefixview.pxd`

 * *Files identical despite different names*

### Comparing `aim-4.0.2/src/python/aim/_core/storage/prefixview.py` & `aim-4.0.3/src/python/aim/_core/storage/prefixview.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.2/src/python/aim/_core/storage/proxy.py` & `aim-4.0.3/src/python/aim/_core/storage/proxy.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.2/src/python/aim/_core/storage/rockscontainer.cpp` & `aim-4.0.3/src/python/aim/_core/storage/rockscontainer.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -10,22 +10,22 @@
             "-Wextra",
             "-Wconversion",
             "-fno-strict-aliasing",
             "-fno-rtti",
             "-fPIC"
         ],
         "include_dirs": [
-            "/tmp/build-env-wi9mgpyx/lib/python3.10/site-packages/aimrocks/include"
+            "/tmp/build-env-ncqe1md6/lib/python3.10/site-packages/aimrocks/include"
         ],
         "language": "c++",
         "libraries": [
             "rocksdb"
         ],
         "library_dirs": [
-            "/tmp/build-env-wi9mgpyx/lib/python3.10/site-packages/aimrocks"
+            "/tmp/build-env-ncqe1md6/lib/python3.10/site-packages/aimrocks"
         ],
         "name": "aim._core.storage.rockscontainer",
         "sources": [
             "src/python/aim/_core/storage/rockscontainer.pyx"
         ]
     },
     "module_name": "aim._core.storage.rockscontainer"
```

### Comparing `aim-4.0.2/src/python/aim/_core/storage/rockscontainer.pyx` & `aim-4.0.3/src/python/aim/_core/storage/rockscontainer.pyx`

 * *Files identical despite different names*

### Comparing `aim-4.0.2/src/python/aim/_core/storage/treearrayview.cpp` & `aim-4.0.3/src/python/aim/_core/storage/treearrayview.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -10,22 +10,22 @@
             "-Wextra",
             "-Wconversion",
             "-fno-strict-aliasing",
             "-fno-rtti",
             "-fPIC"
         ],
         "include_dirs": [
-            "/tmp/build-env-wi9mgpyx/lib/python3.10/site-packages/aimrocks/include"
+            "/tmp/build-env-ncqe1md6/lib/python3.10/site-packages/aimrocks/include"
         ],
         "language": "c++",
         "libraries": [
             "rocksdb"
         ],
         "library_dirs": [
-            "/tmp/build-env-wi9mgpyx/lib/python3.10/site-packages/aimrocks"
+            "/tmp/build-env-ncqe1md6/lib/python3.10/site-packages/aimrocks"
         ],
         "name": "aim._core.storage.treearrayview",
         "sources": [
             "src/python/aim/_core/storage/treearrayview.py"
         ]
     },
     "module_name": "aim._core.storage.treearrayview"
```

### Comparing `aim-4.0.2/src/python/aim/_core/storage/treearrayview.py` & `aim-4.0.3/src/python/aim/_core/storage/treearrayview.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.2/src/python/aim/_core/storage/treeutils.cpp` & `aim-4.0.3/src/python/aim/_core/storage/treeutils.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -11,22 +11,22 @@
             "-Wextra",
             "-Wconversion",
             "-fno-strict-aliasing",
             "-fno-rtti",
             "-fPIC"
         ],
         "include_dirs": [
-            "/tmp/build-env-wi9mgpyx/lib/python3.10/site-packages/aimrocks/include"
+            "/tmp/build-env-ncqe1md6/lib/python3.10/site-packages/aimrocks/include"
         ],
         "language": "c++",
         "libraries": [
             "rocksdb"
         ],
         "library_dirs": [
-            "/tmp/build-env-wi9mgpyx/lib/python3.10/site-packages/aimrocks"
+            "/tmp/build-env-ncqe1md6/lib/python3.10/site-packages/aimrocks"
         ],
         "name": "aim._core.storage.treeutils",
         "sources": [
             "src/python/aim/_core/storage/treeutils.pyx"
         ]
     },
     "module_name": "aim._core.storage.treeutils"
```

### Comparing `aim-4.0.2/src/python/aim/_core/storage/treeutils.pyx` & `aim-4.0.3/src/python/aim/_core/storage/treeutils.pyx`

 * *Files identical despite different names*

### Comparing `aim-4.0.2/src/python/aim/_core/storage/treeutils_non_native.py` & `aim-4.0.3/src/python/aim/_core/storage/treeutils_non_native.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.2/src/python/aim/_core/storage/treeview.cpp` & `aim-4.0.3/src/python/aim/_core/storage/treeview.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -10,22 +10,22 @@
             "-Wextra",
             "-Wconversion",
             "-fno-strict-aliasing",
             "-fno-rtti",
             "-fPIC"
         ],
         "include_dirs": [
-            "/tmp/build-env-wi9mgpyx/lib/python3.10/site-packages/aimrocks/include"
+            "/tmp/build-env-ncqe1md6/lib/python3.10/site-packages/aimrocks/include"
         ],
         "language": "c++",
         "libraries": [
             "rocksdb"
         ],
         "library_dirs": [
-            "/tmp/build-env-wi9mgpyx/lib/python3.10/site-packages/aimrocks"
+            "/tmp/build-env-ncqe1md6/lib/python3.10/site-packages/aimrocks"
         ],
         "name": "aim._core.storage.treeview",
         "sources": [
             "src/python/aim/_core/storage/treeview.py"
         ]
     },
     "module_name": "aim._core.storage.treeview"
```

### Comparing `aim-4.0.2/src/python/aim/_core/storage/treeview.py` & `aim-4.0.3/src/python/aim/_core/storage/treeview.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.2/src/python/aim/_core/storage/types.py` & `aim-4.0.3/src/python/aim/_core/storage/types.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.2/src/python/aim/_core/storage/union.cpp` & `aim-4.0.3/src/python/aim/_core/storage/union.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -10,22 +10,22 @@
             "-Wextra",
             "-Wconversion",
             "-fno-strict-aliasing",
             "-fno-rtti",
             "-fPIC"
         ],
         "include_dirs": [
-            "/tmp/build-env-wi9mgpyx/lib/python3.10/site-packages/aimrocks/include"
+            "/tmp/build-env-ncqe1md6/lib/python3.10/site-packages/aimrocks/include"
         ],
         "language": "c++",
         "libraries": [
             "rocksdb"
         ],
         "library_dirs": [
-            "/tmp/build-env-wi9mgpyx/lib/python3.10/site-packages/aimrocks"
+            "/tmp/build-env-ncqe1md6/lib/python3.10/site-packages/aimrocks"
         ],
         "name": "aim._core.storage.union",
         "sources": [
             "src/python/aim/_core/storage/union.pyx"
         ]
     },
     "module_name": "aim._core.storage.union"
```

### Comparing `aim-4.0.2/src/python/aim/_core/storage/union.pyx` & `aim-4.0.3/src/python/aim/_core/storage/union.pyx`

 * *Files identical despite different names*

### Comparing `aim-4.0.2/src/python/aim/_core/storage/utils.cpp` & `aim-4.0.3/src/python/aim/_core/storage/utils.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -1,56 +1,56 @@
 /* Generated by Cython 3.0.0a11 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [
-            "/tmp/build-env-wi9mgpyx/lib/python3.10/site-packages/aimrocks/include/rdb_include/comparator_wrapper.hpp",
-            "/tmp/build-env-wi9mgpyx/lib/python3.10/site-packages/aimrocks/include/rdb_include/filter_policy_wrapper.hpp",
-            "/tmp/build-env-wi9mgpyx/lib/python3.10/site-packages/aimrocks/include/rdb_include/memtable_factories.hpp",
-            "/tmp/build-env-wi9mgpyx/lib/python3.10/site-packages/aimrocks/include/rdb_include/merge_operator_wrapper.hpp",
-            "/tmp/build-env-wi9mgpyx/lib/python3.10/site-packages/aimrocks/include/rdb_include/slice_transform_wrapper.hpp",
-            "/tmp/build-env-wi9mgpyx/lib/python3.10/site-packages/aimrocks/include/rdb_include/utils.hpp",
-            "/tmp/build-env-wi9mgpyx/lib/python3.10/site-packages/aimrocks/include/rdb_include/write_batch_iter_helper.hpp",
-            "/tmp/build-env-wi9mgpyx/lib/python3.10/site-packages/aimrocks/include/rocksdb/cache.h",
-            "/tmp/build-env-wi9mgpyx/lib/python3.10/site-packages/aimrocks/include/rocksdb/comparator.h",
-            "/tmp/build-env-wi9mgpyx/lib/python3.10/site-packages/aimrocks/include/rocksdb/db.h",
-            "/tmp/build-env-wi9mgpyx/lib/python3.10/site-packages/aimrocks/include/rocksdb/env.h",
-            "/tmp/build-env-wi9mgpyx/lib/python3.10/site-packages/aimrocks/include/rocksdb/filter_policy.h",
-            "/tmp/build-env-wi9mgpyx/lib/python3.10/site-packages/aimrocks/include/rocksdb/iterator.h",
-            "/tmp/build-env-wi9mgpyx/lib/python3.10/site-packages/aimrocks/include/rocksdb/memtablerep.h",
-            "/tmp/build-env-wi9mgpyx/lib/python3.10/site-packages/aimrocks/include/rocksdb/merge_operator.h",
-            "/tmp/build-env-wi9mgpyx/lib/python3.10/site-packages/aimrocks/include/rocksdb/options.h",
-            "/tmp/build-env-wi9mgpyx/lib/python3.10/site-packages/aimrocks/include/rocksdb/slice.h",
-            "/tmp/build-env-wi9mgpyx/lib/python3.10/site-packages/aimrocks/include/rocksdb/slice_transform.h",
-            "/tmp/build-env-wi9mgpyx/lib/python3.10/site-packages/aimrocks/include/rocksdb/status.h",
-            "/tmp/build-env-wi9mgpyx/lib/python3.10/site-packages/aimrocks/include/rocksdb/table.h",
-            "/tmp/build-env-wi9mgpyx/lib/python3.10/site-packages/aimrocks/include/rocksdb/universal_compaction.h",
-            "/tmp/build-env-wi9mgpyx/lib/python3.10/site-packages/aimrocks/include/rocksdb/utilities/backup_engine.h",
-            "/tmp/build-env-wi9mgpyx/lib/python3.10/site-packages/aimrocks/include/rocksdb/write_batch.h"
+            "/tmp/build-env-ncqe1md6/lib/python3.10/site-packages/aimrocks/include/rdb_include/comparator_wrapper.hpp",
+            "/tmp/build-env-ncqe1md6/lib/python3.10/site-packages/aimrocks/include/rdb_include/filter_policy_wrapper.hpp",
+            "/tmp/build-env-ncqe1md6/lib/python3.10/site-packages/aimrocks/include/rdb_include/memtable_factories.hpp",
+            "/tmp/build-env-ncqe1md6/lib/python3.10/site-packages/aimrocks/include/rdb_include/merge_operator_wrapper.hpp",
+            "/tmp/build-env-ncqe1md6/lib/python3.10/site-packages/aimrocks/include/rdb_include/slice_transform_wrapper.hpp",
+            "/tmp/build-env-ncqe1md6/lib/python3.10/site-packages/aimrocks/include/rdb_include/utils.hpp",
+            "/tmp/build-env-ncqe1md6/lib/python3.10/site-packages/aimrocks/include/rdb_include/write_batch_iter_helper.hpp",
+            "/tmp/build-env-ncqe1md6/lib/python3.10/site-packages/aimrocks/include/rocksdb/cache.h",
+            "/tmp/build-env-ncqe1md6/lib/python3.10/site-packages/aimrocks/include/rocksdb/comparator.h",
+            "/tmp/build-env-ncqe1md6/lib/python3.10/site-packages/aimrocks/include/rocksdb/db.h",
+            "/tmp/build-env-ncqe1md6/lib/python3.10/site-packages/aimrocks/include/rocksdb/env.h",
+            "/tmp/build-env-ncqe1md6/lib/python3.10/site-packages/aimrocks/include/rocksdb/filter_policy.h",
+            "/tmp/build-env-ncqe1md6/lib/python3.10/site-packages/aimrocks/include/rocksdb/iterator.h",
+            "/tmp/build-env-ncqe1md6/lib/python3.10/site-packages/aimrocks/include/rocksdb/memtablerep.h",
+            "/tmp/build-env-ncqe1md6/lib/python3.10/site-packages/aimrocks/include/rocksdb/merge_operator.h",
+            "/tmp/build-env-ncqe1md6/lib/python3.10/site-packages/aimrocks/include/rocksdb/options.h",
+            "/tmp/build-env-ncqe1md6/lib/python3.10/site-packages/aimrocks/include/rocksdb/slice.h",
+            "/tmp/build-env-ncqe1md6/lib/python3.10/site-packages/aimrocks/include/rocksdb/slice_transform.h",
+            "/tmp/build-env-ncqe1md6/lib/python3.10/site-packages/aimrocks/include/rocksdb/status.h",
+            "/tmp/build-env-ncqe1md6/lib/python3.10/site-packages/aimrocks/include/rocksdb/table.h",
+            "/tmp/build-env-ncqe1md6/lib/python3.10/site-packages/aimrocks/include/rocksdb/universal_compaction.h",
+            "/tmp/build-env-ncqe1md6/lib/python3.10/site-packages/aimrocks/include/rocksdb/utilities/backup_engine.h",
+            "/tmp/build-env-ncqe1md6/lib/python3.10/site-packages/aimrocks/include/rocksdb/write_batch.h"
         ],
         "extra_compile_args": [
             "-std=c++11",
             "-O3",
             "-Wall",
             "-Wextra",
             "-Wconversion",
             "-fno-strict-aliasing",
             "-fno-rtti",
             "-fPIC"
         ],
         "include_dirs": [
-            "/tmp/build-env-wi9mgpyx/lib/python3.10/site-packages/aimrocks/include"
+            "/tmp/build-env-ncqe1md6/lib/python3.10/site-packages/aimrocks/include"
         ],
         "language": "c++",
         "libraries": [
             "rocksdb"
         ],
         "library_dirs": [
-            "/tmp/build-env-wi9mgpyx/lib/python3.10/site-packages/aimrocks"
+            "/tmp/build-env-ncqe1md6/lib/python3.10/site-packages/aimrocks"
         ],
         "name": "aim._core.storage.utils",
         "sources": [
             "src/python/aim/_core/storage/utils.py"
         ]
     },
     "module_name": "aim._core.storage.utils"
```

### Comparing `aim-4.0.2/src/python/aim/_core/storage/utils.py` & `aim-4.0.3/src/python/aim/_core/storage/utils.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.2/src/python/aim/_core/utils/deprecation.py` & `aim-4.0.3/src/python/aim/_core/utils/deprecation.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.2/src/python/aim/_ext/notebook/manager.py` & `aim-4.0.3/src/python/aim/_ext/notebook/manager.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.2/src/python/aim/_ext/notebook/notebook.py` & `aim-4.0.3/src/python/aim/_ext/notebook/notebook.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.2/src/python/aim/_ext/notifier/__init__.py` & `aim-4.0.3/src/python/aim/_ext/notifier/__init__.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.2/src/python/aim/_ext/notifier/config.py` & `aim-4.0.3/src/python/aim/_ext/notifier/config.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.2/src/python/aim/_ext/notifier/logging_notifier.py` & `aim-4.0.3/src/python/aim/_ext/notifier/logging_notifier.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.2/src/python/aim/_ext/notifier/notifier.py` & `aim-4.0.3/src/python/aim/_ext/notifier/notifier.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.2/src/python/aim/_ext/notifier/notifier_builder.py` & `aim-4.0.3/src/python/aim/_ext/notifier/notifier_builder.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.2/src/python/aim/_ext/notifier/slack_notifier.py` & `aim-4.0.3/src/python/aim/_ext/notifier/slack_notifier.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.2/src/python/aim/_ext/notifier/utils.py` & `aim-4.0.3/src/python/aim/_ext/notifier/utils.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.2/src/python/aim/_ext/notifier/workplace_notifier.py` & `aim-4.0.3/src/python/aim/_ext/notifier/workplace_notifier.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.2/src/python/aim/_ext/system_info/pynvml.py` & `aim-4.0.3/src/python/aim/_ext/system_info/pynvml.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.2/src/python/aim/_ext/system_info/resource_tracker.py` & `aim-4.0.3/src/python/aim/_ext/system_info/resource_tracker.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.2/src/python/aim/_ext/system_info/stat.py` & `aim-4.0.3/src/python/aim/_ext/system_info/stat.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.2/src/python/aim/_ext/system_info/utils.py` & `aim-4.0.3/src/python/aim/_ext/system_info/utils.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.2/src/python/aim/_ext/tracking/__init__.py` & `aim-4.0.3/src/python/aim/_ext/tracking/__init__.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.2/src/python/aim/_sdk/action.py` & `aim-4.0.3/src/python/aim/_sdk/action.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.2/src/python/aim/_sdk/collections.py` & `aim-4.0.3/src/python/aim/_sdk/collections.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.2/src/python/aim/_sdk/constants.py` & `aim-4.0.3/src/python/aim/_sdk/constants.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.2/src/python/aim/_sdk/container.py` & `aim-4.0.3/src/python/aim/_sdk/container.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,7 +1,15 @@
+"""
+The container module provides implementation of a Container class. Container is a core class, representing a inter-related
+set of properties, parameters, Sequence and Record entities. Specific Container types can be used to collect and store
+data representing a process execution, such as model training, LLM chain execution, etc.
+Container class provides interface for getting and setting it's pre-defined Properties as well as free-form dict-like parameters.
+Container class has an interface for managing sequence objects.
+"""
+
 import logging
 import cachetools.func
 
 from collections import defaultdict
 from typing import Optional, Type, Union, Dict, Callable, Iterator, Tuple, Any
 
 from aim._sdk.interfaces.container import (
@@ -112,14 +120,22 @@
 class Container(ABCContainer):
     version = Property(default='1.0.0')
     creation_time = Property(default=utc_timestamp)
 
     def __init__(self, hash_: Optional[str] = None, *,
                  repo: Optional[Union[str, 'Repo']] = None,
                  mode: Optional[Union[str, ContainerOpenMode]] = ContainerOpenMode.WRITE):
+        """
+        Initializes the Container instance.
+
+        Args:
+            hash_ (str, optional): Unique identifier for the container.
+            repo (Union[str, 'Repo'], optional): Repository path or Repo object.
+            mode (Union[str, ContainerOpenMode], optional): Mode for the container (e.g., "READONLY" or "WRITE"). Defaults to "WRITE".
+        """
         if isinstance(mode, str):
             mode = ContainerOpenMode[mode]
         self.mode = mode
 
         if repo is None:
             from aim._sdk.repo import Repo
             repo = Repo.default()
@@ -172,14 +188,22 @@
 
             self.end_time = None
 
         self._resources = ContainerAutoClean(self)
 
     @classmethod
     def from_storage(cls, storage, meta_tree: 'TreeView', *, hash_: str):
+        """
+        Restores a serialized container instance from given storage and meta tree.
+
+        Args:
+            storage: Storage backend instance.
+            meta_tree ('TreeView'): Tree view of the metadata.
+            hash_ (str): Unique identifier for the container.
+        """
         self = cls.__new__(cls)
         self.mode = ContainerOpenMode.READONLY
         self.storage = storage
         self.hash = hash_
 
         self._resources = None
         self._hash = self._calc_hash()
@@ -189,21 +213,34 @@
         self._meta_tree = meta_tree
 
         self.__storage_init__()
         return self
 
     @classmethod
     def filter(cls, expr: str = '', repo: 'Repo' = None) -> 'ContainerCollection':
+        """
+        Filters the containers based on the given expression and repository.
+
+        Args:
+            expr (str, optional): Query expression for filtering.
+            repo ('Repo', optional): Repository instance. Defaults to the active Repo.
+        """
         if repo is None:
             from aim._sdk.repo import Repo
             repo = Repo.active_repo()
         return repo.containers(query_=expr, type_=cls)
 
     @classmethod
     def find(cls, hash_: str) -> Optional['Container']:
+        """
+        Finds and returns a container instance based on the given hash.
+
+        Args:
+            hash_ (str): Unique identifier for the container.
+        """
         from aim._sdk.repo import Repo
         repo = Repo.active_repo()
         try:
             return cls(hash_, repo=repo, mode='READONLY')
         except MissingContainerError:
             return None
 
@@ -227,72 +264,126 @@
     def _sequence_data_tree(self) -> 'TreeView':
         if self.__sequence_data_tree is None:
             self.__sequence_data_tree = self.storage.tree(
                 self.hash, 'seqs', read_only=self._is_readonly).subtree('chunks').subtree(self.hash)
         return self.__sequence_data_tree
 
     def __setitem__(self, key, value):
+        """
+        Sets a value in the container for a given key.
+
+        Args:
+            key: Key to set the value for.
+            value: Value to be set.
+        """
         self._attrs_tree[key] = value
         self._meta_attrs_tree.merge(key, value)
 
     def set(self, key, value, strict: bool):
+        """
+        Sets a value in the container for a given key with optional strictness.
+
+        Args:
+            key: Key to set the value for.
+            value: Value to be set.
+            strict (bool): Whether to enforce strict setting.
+        """
         self._attrs_tree.set(key, value, strict)
         self._meta_attrs_tree.set(key, value, strict)
 
     def __getitem__(self, key):
-        return self._attrs_tree.collect(key, strict=True)
+        """
+        Retrieves a value from the container based on the given key.
 
-    def __delitem__(self, key):
-        del self._attrs_tree[key]
+        Args:
+            key: Key for which value is to be retrieved.
+        """
+        return self._attrs_tree.collect(key, strict=True)
 
     def get(self, key, default: Any = None, strict: bool = False):
+        """
+        Retrieves a value from the container based on the key or returns a default value.
+
+        Args:
+            key: Key for which value is to be retrieved.
+            default (optional): Default value to return if key doesn't exist.
+            strict (bool, optional): Whether to enforce strict retrieval.
+        """
         try:
             return self._attrs_tree.collect(key, strict=strict)
         except KeyError:
             return default
 
+    def __delitem__(self, key):
+        """
+        Deletes a value in the container based on the given key.
+
+        Args:
+            key: Key for which the value is to be deleted.
+        """
+        del self._attrs_tree[key]
+
     def _set_property(self, name: str, value: Any):
         self._props_tree[name] = value
         self._meta_props_tree.merge(name, value)
 
     def _get_property(self, name: str, default: Any = None) -> Any:
         return self._props_tree.get(name, default)
 
     def collect_properties(self) -> Dict:
+        """
+        Collects and returns all properties associated with the container as a dictionary object.
+        """
         try:
             return self._props_tree.collect()
         except KeyError:
             return {}
 
     def get_logged_typename(self) -> str:
+        """
+        Returns the typename of the logged data in the container.
+        """
         return self._tree[KeyNames.INFO_PREFIX, KeyNames.CONTAINER_TYPE]
 
     def match(self, expr) -> bool:
+        """
+        Checks if the container matches the given expression.
+        """
         query = RestrictedPythonQuery(expr)
         query_cache = {}
         return self._check(query, query_cache)
 
     def _check(self, query, query_cache, *, aliases=()) -> bool:
         proxy = ContainerQueryProxy(self.hash, self._tree, query_cache)
 
         if isinstance(aliases, str):
             aliases = (aliases,)
         alias_names = self.default_aliases.union(aliases)
         query_params = {p: proxy for p in alias_names}
         return query.check(**query_params)
 
     def delete_sequence(self, name, context=None):
+        """
+        Deletes a sequence from the container based on the given name and context.
+
+        Args:
+            name: Name of the sequence to delete.
+            context (optional): Contextual information for the sequence. `{}` if not specified.
+        """
         if self._is_readonly:
             raise RuntimeError('Cannot delete sequence in read-only mode.')
 
         context = {} if context is None else context
         sequence = self._sequence_map._sequence(name, context)
         sequence.delete()
 
     def delete(self):
+        """
+        Deletes the container and its associated data.
+        """
         if self._is_readonly:
             raise RuntimeError('Cannot delete container in read-only mode.')
 
         # remove container meta tree
         meta_tree = self.storage.tree(self.hash, 'meta', read_only=False)
         del meta_tree.subtree('chunks')[self.hash]
         # remove container sequence tree
@@ -311,14 +402,17 @@
         self._state['deleted'] = True
 
         # close the container
         self.close()
 
     @property
     def sequences(self) -> 'ContainerSequenceMap':
+        """
+        Returns a map of sequences associated with the container.
+        """
         return self._sequence_map
 
     # TODO [AT]: Implement end_time as a Property similar to other pre-defined props
     @property
     def end_time(self):
         return self._get_property('end_time')
 
@@ -332,14 +426,17 @@
     def __hash__(self) -> int:
         return self._hash
 
     def _calc_hash(self):
         return hash_auto((self.hash, hash(self.storage.url), str(self.mode)))
 
     def close(self):
+        """
+        Closes the container and releases any associated resources.
+        """
         self._resources._close()
 
     @staticmethod
     def _init_properties(cls: Type['Container'], inst: 'Container'):
         if cls != Container:
             for base_cls in cls.__bases__:
                 if issubclass(base_cls, Container):
@@ -356,15 +453,25 @@
         self._sequence_tree: 'TreeView' = container._tree.subtree(KeyNames.SEQUENCES)
         self._data_loader: Callable[[], 'TreeView'] = container._data_loader
 
     def __call__(self,
                  query_: Optional[str] = None,
                  type_: Union[str, Type[Sequence]] = Sequence,
                  **kwargs) -> SequenceCollection:
+        """
+        Retrieves a sequence collection based on a query expression.
+
+        Args:
+            query_ (str, optional): Query expression for filtering.
+            type_ (Union[str, Type[Sequence]]): Sequence type or type name. Defaults to Sequence.
+            **kwargs: Additional keyword arguments.
 
+        Returns:
+            SequenceCollection: The filtered sequence collection.
+        """
         query_context = {
             'storage': self._container.storage,
             'var_name': None,
             'meta_tree': self._container._meta_tree,
             'query_cache': defaultdict(dict),
             KeyNames.ALLOWED_VALUE_TYPES: type_utils.get_sequence_value_types(type_),
             KeyNames.SEQUENCE_TYPE: type_,
@@ -372,48 +479,91 @@
         }
 
         q = construct_query_expression('container', query_, **kwargs)
         seq_collection = ContainerSequenceCollection(self._container.hash, query_context)
         return seq_collection.filter(q) if q else seq_collection
 
     def __iter__(self) -> Iterator[Sequence]:
+        """
+        Returns an iterator over the sequences.
+
+        Yields:
+            Sequence: The next sequence in the container.
+        """
         for ctx_idx in self._sequence_tree.keys():
             for name in self._sequence_tree.subtree(ctx_idx).keys():
                 yield self._sequence_cls(self._container, name=name, context=ctx_idx)
 
     def __getitem__(self, item: Union[str, Tuple[str, Dict]]) -> Sequence:
+        """
+        Retrieves a sequence based on the given item (name or tuple of name and context).
+
+        Args:
+            item (Union[str, Tuple[str, Dict]]): Name of the sequence or a tuple of name and context.
+
+        Returns:
+            Sequence: The retrieved sequence.
+        """
         if isinstance(item, str):
             name = item
             context = {}
         else:
             assert isinstance(item, tuple)
             name = item[0]
             context = {} if item[1] is None else item[1]
 
         return self._sequence(name, Context(context))
 
     def typed_sequence(self, sequence_type: Type[Sequence], name: str, context: Dict):
+        """
+        Retrieves a sequence of specified type based on the given name and context.
+
+        Args:
+            sequence_type (Type[Sequence]): The desired sequence type.
+            name (str): Name of the sequence.
+            context (Dict): Contextual information for the sequence.
+
+        Returns:
+            Sequence: The sequence instance.
+        """
         return self._sequence(name, Context(context), sequence_type=sequence_type)
 
     @cachetools.func.ttl_cache()
     def _sequence(self, name: str, context: Context, *, sequence_type: Optional[Type[Sequence]] = None) -> Sequence:
+        """
+        Retrieves or creates a sequence based on the name, context, and optional type.
+
+        Args:
+            name (str): Name of the sequence.
+            context (Context): Contextual information for the sequence.
+            sequence_type (Type[Sequence], optional): Desired sequence type. Defaults to self._sequence_cls.
+
+        Returns:
+            Sequence: The sequence instance.
+        """
         ctx_idx = context.idx
         try:
             self._sequence_tree.subtree((ctx_idx, name)).last_key()
             exists = True
         except KeyError:
             exists = False
 
         if self._container._is_readonly and not exists:
             raise ValueError('Cannot create sequence from a readonly container.')
 
         seq_cls = sequence_type or self._sequence_cls
         return seq_cls(self._container, name=name, context=context)
 
     def __delitem__(self, item: Union[str, Tuple[str, Dict]]):
+        """
+        Deletes a sequence based on the given item (name or tuple of name and context).
+
+        Args:
+            item (Union[str, Tuple[str, Dict]]): Name of the sequence or a tuple of name and context.
+        """
         if self._container._is_readonly:
             raise ValueError('Cannot delete sequence from a readonly container.')
 
         if isinstance(item, str):
             name = item
             context = {}
         else:
```

### Comparing `aim-4.0.2/src/python/aim/_sdk/context.py` & `aim-4.0.3/src/python/aim/_sdk/context.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.2/src/python/aim/_sdk/dev_package.py` & `aim-4.0.3/src/python/aim/_sdk/dev_package.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.2/src/python/aim/_sdk/exceptions.py` & `aim-4.0.3/src/python/aim/_sdk/exceptions.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.2/src/python/aim/_sdk/interfaces/container.py` & `aim-4.0.3/src/python/aim/_sdk/interfaces/container.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.2/src/python/aim/_sdk/interfaces/sequence.py` & `aim-4.0.3/src/python/aim/_sdk/interfaces/sequence.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.2/src/python/aim/_sdk/local_storage.py` & `aim-4.0.3/src/python/aim/_sdk/local_storage.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.2/src/python/aim/_sdk/lock_manager.py` & `aim-4.0.3/src/python/aim/_sdk/lock_manager.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.2/src/python/aim/_sdk/num_utils.py` & `aim-4.0.3/src/python/aim/_sdk/num_utils.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.2/src/python/aim/_sdk/package_utils.py` & `aim-4.0.3/src/python/aim/_sdk/package_utils.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.2/src/python/aim/_sdk/query.py` & `aim-4.0.3/src/python/aim/_sdk/query.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.2/src/python/aim/_sdk/query_utils.py` & `aim-4.0.3/src/python/aim/_sdk/query_utils.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.2/src/python/aim/_sdk/record.py` & `aim-4.0.3/src/python/aim/_sdk/record.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.2/src/python/aim/_sdk/remote_storage.py` & `aim-4.0.3/src/python/aim/_sdk/remote_storage.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.2/src/python/aim/_sdk/repo.py` & `aim-4.0.3/src/python/aim/_sdk/repo.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,7 +1,14 @@
+"""
+The repo module contains implementation of class Repo; a core class for accessing the data logged in Aim.
+It provides interfaces for creating and managing Aim repositories, for both local and remote setups.
+Repo class can be used to query stored Containers and Sequences, as well as get the metadata about logs, such as
+registered types, actions, packages, summary of logged types, etc.
+"""
+
 import logging
 import os
 import shutil
 
 from collections import defaultdict
 from typing import Union, Type, List, Dict, Optional, Tuple
 from weakref import WeakValueDictionary
@@ -24,22 +31,41 @@
 
 from aim._ext.system_info.resource_tracker import ResourceTracker
 
 logger = logging.getLogger(__name__)
 
 
 class Repo(object):
+    """
+    Represents an Aim repository, handling both local and remote repositories.
+    """
+
     _pool: Dict[str, 'Repo'] = WeakValueDictionary()
 
     @staticmethod
     def is_remote_path(path: str) -> bool:
+        """
+        Determines if the provided path refers to a remote repository.
+
+        Args:
+            path (str): The path to be checked.
+
+        Returns:
+            bool: True if the path is remote, otherwise False.
+        """
         return path.startswith('aim://')
 
     @classmethod
     def default(cls) -> 'Repo':
+        """
+        Retrieves the default repository instance.
+
+        Returns:
+            Repo: Default repository instance.
+        """
         return cls.from_path('aim://127.0.0.1:53800')
 
     @classmethod
     def from_path(cls, path: str, read_only: bool = True) -> 'Repo':
         """Named constructor for Repo for given path.
 
         Arguments:
@@ -56,35 +82,105 @@
         if repo is None:
             repo = cls(path, read_only=read_only)
             cls._pool[path] = repo
         return repo
 
     @classmethod
     def get_version(cls, path: str) -> Optional[Tuple[int, ...]]:
+        """
+        Retrieves the version of the Aim repository at the given path.
+
+        Args:
+            path (str): The repository path.
+
+        Returns:
+            Optional[Tuple[int, ...]]: Version tuple if the path refers to a valid Aim repository, otherwise None.
+        """
         if cls.is_remote_path(path):
             return None
         path = clean_repo_path(path)
         version_file_path = os.path.join(path, get_aim_repo_name(), 'VERSION')
         if os.path.exists(version_file_path):
             with open(version_file_path, 'r') as version_fh:
                 version_tp = version_fh.read().strip().split('.')
                 return tuple(map(int, version_tp))
         return None
 
     @classmethod
     def active_repo(cls) -> 'Repo':
+        """
+        Retrieves the currently active repository.
+
+        Returns:
+            Repo: The active repository instance.
+
+        Raises:
+            ValueError: If it's not possible to determine the active repository.
+        """
         if len(cls._pool) == 0:
             return cls.default()
         elif len(cls._pool) == 1:
             path = next(cls._pool.keys())
             return cls._pool[path]
         else:
             raise ValueError('Cannot determine active Repo. Please use Repo.from_path() instead.')
 
+    @classmethod
+    def exists(cls, path: str) -> bool:
+        """
+        Checks if an Aim repository exists at the given path.
+
+        Args:
+            path (str): The path to check.
+
+        Returns:
+            bool: True if the Aim repository exists, otherwise False.
+        """
+        aim_repo_path = os.path.join(clean_repo_path(path), get_aim_repo_name())
+        return os.path.exists(aim_repo_path)
+
+    @classmethod
+    def init(cls, path: str):
+        """
+        Initializes a new Aim repository at the given path.
+
+        Args:
+            path (str): Path where the Aim repository should be created.
+
+        Returns:
+            Repo: The newly initialized repository instance.
+        """
+        aim_repo_path = os.path.join(clean_repo_path(path), get_aim_repo_name())
+        os.makedirs(aim_repo_path, exist_ok=True)
+
+        version_file_path = os.path.join(aim_repo_path, 'VERSION')
+        with open(version_file_path, 'w') as version_fh:
+            version_fh.write('.'.join(map(str, get_data_version())) + '\n')
+
+        return cls.from_path(aim_repo_path, read_only=False)
+
+    @classmethod
+    def rm(cls, path: str):
+        """
+        Deletes an Aim repository at the given path.
+
+        Args:
+            path (str): The path to the Aim repository to be deleted.
+        """
+        aim_repo_path = os.path.join(clean_repo_path(path), get_aim_repo_name())
+        shutil.rmtree(aim_repo_path)
+
     def __init__(self, path: str, *, read_only: Optional[bool] = True):
+        """
+        Initializes a repository instance.
+
+        Args:
+            path (str): Path to the Aim repository.
+            read_only (bool, optional): If True, opens the repo in read-only mode. Default is True.
+        """
         self.read_only = read_only
         self._is_remote_repo = False
         if self.is_remote_path(path):
             self.path = os.path.join(path, get_aim_repo_name())
             self._is_remote_repo = True
             self._storage_engine = RemoteStorage(path)
             self._remote_repo_proxy = RemoteRepoProxy(self._storage_engine._client)
@@ -102,50 +198,37 @@
 
     def __repr__(self) -> str:
         return f'<Repo#{hash(self)} path={self.path} read_only={self.read_only}>'
 
     def __hash__(self) -> int:
         return hash(self.path)
 
-    @classmethod
-    def exists(cls, path: str) -> bool:
-        aim_repo_path = os.path.join(clean_repo_path(path), get_aim_repo_name())
-        return os.path.exists(aim_repo_path)
-
-    @classmethod
-    def init(cls, path: str):
-        aim_repo_path = os.path.join(clean_repo_path(path), get_aim_repo_name())
-        os.makedirs(aim_repo_path, exist_ok=True)
-
-        version_file_path = os.path.join(aim_repo_path, 'VERSION')
-        with open(version_file_path, 'w') as version_fh:
-            version_fh.write('.'.join(map(str, get_data_version())) + '\n')
-
-        return cls.from_path(aim_repo_path, read_only=False)
-
-    @classmethod
-    def rm(cls, path: str):
-        aim_repo_path = os.path.join(clean_repo_path(path), get_aim_repo_name())
-        shutil.rmtree(aim_repo_path)
-
     @property
     def storage_engine(self) -> StorageEngine:
+        """
+        Returns the storage engine associated with the repository.
+
+        Returns:
+            StorageEngine: The storage engine instance.
+        """
         return self._storage_engine
 
     @property
     def resource_tracker(self) -> ResourceTracker:
+        """
+        Returns the resource tracker associated with the repository.
+
+        Returns:
+            ResourceTracker: The resource tracker instance.
+        """
         if self._system_tracker is None:
             self._system_tracker = ResourceTracker()
         return self._system_tracker
 
     @property
-    def container_hashes(self):
-        return list(self._meta_tree.subtree('chunks').keys())
-
-    @property
     def dev_package_dir(self) -> str:
         dev_package_dir_path = os.path.join(self.path, 'pkgs')
         if not os.path.exists(dev_package_dir_path):
             os.mkdir(dev_package_dir_path)
         return dev_package_dir_path
 
     @property
@@ -165,55 +248,129 @@
                 encryption_key = key_fp.readline()
 
         self._encryption_key = encryption_key
 
         return encryption_key
 
     def tracked_container_types(self) -> List[str]:
+        """
+        Lists all container types being tracked in the repository.
+
+        Returns:
+            List[str]: List of tracked container types.
+        """
         return list(self._meta_tree.subtree(KeyNames.CONTAINERS).keys())
 
     def tracked_sequence_types(self) -> List[str]:
+        """
+        Lists all sequence types being tracked in the repository.
+
+        Returns:
+            List[str]: List of tracked sequence types.
+        """
         return list(self._meta_tree.subtree(KeyNames.SEQUENCES).keys())
 
     def tracked_sequence_infos(self, sequence_type: str) -> Dict[str, List]:
+        """
+        Retrieves information for a specific sequence type.
+
+        Args:
+            sequence_type (str): The sequence type to retrieve information for.
+
+        Returns:
+            Dict[str, List]: Dictionary of tracked sequence names/contexts.
+        """
         if sequence_type not in Sequence.registry:
             raise ValueError(f'Unknown sequence type \'{sequence_type}\'.')
         try:
             infos = self._meta_tree[KeyNames.SEQUENCES, sequence_type]
         except KeyError:
             return {}
         seq_infos = defaultdict(list)
         for ctx_idx, names in infos.items():
             context_dict = self._meta_tree[KeyNames.CONTEXTS, ctx_idx]
             for seq_name in names.keys():
                 seq_infos[seq_name].append(context_dict)
         return seq_infos
 
     def tracked_params(self) -> Dict:
+        """
+        Retrieves all tracked parameters for the repository.
+
+        Returns:
+            Dict: Dictionary of tracked parameters.
+        """
         try:
             return self._meta_tree.collect('attrs', strict=False)
         except KeyError:
             return {}
 
     def registered_container_types(self) -> List[str]:
+        """
+        Lists all registered container types in the repository.
+
+        Returns:
+            List[str]: List of registered container types.
+        """
         return list(Container.registry.keys())
 
     def registered_sequence_types(self) -> List[str]:
+        """
+        Lists all registered sequence types in the repository.
+
+        Returns:
+            List[str]: List of registered sequence types.
+        """
         return list(Sequence.registry.keys())
 
     def registered_actions(self) -> List[str]:
+        """
+        Lists all registered actions in the repository.
+
+        Returns:
+            List[str]: List of registered actions.
+        """
         return list(Action.registry.keys())
 
+    @property
+    def container_hashes(self):
+        """
+        Retrieves a list of hashes for all tracked containers.
+
+        Returs:
+            List[str]: List of container hashes.
+        """
+        return list(self._meta_tree.subtree('chunks').keys())
+
     def get_container(self, hash_) -> Container:
+        """
+        Retrieves a container from the repository based on its hash.
+
+        Args:
+            hash_ (str): The hash of the container to retrieve.
+
+        Returns:
+            Container: The corresponding container object.
+        """
         return Container(hash_, repo=self, mode='READONLY')
 
     def containers(self,
                    query_: Optional[str] = None,
                    type_: Union[str, Type[Container]] = Container,
                    **kwargs) -> ContainerCollection:
+        """
+        Retrieves a collection of containers based on the query expression and type.
+
+        Args:
+            query_ (Optional[str]): The query string to filter containers.
+            type_ (Union[str, Type[Container]]): The type of containers to retrieve.
+
+        Returns:
+            ContainerCollection: The resulting collection of containers.
+        """
         q = construct_query_expression('container', query_, **kwargs)
 
         if isinstance(type_, str):
             cont_types = Container.registry.get(type_)
             if len(cont_types) > 1:
                 raise ValueError(f'Multiple matching container types for type name \'{type_}\'. '
                                  f'Please include container package name.')
@@ -221,25 +378,102 @@
 
         return self._select(type_).filter(q) if q else self._select(type_)
 
     def sequences(self,
                   query_: Optional[str] = None,
                   type_: Union[str, Type[Sequence]] = Sequence,
                   **kwargs) -> SequenceCollection:
+        """
+        Retrieves a collection of sequences based on the query expression and type.
+
+        Args:
+            query_ (Optional[str]): The query string to filter sequences.
+            type_ (Union[str, Type[Sequence]]): The type of sequences to retrieve.
+
+        Returns:
+            SequenceCollection: The resulting collection of sequences.
+        """
         q = construct_query_expression('sequence', query_, **kwargs)
 
         if isinstance(type_, str):
             seq_types = Sequence.registry.get(type_)
             if len(seq_types) > 1:
                 raise ValueError(f'Multiple matching sequence types for type name \'{type_}\'. '
                                  f'Please include sequence package name.')
             type_ = seq_types[0]
 
         return self._select(type_).filter(q) if q else self._select(type_)
 
+    def add_package(self, pkg_name: str) -> bool:
+        """
+        Adds a package to the repository.
+
+        Args:
+            pkg_name (str): The name of the package to be added.
+
+        Returns:
+            bool: True if the package was added successfully, False if it already exists.
+        """
+        if self._is_remote_repo:
+            return self._remote_repo_proxy.add_package(pkg_name)
+        active_pkg_file = os.path.join(self.path, 'active_pkg')
+        with open(active_pkg_file, 'a+') as apf:
+            apf.seek(0)
+            packages = set(line.strip() for line in apf.readlines())
+            if pkg_name in packages:
+                return False
+            packages.add(pkg_name)
+            apf.seek(0)
+            apf.truncate()
+            for package in packages:
+                apf.write(f"{package}\n")
+        return True
+
+    def remove_package(self, pkg_name: str) -> bool:
+        """
+        Removes a package from the repository.
+
+        Args:
+            pkg_name (str): The name of the package to be removed.
+
+        Returns:
+            bool: True if the package was removed successfully, False if it doesn't exist.
+        """
+        if self._is_remote_repo:
+            return self._remote_repo_proxy.remove_package(pkg_name)
+        active_pkg_file = os.path.join(self.path, 'active_pkg')
+        with open(active_pkg_file, 'a+') as apf:
+            apf.seek(0)
+            packages = set(line.strip() for line in apf.readlines())
+            if pkg_name not in packages:
+                return False
+            packages.remove(pkg_name)
+            apf.seek(0)
+            apf.truncate()
+            for package in packages:
+                apf.write(f"{package}\n")
+        return True
+
+    def load_active_packages(self):
+        """
+        Loads all active packages in the repository. Only applicable for local repositories.
+
+        Note:
+            This method doesn't return any value but has side effects on the state of loaded packages.
+        """
+        if self._is_remote_repo:
+            return
+        from aim._sdk.package_utils import Package
+        active_pkg_file = os.path.join(self.path, 'active_pkg')
+        if os.path.exists(active_pkg_file):
+            pkgs_dir = os.path.join(self.path, 'pkgs')
+            with open(active_pkg_file, 'r') as apf:
+                for pkg_name in apf.read().split():
+                    Package.load_package(pkg_name, pkgs_dir)
+
     def _select(self, type_: Type = None, **kwargs):
         if type_ is None:
             assert len(kwargs) == 1
             (var_name, type_) = kwargs.popitem()
         else:
             assert len(kwargs) == 0
             var_name = None
@@ -269,15 +503,15 @@
                 KeyNames.SEQUENCE_TYPE: type_,
                 'required_typename': type_.get_full_typename(),
             })
             # return SequenceCollection[type_](query_context=query_context)
             return SequenceCollection(query_context=query_context)
 
     def delete_containers(self, container_hashes: List[str]) -> Tuple[bool, List[str]]:
-        """Delete multiple Containers data from aim repository
+        """Deletes multiple Containers data from aim repository
 
         This action removes containers data permanently and cannot be reverted.
         If you want to archive container but keep it's data use `repo.get_container(container_hash).archived = True`.
 
         Args:
             container_hashes (:obj:`str`): list of Containers to be deleted.
 
@@ -453,57 +687,14 @@
             tree(-1, 'meta', read_only=False).\
             subtree('chunks').subtree(container_hash)
         if not container_meta_tree.get((KeyNames.INFO_PREFIX, 'end_time')):
             container_meta_tree[(KeyNames.INFO_PREFIX, 'end_time')] = utc_timestamp()
 
     def prune(self):
         """
-        Utility function to remove dangling/orphan params/sequences with no referring containers.
+        Removes dangling/orphan params/sequences with no referring containers.
         """
         from aim._sdk.utils import prune
         if self._is_remote_repo:
             return self._remote_repo_proxy.prune()
 
         prune(self)
-
-    def add_package(self, pkg_name: str) -> bool:
-        if self._is_remote_repo:
-            return self._remote_repo_proxy.add_package(pkg_name)
-        active_pkg_file = os.path.join(self.path, 'active_pkg')
-        with open(active_pkg_file, 'a+') as apf:
-            apf.seek(0)
-            packages = set(line.strip() for line in apf.readlines())
-            if pkg_name in packages:
-                return False
-            packages.add(pkg_name)
-            apf.seek(0)
-            apf.truncate()
-            for package in packages:
-                apf.write(f"{package}\n")
-        return True
-
-    def remove_package(self, pkg_name: str) -> bool:
-        if self._is_remote_repo:
-            return self._remote_repo_proxy.remove_package(pkg_name)
-        active_pkg_file = os.path.join(self.path, 'active_pkg')
-        with open(active_pkg_file, 'a+') as apf:
-            apf.seek(0)
-            packages = set(line.strip() for line in apf.readlines())
-            if pkg_name not in packages:
-                return False
-            packages.remove(pkg_name)
-            apf.seek(0)
-            apf.truncate()
-            for package in packages:
-                apf.write(f"{package}\n")
-        return True
-
-    def load_active_packages(self):
-        if self._is_remote_repo:
-            return
-        from aim._sdk.package_utils import Package
-        active_pkg_file = os.path.join(self.path, 'active_pkg')
-        if os.path.exists(active_pkg_file):
-            pkgs_dir = os.path.join(self.path, 'pkgs')
-            with open(active_pkg_file, 'r') as apf:
-                for pkg_name in apf.read().split():
-                    Package.load_package(pkg_name, pkgs_dir)
```

### Comparing `aim-4.0.2/src/python/aim/_sdk/storage_engine.py` & `aim-4.0.3/src/python/aim/_sdk/storage_engine.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.2/src/python/aim/_sdk/type_utils.py` & `aim-4.0.3/src/python/aim/_sdk/type_utils.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.2/src/python/aim/_sdk/uri_service.py` & `aim-4.0.3/src/python/aim/_sdk/uri_service.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.2/src/python/aim/_sdk/utils.py` & `aim-4.0.3/src/python/aim/_sdk/utils.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.2/src/python/aim/utils.py` & `aim-4.0.3/src/python/aim/utils.py`

 * *Files identical despite different names*

