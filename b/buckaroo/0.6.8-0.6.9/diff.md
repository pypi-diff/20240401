# Comparing `tmp/buckaroo-0.6.8.tar.gz` & `tmp/buckaroo-0.6.9.tar.gz`

## Comparing `buckaroo-0.6.8.tar` & `buckaroo-0.6.9.tar`

### file list

```diff
@@ -1,165 +1,165 @@
--rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 buckaroo-0.6.8/.bumpversion.cfg
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 buckaroo-0.6.8/.coveragerc
--rw-r--r--   0        0        0     7520 2020-02-02 00:00:00.000000 buckaroo-0.6.8/RELEASE.md
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 buckaroo-0.6.8/babel.config.js
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 buckaroo-0.6.8/buckaroo.json
--rwxr-xr-x   0        0        0      251 2020-02-02 00:00:00.000000 buckaroo-0.6.8/full_build.sh
--rw-r--r--   0        0        0    10026 2020-02-02 00:00:00.000000 buckaroo-0.6.8/introduction.ipynb
--rw-r--r--   0        0        0   618201 2020-02-02 00:00:00.000000 buckaroo-0.6.8/package-lock.json
--rw-r--r--   0        0        0     5779 2020-02-02 00:00:00.000000 buckaroo-0.6.8/package.json
--rw-r--r--   0        0        0   151557 2020-02-02 00:00:00.000000 buckaroo-0.6.8/regular-summary-stats.ipynb
--rw-r--r--   0        0        0     8433 2020-02-02 00:00:00.000000 buckaroo-0.6.8/requirements-ui-test.txt
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 buckaroo-0.6.8/setup.py
--rw-r--r--   0        0        0     4479 2020-02-02 00:00:00.000000 buckaroo-0.6.8/tryit.ipynb
--rw-r--r--   0        0        0      864 2020-02-02 00:00:00.000000 buckaroo-0.6.8/tsconfig.json
--rw-r--r--   0        0        0     4725 2020-02-02 00:00:00.000000 buckaroo-0.6.8/webpack-local-dev.config.js
--rw-r--r--   0        0        0     4673 2020-02-02 00:00:00.000000 buckaroo-0.6.8/webpack.config.js
--rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 buckaroo-0.6.8/webpack.lab.config.js
--rw-r--r--   0        0        0   382555 2020-02-02 00:00:00.000000 buckaroo-0.6.8/yarn.lock
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 buckaroo-0.6.8/.yarn/cache/.gitignore
--rw-r--r--   0        0        0     4092 2020-02-02 00:00:00.000000 buckaroo-0.6.8/buckaroo/__init__.py
--rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 buckaroo-0.6.8/buckaroo/_frontend.py
--rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 buckaroo-0.6.8/buckaroo/_version.py
--rw-r--r--   0        0        0     6074 2020-02-02 00:00:00.000000 buckaroo-0.6.8/buckaroo/buckaroo_widget.py
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 buckaroo-0.6.8/buckaroo/channeldata.json
--rw-r--r--   0        0        0     2569 2020-02-02 00:00:00.000000 buckaroo-0.6.8/buckaroo/geopandas_buckaroo.py
--rw-r--r--   0        0        0     3011 2020-02-02 00:00:00.000000 buckaroo-0.6.8/buckaroo/polars_buckaroo.py
--rw-r--r--   0        0        0     2827 2020-02-02 00:00:00.000000 buckaroo-0.6.8/buckaroo/serialization_utils.py
--rw-r--r--   0        0        0     3337 2020-02-02 00:00:00.000000 buckaroo-0.6.8/buckaroo/solara_buckaroo.py
--rw-r--r--   0        0        0     1894 2020-02-02 00:00:00.000000 buckaroo-0.6.8/buckaroo/trait_utils.py
--rw-r--r--   0        0        0     4575 2020-02-02 00:00:00.000000 buckaroo-0.6.8/buckaroo/widget_utils.py
--rw-r--r--   0        0        0     7941 2020-02-02 00:00:00.000000 buckaroo-0.6.8/buckaroo/auto_clean/auto_clean.py
--rw-r--r--   0        0        0     3267 2020-02-02 00:00:00.000000 buckaroo-0.6.8/buckaroo/auto_clean/cleaning_commands.py
--rw-r--r--   0        0        0     5247 2020-02-02 00:00:00.000000 buckaroo-0.6.8/buckaroo/customizations/all_transforms.py
--rw-r--r--   0        0        0     4540 2020-02-02 00:00:00.000000 buckaroo-0.6.8/buckaroo/customizations/analysis.py
--rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 buckaroo-0.6.8/buckaroo/customizations/analysis_utils.py
--rw-r--r--   0        0        0     1130 2020-02-02 00:00:00.000000 buckaroo-0.6.8/buckaroo/customizations/down_sample.py
--rw-r--r--   0        0        0     5165 2020-02-02 00:00:00.000000 buckaroo-0.6.8/buckaroo/customizations/histogram.py
--rw-r--r--   0        0        0     3172 2020-02-02 00:00:00.000000 buckaroo-0.6.8/buckaroo/customizations/order_columns.py
--rw-r--r--   0        0        0    10235 2020-02-02 00:00:00.000000 buckaroo-0.6.8/buckaroo/customizations/polars_analysis.py
--rw-r--r--   0        0        0     3844 2020-02-02 00:00:00.000000 buckaroo-0.6.8/buckaroo/customizations/polars_commands.py
--rw-r--r--   0        0        0     1906 2020-02-02 00:00:00.000000 buckaroo-0.6.8/buckaroo/customizations/styling.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 buckaroo-0.6.8/buckaroo/dataflow/__init__.py
--rw-r--r--   0        0        0     5852 2020-02-02 00:00:00.000000 buckaroo-0.6.8/buckaroo/dataflow/autocleaning.py
--rw-r--r--   0        0        0    13551 2020-02-02 00:00:00.000000 buckaroo-0.6.8/buckaroo/dataflow/dataflow.py
--rw-r--r--   0        0        0     5643 2020-02-02 00:00:00.000000 buckaroo-0.6.8/buckaroo/dataflow/dataflow_extras.py
--rw-r--r--   0        0        0     4514 2020-02-02 00:00:00.000000 buckaroo-0.6.8/buckaroo/dataflow/widget_extension_utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 buckaroo-0.6.8/buckaroo/jlisp/__init__.py
--rw-r--r--   0        0        0     1747 2020-02-02 00:00:00.000000 buckaroo-0.6.8/buckaroo/jlisp/configure_utils.py
--rw-r--r--   0        0        0     1559 2020-02-02 00:00:00.000000 buckaroo-0.6.8/buckaroo/jlisp/lisp_utils.py
--rw-r--r--   0        0        0    17645 2020-02-02 00:00:00.000000 buckaroo-0.6.8/buckaroo/jlisp/lispy.py
--rw-r--r--   0        0        0     5895 2020-02-02 00:00:00.000000 buckaroo-0.6.8/buckaroo/labextension/package.json
--rw-r--r--   0        0        0    46826 2020-02-02 00:00:00.000000 buckaroo-0.6.8/buckaroo/labextension/static/18.40be33ead1389be68394.js
--rw-r--r--   0        0        0    70387 2020-02-02 00:00:00.000000 buckaroo-0.6.8/buckaroo/labextension/static/399.586608614d3a465dfb90.js
--rw-r--r--   0        0        0   292068 2020-02-02 00:00:00.000000 buckaroo-0.6.8/buckaroo/labextension/static/41.09e9fccd97a3341560a5.js
--rw-r--r--   0        0        0     1153 2020-02-02 00:00:00.000000 buckaroo-0.6.8/buckaroo/labextension/static/480.c21c230d26cf429ef68c.js
--rw-r--r--   0        0        0    70484 2020-02-02 00:00:00.000000 buckaroo-0.6.8/buckaroo/labextension/static/486.f08778dfb765d893ceaf.js
--rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 buckaroo-0.6.8/buckaroo/labextension/static/486.f08778dfb765d893ceaf.js.LICENSE.txt
--rw-r--r--   0        0        0     1384 2020-02-02 00:00:00.000000 buckaroo-0.6.8/buckaroo/labextension/static/568.08b2f45d7f28e0148d85.js
--rw-r--r--   0        0        0  1276641 2020-02-02 00:00:00.000000 buckaroo-0.6.8/buckaroo/labextension/static/731.5261de0881822157e809.js
--rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 buckaroo-0.6.8/buckaroo/labextension/static/731.5261de0881822157e809.js.LICENSE.txt
--rw-r--r--   0        0        0   459203 2020-02-02 00:00:00.000000 buckaroo-0.6.8/buckaroo/labextension/static/823.be2613d32e812b0a22b4.js
--rw-r--r--   0        0        0     3918 2020-02-02 00:00:00.000000 buckaroo-0.6.8/buckaroo/labextension/static/823.be2613d32e812b0a22b4.js.LICENSE.txt
--rw-r--r--   0        0        0   150995 2020-02-02 00:00:00.000000 buckaroo-0.6.8/buckaroo/labextension/static/9.33b37b3e8a5123b77c43.js
--rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 buckaroo-0.6.8/buckaroo/labextension/static/9.33b37b3e8a5123b77c43.js.LICENSE.txt
--rw-r--r--   0        0        0   139612 2020-02-02 00:00:00.000000 buckaroo-0.6.8/buckaroo/labextension/static/935.2832d17fef97c1ec6694.js
--rw-r--r--   0        0        0      721 2020-02-02 00:00:00.000000 buckaroo-0.6.8/buckaroo/labextension/static/935.2832d17fef97c1ec6694.js.LICENSE.txt
--rw-r--r--   0        0        0     8364 2020-02-02 00:00:00.000000 buckaroo-0.6.8/buckaroo/labextension/static/remoteEntry.6688f3e07af8a7a781be.js
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 buckaroo-0.6.8/buckaroo/labextension/static/style.js
--rw-r--r--   0        0        0    41115 2020-02-02 00:00:00.000000 buckaroo-0.6.8/buckaroo/labextension/static/third-party-licenses.json
--rw-r--r--   0        0        0  2509213 2020-02-02 00:00:00.000000 buckaroo-0.6.8/buckaroo/nbextension/index.js
--rw-r--r--   0        0        0     5938 2020-02-02 00:00:00.000000 buckaroo-0.6.8/buckaroo/nbextension/index.js.LICENSE.txt
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 buckaroo-0.6.8/buckaroo/noarch/current_repodata.json
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 buckaroo-0.6.8/buckaroo/noarch/current_repodata.json.bz2
--rw-r--r--   0        0        0     2400 2020-02-02 00:00:00.000000 buckaroo-0.6.8/buckaroo/noarch/index.html
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 buckaroo-0.6.8/buckaroo/noarch/repodata.json
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 buckaroo-0.6.8/buckaroo/noarch/repodata.json.bz2
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 buckaroo-0.6.8/buckaroo/noarch/repodata_from_packages.json
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 buckaroo-0.6.8/buckaroo/noarch/repodata_from_packages.json.bz2
--rw-r--r--   0        0        0     8798 2020-02-02 00:00:00.000000 buckaroo-0.6.8/buckaroo/pluggable_analysis_framework/analysis_management.py
--rw-r--r--   0        0        0     3594 2020-02-02 00:00:00.000000 buckaroo-0.6.8/buckaroo/pluggable_analysis_framework/pluggable_analysis_framework.py
--rw-r--r--   0        0        0     3608 2020-02-02 00:00:00.000000 buckaroo-0.6.8/buckaroo/pluggable_analysis_framework/polars_analysis_management.py
--rw-r--r--   0        0        0      613 2020-02-02 00:00:00.000000 buckaroo-0.6.8/buckaroo/pluggable_analysis_framework/polars_utils.py
--rw-r--r--   0        0        0     3589 2020-02-02 00:00:00.000000 buckaroo-0.6.8/buckaroo/pluggable_analysis_framework/safe_summary_df.py
--rw-r--r--   0        0        0     2378 2020-02-02 00:00:00.000000 buckaroo-0.6.8/buckaroo/pluggable_analysis_framework/utils.py
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 buckaroo-0.6.8/buckaroo/solara/__init__.py
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 buckaroo-0.6.8/docs/Makefile
--rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 buckaroo-0.6.8/docs/make.bat
--rw-r--r--   0        0        0     3740 2020-02-02 00:00:00.000000 buckaroo-0.6.8/docs/webpack.typescript.localdev.ts
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 buckaroo-0.6.8/docs/source/.#conf.py -> paddy@Paddys-Air.hsd1.ma.comcast.net.3481:1710349493
--rw-r--r--   0        0        0     5051 2020-02-02 00:00:00.000000 buckaroo-0.6.8/docs/source/FAQ.rst
--rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 buckaroo-0.6.8/docs/source/conf.py
--rw-r--r--   0        0        0     4119 2020-02-02 00:00:00.000000 buckaroo-0.6.8/docs/source/contributing.rst
--rw-r--r--   0        0        0     2439 2020-02-02 00:00:00.000000 buckaroo-0.6.8/docs/source/feature_reference.rst
--rw-r--r--   0        0        0     1474 2020-02-02 00:00:00.000000 buckaroo-0.6.8/docs/source/index.rst
--rwxr-xr-x   0        0        0      295 2020-02-02 00:00:00.000000 buckaroo-0.6.8/docs/source/install.rst
--rw-r--r--   0        0        0     3419 2020-02-02 00:00:00.000000 buckaroo-0.6.8/docs/source/using.rst
--rw-r--r--   0        0        0   835431 2020-02-02 00:00:00.000000 buckaroo-0.6.8/docs/source/_static/Buckaroo-labled.png
--rw-r--r--   0        0        0    15539 2020-02-02 00:00:00.000000 buckaroo-0.6.8/docs/source/_static/Statusbar.png
--rw-r--r--   0        0        0     5938 2020-02-02 00:00:00.000000 buckaroo-0.6.8/docs/source/_static/embed-bundle.js.LICENSE.txt
--rw-r--r--   0        0        0   305847 2020-02-02 00:00:00.000000 buckaroo-0.6.8/docs/source/_static/histograms-categorical-1.png
--rw-r--r--   0        0        0   276591 2020-02-02 00:00:00.000000 buckaroo-0.6.8/docs/source/_static/histograms-common.png
--rw-r--r--   0        0        0    56452 2020-02-02 00:00:00.000000 buckaroo-0.6.8/docs/source/_static/histograms-numeric.png
--rw-r--r--   0        0        0     2537 2020-02-02 00:00:00.000000 buckaroo-0.6.8/docs/source/articles/auto_clean.rst
--rw-r--r--   0        0        0    11868 2020-02-02 00:00:00.000000 buckaroo-0.6.8/docs/source/articles/data_flow.rst
--rw-r--r--   0        0        0     4123 2020-02-02 00:00:00.000000 buckaroo-0.6.8/docs/source/articles/dataflow.dot
--rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 buckaroo-0.6.8/docs/source/articles/dev-notes.rst
--rw-r--r--   0        0        0     4731 2020-02-02 00:00:00.000000 buckaroo-0.6.8/docs/source/articles/dont-use-df-head-buckaroo-instead.rst
--rw-r--r--   0        0        0     1296 2020-02-02 00:00:00.000000 buckaroo-0.6.8/docs/source/articles/glossary.dot
--rw-r--r--   0        0        0     3394 2020-02-02 00:00:00.000000 buckaroo-0.6.8/docs/source/articles/histograms.rst
--rw-r--r--   0        0        0      568 2020-02-02 00:00:00.000000 buckaroo-0.6.8/docs/source/articles/index.rst
--rw-r--r--   0        0        0     4738 2020-02-02 00:00:00.000000 buckaroo-0.6.8/docs/source/articles/pluggable.rst
--rw-r--r--   0        0        0     3637 2020-02-02 00:00:00.000000 buckaroo-0.6.8/docs/source/articles/related_projects.rst
--rw-r--r--   0        0        0     3368 2020-02-02 00:00:00.000000 buckaroo-0.6.8/docs/source/articles/roadmap.rst
--rw-r--r--   0        0        0     2644 2020-02-02 00:00:00.000000 buckaroo-0.6.8/example-notebooks/DFViewer.ipynb
--rw-r--r--   0        0        0    20333 2020-02-02 00:00:00.000000 buckaroo-0.6.8/example-notebooks/Exception-Traits-demo.ipynb
--rw-r--r--   0        0        0    18116 2020-02-02 00:00:00.000000 buckaroo-0.6.8/example-notebooks/Extending.ipynb
--rw-r--r--   0        0        0    54834 2020-02-02 00:00:00.000000 buckaroo-0.6.8/example-notebooks/Filter.ipynb
--rw-r--r--   0        0        0     8115 2020-02-02 00:00:00.000000 buckaroo-0.6.8/example-notebooks/Full-tour.ipynb
--rw-r--r--   0        0        0     5442 2020-02-02 00:00:00.000000 buckaroo-0.6.8/example-notebooks/GeoPandas.ipynb
--rw-r--r--   0        0        0     6660 2020-02-02 00:00:00.000000 buckaroo-0.6.8/example-notebooks/Histograms-demo.ipynb
--rw-r--r--   0        0        0     6695 2020-02-02 00:00:00.000000 buckaroo-0.6.8/example-notebooks/Itables-testcases.ipynb
--rw-r--r--   0        0        0    12822 2020-02-02 00:00:00.000000 buckaroo-0.6.8/example-notebooks/Pluggable-Analysis-Framework.ipynb
--rw-r--r--   0        0        0     5617 2020-02-02 00:00:00.000000 buckaroo-0.6.8/example-notebooks/Solara-Buckaroo.ipynb
--rw-r--r--   0        0        0    59651 2020-02-02 00:00:00.000000 buckaroo-0.6.8/example-notebooks/styling-gallery.ipynb
--rw-r--r--   0        0        0    19040 2020-02-02 00:00:00.000000 buckaroo-0.6.8/example-notebooks/styling-howto.ipynb
--rw-r--r--   0        0        0     6454 2020-02-02 00:00:00.000000 buckaroo-0.6.8/example-notebooks/testcases-fast.ipynb
--rw-r--r--   0        0        0     4185 2020-02-02 00:00:00.000000 buckaroo-0.6.8/js/dcefwidget.ts
--rw-r--r--   0        0        0      681 2020-02-02 00:00:00.000000 buckaroo-0.6.8/js/extension.ts
--rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 buckaroo-0.6.8/js/index.ts
--rw-r--r--   0        0        0     1268 2020-02-02 00:00:00.000000 buckaroo-0.6.8/js/plugin.ts
--rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 buckaroo-0.6.8/js/version.ts
--rw-r--r--   0        0        0     6430 2020-02-02 00:00:00.000000 buckaroo-0.6.8/js/baked_data/colorMap.ts
--rw-r--r--   0        0        0    17341 2020-02-02 00:00:00.000000 buckaroo-0.6.8/js/baked_data/staticData.ts
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 buckaroo-0.6.8/js/components/ColumnsEditor.tsx
--rw-r--r--   0        0        0     1033 2020-02-02 00:00:00.000000 buckaroo-0.6.8/js/components/CommandUtils.ts
--rw-r--r--   0        0        0     5104 2020-02-02 00:00:00.000000 buckaroo-0.6.8/js/components/DCFCell.tsx
--rw-r--r--   0        0        0     3633 2020-02-02 00:00:00.000000 buckaroo-0.6.8/js/components/DependentTabs.tsx
--rw-r--r--   0        0        0     4881 2020-02-02 00:00:00.000000 buckaroo-0.6.8/js/components/OperationDetail.tsx
--rw-r--r--   0        0        0     1259 2020-02-02 00:00:00.000000 buckaroo-0.6.8/js/components/OperationUtils.ts
--rw-r--r--   0        0        0     6748 2020-02-02 00:00:00.000000 buckaroo-0.6.8/js/components/Operations.tsx
--rw-r--r--   0        0        0     6252 2020-02-02 00:00:00.000000 buckaroo-0.6.8/js/components/StatusBar.tsx
--rw-r--r--   0        0        0     1008 2020-02-02 00:00:00.000000 buckaroo-0.6.8/js/components/WidgetTypes.tsx
--rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 buckaroo-0.6.8/js/components/bakedOperationDefaults.ts
--rw-r--r--   0        0        0     1706 2020-02-02 00:00:00.000000 buckaroo-0.6.8/js/components/utils.ts
--rw-r--r--   0        0        0     5213 2020-02-02 00:00:00.000000 buckaroo-0.6.8/js/components/DFViewerParts/DFViewer.tsx
--rw-r--r--   0        0        0     4779 2020-02-02 00:00:00.000000 buckaroo-0.6.8/js/components/DFViewerParts/DFWhole.ts
--rw-r--r--   0        0        0     6163 2020-02-02 00:00:00.000000 buckaroo-0.6.8/js/components/DFViewerParts/Displayer.ts
--rw-r--r--   0        0        0     7679 2020-02-02 00:00:00.000000 buckaroo-0.6.8/js/components/DFViewerParts/HistogramCell.tsx
--rw-r--r--   0        0        0      522 2020-02-02 00:00:00.000000 buckaroo-0.6.8/js/components/DFViewerParts/SeriesSummaryTooltip.tsx
--rw-r--r--   0        0        0     9532 2020-02-02 00:00:00.000000 buckaroo-0.6.8/js/components/DFViewerParts/gridUtils.ts
--rw-r--r--   0        0        0     3931 2020-02-02 00:00:00.000000 buckaroo-0.6.8/js/style/dcf-npm.css
--rw-r--r--   0        0        0      416 2020-02-02 00:00:00.000000 buckaroo-0.6.8/js/style/icons/arrow-down-short-dark.svg
--rwxr-xr-x   0        0        0      416 2020-02-02 00:00:00.000000 buckaroo-0.6.8/js/style/icons/arrow-down-short.svg
--rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 buckaroo-0.6.8/js/style/icons/arrow-up-short-dark.svg
--rwxr-xr-x   0        0        0      400 2020-02-02 00:00:00.000000 buckaroo-0.6.8/js/style/icons/arrow-up-short.svg
--rwxr-xr-x   0        0        0      349 2020-02-02 00:00:00.000000 buckaroo-0.6.8/js/style/icons/filter-dark.svg
--rwxr-xr-x   0        0        0      349 2020-02-02 00:00:00.000000 buckaroo-0.6.8/js/style/icons/filter.svg
--rw-r--r--   0        0        0     2147 2020-02-02 00:00:00.000000 buckaroo-0.6.8/js/vendor/RechartExtra.ts
--rw-r--r--   0        0        0    10368 2020-02-02 00:00:00.000000 buckaroo-0.6.8/js/vendor/RechartTooltip.tsx
--rw-r--r--   0        0        0  1420117 2020-02-02 00:00:00.000000 buckaroo-0.6.8/static/images/Buckaroo-screenshot.png
--rw-r--r--   0        0        0     2120 2020-02-02 00:00:00.000000 buckaroo-0.6.8/.gitignore
--rw-r--r--   0        0        0     1494 2020-02-02 00:00:00.000000 buckaroo-0.6.8/LICENSE.txt
--rw-r--r--   0        0        0     7247 2020-02-02 00:00:00.000000 buckaroo-0.6.8/README.md
--rw-r--r--   0        0        0     4914 2020-02-02 00:00:00.000000 buckaroo-0.6.8/pyproject.toml
--rw-r--r--   0        0        0    10704 2020-02-02 00:00:00.000000 buckaroo-0.6.8/PKG-INFO
+-rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 buckaroo-0.6.9/.bumpversion.cfg
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 buckaroo-0.6.9/.coveragerc
+-rw-r--r--   0        0        0     7520 2020-02-02 00:00:00.000000 buckaroo-0.6.9/RELEASE.md
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 buckaroo-0.6.9/babel.config.js
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 buckaroo-0.6.9/buckaroo.json
+-rwxr-xr-x   0        0        0      251 2020-02-02 00:00:00.000000 buckaroo-0.6.9/full_build.sh
+-rw-r--r--   0        0        0    10026 2020-02-02 00:00:00.000000 buckaroo-0.6.9/introduction.ipynb
+-rw-r--r--   0        0        0   618201 2020-02-02 00:00:00.000000 buckaroo-0.6.9/package-lock.json
+-rw-r--r--   0        0        0     5779 2020-02-02 00:00:00.000000 buckaroo-0.6.9/package.json
+-rw-r--r--   0        0        0   151557 2020-02-02 00:00:00.000000 buckaroo-0.6.9/regular-summary-stats.ipynb
+-rw-r--r--   0        0        0     8433 2020-02-02 00:00:00.000000 buckaroo-0.6.9/requirements-ui-test.txt
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 buckaroo-0.6.9/setup.py
+-rw-r--r--   0        0        0     4479 2020-02-02 00:00:00.000000 buckaroo-0.6.9/tryit.ipynb
+-rw-r--r--   0        0        0      864 2020-02-02 00:00:00.000000 buckaroo-0.6.9/tsconfig.json
+-rw-r--r--   0        0        0     4725 2020-02-02 00:00:00.000000 buckaroo-0.6.9/webpack-local-dev.config.js
+-rw-r--r--   0        0        0     4673 2020-02-02 00:00:00.000000 buckaroo-0.6.9/webpack.config.js
+-rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 buckaroo-0.6.9/webpack.lab.config.js
+-rw-r--r--   0        0        0   382555 2020-02-02 00:00:00.000000 buckaroo-0.6.9/yarn.lock
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 buckaroo-0.6.9/.yarn/cache/.gitignore
+-rw-r--r--   0        0        0     4092 2020-02-02 00:00:00.000000 buckaroo-0.6.9/buckaroo/__init__.py
+-rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 buckaroo-0.6.9/buckaroo/_frontend.py
+-rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 buckaroo-0.6.9/buckaroo/_version.py
+-rw-r--r--   0        0        0     6074 2020-02-02 00:00:00.000000 buckaroo-0.6.9/buckaroo/buckaroo_widget.py
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 buckaroo-0.6.9/buckaroo/channeldata.json
+-rw-r--r--   0        0        0     2799 2020-02-02 00:00:00.000000 buckaroo-0.6.9/buckaroo/geopandas_buckaroo.py
+-rw-r--r--   0        0        0     3011 2020-02-02 00:00:00.000000 buckaroo-0.6.9/buckaroo/polars_buckaroo.py
+-rw-r--r--   0        0        0     2827 2020-02-02 00:00:00.000000 buckaroo-0.6.9/buckaroo/serialization_utils.py
+-rw-r--r--   0        0        0     3337 2020-02-02 00:00:00.000000 buckaroo-0.6.9/buckaroo/solara_buckaroo.py
+-rw-r--r--   0        0        0     1894 2020-02-02 00:00:00.000000 buckaroo-0.6.9/buckaroo/trait_utils.py
+-rw-r--r--   0        0        0     4575 2020-02-02 00:00:00.000000 buckaroo-0.6.9/buckaroo/widget_utils.py
+-rw-r--r--   0        0        0     7941 2020-02-02 00:00:00.000000 buckaroo-0.6.9/buckaroo/auto_clean/auto_clean.py
+-rw-r--r--   0        0        0     3267 2020-02-02 00:00:00.000000 buckaroo-0.6.9/buckaroo/auto_clean/cleaning_commands.py
+-rw-r--r--   0        0        0     5247 2020-02-02 00:00:00.000000 buckaroo-0.6.9/buckaroo/customizations/all_transforms.py
+-rw-r--r--   0        0        0     4540 2020-02-02 00:00:00.000000 buckaroo-0.6.9/buckaroo/customizations/analysis.py
+-rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 buckaroo-0.6.9/buckaroo/customizations/analysis_utils.py
+-rw-r--r--   0        0        0     1130 2020-02-02 00:00:00.000000 buckaroo-0.6.9/buckaroo/customizations/down_sample.py
+-rw-r--r--   0        0        0     5165 2020-02-02 00:00:00.000000 buckaroo-0.6.9/buckaroo/customizations/histogram.py
+-rw-r--r--   0        0        0     3172 2020-02-02 00:00:00.000000 buckaroo-0.6.9/buckaroo/customizations/order_columns.py
+-rw-r--r--   0        0        0    10235 2020-02-02 00:00:00.000000 buckaroo-0.6.9/buckaroo/customizations/polars_analysis.py
+-rw-r--r--   0        0        0     3844 2020-02-02 00:00:00.000000 buckaroo-0.6.9/buckaroo/customizations/polars_commands.py
+-rw-r--r--   0        0        0     1906 2020-02-02 00:00:00.000000 buckaroo-0.6.9/buckaroo/customizations/styling.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 buckaroo-0.6.9/buckaroo/dataflow/__init__.py
+-rw-r--r--   0        0        0     5852 2020-02-02 00:00:00.000000 buckaroo-0.6.9/buckaroo/dataflow/autocleaning.py
+-rw-r--r--   0        0        0    13551 2020-02-02 00:00:00.000000 buckaroo-0.6.9/buckaroo/dataflow/dataflow.py
+-rw-r--r--   0        0        0     5643 2020-02-02 00:00:00.000000 buckaroo-0.6.9/buckaroo/dataflow/dataflow_extras.py
+-rw-r--r--   0        0        0     4514 2020-02-02 00:00:00.000000 buckaroo-0.6.9/buckaroo/dataflow/widget_extension_utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 buckaroo-0.6.9/buckaroo/jlisp/__init__.py
+-rw-r--r--   0        0        0     1747 2020-02-02 00:00:00.000000 buckaroo-0.6.9/buckaroo/jlisp/configure_utils.py
+-rw-r--r--   0        0        0     1559 2020-02-02 00:00:00.000000 buckaroo-0.6.9/buckaroo/jlisp/lisp_utils.py
+-rw-r--r--   0        0        0    17645 2020-02-02 00:00:00.000000 buckaroo-0.6.9/buckaroo/jlisp/lispy.py
+-rw-r--r--   0        0        0     5895 2020-02-02 00:00:00.000000 buckaroo-0.6.9/buckaroo/labextension/package.json
+-rw-r--r--   0        0        0    46826 2020-02-02 00:00:00.000000 buckaroo-0.6.9/buckaroo/labextension/static/18.40be33ead1389be68394.js
+-rw-r--r--   0        0        0    70663 2020-02-02 00:00:00.000000 buckaroo-0.6.9/buckaroo/labextension/static/399.ecec64ae913f98e003c1.js
+-rw-r--r--   0        0        0   292068 2020-02-02 00:00:00.000000 buckaroo-0.6.9/buckaroo/labextension/static/41.09e9fccd97a3341560a5.js
+-rw-r--r--   0        0        0     1153 2020-02-02 00:00:00.000000 buckaroo-0.6.9/buckaroo/labextension/static/480.c21c230d26cf429ef68c.js
+-rw-r--r--   0        0        0    70484 2020-02-02 00:00:00.000000 buckaroo-0.6.9/buckaroo/labextension/static/486.f08778dfb765d893ceaf.js
+-rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 buckaroo-0.6.9/buckaroo/labextension/static/486.f08778dfb765d893ceaf.js.LICENSE.txt
+-rw-r--r--   0        0        0     1384 2020-02-02 00:00:00.000000 buckaroo-0.6.9/buckaroo/labextension/static/568.08b2f45d7f28e0148d85.js
+-rw-r--r--   0        0        0  1276641 2020-02-02 00:00:00.000000 buckaroo-0.6.9/buckaroo/labextension/static/731.5261de0881822157e809.js
+-rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 buckaroo-0.6.9/buckaroo/labextension/static/731.5261de0881822157e809.js.LICENSE.txt
+-rw-r--r--   0        0        0   459203 2020-02-02 00:00:00.000000 buckaroo-0.6.9/buckaroo/labextension/static/823.be2613d32e812b0a22b4.js
+-rw-r--r--   0        0        0     3918 2020-02-02 00:00:00.000000 buckaroo-0.6.9/buckaroo/labextension/static/823.be2613d32e812b0a22b4.js.LICENSE.txt
+-rw-r--r--   0        0        0   150995 2020-02-02 00:00:00.000000 buckaroo-0.6.9/buckaroo/labextension/static/9.33b37b3e8a5123b77c43.js
+-rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 buckaroo-0.6.9/buckaroo/labextension/static/9.33b37b3e8a5123b77c43.js.LICENSE.txt
+-rw-r--r--   0        0        0   139612 2020-02-02 00:00:00.000000 buckaroo-0.6.9/buckaroo/labextension/static/935.2832d17fef97c1ec6694.js
+-rw-r--r--   0        0        0      721 2020-02-02 00:00:00.000000 buckaroo-0.6.9/buckaroo/labextension/static/935.2832d17fef97c1ec6694.js.LICENSE.txt
+-rw-r--r--   0        0        0     8364 2020-02-02 00:00:00.000000 buckaroo-0.6.9/buckaroo/labextension/static/remoteEntry.5457ee1732d4179e8927.js
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 buckaroo-0.6.9/buckaroo/labextension/static/style.js
+-rw-r--r--   0        0        0    41115 2020-02-02 00:00:00.000000 buckaroo-0.6.9/buckaroo/labextension/static/third-party-licenses.json
+-rw-r--r--   0        0        0  2509489 2020-02-02 00:00:00.000000 buckaroo-0.6.9/buckaroo/nbextension/index.js
+-rw-r--r--   0        0        0     5938 2020-02-02 00:00:00.000000 buckaroo-0.6.9/buckaroo/nbextension/index.js.LICENSE.txt
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 buckaroo-0.6.9/buckaroo/noarch/current_repodata.json
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 buckaroo-0.6.9/buckaroo/noarch/current_repodata.json.bz2
+-rw-r--r--   0        0        0     2400 2020-02-02 00:00:00.000000 buckaroo-0.6.9/buckaroo/noarch/index.html
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 buckaroo-0.6.9/buckaroo/noarch/repodata.json
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 buckaroo-0.6.9/buckaroo/noarch/repodata.json.bz2
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 buckaroo-0.6.9/buckaroo/noarch/repodata_from_packages.json
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 buckaroo-0.6.9/buckaroo/noarch/repodata_from_packages.json.bz2
+-rw-r--r--   0        0        0     8798 2020-02-02 00:00:00.000000 buckaroo-0.6.9/buckaroo/pluggable_analysis_framework/analysis_management.py
+-rw-r--r--   0        0        0     3594 2020-02-02 00:00:00.000000 buckaroo-0.6.9/buckaroo/pluggable_analysis_framework/pluggable_analysis_framework.py
+-rw-r--r--   0        0        0     3608 2020-02-02 00:00:00.000000 buckaroo-0.6.9/buckaroo/pluggable_analysis_framework/polars_analysis_management.py
+-rw-r--r--   0        0        0      613 2020-02-02 00:00:00.000000 buckaroo-0.6.9/buckaroo/pluggable_analysis_framework/polars_utils.py
+-rw-r--r--   0        0        0     3589 2020-02-02 00:00:00.000000 buckaroo-0.6.9/buckaroo/pluggable_analysis_framework/safe_summary_df.py
+-rw-r--r--   0        0        0     2378 2020-02-02 00:00:00.000000 buckaroo-0.6.9/buckaroo/pluggable_analysis_framework/utils.py
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 buckaroo-0.6.9/buckaroo/solara/__init__.py
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 buckaroo-0.6.9/docs/Makefile
+-rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 buckaroo-0.6.9/docs/make.bat
+-rw-r--r--   0        0        0     3740 2020-02-02 00:00:00.000000 buckaroo-0.6.9/docs/webpack.typescript.localdev.ts
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 buckaroo-0.6.9/docs/source/.#conf.py -> paddy@Paddys-Air.hsd1.ma.comcast.net.3481:1710349493
+-rw-r--r--   0        0        0     5051 2020-02-02 00:00:00.000000 buckaroo-0.6.9/docs/source/FAQ.rst
+-rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 buckaroo-0.6.9/docs/source/conf.py
+-rw-r--r--   0        0        0     4119 2020-02-02 00:00:00.000000 buckaroo-0.6.9/docs/source/contributing.rst
+-rw-r--r--   0        0        0     2439 2020-02-02 00:00:00.000000 buckaroo-0.6.9/docs/source/feature_reference.rst
+-rw-r--r--   0        0        0     1474 2020-02-02 00:00:00.000000 buckaroo-0.6.9/docs/source/index.rst
+-rwxr-xr-x   0        0        0      295 2020-02-02 00:00:00.000000 buckaroo-0.6.9/docs/source/install.rst
+-rw-r--r--   0        0        0     3419 2020-02-02 00:00:00.000000 buckaroo-0.6.9/docs/source/using.rst
+-rw-r--r--   0        0        0   835431 2020-02-02 00:00:00.000000 buckaroo-0.6.9/docs/source/_static/Buckaroo-labled.png
+-rw-r--r--   0        0        0    15539 2020-02-02 00:00:00.000000 buckaroo-0.6.9/docs/source/_static/Statusbar.png
+-rw-r--r--   0        0        0     5938 2020-02-02 00:00:00.000000 buckaroo-0.6.9/docs/source/_static/embed-bundle.js.LICENSE.txt
+-rw-r--r--   0        0        0   305847 2020-02-02 00:00:00.000000 buckaroo-0.6.9/docs/source/_static/histograms-categorical-1.png
+-rw-r--r--   0        0        0   276591 2020-02-02 00:00:00.000000 buckaroo-0.6.9/docs/source/_static/histograms-common.png
+-rw-r--r--   0        0        0    56452 2020-02-02 00:00:00.000000 buckaroo-0.6.9/docs/source/_static/histograms-numeric.png
+-rw-r--r--   0        0        0     2537 2020-02-02 00:00:00.000000 buckaroo-0.6.9/docs/source/articles/auto_clean.rst
+-rw-r--r--   0        0        0    11868 2020-02-02 00:00:00.000000 buckaroo-0.6.9/docs/source/articles/data_flow.rst
+-rw-r--r--   0        0        0     4123 2020-02-02 00:00:00.000000 buckaroo-0.6.9/docs/source/articles/dataflow.dot
+-rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 buckaroo-0.6.9/docs/source/articles/dev-notes.rst
+-rw-r--r--   0        0        0     4731 2020-02-02 00:00:00.000000 buckaroo-0.6.9/docs/source/articles/dont-use-df-head-buckaroo-instead.rst
+-rw-r--r--   0        0        0     1296 2020-02-02 00:00:00.000000 buckaroo-0.6.9/docs/source/articles/glossary.dot
+-rw-r--r--   0        0        0     3394 2020-02-02 00:00:00.000000 buckaroo-0.6.9/docs/source/articles/histograms.rst
+-rw-r--r--   0        0        0      568 2020-02-02 00:00:00.000000 buckaroo-0.6.9/docs/source/articles/index.rst
+-rw-r--r--   0        0        0     4738 2020-02-02 00:00:00.000000 buckaroo-0.6.9/docs/source/articles/pluggable.rst
+-rw-r--r--   0        0        0     3637 2020-02-02 00:00:00.000000 buckaroo-0.6.9/docs/source/articles/related_projects.rst
+-rw-r--r--   0        0        0     3368 2020-02-02 00:00:00.000000 buckaroo-0.6.9/docs/source/articles/roadmap.rst
+-rw-r--r--   0        0        0     2644 2020-02-02 00:00:00.000000 buckaroo-0.6.9/example-notebooks/DFViewer.ipynb
+-rw-r--r--   0        0        0    20333 2020-02-02 00:00:00.000000 buckaroo-0.6.9/example-notebooks/Exception-Traits-demo.ipynb
+-rw-r--r--   0        0        0    18116 2020-02-02 00:00:00.000000 buckaroo-0.6.9/example-notebooks/Extending.ipynb
+-rw-r--r--   0        0        0    54834 2020-02-02 00:00:00.000000 buckaroo-0.6.9/example-notebooks/Filter.ipynb
+-rw-r--r--   0        0        0     7964 2020-02-02 00:00:00.000000 buckaroo-0.6.9/example-notebooks/Full-tour.ipynb
+-rw-r--r--   0        0        0     5941 2020-02-02 00:00:00.000000 buckaroo-0.6.9/example-notebooks/GeoPandas.ipynb
+-rw-r--r--   0        0        0     6660 2020-02-02 00:00:00.000000 buckaroo-0.6.9/example-notebooks/Histograms-demo.ipynb
+-rw-r--r--   0        0        0     6695 2020-02-02 00:00:00.000000 buckaroo-0.6.9/example-notebooks/Itables-testcases.ipynb
+-rw-r--r--   0        0        0    12822 2020-02-02 00:00:00.000000 buckaroo-0.6.9/example-notebooks/Pluggable-Analysis-Framework.ipynb
+-rw-r--r--   0        0        0     5617 2020-02-02 00:00:00.000000 buckaroo-0.6.9/example-notebooks/Solara-Buckaroo.ipynb
+-rw-r--r--   0        0        0    59651 2020-02-02 00:00:00.000000 buckaroo-0.6.9/example-notebooks/styling-gallery.ipynb
+-rw-r--r--   0        0        0    19040 2020-02-02 00:00:00.000000 buckaroo-0.6.9/example-notebooks/styling-howto.ipynb
+-rw-r--r--   0        0        0     6454 2020-02-02 00:00:00.000000 buckaroo-0.6.9/example-notebooks/testcases-fast.ipynb
+-rw-r--r--   0        0        0     4185 2020-02-02 00:00:00.000000 buckaroo-0.6.9/js/dcefwidget.ts
+-rw-r--r--   0        0        0      681 2020-02-02 00:00:00.000000 buckaroo-0.6.9/js/extension.ts
+-rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 buckaroo-0.6.9/js/index.ts
+-rw-r--r--   0        0        0     1268 2020-02-02 00:00:00.000000 buckaroo-0.6.9/js/plugin.ts
+-rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 buckaroo-0.6.9/js/version.ts
+-rw-r--r--   0        0        0     6430 2020-02-02 00:00:00.000000 buckaroo-0.6.9/js/baked_data/colorMap.ts
+-rw-r--r--   0        0        0    17341 2020-02-02 00:00:00.000000 buckaroo-0.6.9/js/baked_data/staticData.ts
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 buckaroo-0.6.9/js/components/ColumnsEditor.tsx
+-rw-r--r--   0        0        0     1033 2020-02-02 00:00:00.000000 buckaroo-0.6.9/js/components/CommandUtils.ts
+-rw-r--r--   0        0        0     5104 2020-02-02 00:00:00.000000 buckaroo-0.6.9/js/components/DCFCell.tsx
+-rw-r--r--   0        0        0     3633 2020-02-02 00:00:00.000000 buckaroo-0.6.9/js/components/DependentTabs.tsx
+-rw-r--r--   0        0        0     4881 2020-02-02 00:00:00.000000 buckaroo-0.6.9/js/components/OperationDetail.tsx
+-rw-r--r--   0        0        0     1259 2020-02-02 00:00:00.000000 buckaroo-0.6.9/js/components/OperationUtils.ts
+-rw-r--r--   0        0        0     6748 2020-02-02 00:00:00.000000 buckaroo-0.6.9/js/components/Operations.tsx
+-rw-r--r--   0        0        0     6252 2020-02-02 00:00:00.000000 buckaroo-0.6.9/js/components/StatusBar.tsx
+-rw-r--r--   0        0        0     1008 2020-02-02 00:00:00.000000 buckaroo-0.6.9/js/components/WidgetTypes.tsx
+-rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 buckaroo-0.6.9/js/components/bakedOperationDefaults.ts
+-rw-r--r--   0        0        0     1706 2020-02-02 00:00:00.000000 buckaroo-0.6.9/js/components/utils.ts
+-rw-r--r--   0        0        0     6000 2020-02-02 00:00:00.000000 buckaroo-0.6.9/js/components/DFViewerParts/DFViewer.tsx
+-rw-r--r--   0        0        0     4779 2020-02-02 00:00:00.000000 buckaroo-0.6.9/js/components/DFViewerParts/DFWhole.ts
+-rw-r--r--   0        0        0     6163 2020-02-02 00:00:00.000000 buckaroo-0.6.9/js/components/DFViewerParts/Displayer.ts
+-rw-r--r--   0        0        0     7679 2020-02-02 00:00:00.000000 buckaroo-0.6.9/js/components/DFViewerParts/HistogramCell.tsx
+-rw-r--r--   0        0        0      522 2020-02-02 00:00:00.000000 buckaroo-0.6.9/js/components/DFViewerParts/SeriesSummaryTooltip.tsx
+-rw-r--r--   0        0        0     9532 2020-02-02 00:00:00.000000 buckaroo-0.6.9/js/components/DFViewerParts/gridUtils.ts
+-rw-r--r--   0        0        0     3931 2020-02-02 00:00:00.000000 buckaroo-0.6.9/js/style/dcf-npm.css
+-rw-r--r--   0        0        0      416 2020-02-02 00:00:00.000000 buckaroo-0.6.9/js/style/icons/arrow-down-short-dark.svg
+-rwxr-xr-x   0        0        0      416 2020-02-02 00:00:00.000000 buckaroo-0.6.9/js/style/icons/arrow-down-short.svg
+-rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 buckaroo-0.6.9/js/style/icons/arrow-up-short-dark.svg
+-rwxr-xr-x   0        0        0      400 2020-02-02 00:00:00.000000 buckaroo-0.6.9/js/style/icons/arrow-up-short.svg
+-rwxr-xr-x   0        0        0      349 2020-02-02 00:00:00.000000 buckaroo-0.6.9/js/style/icons/filter-dark.svg
+-rwxr-xr-x   0        0        0      349 2020-02-02 00:00:00.000000 buckaroo-0.6.9/js/style/icons/filter.svg
+-rw-r--r--   0        0        0     2147 2020-02-02 00:00:00.000000 buckaroo-0.6.9/js/vendor/RechartExtra.ts
+-rw-r--r--   0        0        0    10368 2020-02-02 00:00:00.000000 buckaroo-0.6.9/js/vendor/RechartTooltip.tsx
+-rw-r--r--   0        0        0  1420117 2020-02-02 00:00:00.000000 buckaroo-0.6.9/static/images/Buckaroo-screenshot.png
+-rw-r--r--   0        0        0     2120 2020-02-02 00:00:00.000000 buckaroo-0.6.9/.gitignore
+-rw-r--r--   0        0        0     1494 2020-02-02 00:00:00.000000 buckaroo-0.6.9/LICENSE.txt
+-rw-r--r--   0        0        0     7247 2020-02-02 00:00:00.000000 buckaroo-0.6.9/README.md
+-rw-r--r--   0        0        0     4914 2020-02-02 00:00:00.000000 buckaroo-0.6.9/pyproject.toml
+-rw-r--r--   0        0        0    10704 2020-02-02 00:00:00.000000 buckaroo-0.6.9/PKG-INFO
```

