# Comparing `tmp/StonerPlots-1.3.0.tar.gz` & `tmp/StonerPlots-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "StonerPlots-1.3.0.tar", last modified: Sun Mar 31 22:38:34 2024, max compression
+gzip compressed data, was "StonerPlots-1.3.1.tar", last modified: Mon Apr  1 20:53:14 2024, max compression
```

## Comparing `StonerPlots-1.3.0.tar` & `StonerPlots-1.3.1.tar`

### file list

```diff
@@ -1,152 +1,163 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 22:38:34.813457 StonerPlots-1.3.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 22:38:34.789457 StonerPlots-1.3.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 22:38:34.793457 StonerPlots-1.3.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1656 2024-03-31 22:35:17.000000 StonerPlots-1.3.0/.github/workflows/build_conda.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      396 2024-03-31 22:35:17.000000 StonerPlots-1.3.0/.github/workflows/publish_sphinx.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3200 2024-03-31 22:35:17.000000 StonerPlots-1.3.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      198 2024-03-31 22:35:17.000000 StonerPlots-1.3.0/CHANGES.md
--rw-r--r--   0 runner    (1001) docker     (127)     1153 2024-03-31 22:35:17.000000 StonerPlots-1.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-03-31 22:35:17.000000 StonerPlots-1.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     5084 2024-03-31 22:38:34.813457 StonerPlots-1.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4392 2024-03-31 22:35:17.000000 StonerPlots-1.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 22:38:34.793457 StonerPlots-1.3.0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      638 2024-03-31 22:35:17.000000 StonerPlots-1.3.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      769 2024-03-31 22:35:17.000000 StonerPlots-1.3.0/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-03-31 22:35:17.000000 StonerPlots-1.3.0/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 22:38:34.793457 StonerPlots-1.3.0/docs/source/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 22:38:34.793457 StonerPlots-1.3.0/docs/source/api/
--rw-r--r--   0 runner    (1001) docker     (127)      258 2024-03-31 22:35:17.000000 StonerPlots-1.3.0/docs/source/api/stonerplots.InsetPlot.rst
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-03-31 22:35:17.000000 StonerPlots-1.3.0/docs/source/api/stonerplots.SavedFigure.rst
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-03-31 22:35:17.000000 StonerPlots-1.3.0/docs/source/api/stonerplots.StackVertical.rst
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-03-31 22:35:17.000000 StonerPlots-1.3.0/docs/source/api.rst
--rw-r--r--   0 runner    (1001) docker     (127)      912 2024-03-31 22:35:17.000000 StonerPlots-1.3.0/docs/source/colours.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1630 2024-03-31 22:35:17.000000 StonerPlots-1.3.0/docs/source/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 22:38:34.797457 StonerPlots-1.3.0/docs/source/figures/
--rw-r--r--   0 runner    (1001) docker     (127)    25332 2024-03-31 22:35:17.000000 StonerPlots-1.3.0/docs/source/figures/StonerLogo2.png
--rw-r--r--   0 runner    (1001) docker     (127)    31938 2024-03-31 22:35:17.000000 StonerPlots-1.3.0/docs/source/figures/colours.png
--rw-r--r--   0 runner    (1001) docker     (127)    23528 2024-03-31 22:35:17.000000 StonerPlots-1.3.0/docs/source/figures/colours10.png
--rw-r--r--   0 runner    (1001) docker     (127)    21940 2024-03-31 22:35:17.000000 StonerPlots-1.3.0/docs/source/figures/colours50.png
--rw-r--r--   0 runner    (1001) docker     (127)    21393 2024-03-31 22:35:17.000000 StonerPlots-1.3.0/docs/source/figures/colours70.png
--rw-r--r--   0 runner    (1001) docker     (127)    22543 2024-03-31 22:35:17.000000 StonerPlots-1.3.0/docs/source/figures/colours90.png
--rw-r--r--   0 runner    (1001) docker     (127)    47643 2024-03-31 22:35:17.000000 StonerPlots-1.3.0/docs/source/figures/example-1.png
--rw-r--r--   0 runner    (1001) docker     (127)     2195 2024-03-31 22:35:17.000000 StonerPlots-1.3.0/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)    13441 2024-03-31 22:35:17.000000 StonerPlots-1.3.0/docs/source/style-gallery.rst
--rw-r--r--   0 runner    (1001) docker     (127)    16575 2024-03-31 22:35:17.000000 StonerPlots-1.3.0/docs/source/userguide.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 22:38:34.797457 StonerPlots-1.3.0/examples/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 22:38:34.801457 StonerPlots-1.3.0/examples/figures/
--rw-r--r--   0 runner    (1001) docker     (127)    29763 2024-03-31 22:35:17.000000 StonerPlots-1.3.0/examples/figures/fig01a.png
--rw-r--r--   0 runner    (1001) docker     (127)    26194 2024-03-31 22:35:17.000000 StonerPlots-1.3.0/examples/figures/fig01b.png
--rw-r--r--   0 runner    (1001) docker     (127)    24459 2024-03-31 22:35:17.000000 StonerPlots-1.3.0/examples/figures/fig02a.png
--rw-r--r--   0 runner    (1001) docker     (127)    17925 2024-03-31 22:35:17.000000 StonerPlots-1.3.0/examples/figures/fig02b.pdf
--rw-r--r--   0 runner    (1001) docker     (127)    27629 2024-03-31 22:35:17.000000 StonerPlots-1.3.0/examples/figures/fig02b.png
--rw-r--r--   0 runner    (1001) docker     (127)    26406 2024-03-31 22:35:17.000000 StonerPlots-1.3.0/examples/figures/fig02c.png
--rw-r--r--   0 runner    (1001) docker     (127)    26371 2024-03-31 22:35:17.000000 StonerPlots-1.3.0/examples/figures/fig02d.png
--rw-r--r--   0 runner    (1001) docker     (127)    25087 2024-03-31 22:35:17.000000 StonerPlots-1.3.0/examples/figures/fig02e.png
--rw-r--r--   0 runner    (1001) docker     (127)    37979 2024-03-31 22:35:17.000000 StonerPlots-1.3.0/examples/figures/fig02f.png
--rw-r--r--   0 runner    (1001) docker     (127)    51713 2024-03-31 22:35:17.000000 StonerPlots-1.3.0/examples/figures/fig02g.png
--rw-r--r--   0 runner    (1001) docker     (127)    27613 2024-03-31 22:35:17.000000 StonerPlots-1.3.0/examples/figures/fig03.png
--rw-r--r--   0 runner    (1001) docker     (127)    28761 2024-03-31 22:35:17.000000 StonerPlots-1.3.0/examples/figures/fig04a.png
--rw-r--r--   0 runner    (1001) docker     (127)    29370 2024-03-31 22:35:17.000000 StonerPlots-1.3.0/examples/figures/fig04b.png
--rw-r--r--   0 runner    (1001) docker     (127)    29396 2024-03-31 22:35:17.000000 StonerPlots-1.3.0/examples/figures/fig04c.png
--rw-r--r--   0 runner    (1001) docker     (127)    28832 2024-03-31 22:35:17.000000 StonerPlots-1.3.0/examples/figures/fig04d.png
--rw-r--r--   0 runner    (1001) docker     (127)    27732 2024-03-31 22:35:17.000000 StonerPlots-1.3.0/examples/figures/fig04e.png
--rw-r--r--   0 runner    (1001) docker     (127)    29246 2024-03-31 22:35:17.000000 StonerPlots-1.3.0/examples/figures/fig04f.png
--rw-r--r--   0 runner    (1001) docker     (127)    28862 2024-03-31 22:35:17.000000 StonerPlots-1.3.0/examples/figures/fig04g.png
--rw-r--r--   0 runner    (1001) docker     (127)    29207 2024-03-31 22:35:17.000000 StonerPlots-1.3.0/examples/figures/fig04h.png
--rw-r--r--   0 runner    (1001) docker     (127)    29145 2024-03-31 22:35:17.000000 StonerPlots-1.3.0/examples/figures/fig04i.png
--rw-r--r--   0 runner    (1001) docker     (127)    80367 2024-03-31 22:35:17.000000 StonerPlots-1.3.0/examples/figures/fig05a.png
--rw-r--r--   0 runner    (1001) docker     (127)    86165 2024-03-31 22:35:17.000000 StonerPlots-1.3.0/examples/figures/fig05b.png
--rw-r--r--   0 runner    (1001) docker     (127)   166258 2024-03-31 22:35:17.000000 StonerPlots-1.3.0/examples/figures/fig05c.png
--rw-r--r--   0 runner    (1001) docker     (127)   140055 2024-03-31 22:35:17.000000 StonerPlots-1.3.0/examples/figures/fig05d.png
--rw-r--r--   0 runner    (1001) docker     (127)   134163 2024-03-31 22:35:17.000000 StonerPlots-1.3.0/examples/figures/fig05e.png
--rw-r--r--   0 runner    (1001) docker     (127)   211090 2024-03-31 22:35:17.000000 StonerPlots-1.3.0/examples/figures/fig05f.png
--rw-r--r--   0 runner    (1001) docker     (127)    36182 2024-03-31 22:35:17.000000 StonerPlots-1.3.0/examples/figures/fig06.png
--rw-r--r--   0 runner    (1001) docker     (127)    30017 2024-03-31 22:35:17.000000 StonerPlots-1.3.0/examples/figures/fig07a.png
--rw-r--r--   0 runner    (1001) docker     (127)    41294 2024-03-31 22:35:17.000000 StonerPlots-1.3.0/examples/figures/fig7b.png
--rw-r--r--   0 runner    (1001) docker     (127)    54714 2024-03-31 22:35:17.000000 StonerPlots-1.3.0/examples/figures/fig7c.png
--rw-r--r--   0 runner    (1001) docker     (127)    43010 2024-03-31 22:35:17.000000 StonerPlots-1.3.0/examples/matplotlibrc
--rw-r--r--   0 runner    (1001) docker     (127)      323 2024-03-31 22:35:17.000000 StonerPlots-1.3.0/examples/plot-examples.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 22:38:34.805457 StonerPlots-1.3.0/examples/plot_examples/
--rw-r--r--   0 runner    (1001) docker     (127)      933 2024-03-31 22:35:17.000000 StonerPlots-1.3.0/examples/plot_examples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      420 2024-03-31 22:35:17.000000 StonerPlots-1.3.0/examples/plot_examples/common.py
--rw-r--r--   0 runner    (1001) docker     (127)      492 2024-03-31 22:35:17.000000 StonerPlots-1.3.0/examples/plot_examples/dark_plot.py
--rw-r--r--   0 runner    (1001) docker     (127)      498 2024-03-31 22:35:17.000000 StonerPlots-1.3.0/examples/plot_examples/default_plot.py
--rw-r--r--   0 runner    (1001) docker     (127)      519 2024-03-31 22:35:17.000000 StonerPlots-1.3.0/examples/plot_examples/default_plot_aip.py
--rw-r--r--   0 runner    (1001) docker     (127)      543 2024-03-31 22:35:17.000000 StonerPlots-1.3.0/examples/plot_examples/default_plot_aps.py
--rw-r--r--   0 runner    (1001) docker     (127)      541 2024-03-31 22:35:17.000000 StonerPlots-1.3.0/examples/plot_examples/default_plot_aps_1_5_column.py
--rw-r--r--   0 runner    (1001) docker     (127)      537 2024-03-31 22:35:17.000000 StonerPlots-1.3.0/examples/plot_examples/default_plot_aps_2_column.py
--rw-r--r--   0 runner    (1001) docker     (127)      523 2024-03-31 22:35:17.000000 StonerPlots-1.3.0/examples/plot_examples/default_plot_bright.py
--rw-r--r--   0 runner    (1001) docker     (127)      537 2024-03-31 22:35:17.000000 StonerPlots-1.3.0/examples/plot_examples/default_plot_high_contrast.py
--rw-r--r--   0 runner    (1001) docker     (127)      527 2024-03-31 22:35:17.000000 StonerPlots-1.3.0/examples/plot_examples/default_plot_high_vis.py
--rw-r--r--   0 runner    (1001) docker     (127)      521 2024-03-31 22:35:17.000000 StonerPlots-1.3.0/examples/plot_examples/default_plot_ieee.py
--rw-r--r--   0 runner    (1001) docker     (127)      519 2024-03-31 22:35:17.000000 StonerPlots-1.3.0/examples/plot_examples/default_plot_iop.py
--rw-r--r--   0 runner    (1001) docker     (127)      526 2024-03-31 22:35:17.000000 StonerPlots-1.3.0/examples/plot_examples/default_plot_latex.py
--rw-r--r--   0 runner    (1001) docker     (127)      521 2024-03-31 22:35:17.000000 StonerPlots-1.3.0/examples/plot_examples/default_plot_light.py
--rw-r--r--   0 runner    (1001) docker     (127)      521 2024-03-31 22:35:17.000000 StonerPlots-1.3.0/examples/plot_examples/default_plot_muted.py
--rw-r--r--   0 runner    (1001) docker     (127)      525 2024-03-31 22:35:17.000000 StonerPlots-1.3.0/examples/plot_examples/default_plot_nature.py
--rw-r--r--   0 runner    (1001) docker     (127)      521 2024-03-31 22:35:17.000000 StonerPlots-1.3.0/examples/plot_examples/default_plot_retro.py
--rw-r--r--   0 runner    (1001) docker     (127)      524 2024-03-31 22:35:17.000000 StonerPlots-1.3.0/examples/plot_examples/default_plot_std_colours.py
--rw-r--r--   0 runner    (1001) docker     (127)      525 2024-03-31 22:35:17.000000 StonerPlots-1.3.0/examples/plot_examples/default_plot_vibrant.py
--rw-r--r--   0 runner    (1001) docker     (127)      489 2024-03-31 22:35:17.000000 StonerPlots-1.3.0/examples/plot_examples/grid_plot.py
--rw-r--r--   0 runner    (1001) docker     (127)      507 2024-03-31 22:35:17.000000 StonerPlots-1.3.0/examples/plot_examples/hi_res_plot.py
--rw-r--r--   0 runner    (1001) docker     (127)      588 2024-03-31 22:35:17.000000 StonerPlots-1.3.0/examples/plot_examples/inset_plot.py
--rw-r--r--   0 runner    (1001) docker     (127)      612 2024-03-31 22:35:17.000000 StonerPlots-1.3.0/examples/plot_examples/multi_panel_plot.py
--rw-r--r--   0 runner    (1001) docker     (127)      500 2024-03-31 22:35:17.000000 StonerPlots-1.3.0/examples/plot_examples/notebook_plot.py
--rw-r--r--   0 runner    (1001) docker     (127)      594 2024-03-31 22:35:17.000000 StonerPlots-1.3.0/examples/plot_examples/poster_plot.py
--rw-r--r--   0 runner    (1001) docker     (127)      606 2024-03-31 22:35:17.000000 StonerPlots-1.3.0/examples/plot_examples/presentation_plot.py
--rw-r--r--   0 runner    (1001) docker     (127)     1035 2024-03-31 22:35:17.000000 StonerPlots-1.3.0/examples/plot_examples/scatter_plot.py
--rw-r--r--   0 runner    (1001) docker     (127)      689 2024-03-31 22:35:17.000000 StonerPlots-1.3.0/examples/plot_examples/small_presentation_dark_plot.py
--rw-r--r--   0 runner    (1001) docker     (127)      638 2024-03-31 22:35:17.000000 StonerPlots-1.3.0/examples/plot_examples/small_presentation_plot.py
--rw-r--r--   0 runner    (1001) docker     (127)      657 2024-03-31 22:35:17.000000 StonerPlots-1.3.0/examples/plot_examples/stacked_plot.py
--rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-03-31 22:35:17.000000 StonerPlots-1.3.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 22:38:34.809457 StonerPlots-1.3.0/recipe/
--rw-r--r--   0 runner    (1001) docker     (127)      181 2024-03-31 22:35:17.000000 StonerPlots-1.3.0/recipe/build-env.yml
--rw-r--r--   0 runner    (1001) docker     (127)      781 2024-03-31 22:35:17.000000 StonerPlots-1.3.0/recipe/meta.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-31 22:38:34.813457 StonerPlots-1.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      714 2024-03-31 22:35:17.000000 StonerPlots-1.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 22:38:34.789457 StonerPlots-1.3.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 22:38:34.813457 StonerPlots-1.3.0/src/StonerPlots.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5084 2024-03-31 22:38:34.000000 StonerPlots-1.3.0/src/StonerPlots.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4669 2024-03-31 22:38:34.000000 StonerPlots-1.3.0/src/StonerPlots.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-31 22:38:34.000000 StonerPlots-1.3.0/src/StonerPlots.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-03-31 22:38:34.000000 StonerPlots-1.3.0/src/StonerPlots.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 22:38:34.809457 StonerPlots-1.3.0/src/stonerplots/
--rw-r--r--   0 runner    (1001) docker     (127)     1316 2024-03-31 22:35:17.000000 StonerPlots-1.3.0/src/stonerplots/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3227 2024-03-31 22:35:17.000000 StonerPlots-1.3.0/src/stonerplots/colours.py
--rw-r--r--   0 runner    (1001) docker     (127)    23320 2024-03-31 22:35:17.000000 StonerPlots-1.3.0/src/stonerplots/context.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 22:38:34.809457 StonerPlots-1.3.0/src/stonerplots/styles/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 22:38:34.809457 StonerPlots-1.3.0/src/stonerplots/styles/color/
--rw-r--r--   0 runner    (1001) docker     (127)      226 2024-03-31 22:35:17.000000 StonerPlots-1.3.0/src/stonerplots/styles/color/bright.mplstyle
--rw-r--r--   0 runner    (1001) docker     (127)      193 2024-03-31 22:35:17.000000 StonerPlots-1.3.0/src/stonerplots/styles/color/high-contrast.mplstyle
--rw-r--r--   0 runner    (1001) docker     (127)      237 2024-03-31 22:35:17.000000 StonerPlots-1.3.0/src/stonerplots/styles/color/high-vis.mplstyle
--rw-r--r--   0 runner    (1001) docker     (127)      245 2024-03-31 22:35:17.000000 StonerPlots-1.3.0/src/stonerplots/styles/color/light.mplstyle
--rw-r--r--   0 runner    (1001) docker     (127)      255 2024-03-31 22:35:17.000000 StonerPlots-1.3.0/src/stonerplots/styles/color/muted.mplstyle
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-03-31 22:35:17.000000 StonerPlots-1.3.0/src/stonerplots/styles/color/retro.mplstyle
--rw-r--r--   0 runner    (1001) docker     (127)      201 2024-03-31 22:35:17.000000 StonerPlots-1.3.0/src/stonerplots/styles/color/std-colours.mplstyle
--rw-r--r--   0 runner    (1001) docker     (127)      880 2024-03-31 22:35:17.000000 StonerPlots-1.3.0/src/stonerplots/styles/color/stoner_dark.mplstyle
--rw-r--r--   0 runner    (1001) docker     (127)      227 2024-03-31 22:35:17.000000 StonerPlots-1.3.0/src/stonerplots/styles/color/vibrant.mplstyle
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 22:38:34.813457 StonerPlots-1.3.0/src/stonerplots/styles/journals/
--rw-r--r--   0 runner    (1001) docker     (127)      973 2024-03-31 22:35:17.000000 StonerPlots-1.3.0/src/stonerplots/styles/journals/aip.mplstyle
--rw-r--r--   0 runner    (1001) docker     (127)      984 2024-03-31 22:35:17.000000 StonerPlots-1.3.0/src/stonerplots/styles/journals/aps.mplstyle
--rw-r--r--   0 runner    (1001) docker     (127)      395 2024-03-31 22:35:17.000000 StonerPlots-1.3.0/src/stonerplots/styles/journals/ieee.mplstyle
--rw-r--r--   0 runner    (1001) docker     (127)      974 2024-03-31 22:35:17.000000 StonerPlots-1.3.0/src/stonerplots/styles/journals/iop.mplstyle
--rw-r--r--   0 runner    (1001) docker     (127)      908 2024-03-31 22:35:17.000000 StonerPlots-1.3.0/src/stonerplots/styles/journals/nature.mplstyle
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 22:38:34.813457 StonerPlots-1.3.0/src/stonerplots/styles/misc/
--rw-r--r--   0 runner    (1001) docker     (127)      272 2024-03-31 22:35:17.000000 StonerPlots-1.3.0/src/stonerplots/styles/misc/grid.mplstyle
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-03-31 22:35:17.000000 StonerPlots-1.3.0/src/stonerplots/styles/misc/pgf.mplstyle
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 22:38:34.813457 StonerPlots-1.3.0/src/stonerplots/styles/modifiers/
--rw-r--r--   0 runner    (1001) docker     (127)      305 2024-03-31 22:35:17.000000 StonerPlots-1.3.0/src/stonerplots/styles/modifiers/aip2.mplstyle
--rw-r--r--   0 runner    (1001) docker     (127)      291 2024-03-31 22:35:17.000000 StonerPlots-1.3.0/src/stonerplots/styles/modifiers/aps1.5.mplstyle
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-03-31 22:35:17.000000 StonerPlots-1.3.0/src/stonerplots/styles/modifiers/aps2.mplstyle
--rw-r--r--   0 runner    (1001) docker     (127)      141 2024-03-31 22:35:17.000000 StonerPlots-1.3.0/src/stonerplots/styles/modifiers/hi-res.mplstyle
--rw-r--r--   0 runner    (1001) docker     (127)      378 2024-03-31 22:35:17.000000 StonerPlots-1.3.0/src/stonerplots/styles/modifiers/latex-sans.mplstyle
--rw-r--r--   0 runner    (1001) docker     (127)      384 2024-03-31 22:35:17.000000 StonerPlots-1.3.0/src/stonerplots/styles/modifiers/latex.mplstyle
--rw-r--r--   0 runner    (1001) docker     (127)      226 2024-03-31 22:35:17.000000 StonerPlots-1.3.0/src/stonerplots/styles/modifiers/no-latex.mplstyle
--rw-r--r--   0 runner    (1001) docker     (127)      261 2024-03-31 22:35:17.000000 StonerPlots-1.3.0/src/stonerplots/styles/modifiers/presentation_dark.mplstyle
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-03-31 22:35:17.000000 StonerPlots-1.3.0/src/stonerplots/styles/modifiers/presentation_sm.mplstyle
--rw-r--r--   0 runner    (1001) docker     (127)      364 2024-03-31 22:35:17.000000 StonerPlots-1.3.0/src/stonerplots/styles/modifiers/sans.mplstyle
--rw-r--r--   0 runner    (1001) docker     (127)      643 2024-03-31 22:35:17.000000 StonerPlots-1.3.0/src/stonerplots/styles/notebook.mplstyle
--rw-r--r--   0 runner    (1001) docker     (127)     1133 2024-03-31 22:35:17.000000 StonerPlots-1.3.0/src/stonerplots/styles/poster.mplstyle
--rw-r--r--   0 runner    (1001) docker     (127)      674 2024-03-31 22:35:17.000000 StonerPlots-1.3.0/src/stonerplots/styles/presentation.mplstyle
--rw-r--r--   0 runner    (1001) docker     (127)      333 2024-03-31 22:35:17.000000 StonerPlots-1.3.0/src/stonerplots/styles/scatter.mplstyle
--rw-r--r--   0 runner    (1001) docker     (127)     2026 2024-03-31 22:35:17.000000 StonerPlots-1.3.0/src/stonerplots/styles/stoner.mplstyle
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:53:14.354100 StonerPlots-1.3.1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:53:14.330100 StonerPlots-1.3.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:53:14.330100 StonerPlots-1.3.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1656 2024-04-01 20:50:09.000000 StonerPlots-1.3.1/.github/workflows/build_conda.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      396 2024-04-01 20:50:09.000000 StonerPlots-1.3.1/.github/workflows/publish_sphinx.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3200 2024-04-01 20:50:09.000000 StonerPlots-1.3.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      198 2024-04-01 20:50:09.000000 StonerPlots-1.3.1/CHANGES.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1153 2024-04-01 20:50:09.000000 StonerPlots-1.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-01 20:50:09.000000 StonerPlots-1.3.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5084 2024-04-01 20:53:14.354100 StonerPlots-1.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4392 2024-04-01 20:50:09.000000 StonerPlots-1.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:53:14.330100 StonerPlots-1.3.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-04-01 20:50:09.000000 StonerPlots-1.3.1/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      769 2024-04-01 20:50:09.000000 StonerPlots-1.3.1/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-01 20:50:09.000000 StonerPlots-1.3.1/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:53:14.334100 StonerPlots-1.3.1/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:53:14.334100 StonerPlots-1.3.1/docs/source/api/
+-rw-r--r--   0 runner    (1001) docker     (127)      258 2024-04-01 20:50:09.000000 StonerPlots-1.3.1/docs/source/api/stonerplots.InsetPlot.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-01 20:50:09.000000 StonerPlots-1.3.1/docs/source/api/stonerplots.MultiPanel.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-04-01 20:50:09.000000 StonerPlots-1.3.1/docs/source/api/stonerplots.SavedFigure.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-01 20:50:09.000000 StonerPlots-1.3.1/docs/source/api/stonerplots.StackVertical.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-01 20:50:09.000000 StonerPlots-1.3.1/docs/source/api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      912 2024-04-01 20:50:09.000000 StonerPlots-1.3.1/docs/source/colours.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1630 2024-04-01 20:50:09.000000 StonerPlots-1.3.1/docs/source/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:53:14.334100 StonerPlots-1.3.1/docs/source/figures/
+-rw-r--r--   0 runner    (1001) docker     (127)    25332 2024-04-01 20:50:09.000000 StonerPlots-1.3.1/docs/source/figures/StonerLogo2.png
+-rw-r--r--   0 runner    (1001) docker     (127)    31938 2024-04-01 20:50:09.000000 StonerPlots-1.3.1/docs/source/figures/colours.png
+-rw-r--r--   0 runner    (1001) docker     (127)    23528 2024-04-01 20:50:09.000000 StonerPlots-1.3.1/docs/source/figures/colours10.png
+-rw-r--r--   0 runner    (1001) docker     (127)    21940 2024-04-01 20:50:09.000000 StonerPlots-1.3.1/docs/source/figures/colours50.png
+-rw-r--r--   0 runner    (1001) docker     (127)    21393 2024-04-01 20:50:09.000000 StonerPlots-1.3.1/docs/source/figures/colours70.png
+-rw-r--r--   0 runner    (1001) docker     (127)    22543 2024-04-01 20:50:09.000000 StonerPlots-1.3.1/docs/source/figures/colours90.png
+-rw-r--r--   0 runner    (1001) docker     (127)    47643 2024-04-01 20:50:09.000000 StonerPlots-1.3.1/docs/source/figures/example-1.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2195 2024-04-01 20:50:09.000000 StonerPlots-1.3.1/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2908 2024-04-01 20:50:09.000000 StonerPlots-1.3.1/docs/source/insetplot.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2214 2024-04-01 20:50:09.000000 StonerPlots-1.3.1/docs/source/multipanel.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     6157 2024-04-01 20:50:09.000000 StonerPlots-1.3.1/docs/source/savedfigure.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4823 2024-04-01 20:50:09.000000 StonerPlots-1.3.1/docs/source/stackvertical.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    15165 2024-04-01 20:50:09.000000 StonerPlots-1.3.1/docs/source/style-gallery.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    14062 2024-04-01 20:50:09.000000 StonerPlots-1.3.1/docs/source/userguide.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:53:14.334100 StonerPlots-1.3.1/examples/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:53:14.342100 StonerPlots-1.3.1/examples/figures/
+-rw-r--r--   0 runner    (1001) docker     (127)    29690 2024-04-01 20:50:09.000000 StonerPlots-1.3.1/examples/figures/fig01a.png
+-rw-r--r--   0 runner    (1001) docker     (127)    26194 2024-04-01 20:50:09.000000 StonerPlots-1.3.1/examples/figures/fig01b.png
+-rw-r--r--   0 runner    (1001) docker     (127)    24459 2024-04-01 20:50:09.000000 StonerPlots-1.3.1/examples/figures/fig02a.png
+-rw-r--r--   0 runner    (1001) docker     (127)    17925 2024-04-01 20:50:09.000000 StonerPlots-1.3.1/examples/figures/fig02b.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)    27629 2024-04-01 20:50:09.000000 StonerPlots-1.3.1/examples/figures/fig02b.png
+-rw-r--r--   0 runner    (1001) docker     (127)    26406 2024-04-01 20:50:09.000000 StonerPlots-1.3.1/examples/figures/fig02c.png
+-rw-r--r--   0 runner    (1001) docker     (127)    26371 2024-04-01 20:50:09.000000 StonerPlots-1.3.1/examples/figures/fig02d.png
+-rw-r--r--   0 runner    (1001) docker     (127)    25087 2024-04-01 20:50:09.000000 StonerPlots-1.3.1/examples/figures/fig02e.png
+-rw-r--r--   0 runner    (1001) docker     (127)    37979 2024-04-01 20:50:09.000000 StonerPlots-1.3.1/examples/figures/fig02f.png
+-rw-r--r--   0 runner    (1001) docker     (127)    51713 2024-04-01 20:50:09.000000 StonerPlots-1.3.1/examples/figures/fig02g.png
+-rw-r--r--   0 runner    (1001) docker     (127)    24873 2024-04-01 20:50:09.000000 StonerPlots-1.3.1/examples/figures/fig02h_0.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)    47051 2024-04-01 20:50:09.000000 StonerPlots-1.3.1/examples/figures/fig02h_0.png
+-rw-r--r--   0 runner    (1001) docker     (127)    28894 2024-04-01 20:50:09.000000 StonerPlots-1.3.1/examples/figures/fig02h_1.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)    50101 2024-04-01 20:50:09.000000 StonerPlots-1.3.1/examples/figures/fig02h_1.png
+-rw-r--r--   0 runner    (1001) docker     (127)    27613 2024-04-01 20:50:09.000000 StonerPlots-1.3.1/examples/figures/fig03.png
+-rw-r--r--   0 runner    (1001) docker     (127)    28761 2024-04-01 20:50:09.000000 StonerPlots-1.3.1/examples/figures/fig04a.png
+-rw-r--r--   0 runner    (1001) docker     (127)    29370 2024-04-01 20:50:09.000000 StonerPlots-1.3.1/examples/figures/fig04b.png
+-rw-r--r--   0 runner    (1001) docker     (127)    29396 2024-04-01 20:50:09.000000 StonerPlots-1.3.1/examples/figures/fig04c.png
+-rw-r--r--   0 runner    (1001) docker     (127)    28832 2024-04-01 20:50:09.000000 StonerPlots-1.3.1/examples/figures/fig04d.png
+-rw-r--r--   0 runner    (1001) docker     (127)    27732 2024-04-01 20:50:09.000000 StonerPlots-1.3.1/examples/figures/fig04e.png
+-rw-r--r--   0 runner    (1001) docker     (127)    29246 2024-04-01 20:50:09.000000 StonerPlots-1.3.1/examples/figures/fig04f.png
+-rw-r--r--   0 runner    (1001) docker     (127)    28862 2024-04-01 20:50:09.000000 StonerPlots-1.3.1/examples/figures/fig04g.png
+-rw-r--r--   0 runner    (1001) docker     (127)    29207 2024-04-01 20:50:09.000000 StonerPlots-1.3.1/examples/figures/fig04h.png
+-rw-r--r--   0 runner    (1001) docker     (127)    29362 2024-04-01 20:50:09.000000 StonerPlots-1.3.1/examples/figures/fig04i.png
+-rw-r--r--   0 runner    (1001) docker     (127)    80367 2024-04-01 20:50:09.000000 StonerPlots-1.3.1/examples/figures/fig05a.png
+-rw-r--r--   0 runner    (1001) docker     (127)    86165 2024-04-01 20:50:09.000000 StonerPlots-1.3.1/examples/figures/fig05b.png
+-rw-r--r--   0 runner    (1001) docker     (127)   166258 2024-04-01 20:50:09.000000 StonerPlots-1.3.1/examples/figures/fig05c.png
+-rw-r--r--   0 runner    (1001) docker     (127)   140055 2024-04-01 20:50:09.000000 StonerPlots-1.3.1/examples/figures/fig05d.png
+-rw-r--r--   0 runner    (1001) docker     (127)   134163 2024-04-01 20:50:09.000000 StonerPlots-1.3.1/examples/figures/fig05e.png
+-rw-r--r--   0 runner    (1001) docker     (127)   211090 2024-04-01 20:50:09.000000 StonerPlots-1.3.1/examples/figures/fig05f.png
+-rw-r--r--   0 runner    (1001) docker     (127)    36182 2024-04-01 20:50:09.000000 StonerPlots-1.3.1/examples/figures/fig06.png
+-rw-r--r--   0 runner    (1001) docker     (127)    30017 2024-04-01 20:50:09.000000 StonerPlots-1.3.1/examples/figures/fig07a.png
+-rw-r--r--   0 runner    (1001) docker     (127)    41294 2024-04-01 20:50:09.000000 StonerPlots-1.3.1/examples/figures/fig7b.png
+-rw-r--r--   0 runner    (1001) docker     (127)    54714 2024-04-01 20:50:09.000000 StonerPlots-1.3.1/examples/figures/fig7c.png
+-rw-r--r--   0 runner    (1001) docker     (127)    43010 2024-04-01 20:50:09.000000 StonerPlots-1.3.1/examples/matplotlibrc
+-rw-r--r--   0 runner    (1001) docker     (127)      323 2024-04-01 20:50:09.000000 StonerPlots-1.3.1/examples/plot-examples.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:53:14.346100 StonerPlots-1.3.1/examples/plot_examples/
+-rw-r--r--   0 runner    (1001) docker     (127)      960 2024-04-01 20:50:09.000000 StonerPlots-1.3.1/examples/plot_examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      420 2024-04-01 20:50:09.000000 StonerPlots-1.3.1/examples/plot_examples/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)      491 2024-04-01 20:50:09.000000 StonerPlots-1.3.1/examples/plot_examples/dark_plot.py
+-rw-r--r--   0 runner    (1001) docker     (127)      497 2024-04-01 20:50:09.000000 StonerPlots-1.3.1/examples/plot_examples/default_plot.py
+-rw-r--r--   0 runner    (1001) docker     (127)      518 2024-04-01 20:50:09.000000 StonerPlots-1.3.1/examples/plot_examples/default_plot_aip.py
+-rw-r--r--   0 runner    (1001) docker     (127)      542 2024-04-01 20:50:09.000000 StonerPlots-1.3.1/examples/plot_examples/default_plot_aps.py
+-rw-r--r--   0 runner    (1001) docker     (127)      540 2024-04-01 20:50:09.000000 StonerPlots-1.3.1/examples/plot_examples/default_plot_aps_1_5_column.py
+-rw-r--r--   0 runner    (1001) docker     (127)      536 2024-04-01 20:50:09.000000 StonerPlots-1.3.1/examples/plot_examples/default_plot_aps_2_column.py
+-rw-r--r--   0 runner    (1001) docker     (127)      522 2024-04-01 20:50:09.000000 StonerPlots-1.3.1/examples/plot_examples/default_plot_bright.py
+-rw-r--r--   0 runner    (1001) docker     (127)      536 2024-04-01 20:50:09.000000 StonerPlots-1.3.1/examples/plot_examples/default_plot_high_contrast.py
+-rw-r--r--   0 runner    (1001) docker     (127)      526 2024-04-01 20:50:09.000000 StonerPlots-1.3.1/examples/plot_examples/default_plot_high_vis.py
+-rw-r--r--   0 runner    (1001) docker     (127)      520 2024-04-01 20:50:09.000000 StonerPlots-1.3.1/examples/plot_examples/default_plot_ieee.py
+-rw-r--r--   0 runner    (1001) docker     (127)      518 2024-04-01 20:50:09.000000 StonerPlots-1.3.1/examples/plot_examples/default_plot_iop.py
+-rw-r--r--   0 runner    (1001) docker     (127)      525 2024-04-01 20:50:09.000000 StonerPlots-1.3.1/examples/plot_examples/default_plot_latex.py
+-rw-r--r--   0 runner    (1001) docker     (127)      520 2024-04-01 20:50:09.000000 StonerPlots-1.3.1/examples/plot_examples/default_plot_light.py
+-rw-r--r--   0 runner    (1001) docker     (127)      520 2024-04-01 20:50:09.000000 StonerPlots-1.3.1/examples/plot_examples/default_plot_muted.py
+-rw-r--r--   0 runner    (1001) docker     (127)      524 2024-04-01 20:50:09.000000 StonerPlots-1.3.1/examples/plot_examples/default_plot_nature.py
+-rw-r--r--   0 runner    (1001) docker     (127)      520 2024-04-01 20:50:09.000000 StonerPlots-1.3.1/examples/plot_examples/default_plot_retro.py
+-rw-r--r--   0 runner    (1001) docker     (127)      523 2024-04-01 20:50:09.000000 StonerPlots-1.3.1/examples/plot_examples/default_plot_std_colours.py
+-rw-r--r--   0 runner    (1001) docker     (127)      895 2024-04-01 20:50:09.000000 StonerPlots-1.3.1/examples/plot_examples/default_plot_thesis.py
+-rw-r--r--   0 runner    (1001) docker     (127)      524 2024-04-01 20:50:09.000000 StonerPlots-1.3.1/examples/plot_examples/default_plot_vibrant.py
+-rw-r--r--   0 runner    (1001) docker     (127)      488 2024-04-01 20:50:09.000000 StonerPlots-1.3.1/examples/plot_examples/grid_plot.py
+-rw-r--r--   0 runner    (1001) docker     (127)      506 2024-04-01 20:50:09.000000 StonerPlots-1.3.1/examples/plot_examples/hi_res_plot.py
+-rw-r--r--   0 runner    (1001) docker     (127)      587 2024-04-01 20:50:09.000000 StonerPlots-1.3.1/examples/plot_examples/inset_plot.py
+-rw-r--r--   0 runner    (1001) docker     (127)      611 2024-04-01 20:50:09.000000 StonerPlots-1.3.1/examples/plot_examples/multi_panel_plot.py
+-rw-r--r--   0 runner    (1001) docker     (127)      499 2024-04-01 20:50:09.000000 StonerPlots-1.3.1/examples/plot_examples/notebook_plot.py
+-rw-r--r--   0 runner    (1001) docker     (127)      593 2024-04-01 20:50:09.000000 StonerPlots-1.3.1/examples/plot_examples/poster_plot.py
+-rw-r--r--   0 runner    (1001) docker     (127)      605 2024-04-01 20:50:09.000000 StonerPlots-1.3.1/examples/plot_examples/presentation_plot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-04-01 20:50:09.000000 StonerPlots-1.3.1/examples/plot_examples/scatter_plot.py
+-rw-r--r--   0 runner    (1001) docker     (127)      688 2024-04-01 20:50:09.000000 StonerPlots-1.3.1/examples/plot_examples/small_presentation_dark_plot.py
+-rw-r--r--   0 runner    (1001) docker     (127)      637 2024-04-01 20:50:09.000000 StonerPlots-1.3.1/examples/plot_examples/small_presentation_plot.py
+-rw-r--r--   0 runner    (1001) docker     (127)      656 2024-04-01 20:50:09.000000 StonerPlots-1.3.1/examples/plot_examples/stacked_plot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-04-01 20:50:09.000000 StonerPlots-1.3.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:53:14.346100 StonerPlots-1.3.1/recipe/
+-rw-r--r--   0 runner    (1001) docker     (127)      181 2024-04-01 20:50:09.000000 StonerPlots-1.3.1/recipe/build-env.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      781 2024-04-01 20:50:09.000000 StonerPlots-1.3.1/recipe/meta.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-01 20:53:14.354100 StonerPlots-1.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      714 2024-04-01 20:50:09.000000 StonerPlots-1.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:53:14.330100 StonerPlots-1.3.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:53:14.354100 StonerPlots-1.3.1/src/StonerPlots.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5084 2024-04-01 20:53:14.000000 StonerPlots-1.3.1/src/StonerPlots.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5028 2024-04-01 20:53:14.000000 StonerPlots-1.3.1/src/StonerPlots.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 20:53:14.000000 StonerPlots-1.3.1/src/StonerPlots.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-01 20:53:14.000000 StonerPlots-1.3.1/src/StonerPlots.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:53:14.350100 StonerPlots-1.3.1/src/stonerplots/
+-rw-r--r--   0 runner    (1001) docker     (127)     1316 2024-04-01 20:50:09.000000 StonerPlots-1.3.1/src/stonerplots/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3227 2024-04-01 20:50:09.000000 StonerPlots-1.3.1/src/stonerplots/colours.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23554 2024-04-01 20:50:09.000000 StonerPlots-1.3.1/src/stonerplots/context.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:53:14.350100 StonerPlots-1.3.1/src/stonerplots/styles/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:53:14.350100 StonerPlots-1.3.1/src/stonerplots/styles/color/
+-rw-r--r--   0 runner    (1001) docker     (127)      226 2024-04-01 20:50:09.000000 StonerPlots-1.3.1/src/stonerplots/styles/color/bright.mplstyle
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-04-01 20:50:09.000000 StonerPlots-1.3.1/src/stonerplots/styles/color/high-contrast.mplstyle
+-rw-r--r--   0 runner    (1001) docker     (127)      237 2024-04-01 20:50:09.000000 StonerPlots-1.3.1/src/stonerplots/styles/color/high-vis.mplstyle
+-rw-r--r--   0 runner    (1001) docker     (127)      245 2024-04-01 20:50:09.000000 StonerPlots-1.3.1/src/stonerplots/styles/color/light.mplstyle
+-rw-r--r--   0 runner    (1001) docker     (127)      255 2024-04-01 20:50:09.000000 StonerPlots-1.3.1/src/stonerplots/styles/color/muted.mplstyle
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-01 20:50:09.000000 StonerPlots-1.3.1/src/stonerplots/styles/color/retro.mplstyle
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-04-01 20:50:09.000000 StonerPlots-1.3.1/src/stonerplots/styles/color/std-colours.mplstyle
+-rw-r--r--   0 runner    (1001) docker     (127)      880 2024-04-01 20:50:09.000000 StonerPlots-1.3.1/src/stonerplots/styles/color/stoner_dark.mplstyle
+-rw-r--r--   0 runner    (1001) docker     (127)      227 2024-04-01 20:50:09.000000 StonerPlots-1.3.1/src/stonerplots/styles/color/vibrant.mplstyle
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:53:14.350100 StonerPlots-1.3.1/src/stonerplots/styles/journals/
+-rw-r--r--   0 runner    (1001) docker     (127)      973 2024-04-01 20:50:09.000000 StonerPlots-1.3.1/src/stonerplots/styles/journals/aip.mplstyle
+-rw-r--r--   0 runner    (1001) docker     (127)      984 2024-04-01 20:50:09.000000 StonerPlots-1.3.1/src/stonerplots/styles/journals/aps.mplstyle
+-rw-r--r--   0 runner    (1001) docker     (127)      395 2024-04-01 20:50:09.000000 StonerPlots-1.3.1/src/stonerplots/styles/journals/ieee.mplstyle
+-rw-r--r--   0 runner    (1001) docker     (127)      974 2024-04-01 20:50:09.000000 StonerPlots-1.3.1/src/stonerplots/styles/journals/iop.mplstyle
+-rw-r--r--   0 runner    (1001) docker     (127)      908 2024-04-01 20:50:09.000000 StonerPlots-1.3.1/src/stonerplots/styles/journals/nature.mplstyle
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:53:14.350100 StonerPlots-1.3.1/src/stonerplots/styles/misc/
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-04-01 20:50:09.000000 StonerPlots-1.3.1/src/stonerplots/styles/misc/grid.mplstyle
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-04-01 20:50:09.000000 StonerPlots-1.3.1/src/stonerplots/styles/misc/pgf.mplstyle
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:53:14.354100 StonerPlots-1.3.1/src/stonerplots/styles/modifiers/
+-rw-r--r--   0 runner    (1001) docker     (127)      305 2024-04-01 20:50:09.000000 StonerPlots-1.3.1/src/stonerplots/styles/modifiers/aip2.mplstyle
+-rw-r--r--   0 runner    (1001) docker     (127)      291 2024-04-01 20:50:09.000000 StonerPlots-1.3.1/src/stonerplots/styles/modifiers/aps1.5.mplstyle
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-01 20:50:09.000000 StonerPlots-1.3.1/src/stonerplots/styles/modifiers/aps2.mplstyle
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-04-01 20:50:09.000000 StonerPlots-1.3.1/src/stonerplots/styles/modifiers/hi-res.mplstyle
+-rw-r--r--   0 runner    (1001) docker     (127)      378 2024-04-01 20:50:09.000000 StonerPlots-1.3.1/src/stonerplots/styles/modifiers/latex-sans.mplstyle
+-rw-r--r--   0 runner    (1001) docker     (127)      384 2024-04-01 20:50:09.000000 StonerPlots-1.3.1/src/stonerplots/styles/modifiers/latex.mplstyle
+-rw-r--r--   0 runner    (1001) docker     (127)      226 2024-04-01 20:50:09.000000 StonerPlots-1.3.1/src/stonerplots/styles/modifiers/no-latex.mplstyle
+-rw-r--r--   0 runner    (1001) docker     (127)      261 2024-04-01 20:50:09.000000 StonerPlots-1.3.1/src/stonerplots/styles/modifiers/presentation_dark.mplstyle
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-01 20:50:09.000000 StonerPlots-1.3.1/src/stonerplots/styles/modifiers/presentation_sm.mplstyle
+-rw-r--r--   0 runner    (1001) docker     (127)      364 2024-04-01 20:50:09.000000 StonerPlots-1.3.1/src/stonerplots/styles/modifiers/sans.mplstyle
+-rw-r--r--   0 runner    (1001) docker     (127)      643 2024-04-01 20:50:09.000000 StonerPlots-1.3.1/src/stonerplots/styles/notebook.mplstyle
+-rw-r--r--   0 runner    (1001) docker     (127)     1133 2024-04-01 20:50:09.000000 StonerPlots-1.3.1/src/stonerplots/styles/poster.mplstyle
+-rw-r--r--   0 runner    (1001) docker     (127)      674 2024-04-01 20:50:09.000000 StonerPlots-1.3.1/src/stonerplots/styles/presentation.mplstyle
+-rw-r--r--   0 runner    (1001) docker     (127)      333 2024-04-01 20:50:09.000000 StonerPlots-1.3.1/src/stonerplots/styles/scatter.mplstyle
+-rw-r--r--   0 runner    (1001) docker     (127)     2026 2024-04-01 20:50:09.000000 StonerPlots-1.3.1/src/stonerplots/styles/stoner.mplstyle
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-01 20:50:09.000000 StonerPlots-1.3.1/src/stonerplots/styles/thesis.mplstyle
```

### Comparing `StonerPlots-1.3.0/.github/workflows/build_conda.yaml` & `StonerPlots-1.3.1/.github/workflows/build_conda.yaml`

 * *Files identical despite different names*

### Comparing `StonerPlots-1.3.0/.gitignore` & `StonerPlots-1.3.1/.gitignore`

 * *Files identical despite different names*

### Comparing `StonerPlots-1.3.0/LICENSE` & `StonerPlots-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `StonerPlots-1.3.0/PKG-INFO` & `StonerPlots-1.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: StonerPlots
-Version: 1.3.0
+Version: 1.3.1
 Summary: This is a fork of scienceplots and provides a range of matplotlib styles for plotting physics...
 Author-email: Gavin Burnell <G.Burnell@leeds.ac.uk>
 Project-URL: Homepage, https://github.com/stonerlab/stonerplots/
 Project-URL: Issues, https://github.com/stonerlab/stonerplots/issues
 Keywords: matplotlib-style-sheets,matplotlib-figures,scientific-papers,thesis-template,matplotlib-styles,python
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `StonerPlots-1.3.0/README.md` & `StonerPlots-1.3.1/README.md`

 * *Files identical despite different names*

### Comparing `StonerPlots-1.3.0/docs/Makefile` & `StonerPlots-1.3.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `StonerPlots-1.3.0/docs/make.bat` & `StonerPlots-1.3.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `StonerPlots-1.3.0/docs/source/colours.rst` & `StonerPlots-1.3.1/docs/source/colours.rst`

 * *Files identical despite different names*

### Comparing `StonerPlots-1.3.0/docs/source/conf.py` & `StonerPlots-1.3.1/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `StonerPlots-1.3.0/docs/source/figures/StonerLogo2.png` & `StonerPlots-1.3.1/docs/source/figures/StonerLogo2.png`

 * *Files identical despite different names*