### Comparing `buckaroo-0.6.8/RELEASE.md` & `buckaroo-0.6.9/RELEASE.md`

 * *Files identical despite different names*

### Comparing `buckaroo-0.6.8/introduction.ipynb` & `buckaroo-0.6.9/introduction.ipynb`

 * *Files identical despite different names*

### Comparing `buckaroo-0.6.8/package-lock.json` & `buckaroo-0.6.9/package-lock.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.899996015936255%*

 * *Differences: {"'packages'": "{'': {'version': '0.6.9'}}", "'version'": "'0.6.9'"}*

```diff
@@ -72,15 +72,15 @@
                 "url-loader": "^4.1.0",
                 "webpack": "^5",
                 "webpack-cli": "^4.5.0",
                 "webpack-dev-server": "^4.0.0"
             },
             "license": "BSD-3-Clause",
             "name": "buckaroo",
-            "version": "0.6.8"
+            "version": "0.6.9"
         },
         "node_modules/@ampproject/remapping": {
             "dependencies": {
                 "@jridgewell/gen-mapping": "^0.3.0",
                 "@jridgewell/trace-mapping": "^0.3.9"
             },
             "dev": true,
@@ -16783,9 +16783,9 @@
             "integrity": "sha512-rVksvsnNCdJ/ohGc6xgPwyN8eheCxsiLM8mxuE/t/mOVqJewPuO1miLpTHQiRgTKCLexL4MeAFVagts7HmNZ2Q==",
             "license": "MIT",
             "resolved": "https://registry.npmjs.org/yocto-queue/-/yocto-queue-0.1.0.tgz",
             "version": "0.1.0"
         }
     },
     "requires": true,
-    "version": "0.6.8"
+    "version": "0.6.9"
 }
```