### Comparing `StonerPlots-1.3.0/docs/source/figures/colours.png` & `StonerPlots-1.3.1/docs/source/figures/colours.png`

 * *Files identical despite different names*

### Comparing `StonerPlots-1.3.0/docs/source/figures/colours10.png` & `StonerPlots-1.3.1/docs/source/figures/colours10.png`

 * *Files identical despite different names*

### Comparing `StonerPlots-1.3.0/docs/source/figures/colours50.png` & `StonerPlots-1.3.1/docs/source/figures/colours50.png`

 * *Files identical despite different names*

### Comparing `StonerPlots-1.3.0/docs/source/figures/colours70.png` & `StonerPlots-1.3.1/docs/source/figures/colours70.png`

 * *Files identical despite different names*

### Comparing `StonerPlots-1.3.0/docs/source/figures/colours90.png` & `StonerPlots-1.3.1/docs/source/figures/colours90.png`

 * *Files identical despite different names*

### Comparing `StonerPlots-1.3.0/docs/source/figures/example-1.png` & `StonerPlots-1.3.1/docs/source/figures/example-1.png`

 * *Files identical despite different names*

### Comparing `StonerPlots-1.3.0/docs/source/index.rst` & `StonerPlots-1.3.1/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `StonerPlots-1.3.0/docs/source/style-gallery.rst` & `StonerPlots-1.3.1/docs/source/style-gallery.rst`

 * *Files 8% similar despite different names*