### Comparing `buckaroo-0.6.8/package.json` & `buckaroo-0.6.9/package.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.96875%*

 * *Differences: {"'version'": "'0.6.9'"}*

```diff
@@ -173,9 +173,9 @@
         "test": "jest --verbose --passWithNoTests",
         "watch": "npm-run-all -p watch:*",
         "watch:labextension": "jupyter labextension watch .",
         "watch:lib": "tsc -w",
         "watch:nbextension": "webpack --watch"
     },
     "types": "./lib/index.d.ts",
-    "version": "0.6.8"
+    "version": "0.6.9"
 }
```

### Comparing `buckaroo-0.6.8/regular-summary-stats.ipynb` & `buckaroo-0.6.9/regular-summary-stats.ipynb`

 * *Files identical despite different names*

### Comparing `buckaroo-0.6.8/requirements-ui-test.txt` & `buckaroo-0.6.9/requirements-ui-test.txt`

 * *Files identical despite different names*

### Comparing `buckaroo-0.6.8/tryit.ipynb` & `buckaroo-0.6.9/tryit.ipynb`

 * *Files identical despite different names*

### Comparing `buckaroo-0.6.8/tsconfig.json` & `buckaroo-0.6.9/tsconfig.json`

 * *Files identical despite different names*

### Comparing `buckaroo-0.6.8/webpack-local-dev.config.js` & `buckaroo-0.6.9/webpack-local-dev.config.js`

 * *Files identical despite different names*

### Comparing `buckaroo-0.6.8/webpack.config.js` & `buckaroo-0.6.9/webpack.config.js`

 * *Files identical despite different names*

### Comparing `buckaroo-0.6.8/yarn.lock` & `buckaroo-0.6.9/yarn.lock`

 * *Files identical despite different names*

### Comparing `buckaroo-0.6.8/buckaroo/__init__.py` & `buckaroo-0.6.9/buckaroo/__init__.py`

 * *Files identical despite different names*

### Comparing `buckaroo-0.6.8/buckaroo/buckaroo_widget.py` & `buckaroo-0.6.9/buckaroo/buckaroo_widget.py`

 * *Files identical despite different names*

### Comparing `buckaroo-0.6.8/buckaroo/geopandas_buckaroo.py` & `buckaroo-0.6.9/buckaroo/geopandas_buckaroo.py`

 * *Files 3% similar despite different names*

```diff
@@ -49,15 +49,15 @@
 
 class GeoPdSampling(Sampling):
         #pre_limit = 500_000
         #no point in a larger limit until summary stats work for Geopandas
         pre_limit = 2_000
     
 
-class GeopandasBuckarooWidget(buckaroo.BuckarooWidget):
+class GeopandasSVGBuckarooWidget(buckaroo.BuckarooWidget):
     analysis_klasses = [
         TypingStats,
         GeoStyling,
         SvgReprPostProcessing]
 
     sampling_klass = GeoPdSampling
 
@@ -66,7 +66,13 @@
         t_state = self.buckaroo_state.copy()
         t_state['post_processing'] = 'svg_geo'
         self.buckaroo_state = t_state
         
     def _df_to_obj(self, df):
         pd_df = pd.DataFrame(dict(zip(df.columns, df.to_numpy().T)))
         return pd_to_obj(self.sampling_klass.serialize_sample(pd_df))
+
+class GeopandasBuckarooWidget(buckaroo.BuckarooWidget):
+
+    def _df_to_obj(self, df):
+        pd_df = pd.DataFrame(dict(zip(df.columns, df.to_numpy().T)))
+        return pd_to_obj(self.sampling_klass.serialize_sample(pd_df))
```

### Comparing `buckaroo-0.6.8/buckaroo/polars_buckaroo.py` & `buckaroo-0.6.9/buckaroo/polars_buckaroo.py`

 * *Files identical despite different names*

### Comparing `buckaroo-0.6.8/buckaroo/serialization_utils.py` & `buckaroo-0.6.9/buckaroo/serialization_utils.py`

 * *Files identical despite different names*

### Comparing `buckaroo-0.6.8/buckaroo/solara_buckaroo.py` & `buckaroo-0.6.9/buckaroo/solara_buckaroo.py`

 * *Files identical despite different names*

### Comparing `buckaroo-0.6.8/buckaroo/trait_utils.py` & `buckaroo-0.6.9/buckaroo/trait_utils.py`

 * *Files identical despite different names*

### Comparing `buckaroo-0.6.8/buckaroo/widget_utils.py` & `buckaroo-0.6.9/buckaroo/widget_utils.py`

 * *Files identical despite different names*

### Comparing `buckaroo-0.6.8/buckaroo/auto_clean/auto_clean.py` & `buckaroo-0.6.9/buckaroo/auto_clean/auto_clean.py`

 * *Files identical despite different names*

### Comparing `buckaroo-0.6.8/buckaroo/auto_clean/cleaning_commands.py` & `buckaroo-0.6.9/buckaroo/auto_clean/cleaning_commands.py`

 * *Files identical despite different names*

### Comparing `buckaroo-0.6.8/buckaroo/customizations/all_transforms.py` & `buckaroo-0.6.9/buckaroo/customizations/all_transforms.py`

 * *Files identical despite different names*

### Comparing `buckaroo-0.6.8/buckaroo/customizations/analysis.py` & `buckaroo-0.6.9/buckaroo/customizations/analysis.py`

 * *Files identical despite different names*

### Comparing `buckaroo-0.6.8/buckaroo/customizations/down_sample.py` & `buckaroo-0.6.9/buckaroo/customizations/down_sample.py`

 * *Files identical despite different names*

### Comparing `buckaroo-0.6.8/buckaroo/customizations/histogram.py` & `buckaroo-0.6.9/buckaroo/customizations/histogram.py`

 * *Files identical despite different names*

### Comparing `buckaroo-0.6.8/buckaroo/customizations/order_columns.py` & `buckaroo-0.6.9/buckaroo/customizations/order_columns.py`

 * *Files identical despite different names*

### Comparing `buckaroo-0.6.8/buckaroo/customizations/polars_analysis.py` & `buckaroo-0.6.9/buckaroo/customizations/polars_analysis.py`

 * *Files identical despite different names*

### Comparing `buckaroo-0.6.8/buckaroo/customizations/polars_commands.py` & `buckaroo-0.6.9/buckaroo/customizations/polars_commands.py`

 * *Files identical despite different names*

### Comparing `buckaroo-0.6.8/buckaroo/customizations/styling.py` & `buckaroo-0.6.9/buckaroo/customizations/styling.py`

 * *Files identical despite different names*

### Comparing `buckaroo-0.6.8/buckaroo/dataflow/autocleaning.py` & `buckaroo-0.6.9/buckaroo/dataflow/autocleaning.py`

 * *Files identical despite different names*

### Comparing `buckaroo-0.6.8/buckaroo/dataflow/dataflow.py` & `buckaroo-0.6.9/buckaroo/dataflow/dataflow.py`

 * *Files identical despite different names*

### Comparing `buckaroo-0.6.8/buckaroo/dataflow/dataflow_extras.py` & `buckaroo-0.6.9/buckaroo/dataflow/dataflow_extras.py`

 * *Files identical despite different names*

### Comparing `buckaroo-0.6.8/buckaroo/dataflow/widget_extension_utils.py` & `buckaroo-0.6.9/buckaroo/dataflow/widget_extension_utils.py`

 * *Files identical despite different names*

### Comparing `buckaroo-0.6.8/buckaroo/jlisp/configure_utils.py` & `buckaroo-0.6.9/buckaroo/jlisp/configure_utils.py`

 * *Files identical despite different names*

### Comparing `buckaroo-0.6.8/buckaroo/jlisp/lisp_utils.py` & `buckaroo-0.6.9/buckaroo/jlisp/lisp_utils.py`

 * *Files identical despite different names*

### Comparing `buckaroo-0.6.8/buckaroo/jlisp/lispy.py` & `buckaroo-0.6.9/buckaroo/jlisp/lispy.py`

 * *Files identical despite different names*

### Comparing `buckaroo-0.6.8/buckaroo/labextension/package.json` & `buckaroo-0.6.9/buckaroo/labextension/package.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.96796875%*

 * *Differences: {"'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.5457ee1732d4179e8927.js'}}",*

 * * "'version'": "'0.6.9'"}*

```diff
@@ -87,15 +87,15 @@
         "dist/*.png",
         "style/**/*.*"
     ],
     "homepage": "https://github.com/paddymul/buckaroo",
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.6688f3e07af8a7a781be.js"
+            "load": "static/remoteEntry.5457ee1732d4179e8927.js"
         },
         "extension": "lib/plugin",
         "outputDir": "./buckaroo/labextension",
         "sharedPackages": {
             "@jupyter-widgets/base": {
                 "bundled": false,
                 "singleton": true
@@ -177,9 +177,9 @@
         "test": "jest --verbose --passWithNoTests",
         "watch": "npm-run-all -p watch:*",
         "watch:labextension": "jupyter labextension watch .",
         "watch:lib": "tsc -w",
         "watch:nbextension": "webpack --watch"
     },
     "types": "./lib/index.d.ts",
-    "version": "0.6.8"
+    "version": "0.6.9"
 }
```

### Comparing `buckaroo-0.6.8/buckaroo/labextension/static/18.40be33ead1389be68394.js` & `buckaroo-0.6.9/buckaroo/labextension/static/18.40be33ead1389be68394.js`

 * *Files identical despite different names*

### Comparing `buckaroo-0.6.8/buckaroo/labextension/static/399.586608614d3a465dfb90.js` & `buckaroo-0.6.9/buckaroo/labextension/static/399.ecec64ae913f98e003c1.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -999,55 +999,69 @@
                     rowSelection: "single",
                     onRowClicked: e => console.log("A row was clicked"),
                     tooltipShowDelay: 0,
                     onCellClicked: e => {
                         const t = e.column.getColId();
                         void 0 !== r && void 0 !== t && r(t)
                     }
-                }, a.extra_grid_config ? a.extra_grid_config : {}), h = (0, i.useRef)(null), v = a.pinned_rows, w = n ? (0, s.extractPinnedRows)(n, v || []) : [], x = (0, t.heightStyle)(b.length, a.pinned_rows.length, null === (f = null == a ? void 0 : a.extra_grid_config) || void 0 === f ? void 0 : f.rowHeight, null == a ? void 0 : a.component_config);
+                }, a.extra_grid_config ? a.extra_grid_config : {}), h = (0, i.useRef)(null), v = a.pinned_rows, w = n ? (0, s.extractPinnedRows)(n, v || []) : [], x = (0, t.heightStyle)({
+                    numRows: b.length,
+                    pinnedRowLen: a.pinned_rows.length,
+                    location: window.location,
+                    compC: null == a ? void 0 : a.component_config,
+                    rowHeight: null === (f = null == a ? void 0 : a.extra_grid_config) || void 0 === f ? void 0 : f.rowHeight
+                });
                 return i.default.createElement("div", {
                     className: `df-viewer  ${x.classMode} ${x.inIframe}`
                 }, i.default.createElement("div", {
                     style: x.applicableStyle,
                     className: "theme-hanger ag-theme-alpine-dark "
                 }, i.default.createElement(u.AgGridReact, {
                     ref: h,
                     domLayout: x.domLayout,
                     defaultColDef: g,
                     gridOptions: y,
                     rowData: b,
                     pinnedTopRowData: w,
                     columnDefs: d.default.cloneDeep(_),
-                    autoSizeStrategy: (console.log("getAutoSize"), _.length < 1 ? {
+                    autoSizeStrategy: _.length < 1 ? {
                         type: "fitProvidedWidth",
                         width: window.innerWidth - 100
                     } : {
                         type: "fitCellContents"
-                    })
+                    }
                 })))
             }