```diff
@@ -85,14 +85,30 @@
 | .. image:: ../../examples/figures/fig02g.png                                                            |
 |    :alt: Example fogure in APS 2 Column format                                                          |
 |    :align: center                                                                                       |
 |                                                                                                         |
 | Using styles ["stoner", "aps","aps2"]                                                                   |
 |                                                                                                         |
 +-----------------------------------------------------+---------------------------------------------------+
+|                                                                                                         |
+| .. image:: ../../examples/figures/fig02h_0.png                                                          |
+|    :alt: Example plot in thesis template format                                                         |
+|    :align: center                                                                                       |
+|                                                                                                         |
+| Using styles ["stoner", "thesis"]                                                                       |
+|                                                                                                         |
++-----------------------------------------------------+---------------------------------------------------+
+|                                                                                                         |
+| .. image:: ../../examples/figures/fig02h_1.png                                                          |
+|    :alt: Example twin plot in thesis template format                                                    |
+|    :align: center                                                                                       |
+|                                                                                                         |
+| Using styles ["stoner", "thesis"] and MultiPanel with manual adjust_figsize=(0,-0.25)                   |
+|                                                                                                         |
++-----------------------------------------------------+---------------------------------------------------+
 
 3. Different Plot Types
 -----------------------
 
 There is a *scatter* plot style that sets up for doing scatter plots.
 
 .. image:: ../../examples/figures/fig03.png
@@ -246,16 +262,16 @@
 The :py:class:`stonerplots.StackVertical` context manager can be used for this.
 
 
 .. image:: ../../examples/figures/fig7b.png
   :alt: 3-panel vertically stacked plot
   :align: center
 
-  MultiPanel Sub-plots
-  ~~~~~~~~~~~~~~~~~~~~
+MultiPanel Sub-plots
+~~~~~~~~~~~~~~~~~~~~
 
 Where a figure just needs to show a collection of related datasets, a multi-panel figure with sub-plots is a good
 option. The :py:class:`stonerplots.MultiPanel` context manager makes this a bit easier.
 
 .. image:: ../../examples/figures/fig7c.png
   :alt: 2x2 multi-panel plot.
   :align: center
```