-            t.DFViewer = p, t.heightStyle = (e, t, a, n) => {
-                const o = window.parent !== window,
-                    l = (null == n ? void 0 : n.dfvHeight) || window.innerHeight / ((null == n ? void 0 : n.height_fraction) || 2),
-                    r = {
-                        height: l
-                    },
-                    i = {
-                        minHeight: 50,
-                        maxHeight: l
+            t.DFViewer = p, t.heightStyle = e => {
+                const {
+                    numRows: t,
+                    pinnedRowLen: a,
+                    location: n,
+                    rowHeight: o,
+                    compC: l
+                } = e, r = -1 !== n.host.indexOf("colab.googleusercontent.com"), i = window.parent !== window, d = window.innerHeight / ((null == l ? void 0 : l.height_fraction) || 2), s = (null == l ? void 0 : l.dfvHeight) || d, c = {
+                    height: s
+                }, u = {
+                    minHeight: 50,
+                    maxHeight: s
+                }, f = t + a < 10, m = (null == l ? void 0 : l.shortMode) || f && void 0 === o;
+                console.log("shortMode", m, "dfvHeight", s, "isGoogleColab", r, "inIframe", i);
+                const p = i ? "inIframe" : "";
+                return r || i ? {
+                    classMode: "regular-mode",
+                    domLayout: "normal",
+                    applicableStyle: {
+                        height: 500
                     },
-                    d = e + t < 10,
-                    s = (null == n ? void 0 : n.shortMode) || d && void 0 === a,
-                    c = (null == n ? void 0 : n.layoutType) || (s ? "autoHeight" : "normal"),
-                    u = s ? i : r;
-                return console.log("shortMode", s, l, o), {
-                    classMode: s ? "short-mode" : "regular-mode",
-                    inIframe: o ? "in-iframe" : "",
-                    domLayout: c,
-                    applicableStyle: u
+                    inIframe: p
+                } : {
+                    classMode: m ? "short-mode" : "regular-mode",
+                    domLayout: (null == l ? void 0 : l.layoutType) || (m ? "autoHeight" : "normal"),
+                    applicableStyle: m ? u : c,
+                    inIframe: p
                 }
             }, t.DFViewerEx = function() {
                 const [e, t] = (0, i.useState)("tripduration");
                 return i.default.createElement(p, {
                     df_data: f.tableDf.data,
                     df_viewer_config: f.tableDf.dfviewer_config,
                     summary_stats_data: f.summaryDfForTableDf,
@@ -2720,11 +2734,11 @@
             o()(l.Z, {
                 insert: "head",
                 singleton: !1
             });
             const r = l.Z.locals || {}
         },
         4147: e => {
-            e.exports = JSON.parse('{"name":"buckaroo","version":"0.6.8","description":"Fast Datagrid widget for the Jupyter Notebook and JupyterLab","keywords":["jupyter","jupyterlab","jupyterlab-extension","widgets"],"files":["lib/**/*.js","lib/**/*.js.map","lib/**/*.ts","dist/*.js","dist/*.js.map","dist/*.png","style/**/*.*"],"homepage":"https://github.com/paddymul/buckaroo","bugs":{"url":"https://github.com/paddymul/buckaroo/issues"},"license":"BSD-3-Clause","author":{"name":"Paddy Mullen","email":""},"main":"lib/index.js","types":"./lib/index.d.ts","repository":{"type":"git","url":"https://github.com/paddymul/buckaroo"},"scripts":{"build":"npm run build:lib && npm run build:nbextension && npm run build:labextension","build-full":"npm run build:lib &&  run build:nbextension && npm run build:labextension","build:dev":"npm run build:lib && npm run build:nbextension && npm run build:labextension:dev","build:labextension":"jupyter labextension build .","build:labextension:dev":"which jupyter && jupyter labextension build --development True .","build:lib":"tsc","build:nbextension":"webpack --mode=production --no-devtool","build:widget-examples":"cd widget-examples/basic && webpack --mode=production","build:examples":"webpack --mode=production --config docs/webpack.typescript.localdev.ts --env production","build:all":"npm run build:labextension && npm run build:nbextension && npm run build:widget-examples","clean":"rimraf dist && npm run clean:lib && npm run clean:labextension && npm run clean:nbextension","clean:lib":"rimraf lib","clean:labextension":"rimraf buckaroo/labextension","clean:nbextension":"rimraf buckaroo/nbextension/index.*","lint":"eslint \'js/**/*.{ts,tsx}\'","lint:check":"eslint \'js/**/*.{ts,tsx}\'","lint:fix":"eslint \'js/**/*.{ts,tsx}\' --fix","prepack":"npm run build:labextension && npm run build:nbextension","test":"jest --verbose --passWithNoTests","watch":"npm-run-all -p watch:*","watch:lib":"tsc -w","watch:nbextension":"webpack --watch","watch:labextension":"jupyter labextension watch .","dev":"webpack-cli serve --config docs/webpack.typescript.localdev.ts  --mode=development --env development --open"},"dependencies":{"@jupyter-widgets/base":"^2 || ^3 || ^4 || ^6.0.0","@jupyterlab/apputils":"^3.0.2","ag-grid-community":"^31.0.3","ag-grid-react":"^31.0.3","lodash":"^4.17.21","react":"^18.0.0","react-dom":"^18.0.0","react-smooth":"^2.0.3","recharts":"^2.7.3"},"devDependencies":{"@babel/cli":"^7.6.3","@babel/core":"^7.6.3","@babel/preset-env":"^7.6.11","@babel/preset-typescript":"7.16.7","@jupyterlab/builder":"^3.0.1","@types/jest":"^28","@types/node":"^10.11.6","@types/react":"^18.0.0","@types/react-dom":"^18.0.0","@types/webpack-dev-server":"^3.11.1","@types/webpack-env":"^1.13.6","@typescript-eslint/eslint-plugin":"^5.9.1","@typescript-eslint/parser":"^5.9.1","acorn":"^6.2.0","babel-jest":"^28","babel-plugin-transform-es2015-modules-commonjs":"^6.26.2","bootstrap":"^5.1.3","css-loader":"^5.0.0","eslint":"^8.6.0","eslint-config-prettier":"^8.3.0","eslint-plugin-prettier":"^4.0.0","eslint-plugin-react":"^7.28.0","eslint-plugin-react-hooks":"^4.3.0","fs-extra":"^7.0.0","fork-ts-checker-webpack-plugin":"^6.1.0","html-loader":"^2.1.2","html-webpack-plugin":"^5.0.0","jest":"^28","lint-staged":"^10.2.11","markdown-loader":"^7.0.0","mkdirp":"^0.5.1","npm-run-all":"^4.1.3","postcss":"^8.4.14","postcss-loader":"^7.0.1","postcss-nested":"^6.0.0","postcss-preset-env":"^7.7.2","prettier":"^2.6.2","prettier-standalone":"^1.3.1-0","prism-themes":"^1.6.0","prismjs":"^1.28.0","react-router":"^6.3.0","react-router-dom":"^5.2.0","react-bootstrap":"^2.0.0","rimraf":"^3.0.2","sass":"^1.53.0","sass-loader":"^13.0.2","source-map-loader":"^0.2.4","style-loader":"^2.0.0","svg-url-loader":"^7.1.1","ts-jest":"^28.0.8","ts-loader":"^8.0.14","ts-node":"^9.1.1","tsconfig-paths-webpack-plugin":"^3.3.0","typescript":"^4.4.3","url-loader":"^4.1.0","webpack":"^5","webpack-cli":"^4.5.0","webpack-dev-server":"^4.0.0"},"jupyterlab":{"extension":"lib/plugin","webpackConfig":"webpack.lab.config.js","outputDir":"./buckaroo/labextension","sharedPackages":{"@jupyter-widgets/base":{"bundled":false,"singleton":true},"@lumino/algorithm":{"bundled":false,"singleton":true},"@lumino/commands":{"bundled":false,"singleton":true},"@lumino/coreutils":{"bundled":false,"singleton":true},"@lumino/datagrid":{"bundled":false,"singleton":true},"@lumino/default-theme":{"bundled":false,"singleton":true},"@lumino/domutils":{"bundled":false,"singleton":true},"@lumino/messaging":{"bundled":false,"singleton":true},"@lumino/virtualdom":{"bundled":false,"singleton":true},"@lumino/widgets":{"bundled":false,"singleton":true},"react":false,"react-dom":false}}}')
+            e.exports = JSON.parse('{"name":"buckaroo","version":"0.6.9","description":"Fast Datagrid widget for the Jupyter Notebook and JupyterLab","keywords":["jupyter","jupyterlab","jupyterlab-extension","widgets"],"files":["lib/**/*.js","lib/**/*.js.map","lib/**/*.ts","dist/*.js","dist/*.js.map","dist/*.png","style/**/*.*"],"homepage":"https://github.com/paddymul/buckaroo","bugs":{"url":"https://github.com/paddymul/buckaroo/issues"},"license":"BSD-3-Clause","author":{"name":"Paddy Mullen","email":""},"main":"lib/index.js","types":"./lib/index.d.ts","repository":{"type":"git","url":"https://github.com/paddymul/buckaroo"},"scripts":{"build":"npm run build:lib && npm run build:nbextension && npm run build:labextension","build-full":"npm run build:lib &&  run build:nbextension && npm run build:labextension","build:dev":"npm run build:lib && npm run build:nbextension && npm run build:labextension:dev","build:labextension":"jupyter labextension build .","build:labextension:dev":"which jupyter && jupyter labextension build --development True .","build:lib":"tsc","build:nbextension":"webpack --mode=production --no-devtool","build:widget-examples":"cd widget-examples/basic && webpack --mode=production","build:examples":"webpack --mode=production --config docs/webpack.typescript.localdev.ts --env production","build:all":"npm run build:labextension && npm run build:nbextension && npm run build:widget-examples","clean":"rimraf dist && npm run clean:lib && npm run clean:labextension && npm run clean:nbextension","clean:lib":"rimraf lib","clean:labextension":"rimraf buckaroo/labextension","clean:nbextension":"rimraf buckaroo/nbextension/index.*","lint":"eslint \'js/**/*.{ts,tsx}\'","lint:check":"eslint \'js/**/*.{ts,tsx}\'","lint:fix":"eslint \'js/**/*.{ts,tsx}\' --fix","prepack":"npm run build:labextension && npm run build:nbextension","test":"jest --verbose --passWithNoTests","watch":"npm-run-all -p watch:*","watch:lib":"tsc -w","watch:nbextension":"webpack --watch","watch:labextension":"jupyter labextension watch .","dev":"webpack-cli serve --config docs/webpack.typescript.localdev.ts  --mode=development --env development --open"},"dependencies":{"@jupyter-widgets/base":"^2 || ^3 || ^4 || ^6.0.0","@jupyterlab/apputils":"^3.0.2","ag-grid-community":"^31.0.3","ag-grid-react":"^31.0.3","lodash":"^4.17.21","react":"^18.0.0","react-dom":"^18.0.0","react-smooth":"^2.0.3","recharts":"^2.7.3"},"devDependencies":{"@babel/cli":"^7.6.3","@babel/core":"^7.6.3","@babel/preset-env":"^7.6.11","@babel/preset-typescript":"7.16.7","@jupyterlab/builder":"^3.0.1","@types/jest":"^28","@types/node":"^10.11.6","@types/react":"^18.0.0","@types/react-dom":"^18.0.0","@types/webpack-dev-server":"^3.11.1","@types/webpack-env":"^1.13.6","@typescript-eslint/eslint-plugin":"^5.9.1","@typescript-eslint/parser":"^5.9.1","acorn":"^6.2.0","babel-jest":"^28","babel-plugin-transform-es2015-modules-commonjs":"^6.26.2","bootstrap":"^5.1.3","css-loader":"^5.0.0","eslint":"^8.6.0","eslint-config-prettier":"^8.3.0","eslint-plugin-prettier":"^4.0.0","eslint-plugin-react":"^7.28.0","eslint-plugin-react-hooks":"^4.3.0","fs-extra":"^7.0.0","fork-ts-checker-webpack-plugin":"^6.1.0","html-loader":"^2.1.2","html-webpack-plugin":"^5.0.0","jest":"^28","lint-staged":"^10.2.11","markdown-loader":"^7.0.0","mkdirp":"^0.5.1","npm-run-all":"^4.1.3","postcss":"^8.4.14","postcss-loader":"^7.0.1","postcss-nested":"^6.0.0","postcss-preset-env":"^7.7.2","prettier":"^2.6.2","prettier-standalone":"^1.3.1-0","prism-themes":"^1.6.0","prismjs":"^1.28.0","react-router":"^6.3.0","react-router-dom":"^5.2.0","react-bootstrap":"^2.0.0","rimraf":"^3.0.2","sass":"^1.53.0","sass-loader":"^13.0.2","source-map-loader":"^0.2.4","style-loader":"^2.0.0","svg-url-loader":"^7.1.1","ts-jest":"^28.0.8","ts-loader":"^8.0.14","ts-node":"^9.1.1","tsconfig-paths-webpack-plugin":"^3.3.0","typescript":"^4.4.3","url-loader":"^4.1.0","webpack":"^5","webpack-cli":"^4.5.0","webpack-dev-server":"^4.0.0"},"jupyterlab":{"extension":"lib/plugin","webpackConfig":"webpack.lab.config.js","outputDir":"./buckaroo/labextension","sharedPackages":{"@jupyter-widgets/base":{"bundled":false,"singleton":true},"@lumino/algorithm":{"bundled":false,"singleton":true},"@lumino/commands":{"bundled":false,"singleton":true},"@lumino/coreutils":{"bundled":false,"singleton":true},"@lumino/datagrid":{"bundled":false,"singleton":true},"@lumino/default-theme":{"bundled":false,"singleton":true},"@lumino/domutils":{"bundled":false,"singleton":true},"@lumino/messaging":{"bundled":false,"singleton":true},"@lumino/virtualdom":{"bundled":false,"singleton":true},"@lumino/widgets":{"bundled":false,"singleton":true},"react":false,"react-dom":false}}}')
         }
     }
 ]);
```

### Comparing `buckaroo-0.6.8/buckaroo/labextension/static/41.09e9fccd97a3341560a5.js` & `buckaroo-0.6.9/buckaroo/labextension/static/41.09e9fccd97a3341560a5.js`

 * *Files identical despite different names*

### Comparing `buckaroo-0.6.8/buckaroo/labextension/static/480.c21c230d26cf429ef68c.js` & `buckaroo-0.6.9/buckaroo/labextension/static/480.c21c230d26cf429ef68c.js`

 * *Files identical despite different names*

### Comparing `buckaroo-0.6.8/buckaroo/labextension/static/486.f08778dfb765d893ceaf.js` & `buckaroo-0.6.9/buckaroo/labextension/static/486.f08778dfb765d893ceaf.js`

 * *Files identical despite different names*

### Comparing `buckaroo-0.6.8/buckaroo/labextension/static/568.08b2f45d7f28e0148d85.js` & `buckaroo-0.6.9/buckaroo/labextension/static/568.08b2f45d7f28e0148d85.js`

 * *Files identical despite different names*

### Comparing `buckaroo-0.6.8/buckaroo/labextension/static/731.5261de0881822157e809.js` & `buckaroo-0.6.9/buckaroo/labextension/static/731.5261de0881822157e809.js`

 * *Files identical despite different names*

### Comparing `buckaroo-0.6.8/buckaroo/labextension/static/823.be2613d32e812b0a22b4.js` & `buckaroo-0.6.9/buckaroo/labextension/static/823.be2613d32e812b0a22b4.js`

 * *Files identical despite different names*

### Comparing `buckaroo-0.6.8/buckaroo/labextension/static/823.be2613d32e812b0a22b4.js.LICENSE.txt` & `buckaroo-0.6.9/buckaroo/labextension/static/823.be2613d32e812b0a22b4.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `buckaroo-0.6.8/buckaroo/labextension/static/9.33b37b3e8a5123b77c43.js` & `buckaroo-0.6.9/buckaroo/labextension/static/9.33b37b3e8a5123b77c43.js`

 * *Files identical despite different names*

### Comparing `buckaroo-0.6.8/buckaroo/labextension/static/9.33b37b3e8a5123b77c43.js.LICENSE.txt` & `buckaroo-0.6.9/buckaroo/labextension/static/9.33b37b3e8a5123b77c43.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `buckaroo-0.6.8/buckaroo/labextension/static/935.2832d17fef97c1ec6694.js` & `buckaroo-0.6.9/buckaroo/labextension/static/935.2832d17fef97c1ec6694.js`

 * *Files identical despite different names*

### Comparing `buckaroo-0.6.8/buckaroo/labextension/static/935.2832d17fef97c1ec6694.js.LICENSE.txt` & `buckaroo-0.6.9/buckaroo/labextension/static/935.2832d17fef97c1ec6694.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `buckaroo-0.6.8/buckaroo/labextension/static/remoteEntry.6688f3e07af8a7a781be.js` & `buckaroo-0.6.9/buckaroo/labextension/static/remoteEntry.5457ee1732d4179e8927.js`

 * *Files 5% similar despite different names*

#### js-beautify {}

```diff
@@ -1,11 +1,11 @@
 var _JUPYTERLAB;
 (() => {
     "use strict";
-    var e, r, t, a, o, n, i, l, u, c, d, f, s, h, p, v, b, m, g, y = {
+    var e, r, t, a, o, n, i, c, l, u, d, s, f, h, p, v, b, m, g, y = {
             5941: (e, r, t) => {
                 var a = {
                         "./index": () => Promise.all([t.e(935), t.e(41), t.e(399), t.e(568)]).then((() => () => t(1568))),
                         "./extension": () => Promise.all([t.e(935), t.e(41), t.e(399), t.e(480)]).then((() => () => t(4480)))
                     },
                     o = (e, r) => (t.R = r, r = t.o(a, e) ? a[e]() : Promise.resolve().then((() => {
                         throw new Error('Module "' + e + '" does not exist in container.')
@@ -47,28 +47,28 @@
             get: r[t]
         })
     }, P.f = {}, P.e = e => Promise.all(Object.keys(P.f).reduce(((r, t) => (P.f[t](e, r), r)), [])), P.u = e => e + "." + {
         9: "33b37b3e8a5123b77c43",
         18: "40be33ead1389be68394",
         41: "09e9fccd97a3341560a5",
         115: "2956041dbe19af089b53",
-        399: "586608614d3a465dfb90",
+        399: "ecec64ae913f98e003c1",
         480: "c21c230d26cf429ef68c",
         486: "f08778dfb765d893ceaf",
         568: "08b2f45d7f28e0148d85",
         731: "5261de0881822157e809",
         809: "1215fc46563d45188e54",
         823: "be2613d32e812b0a22b4",
         935: "2832d17fef97c1ec6694"
     } [e] + ".js?v=" + {
         9: "33b37b3e8a5123b77c43",
         18: "40be33ead1389be68394",
         41: "09e9fccd97a3341560a5",
         115: "2956041dbe19af089b53",
-        399: "586608614d3a465dfb90",
+        399: "ecec64ae913f98e003c1",
         480: "c21c230d26cf429ef68c",
         486: "f08778dfb765d893ceaf",
         568: "08b2f45d7f28e0148d85",
         731: "5261de0881822157e809",
         809: "1215fc46563d45188e54",
         823: "be2613d32e812b0a22b4",
         935: "2832d17fef97c1ec6694"
@@ -78,34 +78,34 @@
             return this || new Function("return this")()
         } catch (e) {
             if ("object" == typeof window) return window
         }
     }(), P.o = (e, r) => Object.prototype.hasOwnProperty.call(e, r), e = {}, r = "buckaroo:", P.l = (t, a, o, n) => {
         if (e[t]) e[t].push(a);
         else {
-            var i, l;
+            var i, c;
             if (void 0 !== o)
-                for (var u = document.getElementsByTagName("script"), c = 0; c < u.length; c++) {
-                    var d = u[c];
+                for (var l = document.getElementsByTagName("script"), u = 0; u < l.length; u++) {
+                    var d = l[u];
                     if (d.getAttribute("src") == t || d.getAttribute("data-webpack") == r + o) {
                         i = d;
                         break
                     }
                 }
-            i || (l = !0, (i = document.createElement("script")).charset = "utf-8", i.timeout = 120, P.nc && i.setAttribute("nonce", P.nc), i.setAttribute("data-webpack", r + o), i.src = t), e[t] = [a];
-            var f = (r, a) => {
-                    i.onerror = i.onload = null, clearTimeout(s);
+            i || (c = !0, (i = document.createElement("script")).charset = "utf-8", i.timeout = 120, P.nc && i.setAttribute("nonce", P.nc), i.setAttribute("data-webpack", r + o), i.src = t), e[t] = [a];
+            var s = (r, a) => {
+                    i.onerror = i.onload = null, clearTimeout(f);
                     var o = e[t];
                     if (delete e[t], i.parentNode && i.parentNode.removeChild(i), o && o.forEach((e => e(a))), r) return r(a)
                 },
-                s = setTimeout(f.bind(null, void 0, {
+                f = setTimeout(s.bind(null, void 0, {
                     type: "timeout",
                     target: i
                 }), 12e4);
-            i.onerror = f.bind(null, i.onerror), i.onload = f.bind(null, i.onload), l && document.head.appendChild(i)
+            i.onerror = s.bind(null, i.onerror), i.onload = s.bind(null, i.onload), c && document.head.appendChild(i)
         }
     }, P.r = e => {
         "undefined" != typeof Symbol && Symbol.toStringTag && Object.defineProperty(e, Symbol.toStringTag, {
             value: "Module"
         }), Object.defineProperty(e, "__esModule", {
             value: !0
         })
@@ -117,25 +117,25 @@
             a || (a = []);
             var o = r[t];
             if (o || (o = r[t] = {}), !(a.indexOf(o) >= 0)) {
                 if (a.push(o), e[t]) return e[t];
                 P.o(P.S, t) || (P.S[t] = {});
                 var n = P.S[t],
                     i = "buckaroo",
-                    l = (e, r, t, a) => {
+                    c = (e, r, t, a) => {
                         var o = n[e] = n[e] || {},
-                            l = o[r];
-                        (!l || !l.loaded && (!a != !l.eager ? a : i > l.from)) && (o[r] = {
+                            c = o[r];
+                        (!c || !c.loaded && (!a != !c.eager ? a : i > c.from)) && (o[r] = {
                             get: t,
                             from: i,
                             eager: !!a
                         })
                     },
-                    u = [];
-                return "default" === t && (l("ag-grid-community", "31.0.3", (() => P.e(731).then((() => () => P(1731))))), l("ag-grid-react", "31.0.3", (() => Promise.all([P.e(935), P.e(9), P.e(115)]).then((() => () => P(7009))))), l("buckaroo", "0.6.8", (() => Promise.all([P.e(935), P.e(41), P.e(399), P.e(568)]).then((() => () => P(1568))))), l("lodash", "4.17.21", (() => P.e(486).then((() => () => P(6486))))), l("react-smooth", "2.0.3", (() => Promise.all([P.e(935), P.e(18)]).then((() => () => P(18))))), l("recharts", "2.7.3", (() => Promise.all([P.e(935), P.e(823), P.e(809)]).then((() => () => P(6823)))))), e[t] = u.length ? Promise.all(u).then((() => e[t] = 1)) : 1
+                    l = [];
+                return "default" === t && (c("ag-grid-community", "31.0.3", (() => P.e(731).then((() => () => P(1731))))), c("ag-grid-react", "31.0.3", (() => Promise.all([P.e(935), P.e(9), P.e(115)]).then((() => () => P(7009))))), c("buckaroo", "0.6.9", (() => Promise.all([P.e(935), P.e(41), P.e(399), P.e(568)]).then((() => () => P(1568))))), c("lodash", "4.17.21", (() => P.e(486).then((() => () => P(6486))))), c("react-smooth", "2.0.3", (() => Promise.all([P.e(935), P.e(18)]).then((() => () => P(18))))), c("recharts", "2.7.3", (() => Promise.all([P.e(935), P.e(823), P.e(809)]).then((() => () => P(6823)))))), e[t] = l.length ? Promise.all(l).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
         P.g.importScripts && (e = P.g.location + "");
         var r = P.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
@@ -154,94 +154,94 @@
         e = t(e), r = t(r);
         for (var a = 0;;) {
             if (a >= e.length) return a < r.length && "u" != (typeof r[a])[0];
             var o = e[a],
                 n = (typeof o)[0];
             if (a >= r.length) return "u" == n;
             var i = r[a],
-                l = (typeof i)[0];
-            if (n != l) return "o" == n && "n" == l || "s" == l || "u" == n;
+                c = (typeof i)[0];
+            if (n != c) return "o" == n && "n" == c || "s" == c || "u" == n;
             if ("o" != n && "u" != n && o != i) return o < i;
             a++
         }
     }, o = e => {
         var r = e[0],
             t = "";
         if (1 === e.length) return "*";
         if (r + .5) {
             t += 0 == r ? ">=" : -1 == r ? "<" : 1 == r ? "^" : 2 == r ? "~" : r > 0 ? "=" : "!=";
-            for (var a = 1, n = 1; n < e.length; n++) a--, t += "u" == (typeof(l = e[n]))[0] ? "-" : (a > 0 ? "." : "") + (a = 2, l);
+            for (var a = 1, n = 1; n < e.length; n++) a--, t += "u" == (typeof(c = e[n]))[0] ? "-" : (a > 0 ? "." : "") + (a = 2, c);
             return t
         }
         var i = [];
         for (n = 1; n < e.length; n++) {
-            var l = e[n];
-            i.push(0 === l ? "not(" + u() + ")" : 1 === l ? "(" + u() + " || " + u() + ")" : 2 === l ? i.pop() + " " + i.pop() : o(l))
+            var c = e[n];
+            i.push(0 === c ? "not(" + l() + ")" : 1 === c ? "(" + l() + " || " + l() + ")" : 2 === c ? i.pop() + " " + i.pop() : o(c))
         }
-        return u();
+        return l();
 
-        function u() {
+        function l() {
             return i.pop().replace(/^\((.+)\)$/, "$1")
         }
     }, n = (e, r) => {
         if (0 in e) {
             r = t(r);
             var a = e[0],
                 o = a < 0;
             o && (a = -a - 1);
-            for (var i = 0, l = 1, u = !0;; l++, i++) {
-                var c, d, f = l < e.length ? (typeof e[l])[0] : "";
-                if (i >= r.length || "o" == (d = (typeof(c = r[i]))[0])) return !u || ("u" == f ? l > a && !o : "" == f != o);
+            for (var i = 0, c = 1, l = !0;; c++, i++) {
+                var u, d, s = c < e.length ? (typeof e[c])[0] : "";
+                if (i >= r.length || "o" == (d = (typeof(u = r[i]))[0])) return !l || ("u" == s ? c > a && !o : "" == s != o);
                 if ("u" == d) {
-                    if (!u || "u" != f) return !1
-                } else if (u)
-                    if (f == d)
-                        if (l <= a) {
-                            if (c != e[l]) return !1
+                    if (!l || "u" != s) return !1
+                } else if (l)
+                    if (s == d)
+                        if (c <= a) {
+                            if (u != e[c]) return !1
                         } else {
-                            if (o ? c > e[l] : c < e[l]) return !1;
-                            c != e[l] && (u = !1)
+                            if (o ? u > e[c] : u < e[c]) return !1;
+                            u != e[c] && (l = !1)
                         }
-                else if ("s" != f && "n" != f) {
-                    if (o || l <= a) return !1;
-                    u = !1, l--
+                else if ("s" != s && "n" != s) {
+                    if (o || c <= a) return !1;
+                    l = !1, c--
                 } else {
-                    if (l <= a || d < f != o) return !1;
-                    u = !1
-                } else "s" != f && "n" != f && (u = !1, l--)
+                    if (c <= a || d < s != o) return !1;
+                    l = !1
+                } else "s" != s && "n" != s && (l = !1, c--)
             }
         }
-        var s = [],
-            h = s.pop.bind(s);
+        var f = [],
+            h = f.pop.bind(f);
         for (i = 1; i < e.length; i++) {
             var p = e[i];
-            s.push(1 == p ? h() | h() : 2 == p ? h() & h() : p ? n(p, r) : !h())
+            f.push(1 == p ? h() | h() : 2 == p ? h() & h() : p ? n(p, r) : !h())
         }
         return !!h()
     }, i = (e, r) => {
         var t = P.S[e];
         if (!t || !P.o(t, r)) throw new Error("Shared module " + r + " doesn't exist in shared scope " + e);
         return t
-    }, l = (e, r) => {
+    }, c = (e, r) => {
         var t = e[r];
         return Object.keys(t).reduce(((e, r) => !e || !t[e].loaded && a(e, r) ? r : e), 0)
-    }, u = (e, r, t, a) => "Unsatisfied version " + t + " from " + (t && e[r][t].from) + " of shared singleton module " + r + " (required " + o(a) + ")", c = (e, r, t, a) => {
-        var o = l(e, t);
-        return n(a, o) || f(u(e, t, o, a)), s(e[t][o])
+    }, l = (e, r, t, a) => "Unsatisfied version " + t + " from " + (t && e[r][t].from) + " of shared singleton module " + r + " (required " + o(a) + ")", u = (e, r, t, a) => {
+        var o = c(e, t);
+        return n(a, o) || s(l(e, t, o, a)), f(e[t][o])
     }, d = (e, r, t) => {
         var o = e[r];
         return (r = Object.keys(o).reduce(((e, r) => !n(t, r) || e && !a(e, r) ? e : r), 0)) && o[r]
-    }, f = e => {
+    }, s = e => {
         "undefined" != typeof console && console.warn && console.warn(e)
-    }, s = e => (e.loaded = 1, e.get()), p = (h = e => function(r, t, a, o) {
+    }, f = e => (e.loaded = 1, e.get()), p = (h = e => function(r, t, a, o) {
         var n = P.I(r);
         return n && n.then ? n.then(e.bind(e, r, P.S[r], t, a, o)) : e(r, P.S[r], t, a, o)
-    })(((e, r, t, a) => (i(e, t), c(r, 0, t, a)))), v = h(((e, r, t, a, o) => {
+    })(((e, r, t, a) => (i(e, t), u(r, 0, t, a)))), v = h(((e, r, t, a, o) => {
         var n = r && P.o(r, t) && d(r, t, a);
-        return n ? s(n) : o()
+        return n ? f(n) : o()
     })), b = {}, m = {
         2492: () => p("default", "@jupyter-widgets/base", [, [1, 6, 0, 0],
             [1, 4],
             [1, 3],
             [1, 2], 1, 1, 1
         ]),
         2661: () => v("default", "react-smooth", [1, 2, 0, 3], (() => P.e(18).then((() => () => P(18))))),
@@ -296,21 +296,21 @@
                             n = t && t.target && t.target.src;
                         i.message = "Loading chunk " + r + " failed.\n(" + o + ": " + n + ")", i.name = "ChunkLoadError", i.type = o, i.request = n, a[1](i)
                     }
                 }), "chunk-" + r, r)
             }
         };
         var r = (r, t) => {
-                var a, o, [n, i, l] = t,
-                    u = 0;
+                var a, o, [n, i, c] = t,
+                    l = 0;
                 if (n.some((r => 0 !== e[r]))) {
                     for (a in i) P.o(i, a) && (P.m[a] = i[a]);
-                    l && l(P)
+                    c && c(P)
                 }
-                for (r && r(t); u < n.length; u++) o = n[u], P.o(e, o) && e[o] && e[o][0](), e[o] = 0
+                for (r && r(t); l < n.length; l++) o = n[l], P.o(e, o) && e[o] && e[o][0](), e[o] = 0
             },
             t = self.webpackChunkbuckaroo = self.webpackChunkbuckaroo || [];
         t.forEach(r.bind(null, 0)), t.push = r.bind(null, t.push.bind(t))
     })(), P.nc = void 0;
     var k = P(5941);
     (_JUPYTERLAB = void 0 === _JUPYTERLAB ? {} : _JUPYTERLAB).buckaroo = k
 })();
```

### Comparing `buckaroo-0.6.8/buckaroo/labextension/static/third-party-licenses.json` & `buckaroo-0.6.9/buckaroo/labextension/static/third-party-licenses.json`

 * *Files identical despite different names*

### Comparing `buckaroo-0.6.8/buckaroo/nbextension/index.js` & `buckaroo-0.6.9/buckaroo/nbextension/index.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -78152,55 +78152,69 @@
                         rowSelection: "single",
                         onRowClicked: e => console.log("A row was clicked"),
                         tooltipShowDelay: 0,
                         onCellClicked: e => {
                             const t = e.column.getColId();
                             void 0 !== a && void 0 !== t && a(t)
                         }
-                    }, n.extra_grid_config ? n.extra_grid_config : {}), w = (0, l.useRef)(null), b = n.pinned_rows, C = r ? (0, c.extractPinnedRows)(r, b || []) : [], S = (0, t.heightStyle)(g.length, n.pinned_rows.length, null === (d = null == n ? void 0 : n.extra_grid_config) || void 0 === d ? void 0 : d.rowHeight, null == n ? void 0 : n.component_config);
+                    }, n.extra_grid_config ? n.extra_grid_config : {}), w = (0, l.useRef)(null), b = n.pinned_rows, C = r ? (0, c.extractPinnedRows)(r, b || []) : [], S = (0, t.heightStyle)({
+                        numRows: g.length,
+                        pinnedRowLen: n.pinned_rows.length,
+                        location: window.location,
+                        compC: null == n ? void 0 : n.component_config,
+                        rowHeight: null === (d = null == n ? void 0 : n.extra_grid_config) || void 0 === d ? void 0 : d.rowHeight
+                    });
                     return l.default.createElement("div", {
                         className: `df-viewer  ${S.classMode} ${S.inIframe}`
                     }, l.default.createElement("div", {
                         style: S.applicableStyle,
                         className: "theme-hanger ag-theme-alpine-dark "
                     }, l.default.createElement(p.AgGridReact, {
                         ref: w,
                         domLayout: S.domLayout,
                         defaultColDef: y,
                         gridOptions: m,
                         rowData: g,
                         pinnedTopRowData: C,
                         columnDefs: s.default.cloneDeep(v),
-                        autoSizeStrategy: (console.log("getAutoSize"), v.length < 1 ? {
+                        autoSizeStrategy: v.length < 1 ? {
                             type: "fitProvidedWidth",
                             width: window.innerWidth - 100
                         } : {
                             type: "fitCellContents"
-                        })
+                        }
                     })))
                 }
-                t.DFViewer = f, t.heightStyle = (e, t, n, r) => {
-                    const o = window.parent !== window,
-                        i = (null == r ? void 0 : r.dfvHeight) || window.innerHeight / ((null == r ? void 0 : r.height_fraction) || 2),
-                        a = {
-                            height: i
-                        },
-                        l = {
-                            minHeight: 50,
-                            maxHeight: i
+                t.DFViewer = f, t.heightStyle = e => {
+                    const {
+                        numRows: t,
+                        pinnedRowLen: n,
+                        location: r,
+                        rowHeight: o,
+                        compC: i
+                    } = e, a = -1 !== r.host.indexOf("colab.googleusercontent.com"), l = window.parent !== window, s = window.innerHeight / ((null == i ? void 0 : i.height_fraction) || 2), c = (null == i ? void 0 : i.dfvHeight) || s, u = {
+                        height: c
+                    }, p = {
+                        minHeight: 50,
+                        maxHeight: c
+                    }, d = t + n < 10, h = (null == i ? void 0 : i.shortMode) || d && void 0 === o;
+                    console.log("shortMode", h, "dfvHeight", c, "isGoogleColab", a, "inIframe", l);
+                    const f = l ? "inIframe" : "";
+                    return a || l ? {
+                        classMode: "regular-mode",
+                        domLayout: "normal",
+                        applicableStyle: {
+                            height: 500
                         },
-                        s = e + t < 10,
-                        c = (null == r ? void 0 : r.shortMode) || s && void 0 === n,
-                        u = (null == r ? void 0 : r.layoutType) || (c ? "autoHeight" : "normal"),
-                        p = c ? l : a;
-                    return console.log("shortMode", c, i, o), {
-                        classMode: c ? "short-mode" : "regular-mode",
-                        inIframe: o ? "in-iframe" : "",
-                        domLayout: u,
-                        applicableStyle: p
+                        inIframe: f
+                    } : {
+                        classMode: h ? "short-mode" : "regular-mode",
+                        domLayout: (null == i ? void 0 : i.layoutType) || (h ? "autoHeight" : "normal"),
+                        applicableStyle: h ? p : u,
+                        inIframe: f
                     }
                 }, t.DFViewerEx = function() {
                     const [e, t] = (0, l.useState)("tripduration");
                     return l.default.createElement(f, {
                         df_data: d.tableDf.data,
                         df_viewer_config: d.tableDf.dfviewer_config,
                         summary_stats_data: d.summaryDfForTableDf,
@@ -79984,15 +79998,15 @@
                     e.exports ? (o.default = o, e.exports = o) : void 0 === (n = function() {
                         return o
                     }.apply(t, [])) || (e.exports = n)
                 }()
             },
             4147: e => {
                 "use strict";
-                e.exports = JSON.parse('{"name":"buckaroo","version":"0.6.8","description":"Fast Datagrid widget for the Jupyter Notebook and JupyterLab","keywords":["jupyter","jupyterlab","jupyterlab-extension","widgets"],"files":["lib/**/*.js","lib/**/*.js.map","lib/**/*.ts","dist/*.js","dist/*.js.map","dist/*.png","style/**/*.*"],"homepage":"https://github.com/paddymul/buckaroo","bugs":{"url":"https://github.com/paddymul/buckaroo/issues"},"license":"BSD-3-Clause","author":{"name":"Paddy Mullen","email":""},"main":"lib/index.js","types":"./lib/index.d.ts","repository":{"type":"git","url":"https://github.com/paddymul/buckaroo"},"scripts":{"build":"npm run build:lib && npm run build:nbextension && npm run build:labextension","build-full":"npm run build:lib &&  run build:nbextension && npm run build:labextension","build:dev":"npm run build:lib && npm run build:nbextension && npm run build:labextension:dev","build:labextension":"jupyter labextension build .","build:labextension:dev":"which jupyter && jupyter labextension build --development True .","build:lib":"tsc","build:nbextension":"webpack --mode=production --no-devtool","build:widget-examples":"cd widget-examples/basic && webpack --mode=production","build:examples":"webpack --mode=production --config docs/webpack.typescript.localdev.ts --env production","build:all":"npm run build:labextension && npm run build:nbextension && npm run build:widget-examples","clean":"rimraf dist && npm run clean:lib && npm run clean:labextension && npm run clean:nbextension","clean:lib":"rimraf lib","clean:labextension":"rimraf buckaroo/labextension","clean:nbextension":"rimraf buckaroo/nbextension/index.*","lint":"eslint \'js/**/*.{ts,tsx}\'","lint:check":"eslint \'js/**/*.{ts,tsx}\'","lint:fix":"eslint \'js/**/*.{ts,tsx}\' --fix","prepack":"npm run build:labextension && npm run build:nbextension","test":"jest --verbose --passWithNoTests","watch":"npm-run-all -p watch:*","watch:lib":"tsc -w","watch:nbextension":"webpack --watch","watch:labextension":"jupyter labextension watch .","dev":"webpack-cli serve --config docs/webpack.typescript.localdev.ts  --mode=development --env development --open"},"dependencies":{"@jupyter-widgets/base":"^2 || ^3 || ^4 || ^6.0.0","@jupyterlab/apputils":"^3.0.2","ag-grid-community":"^31.0.3","ag-grid-react":"^31.0.3","lodash":"^4.17.21","react":"^18.0.0","react-dom":"^18.0.0","react-smooth":"^2.0.3","recharts":"^2.7.3"},"devDependencies":{"@babel/cli":"^7.6.3","@babel/core":"^7.6.3","@babel/preset-env":"^7.6.11","@babel/preset-typescript":"7.16.7","@jupyterlab/builder":"^3.0.1","@types/jest":"^28","@types/node":"^10.11.6","@types/react":"^18.0.0","@types/react-dom":"^18.0.0","@types/webpack-dev-server":"^3.11.1","@types/webpack-env":"^1.13.6","@typescript-eslint/eslint-plugin":"^5.9.1","@typescript-eslint/parser":"^5.9.1","acorn":"^6.2.0","babel-jest":"^28","babel-plugin-transform-es2015-modules-commonjs":"^6.26.2","bootstrap":"^5.1.3","css-loader":"^5.0.0","eslint":"^8.6.0","eslint-config-prettier":"^8.3.0","eslint-plugin-prettier":"^4.0.0","eslint-plugin-react":"^7.28.0","eslint-plugin-react-hooks":"^4.3.0","fs-extra":"^7.0.0","fork-ts-checker-webpack-plugin":"^6.1.0","html-loader":"^2.1.2","html-webpack-plugin":"^5.0.0","jest":"^28","lint-staged":"^10.2.11","markdown-loader":"^7.0.0","mkdirp":"^0.5.1","npm-run-all":"^4.1.3","postcss":"^8.4.14","postcss-loader":"^7.0.1","postcss-nested":"^6.0.0","postcss-preset-env":"^7.7.2","prettier":"^2.6.2","prettier-standalone":"^1.3.1-0","prism-themes":"^1.6.0","prismjs":"^1.28.0","react-router":"^6.3.0","react-router-dom":"^5.2.0","react-bootstrap":"^2.0.0","rimraf":"^3.0.2","sass":"^1.53.0","sass-loader":"^13.0.2","source-map-loader":"^0.2.4","style-loader":"^2.0.0","svg-url-loader":"^7.1.1","ts-jest":"^28.0.8","ts-loader":"^8.0.14","ts-node":"^9.1.1","tsconfig-paths-webpack-plugin":"^3.3.0","typescript":"^4.4.3","url-loader":"^4.1.0","webpack":"^5","webpack-cli":"^4.5.0","webpack-dev-server":"^4.0.0"},"jupyterlab":{"extension":"lib/plugin","webpackConfig":"webpack.lab.config.js","outputDir":"./buckaroo/labextension","sharedPackages":{"@jupyter-widgets/base":{"bundled":false,"singleton":true},"@lumino/algorithm":{"bundled":false,"singleton":true},"@lumino/commands":{"bundled":false,"singleton":true},"@lumino/coreutils":{"bundled":false,"singleton":true},"@lumino/datagrid":{"bundled":false,"singleton":true},"@lumino/default-theme":{"bundled":false,"singleton":true},"@lumino/domutils":{"bundled":false,"singleton":true},"@lumino/messaging":{"bundled":false,"singleton":true},"@lumino/virtualdom":{"bundled":false,"singleton":true},"@lumino/widgets":{"bundled":false,"singleton":true},"react":false,"react-dom":false}}}')
+                e.exports = JSON.parse('{"name":"buckaroo","version":"0.6.9","description":"Fast Datagrid widget for the Jupyter Notebook and JupyterLab","keywords":["jupyter","jupyterlab","jupyterlab-extension","widgets"],"files":["lib/**/*.js","lib/**/*.js.map","lib/**/*.ts","dist/*.js","dist/*.js.map","dist/*.png","style/**/*.*"],"homepage":"https://github.com/paddymul/buckaroo","bugs":{"url":"https://github.com/paddymul/buckaroo/issues"},"license":"BSD-3-Clause","author":{"name":"Paddy Mullen","email":""},"main":"lib/index.js","types":"./lib/index.d.ts","repository":{"type":"git","url":"https://github.com/paddymul/buckaroo"},"scripts":{"build":"npm run build:lib && npm run build:nbextension && npm run build:labextension","build-full":"npm run build:lib &&  run build:nbextension && npm run build:labextension","build:dev":"npm run build:lib && npm run build:nbextension && npm run build:labextension:dev","build:labextension":"jupyter labextension build .","build:labextension:dev":"which jupyter && jupyter labextension build --development True .","build:lib":"tsc","build:nbextension":"webpack --mode=production --no-devtool","build:widget-examples":"cd widget-examples/basic && webpack --mode=production","build:examples":"webpack --mode=production --config docs/webpack.typescript.localdev.ts --env production","build:all":"npm run build:labextension && npm run build:nbextension && npm run build:widget-examples","clean":"rimraf dist && npm run clean:lib && npm run clean:labextension && npm run clean:nbextension","clean:lib":"rimraf lib","clean:labextension":"rimraf buckaroo/labextension","clean:nbextension":"rimraf buckaroo/nbextension/index.*","lint":"eslint \'js/**/*.{ts,tsx}\'","lint:check":"eslint \'js/**/*.{ts,tsx}\'","lint:fix":"eslint \'js/**/*.{ts,tsx}\' --fix","prepack":"npm run build:labextension && npm run build:nbextension","test":"jest --verbose --passWithNoTests","watch":"npm-run-all -p watch:*","watch:lib":"tsc -w","watch:nbextension":"webpack --watch","watch:labextension":"jupyter labextension watch .","dev":"webpack-cli serve --config docs/webpack.typescript.localdev.ts  --mode=development --env development --open"},"dependencies":{"@jupyter-widgets/base":"^2 || ^3 || ^4 || ^6.0.0","@jupyterlab/apputils":"^3.0.2","ag-grid-community":"^31.0.3","ag-grid-react":"^31.0.3","lodash":"^4.17.21","react":"^18.0.0","react-dom":"^18.0.0","react-smooth":"^2.0.3","recharts":"^2.7.3"},"devDependencies":{"@babel/cli":"^7.6.3","@babel/core":"^7.6.3","@babel/preset-env":"^7.6.11","@babel/preset-typescript":"7.16.7","@jupyterlab/builder":"^3.0.1","@types/jest":"^28","@types/node":"^10.11.6","@types/react":"^18.0.0","@types/react-dom":"^18.0.0","@types/webpack-dev-server":"^3.11.1","@types/webpack-env":"^1.13.6","@typescript-eslint/eslint-plugin":"^5.9.1","@typescript-eslint/parser":"^5.9.1","acorn":"^6.2.0","babel-jest":"^28","babel-plugin-transform-es2015-modules-commonjs":"^6.26.2","bootstrap":"^5.1.3","css-loader":"^5.0.0","eslint":"^8.6.0","eslint-config-prettier":"^8.3.0","eslint-plugin-prettier":"^4.0.0","eslint-plugin-react":"^7.28.0","eslint-plugin-react-hooks":"^4.3.0","fs-extra":"^7.0.0","fork-ts-checker-webpack-plugin":"^6.1.0","html-loader":"^2.1.2","html-webpack-plugin":"^5.0.0","jest":"^28","lint-staged":"^10.2.11","markdown-loader":"^7.0.0","mkdirp":"^0.5.1","npm-run-all":"^4.1.3","postcss":"^8.4.14","postcss-loader":"^7.0.1","postcss-nested":"^6.0.0","postcss-preset-env":"^7.7.2","prettier":"^2.6.2","prettier-standalone":"^1.3.1-0","prism-themes":"^1.6.0","prismjs":"^1.28.0","react-router":"^6.3.0","react-router-dom":"^5.2.0","react-bootstrap":"^2.0.0","rimraf":"^3.0.2","sass":"^1.53.0","sass-loader":"^13.0.2","source-map-loader":"^0.2.4","style-loader":"^2.0.0","svg-url-loader":"^7.1.1","ts-jest":"^28.0.8","ts-loader":"^8.0.14","ts-node":"^9.1.1","tsconfig-paths-webpack-plugin":"^3.3.0","typescript":"^4.4.3","url-loader":"^4.1.0","webpack":"^5","webpack-cli":"^4.5.0","webpack-dev-server":"^4.0.0"},"jupyterlab":{"extension":"lib/plugin","webpackConfig":"webpack.lab.config.js","outputDir":"./buckaroo/labextension","sharedPackages":{"@jupyter-widgets/base":{"bundled":false,"singleton":true},"@lumino/algorithm":{"bundled":false,"singleton":true},"@lumino/commands":{"bundled":false,"singleton":true},"@lumino/coreutils":{"bundled":false,"singleton":true},"@lumino/datagrid":{"bundled":false,"singleton":true},"@lumino/default-theme":{"bundled":false,"singleton":true},"@lumino/domutils":{"bundled":false,"singleton":true},"@lumino/messaging":{"bundled":false,"singleton":true},"@lumino/virtualdom":{"bundled":false,"singleton":true},"@lumino/widgets":{"bundled":false,"singleton":true},"react":false,"react-dom":false}}}')
             }
         },
         n = {};
 
     function r(e) {
         var o = n[e];
         if (void 0 !== o) return o.exports;
```

### Comparing `buckaroo-0.6.8/buckaroo/nbextension/index.js.LICENSE.txt` & `buckaroo-0.6.9/buckaroo/nbextension/index.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `buckaroo-0.6.8/buckaroo/noarch/index.html` & `buckaroo-0.6.9/buckaroo/noarch/index.html`

 * *Files identical despite different names*

### Comparing `buckaroo-0.6.8/buckaroo/pluggable_analysis_framework/analysis_management.py` & `buckaroo-0.6.9/buckaroo/pluggable_analysis_framework/analysis_management.py`

 * *Files identical despite different names*

### Comparing `buckaroo-0.6.8/buckaroo/pluggable_analysis_framework/pluggable_analysis_framework.py` & `buckaroo-0.6.9/buckaroo/pluggable_analysis_framework/pluggable_analysis_framework.py`

 * *Files identical despite different names*

### Comparing `buckaroo-0.6.8/buckaroo/pluggable_analysis_framework/polars_analysis_management.py` & `buckaroo-0.6.9/buckaroo/pluggable_analysis_framework/polars_analysis_management.py`

 * *Files identical despite different names*

### Comparing `buckaroo-0.6.8/buckaroo/pluggable_analysis_framework/polars_utils.py` & `buckaroo-0.6.9/buckaroo/pluggable_analysis_framework/polars_utils.py`

 * *Files identical despite different names*

### Comparing `buckaroo-0.6.8/buckaroo/pluggable_analysis_framework/safe_summary_df.py` & `buckaroo-0.6.9/buckaroo/pluggable_analysis_framework/safe_summary_df.py`

 * *Files identical despite different names*

### Comparing `buckaroo-0.6.8/buckaroo/pluggable_analysis_framework/utils.py` & `buckaroo-0.6.9/buckaroo/pluggable_analysis_framework/utils.py`

 * *Files identical despite different names*

### Comparing `buckaroo-0.6.8/docs/Makefile` & `buckaroo-0.6.9/docs/Makefile`

 * *Files identical despite different names*

### Comparing `buckaroo-0.6.8/docs/make.bat` & `buckaroo-0.6.9/docs/make.bat`

 * *Files identical despite different names*

### Comparing `buckaroo-0.6.8/docs/webpack.typescript.localdev.ts` & `buckaroo-0.6.9/docs/webpack.typescript.localdev.ts`

 * *Files identical despite different names*

### Comparing `buckaroo-0.6.8/docs/source/FAQ.rst` & `buckaroo-0.6.9/docs/source/FAQ.rst`

 * *Files identical despite different names*

### Comparing `buckaroo-0.6.8/docs/source/conf.py` & `buckaroo-0.6.9/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `buckaroo-0.6.8/docs/source/contributing.rst` & `buckaroo-0.6.9/docs/source/contributing.rst`

 * *Files identical despite different names*

### Comparing `buckaroo-0.6.8/docs/source/feature_reference.rst` & `buckaroo-0.6.9/docs/source/feature_reference.rst`

 * *Files identical despite different names*

### Comparing `buckaroo-0.6.8/docs/source/index.rst` & `buckaroo-0.6.9/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `buckaroo-0.6.8/docs/source/using.rst` & `buckaroo-0.6.9/docs/source/using.rst`

 * *Files identical despite different names*

### Comparing `buckaroo-0.6.8/docs/source/_static/Buckaroo-labled.png` & `buckaroo-0.6.9/docs/source/_static/Buckaroo-labled.png`

 * *Files identical despite different names*

### Comparing `buckaroo-0.6.8/docs/source/_static/Statusbar.png` & `buckaroo-0.6.9/docs/source/_static/Statusbar.png`

 * *Files identical despite different names*

### Comparing `buckaroo-0.6.8/docs/source/_static/embed-bundle.js.LICENSE.txt` & `buckaroo-0.6.9/docs/source/_static/embed-bundle.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `buckaroo-0.6.8/docs/source/_static/histograms-categorical-1.png` & `buckaroo-0.6.9/docs/source/_static/histograms-categorical-1.png`

 * *Files identical despite different names*

### Comparing `buckaroo-0.6.8/docs/source/_static/histograms-common.png` & `buckaroo-0.6.9/docs/source/_static/histograms-common.png`

 * *Files identical despite different names*

### Comparing `buckaroo-0.6.8/docs/source/_static/histograms-numeric.png` & `buckaroo-0.6.9/docs/source/_static/histograms-numeric.png`

 * *Files identical despite different names*

### Comparing `buckaroo-0.6.8/docs/source/articles/auto_clean.rst` & `buckaroo-0.6.9/docs/source/articles/auto_clean.rst`

 * *Files identical despite different names*

### Comparing `buckaroo-0.6.8/docs/source/articles/data_flow.rst` & `buckaroo-0.6.9/docs/source/articles/data_flow.rst`

 * *Files identical despite different names*

### Comparing `buckaroo-0.6.8/docs/source/articles/dataflow.dot` & `buckaroo-0.6.9/docs/source/articles/dataflow.dot`

 * *Files identical despite different names*

### Comparing `buckaroo-0.6.8/docs/source/articles/dont-use-df-head-buckaroo-instead.rst` & `buckaroo-0.6.9/docs/source/articles/dont-use-df-head-buckaroo-instead.rst`

 * *Files identical despite different names*

### Comparing `buckaroo-0.6.8/docs/source/articles/glossary.dot` & `buckaroo-0.6.9/docs/source/articles/glossary.dot`

 * *Files identical despite different names*

### Comparing `buckaroo-0.6.8/docs/source/articles/histograms.rst` & `buckaroo-0.6.9/docs/source/articles/histograms.rst`

 * *Files identical despite different names*

### Comparing `buckaroo-0.6.8/docs/source/articles/index.rst` & `buckaroo-0.6.9/docs/source/articles/index.rst`

 * *Files identical despite different names*

### Comparing `buckaroo-0.6.8/docs/source/articles/pluggable.rst` & `buckaroo-0.6.9/docs/source/articles/pluggable.rst`

 * *Files identical despite different names*

### Comparing `buckaroo-0.6.8/docs/source/articles/related_projects.rst` & `buckaroo-0.6.9/docs/source/articles/related_projects.rst`

 * *Files identical despite different names*

### Comparing `buckaroo-0.6.8/docs/source/articles/roadmap.rst` & `buckaroo-0.6.9/docs/source/articles/roadmap.rst`

 * *Files identical despite different names*

### Comparing `buckaroo-0.6.8/example-notebooks/DFViewer.ipynb` & `buckaroo-0.6.9/example-notebooks/DFViewer.ipynb`

 * *Files identical despite different names*

### Comparing `buckaroo-0.6.8/example-notebooks/Exception-Traits-demo.ipynb` & `buckaroo-0.6.9/example-notebooks/Exception-Traits-demo.ipynb`

 * *Files identical despite different names*

### Comparing `buckaroo-0.6.8/example-notebooks/Extending.ipynb` & `buckaroo-0.6.9/example-notebooks/Extending.ipynb`

 * *Files identical despite different names*

### Comparing `buckaroo-0.6.8/example-notebooks/Filter.ipynb` & `buckaroo-0.6.9/example-notebooks/Filter.ipynb`

 * *Files identical despite different names*

### Comparing `buckaroo-0.6.8/example-notebooks/Full-tour.ipynb` & `buckaroo-0.6.9/example-notebooks/Full-tour.ipynb`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.993421052631579%*

 * *Differences: {"'cells'": '{delete: [7]}'}*

```diff
@@ -79,25 +79,14 @@
             "source": [
                 "df = pd.read_csv(\"https://github.com/paddymul/buckaroo-data/raw/main/cb_data/2016-04.csv\")\n",
                 "#df = pd.read_parquet(\"https://github.com/paddymul/buckaroo-data/raw/main/cb_data/2016-04.parq\")\n",
                 "df"
             ]
         },
         {
-            "cell_type": "code",
-            "execution_count": null,
-            "metadata": {
-                "tags": []
-            },
-            "outputs": [],
-            "source": [
-                "df[:80]"
-            ]
-        },
-        {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## Histograms\n",
                 "\n",
                 "Histograms are built into Buckaroo.  They enable users to quickly identify distributions of data in columns"
             ]
```

### Comparing `buckaroo-0.6.8/example-notebooks/GeoPandas.ipynb` & `buckaroo-0.6.9/example-notebooks/GeoPandas.ipynb`

 * *Files 9% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9791666666666667%*

 * *Differences: {"'cells'": "{insert: [(3, OrderedDict([('cell_type', 'markdown'), ('id', "*

 * *            "'f6622889-e4a7-4835-90f4-639492052eb5'), ('metadata', OrderedDict()), ('source', ['# "*

 * *            "Use GeopandasSVGBuckarooWidget to see renderings of geometry'])])), (4, "*

 * *            "OrderedDict([('cell_type', 'code'), ('execution_count', None), ('id', "*

 * *            "'6cc1aaea-6add-4b1b-901e-9abacb0425a4'), ('metadata', OrderedDict([('tags', [])])), "*

 * *            "('outputs', []), ('source', ['from buckaroo.geopanda […]*

```diff
@@ -35,14 +35,35 @@
             },
             "outputs": [],
             "source": [
                 "world_df"
             ]
         },
         {
+            "cell_type": "markdown",
+            "id": "f6622889-e4a7-4835-90f4-639492052eb5",
+            "metadata": {},
+            "source": [
+                "# Use GeopandasSVGBuckarooWidget to see renderings of geometry"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "id": "6cc1aaea-6add-4b1b-901e-9abacb0425a4",
+            "metadata": {
+                "tags": []
+            },
+            "outputs": [],
+            "source": [
+                "from buckaroo.geopandas_buckaroo import GeopandasSVGBuckarooWidget\n",
+                "GeopandasSVGBuckarooWidget(world_df)"
+            ]
+        },
+        {
             "cell_type": "code",
             "execution_count": null,
             "id": "dea5fb3e-1e0c-41c0-bbe4-3f4564681665",
             "metadata": {
                 "tags": []
             },
             "outputs": [],
```

### Comparing `buckaroo-0.6.8/example-notebooks/Histograms-demo.ipynb` & `buckaroo-0.6.9/example-notebooks/Histograms-demo.ipynb`

 * *Files identical despite different names*

### Comparing `buckaroo-0.6.8/example-notebooks/Itables-testcases.ipynb` & `buckaroo-0.6.9/example-notebooks/Itables-testcases.ipynb`

 * *Files identical despite different names*

### Comparing `buckaroo-0.6.8/example-notebooks/Pluggable-Analysis-Framework.ipynb` & `buckaroo-0.6.9/example-notebooks/Pluggable-Analysis-Framework.ipynb`

 * *Files identical despite different names*

### Comparing `buckaroo-0.6.8/example-notebooks/Solara-Buckaroo.ipynb` & `buckaroo-0.6.9/example-notebooks/Solara-Buckaroo.ipynb`

 * *Files identical despite different names*

### Comparing `buckaroo-0.6.8/example-notebooks/styling-gallery.ipynb` & `buckaroo-0.6.9/example-notebooks/styling-gallery.ipynb`

 * *Files identical despite different names*

### Comparing `buckaroo-0.6.8/example-notebooks/styling-howto.ipynb` & `buckaroo-0.6.9/example-notebooks/styling-howto.ipynb`

 * *Files identical despite different names*

### Comparing `buckaroo-0.6.8/example-notebooks/testcases-fast.ipynb` & `buckaroo-0.6.9/example-notebooks/testcases-fast.ipynb`

 * *Files identical despite different names*

### Comparing `buckaroo-0.6.8/js/dcefwidget.ts` & `buckaroo-0.6.9/js/dcefwidget.ts`

 * *Files identical despite different names*

### Comparing `buckaroo-0.6.8/js/extension.ts` & `buckaroo-0.6.9/js/extension.ts`

 * *Files identical despite different names*

### Comparing `buckaroo-0.6.8/js/index.ts` & `buckaroo-0.6.9/js/index.ts`

 * *Files identical despite different names*

### Comparing `buckaroo-0.6.8/js/plugin.ts` & `buckaroo-0.6.9/js/plugin.ts`

 * *Files identical despite different names*

### Comparing `buckaroo-0.6.8/js/baked_data/colorMap.ts` & `buckaroo-0.6.9/js/baked_data/colorMap.ts`

 * *Files identical despite different names*

### Comparing `buckaroo-0.6.8/js/baked_data/staticData.ts` & `buckaroo-0.6.9/js/baked_data/staticData.ts`

 * *Files identical despite different names*

### Comparing `buckaroo-0.6.8/js/components/ColumnsEditor.tsx` & `buckaroo-0.6.9/js/components/ColumnsEditor.tsx`

 * *Files identical despite different names*

### Comparing `buckaroo-0.6.8/js/components/CommandUtils.ts` & `buckaroo-0.6.9/js/components/CommandUtils.ts`

 * *Files identical despite different names*

### Comparing `buckaroo-0.6.8/js/components/DCFCell.tsx` & `buckaroo-0.6.9/js/components/DCFCell.tsx`

 * *Files identical despite different names*

### Comparing `buckaroo-0.6.8/js/components/DependentTabs.tsx` & `buckaroo-0.6.9/js/components/DependentTabs.tsx`

 * *Files identical despite different names*

### Comparing `buckaroo-0.6.8/js/components/OperationDetail.tsx` & `buckaroo-0.6.9/js/components/OperationDetail.tsx`

 * *Files identical despite different names*

### Comparing `buckaroo-0.6.8/js/components/OperationUtils.ts` & `buckaroo-0.6.9/js/components/OperationUtils.ts`

 * *Files identical despite different names*

### Comparing `buckaroo-0.6.8/js/components/Operations.tsx` & `buckaroo-0.6.9/js/components/Operations.tsx`

 * *Files identical despite different names*

### Comparing `buckaroo-0.6.8/js/components/StatusBar.tsx` & `buckaroo-0.6.9/js/components/StatusBar.tsx`

 * *Files identical despite different names*

### Comparing `buckaroo-0.6.8/js/components/WidgetTypes.tsx` & `buckaroo-0.6.9/js/components/WidgetTypes.tsx`

 * *Files identical despite different names*

### Comparing `buckaroo-0.6.8/js/components/utils.ts` & `buckaroo-0.6.9/js/components/utils.ts`

 * *Files identical despite different names*

### Comparing `buckaroo-0.6.8/js/components/DFViewerParts/DFViewer.tsx` & `buckaroo-0.6.9/js/components/DFViewerParts/DFViewer.tsx`

 * *Files 13% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import _ from 'lodash';
 import { ComponentConfig, DFData, DFViewerConfig } from './DFWhole';
 
 import { dfToAgrid, extractPinnedRows } from './gridUtils';
 import { replaceAtMatch } from '../utils';
 import { AgGridReact } from 'ag-grid-react'; // the AG Grid React Component
 import {
+  DomLayoutType,
   GridOptions,
   SizeColumnsToContentStrategy,
   SizeColumnsToFitProvidedWidthStrategy,
 } from 'ag-grid-community';
 import { summaryDfForTableDf, tableDf } from '../../baked_data/staticData';
 
 import { getCellRendererSelector } from './gridUtils';
@@ -86,33 +87,32 @@
   const topRowData = summary_stats_data
     ? extractPinnedRows(summary_stats_data, pinned_rows ? pinned_rows : [])
     : [];
 
   const getAutoSize = ():
     | SizeColumnsToFitProvidedWidthStrategy
     | SizeColumnsToContentStrategy => {
-    console.log('getAutoSize');
-
     if (styledColumns.length < 1) {
       return {
         type: 'fitProvidedWidth',
         width: window.innerWidth - 100,
       };
     }
     return {
       type: 'fitCellContents',
     };
   };
 
-  const hs = heightStyle(
-    agData.length,
-    df_viewer_config.pinned_rows.length,
-    df_viewer_config?.extra_grid_config?.rowHeight,
-    df_viewer_config?.component_config
-  );
+  const hs = heightStyle({
+    numRows: agData.length,
+    pinnedRowLen: df_viewer_config.pinned_rows.length,
+    location: window.location,
+    compC: df_viewer_config?.component_config,
+    rowHeight: df_viewer_config?.extra_grid_config?.rowHeight,
+  });
 
   return (
     <div className={`df-viewer  ${hs.classMode} ${hs.inIframe}`}>
       <div
         style={hs.applicableStyle}
         className="theme-hanger ag-theme-alpine-dark "
       >
@@ -127,40 +127,71 @@
           autoSizeStrategy={getAutoSize()}
         ></AgGridReact>
       </div>
     </div>
   );
 }
 
-export const heightStyle = (
-  numRows: number,
-  pinnedRowLen: number,
-  rowHeight?: number,
-  compC?: ComponentConfig
-) => {
+interface HeightStyleArgs {
+  numRows: number;
+  pinnedRowLen: number;
+  readonly location: Location;
+  rowHeight?: number;
+  compC?: ComponentConfig;
+}
+interface HeightStyleI {
+  domLayout: DomLayoutType;
+  inIframe: string;
+  classMode: 'short-mode' | 'regular-mode';
+  applicableStyle: CSSProperties;
+}
+
+export const heightStyle = (hArgs: HeightStyleArgs): HeightStyleI => {
+  const { numRows, pinnedRowLen, location, rowHeight, compC } = hArgs;
+  const isGoogleColab =
+    location.host.indexOf('colab.googleusercontent.com') !== -1;
+
   const inIframe = window.parent !== window;
-  const dfvHeight =
-    compC?.dfvHeight || window.innerHeight / (compC?.height_fraction || 2);
+  const regularCompHeight = window.innerHeight / (compC?.height_fraction || 2);
+  const dfvHeight = compC?.dfvHeight || regularCompHeight;
   const regularDivStyle = { height: dfvHeight };
-
   const shortDivStyle = { minHeight: 50, maxHeight: dfvHeight };
 
-  //   const belowMinRows = agData.length + df_viewer_config.pinned_rows.length < 10;
   const belowMinRows = numRows + pinnedRowLen < 10;
 
   const shortMode =
     compC?.shortMode || (belowMinRows && rowHeight === undefined);
-  const domLayout = compC?.layoutType || (shortMode ? 'autoHeight' : 'normal');
+  console.log(
+    'shortMode',
+    shortMode,
+    'dfvHeight',
+    dfvHeight,
+    'isGoogleColab',
+    isGoogleColab,
+    'inIframe',
+    inIframe
+  );
+  const inIframeClass = inIframe ? 'inIframe' : '';
+  if (isGoogleColab || inIframe) {
+    return {
+      classMode: 'regular-mode',
+      domLayout: 'normal',
+      applicableStyle: { height: 500 },
+      inIframe: inIframeClass,
+    };
+  }
+  const domLayout: DomLayoutType =
+    compC?.layoutType || (shortMode ? 'autoHeight' : 'normal');
   const applicableStyle = shortMode ? shortDivStyle : regularDivStyle;
-  console.log('shortMode', shortMode, dfvHeight, inIframe);
+  const classMode = shortMode ? 'short-mode' : 'regular-mode';
   return {
-    classMode: shortMode ? 'short-mode' : 'regular-mode',
-    inIframe: inIframe ? 'in-iframe' : '',
+    classMode,
     domLayout,
     applicableStyle,
+    inIframe: inIframeClass,
   };
 
   /*
   ab = window.location.host;
  "cskfus796ts-496ff2e9c6d22116-0-colab.googleusercontent.com"
  bc = window.location.pathname
  "/outputframe.html"
```

### Comparing `buckaroo-0.6.8/js/components/DFViewerParts/DFWhole.ts` & `buckaroo-0.6.9/js/components/DFViewerParts/DFWhole.ts`

 * *Files identical despite different names*

### Comparing `buckaroo-0.6.8/js/components/DFViewerParts/Displayer.ts` & `buckaroo-0.6.9/js/components/DFViewerParts/Displayer.ts`

 * *Files identical despite different names*

### Comparing `buckaroo-0.6.8/js/components/DFViewerParts/HistogramCell.tsx` & `buckaroo-0.6.9/js/components/DFViewerParts/HistogramCell.tsx`

 * *Files identical despite different names*

### Comparing `buckaroo-0.6.8/js/components/DFViewerParts/SeriesSummaryTooltip.tsx` & `buckaroo-0.6.9/js/components/DFViewerParts/SeriesSummaryTooltip.tsx`

 * *Files identical despite different names*

### Comparing `buckaroo-0.6.8/js/components/DFViewerParts/gridUtils.ts` & `buckaroo-0.6.9/js/components/DFViewerParts/gridUtils.ts`

 * *Files identical despite different names*

### Comparing `buckaroo-0.6.8/js/style/dcf-npm.css` & `buckaroo-0.6.9/js/style/dcf-npm.css`

 * *Files identical despite different names*

### Comparing `buckaroo-0.6.8/js/vendor/RechartExtra.ts` & `buckaroo-0.6.9/js/vendor/RechartExtra.ts`

 * *Files identical despite different names*

### Comparing `buckaroo-0.6.8/js/vendor/RechartTooltip.tsx` & `buckaroo-0.6.9/js/vendor/RechartTooltip.tsx`

 * *Files identical despite different names*

### Comparing `buckaroo-0.6.8/static/images/Buckaroo-screenshot.png` & `buckaroo-0.6.9/static/images/Buckaroo-screenshot.png`

 * *Files identical despite different names*

### Comparing `buckaroo-0.6.8/.gitignore` & `buckaroo-0.6.9/.gitignore`

 * *Files identical despite different names*

### Comparing `buckaroo-0.6.8/LICENSE.txt` & `buckaroo-0.6.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `buckaroo-0.6.8/README.md` & `buckaroo-0.6.9/README.md`

 * *Files identical despite different names*

### Comparing `buckaroo-0.6.8/pyproject.toml` & `buckaroo-0.6.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
 ]
 dependencies = [
     "ipywidgets>=7.6.0,<9",
     "graphlib_backport>=1.0.0"
 ]
-version = "0.6.8"
+version = "0.6.9"
 
 [project.license]
 file = "LICENSE.txt"
 
 [project.optional-dependencies]
 
 test = [
```

### Comparing `buckaroo-0.6.8/PKG-INFO` & `buckaroo-0.6.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: buckaroo
-Version: 0.6.8
+Version: 0.6.9
 Summary: Buckaroo - GUI Data wrangling for pandas
 Project-URL: Homepage, https://github.com/paddymul/buckaroo
 Author: Paddy Mullen
 License: Copyright (c) 2019 Bloomberg
         All rights reserved.
         
         Redistribution and use in source and binary forms, with or without
```