### Comparing `StonerPlots-1.3.0/docs/source/userguide.rst` & `StonerPlots-1.3.1/docs/source/userguide.rst`

 * *Files 19% similar despite different names*

```diff
@@ -1,333 +1,271 @@
 Stoner Plots User Guide
 =======================
 
+.. currentmodule:: stonerplots.context
+
 Although you can make use of the style sheets directly in matplotlib after impriting stonerplots, it is anticipated
 that using the :doc:`stonerplots<api>` context managers will be the main way of using the package.
 
 The look of the various stylesheets is demonstrated in the :doc:`style gallery<style-gallery>` page.
 
 Context Managers Primer
 -----------------------
 
 In Python, a context manager is used in a `with ... :` statement. Its main advantage is that it ensures that
 initialisiation and cleanup code are executed around the enclosed block of statements, no matter why the code block
 exited (e.g. due to an Exception or due to normal termination). This is generally used to ensure resources, such as
 open network conenctions, open files etc. are opened and cleaned up properly.
 
-The other reason a context manager might be used, is to temporarily change something in the environment the code is
-running in for the duration of the enclosed lines of code. Matplotlib offers context managers that operate in this way
-to temporarily set default parameters (:py:func:`matplotlib.pyplot.rc_context`) or to temporarily apply stylesheets
-(py:func:`matplotlib.style.context`).
-
-.. currentmodule:: stonerplots.context
-
-SavedFigure Context Manager
----------------------------
-
-The  :py:class:`SavedFigure` is used to bpth apply style sheets and capture the current figure and save it to disk.
-It applies stylesheets by wrapping a :py:func:`matplotlib.style.context` context manager. On entry, the context manager
-will note the open matplotlib figures, and on exit it will compare the list of copen figures with those that existed at
-entry, and save all the new figures. Therefore, it is very important that figure creation is done **inside** the
-:py:class:`SavedFigure` context manager.
-
-Simple Example
-~~~~~~~~~~~~~~
-
-In its simplest form, :py:class:`SavedFigure` just needs to know a filename to save the figure as::
-
-    with SavedFigure("example.png"):
-        fig, ax = plt.subplots()
-        ax.plot(x_data, y_data)
-
-In this case, the stylesheet is switched to the default "stoner" style, the format to save the file in is determined
-from the filename to be a PNG file, and the open figure will be saved to the current working directory as
-"example.png". The figure that was created will be left open at the end of the run.
-
-If you don't specify a filename, then :py:class:`SavedFigure` will look for a label for your figures (set with
-:py:meth:`matplotlib.figure.Figure.set_label`).
-
-Applying Styles
-~~~~~~~~~~~~~~~
-
-To apply one or more stylesheets to the :py:class:`SavedFigure`, just pass them as the keyword parameter *stle*::
-
-    with SavedFigure("example.png", style=["stoner","nature"]):
-        fig, ax = plt.subplots()
-        ax.plot(x_data, y_data)
-
-Alternatively, if you want to stop :py:class:`SavedFigure` from messing with the existing style parameters, pass False to *style*::
-
-    with SavedFigure("example.png", style=False):
-        fig, ax = plt.subplots()
-        ax.plot(x_data, y_data)
-
-This will suppress the encapsulated :py:func:`matplotlib.style.context` context manager being used.
-
-Automatically Closing the Plot Figures
-~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-
-Once you have saved your figures to disk, you probably don't want to leave them open as eventually matplotlib will
-complain about the number of open figures. :py:class:`SavedFigure` has an *autoclose* parameter that will close all the figures
-that it has saved for you::
-
-    with SavedFigure("example.png", autoclose=True):
-        fig, ax = plt.subplots()
-        ax.plot(x_data, y_data)
-
-Setting the Format of the Saved Figure
-~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-
-Matplotlib has the ability to save figures in a variety of different formats. For scientific writing, one often wants
-to save in a vector format, such as encapsulated postscript (eps), scalable vector graphics (svg), or portable document
-format (pdf). However, when the graphics are to be used in a PowerPoint presentation (or poster), a bitmapped image
-format such as Portable Network Graphics (png) is easiest to work with.
-
-.. warning::
-    JPEG encoding is not a good choice to use due to the image artefacts it introduces. JPEG uses a wavelet encoding
-    algorithm to achieve high levels of image compression. Whilst this often works well for photographs, it handles
-    sharp changes in contrast rather poorly and produces often very visible artefacts at such features. Unfortunately,
-    scientic plots have lots of such features - axes lines, data lins, axes labels etc. and as a result JPEG encoded
-    plots do not reproduce well and should be avoided.
-
-The :py:class:`SavedFigure` context manager lets you specify the figure format(s) to use via the the *formats* parameter. This can
-be either a single string representing the desired file extension, or a list of such file extensions.  In this latter
-case, :py:class:`SavedFigure` will save multiple copies of the same figure in the different format. This can be helpful if, e.g.
-you need eps formats for a LaTeX document, but also want png images to check the figures look ok.::
-
-    with SavedFigure("example", formats=["png","pdf"]):
-        fig, ax = plt.subplots()
-        ax.plot(x_data, y_data)
-
-
-If you don't specify a format and the figure's filename has an extension, that is used for the format. Otherwise it
-defaults to 'png'. If the figure filename has an extension *and* you sepcify a format, then the extension is strippled
-and the correct extension for the format is used.
-
-The choice of formats is determined by :py:func:`matplotlib.pyplot.savefig`.
-
-Multiple Figures and SavedFigure
-~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-
-If you create multiple figures within a :py:class:`SavedFigure` context manager, it will attempt to save all of yor figures. In
-this case it is rpobably desirable to set how each figure should be named. You can do this by providing a pattern
-within the figure filename. The number of the figure being saved is substituted into a placeholder in the filename
-string like so::
-
-    with SavedFigure("example_{int}", formats=["png","pdf"]):
-        fig, ax = plt.subplots()
-        ax.plot(x_data, y_data)
-       fig, ax = plt.subplots()
-       ax.plot(x_data2, y_data2)
-
-This will then result in example_0.png and example_1.png, with the "{int}" placeholder being replaced with 0,1,2...
-
-As well as the `int` placehold you can also use:
-
-    - `alpha` or `Alpha` for lower and upper case letters (starting from `a`|)
-    - `roman` or `Roman` for lower or upper case Roman numberals (starting from 'i'!)
-
-Including Already Open Figures
-~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-
-By default :py:class:`SavedFigure` will ignore all already open figures. If you want to use the :py:class:`SavedFigure` machinery to save
-figures with adjsuted filenames and in different formats, then you can pass it the *include_open* parameter set to True
-and if will not ignore the already opened figures when saving. Note, however, it is **not** possible to retrospectively
-style figures, so already open figures will be saved with their existing formatting.::
-
-    with SavedFigure("Figure-{int}", formats=["eps","png"],
-                                            include_open=True):
-        pass
-
-Will save all of your figures as Figure-0.eps, Figure-0.png, Figure-1.eps, Figure-1.png... in one go.
-
-
-InsetPlot Context Manager
--------------------------
-
-Inset plots, where a second set of axes are included within the main axes of a figure, are often used to show either a
-detail of the main figure, or possibly an overview or a related dataset. Unfortunately, generating insets with
-matplotlib can be a little tricky as the stadnard tools to setup and position the inset plot can need a bit of work to
-avoid the inset axes clashing with the primary axes.
-
-Stonerplot's :py:class:`InsetPlot` context manager is designed to make this easier by tweakign the placement of the
-inset. It is a wrapper around :py:func:`mpl_toolkits.axes_grid1.inset_locator.inset_axes` with additional logic to
-adjust the position of the inset.::
-
-    with InsetPlot() as inset:
-        inset.plot(x, y)
-
-will create an inset that is placed int he upper-left corner of te current axes and occupies 25% of the axes
-horizontally and vertically. By default the context manager also manipulates the :py:mod:`matplotlib.pyplot`'s
-current axes so that inside the context manager the current axes are the inset plot and afterwards they are restored to
-the originally active axes.
-
-Controlling Inset Location
-~~~~~~~~~~~~~~~~~~~~~~~~~~
+For example, to open a file we might use something like::
 
-The context anager takes a *loc* parameter that defines the location of the inset. These take the same value as for
-:py:func:`matplotlib.pyplot.legend` - except there is no 'auto' setting. (For convenience any hyphens in the location
-string are replaced with spaces and everything is lower-cased).::
+    with open(filename,"r") as data_file:
+        for line in data_file:
+            ...
 
-    with InsetPlot(loc="lower right") as inset:
-        inset.plot(x, y)
+In this case, the :py:func:`open` function is being used not only to open the file for reading, but to create a
+*context manager* that will also mak sure to close the file for you when executing moves out of the enclosed block.
 
-Setting the Inset Size
-~~~~~~~~~~~~~~~~~~~~~~
-
-The *width*, *height* and *dimension* parameters control the size of the inset axes (not this does not include any axes
-labels, tick markers etc.). *width* and *height* are floating point numbers, if *dimension* is "fraction" (the default)
-then these floating point numbers represent the fraction of the parent axes size to take up with the inset axes. Thus,
-the default values are 0.25, or 25%.  If *dimension* is not "fraction" then the units for *width* and *height* are
-inches.::
-
-    with InsetPlot(width=1.1, height=0.7, dimension="inches") as inset:
-        inset.plot(x, y)
-
-
-Control of Axes
-~~~~~~~~~~~~~~~
-
-By default, the parent axes are taken to be the current axes from the current figure, but the *ax* parameter to the
-Context Manager can override this.::
-
-    with InsetPlot(ax=plt.foigure(2).gca()) as inset:
-        inset.plot(x, y)
+The other reason a context manager might be used, is to temporarily change something in the environment the code is
+running in for the duration of the enclosed lines of code. `Matplotlib <https://matplotlib.org/>`_ offers
+context managers that operate in this way to temporarily set default parameters
+(:py:func:`matplotlib.pyplot.rc_context`) or to temporarily apply stylesheets (py:func:`matplotlib.style.context`).
 
-As noted above, be default the context manager switches the current axes around so that pyplot functions will work on
-the inset inside the context manager.::
 
-    plt.plot(x_main,y_main)
-    with InsetPlot():  # Ignore the context manager's return value
-        plt.plot(x_inset,y_inset)  # On the inset axes
-    plt.xlabel("Main X") # Back on the main axes again
-    plt.ylabel("Main Y")
+Using Stoner Plots to make thesis figures
+-----------------------------------------
 
+A common task that this package is aimed towards is to prepare figures for a project report, dissertation or thesis.
+The task here is to try and make the figures look as consistent as possible so that your report/dissertation/thesis
+looks profressional. You want to make all the plots have a similar format in tems of size, fonts, colous and for the
+textual elelemtns of the plot to match the main text in size and style. Matplotlib's stylesheets help you do this, but
+they still need some work to setup. The other thing you will need to do is to save your resulting figures to disk,
+preferably in a vector format that can be easily imported into your document preparation system.
 
-StackVertical Context Manager
------------------------------
+We'll assume that you areleady have a script that uses `matplotlib <https://matplotlib.org/>`_ to make your figures. First
+you probably want to colate all the lines involved in plotting the same figure together so they can be inserted into
+a block.
 
-When comparing several quantities that have a common independent variable, using a sequence of vertically stacked plots
-can be effective. Typically each sub-plot is positioned so that the top x-axis of one panel is the bottom x-axis of the
-one above, and only the bottom x-axis of the whole stack is labelled and.
+First of all we need to import the things we're going to need::
 
-Although matplotlib's builtin features to make multiple plots on a grid have been improved in recent releases, it is
-still quite complex and getting the plots to be adjacent, whilst also not having the labels etc clash is challenging.
-:py:class:`StackVertical` is a context manager designed to make this a bit easier.::
+    import matplotlib.pyplot as plt
+    import numpy as np
+    ...
+    from stonerplots import SavedFigure
 
-    with StackVertical(3) as axes:
-        for ax,y in zip(axes, [y_data1, y_data2, y_data3]):
-            ax.plot(x, y)
+The important line here is the final one. This willgive you access to the :py:class:`SavedFigure` context manager that
+we'll be using, but also importing anything from **stonerplots** will also add some stylesheets and colours to
+matplotlib.
 
-The only required parameter to :py:class:`StackVertical` is the number of plots to stack vertically. It then returns a list of the
-:py:class:`matplotlib.axes.Axes` for each subplot - the first set of axes being the top plot and the last being the
-bottom.
+You will probably also want to set up a variable with where your figures are supposed to go::
 
-When the context manager exits, it adjusts the y-axis limits to ensure the tick markers do not interfere and reduces
-the spacing between the plots to zero so that they are adjacent.
+    from pathlib import Path
+    figures = Path("/some/path/to/your/thesis/Chapters/Chapter_1/Chapter_1_figs")
 
-Adjusting the Figure Size for the Stack
-~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+(here we are using the layout of directories that we use in our standard LaTeX thesis teplate.)
 
-BY default :py:class:`StackVertical` will look at the current figure to work out its dimensions and will then assume that this is
-the correct size for a single plot. It will then adjust the figure height to accommodate the additional stacked plots.
-The equation used for this is:
+To now make your thesis figures, you can do something like::
 
-.. math::
-   h_{new} = h_{old} (f h_{old} (N_{plots}-1)+1)
+    with SavedFigure(figures/"fig_01", style=["stoner","thesis"],
+                                formats=["png","eps"], autoclose=True):
+        fig.ax = plt.subplots()
+        ... # all your plotting commands
+        ... # But don't plt.close() your figure!
 
-with :math:`f` being a fraction of the old plot size set by the *adjust_figsize* parameter to :py:class:`StackVertical`.
-If this is left at the default value of `True`, then :math:`f` is set to 0.6 and to 0 if *adjust_figsize* is `False`.
+When this executes you will find two files in your figures directory - `fig_01.png` and `fig_01.eps`. (If you are using
+pdflatex, you might prefer to have `pdf` rather than `eps` figures). Let's breakdown what that call to
+:py:class:`SavedFigure` is doing.
 
-Typically stacked plots have a bigger aspect ratio (width:height) than a single plot.::
+The first parameter is just the filename - minus the extension as we'll be adding that by specifying the formats.
 
-    with StackVertical(3, adjust_figsize=0.5) as axes:
-        for ax,y in zip(axes, [y_data1, y_data2, y_data3]):
-            ax.plot(x, y)
+The next parameter is the matplotlib stylesheets to use. The two sheeets here, `stoner` and `thesis` are included with
+Stoner Plots and were made available as soon as we imported :py:class:`SavedFigure` above. Matplotlib stylesheets are
+ummulative - so what you get here is the settings from the `stoner` style sheet and then any changed settings from
+the `thesis` stylesheet. These two style sheets together are designed to make a figure that fits in well with the
+`Condensed Matter Group's thesis template <https://github.com/stonerlab/Thesis-template>`_.
 
-Setting Common (Shared) axes
-~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+After specifying the *style* to use, we specify the *formats* to save the figure files in. Here we are asking for both
+`png` and `eps` formats. Finally we ask SavedFigure to close any figures opened after it has saved them with the
+*autoclose* parameter.
 
-By default :py:class:`StackVertical` will set the x-axis to be shared between all the plots and the y-axis of each plot to be
-independent. The *sharex* and *sharey* parameters control this. When the plots are adjacent it probably doesn't make
-sense to not share the x-axis though!::
 
-    with StackVertical(3, sharey=True) as axes:
-        for ax,y in zip(axes, [y_data1, y_data2, y_data3]):
-            ax.plot(x, y)
+.. image:: ../../examples/figures/fig02h_0.png
+  :alt: Thesis style figure
+  :align: center
 
-Labelling the Panels
-~~~~~~~~~~~~~~~~~~~~
+This is an example of a figure produces with a combination of `stoner` and `thesis` stylesheets.
 
-A common requirement of a multi-panel figure is to label the individual sets of axes (a), (b)... or similar. This is
-supported by the *label_panels* parameter. If this takes the value `True` then each set of axes is labelled '(a)',
-'(b)' and so on. For added control, the parameter can also take a string with a similar format to that used in
-:py:class:`SavedFigure` above. Placeholders such as {Alpha} or {roman} can be used and will give the axes number.::
+For the full details see the :doc:`SavedFigure Guide<savedfigure>`.
 
-    with StackVertical(3, label_panels=True) as axes:
-        for ax,y in zip(axes, [y_data1, y_data2, y_data3]):
-            ax.plot(x, y)
+Preparing a Figure for a Paper
+------------------------------
 
-Some journals, e.g. Science, also want the label to be in bold font, and :py:class:`StackVertical` supports passing the font...
-jeyword arguments to control the font size and appearance.::
+Suppose that having gotten your python code to make a nice figure for your thesis or report, you now want to use it in
+a paper submission. The general advice from scientifc journals is to prepare your figures as vector format files at as
+close to the final size as you can. Unfortunately, different journals have different house styles (in terms of exact
+figure sizes, font size and choice and so on) - so potentially there could be a lot of work sorting out the formatting
+details that could be better spent writing good text.
 
-    with StackVertical(3, label_panels='{Alpha}', fontweight='bold') as axes:
-        for ax,y in zip(axes, [y_data1, y_data2, y_data3]):
-            ax.plot(x, y)
+Stoner Plots comes with stylesheets that are set up for the common Physics journal families such as APS, AIP, IEEE etc.
+This makes switching from a figure for your thesis to a digure for a paper a matter of changing one line.::
 
+    with SavedFigure(figures/"fig_01", style=["stoner","ieee"],
+                                formats=["png","eps"], autoclose=True):
+        fig.ax = plt.subplots()
+        ... # all your plotting commands
+        ... # But don't plt.close() your figure!
 
-Specifying a Figure
-~~~~~~~~~~~~~~~~~~~
+Here, by simply changing the style from `thesis` to `aps` we reset the figure size, all of the fonts, and other details
+of the formatting.
 
-The default is to use the current matplotlib figure, but by passing the *figure* parameter into the :py:class:`StackVertical`
-context manager it will use that figure instead.::
+.. image:: ../../examples/figures/fig02a.png
+  :alt: IEEE format figure
+  :align: center
 
-    with StackVertical(3, figure=2) as axes:
-        for ax,y in zip(axes, [y_data1, y_data2, y_data3]):
-            ax.plot(x, y)
+This is what the figure looks like in IEEE format.
 
-The *figure* parameter can be either a :py:class:`matplotlib.figure.Figure` or a figure number or figure label. Within
-the context manager, the current figure is set to be figure specified by the *figure* parameter. The previously active
-figure is reset as active when the context manager exits.
-
-Not Joining the Plots
+Double Column Figures
 ~~~~~~~~~~~~~~~~~~~~~
 
-Although it is envisaged that the main use of the :py:class:`StackVertical` context manager is to make plots with shared x-axes and
-sitting adjacent to each other, setting the *joined* parameter to `False` will stop the post-plotting re-sizing and
-adjustment of the y-limits and therefore set the plots as separate enties.::
-
-    with StackVertical(3, joined=False) as axes:
-        for ax,y in zip(axes, [y_data1, y_data2, y_data3]):
-            ax.plot(x, y)
-
-MultiPanel Context Manager
---------------------------
-
-Another common requirement when writing papers and theses is to create a figure with several distinct panels shwing
-different (related) datasets. In this case, the :py:class:`MultiPanel` context manager works in a very analogous way to the
-:py:class:`StackVertical` context manager.::
+Sometimes a figure won't work wehen fitted into a single column of a two column journal. The Stoner Plots stylesheets
+include some that change the figure sizes to be suitable for 1 1/2 or 2 column formats.::
 
-    with MultiPanel((2,2)) as axes:
-    for ax,x,y in zip (axes,[x1,x2,x3,x4],[y1,y2,y3,y4]):
-        ax.plot(x,y)
+    with SavedFigure(figures/"fig_01", style=["stoner","aps", "aps2"],
+                                formats=["png","eps"], autoclose=True):
+        fig.ax = plt.subplots()
+        ... # all your plotting commands
+        ... # But don't plt.close() your figure!
+
+Note that the extra `aps2` stylesheet is used **in conjunction** to the `stoner` and `aps` stylesheets.
+
+Preparing Poster or Presentation Figures
+----------------------------------------
+
+Having made your nice figures for your thesis and possibly a paper, you are likley to also want to use them for a talk
+or poster. Again, the use of stylesheets lets you quickly swiotch formatting settings to be appropriate. For posters
+and presentations, the main features are that you need to increase the size of all of the plot elements (lines, symbols
+, fonts etc.). Generally we use something like PowerPoint to make posters and presentation (you can use LaTeX if you
+have particularly masochistic tendencies!) and the easiest way to import the figures is as `.png` files.::
+
+    with SavedFigure(figures/"fig_01.png", style=["stoner","[poster"], autoclose=True):
+        fig.ax = plt.subplots()
+        ... # all your plotting commands
+        ... # But don't plt.close() your figure!
+
+The `poster` stylesheet also increases the dpi of the image so that it will look good when printed on A0, albeit at the
+expense of rather large images!
+
+Similarly to the `poster` style there is a `presentation` style that makes figures suitable for placing into a standard
+presentation. The defautl is make a plot that occupies the whole slide, but there is a `presentation_sm` style that
+keeps the font sizes, lines etc) but reduces the size so you can fit two such plots on a slide.::
+
+    with SavedFigure(figures/"fig_01.png",
+                style=["stoner","presentation", "presentation_sm"], autoclose=True):
+        fig.ax = plt.subplots()
+        ... # all your plotting commands
+        ... # But don't plt.close() your figure!
+
+If you want to have a dark background to your presentation, then there is a `stoner_dark` stylesheet that sets colours
+appropriately. One feature of dark plots in presentations is that the light-on-dark elements look heavier or bolder
+than dark-on-light and so `presentation_dark` adjusts elements to make the overal weight look similar.::
+
+    with SavedFigure(figures/"fig_01.png",
+        style=["stoner","stoner_dark", "presentation", "presentation_dark"], autoclose=True):
+        fig.ax = plt.subplots()
+        ... # all your plotting commands
+        ... # But don't plt.close() your figure!
+
+Double and Multi-Panel Figures
+------------------------------
+
+When you want your reader/examiner to compare several related datasets, a multi-panel figure of some description can
+be a useful way to show the data.
+
+If you have several quantities that all functions of the same independent variable, and plotting them all on a single
+set of axes would be overly complex, a stack of plots with a common x-axis can be a good choice. This can be a bit
+awkward to achieve in matplotlib and so StonerPlots offers another context manager that makes this considerably easier.
 
-The only required parameter is the number of panels to show. This can be either a tuple of (n_rows,n_cols) or an
-integer specifying a number of columns (number of rows is assumed to be one in this case.)
-
-Optional Parameters
-~~~~~~~~~~~~~~~~~~~
+StackVertical Context Manager
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
-The *figure*, *sharex*, *sharey* and *label_panels* work exactly as for the :py:class:`StackVertical` Context manager
-described above, except that the default is not to share any axes.
+In this scenario you have several sets of plotting lines for each quantity ad just need to arrange the plots in a stack
+with the top of one plot being the bottom of the next.::
 
-The *adjust_figsize* parameter lets you specify a tuple to give different expansion factors for width and height. The
-default value is to expand the width by exactly the number of columns and the height by the height of one row + 80% of
-additional rows. Since full-page width figures are more than double a single column, it may be useful to do something
-like:
+    with SavedFigure("stacked.pong",style="stoner"):
+        plt.figure() # Create the figure in the stoner style
+        with StackVertical(3) as axes:  # create a stack of three plots
+            ax1,ax2,ax3=axes # Unpack them to separae variables
+            ax1.plot(...)
+            ax2.plot(...)
+            ax3.plot(...)
+
+The :py:class:`SavedFigure` context manager is doing its usual thing here (note the style can be given as a simple
+string). The :py:class:`StackVertical` context manager does the magic. When it is initially called, by default it will
+adjust the figure height to make space for multiple plots. All you need to do is to tell it the number of plots that
+should be stacked in the figure. Again, by default, Lpy:class:`StackVertical` will also label each plot (a), (b).. to
+help identify each subplot in the figure caption. The return value from :py:class:`StackVertical` is a list of the plot
+axes, starting from the top of the figure.
+
+.. image:: ../../examples/figures/fig7b.png
+  :alt: Stacked Plot
+  :align: center
+
+See :doc:`Stacked Plots<stackvertical>` for full details of :py:class:`StackVertical`.
+
+.. note::
+    :py:class:`StackVertical` will only adjust the plot positions togther when it exits - the reason for this is that
+    it is only when plotting is finished that it can work out how to move the plots together for the stack. In
+    particular, it will adjut the y-limits so that y-axis tick labels do not extend beyond the frame of the axes. A0
+    However, if the y-axis label is longer than the axis then the plots will never be properly adjacent and manual
+    addition of line breaks in the axis label may be required.
 
-    with SavedFigure("example.png",stle=["stoner","aip","aip2"]):
-        with MultiPanel((2,2),adjust_figsize=(0,0.12)) as axes:
-            for ax,x,y in zip (axes,[x1,x2,x3,x4],[y1,y2,y3,y4]):
-                ax.plot(x,y)
+Side-bu-side Multi-panel Figures
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
-To make a genuinely full width x 2 single plots high figure.
+Another common requirement is to show several related sets of data together that do not share a common variable, and in
+this case a multi-panel figure can be a good option. For this, Stoner Plots ships with a :py:class:`MulitPanel`
+context manager.::
+
+    with SavedFigure("multi_panel.pong",style="stoner"):
+        plt.figure() # Create the figure in the stoner style
+        with MultiPanel(2) as axes:  # create 2 figures next to each other
+            ax1,ax2=axes # Unpack them to separae variables
+            ax1.plot(...)
+            ax2.plot(...)
+
+As with the previous example, :py:class:`SavedFigure` handles the stylesheets and figure capture, whilst
+:py:class:`MiltiPanel` creates and labels the sub-plot axes. The parameters for this are closely related to that for
+:py:class:`StackVertical`, except the initial parameter can either be a single integer (representing the number of
+plots to place beside each other), or a tuple of rows,columns of sub-plats.
+
+.. image:: ../../examples/figures/fig02h_1.png
+  :alt: A single row of 2 sub-plats created from MultiPanel
+  :align: center
+
+See `Multi Panel Plots<multipanel>` for full details of the :py:class:`MultiPanel` context manager.
+
+
+Inset Plots
+-----------
+
+The final scenario where you might need to show related datasets is where an inset is required to show a detail, or
+perhaps an overview of the main plot axes. This again can be a fiddle with matplotlib to get insets that are placed
+correctly without overlapping the parent axes. :py:class:`InsetPlot` can be used here.::
+
+    with SavedFigure("multi_panel.pong",style="stoner"):
+        fig,ax = plt.subplots()
+        ax.plot(x_main,y_main)
+        ...
+        with InsetPlot() as inset:
+            inset.plot(x_inset,y_inset)
+            ...
+
+:py:class:`InsetPlot` doesn't need any parameters, but it is possible to control where the inset gets placed, and its
+size relative to the parent axes. See `Inset Plots<insetplot>` for the full explanation.
+
+.. toctree::
+   :maxdepth: 2
+
+   Saving Figures <savedfigure>
+   Stacked Plots <stackvertical>
+   Multi-Panel Plots <multipanel>
+   Inset Plots <insetplot>
```

### Comparing `StonerPlots-1.3.0/examples/figures/fig01b.png` & `StonerPlots-1.3.1/examples/figures/fig01b.png`

 * *Files identical despite different names*

### Comparing `StonerPlots-1.3.0/examples/figures/fig02a.png` & `StonerPlots-1.3.1/examples/figures/fig02a.png`

 * *Files identical despite different names*

### Comparing `StonerPlots-1.3.0/examples/figures/fig02b.pdf` & `StonerPlots-1.3.1/examples/figures/fig02b.pdf`

 * *Files identical despite different names*

### Comparing `StonerPlots-1.3.0/examples/figures/fig02b.png` & `StonerPlots-1.3.1/examples/figures/fig02b.png`

 * *Files identical despite different names*

### Comparing `StonerPlots-1.3.0/examples/figures/fig02c.png` & `StonerPlots-1.3.1/examples/figures/fig02c.png`

 * *Files identical despite different names*

### Comparing `StonerPlots-1.3.0/examples/figures/fig02d.png` & `StonerPlots-1.3.1/examples/figures/fig02d.png`

 * *Files identical despite different names*

### Comparing `StonerPlots-1.3.0/examples/figures/fig02e.png` & `StonerPlots-1.3.1/examples/figures/fig02e.png`

 * *Files identical despite different names*

### Comparing `StonerPlots-1.3.0/examples/figures/fig02f.png` & `StonerPlots-1.3.1/examples/figures/fig02f.png`

 * *Files identical despite different names*

### Comparing `StonerPlots-1.3.0/examples/figures/fig02g.png` & `StonerPlots-1.3.1/examples/figures/fig02g.png`

 * *Files identical despite different names*

### Comparing `StonerPlots-1.3.0/examples/figures/fig03.png` & `StonerPlots-1.3.1/examples/figures/fig03.png`

 * *Files identical despite different names*

### Comparing `StonerPlots-1.3.0/examples/figures/fig04a.png` & `StonerPlots-1.3.1/examples/figures/fig04a.png`

 * *Files identical despite different names*

### Comparing `StonerPlots-1.3.0/examples/figures/fig04b.png` & `StonerPlots-1.3.1/examples/figures/fig04b.png`

 * *Files identical despite different names*

### Comparing `StonerPlots-1.3.0/examples/figures/fig04c.png` & `StonerPlots-1.3.1/examples/figures/fig04c.png`

 * *Files identical despite different names*

### Comparing `StonerPlots-1.3.0/examples/figures/fig04d.png` & `StonerPlots-1.3.1/examples/figures/fig04d.png`

 * *Files identical despite different names*

### Comparing `StonerPlots-1.3.0/examples/figures/fig04e.png` & `StonerPlots-1.3.1/examples/figures/fig04e.png`

 * *Files identical despite different names*

### Comparing `StonerPlots-1.3.0/examples/figures/fig04f.png` & `StonerPlots-1.3.1/examples/figures/fig04f.png`

 * *Files identical despite different names*

### Comparing `StonerPlots-1.3.0/examples/figures/fig04g.png` & `StonerPlots-1.3.1/examples/figures/fig04g.png`

 * *Files identical despite different names*

### Comparing `StonerPlots-1.3.0/examples/figures/fig04h.png` & `StonerPlots-1.3.1/examples/figures/fig04h.png`

 * *Files identical despite different names*

### Comparing `StonerPlots-1.3.0/examples/figures/fig05a.png` & `StonerPlots-1.3.1/examples/figures/fig05a.png`

 * *Files identical despite different names*

### Comparing `StonerPlots-1.3.0/examples/figures/fig05b.png` & `StonerPlots-1.3.1/examples/figures/fig05b.png`

 * *Files identical despite different names*

### Comparing `StonerPlots-1.3.0/examples/figures/fig05c.png` & `StonerPlots-1.3.1/examples/figures/fig05c.png`

 * *Files identical despite different names*

### Comparing `StonerPlots-1.3.0/examples/figures/fig05d.png` & `StonerPlots-1.3.1/examples/figures/fig05d.png`

 * *Files identical despite different names*

### Comparing `StonerPlots-1.3.0/examples/figures/fig05e.png` & `StonerPlots-1.3.1/examples/figures/fig05e.png`

 * *Files identical despite different names*

### Comparing `StonerPlots-1.3.0/examples/figures/fig05f.png` & `StonerPlots-1.3.1/examples/figures/fig05f.png`

 * *Files identical despite different names*

### Comparing `StonerPlots-1.3.0/examples/figures/fig06.png` & `StonerPlots-1.3.1/examples/figures/fig06.png`

 * *Files identical despite different names*

### Comparing `StonerPlots-1.3.0/examples/figures/fig07a.png` & `StonerPlots-1.3.1/examples/figures/fig07a.png`

 * *Files identical despite different names*

### Comparing `StonerPlots-1.3.0/examples/figures/fig7b.png` & `StonerPlots-1.3.1/examples/figures/fig7b.png`

 * *Files identical despite different names*

### Comparing `StonerPlots-1.3.0/examples/figures/fig7c.png` & `StonerPlots-1.3.1/examples/figures/fig7c.png`

 * *Files identical despite different names*

### Comparing `StonerPlots-1.3.0/examples/matplotlibrc` & `StonerPlots-1.3.1/examples/matplotlibrc`

 * *Files identical despite different names*

### Comparing `StonerPlots-1.3.0/examples/plot_examples/__init__.py` & `StonerPlots-1.3.1/examples/plot_examples/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,14 +7,15 @@
     "default_plot_ieee",
     "default_plot_aps",
     "default_plot_aip",
     "default_plot_iop",
     "default_plot_nature",
     "default_plot_aps_1_5_column",
     "default_plot_aps_2_column",
+    "default_plot_thesis",
     # 3 Formats
     "scatter_plot",
     # 4 Colour Schemes
     "default_plot_std_colours",
     "default_plot_bright",
     "default_plot_high_contrast",
     "default_plot_high_vis",
```

### Comparing `StonerPlots-1.3.0/examples/plot_examples/default_plot_aip.py` & `StonerPlots-1.3.1/examples/plot_examples/default_plot_aip.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # -*- coding: utf-8 -*-
 """Demonstrate the SavedFigure context manager and default Stoner plot style in AIP format."""
 import matplotlib.pyplot as plt
 
 from stonerplots import SavedFigure
 
-from .common import x, model, pparam, figures
+from common import x, model, pparam, figures
 
 with SavedFigure(figures / "fig02c.png", style=["stoner", "aip"], autoclose=True):
     fig, ax = plt.subplots()
     for p in [10, 15, 20, 30, 50, 100]:
         ax.plot(x, model(x, p), label=p, marker="")
     ax.legend(title="Order")
     ax.autoscale(tight=True)
```

### Comparing `StonerPlots-1.3.0/examples/plot_examples/default_plot_aps.py` & `StonerPlots-1.3.1/examples/plot_examples/default_plot_aps.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # -*- coding: utf-8 -*-
 """Demonstrate the SavedFigure context manager and default Stoner plot style in APS format."""
 import matplotlib.pyplot as plt
 
 from stonerplots import SavedFigure
 
-from .common import x, model, pparam, figures
+from common import x, model, pparam, figures
 
 with SavedFigure(figures / "fig02b.png", style=["stoner", "aps"], autoclose=True, formats=["png", "pdf"]):
     fig, ax = plt.subplots()
     for p in [10, 15, 20, 30, 50, 100]:
         ax.plot(x, model(x, p), label=p, marker="")
     ax.legend(title="Order")
     ax.autoscale(tight=True)
```

### Comparing `StonerPlots-1.3.0/examples/plot_examples/default_plot_aps_1_5_column.py` & `StonerPlots-1.3.1/examples/plot_examples/default_plot_aps_2_column.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # -*- coding: utf-8 -*-
-"""Demonstrate the SavedFigure context manager and default Stoner plot style in APS format 1.5 columns."""
+"""Demonstrate the SavedFigure context manager and default Stoner plot style in APS format 2 columns."""
 import matplotlib.pyplot as plt
 
 from stonerplots import SavedFigure
 
-from .common import x, model, pparam, figures
+from common import x, model, pparam, figures
 
-with SavedFigure(figures / "fig02f.png", style=["stoner", "aps", "aps1.5"], autoclose=True):
+with SavedFigure(figures / "fig02g.png", style=["stoner", "aps", "aps2"], autoclose=True):
     fig, ax = plt.subplots()
     for p in [10, 15, 20, 30, 50, 100]:
         ax.plot(x, model(x, p), label=p, marker="")
     ax.legend(title="Order")
     ax.autoscale(tight=True)
     ax.set(**pparam)
```

### Comparing `StonerPlots-1.3.0/examples/plot_examples/default_plot_aps_2_column.py` & `StonerPlots-1.3.1/examples/plot_examples/default_plot_high_contrast.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # -*- coding: utf-8 -*-
-"""Demonstrate the SavedFigure context manager and default Stoner plot style in APS format 2 columns."""
+"""Demonstrate the SavedFigure context manager and default Stoner plot style with high-contrast colour scheme."""
 import matplotlib.pyplot as plt
 
 from stonerplots import SavedFigure
 
-from .common import x, model, pparam, figures
+from common import x, model, pparam, figures
 
-with SavedFigure(figures / "fig02g.png", style=["stoner", "aps", "aps2"], autoclose=True):
+with SavedFigure(figures / "fig04c.png", style=["stoner", "high-contrast"], autoclose=True):
     fig, ax = plt.subplots()
     for p in [10, 15, 20, 30, 50, 100]:
-        ax.plot(x, model(x, p), label=p, marker="")
+        ax.plot(x, model(x, p), label=p)
     ax.legend(title="Order")
     ax.autoscale(tight=True)
     ax.set(**pparam)
```

### Comparing `StonerPlots-1.3.0/examples/plot_examples/default_plot_bright.py` & `StonerPlots-1.3.1/examples/plot_examples/default_plot_bright.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # -*- coding: utf-8 -*-
 """Demonstrate the SavedFigure context manager and default Stoner plot style with bright colour scheme."""
 import matplotlib.pyplot as plt
 
 from stonerplots import SavedFigure
 
-from .common import x, model, pparam, figures
+from common import x, model, pparam, figures
 
 with SavedFigure(figures / "fig04b.png", style=["stoner", "bright"], autoclose=True):
     fig, ax = plt.subplots()
     for p in [10, 15, 20, 30, 50, 100]:
         ax.plot(x, model(x, p), label=p)
     ax.legend(title="Order")
     ax.autoscale(tight=True)
```

### Comparing `StonerPlots-1.3.0/examples/plot_examples/default_plot_high_contrast.py` & `StonerPlots-1.3.1/examples/plot_examples/default_plot_retro.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # -*- coding: utf-8 -*-
-"""Demonstrate the SavedFigure context manager and default Stoner plot style with high-contrast colour scheme."""
+"""Demonstrate the SavedFigure context manager and default Stoner plot style with retro colour scheme."""
 import matplotlib.pyplot as plt
 
 from stonerplots import SavedFigure
 
-from .common import x, model, pparam, figures
+from common import x, model, pparam, figures
 
-with SavedFigure(figures / "fig04c.png", style=["stoner", "high-contrast"], autoclose=True):
+with SavedFigure(figures / "fig04g.png", style=["stoner", "retro"], autoclose=True):
     fig, ax = plt.subplots()
     for p in [10, 15, 20, 30, 50, 100]:
         ax.plot(x, model(x, p), label=p)
     ax.legend(title="Order")
     ax.autoscale(tight=True)
     ax.set(**pparam)
```

### Comparing `StonerPlots-1.3.0/examples/plot_examples/default_plot_high_vis.py` & `StonerPlots-1.3.1/examples/plot_examples/default_plot_high_vis.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # -*- coding: utf-8 -*-
 """Demonstrate the SavedFigure context manager and default Stoner plot style with high-vis colour scheme."""
 import matplotlib.pyplot as plt
 
 from stonerplots import SavedFigure
 
-from .common import x, model, pparam, figures
+from common import x, model, pparam, figures
 
 with SavedFigure(figures / "fig04d.png", style=["stoner", "high-vis"], autoclose=True):
     fig, ax = plt.subplots()
     for p in [10, 15, 20, 30, 50, 100]:
         ax.plot(x, model(x, p), label=p)
     ax.legend(title="Order")
     ax.autoscale(tight=True)
```

### Comparing `StonerPlots-1.3.0/examples/plot_examples/default_plot_ieee.py` & `StonerPlots-1.3.1/examples/plot_examples/default_plot_ieee.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # -*- coding: utf-8 -*-
 """Demonstrate the SavedFigure context manager and default Stoner plot style in IEEE format."""
 import matplotlib.pyplot as plt
 
 from stonerplots import SavedFigure
 
-from .common import x, model, pparam, figures
+from common import x, model, pparam, figures
 
 with SavedFigure(figures / "fig02a.png", style=["stoner", "ieee"], autoclose=True):
     fig, ax = plt.subplots()
     for p in [10, 15, 20, 30, 50, 100]:
         ax.plot(x, model(x, p), label=p, marker="")
     ax.legend(title="Order")
     ax.autoscale(tight=True)
```

### Comparing `StonerPlots-1.3.0/examples/plot_examples/default_plot_iop.py` & `StonerPlots-1.3.1/examples/plot_examples/default_plot_iop.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # -*- coding: utf-8 -*-
 """Demonstrate the SavedFigure context manager and default Stoner plot style in IOP format."""
 import matplotlib.pyplot as plt
 
 from stonerplots import SavedFigure
 
-from .common import x, model, pparam, figures
+from common import x, model, pparam, figures
 
 with SavedFigure(figures / "fig02d.png", style=["stoner", "iop"], autoclose=True):
     fig, ax = plt.subplots()
     for p in [10, 15, 20, 30, 50, 100]:
         ax.plot(x, model(x, p), label=p, marker="")
     ax.legend(title="Order")
     ax.autoscale(tight=True)
```

### Comparing `StonerPlots-1.3.0/examples/plot_examples/default_plot_latex.py` & `StonerPlots-1.3.1/examples/plot_examples/default_plot_muted.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # -*- coding: utf-8 -*-
-"""Demonstrate the SavedFigure context manager and default Stoner plot style with latex enabled."""
+"""Demonstrate the SavedFigure context manager and default Stoner plot style with muted colour scheme."""
 import matplotlib.pyplot as plt
 
 from stonerplots import SavedFigure
 
-from .common import x, model, pparam, figures
+from common import x, model, pparam, figures
 
-with SavedFigure(figures / "fig01b.png", style=["stoner", "latex"], autoclose=True):
+with SavedFigure(figures / "fig04f.png", style=["stoner", "muted"], autoclose=True):
     fig, ax = plt.subplots()
     for p in [10, 15, 20, 30, 50, 100]:
-        ax.plot(x, model(x, p), label=p, marker="")
+        ax.plot(x, model(x, p), label=p)
     ax.legend(title="Order")
     ax.autoscale(tight=True)
     ax.set(**pparam)
```

### Comparing `StonerPlots-1.3.0/examples/plot_examples/default_plot_light.py` & `StonerPlots-1.3.1/examples/plot_examples/default_plot_light.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # -*- coding: utf-8 -*-
 """Demonstrate the SavedFigure context manager and default Stoner plot style with light colour scheme."""
 import matplotlib.pyplot as plt
 
 from stonerplots import SavedFigure
 
-from .common import x, model, pparam, figures
+from common import x, model, pparam, figures
 
 with SavedFigure(figures / "fig04e.png", style=["stoner", "light"], autoclose=True):
     fig, ax = plt.subplots()
     for p in [10, 15, 20, 30, 50, 100]:
         ax.plot(x, model(x, p), label=p)
     ax.legend(title="Order")
     ax.autoscale(tight=True)
```

### Comparing `StonerPlots-1.3.0/examples/plot_examples/default_plot_muted.py` & `StonerPlots-1.3.1/examples/plot_examples/default_plot_nature.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # -*- coding: utf-8 -*-
-"""Demonstrate the SavedFigure context manager and default Stoner plot style with muted colour scheme."""
+"""Demonstrate the SavedFigure context manager and default Stoner plot style in Nature format."""
 import matplotlib.pyplot as plt
 
 from stonerplots import SavedFigure
 
-from .common import x, model, pparam, figures
+from common import x, model, pparam, figures
 
-with SavedFigure(figures / "fig04f.png", style=["stoner", "muted"], autoclose=True):
+with SavedFigure(figures / "fig02e.png", style=["stoner", "nature"], autoclose=True):
     fig, ax = plt.subplots()
     for p in [10, 15, 20, 30, 50, 100]:
-        ax.plot(x, model(x, p), label=p)
+        ax.plot(x, model(x, p), label=p, marker="")
     ax.legend(title="Order")
     ax.autoscale(tight=True)
     ax.set(**pparam)
```

### Comparing `StonerPlots-1.3.0/examples/plot_examples/default_plot_nature.py` & `StonerPlots-1.3.1/examples/plot_examples/default_plot_latex.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # -*- coding: utf-8 -*-
-"""Demonstrate the SavedFigure context manager and default Stoner plot style in Nature format."""
+"""Demonstrate the SavedFigure context manager and default Stoner plot style with latex enabled."""
 import matplotlib.pyplot as plt
 
 from stonerplots import SavedFigure
 
-from .common import x, model, pparam, figures
+from common import x, model, pparam, figures
 
-with SavedFigure(figures / "fig02e.png", style=["stoner", "nature"], autoclose=True):
+with SavedFigure(figures / "fig01b.png", style=["stoner", "latex"], autoclose=True):
     fig, ax = plt.subplots()
     for p in [10, 15, 20, 30, 50, 100]:
         ax.plot(x, model(x, p), label=p, marker="")
     ax.legend(title="Order")
     ax.autoscale(tight=True)
     ax.set(**pparam)
```

### Comparing `StonerPlots-1.3.0/examples/plot_examples/default_plot_retro.py` & `StonerPlots-1.3.1/examples/plot_examples/small_presentation_plot.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 # -*- coding: utf-8 -*-
-"""Demonstrate the SavedFigure context manager and default Stoner plot style with retro colour scheme."""
+"""Demonstrate the SavedFigure context manager and smaller size presentation format."""
 import matplotlib.pyplot as plt
 
 from stonerplots import SavedFigure
 
-from .common import x, model, pparam, figures
+from common import x, model, pparam, figures
 
-with SavedFigure(figures / "fig04g.png", style=["stoner", "retro"], autoclose=True):
+with SavedFigure(figures / "fig05d.png", style=["stoner", "presentation", "presentation_sm"], autoclose=True):
     fig, ax = plt.subplots()
     for p in [10, 15, 20, 30, 50, 100]:
-        ax.plot(x, model(x, p), label=p)
+        line = ax.plot(x, model(x, p), label=p, marker="")
+        ax.plot(x[::5], model(x[::5], p), label=None, c=line[0].get_color(), linestyle="")
     ax.legend(title="Order")
     ax.autoscale(tight=True)
     ax.set(**pparam)
```

### Comparing `StonerPlots-1.3.0/examples/plot_examples/default_plot_std_colours.py` & `StonerPlots-1.3.1/examples/plot_examples/default_plot_std_colours.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # -*- coding: utf-8 -*-
 """Demonstrate the SavedFigure context manager and default Stoner plot style with standard colours."""
 import matplotlib.pyplot as plt
 
 from stonerplots import SavedFigure
 
-from .common import x, model, pparam, figures
+from common import x, model, pparam, figures
 
 with SavedFigure(figures / "fig04a.png", style=["stoner", "std-colours"], autoclose=True):
     fig, ax = plt.subplots()
     for p in [10, 15, 20, 30, 50, 100]:
         ax.plot(x, model(x, p), label=p)
     ax.legend(title="Order")
     ax.autoscale(tight=True)
```

### Comparing `StonerPlots-1.3.0/examples/plot_examples/default_plot_vibrant.py` & `StonerPlots-1.3.1/examples/plot_examples/presentation_plot.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 # -*- coding: utf-8 -*-
-"""Demonstrate the SavedFigure context manager and default Stoner plot style with vibrant colour scheme."""
+"""Demonstrate the SavedFigure context manager and presentation format."""
 import matplotlib.pyplot as plt
 
 from stonerplots import SavedFigure
 
-from .common import x, model, pparam, figures
+from common import x, model, pparam, figures
 
-with SavedFigure(figures / "fig04h.png", style=["stoner", "vibrant"], autoclose=True):
+with SavedFigure(figures / "fig05c.png", style=["stoner", "presentation"], autoclose=True):
     fig, ax = plt.subplots()
     for p in [10, 15, 20, 30, 50, 100]:
-        ax.plot(x, model(x, p), label=p)
+        line = ax.plot(x, model(x, p), label=p, marker="")
+        ax.plot(x[::5], model(x[::5], p), label=None, c=line[0].get_color(), linestyle="")
     ax.legend(title="Order")
     ax.autoscale(tight=True)
     ax.set(**pparam)
```

### Comparing `StonerPlots-1.3.0/examples/plot_examples/inset_plot.py` & `StonerPlots-1.3.1/examples/plot_examples/inset_plot.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # -*- coding: utf-8 -*-
 """Demonstrate the SavedFigure context manager and InsetPlot context manager."""
 import matplotlib.pyplot as plt
 
 from stonerplots import SavedFigure, InsetPlot
 
-from .common import x, model, pparam, figures
+from common import x, model, pparam, figures
 
 with SavedFigure(figures / "fig07a.png", style=["stoner"], autoclose=True):
     fig, ax = plt.subplots()
     for p in [5, 10, 20, 38, 100]:
         ax.plot(x, model(x, p), label=p, marker="")
     ax.legend(title="Order", fontsize=7)
     ax.set(**pparam)
```

### Comparing `StonerPlots-1.3.0/examples/plot_examples/multi_panel_plot.py` & `StonerPlots-1.3.1/examples/plot_examples/multi_panel_plot.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # -*- coding: utf-8 -*-
 """Demonstrate the SavedFigure context manager and InsetPlot context manager."""
 import matplotlib.pyplot as plt
 
 from stonerplots import SavedFigure, MultiPanel
 
-from .common import x, model, pparam, figures
+from common import x, model, pparam, figures
 
 with SavedFigure(figures / "fig7c.png", style=["stoner","iop"], autoclose=True):
     fig = plt.figure()
     with MultiPanel((2,2)) as axes:
         for ix, ax in enumerate(axes):
             for p in [10, 30, 100]:
                 ax.plot(x, model(x, p + ix * 5), label=p + ix * 5, marker="")
```

### Comparing `StonerPlots-1.3.0/examples/plot_examples/poster_plot.py` & `StonerPlots-1.3.1/examples/plot_examples/poster_plot.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # -*- coding: utf-8 -*-
 """Demonstrate the SavedFigure context manager and poster format."""
 import matplotlib.pyplot as plt
 
 from stonerplots import SavedFigure
 
-from .common import x, model, pparam, figures
+from common import x, model, pparam, figures
 
 with SavedFigure(figures / "fig05b.png", style=["stoner", "poster"], autoclose=True):
     fig, ax = plt.subplots()
     for p in [10, 15, 20, 30, 50, 100]:
         line = ax.plot(x, model(x, p), label=p, marker="")
         ax.plot(x[::5], model(x[::5], p), label=None, c=line[0].get_color(), linestyle="")
     ax.legend(title="Order")
```

### Comparing `StonerPlots-1.3.0/examples/plot_examples/presentation_plot.py` & `StonerPlots-1.3.1/examples/plot_examples/small_presentation_dark_plot.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,20 @@
 # -*- coding: utf-8 -*-
-"""Demonstrate the SavedFigure context manager and presentation format."""
+"""Demonstrate the SavedFigure context manager and smaller size presentation format."""
 import matplotlib.pyplot as plt
 
 from stonerplots import SavedFigure
 
-from .common import x, model, pparam, figures
+from common import x, model, pparam, figures
 
-with SavedFigure(figures / "fig05c.png", style=["stoner", "presentation"], autoclose=True):
+with SavedFigure(
+    figures / "fig05e.png",
+    style=["stoner", "stoner_dark", "presentation", "presentation_sm", "presentation_dark"],
+    autoclose=True,
+):
     fig, ax = plt.subplots()
     for p in [10, 15, 20, 30, 50, 100]:
         line = ax.plot(x, model(x, p), label=p, marker="")
         ax.plot(x[::5], model(x[::5], p), label=None, c=line[0].get_color(), linestyle="")
     ax.legend(title="Order")
     ax.autoscale(tight=True)
     ax.set(**pparam)
```

### Comparing `StonerPlots-1.3.0/examples/plot_examples/scatter_plot.py` & `StonerPlots-1.3.1/examples/plot_examples/scatter_plot.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # -*- coding: utf-8 -*-
 """Demonstrate the SavedFigure context manager and Scatter Plot settings."""
 import matplotlib.pyplot as plt
 import numpy as np
 
 from stonerplots import SavedFigure
 
-from .common import figures
+from common import figures
 
 with SavedFigure(figures / "fig03.png", style=["stoner", "scatter", "latex"], autoclose=True):
     fig, ax = plt.subplots(figsize=(4, 4))
     ax.plot([-2, 2], [-2, 2], "k--")
     ax.fill_between([-2, 2], [-2.2, 1.8], [-1.8, 2.2], color="dodgerblue", alpha=0.2, lw=0)
     for i in range(7):
         x1 = np.random.normal(0, 0.5, 10)
```

### Comparing `StonerPlots-1.3.0/examples/plot_examples/small_presentation_dark_plot.py` & `StonerPlots-1.3.1/examples/plot_examples/stacked_plot.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,20 +1,17 @@
 # -*- coding: utf-8 -*-
-"""Demonstrate the SavedFigure context manager and smaller size presentation format."""
+"""Demonstrate the SavedFigure context manager and InsetPlot context manager."""
 import matplotlib.pyplot as plt
 
-from stonerplots import SavedFigure
+from stonerplots import SavedFigure, StackVertical
 
-from .common import x, model, pparam, figures
+from common import x, model, pparam, figures
 
-with SavedFigure(
-    figures / "fig05e.png",
-    style=["stoner", "stoner_dark", "presentation", "presentation_sm", "presentation_dark"],
-    autoclose=True,
-):
-    fig, ax = plt.subplots()
-    for p in [10, 15, 20, 30, 50, 100]:
-        line = ax.plot(x, model(x, p), label=p, marker="")
-        ax.plot(x[::5], model(x[::5], p), label=None, c=line[0].get_color(), linestyle="")
-    ax.legend(title="Order")
-    ax.autoscale(tight=True)
-    ax.set(**pparam)
+with SavedFigure(figures / "fig7b.png", style=["stoner"], autoclose=True):
+    fig = plt.figure()
+    fig.set_figheight(fig.get_figheight() * 0.6)
+    with StackVertical(3) as axes:
+        for ix, ax in enumerate(axes):
+            for p in [10, 30, 100]:
+                ax.plot(x, model(x, p + ix * 5), label=p + ix * 5, marker="")
+            ax.legend(title="Order", loc="lower right")
+            ax.set(**pparam)
```

### Comparing `StonerPlots-1.3.0/examples/plot_examples/small_presentation_plot.py` & `StonerPlots-1.3.1/examples/plot_examples/default_plot_thesis.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,16 +1,23 @@
 # -*- coding: utf-8 -*-
-"""Demonstrate the SavedFigure context manager and smaller size presentation format."""
+"""Demonstrate the SavedFigure context manager and default Stoner plot style."""
 import matplotlib.pyplot as plt
 
-from stonerplots import SavedFigure
+from stonerplots import SavedFigure, MultiPanel
 
-from .common import x, model, pparam, figures
+from common import x, model, pparam, figures
 
-with SavedFigure(figures / "fig05d.png", style=["stoner", "presentation", "presentation_sm"], autoclose=True):
+with SavedFigure(figures / "fig02h_{int}", style=["stoner", "thesis"], formats=["pdf", "png"], autoclose=True):
     fig, ax = plt.subplots()
     for p in [10, 15, 20, 30, 50, 100]:
-        line = ax.plot(x, model(x, p), label=p, marker="")
-        ax.plot(x[::5], model(x[::5], p), label=None, c=line[0].get_color(), linestyle="")
+        ax.plot(x, model(x, p), label=p, marker="")
     ax.legend(title="Order")
     ax.autoscale(tight=True)
     ax.set(**pparam)
+    fig = plt.figure()
+    with MultiPanel(2, adjust_figsize=(0, -0.25)) as axes:
+        for ix, ax in enumerate(axes):
+            for p in [10, 15, 20, 30, 50, 100]:
+                ax.plot(x, model(x, p + 2 * ix), label=p + 2 * ix, marker="")
+            ax.legend(title="Order")
+            ax.autoscale(tight=True)
+            ax.set(**pparam)
```

### Comparing `StonerPlots-1.3.0/examples/plot_examples/stacked_plot.py` & `StonerPlots-1.3.1/examples/plot_examples/default_plot_vibrant.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 # -*- coding: utf-8 -*-
-"""Demonstrate the SavedFigure context manager and InsetPlot context manager."""
+"""Demonstrate the SavedFigure context manager and default Stoner plot style with vibrant colour scheme."""
 import matplotlib.pyplot as plt
 
-from stonerplots import SavedFigure, StackVertical
+from stonerplots import SavedFigure
 
-from .common import x, model, pparam, figures
+from common import x, model, pparam, figures
 
-with SavedFigure(figures / "fig7b.png", style=["stoner"], autoclose=True):
-    fig = plt.figure()
-    fig.set_figheight(fig.get_figheight() * 0.6)
-    with StackVertical(3) as axes:
-        for ix, ax in enumerate(axes):
-            for p in [10, 30, 100]:
-                ax.plot(x, model(x, p + ix * 5), label=p + ix * 5, marker="")
-            ax.legend(title="Order", loc="lower right")
-            ax.set(**pparam)
+with SavedFigure(figures / "fig04h.png", style=["stoner", "vibrant"], autoclose=True):
+    fig, ax = plt.subplots()
+    for p in [10, 15, 20, 30, 50, 100]:
+        ax.plot(x, model(x, p), label=p)
+    ax.legend(title="Order")
+    ax.autoscale(tight=True)
+    ax.set(**pparam)
```

### Comparing `StonerPlots-1.3.0/pyproject.toml` & `StonerPlots-1.3.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `StonerPlots-1.3.0/recipe/meta.yaml` & `StonerPlots-1.3.1/recipe/meta.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 {% set name = "stonerplots" %}
-{% set version = "1.3.0" %}
+{% set version = "1.3.1" %}
 
 package:
   name: {{ name|lower }}
   version: {{ version }}
 
 source:
   path: ..
```

### Comparing `StonerPlots-1.3.0/setup.py` & `StonerPlots-1.3.1/setup.py`

 * *Files identical despite different names*

### Comparing `StonerPlots-1.3.0/src/StonerPlots.egg-info/PKG-INFO` & `StonerPlots-1.3.1/src/StonerPlots.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: StonerPlots
-Version: 1.3.0
+Version: 1.3.1
 Summary: This is a fork of scienceplots and provides a range of matplotlib styles for plotting physics...
 Author-email: Gavin Burnell <G.Burnell@leeds.ac.uk>
 Project-URL: Homepage, https://github.com/stonerlab/stonerplots/
 Project-URL: Issues, https://github.com/stonerlab/stonerplots/issues
 Keywords: matplotlib-style-sheets,matplotlib-figures,scientific-papers,thesis-template,matplotlib-styles,python
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `StonerPlots-1.3.0/src/StonerPlots.egg-info/SOURCES.txt` & `StonerPlots-1.3.1/src/StonerPlots.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -10,17 +10,22 @@
 docs/Makefile
 docs/make.bat
 docs/requirements.txt
 docs/source/api.rst
 docs/source/colours.rst
 docs/source/conf.py
 docs/source/index.rst
+docs/source/insetplot.rst
+docs/source/multipanel.rst
+docs/source/savedfigure.rst
+docs/source/stackvertical.rst
 docs/source/style-gallery.rst
 docs/source/userguide.rst
 docs/source/api/stonerplots.InsetPlot.rst
+docs/source/api/stonerplots.MultiPanel.rst
 docs/source/api/stonerplots.SavedFigure.rst
 docs/source/api/stonerplots.StackVertical.rst
 docs/source/figures/StonerLogo2.png
 docs/source/figures/colours.png
 docs/source/figures/colours10.png
 docs/source/figures/colours50.png
 docs/source/figures/colours70.png
@@ -34,14 +39,18 @@
 examples/figures/fig02b.pdf
 examples/figures/fig02b.png
 examples/figures/fig02c.png
 examples/figures/fig02d.png
 examples/figures/fig02e.png
 examples/figures/fig02f.png
 examples/figures/fig02g.png
+examples/figures/fig02h_0.pdf
+examples/figures/fig02h_0.png
+examples/figures/fig02h_1.pdf
+examples/figures/fig02h_1.png
 examples/figures/fig03.png
 examples/figures/fig04a.png
 examples/figures/fig04b.png
 examples/figures/fig04c.png
 examples/figures/fig04d.png
 examples/figures/fig04e.png
 examples/figures/fig04f.png
@@ -73,14 +82,15 @@
 examples/plot_examples/default_plot_iop.py
 examples/plot_examples/default_plot_latex.py
 examples/plot_examples/default_plot_light.py
 examples/plot_examples/default_plot_muted.py
 examples/plot_examples/default_plot_nature.py
 examples/plot_examples/default_plot_retro.py
 examples/plot_examples/default_plot_std_colours.py
+examples/plot_examples/default_plot_thesis.py
 examples/plot_examples/default_plot_vibrant.py
 examples/plot_examples/grid_plot.py
 examples/plot_examples/hi_res_plot.py
 examples/plot_examples/inset_plot.py
 examples/plot_examples/multi_panel_plot.py
 examples/plot_examples/notebook_plot.py
 examples/plot_examples/poster_plot.py
@@ -99,14 +109,15 @@
 src/stonerplots/colours.py
 src/stonerplots/context.py
 src/stonerplots/styles/notebook.mplstyle
 src/stonerplots/styles/poster.mplstyle
 src/stonerplots/styles/presentation.mplstyle
 src/stonerplots/styles/scatter.mplstyle
 src/stonerplots/styles/stoner.mplstyle
+src/stonerplots/styles/thesis.mplstyle
 src/stonerplots/styles/color/bright.mplstyle
 src/stonerplots/styles/color/high-contrast.mplstyle
 src/stonerplots/styles/color/high-vis.mplstyle
 src/stonerplots/styles/color/light.mplstyle
 src/stonerplots/styles/color/muted.mplstyle
 src/stonerplots/styles/color/retro.mplstyle
 src/stonerplots/styles/color/std-colours.mplstyle
```

### Comparing `StonerPlots-1.3.0/src/stonerplots/__init__.py` & `StonerPlots-1.3.1/src/stonerplots/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 import matplotlib.pyplot as plt
 from matplotlib.colors import _colors_full_map
 from .context import SavedFigure, InsetPlot, StackVertical, MultiPanel
 from .colours import tube_colours, tube_colours_90, tube_colours_70, tube_colours_50, tube_colours_10
 
 __all__ = ["context", "SavedFigure", "InsetPlot", "StackVertical", "MultiPanel"]
-__version__ = "1.3.0"
+__version__ = "1.3.1"
 
 # register the included stylesheet in the matplotlib style library
 stonerplots_path = Path(__file__).parent
 styles_path = stonerplots_path / "styles"
 
 # Reads styles in /styles
 stylesheets = plt.style.core.read_style_directory(str(styles_path))
```

### Comparing `StonerPlots-1.3.0/src/stonerplots/colours.py` & `StonerPlots-1.3.1/src/stonerplots/colours.py`

 * *Files identical despite different names*

### Comparing `StonerPlots-1.3.0/src/stonerplots/context.py` & `StonerPlots-1.3.1/src/stonerplots/context.py`

 * *Files 2% similar despite different names*

```diff
@@ -370,15 +370,15 @@
             extra_h = self.figsize[1] * self.adjust_figsize * (self.number - 1) + self.figsize[1]
             self.figure.set_figheight(extra_h)
         if self.label_panels:
             fig = self.figure
             for ix, ax in enumerate(self.axes):
                 title_pts = ax.title.get_fontsize()
                 ax_height = ax.bbox.transformed(fig.transFigure.inverted()).height * fig.get_figheight() * 72
-                y = (ax_height - title_pts * 1.25) / ax_height
+                y = (ax_height - title_pts * 1.5) / ax_height
 
                 ax.set_title(
                     f" {_counter(ix,self.label_panels)}", loc="left", y=y, **_filter_dict(self.kwargs, _fontargs)
                 )
         return self.axes
 
     def __exit__(self, type, value, traceback):
@@ -485,24 +485,32 @@
         self.kwargs = kwargs
 
     def __enter__(self):
         """Create the grid of axes."""
         self.gs = self.figure.add_gridspec(*self.panels, **self.kwargs)
         self.axes = self.gs.subplots(sharex=self.sharex, sharey=self.sharey)
         if self.adjust_figsize:
-            extra_h = self.figsize[1] * self.adjust_figsize[1] * (self.panels[1] - 1) + self.figsize[1]
-            self.figure.set_figheight(extra_h)
-            extra_w = self.figsize[0] * self.adjust_figsize[0] * (self.panels[0] - 1) + self.figsize[0]
+            f = self.adjust_figsize[0]
+            if f < 0:
+                extra_w = self.figsize[0] * (1 + f)
+            else:
+                extra_w = self.figsize[0] * f * (self.panels[1] - 1) + self.figsize[0]
+            f = self.adjust_figsize[1]
+            if f < 0:
+                extra_h = self.figsize[1] * (1 + f)
+            else:
+                extra_h = self.figsize[1] * f * (self.panels[0] - 1) + self.figsize[1]
             self.figure.set_figwidth(extra_w)
+            self.figure.set_figheight(extra_h)
         if self.label_panels:
             fig = self.figure
             for ix, ax in enumerate(self):
                 title_pts = ax.title.get_fontsize()
                 ax_height = ax.bbox.transformed(fig.transFigure.inverted()).height * fig.get_figheight() * 72
-                y = (ax_height - title_pts * 1.25) / ax_height
+                y = (ax_height - title_pts * 1.5) / ax_height
 
                 ax.set_title(
                     f" {_counter(ix,self.label_panels)}", loc="left", y=y, **_filter_dict(self.kwargs, _fontargs)
                 )
         return self
 
     def __exit__(self, type, value, traceback):
```

### Comparing `StonerPlots-1.3.0/src/stonerplots/styles/color/stoner_dark.mplstyle` & `StonerPlots-1.3.1/src/stonerplots/styles/color/stoner_dark.mplstyle`

 * *Files identical despite different names*

### Comparing `StonerPlots-1.3.0/src/stonerplots/styles/journals/aip.mplstyle` & `StonerPlots-1.3.1/src/stonerplots/styles/journals/aip.mplstyle`

 * *Files identical despite different names*

### Comparing `StonerPlots-1.3.0/src/stonerplots/styles/journals/aps.mplstyle` & `StonerPlots-1.3.1/src/stonerplots/styles/journals/aps.mplstyle`

 * *Files identical despite different names*

### Comparing `StonerPlots-1.3.0/src/stonerplots/styles/journals/iop.mplstyle` & `StonerPlots-1.3.1/src/stonerplots/styles/journals/iop.mplstyle`

 * *Files identical despite different names*

### Comparing `StonerPlots-1.3.0/src/stonerplots/styles/journals/nature.mplstyle` & `StonerPlots-1.3.1/src/stonerplots/styles/journals/nature.mplstyle`

 * *Files identical despite different names*

### Comparing `StonerPlots-1.3.0/src/stonerplots/styles/notebook.mplstyle` & `StonerPlots-1.3.1/src/stonerplots/styles/notebook.mplstyle`

 * *Files identical despite different names*

### Comparing `StonerPlots-1.3.0/src/stonerplots/styles/poster.mplstyle` & `StonerPlots-1.3.1/src/stonerplots/styles/poster.mplstyle`

 * *Files identical despite different names*

### Comparing `StonerPlots-1.3.0/src/stonerplots/styles/presentation.mplstyle` & `StonerPlots-1.3.1/src/stonerplots/styles/presentation.mplstyle`

 * *Files identical despite different names*

### Comparing `StonerPlots-1.3.0/src/stonerplots/styles/stoner.mplstyle` & `StonerPlots-1.3.1/src/stonerplots/styles/stoner.mplstyle`

 * *Files identical despite different names*

